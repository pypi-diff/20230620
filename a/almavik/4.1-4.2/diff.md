# Comparing `tmp/almavik-4.1.tar.gz` & `tmp/almavik-4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "almavik-4.1.tar", last modified: Tue Jun 20 12:24:34 2023, max compression
+gzip compressed data, was "almavik-4.2.tar", last modified: Tue Jun 20 14:45:49 2023, max compression
```

## Comparing `almavik-4.1.tar` & `almavik-4.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:24:34.850548 almavik-4.1/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-20 12:18:19.000000 almavik-4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-06-20 12:24:34.850548 almavik-4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-06-20 12:18:19.000000 almavik-4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:24:34.850548 almavik-4.1/almavik.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-06-20 12:24:34.000000 almavik-4.1/almavik.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-20 12:24:34.000000 almavik-4.1/almavik.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 12:24:34.000000 almavik-4.1/almavik.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-20 12:24:34.000000 almavik-4.1/almavik.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 12:24:34.000000 almavik-4.1/almavik.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:24:34.850548 almavik-4.1/exp1/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-20 12:18:19.000000 almavik-4.1/exp1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 12:24:34.850548 almavik-4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-20 12:18:19.000000 almavik-4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:24:34.850548 almavik-4.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-06-20 12:18:19.000000 almavik-4.1/src/YPPRPO.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-20 12:18:19.000000 almavik-4.1/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-06-20 12:18:19.000000 almavik-4.1/src/detectorDrop.py
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-06-20 12:18:19.000000 almavik-4.1/src/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:45:49.015084 almavik-4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-20 14:39:54.000000 almavik-4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-20 14:45:49.015084 almavik-4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-20 14:39:54.000000 almavik-4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:45:49.015084 almavik-4.2/almavik.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-20 14:45:48.000000 almavik-4.2/almavik.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-20 14:45:48.000000 almavik-4.2/almavik.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:45:48.000000 almavik-4.2/almavik.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-20 14:45:48.000000 almavik-4.2/almavik.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 14:45:48.000000 almavik-4.2/almavik.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:45:49.015084 almavik-4.2/exp1/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-20 14:39:55.000000 almavik-4.2/exp1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 14:45:49.015084 almavik-4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-20 14:39:55.000000 almavik-4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:45:49.015084 almavik-4.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-06-20 14:39:55.000000 almavik-4.2/src/YPPRPO.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-20 14:39:55.000000 almavik-4.2/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-06-20 14:39:55.000000 almavik-4.2/src/detectorDrop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-06-20 14:39:55.000000 almavik-4.2/src/widgets.py
```

### Comparing `almavik-4.1/PKG-INFO` & `almavik-4.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: almavik
-Version: 4.1
-Summary: Determination of the drop trajectory
-Home-page: https://github.com/markusLons/almavik
-Author: Markus.Alinas.Viktorias
-Author-email: v.tikhonova@g.nsu.ru
-Classifier: Development Status :: 3 - Alpha
-Description-Content-Type: text/markdown
-
 # Алмавик
 
 ![Логотип Алмавик](formalization/logoza.png)
 <br>
 <div>
     <a href="https://hub.docker.com/repository/docker/markuslons/almavik"><img src="https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white" alt="Docker Pulls"></a>
    <a href="https://pypi.org/project/almavik/"><img src="https://pypi.org/static/images/logo-small.2a411bc6.svg" alt="PyPi Pulls"></a>
@@ -31,21 +21,51 @@
 
 ## Использование
 
 ### Установка
 
 ## Запуск
 ### Локальный запуск 
-Для установки и запуска Алмавик и его зависимостей, выполните следующие шаги:
-    1. Установите зависимости из файла requirements.txt, выполнив команду: pip install -r requirements.txt
+    1. Установите зависимости из файла requirements.txt, выполнив команду: 
+    $ pip install -r requirements.txt
     2. Создайте папку "exp1" в корневой директории проекта. В этой папке будут храниться изображения.
-    3. Для запуска Алмавик локально, выполните команду: python YPPRPO.py
+    3. Для запуска Алмавик локально, выполните команду:
+    $python YPPRPO.py
 ### Запуск в Docker контейнере
-    1. Загрузите Docker образ Алмавик из репозитория Docker Hub, выполнив команду: docker pull markuslons/almavik
-    2. Запустите контейнер, используя следующую команду: docker run -it markuslons/almavik
+    1. Загрузите Docker образ Алмавик из репозитория Docker Hub, выполнив команду: 
+    $ docker pull markuslons/almavik
+    2. Запустите контейнер, используя следующую команду: 
+    $ docker run -it markuslons/almavik
 ### Запуск через pip
 Тут типо вика 
+<div align="center">
+  <table>
+    <tr>
+      <td align="center">
+        <a href="ссылка/на/маркус">
+          <img src="formalization/markus.jpg" width="200px" alt="Markus">
+        </a>
+        <br />
+        <sub><b>Markus</b></sub>
+      </td>
+      <td align="center">
+        <a href="ссылка/на/blubbery">
+          <img src="formalization/blubbery.jpg" width="200px" alt="Blubbery">
+        </a>
+        <br />
+        <sub><b>Blubbery</b></sub>
+      </td>
+      <td align="center">
+        <a href="ссылка/на/viktoriatix">
+          <img src="formalization/viktoriatix.jpg" width="200px" alt="Viktoriatix">
+        </a>
+        <br />
+        <sub><b>Viktoriatix</b></sub>
+      </td>
+    </tr>
+  </table>
+</div>
 
 
 ## Ссылки
 https://pypi.org/project/almavik/
 https://hub.docker.com/repository/docker/markuslons/almavik
