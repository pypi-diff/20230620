# Comparing `tmp/rer.newsletter-2.0.0a1.tar.gz` & `tmp/rer.newsletter-2.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rer.newsletter-2.0.0a1.tar", last modified: Tue Mar 14 08:06:16 2023, max compression
+gzip compressed data, was "rer.newsletter-2.0.0a2.tar", last modified: Thu Mar 16 14:37:27 2023, max compression
```

## Comparing `rer.newsletter-2.0.0a1.tar` & `rer.newsletter-2.0.0a2.tar`

### file list

```diff
@@ -1,214 +1,214 @@
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.732394 rer.newsletter-2.0.0a1/
--rw-r--r--   0 filippocampi   (501) staff       (20)     3781 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/CHANGES.rst
--rw-r--r--   0 filippocampi   (501) staff       (20)       91 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/CONTRIBUTORS.rst
--rw-r--r--   0 filippocampi   (501) staff       (20)    18092 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/LICENSE.GPL
--rw-r--r--   0 filippocampi   (501) staff       (20)      658 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/LICENSE.rst
--rw-r--r--   0 filippocampi   (501) staff       (20)      152 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/MANIFEST.in
--rw-r--r--   0 filippocampi   (501) staff       (20)     9354 2023-03-14 08:06:16.732526 rer.newsletter-2.0.0a1/PKG-INFO
--rw-r--r--   0 filippocampi   (501) staff       (20)     4554 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/README.rst
--rw-r--r--   0 filippocampi   (501) staff       (20)       27 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/constraints.txt
--rw-r--r--   0 filippocampi   (501) staff       (20)      105 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/constraints_plone51.txt
--rw-r--r--   0 filippocampi   (501) staff       (20)      105 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/constraints_plone52.txt
--rw-r--r--   0 filippocampi   (501) staff       (20)      105 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/constraints_plone60.txt
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.688038 rer.newsletter-2.0.0a1/docs/
--rw-r--r--   0 filippocampi   (501) staff       (20)       77 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/docs/index.rst
--rw-r--r--   0 filippocampi   (501) staff       (20)    32560 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/docs/rer-logo.png
--rw-r--r--   0 filippocampi   (501) staff       (20)       50 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/requirements.txt
--rw-r--r--   0 filippocampi   (501) staff       (20)      270 2023-03-14 08:06:16.733141 rer.newsletter-2.0.0a1/setup.cfg
--rw-r--r--   0 filippocampi   (501) staff       (20)     2391 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/setup.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.678592 rer.newsletter-2.0.0a1/src/
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.688352 rer.newsletter-2.0.0a1/src/rer/
--rw-r--r--   0 filippocampi   (501) staff       (20)       80 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/__init__.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.693491 rer.newsletter-2.0.0a1/src/rer/newsletter/
--rw-r--r--   0 filippocampi   (501) staff       (20)      184 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/__init__.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.694500 rer.newsletter-2.0.0a1/src/rer/newsletter/adapter/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/adapter/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      648 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/adapter/configure.zcml
--rw-r--r--   0 filippocampi   (501) staff       (20)     8053 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/adapter/sender.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     8353 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/adapter/subscriptions.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.695282 rer.newsletter-2.0.0a1/src/rer/newsletter/behaviors/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/behaviors/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      441 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/behaviors/configure.zcml
--rw-r--r--   0 filippocampi   (501) staff       (20)      970 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/behaviors/ships.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.696000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/__init__.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.698607 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1686 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/add.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1372 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/channelhistory.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      708 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/channelview.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      383 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/channelviewlet.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     5308 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/configure.zcml
--rw-r--r--   0 filippocampi   (501) staff       (20)     2208 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/deleteexpiredusers.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     3177 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/manageusers.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     5321 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/subscribe.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.700769 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/templates/
--rw-r--r--   0 filippocampi   (501) staff       (20)     1607 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/templates/channelhistoryview.pt
--rw-r--r--   0 filippocampi   (501) staff       (20)     2608 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/templates/channelview.pt
--rw-r--r--   0 filippocampi   (501) staff       (20)      787 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/templates/channelviewlet.pt
--rw-r--r--   0 filippocampi   (501) staff       (20)      885 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/templates/confirm_subscription.pt
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.702753 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/templates/mail_templates/
--rw-r--r--   0 filippocampi   (501) staff       (20)      851 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/templates/mail_templates/active_user.pt
--rw-r--r--   0 filippocampi   (501) staff       (20)      568 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/templates/mail_templates/active_user_confirm.pt
--rw-r--r--   0 filippocampi   (501) staff       (20)      603 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/templates/mail_templates/asynch_send_fail.pt
--rw-r--r--   0 filippocampi   (501) staff       (20)      728 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/templates/mail_templates/asynch_send_success.pt
--rw-r--r--   0 filippocampi   (501) staff       (20)      571 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/templates/mail_templates/delete_user.pt
--rw-r--r--   0 filippocampi   (501) staff       (20)      611 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/templates/mail_templates/delete_user_confirm.pt
--rw-r--r--   0 filippocampi   (501) staff       (20)      592 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/templates/mail_templates/unsubscribe_channel.pt
--rw-r--r--   0 filippocampi   (501) staff       (20)     3072 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/templates/manageusers.pt
--rw-r--r--   0 filippocampi   (501) staff       (20)     1685 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/templates/subscribechannel.pt
--rw-r--r--   0 filippocampi   (501) staff       (20)     1080 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/templates/unsubscribechannel.pt
--rw-r--r--   0 filippocampi   (501) staff       (20)     4430 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/unsubscribe.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.703831 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/users/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/users/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1828 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/users/add.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     3892 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/users/confirm_subscription.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     5980 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/users/usersimport.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      907 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/configure.zcml
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.706920 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/message/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/message/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      525 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/message/checkmessageview.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      442 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/message/collectionview.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     2969 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/message/configure.zcml
--rw-r--r--   0 filippocampi   (501) staff       (20)     2692 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/message/messagepreview.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      174 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/message/messageview.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1543 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/message/messageviewlet.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     5509 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/message/sendingtest.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     3057 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/message/sendmessageview.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      288 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/message/shippablecollection.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.708878 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/message/templates/
--rw-r--r--   0 filippocampi   (501) staff       (20)     2687 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/message/templates/collection_sending_view.pt
--rw-r--r--   0 filippocampi   (501) staff       (20)      870 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/message/templates/messagecontentcore.pt
--rw-r--r--   0 filippocampi   (501) staff       (20)     1532 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/message/templates/messagepreview.pt
--rw-r--r--   0 filippocampi   (501) staff       (20)      952 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/message/templates/messageview.pt
--rw-r--r--   0 filippocampi   (501) staff       (20)     1542 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/message/templates/messageviewlet.pt
--rw-r--r--   0 filippocampi   (501) staff       (20)     1132 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/message/templates/sendingtest.pt
--rw-r--r--   0 filippocampi   (501) staff       (20)     1451 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/message/templates/sendmessageview.pt
--rw-r--r--   0 filippocampi   (501) staff       (20)      570 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/message/versionview.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.709267 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/overrides/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/overrides/.gitkeep
--rw-r--r--   0 filippocampi   (501) staff       (20)     1465 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/settings.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.709958 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/static/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/static/.gitkeep
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.710230 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/static/DataTables-1.10.16/
--rw-r--r--   0 filippocampi   (501) staff       (20)     6148 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/static/DataTables-1.10.16/.DS_Store
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.711767 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/static/DataTables-1.10.16/images/
--rwxr-xr-x   0 filippocampi   (501) staff       (20)      160 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/static/DataTables-1.10.16/images/sort_asc.png
--rwxr-xr-x   0 filippocampi   (501) staff       (20)      148 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/static/DataTables-1.10.16/images/sort_asc_disabled.png
--rwxr-xr-x   0 filippocampi   (501) staff       (20)      201 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/static/DataTables-1.10.16/images/sort_both.png
--rwxr-xr-x   0 filippocampi   (501) staff       (20)      158 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/static/DataTables-1.10.16/images/sort_desc.png
--rwxr-xr-x   0 filippocampi   (501) staff       (20)      146 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/static/DataTables-1.10.16/images/sort_desc_disabled.png
--rw-r--r--   0 filippocampi   (501) staff       (20)     1436 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/static/custom.css
--rw-r--r--   0 filippocampi   (501) staff       (20)    16203 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/static/datatables.css
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.713409 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/static/scripts/
--rw-r--r--   0 filippocampi   (501) staff       (20)     2707 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/static/scripts/channelhistory.js
--rwxr-xr-x   0 filippocampi   (501) staff       (20)   443959 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/static/scripts/datatables.js
--rw-r--r--   0 filippocampi   (501) staff       (20)     4087 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/static/scripts/initializedModal.js
--rw-r--r--   0 filippocampi   (501) staff       (20)     4000 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/browser/static/scripts/manageusers.js
--rw-r--r--   0 filippocampi   (501) staff       (20)     2216 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/configure.zcml
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.714585 rer.newsletter-2.0.0a1/src/rer/newsletter/content/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/content/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      217 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/content/channel.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      217 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/content/message.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      261 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/content/shippable_collection.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.716862 rer.newsletter-2.0.0a1/src/rer/newsletter/contentrules/
--rw-r--r--   0 filippocampi   (501) staff       (20)       24 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/contentrules/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      871 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/contentrules/actions.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     3229 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/contentrules/configure.zcml
--rw-r--r--   0 filippocampi   (501) staff       (20)      955 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/contentrules/events.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     2092 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/contentrules/executors.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1907 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/contentrules/forms.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      216 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/contentrules/handlers.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1376 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/contentrules/interfaces.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.717364 rer.newsletter-2.0.0a1/src/rer/newsletter/exceptions/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/exceptions/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      132 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/exceptions/exceptions.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     3577 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/interfaces.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.718153 rer.newsletter-2.0.0a1/src/rer/newsletter/locales/
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.681513 rer.newsletter-2.0.0a1/src/rer/newsletter/locales/it/
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.718410 rer.newsletter-2.0.0a1/src/rer/newsletter/locales/it/LC_MESSAGES/
--rw-r--r--   0 filippocampi   (501) staff       (20)    17392 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/locales/it/LC_MESSAGES/rer.newsletter.po
--rw-r--r--   0 filippocampi   (501) staff       (20)    14638 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/locales/rer.newsletter.pot
--rw-r--r--   0 filippocampi   (501) staff       (20)     1569 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/locales/update.py
--rwxr-xr-x   0 filippocampi   (501) staff       (20)      503 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/locales/update.sh
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.719951 rer.newsletter-2.0.0a1/src/rer/newsletter/portlets/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/portlets/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      573 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/portlets/configure.zcml
--rw-r--r--   0 filippocampi   (501) staff       (20)     1695 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/portlets/interface.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      873 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/portlets/subscribe.pt
--rw-r--r--   0 filippocampi   (501) staff       (20)     1912 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/portlets/subscribe.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.682574 rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.723552 rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/default/
--rw-r--r--   0 filippocampi   (501) staff       (20)      178 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/default/actions.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      161 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/default/browserlayer.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      275 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/default/catalog.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      570 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/default/controlpanel.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      373 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/default/diff_tool.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      184 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/default/metadata.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      280 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/default/portlets.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)     3209 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/default/registry.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      365 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/default/repositorytool.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)     1350 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/default/rolemap.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      252 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/default/sharing.xml
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.724333 rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/default/types/
--rw-r--r--   0 filippocampi   (501) staff       (20)     2961 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/default/types/Channel.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)     3036 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/default/types/Message.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)     3345 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/default/types/Shippable_Collection.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      327 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/default/types.xml
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.682434 rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/default/workflows/
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.724595 rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/default/workflows/channel_workflow/
--rw-r--r--   0 filippocampi   (501) staff       (20)     8132 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/default/workflows/channel_workflow/definition.xml
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.724859 rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/default/workflows/message_workflow/
--rw-r--r--   0 filippocampi   (501) staff       (20)     9923 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/default/workflows/message_workflow/definition.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      643 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/default/workflows.xml
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.726163 rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/uninstall/
--rw-r--r--   0 filippocampi   (501) staff       (20)      824 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/uninstall/actions.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      117 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      321 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/uninstall/controlpanel.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      701 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/uninstall/registry.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      296 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/uninstall/types.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)       30 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/pyproject.toml
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.727504 rer.newsletter-2.0.0a1/src/rer/newsletter/queue/
--rw-r--r--   0 filippocampi   (501) staff       (20)       24 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/queue/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      487 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/queue/configure.zcml
--rw-r--r--   0 filippocampi   (501) staff       (20)      643 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/queue/handler.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      360 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/queue/interfaces.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     5050 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/queue/view.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.728008 rer.newsletter-2.0.0a1/src/rer/newsletter/restapi/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/restapi/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      240 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/restapi/configure.zcml
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.729338 rer.newsletter-2.0.0a1/src/rer/newsletter/restapi/services/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/restapi/services/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      784 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/restapi/services/configure.zcml
--rw-r--r--   0 filippocampi   (501) staff       (20)     3875 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/restapi/services/confirm_subscription.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     3821 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/restapi/services/subscribe.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     3497 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/restapi/services/unsubscribe.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1220 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/setuphandlers.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1174 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/testing.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.730317 rer.newsletter-2.0.0a1/src/rer/newsletter/tests/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/tests/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     3009 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/tests/test_setup.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     2102 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/tests/test_subscription_tile.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     9313 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/tests/test_subscriptions_adapter.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.731391 rer.newsletter-2.0.0a1/src/rer/newsletter/tiles/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/tiles/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      635 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/tiles/configure.zcml
--rw-r--r--   0 filippocampi   (501) staff       (20)     1250 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/tiles/subscribe.pt
--rw-r--r--   0 filippocampi   (501) staff       (20)     1104 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/tiles/subscribe.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.732180 rer.newsletter-2.0.0a1/src/rer/newsletter/transforms/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/transforms/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     2037 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/transforms/link_transform.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      206 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/transforms/mimetype.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     3154 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/upgrades.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1101 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/upgrades.zcml
--rw-r--r--   0 filippocampi   (501) staff       (20)     1309 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/utils.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      864 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer/newsletter/vocabularies.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-03-14 08:06:16.690748 rer.newsletter-2.0.0a1/src/rer.newsletter.egg-info/
--rw-r--r--   0 filippocampi   (501) staff       (20)     9354 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer.newsletter.egg-info/PKG-INFO
--rw-r--r--   0 filippocampi   (501) staff       (20)     8170 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer.newsletter.egg-info/SOURCES.txt
--rw-r--r--   0 filippocampi   (501) staff       (20)        1 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer.newsletter.egg-info/dependency_links.txt
--rw-r--r--   0 filippocampi   (501) staff       (20)      119 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer.newsletter.egg-info/entry_points.txt
--rw-r--r--   0 filippocampi   (501) staff       (20)        4 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer.newsletter.egg-info/namespace_packages.txt
--rw-r--r--   0 filippocampi   (501) staff       (20)        1 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer.newsletter.egg-info/not-zip-safe
--rw-r--r--   0 filippocampi   (501) staff       (20)      292 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer.newsletter.egg-info/requires.txt
--rw-r--r--   0 filippocampi   (501) staff       (20)        4 2023-03-14 08:06:16.000000 rer.newsletter-2.0.0a1/src/rer.newsletter.egg-info/top_level.txt
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.055803 rer.newsletter-2.0.0a2/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     3868 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/CHANGES.rst
+-rw-r--r--   0 pieronicolli   (501) staff       (20)       91 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/CONTRIBUTORS.rst
+-rw-r--r--   0 pieronicolli   (501) staff       (20)    18092 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/LICENSE.GPL
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      658 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/LICENSE.rst
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      152 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/MANIFEST.in
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     9441 2023-03-16 14:37:27.055889 rer.newsletter-2.0.0a2/PKG-INFO
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     4554 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/README.rst
+-rw-r--r--   0 pieronicolli   (501) staff       (20)       27 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/constraints.txt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      105 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/constraints_plone51.txt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      105 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/constraints_plone52.txt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      105 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/constraints_plone60.txt
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.036795 rer.newsletter-2.0.0a2/docs/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)       77 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/docs/index.rst
+-rw-r--r--   0 pieronicolli   (501) staff       (20)    32560 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/docs/rer-logo.png
+-rw-r--r--   0 pieronicolli   (501) staff       (20)       50 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/requirements.txt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      270 2023-03-16 14:37:27.056218 rer.newsletter-2.0.0a2/setup.cfg
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     2391 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/setup.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.032965 rer.newsletter-2.0.0a2/src/
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.036920 rer.newsletter-2.0.0a2/src/rer/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)       80 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/__init__.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.038915 rer.newsletter-2.0.0a2/src/rer/newsletter/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      184 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/__init__.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.039333 rer.newsletter-2.0.0a2/src/rer/newsletter/adapter/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/adapter/__init__.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      648 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/adapter/configure.zcml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     7952 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/adapter/sender.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     8353 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/adapter/subscriptions.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.039648 rer.newsletter-2.0.0a2/src/rer/newsletter/behaviors/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/behaviors/__init__.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      441 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/behaviors/configure.zcml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      970 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/behaviors/ships.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.039988 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/__init__.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.042314 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/__init__.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1686 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/add.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1372 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/channelhistory.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      708 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/channelview.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      383 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/channelviewlet.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     5308 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/configure.zcml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     2208 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/deleteexpiredusers.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     3177 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/manageusers.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     5321 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/subscribe.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.043096 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1607 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/channelhistoryview.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     2608 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/channelview.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      787 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/channelviewlet.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      885 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/confirm_subscription.pt
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.043864 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/mail_templates/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      851 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/mail_templates/active_user.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      568 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/mail_templates/active_user_confirm.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      603 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/mail_templates/asynch_send_fail.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      728 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/mail_templates/asynch_send_success.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      571 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/mail_templates/delete_user.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      611 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/mail_templates/delete_user_confirm.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      592 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/mail_templates/unsubscribe_channel.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     3072 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/manageusers.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1685 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/subscribechannel.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1080 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/unsubscribechannel.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     4430 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/unsubscribe.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.044268 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/users/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/users/__init__.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1828 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/users/add.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     3892 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/users/confirm_subscription.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     5980 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/users/usersimport.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      907 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/configure.zcml
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.045413 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/__init__.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      525 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/checkmessageview.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      442 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/collectionview.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     2969 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/configure.zcml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     2603 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/messagepreview.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      174 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/messageview.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1543 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/messageviewlet.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     5408 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/sendingtest.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     3057 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/sendmessageview.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      288 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/shippablecollection.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.046144 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/templates/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     2687 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/templates/collection_sending_view.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      870 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/templates/messagecontentcore.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1532 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/templates/messagepreview.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      952 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/templates/messageview.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1542 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/templates/messageviewlet.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1132 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/templates/sendingtest.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1451 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/templates/sendmessageview.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      570 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/versionview.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.046254 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/overrides/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/overrides/.gitkeep
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1465 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/settings.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.046527 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/.gitkeep
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.046631 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/DataTables-1.10.16/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     6148 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/DataTables-1.10.16/.DS_Store
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.047165 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/DataTables-1.10.16/images/
+-rwxr-xr-x   0 pieronicolli   (501) staff       (20)      160 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/DataTables-1.10.16/images/sort_asc.png
+-rwxr-xr-x   0 pieronicolli   (501) staff       (20)      148 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/DataTables-1.10.16/images/sort_asc_disabled.png
+-rwxr-xr-x   0 pieronicolli   (501) staff       (20)      201 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/DataTables-1.10.16/images/sort_both.png
+-rwxr-xr-x   0 pieronicolli   (501) staff       (20)      158 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/DataTables-1.10.16/images/sort_desc.png
+-rwxr-xr-x   0 pieronicolli   (501) staff       (20)      146 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/DataTables-1.10.16/images/sort_desc_disabled.png
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1436 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/custom.css
+-rw-r--r--   0 pieronicolli   (501) staff       (20)    16203 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/datatables.css
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.047888 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/scripts/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     2707 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/scripts/channelhistory.js
+-rwxr-xr-x   0 pieronicolli   (501) staff       (20)   443959 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/scripts/datatables.js
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     4087 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/scripts/initializedModal.js
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     4000 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/scripts/manageusers.js
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     2216 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/configure.zcml
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.048304 rer.newsletter-2.0.0a2/src/rer/newsletter/content/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/content/__init__.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      217 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/content/channel.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      217 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/content/message.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      261 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/content/shippable_collection.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.049165 rer.newsletter-2.0.0a2/src/rer/newsletter/contentrules/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)       24 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/contentrules/__init__.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      871 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/contentrules/actions.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     3229 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/contentrules/configure.zcml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      955 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/contentrules/events.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     2092 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/contentrules/executors.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1907 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/contentrules/forms.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      216 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/contentrules/handlers.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1376 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/contentrules/interfaces.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.049358 rer.newsletter-2.0.0a2/src/rer/newsletter/exceptions/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/exceptions/__init__.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      132 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/exceptions/exceptions.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     3577 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/interfaces.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.049673 rer.newsletter-2.0.0a2/src/rer/newsletter/locales/
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.034283 rer.newsletter-2.0.0a2/src/rer/newsletter/locales/it/
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.049776 rer.newsletter-2.0.0a2/src/rer/newsletter/locales/it/LC_MESSAGES/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)    17392 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/locales/it/LC_MESSAGES/rer.newsletter.po
+-rw-r--r--   0 pieronicolli   (501) staff       (20)    14638 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/locales/rer.newsletter.pot
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1569 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/locales/update.py
+-rwxr-xr-x   0 pieronicolli   (501) staff       (20)      503 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/locales/update.sh
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.050334 rer.newsletter-2.0.0a2/src/rer/newsletter/portlets/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/portlets/__init__.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      573 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/portlets/configure.zcml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1695 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/portlets/interface.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      873 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/portlets/subscribe.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1912 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/portlets/subscribe.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.034749 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.051990 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      178 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/actions.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      161 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/browserlayer.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      275 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/catalog.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      570 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/controlpanel.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      373 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/diff_tool.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      184 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/metadata.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      280 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/portlets.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     3209 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/registry.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      365 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/repositorytool.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1350 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/rolemap.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      252 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/sharing.xml
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.052318 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/types/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     2961 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/types/Channel.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     3036 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/types/Message.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     3345 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/types/Shippable_Collection.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      327 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/types.xml
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.034688 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/workflows/
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.052427 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/workflows/channel_workflow/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     8132 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/workflows/channel_workflow/definition.xml
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.052537 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/workflows/message_workflow/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     9923 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/workflows/message_workflow/definition.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      643 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/workflows.xml
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.053074 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/uninstall/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      824 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/uninstall/actions.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      117 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      321 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/uninstall/controlpanel.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      701 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/uninstall/registry.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      296 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/uninstall/types.xml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)       30 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/pyproject.toml
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.053603 rer.newsletter-2.0.0a2/src/rer/newsletter/queue/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)       24 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/queue/__init__.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      487 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/queue/configure.zcml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      643 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/queue/handler.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      360 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/queue/interfaces.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     5050 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/queue/view.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.053811 rer.newsletter-2.0.0a2/src/rer/newsletter/restapi/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/restapi/__init__.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      240 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/restapi/configure.zcml
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.054377 rer.newsletter-2.0.0a2/src/rer/newsletter/restapi/services/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/restapi/services/__init__.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      784 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/restapi/services/configure.zcml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     3875 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/restapi/services/confirm_subscription.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     3821 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/restapi/services/subscribe.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     3497 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/restapi/services/unsubscribe.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1220 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/setuphandlers.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1174 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/testing.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.054850 rer.newsletter-2.0.0a2/src/rer/newsletter/tests/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/tests/__init__.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     3009 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/tests/test_setup.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     2102 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/tests/test_subscription_tile.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     9313 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/tests/test_subscriptions_adapter.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.055362 rer.newsletter-2.0.0a2/src/rer/newsletter/tiles/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/tiles/__init__.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      635 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/tiles/configure.zcml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1250 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/tiles/subscribe.pt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1104 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/tiles/subscribe.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.055696 rer.newsletter-2.0.0a2/src/rer/newsletter/transforms/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/transforms/__init__.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     2037 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/transforms/link_transform.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      206 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/transforms/mimetype.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     3154 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/upgrades.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1101 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/upgrades.zcml
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     1309 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/utils.py
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      864 2023-03-16 14:37:25.000000 rer.newsletter-2.0.0a2/src/rer/newsletter/vocabularies.py
+drwxr-xr-x   0 pieronicolli   (501) staff       (20)        0 2023-03-16 14:37:27.037826 rer.newsletter-2.0.0a2/src/rer.newsletter.egg-info/
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     9441 2023-03-16 14:37:26.000000 rer.newsletter-2.0.0a2/src/rer.newsletter.egg-info/PKG-INFO
+-rw-r--r--   0 pieronicolli   (501) staff       (20)     8170 2023-03-16 14:37:26.000000 rer.newsletter-2.0.0a2/src/rer.newsletter.egg-info/SOURCES.txt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        1 2023-03-16 14:37:26.000000 rer.newsletter-2.0.0a2/src/rer.newsletter.egg-info/dependency_links.txt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      119 2023-03-16 14:37:26.000000 rer.newsletter-2.0.0a2/src/rer.newsletter.egg-info/entry_points.txt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        4 2023-03-16 14:37:26.000000 rer.newsletter-2.0.0a2/src/rer.newsletter.egg-info/namespace_packages.txt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        1 2023-03-16 14:37:26.000000 rer.newsletter-2.0.0a2/src/rer.newsletter.egg-info/not-zip-safe
+-rw-r--r--   0 pieronicolli   (501) staff       (20)      292 2023-03-16 14:37:26.000000 rer.newsletter-2.0.0a2/src/rer.newsletter.egg-info/requires.txt
+-rw-r--r--   0 pieronicolli   (501) staff       (20)        4 2023-03-16 14:37:26.000000 rer.newsletter-2.0.0a2/src/rer.newsletter.egg-info/top_level.txt
```

### Comparing `rer.newsletter-2.0.0a1/CHANGES.rst` & `rer.newsletter-2.0.0a2/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 =========
 Changelog
 =========
 
