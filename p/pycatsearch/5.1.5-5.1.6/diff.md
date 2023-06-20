# Comparing `tmp/pycatsearch-5.1.5.tar.gz` & `tmp/pycatsearch-5.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycatsearch-5.1.5.tar", last modified: Fri May 26 10:59:25 2023, max compression
+gzip compressed data, was "pycatsearch-5.1.6.tar", last modified: Tue Jun 20 15:18:17 2023, max compression
```

## Comparing `pycatsearch-5.1.5.tar` & `pycatsearch-5.1.6.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:59:25.743520 pycatsearch-5.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:59:25.735520 pycatsearch-5.1.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:59:25.739520 pycatsearch-5.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    10610 2023-05-26 10:59:25.743520 pycatsearch-5.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9070 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     1230 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 10:59:25.743520 pycatsearch-5.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:59:25.735520 pycatsearch-5.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:59:25.739520 pycatsearch-5.1.5/src/pycatsearch/
--rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      109 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-26 10:59:25.000000 pycatsearch-5.1.5/src/pycatsearch/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/async_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    18859 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/catalog_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:59:25.743520 pycatsearch-5.1.5/src/pycatsearch/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/gui/catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/gui/download_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/gui/float_spinbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/gui/frequency_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/gui/menu_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/gui/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/gui/selectable_label.py
--rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/gui/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/gui/substance_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/gui/substances_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/gui/titled_list_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    41570 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/gui/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/gui/waiting_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)    24830 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/src/pycatsearch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:59:25.739520 pycatsearch-5.1.5/src/pycatsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10610 2023-05-26 10:59:25.000000 pycatsearch-5.1.5/src/pycatsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-26 10:59:25.000000 pycatsearch-5.1.5/src/pycatsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 10:59:25.000000 pycatsearch-5.1.5/src/pycatsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-26 10:59:25.000000 pycatsearch-5.1.5/src/pycatsearch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 10:59:25.000000 pycatsearch-5.1.5/src/pycatsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 10:59:25.000000 pycatsearch-5.1.5/src/pycatsearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-05-26 10:59:14.000000 pycatsearch-5.1.5/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:18:17.160011 pycatsearch-5.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:18:17.152011 pycatsearch-5.1.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:18:17.156011 pycatsearch-5.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10610 2023-06-20 15:18:17.160011 pycatsearch-5.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9070 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1230 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 15:18:17.160011 pycatsearch-5.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:18:17.156011 pycatsearch-5.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:18:17.156011 pycatsearch-5.1.6/src/pycatsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      109 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-20 15:18:17.000000 pycatsearch-5.1.6/src/pycatsearch/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/async_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18859 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/catalog_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:18:17.160011 pycatsearch-5.1.6/src/pycatsearch/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/gui/catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/gui/download_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/gui/float_spinbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7984 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/gui/frequency_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/gui/menu_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/gui/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/gui/selectable_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/gui/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/gui/substance_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/gui/substances_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/gui/titled_list_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45208 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/gui/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/gui/waiting_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24947 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/src/pycatsearch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:18:17.160011 pycatsearch-5.1.6/src/pycatsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10610 2023-06-20 15:18:17.000000 pycatsearch-5.1.6/src/pycatsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-20 15:18:17.000000 pycatsearch-5.1.6/src/pycatsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:18:17.000000 pycatsearch-5.1.6/src/pycatsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-20 15:18:17.000000 pycatsearch-5.1.6/src/pycatsearch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 15:18:17.000000 pycatsearch-5.1.6/src/pycatsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-20 15:18:17.000000 pycatsearch-5.1.6/src/pycatsearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-06-20 15:18:06.000000 pycatsearch-5.1.6/updater.py
```

### Comparing `pycatsearch-5.1.5/.github/workflows/publish-to-pypi.yml` & `pycatsearch-5.1.6/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.5/LICENSE.md` & `pycatsearch-5.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.5/PKG-INFO` & `pycatsearch-5.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycatsearch
-Version: 5.1.5
+Version: 5.1.6
 Summary: Yet another implementation of JPL and CDMS spectroscopy catalogs offline search
 Author-email: StSav012 <stsav012@gmail.com>
 License: LGPL-3.0-only
 Project-URL: Source Code, https://github.com/StSav012/pycatsearch
 Project-URL: Bug Tracker, https://github.com/StSav012/pycatsearch/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Win32 (MS Windows)
```

### Comparing `pycatsearch-5.1.5/README.md` & `pycatsearch-5.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.5/main.py` & `pycatsearch-5.1.6/main.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.5/pyproject.toml` & `pycatsearch-5.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.5/setup.py` & `pycatsearch-5.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.5/src/pycatsearch/__init__.py` & `pycatsearch-5.1.6/src/pycatsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.5/src/pycatsearch/async_downloader.py` & `pycatsearch-5.1.6/src/pycatsearch/async_downloader.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.5/src/pycatsearch/catalog.py` & `pycatsearch-5.1.6/src/pycatsearch/catalog.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.5/src/pycatsearch/catalog_entry.py` & `pycatsearch-5.1.6/src/pycatsearch/catalog_entry.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.5/src/pycatsearch/downloader.py` & `pycatsearch-5.1.6/src/pycatsearch/downloader.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.5/src/pycatsearch/gui/catalog_info.py` & `pycatsearch-5.1.6/src/pycatsearch/gui/catalog_info.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.5/src/pycatsearch/gui/download_dialog.py` & `pycatsearch-5.1.6/src/pycatsearch/gui/download_dialog.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.5/src/pycatsearch/gui/float_spinbox.py` & `pycatsearch-5.1.6/src/pycatsearch/gui/float_spinbox.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.5/src/pycatsearch/gui/frequency_box.py` & `pycatsearch-5.1.6/src/pycatsearch/gui/frequency_box.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,16 @@
         self.setMaximum(9999999.9999)
         self.setSuffix(self.tr(' MHz'))
         self.setCorrectionMode(QAbstractSpinBox.CorrectionMode.CorrectToNearestValue)
 
 
 class FrequencyBox(QTabWidget):
     def __init__(self, settings: Settings, parent: QWidget | None = None) -> None:
