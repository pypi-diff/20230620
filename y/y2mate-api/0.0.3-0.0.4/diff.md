# Comparing `tmp/y2mate-api-0.0.3.tar.gz` & `tmp/y2mate-api-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "y2mate-api-0.0.3.tar", last modified: Sat Jun 17 22:05:25 2023, max compression
+gzip compressed data, was "y2mate-api-0.0.4.tar", last modified: Tue Jun 20 11:15:14 2023, max compression
```

## Comparing `y2mate-api-0.0.3.tar` & `y2mate-api-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-17 22:05:25.679842 y2mate-api-0.0.3/
--rw-rw----   0 root         (0) everybody  (9997)     1064 2023-06-16 15:42:28.000000 y2mate-api-0.0.3/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)    10355 2023-06-17 22:05:25.663842 y2mate-api-0.0.3/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     9260 2023-06-17 22:05:02.000000 y2mate-api-0.0.3/README.md
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-17 22:05:25.679842 y2mate-api-0.0.3/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     1535 2023-06-17 16:53:45.000000 y2mate-api-0.0.3/setup.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-17 22:05:25.283842 y2mate-api-0.0.3/tests/
--rw-rw----   0 root         (0) everybody  (9997)      255 2023-06-15 19:45:34.000000 y2mate-api-0.0.3/tests/test.py
--rw-rw----   0 root         (0) everybody  (9997)      267 2023-06-15 19:39:07.000000 y2mate-api-0.0.3/tests/test_1.py
--rw-rw----   0 root         (0) everybody  (9997)      261 2023-06-15 20:21:38.000000 y2mate-api-0.0.3/tests/test_3.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-17 22:05:25.399842 y2mate-api-0.0.3/y2mate_api/
--rw-rw----   0 root         (0) everybody  (9997)      490 2023-06-17 16:27:02.000000 y2mate-api-0.0.3/y2mate_api/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     5072 2023-06-17 18:18:06.000000 y2mate-api-0.0.3/y2mate_api/console.py
--rw-rw----   0 root         (0) everybody  (9997)    13244 2023-06-17 21:46:43.000000 y2mate-api-0.0.3/y2mate_api/downloader.py
--rw-rw----   0 root         (0) everybody  (9997)    14839 2023-06-17 19:43:50.000000 y2mate-api-0.0.3/y2mate_api/main.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-17 22:05:25.643842 y2mate-api-0.0.3/y2mate_api.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)    10355 2023-06-17 22:05:24.000000 y2mate-api-0.0.3/y2mate_api.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      367 2023-06-17 22:05:24.000000 y2mate-api-0.0.3/y2mate_api.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-17 22:05:24.000000 y2mate-api-0.0.3/y2mate_api.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       51 2023-06-17 22:05:24.000000 y2mate-api-0.0.3/y2mate_api.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)       85 2023-06-17 22:05:24.000000 y2mate-api-0.0.3/y2mate_api.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)       11 2023-06-17 22:05:24.000000 y2mate-api-0.0.3/y2mate_api.egg-info/top_level.txt
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-20 11:15:14.210421 y2mate-api-0.0.4/
+-rw-rw----   0 root         (0) everybody  (9997)     1064 2023-06-16 15:42:28.000000 y2mate-api-0.0.4/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)    10845 2023-06-20 11:15:14.190421 y2mate-api-0.0.4/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     9750 2023-06-20 11:11:01.000000 y2mate-api-0.0.4/README.md
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-20 11:15:14.214421 y2mate-api-0.0.4/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1535 2023-06-17 16:53:45.000000 y2mate-api-0.0.4/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-20 11:15:13.774421 y2mate-api-0.0.4/tests/
+-rw-rw----   0 root         (0) everybody  (9997)      255 2023-06-15 19:45:34.000000 y2mate-api-0.0.4/tests/test.py
+-rw-rw----   0 root         (0) everybody  (9997)      267 2023-06-15 19:39:07.000000 y2mate-api-0.0.4/tests/test_1.py
+-rw-rw----   0 root         (0) everybody  (9997)      261 2023-06-15 20:21:38.000000 y2mate-api-0.0.4/tests/test_3.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-20 11:15:13.974421 y2mate-api-0.0.4/y2mate_api/
+-rw-rw----   0 root         (0) everybody  (9997)      490 2023-06-19 17:39:27.000000 y2mate-api-0.0.4/y2mate_api/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)       34 2023-06-19 18:39:03.000000 y2mate-api-0.0.4/y2mate_api/__main__.py
+-rw-rw----   0 root         (0) everybody  (9997)     5333 2023-06-19 18:27:02.000000 y2mate-api-0.0.4/y2mate_api/console.py
+-rw-rw----   0 root         (0) everybody  (9997)    13935 2023-06-19 18:39:05.000000 y2mate-api-0.0.4/y2mate_api/downloader.py
+-rw-rw----   0 root         (0) everybody  (9997)    14849 2023-06-19 13:09:05.000000 y2mate-api-0.0.4/y2mate_api/main.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-20 11:15:14.174421 y2mate-api-0.0.4/y2mate_api.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)    10845 2023-06-20 11:15:12.000000 y2mate-api-0.0.4/y2mate_api.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      390 2023-06-20 11:15:12.000000 y2mate-api-0.0.4/y2mate_api.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-20 11:15:12.000000 y2mate-api-0.0.4/y2mate_api.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       51 2023-06-20 11:15:12.000000 y2mate-api-0.0.4/y2mate_api.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)       85 2023-06-20 11:15:12.000000 y2mate-api-0.0.4/y2mate_api.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)       11 2023-06-20 11:15:12.000000 y2mate-api-0.0.4/y2mate_api.egg-info/top_level.txt
```

### Comparing `y2mate-api-0.0.3/LICENSE` & `y2mate-api-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `y2mate-api-0.0.3/PKG-INFO` & `y2mate-api-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: y2mate-api
-Version: 0.0.3
+Version: 0.0.4
 Summary: Download youtube videos and audios by title or link
 Home-page: https://github.com/Simatwa/y2mate-api
 Author: Smartwa
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/y2mate-api/issues/new
@@ -27,15 +27,15 @@
 License-File: LICENSE
 
 # y2mate-api
 
 <p align="center">
 <a href="https://github.com/Simatwa/y2mate-api"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a>
 <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
-<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.3&color=green"/></a>
+<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.4&color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>
 <a href="https://pepy.tech/project/livescore-api"><img src="https://static.pepy.tech/personalized-badge/y2mate-api?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a>
 </p>
 
@@ -155,14 +155,15 @@
 ## Other parameters
 
 - `Handler`
   * author : Video author i.e Youtube Channel
   * timeout : http requests timeout
   * ask : Confirm before downloading media
   * unique : Auto-ignore previously downloaded media
+  * thread : Download (x) value of file at a time.
 
 - `Handler.run`
   * format : Media format mp4/mp3
   * quality : Media qualiy such as 720p/128kbps
   * resolver : Additional format info : [m4a,3gp,mp4,mp3]
   * limit : Total videos to be retrieved
   * keyword : Phrase(s) that must be in media title
@@ -172,74 +173,85 @@
   * dir : Path to Directory for saving the media files
   * iterator : Function that yields third_query object - `Handler.run`
   * progress_bar : Stdout media-name & Display progress bar
  
 - `Handler.save`
   * third_dict : Response of `third_query.run()`
   * dir : Directory for saving the contents
-  * progress_bar : Stdout media-name & Display download progress bar
+  * progress_bar : Display download progress bar
+  * quiet : Not to stdout anything
+  * naming_format : Format for generating media filename using the `third_query` response keys
  
 </details>
  
 <details>
 <summary>
 	
 For more info run `$ y2mate -h`
 
 </summary>
 
 ```
