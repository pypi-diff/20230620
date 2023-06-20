# Comparing `tmp/polygphys-4.6.9.tar.gz` & `tmp/polygphys-6.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polygphys-4.6.9.tar", last modified: Fri Nov 11 21:28:15 2022, max compression
+gzip compressed data, was "polygphys-6.0.5.tar", last modified: Tue Jun 20 12:44:42 2023, max compression
```

## Comparing `polygphys-4.6.9.tar` & `polygphys-6.0.5.tar`

### file list

```diff
@@ -1,112 +1,113 @@
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2022-11-11 21:28:15.010789 polygphys-4.6.9/
--rw-r--r--   0 emilejetzer   (501) staff       (20)     5759 2022-11-11 21:28:15.011016 polygphys-4.6.9/PKG-INFO
--rw-r--r--   0 emilejetzer   (501) staff       (20)      120 2022-03-03 18:41:47.000000 polygphys-4.6.9/pyproject.toml
--rw-r--r--   0 emilejetzer   (501) staff       (20)      983 2022-11-11 21:28:15.012502 polygphys-4.6.9/setup.cfg
--rw-r--r--   0 emilejetzer   (501) staff       (20)      179 2022-01-12 21:30:35.000000 polygphys-4.6.9/setup.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2022-11-11 21:28:14.946161 polygphys-4.6.9/src/
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2022-11-11 21:28:14.953648 polygphys-4.6.9/src/polygphys/
--rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-06-07 15:09:01.000000 polygphys-4.6.9/src/polygphys/__init__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)       77 2022-06-07 15:09:01.000000 polygphys-4.6.9/src/polygphys/__main__.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2022-11-11 21:28:14.957160 polygphys-4.6.9/src/polygphys/admin/
--rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-06-07 15:09:01.000000 polygphys-4.6.9/src/polygphys/admin/__init__.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2022-11-11 21:28:14.959868 polygphys-4.6.9/src/polygphys/admin/heures/
--rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-07-12 22:02:35.000000 polygphys-4.6.9/src/polygphys/admin/heures/__init__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     3112 2022-07-12 22:02:35.000000 polygphys-4.6.9/src/polygphys/admin/heures/exporter.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)       40 2022-07-12 22:02:35.000000 polygphys-4.6.9/src/polygphys/admin/heures/heures.cfg
--rw-r--r--   0 emilejetzer   (501) staff       (20)     2506 2022-07-12 22:02:35.000000 polygphys-4.6.9/src/polygphys/admin/heures/heures.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2022-11-11 21:28:14.962454 polygphys-4.6.9/src/polygphys/admin/inventaire/
--rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-07-12 22:03:51.000000 polygphys-4.6.9/src/polygphys/admin/inventaire/__init__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)      424 2022-07-12 22:03:51.000000 polygphys-4.6.9/src/polygphys/admin/inventaire/default.cfg
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2022-11-11 21:28:14.966523 polygphys-4.6.9/src/polygphys/admin/inventaire/importer/
--rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-07-12 22:03:51.000000 polygphys-4.6.9/src/polygphys/admin/inventaire/importer/__init__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     7228 2022-08-19 17:01:51.000000 polygphys-4.6.9/src/polygphys/admin/inventaire/importer/importer.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     1722 2022-08-19 17:01:51.000000 polygphys-4.6.9/src/polygphys/admin/inventaire/importer/script.py
--rwxr-xr-x   0 emilejetzer   (501) staff       (20)       51 2022-07-12 22:03:51.000000 polygphys-4.6.9/src/polygphys/admin/inventaire/importer/test_argv.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     2681 2022-08-19 17:01:51.000000 polygphys-4.6.9/src/polygphys/admin/inventaire/importer/test_foreignkey.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     4099 2022-08-19 17:01:51.000000 polygphys-4.6.9/src/polygphys/admin/inventaire/inventaire.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     5913 2022-07-12 22:03:51.000000 polygphys-4.6.9/src/polygphys/admin/inventaire/modeles.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2022-11-11 21:28:14.968903 polygphys-4.6.9/src/polygphys/admin/inventaire/zotero/
--rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-07-12 22:03:51.000000 polygphys-4.6.9/src/polygphys/admin/inventaire/zotero/__init__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)      248 2022-07-12 22:03:51.000000 polygphys-4.6.9/src/polygphys/admin/inventaire/zotero/default.cfg
--rw-r--r--   0 emilejetzer   (501) staff       (20)     1340 2022-08-17 21:05:30.000000 polygphys-4.6.9/src/polygphys/admin/inventaire/zotero/script_zotero.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     2790 2022-07-12 22:03:51.000000 polygphys-4.6.9/src/polygphys/admin/inventaire/zotero/zotero.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2022-11-11 21:28:14.969581 polygphys-4.6.9/src/polygphys/atelier/
--rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-06-07 15:09:01.000000 polygphys-4.6.9/src/polygphys/atelier/__init__.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2022-11-11 21:28:14.973492 polygphys-4.6.9/src/polygphys/atelier/assistant_gcode/
--rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-07-12 22:05:31.000000 polygphys-4.6.9/src/polygphys/atelier/assistant_gcode/__init__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     3978 2022-09-07 18:34:40.000000 polygphys-4.6.9/src/polygphys/atelier/assistant_gcode/assistant_gui.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     1810 2022-09-07 18:34:40.000000 polygphys-4.6.9/src/polygphys/atelier/assistant_gcode/gcode.py
--rwxr-xr-x   0 emilejetzer   (501) staff       (20)     3805 2022-09-07 18:34:40.000000 polygphys-4.6.9/src/polygphys/atelier/assistant_gcode/script_svg.py
--rwxr-xr-x   0 emilejetzer   (501) staff       (20)      989 2022-07-12 22:05:31.000000 polygphys-4.6.9/src/polygphys/atelier/assistant_gcode/script_trous.py
--rwxr-xr-x   0 emilejetzer   (501) staff       (20)     2998 2022-09-07 18:34:40.000000 polygphys-4.6.9/src/polygphys/atelier/assistant_gcode/script_xlsx.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2022-11-11 21:28:14.975483 polygphys-4.6.9/src/polygphys/outils/
--rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-06-07 15:09:01.000000 polygphys-4.6.9/src/polygphys/outils/__init__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)       77 2022-06-07 15:09:01.000000 polygphys-4.6.9/src/polygphys/outils/__main__.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2022-11-11 21:28:14.977404 polygphys-4.6.9/src/polygphys/outils/appareils/
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2022-11-11 21:28:14.979733 polygphys-4.6.9/src/polygphys/outils/appareils/HP/
--rw-r--r--   0 emilejetzer   (501) staff       (20)     5662 2022-06-07 15:09:01.000000 polygphys-4.6.9/src/polygphys/outils/appareils/HP/HP4274A_dev.py
--rwxr-xr-x   0 emilejetzer   (501) staff       (20)    22649 2022-06-07 15:09:01.000000 polygphys-4.6.9/src/polygphys/outils/appareils/HP/HP4274A_lab.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)       44 2022-06-07 15:09:01.000000 polygphys-4.6.9/src/polygphys/outils/appareils/HP/__init__.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2022-11-11 21:28:14.981516 polygphys-4.6.9/src/polygphys/outils/appareils/Thorlabs/
--rw-r--r--   0 emilejetzer   (501) staff       (20)    18260 2022-06-07 15:09:01.000000 polygphys-4.6.9/src/polygphys/outils/appareils/Thorlabs/__init__.py
--rwxr-xr-x   0 emilejetzer   (501) staff       (20)    18260 2022-06-07 15:09:01.000000 polygphys-4.6.9/src/polygphys/outils/appareils/Thorlabs/lab.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     2150 2022-06-07 15:09:01.000000 polygphys-4.6.9/src/polygphys/outils/appareils/__init__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)       24 2022-06-07 15:09:01.000000 polygphys-4.6.9/src/polygphys/outils/appareils/__main__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)       75 2022-06-07 15:09:01.000000 polygphys-4.6.9/src/polygphys/outils/appareils/phs8302.cfg
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2022-11-11 21:28:14.985792 polygphys-4.6.9/src/polygphys/outils/base_de_donnees/
--rw-r--r--   0 emilejetzer   (501) staff       (20)    19409 2022-10-13 19:15:23.000000 polygphys-4.6.9/src/polygphys/outils/base_de_donnees/__init__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     1393 2022-06-07 15:09:01.000000 polygphys-4.6.9/src/polygphys/outils/base_de_donnees/__main__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)       81 2022-06-07 15:09:01.000000 polygphys-4.6.9/src/polygphys/outils/base_de_donnees/default.cfg
--rw-r--r--   0 emilejetzer   (501) staff       (20)     4420 2022-11-11 21:24:31.000000 polygphys-4.6.9/src/polygphys/outils/base_de_donnees/dtypes.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)      806 2022-06-07 15:09:01.000000 polygphys-4.6.9/src/polygphys/outils/base_de_donnees/gestion.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     3503 2022-06-07 15:09:01.000000 polygphys-4.6.9/src/polygphys/outils/base_de_donnees/modeles.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2022-11-11 21:28:14.989970 polygphys-4.6.9/src/polygphys/outils/config/
--rw-r--r--   0 emilejetzer   (501) staff       (20)    10760 2022-06-07 15:09:01.000000 polygphys-4.6.9/src/polygphys/outils/config/__init__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     1079 2022-06-07 15:09:01.000000 polygphys-4.6.9/src/polygphys/outils/config/__main__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)      273 2022-06-07 15:09:01.000000 polygphys-4.6.9/src/polygphys/outils/config/default.cfg
--rw-r--r--   0 emilejetzer   (501) staff       (20)       25 2022-06-07 15:09:01.000000 polygphys-4.6.9/src/polygphys/outils/config/json.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)      113 2022-06-07 15:09:01.000000 polygphys-4.6.9/src/polygphys/outils/config/toml.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)       25 2022-06-07 15:09:01.000000 polygphys-4.6.9/src/polygphys/outils/config/yaml.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2022-11-11 21:28:14.992781 polygphys-4.6.9/src/polygphys/outils/interface_graphique/
--rw-r--r--   0 emilejetzer   (501) staff       (20)     1367 2022-06-07 15:09:01.000000 polygphys-4.6.9/src/polygphys/outils/interface_graphique/__init__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)       64 2022-06-07 15:09:01.000000 polygphys-4.6.9/src/polygphys/outils/interface_graphique/__main__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     4678 2022-06-07 15:09:01.000000 polygphys-4.6.9/src/polygphys/outils/interface_graphique/html.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)    10018 2022-07-12 20:31:46.000000 polygphys-4.6.9/src/polygphys/outils/interface_graphique/tableau.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2022-11-11 21:28:14.994632 polygphys-4.6.9/src/polygphys/outils/interface_graphique/tkinter/
--rw-r--r--   0 emilejetzer   (501) staff       (20)     3263 2022-10-11 20:31:37.000000 polygphys-4.6.9/src/polygphys/outils/interface_graphique/tkinter/__init__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)       59 2022-06-07 15:09:01.000000 polygphys-4.6.9/src/polygphys/outils/interface_graphique/tkinter/__main__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)    18300 2022-06-07 15:09:01.000000 polygphys-4.6.9/src/polygphys/outils/interface_graphique/tkinter/onglets.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     7469 2022-11-09 22:42:30.000000 polygphys-4.6.9/src/polygphys/outils/journal.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2022-11-11 21:28:14.997857 polygphys-4.6.9/src/polygphys/outils/reseau/
--rw-r--r--   0 emilejetzer   (501) staff       (20)     9197 2022-06-07 15:09:01.000000 polygphys-4.6.9/src/polygphys/outils/reseau/__init__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)      172 2022-06-07 15:09:01.000000 polygphys-4.6.9/src/polygphys/outils/reseau/__main__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)    13785 2022-11-10 20:55:59.000000 polygphys-4.6.9/src/polygphys/outils/reseau/courriel.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     3899 2022-09-08 22:15:55.000000 polygphys-4.6.9/src/polygphys/outils/reseau/msforms.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2022-11-11 21:28:14.998606 polygphys-4.6.9/src/polygphys/outils/reseau/serveur/
--rw-r--r--   0 emilejetzer   (501) staff       (20)     2405 2022-06-07 15:09:01.000000 polygphys-4.6.9/src/polygphys/outils/reseau/serveur/__init__.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2022-11-11 21:28:15.002256 polygphys-4.6.9/src/polygphys/serveur/
--rw-r--r--   0 emilejetzer   (501) staff       (20)     9705 2022-11-09 22:44:53.000000 polygphys-4.6.9/src/polygphys/serveur/__init__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     1565 2022-11-09 22:46:26.000000 polygphys-4.6.9/src/polygphys/serveur/__main__.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     2339 2022-11-09 22:10:40.000000 polygphys-4.6.9/src/polygphys/serveur/nouveau_script.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)      102 2022-11-09 21:36:04.000000 polygphys-4.6.9/src/polygphys/serveur/serveur.cfg
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2022-11-11 21:28:15.003076 polygphys-4.6.9/src/polygphys/sst/
--rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-06-07 15:09:01.000000 polygphys-4.6.9/src/polygphys/sst/__init__.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2022-11-11 21:28:15.005931 polygphys-4.6.9/src/polygphys/sst/certificats_laser/
--rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-07-12 22:04:49.000000 polygphys-4.6.9/src/polygphys/sst/certificats_laser/__init__.py
--rwxr-xr-x   0 emilejetzer   (501) staff       (20)     1096 2022-07-12 22:04:49.000000 polygphys-4.6.9/src/polygphys/sst/certificats_laser/nouveau_certificat.cfg
--rw-r--r--   0 emilejetzer   (501) staff       (20)     9741 2022-09-23 19:39:17.000000 polygphys-4.6.9/src/polygphys/sst/certificats_laser/nouveau_certificats.py
--rw-r--r--   0 emilejetzer   (501) staff       (20)     1304 2022-07-12 22:07:57.000000 polygphys-4.6.9/src/polygphys/sst/certificats_laser/vérifier.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2022-11-11 21:28:15.008120 polygphys-4.6.9/src/polygphys/sst/inscriptions_sst/
--rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-07-12 22:04:26.000000 polygphys-4.6.9/src/polygphys/sst/inscriptions_sst/__init__.py
--rwxr-xr-x   0 emilejetzer   (501) staff       (20)      652 2022-07-12 22:04:26.000000 polygphys-4.6.9/src/polygphys/sst/inscriptions_sst/inscription.cfg
--rw-r--r--   0 emilejetzer   (501) staff       (20)     3821 2022-09-22 11:30:09.000000 polygphys-4.6.9/src/polygphys/sst/inscriptions_sst/inscriptions_sst.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2022-11-11 21:28:15.010176 polygphys-4.6.9/src/polygphys/sst/trousses_premiers_soins/
--rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-07-12 22:03:15.000000 polygphys-4.6.9/src/polygphys/sst/trousses_premiers_soins/__init__.py
--rwxr-xr-x   0 emilejetzer   (501) staff       (20)     1450 2022-07-12 22:03:15.000000 polygphys-4.6.9/src/polygphys/sst/trousses_premiers_soins/premiers_soins.cfg
--rw-r--r--   0 emilejetzer   (501) staff       (20)     2744 2022-07-12 22:03:15.000000 polygphys-4.6.9/src/polygphys/sst/trousses_premiers_soins/premiers_soins.py
-drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2022-11-11 21:28:14.956566 polygphys-4.6.9/src/polygphys.egg-info/
--rw-r--r--   0 emilejetzer   (501) staff       (20)     5759 2022-11-11 21:28:14.000000 polygphys-4.6.9/src/polygphys.egg-info/PKG-INFO
--rw-r--r--   0 emilejetzer   (501) staff       (20)     3790 2022-11-11 21:28:14.000000 polygphys-4.6.9/src/polygphys.egg-info/SOURCES.txt
--rw-r--r--   0 emilejetzer   (501) staff       (20)        1 2022-11-11 21:28:14.000000 polygphys-4.6.9/src/polygphys.egg-info/dependency_links.txt
--rw-r--r--   0 emilejetzer   (501) staff       (20)      350 2022-11-11 21:28:14.000000 polygphys-4.6.9/src/polygphys.egg-info/requires.txt
--rw-r--r--   0 emilejetzer   (501) staff       (20)       10 2022-11-11 21:28:14.000000 polygphys-4.6.9/src/polygphys.egg-info/top_level.txt
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.856296 polygphys-6.0.5/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     5760 2023-06-20 12:44:42.856501 polygphys-6.0.5/PKG-INFO
+-rw-r--r--   0 emilejetzer   (501) staff       (20)      120 2022-03-03 18:41:47.000000 polygphys-6.0.5/pyproject.toml
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     5477 2022-04-05 17:13:17.000000 polygphys-6.0.5/readme.md
+-rw-r--r--   0 emilejetzer   (501) staff       (20)      976 2023-06-20 12:44:42.857468 polygphys-6.0.5/setup.cfg
+-rw-r--r--   0 emilejetzer   (501) staff       (20)      179 2022-01-12 21:30:35.000000 polygphys-6.0.5/setup.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.783305 polygphys-6.0.5/src/
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.793734 polygphys-6.0.5/src/polygphys/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/__init__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       77 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/__main__.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.796896 polygphys-6.0.5/src/polygphys/admin/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/admin/__init__.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.799526 polygphys-6.0.5/src/polygphys/admin/heures/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-07-12 22:02:35.000000 polygphys-6.0.5/src/polygphys/admin/heures/__init__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     3112 2022-07-12 22:02:35.000000 polygphys-6.0.5/src/polygphys/admin/heures/exporter.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       40 2022-07-12 22:02:35.000000 polygphys-6.0.5/src/polygphys/admin/heures/heures.cfg
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     2506 2022-07-12 22:02:35.000000 polygphys-6.0.5/src/polygphys/admin/heures/heures.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.802509 polygphys-6.0.5/src/polygphys/admin/inventaire/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-07-12 22:03:51.000000 polygphys-6.0.5/src/polygphys/admin/inventaire/__init__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)      424 2022-07-12 22:03:51.000000 polygphys-6.0.5/src/polygphys/admin/inventaire/default.cfg
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.807113 polygphys-6.0.5/src/polygphys/admin/inventaire/importer/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-07-12 22:03:51.000000 polygphys-6.0.5/src/polygphys/admin/inventaire/importer/__init__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     7228 2022-08-19 17:01:51.000000 polygphys-6.0.5/src/polygphys/admin/inventaire/importer/importer.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     1722 2022-08-19 17:01:51.000000 polygphys-6.0.5/src/polygphys/admin/inventaire/importer/script.py
+-rwxr-xr-x   0 emilejetzer   (501) staff       (20)       51 2022-07-12 22:03:51.000000 polygphys-6.0.5/src/polygphys/admin/inventaire/importer/test_argv.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     2681 2022-08-19 17:01:51.000000 polygphys-6.0.5/src/polygphys/admin/inventaire/importer/test_foreignkey.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     4099 2022-08-19 17:01:51.000000 polygphys-6.0.5/src/polygphys/admin/inventaire/inventaire.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     5913 2022-07-12 22:03:51.000000 polygphys-6.0.5/src/polygphys/admin/inventaire/modeles.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.810058 polygphys-6.0.5/src/polygphys/admin/inventaire/zotero/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-07-12 22:03:51.000000 polygphys-6.0.5/src/polygphys/admin/inventaire/zotero/__init__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)      248 2022-07-12 22:03:51.000000 polygphys-6.0.5/src/polygphys/admin/inventaire/zotero/default.cfg
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     1340 2022-08-17 21:05:30.000000 polygphys-6.0.5/src/polygphys/admin/inventaire/zotero/script_zotero.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     2790 2022-07-12 22:03:51.000000 polygphys-6.0.5/src/polygphys/admin/inventaire/zotero/zotero.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.811185 polygphys-6.0.5/src/polygphys/atelier/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/atelier/__init__.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.814216 polygphys-6.0.5/src/polygphys/atelier/assistant_gcode/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-07-12 22:05:31.000000 polygphys-6.0.5/src/polygphys/atelier/assistant_gcode/__init__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     3978 2022-09-07 18:34:40.000000 polygphys-6.0.5/src/polygphys/atelier/assistant_gcode/assistant_gui.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     1810 2022-09-07 18:34:40.000000 polygphys-6.0.5/src/polygphys/atelier/assistant_gcode/gcode.py
+-rwxr-xr-x   0 emilejetzer   (501) staff       (20)     3805 2022-09-07 18:34:40.000000 polygphys-6.0.5/src/polygphys/atelier/assistant_gcode/script_svg.py
+-rwxr-xr-x   0 emilejetzer   (501) staff       (20)      989 2022-07-12 22:05:31.000000 polygphys-6.0.5/src/polygphys/atelier/assistant_gcode/script_trous.py
+-rwxr-xr-x   0 emilejetzer   (501) staff       (20)     2998 2022-09-07 18:34:40.000000 polygphys-6.0.5/src/polygphys/atelier/assistant_gcode/script_xlsx.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.815884 polygphys-6.0.5/src/polygphys/outils/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/__init__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       77 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/__main__.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.817965 polygphys-6.0.5/src/polygphys/outils/appareils/
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.821020 polygphys-6.0.5/src/polygphys/outils/appareils/HP/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     5662 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/appareils/HP/HP4274A_dev.py
+-rwxr-xr-x   0 emilejetzer   (501) staff       (20)    26130 2023-04-05 13:58:01.000000 polygphys-6.0.5/src/polygphys/outils/appareils/HP/HP4274A_lab.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       44 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/appareils/HP/__init__.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.823208 polygphys-6.0.5/src/polygphys/outils/appareils/Thorlabs/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)    18260 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/appareils/Thorlabs/__init__.py
+-rwxr-xr-x   0 emilejetzer   (501) staff       (20)    18260 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/appareils/Thorlabs/lab.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     2148 2023-04-04 15:27:54.000000 polygphys-6.0.5/src/polygphys/outils/appareils/__init__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       24 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/appareils/__main__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       75 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/appareils/phs8302.cfg
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.829692 polygphys-6.0.5/src/polygphys/outils/base_de_donnees/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)    19409 2022-11-24 21:26:10.000000 polygphys-6.0.5/src/polygphys/outils/base_de_donnees/__init__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     1393 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/base_de_donnees/__main__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       81 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/base_de_donnees/default.cfg
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     4420 2022-11-11 21:24:31.000000 polygphys-6.0.5/src/polygphys/outils/base_de_donnees/dtypes.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)      806 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/base_de_donnees/gestion.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     3503 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/base_de_donnees/modeles.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.834150 polygphys-6.0.5/src/polygphys/outils/config/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)    11277 2023-03-08 16:35:11.000000 polygphys-6.0.5/src/polygphys/outils/config/__init__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     1079 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/config/__main__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)      273 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/config/default.cfg
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       25 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/config/json.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)      113 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/config/toml.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       25 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/config/yaml.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.836634 polygphys-6.0.5/src/polygphys/outils/interface_graphique/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     1367 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/interface_graphique/__init__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       64 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/interface_graphique/__main__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     4678 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/interface_graphique/html.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)    10018 2022-07-12 20:31:46.000000 polygphys-6.0.5/src/polygphys/outils/interface_graphique/tableau.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.838619 polygphys-6.0.5/src/polygphys/outils/interface_graphique/tkinter/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     3263 2022-10-11 20:31:37.000000 polygphys-6.0.5/src/polygphys/outils/interface_graphique/tkinter/__init__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       59 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/interface_graphique/tkinter/__main__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)    18300 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/interface_graphique/tkinter/onglets.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     7480 2023-06-20 12:43:39.000000 polygphys-6.0.5/src/polygphys/outils/journal.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.842295 polygphys-6.0.5/src/polygphys/outils/reseau/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     9197 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/reseau/__init__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)      172 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/reseau/__main__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)    15918 2023-03-31 20:31:02.000000 polygphys-6.0.5/src/polygphys/outils/reseau/courriel.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     4021 2022-11-16 15:28:42.000000 polygphys-6.0.5/src/polygphys/outils/reseau/msforms.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.842930 polygphys-6.0.5/src/polygphys/outils/reseau/serveur/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     2405 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/outils/reseau/serveur/__init__.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.846218 polygphys-6.0.5/src/polygphys/serveur/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     9705 2022-11-09 22:44:53.000000 polygphys-6.0.5/src/polygphys/serveur/__init__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     1565 2022-11-09 22:46:26.000000 polygphys-6.0.5/src/polygphys/serveur/__main__.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     2339 2022-11-09 22:10:40.000000 polygphys-6.0.5/src/polygphys/serveur/nouveau_script.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)      102 2022-11-09 21:36:04.000000 polygphys-6.0.5/src/polygphys/serveur/serveur.cfg
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.847052 polygphys-6.0.5/src/polygphys/sst/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-06-07 15:09:01.000000 polygphys-6.0.5/src/polygphys/sst/__init__.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.849905 polygphys-6.0.5/src/polygphys/sst/certificats_laser/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-07-12 22:04:49.000000 polygphys-6.0.5/src/polygphys/sst/certificats_laser/__init__.py
+-rwxr-xr-x   0 emilejetzer   (501) staff       (20)     1096 2022-07-12 22:04:49.000000 polygphys-6.0.5/src/polygphys/sst/certificats_laser/nouveau_certificat.cfg
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     9741 2022-09-23 19:39:17.000000 polygphys-6.0.5/src/polygphys/sst/certificats_laser/nouveau_certificats.py
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     1304 2022-07-12 22:07:57.000000 polygphys-6.0.5/src/polygphys/sst/certificats_laser/vérifier.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.852129 polygphys-6.0.5/src/polygphys/sst/inscriptions_sst/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-07-12 22:04:26.000000 polygphys-6.0.5/src/polygphys/sst/inscriptions_sst/__init__.py
+-rwxr-xr-x   0 emilejetzer   (501) staff       (20)      652 2022-07-12 22:04:26.000000 polygphys-6.0.5/src/polygphys/sst/inscriptions_sst/inscription.cfg
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     3821 2022-09-22 11:30:09.000000 polygphys-6.0.5/src/polygphys/sst/inscriptions_sst/inscriptions_sst.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.855644 polygphys-6.0.5/src/polygphys/sst/trousses_premiers_soins/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       69 2022-07-12 22:03:15.000000 polygphys-6.0.5/src/polygphys/sst/trousses_premiers_soins/__init__.py
+-rwxr-xr-x   0 emilejetzer   (501) staff       (20)     1450 2022-07-12 22:03:15.000000 polygphys-6.0.5/src/polygphys/sst/trousses_premiers_soins/premiers_soins.cfg
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     2744 2022-07-12 22:03:15.000000 polygphys-6.0.5/src/polygphys/sst/trousses_premiers_soins/premiers_soins.py
+drwxr-xr-x   0 emilejetzer   (501) staff       (20)        0 2023-06-20 12:44:42.796345 polygphys-6.0.5/src/polygphys.egg-info/
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     5760 2023-06-20 12:44:42.000000 polygphys-6.0.5/src/polygphys.egg-info/PKG-INFO
+-rw-r--r--   0 emilejetzer   (501) staff       (20)     3800 2023-06-20 12:44:42.000000 polygphys-6.0.5/src/polygphys.egg-info/SOURCES.txt
+-rw-r--r--   0 emilejetzer   (501) staff       (20)        1 2023-06-20 12:44:42.000000 polygphys-6.0.5/src/polygphys.egg-info/dependency_links.txt
+-rw-r--r--   0 emilejetzer   (501) staff       (20)      342 2023-06-20 12:44:42.000000 polygphys-6.0.5/src/polygphys.egg-info/requires.txt
+-rw-r--r--   0 emilejetzer   (501) staff       (20)       10 2023-06-20 12:44:42.000000 polygphys-6.0.5/src/polygphys.egg-info/top_level.txt
```

### Comparing `polygphys-4.6.9/PKG-INFO` & `polygphys-6.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: polygphys
-Version: 4.6.9
+Version: 6.0.5
 Summary: Outils pour des programmes à l'interne du département de physique de Polytechnique Montréal.
 Author: Émile Jetzer
 Author-email: emile.jetzer@polymtl.ca
