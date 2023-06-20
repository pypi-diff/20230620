# Comparing `tmp/omero-cli-transfer-0.3.3.tar.gz` & `tmp/omero-cli-transfer-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/omero-cli-transfer-0.3.3.tar", last modified: Thu Jan 26 15:28:38 2023, max compression
+gzip compressed data, was "dist/omero-cli-transfer-0.4.0.tar", last modified: Mon Feb  6 19:30:04 2023, max compression
```

## Comparing `omero-cli-transfer-0.3.3.tar` & `omero-cli-transfer-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 15:28:38.000000 omero-cli-transfer-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-01-26 15:28:38.000000 omero-cli-transfer-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-01-26 15:28:27.000000 omero-cli-transfer-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-26 15:28:38.000000 omero-cli-transfer-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-01-26 15:28:27.000000 omero-cli-transfer-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 15:28:38.000000 omero-cli-transfer-0.3.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)    19474 2023-01-26 15:28:27.000000 omero-cli-transfer-0.3.3/src/generate_omero_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    35326 2023-01-26 15:28:27.000000 omero-cli-transfer-0.3.3/src/generate_xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 15:28:38.000000 omero-cli-transfer-0.3.3/src/omero/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 15:28:38.000000 omero-cli-transfer-0.3.3/src/omero/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-01-26 15:28:27.000000 omero-cli-transfer-0.3.3/src/omero/plugins/transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 15:28:38.000000 omero-cli-transfer-0.3.3/src/omero_cli_transfer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-01-26 15:28:38.000000 omero-cli-transfer-0.3.3/src/omero_cli_transfer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-01-26 15:28:38.000000 omero-cli-transfer-0.3.3/src/omero_cli_transfer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 15:28:38.000000 omero-cli-transfer-0.3.3/src/omero_cli_transfer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-26 15:28:38.000000 omero-cli-transfer-0.3.3/src/omero_cli_transfer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-26 15:28:38.000000 omero-cli-transfer-0.3.3/src/omero_cli_transfer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20962 2023-01-26 15:28:27.000000 omero-cli-transfer-0.3.3/src/omero_cli_transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 19:30:04.000000 omero-cli-transfer-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-02-06 19:30:04.000000 omero-cli-transfer-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-02-06 19:29:54.000000 omero-cli-transfer-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-06 19:30:04.000000 omero-cli-transfer-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-02-06 19:29:54.000000 omero-cli-transfer-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 19:30:04.000000 omero-cli-transfer-0.4.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    19476 2023-02-06 19:29:54.000000 omero-cli-transfer-0.4.0/src/generate_omero_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36386 2023-02-06 19:29:54.000000 omero-cli-transfer-0.4.0/src/generate_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 19:30:04.000000 omero-cli-transfer-0.4.0/src/omero/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 19:30:04.000000 omero-cli-transfer-0.4.0/src/omero/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-02-06 19:29:54.000000 omero-cli-transfer-0.4.0/src/omero/plugins/transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 19:30:04.000000 omero-cli-transfer-0.4.0/src/omero_cli_transfer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-02-06 19:30:04.000000 omero-cli-transfer-0.4.0/src/omero_cli_transfer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-02-06 19:30:04.000000 omero-cli-transfer-0.4.0/src/omero_cli_transfer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 19:30:04.000000 omero-cli-transfer-0.4.0/src/omero_cli_transfer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-06 19:30:04.000000 omero-cli-transfer-0.4.0/src/omero_cli_transfer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-06 19:30:04.000000 omero-cli-transfer-0.4.0/src/omero_cli_transfer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    21769 2023-02-06 19:29:54.000000 omero-cli-transfer-0.4.0/src/omero_cli_transfer.py
```

### Comparing `omero-cli-transfer-0.3.3/PKG-INFO` & `omero-cli-transfer-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 Metadata-Version: 2.1
 Name: omero-cli-transfer
-Version: 0.3.3
+Version: 0.4.0
 Summary: A set of utilities for exporting a transfer packet from an OMERO server and importing it in a different server. Developed by the Research IT team at The Jackson Laboratory.
 Home-page: https://github.com/TheJacksonLaboratory/omero-cli-transfer
 Maintainer: Erick Ratamero
 Maintainer-email: erick.ratamero@jax.org
 License: UNKNOWN
 Description: # omero-cli-transfer
