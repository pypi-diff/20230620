# Comparing `tmp/cemconvert-0.5.1.tar.gz` & `tmp/cemconvert-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cemconvert-0.5.1.tar", last modified: Fri Jun 16 19:42:26 2023, max compression
+gzip compressed data, was "dist/cemconvert-0.5.4.tar", last modified: Tue Jun 20 17:21:59 2023, max compression
```

## Comparing `cemconvert-0.5.1.tar` & `cemconvert-0.5.4.tar`

### file list

```diff
@@ -1,18 +1,28 @@
-drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-16 19:42:26.000000 cemconvert-0.5.1/
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)      341 2023-05-22 20:27:00.000000 cemconvert-0.5.1/setup.py
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)      198 2023-06-16 19:42:26.000000 cemconvert-0.5.1/PKG-INFO
-drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-16 19:42:26.000000 cemconvert-0.5.1/bin/
--rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     5195 2023-05-12 16:05:11.000000 cemconvert-0.5.1/bin/get_camd_cems
--rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     3996 2023-02-08 15:41:07.000000 cemconvert-0.5.1/bin/cemconvert
-drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-16 19:42:26.000000 cemconvert-0.5.1/cemconvert/
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)     2597 2023-05-17 15:23:53.000000 cemconvert-0.5.1/cemconvert/tz.py
--rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     3821 2023-05-17 15:23:53.000000 cemconvert-0.5.1/cemconvert/temporal.py
--rwxrwxr-x   0 jbeidler  (1855) emis     (54388)    10129 2023-05-17 15:23:53.000000 cemconvert-0.5.1/cemconvert/ff10.py
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)     1995 2023-05-17 15:23:53.000000 cemconvert-0.5.1/cemconvert/qa.py
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)      283 2023-05-17 15:23:53.000000 cemconvert-0.5.1/cemconvert/__init__.py
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)     7071 2023-05-22 20:25:07.000000 cemconvert-0.5.1/cemconvert/cemcorrect.py
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)     5273 2023-05-17 15:23:53.000000 cemconvert-0.5.1/cemconvert/proc.py
--rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     6781 2023-05-19 20:23:16.000000 cemconvert-0.5.1/cemconvert/cem.py
-drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-16 19:42:26.000000 cemconvert-0.5.1/cemconvert/data/
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)    95049 2023-02-08 15:30:00.000000 cemconvert-0.5.1/cemconvert/data/county_fips_tz.csv
--rw-rw-r--   0 jbeidler  (1855) emis     (54388)     4818 2023-05-17 15:23:53.000000 cemconvert-0.5.1/cemconvert/run_parse.py
+drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-20 17:21:59.000000 cemconvert-0.5.4/
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)      671 2023-06-20 17:21:54.000000 cemconvert-0.5.4/setup.py
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)      205 2023-06-20 17:21:59.000000 cemconvert-0.5.4/PKG-INFO
+drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-20 17:21:59.000000 cemconvert-0.5.4/bin/
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     5195 2023-05-12 16:05:11.000000 cemconvert-0.5.4/bin/get_camd_cems
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     3996 2023-02-08 15:41:07.000000 cemconvert-0.5.4/bin/cemconvert
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     6349 2023-05-12 16:11:03.000000 cemconvert-0.5.4/bin/get_camd_cems_bulk
+drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-20 17:21:59.000000 cemconvert-0.5.4/cemconvert/
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)     2597 2023-05-17 15:23:53.000000 cemconvert-0.5.4/cemconvert/tz.py
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     3821 2023-05-17 15:23:53.000000 cemconvert-0.5.4/cemconvert/temporal.py
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)    10129 2023-05-17 15:23:53.000000 cemconvert-0.5.4/cemconvert/ff10.py
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)     1995 2023-05-17 15:23:53.000000 cemconvert-0.5.4/cemconvert/qa.py
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)      283 2023-05-17 15:23:53.000000 cemconvert-0.5.4/cemconvert/__init__.py
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)     7071 2023-05-22 20:25:07.000000 cemconvert-0.5.4/cemconvert/cemcorrect.py
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)     5273 2023-05-17 15:23:53.000000 cemconvert-0.5.4/cemconvert/proc.py
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     6781 2023-05-19 20:23:16.000000 cemconvert-0.5.4/cemconvert/cem.py
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)     4818 2023-06-20 16:36:27.000000 cemconvert-0.5.4/cemconvert/run_parse.py
+drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-20 17:21:59.000000 cemconvert-0.5.4/examples/
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)      307 2023-06-20 16:30:32.000000 cemconvert-0.5.4/examples/get_camd_cems.csh
+-rwxrwxr-x   0 jbeidler  (1855) emis     (54388)     1188 2023-06-16 19:57:48.000000 cemconvert-0.5.4/examples/cemconvert_2021.csh
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)       38 2023-06-20 17:21:59.000000 cemconvert-0.5.4/setup.cfg
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)     2499 2023-06-20 16:44:51.000000 cemconvert-0.5.4/README.md
+drwxrwsr-x   0 jbeidler  (1855) emis     (54388)        0 2023-06-20 17:21:59.000000 cemconvert-0.5.4/cemconvert.egg-info/
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)      484 2023-06-20 17:21:59.000000 cemconvert-0.5.4/cemconvert.egg-info/SOURCES.txt
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)      205 2023-06-20 17:21:59.000000 cemconvert-0.5.4/cemconvert.egg-info/PKG-INFO
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)        1 2023-06-20 17:21:59.000000 cemconvert-0.5.4/cemconvert.egg-info/dependency_links.txt
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)       11 2023-06-20 17:21:59.000000 cemconvert-0.5.4/cemconvert.egg-info/top_level.txt
+-rw-rw-r--   0 jbeidler  (1855) emis     (54388)       28 2023-06-20 17:21:59.000000 cemconvert-0.5.4/cemconvert.egg-info/requires.txt
```

### Comparing `cemconvert-0.5.1/bin/get_camd_cems` & `cemconvert-0.5.4/bin/get_camd_cems`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.1/bin/cemconvert` & `cemconvert-0.5.4/bin/cemconvert`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.1/cemconvert/tz.py` & `cemconvert-0.5.4/cemconvert/tz.py`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.1/cemconvert/temporal.py` & `cemconvert-0.5.4/cemconvert/temporal.py`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.1/cemconvert/ff10.py` & `cemconvert-0.5.4/cemconvert/ff10.py`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.1/cemconvert/qa.py` & `cemconvert-0.5.4/cemconvert/qa.py`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.1/cemconvert/cemcorrect.py` & `cemconvert-0.5.4/cemconvert/cemcorrect.py`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.1/cemconvert/proc.py` & `cemconvert-0.5.4/cemconvert/proc.py`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.1/cemconvert/cem.py` & `cemconvert-0.5.4/cemconvert/cem.py`

 * *Files identical despite different names*

### Comparing `cemconvert-0.5.1/cemconvert/run_parse.py` & `cemconvert-0.5.4/cemconvert/run_parse.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     def get_opts(self):
         '''
         Handle command line arguments and options.
         '''
         self.parser = OptionParser(usage = 'usage: %prog [options] egu_annual_ff10')
         self.parser.add_option('-p', '--cempolls', dest='cempolls', 
-          help='List of pollutants in hourly CEM fires to process', default='NOX,SO2,CO2')
+          help='List of pollutants in hourly CEM files to process', default='NOX,SO2,CO2')
         self.parser.add_option('-y', '--year', dest='year', help='Year to process', default='2016')
         self.parser.add_option('-i', '--input_path', dest='input_path', 
           help='Hourly CEM input path', default='input')
         self.parser.add_option('-o', '--output_path', dest='output_path', 
           help='FF10 inventory output path', default='output')
         self.parser.add_option('-c', '--write_cems', action='store_true', dest='write_cems', 
           help='Write hourly CEM data in old SMOKE format', default=False)
```

