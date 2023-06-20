# Comparing `tmp/imgo-2.5.6.tar.gz` & `tmp/imgo-2.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/imgo-2.5.6.tar", last modified: Thu Jul  8 10:17:15 2021, max compression
+gzip compressed data, was "imgo-2.5.7.tar", last modified: Tue Jun 20 16:12:52 2023, max compression
```

## Comparing `imgo-2.5.6.tar` & `imgo-2.5.7.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2021-07-08 10:17:15.000000 imgo-2.5.6/
--rw-r--r--   0 lucbatty   (501) staff       (20)     3300 2021-07-08 10:17:15.000000 imgo-2.5.6/PKG-INFO
--rw-r--r--   0 lucbatty   (501) staff       (20)     2326 2021-07-07 08:41:29.000000 imgo-2.5.6/README.md
-drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2021-07-08 10:17:15.000000 imgo-2.5.6/imgo/
--rw-r--r--   0 lucbatty   (501) staff       (20)        0 2020-09-26 14:01:11.000000 imgo-2.5.6/imgo/__init__.py
--rw-r--r--   0 lucbatty   (501) staff       (20)    50560 2021-07-08 10:15:04.000000 imgo-2.5.6/imgo/augtools.py
--rw-r--r--   0 lucbatty   (501) staff       (20)    89154 2021-07-08 10:15:16.000000 imgo-2.5.6/imgo/uptools.py
-drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2021-07-08 10:17:15.000000 imgo-2.5.6/imgo.egg-info/
--rw-r--r--   0 lucbatty   (501) staff       (20)     3300 2021-07-08 10:17:14.000000 imgo-2.5.6/imgo.egg-info/PKG-INFO
--rw-r--r--   0 lucbatty   (501) staff       (20)      195 2021-07-08 10:17:14.000000 imgo-2.5.6/imgo.egg-info/SOURCES.txt
--rw-r--r--   0 lucbatty   (501) staff       (20)        1 2021-07-08 10:17:14.000000 imgo-2.5.6/imgo.egg-info/dependency_links.txt
--rw-r--r--   0 lucbatty   (501) staff       (20)        5 2021-07-08 10:17:14.000000 imgo-2.5.6/imgo.egg-info/top_level.txt
--rw-r--r--   0 lucbatty   (501) staff       (20)      226 2020-10-23 14:05:03.000000 imgo-2.5.6/pyproject.toml
--rw-r--r--   0 lucbatty   (501) staff       (20)       38 2021-07-08 10:17:15.000000 imgo-2.5.6/setup.cfg
--rw-r--r--   0 lucbatty   (501) staff       (20)      644 2021-07-08 10:15:28.000000 imgo-2.5.6/setup.py
+drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-20 16:12:52.792151 imgo-2.5.7/
+-rw-r--r--   0 lucbatty   (501) staff       (20)     1066 2020-10-24 16:50:48.000000 imgo-2.5.7/LICENSE.txt
+-rw-r--r--   0 lucbatty   (501) staff       (20)     2998 2023-06-20 16:12:52.791507 imgo-2.5.7/PKG-INFO
+-rw-r--r--   0 lucbatty   (501) staff       (20)     2550 2023-06-20 16:09:32.000000 imgo-2.5.7/README.md
+drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-20 16:12:52.786548 imgo-2.5.7/imgo/
+-rw-r--r--   0 lucbatty   (501) staff       (20)        0 2020-09-26 14:01:11.000000 imgo-2.5.7/imgo/__init__.py
+-rw-r--r--   0 lucbatty   (501) staff       (20)    49895 2023-06-20 09:27:56.000000 imgo-2.5.7/imgo/augtools.py
+-rw-r--r--   0 lucbatty   (501) staff       (20)    87279 2023-06-20 09:27:57.000000 imgo-2.5.7/imgo/uptools.py
+drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-20 16:12:52.790588 imgo-2.5.7/imgo.egg-info/
+-rw-r--r--   0 lucbatty   (501) staff       (20)     2998 2023-06-20 16:12:52.000000 imgo-2.5.7/imgo.egg-info/PKG-INFO
+-rw-r--r--   0 lucbatty   (501) staff       (20)      207 2023-06-20 16:12:52.000000 imgo-2.5.7/imgo.egg-info/SOURCES.txt
+-rw-r--r--   0 lucbatty   (501) staff       (20)        1 2023-06-20 16:12:52.000000 imgo-2.5.7/imgo.egg-info/dependency_links.txt
+-rw-r--r--   0 lucbatty   (501) staff       (20)        5 2023-06-20 16:12:52.000000 imgo-2.5.7/imgo.egg-info/top_level.txt
+-rw-r--r--   0 lucbatty   (501) staff       (20)      226 2020-10-23 14:05:03.000000 imgo-2.5.7/pyproject.toml
+-rw-r--r--   0 lucbatty   (501) staff       (20)       38 2023-06-20 16:12:52.792412 imgo-2.5.7/setup.cfg
+-rw-r--r--   0 lucbatty   (501) staff       (20)      652 2023-06-20 16:11:10.000000 imgo-2.5.7/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `imgo-2.5.6/README.md` & `imgo-2.5.7/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,17 @@
-# IMGO
+# imgo
 
 ## Process, Augment, and Balance Image Data
 
+[![PyPI - Version](https://img.shields.io/pypi/v/imgo.svg)](https://pypi.org/project/imgo/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/imgo.svg)](https://pypi.org/project/imgo/)
+[![License: MIT](https://img.shields.io/badge/license-MIT-C06524)](https://github.com/celerygemini/imgo/blob/main/LICENSE)
+
+## 💡 What is it?
+
 This library is designed to facilitate the preprocessing phase of image classification projects in order to get into the fun part: training the models!
 
 ### Features:
 
 Imgo is composed of two modules: **uptools** and **augtools**.
 
 **Uptools** helps to streamline various image data preprocessing tasks, such as:
@@ -28,39 +34,31 @@
  - Save augmented images in class subdirectories
  - Augment entire image datasets
  - Augment training data in place in preparation for machine learning projects
  - Rebalance class sizes by generating new training images
 
 ![imgo_aug_demo](aux/imgo_aug_demo.jpg)
 
-### Installation
-
-It's as easy as `pip install imgo`!
-
-### Quickstart
+## 🛠️ Setup 
 
-Have a look at the demos [here](https://github.com/elbydata/imgo/tree/master/demos)!
+Install it from **PyPI** by running `pip install imgo`.
 
-### Documentation
+### Dependencies 
 
-Documentation is currently available in the form of docstrings.
-
-### Requirements and Dependencies
+The code was written with **Python 3.6**, and it is recommended to run it in a virtual environment. 
+All the required libraries are listed in the `requirements.txt` file in this repo.
 
-Please see the `requirements.txt` file for all requirements and dependencies.
- 
-### Support
+## 🚀 Execution
 
-The source code is available [here](https://github.com/elbydata/imgo/tree/master/imgo).
-Please direct any queries or issues to info@elbydata.com.
+Once the package has been installed, it is simply a case of experimenting with the various classes and functions. For a quickstart, please see the [demo](https://github.com/celerygemini/imgo/tree/master/demos).
 
-### Issues / To do
+## 📝 Documentation
 
-Some functions currently employ ragged arrays which are deprecated in the latest versions of NumPy. This affects all functions that work with non-standard or inconsistent image dimensions.
+Documentation is currently available in the form of docstrings.
 
-### License
+## ⚖️ License
 
 The project is licensed under the MIT license.
 
 ### Acknowledgements
 
 Some of the **augtools** library is built as a wrapper around **Imgaug**, a powerful image augmentation library. For more information, please see https://imgaug.readthedocs.io/en/latest/.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `imgo-2.5.6/imgo/augtools.py` & `imgo-2.5.7/imgo/augtools.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,15 +273,14 @@
         b_sev=None,
         e_sev=None,
         contrast=False,
         sharpness=False,
         fill_mode=None,
         randomize_params=False,
     ):
