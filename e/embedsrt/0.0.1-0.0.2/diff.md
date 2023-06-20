# Comparing `tmp/embedsrt-0.0.1.tar.gz` & `tmp/embedsrt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedsrt-0.0.1.tar", last modified: Wed Jun  7 14:27:25 2023, max compression
+gzip compressed data, was "embedsrt-0.0.2.tar", last modified: Tue Jun 20 09:12:44 2023, max compression
```

## Comparing `embedsrt-0.0.1.tar` & `embedsrt-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 14:27:25.688803 embedsrt-0.0.1/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 embedsrt-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 embedsrt-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1560 2023-06-07 14:27:25.688803 embedsrt-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3199 2023-06-07 14:26:01.000000 embedsrt-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 14:27:25.664828 embedsrt-0.0.1/embedsrt/
--rw-rw-rw-   0        0        0    61903 2023-06-07 14:21:06.000000 embedsrt-0.0.1/embedsrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:27:25.686557 embedsrt-0.0.1/embedsrt.egg-info/
--rw-rw-rw-   0        0        0     1560 2023-06-07 14:27:25.000000 embedsrt-0.0.1/embedsrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-06-07 14:27:25.000000 embedsrt-0.0.1/embedsrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 14:27:25.000000 embedsrt-0.0.1/embedsrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-06-07 14:27:25.000000 embedsrt-0.0.1/embedsrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2023-06-07 14:27:25.000000 embedsrt-0.0.1/embedsrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-07 14:27:25.000000 embedsrt-0.0.1/embedsrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-06-07 14:27:25.691800 embedsrt-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1355 2023-06-07 14:21:47.000000 embedsrt-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 09:12:44.908788 embedsrt-0.0.2/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 embedsrt-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 embedsrt-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1560 2023-06-20 09:12:44.909539 embedsrt-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3199 2023-06-07 14:26:01.000000 embedsrt-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 09:12:44.866832 embedsrt-0.0.2/embedsrt/
+-rw-rw-rw-   0        0        0    71202 2023-06-20 08:55:52.000000 embedsrt-0.0.2/embedsrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 09:12:44.906541 embedsrt-0.0.2/embedsrt.egg-info/
+-rw-rw-rw-   0        0        0     1560 2023-06-20 09:12:44.000000 embedsrt-0.0.2/embedsrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-06-20 09:12:44.000000 embedsrt-0.0.2/embedsrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 09:12:44.000000 embedsrt-0.0.2/embedsrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-06-20 09:12:44.000000 embedsrt-0.0.2/embedsrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2023-06-20 09:12:44.000000 embedsrt-0.0.2/embedsrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-20 09:12:44.000000 embedsrt-0.0.2/embedsrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-06-20 09:12:44.911786 embedsrt-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1355 2023-06-07 14:21:47.000000 embedsrt-0.0.2/setup.py
```

### Comparing `embedsrt-0.0.1/LICENSE` & `embedsrt-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `embedsrt-0.0.1/PKG-INFO` & `embedsrt-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedsrt
-Version: 0.0.1
+Version: 0.0.2
 Summary: a utility for embedding subtitle file into video file
 Home-page: https://github.com/botbahlul/embedsrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `embedsrt-0.0.1/README.md` & `embedsrt-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `embedsrt-0.0.1/embedsrt/__init__.py` & `embedsrt-0.0.2/embedsrt/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 from progressbar import ProgressBar, Percentage, Bar, ETA
 from glob import glob, escape
 import shlex
 import json
 import pysrt
 from pathlib import Path
 from datetime import datetime, timedelta
+import time
 
 
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 
 
 class Language:
     def __init__(self):
         self.list_codes = []
         self.list_codes.append("af")
         self.list_codes.append("sq")
@@ -744,25 +745,33 @@
             self._timed_subtitles.append(self.get_timed_subtitles(media_filepath, subtitle_stream_index+1))
             subtitle_data.append((index, language, self.get_timed_subtitles(media_filepath, subtitle_stream_index+1)))
 
         self._number_of_streams = len(subtitle_data)
         return subtitle_data
 
     def get_subtitle_streams(self, media_filepath):
+
         ffprobe_cmd = [
                         'ffprobe',
-                        '-v', 'quiet',
+                        '-hide_banner',
+                        '-v', 'error',
+                        '-loglevel', 'error',
                         '-print_format', 'json',
                         '-show_entries', 'stream=index:stream_tags=language',
                         '-select_streams', 's',
                         media_filepath
                       ]
 
         try:
-            result = subprocess.run(ffprobe_cmd, capture_output=True, text=True)
+            result = None
+            if sys.platform == "win32":
+                result = subprocess.run(ffprobe_cmd, stdin=open(os.devnull), capture_output=True, text=True, creationflags=subprocess.CREATE_NO_WINDOW)
+            else:
+                result = subprocess.run(ffprobe_cmd, stdin=open(os.devnull), capture_output=True, text=True)
+
             output = result.stdout
 
             streams = json.loads(output)['streams']
 
             subtitle_streams = []
             empty_stream_exists = False
 
@@ -792,56 +801,64 @@
             if self.error_messages_callback:
                 self.error_messages_callback(e)
             else:
                 print(e)
             return None
 
     def get_timed_subtitles(self, media_filepath, subtitle_stream_index):
+
         ffmpeg_cmd = [
                         'ffmpeg',
+                        '-hide_banner',
+                        '-loglevel', 'error',
+                        '-v', 'error',
                         '-i', media_filepath,
                         '-map', f'0:s:{subtitle_stream_index-1}',
                         '-f', 'srt',
                         '-'
                      ]
 
         try:
-            result = subprocess.run(ffmpeg_cmd, capture_output=True, text=True)
+            result = None
+            if sys.platform == "win32":
+                result = subprocess.run(ffmpeg_cmd, stdin=open(os.devnull), capture_output=True, text=True, creationflags=subprocess.CREATE_NO_WINDOW)
+            else:
+                result = subprocess.run(ffmpeg_cmd, stdin=open(os.devnull), capture_output=True, text=True)
+
             output = result.stdout
-			#print(output)
 
             timed_subtitles = []
             subtitle_data = []
             lines = output.strip().split('\n')
             #print(lines)
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
@@ -884,61 +901,72 @@
             if self.languages()[i] == language:
                 return self.timed_subtitles()[i]
 
 
 class MediaSubtitleEmbedder:
     @staticmethod
     def which(program):
-        def is_exe(media_filepath):
-            return os.path.isfile(media_filepath) and os.access(media_filepath, os.X_OK)
+        def is_exe(file_path):
+            return os.path.isfile(file_path) and os.access(file_path, os.X_OK)
         fpath, _ = os.path.split(program)
         if fpath:
             if is_exe(program):
                 return program
         else:
             for path in os.environ["PATH"].split(os.pathsep):
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
 
-    def __init__(self, subtitle_path=None, language="eng", output_path=None, progress_callback=None, error_messages_callback=None):
+    def __init__(self, subtitle_path=None, language=None, output_path=None, progress_callback=None, error_messages_callback=None):
         self.subtitle_path = subtitle_path
         self.language = language
         self.output_path = output_path
         self.progress_callback = progress_callback
         self.error_messages_callback = error_messages_callback
 
     def get_existing_subtitle_language(self, media_filepath):
         # Run ffprobe to get stream information
         if "\\" in media_filepath:
             media_filepath = media_filepath.replace("\\", "/")
 
         command = [
                     'ffprobe',
-                    '-v', 'quiet',
+                    '-hide_banner',
+                    '-v', 'error',
+                    '-loglevel', 'error',
                     '-of', 'json',
                     '-show_entries',
                     'format:stream',
                     media_filepath
                   ]
 
+        output = None
         if sys.platform == "win32":
-            output = subprocess.run(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True, universal_newlines=True)
+            output = subprocess.run(command, stdin=open(os.devnull), stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
         else:
-            output = subprocess.run(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True)
+            output = subprocess.run(command, stdin=open(os.devnull), stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True)
 
         metadata = json.loads(output.stdout)
         streams = metadata['streams']
 
         # Find the subtitle stream with language metadata
         subtitle_languages = []
         for stream in streams:
@@ -956,23 +984,31 @@
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
@@ -984,53 +1020,77 @@
 
             else:
                 # Determine the next available subtitle index
                 next_index = len(existing_languages)
 
                 ffmpeg_command = [
                                     'ffmpeg',
+                                    '-hide_banner',
+                                    '-loglevel', 'error',
+                                    '-v', 'error',
                                     '-y',
                                     '-i', media_filepath,
                                     '-sub_charenc', 'UTF-8',
                                     '-i', self.subtitle_path,
                                     '-c:v', 'copy',
                                     '-c:a', 'copy',
                                     '-scodec', 'mov_text',
                                     '-metadata:s:s:' + str(next_index), f'language={shlex.quote(self.language)}',
                                     '-map', '0',
                                     '-map', '1',
+                                    '-progress', '-', '-nostats',
                                     self.output_path
                                  ]
 
+                subtitle_file_display_name = os.path.basename(self.subtitle_path).split('/')[-1]
+                media_file_display_name = os.path.basename(media_filepath).split('/')[-1]
+                info = f"Embedding '{self.language}' subtitles file '{subtitle_file_display_name}' into '{media_file_display_name}'"
+                start_time = time.time()
+
+                ffprobe_command = [
+                                    'ffprobe',
+                                    '-hide_banner',
+                                    '-v', 'error',
+                                    '-loglevel', 'error',
+                                    '-show_entries',
+                                    'format=duration',
+                                    '-of', 'default=noprint_wrappers=1:nokey=1',
+                                    media_filepath
+                                  ]
 
-                ffprobe_command = f'ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 "{media_filepath}"'
+                ffprobe_process = None
                 if sys.platform == "win32":
-                    ffprobe_process = subprocess.Popen(ffprobe_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+                    ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
                 else:
-                    ffprobe_process = subprocess.Popen(ffprobe_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+                    ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True)
 
-                total_duration = float(ffprobe_process.stdout.read().decode('utf-8').strip())
+                total_duration = float(ffprobe_process.strip())
 
+                process = None
                 if sys.platform == "win32":
-                    process = subprocess.Popen(ffmpeg_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
+                    process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
                 else:
-                    process = subprocess.Popen(ffmpeg_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
+                    process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
 
-                for line in process.stdout:
-                    if "time=" in line:
-                        #print(line)
-                        time_str = line.split("time=")[1].split()[0]
-                        #print("time_str = %s" %time_str)
-                        current_duration = sum(float(x) * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
-                        #print("current_duration = %s" %current_duration)
+                while True:
+                    if process.stdout is None:
+                        continue
+
+                    stderr_line = (process.stdout.readline().decode("utf-8", errors="replace").strip())
+ 
+                    if stderr_line == '' and process.poll() is not None:
+                        break
+
+                    if "out_time=" in stderr_line:
+                        time_str = stderr_line.split('time=')[1].split()[0]
+                        current_duration = sum(float(x) * 1000 * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
                         if current_duration>0:
-                            percentage = int(current_duration*100/total_duration)
+                            percentage = int(current_duration*100/(int(float(total_duration))*1000))
                             if self.progress_callback:
-                                self.progress_callback(media_filepath, percentage)
-
+                                self.progress_callback(info, media_file_display_name, percentage, start_time)
 
                 if os.path.isfile(self.output_path):
                     return self.output_path
                 else:
                     return None
 
                 if os.path.isfile(self.output_path):
@@ -1049,30 +1109,231 @@
             if self.error_messages_callback:
                 self.error_messages_callback(e)
             else:
                 print(e)
             return
 
 
-def check_file_type(file_path, error_messages_callback=None):
+def embed_subtitle_into_media(media_filepath, media_type, subtitle_path, language_code, output_path, error_messages_callback=None):
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
+    def ffmpeg_check():
+        if which("ffmpeg"):
+            return "ffmpeg"
+        if which("ffmpeg.exe"):
+            return "ffmpeg.exe"
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
+
+    if not ffprobe_check():
+        if error_messages_callback:
+            error_messages_callback("Cannot find ffprobe executable")
+        else:
+            print("Cannot find ffprobe executable")
+            raise Exception("Dependency not found: ffprobe")
+
+    if not ffmpeg_check():
+        if error_messages_callback:
+            error_messages_callback("Cannot find ffmpeg executable")
+        else:
+            print("Cannot find ffmpeg executable")
+            raise Exception("Dependency not found: ffmpeg")
+
+    try:
+        if "\\" in media_filepath:
+            media_filepath = media_filepath.replace("\\", "/")
+
+        if "\\" in subtitle_path:
+            subtitle_path = subtitle_path.replace("\\", "/")
+
+        if "\\" in output_path:
+            output_path = output_path.replace("\\", "/")
+
+        existing_languages = get_existing_subtitle_language(media_filepath)
+        if language_code in existing_languages:
+            #print(f"'{language_code}' subtitles stream already existed in {media_filepath}")
+            return
+
+        else:
+            # Determine the next available subtitles index
+            next_index = len(existing_languages)
+
+            ffmpeg_command = [
+                                'ffmpeg',
+                                '-hide_banner',
+                                '-loglevel', 'error',
+                                '-v', 'error',
+                                '-y',
+                                '-i', media_filepath,
+                                '-sub_charenc', 'UTF-8',
+                                '-i', subtitle_path,
+                                '-c:v', 'copy',
+                                '-c:a', 'copy',
+                                '-scodec', 'mov_text',
+                                '-metadata:s:s:' + str(next_index), f'language={shlex.quote(language_code)}',
+                                '-map', '0',
+                                '-map', '1',
+                                output_path
+                             ]
+
+            ffprobe_command = [
+                                'ffprobe',
+                                '-hide_banner',
+                                '-v', 'error',
+                                '-loglevel', 'error',
+                                '-show_entries',
+                                'format=duration',
+                                '-of', 'default=noprint_wrappers=1:nokey=1',
+                                media_filepath
+                             ]
+
+            ffprobe_process = None
+            if sys.platform == "win32":
+                ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
+            else:
+                ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True)
+
+            total_duration = float(ffprobe_process.strip())
+
+            widgets = [f"Embedding '{language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+            pbar = ProgressBar(widgets=widgets, maxval=100).start()
+            percentage = 0
+
+            process = None
+            if sys.platform == "win32":
+                process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
+            else:
+                process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+
+            while True:
+                if process.stdout is None:
+                    continue
+
+                stderr_line = (process.stdout.readline().decode("utf-8", errors="replace").strip())
+ 
+                if stderr_line == '' and process.poll() is not None:
+                    break
+
+                if "out_time=" in stderr_line:
+                    time_str = stderr_line.split('time=')[1].split()[0]
+                    current_duration = sum(float(x) * 1000 * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
+                    if current_duration>0:
+                        percentage = int(current_duration*100/(int(float(total_duration))*1000))
+                        pbar.update(percentage)
+            pbar.finish()
+
+            return output_path
+
+        return
+
+    except Exception as e:
+        if error_messages_callback:
+            error_messages_callback(e)
+        else:
+            print(e)
+        return None
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
     try:
-        ffprobe_cmd = ['ffprobe', '-v', 'error', '-show_format', '-show_streams', '-print_format', 'json', file_path]
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
         output = None
+
         if sys.platform == "win32":
-            output = subprocess.check_output(ffprobe_cmd, creationflags=subprocess.CREATE_NO_WINDOW).decode('utf-8')
+            output = subprocess.check_output(ffprobe_cmd, stdin=open(os.devnull), stderr=subprocess.PIPE, creationflags=subprocess.CREATE_NO_WINDOW).decode('utf-8')
         else:
-            output = subprocess.check_output(ffprobe_cmd).decode('utf-8')
+            output = subprocess.check_output(ffprobe_cmd, stdin=open(os.devnull), stderr=subprocess.PIPE).decode('utf-8')
+
         data = json.loads(output)
 
         if 'streams' in data:
             for stream in data['streams']:
                 if 'codec_type' in stream and stream['codec_type'] == 'audio':
                     return 'audio'
                 elif 'codec_type' in stream and stream['codec_type'] == 'video':
                     return 'video'
+
     except (subprocess.CalledProcessError, json.JSONDecodeError):
         pass
 
     except Exception as e:
         if error_messages_callback:
             error_messages_callback(e)
         else:
@@ -1093,120 +1354,101 @@
             return False
             if error_messages_callback:
                 error_messages_callback(e)
             else:
                 print(e)
         
 
-def show_progress(media_filepath, progress):
-    global pbar
-    pbar.update(progress)
-
-
-def show_error_messages(messages):
-    print(messages)
-
+def get_existing_subtitle_language(media_path):
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
 
-def get_existing_subtitle_language(media_filepath):
-    # Run ffprobe to get stream information
-    command = [
-                'ffprobe',
-                '-v', 'quiet',
-                '-of', 'json',
-                '-show_entries',
-                'format:stream',
-                media_filepath
-    ]
-
-    output = subprocess.run(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True, universal_newlines=True)
-    metadata = json.loads(output.stdout)
-    streams = metadata['streams']
-
-    # Find the subtitle stream with language metadata
-    subtitle_languages = []
-    for stream in streams:
-        if stream['codec_type'] == 'subtitle' and 'tags' in stream and 'language' in stream['tags']:
-            language = stream['tags']['language']
-            subtitle_languages.append(language)
+    def ffprobe_check():
+        if which("ffprobe"):
+            return "ffprobe"
+        if which("ffprobe.exe"):
+            return "ffprobe.exe"
+        return None
 
-    return subtitle_languages
+    if "\\" in media_filepath:
+        media_filepath = media_filepath.replace("\\", "/")
 
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
 
-def embed_subtitle_to_media(media_filepath, media_type, subtitle_path, language_code, output_path, error_messages_callback=None):
     try:
-        if "\\" in media_filepath:
-            media_filepath = media_filepath.replace("\\", "/")
-
-        if "\\" in subtitle_path:
-            subtitle_path = subtitle_path.replace("\\", "/")
-
-        if "\\" in output_path:
-            output_path = output_path.replace("\\", "/")
-
-        existing_languages = get_existing_subtitle_language(media_filepath)
-        if language_code in existing_languages:
-            print(f"A subtitle stream with language '{language_code}' already exists.")
-            return
-
-        # Determine the next available subtitle index
-        next_index = len(existing_languages)
-
-        ffprobe_command = f'ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 "{media_filepath}"'
-        ffprobe_process = subprocess.Popen(ffprobe_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
-        total_duration = float(ffprobe_process.stdout.read().decode().strip())
-
-        #ffmpeg_command = f'ffmpeg -y -i "{media_filepath}" -vf "subtitles={shlex.quote(subtitle_path)}" "{output_path}"'
-
-        ffmpeg_command = [
-                            'ffmpeg',
-                            '-y',
-                            '-i', media_filepath,
-                            '-sub_charenc', 'UTF-8',
-                            '-i', subtitle_path,
-                            '-c:v', 'copy',
-                            '-c:a', 'copy',
-                            '-scodec', 'mov_text',
-                            '-metadata:s:s:' + str(next_index), f'language={shlex.quote(language_code)}',
-                            '-map', '0',
-                            '-map', '1',
-                            output_path
-                         ]
-
-        widgets = [f"Embeding \'{language_code}\' subtitles with {media_type} : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
-        #widgets = [f"Embeding subtitles with {media_type} : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
-        pbar = ProgressBar(widgets=widgets, maxval=100).start()
-        percentage = 0
+        # Run ffprobe to get stream information
+        command = [
+                    'ffprobe',
+                    '-hide_banner',
+                    '-v', 'error',
+                    '-loglevel', 'error',
+                    '-of', 'json',
+                    '-show_entries',
+                    'format:stream',
+                    media_path
+                  ]
 
+        output = None
         if sys.platform == "win32":
-            process = subprocess.Popen(ffmpeg_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
+            output = subprocess.run(command, stdin=open(os.devnull), stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
         else:
-            process = subprocess.Popen(ffmpeg_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
+            output = subprocess.run(command, stdin=open(os.devnull), stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True)
 
-        for line in process.stdout:
-            if "time=" in line:
-                #print(line)
-                time_str = line.split("time=")[1].split()[0]
-                #print("time_str = %s" %time_str)
-                current_duration = sum(float(x) * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
-                #print("current_duration = %s" %current_duration)
-                if current_duration>0:
-                    percentage = int(current_duration*100/total_duration)
-                    #print("percentage = {}%".format(percentage))
-                    pbar.update(percentage)
-        pbar.finish()
-        return output_path
+        metadata = json.loads(output.stdout)
+        streams = metadata['streams']
+
+        # Find the subtitles stream with language metadata
+        subtitle_languages = []
+        for stream in streams:
+            if stream['codec_type'] == 'subtitles' and 'tags' in stream and 'language' in stream['tags']:
+                language = stream['tags']['language']
+                subtitle_languages.append(language)
+
+        return subtitle_languages
 
     except Exception as e:
-        if error_messages_callback:
-            error_messages_callback(e)
+        if self.error_messages_callback:
+            self.error_messages_callback(e)
         else:
             print(e)
         return None
 
 
+def show_progress(info, media_file_display_name, percentage, start_time):
+    global pbar
+    pbar.update(percentage)
+
+
+def show_error_messages(messages):
+    print(messages)
+
+
 def main():
     global pbar
 
     parser = argparse.ArgumentParser()
     parser.add_argument('media_filepath', help="video file path", nargs='?')
     parser.add_argument('subtitle_file_path', help="SRT subtitle file path", nargs='?')
     parser.add_argument('language', help="ffmpeg subtitle language code", nargs='?')
@@ -1376,15 +1618,15 @@
                 src_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_src_language_code)
 
                 if ffmpeg_src_language_code in subtitle_stream_parser.languages():
                     print("Is '%s' subtitle stream exist      : Yes" %(ffmpeg_src_language_code.center(3)))
                 else:
                     print("Is '%s' subtitle stream exist      : No" %(ffmpeg_src_language_code.center(3)))
 
-                    #result = embed_subtitle_to_media(media_filepaths[0], media_type, valid_subtitle_paths[0], language_code, output_path)
+                    #result = embed_subtitle_into_media(media_filepaths[0], media_type, valid_subtitle_paths[0], language_code, output_path)
 
                     widgets = [f"Embeding \'{language_code}\' subtitles with {media_type} : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                     pbar = ProgressBar(widgets=widgets, maxval=100).start()
                     subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=valid_subtitle_paths[0], language=language_code, output_path=output_path, progress_callback=show_progress, error_messages_callback=show_error_messages)
                     result = subtitle_embedder(media_filepaths[0])
                     pbar.finish()
```

### Comparing `embedsrt-0.0.1/embedsrt.egg-info/PKG-INFO` & `embedsrt-0.0.2/embedsrt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedsrt
-Version: 0.0.1
+Version: 0.0.2
 Summary: a utility for embedding subtitle file into video file
 Home-page: https://github.com/botbahlul/embedsrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `embedsrt-0.0.1/setup.py` & `embedsrt-0.0.2/setup.py`

 * *Files identical despite different names*

