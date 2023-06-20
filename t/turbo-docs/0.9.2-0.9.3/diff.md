# Comparing `tmp/turbo_docs-0.9.2.tar.gz` & `tmp/turbo_docs-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbo_docs-0.9.2.tar", last modified: Wed Jun 14 00:33:14 2023, max compression
+gzip compressed data, was "turbo_docs-0.9.3.tar", last modified: Tue Jun 20 00:33:51 2023, max compression
```

## Comparing `turbo_docs-0.9.2.tar` & `turbo_docs-0.9.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 00:33:14.866591 turbo_docs-0.9.2/
--rw-rw-rw-   0        0        0     2363 2023-06-14 00:33:14.865589 turbo_docs-0.9.2/PKG-INFO
--rw-rw-rw-   0        0        0     1866 2023-06-14 00:24:27.000000 turbo_docs-0.9.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 00:33:14.867594 turbo_docs-0.9.2/setup.cfg
--rw-rw-rw-   0        0        0      844 2023-06-14 00:31:52.000000 turbo_docs-0.9.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 00:33:14.840824 turbo_docs-0.9.2/turbo_docs/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.9.2/turbo_docs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 00:33:14.855582 turbo_docs-0.9.2/turbo_docs/commands/
--rw-rw-rw-   0        0        0        0 2023-04-29 00:25:31.000000 turbo_docs-0.9.2/turbo_docs/commands/__init__.py
--rw-rw-rw-   0        0        0      840 2023-06-14 00:22:59.000000 turbo_docs-0.9.2/turbo_docs/commands/readme.py
--rw-rw-rw-   0        0        0      914 2023-06-14 00:14:25.000000 turbo_docs-0.9.2/turbo_docs/generate.py
-drwxrwxrwx   0        0        0        0 2023-06-14 00:33:14.862590 turbo_docs-0.9.2/turbo_docs/utils/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.9.2/turbo_docs/utils/__init__.py
--rw-rw-rw-   0        0        0      622 2023-06-14 00:14:25.000000 turbo_docs-0.9.2/turbo_docs/utils/cli_options.py
--rw-rw-rw-   0        0        0     2022 2023-06-12 21:03:28.000000 turbo_docs-0.9.2/turbo_docs/utils/directory.py
--rw-rw-rw-   0        0        0      992 2023-06-14 00:20:44.000000 turbo_docs-0.9.2/turbo_docs/utils/openai_api.py
-drwxrwxrwx   0        0        0        0 2023-06-14 00:33:14.851828 turbo_docs-0.9.2/turbo_docs.egg-info/
--rw-rw-rw-   0        0        0     2363 2023-06-14 00:33:14.000000 turbo_docs-0.9.2/turbo_docs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-06-14 00:33:14.000000 turbo_docs-0.9.2/turbo_docs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 00:33:14.000000 turbo_docs-0.9.2/turbo_docs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-06-14 00:33:14.000000 turbo_docs-0.9.2/turbo_docs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       65 2023-06-14 00:33:14.000000 turbo_docs-0.9.2/turbo_docs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-14 00:33:14.000000 turbo_docs-0.9.2/turbo_docs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 00:33:51.481467 turbo_docs-0.9.3/
+-rw-rw-rw-   0        0        0     2677 2023-06-20 00:33:51.480465 turbo_docs-0.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2180 2023-06-19 23:48:10.000000 turbo_docs-0.9.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-20 00:33:51.482463 turbo_docs-0.9.3/setup.cfg
+-rw-rw-rw-   0        0        0      904 2023-06-20 00:33:42.000000 turbo_docs-0.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 00:33:51.454308 turbo_docs-0.9.3/turbo_docs/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.9.3/turbo_docs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 00:33:51.469484 turbo_docs-0.9.3/turbo_docs/commands/
+-rw-rw-rw-   0        0        0        0 2023-04-29 00:25:31.000000 turbo_docs-0.9.3/turbo_docs/commands/__init__.py
+-rw-rw-rw-   0        0        0     1214 2023-06-19 23:47:07.000000 turbo_docs-0.9.3/turbo_docs/commands/readme.py
+-rw-rw-rw-   0        0        0      914 2023-06-14 00:14:25.000000 turbo_docs-0.9.3/turbo_docs/generate.py
+drwxrwxrwx   0        0        0        0 2023-06-20 00:33:51.477464 turbo_docs-0.9.3/turbo_docs/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.9.3/turbo_docs/utils/__init__.py
+-rw-rw-rw-   0        0        0      622 2023-06-14 00:14:25.000000 turbo_docs-0.9.3/turbo_docs/utils/cli_options.py
+-rw-rw-rw-   0        0        0     2022 2023-06-12 21:03:28.000000 turbo_docs-0.9.3/turbo_docs/utils/directory.py
+-rw-rw-rw-   0        0        0      992 2023-06-14 00:20:44.000000 turbo_docs-0.9.3/turbo_docs/utils/openai_api.py
+drwxrwxrwx   0        0        0        0 2023-06-20 00:33:51.466066 turbo_docs-0.9.3/turbo_docs.egg-info/
+-rw-rw-rw-   0        0        0     2677 2023-06-20 00:33:51.000000 turbo_docs-0.9.3/turbo_docs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-06-20 00:33:51.000000 turbo_docs-0.9.3/turbo_docs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 00:33:51.000000 turbo_docs-0.9.3/turbo_docs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-06-20 00:33:51.000000 turbo_docs-0.9.3/turbo_docs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       65 2023-06-20 00:33:51.000000 turbo_docs-0.9.3/turbo_docs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-20 00:33:51.000000 turbo_docs-0.9.3/turbo_docs.egg-info/top_level.txt
```

### Comparing `turbo_docs-0.9.2/PKG-INFO` & `turbo_docs-0.9.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,82 +1,88 @@
 Metadata-Version: 2.1
 Name: turbo_docs
