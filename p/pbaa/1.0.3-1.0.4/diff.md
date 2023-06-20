# Comparing `tmp/pbaa-1.0.3.tar.gz` & `tmp/pbaa-1.0.4.tar.gz`

## Comparing `pbaa-1.0.3.tar` & `pbaa-1.0.4.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rwxr-xr-x   0        0        0      434 2020-02-02 00:00:00.000000 pbaa-1.0.3/.pre-commit-config.yaml
--rwxr-xr-x   0        0        0     1077 2020-02-02 00:00:00.000000 pbaa-1.0.3/.github/workflows/test.yml
--rwxr-xr-x   0        0        0  5701095 2020-02-02 00:00:00.000000 pbaa-1.0.3/assets/demo9.jpg
--rwxr-xr-x   0        0        0   720440 2020-02-02 00:00:00.000000 pbaa-1.0.3/assets/demo9.json
--rwxr-xr-x   0        0        0  1287943 2020-02-02 00:00:00.000000 pbaa-1.0.3/assets/demo9_det.jpg
--rwxr-xr-x   0        0        0  1239235 2020-02-02 00:00:00.000000 pbaa-1.0.3/assets/demo9_seg.jpg
--rwxr-xr-x   0        0        0      170 2020-02-02 00:00:00.000000 pbaa-1.0.3/docker/Dockerfile
--rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 pbaa-1.0.3/src/pbaa/__about__.py
--rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 pbaa-1.0.3/src/pbaa/__init__.py
--rwxr-xr-x   0        0        0      202 2020-02-02 00:00:00.000000 pbaa-1.0.3/src/pbaa/__main__.py
--rwxr-xr-x   0        0        0     1160 2020-02-02 00:00:00.000000 pbaa-1.0.3/src/pbaa/cli/__init__.py
--rwxr-xr-x   0        0        0      248 2020-02-02 00:00:00.000000 pbaa-1.0.3/src/pbaa/core/__init__.py
--rwxr-xr-x   0        0        0     6782 2020-02-02 00:00:00.000000 pbaa-1.0.3/src/pbaa/core/check.py
--rwxr-xr-x   0        0        0     5053 2020-02-02 00:00:00.000000 pbaa-1.0.3/src/pbaa/core/grounded_sam.py
--rwxr-xr-x   0        0        0      285 2020-02-02 00:00:00.000000 pbaa-1.0.3/src/pbaa/core/prerequisite.py
--rwxr-xr-x   0        0        0      111 2020-02-02 00:00:00.000000 pbaa-1.0.3/src/pbaa/core/utils.py
--rwxr-xr-x   0        0        0      111 2020-02-02 00:00:00.000000 pbaa-1.0.3/tests/__init__.py
--rwxr-xr-x   0        0        0      256 2020-02-02 00:00:00.000000 pbaa-1.0.3/tests/test_dependencies.py
--rwxr-xr-x   0        0        0     3092 2020-02-02 00:00:00.000000 pbaa-1.0.3/.gitignore
--rwxr-xr-x   0        0        0    10280 2020-02-02 00:00:00.000000 pbaa-1.0.3/LICENSE.txt
--rwxr-xr-x   0        0        0     3812 2020-02-02 00:00:00.000000 pbaa-1.0.3/README.md
--rwxr-xr-x   0        0        0     3252 2020-02-02 00:00:00.000000 pbaa-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 pbaa-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 pbaa-1.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 pbaa-1.0.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0  5701095 2020-02-02 00:00:00.000000 pbaa-1.0.4/assets/demo9.jpg
+-rw-r--r--   0        0        0   118988 2020-02-02 00:00:00.000000 pbaa-1.0.4/assets/demo9.json
+-rw-r--r--   0        0        0  1287943 2020-02-02 00:00:00.000000 pbaa-1.0.4/assets/demo9_det.jpg
+-rw-r--r--   0        0        0  1239235 2020-02-02 00:00:00.000000 pbaa-1.0.4/assets/demo9_seg.jpg
+-rw-r--r--   0        0        0   978675 2020-02-02 00:00:00.000000 pbaa-1.0.4/assets/gradio_demo.png
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pbaa-1.0.4/docker/Dockerfile
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pbaa-1.0.4/src/pbaa/__about__.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 pbaa-1.0.4/src/pbaa/__init__.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 pbaa-1.0.4/src/pbaa/__main__.py
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 pbaa-1.0.4/src/pbaa/cli/__init__.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 pbaa-1.0.4/src/pbaa/core/__init__.py
+-rw-r--r--   0        0        0     6828 2020-02-02 00:00:00.000000 pbaa-1.0.4/src/pbaa/core/check.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 pbaa-1.0.4/src/pbaa/core/gradio_app.py
+-rw-r--r--   0        0        0     8105 2020-02-02 00:00:00.000000 pbaa-1.0.4/src/pbaa/core/grounded_sam.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 pbaa-1.0.4/src/pbaa/core/prerequisite.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pbaa-1.0.4/src/pbaa/core/utils.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 pbaa-1.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pbaa-1.0.4/tests/test_dependencies.py
+-rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 pbaa-1.0.4/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 pbaa-1.0.4/LICENSE.txt
+-rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 pbaa-1.0.4/README.md
+-rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 pbaa-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5288 2020-02-02 00:00:00.000000 pbaa-1.0.4/PKG-INFO
```

### Comparing `pbaa-1.0.3/.github/workflows/test.yml` & `pbaa-1.0.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pbaa-1.0.3/assets/demo9.jpg` & `pbaa-1.0.4/assets/demo9.jpg`

 * *Files identical despite different names*

### Comparing `pbaa-1.0.3/assets/demo9_det.jpg` & `pbaa-1.0.4/assets/demo9_det.jpg`

 * *Files identical despite different names*

### Comparing `pbaa-1.0.3/assets/demo9_seg.jpg` & `pbaa-1.0.4/assets/demo9_seg.jpg`

 * *Files identical despite different names*

### Comparing `pbaa-1.0.3/src/pbaa/cli/__init__.py` & `pbaa-1.0.4/src/pbaa/cli/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,50 @@
 # SPDX-FileCopyrightText: 2023-present dh031200 <imbird0312@gmail.com>
 #
 # SPDX-License-Identifier: Apache-2.0