+        from . import icon  # import locally to avoid a circular import
+
         super().__init__(parent)
 
         self._settings: Settings = settings
 
         self._frequency_from: float = -inf  # [MHz]
         self._frequency_to: float = inf  # [MHz]
         self._frequency_center: float = 0.0  # [MHz]
@@ -48,23 +50,23 @@
         self._spin_frequency_deviation: FrequencySpinBox = FrequencySpinBox(self._page_by_center)
 
         self._layout_by_range.setLabelAlignment(Qt.AlignmentFlag.AlignLeft)
         self._spin_frequency_from.setValue(118747.341)
         self._layout_by_range.addRow(self._layout_by_range.tr('From:'), self._spin_frequency_from)
         self._spin_frequency_to.setValue(118753.341)
         self._layout_by_range.addRow(self._layout_by_range.tr('To:'), self._spin_frequency_to)
-        self.addTab(self._page_by_range, self.tr('Range'))
+        self.addTab(self._page_by_range, icon('mdi6.arrow-expand-horizontal'), self.tr('Range'))
 
         self._spin_frequency_center.setValue(118750.341)
         self._layout_by_center.addRow(self._layout_by_center.tr('Center:'), self._spin_frequency_center)
         self._spin_frequency_deviation.setMaximum(99.9999)
         self._spin_frequency_deviation.setSingleStep(0.1)
         self._spin_frequency_deviation.setValue(0.4)
         self._layout_by_center.addRow(self._layout_by_center.tr('Deviation:'), self._spin_frequency_deviation)
-        self.addTab(self._page_by_center, self.tr('Center'))
+        self.addTab(self._page_by_center, icon('mdi6.format-horizontal-align-center'), self.tr('Center'))
 
         self.load_settings()
 
         self._spin_frequency_from.editingFinished.connect(self._on_spin_frequency_from_edited)
         self._spin_frequency_to.editingFinished.connect(self._on_spin_frequency_to_edited)
         self._spin_frequency_center.editingFinished.connect(self._on_spin_frequency_center_edited)
         self._spin_frequency_deviation.editingFinished.connect(self._on_spin_frequency_deviation_edited)
```

### Comparing `pycatsearch-5.1.5/src/pycatsearch/gui/menu_bar.py` & `pycatsearch-5.1.6/src/pycatsearch/gui/menu_bar.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 
         self.menu_edit: QMenu = self.addMenu(self.tr('&Edit'))
         self.action_clear: QAction = self.menu_edit.addAction(
             self._icon('edit-clear', 'mdi6.broom', standard_pixmap=QStyle.StandardPixmap.SP_DialogResetButton),
             self.tr('&Clear Results'))
         self.menu_edit.addSeparator()
         self.menu_copy_only: QMenu = self.menu_edit.addMenu(self.tr('Copy &Only'))