+2.0.0a2 (2023-03-16)
+--------------------
+
+- Updated subheader template
+  [pnicolli]
+
+
 2.0.0a1 (2023-03-14)
 --------------------
 
 - added restapi services for Volto usage
 - fixed results for unsubscribe service
 - italian translation
 - remove CSRFProtection when call services
```

### Comparing `rer.newsletter-2.0.0a1/LICENSE.GPL` & `rer.newsletter-2.0.0a2/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/LICENSE.rst` & `rer.newsletter-2.0.0a2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/PKG-INFO` & `rer.newsletter-2.0.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rer.newsletter
-Version: 2.0.0a1
+Version: 2.0.0a2
 Summary: An add-on for Plone
 Home-page: https://pypi.python.org/pypi/rer.newsletter
 Author: Filippo Campi
 Author-email: filippo.campi@redturtle.it
 License: GPL version 2
 Keywords: Python Plone
 Classifier: Development Status :: 5 - Production/Stable
@@ -204,14 +204,21 @@
 - RedTurtle Technology, sviluppoplone@redturtle.it
 
 
 =========
 Changelog
 =========
 
+2.0.0a2 (2023-03-16)
+--------------------
+
+- Updated subheader template
+  [pnicolli]
+
+
 2.0.0a1 (2023-03-14)
 --------------------
 
 - added restapi services for Volto usage
 - fixed results for unsubscribe service
 - italian translation
 - remove CSRFProtection when call services
