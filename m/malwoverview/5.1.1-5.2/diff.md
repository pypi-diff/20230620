# Comparing `tmp/malwoverview-5.1.1.tar.gz` & `tmp/malwoverview-5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malwoverview-5.1.1.tar", last modified: Thu Nov  3 19:59:30 2022, max compression
+gzip compressed data, was "malwoverview-5.2.tar", last modified: Tue Jun 20 05:07:40 2023, max compression
```

## Comparing `malwoverview-5.1.1.tar` & `malwoverview-5.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 remnux    (1000) remnux    (1000)        0 2022-11-03 19:59:30.446075 malwoverview-5.1.1/
--rw-rw-r--   0 remnux    (1000) remnux    (1000)      233 2022-11-03 19:01:48.000000 malwoverview-5.1.1/.malwapi.conf
--rw-rw-r--   0 remnux    (1000) remnux    (1000)    35149 2022-11-03 19:01:48.000000 malwoverview-5.1.1/LICENSE
--rw-rw-r--   0 remnux    (1000) remnux    (1000)    34525 2022-11-03 19:59:30.446075 malwoverview-5.1.1/PKG-INFO
--rw-rw-r--   0 remnux    (1000) remnux    (1000)    33978 2022-11-03 19:02:12.000000 malwoverview-5.1.1/README.md
-drwxrwxr-x   0 remnux    (1000) remnux    (1000)        0 2022-11-03 19:59:30.442075 malwoverview-5.1.1/malwoverview/
--rw-rw-r--   0 remnux    (1000) remnux    (1000)        1 2022-11-03 19:01:48.000000 malwoverview-5.1.1/malwoverview/__init__.py
--rwxrwxr-x   0 remnux    (1000) remnux    (1000)   610442 2022-11-03 19:57:53.000000 malwoverview-5.1.1/malwoverview/malwoverview.py
-drwxrwxr-x   0 remnux    (1000) remnux    (1000)        0 2022-11-03 19:59:30.446075 malwoverview-5.1.1/malwoverview.egg-info/
--rw-rw-r--   0 remnux    (1000) remnux    (1000)    34525 2022-11-03 19:59:29.000000 malwoverview-5.1.1/malwoverview.egg-info/PKG-INFO
--rw-rw-r--   0 remnux    (1000) remnux    (1000)      273 2022-11-03 19:59:29.000000 malwoverview-5.1.1/malwoverview.egg-info/SOURCES.txt
--rw-rw-r--   0 remnux    (1000) remnux    (1000)        1 2022-11-03 19:59:29.000000 malwoverview-5.1.1/malwoverview.egg-info/dependency_links.txt
--rw-rw-r--   0 remnux    (1000) remnux    (1000)      154 2022-11-03 19:59:29.000000 malwoverview-5.1.1/malwoverview.egg-info/requires.txt
--rw-rw-r--   0 remnux    (1000) remnux    (1000)       13 2022-11-03 19:59:29.000000 malwoverview-5.1.1/malwoverview.egg-info/top_level.txt
--rw-rw-r--   0 remnux    (1000) remnux    (1000)       38 2022-11-03 19:59:30.446075 malwoverview-5.1.1/setup.cfg
--rw-rw-r--   0 remnux    (1000) remnux    (1000)     1330 2022-11-03 19:01:48.000000 malwoverview-5.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:07:40.941765 malwoverview-5.2/
+-rw-r--r--   0 root         (0) root         (0)      233 2023-06-20 05:02:57.000000 malwoverview-5.2/.malwapi.conf
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-06-20 05:02:57.000000 malwoverview-5.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    34611 2023-06-20 05:07:40.937765 malwoverview-5.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    34086 2023-06-20 05:04:04.000000 malwoverview-5.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:07:40.937765 malwoverview-5.2/malwoverview/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 05:02:57.000000 malwoverview-5.2/malwoverview/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)   610320 2023-06-20 05:02:57.000000 malwoverview-5.2/malwoverview/malwoverview.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:07:40.937765 malwoverview-5.2/malwoverview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    34611 2023-06-20 05:07:40.000000 malwoverview-5.2/malwoverview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      273 2023-06-20 05:07:40.000000 malwoverview-5.2/malwoverview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 05:07:40.000000 malwoverview-5.2/malwoverview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2023-06-20 05:07:40.000000 malwoverview-5.2/malwoverview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-20 05:07:40.000000 malwoverview-5.2/malwoverview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 05:07:40.941765 malwoverview-5.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-06-20 05:02:57.000000 malwoverview-5.2/setup.py
```

### Comparing `malwoverview-5.1.1/LICENSE` & `malwoverview-5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `malwoverview-5.1.1/PKG-INFO` & `malwoverview-5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 Metadata-Version: 2.1
 Name: malwoverview
-Version: 5.1.1
+Version: 5.2
 Summary: Malwoverview is a first response tool for threat hunting.
 Home-page: https://github.com/alexandreborges/malwoverview
 Author: Alexandre Borges
 Author-email: alexandreborges@blackstormsecurity.com
 License: GNU GPL v3.0
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Malwoverview
 
-      Copyright (C)  2018-2022 Alexandre Borges <alexandreborges at blackstormsecurity dot com>
+      Copyright (C)  2018-2023 Alexandre Borges <alexandreborges at blackstormsecurity dot com>
 
       This program is free software: you can redistribute it and/or modify
       it under the terms of the GNU General Public License as published by
       the Free Software Foundation, either version 3 of the License, or
       (at your option) any later version.
 
       This program is distributed in the hope that it will be useful,
       but WITHOUT ANY WARRANTY; without even the implied warranty of
       MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
       GNU General Public License for more details.
 
       See GNU Public License on <http://www.gnu.org/licenses/>.
 
 
-# Current Version: 5.1.1
+# Current Version: 5.2
 
      Important note:  Malwoverview does NOT submit samples to any endpoint by default, 
      so it respects possible Non-Disclosure Agreements (NDAs). There're specific options
      that explicitly submit samples, but these options are explained in the help.
 
 
 # ABOUT
@@ -374,14 +373,20 @@
     malwoverview.py -i 11 -I list
     malwoverview.py -i 12 -I rebrand.ly
     malwoverview.py -i 13 -I list | more
 
 
 # HISTORY
 
+Version 5.2:
+
+      This version:
+
+            * Multiple issues related to Hybrid Analysis have been fixed.
+
 Version 5.1.1:
 
       This version:
 
             * A formatting issue related to -v 10 option has been fixed.
 
 Version 5.1:
@@ -844,9 +849,7 @@
 
             * Shows the imphash information classified by color. 
             * Checks whether malware samples are packed.  
             * Checks whether malware samples have overlay. 
             * Shows the entropy of the malware samples. 
 
 
-
-
```

