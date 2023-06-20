# Comparing `tmp/omero-cli-transfer-0.4.0.tar.gz` & `tmp/omero-cli-transfer-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/omero-cli-transfer-0.4.0.tar", last modified: Mon Feb  6 19:30:04 2023, max compression
+gzip compressed data, was "omero-cli-transfer-0.5.0.tar", last modified: Tue Jun 20 16:57:38 2023, max compression
```

## Comparing `omero-cli-transfer-0.4.0.tar` & `omero-cli-transfer-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 19:30:04.000000 omero-cli-transfer-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-02-06 19:30:04.000000 omero-cli-transfer-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-02-06 19:29:54.000000 omero-cli-transfer-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-06 19:30:04.000000 omero-cli-transfer-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-02-06 19:29:54.000000 omero-cli-transfer-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 19:30:04.000000 omero-cli-transfer-0.4.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)    19476 2023-02-06 19:29:54.000000 omero-cli-transfer-0.4.0/src/generate_omero_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    36386 2023-02-06 19:29:54.000000 omero-cli-transfer-0.4.0/src/generate_xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 19:30:04.000000 omero-cli-transfer-0.4.0/src/omero/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 19:30:04.000000 omero-cli-transfer-0.4.0/src/omero/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-02-06 19:29:54.000000 omero-cli-transfer-0.4.0/src/omero/plugins/transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 19:30:04.000000 omero-cli-transfer-0.4.0/src/omero_cli_transfer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-02-06 19:30:04.000000 omero-cli-transfer-0.4.0/src/omero_cli_transfer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-02-06 19:30:04.000000 omero-cli-transfer-0.4.0/src/omero_cli_transfer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 19:30:04.000000 omero-cli-transfer-0.4.0/src/omero_cli_transfer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-06 19:30:04.000000 omero-cli-transfer-0.4.0/src/omero_cli_transfer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-06 19:30:04.000000 omero-cli-transfer-0.4.0/src/omero_cli_transfer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    21769 2023-02-06 19:29:54.000000 omero-cli-transfer-0.4.0/src/omero_cli_transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:57:38.350470 omero-cli-transfer-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-06-20 16:57:36.000000 omero-cli-transfer-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-06-20 16:57:38.350470 omero-cli-transfer-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-06-20 16:57:36.000000 omero-cli-transfer-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 16:57:38.350470 omero-cli-transfer-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-20 16:57:36.000000 omero-cli-transfer-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:57:38.350470 omero-cli-transfer-0.5.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    19883 2023-06-20 16:57:36.000000 omero-cli-transfer-0.5.0/src/generate_omero_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41018 2023-06-20 16:57:36.000000 omero-cli-transfer-0.5.0/src/generate_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:57:38.350470 omero-cli-transfer-0.5.0/src/omero/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:57:38.350470 omero-cli-transfer-0.5.0/src/omero/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-20 16:57:36.000000 omero-cli-transfer-0.5.0/src/omero/plugins/transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:57:38.350470 omero-cli-transfer-0.5.0/src/omero_cli_transfer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-06-20 16:57:38.000000 omero-cli-transfer-0.5.0/src/omero_cli_transfer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-20 16:57:38.000000 omero-cli-transfer-0.5.0/src/omero_cli_transfer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:57:38.000000 omero-cli-transfer-0.5.0/src/omero_cli_transfer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-20 16:57:38.000000 omero-cli-transfer-0.5.0/src/omero_cli_transfer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 16:57:38.000000 omero-cli-transfer-0.5.0/src/omero_cli_transfer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    22865 2023-06-20 16:57:36.000000 omero-cli-transfer-0.5.0/src/omero_cli_transfer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `omero-cli-transfer-0.4.0/PKG-INFO` & `omero-cli-transfer-0.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,111 +1,136 @@
 Metadata-Version: 2.1
 Name: omero-cli-transfer
-Version: 0.4.0
+Version: 0.5.0
 Summary: A set of utilities for exporting a transfer packet from an OMERO server and importing it in a different server. Developed by the Research IT team at The Jackson Laboratory.
 Home-page: https://github.com/TheJacksonLaboratory/omero-cli-transfer
 Maintainer: Erick Ratamero
 Maintainer-email: erick.ratamero@jax.org
 License: UNKNOWN
-Description: # omero-cli-transfer
-        
-        
-        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7573592.svg)](https://doi.org/10.5281/zenodo.7573592)
-        
-        
-        An OMERO CLI plugin for creating and using transfer packets between OMERO servers.
-        
-        Transfer packets contain objects and annotations. This project creates a zip file from an object 
-        (Project, Dataset, Image, Screen, Plate) containing all original files necessary to create the images 
-        in that object, plus an XML file detailing the links between entities, annotations and ROIs thereof.
-        
-        The CLI plugin add the subcommand `transfer`, which in its turn has two further subcommands `omero transfer pack` and `omero transfer unpack`. Both subcommands (pack and unpack) will use an existing OMERO session created via CLI or prompt the user for parameters to create one.
-        
-        # Installation
-        tl;dr: if you have `python>=3.7`, a simple `pip install omero-cli-transfer` _might_ do. We recommend conda, though.
-        
-        `omero-cli-transfer` requires at least Python 3.7. This is due to `ome-types` requiring that as well;
-        this package relies heavily on it, and it is not feasible without it. 
-        
-        Of course, this CAN be an issue, especially given `omero-py` _officially_ only supports Python 3.6. However,
-        it is possible to run `omero-py` in Python 3.7 or newer as well. Our recommended way to do so it using `conda`.
-        With conda installed, you can do
-        ```
-        conda create -n myenv -c conda-force python=3.7 zeroc-ice==3.6.5
-        conda activate myenv
-        pip install omero-cli-transfer
-        ```
-        It is possible to do the same thing without `conda` as long as your python/pip version is at least 3.7,
-        but that will require locally building a wheel for `zeroc-ice` (which pip does automatically) - it is a
-        process that can be anything from "completely seamless and without issues" to "I need to install every 
-        dependency ever imagined". Try at your own risk.
-        
-        If you want optional RO-Crate exports, you can do 
-        ```
-        pip install omero-cli-transfer[rocrate]
-        ```
-        instead.
-        
-        # Usage
-        
-        ## `omero transfer pack`
-        
-        Creates a transfer packet for moving objects between OMERO server instances.
-        
-        The syntax for specifying objects is: `<object>:<id>` where `<object>` can be `Image`, `Project`, `Dataset`, `Plate` or `Screen`. `Project` is assumed if `<object>:` is omitted. A file path needs to be provided; a tar file with the contents of the packet will be created at the specified path.
-        
-        Currently, only MapAnnotations, Tags, FileAnnotations and CommentAnnotations are packaged into the transfer pack. All kinds of ROI (except Masks) should work.
-        
-        Note that, if you are packing a `Plate` or `Screen`, default OMERO settings prevent you from downloading Plates and you will generate an empty pack file if you do so. If you want to generate a pack file from these entities, you will need to set `omero.policy.binary_access` appropriately.
-        
-        `--zip` packs the object into a compressed zip file rather than a tarball.
-        
-        `--barchive` creates a package compliant with Bioimage Archive submission standards - see below for more detail.
-        
-        Examples:
-        ```
-        omero transfer pack Image:123 transfer_pack.tar
-        omero transfer pack --zip Image:123 transfer_pack.zip
-        omero transfer pack Dataset:1111 /home/user/new_folder/new_pack.tar
-        omero transfer pack 999 tarfile.tar  # equivalent to Project:999
-        ```
-        
-        ## `omero transfer unpack`
-        
-        Unpacks an existing transfer packet, imports images/plates as orphans and uses the XML contained in the transfer packet to re-create links, annotations and ROIs.
-        
-        Note that unpack needs to be able to identify the images it imports inequivocally; this can be a problem in case you have other images with the same `clientPath` (i.e. that were imported from the exact same location, including filename) and no annotations created by omero-cli-transfer. The most common case to generate this issue is an unpack that fails after the import step - the lingering images are not annotated correctly and a retry of the same unpack will use the same `clientPath` and cause issues. The best solution is cleaning up after failed unpacks.
-        
-        `--ln_s` forces imports to use the transfer=ln_s option, in-place importing files. Same restrictions of regular in-place imports apply.
-        
-        `--output` allows for specifying an optional output folder where the packet will be unzipped.
-        
-        `--folder` allows the user to point to a previously-unpacked folder rather than a single file.
-        
-        Examples:
-        ```
-        omero transfer unpack transfer_pack.zip
-        omero transfer unpack --output /home/user/optional_folder --ln_s
-        omero transfer unpack --folder /home/user/unpacked_folder/
-        ```
-        
-        ### Bioimage Archive submission contents
-        
-        - Folder structure in the generated zip/tar follows project/dataset structure rather than original ManagedRepository folder structure, and instead of a `transfer.xml` file, a `submission.tsv` file is generated.
-        - `submission.tsv` file has:
-        
-            - one line per file being submitted, between `Image` files and `FileAnnotation` files;
-            - a column indicating whether that file was originally an `Image` or `FileAnnotation`;
-            - a "comment" column if any Image has a `CommentAnnotation`;
-            - a column per key in a `MapAnnotation` inside the pack, with an empty value for all images but the ones with a `MapAnnotation` with that key; for those images, it has the value for that annotation;
-            - a final `original_omero_ids` column listing all OMERO IDs associated to that file in the origin server: for images, that is all `Image` IDs that use that file, and for file annotations that is all `Image` IDs that had that `FileAnnotation` attached to them.
-        
-        
-        ### RO-Crate export format
-        
-        - This requires an optional dependency on `ro-crate-py` that can be installed with `pip install omero-cli-transfer[rocrate]`.
-        - Largely due to library limitations, current exports create a flat structure inside a zip file. For each image, `name` and `mimetype` are recorded. A `ro-crate-metadata.json` is added to the zip file.
-        
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: rocrate
+License-File: LICENSE
+
+# omero-cli-transfer
+
+
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7573591.svg)](https://doi.org/10.5281/zenodo.7573591)
+
+
+An OMERO CLI plugin for creating and using transfer packets between OMERO servers.
+
+Transfer packets contain objects and annotations. This project creates a zip file from an object 
+(Project, Dataset, Image, Screen, Plate) containing all original files necessary to create the images 
+in that object, plus an XML file detailing the links between entities, annotations and ROIs thereof.
+
+The CLI plugin add the subcommand `transfer`, which in its turn has two further subcommands `omero transfer pack` and `omero transfer unpack`. Both subcommands (pack and unpack) will use an existing OMERO session created via CLI or prompt the user for parameters to create one.
+
+# Installation
+tl;dr: if you have `python>=3.7`, a simple `pip install omero-cli-transfer` _might_ do. We recommend conda, though.
+
+`omero-cli-transfer` requires at least Python 3.7. This is due to `ome-types` requiring that as well;
+this package relies heavily on it, and it is not feasible without it. 
+
+Of course, this CAN be an issue, especially given `omero-py` _officially_ only supports Python 3.6. However,
+it is possible to run `omero-py` in Python 3.7 or newer as well. Our recommended way to do so it using `conda`.
+With conda installed, you can do
+```
+conda create -n myenv -c conda-force python=3.7 zeroc-ice==3.6.5
+conda activate myenv
+pip install omero-cli-transfer
+```
+It is possible to do the same thing without `conda` as long as your python/pip version is at least 3.7,
+but that will require locally building a wheel for `zeroc-ice` (which pip does automatically) - it is a
+process that can be anything from "completely seamless and without issues" to "I need to install every 
+dependency ever imagined". Try at your own risk.
+
+If you want optional RO-Crate exports, you can do 
+```
+pip install omero-cli-transfer[rocrate]
+```
+instead.
+
+# Usage
+
+## `omero transfer pack`
+
+Creates a transfer packet for moving objects between OMERO server instances.
+
+The syntax for specifying objects is: `<object>:<id>` where `<object>` can be `Image`, `Project`, `Dataset`, `Plate` or `Screen`. `Project` is assumed if `<object>:` is omitted. A file path needs to be provided; a tar file with the contents of the packet will be created at the specified path.
+
+Currently, only MapAnnotations, Tags, FileAnnotations and CommentAnnotations are packaged into the transfer pack. All kinds of ROI (except Masks) should work.
+
+Note that, if you are packing a `Plate` or `Screen`, default OMERO settings prevent you from downloading Plates and you will generate an empty pack file if you do so. If you want to generate a pack file from these entities, you will need to set `omero.policy.binary_access` appropriately.
+
+`--zip` packs the object into a compressed zip file rather than a tarball.
+
+`--barchive` creates a package compliant with Bioimage Archive submission standards - see below for more detail.
+
+Examples:
+```
+omero transfer pack Image:123 transfer_pack.tar
+omero transfer pack --zip Image:123 transfer_pack.zip
+omero transfer pack Dataset:1111 /home/user/new_folder/new_pack.tar
+omero transfer pack 999 tarfile.tar  # equivalent to Project:999
+```
+
+## `omero transfer unpack`
+
+Unpacks an existing transfer packet, imports images/plates as orphans and uses the XML contained in the transfer packet to re-create links, annotations and ROIs.
+
+Note that unpack needs to be able to identify the images it imports inequivocally; this can be a problem in case you have other images with the same `clientPath` (i.e. that were imported from the exact same location, including filename) and no annotations created by omero-cli-transfer. The most common case to generate this issue is an unpack that fails after the import step - the lingering images are not annotated correctly and a retry of the same unpack will use the same `clientPath` and cause issues. The best solution is cleaning up after failed unpacks.
+
+`--ln_s` forces imports to use the transfer=ln_s option, in-place importing files. Same restrictions of regular in-place imports apply.
+
+`--output` allows for specifying an optional output folder where the packet will be unzipped.
+
+`--folder` allows the user to point to a previously-unpacked folder rather than a single file.
+
+Examples:
+```
+omero transfer unpack transfer_pack.zip
+omero transfer unpack --output /home/user/optional_folder --ln_s
+omero transfer unpack --folder /home/user/unpacked_folder/
+```
+
+## `omero transfer prepare`
+
+Creates an XML from a folder with images.
+
+Creates an XML file appropriate for usage with `omero transfer unpack` from
+a folder that contains image files, rather than a source OMERO server. This
+is intended as a first step on a bulk-import workflow, followed by using
+`omero transfer unpack` to complete an import.
+
+Examples:
+```
+omero transfer prepare /home/user/folder_with_files
+```
+
+NOTE: please refer to optional requirement instructions below and consider that this feature is experimental!
+
+### Bioimage Archive submission contents
+
+- Folder structure in the generated zip/tar follows project/dataset structure rather than original ManagedRepository folder structure, and instead of a `transfer.xml` file, a `submission.tsv` file is generated.
+- `submission.tsv` file has:
+
+    - one line per file being submitted, between `Image` files and `FileAnnotation` files;
+    - a column indicating whether that file was originally an `Image` or `FileAnnotation`;
+    - a "comment" column if any Image has a `CommentAnnotation`;
+    - a column per key in a `MapAnnotation` inside the pack, with an empty value for all images but the ones with a `MapAnnotation` with that key; for those images, it has the value for that annotation;
+    - a final `original_omero_ids` column listing all OMERO IDs associated to that file in the origin server: for images, that is all `Image` IDs that use that file, and for file annotations that is all `Image` IDs that had that `FileAnnotation` attached to them.
+
+
+### RO-Crate export format
+
+- This requires an optional dependency on `ro-crate-py` that can be installed with `pip install omero-cli-transfer[rocrate]`.
+- Largely due to library limitations, current exports create a flat structure inside a zip file. For each image, `name` and `mimetype` are recorded. A `ro-crate-metadata.json` is added to the zip file.
+
+
+### `omero transfer prepare` optional requirements
+
+- `prepare` requires [bftools](https://bio-formats.readthedocs.io/en/stable/users/comlinetools/index.html) to work (in particular, we need to be able to run `showinf`). The easiest way to install this is by using conda; A simple `conda install -c bioconda bftools` on your conda environment should suffice.
+- Note that this is a Java application. The conda package will install a JDK for you if necessary, but if you're installing it for yourself you'll need to make sure Java is available.
+- This tool runs `showinf` in a subprocess and needs to be able to parse the output. This can be problematic if your `stdout` is not set to UTF-8; it can mess up special characters is e.g. measurement units and lead to XML validation errors. In addition to that, Java itself might output data in non-UTF-8 encodings, in which case it might be necessary to set `JAVA_TOOL_OPTIONS=-Dfile.encoding=UTF8`.
+
```

