# Comparing `tmp/pydoxtools-0.6.4.tar.gz` & `tmp/pydoxtools-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydoxtools-0.6.4.tar", max compression
+gzip compressed data, was "pydoxtools-0.6.5.tar", max compression
```

## Comparing `pydoxtools-0.6.4.tar` & `pydoxtools-0.6.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1072 2023-03-29 07:08:59.780129 pydoxtools-0.6.4/LICENSE
--rw-r--r--   0        0        0     8260 2023-05-25 18:58:37.513803 pydoxtools-0.6.4/README.md
--rw-r--r--   0        0        0      353 2023-06-05 05:49:41.328878 pydoxtools-0.6.4/pydoxtools/__init__.py
--rw-r--r--   0        0        0    12308 2023-06-05 05:49:41.328878 pydoxtools-0.6.4/pydoxtools/agent.py
--rw-r--r--   0        0        0     2501 2023-06-05 05:49:41.328878 pydoxtools-0.6.4/pydoxtools/class_utils.py
--rwxr-xr-x   0        0        0    30464 2023-06-05 05:49:41.328878 pydoxtools-0.6.4/pydoxtools/classifier.py
--rw-r--r--   0        0        0    29499 2023-06-05 05:49:41.328878 pydoxtools-0.6.4/pydoxtools/cluster_utils.py
--rw-r--r--   0        0        0     6139 2023-06-05 05:49:41.328878 pydoxtools-0.6.4/pydoxtools/dask_operators.py
--rw-r--r--   0        0        0    54128 2023-06-05 05:49:41.328878 pydoxtools-0.6.4/pydoxtools/document.py
--rw-r--r--   0        0        0    35236 2023-06-05 05:49:41.328878 pydoxtools-0.6.4/pydoxtools/document_base.py
--rw-r--r--   0        0        0     1765 2023-06-05 05:49:41.328878 pydoxtools-0.6.4/pydoxtools/extract_classes.py
--rw-r--r--   0        0        0     4065 2023-06-05 05:49:41.328878 pydoxtools-0.6.4/pydoxtools/extract_filesystem.py
--rw-r--r--   0        0        0    13396 2023-06-05 05:49:41.328878 pydoxtools-0.6.4/pydoxtools/extract_html.py
--rw-r--r--   0        0        0    12658 2023-06-05 05:49:41.328878 pydoxtools-0.6.4/pydoxtools/extract_index.py
--rw-r--r--   0        0        0     6069 2023-06-05 05:49:41.328878 pydoxtools-0.6.4/pydoxtools/extract_nlpchat.py
--rw-r--r--   0        0        0     2561 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/extract_objects.py
--rw-r--r--   0        0        0     1750 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/extract_ocr.py
--rw-r--r--   0        0        0     6561 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/extract_pandoc.py
--rw-r--r--   0        0        0     5570 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/extract_spacy.py
--rw-r--r--   0        0        0    43343 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/extract_tables.py
--rw-r--r--   0        0        0     8231 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/extract_textstructure.py
--rw-r--r--   0        0        0     1324 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/file_utils.py
--rwxr-xr-x   0        0        0     6187 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/html_utils.py
--rw-r--r--   0        0        0     7167 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/labeling.py
--rw-r--r--   0        0        0     7327 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/list_utils.py
--rw-r--r--   0        0        0      466 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/math_utils.py
--rw-r--r--   0        0        0     2499 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/models.py
--rwxr-xr-x   0        0        0    18805 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/nlp_utils.py
--rw-r--r--   0        0        0     2504 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/ocr_language_mappings.py
--rw-r--r--   0        0        0     8965 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/operator_huggingface.py
--rw-r--r--   0        0        0     1134 2023-06-04 22:57:01.069614 pydoxtools-0.6.4/pydoxtools/operators.py
--rw-r--r--   0        0        0     7947 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/operators_base.py
--rwxr-xr-x   0        0        0    12182 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/pdf_utils.py
--rw-r--r--   0        0        0    34121 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/random_data_generators.py
--rwxr-xr-x   0        0        0     1400 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/settings.py
--rw-r--r--   0        0        0    17775 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/training.py
--rw-r--r--   0        0        0     3990 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/visual_document_analysis.py
--rw-r--r--   0        0        0     3301 2023-06-05 05:49:41.332879 pydoxtools-0.6.4/pydoxtools/webdav_utils.py
--rw-r--r--   0        0        0     5988 2023-06-05 05:55:24.817152 pydoxtools-0.6.4/pyproject.toml
--rw-r--r--   0        0        0    11246 1970-01-01 00:00:00.000000 pydoxtools-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2022-11-13 06:52:05.633039 pydoxtools-0.6.5/LICENSE
+-rw-r--r--   0        0        0     8260 2023-05-28 21:59:18.876134 pydoxtools-0.6.5/README.md
+-rw-r--r--   0        0        0      353 2023-06-20 07:10:23.054510 pydoxtools-0.6.5/pydoxtools/__init__.py
+-rw-r--r--   0        0        0    12336 2023-06-20 07:10:23.054510 pydoxtools-0.6.5/pydoxtools/agent.py
+-rw-r--r--   0        0        0     2501 2023-06-20 07:10:23.054510 pydoxtools-0.6.5/pydoxtools/class_utils.py
+-rwxr-xr-x   0        0        0    30464 2023-06-20 07:10:23.054510 pydoxtools-0.6.5/pydoxtools/classifier.py
+-rw-r--r--   0        0        0    29499 2023-06-20 07:10:23.054510 pydoxtools-0.6.5/pydoxtools/cluster_utils.py
+-rw-r--r--   0        0        0     6139 2023-06-20 07:10:23.054510 pydoxtools-0.6.5/pydoxtools/dask_operators.py
+-rw-r--r--   0        0        0    56541 2023-06-20 07:10:23.054510 pydoxtools-0.6.5/pydoxtools/document.py
+-rw-r--r--   0        0        0    38002 2023-06-20 07:10:23.058510 pydoxtools-0.6.5/pydoxtools/document_base.py
+-rw-r--r--   0        0        0     1792 2023-06-20 07:10:23.058510 pydoxtools-0.6.5/pydoxtools/extract_classes.py
+-rw-r--r--   0        0        0     4065 2023-06-20 07:10:23.058510 pydoxtools-0.6.5/pydoxtools/extract_filesystem.py
+-rw-r--r--   0        0        0    13396 2023-06-20 07:10:23.058510 pydoxtools-0.6.5/pydoxtools/extract_html.py
+-rw-r--r--   0        0        0    12866 2023-06-20 07:10:23.058510 pydoxtools-0.6.5/pydoxtools/extract_index.py
+-rw-r--r--   0        0        0     6082 2023-06-20 07:10:23.058510 pydoxtools-0.6.5/pydoxtools/extract_nlpchat.py
+-rw-r--r--   0        0        0     2561 2023-06-20 07:10:23.058510 pydoxtools-0.6.5/pydoxtools/extract_objects.py
+-rw-r--r--   0        0        0     1750 2023-06-20 07:10:23.058510 pydoxtools-0.6.5/pydoxtools/extract_ocr.py
+-rw-r--r--   0        0        0     6561 2023-06-20 07:10:23.058510 pydoxtools-0.6.5/pydoxtools/extract_pandoc.py
+-rw-r--r--   0        0        0     5616 2023-06-20 07:10:23.058510 pydoxtools-0.6.5/pydoxtools/extract_spacy.py
+-rw-r--r--   0        0        0    43359 2023-06-20 07:10:23.058510 pydoxtools-0.6.5/pydoxtools/extract_tables.py
+-rw-r--r--   0        0        0     8303 2023-06-20 07:10:23.058510 pydoxtools-0.6.5/pydoxtools/extract_textstructure.py
+-rw-r--r--   0        0        0     1324 2023-06-20 07:10:23.058510 pydoxtools-0.6.5/pydoxtools/file_utils.py
+-rwxr-xr-x   0        0        0     6187 2023-06-20 07:10:23.058510 pydoxtools-0.6.5/pydoxtools/html_utils.py
+-rw-r--r--   0        0        0     7167 2023-06-20 07:10:23.058510 pydoxtools-0.6.5/pydoxtools/labeling.py
+-rw-r--r--   0        0        0     7327 2023-06-20 07:10:23.058510 pydoxtools-0.6.5/pydoxtools/list_utils.py
+-rw-r--r--   0        0        0      466 2023-06-20 07:10:23.058510 pydoxtools-0.6.5/pydoxtools/math_utils.py
+-rw-r--r--   0        0        0     2581 2023-06-20 07:10:23.058510 pydoxtools-0.6.5/pydoxtools/models.py
+-rwxr-xr-x   0        0        0    18805 2023-06-20 07:10:23.058510 pydoxtools-0.6.5/pydoxtools/nlp_utils.py
+-rw-r--r--   0        0        0     2504 2023-06-20 07:10:23.058510 pydoxtools-0.6.5/pydoxtools/ocr_language_mappings.py
+-rw-r--r--   0        0        0     8965 2023-06-20 07:10:23.058510 pydoxtools-0.6.5/pydoxtools/operator_huggingface.py
+-rw-r--r--   0        0        0     1134 2023-05-28 23:27:52.111997 pydoxtools-0.6.5/pydoxtools/operators.py
+-rw-r--r--   0        0        0    13821 2023-06-20 07:10:23.058510 pydoxtools-0.6.5/pydoxtools/operators_base.py
+-rwxr-xr-x   0        0        0    16436 2023-06-20 07:10:23.058510 pydoxtools-0.6.5/pydoxtools/pdf_utils.py
+-rw-r--r--   0        0        0    34121 2023-06-20 07:10:23.058510 pydoxtools-0.6.5/pydoxtools/random_data_generators.py
+-rwxr-xr-x   0        0        0     1400 2023-06-20 07:10:23.058510 pydoxtools-0.6.5/pydoxtools/settings.py
+-rw-r--r--   0        0        0    17775 2023-06-20 07:10:23.058510 pydoxtools-0.6.5/pydoxtools/training.py
+-rw-r--r--   0        0        0     5742 2023-06-20 07:10:23.058510 pydoxtools-0.6.5/pydoxtools/visual_document_analysis.py
+-rw-r--r--   0        0        0     3301 2023-06-20 07:10:23.058510 pydoxtools-0.6.5/pydoxtools/webdav_utils.py
+-rw-r--r--   0        0        0     6005 2023-06-20 07:10:23.058510 pydoxtools-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0    11263 1970-01-01 00:00:00.000000 pydoxtools-0.6.5/PKG-INFO
```

### Comparing `pydoxtools-0.6.4/LICENSE` & `pydoxtools-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.4/README.md` & `pydoxtools-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.4/pydoxtools/agent.py` & `pydoxtools-0.6.5/pydoxtools/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import chromadb
 import dask.diagnostics
 import numpy as np
 import yaml
 
 import pydoxtools as pdx
 from pydoxtools.extract_nlpchat import openai_chat_completion
