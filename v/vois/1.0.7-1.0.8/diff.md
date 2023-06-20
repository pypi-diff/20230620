# Comparing `tmp/vois-1.0.7.tar.gz` & `tmp/vois-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vois-1.0.7.tar", last modified: Fri Jun 16 10:59:41 2023, max compression
+gzip compressed data, was "vois-1.0.8.tar", last modified: Tue Jun 20 05:42:06 2023, max compression
```

## Comparing `vois-1.0.7.tar` & `vois-1.0.8.tar`

### file list

```diff
@@ -1,88 +1,89 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 10:59:41.386439 vois-1.0.7/
--rw-rw-rw-   0        0        0    14155 2023-06-09 08:06:09.000000 vois-1.0.7/LICENCE
--rw-rw-rw-   0        0        0      631 2023-06-09 16:48:21.000000 vois-1.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0    73887 2023-06-09 08:06:09.000000 vois-1.0.7/Notice.txt
--rw-rw-rw-   0        0        0    21433 2023-06-16 10:59:41.384440 vois-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3628 2023-06-16 10:57:43.000000 vois-1.0.7/README.md
--rw-rw-rw-   0        0        0     6091 2023-06-16 10:57:43.000000 vois-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-16 10:59:41.387438 vois-1.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-16 10:59:40.788780 vois-1.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-06-16 10:59:41.018649 vois-1.0.7/src/vois/
--rw-rw-rw-   0        0        0        0 2023-06-09 16:34:02.000000 vois-1.0.7/src/vois/__init__.py
--rw-rw-rw-   0        0        0    11918 2023-06-09 16:34:04.000000 vois-1.0.7/src/vois/colors.py
--rw-rw-rw-   0        0        0     4168 2023-06-09 16:34:04.000000 vois-1.0.7/src/vois/download.py
--rw-rw-rw-   0        0        0    17916 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/eucountries.py
--rw-rw-rw-   0        0        0    10493 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/geojsonUtils.py
--rw-rw-rw-   0        0        0    66667 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/interMap.py
--rw-rw-rw-   0        0        0     9302 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/ipytrees.py
--rw-rw-rw-   0        0        0    35732 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/leafletMap.py
--rw-rw-rw-   0        0        0    29755 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/svgBubblesChart.py
--rw-rw-rw-   0        0        0    11325 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/svgGraph.py
--rw-rw-rw-   0        0        0    18669 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/svgHeatmap.py
--rw-rw-rw-   0        0        0  1033396 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/svgMap.py
--rw-rw-rw-   0        0        0    21956 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/svgPackedCirclesChart.py
--rw-rw-rw-   0        0        0    18049 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/svgRankChart.py
--rw-rw-rw-   0        0        0    48423 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/svgUtils.py
--rw-rw-rw-   0        0        0     7363 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/treemapPlotly.py
--rw-rw-rw-   0        0        0     2290 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/urlOpen.py
--rw-rw-rw-   0        0        0     2017 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/urlUpdate.py
-drwxrwxrwx   0        0        0        0 2023-06-16 10:59:41.360453 vois-1.0.7/src/vois/vuetify/
--rw-rw-rw-   0        0        0        0 2023-06-09 16:34:02.000000 vois-1.0.7/src/vois/vuetify/__init__.py
--rw-rw-rw-   0        0        0    52950 2023-06-13 09:22:47.000000 vois-1.0.7/src/vois/vuetify/app.py
--rw-rw-rw-   0        0        0    43073 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/vuetify/basemaps.py
--rw-rw-rw-   0        0        0    13241 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/vuetify/button.py
--rw-rw-rw-   0        0        0    12779 2023-06-16 10:48:12.000000 vois-1.0.7/src/vois/vuetify/card.py
--rw-rw-rw-   0        0        0    10734 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/vuetify/cardsGrid.py
--rw-rw-rw-   0        0        0     8770 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/vuetify/colorPicker.py
--rw-rw-rw-   0        0        0    10437 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/vuetify/datatable.py
--rw-rw-rw-   0        0        0     7269 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/vuetify/datePicker.py
--rw-rw-rw-   0        0        0     9643 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/vuetify/dialogGeneric.py
--rw-rw-rw-   0        0        0     4250 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/vuetify/dialogMessage.py
--rw-rw-rw-   0        0        0     5785 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/vuetify/dialogWait.py
--rw-rw-rw-   0        0        0     5369 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/vuetify/dialogYesNo.py
-drwxrwxrwx   0        0        0        0 2023-06-16 10:59:41.375445 vois-1.0.7/src/vois/vuetify/extra/
--rw-rw-rw-   0        0        0       47 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/vuetify/extra/__init__.py
--rw-rw-rw-   0        0        0     6838 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/vuetify/extra/file_input.py
--rw-rw-rw-   0        0        0     2251 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/vuetify/extra/file_input.vue
--rw-rw-rw-   0        0        0    12885 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/vuetify/fab.py
--rw-rw-rw-   0        0        0      996 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/vuetify/fontsettings.py
--rw-rw-rw-   0        0        0    13881 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/vuetify/footer.py
--rw-rw-rw-   0        0        0     8029 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/vuetify/label.py
--rw-rw-rw-   0        0        0    48546 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/vuetify/layers.py
--rw-rw-rw-   0        0        0    23017 2023-06-16 10:48:12.000000 vois-1.0.7/src/vois/vuetify/mainPage.py
--rw-rw-rw-   0        0        0     6454 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/vuetify/menu.py
--rw-rw-rw-   0        0        0     7649 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/vuetify/multiSwitch.py
--rw-rw-rw-   0        0        0    56576 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/vuetify/page.py
--rw-rw-rw-   0        0        0    24701 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/vuetify/paletteEditor.py
--rw-rw-rw-   0        0        0    15331 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/vuetify/palettePicker.py
--rw-rw-rw-   0        0        0     8048 2023-06-09 16:34:03.000000 vois-1.0.7/src/vois/vuetify/palettePickerEx.py
--rw-rw-rw-   0        0        0     6284 2023-06-09 16:34:02.000000 vois-1.0.7/src/vois/vuetify/popup.py
--rw-rw-rw-   0        0        0     6181 2023-06-09 16:34:02.000000 vois-1.0.7/src/vois/vuetify/progress.py
--rw-rw-rw-   0        0        0     1821 2023-06-09 16:34:02.000000 vois-1.0.7/src/vois/vuetify/queryStrings.py
--rw-rw-rw-   0        0        0     4708 2023-06-09 16:34:02.000000 vois-1.0.7/src/vois/vuetify/radio.py
--rw-rw-rw-   0        0        0     4390 2023-06-09 16:34:02.000000 vois-1.0.7/src/vois/vuetify/rangeSlider.py
--rw-rw-rw-   0        0        0    17054 2023-06-09 16:34:02.000000 vois-1.0.7/src/vois/vuetify/rangeSliderFloat.py
--rw-rw-rw-   0        0        0     9365 2023-06-09 16:34:02.000000 vois-1.0.7/src/vois/vuetify/selectImage.py
--rw-rw-rw-   0        0        0     6052 2023-06-09 16:34:02.000000 vois-1.0.7/src/vois/vuetify/selectMultiple.py
--rw-rw-rw-   0        0        0     8721 2023-06-09 16:34:02.000000 vois-1.0.7/src/vois/vuetify/selectSingle.py
--rw-rw-rw-   0        0        0     4816 2023-06-09 16:34:02.000000 vois-1.0.7/src/vois/vuetify/settings.py
--rw-rw-rw-   0        0        0     6679 2023-06-09 16:34:02.000000 vois-1.0.7/src/vois/vuetify/sidePanel.py
--rw-rw-rw-   0        0        0     5546 2023-06-09 16:34:02.000000 vois-1.0.7/src/vois/vuetify/slider.py
--rw-rw-rw-   0        0        0    12119 2023-06-09 16:34:02.000000 vois-1.0.7/src/vois/vuetify/sliderFloat.py
--rw-rw-rw-   0        0        0     4590 2023-06-09 16:34:02.000000 vois-1.0.7/src/vois/vuetify/snackbar.py
--rw-rw-rw-   0        0        0    24635 2023-06-09 16:34:02.000000 vois-1.0.7/src/vois/vuetify/sortableList.py
--rw-rw-rw-   0        0        0     6575 2023-06-09 16:34:02.000000 vois-1.0.7/src/vois/vuetify/svgsGrid.py
--rw-rw-rw-   0        0        0     4695 2023-06-09 16:34:02.000000 vois-1.0.7/src/vois/vuetify/switch.py
--rw-rw-rw-   0        0        0     6967 2023-06-09 16:34:02.000000 vois-1.0.7/src/vois/vuetify/tabs.py
--rw-rw-rw-   0        0        0     6369 2023-06-09 16:34:02.000000 vois-1.0.7/src/vois/vuetify/textlist.py
--rw-rw-rw-   0        0        0     7009 2023-06-09 16:34:02.000000 vois-1.0.7/src/vois/vuetify/title.py
--rw-rw-rw-   0        0        0     7465 2023-06-09 16:34:02.000000 vois-1.0.7/src/vois/vuetify/toggle.py
--rw-rw-rw-   0        0        0     3179 2023-06-09 16:34:02.000000 vois-1.0.7/src/vois/vuetify/tooltip.py
--rw-rw-rw-   0        0        0    68877 2023-06-09 16:34:02.000000 vois-1.0.7/src/vois/vuetify/treeview.py
--rw-rw-rw-   0        0        0     5036 2023-06-09 16:34:02.000000 vois-1.0.7/src/vois/vuetify/upload.py
-drwxrwxrwx   0        0        0        0 2023-06-16 10:59:41.076617 vois-1.0.7/src/vois.egg-info/
--rw-rw-rw-   0        0        0    21433 2023-06-16 10:59:40.000000 vois-1.0.7/src/vois.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2188 2023-06-16 10:59:40.000000 vois-1.0.7/src/vois.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 10:59:40.000000 vois-1.0.7/src/vois.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      164 2023-06-16 10:59:40.000000 vois-1.0.7/src/vois.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-16 10:59:40.000000 vois-1.0.7/src/vois.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 05:42:06.153756 vois-1.0.8/
+-rw-rw-rw-   0        0        0    14155 2023-06-09 08:06:09.000000 vois-1.0.8/LICENCE
+-rw-rw-rw-   0        0        0      631 2023-06-09 16:48:21.000000 vois-1.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0    73887 2023-06-09 08:06:09.000000 vois-1.0.8/Notice.txt
+-rw-rw-rw-   0        0        0    21433 2023-06-20 05:42:06.152756 vois-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3628 2023-06-16 10:57:43.000000 vois-1.0.8/README.md
+-rw-rw-rw-   0        0        0     6091 2023-06-20 05:40:20.000000 vois-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-20 05:42:06.154755 vois-1.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-20 05:42:03.117012 vois-1.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-06-20 05:42:04.605162 vois-1.0.8/src/vois/
+-rw-rw-rw-   0        0        0        0 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/__init__.py
+-rw-rw-rw-   0        0        0    11918 2023-06-09 16:34:04.000000 vois-1.0.8/src/vois/colors.py
+-rw-rw-rw-   0        0        0     4168 2023-06-09 16:34:04.000000 vois-1.0.8/src/vois/download.py
+-rw-rw-rw-   0        0        0    17916 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/eucountries.py
+-rw-rw-rw-   0        0        0    10493 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/geojsonUtils.py
+-rw-rw-rw-   0        0        0    66667 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/interMap.py
+-rw-rw-rw-   0        0        0     9302 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/ipytrees.py
+-rw-rw-rw-   0        0        0    35732 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/leafletMap.py
+-rw-rw-rw-   0        0        0    29755 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/svgBubblesChart.py
+-rw-rw-rw-   0        0        0    11325 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/svgGraph.py
+-rw-rw-rw-   0        0        0    18669 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/svgHeatmap.py
+-rw-rw-rw-   0        0        0  1033396 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/svgMap.py
+-rw-rw-rw-   0        0        0    21956 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/svgPackedCirclesChart.py
+-rw-rw-rw-   0        0        0    18049 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/svgRankChart.py
+-rw-rw-rw-   0        0        0    48423 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/svgUtils.py
+-rw-rw-rw-   0        0        0     7363 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/treemapPlotly.py
+-rw-rw-rw-   0        0        0     2290 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/urlOpen.py
+-rw-rw-rw-   0        0        0     2017 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/urlUpdate.py
+drwxrwxrwx   0        0        0        0 2023-06-20 05:42:06.096788 vois-1.0.8/src/vois/vuetify/
+-rw-rw-rw-   0        0        0        0 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/__init__.py
+-rw-rw-rw-   0        0        0    52950 2023-06-13 09:22:47.000000 vois-1.0.8/src/vois/vuetify/app.py
+-rw-rw-rw-   0        0        0    43073 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/basemaps.py
+-rw-rw-rw-   0        0        0    13241 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/button.py
+-rw-rw-rw-   0        0        0    12779 2023-06-16 10:48:12.000000 vois-1.0.8/src/vois/vuetify/card.py
+-rw-rw-rw-   0        0        0    10734 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/cardsGrid.py
+-rw-rw-rw-   0        0        0     8770 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/colorPicker.py
+-rw-rw-rw-   0        0        0    10437 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/datatable.py
+-rw-rw-rw-   0        0        0     7269 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/datePicker.py
+-rw-rw-rw-   0        0        0     9804 2023-06-20 05:40:20.000000 vois-1.0.8/src/vois/vuetify/dialogGeneric.py
+-rw-rw-rw-   0        0        0     4304 2023-06-20 05:40:20.000000 vois-1.0.8/src/vois/vuetify/dialogMessage.py
+-rw-rw-rw-   0        0        0     5785 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/dialogWait.py
+-rw-rw-rw-   0        0        0     5423 2023-06-20 05:40:20.000000 vois-1.0.8/src/vois/vuetify/dialogYesNo.py
+drwxrwxrwx   0        0        0        0 2023-06-20 05:42:06.148757 vois-1.0.8/src/vois/vuetify/extra/
+-rw-rw-rw-   0        0        0       47 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/extra/__init__.py
+-rw-rw-rw-   0        0        0     6838 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/extra/file_input.py
+-rw-rw-rw-   0        0        0     2251 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/extra/file_input.vue
+-rw-rw-rw-   0        0        0    12885 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/fab.py
+-rw-rw-rw-   0        0        0      996 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/fontsettings.py
+-rw-rw-rw-   0        0        0    13881 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/footer.py
+-rw-rw-rw-   0        0        0     5865 2023-06-20 05:40:20.000000 vois-1.0.8/src/vois/vuetify/iconButton.py
+-rw-rw-rw-   0        0        0     8029 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/label.py
+-rw-rw-rw-   0        0        0    48546 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/layers.py
+-rw-rw-rw-   0        0        0    23017 2023-06-16 10:48:12.000000 vois-1.0.8/src/vois/vuetify/mainPage.py
+-rw-rw-rw-   0        0        0     6454 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/menu.py
+-rw-rw-rw-   0        0        0     7649 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/multiSwitch.py
+-rw-rw-rw-   0        0        0    56576 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/page.py
+-rw-rw-rw-   0        0        0    24701 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/paletteEditor.py
+-rw-rw-rw-   0        0        0    15331 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/palettePicker.py
+-rw-rw-rw-   0        0        0     8048 2023-06-09 16:34:03.000000 vois-1.0.8/src/vois/vuetify/palettePickerEx.py
+-rw-rw-rw-   0        0        0     6284 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/popup.py
+-rw-rw-rw-   0        0        0     6181 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/progress.py
+-rw-rw-rw-   0        0        0     1821 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/queryStrings.py
+-rw-rw-rw-   0        0        0     4708 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/radio.py
+-rw-rw-rw-   0        0        0     4390 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/rangeSlider.py
+-rw-rw-rw-   0        0        0    17054 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/rangeSliderFloat.py
+-rw-rw-rw-   0        0        0     9365 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/selectImage.py
+-rw-rw-rw-   0        0        0     6052 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/selectMultiple.py
+-rw-rw-rw-   0        0        0     8721 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/selectSingle.py
+-rw-rw-rw-   0        0        0     4816 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/settings.py
+-rw-rw-rw-   0        0        0     6679 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/sidePanel.py
+-rw-rw-rw-   0        0        0     5546 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/slider.py
+-rw-rw-rw-   0        0        0    12119 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/sliderFloat.py
+-rw-rw-rw-   0        0        0     4590 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/snackbar.py
+-rw-rw-rw-   0        0        0    24635 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/sortableList.py
+-rw-rw-rw-   0        0        0     6575 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/svgsGrid.py
+-rw-rw-rw-   0        0        0     4695 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/switch.py
+-rw-rw-rw-   0        0        0     6967 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/tabs.py
+-rw-rw-rw-   0        0        0     6369 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/textlist.py
+-rw-rw-rw-   0        0        0     7009 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/title.py
+-rw-rw-rw-   0        0        0     7465 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/toggle.py
+-rw-rw-rw-   0        0        0     3179 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/tooltip.py
+-rw-rw-rw-   0        0        0    68877 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/treeview.py
+-rw-rw-rw-   0        0        0     5036 2023-06-09 16:34:02.000000 vois-1.0.8/src/vois/vuetify/upload.py
+drwxrwxrwx   0        0        0        0 2023-06-20 05:42:04.790057 vois-1.0.8/src/vois.egg-info/
+-rw-rw-rw-   0        0        0    21433 2023-06-20 05:42:02.000000 vois-1.0.8/src/vois.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2219 2023-06-20 05:42:03.000000 vois-1.0.8/src/vois.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 05:42:02.000000 vois-1.0.8/src/vois.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      164 2023-06-20 05:42:02.000000 vois-1.0.8/src/vois.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-20 05:42:02.000000 vois-1.0.8/src/vois.egg-info/top_level.txt
```

### Comparing `vois-1.0.7/LICENCE` & `vois-1.0.8/LICENCE`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/MANIFEST.in` & `vois-1.0.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/Notice.txt` & `vois-1.0.8/Notice.txt`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/PKG-INFO` & `vois-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vois
-Version: 1.0.7
+Version: 1.0.8
 Summary: A Python Voilà simplification library
 Author-email: Davide De Marchi <davide.de-marchi@ec.europa.eu>
 Maintainer-email: Davide De Marchi <davide.de-marchi@ec.europa.eu>
 License: Copyright © European Union 2022-2023
         
         
                               EUROPEAN UNION PUBLIC LICENCE v. 1.2