### Comparing `omero-cli-transfer-0.4.0/README.md` & `omero-cli-transfer-0.5.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # omero-cli-transfer
 
 
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7573592.svg)](https://doi.org/10.5281/zenodo.7573592)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7573591.svg)](https://doi.org/10.5281/zenodo.7573591)
 
 
 An OMERO CLI plugin for creating and using transfer packets between OMERO servers.
 
 Transfer packets contain objects and annotations. This project creates a zip file from an object 
 (Project, Dataset, Image, Screen, Plate) containing all original files necessary to create the images 
 in that object, plus an XML file detailing the links between entities, annotations and ROIs thereof.
@@ -76,14 +76,30 @@
 Examples:
 ```
 omero transfer unpack transfer_pack.zip
 omero transfer unpack --output /home/user/optional_folder --ln_s
 omero transfer unpack --folder /home/user/unpacked_folder/
 ```
 
+## `omero transfer prepare`
+
+Creates an XML from a folder with images.
+
+Creates an XML file appropriate for usage with `omero transfer unpack` from
+a folder that contains image files, rather than a source OMERO server. This
+is intended as a first step on a bulk-import workflow, followed by using
+`omero transfer unpack` to complete an import.
+
+Examples:
+```
+omero transfer prepare /home/user/folder_with_files
+```
+
+NOTE: please refer to optional requirement instructions below and consider that this feature is experimental!
+
 ### Bioimage Archive submission contents
 
 - Folder structure in the generated zip/tar follows project/dataset structure rather than original ManagedRepository folder structure, and instead of a `transfer.xml` file, a `submission.tsv` file is generated.
 - `submission.tsv` file has:
 
     - one line per file being submitted, between `Image` files and `FileAnnotation` files;
     - a column indicating whether that file was originally an `Image` or `FileAnnotation`;
@@ -92,7 +108,14 @@
     - a final `original_omero_ids` column listing all OMERO IDs associated to that file in the origin server: for images, that is all `Image` IDs that use that file, and for file annotations that is all `Image` IDs that had that `FileAnnotation` attached to them.
 
 
 ### RO-Crate export format
 
 - This requires an optional dependency on `ro-crate-py` that can be installed with `pip install omero-cli-transfer[rocrate]`.
 - Largely due to library limitations, current exports create a flat structure inside a zip file. For each image, `name` and `mimetype` are recorded. A `ro-crate-metadata.json` is added to the zip file.
+
+
+### `omero transfer prepare` optional requirements
+
+- `prepare` requires [bftools](https://bio-formats.readthedocs.io/en/stable/users/comlinetools/index.html) to work (in particular, we need to be able to run `showinf`). The easiest way to install this is by using conda; A simple `conda install -c bioconda bftools` on your conda environment should suffice.
+- Note that this is a Java application. The conda package will install a JDK for you if necessary, but if you're installing it for yourself you'll need to make sure Java is available.
+- This tool runs `showinf` in a subprocess and needs to be able to parse the output. This can be problematic if your `stdout` is not set to UTF-8; it can mess up special characters is e.g. measurement units and lead to XML validation errors. In addition to that, Java itself might output data in non-UTF-8 encodings, in which case it might be necessary to set `JAVA_TOOL_OPTIONS=-Dfile.encoding=UTF8`.
```

### Comparing `omero-cli-transfer-0.4.0/setup.py` & `omero-cli-transfer-0.5.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+# Copyright (C) 2022 The Jackson Laboratory
+# Copyright (C) 2015-2018 University of Dundee & Open Microscopy Environment.
+# All rights reserved.
+#
+# Use is subject to license terms supplied in LICENSE.
+
 import os
 import sys
 from setuptools import setup
 from setuptools.command.test import test as test_command
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
@@ -74,27 +80,27 @@
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     packages=['', 'omero.plugins'],
     package_dir={"": "src"},
     name="omero-cli-transfer",
-    version=os.environ.get('VERSION', '0.0.0'),
+    version='0.5.0',
     maintainer="Erick Ratamero",
     maintainer_email="erick.ratamero@jax.org",
     description=("A set of utilities for exporting a transfer"
                  " packet from an OMERO server and importing "
                  "it in a different server. Developed by the "
                  "Research IT team at The Jackson Laboratory."),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TheJacksonLaboratory/omero-cli-transfer",
     install_requires=[
-        'ezomero==1.2.1',
-        'ome-types==0.3.3'
+        'ezomero==2.0.0',
+        'ome-types==0.3.4'
     ],
     extras_require={
         "rocrate": ["rocrate==0.7.0"],
     },
     python_requires='>=3.8',
     cmdclass={'test': PyTest},
     tests_require=['pytest', 'restview', 'mox3'],
```

### Comparing `omero-cli-transfer-0.4.0/src/generate_omero_objects.py` & `omero-cli-transfer-0.5.0/src/generate_omero_objects.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# Copyright (C) 2022 The Jackson Laboratory
+# All rights reserved.
+#
+# Use is subject to license terms supplied in LICENSE.
+
 import ezomero
 from typing import List, Tuple
 from omero.model import DatasetI, IObject, PlateI, WellI, WellSampleI, ImageI
 from omero.gateway import DatasetWrapper
 from ome_types.model import TagAnnotation, MapAnnotation, FileAnnotation, ROI
 from ome_types.model import CommentAnnotation, LongAnnotation, Annotation
 from ome_types.model import Line, Point, Rectangle, Ellipse, Polygon, Shape
@@ -241,17 +246,40 @@
         return False
     return True
 
 
 def create_shapes(roi: ROI) -> List[Shape]:
     shapes = []
     for shape in roi.union:
+        if shape.fill_color:
+            fc = shape.fill_color.as_rgb_tuple()
+            if len(fc) == 3:
+                fill_color = fc + (255,)
+            else:
+                alpha = fc[3] * 255
+                fill_color = fc[0:3] + (int(alpha),)
+        else:
+            fill_color = (0, 0, 0, 0)
+        if shape.stroke_color:
+            sc = shape.stroke_color.as_rgb_tuple()
+            if len(sc) == 3:
+                stroke_color = sc + (255,)
+            else:
+                stroke_color = sc
+        else:
+            stroke_color = (255, 255, 255, 255)
+        if shape.stroke_width:
+            stroke_width = int(shape.stroke_width)
+        else:
+            stroke_width = 1
         if isinstance(shape, Point):
             sh = rois.Point(shape.x, shape.y, z=shape.the_z, c=shape.the_c,
-                            t=shape.the_t, label=shape.text)
+                            t=shape.the_t, label=shape.text,
+                            fill_color=fill_color, stroke_color=stroke_color,
+                            stroke_width=stroke_width)
         elif isinstance(shape, Line):
             if shape.marker_start == Marker.ARROW:
                 mk_start = "Arrow"
             else:
                 mk_start = str(shape.marker_start)
             if shape.marker_end == Marker.ARROW:
                 mk_end = "Arrow"
@@ -309,40 +337,17 @@
 
 def create_rois(rois: List[ROI], imgs: List[Image], img_map: dict,
                 conn: BlitzGateway):
     for img in imgs:
         for roiref in img.roi_ref:
             roi = next(filter(lambda x: x.id == roiref.id, rois))
             shapes = create_shapes(roi)
-            if roi.union[0].fill_color:
-                fc = roi.union[0].fill_color.as_rgb_tuple()
-                if len(fc) == 3:
-                    fill_color = fc + (255,)
-                else:
-                    alpha = fc[3] * 255
-                    fill_color = fc[0:3] + (int(alpha),)
-            else:
-                fill_color = (0, 0, 0, 0)
-            if roi.union[0].stroke_color:
-                sc = roi.union[0].stroke_color.as_rgb_tuple()
-                if len(sc) == 3:
-                    stroke_color = sc + (255,)
-                else:
-                    stroke_color = sc
-            else:
-                stroke_color = (255, 255, 255, 255)
-            if roi.union[0].stroke_width:
-                stroke_width = int(roi.union[0].stroke_width)
-            else:
-                stroke_width = 1
             img_id_dest = img_map[img.id]
             ezomero.post_roi(conn, img_id_dest, shapes, name=roi.name,
-                             description=roi.description,
-                             fill_color=fill_color, stroke_color=stroke_color,
-                             stroke_width=stroke_width)
+                             description=roi.description)
     return
 
 
 def link_datasets(ome: OME, proj_map: dict, ds_map: dict, conn: BlitzGateway):
     for proj in ome.projects:
         proj_id = proj_map[proj.id]
         ds_ids = []
