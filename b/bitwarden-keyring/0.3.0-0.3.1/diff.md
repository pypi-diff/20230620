# Comparing `tmp/bitwarden-keyring-0.3.0.tar.gz` & `tmp/bitwarden-keyring-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bitwarden-keyring-0.3.0.tar", last modified: Thu Dec  5 15:02:26 2019, max compression
+gzip compressed data, was "bitwarden-keyring-0.3.1.tar", last modified: Tue Jun 20 19:49:21 2023, max compression
```

## Comparing `bitwarden-keyring-0.3.0.tar` & `bitwarden-keyring-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 joachim   (1000) joachim   (1000)        0 2019-12-05 15:02:26.000000 bitwarden-keyring-0.3.0/
--rw-r--r--   0 joachim   (1000) joachim   (1000)     6259 2019-12-05 15:02:26.000000 bitwarden-keyring-0.3.0/PKG-INFO
--rw-r--r--   0 joachim   (1000) joachim   (1000)     4937 2019-12-05 14:57:15.000000 bitwarden-keyring-0.3.0/README.md
-drwxr-xr-x   0 joachim   (1000) joachim   (1000)        0 2019-12-05 15:02:26.000000 bitwarden-keyring-0.3.0/bitwarden_keyring/
--rw-r--r--   0 joachim   (1000) joachim   (1000)     5237 2019-12-05 15:01:08.000000 bitwarden-keyring-0.3.0/bitwarden_keyring/__init__.py
-drwxr-xr-x   0 joachim   (1000) joachim   (1000)        0 2019-12-05 15:02:26.000000 bitwarden-keyring-0.3.0/bitwarden_keyring.egg-info/
--rw-r--r--   0 joachim   (1000) joachim   (1000)     6259 2019-12-05 15:02:26.000000 bitwarden-keyring-0.3.0/bitwarden_keyring.egg-info/PKG-INFO
--rw-r--r--   0 joachim   (1000) joachim   (1000)      342 2019-12-05 15:02:26.000000 bitwarden-keyring-0.3.0/bitwarden_keyring.egg-info/SOURCES.txt
--rw-r--r--   0 joachim   (1000) joachim   (1000)        1 2019-12-05 15:02:26.000000 bitwarden-keyring-0.3.0/bitwarden_keyring.egg-info/dependency_links.txt
--rw-r--r--   0 joachim   (1000) joachim   (1000)       50 2019-12-05 15:02:26.000000 bitwarden-keyring-0.3.0/bitwarden_keyring.egg-info/entry_points.txt
--rw-r--r--   0 joachim   (1000) joachim   (1000)       64 2019-12-05 15:02:26.000000 bitwarden-keyring-0.3.0/bitwarden_keyring.egg-info/requires.txt
--rw-r--r--   0 joachim   (1000) joachim   (1000)       18 2019-12-05 15:02:26.000000 bitwarden-keyring-0.3.0/bitwarden_keyring.egg-info/top_level.txt
--rw-r--r--   0 joachim   (1000) joachim   (1000)        1 2019-12-05 13:57:45.000000 bitwarden-keyring-0.3.0/bitwarden_keyring.egg-info/zip-safe
--rw-r--r--   0 joachim   (1000) joachim   (1000)     1176 2019-12-05 15:02:26.000000 bitwarden-keyring-0.3.0/setup.cfg
--rw-r--r--   0 joachim   (1000) joachim   (1000)       38 2019-12-05 13:56:56.000000 bitwarden-keyring-0.3.0/setup.py
+drwxr-xr-x   0 joachim    (501) staff       (20)        0 2023-06-20 19:49:21.512392 bitwarden-keyring-0.3.1/
+-rw-r--r--   0 joachim    (501) staff       (20)     1080 2018-10-14 01:17:42.000000 bitwarden-keyring-0.3.1/LICENSE.md
+-rw-r--r--   0 joachim    (501) staff       (20)     5517 2023-06-20 19:49:21.512550 bitwarden-keyring-0.3.1/PKG-INFO
+-rw-r--r--   0 joachim    (501) staff       (20)     4937 2020-08-24 21:18:58.000000 bitwarden-keyring-0.3.1/README.md
+drwxr-xr-x   0 joachim    (501) staff       (20)        0 2023-06-20 19:49:21.488392 bitwarden-keyring-0.3.1/bitwarden_keyring/
+-rw-r--r--   0 joachim    (501) staff       (20)     5239 2023-06-20 19:46:32.000000 bitwarden-keyring-0.3.1/bitwarden_keyring/__init__.py
+drwxr-xr-x   0 joachim    (501) staff       (20)        0 2023-06-20 19:49:21.510564 bitwarden-keyring-0.3.1/bitwarden_keyring.egg-info/
+-rw-r--r--   0 joachim    (501) staff       (20)     5517 2023-06-20 19:49:21.000000 bitwarden-keyring-0.3.1/bitwarden_keyring.egg-info/PKG-INFO
+-rw-r--r--   0 joachim    (501) staff       (20)      385 2023-06-20 19:49:21.000000 bitwarden-keyring-0.3.1/bitwarden_keyring.egg-info/SOURCES.txt
+-rw-r--r--   0 joachim    (501) staff       (20)        1 2023-06-20 19:49:21.000000 bitwarden-keyring-0.3.1/bitwarden_keyring.egg-info/dependency_links.txt
+-rw-r--r--   0 joachim    (501) staff       (20)       49 2023-06-20 19:49:21.000000 bitwarden-keyring-0.3.1/bitwarden_keyring.egg-info/entry_points.txt
+-rw-r--r--   0 joachim    (501) staff       (20)       64 2023-06-20 19:49:21.000000 bitwarden-keyring-0.3.1/bitwarden_keyring.egg-info/requires.txt
+-rw-r--r--   0 joachim    (501) staff       (20)       18 2023-06-20 19:49:21.000000 bitwarden-keyring-0.3.1/bitwarden_keyring.egg-info/top_level.txt
+-rw-r--r--   0 joachim    (501) staff       (20)        1 2018-10-13 18:53:19.000000 bitwarden-keyring-0.3.1/bitwarden_keyring.egg-info/zip-safe
+-rw-r--r--   0 joachim    (501) staff       (20)     1176 2023-06-20 19:49:21.513568 bitwarden-keyring-0.3.1/setup.cfg
+-rw-r--r--   0 joachim    (501) staff       (20)       38 2018-10-13 18:40:26.000000 bitwarden-keyring-0.3.1/setup.py
+drwxr-xr-x   0 joachim    (501) staff       (20)        0 2023-06-20 19:49:21.511815 bitwarden-keyring-0.3.1/tests/
+-rw-r--r--   0 joachim    (501) staff       (20)     8540 2020-08-24 22:03:19.000000 bitwarden-keyring-0.3.1/tests/test_bitwarden_keyring.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bitwarden-keyring-0.3.0/PKG-INFO` & `bitwarden-keyring-0.3.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,109 +1,109 @@
 Metadata-Version: 2.1
 Name: bitwarden-keyring