+import sys
+
 import click
 
-from pbaa import inference, model_init
+from pbaa import PBAA, app
 from pbaa.__about__ import __version__
 
 
 @click.group(context_settings={"help_option_names": ["-h", "--help"]}, invoke_without_command=True)
 @click.version_option(version=__version__, prog_name="pbaa")
-@click.option("--src", "-s", type=str, required=True, help="Source image or directory path")
+@click.option("--src", "-s", type=str, help="Source image or directory path")
 @click.option(
     "--prompt",
     "-p",
     type=(str, str),
-    required=True,
     multiple=True,
     help="Space-separated a pair of prompt and target classe. (Multi)",
 )
 @click.option("--box_threshold", "-b", type=float, default=0.25, help="Threshold for Object Detection (default: 0.25)")
 @click.option("--nms_threshold", "-n", type=float, default=0.8, help="Threshold for NMS (default: 0.8)")
-@click.option("--output_dir", "-o", type=str, default=".", help="Path to result data (default: '.')")
-def pbaa(src, prompt, box_threshold, nms_threshold, output_dir):
-    model_init()
-    _prompt = {i.lower(): v for i, v in prompt}
-    inference(src, _prompt, box_threshold, nms_threshold, output_dir)
+@click.option("--output_dir", "-o", type=str, default="outputs", help="Path to result data (default: 'outputs')")
+@click.option("--gradio", "-g", type=bool, default=False, is_flag=True, help="Launch gradio app")
+def pbaa(src, prompt, box_threshold, nms_threshold, output_dir, gradio):
+    annotator = PBAA()
+    if gradio:
+        click.echo("Launch gradio app")
+        app(annotator.inference)
+    else:
+        is_failed = False
+        if not src:
+            click.echo("Error: Missing option '--src' / '-s'.")
+            is_failed = True
+        if not prompt:
+            click.echo("Error: Missing option '--prompt' / '-p'.")
+            is_failed = True
+        if is_failed:
+            sys.exit(-1)
+        _prompt = {i.lower(): v for i, v in prompt}
+        annotator.inference(
+            src=src,
+            prompt=_prompt,
+            annot_format=None,
+            box_threshold=box_threshold,
+            nms_threshold=nms_threshold,
+            save=True,
+            output_dir=output_dir,
+        )
```

### Comparing `pbaa-1.0.3/src/pbaa/core/check.py` & `pbaa-1.0.4/src/pbaa/core/check.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,14 +184,15 @@
         name = package_rename(name)
         if name == "python":
             python_version_check()
         elif name == "pip":
             pass
         else:
             if not installed_packages[name]:
+                logger.warning(f"Module `{name}` not found. Try to install.")
                 if name == "torch" and is_arm:
                     install_torch_arm()
                 elif name == "torchvision":
                     if is_arm:
                         install_torchvision_arm()
                     elif is_linux:
                         if check_cuda():
@@ -201,16 +202,15 @@
                     elif is_windows:
                         install_dependency(name, version)
                 elif name in ["groundingdino", "segment-anything"]:
                     install_from_git(name)
                 else:
                     install_dependency(name, version)
                 installed_packages = get_installed_packages()
-            else:
-                logger.info(f"{name} : {installed_packages[name]}")
 
             if not installed_packages[name]:
                 raise ModuleNotFoundError
