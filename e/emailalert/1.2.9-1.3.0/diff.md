# Comparing `tmp/emailalert-1.2.9.tar.gz` & `tmp/emailalert-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailalert-1.2.9.tar", last modified: Tue Jun 20 07:32:58 2023, max compression
+gzip compressed data, was "emailalert-1.3.0.tar", last modified: Tue Jun 20 07:35:18 2023, max compression
```

## Comparing `emailalert-1.2.9.tar` & `emailalert-1.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 07:32:58.270278 emailalert-1.2.9/
--rw-rw-rw-   0        0        0      178 2023-06-20 07:32:58.265267 emailalert-1.2.9/PKG-INFO
--rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.2.9/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 07:32:58.192102 emailalert-1.2.9/emailalert.egg-info/
--rw-rw-rw-   0        0        0      178 2023-06-20 07:32:57.000000 emailalert-1.2.9/emailalert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-06-20 07:32:57.000000 emailalert-1.2.9/emailalert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 07:32:57.000000 emailalert-1.2.9/emailalert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-06-20 07:32:57.000000 emailalert-1.2.9/emailalert.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-20 07:32:58.257424 emailalert-1.2.9/sck/
--rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.2.9/sck/__init__.py
--rw-rw-rw-   0        0        0     3757 2023-06-20 07:32:51.000000 emailalert-1.2.9/sck/emailalert.py
--rw-rw-rw-   0        0        0       42 2023-06-20 07:32:58.272428 emailalert-1.2.9/setup.cfg
--rw-rw-rw-   0        0        0      253 2023-06-20 07:30:53.000000 emailalert-1.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 07:35:18.924300 emailalert-1.3.0/
+-rw-rw-rw-   0        0        0      178 2023-06-20 07:35:18.922423 emailalert-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 07:35:18.877526 emailalert-1.3.0/emailalert.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-06-20 07:35:18.000000 emailalert-1.3.0/emailalert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-06-20 07:35:18.000000 emailalert-1.3.0/emailalert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 07:35:18.000000 emailalert-1.3.0/emailalert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-06-20 07:35:18.000000 emailalert-1.3.0/emailalert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 07:35:18.916306 emailalert-1.3.0/sck/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.3.0/sck/__init__.py
+-rw-rw-rw-   0        0        0     3697 2023-06-20 07:35:04.000000 emailalert-1.3.0/sck/emailalert.py
+-rw-rw-rw-   0        0        0       42 2023-06-20 07:35:18.925307 emailalert-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      253 2023-06-20 07:35:14.000000 emailalert-1.3.0/setup.py
```

### Comparing `emailalert-1.2.9/README.md` & `emailalert-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `emailalert-1.2.9/sck/emailalert.py` & `emailalert-1.3.0/sck/emailalert.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,26 +52,25 @@
         th {
             background-color: #f2f2f2;
         }
     </style>
 
     <table>
         <tr>
-            <th>ＮＯ</th>
             <th>エラーファイル</th>
         </tr>
     '''
     i = 1
     for file_name, file_path in zip(attachment_filename, attachment_paths):
         # spec = 'LDD'
         # if 'Tokyo' in file_path:
         #     spec = 'Tokyo'
         # elif 'MCO' in file_path:
         #     spec = 'MCO'
-        table_html += f'<tr><td style="width:50px">{i}</td><td>{file_name}</td></tr>'
+        table_html += f'<tr><td>{file_name}</td></tr>'
         i =i+1
         
 
     table_html += '</table>'
 
     # Create the email body as HTML
     message = message_header
```