-Version: 0.3.0
+Version: 0.3.1
 Summary: Keyring backend reading password data from Bitwarden
 Home-page: https://github.com/ewjoachim/bitwarden-keyring
 Author: Joachim Jablon
 Author-email: ewjoachim@gmail.com
 License: Apache Software License
-Description: # Bitwarden Keyring
-        
-        [![Build Status](https://travis-ci.org/ewjoachim/bitwarden-keyring.svg?branch=master)](https://travis-ci.org/ewjoachim/bitwarden-keyring)
-        [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-        [![PyPI version](https://badge.fury.io/py/bitwarden-keyring.svg)](https://badge.fury.io/py/bitwarden-keyring)
-        [![codecov](https://codecov.io/gh/ewjoachim/bitwarden-keyring/branch/master/graph/badge.svg)](https://codecov.io/gh/ewjoachim/bitwarden-keyring)
-        
-        
-        Implementation of the [Keyring](https://pypi.org/project/keyring/) backend code reading secrets from [Bitwarden](https://bitwarden.com) using [Bitwarden-cli](https://help.bitwarden.com/article/cli/)
-        
-        ## Overview
-        
-        The [Keyring](https://pypi.org/project/keyring/) python package provides a handy single point of entry for any secret holding system, allowing for seemless integration of those systems into applications needing secrets, like [twine]().
-        
-        This projects implement Keyring to be able to read secrets from Bitwarden, an open source multiplatform cloud/self-hostable password manager.
-        
-        This backend assumes that it will be used in the context of a CLI application, and that it can communicate with the user using `sdtin`, `stdout` and `stderr`. We could implement an additional backend for use in a library assuming that everything is already unlocked, or another one using `pinentry` to ask the user.
-        
-        
-        ## Requirements
-        
-        This project uses the official [bitwarden CLI](https://help.bitwarden.com/article/cli/) under the hood, because there's no simple official Python bitwarden lib. Here are the installation instructions as of October 2018 and the link to the [up to date instructions](https://github.com/bitwarden/cli#downloadinstall)
-        
-        You can install the Bitwarden CLI multiple different ways:
-        
-        **NPM**
-        
-        If you already have the Node.js runtime installed on your system, you can install the CLI using NPM. NPM makes it easy to keep your installation updated and should be the preferred installation method if you are already using Node.js.
-        
-        ```bash
-        npm install -g @bitwarden/cli
-        ```
-        
-        **Native Executable**
-        
-        Natively packaged versions of the CLI are provided for each platform which have no requirements on installing the Node.js runtime. You can obtain these from the [downloads section](https://help.bitwarden.com/article/cli/#download--install) in the Bitwarden documentation.
-        
-        **Other Package Managers**
-        
-        - [Chocolatey](https://chocolatey.org/packages/bitwarden-cli)
-          ```powershell
-          choco install bitwarden-cli
-          ```
-        - [Homebrew](https://formulae.brew.sh/formula/bitwarden-cli)
-          ```bash
-          brew install bitwarden-cli
-          ```
-        - [Snap](https://snapcraft.io/bw)
-          ```bash
-          sudo snap install bw
-          ```
-        
-        ## Installation and configuration
-        
-        ```
-        pip install bitwarden-keyring
-        ```
-        
-        The Python packaging ecosystem can be quite a mess.
-        
-        [<img title="XKCD 1987: Python Environment. The Python environmental protection agency wants to seal it in a cement chamber, with pictorial messages to future civilizations warning them about the danger of using sudo to install random Python packages." src="https://imgs.xkcd.com/comics/python_environment_2x.png" width="400">](https://xkcd.com/1987/)
-        
-        Because of this, it's likely that your setup and my setup are nothing alike. Keyring [supports](https://pypi.org/project/keyring/#config-file-content) a configuration file with an option allowing to explicitely define the path to a backend. You may need that for your installation, or maybe not.
-        
-        ## Usage
-        
-        Use as a normal keyring backend. It is installed with priority 10 so it's likely going to be selected
-        first.
-        
-        If you want to use it with [twine](https://pypi.org/project/twine/), good news, you're already set. Just make sure that this package is installed in the same location as twine.
-        
-        `bitwarden-keyring` will automatically ask for credentials when needed. If you don't want to unlock your vault every time, export the vault session to your environment (use `bw unlock` and follow the instructions, or launch `export BW_SESSION=$(bw unlock --raw)`).
-        
-        ## Caveats
-        
-        `bitwarden-keyring` was only tested with:
-        - macOS, using the `bitwarden-cli` from `brew`
-        - ubuntu, using the `bw` from `snap`
-        
-        As mentionned, `bitwarden-keyring` only works in the context of a CLI application with access to standard inputs and output. If you need something that either reads silently or using another method of communication, the best is probably to make another backend and most of the functions can be reused.
-        
-        ## Licensing
-        
-        `bitwarden-keyring` is published under the terms of the [MIT License](LICENSE.md).
-        The name Bitwarden is most probably the property of 8bit Solutions LLC.
-        
-        
-        ## Contributions and Code of Conduct
-        
-        Contributions are welcome, please refer to the [Contributing](CONTRIBUTING.md) guide.
-        Please keep in mind that all interactions with the project are required to follow the
-        [Code of Conduct](CODE_OF_CONDUCT.md).
-        
 Keywords: bitwarden keyring password
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE.md
+
+# Bitwarden Keyring
+
+[![Build Status](https://travis-ci.org/ewjoachim/bitwarden-keyring.svg?branch=master)](https://travis-ci.org/ewjoachim/bitwarden-keyring)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![PyPI version](https://badge.fury.io/py/bitwarden-keyring.svg)](https://badge.fury.io/py/bitwarden-keyring)
+[![codecov](https://codecov.io/gh/ewjoachim/bitwarden-keyring/branch/master/graph/badge.svg)](https://codecov.io/gh/ewjoachim/bitwarden-keyring)
+
+
+Implementation of the [Keyring](https://pypi.org/project/keyring/) backend code reading secrets from [Bitwarden](https://bitwarden.com) using [Bitwarden-cli](https://help.bitwarden.com/article/cli/)
+
+## Overview
+
+The [Keyring](https://pypi.org/project/keyring/) python package provides a handy single point of entry for any secret holding system, allowing for seemless integration of those systems into applications needing secrets, like [twine]().
+
+This projects implement Keyring to be able to read secrets from Bitwarden, an open source multiplatform cloud/self-hostable password manager.
+
+This backend assumes that it will be used in the context of a CLI application, and that it can communicate with the user using `sdtin`, `stdout` and `stderr`. We could implement an additional backend for use in a library assuming that everything is already unlocked, or another one using `pinentry` to ask the user.
+
+
+## Requirements
+
+This project uses the official [bitwarden CLI](https://help.bitwarden.com/article/cli/) under the hood, because there's no simple official Python bitwarden lib. Here are the installation instructions as of October 2018 and the link to the [up to date instructions](https://github.com/bitwarden/cli#downloadinstall)
+
+You can install the Bitwarden CLI multiple different ways:
+
+**NPM**
+
+If you already have the Node.js runtime installed on your system, you can install the CLI using NPM. NPM makes it easy to keep your installation updated and should be the preferred installation method if you are already using Node.js.
+
+```bash
+npm install -g @bitwarden/cli
+```
+
+**Native Executable**
+
+Natively packaged versions of the CLI are provided for each platform which have no requirements on installing the Node.js runtime. You can obtain these from the [downloads section](https://help.bitwarden.com/article/cli/#download--install) in the Bitwarden documentation.
+
+**Other Package Managers**
+
+- [Chocolatey](https://chocolatey.org/packages/bitwarden-cli)
+  ```powershell
+  choco install bitwarden-cli
+  ```
+- [Homebrew](https://formulae.brew.sh/formula/bitwarden-cli)
+  ```bash
+  brew install bitwarden-cli
+  ```
+- [Snap](https://snapcraft.io/bw)
+  ```bash
+  sudo snap install bw
+  ```
+
+## Installation and configuration
+
+```
+pip install bitwarden-keyring
+```
+
+The Python packaging ecosystem can be quite a mess.
+
+[<img title="XKCD 1987: Python Environment. The Python environmental protection agency wants to seal it in a cement chamber, with pictorial messages to future civilizations warning them about the danger of using sudo to install random Python packages." src="https://imgs.xkcd.com/comics/python_environment_2x.png" width="400">](https://xkcd.com/1987/)
+
+Because of this, it's likely that your setup and my setup are nothing alike. Keyring [supports](https://pypi.org/project/keyring/#config-file-content) a configuration file with an option allowing to explicitely define the path to a backend. You may need that for your installation, or maybe not.
+
+## Usage
+
+Use as a normal keyring backend. It is installed with priority 10 so it's likely going to be selected
+first.
+
+If you want to use it with [twine](https://pypi.org/project/twine/), good news, you're already set. Just make sure that this package is installed in the same location as twine.
+
+`bitwarden-keyring` will automatically ask for credentials when needed. If you don't want to unlock your vault every time, export the vault session to your environment (use `bw unlock` and follow the instructions, or launch `export BW_SESSION=$(bw unlock --raw)`).
+
+## Caveats
+
+`bitwarden-keyring` was only tested with:
+- macOS, using the `bitwarden-cli` from `brew`
+- ubuntu, using the `bw` from `snap`
+
+As mentionned, `bitwarden-keyring` only works in the context of a CLI application with access to standard inputs and output. If you need something that either reads silently or using another method of communication, the best is probably to make another backend and most of the functions can be reused.
+
+## Licensing
+
+`bitwarden-keyring` is published under the terms of the [MIT License](LICENSE.md).
+The name Bitwarden is most probably the property of 8bit Solutions LLC.
+
+
+## Contributions and Code of Conduct
+
+Contributions are welcome, please refer to the [Contributing](CONTRIBUTING.md) guide.
+Please keep in mind that all interactions with the project are required to follow the
+[Code of Conduct](CODE_OF_CONDUCT.md).
```

### Comparing `bitwarden-keyring-0.3.0/README.md` & `bitwarden-keyring-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `bitwarden-keyring-0.3.0/bitwarden_keyring/__init__.py` & `bitwarden-keyring-0.3.1/bitwarden_keyring/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import base64
 import json
 import os
 import shutil
 import subprocess
 
 from keyring import backend
-from keyring.util import properties
+from jaraco.classes import properties
 
 PRIORITY = 10  # Doc is oddly vague
 
 
 def user_is_authenticated():
     return bw_run(*bw_args("login", "--check")).returncode == 0
 
@@ -192,15 +192,15 @@
 
     credential = json.loads(result)
 
     confirm_delete(session, credential)
 
 
 class BitwardenBackend(backend.KeyringBackend):
-    @properties.ClassProperty
+    @properties.classproperty
     @classmethod
     def priority(cls):
         if not bitwarden_cli_installed():
             raise RuntimeError(
                 "Requires bitwarden cli: https://help.bitwarden.com/article/cli/"
             )
```

### Comparing `bitwarden-keyring-0.3.0/bitwarden_keyring.egg-info/PKG-INFO` & `bitwarden-keyring-0.3.1/bitwarden_keyring.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,109 +1,109 @@
 Metadata-Version: 2.1
 Name: bitwarden-keyring
-Version: 0.3.0
+Version: 0.3.1
 Summary: Keyring backend reading password data from Bitwarden
 Home-page: https://github.com/ewjoachim/bitwarden-keyring
 Author: Joachim Jablon
 Author-email: ewjoachim@gmail.com
 License: Apache Software License
-Description: # Bitwarden Keyring
-        
-        [![Build Status](https://travis-ci.org/ewjoachim/bitwarden-keyring.svg?branch=master)](https://travis-ci.org/ewjoachim/bitwarden-keyring)
-        [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-        [![PyPI version](https://badge.fury.io/py/bitwarden-keyring.svg)](https://badge.fury.io/py/bitwarden-keyring)
-        [![codecov](https://codecov.io/gh/ewjoachim/bitwarden-keyring/branch/master/graph/badge.svg)](https://codecov.io/gh/ewjoachim/bitwarden-keyring)
-        
-        
-        Implementation of the [Keyring](https://pypi.org/project/keyring/) backend code reading secrets from [Bitwarden](https://bitwarden.com) using [Bitwarden-cli](https://help.bitwarden.com/article/cli/)
-        
-        ## Overview
-        
-        The [Keyring](https://pypi.org/project/keyring/) python package provides a handy single point of entry for any secret holding system, allowing for seemless integration of those systems into applications needing secrets, like [twine]().
-        
-        This projects implement Keyring to be able to read secrets from Bitwarden, an open source multiplatform cloud/self-hostable password manager.
-        
-        This backend assumes that it will be used in the context of a CLI application, and that it can communicate with the user using `sdtin`, `stdout` and `stderr`. We could implement an additional backend for use in a library assuming that everything is already unlocked, or another one using `pinentry` to ask the user.
-        
-        
-        ## Requirements
-        
-        This project uses the official [bitwarden CLI](https://help.bitwarden.com/article/cli/) under the hood, because there's no simple official Python bitwarden lib. Here are the installation instructions as of October 2018 and the link to the [up to date instructions](https://github.com/bitwarden/cli#downloadinstall)
-        
-        You can install the Bitwarden CLI multiple different ways:
-        
-        **NPM**
-        
-        If you already have the Node.js runtime installed on your system, you can install the CLI using NPM. NPM makes it easy to keep your installation updated and should be the preferred installation method if you are already using Node.js.
-        
-        ```bash
-        npm install -g @bitwarden/cli
-        ```
-        
-        **Native Executable**
-        
-        Natively packaged versions of the CLI are provided for each platform which have no requirements on installing the Node.js runtime. You can obtain these from the [downloads section](https://help.bitwarden.com/article/cli/#download--install) in the Bitwarden documentation.
-        
-        **Other Package Managers**
-        
-        - [Chocolatey](https://chocolatey.org/packages/bitwarden-cli)
-          ```powershell
-          choco install bitwarden-cli
-          ```
-        - [Homebrew](https://formulae.brew.sh/formula/bitwarden-cli)
-          ```bash
-          brew install bitwarden-cli
-          ```
-        - [Snap](https://snapcraft.io/bw)
-          ```bash
-          sudo snap install bw
-          ```
-        
-        ## Installation and configuration
-        
-        ```
-        pip install bitwarden-keyring
-        ```
-        
-        The Python packaging ecosystem can be quite a mess.
-        
-        [<img title="XKCD 1987: Python Environment. The Python environmental protection agency wants to seal it in a cement chamber, with pictorial messages to future civilizations warning them about the danger of using sudo to install random Python packages." src="https://imgs.xkcd.com/comics/python_environment_2x.png" width="400">](https://xkcd.com/1987/)
-        
-        Because of this, it's likely that your setup and my setup are nothing alike. Keyring [supports](https://pypi.org/project/keyring/#config-file-content) a configuration file with an option allowing to explicitely define the path to a backend. You may need that for your installation, or maybe not.
-        
-        ## Usage
-        
-        Use as a normal keyring backend. It is installed with priority 10 so it's likely going to be selected
-        first.
-        
-        If you want to use it with [twine](https://pypi.org/project/twine/), good news, you're already set. Just make sure that this package is installed in the same location as twine.
-        
-        `bitwarden-keyring` will automatically ask for credentials when needed. If you don't want to unlock your vault every time, export the vault session to your environment (use `bw unlock` and follow the instructions, or launch `export BW_SESSION=$(bw unlock --raw)`).
-        
-        ## Caveats
-        
-        `bitwarden-keyring` was only tested with:
-        - macOS, using the `bitwarden-cli` from `brew`
-        - ubuntu, using the `bw` from `snap`
-        
-        As mentionned, `bitwarden-keyring` only works in the context of a CLI application with access to standard inputs and output. If you need something that either reads silently or using another method of communication, the best is probably to make another backend and most of the functions can be reused.
-        
-        ## Licensing
-        
-        `bitwarden-keyring` is published under the terms of the [MIT License](LICENSE.md).
-        The name Bitwarden is most probably the property of 8bit Solutions LLC.
-        
-        
-        ## Contributions and Code of Conduct
-        
-        Contributions are welcome, please refer to the [Contributing](CONTRIBUTING.md) guide.
-        Please keep in mind that all interactions with the project are required to follow the
-        [Code of Conduct](CODE_OF_CONDUCT.md).
-        
 Keywords: bitwarden keyring password
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE.md
+
+# Bitwarden Keyring
+
+[![Build Status](https://travis-ci.org/ewjoachim/bitwarden-keyring.svg?branch=master)](https://travis-ci.org/ewjoachim/bitwarden-keyring)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![PyPI version](https://badge.fury.io/py/bitwarden-keyring.svg)](https://badge.fury.io/py/bitwarden-keyring)
+[![codecov](https://codecov.io/gh/ewjoachim/bitwarden-keyring/branch/master/graph/badge.svg)](https://codecov.io/gh/ewjoachim/bitwarden-keyring)
+
+
+Implementation of the [Keyring](https://pypi.org/project/keyring/) backend code reading secrets from [Bitwarden](https://bitwarden.com) using [Bitwarden-cli](https://help.bitwarden.com/article/cli/)
+
+## Overview
+
+The [Keyring](https://pypi.org/project/keyring/) python package provides a handy single point of entry for any secret holding system, allowing for seemless integration of those systems into applications needing secrets, like [twine]().
+
+This projects implement Keyring to be able to read secrets from Bitwarden, an open source multiplatform cloud/self-hostable password manager.
+
+This backend assumes that it will be used in the context of a CLI application, and that it can communicate with the user using `sdtin`, `stdout` and `stderr`. We could implement an additional backend for use in a library assuming that everything is already unlocked, or another one using `pinentry` to ask the user.
+
+
+## Requirements
+
+This project uses the official [bitwarden CLI](https://help.bitwarden.com/article/cli/) under the hood, because there's no simple official Python bitwarden lib. Here are the installation instructions as of October 2018 and the link to the [up to date instructions](https://github.com/bitwarden/cli#downloadinstall)
+
+You can install the Bitwarden CLI multiple different ways:
+
+**NPM**
+
+If you already have the Node.js runtime installed on your system, you can install the CLI using NPM. NPM makes it easy to keep your installation updated and should be the preferred installation method if you are already using Node.js.
+
+```bash
+npm install -g @bitwarden/cli
+```
+
+**Native Executable**
+
+Natively packaged versions of the CLI are provided for each platform which have no requirements on installing the Node.js runtime. You can obtain these from the [downloads section](https://help.bitwarden.com/article/cli/#download--install) in the Bitwarden documentation.
+
+**Other Package Managers**
+
+- [Chocolatey](https://chocolatey.org/packages/bitwarden-cli)
+  ```powershell
+  choco install bitwarden-cli
+  ```
+- [Homebrew](https://formulae.brew.sh/formula/bitwarden-cli)
+  ```bash
+  brew install bitwarden-cli
+  ```
+- [Snap](https://snapcraft.io/bw)
+  ```bash
+  sudo snap install bw
+  ```
+
+## Installation and configuration
+
+```
+pip install bitwarden-keyring
+```
+
+The Python packaging ecosystem can be quite a mess.
+
+[<img title="XKCD 1987: Python Environment. The Python environmental protection agency wants to seal it in a cement chamber, with pictorial messages to future civilizations warning them about the danger of using sudo to install random Python packages." src="https://imgs.xkcd.com/comics/python_environment_2x.png" width="400">](https://xkcd.com/1987/)
+
+Because of this, it's likely that your setup and my setup are nothing alike. Keyring [supports](https://pypi.org/project/keyring/#config-file-content) a configuration file with an option allowing to explicitely define the path to a backend. You may need that for your installation, or maybe not.
+
+## Usage
+
+Use as a normal keyring backend. It is installed with priority 10 so it's likely going to be selected
+first.
+
+If you want to use it with [twine](https://pypi.org/project/twine/), good news, you're already set. Just make sure that this package is installed in the same location as twine.
+
+`bitwarden-keyring` will automatically ask for credentials when needed. If you don't want to unlock your vault every time, export the vault session to your environment (use `bw unlock` and follow the instructions, or launch `export BW_SESSION=$(bw unlock --raw)`).
+
+## Caveats
+
+`bitwarden-keyring` was only tested with:
+- macOS, using the `bitwarden-cli` from `brew`
+- ubuntu, using the `bw` from `snap`
+
+As mentionned, `bitwarden-keyring` only works in the context of a CLI application with access to standard inputs and output. If you need something that either reads silently or using another method of communication, the best is probably to make another backend and most of the functions can be reused.
+
+## Licensing
+
+`bitwarden-keyring` is published under the terms of the [MIT License](LICENSE.md).
+The name Bitwarden is most probably the property of 8bit Solutions LLC.
+
+
+## Contributions and Code of Conduct
+
+Contributions are welcome, please refer to the [Contributing](CONTRIBUTING.md) guide.
+Please keep in mind that all interactions with the project are required to follow the
+[Code of Conduct](CODE_OF_CONDUCT.md).
```

### Comparing `bitwarden-keyring-0.3.0/setup.cfg` & `bitwarden-keyring-0.3.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = bitwarden-keyring
 description = Keyring backend reading password data from Bitwarden
-version = 0.3.0
+version = 0.3.1
 author = Joachim Jablon
 author_email = ewjoachim@gmail.com
 url = https://github.com/ewjoachim/bitwarden-keyring
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = bitwarden keyring password
 license = Apache Software License
```

