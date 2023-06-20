# Comparing `tmp/async_notify-0.9.4-py3-none-any.whl.zip` & `tmp/async_notify-1.0.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,54 +1,86 @@
-Zip file size: 37793 bytes, number of entries: 52
--rw-r--r--  2.0 unx      893 b- defN 23-Jun-06 16:48 notify/__init__.py
--rw-r--r--  2.0 unx     1105 b- defN 23-Jun-06 16:48 notify/exceptions.py
--rw-r--r--  2.0 unx     5070 b- defN 23-Jun-06 16:48 notify/models.py
--rw-r--r--  2.0 unx     2242 b- defN 23-Jun-06 16:48 notify/notify.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 16:48 notify/py.typed
--rw-r--r--  2.0 unx      582 b- defN 23-Jun-06 16:48 notify/settings.py
--rw-r--r--  2.0 unx     1963 b- defN 23-Jun-06 16:48 notify/templates.py
--rw-r--r--  2.0 unx      313 b- defN 23-Jun-06 16:48 notify/version.py
--rw-r--r--  2.0 unx       61 b- defN 23-Jun-06 16:48 notify/providers/__init__.py
--rw-r--r--  2.0 unx    11702 b- defN 23-Jun-06 16:48 notify/providers/abstract.py
--rw-r--r--  2.0 unx     8247 b- defN 23-Jun-06 16:48 notify/providers/mail.py
--rw-r--r--  2.0 unx      109 b- defN 23-Jun-06 16:48 notify/providers/aws/__init__.py
--rw-r--r--  2.0 unx     1567 b- defN 23-Jun-06 16:48 notify/providers/aws/aws.py
--rw-r--r--  2.0 unx      355 b- defN 23-Jun-06 16:48 notify/providers/aws/settings.py
--rw-r--r--  2.0 unx      112 b- defN 23-Jun-06 16:48 notify/providers/dummy/__init__.py
--rw-r--r--  2.0 unx     1206 b- defN 23-Jun-06 16:48 notify/providers/dummy/dummy.py
--rw-r--r--  2.0 unx       97 b- defN 23-Jun-06 16:48 notify/providers/email/__init__.py
--rw-r--r--  2.0 unx     1861 b- defN 23-Jun-06 16:48 notify/providers/email/email.py
--rw-r--r--  2.0 unx      244 b- defN 23-Jun-06 16:48 notify/providers/email/settings.py
--rw-r--r--  2.0 unx      120 b- defN 23-Jun-06 16:48 notify/providers/gmail/__init__.py
--rw-r--r--  2.0 unx     3282 b- defN 23-Jun-06 16:48 notify/providers/gmail/gmail.py
--rw-r--r--  2.0 unx      130 b- defN 23-Jun-06 16:48 notify/providers/gmail/settings.py
--rw-r--r--  2.0 unx      156 b- defN 23-Jun-06 16:48 notify/providers/office365/__init__.py
--rw-r--r--  2.0 unx     4600 b- defN 23-Jun-06 16:48 notify/providers/office365/office365.py
--rw-r--r--  2.0 unx      269 b- defN 23-Jun-06 16:48 notify/providers/office365/settings.py
--rw-r--r--  2.0 unx      127 b- defN 23-Jun-06 16:48 notify/providers/onesignal/__init__.py
--rw-r--r--  2.0 unx     2741 b- defN 23-Jun-06 16:48 notify/providers/onesignal/onesignal.py
--rw-r--r--  2.0 unx      252 b- defN 23-Jun-06 16:48 notify/providers/onesignal/settings.py
--rw-r--r--  2.0 unx      105 b- defN 23-Jun-06 16:48 notify/providers/sendgrid/__init__.py
--rw-r--r--  2.0 unx     1116 b- defN 23-Jun-06 16:48 notify/providers/sendgrid/sendgrid.py
--rw-r--r--  2.0 unx      127 b- defN 23-Jun-06 16:48 notify/providers/sendgrid/settings.py
--rw-r--r--  2.0 unx      100 b- defN 23-Jun-06 16:48 notify/providers/slack/__init__.py
--rw-r--r--  2.0 unx      406 b- defN 23-Jun-06 16:48 notify/providers/slack/settings.py
--rw-r--r--  2.0 unx     4282 b- defN 23-Jun-06 16:48 notify/providers/slack/slack.py
--rw-r--r--  2.0 unx    12741 b- defN 23-Jun-06 16:48 notify/providers/telegram/Telegram.py
--rw-r--r--  2.0 unx      124 b- defN 23-Jun-06 16:48 notify/providers/telegram/__init__.py
--rw-r--r--  2.0 unx      157 b- defN 23-Jun-06 16:48 notify/providers/telegram/settings.py
--rw-r--r--  2.0 unx      115 b- defN 23-Jun-06 16:48 notify/providers/twilio/__init__.py
--rw-r--r--  2.0 unx      199 b- defN 23-Jun-06 16:48 notify/providers/twilio/settings.py
--rw-r--r--  2.0 unx     2137 b- defN 23-Jun-06 16:48 notify/providers/twilio/twilio.py
--rw-r--r--  2.0 unx      114 b- defN 23-Jun-06 16:48 notify/providers/twitter/__init__.py
--rw-r--r--  2.0 unx      286 b- defN 23-Jun-06 16:48 notify/providers/twitter/settings.py
--rw-r--r--  2.0 unx     2862 b- defN 23-Jun-06 16:48 notify/providers/twitter/twitter.py
--rw-r--r--  2.0 unx      108 b- defN 23-Jun-06 16:48 notify/providers/xmpp/__init__.py
--rw-r--r--  2.0 unx      133 b- defN 23-Jun-06 16:48 notify/providers/xmpp/settings.py
--rw-r--r--  2.0 unx     5813 b- defN 23-Jun-06 16:48 notify/providers/xmpp/xmpp.py
--rw-r--r--  2.0 unx      167 b- defN 23-Jun-06 16:48 notify/utils/__init__.py
--rw-r--r--  2.0 unx     1509 b- defN 23-Jun-06 16:49 async_notify-0.9.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     3783 b- defN 23-Jun-06 16:49 async_notify-0.9.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-06 16:49 async_notify-0.9.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jun-06 16:49 async_notify-0.9.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     4511 b- defN 23-Jun-06 16:49 async_notify-0.9.4.dist-info/RECORD
-52 files, 90400 bytes uncompressed, 30545 bytes compressed:  66.2%
+Zip file size: 457154 bytes, number of entries: 84
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 15:32 async_notify-1.0.0.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 15:32 notify/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 15:32 async_notify.libs/
+-rw-r--r--  2.0 unx     5103 b- defN 23-Jun-20 15:32 async_notify-1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx     1509 b- defN 23-Jun-20 15:32 async_notify-1.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      148 b- defN 23-Jun-20 15:32 async_notify-1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-20 15:32 async_notify-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     5353 b- defN 23-Jun-20 15:32 async_notify-1.0.0.dist-info/RECORD
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-20 15:32 async_notify-1.0.0.dist-info/entry_points.txt
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 15:32 notify/utils/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 15:32 notify/types/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 15:32 notify/providers/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 15:32 notify/tests/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 15:32 notify/server/
+-rw-r--r--  2.0 unx     2634 b- defN 23-Jun-20 15:32 notify/notify.py
+-rw-r--r--  2.0 unx     3259 b- defN 23-Jun-20 15:32 notify/conf.py
+-rw-r--r--  2.0 unx      368 b- defN 23-Jun-20 15:32 notify/__init__.py
+-rw-r--r--  2.0 unx     4259 b- defN 23-Jun-20 15:32 notify/templates.py
+-rw-r--r--  2.0 unx     1233 b- defN 23-Jun-20 15:32 notify/exceptions.pyx
+-rw-r--r--  2.0 unx     5303 b- defN 23-Jun-20 15:32 notify/models.py
+-rw-r--r--  2.0 unx      754 b- defN 23-Jun-20 15:32 notify/exceptions.pxd
+-rw-r--r--  2.0 unx   434902 b- defN 23-Jun-20 15:32 notify/exceptions.c
+-rwxr-xr-x  2.0 unx   640736 b- defN 23-Jun-20 15:32 notify/exceptions.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx     1429 b- defN 23-Jun-20 15:32 notify/__main__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-20 15:32 notify/py.typed
+-rw-r--r--  2.0 unx      366 b- defN 23-Jun-20 15:32 notify/version.py
+-rw-r--r--  2.0 unx       75 b- defN 23-Jun-20 15:32 notify/utils/__init__.py
+-rw-r--r--  2.0 unx     2333 b- defN 23-Jun-20 15:32 notify/utils/functions.py
+-rw-r--r--  2.0 unx       85 b- defN 23-Jun-20 15:32 notify/types/__init__.py
+-rw-r--r--  2.0 unx     2249 b- defN 23-Jun-20 15:32 notify/types/typedefs.pyx
+-rwxr-xr-x  2.0 unx   500664 b- defN 23-Jun-20 15:32 notify/types/typedefs.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx   355539 b- defN 23-Jun-20 15:32 notify/types/typedefs.c
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 15:32 notify/providers/smtp/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 15:32 notify/providers/xmpp/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 15:32 notify/providers/aws/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 15:32 notify/providers/office365/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 15:32 notify/providers/onesignal/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 15:32 notify/providers/twilio/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 15:32 notify/providers/email/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 15:32 notify/providers/twitter/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 15:32 notify/providers/outlook/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 15:32 notify/providers/sendgrid/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 15:32 notify/providers/gmail/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 15:32 notify/providers/telegram/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 15:32 notify/providers/dummy/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-20 15:32 notify/providers/slack/
+-rw-r--r--  2.0 unx       61 b- defN 23-Jun-20 15:32 notify/providers/__init__.py
+-rw-r--r--  2.0 unx    11943 b- defN 23-Jun-20 15:32 notify/providers/base.py
+-rw-r--r--  2.0 unx     1465 b- defN 23-Jun-20 15:32 notify/providers/message.py
+-rw-r--r--  2.0 unx     9152 b- defN 23-Jun-20 15:32 notify/providers/mail.py
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-20 15:32 notify/providers/smtp/__init__.py
+-rw-r--r--  2.0 unx     8557 b- defN 23-Jun-20 15:32 notify/providers/smtp/smtp.py
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-20 15:32 notify/providers/xmpp/__init__.py
+-rw-r--r--  2.0 unx     6186 b- defN 23-Jun-20 15:32 notify/providers/xmpp/xmpp.py
+-rw-r--r--  2.0 unx      109 b- defN 23-Jun-20 15:32 notify/providers/aws/__init__.py
+-rw-r--r--  2.0 unx     1572 b- defN 23-Jun-20 15:32 notify/providers/aws/aws.py
+-rw-r--r--  2.0 unx      156 b- defN 23-Jun-20 15:32 notify/providers/office365/__init__.py
+-rw-r--r--  2.0 unx     7047 b- defN 23-Jun-20 15:32 notify/providers/office365/office365.py
+-rw-r--r--  2.0 unx      127 b- defN 23-Jun-20 15:32 notify/providers/onesignal/__init__.py
+-rw-r--r--  2.0 unx     2742 b- defN 23-Jun-20 15:32 notify/providers/onesignal/onesignal.py
+-rw-r--r--  2.0 unx      115 b- defN 23-Jun-20 15:32 notify/providers/twilio/__init__.py
+-rw-r--r--  2.0 unx     2214 b- defN 23-Jun-20 15:32 notify/providers/twilio/twilio.py
+-rw-r--r--  2.0 unx       97 b- defN 23-Jun-20 15:32 notify/providers/email/__init__.py
+-rw-r--r--  2.0 unx     1866 b- defN 23-Jun-20 15:32 notify/providers/email/email.py
+-rw-r--r--  2.0 unx      114 b- defN 23-Jun-20 15:32 notify/providers/twitter/__init__.py
+-rw-r--r--  2.0 unx     2928 b- defN 23-Jun-20 15:32 notify/providers/twitter/twitter.py
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-20 15:32 notify/providers/outlook/__init__.py
+-rw-r--r--  2.0 unx     5957 b- defN 23-Jun-20 15:32 notify/providers/outlook/outlook.py
+-rw-r--r--  2.0 unx      105 b- defN 23-Jun-20 15:32 notify/providers/sendgrid/__init__.py
+-rw-r--r--  2.0 unx     1119 b- defN 23-Jun-20 15:32 notify/providers/sendgrid/sendgrid.py
+-rw-r--r--  2.0 unx      120 b- defN 23-Jun-20 15:32 notify/providers/gmail/__init__.py
+-rw-r--r--  2.0 unx     3353 b- defN 23-Jun-20 15:32 notify/providers/gmail/gmail.py
+-rw-r--r--  2.0 unx      124 b- defN 23-Jun-20 15:32 notify/providers/telegram/__init__.py
+-rw-r--r--  2.0 unx    13410 b- defN 23-Jun-20 15:32 notify/providers/telegram/Telegram.py
+-rw-r--r--  2.0 unx      112 b- defN 23-Jun-20 15:32 notify/providers/dummy/__init__.py
+-rw-r--r--  2.0 unx     1206 b- defN 23-Jun-20 15:32 notify/providers/dummy/dummy.py
+-rw-r--r--  2.0 unx      100 b- defN 23-Jun-20 15:32 notify/providers/slack/__init__.py
+-rw-r--r--  2.0 unx     4291 b- defN 23-Jun-20 15:32 notify/providers/slack/slack.py
+-rw-r--r--  2.0 unx       31 b- defN 23-Jun-20 15:32 notify/tests/__init__.py
+-rw-r--r--  2.0 unx     1309 b- defN 23-Jun-20 15:32 notify/tests/base.py
+-rw-r--r--  2.0 unx    10506 b- defN 23-Jun-20 15:32 notify/server/__init__.py
+-rw-r--r--  2.0 unx     2874 b- defN 23-Jun-20 15:32 notify/server/wrapper.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-20 15:32 notify/server/py.typed
+-rw-r--r--  2.0 unx     4897 b- defN 23-Jun-20 15:32 notify/server/queue.py
+84 files, 2074582 bytes uncompressed, 446148 bytes compressed:  78.5%
```

## zipnote {}

```diff
@@ -1,157 +1,253 @@
-Filename: notify/__init__.py
+Filename: async_notify-1.0.0.dist-info/
 Comment: 
 
