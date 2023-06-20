# Comparing `tmp/addon_tvg-karjakak-0.2.3rc2.tar.gz` & `tmp/addon_tvg-karjakak-0.2.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "addon_tvg-karjakak-0.2.3rc2.tar", last modified: Fri Nov  4 08:24:06 2022, max compression
+gzip compressed data, was "addon_tvg-karjakak-0.2.4rc1.tar", last modified: Tue Jun 20 05:05:11 2023, max compression
```

## Comparing `addon_tvg-karjakak-0.2.3rc2.tar` & `addon_tvg-karjakak-0.2.4rc1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2022-11-04 08:24:06.879452 addon_tvg-karjakak-0.2.3rc2/
--rw-r--r--   0 karja      (501) staff       (20)      671 2022-11-04 08:24:06.879602 addon_tvg-karjakak-0.2.3rc2/PKG-INFO
--rw-r--r--   0 karja      (501) staff       (20)       93 2022-10-04 05:50:24.000000 addon_tvg-karjakak-0.2.3rc2/README.md
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2022-11-04 08:24:06.878263 addon_tvg-karjakak-0.2.3rc2/addon_tvg/
--rw-r--r--   0 karja      (501) staff       (20)       86 2022-09-29 01:04:47.000000 addon_tvg-karjakak-0.2.3rc2/addon_tvg/__init__.py
--rw-r--r--   0 karja      (501) staff       (20)     1326 2022-11-02 14:40:03.000000 addon_tvg-karjakak-0.2.3rc2/addon_tvg/evalexpress.py
--rw-r--r--   0 karja      (501) staff       (20)     2840 2022-11-04 04:23:47.000000 addon_tvg-karjakak-0.2.3rc2/addon_tvg/grapp.py
--rw-r--r--   0 karja      (501) staff       (20)     5520 2022-11-02 14:42:32.000000 addon_tvg-karjakak-0.2.3rc2/addon_tvg/sumall.py
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2022-11-04 08:24:06.879303 addon_tvg-karjakak-0.2.3rc2/addon_tvg_karjakak.egg-info/
--rw-r--r--   0 karja      (501) staff       (20)      671 2022-11-04 08:24:06.000000 addon_tvg-karjakak-0.2.3rc2/addon_tvg_karjakak.egg-info/PKG-INFO
--rw-r--r--   0 karja      (501) staff       (20)      329 2022-11-04 08:24:06.000000 addon_tvg-karjakak-0.2.3rc2/addon_tvg_karjakak.egg-info/SOURCES.txt
--rw-r--r--   0 karja      (501) staff       (20)        1 2022-11-04 08:24:06.000000 addon_tvg-karjakak-0.2.3rc2/addon_tvg_karjakak.egg-info/dependency_links.txt
--rw-r--r--   0 karja      (501) staff       (20)       43 2022-11-04 08:24:06.000000 addon_tvg-karjakak-0.2.3rc2/addon_tvg_karjakak.egg-info/requires.txt
--rw-r--r--   0 karja      (501) staff       (20)       10 2022-11-04 08:24:06.000000 addon_tvg-karjakak-0.2.3rc2/addon_tvg_karjakak.egg-info/top_level.txt
--rw-r--r--   0 karja      (501) staff       (20)      103 2022-09-29 00:17:13.000000 addon_tvg-karjakak-0.2.3rc2/pyproject.toml
--rw-r--r--   0 karja      (501) staff       (20)      694 2022-11-04 08:24:06.879932 addon_tvg-karjakak-0.2.3rc2/setup.cfg
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-06-20 05:05:11.197638 addon_tvg-karjakak-0.2.4rc1/
+-rw-r--r--   0 karja      (501) staff       (20)      671 2023-06-20 05:05:11.197705 addon_tvg-karjakak-0.2.4rc1/PKG-INFO
+-rw-r--r--   0 karja      (501) staff       (20)       93 2022-10-04 05:50:24.000000 addon_tvg-karjakak-0.2.4rc1/README.md
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-06-20 05:05:11.196667 addon_tvg-karjakak-0.2.4rc1/addon_tvg/
+-rw-r--r--   0 karja      (501) staff       (20)       86 2022-09-29 01:04:47.000000 addon_tvg-karjakak-0.2.4rc1/addon_tvg/__init__.py
+-rw-r--r--   0 karja      (501) staff       (20)     1326 2022-11-02 14:40:03.000000 addon_tvg-karjakak-0.2.4rc1/addon_tvg/evalexpress.py
+-rw-r--r--   0 karja      (501) staff       (20)     2840 2022-11-04 04:23:47.000000 addon_tvg-karjakak-0.2.4rc1/addon_tvg/grapp.py
+-rw-r--r--   0 karja      (501) staff       (20)     5597 2023-06-20 05:02:20.000000 addon_tvg-karjakak-0.2.4rc1/addon_tvg/sumall.py
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-06-20 05:05:11.197528 addon_tvg-karjakak-0.2.4rc1/addon_tvg_karjakak.egg-info/
+-rw-r--r--   0 karja      (501) staff       (20)      671 2023-06-20 05:05:11.000000 addon_tvg-karjakak-0.2.4rc1/addon_tvg_karjakak.egg-info/PKG-INFO
+-rw-r--r--   0 karja      (501) staff       (20)      329 2023-06-20 05:05:11.000000 addon_tvg-karjakak-0.2.4rc1/addon_tvg_karjakak.egg-info/SOURCES.txt
+-rw-r--r--   0 karja      (501) staff       (20)        1 2023-06-20 05:05:11.000000 addon_tvg-karjakak-0.2.4rc1/addon_tvg_karjakak.egg-info/dependency_links.txt
+-rw-r--r--   0 karja      (501) staff       (20)       43 2023-06-20 05:05:11.000000 addon_tvg-karjakak-0.2.4rc1/addon_tvg_karjakak.egg-info/requires.txt
+-rw-r--r--   0 karja      (501) staff       (20)       10 2023-06-20 05:05:11.000000 addon_tvg-karjakak-0.2.4rc1/addon_tvg_karjakak.egg-info/top_level.txt
+-rw-r--r--   0 karja      (501) staff       (20)      103 2022-09-29 00:17:13.000000 addon_tvg-karjakak-0.2.4rc1/pyproject.toml
+-rw-r--r--   0 karja      (501) staff       (20)      694 2023-06-20 05:05:11.197954 addon_tvg-karjakak-0.2.4rc1/setup.cfg
```

### Comparing `addon_tvg-karjakak-0.2.3rc2/PKG-INFO` & `addon_tvg-karjakak-0.2.4rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: addon_tvg-karjakak
-Version: 0.2.3rc2
+Version: 0.2.4rc1
 Summary: Add on functions for TVG.
 Home-page: https://github.com/kakkarja/FreeTVG
 Author: karjakak
 Author-email: kakkarja.github@gmail.com
 License: BSD3 License
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
```

### Comparing `addon_tvg-karjakak-0.2.3rc2/addon_tvg/evalexpress.py` & `addon_tvg-karjakak-0.2.4rc1/addon_tvg/evalexpress.py`

 * *Files identical despite different names*

### Comparing `addon_tvg-karjakak-0.2.3rc2/addon_tvg/grapp.py` & `addon_tvg-karjakak-0.2.4rc1/addon_tvg/grapp.py`

 * *Files identical despite different names*

### Comparing `addon_tvg-karjakak-0.2.3rc2/addon_tvg/sumall.py` & `addon_tvg-karjakak-0.2.4rc1/addon_tvg/sumall.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
                 return str(pt.absolute())[:-4]
             case pt if os.path.exists(f"{pt.absolute()}.txt"):
                 return str(pt.absolute())
             case _:
                 return None
 
  
