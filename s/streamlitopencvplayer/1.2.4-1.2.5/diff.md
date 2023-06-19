# Comparing `tmp/streamlitopencvplayer-1.2.4.tar.gz` & `tmp/streamlitopencvplayer-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlitopencvplayer-1.2.4.tar", last modified: Thu Jun  8 14:39:54 2023, max compression
+gzip compressed data, was "streamlitopencvplayer-1.2.5.tar", last modified: Mon Jun 19 23:38:05 2023, max compression
```

## Comparing `streamlitopencvplayer-1.2.4.tar` & `streamlitopencvplayer-1.2.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 14:39:54.936495 streamlitopencvplayer-1.2.4/
--rw-rw-rw-   0        0        0      419 2023-06-08 14:39:54.935492 streamlitopencvplayer-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0      685 2023-05-25 23:06:12.000000 streamlitopencvplayer-1.2.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-08 14:39:54.937493 streamlitopencvplayer-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0      934 2023-06-08 14:39:22.000000 streamlitopencvplayer-1.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-08 14:39:54.903494 streamlitopencvplayer-1.2.4/streamlitopencvplayer/
--rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.2.4/streamlitopencvplayer/__init__.py
--rw-rw-rw-   0        0        0     6901 2023-06-08 14:39:32.000000 streamlitopencvplayer-1.2.4/streamlitopencvplayer/app.py
-drwxrwxrwx   0        0        0        0 2023-06-08 14:39:54.925502 streamlitopencvplayer-1.2.4/streamlitopencvplayer.egg-info/
--rw-rw-rw-   0        0        0      419 2023-06-08 14:39:54.000000 streamlitopencvplayer-1.2.4/streamlitopencvplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-06-08 14:39:54.000000 streamlitopencvplayer-1.2.4/streamlitopencvplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 14:39:54.000000 streamlitopencvplayer-1.2.4/streamlitopencvplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-08 14:39:54.000000 streamlitopencvplayer-1.2.4/streamlitopencvplayer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-08 14:39:54.931492 streamlitopencvplayer-1.2.4/test/
--rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.2.4/test/__init__.py
--rw-rw-rw-   0        0        0     2528 2023-06-08 14:36:47.000000 streamlitopencvplayer-1.2.4/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:38:05.178075 streamlitopencvplayer-1.2.5/
+-rw-rw-rw-   0        0        0      419 2023-06-19 23:38:05.177076 streamlitopencvplayer-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0      685 2023-05-25 23:06:12.000000 streamlitopencvplayer-1.2.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-19 23:38:05.180076 streamlitopencvplayer-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      934 2023-06-19 23:36:26.000000 streamlitopencvplayer-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:38:05.132035 streamlitopencvplayer-1.2.5/streamlitopencvplayer/
+-rw-rw-rw-   0        0        0        0 2023-05-22 10:55:16.000000 streamlitopencvplayer-1.2.5/streamlitopencvplayer/__init__.py
+-rw-rw-rw-   0        0        0     6621 2023-06-19 23:36:44.000000 streamlitopencvplayer-1.2.5/streamlitopencvplayer/app.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:38:05.156644 streamlitopencvplayer-1.2.5/streamlitopencvplayer.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-06-19 23:38:04.000000 streamlitopencvplayer-1.2.5/streamlitopencvplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-06-19 23:38:04.000000 streamlitopencvplayer-1.2.5/streamlitopencvplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 23:38:04.000000 streamlitopencvplayer-1.2.5/streamlitopencvplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-19 23:38:04.000000 streamlitopencvplayer-1.2.5/streamlitopencvplayer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 23:38:05.172800 streamlitopencvplayer-1.2.5/test/
+-rw-rw-rw-   0        0        0        0 2023-05-22 15:15:43.000000 streamlitopencvplayer-1.2.5/test/__init__.py
+-rw-rw-rw-   0        0        0      240 2023-06-19 14:52:06.000000 streamlitopencvplayer-1.2.5/test/app.py
+-rw-rw-rw-   0        0        0     2607 2023-06-19 10:50:47.000000 streamlitopencvplayer-1.2.5/test/test.py
```

### Comparing `streamlitopencvplayer-1.2.4/README.md` & `streamlitopencvplayer-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `streamlitopencvplayer-1.2.4/setup.py` & `streamlitopencvplayer-1.2.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.2.4' 
+VERSION = '1.2.5' 
 DESCRIPTION = 'Streamlit Opencv player'
 LONG_DESCRIPTION = 'Streamlit Opencv Player is a video player written in python for easy video playback and frames management using OpenCV'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="streamlitopencvplayer",
```

### Comparing `streamlitopencvplayer-1.2.4/streamlitopencvplayer/app.py` & `streamlitopencvplayer-1.2.5/streamlitopencvplayer/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,87 @@
 import time
+import urllib.request,json
 
 import cv2
-import pandas as pd
 import streamlit as st
