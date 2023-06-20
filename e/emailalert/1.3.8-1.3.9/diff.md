# Comparing `tmp/emailalert-1.3.8.tar.gz` & `tmp/emailalert-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailalert-1.3.8.tar", last modified: Tue Jun 20 08:27:08 2023, max compression
+gzip compressed data, was "emailalert-1.3.9.tar", last modified: Tue Jun 20 08:36:04 2023, max compression
```

## Comparing `emailalert-1.3.8.tar` & `emailalert-1.3.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 08:27:07.998958 emailalert-1.3.8/
--rw-rw-rw-   0        0        0      178 2023-06-20 08:27:07.996059 emailalert-1.3.8/PKG-INFO
--rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.3.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 08:27:07.964947 emailalert-1.3.8/emailalert.egg-info/
--rw-rw-rw-   0        0        0      178 2023-06-20 08:27:07.000000 emailalert-1.3.8/emailalert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-06-20 08:27:07.000000 emailalert-1.3.8/emailalert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 08:27:07.000000 emailalert-1.3.8/emailalert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-06-20 08:27:07.000000 emailalert-1.3.8/emailalert.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-20 08:27:07.990208 emailalert-1.3.8/sck/
--rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.3.8/sck/__init__.py
--rw-rw-rw-   0        0        0     4113 2023-06-20 08:26:38.000000 emailalert-1.3.8/sck/emailalert.py
--rw-rw-rw-   0        0        0       42 2023-06-20 08:27:07.998958 emailalert-1.3.8/setup.cfg
--rw-rw-rw-   0        0        0      253 2023-06-20 08:26:57.000000 emailalert-1.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:36:04.862899 emailalert-1.3.9/
+-rw-rw-rw-   0        0        0      178 2023-06-20 08:36:04.860924 emailalert-1.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.3.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 08:36:04.848801 emailalert-1.3.9/emailalert.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-06-20 08:36:04.000000 emailalert-1.3.9/emailalert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-06-20 08:36:04.000000 emailalert-1.3.9/emailalert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 08:36:04.000000 emailalert-1.3.9/emailalert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-06-20 08:36:04.000000 emailalert-1.3.9/emailalert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 08:36:04.857814 emailalert-1.3.9/sck/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.3.9/sck/__init__.py
+-rw-rw-rw-   0        0        0     4130 2023-06-20 08:34:16.000000 emailalert-1.3.9/sck/emailalert.py
+-rw-rw-rw-   0        0        0       42 2023-06-20 08:36:04.863813 emailalert-1.3.9/setup.cfg
+-rw-rw-rw-   0        0        0      253 2023-06-20 08:35:41.000000 emailalert-1.3.9/setup.py
```

### Comparing `emailalert-1.3.8/README.md` & `emailalert-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `emailalert-1.3.8/sck/emailalert.py` & `emailalert-1.3.9/sck/emailalert.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         spec = 'MCO'
         if 'VHS' in file_path:
             spec = 'LDD'
         elif 'TT' in file_path:
             spec = 'Tokyo'
         row_color = "#d1ffd4" if index % 2 != 0 else "#ffffff"
         table_html += f'<tr style="background-color: {row_color};" onmouseover="this.style.backgroundColor=\'#e6e6e6\';" onmouseout="this.style.backgroundColor=\'{row_color}\';">'
-        table_html += f'<td style="width:50px">{spec}</td><td style="font-weight:bold">{file_name}</td></tr>'
+        table_html += f'<td style="width:30px;font-weight:bold">{spec}</td><td style="font-weight:bold">{file_name}</td></tr>'
         
 
     table_html += '</table>'
 
     # Create the email body as HTML
     message = message_header
     message += f'<html><body>{table_html}</body></html>'
```