+        self.action_copy_current: QAction = self.menu_copy_only.addAction(self.tr('Active &Cell'))
+        self.menu_copy_only.addSeparator()
         self.action_copy_name: QAction = self.menu_copy_only.addAction(self.tr('&Substance Name'))
         self.action_copy_frequency: QAction = self.menu_copy_only.addAction(self.tr('&Frequency'))
         self.action_copy_intensity: QAction = self.menu_copy_only.addAction(self.tr('&Intensity'))
         self.action_copy_lower_state_energy: QAction = self.menu_copy_only.addAction(
             self.menu_copy_only.tr('&Lower State Energy'))
         self.action_copy: QAction = self.menu_edit.addAction(
             self._icon('edit-copy', 'mdi6.content-copy'),
@@ -54,14 +56,15 @@
         self.menu_edit.addSeparator()
         self.action_substance_info: QAction = self.menu_edit.addAction(
             self._icon('dialog-information', 'mdi6.flask-empty-outline', 'mdi6.information-variant',
                        options=[{}, {'scale_factor': 0.5}]),
             self.tr('Substance &Info'))
 
         self.menu_columns: QMenu = self.addMenu(self.tr('&Columns'))
+        self.action_show_substance: QAction = self.menu_columns.addAction(self.tr('&Substance'))
         self.action_show_frequency: QAction = self.menu_columns.addAction(self.tr('&Frequency'))
         self.action_show_intensity: QAction = self.menu_columns.addAction(self.tr('&Intensity'))
         self.action_show_lower_state_energy: QAction = self.menu_columns.addAction(self.tr('&Lower State Energy'))
 
         self.menu_help: QMenu = self.addMenu(self.tr('&Help'))
         self.action_check_updates: QAction = self.menu_help.addAction(
             self._icon('application-update', 'mdi6.update'),
@@ -85,19 +88,21 @@
         self.action_load.setShortcut('Ctrl+L')
         self.action_quit.setShortcut('Ctrl+Q')
         self.action_about.setShortcut('F1')
         self.action_preferences.setShortcut('Ctrl+,')
         self.action_copy.setShortcut('Ctrl+C')
         self.action_select_all.setShortcut('Ctrl+A')
         self.action_reload.setShortcut('Ctrl+R')
+        self.action_copy_current.setShortcut('Ctrl+Shift+C')
         self.action_copy_name.setShortcut('Ctrl+Shift+C, N')
         self.action_copy_frequency.setShortcut('Ctrl+Shift+C, F')
         self.action_copy_intensity.setShortcut('Ctrl+Shift+C, I')
         self.action_copy_lower_state_energy.setShortcut('Ctrl+Shift+C, E')
         self.action_substance_info.setShortcut('Ctrl+I')
+        self.action_show_substance.setCheckable(True)
         self.action_show_frequency.setCheckable(True)
         self.action_show_intensity.setCheckable(True)
         self.action_show_lower_state_energy.setCheckable(True)
 
     def _icon(self, theme_name: str, *qta_name: str,
               standard_pixmap: QStyle.StandardPixmap | None = None,
               **qta_specs: Any) -> QIcon:
```

### Comparing `pycatsearch-5.1.5/src/pycatsearch/gui/preferences.py` & `pycatsearch-5.1.6/src/pycatsearch/gui/preferences.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import logging
-from contextlib import suppress
 from functools import partial
 from typing import Any, Hashable, cast
 
 from qtpy.QtCore import QByteArray, Qt
-from qtpy.QtGui import QCloseEvent, QIcon
+from qtpy.QtGui import QCloseEvent
 from qtpy.QtWidgets import (QCheckBox, QComboBox, QDialog, QDialogButtonBox, QDoubleSpinBox, QFormLayout, QHBoxLayout,
                             QListWidget, QScrollArea, QSpinBox, QStackedWidget, QVBoxLayout, QWidget, QListWidgetItem)
 
 from .settings import Settings
 
 __all__ = ['Preferences']
 
@@ -85,35 +84,28 @@
         setattr(self.settings, getattr(sender, 'callback'), sender.currentData())
 
 
 class PreferencesBody(QScrollArea):
     """ The main area of the GUI preferences dialog """
 
     def __init__(self, settings: Settings, parent: QWidget | None = None) -> None:
+        from . import icon  # import locally to avoid a circular import
+
         super().__init__(parent)
 
         self.settings: Settings = settings
         logger: logging.Logger = logging.getLogger('preferences')
 
         widget: QWidget = QWidget(self)
         self.setWidget(widget)
         self.setWidgetResizable(True)
         self.setHorizontalScrollBarPolicy(Qt.ScrollBarPolicy.ScrollBarAsNeeded)
         self.setVerticalScrollBarPolicy(Qt.ScrollBarPolicy.ScrollBarAsNeeded)
         self.setFrameStyle(0)
 
-        def icon(*qta_name: str, **qta_specs: Any) -> QIcon:
-            if qta_name:
-                with suppress(ImportError, Exception):
-                    from qtawesome import icon
-
-                    return icon(*qta_name, **qta_specs)  # might raise an `Exception` if the icon is not in the font
-
-            return QIcon()
-
         layout: QHBoxLayout = QHBoxLayout(widget)
         content: QListWidget = QListWidget(widget)
         stack: QStackedWidget = QStackedWidget(widget)
         key: str | tuple[str, tuple[str, ...]] | tuple[str, tuple[str, ...], tuple[tuple[str, Any], ...]]
         value: dict[str, (Settings.CallbackOnly
                           | Settings.SpinboxAndCallback
                           | Settings.ComboboxAndCallback)]
```

### Comparing `pycatsearch-5.1.5/src/pycatsearch/gui/settings.py` & `pycatsearch-5.1.6/src/pycatsearch/gui/settings.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.5/src/pycatsearch/gui/substance_info.py` & `pycatsearch-5.1.6/src/pycatsearch/gui/substance_info.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.5/src/pycatsearch/gui/substances_box.py` & `pycatsearch-5.1.6/src/pycatsearch/gui/substances_box.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 from qtpy.QtCore import QModelIndex, Qt, Slot
-from qtpy.QtWidgets import (QAbstractItemView, QCheckBox, QGroupBox, QLineEdit, QListWidget,
+from qtpy.QtWidgets import (QAbstractItemView, QAbstractScrollArea, QCheckBox, QGroupBox, QLineEdit, QListWidget,
                             QListWidgetItem, QPushButton, QVBoxLayout, QWidget)
 
 from .settings import Settings
 from .substance_info import SubstanceInfo, SubstanceInfoSelector
 from ..catalog import Catalog
 from ..utils import *
 
 __all__ = ['SubstancesBox']
 
 
 class SubstancesBox(QGroupBox):
     def __init__(self, catalog: Catalog, settings: Settings, parent: QWidget | None = None) -> None:
+        from . import icon  # import locally to avoid a circular import
+
         super().__init__(parent)
 
         self._catalog: Catalog = catalog
         self._settings: Settings = settings
         self._selected_substances: set[str] = set()
 
         self._layout_substance: QVBoxLayout = QVBoxLayout(self)
@@ -34,23 +36,26 @@
         self._layout_substance.addWidget(self._text_substance)
         self._list_substance.setEditTriggers(QAbstractItemView.EditTrigger.NoEditTriggers)
         self._list_substance.setDropIndicatorShown(False)
         self._list_substance.setAlternatingRowColors(True)
         self._list_substance.setSelectionMode(QAbstractItemView.SelectionMode.ExtendedSelection)
         self._list_substance.setSelectionBehavior(QAbstractItemView.SelectionBehavior.SelectRows)
         self._list_substance.setSortingEnabled(False)
+        self._list_substance.setSizeAdjustPolicy(QAbstractScrollArea.SizeAdjustPolicy.AdjustToContents)
         self._layout_substance.addWidget(self._list_substance)
         self._check_keep_selection.setStatusTip(
             self._check_keep_selection.tr('Keep substances list selection through filter changes'))
         self._check_keep_selection.setText(self._check_keep_selection.tr('Persistent Selection'))
         self._layout_substance.addWidget(self._check_keep_selection)
         self._button_select_none.setStatusTip(self._button_select_none.tr('Clear substances list selection'))
         self._button_select_none.setText(self._button_select_none.tr('Select None'))
         self._layout_substance.addWidget(self._button_select_none)
 
+        self._button_select_none.setIcon(icon('mdi6.checkbox-blank-off-outline'))
+
         self._text_substance.textChanged.connect(self._on_text_changed)
         self._check_keep_selection.toggled.connect(self._on_check_save_selection_toggled)
         self._button_select_none.clicked.connect(self._on_button_select_none_clicked)
         self._list_substance.doubleClicked.connect(self._on_list_substance_double_clicked)
 
         self.load_settings()
```

### Comparing `pycatsearch-5.1.5/src/pycatsearch/gui/titled_list_widget.py` & `pycatsearch-5.1.6/src/pycatsearch/gui/titled_list_widget.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.5/src/pycatsearch/gui/ui.py` & `pycatsearch-5.1.6/src/pycatsearch/gui/ui.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import math
-from typing import Any, Callable, Final
+from typing import Any, Callable, Final, final
 
-from qtpy.QtCore import QAbstractTableModel, QMimeData, QModelIndex, QPoint, QPointF, QRect, QSize, Qt, Slot
+from qtpy.QtCore import QAbstractTableModel, QByteArray, QMimeData, QModelIndex, QPoint, QPointF, QRect, QSize, Qt, Slot
 from qtpy.QtGui import (QAbstractTextDocumentLayout, QClipboard, QCloseEvent, QCursor, QIcon, QPainter, QPixmap,
                         QScreen, QTextDocument)
-from qtpy.QtWidgets import (QAbstractItemView, QAbstractSpinBox, QApplication, QDoubleSpinBox, QFormLayout, QGridLayout,
-                            QHeaderView, QMainWindow, QMessageBox, QPushButton, QStatusBar, QStyle,
-                            QStyleOptionViewItem, QStyledItemDelegate, QTableView, QTableWidgetSelectionRange, QWidget)
+from qtpy.QtWidgets import (QAbstractItemView, QAbstractSpinBox, QApplication, QDoubleSpinBox, QFormLayout, QHeaderView,
+                            QMainWindow, QMessageBox, QPushButton, QSplitter, QStatusBar, QStyle, QStyleOptionViewItem,
+                            QStyledItemDelegate, QTableView, QVBoxLayout, QWidget)
 from qtpy.compat import getopenfilenames
 
 from .catalog_info import CatalogInfo
 from .download_dialog import DownloadDialog
 from .float_spinbox import FloatSpinBox
 from .frequency_box import FrequencyBox
 from .menu_bar import MenuBar
@@ -26,14 +26,16 @@
 from ..utils import *
 
 __all__ = ['UI']
 
 
 def copy_to_clipboard(text: str, text_type: Qt.TextFormat | str = Qt.TextFormat.PlainText) -> None:
     clipboard: QClipboard = QApplication.clipboard()
+    if not text:
+        return
     mime_data: QMimeData = QMimeData()
     if isinstance(text_type, str):
         mime_data.setData(text_type, text.encode())
     elif text_type == Qt.TextFormat.RichText:
         mime_data.setHtml(wrap_in_html(text))
         mime_data.setText(remove_html(text))
     else:
@@ -265,40 +267,43 @@
         remainder: int = len(self._data) - self._rows_loaded
         items_to_fetch: int = min(remainder, LinesListModel.ROW_BATCH_COUNT)
         self.beginInsertRows(QModelIndex(), self._rows_loaded, self._rows_loaded + items_to_fetch - 1)
         self._rows_loaded += items_to_fetch
         self.endInsertRows()
 
 
+@final
 class UI(QMainWindow):
     def __init__(self, catalog: Catalog,
-                 parent: QWidget = None) -> None:
+                 parent: QWidget | None = None) -> None:
         super().__init__(parent)
         self.catalog: Catalog = catalog
         self.settings: Settings = Settings('SavSoft', 'CatSearch', self)
 
-        self.central_widget: QWidget = QWidget(self)
-        self.layout_main: QGridLayout = QGridLayout(self.central_widget)
-
-        self.layout_options: QFormLayout = QFormLayout()
-        self.spin_intensity: FloatSpinBox = FloatSpinBox(self.central_widget)
-        self.spin_temperature: QDoubleSpinBox = QDoubleSpinBox(self.central_widget)
-
-        self.box_substance: SubstancesBox = SubstancesBox(self.catalog, self.settings, self.central_widget)
-        self.box_frequency: FrequencyBox = FrequencyBox(self.settings, self.central_widget)
-        self.button_search: QPushButton = QPushButton(self.central_widget)
+        self._central_widget: QSplitter = QSplitter(Qt.Orientation.Vertical, self)
+        self._top_matter: QSplitter = QSplitter(Qt.Orientation.Horizontal, self._central_widget)
+        self._right_matter: QWidget = QWidget(self._central_widget)
+
+        self.spin_intensity: FloatSpinBox = FloatSpinBox(self._central_widget)
+        self.spin_temperature: QDoubleSpinBox = QDoubleSpinBox(self._central_widget)
+
+        self.box_substance: SubstancesBox = SubstancesBox(self.catalog, self.settings, self._central_widget)
+        self.box_frequency: FrequencyBox = FrequencyBox(self.settings, self._central_widget)
+        self.button_search: QPushButton = QPushButton(self._central_widget)
 
         self.results_model: LinesListModel = LinesListModel(self.settings, self)
-        self.results_table: QTableView = QTableView(self.central_widget)
+        self.results_table: QTableView = QTableView(self._central_widget)
 
         self.menu_bar: MenuBar = MenuBar(self)
 
         self.status_bar: QStatusBar = QStatusBar(self)
 
         def setup_ui() -> None:
+            from . import icon  # import locally to avoid a circular import
+
             # https://ru.stackoverflow.com/a/1032610
             window_icon: QPixmap = QPixmap()
             window_icon.loadFromData(b'''\
             <svg height="64" width="64" version="1.1">
             <path stroke-linejoin="round" d="m6.722 8.432c-9.05 9.648-6.022 27.23 6.048 33.04 6.269 3.614 13.88 \
             3.1 20-0.1664l20 20c2.013 2.013 5.256 2.013 7.27 0l1.259-1.259c2.013-2.013 2.013-5.256 \
             0-7.27l-19.83-19.83c1.094-1.948 1.868-4.095 2.211-6.403 3.06-13.5-9.72-27.22-23.4-25.12-4.74 \
@@ -308,17 +313,18 @@
             </svg>''')
             self.setWindowIcon(QIcon(window_icon))
 
             if __version__:
                 self.setWindowTitle(self.tr('PyCatSearch (version {0})').format(__version__))
             else:
                 self.setWindowTitle(self.tr('PyCatSearch'))
-            self.setCentralWidget(self.central_widget)
-            self.layout_main.setColumnStretch(0, 1)
-            self.layout_main.setRowStretch(4, 1)
+            self.setCentralWidget(self._central_widget)
+
+            layout_right: QVBoxLayout = QVBoxLayout()
+            layout_options: QFormLayout = QFormLayout()
 
             self.results_table.setModel(self.results_model)
             self.results_table.setItemDelegateForColumn(0, HTMLDelegate())
             self.results_table.setMouseTracking(True)
             self.results_table.setContextMenuPolicy(Qt.ContextMenuPolicy.CustomContextMenu)
             self.results_table.setEditTriggers(QAbstractItemView.EditTrigger.NoEditTriggers)
             self.results_table.setDropIndicatorShown(False)
@@ -329,54 +335,66 @@
             self.results_table.setAlternatingRowColors(True)
             self.results_table.horizontalHeader().setDefaultSectionSize(180)
             self.results_table.horizontalHeader().setHighlightSections(False)
             self.results_table.horizontalHeader().setSectionResizeMode(0, QHeaderView.ResizeMode.Stretch)
             self.results_table.horizontalHeader().setSectionResizeMode(1, QHeaderView.ResizeMode.ResizeToContents)
             self.results_table.horizontalHeader().setSectionResizeMode(2, QHeaderView.ResizeMode.ResizeToContents)
             self.results_table.horizontalHeader().setSectionResizeMode(3, QHeaderView.ResizeMode.ResizeToContents)
+            self.results_table.horizontalHeader().setSectionsMovable(True)
             self.results_table.verticalHeader().setVisible(False)
             self.results_table.verticalHeader().setHighlightSections(False)
-            self.layout_main.addWidget(self.results_table, 4, 0, 1, 3)
 
             # substance selection
-            self.layout_main.addWidget(self.box_substance, 0, 0, 4, 1)
+            self._top_matter.addWidget(self.box_substance)
 
             # frequency limits
-            self.layout_main.addWidget(self.box_frequency, 0, 1, 2, 1)
+            layout_right.addWidget(self.box_frequency, 1)
 
             self.spin_intensity.setAlignment(Qt.AlignmentFlag.AlignRight
                                              | Qt.AlignmentFlag.AlignTrailing
                                              | Qt.AlignmentFlag.AlignVCenter)
             self.spin_intensity.setButtonSymbols(QAbstractSpinBox.ButtonSymbols.NoButtons)
             self.spin_intensity.setDecimals(2)
             self.spin_intensity.setMinimum(-math.inf)
             self.spin_intensity.setMaximum(math.inf)
             self.spin_intensity.setSingleStep(0.1)
             self.spin_intensity.setValue(-6.54)
             self.spin_intensity.setStatusTip(self.spin_intensity.tr('Limit shown spectral lines'))
-            self.layout_options.addRow(self.layout_options.tr('Minimal Intensity:'), self.spin_intensity)
+            layout_options.addRow(layout_options.tr('Minimal Intensity:'), self.spin_intensity)
             self.spin_temperature.setAlignment(Qt.AlignmentFlag.AlignRight
                                                | Qt.AlignmentFlag.AlignTrailing
                                                | Qt.AlignmentFlag.AlignVCenter)
             self.spin_temperature.setButtonSymbols(QAbstractSpinBox.ButtonSymbols.NoButtons)
             self.spin_temperature.setMaximum(999.99)
             self.spin_temperature.setValue(300.0)
             self.spin_temperature.setStatusTip(self.spin_temperature.tr('Temperature to calculate intensity'))
             self.spin_temperature.setSuffix(self.spin_temperature.tr(' K'))
-            self.layout_options.addRow(self.layout_options.tr('Temperature:'), self.spin_temperature)
-            self.layout_main.addLayout(self.layout_options, 2, 1, 1, 1)
+            layout_options.addRow(layout_options.tr('Temperature:'), self.spin_temperature)
+            layout_right.addLayout(layout_options, 0)
 
             self.button_search.setText(self.button_search.tr('Show'))
-            self.layout_main.addWidget(self.button_search, 3, 1, 1, 1)
+            layout_right.addWidget(self.button_search, 0)
+
+            self._right_matter.setLayout(layout_right)
+            self._top_matter.addWidget(self._right_matter)
+            self._top_matter.setStretchFactor(0, 1)
+            self._top_matter.setChildrenCollapsible(False)
+
+            self._central_widget.addWidget(self._top_matter)
+            self._central_widget.addWidget(self.results_table)
+            self._central_widget.setStretchFactor(1, 1)
+            self._central_widget.setChildrenCollapsible(False)
 
             self.setMenuBar(self.menu_bar)
             self.setStatusBar(self.status_bar)
 
             self.button_search.setShortcut('Ctrl+Return')
 
+            self.button_search.setIcon(icon('mdi6.magnify'))
+
             self.adjustSize()
 
         setup_ui()
 
         self.temperature: float = 300.0  # [K]
         self.minimal_intensity: float = -math.inf  # [log10(nm²×MHz)]
 
@@ -403,19 +421,21 @@
         self.menu_bar.action_about.triggered.connect(self._on_action_about_triggered)
         self.menu_bar.action_about_qt.triggered.connect(self._on_action_about_qt_triggered)
         self.menu_bar.action_download_catalog.triggered.connect(self._on_action_download_catalog_triggered)
         self.menu_bar.action_preferences.triggered.connect(self._on_action_preferences_triggered)
         self.menu_bar.action_copy.triggered.connect(self._on_action_copy_triggered)
         self.menu_bar.action_select_all.triggered.connect(self._on_action_select_all_triggered)
         self.menu_bar.action_reload.triggered.connect(self._on_action_reload_triggered)
+        self.menu_bar.action_copy_current.triggered.connect(self._on_action_copy_current_triggered)
         self.menu_bar.action_copy_name.triggered.connect(self._on_action_copy_name_triggered)
         self.menu_bar.action_copy_frequency.triggered.connect(self._on_action_copy_frequency_triggered)
         self.menu_bar.action_copy_intensity.triggered.connect(self._on_action_copy_intensity_triggered)
         self.menu_bar.action_copy_lower_state_energy.triggered.connect(
             self._on_action_copy_lower_state_energy_triggered)
+        self.menu_bar.action_show_substance.toggled.connect(self._on_action_show_substance_toggled)
         self.menu_bar.action_show_frequency.toggled.connect(self._on_action_show_frequency_toggled)
         self.menu_bar.action_show_intensity.toggled.connect(self._on_action_show_intensity_toggled)
         self.menu_bar.action_show_lower_state_energy.toggled.connect(self._on_action_show_lower_state_energy_toggled)
         self.menu_bar.action_substance_info.triggered.connect(self._on_action_substance_info_triggered)
         self.menu_bar.action_clear.triggered.connect(self._on_action_clear_triggered)
 
         if not self.catalog.is_empty:
@@ -480,18 +500,18 @@
 
         def join_file_dialog_formats(_formats: dict[tuple[str, ...], str]) -> str:
             f: tuple[str, ...]
             all_supported_extensions: list[str] = []
             for f in _formats.keys():
                 all_supported_extensions.extend(ensure_prefix(_f, '*') for _f in f)
             format_lines: list[str] = [''.join((
-                    self.tr('All supported', 'file type'),
-                    '(',
-                    ' '.join(ensure_prefix(_f, '*') for _f in all_supported_extensions),
-                    ')'))]
+                self.tr('All supported', 'file type'),
+                '(',
+                ' '.join(ensure_prefix(_f, '*') for _f in all_supported_extensions),
+                ')'))]
             n: str
             for f, n in _formats.items():
                 format_lines.append(''.join((n, '(', ' '.join(ensure_prefix(_f, '*') for _f in f), ')')))
             format_lines.append(self.tr('All files', 'file type') + '(* *.*)')
             return ';;'.join(format_lines)
 
         filename: list[str]
