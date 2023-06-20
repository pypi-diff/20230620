# Comparing `tmp/ipr-3.8.0.tar.gz` & `tmp/ipr-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipr-3.8.0.tar", last modified: Wed Apr 19 23:25:21 2023, max compression
+gzip compressed data, was "ipr-3.9.0.tar", last modified: Wed May 17 22:15:19 2023, max compression
```

## Comparing `ipr-3.8.0.tar` & `ipr-3.9.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:25:21.828331 ipr-3.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-19 23:25:08.000000 ipr-3.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-19 23:25:08.000000 ipr-3.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-19 23:25:21.828331 ipr-3.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-19 23:25:08.000000 ipr-3.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:25:21.828331 ipr-3.8.0/ipr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:25:08.000000 ipr-3.8.0/ipr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18016 2023-04-19 23:25:08.000000 ipr-3.8.0/ipr/annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-04-19 23:25:08.000000 ipr-3.8.0/ipr/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-19 23:25:08.000000 ipr-3.8.0/ipr/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    50360 2023-04-19 23:25:08.000000 ipr-3.8.0/ipr/content.spec.json
--rw-r--r--   0 runner    (1001) docker     (123)    20267 2023-04-19 23:25:08.000000 ipr-3.8.0/ipr/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14862 2023-04-19 23:25:08.000000 ipr-3.8.0/ipr/ipr.py
--rw-r--r--   0 runner    (1001) docker     (123)    13023 2023-04-19 23:25:08.000000 ipr-3.8.0/ipr/main.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:25:08.000000 ipr-3.8.0/ipr/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14586 2023-04-19 23:25:08.000000 ipr-3.8.0/ipr/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-04-19 23:25:08.000000 ipr-3.8.0/ipr/therapeutic_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-04-19 23:25:08.000000 ipr-3.8.0/ipr/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-04-19 23:25:08.000000 ipr-3.8.0/ipr/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:25:21.828331 ipr-3.8.0/ipr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-19 23:25:21.000000 ipr-3.8.0/ipr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-19 23:25:21.000000 ipr-3.8.0/ipr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-19 23:25:21.000000 ipr-3.8.0/ipr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-19 23:25:21.000000 ipr-3.8.0/ipr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-19 23:25:21.000000 ipr-3.8.0/ipr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-19 23:25:21.000000 ipr-3.8.0/ipr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-19 23:25:08.000000 ipr-3.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-19 23:25:21.828331 ipr-3.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 23:25:08.000000 ipr-3.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 23:25:21.828331 ipr-3.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 23:25:08.000000 ipr-3.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-19 23:25:08.000000 ipr-3.8.0/tests/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-04-19 23:25:08.000000 ipr-3.8.0/tests/test_annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-04-19 23:25:08.000000 ipr-3.8.0/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-04-19 23:25:08.000000 ipr-3.8.0/tests/test_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-04-19 23:25:08.000000 ipr-3.8.0/tests/test_ipr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-19 23:25:08.000000 ipr-3.8.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-19 23:25:08.000000 ipr-3.8.0/tests/test_probe.py
--rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-04-19 23:25:08.000000 ipr-3.8.0/tests/test_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-19 23:25:08.000000 ipr-3.8.0/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-19 23:25:08.000000 ipr-3.8.0/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:15:19.280256 ipr-3.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-17 22:15:06.000000 ipr-3.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-17 22:15:06.000000 ipr-3.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-17 22:15:19.280256 ipr-3.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-17 22:15:06.000000 ipr-3.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:15:19.276255 ipr-3.9.0/ipr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:15:06.000000 ipr-3.9.0/ipr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20363 2023-05-17 22:15:06.000000 ipr-3.9.0/ipr/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-05-17 22:15:06.000000 ipr-3.9.0/ipr/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-17 22:15:06.000000 ipr-3.9.0/ipr/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51024 2023-05-17 22:15:06.000000 ipr-3.9.0/ipr/content.spec.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20207 2023-05-17 22:15:06.000000 ipr-3.9.0/ipr/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14809 2023-05-17 22:15:06.000000 ipr-3.9.0/ipr/ipr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14370 2023-05-17 22:15:06.000000 ipr-3.9.0/ipr/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:15:06.000000 ipr-3.9.0/ipr/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14586 2023-05-17 22:15:06.000000 ipr-3.9.0/ipr/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-17 22:15:06.000000 ipr-3.9.0/ipr/therapeutic_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-17 22:15:06.000000 ipr-3.9.0/ipr/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-05-17 22:15:06.000000 ipr-3.9.0/ipr/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:15:19.280256 ipr-3.9.0/ipr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-17 22:15:19.000000 ipr-3.9.0/ipr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-17 22:15:19.000000 ipr-3.9.0/ipr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-17 22:15:19.000000 ipr-3.9.0/ipr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-17 22:15:19.000000 ipr-3.9.0/ipr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-17 22:15:19.000000 ipr-3.9.0/ipr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 22:15:19.000000 ipr-3.9.0/ipr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-17 22:15:06.000000 ipr-3.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-17 22:15:19.284256 ipr-3.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 22:15:06.000000 ipr-3.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:15:19.280256 ipr-3.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:15:06.000000 ipr-3.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-17 22:15:06.000000 ipr-3.9.0/tests/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8729 2023-05-17 22:15:06.000000 ipr-3.9.0/tests/test_annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-05-17 22:15:06.000000 ipr-3.9.0/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-05-17 22:15:06.000000 ipr-3.9.0/tests/test_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-05-17 22:15:06.000000 ipr-3.9.0/tests/test_ipr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-17 22:15:06.000000 ipr-3.9.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-17 22:15:06.000000 ipr-3.9.0/tests/test_probe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-05-17 22:15:06.000000 ipr-3.9.0/tests/test_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-17 22:15:06.000000 ipr-3.9.0/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-17 22:15:06.000000 ipr-3.9.0/tests/util.py
```

### Comparing `ipr-3.8.0/LICENSE` & `ipr-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipr-3.8.0/PKG-INFO` & `ipr-3.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipr
-Version: 3.8.0
+Version: 3.9.0
 Author: ipr
 Author-email: ipr@bcgsc.ca
 Maintainer: ipr
 Maintainer-email: ipr@bcgsc.ca
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: deploy
```

### Comparing `ipr-3.8.0/README.md` & `ipr-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ipr-3.8.0/ipr/annotate.py` & `ipr-3.9.0/ipr/annotate.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 from graphkb import genes as gkb_genes
 from graphkb import match as gkb_match
 from graphkb.constants import STATEMENT_RETURN_PROPERTIES
 from graphkb.genes import get_therapeutic_associated_genes
 from graphkb.match import INPUT_COPY_CATEGORIES
 from graphkb.types import Variant
 from graphkb.util import FeatureNotFoundError, convert_to_rid_list
