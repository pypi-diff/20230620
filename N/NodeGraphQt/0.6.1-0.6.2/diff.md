# Comparing `tmp/NodeGraphQt-0.6.1.tar.gz` & `tmp/NodeGraphQt-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NodeGraphQt-0.6.1.tar", last modified: Sat May 20 11:33:44 2023, max compression
+gzip compressed data, was "NodeGraphQt-0.6.2.tar", last modified: Tue Jun 20 21:52:04 2023, max compression
```

## Comparing `NodeGraphQt-0.6.1.tar` & `NodeGraphQt-0.6.2.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 11:33:44.313837 NodeGraphQt-0.6.1/
--rw-rw-rw-   0        0        0     1102 2021-06-18 10:54:50.000000 NodeGraphQt-0.6.1/LICENSE.md
--rw-rw-rw-   0        0        0       49 2022-05-22 21:37:50.000000 NodeGraphQt-0.6.1/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-20 11:33:43.979762 NodeGraphQt-0.6.1/NodeGraphQt/
--rw-rw-rw-   0        0        0     2469 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.1/NodeGraphQt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 11:33:44.038775 NodeGraphQt-0.6.1/NodeGraphQt/base/
--rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.1/NodeGraphQt/base/__init__.py
--rw-rw-rw-   0        0        0    12642 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.1/NodeGraphQt/base/commands.py
--rw-rw-rw-   0        0        0     2816 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.1/NodeGraphQt/base/factory.py
--rw-rw-rw-   0        0        0   103281 2023-05-20 11:27:20.000000 NodeGraphQt-0.6.1/NodeGraphQt/base/graph.py
--rw-rw-rw-   0        0        0     8273 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.1/NodeGraphQt/base/menu.py
--rw-rw-rw-   0        0        0    20908 2023-05-20 10:49:23.000000 NodeGraphQt-0.6.1/NodeGraphQt/base/model.py
--rw-rw-rw-   0        0        0    15016 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.1/NodeGraphQt/base/node.py
--rw-rw-rw-   0        0        0    16292 2023-05-19 08:52:52.000000 NodeGraphQt-0.6.1/NodeGraphQt/base/port.py
--rw-rw-rw-   0        0        0     7417 2023-05-09 09:46:08.000000 NodeGraphQt-0.6.1/NodeGraphQt/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-20 11:33:44.054778 NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/
--rw-rw-rw-   0        0        0        0 2022-05-08 02:47:52.000000 NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/__init__.py
--rw-rw-rw-   0        0        0    11914 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/nodes_palette.py
--rw-rw-rw-   0        0        0     4749 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/nodes_tree.py
-drwxrwxrwx   0        0        0        0 2023-05-20 11:33:44.114791 NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/
--rw-rw-rw-   0        0        0        0 2022-12-21 22:27:30.000000 NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/__init__.py
--rw-rw-rw-   0        0        0     3550 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py
--rw-rw-rw-   0        0        0     2455 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py
--rw-rw-rw-   0        0        0     4995 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py
--rw-rw-rw-   0        0        0     6304 2022-12-21 22:27:30.000000 NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py
--rw-rw-rw-   0        0        0     2948 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py
--rw-rw-rw-   0        0        0     2489 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py
--rw-rw-rw-   0        0        0    20765 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py
--rw-rw-rw-   0        0        0      761 2022-12-21 22:27:30.000000 NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py
--rw-rw-rw-   0        0        0     7267 2022-12-21 22:27:30.000000 NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py
--rw-rw-rw-   0        0        0      406 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.1/NodeGraphQt/errors.py
-drwxrwxrwx   0        0        0        0 2023-05-20 11:33:44.147800 NodeGraphQt-0.6.1/NodeGraphQt/nodes/
--rw-rw-rw-   0        0        0        0 2022-05-08 02:47:52.000000 NodeGraphQt-0.6.1/NodeGraphQt/nodes/__init__.py
--rw-rw-rw-   0        0        0     4465 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.1/NodeGraphQt/nodes/backdrop_node.py
--rw-rw-rw-   0        0        0    27550 2023-05-20 01:32:47.000000 NodeGraphQt-0.6.1/NodeGraphQt/nodes/base_node.py
--rw-rw-rw-   0        0        0     1253 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.1/NodeGraphQt/nodes/base_node_circle.py
--rw-rw-rw-   0        0        0     5817 2023-05-07 11:27:54.000000 NodeGraphQt-0.6.1/NodeGraphQt/nodes/group_node.py
--rw-rw-rw-   0        0        0     4409 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.1/NodeGraphQt/nodes/port_node.py
--rw-rw-rw-   0        0        0      239 2023-05-20 10:45:33.000000 NodeGraphQt-0.6.1/NodeGraphQt/pkg_info.py
-drwxrwxrwx   0        0        0        0 2023-05-20 11:33:44.221816 NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/
--rw-rw-rw-   0        0        0        0 2021-06-18 10:54:50.000000 NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/__init__.py
--rw-rw-rw-   0        0        0     7060 2023-04-19 08:52:02.000000 NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_abstract.py
--rw-rw-rw-   0        0        0    11022 2023-05-08 10:29:06.000000 NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_backdrop.py
--rw-rw-rw-   0        0        0    37021 2023-05-19 08:52:52.000000 NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_base.py
--rw-rw-rw-   0        0        0    21204 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_circle.py
--rw-rw-rw-   0        0        0    12346 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_group.py
--rw-rw-rw-   0        0        0     4273 2022-05-08 02:47:52.000000 NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_overlay_disabled.py
--rw-rw-rw-   0        0        0     8159 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_port_in.py
--rw-rw-rw-   0        0        0     8158 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_port_out.py
--rw-rw-rw-   0        0        0     3749 2022-05-08 02:47:52.000000 NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_text_item.py
--rw-rw-rw-   0        0        0    23761 2023-05-19 08:52:52.000000 NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/pipe.py
--rw-rw-rw-   0        0        0    10582 2023-04-30 08:29:15.000000 NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/port.py
--rw-rw-rw-   0        0        0     2885 2023-05-03 09:02:56.000000 NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/slicer.py
-drwxrwxrwx   0        0        0        0 2023-05-20 11:33:44.278828 NodeGraphQt-0.6.1/NodeGraphQt/widgets/
--rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.1/NodeGraphQt/widgets/__init__.py
--rw-rw-rw-   0        0        0     3709 2022-12-21 07:01:38.000000 NodeGraphQt-0.6.1/NodeGraphQt/widgets/actions.py
--rw-rw-rw-   0        0        0     1873 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.1/NodeGraphQt/widgets/dialogs.py
-drwxrwxrwx   0        0        0        0 2023-05-20 11:33:44.279829 NodeGraphQt-0.6.1/NodeGraphQt/widgets/icons/
--rw-rw-rw-   0        0        0    17542 2021-06-18 10:54:50.000000 NodeGraphQt-0.6.1/NodeGraphQt/widgets/icons/node_base.png
--rw-rw-rw-   0        0        0     4550 2023-05-03 09:15:23.000000 NodeGraphQt-0.6.1/NodeGraphQt/widgets/node_graph.py
--rw-rw-rw-   0        0        0    14045 2023-05-07 22:11:12.000000 NodeGraphQt-0.6.1/NodeGraphQt/widgets/node_widgets.py
--rw-rw-rw-   0        0        0     5681 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.1/NodeGraphQt/widgets/scene.py
--rw-rw-rw-   0        0        0    11436 2023-05-02 09:54:57.000000 NodeGraphQt-0.6.1/NodeGraphQt/widgets/tab_search.py
--rw-rw-rw-   0        0        0    55886 2023-05-19 08:52:52.000000 NodeGraphQt-0.6.1/NodeGraphQt/widgets/viewer.py
--rw-rw-rw-   0        0        0     6914 2023-05-07 11:27:54.000000 NodeGraphQt-0.6.1/NodeGraphQt/widgets/viewer_nav.py
-drwxrwxrwx   0        0        0        0 2023-05-20 11:33:43.999765 NodeGraphQt-0.6.1/NodeGraphQt.egg-info/
--rw-rw-rw-   0        0        0     2746 2023-05-20 11:33:43.000000 NodeGraphQt-0.6.1/NodeGraphQt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2543 2023-05-20 11:33:43.000000 NodeGraphQt-0.6.1/NodeGraphQt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 11:33:43.000000 NodeGraphQt-0.6.1/NodeGraphQt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-05-20 11:33:43.000000 NodeGraphQt-0.6.1/NodeGraphQt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-20 11:33:43.000000 NodeGraphQt-0.6.1/NodeGraphQt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2746 2023-05-20 11:33:44.313837 NodeGraphQt-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     2042 2023-05-07 23:03:54.000000 NodeGraphQt-0.6.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 11:33:43.946753 NodeGraphQt-0.6.1/examples/
-drwxrwxrwx   0        0        0        0 2023-05-20 11:33:44.286831 NodeGraphQt-0.6.1/examples/hotkeys/
--rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.1/examples/hotkeys/__init__.py
--rw-rw-rw-   0        0        0     6199 2023-05-07 11:27:54.000000 NodeGraphQt-0.6.1/examples/hotkeys/hotkey_functions.py
-drwxrwxrwx   0        0        0        0 2023-05-20 11:33:44.312838 NodeGraphQt-0.6.1/examples/nodes/
--rw-rw-rw-   0        0        0        0 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.1/examples/nodes/__init__.py
--rw-rw-rw-   0        0        0     2157 2023-05-19 07:23:03.000000 NodeGraphQt-0.6.1/examples/nodes/basic_nodes.py
--rw-rw-rw-   0        0        0     3671 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.1/examples/nodes/custom_ports_node.py
--rw-rw-rw-   0        0        0      507 2022-10-18 20:17:59.000000 NodeGraphQt-0.6.1/examples/nodes/group_node.py
--rw-rw-rw-   0        0        0     1822 2023-05-02 10:58:55.000000 NodeGraphQt-0.6.1/examples/nodes/widget_nodes.py
--rw-rw-rw-   0        0        0     1070 2023-05-20 11:33:44.319837 NodeGraphQt-0.6.1/setup.cfg
--rw-rw-rw-   0        0        0      123 2022-12-21 06:31:06.000000 NodeGraphQt-0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 21:52:04.099334 NodeGraphQt-0.6.2/
+-rw-rw-rw-   0        0        0     1102 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/LICENSE.md
+-rw-rw-rw-   0        0        0       49 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-06-20 21:52:04.036828 NodeGraphQt-0.6.2/NodeGraphQt/
+-rw-rw-rw-   0        0        0     2469 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 21:52:04.052456 NodeGraphQt-0.6.2/NodeGraphQt/base/
+-rw-rw-rw-   0        0        0        0 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/base/__init__.py
+-rw-rw-rw-   0        0        0    12642 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/base/commands.py
+-rw-rw-rw-   0        0        0     2816 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/base/factory.py
+-rw-rw-rw-   0        0        0   103281 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/base/graph.py
+-rw-rw-rw-   0        0        0     8273 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/base/menu.py
+-rw-rw-rw-   0        0        0    20908 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/base/model.py
+-rw-rw-rw-   0        0        0    15016 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/base/node.py
+-rw-rw-rw-   0        0        0    16292 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/base/port.py
+-rw-rw-rw-   0        0        0     7417 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/constants.py
+drwxrwxrwx   0        0        0        0 2023-06-20 21:52:04.052456 NodeGraphQt-0.6.2/NodeGraphQt/custom_widgets/
+-rw-rw-rw-   0        0        0        0 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/custom_widgets/__init__.py
+-rw-rw-rw-   0        0        0    11914 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/custom_widgets/nodes_palette.py
+-rw-rw-rw-   0        0        0     4749 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/custom_widgets/nodes_tree.py
+drwxrwxrwx   0        0        0        0 2023-06-20 21:52:04.068082 NodeGraphQt-0.6.2/NodeGraphQt/custom_widgets/properties_bin/
+-rw-rw-rw-   0        0        0        0 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/custom_widgets/properties_bin/__init__.py
+-rw-rw-rw-   0        0        0     3550 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py
+-rw-rw-rw-   0        0        0     2455 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py
+-rw-rw-rw-   0        0        0     4995 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py
+-rw-rw-rw-   0        0        0     6304 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py
+-rw-rw-rw-   0        0        0     2948 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py
+-rw-rw-rw-   0        0        0     2489 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py
+-rw-rw-rw-   0        0        0    20765 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py
+-rw-rw-rw-   0        0        0      761 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py
+-rw-rw-rw-   0        0        0     7267 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py
+-rw-rw-rw-   0        0        0      406 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/errors.py
+drwxrwxrwx   0        0        0        0 2023-06-20 21:52:04.068082 NodeGraphQt-0.6.2/NodeGraphQt/nodes/
+-rw-rw-rw-   0        0        0        0 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/nodes/__init__.py
+-rw-rw-rw-   0        0        0     4465 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/nodes/backdrop_node.py
+-rw-rw-rw-   0        0        0    27550 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/nodes/base_node.py
+-rw-rw-rw-   0        0        0     1253 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/nodes/base_node_circle.py
+-rw-rw-rw-   0        0        0     5817 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/nodes/group_node.py
+-rw-rw-rw-   0        0        0     4409 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/nodes/port_node.py
+-rw-rw-rw-   0        0        0      239 2023-06-20 10:44:12.000000 NodeGraphQt-0.6.2/NodeGraphQt/pkg_info.py
+drwxrwxrwx   0        0        0        0 2023-06-20 21:52:04.083708 NodeGraphQt-0.6.2/NodeGraphQt/qgraphics/
+-rw-rw-rw-   0        0        0        0 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/qgraphics/__init__.py
+-rw-rw-rw-   0        0        0     7060 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/qgraphics/node_abstract.py
+-rw-rw-rw-   0        0        0    11022 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/qgraphics/node_backdrop.py
+-rw-rw-rw-   0        0        0    37021 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/qgraphics/node_base.py
+-rw-rw-rw-   0        0        0    21204 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/qgraphics/node_circle.py
+-rw-rw-rw-   0        0        0    12346 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/qgraphics/node_group.py
+-rw-rw-rw-   0        0        0     4273 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/qgraphics/node_overlay_disabled.py
+-rw-rw-rw-   0        0        0     8159 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/qgraphics/node_port_in.py
+-rw-rw-rw-   0        0        0     8158 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/qgraphics/node_port_out.py
+-rw-rw-rw-   0        0        0     3749 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/qgraphics/node_text_item.py
+-rw-rw-rw-   0        0        0    23782 2023-06-20 10:47:39.000000 NodeGraphQt-0.6.2/NodeGraphQt/qgraphics/pipe.py
+-rw-rw-rw-   0        0        0    10582 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/qgraphics/port.py
+-rw-rw-rw-   0        0        0     2885 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/qgraphics/slicer.py
+drwxrwxrwx   0        0        0        0 2023-06-20 21:52:04.099334 NodeGraphQt-0.6.2/NodeGraphQt/widgets/
+-rw-rw-rw-   0        0        0        0 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3709 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/widgets/actions.py
+-rw-rw-rw-   0        0        0     1873 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/widgets/dialogs.py
+drwxrwxrwx   0        0        0        0 2023-06-20 21:52:04.099334 NodeGraphQt-0.6.2/NodeGraphQt/widgets/icons/
+-rw-rw-rw-   0        0        0    17542 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/widgets/icons/node_base.png
+-rw-rw-rw-   0        0        0     4550 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/widgets/node_graph.py
+-rw-rw-rw-   0        0        0    14045 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/widgets/node_widgets.py
+-rw-rw-rw-   0        0        0     5681 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/widgets/scene.py
+-rw-rw-rw-   0        0        0    11436 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/widgets/tab_search.py
+-rw-rw-rw-   0        0        0    56172 2023-06-20 10:42:34.000000 NodeGraphQt-0.6.2/NodeGraphQt/widgets/viewer.py
+-rw-rw-rw-   0        0        0     6914 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/NodeGraphQt/widgets/viewer_nav.py
+drwxrwxrwx   0        0        0        0 2023-06-20 21:52:04.036828 NodeGraphQt-0.6.2/NodeGraphQt.egg-info/
+-rw-rw-rw-   0        0        0     2746 2023-06-20 21:52:04.000000 NodeGraphQt-0.6.2/NodeGraphQt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2543 2023-06-20 21:52:04.000000 NodeGraphQt-0.6.2/NodeGraphQt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 21:52:04.000000 NodeGraphQt-0.6.2/NodeGraphQt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-06-20 21:52:04.000000 NodeGraphQt-0.6.2/NodeGraphQt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-20 21:52:04.000000 NodeGraphQt-0.6.2/NodeGraphQt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2746 2023-06-20 21:52:04.099334 NodeGraphQt-0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2042 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 21:52:04.036828 NodeGraphQt-0.6.2/examples/
+drwxrwxrwx   0        0        0        0 2023-06-20 21:52:04.099334 NodeGraphQt-0.6.2/examples/hotkeys/
+-rw-rw-rw-   0        0        0        0 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/examples/hotkeys/__init__.py
+-rw-rw-rw-   0        0        0     6199 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/examples/hotkeys/hotkey_functions.py
+drwxrwxrwx   0        0        0        0 2023-06-20 21:52:04.099334 NodeGraphQt-0.6.2/examples/nodes/
+-rw-rw-rw-   0        0        0        0 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/examples/nodes/__init__.py
+-rw-rw-rw-   0        0        0     2320 2023-06-20 10:42:34.000000 NodeGraphQt-0.6.2/examples/nodes/basic_nodes.py
+-rw-rw-rw-   0        0        0     3671 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/examples/nodes/custom_ports_node.py
+-rw-rw-rw-   0        0        0      507 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/examples/nodes/group_node.py
+-rw-rw-rw-   0        0        0     1822 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/examples/nodes/widget_nodes.py
+-rw-rw-rw-   0        0        0     1070 2023-06-20 21:52:04.099334 NodeGraphQt-0.6.2/setup.cfg
+-rw-rw-rw-   0        0        0      123 2023-06-11 21:02:19.000000 NodeGraphQt-0.6.2/setup.py
```

### Comparing `NodeGraphQt-0.6.1/LICENSE.md` & `NodeGraphQt-0.6.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/__init__.py` & `NodeGraphQt-0.6.2/NodeGraphQt/__init__.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/base/commands.py` & `NodeGraphQt-0.6.2/NodeGraphQt/base/commands.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/base/factory.py` & `NodeGraphQt-0.6.2/NodeGraphQt/base/factory.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/base/graph.py` & `NodeGraphQt-0.6.2/NodeGraphQt/base/graph.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/base/menu.py` & `NodeGraphQt-0.6.2/NodeGraphQt/base/menu.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/base/model.py` & `NodeGraphQt-0.6.2/NodeGraphQt/base/model.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/base/node.py` & `NodeGraphQt-0.6.2/NodeGraphQt/base/node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/base/port.py` & `NodeGraphQt-0.6.2/NodeGraphQt/base/port.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/constants.py` & `NodeGraphQt-0.6.2/NodeGraphQt/constants.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/nodes_palette.py` & `NodeGraphQt-0.6.2/NodeGraphQt/custom_widgets/nodes_palette.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/nodes_tree.py` & `NodeGraphQt-0.6.2/NodeGraphQt/custom_widgets/nodes_tree.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py` & `NodeGraphQt-0.6.2/NodeGraphQt/custom_widgets/properties_bin/custom_widget_color_picker.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py` & `NodeGraphQt-0.6.2/NodeGraphQt/custom_widgets/properties_bin/custom_widget_file_paths.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py` & `NodeGraphQt-0.6.2/NodeGraphQt/custom_widgets/properties_bin/custom_widget_slider.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py` & `NodeGraphQt-0.6.2/NodeGraphQt/custom_widgets/properties_bin/custom_widget_value_edit.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py` & `NodeGraphQt-0.6.2/NodeGraphQt/custom_widgets/properties_bin/custom_widget_vectors.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py` & `NodeGraphQt-0.6.2/NodeGraphQt/custom_widgets/properties_bin/node_property_factory.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py` & `NodeGraphQt-0.6.2/NodeGraphQt/custom_widgets/properties_bin/node_property_widgets.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py` & `NodeGraphQt-0.6.2/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_abstract.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py` & `NodeGraphQt-0.6.2/NodeGraphQt/custom_widgets/properties_bin/prop_widgets_base.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/nodes/backdrop_node.py` & `NodeGraphQt-0.6.2/NodeGraphQt/nodes/backdrop_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/nodes/base_node.py` & `NodeGraphQt-0.6.2/NodeGraphQt/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/nodes/base_node_circle.py` & `NodeGraphQt-0.6.2/NodeGraphQt/nodes/base_node_circle.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/nodes/group_node.py` & `NodeGraphQt-0.6.2/NodeGraphQt/nodes/group_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/nodes/port_node.py` & `NodeGraphQt-0.6.2/NodeGraphQt/nodes/port_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_abstract.py` & `NodeGraphQt-0.6.2/NodeGraphQt/qgraphics/node_abstract.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_backdrop.py` & `NodeGraphQt-0.6.2/NodeGraphQt/qgraphics/node_backdrop.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_base.py` & `NodeGraphQt-0.6.2/NodeGraphQt/qgraphics/node_base.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_circle.py` & `NodeGraphQt-0.6.2/NodeGraphQt/qgraphics/node_circle.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_group.py` & `NodeGraphQt-0.6.2/NodeGraphQt/qgraphics/node_group.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_overlay_disabled.py` & `NodeGraphQt-0.6.2/NodeGraphQt/qgraphics/node_overlay_disabled.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_port_in.py` & `NodeGraphQt-0.6.2/NodeGraphQt/qgraphics/node_port_in.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_port_out.py` & `NodeGraphQt-0.6.2/NodeGraphQt/qgraphics/node_port_out.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/node_text_item.py` & `NodeGraphQt-0.6.2/NodeGraphQt/qgraphics/node_text_item.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/pipe.py` & `NodeGraphQt-0.6.2/NodeGraphQt/qgraphics/pipe.py`

 * *Files 0% similar despite different names*

```diff
@@ -426,15 +426,15 @@
         pen = self.pen()
         pen.setWidth(width)
         pen.setColor(QtGui.QColor(*color))
         pen.setStyle(PIPE_STYLES.get(style))
         pen.setJoinStyle(QtCore.Qt.MiterJoin)
         pen.setCapStyle(QtCore.Qt.RoundCap)
         self.setPen(pen)
