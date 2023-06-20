# Comparing `tmp/eodc_faas_snap-2023.6.1.tar.gz` & `tmp/eodc_faas_snap-2023.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc_faas_snap-2023.6.1.tar", max compression
+gzip compressed data, was "eodc_faas_snap-2023.6.2.tar", max compression
```

## Comparing `eodc_faas_snap-2023.6.1.tar` & `eodc_faas_snap-2023.6.2.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0       23 2023-06-01 09:43:57.267253 eodc_faas_snap-2023.6.1/README.md
--rw-r--r--   0        0        0      689 2023-06-06 07:18:22.939253 eodc_faas_snap-2023.6.1/pyproject.toml
--rw-r--r--   0        0        0       91 2023-06-06 07:18:22.939253 eodc_faas_snap-2023.6.1/snap_processor_bindings/__init__.py
--rw-r--r--   0        0        0      937 2023-06-05 13:20:29.499253 eodc_faas_snap-2023.6.1/snap_processor_bindings/model.py
--rw-r--r--   0        0        0     4743 2023-06-06 07:18:22.939253 eodc_faas_snap-2023.6.1/snap_processor_bindings/workflows.py
--rw-r--r--   0        0        0      681 1970-01-01 00:00:00.000000 eodc_faas_snap-2023.6.1/PKG-INFO
+-rw-r--r--   0        0        0       23 2023-06-01 09:43:57.267253 eodc_faas_snap-2023.6.2/README.md
+-rw-r--r--   0        0        0      607 2023-06-20 11:27:26.856000 eodc_faas_snap-2023.6.2/pyproject.toml
+-rw-r--r--   0        0        0       91 2023-06-20 11:27:26.860000 eodc_faas_snap-2023.6.2/snap_processor_bindings/__init__.py
+-rw-r--r--   0        0        0     1298 2023-06-20 11:22:14.016000 eodc_faas_snap-2023.6.2/snap_processor_bindings/model.py
+-rw-r--r--   0        0        0      521 1970-01-01 00:00:00.000000 eodc_faas_snap-2023.6.2/PKG-INFO
```

### Comparing `eodc_faas_snap-2023.6.1/pyproject.toml` & `eodc_faas_snap-2023.6.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 [tool.poetry]
 name = "eodc-faas-snap"
-version = "2023.6.1"
+version = "2023.6.2"
 description = "Bindings for the snap processor exposed at EODC"
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>", "Sean Hoyal <sean.hoyal@eodc.eu>", "Valentina Hutter <valentina.hutter@eodc.eu>"]
 readme = "README.md"
 packages = [{include = "snap_processor_bindings"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pydantic = "^1.10.7"
-requests = "^2.28.2"
-pyproj = "^3.5.0"
-argo-workflows = "6.3.9"
-pystac = "^1.7.3"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.2.1"
 pytest = "^7.2.2"
 ruff = "^0.0.259"
 ipykernel = "^6.22.0"
```

### Comparing `eodc_faas_snap-2023.6.1/snap_processor_bindings/model.py` & `eodc_faas_snap-2023.6.2/snap_processor_bindings/model.py`

 * *Files 22% similar despite different names*

```diff
@@ -34,7 +34,23 @@
         default=SnapCorrectionCoefficient.GAMMA0
     )
     correction_method: SnapCorrectionMethod = Field(
         default=SnapCorrectionMethod.TERRAIN
     )
     dem: Optional[DEM] = Field(default=None)
     save_incidence_angle: bool = Field(default=False)
+
+    @property
+    def root_path(self):
+        return self.user_workspace / "SNAP"
+
+    @property
+    def outputs_path(self) -> Path:
+        return self.root_path / "outputs"
+
+    @property
+    def stac_path(self) -> Path:
+        return self.outputs_path / "STAC"
+
+    @property
+    def stac_items_path(self) -> Path:
+        return self.stac_path / "items"
```

### Comparing `eodc_faas_snap-2023.6.1/PKG-INFO` & `eodc_faas_snap-2023.6.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 Metadata-Version: 2.1
 Name: eodc-faas-snap
-Version: 2023.6.1
+Version: 2023.6.2
 Summary: Bindings for the snap processor exposed at EODC
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: argo-workflows (==6.3.9)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
-Requires-Dist: pyproj (>=3.5.0,<4.0.0)
-Requires-Dist: pystac (>=1.7.3,<2.0.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 # snap Python Bindings
```