@@ -537,35 +557,55 @@
             self.status_bar.clearMessage()
 
     def stringify_selection_html(self) -> str:
         """
         Convert selected rows to string for copying as rich text
         :return: the rich text representation of the selected table lines
         """
-        text: list[str] = []
-        r: QModelIndex
-        units: dict[int, str] = {
-            1: self.settings.frequency_unit_str,
-            2: self.settings.intensity_unit_str,
-            3: self.settings.energy_unit_str,
-        }
-        for r in self.results_table.selectionModel().selectedRows():
-            row: LinesListModel.DataType = self.results_model.row(r.row())
+        if not self.results_table.selectionModel().selectedRows():
+            return ''
+
+        units: list[str] = [
+            '',
+            self.settings.frequency_unit_str,
+            self.settings.intensity_unit_str,
+            self.settings.energy_unit_str,
+        ]
+        with_units: bool = self.settings.with_units
+
+        def format_value(value: Any, unit: str) -> str:
+            return (self.tr('{value} {unit}', 'format value in html').format(value=value, unit=unit)
+                    if with_units and unit
+                    else self.tr('{value}', 'format value in html').format(value=value))
+
+        columns_order: list[int] = [self.results_table.horizontalHeader().logicalIndex(_c)
+                                    for _c, _a in zip(range(self.results_table.horizontalHeader().count()),
+                                                      self.menu_bar.menu_columns.actions(),
+                                                      strict=True)
+                                    if _a.isChecked()]
+        text: list[str] = ['<table>']
+        values: list[str]
+        index: QModelIndex
+        for index in self.results_table.selectionModel().selectedRows():
+            row: LinesListModel.DataType = self.results_model.row(index.row())
+            values = [
+                format_value(_v, _u)
+                for _u, _v, _a in zip(units,
+                                      (row.name, row.frequency, row.intensity, row.lower_state_energy),
+                                      self.menu_bar.menu_columns.actions(),
+                                      strict=True)
+                if _a.isChecked()
+            ]
             text.append(
                 '<tr><td>' +
-                f'</td>{self.settings.csv_separator}<td>'.join(
-                    [row.name] +
-                    [(str(_c) + ((' ' + units[_i]) if self.settings.with_units and _i in units else ''))
-                     for _i, (_c, _a) in enumerate(zip((row.frequency, row.intensity, row.lower_state_energy),
-                                                       self.menu_bar.menu_columns.actions()))
-                     if _a.isChecked()]
-                ) +
-                '</td></tr>' + self.settings.line_end
+                f'</td>{self.settings.csv_separator}<td>'.join(values[_c] for _c in columns_order) +
+                '</td></tr>'
             )
