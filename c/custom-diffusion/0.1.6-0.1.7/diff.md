# Comparing `tmp/custom_diffusion-0.1.6.tar.gz` & `tmp/custom_diffusion-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_diffusion-0.1.6.tar", last modified: Mon Jun 19 20:35:29 2023, max compression
+gzip compressed data, was "custom_diffusion-0.1.7.tar", last modified: Mon Jun 19 22:03:51 2023, max compression
```

## Comparing `custom_diffusion-0.1.6.tar` & `custom_diffusion-0.1.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 20:35:29.444764 custom_diffusion-0.1.6/
--rw-rw-rw-   0        0        0    11357 2023-06-09 21:50:57.000000 custom_diffusion-0.1.6/LICENSE
--rw-rw-rw-   0        0        0       24 2023-06-09 21:50:57.000000 custom_diffusion-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     3489 2023-06-19 20:35:29.445763 custom_diffusion-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2322 2023-06-19 20:27:45.000000 custom_diffusion-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 20:35:29.364748 custom_diffusion-0.1.6/custom_diffusion/
--rw-rw-rw-   0        0        0      317 2023-06-19 20:35:18.000000 custom_diffusion-0.1.6/custom_diffusion/__init__.py
--rw-rw-rw-   0        0        0     1538 2023-06-19 20:27:45.000000 custom_diffusion-0.1.6/custom_diffusion/demo.py
-drwxrwxrwx   0        0        0        0 2023-06-19 20:35:29.424760 custom_diffusion-0.1.6/custom_diffusion/pipelines/
--rw-rw-rw-   0        0        0        0 2023-06-19 20:27:45.000000 custom_diffusion-0.1.6/custom_diffusion/pipelines/__init__.py
--rw-rw-rw-   0        0        0     7349 2023-06-19 20:27:45.000000 custom_diffusion-0.1.6/custom_diffusion/pipelines/controlnet_img2img.py
--rw-rw-rw-   0        0        0     7320 2023-06-19 20:27:45.000000 custom_diffusion-0.1.6/custom_diffusion/pipelines/controlnet_inpaint.py
--rw-rw-rw-   0        0        0     7136 2023-06-19 20:27:45.000000 custom_diffusion-0.1.6/custom_diffusion/pipelines/controlnet_pipeline.py
--rw-rw-rw-   0        0        0     6354 2023-06-19 20:27:45.000000 custom_diffusion-0.1.6/custom_diffusion/pipelines/stable_diffusion_img2img.py
--rw-rw-rw-   0        0        0     6414 2023-06-19 20:27:45.000000 custom_diffusion-0.1.6/custom_diffusion/pipelines/stable_diffusion_instruct_pix2pix.py
--rw-rw-rw-   0        0        0     4598 2023-06-19 20:27:45.000000 custom_diffusion-0.1.6/custom_diffusion/pipelines/stable_diffusion_text2image.py
--rw-rw-rw-   0        0        0     6361 2023-06-19 20:27:45.000000 custom_diffusion-0.1.6/custom_diffusion/pipelines/stable_diffusion_upscale.py
--rw-rw-rw-   0        0        0     8950 2023-06-19 20:27:45.000000 custom_diffusion-0.1.6/custom_diffusion/preprocces.py
-drwxrwxrwx   0        0        0        0 2023-06-19 20:35:29.443764 custom_diffusion-0.1.6/custom_diffusion/utils/
--rw-rw-rw-   0        0        0        0 2023-06-09 21:50:57.000000 custom_diffusion-0.1.6/custom_diffusion/utils/__init__.py
--rw-rw-rw-   0        0        0     2330 2023-06-19 20:27:45.000000 custom_diffusion-0.1.6/custom_diffusion/utils/data_utils.py
--rw-rw-rw-   0        0        0     1759 2023-06-19 20:27:45.000000 custom_diffusion-0.1.6/custom_diffusion/utils/downloads.py
--rw-rw-rw-   0        0        0      811 2023-06-19 20:27:45.000000 custom_diffusion-0.1.6/custom_diffusion/utils/model_list.py
--rw-rw-rw-   0        0        0     1268 2023-06-19 20:27:45.000000 custom_diffusion-0.1.6/custom_diffusion/utils/scheduler_utils.py
--rw-rw-rw-   0        0        0     3584 2023-06-19 20:27:45.000000 custom_diffusion-0.1.6/custom_diffusion/utils/video_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-19 20:35:29.402755 custom_diffusion-0.1.6/custom_diffusion.egg-info/
--rw-rw-rw-   0        0        0     3489 2023-06-19 20:35:28.000000 custom_diffusion-0.1.6/custom_diffusion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1008 2023-06-19 20:35:29.000000 custom_diffusion-0.1.6/custom_diffusion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 20:35:28.000000 custom_diffusion-0.1.6/custom_diffusion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      175 2023-06-19 20:35:29.000000 custom_diffusion-0.1.6/custom_diffusion.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-19 20:35:29.000000 custom_diffusion-0.1.6/custom_diffusion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       80 2023-06-09 21:50:57.000000 custom_diffusion-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0      113 2023-06-10 22:16:53.000000 custom_diffusion-0.1.6/requirements.txt
--rw-rw-rw-   0        0        0      375 2023-06-19 20:35:29.448766 custom_diffusion-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     2151 2023-06-09 21:50:57.000000 custom_diffusion-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 22:03:51.646218 custom_diffusion-0.1.7/
+-rw-rw-rw-   0        0        0    11357 2023-06-09 21:50:57.000000 custom_diffusion-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-06-09 21:50:57.000000 custom_diffusion-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     3489 2023-06-19 22:03:51.646218 custom_diffusion-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2322 2023-06-19 20:27:45.000000 custom_diffusion-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 22:03:51.589212 custom_diffusion-0.1.7/custom_diffusion/
+-rw-rw-rw-   0        0        0      317 2023-06-19 21:43:15.000000 custom_diffusion-0.1.7/custom_diffusion/__init__.py
+-rw-rw-rw-   0        0        0     1538 2023-06-19 20:27:45.000000 custom_diffusion-0.1.7/custom_diffusion/demo.py
+drwxrwxrwx   0        0        0        0 2023-06-19 22:03:51.632214 custom_diffusion-0.1.7/custom_diffusion/pipelines/
+-rw-rw-rw-   0        0        0        0 2023-06-19 20:27:45.000000 custom_diffusion-0.1.7/custom_diffusion/pipelines/__init__.py
+-rw-rw-rw-   0        0        0     7349 2023-06-19 20:27:45.000000 custom_diffusion-0.1.7/custom_diffusion/pipelines/controlnet_img2img.py
+-rw-rw-rw-   0        0        0     7320 2023-06-19 20:27:45.000000 custom_diffusion-0.1.7/custom_diffusion/pipelines/controlnet_inpaint.py
+-rw-rw-rw-   0        0        0     7136 2023-06-19 20:27:45.000000 custom_diffusion-0.1.7/custom_diffusion/pipelines/controlnet_pipeline.py
+-rw-rw-rw-   0        0        0     6052 2023-06-19 21:32:13.000000 custom_diffusion-0.1.7/custom_diffusion/pipelines/stable_diffusion_img2img.py
+-rw-rw-rw-   0        0        0     6414 2023-06-19 20:27:45.000000 custom_diffusion-0.1.7/custom_diffusion/pipelines/stable_diffusion_instruct_pix2pix.py
+-rw-rw-rw-   0        0        0     4598 2023-06-19 20:27:45.000000 custom_diffusion-0.1.7/custom_diffusion/pipelines/stable_diffusion_text2image.py
+-rw-rw-rw-   0        0        0     6361 2023-06-19 20:27:45.000000 custom_diffusion-0.1.7/custom_diffusion/pipelines/stable_diffusion_upscale.py
+-rw-rw-rw-   0        0        0     8950 2023-06-19 20:27:45.000000 custom_diffusion-0.1.7/custom_diffusion/preprocces.py
+drwxrwxrwx   0        0        0        0 2023-06-19 22:03:51.645216 custom_diffusion-0.1.7/custom_diffusion/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-09 21:50:57.000000 custom_diffusion-0.1.7/custom_diffusion/utils/__init__.py
+-rw-rw-rw-   0        0        0     2331 2023-06-19 21:37:09.000000 custom_diffusion-0.1.7/custom_diffusion/utils/data_utils.py
+-rw-rw-rw-   0        0        0     1759 2023-06-19 20:27:45.000000 custom_diffusion-0.1.7/custom_diffusion/utils/downloads.py
+-rw-rw-rw-   0        0        0      811 2023-06-19 20:27:45.000000 custom_diffusion-0.1.7/custom_diffusion/utils/model_list.py
+-rw-rw-rw-   0        0        0     1268 2023-06-19 20:27:45.000000 custom_diffusion-0.1.7/custom_diffusion/utils/scheduler_utils.py
+-rw-rw-rw-   0        0        0     3584 2023-06-19 20:27:45.000000 custom_diffusion-0.1.7/custom_diffusion/utils/video_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-19 22:03:51.616208 custom_diffusion-0.1.7/custom_diffusion.egg-info/
+-rw-rw-rw-   0        0        0     3489 2023-06-19 22:03:50.000000 custom_diffusion-0.1.7/custom_diffusion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1008 2023-06-19 22:03:51.000000 custom_diffusion-0.1.7/custom_diffusion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 22:03:50.000000 custom_diffusion-0.1.7/custom_diffusion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      175 2023-06-19 22:03:51.000000 custom_diffusion-0.1.7/custom_diffusion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-19 22:03:51.000000 custom_diffusion-0.1.7/custom_diffusion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       80 2023-06-09 21:50:57.000000 custom_diffusion-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0      113 2023-06-10 22:16:53.000000 custom_diffusion-0.1.7/requirements.txt
+-rw-rw-rw-   0        0        0      375 2023-06-19 22:03:51.648218 custom_diffusion-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     2151 2023-06-09 21:50:57.000000 custom_diffusion-0.1.7/setup.py
```

### Comparing `custom_diffusion-0.1.6/LICENSE` & `custom_diffusion-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.1.6/PKG-INFO` & `custom_diffusion-0.1.7/custom_diffusion.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: custom_diffusion
-Version: 0.1.6
+Name: custom-diffusion
+Version: 0.1.7
 Summary: Custom Diffusion: Creating Video from Frame Using Multiple Diffusion
 Home-page: https://github.com/kadirnar/Custom-Diffusion
 Author: kadirnar
 License: Apache License 2.0
 Keywords: machine-learning,deep-learning,pytorch,diffusion,diffusion models,controlnet,stable diffusion
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: custom_diffusion Version: 0.1.6 Summary: Custom
+Metadata-Version: 2.1 Name: custom-diffusion Version: 0.1.7 Summary: Custom
 Diffusion: Creating Video from Frame Using Multiple Diffusion Home-page: https:
 //github.com/kadirnar/Custom-Diffusion Author: kadirnar License: Apache License
 2.0 Keywords: machine-learning,deep-learning,pytorch,diffusion,diffusion
 models,controlnet,stable diffusion Platform: UNKNOWN Classifier: Development
 Status :: 5 - Production/Stable Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: Programming Language :: Python :: 3 Classifier:
```

### Comparing `custom_diffusion-0.1.6/README.md` & `custom_diffusion-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.1.6/custom_diffusion/demo.py` & `custom_diffusion-0.1.7/custom_diffusion/demo.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.1.6/custom_diffusion/pipelines/controlnet_img2img.py` & `custom_diffusion-0.1.7/custom_diffusion/pipelines/controlnet_img2img.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.1.6/custom_diffusion/pipelines/controlnet_inpaint.py` & `custom_diffusion-0.1.7/custom_diffusion/pipelines/controlnet_inpaint.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.1.6/custom_diffusion/pipelines/controlnet_pipeline.py` & `custom_diffusion-0.1.7/custom_diffusion/pipelines/controlnet_pipeline.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.1.6/custom_diffusion/pipelines/stable_diffusion_img2img.py` & `custom_diffusion-0.1.7/custom_diffusion/pipelines/stable_diffusion_instruct_pix2pix.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import List, Optional
 
 import torch
-from diffusers import StableDiffusionImg2ImgPipeline
+from diffusers import StableDiffusionInstructPix2PixPipeline
 from PIL import Image
 
 from custom_diffusion.preprocces import preprocces_dicts
 from custom_diffusion.utils.data_utils import center_crop_and_resize
 from custom_diffusion.utils.scheduler_utils import get_scheduler
 
 
