# Comparing `tmp/customtkinterx-0.4.0.tar.gz` & `tmp/customtkinterx-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customtkinterx-0.4.0.tar", max compression
+gzip compressed data, was "customtkinterx-0.4.1.tar", max compression
```

## Comparing `customtkinterx-0.4.0.tar` & `customtkinterx-0.4.1.tar`

### file list

```diff
@@ -1,49 +1,53 @@
--rw-r--r--   0        0        0      242 2023-06-02 14:05:53.035149 customtkinterx-0.4.0/customtkinterx/__base64.py
--rw-r--r--   0        0        0     1036 2023-06-10 00:29:27.871591 customtkinterx-0.4.0/customtkinterx/__init__.py
--rw-r--r--   0        0        0      812 2023-06-04 13:04:43.345604 customtkinterx-0.4.0/customtkinterx/__main__.py
--rw-r--r--   0        0        0     9391 2023-06-19 11:02:43.512474 customtkinterx-0.4.0/customtkinterx/CTkCustom.py
--rw-r--r--   0        0        0     6312 2023-06-03 22:39:55.190954 customtkinterx-0.4.0/customtkinterx/CTkFluentTheme.py
--rw-r--r--   0        0        0     6344 2023-06-04 13:04:43.403550 customtkinterx-0.4.0/customtkinterx/CTkGhostSharkTheme.py
--rw-r--r--   0        0        0     8443 2023-06-19 03:31:06.626442 customtkinterx-0.4.0/customtkinterx/CTkInfoBar.py
--rw-r--r--   0        0        0     1244 2023-06-02 11:00:54.754723 customtkinterx-0.4.0/customtkinterx/CTkListBox.py
--rw-r--r--   0        0        0     2596 2023-06-19 00:35:02.877216 customtkinterx-0.4.0/customtkinterx/CTkMegaMenuBar.py
--rw-r--r--   0        0        0      269 2023-05-29 10:31:31.000000 customtkinterx-0.4.0/customtkinterx/CTkMenuBar/__init__.py
--rw-r--r--   0        0        0      522 2023-06-03 04:06:01.937274 customtkinterx-0.4.0/customtkinterx/CTkMenuBar/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    16174 2023-06-03 04:13:46.399109 customtkinterx-0.4.0/customtkinterx/CTkMenuBar/__pycache__/dropdown_menu.cpython-311.pyc
--rw-r--r--   0        0        0     5239 2023-06-03 04:13:46.393587 customtkinterx-0.4.0/customtkinterx/CTkMenuBar/__pycache__/menu_bar.cpython-311.pyc
--rw-r--r--   0        0        0     9724 2023-06-03 04:13:46.396108 customtkinterx-0.4.0/customtkinterx/CTkMenuBar/__pycache__/title_menu_win.cpython-311.pyc
--rw-r--r--   0        0        0     9636 2023-06-03 04:10:48.431998 customtkinterx-0.4.0/customtkinterx/CTkMenuBar/dropdown_menu.py
--rw-r--r--   0        0        0     3300 2023-06-03 04:10:48.421486 customtkinterx-0.4.0/customtkinterx/CTkMenuBar/menu_bar.py
--rw-r--r--   0        0        0     5858 2023-06-03 04:10:48.439015 customtkinterx-0.4.0/customtkinterx/CTkMenuBar/title_menu_win.py
--rw-r--r--   0        0        0     6285 2023-06-03 22:42:43.931473 customtkinterx-0.4.0/customtkinterx/CTkMinimalTheme.py
--rw-r--r--   0        0        0     6337 2023-06-04 02:14:05.106099 customtkinterx-0.4.0/customtkinterx/CTkOffice2019Theme.py
--rw-r--r--   0        0        0      241 2023-05-31 01:43:30.000000 customtkinterx-0.4.0/customtkinterx/CTkPDFViewer/__init__.py
--rw-r--r--   0        0        0      445 2023-06-03 04:13:46.400109 customtkinterx-0.4.0/customtkinterx/CTkPDFViewer/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     6312 2023-06-03 05:49:55.800794 customtkinterx-0.4.0/customtkinterx/CTkPDFViewer/__pycache__/ctk_pdf_viewer.cpython-311.pyc
--rw-r--r--   0        0        0     3543 2023-06-03 05:14:11.938896 customtkinterx-0.4.0/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py
--rw-r--r--   0        0        0      227 2023-05-31 01:40:22.000000 customtkinterx-0.4.0/customtkinterx/CTkTable/__init__.py
--rw-r--r--   0        0        0      427 2023-06-03 04:41:34.919572 customtkinterx-0.4.0/customtkinterx/CTkTable/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    11621 2023-06-03 04:41:34.922572 customtkinterx-0.4.0/customtkinterx/CTkTable/__pycache__/ctktable.cpython-311.pyc
--rw-r--r--   0        0        0     8158 2023-06-03 04:41:34.520984 customtkinterx-0.4.0/customtkinterx/CTkTable/ctktable.py
--rw-r--r--   0        0        0      225 2023-05-08 22:30:16.000000 customtkinterx-0.4.0/customtkinterx/CTkToolTip/__init__.py
--rw-r--r--   0        0        0      426 2023-06-03 04:22:17.427710 customtkinterx-0.4.0/customtkinterx/CTkToolTip/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    10684 2023-06-03 04:26:02.400121 customtkinterx-0.4.0/customtkinterx/CTkToolTip/__pycache__/ctk_tooltip.cpython-311.pyc
--rw-r--r--   0        0        0     6942 2023-06-03 04:22:52.495987 customtkinterx-0.4.0/customtkinterx/CTkToolTip/ctk_tooltip.py
--rw-r--r--   0        0        0     6122 2023-06-19 11:03:32.207624 customtkinterx-0.4.0/customtkinterx/Fluent.json
--rw-r--r--   0        0        0      113 2023-06-09 23:34:51.644065 customtkinterx-0.4.0/customtkinterx/fluent_android/__init__.py
--rw-r--r--   0        0        0      305 2023-06-09 23:34:52.417977 customtkinterx-0.4.0/customtkinterx/fluent_android/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     7135 2023-06-09 23:42:37.438327 customtkinterx-0.4.0/customtkinterx/fluent_android/__pycache__/CTkFluentAndroidTheme.cpython-311.pyc
--rw-r--r--   0        0        0     6375 2023-06-09 23:42:02.599385 customtkinterx-0.4.0/customtkinterx/fluent_android/CTkFluentAndroidTheme.py
--rw-r--r--   0        0        0     1779 2023-06-19 00:59:49.124414 customtkinterx-0.4.0/customtkinterx/fluent_android/CTkFluentAppBar.py
--rw-r--r--   0        0        0     5680 2023-06-10 00:28:44.744869 customtkinterx-0.4.0/customtkinterx/fluent_android/FluentAndroid.json
--rw-r--r--   0        0        0     5437 2023-06-04 13:11:47.958728 customtkinterx-0.4.0/customtkinterx/GhostShark.json
--rw-r--r--   0        0        0    10024 2023-06-19 11:03:46.583974 customtkinterx-0.4.0/customtkinterx/LaunchMusix.py
--rw-r--r--   0        0        0     6141 2023-06-19 11:02:43.512474 customtkinterx-0.4.0/customtkinterx/Minimal.json
--rw-r--r--   0        0        0     1377 2023-06-04 11:35:40.844283 customtkinterx-0.4.0/customtkinterx/Musix-Dark.png
--rw-r--r--   0        0        0     1039 2023-06-04 11:33:35.093179 customtkinterx-0.4.0/customtkinterx/Musix.png
--rw-r--r--   0        0        0     5683 2023-06-03 23:01:51.610936 customtkinterx-0.4.0/customtkinterx/Office2019.json
--rw-r--r--   0        0        0    84836 2022-04-30 00:01:08.000000 customtkinterx-0.4.0/customtkinterx/PublicSans-Regular.ttf
--rw-r--r--   0        0        0    10586 2023-06-19 01:41:00.500221 customtkinterx-0.4.0/customtkinterx/test.py
--rw-r--r--   0        0        0      368 2023-06-19 11:04:04.640070 customtkinterx-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3686 2023-06-03 06:54:12.682589 customtkinterx-0.4.0/README.md
--rw-r--r--   0        0        0     4165 1970-01-01 00:00:00.000000 customtkinterx-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      242 2023-06-02 14:05:53.035149 customtkinterx-0.4.1/customtkinterx/__base64.py
+-rw-r--r--   0        0        0     1235 2023-06-20 11:05:15.151378 customtkinterx-0.4.1/customtkinterx/__init__.py
+-rw-r--r--   0        0        0      812 2023-06-04 13:04:43.345604 customtkinterx-0.4.1/customtkinterx/__main__.py
+-rw-r--r--   0        0        0     9482 2023-06-19 11:06:59.400919 customtkinterx-0.4.1/customtkinterx/CTkCustom.py
+-rw-r--r--   0        0        0     6744 2023-06-19 11:05:29.722427 customtkinterx-0.4.1/customtkinterx/CTkFluentTheme.py
+-rw-r--r--   0        0        0     6344 2023-06-04 13:04:43.403550 customtkinterx-0.4.1/customtkinterx/CTkGhostSharkTheme.py
+-rw-r--r--   0        0        0     8803 2023-06-20 12:13:02.421335 customtkinterx-0.4.1/customtkinterx/CTkInfoBar.py
+-rw-r--r--   0        0        0     4566 2023-06-20 09:30:34.136863 customtkinterx-0.4.1/customtkinterx/CTkKanban.py
+-rw-r--r--   0        0        0     1279 2023-06-20 10:15:40.135212 customtkinterx-0.4.1/customtkinterx/CTkListBox.py
+-rw-r--r--   0        0        0     7667 2023-06-20 11:05:15.033164 customtkinterx-0.4.1/customtkinterx/CTkMaterialTheme.py
+-rw-r--r--   0        0        0     2596 2023-06-19 00:35:02.877216 customtkinterx-0.4.1/customtkinterx/CTkMegaMenuBar.py
+-rw-r--r--   0        0        0      269 2023-05-29 10:31:31.000000 customtkinterx-0.4.1/customtkinterx/CTkMenuBar/__init__.py
+-rw-r--r--   0        0        0      522 2023-06-03 04:06:01.937274 customtkinterx-0.4.1/customtkinterx/CTkMenuBar/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    16174 2023-06-03 04:13:46.399109 customtkinterx-0.4.1/customtkinterx/CTkMenuBar/__pycache__/dropdown_menu.cpython-311.pyc
+-rw-r--r--   0        0        0     5239 2023-06-03 04:13:46.393587 customtkinterx-0.4.1/customtkinterx/CTkMenuBar/__pycache__/menu_bar.cpython-311.pyc
+-rw-r--r--   0        0        0     9724 2023-06-03 04:13:46.396108 customtkinterx-0.4.1/customtkinterx/CTkMenuBar/__pycache__/title_menu_win.cpython-311.pyc
+-rw-r--r--   0        0        0     9636 2023-06-03 04:10:48.431998 customtkinterx-0.4.1/customtkinterx/CTkMenuBar/dropdown_menu.py
+-rw-r--r--   0        0        0     3300 2023-06-03 04:10:48.421486 customtkinterx-0.4.1/customtkinterx/CTkMenuBar/menu_bar.py
+-rw-r--r--   0        0        0     5858 2023-06-03 04:10:48.439015 customtkinterx-0.4.1/customtkinterx/CTkMenuBar/title_menu_win.py
+-rw-r--r--   0        0        0     7659 2023-06-20 11:03:56.651312 customtkinterx-0.4.1/customtkinterx/CTkMinimalTheme.py
+-rw-r--r--   0        0        0     6337 2023-06-04 02:14:05.106099 customtkinterx-0.4.1/customtkinterx/CTkOffice2019Theme.py
+-rw-r--r--   0        0        0      241 2023-05-31 01:43:30.000000 customtkinterx-0.4.1/customtkinterx/CTkPDFViewer/__init__.py
+-rw-r--r--   0        0        0      445 2023-06-03 04:13:46.400109 customtkinterx-0.4.1/customtkinterx/CTkPDFViewer/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     6312 2023-06-03 05:49:55.800794 customtkinterx-0.4.1/customtkinterx/CTkPDFViewer/__pycache__/ctk_pdf_viewer.cpython-311.pyc
+-rw-r--r--   0        0        0     3543 2023-06-03 05:14:11.938896 customtkinterx-0.4.1/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py
+-rw-r--r--   0        0        0     2971 2023-06-20 10:09:30.744234 customtkinterx-0.4.1/customtkinterx/CTkSnackBar.py
+-rw-r--r--   0        0        0      227 2023-05-31 01:40:22.000000 customtkinterx-0.4.1/customtkinterx/CTkTable/__init__.py
+-rw-r--r--   0        0        0      427 2023-06-03 04:41:34.919572 customtkinterx-0.4.1/customtkinterx/CTkTable/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    11621 2023-06-03 04:41:34.922572 customtkinterx-0.4.1/customtkinterx/CTkTable/__pycache__/ctktable.cpython-311.pyc
+-rw-r--r--   0        0        0     8158 2023-06-03 04:41:34.520984 customtkinterx-0.4.1/customtkinterx/CTkTable/ctktable.py
+-rw-r--r--   0        0        0      225 2023-05-08 22:30:16.000000 customtkinterx-0.4.1/customtkinterx/CTkToolTip/__init__.py
+-rw-r--r--   0        0        0      426 2023-06-03 04:22:17.427710 customtkinterx-0.4.1/customtkinterx/CTkToolTip/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    10684 2023-06-03 04:26:02.400121 customtkinterx-0.4.1/customtkinterx/CTkToolTip/__pycache__/ctk_tooltip.cpython-311.pyc
+-rw-r--r--   0        0        0     6942 2023-06-03 04:22:52.495987 customtkinterx-0.4.1/customtkinterx/CTkToolTip/ctk_tooltip.py
+-rw-r--r--   0        0        0     6122 2023-06-19 11:03:32.207624 customtkinterx-0.4.1/customtkinterx/Fluent.json
+-rw-r--r--   0        0        0      113 2023-06-09 23:34:51.644065 customtkinterx-0.4.1/customtkinterx/fluent_android/__init__.py
+-rw-r--r--   0        0        0      305 2023-06-09 23:34:52.417977 customtkinterx-0.4.1/customtkinterx/fluent_android/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     7135 2023-06-09 23:42:37.438327 customtkinterx-0.4.1/customtkinterx/fluent_android/__pycache__/CTkFluentAndroidTheme.cpython-311.pyc
+-rw-r--r--   0        0        0     6375 2023-06-09 23:42:02.599385 customtkinterx-0.4.1/customtkinterx/fluent_android/CTkFluentAndroidTheme.py
+-rw-r--r--   0        0        0     1779 2023-06-19 00:59:49.124414 customtkinterx-0.4.1/customtkinterx/fluent_android/CTkFluentAppBar.py
+-rw-r--r--   0        0        0     5680 2023-06-10 00:28:44.744869 customtkinterx-0.4.1/customtkinterx/fluent_android/FluentAndroid.json
+-rw-r--r--   0        0        0     5437 2023-06-04 13:11:47.958728 customtkinterx-0.4.1/customtkinterx/GhostShark.json
+-rw-r--r--   0        0        0    10021 2023-06-20 08:42:06.949292 customtkinterx-0.4.1/customtkinterx/LaunchMusix.py
+-rw-r--r--   0        0        0     6706 2023-06-20 12:01:51.720398 customtkinterx-0.4.1/customtkinterx/Material.json
+-rw-r--r--   0        0        0     6706 2023-06-20 10:59:12.383731 customtkinterx-0.4.1/customtkinterx/Minimal.json
+-rw-r--r--   0        0        0     1377 2023-06-04 11:35:40.844283 customtkinterx-0.4.1/customtkinterx/Musix-Dark.png
+-rw-r--r--   0        0        0     1039 2023-06-04 11:33:35.093179 customtkinterx-0.4.1/customtkinterx/Musix.png
+-rw-r--r--   0        0        0     5683 2023-06-03 23:01:51.610936 customtkinterx-0.4.1/customtkinterx/Office2019.json
+-rw-r--r--   0        0        0    84836 2022-04-30 00:01:08.000000 customtkinterx-0.4.1/customtkinterx/PublicSans-Regular.ttf
+-rw-r--r--   0        0        0    11524 2023-06-20 12:12:10.818717 customtkinterx-0.4.1/customtkinterx/test.py
+-rw-r--r--   0        0        0      368 2023-06-20 12:13:08.872433 customtkinterx-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3698 2023-06-20 08:20:21.780955 customtkinterx-0.4.1/README.md
+-rw-r--r--   0        0        0     4177 1970-01-01 00:00:00.000000 customtkinterx-0.4.1/PKG-INFO
```

### Comparing `customtkinterx-0.4.0/customtkinterx/__init__.py` & `customtkinterx-0.4.1/customtkinterx/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from customtkinterx.CTkCustom import CTkCustom
 from customtkinterx.CTkFluentTheme import use_fluent_theme as CTkFluentTheme
 from customtkinterx.CTkMinimalTheme import use_minimal_theme as CTkMinimalTheme
+from customtkinterx.CTkMaterialTheme import use_material_theme as CTkMaterialTheme
 from customtkinterx.CTkOffice2019Theme import use_office2019_theme as CTkOffice2019Theme
 from customtkinterx.CTkGhostSharkTheme import use_ghost_shark_theme as CTkGhostSharkTheme
 
 from customtkinterx.CTkInfoBar import CTkInfoBar, NORMAL, SUCCESS, CAUTION, CRITICAL
 from customtkinterx.CTkMegaMenuBar import CTkMegaMenuBar
+from customtkinterx.CTkSnackBar import CTkSnackBar
+from customtkinterx.CTkKanban import CTkKanbanCard, CTkKanban
 
 from customtkinterx.fluent_android import *
 
 # From https://github.com/Akascape/CTkMenuBar
 from customtkinterx.CTkMenuBar import CTkMenuBar, CTkTitleMenu, CustomDropdownMenu as CTkCustomDropdownMenu
 
 # From https://github.com/Akascape/CTkPDFViewer
```

### Comparing `customtkinterx-0.4.0/customtkinterx/__main__.py` & `customtkinterx-0.4.1/customtkinterx/__main__.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.0/customtkinterx/CTkCustom.py` & `customtkinterx-0.4.1/customtkinterx/CTkCustom.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,29 +155,31 @@
         self.__button_minimize = CTkButton(self.__frame_title, text="–", width=30, height=30,
                                            command=lambda: self.minimize())
         from sys import platform
         if platform == "win32":
             self.__button_minimize.pack(side="right", anchor="e", padx=5, pady=5)
 
         if "CTkCustom" in ThemeManager.theme:
-
-            self.__label_title._text_color = ThemeManager.theme["CTkCustom"]["title_color"]
-            self.__label_title._draw()
-
-            self.__button_close._text_color = ThemeManager.theme["CTkCustom"]["closebutton_text_color"]
-            self.__button_close._fg_color = ThemeManager.theme["CTkCustom"]["closebutton_color"]
-            self.__button_close._hover_color = ThemeManager.theme["CTkCustom"]["closebutton_hover_color"]
-            self.__button_close._border_width = ThemeManager.theme["CTkCustom"]["closebutton_border_width"]
-            self.__button_close._draw()
-
-            self.__button_minimize._text_color = ThemeManager.theme["CTkCustom"]["minimizebutton_text_color"]
-            self.__button_minimize._fg_color = ThemeManager.theme["CTkCustom"]["minimizebutton_color"]
-            self.__button_minimize._hover_color = ThemeManager.theme["CTkCustom"]["minimizebutton_hover_color"]
-            self.__button_minimize._border_width = ThemeManager.theme["CTkCustom"]["minimizebutton_border_width"]
-            self.__button_minimize._draw()
+            try:
+                self.__label_title._text_color = ThemeManager.theme["CTkCustom"]["title_color"]
+                self.__label_title._draw()
+
+                self.__button_close._text_color = ThemeManager.theme["CTkCustom"]["closebutton_text_color"]
+                self.__button_close._fg_color = ThemeManager.theme["CTkCustom"]["closebutton_color"]
+                self.__button_close._hover_color = ThemeManager.theme["CTkCustom"]["closebutton_hover_color"]
+                self.__button_close._border_width = ThemeManager.theme["CTkCustom"]["closebutton_border_width"]
+                self.__button_close._draw()
+
+                self.__button_minimize._text_color = ThemeManager.theme["CTkCustom"]["minimizebutton_text_color"]
+                self.__button_minimize._fg_color = ThemeManager.theme["CTkCustom"]["minimizebutton_color"]
+                self.__button_minimize._hover_color = ThemeManager.theme["CTkCustom"]["minimizebutton_hover_color"]
+                self.__button_minimize._border_width = ThemeManager.theme["CTkCustom"]["minimizebutton_border_width"]
+                self.__button_minimize._draw()
+            except:
+                pass
 
         if platform == "linux":
             self.__frame_border.configure(corner_radius=0)
 
         self.x, self.y = 0, 0
 
         self.sg_x = 0