+import typing
 
 logger = logging.getLogger(__name__)
 
 
 def generate_function_usage_prompt(func: callable):
     # TODO: summarize function usage, only extract the parameter description
     # func.__doc__
@@ -184,15 +185,15 @@
             self,
             task,
             context_size: int = 5,
             previous_task_size=0,
             max_tokens=256,
             formatting="yaml",
             save_task=False
-    ):
+    ) -> typing.Any:
         if context_size:
             context = self.get_context(
                 task,
                 where_clause=self._context_where_info,
                 n_results=context_size)[0]
         else:
             context = ""
```

### Comparing `pydoxtools-0.6.4/pydoxtools/class_utils.py` & `pydoxtools-0.6.5/pydoxtools/class_utils.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.4/pydoxtools/classifier.py` & `pydoxtools-0.6.5/pydoxtools/classifier.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.4/pydoxtools/cluster_utils.py` & `pydoxtools-0.6.5/pydoxtools/cluster_utils.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.4/pydoxtools/dask_operators.py` & `pydoxtools-0.6.5/pydoxtools/dask_operators.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.4/pydoxtools/document.py` & `pydoxtools-0.6.5/pydoxtools/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import functools
 import io
 import json
 import logging
 import mimetypes
 import re
+import typing
 from functools import cached_property
 from pathlib import Path
 from typing import IO, Protocol, Any, Callable
 from urllib.parse import urlparse
 
 import dask.bag
 import langdetect
@@ -40,15 +41,15 @@
 from .extract_textstructure import DocumentElementFilter, TextBoxElementExtractor, TitleExtractor, SectionsExtractor
 from .html_utils import get_text_only_blocks
 from .list_utils import remove_list_from_lonely_object
 from .nlp_utils import calculate_string_embeddings, summarize_long_text
 from .operator_huggingface import QamExtractor
 from .operators_base import Alias, FunctionOperator, ElementWiseOperator, Constant, DictSelector, \
     Operator, Configuration
-from .pdf_utils import PDFFileLoader
+from .pdf_utils import PDFFileLoader, PDFImageRenderer
 
 logger = logging.getLogger(__name__)
 
 
 def is_url(url):
     try:
         result = urlparse(url)
@@ -137,15 +138,15 @@
     # TODO: we need at least define an interface which is cmopatible with
     #       the document class
     docs: dask.bag.Bag
 
     def apply(self, questions: list[str]) -> list[str]: ...
 
 
-def calculate_a_d_ratio(ft: str):
+def calculate_a_d_ratio(ft: str) -> float:
     """
     calculate the retaio of digits vs alphabeticsin a string
 
     can be between 0.0 (no letters) and 1.0 (all letters)
     """
     alphas = sum(1 for c in ft if c.isalpha())
     digits = sum(1 for c in ft if c.isdigit())