+from pandas import isnull
 from progressbar import progressbar
 from typing import Any, Dict, List, Sequence, Set, cast
 
-from .constants import FAILED_REVIEW_STATUS
+from .constants import FAILED_REVIEW_STATUS, TMB_HIGH_CATEGORY
 from .ipr import convert_statements_to_alterations
 from .types import (
     GkbStatement,
     IprCopyVariant,
     IprExprVariant,
     IprGene,
     IprStructuralVariant,
@@ -324,26 +325,46 @@
         if not row.get('gene') and (not row.get('gene1') or not row.get('gene2')):
             # https://www.bcgsc.ca/jira/browse/GERO-56?focusedCommentId=1234791&page=com.atlassian.jira.plugin.system.issuetabpanels:comment-tabpanel#comment-1234791
             # should not match single gene SVs
             continue
 
         for var_key in VARIANT_KEYS:
             variant = row.get(var_key)
-            if not variant:
+            matches = []
+            if not variant or isnull(variant):
                 continue
             try:
-                matches = gkb_match.match_positional_variant(graphkb_conn, variant)
+                try:
+                    matches = gkb_match.match_positional_variant(graphkb_conn, variant)
+                except HTTPError as parse_err:
+                    # DEVSU-1885 - fix malformed single deletion described as substitution of blank
+                    # eg. deletion described as substitution with nothing: 'chr1:g.150951027T>'
+                    if (
+                        variant[-1] == '>'
+                        and 'g.' in variant
+                        and variant[-2].isalpha()
+                        and variant[-3].isnumeric()
+                    ):
+                        logger.warning(
+                            f"Assuming malformed deletion variant {variant} is {variant[:-2] + 'del'}"
+                        )
+                        variant = variant[:-2] + 'del'
+                        matches = gkb_match.match_positional_variant(graphkb_conn, variant)
+                    else:
+                        raise parse_err
 
                 # GERO-299 - check for conflicting nonsense and missense categories
+
                 missense = [
                     m for m in matches if 'missense' in m.get('type', m).get('displayName', '')
                 ]
                 nonsense = [
                     m for m in matches if 'nonsense' in m.get('type', m).get('displayName', '')
                 ]
+
                 missense_cat = [m for m in missense if m.get('@class', '') == 'CategoryVariant']
                 nonsense_cat = [m for m in nonsense if m.get('@class', '') == 'CategoryVariant']
                 if missense_cat and nonsense_cat:
                     conflict_names = sorted(
                         set([m.get('displayName', '') for m in nonsense + missense])
                     )
                     logger.error(
@@ -425,16 +446,16 @@
     )
 
     return alterations
 
 
 def annotate_msi(
     graphkb_conn: GraphKBConnection,
-    msi_category: str,
-    disease_name: str,
+    disease_name: str = 'cancer',
+    msi_category: str = 'microsatellite instability',
 ) -> List[KbMatch]:
     """Annotate microsatellite instablity from GraphKB in the IPR alterations format.
 
     Match to GraphKb Category variants with similar names
     Args:
         graphkb_conn: the graphkb api connection object
         msi_category: such as 'microsatellite instability'
@@ -457,7 +478,47 @@
     )
     if msi_categories:
         for ipr_row in get_ipr_statements_from_variants(graphkb_conn, msi_categories, disease_name):
             ipr_row['variant'] = msi_category
             ipr_row['variantType'] = 'msi'
             gkb_matches.append(ipr_row)
     return gkb_matches
+
+
+def annotate_tmb(
+    graphkb_conn: GraphKBConnection,
+    disease_name: str = 'cancer',
+    category: str = TMB_HIGH_CATEGORY,
+) -> List[KbMatch]:
+    """Annotate Tumour Mutation Burden (tmb) categories from GraphKB in the IPR alterations format.
+
+    Match to GraphKb Category variants with similar names
+    Args:
+        graphkb_conn: the graphkb api connection object
+        disease_name: oncotree disease name for graphkb matching.
+        category: such as 'high mutation burden'
+
+    Returns:
+        list of kbMatches records for IPR
+    """
+    gkb_matches = []
+    categories = graphkb_conn.query(
+        {
+            'target': {
+                'target': 'CategoryVariant',
+                'filters': {
+                    'reference1': {
+                        'target': 'Signature',
+                        'filters': {'OR': [{'name': category}, {'displayName': category}]},
+                    }
+                },
+            },
+            'queryType': 'similarTo',
+            'returnProperties': ['@rid', 'displayName'],
+        },
+    )
+    if categories:
+        for ipr_row in get_ipr_statements_from_variants(graphkb_conn, categories, disease_name):
+            ipr_row['variant'] = category
+            ipr_row['variantType'] = 'tmb'
+            gkb_matches.append(ipr_row)
+    return gkb_matches
```

### Comparing `ipr-3.8.0/ipr/connection.py` & `ipr-3.9.0/ipr/connection.py`

 * *Files identical despite different names*

### Comparing `ipr-3.8.0/ipr/content.spec.json` & `ipr-3.9.0/ipr/content.spec.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999919484702092%*

 * *Differences: {"'properties'": "{'structuralVariants': {'items': {'properties': {'rnaAltCount': "*

 * *                 "OrderedDict([('description', 'the number of alternate reads in the rna "*

 * *                 "supporting the mutation'), ('example', 1), ('type', ['integer', 'null'])]), "*

 * *                 "'rnaDepth': OrderedDict([('description', 'the total number of reads at this "*

 * *                 "position in the rna'), ('example', 2), ('type', ['integer', 'null'])])}}}}"}*

```diff
@@ -1193,14 +1193,30 @@
                     "omicSupport": {
                         "description": "flag to indicate this SV has supprt from both genome and transcriptome",
                         "type": [
                             "boolean",
                             "null"
                         ]
                     },
+                    "rnaAltCount": {
+                        "description": "the number of alternate reads in the rna supporting the mutation",
+                        "example": 1,
+                        "type": [
+                            "integer",
+                            "null"
+                        ]
+                    },
+                    "rnaDepth": {
+                        "description": "the total number of reads at this position in the rna",
+                        "example": 2,
+                        "type": [
+                            "integer",
+                            "null"
+                        ]
+                    },
                     "svg": {
                         "description": "svg image file content for this SV",
                         "type": [
                             "string",
                             "null"
                         ]
                     },
```

### Comparing `ipr-3.8.0/ipr/inputs.py` & `ipr-3.9.0/ipr/inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,16 @@
     'svgTitle',
     'name',
     'frame',
     'omicSupport',
     'highQuality',
     'comments',
     'library',
-    # GERO-307 - tumourAltCount and tumourDepth are available but not rnaAltCount and rnaDepth
+    'rnaAltCount',
+    'rnaDepth',
     'tumourAltCount',
     'tumourDepth',
     'germline',
     'mavis_product_id',
 ]
```

### Comparing `ipr-3.8.0/ipr/ipr.py` & `ipr-3.9.0/ipr/ipr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """
 Contains functions specific to formatting reports for IPR that are unlikely to be used
 by other reporting systems
 """
 from graphkb import GraphKBConnection
 from graphkb import statement as gkb_statement
 from graphkb import vocab as gkb_vocab
-from graphkb.types import Record
 from typing import Dict, Iterable, List, Sequence, Set, Tuple
 
 from .constants import GERMLINE_BASE_TERMS, VARIANT_CLASSES
 from .types import GkbStatement, ImageDefinition, IprFusionVariant, IprGene, IprVariant, KbMatch
-from .util import convert_to_rid_set, find_variant, logger
+from .util import find_variant, logger
 
 
 def display_evidence_levels(statement: GkbStatement) -> str:
     result = []
     for evidence_level in statement.get('evidenceLevel', []) or []:
         if isinstance(evidence_level, str):
             result.append(evidence_level)
```

### Comparing `ipr-3.8.0/ipr/main.py` & `ipr-3.9.0/ipr/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 from typing import Dict, List, Sequence
 
 from .annotate import (
     annotate_copy_variants,
     annotate_expression_variants,
     annotate_msi,
     annotate_positional_variants,
+    annotate_tmb,
     get_gene_information,
 )
 from .connection import IprConnection
-from .constants import DEFAULT_URL
+from .constants import DEFAULT_URL, TMB_HIGH, TMB_HIGH_CATEGORY
 from .inputs import (
     check_comparators,
     check_variant_links,
     preprocess_copy_variants,
     preprocess_expression_variants,
     preprocess_small_mutations,
     preprocess_structural_variants,
@@ -194,33 +195,61 @@
     else:
         graphkb_conn = GraphKBConnection()
     graphkb_conn.login(username, password)
 
     gkb_matches: List[KbMatch] = []
 
     # Signature category variants
+    tmb_variant: IprVariant = {}
+    tmb_matches = []
     if 'tmburMutationBurden' in content.keys():
-        logger.warning(
-            'GERO-296 - not yet implemented - high tumour mutation burden category matching.'
-        )
+        tmb_val = 0.0
+        tmb = {}
+        try:
+            tmb = content.get('tmburMutationBurden', {})
+            tmb_val = tmb['genomeIndelTmb'] + tmb['genomeSnvTmb']
+        except Exception as err:
+            logger.error(f"tmburMutationBurden parsing failure: {err}")
+
+        if tmb_val >= TMB_HIGH:
+            logger.warning(
+                f'GERO-296 - tmburMutationBurden high -checking graphkb matches for {TMB_HIGH_CATEGORY}'
+            )
+            if not tmb.get('key'):
+                tmb['key'] = TMB_HIGH_CATEGORY
+            if not tmb.get('kbCategory'):
+                tmb['kbCategory'] = TMB_HIGH_CATEGORY
+
+            # GERO-296 - try matching to graphkb
+            tmb_matches = annotate_tmb(graphkb_conn, kb_disease_match, TMB_HIGH_CATEGORY)
+            if tmb_matches:
+                tmb_variant['kbCategory'] = TMB_HIGH_CATEGORY  # type: ignore
+                tmb_variant['variant'] = TMB_HIGH_CATEGORY
+                tmb_variant['key'] = tmb['key']
+                tmb_variant['variantType'] = 'tmb'
+                logger.info(
+                    f"GERO-296 '{TMB_HIGH_CATEGORY}' matches {len(tmb_matches)} statements."
+                )
+                gkb_matches.extend(tmb_matches)
+                logger.debug(f"\tgkb_matches: {len(gkb_matches)}")
 
     msi = content.get('msi', [])
     msi_matches = []
     msi_variant: IprVariant = {}
     if msi:
         # only one msi variant per library
         if isinstance(msi, list):
             msi_cat = msi[0].get('kbCategory')
         elif isinstance(msi, str):
             msi_cat = msi
         else:
             msi_cat = msi.get('kbCategory')
             msi_variant = msi.copy()
         logger.info(f'Matching GKB msi {msi_cat}')
-        msi_matches = annotate_msi(graphkb_conn, msi_cat, kb_disease_match)
+        msi_matches = annotate_msi(graphkb_conn, kb_disease_match, msi_cat)
         if msi_matches:
             msi_variant['kbCategory'] = msi_cat  # type: ignore
             msi_variant['variant'] = msi_cat
             msi_variant['key'] = msi_cat
             msi_variant['variantType'] = 'msi'
             logger.info(f"GERO-295 '{msi_cat}' matches {len(msi_matches)} msi statements.")
             gkb_matches.extend(msi_matches)
@@ -258,14 +287,16 @@
     )
     logger.debug(f"\tgkb_matches: {len(gkb_matches)}")
 
     all_variants: Sequence[IprVariant]
     all_variants = expression_variants + copy_variants + structural_variants + small_mutations  # type: ignore
     if msi_matches:
         all_variants.append(msi_variant)  # type: ignore
+    if tmb_matches:
+        all_variants.append(tmb_variant)  # type: ignore
 
     if match_germline:  # verify germline kb statements matched germline observed variants
         gkb_matches = germline_kb_matches(gkb_matches, all_variants)
         if gkb_matches:
             logger.info(f"Removing {len(gkb_matches)} germline events without medical matches.")
 
     if custom_kb_match_filter:
```

### Comparing `ipr-3.8.0/ipr/summary.py` & `ipr-3.9.0/ipr/summary.py`

 * *Files identical despite different names*

### Comparing `ipr-3.8.0/ipr/therapeutic_options.py` & `ipr-3.9.0/ipr/therapeutic_options.py`

 * *Files identical despite different names*

### Comparing `ipr-3.8.0/ipr/types.py` & `ipr-3.9.0/ipr/types.py`

 * *Files identical despite different names*

### Comparing `ipr-3.8.0/ipr/util.py` & `ipr-3.9.0/ipr/util.py`

 * *Files identical despite different names*

### Comparing `ipr-3.8.0/ipr.egg-info/PKG-INFO` & `ipr-3.9.0/ipr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipr
-Version: 3.8.0
+Version: 3.9.0
 Author: ipr
 Author-email: ipr@bcgsc.ca
 Maintainer: ipr
 Maintainer-email: ipr@bcgsc.ca
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: deploy
```

### Comparing `ipr-3.8.0/ipr.egg-info/SOURCES.txt` & `ipr-3.9.0/ipr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipr-3.8.0/setup.cfg` & `ipr-3.9.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -13,29 +13,29 @@
 line_length = 100
 multi_line_output = 3
 include_trailing_comma = true
 known_standard_library = requests
 
 [metadata]
 name = ipr
-version = 3.8.0
+version = 3.9.0
 author_email = ipr@bcgsc.ca
 author = ipr
 maintainer_email = ipr@bcgsc.ca
 maintainer = ipr
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
 packages = find:
 python_requires = >=3.6
 dependency_links = []
 include_package_data = True
 install_requires = 
-	graphkb>=1.8.0, <2
+	graphkb>=1.10.1
 	biopython==1.76
 	progressbar2>=3.51.0, <4
 	pandas>=1.1.0, <2
 	jsonschema
 
 [options.extras_require]
 deploy = twine; wheel; m2r
```

### Comparing `ipr-3.8.0/tests/test_annotate.py` & `ipr-3.9.0/tests/test_annotate.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,74 +68,65 @@
     username = os.environ['IPR_USER']
     password = os.environ['IPR_PASS']
     graphkb_conn = GraphKBConnection()
     graphkb_conn.login(username, password)
     return graphkb_conn
 
 
-@pytest.mark.skipif(EXCLUDE_INTEGRATION_TESTS, reason="SDEV-3381 - github workflow failures.")
 def test_annotate_nonsense_vs_missense(graphkb_conn):
     """Verify missense (point mutation) is not mistaken for a nonsense (stop codon) mutation."""
     disease = 'cancer'
     for key in ('prot_only', 'cds_only', 'genome_only', 'pref'):
         matched = annotate_positional_variants(graphkb_conn, [TP53_MUT_DICT[key]], disease)
         # nonsense - stop codon - should not match.  This is missense not nonsense (#164:933).
         nonsense = [a for a in matched if a['kbVariant'] == 'TP53 nonsense']
         assert not nonsense, f"nonsense matched to {key}: {TP53_MUT_DICT[key]}"
         assert matched, f"should have matched in {key}: {TP53_MUT_DICT[key]}"
 
 
-@pytest.mark.skipif(EXCLUDE_INTEGRATION_TESTS, reason="SDEV-3381 - github workflow failures.")
 def test_annotate_nonsense_vs_missense_protein(graphkb_conn):
     """Verify missense (point mutation) is not mistaken for a nonsense (stop codon) mutation."""
     disease = 'cancer'
     for key in ('prot_only', 'pref'):
         matched = annotate_positional_variants(graphkb_conn, [TP53_MUT_DICT[key]], disease)
         # nonsense - stop codon - should not match.  This is missense not nonsense (#164:933).
         nonsense = [a for a in matched if 'nonsense' in a['kbVariant']]
         assert not nonsense, f"nonsense matched to {key}: {TP53_MUT_DICT[key]}"
         assert matched, f"should have matched in {key}: {TP53_MUT_DICT[key]}"
 
 
-@pytest.mark.skipif(EXCLUDE_INTEGRATION_TESTS, reason="SDEV-3381 - github workflow failures.")
 def test_annotate_structural_variants_tp53(graphkb_conn):
     """Verify alternate TP53 variants match."""
     disease = 'cancer'
     ref_key = 'prot_only'
     pref = annotate_positional_variants(graphkb_conn, [TP53_MUT_DICT[ref_key]], disease)
-    known_issues = set(['TP53:p.M237X'])  # SDEV-3122 -
     # GERO-299 - nonsense - stop codon - should not match.  This is missense not nonsense (#164:933).
     nonsense = [a for a in pref if a['kbVariant'] == 'TP53 nonsense']
     assert not nonsense
     pref_vars = set([m['kbVariant'] for m in pref])
     assert pref_vars, f"No matches to {TP53_MUT_DICT[pref]}"
     print(pref_vars)
     for key, alt_rep in TP53_MUT_DICT.items():
         if key == ref_key:
             continue
         alt = annotate_positional_variants(graphkb_conn, [alt_rep], disease)
         alt_vars = set([m['kbVariant'] for m in alt])
         diff = pref_vars.symmetric_difference(alt_vars)
         missing = pref_vars.difference(alt_vars)
 
-        known_issues = set([])
-        if 'hgvsCds' in alt_rep:
-            known_issues.add('TP53 nonsense')  # GERO-299
-        if 'p.M237' not in alt_rep:
-            known_issues.add('TP53:p.M237X')  # SDEV-3122 - not matching imprecise mutations
+        known_issues = set()
         if key == 'genome_only':
+            # genome_only matched to more precise type 'TP53 deleterious mutation' but not 'TP53 mutation'
             known_issues.add('TP53 mutation')
 
-        # strangely genome_only matched to more precise type 'TP53 deleterious mutation' but not 'TP53 mutation'
         missing = pref_vars.difference(alt_vars).difference(known_issues)
         print(alt_vars)
         assert not missing, f"{key} missing{missing}: {diff}"
 
 
-@pytest.mark.skipif(EXCLUDE_INTEGRATION_TESTS, reason="SDEV-3381 - github workflow failures.")
 def test_get_therapeutic_associated_genes(graphkb_conn):
     gene_list = get_therapeutic_associated_genes(graphkb_conn=graphkb_conn)
     assert gene_list, 'No get_therapeutic_associated_genes found'
     assert (
         len(gene_list) > 500
     ), f'Expected over 500 get_therapeutic_associated_genes but found {len(gene_list)}'
```

### Comparing `ipr-3.8.0/tests/test_connection.py` & `ipr-3.9.0/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `ipr-3.8.0/tests/test_inputs.py` & `ipr-3.9.0/tests/test_inputs.py`

 * *Files identical despite different names*

### Comparing `ipr-3.8.0/tests/test_ipr.py` & `ipr-3.9.0/tests/test_ipr.py`

 * *Files identical despite different names*

### Comparing `ipr-3.8.0/tests/test_main.py` & `ipr-3.9.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `ipr-3.8.0/tests/test_probe.py` & `ipr-3.9.0/tests/test_probe.py`

 * *Files identical despite different names*

### Comparing `ipr-3.8.0/tests/test_summary.py` & `ipr-3.9.0/tests/test_summary.py`

 * *Files identical despite different names*

### Comparing `ipr-3.8.0/tests/test_util.py` & `ipr-3.9.0/tests/test_util.py`

 * *Files identical despite different names*