-Filename: notify/exceptions.py
+Filename: notify/
 Comment: 
 
-Filename: notify/models.py
+Filename: async_notify.libs/
+Comment: 
+
+Filename: async_notify-1.0.0.dist-info/METADATA
+Comment: 
+
+Filename: async_notify-1.0.0.dist-info/LICENSE
+Comment: 
+
+Filename: async_notify-1.0.0.dist-info/WHEEL
+Comment: 
+
+Filename: async_notify-1.0.0.dist-info/top_level.txt
+Comment: 
+
+Filename: async_notify-1.0.0.dist-info/RECORD
+Comment: 
+
+Filename: async_notify-1.0.0.dist-info/entry_points.txt
+Comment: 
+
+Filename: notify/utils/
+Comment: 
+
+Filename: notify/types/
+Comment: 
+
+Filename: notify/providers/
+Comment: 
+
+Filename: notify/tests/
+Comment: 
+
+Filename: notify/server/
 Comment: 
 
 Filename: notify/notify.py
 Comment: 
 
-Filename: notify/py.typed
+Filename: notify/conf.py
 Comment: 
 
-Filename: notify/settings.py
+Filename: notify/__init__.py
 Comment: 
 
 Filename: notify/templates.py
 Comment: 
 
+Filename: notify/exceptions.pyx
+Comment: 
+
+Filename: notify/models.py
+Comment: 
+
+Filename: notify/exceptions.pxd
+Comment: 
+
+Filename: notify/exceptions.c
+Comment: 
+
+Filename: notify/exceptions.cpython-39-x86_64-linux-gnu.so
+Comment: 
+
+Filename: notify/__main__.py
+Comment: 
+
+Filename: notify/py.typed
+Comment: 
+
 Filename: notify/version.py
 Comment: 
 
-Filename: notify/providers/__init__.py
+Filename: notify/utils/__init__.py
 Comment: 
 
-Filename: notify/providers/abstract.py
+Filename: notify/utils/functions.py
 Comment: 
 
-Filename: notify/providers/mail.py
+Filename: notify/types/__init__.py
 Comment: 
 
-Filename: notify/providers/aws/__init__.py
+Filename: notify/types/typedefs.pyx
 Comment: 
 
-Filename: notify/providers/aws/aws.py
+Filename: notify/types/typedefs.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: notify/providers/aws/settings.py
+Filename: notify/types/typedefs.c
 Comment: 
 
-Filename: notify/providers/dummy/__init__.py
+Filename: notify/providers/smtp/
 Comment: 
 
-Filename: notify/providers/dummy/dummy.py
+Filename: notify/providers/xmpp/
 Comment: 
 
-Filename: notify/providers/email/__init__.py
+Filename: notify/providers/aws/
 Comment: 
 
-Filename: notify/providers/email/email.py
+Filename: notify/providers/office365/
 Comment: 
 
-Filename: notify/providers/email/settings.py
+Filename: notify/providers/onesignal/
 Comment: 
 
-Filename: notify/providers/gmail/__init__.py
+Filename: notify/providers/twilio/
 Comment: 
 
-Filename: notify/providers/gmail/gmail.py
+Filename: notify/providers/email/
 Comment: 
 
-Filename: notify/providers/gmail/settings.py
+Filename: notify/providers/twitter/
 Comment: 
 
-Filename: notify/providers/office365/__init__.py
+Filename: notify/providers/outlook/
 Comment: 
 
-Filename: notify/providers/office365/office365.py
+Filename: notify/providers/sendgrid/
 Comment: 
 
-Filename: notify/providers/office365/settings.py
+Filename: notify/providers/gmail/
 Comment: 
 
-Filename: notify/providers/onesignal/__init__.py
+Filename: notify/providers/telegram/
 Comment: 
 
-Filename: notify/providers/onesignal/onesignal.py
+Filename: notify/providers/dummy/
 Comment: 
 
-Filename: notify/providers/onesignal/settings.py
+Filename: notify/providers/slack/
 Comment: 
 
-Filename: notify/providers/sendgrid/__init__.py
+Filename: notify/providers/__init__.py
 Comment: 
 
-Filename: notify/providers/sendgrid/sendgrid.py
+Filename: notify/providers/base.py
 Comment: 
 
-Filename: notify/providers/sendgrid/settings.py
+Filename: notify/providers/message.py
 Comment: 
 
-Filename: notify/providers/slack/__init__.py
+Filename: notify/providers/mail.py
 Comment: 
 
-Filename: notify/providers/slack/settings.py
+Filename: notify/providers/smtp/__init__.py
 Comment: 
 
-Filename: notify/providers/slack/slack.py
+Filename: notify/providers/smtp/smtp.py
 Comment: 
 
-Filename: notify/providers/telegram/Telegram.py
+Filename: notify/providers/xmpp/__init__.py
 Comment: 
 
-Filename: notify/providers/telegram/__init__.py
+Filename: notify/providers/xmpp/xmpp.py
 Comment: 
 
-Filename: notify/providers/telegram/settings.py
+Filename: notify/providers/aws/__init__.py
 Comment: 
 
-Filename: notify/providers/twilio/__init__.py
+Filename: notify/providers/aws/aws.py
+Comment: 
+
+Filename: notify/providers/office365/__init__.py
+Comment: 
+
+Filename: notify/providers/office365/office365.py
+Comment: 
+
+Filename: notify/providers/onesignal/__init__.py
 Comment: 
 