-    def getsums(self, dt: bool = True) -> dict:
+    def getsums(self, dt: bool = True, req = False) -> dict:
         """Sum-up every sub-node in the list"""
 
         lid = {}
         dgt = re.compile(r"\-?\d+\.?\d+")
         for id in self.getidx(dt):
             addnum = 0
             for i, t in islice(self.getdata(), id+1, None):
@@ -76,15 +76,18 @@
                     break
             else:
                 if i not in lid:
                     lid[i+1] = f"{addnum:,.2f}" if dt else addnum
         if dt: 
             return lid
         else:
-            return lid.values()
+            if not req:
+                return lid.values()
+            else:
+                return lid.keys()
 
     def getidx(self, dt: bool = True) -> list:
         """Getting the indicies of every node """
 
         idx = []
         for i, t in self.getdata():
             match (dt, t.startswith(self.sig), t.strip(" ").startswith("-TOTAL")):
@@ -167,8 +170,7 @@
 
     def chktot(self):
         """Check Total"""
 
         for _, d in self.getdata():
             if d.strip(" ").startswith("-TOTAL"):
                 return True
-
```

### Comparing `addon_tvg-karjakak-0.2.3rc2/addon_tvg_karjakak.egg-info/PKG-INFO` & `addon_tvg-karjakak-0.2.4rc1/addon_tvg_karjakak.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: addon-tvg-karjakak
-Version: 0.2.3rc2
+Version: 0.2.4rc1
 Summary: Add on functions for TVG.
 Home-page: https://github.com/kakkarja/FreeTVG
 Author: karjakak
 Author-email: kakkarja.github@gmail.com
 License: BSD3 License
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
```

### Comparing `addon_tvg-karjakak-0.2.3rc2/setup.cfg` & `addon_tvg-karjakak-0.2.4rc1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = addon_tvg-karjakak
-version = 0.2.3rc2
+version = 0.2.4rc1
 author = karjakak
 author_email = kakkarja.github@gmail.com
 description = Add on functions for TVG.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/kakkarja/FreeTVG
 license = BSD3 License
```