-        return '<table>' + self.settings.line_end + ''.join(text) + '</table>'
+        text.append('</table>')
+        return self.settings.line_end.join(text)
 
     @Slot()
     def _on_action_download_catalog_triggered(self) -> None:
         downloader: DownloadDialog = DownloadDialog(
             frequency_limits=(self.catalog.min_frequency, self.catalog.max_frequency),
             parent=self)
         downloader.exec()
@@ -593,23 +633,31 @@
         if col >= self.results_model.columnCount():
             return
 
         def html_list(lines: list[str]) -> str:
             return '<ul><li>' + f'</li>{self.settings.line_end}<li>'.join(lines) + '</li></ul>'
 
         text_to_copy: list[str] = []
-        selection: QTableWidgetSelectionRange
-        for row in self.results_table.selectionModel().selectedRows(col):
-            text_to_copy.append(self.results_model.data(row))
+        index: QModelIndex
+        for index in (self.results_table.selectionModel().selectedRows(col)
+                      or [self.results_table.selectionModel().currentIndex()]):
+            if index.isValid():
+                text_to_copy.append(self.results_model.data(index))
+        if not text_to_copy:
+            return
         if col == 0:
             copy_to_clipboard(html_list(text_to_copy), Qt.TextFormat.RichText)
         else:
             copy_to_clipboard(self.settings.line_end.join(text_to_copy), Qt.TextFormat.PlainText)
 
     @Slot()
