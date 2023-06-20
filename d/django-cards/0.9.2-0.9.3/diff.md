# Comparing `tmp/django-cards-0.9.2.tar.gz` & `tmp/django-cards-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-cards-0.9.2.tar", last modified: Mon Jun 19 15:49:40 2023, max compression
+gzip compressed data, was "django-cards-0.9.3.tar", last modified: Tue Jun 20 11:28:39 2023, max compression
```

## Comparing `django-cards-0.9.2.tar` & `django-cards-0.9.3.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-19 15:49:40.882409 django-cards-0.9.2/
--rw-r--r--   0 tom        (501) staff       (20)     1069 2023-01-16 09:53:41.000000 django-cards-0.9.2/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)       55 2023-01-16 09:53:41.000000 django-cards-0.9.2/MANIFEST.in
--rw-r--r--   0 tom        (501) staff       (20)      588 2023-06-19 15:49:40.882028 django-cards-0.9.2/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      130 2023-01-16 09:53:41.000000 django-cards-0.9.2/README.md
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-19 15:49:40.813541 django-cards-0.9.2/cards/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      166 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/apps.py
--rw-r--r--   0 tom        (501) staff       (20)    26056 2023-05-17 09:12:45.000000 django-cards-0.9.2/cards/base.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-19 15:49:40.816792 django-cards-0.9.2/cards/card_list/
--rw-r--r--   0 tom        (501) staff       (20)      115 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/card_list/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     5753 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/card_list/base.py
--rw-r--r--   0 tom        (501) staff       (20)     3952 2023-02-20 18:38:25.000000 django-cards-0.9.2/cards/card_list/main.py
--rw-r--r--   0 tom        (501) staff       (20)     2468 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/card_list/tree.py
--rw-r--r--   0 tom        (501) staff       (20)      714 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/includes.py
--rw-r--r--   0 tom        (501) staff       (20)     5294 2023-06-19 15:48:35.000000 django-cards-0.9.2/cards/standard.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-19 15:49:40.797833 django-cards-0.9.2/cards/static/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-19 15:49:40.797927 django-cards-0.9.2/cards/static/cards/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-19 15:49:40.798821 django-cards-0.9.2/cards/static/cards/jstree/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-19 15:49:40.798169 django-cards-0.9.2/cards/static/cards/jstree/css/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-19 15:49:40.798493 django-cards-0.9.2/cards/static/cards/jstree/css/themes/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-19 15:49:40.835529 django-cards-0.9.2/cards/static/cards/jstree/css/themes/default/
--rw-r--r--   0 tom        (501) staff       (20)     5660 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/static/cards/jstree/css/themes/default/32px.png
--rw-r--r--   0 tom        (501) staff       (20)     2215 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/static/cards/jstree/css/themes/default/40px.png
--rw-r--r--   0 tom        (501) staff       (20)    31722 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/static/cards/jstree/css/themes/default/style.css
--rw-r--r--   0 tom        (501) staff       (20)    27353 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/static/cards/jstree/css/themes/default/style.min.css
--rw-r--r--   0 tom        (501) staff       (20)     1464 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/static/cards/jstree/css/themes/default/throbber.gif
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-19 15:49:40.844440 django-cards-0.9.2/cards/static/cards/jstree/css/themes/default-dark/
--rw-r--r--   0 tom        (501) staff       (20)     1525 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/static/cards/jstree/css/themes/default-dark/32px.png
--rw-r--r--   0 tom        (501) staff       (20)     6526 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/static/cards/jstree/css/themes/default-dark/40px.png
--rw-r--r--   0 tom        (501) staff       (20)    34459 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/static/cards/jstree/css/themes/default-dark/style.css
--rw-r--r--   0 tom        (501) staff       (20)    29959 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/static/cards/jstree/css/themes/default-dark/style.min.css
--rw-r--r--   0 tom        (501) staff       (20)     1464 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/static/cards/jstree/css/themes/default-dark/throbber.gif
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-19 15:49:40.847991 django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/
--rw-r--r--   0 tom        (501) staff       (20)     6423 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/30px.png
--rw-r--r--   0 tom        (501) staff       (20)     3333 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/32px.png
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-19 15:49:40.798704 django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/fonts/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-19 15:49:40.862990 django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/fonts/titillium/
--rw-r--r--   0 tom        (501) staff       (20)    24108 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.eot
--rw-r--r--   0 tom        (501) staff       (20)   134830 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.svg
--rw-r--r--   0 tom        (501) staff       (20)    49936 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.ttf
--rw-r--r--   0 tom        (501) staff       (20)    27344 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.woff
--rw-r--r--   0 tom        (501) staff       (20)    24056 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.eot
--rw-r--r--   0 tom        (501) staff       (20)   140377 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.svg
--rw-r--r--   0 tom        (501) staff       (20)    50224 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.ttf
--rw-r--r--   0 tom        (501) staff       (20)    27108 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.woff
--rw-r--r--   0 tom        (501) staff       (20)    25059 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.eot
--rw-r--r--   0 tom        (501) staff       (20)   150837 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.svg
--rw-r--r--   0 tom        (501) staff       (20)    50788 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.ttf
--rw-r--r--   0 tom        (501) staff       (20)    28152 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.woff
--rw-r--r--   0 tom        (501) staff       (20)    32574 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/style.css
--rw-r--r--   0 tom        (501) staff       (20)    27752 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/style.min.css
--rw-r--r--   0 tom        (501) staff       (20)     1720 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/throbber.gif
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-19 15:49:40.864443 django-cards-0.9.2/cards/static/cards/jstree/js/
--rw-r--r--   0 tom        (501) staff       (20)   307794 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/static/cards/jstree/js/jstree.js
--rw-r--r--   0 tom        (501) staff       (20)   141222 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/static/cards/jstree/js/jstree.min.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-19 15:49:40.799026 django-cards-0.9.2/cards/templates/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-19 15:49:40.799434 django-cards-0.9.2/cards/templates/cards/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-19 15:49:40.865293 django-cards-0.9.2/cards/templates/cards/groups/
--rw-r--r--   0 tom        (501) staff       (20)      206 2023-01-18 12:35:38.000000 django-cards-0.9.2/cards/templates/cards/groups/groups.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-19 15:49:40.877996 django-cards-0.9.2/cards/templates/cards/standard/
--rw-r--r--   0 tom        (501) staff       (20)       69 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/templates/cards/standard/blank.html
--rw-r--r--   0 tom        (501) staff       (20)     1588 2023-01-26 20:53:02.000000 django-cards-0.9.2/cards/templates/cards/standard/card_group.html
--rw-r--r--   0 tom        (501) staff       (20)     1158 2023-05-05 13:55:45.000000 django-cards-0.9.2/cards/templates/cards/standard/datatable.html
--rw-r--r--   0 tom        (501) staff       (20)      778 2023-05-05 10:39:41.000000 django-cards-0.9.2/cards/templates/cards/standard/default.html
--rw-r--r--   0 tom        (501) staff       (20)     1661 2023-05-17 09:02:56.000000 django-cards-0.9.2/cards/templates/cards/standard/default_body.html
--rw-r--r--   0 tom        (501) staff       (20)     1079 2023-05-05 13:55:45.000000 django-cards-0.9.2/cards/templates/cards/standard/html.html
--rw-r--r--   0 tom        (501) staff       (20)     2606 2023-05-05 13:55:45.000000 django-cards-0.9.2/cards/templates/cards/standard/list_selection.html
--rw-r--r--   0 tom        (501) staff       (20)      576 2023-05-05 11:16:16.000000 django-cards-0.9.2/cards/templates/cards/standard/message.html
--rw-r--r--   0 tom        (501) staff       (20)      859 2023-05-05 11:16:16.000000 django-cards-0.9.2/cards/templates/cards/standard/table.html
--rw-r--r--   0 tom        (501) staff       (20)     1547 2023-05-19 09:31:19.000000 django-cards-0.9.2/cards/templates/cards/standard/table_body.html
--rw-r--r--   0 tom        (501) staff       (20)     2198 2023-05-05 13:55:45.000000 django-cards-0.9.2/cards/templates/cards/standard/tree_selection.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-19 15:49:40.878814 django-cards-0.9.2/cards/templatetags/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/templatetags/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)      362 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/templatetags/django_cards_tags.py
--rw-r--r--   0 tom        (501) staff       (20)      115 2023-01-16 09:53:41.000000 django-cards-0.9.2/cards/url_converters.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-19 15:49:40.881471 django-cards-0.9.2/django_cards.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)      588 2023-06-19 15:49:40.000000 django-cards-0.9.2/django_cards.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)     3065 2023-06-19 15:49:40.000000 django-cards-0.9.2/django_cards.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-19 15:49:40.000000 django-cards-0.9.2/django_cards.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)        6 2023-06-19 15:49:40.000000 django-cards-0.9.2/django_cards.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)       38 2023-06-19 15:49:40.882536 django-cards-0.9.2/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)      645 2023-06-19 15:48:54.000000 django-cards-0.9.2/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.590906 django-cards-0.9.3/
+-rw-r--r--   0 tom        (501) staff       (20)     1069 2023-01-16 09:53:41.000000 django-cards-0.9.3/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)       55 2023-01-16 09:53:41.000000 django-cards-0.9.3/MANIFEST.in
+-rw-r--r--   0 tom        (501) staff       (20)      588 2023-06-20 11:28:39.590667 django-cards-0.9.3/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      130 2023-01-16 09:53:41.000000 django-cards-0.9.3/README.md
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.507187 django-cards-0.9.3/cards/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      166 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/apps.py
+-rw-r--r--   0 tom        (501) staff       (20)    26056 2023-05-17 09:12:45.000000 django-cards-0.9.3/cards/base.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.518119 django-cards-0.9.3/cards/card_list/
+-rw-r--r--   0 tom        (501) staff       (20)      115 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/card_list/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     5753 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/card_list/base.py
+-rw-r--r--   0 tom        (501) staff       (20)     3952 2023-02-20 18:38:25.000000 django-cards-0.9.3/cards/card_list/main.py
+-rw-r--r--   0 tom        (501) staff       (20)     2468 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/card_list/tree.py
+-rw-r--r--   0 tom        (501) staff       (20)      714 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/includes.py
+-rw-r--r--   0 tom        (501) staff       (20)     5294 2023-06-19 15:48:35.000000 django-cards-0.9.3/cards/standard.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.495785 django-cards-0.9.3/cards/static/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.495900 django-cards-0.9.3/cards/static/cards/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.496959 django-cards-0.9.3/cards/static/cards/jstree/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.496177 django-cards-0.9.3/cards/static/cards/jstree/css/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.496567 django-cards-0.9.3/cards/static/cards/jstree/css/themes/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.521608 django-cards-0.9.3/cards/static/cards/jstree/css/themes/default/
+-rw-r--r--   0 tom        (501) staff       (20)     5660 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/default/32px.png
+-rw-r--r--   0 tom        (501) staff       (20)     2215 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/default/40px.png
+-rw-r--r--   0 tom        (501) staff       (20)    31722 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/default/style.css
+-rw-r--r--   0 tom        (501) staff       (20)    27353 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/default/style.min.css
+-rw-r--r--   0 tom        (501) staff       (20)     1464 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/default/throbber.gif
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.555163 django-cards-0.9.3/cards/static/cards/jstree/css/themes/default-dark/
+-rw-r--r--   0 tom        (501) staff       (20)     1525 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/default-dark/32px.png
+-rw-r--r--   0 tom        (501) staff       (20)     6526 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/default-dark/40px.png
+-rw-r--r--   0 tom        (501) staff       (20)    34459 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/default-dark/style.css
+-rw-r--r--   0 tom        (501) staff       (20)    29959 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/default-dark/style.min.css
+-rw-r--r--   0 tom        (501) staff       (20)     1464 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/default-dark/throbber.gif
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.558178 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/
+-rw-r--r--   0 tom        (501) staff       (20)     6423 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/30px.png
+-rw-r--r--   0 tom        (501) staff       (20)     3333 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/32px.png
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.496825 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.573556 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/
+-rw-r--r--   0 tom        (501) staff       (20)    24108 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.eot
+-rw-r--r--   0 tom        (501) staff       (20)   134830 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.svg
+-rw-r--r--   0 tom        (501) staff       (20)    49936 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.ttf
+-rw-r--r--   0 tom        (501) staff       (20)    27344 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.woff
+-rw-r--r--   0 tom        (501) staff       (20)    24056 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.eot
+-rw-r--r--   0 tom        (501) staff       (20)   140377 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.svg
+-rw-r--r--   0 tom        (501) staff       (20)    50224 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.ttf
+-rw-r--r--   0 tom        (501) staff       (20)    27108 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.woff
+-rw-r--r--   0 tom        (501) staff       (20)    25059 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.eot
+-rw-r--r--   0 tom        (501) staff       (20)   150837 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.svg
+-rw-r--r--   0 tom        (501) staff       (20)    50788 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.ttf
+-rw-r--r--   0 tom        (501) staff       (20)    28152 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.woff
+-rw-r--r--   0 tom        (501) staff       (20)    32574 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/style.css
+-rw-r--r--   0 tom        (501) staff       (20)    27752 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/style.min.css
+-rw-r--r--   0 tom        (501) staff       (20)     1720 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/throbber.gif
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.574768 django-cards-0.9.3/cards/static/cards/jstree/js/
+-rw-r--r--   0 tom        (501) staff       (20)   307794 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/js/jstree.js
+-rw-r--r--   0 tom        (501) staff       (20)   141222 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/static/cards/jstree/js/jstree.min.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.497211 django-cards-0.9.3/cards/templates/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.498570 django-cards-0.9.3/cards/templates/cards/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.575443 django-cards-0.9.3/cards/templates/cards/groups/
+-rw-r--r--   0 tom        (501) staff       (20)      206 2023-01-18 12:35:38.000000 django-cards-0.9.3/cards/templates/cards/groups/groups.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.586255 django-cards-0.9.3/cards/templates/cards/standard/
+-rw-r--r--   0 tom        (501) staff       (20)       69 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/templates/cards/standard/blank.html
+-rw-r--r--   0 tom        (501) staff       (20)     1588 2023-01-26 20:53:02.000000 django-cards-0.9.3/cards/templates/cards/standard/card_group.html
+-rw-r--r--   0 tom        (501) staff       (20)     2212 2023-06-20 11:24:38.000000 django-cards-0.9.3/cards/templates/cards/standard/datatable.html
+-rw-r--r--   0 tom        (501) staff       (20)      778 2023-05-05 10:39:41.000000 django-cards-0.9.3/cards/templates/cards/standard/default.html
+-rw-r--r--   0 tom        (501) staff       (20)     1661 2023-05-17 09:02:56.000000 django-cards-0.9.3/cards/templates/cards/standard/default_body.html
+-rw-r--r--   0 tom        (501) staff       (20)     1079 2023-05-05 13:55:45.000000 django-cards-0.9.3/cards/templates/cards/standard/html.html
+-rw-r--r--   0 tom        (501) staff       (20)     2606 2023-05-05 13:55:45.000000 django-cards-0.9.3/cards/templates/cards/standard/list_selection.html
+-rw-r--r--   0 tom        (501) staff       (20)      576 2023-05-05 11:16:16.000000 django-cards-0.9.3/cards/templates/cards/standard/message.html
+-rw-r--r--   0 tom        (501) staff       (20)      859 2023-05-05 11:16:16.000000 django-cards-0.9.3/cards/templates/cards/standard/table.html
+-rw-r--r--   0 tom        (501) staff       (20)     1547 2023-05-19 09:31:19.000000 django-cards-0.9.3/cards/templates/cards/standard/table_body.html
+-rw-r--r--   0 tom        (501) staff       (20)     2198 2023-05-05 13:55:45.000000 django-cards-0.9.3/cards/templates/cards/standard/tree_selection.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.587463 django-cards-0.9.3/cards/templatetags/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/templatetags/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      362 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/templatetags/django_cards_tags.py
+-rw-r--r--   0 tom        (501) staff       (20)      115 2023-01-16 09:53:41.000000 django-cards-0.9.3/cards/url_converters.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-20 11:28:39.590114 django-cards-0.9.3/django_cards.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)      588 2023-06-20 11:28:39.000000 django-cards-0.9.3/django_cards.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)     3065 2023-06-20 11:28:39.000000 django-cards-0.9.3/django_cards.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-20 11:28:39.000000 django-cards-0.9.3/django_cards.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)        6 2023-06-20 11:28:39.000000 django-cards-0.9.3/django_cards.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)       38 2023-06-20 11:28:39.590987 django-cards-0.9.3/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)      645 2023-06-20 11:28:10.000000 django-cards-0.9.3/setup.py
```

### Comparing `django-cards-0.9.2/LICENSE` & `django-cards-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/PKG-INFO` & `django-cards-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cards
-Version: 0.9.2
+Version: 0.9.3
 Summary: Django app that allows you make cards
 Home-page: https://github.com/django-advance-utils/django-cards
 Author: Thomas Turner
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-cards-0.9.2/cards/base.py` & `django-cards-0.9.3/cards/base.py`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/card_list/base.py` & `django-cards-0.9.3/cards/card_list/base.py`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/card_list/main.py` & `django-cards-0.9.3/cards/card_list/main.py`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/card_list/tree.py` & `django-cards-0.9.3/cards/card_list/tree.py`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/includes.py` & `django-cards-0.9.3/cards/includes.py`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/standard.py` & `django-cards-0.9.3/cards/standard.py`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/static/cards/jstree/css/themes/default/32px.png` & `django-cards-0.9.3/cards/static/cards/jstree/css/themes/default/32px.png`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/static/cards/jstree/css/themes/default/40px.png` & `django-cards-0.9.3/cards/static/cards/jstree/css/themes/default/40px.png`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/static/cards/jstree/css/themes/default/style.css` & `django-cards-0.9.3/cards/static/cards/jstree/css/themes/default/style.css`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/static/cards/jstree/css/themes/default/style.min.css` & `django-cards-0.9.3/cards/static/cards/jstree/css/themes/default/style.min.css`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/static/cards/jstree/css/themes/default/throbber.gif` & `django-cards-0.9.3/cards/static/cards/jstree/css/themes/default/throbber.gif`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/static/cards/jstree/css/themes/default-dark/32px.png` & `django-cards-0.9.3/cards/static/cards/jstree/css/themes/default-dark/32px.png`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/static/cards/jstree/css/themes/default-dark/40px.png` & `django-cards-0.9.3/cards/static/cards/jstree/css/themes/default-dark/40px.png`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/static/cards/jstree/css/themes/default-dark/style.css` & `django-cards-0.9.3/cards/static/cards/jstree/css/themes/default-dark/style.css`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/static/cards/jstree/css/themes/default-dark/style.min.css` & `django-cards-0.9.3/cards/static/cards/jstree/css/themes/default-dark/style.min.css`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/static/cards/jstree/css/themes/default-dark/throbber.gif` & `django-cards-0.9.3/cards/static/cards/jstree/css/themes/default-dark/throbber.gif`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/30px.png` & `django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/30px.png`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/32px.png` & `django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/32px.png`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.eot` & `django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.svg` & `django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.ttf` & `django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.woff` & `django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.eot` & `django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.svg` & `django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.ttf` & `django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.woff` & `django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-extralight-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.eot` & `django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.svg` & `django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.ttf` & `django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.woff` & `django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/fonts/titillium/titilliumweb-regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/style.css` & `django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/style.css`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/style.min.css` & `django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/style.min.css`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/static/cards/jstree/css/themes/proton/throbber.gif` & `django-cards-0.9.3/cards/static/cards/jstree/css/themes/proton/throbber.gif`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/static/cards/jstree/js/jstree.js` & `django-cards-0.9.3/cards/static/cards/jstree/js/jstree.js`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/static/cards/jstree/js/jstree.min.js` & `django-cards-0.9.3/cards/static/cards/jstree/js/jstree.min.js`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/templates/cards/standard/card_group.html` & `django-cards-0.9.3/cards/templates/cards/standard/card_group.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/templates/cards/standard/datatable.html` & `django-cards-0.9.3/cards/templates/cards/standard/html.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-{% load datatable_tags %}
-
-    <div class="{{ card_css_class }}" id="{{ card.code }}_card" {% if card_css_style %}style="{{ card_css_style }}"{% endif %} data-title="">
+    <div class="{{ card_css_class }}" id="{{ card.code }}" data-title="" {% if card_css_style %}style="{{ card_css_style }}"{% endif %}>
         <div class="card-header">
             <div class="d-flex align-items-center">
                 <h5 class="mr-auto">{{ card.title }}</h5>
                 {{ card.menu.render }}
             </div>
         </div>
-        {{ card.tab_menu.render }}
         <div class="{{ card_body_css_class }}" id="{{ card.code }}_body" {% if card_body_css_style %}style="{{ card_body_css_style }}"{% endif %}>
-            {{ card.extra_card_info.datatable.render|safe }}
+            {{ card.extra_card_info.html|safe }}
         </div>
         {% if card.footer %}
             <div class="card-footer">
                 <small style="text-align: left">{{ card.footer|safe }}</small>
             </div>
         {% endif %}
         {% if card.created_modified_dates %}
```

