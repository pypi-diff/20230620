# Comparing `tmp/emailalert-1.3.6.tar.gz` & `tmp/emailalert-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailalert-1.3.6.tar", last modified: Tue Jun 20 08:19:42 2023, max compression
+gzip compressed data, was "emailalert-1.3.7.tar", last modified: Tue Jun 20 08:24:43 2023, max compression
```

## Comparing `emailalert-1.3.6.tar` & `emailalert-1.3.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 08:19:42.690249 emailalert-1.3.6/
--rw-rw-rw-   0        0        0      178 2023-06-20 08:19:42.687825 emailalert-1.3.6/PKG-INFO
--rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.3.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 08:19:42.657799 emailalert-1.3.6/emailalert.egg-info/
--rw-rw-rw-   0        0        0      178 2023-06-20 08:19:42.000000 emailalert-1.3.6/emailalert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-06-20 08:19:42.000000 emailalert-1.3.6/emailalert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 08:19:42.000000 emailalert-1.3.6/emailalert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-06-20 08:19:42.000000 emailalert-1.3.6/emailalert.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-20 08:19:42.683820 emailalert-1.3.6/sck/
--rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.3.6/sck/__init__.py
--rw-rw-rw-   0        0        0     4046 2023-06-20 08:19:23.000000 emailalert-1.3.6/sck/emailalert.py
--rw-rw-rw-   0        0        0       42 2023-06-20 08:19:42.691460 emailalert-1.3.6/setup.cfg
--rw-rw-rw-   0        0        0      253 2023-06-20 08:19:32.000000 emailalert-1.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:24:43.234244 emailalert-1.3.7/
+-rw-rw-rw-   0        0        0      178 2023-06-20 08:24:43.231881 emailalert-1.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.3.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 08:24:43.205946 emailalert-1.3.7/emailalert.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-06-20 08:24:43.000000 emailalert-1.3.7/emailalert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-06-20 08:24:43.000000 emailalert-1.3.7/emailalert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 08:24:43.000000 emailalert-1.3.7/emailalert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-06-20 08:24:43.000000 emailalert-1.3.7/emailalert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 08:24:43.228881 emailalert-1.3.7/sck/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.3.7/sck/__init__.py
+-rw-rw-rw-   0        0        0     4112 2023-06-20 08:24:03.000000 emailalert-1.3.7/sck/emailalert.py
+-rw-rw-rw-   0        0        0       42 2023-06-20 08:24:43.234845 emailalert-1.3.7/setup.cfg
+-rw-rw-rw-   0        0        0      253 2023-06-20 08:24:38.000000 emailalert-1.3.7/setup.py
```

### Comparing `emailalert-1.3.6/README.md` & `emailalert-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `emailalert-1.3.6/sck/emailalert.py` & `emailalert-1.3.7/sck/emailalert.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,26 +53,27 @@
         table tr:hover {
             background-color: #e6e6e6 !important;
         }
     </style>
 
     <table>
         <tr>
-            <th>仕様</th>
-            <th>エラーファイル</th>
+            <th>データ仕様</th>
+            <th>エラー発生ファイル</th>
         </tr>
     '''
     for index, (file_name, file_path) in enumerate(zip(attachment_filename, attachment_paths)):
         spec = 'MCO'
         if 'VHS' in file_path:
             spec = 'LDD'
         elif 'TT' in file_path:
             spec = 'Tokyo'
         row_color = "#d1ffd4" if index % 2 != 0 else "#ffffff"
-        table_html += f'<tr style="background-color: {row_color};" onmouseover="this.style.backgroundColor=\'#e6e6e6\';" onmouseout="this.style.backgroundColor=\'{row_color}\';"><td style="width:50px">{spec}</td><td>{file_name}</td></tr>'
+        table_html += f'<tr style="background-color: {row_color};" onmouseover="this.style.backgroundColor=\'#e6e6e6\';" onmouseout="this.style.backgroundColor=\'{row_color}\';">'
+        table_html += '<td style="width:50px">{spec}</td><td style="font-weight:bold">{file_name}</td></tr>'
         
 
     table_html += '</table>'
 
     # Create the email body as HTML
     message = message_header
     message += f'<html><body>{table_html}</body></html>'
```

