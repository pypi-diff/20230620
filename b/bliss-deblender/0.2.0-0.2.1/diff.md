# Comparing `tmp/bliss_deblender-0.2.0.tar.gz` & `tmp/bliss_deblender-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bliss_deblender-0.2.0.tar", max compression
+gzip compressed data, was "bliss_deblender-0.2.1.tar", max compression
```

## Comparing `bliss_deblender-0.2.0.tar` & `bliss_deblender-0.2.1.tar`

### file list

```diff
@@ -1,39 +1,29 @@
--rw-r--r--   0        0        0     1102 2023-05-23 14:00:53.255529 bliss_deblender-0.2.0/LICENSE.md
--rw-r--r--   0        0        0     3815 2023-06-02 15:18:56.594384 bliss_deblender-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-05-23 14:00:53.255529 bliss_deblender-0.2.0/bliss/__init__.py
--rw-r--r--   0        0        0    15704 2023-06-12 20:09:58.928512 bliss_deblender-0.2.0/bliss/api.py
--rw-r--r--   0        0        0    15923 2023-06-05 14:45:24.369403 bliss_deblender-0.2.0/bliss/catalog.py
--rw-r--r--   0        0        0        0 2023-06-02 16:09:58.388337 bliss_deblender-0.2.0/bliss/conf/__init__.py
--rw-r--r--   0        0        0      152 2023-06-02 16:12:28.618668 bliss_deblender-0.2.0/bliss/conf/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      608 2023-06-02 16:13:56.845685 bliss_deblender-0.2.0/bliss/conf/__pycache__/igs.cpython-310.pyc
--rw-r--r--   0        0        0     5089 2023-06-06 20:45:09.947707 bliss_deblender-0.2.0/bliss/conf/base_config.yaml
--rw-r--r--   0        0        0      377 2023-06-02 16:13:22.930063 bliss_deblender-0.2.0/bliss/conf/igs.py
--rw-r--r--   0        0        0    11953 2023-06-12 19:30:00.443780 bliss_deblender-0.2.0/bliss/encoder.py
--rw-r--r--   0        0        0     3855 2023-06-02 15:18:56.598384 bliss_deblender-0.2.0/bliss/generate.py
--rw-r--r--   0        0        0     8343 2023-05-23 14:00:53.259529 bliss_deblender-0.2.0/bliss/metrics.py
--rw-r--r--   0        0        0     6499 2023-05-23 14:00:53.259529 bliss_deblender-0.2.0/bliss/plotting.py
--rw-r--r--   0        0        0     6737 2023-06-12 14:19:07.851845 bliss_deblender-0.2.0/bliss/predict.py
--rw-r--r--   0        0        0        0 2023-05-23 14:00:53.263529 bliss_deblender-0.2.0/bliss/simulator/__init__.py
--rw-r--r--   0        0        0      157 2023-05-23 19:50:39.942679 bliss_deblender-0.2.0/bliss/simulator/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2968 2023-06-02 16:10:03.460281 bliss_deblender-0.2.0/bliss/simulator/__pycache__/background.cpython-310.pyc
--rw-r--r--   0        0        0     7086 2023-06-02 16:15:19.560760 bliss_deblender-0.2.0/bliss/simulator/__pycache__/decoder.cpython-310.pyc
--rw-r--r--   0        0        0     8499 2023-06-02 16:08:20.485420 bliss_deblender-0.2.0/bliss/simulator/__pycache__/prior.cpython-310.pyc
--rw-r--r--   0        0        0     8128 2023-06-02 16:15:19.556760 bliss_deblender-0.2.0/bliss/simulator/__pycache__/simulated_dataset.cpython-310.pyc
--rw-r--r--   0        0        0     2698 2023-06-02 15:18:56.598384 bliss_deblender-0.2.0/bliss/simulator/background.py
--rw-r--r--   0        0        0     8978 2023-06-02 15:18:56.598384 bliss_deblender-0.2.0/bliss/simulator/decoder.py
--rw-r--r--   0        0        0    11764 2023-06-02 15:18:56.598384 bliss_deblender-0.2.0/bliss/simulator/prior.py
--rw-r--r--   0        0        0     8472 2023-06-02 15:18:56.602384 bliss_deblender-0.2.0/bliss/simulator/simulated_dataset.py
--rw-r--r--   0        0        0        0 2023-05-23 14:00:53.263529 bliss_deblender-0.2.0/bliss/surveys/__init__.py
--rw-r--r--   0        0        0      155 2023-05-23 19:50:39.950679 bliss_deblender-0.2.0/bliss/surveys/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4185 2023-05-25 16:12:09.290263 bliss_deblender-0.2.0/bliss/surveys/__pycache__/decals.cpython-310.pyc
--rw-r--r--   0        0        0     6648 2023-06-07 14:59:25.957594 bliss_deblender-0.2.0/bliss/surveys/__pycache__/sdss.cpython-310.pyc
--rw-r--r--   0        0        0     2176 2023-06-08 19:15:21.049829 bliss_deblender-0.2.0/bliss/surveys/__pycache__/sdss_download.cpython-310.pyc
--rw-r--r--   0        0        0     4644 2023-05-23 14:00:53.263529 bliss_deblender-0.2.0/bliss/surveys/decals.py
--rw-r--r--   0        0        0        0 2023-05-23 14:00:53.263529 bliss_deblender-0.2.0/bliss/surveys/hst.py
--rw-r--r--   0        0        0        0 2023-05-23 14:00:53.263529 bliss_deblender-0.2.0/bliss/surveys/lsst.py
--rw-r--r--   0        0        0     7730 2023-06-07 14:59:23.705618 bliss_deblender-0.2.0/bliss/surveys/sdss.py
--rw-r--r--   0        0        0     2482 2023-06-08 19:14:31.130458 bliss_deblender-0.2.0/bliss/surveys/sdss_download.py
--rwxr-xr-x   0        0        0     5278 2023-05-23 14:00:53.263529 bliss_deblender-0.2.0/bliss/train.py
--rw-r--r--   0        0        0     1820 2023-05-23 14:00:53.263529 bliss_deblender-0.2.0/bliss/unconstrained_dists.py
--rw-r--r--   0        0        0     2263 2023-06-12 19:51:19.733301 bliss_deblender-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5096 1970-01-01 00:00:00.000000 bliss_deblender-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-05-23 14:00:53.255529 bliss_deblender-0.2.1/LICENSE.md
+-rw-r--r--   0        0        0     3815 2023-06-02 15:18:56.594384 bliss_deblender-0.2.1/README.md
+-rw-r--r--   0        0        0      290 2023-06-20 14:05:43.894343 bliss_deblender-0.2.1/bliss/__init__.py
+-rw-r--r--   0        0        0    11825 2023-06-20 16:45:22.790472 bliss_deblender-0.2.1/bliss/api.py
+-rw-r--r--   0        0        0    18267 2023-06-20 14:05:43.898343 bliss_deblender-0.2.1/bliss/catalog.py
+-rw-r--r--   0        0        0        0 2023-06-12 21:26:33.956574 bliss_deblender-0.2.1/bliss/conf/__init__.py
+-rw-r--r--   0        0        0     5578 2023-06-20 14:19:50.520029 bliss_deblender-0.2.1/bliss/conf/base_config.yaml
+-rw-r--r--   0        0        0      377 2023-06-12 21:26:33.960574 bliss_deblender-0.2.1/bliss/conf/igs.py
+-rw-r--r--   0        0        0    14847 2023-06-20 14:05:45.342326 bliss_deblender-0.2.1/bliss/encoder.py
+-rw-r--r--   0        0        0     4110 2023-06-20 14:05:43.898343 bliss_deblender-0.2.1/bliss/generate.py
+-rw-r--r--   0        0        0    13466 2023-06-19 13:31:58.161962 bliss_deblender-0.2.1/bliss/metrics.py
+-rw-r--r--   0        0        0     2167 2023-06-19 13:31:58.161962 bliss_deblender-0.2.1/bliss/plotting.py
+-rw-r--r--   0        0        0     5513 2023-06-20 14:05:45.342326 bliss_deblender-0.2.1/bliss/predict.py
+-rw-r--r--   0        0        0        0 2023-05-23 14:00:53.263529 bliss_deblender-0.2.1/bliss/simulator/__init__.py
+-rw-r--r--   0        0        0     2698 2023-06-02 15:18:56.598384 bliss_deblender-0.2.1/bliss/simulator/background.py
+-rw-r--r--   0        0        0    10678 2023-06-20 16:45:22.794472 bliss_deblender-0.2.1/bliss/simulator/decoder.py
+-rw-r--r--   0        0        0    11895 2023-06-20 16:45:22.794472 bliss_deblender-0.2.1/bliss/simulator/prior.py
+-rw-r--r--   0        0        0    10378 2023-06-20 14:05:43.902343 bliss_deblender-0.2.1/bliss/simulator/simulated_dataset.py
+-rw-r--r--   0        0        0        0 2023-05-23 14:00:53.263529 bliss_deblender-0.2.1/bliss/surveys/__init__.py
+-rw-r--r--   0        0        0     5406 2023-06-20 16:45:22.794472 bliss_deblender-0.2.1/bliss/surveys/decals.py
+-rw-r--r--   0        0        0        0 2023-05-23 14:00:53.263529 bliss_deblender-0.2.1/bliss/surveys/hst.py
+-rw-r--r--   0        0        0        0 2023-05-23 14:00:53.263529 bliss_deblender-0.2.1/bliss/surveys/lsst.py
+-rw-r--r--   0        0        0    14266 2023-06-20 16:45:22.794472 bliss_deblender-0.2.1/bliss/surveys/sdss.py
+-rwxr-xr-x   0        0        0     5343 2023-06-20 14:05:44.818332 bliss_deblender-0.2.1/bliss/train.py
+-rw-r--r--   0        0        0     1820 2023-05-23 14:00:53.263529 bliss_deblender-0.2.1/bliss/unconstrained_dists.py
+-rw-r--r--   0        0        0        0 2023-06-20 14:05:45.102329 bliss_deblender-0.2.1/bliss/utils/__init__.py
+-rw-r--r--   0        0        0     1652 2023-06-20 16:45:37.842287 bliss_deblender-0.2.1/bliss/utils/download_utils.py
+-rw-r--r--   0        0        0     2411 2023-06-20 14:05:45.102329 bliss_deblender-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5018 1970-01-01 00:00:00.000000 bliss_deblender-0.2.1/PKG-INFO
```

### Comparing `bliss_deblender-0.2.0/LICENSE.md` & `bliss_deblender-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bliss_deblender-0.2.0/README.md` & `bliss_deblender-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `bliss_deblender-0.2.0/bliss/api.py` & `bliss_deblender-0.2.1/bliss/api.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,95 +1,88 @@
-import base64
 from pathlib import Path
-from typing import Dict, Literal, Optional, Tuple
+from typing import Dict, Literal, Optional, Tuple, TypeAlias
 
-import requests
 import torch
-from astropy import units as u
+from astropy import units as u  # noqa: WPS347
 from astropy.table import Table
 from einops import rearrange
 from omegaconf import OmegaConf
 from torch import Tensor
 
 from bliss.catalog import FullCatalog
 from bliss.conf.igs import base_config
 from bliss.generate import generate as _generate
 from bliss.predict import predict_sdss as _predict_sdss
-from bliss.surveys import sdss_download
+from bliss.surveys.sdss import SDSSDownloader
 from bliss.train import train as _train
+from bliss.utils.download_utils import download_git_lfs_file
 
-SurveyType = Literal["decals", "hst", "lsst", "sdss"]
+SurveyType: TypeAlias = Literal["decals", "hst", "lsst", "sdss"]
 
 
 class BlissClient:
     """Client for interacting with the BLISS API."""
 
     def __init__(self, cwd: str):
         self._cwd = cwd
-        # cached_data_path (str): Path to directory where cached data will be stored.
-        self._cached_data_path = self.cwd + "/dataset"
-        Path(self.cached_data_path).mkdir(parents=True, exist_ok=True)
-        # pretrained_weights_path (str): Path to directory to store pretrained weights.
-        self._pretrained_weights_path = self.cwd + "/pretrained_weights"
-        Path(self.pretrained_weights_path).mkdir(parents=True, exist_ok=True)
-        # output_path (str): Path to directory to store trained model weights.
-        self._output_path = self.cwd + "/output"
-        Path(self.output_path).mkdir(parents=True, exist_ok=True)
+        self.base_cfg = base_config()
+        self.base_cfg.paths.root = self.cwd
 
     def generate(
         self,
         n_batches: int,
         batch_size: int,
         max_images_per_file: int,
         **kwargs,
     ) -> None:
         """Generate and cache simulated images to disk.
 
         Args:
             n_batches (int): Number of batches to simulate.
             batch_size (int): Number of images per batch.
             max_images_per_file (int): Number of images per cached file.
-            kwargs: Keyword arguments to override default configuration values.
-        """  # noqa: RST210
-        cfg = base_config()
+            **kwargs: Keyword arguments to override default configuration values.
+        """
+        cfg = OmegaConf.create(self.base_cfg)
         # apply overrides
         cfg.generate.n_batches = n_batches
         cfg.generate.batch_size = batch_size
         cfg.generate.max_images_per_file = max_images_per_file
-        cfg.generate.cached_data_path = self.cached_data_path
+
         for k, v in kwargs.items():
             OmegaConf.update(cfg, k, v)
 
         _generate(cfg)
 
     def load_pretrained_weights_for_survey(self, survey: SurveyType, filename: str) -> None:
         """Load pretrained weights for a survey.
 
         Args:
             survey (SurveyType): Survey to load pretrained weights for.
-            filename (str): Name of pretrained weights file to load.
+            filename (str): Name of pretrained weights file downloaded.
         """
-        weights = _download_git_lfs_file(
+        weights = download_git_lfs_file(
             "https://api.github.com/repos/prob-ml/bliss/contents/"
             f"data/pretrained_models/{survey}.pt"
         )
-        with open(self.pretrained_weights_path + f"/{filename}", "wb+") as f:
+        Path(self.base_cfg.paths.pretrained_models).mkdir(parents=True, exist_ok=True)
+        with open(self.base_cfg.paths.pretrained_models + f"/{filename}", "wb+") as f:
             f.write(weights)
 
     def train(self, weight_save_path, **kwargs) -> None:
         """Train model on simulated images.
 
         Args:
             weight_save_path (str): Path to directory after cwd where trained model
                 weights will be stored.
-            kwargs: Keyword arguments to override default configuration values.
-        """  # noqa: RST210
-        cfg = base_config()
+            **kwargs: Keyword arguments to override default configuration values.
+        """
+        cfg = OmegaConf.create(self.base_cfg)
         # apply overrides
-        cfg.training.weight_save_path = self.output_path + f"/{weight_save_path}"
+        cfg.training.weight_save_path = cfg.paths.output + f"/{weight_save_path}"
         for k, v in kwargs.items():
             OmegaConf.update(cfg, k, v)
 
         _train(cfg)
 
     def train_on_cached_data(
         self,
@@ -105,93 +98,69 @@
         Args:
             weight_save_path (str): Path to directory after cwd where trained model
                 weights will be stored.
             train_n_batches (int): Number of batches to train on.
             batch_size (int): Number of images per batch.
             val_split_file_idxs (List[int]): List of file indices to use for validation.
             pretrained_weights_filename (str): Name of pretrained weights file to load.
-            kwargs: Keyword arguments to override default configuration values.
-        """  # noqa: RST210
-        cfg = base_config()
+            **kwargs: Keyword arguments to override default configuration values.
+        """
+        cfg = OmegaConf.create(self.base_cfg)
         cfg.training.use_cached_simulator = True
         # apply overrides
-        cfg.training.weight_save_path = self.output_path + f"/{weight_save_path}"
-        cfg.cached_simulator.cached_data_path = self.cached_data_path
+        cfg.training.weight_save_path = cfg.paths.output + f"/{weight_save_path}"
         cfg.cached_simulator.train_n_batches = train_n_batches
         cfg.cached_simulator.batch_size = batch_size
         cfg.cached_simulator.val_split_file_idxs = val_split_file_idxs
         if pretrained_weights_filename is not None:
             cfg.training.pretrained_weights = (
-                self.pretrained_weights_path + f"/{pretrained_weights_filename}"
+                cfg.paths.pretrained_models + f"/{pretrained_weights_filename}"
             )
         for k, v in kwargs.items():
             OmegaConf.update(cfg, k, v)
 
         _train(cfg)
 
     def load_survey(self, survey: SurveyType, run, camcol, field, download_dir: str):
-        sdss_download.download_all(run, camcol, field, self.cwd + f"/{download_dir}")
+        SDSSDownloader(run, camcol, field, self.cwd + f"/{download_dir}").download_all()
         # assert files downloaded at download_dir
 
     def predict_sdss(
         self,
-        data_path: str,
         weight_save_path: str,
         **kwargs,
     ) -> Tuple[FullCatalog, Table, Table, Table]:
         """Predict on SDSS images.
 
         Args:
-            data_path (str): Path to directory after cwd where SDSS images are stored.
             weight_save_path (str): Path to directory after cwd where trained model
                 weights are stored.
-            kwargs: Keyword arguments to override default configuration values.
+            **kwargs: Keyword arguments to override default configuration values.
 
         Returns:
             Tuple[FullCatalog, Table, Table]: Tuple of predicted catalog, astropy.table
             of predicted catalog, and astropy.table of predicted galaxy_params.
         """
-        cfg = base_config()
+        cfg = OmegaConf.create(self.base_cfg)
         # apply overrides
-        cfg.predict.dataset.sdss_dir = self.cwd + f"/{data_path}"
-        cfg.predict.weight_save_path = self.output_path + f"/{weight_save_path}"
-        cfg.paths.sdss = cfg.predict.dataset.sdss_dir
+        cfg.predict.weight_save_path = cfg.paths.output + f"/{weight_save_path}"
         for k, v in kwargs.items():
             OmegaConf.update(cfg, k, v)
 
-        # download survey images if not already downloaded
-        run, camcol, field = (
-            cfg.predict.dataset.run,
-            cfg.predict.dataset.camcol,
-            cfg.predict.dataset.fields[0],
-        )
-        bands = ["u", "g", "r", "i", "z"]
-        for band in bands:
-            sdss_data_file_path = (
-                Path(cfg.predict.dataset.sdss_dir)
-                / f"{run}"
-                / f"{camcol}"
-                / f"{field}"
-                / f"frame-{band}-{'{:06d}'.format(run)}-{camcol}-{'{:04d}'.format(field)}.fits"
-            )
-            if not sdss_data_file_path.exists():
-                self.load_survey("sdss", run, camcol, field, download_dir=data_path)
-                break
-
         est_cat, _, _, _, pred = _predict_sdss(cfg)
         est_cat_table, galaxy_params_table = fullcat_to_astropy_table(est_cat)
         pred_table = pred_to_astropy_table(pred)
         return est_cat, est_cat_table, galaxy_params_table, pred_table
 
     def plot_predictions_in_notebook(self):
         """Plot predictions in notebook."""
         from IPython.core.display import HTML  # pylint: disable=import-outside-toplevel
         from IPython.display import display  # pylint: disable=import-outside-toplevel
 
-        with open("./predict.html", "r", encoding="utf-8") as f:
+        with open(self.base_cfg.predict.plot.out_file_name, "r", encoding="utf-8") as f:
             html_str = f.read()
             display(HTML(html_str))
 
     def get_dataset_file(self, filename: str):
         with open(self.cached_data_path + "/" + filename, "rb") as f:
             return torch.load(f)
 
@@ -217,111 +186,24 @@
     @property
     def cached_data_path(self) -> str:
         """Get path to cached data.
 
         Returns:
             str: Path to cached data.
         """
-        return self._cached_data_path
+        return self.base_cfg.generate.cached_data_path
 
     @cached_data_path.setter
     def cached_data_path(self, cached_data_path: str) -> None:
         """Set path to cached data.
 
         Args:
             cached_data_path (str): Path to cached data.
         """
-        self._cached_data_path = cached_data_path
-
-    @property
-    def pretrained_weights_path(self) -> str:
-        """Get path to directory containing pretrained weights.
-
-        Returns:
-            str: Path to directory containing pretrained weights.
-        """
-        return self._pretrained_weights_path
-
-    @pretrained_weights_path.setter
-    def pretrained_weights_path(self, pretrained_weights_path: str) -> None:
-        """Set path to pretrained weights.
-
-        Args:
-            pretrained_weights_path (str): Path to pretrained weights.
-        """
-        self._pretrained_weights_path = pretrained_weights_path
-
-    @property
-    def output_path(self) -> str:
-        """Get path to output.
-
-        Returns:
-            str: Path to output.
-        """
-        return self._output_path
-
-    @output_path.setter
-    def output_path(self, output_path: str) -> None:
-        """Set path to output.
-
-        Args:
-            output_path (str): Path to output.
-        """
-        self._output_path = output_path
-
-
-def _download_git_lfs_file(url) -> bytes:
-    """Download a file from git-lfs.
-
-    Args:
-        url (str): URL to git-lfs file.
-
-    Returns:
-        bytes: File contents.
-    """
-    ptr_file = requests.get(url, timeout=10)
-    ptr = ptr_file.json()
-    ptr_sha = ptr["sha"]
-
-    blob_file = requests.get(
-        f"https://api.github.com/repos/prob-ml/bliss/git/blobs/{ptr_sha}", timeout=10
-    )
-    blob = blob_file.json()
-    blob_content = blob["content"]
-    assert blob["encoding"] == "base64"
-
-    blob_decoded = base64.b64decode(blob_content).decode("utf-8").split("\n")
-    sha = blob_decoded[1].split(" ")[1].split(":")[1]
-    size = int(blob_decoded[2].split(" ")[1])
-
-    lfs_ptr_file = requests.post(
-        "https://github.com/prob-ml/bliss.git/info/lfs/objects/batch",
-        headers={
-            "Accept": "application/vnd.git-lfs+json",
-            # Already added when you pass json=
-            # 'Content-type': 'application/json',
-        },
-        json={
-            "operation": "download",
-            "transfer": ["basic"],
-            "objects": [
-                {
-                    "oid": sha,
-                    "size": size,
-                }
-            ],
-        },
-        timeout=10,
-    )
-    lfs_ptr = lfs_ptr_file.json()
-    lfs_ptr_download_url = lfs_ptr["objects"][0]["actions"]["download"]["href"]  # noqa: WPS219
-
-    # Get and write weights to pretrained weights path
-    file = requests.get(lfs_ptr_download_url, timeout=10)
-    return file.content
+        self.base_cfg.generate.cached_data_path = cached_data_path
 
 
 def fullcat_to_astropy_table(est_cat: FullCatalog):
     assert list(est_cat.keys()) == [
         "star_log_fluxes",
         "star_fluxes",
         "galaxy_bools",
```

