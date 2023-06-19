# Comparing `tmp/streamlitopencvplayer-1.2.5.tar.gz` & `tmp/streamlitopencvplayer-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlitopencvplayer-1.2.5.tar", last modified: Mon Jun 19 23:38:05 2023, max compression
+gzip compressed data, was "streamlitopencvplayer-1.2.6.tar", last modified: Mon Jun 19 23:50:41 2023, max compression
```

## Comparing `streamlitopencvplayer-1.2.5.tar` & `streamlitopencvplayer-1.2.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 23:38:05.178075 streamlitopencvplayer-1.2.5/
--rw-rw-rw-   0        0        0      419 2023-06-19 23:38:05.177076 streamlitopencvplayer-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      685 2023-05-25 23:06:12.000000 streamlitopencvplayer-1.2.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-19 23:38:05.180076 streamlitopencvplayer-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0      934 2023-06-19 23:36:26.000000 streamlitopencvplayer-1.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:38:05.132035 streamlitopencvplayer-1.2.5/streamlitopencvplayer/
--rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.2.5/streamlitopencvplayer/__init__.py
--rw-rw-rw-   0        0        0     6621 2023-06-19 23:36:44.000000 streamlitopencvplayer-1.2.5/streamlitopencvplayer/app.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:38:05.156644 streamlitopencvplayer-1.2.5/streamlitopencvplayer.egg-info/
--rw-rw-rw-   0        0        0      419 2023-06-19 23:38:04.000000 streamlitopencvplayer-1.2.5/streamlitopencvplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-06-19 23:38:04.000000 streamlitopencvplayer-1.2.5/streamlitopencvplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 23:38:04.000000 streamlitopencvplayer-1.2.5/streamlitopencvplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-19 23:38:04.000000 streamlitopencvplayer-1.2.5/streamlitopencvplayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 23:38:05.172800 streamlitopencvplayer-1.2.5/test/
--rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.2.5/test/__init__.py
--rw-rw-rw-   0        0        0      240 2023-06-19 14:52:06.000000 streamlitopencvplayer-1.2.5/test/app.py
--rw-rw-rw-   0        0        0     2607 2023-06-19 10:50:47.000000 streamlitopencvplayer-1.2.5/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:50:41.446071 streamlitopencvplayer-1.2.6/
+-rw-rw-rw-   0        0        0      419 2023-06-19 23:50:41.445071 streamlitopencvplayer-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      685 2023-05-25 23:06:12.000000 streamlitopencvplayer-1.2.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-19 23:50:41.448075 streamlitopencvplayer-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      934 2023-06-19 23:50:37.000000 streamlitopencvplayer-1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:50:41.411654 streamlitopencvplayer-1.2.6/streamlitopencvplayer/
+-rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.2.6/streamlitopencvplayer/__init__.py
+-rw-rw-rw-   0        0        0     6712 2023-06-19 23:50:14.000000 streamlitopencvplayer-1.2.6/streamlitopencvplayer/app.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:50:41.428221 streamlitopencvplayer-1.2.6/streamlitopencvplayer.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-06-19 23:50:41.000000 streamlitopencvplayer-1.2.6/streamlitopencvplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-06-19 23:50:41.000000 streamlitopencvplayer-1.2.6/streamlitopencvplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 23:50:41.000000 streamlitopencvplayer-1.2.6/streamlitopencvplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-19 23:50:41.000000 streamlitopencvplayer-1.2.6/streamlitopencvplayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 23:50:41.439863 streamlitopencvplayer-1.2.6/test/
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.2.6/test/__init__.py
+-rw-rw-rw-   0        0        0      240 2023-06-19 14:52:06.000000 streamlitopencvplayer-1.2.6/test/app.py
+-rw-rw-rw-   0        0        0     1901 2023-06-19 23:47:36.000000 streamlitopencvplayer-1.2.6/test/test.py
```

### Comparing `streamlitopencvplayer-1.2.5/README.md` & `streamlitopencvplayer-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `streamlitopencvplayer-1.2.5/setup.py` & `streamlitopencvplayer-1.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.2.5' 
+VERSION = '1.2.6' 
 DESCRIPTION = 'Streamlit Opencv player'
 LONG_DESCRIPTION = 'Streamlit Opencv Player is a video player written in python for easy video playback and frames management using OpenCV'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="streamlitopencvplayer",
```

### Comparing `streamlitopencvplayer-1.2.5/streamlitopencvplayer/app.py` & `streamlitopencvplayer-1.2.6/streamlitopencvplayer/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,33 +19,34 @@
     st.session_state['name_vid_sel'] = "1678352121.8713963_1678352127.8713963"
 
 
 # Function to display video in the Streamlit app
 
 def display_video(video_path, json_file):
     # Open the video file
