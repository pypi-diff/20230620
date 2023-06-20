# Comparing `tmp/emailalert-1.2.7.tar.gz` & `tmp/emailalert-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailalert-1.2.7.tar", last modified: Tue Jun 20 06:21:07 2023, max compression
+gzip compressed data, was "emailalert-1.2.8.tar", last modified: Tue Jun 20 06:45:35 2023, max compression
```

## Comparing `emailalert-1.2.7.tar` & `emailalert-1.2.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 06:21:07.616968 emailalert-1.2.7/
--rw-rw-rw-   0        0        0      178 2023-06-20 06:21:07.615092 emailalert-1.2.7/PKG-INFO
--rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 06:21:07.585761 emailalert-1.2.7/emailalert.egg-info/
--rw-rw-rw-   0        0        0      178 2023-06-20 06:21:07.000000 emailalert-1.2.7/emailalert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-06-20 06:21:07.000000 emailalert-1.2.7/emailalert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 06:21:07.000000 emailalert-1.2.7/emailalert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-06-20 06:21:07.000000 emailalert-1.2.7/emailalert.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-20 06:21:07.610779 emailalert-1.2.7/sck/
--rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.2.7/sck/__init__.py
--rw-rw-rw-   0        0        0     4032 2023-06-20 06:20:57.000000 emailalert-1.2.7/sck/emailalert.py
--rw-rw-rw-   0        0        0       42 2023-06-20 06:21:07.618451 emailalert-1.2.7/setup.cfg
--rw-rw-rw-   0        0        0      253 2023-06-20 06:21:03.000000 emailalert-1.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 06:45:35.322692 emailalert-1.2.8/
+-rw-rw-rw-   0        0        0      178 2023-06-20 06:45:35.320711 emailalert-1.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.2.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 06:45:35.287186 emailalert-1.2.8/emailalert.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-06-20 06:45:35.000000 emailalert-1.2.8/emailalert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-06-20 06:45:35.000000 emailalert-1.2.8/emailalert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 06:45:35.000000 emailalert-1.2.8/emailalert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-06-20 06:45:35.000000 emailalert-1.2.8/emailalert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 06:45:35.313740 emailalert-1.2.8/sck/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.2.8/sck/__init__.py
+-rw-rw-rw-   0        0        0     3704 2023-06-20 06:45:20.000000 emailalert-1.2.8/sck/emailalert.py
+-rw-rw-rw-   0        0        0       42 2023-06-20 06:45:35.322692 emailalert-1.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      253 2023-06-20 06:22:41.000000 emailalert-1.2.8/setup.py
```

### Comparing `emailalert-1.2.7/README.md` & `emailalert-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `emailalert-1.2.7/sck/emailalert.py` & `emailalert-1.2.8/sck/emailalert.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,30 +4,23 @@
 from email.mime.multipart import MIMEMultipart
 from email.mime.base import MIMEBase
 from email import encoders
 import shutil
 
 def get_files_in_folders(folder_paths):
     file_paths = []
+    file_names = []
     for folder_path in folder_paths:
         for root, dirs, files in os.walk(folder_path):
             for file in files:
                 file_paths.append(os.path.join(root, file))
-    return file_paths
-
-def get_filenames_in_folders(folder_paths):
-    file_names = []
-    for folder_path in folder_paths:
-        for root, dirs, files in os.walk(folder_path):
-            for file_name in files:
-                file_names.append(file_name)
-    return file_names
+                file_names.append(file)
+    return file_paths, file_names
 
-
-def send(recipients,subject,message, folder_paths, backup_folders):
+def send(recipients,subject,message_header,message_footer, folder_paths):
     # Email details
     smtp_server = 'mrelay.noc.sony.co.jp'
     smtp_port = 25
     #sender = 'SCK-H5BAREVOS-NGK-SYSADMIN@sony.com'
     sender = 'VOS_MAP_SYSTEM@sony.com'
 
     # Create a MIME text object
@@ -35,21 +28,15 @@
     msg = MIMEMultipart()
     msg['Subject'] = subject
     msg['From'] = sender
     #msg['To'] = recipient
     msg['To'] = ', '.join(recipients)
 
     # Get all file paths in the folders
-    attachment_paths = get_files_in_folders(folder_paths)
-
-    # Get all file names in the folders
-    attachment_file_names = get_filenames_in_folders(folder_paths)
-
-    # Add the email body with the list of attached files
-    #message += "\n\r".join(attachment_file_names)
+    attachment_paths,attachment_filename = get_files_in_folders(folder_paths)
 
     # Create the HTML table with CSS styles
     table_html = '''
     <style>
         table {
             border-collapse: collapse;
             width: 70%;
@@ -69,29 +56,29 @@
 
     <table>
         <tr>
             <th>仕様</th>
             <th>エラーファイル</th>
         </tr>
     '''
-    spec = 'LDD'
-    for file_path in attachment_paths:
+    for file_name, file_path in zip(attachment_filename, attachment_paths):
+        spec = 'LDD'
         if 'Tokyo' in file_path:
             spec = 'Tokyo'
         elif 'MCO' in file_path:
             spec = 'MCO'
-
-    for filename in attachment_file_names:
-        table_html += f'<tr><td>{spec}</td><td>{filename}</td></tr>'
+        table_html += f'<tr><td>{spec}</td><td>{file_name}</td></tr>'
+        
 
     table_html += '</table>'
 
     # Create the email body as HTML
+    message = message_header
     message += f'<html><body>{table_html}</body></html>'
-
+    message += message_footer
 
     # Attach the email body
     msg.attach(MIMEText(message, 'html'))
 
 
     # Attach the files to the email
     # for file_path in attachment_paths:
```