+        
+        
+        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7573592.svg)](https://doi.org/10.5281/zenodo.7573592)
+        
+        
         An OMERO CLI plugin for creating and using transfer packets between OMERO servers.
         
         Transfer packets contain objects and annotations. This project creates a zip file from an object 
         (Project, Dataset, Image, Screen, Plate) containing all original files necessary to create the images 
         in that object, plus an XML file detailing the links between entities, annotations and ROIs thereof.
         
         The CLI plugin add the subcommand `transfer`, which in its turn has two further subcommands `omero transfer pack` and `omero transfer unpack`. Both subcommands (pack and unpack) will use an existing OMERO session created via CLI or prompt the user for parameters to create one.
@@ -30,14 +35,20 @@
         pip install omero-cli-transfer
         ```
         It is possible to do the same thing without `conda` as long as your python/pip version is at least 3.7,
         but that will require locally building a wheel for `zeroc-ice` (which pip does automatically) - it is a
         process that can be anything from "completely seamless and without issues" to "I need to install every 
         dependency ever imagined". Try at your own risk.
         
+        If you want optional RO-Crate exports, you can do 
+        ```
+        pip install omero-cli-transfer[rocrate]
+        ```
+        instead.
+        
         # Usage
         
         ## `omero transfer pack`
         
         Creates a transfer packet for moving objects between OMERO server instances.
         
         The syntax for specifying objects is: `<object>:<id>` where `<object>` can be `Image`, `Project`, `Dataset`, `Plate` or `Screen`. `Project` is assumed if `<object>:` is omitted. A file path needs to be provided; a tar file with the contents of the packet will be created at the specified path.
@@ -84,10 +95,17 @@
         
             - one line per file being submitted, between `Image` files and `FileAnnotation` files;
             - a column indicating whether that file was originally an `Image` or `FileAnnotation`;
             - a "comment" column if any Image has a `CommentAnnotation`;
             - a column per key in a `MapAnnotation` inside the pack, with an empty value for all images but the ones with a `MapAnnotation` with that key; for those images, it has the value for that annotation;
             - a final `original_omero_ids` column listing all OMERO IDs associated to that file in the origin server: for images, that is all `Image` IDs that use that file, and for file annotations that is all `Image` IDs that had that `FileAnnotation` attached to them.
         
+        
+        ### RO-Crate export format
+        
+        - This requires an optional dependency on `ro-crate-py` that can be installed with `pip install omero-cli-transfer[rocrate]`.
+        - Largely due to library limitations, current exports create a flat structure inside a zip file. For each image, `name` and `mimetype` are recorded. A `ro-crate-metadata.json` is added to the zip file.
+        
 Platform: UNKNOWN
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: rocrate
```

### Comparing `omero-cli-transfer-0.3.3/README.md` & `omero-cli-transfer-0.4.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 # omero-cli-transfer
+
+
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7573592.svg)](https://doi.org/10.5281/zenodo.7573592)
+
+
 An OMERO CLI plugin for creating and using transfer packets between OMERO servers.
 
 Transfer packets contain objects and annotations. This project creates a zip file from an object 
 (Project, Dataset, Image, Screen, Plate) containing all original files necessary to create the images 
 in that object, plus an XML file detailing the links between entities, annotations and ROIs thereof.
 
 The CLI plugin add the subcommand `transfer`, which in its turn has two further subcommands `omero transfer pack` and `omero transfer unpack`. Both subcommands (pack and unpack) will use an existing OMERO session created via CLI or prompt the user for parameters to create one.
@@ -22,14 +27,20 @@
 pip install omero-cli-transfer
 ```
 It is possible to do the same thing without `conda` as long as your python/pip version is at least 3.7,
 but that will require locally building a wheel for `zeroc-ice` (which pip does automatically) - it is a
 process that can be anything from "completely seamless and without issues" to "I need to install every 
 dependency ever imagined". Try at your own risk.
 
+If you want optional RO-Crate exports, you can do 
+```
+pip install omero-cli-transfer[rocrate]
+```
+instead.
+
 # Usage
 
 ## `omero transfer pack`
 
 Creates a transfer packet for moving objects between OMERO server instances.
 
 The syntax for specifying objects is: `<object>:<id>` where `<object>` can be `Image`, `Project`, `Dataset`, `Plate` or `Screen`. `Project` is assumed if `<object>:` is omitted. A file path needs to be provided; a tar file with the contents of the packet will be created at the specified path.
@@ -75,7 +86,13 @@
 - `submission.tsv` file has:
 
     - one line per file being submitted, between `Image` files and `FileAnnotation` files;
     - a column indicating whether that file was originally an `Image` or `FileAnnotation`;
     - a "comment" column if any Image has a `CommentAnnotation`;
     - a column per key in a `MapAnnotation` inside the pack, with an empty value for all images but the ones with a `MapAnnotation` with that key; for those images, it has the value for that annotation;
     - a final `original_omero_ids` column listing all OMERO IDs associated to that file in the origin server: for images, that is all `Image` IDs that use that file, and for file annotations that is all `Image` IDs that had that `FileAnnotation` attached to them.
+
+
+### RO-Crate export format
+
+- This requires an optional dependency on `ro-crate-py` that can be installed with `pip install omero-cli-transfer[rocrate]`.
+- Largely due to library limitations, current exports create a flat structure inside a zip file. For each image, `name` and `mimetype` are recorded. A `ro-crate-metadata.json` is added to the zip file.
```

### Comparing `omero-cli-transfer-0.3.3/setup.py` & `omero-cli-transfer-0.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -85,14 +85,17 @@
                  " packet from an OMERO server and importing "
                  "it in a different server. Developed by the "
                  "Research IT team at The Jackson Laboratory."),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TheJacksonLaboratory/omero-cli-transfer",
     install_requires=[
-        'ezomero',
-        'ome-types'
+        'ezomero==1.2.1',
+        'ome-types==0.3.3'
     ],
