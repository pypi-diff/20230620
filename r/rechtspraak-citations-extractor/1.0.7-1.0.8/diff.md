# Comparing `tmp/rechtspraak_citations_extractor-1.0.7.tar.gz` & `tmp/rechtspraak_citations_extractor-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rechtspraak_citations_extractor-1.0.7.tar", last modified: Fri Jun 16 20:33:26 2023, max compression
+gzip compressed data, was "rechtspraak_citations_extractor-1.0.8.tar", last modified: Tue Jun 20 19:24:11 2023, max compression
```

## Comparing `rechtspraak_citations_extractor-1.0.7.tar` & `rechtspraak_citations_extractor-1.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 20:33:26.275062 rechtspraak_citations_extractor-1.0.7/
--rw-rw-rw-   0        0        0     4818 2023-06-16 20:33:26.274063 rechtspraak_citations_extractor-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     4298 2023-06-02 17:47:16.000000 rechtspraak_citations_extractor-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 20:33:26.264062 rechtspraak_citations_extractor-1.0.7/rechtspraak_citations_extractor/
--rw-rw-rw-   0        0        0       79 2023-06-03 12:22:13.000000 rechtspraak_citations_extractor-1.0.7/rechtspraak_citations_extractor/__init__.py
--rw-rw-rw-   0        0        0    13439 2023-06-16 20:31:25.000000 rechtspraak_citations_extractor-1.0.7/rechtspraak_citations_extractor/citations_extractor.py
--rw-rw-rw-   0        0        0      247 2023-06-02 17:18:56.000000 rechtspraak_citations_extractor-1.0.7/rechtspraak_citations_extractor/testing.py
-drwxrwxrwx   0        0        0        0 2023-06-16 20:33:26.272064 rechtspraak_citations_extractor-1.0.7/rechtspraak_citations_extractor.egg-info/
--rw-rw-rw-   0        0        0     4818 2023-06-16 20:33:26.000000 rechtspraak_citations_extractor-1.0.7/rechtspraak_citations_extractor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-06-16 20:33:26.000000 rechtspraak_citations_extractor-1.0.7/rechtspraak_citations_extractor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 20:33:26.000000 rechtspraak_citations_extractor-1.0.7/rechtspraak_citations_extractor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-06-16 20:33:26.000000 rechtspraak_citations_extractor-1.0.7/rechtspraak_citations_extractor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-06-16 20:33:26.000000 rechtspraak_citations_extractor-1.0.7/rechtspraak_citations_extractor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 20:33:26.275062 rechtspraak_citations_extractor-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1015 2023-06-16 20:33:21.000000 rechtspraak_citations_extractor-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:24:11.499824 rechtspraak_citations_extractor-1.0.8/
+-rw-rw-rw-   0        0        0     4818 2023-06-20 19:24:11.498824 rechtspraak_citations_extractor-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4298 2023-06-02 17:47:16.000000 rechtspraak_citations_extractor-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 19:24:11.487824 rechtspraak_citations_extractor-1.0.8/rechtspraak_citations_extractor/
+-rw-rw-rw-   0        0        0       79 2023-06-03 12:22:13.000000 rechtspraak_citations_extractor-1.0.8/rechtspraak_citations_extractor/__init__.py
+-rw-rw-rw-   0        0        0    13457 2023-06-20 19:22:48.000000 rechtspraak_citations_extractor-1.0.8/rechtspraak_citations_extractor/citations_extractor.py
+-rw-rw-rw-   0        0        0      247 2023-06-02 17:18:56.000000 rechtspraak_citations_extractor-1.0.8/rechtspraak_citations_extractor/testing.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:24:11.496824 rechtspraak_citations_extractor-1.0.8/rechtspraak_citations_extractor.egg-info/
+-rw-rw-rw-   0        0        0     4818 2023-06-20 19:24:11.000000 rechtspraak_citations_extractor-1.0.8/rechtspraak_citations_extractor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-06-20 19:24:11.000000 rechtspraak_citations_extractor-1.0.8/rechtspraak_citations_extractor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 19:24:11.000000 rechtspraak_citations_extractor-1.0.8/rechtspraak_citations_extractor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-06-20 19:24:11.000000 rechtspraak_citations_extractor-1.0.8/rechtspraak_citations_extractor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-06-20 19:24:11.000000 rechtspraak_citations_extractor-1.0.8/rechtspraak_citations_extractor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 19:24:11.499824 rechtspraak_citations_extractor-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1015 2023-06-20 19:24:05.000000 rechtspraak_citations_extractor-1.0.8/setup.py
```

### Comparing `rechtspraak_citations_extractor-1.0.7/PKG-INFO` & `rechtspraak_citations_extractor-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rechtspraak_citations_extractor
-Version: 1.0.7
+Version: 1.0.8
 Summary: Library for extracting rechtspraak citations via LIDO
 Author: LawTech Lab
 Author-email: p.lewandowski@student.maastrichtuniversity.nl
 License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/extraction_libraries
 Project-URL: Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: rechtspraak,citations,rechtspraak citations,RS citations
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rechtspraak_citations_extractor Version: 1.0.7
+Metadata-Version: 2.1 Name: rechtspraak_citations_extractor Version: 1.0.8
 Summary: Library for extracting rechtspraak citations via LIDO Author: LawTech
 Lab Author-email: p.lewandowski@student.maastrichtuniversity.nl License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/
 extraction_libraries Project-URL: Build Source, https://github.com/
 maastrichtlawtech/extraction_libraries Keywords:
 rechtspraak,citations,rechtspraak citations,RS citations Description-Content-
 Type: text/markdown ## Rechtspraak citations This library contains a function