-
         """
         Constructs all the necessary attributes for the augmenter.
 
         Once initialized, the augmenter applies one or more augmentation
         functions to the image, depending on which keyword arguments are
         given, in a random order. If the batch is randomized (specified
         with the randomize_params argument), the functions will be applied
@@ -414,43 +413,38 @@
             "x_scale": x_scale,
             "y_scale": y_scale,
             "x_shift": x_shift,
             "y_shift": y_shift,
             "clip_limit": clip_limit,
             "pwa_scale": pwa_scale,
         }.items():
-
             if v is None:
                 setattr(self, k, None)
-            elif ((type(v) is tuple) or (type(v) is list)) and len(
-                v
-            ) == 2:
+            elif ((type(v) is tuple) or (type(v) is list)) and len(v) == 2:
                 setattr(self, k, v)
             else:
                 setattr(self, k, None)
 
         for k, v in {
             "h_flip": h_flip,
             "v_flip": v_flip,
             "g_sev": g_sev,
             "b_sev": b_sev,
             "e_sev": e_sev,
         }.items():
-
             if (v is None) or (v == 0):
                 setattr(self, k, None)
             else:
                 setattr(self, k, v)
 
         for k, v in {
             "contrast": contrast,
             "sharpness": sharpness,
             "randomize_params": randomize_params,
         }.items():
-
             if v == True:
                 setattr(self, k, True)
             else:
                 setattr(self, k, False)
 
         if fill_mode is not None:
             if fill_mode in ["edge", "reflect"]:
@@ -474,105 +468,87 @@
         self.f_list = [getattr(self, i) for i in f_names]
 
         self.argno = len(self.f_list)
 
     #     ----------
 
     def details(self):
-
         """
         Prints summary of parameters with which the selfmenter was
         initialized.
         """
 
-        exclude_set = set(
-            ["f_list", "argno", "randomize_params", "fill_mode"]
-        )
+        exclude_set = set(["f_list", "argno", "randomize_params", "fill_mode"])
         param_list = sorted(
             list(set([k for k in vars(self).keys()]) - exclude_set),
             key=lambda f: f.lower(),
         )
         add_list = ["fill_mode", "randomize_params"]
-        print(
-            "Augmenter initialized with the following parameter ranges:"
-        )
-        print(
-            "----------------------------------------------------------"
-        )
+        print("Augmenter initialized with the following parameter ranges:")
+        print("----------------------------------------------------------")
         for i in param_list:
             val = str(vars(self)[i])
             print(f"{i:<20}{val}")
         print("-")
         for i in add_list:
             val = str(vars(self)[i])
             print(f"{i:<20}{val}")
 
     #     ----------
 
     def aug_rotate(self, img, pre_norm=False):
-
         """
         Rotates the image by a random angle within the range given
         (set pre_norm to True if image has been normalized to [0,1]).
         """
 
         if self.rotate_range is not None:
-            rotate = iaa.Affine(
-                rotate=self.rotate_range, mode=self.fill_mode
-            )
+            rotate = iaa.Affine(rotate=self.rotate_range, mode=self.fill_mode)
             if pre_norm:
                 img = (img * 255).astype(np.uint8)
                 rotated_img = (rotate(image=img)) / 255
             else:
                 rotated_img = rotate(image=img)
             return rotated_img
         else:
             return img
 
     #     ----------
 
     def aug_shear(self, img, pre_norm=False):
-
         """
         Shear-transforms the image by a random angle within the range
         given (set pre_norm to True if image has been normalized to
         [0,1]).
         """
 
         if self.shear_range is not None:
-            shear = iaa.Affine(
-                shear=self.shear_range, mode=self.fill_mode
-            )
+            shear = iaa.Affine(shear=self.shear_range, mode=self.fill_mode)
             if pre_norm:
                 img = (img * 255).astype(np.uint8)
                 shear_img = (shear(image=img)) / 255
             else:
                 shear_img = shear(image=img)
             return shear_img
         else:
             return img
 
     #     ----------
 
     def aug_dropout(self, img, pre_norm=False):
-
         """
         Drops a portion of pixel values to zero (set pre_norm to True
         if image has been normalized to [0,1]).
         """
 
         if self.dropout_pair is not None:
             if self.randomize_params == True:
-                drop_1 = (
-                    np.random.randint(0, self.dropout_pair[0] * 100)
-                    / 100
-                )
+                drop_1 = np.random.randint(0, self.dropout_pair[0] * 100) / 100
                 drop_2 = (
-                    np.random.randint(self.dropout_pair[1] * 100, 100)
-                    / 100
+                    np.random.randint(self.dropout_pair[1] * 100, 100) / 100
                 )
                 dropout = iaa.CoarseDropout(drop_1, size_percent=drop_2)
             else:
                 dropout = iaa.CoarseDropout(
                     self.dropout_pair[0],
                     size_percent=self.dropout_pair[1],
                 )
@@ -584,15 +560,14 @@
             return dropout_img
         else:
             return img
 
     #     ----------
 
     def aug_x_scale(self, img, pre_norm=False):
-
         """
         Scales (squashes or stretches) the image on the x-axis by a
         random amount within the range given (set pre_norm to True
         if image has been normalized to [0,1]).
         """
 
         if self.x_scale is not None:
@@ -605,15 +580,14 @@
             return x_scale_img
         else:
             return img
 
     #     ----------
 
     def aug_y_scale(self, img, pre_norm=False):
-
         """
         Scales (squashes or stretches) the image on the y-axis by a
         random amount within the range given (set pre_norm to True
         if image has been normalized to [0,1]).
         """
 
         if self.y_scale is not None:
@@ -626,61 +600,54 @@
             return y_scale_img
         else:
             return img
 
     #     ----------
 
     def aug_x_shift(self, img, pre_norm=False):
-
         """
         Shifts the image on the x-axis by a random amount within the
         range given (set pre_norm to True if image has been
         normalized to [0,1]).
         """
 
         if self.x_shift is not None:
-            x_shift = iaa.TranslateX(
-                percent=self.x_shift, mode=self.fill_mode
-            )
+            x_shift = iaa.TranslateX(percent=self.x_shift, mode=self.fill_mode)
             if pre_norm:
                 img = (img * 255).astype(np.uint8)
                 x_shift_img = (x_shift(image=img)) / 255
             else:
                 x_shift_img = x_shift(image=img)
             return x_shift_img
         else:
             return img
 
     #     ----------
 
     def aug_y_shift(self, img, pre_norm=False):
-
         """
         Shifts the image on the y-axis by a random amount within the
         range given (set pre_norm to True if image has been
         normalized to [0,1]).
         """
 
         if self.y_shift is not None:
-            y_shift = iaa.TranslateY(
-                percent=self.y_shift, mode=self.fill_mode
-            )
+            y_shift = iaa.TranslateY(percent=self.y_shift, mode=self.fill_mode)
             if pre_norm:
                 img = (img * 255).astype(np.uint8)
                 y_shift_img = (y_shift(image=img)) / 255
             else:
                 y_shift_img = y_shift(image=img)
             return y_shift_img
         else:
             return img
 
     #     ----------
 
     def aug_clahe(self, img, pre_norm=False):
-
         """
         Applies a CLAH equalization using a random clip limit within
         the range given (set pre_norm to True if image has been
         normalized to [0,1]).
         """
 
         if self.clip_limit is not None:
@@ -693,38 +660,34 @@
             return clahe_img
         else:
             return img
 
     #     ----------
 
     def aug_pwa(self, img, pre_norm=False):
-
         """
         Shifts local pixel areas by a random amount within the range
         given (set pre_norm to True if image has been normalized
         to [0,1]).
         """
 
         if self.pwa_scale is not None:
-            pwa = iaa.PiecewiseAffine(
-                scale=self.pwa_scale, mode=self.fill_mode
-            )
+            pwa = iaa.PiecewiseAffine(scale=self.pwa_scale, mode=self.fill_mode)
             if pre_norm:
                 img = (img * 255).astype(np.uint8)
                 pwa_img = (pwa(image=img)) / 255
             else:
                 pwa_img = pwa(image=img)
             return pwa_img
         else:
             return img
 
     #     ----------
 
     def aug_h_flip(self, img, pre_norm=False):
-
         """
         Flips a random subset of images horizontally (set pre_norm
         to True if image has been normalized to [0,1]).
         """
 
         if self.h_flip is not None:
             h_flip = iaa.Fliplr(self.h_flip)
@@ -736,15 +699,14 @@
             return h_flip_img
         else:
             return img
 
     #     ----------
 
     def aug_v_flip(self, img, pre_norm=False):
-
         """
         Flipts a random subset of images vertically (set pre_norm
         to True if image has been normalized to [0,1]).
         """
 
         if self.v_flip is not None:
             v_flip = iaa.Flipud(self.v_flip)
@@ -756,15 +718,14 @@
             return v_flip_img
         else:
             return img
 
     #     ----------
 
     def aug_g_noise(self, img, pre_norm=False):
-
         """
         Adds Gaussian noise to the image (set pre_norm to True if
         image has been normalized to [0,1]).
         """
 
         if self.g_sev is not None:
             rand_sev = np.random.randint(self.g_sev + 1)
@@ -772,17 +733,15 @@
                 if rand_sev == 0:
                     g_noise = None
                 else:
                     g_noise = iaa.imgcorruptlike.GaussianNoise(
                         severity=rand_sev
                     )
             else:
-                g_noise = iaa.imgcorruptlike.GaussianNoise(
-                    severity=self.g_sev
-                )
+                g_noise = iaa.imgcorruptlike.GaussianNoise(severity=self.g_sev)
             if g_noise is None:
                 return img
             else:
                 if pre_norm:
                     img = (img * 255).astype(np.uint8)
                     g_noise_img = (g_noise(image=img)) / 255
                 else:
@@ -790,15 +749,14 @@
                 return g_noise_img
         else:
             return img
 
     #     ----------
 
     def aug_brightness(self, img, pre_norm=False):
-
         """
         Adjusts brightness of the image (set pre_norm to True if
         image has been normalized to [0,1]).
         """
 
         if self.b_sev is not None:
             rand_sev = np.random.randint(self.b_sev + 1)
@@ -806,17 +764,15 @@
                 if rand_sev == 0:
                     brightness = None
                 else:
                     brightness = iaa.imgcorruptlike.Brightness(
                         severity=rand_sev
                     )
             else:
-                brightness = iaa.imgcorruptlike.Brightness(
-                    severity=self.b_sev
-                )
+                brightness = iaa.imgcorruptlike.Brightness(severity=self.b_sev)
             if brightness is None:
                 return img
             else:
                 if pre_norm:
                     img = (img * 255).astype(np.uint8)
                     brightness_img = (brightness(image=img)) / 255
                 else:
@@ -824,15 +780,14 @@
                 return brightness_img
         else:
             return img
 
     #     ----------
 
     def aug_elastic(self, img, pre_norm=False):
-
         """
         Applies elastic transformation to the image (set pre_norm
         to True if image has been normalized to [0,1]).
         """
 
         if self.e_sev is not None:
             rand_sev = np.random.randint(self.e_sev + 1)
@@ -858,15 +813,14 @@
                 return elastic_img
         else:
             return img
 
     #     ----------
 
     def aug_contrast(self, img, pre_norm=False):
-
         """
         Adusts contrast to a random subset of images (set pre_norm
         to True if image has been normalized to [0,1]).
         """
 
         if self.contrast == True:
             contrast = iaa.pillike.EnhanceContrast()
@@ -892,15 +846,14 @@
             return contrast_img
         else:
             return img
 
     #     ----------
 
     def aug_sharpness(self, img, pre_norm=False):
-
         """
         Adjusts sharpness to a random subset of images (set pre_norm
         to True if image has been normalized to [0,1]).
         """
 
         if self.sharpness == True:
             sharpness = iaa.pillike.EnhanceSharpness()
@@ -926,15 +879,14 @@
             return sharpness_img
         else:
             return img
 
     #     ----------
 
     def simple_augment(self, img, order=None, pre_norm=False):
-
         """
         Performs the augmentations (for which a parameter was provided) in
         a particular order.
 
         Arguments:
             img (array): image to augment.
 