@@ -221,12 +223,12 @@
 
 
 class CTkCustomToplevel(CTkCustom, CTkToplevel):
     pass
 
 
 if __name__ == '__main__':
-    root = CTkCustom(window_edge=True)
+    root = CTkCustom()
     root.title("helloworld")
     root.titlebar_title.configure(text="helloworld")
 
     root.mainloop()
```

### Comparing `customtkinterx-0.4.0/customtkinterx/CTkFluentTheme.py` & `customtkinterx-0.4.1/customtkinterx/fluent_android/CTkFluentAndroidTheme.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-fluent_json = """
+fluent_android_json = """
 {
   "CTkCustom": {
     "titlebar_color": ["#ffffff", "#2c2c2c"],
     "title_color": ["gray10", "#DCE4EE"],
 
     "transparent_color": "#101010",
 
@@ -34,17 +34,17 @@
   "CTk": {
     "fg_color": ["#ffffff", "#101010"]
   },
   "CTkToplevel": {
     "fg_color": ["#ffffff", "#101010"]
   },
   "CTkFrame": {
-    "corner_radius": 8,
+    "corner_radius": 0,
     "border_width": 1,
-    "fg_color": ["#ffffff", "#1c1c1c"],
+    "fg_color": ["#ffffff", "#212121"],
     "top_fg_color": ["#ffffff", "#2c2c2c"],
     "border_color": ["#b0b2b2", "#424556"]
   },
   "CTkButton": {
     "corner_radius": 6,
     "border_width": 0,
     "fg_color": ["#0067c0", "#4cc2ff"],
@@ -187,25 +187,25 @@
 }
 """
 
 
 import os.path
 
 
-fluent_path = os.path.abspath(os.path.dirname(__file__)).replace("\\", "/") + "/Fluent.json"
+fluent_android_path = os.path.abspath(os.path.dirname(__file__)).replace("\\", "/") + "/FluentAndroid.json"
 
 
-def fluent_theme():
+def fluent_android_theme():
     from tempfile import mkstemp
     from customtkinter import set_default_color_theme
     _, __temp = mkstemp(suffix=".json")
     with open(__temp, "w") as __temp_file:
-        __temp_file.write(fluent_json)
+        __temp_file.write(fluent_android_json)
     return __temp
 
 
-def use_fluent_theme():
+def use_fluent_android_theme():
     from customtkinter import set_default_color_theme
     try:
-        set_default_color_theme(fluent_path)
+        set_default_color_theme(fluent_android_path)
     except FileNotFoundError:
-        set_default_color_theme(fluent_theme())
+        set_default_color_theme(fluent_android_theme())
```

### Comparing `customtkinterx-0.4.0/customtkinterx/CTkGhostSharkTheme.py` & `customtkinterx-0.4.1/customtkinterx/CTkGhostSharkTheme.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.0/customtkinterx/CTkInfoBar.py` & `customtkinterx-0.4.1/customtkinterx/CTkInfoBar.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,42 +49,47 @@
                 severity = SUCCESS
             elif __r == 2:
                 severity = CAUTION
             elif __r == 3:
                 severity = CRITICAL
 
         if "CTkInfoBar" in ThemeManager.theme:
-            if fg_color is None:
-                if severity == NORMAL:
-                    self._fg_color = ThemeManager.theme["CTkInfoBar"]["fg_color"]
-                elif severity == SUCCESS:
-                    self._fg_color = ThemeManager.theme["CTkInfoBar"]["success_color"]
-                elif severity == CAUTION:
-                    self._fg_color = ThemeManager.theme["CTkInfoBar"]["caution_color"]
-                elif severity == CRITICAL:
-                    self._fg_color = ThemeManager.theme["CTkInfoBar"]["critical_color"]
-            if border_color is None:
-                if severity == NORMAL:
-                    self._border_color = ThemeManager.theme["CTkInfoBar"]["border_color"]
-                elif severity == SUCCESS:
-                    self._border_color = ThemeManager.theme["CTkInfoBar"]["success_border_color"]
-                elif severity == CAUTION:
-                    self._border_color = ThemeManager.theme["CTkInfoBar"]["caution_border_color"]
-                elif severity == CRITICAL:
-                    self._border_color = ThemeManager.theme["CTkInfoBar"]["critical_border_color"]
+            try:
+                if fg_color is None:
+                    if severity == NORMAL:
+                        self._fg_color = ThemeManager.theme["CTkInfoBar"]["fg_color"]
+                    elif severity == SUCCESS:
+                        self._fg_color = ThemeManager.theme["CTkInfoBar"]["success_color"]
+                    elif severity == CAUTION:
+                        self._fg_color = ThemeManager.theme["CTkInfoBar"]["caution_color"]
+                    elif severity == CRITICAL:
+                        self._fg_color = ThemeManager.theme["CTkInfoBar"]["critical_color"]
+                if border_color is None:
+                    if severity == NORMAL:
+                        self._border_color = ThemeManager.theme["CTkInfoBar"]["border_color"]
+                    elif severity == SUCCESS:
+                        self._border_color = ThemeManager.theme["CTkInfoBar"]["success_border_color"]
+                    elif severity == CAUTION:
+                        self._border_color = ThemeManager.theme["CTkInfoBar"]["caution_border_color"]
+                    elif severity == CRITICAL:
+                        self._border_color = ThemeManager.theme["CTkInfoBar"]["critical_border_color"]
+                if corner_radius is None:
+                    self._corner_radius = ThemeManager.theme["CTkInfoBar"]["corner_radius"]
+            except:
+                pass
 
         self.__label_title = CTkLabel(self, text=title, font=CTkFont(weight="bold"), anchor="w")
         self.__label_title.pack(fill="y", padx=(8, 4), pady=8, side="left")
 
         self.__label_info = CTkLabel(self, text=text, anchor="w")
 
         self.__label_info.pack(fill="y", padx=(4, 8), pady=8, side="left")
 
         self.__button_close = CTkButton(self, border_width=0, width=30, height=30, text="✕",
-                                        command=lambda: self.destroy())
+                                        command=lambda: self.forget())
 
         self.configure(can_close=can_close)
 
         if "CTkInfoBar" in ThemeManager.theme:
             if fg_color is None:
                 if severity == NORMAL:
                     self.__button_close._fg_color = ThemeManager.theme["CTkInfoBar"]["fg_color"]
@@ -95,31 +100,33 @@
                 elif severity == CAUTION:
                     self.__button_close._fg_color = ThemeManager.theme["CTkInfoBar"]["caution_color"]
                     self.__button_close._hover_color = ThemeManager.theme["CTkInfoBar"]["caution_hover_color"]
                 elif severity == CRITICAL:
                     self.__button_close._fg_color = ThemeManager.theme["CTkInfoBar"]["critical_color"]
                     self.__button_close._hover_color = ThemeManager.theme["CTkInfoBar"]["critical_hover_color"]
             if text_color is None:
-                print("asd")
-                if severity == NORMAL:
-                    self.__button_close._text_color = ThemeManager.theme["CTkInfoBar"]["text_color"]
-                    self.__label_title._text_color = ThemeManager.theme["CTkInfoBar"]["text_color"]
-                    self.__label_info._text_color = ThemeManager.theme["CTkInfoBar"]["text_color"]
-                elif severity == SUCCESS:
-                    self.__button_close._text_color = ThemeManager.theme["CTkInfoBar"]["success_text_color"]
-                    self.__label_title._text_color = ThemeManager.theme["CTkInfoBar"]["success_text_color"]
-                    self.__label_info._text_color = ThemeManager.theme["CTkInfoBar"]["success_text_color"]
-                elif severity == CAUTION:
-                    self.__button_close._text_color = ThemeManager.theme["CTkInfoBar"]["caution_text_color"]
-                    self.__label_title._text_color = ThemeManager.theme["CTkInfoBar"]["caution_text_color"]
-                    self.__label_info._text_color = ThemeManager.theme["CTkInfoBar"]["caution_text_color"]
-                elif severity == CRITICAL:
-                    self.__button_close._text_color = ThemeManager.theme["CTkInfoBar"]["critical_text_color"]
-                    self.__label_title._text_color = ThemeManager.theme["CTkInfoBar"]["critical_text_color"]
-                    self.__label_info._text_color = ThemeManager.theme["CTkInfoBar"]["critical_text_color"]
+                try:
+                    if severity == NORMAL:
+                        self.__button_close._text_color = ThemeManager.theme["CTkInfoBar"]["text_color"]
+                        self.__label_title._text_color = ThemeManager.theme["CTkInfoBar"]["text_color"]
+                        self.__label_info._text_color = ThemeManager.theme["CTkInfoBar"]["text_color"]
+                    elif severity == SUCCESS:
+                        self.__button_close._text_color = ThemeManager.theme["CTkInfoBar"]["success_text_color"]
+                        self.__label_title._text_color = ThemeManager.theme["CTkInfoBar"]["success_text_color"]
+                        self.__label_info._text_color = ThemeManager.theme["CTkInfoBar"]["success_text_color"]
+                    elif severity == CAUTION:
+                        self.__button_close._text_color = ThemeManager.theme["CTkInfoBar"]["caution_text_color"]
+                        self.__label_title._text_color = ThemeManager.theme["CTkInfoBar"]["caution_text_color"]
+                        self.__label_info._text_color = ThemeManager.theme["CTkInfoBar"]["caution_text_color"]
+                    elif severity == CRITICAL:
+                        self.__button_close._text_color = ThemeManager.theme["CTkInfoBar"]["critical_text_color"]
+                        self.__label_title._text_color = ThemeManager.theme["CTkInfoBar"]["critical_text_color"]
+                        self.__label_info._text_color = ThemeManager.theme["CTkInfoBar"]["critical_text_color"]
+                except:
+                    pass
 
         self._draw()
         self.__button_close._draw()
         self.__label_title._draw()
         self.__label_info._draw()
 
     @property
@@ -153,18 +160,18 @@
 
     def show(self, **kwargs):
         self.pack_configure(side="top", fill="x", ipadx=1, ipady=1, padx=5, pady=5)
         self.pack(**kwargs)
 
 
 if __name__ == '__main__':
-    from customtkinterx import CTkCustom, CTkMinimalTheme, CTkFluentTheme
+    from customtkinterx import CTkCustom, CTkMinimalTheme
     from customtkinter import set_appearance_mode, CTkButton, CTkSwitch
 
-    CTkFluentTheme()
+    CTkMinimalTheme()
 
     root = CTkCustom()
     root.create_sizegrip()
 
     set_appearance_mode("system")
 
     CTkInfoBar(root.mainframe, text="hello, i am a infobar", severity=NORMAL).show()
```

### Comparing `customtkinterx-0.4.0/customtkinterx/CTkListBox.py` & `customtkinterx-0.4.1/customtkinterx/CTkListBox.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 
 class CTkList(CTkScrollableFrame):
     def __init__(self, master=None, **kwargs):
         super().__init__(master, **kwargs)
 
     def add(self, text="", text_anchor="w"):
-        __frame = CTkFrame(self)
+        __frame = CTkFrame(self, fg_color=self._parent_frame._fg_color, border_width=0)
         __label = CTkLabel(__frame, text=text, anchor=text_anchor)
-        __label.pack(fill="x", padx=5, pady=5, ipadx=2.5, ipady=2.5)
+        __label.pack(fill="x", padx=2, pady=2)
         __frame.pack(fill="x", padx=2.5, pady=2.5)
 
         def click(event):
             self.event_generate("<<ListSelected>>", x=event.x, y=event.y, state=event.state, data={"text": text})
 
         __frame.bind("<Button-1>", click)
         __label.bind("<Button-1>", click)
@@ -20,17 +20,17 @@
         return __frame, __label
 
     def clear(self):
         for index in self.winfo_children(): index.destroy()
 
 
 if __name__ == '__main__':
-    from customtkinterx import CTkCustom, CTkFluentTheme
+    from customtkinterx import CTkCustom, CTkMinimalTheme
 
-    CTkFluentTheme()
+    CTkMinimalTheme()
 
     root = CTkCustom()
     root.create_sizegrip()
 
     list = CTkList(root.mainframe)
 
     for index in range(20):
```

### Comparing `customtkinterx-0.4.0/customtkinterx/CTkMegaMenuBar.py` & `customtkinterx-0.4.1/customtkinterx/CTkMegaMenuBar.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.0/customtkinterx/CTkMenuBar/__pycache__/__init__.cpython-311.pyc` & `customtkinterx-0.4.1/customtkinterx/CTkMenuBar/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.0/customtkinterx/CTkMenuBar/__pycache__/dropdown_menu.cpython-311.pyc` & `customtkinterx-0.4.1/customtkinterx/CTkMenuBar/__pycache__/dropdown_menu.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.0/customtkinterx/CTkMenuBar/__pycache__/menu_bar.cpython-311.pyc` & `customtkinterx-0.4.1/customtkinterx/CTkMenuBar/__pycache__/menu_bar.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.0/customtkinterx/CTkMenuBar/__pycache__/title_menu_win.cpython-311.pyc` & `customtkinterx-0.4.1/customtkinterx/CTkMenuBar/__pycache__/title_menu_win.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.0/customtkinterx/CTkMenuBar/dropdown_menu.py` & `customtkinterx-0.4.1/customtkinterx/CTkMenuBar/dropdown_menu.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.0/customtkinterx/CTkMenuBar/menu_bar.py` & `customtkinterx-0.4.1/customtkinterx/CTkMenuBar/menu_bar.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.0/customtkinterx/CTkMenuBar/title_menu_win.py` & `customtkinterx-0.4.1/customtkinterx/CTkMenuBar/title_menu_win.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.0/customtkinterx/CTkMinimalTheme.py` & `customtkinterx-0.4.1/customtkinterx/CTkOffice2019Theme.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-minimal_json = """
+office2019_json = """
 {
   "CTkCustom": {
-    "titlebar_color": ["#f4f6f8", "#212b36"],
-    "title_color": ["gray10", "#DCE4EE"],
+    "titlebar_color": ["#106ebe", "#106ebe"],
+    "title_color": ["#ffffff", "#ffffff"],
 
     "transparent_color": "#101010",
 
     "closebutton_text_color": ["#000000", "#ffffff"],
-    "closebutton_color": ["#f4f6f8", "#212b36"],
+    "closebutton_color": ["#ffffff", "#2c2c2c"],
     "closebutton_hover_color": ["#b40d1b", "#b40d1b"],
 
     "minimizebutton_text_color": ["#000000", "#ffffff"],
-    "minimizebutton_color": ["#f4f6f8", "#212b36"],
-    "minimizebutton_hover_color": ["#dfe3e8", "#454f5b"]
+    "minimizebutton_color": ["#ffffff", "#2c2c2c"],
+    "minimizebutton_hover_color": ["#cccccc", "#282828"]
   },
   "CTkInfoBar": {
     "corner_radius": 8,
     "border_width": 0,
 
-    "fg_color": ["#61f3f3", "#006c9c"],
-    "fg_hover_color": ["#cafdf5", "#003768"],
+    "fg_color": ["#f7f7f7", "#2f2f2f"],
+    "fg_hover_color": ["#c3c3c3", "#555555"],
 
     "border_color": ["#b0b2b2", "#424556"],
 
-    "success_color": ["#86e8ab", "#1b806a"],
-    "success_hover_color": ["#d8fbde", "#0a5554"],
-    "caution_color": ["#ffd666", "#b76e00"],
-    "caution_hover_color": ["#fff5cc", "#7a4100"],
-    "critical_color": ["#ffac82", "#b71d18"],
-    "critical_hover_color": ["#ffe9d5", "#7a0916"]
+    "success_color": ["#dff6dd", "#393d1b"],
+    "success_hover_color": ["#b0c3af", "#5c632b"],
+    "caution_color": ["#fff4ce", "#433519"],
+    "caution_hover_color": ["#ccc3a4", "#695327"],
+    "critical_color": ["#fde7e9", "#442726"],
+    "critical_hover_color": ["#cab8ba", "#6a3c3b"]
 
   },
   "CTk": {
-    "fg_color": ["#f9fafb", "#161c24"]
+    "fg_color": ["#ffffff", "#101010"]
   },
   "CTkToplevel": {
-    "fg_color": ["#f9fafb", "#161c24"]
+    "fg_color": ["#ffffff", "#101010"]
   },
   "CTkFrame": {
-    "corner_radius": 10,
+    "corner_radius": 0,
     "border_width": 1,
-    "fg_color": ["#f9fafb", "#161c24"],
-    "top_fg_color": ["#f4f6f8", "#212b36"],
-    "border_color": ["#edeff1", "#212b36"]
+    "fg_color": ["#ffffff", "#1c1c1c"],
+    "top_fg_color": ["#ffffff", "#2c2c2c"],
+    "border_color": ["#b0b2b2", "#424556"]
   },
   "CTkButton": {
-    "corner_radius": 10,
-    "border_width": 0,
-    "fg_color": "#00ab55",
-    "hover_color": "#007b55",
+    "corner_radius": 0,
+    "border_width": 1,
+    "fg_color": ["#e5e5e5", "#3d3d3d"],
+    "hover_color": ["#b2b2b2", "#151515"],
     "border_color": ["#f3f3f3", "#949A9F"],
-    "text_color": ["#ffffff", "#000000"],
+    "text_color": ["#000000", "#ffffff"],
     "text_color_disabled": ["gray74", "gray60"]
   },
   "CTkLabel": {
     "corner_radius": 0,
     "fg_color": "transparent",
     "text_color": ["gray10", "#DCE4EE"]
   },
   "CTkEntry": {
-    "corner_radius": 10,
+    "corner_radius": 0,
     "border_width": 1,
-    "fg_color": ["#dfe3e8", "#454f5b"],
-    "border_color": ["#c4cdd5", "#637381"],
+    "fg_color": ["#ffffff", "#2f2f2f"],
+    "border_color": ["#f3f3f3", "#949A9F"],
     "text_color":["#000000", "#ffffff"],
     "placeholder_text_color": ["gray52", "gray62"]
   },
   "CTkCheckbox": {
     "corner_radius": 6,
     "border_width": 3,
     "fg_color": ["#3B8ED0", "#1F6AA5"],
     "border_color": ["#3E454A", "#949A9F"],
     "hover_color": ["#3B8ED0", "#1F6AA5"],
     "checkmark_color": ["#DCE4EE", "gray90"],
     "text_color": ["gray10", "#DCE4EE"],
     "text_color_disabled": ["gray60", "gray45"]
   },
   "CTkSwitch": {
-    "corner_radius": 1000,
-    "border_width": 0,
-    "button_length": 0,
-    "fg_color": ["#c4cdd5", "#637381"],
-    "progress_color": "#00ab55",
-    "button_color": ["#f9fafb", "#161c24"],
-    "button_hover_color": ["#f4f6f8", "#212b36"],
+    "corner_radius": 8,
+    "border_width": 1,
+    "button_length": 2,
+    "fg_color": ["#ededed", "#1d1d1d"],
+    "progress_color": ["#0067c0", "#4cc2ff"],
+    "button_color": ["#f3f3f3", "#000000"],
+    "button_hover_color": ["#bfbfbf", "#050505"],
     "text_color": ["gray10", "#DCE4EE"],
     "text_color_disabled": ["gray60", "gray45"]
   },
   "CTkRadiobutton": {
     "corner_radius": 1000,
     "border_width_checked": 6,
     "border_width_unchecked": 3,
@@ -119,46 +119,46 @@
     "fg_color": ["#3B8ED0", "#1F6AA5"],
     "button_color": ["#36719F", "#144870"],
     "button_hover_color": ["#27577D", "#203A4F"],
     "text_color": ["#DCE4EE", "#DCE4EE"],
     "text_color_disabled": ["gray74", "gray60"]
   },
   "CTkComboBox": {
-    "corner_radius": 10,
+    "corner_radius": 0,
     "border_width": 1,
-    "fg_color": ["#dfe3e8", "#454f5b"],
-    "border_color": ["#c4cdd5", "#637381"],
-    "button_color": ["#c4cdd5", "#637381"],
-    "button_hover_color": ["#919eab", "#919eab"],
+    "fg_color": ["#ffffff", "#2f2f2f"],
+    "border_color": ["#f3f3f3", "#949A9F"],
+    "button_color": ["#f2f2f2", "#565B5E"],
+    "button_hover_color": ["#f2f2f2", "#565B5E"],
     "text_color": ["gray10", "#ffffff"],
     "text_color_disabled": ["gray50", "gray45"]
   },
   "CTkScrollbar": {
-    "corner_radius": 1000,
-    "border_spacing": 4,
+    "corner_radius": 0,
+    "border_spacing": 9,
     "fg_color": "transparent",
-    "button_color": ["#f4f6f8", "#212b36"],
-    "button_hover_color": ["#dfe3e8", "#454f5b"]
+    "button_color": ["gray55", "gray41"],
+    "button_hover_color": ["gray40", "gray53"]
   },
   "CTkSegmentedButton": {
     "corner_radius": 6,
     "border_width": 2,
     "fg_color": ["#979DA2", "gray29"],
     "selected_color": ["#3B8ED0", "#1F6AA5"],
     "selected_hover_color": ["#36719F", "#144870"],
     "unselected_color": ["#979DA2", "gray29"],
     "unselected_hover_color": ["gray70", "gray41"],
     "text_color": ["#DCE4EE", "#DCE4EE"],
     "text_color_disabled": ["gray74", "gray60"]
   },
   "CTkTextbox": {
-    "corner_radius": 6,
-    "border_width": 0,
-    "fg_color": ["#dfe3e8", "#454f5b"],
-    "border_color": ["#979DA2", "#565B5E"],
+    "corner_radius": 0,
+    "border_width": 1,
+    "fg_color": ["#F9F9FA", "#1D1E1E"],
+    "border_color": ["#f3f3f3", "#949A9F"],
     "text_color":["gray10", "#DCE4EE"],
     "scrollbar_button_color": ["gray55", "gray41"],
     "scrollbar_button_hover_color": ["gray40", "gray53"]
   },
   "CTkScrollableFrame": {
     "label_fg_color": ["gray78", "gray23"]
   },
@@ -170,15 +170,15 @@
   "CTkFont": {
     "macOS": {
       "family": "SF Display",
       "size": 13,
       "weight": "normal"
     },
     "Windows": {
-      "family": "Roboto",
+      "family": "Segoe UI",
       "size": 13,
       "weight": "normal"
     },
     "Linux": {
       "family": "Roboto",
       "size": 13,
       "weight": "normal"
@@ -187,25 +187,25 @@
 }
 """
 
 
 import os.path
 
 
-minimal_path = os.path.abspath(os.path.dirname(__file__)).replace("\\", "/") + "/Minimal.json"
+office2019_path = os.path.abspath(os.path.dirname(__file__)).replace("\\", "/") + "/Office2019.json"
 
 
-def minimal_theme():
+def office2019_theme():
     from tempfile import mkstemp
     from customtkinter import set_default_color_theme
     _, __temp = mkstemp(suffix=".json")
     with open(__temp, "w") as __temp_file:
-        __temp_file.write(minimal_json)
+        __temp_file.write(office2019_json)
     return __temp
 
 
-def use_minimal_theme():
+def use_office2019_theme():
     from customtkinter import set_default_color_theme
     try:
-        set_default_color_theme(minimal_path)
+        set_default_color_theme(office2019_path)
     except FileNotFoundError:
-        set_default_color_theme(minimal_theme())
+        set_default_color_theme(office2019_theme())
```

### Comparing `customtkinterx-0.4.0/customtkinterx/CTkOffice2019Theme.py` & `customtkinterx-0.4.1/customtkinterx/Office2019.json`

 * *Files 4% similar despite different names*

```diff
@@ -1,397 +1,356 @@
-00000000: 6f66 6669 6365 3230 3139 5f6a 736f 6e20  office2019_json 
-00000010: 3d20 2222 220d 0a7b 0d0a 2020 2243 546b  = """..{..  "CTk
-00000020: 4375 7374 6f6d 223a 207b 0d0a 2020 2020  Custom": {..    
-00000030: 2274 6974 6c65 6261 725f 636f 6c6f 7222  "titlebar_color"
-00000040: 3a20 5b22 2331 3036 6562 6522 2c20 2223  : ["#106ebe", "#
-00000050: 3130 3665 6265 225d 2c0d 0a20 2020 2022  106ebe"],..    "
-00000060: 7469 746c 655f 636f 6c6f 7222 3a20 5b22  title_color": ["
-00000070: 2366 6666 6666 6622 2c20 2223 6666 6666  #ffffff", "#ffff
-00000080: 6666 225d 2c0d 0a0d 0a20 2020 2022 7472  ff"],....    "tr
-00000090: 616e 7370 6172 656e 745f 636f 6c6f 7222  ansparent_color"
-000000a0: 3a20 2223 3130 3130 3130 222c 0d0a 0d0a  : "#101010",....
-000000b0: 2020 2020 2263 6c6f 7365 6275 7474 6f6e      "closebutton
-000000c0: 5f74 6578 745f 636f 6c6f 7222 3a20 5b22  _text_color": ["
-000000d0: 2330 3030 3030 3022 2c20 2223 6666 6666  #000000", "#ffff
-000000e0: 6666 225d 2c0d 0a20 2020 2022 636c 6f73  ff"],..    "clos
-000000f0: 6562 7574 746f 6e5f 636f 6c6f 7222 3a20  ebutton_color": 
-00000100: 5b22 2366 6666 6666 6622 2c20 2223 3263  ["#ffffff", "#2c
-00000110: 3263 3263 225d 2c0d 0a20 2020 2022 636c  2c2c"],..    "cl
-00000120: 6f73 6562 7574 746f 6e5f 686f 7665 725f  osebutton_hover_
-00000130: 636f 6c6f 7222 3a20 5b22 2362 3430 6431  color": ["#b40d1
-00000140: 6222 2c20 2223 6234 3064 3162 225d 2c0d  b", "#b40d1b"],.
-00000150: 0a0d 0a20 2020 2022 6d69 6e69 6d69 7a65  ...    "minimize
-00000160: 6275 7474 6f6e 5f74 6578 745f 636f 6c6f  button_text_colo
-00000170: 7222 3a20 5b22 2330 3030 3030 3022 2c20  r": ["#000000", 
-00000180: 2223 6666 6666 6666 225d 2c0d 0a20 2020  "#ffffff"],..   
-00000190: 2022 6d69 6e69 6d69 7a65 6275 7474 6f6e   "minimizebutton
-000001a0: 5f63 6f6c 6f72 223a 205b 2223 6666 6666  _color": ["#ffff
-000001b0: 6666 222c 2022 2332 6332 6332 6322 5d2c  ff", "#2c2c2c"],
-000001c0: 0d0a 2020 2020 226d 696e 696d 697a 6562  ..    "minimizeb
-000001d0: 7574 746f 6e5f 686f 7665 725f 636f 6c6f  utton_hover_colo
-000001e0: 7222 3a20 5b22 2363 6363 6363 6322 2c20  r": ["#cccccc", 
-000001f0: 2223 3238 3238 3238 225d 0d0a 2020 7d2c  "#282828"]..  },
-00000200: 0d0a 2020 2243 546b 496e 666f 4261 7222  ..  "CTkInfoBar"
-00000210: 3a20 7b0d 0a20 2020 2022 636f 726e 6572  : {..    "corner
-00000220: 5f72 6164 6975 7322 3a20 382c 0d0a 2020  _radius": 8,..  
-00000230: 2020 2262 6f72 6465 725f 7769 6474 6822    "border_width"
-00000240: 3a20 302c 0d0a 0d0a 2020 2020 2266 675f  : 0,....    "fg_
-00000250: 636f 6c6f 7222 3a20 5b22 2366 3766 3766  color": ["#f7f7f
-00000260: 3722 2c20 2223 3266 3266 3266 225d 2c0d  7", "#2f2f2f"],.
-00000270: 0a20 2020 2022 6667 5f68 6f76 6572 5f63  .    "fg_hover_c
-00000280: 6f6c 6f72 223a 205b 2223 6333 6333 6333  olor": ["#c3c3c3
-00000290: 222c 2022 2335 3535 3535 3522 5d2c 0d0a  ", "#555555"],..
-000002a0: 0d0a 2020 2020 2262 6f72 6465 725f 636f  ..    "border_co
-000002b0: 6c6f 7222 3a20 5b22 2362 3062 3262 3222  lor": ["#b0b2b2"
-000002c0: 2c20 2223 3432 3435 3536 225d 2c0d 0a0d  , "#424556"],...
-000002d0: 0a20 2020 2022 7375 6363 6573 735f 636f  .    "success_co
-000002e0: 6c6f 7222 3a20 5b22 2364 6666 3664 6422  lor": ["#dff6dd"
-000002f0: 2c20 2223 3339 3364 3162 225d 2c0d 0a20  , "#393d1b"],.. 
-00000300: 2020 2022 7375 6363 6573 735f 686f 7665     "success_hove
-00000310: 725f 636f 6c6f 7222 3a20 5b22 2362 3063  r_color": ["#b0c
-00000320: 3361 6622 2c20 2223 3563 3633 3262 225d  3af", "#5c632b"]
-00000330: 2c0d 0a20 2020 2022 6361 7574 696f 6e5f  ,..    "caution_
-00000340: 636f 6c6f 7222 3a20 5b22 2366 6666 3463  color": ["#fff4c
-00000350: 6522 2c20 2223 3433 3335 3139 225d 2c0d  e", "#433519"],.
-00000360: 0a20 2020 2022 6361 7574 696f 6e5f 686f  .    "caution_ho
-00000370: 7665 725f 636f 6c6f 7222 3a20 5b22 2363  ver_color": ["#c
-00000380: 6363 3361 3422 2c20 2223 3639 3533 3237  cc3a4", "#695327
-00000390: 225d 2c0d 0a20 2020 2022 6372 6974 6963  "],..    "critic
-000003a0: 616c 5f63 6f6c 6f72 223a 205b 2223 6664  al_color": ["#fd
-000003b0: 6537 6539 222c 2022 2334 3432 3732 3622  e7e9", "#442726"
-000003c0: 5d2c 0d0a 2020 2020 2263 7269 7469 6361  ],..    "critica
-000003d0: 6c5f 686f 7665 725f 636f 6c6f 7222 3a20  l_hover_color": 
-000003e0: 5b22 2363 6162 3862 6122 2c20 2223 3661  ["#cab8ba", "#6a
-000003f0: 3363 3362 225d 0d0a 0d0a 2020 7d2c 0d0a  3c3b"]....  },..
-00000400: 2020 2243 546b 223a 207b 0d0a 2020 2020    "CTk": {..    
-00000410: 2266 675f 636f 6c6f 7222 3a20 5b22 2366  "fg_color": ["#f
-00000420: 6666 6666 6622 2c20 2223 3130 3130 3130  fffff", "#101010
-00000430: 225d 0d0a 2020 7d2c 0d0a 2020 2243 546b  "]..  },..  "CTk
-00000440: 546f 706c 6576 656c 223a 207b 0d0a 2020  Toplevel": {..  
-00000450: 2020 2266 675f 636f 6c6f 7222 3a20 5b22    "fg_color": ["
-00000460: 2366 6666 6666 6622 2c20 2223 3130 3130  #ffffff", "#1010
-00000470: 3130 225d 0d0a 2020 7d2c 0d0a 2020 2243  10"]..  },..  "C
-00000480: 546b 4672 616d 6522 3a20 7b0d 0a20 2020  TkFrame": {..   
-00000490: 2022 636f 726e 6572 5f72 6164 6975 7322   "corner_radius"
-000004a0: 3a20 302c 0d0a 2020 2020 2262 6f72 6465  : 0,..    "borde
-000004b0: 725f 7769 6474 6822 3a20 312c 0d0a 2020  r_width": 1,..  
-000004c0: 2020 2266 675f 636f 6c6f 7222 3a20 5b22    "fg_color": ["
-000004d0: 2366 6666 6666 6622 2c20 2223 3163 3163  #ffffff", "#1c1c
-000004e0: 3163 225d 2c0d 0a20 2020 2022 746f 705f  1c"],..    "top_
-000004f0: 6667 5f63 6f6c 6f72 223a 205b 2223 6666  fg_color": ["#ff
-00000500: 6666 6666 222c 2022 2332 6332 6332 6322  ffff", "#2c2c2c"
-00000510: 5d2c 0d0a 2020 2020 2262 6f72 6465 725f  ],..    "border_
-00000520: 636f 6c6f 7222 3a20 5b22 2362 3062 3262  color": ["#b0b2b
-00000530: 3222 2c20 2223 3432 3435 3536 225d 0d0a  2", "#424556"]..
-00000540: 2020 7d2c 0d0a 2020 2243 546b 4275 7474    },..  "CTkButt
-00000550: 6f6e 223a 207b 0d0a 2020 2020 2263 6f72  on": {..    "cor
-00000560: 6e65 725f 7261 6469 7573 223a 2030 2c0d  ner_radius": 0,.
-00000570: 0a20 2020 2022 626f 7264 6572 5f77 6964  .    "border_wid
-00000580: 7468 223a 2031 2c0d 0a20 2020 2022 6667  th": 1,..    "fg
-00000590: 5f63 6f6c 6f72 223a 205b 2223 6535 6535  _color": ["#e5e5
-000005a0: 6535 222c 2022 2333 6433 6433 6422 5d2c  e5", "#3d3d3d"],
-000005b0: 0d0a 2020 2020 2268 6f76 6572 5f63 6f6c  ..    "hover_col
-000005c0: 6f72 223a 205b 2223 6232 6232 6232 222c  or": ["#b2b2b2",
-000005d0: 2022 2331 3531 3531 3522 5d2c 0d0a 2020   "#151515"],..  
-000005e0: 2020 2262 6f72 6465 725f 636f 6c6f 7222    "border_color"
-000005f0: 3a20 5b22 2366 3366 3366 3322 2c20 2223  : ["#f3f3f3", "#
-00000600: 3934 3941 3946 225d 2c0d 0a20 2020 2022  949A9F"],..    "
-00000610: 7465 7874 5f63 6f6c 6f72 223a 205b 2223  text_color": ["#
-00000620: 3030 3030 3030 222c 2022 2366 6666 6666  000000", "#fffff
-00000630: 6622 5d2c 0d0a 2020 2020 2274 6578 745f  f"],..    "text_
-00000640: 636f 6c6f 725f 6469 7361 626c 6564 223a  color_disabled":
-00000650: 205b 2267 7261 7937 3422 2c20 2267 7261   ["gray74", "gra
-00000660: 7936 3022 5d0d 0a20 207d 2c0d 0a20 2022  y60"]..  },..  "
-00000670: 4354 6b4c 6162 656c 223a 207b 0d0a 2020  CTkLabel": {..  
-00000680: 2020 2263 6f72 6e65 725f 7261 6469 7573    "corner_radius
-00000690: 223a 2030 2c0d 0a20 2020 2022 6667 5f63  ": 0,..    "fg_c
-000006a0: 6f6c 6f72 223a 2022 7472 616e 7370 6172  olor": "transpar
-000006b0: 656e 7422 2c0d 0a20 2020 2022 7465 7874  ent",..    "text
-000006c0: 5f63 6f6c 6f72 223a 205b 2267 7261 7931  _color": ["gray1
-000006d0: 3022 2c20 2223 4443 4534 4545 225d 0d0a  0", "#DCE4EE"]..
-000006e0: 2020 7d2c 0d0a 2020 2243 546b 456e 7472    },..  "CTkEntr
-000006f0: 7922 3a20 7b0d 0a20 2020 2022 636f 726e  y": {..    "corn
-00000700: 6572 5f72 6164 6975 7322 3a20 302c 0d0a  er_radius": 0,..
-00000710: 2020 2020 2262 6f72 6465 725f 7769 6474      "border_widt
-00000720: 6822 3a20 312c 0d0a 2020 2020 2266 675f  h": 1,..    "fg_
-00000730: 636f 6c6f 7222 3a20 5b22 2366 6666 6666  color": ["#fffff
-00000740: 6622 2c20 2223 3266 3266 3266 225d 2c0d  f", "#2f2f2f"],.
-00000750: 0a20 2020 2022 626f 7264 6572 5f63 6f6c  .    "border_col
-00000760: 6f72 223a 205b 2223 6633 6633 6633 222c  or": ["#f3f3f3",
-00000770: 2022 2339 3439 4139 4622 5d2c 0d0a 2020   "#949A9F"],..  
-00000780: 2020 2274 6578 745f 636f 6c6f 7222 3a5b    "text_color":[
-00000790: 2223 3030 3030 3030 222c 2022 2366 6666  "#000000", "#fff
-000007a0: 6666 6622 5d2c 0d0a 2020 2020 2270 6c61  fff"],..    "pla
-000007b0: 6365 686f 6c64 6572 5f74 6578 745f 636f  ceholder_text_co
-000007c0: 6c6f 7222 3a20 5b22 6772 6179 3532 222c  lor": ["gray52",
-000007d0: 2022 6772 6179 3632 225d 0d0a 2020 7d2c   "gray62"]..  },
-000007e0: 0d0a 2020 2243 546b 4368 6563 6b62 6f78  ..  "CTkCheckbox
-000007f0: 223a 207b 0d0a 2020 2020 2263 6f72 6e65  ": {..    "corne
-00000800: 725f 7261 6469 7573 223a 2036 2c0d 0a20  r_radius": 6,.. 
-00000810: 2020 2022 626f 7264 6572 5f77 6964 7468     "border_width
-00000820: 223a 2033 2c0d 0a20 2020 2022 6667 5f63  ": 3,..    "fg_c
-00000830: 6f6c 6f72 223a 205b 2223 3342 3845 4430  olor": ["#3B8ED0
-00000840: 222c 2022 2331 4636 4141 3522 5d2c 0d0a  ", "#1F6AA5"],..
-00000850: 2020 2020 2262 6f72 6465 725f 636f 6c6f      "border_colo
-00000860: 7222 3a20 5b22 2333 4534 3534 4122 2c20  r": ["#3E454A", 
-00000870: 2223 3934 3941 3946 225d 2c0d 0a20 2020  "#949A9F"],..   
-00000880: 2022 686f 7665 725f 636f 6c6f 7222 3a20   "hover_color": 
-00000890: 5b22 2333 4238 4544 3022 2c20 2223 3146  ["#3B8ED0", "#1F
-000008a0: 3641 4135 225d 2c0d 0a20 2020 2022 6368  6AA5"],..    "ch
-000008b0: 6563 6b6d 6172 6b5f 636f 6c6f 7222 3a20  eckmark_color": 
-000008c0: 5b22 2344 4345 3445 4522 2c20 2267 7261  ["#DCE4EE", "gra
-000008d0: 7939 3022 5d2c 0d0a 2020 2020 2274 6578  y90"],..    "tex
-000008e0: 745f 636f 6c6f 7222 3a20 5b22 6772 6179  t_color": ["gray
-000008f0: 3130 222c 2022 2344 4345 3445 4522 5d2c  10", "#DCE4EE"],
-00000900: 0d0a 2020 2020 2274 6578 745f 636f 6c6f  ..    "text_colo
-00000910: 725f 6469 7361 626c 6564 223a 205b 2267  r_disabled": ["g
-00000920: 7261 7936 3022 2c20 2267 7261 7934 3522  ray60", "gray45"
-00000930: 5d0d 0a20 207d 2c0d 0a20 2022 4354 6b53  ]..  },..  "CTkS
-00000940: 7769 7463 6822 3a20 7b0d 0a20 2020 2022  witch": {..    "
-00000950: 636f 726e 6572 5f72 6164 6975 7322 3a20  corner_radius": 
-00000960: 382c 0d0a 2020 2020 2262 6f72 6465 725f  8,..    "border_
-00000970: 7769 6474 6822 3a20 312c 0d0a 2020 2020  width": 1,..    
-00000980: 2262 7574 746f 6e5f 6c65 6e67 7468 223a  "button_length":
-00000990: 2032 2c0d 0a20 2020 2022 6667 5f63 6f6c   2,..    "fg_col
-000009a0: 6f72 223a 205b 2223 6564 6564 6564 222c  or": ["#ededed",
-000009b0: 2022 2331 6431 6431 6422 5d2c 0d0a 2020   "#1d1d1d"],..  
-000009c0: 2020 2270 726f 6772 6573 735f 636f 6c6f    "progress_colo
-000009d0: 7222 3a20 5b22 2330 3036 3763 3022 2c20  r": ["#0067c0", 
-000009e0: 2223 3463 6332 6666 225d 2c0d 0a20 2020  "#4cc2ff"],..   
-000009f0: 2022 6275 7474 6f6e 5f63 6f6c 6f72 223a   "button_color":
-00000a00: 205b 2223 6633 6633 6633 222c 2022 2330   ["#f3f3f3", "#0
-00000a10: 3030 3030 3022 5d2c 0d0a 2020 2020 2262  00000"],..    "b
-00000a20: 7574 746f 6e5f 686f 7665 725f 636f 6c6f  utton_hover_colo
-00000a30: 7222 3a20 5b22 2362 6662 6662 6622 2c20  r": ["#bfbfbf", 
-00000a40: 2223 3035 3035 3035 225d 2c0d 0a20 2020  "#050505"],..   
-00000a50: 2022 7465 7874 5f63 6f6c 6f72 223a 205b   "text_color": [
-00000a60: 2267 7261 7931 3022 2c20 2223 4443 4534  "gray10", "#DCE4
-00000a70: 4545 225d 2c0d 0a20 2020 2022 7465 7874  EE"],..    "text
-00000a80: 5f63 6f6c 6f72 5f64 6973 6162 6c65 6422  _color_disabled"
-00000a90: 3a20 5b22 6772 6179 3630 222c 2022 6772  : ["gray60", "gr
-00000aa0: 6179 3435 225d 0d0a 2020 7d2c 0d0a 2020  ay45"]..  },..  
-00000ab0: 2243 546b 5261 6469 6f62 7574 746f 6e22  "CTkRadiobutton"
-00000ac0: 3a20 7b0d 0a20 2020 2022 636f 726e 6572  : {..    "corner
-00000ad0: 5f72 6164 6975 7322 3a20 3130 3030 2c0d  _radius": 1000,.
-00000ae0: 0a20 2020 2022 626f 7264 6572 5f77 6964  .    "border_wid
-00000af0: 7468 5f63 6865 636b 6564 223a 2036 2c0d  th_checked": 6,.
-00000b00: 0a20 2020 2022 626f 7264 6572 5f77 6964  .    "border_wid
-00000b10: 7468 5f75 6e63 6865 636b 6564 223a 2033  th_unchecked": 3
-00000b20: 2c0d 0a20 2020 2022 6667 5f63 6f6c 6f72  ,..    "fg_color
-00000b30: 223a 205b 2223 3342 3845 4430 222c 2022  ": ["#3B8ED0", "
-00000b40: 2331 4636 4141 3522 5d2c 0d0a 2020 2020  #1F6AA5"],..    
-00000b50: 2262 6f72 6465 725f 636f 6c6f 7222 3a20  "border_color": 
-00000b60: 5b22 2333 4534 3534 4122 2c20 2223 3934  ["#3E454A", "#94
-00000b70: 3941 3946 225d 2c0d 0a20 2020 2022 686f  9A9F"],..    "ho
-00000b80: 7665 725f 636f 6c6f 7222 3a20 5b22 2333  ver_color": ["#3
-00000b90: 3637 3139 4622 2c20 2223 3134 3438 3730  6719F", "#144870
-00000ba0: 225d 2c0d 0a20 2020 2022 7465 7874 5f63  "],..    "text_c
-00000bb0: 6f6c 6f72 223a 205b 2267 7261 7931 3022  olor": ["gray10"
-00000bc0: 2c20 2223 4443 4534 4545 225d 2c0d 0a20  , "#DCE4EE"],.. 
-00000bd0: 2020 2022 7465 7874 5f63 6f6c 6f72 5f64     "text_color_d
-00000be0: 6973 6162 6c65 6422 3a20 5b22 6772 6179  isabled": ["gray
-00000bf0: 3630 222c 2022 6772 6179 3435 225d 0d0a  60", "gray45"]..
-00000c00: 2020 7d2c 0d0a 2020 2243 546b 5072 6f67    },..  "CTkProg
-00000c10: 7265 7373 4261 7222 3a20 7b0d 0a20 2020  ressBar": {..   
-00000c20: 2022 636f 726e 6572 5f72 6164 6975 7322   "corner_radius"
-00000c30: 3a20 3130 3030 2c0d 0a20 2020 2022 626f  : 1000,..    "bo
-00000c40: 7264 6572 5f77 6964 7468 223a 2030 2c0d  rder_width": 0,.
-00000c50: 0a20 2020 2022 6667 5f63 6f6c 6f72 223a  .    "fg_color":
-00000c60: 205b 2223 3933 3942 4132 222c 2022 2334   ["#939BA2", "#4
-00000c70: 4134 4435 3022 5d2c 0d0a 2020 2020 2270  A4D50"],..    "p
-00000c80: 726f 6772 6573 735f 636f 6c6f 7222 3a20  rogress_color": 
-00000c90: 5b22 2333 4238 4544 3022 2c20 2223 3146  ["#3B8ED0", "#1F
-00000ca0: 3641 4135 225d 2c0d 0a20 2020 2022 626f  6AA5"],..    "bo
-00000cb0: 7264 6572 5f63 6f6c 6f72 223a 205b 2267  rder_color": ["g
-00000cc0: 7261 7922 2c20 2267 7261 7922 5d0d 0a20  ray", "gray"].. 
-00000cd0: 207d 2c0d 0a20 2022 4354 6b53 6c69 6465   },..  "CTkSlide
-00000ce0: 7222 3a20 7b0d 0a20 2020 2022 636f 726e  r": {..    "corn
-00000cf0: 6572 5f72 6164 6975 7322 3a20 3130 3030  er_radius": 1000
-00000d00: 2c0d 0a20 2020 2022 6275 7474 6f6e 5f63  ,..    "button_c
-00000d10: 6f72 6e65 725f 7261 6469 7573 223a 2031  orner_radius": 1
-00000d20: 3030 302c 0d0a 2020 2020 2262 6f72 6465  000,..    "borde
-00000d30: 725f 7769 6474 6822 3a20 362c 0d0a 2020  r_width": 6,..  
-00000d40: 2020 2262 7574 746f 6e5f 6c65 6e67 7468    "button_length
-00000d50: 223a 2030 2c0d 0a20 2020 2022 6667 5f63  ": 0,..    "fg_c
-00000d60: 6f6c 6f72 223a 205b 2223 3933 3942 4132  olor": ["#939BA2
-00000d70: 222c 2022 2334 4134 4435 3022 5d2c 0d0a  ", "#4A4D50"],..
-00000d80: 2020 2020 2270 726f 6772 6573 735f 636f      "progress_co
-00000d90: 6c6f 7222 3a20 5b22 6772 6179 3430 222c  lor": ["gray40",
-00000da0: 2022 2341 4142 3042 3522 5d2c 0d0a 2020   "#AAB0B5"],..  
-00000db0: 2020 2262 7574 746f 6e5f 636f 6c6f 7222    "button_color"
-00000dc0: 3a20 5b22 2333 4238 4544 3022 2c20 2223  : ["#3B8ED0", "#
-00000dd0: 3146 3641 4135 225d 2c0d 0a20 2020 2022  1F6AA5"],..    "
-00000de0: 6275 7474 6f6e 5f68 6f76 6572 5f63 6f6c  button_hover_col
-00000df0: 6f72 223a 205b 2223 3336 3731 3946 222c  or": ["#36719F",
-00000e00: 2022 2331 3434 3837 3022 5d0d 0a20 207d   "#144870"]..  }
-00000e10: 2c0d 0a20 2022 4354 6b4f 7074 696f 6e4d  ,..  "CTkOptionM
-00000e20: 656e 7522 3a20 7b0d 0a20 2020 2022 636f  enu": {..    "co
-00000e30: 726e 6572 5f72 6164 6975 7322 3a20 362c  rner_radius": 6,
-00000e40: 0d0a 2020 2020 2266 675f 636f 6c6f 7222  ..    "fg_color"
-00000e50: 3a20 5b22 2333 4238 4544 3022 2c20 2223  : ["#3B8ED0", "#
-00000e60: 3146 3641 4135 225d 2c0d 0a20 2020 2022  1F6AA5"],..    "
-00000e70: 6275 7474 6f6e 5f63 6f6c 6f72 223a 205b  button_color": [
-00000e80: 2223 3336 3731 3946 222c 2022 2331 3434  "#36719F", "#144
-00000e90: 3837 3022 5d2c 0d0a 2020 2020 2262 7574  870"],..    "but
-00000ea0: 746f 6e5f 686f 7665 725f 636f 6c6f 7222  ton_hover_color"
-00000eb0: 3a20 5b22 2332 3735 3737 4422 2c20 2223  : ["#27577D", "#
-00000ec0: 3230 3341 3446 225d 2c0d 0a20 2020 2022  203A4F"],..    "
-00000ed0: 7465 7874 5f63 6f6c 6f72 223a 205b 2223  text_color": ["#
-00000ee0: 4443 4534 4545 222c 2022 2344 4345 3445  DCE4EE", "#DCE4E
-00000ef0: 4522 5d2c 0d0a 2020 2020 2274 6578 745f  E"],..    "text_
-00000f00: 636f 6c6f 725f 6469 7361 626c 6564 223a  color_disabled":
-00000f10: 205b 2267 7261 7937 3422 2c20 2267 7261   ["gray74", "gra
-00000f20: 7936 3022 5d0d 0a20 207d 2c0d 0a20 2022  y60"]..  },..  "
-00000f30: 4354 6b43 6f6d 626f 426f 7822 3a20 7b0d  CTkComboBox": {.
-00000f40: 0a20 2020 2022 636f 726e 6572 5f72 6164  .    "corner_rad
-00000f50: 6975 7322 3a20 302c 0d0a 2020 2020 2262  ius": 0,..    "b
-00000f60: 6f72 6465 725f 7769 6474 6822 3a20 312c  order_width": 1,
-00000f70: 0d0a 2020 2020 2266 675f 636f 6c6f 7222  ..    "fg_color"
-00000f80: 3a20 5b22 2366 6666 6666 6622 2c20 2223  : ["#ffffff", "#
-00000f90: 3266 3266 3266 225d 2c0d 0a20 2020 2022  2f2f2f"],..    "
-00000fa0: 626f 7264 6572 5f63 6f6c 6f72 223a 205b  border_color": [
-00000fb0: 2223 6633 6633 6633 222c 2022 2339 3439  "#f3f3f3", "#949
-00000fc0: 4139 4622 5d2c 0d0a 2020 2020 2262 7574  A9F"],..    "but
-00000fd0: 746f 6e5f 636f 6c6f 7222 3a20 5b22 2366  ton_color": ["#f
-00000fe0: 3266 3266 3222 2c20 2223 3536 3542 3545  2f2f2", "#565B5E
-00000ff0: 225d 2c0d 0a20 2020 2022 6275 7474 6f6e  "],..    "button
-00001000: 5f68 6f76 6572 5f63 6f6c 6f72 223a 205b  _hover_color": [
-00001010: 2223 6632 6632 6632 222c 2022 2335 3635  "#f2f2f2", "#565
-00001020: 4235 4522 5d2c 0d0a 2020 2020 2274 6578  B5E"],..    "tex
-00001030: 745f 636f 6c6f 7222 3a20 5b22 6772 6179  t_color": ["gray
-00001040: 3130 222c 2022 2366 6666 6666 6622 5d2c  10", "#ffffff"],
-00001050: 0d0a 2020 2020 2274 6578 745f 636f 6c6f  ..    "text_colo
-00001060: 725f 6469 7361 626c 6564 223a 205b 2267  r_disabled": ["g
-00001070: 7261 7935 3022 2c20 2267 7261 7934 3522  ray50", "gray45"
-00001080: 5d0d 0a20 207d 2c0d 0a20 2022 4354 6b53  ]..  },..  "CTkS
-00001090: 6372 6f6c 6c62 6172 223a 207b 0d0a 2020  crollbar": {..  
-000010a0: 2020 2263 6f72 6e65 725f 7261 6469 7573    "corner_radius
-000010b0: 223a 2030 2c0d 0a20 2020 2022 626f 7264  ": 0,..    "bord
-000010c0: 6572 5f73 7061 6369 6e67 223a 2039 2c0d  er_spacing": 9,.
-000010d0: 0a20 2020 2022 6667 5f63 6f6c 6f72 223a  .    "fg_color":
-000010e0: 2022 7472 616e 7370 6172 656e 7422 2c0d   "transparent",.
-000010f0: 0a20 2020 2022 6275 7474 6f6e 5f63 6f6c  .    "button_col
-00001100: 6f72 223a 205b 2267 7261 7935 3522 2c20  or": ["gray55", 
-00001110: 2267 7261 7934 3122 5d2c 0d0a 2020 2020  "gray41"],..    
-00001120: 2262 7574 746f 6e5f 686f 7665 725f 636f  "button_hover_co
-00001130: 6c6f 7222 3a20 5b22 6772 6179 3430 222c  lor": ["gray40",
-00001140: 2022 6772 6179 3533 225d 0d0a 2020 7d2c   "gray53"]..  },
-00001150: 0d0a 2020 2243 546b 5365 676d 656e 7465  ..  "CTkSegmente
-00001160: 6442 7574 746f 6e22 3a20 7b0d 0a20 2020  dButton": {..   
-00001170: 2022 636f 726e 6572 5f72 6164 6975 7322   "corner_radius"
-00001180: 3a20 362c 0d0a 2020 2020 2262 6f72 6465  : 6,..    "borde
-00001190: 725f 7769 6474 6822 3a20 322c 0d0a 2020  r_width": 2,..  
-000011a0: 2020 2266 675f 636f 6c6f 7222 3a20 5b22    "fg_color": ["
-000011b0: 2339 3739 4441 3222 2c20 2267 7261 7932  #979DA2", "gray2
-000011c0: 3922 5d2c 0d0a 2020 2020 2273 656c 6563  9"],..    "selec
-000011d0: 7465 645f 636f 6c6f 7222 3a20 5b22 2333  ted_color": ["#3
-000011e0: 4238 4544 3022 2c20 2223 3146 3641 4135  B8ED0", "#1F6AA5
-000011f0: 225d 2c0d 0a20 2020 2022 7365 6c65 6374  "],..    "select
-00001200: 6564 5f68 6f76 6572 5f63 6f6c 6f72 223a  ed_hover_color":
-00001210: 205b 2223 3336 3731 3946 222c 2022 2331   ["#36719F", "#1
-00001220: 3434 3837 3022 5d2c 0d0a 2020 2020 2275  44870"],..    "u
-00001230: 6e73 656c 6563 7465 645f 636f 6c6f 7222  nselected_color"
-00001240: 3a20 5b22 2339 3739 4441 3222 2c20 2267  : ["#979DA2", "g
-00001250: 7261 7932 3922 5d2c 0d0a 2020 2020 2275  ray29"],..    "u
-00001260: 6e73 656c 6563 7465 645f 686f 7665 725f  nselected_hover_
-00001270: 636f 6c6f 7222 3a20 5b22 6772 6179 3730  color": ["gray70
-00001280: 222c 2022 6772 6179 3431 225d 2c0d 0a20  ", "gray41"],.. 
-00001290: 2020 2022 7465 7874 5f63 6f6c 6f72 223a     "text_color":
-000012a0: 205b 2223 4443 4534 4545 222c 2022 2344   ["#DCE4EE", "#D
-000012b0: 4345 3445 4522 5d2c 0d0a 2020 2020 2274  CE4EE"],..    "t
-000012c0: 6578 745f 636f 6c6f 725f 6469 7361 626c  ext_color_disabl
-000012d0: 6564 223a 205b 2267 7261 7937 3422 2c20  ed": ["gray74", 
-000012e0: 2267 7261 7936 3022 5d0d 0a20 207d 2c0d  "gray60"]..  },.
-000012f0: 0a20 2022 4354 6b54 6578 7462 6f78 223a  .  "CTkTextbox":
-00001300: 207b 0d0a 2020 2020 2263 6f72 6e65 725f   {..    "corner_
-00001310: 7261 6469 7573 223a 2030 2c0d 0a20 2020  radius": 0,..   
-00001320: 2022 626f 7264 6572 5f77 6964 7468 223a   "border_width":
-00001330: 2031 2c0d 0a20 2020 2022 6667 5f63 6f6c   1,..    "fg_col
-00001340: 6f72 223a 205b 2223 4639 4639 4641 222c  or": ["#F9F9FA",
-00001350: 2022 2331 4431 4531 4522 5d2c 0d0a 2020   "#1D1E1E"],..  
-00001360: 2020 2262 6f72 6465 725f 636f 6c6f 7222    "border_color"
-00001370: 3a20 5b22 2366 3366 3366 3322 2c20 2223  : ["#f3f3f3", "#
-00001380: 3934 3941 3946 225d 2c0d 0a20 2020 2022  949A9F"],..    "
-00001390: 7465 7874 5f63 6f6c 6f72 223a 5b22 6772  text_color":["gr
-000013a0: 6179 3130 222c 2022 2344 4345 3445 4522  ay10", "#DCE4EE"
-000013b0: 5d2c 0d0a 2020 2020 2273 6372 6f6c 6c62  ],..    "scrollb
-000013c0: 6172 5f62 7574 746f 6e5f 636f 6c6f 7222  ar_button_color"
-000013d0: 3a20 5b22 6772 6179 3535 222c 2022 6772  : ["gray55", "gr
-000013e0: 6179 3431 225d 2c0d 0a20 2020 2022 7363  ay41"],..    "sc
-000013f0: 726f 6c6c 6261 725f 6275 7474 6f6e 5f68  rollbar_button_h
-00001400: 6f76 6572 5f63 6f6c 6f72 223a 205b 2267  over_color": ["g
-00001410: 7261 7934 3022 2c20 2267 7261 7935 3322  ray40", "gray53"
-00001420: 5d0d 0a20 207d 2c0d 0a20 2022 4354 6b53  ]..  },..  "CTkS
-00001430: 6372 6f6c 6c61 626c 6546 7261 6d65 223a  crollableFrame":
-00001440: 207b 0d0a 2020 2020 226c 6162 656c 5f66   {..    "label_f
-00001450: 675f 636f 6c6f 7222 3a20 5b22 6772 6179  g_color": ["gray
-00001460: 3738 222c 2022 6772 6179 3233 225d 0d0a  78", "gray23"]..
-00001470: 2020 7d2c 0d0a 2020 2244 726f 7064 6f77    },..  "Dropdow
-00001480: 6e4d 656e 7522 3a20 7b0d 0a20 2020 2022  nMenu": {..    "
-00001490: 6667 5f63 6f6c 6f72 223a 205b 2267 7261  fg_color": ["gra
-000014a0: 7939 3022 2c20 2223 3163 3163 3163 225d  y90", "#1c1c1c"]
-000014b0: 2c0d 0a20 2020 2022 686f 7665 725f 636f  ,..    "hover_co
-000014c0: 6c6f 7222 3a20 5b22 6772 6179 3735 222c  lor": ["gray75",
-000014d0: 2022 2333 3133 3133 3122 5d2c 0d0a 2020   "#313131"],..  
-000014e0: 2020 2274 6578 745f 636f 6c6f 7222 3a20    "text_color": 
-000014f0: 5b22 6772 6179 3130 222c 2022 2366 6666  ["gray10", "#fff
-00001500: 6666 6622 5d0d 0a20 207d 2c0d 0a20 2022  fff"]..  },..  "
-00001510: 4354 6b46 6f6e 7422 3a20 7b0d 0a20 2020  CTkFont": {..   
-00001520: 2022 6d61 634f 5322 3a20 7b0d 0a20 2020   "macOS": {..   
-00001530: 2020 2022 6661 6d69 6c79 223a 2022 5346     "family": "SF
-00001540: 2044 6973 706c 6179 222c 0d0a 2020 2020   Display",..    
-00001550: 2020 2273 697a 6522 3a20 3133 2c0d 0a20    "size": 13,.. 
-00001560: 2020 2020 2022 7765 6967 6874 223a 2022       "weight": "
-00001570: 6e6f 726d 616c 220d 0a20 2020 207d 2c0d  normal"..    },.
-00001580: 0a20 2020 2022 5769 6e64 6f77 7322 3a20  .    "Windows": 
-00001590: 7b0d 0a20 2020 2020 2022 6661 6d69 6c79  {..      "family
-000015a0: 223a 2022 5365 676f 6520 5549 222c 0d0a  ": "Segoe UI",..
-000015b0: 2020 2020 2020 2273 697a 6522 3a20 3133        "size": 13
-000015c0: 2c0d 0a20 2020 2020 2022 7765 6967 6874  ,..      "weight
-000015d0: 223a 2022 6e6f 726d 616c 220d 0a20 2020  ": "normal"..   
-000015e0: 207d 2c0d 0a20 2020 2022 4c69 6e75 7822   },..    "Linux"
-000015f0: 3a20 7b0d 0a20 2020 2020 2022 6661 6d69  : {..      "fami
-00001600: 6c79 223a 2022 526f 626f 746f 222c 0d0a  ly": "Roboto",..
-00001610: 2020 2020 2020 2273 697a 6522 3a20 3133        "size": 13
-00001620: 2c0d 0a20 2020 2020 2022 7765 6967 6874  ,..      "weight
-00001630: 223a 2022 6e6f 726d 616c 220d 0a20 2020  ": "normal"..   
-00001640: 207d 0d0a 2020 7d0d 0a7d 0d0a 2222 220d   }..  }..}..""".
-00001650: 0a0d 0a0d 0a69 6d70 6f72 7420 6f73 2e70  .....import os.p
-00001660: 6174 680d 0a0d 0a0d 0a6f 6666 6963 6532  ath......office2
-00001670: 3031 395f 7061 7468 203d 206f 732e 7061  019_path = os.pa
-00001680: 7468 2e61 6273 7061 7468 286f 732e 7061  th.abspath(os.pa
-00001690: 7468 2e64 6972 6e61 6d65 285f 5f66 696c  th.dirname(__fil
-000016a0: 655f 5f29 292e 7265 706c 6163 6528 225c  e__)).replace("\
-000016b0: 5c22 2c20 222f 2229 202b 2022 2f4f 6666  \", "/") + "/Off
-000016c0: 6963 6532 3031 392e 6a73 6f6e 220d 0a0d  ice2019.json"...
-000016d0: 0a0d 0a64 6566 206f 6666 6963 6532 3031  ...def office201
-000016e0: 395f 7468 656d 6528 293a 0d0a 2020 2020  9_theme():..    
-000016f0: 6672 6f6d 2074 656d 7066 696c 6520 696d  from tempfile im
-00001700: 706f 7274 206d 6b73 7465 6d70 0d0a 2020  port mkstemp..  
-00001710: 2020 6672 6f6d 2063 7573 746f 6d74 6b69    from customtki
-00001720: 6e74 6572 2069 6d70 6f72 7420 7365 745f  nter import set_
-00001730: 6465 6661 756c 745f 636f 6c6f 725f 7468  default_color_th
-00001740: 656d 650d 0a20 2020 205f 2c20 5f5f 7465  eme..    _, __te
-00001750: 6d70 203d 206d 6b73 7465 6d70 2873 7566  mp = mkstemp(suf
-00001760: 6669 783d 222e 6a73 6f6e 2229 0d0a 2020  fix=".json")..  
-00001770: 2020 7769 7468 206f 7065 6e28 5f5f 7465    with open(__te
-00001780: 6d70 2c20 2277 2229 2061 7320 5f5f 7465  mp, "w") as __te
-00001790: 6d70 5f66 696c 653a 0d0a 2020 2020 2020  mp_file:..      
-000017a0: 2020 5f5f 7465 6d70 5f66 696c 652e 7772    __temp_file.wr
-000017b0: 6974 6528 6f66 6669 6365 3230 3139 5f6a  ite(office2019_j
-000017c0: 736f 6e29 0d0a 2020 2020 7265 7475 726e  son)..    return
-000017d0: 205f 5f74 656d 700d 0a0d 0a0d 0a64 6566   __temp......def
-000017e0: 2075 7365 5f6f 6666 6963 6532 3031 395f   use_office2019_
-000017f0: 7468 656d 6528 293a 0d0a 2020 2020 6672  theme():..    fr
-00001800: 6f6d 2063 7573 746f 6d74 6b69 6e74 6572  om customtkinter
-00001810: 2069 6d70 6f72 7420 7365 745f 6465 6661   import set_defa
-00001820: 756c 745f 636f 6c6f 725f 7468 656d 650d  ult_color_theme.
-00001830: 0a20 2020 2074 7279 3a0d 0a20 2020 2020  .    try:..     
-00001840: 2020 2073 6574 5f64 6566 6175 6c74 5f63     set_default_c
-00001850: 6f6c 6f72 5f74 6865 6d65 286f 6666 6963  olor_theme(offic
-00001860: 6532 3031 395f 7061 7468 290d 0a20 2020  e2019_path)..   
-00001870: 2065 7863 6570 7420 4669 6c65 4e6f 7446   except FileNotF
-00001880: 6f75 6e64 4572 726f 723a 0d0a 2020 2020  oundError:..    
-00001890: 2020 2020 7365 745f 6465 6661 756c 745f      set_default_
-000018a0: 636f 6c6f 725f 7468 656d 6528 6f66 6669  color_theme(offi
-000018b0: 6365 3230 3139 5f74 6865 6d65 2829 290d  ce2019_theme()).
-000018c0: 0a                                       .
+00000000: 7b0d 0a20 2022 4354 6b43 7573 746f 6d22  {..  "CTkCustom"
+00000010: 3a20 7b0d 0a20 2020 2022 7469 746c 6562  : {..    "titleb
+00000020: 6172 5f63 6f6c 6f72 223a 205b 2223 3130  ar_color": ["#10
+00000030: 3665 6265 222c 2022 2331 3036 6562 6522  6ebe", "#106ebe"
+00000040: 5d2c 0d0a 2020 2020 2274 6974 6c65 5f63  ],..    "title_c
+00000050: 6f6c 6f72 223a 205b 2223 6666 6666 6666  olor": ["#ffffff
+00000060: 222c 2022 2366 6666 6666 6622 5d2c 0d0a  ", "#ffffff"],..
+00000070: 0d0a 2020 2020 2274 7261 6e73 7061 7265  ..    "transpare
+00000080: 6e74 5f63 6f6c 6f72 223a 2022 2331 3031  nt_color": "#101
+00000090: 3031 3022 2c0d 0a0d 0a20 2020 2022 636c  010",....    "cl
+000000a0: 6f73 6562 7574 746f 6e5f 7465 7874 5f63  osebutton_text_c
+000000b0: 6f6c 6f72 223a 205b 2223 3030 3030 3030  olor": ["#000000
+000000c0: 222c 2022 2366 6666 6666 6622 5d2c 0d0a  ", "#ffffff"],..
+000000d0: 2020 2020 2263 6c6f 7365 6275 7474 6f6e      "closebutton
+000000e0: 5f63 6f6c 6f72 223a 205b 2223 6666 6666  _color": ["#ffff
+000000f0: 6666 222c 2022 2332 6332 6332 6322 5d2c  ff", "#2c2c2c"],
+00000100: 0d0a 2020 2020 2263 6c6f 7365 6275 7474  ..    "closebutt
+00000110: 6f6e 5f68 6f76 6572 5f63 6f6c 6f72 223a  on_hover_color":
+00000120: 205b 2223 6234 3064 3162 222c 2022 2362   ["#b40d1b", "#b
+00000130: 3430 6431 6222 5d2c 0d0a 0d0a 2020 2020  40d1b"],....    
+00000140: 226d 696e 696d 697a 6562 7574 746f 6e5f  "minimizebutton_
+00000150: 7465 7874 5f63 6f6c 6f72 223a 205b 2223  text_color": ["#
+00000160: 3030 3030 3030 222c 2022 2366 6666 6666  000000", "#fffff
+00000170: 6622 5d2c 0d0a 2020 2020 226d 696e 696d  f"],..    "minim
+00000180: 697a 6562 7574 746f 6e5f 636f 6c6f 7222  izebutton_color"
+00000190: 3a20 5b22 2366 6666 6666 6622 2c20 2223  : ["#ffffff", "#
+000001a0: 3263 3263 3263 225d 2c0d 0a20 2020 2022  2c2c2c"],..    "
+000001b0: 6d69 6e69 6d69 7a65 6275 7474 6f6e 5f68  minimizebutton_h
+000001c0: 6f76 6572 5f63 6f6c 6f72 223a 205b 2223  over_color": ["#
+000001d0: 6363 6363 6363 222c 2022 2332 3832 3832  cccccc", "#28282
+000001e0: 3822 5d0d 0a20 207d 2c0d 0a20 2022 4354  8"]..  },..  "CT
+000001f0: 6b49 6e66 6f42 6172 223a 207b 0d0a 2020  kInfoBar": {..  
+00000200: 2020 2263 6f72 6e65 725f 7261 6469 7573    "corner_radius
+00000210: 223a 2038 2c0d 0a20 2020 2022 626f 7264  ": 8,..    "bord
+00000220: 6572 5f77 6964 7468 223a 2030 2c0d 0a0d  er_width": 0,...
+00000230: 0a20 2020 2022 6667 5f63 6f6c 6f72 223a  .    "fg_color":
+00000240: 205b 2223 6637 6637 6637 222c 2022 2332   ["#f7f7f7", "#2
+00000250: 6632 6632 6622 5d2c 0d0a 2020 2020 2266  f2f2f"],..    "f
+00000260: 675f 686f 7665 725f 636f 6c6f 7222 3a20  g_hover_color": 
+00000270: 5b22 2363 3363 3363 3322 2c20 2223 3535  ["#c3c3c3", "#55
+00000280: 3535 3535 225d 2c0d 0a0d 0a20 2020 2022  5555"],....    "
+00000290: 626f 7264 6572 5f63 6f6c 6f72 223a 205b  border_color": [
+000002a0: 2223 6230 6232 6232 222c 2022 2334 3234  "#b0b2b2", "#424
+000002b0: 3535 3622 5d2c 0d0a 0d0a 2020 2020 2273  556"],....    "s
+000002c0: 7563 6365 7373 5f63 6f6c 6f72 223a 205b  uccess_color": [
+000002d0: 2223 6466 6636 6464 222c 2022 2333 3933  "#dff6dd", "#393
+000002e0: 6431 6222 5d2c 0d0a 2020 2020 2273 7563  d1b"],..    "suc
+000002f0: 6365 7373 5f68 6f76 6572 5f63 6f6c 6f72  cess_hover_color
+00000300: 223a 205b 2223 6230 6333 6166 222c 2022  ": ["#b0c3af", "
+00000310: 2335 6336 3332 6222 5d2c 0d0a 2020 2020  #5c632b"],..    
+00000320: 2263 6175 7469 6f6e 5f63 6f6c 6f72 223a  "caution_color":
+00000330: 205b 2223 6666 6634 6365 222c 2022 2334   ["#fff4ce", "#4
+00000340: 3333 3531 3922 5d2c 0d0a 2020 2020 2263  33519"],..    "c
+00000350: 6175 7469 6f6e 5f68 6f76 6572 5f63 6f6c  aution_hover_col
+00000360: 6f72 223a 205b 2223 6363 6333 6134 222c  or": ["#ccc3a4",
+00000370: 2022 2336 3935 3332 3722 5d2c 0d0a 2020   "#695327"],..  
+00000380: 2020 2263 7269 7469 6361 6c5f 636f 6c6f    "critical_colo
+00000390: 7222 3a20 5b22 2366 6465 3765 3922 2c20  r": ["#fde7e9", 
+000003a0: 2223 3434 3237 3236 225d 2c0d 0a20 2020  "#442726"],..   
+000003b0: 2022 6372 6974 6963 616c 5f68 6f76 6572   "critical_hover
+000003c0: 5f63 6f6c 6f72 223a 205b 2223 6361 6238  _color": ["#cab8
+000003d0: 6261 222c 2022 2336 6133 6333 6222 5d0d  ba", "#6a3c3b"].
+000003e0: 0a0d 0a20 207d 2c0d 0a20 2022 4354 6b22  ...  },..  "CTk"
+000003f0: 3a20 7b0d 0a20 2020 2022 6667 5f63 6f6c  : {..    "fg_col
+00000400: 6f72 223a 205b 2223 6666 6666 6666 222c  or": ["#ffffff",
+00000410: 2022 2331 3031 3031 3022 5d0d 0a20 207d   "#101010"]..  }
+00000420: 2c0d 0a20 2022 4354 6b54 6f70 6c65 7665  ,..  "CTkTopleve
+00000430: 6c22 3a20 7b0d 0a20 2020 2022 6667 5f63  l": {..    "fg_c
+00000440: 6f6c 6f72 223a 205b 2223 6666 6666 6666  olor": ["#ffffff
+00000450: 222c 2022 2331 3031 3031 3022 5d0d 0a20  ", "#101010"].. 
+00000460: 207d 2c0d 0a20 2022 4354 6b46 7261 6d65   },..  "CTkFrame
+00000470: 223a 207b 0d0a 2020 2020 2263 6f72 6e65  ": {..    "corne
+00000480: 725f 7261 6469 7573 223a 2030 2c0d 0a20  r_radius": 0,.. 
+00000490: 2020 2022 626f 7264 6572 5f77 6964 7468     "border_width
+000004a0: 223a 2031 2c0d 0a20 2020 2022 6667 5f63  ": 1,..    "fg_c
+000004b0: 6f6c 6f72 223a 205b 2223 6666 6666 6666  olor": ["#ffffff
+000004c0: 222c 2022 2331 6331 6331 6322 5d2c 0d0a  ", "#1c1c1c"],..
+000004d0: 2020 2020 2274 6f70 5f66 675f 636f 6c6f      "top_fg_colo
+000004e0: 7222 3a20 5b22 2366 6666 6666 6622 2c20  r": ["#ffffff", 
+000004f0: 2223 3263 3263 3263 225d 2c0d 0a20 2020  "#2c2c2c"],..   
+00000500: 2022 626f 7264 6572 5f63 6f6c 6f72 223a   "border_color":
+00000510: 205b 2223 6230 6232 6232 222c 2022 2334   ["#b0b2b2", "#4
+00000520: 3234 3535 3622 5d0d 0a20 207d 2c0d 0a20  24556"]..  },.. 
+00000530: 2022 4354 6b42 7574 746f 6e22 3a20 7b0d   "CTkButton": {.
+00000540: 0a20 2020 2022 636f 726e 6572 5f72 6164  .    "corner_rad
+00000550: 6975 7322 3a20 302c 0d0a 2020 2020 2262  ius": 0,..    "b
+00000560: 6f72 6465 725f 7769 6474 6822 3a20 312c  order_width": 1,
+00000570: 0d0a 2020 2020 2266 675f 636f 6c6f 7222  ..    "fg_color"
+00000580: 3a20 5b22 2365 3565 3565 3522 2c20 2223  : ["#e5e5e5", "#
+00000590: 3364 3364 3364 225d 2c0d 0a20 2020 2022  3d3d3d"],..    "
+000005a0: 686f 7665 725f 636f 6c6f 7222 3a20 5b22  hover_color": ["
+000005b0: 2362 3262 3262 3222 2c20 2223 3135 3135  #b2b2b2", "#1515
+000005c0: 3135 225d 2c0d 0a20 2020 2022 626f 7264  15"],..    "bord
+000005d0: 6572 5f63 6f6c 6f72 223a 205b 2223 6633  er_color": ["#f3
+000005e0: 6633 6633 222c 2022 2339 3439 4139 4622  f3f3", "#949A9F"
+000005f0: 5d2c 0d0a 2020 2020 2274 6578 745f 636f  ],..    "text_co
+00000600: 6c6f 7222 3a20 5b22 2330 3030 3030 3022  lor": ["#000000"
+00000610: 2c20 2223 6666 6666 6666 225d 2c0d 0a20  , "#ffffff"],.. 
+00000620: 2020 2022 7465 7874 5f63 6f6c 6f72 5f64     "text_color_d
+00000630: 6973 6162 6c65 6422 3a20 5b22 6772 6179  isabled": ["gray
+00000640: 3734 222c 2022 6772 6179 3630 225d 0d0a  74", "gray60"]..
+00000650: 2020 7d2c 0d0a 2020 2243 546b 4c61 6265    },..  "CTkLabe
+00000660: 6c22 3a20 7b0d 0a20 2020 2022 636f 726e  l": {..    "corn
+00000670: 6572 5f72 6164 6975 7322 3a20 302c 0d0a  er_radius": 0,..
+00000680: 2020 2020 2266 675f 636f 6c6f 7222 3a20      "fg_color": 
+00000690: 2274 7261 6e73 7061 7265 6e74 222c 0d0a  "transparent",..
+000006a0: 2020 2020 2274 6578 745f 636f 6c6f 7222      "text_color"
+000006b0: 3a20 5b22 6772 6179 3130 222c 2022 2344  : ["gray10", "#D
+000006c0: 4345 3445 4522 5d0d 0a20 207d 2c0d 0a20  CE4EE"]..  },.. 
+000006d0: 2022 4354 6b45 6e74 7279 223a 207b 0d0a   "CTkEntry": {..
+000006e0: 2020 2020 2263 6f72 6e65 725f 7261 6469      "corner_radi
+000006f0: 7573 223a 2030 2c0d 0a20 2020 2022 626f  us": 0,..    "bo
+00000700: 7264 6572 5f77 6964 7468 223a 2031 2c0d  rder_width": 1,.
+00000710: 0a20 2020 2022 6667 5f63 6f6c 6f72 223a  .    "fg_color":
+00000720: 205b 2223 6666 6666 6666 222c 2022 2332   ["#ffffff", "#2
+00000730: 6632 6632 6622 5d2c 0d0a 2020 2020 2262  f2f2f"],..    "b
+00000740: 6f72 6465 725f 636f 6c6f 7222 3a20 5b22  order_color": ["
+00000750: 2366 3366 3366 3322 2c20 2223 3934 3941  #f3f3f3", "#949A
+00000760: 3946 225d 2c0d 0a20 2020 2022 7465 7874  9F"],..    "text
+00000770: 5f63 6f6c 6f72 223a 5b22 2330 3030 3030  _color":["#00000
+00000780: 3022 2c20 2223 6666 6666 6666 225d 2c0d  0", "#ffffff"],.
+00000790: 0a20 2020 2022 706c 6163 6568 6f6c 6465  .    "placeholde
+000007a0: 725f 7465 7874 5f63 6f6c 6f72 223a 205b  r_text_color": [
+000007b0: 2267 7261 7935 3222 2c20 2267 7261 7936  "gray52", "gray6
+000007c0: 3222 5d0d 0a20 207d 2c0d 0a20 2022 4354  2"]..  },..  "CT
+000007d0: 6b43 6865 636b 626f 7822 3a20 7b0d 0a20  kCheckbox": {.. 
+000007e0: 2020 2022 636f 726e 6572 5f72 6164 6975     "corner_radiu
+000007f0: 7322 3a20 362c 0d0a 2020 2020 2262 6f72  s": 6,..    "bor
+00000800: 6465 725f 7769 6474 6822 3a20 332c 0d0a  der_width": 3,..
+00000810: 2020 2020 2266 675f 636f 6c6f 7222 3a20      "fg_color": 
+00000820: 5b22 2333 4238 4544 3022 2c20 2223 3146  ["#3B8ED0", "#1F
+00000830: 3641 4135 225d 2c0d 0a20 2020 2022 626f  6AA5"],..    "bo
+00000840: 7264 6572 5f63 6f6c 6f72 223a 205b 2223  rder_color": ["#
+00000850: 3345 3435 3441 222c 2022 2339 3439 4139  3E454A", "#949A9
+00000860: 4622 5d2c 0d0a 2020 2020 2268 6f76 6572  F"],..    "hover
+00000870: 5f63 6f6c 6f72 223a 205b 2223 3342 3845  _color": ["#3B8E
+00000880: 4430 222c 2022 2331 4636 4141 3522 5d2c  D0", "#1F6AA5"],
+00000890: 0d0a 2020 2020 2263 6865 636b 6d61 726b  ..    "checkmark
+000008a0: 5f63 6f6c 6f72 223a 205b 2223 4443 4534  _color": ["#DCE4
+000008b0: 4545 222c 2022 6772 6179 3930 225d 2c0d  EE", "gray90"],.
+000008c0: 0a20 2020 2022 7465 7874 5f63 6f6c 6f72  .    "text_color
+000008d0: 223a 205b 2267 7261 7931 3022 2c20 2223  ": ["gray10", "#
+000008e0: 4443 4534 4545 225d 2c0d 0a20 2020 2022  DCE4EE"],..    "
+000008f0: 7465 7874 5f63 6f6c 6f72 5f64 6973 6162  text_color_disab
+00000900: 6c65 6422 3a20 5b22 6772 6179 3630 222c  led": ["gray60",
+00000910: 2022 6772 6179 3435 225d 0d0a 2020 7d2c   "gray45"]..  },
+00000920: 0d0a 2020 2243 546b 5377 6974 6368 223a  ..  "CTkSwitch":
+00000930: 207b 0d0a 2020 2020 2263 6f72 6e65 725f   {..    "corner_
+00000940: 7261 6469 7573 223a 2038 2c0d 0a20 2020  radius": 8,..   
+00000950: 2022 626f 7264 6572 5f77 6964 7468 223a   "border_width":
+00000960: 2031 2c0d 0a20 2020 2022 6275 7474 6f6e   1,..    "button
+00000970: 5f6c 656e 6774 6822 3a20 322c 0d0a 2020  _length": 2,..  
+00000980: 2020 2266 675f 636f 6c6f 7222 3a20 5b22    "fg_color": ["
+00000990: 2365 6465 6465 6422 2c20 2223 3164 3164  #ededed", "#1d1d
+000009a0: 3164 225d 2c0d 0a20 2020 2022 7072 6f67  1d"],..    "prog
+000009b0: 7265 7373 5f63 6f6c 6f72 223a 205b 2223  ress_color": ["#
+000009c0: 3030 3637 6330 222c 2022 2334 6363 3266  0067c0", "#4cc2f
+000009d0: 6622 5d2c 0d0a 2020 2020 2262 7574 746f  f"],..    "butto
+000009e0: 6e5f 636f 6c6f 7222 3a20 5b22 2366 3366  n_color": ["#f3f
+000009f0: 3366 3322 2c20 2223 3030 3030 3030 225d  3f3", "#000000"]
+00000a00: 2c0d 0a20 2020 2022 6275 7474 6f6e 5f68  ,..    "button_h
+00000a10: 6f76 6572 5f63 6f6c 6f72 223a 205b 2223  over_color": ["#
+00000a20: 6266 6266 6266 222c 2022 2330 3530 3530  bfbfbf", "#05050
+00000a30: 3522 5d2c 0d0a 2020 2020 2274 6578 745f  5"],..    "text_
+00000a40: 636f 6c6f 7222 3a20 5b22 6772 6179 3130  color": ["gray10
+00000a50: 222c 2022 2344 4345 3445 4522 5d2c 0d0a  ", "#DCE4EE"],..
+00000a60: 2020 2020 2274 6578 745f 636f 6c6f 725f      "text_color_
+00000a70: 6469 7361 626c 6564 223a 205b 2267 7261  disabled": ["gra
+00000a80: 7936 3022 2c20 2267 7261 7934 3522 5d0d  y60", "gray45"].
+00000a90: 0a20 207d 2c0d 0a20 2022 4354 6b52 6164  .  },..  "CTkRad
+00000aa0: 696f 6275 7474 6f6e 223a 207b 0d0a 2020  iobutton": {..  
+00000ab0: 2020 2263 6f72 6e65 725f 7261 6469 7573    "corner_radius
+00000ac0: 223a 2031 3030 302c 0d0a 2020 2020 2262  ": 1000,..    "b
+00000ad0: 6f72 6465 725f 7769 6474 685f 6368 6563  order_width_chec
+00000ae0: 6b65 6422 3a20 362c 0d0a 2020 2020 2262  ked": 6,..    "b
+00000af0: 6f72 6465 725f 7769 6474 685f 756e 6368  order_width_unch
+00000b00: 6563 6b65 6422 3a20 332c 0d0a 2020 2020  ecked": 3,..    
+00000b10: 2266 675f 636f 6c6f 7222 3a20 5b22 2333  "fg_color": ["#3
+00000b20: 4238 4544 3022 2c20 2223 3146 3641 4135  B8ED0", "#1F6AA5
+00000b30: 225d 2c0d 0a20 2020 2022 626f 7264 6572  "],..    "border
+00000b40: 5f63 6f6c 6f72 223a 205b 2223 3345 3435  _color": ["#3E45
+00000b50: 3441 222c 2022 2339 3439 4139 4622 5d2c  4A", "#949A9F"],
+00000b60: 0d0a 2020 2020 2268 6f76 6572 5f63 6f6c  ..    "hover_col
+00000b70: 6f72 223a 205b 2223 3336 3731 3946 222c  or": ["#36719F",
+00000b80: 2022 2331 3434 3837 3022 5d2c 0d0a 2020   "#144870"],..  
+00000b90: 2020 2274 6578 745f 636f 6c6f 7222 3a20    "text_color": 
+00000ba0: 5b22 6772 6179 3130 222c 2022 2344 4345  ["gray10", "#DCE
+00000bb0: 3445 4522 5d2c 0d0a 2020 2020 2274 6578  4EE"],..    "tex
+00000bc0: 745f 636f 6c6f 725f 6469 7361 626c 6564  t_color_disabled
+00000bd0: 223a 205b 2267 7261 7936 3022 2c20 2267  ": ["gray60", "g
+00000be0: 7261 7934 3522 5d0d 0a20 207d 2c0d 0a20  ray45"]..  },.. 
+00000bf0: 2022 4354 6b50 726f 6772 6573 7342 6172   "CTkProgressBar
+00000c00: 223a 207b 0d0a 2020 2020 2263 6f72 6e65  ": {..    "corne
+00000c10: 725f 7261 6469 7573 223a 2031 3030 302c  r_radius": 1000,
+00000c20: 0d0a 2020 2020 2262 6f72 6465 725f 7769  ..    "border_wi
+00000c30: 6474 6822 3a20 302c 0d0a 2020 2020 2266  dth": 0,..    "f
+00000c40: 675f 636f 6c6f 7222 3a20 5b22 2339 3339  g_color": ["#939
+00000c50: 4241 3222 2c20 2223 3441 3444 3530 225d  BA2", "#4A4D50"]
+00000c60: 2c0d 0a20 2020 2022 7072 6f67 7265 7373  ,..    "progress
+00000c70: 5f63 6f6c 6f72 223a 205b 2223 3342 3845  _color": ["#3B8E
+00000c80: 4430 222c 2022 2331 4636 4141 3522 5d2c  D0", "#1F6AA5"],
+00000c90: 0d0a 2020 2020 2262 6f72 6465 725f 636f  ..    "border_co
+00000ca0: 6c6f 7222 3a20 5b22 6772 6179 222c 2022  lor": ["gray", "
+00000cb0: 6772 6179 225d 0d0a 2020 7d2c 0d0a 2020  gray"]..  },..  
+00000cc0: 2243 546b 536c 6964 6572 223a 207b 0d0a  "CTkSlider": {..
+00000cd0: 2020 2020 2263 6f72 6e65 725f 7261 6469      "corner_radi
+00000ce0: 7573 223a 2031 3030 302c 0d0a 2020 2020  us": 1000,..    
+00000cf0: 2262 7574 746f 6e5f 636f 726e 6572 5f72  "button_corner_r
+00000d00: 6164 6975 7322 3a20 3130 3030 2c0d 0a20  adius": 1000,.. 
+00000d10: 2020 2022 626f 7264 6572 5f77 6964 7468     "border_width
+00000d20: 223a 2036 2c0d 0a20 2020 2022 6275 7474  ": 6,..    "butt
+00000d30: 6f6e 5f6c 656e 6774 6822 3a20 302c 0d0a  on_length": 0,..
+00000d40: 2020 2020 2266 675f 636f 6c6f 7222 3a20      "fg_color": 
+00000d50: 5b22 2339 3339 4241 3222 2c20 2223 3441  ["#939BA2", "#4A
+00000d60: 3444 3530 225d 2c0d 0a20 2020 2022 7072  4D50"],..    "pr
+00000d70: 6f67 7265 7373 5f63 6f6c 6f72 223a 205b  ogress_color": [
+00000d80: 2267 7261 7934 3022 2c20 2223 4141 4230  "gray40", "#AAB0
+00000d90: 4235 225d 2c0d 0a20 2020 2022 6275 7474  B5"],..    "butt
+00000da0: 6f6e 5f63 6f6c 6f72 223a 205b 2223 3342  on_color": ["#3B
+00000db0: 3845 4430 222c 2022 2331 4636 4141 3522  8ED0", "#1F6AA5"
+00000dc0: 5d2c 0d0a 2020 2020 2262 7574 746f 6e5f  ],..    "button_
+00000dd0: 686f 7665 725f 636f 6c6f 7222 3a20 5b22  hover_color": ["
+00000de0: 2333 3637 3139 4622 2c20 2223 3134 3438  #36719F", "#1448
+00000df0: 3730 225d 0d0a 2020 7d2c 0d0a 2020 2243  70"]..  },..  "C
+00000e00: 546b 4f70 7469 6f6e 4d65 6e75 223a 207b  TkOptionMenu": {
+00000e10: 0d0a 2020 2020 2263 6f72 6e65 725f 7261  ..    "corner_ra
+00000e20: 6469 7573 223a 2036 2c0d 0a20 2020 2022  dius": 6,..    "
+00000e30: 6667 5f63 6f6c 6f72 223a 205b 2223 3342  fg_color": ["#3B
+00000e40: 3845 4430 222c 2022 2331 4636 4141 3522  8ED0", "#1F6AA5"
+00000e50: 5d2c 0d0a 2020 2020 2262 7574 746f 6e5f  ],..    "button_
+00000e60: 636f 6c6f 7222 3a20 5b22 2333 3637 3139  color": ["#36719
+00000e70: 4622 2c20 2223 3134 3438 3730 225d 2c0d  F", "#144870"],.
+00000e80: 0a20 2020 2022 6275 7474 6f6e 5f68 6f76  .    "button_hov
+00000e90: 6572 5f63 6f6c 6f72 223a 205b 2223 3237  er_color": ["#27
+00000ea0: 3537 3744 222c 2022 2332 3033 4134 4622  577D", "#203A4F"
+00000eb0: 5d2c 0d0a 2020 2020 2274 6578 745f 636f  ],..    "text_co
+00000ec0: 6c6f 7222 3a20 5b22 2344 4345 3445 4522  lor": ["#DCE4EE"
+00000ed0: 2c20 2223 4443 4534 4545 225d 2c0d 0a20  , "#DCE4EE"],.. 
+00000ee0: 2020 2022 7465 7874 5f63 6f6c 6f72 5f64     "text_color_d
+00000ef0: 6973 6162 6c65 6422 3a20 5b22 6772 6179  isabled": ["gray
+00000f00: 3734 222c 2022 6772 6179 3630 225d 0d0a  74", "gray60"]..
+00000f10: 2020 7d2c 0d0a 2020 2243 546b 436f 6d62    },..  "CTkComb
+00000f20: 6f42 6f78 223a 207b 0d0a 2020 2020 2263  oBox": {..    "c
+00000f30: 6f72 6e65 725f 7261 6469 7573 223a 2030  orner_radius": 0
+00000f40: 2c0d 0a20 2020 2022 626f 7264 6572 5f77  ,..    "border_w
+00000f50: 6964 7468 223a 2031 2c0d 0a20 2020 2022  idth": 1,..    "
+00000f60: 6667 5f63 6f6c 6f72 223a 205b 2223 6666  fg_color": ["#ff
+00000f70: 6666 6666 222c 2022 2332 6632 6632 6622  ffff", "#2f2f2f"
+00000f80: 5d2c 0d0a 2020 2020 2262 6f72 6465 725f  ],..    "border_
+00000f90: 636f 6c6f 7222 3a20 5b22 2366 3366 3366  color": ["#f3f3f
+00000fa0: 3322 2c20 2223 3934 3941 3946 225d 2c0d  3", "#949A9F"],.
+00000fb0: 0a20 2020 2022 6275 7474 6f6e 5f63 6f6c  .    "button_col
+00000fc0: 6f72 223a 205b 2223 6632 6632 6632 222c  or": ["#f2f2f2",
+00000fd0: 2022 2335 3635 4235 4522 5d2c 0d0a 2020   "#565B5E"],..  
+00000fe0: 2020 2262 7574 746f 6e5f 686f 7665 725f    "button_hover_
+00000ff0: 636f 6c6f 7222 3a20 5b22 2366 3266 3266  color": ["#f2f2f
+00001000: 3222 2c20 2223 3536 3542 3545 225d 2c0d  2", "#565B5E"],.
+00001010: 0a20 2020 2022 7465 7874 5f63 6f6c 6f72  .    "text_color
+00001020: 223a 205b 2267 7261 7931 3022 2c20 2223  ": ["gray10", "#
+00001030: 6666 6666 6666 225d 2c0d 0a20 2020 2022  ffffff"],..    "
+00001040: 7465 7874 5f63 6f6c 6f72 5f64 6973 6162  text_color_disab
+00001050: 6c65 6422 3a20 5b22 6772 6179 3530 222c  led": ["gray50",
+00001060: 2022 6772 6179 3435 225d 0d0a 2020 7d2c   "gray45"]..  },
+00001070: 0d0a 2020 2243 546b 5363 726f 6c6c 6261  ..  "CTkScrollba
+00001080: 7222 3a20 7b0d 0a20 2020 2022 636f 726e  r": {..    "corn
+00001090: 6572 5f72 6164 6975 7322 3a20 302c 0d0a  er_radius": 0,..
+000010a0: 2020 2020 2262 6f72 6465 725f 7370 6163      "border_spac
+000010b0: 696e 6722 3a20 392c 0d0a 2020 2020 2266  ing": 9,..    "f
+000010c0: 675f 636f 6c6f 7222 3a20 2274 7261 6e73  g_color": "trans
+000010d0: 7061 7265 6e74 222c 0d0a 2020 2020 2262  parent",..    "b
+000010e0: 7574 746f 6e5f 636f 6c6f 7222 3a20 5b22  utton_color": ["
+000010f0: 6772 6179 3535 222c 2022 6772 6179 3431  gray55", "gray41
+00001100: 225d 2c0d 0a20 2020 2022 6275 7474 6f6e  "],..    "button
+00001110: 5f68 6f76 6572 5f63 6f6c 6f72 223a 205b  _hover_color": [
+00001120: 2267 7261 7934 3022 2c20 2267 7261 7935  "gray40", "gray5
+00001130: 3322 5d0d 0a20 207d 2c0d 0a20 2022 4354  3"]..  },..  "CT
+00001140: 6b53 6567 6d65 6e74 6564 4275 7474 6f6e  kSegmentedButton
+00001150: 223a 207b 0d0a 2020 2020 2263 6f72 6e65  ": {..    "corne
+00001160: 725f 7261 6469 7573 223a 2036 2c0d 0a20  r_radius": 6,.. 
+00001170: 2020 2022 626f 7264 6572 5f77 6964 7468     "border_width
+00001180: 223a 2032 2c0d 0a20 2020 2022 6667 5f63  ": 2,..    "fg_c
+00001190: 6f6c 6f72 223a 205b 2223 3937 3944 4132  olor": ["#979DA2
+000011a0: 222c 2022 6772 6179 3239 225d 2c0d 0a20  ", "gray29"],.. 
+000011b0: 2020 2022 7365 6c65 6374 6564 5f63 6f6c     "selected_col
+000011c0: 6f72 223a 205b 2223 3342 3845 4430 222c  or": ["#3B8ED0",
+000011d0: 2022 2331 4636 4141 3522 5d2c 0d0a 2020   "#1F6AA5"],..  
+000011e0: 2020 2273 656c 6563 7465 645f 686f 7665    "selected_hove
+000011f0: 725f 636f 6c6f 7222 3a20 5b22 2333 3637  r_color": ["#367
+00001200: 3139 4622 2c20 2223 3134 3438 3730 225d  19F", "#144870"]
+00001210: 2c0d 0a20 2020 2022 756e 7365 6c65 6374  ,..    "unselect
+00001220: 6564 5f63 6f6c 6f72 223a 205b 2223 3937  ed_color": ["#97
+00001230: 3944 4132 222c 2022 6772 6179 3239 225d  9DA2", "gray29"]
+00001240: 2c0d 0a20 2020 2022 756e 7365 6c65 6374  ,..    "unselect
+00001250: 6564 5f68 6f76 6572 5f63 6f6c 6f72 223a  ed_hover_color":
+00001260: 205b 2267 7261 7937 3022 2c20 2267 7261   ["gray70", "gra
+00001270: 7934 3122 5d2c 0d0a 2020 2020 2274 6578  y41"],..    "tex
+00001280: 745f 636f 6c6f 7222 3a20 5b22 2344 4345  t_color": ["#DCE
+00001290: 3445 4522 2c20 2223 4443 4534 4545 225d  4EE", "#DCE4EE"]
+000012a0: 2c0d 0a20 2020 2022 7465 7874 5f63 6f6c  ,..    "text_col
+000012b0: 6f72 5f64 6973 6162 6c65 6422 3a20 5b22  or_disabled": ["
+000012c0: 6772 6179 3734 222c 2022 6772 6179 3630  gray74", "gray60
+000012d0: 225d 0d0a 2020 7d2c 0d0a 2020 2243 546b  "]..  },..  "CTk
+000012e0: 5465 7874 626f 7822 3a20 7b0d 0a20 2020  Textbox": {..   
+000012f0: 2022 636f 726e 6572 5f72 6164 6975 7322   "corner_radius"
+00001300: 3a20 302c 0d0a 2020 2020 2262 6f72 6465  : 0,..    "borde
+00001310: 725f 7769 6474 6822 3a20 312c 0d0a 2020  r_width": 1,..  
+00001320: 2020 2266 675f 636f 6c6f 7222 3a20 5b22    "fg_color": ["
+00001330: 2346 3946 3946 4122 2c20 2223 3144 3145  #F9F9FA", "#1D1E
+00001340: 3145 225d 2c0d 0a20 2020 2022 626f 7264  1E"],..    "bord
+00001350: 6572 5f63 6f6c 6f72 223a 205b 2223 6633  er_color": ["#f3
+00001360: 6633 6633 222c 2022 2339 3439 4139 4622  f3f3", "#949A9F"
+00001370: 5d2c 0d0a 2020 2020 2274 6578 745f 636f  ],..    "text_co
+00001380: 6c6f 7222 3a5b 2267 7261 7931 3022 2c20  lor":["gray10", 
+00001390: 2223 4443 4534 4545 225d 2c0d 0a20 2020  "#DCE4EE"],..   
+000013a0: 2022 7363 726f 6c6c 6261 725f 6275 7474   "scrollbar_butt
+000013b0: 6f6e 5f63 6f6c 6f72 223a 205b 2267 7261  on_color": ["gra
+000013c0: 7935 3522 2c20 2267 7261 7934 3122 5d2c  y55", "gray41"],
+000013d0: 0d0a 2020 2020 2273 6372 6f6c 6c62 6172  ..    "scrollbar
+000013e0: 5f62 7574 746f 6e5f 686f 7665 725f 636f  _button_hover_co
+000013f0: 6c6f 7222 3a20 5b22 6772 6179 3430 222c  lor": ["gray40",
+00001400: 2022 6772 6179 3533 225d 0d0a 2020 7d2c   "gray53"]..  },
+00001410: 0d0a 2020 2243 546b 5363 726f 6c6c 6162  ..  "CTkScrollab
+00001420: 6c65 4672 616d 6522 3a20 7b0d 0a20 2020  leFrame": {..   
+00001430: 2022 6c61 6265 6c5f 6667 5f63 6f6c 6f72   "label_fg_color
+00001440: 223a 205b 2267 7261 7937 3822 2c20 2267  ": ["gray78", "g
+00001450: 7261 7932 3322 5d0d 0a20 207d 2c0d 0a20  ray23"]..  },.. 
+00001460: 2022 4472 6f70 646f 776e 4d65 6e75 223a   "DropdownMenu":
+00001470: 207b 0d0a 2020 2020 2266 675f 636f 6c6f   {..    "fg_colo
+00001480: 7222 3a20 5b22 6772 6179 3930 222c 2022  r": ["gray90", "
+00001490: 2331 6331 6331 6322 5d2c 0d0a 2020 2020  #1c1c1c"],..    
+000014a0: 2268 6f76 6572 5f63 6f6c 6f72 223a 205b  "hover_color": [
+000014b0: 2267 7261 7937 3522 2c20 2223 3331 3331  "gray75", "#3131
+000014c0: 3331 225d 2c0d 0a20 2020 2022 7465 7874  31"],..    "text
+000014d0: 5f63 6f6c 6f72 223a 205b 2267 7261 7931  _color": ["gray1
+000014e0: 3022 2c20 2223 6666 6666 6666 225d 0d0a  0", "#ffffff"]..
+000014f0: 2020 7d2c 0d0a 2020 2243 546b 466f 6e74    },..  "CTkFont
+00001500: 223a 207b 0d0a 2020 2020 226d 6163 4f53  ": {..    "macOS
+00001510: 223a 207b 0d0a 2020 2020 2020 2266 616d  ": {..      "fam
+00001520: 696c 7922 3a20 2253 4620 4469 7370 6c61  ily": "SF Displa
+00001530: 7922 2c0d 0a20 2020 2020 2022 7369 7a65  y",..      "size
+00001540: 223a 2031 332c 0d0a 2020 2020 2020 2277  ": 13,..      "w
+00001550: 6569 6768 7422 3a20 226e 6f72 6d61 6c22  eight": "normal"
+00001560: 0d0a 2020 2020 7d2c 0d0a 2020 2020 2257  ..    },..    "W
+00001570: 696e 646f 7773 223a 207b 0d0a 2020 2020  indows": {..    
+00001580: 2020 2266 616d 696c 7922 3a20 2253 6567    "family": "Seg
+00001590: 6f65 2055 4922 2c0d 0a20 2020 2020 2022  oe UI",..      "
+000015a0: 7369 7a65 223a 2031 332c 0d0a 2020 2020  size": 13,..    
+000015b0: 2020 2277 6569 6768 7422 3a20 226e 6f72    "weight": "nor
+000015c0: 6d61 6c22 0d0a 2020 2020 7d2c 0d0a 2020  mal"..    },..  
+000015d0: 2020 224c 696e 7578 223a 207b 0d0a 2020    "Linux": {..  
+000015e0: 2020 2020 2266 616d 696c 7922 3a20 2252      "family": "R
+000015f0: 6f62 6f74 6f22 2c0d 0a20 2020 2020 2022  oboto",..      "
+00001600: 7369 7a65 223a 2031 332c 0d0a 2020 2020  size": 13,..    
+00001610: 2020 2277 6569 6768 7422 3a20 226e 6f72    "weight": "nor
+00001620: 6d61 6c22 0d0a 2020 2020 7d0d 0a20 207d  mal"..    }..  }
+00001630: 0d0a 7d                                  ..}
```

### Comparing `customtkinterx-0.4.0/customtkinterx/CTkPDFViewer/__pycache__/ctk_pdf_viewer.cpython-311.pyc` & `customtkinterx-0.4.1/customtkinterx/CTkPDFViewer/__pycache__/ctk_pdf_viewer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.0/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py` & `customtkinterx-0.4.1/customtkinterx/CTkPDFViewer/ctk_pdf_viewer.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.0/customtkinterx/CTkTable/__pycache__/ctktable.cpython-311.pyc` & `customtkinterx-0.4.1/customtkinterx/CTkTable/__pycache__/ctktable.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.0/customtkinterx/CTkTable/ctktable.py` & `customtkinterx-0.4.1/customtkinterx/CTkTable/ctktable.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.0/customtkinterx/CTkToolTip/__pycache__/ctk_tooltip.cpython-311.pyc` & `customtkinterx-0.4.1/customtkinterx/CTkToolTip/__pycache__/ctk_tooltip.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.0/customtkinterx/CTkToolTip/ctk_tooltip.py` & `customtkinterx-0.4.1/customtkinterx/CTkToolTip/ctk_tooltip.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.0/customtkinterx/Fluent.json` & `customtkinterx-0.4.1/customtkinterx/Fluent.json`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.0/customtkinterx/fluent_android/__pycache__/CTkFluentAndroidTheme.cpython-311.pyc` & `customtkinterx-0.4.1/customtkinterx/fluent_android/__pycache__/CTkFluentAndroidTheme.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.0/customtkinterx/fluent_android/CTkFluentAndroidTheme.py` & `customtkinterx-0.4.1/customtkinterx/CTkFluentTheme.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,59 @@
-fluent_android_json = """
+fluent_json = """
 {
   "CTkCustom": {
     "titlebar_color": ["#ffffff", "#2c2c2c"],
     "title_color": ["gray10", "#DCE4EE"],
 
     "transparent_color": "#101010",
 
     "closebutton_text_color": ["#000000", "#ffffff"],
     "closebutton_color": ["#ffffff", "#2c2c2c"],
     "closebutton_hover_color": ["#b40d1b", "#b40d1b"],
+    "closebutton_border_width": 0,
 
     "minimizebutton_text_color": ["#000000", "#ffffff"],
     "minimizebutton_color": ["#ffffff", "#2c2c2c"],
-    "minimizebutton_hover_color": ["#cccccc", "#282828"]
+    "minimizebutton_hover_color": ["#cccccc", "#282828"],
+    "minimizebutton_border_width": 0
   },
   "CTkInfoBar": {
     "corner_radius": 8,
-    "border_width": 0,
+    "border_width": 1,
 
+    "text_color": ["#000000", "#ffffff"],
     "fg_color": ["#f7f7f7", "#2f2f2f"],
     "fg_hover_color": ["#c3c3c3", "#555555"],
-
     "border_color": ["#b0b2b2", "#424556"],
 
+    "success_text_color": ["#118d57", "#77ed8b"],
     "success_color": ["#dff6dd", "#393d1b"],
     "success_hover_color": ["#b0c3af", "#5c632b"],
+    "success_border_color": ["#c8eed7", "#194331"],
+
+    "caution_text_color": ["#b76e00", "#fed566"],
     "caution_color": ["#fff4ce", "#433519"],
     "caution_hover_color": ["#ccc3a4", "#695327"],
-    "critical_color": ["#fde7e9", "#442726"],
-    "critical_hover_color": ["#cab8ba", "#6a3c3b"]
+    "caution_border_color": ["#fae7c2", "#4b3c1c"],
 
+    "critical_text_color": ["#b71d18", "#ffac82"],
+    "critical_color": ["#fde7e9", "#442726"],
+    "critical_hover_color": ["#cab8ba", "#6a3c3b"],
+    "critical_border_color": ["#fad5cd", "#4b2927"]
   },
   "CTk": {
     "fg_color": ["#ffffff", "#101010"]
   },
   "CTkToplevel": {
     "fg_color": ["#ffffff", "#101010"]
   },
   "CTkFrame": {
-    "corner_radius": 0,
+    "corner_radius": 8,
     "border_width": 1,
-    "fg_color": ["#ffffff", "#212121"],
+    "fg_color": ["#ffffff", "#1c1c1c"],
     "top_fg_color": ["#ffffff", "#2c2c2c"],
     "border_color": ["#b0b2b2", "#424556"]
   },
   "CTkButton": {
     "corner_radius": 6,
     "border_width": 0,
     "fg_color": ["#0067c0", "#4cc2ff"],
@@ -187,25 +196,25 @@
 }
 """
 
 
 import os.path
 
 
-fluent_android_path = os.path.abspath(os.path.dirname(__file__)).replace("\\", "/") + "/FluentAndroid.json"
+fluent_path = os.path.abspath(os.path.dirname(__file__)).replace("\\", "/") + "/Fluent.json"
 
 
-def fluent_android_theme():
+def fluent_theme():
     from tempfile import mkstemp
     from customtkinter import set_default_color_theme
     _, __temp = mkstemp(suffix=".json")
     with open(__temp, "w") as __temp_file:
-        __temp_file.write(fluent_android_json)
+        __temp_file.write(fluent_json)
     return __temp
 
 
-def use_fluent_android_theme():
+def use_fluent_theme():
     from customtkinter import set_default_color_theme
     try:
-        set_default_color_theme(fluent_android_path)
+        set_default_color_theme(fluent_path)
     except FileNotFoundError:
-        set_default_color_theme(fluent_android_theme())
+        set_default_color_theme(fluent_theme())
```