```

#### html2text {}

```diff
@@ -1,12 +1,8 @@
-Metadata-Version: 2.1 Name: almavik Version: 4.1 Summary: Determination of the
-drop trajectory Home-page: https://github.com/markusLons/almavik Author:
-Markus.Alinas.Viktorias Author-email: v.tikhonova@g.nsu.ru Classifier:
-Development Status :: 3 - Alpha Description-Content-Type: text/markdown #
-ÐÐ»Ð¼Ð°Ð²Ð¸Ðº ![ÐÐ¾Ð³Ð¾ÑÐ¸Ð¿ ÐÐ»Ð¼Ð°Ð²Ð¸Ðº](formalization/logoza.png)
+# ÐÐ»Ð¼Ð°Ð²Ð¸Ðº ![ÐÐ¾Ð³Ð¾ÑÐ¸Ð¿ ÐÐ»Ð¼Ð°Ð²Ð¸Ðº](formalization/logoza.png)
 [Docker_Pulls] [PyPi_Pulls]
 
 ÐÐ»Ð¼Ð°Ð²Ð¸Ðº - Ð¿ÑÐ¾Ð³ÑÐ°Ð¼Ð¼Ð° Ð´Ð»Ñ Ð¾Ð¿ÑÐµÐ´ÐµÐ»ÐµÐ½Ð¸Ñ ÑÐµÐ½ÑÑÐ°
 Ð¼Ð°ÑÑ ÐºÐ°Ð¿Ð»Ð¸ Ð¿Ð¾ Ð¸Ð·Ð¾Ð±ÑÐ°Ð¶ÐµÐ½Ð¸Ñ. ÐÐ½Ð°
 Ð¿ÑÐµÐ´Ð¾ÑÑÐ°Ð²Ð»ÑÐµÑ ÑÐ´Ð¾Ð±Ð½ÑÐ¹ Ð¸Ð½ÑÐµÑÑÐµÐ¹Ñ Ð¸ ÑÑÐ½ÐºÑÐ¸Ð¸
 Ð¾Ð±ÑÐ°Ð±Ð¾ÑÐºÐ¸ Ð¸Ð·Ð¾Ð±ÑÐ°Ð¶ÐµÐ½Ð¸Ð¹, ÐºÐ¾ÑÐ¾ÑÑÐµ Ð¿Ð¾Ð·Ð²Ð¾Ð»ÑÑÑ
 ÑÐ¾ÑÐ½Ð¾ Ð¸ Ð±ÑÑÑÑÐ¾ Ð¾Ð¿ÑÐµÐ´ÐµÐ»Ð¸ÑÑ ÑÐµÐ½ÑÑ Ð¼Ð°ÑÑ ÐºÐ°Ð¿Ð»Ð¸.
@@ -19,22 +15,23 @@
 Ð»ÐµÐ³ÐºÐ¾ Ð·Ð°Ð³ÑÑÐ¶Ð°ÑÑ Ð¸Ð·Ð¾Ð±ÑÐ°Ð¶ÐµÐ½Ð¸Ñ Ð¸
 Ð¿ÑÐ¾ÑÐ¼Ð°ÑÑÐ¸Ð²Ð°ÑÑ ÑÐµÐ·ÑÐ»ÑÑÐ°ÑÑ Ð¾Ð±ÑÐ°Ð±Ð¾ÑÐºÐ¸. -
 **ÐÑÐ°ÑÐ¸ÑÐµÑÐºÐ¾Ðµ Ð¿ÑÐµÐ´ÑÑÐ°Ð²Ð»ÐµÐ½Ð¸Ðµ**: ÐÐ»Ð¼Ð°Ð²Ð¸Ðº
 Ð¿ÑÐµÐ´Ð¾ÑÑÐ°Ð²Ð»ÑÐµÑ Ð³ÑÐ°ÑÐ¸ÑÐµÑÐºÐ¾Ðµ Ð¿ÑÐµÐ´ÑÑÐ°Ð²Ð»ÐµÐ½Ð¸Ðµ
 ÐºÐ°Ð¿Ð»Ð¸, Ð¿Ð¾Ð·Ð²Ð¾Ð»ÑÑ Ð²Ð¸Ð·ÑÐ°Ð»ÑÐ½Ð¾ Ð¾ÑÐµÐ½Ð¸ÑÑ ÐµÐµ ÑÐ¾ÑÐ¼Ñ
 Ð¸ ÑÐ°Ð·Ð¼ÐµÑ. ![ÐÐ¾Ð³Ð¾ÑÐ¸Ð¿ ÐÐ»Ð¼Ð°Ð²Ð¸Ðº](formalization/int.jpg) ##
 ÐÑÐ¿Ð¾Ð»ÑÐ·Ð¾Ð²Ð°Ð½Ð¸Ðµ ### Ð£ÑÑÐ°Ð½Ð¾Ð²ÐºÐ° ## ÐÐ°Ð¿ÑÑÐº ###
