# Comparing `tmp/apidownload-2.0.0-py3-none-any.whl.zip` & `tmp/apidownload-2.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 4470 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat     2004 b- defN 23-Jun-09 20:22 apidownload/__init__.py
--rw-rw-rw-  2.0 fat       62 b- defN 23-Jun-09 20:58 apidownload/__main__.py
+Zip file size: 4978 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat     3049 b- defN 23-Jun-20 19:59 apidownload/__init__.py
+-rw-rw-rw-  2.0 fat      446 b- defN 23-Jun-20 20:10 apidownload/__main__.py
 -rw-rw-rw-  2.0 fat      190 b- defN 23-May-16 19:19 apidownload/apidownload.json
 -rw-rw-rw-  2.0 fat      190 b- defN 23-May-16 19:19 apidownload/default_settings.json
--rw-rw-rw-  2.0 fat     1714 b- defN 23-Jun-09 21:04 apidownload-2.0.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     1060 b- defN 23-Jun-09 21:04 apidownload-2.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-09 21:04 apidownload-2.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       49 b- defN 23-Jun-09 21:04 apidownload-2.0.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       12 b- defN 23-Jun-09 21:04 apidownload-2.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      840 b- defN 23-Jun-09 21:04 apidownload-2.0.0.dist-info/RECORD
-10 files, 6213 bytes uncompressed, 3020 bytes compressed:  51.4%
+-rw-rw-rw-  2.0 fat     1714 b- defN 23-Jun-20 20:14 apidownload-2.1.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     1317 b- defN 23-Jun-20 20:14 apidownload-2.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-20 20:14 apidownload-2.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       58 b- defN 23-Jun-20 20:14 apidownload-2.1.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Jun-20 20:14 apidownload-2.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      841 b- defN 23-Jun-20 20:14 apidownload-2.1.0.dist-info/RECORD
+10 files, 7909 bytes uncompressed, 3528 bytes compressed:  55.4%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: apidownload/apidownload.json
 Comment: 
 
 Filename: apidownload/default_settings.json
 Comment: 
 
-Filename: apidownload-2.0.0.dist-info/LICENSE.txt
+Filename: apidownload-2.1.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: apidownload-2.0.0.dist-info/METADATA
+Filename: apidownload-2.1.0.dist-info/METADATA
 Comment: 
 
-Filename: apidownload-2.0.0.dist-info/WHEEL
+Filename: apidownload-2.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: apidownload-2.0.0.dist-info/entry_points.txt
+Filename: apidownload-2.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: apidownload-2.0.0.dist-info/top_level.txt
+Filename: apidownload-2.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: apidownload-2.0.0.dist-info/RECORD
+Filename: apidownload-2.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## apidownload/__init__.py