### Comparing `customtkinterx-0.4.0/customtkinterx/fluent_android/CTkFluentAppBar.py` & `customtkinterx-0.4.1/customtkinterx/fluent_android/CTkFluentAppBar.py`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.0/customtkinterx/fluent_android/FluentAndroid.json` & `customtkinterx-0.4.1/customtkinterx/fluent_android/FluentAndroid.json`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.0/customtkinterx/GhostShark.json` & `customtkinterx-0.4.1/customtkinterx/GhostShark.json`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.0/customtkinterx/LaunchMusix.py` & `customtkinterx-0.4.1/customtkinterx/LaunchMusix.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Union, Callable
 
 
 
 def run_v1():
     from sys import platform
 
-    CTkOffice2019Theme()
+    CTkMinimalTheme()
 
     set_appearance_mode("system")
 
     tk_root = CTkCustom()
     tk_root.create_sizegrip()
     tk_root.wm_geometry(f"350x620")
 
@@ -265,12 +265,12 @@
     searchbox.pack(side="right", fill="x", expand="yes", padx=(15, 5), pady=5)
 
     #set_widget_scaling(1.15)
     root.wm_iconphoto(False, PhotoImage(file="Musix.png"))
     root.mainloop()
 
 def run():
-    run_v2()
+    run_v1()
 
 
 if __name__ == '__main__':
     run()