```

### Comparing `rechtspraak_citations_extractor-1.0.7/README.md` & `rechtspraak_citations_extractor-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `rechtspraak_citations_extractor-1.0.7/rechtspraak_citations_extractor/citations_extractor.py` & `rechtspraak_citations_extractor-1.0.8/rechtspraak_citations_extractor/citations_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
     ecli = dataframe['ecli'].dropna().reset_index(drop=True)
     length = ecli.size
     at_once_threads = int(length / threads)
     big_incoming = []
     big_outgoing = []
     big_legislations = []
     threads = []
-    bar = tqdm(total=length, colour="GREEN",position=0, leave=True,miniters=int(length/100))
+    bar = tqdm(total=length, colour="GREEN",position=0, leave=True,miniters=int(length/100),maxinterval=10000)
     for i in range(0, length, at_once_threads):
         curr_ecli = ecli[i:(i + at_once_threads)]
         t = threading.Thread(target=citations_multithread_single,
                              args=[big_incoming, big_outgoing, big_legislations, curr_ecli, username, password, i,bar])
         threads.append(t)
     for t in threads:
         t.start()
```

### Comparing `rechtspraak_citations_extractor-1.0.7/rechtspraak_citations_extractor.egg-info/PKG-INFO` & `rechtspraak_citations_extractor-1.0.8/rechtspraak_citations_extractor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rechtspraak-citations-extractor
-Version: 1.0.7
+Version: 1.0.8
 Summary: Library for extracting rechtspraak citations via LIDO
 Author: LawTech Lab
 Author-email: p.lewandowski@student.maastrichtuniversity.nl
 License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/extraction_libraries
 Project-URL: Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: rechtspraak,citations,rechtspraak citations,RS citations
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rechtspraak-citations-extractor Version: 1.0.7
+Metadata-Version: 2.1 Name: rechtspraak-citations-extractor Version: 1.0.8
 Summary: Library for extracting rechtspraak citations via LIDO Author: LawTech
 Lab Author-email: p.lewandowski@student.maastrichtuniversity.nl License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/
 extraction_libraries Project-URL: Build Source, https://github.com/
 maastrichtlawtech/extraction_libraries Keywords:
 rechtspraak,citations,rechtspraak citations,RS citations Description-Content-
 Type: text/markdown ## Rechtspraak citations This library contains a function
```

### Comparing `rechtspraak_citations_extractor-1.0.7/setup.py` & `rechtspraak_citations_extractor-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 p = Path("README.md")
 long_descr = p.read_text()
 
 setup(
     name='rechtspraak_citations_extractor',
     packages=find_packages(include=['rechtspraak_citations_extractor']),
-    version='1.0.7',
+    version='1.0.8',
     description='Library for extracting rechtspraak citations via LIDO',
     author='LawTech Lab',
     license='MIT',
     install_requires=['requests>=2.26.0', 'python_dotenv==0.15.0', 'pandas >=1.2.5','urllib3>=1.26.12','lxml>=4.6.3','tqdm'],
     author_email='p.lewandowski@student.maastrichtuniversity.nl',
     keywords=['rechtspraak', 'citations', 'rechtspraak citations', 'RS citations'],
     long_description=long_descr,
```