```diff
@@ -4,72 +4,92 @@
 import json
 import shutil
 import sys
 from pathlib import Path
 
 import requests
 
-SETTINGS_FILE = Path('apidownload.json')
 
-
-def fetch_endpoint(url: str, file: str, indent: int = 2):
+class ApiDownload:
     """
-    Download the JSON data at url and save it in file
+    Class for downloading from the endpoints given in a file
     """
-    print('Updating ', file, sep='')
-    try:
-        request = requests.get(url, timeout=20)
-    except requests.ConnectionError:
-        print('\tCouldn\'t connect to', url, file=sys.stderr)
-        return
-    try:
-        data = request.json()
-    except requests.JSONDecodeError:
-        print('\tInvalid JSON format returned', file=sys.stderr)
-        return
-    Path(file).write_text(json.dumps(data, indent=indent))
-    print('\tDone')
 
+    DEFAULT_SETTINGS_FILE = Path('apidownload.json')
 
-def create_settings_file():
-    """
-    Copy the example settings.json file into this directory
-    """
-    shutil.copyfile(
-        Path(__file__).parent / 'apidownload.json',
-        SETTINGS_FILE
-    )
-    print('Created', SETTINGS_FILE.absolute())
-
-
-def check_endpoint(endpoint: dict):
-    valid = True
-    if 'url' not in endpoint:
-        print('Missing "url" parameter:', endpoint)
-        valid = False
-    if 'file' not in endpoint:
-        print('Missing "file" parameter:', endpoint)
-        valid = False
-    return valid
+    def __init__(self, settings_path: str | None = None):
+        if settings_path is None:
+            self.settings_folder = Path()
+            self.settings_file = self.DEFAULT_SETTINGS_FILE
+        else:
+            path = Path(settings_path)
+            if path.is_dir():
+                self.settings_folder = path
+                self.settings_file = path / self.DEFAULT_SETTINGS_FILE
+            else:
+                self.settings_folder = path.parent
+                self.settings_file = path
 
-def main():
-    """
-    Entry-point to program
-    """
-    if SETTINGS_FILE.exists():
+    def _fetch_endpoint(self, url: str, file: str, indent: int = 2):
+        """
+        Download the JSON data at url and save it in file
+        """
+        print('Updating ', file, sep='')
         try:
-            settings = json.loads(SETTINGS_FILE.read_text())
-        except json.JSONDecodeError:
-            print('Invalid JSON format:', SETTINGS_FILE.absolute(), file=sys.stderr)
+            request = requests.get(url, timeout=20)
+        except requests.ConnectionError:
+            print('\tCouldn\'t connect to', url, file=sys.stderr)
             return
-        for endpoint in settings:
-            if isinstance(endpoint, dict):
-                if check_endpoint(endpoint):
-                    fetch_endpoint(**endpoint)
-            else:
-                print('Invalid endpoint type:', endpoint, file=sys.stderr)
-    else:
-        create_settings_file()
+        try:
+            data = request.json()
+        except requests.JSONDecodeError:
+            print('\tInvalid JSON format returned', file=sys.stderr)
+            return
+        path = Path(file)
+        if not path.is_absolute():
+            path = self.settings_folder / path
+        path.write_text(json.dumps(data, indent=indent))
+        print('\tDone')
+
+    def _create_settings_file(self):
+        """
+        Copy the example settings.json file into this directory
+        """
+        shutil.copyfile(
+            Path(__file__).parent / 'apidownload.json',
+            self.settings_file
+        )
+        print('Created', self.settings_file.absolute())
+
+    def _check_endpoint(self, endpoint: dict):
+        valid = True
+        if 'url' not in endpoint:
+            print('Missing "url" parameter:', endpoint)
+            valid = False
+        if 'file' not in endpoint:
+            print('Missing "file" parameter:', endpoint)
+            valid = False
+        return valid
+
+    def run(self):
+        """
+        Entry-point to program
+        """
+        if self.settings_file.exists():
+            try:
+                settings = json.loads(self.settings_file.read_text())
+            except json.JSONDecodeError:
+                print('Invalid JSON format:',
+                      self.settings_file.absolute(), file=sys.stderr)
+                return
+            for endpoint in settings:
+                if isinstance(endpoint, dict):
+                    if self._check_endpoint(endpoint):
+                        self._fetch_endpoint(**endpoint)
+                else:
+                    print('Invalid endpoint type:', endpoint, file=sys.stderr)
+        else:
+            self._create_settings_file()
 
 
 if __name__ == '__main__':
-    main()
+    ApiDownload().run()
```

## apidownload/__main__.py

```diff
@@ -1,4 +1,15 @@
-from . import main
+from argparse import ArgumentParser
+from . import ApiDownload
+
+def main():
+    parser = ArgumentParser(
+        prog='apidownload',
+        description='Download JSON data from API endpoints',
+    )
+    parser.add_argument('path', default='.', nargs='?',
+                        help='Provide an alternative directory or file')
+    args = parser.parse_args()
+    ApiDownload(args.path).run()
 
 if __name__ == '__main__':
     main()
```

## Comparing `apidownload-2.0.0.dist-info/LICENSE.txt` & `apidownload-2.1.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `apidownload-2.0.0.dist-info/METADATA` & `apidownload-2.1.0.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidownload
-Version: 2.0.0
+Version: 2.1.0
 Summary: Download the data from an API endpoint to a file
 Author: Joe Greaves
 Project-URL: Homepage, https://github.com/Grvs44/API-Download
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -23,12 +23,23 @@
 ## Run
 ```cmd
 apidownload
 ```
 or
 ```cmd
 python -m apidownload
-````
+```
 * The first time `apidownload` is run in a directory, an `apidownload.json` file is created.
   * This contains the endpoint URLs and the file paths to store the data in.
   * Optionally, the `indent` property may be provided to override the default indentation level of 2 spaces.
 * If the `apidownload.json` file exists in this directory, the endpoints are downloaded to the specified files.
+
+The path to the file/folder can optionally be given as a positional parameter:
+* Custom folder:
+  ```cmd
+  apidownload myfolder
+  ```
+* Custom file:
+  ```cmd
+  apidownload myfolder/myfile.txt
+  ```
+* Both absolute and relative paths are allowed.
```