@@ -259,39 +260,53 @@
 
     # TODO: rename extractors to operators
     _operators = {
         # .pdf
         "application/pdf": [
             PDFFileLoader()
             .pipe(fobj="raw_content", page_numbers="_page_numbers", max_pages="_max_pages")
-            .out("pages_bbox", "elements", meta="meta_pdf", pages="page_set")
-            .cache(),
-            FunctionOperator(lambda pages: len(pages))
+            .out("pages_bbox", "elements", meta="meta_pdf", pages="page_set").cache().docs(),
+            Configuration(image_dpi=200)
+            .docs("The dpi when rendering the document"),
+            PDFImageRenderer()
+            .pipe(fobj="raw_content", dpi="image_dpi", page_numbers="page_set")
+            .out("images").cache(),
+            FunctionOperator(lambda pages: len(pages)).t(int)
             .pipe(pages="page_set").out("num_pages").cache(),
             # TODO: move these filters etc... into a generalized text-structure pipeline!
             #  we are converting pandoc elements into the same thing
             #  anyways!!
             DocumentElementFilter(element_type=ElementType.Text)
             .pipe("elements").out("line_elements").cache(),
             DocumentElementFilter(element_type=ElementType.Graphic)
             .pipe("elements").out("graphic_elements").cache(),
+            DocumentElementFilter(element_type=ElementType.Image)
+            .pipe("elements").out("image_elements").cache(),
             ListExtractor().cache()
             .pipe("line_elements").out("lists"),
             TableCandidateAreasExtractor()
             .pipe("graphic_elements", "line_elements", "pages_bbox", "text_box_elements", "filename")
             .out("table_candidates", box_levels="table_box_levels").cache(),
-            FunctionOperator(lambda candidates: [t.df for t in candidates if t.is_valid])
-            .pipe(candidates="table_candidates").out("table_df0").cache(),
-            FunctionOperator(lambda table_df0, lists: table_df0 + [lists]).cache()
+            FunctionOperator[list[pd.DataFrame]](
+                lambda candidates: {
+                    "table_df0": [t.df for t in candidates if t.is_valid],
+                    "table_areas": pd.DataFrame([t._initial_area for t in candidates if t.is_valid])
+                }).pipe(candidates="table_candidates")
+            .out("table_df0", "table_areas").cache().t(table_df0=list[pd.DataFrame], table_areas=list[np.ndarray])
+            .docs(
+                table_df0="Filter valid tables from table candidates by looking if meaningful values can be extracted",
+                table_areas="Areas of all detected tables"
+            ),
+            FunctionOperator[list[pd.DataFrame]](lambda table_df0, lists: table_df0 + [lists]).cache()
             .pipe("table_df0", "lists").out("tables_df").cache(),
             TextBoxElementExtractor()
             .pipe("line_elements").out("text_box_elements").cache(),
-            FunctionOperator(lambda df: df.get("text", None).to_list())
+            FunctionOperator[list[str]](lambda df: df.get("text", None).to_list())
             .pipe(df="text_box_elements").out("text_box_list").cache(),
-            FunctionOperator(lambda tb: "\n\n".join(tb))
+            FunctionOperator(lambda tb: "\n\n".join(tb)).t(str)
             .pipe(tb="text_box_list").out("full_text").cache(),
             TitleExtractor()
             .pipe("line_elements").out("titles", "side_titles").cache(),
             LanguageExtractor().cache()
             .pipe(text="full_text").out("language").cache()
         ],
         # .html
@@ -301,15 +316,15 @@
             .out("main_content_clean_html", "summary", "language", "goose_article",
                  "main_content", "schemadata", "final_urls", "pdf_links", "title",
                  "short_title", "url", tables="tables_df", html_keywords="html_keywords_str").cache(),
             FunctionOperator(lambda article: article.links)
             .pipe(article="goose_article").out("urls").cache(),
             FunctionOperator(lambda article: article.top_image)
             .pipe(article="goose_article").out("main_image").cache(),
-            Alias(full_text="main_content"),
+            Alias(full_text="main_content").t(str),
             FunctionOperator(lambda x: pd.DataFrame(get_text_only_blocks(x), columns=["text"])).cache()
             .pipe(x="raw_content").out("text_box_elements"),
             FunctionOperator(lambda t, s: [t, s])
             .pipe(t="title", s="short_title").out("titles").cache(),
             FunctionOperator(lambda x: {w.strip() for w in x.split(",")})
             .pipe(x="html_keywords_str").out("html_keywords").cache(),
 
@@ -333,15 +348,15 @@
         "pandoc": [
             PandocLoader()
             .pipe(raw_content="raw_content", document_type="document_type")
             .out("pandoc_document").cache(),
             Configuration(full_text_format="markdown"),
             PandocConverter()
             .pipe(output_format="full_text_format", pandoc_document="pandoc_document")
-            .out("full_text").cache(),
+            .out("full_text").t(str).cache(),
             FunctionOperator(lambda x: lambda o: PandocConverter()(x, output_format=o))
             .pipe(x="pandoc_document").out("convert_to").cache(),
             Constant(clean_format="plain"),
             PandocToPdxConverter()
             .pipe("pandoc_document").out("text_box_elements").cache().docs(
                 "split a pandoc document into text elements."),
             SectionsExtractor()
@@ -361,14 +376,16 @@
         ],
         # standard image pipeline
         "image": [
             # add a "base-document" type (.pdf) images get converted into pdfs
             # and then further processed from there
             "application/pdf",  # as we are extracting a pdf we would like to use the pdf functions...
             Configuration(ocr_lang="auto", ocr_on=True),
+            FunctionOperator(lambda x: [x]).pipe(x="raw_content")
+            .out("images").no_cache(),
             OCRExtractor()
             .pipe("ocr_on", "ocr_lang", file="raw_content")
             .out("ocr_pdf_file").cache(),
             # we need to do overwrite the pdf loading for images we inherited from
             # the ".pdf" logic as we are
             # now taking the pdf from a different variable
             PDFFileLoader()
@@ -387,141 +404,156 @@
             FunctionOperator(lambda x: dict(data=yaml.unsafe_load(x)))
             .pipe(x="full_text").out("data").cache()
             # TODO: we might need to have a special "result" message, that we
             #       pass around....
         ],
         # simple dictionary with arbitrary data from python
         "<class 'dict'>": [  # pipeline to handle data based documents
-            FunctionOperator(lambda x: yaml.dump(list_utils.deep_str_convert(x)))
+            FunctionOperator(lambda x: yaml.dump(list_utils.deep_str_convert(x))).t(str)
             .pipe(x="data").out("full_text").cache(),
             DictSelector()
             .pipe(selectable="data").out("data_sel").cache().docs(
                 "select values by key from source data in Document"),
             FunctionOperator(lambda x: pd.DataFrame([
                 str(k) + ": " + str(v) for k, v in list_utils.flatten_dict(x).items()],
                 columns=["text"]
             )).pipe(x="data").out("text_box_elements").cache(),
-            Alias(text_segments="text_box_list"),
+            Alias(text_segments="text_box_list").t(list[str]),
             FunctionOperator(lambda x: x.keys())
             .pipe(x="data").out("keys").no_cache(),
             FunctionOperator(lambda x: x.values())
             .pipe(x="data").out("values").no_cache(),
             FunctionOperator(lambda x: x.values())
             .pipe(x="data").out("items").no_cache()
         ],
         "<class 'list'>": [
-            FunctionOperator(lambda x: yaml.dump(list_utils.deep_str_convert(x)))
+            FunctionOperator(lambda x: yaml.dump(list_utils.deep_str_convert(x))).t(str)
             .pipe(x="data").out("full_text").cache(),
             FunctionOperator(lambda x: pd.DataFrame([
                 list_utils.deep_str_convert(v) for v in x],
                 columns=["text"]
             )).pipe(x="data").out("text_box_elements").cache(),
-            Alias(text_segments="text_box_list"),
+            Alias(text_segments="text_box_list").t(list[str]),
         ],
         # TODO: json, csv etc...
         # TODO: pptx, odp etc...
         "*": [
-            Alias(data="raw_content"),
-            FunctionOperator(lambda x: force_decode(x))
+            Alias(data="raw_content").t(Any).docs("The unprocessed data."),
+            FunctionOperator(lambda x: force_decode(x)).t(str)
             .pipe(x="raw_content").out("full_text").docs(
-                "will always return a string, no matter what..."),
-            Alias(clean_text="full_text"),
-            FunctionOperator(lambda x: {"meta": (x or dict())})
-            .pipe(x="_meta").out("meta"),
+                "Full text as a string value"),
+            Alias(clean_text="full_text").t(str),
+            FunctionOperator(lambda x: {"meta": (x or dict())}).t(dict[str, Any])
+            .pipe(x="_meta").out("meta").docs("Metadata of the document"),
 
             ##### calculate some metadata ####
             FunctionOperator(
                 lambda x: dict(file_meta=x(
                     "filename",
                     # "keywords",
                     "document_type",
                     "url",
                     "path",
                     "num_pages",
                     "num_words",
                     # "num_sents",
                     "a_d_ratio",
                     "language")))
-            .pipe(x="to_dict").out("file_meta").cache().docs(
-                "some fast-to-calculate metadata information about a file"),
+            .pipe(x="to_dict").t(dict[str, Any])
+            .out("file_meta").cache().docs(
+                "Some fast-to-calculate metadata information about a document"),
 
             ## Standard text splitter for splitting text along lines...
             FunctionOperator(lambda x: pd.DataFrame(x.split("\n\n"), columns=["text"]))
-            .pipe(x="full_text").out("text_box_elements").cache(),
-            FunctionOperator(lambda df: df.get("text", None).to_list())
-            .pipe(df="text_box_elements").out("text_box_list").cache(),
+            .pipe(x="full_text").out("text_box_elements").t(pd.DataFrame).cache()
+            .docs("Text boxes extracted as a pandas Dataframe with some additional metadata"),
+            FunctionOperator(lambda df: df.get("text", None).to_list()).t(list[str])
+            .pipe(df="text_box_elements").out("text_box_list").cache()
+            .docs("Text boxes as a list"),
             # TODO: replace this with a real, generic table detection
             #       e.g. running the text through pandoc or scan for html tables
             Constant(tables_df=[]),
+            # TODO: define datatype correctly
             FunctionOperator(lambda tables_df: [df.to_dict('index') for df in tables_df]).cache()
-            .pipe("tables_df").out("tables_dict"),
+            .pipe("tables_df").out("tables_dict").t(list[dict])
+            .docs("List of Table"),
             Alias(tables="tables_dict"),
             TextBlockClassifier()
             .pipe("text_box_elements").out("addresses").cache(),
 
             ## calculate some metadata values
             FunctionOperator(lambda full_text: 1 + (len(full_text) // 1000))
-            .pipe("full_text").out("num_pages").cache(),
+            .pipe("full_text").out("num_pages").cache().t(int),
             FunctionOperator(lambda clean_text: len(clean_text.split()))
-            .pipe("clean_text").out("num_words").cache(),
+            .pipe("clean_text").out("num_words").cache().t(int),
             FunctionOperator(lambda spacy_sents: len(spacy_sents))
-            .pipe("spacy_sents").out("num_sents").no_cache(),
+            .pipe("spacy_sents").out("num_sents").no_cache().t(int)
+            .docs("number of sentences"),
             FunctionOperator(calculate_a_d_ratio)
-            .pipe(ft="full_text").out("a_d_ratio").cache(),
+            .pipe(ft="full_text").out("a_d_ratio").cache()
+            .docs("Letter/digit ratio of the text"),
             FunctionOperator(
                 lambda full_text: langdetect.detect(full_text)
             ).pipe("full_text").out("language").cache()
             .default("unknown").docs(
                 "Detect language of a document, return 'unknown' in case of an error"),
 
             #########  SPACY WRAPPERS  #############
             Configuration(spacy_model_size="md", spacy_model="auto"),
             SpacyOperator()
             .pipe(
                 "language", "spacy_model",
                 full_text="clean_text", model_size="spacy_model_size"
-            ).out(doc="spacy_doc", nlp="spacy_nlp").cache(),
+            ).out(doc="spacy_doc", nlp="spacy_nlp").cache()
+            .docs("Spacy Document and Language Model for this document"),
             FunctionOperator(extract_spacy_token_vecs)
-            .pipe("spacy_doc").out("spacy_vectors"),
+            .pipe("spacy_doc").out("spacy_vectors")
+            .docs("Vectors for all tokens calculated by spacy"),
             FunctionOperator(get_spacy_embeddings)
-            .pipe("spacy_nlp").out("spacy_embeddings"),
+            .pipe("spacy_nlp").out("spacy_embeddings")
+            .docs("Embeddings calculated by a spacy transformer"),
             FunctionOperator(lambda spacy_doc: list(spacy_doc.sents))
-            .pipe("spacy_doc").out("spacy_sents"),
+            .pipe("spacy_doc").out("spacy_sents").t(list[str])
+            .docs("List of sentences by spacy nlp framework"),
             FunctionOperator(extract_noun_chunks)
             .pipe("spacy_doc").out("spacy_noun_chunks")
             .docs("exracts nounchunks from spacy. Will not be cached because it is all"
                   "in the spacy doc already"),
             ########## END OF SPACY ################
 
             EntityExtractor().cache()
-            .pipe("spacy_doc").out("entities").cache(),
+            .pipe("spacy_doc").out("entities").cache()
+            .docs("Extract entities from text"),
             # TODO: try to implement as much as possible from the constants below for all documentypes
             #       summary, urls, main_image, keywords, final_url, pdf_links, schemadata, tables_df
             # TODO: implement summarizer based on textrank
-            Alias(url="source"),
+            Alias(url="source").docs("Url of this document"),
 
             ########### VECTORIZATION (SPACY) ##########
-            Alias(sents="spacy_sents"),
-            Alias(noun_chunks="spacy_noun_chunks"),
+            Alias(sents="spacy_sents").docs("Sentences of this document"),
+            Alias(noun_chunks="spacy_noun_chunks").docs("Noun chunks of this documents"),
 
             FunctionOperator(lambda x: x.vector)
-            .pipe(x="spacy_doc").out("vector").cache(),
+            .pipe(x="spacy_doc").out("vector").cache()
+            .docs("Embeddings from spacy"),
             # TODO: make this configurable.. either we want
             #       to use spacy for this or we would rather have a huggingface
             #       model doing this...
             FunctionOperator(
                 lambda x: dict(
                     sent_vecs=np.array([e.vector for e in x]),
                     sent_ids=list(range(len(x)))))
-            .pipe(x="sents").out("sent_vecs", "sent_ids").cache(),
+            .pipe(x="sents").out("sent_vecs", "sent_ids").cache()
+            .docs("Vectors for sentences & sentence_ids"),
             FunctionOperator(
                 lambda x: dict(
                     noun_vecs=np.array([e.vector for e in x]),
                     noun_ids=list(range(len(x)))))
-            .pipe(x="noun_chunks").out("noun_vecs", "noun_ids").cache(),
+            .pipe(x="noun_chunks").out("noun_vecs", "noun_ids").cache()
+            .docs("Vectors for nouns and corresponding noun ids in order to find them in the spacy document"),
 
             ########### VECTORIZATION (Huggingface) ##########
             Alias(sents="spacy_sents"),
             Alias(noun_chunks="spacy_noun_chunks"),
             Configuration(
                 vectorizer_model="sentence-transformers/all-MiniLM-L6-v2",
                 vectorizer_only_tokenizer=False,
@@ -532,19 +564,22 @@
                    "contextual embeddings using the model. BUt is also lower quality"
                    "because it lacks the context."),
             FunctionOperator(
                 lambda x, m, t, o: nlp_utils.calculate_string_embeddings(
                     text=x, model_id=m, only_tokenizer=t, overlap_ratio=o)
             ).pipe(x="full_text", m="vectorizer_model",
                    t="vectorizer_only_tokenizer", o="vectorizer_overlap_ratio")
-            .out("vec_res").cache(),
+            .out("vec_res").cache()
+            .docs("Calculate context-based vectors for the entire text"),
             FunctionOperator(lambda x: dict(emb=x[0], tok=x[1]))
-            .pipe(x="vec_res").out(emb="tok_embeddings", tok="tokens").no_cache(),
-            FunctionOperator(lambda x: x.mean(0))
-            .pipe(x="tok_embeddings").out("embedding").cache(),
+            .pipe(x="vec_res").out(emb="tok_embeddings", tok="tokens").no_cache()
+            .docs("Get the tokenized text"),
+            FunctionOperator[list[float]](lambda x: x.mean(0))
+            .pipe(x="tok_embeddings").out("embedding").cache()
+            .docs("Get an embedding for the entire text"),
 
             ########### SEGMENT_INDEX ##########
             Configuration(
                 min_size_text_segment=256,
                 max_size_text_segment=512,
                 text_segment_overlap=0.3,
                 max_text_segment_num=100,
@@ -896,15 +931,15 @@
             return "*"
 
     def __repr__(self):
         """
         Returns:
             str: A string representation of the instance.
         """
-        if isinstance(self._source, (str,bytes)):
+        if isinstance(self._source, (str, bytes)):
             return f"{self.__module__}.{self.__class__.__name__}(source={self.source[:10]})"
         else:
             return f"{self.__module__}.{self.__class__.__name__}(source={self.source})"
 
     """
     @property
     def final_url(self) -> list[str]:
```

### Comparing `pydoxtools-0.6.4/pydoxtools/document_base.py` & `pydoxtools-0.6.5/pydoxtools/document_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations  # this is so, that we can use python3.10 annotations..
 
 import functools
+import typing
 import json
+import pydantic
 import logging
 import pathlib
 import pickle
 import sys
 import uuid
 from dataclasses import dataclass
 from enum import Enum
@@ -423,15 +425,15 @@
         return out
 
     def non_interactive_pipeline(self) -> dict[str, Operator]:
         """return all non-interactive extractors/pipeline nodes"""
         NotImplementedError("TODO: search for functions that are type hinted as callable")
 
     @classmethod
-    def pipeline_docs(cls, pipeline_type=None):
+    def operator_infos(cls, pipeline_type=None) -> dict[str, dict[str, Any]]:
         """
         Aggregates the pipeline operations and their corresponding types and metadata.
 
         This method iterates through all the pipelines registered in the class, and gathers
         information about each operation, such as the pipeline types it appears in,
         the return type of the operation, and the operation's docstring.
 
@@ -439,21 +441,35 @@
             output_infos (Dict[str, Dict[str, Union[Set, str]]]): The aggregated information
                 about pipeline operations, with operation keys as the top-level keys, and
                 metadata such as pipeline types, output types, and descriptions as nested
                 dictionaries.
         """
         output_infos = {}
         # aggregate information
+        op: Operator
         for pipeline_id, ops in cls._pipelines.items():
             for op_k, op in ops.items():
-                oi: dict[str, set] = output_infos.get(op_k, None) or dict(pipe_types=set(), output_types=set())
+                # BUG: TODO: find a better method here than just "overwriting" operator information
+                #       for different pipelines
+                oi: dict[str, set] = output_infos.get(op_k, None) or dict(
+                    pipe_types=set(), output_types=set(), operator_class=set())
                 oi["pipe_types"].add(pipeline_id)
-                if return_type := get_type_hints(op.__class__.__call__).get("return", None):
-                    oi["output_types"].add(return_type)
-                oi["description"] = op.__node_doc__
+                if return_type := op.return_type:
+                    oi["output_types"].add(return_type[op_k])
+                else:
+                    oi["output_types"].add(typing.Any)
+                # TODO: merge multiple descriptions by making clear which description is for which pipeline type.
+                try:
+                    oi["description"] = op.documentation[op_k]
+                except TypeError:
+                    oi["description"] = op.documentation
+                oi["description"] = oi["description"].strip()
+                # TODO: merge multiple callable params by pipeline type.
+                oi["callable_params"] = getattr(op, "callable_params", None)
+                oi["operator_class"].add(op.__class__)
                 output_infos[op_k] = oi
 
         if pipeline_type:
             return output_infos[pipeline_type]
         else:
             return output_infos
 
@@ -465,15 +481,15 @@
         This class method iterates through the pipeline operations, collects information about their
         output types and supported pipelines, and formats the documentation accordingly.
 
         Returns:
             str: A formatted string containing the documentation for each pipeline operation, including
                  operation name, usage, return type, and supported pipelines.
         """
-        output_infos = cls.pipeline_docs()
+        output_infos = cls.operator_infos()
 
         node_docs = []
         for k, v in output_infos.items():
             return_types = " | ".join(sorted(str(i) for i in v['output_types']))
             return_types = return_types.replace(">", r"\>")
             pipeline_flows = ", ".join(sorted(v['pipe_types']))
             pipeline_flows = pipeline_flows.replace(">", r"\>")
@@ -512,48 +528,46 @@
         Returns:
             dict: A dictionary containing the mapped keys and their corresponding values.
         """
         mapped_kwargs = {}
         # get all required input parameters from _in_mapping which was declared with "pipe"
         for k, v in kwargs.items():
             # first check if parameter is available as an extractor
-            if v in self.x_funcs:
-                # then call the function to get the value
-                mapped_kwargs[k] = self.x(v)
-            else:
-                # get "native" member-variables or other functions
-                # if not found an extractor with that name
-                mapped_kwargs[k] = getattr(self, v)
+            mapped_kwargs[k] = self.x(v)
         return mapped_kwargs
 
-    def x(self, operator_name: str) -> Any:
+    def x(self, operator_name: str, disk_cache: bool = False) -> Any:
         """
         Calls an extractor from the defined pipeline and returns the result.
 
         Args:
             operator_name (str): The name of the extractor to be called.
+            cache: if we want to cache the call. We can explicitly tell
+                    the pipeline to cache a call. to make caching more efficient
+                    by only caching the calls we want.
 
         Returns:
             Any: The result of the extractor after processing the document.
 
         Raises:
             operators.OperatorException: If an error occurs while executing the extractor.
 
         Notes:
             The extractor's parameters can be overridden using *args and **kwargs.
         """
         # override the operator if this instance has its own configuration
         if operator_name in self._configuration:
             return self._configuration[operator_name]
         elif not (operator_function := self.x_funcs.get(operator_name, None)):
-            return self.__dict__[operator_name]  # choose the class' own properties as a fallback
+            return super().__getattribute__(operator_name)  # choose the class' own properties as a fallback
 
         try:
             # whether function should be cached or not...
             finished_calculation = False
+            use_disk_cache = self._disk_cache_enabled or disk_cache
             # taking the operator_function instead of the output as a key makes everything here more
             # efficient, because we don't have to store the output for individual
             # keys in case a function has multiple keys as an output...
             dict_cache_key = operator_function
             disk_cache_key = None
             if operator_function._cache:
                 # first check if we already have the result in memory-cache,
@@ -565,15 +579,15 @@
                 # we need to check for "is not None" as we also have pandas dataframes in this
                 # which cannot be checked for by simply using "if"
                 if (res := self._cache.get(dict_cache_key, None)) is not None:
                     self._stats["cache_hits"] += 1
                     finished_calculation = True
 
                 # TODO: hash pandas.util.hash_pandas_object for mapped kwargs key
-                if (not finished_calculation) and self._disk_cache_enabled \
+                if (not finished_calculation) and use_disk_cache \
                         and operator_function._allow_disk_cache:
                     # We are creating a key using a hash value
                     # for this specific instance of a pipeline object.
                     # this key should be provided by the pipeline itself.
                     # we can not use the function arguments as keys, as they are iteratively
                     # calculated through the pipeline. this means
                     # that we would have to calculate the entire tree in the pipeline to get the
@@ -604,15 +618,15 @@
                     except:
                         res = operator_function._default
                 else:
                     res = operator_function(**mapped_kwargs)
                 # and save the result in both caches
                 if operator_function._cache:
                     self._cache[dict_cache_key] = res
-                    if self._disk_cache_enabled and disk_cache_key:
+                    if use_disk_cache and disk_cache_key:
                         try:
                             # self._disk_cache.set(disk_cache_key, res, expire=self._disk_cache_ttl)
                             self._disk_cache.set(disk_cache_key, res)
                         except (pickle.PicklingError, AttributeError, TypeError) as error:
                             self._stats["cache_errors"].add((operator_name, error))
 
             # TODO: this can probably made more elegant
@@ -644,14 +658,61 @@
 
     def get(self, property: str, default_return: Any = None) -> Any:
         try:
             return self.x(property)
         except KeyError:
             return default_return
 
+    @classmethod
+    def operator_types(cls, json_schema=False):
+        """
+        This function returns a dictionary of operators with their types
+        which is suitable for declaring a pydantic model.
+
+        json_schema: if this is set to True, we make sure that only valid json
+                     schema types are included in the model.
+                     The typical use case is to expose the pipeline via this
+                     model to an http API e.g. through fastapi. In this
+                     case we should only allow types that are valid json schema.
+                     Therefore, this is set to "False" by default.
+        """
+        # get types
+        types = cls.operator_infos()
+        operator_signatures = {}
+        for k, v in types.items():
+            operator_types = tuple(t for t in v['output_types']) or typing.Any
+            if isinstance(operator_types, typing.Tuple):
+                operator_types = typing.Union[operator_types]
+            # check if we can generate json schema otherwise omit value:
+            try:
+                pydantic.schema_json_of(operator_types)
+            except:
+                if json_schema:
+                    # if a model should be a valid json schema, omit the definition
+                    continue
+            arg = (typing.Optional[operator_types],
+                   pydantic.Field(
+                       None, description=v['description'],
+                       callable_params=v['callable_params'],
+                       operator_class=v['operator_class']
+                   ))
+            operator_signatures[k] = arg
+
+        return operator_signatures
+
+    @classmethod
+    def Model(cls):
+        operator_signatures = cls.operator_types(json_schema=True)
+
+        class Config:
+            arbitrary_types_allowed = True
+
+        PydanticModel = pydantic.create_model(cls.__name__, **operator_signatures, __config__=Config)
+        return PydanticModel
+
     def __getitem__(self, extract_name) -> Any:
         """
         Retrieves an extractor result by directly accessing it as an attribute.
 
         This method is automatically called for attribute names that
         aren't defined on class level, allowing for a convenient
         way to access pipeline operator outputs without needing to call the 'x' method.
@@ -687,16 +748,16 @@
             Any: The result of the extractor after processing the document.
         """
         return self.x(extract_name)
 
     def __getstate__(self):
         """
         return necessary variables for pickling, ensuring that
-        we leave out everything that can potentiall have some sort
-        of a lambda function in it...
+        we leave out everything that can potentially have
+        a lambda function in it...
         """
         state = self.__dict__.copy()
         drop_vars = [
             "x_funcs", "_pipelines", "_cache",
             "_disk_cache", "_operators",
         ]
         for v in drop_vars:
```

### Comparing `pydoxtools-0.6.4/pydoxtools/extract_classes.py` & `pydoxtools-0.6.5/pydoxtools/extract_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations  # this is so, that we can use python3.10 annotations..
 
 import logging
+import typing
 
 import langdetect
 import pandas as pd
 from transformers import AutoModelForSequenceClassification, pipeline, AutoTokenizer
 
 from pydoxtools.operators_base import Operator
 from pydoxtools.settings import settings
@@ -22,15 +23,15 @@
         return lang
 
 
 class TextBlockClassifier(Operator):
     def __init__(self):
         super().__init__()
 
-    def __call__(self, text_box_elements: pd.DataFrame):
+    def __call__(self, text_box_elements: pd.DataFrame) -> list[str]:
         tokenizer = AutoTokenizer.from_pretrained("bert-base-uncased")
         model_name = "txtblockclassifier"
         model_dir = settings.PDX_MODEL_DIR / model_name
         if not model_dir.exists():
             # TODO: download "any" model that we want from transformers
             logger.info(f"model {model_name} not found in pydoxtools models, download directly from transformers!")
             model_dir = "xyntopia/tb_classifier"
```

### Comparing `pydoxtools-0.6.4/pydoxtools/extract_filesystem.py` & `pydoxtools-0.6.5/pydoxtools/extract_filesystem.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.4/pydoxtools/extract_html.py` & `pydoxtools-0.6.5/pydoxtools/extract_html.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.4/pydoxtools/extract_index.py` & `pydoxtools-0.6.5/pydoxtools/extract_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import uuid
 from typing import Callable
 
 import dask.bag
 import hnswlib
 import networkx as nx
 import numpy as np
+import pydantic
 
 import pydoxtools
 from pydoxtools.document_base import TokenCollection
 from pydoxtools.nlp_utils import calculate_string_embeddings
 from pydoxtools.operators_base import Operator
 from . import list_utils
 
@@ -32,15 +33,15 @@
     if we split up large text blocks we will let the individual pieces overlap
     just a little bit in order to preserve some of the context.
     """
 
     def __call__(
             self, full_text, min_size: int = 256, max_size: int = 512,
             large_segment_overlap=0.3, max_text_segment_num=100,
-    ):
+    ) -> list[str]:
         # TODO: also accept text elements which have bounding boxes for better text box identification.
         # TODO: identify tables and convert them into a readable format.
         # TODO: identify other things such as images, plots etc..  and convert them into
         #       a vector
         # TODO: use this approach for faster questions-answering!
         split_text = full_text.split("\n\n")
 
@@ -127,20 +128,25 @@
         # Controlling the recall by setting ef:
         # index.set_ef(100)  # ef should always be > k
 
         return index
 
 
 class KnnQuery(Operator):
+    class callable_params(pydoxtools.operators_base.OperatorParams):
+        txt: str | np.ndarray | TokenCollection
+        k: int = 5
+        indices = False
+
     def __call__(
             self,
             index: hnswlib.Index,
             idx_values: list,
             vectorizer: Callable,  # e.g. lambda spacy_nlp, txt: spacy_nlp spacy_nlp(txt).vector
-    ) -> Callable:
+    ) -> Callable[..., list[tuple]]:
         def knn_query(txt: str | np.ndarray | TokenCollection, k: int = 5, indices=False) -> list[tuple]:
             if isinstance(txt, str):
                 search_vec = vectorizer(txt)
             elif isinstance(txt, np.ndarray):
                 search_vec = txt
             else:
                 search_vec = txt.vector
```

### Comparing `pydoxtools-0.6.4/pydoxtools/extract_nlpchat.py` & `pydoxtools-0.6.5/pydoxtools/extract_nlpchat.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
                         model_id=model_id, temperature=0.0, messages=msgs
                     )
                     result = completion.choices[0].message
                 elif model_id in gpt4_models():
                     completion = gpt4allchat(
                         model_id=model_id, temperature=0.0, messages=msgs
                     )