-from st_aggrid import AgGrid, GridOptionsBuilder
 
 # Initiate all session states used
 if 'counter' not in st.session_state:
     st.session_state['counter'] = 0
 if 'frames' not in st.session_state:
     st.session_state['frames'] = []
+if 'alerts' not in st.session_state:
+    st.session_state['alerts'] = []
+if 'data' not in st.session_state:
+    st.session_state['data'] = []
+if 'alerts_list' not in st.session_state:
+    st.session_state['alerts_list'] = []
+if 'name_vid_sel' not in st.session_state:
+    st.session_state['name_vid_sel'] = "1678352121.8713963_1678352127.8713963"
 
-# Use a callback to display the current value of the slider when changed
-
-
-def display_value():
-    if 'myslider' in st.session_state:
-        st.session_state['counter'] = st.session_state.myslider
 
 # Function to display video in the Streamlit app
 
-
-def display_video(video_path, alerts_dict, alerts, data):
+def display_video(video_path, json_file):
     # Open the video file
+    # Opening JSON file and returns JSON object as a dictionnary
+    response = urllib.request.urlopen(json_file)
+    fileReader = json.loads(response.read())
+    list_json = []
+    list_json.append(fileReader['timestamp'])
+    list_json.append(fileReader['data'])
+    st.session_state['alerts_list'].append(list_json)
+    #st.write(st.session_state['alerts_list'])
     cap = cv2.VideoCapture(video_path)
     fps = cap.get(cv2.CAP_PROP_FPS)
-    i = 0
 
+    if not st.session_state['alerts'] and not st.session_state['data'] :
+        st.session_state['alerts'] = []
+        st.session_state['data'] = []
+        for x in range(len(st.session_state['alerts_list'])):
+            time_alert = st.session_state['alerts_list'][x][0]-float(
+                st.session_state['name_vid_sel'].partition('_')[0])
+            st.session_state['alerts'].append(int((time_alert)*fps))
+            st.session_state['data'].append(st.session_state['alerts_list'][x][1])
+    i = 0
+    #st.write(st.session_state['alerts'])
+    data = st.session_state['data']
+    alerts = st.session_state['alerts']
     resume = False
     column1, column2, column3 = st.columns([1, 2, 1])
     with column1:
         # zone to display images
         stframe = st.empty()
     with column3:
-        # Display the table
-        df = pd.DataFrame(alerts_dict)
-        options_builder = GridOptionsBuilder.from_dataframe(df)
-        options_builder.configure_selection(
-            selection_mode="single", use_checkbox=True)
-        grid_options = options_builder.build()
-        grid_return = AgGrid(df, grid_options)
-        selected_rows = grid_return["selected_rows"]
+        # Alerts
+        st.subheader('Alerts :')
+        num_buttons = len(alerts)
+
+        button_values = {f'{i}': 0 for i in range(num_buttons)}
+
+        for button_label, button_value in button_values.items():
+            if st.button(str('Alert ')+button_label):
+                button_values = {label: 1 if label == button_label else 0 for label in button_values}
+
+        for button_label, button_value in button_values.items():
+            if button_value == 1:
+                st.session_state['counter'] = alerts[int(button_label)]
+                #st.write(f'Alert "{button_label}", Frame: {alerts[int(button_label)]}')
+
+
     # Buttons and zone of display
     col1, col2, col3, col4, col5 = st.columns([1,1,1,1,1])
     with col1:
         st.write('')
         st.write('')
         container_2 = st.empty()
         pause = container_2.button('⏸')
 
     with col2:
-        widget = st.empty()
-        # Create a Streamlit slider for navigating the video
-        widget.slider("", min_value=0, max_value=int(
-            cap.get(cv2.CAP_PROP_FRAME_COUNT)), value=st.session_state['counter'], key="myslider", on_change=display_value)
-        if 'myslider'  in st.session_state:
-            st.session_state['counter'] = st.session_state.myslider
+        st.write('')
     with col3:
         st.write('')
         st.write('')
         replay = st.button("↻")
     with col4:
         st.write('')
         st.write('')
@@ -69,44 +91,30 @@
         st.write('')
         minus = st.button("➖")
 
     if replay:
         st.session_state['counter'] = 0
         st.session_state['frames'] = []
         resume = False
-    if selected_rows:
-        selected_rows = grid_return["selected_rows"][0]["Alerts"]
 
-        if plus:
-            st.session_state['counter'] = st.session_state['counter']+1
-        elif minus:
-            st.session_state['counter'] = st.session_state['counter']-1
-        else:
-            st.session_state['counter'] = selected_rows
 
