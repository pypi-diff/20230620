# Comparing `tmp/hrbot-0.1.1.tar.gz` & `tmp/hrbot-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hrbot-0.1.1.tar", max compression
+gzip compressed data, was "hrbot-0.1.2.tar", max compression
```

## Comparing `hrbot-0.1.1.tar` & `hrbot-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      158 2023-06-15 08:01:29.191231 hrbot-0.1.1/hrbot/__init__.py
--rw-r--r--   0        0        0       31 2023-05-18 14:31:32.146814 hrbot-0.1.1/hrbot/bot/__init__.py
--rw-r--r--   0        0        0      988 2023-06-15 08:48:39.851385 hrbot-0.1.1/hrbot/bot/base.py
--rw-r--r--   0        0        0     3138 2023-06-19 05:53:59.271960 hrbot-0.1.1/hrbot/bot/bot.py
--rw-r--r--   0        0        0       59 2023-05-18 14:31:32.138854 hrbot-0.1.1/hrbot/dispatcher/__init__.py
--rw-r--r--   0        0        0     8542 2023-06-19 03:04:48.395643 hrbot-0.1.1/hrbot/dispatcher/__pycache__/dispatсher.cpython-311.pyc
--rw-r--r--   0        0        0     5652 2023-06-19 02:47:45.490439 hrbot-0.1.1/hrbot/dispatcher/dispatсher.py
--rw-r--r--   0        0        0     9361 2023-06-19 02:47:45.478983 hrbot-0.1.1/hrbot/dispatcher/filter.py
--rw-r--r--   0        0        0       30 2023-05-31 10:19:08.115326 hrbot-0.1.1/hrbot/dispatcher/fsm/__init__.py
--rw-r--r--   0        0        0     1972 2023-06-15 09:02:33.436860 hrbot-0.1.1/hrbot/dispatcher/fsm/state.py
--rw-r--r--   0        0        0     4675 2023-06-14 06:55:24.164338 hrbot-0.1.1/hrbot/dispatcher/fsm/storage.py
--rw-r--r--   0        0        0     1337 2023-06-14 07:07:30.601511 hrbot-0.1.1/hrbot/dispatcher/handler.py
--rw-r--r--   0        0        0      284 2023-06-11 09:43:38.740611 hrbot-0.1.1/hrbot/types/__init__.py
--rw-r--r--   0        0        0      402 2023-06-19 02:47:45.500862 hrbot-0.1.1/hrbot/types/handler.py
--rw-r--r--   0        0        0       31 2023-05-14 15:25:08.437975 hrbot-0.1.1/hrbot/types/hr.py
--rw-r--r--   0        0        0        0 2023-05-14 13:14:36.307325 hrbot-0.1.1/hrbot/utils/__init__.py
--rw-r--r--   0        0        0     1084 2023-06-18 13:15:36.011849 hrbot-0.1.1/LICENSE
--rw-r--r--   0        0        0      459 2023-06-19 10:20:38.280823 hrbot-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1612 2023-06-19 07:04:11.369368 hrbot-0.1.1/README.md
--rw-r--r--   0        0        0     2145 1970-01-01 00:00:00.000000 hrbot-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      158 2023-06-15 08:01:29.191231 hrbot-0.1.2/hrbot/__init__.py
+-rw-r--r--   0        0        0       31 2023-05-18 14:31:32.146814 hrbot-0.1.2/hrbot/bot/__init__.py
+-rw-r--r--   0        0        0      988 2023-06-15 08:48:39.851385 hrbot-0.1.2/hrbot/bot/base.py
+-rw-r--r--   0        0        0     3602 2023-06-20 03:58:41.942703 hrbot-0.1.2/hrbot/bot/bot.py
+-rw-r--r--   0        0        0       59 2023-05-18 14:31:32.138854 hrbot-0.1.2/hrbot/dispatcher/__init__.py
+-rw-r--r--   0        0        0     9474 2023-06-20 03:13:28.257902 hrbot-0.1.2/hrbot/dispatcher/__pycache__/dispatсher.cpython-311.pyc
+-rw-r--r--   0        0        0     6343 2023-06-20 03:13:27.988046 hrbot-0.1.2/hrbot/dispatcher/dispatсher.py
+-rw-r--r--   0        0        0    10632 2023-06-20 03:12:45.077146 hrbot-0.1.2/hrbot/dispatcher/filter.py
+-rw-r--r--   0        0        0       30 2023-05-31 10:19:08.115326 hrbot-0.1.2/hrbot/dispatcher/fsm/__init__.py
+-rw-r--r--   0        0        0     1972 2023-06-15 09:02:33.436860 hrbot-0.1.2/hrbot/dispatcher/fsm/state.py
+-rw-r--r--   0        0        0     4675 2023-06-14 06:55:24.164338 hrbot-0.1.2/hrbot/dispatcher/fsm/storage.py
+-rw-r--r--   0        0        0     1337 2023-06-14 07:07:30.601511 hrbot-0.1.2/hrbot/dispatcher/handler.py
+-rw-r--r--   0        0        0      284 2023-06-11 09:43:38.740611 hrbot-0.1.2/hrbot/types/__init__.py
+-rw-r--r--   0        0        0      402 2023-06-19 02:47:45.500862 hrbot-0.1.2/hrbot/types/handler.py
+-rw-r--r--   0        0        0       31 2023-05-14 15:25:08.437975 hrbot-0.1.2/hrbot/types/hr.py
+-rw-r--r--   0        0        0        0 2023-05-14 13:14:36.307325 hrbot-0.1.2/hrbot/utils/__init__.py
+-rw-r--r--   0        0        0     1084 2023-06-18 13:15:36.011849 hrbot-0.1.2/LICENSE
+-rw-r--r--   0        0        0      459 2023-06-20 03:58:41.907078 hrbot-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1612 2023-06-19 07:04:11.369368 hrbot-0.1.2/README.md
+-rw-r--r--   0        0        0     2145 1970-01-01 00:00:00.000000 hrbot-0.1.2/PKG-INFO
```

### Comparing `hrbot-0.1.1/hrbot/bot/base.py` & `hrbot-0.1.2/hrbot/bot/base.py`

 * *Files identical despite different names*

### Comparing `hrbot-0.1.1/hrbot/bot/bot.py` & `hrbot-0.1.2/hrbot/bot/bot.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .base import BaseBot
 from ..types import _bcolors
 from ..types.hr import SessionMetadata, User, Position, AnchorPosition, Reaction, CurrencyItem, Item