-    python_requires='>=3.7',
+    extras_require={
+        "rocrate": ["rocrate==0.7.0"],
+    },
+    python_requires='>=3.8',
     cmdclass={'test': PyTest},
     tests_require=['pytest', 'restview', 'mox3'],
 )
```

### Comparing `omero-cli-transfer-0.3.3/src/generate_omero_objects.py` & `omero-cli-transfer-0.4.0/src/generate_omero_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,15 +312,15 @@
     for img in imgs:
         for roiref in img.roi_ref:
             roi = next(filter(lambda x: x.id == roiref.id, rois))
             shapes = create_shapes(roi)
             if roi.union[0].fill_color:
                 fc = roi.union[0].fill_color.as_rgb_tuple()
                 if len(fc) == 3:
-                    fill_color = fc + (0,)
+                    fill_color = fc + (255,)
                 else:
                     alpha = fc[3] * 255
                     fill_color = fc[0:3] + (int(alpha),)
             else:
                 fill_color = (0, 0, 0, 0)
             if roi.union[0].stroke_color:
                 sc = roi.union[0].stroke_color.as_rgb_tuple()
```

### Comparing `omero-cli-transfer-0.3.3/src/generate_xml.py` & `omero-cli-transfer-0.4.0/src/generate_xml.py`

 * *Files 1% similar despite different names*

```diff
@@ -737,14 +737,42 @@
         return
     with open(filepath, 'w') as fp:
         write_lines(datatype, ome, fp, path_id_dict, folder)
         fp.close()
     return
 
 
