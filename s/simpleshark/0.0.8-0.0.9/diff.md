# Comparing `tmp/simpleshark-0.0.8.tar.gz` & `tmp/simpleshark-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/root/Naveen/simpleshark/src/dist/.tmp-tih7mvko/simpleshark-0.0.8.tar", last modified: Mon Dec 12 16:08:02 2022, max compression
+gzip compressed data, was "/root/Naveen/simpleshark/src/dist/.tmp-qxeg1ed3/simpleshark-0.0.9.tar", last modified: Wed Dec 14 13:12:15 2022, max compression
```

## Comparing `simpleshark-0.0.8.tar` & `simpleshark-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-12 16:08:02.512467 simpleshark-0.0.8/
--rw-r--r--   0 root         (0) root         (0)     1074 2021-06-11 06:03:14.000000 simpleshark-0.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       31 2021-06-11 06:03:14.000000 simpleshark-0.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      673 2022-12-12 16:08:02.512467 simpleshark-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      175 2021-06-11 06:03:14.000000 simpleshark-0.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-12 16:08:02.513467 simpleshark-0.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      835 2022-12-12 15:04:44.000000 simpleshark-0.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-12 16:08:02.509467 simpleshark-0.0.8/simpleshark/
--rw-r--r--   0 root         (0) root         (0)      388 2021-06-11 06:03:14.000000 simpleshark-0.0.8/simpleshark/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-12 16:08:02.510467 simpleshark-0.0.8/simpleshark/capture/
--rw-r--r--   0 root         (0) root         (0)        0 2021-06-11 06:03:14.000000 simpleshark-0.0.8/simpleshark/capture/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24215 2021-06-11 06:03:14.000000 simpleshark-0.0.8/simpleshark/capture/capture.py
--rw-r--r--   0 root         (0) root         (0)      471 2021-06-11 06:03:14.000000 simpleshark-0.0.8/simpleshark/config.ini
--rw-r--r--   0 root         (0) root         (0)      189 2021-06-11 06:03:14.000000 simpleshark-0.0.8/simpleshark/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-12 16:08:02.511467 simpleshark-0.0.8/simpleshark/packet/
--rw-r--r--   0 root         (0) root         (0)        0 2021-06-11 06:03:14.000000 simpleshark-0.0.8/simpleshark/packet/__init__.py
--rw-r--r--   0 root         (0) root         (0)      576 2021-06-11 06:03:14.000000 simpleshark-0.0.8/simpleshark/packet/common.py
--rw-r--r--   0 root         (0) root         (0)       34 2021-06-11 06:03:14.000000 simpleshark-0.0.8/simpleshark/packet/consts.py
--rw-r--r--   0 root         (0) root         (0)     5971 2022-12-12 15:10:54.000000 simpleshark-0.0.8/simpleshark/packet/fields.py
--rw-r--r--   0 root         (0) root         (0)     3427 2022-12-12 15:07:51.000000 simpleshark-0.0.8/simpleshark/packet/packet.py
--rw-r--r--   0 root         (0) root         (0)      946 2021-06-11 06:03:14.000000 simpleshark-0.0.8/simpleshark/packet/packet_summary.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-12 16:08:02.512467 simpleshark-0.0.8/simpleshark/tshark/
--rw-r--r--   0 root         (0) root         (0)        0 2021-06-11 06:03:14.000000 simpleshark-0.0.8/simpleshark/tshark/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3394 2021-06-11 06:03:14.000000 simpleshark-0.0.8/simpleshark/tshark/tshark.py
--rw-r--r--   0 root         (0) root         (0)     1453 2021-06-11 06:03:14.000000 simpleshark-0.0.8/simpleshark/tshark/tshark_xml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-12 16:08:02.510467 simpleshark-0.0.8/simpleshark.egg-info/
--rw-r--r--   0 root         (0) root         (0)      673 2022-12-12 16:08:02.000000 simpleshark-0.0.8/simpleshark.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      621 2022-12-12 16:08:02.000000 simpleshark-0.0.8/simpleshark.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-12 16:08:02.000000 simpleshark-0.0.8/simpleshark.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-12-12 16:08:02.000000 simpleshark-0.0.8/simpleshark.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-12-12 16:08:02.000000 simpleshark-0.0.8/simpleshark.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-14 13:12:15.546856 simpleshark-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)     1074 2021-06-11 06:03:14.000000 simpleshark-0.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       31 2021-06-11 06:03:14.000000 simpleshark-0.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      673 2022-12-14 13:12:15.546856 simpleshark-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      175 2021-06-11 06:03:14.000000 simpleshark-0.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2022-12-14 13:12:15.546856 simpleshark-0.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      835 2022-12-14 13:06:33.000000 simpleshark-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-14 13:12:15.543856 simpleshark-0.0.9/simpleshark/
+-rw-r--r--   0 root         (0) root         (0)      388 2021-06-11 06:03:14.000000 simpleshark-0.0.9/simpleshark/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-14 13:12:15.544856 simpleshark-0.0.9/simpleshark/capture/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-06-11 06:03:14.000000 simpleshark-0.0.9/simpleshark/capture/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24215 2021-06-11 06:03:14.000000 simpleshark-0.0.9/simpleshark/capture/capture.py
+-rw-r--r--   0 root         (0) root         (0)      471 2021-06-11 06:03:14.000000 simpleshark-0.0.9/simpleshark/config.ini
+-rw-r--r--   0 root         (0) root         (0)      189 2021-06-11 06:03:14.000000 simpleshark-0.0.9/simpleshark/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-14 13:12:15.545857 simpleshark-0.0.9/simpleshark/packet/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-06-11 06:03:14.000000 simpleshark-0.0.9/simpleshark/packet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      576 2021-06-11 06:03:14.000000 simpleshark-0.0.9/simpleshark/packet/common.py
+-rw-r--r--   0 root         (0) root         (0)       34 2021-06-11 06:03:14.000000 simpleshark-0.0.9/simpleshark/packet/consts.py
+-rw-r--r--   0 root         (0) root         (0)     5971 2022-12-12 15:10:54.000000 simpleshark-0.0.9/simpleshark/packet/fields.py
+-rw-r--r--   0 root         (0) root         (0)     3427 2022-12-12 15:07:51.000000 simpleshark-0.0.9/simpleshark/packet/packet.py
+-rw-r--r--   0 root         (0) root         (0)      946 2021-06-11 06:03:14.000000 simpleshark-0.0.9/simpleshark/packet/packet_summary.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-14 13:12:15.545857 simpleshark-0.0.9/simpleshark/tshark/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-06-11 06:03:14.000000 simpleshark-0.0.9/simpleshark/tshark/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3394 2021-06-11 06:03:14.000000 simpleshark-0.0.9/simpleshark/tshark/tshark.py
+-rw-r--r--   0 root         (0) root         (0)     1737 2022-12-14 13:07:42.000000 simpleshark-0.0.9/simpleshark/tshark/tshark_xml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-14 13:12:15.544856 simpleshark-0.0.9/simpleshark.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      673 2022-12-14 13:12:15.000000 simpleshark-0.0.9/simpleshark.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      621 2022-12-14 13:12:15.000000 simpleshark-0.0.9/simpleshark.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-12-14 13:12:15.000000 simpleshark-0.0.9/simpleshark.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-12-14 13:12:15.000000 simpleshark-0.0.9/simpleshark.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-12-14 13:12:15.000000 simpleshark-0.0.9/simpleshark.egg-info/top_level.txt
```

### Comparing `simpleshark-0.0.8/LICENSE` & `simpleshark-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `simpleshark-0.0.8/PKG-INFO` & `simpleshark-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleshark
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python package to parse tshark/wireshark/tcpdump captured pcaps and return python objects.
 Home-page: https://github.com/naveenraju23/simpleshark
 Author: Naveen Raju
 Author-email: naveen.raju23@gmail.com
 Keywords: wireshark packets parsing pcap packets
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `simpleshark-0.0.8/setup.py` & `simpleshark-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as f:
     long_description = f.read()
 
 setuptools.setup(
     name="simpleshark",
-    version="0.0.8",
+    version="0.0.9",
     author="Naveen Raju",
     author_email="naveen.raju23@gmail.com",
     package_data={'': ['*.ini']},
     packages=setuptools.find_packages(),
     install_requires=['lxml', 'py'],
     url="https://github.com/naveenraju23/simpleshark",
     long_description=long_description,
```

### Comparing `simpleshark-0.0.8/simpleshark/capture/capture.py` & `simpleshark-0.0.9/simpleshark/capture/capture.py`

 * *Files identical despite different names*

### Comparing `simpleshark-0.0.8/simpleshark/packet/common.py` & `simpleshark-0.0.9/simpleshark/packet/common.py`

 * *Files identical despite different names*

### Comparing `simpleshark-0.0.8/simpleshark/packet/fields.py` & `simpleshark-0.0.9/simpleshark/packet/fields.py`

 * *Files identical despite different names*

### Comparing `simpleshark-0.0.8/simpleshark/packet/packet.py` & `simpleshark-0.0.9/simpleshark/packet/packet.py`

 * *Files identical despite different names*

### Comparing `simpleshark-0.0.8/simpleshark/packet/packet_summary.py` & `simpleshark-0.0.9/simpleshark/packet/packet_summary.py`

 * *Files identical despite different names*

### Comparing `simpleshark-0.0.8/simpleshark/tshark/tshark.py` & `simpleshark-0.0.9/simpleshark/tshark/tshark.py`

 * *Files identical despite different names*

### Comparing `simpleshark-0.0.8/simpleshark/tshark/tshark_xml.py` & `simpleshark-0.0.9/simpleshark/tshark/tshark_xml.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """This module contains functions to turn TShark XML parts into Packet objects."""
 import lxml.objectify
 
 from simpleshark.packet.fields import Field
 from simpleshark.packet.packet import Packet
 from simpleshark.packet.packet_summary import PacketSummary
+import re
 
 
 def psml_structure_from_xml(psml_structure):
     if not isinstance(psml_structure, lxml.objectify.ObjectifiedElement):
         psml_structure = lxml.objectify.fromstring(psml_structure)
     return psml_structure.findall('section')
 
@@ -19,15 +20,20 @@
     :param xml_pkt: str or xml object.
     :param psml_structure: a list of the fields in each packet summary in the psml data. If given, packet will
     be returned as a PacketSummary object.
     :return: Packet object.
     """
     if not isinstance(xml_pkt, lxml.objectify.ObjectifiedElement):
         parser = lxml.objectify.makeparser(huge_tree=True)
-        xml_pkt = lxml.objectify.fromstring(xml_pkt, parser)
+        try:
+            xml_pkt = lxml.objectify.fromstring(xml_pkt, parser)
+        except lxml.etree.XMLSyntaxError:
+            res = re.findall(r'<field name="num" pos="0" show="(.*?)"', xml_pkt.decode(), re.S)[0]
+            print(f'Packet conversion error from xml to python object for packet number {res}.')
+            return
     if psml_structure:
         return _packet_from_psml_packet(xml_pkt, psml_structure)
     return _packet_object_from_xml(xml_pkt)
 
 
 def _packet_from_psml_packet(psml_packet, structure):
     return PacketSummary(structure, psml_packet.findall('section'))
```

### Comparing `simpleshark-0.0.8/simpleshark.egg-info/PKG-INFO` & `simpleshark-0.0.9/simpleshark.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleshark
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python package to parse tshark/wireshark/tcpdump captured pcaps and return python objects.
 Home-page: https://github.com/naveenraju23/simpleshark
 Author: Naveen Raju
 Author-email: naveen.raju23@gmail.com
 Keywords: wireshark packets parsing pcap packets
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `simpleshark-0.0.8/simpleshark.egg-info/SOURCES.txt` & `simpleshark-0.0.9/simpleshark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