-Filename: notify/providers/twilio/settings.py
+Filename: notify/providers/onesignal/onesignal.py
+Comment: 
+
+Filename: notify/providers/twilio/__init__.py
 Comment: 
 
 Filename: notify/providers/twilio/twilio.py
 Comment: 
 
-Filename: notify/providers/twitter/__init__.py
+Filename: notify/providers/email/__init__.py
 Comment: 
 
-Filename: notify/providers/twitter/settings.py
+Filename: notify/providers/email/email.py
+Comment: 
+
+Filename: notify/providers/twitter/__init__.py
 Comment: 
 
 Filename: notify/providers/twitter/twitter.py
 Comment: 
 
-Filename: notify/providers/xmpp/__init__.py
+Filename: notify/providers/outlook/__init__.py
 Comment: 
 
-Filename: notify/providers/xmpp/settings.py
+Filename: notify/providers/outlook/outlook.py
 Comment: 
 
-Filename: notify/providers/xmpp/xmpp.py
+Filename: notify/providers/sendgrid/__init__.py
 Comment: 
 
-Filename: notify/utils/__init__.py
+Filename: notify/providers/sendgrid/sendgrid.py
+Comment: 
+
+Filename: notify/providers/gmail/__init__.py
+Comment: 
+
+Filename: notify/providers/gmail/gmail.py
+Comment: 
+
+Filename: notify/providers/telegram/__init__.py
+Comment: 
+
+Filename: notify/providers/telegram/Telegram.py
+Comment: 
+
+Filename: notify/providers/dummy/__init__.py
+Comment: 
+
+Filename: notify/providers/dummy/dummy.py
+Comment: 
+
+Filename: notify/providers/slack/__init__.py
+Comment: 
+
+Filename: notify/providers/slack/slack.py
+Comment: 
+
+Filename: notify/tests/__init__.py
 Comment: 
 
-Filename: async_notify-0.9.4.dist-info/LICENSE
+Filename: notify/tests/base.py
 Comment: 
 
-Filename: async_notify-0.9.4.dist-info/METADATA
+Filename: notify/server/__init__.py
 Comment: 
 
-Filename: async_notify-0.9.4.dist-info/WHEEL
+Filename: notify/server/wrapper.py
 Comment: 
 
-Filename: async_notify-0.9.4.dist-info/top_level.txt
+Filename: notify/server/py.typed
 Comment: 
 
-Filename: async_notify-0.9.4.dist-info/RECORD
+Filename: notify/server/queue.py
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## notify/__init__.py

```diff
@@ -1,41 +1,18 @@
 # -*- coding: utf-8 -*-
 """Async-Notify.
 
 Asyncio-based Notifications connectors for NAV.
 """
 import asyncio
-import pkgutil
-from pathlib import Path
 import uvloop
-from notify.settings import TEMPLATE_DIR
-from notify.templates import TemplateParser
-from notify.providers.abstract import ProviderType
-from .notify import PROVIDERS, Notify, LoadProvider
-
-from .version import (
-    __title__,
-    __description__,
-    __version__,
-    __author__,
-    __author_email__,
-)
-
-## more information
-__copyright__ = "Copyright (c) 2020-2022 Jesus Lara"
-__license__ = "BSD"
+from .providers.base import ProviderType
+from .notify import Notify
 
 # install uvloop and set as default loop for asyncio.
 asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
+uvloop.install()
 
 __all__ = (
-    "PROVIDERS",
     "Notify",
-    "LoadProvider",
     "ProviderType",
 )
-TemplateEnv = None
-
-
-if __name__ == "notify":
-    # loading template parser:
-    TemplateEnv = TemplateParser(directory=TEMPLATE_DIR)
```

## notify/models.py

```diff
@@ -5,15 +5,20 @@
 from dataclasses import InitVar
 from typing import Any, Union
 from email.parser import Parser
 from email.policy import default as policy_default
 from datamodel import BaseModel, Column, Field
 
 
-CONTENT_TYPES = ["text/plain", "text/html", "multipart/alternative", "application/json"]
+CONTENT_TYPES = [
+    "text/plain",
+    "text/html",
+    "multipart/alternative",
+    "application/json"
+]
 
 
 def auto_uuid(*args, **kwargs):  # pylint: disable=W0613
     return uuid.uuid4()
 
 
 def now():
@@ -23,20 +28,24 @@
 class Account(BaseModel):
     """
     Attributes for using a Provider by an User (Actor)
     """
 
     provider: str = Column(required=True, default="dummy")
     enabled: bool = Column(required=True, default=True)
-    address: Union[str, list] = Column(required=False, default="")
-    phone: Union[str, list] = Column(required=False, default="")
+    address: Union[str, list[str]] = Column(required=False, default_factory=list)
+    number: Union[str, list[str]] = Column(required=False, default_factory=list)
     userid: str = Column(required=False, default="")
+    attributes: dict = Column(required=False, default_factory=dict)
 
-    def set_address(self, address: str):
-        self.address = address
+    def set_address(self, address: Union[str, list[str]]):
+        if isinstance(address, str):
+            self.address = [address]
+        else:
+            self.address = address
 
 
 class Actor(BaseModel):
     """
     Basic Actor (meta-definition), can be an Sender or a Recipient
     """
 
@@ -59,15 +68,15 @@
 
     chat_name: str = Column(required=False)
     chat_id: str = Column(required=True, primary_key=True)
 
 
 class Channel(BaseModel):
     """
-    Basic configuration for Channel (group) notifications.
+    Basic configuration for Channel (Group-based) notifications.
     """
 
     channel_name: str = Column(required=False)
     channel_id: str = Column(required=True, primary_key=True)
 
 
 class Message(BaseModel):
```

## notify/notify.py

```diff
@@ -1,72 +1,87 @@
-import logging
 import importlib
-from .exceptions import ProviderError, notifyException
+from navconfig.logging import logger
+from .providers.base import ProviderBase
+from .exceptions import ProviderError, NotifyException
+from .conf import TEMPLATE_DIR
+from .templates import TemplateParser
 
-PROVIDERS = {}
 
+PROVIDERS = {}
+TemplateEnv = None
 
 class Notify:
     """Notify
 
         Factory object for getting a new Notification Provider.
     Args:
         provider (str): Name of the provider.
 
     Raises:
         ProviderError: when a driver cannot be loaded.
         NotSupported: when a method is not supported.
     Returns:
         ProviderBase: a Notify Provider.
     """
-
-    def __new__(cls, provider: str, *args, **kwargs):
+    def __new__(cls: type['ProviderBase'], provider: str, *args, **kwargs):
         _provider = None
         try:
-            if not provider in PROVIDERS:
-                obj = LoadProvider(provider)
-                PROVIDERS[provider] = obj
+            if provider not in PROVIDERS:
+                PROVIDERS[provider] = LoadProvider(provider)
             obj = PROVIDERS[provider]
             _provider = obj(*args, **kwargs)
-            logging.debug(f":: Load Provider: {provider}")
+            logger.debug(
+                f":: Load Provider: {provider}"
+            )
             return _provider
         except Exception as ex:
-            logging.exception(f"Cannot Load provider {provider}: {ex}")
+            logger.critical(
+                f"Cannot Load provider {provider}: {ex}"
+            )
             raise ProviderError(
                 message=f"Cannot Load provider {provider}: {ex}"
             ) from ex
 
     @classmethod
-    def provider(cls, provider, *args, **kwargs):
+    def provider(cls: type['ProviderBase'], provider: str, *args, **kwargs):
         try:
-            if not provider in PROVIDERS:
-                obj = LoadProvider(provider)
-                PROVIDERS[provider] = obj
+            if provider not in PROVIDERS:
+                PROVIDERS[provider] = LoadProvider(provider)
             obj = PROVIDERS[provider]
             _provider = obj(*args, **kwargs)
-            logging.debug(f":: Load Provider: {provider}")
+            logger.debug(
+                f":: Loaded Provider: {provider}"
+            )
             return _provider
         except Exception as ex:
-            logging.exception(f"Cannot Load provider {provider}: {ex}")
+            logger.critical(
+                f"Cannot Load provider {provider}: {ex}"
+            )
             raise ProviderError(
                 message=f"Cannot Load provider {provider}: {ex}"
             ) from ex
 
 
-def LoadProvider(provider):
+def LoadProvider(provider: str):
     """
     loadProvider.
-
-    Dynamically load a defined provider
+    Dynamically load a Notify provider
     """
     try:
-        # try to using importlib
         classpath = f"notify.providers.{provider}"
         module = importlib.import_module(classpath, package="providers")
-        obj = getattr(module, provider.capitalize())
-        return obj
+        return getattr(module, provider.capitalize())
     except ImportError:
         try:
             obj = __import__(classpath, fromlist=[provider])
             return obj
-        except ImportError as e:
-            raise notifyException(f"Error: No Provider {provider} was Found") from e
+        except ImportError as exc:
+            raise NotifyException(
+                f"Error: No Provider {provider} was Found: {exc}"
+            ) from exc
+
+
+if __name__ == "notify.notify":
+    # loading template parser:
+    TemplateEnv = TemplateParser(
+        directory=TEMPLATE_DIR
+    )
```

## notify/templates.py

