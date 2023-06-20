# Comparing `tmp/xenoslib-0.1.29.0.tar.gz` & `tmp/xenoslib-0.1.29.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xenoslib-0.1.29.0.tar", last modified: Fri Jun  9 05:47:21 2023, max compression
+gzip compressed data, was "xenoslib-0.1.29.1.tar", last modified: Tue Jun 20 01:40:19 2023, max compression
```

## Comparing `xenoslib-0.1.29.0.tar` & `xenoslib-0.1.29.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:47:21.372109 xenoslib-0.1.29.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-09 05:47:06.000000 xenoslib-0.1.29.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-09 05:47:21.372109 xenoslib-0.1.29.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-09 05:47:06.000000 xenoslib-0.1.29.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 05:47:21.372109 xenoslib-0.1.29.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-09 05:47:06.000000 xenoslib-0.1.29.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:47:21.372109 xenoslib-0.1.29.0/xenoslib/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-09 05:47:06.000000 xenoslib-0.1.29.0/xenoslib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-09 05:47:06.000000 xenoslib-0.1.29.0/xenoslib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-09 05:47:06.000000 xenoslib-0.1.29.0/xenoslib/about.py
--rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-06-09 05:47:06.000000 xenoslib-0.1.29.0/xenoslib/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-09 05:47:06.000000 xenoslib-0.1.29.0/xenoslib/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-06-09 05:47:06.000000 xenoslib-0.1.29.0/xenoslib/extend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-09 05:47:06.000000 xenoslib-0.1.29.0/xenoslib/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-09 05:47:06.000000 xenoslib-0.1.29.0/xenoslib/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-09 05:47:06.000000 xenoslib-0.1.29.0/xenoslib/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-06-09 05:47:06.000000 xenoslib-0.1.29.0/xenoslib/onedrive.py
--rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-06-09 05:47:06.000000 xenoslib-0.1.29.0/xenoslib/win_trayicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-09 05:47:06.000000 xenoslib-0.1.29.0/xenoslib/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 05:47:21.372109 xenoslib-0.1.29.0/xenoslib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-09 05:47:21.000000 xenoslib-0.1.29.0/xenoslib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-09 05:47:21.000000 xenoslib-0.1.29.0/xenoslib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 05:47:21.000000 xenoslib-0.1.29.0/xenoslib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-09 05:47:21.000000 xenoslib-0.1.29.0/xenoslib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 05:47:21.000000 xenoslib-0.1.29.0/xenoslib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:40:19.181737 xenoslib-0.1.29.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-20 01:40:06.000000 xenoslib-0.1.29.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-20 01:40:19.181737 xenoslib-0.1.29.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-20 01:40:06.000000 xenoslib-0.1.29.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 01:40:19.181737 xenoslib-0.1.29.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-20 01:40:06.000000 xenoslib-0.1.29.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:40:19.177737 xenoslib-0.1.29.1/xenoslib/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-20 01:40:06.000000 xenoslib-0.1.29.1/xenoslib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-20 01:40:06.000000 xenoslib-0.1.29.1/xenoslib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-20 01:40:06.000000 xenoslib-0.1.29.1/xenoslib/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-06-20 01:40:06.000000 xenoslib-0.1.29.1/xenoslib/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-20 01:40:06.000000 xenoslib-0.1.29.1/xenoslib/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-06-20 01:40:06.000000 xenoslib-0.1.29.1/xenoslib/extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-20 01:40:06.000000 xenoslib-0.1.29.1/xenoslib/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-06-20 01:40:06.000000 xenoslib-0.1.29.1/xenoslib/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-20 01:40:06.000000 xenoslib-0.1.29.1/xenoslib/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-06-20 01:40:06.000000 xenoslib-0.1.29.1/xenoslib/onedrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-06-20 01:40:06.000000 xenoslib-0.1.29.1/xenoslib/win_trayicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-20 01:40:06.000000 xenoslib-0.1.29.1/xenoslib/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:40:19.181737 xenoslib-0.1.29.1/xenoslib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-20 01:40:19.000000 xenoslib-0.1.29.1/xenoslib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-20 01:40:19.000000 xenoslib-0.1.29.1/xenoslib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 01:40:19.000000 xenoslib-0.1.29.1/xenoslib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-20 01:40:19.000000 xenoslib-0.1.29.1/xenoslib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 01:40:19.000000 xenoslib-0.1.29.1/xenoslib.egg-info/top_level.txt
```

### Comparing `xenoslib-0.1.29.0/LICENSE` & `xenoslib-0.1.29.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.0/README.md` & `xenoslib-0.1.29.1/README.md`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.0/setup.py` & `xenoslib-0.1.29.1/setup.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.0/xenoslib/base.py` & `xenoslib-0.1.29.1/xenoslib/base.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.0/xenoslib/dev.py` & `xenoslib-0.1.29.1/xenoslib/dev.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.0/xenoslib/extend.py` & `xenoslib-0.1.29.1/xenoslib/extend.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.0/xenoslib/linux.py` & `xenoslib-0.1.29.1/xenoslib/linux.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.0/xenoslib/mail.py` & `xenoslib-0.1.29.1/xenoslib/mail.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,77 +57,83 @@
             self.msg_ids.extend(mails.keys())
         return self.fetching(interval=interval, endless=endless)
 
     def fetching(self, interval=30, endless=True):
         """Continuously fetch emails at the specified interval."""
         logger.debug("Start checking emails...")
         while True:
-            try:
-                yield from self.parse_emails(self.fetch_emails())
-            except Exception as exc:
-                logger.warning(exc)
+            yield from self.parse_emails(self.fetch_emails())
             if not endless:
                 break
             sleep(interval)
 
     def parse_emails(self, emails):
         for msg_id, msg in emails.items():
             if msg_id in self.msg_ids:
                 continue
             body = email.message_from_bytes(msg[b"BODY[]"])
             subject = str(email.header.make_header(email.header.decode_header(body["Subject"])))
 
             payload = body.get_payload(decode=True)
             if payload:
                 payload = payload.decode()
-            internal_date = msg[b"INTERNALDATE"]
             body["subjectx"] = subject
             body["payload"] = payload
-            body["internal_date"] = internal_date
+            body["internal_date"] = msg[b"INTERNALDATE"]
             yield body
             self.msg_ids.append(msg_id)
 
     def fetch_emails(self):
         """Login and fetch emails."""
         logger.debug(f"Fetching emails from the past {self.days} day(s)...")
         date_str = datetime.datetime.today() - datetime.timedelta(days=self.days)
-        with IMAPClient(self.imap_server, timeout=30) as client:
-            client.login(self.mail_addr, self.mail_pwd)
-            client.select_folder("INBOX", readonly=True)
-            messages = client.search(["SINCE", date_str])
-            emails = client.fetch(messages, ["INTERNALDATE", "BODY.PEEK[]"])
-            return emails
+        for i in range(3):
+            try:
+                with IMAPClient(self.imap_server, timeout=30) as client:
+                    client.login(self.mail_addr, self.mail_pwd)
+                    client.select_folder("INBOX", readonly=True)
+                    messages = client.search(["SINCE", date_str])
+                    emails = client.fetch(messages, ["INTERNALDATE", "BODY.PEEK[]"])
+                    return emails
+            except Exception as exc:
+                logger.warning(exc)
+        raise Exception("Reached maximum retry attempts. Giving up connection.")
 
 
 class SMTPMail:
     def __init__(self, smtp_server="", sender="", password="", port=25):
         self.smtp_server = smtp_server
         self.port = int(port)
         self.sender = sender
         self.password = password
         if self.port == 465:  # use SSL by port
             self.SMTP = smtplib.SMTP_SSL
         else:
             self.SMTP = smtplib.SMTP
 
-    def send(self, subject, message, receiver, receivers=[], cc=[], bcc=[], filename=None):
+    def send(
+        self, subject, message, receiver=None, receivers=None, cc=None, bcc=None, filename=None
+    ):
+        if receivers is None:
+            receivers = []
         if isinstance(receiver, str):
             receivers.append(receiver)
         elif isinstance(receiver, (list, tuple)):
             receivers.extend(receiver)
         msg = MIMEMultipart()
         msg["Subject"] = Header(subject, "utf-8")
         msg["From"] = Header(self.sender, "utf-8")
         msg["To"] = ";".join(receivers)
-        msg["Cc"] = ";".join(cc)
+        if cc:
+            msg["Cc"] = ";".join(cc)
+            receivers.extend(cc)
+        if bcc:
+            receivers.extend(bcc)
         msg["Message-ID"] = make_msgid()
-        receivers.extend(cc)
-        receivers.extend(bcc)
         msg.attach(MIMEText(message, "html", "utf-8"))
-
         if filename:
             attachment = MIMEApplication(open(filename, "rb").read())
             attachment.add_header("Content-Disposition", "attachment", filename=filename)
             msg.attach(attachment)
 
         with self.SMTP(self.smtp_server, self.port) as smtp:
             print(smtp.has_extn("STARTTLS"))
```

### Comparing `xenoslib-0.1.29.0/xenoslib/mock.py` & `xenoslib-0.1.29.1/xenoslib/mock.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.0/xenoslib/onedrive.py` & `xenoslib-0.1.29.1/xenoslib/onedrive.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.0/xenoslib/win_trayicon.py` & `xenoslib-0.1.29.1/xenoslib/win_trayicon.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.29.0/xenoslib/windows.py` & `xenoslib-0.1.29.1/xenoslib/windows.py`

 * *Files identical despite different names*