-usage: y2mate [-h] [-v] [-f mp4|mp3]
+usage: y2mate [-h] [-v] [-f mp3|mp4]
               [-q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps]
               [-r m4a|3gp|mp4|mp3] [-k [KEYWORD ...]]
               [-a [AUTHOR ...]] [-l LIMIT] [-d PATH]
-              [-t TIMEOUT] [-i PATH] [-thr THREAD]
-              [--disable-bar] [--ask] [--unique] [--quiet]
-              [--history] [--clear]
+              [-t TIMEOUT] [-i PATH] [-o FORMAT]
+              [-thr THREAD] [--disable-bar] [--ask]
+              [--unique] [--quiet] [--history] [--clear]
               [query ...]
 
 Download youtube videos and audios by title or link
 
 positional arguments:
-  query                 Youtube video title, link or id - None
+  query                 Youtube video title, link or id -
+                        None
 
 options:
   -h, --help            show this help message and exit
-  -v, --version         show program's version number and exit
-  -f mp4|mp3, --format mp4|mp3
+  -v, --version         show program's version number and
+                        exit
+  -f mp3|mp4, --format mp3|mp4
                         Specify media type - audio/video
   -q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps, --quality 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps
                         Media quality -720p
   -r m4a|3gp|mp4|mp3, --resolver m4a|3gp|mp4|mp3
-                        Other media formats incase of multiple
-                        options - mp4/mp3
+                        Other media formats incase of
+                        multiple options - mp4/mp3
   -k [KEYWORD ...], --keyword [KEYWORD ...]
                         Media should contain this keywords -
                         None
   -a [AUTHOR ...], --author [AUTHOR ...]
-                        Media author i.e YouTube channel name -
-                        None
+                        Media author i.e YouTube channel
+                        name - None
   -l LIMIT, --limit LIMIT
                         Total videos to be downloaded - 1
   -d PATH, --dir PATH   Directory for saving the contents -
-                        /storage/emulated/0/git/Smartwa
+                        /storage/emulated/0/git/Smartwa/y2ma
+                        te-api
   -t TIMEOUT, --timeout TIMEOUT
-                        Http request timeout - 30s
+                        Http request timeout in seconds - 30
   -i PATH, --input PATH
-                        Path to text file containing query per
-                        line - None
+                        Path to text file containing query
+                        per line - None
+  -o FORMAT, --output FORMAT
+                        Format for generating filename
+                        %(key)s : [title,vid,fquality,ftype]
+                        - None
   -thr THREAD, --thread THREAD
-                        Download [x] amount of videos/audios at
-                        once - 1
-  --disable-bar         Disables download progress bar - False
-  --ask                 Confirm before downloading file - False
+                        Download [x] amount of videos/audios
+                        at once - 1
+  --disable-bar         Disable download progress bar -
+                        False
+  --ask                 Confirm before downloading file -
+                        False
   --unique              Auto-skip any media that you once
                         dowloaded - False
