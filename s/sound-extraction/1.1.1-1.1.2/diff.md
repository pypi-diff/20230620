# Comparing `tmp/sound-extraction-1.1.1.tar.gz` & `tmp/sound-extraction-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sound-extraction-1.1.1.tar", last modified: Thu Jun 15 13:17:19 2023, max compression
+gzip compressed data, was "dist\sound-extraction-1.1.2.tar", last modified: Mon Jun 19 20:04:09 2023, max compression
```

## Comparing `sound-extraction-1.1.1.tar` & `sound-extraction-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 13:17:19.981634 sound-extraction-1.1.1/
--rw-rw-rw-   0        0        0     1087 2023-06-12 17:14:00.000000 sound-extraction-1.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0     6223 2023-06-15 13:17:19.979171 sound-extraction-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5717 2023-06-15 02:45:40.000000 sound-extraction-1.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-15 13:17:19.983633 sound-extraction-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1131 2023-06-15 13:17:07.000000 sound-extraction-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 13:17:19.968667 sound-extraction-1.1.1/sound_extraction.egg-info/
--rw-rw-rw-   0        0        0     6223 2023-06-15 13:17:19.000000 sound-extraction-1.1.1/sound_extraction.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-06-15 13:17:19.000000 sound-extraction-1.1.1/sound_extraction.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 13:17:19.000000 sound-extraction-1.1.1/sound_extraction.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-06-15 13:17:19.000000 sound-extraction-1.1.1/sound_extraction.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      153 2023-06-15 13:17:19.000000 sound-extraction-1.1.1/sound_extraction.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-15 13:17:19.000000 sound-extraction-1.1.1/sound_extraction.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-15 13:17:19.973654 sound-extraction-1.1.1/src/
--rw-rw-rw-   0        0        0    17950 2023-06-15 02:35:01.000000 sound-extraction-1.1.1/src/sound_extraction.py
+drwxrwxrwx   0        0        0        0 2023-06-19 20:04:09.809977 sound-extraction-1.1.2/
+-rw-rw-rw-   0        0        0     1087 2023-06-12 17:14:00.000000 sound-extraction-1.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     7109 2023-06-19 20:04:09.806985 sound-extraction-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6603 2023-06-19 19:59:46.000000 sound-extraction-1.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-19 20:04:09.809977 sound-extraction-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1131 2023-06-19 20:04:03.000000 sound-extraction-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 20:04:09.789434 sound-extraction-1.1.2/sound_extraction.egg-info/
+-rw-rw-rw-   0        0        0     7109 2023-06-19 20:04:09.000000 sound-extraction-1.1.2/sound_extraction.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2023-06-19 20:04:09.000000 sound-extraction-1.1.2/sound_extraction.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 20:04:09.000000 sound-extraction-1.1.2/sound_extraction.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-06-19 20:04:09.000000 sound-extraction-1.1.2/sound_extraction.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      153 2023-06-19 20:04:09.000000 sound-extraction-1.1.2/sound_extraction.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-19 20:04:09.000000 sound-extraction-1.1.2/sound_extraction.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 20:04:09.804990 sound-extraction-1.1.2/src/
+-rw-rw-rw-   0        0        0    18042 2023-06-19 20:03:52.000000 sound-extraction-1.1.2/src/sound_extraction.py
```

### Comparing `sound-extraction-1.1.1/LICENSE.txt` & `sound-extraction-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sound-extraction-1.1.1/PKG-INFO` & `sound-extraction-1.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,57 @@
-Metadata-Version: 2.1
-Name: sound-extraction
-Version: 1.1.1
-Home-page: https://github.com/prayagnshah/Sound-Extraction
-Author: Prayag Shah
-Author-email: prayagshah07@gmail.com
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # Audio-File Extraction
 
 ## About
 
 Use this tool to segment (i.e., clip or slice), copy, and extract short-duration recordings, from long-duration WAV or FLAC files. Segmenting audio files into smaller parts can make recordings compatible for certain analytical workflows and allow for easier manipulation and sharing. Segment and extracting recordings based on a list of recording start times (date times) and a desired duration. This allows for applications such as the extraction of stratified audio samples, among others.
 
