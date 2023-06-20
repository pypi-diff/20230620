# Comparing `tmp/ParUtils-1.1.8-py3-none-any.whl.zip` & `tmp/ParUtils-1.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,25 @@
-Zip file size: 16518 bytes, number of entries: 22
--rw-rw-rw-  2.0 fat     1415 b- defN 23-Jun-07 07:01 parutils/__init__.py
--rw-rw-rw-  2.0 fat     1258 b- defN 23-Jun-07 07:03 parutils/changelog.py
+Zip file size: 16715 bytes, number of entries: 23
+-rw-rw-rw-  2.0 fat     1434 b- defN 23-Jun-20 13:56 parutils/__init__.py
+-rw-rw-rw-  2.0 fat     1347 b- defN 23-Jun-20 14:06 parutils/changelog.py
 -rw-rw-rw-  2.0 fat     2874 b- defN 23-Jun-07 06:35 parutils/csvl.py
 -rw-rw-rw-  2.0 fat     2302 b- defN 22-Sep-22 06:06 parutils/dq.py
 -rw-rw-rw-  2.0 fat     2881 b- defN 23-Jun-07 06:35 parutils/file.py
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-20 13:55 parutils/g.py
 -rw-rw-rw-  2.0 fat      745 b- defN 23-Jun-07 06:35 parutils/msc.py
 -rw-rw-rw-  2.0 fat     5563 b- defN 23-Jun-07 07:00 parutils/strg.py
 -rw-rw-rw-  2.0 fat      610 b- defN 22-Dec-13 06:12 parutils/testing.py
 -rw-rw-rw-  2.0 fat      421 b- defN 22-Sep-21 17:28 parutils/wrap.py
 -rw-rw-rw-  2.0 fat      461 b- defN 23-Jun-07 06:35 parutils/logging/__init__.py
--rw-rw-rw-  2.0 fat     2027 b- defN 23-Jun-07 06:35 parutils/logging/cl.py
+-rw-rw-rw-  2.0 fat     2079 b- defN 23-Jun-15 05:52 parutils/logging/cl.py
 -rw-rw-rw-  2.0 fat      115 b- defN 22-Sep-21 17:28 parutils/logging/const.py
 -rw-rw-rw-  2.0 fat      843 b- defN 23-Jun-07 06:35 parutils/logging/core.py
--rw-rw-rw-  2.0 fat       47 b- defN 23-Jun-07 06:35 parutils/logging/g.py
--rw-rw-rw-  2.0 fat     2879 b- defN 23-Jun-07 06:35 parutils/logging/logger.py
+-rw-rw-rw-  2.0 fat       47 b- defN 23-Jun-20 13:56 parutils/logging/g.py
+-rw-rw-rw-  2.0 fat     2907 b- defN 23-Jun-20 13:56 parutils/logging/logger.py
 -rw-rw-rw-  2.0 fat     1908 b- defN 23-Mar-23 08:21 parutils/logging/main.py
 -rw-rw-rw-  2.0 fat     1164 b- defN 22-Dec-13 06:13 parutils/logging/sl.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-07 07:04 ParUtils-1.1.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     5175 b- defN 23-Jun-07 07:04 ParUtils-1.1.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-07 07:04 ParUtils-1.1.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-07 07:04 ParUtils-1.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1696 b- defN 23-Jun-07 07:04 ParUtils-1.1.8.dist-info/RECORD
-22 files, 35576 bytes uncompressed, 13806 bytes compressed:  61.2%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-20 14:08 ParUtils-1.1.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     5175 b- defN 23-Jun-20 14:08 ParUtils-1.1.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-20 14:08 ParUtils-1.1.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-20 14:08 ParUtils-1.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1764 b- defN 23-Jun-20 14:08 ParUtils-1.1.9.dist-info/RECORD
+23 files, 35843 bytes uncompressed, 13901 bytes compressed:  61.2%
```

## zipnote {}

```diff
@@ -9,14 +9,17 @@
 
 Filename: parutils/dq.py
 Comment: 
 
 Filename: parutils/file.py
 Comment: 
 
+Filename: parutils/g.py
+Comment: 
+
 Filename: parutils/msc.py
 Comment: 
 
 Filename: parutils/strg.py
 Comment: 
 
 Filename: parutils/testing.py