-
+from typing import Literal
 
 class Bot(BaseBot):
     @staticmethod
     def __event_handler(func):
         async def wrapper(self, *args, **kwargs):
             event_name = func.__name__
             await func(self, *args, **kwargs)
@@ -79,8 +79,21 @@
 
     @__event_handler
     async def on_user_move(
             self, user: User, destination: Position | AnchorPosition
     ) -> None:
         """On a user moving in the room."""
         pass
-    
+
+    @__event_handler
+    async def on_voice_change(
+        self, users: list[tuple[User, Literal["voice", "muted"]]], seconds_left: int
+    ) -> None:
+        """On a change in voice status in the room."""
+        pass
+
+    @__event_handler
+    async def on_message(
+        self, user_id: str, conversation_id: str, is_new_conversation: bool
+    ) -> None:
+        """On a inbox message received from a user."""
+        pass
```

### Comparing `hrbot-0.1.1/hrbot/dispatcher/__pycache__/dispatсher.cpython-311.pyc` & `hrbot-0.1.2/hrbot/dispatcher/__pycache__/dispatсher.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,21 +1,21 @@
 magic:    0xa70d0d0a
-moddate:  0xd1c18f64 (Mon Jun 19 02:47:45 2023 UTC)
-files sz: 5652
+moddate:  0x57199164 (Tue Jun 20 03:13:27 2023 UTC)
+files sz: 6343
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640264036c026d035a036d
       045a046d055a050100640264046c066d075a076d085a080100640564066c
-      096d025a020100640064076c0a6d0b5a0b010002004700640884006409a6
-      020000ab0200000000000000005a0c02004700640a8400640b650ca60300
-      00ab0300000000000000005a0d64015300
+      096d025a020100640064076c0a6d0b5a0b6d0c5a0c010002004700640884
+      006409a6020000ab0200000000000000005a0d02004700640a8400640b65
+      0da6030000ab0300000000000000005a0e64015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (importlib)
                  8 STORE_NAME               0 (importlib)
    
@@ -48,49 +48,51 @@
                 56 LOAD_CONST               6 (('handler',))
                 58 IMPORT_NAME              9 (types)
                 60 IMPORT_FROM              2 (handler)
                 62 STORE_NAME               2 (handler)
                 64 POP_TOP
    
      7          66 LOAD_CONST               0 (0)
-                68 LOAD_CONST               7 (('Optional',))
+                68 LOAD_CONST               7 (('Optional', 'Literal'))
                 70 IMPORT_NAME             10 (typing)
                 72 IMPORT_FROM             11 (Optional)
                 74 STORE_NAME              11 (Optional)
-                76 POP_TOP
+                76 IMPORT_FROM             12 (Literal)
+                78 STORE_NAME              12 (Literal)
+                80 POP_TOP
    
-    10          78 PUSH_NULL
-                80 LOAD_BUILD_CLASS
-                82 LOAD_CONST               8 (<code object DispatcherEvents, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 10>)
-                84 MAKE_FUNCTION            0
-                86 LOAD_CONST               9 ('DispatcherEvents')
-                88 PRECALL                  2
-                92 CALL                     2
-               102 STORE_NAME              12 (DispatcherEvents)
+    10          82 PUSH_NULL
+                84 LOAD_BUILD_CLASS
+                86 LOAD_CONST               8 (<code object DispatcherEvents, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 10>)
+                88 MAKE_FUNCTION            0
+                90 LOAD_CONST               9 ('DispatcherEvents')
+                92 PRECALL                  2
+                96 CALL                     2
+               106 STORE_NAME              13 (DispatcherEvents)
    
-   133         104 PUSH_NULL
-               106 LOAD_BUILD_CLASS
-               108 LOAD_CONST              10 (<code object Dispatcher, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 133>)
-               110 MAKE_FUNCTION            0
-               112 LOAD_CONST              11 ('Dispatcher')
-               114 LOAD_NAME               12 (DispatcherEvents)
-               116 PRECALL                  3
-               120 CALL                     3
-               130 STORE_NAME              13 (Dispatcher)
-               132 LOAD_CONST               1 (None)
-               134 RETURN_VALUE
+   155         108 PUSH_NULL
+               110 LOAD_BUILD_CLASS
+               112 LOAD_CONST              10 (<code object Dispatcher, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 155>)
+               114 MAKE_FUNCTION            0
+               116 LOAD_CONST              11 ('Dispatcher')
+               118 LOAD_NAME               13 (DispatcherEvents)
+               120 PRECALL                  3
+               124 CALL                     3
+               134 STORE_NAME              14 (Dispatcher)
+               136 LOAD_CONST               1 (None)
+               138 RETURN_VALUE
    consts
       0
       None
       1
       ('HandlerFactory', 'DictWrapper', 'HandlerObj')
       ('filter', 'fsm')
       2
       ('handler',)
-      ('Optional',)
+      ('Optional', 'Literal')
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 18
          flags     : 0
          code
             0x970065005a0164005a02640184005a03640264026402640365046a0500
@@ -119,16 +121,21 @@
             060000000000000000641c65046a120000000000000000640c6508650919
             000000000000000000640d6508650a19000000000000000000660a641d84
             065a136402640264026404641e9c04641f65086509190000000000000000
             00640765046a070000000000000000642065086514650919000000000000
             00000019000000000000000000640d6508650a1900000000000000000066
             08642184065a15640264026402640464229c04640665046a060000000000
             000000642365046a160000000000000000640c6508650919000000000000
-            000000640d6508650a190000000000000000006608642484065a17640253
-            00
+            000000640d6508650a190000000000000000006608642484065a17640264
+            02640464259c0364266518651965046a060000000000000000651a642719
+            000000000000000000660219000000000000000000190000000000000000
+            006428651b640d6508650a190000000000000000006606642984065a1c64
+            026402640264026404642a9c05642b6509642c6509642d650a640c650865
+            0919000000000000000000640d6508650a19000000000000000000660a64
+            2e84065a1d64025300
           10           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('DispatcherEvents')
                        8 STORE_NAME               2 (__qualname__)
          
           11          10 LOAD_CONST               1 (<code object on_start, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 11>)