-                    res = ["choices"][0]['message']['content']
+                    result = completion["choices"][0]['message']['content']
                 else:
                     NotImplementedError(f"We can currently not handle the model {model_id}")
 
                 results.append(result)
             return results
 
         # list models
```

### Comparing `pydoxtools-0.6.4/pydoxtools/extract_objects.py` & `pydoxtools-0.6.5/pydoxtools/extract_objects.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.4/pydoxtools/extract_ocr.py` & `pydoxtools-0.6.5/pydoxtools/extract_ocr.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.4/pydoxtools/extract_pandoc.py` & `pydoxtools-0.6.5/pydoxtools/extract_pandoc.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.4/pydoxtools/extract_spacy.py` & `pydoxtools-0.6.5/pydoxtools/extract_spacy.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 import subprocess
 import typing
 from typing import Optional, Any
 
 import numpy as np
 import spacy
+import torch
 from spacy import Language
 from spacy.tokens import Doc, Token, Span
 
 from .document_base import TokenCollection
 from .operators_base import Operator
 
 logger = logging.getLogger(__name__)
@@ -27,15 +28,15 @@
         tc = TokenCollection([t for t in nc if t.pos_ not in ["DET", "SPACE", "PRON"]])
         if len(tc) > 0:
             token_list.append(tc)
     # filter = ["DET"]
     return token_list
 
 