@@ -45,23 +48,23 @@
 
 Filename: parutils/logging/main.py
 Comment: 
 
 Filename: parutils/logging/sl.py
 Comment: 
 
-Filename: ParUtils-1.1.8.dist-info/LICENSE
+Filename: ParUtils-1.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: ParUtils-1.1.8.dist-info/METADATA
+Filename: ParUtils-1.1.9.dist-info/METADATA
 Comment: 
 
-Filename: ParUtils-1.1.8.dist-info/WHEEL
+Filename: ParUtils-1.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: ParUtils-1.1.8.dist-info/top_level.txt
+Filename: ParUtils-1.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: ParUtils-1.1.8.dist-info/RECORD
+Filename: ParUtils-1.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## parutils/__init__.py

```diff
@@ -1,9 +1,11 @@
 from .changelog import __VERSION__
 
+from . import g
+
 from .logging import log
 from .logging import Logger
 from .logging import log_dict
 from .logging import step_log
 from .logging import get_logs
 from .logging import log_print
 from .logging import log_array
```

## parutils/changelog.py

```diff
@@ -1,10 +1,14 @@
-__VERSION__ = '1.1.8'
-# check_log - in_list optional
-# strg - truncate
+__VERSION__ = '1.1.9'
+# check_log - name appears when check_log ok
+# u.g.logs
+
+# __VERSION__ = '1.1.8'
+# # check_log - in_list optional
+# # strg - truncate
 
 # __VERSION__ = '1.1.7'
 # # log_array - char_tab arg
 # # check_log - name arg
 
 # __VERSION__ = '1.1.6'
 # # exact arg for like, like_list and like_dict
```

## parutils/logging/cl.py

```diff
@@ -19,15 +19,15 @@
     logger = get_logger()
     txt = load_txt(logger)
 
     n_w = 0
     n_w += check(in_list, txt, logger.log_path, log_matches)
     n_w += check_not(in_list_not, txt, logger.log_path)
 
-    check_warn(n_w, max_warn)
+    check_warn(n_w, max_warn, name)
 
 
 def load_txt(logger: Logger):
     if not hasattr(logger, 'log_path'):
         s = 'No log file has been initialised. Initialise a log file by instanciating a logger object with Logger().'
         raise Exception(s)
     txt = u.load_txt(logger.log_path, False)
@@ -56,16 +56,17 @@
             n_w += 1
             s = f"Expression '{elt}' was found in log file {log_path}"
             log(s, c_out=False)
             warnings.warn(s)
     return n_w
 
 
-def check_warn(n_w, max_warn):
+def check_warn(n_w, max_warn, name):
+    s = f' {name}' if name else ''
     if n_w == 0:
-        log('check_log ok')
+        log(f'check_log{s} ok')
     elif n_w <= max_warn:
         log(f'check_log ended with {n_w} warnings')
     else:
         s = f'check_log ko, too many warnings ({n_w} warnings)'
         log(s)
         raise Exception(s)
```

## parutils/logging/logger.py

```diff
@@ -86,12 +86,13 @@
         with lock:
             if c_out:
                 print(s)
             self._write_log(s)
 
     def _write_log(self, str_in):
         s = str(str_in)
+        u.g.logs.append(s)
         self.logs.append(s)
         if not self.file_write:
             return
         with open(self.log_path, 'a', encoding='utf-8') as in_file:
             in_file.write(s + '\n')
```

## Comparing `ParUtils-1.1.8.dist-info/LICENSE` & `ParUtils-1.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ParUtils-1.1.8.dist-info/METADATA` & `ParUtils-1.1.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ParUtils
-Version: 1.1.8
+Version: 1.1.9
 Summary: This package contains a bunch of Python utils developed for Support, Test and Automation IT Engineers
 Home-page: https://github.com/paularnaud2/ParUtils
 Author: Paul ARNAUD
 Author-email: paularnaud2@gmail.com
 Project-URL: Bug Tracker, https://github.com/paularnaud2/ParUtils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `ParUtils-1.1.8.dist-info/RECORD` & `ParUtils-1.1.9.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-parutils/__init__.py,sha256=YoCYntQVfZD-1K1yQeMejwfT-2tYp9MF0qoUwqGkzt4,1415
