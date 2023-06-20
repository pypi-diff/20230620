# Comparing `tmp/SkPy-0.9.tar.gz` & `tmp/SkPy-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Wed Jul 11 19:56:08 2018, from Unix
+gzip compressed data, was "dist/SkPy-0.9.1.tar", last modified: Mon Oct 14 17:58:50 2019, max compression
```

## Comparing `SkPy-0.9.tar` & `SkPy-0.9.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0        0        0        0 2018-07-11 19:47:21.000000 SkPy-0.9/
--rw-r--r--   0        0        0     4338 2018-07-11 19:47:21.000000 SkPy-0.9/PKG-INFO
--rw-r--r--   0        0        0     3207 2016-09-06 21:34:44.000000 SkPy-0.9/README.rst
--rw-r--r--   0        0        0       38 2018-07-11 19:47:21.000000 SkPy-0.9/setup.cfg
--rw-r--r--   0        0        0      790 2018-07-11 19:35:52.000000 SkPy-0.9/setup.py
-drwxr-xr-x   0        0        0        0 2018-07-11 19:47:21.000000 SkPy-0.9/skpy/
--rw-r--r--   0        0        0    20984 2018-04-11 17:38:34.000000 SkPy-0.9/skpy/chat.py
--rw-r--r--   0        0        0    39548 2018-07-11 19:34:27.000000 SkPy-0.9/skpy/conn.py
--rw-r--r--   0        0        0     7908 2017-04-20 17:27:16.000000 SkPy-0.9/skpy/core.py
--rw-r--r--   0        0        0     8344 2017-04-20 17:27:19.000000 SkPy-0.9/skpy/event.py
--rw-r--r--   0        0        0    16499 2018-07-11 19:32:10.000000 SkPy-0.9/skpy/main.py
--rw-r--r--   0        0        0    31546 2018-07-11 19:17:44.000000 SkPy-0.9/skpy/msg.py
--rw-r--r--   0        0        0    21298 2018-07-11 19:17:44.000000 SkPy-0.9/skpy/user.py
--rw-r--r--   0        0        0    10165 2017-04-24 19:03:42.000000 SkPy-0.9/skpy/util.py
--rw-r--r--   0        0        0     1218 2017-04-20 17:32:47.000000 SkPy-0.9/skpy/__init__.py
-drwxr-xr-x   0        0        0        0 2018-07-11 19:47:21.000000 SkPy-0.9/SkPy.egg-info/
--rw-r--r--   0        0        0        1 2018-07-11 19:47:21.000000 SkPy-0.9/SkPy.egg-info/dependency_links.txt
--rw-r--r--   0        0        0     4338 2018-07-11 19:47:21.000000 SkPy-0.9/SkPy.egg-info/PKG-INFO
--rw-r--r--   0        0        0       24 2018-07-11 19:47:21.000000 SkPy-0.9/SkPy.egg-info/requires.txt
--rw-r--r--   0        0        0      279 2018-07-11 19:47:21.000000 SkPy-0.9/SkPy.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        5 2018-07-11 19:47:21.000000 SkPy-0.9/SkPy.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2019-10-14 17:58:50.000000 SkPy-0.9.1/
+-rw-r--r--   0 user      (1000) user      (1000)     4307 2019-10-14 17:58:50.000000 SkPy-0.9.1/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     3207 2019-10-14 17:48:58.000000 SkPy-0.9.1/README.rst
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2019-10-14 17:58:50.000000 SkPy-0.9.1/SkPy.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     4307 2019-10-14 17:58:50.000000 SkPy-0.9.1/SkPy.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      279 2019-10-14 17:58:50.000000 SkPy-0.9.1/SkPy.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2019-10-14 17:58:50.000000 SkPy-0.9.1/SkPy.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       24 2019-10-14 17:58:50.000000 SkPy-0.9.1/SkPy.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        5 2019-10-14 17:58:50.000000 SkPy-0.9.1/SkPy.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2019-10-14 17:58:50.000000 SkPy-0.9.1/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      793 2019-10-14 17:58:37.000000 SkPy-0.9.1/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2019-10-14 17:58:50.000000 SkPy-0.9.1/skpy/
+-rw-r--r--   0 user      (1000) user      (1000)     1218 2019-10-14 17:48:58.000000 SkPy-0.9.1/skpy/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)    22503 2019-10-14 17:48:58.000000 SkPy-0.9.1/skpy/chat.py
+-rw-r--r--   0 user      (1000) user      (1000)    39548 2019-10-14 17:48:58.000000 SkPy-0.9.1/skpy/conn.py
+-rw-r--r--   0 user      (1000) user      (1000)     7908 2019-10-14 17:48:58.000000 SkPy-0.9.1/skpy/core.py
+-rw-r--r--   0 user      (1000) user      (1000)     8344 2019-10-14 17:48:58.000000 SkPy-0.9.1/skpy/event.py
+-rw-r--r--   0 user      (1000) user      (1000)    16454 2019-10-14 17:48:58.000000 SkPy-0.9.1/skpy/main.py
+-rw-r--r--   0 user      (1000) user      (1000)    31540 2019-10-14 17:48:58.000000 SkPy-0.9.1/skpy/msg.py
+-rw-r--r--   0 user      (1000) user      (1000)    21298 2019-10-14 17:48:58.000000 SkPy-0.9.1/skpy/user.py
+-rw-r--r--   0 user      (1000) user      (1000)    10165 2019-10-14 17:48:58.000000 SkPy-0.9.1/skpy/util.py
```

### Comparing `SkPy-0.9/PKG-INFO` & `SkPy-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 1.1
 Name: SkPy