@@ -967,15 +919,14 @@
             return outp / 255
         else:
             return outp
 
     #     ----------
 
     def random_augment(self, img, full_set=True, pre_norm=False):
-
         """
         Performs the augmentations (for which a parameter was provided) in
         a random order.
 
         Arguments:
             img (array): image to augment.
 
@@ -1012,18 +963,15 @@
         if pre_norm:
             return outp / 255
         else:
             return outp
 
     #     ----------
 
-    def display(
-        self, img, n_rows, n_cols, augment_type=None, order=None
-    ):
-
+    def display(self, img, n_rows, n_cols, augment_type=None, order=None):
         """
         Applies the Augmenter to an input image according to the
         parameters given, in order to visualize augmentations.
 
         Arguments:
             img (array): image to augment.
             -
@@ -1087,15 +1035,14 @@
         source,
         n_rows,
         n_cols,
         augment_type=None,
         order=None,
         pre_norm=False,
     ):
-
         """
         Fetches a sample image from a collection of images located in
         a main directory or an uptools.Image_Dataset and applies the
         Augmenter according to the parameters given, in order to
         visualize augmentations prior to running on multiple images.
 
         Arguments:
@@ -1138,27 +1085,24 @@
             Only relevant if using "path" mode. Defaults to False.
 
         Returns:
             Visualization of augmented image.
         """
 
         if source_type == "path":