### Comparing `bliss_deblender-0.2.0/bliss/catalog.py` & `bliss_deblender-0.2.1/bliss/catalog.py`

 * *Files 12% similar despite different names*

```diff
@@ -99,41 +99,39 @@
 
         Returns:
             The FullCatalog instance corresponding to the TileCatalog instance.
 
             NOTE: The locations (`"locs"`) are between 0 and 1. The output also contains
             pixel locations ("plocs") that are between 0 and `slen`.
         """
-        plocs = self._get_full_locs_from_tiles()
+        plocs = self.get_full_locs_from_tiles()
         param_names_to_mask = {"plocs"}.union(set(self.keys()))
         tile_params_to_gather = {"plocs": plocs}
         tile_params_to_gather.update(self)
 
         params = {}
-        indices_to_retrieve, is_on_array = self._get_indices_of_on_sources()
+        indices_to_retrieve, is_on_array = self.get_indices_of_on_sources()
         for param_name, tile_param in tile_params_to_gather.items():
             k = tile_param.shape[-1]
             param = rearrange(tile_param, "b nth ntw s k -> b (nth ntw s) k", k=k)
             indices_for_param = repeat(indices_to_retrieve, "b nth_ntw_s -> b nth_ntw_s k", k=k)
             param = torch.gather(param, dim=1, index=indices_for_param)
             if param_name in param_names_to_mask:
                 param = param * is_on_array.unsqueeze(-1)
             params[param_name] = param
 
         params["n_sources"] = reduce(self.n_sources, "b nth ntw -> b", "sum")
         height, width = self.n_tiles_h * self.tile_slen, self.n_tiles_w * self.tile_slen
         return FullCatalog(height, width, params)
 
-    def _get_full_locs_from_tiles(self) -> Tensor:
+    def get_full_locs_from_tiles(self) -> Tensor:
         """Get the full image locations from tile locations.
 
         Returns:
-            A tuple of two elements, "plocs" and "locs".
-            "plocs" are the pixel coordinates of each source (between 0 and slen).
-            "locs" are the scaled locations of each source (between 0 and 1).
+            Tensor: pixel coordinates of each source (between 0 and slen).
         """
         slen = self.n_tiles_h * self.tile_slen
         wlen = self.n_tiles_w * self.tile_slen
         # coordinates on tiles.
         x_coords = torch.arange(0, slen, self.tile_slen, device=self.locs.device).long()
         y_coords = torch.arange(0, wlen, self.tile_slen, device=self.locs.device).long()
         tile_coords = torch.cartesian_prod(x_coords, y_coords)
@@ -147,15 +145,15 @@
             plocs,
             "(b nth ntw) d xy -> b nth ntw d xy",
             b=self.batch_size,
             nth=self.n_tiles_h,
             ntw=self.n_tiles_w,
         )
 
-    def _get_indices_of_on_sources(self) -> Tuple[Tensor, Tensor]:
+    def get_indices_of_on_sources(self) -> Tuple[Tensor, Tensor]:
         """Get the indices of detected sources from each tile.
 
         Returns:
             A 2-D tensor of integers with shape `n_samples x max(n_sources)`,
             where `max(n_sources)` is the maximum number of sources detected across all samples.
 
             Each element of this tensor is an index of a particular source within a particular tile.
@@ -179,35 +177,93 @@
         out = {}
         out["locs"] = self.locs
         out["n_sources"] = self.n_sources
         for k, v in self.items():
             out[k] = v
         return out
 
-    def get_tile_params_at_coord(self, plocs: torch.Tensor) -> Dict[str, Tensor]:
-        """Return the parameters of the tiles that contain each of the locations in plocs."""
-        assert len(plocs.shape) == 2 and plocs.shape[1] == 2
-        assert plocs.device == self.locs.device
-        n_total = len(plocs)
-        slen = self.n_tiles_h * self.tile_slen
-        wlen = self.n_tiles_w * self.tile_slen
-        # coordinates on tiles.
-        x_coords = torch.arange(0, slen, self.tile_slen, device=self.locs.device).long()
-        y_coords = torch.arange(0, wlen, self.tile_slen, device=self.locs.device).long()
+    def gather_param_at_tiles(self, param_name: str, indices: Tensor) -> Tensor:
+        """Gets the tile parameters at the desired indices.
+
+        Args:
+            param_name (str): Param name. Must be either "locs" or in keys of catalog.
+            indices (Tensor): The indices to gather. Normally this will come from
+                get_indices_of_on_sources, but notably, we use the indices of the true catalog to
+                gather from the tile catalog when computing metrics.
+
+        Returns:
+            Tensor: (b, n, k) tensor, where b=batch size, n=length of indices, and k=param dims
+        """
+        assert param_name == "locs" or param_name in self.keys(), f"'{param_name}' not in catalog"
+        param = self.get_full_locs_from_tiles() if param_name == "locs" else self[param_name]
+        param = rearrange(param, "b h w s k -> b (h w s) k")
+        idx_to_gather = repeat(indices, "... -> ... k", k=param.size(-1))
+        return torch.gather(param, dim=1, index=idx_to_gather)
+
+    def _get_fluxes_of_on_sources(self):
+        """Gets fluxes of "on" sources based on whether the source is a star or galaxy.
 
-        x_indx = torch.searchsorted(x_coords.contiguous(), plocs[:, 0].contiguous()) - 1
-        y_indx = torch.searchsorted(y_coords.contiguous(), plocs[:, 1].contiguous()) - 1
+        Returns:
+            Tensor: a tensor of fluxes of size (b x nth x ntw x max_sources x 1)
+        """
+        fluxes = torch.where(
+            self["galaxy_bools"], self["galaxy_params"][..., 0, None], self["star_fluxes"]
+        )
+        return torch.where(self.is_on_array[..., None], fluxes, torch.zeros_like(fluxes))
+
+    def get_brightest_source_per_tile(self):
+        """Restrict TileCatalog to only the brightest 'on' source per tile.
+
+        Returns:
+            TileCatalog: a new catalog with only one source per tile
+        """
+        if self.max_sources == 1:
+            return self
+
+        # sort by fluxes of "on" sources to get brightest source per tile
+        on_fluxes = self._get_fluxes_of_on_sources()
+        top_idx = on_fluxes.argsort(dim=3, descending=True)[
+            :, :, :, 0:1, 0
+        ]  # 0:1 keeps dims right for slicing
+
+        d = {}
+        for key, val in self.to_dict().items():
+            if key == "n_sources":
+                d[key] = self.n_sources.bool().int()  # send all positive values to 1, 0 to 0
+            else:
+                param_dim = val.size(-1)
+                idx_to_gather = repeat(top_idx, "... -> ... k", k=param_dim)
+                d[key] = torch.take_along_dim(val, idx_to_gather, dim=3)
+
+        return TileCatalog(self.tile_slen, d)
+
+    def filter_tile_catalog_by_flux(self, min_flux=0, max_flux=torch.inf):
+        """Restricts TileCatalog to sources that have a flux between min_flux and max_flux.
+
+        Args:
+            min_flux (float): Minimum flux value to keep. Defaults to 622.
+            max_flux (float): Maximum flux value to keep. Defaults to 1e6.
 
-        # gather in dictionary
-        d = {k: v[:, x_indx, y_indx, :, :].reshape(n_total, -1) for k, v in self.items()}
+        Returns:
+            TileCatalog: a new catalog with only sources within the flux range. Note that the size
+                of the tensors stays the same, but params at sources outside the range are set to 0.
+        """
 
-        # also include locs
-        d["locs"] = self.locs[:, x_indx, y_indx, :, :].reshape(n_total, -1)
+        # get fluxes of "on" sources to mask by
+        on_fluxes = self._get_fluxes_of_on_sources()
+        flux_mask = (on_fluxes > min_flux) & (on_fluxes < max_flux)
+
+        d = {}
+        for key, val in self.to_dict().items():
+            if key == "n_sources":
+                d[key] = flux_mask.sum(dim=3).squeeze()  # number of sources within range in tile
+            else:
+                d[key] = torch.where(flux_mask, val, torch.zeros_like(val))
 
-        return d
+        return TileCatalog(self.tile_slen, d)
 
 
 class FullCatalog(UserDict):
     allowed_params = TileCatalog.allowed_params
 
     def __init__(self, height: int, width: int, d: Dict[str, Tensor]) -> None:
         """Initialize FullCatalog.
```