+def populate_rocrate(datatype: str, ome: OME, filepath: str,
+                     path_id_dict: dict, folder):
+    import importlib.util
+    import mimetypes
+    if (importlib.util.find_spec('rocrate')):
+        from rocrate.rocrate import ROCrate
+    else:
+        raise ImportError("Could not import rocrate library. Make sure to "
+                          "install omero-cli-transfer with the optional "
+                          "[rocrate] addition")
+    if datatype == "Plate" or datatype == "Screen":
+        print("RO-Crate export of Plate/Screen currently unsupported")
+        return
+    rc = ROCrate()
+    files = path_id_dict.items()
+    for id, file in files:
+        img = next(filter(lambda x: x.id == id, ome.images))
+        format = mimetypes.MimeTypes().guess_type(file)[0]
+        if not format:
+            format = "image"
+        rc.add_file(os.path.join(folder, file), properties={
+                        "name": img.name,
+                        "encodingFormat": format
+                    })
+    rc.write_zip(filepath)
+    return
+
+
 def generate_columns(ome: OME, ids: dict) -> List[str]:
     columns = ["filename"]
     if [v for v in ids.values() if v.startswith("file_annotations")]:
         columns.append("data_type")
     for ann in ome.structured_annotations:
         if isinstance(ann, CommentAnnotation) and ("comment" not in columns):
             clean_id = int(ann.id.split(":")[-1])
```

### Comparing `omero-cli-transfer-0.3.3/src/omero_cli_transfer.egg-info/PKG-INFO` & `omero-cli-transfer-0.4.0/src/omero_cli_transfer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 Metadata-Version: 2.1
 Name: omero-cli-transfer
-Version: 0.3.3
+Version: 0.4.0
 Summary: A set of utilities for exporting a transfer packet from an OMERO server and importing it in a different server. Developed by the Research IT team at The Jackson Laboratory.
 Home-page: https://github.com/TheJacksonLaboratory/omero-cli-transfer
 Maintainer: Erick Ratamero
 Maintainer-email: erick.ratamero@jax.org
 License: UNKNOWN
 Description: # omero-cli-transfer
+        
+        
+        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7573592.svg)](https://doi.org/10.5281/zenodo.7573592)
+        
+        
         An OMERO CLI plugin for creating and using transfer packets between OMERO servers.
         
         Transfer packets contain objects and annotations. This project creates a zip file from an object 
         (Project, Dataset, Image, Screen, Plate) containing all original files necessary to create the images 
         in that object, plus an XML file detailing the links between entities, annotations and ROIs thereof.
         
         The CLI plugin add the subcommand `transfer`, which in its turn has two further subcommands `omero transfer pack` and `omero transfer unpack`. Both subcommands (pack and unpack) will use an existing OMERO session created via CLI or prompt the user for parameters to create one.
@@ -30,14 +35,20 @@
         pip install omero-cli-transfer
         ```
         It is possible to do the same thing without `conda` as long as your python/pip version is at least 3.7,
         but that will require locally building a wheel for `zeroc-ice` (which pip does automatically) - it is a
         process that can be anything from "completely seamless and without issues" to "I need to install every 
         dependency ever imagined". Try at your own risk.
         
+        If you want optional RO-Crate exports, you can do 
+        ```
+        pip install omero-cli-transfer[rocrate]
+        ```
+        instead.
+        
         # Usage
         
         ## `omero transfer pack`
         
         Creates a transfer packet for moving objects between OMERO server instances.
         
         The syntax for specifying objects is: `<object>:<id>` where `<object>` can be `Image`, `Project`, `Dataset`, `Plate` or `Screen`. `Project` is assumed if `<object>:` is omitted. A file path needs to be provided; a tar file with the contents of the packet will be created at the specified path.
@@ -84,10 +95,17 @@
         
             - one line per file being submitted, between `Image` files and `FileAnnotation` files;
             - a column indicating whether that file was originally an `Image` or `FileAnnotation`;
             - a "comment" column if any Image has a `CommentAnnotation`;
             - a column per key in a `MapAnnotation` inside the pack, with an empty value for all images but the ones with a `MapAnnotation` with that key; for those images, it has the value for that annotation;
             - a final `original_omero_ids` column listing all OMERO IDs associated to that file in the origin server: for images, that is all `Image` IDs that use that file, and for file annotations that is all `Image` IDs that had that `FileAnnotation` attached to them.
         
+        
+        ### RO-Crate export format
+        
+        - This requires an optional dependency on `ro-crate-py` that can be installed with `pip install omero-cli-transfer[rocrate]`.
+        - Largely due to library limitations, current exports create a flat structure inside a zip file. For each image, `name` and `mimetype` are recorded. A `ro-crate-metadata.json` is added to the zip file.
+        
 Platform: UNKNOWN
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: rocrate
```

### Comparing `omero-cli-transfer-0.3.3/src/omero_cli_transfer.py` & `omero-cli-transfer-0.4.0/src/omero_cli_transfer.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from functools import wraps
 import shutil
 from typing import DefaultDict
 import hashlib
 from zipfile import ZipFile
 from typing import Callable, List, Any, Dict, Union, Optional, Tuple
 
-from generate_xml import populate_xml, populate_tsv
+from generate_xml import populate_xml, populate_tsv, populate_rocrate
 from generate_omero_objects import populate_omero
 
 import ezomero
 from ome_types.model import CommentAnnotation, OME
 from ome_types import from_xml
 from omero.sys import Parameters
 from omero.rtypes import rstring
@@ -147,14 +147,18 @@
                 "--zip", help="Pack into a zip file rather than a tarball",
                 action="store_true")
         pack.add_argument(
                 "--barchive", help="Pack into a file compliant with Bioimage"
                                    " Archive submission standards",
                 action="store_true")
         pack.add_argument(
+                "--rocrate", help="Pack into a file compliant with "
+                                  "RO-Crate standards",
+                action="store_true")
+        pack.add_argument(
             "--metadata",
             choices=['all', 'none', 'img_id', 'timestamp',
                      'software', 'version', 'md5', 'hostname', 'db_id',
                      'orig_user', 'orig_group'], nargs='+',
             help="Metadata field to be added to MapAnnotation"
         )
         pack.add_argument("filepath", type=str, help=file_help)