### Comparing `malwoverview-5.1.1/README.md` & `malwoverview-5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # Malwoverview
 
-      Copyright (C)  2018-2022 Alexandre Borges <alexandreborges at blackstormsecurity dot com>
+      Copyright (C)  2018-2023 Alexandre Borges <alexandreborges at blackstormsecurity dot com>
 
       This program is free software: you can redistribute it and/or modify
       it under the terms of the GNU General Public License as published by
       the Free Software Foundation, either version 3 of the License, or
       (at your option) any later version.
 
       This program is distributed in the hope that it will be useful,
       but WITHOUT ANY WARRANTY; without even the implied warranty of
       MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
       GNU General Public License for more details.
 
       See GNU Public License on <http://www.gnu.org/licenses/>.
 
 
-# Current Version: 5.1.1
+# Current Version: 5.2
 
      Important note:  Malwoverview does NOT submit samples to any endpoint by default, 
      so it respects possible Non-Disclosure Agreements (NDAs). There're specific options
      that explicitly submit samples, but these options are explained in the help.
 
 
 # ABOUT
@@ -359,14 +359,20 @@
     malwoverview.py -i 11 -I list
     malwoverview.py -i 12 -I rebrand.ly
     malwoverview.py -i 13 -I list | more
 
 
 # HISTORY
 
+Version 5.2:
+
+      This version:
+
+            * Multiple issues related to Hybrid Analysis have been fixed.
+
 Version 5.1.1:
 
       This version:
 
             * A formatting issue related to -v 10 option has been fixed.
 
 Version 5.1:
```

### Comparing `malwoverview-5.1.1/malwoverview/malwoverview.py` & `malwoverview-5.2/malwoverview/malwoverview.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 #CONTRIBUTORS
 
 # Alexandre Borges (project owner)
 # Corey Forman (https://github.com/digitalsleuth)
 # Christian Clauss (https://github.com/cclauss)
 
-# Malwoverview.py: version 5.1.1
+# Malwoverview.py: version 5.2
 
 import os
 import sys
 import re
 import pefile
 import peutils
 import magic
@@ -58,15 +58,15 @@
 from requests import Request, Session, exceptions
 
 # On Windows systems, it is necessary to install python-magic-bin: pip install python-magic-bin
 
 __author__ = "Alexandre Borges"
 __copyright__ = "Copyright 2018-2021, Alexandre Borges"
 __license__ = "GNU General Public License v3.0"
-__version__ = "5.1.1"
+__version__ = "5.2"
 __email__ = "alexandreborges at blackstormsecurity.com"
 
 haurl = 'https://www.hybrid-analysis.com/api/v2'
 urlfilevt3 = 'https://www.virustotal.com/api/v3/files'
 urlurlvt3 = 'https://www.virustotal.com/api/v3/urls'
 urlipvt3 = 'https://www.virustotal.com/api/v3/ip_addresses'
 urldomainvt3 = 'https://www.virustotal.com/api/v3/domains'