-Version: 0.9.2
+Version: 0.9.3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
-# Turbo Docs
+# Turbo Docs 🚀
 
-Turbo Docs is a Python package that helps you generate a professional README.md file for your repository using GPT-3.5 Turbo or GPT-4. It can also copy the text from all files in the current directory to the clipboard, which is useful when working with ChatGPT.
+Turbo Docs is a powerful Python tool that helps developers generate high-quality README.md files for their repositories. It uses OpenAI's GPT-3.5 Turbo and GPT-4 models to create well-structured and informative documentation.
 
-## Installation
+## Why Turbo Docs? 🤔
 
-To install Turbo Docs, you need to have Python 3.6 or higher. You can install the package using pip:
+Writing a good README.md file is essential for any software project, as it provides an overview of the project, its purpose, and how to use it. However, creating a comprehensive and well-structured README.md can be time-consuming. Turbo Docs automates this process, allowing developers to focus on writing code while ensuring their documentation is up-to-date and professional.
+
+## Table of Contents 📚
+
+- [Installation](#installation)
+- [Usage](#usage)
+  - [Generate README.md](#generate-readmemd)
+  - [Copy Directory Text](#copy-directory-text)
+- [Requirements](#requirements)
+- [Contributing](#contributing)
+- [License](#license)
+
+## Installation 💻
+
+To install Turbo Docs, simply run the following command:
 
 ```bash
 pip install turbo_docs
 ```
 
-## Setup
+## Usage 🛠️
+
+### Generate README.md 📝
 
-Before using Turbo Docs, you need to set up your OpenAI API key. If you don't have an API key, create an OpenAI account at https://platform.openai.com/overview. Then, set the API key as an environment variable:
+To generate a README.md file for your repository, navigate to the root directory of your project and run the following command:
 
 ```bash
-export OPENAI_API_KEY=<your_api_key>
+turbo_docs --readme
 ```
 
-## Usage
-
-To use Turbo Docs, navigate to your project directory and run the following command:
+By default, Turbo Docs uses the GPT-4 model. To use the GPT-3.5 Turbo model instead, add the `--gpt3` flag:
 
 ```bash
-turbo_docs
+turbo_docs --readme --gpt3
 ```
 
-### Options
+### Copy Directory Text 📋
 
-- `--copy`: Copy the directory text to the clipboard. Useful for working with ChatGPT.
-- `--readme`: Generate a README.md file. Useful for keeping documentation up to date.
-- `--gpt3`: Use the GPT-3.5 Turbo model instead of GPT-4.
-
-## Configuration
-
-You can configure Turbo Docs to ignore specific files and folders by creating a `turbo_docs.toml` file in your project directory. Add the files and folders you want to ignore in the `ignore` list:
-
-```toml
-ignore = [
-    "__pycache__",
-    "venv",
-    "build",
-    "dist",
-    "*.egg-info",
-    ".git",
-    "README.md",  # This is recommended so that --readme doesn't include the readme file itself
-]
+To copy the text from all files in the current directory to your clipboard, run the following command:
+
+```bash
+turbo_docs --copy
 ```
 
-## Dependencies
+This can be useful when working with ChatGPT.
+
+## Requirements 📦
 
 Turbo Docs requires the following packages:
 
 - requests
 - openai
 - llm-blocks
 - click
 - pyperclip
 - redbaron
 - gitpython
 - toml
 - pathspec
 
-These dependencies will be installed automatically when you install Turbo Docs using pip.
+These dependencies are automatically installed when you install Turbo Docs using pip.
+
+## Contributing 🤝
+
+Contributions are welcome! If you'd like to improve Turbo Docs, please feel free to submit a pull request or open an issue on GitHub.
 
-## License
+## License 📄
 
-Turbo Docs is released under the MIT License.
+Turbo Docs is released under the MIT License. See [LICENSE](LICENSE) for more information.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `turbo_docs-0.9.2/setup.py` & `turbo_docs-0.9.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
 	name="turbo_docs",
-	version="0.9.2",
+	version="0.9.3",
 	packages=find_packages(),
 	install_requires=[
 		"requests",
 		"openai",
 		"click",
 		"pyperclip",
 		"redbaron",
@@ -28,7 +28,10 @@
 		"Programming Language :: Python :: 3.7",
 		"Programming Language :: Python :: 3.8",
 		"Programming Language :: Python :: 3.9",
 	],
 	long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type='text/markdown'
 )
+
+# python setup.py sdist bdist_wheel
+# twine upload dist/*
```

### Comparing `turbo_docs-0.9.2/turbo_docs/generate.py` & `turbo_docs-0.9.3/turbo_docs/generate.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.9.2/turbo_docs/utils/cli_options.py` & `turbo_docs-0.9.3/turbo_docs/utils/cli_options.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.9.2/turbo_docs/utils/directory.py` & `turbo_docs-0.9.3/turbo_docs/utils/directory.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.9.2/turbo_docs/utils/openai_api.py` & `turbo_docs-0.9.3/turbo_docs/utils/openai_api.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.9.2/turbo_docs.egg-info/PKG-INFO` & `turbo_docs-0.9.3/turbo_docs.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,82 +1,88 @@
 Metadata-Version: 2.1
 Name: turbo-docs
-Version: 0.9.2
+Version: 0.9.3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
-# Turbo Docs
+# Turbo Docs 🚀
 
-Turbo Docs is a Python package that helps you generate a professional README.md file for your repository using GPT-3.5 Turbo or GPT-4. It can also copy the text from all files in the current directory to the clipboard, which is useful when working with ChatGPT.
+Turbo Docs is a powerful Python tool that helps developers generate high-quality README.md files for their repositories. It uses OpenAI's GPT-3.5 Turbo and GPT-4 models to create well-structured and informative documentation.
 
-## Installation
+## Why Turbo Docs? 🤔
 
-To install Turbo Docs, you need to have Python 3.6 or higher. You can install the package using pip:
+Writing a good README.md file is essential for any software project, as it provides an overview of the project, its purpose, and how to use it. However, creating a comprehensive and well-structured README.md can be time-consuming. Turbo Docs automates this process, allowing developers to focus on writing code while ensuring their documentation is up-to-date and professional.
+
+## Table of Contents 📚
+
+- [Installation](#installation)
+- [Usage](#usage)
+  - [Generate README.md](#generate-readmemd)
+  - [Copy Directory Text](#copy-directory-text)
+- [Requirements](#requirements)
+- [Contributing](#contributing)
+- [License](#license)
+
+## Installation 💻
+
+To install Turbo Docs, simply run the following command:
 
 ```bash
 pip install turbo_docs
 ```
 
-## Setup
+## Usage 🛠️
+
+### Generate README.md 📝
 
-Before using Turbo Docs, you need to set up your OpenAI API key. If you don't have an API key, create an OpenAI account at https://platform.openai.com/overview. Then, set the API key as an environment variable:
+To generate a README.md file for your repository, navigate to the root directory of your project and run the following command:
 
 ```bash
-export OPENAI_API_KEY=<your_api_key>
+turbo_docs --readme
 ```
 
-## Usage
-
-To use Turbo Docs, navigate to your project directory and run the following command:
+By default, Turbo Docs uses the GPT-4 model. To use the GPT-3.5 Turbo model instead, add the `--gpt3` flag:
 
 ```bash
-turbo_docs
+turbo_docs --readme --gpt3
 ```
 
-### Options
+### Copy Directory Text 📋
 
-- `--copy`: Copy the directory text to the clipboard. Useful for working with ChatGPT.
-- `--readme`: Generate a README.md file. Useful for keeping documentation up to date.
-- `--gpt3`: Use the GPT-3.5 Turbo model instead of GPT-4.
-
-## Configuration
-
-You can configure Turbo Docs to ignore specific files and folders by creating a `turbo_docs.toml` file in your project directory. Add the files and folders you want to ignore in the `ignore` list:
-
-```toml
-ignore = [
-    "__pycache__",
-    "venv",
-    "build",
-    "dist",
-    "*.egg-info",
-    ".git",
-    "README.md",  # This is recommended so that --readme doesn't include the readme file itself
-]
+To copy the text from all files in the current directory to your clipboard, run the following command:
+
+```bash
+turbo_docs --copy
 ```
 
-## Dependencies
+This can be useful when working with ChatGPT.
+
+## Requirements 📦
 
 Turbo Docs requires the following packages:
 
 - requests
 - openai
 - llm-blocks
 - click
 - pyperclip
 - redbaron
 - gitpython
 - toml
 - pathspec
 
-These dependencies will be installed automatically when you install Turbo Docs using pip.
+These dependencies are automatically installed when you install Turbo Docs using pip.
+
+## Contributing 🤝
+
+Contributions are welcome! If you'd like to improve Turbo Docs, please feel free to submit a pull request or open an issue on GitHub.
 
-## License
+## License 📄
 
-Turbo Docs is released under the MIT License.
+Turbo Docs is released under the MIT License. See [LICENSE](LICENSE) for more information.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