+    def _on_action_copy_current_triggered(self) -> None:
+        self.copy_selected_items(self.results_table.selectionModel().currentIndex().column())
+
+    @Slot()
     def _on_action_copy_name_triggered(self) -> None:
         self.copy_selected_items(0)
 
     @Slot()
     def _on_action_copy_frequency_triggered(self) -> None:
         self.copy_selected_items(1)
 
@@ -635,20 +683,26 @@
             syn: SubstanceInfo = SubstanceInfo(
                 self.catalog,
                 self.results_model.row(self.results_table.selectionModel().selectedRows()[0].row()).id,
                 self)
             syn.exec()
 
     def toggle_results_table_column_visibility(self, column: int, is_visible: bool) -> None:
+        if is_visible != self.results_table.isColumnHidden(column):
+            return
         if is_visible:
             self.results_table.showColumn(column)
         else:
             self.results_table.hideColumn(column)
 
     @Slot(bool)
+    def _on_action_show_substance_toggled(self, is_checked: bool) -> None:
+        self.toggle_results_table_column_visibility(0, is_checked)
+
+    @Slot(bool)
     def _on_action_show_frequency_toggled(self, is_checked: bool) -> None:
         self.toggle_results_table_column_visibility(1, is_checked)
 
     @Slot(bool)
     def _on_action_show_intensity_toggled(self, is_checked: bool) -> None:
         self.toggle_results_table_column_visibility(2, is_checked)
 