```

### Comparing `rer.newsletter-2.0.0a1/README.rst` & `rer.newsletter-2.0.0a2/README.rst`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/docs/rer-logo.png` & `rer.newsletter-2.0.0a2/docs/rer-logo.png`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/setup.py` & `rer.newsletter-2.0.0a2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="rer.newsletter",
-    version="2.0.0a1",
+    version="2.0.0a2",
     description="An add-on for Plone",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/adapter/configure.zcml` & `rer.newsletter-2.0.0a2/src/rer/newsletter/adapter/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/adapter/sender.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/adapter/sender.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,17 +80,14 @@
         parameters = {
             "css": self.context.css_style,
             "message_header": self.context.header
             if self.context.header
             else "",
             "message_subheader": f"""
                 <tr>
-                    <td class="divider" colspan="2"></td>
-                </tr>
-                <tr>
                     <td align="left" colspan="2">
                       <div class="newsletterTitle">
                         <h1>{self.context.title}</h1>
                       </div>
                     </td>
                 </tr>""",
             "message_footer": self.context.footer
```

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/adapter/subscriptions.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/adapter/subscriptions.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/behaviors/ships.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/behaviors/ships.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/add.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/add.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/channelhistory.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/channelhistory.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/channelview.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/channelview.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/configure.zcml` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/deleteexpiredusers.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/deleteexpiredusers.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/manageusers.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/manageusers.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/subscribe.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/subscribe.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/templates/channelhistoryview.pt` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/channelhistoryview.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/templates/channelview.pt` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/channelview.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/templates/channelviewlet.pt` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/channelviewlet.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/templates/confirm_subscription.pt` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/confirm_subscription.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/templates/mail_templates/active_user.pt` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/mail_templates/active_user.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/templates/mail_templates/active_user_confirm.pt` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/mail_templates/active_user_confirm.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/templates/mail_templates/asynch_send_fail.pt` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/mail_templates/asynch_send_fail.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/templates/mail_templates/asynch_send_success.pt` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/mail_templates/asynch_send_success.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/templates/mail_templates/delete_user.pt` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/mail_templates/delete_user.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/templates/mail_templates/delete_user_confirm.pt` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/mail_templates/delete_user_confirm.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/templates/mail_templates/unsubscribe_channel.pt` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/mail_templates/unsubscribe_channel.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/templates/manageusers.pt` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/manageusers.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/templates/subscribechannel.pt` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/subscribechannel.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/templates/unsubscribechannel.pt` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/templates/unsubscribechannel.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/unsubscribe.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/unsubscribe.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/users/add.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/users/add.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/users/confirm_subscription.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/users/confirm_subscription.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/channel/users/usersimport.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/channel/users/usersimport.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/configure.zcml` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/message/checkmessageview.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/checkmessageview.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/message/configure.zcml` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/message/messagepreview.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/messagepreview.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,17 +26,14 @@
 
     def getMessageFooter(self):
         return self.getChannel().footer if self.getChannel().footer else ""
 
     def getMessageSubHeader(self):
         return f"""
             <tr>
-                <td class="divider" colspan="2"></td>
-            </tr>
-            <tr>
                 <td align="left" colspan="2">
                   <div class="newsletterTitle">
                     <h1>{self.context.title}</h1>
                   </div>
                 </td>
             </tr>
         """
```

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/message/messageviewlet.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/messageviewlet.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/message/sendingtest.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/sendingtest.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,17 +52,14 @@
             "@@messagepreview_view"
         )
         parameters = {
             "css": channel.css_style,
             "message_header": channel.header if channel.header else "",
             "message_subheader": f"""
                 <tr>
-                    <td class="divider" colspan="2"></td>
-                </tr>
-                <tr>
                     <td align="left" colspan="2">
                       <div class="newsletterTitle">
                         <h1>{self.context.title}</h1>
                       </div>
                     </td>
                 </tr>""",
             "message_footer": channel.footer if channel.footer else "",
```

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/message/sendmessageview.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/sendmessageview.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/message/templates/collection_sending_view.pt` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/templates/collection_sending_view.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/message/templates/messagecontentcore.pt` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/templates/messagecontentcore.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/message/templates/messagepreview.pt` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/templates/messagepreview.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/message/templates/messageview.pt` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/templates/messageview.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/message/templates/messageviewlet.pt` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/templates/messageviewlet.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/message/templates/sendingtest.pt` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/templates/sendingtest.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/message/templates/sendmessageview.pt` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/templates/sendmessageview.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/message/versionview.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/message/versionview.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/settings.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/settings.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/static/DataTables-1.10.16/.DS_Store` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/DataTables-1.10.16/.DS_Store`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/static/custom.css` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/custom.css`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/static/datatables.css` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/datatables.css`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/static/scripts/channelhistory.js` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/scripts/channelhistory.js`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/static/scripts/datatables.js` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/scripts/datatables.js`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/static/scripts/initializedModal.js` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/scripts/initializedModal.js`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/browser/static/scripts/manageusers.js` & `rer.newsletter-2.0.0a2/src/rer/newsletter/browser/static/scripts/manageusers.js`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/configure.zcml` & `rer.newsletter-2.0.0a2/src/rer/newsletter/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/contentrules/actions.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/contentrules/actions.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/contentrules/configure.zcml` & `rer.newsletter-2.0.0a2/src/rer/newsletter/contentrules/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/contentrules/events.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/contentrules/events.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/contentrules/executors.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/contentrules/executors.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/contentrules/forms.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/contentrules/forms.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/contentrules/interfaces.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/contentrules/interfaces.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/interfaces.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/interfaces.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/locales/it/LC_MESSAGES/rer.newsletter.po` & `rer.newsletter-2.0.0a2/src/rer/newsletter/locales/it/LC_MESSAGES/rer.newsletter.po`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/locales/rer.newsletter.pot` & `rer.newsletter-2.0.0a2/src/rer/newsletter/locales/rer.newsletter.pot`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/locales/update.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/locales/update.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/portlets/configure.zcml` & `rer.newsletter-2.0.0a2/src/rer/newsletter/portlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/portlets/interface.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/portlets/interface.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/portlets/subscribe.pt` & `rer.newsletter-2.0.0a2/src/rer/newsletter/portlets/subscribe.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/portlets/subscribe.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/portlets/subscribe.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/default/controlpanel.xml` & `rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/default/registry.xml` & `rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/default/rolemap.xml` & `rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/default/types/Channel.xml` & `rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/types/Channel.xml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/default/types/Message.xml` & `rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/types/Message.xml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/default/types/Shippable_Collection.xml` & `rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/types/Shippable_Collection.xml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/default/workflows/channel_workflow/definition.xml` & `rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/workflows/channel_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/default/workflows/message_workflow/definition.xml` & `rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/workflows/message_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/default/workflows.xml` & `rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/default/workflows.xml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/uninstall/actions.xml` & `rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/uninstall/actions.xml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/profiles/uninstall/registry.xml` & `rer.newsletter-2.0.0a2/src/rer/newsletter/profiles/uninstall/registry.xml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/queue/handler.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/queue/handler.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/queue/view.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/queue/view.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/restapi/services/configure.zcml` & `rer.newsletter-2.0.0a2/src/rer/newsletter/restapi/services/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/restapi/services/confirm_subscription.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/restapi/services/confirm_subscription.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/restapi/services/subscribe.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/restapi/services/subscribe.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/restapi/services/unsubscribe.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/restapi/services/unsubscribe.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/setuphandlers.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/testing.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/testing.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/tests/test_setup.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/tests/test_subscription_tile.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/tests/test_subscription_tile.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/tests/test_subscriptions_adapter.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/tests/test_subscriptions_adapter.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/tiles/configure.zcml` & `rer.newsletter-2.0.0a2/src/rer/newsletter/tiles/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/tiles/subscribe.pt` & `rer.newsletter-2.0.0a2/src/rer/newsletter/tiles/subscribe.pt`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/tiles/subscribe.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/tiles/subscribe.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/transforms/link_transform.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/transforms/link_transform.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/upgrades.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/upgrades.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/upgrades.zcml` & `rer.newsletter-2.0.0a2/src/rer/newsletter/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/utils.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/utils.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer/newsletter/vocabularies.py` & `rer.newsletter-2.0.0a2/src/rer/newsletter/vocabularies.py`

 * *Files identical despite different names*

### Comparing `rer.newsletter-2.0.0a1/src/rer.newsletter.egg-info/PKG-INFO` & `rer.newsletter-2.0.0a2/src/rer.newsletter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rer.newsletter
-Version: 2.0.0a1
+Version: 2.0.0a2
 Summary: An add-on for Plone
 Home-page: https://pypi.python.org/pypi/rer.newsletter
 Author: Filippo Campi
 Author-email: filippo.campi@redturtle.it
 License: GPL version 2
 Keywords: Python Plone
 Classifier: Development Status :: 5 - Production/Stable
@@ -204,14 +204,21 @@
 - RedTurtle Technology, sviluppoplone@redturtle.it
 
 
 =========
 Changelog
 =========
 
+2.0.0a2 (2023-03-16)
+--------------------
+
+- Updated subheader template
+  [pnicolli]
+
+
 2.0.0a1 (2023-03-14)
 --------------------
 
 - added restapi services for Volto usage
 - fixed results for unsubscribe service
 - italian translation
 - remove CSRFProtection when call services
```

### Comparing `rer.newsletter-2.0.0a1/src/rer.newsletter.egg-info/SOURCES.txt` & `rer.newsletter-2.0.0a2/src/rer.newsletter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