```

### Comparing `customtkinterx-0.4.0/customtkinterx/Minimal.json` & `customtkinterx-0.4.1/customtkinterx/Minimal.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9088164251207729%*

 * *Differences: {"'CTkCustom'": "{'corner_radius': 10}",*

 * * "'CTkFont'": "{'macOS': {'weight': 'bold'}, 'Windows': {'family': 'Microsoft YaHei', 'weight': "*

 * *              "'bold'}, 'Linux': {'weight': 'bold'}}",*

 * * "'CTkKanban'": "OrderedDict([('fg_color', ['#ffffff', '#212b36']), ('corner_radius', 10), "*

 * *                "('border_width', 0), ('card_corner_radius', 8), ('card_color', ['#ffffff', "*

 * *                "'#212b36']), ('card_border_width', 0), ('card_border_color', ['#e8eaee', "*

 * *                "'#27303b']), ('task_co […]*

```diff
@@ -95,14 +95,15 @@
             "#b40d1b",
             "#b40d1b"
         ],
         "closebutton_text_color": [
             "#000000",
             "#ffffff"
         ],
+        "corner_radius": 10,
         "minimizebutton_border_width": 0,
         "minimizebutton_color": [
             "#f4f6f8",
             "#212b36"
         ],
         "minimizebutton_hover_color": [
             "#dfe3e8",
@@ -142,25 +143,25 @@
             "#ffffff"
         ]
     },
     "CTkFont": {
         "Linux": {
             "family": "Roboto",
             "size": 13,
-            "weight": "normal"
+            "weight": "bold"
         },
         "Windows": {
-            "family": "Roboto",
+            "family": "Microsoft YaHei",
             "size": 13,
-            "weight": "normal"
+            "weight": "bold"
         },
         "macOS": {
             "family": "SF Display",
             "size": 13,
-            "weight": "normal"
+            "weight": "bold"
         }
     },
     "CTkFrame": {
         "border_color": [
             "#edeff1",
             "#212b36"
         ],
@@ -239,14 +240,42 @@
             "#77ed8b"
         ],
         "text_color": [
             "#006c9c",
             "#61f3f3"
         ]
     },
+    "CTkKanban": {
+        "border_width": 0,
+        "card_border_color": [
+            "#e8eaee",
+            "#27303b"
+        ],
+        "card_border_width": 0,
+        "card_color": [
+            "#ffffff",
+            "#212b36"
+        ],
+        "card_corner_radius": 8,
+        "corner_radius": 10,
+        "fg_color": [
+            "#ffffff",
+            "#212b36"
+        ],
+        "task_border_color": [
+            "#fefefe",
+            "#1c242e"
+        ],
+        "task_border_width": 0,
+        "task_color": [
+            "#f4f6f8",
+            "#2e3944"
+        ],
+        "task_corner_radius": 10
+    },
     "CTkLabel": {
         "corner_radius": 0,
         "fg_color": "transparent",
         "text_color": [
             "gray10",
             "#DCE4EE"
         ]
@@ -384,14 +413,24 @@
             "#113d36"
         ],
         "progress_color": [
             "#00a76f",
             "#00a76f"
         ]
     },
+    "CTkSnackBar": {
+        "fg_color": [
+            "#ffffff",
+            "#212b36"
+        ],
+        "text_color": [
+            "#000000",
+            "#ffffff"
+        ]
+    },
     "CTkSwitch": {
         "border_width": 0,
         "button_color": [
             "#f9fafb",
             "#ffffff"
         ],
         "button_hover_color": [
```

### Comparing `customtkinterx-0.4.0/customtkinterx/Musix-Dark.png` & `customtkinterx-0.4.1/customtkinterx/Musix-Dark.png`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.0/customtkinterx/Musix.png` & `customtkinterx-0.4.1/customtkinterx/Musix.png`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.0/customtkinterx/Office2019.json` & `customtkinterx-0.4.1/customtkinterx/Material.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7318567402806534%*

 * *Differences: {"'CTk'": "{'fg_color': ['#FFFFFF', '#000000']}",*

 * * "'CTkButton'": "{'corner_radius': 6, 'border_width': 0, 'fg_color': ['#5956EB', '#B6C3FD'], "*

 * *                "'hover_color': ['#6365F1', '#A5B4FC'], 'border_color': ['#5956eb', '#b6c3fd'], "*

 * *                "'text_color': ['#FFFFFF', '#1E1E1E'], 'text_color_disabled': ['#a6b0bb', "*

 * *                "'#788490']}",*

 * * "'CTkCheckbox'": "{'corner_radius': 8, 'border_width': 2, 'fg_color': ['#00a76f', '#00a76f'], "*

 * *                  "'border_color': ['#637381', '# […]*

```diff
@@ -1,434 +1,500 @@
 {
     "CTk": {
         "fg_color": [
-            "#ffffff",
-            "#101010"
+            "#FFFFFF",
+            "#000000"
         ]
     },
     "CTkButton": {
         "border_color": [
-            "#f3f3f3",
-            "#949A9F"
+            "#5956eb",
+            "#b6c3fd"
         ],
-        "border_width": 1,
-        "corner_radius": 0,
+        "border_width": 0,
+        "corner_radius": 6,
         "fg_color": [
-            "#e5e5e5",
-            "#3d3d3d"
+            "#5956EB",
+            "#B6C3FD"
         ],
         "hover_color": [
-            "#b2b2b2",
-            "#151515"
+            "#6365F1",
+            "#A5B4FC"
         ],
         "text_color": [
-            "#000000",
-            "#ffffff"
+            "#FFFFFF",
+            "#1E1E1E"
         ],
         "text_color_disabled": [
-            "gray74",
-            "gray60"
+            "#a6b0bb",
+            "#788490"
         ]
     },
     "CTkCheckbox": {
         "border_color": [
-            "#3E454A",
-            "#949A9F"
+            "#637381",
+            "#919eab"
         ],
-        "border_width": 3,
+        "border_width": 2,
         "checkmark_color": [
-            "#DCE4EE",
-            "gray90"
+            "#f9fafb",
+            "#161c24"
         ],
-        "corner_radius": 6,
+        "corner_radius": 8,
         "fg_color": [
-            "#3B8ED0",
-            "#1F6AA5"
+            "#00a76f",
+            "#00a76f"
         ],
         "hover_color": [
-            "#3B8ED0",
-            "#1F6AA5"
+            "#00a76f",
+            "#00a76f"
         ],
         "text_color": [
-            "gray10",
-            "#DCE4EE"
+            "#212b36",
+            "#f8f8f8"
         ],
         "text_color_disabled": [
             "gray60",
             "gray45"
         ]
     },
     "CTkComboBox": {
         "border_color": [
-            "#f3f3f3",
-            "#949A9F"
+            "#c4cdd5",
+            "#637381"
         ],
         "border_width": 1,
         "button_color": [
-            "#f2f2f2",
-            "#565B5E"
+            "#c4cdd5",
+            "#637381"
         ],
         "button_hover_color": [
-            "#f2f2f2",
-            "#565B5E"
+            "#919eab",
+            "#919eab"
         ],
-        "corner_radius": 0,
+        "corner_radius": 10,
         "fg_color": [
-            "#ffffff",
-            "#2f2f2f"
+            "#dfe3e8",
+            "#454f5b"
         ],
         "text_color": [
             "gray10",
             "#ffffff"
         ],
         "text_color_disabled": [
             "gray50",
             "gray45"
         ]
     },
     "CTkCustom": {
+        "closebutton_border_width": 0,
         "closebutton_color": [
-            "#ffffff",
-            "#2c2c2c"
+            "#f4f6f8",
+            "#212b36"
         ],
         "closebutton_hover_color": [
             "#b40d1b",
             "#b40d1b"
         ],
         "closebutton_text_color": [
             "#000000",
             "#ffffff"
         ],
+        "corner_radius": 10,
+        "minimizebutton_border_width": 0,
         "minimizebutton_color": [
-            "#ffffff",
-            "#2c2c2c"
+            "#f4f6f8",
+            "#212b36"
         ],
         "minimizebutton_hover_color": [
-            "#cccccc",
-            "#282828"
+            "#dfe3e8",
+            "#454f5b"
         ],
         "minimizebutton_text_color": [
             "#000000",
             "#ffffff"
         ],
         "title_color": [
-            "#ffffff",
-            "#ffffff"
+            "gray10",
+            "#DCE4EE"
         ],
         "titlebar_color": [
-            "#106ebe",
-            "#106ebe"
+            "#f4f6f8",
+            "#161c24"
         ],
         "transparent_color": "#101010"
     },
     "CTkEntry": {
         "border_color": [
-            "#f3f3f3",
-            "#949A9F"
+            "#eaedf0",
+            "#2f363f"
         ],
         "border_width": 1,
-        "corner_radius": 0,
+        "corner_radius": 10,
         "fg_color": [
-            "#ffffff",
-            "#2f2f2f"
+            "#f9fafb",
+            "#161c24"
         ],
         "placeholder_text_color": [
-            "gray52",
-            "gray62"
+            "#a6b0bb",
+            "#637381"
         ],
         "text_color": [
-            "#000000",
+            "#212b36",
             "#ffffff"
         ]
     },
     "CTkFont": {
         "Linux": {
             "family": "Roboto",
             "size": 13,
-            "weight": "normal"
+            "weight": "bold"
         },
         "Windows": {
-            "family": "Segoe UI",
+            "family": "Microsoft YaHei",
             "size": 13,
-            "weight": "normal"
+            "weight": "bold"
         },
         "macOS": {
             "family": "SF Display",
             "size": 13,
-            "weight": "normal"
+            "weight": "bold"
         }
     },
     "CTkFrame": {
         "border_color": [
-            "#b0b2b2",
-            "#424556"
+            "#edeff1",
+            "#212b36"
         ],
         "border_width": 1,
-        "corner_radius": 0,
+        "corner_radius": 10,
         "fg_color": [
-            "#ffffff",
-            "#1c1c1c"
+            "#F5F5F5",
+            "#121212"
         ],
         "top_fg_color": [
-            "#ffffff",
-            "#2c2c2c"
+            "#F5F5F5",
+            "#121212"
         ]
     },
     "CTkInfoBar": {
         "border_color": [
-            "#b0b2b2",
-            "#424556"
+            "#c0ebf3",
+            "#113f4d"
+        ],
+        "border_width": 1,
+        "caution_border_color": [
+            "#fae7c2",
+            "#4b3c1c"
         ],
-        "border_width": 0,
         "caution_color": [
-            "#fff4ce",
-            "#433519"
+            "#f9f3e7",
+            "#292721"
         ],
         "caution_hover_color": [
-            "#ccc3a4",
-            "#695327"
+            "#fae7c2",
+            "#4b3c1c"
+        ],
+        "caution_text_color": [
+            "#b76e00",
+            "#fed566"
         ],
         "corner_radius": 8,
+        "critical_border_color": [
+            "#fad5cd",
+            "#4b2927"
+        ],
         "critical_color": [
-            "#fde7e9",
-            "#442726"
+            "#f9edeb",
+            "#292125"
         ],
         "critical_hover_color": [
-            "#cab8ba",
-            "#6a3c3b"
+            "#fad5cd",
+            "#4b2927"
+        ],
+        "critical_text_color": [
+            "#b71d18",
+            "#ffac82"
         ],
         "fg_color": [
-            "#f7f7f7",
-            "#2f2f2f"
+            "#e5f4f8",
+            "#142832"
         ],
         "fg_hover_color": [
-            "#c3c3c3",
-            "#555555"
+            "#c0ebf3",
+            "#113f4d"
+        ],
+        "success_border_color": [
+            "#c8eed7",
+            "#194331"
         ],
         "success_color": [
-            "#dff6dd",
-            "#393d1b"
+            "#e8f5ee",
+            "#172a29"
         ],
         "success_hover_color": [
-            "#b0c3af",
-            "#5c632b"
+            "#c8eed7",
+            "#194331"
+        ],
+        "success_text_color": [
+            "#118d57",
+            "#77ed8b"
+        ],
+        "text_color": [
+            "#006c9c",
+            "#61f3f3"
         ]
     },
+    "CTkKanban": {
+        "border_width": 0,
+        "card_border_color": [
+            "#e8eaee",
+            "#27303b"
+        ],
+        "card_border_width": 0,
+        "card_color": [
+            "#ffffff",
+            "#212b36"
+        ],
+        "card_corner_radius": 8,
+        "corner_radius": 10,
+        "fg_color": [
+            "#ffffff",
+            "#212b36"
+        ],
+        "task_border_color": [
+            "#fefefe",
+            "#1c242e"
+        ],
+        "task_border_width": 0,
+        "task_color": [
+            "#f4f6f8",
+            "#2e3944"
+        ],
+        "task_corner_radius": 10
+    },
     "CTkLabel": {
         "corner_radius": 0,
         "fg_color": "transparent",
         "text_color": [
             "gray10",
             "#DCE4EE"
         ]
     },
     "CTkOptionMenu": {
         "button_color": [
-            "#36719F",
-            "#144870"
+            "#007867",
+            "#007867"
         ],
         "button_hover_color": [
-            "#27577D",
-            "#203A4F"
+            "#007867",
+            "#007867"
         ],
-        "corner_radius": 6,
+        "corner_radius": 8,
         "fg_color": [
-            "#3B8ED0",
-            "#1F6AA5"
+            "#00a76f",
+            "#00a76f"
         ],
         "text_color": [
-            "#DCE4EE",
-            "#DCE4EE"
+            "#ffffff",
+            "#ffffff"
         ],
         "text_color_disabled": [
             "gray74",
             "gray60"
         ]
     },
     "CTkProgressBar": {
         "border_color": [
-            "gray",
-            "gray"
+            "#00a76f",
+            "#00a76f"
         ],
         "border_width": 0,
-        "corner_radius": 1000,
+        "corner_radius": 16,
         "fg_color": [
-            "#939BA2",
-            "#4A4D50"
+            "#bde6da",
+            "#113d36"
         ],
         "progress_color": [
-            "#3B8ED0",
-            "#1F6AA5"
+            "#00a76f",
+            "#00a76f"
         ]
     },
     "CTkRadiobutton": {
         "border_color": [
-            "#3E454A",
-            "#949A9F"
+            "#637381",
+            "#919eab"
         ],
         "border_width_checked": 6,
-        "border_width_unchecked": 3,
+        "border_width_unchecked": 2,
         "corner_radius": 1000,
         "fg_color": [
-            "#3B8ED0",
-            "#1F6AA5"
+            "#00a76f",
+            "#00a76f"
         ],
         "hover_color": [
-            "#36719F",
-            "#144870"
+            "#00a76f",
+            "#00a76f"
         ],
         "text_color": [
-            "gray10",
-            "#DCE4EE"
+            "#212b36",
+            "#f8f8f8"
         ],
         "text_color_disabled": [
             "gray60",
             "gray45"
         ]
     },
     "CTkScrollableFrame": {
         "label_fg_color": [
-            "gray78",
-            "gray23"
+            "#f9fafb",
+            "#161c24"
         ]
     },
     "CTkScrollbar": {
-        "border_spacing": 9,
+        "border_spacing": 4,
         "button_color": [
-            "gray55",
-            "gray41"
+            "#a0abb7",
+            "#788490"
         ],
         "button_hover_color": [
-            "gray40",
-            "gray53"
+            "#a3aeb9",
+            "#7b8793"
         ],
-        "corner_radius": 0,
+        "corner_radius": 1000,
         "fg_color": "transparent"
     },
     "CTkSegmentedButton": {
-        "border_width": 2,
-        "corner_radius": 6,
+        "border_width": 4,
+        "corner_radius": 12,
         "fg_color": [
-            "#979DA2",
-            "gray29"
+            "#ffffff",
+            "#212b36"
         ],
         "selected_color": [
-            "#3B8ED0",
-            "#1F6AA5"
+            "#ffffff",
+            "#212b36"
         ],
         "selected_hover_color": [
-            "#36719F",
-            "#144870"
+            "#00744d",
+            "#00744d"
         ],
         "text_color": [
-            "#DCE4EE",
+            "#212b36",
             "#DCE4EE"
         ],
         "text_color_disabled": [
-            "gray74",
+            "#637381",
             "gray60"
         ],
         "unselected_color": [
-            "#979DA2",
-            "gray29"
+            "#ffffff",
+            "#212b36"
         ],
         "unselected_hover_color": [
-            "gray70",
-            "gray41"
+            "#00a76f",
+            "#00a76f"
         ]
     },
     "CTkSlider": {
         "border_width": 6,
         "button_color": [
-            "#3B8ED0",
-            "#1F6AA5"
+            "#00a76f",
+            "#00a76f"
         ],
         "button_corner_radius": 1000,
         "button_hover_color": [
-            "#36719F",
-            "#144870"
+            "#00a76f",
+            "#00a76f"
         ],
         "button_length": 0,
         "corner_radius": 1000,
         "fg_color": [
-            "#939BA2",
-            "#4A4D50"
+            "#bde6da",
+            "#113d36"
         ],
         "progress_color": [
-            "gray40",
-            "#AAB0B5"
+            "#00a76f",
+            "#00a76f"
+        ]
+    },
+    "CTkSnackBar": {
+        "fg_color": [
+            "#ffffff",
+            "#212b36"
+        ],
+        "text_color": [
+            "#000000",
+            "#ffffff"
         ]
     },
     "CTkSwitch": {
-        "border_width": 1,
+        "border_width": 0,
         "button_color": [
-            "#f3f3f3",
-            "#000000"
+            "#f9fafb",
+            "#ffffff"
         ],
         "button_hover_color": [
-            "#bfbfbf",
-            "#050505"
+            "#f4f6f8",
+            "#ffffff"
         ],
-        "button_length": 2,
-        "corner_radius": 8,
+        "button_length": 0,
+        "corner_radius": 1000,
         "fg_color": [
-            "#ededed",
-            "#1d1d1d"
-        ],
-        "progress_color": [
-            "#0067c0",
-            "#4cc2ff"
+            "#c7ced5",
+            "#637381"
         ],
+        "progress_color": "#00a46d",
         "text_color": [
             "gray10",
             "#DCE4EE"
         ],
         "text_color_disabled": [
             "gray60",
             "gray45"
         ]
     },
     "CTkTextbox": {
         "border_color": [
-            "#f3f3f3",
-            "#949A9F"
+            "#eaedf0",
+            "#2f363f"
         ],
         "border_width": 1,
-        "corner_radius": 0,
+        "corner_radius": 10,
         "fg_color": [
-            "#F9F9FA",
-            "#1D1E1E"
+            "#f9fafb",
+            "#161c24"
         ],
         "scrollbar_button_color": [
-            "gray55",
-            "gray41"
+            "#a0abb7",
+            "#788490"
         ],
         "scrollbar_button_hover_color": [
-            "gray40",
-            "gray53"
+            "#a3aeb9",
+            "#7b8793"
         ],
         "text_color": [
-            "gray10",
-            "#DCE4EE"
+            "#212b36",
+            "#ffffff"
         ]
     },
     "CTkToplevel": {
         "fg_color": [
-            "#ffffff",
-            "#101010"
+            "#FFFFFF",
+            "#000000"
         ]
     },
     "DropdownMenu": {
         "fg_color": [
-            "gray90",
-            "#1c1c1c"
+            "#feffff",
+            "#202a34"
         ],
         "hover_color": [
-            "gray75",
-            "#313131"
+            "#eaeff1",
+            "#323c47"
         ],
         "text_color": [
-            "gray10",
-            "#ffffff"
+            "#212b36",
+            "#f1f1f2"
         ]
     }
 }
```

### Comparing `customtkinterx-0.4.0/customtkinterx/PublicSans-Regular.ttf` & `customtkinterx-0.4.1/customtkinterx/PublicSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `customtkinterx-0.4.0/customtkinterx/test.py` & `customtkinterx-0.4.1/customtkinterx/test.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,83 +7,94 @@
 customtkinterx.CTkMinimalTheme()
 
 
 class App(customtkinter.CTk):
     def __init__(self):
         super().__init__()
 
+        font = customtkinter.CTkFont(family="Microsoft YaHei", weight="bold")
+
         # configure window
         self.title("CustomTkinter complex_example.py")
         self.geometry(f"{1100}x{580}")
 
         # configure grid layout (4x4)
         self.grid_columnconfigure(1, weight=1)
         self.grid_columnconfigure((2, 3), weight=0)
         self.grid_rowconfigure((0, 1, 2), weight=1)
 
         # create sidebar frame with widgets
         self.sidebar_frame = customtkinter.CTkFrame(self, width=140, corner_radius=0)
         self.sidebar_frame.grid(row=0, column=0, rowspan=4, sticky="nsew")
         self.sidebar_frame.grid_rowconfigure(4, weight=1)
-        self.logo_label = customtkinter.CTkLabel(self.sidebar_frame, text="CustomTkinter", font=customtkinter.CTkFont(size=20, weight="bold"))
+        self.logo_label = customtkinter.CTkLabel(self.sidebar_frame, text="CustomTkinter", font=customtkinter.CTkFont(family="Public Sans", size=20, weight="bold"))
         self.logo_label.grid(row=0, column=0, padx=20, pady=(20, 10))
-        self.sidebar_button_1 = customtkinter.CTkButton(self.sidebar_frame, command=self.sidebar_button_event)
+        self.sidebar_button_1 = customtkinter.CTkButton(self.sidebar_frame, command=self.sidebar_button_event, font=font)
         self.sidebar_button_1.grid(row=1, column=0, padx=20, pady=10)
-        self.sidebar_button_2 = customtkinter.CTkButton(self.sidebar_frame, command=self.sidebar_button_event)
+        self.sidebar_button_2 = customtkinter.CTkButton(self.sidebar_frame, command=self.sidebar_button_event, font=font)
         self.sidebar_button_2.grid(row=2, column=0, padx=20, pady=10)
-        self.sidebar_button_3 = customtkinter.CTkButton(self.sidebar_frame, command=self.sidebar_button_event)
+        self.sidebar_button_3 = customtkinter.CTkButton(self.sidebar_frame, command=self.sidebar_button_event, font=font)
         self.sidebar_button_3.grid(row=3, column=0, padx=20, pady=10)
-        self.appearance_mode_label = customtkinter.CTkLabel(self.sidebar_frame, text="Appearance Mode:", anchor="w")
+        self.appearance_mode_label = customtkinter.CTkLabel(self.sidebar_frame, text="Appearance Mode:", anchor="w", font=font)
         self.appearance_mode_label.grid(row=5, column=0, padx=20, pady=(10, 0))
-        self.appearance_mode_optionemenu = customtkinter.CTkOptionMenu(self.sidebar_frame, values=["Light", "Dark", "System"],
+        self.appearance_mode_optionemenu = customtkinter.CTkOptionMenu(self.sidebar_frame, values=["Light", "Dark", "System"], font=font,
                                                                        command=self.change_appearance_mode_event)
         self.appearance_mode_optionemenu.grid(row=6, column=0, padx=20, pady=(10, 10))
-        self.scaling_label = customtkinter.CTkLabel(self.sidebar_frame, text="UI Scaling:", anchor="w")
+        self.scaling_label = customtkinter.CTkLabel(self.sidebar_frame, text="UI Scaling:", anchor="w", font=font)
         self.scaling_label.grid(row=7, column=0, padx=20, pady=(10, 0))
         self.scaling_optionemenu = customtkinter.CTkOptionMenu(self.sidebar_frame, values=["80%", "90%", "100%", "110%", "120%"],
-                                                               command=self.change_scaling_event)
+                                                               command=self.change_scaling_event, font=font)
         self.scaling_optionemenu.grid(row=8, column=0, padx=20, pady=(10, 20))
 
         # create main entry and button
-        self.entry = customtkinter.CTkEntry(self, placeholder_text="CTkEntry")
+        self.entry = customtkinter.CTkEntry(self, placeholder_text="CTkEntry", font=font)
         self.entry.grid(row=3, column=1, columnspan=2, padx=(20, 0), pady=(20, 20), sticky="nsew")
 
-        self.main_button_1 = customtkinter.CTkButton(master=self, fg_color="transparent", border_width=2, text_color=("gray10", "#DCE4EE"))
+        self.main_button_1 = customtkinter.CTkButton(master=self, fg_color="transparent", border_width=2, text_color=("gray10", "#DCE4EE"), font=font)
         self.main_button_1.grid(row=3, column=3, padx=(20, 20), pady=(20, 20), sticky="nsew")
 
         # create textbox
-        self.textbox = customtkinter.CTkTextbox(self, width=250)
+        self.textbox = customtkinter.CTkTextbox(self, width=250, font=font)
         self.textbox.grid(row=0, column=1, padx=(20, 0), pady=(20, 0), sticky="nsew")
 
         # create tabview
         self.tabview = customtkinter.CTkTabview(self, width=250)
         self.tabview.grid(row=0, column=2, padx=(20, 0), pady=(20, 0), sticky="nsew")
         self.tabview.add("CTkTabview")
         self.tabview.add("Tab 2")
         self.tabview.add("Tab 3")
         self.tabview.tab("CTkTabview").grid_columnconfigure(0, weight=1)  # configure grid of individual tabs
         self.tabview.tab("Tab 2").grid_columnconfigure(0, weight=1)
 
         self.optionmenu_1 = customtkinter.CTkOptionMenu(self.tabview.tab("CTkTabview"), dynamic_resizing=False,
-                                                        values=["Value 1", "Value 2", "Value Long Long Long"])
+                                                        values=["Value 1", "Value 2", "Value Long Long Long"], font=font)
         self.optionmenu_1.grid(row=0, column=0, padx=20, pady=(20, 10))
         self.combobox_1 = customtkinter.CTkComboBox(self.tabview.tab("CTkTabview"),
-                                                    values=["Value 1", "Value 2", "Value Long....."])
+                                                    values=["Value 1", "Value 2", "Value Long....."], font=font)
         self.combobox_1.grid(row=1, column=0, padx=20, pady=(10, 10))
         self.string_input_button = customtkinter.CTkButton(self.tabview.tab("CTkTabview"), text="Open CTkInputDialog",
-                                                           command=self.open_input_dialog_event)
+                                                           command=self.open_input_dialog_event, font=font)
         self.string_input_button.grid(row=2, column=0, padx=20, pady=(10, 10))