```

### Comparing `vois-1.0.7/README.md` & `vois-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/pyproject.toml` & `vois-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 name = "vois"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.7"  # Required
+version = "1.0.8"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "A Python Voilà simplification library"  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `vois-1.0.7/src/vois/colors.py` & `vois-1.0.8/src/vois/colors.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/download.py` & `vois-1.0.8/src/vois/download.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/eucountries.py` & `vois-1.0.8/src/vois/eucountries.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/geojsonUtils.py` & `vois-1.0.8/src/vois/geojsonUtils.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/interMap.py` & `vois-1.0.8/src/vois/interMap.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/ipytrees.py` & `vois-1.0.8/src/vois/ipytrees.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/leafletMap.py` & `vois-1.0.8/src/vois/leafletMap.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/svgBubblesChart.py` & `vois-1.0.8/src/vois/svgBubblesChart.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/svgGraph.py` & `vois-1.0.8/src/vois/svgGraph.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/svgHeatmap.py` & `vois-1.0.8/src/vois/svgHeatmap.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/svgMap.py` & `vois-1.0.8/src/vois/svgMap.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/svgPackedCirclesChart.py` & `vois-1.0.8/src/vois/svgPackedCirclesChart.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/svgRankChart.py` & `vois-1.0.8/src/vois/svgRankChart.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/svgUtils.py` & `vois-1.0.8/src/vois/svgUtils.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/treemapPlotly.py` & `vois-1.0.8/src/vois/treemapPlotly.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/urlOpen.py` & `vois-1.0.8/src/vois/urlOpen.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/urlUpdate.py` & `vois-1.0.8/src/vois/urlUpdate.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/app.py` & `vois-1.0.8/src/vois/vuetify/app.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/basemaps.py` & `vois-1.0.8/src/vois/vuetify/basemaps.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/button.py` & `vois-1.0.8/src/vois/vuetify/button.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/card.py` & `vois-1.0.8/src/vois/vuetify/card.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/cardsGrid.py` & `vois-1.0.8/src/vois/vuetify/cardsGrid.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/colorPicker.py` & `vois-1.0.8/src/vois/vuetify/colorPicker.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/datatable.py` & `vois-1.0.8/src/vois/vuetify/datatable.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/datePicker.py` & `vois-1.0.8/src/vois/vuetify/datePicker.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/dialogGeneric.py` & `vois-1.0.8/src/vois/vuetify/dialogGeneric.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,16 +45,16 @@
         Color of the title bar of the dialog (default is settings.color_first)
     dark : bool, optional
         Flag that controls the color of the text in foreground (if True, the text will be displayed in white, elsewhere in black)
     show : bool, optional
         Flag to immediately show the dialog-box upon creation (default is False)
     content: list of ipyvuetify widgets, optional
         List of ipyvuietify widgets to be displayed in the body of the dialog-box (default is [])
-    width : int, optional
-        Width in pixel of the dialog-box (default is 500 pixels)
+    width : int or str, optional
+        Width of the dialog-box. If an integer is passed the width is intended in pixels. Default is 500 pixels
     fullscreen : bool, optional
         If True, the dialog-box is opened in fullscreen mode (default is False)
     persistent : bool, optional
         If True, clicking outside of the dialog or pressing esc key will not deactivate it (default is False)
     no_click_animation : bool, optional
         If True, disables the bounce effect when clicking outside of a dialog's content when using the persistent property (default is False)
     addclosebuttons : bool, optional
@@ -161,15 +161,19 @@
         # Dialog
         clist = [toolbar]
         if len(text) > 0:
             clist += [ v.CardText(class_='pa-0 ma-0 mt-9', children=['']) ]
             clist += [ v.CardText(children=[x], class_="mt-n5") for x in vvv ]
         clist += content + r
         
-        self.dialog = v.Dialog(width='%d' % width, v_model=show, fullscreen=fullscreen, transition=transition,
+        if type(width)==int:
+            swidth = "%dpx"%width
+        else:
+            swidth = str(width)
+        self.dialog = v.Dialog(width=swidth, v_model=show, fullscreen=fullscreen, transition=transition,
                                persistent=persistent, no_click_animation=no_click_animation,
                                style_="background-color: transparent; z-index:20001;", 
                                children=[v.Card(children=clist)])
         
         # Display of the dialog
         if not output is None:
             with output:
```