### Comparing `bliss_deblender-0.2.0/bliss/conf/base_config.yaml` & `bliss_deblender-0.2.1/bliss/conf/base_config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -78,14 +78,17 @@
     tiles_to_crop: 1
     slack: 1.0
     optimizer_params:
         lr: 1e-3
     scheduler_params:
         milestones: [32]
         gamma: 0.1
+    input_transform_params:
+        use_deconv_channel: false
+        concat_psf_params: false
     architecture:
         # this architecture is based on yolov5l.yaml, see
         # https://github.com/ultralytics/yolov5/blob/master/models/yolov5l.yaml
         depth_multiple: 1.0  # model depth multiple
         width_multiple: 1.0  # layer channel multiple
         anchors:
             - [4, 4]  # P3/8
@@ -156,21 +159,31 @@
     dataset:
         _target_: bliss.surveys.sdss.SloanDigitalSkySurvey
         sdss_dir: ${paths.sdss}
         run: 94
         camcol: 1
         fields: [12]
         bands: [2]
+        predict_device: ${predict.device}
+        predict_crop: ${predict.crop}
+    photo_catalog:
+        _target_: bliss.surveys.sdss.PhotoFullCatalog
+        sdss_dir: ${paths.sdss}
+        run: ${predict.dataset.run}
+        camcol: ${predict.dataset.camcol}
+        fields: ${predict.dataset.fields}
+        bands: ${predict.dataset.bands}
+    trainer: ${training.trainer}
     encoder: ${encoder}
     weight_save_path: ${paths.pretrained_models}/sdss.pt
     device: "cuda:0"
     crop:
         do_crop: true
         left_upper_corner: [160, 160]
         width: 640
         height: 640
     plot:
         show_plot: true
         width: 1000
         height: 1000