-        self.setBrush(QtCore.Qt.NoBrush)
+        self.setBrush(QtGui.QBrush(QtGui.QColor(0, 0, 0, 0)))
 
         pen = self._dir_pointer.pen()
         pen.setJoinStyle(QtCore.Qt.MiterJoin)
         pen.setCapStyle(QtCore.Qt.RoundCap)
         pen.setWidth(width)
         pen.setColor(QtGui.QColor(*color))
         self._dir_pointer.setPen(pen)
```

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/port.py` & `NodeGraphQt-0.6.2/NodeGraphQt/qgraphics/port.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/qgraphics/slicer.py` & `NodeGraphQt-0.6.2/NodeGraphQt/qgraphics/slicer.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/widgets/actions.py` & `NodeGraphQt-0.6.2/NodeGraphQt/widgets/actions.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/widgets/dialogs.py` & `NodeGraphQt-0.6.2/NodeGraphQt/widgets/dialogs.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/widgets/icons/node_base.png` & `NodeGraphQt-0.6.2/NodeGraphQt/widgets/icons/node_base.png`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/widgets/node_graph.py` & `NodeGraphQt-0.6.2/NodeGraphQt/widgets/node_graph.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/widgets/node_widgets.py` & `NodeGraphQt-0.6.2/NodeGraphQt/widgets/node_widgets.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/widgets/scene.py` & `NodeGraphQt-0.6.2/NodeGraphQt/widgets/scene.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/widgets/tab_search.py` & `NodeGraphQt-0.6.2/NodeGraphQt/widgets/tab_search.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/widgets/viewer.py` & `NodeGraphQt-0.6.2/NodeGraphQt/widgets/viewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,22 +96,22 @@
         self._rubber_band.isActive = False
 
         text_color = QtGui.QColor(*tuple(map(
             lambda i, j: i - j, (255, 255, 255),
             ViewerEnum.BACKGROUND_COLOR.value
         )))
         text_color.setAlpha(50)
