# Comparing `tmp/me_setups-1.9.0.tar.gz` & `tmp/me_setups-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "me_setups-1.9.0.tar", last modified: Mon Jun 19 10:37:28 2023, max compression
+gzip compressed data, was "me_setups-1.9.1.tar", last modified: Tue Jun 20 18:05:45 2023, max compression
```

## Comparing `me_setups-1.9.0.tar` & `me_setups-1.9.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-19 10:37:28.087595 me_setups-1.9.0/
--rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-06-19 10:37:28.087611 me_setups-1.9.0/PKG-INFO
--rw-r--r--   0 idof     (12090585) develop   (1000)       19 2023-01-29 18:05:41.000000 me_setups-1.9.0/README.md
--rw-r--r--   0 idof     (12090585) develop   (1000)     1242 2023-06-19 10:37:28.089621 me_setups-1.9.0/setup.cfg
--rw-r--r--   0 idof     (12090585) develop   (1000)       74 2023-01-29 18:02:02.000000 me_setups-1.9.0/setup.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-19 10:37:28.051569 me_setups-1.9.0/src/
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-19 10:37:28.061603 me_setups-1.9.0/src/me_setups/
--rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-29 21:40:13.000000 me_setups-1.9.0/src/me_setups/__init__.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-19 10:37:28.079025 me_setups-1.9.0/src/me_setups/boards/
--rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-02-15 14:02:28.000000 me_setups-1.9.0/src/me_setups/boards/__init__.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      920 2023-03-12 12:03:35.000000 me_setups-1.9.0/src/me_setups/boards/default_boards.py
--rw-r--r--   0 idof     (12090585) develop   (1000)    11767 2023-06-15 20:19:29.000000 me_setups-1.9.0/src/me_setups/boards/gas52.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      119 2023-02-16 19:57:32.000000 me_setups-1.9.0/src/me_setups/boards/types.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-19 10:37:28.086234 me_setups-1.9.0/src/me_setups/components/
--rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-30 07:57:12.000000 me_setups-1.9.0/src/me_setups/components/__init__.py
--rw-r--r--   0 idof     (12090585) develop   (1000)     8703 2023-06-19 10:33:52.000000 me_setups-1.9.0/src/me_setups/components/comp.py
--rw-r--r--   0 idof     (12090585) develop   (1000)    14193 2023-06-15 20:19:29.000000 me_setups-1.9.0/src/me_setups/components/eqs.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      198 2023-05-18 10:10:02.000000 me_setups-1.9.0/src/me_setups/components/mcs.py
--rw-r--r--   0 idof     (12090585) develop   (1000)     4187 2023-05-18 10:10:02.000000 me_setups-1.9.0/src/me_setups/components/mcu.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      488 2023-06-06 17:26:44.000000 me_setups-1.9.0/src/me_setups/utils.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-19 10:37:28.070602 me_setups-1.9.0/src/me_setups.egg-info/
--rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-06-19 10:37:27.000000 me_setups-1.9.0/src/me_setups.egg-info/PKG-INFO
--rw-r--r--   0 idof     (12090585) develop   (1000)      559 2023-06-19 10:37:27.000000 me_setups-1.9.0/src/me_setups.egg-info/SOURCES.txt
--rw-r--r--   0 idof     (12090585) develop   (1000)        1 2023-06-19 10:37:27.000000 me_setups-1.9.0/src/me_setups.egg-info/dependency_links.txt
--rw-r--r--   0 idof     (12090585) develop   (1000)       66 2023-06-19 10:37:27.000000 me_setups-1.9.0/src/me_setups.egg-info/requires.txt
--rw-r--r--   0 idof     (12090585) develop   (1000)       10 2023-06-19 10:37:27.000000 me_setups-1.9.0/src/me_setups.egg-info/top_level.txt
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-20 18:05:45.247057 me_setups-1.9.1/
+-rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-06-20 18:05:45.247083 me_setups-1.9.1/PKG-INFO
+-rw-r--r--   0 idof     (12090585) develop   (1000)       19 2023-01-29 18:05:41.000000 me_setups-1.9.1/README.md
+-rw-r--r--   0 idof     (12090585) develop   (1000)     1242 2023-06-20 18:05:45.249061 me_setups-1.9.1/setup.cfg
+-rw-r--r--   0 idof     (12090585) develop   (1000)       74 2023-01-29 18:02:02.000000 me_setups-1.9.1/setup.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-20 18:05:45.213816 me_setups-1.9.1/src/
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-20 18:05:45.218854 me_setups-1.9.1/src/me_setups/
+-rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-29 21:40:13.000000 me_setups-1.9.1/src/me_setups/__init__.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-20 18:05:45.235843 me_setups-1.9.1/src/me_setups/boards/
+-rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-02-15 14:02:28.000000 me_setups-1.9.1/src/me_setups/boards/__init__.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      920 2023-03-12 12:03:35.000000 me_setups-1.9.1/src/me_setups/boards/default_boards.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)    11767 2023-06-15 20:19:29.000000 me_setups-1.9.1/src/me_setups/boards/gas52.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      119 2023-02-16 19:57:32.000000 me_setups-1.9.1/src/me_setups/boards/types.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-20 18:05:45.251794 me_setups-1.9.1/src/me_setups/components/
+-rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-30 07:57:12.000000 me_setups-1.9.1/src/me_setups/components/__init__.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)     8703 2023-06-19 10:33:52.000000 me_setups-1.9.1/src/me_setups/components/comp.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)    14195 2023-06-20 17:46:10.000000 me_setups-1.9.1/src/me_setups/components/eqs.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      198 2023-05-18 10:10:02.000000 me_setups-1.9.1/src/me_setups/components/mcs.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)     4187 2023-05-18 10:10:02.000000 me_setups-1.9.1/src/me_setups/components/mcu.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      488 2023-06-06 17:26:44.000000 me_setups-1.9.1/src/me_setups/utils.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-20 18:05:45.232790 me_setups-1.9.1/src/me_setups.egg-info/
+-rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-06-20 18:05:45.000000 me_setups-1.9.1/src/me_setups.egg-info/PKG-INFO
+-rw-r--r--   0 idof     (12090585) develop   (1000)      559 2023-06-20 18:05:45.000000 me_setups-1.9.1/src/me_setups.egg-info/SOURCES.txt
+-rw-r--r--   0 idof     (12090585) develop   (1000)        1 2023-06-20 18:05:45.000000 me_setups-1.9.1/src/me_setups.egg-info/dependency_links.txt
+-rw-r--r--   0 idof     (12090585) develop   (1000)       66 2023-06-20 18:05:45.000000 me_setups-1.9.1/src/me_setups.egg-info/requires.txt
+-rw-r--r--   0 idof     (12090585) develop   (1000)       10 2023-06-20 18:05:45.000000 me_setups-1.9.1/src/me_setups.egg-info/top_level.txt
```

### Comparing `me_setups-1.9.0/PKG-INFO` & `me_setups-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: me_setups
-Version: 1.9.0
+Version: 1.9.1
 Summary: Abstraction for Mobileye setups.
 Home-page: http://gitlab.mobileye.com/idof/me-setups
 Author: Ido Frenkel
 Author-email: ido.frenkel@mobileye.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `me_setups-1.9.0/setup.cfg` & `me_setups-1.9.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = me_setups
-version = 1.9.0
+version = 1.9.1
 description = Abstraction for Mobileye setups.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = http://gitlab.mobileye.com/idof/me-setups
 author = Ido Frenkel
 author_email = ido.frenkel@mobileye.com
 classifiers =
```