@@ -2213,15 +2213,15 @@
         else:
             finalurl = '/'.join([haurl,'report', resource + ':300', 'summary'])
 
         haresponse = requestsession.get(url=finalurl)
         hatext = json.loads(haresponse.text)
 
         rc = str(hatext)
-        if 'message' in rc:
+        if 'Failed' in rc:
             final = 'Malware sample was not found in Hybrid-Analysis repository.'
             if (bkg == 1):
                 print((mycolors.foreground.lightred + "\n" + final + "\n"))
             else:
                 print((mycolors.foreground.red + "\n" + final + "\n"))
             return final
 
@@ -10326,15 +10326,15 @@
     bazaararg = ''
     triage = 0
     triagearg = ''
     virustotalarg = ''
     ipaddrvtx = ''
     ffpname = ''
 
-    parser = argparse.ArgumentParser(prog=None, description="Malwoverview is a first response tool for threat hunting written by Alexandre Borges. This version is 5.1.1", usage= "python malwoverview.py -c <API configuration file> -d <directory> -o <0|1> -v <1-13> -V <virustotal arg> -a <1-15> -w <0|1> -A <filename> -l <1-6> -L <hash> -j <1-7> -J <URLhaus argument> -p <1-8> -P <polyswarm argument> -y <1-5> -Y <file name> -n <1-5> -N <argument> -m <1-8> -M <argument> -b <1-10> -B <arg> -x <1-7> -X <arg> -i <1-13> -I <INQUEST argument>")
+    parser = argparse.ArgumentParser(prog=None, description="Malwoverview is a first response tool for threat hunting written by Alexandre Borges. This version is 5.2", usage= "python malwoverview.py -c <API configuration file> -d <directory> -o <0|1> -v <1-13> -V <virustotal arg> -a <1-15> -w <0|1> -A <filename> -l <1-6> -L <hash> -j <1-7> -J <URLhaus argument> -p <1-8> -P <polyswarm argument> -y <1-5> -Y <file name> -n <1-5> -N <argument> -m <1-8> -M <argument> -b <1-10> -B <arg> -x <1-7> -X <arg> -i <1-13> -I <INQUEST argument>")
     parser.add_argument('-c', '--config', dest='config', type=str, metavar = "CONFIG FILE", default = (USER_HOME_DIR + '.malwapi.conf'), help='Use a custom config file to specify API\'s.')
     parser.add_argument('-d', '--directory', dest='direct',type=str, metavar = "DIRECTORY", help='Specifies the directory containing malware samples to be checked against VIRUS TOTAL. Use the option -D to decide whether you are being using a public VT API or a Premium VT API.')
     parser.add_argument('-o', '--background', dest='backg', type=int,default = 1, metavar = "BACKGROUND", help='Adapts the output colors to a light background color terminal. The default is dark background color terminal.')
     parser.add_argument('-v', '--virustotal_option', dest='virustotaloption', type=int,default = 0, metavar = "VIRUSTOTAL", help='-v 1: given a file using -V option, it queries the VIRUS TOTAL database (API v.3) to get the report for the given file through -V option.; -v 2: it shows an antivirus report for a given file using -V option (API v.3); -v 3: equal to -v2, but the binary\'s IAT and EAT are also shown (API v.3); -v 4: it extracts the overlay; -v 5: submits an URL to VT scanning; -v 6: submits an IP address to Virus Total; -v 7: this options gets a report on the provided domain from Virus Total; -v 8: verifies a given hash against Virus Total; -v 9: submits a sample to VT (up to 32 MB). Use forward slash to specify the target file on Windows systems. Demands passing sample file with -V option; -v 10: verifies hashes from a provided file through option -V. This option uses public VT API v.3; -v 11: verifies hashes from a provided file through option -V. This option uses Premium API v.3; -v 12: it shows behaviour information of a sample given a hash through option -V. This option uses VT API v.3; -v 13: it submits LARGE files (above 32 MB) to VT using API v.3;')
     parser.add_argument('-V', '--virustotal_arg', dest='virustotalarg', type=str, metavar = "VIRUSTOTAL_ARG", help='Provides arguments for -v option.')
     parser.add_argument('-a', '--hybrid_option', dest='haoption', type=int,default = 0, metavar = "HYBRID_ANALYSIS", help='This parameter fetches reports from HYBRID ANALYSIS, download samples and submits samples to be analyzed. The possible values are: 1: gets a report for a given hash or sample from a Windows 7 32-bit environment; 2: gets a report for a given hash or sample from a Windows 7 32-bit environment (HWP Support); 3: gets a report for given hash or sample from a Windows 64-bit environment; 4: gets a report for a given hash or sample from an Android environment; 5: gets a report for a given hash or sample from a Linux 64-bit environment; 6: submits a sample to Windows 7 32-bit environment; 7. submits a sample to Windows 7 32-bit environment with HWP support environment; 8. submits a sample to Windows 7 64-bit environment ; 9. submits a sample to an Android environment ; 10. submits a sample to a Linux 64-bit environment; 11. downloads a sample from a Windows 7 32-bit environment; 12. downloads a sample from a Windows 7 32-bit HWP environment; 13. downloads a sample from a Windows 7 64-bit environment; 14. downloads a sample from an Android environment; 15. downloads a sample from a Linux 64-bit environment.')
     parser.add_argument('-A', '--ha_arg', dest='haarg', type=str, metavar = "SUBMIT_HA", help='Provides an argument for -a option from HYBRID ANALYSIS.')
