# Comparing `tmp/emailalert-1.2.3.tar.gz` & `tmp/emailalert-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailalert-1.2.3.tar", last modified: Tue Jun 20 02:14:46 2023, max compression
+gzip compressed data, was "emailalert-1.2.4.tar", last modified: Tue Jun 20 02:25:57 2023, max compression
```

## Comparing `emailalert-1.2.3.tar` & `emailalert-1.2.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 02:14:46.523948 emailalert-1.2.3/
--rw-rw-rw-   0        0        0      178 2023-06-20 02:14:46.522153 emailalert-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 02:14:46.485218 emailalert-1.2.3/emailalert.egg-info/
--rw-rw-rw-   0        0        0      178 2023-06-20 02:14:46.000000 emailalert-1.2.3/emailalert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-06-20 02:14:46.000000 emailalert-1.2.3/emailalert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 02:14:46.000000 emailalert-1.2.3/emailalert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-06-20 02:14:46.000000 emailalert-1.2.3/emailalert.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-20 02:14:46.515087 emailalert-1.2.3/sck/
--rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.2.3/sck/__init__.py
--rw-rw-rw-   0        0        0     3742 2023-06-20 02:14:30.000000 emailalert-1.2.3/sck/emailalert.py
--rw-rw-rw-   0        0        0       42 2023-06-20 02:14:46.526958 emailalert-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0      253 2023-06-20 02:14:39.000000 emailalert-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 02:25:57.605161 emailalert-1.2.4/
+-rw-rw-rw-   0        0        0      178 2023-06-20 02:25:57.602447 emailalert-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 02:25:57.546905 emailalert-1.2.4/emailalert.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-06-20 02:25:57.000000 emailalert-1.2.4/emailalert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-06-20 02:25:57.000000 emailalert-1.2.4/emailalert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 02:25:57.000000 emailalert-1.2.4/emailalert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-06-20 02:25:57.000000 emailalert-1.2.4/emailalert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 02:25:57.594042 emailalert-1.2.4/sck/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.2.4/sck/__init__.py
+-rw-rw-rw-   0        0        0     4094 2023-06-20 02:25:50.000000 emailalert-1.2.4/sck/emailalert.py
+-rw-rw-rw-   0        0        0       42 2023-06-20 02:25:57.607095 emailalert-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      253 2023-06-20 02:24:30.000000 emailalert-1.2.4/setup.py
```

### Comparing `emailalert-1.2.3/README.md` & `emailalert-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `emailalert-1.2.3/sck/emailalert.py` & `emailalert-1.2.4/sck/emailalert.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,21 +40,44 @@
     # Get all file paths in the folders
     attachment_paths = get_files_in_folders(folder_paths)
 
     # Get all file names in the folders
     attachment_file_names = get_filenames_in_folders(folder_paths)
 
     # Add the email body with the list of attached files
-    message += "\n\r".join(attachment_file_names)
+    #message += "\n\r".join(attachment_file_names)
+
+    # Create the HTML table with CSS styles
+    table_html = '''
+    <style>
+        table {
+            border-collapse: collapse;
+            width: 100%;
+        }
+
+        th, td {
+            border: 1px solid black;
+            padding: 8px;
+            text-align: left;
+        }
+
+        th {
+            background-color: #f2f2f2;
+        }
+    </style>
+
+    <table>
+        <tr>
+            <th>Folder Paths</th>
+        </tr>
+    '''
+
+    for folder_path in folder_paths:
+        table_html += f'<tr><td>{folder_path}</td></tr>'
 
-    # Create the HTML table
-    table_html = '<table>'
-    table_html += '<tr><th>エラーファイル</th></tr>'
-    for errorfile in attachment_file_names:
-        table_html += f'<tr><td>{errorfile}</td></tr>'
     table_html += '</table>'
 
     # Create the email body as HTML
     message += f'<html><body>{table_html}</body></html>'
 
     #msg.attach(MIMEText(message, 'plain'))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

