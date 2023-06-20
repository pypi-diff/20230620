# Comparing `tmp/emailalert-1.3.0.tar.gz` & `tmp/emailalert-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailalert-1.3.0.tar", last modified: Tue Jun 20 07:35:18 2023, max compression
+gzip compressed data, was "emailalert-1.3.1.tar", last modified: Tue Jun 20 07:50:48 2023, max compression
```

## Comparing `emailalert-1.3.0.tar` & `emailalert-1.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 07:35:18.924300 emailalert-1.3.0/
--rw-rw-rw-   0        0        0      178 2023-06-20 07:35:18.922423 emailalert-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 07:35:18.877526 emailalert-1.3.0/emailalert.egg-info/
--rw-rw-rw-   0        0        0      178 2023-06-20 07:35:18.000000 emailalert-1.3.0/emailalert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-06-20 07:35:18.000000 emailalert-1.3.0/emailalert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 07:35:18.000000 emailalert-1.3.0/emailalert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-06-20 07:35:18.000000 emailalert-1.3.0/emailalert.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-20 07:35:18.916306 emailalert-1.3.0/sck/
--rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.3.0/sck/__init__.py
--rw-rw-rw-   0        0        0     3697 2023-06-20 07:35:04.000000 emailalert-1.3.0/sck/emailalert.py
--rw-rw-rw-   0        0        0       42 2023-06-20 07:35:18.925307 emailalert-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0      253 2023-06-20 07:35:14.000000 emailalert-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 07:50:48.842582 emailalert-1.3.1/
+-rw-rw-rw-   0        0        0      178 2023-06-20 07:50:48.839245 emailalert-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 07:50:48.811263 emailalert-1.3.1/emailalert.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-06-20 07:50:48.000000 emailalert-1.3.1/emailalert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-06-20 07:50:48.000000 emailalert-1.3.1/emailalert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 07:50:48.000000 emailalert-1.3.1/emailalert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-06-20 07:50:48.000000 emailalert-1.3.1/emailalert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 07:50:48.833273 emailalert-1.3.1/sck/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.3.1/sck/__init__.py
+-rw-rw-rw-   0        0        0     3720 2023-06-20 07:50:35.000000 emailalert-1.3.1/sck/emailalert.py
+-rw-rw-rw-   0        0        0       42 2023-06-20 07:50:48.843340 emailalert-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      253 2023-06-20 07:50:44.000000 emailalert-1.3.1/setup.py
```

### Comparing `emailalert-1.3.0/README.md` & `emailalert-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `emailalert-1.3.0/sck/emailalert.py` & `emailalert-1.3.1/sck/emailalert.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,26 +52,25 @@
         th {
             background-color: #f2f2f2;
         }
     </style>
 
     <table>
         <tr>
+            <th>仕様</th>
             <th>エラーファイル</th>
         </tr>
     '''
-    i = 1
     for file_name, file_path in zip(attachment_filename, attachment_paths):
-        # spec = 'LDD'
-        # if 'Tokyo' in file_path:
-        #     spec = 'Tokyo'
-        # elif 'MCO' in file_path:
-        #     spec = 'MCO'
-        table_html += f'<tr><td>{file_name}</td></tr>'
-        i =i+1
+        spec = 'MCO'
+        if 'VHS' in file_path:
+            spec = 'LDD'
+        elif 'TT' in file_path:
+            spec = 'Tokyo'
+        table_html += f'<tr><td style="width:50px">{spec}</td><td>{file_name}</td></tr>'
         
 
     table_html += '</table>'
 
     # Create the email body as HTML
     message = message_header
     message += f'<html><body>{table_html}</body></html>'
```

