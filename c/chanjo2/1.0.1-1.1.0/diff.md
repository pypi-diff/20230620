# Comparing `tmp/chanjo2-1.0.1.tar.gz` & `tmp/chanjo2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chanjo2-1.0.1.tar", max compression
+gzip compressed data, was "chanjo2-1.1.0.tar", max compression
```

## Comparing `chanjo2-1.0.1.tar` & `chanjo2-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      734 2023-06-13 08:09:50.153914 chanjo2-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       68 2023-06-13 08:09:50.153914 chanjo2-1.0.1/src/chanjo2/__init__.py
--rw-r--r--   0        0        0     3099 2023-06-13 08:09:50.153914 chanjo2-1.0.1/src/chanjo2/constants.py
--rw-r--r--   0        0        0     2743 2023-06-13 08:09:50.153914 chanjo2-1.0.1/src/chanjo2/crud/cases.py
--rw-r--r--   0        0        0     5309 2023-06-13 08:09:50.153914 chanjo2-1.0.1/src/chanjo2/crud/intervals.py
--rw-r--r--   0        0        0     3110 2023-06-13 08:09:50.153914 chanjo2-1.0.1/src/chanjo2/crud/samples.py
--rw-r--r--   0        0        0     1067 2023-06-13 08:09:50.153914 chanjo2-1.0.1/src/chanjo2/dbutil.py
--rw-r--r--   0        0        0      346 2023-06-13 08:09:50.153914 chanjo2-1.0.1/src/chanjo2/demo/109_green.bed
--rw-r--r--   0        0        0      292 2023-06-13 08:09:50.153914 chanjo2-1.0.1/src/chanjo2/demo/__init__.py
--rw-r--r--   0        0        0   450444 2023-06-13 08:09:50.157914 chanjo2-1.0.1/src/chanjo2/demo/panelapp_109_example.d4
--rw-r--r--   0        0        0        0 2023-06-13 08:09:50.157914 chanjo2-1.0.1/src/chanjo2/endpoints/__init__.py
--rw-r--r--   0        0        0     1588 2023-06-13 08:09:50.157914 chanjo2-1.0.1/src/chanjo2/endpoints/cases.py
--rw-r--r--   0        0        0     6649 2023-06-13 08:09:50.157914 chanjo2-1.0.1/src/chanjo2/endpoints/coverage.py
--rw-r--r--   0        0        0     5278 2023-06-13 08:09:50.157914 chanjo2-1.0.1/src/chanjo2/endpoints/intervals.py
--rw-r--r--   0        0        0     2018 2023-06-13 08:09:50.157914 chanjo2-1.0.1/src/chanjo2/endpoints/samples.py
--rw-r--r--   0        0        0     1690 2023-06-13 08:09:50.157914 chanjo2-1.0.1/src/chanjo2/main.py
--rw-r--r--   0        0        0        0 2023-06-13 08:09:50.157914 chanjo2-1.0.1/src/chanjo2/meta/__init__.py
--rw-r--r--   0        0        0      694 2023-06-13 08:09:50.157914 chanjo2-1.0.1/src/chanjo2/meta/handle_bed.py
--rw-r--r--   0        0        0     6816 2023-06-13 08:09:50.157914 chanjo2-1.0.1/src/chanjo2/meta/handle_d4.py
--rw-r--r--   0        0        0     7707 2023-06-13 08:09:50.157914 chanjo2-1.0.1/src/chanjo2/meta/handle_load_intervals.py
--rw-r--r--   0        0        0        0 2023-06-13 08:09:50.157914 chanjo2-1.0.1/src/chanjo2/meta/handle_query_intervals.py
--rw-r--r--   0        0        0        0 2023-06-13 08:09:50.157914 chanjo2-1.0.1/src/chanjo2/models/__init__.py
--rw-r--r--   0        0        0     3913 2023-06-13 08:09:50.157914 chanjo2-1.0.1/src/chanjo2/models/pydantic_models.py
--rw-r--r--   0        0        0     4360 2023-06-13 08:09:50.157914 chanjo2-1.0.1/src/chanjo2/models/sql_models.py
--rw-r--r--   0        0        0     2999 2023-06-13 08:09:50.157914 chanjo2-1.0.1/src/chanjo2/populate_demo.py
--rw-r--r--   0        0        0     1066 1970-01-01 00:00:00.000000 chanjo2-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      734 2023-06-20 05:21:57.241410 chanjo2-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       68 2023-06-20 05:21:57.241410 chanjo2-1.1.0/src/chanjo2/__init__.py
+-rw-r--r--   0        0        0     3099 2023-06-20 05:21:57.241410 chanjo2-1.1.0/src/chanjo2/constants.py
+-rw-r--r--   0        0        0     2743 2023-06-20 05:21:57.241410 chanjo2-1.1.0/src/chanjo2/crud/cases.py
+-rw-r--r--   0        0        0     5309 2023-06-20 05:21:57.241410 chanjo2-1.1.0/src/chanjo2/crud/intervals.py
+-rw-r--r--   0        0        0     3110 2023-06-20 05:21:57.241410 chanjo2-1.1.0/src/chanjo2/crud/samples.py
+-rw-r--r--   0        0        0     1067 2023-06-20 05:21:57.241410 chanjo2-1.1.0/src/chanjo2/dbutil.py
+-rw-r--r--   0        0        0      346 2023-06-20 05:21:57.241410 chanjo2-1.1.0/src/chanjo2/demo/109_green.bed
+-rw-r--r--   0        0        0      292 2023-06-20 05:21:57.241410 chanjo2-1.1.0/src/chanjo2/demo/__init__.py
+-rw-r--r--   0        0        0   450444 2023-06-20 05:21:57.245410 chanjo2-1.1.0/src/chanjo2/demo/panelapp_109_example.d4
+-rw-r--r--   0        0        0        0 2023-06-20 05:21:57.245410 chanjo2-1.1.0/src/chanjo2/endpoints/__init__.py
+-rw-r--r--   0        0        0     1588 2023-06-20 05:21:57.245410 chanjo2-1.1.0/src/chanjo2/endpoints/cases.py
+-rw-r--r--   0        0        0     7089 2023-06-20 05:21:57.245410 chanjo2-1.1.0/src/chanjo2/endpoints/coverage.py
+-rw-r--r--   0        0        0     5278 2023-06-20 05:21:57.245410 chanjo2-1.1.0/src/chanjo2/endpoints/intervals.py
+-rw-r--r--   0        0        0     2018 2023-06-20 05:21:57.245410 chanjo2-1.1.0/src/chanjo2/endpoints/samples.py
+-rw-r--r--   0        0        0     1690 2023-06-20 05:21:57.245410 chanjo2-1.1.0/src/chanjo2/main.py
+-rw-r--r--   0        0        0        0 2023-06-20 05:21:57.245410 chanjo2-1.1.0/src/chanjo2/meta/__init__.py
+-rw-r--r--   0        0        0      710 2023-06-20 05:21:57.245410 chanjo2-1.1.0/src/chanjo2/meta/handle_bed.py
+-rw-r--r--   0        0        0     7091 2023-06-20 05:21:57.245410 chanjo2-1.1.0/src/chanjo2/meta/handle_d4.py
+-rw-r--r--   0        0        0     7707 2023-06-20 05:21:57.245410 chanjo2-1.1.0/src/chanjo2/meta/handle_load_intervals.py
+-rw-r--r--   0        0        0        0 2023-06-20 05:21:57.245410 chanjo2-1.1.0/src/chanjo2/meta/handle_query_intervals.py
+-rw-r--r--   0        0        0        0 2023-06-20 05:21:57.245410 chanjo2-1.1.0/src/chanjo2/models/__init__.py
+-rw-r--r--   0        0        0     4290 2023-06-20 05:21:57.245410 chanjo2-1.1.0/src/chanjo2/models/pydantic_models.py
+-rw-r--r--   0        0        0     4360 2023-06-20 05:21:57.245410 chanjo2-1.1.0/src/chanjo2/models/sql_models.py
+-rw-r--r--   0        0        0     2999 2023-06-20 05:21:57.245410 chanjo2-1.1.0/src/chanjo2/populate_demo.py
+-rw-r--r--   0        0        0     1066 1970-01-01 00:00:00.000000 chanjo2-1.1.0/PKG-INFO
```

### Comparing `chanjo2-1.0.1/pyproject.toml` & `chanjo2-1.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chanjo2"
-version = "1.0.1"
+version = "1.1.0"
 description = "Next generation coverage analysis"
 authors = ["northwestwitch <chiara.rasi@scilifelab.se>"]
 
 [tool.poetry_bumpversion.file."src/chanjo2/__init__.py"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `chanjo2-1.0.1/src/chanjo2/constants.py` & `chanjo2-1.1.0/src/chanjo2/constants.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.0.1/src/chanjo2/crud/cases.py` & `chanjo2-1.1.0/src/chanjo2/crud/cases.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.0.1/src/chanjo2/crud/intervals.py` & `chanjo2-1.1.0/src/chanjo2/crud/intervals.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.0.1/src/chanjo2/crud/samples.py` & `chanjo2-1.1.0/src/chanjo2/crud/samples.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.0.1/src/chanjo2/dbutil.py` & `chanjo2-1.1.0/src/chanjo2/dbutil.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.0.1/src/chanjo2/demo/panelapp_109_example.d4` & `chanjo2-1.1.0/src/chanjo2/demo/panelapp_109_example.d4`

 * *Files identical despite different names*

### Comparing `chanjo2-1.0.1/src/chanjo2/endpoints/cases.py` & `chanjo2-1.1.0/src/chanjo2/endpoints/cases.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.0.1/src/chanjo2/endpoints/coverage.py` & `chanjo2-1.1.0/src/chanjo2/endpoints/coverage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Optional, Tuple, Union
 
-from fastapi import APIRouter, HTTPException, File, status, Depends
+from fastapi import APIRouter, HTTPException, status, Depends
 from fastapi.responses import JSONResponse
 from pyd4 import D4File
 from sqlmodel import Session
 
 from chanjo2.constants import (
     WRONG_BED_FILE_MSG,
     WRONG_COVERAGE_FILE_MSG,
@@ -17,83 +17,92 @@
 from chanjo2.meta.handle_d4 import (
     intervals_coverage,
     get_intervals_mean_coverage,
     get_d4_file,
     set_interval,
     get_genes_coverage_completeness,
     get_gene_interval_coverage_completeness,
+    get_intervals_completeness,
 )
 from chanjo2.models.pydantic_models import (
     CoverageInterval,
     SampleGeneIntervalQuery,
+    FileCoverageQuery,
+    FileCoverageIntervalsFileQuery,
 )
 from chanjo2.models.sql_models import Exon as SQLExon
 from chanjo2.models.sql_models import Gene as SQLGene
 from chanjo2.models.sql_models import Transcript as SQLTranscript
 
 router = APIRouter()
 
 
-@router.get("/coverage/d4/interval/", response_model=CoverageInterval)
-def d4_interval_coverage(
-    coverage_file_path: str,
-    chromosome: str,
-    start: Optional[int] = None,
-    end: Optional[int] = None,
-):
+@router.post("/coverage/d4/interval/", response_model=CoverageInterval)
+def d4_interval_coverage(query: FileCoverageQuery):
     """Return coverage on the given interval for a D4 resource located on the disk or on a remote server."""
 
     interval: Tuple[str, Optional[int], Optional[int]] = set_interval(
-        chrom=chromosome, start=start, end=end
+        chrom=query.chromosome, start=query.start, end=query.end
     )
     try:
-        d4_file: D4File = get_d4_file(coverage_file_path)
+        d4_file: D4File = get_d4_file(query.coverage_file_path)
     except Exception:
         raise HTTPException(
             status_code=status.HTTP_404_NOT_FOUND,
             detail=WRONG_COVERAGE_FILE_MSG,
         )
 
     return CoverageInterval(
-        chromosome=chromosome,
-        start=start,
-        end=end,
+        chromosome=query.chromosome,
+        start=query.start,
+        end=query.end,
         interval=interval,
         mean_coverage=[
             (
                 "D4File",
                 get_intervals_mean_coverage(d4_file=d4_file, intervals=[interval])[0],
             )
         ],
+        completeness=get_intervals_completeness(
+            d4_file=d4_file,
+            intervals=[interval],
+            completeness_threholds=query.completeness_thresholds,
+        ),
     )
 
 
 @router.post("/coverage/d4/interval_file/", response_model=List[CoverageInterval])
-def d4_intervals_coverage(coverage_file_path: str, bed_file: bytes = File(...)):
+def d4_intervals_coverage(query: FileCoverageIntervalsFileQuery):
     """Return coverage on the given intervals for a D4 resource located on the disk or on a remote server."""
 
     try:
-        d4_file: D4File = get_d4_file(coverage_file_path=coverage_file_path)
+        d4_file: D4File = get_d4_file(coverage_file_path=query.coverage_file_path)
     except Exception:
         raise HTTPException(
             status_code=status.HTTP_404_NOT_FOUND,
             detail=WRONG_COVERAGE_FILE_MSG,
         )
 
     try:
-        intervals: List[Tuple[str, Optional[int], Optional[int]]] = parse_bed(
-            bed_file=bed_file
-        )
+        with open(query.intervals_bed_path, "rb") as bed_file:
+            bed_file_content = bed_file.read()
+            intervals: List[Tuple[str, Optional[int], Optional[int]]] = parse_bed(
+                bed_file_content=bed_file_content
+            )
     except Exception:
         raise HTTPException(
             status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
             detail=WRONG_BED_FILE_MSG,
         )
 
-    return intervals_coverage(d4_file=d4_file, intervals=intervals)
+    return intervals_coverage(
+        d4_file=d4_file,
+        intervals=intervals,
+        completeness_threholds=query.completeness_thresholds,
+    )
 
 
 def get_samples_coverage_file(
     db: Session, samples: Optional[List[str]], case: Optional[str]
 ) -> Union[List[Tuple[str, D4File]], JSONResponse]:
     """Return a list of sample names with relative D4 coverage files."""
```

### Comparing `chanjo2-1.0.1/src/chanjo2/endpoints/intervals.py` & `chanjo2-1.1.0/src/chanjo2/endpoints/intervals.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.0.1/src/chanjo2/endpoints/samples.py` & `chanjo2-1.1.0/src/chanjo2/endpoints/samples.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.0.1/src/chanjo2/main.py` & `chanjo2-1.1.0/src/chanjo2/main.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.0.1/src/chanjo2/meta/handle_bed.py` & `chanjo2-1.1.0/src/chanjo2/meta/handle_bed.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List, Tuple
 
 
-def parse_bed(bed_file: bytes) -> List[Tuple[str, int, int]]:
+def parse_bed(bed_file_content: bytes) -> List[Tuple[str, int, int]]:
     """Parses a bed file containing genomic coordinates."""
     intervals: List[Tuple[str, int, int]] = []
-    for line_byte in bed_file.rsplit(b"\n"):
+    for line_byte in bed_file_content.rsplit(b"\n"):
         if len(line_byte) > 0 and not line_byte.startswith(b"#"):
             intervals.append(bed_line_to_region(bytes_line=line_byte))
     return intervals
 
 
 def bed_line_to_region(bytes_line: bytes) -> Tuple[str, int, int]:
     """Returns a single genomic interval corresponding to a bed file line."""
```

### Comparing `chanjo2-1.0.1/src/chanjo2/meta/handle_d4.py` & `chanjo2-1.1.0/src/chanjo2/meta/handle_d4.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,30 +33,37 @@
         interval_coords.append((interval.chromosome, interval.start, interval.stop))
     return interval_coords
 
 
 def get_intervals_mean_coverage(
     d4_file: D4File, intervals: List[Tuple[str, int, int]]
 ) -> List[float]:
-    """Return the mean value over a list of intervals of a D4 file."""
+    """Return the mean value over a list of intervals of a d4 file."""
     return d4_file.mean(intervals)
 
 
 def intervals_coverage(
-    d4_file: D4File, intervals: List[Tuple[str, int, int]]
+    d4_file: D4File,
+    intervals: List[Tuple[str, int, int]],
+    completeness_threholds: Optional[List[int]],
 ) -> List[CoverageInterval]:
     """Return coverage over a list of intervals."""
     intervals_cov: List[CoverageInterval] = []
     for interval in intervals:
         intervals_cov.append(
             CoverageInterval(
                 chromosome=interval[0],
                 start=interval[1],
                 end=interval[2],
                 mean_coverage={"D4File": d4_file.mean(interval)},
+                completeness=get_intervals_completeness(
+                    d4_file=d4_file,
+                    intervals=[interval],
+                    completeness_threholds=completeness_threholds,
+                ),
             )
         )
     return intervals_cov
 
 
 def get_intervals_completeness(
     d4_file: D4File,
@@ -94,15 +101,14 @@
             (
                 threshold,
                 Decimal(nr_complete_bases_by_threshold[index] / total_region_length)
                 if nr_complete_bases_by_threshold[index]
                 else 0,
             )
         )
-
     return completeness_values
 
 
 def get_genes_coverage_completeness(
     samples_d4_files: List[Tuple[str, D4File]],
     genes: List[SQLGene],
     completeness_threholds: List[Optional[int]],
```

### Comparing `chanjo2-1.0.1/src/chanjo2/meta/handle_load_intervals.py` & `chanjo2-1.1.0/src/chanjo2/meta/handle_load_intervals.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.0.1/src/chanjo2/models/pydantic_models.py` & `chanjo2-1.1.0/src/chanjo2/models/pydantic_models.py`

 * *Files 18% similar despite different names*

```diff
@@ -140,14 +140,30 @@
     hgnc_id: Optional[int]
     hgnc_symbol: Optional[str]
     interval_id: Optional[int]
     mean_coverage: Dict = Field(default_factory=dict)
     start: Optional[int]
 
 
+class FileCoverageBaseQuery(BaseModel):
+    coverage_file_path: str
+
+
+class FileCoverageQuery(FileCoverageBaseQuery):
+    chromosome: str
+    start: Optional[int]
+    end: Optional[int]
+    completeness_thresholds: Optional[List[int]]
+
+
+class FileCoverageIntervalsFileQuery(FileCoverageBaseQuery):
+    intervals_bed_path: str
+    completeness_thresholds: Optional[List[int]]
+
+
 class SampleGeneIntervalQuery(BaseModel):
     build: Builds
     completeness_thresholds: Optional[List[int]]
     ensembl_gene_ids: Optional[List[str]]
     hgnc_gene_ids: Optional[List[int]]
     hgnc_gene_symbols: Optional[List[str]]
     samples: Optional[List[str]]
```

### Comparing `chanjo2-1.0.1/src/chanjo2/models/sql_models.py` & `chanjo2-1.1.0/src/chanjo2/models/sql_models.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.0.1/src/chanjo2/populate_demo.py` & `chanjo2-1.1.0/src/chanjo2/populate_demo.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.0.1/PKG-INFO` & `chanjo2-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chanjo2
-Version: 1.0.1
+Version: 1.1.0
 Summary: Next generation coverage analysis
 Author: northwestwitch
 Author-email: chiara.rasi@scilifelab.se
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

