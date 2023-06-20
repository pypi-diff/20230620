# Comparing `tmp/pyautosrt-0.2.6.tar.gz` & `tmp/pyautosrt-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyautosrt-0.2.6.tar", last modified: Mon Jun 19 03:35:21 2023, max compression
+gzip compressed data, was "pyautosrt-0.2.7.tar", last modified: Tue Jun 20 10:42:12 2023, max compression
```

## Comparing `pyautosrt-0.2.6.tar` & `pyautosrt-0.2.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 03:35:21.499935 pyautosrt-0.2.6/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 pyautosrt-0.2.6/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 pyautosrt-0.2.6/MANIFEST.in
--rw-rw-rw-   0        0        0     2055 2023-06-19 03:35:21.500682 pyautosrt-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     3452 2023-04-24 17:27:22.000000 pyautosrt-0.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 03:35:21.407783 pyautosrt-0.2.6/pyautosrt/
--rw-rw-rw-   0        0        0   222764 2023-06-19 03:35:00.000000 pyautosrt-0.2.6/pyautosrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 03:35:21.491689 pyautosrt-0.2.6/pyautosrt.egg-info/
--rw-rw-rw-   0        0        0     2055 2023-06-19 03:35:20.000000 pyautosrt-0.2.6/pyautosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-06-19 03:35:21.000000 pyautosrt-0.2.6/pyautosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 03:35:20.000000 pyautosrt-0.2.6/pyautosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-06-19 03:35:20.000000 pyautosrt-0.2.6/pyautosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      114 2023-06-19 03:35:20.000000 pyautosrt-0.2.6/pyautosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-19 03:35:20.000000 pyautosrt-0.2.6/pyautosrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-06-19 03:35:21.517164 pyautosrt-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1772 2023-06-19 03:34:35.000000 pyautosrt-0.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 03:35:21.495439 pyautosrt-0.2.6/test/
--rw-rw-rw-   0        0        0    40142 2023-04-15 02:08:42.000000 pyautosrt-0.2.6/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:42:12.509774 pyautosrt-0.2.7/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 pyautosrt-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 pyautosrt-0.2.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     2055 2023-06-20 10:42:12.509774 pyautosrt-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3452 2023-04-24 17:27:22.000000 pyautosrt-0.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 10:42:12.454354 pyautosrt-0.2.7/pyautosrt/
+-rw-rw-rw-   0        0        0   227755 2023-06-20 08:43:49.000000 pyautosrt-0.2.7/pyautosrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:42:12.491816 pyautosrt-0.2.7/pyautosrt.egg-info/
+-rw-rw-rw-   0        0        0     2055 2023-06-20 10:42:12.000000 pyautosrt-0.2.7/pyautosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-06-20 10:42:12.000000 pyautosrt-0.2.7/pyautosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 10:42:12.000000 pyautosrt-0.2.7/pyautosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-20 10:42:12.000000 pyautosrt-0.2.7/pyautosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      114 2023-06-20 10:42:12.000000 pyautosrt-0.2.7/pyautosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-20 10:42:12.000000 pyautosrt-0.2.7/pyautosrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-06-20 10:42:12.512776 pyautosrt-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1772 2023-06-19 03:34:35.000000 pyautosrt-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:42:12.507526 pyautosrt-0.2.7/test/
+-rw-rw-rw-   0        0        0    40142 2023-04-15 02:08:42.000000 pyautosrt-0.2.7/test/__init__.py
```

### Comparing `pyautosrt-0.2.6/LICENSE` & `pyautosrt-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyautosrt-0.2.6/PKG-INFO` & `pyautosrt-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyautosrt
-Version: 0.2.6
+Version: 0.2.7
 Summary: pyautosrt is a python based desktop app to generate subtitle and translated subtitle file
 Home-page: https://github.com/botbahlul/pyautosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `pyautosrt-0.2.6/README.md` & `pyautosrt-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `pyautosrt-0.2.6/pyautosrt/__init__.py` & `pyautosrt-0.2.7/pyautosrt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,146 +37,16 @@
 import shlex
 
 #import warnings
 #warnings.filterwarnings("ignore", category=DeprecationWarning)
 #warnings.filterwarnings("ignore", category=RuntimeWarning)
 #sys.tracebacklimit = 0
 
-VERSION = "0.2.6"
 