@@ -537,16 +544,93 @@
                      906 LOAD_NAME               10 (bool)
                      908 BINARY_SUBSCR
          
          121         918 BUILD_TUPLE              8
                      920 LOAD_CONST              36 (<code object on_user_move, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 121>)
                      922 MAKE_FUNCTION            6 (kwdefaults, annotations)
                      924 STORE_NAME              23 (on_user_move)
-                     926 LOAD_CONST               2 (None)
-                     928 RETURN_VALUE
+         
+         134         926 LOAD_CONST               2 (None)
+         
+         135         928 LOAD_CONST               2 (None)
+         
+         136         930 LOAD_CONST               4 (False)
+         
+         132         932 LOAD_CONST              37 (('users', 'seconds_left', 'go_on'))
+                     934 BUILD_CONST_KEY_MAP      3
+                     936 LOAD_CONST              38 ('users')
+         
+         134         938 LOAD_NAME               24 (list)
+                     940 LOAD_NAME               25 (tuple)
+                     942 LOAD_NAME                4 (handler)
+                     944 LOAD_ATTR                6 (User)
+                     954 LOAD_NAME               26 (Literal)
+                     956 LOAD_CONST              39 (('voice', 'muted'))
+                     958 BINARY_SUBSCR
+                     968 BUILD_TUPLE              2
+                     970 BINARY_SUBSCR
+                     980 BINARY_SUBSCR
+         
+         132         990 LOAD_CONST              40 ('seconds_left')
+         
+         135         992 LOAD_NAME               27 (int)
+         
+         132         994 LOAD_CONST              13 ('go_on')
+         
+         136         996 LOAD_NAME                8 (Optional)
+                     998 LOAD_NAME               10 (bool)
+                    1000 BINARY_SUBSCR
+         
+         132        1010 BUILD_TUPLE              6
+                    1012 LOAD_CONST              41 (<code object on_voice_change, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 132>)
+                    1014 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                    1016 STORE_NAME              28 (on_voice_change)
+         
+         144        1018 LOAD_CONST               2 (None)
+         
+         145        1020 LOAD_CONST               2 (None)
+         
+         146        1022 LOAD_CONST               2 (None)
+         
+         147        1024 LOAD_CONST               2 (None)
+         
+         148        1026 LOAD_CONST               4 (False)
+         
+         142        1028 LOAD_CONST              42 (('user_id', 'conversation_id', 'is_new_conversation', 'state', 'go_on'))
+                    1030 BUILD_CONST_KEY_MAP      5
+                    1032 LOAD_CONST              43 ('user_id')
+         
+         144        1034 LOAD_NAME                9 (str)
+         
+         142        1036 LOAD_CONST              44 ('conversation_id')
+         
+         145        1038 LOAD_NAME                9 (str)
+         
+         142        1040 LOAD_CONST              45 ('is_new_conversation')
+         
+         146        1042 LOAD_NAME               10 (bool)
+         
+         142        1044 LOAD_CONST              12 ('state')
+         
+         147        1046 LOAD_NAME                8 (Optional)
+                    1048 LOAD_NAME                9 (str)
+                    1050 BINARY_SUBSCR
+         
+         142        1060 LOAD_CONST              13 ('go_on')
+         
+         148        1062 LOAD_NAME                8 (Optional)
+                    1064 LOAD_NAME               10 (bool)
+                    1066 BINARY_SUBSCR
+         
+         142        1076 BUILD_TUPLE             10
+                    1078 LOAD_CONST              46 (<code object on_message, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 142>)
+                    1080 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                    1082 STORE_NAME              29 (on_message)
+                    1084 LOAD_CONST               2 (None)
+                    1086 RETURN_VALUE
          consts
             'DispatcherEvents'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
