# Comparing `tmp/lamin_logger-0.6.0.tar.gz` & `tmp/lamin_logger-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamin_logger-0.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamin_logger-0.6.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamin_logger-0.6.0.tar` & `lamin_logger-0.6.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     2370 2023-06-15 15:21:07.826183 lamin_logger-0.6.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2022-07-20 09:06:09.796155 lamin_logger-0.6.0/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2022-07-20 09:06:09.796533 lamin_logger-0.6.0/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1199 2022-07-20 09:06:09.775542 lamin_logger-0.6.0/.gitignore
--rw-r--r--   0        0        0     1798 2023-06-15 19:45:48.148471 lamin_logger-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11357 2022-07-28 04:40:34.570134 lamin_logger-0.6.0/LICENSE
--rw-r--r--   0        0        0      357 2022-07-24 07:22:44.261019 lamin_logger-0.6.0/README.md
--rw-r--r--   0        0        0       54 2022-07-20 09:06:09.787660 lamin_logger-0.6.0/docs/api.md
--rw-r--r--   0        0        0     3814 2023-06-19 17:20:57.523889 lamin_logger-0.6.0/docs/changelog.md
--rw-r--r--   0        0        0      124 2022-07-24 07:22:44.261457 lamin_logger-0.6.0/docs/index.md
--rw-r--r--   0        0        0     1360 2022-07-24 07:22:44.261650 lamin_logger-0.6.0/docs/quickstart.ipynb
--rw-r--r--   0        0        0      138 2022-07-20 09:06:09.769122 lamin_logger-0.6.0/lamin-project.yaml
--rw-r--r--   0        0        0      291 2023-06-19 17:21:03.326344 lamin_logger-0.6.0/lamin_logger/__init__.py
--rw-r--r--   0        0        0     1357 2023-06-15 19:45:48.149902 lamin_logger-0.6.0/lamin_logger/_core.py
--rw-r--r--   0        0        0     7600 2023-06-17 12:43:22.076152 lamin_logger-0.6.0/lamin_logger/_logger.py
--rw-r--r--   0        0        0     4202 2023-06-17 12:43:22.076659 lamin_logger-0.6.0/lamin_logger/_lookup.py
--rw-r--r--   0        0        0     6306 2023-06-19 17:18:48.694840 lamin_logger-0.6.0/lamin_logger/_map_synonyms.py
--rw-r--r--   0        0        0      683 2023-06-15 19:45:48.150822 lamin_logger-0.6.0/lamin_logger/_python_version.py
--rw-r--r--   0        0        0     3056 2023-06-19 17:18:48.695302 lamin_logger-0.6.0/lamin_logger/_search.py
--rw-r--r--   0        0        0      321 2023-06-17 12:43:22.077332 lamin_logger-0.6.0/noxfile.py
--rw-r--r--   0        0        0      898 2023-06-17 12:43:22.077532 lamin_logger-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      115 2023-06-15 19:45:48.151666 lamin_logger-0.6.0/tests/test_base.py
--rw-r--r--   0        0        0     1489 2023-06-17 12:43:22.077768 lamin_logger-0.6.0/tests/test_lookup.py
--rw-r--r--   0        0        0     5093 2023-06-19 17:18:48.695758 lamin_logger-0.6.0/tests/test_map_synonyms.py
--rw-r--r--   0        0        0      417 2023-06-15 15:21:07.828069 lamin_logger-0.6.0/tests/test_notebooks.py
--rw-r--r--   0        0        0     2595 2023-06-19 17:18:48.696179 lamin_logger-0.6.0/tests/test_search.py
--rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 lamin_logger-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     2370 2023-06-15 15:21:07.826183 lamin_logger-0.6.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2022-07-20 09:06:09.796155 lamin_logger-0.6.1/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2022-07-20 09:06:09.796533 lamin_logger-0.6.1/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1199 2022-07-20 09:06:09.775542 lamin_logger-0.6.1/.gitignore
+-rw-r--r--   0        0        0     1798 2023-06-15 19:45:48.148471 lamin_logger-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11357 2022-07-28 04:40:34.570134 lamin_logger-0.6.1/LICENSE
+-rw-r--r--   0        0        0      357 2022-07-24 07:22:44.261019 lamin_logger-0.6.1/README.md
+-rw-r--r--   0        0        0       54 2022-07-20 09:06:09.787660 lamin_logger-0.6.1/docs/api.md
+-rw-r--r--   0        0        0     3969 2023-06-19 17:50:25.626594 lamin_logger-0.6.1/docs/changelog.md
+-rw-r--r--   0        0        0      124 2022-07-24 07:22:44.261457 lamin_logger-0.6.1/docs/index.md
+-rw-r--r--   0        0        0     1360 2022-07-24 07:22:44.261650 lamin_logger-0.6.1/docs/quickstart.ipynb
+-rw-r--r--   0        0        0      138 2022-07-20 09:06:09.769122 lamin_logger-0.6.1/lamin-project.yaml
+-rw-r--r--   0        0        0      291 2023-06-19 17:50:19.291064 lamin_logger-0.6.1/lamin_logger/__init__.py
+-rw-r--r--   0        0        0     1357 2023-06-15 19:45:48.149902 lamin_logger-0.6.1/lamin_logger/_core.py
+-rw-r--r--   0        0        0     7600 2023-06-17 12:43:22.076152 lamin_logger-0.6.1/lamin_logger/_logger.py
+-rw-r--r--   0        0        0     4202 2023-06-17 12:43:22.076659 lamin_logger-0.6.1/lamin_logger/_lookup.py
+-rw-r--r--   0        0        0     6453 2023-06-19 17:49:41.483006 lamin_logger-0.6.1/lamin_logger/_map_synonyms.py
+-rw-r--r--   0        0        0      683 2023-06-15 19:45:48.150822 lamin_logger-0.6.1/lamin_logger/_python_version.py
+-rw-r--r--   0        0        0     3139 2023-06-19 17:49:41.483432 lamin_logger-0.6.1/lamin_logger/_search.py
+-rw-r--r--   0        0        0      321 2023-06-17 12:43:22.077332 lamin_logger-0.6.1/noxfile.py
+-rw-r--r--   0        0        0      898 2023-06-17 12:43:22.077532 lamin_logger-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      115 2023-06-15 19:45:48.151666 lamin_logger-0.6.1/tests/test_base.py
+-rw-r--r--   0        0        0     1608 2023-06-19 17:49:41.483785 lamin_logger-0.6.1/tests/test_lookup.py
+-rw-r--r--   0        0        0     5300 2023-06-19 17:49:41.484125 lamin_logger-0.6.1/tests/test_map_synonyms.py
+-rw-r--r--   0        0        0      417 2023-06-15 15:21:07.828069 lamin_logger-0.6.1/tests/test_notebooks.py
+-rw-r--r--   0        0        0     2701 2023-06-19 17:49:41.484369 lamin_logger-0.6.1/tests/test_search.py
+-rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 lamin_logger-0.6.1/PKG-INFO
```

### Comparing `lamin_logger-0.6.0/.github/workflows/build.yml` & `lamin_logger-0.6.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.6.0/.github/workflows/latest-changes.yml` & `lamin_logger-0.6.1/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.6.0/.gitignore` & `lamin_logger-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.6.0/.pre-commit-config.yaml` & `lamin_logger-0.6.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.6.0/LICENSE` & `lamin_logger-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.6.0/docs/changelog.md` & `lamin_logger-0.6.1/docs/changelog.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🧪 Deal with empty dataframes | [28](https://github.com/laminlabs/lamin-logger/pull/28) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-19 | 0.6.1
 ✨ Add case_sensitive to map_synonyms | [27](https://github.com/laminlabs/lamin-logger/pull/27) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-19 | 0.6.0
 🧪 Test every line of search | [25](https://github.com/laminlabs/lamin-logger/pull/25) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-17 | 0.5.3
 🚑️ Fix empty string input for `map_synonyms` | [24](https://github.com/laminlabs/lamin-logger/pull/24) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-17 |
 💄 Log to stdout rather than stderr | [23](https://github.com/laminlabs/lamin-logger/pull/23) | [falexwolf](https://github.com/falexwolf) | 2023-06-16 | 0.5.2
 ✨ Lookup can also return sql records | [22](https://github.com/laminlabs/lamin-logger/pull/22) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-15 | 0.5.1
 ✨ Remove loguru and replace with standard (Scanpy-based) logger | [18](https://github.com/laminlabs/lamin-logger/pull/18) | [falexwolf](https://github.com/falexwolf) | 2023-06-15 | 0.5.0
 🚚 Moved search and map_synonyms from bionty here | [21](https://github.com/laminlabs/lamin-logger/pull/21) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-15 | 0.4.0
```

### Comparing `lamin_logger-0.6.0/docs/quickstart.ipynb` & `lamin_logger-0.6.1/docs/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.6.0/lamin_logger/_core.py` & `lamin_logger-0.6.1/lamin_logger/_core.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.6.0/lamin_logger/_logger.py` & `lamin_logger-0.6.1/lamin_logger/_logger.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.6.0/lamin_logger/_lookup.py` & `lamin_logger-0.6.1/lamin_logger/_lookup.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.6.0/lamin_logger/_map_synonyms.py` & `lamin_logger-0.6.1/lamin_logger/_map_synonyms.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,21 @@
     Returns:
         - If return_mapper is False: a list of mapped field values.
         - If return_mapper is True: a dictionary of mapped values with mappable
             identifiers as keys and values mapped to field as values.
     """
     import pandas as pd
 
+    # empty DataFrame
+    if df.shape[0] == 0:
+        if return_mapper:
+            return {}
+        else:
+            return list(identifiers)
+
     if field not in df.columns:
         raise KeyError(
             f"field '{field}' is invalid! Available fields are: {list(df.columns)}"
         )
     if synonyms_field not in df.columns:
         raise KeyError(
             f"synonyms_field '{synonyms_field}' is invalid! Available fields"
```

### Comparing `lamin_logger-0.6.0/lamin_logger/_python_version.py` & `lamin_logger-0.6.1/lamin_logger/_python_version.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.6.0/lamin_logger/_search.py` & `lamin_logger-0.6.1/lamin_logger/_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,21 @@
 
     def _fuzz_ratio(string: str, iterable: pd.Series, case_sensitive: bool = True):
         from rapidfuzz import fuzz, utils
 
         processor = None if case_sensitive else utils.default_process
         return iterable.apply(lambda x: fuzz.ratio(string, x, processor=processor))
 
+    # empty DataFrame
+    if df.shape[0] == 0:
+        if return_ranked_results:
+            return df
+        else:
+            return None
+
     # search against each of the synonyms
     if (synonyms_field in df.columns) and (synonyms_field != field):
         mapper = explode_aggregated_column_to_map(
             df,
             agg_col=synonyms_field,  # type:ignore
             target_col=field,
             keep=keep,
@@ -76,11 +83,9 @@
         return df_scored.sort_values("__ratio__", ascending=False)
     else:
         res = df_scored[df_scored["__ratio__"] == df_scored["__ratio__"].max()]
         res = res.drop(columns=["__ratio__"])
         res_records = list(res.reset_index().itertuples(index=False, name=tuple_name))
         if len(res_records) == 1:
             return res_records[0]
-        elif len(res_records) > 1:
-            return res_records
         else:
-            return None
+            return res_records
```

### Comparing `lamin_logger-0.6.0/pyproject.toml` & `lamin_logger-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.6.0/tests/test_lookup.py` & `lamin_logger-0.6.1/tests/test_lookup.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,7 +41,11 @@
     assert lookup_dict["1 sample"]._asdict() == {
         "name": "1 sample",
         "meta1": "1 metadata",
     }
 
     assert lookup.__class__.__name__ == "Lookup"
     assert lookup.prefix_1_sample.__class__.__name__ == "TestTuple"
+
+
+def test_lookup_empty_df():
+    assert Lookup(df=pd.DataFrame(columns=["name"]), field="name").lookup().dict() == {}
```

### Comparing `lamin_logger-0.6.0/tests/test_map_synonyms.py` & `lamin_logger-0.6.1/tests/test_map_synonyms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
+import pandas as pd
 import pytest
 
 from lamin_logger._map_synonyms import (
     check_if_ids_in_field_values,
     explode_aggregated_column_to_map,
     map_synonyms,
     not_empty_none_na,
     to_str,
 )
 
 
 @pytest.fixture(scope="module")
 def genes():
-    import pandas as pd
-
     gene_symbols = ["A1CF", "A1BG", "FANCD1", "FANCD20", "GCS"]
 
     records = [
         {
             "symbol": "BRCA1",
             "synonyms": "PPP1R53|RNF53|FANCS|BRCC1",
         },
@@ -116,15 +115,14 @@
             synonyms_field="symbol",
             return_mapper=False,
         )
 
 
 def test_to_str():
     import numpy as np
-    import pandas as pd
 
     assert to_str(pd.Index(["A", "a", None, np.nan])).tolist() == ["a", "a", "", ""]
     assert to_str(pd.Series(["A", "a", None, np.nan])).tolist() == ["a", "a", "", ""]
     assert to_str(
         pd.Series(["A", "a", None, np.nan]), case_sensitive=True
     ).tolist() == ["A", "a", "", ""]
 
@@ -140,15 +138,14 @@
     assert check_if_ids_in_field_values(
         identifiers=df["symbol"], field_values=df["symbol"]
     )["__mapped__"].tolist() == [True, True, True, True, True, True]
 
 
 def test_not_empty_none_na():
     import numpy as np
-    import pandas as pd
 
     assert not_empty_none_na(["a", None, "", np.nan]).loc[0] == "a"
     assert not_empty_none_na(pd.Index(["a", None, "", np.nan])).tolist() == ["a"]
     assert not_empty_none_na(
         pd.Series(["a", None, "", np.nan], index=["1", "2", "3", "4"])
     ).to_dict() == {"1": "a"}
 
@@ -182,7 +179,17 @@
             df, agg_col="synonyms", target_col="symbol", keep="last"
         ).get("GCS")
         == "UGCG"
     )
     assert explode_aggregated_column_to_map(
         df, agg_col="synonyms", target_col="symbol", keep=False
     ).get("GCS") == ["GCLC", "UGCG"]
+
+
+def test_map_synonyms_empty_df():
+    assert (
+        map_synonyms(
+            df=pd.DataFrame(), identifiers=[], field="name", return_mapper=True
+        )
+        == {}
+    )
+    assert map_synonyms(df=pd.DataFrame(), identifiers=[], field="name") == []
```

### Comparing `lamin_logger-0.6.0/tests/test_search.py` & `lamin_logger-0.6.1/tests/test_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
+import pandas as pd
 import pytest
 
 from lamin_logger._search import search
 
 
 @pytest.fixture(scope="module")
 def df():
-    import pandas as pd
-
     records = [
         {
             "ontology_id": "CL:0000084",
             "name": "T cell",
             "synonyms": "T-cell|T lymphocyte|T-lymphocyte",
             "children": ["CL:0000798", "CL:0002420", "CL:0002419", "CL:0000789"],
         },
@@ -78,12 +77,15 @@
     res = search(df=df, string="b cell", case_sensitive=True)
     assert len(res) == 3
 
     res = search(df=df, string="b cell", case_sensitive=False)
     assert res.name == "B cell"
 
 
-def test_search_return_none(df):
-    import pandas as pd
+def test_search_empty_df():
+    res = search(
+        pd.DataFrame(columns=["a", "b", "c"]), string="", return_ranked_results=True
+    )
+    assert res.shape == (0, 3)
 
-    res = search(df=pd.DataFrame([], columns=["name"]), string="")
+    res = search(pd.DataFrame(columns=["a", "b", "c"]), string="")
     assert res is None
```

### Comparing `lamin_logger-0.6.0/PKG-INFO` & `lamin_logger-0.6.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamin_logger
-Version: 0.6.0
+Version: 0.6.1
 Summary: Logging setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

