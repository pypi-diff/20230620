# Comparing `tmp/emailalert-1.2.0.tar.gz` & `tmp/emailalert-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailalert-1.2.0.tar", last modified: Mon Jun 19 10:27:13 2023, max compression
+gzip compressed data, was "emailalert-1.2.1.tar", last modified: Tue Jun 20 01:12:21 2023, max compression
```

## Comparing `emailalert-1.2.0.tar` & `emailalert-1.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 10:27:13.937209 emailalert-1.2.0/
--rw-rw-rw-   0        0        0      178 2023-06-19 10:27:13.934198 emailalert-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 10:27:13.900358 emailalert-1.2.0/emailalert.egg-info/
--rw-rw-rw-   0        0        0      178 2023-06-19 10:27:13.000000 emailalert-1.2.0/emailalert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-06-19 10:27:13.000000 emailalert-1.2.0/emailalert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 10:27:13.000000 emailalert-1.2.0/emailalert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-06-19 10:27:13.000000 emailalert-1.2.0/emailalert.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 10:27:13.929196 emailalert-1.2.0/sck/
--rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.2.0/sck/__init__.py
--rw-rw-rw-   0        0        0     3318 2023-06-19 10:27:02.000000 emailalert-1.2.0/sck/emailalert.py
--rw-rw-rw-   0        0        0       42 2023-06-19 10:27:13.937209 emailalert-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      253 2023-06-19 10:27:09.000000 emailalert-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 01:12:21.742984 emailalert-1.2.1/
+-rw-rw-rw-   0        0        0      178 2023-06-20 01:12:21.741023 emailalert-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 01:12:21.711984 emailalert-1.2.1/emailalert.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-06-20 01:12:21.000000 emailalert-1.2.1/emailalert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-06-20 01:12:21.000000 emailalert-1.2.1/emailalert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 01:12:21.000000 emailalert-1.2.1/emailalert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-06-20 01:12:21.000000 emailalert-1.2.1/emailalert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 01:12:21.737020 emailalert-1.2.1/sck/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.2.1/sck/__init__.py
+-rw-rw-rw-   0        0        0     3317 2023-06-20 01:11:58.000000 emailalert-1.2.1/sck/emailalert.py
+-rw-rw-rw-   0        0        0       42 2023-06-20 01:12:21.744097 emailalert-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      253 2023-06-20 00:15:33.000000 emailalert-1.2.1/setup.py
```

### Comparing `emailalert-1.2.0/README.md` & `emailalert-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `emailalert-1.2.0/sck/emailalert.py` & `emailalert-1.2.1/sck/emailalert.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     for folder_path in folder_paths:
         for root, dirs, files in os.walk(folder_path):
             for file_name in files:
                 file_names.append(file_name)
     return file_names
 
 
-def send(recipients,subject,message, folder_paths):
+def send(recipients,subject,message, folder_paths, backup_folders):
     # Email details
     smtp_server = 'mrelay.noc.sony.co.jp'
     smtp_port = 25
     sender = 'SCK-H5BAREVOS-NGK-SYSADMIN@sony.com'
 
     # Create a MIME text object
     #msg = MIMEText(message)
@@ -65,19 +65,19 @@
         encoders.encode_base64(attachment)
         attachment.add_header(
             "Content-Disposition",
             f"attachment; filename= {os.path.basename(file_path)}",
         )
         msg.attach(attachment)
         # Move the attached file to the backup folder
-        backup_folder = "LDD_in/error/backup/"
+        backup_folder = backup_folders[0]
         if 'Tokyo' in file_path:
-            backup_folder = "Tokyo_in/error/backup/"  # Relative path to the backup folder
+            backup_folder = backup_folders[1]  # Relative path to the backup folder
         elif 'MCO' in file_path:
-            backup_folder = "MCO_in/error/backup/"  # Relative path to the backup folder
+            backup_folder = backup_folders[2]  # Relative path to the backup folder
         current_dir = os.getcwd()  # Get the current working directory
         backup_file_path = os.path.abspath(os.path.join(current_dir, backup_folder, os.path.basename(file_path)))
         shutil.move(file_path, backup_file_path)
 
     # Connect to the SMTP server
     with smtplib.SMTP(smtp_server, smtp_port) as server:
         try:
```