-        self._cusor_text = QtWidgets.QGraphicsTextItem()
-        self._cusor_text.setFlag(self._cusor_text.ItemIsSelectable, False)
-        self._cusor_text.setDefaultTextColor(text_color)
-        self._cusor_text.setZValue(Z_VAL_PIPE - 1)
-        font = self._cusor_text.font()
+        self._cursor_text = QtWidgets.QGraphicsTextItem()
+        self._cursor_text.setFlag(self._cursor_text.ItemIsSelectable, False)
+        self._cursor_text.setDefaultTextColor(text_color)
+        self._cursor_text.setZValue(Z_VAL_PIPE - 1)
+        font = self._cursor_text.font()
         font.setPointSize(7)
-        self._cusor_text.setFont(font)
-        self.scene().addItem(self._cusor_text)
+        self._cursor_text.setFont(font)
+        self.scene().addItem(self._cursor_text)
 
         self._LIVE_PIPE = LivePipeItem()
         self._LIVE_PIPE.setVisible(False)
         self.scene().addItem(self._LIVE_PIPE)
 
         self._SLICER_PIPE = SlicerPipeItem()
         self._SLICER_PIPE.setVisible(False)
@@ -463,15 +463,15 @@
                         selection.add(node)
 
         selection.update(self.selected_nodes())
 
         # update the recorded node positions.
         self._node_positions.update({n: n.xy_pos for n in selection})
 