+    logger.info("Dependencies checked successfully.")
 
 
 if __name__ == "__main__":
     check()
```

### Comparing `pbaa-1.0.3/.gitignore` & `pbaa-1.0.4/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -155,7 +155,9 @@
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 /.ruff_cache/
+/flagged/
+/outputs/
```

### Comparing `pbaa-1.0.3/LICENSE.txt` & `pbaa-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pbaa-1.0.3/README.md` & `pbaa-1.0.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -7,27 +7,28 @@
 **Prompt-based automatic annotation**
 
 -----
 
 **Table of Contents**
 
 - [Installation](#installation)
-- [Usage](#Usage)
-- [Demo](#Demo)
+- [Usage](#usage)
+- [Gradio](#gradio)
+- [Demo](#demo)
 - [License](#license)
 - [Acknowledgements](#acknowledgements)
 
 ## Installation
 
 ### Docker (Recommend)
 
 ```console
 git clone https://github.com/dh031200/pbaa.git
 docker build docker -t pbaa:latest
-docker run --gpus all -it --ipc=host -v `pwd`:/workspace pbaa:latest
+docker run --gpus all -it --ipc=host -v `pwd`:/workspace -p 7860:7860 pbaa:latest
 ```
 
 ### Without docker
 
 The code requires `python>=3.8`, `CUDA==11.7`.
 
 ```console
@@ -39,20 +40,21 @@
 ### Options
 
 ```console
 Usage: pbaa [OPTIONS]
 
 Options:
   --version                    Show the version and exit.
-  -s, --src TEXT               Source image or directory path  [required]
+  -s, --src TEXT               Source image or directory path
   -p, --prompt <TEXT TEXT>...  Space-separated a pair of prompt and target
-                               classe. (Multi)  [required]
+                               classe. (Multi)
   -b, --box_threshold FLOAT    Threshold for Object Detection (default: 0.25)
   -n, --nms_threshold FLOAT    Threshold for NMS (default: 0.8)
-  -o, --output_dir TEXT        Path to result data (default: '.')
+  -o, --output_dir TEXT        Path to result data (default: 'outputs')
+  -g, --gradio                 Launch gradio app
   -h, --help                   Show this message and exit.
 ```
 
 ### CLI
 
 ```console
 # pbaa -s <Source> -p <prompt> <class> -p <prompt> <class> ...
@@ -60,21 +62,41 @@
 pbaa -s source_image.jpg -p "black dog" dog
 pbaa -s source_image.jpg -p "black dog" dog -p "white cat" cat
 ```
 
 ### Python
 
 ```python
-from pbaa import model_init, inference
+from pbaa import PBAA
 
-model_init()
-# inference(<Source path>, <prompt:class>, box_threshold=0.25, nms_threshold=0.8, output_dir=".")
-inference("path/to/source_image.jpg", {"black dog": "dog", "white cat": "cat"})
+annotator = PBAA()
+# inference(<Source path>, <prompt:class dict>, box_threshold=0.25, nms_threshold=0.8, save=None, output_dir="outputs")
+annotator("path/to/source_image.jpg", {"black dog": "dog", "white cat": "cat"})
 ```
 
+## Gradio
+
+Run the [gradio](https://github.com/gradio-app/gradio) demo with a simple command
+
+```console
+pbaa -g
+```
+
+Output
+
+```
+Launch gradio app
+Running on local URL:  http://0.0.0.0:7860
+```
+
+You can now access Gradio demos using your browser.
+[localhost:7860](http://localhost:7860)
+
+![gradio_demo](https://github.com/dh031200/pbaa/blob/main/assets/gradio_demo.png?raw=true)
+
 ## Demo
 
 ```console
 # Source : assets/demo9.jpg
 # prompts : {"plant" : "plant", "picture" : "picture", "dog": "dog", "lamp" : "lamp", "carpet" : "carpet", "sofa" : "sofa"}
 
 pbaa -s assets/demo9.jpg -p plant plant -p picture picture -p dog dog -p lamp lamp -p carpet carpet -p sofa sofa
@@ -87,14 +109,16 @@
 ### Result data
 
 [demo9.json](https://github.com/dh031200/pbaa/blob/main/assets/demo9.json)<br>
 
 ```console
 json structure
 
+filename
+prompt
 index
   ├ cls : class name
   ├ conf : confidence score
   ├ box : bounding box coordinates
   └ poly : polygon coordinates
 ```
```

### Comparing `pbaa-1.0.3/pyproject.toml` & `pbaa-1.0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -125,14 +125,16 @@
   "B027",
   # Allow boolean positional values in function calls, like `dict.get(... True)`
   "FBT003",
   # Ignore checks for possible passwords
   "S105", "S106", "S107",
   # Ignore complexity
   "C901", "PLR0911", "PLR0912", "PLR0913", "PLR0915",
+  # Ignore binding all interfaces
+  "S104",
   # Ignore Subprocess
   "S602", "S603", "S605", "S607",
 ]
 unfixable = [
   # Don't touch unused imports
   "F401",
 ]
```

### Comparing `pbaa-1.0.3/PKG-INFO` & `pbaa-1.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbaa
-Version: 1.0.3
+Version: 1.0.4
 Summary: Prompt based automatic annotation
 Project-URL: Documentation, https://github.com/dh031200/pbaa#readme
 Project-URL: Issues, https://github.com/dh031200/pbaa/issues
 Project-URL: Source, https://github.com/dh031200/pbaa
 Author-email: dh031200 <imbird0312@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
@@ -32,27 +32,28 @@
 **Prompt-based automatic annotation**
 
 -----
 
 **Table of Contents**
 
 - [Installation](#installation)
-- [Usage](#Usage)
-- [Demo](#Demo)
+- [Usage](#usage)
+- [Gradio](#gradio)
+- [Demo](#demo)
 - [License](#license)
 - [Acknowledgements](#acknowledgements)
 
 ## Installation
 
 ### Docker (Recommend)
 
 ```console
 git clone https://github.com/dh031200/pbaa.git
 docker build docker -t pbaa:latest
-docker run --gpus all -it --ipc=host -v `pwd`:/workspace pbaa:latest
+docker run --gpus all -it --ipc=host -v `pwd`:/workspace -p 7860:7860 pbaa:latest
 ```
 
 ### Without docker
 
 The code requires `python>=3.8`, `CUDA==11.7`.
 
 ```console
@@ -64,20 +65,21 @@
 ### Options
 
 ```console
 Usage: pbaa [OPTIONS]
 
 Options:
   --version                    Show the version and exit.
-  -s, --src TEXT               Source image or directory path  [required]
+  -s, --src TEXT               Source image or directory path
   -p, --prompt <TEXT TEXT>...  Space-separated a pair of prompt and target
-                               classe. (Multi)  [required]
+                               classe. (Multi)
   -b, --box_threshold FLOAT    Threshold for Object Detection (default: 0.25)
   -n, --nms_threshold FLOAT    Threshold for NMS (default: 0.8)
-  -o, --output_dir TEXT        Path to result data (default: '.')
+  -o, --output_dir TEXT        Path to result data (default: 'outputs')
+  -g, --gradio                 Launch gradio app
   -h, --help                   Show this message and exit.
 ```
 
 ### CLI
 
 ```console
 # pbaa -s <Source> -p <prompt> <class> -p <prompt> <class> ...
@@ -85,21 +87,41 @@
 pbaa -s source_image.jpg -p "black dog" dog
 pbaa -s source_image.jpg -p "black dog" dog -p "white cat" cat
 ```
 
 ### Python
 
 ```python
-from pbaa import model_init, inference
+from pbaa import PBAA
 
-model_init()
-# inference(<Source path>, <prompt:class>, box_threshold=0.25, nms_threshold=0.8, output_dir=".")
-inference("path/to/source_image.jpg", {"black dog": "dog", "white cat": "cat"})
+annotator = PBAA()
+# inference(<Source path>, <prompt:class dict>, box_threshold=0.25, nms_threshold=0.8, save=None, output_dir="outputs")
+annotator("path/to/source_image.jpg", {"black dog": "dog", "white cat": "cat"})
 ```
 
+## Gradio
+
+Run the [gradio](https://github.com/gradio-app/gradio) demo with a simple command
+
+```console
+pbaa -g
+```
+
+Output
+
+```
+Launch gradio app
+Running on local URL:  http://0.0.0.0:7860
+```
+
+You can now access Gradio demos using your browser.
+[localhost:7860](http://localhost:7860)
+
+![gradio_demo](https://github.com/dh031200/pbaa/blob/main/assets/gradio_demo.png?raw=true)
+
 ## Demo
 
 ```console
 # Source : assets/demo9.jpg
 # prompts : {"plant" : "plant", "picture" : "picture", "dog": "dog", "lamp" : "lamp", "carpet" : "carpet", "sofa" : "sofa"}
 
 pbaa -s assets/demo9.jpg -p plant plant -p picture picture -p dog dog -p lamp lamp -p carpet carpet -p sofa sofa
@@ -112,14 +134,16 @@
 ### Result data
 
 [demo9.json](https://github.com/dh031200/pbaa/blob/main/assets/demo9.json)<br>
 
 ```console
 json structure
 
+filename
+prompt
 index
   ├ cls : class name
   ├ conf : confidence score
   ├ box : bounding box coordinates
   └ poly : polygon coordinates
 ```
```

