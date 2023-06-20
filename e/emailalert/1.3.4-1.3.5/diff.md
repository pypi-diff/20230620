# Comparing `tmp/emailalert-1.3.4.tar.gz` & `tmp/emailalert-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailalert-1.3.4.tar", last modified: Tue Jun 20 08:11:03 2023, max compression
+gzip compressed data, was "emailalert-1.3.5.tar", last modified: Tue Jun 20 08:16:30 2023, max compression
```

## Comparing `emailalert-1.3.4.tar` & `emailalert-1.3.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 08:11:03.405285 emailalert-1.3.4/
--rw-rw-rw-   0        0        0      178 2023-06-20 08:11:03.402790 emailalert-1.3.4/PKG-INFO
--rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.3.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 08:11:03.369311 emailalert-1.3.4/emailalert.egg-info/
--rw-rw-rw-   0        0        0      178 2023-06-20 08:11:03.000000 emailalert-1.3.4/emailalert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-06-20 08:11:03.000000 emailalert-1.3.4/emailalert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 08:11:03.000000 emailalert-1.3.4/emailalert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-06-20 08:11:03.000000 emailalert-1.3.4/emailalert.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-20 08:11:03.395274 emailalert-1.3.4/sck/
--rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.3.4/sck/__init__.py
--rw-rw-rw-   0        0        0     3953 2023-06-20 08:10:45.000000 emailalert-1.3.4/sck/emailalert.py
--rw-rw-rw-   0        0        0       42 2023-06-20 08:11:03.406280 emailalert-1.3.4/setup.cfg
--rw-rw-rw-   0        0        0      253 2023-06-20 08:10:52.000000 emailalert-1.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:16:30.878393 emailalert-1.3.5/
+-rw-rw-rw-   0        0        0      178 2023-06-20 08:16:30.875378 emailalert-1.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.3.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 08:16:30.851537 emailalert-1.3.5/emailalert.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-06-20 08:16:30.000000 emailalert-1.3.5/emailalert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-06-20 08:16:30.000000 emailalert-1.3.5/emailalert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 08:16:30.000000 emailalert-1.3.5/emailalert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-06-20 08:16:30.000000 emailalert-1.3.5/emailalert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 08:16:30.871411 emailalert-1.3.5/sck/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.3.5/sck/__init__.py
+-rw-rw-rw-   0        0        0     3958 2023-06-20 08:16:27.000000 emailalert-1.3.5/sck/emailalert.py
+-rw-rw-rw-   0        0        0       42 2023-06-20 08:16:30.879386 emailalert-1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      253 2023-06-20 08:12:24.000000 emailalert-1.3.5/setup.py
```

### Comparing `emailalert-1.3.4/README.md` & `emailalert-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `emailalert-1.3.4/sck/emailalert.py` & `emailalert-1.3.5/sck/emailalert.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,16 +60,16 @@
     '''
     for index, (file_name, file_path) in enumerate(zip(attachment_filename, attachment_paths)):
         spec = 'MCO'
         if 'VHS' in file_path:
             spec = 'LDD'
         elif 'TT' in file_path:
             spec = 'Tokyo'
-        row_color = "#d1ffd4" if index == 0 else "#ffffff"
-        table_html += f'<tr style="background-color: {row_color}" onmouseover="this.style.backgroundColor=\'#e6e6e6\';" onmouseout="this.style.backgroundColor=\'{row_color}\';"><td style="width:50px">{spec}</td><td>{file_name}</td></tr>'
+        row_color = "#d1ffd4" if index % 2 == 0 else "#ffffff"
+        table_html += f'<tr style="background-color: {row_color};" onmouseover="this.style.backgroundColor=\'#e6e6e6\';" onmouseout="this.style.backgroundColor=\'{row_color}\';"><td style="width:50px">{spec}</td><td>{file_name}</td></tr>'
         
 
     table_html += '</table>'
 
     # Create the email body as HTML
     message = message_header
     message += f'<html><body>{table_html}</body></html>'
```

