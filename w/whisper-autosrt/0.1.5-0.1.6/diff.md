# Comparing `tmp/whisper_autosrt-0.1.5.tar.gz` & `tmp/whisper_autosrt-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper_autosrt-0.1.5.tar", last modified: Sat Jun 17 22:56:11 2023, max compression
+gzip compressed data, was "whisper_autosrt-0.1.6.tar", last modified: Tue Jun 20 09:59:16 2023, max compression
```

## Comparing `whisper_autosrt-0.1.5.tar` & `whisper_autosrt-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 22:56:11.221884 whisper_autosrt-0.1.5/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 whisper_autosrt-0.1.5/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 whisper_autosrt-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1956 2023-06-17 22:56:11.221884 whisper_autosrt-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     4700 2023-05-27 16:57:41.000000 whisper_autosrt-0.1.5/README.md
--rw-rw-rw-   0        0        0      147 2023-06-17 22:56:11.224878 whisper_autosrt-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1642 2023-06-02 17:36:46.000000 whisper_autosrt-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-17 22:56:11.178054 whisper_autosrt-0.1.5/whisper_autosrt/
--rw-rw-rw-   0        0        0   151532 2023-06-17 22:55:25.000000 whisper_autosrt-0.1.5/whisper_autosrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 22:56:11.219634 whisper_autosrt-0.1.5/whisper_autosrt.egg-info/
--rw-rw-rw-   0        0        0     1956 2023-06-17 22:56:10.000000 whisper_autosrt-0.1.5/whisper_autosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-06-17 22:56:11.000000 whisper_autosrt-0.1.5/whisper_autosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 22:56:10.000000 whisper_autosrt-0.1.5/whisper_autosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-06-17 22:56:10.000000 whisper_autosrt-0.1.5/whisper_autosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      119 2023-06-17 22:56:10.000000 whisper_autosrt-0.1.5/whisper_autosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-17 22:56:10.000000 whisper_autosrt-0.1.5/whisper_autosrt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 09:59:16.226019 whisper_autosrt-0.1.6/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 whisper_autosrt-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 whisper_autosrt-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2056 2023-06-20 09:59:16.226768 whisper_autosrt-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4700 2023-05-27 16:57:41.000000 whisper_autosrt-0.1.6/README.md
+-rw-rw-rw-   0        0        0      147 2023-06-20 09:59:16.229232 whisper_autosrt-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1749 2023-06-19 22:39:09.000000 whisper_autosrt-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 09:59:16.188559 whisper_autosrt-0.1.6/whisper_autosrt/
+-rw-rw-rw-   0        0        0   167742 2023-06-20 09:58:48.000000 whisper_autosrt-0.1.6/whisper_autosrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 09:59:16.224519 whisper_autosrt-0.1.6/whisper_autosrt.egg-info/
+-rw-rw-rw-   0        0        0     2056 2023-06-20 09:59:15.000000 whisper_autosrt-0.1.6/whisper_autosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-06-20 09:59:16.000000 whisper_autosrt-0.1.6/whisper_autosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 09:59:15.000000 whisper_autosrt-0.1.6/whisper_autosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-06-20 09:59:15.000000 whisper_autosrt-0.1.6/whisper_autosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      119 2023-06-20 09:59:15.000000 whisper_autosrt-0.1.6/whisper_autosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-20 09:59:15.000000 whisper_autosrt-0.1.6/whisper_autosrt.egg-info/top_level.txt
```

### Comparing `whisper_autosrt-0.1.5/LICENSE` & `whisper_autosrt-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper_autosrt-0.1.5/PKG-INFO` & `whisper_autosrt-0.1.6/whisper_autosrt.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: whisper_autosrt
-Version: 0.1.5
+Name: whisper-autosrt
+Version: 0.1.6
 Summary: a command line utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/whisper_autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
@@ -24,8 +24,8 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 
-whisper_autosrt is a command line utility for automatic speech recognition and subtitle generation. It takes video or audio files as input, generate transcriptions for them and optionally translates  them to a different language, and finally saves the resulting subtitles file to disk.               It supports a variety of input and output languages and can currently produce subtitles in SRT, VTT,JSON, and RAW format.
+whisper_autosrt is a command line utility for automatic speech recognition and subtitle generation  using faster_whisper module which is a reimplementation of OpenAI Whisper module. It takes video or audio files as input, generate transcriptions for them and optionally translates them to a differentlanguage, and finally saves the resulting subtitles file to disk.                                   It supports a variety of input and output languages and can currently produce subtitles in SRT, VTT,JSON, and RAW format.
```

### Comparing `whisper_autosrt-0.1.5/README.md` & `whisper_autosrt-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `whisper_autosrt-0.1.5/setup.py` & `whisper_autosrt-0.1.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 from whisper_autosrt import VERSION
 
 long_description = (
-    'whisper_autosrt is a command line utility for automatic speech recognition and subtitle generation. '
-    'It takes video or audio files as input, generate transcriptions for them and optionally translates  '
-    'them to a different language, and finally saves the resulting subtitles file to disk.               '
+    'whisper_autosrt is a command line utility for automatic speech recognition and subtitle generation  '
+    'using faster_whisper module which is a reimplementation of OpenAI Whisper module. It takes video or '
+    'audio files as input, generate transcriptions for them and optionally translates them to a different'
+    'language, and finally saves the resulting subtitles file to disk.                                   '
     'It supports a variety of input and output languages and can currently produce subtitles in SRT, VTT,'
     'JSON, and RAW format.'
 )
 
 install_requires=[
     "requests>=2.3.0",
     "httpx>=0.24.0",
```

### Comparing `whisper_autosrt-0.1.5/whisper_autosrt/__init__.py` & `whisper_autosrt-0.1.6/whisper_autosrt/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,17 +25,19 @@
 from pathlib import Path
 import warnings
 warnings.filterwarnings("ignore", message=".*The 'nopython' keyword.*")
 from faster_whisper import WhisperModel
 import ctypes
 import shutil
 
-VERSION = "0.1.5"
+
+VERSION = "0.1.6"
 #marker='█'
 