-Version: 0.9
+Version: 0.9.1
 Summary: An unofficial Python library for interacting with the Skype HTTP API.
 Home-page: https://skpy.t.allofti.me
-Author: Terrance
+Author: Ollie Terrance
 Author-email: UNKNOWN
 License: UNKNOWN
-Download-URL: https://github.com/OllieTerrance/SkPy/releases
-Description-Content-Type: UNKNOWN
+Download-URL: https://github.com/Terrance/SkPy/releases
 Description: SkPy
         ====
         
         An unofficial Python library for interacting with the Skype HTTP API.
         
         Here be dragons
         ---------------
```

### Comparing `SkPy-0.9/README.rst` & `SkPy-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `SkPy-0.9/setup.py` & `SkPy-0.9.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup
 from os import path
 
 setup(name="SkPy",
       description="An unofficial Python library for interacting with the Skype HTTP API.",
       long_description=open(path.join(path.abspath(path.dirname(__file__)), "README.rst"), "r").read(),
-      author="Terrance",
-      version="0.9",
+      author="Ollie Terrance",
+      version="0.9.1",
       packages=["skpy"],
       install_requires=["beautifulsoup4", "requests"],
       tests_require=["beautifulsoup4", "requests", "responses"],
       url="https://skpy.t.allofti.me",
-      download_url="https://github.com/OllieTerrance/SkPy/releases",
+      download_url="https://github.com/Terrance/SkPy/releases",
       classifiers=["Development Status :: 4 - Beta",
                    "Intended Audience :: Developers",
                    "Topic :: Communications :: Chat",
                    "Topic :: Software Development :: Libraries"])
```

### Comparing `SkPy-0.9/skpy/chat.py` & `SkPy-0.9.1/skpy/chat.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime
 import re
 import time
 
-from .core import SkypeObj, SkypeObjs
+from .core import SkypeObj, SkypeObjs, SkypeApiException
 from .util import SkypeUtils
 from .conn import SkypeConnection
 from .msg import SkypeMsg
 
 
 @SkypeUtils.initAttrs
 class SkypeChat(SkypeObj):
@@ -43,14 +43,43 @@
         url = "{0}/users/ME/conversations/{1}/messages".format(self.skype.conn.msgsHost, self.id)
         params = {"startTime": 0,
                   "view": "msnp24Equivalent",
                   "targetType": "Passport|Skype|Lync|Thread"}
         resp = self.skype.conn.syncStateCall("GET", url, params, auth=SkypeConnection.Auth.RegToken).json()
         return [SkypeMsg.fromRaw(self.skype, json) for json in resp.get("messages", [])]
 