@@ -727,32 +781,36 @@
         self.settings.endArray()
         if not catalog_file_names:
             catalog_file_names = ['catalog.json.gz', 'catalog.json']
         self.temperature = self.settings.value('temperature', self.spin_temperature.value(), float)
         self.minimal_intensity = self.settings.value('intensity', self.spin_intensity.value(), float)
         self.settings.endGroup()
         self.settings.beginGroup('displayedColumns')
+        self.menu_bar.action_show_substance.setChecked(self.settings.value('substance', True, bool))
+        self.toggle_results_table_column_visibility(0, self.menu_bar.action_show_substance.isChecked())
         self.menu_bar.action_show_frequency.setChecked(self.settings.value('frequency', True, bool))
         self.toggle_results_table_column_visibility(1, self.menu_bar.action_show_frequency.isChecked())
         self.menu_bar.action_show_intensity.setChecked(self.settings.value('intensity', True, bool))
         self.toggle_results_table_column_visibility(2, self.menu_bar.action_show_intensity.isChecked())
         self.menu_bar.action_show_lower_state_energy.setChecked(self.settings.value('lowerStateEnergy', False, bool))
         self.toggle_results_table_column_visibility(3, self.menu_bar.action_show_lower_state_energy.isChecked())
+        self.results_table.horizontalHeader().restoreState(self.settings.value('state', QByteArray()))
+        self.results_table.horizontalHeader().restoreGeometry(self.settings.value('geometry', QByteArray()))
         self.settings.endGroup()
         self.settings.beginGroup('window')
         screens: list[QScreen] = QApplication.screens()
         if screens:
             self.move(round(0.5 * (screens[0].size().width() - self.size().width())),
                       round(0.5 * (screens[0].size().height() - self.size().height())))  # Fallback: Center the window