-Requires-Python: >=3.9
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # Outils & programmes du département de génie physique de Polytechnique [![Python application](https://github.com/ejetzer/polygphys/actions/workflows/python-app.yml/badge.svg)](https://github.com/ejetzer/polygphys/actions/workflows/python-app.yml) [![CodeQL](https://github.com/ejetzer/polygphys/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/ejetzer/polygphys/actions/workflows/codeql-analysis.yml) [![Upload Python Package](https://github.com/ejetzer/polygphys/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ejetzer/polygphys/actions/workflows/python-publish.yml) [![Documentation Status](https://readthedocs.org/projects/polygphys/badge/?version=latest)](https://polygphys.readthedocs.io/en/latest/?badge=latest)
 
 - Installation via PyPI: https://pypi.org/project/polygphys/
     ```
     pip install polygphys
```

### Comparing `polygphys-4.6.9/setup.cfg` & `polygphys-6.0.5/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [metadata]
 name = polygphys
-version = 4.6.9
+version = 6.0.5
 description = Outils pour des programmes à l'interne du département de physique de Polytechnique Montréal.
 author = Émile Jetzer
 author_email = emile.jetzer@polymtl.ca
 long_description = file: readme.md
 long_description_content_type = text/markdown
 
 [options]
-python_requires = >=3.9
+python_requires = >=3.11
 install_requires = 
 	pandas
 	sqlalchemy
 	openpyxl
 	xlwt
 	gitpython
 	pyserial
