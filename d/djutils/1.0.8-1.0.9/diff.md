# Comparing `tmp/djutils-1.0.8.tar.gz` & `tmp/djutils-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\djutils-1.0.8.tar", last modified: Sun Mar 22 20:37:46 2020, max compression
+gzip compressed data, was "dist\djutils-1.0.9.tar", last modified: Wed Mar 25 16:16:07 2020, max compression
```

## Comparing `djutils-1.0.8.tar` & `djutils-1.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2020-03-22 20:37:46.000000 djutils-1.0.8/
--rw-rw-rw-   0        0        0     2035 2020-03-22 20:37:46.000000 djutils-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      982 2020-01-20 19:18:29.000000 djutils-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2020-03-22 20:37:46.000000 djutils-1.0.8/djutils/
--rw-rw-rw-   0        0        0       76 2020-01-20 19:17:29.000000 djutils-1.0.8/djutils/__init__.py
--rw-rw-rw-   0        0        0     2800 2019-12-07 19:41:30.000000 djutils-1.0.8/djutils/admin.py
--rw-rw-rw-   0        0        0      218 2019-12-25 22:46:52.000000 djutils-1.0.8/djutils/app_settings.py
--rw-rw-rw-   0        0        0     1056 2019-12-07 19:41:30.000000 djutils-1.0.8/djutils/crypt.py
--rw-rw-rw-   0        0        0      422 2019-12-07 19:41:30.000000 djutils-1.0.8/djutils/db.py
--rw-rw-rw-   0        0        0      813 2019-12-11 21:57:38.000000 djutils-1.0.8/djutils/exceptions.py
--rw-rw-rw-   0        0        0     2895 2019-12-29 21:54:08.000000 djutils-1.0.8/djutils/http.py
--rw-rw-rw-   0        0        0      632 2019-12-07 19:45:50.000000 djutils-1.0.8/djutils/ip.py
--rw-rw-rw-   0        0        0     1092 2019-12-07 19:41:30.000000 djutils-1.0.8/djutils/mail.py
--rw-rw-rw-   0        0        0      804 2020-01-20 20:43:19.000000 djutils-1.0.8/djutils/mixins.py
--rw-rw-rw-   0        0        0     4926 2020-03-22 20:37:16.000000 djutils-1.0.8/djutils/models.py
-drwxrwxrwx   0        0        0        0 2020-03-22 20:37:46.000000 djutils-1.0.8/djutils.egg-info/
--rw-rw-rw-   0        0        0     2035 2020-03-22 20:37:45.000000 djutils-1.0.8/djutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      378 2020-03-22 20:37:46.000000 djutils-1.0.8/djutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-03-22 20:37:45.000000 djutils-1.0.8/djutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2020-03-22 20:37:45.000000 djutils-1.0.8/djutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2020-03-22 20:37:45.000000 djutils-1.0.8/djutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      797 2020-03-22 20:37:46.000000 djutils-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0       41 2019-12-25 22:52:04.000000 djutils-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2020-03-25 16:16:07.000000 djutils-1.0.9/
+-rw-rw-rw-   0        0        0     2035 2020-03-25 16:16:07.000000 djutils-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      982 2020-01-20 19:18:29.000000 djutils-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2020-03-25 16:16:07.000000 djutils-1.0.9/djutils/
+-rw-rw-rw-   0        0        0       76 2020-01-20 19:17:29.000000 djutils-1.0.9/djutils/__init__.py
+-rw-rw-rw-   0        0        0     2800 2019-12-07 19:41:30.000000 djutils-1.0.9/djutils/admin.py
+-rw-rw-rw-   0        0        0      218 2019-12-25 22:46:52.000000 djutils-1.0.9/djutils/app_settings.py
+-rw-rw-rw-   0        0        0     1056 2019-12-07 19:41:30.000000 djutils-1.0.9/djutils/crypt.py
+-rw-rw-rw-   0        0        0      422 2019-12-07 19:41:30.000000 djutils-1.0.9/djutils/db.py
+-rw-rw-rw-   0        0        0      813 2019-12-11 21:57:38.000000 djutils-1.0.9/djutils/exceptions.py
+-rw-rw-rw-   0        0        0     2895 2019-12-29 21:54:08.000000 djutils-1.0.9/djutils/http.py
+-rw-rw-rw-   0        0        0      632 2019-12-07 19:45:50.000000 djutils-1.0.9/djutils/ip.py
+-rw-rw-rw-   0        0        0     1092 2019-12-07 19:41:30.000000 djutils-1.0.9/djutils/mail.py
+-rw-rw-rw-   0        0        0      804 2020-01-20 20:43:19.000000 djutils-1.0.9/djutils/mixins.py
+-rw-rw-rw-   0        0        0     6406 2020-03-25 16:15:54.000000 djutils-1.0.9/djutils/models.py
+drwxrwxrwx   0        0        0        0 2020-03-25 16:16:07.000000 djutils-1.0.9/djutils.egg-info/
+-rw-rw-rw-   0        0        0     2035 2020-03-25 16:16:07.000000 djutils-1.0.9/djutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2020-03-25 16:16:07.000000 djutils-1.0.9/djutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-03-25 16:16:07.000000 djutils-1.0.9/djutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2020-03-25 16:16:07.000000 djutils-1.0.9/djutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2020-03-25 16:16:07.000000 djutils-1.0.9/djutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      797 2020-03-25 16:16:07.000000 djutils-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0       41 2019-12-25 22:52:04.000000 djutils-1.0.9/setup.py
```

### Comparing `djutils-1.0.8/PKG-INFO` & `djutils-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djutils
-Version: 1.0.8
+Version: 1.0.9
 Summary: Utilities for use with the django web framework
 Home-page: https://git.voltane.eu/voltane/pypi/djutils
 Author: Manuel Stingl
 Author-email: opensource@voltane.eu
 License: GNU GPLv3
 Description: # djutils
         ## Tools for use within the django framework
