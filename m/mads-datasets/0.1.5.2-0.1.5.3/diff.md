# Comparing `tmp/mads_datasets-0.1.5.2.tar.gz` & `tmp/mads_datasets-0.1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mads_datasets-0.1.5.2.tar", max compression
+gzip compressed data, was "mads_datasets-0.1.5.3.tar", max compression
```

## Comparing `mads_datasets-0.1.5.2.tar` & `mads_datasets-0.1.5.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1393 2023-06-07 14:25:34.493117 mads_datasets-0.1.5.2/README.md
--rw-r--r--   0        0        0      188 2023-06-12 07:06:56.170150 mads_datasets-0.1.5.2/mads_datasets/__init__.py
--rw-r--r--   0        0        0    15387 2023-06-06 10:23:56.869646 mads_datasets-0.1.5.2/mads_datasets/datasetfactory.py
--rw-r--r--   0        0        0     5057 2023-06-06 09:56:28.815925 mads_datasets-0.1.5.2/mads_datasets/datasets.py
--rw-r--r--   0        0        0     4778 2023-06-05 10:37:07.673949 mads_datasets-0.1.5.2/mads_datasets/datatools.py
--rw-r--r--   0        0        0     3251 2023-06-06 08:42:57.768632 mads_datasets-0.1.5.2/mads_datasets/settings.py
--rw-r--r--   0        0        0      982 2023-06-12 07:06:51.311671 mads_datasets-0.1.5.2/pyproject.toml
--rw-r--r--   0        0        0     2233 1970-01-01 00:00:00.000000 mads_datasets-0.1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1393 2023-06-07 14:25:34.493117 mads_datasets-0.1.5.3/README.md
+-rw-r--r--   0        0        0      188 2023-06-20 09:12:10.155928 mads_datasets-0.1.5.3/mads_datasets/__init__.py
+-rw-r--r--   0        0        0    15781 2023-06-20 09:11:17.134168 mads_datasets-0.1.5.3/mads_datasets/datasetfactory.py
+-rw-r--r--   0        0        0     5057 2023-06-06 09:56:28.815925 mads_datasets-0.1.5.3/mads_datasets/datasets.py
+-rw-r--r--   0        0        0     4778 2023-06-05 10:37:07.673949 mads_datasets-0.1.5.3/mads_datasets/datatools.py
+-rw-r--r--   0        0        0     3534 2023-06-20 09:06:01.252755 mads_datasets-0.1.5.3/mads_datasets/settings.py
+-rw-r--r--   0        0        0      982 2023-06-20 09:12:03.389393 mads_datasets-0.1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     2233 1970-01-01 00:00:00.000000 mads_datasets-0.1.5.3/PKG-INFO
```

### Comparing `mads_datasets-0.1.5.2/README.md` & `mads_datasets-0.1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.1.5.2/mads_datasets/datasetfactory.py` & `mads_datasets-0.1.5.3/mads_datasets/datasetfactory.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     TextDatasetSettings,
     WindowedDatasetSettings,
     fashionmnistsettings,
     flowersdatasetsettings,
     gesturesdatasetsettings,
     imdbdatasetsettings,
     sunspotsettings,
+    irissettings
 )
 
 Tensor = torch.Tensor
 
 
 class DatastreamerProtocol(Protocol):
     def stream(self) -> Iterator:
@@ -92,14 +93,15 @@
             self.filepath = self.subfolder / filename
 
         digest = self.calculate_md5(self.filepath)
         if self.settings.digest is not None:
             if digest != self.settings.digest:
                 raise ValueError(
                     f"Digest of downloaded file {self.filepath} does not match expected digest"
+                    f"\nExpected: {self.settings.digest}\nGot: {digest}"
                 )
             else:
                 logger.info(
                     f"Digest of downloaded {self.filepath} matches expected digest"
                 )
         else:
             logger.info(f"Digest of downloaded {self.filepath} is {digest}")
@@ -131,14 +133,18 @@
             traindataset, batchsize=batchsize, preprocessor=preprocessor
         )
         validstreamer = BaseDatastreamer(
             validdataset, batchsize=batchsize, preprocessor=preprocessor
         )
         return {"train": trainstreamer, "valid": validstreamer}
 