-        # show selection selection marquee.
+        # show selection marquee.
         if self.LMB_state and not items:
             rect = QtCore.QRect(self._previous_pos, QtCore.QSize())
             rect = rect.normalized()
             map_rect = self.mapToScene(rect).boundingRect()
             self.scene().update(map_rect)
             self._rubber_band.setGeometry(rect)
             self._rubber_band.isActive = True
@@ -484,16 +484,16 @@
         # allow new live pipe with the shift modifier on port that allow
         # for multi connection.
         if self.SHIFT_state:
             if pipes:
                 pipes[0].reset()
                 port = pipes[0].port_from_pos(map_pos, reverse=True)
                 if not port.locked and port.multi_connection:
-                    self._cusor_text.setPlainText('')
-                    self._cusor_text.setVisible(False)
+                    self._cursor_text.setPlainText('')
+                    self._cursor_text.setVisible(False)
                     self.start_live_connection(port)
 
             # return here as the default behaviour unselects nodes with
             # the shift modifier.
             return
 
         if not self._LIVE_PIPE.isVisible():
@@ -589,15 +589,15 @@
             current_pos = self.mapToScene(event.pos())
             delta = previous_pos - current_pos
             self._set_viewer_pan(delta.x(), delta.y())
 
         if not self.ALT_state:
             if self.SHIFT_state or self.CTRL_state:
                 if not self._LIVE_PIPE.isVisible():