-ÐÐ¾ÐºÐ°Ð»ÑÐ½ÑÐ¹ Ð·Ð°Ð¿ÑÑÐº ÐÐ»Ñ ÑÑÑÐ°Ð½Ð¾Ð²ÐºÐ¸ Ð¸ Ð·Ð°Ð¿ÑÑÐºÐ°
-ÐÐ»Ð¼Ð°Ð²Ð¸Ðº Ð¸ ÐµÐ³Ð¾ Ð·Ð°Ð²Ð¸ÑÐ¸Ð¼Ð¾ÑÑÐµÐ¹, Ð²ÑÐ¿Ð¾Ð»Ð½Ð¸ÑÐµ
-ÑÐ»ÐµÐ´ÑÑÑÐ¸Ðµ ÑÐ°Ð³Ð¸: 1. Ð£ÑÑÐ°Ð½Ð¾Ð²Ð¸ÑÐµ Ð·Ð°Ð²Ð¸ÑÐ¸Ð¼Ð¾ÑÑÐ¸
-Ð¸Ð· ÑÐ°Ð¹Ð»Ð° requirements.txt, Ð²ÑÐ¿Ð¾Ð»Ð½Ð¸Ð² ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ: pip install
--r requirements.txt 2. Ð¡Ð¾Ð·Ð´Ð°Ð¹ÑÐµ Ð¿Ð°Ð¿ÐºÑ "exp1" Ð² ÐºÐ¾ÑÐ½ÐµÐ²Ð¾Ð¹
-Ð´Ð¸ÑÐµÐºÑÐ¾ÑÐ¸Ð¸ Ð¿ÑÐ¾ÐµÐºÑÐ°. Ð ÑÑÐ¾Ð¹ Ð¿Ð°Ð¿ÐºÐµ Ð±ÑÐ´ÑÑ
-ÑÑÐ°Ð½Ð¸ÑÑÑÑ Ð¸Ð·Ð¾Ð±ÑÐ°Ð¶ÐµÐ½Ð¸Ñ. 3. ÐÐ»Ñ Ð·Ð°Ð¿ÑÑÐºÐ°
-ÐÐ»Ð¼Ð°Ð²Ð¸Ðº Ð»Ð¾ÐºÐ°Ð»ÑÐ½Ð¾, Ð²ÑÐ¿Ð¾Ð»Ð½Ð¸ÑÐµ ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ: python
+ÐÐ¾ÐºÐ°Ð»ÑÐ½ÑÐ¹ Ð·Ð°Ð¿ÑÑÐº 1. Ð£ÑÑÐ°Ð½Ð¾Ð²Ð¸ÑÐµ Ð·Ð°Ð²Ð¸ÑÐ¸Ð¼Ð¾ÑÑÐ¸
+Ð¸Ð· ÑÐ°Ð¹Ð»Ð° requirements.txt, Ð²ÑÐ¿Ð¾Ð»Ð½Ð¸Ð² ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ: $ pip
+install -r requirements.txt 2. Ð¡Ð¾Ð·Ð´Ð°Ð¹ÑÐµ Ð¿Ð°Ð¿ÐºÑ "exp1" Ð²
+ÐºÐ¾ÑÐ½ÐµÐ²Ð¾Ð¹ Ð´Ð¸ÑÐµÐºÑÐ¾ÑÐ¸Ð¸ Ð¿ÑÐ¾ÐµÐºÑÐ°. Ð ÑÑÐ¾Ð¹ Ð¿Ð°Ð¿ÐºÐµ
+Ð±ÑÐ´ÑÑ ÑÑÐ°Ð½Ð¸ÑÑÑÑ Ð¸Ð·Ð¾Ð±ÑÐ°Ð¶ÐµÐ½Ð¸Ñ. 3. ÐÐ»Ñ Ð·Ð°Ð¿ÑÑÐºÐ°
+ÐÐ»Ð¼Ð°Ð²Ð¸Ðº Ð»Ð¾ÐºÐ°Ð»ÑÐ½Ð¾, Ð²ÑÐ¿Ð¾Ð»Ð½Ð¸ÑÐµ ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ: $python
 YPPRPO.py ### ÐÐ°Ð¿ÑÑÐº Ð² Docker ÐºÐ¾Ð½ÑÐµÐ¹Ð½ÐµÑÐµ 1. ÐÐ°Ð³ÑÑÐ·Ð¸ÑÐµ
 Docker Ð¾Ð±ÑÐ°Ð· ÐÐ»Ð¼Ð°Ð²Ð¸Ðº Ð¸Ð· ÑÐµÐ¿Ð¾Ð·Ð¸ÑÐ¾ÑÐ¸Ñ Docker Hub,
-Ð²ÑÐ¿Ð¾Ð»Ð½Ð¸Ð² ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ: docker pull markuslons/almavik 2.
+Ð²ÑÐ¿Ð¾Ð»Ð½Ð¸Ð² ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ: $ docker pull markuslons/almavik 2.
 ÐÐ°Ð¿ÑÑÑÐ¸ÑÐµ ÐºÐ¾Ð½ÑÐµÐ¹Ð½ÐµÑ, Ð¸ÑÐ¿Ð¾Ð»ÑÐ·ÑÑ ÑÐ»ÐµÐ´ÑÑÑÑÑ
-ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ: docker run -it markuslons/almavik ### ÐÐ°Ð¿ÑÑÐº ÑÐµÑÐµÐ·
-pip Ð¢ÑÑ ÑÐ¸Ð¿Ð¾ Ð²Ð¸ÐºÐ° ## Ð¡ÑÑÐ»ÐºÐ¸ https://pypi.org/project/almavik/
-https://hub.docker.com/repository/docker/markuslons/almavik
+ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ: $ docker run -it markuslons/almavik ### ÐÐ°Ð¿ÑÑÐº ÑÐµÑÐµÐ·
+pip Ð¢ÑÑ ÑÐ¸Ð¿Ð¾ Ð²Ð¸ÐºÐ°
+                     [Markus]  [Blubbery]  [Viktoriatix]
+                      Markus    Blubbery    Viktoriatix
+## Ð¡ÑÑÐ»ÐºÐ¸ https://pypi.org/project/almavik/ https://hub.docker.com/
+repository/docker/markuslons/almavik
```

### Comparing `almavik-4.1/README.md` & `almavik-4.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: almavik
+Version: 4.2
+Summary: Determination of the drop trajectory
+Home-page: https://github.com/markusLons/almavik
+Author: Markus.Alinas.Viktorias
+Author-email: v.tikhonova@g.nsu.ru
+Description-Content-Type: text/markdown
+
 # Алмавик
 
 ![Логотип Алмавик](formalization/logoza.png)
 <br>
 <div>
     <a href="https://hub.docker.com/repository/docker/markuslons/almavik"><img src="https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white" alt="Docker Pulls"></a>
    <a href="https://pypi.org/project/almavik/"><img src="https://pypi.org/static/images/logo-small.2a411bc6.svg" alt="PyPi Pulls"></a>
