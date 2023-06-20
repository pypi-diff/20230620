# Comparing `tmp/xenoslib-0.1.29.1.tar.gz` & `tmp/xenoslib-0.1.29.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xenoslib-0.1.29.1.tar", last modified: Tue Jun 20 01:40:19 2023, max compression
+gzip compressed data, was "xenoslib-0.1.29.2.tar", last modified: Tue Jun 20 05:39:47 2023, max compression
```

## Comparing `xenoslib-0.1.29.1.tar` & `xenoslib-0.1.29.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:40:19.181737 xenoslib-0.1.29.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-20 01:40:06.000000 xenoslib-0.1.29.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-20 01:40:19.181737 xenoslib-0.1.29.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-20 01:40:06.000000 xenoslib-0.1.29.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 01:40:19.181737 xenoslib-0.1.29.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-20 01:40:06.000000 xenoslib-0.1.29.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:40:19.177737 xenoslib-0.1.29.1/xenoslib/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-20 01:40:06.000000 xenoslib-0.1.29.1/xenoslib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-20 01:40:06.000000 xenoslib-0.1.29.1/xenoslib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-20 01:40:06.000000 xenoslib-0.1.29.1/xenoslib/about.py
--rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-06-20 01:40:06.000000 xenoslib-0.1.29.1/xenoslib/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-20 01:40:06.000000 xenoslib-0.1.29.1/xenoslib/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-06-20 01:40:06.000000 xenoslib-0.1.29.1/xenoslib/extend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-20 01:40:06.000000 xenoslib-0.1.29.1/xenoslib/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-06-20 01:40:06.000000 xenoslib-0.1.29.1/xenoslib/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-20 01:40:06.000000 xenoslib-0.1.29.1/xenoslib/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-06-20 01:40:06.000000 xenoslib-0.1.29.1/xenoslib/onedrive.py
--rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-06-20 01:40:06.000000 xenoslib-0.1.29.1/xenoslib/win_trayicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-20 01:40:06.000000 xenoslib-0.1.29.1/xenoslib/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:40:19.181737 xenoslib-0.1.29.1/xenoslib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-20 01:40:19.000000 xenoslib-0.1.29.1/xenoslib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-20 01:40:19.000000 xenoslib-0.1.29.1/xenoslib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 01:40:19.000000 xenoslib-0.1.29.1/xenoslib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-20 01:40:19.000000 xenoslib-0.1.29.1/xenoslib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 01:40:19.000000 xenoslib-0.1.29.1/xenoslib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:39:47.467909 xenoslib-0.1.29.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-20 05:39:34.000000 xenoslib-0.1.29.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-20 05:39:47.467909 xenoslib-0.1.29.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-20 05:39:34.000000 xenoslib-0.1.29.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 05:39:47.467909 xenoslib-0.1.29.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-20 05:39:34.000000 xenoslib-0.1.29.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:39:47.467909 xenoslib-0.1.29.2/xenoslib/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-20 05:39:34.000000 xenoslib-0.1.29.2/xenoslib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-20 05:39:34.000000 xenoslib-0.1.29.2/xenoslib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-20 05:39:34.000000 xenoslib-0.1.29.2/xenoslib/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-06-20 05:39:34.000000 xenoslib-0.1.29.2/xenoslib/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-20 05:39:34.000000 xenoslib-0.1.29.2/xenoslib/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-06-20 05:39:34.000000 xenoslib-0.1.29.2/xenoslib/extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-20 05:39:34.000000 xenoslib-0.1.29.2/xenoslib/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-06-20 05:39:34.000000 xenoslib-0.1.29.2/xenoslib/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-20 05:39:34.000000 xenoslib-0.1.29.2/xenoslib/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-06-20 05:39:34.000000 xenoslib-0.1.29.2/xenoslib/onedrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-06-20 05:39:34.000000 xenoslib-0.1.29.2/xenoslib/win_trayicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-20 05:39:34.000000 xenoslib-0.1.29.2/xenoslib/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:39:47.467909 xenoslib-0.1.29.2/xenoslib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-20 05:39:47.000000 xenoslib-0.1.29.2/xenoslib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-20 05:39:47.000000 xenoslib-0.1.29.2/xenoslib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 05:39:47.000000 xenoslib-0.1.29.2/xenoslib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-20 05:39:47.000000 xenoslib-0.1.29.2/xenoslib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 05:39:47.000000 xenoslib-0.1.29.2/xenoslib.egg-info/top_level.txt
```

### Comparing `xenoslib-0.1.29.1/LICENSE` & `xenoslib-0.1.29.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.1/README.md` & `xenoslib-0.1.29.2/README.md`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.1/setup.py` & `xenoslib-0.1.29.2/setup.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.1/xenoslib/base.py` & `xenoslib-0.1.29.2/xenoslib/base.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.1/xenoslib/dev.py` & `xenoslib-0.1.29.2/xenoslib/dev.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.1/xenoslib/extend.py` & `xenoslib-0.1.29.2/xenoslib/extend.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.1/xenoslib/linux.py` & `xenoslib-0.1.29.2/xenoslib/linux.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.1/xenoslib/mail.py` & `xenoslib-0.1.29.2/xenoslib/mail.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,22 +80,22 @@
             body["payload"] = payload
             body["internal_date"] = msg[b"INTERNALDATE"]
             yield body
             self.msg_ids.append(msg_id)
 
     def fetch_emails(self):
         """Login and fetch emails."""
-        logger.debug(f"Fetching emails from the past {self.days} day(s)...")
-        date_str = datetime.datetime.today() - datetime.timedelta(days=self.days)
+        from_date = datetime.datetime.today() - datetime.timedelta(days=self.days)
+        logger.debug(f"Fetching emails since {from_date:%Y-%m-%d %H:%M:%S} ({self.days} days ago)")
         for i in range(3):
             try:
                 with IMAPClient(self.imap_server, timeout=30) as client:
                     client.login(self.mail_addr, self.mail_pwd)
                     client.select_folder("INBOX", readonly=True)
-                    messages = client.search(["SINCE", date_str])
+                    messages = client.search(["SINCE", from_date])
                     emails = client.fetch(messages, ["INTERNALDATE", "BODY.PEEK[]"])
                     return emails
             except Exception as exc:
                 logger.warning(exc)
         raise Exception("Reached maximum retry attempts. Giving up connection.")
```

### Comparing `xenoslib-0.1.29.1/xenoslib/mock.py` & `xenoslib-0.1.29.2/xenoslib/mock.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.1/xenoslib/onedrive.py` & `xenoslib-0.1.29.2/xenoslib/onedrive.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.1/xenoslib/win_trayicon.py` & `xenoslib-0.1.29.2/xenoslib/win_trayicon.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.1/xenoslib/windows.py` & `xenoslib-0.1.29.2/xenoslib/windows.py`

 * *Files identical despite different names*

