# Comparing `tmp/emailalert-1.2.5.tar.gz` & `tmp/emailalert-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailalert-1.2.5.tar", last modified: Tue Jun 20 02:43:28 2023, max compression
+gzip compressed data, was "emailalert-1.2.6.tar", last modified: Tue Jun 20 04:33:42 2023, max compression
```

## Comparing `emailalert-1.2.5.tar` & `emailalert-1.2.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 02:43:28.073362 emailalert-1.2.5/
--rw-rw-rw-   0        0        0      178 2023-06-20 02:43:28.071358 emailalert-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 02:43:28.028948 emailalert-1.2.5/emailalert.egg-info/
--rw-rw-rw-   0        0        0      178 2023-06-20 02:43:27.000000 emailalert-1.2.5/emailalert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-06-20 02:43:27.000000 emailalert-1.2.5/emailalert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 02:43:27.000000 emailalert-1.2.5/emailalert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-06-20 02:43:27.000000 emailalert-1.2.5/emailalert.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-20 02:43:28.066359 emailalert-1.2.5/sck/
--rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.2.5/sck/__init__.py
--rw-rw-rw-   0        0        0     4133 2023-06-20 02:43:22.000000 emailalert-1.2.5/sck/emailalert.py
--rw-rw-rw-   0        0        0       42 2023-06-20 02:43:28.074369 emailalert-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0      253 2023-06-20 02:40:59.000000 emailalert-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 04:33:42.822183 emailalert-1.2.6/
+-rw-rw-rw-   0        0        0      178 2023-06-20 04:33:42.817181 emailalert-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 04:33:42.768180 emailalert-1.2.6/emailalert.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-06-20 04:33:42.000000 emailalert-1.2.6/emailalert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-06-20 04:33:42.000000 emailalert-1.2.6/emailalert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 04:33:42.000000 emailalert-1.2.6/emailalert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-06-20 04:33:42.000000 emailalert-1.2.6/emailalert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 04:33:42.810184 emailalert-1.2.6/sck/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.2.6/sck/__init__.py
+-rw-rw-rw-   0        0        0     3854 2023-06-20 04:33:35.000000 emailalert-1.2.6/sck/emailalert.py
+-rw-rw-rw-   0        0        0       42 2023-06-20 04:33:42.822794 emailalert-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      253 2023-06-20 04:33:29.000000 emailalert-1.2.6/setup.py
```

### Comparing `emailalert-1.2.5/README.md` & `emailalert-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `emailalert-1.2.5/sck/emailalert.py` & `emailalert-1.2.6/sck/emailalert.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,15 +23,16 @@
     return file_names
 
 
 def send(recipients,subject,message, folder_paths, backup_folders):
     # Email details
     smtp_server = 'mrelay.noc.sony.co.jp'
     smtp_port = 25
-    sender = 'SCK-H5BAREVOS-NGK-SYSADMIN@sony.com'
+    #sender = 'SCK-H5BAREVOS-NGK-SYSADMIN@sony.com'
+    sender = 'VOS_MAP_SYSTEM@sony.com'
 
     # Create a MIME text object
     #msg = MIMEText(message)
     msg = MIMEMultipart()
     msg['Subject'] = subject
     msg['From'] = sender
     #msg['To'] = recipient
@@ -81,44 +82,36 @@
     message += f'<html><body>{table_html}</body></html>'
 
     #msg.attach(MIMEText(message, 'plain'))
 
     # Attach the email body
     msg.attach(MIMEText(message, 'html'))
 
-    # Find files with the specified extension in the folder
-    # attachment_paths = []
-    # sendEmail = 0
-    # for file_name in os.listdir(folder_path):
-    #     if file_name.endswith(file_extension):
-    #         attachment_paths.append(os.path.join(folder_path, file_name))
-    #         sendEmail = 1
-    # if sendEmail==0:
-    #     return 0
 
     # Attach the files to the email
-    for file_path in attachment_paths:
-        attachment = MIMEBase("application", "octet-stream")
-        with open(file_path, "rb") as file:
-            attachment.set_payload(file.read())
-        encoders.encode_base64(attachment)
-        attachment.add_header(
-            "Content-Disposition",
-            f"attachment; filename= {os.path.basename(file_path)}",
-        )
-        msg.attach(attachment)
-        # Move the attached file to the backup folder
-        backup_folder = backup_folders[0]
-        if 'Tokyo' in file_path:
-            backup_folder = backup_folders[1]  # Relative path to the backup folder
-        elif 'MCO' in file_path:
-            backup_folder = backup_folders[2]  # Relative path to the backup folder
-        current_dir = os.getcwd()  # Get the current working directory
-        backup_file_path = os.path.abspath(os.path.join(current_dir, backup_folder, os.path.basename(file_path)))
-        shutil.move(file_path, backup_file_path)
+    # for file_path in attachment_paths:
+    #     attachment = MIMEBase("application", "octet-stream")
+    #     with open(file_path, "rb") as file:
+    #         attachment.set_payload(file.read())
+    #     encoders.encode_base64(attachment)
+    #     attachment.add_header(
+    #         "Content-Disposition",
+    #         f"attachment; filename= {os.path.basename(file_path)}",
+    #     )
+    #     msg.attach(attachment)
+    #     # Move the attached file to the backup folder
+    #     backup_folder = backup_folders[0]
+    #     if 'Tokyo' in file_path:
+    #         backup_folder = backup_folders[1]  # Relative path to the backup folder
+    #     elif 'MCO' in file_path:
+    #         backup_folder = backup_folders[2]  # Relative path to the backup folder
+    #     current_dir = os.getcwd()  # Get the current working directory
+    #     backup_file_path = os.path.abspath(os.path.join(current_dir, backup_folder, os.path.basename(file_path)))
+    #     shutil.move(file_path, backup_file_path)
+
 
     # Connect to the SMTP server
     with smtplib.SMTP(smtp_server, smtp_port) as server:
         try:    
             server.sendmail(sender, recipients, msg.as_string())
             return 1
         except Exception as e:
```