@@ -21,21 +30,51 @@
 
 ## Использование
 
 ### Установка
 
 ## Запуск
 ### Локальный запуск 
-Для установки и запуска Алмавик и его зависимостей, выполните следующие шаги:
-    1. Установите зависимости из файла requirements.txt, выполнив команду: pip install -r requirements.txt
+    1. Установите зависимости из файла requirements.txt, выполнив команду: 
+    $ pip install -r requirements.txt
     2. Создайте папку "exp1" в корневой директории проекта. В этой папке будут храниться изображения.
-    3. Для запуска Алмавик локально, выполните команду: python YPPRPO.py
+    3. Для запуска Алмавик локально, выполните команду:
+    $python YPPRPO.py
 ### Запуск в Docker контейнере
-    1. Загрузите Docker образ Алмавик из репозитория Docker Hub, выполнив команду: docker pull markuslons/almavik
-    2. Запустите контейнер, используя следующую команду: docker run -it markuslons/almavik
+    1. Загрузите Docker образ Алмавик из репозитория Docker Hub, выполнив команду: 
+    $ docker pull markuslons/almavik
+    2. Запустите контейнер, используя следующую команду: 
+    $ docker run -it markuslons/almavik
 ### Запуск через pip
 Тут типо вика 
+<div align="center">
+  <table>
+    <tr>
+      <td align="center">
+        <a href="ссылка/на/маркус">
+          <img src="formalization/markus.jpg" width="200px" alt="Markus">
+        </a>
+        <br />
+        <sub><b>Markus</b></sub>
+      </td>
+      <td align="center">
+        <a href="ссылка/на/blubbery">
+          <img src="formalization/blubbery.jpg" width="200px" alt="Blubbery">
+        </a>
+        <br />
+        <sub><b>Blubbery</b></sub>
+      </td>
+      <td align="center">
+        <a href="ссылка/на/viktoriatix">
+          <img src="formalization/viktoriatix.jpg" width="200px" alt="Viktoriatix">
+        </a>
+        <br />
+        <sub><b>Viktoriatix</b></sub>
+      </td>
+    </tr>
+  </table>
+</div>
 
 
 ## Ссылки
 https://pypi.org/project/almavik/
 https://hub.docker.com/repository/docker/markuslons/almavik
```

#### html2text {}

```diff
@@ -1,8 +1,12 @@
-# ÐÐ»Ð¼Ð°Ð²Ð¸Ðº ![ÐÐ¾Ð³Ð¾ÑÐ¸Ð¿ ÐÐ»Ð¼Ð°Ð²Ð¸Ðº](formalization/logoza.png)
+Metadata-Version: 2.1 Name: almavik Version: 4.2 Summary: Determination of the
+drop trajectory Home-page: https://github.com/markusLons/almavik Author:
+Markus.Alinas.Viktorias Author-email: v.tikhonova@g.nsu.ru Description-Content-
+Type: text/markdown # ÐÐ»Ð¼Ð°Ð²Ð¸Ðº ![ÐÐ¾Ð³Ð¾ÑÐ¸Ð¿ ÐÐ»Ð¼Ð°Ð²Ð¸Ðº]
+(formalization/logoza.png)
 [Docker_Pulls] [PyPi_Pulls]
 
 ÐÐ»Ð¼Ð°Ð²Ð¸Ðº - Ð¿ÑÐ¾Ð³ÑÐ°Ð¼Ð¼Ð° Ð´Ð»Ñ Ð¾Ð¿ÑÐµÐ´ÐµÐ»ÐµÐ½Ð¸Ñ ÑÐµÐ½ÑÑÐ°
 Ð¼Ð°ÑÑ ÐºÐ°Ð¿Ð»Ð¸ Ð¿Ð¾ Ð¸Ð·Ð¾Ð±ÑÐ°Ð¶ÐµÐ½Ð¸Ñ. ÐÐ½Ð°
 Ð¿ÑÐµÐ´Ð¾ÑÑÐ°Ð²Ð»ÑÐµÑ ÑÐ´Ð¾Ð±Ð½ÑÐ¹ Ð¸Ð½ÑÐµÑÑÐµÐ¹Ñ Ð¸ ÑÑÐ½ÐºÑÐ¸Ð¸
 Ð¾Ð±ÑÐ°Ð±Ð¾ÑÐºÐ¸ Ð¸Ð·Ð¾Ð±ÑÐ°Ð¶ÐµÐ½Ð¸Ð¹, ÐºÐ¾ÑÐ¾ÑÑÐµ Ð¿Ð¾Ð·Ð²Ð¾Ð»ÑÑÑ
 ÑÐ¾ÑÐ½Ð¾ Ð¸ Ð±ÑÑÑÑÐ¾ Ð¾Ð¿ÑÐµÐ´ÐµÐ»Ð¸ÑÑ ÑÐµÐ½ÑÑ Ð¼Ð°ÑÑ ÐºÐ°Ð¿Ð»Ð¸.
