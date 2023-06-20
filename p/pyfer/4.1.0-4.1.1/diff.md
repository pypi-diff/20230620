# Comparing `tmp/pyfer-4.1.0.tar.gz` & `tmp/pyfer-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyfer-4.1.0.tar", last modified: Tue Apr  5 10:00:10 2022, max compression
+gzip compressed data, was "pyfer-4.1.1.tar", last modified: Tue Jun 20 16:19:31 2023, max compression
```

## Comparing `pyfer-4.1.0.tar` & `pyfer-4.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2022-04-05 10:00:10.000000 pyfer-4.1.0/
--rw-r--r--   0 lucbatty   (501) staff       (20)     1689 2022-04-05 10:00:10.000000 pyfer-4.1.0/PKG-INFO
--rw-r--r--   0 lucbatty   (501) staff       (20)      941 2020-10-23 10:44:22.000000 pyfer-4.1.0/README.md
-drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2022-04-05 10:00:10.000000 pyfer-4.1.0/pyfer/
--rw-r--r--   0 lucbatty   (501) staff       (20)       46 2022-04-05 09:58:34.000000 pyfer-4.1.0/pyfer/__init__.py
--rw-r--r--   0 lucbatty   (501) staff       (20)    10689 2022-04-05 09:59:08.000000 pyfer-4.1.0/pyfer/pyfer.py
-drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2022-04-05 10:00:10.000000 pyfer-4.1.0/pyfer.egg-info/
--rw-r--r--   0 lucbatty   (501) staff       (20)     1689 2022-04-05 10:00:09.000000 pyfer-4.1.0/pyfer.egg-info/PKG-INFO
--rw-r--r--   0 lucbatty   (501) staff       (20)      182 2022-04-05 10:00:09.000000 pyfer-4.1.0/pyfer.egg-info/SOURCES.txt
--rw-r--r--   0 lucbatty   (501) staff       (20)        1 2022-04-05 10:00:09.000000 pyfer-4.1.0/pyfer.egg-info/dependency_links.txt
--rw-r--r--   0 lucbatty   (501) staff       (20)        6 2022-04-05 10:00:09.000000 pyfer-4.1.0/pyfer.egg-info/top_level.txt
--rw-r--r--   0 lucbatty   (501) staff       (20)      226 2020-09-27 15:49:53.000000 pyfer-4.1.0/pyproject.toml
--rw-r--r--   0 lucbatty   (501) staff       (20)       38 2022-04-05 10:00:10.000000 pyfer-4.1.0/setup.cfg
--rw-r--r--   0 lucbatty   (501) staff       (20)      626 2022-04-05 09:59:47.000000 pyfer-4.1.0/setup.py
+drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-20 16:19:31.642626 pyfer-4.1.1/
+-rw-r--r--   0 lucbatty   (501) staff       (20)     1065 2023-04-03 07:33:30.000000 pyfer-4.1.1/LICENSE.txt
+-rw-r--r--   0 lucbatty   (501) staff       (20)     1944 2023-06-20 16:19:31.641928 pyfer-4.1.1/PKG-INFO
+-rw-r--r--   0 lucbatty   (501) staff       (20)     1292 2023-06-20 16:06:14.000000 pyfer-4.1.1/README.md
+drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-20 16:19:31.635771 pyfer-4.1.1/pyfer/
+-rw-r--r--   0 lucbatty   (501) staff       (20)       46 2023-04-03 07:33:30.000000 pyfer-4.1.1/pyfer/__init__.py
+-rw-r--r--   0 lucbatty   (501) staff       (20)    10451 2023-06-20 09:28:21.000000 pyfer-4.1.1/pyfer/pyfer.py
+drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-20 16:19:31.641065 pyfer-4.1.1/pyfer.egg-info/
+-rw-r--r--   0 lucbatty   (501) staff       (20)     1944 2023-06-20 16:19:31.000000 pyfer-4.1.1/pyfer.egg-info/PKG-INFO
+-rw-r--r--   0 lucbatty   (501) staff       (20)      194 2023-06-20 16:19:31.000000 pyfer-4.1.1/pyfer.egg-info/SOURCES.txt
+-rw-r--r--   0 lucbatty   (501) staff       (20)        1 2023-06-20 16:19:31.000000 pyfer-4.1.1/pyfer.egg-info/dependency_links.txt
+-rw-r--r--   0 lucbatty   (501) staff       (20)        6 2023-06-20 16:19:31.000000 pyfer-4.1.1/pyfer.egg-info/top_level.txt
+-rw-r--r--   0 lucbatty   (501) staff       (20)      226 2023-04-03 07:33:30.000000 pyfer-4.1.1/pyproject.toml
+-rw-r--r--   0 lucbatty   (501) staff       (20)       38 2023-06-20 16:19:31.642868 pyfer-4.1.1/setup.cfg
+-rw-r--r--   0 lucbatty   (501) staff       (20)      852 2023-06-20 16:11:32.000000 pyfer-4.1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyfer-4.1.0/README.md` & `pyfer-4.1.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,54 @@
-# PYFER
+![pyfer_cover](aux/rm_cover.jpg)
 