-                    self._cusor_text.setPos(self.mapToScene(event.pos()))
+                    self._cursor_text.setPos(self.mapToScene(event.pos()))
 
         if self.LMB_state and self._rubber_band.isActive:
             rect = QtCore.QRect(self._origin_pos, event.pos()).normalized()
             # if the rubber band is too small, do not show it.
             if max(rect.width(), rect.height()) > 5:
                 if not self._rubber_band.isVisible():
                     self._rubber_band.show()
@@ -701,27 +701,27 @@
 
         if self._LIVE_PIPE.isVisible():
             super(NodeViewer, self).keyPressEvent(event)
             return
 
         # show cursor text
         overlay_text = None
-        self._cusor_text.setVisible(False)
+        self._cursor_text.setVisible(False)
         if not self.ALT_state:
             if self.SHIFT_state:
                 overlay_text = '\n    SHIFT:\n    Toggle/Extend Selection'
             elif self.CTRL_state:
                 overlay_text = '\n    CTRL:\n    Deselect Nodes'
         elif self.ALT_state and self.SHIFT_state:
             if self.pipe_slicing:
                 overlay_text = '\n    ALT + SHIFT:\n    Pipe Slicer Enabled'
         if overlay_text:
-            self._cusor_text.setPlainText(overlay_text)
-            self._cusor_text.setPos(self.mapToScene(self._previous_pos))
-            self._cusor_text.setVisible(True)
+            self._cursor_text.setPlainText(overlay_text)
+            self._cursor_text.setPos(self.mapToScene(self._previous_pos))
+            self._cursor_text.setVisible(True)
 
         super(NodeViewer, self).keyPressEvent(event)
 
     def keyReleaseEvent(self, event):
         """
         Key release event re-implemented to update the states for attributes:
         - ALT_state
@@ -733,16 +733,16 @@
         """
         self.ALT_state = event.modifiers() == QtCore.Qt.AltModifier
         self.CTRL_state = event.modifiers() == QtCore.Qt.ControlModifier
         self.SHIFT_state = event.modifiers() == QtCore.Qt.ShiftModifier
         super(NodeViewer, self).keyReleaseEvent(event)
 
         # hide and reset cursor text.