-  --quiet               Not to stdout anything other than logs -
-                        False
+  --quiet               Not to stdout anything other than
+                        logs - False
   --history             Stdout all media metadata ever
                         downloaded - False
   --clear               Clear all download histories - False
 
 This script has no official relation with y2mate.com
 ```
 </details>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: y2mate-api Version: 0.0.3 Summary: Download youtube
+Metadata-Version: 2.1 Name: y2mate-api Version: 0.0.4 Summary: Download youtube
 videos and audios by title or link Home-page: https://github.com/Simatwa/
 y2mate-api Author: Smartwa Author-email: smartwacaleb@gmail.com Maintainer:
 Smartwa License: MIT Project-URL: Bug Report, https://github.com/Simatwa/
 y2mate-api/issues/new Keywords: y2mate,videos,video-api,youtube Classifier:
 License :: OSI Approved :: MIT License Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: License :: Free For Home Use Classifier: Intended
@@ -53,50 +53,52 @@
 as well specify total videos to be downloaded by using `limit` argument. For
 instance: ```py from y2mate_api import Handler api = Handler("https://youtu.be/
 POPoAjWFkGg") api.auto_save(limit=10) # This will download the video in path
 and 9 other videos related to the query specified ``` **Note** : You can still
 use **video id** such as `POPoAjWFkGg` as query parameter. ## Other parameters
 - `Handler` * author : Video author i.e Youtube Channel * timeout : http
 requests timeout * ask : Confirm before downloading media * unique : Auto-
-ignore previously downloaded media - `Handler.run` * format : Media format mp4/
-mp3 * quality : Media qualiy such as 720p/128kbps * resolver : Additional
-format info : [m4a,3gp,mp4,mp3] * limit : Total videos to be retrieved *
-keyword : Phrase(s) that must be in media title * author : Video author i.e
-Youtube Channel - `Handler.auto_save` * dir : Path to Directory for saving the
-media files * iterator : Function that yields third_query object -
-`Handler.run` * progress_bar : Stdout media-name & Display progress bar -
-`Handler.save` * third_dict : Response of `third_query.run()` * dir : Directory
-for saving the contents * progress_bar : Stdout media-name & Display download
-progress bar    For more info run `$ y2mate -h`  ``` usage: y2mate [-h] [-v] [-
-f mp4|mp3] [-
+ignore previously downloaded media * thread : Download (x) value of file at a
+time. - `Handler.run` * format : Media format mp4/mp3 * quality : Media qualiy
+such as 720p/128kbps * resolver : Additional format info : [m4a,3gp,mp4,mp3] *
+limit : Total videos to be retrieved * keyword : Phrase(s) that must be in
+media title * author : Video author i.e Youtube Channel - `Handler.auto_save` *
+dir : Path to Directory for saving the media files * iterator : Function that
+yields third_query object - `Handler.run` * progress_bar : Stdout media-name &
+Display progress bar - `Handler.save` * third_dict : Response of
+`third_query.run()` * dir : Directory for saving the contents * progress_bar :
+Display download progress bar * quiet : Not to stdout anything * naming_format
+: Format for generating media filename using the `third_query` response keys
+For more info run `$ y2mate -h`  ``` usage: y2mate [-h] [-v] [-f mp3|mp4] [-
 q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps]
 [-r m4a|3gp|mp4|mp3] [-k [KEYWORD ...]] [-a [AUTHOR ...]] [-l LIMIT] [-d PATH]
-[-t TIMEOUT] [-i PATH] [-thr THREAD] [--disable-bar] [--ask] [--unique] [--
-quiet] [--history] [--clear] [query ...] Download youtube videos and audios by
-title or link positional arguments: query Youtube video title, link or id -
-None options: -h, --help show this help message and exit -v, --version show
-program's version number and exit -f mp4|mp3, --format mp4|mp3 Specify media
-type - audio/video -
+[-t TIMEOUT] [-i PATH] [-o FORMAT] [-thr THREAD] [--disable-bar] [--ask] [--
+unique] [--quiet] [--history] [--clear] [query ...] Download youtube videos and
+audios by title or link positional arguments: query Youtube video title, link
+or id - None options: -h, --help show this help message and exit -v, --version
+show program's version number and exit -f mp3|mp4, --format mp3|mp4 Specify
+media type - audio/video -
 q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps,
 --quality
 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps
 Media quality -720p -r m4a|3gp|mp4|mp3, --resolver m4a|3gp|mp4|mp3 Other media
 formats incase of multiple options - mp4/mp3 -k [KEYWORD ...], --keyword
 [KEYWORD ...] Media should contain this keywords - None -a [AUTHOR ...], --
 author [AUTHOR ...] Media author i.e YouTube channel name - None -l LIMIT, --
 limit LIMIT Total videos to be downloaded - 1 -d PATH, --dir PATH Directory for
-saving the contents - /storage/emulated/0/git/Smartwa -t TIMEOUT, --timeout
-TIMEOUT Http request timeout - 30s -i PATH, --input PATH Path to text file
-containing query per line - None -thr THREAD, --thread THREAD Download [x]
-amount of videos/audios at once - 1 --disable-bar Disables download progress
-bar - False --ask Confirm before downloading file - False --unique Auto-skip
-any media that you once dowloaded - False --quiet Not to stdout anything other
-than logs - False --history Stdout all media metadata ever downloaded - False -
--clear Clear all download histories - False This script has no official
-relation with y2mate.com ```  - Review [CHANGELOG](https://github.com/Simatwa/
-y2mate-api/blob/main/Docs/CHANGELOG.md) for latest updates. ## Disclaimer This
-repository is intended for educational and personal use only. The use of this
-repository for any commercial or illegal purposes is strictly prohibited. The
-repository owner does not endorse or encourage the downloading or sharing of
-copyrighted material without permission. The repository owner is not
-responsible for any misuse of the software or any legal consequences that may
-arise from such misuse.
+saving the contents - /storage/emulated/0/git/Smartwa/y2ma te-api -t TIMEOUT, -
+-timeout TIMEOUT Http request timeout in seconds - 30 -i PATH, --input PATH
+Path to text file containing query per line - None -o FORMAT, --output FORMAT
+Format for generating filename %(key)s : [title,vid,fquality,ftype] - None -thr
+THREAD, --thread THREAD Download [x] amount of videos/audios at once - 1 --
+disable-bar Disable download progress bar - False --ask Confirm before
+downloading file - False --unique Auto-skip any media that you once dowloaded -
+False --quiet Not to stdout anything other than logs - False --history Stdout
+all media metadata ever downloaded - False --clear Clear all download histories
+- False This script has no official relation with y2mate.com ```  - Review
+[CHANGELOG](https://github.com/Simatwa/y2mate-api/blob/main/Docs/CHANGELOG.md)
+for latest updates. ## Disclaimer This repository is intended for educational
+and personal use only. The use of this repository for any commercial or illegal
+purposes is strictly prohibited. The repository owner does not endorse or
+encourage the downloading or sharing of copyrighted material without
+permission. The repository owner is not responsible for any misuse of the
+software or any legal consequences that may arise from such misuse.
```

### Comparing `y2mate-api-0.0.3/README.md` & `y2mate-api-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # y2mate-api
 
 <p align="center">
 <a href="https://github.com/Simatwa/y2mate-api"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a>
 <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
-<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.3&color=green"/></a>
+<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.4&color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>
 <a href="https://pepy.tech/project/livescore-api"><img src="https://static.pepy.tech/personalized-badge/y2mate-api?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a>
 </p>
 
@@ -127,14 +127,15 @@
 ## Other parameters
 
 - `Handler`
   * author : Video author i.e Youtube Channel
   * timeout : http requests timeout
   * ask : Confirm before downloading media
   * unique : Auto-ignore previously downloaded media
+  * thread : Download (x) value of file at a time.
 
 - `Handler.run`
   * format : Media format mp4/mp3
   * quality : Media qualiy such as 720p/128kbps
   * resolver : Additional format info : [m4a,3gp,mp4,mp3]
   * limit : Total videos to be retrieved
   * keyword : Phrase(s) that must be in media title
@@ -144,74 +145,85 @@
   * dir : Path to Directory for saving the media files
   * iterator : Function that yields third_query object - `Handler.run`
   * progress_bar : Stdout media-name & Display progress bar
  
 - `Handler.save`
   * third_dict : Response of `third_query.run()`
   * dir : Directory for saving the contents
-  * progress_bar : Stdout media-name & Display download progress bar
+  * progress_bar : Display download progress bar
+  * quiet : Not to stdout anything
+  * naming_format : Format for generating media filename using the `third_query` response keys
  
 </details>
  
 <details>
 <summary>
 	
 For more info run `$ y2mate -h`
 
 </summary>
 
 ```
-usage: y2mate [-h] [-v] [-f mp4|mp3]
+usage: y2mate [-h] [-v] [-f mp3|mp4]
               [-q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps]
               [-r m4a|3gp|mp4|mp3] [-k [KEYWORD ...]]
               [-a [AUTHOR ...]] [-l LIMIT] [-d PATH]
-              [-t TIMEOUT] [-i PATH] [-thr THREAD]
-              [--disable-bar] [--ask] [--unique] [--quiet]
-              [--history] [--clear]
+              [-t TIMEOUT] [-i PATH] [-o FORMAT]
+              [-thr THREAD] [--disable-bar] [--ask]
+              [--unique] [--quiet] [--history] [--clear]
               [query ...]
 
 Download youtube videos and audios by title or link
 
 positional arguments:
-  query                 Youtube video title, link or id - None
+  query                 Youtube video title, link or id -
+                        None
 
 options:
   -h, --help            show this help message and exit
-  -v, --version         show program's version number and exit
-  -f mp4|mp3, --format mp4|mp3
+  -v, --version         show program's version number and
+                        exit
+  -f mp3|mp4, --format mp3|mp4
                         Specify media type - audio/video
   -q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps, --quality 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps
                         Media quality -720p
   -r m4a|3gp|mp4|mp3, --resolver m4a|3gp|mp4|mp3
-                        Other media formats incase of multiple
-                        options - mp4/mp3
+                        Other media formats incase of
+                        multiple options - mp4/mp3
   -k [KEYWORD ...], --keyword [KEYWORD ...]
                         Media should contain this keywords -
                         None
   -a [AUTHOR ...], --author [AUTHOR ...]
-                        Media author i.e YouTube channel name -
-                        None
+                        Media author i.e YouTube channel
+                        name - None
   -l LIMIT, --limit LIMIT
                         Total videos to be downloaded - 1
   -d PATH, --dir PATH   Directory for saving the contents -
-                        /storage/emulated/0/git/Smartwa
+                        /storage/emulated/0/git/Smartwa/y2ma
+                        te-api
   -t TIMEOUT, --timeout TIMEOUT
-                        Http request timeout - 30s
+                        Http request timeout in seconds - 30
   -i PATH, --input PATH
-                        Path to text file containing query per
-                        line - None
+                        Path to text file containing query
+                        per line - None
+  -o FORMAT, --output FORMAT
+                        Format for generating filename
+                        %(key)s : [title,vid,fquality,ftype]
+                        - None
   -thr THREAD, --thread THREAD
-                        Download [x] amount of videos/audios at
-                        once - 1
-  --disable-bar         Disables download progress bar - False
-  --ask                 Confirm before downloading file - False
+                        Download [x] amount of videos/audios
+                        at once - 1
+  --disable-bar         Disable download progress bar -
+                        False
+  --ask                 Confirm before downloading file -
+                        False
   --unique              Auto-skip any media that you once
                         dowloaded - False
-  --quiet               Not to stdout anything other than logs -
-                        False
+  --quiet               Not to stdout anything other than
+                        logs - False
   --history             Stdout all media metadata ever
                         downloaded - False
   --clear               Clear all download histories - False
 
 This script has no official relation with y2mate.com
 ```
 </details>
```

#### html2text {}

```diff
@@ -39,50 +39,52 @@
 as well specify total videos to be downloaded by using `limit` argument. For
 instance: ```py from y2mate_api import Handler api = Handler("https://youtu.be/
 POPoAjWFkGg") api.auto_save(limit=10) # This will download the video in path
 and 9 other videos related to the query specified ``` **Note** : You can still
 use **video id** such as `POPoAjWFkGg` as query parameter. ## Other parameters
 - `Handler` * author : Video author i.e Youtube Channel * timeout : http
 requests timeout * ask : Confirm before downloading media * unique : Auto-
-ignore previously downloaded media - `Handler.run` * format : Media format mp4/
-mp3 * quality : Media qualiy such as 720p/128kbps * resolver : Additional
-format info : [m4a,3gp,mp4,mp3] * limit : Total videos to be retrieved *
-keyword : Phrase(s) that must be in media title * author : Video author i.e
-Youtube Channel - `Handler.auto_save` * dir : Path to Directory for saving the
-media files * iterator : Function that yields third_query object -
-`Handler.run` * progress_bar : Stdout media-name & Display progress bar -
-`Handler.save` * third_dict : Response of `third_query.run()` * dir : Directory
-for saving the contents * progress_bar : Stdout media-name & Display download
-progress bar    For more info run `$ y2mate -h`  ``` usage: y2mate [-h] [-v] [-
-f mp4|mp3] [-
+ignore previously downloaded media * thread : Download (x) value of file at a
+time. - `Handler.run` * format : Media format mp4/mp3 * quality : Media qualiy
+such as 720p/128kbps * resolver : Additional format info : [m4a,3gp,mp4,mp3] *
+limit : Total videos to be retrieved * keyword : Phrase(s) that must be in
+media title * author : Video author i.e Youtube Channel - `Handler.auto_save` *
+dir : Path to Directory for saving the media files * iterator : Function that
+yields third_query object - `Handler.run` * progress_bar : Stdout media-name &
+Display progress bar - `Handler.save` * third_dict : Response of
+`third_query.run()` * dir : Directory for saving the contents * progress_bar :
+Display download progress bar * quiet : Not to stdout anything * naming_format
+: Format for generating media filename using the `third_query` response keys
+For more info run `$ y2mate -h`  ``` usage: y2mate [-h] [-v] [-f mp3|mp4] [-
 q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps]
 [-r m4a|3gp|mp4|mp3] [-k [KEYWORD ...]] [-a [AUTHOR ...]] [-l LIMIT] [-d PATH]
-[-t TIMEOUT] [-i PATH] [-thr THREAD] [--disable-bar] [--ask] [--unique] [--
-quiet] [--history] [--clear] [query ...] Download youtube videos and audios by
-title or link positional arguments: query Youtube video title, link or id -
-None options: -h, --help show this help message and exit -v, --version show
-program's version number and exit -f mp4|mp3, --format mp4|mp3 Specify media
-type - audio/video -
+[-t TIMEOUT] [-i PATH] [-o FORMAT] [-thr THREAD] [--disable-bar] [--ask] [--
+unique] [--quiet] [--history] [--clear] [query ...] Download youtube videos and
+audios by title or link positional arguments: query Youtube video title, link
+or id - None options: -h, --help show this help message and exit -v, --version
+show program's version number and exit -f mp3|mp4, --format mp3|mp4 Specify
+media type - audio/video -
 q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps,
 --quality
 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps
 Media quality -720p -r m4a|3gp|mp4|mp3, --resolver m4a|3gp|mp4|mp3 Other media
 formats incase of multiple options - mp4/mp3 -k [KEYWORD ...], --keyword
 [KEYWORD ...] Media should contain this keywords - None -a [AUTHOR ...], --
 author [AUTHOR ...] Media author i.e YouTube channel name - None -l LIMIT, --
 limit LIMIT Total videos to be downloaded - 1 -d PATH, --dir PATH Directory for
-saving the contents - /storage/emulated/0/git/Smartwa -t TIMEOUT, --timeout
-TIMEOUT Http request timeout - 30s -i PATH, --input PATH Path to text file
-containing query per line - None -thr THREAD, --thread THREAD Download [x]
-amount of videos/audios at once - 1 --disable-bar Disables download progress
-bar - False --ask Confirm before downloading file - False --unique Auto-skip
-any media that you once dowloaded - False --quiet Not to stdout anything other
-than logs - False --history Stdout all media metadata ever downloaded - False -
--clear Clear all download histories - False This script has no official
-relation with y2mate.com ```  - Review [CHANGELOG](https://github.com/Simatwa/
-y2mate-api/blob/main/Docs/CHANGELOG.md) for latest updates. ## Disclaimer This
-repository is intended for educational and personal use only. The use of this
-repository for any commercial or illegal purposes is strictly prohibited. The
-repository owner does not endorse or encourage the downloading or sharing of
-copyrighted material without permission. The repository owner is not
-responsible for any misuse of the software or any legal consequences that may
-arise from such misuse.
+saving the contents - /storage/emulated/0/git/Smartwa/y2ma te-api -t TIMEOUT, -
+-timeout TIMEOUT Http request timeout in seconds - 30 -i PATH, --input PATH
+Path to text file containing query per line - None -o FORMAT, --output FORMAT
+Format for generating filename %(key)s : [title,vid,fquality,ftype] - None -thr
+THREAD, --thread THREAD Download [x] amount of videos/audios at once - 1 --
+disable-bar Disable download progress bar - False --ask Confirm before
+downloading file - False --unique Auto-skip any media that you once dowloaded -
+False --quiet Not to stdout anything other than logs - False --history Stdout
+all media metadata ever downloaded - False --clear Clear all download histories
+- False This script has no official relation with y2mate.com ```  - Review
+[CHANGELOG](https://github.com/Simatwa/y2mate-api/blob/main/Docs/CHANGELOG.md)
+for latest updates. ## Disclaimer This repository is intended for educational
+and personal use only. The use of this repository for any commercial or illegal
+purposes is strictly prohibited. The repository owner does not endorse or
+encourage the downloading or sharing of copyrighted material without
+permission. The repository owner is not responsible for any misuse of the
+software or any legal consequences that may arise from such misuse.
```

### Comparing `y2mate-api-0.0.3/setup.py` & `y2mate-api-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `y2mate-api-0.0.3/y2mate_api/console.py` & `y2mate-api-0.0.4/y2mate_api/console.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,16 +36,16 @@
     parser.add_argument(
         "query", nargs="*", help="Youtube video title, link or id - %(default)s"
     )
     parser.add_argument(
         "-f",
         "--format",
         help="Specify media type - audio/video",
-        choices=["mp4", "mp3"],
-        metavar="mp4|mp3",
+        choices=["mp3", "mp4"],
+        metavar="mp3|mp4",
     )
     parser.add_argument(
         "-q",
         "--quality",
         help="Media quality -%(default)s",
         choices=media_qualities,
         metavar="|".join(media_qualities),
@@ -83,34 +83,40 @@
         help="Directory for saving the contents - %(default)s",
         default=getcwd(),
         metavar="PATH",
     )
     parser.add_argument(
         "-t",
         "--timeout",
-        help="Http request timeout - %(default)ss",
+        help="Http request timeout in seconds - %(default)s",
         type=int,
         default=30,
     )
     parser.add_argument(
         "-i",
         "--input",
         help="Path to text file containing query per line - %(default)s",
         metavar="PATH",
     )
     parser.add_argument(
+        "-o",
+        "--output",
+        metavar="FORMAT",
+        help="Format for generating filename %%(key)s : [title,vid,fquality,ftype] - %(default)s",
+    )
+    parser.add_argument(
         "-thr",
         "--thread",
         help="Download [x] amount of videos/audios at once - 1",
         type=int,
         default=0,
     )
     parser.add_argument(
         "--disable-bar",
-        help="Disables download progress bar - %(default)s",
+        help="Disable download progress bar - %(default)s",
         action="store_true",
     )
     parser.add_argument(
         "--ask",
         help="Confirm before downloading file - %(default)s",
         action="store_true",
     )
@@ -160,14 +166,15 @@
         unique=args.unique,
         thread=args.thread,
     )
     auto_save_args = dict(
         dir=args.dir,
         progress_bar=args.disable_bar == False,
         quiet=args.quiet,
+        naming_format=args.output,
         format=args.format,
         quality=args.quality,
         resolver=args.resolver,
         limit=args.limit,
         keyword=h_mult_args(args.keyword),
         author=h_mult_args(args.author),
     )
@@ -176,9 +183,9 @@
         for query in open(args.input).read().strip().split("\n"):
             handler_init_args["query"] = query
             auto_save_args["limit"] = 1
             Handler(**handler_init_args).auto_save(**auto_save_args)
     else:
         Handler(**handler_init_args).auto_save(**auto_save_args)
     logging.info(
-        f"Done downloading [{args.limit}] {'audio' if args.format=='mp3' else 'video'}(s)"
+        f"Done downloading [{args.limit}] {'audio' if args.format=='mp3' else 'video'}{'' if args.limit==1 else 's'}"
     )
```

### Comparing `y2mate-api-0.0.3/y2mate_api/downloader.py` & `y2mate-api-0.0.4/y2mate_api/downloader.py`

 * *Files 11% similar despite different names*

```diff
@@ -49,14 +49,15 @@
         self.timeout = timeout
         self.keyword = None
         self.ask = ask
         self.unique = unique
         self.thread = thread
         self.vitems = []
         self.related = []
+        self.dropped = []
         self.total = 1
         self.saved_videos = utils.get_history()
 
     def __str__(self):
         return self.query
 
     def __enter__(self):
@@ -125,25 +126,28 @@
         init_query_two = second_query(self.query_one)
         x = 0
         if not self.query_one.is_link:
             for video_dict in self.vitems:
                 init_query_two.video_dict = video_dict
                 query_2 = init_query_two.main(timeout=self.timeout)
                 if query_2.processed:
+                    if query_2.vid in self.dropped:
+                        continue
                     if self.author and not self.author.lower() in query_2.a.lower():
                         logging.warning(
                             f"Dropping {Fore.YELLOW+query_2.title+Fore.RESET} by  {Fore.RED+query_2.a+Fore.RESET}"
                         )
                         continue
                     else:
                         yes_download, reason = self.__verify_item(query_2)
                         if not yes_download:
                             logging.warning(
                                 f"Skipping {Fore.YELLOW+query_2.title+Fore.RESET} by {Fore.MAGENTA+query_2.a+Fore.RESET} -  Reason : {Fore.BLUE+reason+Fore.RESET}"
                             )
+                            self.dropped.append(query_2.vid)
                             continue
                         self.related.append(query_2.related)
                         yield query_2
                         x += 1
                         if x >= self.total:
                             break
                 else:
@@ -174,14 +178,15 @@
                                 continue
                             else:
                                 yes_download, reason = self.__verify_item(query_2)
                                 if not yes_download:
                                     logging.warning(
                                         f"Skipping {Fore.YELLOW+query_2.title+Fore.RESET} by {Fore.MAGENTA+query_2.a+Fore.RESET} -  Reason : {Fore.BLUE+reason+Fore.RESET}"
                                     )
+                                    self.dropped.append(query_2.vid)
                                     continue
 
                                 self.related.append(query_2.related)
                                 yield query_2
                                 x += 1
                                 if x >= self.total:
                                     break
@@ -230,25 +235,25 @@
                         resolver=resolver,
                         timeout=self.timeout,
                     )
                 )
             else:
                 logging.error(f"Empty object - {query_two_obj}")
 
-    def generate_filename(self, third_dict: dict, format: str = None) -> str:
+    def generate_filename(self, third_dict: dict, naming_format: str = None) -> str:
         r"""Generate filename based on the response of `third_query`
         :param third_dict: response of `third_query.main()` object
-        :param format: (Optional) Format for formatting fnm based on `third_dict` keys
+        :param naming_format: (Optional) Format for generating filename based on `third_dict` keys
         :type third_dict: dict
-        :type format: str
+        :type naming_format: str
         :rtype: str
         """
         fnm = (
-            f"{format}" % third_dict
-            if format
+            f"{naming_format}" % third_dict
+            if naming_format
             else f"{third_dict['title']} {third_dict['vid']}_{third_dict['fquality']}.{third_dict['ftype']}"
         )
 
         def sanitize(nm):
             trash = ["\\", "/", ":", "*", "?", '"', "<", "|", ">"]
             for val in trash:
                 nm = nm.replace(val, "")
@@ -258,26 +263,29 @@
 
     def auto_save(
         self,
         dir: str = "",
         iterator: object = None,
         progress_bar=True,
         quiet: bool = False,
+        naming_format: str = None,
         *args,
         **kwargs,
     ):
         r"""Query and save all the media
         :param dir: (Optional) Path to Directory for saving the media files
         :param iterator: (Optional) Function that yields third_query object - `Handler.run`
         :param progress_bar: (Optional) Display progress bar
         :param quiet: (Optional) Not to stdout anything
+        :param naming_format: (Optional) Format for generating filename
         :type dir: str
         :type iterator: object
         :type progress_bar: bool
         :type quiet: bool
+        :type naming_format: str
         args & kwargs for the iterator
         :rtype: None
         """
         iterator_object = iterator or self.run(*args, **kwargs)
 
         for x, entry in enumerate(iterator_object):
 
@@ -285,50 +293,58 @@
                 t1 = Thread(
                     target=self.save,
                     args=(
                         entry,
                         dir,
                         False,
                         quiet,
+                        naming_format,
                     ),
                 )
                 t1.start()
                 thread_count = x + 1
                 if thread_count % self.thread == 0 or thread_count == self.total:
                     logging.debug(
                         f"Waiting for current running threads to finish - thread_count : {thread_count}"
                     )
                     t1.join()
             else:
-                self.save(entry, dir, progress_bar, quiet)
+                self.save(entry, dir, progress_bar, quiet, naming_format)
 
     def save(
-        self, third_dict: dict, dir: str = "", progress_bar=True, quiet: bool = False
+        self,
+        third_dict: dict,
+        dir: str = "",
+        progress_bar=True,
+        quiet: bool = False,
+        naming_format: str = None,
     ):
         r"""Download media based on response of `third_query` dict-data-type
         :param third_dict: Response of `third_query.run()`
         :param dir: (Optional) Directory for saving the contents
         :param progress_bar: (Optional) Display download progress bar
         :param quiet: (Optional) Not to stdout anything
+        :param naming_format: (Optional) Format for generating filename
         :type third_dict: dict
         :type dir: str
         :type progress_bar: bool
         :type quiet: bool
+        :type naming_format: str
         :rtype: None
         """
         if third_dict:
             resp = requests.get(third_dict["dlink"], stream=True)
-            size_in_bits = int(resp.headers["content-length"])
+            size_in_bits = int(resp.headers.get("content-length", 1000000000000))
             size_in_mb = round(size_in_bits / 1000000, 2)
             chunk_size = 1024
-            filename = self.generate_filename(third_dict)
+            filename = self.generate_filename(third_dict, naming_format)
             save_to = path.join(dir, filename)
             third_dict["saved_to"] = (
                 save_to
-                if save_to.startswith(("/", "C:", "D:"))
+                if any([save_to.startswith("/"), ":" in save_to])
                 else path.join(getcwd(), dir, filename)
             )
             if progress_bar:
                 if not quiet:
                     print(f"{filename}")
                 with tqdm(
                     total=size_in_bits,
```

### Comparing `y2mate-api-0.0.3/y2mate_api/main.py` & `y2mate-api-0.0.4/y2mate_api/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         try:
             if not path.isfile(history_path):
                 data1 = {__prog__: []}
                 with open(history_path, "w") as fh:
                     json.dump(data1, fh)
             with open(history_path) as fh:
                 saved_data = json.load(fh).get(__prog__)
-            data["datetime"] = str(datetime.now())
+            data["datetime"] = datetime.now().strftime("%c")
             saved_data.append(data)
             with open(history_path, "w") as fh:
                 json.dump({__prog__: saved_data}, fh, indent=4)
         except Exception as e:
             logging.error(f"Failed to add to history - {get_excep(e)}")
 
     @staticmethod
```

### Comparing `y2mate-api-0.0.3/y2mate_api.egg-info/PKG-INFO` & `y2mate-api-0.0.4/y2mate_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: y2mate-api
-Version: 0.0.3
+Version: 0.0.4
 Summary: Download youtube videos and audios by title or link
 Home-page: https://github.com/Simatwa/y2mate-api
 Author: Smartwa
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/y2mate-api/issues/new
@@ -27,15 +27,15 @@
 License-File: LICENSE
 
 # y2mate-api
 
 <p align="center">
 <a href="https://github.com/Simatwa/y2mate-api"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a>
 <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
-<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.3&color=green"/></a>
+<a href="https://pypi.org/project/y2mate-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.4&color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>
 <a href="https://pepy.tech/project/livescore-api"><img src="https://static.pepy.tech/personalized-badge/y2mate-api?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a>
 </p>
 
@@ -155,14 +155,15 @@
 ## Other parameters
 
 - `Handler`
   * author : Video author i.e Youtube Channel
   * timeout : http requests timeout
   * ask : Confirm before downloading media
   * unique : Auto-ignore previously downloaded media
+  * thread : Download (x) value of file at a time.
 
 - `Handler.run`
   * format : Media format mp4/mp3
   * quality : Media qualiy such as 720p/128kbps
   * resolver : Additional format info : [m4a,3gp,mp4,mp3]
   * limit : Total videos to be retrieved
   * keyword : Phrase(s) that must be in media title
@@ -172,74 +173,85 @@
   * dir : Path to Directory for saving the media files
   * iterator : Function that yields third_query object - `Handler.run`
   * progress_bar : Stdout media-name & Display progress bar
  
 - `Handler.save`
   * third_dict : Response of `third_query.run()`
   * dir : Directory for saving the contents
-  * progress_bar : Stdout media-name & Display download progress bar
+  * progress_bar : Display download progress bar
+  * quiet : Not to stdout anything
+  * naming_format : Format for generating media filename using the `third_query` response keys
  
 </details>
  
 <details>
 <summary>
 	
 For more info run `$ y2mate -h`
 
 </summary>
 
 ```
-usage: y2mate [-h] [-v] [-f mp4|mp3]
+usage: y2mate [-h] [-v] [-f mp3|mp4]
               [-q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps]
               [-r m4a|3gp|mp4|mp3] [-k [KEYWORD ...]]
               [-a [AUTHOR ...]] [-l LIMIT] [-d PATH]
-              [-t TIMEOUT] [-i PATH] [-thr THREAD]
-              [--disable-bar] [--ask] [--unique] [--quiet]
-              [--history] [--clear]
+              [-t TIMEOUT] [-i PATH] [-o FORMAT]
+              [-thr THREAD] [--disable-bar] [--ask]
+              [--unique] [--quiet] [--history] [--clear]
               [query ...]
 
 Download youtube videos and audios by title or link
 
 positional arguments:
-  query                 Youtube video title, link or id - None
+  query                 Youtube video title, link or id -
+                        None
 
 options:
   -h, --help            show this help message and exit
-  -v, --version         show program's version number and exit
-  -f mp4|mp3, --format mp4|mp3
+  -v, --version         show program's version number and
+                        exit
+  -f mp3|mp4, --format mp3|mp4
                         Specify media type - audio/video
   -q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps, --quality 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps
                         Media quality -720p
   -r m4a|3gp|mp4|mp3, --resolver m4a|3gp|mp4|mp3
-                        Other media formats incase of multiple
-                        options - mp4/mp3
+                        Other media formats incase of
+                        multiple options - mp4/mp3
   -k [KEYWORD ...], --keyword [KEYWORD ...]
                         Media should contain this keywords -
                         None
   -a [AUTHOR ...], --author [AUTHOR ...]
-                        Media author i.e YouTube channel name -
-                        None
+                        Media author i.e YouTube channel
+                        name - None
   -l LIMIT, --limit LIMIT
                         Total videos to be downloaded - 1
   -d PATH, --dir PATH   Directory for saving the contents -
-                        /storage/emulated/0/git/Smartwa
+                        /storage/emulated/0/git/Smartwa/y2ma
+                        te-api
   -t TIMEOUT, --timeout TIMEOUT
-                        Http request timeout - 30s
+                        Http request timeout in seconds - 30
   -i PATH, --input PATH
-                        Path to text file containing query per
-                        line - None
+                        Path to text file containing query
+                        per line - None
+  -o FORMAT, --output FORMAT
+                        Format for generating filename
+                        %(key)s : [title,vid,fquality,ftype]
+                        - None
   -thr THREAD, --thread THREAD
-                        Download [x] amount of videos/audios at
-                        once - 1
-  --disable-bar         Disables download progress bar - False
-  --ask                 Confirm before downloading file - False
+                        Download [x] amount of videos/audios
+                        at once - 1
+  --disable-bar         Disable download progress bar -
+                        False
+  --ask                 Confirm before downloading file -
+                        False
   --unique              Auto-skip any media that you once
                         dowloaded - False
-  --quiet               Not to stdout anything other than logs -
-                        False
+  --quiet               Not to stdout anything other than
+                        logs - False
   --history             Stdout all media metadata ever
                         downloaded - False
   --clear               Clear all download histories - False
 
 This script has no official relation with y2mate.com
 ```
 </details>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: y2mate-api Version: 0.0.3 Summary: Download youtube
+Metadata-Version: 2.1 Name: y2mate-api Version: 0.0.4 Summary: Download youtube
 videos and audios by title or link Home-page: https://github.com/Simatwa/
 y2mate-api Author: Smartwa Author-email: smartwacaleb@gmail.com Maintainer:
 Smartwa License: MIT Project-URL: Bug Report, https://github.com/Simatwa/
 y2mate-api/issues/new Keywords: y2mate,videos,video-api,youtube Classifier:
 License :: OSI Approved :: MIT License Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: License :: Free For Home Use Classifier: Intended
@@ -53,50 +53,52 @@
 as well specify total videos to be downloaded by using `limit` argument. For
 instance: ```py from y2mate_api import Handler api = Handler("https://youtu.be/
 POPoAjWFkGg") api.auto_save(limit=10) # This will download the video in path
 and 9 other videos related to the query specified ``` **Note** : You can still
 use **video id** such as `POPoAjWFkGg` as query parameter. ## Other parameters
 - `Handler` * author : Video author i.e Youtube Channel * timeout : http
 requests timeout * ask : Confirm before downloading media * unique : Auto-
-ignore previously downloaded media - `Handler.run` * format : Media format mp4/
-mp3 * quality : Media qualiy such as 720p/128kbps * resolver : Additional
-format info : [m4a,3gp,mp4,mp3] * limit : Total videos to be retrieved *
-keyword : Phrase(s) that must be in media title * author : Video author i.e
-Youtube Channel - `Handler.auto_save` * dir : Path to Directory for saving the
-media files * iterator : Function that yields third_query object -
-`Handler.run` * progress_bar : Stdout media-name & Display progress bar -
-`Handler.save` * third_dict : Response of `third_query.run()` * dir : Directory
-for saving the contents * progress_bar : Stdout media-name & Display download
-progress bar    For more info run `$ y2mate -h`  ``` usage: y2mate [-h] [-v] [-
-f mp4|mp3] [-
+ignore previously downloaded media * thread : Download (x) value of file at a
+time. - `Handler.run` * format : Media format mp4/mp3 * quality : Media qualiy
+such as 720p/128kbps * resolver : Additional format info : [m4a,3gp,mp4,mp3] *
+limit : Total videos to be retrieved * keyword : Phrase(s) that must be in
+media title * author : Video author i.e Youtube Channel - `Handler.auto_save` *
+dir : Path to Directory for saving the media files * iterator : Function that
+yields third_query object - `Handler.run` * progress_bar : Stdout media-name &
+Display progress bar - `Handler.save` * third_dict : Response of
+`third_query.run()` * dir : Directory for saving the contents * progress_bar :
+Display download progress bar * quiet : Not to stdout anything * naming_format
+: Format for generating media filename using the `third_query` response keys
+For more info run `$ y2mate -h`  ``` usage: y2mate [-h] [-v] [-f mp3|mp4] [-
 q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps]
 [-r m4a|3gp|mp4|mp3] [-k [KEYWORD ...]] [-a [AUTHOR ...]] [-l LIMIT] [-d PATH]
-[-t TIMEOUT] [-i PATH] [-thr THREAD] [--disable-bar] [--ask] [--unique] [--
-quiet] [--history] [--clear] [query ...] Download youtube videos and audios by
-title or link positional arguments: query Youtube video title, link or id -
-None options: -h, --help show this help message and exit -v, --version show
-program's version number and exit -f mp4|mp3, --format mp4|mp3 Specify media
-type - audio/video -
+[-t TIMEOUT] [-i PATH] [-o FORMAT] [-thr THREAD] [--disable-bar] [--ask] [--
+unique] [--quiet] [--history] [--clear] [query ...] Download youtube videos and
+audios by title or link positional arguments: query Youtube video title, link
+or id - None options: -h, --help show this help message and exit -v, --version
+show program's version number and exit -f mp3|mp4, --format mp3|mp4 Specify
+media type - audio/video -
 q 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps,
 --quality
 4k|1080p|720p|480p|360p|240p|144p|auto|mp3|m4a|.m4a|128kbps|192kbps|328kbps
 Media quality -720p -r m4a|3gp|mp4|mp3, --resolver m4a|3gp|mp4|mp3 Other media
 formats incase of multiple options - mp4/mp3 -k [KEYWORD ...], --keyword
 [KEYWORD ...] Media should contain this keywords - None -a [AUTHOR ...], --
 author [AUTHOR ...] Media author i.e YouTube channel name - None -l LIMIT, --
 limit LIMIT Total videos to be downloaded - 1 -d PATH, --dir PATH Directory for
-saving the contents - /storage/emulated/0/git/Smartwa -t TIMEOUT, --timeout
-TIMEOUT Http request timeout - 30s -i PATH, --input PATH Path to text file
-containing query per line - None -thr THREAD, --thread THREAD Download [x]
-amount of videos/audios at once - 1 --disable-bar Disables download progress
-bar - False --ask Confirm before downloading file - False --unique Auto-skip
-any media that you once dowloaded - False --quiet Not to stdout anything other
-than logs - False --history Stdout all media metadata ever downloaded - False -
--clear Clear all download histories - False This script has no official
-relation with y2mate.com ```  - Review [CHANGELOG](https://github.com/Simatwa/
-y2mate-api/blob/main/Docs/CHANGELOG.md) for latest updates. ## Disclaimer This
-repository is intended for educational and personal use only. The use of this
-repository for any commercial or illegal purposes is strictly prohibited. The
-repository owner does not endorse or encourage the downloading or sharing of
-copyrighted material without permission. The repository owner is not
-responsible for any misuse of the software or any legal consequences that may
-arise from such misuse.
+saving the contents - /storage/emulated/0/git/Smartwa/y2ma te-api -t TIMEOUT, -
+-timeout TIMEOUT Http request timeout in seconds - 30 -i PATH, --input PATH
+Path to text file containing query per line - None -o FORMAT, --output FORMAT
+Format for generating filename %(key)s : [title,vid,fquality,ftype] - None -thr
+THREAD, --thread THREAD Download [x] amount of videos/audios at once - 1 --
+disable-bar Disable download progress bar - False --ask Confirm before
+downloading file - False --unique Auto-skip any media that you once dowloaded -
+False --quiet Not to stdout anything other than logs - False --history Stdout
+all media metadata ever downloaded - False --clear Clear all download histories
+- False This script has no official relation with y2mate.com ```  - Review
+[CHANGELOG](https://github.com/Simatwa/y2mate-api/blob/main/Docs/CHANGELOG.md)
+for latest updates. ## Disclaimer This repository is intended for educational
+and personal use only. The use of this repository for any commercial or illegal
+purposes is strictly prohibited. The repository owner does not endorse or
+encourage the downloading or sharing of copyrighted material without
+permission. The repository owner is not responsible for any misuse of the
+software or any legal consequences that may arise from such misuse.
```

