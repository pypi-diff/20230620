# Comparing `tmp/voila-vuetify-tuwien-0.6.0.tar.gz` & `tmp/voila-vuetify-tuwien-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voila-vuetify-tuwien-0.6.0.tar", last modified: Mon Jun 19 11:22:59 2023, max compression
+gzip compressed data, was "voila-vuetify-tuwien-0.6.1.tar", last modified: Tue Jun 20 12:44:17 2023, max compression
```

## Comparing `voila-vuetify-tuwien-0.6.0.tar` & `voila-vuetify-tuwien-0.6.1.tar`

### file list

```diff
@@ -1,32 +1,30 @@
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-19 11:22:59.946442 voila-vuetify-tuwien-0.6.0/
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1545 2023-06-16 13:39:42.000000 voila-vuetify-tuwien-0.6.0/LICENSE
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       16 2023-06-16 13:39:42.000000 voila-vuetify-tuwien-0.6.0/MANIFEST.in
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      344 2023-06-19 11:22:59.946442 voila-vuetify-tuwien-0.6.0/PKG-INFO
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1574 2023-06-16 13:39:42.000000 voila-vuetify-tuwien-0.6.0/README.md
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      101 2023-06-19 11:22:59.946442 voila-vuetify-tuwien-0.6.0/setup.cfg
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     3363 2023-06-19 10:26:18.000000 voila-vuetify-tuwien-0.6.0/setup.py
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-19 11:22:59.942443 voila-vuetify-tuwien-0.6.0/share/
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-19 11:22:59.942443 voila-vuetify-tuwien-0.6.0/share/jupyter/
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-19 11:22:59.942443 voila-vuetify-tuwien-0.6.0/share/jupyter/nbconvert/
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-19 11:22:59.942443 voila-vuetify-tuwien-0.6.0/share/jupyter/nbconvert/templates/
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-19 11:22:59.946442 voila-vuetify-tuwien-0.6.0/share/jupyter/nbconvert/templates/static/
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)    15256 2023-06-19 10:05:08.000000 voila-vuetify-tuwien-0.6.0/share/jupyter/nbconvert/templates/static/TU_logo.svg
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-19 11:22:59.946442 voila-vuetify-tuwien-0.6.0/share/jupyter/nbconvert/templates/vuetify-base/
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     7797 2023-06-16 13:39:42.000000 voila-vuetify-tuwien-0.6.0/share/jupyter/nbconvert/templates/vuetify-base/ansi.js
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1434 2023-06-16 13:39:42.000000 voila-vuetify-tuwien-0.6.0/share/jupyter/nbconvert/templates/vuetify-base/app.html
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       25 2023-06-16 13:39:42.000000 voila-vuetify-tuwien-0.6.0/share/jupyter/nbconvert/templates/vuetify-base/conf.json
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     3174 2023-06-19 10:30:10.000000 voila-vuetify-tuwien-0.6.0/share/jupyter/nbconvert/templates/vuetify-base/index.html.j2
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     7280 2023-06-16 13:39:42.000000 voila-vuetify-tuwien-0.6.0/share/jupyter/nbconvert/templates/vuetify-base/util.js
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-19 11:22:59.946442 voila-vuetify-tuwien-0.6.0/share/jupyter/nbconvert/templates/vuetify-default/
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     6406 2023-06-19 11:22:37.000000 voila-vuetify-tuwien-0.6.0/share/jupyter/nbconvert/templates/vuetify-default/app.html
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       40 2023-06-19 09:49:03.000000 voila-vuetify-tuwien-0.6.0/share/jupyter/nbconvert/templates/vuetify-default/conf.json
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-19 11:22:59.942443 voila-vuetify-tuwien-0.6.0/share/jupyter/voila/
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-19 11:22:59.942443 voila-vuetify-tuwien-0.6.0/share/jupyter/voila/templates/
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-19 11:22:59.946442 voila-vuetify-tuwien-0.6.0/share/jupyter/voila/templates/vuetify-base/
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1757 2023-06-16 13:39:42.000000 voila-vuetify-tuwien-0.6.0/share/jupyter/voila/templates/vuetify-base/index.html.j2
-drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-19 11:22:59.946442 voila-vuetify-tuwien-0.6.0/voila_vuetify_tuwien.egg-info/
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      344 2023-06-19 11:22:59.000000 voila-vuetify-tuwien-0.6.0/voila_vuetify_tuwien.egg-info/PKG-INFO
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      780 2023-06-19 11:22:59.000000 voila-vuetify-tuwien-0.6.0/voila_vuetify_tuwien.egg-info/SOURCES.txt
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)        1 2023-06-19 11:22:59.000000 voila-vuetify-tuwien-0.6.0/voila_vuetify_tuwien.egg-info/dependency_links.txt
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       20 2023-06-19 11:22:59.000000 voila-vuetify-tuwien-0.6.0/voila_vuetify_tuwien.egg-info/requires.txt
--rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)        6 2023-06-19 11:22:59.000000 voila-vuetify-tuwien-0.6.0/voila_vuetify_tuwien.egg-info/top_level.txt
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-20 12:44:17.410409 voila-vuetify-tuwien-0.6.1/
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1545 2023-06-16 13:39:42.000000 voila-vuetify-tuwien-0.6.1/LICENSE
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       16 2023-06-16 13:39:42.000000 voila-vuetify-tuwien-0.6.1/MANIFEST.in
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      344 2023-06-20 12:44:17.410409 voila-vuetify-tuwien-0.6.1/PKG-INFO
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1574 2023-06-16 13:39:42.000000 voila-vuetify-tuwien-0.6.1/README.md
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      101 2023-06-20 12:44:17.410409 voila-vuetify-tuwien-0.6.1/setup.cfg
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     3363 2023-06-20 12:44:08.000000 voila-vuetify-tuwien-0.6.1/setup.py
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-20 12:44:17.410409 voila-vuetify-tuwien-0.6.1/share/
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-20 12:44:17.410409 voila-vuetify-tuwien-0.6.1/share/jupyter/
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-20 12:44:17.410409 voila-vuetify-tuwien-0.6.1/share/jupyter/nbconvert/
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-20 12:44:17.410409 voila-vuetify-tuwien-0.6.1/share/jupyter/nbconvert/templates/
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-20 12:44:17.410409 voila-vuetify-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     7797 2023-06-16 13:39:42.000000 voila-vuetify-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/ansi.js
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1434 2023-06-16 13:39:42.000000 voila-vuetify-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/app.html
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       25 2023-06-19 13:49:52.000000 voila-vuetify-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/conf.json
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     3209 2023-06-20 12:43:26.000000 voila-vuetify-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/index.html.j2
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     7280 2023-06-16 13:39:42.000000 voila-vuetify-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/util.js
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-20 12:44:17.410409 voila-vuetify-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-default-tuwien/
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     6408 2023-06-20 10:49:16.000000 voila-vuetify-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-default-tuwien/app.html
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       40 2023-06-20 11:41:15.000000 voila-vuetify-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-default-tuwien/conf.json
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-20 12:44:17.410409 voila-vuetify-tuwien-0.6.1/share/jupyter/voila/
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-20 12:44:17.410409 voila-vuetify-tuwien-0.6.1/share/jupyter/voila/templates/
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-20 12:44:17.410409 voila-vuetify-tuwien-0.6.1/share/jupyter/voila/templates/vuetify-base-tuwien/
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)     1764 2023-06-20 12:16:19.000000 voila-vuetify-tuwien-0.6.1/share/jupyter/voila/templates/vuetify-base-tuwien/index.html.j2
+drwxrwxr-x   0 mpetojevic  (1000) mpetojevic  (1000)        0 2023-06-20 12:44:17.410409 voila-vuetify-tuwien-0.6.1/voila_vuetify_tuwien.egg-info/
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      344 2023-06-20 12:44:17.000000 voila-vuetify-tuwien-0.6.1/voila_vuetify_tuwien.egg-info/PKG-INFO
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)      783 2023-06-20 12:44:17.000000 voila-vuetify-tuwien-0.6.1/voila_vuetify_tuwien.egg-info/SOURCES.txt
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)        1 2023-06-20 12:44:17.000000 voila-vuetify-tuwien-0.6.1/voila_vuetify_tuwien.egg-info/dependency_links.txt
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)       20 2023-06-20 12:44:17.000000 voila-vuetify-tuwien-0.6.1/voila_vuetify_tuwien.egg-info/requires.txt
+-rw-rw-r--   0 mpetojevic  (1000) mpetojevic  (1000)        6 2023-06-20 12:44:17.000000 voila-vuetify-tuwien-0.6.1/voila_vuetify_tuwien.egg-info/top_level.txt
```

### Comparing `voila-vuetify-tuwien-0.6.0/LICENSE` & `voila-vuetify-tuwien-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `voila-vuetify-tuwien-0.6.0/README.md` & `voila-vuetify-tuwien-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `voila-vuetify-tuwien-0.6.0/setup.py` & `voila-vuetify-tuwien-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 for (dirpath, dirnames, filenames) in os.walk('share/jupyter/'):
     if filenames:
         data_files.append((dirpath, [os.path.join(dirpath, filename) for filename in filenames]))
 
 
 setup(
     name='voila-vuetify-tuwien',
-    version="0.6.0",
+    version="0.6.1",
     description="TU Wien vuetify template for Voila",
     data_files=data_files,
     install_requires=['voila>=0.2.1,<0.6.0'],
     include_package_data=True,
     author=['Voila Development Team', "Marijana Petojevic"],
     url='https://gitlab.tuwien.ac.at/hpc/datalab/jupyter/voila/voila-vuetify-tu-wien-template',
     keywords=[
```

### Comparing `voila-vuetify-tuwien-0.6.0/share/jupyter/nbconvert/templates/vuetify-base/ansi.js` & `voila-vuetify-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/ansi.js`

 * *Files identical despite different names*

### Comparing `voila-vuetify-tuwien-0.6.0/share/jupyter/nbconvert/templates/vuetify-base/app.html` & `voila-vuetify-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/app.html`

 * *Files identical despite different names*

### Comparing `voila-vuetify-tuwien-0.6.0/share/jupyter/nbconvert/templates/vuetify-base/index.html.j2` & `voila-vuetify-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/index.html.j2`

 * *Files 6% similar despite different names*

```diff
@@ -44,33 +44,33 @@
         app.loading_text = 'Already executed'
         app.loadingPercentage = 100;
         app.loading = false;
     </script>
     {% endblock cell_generator %}
 
     <script>
-        {% if 'jupyter-vuetify/extension' in resources.nbextensions-%}
+        {% if 'jupyter-vuetify-tuwien/extension' in resources.nbextensions-%}
         window.enable_nbextensions = true;
         {% endif-%}
         requirejs.config({
             baseUrl: '{{resources.base_url}}voila',
             waitSeconds: 3000,
             map: {
                 '*': {
                     {% if 'jupyter-vue/extension' in resources.nbextensions-%}
                     'jupyter-vue': 'nbextensions/jupyter-vue/nodeps',
                     {% endif-%}
-                    {% if 'jupyter-vuetify/extension' in resources.nbextensions-%}
-                    'jupyter-vuetify': 'nbextensions/jupyter-vuetify/nodeps',
+                    {% if 'jupyter-vuetify-tuwien/extension' in resources.nbextensions-%}
+                    'jupyter-vuetify-tuwien': 'nbextensions/jupyter-vuetify-tuwien/nodeps',
                     {% endif-%}
                 },
             }
         });
         requirejs([
-            {% for ext in resources.nbextensions if ext != 'jupyter-vuetify/extension' and ext != 'jupyter-vue/extension'-%}
+            {% for ext in resources.nbextensions if ext != 'jupyter-vuetify-tuwien/extension' and ext != 'jupyter-vue/extension'-%}
                 "{{resources.base_url}}voila/nbextensions/{{ ext }}.js",
             {% endfor %}
         ]);
         requirejs(['static/voila'], (voila) => init(voila));
     </script>
 </html>
```

### Comparing `voila-vuetify-tuwien-0.6.0/share/jupyter/nbconvert/templates/vuetify-base/util.js` & `voila-vuetify-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-base-tuwien/util.js`

 * *Files identical despite different names*

### Comparing `voila-vuetify-tuwien-0.6.0/share/jupyter/nbconvert/templates/vuetify-default/app.html` & `voila-vuetify-tuwien-0.6.1/share/jupyter/nbconvert/templates/vuetify-default-tuwien/app.html`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             <v-layout v-show="!loading">
                 <v-navigation-drawer v-model="showNavBar" app>
                     <v-toolbar flat>
                         <v-list>
                             <v-list-item>
                                 <v-list-item-title class="title">
                                     <jupyter-widget-mount-point mount-id="content-title">
-                                        Navigation 
+                                        My Navigation
                                     </jupyter-widget-mount-point>
                                 </v-list-item-title>
                             </v-list-item>
                         </v-list>
                     </v-toolbar>
 
                     <v-divider></v-divider>
```

### Comparing `voila-vuetify-tuwien-0.6.0/share/jupyter/voila/templates/vuetify-base/index.html.j2` & `voila-vuetify-tuwien-0.6.1/share/jupyter/voila/templates/vuetify-base-tuwien/index.html.j2`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{%- extends 'nbconvert/templates/vuetify-base/index.html.j2' -%}
+{%- extends 'nbconvert/templates/vuetify-base-tuwien/index.html.j2' -%}
 {% block notebook_execute %}
 
 {%- set kernel_id = kernel_start(nb) -%}
     <script id="jupyter-config-data" type="application/json">
         {
             "baseUrl": "{{resources.base_url}}",
             "kernelId": "{{kernel_id}}"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{%- extends 'nbconvert/templates/vuetify-base/index.html.j2' -%} {% block
-notebook_execute %} {%- set kernel_id = kernel_start(nb) -%}
+{%- extends 'nbconvert/templates/vuetify-base-tuwien/index.html.j2' -%} {%
+block notebook_execute %} {%- set kernel_id = kernel_start(nb) -%}
  {% endblock notebook_execute %} {% block cell_generator %}
  {% for cell in cell_generator(nb, kernel_id) %}
  {% if cell.cell_type == 'code' %} {% for output in cell.outputs %} {% if
 output.output_type == 'error' %}
  {% endif %} {% endfor %} {% endif %} {% endfor %} {% endblock cell_generator
 %}
```

