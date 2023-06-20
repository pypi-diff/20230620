# Comparing `tmp/test_helper_vbot3-1.4.tar.gz` & `tmp/test_helper_vbot3-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_helper_vbot3-1.4.tar", last modified: Sat May 27 09:44:51 2023, max compression
+gzip compressed data, was "test_helper_vbot3-1.5.tar", last modified: Tue Jun 20 06:34:58 2023, max compression
```

## Comparing `test_helper_vbot3-1.4.tar` & `test_helper_vbot3-1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 09:44:51.779849 test_helper_vbot3-1.4/
--rw-rw-rw-   0        0        0     1094 2023-05-13 15:59:41.000000 test_helper_vbot3-1.4/LICENSE
--rw-rw-rw-   0        0        0       60 2023-05-14 08:37:46.000000 test_helper_vbot3-1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1036 2023-05-27 09:44:51.779849 test_helper_vbot3-1.4/PKG-INFO
--rw-rw-rw-   0        0        0      512 2023-05-14 08:39:31.000000 test_helper_vbot3-1.4/README.md
--rw-rw-rw-   0        0        0      110 2023-05-14 08:37:46.000000 test_helper_vbot3-1.4/pyproject.toml
--rw-rw-rw-   0        0        0      707 2023-05-27 09:44:51.779849 test_helper_vbot3-1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-27 09:44:51.779849 test_helper_vbot3-1.4/test_helper_vbot3.egg-info/
--rw-rw-rw-   0        0        0     1036 2023-05-27 09:44:51.000000 test_helper_vbot3-1.4/test_helper_vbot3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-05-27 09:44:51.000000 test_helper_vbot3-1.4/test_helper_vbot3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 09:44:51.000000 test_helper_vbot3-1.4/test_helper_vbot3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-05-27 09:44:51.000000 test_helper_vbot3-1.4/test_helper_vbot3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-27 09:44:51.000000 test_helper_vbot3-1.4/test_helper_vbot3.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-27 09:44:51.779849 test_helper_vbot3-1.4/tester_vbot3/
--rw-rw-rw-   0        0        0     4078 2023-05-16 07:09:11.000000 test_helper_vbot3-1.4/tester_vbot3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 06:34:58.563821 test_helper_vbot3-1.5/
+-rw-rw-rw-   0        0        0     1073 2023-06-20 06:07:13.000000 test_helper_vbot3-1.5/LICENSE
+-rw-rw-rw-   0        0        0       58 2023-06-20 06:07:13.000000 test_helper_vbot3-1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1036 2023-06-20 06:34:58.563821 test_helper_vbot3-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      506 2023-06-20 06:07:13.000000 test_helper_vbot3-1.5/README.md
+-rw-rw-rw-   0        0        0      104 2023-06-20 06:07:13.000000 test_helper_vbot3-1.5/pyproject.toml
+-rw-rw-rw-   0        0        0      707 2023-06-20 06:34:58.565514 test_helper_vbot3-1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-20 06:34:58.551641 test_helper_vbot3-1.5/test_helper_vbot3.egg-info/
+-rw-rw-rw-   0        0        0     1036 2023-06-20 06:34:58.000000 test_helper_vbot3-1.5/test_helper_vbot3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-06-20 06:34:58.000000 test_helper_vbot3-1.5/test_helper_vbot3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 06:34:58.000000 test_helper_vbot3-1.5/test_helper_vbot3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-06-20 06:34:58.000000 test_helper_vbot3-1.5/test_helper_vbot3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-20 06:34:58.000000 test_helper_vbot3-1.5/test_helper_vbot3.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 06:34:58.551641 test_helper_vbot3-1.5/tester_vbot3/
+-rw-rw-rw-   0        0        0     5512 2023-06-20 04:48:45.000000 test_helper_vbot3-1.5/tester_vbot3/__init__.py
```

### Comparing `test_helper_vbot3-1.4/PKG-INFO` & `test_helper_vbot3-1.5/test_helper_vbot3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: test_helper_vbot3
-Version: 1.4
+Name: test-helper-vbot3
+Version: 1.5
 Summary: Tester for Vbot3
 Home-page: https://github.com/vb64/test.helper.vbot3
 Author: Vitaly Bogomolov
 Author-email: mail@vitaly-bogomolov.ru
 Project-URL: Bug Tracker, https://github.com/vb64/test.helper.vbot3/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `test_helper_vbot3-1.4/README.md` & `test_helper_vbot3-1.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,6 +1,21 @@