-        out_file_name: predict.html
+        out_file_name: ${paths.output}/predict.html
     is_simulated: false
```

### Comparing `bliss_deblender-0.2.0/bliss/encoder.py` & `bliss_deblender-0.2.1/bliss/encoder.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import math
-from typing import Dict, Optional
+from typing import Dict, Optional, Union
 
 import pytorch_lightning as pl
 import torch
 from einops import rearrange
 from matplotlib import pyplot as plt
 from omegaconf import OmegaConf
 from omegaconf.dictconfig import DictConfig
 from torch import Tensor
 from torch.distributions import Distribution
 from torch.optim import Adam
 from torch.optim.lr_scheduler import MultiStepLR
 from yolov5.models.yolo import DetectionModel
 
-from bliss.catalog import TileCatalog
+from bliss.catalog import FullCatalog, TileCatalog
 from bliss.metrics import BlissMetrics
 from bliss.plotting import plot_detections
 from bliss.unconstrained_dists import (
     UnconstrainedBernoulli,
     UnconstrainedDiagonalBivariateNormal,
     UnconstrainedLogitNormal,
     UnconstrainedLogNormal,
@@ -38,47 +38,53 @@
         architecture: DictConfig,
         bands: list,
         tile_slen: int,
         tiles_to_crop: int,
         slack: float = 1.0,
         optimizer_params: Optional[dict] = None,
         scheduler_params: Optional[dict] = None,
+        input_transform_params: Optional[dict] = None,
     ):
         """Initializes DetectionEncoder.
 
         Args:
             architecture: yaml to specifying the encoder network architecture
             bands: specified band-pass filters
             tile_slen: dimension in pixels of a square tile
             tiles_to_crop: margin of tiles not to use for computing loss
             slack: Slack to use when matching locations for validation metrics.
             optimizer_params: arguments passed to the Adam optimizer
             scheduler_params: arguments passed to the learning rate scheduler
+            input_transform_params: used for determining what channels to use as input (e.g.
+                deconvolution, concatenate PSF parameters, z-score inputs, etc.)
         """
         super().__init__()
         self.save_hyperparameters()
 
         self.bands = bands
         self.n_bands = len(self.bands)
         self.optimizer_params = optimizer_params
         self.scheduler_params = scheduler_params if scheduler_params else {"milestones": []}
+        self.input_transform_params = input_transform_params
 
         self.tile_slen = tile_slen
 
         # number of distributional parameters used to characterize each source
         self.n_params_per_source = sum(param.dim for param in self.dist_param_groups.values())
 
         # a hack to get the right number of outputs from yolo
         architecture["nc"] = self.n_params_per_source - 5
         arch_dict = OmegaConf.to_container(architecture)
-        self.model = DetectionModel(cfg=arch_dict, ch=2 * self.n_bands)
+
+        num_channels = self._get_num_input_channels()
+        self.model = DetectionModel(cfg=arch_dict, ch=num_channels)
         self.tiles_to_crop = tiles_to_crop
 
         # metrics
