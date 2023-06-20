# Comparing `tmp/emailalert-1.2.1.tar.gz` & `tmp/emailalert-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailalert-1.2.1.tar", last modified: Tue Jun 20 01:12:21 2023, max compression
+gzip compressed data, was "emailalert-1.2.2.tar", last modified: Tue Jun 20 02:08:00 2023, max compression
```

## Comparing `emailalert-1.2.1.tar` & `emailalert-1.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 01:12:21.742984 emailalert-1.2.1/
--rw-rw-rw-   0        0        0      178 2023-06-20 01:12:21.741023 emailalert-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 01:12:21.711984 emailalert-1.2.1/emailalert.egg-info/
--rw-rw-rw-   0        0        0      178 2023-06-20 01:12:21.000000 emailalert-1.2.1/emailalert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-06-20 01:12:21.000000 emailalert-1.2.1/emailalert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 01:12:21.000000 emailalert-1.2.1/emailalert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-06-20 01:12:21.000000 emailalert-1.2.1/emailalert.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-20 01:12:21.737020 emailalert-1.2.1/sck/
--rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.2.1/sck/__init__.py
--rw-rw-rw-   0        0        0     3317 2023-06-20 01:11:58.000000 emailalert-1.2.1/sck/emailalert.py
--rw-rw-rw-   0        0        0       42 2023-06-20 01:12:21.744097 emailalert-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0      253 2023-06-20 00:15:33.000000 emailalert-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 02:08:00.353196 emailalert-1.2.2/
+-rw-rw-rw-   0        0        0      178 2023-06-20 02:08:00.349806 emailalert-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 02:08:00.314375 emailalert-1.2.2/emailalert.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-06-20 02:08:00.000000 emailalert-1.2.2/emailalert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-06-20 02:08:00.000000 emailalert-1.2.2/emailalert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 02:08:00.000000 emailalert-1.2.2/emailalert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-06-20 02:08:00.000000 emailalert-1.2.2/emailalert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 02:08:00.344810 emailalert-1.2.2/sck/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.2.2/sck/__init__.py
+-rw-rw-rw-   0        0        0     3744 2023-06-20 02:07:38.000000 emailalert-1.2.2/sck/emailalert.py
+-rw-rw-rw-   0        0        0       42 2023-06-20 02:08:00.354225 emailalert-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      253 2023-06-20 02:07:56.000000 emailalert-1.2.2/setup.py
```

### Comparing `emailalert-1.2.1/README.md` & `emailalert-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `emailalert-1.2.1/sck/emailalert.py` & `emailalert-1.2.2/sck/emailalert.py`

 * *Files 24% similar despite different names*

```diff
@@ -41,16 +41,30 @@
     attachment_paths = get_files_in_folders(folder_paths)
 
     # Get all file names in the folders
     attachment_file_names = get_filenames_in_folders(folder_paths)
 
     # Add the email body with the list of attached files
     message += "\n\r".join(attachment_file_names)
+
+    # Create the HTML table
+    table_html = '<table>'
+    table_html += '<tr><th>エラーファイル</th></tr>'
+    for errorfile in attachment_file_names:
+        table_html += f'<tr><td>{errorfile}</td></tr>'
+    table_html += '</table>'
+
+    # Create the email body as HTML
+    body_html = f'<html><body>{table_html}</body></html>'
+
     msg.attach(MIMEText(message, 'plain'))
 
+    # Attach the email body
+    msg.attach(MIMEText(body_html, 'html'))
+
     # Find files with the specified extension in the folder
     # attachment_paths = []
     # sendEmail = 0
     # for file_name in os.listdir(folder_path):
     #     if file_name.endswith(file_extension):
     #         attachment_paths.append(os.path.join(folder_path, file_name))
     #         sendEmail = 1
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