-        self._cusor_text.setPlainText('')
-        self._cusor_text.setVisible(False)
+        self._cursor_text.setPlainText('')
+        self._cursor_text.setVisible(False)
 
     # --- scene events ---
 
     def sceneMouseMoveEvent(self, event):
         """
         triggered mouse move event for the scene.
          - redraw the live connection pipe.
@@ -889,45 +889,52 @@
         if event.button() != QtCore.Qt.MiddleButton:
             self.apply_live_connection(event)
 
     # --- port connections ---
 
     def _validate_accept_connection(self, from_port, to_port):
         """
-        Check if a pipe connection is allowed if there are a constrains set
+        Check if a pipe connection is allowed if there are a constraints set
         on the ports.
 
         Args:
             from_port (PortItem):
             to_port (PortItem):
 
         Returns:
             bool: true to allow connection.
         """
+        accept_validation = []
+
         to_ptype = to_port.port_type
         from_ptype = from_port.port_type
 
-        to_data = self.accept_connection_types.get(to_port.node.type_) or {}
-        constraints = to_data.get(to_ptype, {}).get(to_port.name, {})
-        accept_data = constraints.get(from_port.node.type_, {})
-
-        accepted_pnames = accept_data.get(from_ptype)
-        if accepted_pnames:
-            if from_port.name in accepted_pnames:
-                return True
-            return False
-
+        # validate the start.
         from_data = self.accept_connection_types.get(from_port.node.type_) or {}
         constraints = from_data.get(from_ptype, {}).get(from_port.name, {})
         accept_data = constraints.get(to_port.node.type_, {})
+        accepted_pnames = accept_data.get(to_ptype, {})
+        if constraints:
+            if to_port.name in accepted_pnames:
+                accept_validation.append(True)
+            else:
+                accept_validation.append(False)
 
-        accepted_pnames = accept_data.get(to_ptype)
-        if accepted_pnames:
+        # validate the end.
+        to_data = self.accept_connection_types.get(to_port.node.type_) or {}
+        constraints = to_data.get(to_ptype, {}).get(to_port.name, {})
+        accept_data = constraints.get(from_port.node.type_, {})
+        accepted_pnames = accept_data.get(from_ptype, {})
+        if constraints:
             if from_port.name in accepted_pnames:
-                return True
+                accept_validation.append(True)
+            else:
+                accept_validation.append(False)
+
+        if False in accept_validation:
             return False
         return True
 
     def _validate_reject_connection(self, from_port, to_port):
         """
         Check if a pipe connection is NOT allowed if there are a constrains set
         on the ports.