-        self.metrics = BlissMetrics(slack)
+        self.metrics = BlissMetrics(mode=BlissMetrics.Mode.Tile, slack=slack)
 
     @property
     def dist_param_groups(self):
         return {
             "on_prob": UnconstrainedBernoulli(),
             "loc": UnconstrainedDiagonalBivariateNormal(),
             "star_log_flux": UnconstrainedNormal(low_clamp=-6, high_clamp=3),
@@ -89,27 +95,68 @@
             "galsim_beta_radians": UnconstrainedLogitNormal(high=2 * torch.pi),
             "galsim_disk_q": UnconstrainedLogitNormal(),
             "galsim_a_d": UnconstrainedLogNormal(),
             "galsim_bulge_q": UnconstrainedLogitNormal(),
             "galsim_a_b": UnconstrainedLogNormal(),
         }
 
+    def _get_num_input_channels(self):
+        """Determine number of input channels for model based on desired input transforms."""
+        num_channels = 2  # image + background
+        if self.input_transform_params.get("use_deconv_channel"):
+            num_channels += 1
+        if self.input_transform_params.get("concat_psf_params"):
+            num_channels += 6
+        num_channels *= self.n_bands
+        return num_channels
+
+    def get_input_tensor(self, batch):
+        """Extracts data from batch and concatenates into a single tensor to be input into model.
+
+        By default, only the image and background are used. Other input transforms can be specified
+        in self.input_transform_params. Supported options are:
+            use_deconv_channel: add channel for image deconvolved with PSF
+            concat_psf_params: add each PSF parameter as a channel
+            #TODO: add other transforms here, like z-score and multi-band
+
+        Args:
+            batch: input batch (as dictionary)
+
+        Returns:
+            Tensor: b x c x h x w tensor, where the number of input channels `c` is based on the
+                input transformations to use
+        """
+        inputs = [batch["images"], batch["background"]]
+        if self.input_transform_params.get("use_deconv_channel"):
+            assert (
+                "deconvolution" in batch
+            ), "use_deconv_channel specified but deconvolution not present in data"
+            inputs.append(batch["deconvolution"])
+        if self.input_transform_params.get("concat_psf_params"):
+            assert (
+                "psf_params" in batch
+            ), "concat_psf_params specified but psf params not present in data"
+            n, _, h, w = batch["images"].size()
+            inputs.append(batch["psf_params"].view(n, 6, 1, 1).expand(n, 6, h, w))
+        return torch.cat(inputs, dim=1)
+
     def encode_batch(self, batch):
-        images_with_background = torch.cat((batch["images"], batch["background"]), dim=1)
+        # get input tensor from batch with specified channels and transforms
+        inputs = self.get_input_tensor(batch)
 
         # setting this to true every time is a hack to make yolo DetectionModel
         # give us output of the right dimension
         self.model.model[-1].training = True
 
-        assert images_with_background.size(2) % 16 == 0, "image dims must be multiples of 16"
-        assert images_with_background.size(3) % 16 == 0, "image dims must be multiples of 16"
+        assert inputs.size(2) % 16 == 0, "image dims must be multiples of 16"
+        assert inputs.size(3) % 16 == 0, "image dims must be multiples of 16"
         bn_warn = "batchnorm training requires a larger batch. did you mean to use eval mode?"
         assert (not self.training) or batch["images"].size(0) > 4, bn_warn
 
-        output = self.model(images_with_background)
+        output = self.model(inputs)
         # there's an extra dimension for channel that is always a singleton
         output4d = rearrange(output[0], "b 1 ht wt pps -> b ht wt pps")
 
         ttc = self.tiles_to_crop
         if ttc > 0:
             output4d = output4d[:, ttc:-ttc, ttc:-ttc, :]
 
@@ -119,23 +166,33 @@
         pred = dict(zip(names, dist_params_split))
 
         for k, v in pred.items():
             pred[k] = self.dist_param_groups[k].get_dist(v)
 
         return pred
 
-    def variational_mode(self, pred: Dict[str, Tensor]) -> Dict[str, Tensor]:
-        """Compute the mode of the variational distribution."""
+    def variational_mode(
+        self, pred: Dict[str, Tensor], return_full: Optional[bool] = True
+    ) -> Union[FullCatalog, TileCatalog]:
+        """Compute the mode of the variational distribution.
+
+        Args:
+            pred (Dict[str, Tensor]): model predictions
+            return_full (bool, optional): If True, returns a FullCatalog instead of a TileCatalog.
+                Defaults to False.
+
+        Returns:
+            Union[FullCatalog, TileCatalog]: Catalog based on predictions.
+        """
         # the mean would be better at minimizing squared error...should we return that instead?
         tile_is_on_array = pred["on_prob"].mode
         # this is the mode of star_log_flux but not the mean of the star_flux distribution
         star_fluxes = pred["star_log_flux"].mode.exp()  # type: ignore
-        star_fluxes *= tile_is_on_array
-        galaxy_bools = pred["galaxy_prob"].mode * pred["on_prob"].mode  # type: ignore
-        star_bools = (1 - pred["galaxy_prob"].mode) * pred["on_prob"].mode  # type: ignore
+        galaxy_bools = pred["galaxy_prob"].mode  # type: ignore
+        star_bools = 1 - pred["galaxy_prob"].mode  # type: ignore
 
         galsim_names = ["flux", "disk_frac", "beta_radians", "disk_q", "a_d", "bulge_q", "a_b"]
         galsim_dists = [pred[f"galsim_{name}"] for name in galsim_names]
         # for params with transformed distribution mode and median aren't implemented.
         # instead, we compute median using inverse cdf 0.5
         galsim_param_lst = [d.icdf(torch.tensor(0.5)) for d in galsim_dists]  # type: ignore
         galaxy_params = torch.stack(galsim_param_lst, dim=3)
@@ -149,15 +206,15 @@
             "n_sources": tile_is_on_array,
             "galaxy_bools": rearrange(galaxy_bools, "b ht wt -> b ht wt 1 1"),
             "star_bools": rearrange(star_bools, "b ht wt -> b ht wt 1 1"),
             "galaxy_params": rearrange(galaxy_params, "b ht wt d -> b ht wt 1 d"),
         }
 
         est_tile_catalog = TileCatalog(self.tile_slen, est_catalog_dict)
-        return est_tile_catalog.to_full_params()
+        return est_tile_catalog if not return_full else est_tile_catalog.to_full_params()
 
     def configure_optimizers(self):
         """Configure optimizers for training (pytorch lightning)."""
         optimizer = Adam(self.parameters(), **self.optimizer_params)
         scheduler = MultiStepLR(optimizer, **self.scheduler_params)
         return [optimizer], [scheduler]
 
@@ -212,37 +269,40 @@
 
     def _generic_step(self, batch, logging_name, log_metrics=False, plot_images=False):
         batch_size = batch["images"].size(0)
         pred = self.encode_batch(batch)
         true_tile_cat = TileCatalog(self.tile_slen, batch["tile_catalog"])
         true_tile_cat = true_tile_cat.symmetric_crop(self.tiles_to_crop)
         loss_dict = self._get_loss(pred, true_tile_cat)
-        true_full_cat = true_tile_cat.to_full_params()
-        est_cat = self.variational_mode(pred)
+        est_tile_cat = self.variational_mode(pred, return_full=False)  # get tile cat for metrics
 
         # log all losses
         for k, v in loss_dict.items():
             self.log("{}/{}".format(logging_name, k), v, batch_size=batch_size)
 
         # log all metrics
         if log_metrics:
-            metrics = self.metrics(true_full_cat, est_cat)
+            metrics = self.metrics(true_tile_cat, est_tile_cat)
             for k, v in metrics.items():
                 self.log("{}/{}".format(logging_name, k), v, batch_size=batch_size)
 
         # log a grid of figures to the tensorboard
         if plot_images:
             batch_size = len(batch["images"])
             n_samples = min(int(math.sqrt(batch_size)) ** 2, 16)
             nrows = int(n_samples**0.5)  # for figure
-            wrong_idx = (est_cat.n_sources != true_full_cat.n_sources).nonzero()
+
+            true_full_cat = true_tile_cat.to_full_params()
+            est_full_cat = est_tile_cat.to_full_params()
+            wrong_idx = (est_full_cat.n_sources != true_full_cat.n_sources).nonzero()
             wrong_idx = wrong_idx.view(-1)[:n_samples]
+
             margin_px = self.tiles_to_crop * self.tile_slen
             fig = plot_detections(
-                batch["images"], true_full_cat, est_cat, nrows, wrong_idx, margin_px
+                batch["images"], true_full_cat, est_full_cat, nrows, wrong_idx, margin_px
             )
             title_root = f"Epoch:{self.current_epoch}/"
             title = f"{title_root}{logging_name} images"
             if self.logger:
                 self.logger.experiment.add_figure(title, fig)
             plt.close(fig)
 
