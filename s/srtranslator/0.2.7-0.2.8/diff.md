# Comparing `tmp/srtranslator-0.2.7.tar.gz` & `tmp/srtranslator-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srtranslator-0.2.7.tar", last modified: Tue May  9 19:17:52 2023, max compression
+gzip compressed data, was "srtranslator-0.2.8.tar", last modified: Tue Jun 20 18:44:52 2023, max compression
```

## Comparing `srtranslator-0.2.7.tar` & `srtranslator-0.2.8.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 19:17:52.703159 srtranslator-0.2.7/
--rw-rw-rw-   0        0        0      485 2022-12-29 01:22:11.000000 srtranslator-0.2.7/LICENSE.md
--rw-rw-rw-   0        0        0     2891 2023-05-09 19:17:52.703159 srtranslator-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     2486 2023-04-23 15:51:51.000000 srtranslator-0.2.7/README.md
--rw-rw-rw-   0        0        0       42 2023-05-09 19:17:52.703159 srtranslator-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      709 2023-05-09 19:17:01.000000 srtranslator-0.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-09 19:17:52.697154 srtranslator-0.2.7/srtranslator/
--rw-rw-rw-   0        0        0       78 2022-12-29 23:26:03.000000 srtranslator-0.2.7/srtranslator/__init__.py
--rw-rw-rw-   0        0        0     2382 2023-05-04 18:24:01.000000 srtranslator-0.2.7/srtranslator/__main__.py
--rw-rw-rw-   0        0        0     6026 2023-05-05 15:00:20.000000 srtranslator-0.2.7/srtranslator/srt_file.py
-drwxrwxrwx   0        0        0        0 2023-05-09 19:17:52.702158 srtranslator-0.2.7/srtranslator/translators/
--rw-rw-rw-   0        0        0       30 2023-02-25 14:27:16.000000 srtranslator-0.2.7/srtranslator/translators/__init__.py
--rw-rw-rw-   0        0        0      338 2023-03-31 14:53:20.000000 srtranslator-0.2.7/srtranslator/translators/base.py
--rw-rw-rw-   0        0        0      445 2023-03-31 14:58:33.000000 srtranslator-0.2.7/srtranslator/translators/deepl_api.py
--rw-rw-rw-   0        0        0     4698 2023-05-09 19:17:20.000000 srtranslator-0.2.7/srtranslator/translators/deepl_scrap.py
--rw-rw-rw-   0        0        0     4235 2023-05-04 18:23:52.000000 srtranslator-0.2.7/srtranslator/translators/selenium_utils.py
--rw-rw-rw-   0        0        0      568 2023-04-21 21:48:27.000000 srtranslator-0.2.7/srtranslator/translators/translatepy.py
-drwxrwxrwx   0        0        0        0 2023-05-09 19:17:52.699156 srtranslator-0.2.7/srtranslator.egg-info/
--rw-rw-rw-   0        0        0     2891 2023-05-09 19:17:52.000000 srtranslator-0.2.7/srtranslator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      514 2023-05-09 19:17:52.000000 srtranslator-0.2.7/srtranslator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 19:17:52.000000 srtranslator-0.2.7/srtranslator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      657 2023-05-09 19:17:52.000000 srtranslator-0.2.7/srtranslator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-09 19:17:52.000000 srtranslator-0.2.7/srtranslator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 18:44:52.084520 srtranslator-0.2.8/
+-rw-rw-rw-   0        0        0      485 2022-12-29 01:22:11.000000 srtranslator-0.2.8/LICENSE.md
+-rw-rw-rw-   0        0        0     2923 2023-06-20 18:44:52.084520 srtranslator-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2518 2023-06-20 18:44:06.000000 srtranslator-0.2.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-20 18:44:52.085520 srtranslator-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      709 2023-06-20 18:44:20.000000 srtranslator-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 18:44:52.076513 srtranslator-0.2.8/srtranslator/
+-rw-rw-rw-   0        0        0       78 2022-12-29 23:26:03.000000 srtranslator-0.2.8/srtranslator/__init__.py
+-rw-rw-rw-   0        0        0     2455 2023-06-08 15:16:00.000000 srtranslator-0.2.8/srtranslator/__main__.py
+-rw-rw-rw-   0        0        0     6026 2023-05-05 15:00:20.000000 srtranslator-0.2.8/srtranslator/srt_file.py
+drwxrwxrwx   0        0        0        0 2023-06-20 18:44:52.083518 srtranslator-0.2.8/srtranslator/translators/
+-rw-rw-rw-   0        0        0       30 2023-02-25 14:27:16.000000 srtranslator-0.2.8/srtranslator/translators/__init__.py
+-rw-rw-rw-   0        0        0      338 2023-03-31 14:53:20.000000 srtranslator-0.2.8/srtranslator/translators/base.py
+-rw-rw-rw-   0        0        0      445 2023-03-31 14:58:33.000000 srtranslator-0.2.8/srtranslator/translators/deepl_api.py
+-rw-rw-rw-   0        0        0     5476 2023-06-20 18:42:52.000000 srtranslator-0.2.8/srtranslator/translators/deepl_scrap.py
+-rw-rw-rw-   0        0        0     1074 2023-06-12 14:36:42.000000 srtranslator-0.2.8/srtranslator/translators/deeplx.py
+-rw-rw-rw-   0        0        0     4235 2023-05-04 18:23:52.000000 srtranslator-0.2.8/srtranslator/translators/selenium_utils.py
+-rw-rw-rw-   0        0        0      568 2023-04-21 21:48:27.000000 srtranslator-0.2.8/srtranslator/translators/translatepy.py
+drwxrwxrwx   0        0        0        0 2023-06-20 18:44:52.079515 srtranslator-0.2.8/srtranslator.egg-info/
+-rw-rw-rw-   0        0        0     2923 2023-06-20 18:44:52.000000 srtranslator-0.2.8/srtranslator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      549 2023-06-20 18:44:52.000000 srtranslator-0.2.8/srtranslator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 18:44:52.000000 srtranslator-0.2.8/srtranslator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      657 2023-06-20 18:44:52.000000 srtranslator-0.2.8/srtranslator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-20 18:44:52.000000 srtranslator-0.2.8/srtranslator.egg-info/top_level.txt
```

### Comparing `srtranslator-0.2.7/PKG-INFO` & `srtranslator-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srtranslator
-Version: 0.2.7
+Version: 0.2.8
 Summary: Traslate a .SRT file using any custom translator
 Home-page: https://github.com/sinedie/SRTranslator
 Author: EAR
 Author-email: sinedie@protonmail.com
 License: FREE
 Keywords: python,srt,languages,translator,subtitles
 Platform: UNKNOWN