-
             from imgo.uptools import img_to_df
 
             df = img_to_df(source)
             sample = df.sample()
             img = imageio.imread(sample.iloc[0]["image"])
 
         elif source_type == "ids":
             if source.shadow["data"][0] is None:
                 img = source.shadow["train"][0][
-                    np.random.randint(
-                        source.shadow["train"][0].shape[0]
-                    )
+                    np.random.randint(source.shadow["train"][0].shape[0])
                 ]
             else:
                 img = source.shadow["data"][0][
                     np.random.randint(source.shadow["data"][0].shape[0])
                 ]
         else:
             raise Exception(
@@ -1202,15 +1146,14 @@
         augment_type=None,
         order=None,
         class_selection=None,
         number=None,
         size=None,
         save=False,
     ):
-
         """
         Fetches all the images from a collection of images located in a
         main directory and applies a series of random augmentations to
         them according to the parameters given to an (initialized)
         Augmenter object. Depending on the parameters given, a subset of
         the images can be augmented, or the entire dataset can be
         augmented.
@@ -1288,29 +1231,25 @@
                     f"Class selection must be a list; {type(class_selection)} given."
                 )
             else:
                 df = df.loc[df["class"].isin(class_selection)]
 
         if len(df.loc[df["class"] == "no_class"]) != 0:
             if int(
-                df.loc[df["class"] == "no_class"][
-                    "class"
-                ].value_counts()
+                df.loc[df["class"] == "no_class"]["class"].value_counts()
             ) == len(df):
                 no_class = True
 
         class_list = list(df["class"].unique())
         for c in class_list:
             class_arrays = read_img_df(df, class_name=c)
             all_class_arrays.append(class_arrays)
 
         if (number is not None) and (size is not None):
-            raise Exception(
-                "Cannot accept both number and size arguments."
-            )
+            raise Exception("Cannot accept both number and size arguments.")
 
         elif (number is not None) and (size is None):
             for a in all_class_arrays:
                 to_augment = np.random.randint(a.shape[0], size=number)
                 all_aug_indices.append(to_augment)
 
         elif (number is None) and (size is not None):
@@ -1350,17 +1289,15 @@
                     total=len(all_aug_indices[0]),
                 ):
                     if augment_type == "simple":
                         aug_img = self.simple_augment(
                             all_class_arrays[0][j], order=order
                         )
                     else:
-                        aug_img = self.random_augment(
-                            all_class_arrays[0][j]
-                        )
+                        aug_img = self.random_augment(all_class_arrays[0][j])
                     imageio.imwrite(f"{r}/aug_{i+1}.jpg", aug_img)
                     aug_imgs.append(aug_img)
                 print("Augmented images saved successfully.")
 
             else:
                 for x in range(len(all_class_arrays)):
                     for i, j in tqdm(
@@ -1390,17 +1327,15 @@
                     total=len(all_aug_indices[0]),
                 ):
                     if augment_type == "simple":
                         aug_img = self.simple_augment(
                             all_class_arrays[0][j], order=order
                         )
                     else:
-                        aug_img = self.random_augment(
-                            all_class_arrays[0][j]
-                        )
+                        aug_img = self.random_augment(all_class_arrays[0][j])
                     aug_imgs.append(aug_img)
 
             else:
                 for x in range(len(all_class_arrays)):
                     for i, j in tqdm(
                         enumerate(all_aug_indices[x]),
                         total=len(all_aug_indices[x]),
```

### Comparing `imgo-2.5.6/imgo/uptools.py` & `imgo-2.5.7/imgo/uptools.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,14 @@
 from sklearn.model_selection import train_test_split
 from send2trash import send2trash
 
 # ------------------------------------------------------------------------
 
 
 def get_class_names(base_path):
-
     """
     Fetches class names from subdirectories in the directory given as the
     base path.
 
     Arguments:
         base_path (str): path to the directory containing images or class
         subdirectories.
@@ -180,15 +179,14 @@
     return class_list
 
 
 # ------------------------------------------------------------------------
 
 
 def img_to_df(base_path):
-
     """
     Fetches images and class names from subdirectories in the directory
     given as the base path and returns a DataFrame.
 
     Arguments:
         base_path (str): path to the directory containing images or class
         subdirectories.
@@ -228,15 +226,14 @@
         return df
 
 
 # ------------------------------------------------------------------------
 
 
 def display_img_df(df, batch_no, batch_size, n_rows, n_cols):
-
     """
     Displays images contained in an x-by-2 DataFrame (where column 0 is
     the image path, column 1 is the class name, and x is the number of
     images).
 
     Arguments:
         df (pandas-DataFrame): x-by-2 DataFrame (where column 0 is the
@@ -308,15 +305,14 @@
     plt.show()
 
 
 # ------------------------------------------------------------------------
 
 
 def read_img_df(df, img_scale=None, class_name=None, save=False):
-
     """
     Reads images contained in an x-by-2 DataFrame (where column 0 is the
     image path, column 1 is the class name, and x is the number of
     images).
 
     Arguments:
         df (pandas-DataFrame): x-by-2 DataFrame (where column 0 is the
@@ -362,19 +358,16 @@
             label = j[1]
         label_list.append(label)
     img_array = np.array(img_list)
     label_array = np.array(label_list)
 
     if save:
         if img_scale == None:
-            raise Exception(
-                "Cannot save images with inconsistent dimensions."
-            )
+            raise Exception("Cannot save images with inconsistent dimensions.")
         else:
-
             my_path = "imgo_output/uptools/preprocessing"
 
             r = None
             for i in my_path.split("/"):
                 if r == None:
                     if not os.path.exists(i):
                         os.mkdir(i)
@@ -391,15 +384,14 @@
     return img_array
 
 
 # ------------------------------------------------------------------------
 
 
 def one_hot_encode(y_data, class_list, save=False):
-
     """
     One-hot encodes list of class labels.
 
     Note that the one-hot encoded data returned will be based on the
     class_list given sorted in alphabetical order.
 
     Arguments:
@@ -417,17 +409,15 @@
         y_data (numpy-array): one-hot encoded class label data as numpy-
         array.
     """
 
     y_list = []
     labels = []
     if type(class_list) is not list:
-        raise Exception(
-            f"class_list must be a list; {type(class_list)} given."
-        )
+        raise Exception(f"class_list must be a list; {type(class_list)} given.")
     else:
         classes = sorted(list(set(class_list)), key=lambda f: f.lower())
         class_no = len(classes)
 
     for i in y_data:
         ohe_init = np.zeros(class_no)
         label = i
@@ -435,15 +425,14 @@
         ohe_init[classes.index(label)] = 1
         ohe_label = ohe_init
         y_list.append(ohe_label)
 
     y_data = np.array(y_list)
 
     if save:
-
         my_path = "imgo_output/uptools/preprocessing"
 
         r = None
         for i in my_path.split("/"):
             if r == None:
                 if not os.path.exists(i):
                     os.mkdir(i)
@@ -460,15 +449,14 @@
     return y_data
 
 
 # ------------------------------------------------------------------------
 
 
 def auto_rescale(img, dim):
-
     """
     Rescales image to a square of n-by-n pixels, where n is the integer
     value given by the 'dim' argument. Rescaling is performed with cv2
     'inter cubic' interpolation if the original dimensions are smaller than
     the target dimensions, and cv2 'inter area' interpolation if the
     original dimensions are greater than the target dimensions.
 
@@ -483,33 +471,28 @@
     """
 
     raw_dims = np.max(img.shape)
 
     scale = (dim, dim)
 
     if raw_dims < dim:
-        scaled_img = cv2.resize(
-            img, scale, interpolation=cv2.INTER_CUBIC
-        )
+        scaled_img = cv2.resize(img, scale, interpolation=cv2.INTER_CUBIC)
     else:
-        scaled_img = cv2.resize(
-            img, scale, interpolation=cv2.INTER_AREA
-        )
+        scaled_img = cv2.resize(img, scale, interpolation=cv2.INTER_AREA)
 
     if len(scaled_img.shape) == 2:
         scaled_img = np.expand_dims(scaled_img, 2)
 
     return scaled_img
 
 
 # ------------------------------------------------------------------------
 
 
 def threshold_rescale(img, lower=None, upper=None):
-
     """
     Rescales image to a square of n-by-n pixels if the square root of the
     product of the image dimensions are lower or higher than the
     respective threshold values given by the 'lower' and 'upper' arguments.
     Rescaling is performed with cv2 'inter cubic' interpolation if the
     original dimensions are smaller than the target dimensions, and cv2
     'inter area' interpolation if the original dimensions are greater than
@@ -574,15 +557,14 @@
     rescale_mode,
     dim=None,
     lower=None,
     upper=None,
     class_selection=None,
     save=False,
 ):