+Metadata-Version: 2.1
+Name: test_helper_vbot3
+Version: 1.5
+Summary: Tester for Vbot3
+Home-page: https://github.com/vb64/test.helper.vbot3
+Author: Vitaly Bogomolov
+Author-email: mail@vitaly-bogomolov.ru
+Project-URL: Bug Tracker, https://github.com/vb64/test.helper.vbot3/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # test.helper.vbot3
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/vb64/test.helper.vbot3/pep257.yml?label=Pep257&style=plastic&branch=main)](https://github.com/vb64/test.helper.vbot3/actions?query=workflow%3Apep257)
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/vb64/test.helper.vbot3/py3.yml?label=Python%203.7-3.11&style=plastic&branch=main)](https://github.com/vb64/test.helper.vbot3/actions?query=workflow%3Apy3)
 
 Tester for Vbot3
```

### Comparing `test_helper_vbot3-1.4/setup.cfg` & `test_helper_vbot3-1.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 6573 745f 6865 6c70 6572 5f76   = test_helper_v
 00000020: 626f 7433 0d0a 7665 7273 696f 6e20 3d20  bot3..version = 
-00000030: 312e 340d 0a61 7574 686f 7220 3d20 5669  1.4..author = Vi
+00000030: 312e 350d 0a61 7574 686f 7220 3d20 5669  1.5..author = Vi
 00000040: 7461 6c79 2042 6f67 6f6d 6f6c 6f76 0d0a  taly Bogomolov..
 00000050: 6175 7468 6f72 5f65 6d61 696c 203d 206d  author_email = m
 00000060: 6169 6c40 7669 7461 6c79 2d62 6f67 6f6d  ail@vitaly-bogom
 00000070: 6f6c 6f76 2e72 750d 0a64 6573 6372 6970  olov.ru..descrip
 00000080: 7469 6f6e 203d 2054 6573 7465 7220 666f  tion = Tester fo
 00000090: 7220 5662 6f74 330d 0a6c 6f6e 675f 6465  r Vbot3..long_de
 000000a0: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
```

### Comparing `test_helper_vbot3-1.4/tester_vbot3/__init__.py` & `test_helper_vbot3-1.5/tester_vbot3/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Vbot3 tester."""
-from telemulator3 import Telemulator, private_command, private_text
-from telemulator3.update.message import Text, Command
+from telemulator3 import Telemulator, private_command, private_text, private_document, send_text
+from telemulator3.update.message import Text, Command, Contact
 from tester_flask import TestFlask
 from test_helper_gae3 import TestGae3
 
 
 class MockReq:
     """Mock flask request."""
 
@@ -61,14 +61,29 @@
             return chat.send(message)
 
     def send_command(self, chat, command, from_user=None, **kwargs):
         """Send command to given chat."""
         from_user = from_user or self.teleuser
         return self.send2chat(chat, Command(chat, from_user, command, **kwargs))
 
+    def send_contact(  # pylint: disable=too-many-arguments
+      self, chat, phone_number, from_user=None, first_name='Contact', last_name='User', user_id=777, **kwargs
+    ):
+        """Send contact to given chat."""
+        from_user = from_user or self.teleuser
+        return self.send2chat(
+          chat,
+          Contact(chat, from_user, phone_number, first_name, last_name, user_id, **kwargs)
+        )
+
+    def send_text(self, chat, text, from_user=None):
+        """Send text to chat and return sended message."""
+        from_user = from_user or self.teleuser
+        return send_text(chat, text, from_user)
+
     def tg_button(self, row, index=0, chat=None, user=None):
         """Send custom keyboard item to chat."""
         chat = chat or self.private
         user = user or self.teleuser
         chat.keyboard.menu_item(user, index, row=row)
 
     def private_command(self, cmd, from_user=None):
@@ -79,14 +94,30 @@
 
     def private_text(self, text, from_user=None):
         """Call private command."""
         from_user = from_user or self.teleuser
         with self.app.test_request_context():
             private_text(text, from_user)
 
+    def private_document(self, file_name, from_user=None, file_size=600):
+        """Call private command."""
+        from_user = from_user or self.teleuser
+        with self.app.test_request_context():
+            private_document(file_name, from_user=from_user, file_size=file_size)
+
+    def private_contact(  # pylint: disable=too-many-arguments
+      self, phone_number, from_user=None, first_name='Contact', last_name='User', user_id=777, **kwargs
+    ):
+        """Send contact to private chat."""
+        from_user = from_user or self.teleuser
+        return self.send_contact(
+          from_user.private(), phone_number, from_user=from_user,
+          first_name=first_name, last_name=last_name, user_id=user_id, **kwargs
+        )
+
     def assert_in_history(self, substring, chat=None):
         """Check substring in the history of given chat."""
         chat = chat or self.private
         assert chat.history.contain(substring)
 
     def assert_not_in_history(self, substring, chat=None):
         """Check substring not in the history of given chat."""
```