-parutils/changelog.py,sha256=XDw6kHW409tE3iL_LtrTAw0VYQMAXBR0YASkZ2MdLCs,1258
+parutils/__init__.py,sha256=EaFtUmU0kYgnjvAFwPmoKt7I5zn9bxY02R7TUtcE6M4,1434
+parutils/changelog.py,sha256=cDppejgTUKwpHW9xL5NJX-J91hJnyZKQScbY9vVeZlU,1347
 parutils/csvl.py,sha256=UBqw0lyhTNqFLSNIE-JM7TAQYCRgHftYQmHi21ru8-A,2874
 parutils/dq.py,sha256=kdvzOo5FLCumXagY05kGSseYlbR-zvjjmsMtGVliVc8,2302
 parutils/file.py,sha256=-OPfMhTjHDqubZLWJquY-FOv3W_k9GWoMq_rNgtdU9Y,2881
+parutils/g.py,sha256=n99gQbLs2rmszBYw_wy43P4iQo3lqpBHz3-Q7sm9n_U,11
 parutils/msc.py,sha256=0hf-WrYhDquaDtfHXINNs9tROwJ7iYV2J6y0umkaGRA,745
 parutils/strg.py,sha256=_8NQJ1iY58Z_xACTDVcyonvRHDRuy9Ai3Kv3CvVXRh4,5563
 parutils/testing.py,sha256=kXrMz8Kze4mZejaePmV_OIca4iuNcG_dhGVHCgVuF-k,610
 parutils/wrap.py,sha256=PqMyKodgEjWDXoIVZZXRaBSdkGFL5OWmVJttl2Crrg8,421
 parutils/logging/__init__.py,sha256=rSNpgjuYer-Hhn6zKzKwKSn_KfcajEXlk6cJnPC9eJU,461
-parutils/logging/cl.py,sha256=jhQyCpWT-qwW0ictD6KGAu3K1mXACBUmyxE3F5YGbpA,2027
+parutils/logging/cl.py,sha256=L40SkNdrdAT-7hfXAcFPHdB73PVqAhKVlMGC7Awtx1w,2079
 parutils/logging/const.py,sha256=YvIi9AROVeQHLS0hFrL96dWjW6jh4DO9r_ghZ4G-adA,115
 parutils/logging/core.py,sha256=vBwZnpM2GRNSSABPdzEM9SRpqr_YNqdPlG3T3lNPSiY,843
 parutils/logging/g.py,sha256=ZSrgZw63kwxIW66A7-9_iYeDt4AstNZ_XXQgK8MglyQ,47
-parutils/logging/logger.py,sha256=TcBRTiDPToxrMAI82sdLs8Lif8Oy9IgWooJy-jW43iE,2879
+parutils/logging/logger.py,sha256=bBExUDHcqbaL4-7XktyAcJg5Pr0Bt52rLOpRYfiZqGA,2907
 parutils/logging/main.py,sha256=Z-ooY43PUk36nwVB_D9c9ZF7HUGngrFyVS8yBUVsTXA,1908
 parutils/logging/sl.py,sha256=3-sj_o33cZmOqeFxlTl5HyHOvSAhn9glYcc-BmTUpZc,1164
-ParUtils-1.1.8.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-ParUtils-1.1.8.dist-info/METADATA,sha256=63JjyC2P27ZiyZbvVaXjaeAg80R0PVtNfN6sjsP39ko,5175
-ParUtils-1.1.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-ParUtils-1.1.8.dist-info/top_level.txt,sha256=1MDobUcroeYEvdupZCAFvA5hJjm7LSDUV5A4jHySNis,9
-ParUtils-1.1.8.dist-info/RECORD,,
+ParUtils-1.1.9.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+ParUtils-1.1.9.dist-info/METADATA,sha256=wHEdosiDfPzz7PzwJB4LyTqQF8KiqkPbikZBsvmU4RI,5175
+ParUtils-1.1.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+ParUtils-1.1.9.dist-info/top_level.txt,sha256=1MDobUcroeYEvdupZCAFvA5hJjm7LSDUV5A4jHySNis,9
+ParUtils-1.1.9.dist-info/RECORD,,
```

