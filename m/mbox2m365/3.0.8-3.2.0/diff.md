# Comparing `tmp/mbox2m365-3.0.8.tar.gz` & `tmp/mbox2m365-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbox2m365-3.0.8.tar", last modified: Thu Mar 30 20:07:13 2023, max compression
+gzip compressed data, was "mbox2m365-3.2.0.tar", last modified: Mon Jun 19 23:02:20 2023, max compression
```

## Comparing `mbox2m365-3.0.8.tar` & `mbox2m365-3.2.0.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-03-30 20:07:13.379853 mbox2m365-3.0.8/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    11456 2023-03-30 20:07:13.379853 mbox2m365-3.0.8/PKG-INFO
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    11135 2023-03-30 19:52:19.000000 mbox2m365-3.0.8/README.rst
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-03-30 20:07:13.378853 mbox2m365-3.0.8/jobber/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     5167 2022-09-19 13:44:42.000000 mbox2m365-3.0.8/jobber/jobber.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-03-30 20:07:13.379853 mbox2m365-3.0.8/mbox2m365/
--rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)      268 2022-09-19 20:24:22.000000 mbox2m365-3.0.8/mbox2m365/__init__.py
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    11546 2022-09-20 13:57:52.000000 mbox2m365-3.0.8/mbox2m365/__main__.py
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    30539 2023-03-30 19:26:06.000000 mbox2m365-3.0.8/mbox2m365/mbox2m365.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-03-30 20:07:13.379853 mbox2m365-3.0.8/mbox2m365.egg-info/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    11456 2023-03-30 20:07:12.000000 mbox2m365-3.0.8/mbox2m365.egg-info/PKG-INFO
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      328 2023-03-30 20:07:13.000000 mbox2m365-3.0.8/mbox2m365.egg-info/SOURCES.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        1 2023-03-30 20:07:12.000000 mbox2m365-3.0.8/mbox2m365.egg-info/dependency_links.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       54 2023-03-30 20:07:13.000000 mbox2m365-3.0.8/mbox2m365.egg-info/entry_points.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       20 2023-03-30 20:07:13.000000 mbox2m365-3.0.8/mbox2m365.egg-info/requires.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       17 2023-03-30 20:07:13.000000 mbox2m365-3.0.8/mbox2m365.egg-info/top_level.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      260 2023-03-30 20:06:34.000000 mbox2m365-3.0.8/pyproject.toml
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      449 2023-03-30 20:07:13.380853 mbox2m365-3.0.8/setup.cfg
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      399 2023-03-30 20:03:26.000000 mbox2m365-3.0.8/setup.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-06-19 23:02:20.891032 mbox2m365-3.2.0/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1551 2023-03-30 20:17:54.000000 mbox2m365-3.2.0/LICENSE
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       26 2023-03-30 20:16:20.000000 mbox2m365-3.2.0/MANIFEST.in
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    11458 2023-06-19 23:02:20.892032 mbox2m365-3.2.0/PKG-INFO
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    11135 2023-03-30 20:02:42.000000 mbox2m365-3.2.0/README.md
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    11135 2023-03-30 19:52:19.000000 mbox2m365-3.2.0/README.rst
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-06-19 23:02:20.889032 mbox2m365-3.2.0/jobber/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     5167 2022-09-19 13:44:42.000000 mbox2m365-3.2.0/jobber/jobber.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-06-19 23:02:20.890032 mbox2m365-3.2.0/mbox2m365/
+-rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)      268 2022-09-19 20:24:22.000000 mbox2m365-3.2.0/mbox2m365/__init__.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    11547 2023-05-30 16:25:03.000000 mbox2m365-3.2.0/mbox2m365/__main__.py
+-rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)      908 2023-06-19 23:00:20.000000 mbox2m365-3.2.0/mbox2m365/mailSink.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    31187 2023-06-19 23:00:20.000000 mbox2m365-3.2.0/mbox2m365/mbox2m365.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-06-19 23:02:20.891032 mbox2m365-3.2.0/mbox2m365.egg-info/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    11458 2023-06-19 23:02:20.000000 mbox2m365-3.2.0/mbox2m365.egg-info/PKG-INFO
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      380 2023-06-19 23:02:20.000000 mbox2m365-3.2.0/mbox2m365.egg-info/SOURCES.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        1 2023-06-19 23:02:20.000000 mbox2m365-3.2.0/mbox2m365.egg-info/dependency_links.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       54 2023-06-19 23:02:20.000000 mbox2m365-3.2.0/mbox2m365.egg-info/entry_points.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       20 2023-06-19 23:02:20.000000 mbox2m365-3.2.0/mbox2m365.egg-info/requires.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       17 2023-06-19 23:02:20.000000 mbox2m365-3.2.0/mbox2m365.egg-info/top_level.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      260 2023-06-19 23:00:39.000000 mbox2m365-3.2.0/pyproject.toml
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      449 2023-06-19 23:02:20.892032 mbox2m365-3.2.0/setup.cfg
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      441 2023-03-30 20:18:43.000000 mbox2m365-3.2.0/setup.py
```

### Comparing `mbox2m365-3.0.8/PKG-INFO` & `mbox2m365-3.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: mbox2m365
-Version: 3.0.8
-Summary: 'Send a message stored within an mbox using m365 (Office365)'
-Home-page: https://github.com/FNNDSC/mbox2m365
-Author: Rudolph Pienaar
-Author-email: rudolph.pienaar@childrens.harvard.edu
-License: MIT
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 # Abstract
 
 This repository contains a simple python script that (1) processes an
 `mbox` style mailbox file, (2) parses out (typically) the last message
 and then (3) re-transmits this using the CLI `m365` toolset. While this
 script can be used in a completely stand-alone manner to extract a
 message from an `mbox` and then *send* using `m365`, it’s main utility