@@ -11185,43 +11185,38 @@
             if (bkg == 0):
                 print(mycolors.foreground.red + "\nYou didn't provide a valid file!\n")
         print(mycolors.reset)
         exit(0)
 
     if (haoptionx == 11):
         xx = 0
-        hashow(haargx)
         downhash(haargx)
         print(mycolors.reset)
         exit(0)
     
     if (haoptionx == 12):
         xx = 1
-        hashow(haargx)
         downhash(haargx)
         print(mycolors.reset)
         exit(0)
 
     if (haoptionx == 13):
         xx = 2
-        hashow(haargx)
         downhash(haargx)
         print(mycolors.reset)
         exit(0)
 
     if (haoptionx == 14):
         xx = 3
-        hashow(haargx)
         downhash(haargx)
         print(mycolors.reset)
         exit(0)
 
     if (haoptionx == 15):
         xx = 4
-        hashow(haargx)
         downhash(haargx)
         print(mycolors.reset)
         exit(0)
 
     if (mallist != 0 and mallist >= 2):
         malsharelastlist(maltype)
         print(mycolors.reset)
```

### Comparing `malwoverview-5.1.1/malwoverview.egg-info/PKG-INFO` & `malwoverview-5.2/malwoverview.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 Metadata-Version: 2.1
 Name: malwoverview
-Version: 5.1.1
+Version: 5.2
 Summary: Malwoverview is a first response tool for threat hunting.
 Home-page: https://github.com/alexandreborges/malwoverview
 Author: Alexandre Borges
 Author-email: alexandreborges@blackstormsecurity.com
 License: GNU GPL v3.0
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Malwoverview
 
-      Copyright (C)  2018-2022 Alexandre Borges <alexandreborges at blackstormsecurity dot com>
+      Copyright (C)  2018-2023 Alexandre Borges <alexandreborges at blackstormsecurity dot com>
 
       This program is free software: you can redistribute it and/or modify
       it under the terms of the GNU General Public License as published by
       the Free Software Foundation, either version 3 of the License, or
       (at your option) any later version.
 
       This program is distributed in the hope that it will be useful,
       but WITHOUT ANY WARRANTY; without even the implied warranty of
       MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
       GNU General Public License for more details.
 
       See GNU Public License on <http://www.gnu.org/licenses/>.
 
 
-# Current Version: 5.1.1
+# Current Version: 5.2
 
      Important note:  Malwoverview does NOT submit samples to any endpoint by default, 
      so it respects possible Non-Disclosure Agreements (NDAs). There're specific options
      that explicitly submit samples, but these options are explained in the help.
 
 
 # ABOUT
@@ -374,14 +373,20 @@
     malwoverview.py -i 11 -I list
     malwoverview.py -i 12 -I rebrand.ly
     malwoverview.py -i 13 -I list | more
 
 
 # HISTORY
 
+Version 5.2:
+
+      This version:
+
+            * Multiple issues related to Hybrid Analysis have been fixed.
+
 Version 5.1.1:
 
       This version:
 
             * A formatting issue related to -v 10 option has been fixed.
 
 Version 5.1:
@@ -844,9 +849,7 @@
 
             * Shows the imphash information classified by color. 
             * Checks whether malware samples are packed.  
             * Checks whether malware samples have overlay. 
             * Shows the entropy of the malware samples. 
 
 
-
-
```

### Comparing `malwoverview-5.1.1/setup.py` & `malwoverview-5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 USER_HOME_DIR = str(Path.home()) + os.sep
 
 with open("README.md", encoding='utf8') as readme:
     long_description = readme.read()
 
 setup(
     name="malwoverview",
-    version="5.1.1",
+    version="5.2",
     author="Alexandre Borges",
     author_email="alexandreborges@blackstormsecurity.com",
     license="GNU GPL v3.0",
     url="https://github.com/alexandreborges/malwoverview",
     description=("Malwoverview is a first response tool for threat hunting."),
     long_description=long_description,
     long_description_content_type="text/markdown",
```