### Comparing `django-cards-0.9.2/cards/templates/cards/standard/default.html` & `django-cards-0.9.3/cards/templates/cards/standard/default.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/templates/cards/standard/default_body.html` & `django-cards-0.9.3/cards/templates/cards/standard/default_body.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/templates/cards/standard/list_selection.html` & `django-cards-0.9.3/cards/templates/cards/standard/list_selection.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/templates/cards/standard/message.html` & `django-cards-0.9.3/cards/templates/cards/standard/message.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/templates/cards/standard/table.html` & `django-cards-0.9.3/cards/templates/cards/standard/table.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/templates/cards/standard/table_body.html` & `django-cards-0.9.3/cards/templates/cards/standard/table_body.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/cards/templates/cards/standard/tree_selection.html` & `django-cards-0.9.3/cards/templates/cards/standard/tree_selection.html`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/django_cards.egg-info/PKG-INFO` & `django-cards-0.9.3/django_cards.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cards
-Version: 0.9.2
+Version: 0.9.3
 Summary: Django app that allows you make cards
 Home-page: https://github.com/django-advance-utils/django-cards
 Author: Thomas Turner
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-cards-0.9.2/django_cards.egg-info/SOURCES.txt` & `django-cards-0.9.3/django_cards.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-cards-0.9.2/setup.py` & `django-cards-0.9.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django-cards",
-    version="0.9.2",
+    version="0.9.3",
     author="Thomas Turner",
     description="Django app that allows you make cards",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/django-advance-utils/django-cards",
     include_package_data=True,
     packages=['cards'],
```