-## Downloading the package from PyPI
+## Types of Installation
+
+1. Download the python package:
+    
+    `pip install sound-extraction`
+
+    a. After the installation you can use the following command to run the program or use `--help` to see the arguments list:
+
+    `sound-extraction -r "/path/to/original/audio/files" -o "/path/to/output/folder" -c "/path/to/csv/file" -s "site_name"`
+
+and then you can follow the instructions for the arguments mentioned below to run the program. [Python-Package](#Arguments) OR
 
-    pip install sound-extraction
+2. If you want to run the program thorugh Docker then follow the steps below: [Docker](#using-dockerfile) OR
 
-After downloading the package from PyPI, you can use the following command to run the program:
+3. If you want to run the program from the source files then follow the steps below: [Source-File](#setup).
 
-    sound-extraction -r "/path/to/original/audio/files" -o "/path/to/output/folder" -c "/path/to/csv/file" -s "site_name"
+<b>Note: You can use any one of the installation above to run the program.</b>
 
-Users can follow the same arguments and commands mentioned below to run the program. [Here](#usage)
+## Using Dockerfile
 
-- If you want to run the program from the source files then follow the steps below:
+1. Download the Docker application: [Docker](https://www.docker.com/products/docker-desktop).
+
+2. Download `Dockerfile` and `requirements.txt` files: [Docker-File](https://github.com/prayagnshah/Sound-Extraction/blob/main/Dockerfile) and [Requirements](https://github.com/prayagnshah/Sound-Extraction/blob/main/requirements.txt).
+
+3. Open the terminal and go to the directory where you have downloaded the `Dockerfile` and `requirements.txt` files. Run the following command:
+
+    `docker build -t sound-extraction .`
+    `docker run sound-extraction`
 
 ## Setup (Windows)
 
-Download Audio-File Extraction Files: [Sound-File Extraction](https://drive.google.com/file/d/1HX9Cz0I7uKsIPuhHCdB1lfCmbtFY_YxJ/view?usp=share_link)
+Download Audio-File Extraction Files: [Sound-File Extraction](https://github.com/prayagnshah/Sound-Extraction/archive/refs/tags/v1.1.1.zip)
 
     python -m venv venv
     venv\Scripts\Activate
     pip install -r requirements.txt
 
 If creating virtual environment gives us an error then open the Powershell with <b>administrator</b> and run the following command:
 
     Set-ExecutionPolicy Unrestricted
 
 ## Setup (Linux)
 
-Download Audio-File Extraction Files: [Sound-File Extraction](https://drive.google.com/file/d/1HX9Cz0I7uKsIPuhHCdB1lfCmbtFY_YxJ/view?usp=share_link)
+Download Audio-File Extraction Files: [Sound-File Extraction](https://github.com/prayagnshah/Sound-Extraction/archive/refs/tags/v1.1.1.zip)
 
     python -m venv venv
     source venv/bin/activate
     pip install -r requirements.txt
 
 ## Test Files Usage
 
@@ -66,36 +69,38 @@
 
 2.  Run sound_extraction.py to get the sliced audio files which can handle around 192K sample rate. Here is an example:
 
     `python sound_extraction.py -r "/path/to/original/audio/files" -o "/path/to/output/folder" -slice 10`
 
 Arguments and commands used are required to get the slicing of larger audio files into smaller audio files of your choice.
 
+## Arguments
+
 Here's a complete list of all command line arguments:
 
     -r, Path to original audio files (required). Need to make sure all the audio files are stored in a folder.
     -o, Path to output folder (required). Program will create a folder for you with current time, name of site and extraction of duration to the specified path.
-    -c, Path to the CSV file with the following requirements: Header should include "sample file" and "categories" columns. The "sample file" column should be in the format 20220608_170343, and the "categories" column should contain categories such as "Nocturnal", etc.
+    -c, Path to the CSV file with the following requirements: Header should include "sample file" and "category" columns. The "sample file" column should be in the format 20220608_170343, and the "category" column should contain categories such as "Nocturnal", etc.
     -s, Prefix or the recording name, or ID, etc. This will be used to name the extracted audio files.
     -d, Duration of the extracted audio file. Change the duration of the extracted audio files, if required. Default is 3 minutes.
     -span, Span of the audio file. Extracted audio files will not span to 3 minutes if the original file is shorter.
     -e, Extension of the audio file (.wav or .flac). If your original audio files are flac then you need to use ".wav". Default is flac.
     -slice, Slice the audio file in smaller segments/chunks. Default is 10 seconds.
 
 We can see the arguments list by using the following command:
 
     python sound_extraction.py -h
 
-3. This is very basic version of the analysis of the workflow, you can adjust it to your needs.
+1. This is very basic version of the analysis of the workflow, you can adjust it to your needs.
 
-4. All the unusual files are handled and will show in console as a log message.
+2. All the unusual files are handled and will show in console as a log message.
 
-5. Please open an issue if you have any questions or suggestions to add any features.
+3. Please open an issue if you have any questions or suggestions to add any features.
 
-6. I will keep on updating the code and making it more efficient.
+4. I will keep on updating the code and making it more efficient.
 
 ## Error Handling
 
 1. Log file will be created in the output folder with the name of `sound_extraction_logs.txt` which will show all the corrupted files which happened during the extraction process.
 
 2. This program will send the error message to the Sentry server to improve the user performace and to keep track of the errors which will be handled by myself.
```

### Comparing `sound-extraction-1.1.1/README.md` & `sound-extraction-1.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,71 @@
+Metadata-Version: 2.1
+Name: sound-extraction
+Version: 1.1.2
+Home-page: https://github.com/prayagnshah/Sound-Extraction
+Author: Prayag Shah
+Author-email: prayagshah07@gmail.com
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # Audio-File Extraction
 
 ## About
 
 Use this tool to segment (i.e., clip or slice), copy, and extract short-duration recordings, from long-duration WAV or FLAC files. Segmenting audio files into smaller parts can make recordings compatible for certain analytical workflows and allow for easier manipulation and sharing. Segment and extracting recordings based on a list of recording start times (date times) and a desired duration. This allows for applications such as the extraction of stratified audio samples, among others.
 
-## Downloading the package from PyPI
+## Types of Installation
+
+1. Download the python package:
+    
+    `pip install sound-extraction`
+
+    a. After the installation you can use the following command to run the program or use `--help` to see the arguments list:
+
+    `sound-extraction -r "/path/to/original/audio/files" -o "/path/to/output/folder" -c "/path/to/csv/file" -s "site_name"`
+
+and then you can follow the instructions for the arguments mentioned below to run the program. [Python-Package](#Arguments) OR
 
-    pip install sound-extraction
+2. If you want to run the program thorugh Docker then follow the steps below: [Docker](#using-dockerfile) OR
 
-After downloading the package from PyPI, you can use the following command to run the program:
+3. If you want to run the program from the source files then follow the steps below: [Source-File](#setup).
 
-    sound-extraction -r "/path/to/original/audio/files" -o "/path/to/output/folder" -c "/path/to/csv/file" -s "site_name"
+<b>Note: You can use any one of the installation above to run the program.</b>
 
-Users can follow the same arguments and commands mentioned below to run the program. [Here](#usage)
+## Using Dockerfile
 
-- If you want to run the program from the source files then follow the steps below:
+1. Download the Docker application: [Docker](https://www.docker.com/products/docker-desktop).
+
+2. Download `Dockerfile` and `requirements.txt` files: [Docker-File](https://github.com/prayagnshah/Sound-Extraction/blob/main/Dockerfile) and [Requirements](https://github.com/prayagnshah/Sound-Extraction/blob/main/requirements.txt).
+
+3. Open the terminal and go to the directory where you have downloaded the `Dockerfile` and `requirements.txt` files. Run the following command:
+
+    `docker build -t sound-extraction .`
+    `docker run sound-extraction`
 
 ## Setup (Windows)
 
-Download Audio-File Extraction Files: [Sound-File Extraction](https://drive.google.com/file/d/1HX9Cz0I7uKsIPuhHCdB1lfCmbtFY_YxJ/view?usp=share_link)
+Download Audio-File Extraction Files: [Sound-File Extraction](https://github.com/prayagnshah/Sound-Extraction/archive/refs/tags/v1.1.1.zip)
 
     python -m venv venv
     venv\Scripts\Activate
     pip install -r requirements.txt
 
 If creating virtual environment gives us an error then open the Powershell with <b>administrator</b> and run the following command:
 
     Set-ExecutionPolicy Unrestricted
 
 ## Setup (Linux)
 
-Download Audio-File Extraction Files: [Sound-File Extraction](https://drive.google.com/file/d/1HX9Cz0I7uKsIPuhHCdB1lfCmbtFY_YxJ/view?usp=share_link)
+Download Audio-File Extraction Files: [Sound-File Extraction](https://github.com/prayagnshah/Sound-Extraction/archive/refs/tags/v1.1.1.zip)
 
     python -m venv venv
     source venv/bin/activate
     pip install -r requirements.txt
 
 ## Test Files Usage
 
@@ -52,36 +83,38 @@
 
 2.  Run sound_extraction.py to get the sliced audio files which can handle around 192K sample rate. Here is an example:
 
     `python sound_extraction.py -r "/path/to/original/audio/files" -o "/path/to/output/folder" -slice 10`
 
 Arguments and commands used are required to get the slicing of larger audio files into smaller audio files of your choice.
 
+## Arguments
+
 Here's a complete list of all command line arguments:
 
     -r, Path to original audio files (required). Need to make sure all the audio files are stored in a folder.
     -o, Path to output folder (required). Program will create a folder for you with current time, name of site and extraction of duration to the specified path.
-    -c, Path to the CSV file with the following requirements: Header should include "sample file" and "categories" columns. The "sample file" column should be in the format 20220608_170343, and the "categories" column should contain categories such as "Nocturnal", etc.
+    -c, Path to the CSV file with the following requirements: Header should include "sample file" and "category" columns. The "sample file" column should be in the format 20220608_170343, and the "category" column should contain categories such as "Nocturnal", etc.
     -s, Prefix or the recording name, or ID, etc. This will be used to name the extracted audio files.
     -d, Duration of the extracted audio file. Change the duration of the extracted audio files, if required. Default is 3 minutes.
     -span, Span of the audio file. Extracted audio files will not span to 3 minutes if the original file is shorter.
     -e, Extension of the audio file (.wav or .flac). If your original audio files are flac then you need to use ".wav". Default is flac.
     -slice, Slice the audio file in smaller segments/chunks. Default is 10 seconds.
 
 We can see the arguments list by using the following command:
 
     python sound_extraction.py -h
 
-3. This is very basic version of the analysis of the workflow, you can adjust it to your needs.
+1. This is very basic version of the analysis of the workflow, you can adjust it to your needs.
 
-4. All the unusual files are handled and will show in console as a log message.
+2. All the unusual files are handled and will show in console as a log message.
 
-5. Please open an issue if you have any questions or suggestions to add any features.
+3. Please open an issue if you have any questions or suggestions to add any features.
 
-6. I will keep on updating the code and making it more efficient.
+4. I will keep on updating the code and making it more efficient.
 
 ## Error Handling
 
 1. Log file will be created in the output folder with the name of `sound_extraction_logs.txt` which will show all the corrupted files which happened during the extraction process.
 
 2. This program will send the error message to the Sentry server to improve the user performace and to keep track of the errors which will be handled by myself.
```

### Comparing `sound-extraction-1.1.1/setup.py` & `sound-extraction-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="sound-extraction",
-    version="1.1.1",
+    version="1.1.2",
     packages=["src"],
     install_requires=[
         "certifi==2023.5.7",
         "cffi==1.15.1",
         "load-dotenv==0.1.0",
         "numpy==1.24.3",
         "pycparser==2.21",
```

### Comparing `sound-extraction-1.1.1/sound_extraction.egg-info/PKG-INFO` & `sound-extraction-1.1.2/sound_extraction.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sound-extraction
-Version: 1.1.1
+Version: 1.1.2
 Home-page: https://github.com/prayagnshah/Sound-Extraction
 Author: Prayag Shah
 Author-email: prayagshah07@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
@@ -14,41 +14,58 @@
 
 # Audio-File Extraction
 
 ## About
 
 Use this tool to segment (i.e., clip or slice), copy, and extract short-duration recordings, from long-duration WAV or FLAC files. Segmenting audio files into smaller parts can make recordings compatible for certain analytical workflows and allow for easier manipulation and sharing. Segment and extracting recordings based on a list of recording start times (date times) and a desired duration. This allows for applications such as the extraction of stratified audio samples, among others.
 
-## Downloading the package from PyPI
+## Types of Installation
 
-    pip install sound-extraction
+1. Download the python package:
+    
+    `pip install sound-extraction`
 
-After downloading the package from PyPI, you can use the following command to run the program:
+    a. After the installation you can use the following command to run the program or use `--help` to see the arguments list:
 
-    sound-extraction -r "/path/to/original/audio/files" -o "/path/to/output/folder" -c "/path/to/csv/file" -s "site_name"
+    `sound-extraction -r "/path/to/original/audio/files" -o "/path/to/output/folder" -c "/path/to/csv/file" -s "site_name"`
 
-Users can follow the same arguments and commands mentioned below to run the program. [Here](#usage)
+and then you can follow the instructions for the arguments mentioned below to run the program. [Python-Package](#Arguments) OR
 
-- If you want to run the program from the source files then follow the steps below:
+2. If you want to run the program thorugh Docker then follow the steps below: [Docker](#using-dockerfile) OR
+
+3. If you want to run the program from the source files then follow the steps below: [Source-File](#setup).
+
+<b>Note: You can use any one of the installation above to run the program.</b>
+
+## Using Dockerfile
+
+1. Download the Docker application: [Docker](https://www.docker.com/products/docker-desktop).
+
+2. Download `Dockerfile` and `requirements.txt` files: [Docker-File](https://github.com/prayagnshah/Sound-Extraction/blob/main/Dockerfile) and [Requirements](https://github.com/prayagnshah/Sound-Extraction/blob/main/requirements.txt).
+
+3. Open the terminal and go to the directory where you have downloaded the `Dockerfile` and `requirements.txt` files. Run the following command:
+
+    `docker build -t sound-extraction .`
+    `docker run sound-extraction`
 
 ## Setup (Windows)
 
-Download Audio-File Extraction Files: [Sound-File Extraction](https://drive.google.com/file/d/1HX9Cz0I7uKsIPuhHCdB1lfCmbtFY_YxJ/view?usp=share_link)
+Download Audio-File Extraction Files: [Sound-File Extraction](https://github.com/prayagnshah/Sound-Extraction/archive/refs/tags/v1.1.1.zip)
 
     python -m venv venv
     venv\Scripts\Activate
     pip install -r requirements.txt
 
 If creating virtual environment gives us an error then open the Powershell with <b>administrator</b> and run the following command:
 
     Set-ExecutionPolicy Unrestricted
 
 ## Setup (Linux)
 
-Download Audio-File Extraction Files: [Sound-File Extraction](https://drive.google.com/file/d/1HX9Cz0I7uKsIPuhHCdB1lfCmbtFY_YxJ/view?usp=share_link)
+Download Audio-File Extraction Files: [Sound-File Extraction](https://github.com/prayagnshah/Sound-Extraction/archive/refs/tags/v1.1.1.zip)
 
     python -m venv venv
     source venv/bin/activate
     pip install -r requirements.txt
 
 ## Test Files Usage
 
@@ -66,36 +83,38 @@
 
 2.  Run sound_extraction.py to get the sliced audio files which can handle around 192K sample rate. Here is an example:
 
     `python sound_extraction.py -r "/path/to/original/audio/files" -o "/path/to/output/folder" -slice 10`
 
 Arguments and commands used are required to get the slicing of larger audio files into smaller audio files of your choice.
 
+## Arguments
+
 Here's a complete list of all command line arguments:
 
     -r, Path to original audio files (required). Need to make sure all the audio files are stored in a folder.
     -o, Path to output folder (required). Program will create a folder for you with current time, name of site and extraction of duration to the specified path.
-    -c, Path to the CSV file with the following requirements: Header should include "sample file" and "categories" columns. The "sample file" column should be in the format 20220608_170343, and the "categories" column should contain categories such as "Nocturnal", etc.
+    -c, Path to the CSV file with the following requirements: Header should include "sample file" and "category" columns. The "sample file" column should be in the format 20220608_170343, and the "category" column should contain categories such as "Nocturnal", etc.
     -s, Prefix or the recording name, or ID, etc. This will be used to name the extracted audio files.
     -d, Duration of the extracted audio file. Change the duration of the extracted audio files, if required. Default is 3 minutes.
     -span, Span of the audio file. Extracted audio files will not span to 3 minutes if the original file is shorter.
     -e, Extension of the audio file (.wav or .flac). If your original audio files are flac then you need to use ".wav". Default is flac.
     -slice, Slice the audio file in smaller segments/chunks. Default is 10 seconds.
 
 We can see the arguments list by using the following command:
 
     python sound_extraction.py -h
 
-3. This is very basic version of the analysis of the workflow, you can adjust it to your needs.
+1. This is very basic version of the analysis of the workflow, you can adjust it to your needs.
 
-4. All the unusual files are handled and will show in console as a log message.
+2. All the unusual files are handled and will show in console as a log message.
 
-5. Please open an issue if you have any questions or suggestions to add any features.
+3. Please open an issue if you have any questions or suggestions to add any features.
 
-6. I will keep on updating the code and making it more efficient.
+4. I will keep on updating the code and making it more efficient.
 
 ## Error Handling
 
 1. Log file will be created in the output folder with the name of `sound_extraction_logs.txt` which will show all the corrupted files which happened during the extraction process.
 
 2. This program will send the error message to the Sentry server to improve the user performace and to keep track of the errors which will be handled by myself.
```

### Comparing `sound-extraction-1.1.1/src/sound_extraction.py` & `sound-extraction-1.1.2/src/sound_extraction.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 load_dotenv()
 
 # Get the sentry DSN from the environment variables
 sentry_dsn = os.getenv("sentry_dsn")
 
 sentry_sdk.init(
     dsn=sentry_dsn,
-    release="v1.0.2",
+    release="v1.1.2",
     # Set traces_sample_rate to 1.0 to capture 100%
     # of transactions for performance monitoring.
     traces_sample_rate=1.0,
 )
 
 
 def main():
@@ -59,15 +59,17 @@
 
             sampleFile_index = header.index(sampleFile)
 
             # Checking if the categories column is present in the CSV file
 
             categories_bool = False
             if categories_col not in header:
-                logging.info("Categories column not found in CSV file")
+                logging.info(
+                    "Categories column not found in CSV file, so there is no folder named Nocturnal, Daytime, etc."
+                )
 
                 categories_bool = True
 
             else:
                 categories_index = header.index(categories_col)
 
             # storing the values in list so that it can be used once the file is closed
@@ -438,15 +440,15 @@
 
     else:
         # Calling the functions
 
         directory, all_files = get_directories(root_directory)
 
         sampleFile = "sampleFile"
-        categories_col = "Categories"
+        categories_col = "category"
         sample_recordings, categories_dict = read_csv_file(
             csv_file_path, sampleFile, categories_col
         )
 
         filtered_recordings_dict = process_recordings(all_files, sample_recordings)
 
         export_segment, output_directory = extract_audio_segments(
```