@@ -291,9 +280,7 @@
 cd /var/mail
 find . | entr mbox2m365 --mbox rudolph --b64_encode         \
                         --sendFromFile --cleanUp            \
                         --waitForStragglers 5
 ```
 
 *-30-*
-
-
```

### Comparing `mbox2m365-3.0.8/README.rst` & `mbox2m365-3.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `mbox2m365-3.0.8/jobber/jobber.py` & `mbox2m365-3.2.0/jobber/jobber.py`

 * *Files identical despite different names*

### Comparing `mbox2m365-3.0.8/mbox2m365/__main__.py` & `mbox2m365-3.2.0/mbox2m365/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 import  pfmisc
 from    pfmisc._colors      import Colors
 from    pfmisc              import other
 
 import  json
 
-str_desc = Colors.CYAN + """
+str_desc = Colors.CYAN + r"""
 
 
                         _               ___            ____    __ _____
                        | |             |__ \          |___ \  / /| ____|
               _ __ ___ | |__   _____  __  ) |_ __ ___   __) |/ /_| |__
              | '_ ` _ \| '_ \ / _ \ \/ / / /| '_ ` _ \ |__ <| '_ \___ \
              | | | | | | |_) | (_) >  < / /_| | | | | |___) | (_) |__) |
@@ -145,19 +145,19 @@
 """
 
 def synopsis(ab_shortOnly = False):
     scriptName = os.path.basename(sys.argv[0])
     shortSynopsis =  """
     NAME
 
-        mbox2m365                                                               \\
+        mbox2m365
 
     SYNOPSIS
 
-        mbox2m365 """ + package_CLIself + package_CLIcore + """
+        mbox2m365                                                               \\""" + package_CLIself + package_CLIcore + """
 
     BRIEF EXAMPLE
 
         cd /var/mail
         find rudolph | entr mbox2m365 --inputFile rudolph
     """
 
@@ -301,8 +301,8 @@
         )
 
     mbox_2_m365.log("%s:%s all done and going to sleep!" % (__pkg.name, __version__), comms = 'rx')
 
     return 0
 
 if __name__ == "__main__":
-    sys.exit(main())
+    sys.exit(main())
```

### Comparing `mbox2m365-3.0.8/mbox2m365/mbox2m365.py` & `mbox2m365-3.2.0/mbox2m365/mbox2m365.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,26 @@
 import      time
 import      base64
 import      re
 import      hashlib
 
 from        collections         import defaultdict
 
+def field_get(message:dict, field:str) -> str:
+    ret:str     = ""
+    if 'Delivered-To' in field:
+        if message.get(field):
+            ret = str(message.get(field))
+        elif message.get('To'):
+            ret = str(message.get('To'))
+    else:
+            ret = str(message.get(field))
+    return ret
+
+
 class Mbox2m365(object):
     """
 
     The core class for filtering a message out of an mbox and retransmitting
     it using m365
 
     """
@@ -117,15 +129,16 @@
             'output':           'json',     # json,text,csv
             'bodyHash':         '',
             'attachments':      ()
         }
 
         self.dp             = pfmisc.debug(
                                  verbosity   = int(self.args['verbosity']),
-                                 within      = self.__name__
+                                 within      = self.__name__,
+                                 methodcol   = 55
                              )
         self.log            = self.dp.qprint
         self.configPath     = Path(user_config_dir(self.__name__))
         self.keyParsedFile  = self.configPath / Path('keysParsed.json')
         self.mboxPath       = Path(self.args['inputDir']) / Path(self.args['mbox'])
 
     def env_check(self, *args, **kwargs) -> dict:
@@ -396,17 +409,20 @@
         lhash_msgBody       : list  = []
         lstr_attachments    : list  = []
         count               : int   = 0
 
         if d_extract['status']:
             if self.lo_msg: b_status = True
             for message in self.lo_msg:
-                lstr_subject.append(message['Subject'])
-                lstr_to.append(message['Delivered-To'])
-                lstr_date.append(message['Date'])
+                # lstr_subject.append(message['Subject'])
+                # lstr_to.append(message['Delivered-To'])
+                # lstr_date.append(message['Date'])
+                lstr_subject.append(field_get(message, 'Subject'))
+                lstr_to.append(field_get(message, 'Delivered-To'))
+                lstr_date.append(field_get(message, 'Date'))
                 if message.is_multipart():
                     d_parts:dict = self.multipart_separateAttachments(message)
                     lstr_msgBody.append(d_parts['textBody'])
                     lstr_attachments.append(tuple(d_parts['attachFilesList']))
                 else:
                     lstr_msgBody.append(message.get_payload())
                 lhash_msgBody.append(hashlib.md5(lstr_msgBody[-1].encode('utf-8')).hexdigest())
@@ -537,18 +553,19 @@
                 l_target (list): The list of indices in the original mbox
                                  message structure to consult for "to"
                                  recipients.
 
             Returns:
                 str: The (comma separated) string (list) of recipients
             """
