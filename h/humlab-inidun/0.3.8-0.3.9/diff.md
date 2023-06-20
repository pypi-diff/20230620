# Comparing `tmp/humlab-inidun-0.3.8.tar.gz` & `tmp/humlab-inidun-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "humlab-inidun-0.3.8.tar", max compression
+gzip compressed data, was "humlab-inidun-0.3.9.tar", max compression
```

## Comparing `humlab-inidun-0.3.8.tar` & `humlab-inidun-0.3.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       88 2021-03-15 20:16:23.530000 humlab-inidun-0.3.8/README.md
--rw-r--r--   0        0        0      639 2021-05-06 11:31:28.689594 humlab-inidun-0.3.8/__paths__.py
--rw-r--r--   0        0        0        0 2021-03-15 20:16:29.330000 humlab-inidun-0.3.8/notebooks/__init__.py
--rw-r--r--   0        0        0        0 2021-03-15 20:16:29.250000 humlab-inidun-0.3.8/notebooks/co_occurrence/__init__.py
--rw-r--r--   0        0        0     8297 2021-10-11 09:19:39.398360 humlab-inidun-0.3.8/notebooks/co_occurrence/co_occurrence_trends.ipynb
--rw-r--r--   0        0        0     7273 2021-10-11 09:19:39.398360 humlab-inidun-0.3.8/notebooks/co_occurrence/co_occurrence_trends.py
--rw-r--r--   0        0        0        0 2021-03-15 20:16:29.310000 humlab-inidun-0.3.8/notebooks/common/__init__.py
--rw-r--r--   0        0        0      174 2021-05-28 10:10:52.218961 humlab-inidun-0.3.8/notebooks/common/utils.py
--rw-r--r--   0        0        0        0 2021-03-15 20:16:29.270000 humlab-inidun-0.3.8/notebooks/most_discriminating_words/__init__.py
--rw-r--r--   0        0        0     1203 2021-10-11 09:19:39.418360 humlab-inidun-0.3.8/notebooks/most_discriminating_words/most_discriminating_terms.ipynb
--rw-r--r--   0        0        0      787 2021-10-11 09:19:39.418360 humlab-inidun-0.3.8/notebooks/most_discriminating_words/most_discriminating_terms.py
--rw-r--r--   0        0        0        0 2021-03-15 20:16:29.290000 humlab-inidun-0.3.8/notebooks/pos_statistics/__init__.py
--rw-r--r--   0        0        0     2269 2021-10-11 09:19:39.438360 humlab-inidun-0.3.8/notebooks/pos_statistics/pos_statistics.ipynb
--rw-r--r--   0        0        0     1762 2021-10-11 09:19:39.438360 humlab-inidun-0.3.8/notebooks/pos_statistics/pos_statistics.py
--rw-r--r--   0        0        0     7526 2021-10-11 09:19:39.518360 humlab-inidun-0.3.8/notebooks/topic_modelling/explore_topic_models.ipynb
--rw-r--r--   0        0        0     4478 2021-10-11 09:19:39.518360 humlab-inidun-0.3.8/notebooks/topic_modelling/explore_topic_models.py
--rw-r--r--   0        0        0        0 2021-03-15 20:16:29.330000 humlab-inidun-0.3.8/notebooks/word_trends/__init__.py
--rw-r--r--   0        0        0     6616 2021-10-11 09:19:39.538360 humlab-inidun-0.3.8/notebooks/word_trends/word_trends.ipynb
--rw-r--r--   0        0        0     5660 2021-10-11 09:19:39.538360 humlab-inidun-0.3.8/notebooks/word_trends/word_trends.py
--rw-r--r--   0        0        0     2819 2021-10-11 09:19:46.128360 humlab-inidun-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     1102 2021-10-11 09:19:48.935828 humlab-inidun-0.3.8/setup.py
--rw-r--r--   0        0        0     1062 2021-10-11 09:19:48.936097 humlab-inidun-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0       88 2021-03-15 20:16:23.530000 humlab-inidun-0.3.9/README.md
+-rw-r--r--   0        0        0      639 2021-05-06 11:31:28.689594 humlab-inidun-0.3.9/__paths__.py
+-rw-r--r--   0        0        0        0 2021-03-15 20:16:29.330000 humlab-inidun-0.3.9/notebooks/__init__.py
+-rw-r--r--   0        0        0        0 2021-03-15 20:16:29.250000 humlab-inidun-0.3.9/notebooks/co_occurrence/__init__.py
+-rw-r--r--   0        0        0     8297 2021-10-17 09:25:11.422640 humlab-inidun-0.3.9/notebooks/co_occurrence/co_occurrence_trends.ipynb
+-rw-r--r--   0        0        0     7273 2021-10-17 09:25:11.422640 humlab-inidun-0.3.9/notebooks/co_occurrence/co_occurrence_trends.py
+-rw-r--r--   0        0        0        0 2021-03-15 20:16:29.310000 humlab-inidun-0.3.9/notebooks/common/__init__.py
+-rw-r--r--   0        0        0      174 2021-05-28 10:10:52.218961 humlab-inidun-0.3.9/notebooks/common/utils.py
+-rw-r--r--   0        0        0        0 2021-03-15 20:16:29.270000 humlab-inidun-0.3.9/notebooks/most_discriminating_words/__init__.py
+-rw-r--r--   0        0        0     1203 2021-10-17 09:25:11.432640 humlab-inidun-0.3.9/notebooks/most_discriminating_words/most_discriminating_terms.ipynb
+-rw-r--r--   0        0        0      787 2021-10-17 09:25:11.432640 humlab-inidun-0.3.9/notebooks/most_discriminating_words/most_discriminating_terms.py
+-rw-r--r--   0        0        0        0 2021-03-15 20:16:29.290000 humlab-inidun-0.3.9/notebooks/pos_statistics/__init__.py
+-rw-r--r--   0        0        0     2269 2021-10-17 09:25:11.452640 humlab-inidun-0.3.9/notebooks/pos_statistics/pos_statistics.ipynb
+-rw-r--r--   0        0        0     1762 2021-10-17 09:25:11.452640 humlab-inidun-0.3.9/notebooks/pos_statistics/pos_statistics.py
+-rw-r--r--   0        0        0     7526 2021-10-17 09:25:11.542640 humlab-inidun-0.3.9/notebooks/topic_modelling/explore_topic_models.ipynb
+-rw-r--r--   0        0        0     4478 2021-10-17 09:25:11.542640 humlab-inidun-0.3.9/notebooks/topic_modelling/explore_topic_models.py
+-rw-r--r--   0        0        0        0 2021-03-15 20:16:29.330000 humlab-inidun-0.3.9/notebooks/word_trends/__init__.py
+-rw-r--r--   0        0        0     6616 2021-10-17 09:25:11.552640 humlab-inidun-0.3.9/notebooks/word_trends/word_trends.ipynb
+-rw-r--r--   0        0        0     5660 2021-10-17 09:25:11.552640 humlab-inidun-0.3.9/notebooks/word_trends/word_trends.py
+-rw-r--r--   0        0        0     2819 2021-10-17 09:25:18.522640 humlab-inidun-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     1102 2021-10-17 09:25:20.203264 humlab-inidun-0.3.9/setup.py
+-rw-r--r--   0        0        0     1062 2021-10-17 09:25:20.203493 humlab-inidun-0.3.9/PKG-INFO
```

### Comparing `humlab-inidun-0.3.8/__paths__.py` & `humlab-inidun-0.3.9/__paths__.py`

 * *Files identical despite different names*

### Comparing `humlab-inidun-0.3.8/notebooks/co_occurrence/co_occurrence_trends.ipynb` & `humlab-inidun-0.3.9/notebooks/co_occurrence/co_occurrence_trends.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9878472222222222%*

 * *Differences: {"'cells'": "{0: {'id': 'fa7665cf'}, 1: {'id': '104314c1'}, 2: {'id': '4a39358d'}}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "9956aaa0",
+            "id": "fa7665cf",
             "metadata": {},
             "source": [
                 "### Overview\n",
                 "\n",
                 "This notebook implements a processing pipeline from computes word co-occurrences from plain text. The term-term co-occurrence matrix is transformed into a DTM corpus that has a vocabulary consisting of token-pairs. The co-occurring word trends can hence be xxplored using the ordinary word trends analysis tools.\n",
                 "\n",
                 "For large corpora the processing time can be considerable and in such a case you\n",
@@ -90,15 +90,15 @@
                 "\n",
                 "The \"words\" in this case are co-occurrence pairs and to find instances matching \"information\" you could enter ```information*```, ```*information``` or ```*information*``` to match pairs starting with information, ending with information or containing information respectively."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "41d423a8",
+            "id": "104314c1",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from bokeh.plotting import output_notebook\n",
                 "from IPython.core.display import display\n",
                 "from penelope.notebook.co_occurrence import MainGUI\n",
                 "\n",
@@ -113,15 +113,15 @@
                 ")\n",
                 "display(gui.layout())"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "4fa87f81",
+            "id": "4a39358d",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "jupytext": {
```

### Comparing `humlab-inidun-0.3.8/notebooks/co_occurrence/co_occurrence_trends.py` & `humlab-inidun-0.3.9/notebooks/co_occurrence/co_occurrence_trends.py`

 * *Files identical despite different names*

### Comparing `humlab-inidun-0.3.8/notebooks/most_discriminating_words/most_discriminating_terms.ipynb` & `humlab-inidun-0.3.9/notebooks/most_discriminating_words/most_discriminating_terms.ipynb`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9878472222222222%*

 * *Differences: {"'cells'": "{0: {'id': '62ee0d2f'}, 1: {'id': 'd429361f'}, 2: {'id': '17f01dde'}}"}*

```diff
@@ -1,25 +1,25 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "46adc2c1",
+            "id": "62ee0d2f",
             "metadata": {},
             "source": [
                 "## Most Discriminating Terms\n",
                 "References:\n",
                 "    King, Gary, Patrick Lam, and Margaret Roberts. \"Computer-Assisted Keyword\n",
                 "    and Document Set Discovery from Unstructured Text.\" (2014).\n",
                 "    http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.458.1445&rep=rep1&type=pdf"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "647299cc",
+            "id": "d429361f",
             "metadata": {
                 "lines_to_next_cell": 0
             },
             "outputs": [],
             "source": [
                 "\n",
                 "from IPython.display import display\n",
@@ -31,15 +31,15 @@
                 "\n",
                 "display(gui)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "68e3352e",
+            "id": "17f01dde",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "jupytext": {
```

### Comparing `humlab-inidun-0.3.8/notebooks/most_discriminating_words/most_discriminating_terms.py` & `humlab-inidun-0.3.9/notebooks/most_discriminating_words/most_discriminating_terms.py`

 * *Files identical despite different names*

### Comparing `humlab-inidun-0.3.8/notebooks/pos_statistics/pos_statistics.ipynb` & `humlab-inidun-0.3.9/notebooks/pos_statistics/pos_statistics.ipynb`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9878472222222222%*

 * *Differences: {"'cells'": "{0: {'id': '5018cfdc'}, 1: {'id': '06d8b11d'}, 2: {'id': '9d3e6552'}}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "a954f454",
+            "id": "5018cfdc",
             "metadata": {},
             "source": [
                 "# Token Count Statistics\n",
                 "### Text Processing Pipeline\n",
                 "\n",
                 "| | Building block | Arguments | Description |\n",
                 "| -- | :------------- | :------------- | :------------- |\n",
@@ -20,15 +20,15 @@
                 "Note: The dcument index file is either a pre-existing document index or, if no such index exists, automatically generated during the initial text loading pipeline task.\n",
                 "If no pre-existing file exists, then the necessary attributes (e.g. document's year) are extracted from the filename of each  document."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "aa8a0608",
+            "id": "06d8b11d",
             "metadata": {
                 "lines_to_next_cell": 0,
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "from IPython.core.display import display\n",
@@ -41,15 +41,15 @@
                 ")\n",
                 "display(gui.layout())"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "78e833cc",
+            "id": "9d3e6552",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "jupytext": {
```

### Comparing `humlab-inidun-0.3.8/notebooks/pos_statistics/pos_statistics.py` & `humlab-inidun-0.3.9/notebooks/pos_statistics/pos_statistics.py`

 * *Files identical despite different names*

### Comparing `humlab-inidun-0.3.8/notebooks/topic_modelling/explore_topic_models.ipynb` & `humlab-inidun-0.3.9/notebooks/topic_modelling/explore_topic_models.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9870833333333333%*

 * *Differences: {"'cells'": "{0: {'id': 'cc004496'}, 1: {'id': '4daefb15'}, 2: {'id': 'ee890472'}, 3: {'id': "*

 * *            "'e1412ac0'}, 4: {'id': 'aba6d243'}, 5: {'id': '62009824'}, 6: {'id': 'b6323cc6'}, 7: "*

 * *            "{'id': 'cf5c0854'}, 8: {'id': '3b833fd9'}, 9: {'id': 'ecf4c552'}, 10: {'id': "*

 * *            "'9a5616d2'}, 11: {'id': 'f93c8772'}, 12: {'id': '8bdfc245'}, 13: {'id': 'c0f81cab'}, "*

 * *            "14: {'id': '5db26ca2'}, 15: {'id': '400d951d'}, 16: {'id': 'd2611044'}, 17: {'id': "*

 * *            "'74725f5a'}, 1 […]*

```diff
@@ -1,22 +1,22 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "0a177c41",
+            "id": "cc004496",
             "metadata": {},
             "source": [
                 "## Text Analysis - Topic Modelling\n",
                 "### <span style='color: green'>SETUP </span> Prepare and Setup Notebook <span style='float: right; color: red'>MANDATORY</span>"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "b6d497fe",
+            "id": "4daefb15",
             "metadata": {},
             "outputs": [],
             "source": [
                 "\n",
                 "import os\n",
                 "from typing import Callable\n",
                 "\n",
@@ -34,232 +34,232 @@
                 "current_state: Callable[[], gui.TopicModelContainer] = gui.TopicModelContainer.singleton\n",
                 "corpus_folder: str = \"/data/inidun\"\n",
                 "corpus_config: CorpusConfig = CorpusConfig.load(os.path.join(__paths__.resources_folder, 'courier_page.yml'))"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "86a9d930",
+            "id": "ee890472",
             "metadata": {},
             "source": [
                 "### <span style='color: green'>PREPARE</span> Load Topic Model <span style='float: right; color: red'>MANDATORY</span>"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "3c536754",
+            "id": "e1412ac0",
             "metadata": {},
             "outputs": [],
             "source": [
                 "load_gui = gui.create_load_topic_model_gui(corpus_config, corpus_folder, current_state())\n",
                 "display(load_gui.layout())"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "add168ee",
+            "id": "aba6d243",
             "metadata": {},
             "source": [
                 "### <span style='color: green;'>BROWSE</span> Find topics by token<span style='color: red; float: right'>TRY IT</span>\n",
                 "\n",
                 "Displays topics in which given token is among toplist of dominant words."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "15d7d8f5",
+            "id": "62009824",
             "metadata": {},
             "outputs": [],
             "source": [
                 "gui.find_topic_documents_gui(\n",
                 "    current_state().inferred_topics.document_topic_weights, current_state().inferred_topics.topic_token_overview\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "eb41d28d",
+            "id": "b6323cc6",
             "metadata": {},
             "source": [
                 "### <span style='color: green;'>BROWSE</span> Browse Topic Documents<span style='color: red; float: right'>TRY IT</span>\n",
                 "\n",
                 "Displays documents in which a topic occurs above a given threshold."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "4c3d21fe",
+            "id": "cf5c0854",
             "metadata": {},
             "outputs": [],
             "source": [
                 "gui.display_topic_documents_gui(current_state())"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "0ada29e6",
+            "id": "3b833fd9",
             "metadata": {},
             "source": [
                 "### <span style='color: green;'>VISUALIZE</span> Display Topic's Word Distribution as a Wordcloud<span style='color: red; float: right'> TRY IT</span>"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "6a450ea4",
+            "id": "ecf4c552",
             "metadata": {},
             "outputs": [],
             "source": [
                 "gui.display_topic_wordcloud_gui(current_state())"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "302350c5",
+            "id": "9a5616d2",
             "metadata": {},
             "source": [
                 "### <span style='color: green;'>VISUALIZE</span> Topic-Word Distribution<span style='color: red; float: right'>TRY IT</span>\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "43ab229e",
+            "id": "f93c8772",
             "metadata": {},
             "outputs": [],
             "source": [
                 "gui.display_topic_word_distribution_gui(current_state())"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "1a5f062e",
+            "id": "8bdfc245",
             "metadata": {},
             "source": [
                 "### <span style='color: green;'>VISUALIZE</span> Topic Trends over Time<span style='color: red; float: right'>RUN</span>"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "ea0f5222",
+            "id": "c0f81cab",
             "metadata": {},
             "outputs": [],
             "source": [
                 "gui.display_topic_trends_gui(current_state())"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "a9e073fa",
+            "id": "5db26ca2",
             "metadata": {},
             "source": [
                 "### <span style='color: green;'>VISUALIZE</span> Topic Trends Overview<span style='color: red; float: right'>TRY IT</span>\n",
                 "\n",
                 "- The topic shares  displayed as a scattered heatmap plot using gradient color based on topic's weight in document.\n",
                 "- [Stanford\u2019s Termite software](http://vis.stanford.edu/papers/termite) uses a similar visualization."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "931f186c",
+            "id": "400d951d",
             "metadata": {},
             "outputs": [],
             "source": [
                 "gui.display_topic_trends_overview_gui(current_state())"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "d09a2371",
+            "id": "d2611044",
             "metadata": {},
             "source": [
                 "### <span style='color: green;'>VISUALIZE</span> Topic Topic Network<span style='color: red; float: right'>TRY IT</span>\n",
                 "\n",
                 "Computes weighted graph of topics co-occurring in the same document. Topics are defined as co-occurring in a document if they both have a weight above given threshold. The edge weights are the number of co-occurrences (binary yes or no). Node size reflects topic proportions over the entire corpus computed in accordance to LDAvis topic proportions."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "84e0cff7",
+            "id": "74725f5a",
             "metadata": {
                 "code_folding": [
                     0
                 ]
             },
             "outputs": [],
             "source": [
                 "gui.display_topic_topic_network_gui(current_state())"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "9dc63f07",
+            "id": "70960e72",
             "metadata": {},
             "source": [
                 "### <span style='color: green;'>VISUALIZE</span> Document Topic Network<span style='color: red; float: right'>TRY IT</span>\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "ef195672",
+            "id": "1bc85cf4",
             "metadata": {},
             "outputs": [],
             "source": [
                 "gui.display_topic_document_network_gui(plot_mode=gui.PlotMode.Default, state=current_state())  # type: ignore"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "75663b9b",
+            "id": "e86adc58",
             "metadata": {},
             "source": [
                 "### <span style='color: green;'>VISUALIZE</span> Focus-Topic Document Network<span style='color: red; float: right'>TRY IT</span>\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "5dd4d1ab",
+            "id": "20948e89",
             "metadata": {},
             "outputs": [],
             "source": [
                 "gui.display_topic_document_network_gui(plot_mode=gui.PlotMode.FocusTopics, state=current_state())"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "6881c77c",
+            "id": "6374ddf7",
             "metadata": {},
             "source": [
                 "### <span style='color: green;'>VISUALIZE</span> Topic-Token  Network<span style='color: red; float: right'>TRY IT</span>"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "9d7fbd40",
+            "id": "2a2e4c71",
             "metadata": {},
             "outputs": [],
             "source": [
                 "custom_styles = {'edges': {'curve-style': 'haystack'}}\n",
                 "w = gui.create_topics_token_network_gui(data_folder=corpus_folder, custom_styles=custom_styles)\n",
                 "display(w.layout())"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d6544630",
+            "id": "7590de0e",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "jupytext": {
```

### Comparing `humlab-inidun-0.3.8/notebooks/topic_modelling/explore_topic_models.py` & `humlab-inidun-0.3.9/notebooks/topic_modelling/explore_topic_models.py`

 * *Files identical despite different names*

### Comparing `humlab-inidun-0.3.8/notebooks/word_trends/word_trends.ipynb` & `humlab-inidun-0.3.9/notebooks/word_trends/word_trends.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9878472222222222%*

 * *Differences: {"'cells'": "{0: {'id': '409c74dd'}, 1: {'id': 'a7df479a'}, 2: {'id': '202eb374'}}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "9a7d5d9a",
+            "id": "409c74dd",
             "metadata": {
                 "lines_to_next_cell": 0
             },
             "source": [
                 "## Word, or part-of-word, trend analysis\n",
                 "\n",
                 "### Text Processing Pipeline\n",
@@ -77,23 +77,23 @@
                 "To match all words starting with `info`you can enter `|^info.*|` where `^` specifies the start of the word.\n",
                 "\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "6fd52138",
+            "id": "a7df479a",
             "metadata": {},
             "outputs": [],
             "source": []
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "4b80e05b",
+            "id": "202eb374",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from bokeh.plotting import output_notebook\n",
                 "from IPython.core.display import display\n",
                 "from penelope.notebook.word_trends import main_gui\n",
                 "\n",
```

### Comparing `humlab-inidun-0.3.8/notebooks/word_trends/word_trends.py` & `humlab-inidun-0.3.9/notebooks/word_trends/word_trends.py`

 * *Files identical despite different names*

### Comparing `humlab-inidun-0.3.8/pyproject.toml` & `humlab-inidun-0.3.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "humlab-inidun"
-version = "0.3.8"
+version = "0.3.9"
 description = "INIDUN research project text analysis tools and utilities"
 authors = ["Roger Mähler <roger.mahler@hotmail.com>"]
 packages = [
     { include = "notebooks" }
 ]
 classifiers = [
     'License :: OSI Approved :: Apache Software License',
@@ -28,15 +28,15 @@
 jupyterlab = "==3.0.16"
 matplotlib = "*"
 msgpack = "^1.0.2"
 pandas = "*"
 pandas-bokeh = "*"
 python = "==3.8.*"
 tqdm = "*"
-humlab-penelope = "^0.5.27"
+humlab-penelope = "^0.5.30"
 
 [tool.poetry.dev-dependencies]
 black = "==20.*,>=20.8.0.b1"
 coverage = "*"
 flake8 = "==3.*,>=3.8.4"
 flake8-black = "==0.*,>=0.2.1"
 flake8-pytest-style = "==1.*,>=1.3.0"
```

### Comparing `humlab-inidun-0.3.8/setup.py` & `humlab-inidun-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['bokeh',
  'click',
- 'humlab-penelope>=0.5.27,<0.6.0',
+ 'humlab-penelope>=0.5.30,<0.6.0',
  'ipywidgets==7.6.3',
  'jupyterlab==3.0.16',
  'matplotlib',
  'msgpack>=1.0.2,<2.0.0',
  'pandas',
  'pandas-bokeh',
  'tqdm']
 
 setup_kwargs = {
     'name': 'humlab-inidun',
-    'version': '0.3.8',
+    'version': '0.3.9',
     'description': 'INIDUN research project text analysis tools and utilities',
     'long_description': '# The INIDUN Text Analytics Repository\n\n### Prerequisites\n\n### Installation\n\n### Note\n\n\n',
     'author': 'Roger Mähler',
     'author_email': 'roger.mahler@hotmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://inidun.github.io',
```

### Comparing `humlab-inidun-0.3.8/PKG-INFO` & `humlab-inidun-0.3.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: humlab-inidun
-Version: 0.3.8
+Version: 0.3.9
 Summary: INIDUN research project text analysis tools and utilities
 Home-page: https://inidun.github.io
 License: Apache-2.0
 Author: Roger Mähler
 Author-email: roger.mahler@hotmail.com
 Requires-Python: >=3.8.0,<3.9.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development
 Requires-Dist: bokeh
 Requires-Dist: click
-Requires-Dist: humlab-penelope (>=0.5.27,<0.6.0)
+Requires-Dist: humlab-penelope (>=0.5.30,<0.6.0)
 Requires-Dist: ipywidgets (==7.6.3)
 Requires-Dist: jupyterlab (==3.0.16)
 Requires-Dist: matplotlib
 Requires-Dist: msgpack (>=1.0.2,<2.0.0)
 Requires-Dist: pandas
 Requires-Dist: pandas-bokeh
 Requires-Dist: tqdm
```