-        window_settings = self.settings.value('geometry')
-        if window_settings is not None:
-            self.restoreGeometry(window_settings)
-        window_settings = self.settings.value('state')
-        if window_settings is not None:
-            self.restoreState(window_settings)
+        self.restoreGeometry(self.settings.value('geometry', QByteArray()))
+        self.restoreState(self.settings.value('state', QByteArray()))
+        self._top_matter.restoreGeometry(self.settings.value('verticalSplitterGeometry', QByteArray()))
+        self._top_matter.restoreState(self.settings.value('verticalSplitterState', QByteArray()))
+        self._central_widget.restoreGeometry(self.settings.value('horizontalSplitterGeometry', QByteArray()))
+        self._central_widget.restoreState(self.settings.value('horizontalSplitterState', QByteArray()))
         self.settings.endGroup()
         self.fill_parameters()
 
         if self.settings.load_last_catalogs:
             self.load_catalog(*catalog_file_names)
 
     def save_settings(self) -> None:
@@ -762,21 +820,28 @@
             self.settings.setArrayIndex(i)
             self.settings.setValue('path', s)
         self.settings.endArray()
         self.settings.setValue('temperature', self.temperature)
         self.settings.setValue('intensity', self.minimal_intensity)
         self.settings.endGroup()
         self.settings.beginGroup('displayedColumns')
+        self.settings.setValue('substance', self.menu_bar.action_show_substance.isChecked())
         self.settings.setValue('frequency', self.menu_bar.action_show_frequency.isChecked())
         self.settings.setValue('intensity', self.menu_bar.action_show_intensity.isChecked())
         self.settings.setValue('lowerStateEnergy', self.menu_bar.action_show_lower_state_energy.isChecked())
+        self.settings.setValue('geometry', self.results_table.horizontalHeader().saveGeometry())
+        self.settings.setValue('state', self.results_table.horizontalHeader().saveState())
         self.settings.endGroup()
         self.settings.beginGroup('window')
         self.settings.setValue('geometry', self.saveGeometry())
         self.settings.setValue('state', self.saveState())
+        self.settings.setValue('verticalSplitterGeometry', self._top_matter.saveGeometry())
+        self.settings.setValue('verticalSplitterState', self._top_matter.saveState())
+        self.settings.setValue('horizontalSplitterGeometry', self._central_widget.saveGeometry())
+        self.settings.setValue('horizontalSplitterState', self._central_widget.saveState())
         self.settings.endGroup()
         self.box_substance.save_settings()
         self.box_frequency.save_settings()
         self.settings.sync()
 
     def preset_table(self) -> None:
         self.results_shown = False
```

### Comparing `pycatsearch-5.1.5/src/pycatsearch/utils.py` & `pycatsearch-5.1.6/src/pycatsearch/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,19 @@
            'within', 'chem_html', 'best_name', 'remove_html', 'wrap_in_html',
            'ensure_prefix', 'all_cases',
            'save_catalog_to_file',
            'ReleaseInfo', 'latest_release', 'update_with_pip']
 
 M_LOG10E: Final[float] = math.log10(math.e)
 
-T0: Final[float] = 300.00
-k: Final[float] = 1.380649000e-23  # https://physics.nist.gov/cgi-bin/cuu/Value?k
-h: Final[float] = 6.626070150e-34  # https://physics.nist.gov/cgi-bin/cuu/Value?h
-e: Final[float] = 1.602176634e-19  # https://physics.nist.gov/cgi-bin/cuu/Value?e
-c: Final[float] = 299792458.00000  # https://physics.nist.gov/cgi-bin/cuu/Value?c
+T0: Final[float] = 300.00  # [K], see https://spec.jpl.nasa.gov/ftp/pub/catalog/doc/catdoc.pdf
+k: Final[float] = 1.380649000e-23  # [J/K],  see https://physics.nist.gov/cgi-bin/cuu/Value?k
+h: Final[float] = 6.626070150e-34  # [J/Hz], see https://physics.nist.gov/cgi-bin/cuu/Value?h
+e: Final[float] = 1.602176634e-19  # [C],    see https://physics.nist.gov/cgi-bin/cuu/Value?e
+c: Final[float] = 299_792_458.000  # [m/s],  see https://physics.nist.gov/cgi-bin/cuu/Value?c
 
 CATALOG: Final[str] = 'catalog'
 BUILD_TIME: Final[str] = 'build_time'
 LINES: Final[str] = 'lines'
 FREQUENCY: Final[str] = 'frequency'
 INTENSITY: Final[str] = 'intensity'
 ID: Final[str] = 'id'
```

### Comparing `pycatsearch-5.1.5/src/pycatsearch.egg-info/PKG-INFO` & `pycatsearch-5.1.6/src/pycatsearch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycatsearch
-Version: 5.1.5
+Version: 5.1.6
 Summary: Yet another implementation of JPL and CDMS spectroscopy catalogs offline search
 Author-email: StSav012 <stsav012@gmail.com>
 License: LGPL-3.0-only
 Project-URL: Source Code, https://github.com/StSav012/pycatsearch
 Project-URL: Bug Tracker, https://github.com/StSav012/pycatsearch/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Win32 (MS Windows)
```

### Comparing `pycatsearch-5.1.5/src/pycatsearch.egg-info/SOURCES.txt` & `pycatsearch-5.1.6/src/pycatsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.5/updater.py` & `pycatsearch-5.1.6/updater.py`

 * *Files identical despite different names*