-
-def stop_ffmpeg_windows(error_messages_callback=None):
-    try:
-        tasklist_output = subprocess.check_output(['tasklist'], creationflags=subprocess.CREATE_NO_WINDOW).decode('utf-8')
-        ffmpeg_pid = None
-        for line in tasklist_output.split('\n'):
-            if "ffmpeg" in line:
-                ffmpeg_pid = line.split()[1]
-                break
-        if ffmpeg_pid:
-            devnull = open(os.devnull, 'w')
-            subprocess.Popen(['taskkill', '/F', '/T', '/PID', ffmpeg_pid], stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
-
-    except KeyboardInterrupt:
-        if error_messages_callback:
-            error_messages_callback("Cancelling all tasks")
-        else:
-            print("Cancelling all tasks")
-        return
-
-    except Exception as e:
-        if error_messages_callback:
-            error_messages_callback(e)
-        else:
-            print(e)
-        return
-
-
-def stop_ffmpeg_linux(error_messages_callback=None):
-    process_name = 'ffmpeg'
-    try:
-        output = subprocess.check_output(['ps', '-ef'])
-        pid = [line.split()[1] for line in output.decode('utf-8').split('\n') if process_name in line][0]
-        subprocess.call(['kill', '-9', str(pid)])
-        #print(f"{process_name} has been killed")
-    except IndexError:
-        #print(f"{process_name} is not running")
-        pass
-
-    except KeyboardInterrupt:
-        if error_messages_callback:
-            error_messages_callback("Cancelling all tasks")
-        else:
-            print("Cancelling all tasks")
-        return
-
-    except Exception as e:
-        if error_messages_callback:
-            error_messages_callback(e)
-        else:
-            print(e)
-        return
-
-
-def remove_temp_files(extension, error_messages_callback=None):
-    try:
-        temp_dir = tempfile.gettempdir()
-        for root, dirs, files in os.walk(temp_dir):
-            for file in files:
-                if file.endswith("." + extension):
-                    os.remove(os.path.join(root, file))
-    except KeyboardInterrupt:
-        if error_messages_callback:
-            error_messages_callback("Cancelling all tasks")
-        else:
-            print("Cancelling all tasks")
-        return
-
-    except Exception as e:
-        if error_messages_callback:
-            error_messages_callback(e)
-        else:
-            print(e)
-        return
-
-
-def is_same_language(src, dst, error_messages_callback=None):
-    try:
-        return src.split("-")[0] == dst.split("-")[0]
-    except Exception as e:
-        if error_messages_callback:
-            error_messages_callback(e)
-        else:
-            print(e)
-        return
-
-
-def check_file_type(file_path, error_messages_callback=None):
-    try:
-        if "\\" in file_path:
-            file_path = file_path.replace("\\", "/")
-
-        ffprobe_cmd = [
-                        'ffprobe',
-                        '-hide_banner',
-                        '-v', 'error',
-                        '-loglevel', 'error',
-                        '-show_format',
-                        '-show_streams',
-                        '-print_format',
-                        'json',
-                        file_path
-                      ]
-
-        output = None
-
-        if sys.platform == "win32":
-            output = subprocess.check_output(ffprobe_cmd, stdin=open(os.devnull), stderr=subprocess.PIPE, creationflags=subprocess.CREATE_NO_WINDOW).decode('utf-8')
-        else:
-            output = subprocess.check_output(ffprobe_cmd, stdin=open(os.devnull), stderr=subprocess.PIPE).decode('utf-8')
-
-        data = json.loads(output)
-
-        if 'streams' in data:
-            for stream in data['streams']:
-                if 'codec_type' in stream and stream['codec_type'] == 'audio':
-                    return 'audio'
-                elif 'codec_type' in stream and stream['codec_type'] == 'video':
-                    return 'video'
-
-    except (subprocess.CalledProcessError, json.JSONDecodeError):
-        pass
-
-    except Exception as e:
-        if error_messages_callback:
-            error_messages_callback(e)
-        else:
-            print(e)
-
-    return None
+VERSION = "0.2.7"
 
 
 class Language:
     def __init__(self):
         self.list_codes = []
         self.list_codes.append("af")
         self.list_codes.append("sq")
@@ -885,14 +755,22 @@
                 path = path.strip('"')
                 exe_file = os.path.join(path, program)
                 if is_exe(exe_file):
                     return exe_file
         return None
 
     @staticmethod
+    def ffprobe_check():
+        if WavConverter.which("ffprobe"):
+            return "ffprobe"
+        if WavConverter.which("ffprobe.exe"):
+            return "ffprobe.exe"
+        return None
+
+    @staticmethod
     def ffmpeg_check():
         if WavConverter.which("ffmpeg"):
             return "ffmpeg"
         if WavConverter.which("ffmpeg.exe"):
             return "ffmpeg.exe"
         return None
 
@@ -906,23 +784,31 @@
         temp = tempfile.NamedTemporaryFile(suffix='.wav', delete=False)
 
         if "\\" in media_filepath:
             media_filepath = media_filepath.replace("\\", "/")
 
         if not os.path.isfile(media_filepath):
             if self.error_messages_callback:
-                self.error_messages_callback("The given file does not exist: {0}".format(media_filepath))
+                self.error_messages_callback(f"The given file does not exist: {media_filepath}")
+            else:
+                print(f"The given file does not exist: {media_filepath}")
+                raise Exception(f"Invalid file: {media_filepath}")
+
+        if not self.ffprobe_check():
+            if self.error_messages_callback:
+                self.error_messages_callback("Cannot find ffprobe executable")
             else:
-                print("The given file does not exist: {0}".format(media_filepath))
-                raise Exception("Invalid file: {0}".format(media_filepath))
+                print("Cannot find ffprobe executable")
+                raise Exception("Dependency not found: ffprobe")
+
         if not self.ffmpeg_check():
             if self.error_messages_callback:
-                self.error_messages_callback("ffmpeg: Executable not found on machine.")
+                self.error_messages_callback("Cannot find ffmpeg executable")
             else:
-                print("ffmpeg: Executable not found on machine.")
+                print("Cannot find ffmpeg executable")
                 raise Exception("Dependency not found: ffmpeg")
 
         ffmpeg_command = [
                             'ffmpeg',
                             '-hide_banner',
                             '-loglevel', 'error',
                             '-v', 'error',
@@ -991,19 +877,20 @@
                 self.error_messages_callback("Cancelling all tasks")
             else:
                 print("Cancelling all tasks")
             return
 
         except Exception as e:
             if self.error_messages_callback:
-                self.error_messages_callback(f"WavConverter : {e}")
+                self.error_messages_callback(e)
             else:
-                print(f"WavConverter : {e}")
+                print(e)
             return
 
+
 # DEFINE progress_callback FUNCTION TO SHOW ffmpeg PROGRESS
 # IF WE'RE IN pysimplegui ENVIRONMENT WE CAN DO :
 #def show_progress(info, media_file_display_name, percentage, start_time):
     #global main_window
     #main_window.write_event_value('-UPDATE-PROGRESS-', percentage) AND HANDLE THAT EVENT IN pysimplegui MAIN LOOP
 # IF WE'RE IN console ENVIRONMENT WE CAN DO :
 #def show_progress(info, media_file_display_name, percentage, start_time):
@@ -1079,21 +966,54 @@
                 self.error_messages_callback(e)
             else:
                 print(e)
             return
 
 
 class FLACConverter(object):
+    @staticmethod
+    def which(program):
+        def is_exe(file_path):
+            return os.path.isfile(file_path) and os.access(file_path, os.X_OK)
+        fpath, _ = os.path.split(program)
+        if fpath:
+            if is_exe(program):
+                return program
+        else:
+            for path in os.environ["PATH"].split(os.pathsep):
+                path = path.strip('"')
+                exe_file = os.path.join(path, program)
+                if is_exe(exe_file):
+                    return exe_file
+        return None
+
+    @staticmethod
+    def ffmpeg_check():
+        if FLACConverter.which("ffmpeg"):
+            return "ffmpeg"
+        if FLACConverter.which("ffmpeg.exe"):
+            return "ffmpeg.exe"
+        return None
+
+    #def __init__(self, wav_filepath, include_before=0.25, include_after=0.25):
     def __init__(self, wav_filepath, include_before=0.25, include_after=0.25, error_messages_callback=None):
         self.wav_filepath = wav_filepath
         self.include_before = include_before
         self.include_after = include_after
         self.error_messages_callback = error_messages_callback
 
+    #def __call__(self, region, error_messages_callback=None):
     def __call__(self, region):
+        if not self.ffmpeg_check():
+            if self.error_messages_callback:
+                self.error_messages_callback("Cannot find ffmpeg executable")
+            else:
+                print("Cannot find ffmpeg executable")
+                raise Exception("Dependency not found: ffmpeg")
+
         try:
             if "\\" in self.wav_filepath:
                 self.wav_filepath = self.wav_filepath.replace("\\", "/")
 
             start, end = region
             start = max(0, start - self.include_before)
             end += self.include_after
@@ -1441,44 +1361,45 @@
                 self.error_messages_callback(e)
             else:
                 print(e)
             return
 
 
 class SubtitleStreamParser:
+    @staticmethod
+    def which(program):
+        def is_exe(file_path):
+            return os.path.isfile(file_path) and os.access(file_path, os.X_OK)
+        fpath, _ = os.path.split(program)
+        if fpath:
+            if is_exe(program):
+                return program
+        else:
+            for path in os.environ["PATH"].split(os.pathsep):
+                path = path.strip('"')
+                exe_file = os.path.join(path, program)
+                if is_exe(exe_file):
+                    return exe_file
+        return None
+
+    @staticmethod
+    def ffprobe_check():
+        if SubtitleStreamParser.which("ffprobe"):
+            return "ffprobe"
+        if SubtitleStreamParser.which("ffprobe.exe"):
+            return "ffprobe.exe"
+        return None
+
     def __init__(self, error_messages_callback=None):
         self.error_messages_callback = error_messages_callback
         self._indexes = []
         self._languages = []
         self._timed_subtitles = []
         self._number_of_streams = 0
 
-    def __call__(self, media_filepath):
-        if "\\" in media_filepath:
-            media_filepath = media_filepath.replace("\\", "/")
-        subtitle_streams = self.get_subtitle_streams(media_filepath)
-        subtitle_streams_data = []
-        if subtitle_streams:
-            for subtitle_stream in subtitle_streams:
-                subtitle_stream_index = subtitle_stream['index']
-                subtitle_stream_language = subtitle_stream['language']
-                subtitle_streams_data.append((subtitle_stream_index, subtitle_stream_language))
-
-        subtitle_data = []
-        subtitle_contents = []
-
-        for subtitle_stream_index in range(len(subtitle_streams)):
-            index, language = subtitle_streams_data[subtitle_stream_index]
-            self._indexes.append(index)
-            self._languages.append(language)
-            self._timed_subtitles.append(self.get_timed_subtitles(media_filepath, subtitle_stream_index+1))
-            subtitle_data.append((index, language, self.get_timed_subtitles(media_filepath, subtitle_stream_index+1)))
-
-        self._number_of_streams = len(subtitle_data)
-        return subtitle_data
 
     def get_subtitle_streams(self, media_filepath):
 
         ffprobe_cmd = [
                         'ffprobe',
                         '-hide_banner',
                         '-v', 'error',
@@ -1553,39 +1474,40 @@
                 result = subprocess.run(ffmpeg_cmd, stdin=open(os.devnull), capture_output=True, text=True)
 
             output = result.stdout
 
             timed_subtitles = []
             subtitle_data = []
             lines = output.strip().split('\n')
+            #print(lines)
             subtitles = []
-            subtitle = None
+            subtitles = None
             subtitle_blocks = []
             block = []
             for line in lines:
                 if line.strip() == '':
                     subtitle_blocks.append(block)
                     block = []
                 else:
                     block.append(line.strip())
             subtitle_blocks.append(block)
 
-            # Parse each subtitle block and store as tuple in timed_subtitles list
+            # Parse each subtitles block and store as tuple in timed_subtitles list
             for block in subtitle_blocks:
                 if block:
-                    # Extract start and end times from subtitle block
+                    # Extract start and end times from subtitles block
                     start_time_str, end_time_str = block[1].split(' --> ')
                     time_format = '%H:%M:%S,%f'
                     start_time_time_delta = datetime.strptime(start_time_str, time_format) - datetime.strptime('00:00:00,000', time_format)
                     start_time_total_seconds = start_time_time_delta.total_seconds()
                     end_time_time_delta = datetime.strptime(end_time_str, time_format) - datetime.strptime('00:00:00,000', time_format)
                     end_time_total_seconds = end_time_time_delta.total_seconds()
-                    # Extract subtitle text from subtitle block
-                    subtitle = ' '.join(block[2:])
-                    timed_subtitles.append(((start_time_total_seconds, end_time_total_seconds), subtitle))
+                    # Extract subtitles text from subtitles block
+                    subtitles = ' '.join(block[2:])
+                    timed_subtitles.append(((start_time_total_seconds, end_time_total_seconds), subtitles))
             return timed_subtitles
 
         except FileNotFoundError:
             if self.error_messages_callback:
                 msg = 'ffmpeg not found. Make sure it is installed and added to the system PATH.'
                 self.error_messages_callback(msg)
             else:
@@ -1624,14 +1546,48 @@
         return self.timed_subtitles()[index-1]
 
     def timed_subtitles_of_language(self, language):
         for i in range(self.number_of_streams()):
             if self.languages()[i] == language:
                 return self.timed_subtitles()[i]
 
+    def __call__(self, media_filepath):
+        if "\\" in media_filepath:
+            media_filepath = media_filepath.replace("\\", "/")
+
+        if not self.ffprobe_check():
+            if self.error_messages_callback:
+                self.error_messages_callback("Cannot find ffprobe executable")
+            else:
+                print("Cannot find ffprobe executable")
+                raise Exception("Dependency not found: ffprobe")
+
+        subtitle_streams = self.get_subtitle_streams(media_filepath)
+        subtitle_streams_data = []
+        if subtitle_streams:
+            for subtitle_stream in subtitle_streams:
+                subtitle_stream_index = subtitle_stream['index']
+                subtitle_stream_language = subtitle_stream['language']
+                #print(f"Stream Index: {subtitle_stream_index}, Language: {subtitle_stream_language}")
+                subtitle_streams_data.append((subtitle_stream_index, subtitle_stream_language))
+
+        subtitle_data = []
+        subtitle_contents = []
+
+        for subtitle_stream_index in range(len(subtitle_streams)):
+            index, language = subtitle_streams_data[subtitle_stream_index]
+            self._indexes.append(index)
+            self._languages.append(language)
+            self._timed_subtitles.append(self.get_timed_subtitles(media_filepath, subtitle_stream_index+1))
+            subtitle_data.append((index, language, self.get_timed_subtitles(media_filepath, subtitle_stream_index+1)))
+
+        self._number_of_streams = len(subtitle_data)
+
+        return subtitle_data
+
 
 class MediaSubtitleRenderer:
     @staticmethod
     def which(program):
         def is_exe(file_path):
             return os.path.isfile(file_path) and os.access(file_path, os.X_OK)
         fpath, _ = os.path.split(program)
@@ -1650,14 +1606,22 @@
     def ffmpeg_check():
         if MediaSubtitleRenderer.which("ffmpeg"):
             return "ffmpeg"
         if MediaSubtitleRenderer.which("ffmpeg.exe"):
             return "ffmpeg.exe"
         return None
 
+    @staticmethod
+    def ffprobe_check():
+        if MediaSubtitleRenderer.which("ffprobe"):
+            return "ffprobe"
+        if MediaSubtitleRenderer.which("ffprobe.exe"):
+            return "ffprobe.exe"
+        return None
+
     def __init__(self, subtitle_path=None, language=None, output_path=None, progress_callback=None, error_messages_callback=None):
         self.subtitle_path = subtitle_path
         self.language = language
         self.output_path = output_path
         self.progress_callback = progress_callback
         self.error_messages_callback = error_messages_callback
 
@@ -1667,51 +1631,45 @@
 
         if "\\" in self.subtitle_path:
             self.subtitle_path = self.subtitle_path.replace("\\", "/")
 
         if "\\" in self.output_path:
             self.output_path = self.output_path.replace("\\", "/")
 
-        if ":" in self.subtitle_path:
-            self.subtitle_path = self.subtitle_path.replace(":", "\:")
-
-        subtitle_path_str = None
-        if sys.platform == "win32":
-            if ("[" or "]") in str(self.subtitle_path):
-                subtitle_path_str = str(self.subtitle_path)
-                subtitle_path_str = subtitle_path_str.replace("]", "\]")
-                subtitle_path_str = subtitle_path_str.replace("[", "\[")
+        if not os.path.isfile(media_filepath):
+            if self.error_messages_callback:
+                self.error_messages_callback(f"The given file does not exist: {media_filepath}")
             else:
-                subtitle_path_str = str(self.subtitle_path)
-        else:
-            subtitle_path_str = str(self.subtitle_path)
+                print(f"The given file does not exist: {media_filepath}")
+                raise Exception(f"Invalid file: {media_filepath}")
 
-        if not os.path.isfile(media_filepath):
+        if not self.ffprobe_check():
             if self.error_messages_callback:
-                self.error_messages_callback("The given file does not exist: {0}".format(media_filepath))
+                self.error_messages_callback("Cannot find ffprobe executable")
             else:
-                print("The given file does not exist: {0}".format(media_filepath))
-                raise Exception("Invalid file: {0}".format(media_filepath))
+                print("Cannot find ffprobe executable")
+                raise Exception("Dependency not found: ffprobe")
+
         if not self.ffmpeg_check():
             if self.error_messages_callback:
-                self.error_messages_callback("ffmpeg: Executable not found on machine.")
+                self.error_messages_callback("Cannot find ffmpeg executable")
             else:
-                print("ffmpeg: Executable not found on machine.")
+                print("Cannot find ffmpeg executable")
                 raise Exception("Dependency not found: ffmpeg")
 
         try:
             scale_switch = "'trunc(iw/2)*2'\:'trunc(ih/2)*2'"
             ffmpeg_command = [
                                 'ffmpeg',
                                 '-hide_banner',
                                 '-loglevel', 'error',
                                 '-v', 'error',
                                 '-y',
                                 '-i', media_filepath,
-                                '-vf', f'subtitles={shlex.quote(subtitle_path_str)},scale={scale_switch}',
+                                '-vf', f'subtitles={shlex.quote(self.subtitle_path)},scale={scale_switch}',
                                 '-c:v', 'libx264',
                                 '-crf', '23',
                                 '-preset', 'medium',
                                 '-c:a', 'copy',
                                 '-progress', '-', '-nostats',
                                 self.output_path
                              ]
@@ -1797,14 +1755,22 @@
                 path = path.strip('"')
                 exe_file = os.path.join(path, program)
                 if is_exe(exe_file):
                     return exe_file
         return None
 
     @staticmethod
+    def ffprobe_check():
+        if MediaSubtitleEmbedder.which("ffprobe"):
+            return "ffprobe"
+        if MediaSubtitleEmbedder.which("ffprobe.exe"):
+            return "ffprobe.exe"
+        return None
+
+    @staticmethod
     def ffmpeg_check():
         if MediaSubtitleEmbedder.which("ffmpeg"):
             return "ffmpeg"
         if MediaSubtitleEmbedder.which("ffmpeg.exe"):
             return "ffmpeg.exe"
         return None
 
@@ -1857,23 +1823,31 @@
             self.subtitle_path = self.subtitle_path.replace("\\", "/")
 
         if "\\" in self.output_path:
             self.output_path = self.output_path.replace("\\", "/")
 
         if not os.path.isfile(media_filepath):
             if self.error_messages_callback:
-                self.error_messages_callback("The given file does not exist: {0}".format(media_filepath))
+                self.error_messages_callback(f"The given file does not exist: {media_filepath}")
+            else:
+                print(f"The given file does not exist: {media_filepath}")
+                raise Exception(f"Invalid file: {media_filepath}")
+
+        if not self.ffprobe_check():
+            if self.error_messages_callback:
+                self.error_messages_callback("Cannot find ffprobe executable")
             else:
-                print("The given file does not exist: {0}".format(media_filepath))
-                raise Exception("Invalid file: {0}".format(media_filepath))
+                print("Cannot find ffprobe executable")
+                raise Exception("Dependency not found: ffprobe")
+
         if not self.ffmpeg_check():
             if self.error_messages_callback:
-                self.error_messages_callback("ffmpeg: Executable not found on machine.")
+                self.error_messages_callback("Cannot find ffmpeg executable")
             else:
-                print("ffmpeg: Executable not found on machine.")
+                print("Cannot find ffmpeg executable")
                 raise Exception("Dependency not found: ffmpeg")
 
         try:
             existing_languages = self.get_existing_subtitle_language(media_filepath)
             if self.language in existing_languages:
                 # THIS 'print' THINGS WILL MAKE progresbar screwed up!
                 #msg = (f"'{self.language}' subtitle stream already existed in {media_filepath}")
@@ -1993,14 +1967,22 @@
                 path = path.strip('"')
                 exe_file = os.path.join(path, program)
                 if is_exe(exe_file):
                     return exe_file
         return None
 
     @staticmethod
+    def ffprobe_check():
+        if MediaSubtitleRemover.which("ffprobe"):
+            return "ffprobe"
+        if MediaSubtitleRemover.which("ffprobe.exe"):
+            return "ffprobe.exe"
+        return None
+
+    @staticmethod
     def ffmpeg_check():
         if MediaSubtitleRemover.which("ffmpeg"):
             return "ffmpeg"
         if MediaSubtitleRemover.which("ffmpeg.exe"):
             return "ffmpeg.exe"
         return None
 
@@ -2014,23 +1996,31 @@
             media_filepath = media_filepath.replace("\\", "/")
 
         if "\\" in self.output_path:
             self.output_path = self.output_path.replace("\\", "/")
 
         if not os.path.isfile(media_filepath):
             if self.error_messages_callback:
-                self.error_messages_callback("The given file does not exist: {0}".format(media_filepath))
+                self.error_messages_callback(f"The given file does not exist: {media_filepath}")
+            else:
+                print(f"The given file does not exist: {media_filepath}")
+                raise Exception(f"Invalid file: {media_filepath}")
+
+        if not self.ffprobe_check():
+            if self.error_messages_callback:
+                self.error_messages_callback("Cannot find ffprobe executable")
             else:
-                print("The given file does not exist: {0}".format(media_filepath))
-                raise Exception("Invalid file: {0}".format(media_filepath))
+                print("Cannot find ffprobe executable")
+                raise Exception("Dependency not found: ffprobe")
+
         if not self.ffmpeg_check():
             if self.error_messages_callback:
-                self.error_messages_callback("ffmpeg: Executable not found on machine.")
+                self.error_messages_callback("Cannot find ffmpeg executable")
             else:
-                print("ffmpeg: Executable not found on machine.")
+                print("Cannot find ffmpeg executable")
                 raise Exception("Dependency not found: ffmpeg")
 
         try:
             ffmpeg_command = [
                                 'ffmpeg',
                                 '-hide_banner',
                                 '-loglevel', 'error',
@@ -2040,15 +2030,15 @@
                                 '-c', 'copy',
                                 '-sn',
                                 '-progress', '-', '-nostats',
                                 self.output_path
                              ]
 
             media_file_display_name = os.path.basename(media_filepath).split('/')[-1]
-            info = f"Removing subtitle streams from '{media_file_display_name}'"
+            info = f"Removing subtitles streams from '{media_file_display_name}'"
             start_time = time.time()
 
             ffprobe_command = [
                                 'ffprobe',
                                 '-hide_banner',
                                 '-v', 'error',
                                 '-loglevel', 'error',
@@ -2111,15 +2101,179 @@
             if self.error_messages_callback:
                 self.error_messages_callback(e)
             else:
                 print(e)
             return
 
 
-#=======================================================================================================================================#
+def stop_ffmpeg_windows(error_messages_callback=None):
+    try:
+        tasklist_output = subprocess.check_output(['tasklist'], creationflags=subprocess.CREATE_NO_WINDOW).decode('utf-8')
+        ffmpeg_pid = None
+        for line in tasklist_output.split('\n'):
+            if "ffmpeg" in line:
+                ffmpeg_pid = line.split()[1]
+                break
+        if ffmpeg_pid:
+            devnull = open(os.devnull, 'w')
+            subprocess.Popen(['taskkill', '/F', '/T', '/PID', ffmpeg_pid], stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
+
+    except KeyboardInterrupt:
+        if error_messages_callback:
+            error_messages_callback("Cancelling all tasks")
+        else:
+            print("Cancelling all tasks")
+        return
+
+    except Exception as e:
+        if error_messages_callback:
+            error_messages_callback(e)
+        else:
+            print(e)
+        return
+
+
+def stop_ffmpeg_linux(error_messages_callback=None):
+    process_name = 'ffmpeg'
+    try:
+        output = subprocess.check_output(['ps', '-ef'])
+        pid = [line.split()[1] for line in output.decode('utf-8').split('\n') if process_name in line][0]
+        subprocess.call(['kill', '-9', str(pid)])
+        #print(f"{process_name} has been killed")
+    except IndexError:
+        #print(f"{process_name} is not running")
+        pass
+
+    except KeyboardInterrupt:
+        if error_messages_callback:
+            error_messages_callback("Cancelling all tasks")
+        else:
+            print("Cancelling all tasks")
+        return
+
+    except Exception as e:
+        if error_messages_callback:
+            error_messages_callback(e)
+        else:
+            print(e)
+        return
+
+
+def remove_temp_files(extension, error_messages_callback=None):
+    try:
+        temp_dir = tempfile.gettempdir()
+        for root, dirs, files in os.walk(temp_dir):
+            for file in files:
+                if file.endswith("." + extension):
+                    os.remove(os.path.join(root, file))
+    except KeyboardInterrupt:
+        if error_messages_callback:
+            error_messages_callback("Cancelling all tasks")
+        else:
+            print("Cancelling all tasks")
+        return
+
+    except Exception as e:
+        if error_messages_callback:
+            error_messages_callback(e)
+        else:
+            print(e)
+        return
+
+
+def is_same_language(src, dst, error_messages_callback=None):
+    try:
+        return src.split("-")[0] == dst.split("-")[0]
+    except Exception as e:
+        if error_messages_callback:
+            error_messages_callback(e)
+        else:
+            print(e)
+        return
+
+
+def check_file_type(media_filepath, error_messages_callback=None):
+    def which(program):
+        def is_exe(file_path):
+            return os.path.isfile(file_path) and os.access(file_path, os.X_OK)
+        fpath, _ = os.path.split(program)
+        if fpath:
+            if is_exe(program):
+                return program
+        else:
+            for path in os.environ["PATH"].split(os.pathsep):
+                path = path.strip('"')
+                exe_file = os.path.join(path, program)
+                if is_exe(exe_file):
+                    return exe_file
+        return None
+
+    def ffprobe_check():
+        if which("ffprobe"):
+            return "ffprobe"
+        if which("ffprobe.exe"):
+            return "ffprobe.exe"
+        return None
+
+    if "\\" in media_filepath:
+        media_filepath = media_filepath.replace("\\", "/")
+
+    if not os.path.isfile(media_filepath):
+        if error_messages_callback:
+           error_messages_callback(f"The given file does not exist: {media_filepath}")
+        else:
+            print(f"The given file does not exist: {media_filepath}")
+            raise Exception(f"Invalid file: {media_filepath}")
+    if not ffprobe_check():
+        if error_messages_callback:
+            error_messages_callback("Cannot find ffprobe executable")
+        else:
+            print("Cannot find ffprobe executable")
+            raise Exception("Dependency not found: ffprobe")
+
+    try:
+        ffprobe_cmd = [
+                        'ffprobe',
+                        '-hide_banner',
+                        '-loglevel', 'error',
+                        '-v', 'error',
+                        '-show_format',
+                        '-show_streams',
+                        '-print_format',
+                        'json',
+                        media_filepath
+                      ]
+
+        output = None
+
+        if sys.platform == "win32":
+            output = subprocess.check_output(ffprobe_cmd, stdin=open(os.devnull), stderr=subprocess.PIPE, creationflags=subprocess.CREATE_NO_WINDOW).decode('utf-8')
+        else:
+            output = subprocess.check_output(ffprobe_cmd, stdin=open(os.devnull), stderr=subprocess.PIPE).decode('utf-8')
+
+        data = json.loads(output)
+
+        if 'streams' in data:
+            for stream in data['streams']:
+                if 'codec_type' in stream and stream['codec_type'] == 'audio':
+                    return 'audio'
+                elif 'codec_type' in stream and stream['codec_type'] == 'video':
+                    return 'video'
+
+    except (subprocess.CalledProcessError, json.JSONDecodeError):
+        pass
+
+    except Exception as e:
+        if error_messages_callback:
+            error_messages_callback(e)
+        else:
+            print(e)
+
+    return None
+
 
 #----------------------------------------------------------- MISC FUNCTIONS -----------------------------------------------------------#
 
 
 def stop_thread(thread):
     global main_window
     exc = ctypes.py_object(SystemExit)
```

### Comparing `pyautosrt-0.2.6/pyautosrt.egg-info/PKG-INFO` & `pyautosrt-0.2.7/pyautosrt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyautosrt
-Version: 0.2.6
+Version: 0.2.7
 Summary: pyautosrt is a python based desktop app to generate subtitle and translated subtitle file
 Home-page: https://github.com/botbahlul/pyautosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `pyautosrt-0.2.6/setup.py` & `pyautosrt-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `pyautosrt-0.2.6/test/__init__.py` & `pyautosrt-0.2.7/test/__init__.py`

 * *Files identical despite different names*