-
     """
     Fetches images and class names from subdirectories in the directory
     given as the base path and rescales the images using either the
     'auto_rescale' or the 'threshold_rescale' function, with the option
     to save the rescaled images in place of the original images.
 
     Arguments:
@@ -613,57 +595,49 @@
     Returns:
         X (numpy-array): images in array form (if 'save' is False).
         -
         y (numpy-array): one-hot encoded label data (if 'save' is False).
     """
 
     if rescale_mode not in ["auto", "threshold"]:
-        raise Exception(
-            "Choose valid rescale mode: 'auto' or 'threshold'."
-        )
+        raise Exception("Choose valid rescale mode: 'auto' or 'threshold'.")
 
     df = img_to_df(base_path)
     scaled_imgs = []
     scaled_imgs_labels = []
 
     if class_selection:
         if type(class_selection) is not list:
             raise Exception(
                 f"Class selection must be a list; {type(class_selection)} given."
             )
         else:
             df = df.loc[df["class"].isin(class_selection)]
 
-    class_list = sorted(
-        list(df["class"].unique()), key=lambda f: f.lower()
-    )
+    class_list = sorted(list(df["class"].unique()), key=lambda f: f.lower())
 
     for i, j in tqdm(df.iterrows(), total=len(df)):
-
         img = imageio.imread(j[0])
         if rescale_mode == "auto":
             scaled_img = auto_rescale(img, dim)
         elif rescale_mode == "threshold":
-            scaled_img = threshold_rescale(
-                img, lower=lower, upper=upper
-            )
+            scaled_img = threshold_rescale(img, lower=lower, upper=upper)
         else:
             scaled_img = img
 
         if len(scaled_img.shape) == 2:
             scaled_img = np.expand_dims(scaled_img, 2)
 
         if save:
             imageio.imwrite(j[0], scaled_img)
         else:
             scaled_imgs.append(scaled_img)
             scaled_imgs_labels.append(j[1])
 
     if not save:
-
         X = np.array(scaled_imgs)
         y = one_hot_encode(scaled_imgs_labels, class_list)
 
         return X, y
 
 
 # ------------------------------------------------------------------------
@@ -786,15 +760,14 @@
         img_scale,
         pre_norm=False,
         pre_std=False,
         normalize=False,
         standardize=False,
         manual_classes=None,
     ):
-
         """
         Constructs all the necessary attributes for the dataset.
 
         Arguments:
             base_path (str): path to the directory containing images or
             class subdirectories.
             -
@@ -839,17 +812,15 @@
         """
 
         self.base_path = base_path
 
         if mode in ["imgs", "np", "h5"]:
             self.mode = mode
         else:
-            raise Exception(
-                "Must select valid mode: 'imgs', 'np', or 'h5'."
-            )
+            raise Exception("Must select valid mode: 'imgs', 'np', or 'h5'.")
 
         if type(img_scale) is int:
             rescale_dims = img_scale
         else:
             raise Exception(
                 f"'img_scale' argument must be integer, {type(img_scale)} given."
             )
@@ -904,78 +875,61 @@
             "train": [None, None],
             "val": [None, None],
             "test": [None, None],
             "data": [None, None],
         }
 
         if (self.mode == "np") or (self.mode == "h5"):
-
             file_list = []
             for r, d, f in os.walk(base_path):
                 for i in f:
                     if not i.startswith("."):
                         file_list.append(
                             [i, os.path.relpath(os.path.join(r, i))]
                         )
 
             for file in file_list:
                 if file[0].lower().endswith(".npz"):
                     for k, v in combo_sets.items():
                         if file[0].lower().startswith(f"x_{k}".lower()):
-                            data_load = np.load(
-                                file[1], allow_pickle=True
-                            )
-                            combo_sets[k][0] = data_load[
-                                data_load.files[0]
-                            ]
-                        elif (
-                            file[0].lower().startswith(f"y_{k}".lower())
-                        ):
-                            data_load = np.load(
-                                file[1], allow_pickle=True
-                            )
-                            combo_sets[k][1] = data_load[
-                                data_load.files[0]
-                            ]
+                            data_load = np.load(file[1], allow_pickle=True)
+                            combo_sets[k][0] = data_load[data_load.files[0]]
+                        elif file[0].lower().startswith(f"y_{k}".lower()):
+                            data_load = np.load(file[1], allow_pickle=True)
+                            combo_sets[k][1] = data_load[data_load.files[0]]
 
                 elif file[0].lower().endswith(".npy"):
                     for k, v in combo_sets.items():
                         if file[0].lower().startswith(f"x_{k}".lower()):
                             combo_sets[k][0] = np.load(
                                 file[1], allow_pickle=True
                             )
-                        elif (
-                            file[0].lower().startswith(f"y_{k}".lower())
-                        ):
+                        elif file[0].lower().startswith(f"y_{k}".lower()):
                             combo_sets[k][1] = np.load(
                                 file[1], allow_pickle=True
                             )
 
                 elif file[0].lower().endswith(".h5"):
                     for k, v in combo_sets.items():
                         if file[0].lower().startswith(f"x_{k}".lower()):
                             with h5py.File(f"{file[1]}", "r") as hf:
                                 combo_sets[k][0] = hf[f"X_{k}"][:]