```diff
@@ -1,58 +1,130 @@
 from pathlib import Path
 from typing import Optional
-from jinja2 import Environment, FileSystemLoader
-
-
-jinja_config = {"enable_async": False, "extensions": ["jinja2.ext.i18n"]}
+from collections.abc import Callable
+from navconfig import config
+from jinja2 import Environment, FileSystemLoader, TemplateError, TemplateNotFound
+
+jinja_config = {
+    "enable_async": True,
+    "extensions": ["jinja2.ext.i18n", "jinja2.ext.loopcontrols"],
+}
 
 
 class TemplateParser:
     """
     TemplateParser.
 
     This is a wrapper for the Jinja2 template engine.
     """
 
-    def __init__(self, directory: Path, **kwargs):
+    def __init__(
+        self,
+        directory: Path,
+        filters: Optional[list] = None,
+        **kwargs
+    ):
         self.template = None
         self.path = directory.resolve()
+        self.filters = filters
         if not self.path.exists():
-            raise RuntimeError(f"Notify: template directory {directory} does not exist")
+            raise RuntimeError(
+                f"Notify: template directory {directory} does not exist"
+            )
         if "config" in kwargs:
             self.config = {**jinja_config, **kwargs["config"]}
         else:
             self.config = jinja_config
+        template_debug = config.getboolean(
+            "TEMPLATE_DEBUG", fallback=False
+        )
+        if template_debug is True:
+            self.config["extensions"].append("jinja2.ext.debug")
         # creating loader:
-        templateLoader = FileSystemLoader(searchpath=[str(self.path)])
+        templateLoader = FileSystemLoader(
+            searchpath=[str(self.path)]
+        )
         # initialize the environment
         try:
             # TODO: check the bug ,encoding='ANSI'
-            self.env = Environment(loader=templateLoader, **self.config)
+            self.env: Optional[Environment] = Environment(
+                loader=templateLoader, **self.config
+            )
             # compiled_path = BytesIO()
-            compiled_path = str(self.path.joinpath(".compiled"))
-            self.env.compile_templates(target=compiled_path, zip="deflated")
+            compiled_path = str(
+                self.path.joinpath(".compiled")
+            )
+            self.env.compile_templates(
+                target=compiled_path, zip="deflated"
+            )
         except Exception as err:
             raise RuntimeError(
                 f"Notify: Error loading Template Environment: {err}"
             ) from err
+        ### adding custom filters:
+        if self.filters is not None:
+            self.env.filters.update(self.filters)
 
     def get_template(self, filename: str):
-        self.template = self.env.get_template(str(filename))
-        return self.template
+        """
+        Get a template from Template Environment using the Filename.
+        """
+        try:
+            self.template = self.env.get_template(str(filename))
+            return self.template
+        except TemplateNotFound as ex:
+            raise FileNotFoundError(
+                f"Template cannot be found: {filename}"
+            ) from ex
+        except Exception as ex:
+            raise RuntimeError(
+                f"Error parsing Template {filename}: {ex}"
+            ) from ex
 
     @property
     def environment(self):
         return self.env
 
+    def add_filter(self, func: Callable, name: Optional[str] = None) -> None:
+        """add_filter.
+        Register a custom function as Template Filter.
+        """
+        if name is not None:
+            filter_name = name
+        elif callable(func):
+            filter_name = name.__name__
+        else:
+            raise TypeError(f"Template Filter must be a callable function: {func!r}")
+        self.env.filters[filter_name] = func
+
     def render(self, filename: str, params: Optional[dict] = None) -> str:
         if not params:
             params = {}
         result = None
         try:
             self.template = self.env.get_template(str(filename))
             result = self.template.render(**params)
             return result
         except Exception as err:
             raise RuntimeError(
                 f"Notify: Error rendering template: {filename}, error: {err}"
             ) from err
+
+    async def render_async(self, filename: str, params: Optional[dict] = None) -> str:
+        """Render.
+        Renders a Jinja2 template using async-await syntax.
+        """
+        result = None
+        if not params:
+            params = {}
+        try:
+            template = self.env.get_template(str(filename))
+            result = await template.render_async(**params)
+            return result
+        except TemplateError as ex:
+            raise ValueError(
+                f"Template parsing error, template: {filename}: {ex}"
+            ) from ex
+        except Exception as err:
+            raise RuntimeError(
+                f"NAV: Error rendering: {filename}, error: {err}"
+            ) from err
```

## notify/version.py

```diff
@@ -1,11 +1,12 @@
 """Notify Meta information."""
 
 __title__ = "async-notify"
 __description__ = (
     "Library for send notifications. "
     "simple and powerful asyncio-based library for sending notifications."
 )
-__version__ = "0.9.4"
+__version__ = "1.0.0"
+__copyright__ = "Copyright (c) 2020-2023 Jesus Lara"
 __author__ = "Jesus Lara"
 __author_email__ = "jesuslara@phenobarbital.info"
 __license__ = "BSD"
```

## notify/providers/mail.py

```diff
@@ -2,37 +2,38 @@
 import os
 import ssl
 import asyncio
 from abc import ABC
 from typing import Union, Any
 from collections.abc import Callable
 from email import encoders
-
 # from email.message import EmailMessage
 from email.mime.multipart import MIMEMultipart
 from email.mime.base import MIMEBase
 from email.mime.text import MIMEText
 from email.mime.image import MIMEImage
 from email.utils import formatdate
+from functools import partial
 import aiosmtplib
 from notify.models import Actor
 from notify.exceptions import ProviderError
-
 # abstract class
-from .abstract import ProviderBase, ProviderType
+from .base import ProviderBase, ProviderType
 
 
 class ProviderEmail(ProviderBase, ABC):
     """
     ProviderEmail.
 
     Base class for All Email-based providers
     """
 
     provider_type = ProviderType.EMAIL
+    blocking: str = 'asyncio'
+    timeout: int = 60
 
     def __init__(self, *args, **kwargs):
         self.host: str = None
         self.port: int = None
         self._server: Callable = None
         super(ProviderEmail, self).__init__(*args, **kwargs)
 
@@ -43,15 +44,15 @@
     async def close(self):
         if self._server:
             try:
                 await self._server.quit()
             except aiosmtplib.errors.SMTPServerDisconnected:
                 pass
             except Exception as err:  # pylint: disable=W0703
-                self._logger.exception(err, stack_info=True)
+                self.logger.exception(err, stack_info=True)
             finally:
                 self._server = None
 
     async def connect(self, *args, **kwargs):
         """
         Make a connection to the SMTP Server
         """
@@ -69,21 +70,23 @@
                 password=self.password,
                 start_tls=True,
                 tls_context=context,
                 # loop=self._loop
             )
             try:
                 await self._server.connect()
-                self._logger.debug(f":: {self.__name__}: Connected to: {self._server}")
+                self.logger.debug(
+                    f":: {self.__name__}: Connected to: {self._server}"
+                )
                 try:
                     if self._server.is_ehlo_or_helo_needed:
                         await self._server.ehlo()
-                except aiosmtplib.errors.SMTPHeloError:
-                    pass
-                await asyncio.sleep(0)
+                except aiosmtplib.errors.SMTPHeloError as exc:
+                    print(exc)
+                await asyncio.sleep(.1)
                 # # making authentication:
                 # await self._server.login(
                 #     username=self.username,
                 #     password=self.password
                 # )
             except aiosmtplib.errors.SMTPAuthenticationError as err:
                 raise RuntimeError(
@@ -124,52 +127,49 @@
             # message.set_payload(html)
         else:
             message.add_header("Content-Type", "text/plain")
             message.attach(MIMEText(text, "plain"))
         return message
 
     async def _render_(
-        self, to: Actor = None, subject: str = None, content: str = None, **kwargs
+        self, to: Actor = None, message: str = None, subject: str = None, **kwargs
     ):
         """
-        _render.
+        _render_.
 
         Returns the parseable version of Email.
         """
         # TODO: add attachments
-        message = MIMEMultipart("alternative")
-        message["From"] = self.actor
+        msg = MIMEMultipart("alternative")
+        msg["From"] = self.actor
         if isinstance(to, list):
             # TODO: iterate over actors
-            message["To"] = ", ".join(to)
+            msg["To"] = ", ".join(to)
         else:
-            message["To"] = to.account.address
-        message["Subject"] = subject
-        message["Date"] = formatdate(localtime=True)
-        message["sender"] = self.actor
-        message.preamble = subject
-        if content:
-            message.attach(MIMEText(content, "plain"))
+            msg["To"] = to.account.address
+        msg["Subject"] = subject
+        msg["Date"] = formatdate(localtime=True)
+        msg["sender"] = self.actor
+        msg.preamble = subject
+        if message:
+            msg.attach(MIMEText(message, "plain"))
         if self._template:
             self._templateargs = {
                 "recipient": to,
                 "username": to,
-                "message": content,
-                "content": content,
+                "message": message,
+                "content": message,
                 **kwargs,
             }
-            msg = self._template.render(**self._templateargs)
+            content = await self._template.render_async(**self._templateargs)
         else:
-            msg = content
-        message.add_header("Content-Type", "text/html")
-        # message.add_header('Content-Type', 'multipart/mixed')
-        # message.add_header('Content-Transfer-Encoding', 'base64')
-        message.attach(MIMEText(msg, "html"))
-        # message.set_payload(msg)
-        return message
+            content = message
+        msg.add_header("Content-Type", "text/html")
+        msg.attach(MIMEText(content, "html"))
+        return msg
 
     def add_attachment(self, message, filename, mimetype="octect-stream"):
         content = None
         with open(filename, "rb") as fp:
             content = fp.read()
         if mimetype in ("image/png"):
             part = MIMEImage(content)
@@ -181,55 +181,86 @@
         part.add_header("Content-Disposition", "attachment", filename=str(file))
         message.attach(part)
 
     async def _send_(
         self, to: Actor, message: str, subject: str, **kwargs
     ):  # pylint: disable=W0221
         """
-        _send.
+        _send_.
 
         Logic associated with the construction of notifications
         """
-        msg = await self._render_(to, subject, message, **kwargs)
+        msg = await self._render_(to, message, subject, **kwargs)
         if "attachments" in kwargs:
             for attach in kwargs["attachments"]:
                 self.add_attachment(message=msg, filename=attach)
         try:
             try:
                 response = await self._server.send_message(msg)
                 if self._debug is True:
-                    self._logger.debug(response)
+                    self.logger.debug(response)
             except aiosmtplib.errors.SMTPServerDisconnected as err:
                 raise RuntimeError(
                     f"{self.__name__} Server Disconnected {err}"
                 ) from err
             return response
         except Exception as e:
-            print("AQUI ERROR: ", e)
-            self._logger.exception(e)
-            raise ProviderError(f"{self.__name__} Error: got {e.__class__}, {e}") from e
+            self.logger.exception(e)
+            raise ProviderError(
+                f"{self.__name__} Error: got {e.__class__}, {e}"
+            ) from e
 
     async def send(
         self,
         recipient: list[Actor] = None,
         message: Union[str, Any] = None,
         subject: str = None,
         **kwargs,
     ):
         result = None
         # making the connection to the service:
-        if not self._server:
-            try:
-                if asyncio.iscoroutinefunction(self.connect):
-                    await self.connect()
-                else:
-                    self.connect()
-            except Exception as err:
-                raise ProviderError(f"Error connecting to Mail Backend: {err}") from err
-        # after connection, proceed exactly like other connectors.
+        loop = asyncio.get_running_loop()
+        asyncio.set_event_loop(loop)
         try:
-            result = await super(ProviderEmail, self).send(
-                recipient, message, subject=subject, **kwargs
-            )
+            await self.connect()
         except Exception as err:
-            raise ProviderError(f"Error sending Email: {err}") from err
-        return result
+            raise ProviderError(
+                f"Error connecting to Mail Backend: {err}"
+            ) from err
+        # after connection, proceed exactly like other connectors.
+        ## recipients:
+        # template (or message) for preparation
+        message = await self._prepare_(
+            recipient=recipient,
+            message=message,
+            **kwargs
+        )
+        results = []
+        recipients = [recipient] if not isinstance(recipient, list) else recipient
+        tasks = []
+        for to in recipients:
+            task = loop.create_task(
+                self._send_(to, message, subject=subject, **kwargs)
+            )
+            fn = partial(self.__sent__, to, message, **kwargs)
+            task.add_done_callback(fn)
+            tasks.append(task)
+            done, pending = await asyncio.wait(
+                tasks,
+                timeout=self.timeout,
+                return_when="ALL_COMPLETED"
+            )
+            for task in done:
+                exception = task.exception()
+                if exception is not None:
+                    self.logger.error(
+                        f"Mail error: {exception}"
+                    )
+                else:
+                    result = task.result()
+                    results.append(result)
+            for task in pending:
+                self.logger.warning(
+                    f"Task {task} pending, not completed"
+                )
+                task.cancel()
+        return results
```