@@ -22,15 +22,15 @@
 	zipp
 	importlib_metadata
 	docutils
 	tornado
 	cryptography
 	toml
 	keyring
-	numpy==1.22.1
+	numpy
 	brotli
 	Cython
 	lockfile
 	lxml
 	mock
 	ordereddict
 	protobuf
```

### Comparing `polygphys-4.6.9/src/polygphys/admin/heures/exporter.py` & `polygphys-6.0.5/src/polygphys/admin/heures/exporter.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/admin/heures/heures.py` & `polygphys-6.0.5/src/polygphys/admin/heures/heures.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/admin/inventaire/importer/importer.py` & `polygphys-6.0.5/src/polygphys/admin/inventaire/importer/importer.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/admin/inventaire/importer/script.py` & `polygphys-6.0.5/src/polygphys/admin/inventaire/importer/script.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/admin/inventaire/importer/test_foreignkey.py` & `polygphys-6.0.5/src/polygphys/admin/inventaire/importer/test_foreignkey.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/admin/inventaire/inventaire.py` & `polygphys-6.0.5/src/polygphys/admin/inventaire/inventaire.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/admin/inventaire/modeles.py` & `polygphys-6.0.5/src/polygphys/admin/inventaire/modeles.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/admin/inventaire/zotero/script_zotero.py` & `polygphys-6.0.5/src/polygphys/admin/inventaire/zotero/script_zotero.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/admin/inventaire/zotero/zotero.py` & `polygphys-6.0.5/src/polygphys/admin/inventaire/zotero/zotero.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/atelier/assistant_gcode/assistant_gui.py` & `polygphys-6.0.5/src/polygphys/atelier/assistant_gcode/assistant_gui.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/atelier/assistant_gcode/gcode.py` & `polygphys-6.0.5/src/polygphys/atelier/assistant_gcode/gcode.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/atelier/assistant_gcode/script_svg.py` & `polygphys-6.0.5/src/polygphys/atelier/assistant_gcode/script_svg.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/atelier/assistant_gcode/script_trous.py` & `polygphys-6.0.5/src/polygphys/atelier/assistant_gcode/script_trous.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/atelier/assistant_gcode/script_xlsx.py` & `polygphys-6.0.5/src/polygphys/atelier/assistant_gcode/script_xlsx.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/outils/appareils/HP/HP4274A_dev.py` & `polygphys-6.0.5/src/polygphys/outils/appareils/HP/HP4274A_dev.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/outils/appareils/HP/HP4274A_lab.py` & `polygphys-6.0.5/src/polygphys/outils/appareils/HP/HP4274A_lab.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg,\
     NavigationToolbar2Tk
 
 from numpy import linspace  # Domaine de balayage
 from pandas import DataFrame  # Stockage et manipulation des données
 from matplotlib import pyplot as plt  # Affichage des données
 