### Comparing `vois-1.0.7/src/vois/vuetify/dialogMessage.py` & `vois-1.0.8/src/vois/vuetify/dialogMessage.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,16 +40,16 @@
         Title of the dialog-box to be displayed in the top toolbar (default is '')
     text : str, optional
         Text to display on top of the dialog-box body (default is '')
     dark : bool, optional
         Flag that controls the color of the text in foreground (if True, the text will be displayed in white, elsewhere in black)
     show : bool, optional
         Flag to immediately show the dialog-box upon creation (default is False)
-    width : int, optional
-        Width in pixel of the dialog-box (default is 500 pixels)
+    width : int or str, optional
+        Width of the dialog-box. If an integer is passed the width is intended in pixels. Default is 500 pixels
     addclosebuttons : bool, optional
         If True, the dialog will have a 'close' button in the top toolbar (default is True)
     transition : str, optional
         Transition to use for the dialog display and close (default is 'dialog-fade-transition'). See: https://vuetifyjs.com/en/styles/transitions/ for a list of available transitions (substitute 'v-' with 'dialog-')
     output : ipywidgets.Output, optional
         Output widget on which the widget has to be displayed
     titleheight : str, optional
```

### Comparing `vois-1.0.7/src/vois/vuetify/dialogWait.py` & `vois-1.0.8/src/vois/vuetify/dialogWait.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/dialogYesNo.py` & `vois-1.0.8/src/vois/vuetify/dialogYesNo.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,16 +44,16 @@
     ----------
     title : str, optional
         Title of the dialog-box to be displayed in the top toolbar (default is '')
     dark : bool, optional
         Flag that controls the color of the text in foreground (if True, the text will be displayed in white, elsewhere in black)
     show : bool, optional
         Flag to immediately show the dialog-box upon creation (default is False)