-    # Opening JSON file and returns JSON object as a dictionnary
-    response = urllib.request.urlopen(json_file)
-    fileReader = json.loads(response.read())
-    list_json = []
-    list_json.append(fileReader['timestamp'])
-    list_json.append(fileReader['data'])
-    st.session_state['alerts_list'].append(list_json)
-    #st.write(st.session_state['alerts_list'])
     cap = cv2.VideoCapture(video_path)
     fps = cap.get(cv2.CAP_PROP_FPS)
+    # Opening JSON file and returns JSON object as a dictionnary
+    if json_file is not None:
+        response = urllib.request.urlopen(json_file)
+        fileReader = json.loads(response.read())
+        list_json = []
+        list_json.append(fileReader['timestamp'])
+        list_json.append(fileReader['data'])
+        st.session_state['alerts_list'].append(list_json)
+        #st.write(st.session_state['alerts_list'])
 
-    if not st.session_state['alerts'] and not st.session_state['data'] :
-        st.session_state['alerts'] = []
-        st.session_state['data'] = []
-        for x in range(len(st.session_state['alerts_list'])):
-            time_alert = st.session_state['alerts_list'][x][0]-float(
-                st.session_state['name_vid_sel'].partition('_')[0])
-            st.session_state['alerts'].append(int((time_alert)*fps))
-            st.session_state['data'].append(st.session_state['alerts_list'][x][1])
+        if not st.session_state['alerts'] and not st.session_state['data'] :
+            st.session_state['alerts'] = []
+            st.session_state['data'] = []
+            for x in range(len(st.session_state['alerts_list'])):
+                time_alert = st.session_state['alerts_list'][x][0]-float(
+                    st.session_state['name_vid_sel'].partition('_')[0])
+                st.session_state['alerts'].append(int((time_alert)*fps))
+                st.session_state['data'].append(st.session_state['alerts_list'][x][1])
     i = 0
     #st.write(st.session_state['alerts'])
     data = st.session_state['data']
     alerts = st.session_state['alerts']
     resume = False
     column1, column2, column3 = st.columns([1, 2, 1])
     with column1:
```

### Comparing `streamlitopencvplayer-1.2.5/test/test.py` & `streamlitopencvplayer-1.2.6/test/test.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 """Test script."""
 
 import argparse
 import uuid
 
 import streamlit as st
-from ..streamlitopencvplayer.app import display_video
+from streamlitopencvplayer.app import display_video
 
 #from streamlitopencvplayer.app import display_video
 
 # Initiate all session states used
 if 'counter' not in st.session_state:
     st.session_state['counter'] = 0
 if 'frames' not in st.session_state:
     st.session_state['frames'] = []
 
 
 class opencvplayer:
     """Class streamlit opencv player."""
 
-    def __init__(self, video_path, alerts_dict={}, alerts=[], data=[]):
+    def __init__(self, video_path, json_file):
         self.video_path = video_path
-        self.alerts_dict = alerts_dict
-        self.alerts = alerts
-        self.data = data
+        self.json_file = json_file
+
 
     #@st.cache_data()
     def main(self):
         """Test function.
 
         Args:
             video_path (required): video file path or video url.
@@ -39,40 +38,27 @@
                 self.data = [[[10, 100, 290, 200], 0.82, 0, "Class 0"],
                         [[55, 22, 100, 120], 0.9, 1, "Class 1"]]
 
         Returns:
             The video Player.
         """
         if self.video_path is not None:
-            return display_video(self.video_path, self.alerts_dict, self.alerts, self.data)
+            return display_video(self.video_path, self.json_file)
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description="Runnnig...")
     parser.add_argument(
         "--video-path",
         "-V",
         help="Enter the video path",
         default=str(uuid.uuid4().hex),
     )
-    parser.add_argument("--alerts-dict",
-                        "-T",
-                        default={"Alerts": []},
-                        help="Add alerts time to dict"
-                        )
-    parser.add_argument("--alerts",
-                        "-A",
-                        default=[],
-                        type=list,
-                        help="Add alerts time to list"
-                        )
-
-    parser.add_argument("--data",
-                        "-D",
-                        default=[],
-                        type=list,
-                        help="Add bounding box coordinates, score and class to list"
-                        )
+    parser.add_argument(
+        "--json-file",
+        "-J",
+        help="Enter the json file path",
+    )
     args = parser.parse_args()
     opencvplayer = opencvplayer(
-        args.video_path, args.alerts_dict, args.alerts, args.data)
+        args.video_path, args.json_file)
     opencvplayer.main()
```