@@ -250,19 +310,26 @@
 
     def training_step(self, batch, batch_idx, optimizer_idx=0):
         """Training step (pytorch lightning)."""
         return self._generic_step(batch, "train")
 
     def validation_step(self, batch, batch_idx):
         """Pytorch lightning method."""
-        self._generic_step(batch, "val", log_metrics=True, plot_images=batch_idx == 0)
-        return batch  # do we really need to save all these batches?
-
-    def validation_epoch_end(self, outputs):
-        """Pytorch lightning method."""
-        batch: Dict[str, Tensor] = outputs[-1]
-        self._generic_step(batch, "val")
+        # only plot images on the first batch of epoch
+        plot_images = batch_idx == 0
+        self._generic_step(batch, "val", log_metrics=True, plot_images=plot_images)
 
     def test_step(self, batch, batch_idx):
         """Pytorch lightning method."""
         self._generic_step(batch, "test", log_metrics=True)
-        return batch  # do we really need to save all these batches?
+
+    def predict_step(self, batch, batch_idx, dataloader_idx=0):
+        """Pytorch lightning method."""
+        with torch.no_grad():
+            pred = self.encode_batch(batch)
+            est_cat = self.variational_mode(pred)
+        return {
+            "est_cat": est_cat,
+            "images": batch["images"],
+            "background": batch["background"],
+            "pred": pred,
+        }
```

### Comparing `bliss_deblender-0.2.0/bliss/generate.py` & `bliss_deblender-0.2.1/bliss/generate.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,21 @@
 from omegaconf import DictConfig, OmegaConf
 from tqdm import tqdm
 
 from bliss.catalog import TileCatalog
 
 FileDatum = TypedDict(
     "FileDatum",
-    {"tile_catalog": TileCatalog, "images": torch.Tensor, "background": torch.Tensor},
+    {
+        "tile_catalog": TileCatalog,
+        "images": torch.Tensor,
+        "background": torch.Tensor,
+        "deconvolution": torch.Tensor,
+        "psf_params": torch.Tensor,
+    },
 )
 
 
 def generate(cfg: DictConfig):
     max_images_per_file = cfg.generate.max_images_per_file
     cached_data_path = cfg.generate.cached_data_path
     files_start_idx = cfg.generate.files_start_idx
@@ -36,15 +42,15 @@
         cfg.simulator, num_workers=n_workers_per_process, prior={"batch_size": bs}
     )
     simulated_dataset = simulator.train_dataloader().dataset
 
     # create cached_data_path if it doesn't exist
     if not os.path.exists(cached_data_path):
         os.makedirs(cached_data_path)
-    print("Data will be saved to {}".format(cached_data_path))
+    print("Data will be saved to {}".format(cached_data_path))  # noqa: WPS421
 
     # Save Hydra config (used to generate data) to cached_data_path
     with open(f"{cfg.generate.cached_data_path}/hparams.yaml", "w", encoding="utf-8") as f:
         OmegaConf.save(cfg, f)
 
     # assume overwriting any existing cached image files
     file_idxs = range(files_start_idx, files_start_idx + n_files)
@@ -63,32 +69,37 @@
         batch_data.append(next(iter(simulated_dataset)))
     return batch_data
 
 
 def itemize_data(batch_data) -> List[FileDatum]:
     flat_data = {}
 
+    # flatten tile catalog
     tile_catalog_flattened = {}
     for key in batch_data[0]["tile_catalog"].keys():
         batch_tc_key = torch.stack([data["tile_catalog"][key] for data in batch_data])
         tile_catalog_flattened[key] = rearrange(batch_tc_key, "b c ... -> (b c) ...")
     flat_data["tile_catalog"] = tile_catalog_flattened
 
-    batch_images = torch.stack([data["images"] for data in batch_data])
-    batch_bg = torch.stack([data["background"] for data in batch_data])
-    flat_data["images"] = rearrange(batch_images, "b c ... -> (b c) ...")  # type: ignore
-    flat_data["background"] = rearrange(batch_bg, "b c ... -> (b c) ...")  # type: ignore
+    # flatten the rest of the data
+    keys = ["images", "background", "deconvolution", "psf_params"]
+    for key in keys:
+        if key in batch_data[0]:
+            batch_ch = torch.stack([data[key] for data in batch_data])
+            flat_data[key] = rearrange(batch_ch, "b c ... -> (b c) ...")
 
     # reconstruct data as list of single-input FileDatum dictionaries
     n_items = len(flat_data["images"])
     file_data: List[FileDatum] = []
     for i in range(n_items):
         file_datum: FileDatum = {}  # type: ignore
         # construct a TileCatalog dictionary of ith-input tensors
         file_datum["tile_catalog"] = {  # type: ignore
             k: flat_data["tile_catalog"][k][i] for k in flat_data["tile_catalog"].keys()
         }
         file_datum["images"] = flat_data["images"][i]
         file_datum["background"] = flat_data["background"][i]
+        file_datum["deconvolution"] = flat_data["deconvolution"][i]
+        file_datum["psf_params"] = flat_data["psf_params"][i]
         file_data.append(file_datum)
 
     return file_data
```

### Comparing `bliss_deblender-0.2.0/bliss/simulator/background.py` & `bliss_deblender-0.2.1/bliss/simulator/background.py`

 * *Files identical despite different names*

### Comparing `bliss_deblender-0.2.0/bliss/simulator/decoder.py` & `bliss_deblender-0.2.1/bliss/simulator/decoder.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-import os
+from pathlib import Path
 from typing import Tuple
 
 import galsim
 import numpy as np
 import torch
 from astropy.io import fits
 from einops import rearrange, reduce
 from omegaconf import DictConfig
 from torch import Tensor, nn
 
 from bliss.catalog import TileCatalog
+from bliss.surveys.sdss import SDSSDownloader
 
 
 class ImageDecoder(nn.Module):
     def __init__(
         self,
         pixel_scale: float,
         psf_slen: int,
@@ -21,31 +22,35 @@
     ) -> None:
         super().__init__()
 
         self.n_bands = len(sdss_fields["bands"])
         self.pixel_scale = pixel_scale
         self.psf_slen = psf_slen
         self.psf_galsim = {}  # Dictionary indexed by (run, camcol, field) tuple
+        self.psf_params = {}
 
         sdss_dir = sdss_fields["dir"]
         sdss_bands = sdss_fields["bands"]
 
         for field_params in sdss_fields["field_list"]:
             run = field_params["run"]
             camcol = field_params["camcol"]
             fields = field_params["fields"]
 
             for field in fields:
                 # load raw params from file
                 field_dir = f"{sdss_dir}/{run}/{camcol}/{field}"
                 filename = f"{field_dir}/psField-{run:06}-{camcol}-{field:04}.fits"
+                if not Path(filename).exists():
+                    SDSSDownloader(run, camcol, field, download_dir=sdss_dir).download_psfield()
                 psf_params = self._get_fit_file_psf_params(filename, sdss_bands)
 
                 # load psf image from params
                 self.psf_galsim[(run, camcol, field)] = self._get_psf(psf_params)
+                self.psf_params[(run, camcol, field)] = psf_params
 
     def _get_psf(self, params):
         """Construct PSF image from parameters. This is the main entry point for generating the psf.
 
         Args:
             params: list of psf parameters, loaded from _get_fit_file_psf_params
 
@@ -99,15 +104,15 @@
         Returns:
             psf_params: tensor of parameters for each band
         """
         msg = (
             f"{psf_fit_file} does not exist. "
             + "Make sure data files are available for fields specified in config."
         )
-        assert os.path.exists(psf_fit_file), msg
+        assert Path(psf_fit_file).exists(), msg
         # HDU 6 contains the PSF header (after primary and eigenimages)
         data = fits.open(psf_fit_file, ignore_missing_end=True).pop(6).data
         psf_params = torch.zeros(len(bands), 6)
         for i, band in enumerate(bands):
             sigma1 = data["psf_sigma1"][0][band] ** 2
             sigma2 = data["psf_sigma2"][0][band] ** 2
             sigmap = data["psf_sigmap"][0][band] ** 2
@@ -141,14 +146,31 @@
 
         term1 = torch.exp(-(r**2) / (2 * sigma1))
         term2 = b * torch.exp(-(r**2) / (2 * sigma2))
         term3 = p0 * (1 + r**2 / (beta * sigmap)) ** (-beta / 2)
         return (term1 + term2 + term3) / (1 + b + p0)
 
     def render_galaxy(self, galaxy_params: Tensor, psf, bnd: int):
+        """Render a galaxy with given params and PSF.
+
+        Args:
+            galaxy_params (Tensor): Tensor containing the following parameters:
+                - total_flux: the total flux of the galaxy
+                - disk_frac: the fraction of flux attributed to the disk (rest goes to bulge)
+                - beta_radians: the angle of shear in radians
+                - disk_q: the minor-to-major axis ratio of the disk
+                - a_d: semi-major axis of disk
+                - bulge_q: minor-to-major axis ratio of the bulge
+                - a_b: semi-major axis of bulge
+            psf (List): a list of PSFs for each band
+            bnd (int): band
+
+        Returns:
+            GSObject: a galsim representation of the rendered galaxy convolved with the PSF
+        """
         galaxy_params = galaxy_params.cpu().detach()
         total_flux, disk_frac, beta_radians, disk_q, a_d, bulge_q, a_b = galaxy_params
         bulge_frac = 1 - disk_frac
 
         disk_flux = total_flux * disk_frac
         bulge_flux = total_flux * bulge_frac
 
