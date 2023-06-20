# Comparing `tmp/PlexLabExchange-0.8.4.tar.gz` & `tmp/PlexLabExchange-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlexLabExchange-0.8.4.tar", last modified: Tue Jun 20 19:04:51 2023, max compression
+gzip compressed data, was "PlexLabExchange-0.8.5.tar", last modified: Tue Jun 20 19:12:36 2023, max compression
```

## Comparing `PlexLabExchange-0.8.4.tar` & `PlexLabExchange-0.8.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 mcmenemy   (501) staff       (20)        0 2023-06-20 19:04:51.772650 PlexLabExchange-0.8.4/
--rw-r--r--   0 mcmenemy   (501) staff       (20)      603 2023-06-20 19:04:51.772508 PlexLabExchange-0.8.4/PKG-INFO
-drwxr-xr-x   0 mcmenemy   (501) staff       (20)        0 2023-06-20 19:04:51.772329 PlexLabExchange-0.8.4/PlexLabExchange.egg-info/
--rw-r--r--   0 mcmenemy   (501) staff       (20)      603 2023-06-20 19:04:51.000000 PlexLabExchange-0.8.4/PlexLabExchange.egg-info/PKG-INFO
--rw-r--r--   0 mcmenemy   (501) staff       (20)      174 2023-06-20 19:04:51.000000 PlexLabExchange-0.8.4/PlexLabExchange.egg-info/SOURCES.txt
--rw-r--r--   0 mcmenemy   (501) staff       (20)        1 2023-06-20 19:04:51.000000 PlexLabExchange-0.8.4/PlexLabExchange.egg-info/dependency_links.txt
--rw-r--r--   0 mcmenemy   (501) staff       (20)        1 2023-06-20 19:04:51.000000 PlexLabExchange-0.8.4/PlexLabExchange.egg-info/top_level.txt
--rw-r--r--   0 mcmenemy   (501) staff       (20)      117 2023-06-20 18:06:34.000000 PlexLabExchange-0.8.4/README.md
--rw-r--r--   0 mcmenemy   (501) staff       (20)       38 2023-06-20 19:04:51.772689 PlexLabExchange-0.8.4/setup.cfg
--rw-r--r--   0 mcmenemy   (501) staff       (20)     3980 2023-06-20 19:04:45.000000 PlexLabExchange-0.8.4/setup.py
+drwxr-xr-x   0 mcmenemy   (501) staff       (20)        0 2023-06-20 19:12:36.486742 PlexLabExchange-0.8.5/
+-rw-r--r--   0 mcmenemy   (501) staff       (20)      603 2023-06-20 19:12:36.486560 PlexLabExchange-0.8.5/PKG-INFO
+drwxr-xr-x   0 mcmenemy   (501) staff       (20)        0 2023-06-20 19:12:36.486352 PlexLabExchange-0.8.5/PlexLabExchange.egg-info/
+-rw-r--r--   0 mcmenemy   (501) staff       (20)      603 2023-06-20 19:12:36.000000 PlexLabExchange-0.8.5/PlexLabExchange.egg-info/PKG-INFO
+-rw-r--r--   0 mcmenemy   (501) staff       (20)      174 2023-06-20 19:12:36.000000 PlexLabExchange-0.8.5/PlexLabExchange.egg-info/SOURCES.txt
+-rw-r--r--   0 mcmenemy   (501) staff       (20)        1 2023-06-20 19:12:36.000000 PlexLabExchange-0.8.5/PlexLabExchange.egg-info/dependency_links.txt
+-rw-r--r--   0 mcmenemy   (501) staff       (20)        1 2023-06-20 19:12:36.000000 PlexLabExchange-0.8.5/PlexLabExchange.egg-info/top_level.txt
+-rw-r--r--   0 mcmenemy   (501) staff       (20)      117 2023-06-20 18:06:34.000000 PlexLabExchange-0.8.5/README.md
+-rw-r--r--   0 mcmenemy   (501) staff       (20)       38 2023-06-20 19:12:36.486784 PlexLabExchange-0.8.5/setup.cfg
+-rw-r--r--   0 mcmenemy   (501) staff       (20)     3659 2023-06-20 19:12:21.000000 PlexLabExchange-0.8.5/setup.py
```

### Comparing `PlexLabExchange-0.8.4/PKG-INFO` & `PlexLabExchange-0.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexLabExchange
-Version: 0.8.4
+Version: 0.8.5
 Summary: A Python interface to the Plex Go CLI.
 Home-page: https://github.com/labdao/plex
 Author: LabDAO
 Author-email: media@labdao.xyz
 License: MIT
 Keywords: plex golang cli wrapper
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `PlexLabExchange-0.8.4/PlexLabExchange.egg-info/PKG-INFO` & `PlexLabExchange-0.8.5/PlexLabExchange.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexLabExchange
-Version: 0.8.4
+Version: 0.8.5
 Summary: A Python interface to the Plex Go CLI.
 Home-page: https://github.com/labdao/plex
 Author: LabDAO
 Author-email: media@labdao.xyz
 License: MIT
 Keywords: plex golang cli wrapper
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `PlexLabExchange-0.8.4/setup.py` & `PlexLabExchange-0.8.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -41,38 +41,32 @@
                 go_bin_url = "https://github.com/labdao/plex/releases/download/v0.8.0/plex_0.8.0_darwin_arm64.tar.gz"
         # Download Go binary to scripts path
         if go_bin_url:
             try:
                 with tempfile.TemporaryDirectory() as temp_dir:
                     self.download_and_extract(go_bin_url, temp_dir)
 
-                    # move the binary to the package directory
+                    # move the binary to the bin directory
                     src = os.path.join(temp_dir, 'plex')
-                    dst_dir = os.path.join(self.install_lib, 'PlexLabExchange')
+                    dst = os.path.join(self.install_scripts, 'plex')
 
-                    # Create target Directory if don't exist
-                    if not os.path.exists(dst_dir):
-                        os.makedirs(dst_dir)
-                    dst = os.path.join(dst_dir, 'plex')
                     shutil.move(src, dst)
-                    # set the binary as executable
-                    os.chmod(dst, 0o755)
             except Exception as e:
                 print(f"Failed to download and extract the Go binary: {e}")
         else:
             raise RuntimeError(f"The current platform/machine of {system_platform}/{machine} is not supported.")
 
     def download_and_extract(self, go_bin_url, temp_dir):
         # Note: This assumes that curl and tar are installed on the system
         subprocess.run(f"curl -sSL {go_bin_url} | tar xvz -C {temp_dir}", shell=True, check=True)
 
 
 setup(
     name="PlexLabExchange",
-    version="0.8.4",
+    version="0.8.5",
     packages=find_packages(),
     cmdclass={
         'install': PostInstallCommand,
     },
     author="LabDAO",
     author_email="media@labdao.xyz",
     description="A Python interface to the Plex Go CLI.",
```