```

### Comparing `djutils-1.0.8/README.md` & `djutils-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `djutils-1.0.8/djutils/admin.py` & `djutils-1.0.9/djutils/admin.py`

 * *Files identical despite different names*

### Comparing `djutils-1.0.8/djutils/crypt.py` & `djutils-1.0.9/djutils/crypt.py`

 * *Files identical despite different names*

### Comparing `djutils-1.0.8/djutils/exceptions.py` & `djutils-1.0.9/djutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `djutils-1.0.8/djutils/http.py` & `djutils-1.0.9/djutils/http.py`

 * *Files identical despite different names*

### Comparing `djutils-1.0.8/djutils/ip.py` & `djutils-1.0.9/djutils/ip.py`

 * *Files identical despite different names*

### Comparing `djutils-1.0.8/djutils/mail.py` & `djutils-1.0.9/djutils/mail.py`

 * *Files identical despite different names*

### Comparing `djutils-1.0.8/djutils/mixins.py` & `djutils-1.0.9/djutils/mixins.py`

 * *Files identical despite different names*

### Comparing `djutils-1.0.8/djutils/models.py` & `djutils-1.0.9/djutils/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         if stderr:
             raise IOError(stderr)
 
         return BytesIO(stdout)
 
 
 class AbstractImageStorage(FileSystemStorage):
-    def __init__(self, *args, resize_to: tuple = None, resample=Image.BICUBIC, output_format='png', just_hash=False, hash_algo=hashlib.sha256, post_process=None, **kwargs):
+    def __init__(self, *args, resize_to: tuple = None, resample=Image.BICUBIC, output_format='png', just_hash=False, hash_algo=hashlib.sha256, post_process=None, should_fix_colorspace=True, **kwargs):
         """
         Image Storage.
         Resamples an Image before storing as File.
 
         Params:
         resize_to: tuple, (width, height)
         resample: PIL.Image resampling metho
@@ -79,21 +79,57 @@
         super().__init__(*args, **kwargs)
         self.resize_to = resize_to
         self.resample = resample
         self.format = output_format
         self.just_hash = just_hash
         self.hash_algo = hash_algo
         self.post_process = post_process
+        self.should_fix_colorspace = should_fix_colorspace
 
     def process_picture(self, file):
         raise NotImplementedError
 
+    @classmethod
+    def _fix_colorspace(cls, image, colorspace, output_format):
+        """
+        From https://github.com/jazzband/sorl-thumbnail/issues/564
+        """
+        if colorspace == 'RGB':
+            # Pillow JPEG doesn't allow RGBA anymore. It was converted to RGB before.
+            if image.mode == 'RGBA' and output_format != 'JPEG':
+                return image  # RGBA is just RGB + Alpha
+
+            if image.mode == 'LA' or (image.mode == 'P' and 'transparency' in image.info):
+                if output_format == 'JPEG':
+                    newimage = Image.new('RGB', image.size, '#ffffff')
+                    mask = image.convert('RGBA').split()[-1]
+                    newimage.paste(image.convert('RGBA'), (0, 0), mask)
+
+                else:
+                    newimage = image.convert('RGBA')
+                    transparency = image.info.get('transparency')
+                    if transparency is not None:
+                        mask = image.convert('RGBA').split()[-1]
+                        newimage.putalpha(mask)
+
+                return newimage
+
+            return image.convert('RGB')
+
+        if colorspace == 'GRAY':
+            return image.convert('L')
+
+        return image
+
     def _save(self, name, content):
         file = BytesIO()
         content.image = self.process_picture(content.file)
+        if self.should_fix_colorspace:
+            content.image = self._fix_colorspace(content.image, "RGB", self.format.upper())
+
         content.image.save(file, format=self.format)
 
         if self.post_process:
             file = self.post_process(file)
 
         hash_name = self.hash_algo(file.read()).hexdigest()
         content.file.seek(0)
```

### Comparing `djutils-1.0.8/djutils.egg-info/PKG-INFO` & `djutils-1.0.9/djutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djutils
-Version: 1.0.8
+Version: 1.0.9
 Summary: Utilities for use with the django web framework
 Home-page: https://git.voltane.eu/voltane/pypi/djutils
 Author: Manuel Stingl
 Author-email: opensource@voltane.eu
 License: GNU GPLv3
 Description: # djutils
         ## Tools for use within the django framework
```