-                        elif (
-                            file[0].lower().startswith(f"y_{k}".lower())
-                        ):
+                        elif file[0].lower().startswith(f"y_{k}".lower()):
                             with h5py.File(f"{file[1]}", "r") as hf:
                                 combo_sets[k][1] = hf[f"y_{k}"][:]
 
                 else:
                     raise Exception(
                         "No valid '.npy', '.npz', or '.h5' files identified."
                     )
 
             if class_list_pending:
                 y_shapes = {}
                 for v in [
-                    v
-                    for k, v in combo_sets.items()
-                    if (v[1] is not None)
+                    v for k, v in combo_sets.items() if (v[1] is not None)
                 ]:
                     y_shapes[k] = v[1].shape[1]
                 if len(set(y_shapes.values())) == 1:
                     clist = []
                     self.class_no = list(set(y_shapes.values()))[0]
                     c = str(0) * len(str(self.class_no))
                     for i in range(1, self.class_no + 1):
@@ -1016,29 +970,26 @@
                     img = img_data
                 X_list.append(img)
 
             combo_sets["data"][0] = np.array(X_list)
             combo_sets["data"][1] = np.array(y_list)
 
         self.split = int(
-            len([1 for k, v in combo_sets.items() if v[0] is not None])
-            - 1
+            len([1 for k, v in combo_sets.items() if v[0] is not None]) - 1
         )
 
         x_eqdims = []
         for k, v in combo_sets.items():
             if v[0] is not None:
-                if (
-                    (len(v[0].shape) == 4) or (len(v[0].shape) == 3)
-                ) and (v[0].shape[1] == v[0].shape[2]):
+                if ((len(v[0].shape) == 4) or (len(v[0].shape) == 3)) and (
+                    v[0].shape[1] == v[0].shape[2]
+                ):
                     x_eqdims.append(v[0].shape[1])
 
-        if (len(set(x_eqdims)) == 1) and (
-            len(x_eqdims) - 1 == self.split
-        ):
+        if (len(set(x_eqdims)) == 1) and (len(x_eqdims) - 1 == self.split):
             self.dims = (list(set(x_eqdims))[0], list(set(x_eqdims))[0])
         else:
             self.dims = "various"
 
         if pre_norm and pre_std:
             raise Exception(
                 "Cannot expand data if both pre-normalized and pre-standardized."
@@ -1051,17 +1002,15 @@
         elif (not pre_norm) and pre_std:
             if self.dims == "various":
                 raise Exception(
                     "Cannot expand data if image dimensions are not the same."
                 )
             else:
                 if self.split == 0:
-                    raise Exception(
-                        "Cannot de-standardize unsplit data."
-                    )
+                    raise Exception("Cannot de-standardize unsplit data.")
                     self.expand = None
                 else:
                     self.expand = "de_std"
         else:
             self.expand = None
 
         X_sets = {"train": [], "val": [], "test": [], "data": []}
@@ -1071,43 +1020,40 @@
         for k, v in X_sets.items():
             if combo_sets[k][0] is not None:
                 for i in tqdm(
                     np.arange(combo_sets[k][0].shape[0]),
                     total=combo_sets[k][0].shape[0],
                     desc=f"Processing X_{k}",
                 ):
-
                     if self.expand is not None:
                         if self.expand == "de_std":
                             img_min = np.min(combo_sets[k][0][i])
                             img_max = np.max(combo_sets[k][0][i])
                             raw_img = (
                                 ((combo_sets[k][0][i] - img_min) * 255)
                                 / (img_max - img_min)
                             ).astype(np.uint8)
                             clean_img = np.clip(raw_img, 0, 255).astype(
                                 np.uint8
                             )
                         elif self.expand == "de_norm":
-                            raw_img = (
-                                combo_sets[k][0][i] * 255
-                            ).astype(np.uint8)
+                            raw_img = (combo_sets[k][0][i] * 255).astype(
+                                np.uint8
+                            )
                             clean_img = np.clip(raw_img, 0, 255).astype(
                                 np.uint8
                             )
                         else:
                             raw_img = combo_sets[k][0][i]
                             clean_img = np.clip(raw_img, 0, 255).astype(
                                 np.uint8
                             )
                     else:
                         raw_img = combo_sets[k][0][i]
-                        clean_img = np.clip(raw_img, 0, 255).astype(
-                            np.uint8
-                        )
+                        clean_img = np.clip(raw_img, 0, 255).astype(np.uint8)
 
                     if self.mode == "imgs":
                         img = clean_img
 
                     else:
                         if rescale_dims:
                             img = auto_rescale(clean_img, rescale_dims)
@@ -1241,15 +1187,14 @@
             )
 
         print("Image_Datset initialized successfully.")
 
     #     ----------
 
     def details(self, plot=False):
-
         """
         Prints summary details of Image_Dataset object, or displays the
         details as a visualization if kwarg 'plot' is given as True.
         """
 
         labels = {}
         labs_nums = {}
@@ -1289,15 +1234,14 @@
             "splits": splits,
             "images_per_class": imgs_per_class,
             "image_shape": self.img_shape,
             "pixel_values": val_ranges,
         }
 
         if plot:
-
             ldf = pd.DataFrame(labs_nums, columns=df_cols).fillna(0)
             ldf = ldf.iloc[::-1]
 
             plt.rcParams["font.family"] = "sans-serif"
             plt.rcParams["font.sans-serif"] = "Helvetica"
             plt.rcParams["axes.edgecolor"] = "#333F4B"
             plt.rcParams["axes.linewidth"] = 0.8
@@ -1331,41 +1275,35 @@
                 ax.legend(bbox_to_anchor=(1, 0.5))
             ax.spines["top"].set_color("none")
             ax.spines["right"].set_color("none")
 
             plt.show()
 
         else:
-
             print("Image_Dataset details")
             print("---------------------")
             for k, v in {
-                i: ds_dict[i]
-                for i in ds_dict
-                if i != "images_per_class"
+                i: ds_dict[i] for i in ds_dict if i != "images_per_class"
             }.items():
                 print(f"{k:<20}{v}\n---")
             print("images_per_class\n-")
             for k, v in ds_dict["images_per_class"].items():
                 print(f"{k:<20}{v}\n-")
             if self.split != 0:
                 totals = {}
                 for c in self.class_list:
                     c_total = []
                     for k, v in ds_dict["images_per_class"].items():
-                        c_total.append(
-                            ds_dict["images_per_class"][k][c]
-                        )
+                        c_total.append(ds_dict["images_per_class"][k][c])
                         totals[c] = sum(c_total)
                 print(f"{'totals':<20}{totals}")
 
     #     ----------
 
     def map_classes(self, class_list):