-def extract_spacy_token_vecs(spacy_doc):
+def extract_spacy_token_vecs(spacy_doc) -> torch.Tensor | Any:
     if spacy_doc.has_vector:
         return spacy_doc.tensor
     else:
         return spacy_doc._.trf_token_vecs
 
 
 def get_spacy_embeddings(spacy_nlp):
@@ -149,15 +150,15 @@
 class SpacyOperator(Operator):
     def __call__(
             self,
             full_text: str,
             language: str,
             spacy_model: str,
             model_size: str
-    ) -> typing.Dict[str, Any]:
+    ) -> typing.Dict[str, Language | Doc]:
         """Load a document using spacy"""
         if spacy_model == "auto":
             nlp_modelid = get_spacy_model_id(language, model_size)
         else:
             nlp_modelid = spacy_model
 
         spacy_nlp = load_cached_spacy_model(nlp_modelid)
```

### Comparing `pydoxtools-0.6.4/pydoxtools/extract_tables.py` & `pydoxtools-0.6.5/pydoxtools/extract_tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,15 +196,15 @@
 
 
 class ListExtractor(Operator):
     """
     Extract lines that might be part of a "list".
     """
 
-    def __call__(self, line_elements: pd.DataFrame):
+    def __call__(self, line_elements: pd.DataFrame) -> pd.DataFrame:
         # search for lines that are part of lists
         # play around with this expression here: https://regex101.com/r/xrnKlm/1
         degree_search = r"^[\-\*∙•](?![\d\-]+\s?(?:(?:[°˚][CKF]?)|[℃℉]))"
         has_list_char = line_elements.rawtext.str.strip().str.contains(degree_search, regex=True, flags=re.UNICODE)
         list_lines = line_elements[has_list_char].rawtext.str.strip().to_frame()
 
         return list_lines
