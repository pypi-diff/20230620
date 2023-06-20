# Comparing `tmp/rechtspraak_extractor-1.1.8.tar.gz` & `tmp/rechtspraak_extractor-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rechtspraak_extractor-1.1.8.tar", last modified: Mon Apr 10 11:11:24 2023, max compression
+gzip compressed data, was "rechtspraak_extractor-1.1.9.tar", last modified: Sat Jun 10 19:17:59 2023, max compression
```

## Comparing `rechtspraak_extractor-1.1.8.tar` & `rechtspraak_extractor-1.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 11:11:24.659837 rechtspraak_extractor-1.1.8/
--rw-rw-rw-   0        0        0     6911 2023-04-10 11:11:24.658837 rechtspraak_extractor-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     6386 2023-03-14 13:47:20.000000 rechtspraak_extractor-1.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 11:11:24.646834 rechtspraak_extractor-1.1.8/rechtspraak_extractor/
--rw-rw-rw-   0        0        0      251 2022-10-29 13:29:59.000000 rechtspraak_extractor-1.1.8/rechtspraak_extractor/__init__.py
--rw-rw-rw-   0        0        0     3800 2023-04-10 10:34:04.000000 rechtspraak_extractor-1.1.8/rechtspraak_extractor/rechtspraak.py
--rw-rw-rw-   0        0        0     1391 2023-04-04 16:48:14.000000 rechtspraak_extractor-1.1.8/rechtspraak_extractor/rechtspraak_functions.py
--rw-rw-rw-   0        0        0    14747 2023-04-10 10:34:04.000000 rechtspraak_extractor-1.1.8/rechtspraak_extractor/rechtspraak_metadata.py
--rw-rw-rw-   0        0        0      187 2023-04-10 10:58:00.000000 rechtspraak_extractor-1.1.8/rechtspraak_extractor/testing_file.py
-drwxrwxrwx   0        0        0        0 2023-04-10 11:11:24.656834 rechtspraak_extractor-1.1.8/rechtspraak_extractor.egg-info/
--rw-rw-rw-   0        0        0     6911 2023-04-10 11:11:24.000000 rechtspraak_extractor-1.1.8/rechtspraak_extractor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      444 2023-04-10 11:11:24.000000 rechtspraak_extractor-1.1.8/rechtspraak_extractor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 11:11:24.000000 rechtspraak_extractor-1.1.8/rechtspraak_extractor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-04-10 11:11:24.000000 rechtspraak_extractor-1.1.8/rechtspraak_extractor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-04-10 11:11:24.000000 rechtspraak_extractor-1.1.8/rechtspraak_extractor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 11:11:24.659837 rechtspraak_extractor-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0      959 2023-04-10 11:11:16.000000 rechtspraak_extractor-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-10 19:17:59.630228 rechtspraak_extractor-1.1.9/
+-rw-rw-rw-   0        0        0     6868 2023-06-10 19:17:59.629228 rechtspraak_extractor-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6386 2023-03-14 13:47:20.000000 rechtspraak_extractor-1.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-10 19:17:59.618229 rechtspraak_extractor-1.1.9/rechtspraak_extractor/
+-rw-rw-rw-   0        0        0      251 2022-10-29 13:29:59.000000 rechtspraak_extractor-1.1.9/rechtspraak_extractor/__init__.py
+-rw-rw-rw-   0        0        0     3800 2023-04-10 10:34:04.000000 rechtspraak_extractor-1.1.9/rechtspraak_extractor/rechtspraak.py
+-rw-rw-rw-   0        0        0     1391 2023-04-04 16:48:14.000000 rechtspraak_extractor-1.1.9/rechtspraak_extractor/rechtspraak_functions.py
+-rw-rw-rw-   0        0        0    14948 2023-06-10 19:15:13.000000 rechtspraak_extractor-1.1.9/rechtspraak_extractor/rechtspraak_metadata.py
+-rw-rw-rw-   0        0        0      188 2023-06-02 15:45:28.000000 rechtspraak_extractor-1.1.9/rechtspraak_extractor/testing_file.py
+drwxrwxrwx   0        0        0        0 2023-06-10 19:17:59.628229 rechtspraak_extractor-1.1.9/rechtspraak_extractor.egg-info/
+-rw-rw-rw-   0        0        0     6868 2023-06-10 19:17:59.000000 rechtspraak_extractor-1.1.9/rechtspraak_extractor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      444 2023-06-10 19:17:59.000000 rechtspraak_extractor-1.1.9/rechtspraak_extractor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-10 19:17:59.000000 rechtspraak_extractor-1.1.9/rechtspraak_extractor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-06-10 19:17:59.000000 rechtspraak_extractor-1.1.9/rechtspraak_extractor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-10 19:17:59.000000 rechtspraak_extractor-1.1.9/rechtspraak_extractor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-10 19:17:59.630228 rechtspraak_extractor-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      966 2023-06-10 19:17:55.000000 rechtspraak_extractor-1.1.9/setup.py
```

### Comparing `rechtspraak_extractor-1.1.8/PKG-INFO` & `rechtspraak_extractor-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: rechtspraak_extractor
-Version: 1.1.8
+Version: 1.1.9
 Summary: Library for extracting rechtspraak data