+
 class WhisperLanguage:
     def __init__(self):
         self.list_codes = []
         self.list_codes.append("auto")
         self.list_codes.append("af")
         self.list_codes.append("sq")
         self.list_codes.append("am")
@@ -1055,29 +1057,37 @@
 
 google_unsupported_languages = ["auto", "ba", "br", "fo", "nn", "oc", "tl", "bo"]
 
 
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
 
@@ -1091,71 +1101,73 @@
         temp = tempfile.NamedTemporaryFile(suffix='.wav', delete=False)
 
         if "\\" in media_filepath:
             media_filepath = media_filepath.replace("\\", "/")
 
         if not os.path.isfile(media_filepath):
             if self.error_messages_callback:
-                self.error_messages_callback(f"The given file does not exist: '{media_filepath}'")
+                self.error_messages_callback(f"The given file does not exist: {media_filepath}")
+            else:
+                print(f"The given file does not exist: {media_filepath}")
+                raise Exception(f"Invalid file: {media_filepath}")
+
+        if not self.ffprobe_check():
+            if self.error_messages_callback:
+                self.error_messages_callback("Cannot find ffprobe executable")
             else:
-                print(f"The given file does not exist: '{media_filepath}'")
-                raise Exception(f"Invalid file: '{media_filepath}'")
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
-                            "ffmpeg",
-                            "-y",
-                            "-i", media_filepath,
-                            "-ac", str(self.channels),
-                            "-ar", str(self.rate),
-                            "-loglevel", "error",
-                            "-hide_banner",
-                            "-progress", "-", "-nostats",
+                            'ffmpeg',
+                            '-hide_banner',
+                            '-loglevel', 'error',
+                            '-v', 'error',
+                            '-y',
+                            '-i', media_filepath,
+                            '-ac', str(self.channels),
+                            '-ar', str(self.rate),
+                            '-progress', '-', '-nostats',
                             temp.name
                          ]
 
-
         try:
-            info = f"Converting to a temporary WAV file"
-
-            # RUNNING ffmpeg WITHOUT SHOWING PROGRESSS
-            #use_shell = True if os.name == "nt" else False
-            #subprocess.check_output(command, stdin=open(os.devnull), shell=use_shell)
-
-
-            # RUNNING ffmpeg WITH SHOWING PROGRESSS
-            '''
-            # RUNNING ffmpeg WITH ffmpeg_progress_yield
-            ff = FfmpegProgress(command)
-            percentage = 0
-            for progress in ff.run_command_with_progress():
-                percentage = progress
-                if self.progress_callback:
-                    self.progress_callback(info, media_filepath, percentage)
-            temp.close()
-            '''
-
-            # RUNNING ffmpeg_command WITHOUT ffmpeg_progress_yield
-            ffprobe_command = f'ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 "{media_filepath}"'
+            media_file_display_name = os.path.basename(media_filepath).split('/')[-1]
+            info = f"Converting '{media_file_display_name}' to a temporary WAV file"
+            start_time = time.time()
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
+                              ]
 
+            ffprobe_process = None
             if sys.platform == "win32":
-                ffprobe_process = subprocess.Popen(ffprobe_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, creationflags=subprocess.CREATE_NO_WINDOW)
+                ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
             else:
-                ffprobe_process = subprocess.Popen(ffprobe_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
-
-            total_duration = float(ffprobe_process.stdout.read().decode('utf-8').strip())
+                ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True)
 
+            total_duration = float(ffprobe_process.strip())
 
+            process = None
             if sys.platform == "win32":
-                process = subprocess.Popen(ffmpeg_command, shell=True, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, creationflags=subprocess.CREATE_NO_WINDOW)
+                process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
             else:
                 process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
 
             while True:
                 if process.stdout is None:
                     continue
 
@@ -1167,15 +1179,15 @@
                 if "out_time=" in stderr_line:
                     time_str = stderr_line.split('time=')[1].split()[0]
                     current_duration = sum(float(x) * 1000 * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
 
                     if current_duration>0:
                         percentage = int(current_duration*100/(int(float(total_duration))*1000))
                         if self.progress_callback:
-                            self.progress_callback(info, media_filepath, percentage)
+                            self.progress_callback(info, media_file_display_name, percentage, start_time)
 
             temp.close()
 
             return temp.name, self.rate
 
         except KeyboardInterrupt:
             if self.error_messages_callback:
@@ -1372,15 +1384,15 @@
         try:
             formatter = SubtitleFormatter(self.format)
             formatted_subtitles = formatter(self.timed_subtitles)
             saved_subtitle_filepath = declared_subtitle_filepath
             if saved_subtitle_filepath:
                 subtitle_file_base, subtitle_file_ext = os.path.splitext(saved_subtitle_filepath)
                 if not subtitle_file_ext:
-                    saved_subtitle_filepath = "{base}.{format}".format(base=subtitle_file_base, format=self.format)
+                    saved_subtitle_filepath = f"{subtitle_file_base}.{self.format}"
                 else:
                     saved_subtitle_filepath = declared_subtitle_filepath
             with open(saved_subtitle_filepath, 'wb') as f:
                 f.write(formatted_subtitles.encode("utf-8"))
             #with open(saved_subtitle_filepath, 'a') as f:
             #    f.write("\n")
 
@@ -1396,58 +1408,66 @@
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
 
@@ -1477,26 +1497,34 @@
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
             subtitles = None
@@ -1565,14 +1593,48 @@
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
@@ -1591,16 +1653,25 @@
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
@@ -1613,61 +1684,73 @@
 
         if not os.path.isfile(media_filepath):
             if self.error_messages_callback:
                 self.error_messages_callback(f"The given file does not exist: {media_filepath}")
             else:
                 print(f"The given file does not exist: {media_filepath}")
                 raise Exception(f"Invalid file: {media_filepath}")
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
-                self.error_messages_callback("Cannot find ffmpeg executable on this machine")
+                self.error_messages_callback("Cannot find ffmpeg executable")
             else:
-                print("Cannot find ffmpeg executable on this machine")
+                print("Cannot find ffmpeg executable")
                 raise Exception("Dependency not found: ffmpeg")
 
         try:
-            scale_switch = "'trunc(iw/2)*2':'trunc(ih/2)*2'"
+            scale_switch = "'trunc(iw/2)*2'\:'trunc(ih/2)*2'"
             ffmpeg_command = [
-                                "ffmpeg",
-                                "-y",
-                                "-i", media_filepath,
-                                "-vf", f"subtitles={shlex.quote(self.subtitle_path)},scale={scale_switch}",
-                                "-c:v", "libx264",
-                                "-crf", "23",
-                                "-preset", "medium",
-                                "-c:a", "copy",
-                                "-progress", "-", "-nostats",
+                                'ffmpeg',
+                                '-hide_banner',
+                                '-loglevel', 'error',
+                                '-v', 'error',
+                                '-y',
+                                '-i', media_filepath,
+                                '-vf', f'subtitles={shlex.quote(self.subtitle_path)},scale={scale_switch}',
+                                '-c:v', 'libx264',
+                                '-crf', '23',
+                                '-preset', 'medium',
+                                '-c:a', 'copy',
+                                '-progress', '-', '-nostats',
                                 self.output_path
                              ]
 
-            info = f"Rendering subtitles file into {media_type} file : "
-
-            '''
-            # RUNNING ffmpeg_command USING ffmpeg_progress_yield MODULE
-            ff = FfmpegProgress(ffmpeg_command)
-            percentage = 0
-            for progress in ff.run_command_with_progress():
-                percentage = progress
-                if self.progress_callback:
-                    self.progress_callback(info, media_filepath, percentage)
-            '''
-
-            # RUNNING ffmpeg_command WITHOUT ffmpeg_progress_yield MODULE
-            ffprobe_command = f'ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 "{media_filepath}"'
+            media_file_display_name = os.path.basename(media_filepath).split('/')[-1]
+            info = f"Rendering subtitles file into '{media_file_display_name}'"
+            start_time = time.time()
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
+                              ]
 
