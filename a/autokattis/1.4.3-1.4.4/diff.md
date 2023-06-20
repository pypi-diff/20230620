# Comparing `tmp/autokattis-1.4.3.tar.gz` & `tmp/autokattis-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autokattis-1.4.3.tar", last modified: Sun May 14 13:46:16 2023, max compression
+gzip compressed data, was "autokattis-1.4.4.tar", last modified: Tue Jun 20 09:10:38 2023, max compression
```

## Comparing `autokattis-1.4.3.tar` & `autokattis-1.4.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-05-14 13:46:15.998263 autokattis-1.4.3/
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)    35148 2023-05-04 07:45:56.000000 autokattis-1.4.3/LICENSE
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)     2580 2023-05-14 13:46:15.993262 autokattis-1.4.3/PKG-INFO
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)     2226 2023-05-11 09:23:16.000000 autokattis-1.4.3/README.md
-drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-05-14 13:46:15.861648 autokattis-1.4.3/autokattis/
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       24 2023-05-11 09:21:05.000000 autokattis-1.4.3/autokattis/__init__.py
-drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-05-14 13:46:15.941265 autokattis-1.4.3/autokattis/api/
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)    22037 2023-05-14 13:37:52.000000 autokattis-1.4.3/autokattis/api/__init__.py
-drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-05-14 13:46:15.948259 autokattis-1.4.3/autokattis/database/
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)   133880 2023-05-08 08:31:18.000000 autokattis-1.4.3/autokattis/database/__init__.py
-drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-05-14 13:46:15.974265 autokattis-1.4.3/autokattis/scraper/
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       37 2023-05-11 07:47:42.000000 autokattis-1.4.3/autokattis/scraper/__init__.py
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)     3031 2023-05-11 07:45:04.000000 autokattis-1.4.3/autokattis/scraper/country.py
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)      977 2023-05-11 07:45:16.000000 autokattis-1.4.3/autokattis/scraper/university.py
-drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-05-14 13:46:15.981261 autokattis-1.4.3/autokattis/utils/
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)      518 2023-05-11 07:23:19.000000 autokattis-1.4.3/autokattis/utils/__init__.py
-drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-05-14 13:46:15.932258 autokattis-1.4.3/autokattis.egg-info/
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)     2580 2023-05-14 13:46:15.000000 autokattis-1.4.3/autokattis.egg-info/PKG-INFO
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)      400 2023-05-14 13:46:15.000000 autokattis-1.4.3/autokattis.egg-info/SOURCES.txt
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)        1 2023-05-14 13:46:15.000000 autokattis-1.4.3/autokattis.egg-info/dependency_links.txt
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       80 2023-05-14 13:46:15.000000 autokattis-1.4.3/autokattis.egg-info/requires.txt
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       11 2023-05-14 13:46:15.000000 autokattis-1.4.3/autokattis.egg-info/top_level.txt
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       38 2023-05-14 13:46:15.999261 autokattis-1.4.3/setup.cfg
--rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)      878 2023-05-14 13:40:47.000000 autokattis-1.4.3/setup.py
+drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-06-20 09:10:38.300587 autokattis-1.4.4/
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)    35148 2023-05-04 07:45:56.000000 autokattis-1.4.4/LICENSE
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)     2639 2023-06-20 09:10:38.299526 autokattis-1.4.4/PKG-INFO
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)     2285 2023-06-20 09:03:54.000000 autokattis-1.4.4/README.md
+drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-06-20 09:10:38.274178 autokattis-1.4.4/autokattis/
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       24 2023-05-11 09:21:05.000000 autokattis-1.4.4/autokattis/__init__.py
+drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-06-20 09:10:38.288192 autokattis-1.4.4/autokattis/api/
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)    22404 2023-06-20 08:58:31.000000 autokattis-1.4.4/autokattis/api/__init__.py
+drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-06-20 09:10:38.290491 autokattis-1.4.4/autokattis/database/
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)   133880 2023-05-08 08:31:18.000000 autokattis-1.4.4/autokattis/database/__init__.py
+drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-06-20 09:10:38.295490 autokattis-1.4.4/autokattis/scraper/
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       37 2023-05-11 07:47:42.000000 autokattis-1.4.4/autokattis/scraper/__init__.py
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)     3031 2023-05-11 07:45:04.000000 autokattis-1.4.4/autokattis/scraper/country.py
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)      977 2023-05-11 07:45:16.000000 autokattis-1.4.4/autokattis/scraper/university.py
+drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-06-20 09:10:38.298490 autokattis-1.4.4/autokattis/utils/
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)      518 2023-05-11 07:23:19.000000 autokattis-1.4.4/autokattis/utils/__init__.py
+drwxr-xr-x   0 russellsaerang  (1000) russellsaerang  (1000)        0 2023-06-20 09:10:38.287178 autokattis-1.4.4/autokattis.egg-info/
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)     2639 2023-06-20 09:10:38.000000 autokattis-1.4.4/autokattis.egg-info/PKG-INFO
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)      400 2023-06-20 09:10:38.000000 autokattis-1.4.4/autokattis.egg-info/SOURCES.txt
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)        1 2023-06-20 09:10:38.000000 autokattis-1.4.4/autokattis.egg-info/dependency_links.txt
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       80 2023-06-20 09:10:38.000000 autokattis-1.4.4/autokattis.egg-info/requires.txt
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       11 2023-06-20 09:10:38.000000 autokattis-1.4.4/autokattis.egg-info/top_level.txt
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)       38 2023-06-20 09:10:38.301490 autokattis-1.4.4/setup.cfg
+-rw-r--r--   0 russellsaerang  (1000) russellsaerang  (1000)      878 2023-06-20 08:56:45.000000 autokattis-1.4.4/setup.py
```

### Comparing `autokattis-1.4.3/LICENSE` & `autokattis-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `autokattis-1.4.3/PKG-INFO` & `autokattis-1.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autokattis
-Version: 1.4.3
+Version: 1.4.4
 Summary: Updated Kattis API wrapper
 Home-page: https://github.com/RussellDash332/autokattis
 Download-URL: https://pypi.org/project/autokattis/
 Author: Russell Saerang
 Author-email: russellsaerang@gmail.com
 License: MIT
 Keywords: Kattis
@@ -38,14 +38,15 @@
 
 ### Problem-specific
 
 ```py
 kt.problems()                               # problems you have solved so far
 kt.problems(show_partial=False)             # exclude partial submissions
 kt.problems(*[True]*4)                      # literally all problems on Kattis