+class IrisDatasetFactory(AbstractDatasetFactory[DatasetSettings]):
+    def create_dataset(self, *args: Any, **kwargs: Any) -> Mapping[str, DatasetProtocol]:
+        pass
+
 
 class SunspotsDatasetFactory(AbstractDatasetFactory[WindowedDatasetSettings]):
     """
     Data from https://www.sidc.be/SILSO/datafiles
     """
 
     def create_dataset(
@@ -407,14 +413,16 @@
                 fashionmnistsettings, preprocessor=preprocessor, datadir=datadir
             )
         if dataset_type == DatasetType.SUNSPOTS:
             preprocessor = kwargs.get("preprocessor", BasePreprocessor)
             return SunspotsDatasetFactory(
                 sunspotsettings, preprocessor=preprocessor, datadir=datadir
             )
+        if dataset_type == DatasetType.IRIS:
+            return IrisDatasetFactory(irissettings, preprocessor=None, datadir=datadir)
 
         raise ValueError(f"Invalid dataset type: {dataset_type}")
 
 
 class BaseDatastreamer:
     """This datastreamer wil never stop
     The dataset should have a:
```

### Comparing `mads_datasets-0.1.5.2/mads_datasets/datasets.py` & `mads_datasets-0.1.5.3/mads_datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.1.5.2/mads_datasets/datatools.py` & `mads_datasets-0.1.5.3/mads_datasets/datatools.py`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.1.5.2/mads_datasets/settings.py` & `mads_datasets-0.1.5.3/mads_datasets/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     PNG = ".png"
     TXT = ".txt"
     ZIP = ".zip"
     TGZ = ".tgz"
     TAR = ".tar.gz"
     GZ = ".gz"
     PT = ".pt"
+    CSV = ".csv"
 
 
 class ReportTypes(Enum):
     GIN = 1
     TENSORBOARD = 2
     MLFLOW = 3
     RAY = 4
@@ -27,14 +28,15 @@
 
 class DatasetType(Enum):
     FLOWERS = 1
     IMDB = 2
     GESTURES = 3
     FASHION = 4
     SUNSPOTS = 5
+    IRIS = 6
 
 
 class BaseSettings(BaseModel):
     def __str__(self) -> str:
         return "\n".join(f"{k}: {v}" for k, v in self.__dict__.items())
 
     def __repr__(self) -> str:
@@ -60,14 +62,21 @@
     clean_fn: Callable
 
 
 class WindowedDatasetSettings(DatasetSettings):
     horizon: int
     window_size: int
 
+irissettings = DatasetSettings(
+    dataset_url=cast(HttpUrl, "https://github.com/raoulg/data_assets/raw/main/iris_dirty.csv"),
+    filename=Path("iris.csv"),
+    name="iris",
+    formats=[FileTypes.CSV],
+    digest="3679279dc61f6fdd859be9888db27f75"
+)
 
 sunspotsettings = WindowedDatasetSettings(
     dataset_url=cast(HttpUrl, "https://www.sidc.be/SILSO/DATA/SN_m_tot_V2.0.txt"),
     filename=Path("sunspots.txt"),
     name="sunspots",
     formats=[],
     horizon=3,
```

### Comparing `mads_datasets-0.1.5.2/pyproject.toml` & `mads_datasets-0.1.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mads-datasets"
-version = "0.1.5.2"
+version = "0.1.5.3"
 description = "Datasets for the master applied data science"
 authors = ["Raoul Grouls <Raoul.Grouls@han.nl>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "mads_datasets"}]
 
 [tool.poetry.urls]
```

### Comparing `mads_datasets-0.1.5.2/PKG-INFO` & `mads_datasets-0.1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mads-datasets
-Version: 0.1.5.2
+Version: 0.1.5.3
 Summary: Datasets for the master applied data science
 License: MIT
 Author: Raoul Grouls
 Author-email: Raoul.Grouls@han.nl
 Requires-Python: >=3.9.16,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