@@ -167,25 +189,39 @@
             bulge = galsim.DeVaucouleurs(flux=bulge_flux, half_light_radius=bulge_hlr_arcsecs)
             sheared_bulge = bulge.shear(q=bulge_q, beta=beta_radians * galsim.radians)
             components.append(sheared_bulge)
         galaxy = galsim.Add(components)
         return galsim.Convolution(galaxy, psf[bnd])
 
     def render_images(self, tile_cat: TileCatalog, rcf):
+        """Render images from a tile catalog.
+
+        Args:
+            tile_cat (TileCatalog): the tile catalog to create images from
+            rcf (ndarray): array containing the row/camcol/field of PSFs to use
+
+        Raises:
+            AssertionError: rcf must contain batch_size values
+
+        Returns:
+            Tuple[Tensor, List, Tensor]: tensor of images, list of PSFs, tensor of PSF params
+        """
         batch_size, n_tiles_h, n_tiles_w = tile_cat.n_sources.shape
         assert rcf.shape[0] == batch_size
 
         slen_h = tile_cat.tile_slen * n_tiles_h
         slen_w = tile_cat.tile_slen * n_tiles_w
         images = np.zeros((batch_size, self.n_bands, slen_h, slen_w), dtype=np.float32)
 
         full_cat = tile_cat.to_full_params()
 
         # use the PSF from specified row/camcol/field
         psfs = [self.psf_galsim[tuple(rcf[b])] for b in range(batch_size)]  # type: ignore
+        param_list = [self.psf_params[tuple(rcf[b])] for b in range(batch_size)]  # type: ignore
+        psf_params = torch.stack(param_list, dim=0)  # type: ignore
 
         # Nested looping + conditionals are necessary for the drawing of each light
         # source. Ignored relevant style checks for that reason.
         for b in range(batch_size):
             n_sources = int(full_cat.n_sources[b].item())
             psf = psfs[b]
             for bnd in range(self.n_bands):
@@ -213,8 +249,8 @@
                     # to drawImage
                     galsim_obj.drawImage(
                         offset=offset, method="auto", add_to_image=True, image=gs_img
                     )
         # TODO: clamp image values. strange issue - happens only after galsim rendering
         images[images < 1e-8] = 1.1e-8
 
-        return torch.from_numpy(images)
+        return torch.from_numpy(images), psfs, psf_params
```

### Comparing `bliss_deblender-0.2.0/bliss/simulator/prior.py` & `bliss_deblender-0.2.1/bliss/simulator/prior.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import itertools
-import os
 import random
 from pathlib import Path
 
 import numpy as np
 import pytorch_lightning as pl
 import torch
 from astropy.io import fits
 from omegaconf.dictconfig import DictConfig
 from torch import Tensor
 from torch.distributions import Gamma, Poisson, Uniform
 
 from bliss.catalog import TileCatalog, get_is_on_from_n_sources
-from bliss.surveys.sdss import column_to_tensor
+from bliss.surveys.sdss import SDSSDownloader, column_to_tensor
 
 
 class ImagePrior(pl.LightningModule):
     """Prior distribution of objects in an astronomical image.
 
     After the module is initialized, sampling is done with the sample_prior method.
     The input parameters correspond to the number of sources, the fluxes, whether an
@@ -214,19 +213,21 @@
             run = field_params["run"]
             camcol = field_params["camcol"]
             fields = field_params["fields"]
             for field in fields:
                 sdss_path = Path(self.sdss)
                 camcol_dir = sdss_path / str(run) / str(camcol) / str(field)
                 po_path = camcol_dir / f"photoObj-{run:06d}-{camcol:d}-{field:04d}.fits"
+                if not po_path.exists():
+                    SDSSDownloader(run, camcol, field, str(sdss_path)).download_po()
                 msg = (
                     f"{po_path} does not exist. "
                     + "Make sure data files are available for fields specified in config."
                 )
-                assert os.path.exists(po_path), msg
+                assert Path(po_path).exists(), msg
                 po_fits = fits.getdata(po_path)
 
                 fluxes = column_to_tensor(po_fits, "psfflux")
                 objc_type = column_to_tensor(po_fits, "objc_type").numpy()
                 thing_id = column_to_tensor(po_fits, "thing_id").numpy()
 
                 star_fluxes_rest = []
```

### Comparing `bliss_deblender-0.2.0/bliss/simulator/simulated_dataset.py` & `bliss_deblender-0.2.1/bliss/simulator/simulated_dataset.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import warnings
 from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import pytorch_lightning as pl
 import torch
 from omegaconf.listconfig import ListConfig
+from skimage.restoration import richardson_lucy
 from torch import Tensor
 from torch.utils.data import DataLoader, Dataset, IterableDataset
 from tqdm import tqdm
 
 from bliss.catalog import TileCatalog
 from bliss.generate import FileDatum
 from bliss.simulator.background import ConstantBackground, SimulatedSDSSBackground
@@ -75,51 +76,93 @@
     def _apply_noise(images_mean):
         # add noise to images.
         assert torch.all(images_mean > 1e-8)
         images = torch.sqrt(images_mean) * torch.randn_like(images_mean)
         images += images_mean
         return images
 
-    def simulate_image(self, tile_catalog: TileCatalog, rcf_indices) -> Tuple[Tensor, Tensor]:
+    def simulate_image(
+        self, tile_catalog: TileCatalog, rcf_indices
+    ) -> Tuple[Tensor, Tensor, Tensor, Tensor]:
         """Simulate a batch of images.
 
         Args:
             tile_catalog (TileCatalog): The TileCatalog to render.
             rcf_indices: Indices of row/camcol/field in self.rcf_list to sample from.
 
         Returns:
-            Tuple[Tensor, Tensor]: tuple of images and backgrounds
+            Tuple[Tensor, Tensor, Tensor, Tensor]: tuple of images, backgrounds, deconvolved images,
+            and psf parameters
         """
         rcf = self.rcf_list[rcf_indices]
-        images = self.image_decoder.render_images(tile_catalog, rcf)
+        images, psfs, psf_params = self.image_decoder.render_images(tile_catalog, rcf)
         background = self.background.sample(images.shape, rcf_indices=rcf_indices)  # type: ignore
         images += background
         images = self._apply_noise(images)
-        return images, background
+        deconv_images = self.get_deconvolved_images(images, background, psfs)
+        return images, background, deconv_images, psf_params
+
+    def get_deconvolved_images(self, images, backgrounds, psfs) -> Tensor:
+        """Deconvolve the synthetic images with the psf used to generate them.
+
+        Args:
+            images (ndarray): batch of images
+            backgrounds (ndarray): batch of backgrounds
+            psfs (ndarray): batch of psfs
+
+        Returns:
+            Tensor: batch of deconvolved images
+        """
+        deconv_images = np.zeros_like(images)
+        for i in range(images.shape[0]):
+            for band in range(self.image_prior.n_bands):
+                deconv_images[i][band] = self.deconvolve_image(
+                    images[i][band], backgrounds[i][band], psfs[i][band]
+                )
+        return torch.from_numpy(deconv_images)
+
+    def deconvolve_image(self, image, background, psf, pad=10):
+        """Deconvolve a single image.
+
+        Args:
+            image (Tensor): the image to deconvolve
+            background (Tensor): background of the image (used for padding)
+            psf (ndarray): the psf used to generate the image
+            pad (int): the pad width (in pixels). Defaults to 10.
+
+        Returns:
+            ndarray: the deconvolved image, same size as the original
+        """
+        padded_image = np.pad(image, pad, mode="constant", constant_values=background.mean().item())
+        normalized = padded_image / np.max(padded_image)
+        deconv = richardson_lucy(normalized, psf.original.image.array)
+        return deconv[pad:-pad, pad:-pad]
 
     def get_batch(self) -> Dict:
         """Get a batch of simulated images.
 
         The images are simulated by first generating a tile catalog from the prior, followed
         by choosing a random background and PSF and using those to generate the image. By default,
         the same row, camcol, and field combination is used for the background, PSF, and flux ratios
         of a single simulated image.
 
         Returns:
-            A dictionary of the simulated TileCatalog, and (batch_size, bands, height, width)
-            tensors for images and background.
+            Dict: A dictionary of the simulated TileCatalog, (batch_size, bands, height, width)
+            tensors for images and background, and a (batch_size, 1, 6) tensor for the psf params.
         """
         rcfs, rcf_indices = self.get_random_rcf(self.image_prior.batch_size)
         with torch.no_grad():
             tile_catalog = self.image_prior.sample_prior(rcfs)
-            images, background = self.simulate_image(tile_catalog, rcf_indices)
+            images, background, deconv, psf_params = self.simulate_image(tile_catalog, rcf_indices)
             return {
                 "tile_catalog": tile_catalog.to_dict(),
                 "images": images,
                 "background": background,
+                "deconvolution": deconv,
+                "psf_params": psf_params,
             }
 
     def __iter__(self):
         for _ in range(self.n_batches):
             yield self.get_batch()
 
     def train_dataloader(self):
```

### Comparing `bliss_deblender-0.2.0/bliss/surveys/decals.py` & `bliss_deblender-0.2.1/bliss/surveys/decals.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import torch
 from astropy.table import Table
 from astropy.wcs import WCS
 
 from bliss.catalog import FullCatalog
 from bliss.surveys.sdss import column_to_tensor
+from bliss.utils.download_utils import download_git_lfs_file
 
 
 class DecalsFullCatalog(FullCatalog):
     """Class for the Decals Sweep Tractor Catalog.
 
     Some resources:
     - https://portal.nersc.gov/cfs/cosmo/data/legacysurvey/dr9/south/sweep/9.0/
@@ -43,14 +44,16 @@
 
         Returns:
             A DecalsFullCatalog containing data from the provided file. Note that the
             coordinates in (RA, DEC) are not converted to plocs by default. For this,
             use get_plocs_from_ra_dec after loading the data.
         """
         catalog_path = Path(decals_cat_path)
+        if not catalog_path.exists():
+            download_decals_base(str(catalog_path.parent))
         table = Table.read(catalog_path, format="fits", unit_parse_strict="silent")
         table = {k.upper(): v for k, v in table.items()}  # uppercase keys
         band = band.capitalize()
 
         # filter out pixels that aren't in primary region, had issues with source fitting,
         # in SGA large galaxy, or in a globular cluster. In the future this should probably
         # be an input parameter.
@@ -119,7 +122,22 @@
         dec = self["dec"].numpy().squeeze()
 
         pt, pr = wcs.all_world2pix(ra, dec, 0)  # convert to pixel coordinates
         pt = torch.tensor(pt)
         pr = torch.tensor(pr)
         plocs = torch.stack((pr, pt), dim=-1)
         return plocs.reshape(1, plocs.size()[0], 2) + 0.5  # BLISS consistency
+
+
+def download_decals_base(download_dir: str):
+    cutout_filename = "cutout_336.635_-0.9600.fits"
+    tractor_filename = "tractor-3366m010.fits"
+    cutout = download_git_lfs_file(
+        f"https://api.github.com/repos/prob-ml/bliss/contents/data/decals/{cutout_filename}"
+    )
+    tractor = download_git_lfs_file(
+        f"https://api.github.com/repos/prob-ml/bliss/contents/data/decals/{tractor_filename}"
+    )
+    cutout_path = Path(download_dir) / cutout_filename
+    tractor_path = Path(download_dir) / tractor_filename
+    cutout_path.write_bytes(cutout)
+    tractor_path.write_bytes(tractor)
```

### Comparing `bliss_deblender-0.2.0/bliss/train.py` & `bliss_deblender-0.2.1/bliss/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 def train(cfg: DictConfig):  # pylint: disable=too-many-branches, too-many-statements
     # setup paths and seed
     paths = OmegaConf.to_container(cfg.paths, resolve=True)
     assert isinstance(paths, dict)
     for key in paths.keys():
         path = Path(paths[key])
         if not path.exists():
-            if key == "output":
+            if key in ["data", "sdss", "decals", "output", "pretrained_models"]:  # noqa: WPS510
                 path.mkdir(parents=True)
             else:
                 err = "path for {} ({}) does not exist".format(str(key), path.as_posix())
                 raise FileNotFoundError(err)
     pl.seed_everything(cfg.training.seed)
 
     # setup dataset.
```

### Comparing `bliss_deblender-0.2.0/bliss/unconstrained_dists.py` & `bliss_deblender-0.2.1/bliss/unconstrained_dists.py`

 * *Files identical despite different names*

### Comparing `bliss_deblender-0.2.0/pyproject.toml` & `bliss_deblender-0.2.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -14,38 +14,36 @@
 documentation = "https://prob-ml.github.io/bliss/"
 keywords = ["cosmology", "blending", "weak lensing", "bayesian", "ml", "pytorch"]
 license = "MIT"
 name = "bliss-deblender"
 packages = [{include = "bliss"}]
 readme = "README.md"
 repository = "https://github.com/prob-ml/bliss"
-version = "0.2.0"
+version = "0.2.1"
 
 [tool.poetry.scripts]
 bliss = "main:main"
 
 [tool.poetry.dependencies]
-astropy = ">=4.2.1"
-einops = ">=0.3.0"
-galsim = ">=2.2.4"
-hydra-core = ">=1.0.4"
-matplotlib = ">=3.3.3"
-nflows = ">=0.14"
-numpy = ">=1.18.5"
 python = "^3.10"
-pytorch-lightning = ">=1.9"
-scikit-learn = ">=0.24.2"
+numpy = ">=1.18.5"
 scipy = ">=1.4.1"
-seaborn = ">=0.11.2"
+matplotlib = ">=3.3.3"
+scikit-learn = ">=0.24.2"
+scikit-image = ">=0.20.0"
+requests = "^2.31.0"
 torch = ">=1.9"
 torchmetrics = ">=0.5.1"
+pytorch-lightning = ">=1.9"
+einops = ">=0.3.0"
+hydra-core = ">=1.0.4"
 yolov5 = "^7.0.9"
 bokeh = "^3.1.1"
-requests = "^2.31.0"
-types-requests = "^2.31.0.1"
+astropy = ">=4.2.1"
+galsim = ">=2.2.4"
 
 [tool.poetry.dev-dependencies]
 Cython = ">=0.29.21"
 Sphinx = ">=4.0.2"
 black = ">=22.3.0"
 darglint = ">=1.8.1"
 flake8 = ">=4.0.1"
@@ -58,30 +56,39 @@
 nbstripout = ">=0.5.0"
 plotly = ">=4.14.3"
 pre-commit = ">=2.9.2"
 pre-commit-hooks = "^4.4.0"
 pylint = ">=2.6.0"
 pytest = ">=6.1.2"
 pytest-cov = ">=2.10"
-pytest-mypy = ">=0.9.1"
 sphinx-rtd-theme = ">=0.5.2"
 torch-tb-profiler = "^0.4.1"
 tqdm = ">=4.62.3"
 wemake-python-styleguide = ">=0.16.1"
 nbsphinx = "^0.9.2"
+pypandoc = "^1.11"
+types-requests = "^2.31.0.1"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
 
 [tool.black]
 line-length = 100
 target-version = ['py310']
 
-# pyproject.toml
+[tool.isort]
+multi_line_output = 3
+profile = "black"
+include_trailing_comma = true
+force_grid_wrap = 0
+use_parentheses = true
+ensure_newline_before_comments = true
+line_length = 100
+
 [tool.pytest.ini_options]
 addopts = "-ra"
 filterwarnings = [
   "ignore:.*does not have many workers which may be a bottleneck.*:UserWarning",
   "ignore:GPU available but not used.*:UserWarning",
   "ignore:numpy.ndarray size changed:RuntimeWarning",
   "ignore:.*when logging on epoch level in distributed setting.*",
```

### Comparing `bliss_deblender-0.2.0/PKG-INFO` & `bliss_deblender-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bliss-deblender
-Version: 0.2.0
+Version: 0.2.1
 Summary: Bayesian Light Source Separator
 Home-page: https://github.com/prob-ml/bliss
 License: MIT
 Keywords: cosmology,blending,weak lensing,bayesian,ml,pytorch
 Author: Ismael Mendoza
 Author-email: imendoza@umich.edu
 Requires-Python: >=3.10,<4.0
@@ -14,24 +14,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: astropy (>=4.2.1)
 Requires-Dist: bokeh (>=3.1.1,<4.0.0)
 Requires-Dist: einops (>=0.3.0)
 Requires-Dist: galsim (>=2.2.4)
 Requires-Dist: hydra-core (>=1.0.4)
 Requires-Dist: matplotlib (>=3.3.3)
-Requires-Dist: nflows (>=0.14)
 Requires-Dist: numpy (>=1.18.5)
 Requires-Dist: pytorch-lightning (>=1.9)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: scikit-image (>=0.20.0)
 Requires-Dist: scikit-learn (>=0.24.2)
 Requires-Dist: scipy (>=1.4.1)
-Requires-Dist: seaborn (>=0.11.2)
 Requires-Dist: torch (>=1.9)
 Requires-Dist: torchmetrics (>=0.5.1)
-Requires-Dist: types-requests (>=2.31.0.1,<3.0.0.0)
 Requires-Dist: yolov5 (>=7.0.9,<8.0.0)
 Project-URL: Documentation, https://prob-ml.github.io/bliss/
 Project-URL: Repository, https://github.com/prob-ml/bliss
 Description-Content-Type: text/markdown
 
 ![](http://portal.nersc.gov/project/dasrepo/celeste/sample_sky.jpg)
```