```

### Comparing `pydoxtools-0.6.4/pydoxtools/extract_textstructure.py` & `pydoxtools-0.6.5/pydoxtools/extract_textstructure.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 class DocumentElementFilter(pydoxtools.operators_base.Operator):
     """Filter document elements for various criteria"""
 
     def __init__(self, element_type: document_base.ElementType):
         super().__init__()
         self.element_type = element_type
 
-    def __call__(self, elements: pd.DataFrame):
+    def __call__(self, elements: pd.DataFrame) -> pd.DataFrame:
         df = elements.loc[elements["type"] == self.element_type].copy()
         return df
 
 
 def group_elements(elements: pd.DataFrame, by: list[str], agg: str):
     group = elements.groupby(by)
     if agg == "boxes_from_lines_w_bb":
@@ -118,15 +118,15 @@
     TODO: detect textboxes if they weren't loaded from another framewok
           already (for example pdfminer.six automatically detects textboxes ad
           we save them in the elements array)
 
     TODO: do some schema validation on the pandas dataframes...
     """
 
-    def __call__(self, line_elements: pd.DataFrame):
+    def __call__(self, line_elements: pd.DataFrame) -> dict[str, pd.DataFrame | None]:
         if "boxnum" in line_elements:
             bg = group_elements(line_elements, ['p_num', 'boxnum'], agg="boxes_from_lines_w_bb")
             return dict(text_box_elements=bg)
         else:
             return dict(text_box_elements=None)
 
 
@@ -167,15 +167,15 @@
         TODO: convert this function into a function of "feature-generation"
               and move the anomaly detection into the cached_property functions
         """
 
         # TODO: extract the necessary features that we need here "on-the-fly" from
         #       LTLineObj
         # extract more features for every line
-        dfl = df_le
+        dfl = df_le.dropna(axis=1).copy()
         # get font with largest size to characterize line
         # TODO: this can probably be made better..  (e.g. only take the font of the "majority" content)
         dfl[['font', 'size', 'color']] = dfl.font_infos.apply(
             lambda x: pd.Series(asdict(max(x, key=operator.attrgetter("size"))))
         )
 
         # generate some more features
```

### Comparing `pydoxtools-0.6.4/pydoxtools/file_utils.py` & `pydoxtools-0.6.5/pydoxtools/file_utils.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.4/pydoxtools/html_utils.py` & `pydoxtools-0.6.5/pydoxtools/html_utils.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.4/pydoxtools/labeling.py` & `pydoxtools-0.6.5/pydoxtools/labeling.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.4/pydoxtools/list_utils.py` & `pydoxtools-0.6.5/pydoxtools/list_utils.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.4/pydoxtools/models.py` & `pydoxtools-0.6.5/pydoxtools/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,15 @@
         return self
 
     def decompress(self):
         self.html = gzip.decompress(self.html).decode('utf-8') if self.html else None
         return self
 
 