```

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt/widgets/viewer_nav.py` & `NodeGraphQt-0.6.2/NodeGraphQt/widgets/viewer_nav.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt.egg-info/PKG-INFO` & `NodeGraphQt-0.6.2/NodeGraphQt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NodeGraphQt
-Version: 0.6.1
+Version: 0.6.2
 Summary: Node graph framework for PySide2/PyQt5 that can be
 Home-page: https://github.com/jchanvfx/NodeGraphQt
 Author: Johnny Chan
 License: MIT License
 Project-URL: Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/
 Project-URL: Tracker, https://github.com/jchanvfx/NodeGraphQt/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.6.1 Summary: Node graph
+Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.6.2 Summary: Node graph
 framework for PySide2/PyQt5 that can be Home-page: https://github.com/jchanvfx/
 NodeGraphQt Author: Johnny Chan License: MIT License Project-URL:
 Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/ Project-URL:
 Tracker, https://github.com/jchanvfx/NodeGraphQt/issues Classifier: Operating
 System :: OS Independent Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6 Requires-Python: >=3.6
```

### Comparing `NodeGraphQt-0.6.1/NodeGraphQt.egg-info/SOURCES.txt` & `NodeGraphQt-0.6.2/NodeGraphQt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/PKG-INFO` & `NodeGraphQt-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NodeGraphQt
-Version: 0.6.1
+Version: 0.6.2
 Summary: Node graph framework for PySide2/PyQt5 that can be
 Home-page: https://github.com/jchanvfx/NodeGraphQt
 Author: Johnny Chan
 License: MIT License
 Project-URL: Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/
 Project-URL: Tracker, https://github.com/jchanvfx/NodeGraphQt/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.6.1 Summary: Node graph