+    def createRaw(self, msg):
+        resp = self.skype.conn("POST", "{0}/users/ME/conversations/{1}/messages"
+                                       .format(self.skype.conn.msgsHost, self.id),
+                               auth=SkypeConnection.Auth.RegToken, json=msg)
+        url = resp.headers.get("Location")
+        msgId = url.rsplit("/", 1)[-1] if url else None
+        arriveTime = resp.json().get("OriginalArrivalTime")
+        return (msgId, arriveTime)
+
+    def editRaw(self, msgId, msg):
+        resp = self.skype.conn("PUT", "{0}/users/ME/conversations/{1}/messages/{2}"
+                                      .format(self.skype.conn.msgsHost, self.id, msgId),
+                               auth=SkypeConnection.Auth.RegToken, json=msg)
+        json = resp.json()
+        if "errorCode" in json:
+            raise SkypeApiException("Error code {0} from message edit".format(json["errorCode"]), resp)
+        else:
+            return json.get("edittime")
+
+    def deleteRaw(self, msgId):
+        resp = self.skype.conn("DELETE", "{0}/users/ME/conversations/{1}/messages/{2}"
+                                         .format(self.skype.conn.msgsHost, self.id, msgId),
+                               auth=SkypeConnection.Auth.RegToken)
+        json = resp.json()
+        if "errorCode" in json:
+            raise SkypeApiException("Error code {0} from message delete".format(json["errorCode"]), resp)
+        else:
+            return json.get("deletetime")
+
     def sendRaw(self, editId=None, **kwargs):
         """
         Send a raw message to the conversation.  At a minimum, values for ``content``, ``messagetype`` and
         ``contenttype`` should be provided.
 
         The message object returned here will not have a server-provided identifier (needed for acks), as the messages
         API does not provide it.  Note that message edits depend on the client identifier, which is included.
@@ -67,30 +96,38 @@
             Has-Mentions (str): whether the message mentions any other users
             kwargs (dict): any additional arguments not listed above
 
         Returns:
             .SkypeMsg: copy of the sent message object
         """
         msg = {"contenttype": "text", "messagetype": "Text"}
-        # Skype timestamps are integers and in milliseconds, whereas Python's are floats and in seconds.
-        clientTime = int(time.time() * 1000)
-        clientDate = datetime.fromtimestamp(clientTime / 1000)
-        msg["skypeeditedid" if editId else "clientmessageid"] = str(editId or clientTime)
         msg.update(kwargs)
-        arriveTime = self.skype.conn("POST", "{0}/users/ME/conversations/{1}/messages"
-                                             .format(self.skype.conn.msgsHost, self.id),
-                                     auth=SkypeConnection.Auth.RegToken, json=msg).json().get("OriginalArrivalTime")
+        if editId:
+            msgId = editId
+            clientTime = None
+            if msg.get("content"):
+                arriveTime = self.editRaw(editId, msg)
+            else:
+                arriveTime = self.deleteRaw(editId)
+        else:
+            # Skype timestamps are integers and in milliseconds, whereas Python's are floats and in seconds.
+            clientTime = int(time.time() * 1000)
+            msg["clientmessageid"] = str(clientTime)
+            msgId, arriveTime = self.createRaw(msg)
         arriveDate = datetime.fromtimestamp(arriveTime / 1000) if arriveTime else datetime.now()
