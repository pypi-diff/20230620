# Comparing `tmp/emailalert-1.2.2.tar.gz` & `tmp/emailalert-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailalert-1.2.2.tar", last modified: Tue Jun 20 02:08:00 2023, max compression
+gzip compressed data, was "emailalert-1.2.3.tar", last modified: Tue Jun 20 02:14:46 2023, max compression
```

## Comparing `emailalert-1.2.2.tar` & `emailalert-1.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 02:08:00.353196 emailalert-1.2.2/
--rw-rw-rw-   0        0        0      178 2023-06-20 02:08:00.349806 emailalert-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 02:08:00.314375 emailalert-1.2.2/emailalert.egg-info/
--rw-rw-rw-   0        0        0      178 2023-06-20 02:08:00.000000 emailalert-1.2.2/emailalert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-06-20 02:08:00.000000 emailalert-1.2.2/emailalert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 02:08:00.000000 emailalert-1.2.2/emailalert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-06-20 02:08:00.000000 emailalert-1.2.2/emailalert.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-20 02:08:00.344810 emailalert-1.2.2/sck/
--rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.2.2/sck/__init__.py
--rw-rw-rw-   0        0        0     3744 2023-06-20 02:07:38.000000 emailalert-1.2.2/sck/emailalert.py
--rw-rw-rw-   0        0        0       42 2023-06-20 02:08:00.354225 emailalert-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      253 2023-06-20 02:07:56.000000 emailalert-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 02:14:46.523948 emailalert-1.2.3/
+-rw-rw-rw-   0        0        0      178 2023-06-20 02:14:46.522153 emailalert-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 02:14:46.485218 emailalert-1.2.3/emailalert.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-06-20 02:14:46.000000 emailalert-1.2.3/emailalert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-06-20 02:14:46.000000 emailalert-1.2.3/emailalert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 02:14:46.000000 emailalert-1.2.3/emailalert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-06-20 02:14:46.000000 emailalert-1.2.3/emailalert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 02:14:46.515087 emailalert-1.2.3/sck/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.2.3/sck/__init__.py
+-rw-rw-rw-   0        0        0     3742 2023-06-20 02:14:30.000000 emailalert-1.2.3/sck/emailalert.py
+-rw-rw-rw-   0        0        0       42 2023-06-20 02:14:46.526958 emailalert-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      253 2023-06-20 02:14:39.000000 emailalert-1.2.3/setup.py
```

### Comparing `emailalert-1.2.2/README.md` & `emailalert-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `emailalert-1.2.2/sck/emailalert.py` & `emailalert-1.2.3/sck/emailalert.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,20 +50,20 @@
     table_html = '<table>'
     table_html += '<tr><th>エラーファイル</th></tr>'
     for errorfile in attachment_file_names:
         table_html += f'<tr><td>{errorfile}</td></tr>'
     table_html += '</table>'
 
     # Create the email body as HTML
-    body_html = f'<html><body>{table_html}</body></html>'
+    message += f'<html><body>{table_html}</body></html>'
 
-    msg.attach(MIMEText(message, 'plain'))
+    #msg.attach(MIMEText(message, 'plain'))
 
     # Attach the email body
-    msg.attach(MIMEText(body_html, 'html'))
+    msg.attach(MIMEText(message, 'html'))
 
     # Find files with the specified extension in the folder
     # attachment_paths = []
     # sendEmail = 0
     # for file_name in os.listdir(folder_path):
     #     if file_name.endswith(file_extension):
     #         attachment_paths.append(os.path.join(folder_path, file_name))
```