+kt.list_unsolved()                          # let's grind!
 
 kt.plot_problems()                          # plot the points distribution
 kt.plot_problems(filepath='plot.png')       # save to a filepath
 kt.plot_problems(show_partial=False)        # plot fully solved submissions
 
 kt.problem('2048')                          # fetch info about a problem
 kt.problem('2048', 'abinitio', 'dasort')    # fetch multiple in one
```

### Comparing `autokattis-1.4.3/README.md` & `autokattis-1.4.4/autokattis.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: autokattis
+Version: 1.4.4
+Summary: Updated Kattis API wrapper
+Home-page: https://github.com/RussellDash332/autokattis
+Download-URL: https://pypi.org/project/autokattis/
+Author: Russell Saerang
+Author-email: russellsaerang@gmail.com
+License: MIT
+Keywords: Kattis
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # autokattis
 
 Updated Kattis API wrapper as of May 2023 after the major UI/UX change.
 
 ## Setup
 
 Simply install it as a Python package.
@@ -25,14 +38,15 @@
 
 ### Problem-specific
 
 ```py
 kt.problems()                               # problems you have solved so far
 kt.problems(show_partial=False)             # exclude partial submissions
 kt.problems(*[True]*4)                      # literally all problems on Kattis
+kt.list_unsolved()                          # let's grind!
 
 kt.plot_problems()                          # plot the points distribution
 kt.plot_problems(filepath='plot.png')       # save to a filepath
 kt.plot_problems(show_partial=False)        # plot fully solved submissions
 
 kt.problem('2048')                          # fetch info about a problem
 kt.problem('2048', 'abinitio', 'dasort')    # fetch multiple in one
@@ -66,8 +80,8 @@
 
 - Kattis official CLI tool: https://github.com/Kattis/kattis-cli
 
     > Since Kattis has provided an official tool to automate submissions, there won't be such feature in `autokattis`.
 
 ## Contributing
 
-asdf
+asdf
```

### Comparing `autokattis-1.4.3/autokattis/api/__init__.py` & `autokattis-1.4.4/autokattis/api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,16 +93,16 @@
                     table = soup.find('table', class_='table2')
                     for row in table.tbody.find_all('tr'):
                         columns = row.find_all('td')
                         if columns:
                             has_content = True
                             link = f"{self.BASE_URL}{columns[0].find('a').get('href')}"
                             name = columns[0].text
-                            fastest = float(columns[2].text)
-                            shortest = int(columns[3].text)
+                            fastest = float(columns[2].text.replace('--', 'inf'))
+                            shortest = int(columns[3].text.replace('--', '-1'))
                             total = int(columns[4].text)
                             acc = int(columns[5].text)
                             difficulty = float(re.findall('[\d\.]+', columns[7].text)[-1])
                                 # [0] instead of [-1] if we want to take min instead of max
                                 # for example:
                                 # - difficulty 9.1-9.6 -> [9.1, 9.6]
                                 # - difficulty 5.0 -> [5.0]
@@ -131,14 +131,22 @@
         hist.set(title=f'Solved Kattis Problems ({df.shape[0]})', xlabel='Difficulty')
         plt.xticks([*range(math.floor(min(df.difficulty)), math.ceil(max(df.difficulty))+1)])
         plt.show()
         if filepath != None:
             plt.savefig(filepath)
             print(f'Saved to {filepath}')
 
+    def list_unsolved(self, show_partial=True):
+        '''
+        Quick shortcut for all Kattis grinders to list all unsolved questions.
+
+        Default: includes partially solved questions.
+        '''
+        return self.problems(show_solved=False, show_partial=show_partial, show_tried=True, show_untried=True)
+
     def problem(self, problem_id, *problem_ids):
         '''
         Obtain information about one or more specific problems.
         Returns a JSON-like structure of the problem body text and their metadata.
         '''
 
         response = self.get(f'{self.BASE_URL}/problems/{problem_id}')
```

### Comparing `autokattis-1.4.3/autokattis/database/__init__.py` & `autokattis-1.4.4/autokattis/database/__init__.py`

 * *Files identical despite different names*

### Comparing `autokattis-1.4.3/autokattis/scraper/country.py` & `autokattis-1.4.4/autokattis/scraper/country.py`

 * *Files identical despite different names*

### Comparing `autokattis-1.4.3/autokattis/scraper/university.py` & `autokattis-1.4.4/autokattis/scraper/university.py`

 * *Files identical despite different names*

### Comparing `autokattis-1.4.3/autokattis/utils/__init__.py` & `autokattis-1.4.4/autokattis/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `autokattis-1.4.3/setup.py` & `autokattis-1.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='autokattis',
-    version='1.4.3',
+    version='1.4.4',
     description='Updated Kattis API wrapper',
     long_description_content_type="text/markdown",
     long_description=README,
     license='MIT',
     packages=find_packages(),
     author='Russell Saerang',
     author_email='russellsaerang@gmail.com',
```

