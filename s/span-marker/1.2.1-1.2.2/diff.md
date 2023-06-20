# Comparing `tmp/span_marker-1.2.1.tar.gz` & `tmp/span_marker-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "span_marker-1.2.1.tar", last modified: Mon Jun 19 14:11:24 2023, max compression
+gzip compressed data, was "span_marker-1.2.2.tar", last modified: Tue Jun 20 09:28:22 2023, max compression
```

## Comparing `span_marker-1.2.1.tar` & `span_marker-1.2.2.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 14:11:24.682843 span_marker-1.2.1/
--rw-rw-rw-   0        0        0    11558 2023-05-04 23:33:40.000000 span_marker-1.2.1/LICENSE
--rw-rw-rw-   0        0        0    15006 2023-06-19 14:11:24.681844 span_marker-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    14438 2023-06-19 14:01:35.000000 span_marker-1.2.1/README.md
--rw-rw-rw-   0        0        0     2650 2023-06-19 13:46:11.000000 span_marker-1.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-19 14:11:24.682843 span_marker-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-06-19 13:47:30.000000 span_marker-1.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 14:11:24.668761 span_marker-1.2.1/span_marker/
--rw-rw-rw-   0        0        0     1659 2023-06-19 14:09:48.000000 span_marker-1.2.1/span_marker/__init__.py
--rw-rw-rw-   0        0        0     7070 2023-06-15 09:34:01.000000 span_marker-1.2.1/span_marker/configuration.py
--rw-rw-rw-   0        0        0     6630 2023-06-13 22:30:33.000000 span_marker-1.2.1/span_marker/data_collator.py
--rw-rw-rw-   0        0        0     5276 2023-06-15 14:37:15.000000 span_marker-1.2.1/span_marker/evaluation.py
--rw-rw-rw-   0        0        0     5230 2023-05-31 13:34:45.000000 span_marker-1.2.1/span_marker/label_normalizer.py
--rw-rw-rw-   0        0        0     2472 2023-06-13 22:30:43.000000 span_marker-1.2.1/span_marker/model_card.py
--rw-rw-rw-   0        0        0    31577 2023-06-16 08:01:13.000000 span_marker-1.2.1/span_marker/modeling.py
--rw-rw-rw-   0        0        0     2221 2023-06-13 22:30:33.000000 span_marker-1.2.1/span_marker/output.py
--rw-rw-rw-   0        0        0     3914 2023-06-19 13:45:55.000000 span_marker-1.2.1/span_marker/spacy_integration.py
--rw-rw-rw-   0        0        0    11828 2023-06-19 13:54:52.000000 span_marker-1.2.1/span_marker/tokenizer.py
--rw-rw-rw-   0        0        0    21019 2023-06-15 10:02:14.000000 span_marker-1.2.1/span_marker/trainer.py
-drwxrwxrwx   0        0        0        0 2023-06-19 14:11:24.678843 span_marker-1.2.1/span_marker.egg-info/
--rw-rw-rw-   0        0        0    15006 2023-06-19 14:11:24.000000 span_marker-1.2.1/span_marker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      638 2023-06-19 14:11:24.000000 span_marker-1.2.1/span_marker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 14:11:24.000000 span_marker-1.2.1/span_marker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      267 2023-06-19 14:11:24.000000 span_marker-1.2.1/span_marker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-19 14:11:24.000000 span_marker-1.2.1/span_marker.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 14:11:24.681844 span_marker-1.2.1/tests/
--rw-rw-rw-   0        0        0     1645 2023-06-10 13:15:43.000000 span_marker-1.2.1/tests/test_configuration.py
--rw-rw-rw-   0        0        0     1410 2023-06-01 07:33:08.000000 span_marker-1.2.1/tests/test_model_card.py
--rw-rw-rw-   0        0        0     9228 2023-06-15 09:34:01.000000 span_marker-1.2.1/tests/test_modeling.py
--rw-rw-rw-   0        0        0     1148 2023-06-15 14:47:29.000000 span_marker-1.2.1/tests/test_spacy_integration.py
--rw-rw-rw-   0        0        0    10372 2023-06-15 09:34:01.000000 span_marker-1.2.1/tests/test_trainer.py
+drwxrwxrwx   0        0        0        0 2023-06-20 09:28:22.535627 span_marker-1.2.2/
+-rw-rw-rw-   0        0        0    11558 2023-05-04 23:33:40.000000 span_marker-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0    15023 2023-06-20 09:28:22.535627 span_marker-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    14455 2023-06-20 09:23:03.000000 span_marker-1.2.2/README.md
+-rw-rw-rw-   0        0        0     2521 2023-06-20 09:21:34.000000 span_marker-1.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-20 09:28:22.535627 span_marker-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      140 2023-06-20 09:21:47.000000 span_marker-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 09:28:22.522716 span_marker-1.2.2/span_marker/
+-rw-rw-rw-   0        0        0     1659 2023-06-20 09:27:28.000000 span_marker-1.2.2/span_marker/__init__.py
+-rw-rw-rw-   0        0        0     7070 2023-06-15 09:34:01.000000 span_marker-1.2.2/span_marker/configuration.py
+-rw-rw-rw-   0        0        0     6630 2023-06-13 22:30:33.000000 span_marker-1.2.2/span_marker/data_collator.py
+-rw-rw-rw-   0        0        0     5276 2023-06-15 14:37:15.000000 span_marker-1.2.2/span_marker/evaluation.py
+-rw-rw-rw-   0        0        0     5230 2023-05-31 13:34:45.000000 span_marker-1.2.2/span_marker/label_normalizer.py
+-rw-rw-rw-   0        0        0     2472 2023-06-13 22:30:43.000000 span_marker-1.2.2/span_marker/model_card.py
+-rw-rw-rw-   0        0        0    31577 2023-06-20 07:05:23.000000 span_marker-1.2.2/span_marker/modeling.py
+-rw-rw-rw-   0        0        0     2221 2023-06-13 22:30:33.000000 span_marker-1.2.2/span_marker/output.py
+-rw-rw-rw-   0        0        0     3902 2023-06-20 09:24:39.000000 span_marker-1.2.2/span_marker/spacy_integration.py
+-rw-rw-rw-   0        0        0    11828 2023-06-19 13:54:52.000000 span_marker-1.2.2/span_marker/tokenizer.py
+-rw-rw-rw-   0        0        0    21019 2023-06-15 10:02:14.000000 span_marker-1.2.2/span_marker/trainer.py
+drwxrwxrwx   0        0        0        0 2023-06-20 09:28:22.532121 span_marker-1.2.2/span_marker.egg-info/
+-rw-rw-rw-   0        0        0    15023 2023-06-20 09:28:22.000000 span_marker-1.2.2/span_marker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      676 2023-06-20 09:28:22.000000 span_marker-1.2.2/span_marker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 09:28:22.000000 span_marker-1.2.2/span_marker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-06-20 09:28:22.000000 span_marker-1.2.2/span_marker.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      267 2023-06-20 09:28:22.000000 span_marker-1.2.2/span_marker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-20 09:28:22.000000 span_marker-1.2.2/span_marker.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 09:28:22.534624 span_marker-1.2.2/tests/
+-rw-rw-rw-   0        0        0     1645 2023-06-10 13:15:43.000000 span_marker-1.2.2/tests/test_configuration.py
+-rw-rw-rw-   0        0        0     1410 2023-06-01 07:33:08.000000 span_marker-1.2.2/tests/test_model_card.py
+-rw-rw-rw-   0        0        0     9228 2023-06-15 09:34:01.000000 span_marker-1.2.2/tests/test_modeling.py
+-rw-rw-rw-   0        0        0     1165 2023-06-20 09:23:58.000000 span_marker-1.2.2/tests/test_spacy_integration.py
+-rw-rw-rw-   0        0        0    10372 2023-06-15 09:34:01.000000 span_marker-1.2.2/tests/test_trainer.py
```

### Comparing `span_marker-1.2.1/LICENSE` & `span_marker-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.1/PKG-INFO` & `span_marker-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: span_marker
-Version: 1.2.1
+Version: 1.2.2
 Summary: Named Entity Recognition using Span Markers
 Author: Tom Aarsen
 Maintainer: Tom Aarsen
 Project-URL: Documentation, https://tomaarsen.github.io/SpanMarkerNER
 Project-URL: Repository, https://github.com/tomaarsen/SpanMarkerNER
 Keywords: data-science,natural-language-processing,artificial-intelligence,mlops,nlp,machine-learning,transformers
 Requires-Python: >=3.7
