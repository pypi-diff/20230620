# Comparing `tmp/streamlitopencvplayer-1.2.6.tar.gz` & `tmp/streamlitopencvplayer-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlitopencvplayer-1.2.6.tar", last modified: Mon Jun 19 23:50:41 2023, max compression
+gzip compressed data, was "streamlitopencvplayer-1.2.7.tar", last modified: Tue Jun 20 08:47:01 2023, max compression
```

## Comparing `streamlitopencvplayer-1.2.6.tar` & `streamlitopencvplayer-1.2.7.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 23:50:41.446071 streamlitopencvplayer-1.2.6/
--rw-rw-rw-   0        0        0      419 2023-06-19 23:50:41.445071 streamlitopencvplayer-1.2.6/PKG-INFO
--rw-rw-rw-   0        0        0      685 2023-05-25 23:06:12.000000 streamlitopencvplayer-1.2.6/README.md
--rw-rw-rw-   0        0        0       42 2023-06-19 23:50:41.448075 streamlitopencvplayer-1.2.6/setup.cfg
--rw-rw-rw-   0        0        0      934 2023-06-19 23:50:37.000000 streamlitopencvplayer-1.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:50:41.411654 streamlitopencvplayer-1.2.6/streamlitopencvplayer/
--rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.2.6/streamlitopencvplayer/__init__.py
--rw-rw-rw-   0        0        0     6712 2023-06-19 23:50:14.000000 streamlitopencvplayer-1.2.6/streamlitopencvplayer/app.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:50:41.428221 streamlitopencvplayer-1.2.6/streamlitopencvplayer.egg-info/
--rw-rw-rw-   0        0        0      419 2023-06-19 23:50:41.000000 streamlitopencvplayer-1.2.6/streamlitopencvplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-06-19 23:50:41.000000 streamlitopencvplayer-1.2.6/streamlitopencvplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 23:50:41.000000 streamlitopencvplayer-1.2.6/streamlitopencvplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-19 23:50:41.000000 streamlitopencvplayer-1.2.6/streamlitopencvplayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 23:50:41.439863 streamlitopencvplayer-1.2.6/test/
--rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.2.6/test/__init__.py
--rw-rw-rw-   0        0        0      240 2023-06-19 14:52:06.000000 streamlitopencvplayer-1.2.6/test/app.py
--rw-rw-rw-   0        0        0     1901 2023-06-19 23:47:36.000000 streamlitopencvplayer-1.2.6/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:47:01.872329 streamlitopencvplayer-1.2.7/
+-rw-rw-rw-   0        0        0      419 2023-06-20 08:47:01.870329 streamlitopencvplayer-1.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0      685 2023-05-25 23:06:12.000000 streamlitopencvplayer-1.2.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-20 08:47:01.873326 streamlitopencvplayer-1.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      934 2023-06-20 08:46:58.000000 streamlitopencvplayer-1.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:47:01.841327 streamlitopencvplayer-1.2.7/streamlitopencvplayer/
+-rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.2.7/streamlitopencvplayer/__init__.py
+-rw-rw-rw-   0        0        0     6565 2023-06-20 00:38:01.000000 streamlitopencvplayer-1.2.7/streamlitopencvplayer/app.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:47:01.857329 streamlitopencvplayer-1.2.7/streamlitopencvplayer.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-06-20 08:47:01.000000 streamlitopencvplayer-1.2.7/streamlitopencvplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2023-06-20 08:47:01.000000 streamlitopencvplayer-1.2.7/streamlitopencvplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 08:47:01.000000 streamlitopencvplayer-1.2.7/streamlitopencvplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-20 08:47:01.000000 streamlitopencvplayer-1.2.7/streamlitopencvplayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 08:47:01.866325 streamlitopencvplayer-1.2.7/test/
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.2.7/test/__init__.py
+-rw-rw-rw-   0        0        0     2200 2023-06-20 00:01:41.000000 streamlitopencvplayer-1.2.7/test/test.py
```

### Comparing `streamlitopencvplayer-1.2.6/README.md` & `streamlitopencvplayer-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `streamlitopencvplayer-1.2.6/setup.py` & `streamlitopencvplayer-1.2.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.2.6' 
+VERSION = '1.2.7' 
 DESCRIPTION = 'Streamlit Opencv player'
 LONG_DESCRIPTION = 'Streamlit Opencv Player is a video player written in python for easy video playback and frames management using OpenCV'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="streamlitopencvplayer",
```

### Comparing `streamlitopencvplayer-1.2.6/streamlitopencvplayer/app.py` & `streamlitopencvplayer-1.2.7/streamlitopencvplayer/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     if json_file is not None:
         response = urllib.request.urlopen(json_file)
         fileReader = json.loads(response.read())
         list_json = []
         list_json.append(fileReader['timestamp'])
         list_json.append(fileReader['data'])
         st.session_state['alerts_list'].append(list_json)
-        #st.write(st.session_state['alerts_list'])
+        #st.write(st.session_state['alerts_list'][0][0])
 
         if not st.session_state['alerts'] and not st.session_state['data'] :
             st.session_state['alerts'] = []
             st.session_state['data'] = []
             for x in range(len(st.session_state['alerts_list'])):
                 time_alert = st.session_state['alerts_list'][x][0]-float(
                     st.session_state['name_vid_sel'].partition('_')[0])
@@ -66,35 +66,32 @@
         for button_label, button_value in button_values.items():
             if button_value == 1:
                 st.session_state['counter'] = alerts[int(button_label)]
                 #st.write(f'Alert "{button_label}", Frame: {alerts[int(button_label)]}')
 
 
     # Buttons and zone of display
-    col1, col2, col3, col4, col5 = st.columns([1,1,1,1,1])
+    col1, col2, col3, col4, col5,col6,col7 = st.columns(7, gap="small")
     with col1:
-        st.write('')
-        st.write('')
+
         container_2 = st.empty()
         pause = container_2.button('⏸')
 
     with col2:
-        st.write('')
-    with col3:
-        st.write('')
-        st.write('')
-        replay = st.button("↻")
-    with col4:
-        st.write('')
-        st.write('')
+
         plus = st.button("➕")
+    with col4:
+
+        replay = st.button("↻")
+    with col3:
+
+        minus = st.button("➖")
     with col5:
         st.write('')
-        st.write('')
-        minus = st.button("➖")
+
 
     if replay:
         st.session_state['counter'] = 0
         st.session_state['frames'] = []
         resume = False
```

### Comparing `streamlitopencvplayer-1.2.6/test/test.py` & `streamlitopencvplayer-1.2.7/test/test.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,22 +2,28 @@
 
 import argparse
 import uuid
 
 import streamlit as st
 from streamlitopencvplayer.app import display_video
 
-#from streamlitopencvplayer.app import display_video
 
 # Initiate all session states used
 if 'counter' not in st.session_state:
     st.session_state['counter'] = 0
 if 'frames' not in st.session_state:
     st.session_state['frames'] = []
-
+if 'alerts' not in st.session_state:
+    st.session_state['alerts'] = []
+if 'data' not in st.session_state:
+    st.session_state['data'] = []
+if 'alerts_list' not in st.session_state:
+    st.session_state['alerts_list'] = []
+if 'name_vid_sel' not in st.session_state:
+    st.session_state['name_vid_sel'] = "1678352121.8713963_1678352127.8713963"
 
 class opencvplayer:
     """Class streamlit opencv player."""
 
     def __init__(self, video_path, json_file):
         self.video_path = video_path
         self.json_file = json_file
```