### Comparing `me_setups-1.9.0/src/me_setups/boards/default_boards.py` & `me_setups-1.9.1/src/me_setups/boards/default_boards.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.9.0/src/me_setups/boards/gas52.py` & `me_setups-1.9.1/src/me_setups/boards/gas52.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.9.0/src/me_setups/components/comp.py` & `me_setups-1.9.1/src/me_setups/components/comp.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.9.0/src/me_setups/components/eqs.py` & `me_setups-1.9.1/src/me_setups/components/eqs.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     NO_KEY_CHECK = "-o StrictHostKeyChecking=no -o LogLevel=FATAL"
 
     def __init__(self, prefix: str, timeout: float) -> None:
         self.prefix = f"{prefix} {self.NO_KEY_CHECK}"
         self.timeout = timeout
 
     def _run(self, cmd: str, *args: Any, **kwargs: Any) -> CompletedProcess[str]:
-        _cmd = shlex.split(f"{self.prefix} {cmd}")
+        _cmd = shlex.split(f'{self.prefix} "{cmd}"')
         return subprocess.run(
             _cmd,
             *args,
             timeout=self.timeout,
             capture_output=True,
             text=True,
             **kwargs,
```

### Comparing `me_setups-1.9.0/src/me_setups/components/mcu.py` & `me_setups-1.9.1/src/me_setups/components/mcu.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.9.0/src/me_setups.egg-info/PKG-INFO` & `me_setups-1.9.1/src/me_setups.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: me-setups
-Version: 1.9.0
+Version: 1.9.1
 Summary: Abstraction for Mobileye setups.
 Home-page: http://gitlab.mobileye.com/idof/me-setups
 Author: Ido Frenkel
 Author-email: ido.frenkel@mobileye.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `me_setups-1.9.0/src/me_setups.egg-info/SOURCES.txt` & `me_setups-1.9.1/src/me_setups.egg-info/SOURCES.txt`

 * *Files identical despite different names*