-    width : int, optional
-        Width in pixel of the dialog-box (default is 500 pixels)
+    width : int or str, optional
+        Width of the dialog-box. If an integer is passed the width is intended in pixels. Default is 500 pixels
     addclosebuttons : bool, optional
         If True, the dialog will have a 'close' button in the top toolbar (default is True)
     transition : str, optional
         Transition to use for the dialog display and close (default is 'dialog-fade-transition'. See: https://vuetifyjs.com/en/styles/transitions/ for a list of available transitions (substitute 'v-' with 'dialog-'')
     output : ipywidgets.Output, optional
         Output widget on which the widget has to be displayed
     titleheight : str, optional
```

### Comparing `vois-1.0.7/src/vois/vuetify/extra/file_input.py` & `vois-1.0.8/src/vois/vuetify/extra/file_input.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/extra/file_input.vue` & `vois-1.0.8/src/vois/vuetify/extra/file_input.vue`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/fab.py` & `vois-1.0.8/src/vois/vuetify/fab.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/fontsettings.py` & `vois-1.0.8/src/vois/vuetify/fontsettings.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/footer.py` & `vois-1.0.8/src/vois/vuetify/footer.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/label.py` & `vois-1.0.8/src/vois/vuetify/label.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/layers.py` & `vois-1.0.8/src/vois/vuetify/layers.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/mainPage.py` & `vois-1.0.8/src/vois/vuetify/mainPage.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/menu.py` & `vois-1.0.8/src/vois/vuetify/menu.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/multiSwitch.py` & `vois-1.0.8/src/vois/vuetify/multiSwitch.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/page.py` & `vois-1.0.8/src/vois/vuetify/page.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/paletteEditor.py` & `vois-1.0.8/src/vois/vuetify/paletteEditor.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/palettePicker.py` & `vois-1.0.8/src/vois/vuetify/palettePicker.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/palettePickerEx.py` & `vois-1.0.8/src/vois/vuetify/palettePickerEx.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/popup.py` & `vois-1.0.8/src/vois/vuetify/popup.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/progress.py` & `vois-1.0.8/src/vois/vuetify/progress.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/queryStrings.py` & `vois-1.0.8/src/vois/vuetify/queryStrings.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/radio.py` & `vois-1.0.8/src/vois/vuetify/radio.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/rangeSlider.py` & `vois-1.0.8/src/vois/vuetify/rangeSlider.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/rangeSliderFloat.py` & `vois-1.0.8/src/vois/vuetify/rangeSliderFloat.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/selectImage.py` & `vois-1.0.8/src/vois/vuetify/selectImage.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/selectMultiple.py` & `vois-1.0.8/src/vois/vuetify/selectMultiple.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/selectSingle.py` & `vois-1.0.8/src/vois/vuetify/selectSingle.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/settings.py` & `vois-1.0.8/src/vois/vuetify/settings.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/sidePanel.py` & `vois-1.0.8/src/vois/vuetify/sidePanel.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/slider.py` & `vois-1.0.8/src/vois/vuetify/slider.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/sliderFloat.py` & `vois-1.0.8/src/vois/vuetify/sliderFloat.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/snackbar.py` & `vois-1.0.8/src/vois/vuetify/snackbar.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/sortableList.py` & `vois-1.0.8/src/vois/vuetify/sortableList.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/svgsGrid.py` & `vois-1.0.8/src/vois/vuetify/svgsGrid.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/switch.py` & `vois-1.0.8/src/vois/vuetify/switch.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/tabs.py` & `vois-1.0.8/src/vois/vuetify/tabs.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/textlist.py` & `vois-1.0.8/src/vois/vuetify/textlist.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/title.py` & `vois-1.0.8/src/vois/vuetify/title.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/toggle.py` & `vois-1.0.8/src/vois/vuetify/toggle.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/tooltip.py` & `vois-1.0.8/src/vois/vuetify/tooltip.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/treeview.py` & `vois-1.0.8/src/vois/vuetify/treeview.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois/vuetify/upload.py` & `vois-1.0.8/src/vois/vuetify/upload.py`

 * *Files identical despite different names*

### Comparing `vois-1.0.7/src/vois.egg-info/PKG-INFO` & `vois-1.0.8/src/vois.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vois
-Version: 1.0.7
+Version: 1.0.8
 Summary: A Python Voilà simplification library
 Author-email: Davide De Marchi <davide.de-marchi@ec.europa.eu>
 Maintainer-email: Davide De Marchi <davide.de-marchi@ec.europa.eu>
 License: Copyright © European Union 2022-2023
         
         
                               EUROPEAN UNION PUBLIC LICENCE v. 1.2
```

### Comparing `vois-1.0.7/src/vois.egg-info/SOURCES.txt` & `vois-1.0.8/src/vois.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 src/vois/vuetify/dialogGeneric.py
 src/vois/vuetify/dialogMessage.py
 src/vois/vuetify/dialogWait.py
 src/vois/vuetify/dialogYesNo.py
 src/vois/vuetify/fab.py
 src/vois/vuetify/fontsettings.py
 src/vois/vuetify/footer.py
+src/vois/vuetify/iconButton.py
 src/vois/vuetify/label.py
 src/vois/vuetify/layers.py
 src/vois/vuetify/mainPage.py
 src/vois/vuetify/menu.py
 src/vois/vuetify/multiSwitch.py
 src/vois/vuetify/page.py
 src/vois/vuetify/paletteEditor.py
```

