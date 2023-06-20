# Comparing `tmp/whatsapp-chatbot-python-0.2.3.tar.gz` & `tmp/whatsapp-chatbot-python-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp-chatbot-python-0.2.3.tar", last modified: Thu Jun 15 04:46:38 2023, max compression
+gzip compressed data, was "whatsapp-chatbot-python-0.3.0.tar", last modified: Tue Jun 20 08:37:10 2023, max compression
```

## Comparing `whatsapp-chatbot-python-0.2.3.tar` & `whatsapp-chatbot-python-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 04:46:38.808624 whatsapp-chatbot-python-0.2.3/
--rw-rw-rw-   0        0        0    18829 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.3/LICENSE
--rw-rw-rw-   0        0        0     9060 2023-06-15 04:46:38.807622 whatsapp-chatbot-python-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     8035 2023-06-08 08:50:01.000000 whatsapp-chatbot-python-0.2.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-15 04:46:38.808624 whatsapp-chatbot-python-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1405 2023-06-15 04:43:42.000000 whatsapp-chatbot-python-0.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 04:46:38.795589 whatsapp-chatbot-python-0.2.3/tests/
--rw-rw-rw-   0        0        0     1224 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.3/tests/test_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-15 04:46:38.798597 whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python/
--rw-rw-rw-   0        0        0      184 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python/__init__.py
--rw-rw-rw-   0        0        0     1020 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python/bot.py
--rw-rw-rw-   0        0        0     3569 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python/filters.py
-drwxrwxrwx   0        0        0        0 2023-06-15 04:46:38.806618 whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python/manager/
--rw-rw-rw-   0        0        0        0 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python/manager/__init__.py
--rw-rw-rw-   0        0        0     3277 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python/manager/handler.py
--rw-rw-rw-   0        0        0     1821 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python/manager/observer.py
--rw-rw-rw-   0        0        0     1144 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python/manager/router.py
-drwxrwxrwx   0        0        0        0 2023-06-15 04:46:38.802609 whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python.egg-info/
--rw-rw-rw-   0        0        0     9060 2023-06-15 04:46:38.000000 whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      557 2023-06-15 04:46:38.000000 whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 04:46:38.000000 whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-06-15 04:46:38.000000 whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-06-15 04:46:38.000000 whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 08:37:10.542245 whatsapp-chatbot-python-0.3.0/
+-rw-rw-rw-   0        0        0    18829 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0    10908 2023-06-20 08:37:10.541448 whatsapp-chatbot-python-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9883 2023-06-20 08:33:46.000000 whatsapp-chatbot-python-0.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-20 08:37:10.542245 whatsapp-chatbot-python-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1405 2023-06-20 08:34:37.000000 whatsapp-chatbot-python-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:37:10.530419 whatsapp-chatbot-python-0.3.0/tests/
+-rw-rw-rw-   0        0        0     1224 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.3.0/tests/test_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:37:10.533427 whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python/
+-rw-rw-rw-   0        0        0      184 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python/__init__.py
+-rw-rw-rw-   0        0        0     1020 2023-06-18 19:42:33.000000 whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python/bot.py
+-rw-rw-rw-   0        0        0     3673 2023-06-20 08:33:46.000000 whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python/filters.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:37:10.540447 whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python/manager/
+-rw-rw-rw-   0        0        0        0 2023-06-04 05:34:07.000000 whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python/manager/__init__.py
+-rw-rw-rw-   0        0        0     3289 2023-06-20 08:33:46.000000 whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python/manager/handler.py
+-rw-rw-rw-   0        0        0     1881 2023-06-20 08:33:46.000000 whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python/manager/observer.py
+-rw-rw-rw-   0        0        0     1144 2023-06-15 14:08:46.000000 whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python/manager/router.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:37:10.537438 whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python.egg-info/
+-rw-rw-rw-   0        0        0    10908 2023-06-20 08:37:10.000000 whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      557 2023-06-20 08:37:10.000000 whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 08:37:10.000000 whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-20 08:37:10.000000 whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-06-20 08:37:10.000000 whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python.egg-info/top_level.txt
```

### Comparing `whatsapp-chatbot-python-0.2.3/LICENSE` & `whatsapp-chatbot-python-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.2.3/PKG-INFO` & `whatsapp-chatbot-python-0.3.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: whatsapp-chatbot-python
-Version: 0.2.3
-Summary: This library helps you easily create a Python chatbot with WhatsApp API.
-Home-page: https://github.com/green-api/whatsapp-chatbot-python
-Author: GREEN API
-Author-email: support@green-api.com
-License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: Other/Proprietary License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # whatsapp-chatbot-python
 
 ![](https://img.shields.io/badge/license-CC%20BY--ND%204.0-green)
 ![](https://img.shields.io/pypi/status/whatsapp-chatbot-python)
 ![](https://img.shields.io/pypi/pyversions/whatsapp-chatbot-python)
 ![](https://img.shields.io/github/actions/workflow/status/green-api/whatsapp-chatbot-python/python-package.yml)
 ![](https://img.shields.io/pypi/dm/whatsapp-chatbot-python)
@@ -123,15 +100,15 @@
 expressions. Below is a table with filter names and possible values.
 
 | Filter name    | Description                                                                               | Possible values                                                    |
 |----------------|-------------------------------------------------------------------------------------------|--------------------------------------------------------------------|
 | `from_chat`    | Chats or chats from which you want to receive messages                                    | `"11001234567@c.us"` or `["11001234567@c.us", "11002345678@c.us"]` |
 | `from_sender`  | The sender or senders from whom you want to receive messages                              | `"11001234567@c.us"` or `["11001234567@c.us", "11002345678@c.us"]` |
 | `type_message` | The type or types of message to be handled                                                | `"textMessage"` or `["textMessage", "extendedTextMessage"]`        |
-| `text_message` | Your function will be executed if the text fully matches the text                         | `"Hello. I need help."`                                            |
+| `text_message` | Your function will be executed if the text fully matches the text                         | `"Hello. I need help."` or `["Hello", "I need help"]`              |
 | `regexp`       | Your function will be executed if the text matches the regular expression pattern         | `r"Hello. I need help."`                                           |
 | `command`      | Your function will be executed if the prefix and the command match your values completely | `"help"` or `("help", "!/")`                                       |
 
 #### How to add filters through the decorator
 
 ```
 @bot.router.message(command="command")
@@ -185,17 +162,17 @@
 ```
 
 #### Example
 
 Link to example: [filters.py](https://github.com/green-api/whatsapp-chatbot-python/blob/master/examples/filters.py).
 
 ```
-@bot.router.message(command="help")
+@bot.router.message(command="rates")
 def message_handler(notification: Notification) -> None:
-    notification.answer_with_file(file="help.png")
+    notification.answer_with_file(file="data/rates.png")
 
 
 bot.run_forever()
 ```
 
 ### How to handle buttons
 
@@ -221,17 +198,78 @@
         }
     ])
 
 
 bot.run_forever()
 ```
 
+### Example of a bot
+
+Link to example: [full_example.py](
+https://github.com/green-api/whatsapp-chatbot-python/blob/master/examples/full_example.py
+).
+
+```python
+from whatsapp_chatbot_python import GreenAPIBot, Notification
+
+bot = GreenAPIBot(
+    "1101000001", "d75b3a66374942c5b3c019c698abc2067e151558acbd412345"
+)
+
+
+@bot.router.message(command="start")
+def message_handler(notification: Notification) -> None:
+    sender_data = notification.event["senderData"]
+    sender_name = sender_data["senderName"]
+
+    notification.answer(
+        (
+            f"Hello, {sender_name}. Here's what I can do:\n\n"
+            "1. Report a problem\n"
+            "2. Show office address\n"
+            "3. Show available rates\n"
+            "4. Call a support operator\n\n"
+            "Choose a number and send to me."
+        )
+    )
+
+
+@bot.router.message(text_message=["1", "Report a problem"])
+def report_problem_handler(notification: Notification) -> None:
+    notification.answer(
+        "https://github.com/green-api/issues/issues/new", link_preview=False
+    )
+
+
+@bot.router.message(text_message=["2", "Show office address"])
+def show_office_address_handler(notification: Notification) -> None:
+    chat = notification.get_chat()
+
+    notification.api.sending.sendLocation(
+        chatId=chat, latitude=55.7522200, longitude=37.6155600
+    )
+
+
+@bot.router.message(text_message=["3", "Show available rates"])
+def show_available_rates_handler(notification: Notification) -> None:
+    notification.answer_with_file("data/rates.png")
+
+
+@bot.router.message(text_message=["4", "Call a support operator"])
+def call_support_operator_handler(notification: Notification) -> None:
+    notification.answer("Good. A tech support operator will contact you soon.")
+
+
+bot.run_forever()
+```
+
 ## Service methods documentation
 
 [Service methods documentation](https://green-api.com/en/docs/api/)
 
 ## License
 
 Licensed under [
 Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
-](https://creativecommons.org/licenses/by-nd/4.0/) terms.
-Please see file [LICENSE](https://github.com/green-api/whatsapp-chatbot-python/blob/master/LICENSE).
+](https://creativecommons.org/licenses/by-nd/4.0/) terms. Please see file [LICENSE](
+https://github.com/green-api/whatsapp-chatbot-python/blob/master/LICENSE
+).
```

### Comparing `whatsapp-chatbot-python-0.2.3/README.md` & `whatsapp-chatbot-python-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: whatsapp-chatbot-python
+Version: 0.3.0
+Summary: This library helps you easily create a Python chatbot with WhatsApp API.
+Home-page: https://github.com/green-api/whatsapp-chatbot-python
+Author: GREEN API
+Author-email: support@green-api.com
+License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # whatsapp-chatbot-python
 
 ![](https://img.shields.io/badge/license-CC%20BY--ND%204.0-green)
 ![](https://img.shields.io/pypi/status/whatsapp-chatbot-python)
 ![](https://img.shields.io/pypi/pyversions/whatsapp-chatbot-python)
 ![](https://img.shields.io/github/actions/workflow/status/green-api/whatsapp-chatbot-python/python-package.yml)
 ![](https://img.shields.io/pypi/dm/whatsapp-chatbot-python)
@@ -100,15 +123,15 @@
 expressions. Below is a table with filter names and possible values.
 
 | Filter name    | Description                                                                               | Possible values                                                    |
 |----------------|-------------------------------------------------------------------------------------------|--------------------------------------------------------------------|
 | `from_chat`    | Chats or chats from which you want to receive messages                                    | `"11001234567@c.us"` or `["11001234567@c.us", "11002345678@c.us"]` |
 | `from_sender`  | The sender or senders from whom you want to receive messages                              | `"11001234567@c.us"` or `["11001234567@c.us", "11002345678@c.us"]` |
 | `type_message` | The type or types of message to be handled                                                | `"textMessage"` or `["textMessage", "extendedTextMessage"]`        |
-| `text_message` | Your function will be executed if the text fully matches the text                         | `"Hello. I need help."`                                            |
+| `text_message` | Your function will be executed if the text fully matches the text                         | `"Hello. I need help."` or `["Hello", "I need help"]`              |
 | `regexp`       | Your function will be executed if the text matches the regular expression pattern         | `r"Hello. I need help."`                                           |
 | `command`      | Your function will be executed if the prefix and the command match your values completely | `"help"` or `("help", "!/")`                                       |
 
 #### How to add filters through the decorator
 
 ```
 @bot.router.message(command="command")
@@ -162,17 +185,17 @@
 ```
 
 #### Example
 
 Link to example: [filters.py](https://github.com/green-api/whatsapp-chatbot-python/blob/master/examples/filters.py).
 
 ```
-@bot.router.message(command="help")
+@bot.router.message(command="rates")
 def message_handler(notification: Notification) -> None:
-    notification.answer_with_file(file="help.png")
+    notification.answer_with_file(file="data/rates.png")
 
 
 bot.run_forever()
 ```
 
 ### How to handle buttons
 
@@ -198,17 +221,78 @@
         }
     ])
 
 
 bot.run_forever()
 ```
 
+### Example of a bot
+
+Link to example: [full_example.py](
+https://github.com/green-api/whatsapp-chatbot-python/blob/master/examples/full_example.py
+).
+
+```python
+from whatsapp_chatbot_python import GreenAPIBot, Notification
+
+bot = GreenAPIBot(
+    "1101000001", "d75b3a66374942c5b3c019c698abc2067e151558acbd412345"
+)
+
+
+@bot.router.message(command="start")
+def message_handler(notification: Notification) -> None:
+    sender_data = notification.event["senderData"]
+    sender_name = sender_data["senderName"]
+
+    notification.answer(
+        (
+            f"Hello, {sender_name}. Here's what I can do:\n\n"
+            "1. Report a problem\n"
+            "2. Show office address\n"
+            "3. Show available rates\n"
+            "4. Call a support operator\n\n"
+            "Choose a number and send to me."
+        )
+    )
+
+
+@bot.router.message(text_message=["1", "Report a problem"])
+def report_problem_handler(notification: Notification) -> None:
+    notification.answer(
+        "https://github.com/green-api/issues/issues/new", link_preview=False
+    )
+
+
+@bot.router.message(text_message=["2", "Show office address"])
+def show_office_address_handler(notification: Notification) -> None:
+    chat = notification.get_chat()
+
+    notification.api.sending.sendLocation(
+        chatId=chat, latitude=55.7522200, longitude=37.6155600
+    )
+
+
+@bot.router.message(text_message=["3", "Show available rates"])
+def show_available_rates_handler(notification: Notification) -> None:
+    notification.answer_with_file("data/rates.png")
+
+
+@bot.router.message(text_message=["4", "Call a support operator"])
+def call_support_operator_handler(notification: Notification) -> None:
+    notification.answer("Good. A tech support operator will contact you soon.")
+
+
+bot.run_forever()
+```
+
 ## Service methods documentation
 
 [Service methods documentation](https://green-api.com/en/docs/api/)
 
 ## License
 
 Licensed under [
 Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
-](https://creativecommons.org/licenses/by-nd/4.0/) terms.
-Please see file [LICENSE](https://github.com/green-api/whatsapp-chatbot-python/blob/master/LICENSE).
+](https://creativecommons.org/licenses/by-nd/4.0/) terms. Please see file [LICENSE](
+https://github.com/green-api/whatsapp-chatbot-python/blob/master/LICENSE
+).
```

### Comparing `whatsapp-chatbot-python-0.2.3/setup.py` & `whatsapp-chatbot-python-0.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="UTF-8") as file:
     long_description = file.read()
 
 setup(
     name="whatsapp-chatbot-python",
-    version="0.2.3",
+    version="0.3.0",
     description=(
         "This library helps you easily create"
         " a Python chatbot with WhatsApp API."
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="GREEN API",
```

### Comparing `whatsapp-chatbot-python-0.2.3/tests/test_manager.py` & `whatsapp-chatbot-python-0.3.0/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python/bot.py` & `whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python/bot.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python/filters.py` & `whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python/filters.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,20 +49,24 @@
                 or type_message in self.type_message
         ):
             return True
         return False
 
 
 class TextMessageFilter(AbstractFilter):
-    def __init__(self, text_message: str):
+    def __init__(self, text_message: Union[str, List[str]]):
         self.text_message = text_message
 
     def check_event(self, event: dict) -> bool:
         text_message = self.get_text_message(event)
-        if text_message == self.text_message:
+
+        if (
+                text_message == self.text_message
+                or text_message in self.text_message
+        ):
             return True
         return False
 
     @staticmethod
     def get_text_message(event: dict) -> Optional[str]:
         message_data = event["messageData"]
```

### Comparing `whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python/manager/handler.py` & `whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python/manager/handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     filters: Dict[str, Any]
 
     @abstractmethod
     def check_event(self, event: dict) -> bool:
         pass
 
     @abstractmethod
-    def execute_handler(self, observer: "Observer") -> Any:
+    def execute_handler(self, observer: "Observer") -> bool:
         pass
 
 
 class Handler(AbstractHandler):
     def __init__(self, handler: HandlerType, **filters: Any):
         self.handler = handler
         self.filters = filters
@@ -94,16 +94,17 @@
                 filter_data = self.filters[filter_name]
                 response = filter_(filter_data).check_event(event)
                 if not response:
                     return False
 
         return True
 
-    def execute_handler(self, observer: "Observer") -> Any:
+    def execute_handler(self, observer: "Observer") -> bool:
         response = self.check_event(observer.event)
         if response:
-            return self.handler(
-                Notification(observer.event, observer.router.api)
-            )
+            self.handler(Notification(observer.event, observer.router.api))
+
+            return True
+        return False
 
 
 __all__ = ["Notification", "HandlerType", "AbstractHandler", "Handler"]
```

### Comparing `whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python/manager/observer.py` & `whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python/manager/observer.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,17 @@
         self.handlers = []
 
     def add_handler(self, handler: HandlerType, **filters: Any) -> None:
         self.handlers.append(Handler(handler, **filters))
 
     def propagate_event(self) -> None:
         for handler in self.handlers:
-            handler.execute_handler(self)
+            response = handler.execute_handler(self)
+            if response:
+                break
 
     def __call__(self, **filters: Any) -> Callable[[HandlerType], HandlerType]:
         def wrapper(handler: HandlerType) -> HandlerType:
             self.add_handler(handler, **filters)
 
             return handler
```

### Comparing `whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python/manager/router.py` & `whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python/manager/router.py`

 * *Files identical despite different names*

### Comparing `whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python.egg-info/PKG-INFO` & `whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whatsapp-chatbot-python
-Version: 0.2.3
+Version: 0.3.0
 Summary: This library helps you easily create a Python chatbot with WhatsApp API.
 Home-page: https://github.com/green-api/whatsapp-chatbot-python
 Author: GREEN API
 Author-email: support@green-api.com
 License: Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -123,15 +123,15 @@
 expressions. Below is a table with filter names and possible values.
 
 | Filter name    | Description                                                                               | Possible values                                                    |
 |----------------|-------------------------------------------------------------------------------------------|--------------------------------------------------------------------|
 | `from_chat`    | Chats or chats from which you want to receive messages                                    | `"11001234567@c.us"` or `["11001234567@c.us", "11002345678@c.us"]` |
 | `from_sender`  | The sender or senders from whom you want to receive messages                              | `"11001234567@c.us"` or `["11001234567@c.us", "11002345678@c.us"]` |
 | `type_message` | The type or types of message to be handled                                                | `"textMessage"` or `["textMessage", "extendedTextMessage"]`        |
-| `text_message` | Your function will be executed if the text fully matches the text                         | `"Hello. I need help."`                                            |
+| `text_message` | Your function will be executed if the text fully matches the text                         | `"Hello. I need help."` or `["Hello", "I need help"]`              |
 | `regexp`       | Your function will be executed if the text matches the regular expression pattern         | `r"Hello. I need help."`                                           |
 | `command`      | Your function will be executed if the prefix and the command match your values completely | `"help"` or `("help", "!/")`                                       |
 
 #### How to add filters through the decorator
 
 ```
 @bot.router.message(command="command")
@@ -185,17 +185,17 @@
 ```
 
 #### Example
 
 Link to example: [filters.py](https://github.com/green-api/whatsapp-chatbot-python/blob/master/examples/filters.py).
 
 ```
-@bot.router.message(command="help")
+@bot.router.message(command="rates")
 def message_handler(notification: Notification) -> None:
-    notification.answer_with_file(file="help.png")
+    notification.answer_with_file(file="data/rates.png")
 
 
 bot.run_forever()
 ```
 
 ### How to handle buttons
 
@@ -221,17 +221,78 @@
         }
     ])
 
 
 bot.run_forever()
 ```
 
+### Example of a bot
+
+Link to example: [full_example.py](
+https://github.com/green-api/whatsapp-chatbot-python/blob/master/examples/full_example.py
+).
+
+```python
+from whatsapp_chatbot_python import GreenAPIBot, Notification
+
+bot = GreenAPIBot(
+    "1101000001", "d75b3a66374942c5b3c019c698abc2067e151558acbd412345"
+)
+
+
+@bot.router.message(command="start")
+def message_handler(notification: Notification) -> None:
+    sender_data = notification.event["senderData"]
+    sender_name = sender_data["senderName"]
+
+    notification.answer(
+        (
+            f"Hello, {sender_name}. Here's what I can do:\n\n"
+            "1. Report a problem\n"
+            "2. Show office address\n"
+            "3. Show available rates\n"
+            "4. Call a support operator\n\n"
+            "Choose a number and send to me."
+        )
+    )
+
+
+@bot.router.message(text_message=["1", "Report a problem"])
+def report_problem_handler(notification: Notification) -> None:
+    notification.answer(
+        "https://github.com/green-api/issues/issues/new", link_preview=False
+    )
+
+
+@bot.router.message(text_message=["2", "Show office address"])
+def show_office_address_handler(notification: Notification) -> None:
+    chat = notification.get_chat()
+
+    notification.api.sending.sendLocation(
+        chatId=chat, latitude=55.7522200, longitude=37.6155600
+    )
+
+
+@bot.router.message(text_message=["3", "Show available rates"])
+def show_available_rates_handler(notification: Notification) -> None:
+    notification.answer_with_file("data/rates.png")
+
+
+@bot.router.message(text_message=["4", "Call a support operator"])
+def call_support_operator_handler(notification: Notification) -> None:
+    notification.answer("Good. A tech support operator will contact you soon.")
+
+
+bot.run_forever()
+```
+
 ## Service methods documentation
 
 [Service methods documentation](https://green-api.com/en/docs/api/)
 
 ## License
 
 Licensed under [
 Creative Commons Attribution-NoDerivatives 4.0 International (CC BY-ND 4.0)
-](https://creativecommons.org/licenses/by-nd/4.0/) terms.
-Please see file [LICENSE](https://github.com/green-api/whatsapp-chatbot-python/blob/master/LICENSE).
+](https://creativecommons.org/licenses/by-nd/4.0/) terms. Please see file [LICENSE](
+https://github.com/green-api/whatsapp-chatbot-python/blob/master/LICENSE
+).
```

### Comparing `whatsapp-chatbot-python-0.2.3/whatsapp_chatbot_python.egg-info/SOURCES.txt` & `whatsapp-chatbot-python-0.3.0/whatsapp_chatbot_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