-## Encrypt and Decrypt Strings
+-----------------
 
-Pyfer is a simple encryption and decryption tool built in Python. 
+# Pyfer ~ Encrypt and Decrypt Strings
 
-![pyfer_cover](aux/rm_cover.jpg)
+[![PyPI - Version](https://img.shields.io/pypi/v/pyfer.svg)](https://pypi.org/project/pyfer/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyfer.svg)](https://pypi.org/project/pyfer/)
+[![License: MIT](https://img.shields.io/badge/license-MIT-C06524)](https://github.com/celerygemini/pyfer/blob/main/LICENSE)
+
+## 💡 What is it?
+
+Pyfer is a simple encryption and decryption tool built in Python. 
 
 ### Features
 
 With this little library you can do the following:
 
  - Encrypt and decrypt strings
  - Use one of three available encryption modes, each using a different ciphertext alphabet
  - Generate random digit keys
 
-### Installation
+## 🛠️ Setup 
+
+Install it from **PyPI** by running `pip install pyfer`.
 
-It's as easy as `pip install pyfer`!
+### Dependencies 
+
+The only dependency is [NumPy](https://numpy.org)
+
+## 🚀 Execution
 
 ### Quickstart
 
-Have a look at the demo [here](https://github.com/elbydata/pyfer/blob/master/demos/demo.ipynb)!
+```
+import pyfer
 
-### Documentation
+k = pyfer.generate_key(45)
+m = "Hello_world!"
+pm = pyfer.Machine(k)
 
-Documentation is currently available in the form of docstrings.
+pm.scramble(m)
 
-### Requirements and Dependencies
+```
 
-Please see the `requirements.txt` file for all requirements and dependencies.
- 
-### Support
+For more information, have a look at the demo [here](https://github.com/elbydata/pyfer/blob/master/demos/demo.ipynb)!
 
-The source code is available [here](https://github.com/elbydata/pyfer/tree/master/pyfer).
-Please direct any queries to info@elbydata.com.
+## 📝 Documentation
 
-### License
+Documentation is currently available in the form of docstrings.
+ 
+## ⚖️ License
 
 The project is licensed under the MIT license.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyfer-4.1.0/pyfer/pyfer.py` & `pyfer-4.1.1/pyfer/pyfer.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 import string
 import itertools
 
 # ------------------------------------------------------------------------
 
 
 def generate_key(key_length):
-
     """
     Generates a random string of digits of the specified length.
     """
 
     if type(key_length) is int:
         n = key_length
     else:
@@ -76,15 +75,14 @@
     -
     scramble: encrypts a message.
     -
     unscramble: decrypts a message.
     """
 
     def __init__(self, key, ws=False):
-
         """
         Constructs all the necessary attributes for the Crypt encryption
         machine.
 
         Arguments:
             key (str): string of 30, 40, or 45 digits to serving as
             encryption key.
@@ -165,28 +163,24 @@
                 if x
             ]
         elif len(key) == 40:
             self.key = key
             self.char_list = [
                 x
                 for x in itertools.chain.from_iterable(
-                    itertools.zip_longest(
-                        lc_list, uc_list, d_list, p_med
-                    )
+                    itertools.zip_longest(lc_list, uc_list, d_list, p_med)
                 )
                 if x
             ]
         elif len(key) == 45:
             self.key = key
             self.char_list = [
                 x
                 for x in itertools.chain.from_iterable(
-                    itertools.zip_longest(
-                        lc_list, uc_list, d_list, p_full
-                    )
+                    itertools.zip_longest(lc_list, uc_list, d_list, p_full)
                 )
                 if x
             ]
         else:
             self.key = None
             self.char_list = None
             raise Exception(
@@ -223,60 +217,57 @@
                     y2_key = np.argsort(np.array(key_y2_elements))
 
                 key_z_elements = []
                 for i in self.key[(-1 * square) :]:
                     key_z_elements.append(int(i))
                     z_key = np.argsort(np.array(key_z_elements))
 
-        self.char_grid = np.asarray(self.char_list).reshape(
-            square, square
-        )
+        self.char_grid = np.asarray(self.char_list).reshape(square, square)
 
         reshuffle_1 = self.char_grid[:, x_key]
         if len(self.key) == 40:
             reshuffle_2 = reshuffle_1.reshape(
-                4, int((square ** 2) / 4)
+                4, int((square**2) / 4)
             ).transpose()
         else:
             reshuffle_2 = reshuffle_1.reshape(
-                3, int((square ** 2) / 3)
+                3, int((square**2) / 3)
             ).transpose()
         reshuffle_3 = reshuffle_2.reshape(square, square)
         reshuffle_4 = reshuffle_3[y_key, :]
 
         reshuffle_5 = reshuffle_4[:, x2_key]
         if len(self.key) == 40:
             reshuffle_6 = reshuffle_5.reshape(
-                4, int((square ** 2) / 4)
+                4, int((square**2) / 4)
             ).transpose()
         else:
             reshuffle_6 = reshuffle_5.reshape(
-                3, int((square ** 2) / 3)
+                3, int((square**2) / 3)
             ).transpose()
         reshuffle_7 = reshuffle_6.reshape(square, square)
         reshuffle_8 = reshuffle_7[y2_key, :]
 
         reshuffle_9 = reshuffle_8[:, z_key]
         if len(self.key) == 40:
             reshuffle_10 = reshuffle_9.reshape(
-                4, int((square ** 2) / 4)
+                4, int((square**2) / 4)
             ).transpose()
         else:
             reshuffle_10 = reshuffle_9.reshape(
-                3, int((square ** 2) / 3)
+                3, int((square**2) / 3)
             ).transpose()
         reshuffle_11 = reshuffle_10.reshape(square, square)
         reshuffle_12 = reshuffle_11[z_key, :]
 
         self.scramble_grid = reshuffle_12
 
     #     ----------
 
     def scramble(self, input_string):
-
         """
         Scramble the input message using the Crypt Machine.
 
         Arguments:
             input_string (str): message to encrypt.
 
         Returns:
@@ -285,17 +276,15 @@
 
         if type(input_string) is str:
             if np.mod(len(input_string), 2) == 0:
                 if len(input_string) > 1:
                     if all(i in self.char_list for i in input_string):
                         pass
                     else:
-                        raise Exception(
-                            "Disallowed characters in input string"
-                        )
+                        raise Exception("Disallowed characters in input string")
                 else:
                     raise Exception(
                         "Input string must have length greater than 1."
                     )
             else:
                 input_string = input_string + "00000"
         else:
@@ -318,15 +307,14 @@
         output_string = "".join(output_list)
 
         return output_string
 
     #     ----------
 
     def unscramble(self, input_string):
-
         """
         Unscramble the input message using the Crypt Machine.
 
         Arguments:
             input_string (str): message to decrypt.
 
         Returns:
@@ -335,17 +323,15 @@
 
         if type(input_string) is str:
             if np.mod(len(input_string), 2) == 0:
                 if len(input_string) > 1:
                     if all(i in self.char_list for i in input_string):
                         pass
                     else:
-                        raise Exception(
-                            "Disallowed characters in input string"
-                        )
+                        raise Exception("Disallowed characters in input string")
                 else:
                     raise Exception(
                         "Input string must have length greater than 1."
                     )
             else:
                 input_string = input_string + "00000"
         else:
```