@@ -459,21 +464,34 @@
             im_obj.setName(img.name)
             im_obj.save()
         except KeyError:
             print(f"Image corresponding to {img.id} not found. Skipping.")
     return
 
 
+def rename_plates(pls: List[Plate], pl_map: dict, conn: BlitzGateway):
+    for pl in pls:
+        try:
+            pl_id = pl_map[pl.id]
+            pl_obj = conn.getObject("Plate", pl_id)
+            pl_obj.setName(pl.name)
+            pl_obj.save()
+        except KeyError:
+            print(f"Plate corresponding to {pl.id} not found. Skipping.")
+    return
+
+
 def populate_omero(ome: OME, img_map: dict, conn: BlitzGateway, hash: str,
                    folder: str, metadata: List[str]):
+    plate_map, ome = create_plate_map(ome, img_map, conn)
     rename_images(ome.images, img_map, conn)
+    rename_plates(ome.plates, plate_map, conn)
     proj_map = create_projects(ome.projects, conn)
     ds_map = create_datasets(ome.datasets, conn)
     screen_map = create_screens(ome.screens, conn)
-    plate_map, ome = create_plate_map(ome, img_map, conn)
     ann_map = create_annotations(ome.structured_annotations, conn,
                                  hash, folder, metadata)
     create_rois(ome.rois, ome.images, img_map, conn)
     link_plates(ome, screen_map, plate_map, conn)
     link_datasets(ome, proj_map, ds_map, conn)
     link_images(ome, ds_map, img_map, conn)
     link_annotations(ome, proj_map, ds_map, img_map, ann_map,
```

### Comparing `omero-cli-transfer-0.4.0/src/generate_xml.py` & `omero-cli-transfer-0.5.0/src/generate_xml.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-from ome_types import to_xml, OME
+# Copyright (C) 2022 The Jackson Laboratory
+# All rights reserved.
+#
+# Use is subject to license terms supplied in LICENSE.
+
+from ome_types import to_xml, OME, from_xml
 from ome_types.model import Project, ProjectRef
 from ome_types.model import Screen
 from ome_types.model.screen import PlateRef
 from ome_types.model import Well, WellSample
 from ome_types.model import Plate
 from ome_types.model import Dataset, DatasetRef
 from ome_types.model import Image, ImageRef, Pixels
@@ -15,25 +20,28 @@
 from ome_types.model.map import M
 from omero.gateway import BlitzGateway
 from omero.model import TagAnnotationI, MapAnnotationI, FileAnnotationI
 from omero.model import CommentAnnotationI, LongAnnotationI, Fileset
 from omero.model import PointI, LineI, RectangleI, EllipseI, PolygonI
 from omero.model import PolylineI, LabelI, ImageI, RoiI, IObject
 from omero.model import DatasetI, ProjectI, ScreenI, PlateI, WellI, Annotation
+from omero.cli import CLI
 from typing import Tuple, List, Optional, Union, Any, Dict, TextIO
+from subprocess import PIPE, DEVNULL
 from os import PathLike
 import pkg_resources
 import ezomero
 import os
 import csv
 import base64
 from uuid import uuid4
 from datetime import datetime
 from pathlib import Path
 import shutil
+import copy
 
 
 def create_proj_and_ref(**kwargs) -> Tuple[Project, ProjectRef]:
     proj = Project(**kwargs)
     proj_ref = ProjectRef(id=proj.id)
     return proj, proj_ref
 
@@ -451,14 +459,130 @@
             mmap.append(M(k=_key, value=''))
     kv, ref = create_kv_and_ref(id=id,
                                 namespace=ns,
                                 value=Map(m=mmap))
     return kv, ref
 
 
+def create_objects(folder):
+    img_files = []
+    for path, subdirs, files in os.walk(folder):
+        for f in files:
+            img_files.append(os.path.abspath(os.path.join(path, f)))
+    targets = copy.deepcopy(img_files)
+    cli = CLI()
+    cli.loadplugins()
+    for img in img_files:
+        if img not in (targets):
+            continue
+        cmd = ["omero", 'import', '-f', img, "\n"]
+        res = cli.popen(cmd, stdout=PIPE, stderr=DEVNULL)
+        std = res.communicate()
+        files = parse_files_import(std[0].decode('UTF-8'))
+        if len(files) > 1:
+            for f in files:
+                targets.remove(f)
+            targets.append(img)
+        if len(files) == 0:
+            targets.remove(img)
+    images = []
+    plates = []
+    annotations = []
+    counter_imgs = 1
+    counter_pls = 1
+    for target in targets:
+        print(f"Processing file {target}\n")
+        res = run_showinf(target, cli)
+        imgs, pls, anns = parse_showinf(res,
+                                        counter_imgs, counter_pls, target)
+        images.extend(imgs)
+        counter_imgs = counter_imgs + len(imgs)
+        plates.extend(pls)
+        counter_pls = counter_pls + len(pls)
+        annotations.extend(anns)
+    return images, plates, annotations
+
+
+def run_showinf(target, cli):
+    cmd = ["showinf", target, '-nopix', '-omexml-only',
+           '-no-sas', '-noflat']
+    res = cli.popen(cmd, stdout=PIPE, stderr=DEVNULL)
+    std = res.communicate()
+    return std[0].decode('UTF-8')
+
+
+def parse_files_import(text):
+    lines = text.split("\n")
+    targets = [line for line in lines if not line.startswith("#")
+               and len(line) > 0]
+    return targets
+
+
+def parse_showinf(text, counter_imgs, counter_plates, target):
+    ome = from_xml(text, parser='xmlschema')
+    images = []
+    plates = []
+    annotations = []
+    img_id = counter_imgs
+    pl_id = counter_plates
+    img_ref = {}
+    for image in ome.images:
+        img_id_str = f"Image:{str(img_id)}"
+        img_ref[image.id] = img_id_str
+        pix = create_empty_pixels(image, img_id)
+        if len(ome.images) > 1:  # differentiating names
+            filename = Path(target).name
+            img = Image(id=img_id_str, name=filename + " [" + image.name + "]",
+                        pixels=pix)
+        else:
+            img = Image(id=img_id_str, name=image.name, pixels=pix)
+        img_id += 1
+        uid = (-1) * uuid4().int
+        an = CommentAnnotation(id=uid,
+                               namespace=img_id_str,
+                               value=target
+                               )
+        annotations.append(an)
+        anref = AnnotationRef(id=an.id)
+        img.annotation_ref.append(anref)
+        images.append(img)
+    for plate in ome.plates:
+        pl_id_str = f"Plate:{str(pl_id)}"
+        pl = Plate(id=pl_id_str, name=plate.name, wells=plate.wells)
+        for w in pl.wells:
+            for ws in w.well_samples:
+                ws.image_ref.id = img_ref[ws.image_ref.id]
+        pl_id += 1
+        uid = (-1) * uuid4().int
+        an = CommentAnnotation(id=uid,
+                               namespace=pl_id_str,
+                               value=target
+                               )
+        annotations.append(an)
+        anref = AnnotationRef(id=an.id)
+        pl.annotation_ref.append(anref)
+        plates.append(pl)
+    return images, plates, annotations
+
+
+def create_empty_pixels(image, id):
+    pix_id = f"Pixels:{str(id)}"
+    pixels = Pixels(
+        id=pix_id,
+        dimension_order=image.pixels.dimension_order,
+        size_c=image.pixels.size_c,
+        size_t=image.pixels.size_t,
+        size_x=image.pixels.size_x,
+        size_y=image.pixels.size_y,
+        size_z=image.pixels.size_z,
+        type=image.pixels.type,
+        metadata_only=True)
+    return pixels
+
+
 def populate_roi(obj: RoiI, roi_obj: IObject, ome: OME, conn: BlitzGateway
                  ) -> Union[ROIRef, None]:
     id = obj.getId().getValue()
     name = obj.getName()
     if name is not None:
         name = name.getValue()
     desc = obj.getDescription()
@@ -726,14 +850,32 @@
         with open(filepath, 'w') as fp:
             print(to_xml(ome), file=fp)
             fp.close()
     path_id_dict = list_file_ids(ome)
     return ome, path_id_dict
 
 
+def populate_xml_folder(folder: str, conn: BlitzGateway, session: str
+                        ) -> Tuple[OME, dict]:
+    ome = OME()
+    images, plates, annotations = create_objects(folder)
+    ome.images = images
+    ome.plates = plates
+    ome.structured_annotations = annotations
+    filepath = str(Path(folder) / "transfer.xml")
+    if Path(folder).exists():
+        with open(filepath, 'w') as fp:
+            print(to_xml(ome), file=fp)
+            fp.close()
+    else:
+        raise ValueError("Folder cannot be found!")
+    path_id_dict = list_file_ids(ome)
+    return ome, path_id_dict
+
+
 def populate_tsv(datatype: str, ome: OME, filepath: str,
                  path_id_dict: dict, folder: str):
     if datatype == "Plate" or datatype == "Screen":
         print("Bioimage Archive export of Plate/Screen currently unsupported")
         return
     with open(filepath, 'w') as fp:
         write_lines(datatype, ome, fp, path_id_dict, folder)
```

### Comparing `omero-cli-transfer-0.4.0/src/omero_cli_transfer.egg-info/PKG-INFO` & `omero-cli-transfer-0.5.0/src/omero_cli_transfer.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,111 +1,136 @@
 Metadata-Version: 2.1
 Name: omero-cli-transfer
-Version: 0.4.0
+Version: 0.5.0
 Summary: A set of utilities for exporting a transfer packet from an OMERO server and importing it in a different server. Developed by the Research IT team at The Jackson Laboratory.
 Home-page: https://github.com/TheJacksonLaboratory/omero-cli-transfer
 Maintainer: Erick Ratamero
 Maintainer-email: erick.ratamero@jax.org
 License: UNKNOWN
-Description: # omero-cli-transfer
-        
-        
-        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7573592.svg)](https://doi.org/10.5281/zenodo.7573592)
-        
-        
-        An OMERO CLI plugin for creating and using transfer packets between OMERO servers.
-        
-        Transfer packets contain objects and annotations. This project creates a zip file from an object 
-        (Project, Dataset, Image, Screen, Plate) containing all original files necessary to create the images 
-        in that object, plus an XML file detailing the links between entities, annotations and ROIs thereof.
-        
-        The CLI plugin add the subcommand `transfer`, which in its turn has two further subcommands `omero transfer pack` and `omero transfer unpack`. Both subcommands (pack and unpack) will use an existing OMERO session created via CLI or prompt the user for parameters to create one.
-        
-        # Installation
-        tl;dr: if you have `python>=3.7`, a simple `pip install omero-cli-transfer` _might_ do. We recommend conda, though.
-        
-        `omero-cli-transfer` requires at least Python 3.7. This is due to `ome-types` requiring that as well;
-        this package relies heavily on it, and it is not feasible without it. 
-        
-        Of course, this CAN be an issue, especially given `omero-py` _officially_ only supports Python 3.6. However,
-        it is possible to run `omero-py` in Python 3.7 or newer as well. Our recommended way to do so it using `conda`.
-        With conda installed, you can do
-        ```
-        conda create -n myenv -c conda-force python=3.7 zeroc-ice==3.6.5
-        conda activate myenv
-        pip install omero-cli-transfer
-        ```
-        It is possible to do the same thing without `conda` as long as your python/pip version is at least 3.7,
-        but that will require locally building a wheel for `zeroc-ice` (which pip does automatically) - it is a
-        process that can be anything from "completely seamless and without issues" to "I need to install every 
-        dependency ever imagined". Try at your own risk.
-        
-        If you want optional RO-Crate exports, you can do 
-        ```
-        pip install omero-cli-transfer[rocrate]
-        ```
-        instead.
-        
-        # Usage
-        
-        ## `omero transfer pack`
-        
-        Creates a transfer packet for moving objects between OMERO server instances.
-        
-        The syntax for specifying objects is: `<object>:<id>` where `<object>` can be `Image`, `Project`, `Dataset`, `Plate` or `Screen`. `Project` is assumed if `<object>:` is omitted. A file path needs to be provided; a tar file with the contents of the packet will be created at the specified path.
-        
-        Currently, only MapAnnotations, Tags, FileAnnotations and CommentAnnotations are packaged into the transfer pack. All kinds of ROI (except Masks) should work.
-        
-        Note that, if you are packing a `Plate` or `Screen`, default OMERO settings prevent you from downloading Plates and you will generate an empty pack file if you do so. If you want to generate a pack file from these entities, you will need to set `omero.policy.binary_access` appropriately.
-        
-        `--zip` packs the object into a compressed zip file rather than a tarball.
-        
-        `--barchive` creates a package compliant with Bioimage Archive submission standards - see below for more detail.
-        
-        Examples:
-        ```
-        omero transfer pack Image:123 transfer_pack.tar
-        omero transfer pack --zip Image:123 transfer_pack.zip
-        omero transfer pack Dataset:1111 /home/user/new_folder/new_pack.tar
-        omero transfer pack 999 tarfile.tar  # equivalent to Project:999
-        ```
-        
-        ## `omero transfer unpack`
-        
-        Unpacks an existing transfer packet, imports images/plates as orphans and uses the XML contained in the transfer packet to re-create links, annotations and ROIs.
-        
-        Note that unpack needs to be able to identify the images it imports inequivocally; this can be a problem in case you have other images with the same `clientPath` (i.e. that were imported from the exact same location, including filename) and no annotations created by omero-cli-transfer. The most common case to generate this issue is an unpack that fails after the import step - the lingering images are not annotated correctly and a retry of the same unpack will use the same `clientPath` and cause issues. The best solution is cleaning up after failed unpacks.
-        
-        `--ln_s` forces imports to use the transfer=ln_s option, in-place importing files. Same restrictions of regular in-place imports apply.
-        
-        `--output` allows for specifying an optional output folder where the packet will be unzipped.
-        
-        `--folder` allows the user to point to a previously-unpacked folder rather than a single file.
-        
-        Examples:
-        ```
-        omero transfer unpack transfer_pack.zip
-        omero transfer unpack --output /home/user/optional_folder --ln_s
-        omero transfer unpack --folder /home/user/unpacked_folder/
-        ```
-        
-        ### Bioimage Archive submission contents
-        
-        - Folder structure in the generated zip/tar follows project/dataset structure rather than original ManagedRepository folder structure, and instead of a `transfer.xml` file, a `submission.tsv` file is generated.
-        - `submission.tsv` file has:
-        
-            - one line per file being submitted, between `Image` files and `FileAnnotation` files;
-            - a column indicating whether that file was originally an `Image` or `FileAnnotation`;
-            - a "comment" column if any Image has a `CommentAnnotation`;
-            - a column per key in a `MapAnnotation` inside the pack, with an empty value for all images but the ones with a `MapAnnotation` with that key; for those images, it has the value for that annotation;
-            - a final `original_omero_ids` column listing all OMERO IDs associated to that file in the origin server: for images, that is all `Image` IDs that use that file, and for file annotations that is all `Image` IDs that had that `FileAnnotation` attached to them.
-        
-        
-        ### RO-Crate export format
-        
-        - This requires an optional dependency on `ro-crate-py` that can be installed with `pip install omero-cli-transfer[rocrate]`.
-        - Largely due to library limitations, current exports create a flat structure inside a zip file. For each image, `name` and `mimetype` are recorded. A `ro-crate-metadata.json` is added to the zip file.
-        
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: rocrate
+License-File: LICENSE
+
+# omero-cli-transfer
+
+
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7573591.svg)](https://doi.org/10.5281/zenodo.7573591)
+
+
+An OMERO CLI plugin for creating and using transfer packets between OMERO servers.
+
+Transfer packets contain objects and annotations. This project creates a zip file from an object 
+(Project, Dataset, Image, Screen, Plate) containing all original files necessary to create the images 
+in that object, plus an XML file detailing the links between entities, annotations and ROIs thereof.
+
+The CLI plugin add the subcommand `transfer`, which in its turn has two further subcommands `omero transfer pack` and `omero transfer unpack`. Both subcommands (pack and unpack) will use an existing OMERO session created via CLI or prompt the user for parameters to create one.
+
+# Installation
+tl;dr: if you have `python>=3.7`, a simple `pip install omero-cli-transfer` _might_ do. We recommend conda, though.
+
+`omero-cli-transfer` requires at least Python 3.7. This is due to `ome-types` requiring that as well;
+this package relies heavily on it, and it is not feasible without it. 
+
+Of course, this CAN be an issue, especially given `omero-py` _officially_ only supports Python 3.6. However,
+it is possible to run `omero-py` in Python 3.7 or newer as well. Our recommended way to do so it using `conda`.
+With conda installed, you can do
+```
+conda create -n myenv -c conda-force python=3.7 zeroc-ice==3.6.5
+conda activate myenv
+pip install omero-cli-transfer
+```
+It is possible to do the same thing without `conda` as long as your python/pip version is at least 3.7,
+but that will require locally building a wheel for `zeroc-ice` (which pip does automatically) - it is a
+process that can be anything from "completely seamless and without issues" to "I need to install every 
+dependency ever imagined". Try at your own risk.
+
+If you want optional RO-Crate exports, you can do 
+```
+pip install omero-cli-transfer[rocrate]
+```
+instead.
+
+# Usage
+
+## `omero transfer pack`
+
+Creates a transfer packet for moving objects between OMERO server instances.
+
+The syntax for specifying objects is: `<object>:<id>` where `<object>` can be `Image`, `Project`, `Dataset`, `Plate` or `Screen`. `Project` is assumed if `<object>:` is omitted. A file path needs to be provided; a tar file with the contents of the packet will be created at the specified path.
+
+Currently, only MapAnnotations, Tags, FileAnnotations and CommentAnnotations are packaged into the transfer pack. All kinds of ROI (except Masks) should work.
+
+Note that, if you are packing a `Plate` or `Screen`, default OMERO settings prevent you from downloading Plates and you will generate an empty pack file if you do so. If you want to generate a pack file from these entities, you will need to set `omero.policy.binary_access` appropriately.
+
+`--zip` packs the object into a compressed zip file rather than a tarball.
+
+`--barchive` creates a package compliant with Bioimage Archive submission standards - see below for more detail.
+
+Examples:
+```
+omero transfer pack Image:123 transfer_pack.tar
+omero transfer pack --zip Image:123 transfer_pack.zip
+omero transfer pack Dataset:1111 /home/user/new_folder/new_pack.tar
+omero transfer pack 999 tarfile.tar  # equivalent to Project:999
+```
+
+## `omero transfer unpack`
+
+Unpacks an existing transfer packet, imports images/plates as orphans and uses the XML contained in the transfer packet to re-create links, annotations and ROIs.
+
+Note that unpack needs to be able to identify the images it imports inequivocally; this can be a problem in case you have other images with the same `clientPath` (i.e. that were imported from the exact same location, including filename) and no annotations created by omero-cli-transfer. The most common case to generate this issue is an unpack that fails after the import step - the lingering images are not annotated correctly and a retry of the same unpack will use the same `clientPath` and cause issues. The best solution is cleaning up after failed unpacks.
+
+`--ln_s` forces imports to use the transfer=ln_s option, in-place importing files. Same restrictions of regular in-place imports apply.
+
+`--output` allows for specifying an optional output folder where the packet will be unzipped.
+
+`--folder` allows the user to point to a previously-unpacked folder rather than a single file.
+
+Examples:
+```
+omero transfer unpack transfer_pack.zip
+omero transfer unpack --output /home/user/optional_folder --ln_s
+omero transfer unpack --folder /home/user/unpacked_folder/
+```
+
+## `omero transfer prepare`
+
+Creates an XML from a folder with images.
+
+Creates an XML file appropriate for usage with `omero transfer unpack` from
+a folder that contains image files, rather than a source OMERO server. This
+is intended as a first step on a bulk-import workflow, followed by using
+`omero transfer unpack` to complete an import.
+
+Examples:
+```
+omero transfer prepare /home/user/folder_with_files
+```
+
+NOTE: please refer to optional requirement instructions below and consider that this feature is experimental!
+
+### Bioimage Archive submission contents
+
+- Folder structure in the generated zip/tar follows project/dataset structure rather than original ManagedRepository folder structure, and instead of a `transfer.xml` file, a `submission.tsv` file is generated.
+- `submission.tsv` file has:
+
+    - one line per file being submitted, between `Image` files and `FileAnnotation` files;
+    - a column indicating whether that file was originally an `Image` or `FileAnnotation`;
+    - a "comment" column if any Image has a `CommentAnnotation`;
+    - a column per key in a `MapAnnotation` inside the pack, with an empty value for all images but the ones with a `MapAnnotation` with that key; for those images, it has the value for that annotation;
+    - a final `original_omero_ids` column listing all OMERO IDs associated to that file in the origin server: for images, that is all `Image` IDs that use that file, and for file annotations that is all `Image` IDs that had that `FileAnnotation` attached to them.
+
+
+### RO-Crate export format
+
+- This requires an optional dependency on `ro-crate-py` that can be installed with `pip install omero-cli-transfer[rocrate]`.
+- Largely due to library limitations, current exports create a flat structure inside a zip file. For each image, `name` and `mimetype` are recorded. A `ro-crate-metadata.json` is added to the zip file.
+
+
+### `omero transfer prepare` optional requirements
+
+- `prepare` requires [bftools](https://bio-formats.readthedocs.io/en/stable/users/comlinetools/index.html) to work (in particular, we need to be able to run `showinf`). The easiest way to install this is by using conda; A simple `conda install -c bioconda bftools` on your conda environment should suffice.
+- Note that this is a Java application. The conda package will install a JDK for you if necessary, but if you're installing it for yourself you'll need to make sure Java is available.
+- This tool runs `showinf` in a subprocess and needs to be able to parse the output. This can be problematic if your `stdout` is not set to UTF-8; it can mess up special characters is e.g. measurement units and lead to XML validation errors. In addition to that, Java itself might output data in non-UTF-8 encodings, in which case it might be necessary to set `JAVA_TOOL_OPTIONS=-Dfile.encoding=UTF8`.
+
```

### Comparing `omero-cli-transfer-0.4.0/src/omero_cli_transfer.py` & `omero-cli-transfer-0.5.0/src/omero_cli_transfer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-
+# Copyright (C) 2022 The Jackson Laboratory
+# All rights reserved.
+#
+# Use is subject to license terms supplied in LICENSE.
 
 """
    Plugin for transfering objects and annotations between servers
 
 """
 
 from pathlib import Path
@@ -15,14 +18,15 @@
 import shutil
 from typing import DefaultDict
 import hashlib
 from zipfile import ZipFile
 from typing import Callable, List, Any, Dict, Union, Optional, Tuple
 
 from generate_xml import populate_xml, populate_tsv, populate_rocrate
+from generate_xml import populate_xml_folder
 from generate_omero_objects import populate_omero
 
 import ezomero
 from ome_types.model import CommentAnnotation, OME
 from ome_types import from_xml
 from omero.sys import Parameters
 from omero.rtypes import rstring
@@ -104,24 +108,36 @@
 Examples:
 omero transfer unpack transfer_pack.zip
 omero transfer unpack --output /home/user/optional_folder --ln_s
 omero transfer unpack --folder /home/user/unpacked_folder/ --skip upgrade
 omero transfer unpack pack.tar --metadata db_id orig_user hostname
 """)
 
+PREPARE_HELP = ("""Creates an XML from a folder with images.
+
+Creates an XML file appropriate for usage with `omero transfer unpack` from
+a folder that contains image files, rather than a source OMERO server. This
+is intended as a first step on a bulk-import workflow, followed by using
+`omero transfer unpack` to complete an import.
+
+Examples:
+omero transfer prepare /home/user/folder_with_files
+""")
+
 
 def gateway_required(func: Callable) -> Callable:
     """
     Decorator which initializes a client (self.client),
     a BlitzGateway (self.gateway), and makes sure that
     all services of the Blitzgateway are closed again.
     """
     @wraps(func)
     def _wrapper(self, *args, **kwargs):
         self.client = self.ctx.conn(*args)
+        self.session = self.client.getSessionId()
         self.gateway = BlitzGateway(client_obj=self.client)
         router = self.client.getRouter(self.client.getCommunicator())
         self.hostname = str(router).split('-h ')[-1].split()[0]
         try:
             return func(self, *args, **kwargs)
         finally:
             if self.gateway is not None:
@@ -134,14 +150,15 @@
 class TransferControl(GraphControl):
 
     def _configure(self, parser):
         parser.add_login_arguments()
         sub = parser.sub()
         pack = parser.add(sub, self.pack, PACK_HELP)
         unpack = parser.add(sub, self.unpack, UNPACK_HELP)
+        prepare = parser.add(sub, self.prepare, PREPARE_HELP)
 
         render_type = ProxyStringType("Project")
         obj_help = ("Object to be packed for transfer")
         pack.add_argument("object", type=render_type, help=obj_help)
         file_help = ("Path to where the packed file will be saved")
         pack.add_argument(
                 "--zip", help="Pack into a zip file rather than a tarball",
@@ -183,25 +200,32 @@
         unpack.add_argument(
             "--metadata",
             choices=['all', 'none', 'img_id', 'plate_id', 'timestamp',
                      'software', 'version', 'md5', 'hostname', 'db_id',
                      'orig_user', 'orig_group'], nargs='+',
             help="Metadata field to be added to MapAnnotation"
         )
+        folder_help = ("Path to folder with image files")
+        prepare.add_argument("folder", type=str, help=folder_help)
 
     @gateway_required
     def pack(self, args):
         """ Implements the 'pack' command """
         self.__pack(args)
 
     @gateway_required
     def unpack(self, args):
-        """ Implements the 'pack' command """
+        """ Implements the 'unpack' command """
         self.__unpack(args)
 
+    @gateway_required
+    def prepare(self, args):
+        """ Implements the 'prepare' command """
+        self.__prepare(args)
+
     def _get_path_to_repo(self) -> List[str]:
         shared = self.client.sf.sharedResources()
         repos = shared.repositories()
         repos = list(zip(repos.descriptions, repos.proxies))
         mrepos = []
         for _, pair in enumerate(repos):
             desc, prx = pair
@@ -340,15 +364,15 @@
         self._process_metadata(args.metadata)
         if not args.folder:
             print(f"Unzipping {args.filepath}...")
             hash, ome, folder = self._load_from_pack(args.filepath,
                                                      args.output)
         else:
             folder = Path(args.filepath)
-            ome = from_xml(folder / "transfer.xml")
+            ome = from_xml(folder / "transfer.xml", parser='xmlschema')
             hash = "imported from folder"
         print("Generating Image mapping and import filelist...")
         ome, src_img_map, filelist = self._create_image_map(ome)
         print("Importing data as orphans...")
         if args.ln_s_import:
             ln_s = True
         else:
@@ -389,15 +413,15 @@
                     zipobj.extractall(str(folder))
             elif Path(filepath).suffix == '.tar':
                 shutil.unpack_archive(filepath, str(folder), 'tar')
             else:
                 raise ValueError("File is not a zip or tar file")
         else:
             raise FileNotFoundError("filepath is not a zip file")
-        ome = from_xml(folder / "transfer.xml")
+        ome = from_xml(folder / "transfer.xml", parser='xmlschema')
         return hash, ome, folder
 
     def _create_image_map(self, ome: OME
                           ) -> Tuple[OME, DefaultDict, List[str]]:
         if not (type(ome) is OME):
             raise TypeError("XML is not valid OME format")
         img_map = DefaultDict(list)
@@ -517,14 +541,18 @@
                 dest_v = dest_dict[src_k]
                 if len(src_v) == len(dest_v):
                     for count in range(len(src_v)):
                         map_key = f"Image:{src_v[count]}"
                         imgmap[map_key] = dest_v[count]
         return imgmap
 
+    def __prepare(self, args):
+        populate_xml_folder(args.folder, self.gateway, self.session)
+        return
+
 
 try:
     register("transfer", TransferControl, HELP)
 except NameError:
     if __name__ == "__main__":
         cli = CLI()
         cli.register("transfer", TransferControl, HELP)
```