@@ -15,22 +19,23 @@
 Ð»ÐµÐ³ÐºÐ¾ Ð·Ð°Ð³ÑÑÐ¶Ð°ÑÑ Ð¸Ð·Ð¾Ð±ÑÐ°Ð¶ÐµÐ½Ð¸Ñ Ð¸
 Ð¿ÑÐ¾ÑÐ¼Ð°ÑÑÐ¸Ð²Ð°ÑÑ ÑÐµÐ·ÑÐ»ÑÑÐ°ÑÑ Ð¾Ð±ÑÐ°Ð±Ð¾ÑÐºÐ¸. -
 **ÐÑÐ°ÑÐ¸ÑÐµÑÐºÐ¾Ðµ Ð¿ÑÐµÐ´ÑÑÐ°Ð²Ð»ÐµÐ½Ð¸Ðµ**: ÐÐ»Ð¼Ð°Ð²Ð¸Ðº
 Ð¿ÑÐµÐ´Ð¾ÑÑÐ°Ð²Ð»ÑÐµÑ Ð³ÑÐ°ÑÐ¸ÑÐµÑÐºÐ¾Ðµ Ð¿ÑÐµÐ´ÑÑÐ°Ð²Ð»ÐµÐ½Ð¸Ðµ
 ÐºÐ°Ð¿Ð»Ð¸, Ð¿Ð¾Ð·Ð²Ð¾Ð»ÑÑ Ð²Ð¸Ð·ÑÐ°Ð»ÑÐ½Ð¾ Ð¾ÑÐµÐ½Ð¸ÑÑ ÐµÐµ ÑÐ¾ÑÐ¼Ñ
 Ð¸ ÑÐ°Ð·Ð¼ÐµÑ. ![ÐÐ¾Ð³Ð¾ÑÐ¸Ð¿ ÐÐ»Ð¼Ð°Ð²Ð¸Ðº](formalization/int.jpg) ##
 ÐÑÐ¿Ð¾Ð»ÑÐ·Ð¾Ð²Ð°Ð½Ð¸Ðµ ### Ð£ÑÑÐ°Ð½Ð¾Ð²ÐºÐ° ## ÐÐ°Ð¿ÑÑÐº ###
-ÐÐ¾ÐºÐ°Ð»ÑÐ½ÑÐ¹ Ð·Ð°Ð¿ÑÑÐº ÐÐ»Ñ ÑÑÑÐ°Ð½Ð¾Ð²ÐºÐ¸ Ð¸ Ð·Ð°Ð¿ÑÑÐºÐ°
-ÐÐ»Ð¼Ð°Ð²Ð¸Ðº Ð¸ ÐµÐ³Ð¾ Ð·Ð°Ð²Ð¸ÑÐ¸Ð¼Ð¾ÑÑÐµÐ¹, Ð²ÑÐ¿Ð¾Ð»Ð½Ð¸ÑÐµ
-ÑÐ»ÐµÐ´ÑÑÑÐ¸Ðµ ÑÐ°Ð³Ð¸: 1. Ð£ÑÑÐ°Ð½Ð¾Ð²Ð¸ÑÐµ Ð·Ð°Ð²Ð¸ÑÐ¸Ð¼Ð¾ÑÑÐ¸
-Ð¸Ð· ÑÐ°Ð¹Ð»Ð° requirements.txt, Ð²ÑÐ¿Ð¾Ð»Ð½Ð¸Ð² ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ: pip install
--r requirements.txt 2. Ð¡Ð¾Ð·Ð´Ð°Ð¹ÑÐµ Ð¿Ð°Ð¿ÐºÑ "exp1" Ð² ÐºÐ¾ÑÐ½ÐµÐ²Ð¾Ð¹
-Ð´Ð¸ÑÐµÐºÑÐ¾ÑÐ¸Ð¸ Ð¿ÑÐ¾ÐµÐºÑÐ°. Ð ÑÑÐ¾Ð¹ Ð¿Ð°Ð¿ÐºÐµ Ð±ÑÐ´ÑÑ
-ÑÑÐ°Ð½Ð¸ÑÑÑÑ Ð¸Ð·Ð¾Ð±ÑÐ°Ð¶ÐµÐ½Ð¸Ñ. 3. ÐÐ»Ñ Ð·Ð°Ð¿ÑÑÐºÐ°
-ÐÐ»Ð¼Ð°Ð²Ð¸Ðº Ð»Ð¾ÐºÐ°Ð»ÑÐ½Ð¾, Ð²ÑÐ¿Ð¾Ð»Ð½Ð¸ÑÐµ ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ: python
+ÐÐ¾ÐºÐ°Ð»ÑÐ½ÑÐ¹ Ð·Ð°Ð¿ÑÑÐº 1. Ð£ÑÑÐ°Ð½Ð¾Ð²Ð¸ÑÐµ Ð·Ð°Ð²Ð¸ÑÐ¸Ð¼Ð¾ÑÑÐ¸
+Ð¸Ð· ÑÐ°Ð¹Ð»Ð° requirements.txt, Ð²ÑÐ¿Ð¾Ð»Ð½Ð¸Ð² ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ: $ pip
+install -r requirements.txt 2. Ð¡Ð¾Ð·Ð´Ð°Ð¹ÑÐµ Ð¿Ð°Ð¿ÐºÑ "exp1" Ð²
+ÐºÐ¾ÑÐ½ÐµÐ²Ð¾Ð¹ Ð´Ð¸ÑÐµÐºÑÐ¾ÑÐ¸Ð¸ Ð¿ÑÐ¾ÐµÐºÑÐ°. Ð ÑÑÐ¾Ð¹ Ð¿Ð°Ð¿ÐºÐµ
+Ð±ÑÐ´ÑÑ ÑÑÐ°Ð½Ð¸ÑÑÑÑ Ð¸Ð·Ð¾Ð±ÑÐ°Ð¶ÐµÐ½Ð¸Ñ. 3. ÐÐ»Ñ Ð·Ð°Ð¿ÑÑÐºÐ°
+ÐÐ»Ð¼Ð°Ð²Ð¸Ðº Ð»Ð¾ÐºÐ°Ð»ÑÐ½Ð¾, Ð²ÑÐ¿Ð¾Ð»Ð½Ð¸ÑÐµ ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ: $python
 YPPRPO.py ### ÐÐ°Ð¿ÑÑÐº Ð² Docker ÐºÐ¾Ð½ÑÐµÐ¹Ð½ÐµÑÐµ 1. ÐÐ°Ð³ÑÑÐ·Ð¸ÑÐµ
 Docker Ð¾Ð±ÑÐ°Ð· ÐÐ»Ð¼Ð°Ð²Ð¸Ðº Ð¸Ð· ÑÐµÐ¿Ð¾Ð·Ð¸ÑÐ¾ÑÐ¸Ñ Docker Hub,