+# TODO: get rid of this.  this is now generic and generated by the pipeline class
 class DocumentExtract(BaseModel):
     uid: str | None
     source: str = Field(
         ..., description="Where does the extracted data come from? (Examples: URL, 'pdfupload', parent-URL, or a path)"
     )
     type: str = Field(..., description="filetype of the data such as 'html' or 'pdf' or 'doc'")
     filename: str | None
```

### Comparing `pydoxtools-0.6.4/pydoxtools/nlp_utils.py` & `pydoxtools-0.6.5/pydoxtools/nlp_utils.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.4/pydoxtools/ocr_language_mappings.py` & `pydoxtools-0.6.5/pydoxtools/ocr_language_mappings.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.4/pydoxtools/operator_huggingface.py` & `pydoxtools-0.6.5/pydoxtools/operator_huggingface.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.4/pydoxtools/operators.py` & `pydoxtools-0.6.5/pydoxtools/operators.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.4/pydoxtools/pdf_utils.py` & `pydoxtools-0.6.5/pydoxtools/pdf_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,29 +7,41 @@
 # alternatives to camelot:
 # https://github.com/tabulapdf/tabula for "stream-tables"
 # 
 
 
 from __future__ import annotations  # this is so, that we can use python3.10 annotations..
 
+import typing
+from io import StringIO
+
+from pdfminer.converter import TextConverter
+from pdfminer.layout import LAParams
+import pdf2image
+import PIL
+from pdfminer.pdfdocument import PDFDocument
+from pdfminer.pdfinterp import PDFResourceManager, PDFPageInterpreter
+from pdfminer.pdfpage import PDFPage
+from pdfminer.pdfparser import PDFParser
 import functools
+import numpy as np
 import io
 import logging
 from pathlib import Path
 
 import pandas as pd
 # TODO: evaluate tabula as an additional table-read mechanism
 import pdfminer
 import pdfminer.high_level
 import pdfminer.pdfdocument
 import pdfminer.psparser
 import pikepdf
 from pdfminer.high_level import extract_pages
 from pdfminer.layout import LAParams
-from pdfminer.layout import LTChar, LTCurve, LTFigure, LTTextLine
+from pdfminer.layout import LTChar, LTCurve, LTFigure, LTTextLine, LTAnno
 from pdfminer.layout import LTTextContainer
 from pdfminer.pdfinterp import resolve1
 from pdfminer.pdfparser import PDFParser
 
 import pydoxtools.operators_base
 from pydoxtools import document_base, list_utils
 
@@ -52,17 +64,20 @@
 > pdftotext -layout PFR-PR05-HRVI-6HD-Flyer-V1.00-SV003.pdf output.txt
 """
 
 
 def _set_log_levels():
     """default loglevels of the libraries used here are very verbose...
     so we can optionally decrease the verbosity here"""
-    logging.getLogger('pdfminer.pdfinterp').setLevel(logging.WARNING)
-    logging.getLogger('pdfminer.pdfdocument').setLevel(logging.WARNING)
-    logging.getLogger('pdfminer').setLevel(logging.WARNING)
+    # logging.getLogger('pdfminer.pdfinterp').setLevel(logging.WARNING)
+    # logging.getLogger('pdfminer.pdfdocument').setLevel(logging.WARNING)
+    # logging.getLogger('pdfminer').setLevel(logging.WARNING)
+    pdflogs = [logging.getLogger(name) for name in logging.root.manager.loggerDict if name.startswith('pdfminer')]
+    for ll in pdflogs:
+        ll.setLevel(logging.WARNING)
     # logging.getLogger('camelot').setLevel(logging.WARNING) #not needed anymore...
 
 
 _set_log_levels()
 
 
 def repair_pdf(pdf_file_path: str) -> str:
@@ -131,14 +146,27 @@
         except:
             logger.exception(f"Not able to process pdf: {pdf_file}")
             raise PDFRepairError(f"Not able to process pdf: {pdf_file}")
 
     return wrapper
 
 
+class PDFImageRenderer(pydoxtools.operators_base.Operator):
+    """Take a document PDF and render an image from it."""
+
+    def __call__(self, fobj: bytes, dpi: int, page_numbers: list[int]) -> dict[str, dict[PIL.Image]]:
+        images = {}
+        for page in page_numbers:
+            image = pdf2image.convert_from_bytes(
+                fobj, dpi=240, first_page=page + 1, last_page=page + 1, use_cropbox=False
+            )
+            images[page] = image[0]
+        return dict(images=images)
+
+
 def meta_infos(f: io.IOBase):
     parser = PDFParser(f)
 
     doc = pdfminer.pdfdocument.PDFDocument(parser)
 
     try:
         pagenum = resolve1(doc.catalog['Pages'])['Count']
@@ -166,50 +194,104 @@
     - extract table data
 
     TODO: move extract_elements into the page class...
     """
 
     def __init__(
             self,
-            laparams=LAParams(),
+            # laparams=LAParams(detect_vertical=True, boxes_flow=-1.0, all_texts=False),
+            laparams=LAParams(detect_vertical=False),
             **kwargs
     ):
         """
         :param laparams: An LAParams object from pdfminer.layout. If None, uses
         some default settings that often work well.
 
         LAParams(
            line_overlap=0.5,  # 0.5, are chars in the same line?
            char_margin=2.0,  # 2.0, max distance between chars in words
            word_margin=0.1,  # 0.1, max distance between words in line
            line_margin=0.5,  # 0.5, max distance between lines in box
            boxes_flow=+0.5,  # 0.5, box order
-           detect_vertical=False,
+           detect_vertical=True,
            all_texts=False
         )
         """
         super().__init__()
         self._laparams = laparams
+        self.docs(
+            pages_bbox="Return the 'mediabox' property of the pdf page which gives"
+                       " the size of the page of a pdf in 72 dpi,"
+                       " which is the standard unit of measurement in pdfs.",
+            meta="Extract metadata from pdf",
+            pages="A list of the extracted pages of the pdf",
+            elements="Extract a list of textelements from pdf: Textlines, Graphics, Figures")
+        self.t(
+            meta=typing.Any,
+            elements=pd.DataFrame,
+            pages=set[int],
+            pages_bbox=np.ndarray
+        )
 
     def __call__(self, fobj: bytes, page_numbers=None, max_pages=0):
         doc_obj = io.BytesIO(fobj)