-        self.label_tab_2 = customtkinter.CTkLabel(self.tabview.tab("Tab 2"), text="CTkLabel on Tab 2")
-        self.label_tab_2.grid(row=0, column=0, padx=20, pady=20)
+
+        self.frame_1 = customtkinter.CTkScrollableFrame(self.tabview.tab("Tab 2"), fg_color=self.tabview.tab("Tab 2")._fg_color)
+        self.frame_1.pack(fill="both", expand="yes", padx=5, pady=5, ipadx=60, ipady=30)
+
+        customtkinterx.CTkInfoBar(self.frame_1, text="hello, i am a infobar", severity=customtkinterx.NORMAL).show()
+        customtkinterx.CTkInfoBar(self.frame_1, text="hello, i am a infobar", severity=customtkinterx.SUCCESS).show()
+        customtkinterx.CTkInfoBar(self.frame_1, text="hello, i am a infobar", severity=customtkinterx.CAUTION).show()
+        customtkinterx.CTkInfoBar(self.frame_1, text="hello, i am a infobar", severity=customtkinterx.CRITICAL).show()
+
+        self.snackbar_1 = customtkinterx.CTkSnackBar(self.frame_1, info="CTkSnackBar", action=["action", "$close"])
+        self.snackbar_1.show()
 
         # create radiobutton frame
         self.radiobutton_frame = customtkinter.CTkFrame(self)
         self.radiobutton_frame.grid(row=0, column=3, padx=(20, 20), pady=(20, 0), sticky="nsew")
         self.radio_var = tkinter.IntVar(value=0)
