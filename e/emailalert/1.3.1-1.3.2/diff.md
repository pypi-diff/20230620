# Comparing `tmp/emailalert-1.3.1.tar.gz` & `tmp/emailalert-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailalert-1.3.1.tar", last modified: Tue Jun 20 07:50:48 2023, max compression
+gzip compressed data, was "emailalert-1.3.2.tar", last modified: Tue Jun 20 07:58:42 2023, max compression
```

## Comparing `emailalert-1.3.1.tar` & `emailalert-1.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 07:50:48.842582 emailalert-1.3.1/
--rw-rw-rw-   0        0        0      178 2023-06-20 07:50:48.839245 emailalert-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 07:50:48.811263 emailalert-1.3.1/emailalert.egg-info/
--rw-rw-rw-   0        0        0      178 2023-06-20 07:50:48.000000 emailalert-1.3.1/emailalert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-06-20 07:50:48.000000 emailalert-1.3.1/emailalert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 07:50:48.000000 emailalert-1.3.1/emailalert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-06-20 07:50:48.000000 emailalert-1.3.1/emailalert.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-20 07:50:48.833273 emailalert-1.3.1/sck/
--rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.3.1/sck/__init__.py
--rw-rw-rw-   0        0        0     3720 2023-06-20 07:50:35.000000 emailalert-1.3.1/sck/emailalert.py
--rw-rw-rw-   0        0        0       42 2023-06-20 07:50:48.843340 emailalert-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0      253 2023-06-20 07:50:44.000000 emailalert-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 07:58:42.873595 emailalert-1.3.2/
+-rw-rw-rw-   0        0        0      178 2023-06-20 07:58:42.870600 emailalert-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 07:58:42.840656 emailalert-1.3.2/emailalert.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-06-20 07:58:42.000000 emailalert-1.3.2/emailalert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-06-20 07:58:42.000000 emailalert-1.3.2/emailalert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 07:58:42.000000 emailalert-1.3.2/emailalert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-06-20 07:58:42.000000 emailalert-1.3.2/emailalert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 07:58:42.864591 emailalert-1.3.2/sck/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.3.2/sck/__init__.py
+-rw-rw-rw-   0        0        0     3870 2023-06-20 07:58:23.000000 emailalert-1.3.2/sck/emailalert.py
+-rw-rw-rw-   0        0        0       42 2023-06-20 07:58:42.874595 emailalert-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      253 2023-06-20 07:58:34.000000 emailalert-1.3.2/setup.py
```

### Comparing `emailalert-1.3.1/README.md` & `emailalert-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `emailalert-1.3.1/sck/emailalert.py` & `emailalert-1.3.2/sck/emailalert.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,15 +37,20 @@
     # Create the HTML table with CSS styles
     table_html = '''
     <style>
         table {
             border-collapse: collapse;
             width: 70%;
         }
-
+        table tr:nth-child(odd) td{
+           background:#d1ffd4;
+        }
+        table tr td:hover {
+           background:#f7f091;
+        }
         th, td {
             border: 1px solid black;
             padding: 8px;
             width: 300px;
             text-align: left;
         }
```