@@ -159,15 +159,15 @@
 
 ## Using pretrained SpanMarker models with spaCy
 All [SpanMarker models on the Hugging Face Hub](https://huggingface.co/models?library=span-marker) can also be easily used in spaCy. It's as simple as including 1 line to add the `span_marker` pipeline. See the Documentation or API Reference for more information.
 ```python
 import spacy
 
 # Load the spaCy model with the span_marker pipeline component
-nlp = spacy.load("en_core_web_sm")
+nlp = spacy.load("en_core_web_sm", disable=["ner"])
 nlp.add_pipe("span_marker", config={"model": "tomaarsen/span-marker-roberta-large-ontonotes5"})
 
 # Feed some text through the model to get a spacy Doc
 text = """Cleopatra VII, also known as Cleopatra the Great, was the last active ruler of the \
 Ptolemaic Kingdom of Egypt. She was born in 69 BCE and ruled Egypt from 51 BCE until her \
 death in 30 BCE."""
 doc = nlp(text)
```

### Comparing `span_marker-1.2.1/README.md` & `span_marker-1.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 
 ## Using pretrained SpanMarker models with spaCy
 All [SpanMarker models on the Hugging Face Hub](https://huggingface.co/models?library=span-marker) can also be easily used in spaCy. It's as simple as including 1 line to add the `span_marker` pipeline. See the Documentation or API Reference for more information.
 ```python
 import spacy
 
 # Load the spaCy model with the span_marker pipeline component
-nlp = spacy.load("en_core_web_sm")
+nlp = spacy.load("en_core_web_sm", disable=["ner"])
 nlp.add_pipe("span_marker", config={"model": "tomaarsen/span-marker-roberta-large-ontonotes5"})
 
 # Feed some text through the model to get a spacy Doc
 text = """Cleopatra VII, also known as Cleopatra the Great, was the last active ruler of the \
 Ptolemaic Kingdom of Egypt. She was born in 69 BCE and ruled Egypt from 51 BCE until her \
 death in 30 BCE."""
 doc = nlp(text)
```

### Comparing `span_marker-1.2.1/pyproject.toml` & `span_marker-1.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -124,12 +124,7 @@
 
 [tool.ruff.per-file-ignores]
 # Ignore imported but unused;
 "__init__.py" = ["F401"]
 
 [tool.black]
 line-length = 120
-
-[tool.poetry.plugins]
-
-[tool.poetry.plugins."spacy_factories"]
-"spacy" = "span_marker.__init__:_spacy_span_marker_factory"
```

### Comparing `span_marker-1.2.1/span_marker/__init__.py` & `span_marker-1.2.2/span_marker/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.2.1"
+__version__ = "1.2.2"
 
 import logging
 from typing import Optional, Union
 
 import torch
 from transformers import AutoConfig, AutoModel, TrainingArguments
```

### Comparing `span_marker-1.2.1/span_marker/configuration.py` & `span_marker-1.2.2/span_marker/configuration.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.1/span_marker/data_collator.py` & `span_marker-1.2.2/span_marker/data_collator.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.1/span_marker/evaluation.py` & `span_marker-1.2.2/span_marker/evaluation.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.1/span_marker/label_normalizer.py` & `span_marker-1.2.2/span_marker/label_normalizer.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.1/span_marker/model_card.py` & `span_marker-1.2.2/span_marker/model_card.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.1/span_marker/modeling.py` & `span_marker-1.2.2/span_marker/modeling.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.1/span_marker/output.py` & `span_marker-1.2.2/span_marker/output.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.1/span_marker/spacy_integration.py` & `span_marker-1.2.2/span_marker/spacy_integration.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,29 +12,28 @@
     """This wrapper allows SpanMarker to be used as a drop-in replacement of the "ner" pipeline component.
 
     Usage:
 
     .. code-block:: diff
 
          import spacy
-       + import span_marker
 
          nlp = spacy.load("en_core_web_sm")
        + nlp.add_pipe("span_marker", config={"model": "tomaarsen/span-marker-roberta-large-ontonotes5"})
 
          text = '''Cleopatra VII, also known as Cleopatra the Great, was the last active ruler of the
          Ptolemaic Kingdom of Egypt. She was born in 69 BCE and ruled Egypt from 51 BCE until her
          death in 30 BCE.'''
          doc = nlp(text)
 
     Example::
 
         >>> import spacy
         >>> import span_marker
-        >>> nlp = spacy.load("en_core_web_sm")
+        >>> nlp = spacy.load("en_core_web_sm", disable=["ner"])
         >>> nlp.add_pipe("span_marker", config={"model": "tomaarsen/span-marker-roberta-large-ontonotes5"})
         >>> text = '''Cleopatra VII, also known as Cleopatra the Great, was the last active ruler of the
         ... Ptolemaic Kingdom of Egypt. She was born in 69 BCE and ruled Egypt from 51 BCE until her
         ... death in 30 BCE.'''
         >>> doc = nlp(text)
         >>> doc.ents
         (Cleopatra VII, Cleopatra the Great, 69 BCE, Egypt, 51 BCE, 30 BCE)
```

### Comparing `span_marker-1.2.1/span_marker/tokenizer.py` & `span_marker-1.2.2/span_marker/tokenizer.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.1/span_marker/trainer.py` & `span_marker-1.2.2/span_marker/trainer.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.1/span_marker.egg-info/PKG-INFO` & `span_marker-1.2.2/span_marker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: span-marker
-Version: 1.2.1
+Version: 1.2.2
 Summary: Named Entity Recognition using Span Markers
 Author: Tom Aarsen
 Maintainer: Tom Aarsen
 Project-URL: Documentation, https://tomaarsen.github.io/SpanMarkerNER
 Project-URL: Repository, https://github.com/tomaarsen/SpanMarkerNER
 Keywords: data-science,natural-language-processing,artificial-intelligence,mlops,nlp,machine-learning,transformers
 Requires-Python: >=3.7
@@ -159,15 +159,15 @@
 
 ## Using pretrained SpanMarker models with spaCy
 All [SpanMarker models on the Hugging Face Hub](https://huggingface.co/models?library=span-marker) can also be easily used in spaCy. It's as simple as including 1 line to add the `span_marker` pipeline. See the Documentation or API Reference for more information.
 ```python
 import spacy
 
 # Load the spaCy model with the span_marker pipeline component
-nlp = spacy.load("en_core_web_sm")
+nlp = spacy.load("en_core_web_sm", disable=["ner"])
 nlp.add_pipe("span_marker", config={"model": "tomaarsen/span-marker-roberta-large-ontonotes5"})
 
 # Feed some text through the model to get a spacy Doc
 text = """Cleopatra VII, also known as Cleopatra the Great, was the last active ruler of the \
 Ptolemaic Kingdom of Egypt. She was born in 69 BCE and ruled Egypt from 51 BCE until her \
 death in 30 BCE."""
 doc = nlp(text)
```

### Comparing `span_marker-1.2.1/span_marker.egg-info/SOURCES.txt` & `span_marker-1.2.2/span_marker.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 span_marker/output.py
 span_marker/spacy_integration.py
 span_marker/tokenizer.py
 span_marker/trainer.py
 span_marker.egg-info/PKG-INFO
 span_marker.egg-info/SOURCES.txt
 span_marker.egg-info/dependency_links.txt
+span_marker.egg-info/entry_points.txt
 span_marker.egg-info/requires.txt
 span_marker.egg-info/top_level.txt
 tests/test_configuration.py
 tests/test_model_card.py
 tests/test_modeling.py
 tests/test_spacy_integration.py
 tests/test_trainer.py
```

### Comparing `span_marker-1.2.1/tests/test_configuration.py` & `span_marker-1.2.2/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.1/tests/test_model_card.py` & `span_marker-1.2.2/tests/test_model_card.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.1/tests/test_modeling.py` & `span_marker-1.2.2/tests/test_modeling.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.2.1/tests/test_spacy_integration.py` & `span_marker-1.2.2/tests/test_spacy_integration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import spacy
 
 
 def test_span_marker_as_spacy_pipeline_component():
-    nlp = spacy.load("en_core_web_sm")
+    nlp = spacy.load("en_core_web_sm", disable=["ner"])
     batch_size = 2
     wrapper = nlp.add_pipe(
         "span_marker", config={"model": "tomaarsen/span-marker-bert-tiny-conll03", "batch_size": batch_size}
     )
     assert wrapper.batch_size == batch_size
 
     doc = nlp("Amelia Earhart flew her single engine Lockheed Vega 5B across the Atlantic to Paris.")
```

### Comparing `span_marker-1.2.1/tests/test_trainer.py` & `span_marker-1.2.2/tests/test_trainer.py`

 * *Files identical despite different names*