-class StableDiffusionImg2ImgGenerator:
+class StableDiffusionInstructPix2PixGenerator:
     """
     A class to handle image generation using stable diffusion and control net models.
     """
 
     def __init__(self):
         self.pipe = None
         self.model_cache = {}
@@ -22,15 +22,15 @@
         """
         This function loads the stable diffusion pipeline.
 
         Args:
         stable_model_path (str): Path to the stable diffusion pipeline.
 
         """
-        self.pipe = StableDiffusionImg2ImgPipeline.from_pretrained(
+        self.pipe = StableDiffusionInstructPix2PixPipeline.from_pretrained(
             pretrained_model_name_or_path=stable_model_path,
             safety_checker=None,
             torch_dtype=torch.float16,
         )
 
     def load_model(
         self,
@@ -110,15 +110,15 @@
         scheduler_name: str = "DDIM",
         images_path_list: List[str] = ["test.png"],
         prompt: List[str] = ["A photo of a cat."],
         negative_prompt: List[str] = ["bad"],
         num_images_per_prompt: int = 1,
         num_inference_steps: int = 20,
         guidance_scale: int = 7.0,
-        strength: float = 0.5,
+        image_guidance_scale: float = 1.5,
         generator_seed: int = 0,
         preprocess_type: str = "Canny",
         resize_type: str = "center_crop_and_resize",
     ):
         """
         This function generates an image based on the given parameters.
 
@@ -160,15 +160,15 @@
 
         generator = self._setup_generator(generator_seed)
 
         output = pipe(
             prompt=prompt,
             control_image=control_image_list,
             image=read_image_list,
-            strength=strength,
+            image_guidance_scale=image_guidance_scale,
             negative_prompt=negative_prompt,
             num_images_per_prompt=num_images_per_prompt,
             num_inference_steps=num_inference_steps,
             guidance_scale=guidance_scale,
             generator=generator,
         ).images
```

### Comparing `custom_diffusion-0.1.6/custom_diffusion/pipelines/stable_diffusion_instruct_pix2pix.py` & `custom_diffusion-0.1.7/custom_diffusion/pipelines/stable_diffusion_upscale.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import List, Optional
 
 import torch
-from diffusers import StableDiffusionInstructPix2PixPipeline
+from diffusers import StableDiffusionUpscalePipeline
 from PIL import Image
 
 from custom_diffusion.preprocces import preprocces_dicts
 from custom_diffusion.utils.data_utils import center_crop_and_resize
 from custom_diffusion.utils.scheduler_utils import get_scheduler
 
 
-class StableDiffusionInstructPix2PixGenerator:
+class StableDiffusionUpscalerGenerator:
     """
     A class to handle image generation using stable diffusion and control net models.
     """
 
     def __init__(self):
         self.pipe = None
         self.model_cache = {}
@@ -22,15 +22,15 @@
         """
         This function loads the stable diffusion pipeline.
 
         Args:
         stable_model_path (str): Path to the stable diffusion pipeline.
 
         """
-        self.pipe = StableDiffusionInstructPix2PixPipeline.from_pretrained(
+        self.pipe = StableDiffusionUpscalePipeline.from_pretrained(
             pretrained_model_name_or_path=stable_model_path,
             safety_checker=None,
             torch_dtype=torch.float16,
         )
 
     def load_model(
         self,
@@ -110,15 +110,15 @@
         scheduler_name: str = "DDIM",
         images_path_list: List[str] = ["test.png"],
         prompt: List[str] = ["A photo of a cat."],
         negative_prompt: List[str] = ["bad"],
         num_images_per_prompt: int = 1,
         num_inference_steps: int = 20,
         guidance_scale: int = 7.0,
-        image_guidance_scale: float = 1.5,
+        noise_level: int = 20,
         generator_seed: int = 0,
         preprocess_type: str = "Canny",
         resize_type: str = "center_crop_and_resize",
     ):
         """
         This function generates an image based on the given parameters.
 
@@ -160,15 +160,15 @@
 
         generator = self._setup_generator(generator_seed)
 
         output = pipe(
             prompt=prompt,
             control_image=control_image_list,
             image=read_image_list,
-            image_guidance_scale=image_guidance_scale,
+            noise_level=noise_level,
             negative_prompt=negative_prompt,
             num_images_per_prompt=num_images_per_prompt,
             num_inference_steps=num_inference_steps,
             guidance_scale=guidance_scale,
             generator=generator,
         ).images
```

### Comparing `custom_diffusion-0.1.6/custom_diffusion/pipelines/stable_diffusion_text2image.py` & `custom_diffusion-0.1.7/custom_diffusion/pipelines/stable_diffusion_text2image.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.1.6/custom_diffusion/pipelines/stable_diffusion_upscale.py` & `custom_diffusion-0.1.7/custom_diffusion/pipelines/stable_diffusion_img2img.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from typing import List, Optional
 
 import torch
-from diffusers import StableDiffusionUpscalePipeline
+from diffusers import StableDiffusionImg2ImgPipeline
 from PIL import Image
 
-from custom_diffusion.preprocces import preprocces_dicts
 from custom_diffusion.utils.data_utils import center_crop_and_resize
 from custom_diffusion.utils.scheduler_utils import get_scheduler
 
 
-class StableDiffusionUpscalerGenerator:
+class StableDiffusionImg2ImgGenerator:
     """
     A class to handle image generation using stable diffusion and control net models.
     """
 
     def __init__(self):
         self.pipe = None
         self.model_cache = {}
@@ -22,15 +21,15 @@
         """
         This function loads the stable diffusion pipeline.
 
         Args:
         stable_model_path (str): Path to the stable diffusion pipeline.
 
         """
-        self.pipe = StableDiffusionUpscalePipeline.from_pretrained(
+        self.pipe = StableDiffusionImg2ImgPipeline.from_pretrained(
             pretrained_model_name_or_path=stable_model_path,
             safety_checker=None,
             torch_dtype=torch.float16,
         )
 
     def load_model(
         self,
@@ -110,17 +109,16 @@
         scheduler_name: str = "DDIM",
         images_path_list: List[str] = ["test.png"],
         prompt: List[str] = ["A photo of a cat."],
         negative_prompt: List[str] = ["bad"],
         num_images_per_prompt: int = 1,
         num_inference_steps: int = 20,
         guidance_scale: int = 7.0,
-        noise_level: int = 20,
+        strength: float = 0.5,
         generator_seed: int = 0,
-        preprocess_type: str = "Canny",
         resize_type: str = "center_crop_and_resize",
     ):
         """
         This function generates an image based on the given parameters.
 
         Args:
         stable_model_path (str): Path to the stable model.
@@ -138,37 +136,33 @@
         controlnet_conditioning_scale (int): The scale of controlnet conditioning in image generation.
         generator_seed (int): The seed for the random generator.
         preprocess_type (str): The type of preprocessing to apply.
 
         Returns:
         output: The generated image.
         """
-        control_image_list = []
         read_image_list = []
         for image_path in images_path_list:
             read_image = self.load_and_resize_image(
                 image_path=image_path, resize_type=resize_type, height=512, width=512, crop_size=512
             )
-            control_image = preprocces_dicts[preprocess_type](read_image)
-            control_image_list.append(control_image)
             read_image_list.append(read_image)
 
         pipe = self.load_model(
             stable_model_path=stable_model_path,
             controlnet_model_path=controlnet_model_path,
             scheduler_name=scheduler_name,
         )
 
         generator = self._setup_generator(generator_seed)
 
         output = pipe(
             prompt=prompt,
-            control_image=control_image_list,
             image=read_image_list,
-            noise_level=noise_level,
+            strength=strength,
             negative_prompt=negative_prompt,
             num_images_per_prompt=num_images_per_prompt,
             num_inference_steps=num_inference_steps,
             guidance_scale=guidance_scale,
             generator=generator,
         ).images
```

### Comparing `custom_diffusion-0.1.6/custom_diffusion/preprocces.py` & `custom_diffusion-0.1.7/custom_diffusion/preprocces.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.1.6/custom_diffusion/utils/data_utils.py` & `custom_diffusion-0.1.7/custom_diffusion/utils/data_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     grid = Image.new("RGB", size=(cols * w, rows * h))
 
     for i, img in enumerate(imgs):
         grid.paste(img, box=(i % cols * w, i // cols * h))
     return grid
 
 
-def load_images_from_folder(folder, pil_image=True):
+def load_images_from_folder(folder, pil_image=False):
     """
     Loads all .jpg and .png images in a specified folder and returns them as a list of PIL.Image objects.
 
     Parameters:
     folder (str): The path to the folder containing the images.
 
     Returns:
```

### Comparing `custom_diffusion-0.1.6/custom_diffusion/utils/downloads.py` & `custom_diffusion-0.1.7/custom_diffusion/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.1.6/custom_diffusion/utils/model_list.py` & `custom_diffusion-0.1.7/custom_diffusion/utils/model_list.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.1.6/custom_diffusion/utils/scheduler_utils.py` & `custom_diffusion-0.1.7/custom_diffusion/utils/scheduler_utils.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.1.6/custom_diffusion/utils/video_utils.py` & `custom_diffusion-0.1.7/custom_diffusion/utils/video_utils.py`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.1.6/custom_diffusion.egg-info/PKG-INFO` & `custom_diffusion-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: custom-diffusion
-Version: 0.1.6
+Name: custom_diffusion
+Version: 0.1.7
 Summary: Custom Diffusion: Creating Video from Frame Using Multiple Diffusion
 Home-page: https://github.com/kadirnar/Custom-Diffusion
 Author: kadirnar
 License: Apache License 2.0
 Keywords: machine-learning,deep-learning,pytorch,diffusion,diffusion models,controlnet,stable diffusion
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: custom-diffusion Version: 0.1.6 Summary: Custom
+Metadata-Version: 2.1 Name: custom_diffusion Version: 0.1.7 Summary: Custom
 Diffusion: Creating Video from Frame Using Multiple Diffusion Home-page: https:
 //github.com/kadirnar/Custom-Diffusion Author: kadirnar License: Apache License
 2.0 Keywords: machine-learning,deep-learning,pytorch,diffusion,diffusion
 models,controlnet,stable diffusion Platform: UNKNOWN Classifier: Development
 Status :: 5 - Production/Stable Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: Programming Language :: Python :: 3 Classifier:
```

### Comparing `custom_diffusion-0.1.6/custom_diffusion.egg-info/SOURCES.txt` & `custom_diffusion-0.1.7/custom_diffusion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `custom_diffusion-0.1.6/setup.py` & `custom_diffusion-0.1.7/setup.py`

 * *Files identical despite different names*