+from polygphys.outils.reseau.courriel import Courriel
+
 
 class HP4274AException(Exception):
     """Exception générique pour l'appareil HP4274A."""
 
     pass
 
 
@@ -269,14 +271,50 @@
     ax = plt.gca()
     df.plot(ax=ax)
     plt.title(f'Courbes C-V pour composant {comp}')
     plt.legend()
     plt.savefig(sauvegarde / 'fig.png')
     plt.close(fig)
 
+def dessiner(ax, df, canvas, vb, axes_var):
+    ax.clear()
+    ax.set_axis_on()
+    df.plot(ax=ax, style='.', legend=True)
+    ax.set_xticks(vb, [f'{v:.2e}' for v in vb], rotation=45)
+    cs = linspace(min(df.min()), max(df.max()), 10)
+    ax.set_yticks(cs[::int(len(cs) / 10)],
+                  [f'{c:.2e}' for c in
+                   cs[::int(len(cs) / 10)]])
+    ax.set_xlabel('Potentiel de biais (V)')
+    ax.set_ylabel('Mesure de capacité (F)')
+    
+    if axes_var.get() == 'loglog':
+        ax.set_xscale('log')
+        ax.set_yscale('log')
+    elif axes_var.get() == 'xlog':
+        ax.set_xscale('log')
+        ax.set_yscale('linear')
+    elif axes_var.get() == 'ylog':
+        ax.set_xscale('linear')
+        ax.set_yscale('log')
+    else:
+        ax.set_xscale('linear')
+        ax.set_yscale('linear')
+    
+    canvas.draw()
+
+def partager(df: DataFrame, sauvegarde: Path):
+    'Envoyer les données par courriel'
+    pièces_jointes = tuple(filter(Path.is_file, sauvegarde.iterdir()))
+    courriel = Courriel(destinataire='emile.jetzer@polymtl.ca',
+                        expéditeur='emile.jetzer@polymtl.ca',
+                        objet='Courbes C-V pour PHS8302',
+                        contenu='Courbes C-V (voir les pièces jointes pour les détails).',
+                        pièces_jointes=pièces_jointes)
+    courriel.envoyer('smtp.polymtl.ca')
 
 def exe(root,
         matricule_var,
         ressource_var,
         max_vb_var,
         min_vb_var,
         composante_var,
@@ -286,15 +324,19 @@
         biais_var,
         freq_var,
         delai_var,
         nbr_var,
         res_var,
         stop_var,
         min_freq_var,
-        max_freq_var):
+        max_freq_var,
+        dessiner_a_chaque_var,
+        moy_var,
+        sauvegarde_var,
+        axes_var):
     """
     Prendre une série de mesures.
 
     Parameters
     ----------
     root : TYPE
         DESCRIPTION.
@@ -363,21 +405,24 @@
 
     _ = datetime.datetime.now()
     _ = _.isoformat()
     _ = _.replace(':', '_')
     _ = _.replace('.', '_')
     sauvegarde /= _
     sauvegarde.mkdir()
+    sauvegarde_var.set(str(sauvegarde))
 
     # Enregistrer les paramètres de mesure
     with (sauvegarde / 'details.txt').open('w') as F:
         msg = f'''{nom=}
 {comp=}
 {freqs=}
 {vb=}
+{delai=}
+{moy_var=}
 {nom_ressource=}'''
         print(msg, file=F)
         logging.info(msg)
 
     try:
         # Ouvrir la connection avec l'appareil
         hp4274a = rm.open_resource(nom_ressource)
@@ -393,52 +438,57 @@
         for f in freqs:
             regler_freq(hp4274a, f, delai=delai)
             freq_var.set(f'{f:.2e}')
             root.update()
 
             # Balayage en potentiel
             for v in vb:
+                dessiner_a_chaque_point = dessiner_a_chaque_var.get() == 'Dessiner à chaque point'
+                dessiner_a_chaque_courbe = dessiner_a_chaque_var.get() == 'Dessiner à chaque courbe'
+                dessiner_a_la_fin = dessiner_a_chaque_var.get() == 'Dessiner à la fin'
                 if stop_var.get():
                     stop_var.set(0)
                     raise StopIteration
 
                 res = regler_biais(hp4274a, v, delai=delai)
                 biais_var.set(f'{v:.2e}')
                 root.update()
-                time.sleep(delai)
+                #time.sleep(delai)
                 if res.data_status_A == 'N' or res.value_A < 0:
-                    res = mesure_moyenne(hp4274a, 'A2', 10, delai=delai)
+                    res = mesure_moyenne(hp4274a, 'A2', moy_var.get(), delai=delai)
                     df.loc[v, f] = res
                     res_var.set(res)
 
                     # Clear axis
-                    ax.clear()
-                    ax.set_axis_on()
-                    df.plot(ax=ax, style='.', legend=True)
-                    ax.set_xticks(vb, [f'{v:.2e}' for v in vb], rotation=45)
-                    cs = linspace(min(df.min()), max(df.max()), 10)
-                    ax.set_yticks(cs[::int(len(cs) / 10)],
-                                  [f'{c:.2e}' for c in
-                                   cs[::int(len(cs) / 10)]])
-                    ax.set_xlabel('Potentiel de biais (V)')
-                    ax.set_ylabel('Mesure de capacité (F)')
-                    canvas.draw()
+                    if dessiner_a_chaque_point:
+                        dessiner(ax, df, canvas, vb, axes_var)
+                else:
+                    with (sauvegarde / 'erreurs.txt').open('a') as F:
+                        print(f, v, res, file=F)
+                        logging.info(str(res))
 
                 progres.step()
                 root.update()
+            
+            if dessiner_a_chaque_courbe:
+                dessiner(ax, df, canvas, vb, axes_var)
+
+        if dessiner_a_la_fin:
+            dessiner(ax, df, canvas, vb, axes_var)
 
         enregistrer(df, sauvegarde, comp)
     except StopIteration:
         pass
     except Exception as e:
         msg = f'Une erreur {e!r} est survenue, voir console ou journal.'
         mb.showerror(f'{type(e)}', msg)
         msg += f'\n{traceback.format_exc()}'
         logging.error(msg)
     finally:
+        partager(df, sauvegarde)
         # Toujours fermer la connection à l'appareil
         hp4274a.close()
 
 
 def exe1(root,
          matricule_var,
          ressource_var,
@@ -592,15 +642,19 @@
                                                 biais_var=biais_var,
                                                 freq_var=freq_var,
                                                 delai_var=delai_var,
                                                 nbr_var=nbr_var,
                                                 res_var=res_var,
                                                 stop_var=stop_var,
                                                 min_freq_var=min_freq_var,
-                                                max_freq_var=max_freq_var))
+                                                max_freq_var=max_freq_var,
+                                                dessiner_a_chaque_var=dessiner_a_chaque_var,
+                                                moy_var=moy_var,
+                                                sauvegarde_var=sauvegarde_var,
+                                                axes_var=axes_var))
     exe1_bouton = ttk.Button(root,
                              text='1 mesure',
                              command=lambda: exe1(root=root,
                                                   matricule_var=matricule_var,
                                                   ressource_var=ressource_var,
                                                   max_vb_var=max_vb_var,
                                                   min_vb_var=min_vb_var,
@@ -651,14 +705,16 @@
     # Identification de la série de mesures
     matricule_var = tk.StringVar(root)
     composante_var = tk.StringVar(root)
     matricule_entry = ttk.Entry(root, textvariable=matricule_var)
     matricule_label = ttk.Label(root, text="Matricule")
     composante_entry = ttk.Entry(root, textvariable=composante_var)
     composante_label = ttk.Label(root, text="Composante")
+    sauvegarde_var = tk.StringVar(root)
+    sauvegarde_entry = ttk.Entry(root, textvariable=sauvegarde_var, state=tk.DISABLED)
 
     # Barre de progrès
     progres = ttk.Progressbar(root,
                               orient=tk.HORIZONTAL,
                               maximum=220,
                               mode='determinate')
 
@@ -681,14 +737,27 @@
     delai_label = ttk.Label(root, text='Délai (s)')
     nbr_var = tk.StringVar(root, value=10)
     nbr_entry = ttk.Spinbox(root, increment=1, textvariable=nbr_var)
     nbr_label = ttk.Label(root, text='Nombre de points')
     res_var = tk.StringVar(root)
     res_entry = ttk.Entry(root, textvariable=res_var, state=tk.DISABLED)
     res_label = ttk.Label(root, text='Mesure (F)')
+    moy_var = tk.IntVar(root, value=10)
+    moy_entry = ttk.Spinbox(root, textvariable=moy_var, increment=1)
+    moy_label = ttk.Label(root, text='Nombre de mesures par point (moyenne)')
+    
+    # Paramètres de graphique
+    valeurs = ('Dessiner à chaque point',
+               'Dessiner à chaque courbe',
+               'Dessiner à la fin')
+    dessiner_a_chaque_var = tk.StringVar(root, value=valeurs[0])
+    dessiner_a_chaque_ctl = ttk.Combobox(root, textvariable=dessiner_a_chaque_var, values=valeurs, state='readonly')
+    axes_var = tk.StringVar(root, 'linear')
+    axes_ctl = ttk.Combobox(root, textvariable=axes_var, values=('linear', 'xlog', 'ylog', 'loglog'), state='readonly')
+    axes_lbl = ttk.Label(root, text='Type d\'axes')
 
     # Positionnement
     pad = 5
     label_adresse.grid(row=0, column=0, sticky=tk.E, padx=pad, pady=pad)
     combo_adresse.grid(row=0, column=1, sticky=tk.E + tk.W, padx=pad, pady=pad)
     matricule_label.grid(row=1, column=0, sticky=tk.E, padx=pad, pady=pad)
     matricule_entry.grid(row=1, column=1,
@@ -714,25 +783,34 @@
     biais_entry.grid(row=7, column=1, sticky=tk.E + tk.W, padx=pad, pady=pad)
     freq_label.grid(row=8, column=0, sticky=tk.E, padx=pad, pady=pad)
     freq_entry.grid(row=8, column=1, sticky=tk.E + tk.W, padx=pad, pady=pad)
     delai_label.grid(row=9, column=0, sticky=tk.E, padx=pad, pady=pad)
     delai_entry.grid(row=9, column=1, sticky=tk.E + tk.W, padx=pad, pady=pad)
     nbr_label.grid(row=10, column=0, sticky=tk.E, padx=pad, pady=pad)
     nbr_entry.grid(row=10, column=1, sticky=tk.E + tk.W, padx=pad, pady=pad)
-    res_label.grid(row=11, column=0, sticky=tk.E, padx=pad, pady=pad)
-    res_entry.grid(row=11, column=1, sticky=tk.E + tk.W, padx=pad, pady=pad)
-    exe_bouton.grid(row=12, column=0, sticky=tk.E + tk.W, padx=pad, pady=pad)
-    exe1_bouton.grid(row=12, column=1, sticky=tk.E + tk.W, padx=pad, pady=pad)
-    stop_bouton.grid(row=13, column=0, sticky=tk.E + tk.W, padx=pad, pady=pad)
-    progres.grid(row=14, column=0, columnspan=2,
+    moy_label.grid(row=11, column=0, sticky=tk.E+tk.W, padx=pad, pady=pad)
+    moy_entry.grid(row=11, column=1, sticky=tk.E+tk.W, padx=pad, pady=pad)
+    res_label.grid(row=12, column=0, sticky=tk.E, padx=pad, pady=pad)
+    res_entry.grid(row=12, column=1, sticky=tk.E + tk.W, padx=pad, pady=pad)
+    
+    dessiner_a_chaque_ctl.grid(row=13, column=1, sticky=tk.E+tk.W, padx=pad, pady=pad)
+    axes_lbl.grid(row=14, column=0, sticky=tk.E, padx=pad, pady=pad)
+    axes_ctl.grid(row=14, column=1, sticky=tk.E+tk.W, padx=pad, pady=pad)
+    
+    exe_bouton.grid(row=15, column=0, sticky=tk.E + tk.W, padx=pad, pady=pad)
+    exe1_bouton.grid(row=15, column=1, sticky=tk.E + tk.W, padx=pad, pady=pad)
+    stop_bouton.grid(row=16, column=0, sticky=tk.E + tk.W, padx=pad, pady=pad)
+    progres.grid(row=17, column=0, columnspan=2,
                  sticky=tk.E + tk.W, padx=pad, pady=pad)
+    sauvegarde_entry.grid(row=18, column=0, columnspan=2,
+                 sticky=tk.E+tk.W, padx=pad, pady=pad)
     canvas.get_tk_widget().grid(row=0, column=2,
-                                rowspan=14,
+                                rowspan=18,
                                 padx=pad, pady=pad)
-    barre.grid(row=14, column=2, padx=pad, pady=pad)
+    barre.grid(row=18, column=2, padx=pad, pady=pad)
 
     root.mainloop()
     logging.shutdown()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `polygphys-4.6.9/src/polygphys/outils/appareils/Thorlabs/__init__.py` & `polygphys-6.0.5/src/polygphys/outils/appareils/Thorlabs/__init__.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/outils/appareils/Thorlabs/lab.py` & `polygphys-6.0.5/src/polygphys/outils/appareils/Thorlabs/lab.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/outils/appareils/__init__.py` & `polygphys-6.0.5/src/polygphys/outils/appareils/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     def __init__(self):
         self.rm = visa.ResourceManager()
 
     def list_resources(self):
         return self.rm.list_resources()
 
-    def open(self, nom: str) -> Appareil:
+    def open(self, nom: str) -> object:
         return Appareil(self, nom).open()
 
     def grid(self):
         pass
 
     def pack(self):
         pass
```

### Comparing `polygphys-4.6.9/src/polygphys/outils/base_de_donnees/__init__.py` & `polygphys-6.0.5/src/polygphys/outils/base_de_donnees/__init__.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/outils/base_de_donnees/__main__.py` & `polygphys-6.0.5/src/polygphys/outils/base_de_donnees/__main__.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/outils/base_de_donnees/dtypes.py` & `polygphys-6.0.5/src/polygphys/outils/base_de_donnees/dtypes.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/outils/base_de_donnees/gestion.py` & `polygphys-6.0.5/src/polygphys/outils/base_de_donnees/gestion.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/outils/base_de_donnees/modeles.py` & `polygphys-6.0.5/src/polygphys/outils/base_de_donnees/modeles.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/outils/config/__init__.py` & `polygphys-6.0.5/src/polygphys/outils/config/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Enveloppe pour les fichiers de configuration.
 
 La classe FichierConfig permet de garder un fichier de configuration
 synchronisé quand des modifications y sont faites dans le programme.
 """
 
 # Bibliothèque standard