## notify/providers/aws/aws.py

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 Amazon AWS Email.
 
 Sending Emails using Amazon SMTP services
 """
 from notify.providers.mail import ProviderEmail
-from .settings import (
+from notify.conf import (
     AWS_EMAIL_USER,
     AWS_EMAIL_ACCOUNT,
     AWS_EMAIL_PASSWORD,
     AWS_EMAIL_HOST,
     AWS_EMAIL_PORT,
 )
 
@@ -18,23 +18,23 @@
     """AWS-based Email Provider
     Args:
         :param username: Email client username
         :param password: Email client password
     """
 
     provider = "aws_email"
-    blocking: bool = False
+    blocking: str = 'asyncio'
 
     def __init__(
         self,
+        *args,
         hostname: str = None,
         port: str = None,
         username: str = None,
         password: str = None,
-        *args,
         **kwargs
     ):
         super(Aws, self).__init__(*args, **kwargs)
 
         self.username = username
         self.password = password
         self.host = hostname
```

## notify/providers/dummy/dummy.py

```diff
@@ -3,15 +3,15 @@
 
 """
 from typing import Any, Union
 from collections.abc import Callable
 from navconfig.logging import logging
 from notify.utils import Msg
 from notify.models import Actor
-from notify.providers.abstract import ProviderBase, ProviderType
+from notify.providers.base import ProviderBase, ProviderType
 
 
 def dummy_sent(
     obj: ProviderBase, recipient: Actor, message: Union[str, Any], result: Any, **kwargs
 ):  # pylint: disable=W0613
     logging.debug(f"Message Sent! {recipient!s}")
     #
@@ -22,15 +22,15 @@
     dummy.
 
     Dummy Provider to send messages to stdout
     """
 
     provider = "dummy"
     provider_type = ProviderType.NOTIFY
-    blocking: bool = True
+    blocking: str = 'asyncio'
     sent: Callable = dummy_sent
 
     async def connect(self, *args, **kwargs):
         print("Connecting to Dummy ...")
 
     async def close(self):
         print("Closing to Dummy...")
```

## notify/providers/email/email.py

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 from notify.providers.mail import ProviderEmail
-from .settings import (
+from notify.conf import (
     EMAIL_SMTP_USERNAME,
     EMAIL_SMTP_PASSWORD,
     EMAIL_SMTP_HOST,
     EMAIL_SMTP_PORT,
 )
 
 
@@ -12,15 +12,15 @@
     """
     email.
 
     Basic SMTP Provider.
     """
 
     provider = "email"
-    blocking: bool = False
+    blocking: str = 'asyncio'
 
     def __init__(
         self,
         hostname: str = None,
         port: str = None,
         username: str = None,
         password: str = None,
```

## notify/providers/gmail/gmail.py

```diff
@@ -7,15 +7,15 @@
 
 # 3rd party gmail support
 import smtplib
 from gmail import GMail as GMailWorker, Message
 from notify.providers.mail import ProviderEmail
 from notify.exceptions import ProviderError
 from notify.models import Actor
-from .settings import GMAIL_USERNAME, GMAIL_PASSWORD
+from notify.conf import GMAIL_USERNAME, GMAIL_PASSWORD
 
 
 class Gmail(ProviderEmail):
     """
     Gmail.
 
         Gmail-based Email Provider.
@@ -44,51 +44,53 @@
                 f"to send emails via **{self.provider}** you need to configure username & password. \n"
                 "Either send them as function argument via key \n"
                 "`username` & `password` or set up env variable \n"
                 "as `GMAIL_USERNAME` & `GMAIL_PASSWORD`."
             )
         self.actor = self.username
 
-    def close(self):
+    async def close(self):
         if self._server:
             try:
                 self._server.close()
             except Exception as err:
-                self._logger.warning(err)
+                self.logger.warning(err)
 
-    def connect(self):
+    async def connect(self):
         """
         connect.
 
         Making a connection to Gmail Servers
         """
         try:
             self._server = GMailWorker(self.username, self.password)
         except smtplib.SMTPAuthenticationError as err:
-            raise Exception(f"Authentication Error: {err}") from err
+            raise ProviderError(
+                f"Authentication Error: {err}"
+            ) from err
         except Exception as err:
             raise RuntimeError(err) from err
 
-    def _render_(self, to: Actor, content: str = None, subject: str = None, **kwargs):
+    async def _render_(self, to: Actor, message: str = None, subject: str = None, **kwargs):
         """ """
-        msg = content
+        msg = message
         if self._template:
             self._templateargs = {
                 "recipient": to,
                 "username": to,
-                "message": content,
-                "content": content,
+                "message": message,
+                "content": message,
                 **kwargs,
             }
-            msg = self._template.render(**self._templateargs)
+            msg = await self._template.render_async(**self._templateargs)
         else:
             try:
                 msg = kwargs["body"]
             except KeyError:
-                msg = content
+                msg = message
         # email
         email = {
             "subject": subject,
             "text": msg,
             "sender": self.actor,
             "to": to.account.address,
             "html": msg,
@@ -99,13 +101,13 @@
         self, to: Actor, message: Union[str, Any], subject: str = None, **kwargs
     ) -> Any:
         """
         _send_.
 
         Logic associated with the construction of notifications
         """
-        data = self._render_(to, message, subject, **kwargs)
+        data = await self._render_(to, message, subject, **kwargs)
         # making email connnection
         try:
             return self._server.send(data)
         except Exception as e:
             raise ProviderError(f"Gmail: Error sending Email to {to}: {e}") from e
```

## notify/providers/office365/office365.py

```diff
@@ -1,53 +1,63 @@
 # -*- coding: utf-8 -*-
 """
 o365.
 
 Office 365 Email-based provider
 """
-from typing import Union, Any
 from collections.abc import Callable
-
+from datetime import datetime
 # 3rd party Office 365 support
-from O365 import Account, Connection, MSOffice365Protocol, Message
+from O365 import (
+    Account,
+    MSOffice365Protocol,
+    Message,
+    Connection,
+    FileSystemTokenBackend
+)
+from navconfig import BASE_DIR
 from navconfig.logging import logging
 from notify.providers.mail import ProviderEmail
+from notify.exceptions import NotifyAuthError
 from notify.models import Actor