-        msg.update({"composetime": datetime.strftime(clientDate, "%Y-%m-%dT%H:%M:%S.%fZ"),
+        msg.update({"id": msgId,
                     "conversationLink": "{0}/users/ME/conversations/{1}".format(self.skype.conn.msgsHost, self.id),
                     "from": "{0}/users/ME/contacts/8:{1}".format(self.skype.conn.msgsHost, self.skype.userId),
                     "imdisplayname": str(self.skype.user.name),
                     "isactive": True,
                     "originalarrivaltime": datetime.strftime(arriveDate, "%Y-%m-%dT%H:%M:%S.%fZ"),
                     "type": "Message"})
+        if clientTime:
+            clientDate = datetime.fromtimestamp(clientTime / 1000)
+            msg["composetime"] = datetime.strftime(clientDate, "%Y-%m-%dT%H:%M:%S.%fZ")
         if arriveTime:
             arriveDate = datetime.fromtimestamp(arriveTime / 1000)
             msg["originalarrivaltime"] = datetime.strftime(arriveDate, "%Y-%m-%dT%H:%M:%S.%fZ")
         return SkypeMsg.fromRaw(self.skype, msg)
 
     def setTyping(self, active=True):
         """
@@ -262,17 +299,17 @@
             Description of the conversation, shown to all participants.
         creator (:class:`.SkypeUser`):
             User who originally created the conversation.
         users (:class:`.SkypeUser` list):
             Users currently participating in the conversation.
         admins (:class:`.SkypeUser` list):
             Participants with admin privileges.
-        open (boolean):
+        open (bool):
             Whether new participants can join via a public join link.
-        history (boolean):
+        history (bool):
             Whether message history is provided to new participants.
         picture (str):
             URL to retrieve the conversation picture.
         joinUrl (str):
             Public ``join.skype.com`` URL for any other users to access the conversation.
     """
```

### Comparing `SkPy-0.9/skpy/conn.py` & `SkPy-0.9.1/skpy/conn.py`

 * *Files identical despite different names*

### Comparing `SkPy-0.9/skpy/core.py` & `SkPy-0.9.1/skpy/core.py`

 * *Files identical despite different names*

### Comparing `SkPy-0.9/skpy/event.py` & `SkPy-0.9.1/skpy/event.py`

 * *Files identical despite different names*

### Comparing `SkPy-0.9/skpy/main.py` & `SkPy-0.9.1/skpy/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,16 +272,15 @@
             Only allow from Skype users on the connected account's contact list.
         Privacy.Nobody
             Deny from all Skype users.
     """
 
     def __init__(self, skype=None, raw=None):
         super(SkypeSettings, self).__init__(skype, raw)
-        if skype and skype.conn.connected:
-            self.syncFlags()
+        self.flags = set()
 
     def syncFlags(self):
         """
         Update the cached list of all enabled flags, and store it in the :attr:`flags` attribute.
         """
         self.flags = set(self.skype.conn("GET", SkypeConnection.API_FLAGS,
                                          auth=SkypeConnection.Auth.SkypeToken).json())
```

### Comparing `SkPy-0.9/skpy/msg.py` & `SkPy-0.9.1/skpy/msg.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,15 +275,15 @@
             content (str): main message body
             me (bool): whether to send as an action, where the current account's name prefixes the message
             rich (bool): whether to send with rich text formatting
 
         Returns:
             .SkypeMsg: copy of the edited message object
         """
-        return self.chat.sendMsg(content, me, rich, self.clientId)
+        return self.chat.sendMsg(content, me, rich, self.id)
 
     def delete(self):
         """
         Delete the message and remove it from the conversation.
 
         Equivalent to calling :meth:`edit` with an empty ``content`` string.
```

### Comparing `SkPy-0.9/skpy/user.py` & `SkPy-0.9.1/skpy/user.py`

 * *Files identical despite different names*

### Comparing `SkPy-0.9/skpy/util.py` & `SkPy-0.9.1/skpy/util.py`

 * *Files identical despite different names*

### Comparing `SkPy-0.9/skpy/__init__.py` & `SkPy-0.9.1/skpy/__init__.py`

 * *Files identical despite different names*

### Comparing `SkPy-0.9/SkPy.egg-info/PKG-INFO` & `SkPy-0.9.1/SkPy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 1.1
 Name: SkPy
-Version: 0.9
+Version: 0.9.1
 Summary: An unofficial Python library for interacting with the Skype HTTP API.
 Home-page: https://skpy.t.allofti.me
-Author: Terrance
+Author: Ollie Terrance
 Author-email: UNKNOWN
 License: UNKNOWN
-Download-URL: https://github.com/OllieTerrance/SkPy/releases
-Description-Content-Type: UNKNOWN
+Download-URL: https://github.com/Terrance/SkPy/releases
 Description: SkPy
         ====
         
         An unofficial Python library for interacting with the Skype HTTP API.
         
         Here be dragons
         ---------------
```