@@ -272,14 +276,18 @@
 
     def __pack(self, args):
         if isinstance(args.object, Image) or isinstance(args.object, Plate) \
            or isinstance(args.object, Screen):
             if args.barchive:
                 raise ValueError("Single image, plate or screen cannot be "
                                  "packaged for Bioimage Archive")
+        if isinstance(args.object, Plate) or isinstance(args.object, Screen):
+            if args.rocrate:
+                raise ValueError("Single image, plate or screen cannot be "
+                                 "packaged in a RO-Crate")
         if isinstance(args.object, Image):
             src_datatype, src_dataid = "Image", args.object.id
         elif isinstance(args.object, Dataset):
             src_datatype, src_dataid = "Dataset", args.object.id
         elif isinstance(args.object, Project):
             src_datatype, src_dataid = "Project", args.object.id
         elif isinstance(args.object, Plate):
@@ -297,28 +305,36 @@
                              " permissions for current user.")
         print("Populating xml...")
         tar_path = Path(args.filepath)
         folder = str(tar_path) + "_folder"
         os.makedirs(folder, mode=DIR_PERM, exist_ok=True)
         if args.barchive:
             md_fp = str(Path(folder) / "submission.tsv")
+        elif args.rocrate:
+            md_fp = str(Path(folder) / "ro-crate-metadata.json")
         else:
             md_fp = str(Path(folder) / "transfer.xml")
             print(f"Saving metadata at {md_fp}.")
         ome, path_id_dict = populate_xml(src_datatype, src_dataid, md_fp,
                                          self.gateway, self.hostname,
                                          args.barchive, self.metadata)
 
         print("Starting file copy...")
         self._copy_files(path_id_dict, folder, self.gateway)
         if args.barchive:
             print(f"Creating Bioimage Archive TSV at {md_fp}.")
             populate_tsv(src_datatype, ome, md_fp,
                          path_id_dict, folder)
-        self._package_files(os.path.splitext(tar_path)[0], args.zip, folder)
+        if args.rocrate:
+            print(f"Creating RO-Crate metadata at {md_fp}.")
+            populate_rocrate(src_datatype, ome, os.path.splitext(tar_path)[0],
+                             path_id_dict, folder)
+        else:
+            self._package_files(os.path.splitext(tar_path)[0], args.zip,
+                                folder)
         print("Cleaning up...")
         shutil.rmtree(folder)
         return
 
     def __unpack(self, args):
         self.metadata = []
         self._process_metadata(args.metadata)
```

