# Comparing `tmp/speedtab-0.1.4.3.tar.gz` & `tmp/speedtab-0.1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedtab-0.1.4.3.tar", max compression
+gzip compressed data, was "speedtab-0.1.4.4.tar", max compression
```

## Comparing `speedtab-0.1.4.3.tar` & `speedtab-0.1.4.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      567 2023-06-09 14:06:58.840419 speedtab-0.1.4.3/pyproject.toml
--rw-r--r--   0        0        0      365 2023-06-09 12:04:52.821400 speedtab-0.1.4.3/speedtab/__init__.py
--rw-r--r--   0        0        0    49965 2023-06-09 14:02:35.172019 speedtab-0.1.4.3/speedtab/client.py
--rw-r--r--   0        0        0     6192 2023-05-19 11:01:11.239027 speedtab-0.1.4.3/speedtab/enums.py
--rw-r--r--   0        0        0     1724 2023-06-02 10:10:18.366392 speedtab-0.1.4.3/speedtab/formats.py
--rw-r--r--   0        0        0      783 2023-06-09 14:07:05.126043 speedtab-0.1.4.3/setup.py
--rw-r--r--   0        0        0      808 2023-06-09 14:07:05.126043 speedtab-0.1.4.3/PKG-INFO
+-rw-r--r--   0        0        0      567 2023-06-20 10:33:01.350911 speedtab-0.1.4.4/pyproject.toml
+-rw-r--r--   0        0        0      365 2023-06-09 12:04:52.821400 speedtab-0.1.4.4/speedtab/__init__.py
+-rw-r--r--   0        0        0    50278 2023-06-20 10:30:24.690346 speedtab-0.1.4.4/speedtab/client.py
+-rw-r--r--   0        0        0     6192 2023-05-19 11:01:11.239027 speedtab-0.1.4.4/speedtab/enums.py
+-rw-r--r--   0        0        0     1724 2023-06-02 10:10:18.366392 speedtab-0.1.4.4/speedtab/formats.py
+-rw-r--r--   0        0        0      783 2023-06-20 10:33:07.196287 speedtab-0.1.4.4/setup.py
+-rw-r--r--   0        0        0      808 2023-06-20 10:33:07.196287 speedtab-0.1.4.4/PKG-INFO
```

### Comparing `speedtab-0.1.4.3/pyproject.toml` & `speedtab-0.1.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "speedtab"
-version = "0.1.4.3"
+version = "0.1.4.4"
 description = "Convenient wrapper for working with Google Spreadsheets"
 authors = ["Bogdan Gergel <bogger147@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/BoggerSancho/SpeedTab-beta"
 repository = "https://github.com/BoggerSancho/SpeedTab-beta"
 
 [tool.poetry.dependencies]
```

### Comparing `speedtab-0.1.4.3/speedtab/client.py` & `speedtab-0.1.4.4/speedtab/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import io
 import re
-from collections.abc import Iterable
 from datetime import datetime, date
 from itertools import zip_longest
 from typing import Union
 
 import numpy as np
 import pandas as pd
 from google.oauth2.credentials import Credentials
@@ -528,15 +527,19 @@
                   offset_y_pixels: int = 0,
                   header_count: int = 1,
                   data_start: tuple = (0, 0),
                   nrows: int = None,
                   data_sheet_name=None,):
 
         data_start_cell = parse_range(data_start)
-        target_axis = [target_axis] if not isinstance(target_axis, Iterable) else target_axis
+        target_axis = [target_axis] if not isinstance(target_axis, (list, tuple)) else target_axis
+
+        if len(columns) < len(target_axis):
+            raise ValueError('Amount of target_axis must be lower than amount of columns in chart')
+
         series = [{
             'series': {
                 'sourceRange': {
                     'sources': [
                         {
                             'sheetId': self.sheet_id if not data_sheet_name else self.base.sheets.get(data_sheet_name).get('sheetId'),
                             'startRowIndex': data_start_cell[0],
@@ -1010,14 +1013,17 @@
                                                                 'gridProperties': {'hideGridlines': grid}}}
                                                 for sheet_name, grid in zip(sheets, hide_grid_lines)]})
                          .execute().get('spreadsheetId'), token_path=self.token_path,
                          credentials=self.credentials, connect_v4=self.connect_v4, connect_v3=self.connect_v3)
         self.list_of_spreadsheets.append(ss)
         return ss
 
+    def create_copy_of_spreadsheet(self, file_id: str, new_title: str):
+        return self.connect_v3.files().copy(fileId=file_id, body={'name': new_title}, supportsAllDrives=True).execute()
+
     def create_folder(self, folder_name: str, parent_id: str = None):
         return self.connect_v3.files().create(body={
             'name': folder_name,
             'mimeType': "application/vnd.google-apps.folder",
             'parents': [parent_id] if parent_id else None,
         }, supportsAllDrives=True).execute()['id']
```

### Comparing `speedtab-0.1.4.3/speedtab/enums.py` & `speedtab-0.1.4.4/speedtab/enums.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.1.4.3/speedtab/formats.py` & `speedtab-0.1.4.4/speedtab/formats.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.1.4.3/setup.py` & `speedtab-0.1.4.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['google-api-python-client>=2.58.0,<3.0.0',
  'google-auth-httplib2>=0.1.0,<0.2.0',
  'google-auth-oauthlib>=0.5.2,<0.6.0']
 
 setup_kwargs = {
     'name': 'speedtab',
-    'version': '0.1.4.3',
+    'version': '0.1.4.4',
     'description': 'Convenient wrapper for working with Google Spreadsheets',
     'long_description': None,
     'author': 'Bogdan Gergel',
     'author_email': 'bogger147@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/BoggerSancho/SpeedTab-beta',
```

### Comparing `speedtab-0.1.4.3/PKG-INFO` & `speedtab-0.1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtab
-Version: 0.1.4.3
+Version: 0.1.4.4
 Summary: Convenient wrapper for working with Google Spreadsheets
 Home-page: https://github.com/BoggerSancho/SpeedTab-beta
 License: MIT
 Author: Bogdan Gergel
 Author-email: bogger147@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