+            ffprobe_process = None
             if sys.platform == "win32":
-                ffprobe_process = subprocess.Popen(ffprobe_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, creationflags=subprocess.CREATE_NO_WINDOW)
+                ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
             else:
-                ffprobe_process = subprocess.Popen(ffprobe_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
-
-            total_duration = float(ffprobe_process.stdout.read().decode('utf-8').strip())
+                ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True)
 
+            total_duration = float(ffprobe_process.strip())
 
+            process = None
             if sys.platform == "win32":
-                process = subprocess.Popen(ffmpeg_command, shell=True, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, creationflags=subprocess.CREATE_NO_WINDOW)
+                process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
             else:
                 process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
 
             while True:
                 if process.stdout is None:
                     continue
 
@@ -1679,15 +1762,15 @@
                 if "out_time=" in stderr_line:
                     time_str = stderr_line.split('time=')[1].split()[0]
                     current_duration = sum(float(x) * 1000 * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
 
                     if current_duration>0:
                         percentage = int(current_duration*100/(int(float(total_duration))*1000))
                         if self.progress_callback:
-                            self.progress_callback(info, media_filepath, percentage)
+                            self.progress_callback(info, media_file_display_name, percentage, start_time)
 
             if os.path.isfile(self.output_path):
                 return self.output_path
             else:
                 return None
 
         except KeyboardInterrupt:
@@ -1704,69 +1787,80 @@
                 print(e)
             return
 
 
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
 
-        # Find the subtitles stream with language metadata
+        # Find the subtitle stream with language metadata
         subtitle_languages = []
         for stream in streams:
-            if stream['codec_type'] == 'subtitles' and 'tags' in stream and 'language' in stream['tags']:
+            if stream['codec_type'] == 'subtitle' and 'tags' in stream and 'language' in stream['tags']:
                 language = stream['tags']['language']
                 subtitle_languages.append(language)
 
         return subtitle_languages
 
     def __call__(self, media_filepath):
         if "\\" in media_filepath:
@@ -1780,77 +1874,90 @@
 
         if not os.path.isfile(media_filepath):
             if self.error_messages_callback:
                 self.error_messages_callback(f"The given file does not exist: {media_filepath}")
             else:
                 print(f"The given file does not exist: {media_filepath}")
                 raise Exception(f"Invalid file: {media_filepath}")
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
-                self.error_messages_callback("Cannot find ffmpeg executable on this machine")
+                self.error_messages_callback("Cannot find ffmpeg executable")
             else:
-                print("Cannot find ffmpeg executable on this machine")
+                print("Cannot find ffmpeg executable")
                 raise Exception("Dependency not found: ffmpeg")
 
         try:
             existing_languages = self.get_existing_subtitle_language(media_filepath)
             if self.language in existing_languages:
                 # THIS 'print' THINGS WILL MAKE progresbar screwed up!
-                #msg = (f"'{self.language}' subtitles stream already existed in {media_filepath}")
+                #msg = (f"'{self.language}' subtitle stream already existed in {media_filepath}")
                 #if self.error_messages_callback:
                 #    self.error_messages_callback(msg)
                 #else:
                 #    print(msg)
                 return
 
             else:
-                # Determine the next available subtitles index
+                # Determine the next available subtitle index
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
                                     '-progress', '-', '-nostats',
                                     self.output_path
                                  ]
 
-                info = f"Embedding subtitles file into {media_filepath}"
-
-                '''
-                # USING ffmpeg_progress_yield MODULE
-                ff = FfmpegProgress(ffmpeg_command)
-                percentage = 0
-                for progress in ff.run_command_with_progress():
-                    percentage = progress
-                    if self.progress_callback:
-                        self.progress_callback(info, media_filepath, percentage)
-                '''
-
-                # RUNNING ffmpeg_command WITHOUT ffmpeg_progress_yield MODULE
-                ffprobe_command = f'ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 "{media_filepath}"'
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
 
+                ffprobe_process = None
                 if sys.platform == "win32":
-                    ffprobe_process = subprocess.Popen(ffprobe_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, creationflags=subprocess.CREATE_NO_WINDOW)
+                    ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
                 else:
-                    ffprobe_process = subprocess.Popen(ffprobe_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
-
-                total_duration = float(ffprobe_process.stdout.read().decode('utf-8').strip())
+                    ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True)
 
+                total_duration = float(ffprobe_process.strip())
 
+                process = None
                 if sys.platform == "win32":
-                    process = subprocess.Popen(ffmpeg_command, shell=True, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, creationflags=subprocess.CREATE_NO_WINDOW)
+                    process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
                 else:
                     process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
 
                 while True:
                     if process.stdout is None:
                         continue
 
@@ -1862,15 +1969,15 @@
                     if "out_time=" in stderr_line:
                         time_str = stderr_line.split('time=')[1].split()[0]
                         current_duration = sum(float(x) * 1000 * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
 
                         if current_duration>0:
                             percentage = int(current_duration*100/(int(float(total_duration))*1000))
                             if self.progress_callback:
-                                self.progress_callback(info, media_filepath, percentage)
+                                self.progress_callback(info, media_file_display_name, percentage, start_time)
 
                 if os.path.isfile(self.output_path):
                     return self.output_path
                 else:
                     return None
 
                 if os.path.isfile(self.output_path):
@@ -1892,29 +1999,37 @@
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
 
@@ -1932,56 +2047,69 @@
 
         if not os.path.isfile(media_filepath):
             if self.error_messages_callback:
                 self.error_messages_callback(f"The given file does not exist: {media_filepath}")
             else:
                 print(f"The given file does not exist: {media_filepath}")
                 raise Exception(f"Invalid file: {media_filepath}")
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
-                self.error_messages_callback("Cannot find ffmpeg executable on this machine")
+                self.error_messages_callback("Cannot find ffmpeg executable")
             else:
-                print("Cannot find ffmpeg executable on this machine")
+                print("Cannot find ffmpeg executable")
                 raise Exception("Dependency not found: ffmpeg")
 
         try:
             ffmpeg_command = [
                                 'ffmpeg',
+                                '-hide_banner',
+                                '-loglevel', 'error',
+                                '-v', 'error',
                                 '-y',
                                 '-i', media_filepath,
                                 '-c', 'copy',
                                 '-sn',
-                                "-progress", "-", "-nostats",
+                                '-progress', '-', '-nostats',
                                 self.output_path
                              ]
 
-            info = "Removing subtitles streams from file"
-
-            '''
-            # USING ffmpeg_progress_yield MODULE
-            ff = FfmpegProgress(ffmpeg_command)
-            percentage = 0
-            for progress in ff.run_command_with_progress():
-                percentage = progress
-                if self.progress_callback:
-                    self.progress_callback(info, media_filepath, percentage)
-            '''
-
-            # RUNNING ffmpeg_command WITHOUT ffmpeg_progress_yield MODULE
-            ffprobe_command = f'ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 "{media_filepath}"'
+            media_file_display_name = os.path.basename(media_filepath).split('/')[-1]
+            info = f"Removing subtitles streams from '{media_file_display_name}'"
+            start_time = time.time()
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
+                              ]
 
+            ffprobe_process = None
             if sys.platform == "win32":
-                ffprobe_process = subprocess.Popen(ffprobe_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, creationflags=subprocess.CREATE_NO_WINDOW)
+                ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
             else:
-                ffprobe_process = subprocess.Popen(ffprobe_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+                ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True)
 
-            total_duration = float(ffprobe_process.stdout.read().decode('utf-8').strip())
+            total_duration = float(ffprobe_process.strip())
 
+            process = None
             if sys.platform == "win32":
-                process = subprocess.Popen(ffmpeg_command, shell=True, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, creationflags=subprocess.CREATE_NO_WINDOW)
+                process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
             else:
                 process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
 
             while True:
                 if process.stdout is None:
                     continue
 