-        self.label_radio_group = customtkinter.CTkLabel(master=self.radiobutton_frame, text="CTkRadioButton Group:")
+        self.label_radio_group = customtkinter.CTkLabel(master=self.radiobutton_frame, text="CTkRadioButton Group:", font=font)
         self.label_radio_group.grid(row=0, column=2, columnspan=1, padx=10, pady=10, sticky="")
         self.radio_button_1 = customtkinter.CTkRadioButton(master=self.radiobutton_frame, variable=self.radio_var, value=0)
         self.radio_button_1.grid(row=1, column=2, pady=10, padx=20, sticky="n")
         self.radio_button_2 = customtkinter.CTkRadioButton(master=self.radiobutton_frame, variable=self.radio_var, value=1)
         self.radio_button_2.grid(row=2, column=2, pady=10, padx=20, sticky="n")
         self.radio_button_3 = customtkinter.CTkRadioButton(master=self.radiobutton_frame, variable=self.radio_var, value=2)
         self.radio_button_3.grid(row=3, column=2, pady=10, padx=20, sticky="n")
```

### Comparing `customtkinterx-0.4.0/README.md` & `customtkinterx-0.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 ### 添加缩放窗口大小的手柄
 ```python
 CTKCustom.create_sizegrip()
 ```
 自定义手柄，将会使用库`pyautogui`。
 ```bash
-python -m pyautogui
+python -m pip install pyautogui
 ```
 ```python
 CTKCustom.create_sizegrip(True)
 ```
 
 ```python
 from customtkinter import *
```

### Comparing `customtkinterx-0.4.0/PKG-INFO` & `customtkinterx-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: customtkinterx
-Version: 0.4.0
+Version: 0.4.1
 Summary: extra widgets for customtkinter
 Author: XiangQinxi
 Author-email: XiangQinxi@outlook.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -75,15 +75,15 @@
 
 ### 添加缩放窗口大小的手柄
 ```python
 CTKCustom.create_sizegrip()
 ```
 自定义手柄，将会使用库`pyautogui`。
 ```bash
-python -m pyautogui
+python -m pip install pyautogui
 ```
 ```python
 CTKCustom.create_sizegrip(True)
 ```
 
 ```python
 from customtkinter import *
```