-Ð²ÑÐ¿Ð¾Ð»Ð½Ð¸Ð² ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ: docker pull markuslons/almavik 2.
+Ð²ÑÐ¿Ð¾Ð»Ð½Ð¸Ð² ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ: $ docker pull markuslons/almavik 2.
 ÐÐ°Ð¿ÑÑÑÐ¸ÑÐµ ÐºÐ¾Ð½ÑÐµÐ¹Ð½ÐµÑ, Ð¸ÑÐ¿Ð¾Ð»ÑÐ·ÑÑ ÑÐ»ÐµÐ´ÑÑÑÑÑ
-ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ: docker run -it markuslons/almavik ### ÐÐ°Ð¿ÑÑÐº ÑÐµÑÐµÐ·
-pip Ð¢ÑÑ ÑÐ¸Ð¿Ð¾ Ð²Ð¸ÐºÐ° ## Ð¡ÑÑÐ»ÐºÐ¸ https://pypi.org/project/almavik/
-https://hub.docker.com/repository/docker/markuslons/almavik
+ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ: $ docker run -it markuslons/almavik ### ÐÐ°Ð¿ÑÑÐº ÑÐµÑÐµÐ·
+pip Ð¢ÑÑ ÑÐ¸Ð¿Ð¾ Ð²Ð¸ÐºÐ°
+                     [Markus]  [Blubbery]  [Viktoriatix]
+                      Markus    Blubbery    Viktoriatix
+## Ð¡ÑÑÐ»ÐºÐ¸ https://pypi.org/project/almavik/ https://hub.docker.com/
+repository/docker/markuslons/almavik
```

### Comparing `almavik-4.1/almavik.egg-info/PKG-INFO` & `almavik-4.2/almavik.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: almavik
-Version: 4.1
+Version: 4.2
 Summary: Determination of the drop trajectory
 Home-page: https://github.com/markusLons/almavik
 Author: Markus.Alinas.Viktorias
 Author-email: v.tikhonova@g.nsu.ru
-Classifier: Development Status :: 3 - Alpha
 Description-Content-Type: text/markdown
 
 # Алмавик
 
 ![Логотип Алмавик](formalization/logoza.png)
 <br>
 <div>
@@ -31,21 +30,51 @@
 
 ## Использование
 
 ### Установка
 
 ## Запуск
 ### Локальный запуск 
-Для установки и запуска Алмавик и его зависимостей, выполните следующие шаги:
-    1. Установите зависимости из файла requirements.txt, выполнив команду: pip install -r requirements.txt
+    1. Установите зависимости из файла requirements.txt, выполнив команду: 
+    $ pip install -r requirements.txt
     2. Создайте папку "exp1" в корневой директории проекта. В этой папке будут храниться изображения.
-    3. Для запуска Алмавик локально, выполните команду: python YPPRPO.py
+    3. Для запуска Алмавик локально, выполните команду:
+    $python YPPRPO.py
 ### Запуск в Docker контейнере
-    1. Загрузите Docker образ Алмавик из репозитория Docker Hub, выполнив команду: docker pull markuslons/almavik
-    2. Запустите контейнер, используя следующую команду: docker run -it markuslons/almavik
+    1. Загрузите Docker образ Алмавик из репозитория Docker Hub, выполнив команду: 
+    $ docker pull markuslons/almavik
+    2. Запустите контейнер, используя следующую команду: 
+    $ docker run -it markuslons/almavik
 ### Запуск через pip
 Тут типо вика 
+<div align="center">
+  <table>
+    <tr>
+      <td align="center">
+        <a href="ссылка/на/маркус">
+          <img src="formalization/markus.jpg" width="200px" alt="Markus">
+        </a>
+        <br />
+        <sub><b>Markus</b></sub>
+      </td>
+      <td align="center">
+        <a href="ссылка/на/blubbery">
+          <img src="formalization/blubbery.jpg" width="200px" alt="Blubbery">
+        </a>
+        <br />
+        <sub><b>Blubbery</b></sub>
+      </td>
+      <td align="center">
+        <a href="ссылка/на/viktoriatix">
+          <img src="formalization/viktoriatix.jpg" width="200px" alt="Viktoriatix">
+        </a>
+        <br />
+        <sub><b>Viktoriatix</b></sub>
+      </td>
+    </tr>
+  </table>
+</div>
 
 
 ## Ссылки
 https://pypi.org/project/almavik/
 https://hub.docker.com/repository/docker/markuslons/almavik
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: almavik Version: 4.1 Summary: Determination of the
+Metadata-Version: 2.1 Name: almavik Version: 4.2 Summary: Determination of the
 drop trajectory Home-page: https://github.com/markusLons/almavik Author:
-Markus.Alinas.Viktorias Author-email: v.tikhonova@g.nsu.ru Classifier:
-Development Status :: 3 - Alpha Description-Content-Type: text/markdown #
-ÐÐ»Ð¼Ð°Ð²Ð¸Ðº ![ÐÐ¾Ð³Ð¾ÑÐ¸Ð¿ ÐÐ»Ð¼Ð°Ð²Ð¸Ðº](formalization/logoza.png)
+Markus.Alinas.Viktorias Author-email: v.tikhonova@g.nsu.ru Description-Content-
+Type: text/markdown # ÐÐ»Ð¼Ð°Ð²Ð¸Ðº ![ÐÐ¾Ð³Ð¾ÑÐ¸Ð¿ ÐÐ»Ð¼Ð°Ð²Ð¸Ðº]
+(formalization/logoza.png)
 [Docker_Pulls] [PyPi_Pulls]
 
 ÐÐ»Ð¼Ð°Ð²Ð¸Ðº - Ð¿ÑÐ¾Ð³ÑÐ°Ð¼Ð¼Ð° Ð´Ð»Ñ Ð¾Ð¿ÑÐµÐ´ÐµÐ»ÐµÐ½Ð¸Ñ ÑÐµÐ½ÑÑÐ°
 Ð¼Ð°ÑÑ ÐºÐ°Ð¿Ð»Ð¸ Ð¿Ð¾ Ð¸Ð·Ð¾Ð±ÑÐ°Ð¶ÐµÐ½Ð¸Ñ. ÐÐ½Ð°
 Ð¿ÑÐµÐ´Ð¾ÑÑÐ°Ð²Ð»ÑÐµÑ ÑÐ´Ð¾Ð±Ð½ÑÐ¹ Ð¸Ð½ÑÐµÑÑÐµÐ¹Ñ Ð¸ ÑÑÐ½ÐºÑÐ¸Ð¸
 Ð¾Ð±ÑÐ°Ð±Ð¾ÑÐºÐ¸ Ð¸Ð·Ð¾Ð±ÑÐ°Ð¶ÐµÐ½Ð¸Ð¹, ÐºÐ¾ÑÐ¾ÑÑÐµ Ð¿Ð¾Ð·Ð²Ð¾Ð»ÑÑÑ
 ÑÐ¾ÑÐ½Ð¾ Ð¸ Ð±ÑÑÑÑÐ¾ Ð¾Ð¿ÑÐµÐ´ÐµÐ»Ð¸ÑÑ ÑÐµÐ½ÑÑ Ð¼Ð°ÑÑ ÐºÐ°Ð¿Ð»Ð¸.
@@ -19,22 +19,23 @@
 Ð»ÐµÐ³ÐºÐ¾ Ð·Ð°Ð³ÑÑÐ¶Ð°ÑÑ Ð¸Ð·Ð¾Ð±ÑÐ°Ð¶ÐµÐ½Ð¸Ñ Ð¸
 Ð¿ÑÐ¾ÑÐ¼Ð°ÑÑÐ¸Ð²Ð°ÑÑ ÑÐµÐ·ÑÐ»ÑÑÐ°ÑÑ Ð¾Ð±ÑÐ°Ð±Ð¾ÑÐºÐ¸. -
 **ÐÑÐ°ÑÐ¸ÑÐµÑÐºÐ¾Ðµ Ð¿ÑÐµÐ´ÑÑÐ°Ð²Ð»ÐµÐ½Ð¸Ðµ**: ÐÐ»Ð¼Ð°Ð²Ð¸Ðº
 Ð¿ÑÐµÐ´Ð¾ÑÑÐ°Ð²Ð»ÑÐµÑ Ð³ÑÐ°ÑÐ¸ÑÐµÑÐºÐ¾Ðµ Ð¿ÑÐµÐ´ÑÑÐ°Ð²Ð»ÐµÐ½Ð¸Ðµ
 ÐºÐ°Ð¿Ð»Ð¸, Ð¿Ð¾Ð·Ð²Ð¾Ð»ÑÑ Ð²Ð¸Ð·ÑÐ°Ð»ÑÐ½Ð¾ Ð¾ÑÐµÐ½Ð¸ÑÑ ÐµÐµ ÑÐ¾ÑÐ¼Ñ
 Ð¸ ÑÐ°Ð·Ð¼ÐµÑ. ![ÐÐ¾Ð³Ð¾ÑÐ¸Ð¿ ÐÐ»Ð¼Ð°Ð²Ð¸Ðº](formalization/int.jpg) ##
 ÐÑÐ¿Ð¾Ð»ÑÐ·Ð¾Ð²Ð°Ð½Ð¸Ðµ ### Ð£ÑÑÐ°Ð½Ð¾Ð²ÐºÐ° ## ÐÐ°Ð¿ÑÑÐº ###