+Metadata-Version: 2.1 Name: NodeGraphQt Version: 0.6.2 Summary: Node graph
 framework for PySide2/PyQt5 that can be Home-page: https://github.com/jchanvfx/
 NodeGraphQt Author: Johnny Chan License: MIT License Project-URL:
 Documentation, https://jchanvfx.github.io/NodeGraphQt/api/html/index.html
 Project-URL: Source, https://github.com/jchanvfx/NodeGraphQt/ Project-URL:
 Tracker, https://github.com/jchanvfx/NodeGraphQt/issues Classifier: Operating
 System :: OS Independent Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6 Requires-Python: >=3.6
```

### Comparing `NodeGraphQt-0.6.1/README.md` & `NodeGraphQt-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/examples/hotkeys/hotkey_functions.py` & `NodeGraphQt-0.6.2/examples/hotkeys/hotkey_functions.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/examples/nodes/basic_nodes.py` & `NodeGraphQt-0.6.2/examples/nodes/basic_nodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,21 @@
     NODE_NAME = 'Circle Node'
 
     def __init__(self):
         super(CircleNode, self).__init__()
         self.set_color(10, 24, 38)
 
         # create node inputs
-        self.add_input('in 1')
+        p = self.add_input('in 1')
+        p.add_accept_port_type(
+            port_name='single 1',
+            port_type='out',
+            node_type='nodes.basic.BasicNodeB'
+        )
+
         self.add_input('in 2')
         self.add_input('in 3', multi_input=True)
         self.add_input('in 4', display_name=False)
         self.add_input('in 5', display_name=False)
 
         # create node outputs
         self.add_output('out 1')
```

### Comparing `NodeGraphQt-0.6.1/examples/nodes/custom_ports_node.py` & `NodeGraphQt-0.6.2/examples/nodes/custom_ports_node.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/examples/nodes/widget_nodes.py` & `NodeGraphQt-0.6.2/examples/nodes/widget_nodes.py`

 * *Files identical despite different names*

### Comparing `NodeGraphQt-0.6.1/setup.cfg` & `NodeGraphQt-0.6.2/setup.cfg`

 * *Files identical despite different names*