-        widget.slider("", min_value=0, max_value=int(
-            cap.get(cv2.CAP_PROP_FRAME_COUNT)), value=st.session_state['counter'], on_change=display_value)
-        container_2.empty()
-        pause = container_2.button('▶')
-        resume = True
         # get all the frames from video when the list is empty
     if not st.session_state['frames']:
         while True:
             successs, frames = cap.read()
             if successs:
                 frames = cv2.cvtColor(frames, cv2.COLOR_BGR2RGB)
                 st.session_state['frames'].append(frames)
             else:
                 break
         cap.release()
     # back to the first frame if the video is finished
     if st.session_state['counter'] == len(st.session_state['frames']):
         st.session_state['counter'] = 0
-        if 'myslider' in st.session_state:
-            del st.session_state.myslider
+
     stframe.image(st.session_state['frames']
                   [st.session_state['counter']], caption='', width=450)
 
     while st.session_state['counter'] < len(st.session_state['frames']):
         if not resume:
             if i < len(data):
                 if st.session_state['counter'] == int(alerts[i]*fps):
@@ -118,54 +126,51 @@
                             st.session_state['frames'][st.session_state['counter']], data[i][j][3], (data[i][j][0][0], data[i][j][0][1]-10), cv2.FONT_HERSHEY_SIMPLEX, 0.9, (0, 0, 255), 2)
                     # update image zone with detections
                     stframe.image(output, caption='', width=500)
                     time.sleep(0.08)
                     # the detection is drawn, to the next one
                     i += 1
                     st.session_state['counter'] += 1
-                    # frame_number.slider_changed(st.session_state['counter'])
 
-                    # update slider value
-                    widget.slider("", min_value=0, max_value=int(
-                        cap.get(cv2.CAP_PROP_FRAME_COUNT)), value=st.session_state['counter'], on_change=display_value)
             stframe.image(
                 st.session_state['frames'][st.session_state['counter']], caption='', width=500)
             time.sleep(0.08)
             st.session_state['counter'] += 1
-            # update slider value
-
-            frame_num = widget.slider("", min_value=0, max_value=int(
-                cap.get(cv2.CAP_PROP_FRAME_COUNT)), value=st.session_state['counter'], on_change=display_value)
-            if 'myslider' in st.session_state:
-                if st.session_state.myslider > frame_num:
-                    del st.session_state.myslider
-                    #st.session_state.clear()
-                    st.session_state['counter'] = frame_num
-                    #st.session_state['counter'] = 0
-                    resume = True
-                    #st.experimental_rerun() #remove cache
                 
 
             if pause:
                 resume = True
                 break
             if plus:
                 resume = True
                 break
             if minus:
-                st.session_state['counter'] = st.session_state['counter']-2                
+                st.session_state['counter'] = st.session_state['counter']-2           
                 resume = True
                 break
-            if replay:
-                st.session_state['counter'] = 0
-                st.session_state['frames'] = []
+
                 # back to the first frame if the video is finished
             if st.session_state['counter'] == len(st.session_state['frames']):
                 st.session_state['counter'] = 0
-                if 'myslider'  in st.session_state:
-                    del st.session_state.myslider
-            st.session_state['counter'] = frame_num
+                resume = True
+                break
+
 
     if resume:
         container_2.empty()
         pause = container_2.button('▶')
         resume = False
+
+def main():
+
+
+    video_path = "https://cvlogger.blob.core.windows.net/clientsample/1678352121.8713963_1678352127.8713963.webm?se=2023-06-20T10%3A49%3A01Z&sp=r&sv=2021-08-06&sr=b&sig=9o/0AhqY8v3E%2B8WATBI69aYNddekddb49g9YuXG1wVU%3D"
+    down_json = "https://cvlogger.blob.core.windows.net/clientsample/1678352123.8713963.json?sp=r&st=2023-06-19T22:46:06Z&se=2023-06-20T16:46:06Z&sv=2022-11-02&sr=b&sig=GoE3UurhwkYgjKRd7yiBVRpKgIPHCt0WvTEK84CERqg%3D"
+    
+    if video_path is not None:
+        display_video(video_path, down_json)
+
+
+
+if __name__ == "__main__":
+    main()
+
```

### Comparing `streamlitopencvplayer-1.2.4/test/test.py` & `streamlitopencvplayer-1.2.5/test/test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Test script."""
 
 import argparse
 import uuid
 
 import streamlit as st
+from ..streamlitopencvplayer.app import display_video
 
-from streamlitopencvplayer.app import display_video
+#from streamlitopencvplayer.app import display_video
 
 # Initiate all session states used
 if 'counter' not in st.session_state:
     st.session_state['counter'] = 0
 if 'frames' not in st.session_state:
     st.session_state['frames'] = []
 
@@ -19,14 +20,15 @@
 
     def __init__(self, video_path, alerts_dict={}, alerts=[], data=[]):
         self.video_path = video_path
         self.alerts_dict = alerts_dict
         self.alerts = alerts
         self.data = data
 
+    #@st.cache_data()
     def main(self):
         """Test function.
 
         Args:
             video_path (required): video file path or video url.
             alerts_dict (Optional) : Dictionary of alerts passed to the alerts table.
             alerts (Required when data is used) : List of alerts time
```