-Home-page: UNKNOWN
 Author: LawTech Lab
 Author-email: pranav.bapat@student.maastrichtuniversity.nl
 License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/extraction_libraries
 Project-URL: Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: rechtspraak,extractor,rechtspraak extractor
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 ## Rechtspraak extractor
 This library contains two functions to get rechtspraak data and metadata from the API.
 
 ## Version
 Python 3.9
@@ -167,9 +165,7 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 ```
-
-
```

#### html2text {}

```diff
@@ -1,17 +1,16 @@
-Metadata-Version: 2.1 Name: rechtspraak_extractor Version: 1.1.8 Summary:
-Library for extracting rechtspraak data Home-page: UNKNOWN Author: LawTech Lab
-Author-email: pranav.bapat@student.maastrichtuniversity.nl License: MIT
-Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/
-extraction_libraries Project-URL: Build Source, https://github.com/
-maastrichtlawtech/extraction_libraries Keywords:
-rechtspraak,extractor,rechtspraak extractor Platform: UNKNOWN Description-
-Content-Type: text/markdown ## Rechtspraak extractor This library contains two
-functions to get rechtspraak data and metadata from the API. ## Version Python
-3.9 ## Contributors
+Metadata-Version: 2.1 Name: rechtspraak_extractor Version: 1.1.9 Summary:
+Library for extracting rechtspraak data Author: LawTech Lab Author-email:
+pranav.bapat@student.maastrichtuniversity.nl License: MIT Project-URL: Bug
+Tracker, https://github.com/maastrichtlawtech/extraction_libraries Project-URL:
+Build Source, https://github.com/maastrichtlawtech/extraction_libraries
+Keywords: rechtspraak,extractor,rechtspraak extractor Description-Content-Type:
+text/markdown ## Rechtspraak extractor This library contains two functions to
+get rechtspraak data and metadata from the API. ## Version Python 3.9 ##
+Contributors
 [pranavnbapat]_ [running-machin]_    [Cloud956]_    [shashankmc]_ [gijsvd]_
  Pranav_Bapat    running-machin   Piotr_Lewandowski  shashankmc    gijsvd
  ## How to install? pip install rechtspraak_extractor ## What are the
 functions?
 Rechtspraak Extractor
    1. get_rechtspraak
    2. Gets all the ECLIs and saves them in the CSV file or in-memory.
```

### Comparing `rechtspraak_extractor-1.1.8/README.md` & `rechtspraak_extractor-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `rechtspraak_extractor-1.1.8/rechtspraak_extractor/rechtspraak.py` & `rechtspraak_extractor-1.1.9/rechtspraak_extractor/rechtspraak.py`

 * *Files identical despite different names*

### Comparing `rechtspraak_extractor-1.1.8/rechtspraak_extractor/rechtspraak_functions.py` & `rechtspraak_extractor-1.1.9/rechtspraak_extractor/rechtspraak_functions.py`

 * *Files identical despite different names*

### Comparing `rechtspraak_extractor-1.1.8/rechtspraak_extractor/rechtspraak_metadata.py` & `rechtspraak_extractor-1.1.9/rechtspraak_extractor/rechtspraak_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 import urllib
 import multiprocessing
 from bs4 import BeautifulSoup
 from datetime import datetime
 from concurrent.futures import ThreadPoolExecutor
 import platform
 import shutil
-
+from tqdm import tqdm
 from rechtspraak_extractor.rechtspraak_functions import *
-
+from functools import partial
 # Define base url
 RECHTSPRAAK_METADATA_API_BASE_URL = "http://data.rechtspraak.nl/uitspraken/content?id=" # old one = "https://uitspraken.rechtspraak.nl/#!/details?id="
 return_type = "&return=DOC"
 
 # Define empty lists where we'll store our data temporarily
 ecli_df = []
 full_text_df = []
@@ -287,17 +287,19 @@
         # Get all ECLIs in a list
         ecli_list = list(rs_data.loc[:, 'id'])
 
         # Create a temporary directory to save files
         Path('temp_rs_data').mkdir(parents=True, exist_ok=True)
 
         with ThreadPoolExecutor(max_workers=max_workers) as executor:
+            bar = tqdm(total=len(ecli_list), colour="GREEN")
             for ecli in ecli_list:
                 threads.append(executor.submit(get_data_from_api, ecli))
-
+            for t in threads:
+                t.add_done_callback(partial(bar.update,1))
         # Delete temporary directory
         shutil.rmtree('temp_rs_data')
 
         # global ecli_df, full_text_df, creator_df, date_decision_df, issued_df, zaaknummer_df, \
         #    relations_df, subject_df, procedure_df, inhoudsindicatie_df, hasVersion_df
 
         rsm_df['ecli'] = ecli_df
```

### Comparing `rechtspraak_extractor-1.1.8/rechtspraak_extractor.egg-info/PKG-INFO` & `rechtspraak_extractor-1.1.9/rechtspraak_extractor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: rechtspraak-extractor
-Version: 1.1.8
+Version: 1.1.9
 Summary: Library for extracting rechtspraak data
-Home-page: UNKNOWN
 Author: LawTech Lab
 Author-email: pranav.bapat@student.maastrichtuniversity.nl
 License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/extraction_libraries
 Project-URL: Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: rechtspraak,extractor,rechtspraak extractor
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 ## Rechtspraak extractor
 This library contains two functions to get rechtspraak data and metadata from the API.
 
 ## Version
 Python 3.9
@@ -167,9 +165,7 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 ```
-
-
```

#### html2text {}

```diff
@@ -1,17 +1,16 @@
-Metadata-Version: 2.1 Name: rechtspraak-extractor Version: 1.1.8 Summary:
-Library for extracting rechtspraak data Home-page: UNKNOWN Author: LawTech Lab
-Author-email: pranav.bapat@student.maastrichtuniversity.nl License: MIT
-Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/
-extraction_libraries Project-URL: Build Source, https://github.com/
-maastrichtlawtech/extraction_libraries Keywords:
-rechtspraak,extractor,rechtspraak extractor Platform: UNKNOWN Description-
-Content-Type: text/markdown ## Rechtspraak extractor This library contains two
-functions to get rechtspraak data and metadata from the API. ## Version Python
-3.9 ## Contributors
+Metadata-Version: 2.1 Name: rechtspraak-extractor Version: 1.1.9 Summary:
+Library for extracting rechtspraak data Author: LawTech Lab Author-email:
+pranav.bapat@student.maastrichtuniversity.nl License: MIT Project-URL: Bug
+Tracker, https://github.com/maastrichtlawtech/extraction_libraries Project-URL:
+Build Source, https://github.com/maastrichtlawtech/extraction_libraries
+Keywords: rechtspraak,extractor,rechtspraak extractor Description-Content-Type:
+text/markdown ## Rechtspraak extractor This library contains two functions to
+get rechtspraak data and metadata from the API. ## Version Python 3.9 ##
+Contributors
 [pranavnbapat]_ [running-machin]_    [Cloud956]_    [shashankmc]_ [gijsvd]_
  Pranav_Bapat    running-machin   Piotr_Lewandowski  shashankmc    gijsvd
  ## How to install? pip install rechtspraak_extractor ## What are the
 functions?
 Rechtspraak Extractor
    1. get_rechtspraak
    2. Gets all the ECLIs and saves them in the CSV file or in-memory.
```

### Comparing `rechtspraak_extractor-1.1.8/setup.py` & `rechtspraak_extractor-1.1.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 
 p = Path("README.md")
 long_descr = p.read_text()
 
 setup(
     name='rechtspraak_extractor',
     packages=find_packages(include=['rechtspraak_extractor']),
-    version='1.1.8',
+    version='1.1.9',
     description='Library for extracting rechtspraak data',
     author='LawTech Lab',
     license='MIT',
-    install_requires=['bs4', 'lxml==4.6.3', 'requests==2.26.0', 'xmltodict==0.13.0', 'python_dotenv==0.15.0', 'pandas'],
+    install_requires=['bs4', 'lxml==4.6.3', 'requests==2.26.0', 'xmltodict==0.13.0', 'python_dotenv==0.15.0', 'pandas','tqdm'],
     author_email='pranav.bapat@student.maastrichtuniversity.nl',
     keywords=['rechtspraak', 'extractor', 'rechtspraak extractor'],
     long_description=long_descr,
     long_description_content_type='text/markdown',
     project_urls={
         "Bug Tracker": "https://github.com/maastrichtlawtech/extraction_libraries",
         "Build Source": "https://github.com/maastrichtlawtech/extraction_libraries",
```