-from .settings import (
+from notify.conf import (
     O365_CLIENT_ID,
     O365_CLIENT_SECRET,
     O365_TENANT_ID,
     O365_USER,
     O365_PASSWORD,
 )
 
 
 logging.getLogger("requests_oauthlib").setLevel(logging.CRITICAL)
-
+logging.getLogger("O365.connection").setLevel(logging.CRITICAL)
 
 class Office365(ProviderEmail):
     """O365-based Email Provider
     :param client-id: Email client id
     :param client-secret: Email client secret
     :param client-email: actor email
     """
 
     provider = "office365"
-    blocking: bool = True
+    blocking: str = 'asyncio'
 
     def __init__(
         self,
+        *args,
+        username: str = None,
+        password: str = None,
+        use_credentials: bool = True,
         client_id: str = None,
         client_secret: str = None,
         tenant_id: str = None,
-        username: str = None,
-        password: str = None,
-        *args,
+
         **kwargs,
     ):
+        self.authenticate: bool = False
         self.account: Callable = None
         self.protocol: Callable = None
         super(Office365, self).__init__(*args, **kwargs)
 
         # connection related settings
         self.client_id = client_id if client_id is not None else O365_CLIENT_ID
 
@@ -56,95 +66,142 @@
             self.client_secret = O365_CLIENT_SECRET
 
         # tenant id
         self.tenant_id = tenant_id if tenant_id is not None else O365_TENANT_ID
 
         # username and password:
         self.username = username
-        if not self.username:
-            self.username = O365_USER
-
         self.password = password
-        if not self.password:
-            self.password = O365_PASSWORD
+        self.use_credentials = use_credentials
+        if use_credentials is True:
+            if not self.username:
+                self.username = O365_USER
+            if not self.password:
+                self.password = O365_PASSWORD
 
         if self.client_id is None or self.client_secret is None:
             raise RuntimeWarning(
                 f"to send emails via {self.name} you need to configure client id & client secret. \n"
                 "Either send them as function argument via key id and secret or setup variables \n"
                 "as `O365_CLIENT_ID` & `O365_CLIENT_SECRET`."
             )
 
-    def connect(self):
-        """ """
-        self.protocol = MSOffice365Protocol()
-        # scopes_graph = self.protocol.get_scopes_for('Mail.ReadWrite')
-        scopes = ["https://graph.microsoft.com/.default"]
-        if self.username is not None:
+    async def connect(self, **kwargs):
+        """Connect.
+        Making a connection using MS Office 365 Protocol.
+        """
+        self.protocol = MSOffice365Protocol(**kwargs)
+        credentials = (self.client_id, self.client_secret)
+        # "https://graph.microsoft.com/.default",
+        scopes = ["https://outlook.office.com/.default"]
+        # first: check if credential file exists:
+        o365_token = BASE_DIR.joinpath('.o365_token.txt')
+        token_backend = FileSystemTokenBackend(
+            token_path='.',
+            token_filename='.o365_token.txt'
+        )
+        if not o365_token.exists():
+            ## create a authorization code flow:
+            self.account = Account(
+                credentials=credentials,
+                auth_flow_type="authorization",
+                tenant_id=self.tenant_id,
+                protocol=self.protocol,
+                token_backend=token_backend
+            )
+            # This will print the URL to the console
+            print(self.account.con.get_authorization_url(scopes))
+            # After you have logged in in the browser, you need to paste the resulting URL back into the console
+            result_url = input('Paste the result URL here: ')
+            # This will save the token to a file
+            self.account.con.request_token(result_url)
+            self.mailbox = self.account.mailbox(
+                resource=self.username
+            )
+            return self.account
+        if self.use_credentials is True:
             self.account = Connection(
-                credentials=(self.client_id, self.client_secret),
+                credentials=credentials,
                 auth_flow_type="credentials",
                 tenant_id=self.tenant_id,
+                protocol=self.protocol,
+                token_backend=token_backend
             )
         else:
             self.account = Account(
-                credentials=(self.client_id, self.client_secret),
+                credentials=credentials,
                 auth_flow_type="credentials",
                 tenant_id=self.tenant_id,
                 protocol=self.protocol,
+                token_backend=token_backend
             )
-            result = self.account.authenticate(scope=scopes)
-            print("OFFICE635 Auth: ", result)
-        try:
-            return self.account
-        except Exception as e:
-            return e
+            try:
+                if result := self.account.authenticate(scopes=scopes):
+                    self.authenticate = True
+                    self.mailbox = self.account.mailbox(
+                        resource=self.username
+                    )
+                    return self.account
+                raise NotifyAuthError(
+                    f"Unable to authenticate with Office 365 Backend: {result}"
+                )
+            except Exception as e:
+                print(f"Error during authentication: {e}")
+                # Token might be expired or invalid, delete it and start over
+                o365_token.unlink()
+                return await self.connect(**kwargs)
 
     async def close(self):
         pass
 
-    def _render_(self, to: Actor, subject: str = None, content: str = None, **kwargs):
+    async def _render_(self, to: Actor, message: str = None, subject: str = None, **kwargs):
         """ """
-        msg = content
         if self._template:
             templateargs = {
                 "recipient": to,
                 "username": to,
-                "message": content,
-                "content": content,
+                "message": message,
+                "content": message,
                 **kwargs,
             }
-            msg = self._template.render(**templateargs)
+            msg = await self._template.render_async(**templateargs)
         else:
             try:
                 msg = kwargs["body"]
             except KeyError:
-                msg = content
+                msg = message
         # email message
-        if self.username is not None:
+        if self.use_credentials is True:
             # using basic auth instead API
-            message = Message(
+            content = Message(
                 auth=(self.username, self.password),
                 protocol=self.protocol,
                 con=self.account,
             )
         else:
-            message = self.account.new_message()
-        message.to.add(to.account.address)
-        message.subject = subject
-        message.body = msg
-        return message
+            content = self.mailbox.new_message()
+        content.to.add(to.account.address)
+        content.subject = subject
+        try:
+            content.setBodyHTML(msg)
+        except (AttributeError, ValueError):
+            content.body = msg
+        return content
 
     async def _send_(self, to: Actor, message: str, subject: str, **kwargs):
         """
         _send_.
         Logic associated with the construction of notifications
         """
         # making email connnection
         try:
-            message = self._render_(to, subject, message, **kwargs)
-            status = message.send()
-            logging.debug(status)
-            return status
-        except Exception as e:
-            print(e)
-            raise RuntimeError(f"{e}") from e
+            message = await self._render_(to, message, subject, **kwargs)
+        except (TypeError, ValueError) as exc:
+            print(exc)
+            return False
+        try:
+            result = message.send()
+            return result
+        except Exception as exc:
+            print('Error: ', exc)
+            logging.exception(exc, stack_info=True)
+            raise RuntimeError(f"{exc}") from exc
```

## notify/providers/onesignal/onesignal.py

```diff
@@ -3,31 +3,31 @@
 
 Using OneSignal infraestructure to send push notifications to browsers.
 """
 from typing import Union, Any
 from requests.exceptions import HTTPError
 from onesignal_sdk.client import AsyncClient
 from onesignal_sdk.error import OneSignalHTTPError
-from notify.providers.abstract import ProviderIMBase, ProviderType
+from notify.providers.base import ProviderIMBase, ProviderType
 from notify.models import Actor
 from notify.exceptions import ProviderError
-from .settings import ONESIGNAL_PLAYER_ID, ONESIGNAL_OS_APP_ID, ONESIGNAL_OS_API_KEY
+from notify.conf import ONESIGNAL_PLAYER_ID, ONESIGNAL_OS_APP_ID, ONESIGNAL_OS_API_KEY
 
 
 class Onesignal(ProviderIMBase):
     """
     onesignal.
 
     param:: player_ids: a list of "players", recipients of push messages
     param:: app_id: passing an APP_ID
     """
 
     provider = "onesignal"
     provider_type = ProviderType.PUSH
-    blocking: bool = False
+    blocking: str = 'asyncio'
 
     def __init__(
         self,
         player_ids: str = None,
         app_id: str = None,
         api_key: str = None,
         *args,
```

## notify/providers/sendgrid/sendgrid.py

```diff
@@ -1,33 +1,33 @@
 # -*- coding: utf-8 -*-
 from notify.providers.mail import ProviderEmail
-from .settings import SENDGRID_USER, SENDGRID_KEY
+from notify.conf import SENDGRID_USER, SENDGRID_KEY
 
 
 class Sendgrid(ProviderEmail):
     """
     Sendgrid.
 
     Sendgrid SMTP Client.
     TODO: migrate to API.
     """
 
     provider = "sendgrid"
-    blocking: bool = False
+    blocking: str = 'asyncio'
 
     def __init__(self, username: str = None, password: str = None, **kwargs):
         """ """
         self._attachments: list = []
         self.force_tls: bool = True
 
         super(Sendgrid, self).__init__(**kwargs)
 
         # server information
-        self._host = "smtp.sendgrid.net"
-        self._port = 587
+        self.host = "smtp.sendgrid.net"
+        self.port = 587
         # connection related settings
         self.username = username
         if not self.username:
             self.username = SENDGRID_USER
 
         self.password = password
         if not self.password:
```

## notify/providers/slack/slack.py

```diff
@@ -1,28 +1,26 @@
 """
 onesignal.
 
 Using OneSignal infraestructure to send push notifications to browsers.
 """
 from typing import Union, Any
 from collections.abc import Callable
-from requests.exceptions import HTTPError
-
 # Slack API
 from slack_bolt.authorization import AuthorizeResult
-from slack_bolt.async_app import AsyncApp
+# from slack_bolt.async_app import AsyncApp
 from slack_sdk.web.async_client import AsyncWebClient
 from slack_sdk.errors import SlackApiError
 
 # notify
-from navconfig.logging import logging, loglevel
-from notify.providers.abstract import ProviderIM, ProviderType
+from navconfig.logging import logging
+from notify.providers.base import ProviderIM, ProviderType
 from notify.models import Actor, Channel
 from notify.exceptions import ProviderError, MessageError
-from .settings import (
+from notify.conf import (
     SLACK_APP_ID,
     SLACK_CLIENT_ID,
     SLACK_CLIENT_SECRET,
     SLACK_SIGNING_SECRET,
     # Bot information:
     SLACK_TEAM_ID,
     SLACK_BOT_TOKEN,
@@ -42,18 +40,17 @@
 class Slack(ProviderIM):
     """
     Slack.
 
     param:: player_ids: a list of "players", recipients of push messages
     param:: app_id: passing an APP_ID
     """
-
     provider = "slack"
     provider_type = ProviderType.IM
-    blocking: bool = False
+    blocking: str = 'asyncio'
 
     def __init__(self, *args, **kwargs):
         """
         :param player_id: user token given by OneSignal API
         :param app_id:
         :param api_key:
 
@@ -72,15 +69,17 @@
                 token=SLACK_BOT_TOKEN, logger=logger, team_id=SLACK_TEAM_ID
             )
             self.conversations = await self.client.conversations_list(
                 limit=10, team_id=SLACK_TEAM_ID
             )
         except Exception as err:
             self._logger.error(err)
-            raise ProviderError(f"Error connecting to Slack API {err}") from err
+            raise ProviderError(
+                f"Error connecting to Slack API {err}"
+            ) from err
 
     async def close(self):
         print("CLOSE")
         self.client = None
         self.app = None
 
     async def _send_(self, to: Actor, message: Union[str, Any], **kwargs) -> Any:
@@ -120,8 +119,10 @@
         except (
             SlackApiError
         ) as ex:  # An exception is raised if response.status_code != 2xx
             raise MessageError(
                 f"Slack: Error sending Notification: {ex}",
             ) from ex
         except Exception as ex:
-            raise ProviderError(f"Slack: Exception on Slack Client: {ex}") from ex
+            raise ProviderError(
+                f"Slack: Exception on Slack Client: {ex}"
+            ) from ex
```

## notify/providers/telegram/Telegram.py

```diff
@@ -1,47 +1,49 @@
-import logging
 from io import BytesIO
-from pathlib import PurePath
+from pathlib import Path, PurePath
 from typing import Union, Any
 import emoji
 from PIL import Image
 
 # telegram
 from aiogram import Bot, types
-
 # from aiogram.dispatcher import Dispatcher
 # from aiogram.dispatcher.webhook import SendMessage
 from aiogram.utils.exceptions import (
     TelegramAPIError,
     # BotBlocked,
     BadRequest,
     MessageError,
     Unauthorized,
     NetworkError,
     ChatNotFound,
 )
 import aiofiles
-
 # from aiogram.utils.emoji import emojize
 # from aiogram.utils.markdown import bold, code, italic, text
 # TODO: web-hooks
 # from aiogram.utils.executor import start_webhook
+from navconfig.logging import logging
 from notify.models import Actor, Chat
-from notify.exceptions import notifyException
-from notify.providers.abstract import ProviderIM, ProviderType
-from .settings import TELEGRAM_BOT_TOKEN, TELEGRAM_CHAT_ID
+from notify.exceptions import NotifyException
+from notify.providers.base import ProviderIM, ProviderType
+
+from notify.conf import (
+    TELEGRAM_BOT_TOKEN,
+    TELEGRAM_CHAT_ID
+)
 
 aiogram_logger = logging.getLogger("aiogram")
 aiogram_logger.setLevel(logging.WARNING)
 
 
 class Telegram(ProviderIM):
     provider: str = "telegram"
     provider_type = ProviderType.IM
-    blocking: bool = False
+    blocking: str = 'asyncio'
     parseMode: str = "html"  # can be MARKDOWN_V2 or HTML
 
     def __init__(self, *args, **kwargs):
         try:
             self.parseMode = kwargs["parse_mode"]
             del kwargs["parse_mode"]
         except KeyError:
@@ -74,20 +76,22 @@
         self._connected = False
 
     async def connect(self, *args, **kwargs):
         # creation of bot
         try:
             self._bot = Bot(token=self._bot_token)
             self._info = await self._bot.get_me()
-            self._logger.debug(
+            self.logger.debug(
                 f"🤖 Hello, I'm {self._info.first_name}.\nHave a nice Day!"
             )
             self._connected = True
         except Exception as err:
-            raise notifyException(f"Notify: Error creating Telegram Bot {err}") from err
+            raise NotifyException(
+                f"Notify: Error creating Telegram Bot {err}"
+            ) from err
 
     def set_chat(self, chat):
         self._chat_id = chat
 
     def get_chat(self, **kwargs):
         # define destination
         try:
@@ -110,15 +114,17 @@
         _send_.
 
         Logic associated with the construction of notifications
         """
         # start sending a message:
         try:
             msg = await self._render_(to, message, subject=subject, **kwargs)
-            self._logger.info(f"Messsage> {msg}")
+            self.logger.info(
+                f"Messsage> {msg}"
+            )
         except Exception as err:
             raise RuntimeError(
                 f"Notify Telegram: Error Parsing Message: {err}"
             ) from err
         # Parsing Mode:
         if self.parseMode == "html":
             mode = types.ParseMode.HTML
@@ -152,14 +158,17 @@
             # handle slow connection problems
             print(err)
         except TelegramAPIError as err:
             # handle all other telegram related errors
             print(err)
         except Exception as err:
             print("ERROR: ", err)
+            raise NotifyException(
+                f"{err}"
+            ) from err
 
     async def prepare_photo(self, photo):
         # Migrate to aiofile
         if isinstance(photo, PurePath):
             # is a path, I need to open that image
             img = Image.open(r"{}".format(photo))
             bio = BytesIO()
@@ -197,15 +206,17 @@
             except NetworkError as err:
                 # handle slow connection problems
                 print(err)
             except TelegramAPIError as err:
                 # handle all other telegram related errors
                 print(err)
             except Exception as err:
-                print("ERROR: ", err)
+                raise NotifyException(
+                    f"{err}"
+                ) from err
 
     async def get_document(self, doc: Union[str, PurePath, Any]) -> Any:
         if isinstance(doc, PurePath):  # Path to a File:
             if doc.exists():
                 async with aiofiles.open(doc, "rb") as f:
                     content = await f.read()
                 return content
@@ -215,15 +226,19 @@
             # TODO: check if URL or get file_id
             return doc
 
     async def send_document(self, document, **kwargs):
         chat_id = self.get_chat()
         doc = await self.get_document(document)
         try:
-            response = await self._bot.send_document(chat_id, document=doc, **kwargs)
+            response = await self._bot.send_document(
+                chat_id,
+                document=doc,
+                **kwargs
+            )
             # print(response) # TODO: make the processing of response
             return response
         except Unauthorized as err:
             # remove update.message.chat_id from conversation list
             print(err)
         except MessageError as err:
             print(err)
@@ -237,30 +252,35 @@
             # handle slow connection problems
             print(err)
         except TelegramAPIError as err:
             # handle all other telegram related errors
             print(err)
         except Exception as err:
             print("ERROR: ", err)
+            raise NotifyException(
+                f"{err}"
+            ) from err
 
     async def get_sticker(self, sticker_id):
         if isinstance(sticker_id, dict):  # getting from an sticker_set
             name = sticker_id["set"]
             em = sticker_id["emoji"]
             print(emoji.emojize(em))
             if isinstance(em, str) and em.startswith(":"):
                 em = emoji.emojize(em)
             try:
                 sticker_set = await self._bot.get_sticker_set(name)
-                self._logger.debug(f"Set Found: {sticker_set!r}")
+                self.logger.debug(f"Set Found: {sticker_set!r}")
                 st = [x for x in sticker_set["stickers"] if x["emoji"] == em]
                 sticker = st[0].file_id
                 return sticker
             except Exception as err:
-                self._logger.warning(f"Sticker finder error: {err}")
+                self.logger.warning(
+                    f"Sticker finder error: {err}"
+                )
                 return None
         else:
             return "CAACAgEAAxkBAAIuOWMze9CZzg6cQaEulHqjrcRCvBh2AAK_AgACJjFuAVdTX0Nu_LoxKgQ"
 
     async def send_sticker(self, sticker: Union[str, Any], **kwargs):
         chat_id = self.get_chat()
         sticker = await self.get_sticker(sticker)
@@ -283,14 +303,17 @@
             # handle slow connection problems
             print(err)
         except TelegramAPIError as err:
             # handle all other telegram related errors
             print(err)
         except Exception as err:
             print("ERROR: ", err)
+            raise NotifyException(
+                f"{err}"
+            ) from err
 
     async def get_media(self, media: Union[str, PurePath, Any]) -> Any:
         if isinstance(media, PurePath):  # Path to a File:
             if media.exists():
                 async with aiofiles.open(media, "rb") as f:
                     content = await f.read()
                 return content
@@ -322,14 +345,17 @@
             # handle slow connection problems
             print(err)
         except TelegramAPIError as err:
             # handle all other telegram related errors
             print(err)
         except Exception as err:
             print("ERROR: ", err)
+            raise NotifyException(
+                f"{err}"
+            ) from err
 
     async def send_audio(self, audio: Union[str, PurePath, Any], **kwargs):
         chat_id = self.get_chat()
         sound = await self.get_media(audio)
         try:
             response = await self._bot.send_audio(chat_id, audio=sound, **kwargs)
             # print(response) # TODO: make the processing of response
@@ -349,7 +375,10 @@
             # handle slow connection problems
             print(err)
         except TelegramAPIError as err:
             # handle all other telegram related errors
             print(err)
         except Exception as err:
             print("ERROR: ", err)
+            raise NotifyException(
+                f"{err}"
+            ) from err
```

## notify/providers/twilio/twilio.py

```diff
@@ -1,44 +1,49 @@
 from typing import Union, Any
 from twilio.base.exceptions import TwilioRestException
 from twilio.rest import Client
 from notify.providers.abstract import ProviderMessageBase, ProviderType
 from notify.models import Actor
 from notify.exceptions import ProviderError
-from .settings import TWILIO_AUTH_TOKEN, TWILIO_ACCOUNT_SID, TWILIO_PHONE
-
+from notify.conf import (
+    TWILIO_AUTH_TOKEN,
+    TWILIO_ACCOUNT_SID,
+    TWILIO_PHONE
+)
 
 class Twilio(ProviderMessageBase):
     provider = "sms"
     provider_type = ProviderType.SMS
     level = ""
+    blocking: str = 'asyncio'
 
     def __init__(self, sid: str = None, token: str = None, **kwargs):
         """
         :param token: twilio auth token given by Twilio
         :param sid: twilio auth id given by Twilio
 
         """
         self._msg = None
         self.client = None
         super(Twilio, self).__init__(**kwargs)
         self.token = TWILIO_AUTH_TOKEN if token is None else token
         self.sid = TWILIO_ACCOUNT_SID if sid is None else sid
 
-    def close(self):
+    async def close(self):
         self.client = None
 
-    def connect(self):
+    async def connect(self):
         """
         Verifies that a token and sid were given
 
         """
         if self.token is None or self.sid is None:
             raise RuntimeError(
-                f"to send SMS via {self.__name__} you need to configure TWILIO_ACCOUNT_SID & TWILIO_AUTH_TOKEN in \n"
+                f"to send SMS via {self.__name__} you need to configure \
+                TWILIO_ACCOUNT_SID & TWILIO_AUTH_TOKEN in \n"
                 "environment variables or send account_sid & auth_token in instance."
             )
         self.client = Client(self.sid, self.token)
 
     async def _send_(self, to: Actor, message: Union[str, Any], **kwargs) -> Any:
         """
         _send.
```

## notify/providers/twitter/twitter.py

```diff
@@ -1,18 +1,18 @@
 """
 Twitter API.
 
 Using tweepy to send (publish) Tweets.
 """
 from typing import Optional, Union, Any
 import tweepy
-from notify.providers import ProviderIMBase, ProviderType
+from notify.providers.base import ProviderIMBase, ProviderType
 from notify.models import Actor
 from notify.exceptions import ProviderError
-from .settings import (
+from notify.conf import (
     TWITTER_ACCESS_TOKEN,
     TWITTER_TOKEN_SECRET,
     TWITTER_CONSUMER_KEY,
     TWITTER_CONSUMER_SECRET,
 )
 
 
@@ -20,15 +20,15 @@
     provider = "twitter"
     provider_type = ProviderType.IM
     _consumer_key: str = None
     _consumer_secret: str = None
     _token: str = None
     _secret: str = None
     client = None
-
+    blocking: str = 'asyncio'
     sid = None
 
     def __init__(
         self,
         consumer_key=None,
         consumer_secret=None,
         token=None,
@@ -47,25 +47,26 @@
         self._consumer_key = (
             TWITTER_CONSUMER_KEY if consumer_key is None else consumer_key
         )
         self._consumer_secret = (
             TWITTER_CONSUMER_SECRET if consumer_secret is None else consumer_secret
         )
 
-    def close(self):
+    async def close(self):
         self.client = None
 
-    def connect(self):
+    async def connect(self):
         """
         Verifies that a token and sid were given
 
         """
         if self._token is None or self._secret is None:
             raise RuntimeError(
-                f"to send Tweets via {self._token} you need to configure TWITTER_ACCESS_TOKEN & TWITTER_TOKEN_SECRET in \n"
+                f"to send Tweets via {self._token} you need to configure \
+                TWITTER_ACCESS_TOKEN & TWITTER_TOKEN_SECRET in \n"
                 "environment variables or send properties to theinstance."
             )
         try:
             auth = tweepy.OAuthHandler(self._consumer_key, self._consumer_secret)
             if auth:
                 auth.set_access_token(self._token, self._secret)
                 self.client = tweepy.API(auth)
```

## notify/providers/xmpp/xmpp.py

```diff
@@ -1,67 +1,83 @@
 """
 xmpp.
 
 XMPP use slixmpp to send jabber messages (XMPP protocol)
 """
-import logging
-import ssl
 from typing import Union, Any
-
+import ssl
 # XMPP library
 from slixmpp import ClientXMPP
 from slixmpp.exceptions import IqError, IqTimeout
 from slixmpp.xmlstream.xmlstream import NotConnectedError
+from navconfig.logging import logging
 from notify.models import Actor
-from notify.providers import ProviderIMBase, IM
+from notify.providers.base import ProviderIM, ProviderType
 from notify.exceptions import ProviderError
-
-from .settings import JABBER_JID, JABBER_PASSWORD
+from notify.conf import (
+    JABBER_JID,
+    JABBER_PASSWORD
+)
 
 
 class Client(ClientXMPP):
     """
     Client.
 
     Extending Class to registering session and plugins
     """
-
     provider = "xmpp"
-    provider_type = IM
+    provider_type = ProviderType.IM
 
     def __init__(self, jid, password, plugins: list = None):
         ClientXMPP.__init__(self, jid, password)
         # The session_start event will be triggered when
         # the bot establishes its connection with the server
         # and the XML streams are ready for use. We want to
         # listen for this event so that we we can initialize
         # our roster.
-        self.add_event_handler("session_start", self.session_start)
+        self.add_event_handler(
+            "session_start",
+            self.session_start
+        )
         # The message event is triggered whenever a message
         # stanza is received. Be aware that that includes
         # MUC messages and error messages.
-        self.add_event_handler("message", self.message)
-        self.add_event_handler("disconnected", self.on_disconnect)
-        self.add_event_handler("connection_failed", self.on_connection_failure)
+        self.add_event_handler(
+            "message",
+            self.message
+        )
+        self.add_event_handler(
+            "disconnected",
+            self.on_disconnect
+        )
+        self.add_event_handler(
+            "connection_failed",
+            self.on_connection_failure
+        )
         if isinstance(plugins, list):
             for p in plugins:
                 self.register_plugin(p)
         self["xep_0030"].add_feature("echo_demo")
         self.ssl_version = ssl.PROTOCOL_SSLv3
 
     async def session_start(self, event):
         self.send_presence()
         try:
             await self.get_roster()
         except IqError as err:
-            logging.error("There was an error getting the roster")
+            logging.error(
+                "There was an error getting the roster"
+            )
             logging.error(err.iq["error"]["condition"])
             self.disconnect()
         except IqTimeout:
-            logging.error("Server is taking too long to respond")
+            logging.error(
+                "Server is taking too long to respond"
+            )
             self.disconnect()
 
     def message(self, msg):
         """
         called by slixmpp on incoming XMPP messages
         """
         if msg["type"] in ("chat", "normal"):
@@ -80,25 +96,25 @@
     async def close(self):
         logging.info("Terminating XMPP session")
         self.do_reconnections = False
         self.disconnect()
         logging.info("XMPP session terminated.")
 
 
-class Xmpp(ProviderIMBase):
+class Xmpp(ProviderIM):
     """
     xmpp.
 
     XMPP message provider
     :param username: JID Jabber
     :param password: Jabber password
     """
 
     provider = "xmpp"
-    provider_type = IM
+    provider_type = ProviderType.IM
     client = None
     _session = None
     _id = None
     _plugins = [
         "xep_0030",  # Service Discovery
         "xep_0199",  # XMPP Ping
         "xep_0060",  # PubSub
@@ -132,26 +148,30 @@
             self._plugins = self._plugins + kwargs["plugins"]
 
     async def test(self, jid: str = None):
         if not jid:
             jid = self.client.boundjid.bare
         try:
             rtt = await self.client["xep_0199"].ping(jid, timeout=10)
-            self._logger.info(f"Success! RTT: {rtt!s}")
+            self.logger.info(f"Success! RTT: {rtt!s}")
         except IqError as e:
             error = e.iq["error"]["condition"]
-            self._logger.info(f"Error pinging {jid}: {error}")
+            self.logger.info(f"Error pinging {jid}: {error}")
         except IqTimeout:
-            self._logger.info(f"No response from {jid}")
+            self.logger.info(f"No response from {jid}")
         finally:
             self.client.disconnect()
 
-    def connect(self):
+    def connect(self, **kwargs):
         try:
-            self.client = Client(self.username, self.password, plugins=self._plugins)
+            self.client = Client(
+                self.username,
+                self.password,
+                plugins=self._plugins
+            )
             # Connect to the XMPP server and start processing XMPP stanzas
             self.client.connect()
             self.client.process(forever=False)
         except Exception as e:
             raise ProviderError(e) from e
         return self.client
 
@@ -163,15 +183,17 @@
         except KeyError:
             context = None
         try:
             self.client.send_message(
                 mto=to, mbody=f"{subject}: {message}", mtype="chat"
             )
         except NotConnectedError:
-            self.log("Message NOT SENT, not connected.")
+            self.logger.warning(
+                "Message NOT SENT, not connected."
+            )
         except IqError as e:
             raise ProviderError(e) from e
         except IqTimeout as e:
             raise ProviderError(e) from e
         except Exception as e:
             raise ProviderError(e) from e
```

## notify/utils/__init__.py

```diff
@@ -1,9 +1,6 @@
-from asyncdb.utils.functions import colors, cPrint, Msg
-from asyncdb.utils.types import SafeDict
+from .functions import cPrint, Msg
 
 __all__ = (
-    "SafeDict",
-    "colors",
     "cPrint",
     "Msg",
 )
```

## Comparing `notify/exceptions.py` & `notify/exceptions.pyx`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,46 @@
-class notifyException(Exception):
-    """Base class for other exceptions."""
+# cython: language_level=3, embedsignature=True, boundscheck=False, wraparound=True, initializedcheck=False
+# Copyright (C) 2018-present Jesus Lara
+#
+"""NotifyException Exceptions."""
+cdef class NotifyException(Exception):
+    """Base class for other exceptions"""
 
-    code: int = None
-    payload: str = None
+    code: int = 400
 
-    def __init__(
-        self, message: str, *args, code: int = None, payload: str = None, **kwargs
-    ):
-        super().__init__(*args, **kwargs)
-        self.args = (
-            message,
-            code,
-        )
+    def __init__(self, str message, int code = 0, str payload = None, **kwargs):
+        super().__init__(message)
         self.message = message
-        if code:
-            self.code = code
-        if payload:
-            self.payload = payload
+        self.args = kwargs
+        self.code = int(code)
+        self.payload = payload
+
+    def __repr__(self):
+        return f"{__name__} -> {self.message}, code: {self.code}"
 
     def __str__(self):
-        return f"{__name__} -> {self.message}"
+        return f"{self.message!s}"
 
     def get(self):
         return self.message
 
-
-class DataError(notifyException, ValueError):
-    """An error caused by invalid query input."""
-
-
-class NotSupported(notifyException):
+cdef class NotSupported(NotifyException):
     """Not Supported functionality."""
 
 
-class ProviderError(notifyException):
+cdef class ProviderError(NotifyException):
     """Database Provider Error."""
 
 
-class MessageError(notifyException):
+cdef class MessageError(NotifyException):
     """Raises when an error on Message."""
 
 
-class UninitializedError(ProviderError):
+cdef class UninitializedError(ProviderError):
     """Exception when provider cant be initialized."""
 
 
-class ConnectionTimeout(ProviderError):
+cdef class NotifyTimeout(ProviderError):
     """Connection Timeout Error."""
+
+cdef class NotifyAuthError(ProviderError):
+    """Notify Authentication error."""
```

## Comparing `async_notify-0.9.4.dist-info/LICENSE` & `async_notify-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