-            str_ret         = ""
-            l_to : list     = []
+            str_ret:str     = ""
+            l_to:list       = []
             for msgi in l_target:
-                l_to.append(self.lo_msg[msgi]['Delivered-To'])
+                # pudb.set_trace()
+                l_to.append(field_get(self.lo_msg[msgi], 'Delivered-To'))
                 self.l_keysParsed.append(self.l_keysToParse[msgi])
             str_ret         = ','.join(l_to)
             return str_ret
 
         def attachments_get(l_messageList: list) -> tuple:
             """Resolve the attachments (if any) for a given message
 
@@ -578,14 +595,15 @@
                 # This test was originally predicated on the idea that tallying
                 # occurences across dates and hashes would always match. Sometimes
                 # with attachments, however, it seems the hashes do not. Hence for
                 # now this "dummy" fall through based solely on the date stamp
                 # only.
                 if lists_haveEqualValues(['l_date', 'l_date'], idx):
                     self.ld_m365.append(self.d_m365.copy())
+                    # pudb.set_trace()
                     self.ld_m365[idx]['subject']      = get('list', 'key', 'l_subject', idx)
                     self.ld_m365[idx]['to']           = recipients_get(get('list', 'value', 'l_date', idx))
                     self.ld_m365[idx]['attachments']  = attachments_get(get('list', 'value', 'l_date', idx))
                     self.ld_m365[idx]['bodyContents'] = get('list', 'key', 'l_body', idx)
                     self.ld_m365[idx]['bodyHash']     = get('list', 'key', 'l_hash', idx)
 
         return {
@@ -699,15 +717,15 @@
 
         d_env           : dict  = {}
         b_sizeStable    : bool  = False
         mboxSizeOld     : Path  = Path(self.mboxPath).stat().st_size
         mboxSizeNew     : Path  = Path(self.mboxPath).stat().st_size
         while not b_sizeStable:
             self.log('mbox file size currently: %d' % mboxSizeOld, comms = 'status')
-            self.log('waiting for %s seconds for stragglers...' % \
+            self.log('waiting %s seconds for stragglers...' % \
                         self.args['waitForStragglers'])
             time.sleep(int(self.args['waitForStragglers']))
             mboxSizeNew = Path(self.mboxPath).stat().st_size
             if mboxSizeNew == mboxSizeOld:
                 b_sizeStable    = True
                 self.log('mbox size stable, continuing with processing...')
                 d_env           = self.env_check()
```

### Comparing `mbox2m365-3.0.8/mbox2m365.egg-info/PKG-INFO` & `mbox2m365-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: mbox2m365
-Version: 3.0.8
+Version: 3.2.0
 Summary: 'Send a message stored within an mbox using m365 (Office365)'
 Home-page: https://github.com/FNNDSC/mbox2m365
 Author: Rudolph Pienaar
 Author-email: rudolph.pienaar@childrens.harvard.edu
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Abstract
 
 This repository contains a simple python script that (1) processes an
 `mbox` style mailbox file, (2) parses out (typically) the last message
 and then (3) re-transmits this using the CLI `m365` toolset. While this
 script can be used in a completely stand-alone manner to extract a
@@ -291,9 +291,7 @@
 cd /var/mail
 find . | entr mbox2m365 --mbox rudolph --b64_encode         \
                         --sendFromFile --cleanUp            \
                         --waitForStragglers 5
 ```
 
 *-30-*
-
-
```

