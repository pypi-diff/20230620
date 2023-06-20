# Comparing `tmp/autosrt-1.4.2.tar.gz` & `tmp/autosrt-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosrt-1.4.2.tar", last modified: Mon Jun 19 08:36:33 2023, max compression
+gzip compressed data, was "autosrt-1.4.3.tar", last modified: Tue Jun 20 10:29:50 2023, max compression
```

## Comparing `autosrt-1.4.2.tar` & `autosrt-1.4.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 08:36:33.049387 autosrt-1.4.2/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.4.2/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.4.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2018 2023-06-19 08:36:33.050137 autosrt-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     5260 2023-04-30 04:22:31.000000 autosrt-1.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 08:36:32.776081 autosrt-1.4.2/autosrt/
--rw-rw-rw-   0        0        0   147744 2023-06-19 08:36:00.000000 autosrt-1.4.2/autosrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:36:32.981958 autosrt-1.4.2/autosrt.egg-info/
--rw-rw-rw-   0        0        0     2018 2023-06-19 08:36:32.000000 autosrt-1.4.2/autosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-06-19 08:36:32.000000 autosrt-1.4.2/autosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 08:36:32.000000 autosrt-1.4.2/autosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-06-19 08:36:32.000000 autosrt-1.4.2/autosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       97 2023-06-19 08:36:32.000000 autosrt-1.4.2/autosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-19 08:36:32.000000 autosrt-1.4.2/autosrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-06-19 08:36:33.097098 autosrt-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-06-03 00:59:56.000000 autosrt-1.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 08:36:33.035901 autosrt-1.4.2/test/
--rw-rw-rw-   0        0        0     7435 2023-06-06 20:34:53.000000 autosrt-1.4.2/test/test1.py
--rw-rw-rw-   0        0        0     4481 2023-06-06 20:37:56.000000 autosrt-1.4.2/test/test2.py
--rw-rw-rw-   0        0        0     9938 2023-06-06 20:52:44.000000 autosrt-1.4.2/test/test3.py
--rw-rw-rw-   0        0        0    68818 2023-06-16 20:05:01.000000 autosrt-1.4.2/test/test4.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:29:50.945791 autosrt-1.4.3/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.4.3/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.4.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2018 2023-06-20 10:29:50.946539 autosrt-1.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5260 2023-04-30 04:22:31.000000 autosrt-1.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 10:29:50.740152 autosrt-1.4.3/autosrt/
+-rw-rw-rw-   0        0        0   161800 2023-06-20 08:16:41.000000 autosrt-1.4.3/autosrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:29:50.825841 autosrt-1.4.3/autosrt.egg-info/
+-rw-rw-rw-   0        0        0     2018 2023-06-20 10:29:50.000000 autosrt-1.4.3/autosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-06-20 10:29:50.000000 autosrt-1.4.3/autosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 10:29:50.000000 autosrt-1.4.3/autosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-20 10:29:50.000000 autosrt-1.4.3/autosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       97 2023-06-20 10:29:50.000000 autosrt-1.4.3/autosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-20 10:29:50.000000 autosrt-1.4.3/autosrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-06-20 10:29:50.951036 autosrt-1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-06-03 00:59:56.000000 autosrt-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:29:50.941295 autosrt-1.4.3/test/
+-rw-rw-rw-   0        0        0     7435 2023-06-06 20:34:53.000000 autosrt-1.4.3/test/test1.py
+-rw-rw-rw-   0        0        0     4481 2023-06-06 20:37:56.000000 autosrt-1.4.3/test/test2.py
+-rw-rw-rw-   0        0        0     9938 2023-06-06 20:52:44.000000 autosrt-1.4.3/test/test3.py
+-rw-rw-rw-   0        0        0    68818 2023-06-16 20:05:01.000000 autosrt-1.4.3/test/test4.py
```

### Comparing `autosrt-1.4.2/LICENSE` & `autosrt-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `autosrt-1.4.2/PKG-INFO` & `autosrt-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosrt
-Version: 1.4.2
+Version: 1.4.3
 Summary: a utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `autosrt-1.4.2/README.md` & `autosrt-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `autosrt-1.4.2/autosrt/__init__.py` & `autosrt-1.4.3/autosrt/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,143 +24,15 @@
 import time
 from datetime import datetime, timedelta
 from pathlib import Path
 import shlex
 import shutil
 
 
-VERSION = "1.4.2"
-
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
-def check_file_type(media_filepath, error_messages_callback=None):
-    try:
-        ffprobe_cmd = [
-                        'ffprobe',
-                        '-hide_banner',
-                        '-loglevel', 'error',
-                        '-v', 'error',
-                        '-show_format',
-                        '-show_streams',
-                        '-print_format',
-                        'json',
-                        media_filepath
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
+VERSION = "1.4.3"
 
 
 class Language:
     def __init__(self):
         self.list_codes = []
         self.list_codes.append("af")
         self.list_codes.append("sq")
@@ -854,29 +726,37 @@
     def get_ffmpeg_code(self, code):
         return self.ffmpeg_code_of_code[code]
 
 
 class WavConverter:
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
 
@@ -890,23 +770,31 @@
         temp = tempfile.NamedTemporaryFile(suffix='.wav', delete=False)
 
         if "\\" in media_filepath:
             media_filepath = media_filepath.replace("\\", "/")
 
         if not os.path.isfile(media_filepath):
             if self.error_messages_callback:
-                self.error_messages_callback("The given file does not exist: {0}".format(media_filepath))
+                self.error_messages_callback(f"The given file does not exist: {media_filepath}")
             else:
-                print("The given file does not exist: {0}".format(media_filepath))
-                raise Exception("Invalid file: {0}".format(media_filepath))
+                print(f"The given file does not exist: {media_filepath}")
+                raise Exception(f"Invalid file: {media_filepath}")
+
+        if not self.ffprobe_check():
+            if self.error_messages_callback:
+                self.error_messages_callback("Cannot find ffprobe executable")
+            else:
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
@@ -1065,23 +953,54 @@
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
     #def __init__(self, wav_filepath, include_before=0.25, include_after=0.25):
     def __init__(self, wav_filepath, include_before=0.25, include_after=0.25, error_messages_callback=None):
         self.wav_filepath = wav_filepath
         self.include_before = include_before
         self.include_after = include_after
         self.error_messages_callback = error_messages_callback
 
     #def __call__(self, region, error_messages_callback=None):
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
@@ -1131,15 +1050,15 @@
         self.retries = retries
         self.timeout = timeout
         self.error_messages_callback = error_messages_callback
 
     def __call__(self, data):
         try:
             for i in range(self.retries):
-                url = "http://www.google.com/speech-api/v2/recognize?client=chromium&lang={lang}&key={key}".format(lang=self.language, key=self.api_key)
+                url = f"http://www.google.com/speech-api/v2/recognize?client=chromium&lang={self.language}&key={self.api_key}"
                 headers = {"Content-Type": "audio/x-flac rate=%d" % self.rate}
 
                 try:
                     resp = requests.post(url, data=data, headers=headers, timeout=self.timeout)
                 except requests.exceptions.ConnectionError:
                     try:
                         resp = httpx.post(url, data=data, headers=headers, timeout=self.timeout)
@@ -1350,15 +1269,15 @@
         try:
             formatter = SubtitleFormatter(self.format)
             formatted_subtitles = formatter(self.timed_subtitles)
             saved_subtitle_filepath = declared_subtitle_filepath
             if saved_subtitle_filepath:
                 subtitle_file_base, subtitle_file_ext = os.path.splitext(saved_subtitle_filepath)
                 if not subtitle_file_ext:
-                    saved_subtitle_filepath = "{base}.{format}".format(base=subtitle_file_base, format=self.format)
+                    saved_subtitle_filepath = "{subtitle_file_base}.{self.format}"
                 else:
                     saved_subtitle_filepath = declared_subtitle_filepath
             with open(saved_subtitle_filepath, 'wb') as f:
                 f.write(formatted_subtitles.encode("utf-8"))
 
         except KeyboardInterrupt:
             if self.error_messages_callback:
@@ -1372,45 +1291,45 @@
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
-                #print(f"Stream Index: {subtitle_stream_index}, Language: {subtitle_stream_language}")
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
@@ -1557,14 +1476,48 @@
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
@@ -1583,16 +1536,25 @@
     def ffmpeg_check():
         if MediaSubtitleRenderer.which("ffmpeg"):
             return "ffmpeg"
         if MediaSubtitleRenderer.which("ffmpeg.exe"):
             return "ffmpeg.exe"
         return None
 
-    def __init__(self, subtitle_path=None, output_path=None, progress_callback=None, error_messages_callback=None):
+    @staticmethod
+    def ffprobe_check():
+        if MediaSubtitleRenderer.which("ffprobe"):
+            return "ffprobe"
+        if MediaSubtitleRenderer.which("ffprobe.exe"):
+            return "ffprobe.exe"
+        return None
+
+    def __init__(self, subtitle_path=None, language=None, output_path=None, progress_callback=None, error_messages_callback=None):
         self.subtitle_path = subtitle_path
+        self.language = language
         self.output_path = output_path
         self.progress_callback = progress_callback
         self.error_messages_callback = error_messages_callback
 
     def __call__(self, media_filepath):
         if "\\" in media_filepath:
             media_filepath = media_filepath.replace("\\", "/")
@@ -1601,35 +1563,43 @@
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
@@ -1715,14 +1685,22 @@
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
 
@@ -1775,23 +1753,31 @@
             self.subtitle_path = self.subtitle_path.replace("\\", "/")
 
         if "\\" in self.output_path:
             self.output_path = self.output_path.replace("\\", "/")
 
         if not os.path.isfile(media_filepath):
             if self.error_messages_callback:
-                self.error_messages_callback("The given file does not exist: {0}".format(media_filepath))
+                self.error_messages_callback(f"The given file does not exist: {media_filepath}")
             else:
-                print("The given file does not exist: {0}".format(media_filepath))
-                raise Exception("Invalid file: {0}".format(media_filepath))
+                print(f"The given file does not exist: {media_filepath}")
+                raise Exception(f"Invalid file: {media_filepath}")
+
+        if not self.ffprobe_check():
+            if self.error_messages_callback:
+                self.error_messages_callback("Cannot find ffprobe executable")
+            else:
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
@@ -1896,29 +1882,37 @@
                 print(e)
             return
 
 
 class MediaSubtitleRemover:
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
 
@@ -1932,23 +1926,31 @@
             media_filepath = media_filepath.replace("\\", "/")
 
         if "\\" in self.output_path:
             self.output_path = self.output_path.replace("\\", "/")
 
         if not os.path.isfile(media_filepath):
             if self.error_messages_callback:
-                self.error_messages_callback("The given file does not exist: {0}".format(media_filepath))
+                self.error_messages_callback(f"The given file does not exist: {media_filepath}")
             else:
-                print("The given file does not exist: {0}".format(media_filepath))
-                raise Exception("Invalid file: {0}".format(media_filepath))
+                print(f"The given file does not exist: {media_filepath}")
+                raise Exception(f"Invalid file: {media_filepath}")
+
+        if not self.ffprobe_check():
+            if self.error_messages_callback:
+                self.error_messages_callback("Cannot find ffprobe executable")
+            else:
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
@@ -2085,14 +2087,52 @@
                 self.error_messages_callback(e)
             else:
                 print(e)
             return
 
 
 def has_subtitles(media_filepath, error_messages_callback=None):
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
+    if not ffmpeg_check():
+        if error_messages_callback:
+            error_messages_callback("Cannot find ffmpeg executable")
+        else:
+            print("Cannot find ffmpeg executable")
+            raise Exception("Dependency not found: ffmpeg")
+
     try:
         if "\\" in media_filepath:
             media_filepath = media_filepath.replace("\\", "/")
 
         ffmpeg_cmd = [
                         'ffmpeg',
                         '-hide_banner',
@@ -2121,89 +2161,194 @@
             self.error_messages_callback(e)
         else:
             print(e)
         return False
 
 
 def get_existing_subtitle_language(media_path):
-    # Run ffprobe to get stream information
-    command = [
-                'ffprobe',
-                '-hide_banner',
-                '-v', 'error',
-                '-loglevel', 'error',
-                '-of', 'json',
-                '-show_entries',
-                'format:stream',
-                media_path
-              ]
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
 
-    output = None
-    if sys.platform == "win32":
-        output = subprocess.run(command, stdin=open(os.devnull), stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
-    else:
-        output = subprocess.run(command, stdin=open(os.devnull), stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True)
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
 
-    metadata = json.loads(output.stdout)
-    streams = metadata['streams']
+        output = None
+        if sys.platform == "win32":
+            output = subprocess.run(command, stdin=open(os.devnull), stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
+        else:
+            output = subprocess.run(command, stdin=open(os.devnull), stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True)
 
-    # Find the subtitles stream with language metadata
-    subtitle_languages = []
-    for stream in streams:
-        if stream['codec_type'] == 'subtitles' and 'tags' in stream and 'language' in stream['tags']:
-            language = stream['tags']['language']
-            subtitle_languages.append(language)
+        metadata = json.loads(output.stdout)
+        streams = metadata['streams']
 
-    return subtitle_languages
+        # Find the subtitles stream with language metadata
+        subtitle_languages = []
+        for stream in streams:
+            if stream['codec_type'] == 'subtitles' and 'tags' in stream and 'language' in stream['tags']:
+                language = stream['tags']['language']
+                subtitle_languages.append(language)
 
+        return subtitle_languages
+
+    except Exception as e:
+        if self.error_messages_callback:
+            self.error_messages_callback(e)
+        else:
+            print(e)
+        return None
+
+
+def render_subtitle_into_media(media_filepath, media_type, subtitle_path, language_code, output_path, error_messages_callback=None):
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
 
-def render_subtitle_to_media(media_filepath, media_type, media_ext, subtitle_path, output_path, error_messages_callback=None):
     try:
         if "\\" in media_filepath:
             media_filepath = media_filepath.replace("\\", "/")
 
         if "\\" in subtitle_path:
             subtitle_path = subtitle_path.replace("\\", "/")
 
         if "\\" in output_path:
             output_path = output_path.replace("\\", "/")
 
-        scale_switch = "'trunc(iw/2)*2':'trunc(ih/2)*2'"
+        scale_switch = "'trunc(iw/2)*2'\:'trunc(ih/2)*2'"
+
         ffmpeg_command = [
                             'ffmpeg',
+                            '-hide_banner',
+                            '-loglevel', 'error',
+                            '-v', 'error',
                             '-y',
                             '-i', media_filepath,
-                            '-vf', f'subtitles={shlex.quote(self.subtitle_path)},scale={scale_switch}',
+                            '-vf', f'subtitles={shlex.quote(subtitle_path)},scale={scale_switch}',
                             '-c:v', 'libx264',
                             '-crf', '23',
                             '-preset', 'medium',
                             '-c:a', 'copy',
-                            self.output_path
+                            '-progress', '-', '-nostats',
+                            output_path
                          ]
 
         ffprobe_command = [
                             'ffprobe',
                             '-hide_banner',
                             '-v', 'error',
                             '-loglevel', 'error',
                             '-show_entries',
                             'format=duration',
                             '-of', 'default=noprint_wrappers=1:nokey=1',
                             media_filepath
                           ]
 
         ffprobe_process = None
+
         if sys.platform == "win32":
             ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
         else:
             ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True)
 
         total_duration = float(ffprobe_process.strip())
 
-        widgets = [f"Rendering '{language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+        widgets = [f"Rendering '{language_code}' subtitles into {media_type} : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
         pbar = ProgressBar(widgets=widgets, maxval=100).start()
         percentage = 0
 
         process = None
         if sys.platform == "win32":
             process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
         else:
@@ -2228,18 +2373,71 @@
         return output_path
 
     except Exception as e:
         if error_messages_callback:
             error_messages_callback(e)
         else:
             print(e)
-        return
+        return None
+
+
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
 
-def embed_subtitle_to_media(media_filepath, media_type, subtitle_path, language_code, output_path, error_messages_callback=None):
     try:
         if "\\" in media_filepath:
             media_filepath = media_filepath.replace("\\", "/")
 
         if "\\" in subtitle_path:
             subtitle_path = subtitle_path.replace("\\", "/")
 
@@ -2328,14 +2526,67 @@
             error_messages_callback(e)
         else:
             print(e)
         return None
 
 
 def remove_subtitles_from_media(media_filepath, output_path, progress_callback=None, error_messages_callback=None):
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
     try:
         if "\\" in media_filepath:
             media_filepath = media_filepath.replace("\\", "/")
 
         if "\\" in output_path:
             output_path = output_path.replace("\\", "/")
 
@@ -2408,17 +2659,183 @@
         return
 
     except Exception as e:
         if error_messages_callback:
             error_messages_callback(e)
         else:
             print(e)
+        return None
+
+
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
         return
 
 
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
+
 def show_progress(info, media_file_display_name, progress, start_time):
     global pbar
     pbar.update(progress)
 
 
 def show_error_messages(messages):
     print(messages)
@@ -2476,15 +2893,15 @@
             do_translate = False
     else:
         do_translate = False
 
     if args.list_formats:
         print("List of supported subtitles formats:")
         for subtitle_format in SubtitleFormatter.supported_formats:
-            print("{format}".format(format=subtitle_format))
+            print(f"{subtitle_format}")
         return 0
 
     if args.format not in SubtitleFormatter.supported_formats:
         print("Subtitle format is not supported. Run with --list-formats to see all supported formats.")
         return 1
 
     if not args.source_path:
@@ -2545,23 +2962,23 @@
                     media_type = None
             else:
                 not_exist_filepaths.append(argpath)
                 media_type = None
 
         if invalid_media_filepaths:
             for invalid_media_filepath in invalid_media_filepaths:
-                msg = "{} is not valid media files".format(invalid_media_filepath)
+                msg = f"{invalid_media_filepath} is not valid media files"
                 print(msg)
 
     #print("not_exist_filepaths = %s" %(not_exist_filepaths))
 
     if not_exist_filepaths:
         if (not "*" in str(args_source_path)) and (not "?" in str(args_source_path)):
             for not_exist_filepath in not_exist_filepaths:
-                msg = "{} is not exist".format(not_exist_filepath)
+                msg = f"{not_exist_filepath} is not exist"
                 print(msg)
                 sys.exit(0)
 
     if not arg_filepaths and not not_exist_filepaths:
         print("No any files matching filenames you typed")
         sys.exit(0)
 
@@ -2575,15 +2992,15 @@
     dst_subtitle_filepath = None
     ffmpeg_src_language_code = None
     ffmpeg_dst_language_code = None
     embedded_media_filepath = None
 
     subtitle_format = args.format
 
-    #print("media_filepaths = {}".format(media_filepaths))
+    #print(f"media_filepaths = {media_filepaths}")
 
     removed_media_filepaths = []
 
     if args.force_recognize == False:
 
         print("CHECKING EXISTING SUBTITLES STREAMS")
         print("===================================")
@@ -2610,15 +3027,15 @@
                         subtitle_stream_regions = []
                         subtitle_stream_transcripts = []
                         for entry in src_subtitle_stream_timed_subtitles:
                             subtitle_stream_regions.append(entry[0])
                             subtitle_stream_transcripts.append(entry[1])
 
                         base, ext = os.path.splitext(media_filepath)
-                        src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=args.src_language, format=subtitle_format)
+                        src_subtitle_filepath = f"{base}.{args.src_language}.{subtitle_format}"
 
                         print(f"Extracting '{ffmpeg_src_language_code}'subtitles stream as     : {src_subtitle_filepath}")
 
                         writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
                         writer.write(src_subtitle_filepath)
 
                         # no translate process as instructed in command arguments
@@ -2677,15 +3094,15 @@
                         subtitle_stream_regions = []
                         subtitle_stream_transcripts = []
                         for entry in src_subtitle_stream_timed_subtitles:
                             subtitle_stream_regions.append(entry[0])
                             subtitle_stream_transcripts.append(entry[1])
 
                         base, ext = os.path.splitext(media_filepath)
-                        src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=args.src_language, format=subtitle_format)
+                        src_subtitle_filepath = f"{base}.{args.src_language}.{subtitle_format}"
 
                         print(f"Extracting '{ffmpeg_src_language_code}'subtitles stream as     : {src_subtitle_filepath}")
 
                         writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
                         writer.write(src_subtitle_filepath)
 
                     # ffmpeg_src_language_code subtitles stream not exist, just print it
@@ -2699,15 +3116,15 @@
                         subtitle_stream_regions = []
                         subtitle_stream_transcripts = []
                         for entry in dst_subtitle_stream_timed_subtitles:
                             subtitle_stream_regions.append(entry[0])
                             subtitle_stream_transcripts.append(entry[1])
 
                         base, ext = os.path.splitext(media_filepath)
-                        dst_subtitle_filepath = "{base}.{dst}.{format}".format(base=base, dst=args.dst_language, format=subtitle_format)
+                        dst_subtitle_filepath = f"{base}.{args.dst_language}.{subtitle_format}"
 
                         print(f"Extracting '{ffmpeg_dst_language_code}'subtitles stream as     : {dst_subtitle_filepath}")
 
                         writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
                         writer.write(dst_subtitle_filepath)
 
                     # ffmpeg_dst_language_code subtitles stream not exist, just print it
@@ -2729,15 +3146,15 @@
                             translated_subtitle_stream_transcripts = []
                             for i, translated_subtitle_stream_transcript in enumerate(pool.imap(transcript_translator, subtitle_stream_transcripts)):
                                 translated_subtitle_stream_transcripts.append(translated_subtitle_stream_transcript)
                                 pbar.update(i)
                             pbar.finish()
 
                             base, ext = os.path.splitext(media_filepath)
-                            src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=args.src_language, format=subtitle_format)
+                            src_subtitle_filepath = f"{base}.{args.src_language}.{subtitle_format}"
 
                             translation_writer = SubtitleWriter(subtitle_stream_regions, translated_subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
                             translation_writer.write(src_subtitle_filepath)
 
                             print("Translated subtitles file saved as      : {}" .format(src_subtitle_filepath))
 
                             # remove media_filepath from transcribe proceed_list because all needed srt files already saved
@@ -2932,15 +3349,15 @@
                 transcripts = []
                 for i, transcript in enumerate(pool.imap(recognizer, extracted_regions)):
                     transcripts.append(transcript)
                     pbar.update(i)
                 pbar.finish()
 
                 base, ext = os.path.splitext(media_filepath)
-                src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=args.src_language, format=subtitle_format)
+                src_subtitle_filepath = f"{base}.{args.src_language}.{subtitle_format}"
                 writer = SubtitleWriter(regions, transcripts, subtitle_format, error_messages_callback=show_error_messages)
                 writer.write(src_subtitle_filepath)
 
                 if do_translate == True:
                     # CONCURRENT TRANSLATION USING class SentenceTranslator(object)
                     # NO NEED TO TRANSLATE ALL transcript IN transcripts
                     # BECAUSE SOME region IN regions MAY JUST HAVE transcript WITH EMPTY STRING
@@ -3009,17 +3426,17 @@
                         base, ext = os.path.splitext(media_filepath)
                         src_tmp_embedded_media_filepath = "{base}.{src}.tmp.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
                         src_dst_tmp_embedded_media_filepath = "{base}.{src}.{dst}.tmp.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, dst=ffmpeg_dst_language_code, format=ext[1:])
                         embedded_media_filepath = "{base}.{src}.{dst}.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, dst=ffmpeg_dst_language_code, format=ext[1:])
 
                         '''
                         # USING FUNCTION
-                        src_tmp_output = embed_subtitle_to_media(media_filepath, media_type, src_subtitle_filepath, ffmpeg_src_language_code, src_tmp_embedded_media_filepath)
+                        src_tmp_output = embed_subtitle_into_media(media_filepath, media_type, src_subtitle_filepath, ffmpeg_src_language_code, src_tmp_embedded_media_filepath)
                         if os.path.isfile(src_tmp_output) and os.path.isfile(dst_subtitle_filepath):
-                            src_dst_tmp_output = embed_subtitle_to_media(src_tmp_embedded_media_filepath, media_type, dst_subtitle_filepath, ffmpeg_dst_language_code, src_dst_tmp_embedded_media_filepath)
+                            src_dst_tmp_output = embed_subtitle_into_media(src_tmp_embedded_media_filepath, media_type, dst_subtitle_filepath, ffmpeg_dst_language_code, src_dst_tmp_embedded_media_filepath)
                         '''
 
 
                         # USING CLASS
                         widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                         pbar = ProgressBar(widgets=widgets, maxval=100).start()
                         subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
```

### Comparing `autosrt-1.4.2/autosrt.egg-info/PKG-INFO` & `autosrt-1.4.3/autosrt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosrt
-Version: 1.4.2
+Version: 1.4.3
 Summary: a utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `autosrt-1.4.2/setup.py` & `autosrt-1.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.4.2/test/test1.py` & `autosrt-1.4.3/test/test1.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.4.2/test/test2.py` & `autosrt-1.4.3/test/test2.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.4.2/test/test3.py` & `autosrt-1.4.3/test/test3.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.4.2/test/test4.py` & `autosrt-1.4.3/test/test4.py`

 * *Files identical despite different names*