-        docelements, extracted_page_numbers, pages_bbox = self.extract_pdf_elements(
+        docelements, extracted_page_numbers, pages_bbox = self.extract_pdf_elements_pdfsix_version(
             doc_obj, page_numbers, max_pages)
         meta = meta_infos(doc_obj)
 
         return dict(
             meta=meta,
             elements=docelements,
             pages=extracted_page_numbers,
             pages_bbox=pages_bbox
         )
 
     def extract_pdf_elements(self, fobj, page_numbers, max_pages):
         """
+        extract pdf elements "manually"  which should be a bit faster due
+        to better textbox algorithms
+        """
+
+        # read the docs here:   https://euske.github.io/pdfminer/programming.html#overview
+        output_string = StringIO()
+        with open('samples/simple1.pdf', 'rb') as in_file:
+            parser = PDFParser(in_file)
+            doc = PDFDocument(parser)
+            rsrcmgr = PDFResourceManager(caching=True)
+            #    device = PDFPageAggregator(resource_manager, laparams=laparams)
+            device = TextConverter(rsrcmgr, output_string, laparams=LAParams())
+
+            interpreter = PDFPageInterpreter(rsrcmgr, device)
+            for page in PDFPage.create_pages(doc):
+                interpreter.process_page(page)
+
+        print(output_string.getvalue())
+
+        """
+        with open_filename(pdf_file, "rb") as fp:
+            fp = cast(BinaryIO, fp)  # we opened in binary mode
+            resource_manager = PDFResourceManager(caching=caching)
+            device = PDFPageAggregator(resource_manager, laparams=laparams)
+            interpreter = PDFPageInterpreter(resource_manager, device)
+            for page in PDFPage.get_pages(
+                    fp, page_numbers, maxpages=maxpages, password=password, caching=caching
+            ):
+                interpreter.process_page(page)
+                layout = device.get_result()
+                yield layout
+        """
+
+        pass
+
+    def extract_pdf_elements_pdfsix_version(self, fobj, page_numbers, max_pages):
+        """
         extracts all text lines from a pdf and annotates them with various features.
+
+        This is the "out-of-the-box" version of pdfminer.six it is sometimes very slow.
+        Specifically for PDFs with a lot of graphic elements and small, distributed textboxes.
         TODO: make use of other pdf-pobjects as well (images, figures, drawings  etc...)
         TODO: check for already extracted pages and only extract missing ones...
         TODO: implement our own algorithm in order to identify textboxes...  the pdfminer.six
               one has problems with boxes when there is a line with a right- and a left justified
               text in the same line..  in most cases they should be split into two boxes...
         """
         docelements = []  # should be of type list[dict]
@@ -220,73 +302,94 @@
         pages_bbox = {}
 
         # iterate through pages
         for page_layout in extract_pages(fobj,
                                          laparams=self._laparams,
                                          page_numbers=page_numbers,
                                          maxpages=max_pages):
-            extracted_page_numbers.add(page_layout.pageid)
-            pages_bbox[page_layout.pageid] = page_layout.bbox
+            if page_numbers:
+                page_num = page_numbers[page_layout.pageid - 1]
+            else:
+                page_num = page_layout.pageid - 1
+            extracted_page_numbers.add(page_num)
+            pages_bbox[page_num] = np.array(page_layout.bbox)
+            # len(page_layout)
             # iterate through all page elements and translate them
             # TODO: make sure we adhere to a common schema for all file types here...
             for boxnum, element in enumerate(page_layout):
+                docelement = None
                 if isinstance(element, LTCurve):  # LTCurve are rectangles AND lines
                     # docelements should be compatible with document_base.DocumentElement
-                    docelements.append(dict(
+                    docelement = document_base.DocumentElement(
                         type=document_base.ElementType.Graphic,
                         gobj=element,
                         linewidth=element.linewidth,
                         non_stroking_color=element.non_stroking_color,
                         stroking_color=element.stroking_color,
                         stroke=element.stroke,
                         fill=element.fill,
                         evenodd=element.evenodd,
-                        p_num=page_layout.pageid,
+                        p_num=page_num,
                         boxnum=boxnum,
                         x0=element.x0,
                         y0=element.y0,
                         x1=element.x1,
                         y1=element.y1
-                    ))
+                    )
+                    docelements.append(docelement)
                 elif isinstance(element, LTTextContainer):
                     if isinstance(element, LTTextLine):
                         element = [element]
+                    # linetext = ""
                     for linenum, text_line in enumerate(element):
                         fontset = set()
                         # TODO: this could be moved somewhere else and probably be made more efficient
                         for character in text_line:
                             if isinstance(character, LTChar):
                                 charfont = document_base.Font(
                                     character.fontname, character.size,
                                     str(character.graphicstate.ncolor))
                                 fontset.add(charfont)
-                        linetext = text_line.get_text()
+                            elif isinstance(character, LTAnno):
+                                continue
+                            else:  # couldbe LTAnno,
+                                pass
+                        linetext = text_line.get_text().strip()
+                        if linetext.strip() == "":
+                            continue
                         # extract metadata
                         # TODO: move most of these function to a "feature-generation-function"
                         # which extracts the information directly from the LTTextLine object
-                        docelements.append(dict(
+                        docelement = document_base.DocumentElement(
                             type=document_base.ElementType.Text,
                             lineobj=text_line,
                             rawtext=linetext,
                             font_infos=fontset,
-                            p_num=page_layout.pageid,
+                            p_num=page_num,
                             linenum=linenum,
                             boxnum=boxnum,
                             x0=text_line.x0,
                             y0=text_line.y0,
                             x1=text_line.x1,
                             y1=text_line.y1
-                        ))
+                        )
+                        docelements.append(docelement)
                 elif isinstance(element, LTFigure):
-                    # TODO: use pdfminer.six to also group Char in LTFigure
-                    # TODO: extract text from figures as well...
-                    # chars =[e for e in list_utils.flatten(element, max_level=1)):
-                    # list(list_utils.flatten(element, max_level=1))
-                    # txt = "".join(e.get_text() for e in list_utils.flatten(element) if isinstance(e, LTChar))
-                    # es = list(list_utils.flatten(element))
-                    # import pdfminer.converter
-                    pass
+                    docelement = document_base.DocumentElement(
+                        type=document_base.ElementType.Image,
+                        p_num=page_num,
+                        boxnum=boxnum,
+                        x0=element.x0,
+                        y0=element.y0,
+                        x1=element.x1,
+                        y1=element.y1
+                    )
+                    docelements.append(docelement)
+                else:
+                    continue
+
+            logger.debug(f"process page {page_num}")
 
         # TODO: validate pandas dataframe using document_base.DocumentElement
-        docelementsframe = pd.DataFrame.from_records(docelements)
+        docelementsframe = pd.DataFrame(docelements)
 
         return docelementsframe, extracted_page_numbers, pages_bbox
```

### Comparing `pydoxtools-0.6.4/pydoxtools/random_data_generators.py` & `pydoxtools-0.6.5/pydoxtools/random_data_generators.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.4/pydoxtools/settings.py` & `pydoxtools-0.6.5/pydoxtools/settings.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.4/pydoxtools/training.py` & `pydoxtools-0.6.5/pydoxtools/training.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.4/pydoxtools/webdav_utils.py` & `pydoxtools-0.6.5/pydoxtools/webdav_utils.py`

 * *Files identical despite different names*

### Comparing `pydoxtools-0.6.4/pyproject.toml` & `pydoxtools-0.6.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydoxtools"
-version = "0.6.4"
+version = "0.6.5"
 description = "This library contains a set of tools in order to extract and synthesize structured information from documents"
 authors = ["thomas meschede <yeusblender@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://pydoxtools.xyntopia.com"
 repository = "https://github.com/xyntopia/pydoxtools"
 documentation = "https://pydoxtools.xyntopia.com"
@@ -61,15 +61,16 @@
 gpt4all = {version = "^0.2.3", optional = true}
 
 [tool.poetry.extras]
 # extraction-transformation-load facilities
 etl = ["goose3", "langdetect", "tldextract", "spacy", "pdfminer.six",
     "extruct", "urlextract", "quantulum3", "stemming",
     "quantities", "readability-lxml", "pandas", "beautifulsoup4", "hnswlib",
-    "networkx", "openai", "textract", "pandoc", "python-pptx", "dask", "pytesseract"
+    "networkx", "openai", "textract", "pandoc", "python-pptx", "dask", "pytesseract",
+    "pdf2image"
 ]
 # TODO: rename & regroups extras (e.g. light, medium average or something like that...)
 inference = ["transformers", "scikit-learn", "tqdm", "torch", "pytorch-lightning", "spacy",
     "beautifulsoup4", "pandas", "urlextract", "hnswlib", "chromadb", "gpt4all"]
 
 [tool.poetry.group.colab]
 optional = true
```

### Comparing `pydoxtools-0.6.4/PKG-INFO` & `pydoxtools-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydoxtools
-Version: 0.6.4
+Version: 0.6.5
 Summary: This library contains a set of tools in order to extract and synthesize structured information from documents
 Home-page: https://pydoxtools.xyntopia.com
 License: MIT
 Keywords: AI,document-analysis,LLM,NLP,ML
 Author: thomas meschede
 Author-email: yeusblender@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -31,15 +31,15 @@
 Requires-Dist: langdetect (>=1.0.8) ; extra == "etl"
 Requires-Dist: lxml (>=4.6.2)
 Requires-Dist: networkx (>=2.8.6,<3.0.0) ; extra == "etl"
 Requires-Dist: openai (>=0.27.4,<0.28.0) ; extra == "etl"
 Requires-Dist: packaging (>=23.0,<24.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0) ; extra == "etl" or extra == "inference"
 Requires-Dist: pandoc (>=2.3,<3.0) ; extra == "etl"
-Requires-Dist: pdf2image (>=1.16.0,<2.0.0)
+Requires-Dist: pdf2image (>=1.16.0,<2.0.0) ; extra == "etl"
 Requires-Dist: pdfminer.six (>=20200726) ; extra == "etl"
 Requires-Dist: pikepdf (>=2.10.0)
 Requires-Dist: pydantic (>=1.7.2)
 Requires-Dist: pytesseract (>=0.3.10,<0.4.0) ; extra == "etl"
 Requires-Dist: python-magic (>=0.4.27,<0.5.0)
 Requires-Dist: python-pptx (>=0.6.21,<0.7.0) ; extra == "etl"
 Requires-Dist: pytorch-lightning (>=1.5.6) ; extra == "inference"
```