@@ -777,15 +861,65 @@
                varnames   ('user', 'destination', 'state', 'go_on', 'custom_filter', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
                name       'on_user_move'
                firstlineno 121
                lnotab 0x0209
-         names      ('__name__', '__module__', '__qualname__', 'on_start', 'handler', 'CaseIgnoreDefaultValue', 'User', 'Message', 'Optional', 'str', 'bool', 'on_chat', 'on_whisper', 'on_emote', 'Reaction', 'on_reaction', 'on_user_join', 'on_user_leave', 'Tip', 'on_tip', 'set', 'on_channel', 'Destination', 'on_user_move')
+            ('users', 'seconds_left', 'go_on')
+            'users'
+            ('voice', 'muted')
+            'seconds_left'
+            code
+               argcount  : 0
+               nlocals   : 5
+               stacksize : 1
+               flags     : 15
+               code 0x970064015300
+               132           0 RESUME                   0
+               
+               140           2 LOAD_CONST               1 (None)
+                             4 RETURN_VALUE
+               consts
+                  'On a change in voice status in the room.'
+                  None
+               names      ()
+               varnames   ('users', 'seconds_left', 'go_on', 'custom_filter', 'kwargs')
+               freevars   ()
+               cellvars   ()
+               filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
+               name       'on_voice_change'
+               firstlineno 132
+               lnotab 0x0208
+            ('user_id', 'conversation_id', 'is_new_conversation', 'state', 'go_on')
+            'user_id'
+            'conversation_id'
+            'is_new_conversation'
+            code
+               argcount  : 0
+               nlocals   : 7
+               stacksize : 1
+               flags     : 15
+               code 0x970064015300
+               142           0 RESUME                   0
+               
+               152           2 LOAD_CONST               1 (None)
+                             4 RETURN_VALUE
+               consts
+                  'On a inbox message received from a user.'
+                  None
+               names      ()
+               varnames   ('user_id', 'conversation_id', 'is_new_conversation', 'state', 'go_on', 'custom_filter', 'kwargs')
+               freevars   ()
+               cellvars   ()
+               filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
+               name       'on_message'
+               firstlineno 142
+               lnotab 0x020a
+         names      ('__name__', '__module__', '__qualname__', 'on_start', 'handler', 'CaseIgnoreDefaultValue', 'User', 'Message', 'Optional', 'str', 'bool', 'on_chat', 'on_whisper', 'on_emote', 'Reaction', 'on_reaction', 'on_user_join', 'on_user_leave', 'Tip', 'on_tip', 'set', 'on_channel', 'Destination', 'on_user_move', 'list', 'tuple', 'Literal', 'int', 'on_voice_change', 'on_message')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
          name       'DispatcherEvents'
          firstlineno 10
          lnotab
@@ -794,80 +928,82 @@
             0102010c010201020102f606030cfd02040cfc02050cfb02060efa02070e
             f902080ef802090ef7020a0ef60813020102010201020102f906030cfd02
             040cfc02050cfb02060efa02070ef9080f020102010201020102fa06020c
             fe02030cfd02040cfc02050efb02060efa080f0201020102fb06030cfd02
             040efc02050efb080e0201020102fb06030cfd02040efc02050efb080d02
             0102010201020102fa06020cfe02030cfd02040cfc02050efb02060efa08
             0e02010201020102fb06020efe02030cfd02041afc02050efb080d020102
-            01020102fb06020cfe02030cfd02040efc02050efb
+            01020102fb06020cfe02030cfd02040efc02050efb080d0201020102fc06
+            0234fe020302fd02040efc080c020102010201020102fa060202fe020302
+            fd020402fc02050efb02060efa
       'DispatcherEvents'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
             0x8700970065005a0164005a020900640b6402650365046a050000000000
             0000006a060000000000000000190000000000000000006602640384055a
             07640465086602640584045a09650a6406650b6407650b660464088404a6
             000000ab0000000000000000005a0c88006601640984085a0d640a84005a
             0e880078015a0f5300
                        0 MAKE_CELL                0 (__class__)
          
-         133           2 RESUME                   0
+         155           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('Dispatcher')
                       10 STORE_NAME               2 (__qualname__)
          
-         136          12 NOP
+         158          12 NOP
          
-         134          14 LOAD_CONST              11 ((None,))
+         156          14 LOAD_CONST              11 ((None,))
                       16 LOAD_CONST               2 ('fsm_storage')
          
-         136          18 LOAD_NAME                3 (Optional)
+         158          18 LOAD_NAME                3 (Optional)
                       20 LOAD_NAME                4 (fsm)
                       22 LOAD_ATTR                5 (storage)
                       32 LOAD_ATTR                6 (BaseStorage)
                       42 BINARY_SUBSCR
          
-         134          52 BUILD_TUPLE              2
-                      54 LOAD_CONST               3 (<code object __init__, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 134>)
+         156          52 BUILD_TUPLE              2
+                      54 LOAD_CONST               3 (<code object __init__, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 156>)
                       56 MAKE_FUNCTION            5 (defaults, annotations)
                       58 STORE_NAME               7 (__init__)
          
-         146          60 LOAD_CONST               4 ('handler_type')
+         168          60 LOAD_CONST               4 ('handler_type')
                       62 LOAD_NAME                8 (str)
                       64 BUILD_TUPLE              2
-                      66 LOAD_CONST               5 (<code object _process_event, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 146>)
+                      66 LOAD_CONST               5 (<code object _process_event, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 168>)
                       68 MAKE_FUNCTION            4 (annotations)
                       70 STORE_NAME               9 (_process_event)
          
-         149          72 LOAD_NAME               10 (staticmethod)
+         171          72 LOAD_NAME               10 (staticmethod)
          
-         150          74 LOAD_CONST               6 ('handler_data')
+         172          74 LOAD_CONST               6 ('handler_data')
                       76 LOAD_NAME               11 (dict)
                       78 LOAD_CONST               7 ('return')
                       80 LOAD_NAME               11 (dict)
                       82 BUILD_TUPLE              4
-                      84 LOAD_CONST               8 (<code object __pre_processing_handler_data, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 149>)
+                      84 LOAD_CONST               8 (<code object __pre_processing_handler_data, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 171>)
                       86 MAKE_FUNCTION            4 (annotations)
          
-         149          88 PRECALL                  0
+         171          88 PRECALL                  0
                       92 CALL                     0
          
-         150         102 STORE_NAME              12 (_Dispatcher__pre_processing_handler_data)
+         172         102 STORE_NAME              12 (_Dispatcher__pre_processing_handler_data)
          
-         155         104 LOAD_CLOSURE             0 (__class__)
+         177         104 LOAD_CLOSURE             0 (__class__)
                      106 BUILD_TUPLE              1
-                     108 LOAD_CONST               9 (<code object __getattribute__, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 155>)
+                     108 LOAD_CONST               9 (<code object __getattribute__, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 177>)
                      110 MAKE_FUNCTION            8 (closure)
                      112 STORE_NAME              13 (__getattribute__)
          
-         161         114 LOAD_CONST              10 (<code object __create_decorator, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 161>)
+         183         114 LOAD_CONST              10 (<code object __create_decorator, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 183>)
                      116 MAKE_FUNCTION            0
                      118 STORE_NAME              14 (_Dispatcher__create_decorator)
                      120 LOAD_CLOSURE             0 (__class__)
                      122 COPY                     1
                      124 STORE_NAME              15 (__classcell__)
                      126 RETURN_VALUE
          consts
@@ -886,49 +1022,49 @@
                   0400000000000000000000000000000000000000007c01ac01a6010000ab
                   0100000000000000007c005f0300000000000000007c006a030000000000
                   000000740a000000000000000000006a0600000000000000005f00000000
                   0000000000740f00000000000000000000a6000000ab0000000000000000
                   007c005f0800000000000000007413000000000000000000007c006a0800
                   00000000000000ac02a6010000ab0100000000000000007c005f0a000000
                   000000000064005300
-               134           0 RESUME                   0
+               156           0 RESUME                   0
                
-               138           2 LOAD_FAST                1 (fsm_storage)
+               160           2 LOAD_FAST                1 (fsm_storage)
                              4 POP_JUMP_FORWARD_IF_TRUE    30 (to 66)
                
-               139           6 LOAD_GLOBAL              0 (fsm)
+               161           6 LOAD_GLOBAL              0 (fsm)
                             18 LOAD_ATTR                1 (storage)
                             28 LOAD_METHOD              2 (Memory)
                             50 PRECALL                  0
                             54 CALL                     0
                             64 STORE_FAST               1 (fsm_storage)
                
-               140     >>   66 LOAD_GLOBAL              0 (fsm)
+               162     >>   66 LOAD_GLOBAL              0 (fsm)
                             78 LOAD_ATTR                3 (state)
                             88 LOAD_METHOD              4 (FSMState)
                            110 LOAD_FAST                1 (fsm_storage)
                            112 KW_NAMES                 1
                            114 PRECALL                  1
                            118 CALL                     1
                            128 LOAD_FAST                0 (self)
                            130 STORE_ATTR               3 (state)
                
-               141         140 LOAD_FAST                0 (self)
+               163         140 LOAD_FAST                0 (self)
                            142 LOAD_ATTR                3 (state)
                            152 LOAD_GLOBAL             10 (filter)
                            164 LOAD_ATTR                6 (Check)
                            174 STORE_ATTR               0 (fsm)
                
-               143         184 LOAD_GLOBAL             15 (NULL + list)
+               165         184 LOAD_GLOBAL             15 (NULL + list)
                            196 PRECALL                  0
                            200 CALL                     0
                            210 LOAD_FAST                0 (self)
                            212 STORE_ATTR               8 (_Dispatcher__handlers)
                
-               144         222 LOAD_GLOBAL             19 (NULL + HandlerFactory)
+               166         222 LOAD_GLOBAL             19 (NULL + HandlerFactory)
                            234 LOAD_FAST                0 (self)
                            236 LOAD_ATTR                8 (_Dispatcher__handlers)
                            246 KW_NAMES                 2
                            248 PRECALL                  1
                            252 CALL                     1
                            262 LOAD_FAST                0 (self)
                            264 STORE_ATTR              10 (_Dispatcher__handler_factory)
@@ -940,31 +1076,31 @@
                   ('handlers',)
                names      ('fsm', 'storage', 'Memory', 'state', 'FSMState', 'filter', 'Check', 'list', '_Dispatcher__handlers', 'HandlerFactory', '_Dispatcher__handler_factory')
                varnames   ('self', 'fsm_storage')
                freevars   ()
                cellvars   ()
                filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
                name       '__init__'
-               firstlineno 134
+               firstlineno 156
                lnotab 0x020404013c014a012c022601
             'handler_type'
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 5
                flags     : 143
                code
                   0x4b000100970002007c006a0000000000000000006a0100000000000000
                   007c0167017c02a201520069007c03a4018e01830064007b035600970386
                   04010064005300
-               146           0 RETURN_GENERATOR
+               168           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               147           6 PUSH_NULL
+               169           6 PUSH_NULL
                              8 LOAD_FAST                0 (self)
                             10 LOAD_ATTR                0 (_Dispatcher__handler_factory)
                             20 LOAD_ATTR                1 (_process)
                             30 LOAD_FAST                1 (handler_type)
                             32 BUILD_LIST               1
                             34 LOAD_FAST                2 (args)
                             36 LIST_EXTEND              1
@@ -986,61 +1122,61 @@
                   None
                names      ('_Dispatcher__handler_factory', '_process')
                varnames   ('self', 'handler_type', 'args', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
                name       '_process_event'
-               firstlineno 146
+               firstlineno 168
                lnotab 0x0601
             'handler_data'
             'return'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   00a6020000ab020000000000000000721d7403000000000000000000006a
                   0200000000000000007c00640119000000000000000000a6010000ab0100
                   000000000000007c0064013c0000007c005300
-               149           0 RESUME                   0
+               171           0 RESUME                   0
                
-               151           2 LOAD_FAST                0 (handler_data)
+               173           2 LOAD_FAST                0 (handler_data)
                              4 LOAD_METHOD              0 (get)
                             26 LOAD_CONST               1 ('regex')
                             28 LOAD_CONST               0 (None)
                             30 PRECALL                  2
                             34 CALL                     2
                             44 POP_JUMP_FORWARD_IF_FALSE    29 (to 104)
                
-               152          46 LOAD_GLOBAL              3 (NULL + re)
+               174          46 LOAD_GLOBAL              3 (NULL + re)
                             58 LOAD_ATTR                2 (compile)
                             68 LOAD_FAST                0 (handler_data)
                             70 LOAD_CONST               1 ('regex')
                             72 BINARY_SUBSCR
                             82 PRECALL                  1
                             86 CALL                     1
                             96 LOAD_FAST                0 (handler_data)
                             98 LOAD_CONST               1 ('regex')
                            100 STORE_SUBSCR
                
-               153     >>  104 LOAD_FAST                0 (handler_data)
+               175     >>  104 LOAD_FAST                0 (handler_data)
                            106 RETURN_VALUE
                consts
                   None
                   'regex'
                names      ('get', 're', 'compile')
                varnames   ('handler_data',)
                freevars   ()
                cellvars   ()
                filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
                name       '__pre_processing_handler_data'
-               firstlineno 149
+               firstlineno 171
                lnotab 0x02022c013a01
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
@@ -1049,39 +1185,39 @@
                   0300000000000000007c01a6020000ab02000000000000000072157c00a0
                   0400000000000000000000000000000000000000007c01a6010000ab0100
                   000000000000005300740b00000000000000000000a6000000ab00000000
                   0000000000a00600000000000000000000000000000000000000007c01a6
                   010000ab0100000000000000005300
                              0 COPY_FREE_VARS           1
                
-               155           2 RESUME                   0
+               177           2 RESUME                   0
                
-               156           4 LOAD_GLOBAL              1 (NULL + importlib)
+               178           4 LOAD_GLOBAL              1 (NULL + importlib)
                             16 LOAD_ATTR                1 (import_module)
                             26 LOAD_CONST               1 ('hrbot.bot.bot')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 STORE_FAST               2 (bot_module)
                
-               157          44 LOAD_GLOBAL              5 (NULL + hasattr)
+               179          44 LOAD_GLOBAL              5 (NULL + hasattr)
                             56 LOAD_FAST                2 (bot_module)
                             58 LOAD_ATTR                3 (Bot)
                             68 LOAD_FAST                1 (method_name)
                             70 PRECALL                  2
                             74 CALL                     2
                             84 POP_JUMP_FORWARD_IF_FALSE    21 (to 128)
                
-               158          86 LOAD_FAST                0 (self)
+               180          86 LOAD_FAST                0 (self)
                             88 LOAD_METHOD              4 (_Dispatcher__create_decorator)
                            110 LOAD_FAST                1 (method_name)
                            112 PRECALL                  1
                            116 CALL                     1
                            126 RETURN_VALUE
                
-               159     >>  128 LOAD_GLOBAL             11 (NULL + super)
+               181     >>  128 LOAD_GLOBAL             11 (NULL + super)
                            140 PRECALL                  0
                            144 CALL                     0
                            154 LOAD_METHOD              6 (__getattribute__)
                            176 LOAD_FAST                1 (method_name)
                            178 PRECALL                  1
                            182 CALL                     1
                            192 RETURN_VALUE
@@ -1090,35 +1226,35 @@
                   'hrbot.bot.bot'
                names      ('importlib', 'import_module', 'hasattr', 'Bot', '_Dispatcher__create_decorator', 'super', '__getattribute__')
                varnames   ('self', 'method_name', 'bot_module')
                freevars   ('__class__',)
                cellvars   ()
                filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
                name       '__getattribute__'
-               firstlineno 155
+               firstlineno 177
                lnotab 0x040128012a012a01
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 2
                flags     : 3
                code 0x870087019700880188006602640184087d027c025300
                              0 MAKE_CELL                0 (self)
                              2 MAKE_CELL                1 (method_name)
                
-               161           4 RESUME                   0
+               183           4 RESUME                   0
                
-               162           6 LOAD_CLOSURE             1 (method_name)
+               184           6 LOAD_CLOSURE             1 (method_name)
                              8 LOAD_CLOSURE             0 (self)
                             10 BUILD_TUPLE              2
-                            12 LOAD_CONST               1 (<code object wrapper, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 162>)
+                            12 LOAD_CONST               1 (<code object wrapper, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 184>)
                             14 MAKE_FUNCTION            8 (closure)
                             16 STORE_FAST               2 (wrapper)
                
-               178          18 LOAD_FAST                2 (wrapper)
+               200          18 LOAD_FAST                2 (wrapper)
                             20 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 0
                      nlocals   : 3
                      stacksize : 4
@@ -1127,33 +1263,33 @@
                         0x95028700870197008904a0000000000000000000000000000000000000
                         0000008901a6010000ab0100000000000000008a01880088018803880466
                         04640184087d027c025300
                                    0 COPY_FREE_VARS           2
                                    2 MAKE_CELL                0 (custom_filter)
                                    4 MAKE_CELL                1 (kwargs)
                      
-                     162           6 RESUME                   0
+                     184           6 RESUME                   0
                      
-                     163           8 LOAD_DEREF               4 (self)
+                     185           8 LOAD_DEREF               4 (self)
                                   10 LOAD_METHOD              0 (_Dispatcher__pre_processing_handler_data)
                                   32 LOAD_DEREF               1 (kwargs)
                                   34 PRECALL                  1
                                   38 CALL                     1
                                   48 STORE_DEREF              1 (kwargs)
                      
-                     165          50 LOAD_CLOSURE             0 (custom_filter)
+                     187          50 LOAD_CLOSURE             0 (custom_filter)
                                   52 LOAD_CLOSURE             1 (kwargs)
                                   54 LOAD_CLOSURE             3 (method_name)
                                   56 LOAD_CLOSURE             4 (self)
                                   58 BUILD_TUPLE              4
-                                  60 LOAD_CONST               1 (<code object decorator, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 165>)
+                                  60 LOAD_CONST               1 (<code object decorator, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 187>)
                                   62 MAKE_FUNCTION            8 (closure)
                                   64 STORE_FAST               2 (decorator)
                      
-                     176          66 LOAD_FAST                2 (decorator)
+                     198          66 LOAD_FAST                2 (decorator)
                                   68 RETURN_VALUE
                      consts
                         None
                         code
                            argcount  : 1
                            nlocals   : 1
                            stacksize : 12
@@ -1163,89 +1299,89 @@
                               000000000000000000740500000000000000000000890374070000000000
                               00000000007408000000000000000000008903a6020000ab020000000000
                               0000007c008901740b0000000000000000000089026401ac02a6020000ab
                               020000000000000000ac03a6050000ab050000000000000000a6010000ab
                               01000000000000000001007c005300
                                          0 COPY_FREE_VARS           4
                            
-                           165           2 RESUME                   0
+                           187           2 RESUME                   0
                            
-                           167           4 LOAD_DEREF               4 (self)
+                           189           4 LOAD_DEREF               4 (self)
                                          6 LOAD_ATTR                0 (_Dispatcher__handlers)
                                         16 LOAD_METHOD              1 (append)
                                         38 LOAD_GLOBAL              5 (NULL + HandlerObj)
                            
-                           168          50 LOAD_DEREF               3 (method_name)
+                           190          50 LOAD_DEREF               3 (method_name)
                            
-                           169          52 LOAD_GLOBAL              7 (NULL + getattr)
+                           191          52 LOAD_GLOBAL              7 (NULL + getattr)
                                         64 LOAD_GLOBAL              8 (filter)
                                         76 LOAD_DEREF               3 (method_name)
                                         78 PRECALL                  2
                                         82 CALL                     2
                            
-                           170          92 LOAD_FAST                0 (callback)
+                           192          92 LOAD_FAST                0 (callback)
                            
-                           171          94 LOAD_DEREF               1 (custom_filter)
+                           193          94 LOAD_DEREF               1 (custom_filter)
                            
-                           172          96 LOAD_GLOBAL             11 (NULL + DictWrapper)
+                           194          96 LOAD_GLOBAL             11 (NULL + DictWrapper)
                                        108 LOAD_DEREF               2 (kwargs)
                                        110 LOAD_CONST               1 (False)
                                        112 KW_NAMES                 2
                                        114 PRECALL                  2
                                        118 CALL                     2
                            
-                           167         128 KW_NAMES                 3
+                           189         128 KW_NAMES                 3
                                        130 PRECALL                  5
                                        134 CALL                     5
                                        144 PRECALL                  1
                                        148 CALL                     1
                                        158 POP_TOP
                            
-                           174         160 LOAD_FAST                0 (callback)
+                           196         160 LOAD_FAST                0 (callback)
                                        162 RETURN_VALUE
                            consts
                               None
                               False
                               ('rise_exception',)
                               ('type', 'filter_func', 'callback', 'custom_filters', 'data')
                            names      ('_Dispatcher__handlers', 'append', 'HandlerObj', 'getattr', 'filter', 'DictWrapper')
                            varnames   ('callback',)
                            freevars   ('custom_filter', 'kwargs', 'method_name', 'self')
                            cellvars   ()
                            filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
                            name       'decorator'
-                           firstlineno 165
+                           firstlineno 187
                            lnotab 0x04022e01020128010201020120fb2007
                      names      ('_Dispatcher__pre_processing_handler_data',)
                      varnames   ('custom_filter', 'kwargs', 'decorator')
                      freevars   ('method_name', 'self')
                      cellvars   ('custom_filter', 'kwargs')
                      filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
                      name       'wrapper'
-                     firstlineno 162
+                     firstlineno 184
                      lnotab 0x08012a02100b
                names      ()
                varnames   ('self', 'method_name', 'wrapper')
                freevars   ()
                cellvars   ('self', 'method_name')
                filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
                name       '__create_decorator'
-               firstlineno 161
+               firstlineno 183
                lnotab 0x06010c10
             (None,)
          names      ('__name__', '__module__', '__qualname__', 'Optional', 'fsm', 'storage', 'BaseStorage', '__init__', 'str', '_process_event', 'staticmethod', 'dict', '_Dispatcher__pre_processing_handler_data', '__getattribute__', '_Dispatcher__create_decorator', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
          name       'Dispatcher'
-         firstlineno 133
+         firstlineno 155
          lnotab 0x0c0302fe040222fe080c0c0302010eff0e0102050a06
       'Dispatcher'
-   names      ('importlib', 're', 'handler', 'HandlerFactory', 'DictWrapper', 'HandlerObj', '', 'filter', 'fsm', 'types', 'typing', 'Optional', 'DispatcherEvents', 'Dispatcher')
+   names      ('importlib', 're', 'handler', 'HandlerFactory', 'DictWrapper', 'HandlerObj', '', 'filter', 'fsm', 'types', 'typing', 'Optional', 'Literal', 'DispatcherEvents', 'Dispatcher')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020108010802140110010c010c031a7b
+   lnotab 0x00ff020108010802140110010c0110031a7f0012
```

### Comparing `hrbot-0.1.1/hrbot/dispatcher/dispatсher.py` & `hrbot-0.1.2/hrbot/dispatcher/dispatсher.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import importlib
 import re
 
 from .handler import HandlerFactory, DictWrapper, HandlerObj
 from . import filter, fsm
 from ..types import handler
-from typing import Optional
+from typing import Optional, Literal
 
 
 class DispatcherEvents:
     def on_start(self):
         """On a connection to the room being established.
 
         This may be called multiple times, since the connection may be dropped
@@ -125,14 +125,36 @@
             state: Optional[str] = None,
             go_on: Optional[bool] = False,
             **kwargs
     ):
         """On a user moving in the room."""
         pass
 
+    def on_voice_change(
+            *custom_filter,
+            users: list[tuple[handler.User, Literal["voice", "muted"]]] = None,
+            seconds_left: int = None,
+            go_on: Optional[bool] = False,
+            **kwargs
+    ):
+        """On a change in voice status in the room."""
+        pass
+
+    def on_message(
+            *custom_filter,
+            user_id: str = None,
+            conversation_id: str = None,
+            is_new_conversation: bool = None,
+            state: Optional[str] = None,
+            go_on: Optional[bool] = False,
+            **kwargs
+    ):
+        """On a inbox message received from a user."""
+        pass
+
 
 class Dispatcher(DispatcherEvents):
     def __init__(
             self,
             fsm_storage: Optional[fsm.storage.BaseStorage] = None
     ):
         if not fsm_storage:
```

### Comparing `hrbot-0.1.1/hrbot/dispatcher/filter.py` & `hrbot-0.1.2/hrbot/dispatcher/filter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import re
-from typing import Any, Callable, Optional
+from typing import Any, Callable, Optional, Literal
 
 from . import fsm
 from .handler import HandlerObj
 from ..types import handler, hr, _bcolors
 
 
 class Check:
@@ -35,22 +35,22 @@
             if isinstance(handler, (list, tuple, set)) and event not in handler:
                 return False
             if not isinstance(handler, (list, tuple, set)) and not event == handler:
                 return False
         return True
 
     @staticmethod
-    async def state(user: hr.User, handler_filter: HandlerObj):
+    async def state(user_id: str, handler_filter: HandlerObj):
         handler_state = handler_filter.data.state
 
         if handler_state == '*':
             return True
 
         if 'state' in handler_filter.data._data.keys():
-            if await Check.fsm.get_state(user.id) != handler_state:
+            if await Check.fsm.get_state(user_id) != handler_state:
                 return False
         return True
 
     @staticmethod
     async def regex(handler_regex: re.Pattern | None, event_message: str) -> bool:
         if handler_regex and not handler_regex.fullmatch(event_message):
             return False
@@ -93,15 +93,15 @@
 
 async def on_chat(
         handler_filter: HandlerObj,
         user: hr.User,
         message: str,
         *args, **kwargs
 ) -> bool:
-    if not await Check.state(user, handler_filter): return False
+    if not await Check.state(user.id, handler_filter): return False
     if not await Check.compare_two_value(handler_filter.data.user, user): return False
     if not await Check.compare_two_value(handler_filter.data.message,
                                          message, handler_filter.data.case_ignore): return False
     if not await Check.command(handler_filter.data.command,
                                handler_filter.data.prefix if handler_filter.data.prefix else '/.!$#',
                                message, handler_filter.data.case_ignore): return False
     if not await Check.regex(handler_filter.data.regex, message): return False
@@ -113,15 +113,15 @@
 
 async def on_whisper(
         handler_filter: HandlerObj,
         user: hr.User,
         message: str,
         *args, **kwargs
 ) -> bool:
-    if not await Check.state(user, handler_filter): return False
+    if not await Check.state(user.id, handler_filter): return False
     if not await Check.compare_two_value(handler_filter.data.user, user): return False
     if not await Check.compare_two_value(handler_filter.data.message,
                                          message, handler_filter.data.case_ignore): return False
     if not await Check.command(handler_filter.data.command,
                                handler_filter.data.prefix if handler_filter.data.prefix else '/.!$#',
                                message, handler_filter.data.case_ignore): return False
     if not await Check.regex(handler_filter.data.regex, message): return False
@@ -134,15 +134,15 @@
 async def on_emote(
         handler_filter: HandlerObj,
         user: hr.User,
         emote_id: str,
         receiver: hr.User | None,
         *args, **kwargs
 ) -> bool:
-    if not await Check.state(user, handler_filter): return False
+    if not await Check.state(user.id, handler_filter): return False
     if not await Check.compare_two_value(handler_filter.data.user, user): return False
     if not await Check.compare_two_value(handler_filter.data.receiver, receiver): return False
     if not await Check.compare_two_value(handler_filter.data.emote_id, emote_id): return False
     for filter_func in handler_filter.custom_filters:
         if callable(filter_func) and not await Check.func(emote_id, filter_func):
             return False
     return True
@@ -151,58 +151,58 @@
 async def on_reaction(
         handler_filter: HandlerObj,
         user: hr.User,
         reaction: hr.Reaction,
         receiver: hr.User | None,
         *args, **kwargs
 ) -> bool:
-    if not await Check.state(user, handler_filter): return False
+    if not await Check.state(user.id, handler_filter): return False
     if not await Check.compare_two_value(handler_filter.data.user, user): return False
     if not await Check.compare_two_value(handler_filter.data.receiver, receiver): return False
     if not await Check.compare_two_value(handler_filter.data.reaction, reaction): return False
     for filter_func in handler_filter.custom_filters:
         if callable(filter_func) and not await Check.func(reaction, filter_func):
             return False
     return True
 
 
 async def on_user_join(
         handler_filter: HandlerObj,
         user: hr.User,
         *args, **kwargs
 ) -> bool:
-    if not await Check.state(user, handler_filter): return False
+    if not await Check.state(user.id, handler_filter): return False
     if not await Check.compare_two_value(handler_filter.data.user, user): return False
     for filter_func in handler_filter.custom_filters:
         if callable(filter_func) and not await Check.func(user, filter_func):
             return False
     return True
 
 
 async def on_user_leave(
         handler_filter: HandlerObj,
         user: hr.User,
         *args, **kwargs
 ) -> bool:
-    if not await Check.state(user, handler_filter): return False
+    if not await Check.state(user.id, handler_filter): return False
     if not await Check.compare_two_value(handler_filter.data.user, user): return False
     for filter_func in handler_filter.custom_filters:
         if callable(filter_func) and not await Check.func(user, filter_func):
             return False
     return True
 
 
 async def on_tip(
         handler_filter: HandlerObj,
         sender: hr.User,
         receiver: hr.User | None,
         tip: hr.CurrencyItem | hr.Item,
         *args, **kwargs
 ) -> bool:
-    if not await Check.state(sender, handler_filter): return False
+    if not await Check.state(sender.id, handler_filter): return False
     if not await Check.compare_two_value(handler_filter.data.sender, sender): return False
     if not await Check.compare_two_value(handler_filter.data.receiver, receiver): return False
     if not await Check.compare_two_value(handler_filter.data.tip, tip): return False
     for filter_func in handler_filter.custom_filters:
         if callable(filter_func) and not await Check.func(tip, filter_func):
             return False
     return True
@@ -226,14 +226,42 @@
 
 async def on_user_move(
         handler_filter: HandlerObj,
         user: hr.User,
         destination: hr.Position | hr.AnchorPosition,
         *args, **kwargs
 ) -> bool:
-    if not await Check.state(user, handler_filter): return False
+    if not await Check.state(user.id, handler_filter): return False
     if not await Check.compare_two_value(handler_filter.data.user, user): return False
     if not await Check.compare_two_value(handler_filter.data.destination, destination): return False
     for filter_func in handler_filter.custom_filters:
         if callable(filter_func) and not await Check.func(user, filter_func):
             return False
     return True
+
+async def on_voice_change(
+        handler_filter: HandlerObj,
+        users: list[tuple[hr.User, Literal["voice", "muted"]]],
+        seconds_left: int,
+        *args, **kwargs
+) -> bool:
+    if not await Check.compare_two_value(handler_filter.data.seconds_left, seconds_left): return False
+    for filter_func in handler_filter.custom_filters:
+        if callable(filter_func) and not await Check.func(users, filter_func):
+            return False
+    return True
+
+async def on_message(
+        handler_filter: HandlerObj,
+        user_id: str,
+        conversation_id: str,
+        is_new_conversation: bool,
+        *args, **kwargs
+) -> bool:
+    if not await Check.state(user_id, handler_filter): return False
+    if not await Check.compare_two_value(handler_filter.data.user_id, user_id): return False
+    if not await Check.compare_two_value(handler_filter.data.conversation_id, conversation_id): return False
+    if not await Check.compare_two_value(handler_filter.data.is_new_conversation, is_new_conversation): return False
+    for filter_func in handler_filter.custom_filters:
+        if callable(filter_func) and not await Check.func(user_id, filter_func):
+            return False
+    return True
```

### Comparing `hrbot-0.1.1/hrbot/dispatcher/fsm/state.py` & `hrbot-0.1.2/hrbot/dispatcher/fsm/state.py`

 * *Files identical despite different names*

### Comparing `hrbot-0.1.1/hrbot/dispatcher/fsm/storage.py` & `hrbot-0.1.2/hrbot/dispatcher/fsm/storage.py`

 * *Files identical despite different names*

### Comparing `hrbot-0.1.1/hrbot/dispatcher/handler.py` & `hrbot-0.1.2/hrbot/dispatcher/handler.py`

 * *Files identical despite different names*

### Comparing `hrbot-0.1.1/LICENSE` & `hrbot-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hrbot-0.1.1/README.md` & `hrbot-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `hrbot-0.1.1/PKG-INFO` & `hrbot-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: hrbot
-Version: 0.1.1
+Version: 0.1.2
 Summary: The hrbot is a wrapper on top of the HighRise Python Bot SDK that makes it easy to create bots in HighRise.
 License: MIT
 Author: MuoDosta
 Author-email: MuoDostaWork@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: highrise-bot-sdk (==23.1.0b12)
+Requires-Dist: highrise-bot-sdk (==23.1.0b13)
 Requires-Dist: redis (==4.5.5)
 Description-Content-Type: text/markdown
 
 
 # The hrbot  
 The hrbot is a wrapper on top of the [HighRise Python Bot SDK](https://github.com/pocketzworld/python-bot-sdk) that makes it easy to create bots in [HighRise](https://highrise.game/).
```