-
         """
         Maps class names from a given list of class names.
         """
 
         if type(class_list) is list:
             new_list = sorted(
                 [str(i) for i in class_list], key=lambda f: f.lower()
@@ -1382,15 +1320,14 @@
             raise Exception(
                 f"'class_list' argument must be list, {type(class_list)} given."
             )
 
     #     ----------
 
     def normalize(self):
-
         """
         Normalizes pixel values to range [0,1].
         """
 
         if self.reduce == "norm":
             raise Exception("Data has already been normalized.")
         elif self.reduce == "std":
@@ -1412,15 +1349,14 @@
             self.max_pv = self.max_pv / 255
             self.reduce = "norm"
             print("Normalization complete.")
 
     #     ----------
 
     def standardize(self):
-
         """
         Standardizes pixel values using the mean and standard deviation of
         the training subset (note that the dataset must be split in order
         to standardize).
         """
 
         if self.reduce == "std":
@@ -1434,18 +1370,15 @@
                 raise Exception(
                     "Cannot standardize data if image dimensions are not the same."
                 )
             elif self.split == 0:
                 raise Exception("Cannot standardize unsplit data.")
             else:
                 print("Standardizing...")
-                self.mu = (
-                    np.sum(subsets["train"][0])
-                    / subsets["train"][0].size
-                )
+                self.mu = np.sum(subsets["train"][0]) / subsets["train"][0].size
                 self.sigma = np.sqrt(
                     np.sum((subsets["train"][0] - self.mu) ** 2)
                     / subsets["train"][0].size
                 )
                 for k, v in subsets.items():
                     if v[0] is None:
                         setattr(self, f"X_{k}", None)
@@ -1464,15 +1397,14 @@
                 self.max_pv = (self.max_pv - self.mu) / self.sigma
                 self.reduce = "std"
                 print("Standardization complete.")
 
     #     ----------
 
     def data_split(self, split_ratio, seed=None, stratify=False):
-
         """
         Splits the Image_Dataset object into training and testing, and/or
         validation subsets.
 
         Note that this method is built using Scikit-Learn's
         train_test_split. For more information see:
         https://scikit-learn.org/stable/modules/classes.html#
@@ -1499,22 +1431,17 @@
             and 'y_train', 'X_test' and 'y_test' (and 'X_val' and 'y_val'
             if 3 values passed into the 'split_ratio' argument) attributes
             of the Image_Dataset object. None as 'X_data' and 'y_data'
             attributes of the Image_Dataset object.
         """
 
         if self.split != 0:
-            raise Exception(
-                "Cannot split dataset that has already been split."
-            )
+            raise Exception("Cannot split dataset that has already been split.")
         else:
-
-            if (type(split_ratio) is list) or (
-                type(split_ratio) is tuple
-            ):
+            if (type(split_ratio) is list) or (type(split_ratio) is tuple):
                 split_ratio = [np.round(i, 2) for i in split_ratio]
                 if sum(split_ratio) == 1:
                     print("Splitting...")
                     if len(split_ratio) == 3:
                         if stratify:
                             (
                                 self.shadow["train"][0],
@@ -1535,17 +1462,15 @@
                                 self.shadow["test"][0],
                                 self.shadow["val"][1],
                                 self.shadow["test"][1],
                             ) = train_test_split(
                                 Xtv,
                                 ytv,
                                 test_size=split_ratio[2]
-                                / round(
-                                    split_ratio[1] + split_ratio[2], 2
-                                ),
+                                / round(split_ratio[1] + split_ratio[2], 2),
                                 stratify=ytv,
                                 random_state=seed,
                             )
                         else:
                             (
                                 self.shadow["train"][0],
                                 Xtv,
@@ -1564,17 +1489,15 @@
                                 self.shadow["test"][0],
                                 self.shadow["val"][1],
                                 self.shadow["test"][1],
                             ) = train_test_split(
                                 Xtv,
                                 ytv,
                                 test_size=split_ratio[2]
-                                / round(
-                                    split_ratio[1] + split_ratio[2], 2
-                                ),
+                                / round(split_ratio[1] + split_ratio[2], 2),
                                 random_state=seed,
                             )
                         del Xtv
                         del ytv
                         self.shadow["data"][0] = None
                         self.shadow["data"][1] = None
                         self.split = 2
@@ -1611,17 +1534,15 @@
                         self.shadow["val"][1] = None
                         self.split = 1
                     else:
                         raise Exception(
                             "'split_ratio' argument must be list or tuple of 2 or 3 floats."
                         )
                 else:
-                    raise Exception(
-                        "'split_ratio' argument must sum to 1."
-                    )
+                    raise Exception("'split_ratio' argument must sum to 1.")
             else:
                 raise Exception(
                     f"'split_ratio' argument must be list or tuple, {type(split_ratio)} given."
                 )
 
             subsets = self.shadow
 
@@ -1629,16 +1550,15 @@
                 if self.dims == "various":
                     raise Exception(
                         "Cannot standardize data if image dimensions are not the same."
                     )
                 else:
                     print("Standardizing...")
                     self.mu = (
-                        np.sum(subsets["train"][0])
-                        / subsets["train"][0].size
+                        np.sum(subsets["train"][0]) / subsets["train"][0].size
                     )
                     self.sigma = np.sqrt(
                         np.sum((subsets["train"][0] - self.mu) ** 2)
                         / subsets["train"][0].size
                     )
                     for k, v in subsets.items():
                         if v[0] is None:
@@ -1688,53 +1608,38 @@
                 print(
                     "Data sucessfully split into training, validation, and testing subsets."
                 )
 
     #     ----------
 
     def data_merge(self):
-
         """
         Merges a split Image_Dataset object into a single dataset.
         Yields full X and y data arrays as 'X_data' and 'y_data'
         attributes of the Image_Dataset object, and None as the 'X_train',
         'y_train', 'X_val', 'y_val', 'X_test', and 'y_test' attributes of
         the Image_Dataset object.
         """
 
         if self.split == 0:
-            raise Exception(
-                "Cannot merge dataset that has not been split."
-            )
+            raise Exception("Cannot merge dataset that has not been split.")
         else:
             print("Merging...")
             x_merge = [
-                v[0]
-                for k, v in self.shadow.items()
-                if (v[0] is not None)
+                v[0] for k, v in self.shadow.items() if (v[0] is not None)
             ]
             y_merge = [
-                v[1]
-                for k, v in self.shadow.items()
-                if (v[1] is not None)
+                v[1] for k, v in self.shadow.items() if (v[1] is not None)
             ]
             try:
                 self.shadow["data"][0] = np.concatenate(
-                    [
-                        v[0]
-                        for k, v in self.shadow.items()
-                        if (v[0] is not None)
-                    ]
+                    [v[0] for k, v in self.shadow.items() if (v[0] is not None)]
                 )
                 self.shadow["data"][1] = np.concatenate(
-                    [
-                        v[1]
-                        for k, v in self.shadow.items()
-                        if (v[1] is not None)
-                    ]
+                    [v[1] for k, v in self.shadow.items() if (v[1] is not None)]
                 )
             except:
                 merge_x_listwise = []
                 merge_y_listwise = []
                 for i in x_merge:
                     for x in np.arange(i.shape[0]):
                         merge_x_listwise.append(i[x])
@@ -1754,33 +1659,31 @@
 
             if self.reduce == "std":
                 if self.dims == "various":
                     raise Exception(
                         "Cannot standardize data if image dimensions are not the same."
                     )
                 else:
-                    print(
-                        "Note: merged dataset will not be standardized."
-                    )
+                    print("Note: merged dataset will not be standardized.")
                     for k, v in subsets.items():
                         if v[0] is None:
                             setattr(self, f"X_{k}", None)
                         else:
                             setattr(self, f"X_{k}", v[0])
                         if v[1] is None:
                             setattr(self, f"y_{k}", None)
                         else:
                             setattr(self, f"y_{k}", v[1])
 
-                    self.min_pv = (
-                        (self.min_pv * self.sigma) + self.mu
-                    ).astype(np.uint8)
-                    self.max_pv = (
-                        (self.max_pv * self.sigma) + self.mu
-                    ).astype(np.uint8)
+                    self.min_pv = ((self.min_pv * self.sigma) + self.mu).astype(
+                        np.uint8
+                    )
+                    self.max_pv = ((self.max_pv * self.sigma) + self.mu).astype(
+                        np.uint8
+                    )
 
             elif self.reduce == "norm":
                 print("Normalizing...")
                 for k, v in subsets.items():
                     if v[0] is None:
                         setattr(self, f"X_{k}", None)
                     else:
@@ -1802,15 +1705,14 @@
                         setattr(self, f"y_{k}", v[1])
 
             print("Data sucessfully merged into single data set.")
 
     #     ----------
 
     def display_batch(self, n_rows, n_cols):
-
         """
         Displays random batch of images from the Image_Dataset object,
         along with class label and data subset if drawn from a split
         dataset.
 
         Arguments:
             n_rows (int): number of rows of images to display.
@@ -1861,15 +1763,14 @@
 
             fig.tight_layout()
             plt.show()
 
     #     ----------
 
     def save_arrays(self, save_dir):
-
         """
         Saves the dataset in HDF5 format into a directory specified by
         the 'save_dir' argument. Note that the directory will be
         created if it does not already exist, and that existing data
         within the specified directory will be overwritten.
         """
 
@@ -1900,15 +1801,14 @@
                 with h5py.File(f"{r}/y_{k}.h5", "w") as hf:
                     hf.create_dataset(f"y_{k}", data=v[1])
                 print(f"{r}/y_{k}.h5 saved successfully.")
 
     #     ----------
 
     def save_imgs(self, save_dir):
-
         """
         Saves the dataset in image format into a directory specified
         by the 'save_dir' argument (images are saved into
         subdirectories for each class within the this directory).
         Note that the directory will be created if it does not already
         exist, and that existing data within the specified directory
         will be overwritten.
@@ -1957,15 +1857,14 @@
         self,
         portion,
         augmenter=None,
         augment_scale=None,
         augment_type="random",
         order=None,
     ):