@@ -14,66 +14,66 @@
 
 # SRTranslator
 
 ## Install
 
 [PyPI](https://pypi.org/project/srtranslator/)
 
-```
+```bash
 pip install srtranslator
 ```
 
 ## Usage in Blender
 
 [tin2tin](https://github.com/tin2tin) has made this [blender addon](https://github.com/tin2tin/import_subtitles). Check it out.
 
 ## Usage from script
 
 Import stuff
 
-```
+```python
 import os
 from srtranslator import SrtFile
 from srtranslator.translators.deepl_api import DeeplApi
 from srtranslator.translators.deepl_scrap import DeeplTranslator
 from srtranslator.translators.translatepy import TranslatePy
 ```
 
 Initialize translator. It can be any translator, even your own, check the docs, there are instructions per translator and how to create your own.
 
-```
+```python
 translator = DeeplTranslator() # or TranslatePy() or DeeplApi(api_key)
 ```
 
 Load, translate and save. For multiple recursive files in folder, check `examples folder`
 
-```
+```python
 filepath = "./filepath/to/srt"
 srt = SrtFile(filepath)
 srt.translate(translator, "en", "es")
 
 # Making the result subtitles prettier
 srt.wrap_lines()
 
 srt.save(f"{os.path.splitext(filepath)[0]}_translated.srt")
 ```
 
 Quit translator
 
-```
+```python
 translator.quit()
 ```
 
 ## Usage from GUI
 
 [KryptoST](https://github.com/KryptoST) has made a graphical user interface. You can check it out [here](https://github.com/KryptoST/SRTranslatorGUI)
 
 ## Usage command line
 
-```
+```bash
 python -m srtranslator ./filepath/to/srt -i SRC_LANG -o DEST_LANG
 ```
 
 ## Advanced usage
 
 ```
 usage: __main__.py [-h] [-i SRC_LANG] [-o DEST_LANG] [-v] [-vv] [-s] [-w WRAP_LIMIT] [-t {deepl-scrap,translatepy,deepl-api}] [--auth AUTH] path
```

### Comparing `srtranslator-0.2.7/README.md` & `srtranslator-0.2.8/srtranslator.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,65 +1,79 @@
+Metadata-Version: 2.1
+Name: srtranslator
+Version: 0.2.8
+Summary: Traslate a .SRT file using any custom translator
+Home-page: https://github.com/sinedie/SRTranslator
+Author: EAR
+Author-email: sinedie@protonmail.com
+License: FREE
+Keywords: python,srt,languages,translator,subtitles
+Platform: UNKNOWN
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 # SRTranslator
 
 ## Install
 
 [PyPI](https://pypi.org/project/srtranslator/)
 
-```
+```bash
 pip install srtranslator
 ```
 
 ## Usage in Blender
 
 [tin2tin](https://github.com/tin2tin) has made this [blender addon](https://github.com/tin2tin/import_subtitles). Check it out.
 
 ## Usage from script
 
 Import stuff
 
-```
+```python
 import os
 from srtranslator import SrtFile
 from srtranslator.translators.deepl_api import DeeplApi
 from srtranslator.translators.deepl_scrap import DeeplTranslator
 from srtranslator.translators.translatepy import TranslatePy
 ```
 
 Initialize translator. It can be any translator, even your own, check the docs, there are instructions per translator and how to create your own.
 
-```
+```python
 translator = DeeplTranslator() # or TranslatePy() or DeeplApi(api_key)
 ```
 
 Load, translate and save. For multiple recursive files in folder, check `examples folder`
 
-```
+```python
 filepath = "./filepath/to/srt"
 srt = SrtFile(filepath)
 srt.translate(translator, "en", "es")
 
 # Making the result subtitles prettier
 srt.wrap_lines()
 
 srt.save(f"{os.path.splitext(filepath)[0]}_translated.srt")
 ```
 
 Quit translator
 
-```
+```python
 translator.quit()
 ```
 
 ## Usage from GUI
 
 [KryptoST](https://github.com/KryptoST) has made a graphical user interface. You can check it out [here](https://github.com/KryptoST/SRTranslatorGUI)
 
 ## Usage command line
 
-```
+```bash
 python -m srtranslator ./filepath/to/srt -i SRC_LANG -o DEST_LANG
 ```
 
 ## Advanced usage
 
 ```
 usage: __main__.py [-h] [-i SRC_LANG] [-o DEST_LANG] [-v] [-vv] [-s] [-w WRAP_LIMIT] [-t {deepl-scrap,translatepy,deepl-api}] [--auth AUTH] path
@@ -80,7 +94,9 @@
   -s, --show-browser    Show browser window
   -w WRAP_LIMIT, --wrap-limit WRAP_LIMIT
                         Number of characters -including spaces- to wrap a line of text. Default: 50
   -t {deepl-scrap,translatepy,deepl-api}, --translator {deepl-scrap,translatepy,deepl-api}
                         Built-in translator to use
   --auth AUTH           Api key if needed on translator
 ```
+
+
```

### Comparing `srtranslator-0.2.7/setup.py` & `srtranslator-0.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 setup(
     name="srtranslator",
     description="Traslate a .SRT file using any custom translator",
     long_description=Path("README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/sinedie/SRTranslator",
-    version="0.2.7",
+    version="0.2.8",
     author="EAR",
     author_email="sinedie@protonmail.com",
     license="FREE",
     python_requires=">=3.6",
     install_requires=requirements,
     packages=find_packages(),
     keywords=["python", "srt", "languages", "translator", "subtitles"],
```

### Comparing `srtranslator-0.2.7/srtranslator/__main__.py` & `srtranslator-0.2.8/srtranslator/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import argparse
 import logging
 
 from .srt_file import SrtFile
 from .translators.deepl_api import DeeplApi
 from .translators.deepl_scrap import DeeplTranslator
 from .translators.translatepy import TranslatePy
+from .translators.deeplx import DeeplX
 
 parser = argparse.ArgumentParser(description="Translate an .STR file")
 
 parser.add_argument(
     "filepath",
     metavar="path",
     type=str,
@@ -66,29 +67,30 @@
     help="Number of characters -including spaces- to wrap a line of text. Default: 50",
 )
 
 parser.add_argument(
     "-t",
     "--translator",
     type=str,
-    choices=["deepl-scrap", "translatepy", "deepl-api"],
+    choices=["deepl-scrap", "translatepy", "deepl-api", "deeplx"],
     help="Built-in translator to use",
     default="deepl-scrap",
 )
 
 parser.add_argument(
     "--auth",
     type=str,
     help="Api key if needed on translator",
 )
 
 builtin_translators = {
     "deepl-scrap": DeeplTranslator,
     "deepl-api": DeeplApi,
     "translatepy": TranslatePy,
+    "deeplx": DeeplX,
 }
 
 args = parser.parse_args()
 logging.basicConfig(level=args.loglevel)
 
 try:
     os.environ.pop("MOZ_HEADLESS")
```

### Comparing `srtranslator-0.2.7/srtranslator/srt_file.py` & `srtranslator-0.2.8/srtranslator/srt_file.py`

 * *Files identical despite different names*

### Comparing `srtranslator-0.2.7/srtranslator/translators/deepl_scrap.py` & `srtranslator-0.2.8/srtranslator/translators/deepl_scrap.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,33 +51,48 @@
         "es": "Spanish",
         "sv": "Swedish",
         "tr": "Turkish",
         "uk": "Ukrainian",
     }
 
     def __init__(self, driver: Optional[WebDriver] = None):
+        self.last_translation_failed = False
         self.driver = driver
+
         if self.driver is None:
-            proxy = create_proxy()
-            self.driver = create_driver(proxy)
+            self._rotate_proxy()
+            return
+
+        self._reset()
 
+    def _reset(self):
         logging.info(f"Going to {self.url}")
         self.driver.get(self.url)
         self._closePopUp()
 
         self.input_lang_from = TextArea(
             self.driver, "CLASS_NAME", "lmt__source_textarea"
         )
         self.input_destination_language = TextArea(
             self.driver, "CLASS_NAME", "lmt__target_textarea"
         )
 
         self.src_lang = None
         self.target_lang = None
 
+    def _rotate_proxy(self):
+        if self.driver is not None:
+            logging.info(" ======= Translation failed. Probably got banned. ======= ")
+            logging.info("Rotating proxy")
+            self.quit()
+
+        proxy = create_proxy()
+        self.driver = create_driver(proxy)
+        self._reset()
+
     def _closePopUp(self):
         Button(
             self.driver,
             "CSS_SELECTOR",
             "[aria-label=Close]",
             wait_time=5,
             optional=True,
@@ -126,15 +141,24 @@
         # Maximun number of iterations 60 seconds
         for _ in range(60):
             translation = self.input_destination_language.value
 
             if self._is_translated(clean_text, translation):
                 time.sleep(2)
                 translation = self.input_destination_language.value
+
+                # Reset the proxy flag
+                self.last_translation_failed = False
                 return translation.replace("@[.]@", "[...]")
             time.sleep(1)
 
+        # Maybe proxy got banned, so we try with a new proxy, but just once.
+        if not self.last_translation_failed:
+            self.last_translation_failed = True
+            self._rotate_proxy()
+            return self.translate(text, source_language, destination_language)
+
         self.quit()
         raise TimeOutException("Translation timed out")
 
     def quit(self):
         self.driver.quit()
```

### Comparing `srtranslator-0.2.7/srtranslator/translators/selenium_utils.py` & `srtranslator-0.2.8/srtranslator/translators/selenium_utils.py`

 * *Files identical despite different names*

### Comparing `srtranslator-0.2.7/srtranslator/translators/translatepy.py` & `srtranslator-0.2.8/srtranslator/translators/translatepy.py`

 * *Files identical despite different names*

### Comparing `srtranslator-0.2.7/srtranslator.egg-info/PKG-INFO` & `srtranslator-0.2.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,79 +1,65 @@
-Metadata-Version: 2.1
-Name: srtranslator
-Version: 0.2.7
-Summary: Traslate a .SRT file using any custom translator
-Home-page: https://github.com/sinedie/SRTranslator
-Author: EAR
-Author-email: sinedie@protonmail.com
-License: FREE
-Keywords: python,srt,languages,translator,subtitles
-Platform: UNKNOWN
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # SRTranslator
 
 ## Install
 
 [PyPI](https://pypi.org/project/srtranslator/)
 
-```
+```bash
 pip install srtranslator
 ```
 
 ## Usage in Blender
 
 [tin2tin](https://github.com/tin2tin) has made this [blender addon](https://github.com/tin2tin/import_subtitles). Check it out.
 
 ## Usage from script
 
 Import stuff
 
-```
+```python
 import os
 from srtranslator import SrtFile
 from srtranslator.translators.deepl_api import DeeplApi
 from srtranslator.translators.deepl_scrap import DeeplTranslator
 from srtranslator.translators.translatepy import TranslatePy
 ```
 
 Initialize translator. It can be any translator, even your own, check the docs, there are instructions per translator and how to create your own.
 
-```
+```python
 translator = DeeplTranslator() # or TranslatePy() or DeeplApi(api_key)
 ```
 
 Load, translate and save. For multiple recursive files in folder, check `examples folder`
 
-```
+```python
 filepath = "./filepath/to/srt"
 srt = SrtFile(filepath)
 srt.translate(translator, "en", "es")
 
 # Making the result subtitles prettier
 srt.wrap_lines()
 
 srt.save(f"{os.path.splitext(filepath)[0]}_translated.srt")
 ```
 
 Quit translator
 
-```
+```python
 translator.quit()
 ```
 
 ## Usage from GUI
 
 [KryptoST](https://github.com/KryptoST) has made a graphical user interface. You can check it out [here](https://github.com/KryptoST/SRTranslatorGUI)
 
 ## Usage command line
 
-```
+```bash
 python -m srtranslator ./filepath/to/srt -i SRC_LANG -o DEST_LANG
 ```
 
 ## Advanced usage
 
 ```
 usage: __main__.py [-h] [-i SRC_LANG] [-o DEST_LANG] [-v] [-vv] [-s] [-w WRAP_LIMIT] [-t {deepl-scrap,translatepy,deepl-api}] [--auth AUTH] path
@@ -94,9 +80,7 @@
   -s, --show-browser    Show browser window
   -w WRAP_LIMIT, --wrap-limit WRAP_LIMIT
                         Number of characters -including spaces- to wrap a line of text. Default: 50
   -t {deepl-scrap,translatepy,deepl-api}, --translator {deepl-scrap,translatepy,deepl-api}
                         Built-in translator to use
   --auth AUTH           Api key if needed on translator
 ```
-
-
```

### Comparing `srtranslator-0.2.7/srtranslator.egg-info/SOURCES.txt` & `srtranslator-0.2.8/srtranslator.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -9,9 +9,10 @@
 srtranslator.egg-info/dependency_links.txt
 srtranslator.egg-info/requires.txt
 srtranslator.egg-info/top_level.txt
 srtranslator/translators/__init__.py
 srtranslator/translators/base.py
 srtranslator/translators/deepl_api.py
 srtranslator/translators/deepl_scrap.py
+srtranslator/translators/deeplx.py
 srtranslator/translators/selenium_utils.py
 srtranslator/translators/translatepy.py
```

### Comparing `srtranslator-0.2.7/srtranslator.egg-info/requires.txt` & `srtranslator-0.2.8/srtranslator.egg-info/requires.txt`

 * *Files identical despite different names*