-ÐÐ¾ÐºÐ°Ð»ÑÐ½ÑÐ¹ Ð·Ð°Ð¿ÑÑÐº ÐÐ»Ñ ÑÑÑÐ°Ð½Ð¾Ð²ÐºÐ¸ Ð¸ Ð·Ð°Ð¿ÑÑÐºÐ°
-ÐÐ»Ð¼Ð°Ð²Ð¸Ðº Ð¸ ÐµÐ³Ð¾ Ð·Ð°Ð²Ð¸ÑÐ¸Ð¼Ð¾ÑÑÐµÐ¹, Ð²ÑÐ¿Ð¾Ð»Ð½Ð¸ÑÐµ
-ÑÐ»ÐµÐ´ÑÑÑÐ¸Ðµ ÑÐ°Ð³Ð¸: 1. Ð£ÑÑÐ°Ð½Ð¾Ð²Ð¸ÑÐµ Ð·Ð°Ð²Ð¸ÑÐ¸Ð¼Ð¾ÑÑÐ¸
-Ð¸Ð· ÑÐ°Ð¹Ð»Ð° requirements.txt, Ð²ÑÐ¿Ð¾Ð»Ð½Ð¸Ð² ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ: pip install
--r requirements.txt 2. Ð¡Ð¾Ð·Ð´Ð°Ð¹ÑÐµ Ð¿Ð°Ð¿ÐºÑ "exp1" Ð² ÐºÐ¾ÑÐ½ÐµÐ²Ð¾Ð¹
-Ð´Ð¸ÑÐµÐºÑÐ¾ÑÐ¸Ð¸ Ð¿ÑÐ¾ÐµÐºÑÐ°. Ð ÑÑÐ¾Ð¹ Ð¿Ð°Ð¿ÐºÐµ Ð±ÑÐ´ÑÑ
-ÑÑÐ°Ð½Ð¸ÑÑÑÑ Ð¸Ð·Ð¾Ð±ÑÐ°Ð¶ÐµÐ½Ð¸Ñ. 3. ÐÐ»Ñ Ð·Ð°Ð¿ÑÑÐºÐ°
-ÐÐ»Ð¼Ð°Ð²Ð¸Ðº Ð»Ð¾ÐºÐ°Ð»ÑÐ½Ð¾, Ð²ÑÐ¿Ð¾Ð»Ð½Ð¸ÑÐµ ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ: python
+ÐÐ¾ÐºÐ°Ð»ÑÐ½ÑÐ¹ Ð·Ð°Ð¿ÑÑÐº 1. Ð£ÑÑÐ°Ð½Ð¾Ð²Ð¸ÑÐµ Ð·Ð°Ð²Ð¸ÑÐ¸Ð¼Ð¾ÑÑÐ¸
+Ð¸Ð· ÑÐ°Ð¹Ð»Ð° requirements.txt, Ð²ÑÐ¿Ð¾Ð»Ð½Ð¸Ð² ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ: $ pip
+install -r requirements.txt 2. Ð¡Ð¾Ð·Ð´Ð°Ð¹ÑÐµ Ð¿Ð°Ð¿ÐºÑ "exp1" Ð²
+ÐºÐ¾ÑÐ½ÐµÐ²Ð¾Ð¹ Ð´Ð¸ÑÐµÐºÑÐ¾ÑÐ¸Ð¸ Ð¿ÑÐ¾ÐµÐºÑÐ°. Ð ÑÑÐ¾Ð¹ Ð¿Ð°Ð¿ÐºÐµ
+Ð±ÑÐ´ÑÑ ÑÑÐ°Ð½Ð¸ÑÑÑÑ Ð¸Ð·Ð¾Ð±ÑÐ°Ð¶ÐµÐ½Ð¸Ñ. 3. ÐÐ»Ñ Ð·Ð°Ð¿ÑÑÐºÐ°
+ÐÐ»Ð¼Ð°Ð²Ð¸Ðº Ð»Ð¾ÐºÐ°Ð»ÑÐ½Ð¾, Ð²ÑÐ¿Ð¾Ð»Ð½Ð¸ÑÐµ ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ: $python
 YPPRPO.py ### ÐÐ°Ð¿ÑÑÐº Ð² Docker ÐºÐ¾Ð½ÑÐµÐ¹Ð½ÐµÑÐµ 1. ÐÐ°Ð³ÑÑÐ·Ð¸ÑÐµ
 Docker Ð¾Ð±ÑÐ°Ð· ÐÐ»Ð¼Ð°Ð²Ð¸Ðº Ð¸Ð· ÑÐµÐ¿Ð¾Ð·Ð¸ÑÐ¾ÑÐ¸Ñ Docker Hub,
-Ð²ÑÐ¿Ð¾Ð»Ð½Ð¸Ð² ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ: docker pull markuslons/almavik 2.
+Ð²ÑÐ¿Ð¾Ð»Ð½Ð¸Ð² ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ: $ docker pull markuslons/almavik 2.
 ÐÐ°Ð¿ÑÑÑÐ¸ÑÐµ ÐºÐ¾Ð½ÑÐµÐ¹Ð½ÐµÑ, Ð¸ÑÐ¿Ð¾Ð»ÑÐ·ÑÑ ÑÐ»ÐµÐ´ÑÑÑÑÑ
-ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ: docker run -it markuslons/almavik ### ÐÐ°Ð¿ÑÑÐº ÑÐµÑÐµÐ·
-pip Ð¢ÑÑ ÑÐ¸Ð¿Ð¾ Ð²Ð¸ÐºÐ° ## Ð¡ÑÑÐ»ÐºÐ¸ https://pypi.org/project/almavik/
-https://hub.docker.com/repository/docker/markuslons/almavik
+ÐºÐ¾Ð¼Ð°Ð½Ð´Ñ: $ docker run -it markuslons/almavik ### ÐÐ°Ð¿ÑÑÐº ÑÐµÑÐµÐ·
+pip Ð¢ÑÑ ÑÐ¸Ð¿Ð¾ Ð²Ð¸ÐºÐ°
+                     [Markus]  [Blubbery]  [Viktoriatix]
+                      Markus    Blubbery    Viktoriatix
+## Ð¡ÑÑÐ»ÐºÐ¸ https://pypi.org/project/almavik/ https://hub.docker.com/
+repository/docker/markuslons/almavik
```

### Comparing `almavik-4.1/setup.py` & `almavik-4.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 from setuptools import setup
 from io import open
 
 setup(
     name='almavik',
-    version='4.1',
+    version='4.2',
     description='Determination of the drop trajectory',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/markusLons/almavik',
     author='Markus.Alinas.Viktorias',
     author_email='v.tikhonova@g.nsu.ru',
     packages=['src', 'exp1'],
     package_data={'almavik.exp1': ['*.jpeg']},
     install_requires=[
         'opencv-python',
         'numpy',
         'PyQt5',
         'matplotlib',
     ],
-    classifiers=[
-        "Development Status :: 3 - Alpha",
-    ]
 )
```

### Comparing `almavik-4.1/src/YPPRPO.py` & `almavik-4.2/src/YPPRPO.py`

 * *Files identical despite different names*

### Comparing `almavik-4.1/src/detectorDrop.py` & `almavik-4.2/src/detectorDrop.py`

 * *Files identical despite different names*

### Comparing `almavik-4.1/src/widgets.py` & `almavik-4.2/src/widgets.py`

 * *Files identical despite different names*