@@ -1993,15 +2121,15 @@
                 if "out_time=" in stderr_line:
                     time_str = stderr_line.split('time=')[1].split()[0]
                     current_duration = sum(float(x) * 1000 * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
 
                     if current_duration>0:
                         percentage = int(current_duration*100/(int(float(total_duration))*1000))
                         if self.progress_callback:
-                            self.progress_callback(info, media_filepath, percentage)
+                            self.progress_callback(info, media_file_display_name, percentage, start_time)
 
             if os.path.isfile(self.output_path):
                 return self.output_path
             else:
                 return None
 
             if os.path.isfile(self.output_path):
@@ -2165,162 +2293,341 @@
         if error_messages_callback:
             error_messages_callback(e)
         else:
             print(e)
         return
 
 
-def check_file_type(file_path, error_messages_callback=None):
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
             print(e)
 
     return None
 
 
-def get_duration(filename, error_messages_callback=None):
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
-        command = f'ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 "{filename}"'
-        result = subprocess.run(command, capture_output=True, text=True, shell=True)
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
 
-        if result.returncode == 0:
-            duration = float(result.stdout)
-            return duration
-        else:
-            msg = f"Failed to get duration for {filename}."
-            if error_messages_callback:
-                error_messages_callback(msg)
-            return None
+        output = None
+        if sys.platform == "win32":
+            output = subprocess.run(command, stdin=open(os.devnull), stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
+        else:
+            output = subprocess.run(command, stdin=open(os.devnull), stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True)
+
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
-        return
+        return None
 
 
-def get_existing_subtitle_language(media_path):
-    # Run ffprobe to get stream information
-    command = [
-                'ffprobe',
-                '-v', 'quiet',
-                '-of', 'json',
-                '-show_entries',
-                'format:stream',
-                media_path
-    ]
-
-    output = subprocess.run(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True, universal_newlines=True)
-    metadata = json.loads(output.stdout)
-    streams = metadata['streams']
-
-    # Find the subtitles stream with language metadata
-    subtitle_languages = []
-    for stream in streams:
-        if stream['codec_type'] == 'subtitles' and 'tags' in stream and 'language' in stream['tags']:
-            language = stream['tags']['language']
-            subtitle_languages.append(language)
+def render_subtitle_to_media(media_filepath, media_type, media_ext, subtitle_path, output_path, error_messages_callback=None):
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
 
-    return subtitle_languages
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
 
-def render_subtitle_to_media(media_filepath, media_type, media_ext, subtitle_path, output_path, error_messages_callback=None):
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
+    if not ffmpeg_check():
+        if error_messages_callback:
+            error_messages_callback("Cannot find ffmpeg executable")
+        else:
+            print("Cannot find ffmpeg executable")
+            raise Exception("Dependency not found: ffmpeg")
 
     try:
         if "\\" in media_filepath:
             media_filepath = media_filepath.replace("\\", "/")
 
         if "\\" in subtitle_path:
             subtitle_path = subtitle_path.replace("\\", "/")
 
         if "\\" in output_path:
             output_path = output_path.replace("\\", "/")
 
-        ffprobe_command = f'ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 "{media_filepath}"'
-        ffprobe_process = subprocess.Popen(ffprobe_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
-        total_duration = float(ffprobe_process.stdout.read().decode().strip())
-
-        #ffmpeg_command = f'ffmpeg -y -i "{media_filepath}" -vf "subtitles={shlex.quote(subtitle_path)}" "{output_path}"'
-
-        '''
-        ffmpeg_command = [
-                            "ffmpeg",
-                            "-y",
-                            "-i", media_filepath,
-                            "-vf", f"subtitles={shlex.quote(self.subtitle_path)}",
-                            "-y", self.output_path
-                         ]
-        '''
-
         scale_switch = "'trunc(iw/2)*2':'trunc(ih/2)*2'"
         ffmpeg_command = [
-                            "ffmpeg",
-                            "-y",
-                            "-i", media_filepath,
-                            "-vf", f"subtitles={shlex.quote(self.subtitle_path)},scale={scale_switch}",
-                            "-c:v", "libx264",
-                            "-crf", "23",
-                            "-preset", "medium",
-                            "-c:a", "copy",
+                            'ffmpeg',
+                            '-y',
+                            '-i', media_filepath,
+                            '-vf', f'subtitles={shlex.quote(self.subtitle_path)},scale={scale_switch}',
+                            '-c:v', 'libx264',
+                            '-crf', '23',
+                            '-preset', 'medium',
+                            '-c:a', 'copy',
                             self.output_path
                          ]
 
-        widgets = [f"Rendering subtitles into {media_type} : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+        ffprobe_command = [
+                            'ffprobe',
+                            '-hide_banner',
+                            '-v', 'error',
+                            '-loglevel', 'error',
+                            '-show_entries',
+                            'format=duration',
+                            '-of', 'default=noprint_wrappers=1:nokey=1',
+                            media_filepath
+                          ]
+
+        ffprobe_process = None
+        if sys.platform == "win32":
+            ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
+        else:
+            ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True)
+
+        total_duration = float(ffprobe_process.strip())
+
+        widgets = [f"Rendering '{language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
         pbar = ProgressBar(widgets=widgets, maxval=100).start()
         percentage = 0
 
+        process = None
         if sys.platform == "win32":
-            process = subprocess.Popen(ffmpeg_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
+            process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
         else:
-            process = subprocess.Popen(ffmpeg_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
+            process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+
+        while True:
+            if process.stdout is None:
+                continue
+
+            stderr_line = (process.stdout.readline().decode("utf-8", errors="replace").strip())
+ 
+            if stderr_line == '' and process.poll() is not None:
+                break
 
-        for line in process.stdout:
-            if "time=" in line:
-                #print(line)
-                time_str = line.split("time=")[1].split()[0]
-                #print(f"time_str = {time_str})
-                current_duration = sum(float(x) * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
-                #print(f"current_duration = {current_duration}")
+            if "out_time=" in stderr_line:
+                time_str = stderr_line.split('time=')[1].split()[0]
+                current_duration = sum(float(x) * 1000 * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
                 if current_duration>0:
-                    percentage = int(current_duration*100/total_duration)
-                    #print(f"percentage = {percentage}%")
+                    percentage = int(current_duration*100/(int(float(total_duration))*1000))
                     pbar.update(percentage)
         pbar.finish()
         return output_path
 
     except Exception as e:
         if error_messages_callback:
             error_messages_callback(e)
         else:
             print(e)
-        return
+        return None
 
 
 def embed_subtitle_to_media(media_filepath, media_type, subtitle_path, language_code, output_path, error_messages_callback=None):
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
 
         if "\\" in subtitle_path:
             subtitle_path = subtitle_path.replace("\\", "/")
 
@@ -2332,70 +2639,213 @@
             #print(f"'{language_code}' subtitles stream already existed in {media_filepath}")
             return
 
         else:
             # Determine the next available subtitles index
             next_index = len(existing_languages)
 
-            ffprobe_command = f'ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 "{media_filepath}"'
-            if sys.platform == "win32":
-                ffprobe_process = subprocess.Popen(ffprobe_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
-            else:
-                ffprobe_process = subprocess.Popen(ffprobe_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
-
-            total_duration = float(ffprobe_process.stdout.read().decode('utf-8').strip())
-
             ffmpeg_command = [
                                 'ffmpeg',
+                                '-hide_banner',
+                                '-loglevel', 'error',
+                                '-v', 'error',
                                 '-y',
                                 '-i', media_filepath,
                                 '-sub_charenc', 'UTF-8',
                                 '-i', subtitle_path,
                                 '-c:v', 'copy',
                                 '-c:a', 'copy',
                                 '-scodec', 'mov_text',
                                 '-metadata:s:s:' + str(next_index), f'language={shlex.quote(language_code)}',
                                 '-map', '0',
                                 '-map', '1',
                                 output_path
                              ]
 
-            widgets = [f"Embeding \'{language_code}\' subtitles into {media_type}  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
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
             pbar = ProgressBar(widgets=widgets, maxval=100).start()
             percentage = 0
 
+            process = None
             if sys.platform == "win32":
-                process = subprocess.Popen(ffmpeg_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
+                process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
             else:
-                process = subprocess.Popen(ffmpeg_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
+                process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
 
-            for line in process.stdout:
-                if "time=" in line:
-                    #print(line)
-                    time_str = line.split("time=")[1].split()[0]
-                    #print(f"time_str = {time_str}")
-                    current_duration = sum(float(x) * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
-                    #print(f"current_duration = {current_duration}")
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
                     if current_duration>0:
-                        percentage = int(current_duration*100/total_duration)
-                        #print(f"percentage = {percentage}%")
+                        percentage = int(current_duration*100/(int(float(total_duration))*1000))
                         pbar.update(percentage)
             pbar.finish()
+
             return output_path
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
+def remove_subtitles_from_media(media_filepath, output_path, progress_callback=None, error_messages_callback=None):
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
+    try:
+        if "\\" in media_filepath:
+            media_filepath = media_filepath.replace("\\", "/")
+
+        if "\\" in output_path:
+            output_path = output_path.replace("\\", "/")
+
+        ffmpeg_command = [
+                            'ffmpeg',
+                            '-hide_banner',
+                            '-loglevel', 'error',
+                            '-v', 'error',
+                            '-y',
+                            '-i', media_filepath,
+                            '-c', 'copy',
+                            '-sn',
+                            '-progress', '-', '-nostats',
+                            self.output_path
+                         ]
+
+        ffprobe_command = [
+                            'ffprobe',
+                            '-hide_banner',
+                            '-v', 'error',
+                            '-loglevel', 'error',
+                            '-show_entries',
+                            'format=duration',
+                            '-of', 'default=noprint_wrappers=1:nokey=1',
+                            media_filepath
+                          ]
+
+        ffprobe_process = None
+        if sys.platform == "win32":
+            ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
+        else:
+            ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True)
+
+        total_duration = float(ffprobe_process.strip())
+
+        widgets = ["Removing subtitles streams from file    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+        pbar = ProgressBar(widgets=widgets, maxval=100).start()
+        percentage = 0
+
+        process = None
+        if sys.platform == "win32":
+            process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
+        else:
+            process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+
+        while True:
+            if process.stdout is None:
+                continue
+
+            stderr_line = (process.stdout.readline().decode("utf-8", errors="replace").strip())
+ 
+            if stderr_line == '' and process.poll() is not None:
+                break
+
+            if "out_time=" in stderr_line:
+                time_str = stderr_line.split('time=')[1].split()[0]
+                current_duration = sum(float(x) * 1000 * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
+                if current_duration>0:
+                    percentage = int(current_duration*100/(int(float(total_duration))*1000))
+                    pbar.update(percentage)
+        pbar.finish()
+
+        return output_path
+
+    except KeyboardInterrupt:
+        if error_messages_callback:
+            error_messages_callback("Cancelling all tasks")
+        else:
+            print("Cancelling all tasks")
         return
 
     except Exception as e:
         if error_messages_callback:
             error_messages_callback(e)
         else:
             print(e)
         return None
 
 
-def show_progress(info, media_filepath, progress):
+def show_progress(info, media_file_display_name, progress, start_time):
     global pbar
     pbar.update(progress)
 
 
 def show_error_messages(messages):
     print(messages)
 
@@ -2684,15 +3134,15 @@
                             subtitle_stream_regions = []
                             subtitle_stream_transcripts = []
                             for entry in src_subtitle_stream_timed_subtitles:
                                 subtitle_stream_regions.append(entry[0])
                                 subtitle_stream_transcripts.append(entry[1])
 
                             base, ext = os.path.splitext(media_filepath)
-                            src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=src_language, format=subtitle_format)
+                            src_subtitle_filepath = f"{base}.{src_language}.{subtitle_format}"
 
                             print(f"Extracting '{ffmpeg_src_language_code}' subtitles stream as       : '{src_subtitle_filepath}'")
 
                             writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
                             writer.write(src_subtitle_filepath)
 
                             if args.force_recognize == False:
@@ -2798,15 +3248,15 @@
                             subtitle_stream_regions = []
                             subtitle_stream_transcripts = []
                             for entry in src_subtitle_stream_timed_subtitles:
                                 subtitle_stream_regions.append(entry[0])
                                 subtitle_stream_transcripts.append(entry[1])
 
                             base, ext = os.path.splitext(media_filepath)
-                            src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=src_language, format=subtitle_format)
+                            src_subtitle_filepath = f"{base}.{src_language}.{subtitle_format}"
 
                             print(f"Extracting '{ffmpeg_src_language_code}' subtitles stream as       : '{src_subtitle_filepath}'")
 
                             writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
                             writer.write(src_subtitle_filepath)
 
                         # ffmpeg_src_language_code subtitles stream not exist, just print it
@@ -2818,15 +3268,15 @@
                             print("Is '%s' subtitles stream exist            : Yes" %(ffmpeg_dst_language_code.center(3)))
                             subtitle_stream_regions = []
                             subtitle_stream_transcripts = []
                             for entry in dst_subtitle_stream_timed_subtitles:
                                 subtitle_stream_regions.append(entry[0])
                                 subtitle_stream_transcripts.append(entry[1])
                             base, ext = os.path.splitext(media_filepath)
-                            dst_subtitle_filepath = "{base}.{dst}.{format}".format(base=base, dst=dst_language, format=subtitle_format)
+                            dst_subtitle_filepath = f"{base}.{dst_language}.{subtitle_format}"
                             writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
                             print(f"Extracting '{ffmpeg_dst_language_code}' subtitles stream as       : '{dst_subtitle_filepath}'")
                             writer.write(dst_subtitle_filepath)
 
                         # ffmpeg_dst_language_code subtitles stream not exist, just print it
                         else:
                             print("Is '%s' subtitles stream exist            : No" %(ffmpeg_dst_language_code.center(3)))
@@ -2846,30 +3296,30 @@
                                 translated_subtitle_stream_transcripts = []
                                 for i, translated_subtitle_stream_transcript in enumerate(pool.imap(transcript_translator, subtitle_stream_transcripts)):
                                     translated_subtitle_stream_transcripts.append(translated_subtitle_stream_transcript)
                                     pbar.update(i)
                                 pbar.finish()
 
                                 base, ext = os.path.splitext(media_filepath)
-                                src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=src_language, format=subtitle_format)
+                                src_subtitle_filepath = f"{base}.{src_language}.{subtitle_format}"
 
                                 translation_writer = SubtitleWriter(subtitle_stream_regions, translated_subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
                                 translation_writer.write(src_subtitle_filepath)
 
                                 print(f"Translated subtitles file saved as         : '{src_subtitle_filepath}'")
 
                                 if args.force_recognize == False:
                                     removed_media_filepaths.append(media_filepath)
 
                                 if args.embed_src and dst_subtitle_stream_timed_subtitles and dst_subtitle_stream_timed_subtitles != []:
                                     ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
 
                                     base, ext = os.path.splitext(media_filepath)
-                                    src_tmp_embedded_media_filepath = "{base}.{src}.tmp.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
-                                    embedded_media_filepath = "{base}.{src}.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
+                                    src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{ext[1:]}"
+                                    embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.embedded.{ext[1:]}"
 
                                     widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type} file  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                                     pbar = ProgressBar(widgets=widgets, maxval=100).start()
                                     subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
                                     src_tmp_output = subtitle_embedder(media_filepath)
                                     pbar.finish()
 
@@ -2899,30 +3349,30 @@
                                 translated_subtitle_stream_transcripts = []
                                 for i, translated_subtitle_stream_transcript in enumerate(pool.imap(transcript_translator, subtitle_stream_transcripts)):
                                     translated_subtitle_stream_transcripts.append(translated_subtitle_stream_transcript)
                                     pbar.update(i)
                                 pbar.finish()
 
                                 base, ext = os.path.splitext(media_filepath)
-                                dst_subtitle_filepath = "{base}.{dst}.{format}".format(base=base, dst=dst_language, format=subtitle_format)
+                                dst_subtitle_filepath = f"{base}.{dst_language}.{subtitle_format}"
 
                                 translation_writer = SubtitleWriter(subtitle_stream_regions, translated_subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
                                 translation_writer.write(dst_subtitle_filepath)
 
                                 print(f"Translated subtitles file saved as         : '{dst_subtitle_filepath}'")
 
                                 if args.force_recognize == False:
                                     removed_media_filepaths.append(media_filepath)
 
                                 if args.embed_dst == True and src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
                                     ffmpeg_dst_language_code = google_language.ffmpeg_code_of_code[dst_language]
 
                                     base, ext = os.path.splitext(media_filepath)
-                                    dst_tmp_embedded_media_filepath = "{base}.{dst}.tmp.embedded.{format}".format(base=base, dst=ffmpeg_dst_language_code, format=ext[1:])
-                                    embedded_media_filepath = "{base}.{dst}.embedded.{format}".format(base=base, dst=ffmpeg_dst_language_code, format=ext[1:])
+                                    dst_tmp_embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.tmp.embedded.{ext[1:]}"
+                                    embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.embedded.{ext[1:]}"
 
                                     widgets = [f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_type} file  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                                     pbar = ProgressBar(widgets=widgets, maxval=100).start()
                                     subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=dst_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
                                     dst_tmp_output = subtitle_embedder(media_filepath)
                                     pbar.finish()
 
@@ -2976,16 +3426,16 @@
     print("=========================================================================================================")
 
     proceed_list = []
     # if args.force_recognize is true then we need to remove subtitles streams and save it as new media file to proceed with transcribe
     if args.force_recognize == True:
         for media_filepath in media_filepaths:
             base, ext = os.path.splitext(media_filepath)
-            tmp_subtitle_removed_media_filepath = "{base}.tmp.subtitles.removed.media_filepath.{format}".format(base=base, format=ext[1:])
-            subtitle_removed_media_filepath = "{base}.force.recognize.{format}".format(base=base, format=ext[1:])
+            tmp_subtitle_removed_media_filepath = f"{base}.tmp.subtitles.removed.media_filepath.{ext[1:]}"
+            subtitle_removed_media_filepath = f"{base}.force.recognize.{ext[1:]}"
 
             #src_tmp_output = remove_subtitles_from_media(media_filepath, tmp_subtitle_removed_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
 
             widgets = [f"Removing subtitles streams from {media_type} file : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
             pbar = ProgressBar(widgets=widgets, maxval=100).start()
             subtitle_remover = MediaSubtitleRemover(output_path=tmp_subtitle_removed_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
             tmp_output = subtitle_remover(media_filepath)
@@ -3042,15 +3492,15 @@
                 regions.append((segment.start, segment.end))
                 transcripts.append(segment.text)
                 pbar.update(progress)
             pbar.finish()
             timed_subtitles = [(r, t) for r, t in zip(regions, transcripts) if t]
 
             base, ext = os.path.splitext(media_filepath)
-            src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=src_language, format=subtitle_format)
+            src_subtitle_filepath = f"{base}.{src_language}.{subtitle_format}"
 
             writer = SubtitleWriter(regions, transcripts, subtitle_format, error_messages_callback=show_error_messages)
             writer.write(src_subtitle_filepath)
 
             if do_translate:
                 timed_subtitles = writer.timed_subtitles
                 created_regions = []
@@ -3068,15 +3518,15 @@
                 translated_subtitles = []
                 for i, translated_subtitle in enumerate(pool.imap(transcript_translator, created_subtitles)):
                     translated_subtitles.append(translated_subtitle)
                     pbar.update(i)
                 pbar.finish()
 
                 base, ext = os.path.splitext(media_filepath)
-                dst_subtitle_filepath = "{base}.{dst}.{format}".format(base=base, dst=args.dst_language, format=subtitle_format)
+                dst_subtitle_filepath = f"{base}.{dst_language}.{subtitle_format}"
 
                 translation_writer = SubtitleWriter(created_regions, translated_subtitles, subtitle_format, error_messages_callback=show_error_messages)
                 translation_writer.write(dst_subtitle_filepath)
 
             if do_translate:
                 print(f"Original subtitles file saved as           : '{src_subtitle_filepath}'")
                 print(f"Translated subtitles file saved as         : '{dst_subtitle_filepath}'")
@@ -3091,16 +3541,16 @@
             if do_translate == False:
 
                 if args.embed_src == True:
 
                     ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
 
                     base, ext = os.path.splitext(media_filepath)
-                    src_tmp_embedded_media_filepath = "{base}.{src}.tmp.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
-                    embedded_media_filepath = "{base}.{src}.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
+                    src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{ext[1:]}"
+                    embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.embedded.{ext[1:]}"
 
                     widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type} file  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                     pbar = ProgressBar(widgets=widgets, maxval=100).start()
                     subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
                     src_tmp_output = subtitle_embedder(media_filepath)
                     pbar.finish()
 
@@ -3111,52 +3561,55 @@
 
             elif do_translate == True:
 
                 if args.embed_src == True and args.embed_dst == True:
 
                     ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
                     ffmpeg_dst_language_code = google_language.ffmpeg_code_of_code[dst_language]
+                    print(f"ffmpeg_src_language_code = {ffmpeg_src_language_code}")
+                    print(f"ffmpeg_dst_language_code = {ffmpeg_dst_language_code}")
 
                     base, ext = os.path.splitext(media_filepath)
-                    src_tmp_embedded_media_filepath = "{base}.{src}.tmp.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
-                    src_dst_tmp_embedded_media_filepath = "{base}.{src}.{dst}.tmp.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, dst=ffmpeg_dst_language_code, format=ext[1:])
-                    embedded_media_filepath = "{base}.{src}.{dst}.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, dst=ffmpeg_dst_language_code, format=ext[1:])
+                    src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{ext[1:]}"
+                    src_dst_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.{ffmpeg_dst_language_code}.tmp.embedded.{ext[1:]}"
+                    embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.{ffmpeg_dst_language_code}.embedded.{ext[1:]}"
 
                     widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type} file  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                     pbar = ProgressBar(widgets=widgets, maxval=100).start()
                     subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
                     src_tmp_output = subtitle_embedder(media_filepath)
                     pbar.finish()
 
                     if os.path.isfile(src_tmp_output) and os.path.isfile(dst_subtitle_filepath):
                         widgets = [f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_type} file  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                         pbar = ProgressBar(widgets=widgets, maxval=100).start()
                         subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=src_dst_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                        src_dst_tmp_output = subtitle_embedder(src_tmp_embedded_media_filepath)
+                        src_dst_tmp_output = subtitle_embedder(src_tmp_output)
                         pbar.finish()
-                    else:
-                        print("Unknown error!")
 
                     if os.path.isfile(src_dst_tmp_output):
                         shutil.copy(src_dst_tmp_output, embedded_media_filepath)
                         print(f"Subtitles embedded {media_type} file saved as     : '{embedded_media_filepath}'")
+                    else:
+                        print("Unknown error!")
 
                     if os.path.isfile(src_dst_tmp_output):
                         os.remove(src_dst_tmp_output)
 
                     if os.path.isfile(src_tmp_output):
                         os.remove(src_tmp_output)
 
+
                 elif args.embed_src == True and args.embed_dst == False:
 
                     ffmpeg_src_language_code = google_language.ffmpeg_code_of_code[src_language]
 
                     base, ext = os.path.splitext(media_filepath)
-                    src_tmp_embedded_media_filepath = "{base}.{src}.tmp.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
-                    embedded_media_filepath = "{base}.{src}.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
+                    src_tmp_embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.tmp.embedded.{ext[1:]}"
+                    embedded_media_filepath = f"{base}.{ffmpeg_src_language_code}.embedded.{ext[1:]}"
 
                     widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type} file  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                     pbar = ProgressBar(widgets=widgets, maxval=100).start()
                     subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
                     src_tmp_output = subtitle_embedder(media_filepath)
                     pbar.finish()
 
@@ -3168,16 +3621,16 @@
                         print("Unknown error!")
 
                 elif args.embed_src == False and args.embed_dst == True:
 
                     ffmpeg_dst_language_code = google_language.ffmpeg_code_of_code[dst_language]
 
                     base, ext = os.path.splitext(media_filepath)
-                    dst_tmp_embedded_media_filepath = "{base}.{dst}.tmp.embedded.{format}".format(base=base, dst=ffmpeg_dst_language_code, format=ext[1:])
-                    embedded_media_filepath = "{base}.{dst}.embedded.{format}".format(base=base, dst=ffmpeg_dst_language_code, format=ext[1:])
+                    dst_tmp_embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.tmp.embedded.{ext[1:]}"
+                    embedded_media_filepath = f"{base}.{ffmpeg_dst_language_code}.embedded.{ext[1:]}"
 
                     widgets = [f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_type} file  : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                     pbar = ProgressBar(widgets=widgets, maxval=100).start()
                     subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=dst_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
                     dst_tmp_output = subtitle_embedder(media_filepath)
                     pbar.finish()
```

### Comparing `whisper_autosrt-0.1.5/whisper_autosrt.egg-info/PKG-INFO` & `whisper_autosrt-0.1.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: whisper-autosrt
-Version: 0.1.5
+Name: whisper_autosrt
+Version: 0.1.6
 Summary: a command line utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/whisper_autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
@@ -24,8 +24,8 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 
-whisper_autosrt is a command line utility for automatic speech recognition and subtitle generation. It takes video or audio files as input, generate transcriptions for them and optionally translates  them to a different language, and finally saves the resulting subtitles file to disk.               It supports a variety of input and output languages and can currently produce subtitles in SRT, VTT,JSON, and RAW format.
+whisper_autosrt is a command line utility for automatic speech recognition and subtitle generation  using faster_whisper module which is a reimplementation of OpenAI Whisper module. It takes video or audio files as input, generate transcriptions for them and optionally translates them to a differentlanguage, and finally saves the resulting subtitles file to disk.                                   It supports a variety of input and output languages and can currently produce subtitles in SRT, VTT,JSON, and RAW format.
```