-
         """
         Calls on an (initialized) imgo.augtools augmenter to apply image
         augmentation to the Image_Dataset's X_train subset.
 
         Arguments:
             portion (float): float within the range [0,1]. This is the
             portion of images in the set that will be augmented.
@@ -2003,54 +1902,46 @@
 
         from imgo import augtools
 
         if self.split == 0:
             raise Exception("Data has not been split.")
 
         else:
-
             if (portion >= 0) and (portion <= 1):
                 n = int(np.round(self.X_train.shape[0] * (portion)))
                 img_indices = np.random.choice(
                     self.X_train.shape[0], n, replace=False
                 )
             else:
-                raise Exception(
-                    "Portion argument must be in range [0,1]."
-                )
+                raise Exception("Portion argument must be in range [0,1].")
 
             X_aug_list = []
             y_aug_list = []
 
             for x in tqdm(
                 np.arange(self.shadow["train"][0].shape[0]), position=0
             ):
                 if x in img_indices:
-
                     img = self.shadow["train"][0][x]
                     label = self.shadow["train"][1][x]
 
                     if augment_scale:
                         scaled_img = auto_rescale(img, augment_scale)
                         if augment_type == "simple":
                             aug_scaled_img = augmenter.simple_augment(
                                 scaled_img, order=order
                             )
                         else:
                             aug_scaled_img = augmenter.random_augment(
                                 scaled_img
                             )
-                        aug_img = auto_rescale(
-                            aug_scaled_img, self.dims[0]
-                        )
+                        aug_img = auto_rescale(aug_scaled_img, self.dims[0])
                     else:
                         if augment_type == "simple":
-                            aug_img = augmenter.simple_augment(
-                                img, order=order
-                            )
+                            aug_img = augmenter.simple_augment(img, order=order)
                         else:
                             aug_img = augmenter.random_augment(
                                 self.shadow["train"][0][x]
                             )
 
                     X_aug_list.append(aug_img)
                     y_aug_list.append(label)
@@ -2133,15 +2024,14 @@
         split_ratio,
         augmenter=None,
         augment_scale=None,
         augment_type=None,
         order=None,
         force=False,
     ):
-
         """
         Splits dataset into training and testing (and validation) subsets
         and rebalances class sizes by calling on an (initialized)
         imgo.augtools augmenter to generate new training images (without
         affecting the validation/testing subsets). The number of images
         generated for each class will depend on the ratios given by the
         'split_ratio' argument as well as the number of images already
@@ -2222,20 +2112,17 @@
                 raise Exception("'split_ratio' argument must sum to 1.")
         else:
             raise Exception(
                 f"'split_ratio' argument must be list or tuple, {type(split_ratio)} given."
             )
 
         if self.split != 0:
-            raise Exception(
-                "Cannot split dataset that has already been split."
-            )
+            raise Exception("Cannot split dataset that has already been split.")
 
         else:
-
             indices = {}
             for i in self.class_list:
                 indices[i] = {
                     "imgs": [],
                     "to_bal": [],
                     "to_rem": [],
                     "valtest": [],
@@ -2364,37 +2251,32 @@
 
             for i in tqdm(
                 bal_indices,
                 total=len(bal_indices),
                 desc="Rebalancing",
                 position=0,
             ):
-
                 img = self.shadow["data"][0][i]
                 label = self.shadow["data"][1][i]
 
                 if augment_scale:
                     scaled_img = auto_rescale(img, augment_scale)
 
                     if augment_type == "simple":
                         aug_scaled_img = augmenter.simple_augment(
                             scaled_img, order=order
                         )
                     else:
-                        aug_scaled_img = augmenter.random_augment(
-                            scaled_img
-                        )
+                        aug_scaled_img = augmenter.random_augment(scaled_img)
 
                     aug_img = auto_rescale(aug_scaled_img, self.dims[0])
 
                 else:
                     if augment_type == "simple":
-                        aug_img = augmenter.simple_augment(
-                            img, order=order
-                        )
+                        aug_img = augmenter.simple_augment(img, order=order)
                     else:
                         aug_img = augmenter.random_augment(img)
 
                 X_train.append(aug_img)
                 y_train.append(label)
 
                 X_train_array = np.array(X_train)
@@ -2430,16 +2312,15 @@
                 if self.dims == "various":
                     raise Exception(
                         "Cannot standardize data if image dimensions are not the same."
                     )
                 else:
                     print("Standardizing...")
                     self.mu = (
-                        np.sum(subsets["train"][0])
-                        / subsets["train"][0].size
+                        np.sum(subsets["train"][0]) / subsets["train"][0].size
                     )
                     self.sigma = np.sqrt(
                         np.sum((subsets["train"][0] - self.mu) ** 2)
                         / subsets["train"][0].size
                     )
                     for k, v in subsets.items():
                         if v[0] is None:
```