+import platformdirs
 from io import StringIO  # Pour FichierConfig.__str__
 from pathlib import Path  # Manipulation de chemins
 # Pour parsage d'urls, utilisé dans FichierConfig.__init__
 from urllib.parse import urlparse
 from typing import Any, Callable
 from functools import partial
 
@@ -24,14 +25,17 @@
 
     def __init__(self,
                  chemin: Path,
                  defaults: dict = None,
                  dict_type: type = _default_dict,
                  allow_no_value: bool = False,
                  *,
+                 emplacement_système: bool = False,
+                 platformdirs_func=platformdirs.user_config_dir,
+                 platformdirs_args={},
                  fichier_defaut: Path = Path(__file__).parent / 'default.cfg',
                  delimiters: tuple[str] = ('=', ':'),
                  comment_prefixes: tuple[str] = ('#', ';'),
                  inline_comment_prefixes: tuple[str] = None,
                  strict: bool = True,
                  empty_lines_in_values: bool = True,
                  default_section: str = DEFAULTSECT,
@@ -97,15 +101,22 @@
         -------
         None.
 
         """
         # Principale différence avec ConfigParser:
         # l'attribut chemin réfère au fichier de configuration
         # lu et écrit dans le programme.
-        self.chemin: Path = Path(chemin)
+        chemin = Path(chemin)
+        if emplacement_système and not chemin.is_absolute():
+            if isinstance(platformdirs_func, str):
+                platformdirs_func = getattr(platformdirs, platformdirs_func)
+            racine = platformdirs_func(**platformdirs_args)
+            self.chemin = racine / chemin
+        else:
+            self.chemin: Path = Path(chemin)
 
         # Si le fichier n'existe pas, il est créé,
         # et on lui donne la valeur par défaut,
         # telle que définie par la méthode défaut
         self.fichier_defaut: Path = fichier_defaut
         if not self.chemin.exists():
             self.chemin.touch()
```

### Comparing `polygphys-4.6.9/src/polygphys/outils/config/__main__.py` & `polygphys-6.0.5/src/polygphys/outils/config/__main__.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/outils/interface_graphique/__init__.py` & `polygphys-6.0.5/src/polygphys/outils/interface_graphique/__init__.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/outils/interface_graphique/html.py` & `polygphys-6.0.5/src/polygphys/outils/interface_graphique/html.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/outils/interface_graphique/tableau.py` & `polygphys-6.0.5/src/polygphys/outils/interface_graphique/tableau.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/outils/interface_graphique/tkinter/__init__.py` & `polygphys-6.0.5/src/polygphys/outils/interface_graphique/tkinter/__init__.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/outils/interface_graphique/tkinter/onglets.py` & `polygphys-6.0.5/src/polygphys/outils/interface_graphique/tkinter/onglets.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/outils/journal.py` & `polygphys-6.0.5/src/polygphys/outils/journal.py`

 * *Files 2% similar despite different names*

```diff
@@ -324,10 +324,10 @@
         else:
             en_têtes = True
             csv.touch()
 
         message.to_csv(csv, mode='a', header=en_têtes, index=False)
         self.repo.add(csv.name)
 
-        self.repo.commit(msg, '-a')
+        self.repo.commit(msg, '-a', '--amend')
 
 # TODO Modèle de base de données pour journal
```

### Comparing `polygphys-4.6.9/src/polygphys/outils/reseau/__init__.py` & `polygphys-6.0.5/src/polygphys/outils/reseau/__init__.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/outils/reseau/courriel.py` & `polygphys-6.0.5/src/polygphys/outils/reseau/courriel.py`

 * *Files 4% similar despite different names*

```diff
@@ -127,15 +127,16 @@
     def __init__(self,
                  destinataire=None,
                  expéditeur=None,
                  objet=None,
                  contenu=None,
                  html=None,
                  pièces_jointes=tuple(),
-                 message: EmailMessage = None):
+                 message: EmailMessage = None,
+                 boîte=None):
         if message:
             self.message = message
         else:
             self.message = EmailMessage()
 
         if destinataire is not None:
             self.destinataire = destinataire
@@ -144,14 +145,16 @@
         if objet is not None:
             self.objet = objet
         if contenu is not None:
             self.contenu = contenu
         if html is not None:
             self.html = html
 
+        self.boîte = boîte
+
         if pièces_jointes:
             self.joindre(*pièces_jointes)
 
     def __getitem__(self, clé: Any) -> Any:
         return self.message[clé]
 
     def __setitem__(self, clé: Any, val: Any) -> Any:
@@ -194,16 +197,25 @@
     @property
     def pièces_jointes(self):
         if self.is_multipart() and len(self.get_payload()) > 1:
             for pj in self.get_payload():
                 if pj.get('Content-Disposition', '').startswith('attachment'):
                     nom = pj.get_filename()
                     content_type = pj.get_content_type()
+                    if nom is None:
+                        continue
+                    elif isinstance(nom, bytes):
+                        nom = str(nom, encoding='utf-8')
+                    # print(nom, content_type, pj.get_charset())
+                    # De temps en temps il y a une erreur ici,
+                    # Je ne sais pas pourquoi.
                     pj.set_charset('utf-8')
                     contenu = pj.get_payload(decode=True)
+                    if contenu is None:
+                        continue
                     yield PièceJointe(nom, content_type, contenu)
 
     def envoyer(self, adresse, port=25):
         serveur = smtplib.SMTP(adresse, port)
         serveur.send_message(self.message)
         serveur.quit()
 
@@ -213,26 +225,29 @@
             return dateutil.parser.parse(self['Date'], ignoretz=True)
         else:
             return None
 
     @property
     def contenu(self):
         contenu = self.message.get_body(('plain', 'html', 'related'))
+        charset = contenu.get_charset()
 
         if contenu is None:
             contenu = f'{contenu!r}'
         else:
             contenu = contenu.get_payload()
 
         if contenu.isascii():
             contenu = quopri.decodestring(contenu.encode('utf-8'))
 
             encodings = ('utf-8',
                          'cp1252',
                          chardet.detect(contenu)['encoding'])
+            if charset is not None:
+                encodings = (charset,) + encodings
             for encoding in encodings:
                 try:
                     contenu = contenu.decode(encoding)
                 except UnicodeDecodeError:
                     logging.exception(f'{encoding} ne fonctionne pas.')
                 else:
                     break
@@ -255,15 +270,18 @@
 
         nom = nom.strip('_')
 
         return nom
 
     @property
     def name(self) -> str:
-        sujet: str = self['Subject']\
+        sujet = self['Subject']
+        if sujet is None:
+            sujet = 'Sujet vide'
+        sujet: str = sujet\
             .encode('ascii', 'ignore')\
             .decode('utf-8')\
             .strip()
 
         sujet = self.nettoyer_nom(sujet)
 
         return sujet + '.md'
@@ -284,34 +302,44 @@
         return Path(nom)
 
     @property
     def path(self):
         return self.parent / self.name
 
     def __str__(self):
+        date = self.date if self.date is not None else datetime(1970, 1, 1)
         return f'''- - -
-Date: {self.date.isoformat()}
+Date: {date.isoformat()}
 De: {self['From']}
 À: {self['To']}
 Sujet: {self['Subject']}
+aliases:
+    - "{self['Subject']}"
+tags: courriel
+- - -
 
 {self.contenu}
 '''
 
-    def sauver(self, dossier: Path):
+    def sauver(self, dossier: Path, pièces_jointes: bool = True):
         chemin = dossier / self.path
 
         if not chemin.parent.exists():
             chemin.parent.mkdir()
         if not chemin.exists():
             chemin.touch()
 
         with chemin.open('w', encoding='utf-8') as f:
             f.write(str(self))
 
+        if pièces_jointes == True:
+            for pj in self.pièces_jointes:
+                with (chemin.parent / pj.nom).open('wb') as f:
+                    f.write(pj.contenu)
+
 
 BoîteAuxLettres = namedtuple('BoîteAuxLettres', ['est_parent',
                                                  'sep',
                                                  'nom'])
 
 
 class Messagerie:
@@ -320,14 +348,15 @@
         if isinstance(config, (str, Path)):
             self.config = CourrielsConfig(config)
         else:
             self.config = config
 
         self._mdp = None
         self.sélection = 'INBOX'
+        self.boîte = 'INBOX'
 
     @property
     def adresse(self):
         return self.config.get('messagerie', 'adresse')
 
     @property
     def nom(self):
@@ -346,15 +375,15 @@
         return self._mdp
 
     def message(self, serveur: IMAP4_SSL, numéro: str) -> Courriel:
         typ, data = serveur.fetch(numéro, '(RFC822)')
         message = email.parser.BytesParser(policy=email.policy.default)\
             .parsebytes(bytes(data[0][1]))
 
-        return Courriel(message=message)
+        return Courriel(message=message, boîte=self.boîte)
 
     def messages(self, *recherche) -> Courriel:
         if not recherche:
             recherche = ('ALL',)
         with self.connecter() as serveur:
             serveur.select(self.sélection)
             typ, data = serveur.search(None, *recherche)
@@ -384,29 +413,48 @@
                 if b.nom == boîte:
                     boîte = b
             if isinstance(boîte, str):
                 raise ValueError('Cette boîte aux lettres n\'existe pas.')
 
         nom, l = encode_imap4_utf7(boîte.nom)
         self.sélection = '"{}"'.format(nom)
+        self.boîte = boîte
 
     @ property
     def df(self) -> pandas.DataFrame:
         return pandas.DataFrame([[c.date,
                                   c['Subject'],
                                   c['From'],
                                   c['To'],
                                   c.parent.name,
-                                  c.contenu] for c in self],
+                                  c.contenu,
+                                  c.boîte.nom] for c in self],
+                                columns=('date',
+                                         'sujet',
+                                         'de',
+                                         'a',
+                                         'chaine',
+                                         'contenu',
+                                         'dossier'))
+
+    def df_filtré(self, *critères) -> pandas.DataFrame:
+        return pandas.DataFrame([[c.date,
+                                  c['Subject'],
+                                  c['From'],
+                                  c['To'],
+                                  c.parent.name,
+                                  c.contenu,
+                                  c.boîte.nom] for c in self.messages(*critères)],
                                 columns=('date',
                                          'sujet',
                                          'de',
                                          'a',
                                          'chaine',
-                                         'contenu'))
+                                         'contenu',
+                                         'dossier'))
 
     def connecter(self):
         serveur = IMAP4_SSL(self.adresse)
         serveur.login(self.nom, self.mdp)
         serveur.enable('UTF-8=ACCEPT')
         return serveur
 
@@ -420,27 +468,29 @@
             self.config = config
 
         db = self.config.get('db', 'adresse')
         table = 'courriels'
 
         super().__init__(db, table)
 
-    def ajouter_messagerie(self, messagerie: Messagerie):
+    def ajouter_messagerie(self, messagerie: Messagerie, *critères):
         courriels_actuels = self.df
-        nouveaux_courriels = messagerie.df.fillna('')
+        nouveaux_courriels = messagerie.df_filtré(*critères).fillna('')
 
         lim_db = 1000
         nouveaux_courriels.a = nouveaux_courriels.a.map(
             lambda x: x[:lim_db])
         nouveaux_courriels.sujet = nouveaux_courriels.sujet.map(
             lambda x: x[:lim_db])
         nouveaux_courriels.chaine = nouveaux_courriels.chaine.map(
             lambda x: x[:lim_db])
         nouveaux_courriels.contenu = nouveaux_courriels.contenu.map(
             partial(bytes, encoding='utf-8'))
+        nouveaux_courriels.loc[nouveaux_courriels.date
+                               == None, 'date'] = datetime(1970, 1, 1)
 
         tous_courriels = pandas.concat([courriels_actuels,
                                         nouveaux_courriels])
 
         nouveaux_courriels = tous_courriels.drop_duplicates(('date',
                                                              'de',
                                                             'a',
```

### Comparing `polygphys-4.6.9/src/polygphys/outils/reseau/msforms.py` & `polygphys-6.0.5/src/polygphys/outils/reseau/msforms.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 msforms.
 
 Suivre les modifications à des fichiers Excel contenant les résultats de
 formulaires.
 """
 
 # Bibliothèque standard
+import pathlib
 
 from datetime import datetime as dt
 
 # Bibliothèque PIPy
 import pandas as pd
 import sqlalchemy as sqla
 
@@ -176,15 +177,17 @@
 
         Returns
         -------
         None.
 
         """
         cadre = self.nouvelles_entrées()
-        self.config.set('màj', 'dernière', dt.now().isoformat())
+        dernière_modif = dt.fromtimestamp(pathlib.Path(
+            self.fichier).stat().st_mtime).isoformat()
+        self.config.set('màj', 'dernière', dernière_modif)
         self.action(cadre)
 
 
 class MSFormExportBD(MSForm):
 
     def action(self, cadre: pd.DataFrame):
         adresse = self.config.get('bd', 'adresse')
```

### Comparing `polygphys-4.6.9/src/polygphys/outils/reseau/serveur/__init__.py` & `polygphys-6.0.5/src/polygphys/outils/reseau/serveur/__init__.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/serveur/__init__.py` & `polygphys-6.0.5/src/polygphys/serveur/__init__.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/serveur/__main__.py` & `polygphys-6.0.5/src/polygphys/serveur/__main__.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/serveur/nouveau_script.py` & `polygphys-6.0.5/src/polygphys/serveur/nouveau_script.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/sst/certificats_laser/nouveau_certificat.cfg` & `polygphys-6.0.5/src/polygphys/sst/certificats_laser/nouveau_certificat.cfg`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/sst/certificats_laser/nouveau_certificats.py` & `polygphys-6.0.5/src/polygphys/sst/certificats_laser/nouveau_certificats.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/sst/certificats_laser/vérifier.py` & `polygphys-6.0.5/src/polygphys/sst/certificats_laser/vérifier.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/sst/inscriptions_sst/inscription.cfg` & `polygphys-6.0.5/src/polygphys/sst/inscriptions_sst/inscription.cfg`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/sst/inscriptions_sst/inscriptions_sst.py` & `polygphys-6.0.5/src/polygphys/sst/inscriptions_sst/inscriptions_sst.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/sst/trousses_premiers_soins/premiers_soins.cfg` & `polygphys-6.0.5/src/polygphys/sst/trousses_premiers_soins/premiers_soins.cfg`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys/sst/trousses_premiers_soins/premiers_soins.py` & `polygphys-6.0.5/src/polygphys/sst/trousses_premiers_soins/premiers_soins.py`

 * *Files identical despite different names*

### Comparing `polygphys-4.6.9/src/polygphys.egg-info/PKG-INFO` & `polygphys-6.0.5/src/polygphys.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: polygphys
-Version: 4.6.9
+Version: 6.0.5
 Summary: Outils pour des programmes à l'interne du département de physique de Polytechnique Montréal.
 Author: Émile Jetzer
 Author-email: emile.jetzer@polymtl.ca
-Requires-Python: >=3.9
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # Outils & programmes du département de génie physique de Polytechnique [![Python application](https://github.com/ejetzer/polygphys/actions/workflows/python-app.yml/badge.svg)](https://github.com/ejetzer/polygphys/actions/workflows/python-app.yml) [![CodeQL](https://github.com/ejetzer/polygphys/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/ejetzer/polygphys/actions/workflows/codeql-analysis.yml) [![Upload Python Package](https://github.com/ejetzer/polygphys/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ejetzer/polygphys/actions/workflows/python-publish.yml) [![Documentation Status](https://readthedocs.org/projects/polygphys/badge/?version=latest)](https://polygphys.readthedocs.io/en/latest/?badge=latest)
 
 - Installation via PyPI: https://pypi.org/project/polygphys/
     ```
     pip install polygphys
```

### Comparing `polygphys-4.6.9/src/polygphys.egg-info/SOURCES.txt` & `polygphys-6.0.5/src/polygphys.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 pyproject.toml
+readme.md
 setup.cfg
 setup.py
 src/polygphys/__init__.py
 src/polygphys/__main__.py
 src/polygphys.egg-info/PKG-INFO
 src/polygphys.egg-info/SOURCES.txt
 src/polygphys.egg-info/dependency_links.txt
```

