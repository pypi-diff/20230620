# Comparing `tmp/henhoe2vec-1.0.0.tar.gz` & `tmp/henhoe2vec-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "henhoe2vec-1.0.0.tar", last modified: Tue Jun 20 08:11:48 2023, max compression
+gzip compressed data, was "henhoe2vec-1.0.1.tar", last modified: Tue Jun 20 13:35:26 2023, max compression
```

## Comparing `henhoe2vec-1.0.0.tar` & `henhoe2vec-1.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-06-20 08:11:48.688804 henhoe2vec-1.0.0/
--rw-r--r--   0 bob        (501) staff       (20)     1071 2023-06-08 16:39:49.000000 henhoe2vec-1.0.0/LICENSE.txt
--rw-r--r--   0 bob        (501) staff       (20)     6892 2023-06-20 08:11:48.688666 henhoe2vec-1.0.0/PKG-INFO
--rw-r--r--   0 bob        (501) staff       (20)     4741 2023-06-13 09:45:20.000000 henhoe2vec-1.0.0/README.md
--rw-r--r--   0 bob        (501) staff       (20)     1199 2023-06-20 08:11:39.000000 henhoe2vec-1.0.0/pyproject.toml
--rw-r--r--   0 bob        (501) staff       (20)       38 2023-06-20 08:11:48.688850 henhoe2vec-1.0.0/setup.cfg
--rw-r--r--   0 bob        (501) staff       (20)       38 2023-06-13 07:41:13.000000 henhoe2vec-1.0.0/setup.py
-drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-06-20 08:11:48.685393 henhoe2vec-1.0.0/src/
-drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-06-20 08:11:48.686903 henhoe2vec-1.0.0/src/henhoe2vec/
--rw-r--r--   0 bob        (501) staff       (20)       78 2023-06-11 08:46:34.000000 henhoe2vec-1.0.0/src/henhoe2vec/__init__.py
--rw-r--r--   0 bob        (501) staff       (20)     2188 2023-06-10 19:24:50.000000 henhoe2vec-1.0.0/src/henhoe2vec/alias_sampling.py
--rw-r--r--   0 bob        (501) staff       (20)     1820 2023-06-11 08:32:37.000000 henhoe2vec-1.0.0/src/henhoe2vec/embeddings.py
--rw-r--r--   0 bob        (501) staff       (20)     9515 2023-06-13 08:03:06.000000 henhoe2vec-1.0.0/src/henhoe2vec/henhoe2vec.py
--rw-r--r--   0 bob        (501) staff       (20)    12288 2023-06-10 22:17:49.000000 henhoe2vec-1.0.0/src/henhoe2vec/henhoe2vec_walks.py
--rw-r--r--   0 bob        (501) staff       (20)      573 2023-06-10 21:52:42.000000 henhoe2vec-1.0.0/src/henhoe2vec/napkin.py
--rw-r--r--   0 bob        (501) staff       (20)     5262 2023-06-17 08:10:10.000000 henhoe2vec-1.0.0/src/henhoe2vec/utils.py
-drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-06-20 08:11:48.687690 henhoe2vec-1.0.0/src/henhoe2vec.egg-info/
--rw-r--r--   0 bob        (501) staff       (20)     6892 2023-06-20 08:11:48.000000 henhoe2vec-1.0.0/src/henhoe2vec.egg-info/PKG-INFO
--rw-r--r--   0 bob        (501) staff       (20)      566 2023-06-20 08:11:48.000000 henhoe2vec-1.0.0/src/henhoe2vec.egg-info/SOURCES.txt
--rw-r--r--   0 bob        (501) staff       (20)        1 2023-06-20 08:11:48.000000 henhoe2vec-1.0.0/src/henhoe2vec.egg-info/dependency_links.txt
--rw-r--r--   0 bob        (501) staff       (20)       76 2023-06-20 08:11:48.000000 henhoe2vec-1.0.0/src/henhoe2vec.egg-info/requires.txt
--rw-r--r--   0 bob        (501) staff       (20)       11 2023-06-20 08:11:48.000000 henhoe2vec-1.0.0/src/henhoe2vec.egg-info/top_level.txt
-drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-06-20 08:11:48.688421 henhoe2vec-1.0.0/tests/
--rw-r--r--   0 bob        (501) staff       (20)     1095 2023-06-10 22:18:24.000000 henhoe2vec-1.0.0/tests/test_alias_sampling.py
--rw-r--r--   0 bob        (501) staff       (20)      764 2023-06-10 22:18:24.000000 henhoe2vec-1.0.0/tests/test_embeddings.py
--rw-r--r--   0 bob        (501) staff       (20)     2171 2023-06-14 09:26:45.000000 henhoe2vec-1.0.0/tests/test_henhoe2vec.py
--rw-r--r--   0 bob        (501) staff       (20)     3913 2023-06-10 22:18:24.000000 henhoe2vec-1.0.0/tests/test_henhoe2vec_walks.py
--rw-r--r--   0 bob        (501) staff       (20)     4215 2023-06-17 08:08:24.000000 henhoe2vec-1.0.0/tests/test_utils.py
+drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-06-20 13:35:26.502830 henhoe2vec-1.0.1/
+-rw-r--r--   0 bob        (501) staff       (20)     1071 2023-06-08 16:39:49.000000 henhoe2vec-1.0.1/LICENSE.txt
+-rw-r--r--   0 bob        (501) staff       (20)     7136 2023-06-20 13:35:26.502679 henhoe2vec-1.0.1/PKG-INFO
+-rw-r--r--   0 bob        (501) staff       (20)     4985 2023-06-20 13:30:29.000000 henhoe2vec-1.0.1/README.md
+-rw-r--r--   0 bob        (501) staff       (20)     1199 2023-06-20 13:33:41.000000 henhoe2vec-1.0.1/pyproject.toml
+-rw-r--r--   0 bob        (501) staff       (20)       38 2023-06-20 13:35:26.502879 henhoe2vec-1.0.1/setup.cfg
+-rw-r--r--   0 bob        (501) staff       (20)       38 2023-06-13 07:41:13.000000 henhoe2vec-1.0.1/setup.py
+drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-06-20 13:35:26.498708 henhoe2vec-1.0.1/src/
+drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-06-20 13:35:26.500370 henhoe2vec-1.0.1/src/henhoe2vec/
+-rw-r--r--   0 bob        (501) staff       (20)       78 2023-06-11 08:46:34.000000 henhoe2vec-1.0.1/src/henhoe2vec/__init__.py
+-rw-r--r--   0 bob        (501) staff       (20)     2188 2023-06-10 19:24:50.000000 henhoe2vec-1.0.1/src/henhoe2vec/alias_sampling.py
+-rw-r--r--   0 bob        (501) staff       (20)     2109 2023-06-20 13:32:52.000000 henhoe2vec-1.0.1/src/henhoe2vec/embeddings.py
+-rw-r--r--   0 bob        (501) staff       (20)    10636 2023-06-20 13:32:52.000000 henhoe2vec-1.0.1/src/henhoe2vec/henhoe2vec.py
+-rw-r--r--   0 bob        (501) staff       (20)    12288 2023-06-10 22:17:49.000000 henhoe2vec-1.0.1/src/henhoe2vec/henhoe2vec_walks.py
+-rw-r--r--   0 bob        (501) staff       (20)      573 2023-06-10 21:52:42.000000 henhoe2vec-1.0.1/src/henhoe2vec/napkin.py
+-rw-r--r--   0 bob        (501) staff       (20)     5262 2023-06-17 08:10:10.000000 henhoe2vec-1.0.1/src/henhoe2vec/utils.py
+drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-06-20 13:35:26.501401 henhoe2vec-1.0.1/src/henhoe2vec.egg-info/
+-rw-r--r--   0 bob        (501) staff       (20)     7136 2023-06-20 13:35:26.000000 henhoe2vec-1.0.1/src/henhoe2vec.egg-info/PKG-INFO
+-rw-r--r--   0 bob        (501) staff       (20)      566 2023-06-20 13:35:26.000000 henhoe2vec-1.0.1/src/henhoe2vec.egg-info/SOURCES.txt
+-rw-r--r--   0 bob        (501) staff       (20)        1 2023-06-20 13:35:26.000000 henhoe2vec-1.0.1/src/henhoe2vec.egg-info/dependency_links.txt
+-rw-r--r--   0 bob        (501) staff       (20)       76 2023-06-20 13:35:26.000000 henhoe2vec-1.0.1/src/henhoe2vec.egg-info/requires.txt
+-rw-r--r--   0 bob        (501) staff       (20)       11 2023-06-20 13:35:26.000000 henhoe2vec-1.0.1/src/henhoe2vec.egg-info/top_level.txt
+drwxr-xr-x   0 bob        (501) staff       (20)        0 2023-06-20 13:35:26.502458 henhoe2vec-1.0.1/tests/
+-rw-r--r--   0 bob        (501) staff       (20)     1095 2023-06-10 22:18:24.000000 henhoe2vec-1.0.1/tests/test_alias_sampling.py
+-rw-r--r--   0 bob        (501) staff       (20)      764 2023-06-10 22:18:24.000000 henhoe2vec-1.0.1/tests/test_embeddings.py
+-rw-r--r--   0 bob        (501) staff       (20)     2171 2023-06-14 09:26:45.000000 henhoe2vec-1.0.1/tests/test_henhoe2vec.py
+-rw-r--r--   0 bob        (501) staff       (20)     3913 2023-06-10 22:18:24.000000 henhoe2vec-1.0.1/tests/test_henhoe2vec_walks.py
+-rw-r--r--   0 bob        (501) staff       (20)     4215 2023-06-17 08:08:24.000000 henhoe2vec-1.0.1/tests/test_utils.py
```

### Comparing `henhoe2vec-1.0.0/LICENSE.txt` & `henhoe2vec-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `henhoe2vec-1.0.0/PKG-INFO` & `henhoe2vec-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: henhoe2vec
-Version: 1.0.0
+Version: 1.0.1
 Summary: Implementation of the HeNHoE-2vec algorithm by Valentini et al. (2021).
 Author-email: Robert Giesler <robert.giesler@rwth-aachen.de>
 License: MIT License
         
         Copyright (c) 2023 Robert Giesler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,14 +36,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+![PyPI](https://img.shields.io/pypi/v/henhoe2vec)
 [![Tests](https://github.com/Bertr0/HeNHoE-2vec/actions/workflows/tests.yml/badge.svg)](https://github.com/Bertr0/HeNHoE-2vec/actions/workflows/tests.yml)
 
 # HeNHoE-2vec
 A Python implementation of the HeNHoE-2vec algorithm by [Valentini et al.](https://arxiv.org/abs/2101.01425) for the embedding of networks with heterogeneous nodes and homogeneous edges (HeNHoE).
 
 _Note_: HeNHoE networks are analogous to multilayer networks: in HeNHoE networks, each node has a distinct node type, and in multilayer networks, each node belongs to a distinct layer. The terms `type` and `layer` may therefore be regarded synonymous. Throughout the code and for the remainder of this documentation, we will use the terms `multilayer network` and `layer` as opposed to `HeNHoE network` and `type`.
 
@@ -72,40 +73,43 @@
 The many individual steps of HeNHoE-2vec are accumulated in a single `run()` method in the `henhoe2vec.henhoe2vec` module. HeNHoE-2vec can be run from start to finish as follows:
 ```python
 import henho2vec as hh2v
 
 hh2v.henhoe2vec.run(input_csv, output_dir)
 ```
 
-`input_csv` is the path to the multilayer edge list of the network to be embedded (csv file with tab delimiter, no header, no index). `output_dir` is the path to the output directory where the embedding files will be saved. The `run()` method takes a bunch of other optional parameters which can be used to configure HeNHoE-2vec. A comprehensive overview of parameters can be found in the code documentation.
+`input_csv` is the path to the multilayer edge list of the network to be embedded (csv file with no index). `output_dir` is the path to the output directory where the embedding files will be saved. The `run()` method takes a bunch of other optional parameters which can be used to configure HeNHoE-2vec. A comprehensive overview of parameters can be found in the code documentation.
 
 ### As a Python Script
-To run HeNHoE-2vec as a script, clone this repositiory using
+To run HeNHoE-2vec as a script, clone this repository using
 ```
 $ git clone git@github.com:Bertr0/HeNHoE-2vec.git
 ```
 , install the requirements found in `requirements.txt` and run the following command from the root of the repository:
 ```
 $ python3 -m src.henhoe2vec.henhoe2vec --input <input_path> --output_dir <output_dir_path>
 ```
 
-This will generate node embedddings for the nodes of the network specified by the mutlilayer edge list saved at `<input_path>` and saves the embedding files in `<output_dir>`.
+This will generate node embeddings for the nodes of the network specified by the multilayer edge list saved at `<input_path>` and saves the embedding files in `<output_dir>`.
 
 Run `python3 -m src.henhoe2vec.henhoe2vec --help` from the root of the repository to show an overview of all arguments taken by the script. The following table also shows an overview of all arguments:
 
 #### Script Arguments
 | Argument | Type | Description | Default Value |
 | -------- | ---- | ----------- | ------------- |
-| `--input` | str | Path to the multilayer edge list of the network to be embedded (.csv file with tab delimiter, no header, no index). | - |
+| `--input` | str | Path to the multilayer edge list of the network to be embedded (csv file with no index). | - |
+| `--sep` | str | Delimiter of the input csv edge list. | "\t" |
+| `--header` | store_true | Pass this argument if the input csv edge list has a header. | - |
+| `--output-name` | str | Name of the output .csv file (without suffix). | "embeddings" |
 | `--is-directed` | store_true | Pass this argument if the network is directed. | - |
 | `--edges-are-distances` | store_true | Pass this argument if edge weights indicate distance between nodes (opposed to weight/similarity). | - |
 | `--output_dir` | str | Path of the output directory where the embedding files will be saved. | - |
 | `--dimensions` | int | The dimensionality of the embeddings. | 128 |
 | `--walk-length` | int | Length of each random walk. | 20 |
-| `--num-walks` | int | Number of randwom walks to simulate for each node. | 10 |
+| `--num-walks` | int | Number of random walks to simulate for each node. | 10 |
 | `--p` | float | Return parameter `p` from the node2vec algorithm. | 1.0 |
-| `--q` | float | In-out parameter `q` from the node2vec algoritym. | 0.5 |
+| `--q` | float | In-out parameter `q` from the node2vec algorithm. | 0.5 |
 | `--s` | float | Default switching parameter for layer pairs which are not specified in the `--s-dict` argument. | 1.0 |
-| `--s-dict` | list | Switching parameters for specific layer pairs in a dict-like manner. Pass the names of layer pairs followed by their switching parameters, separated by whitespaces. E.g., if the switching parameter from `layer1` to `layer2` is `0.5` and the switching parameter from `layer2` to `layer1` is `0.7`, you would pass `layer1 layer2 0.5 layer2 layer1 0.7`. Note that layer pairs are directed. For all layer pairs which are not specified here, the default parameter `--s` is adopted. | empty list |
+| `--s-dict` | list | Switching parameters for specific layer pairs in a dict-like manner. Pass the names of layer pairs followed by their switching parameters, separated by white spaces. E.g., if the switching parameter from `layer1` to `layer2` is `0.5` and the switching parameter from `layer2` to `layer1` is `0.7`, you would pass `layer1 layer2 0.5 layer2 layer1 0.7`. Note that layer pairs are directed. For all layer pairs which are not specified here, the default parameter `--s` is adopted. | empty list |
 | `--window-size` | int | Context size for the word2vec optimization. | 10 |
 | `--epochs` | int | Number of epochs in SGD. | 1 |
 | `--workers` | int | Number of parallel workers (threads). | 8 |
```

### Comparing `henhoe2vec-1.0.0/README.md` & `henhoe2vec-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+![PyPI](https://img.shields.io/pypi/v/henhoe2vec)
 [![Tests](https://github.com/Bertr0/HeNHoE-2vec/actions/workflows/tests.yml/badge.svg)](https://github.com/Bertr0/HeNHoE-2vec/actions/workflows/tests.yml)
 
 # HeNHoE-2vec
 A Python implementation of the HeNHoE-2vec algorithm by [Valentini et al.](https://arxiv.org/abs/2101.01425) for the embedding of networks with heterogeneous nodes and homogeneous edges (HeNHoE).
 
 _Note_: HeNHoE networks are analogous to multilayer networks: in HeNHoE networks, each node has a distinct node type, and in multilayer networks, each node belongs to a distinct layer. The terms `type` and `layer` may therefore be regarded synonymous. Throughout the code and for the remainder of this documentation, we will use the terms `multilayer network` and `layer` as opposed to `HeNHoE network` and `type`.
 
@@ -31,40 +32,43 @@
 The many individual steps of HeNHoE-2vec are accumulated in a single `run()` method in the `henhoe2vec.henhoe2vec` module. HeNHoE-2vec can be run from start to finish as follows:
 ```python
 import henho2vec as hh2v
 
 hh2v.henhoe2vec.run(input_csv, output_dir)
 ```
 
-`input_csv` is the path to the multilayer edge list of the network to be embedded (csv file with tab delimiter, no header, no index). `output_dir` is the path to the output directory where the embedding files will be saved. The `run()` method takes a bunch of other optional parameters which can be used to configure HeNHoE-2vec. A comprehensive overview of parameters can be found in the code documentation.
+`input_csv` is the path to the multilayer edge list of the network to be embedded (csv file with no index). `output_dir` is the path to the output directory where the embedding files will be saved. The `run()` method takes a bunch of other optional parameters which can be used to configure HeNHoE-2vec. A comprehensive overview of parameters can be found in the code documentation.
 
 ### As a Python Script
-To run HeNHoE-2vec as a script, clone this repositiory using
+To run HeNHoE-2vec as a script, clone this repository using
 ```
 $ git clone git@github.com:Bertr0/HeNHoE-2vec.git
 ```
 , install the requirements found in `requirements.txt` and run the following command from the root of the repository:
 ```
 $ python3 -m src.henhoe2vec.henhoe2vec --input <input_path> --output_dir <output_dir_path>
 ```
 
-This will generate node embedddings for the nodes of the network specified by the mutlilayer edge list saved at `<input_path>` and saves the embedding files in `<output_dir>`.
+This will generate node embeddings for the nodes of the network specified by the multilayer edge list saved at `<input_path>` and saves the embedding files in `<output_dir>`.
 
 Run `python3 -m src.henhoe2vec.henhoe2vec --help` from the root of the repository to show an overview of all arguments taken by the script. The following table also shows an overview of all arguments:
 
 #### Script Arguments
 | Argument | Type | Description | Default Value |
 | -------- | ---- | ----------- | ------------- |
-| `--input` | str | Path to the multilayer edge list of the network to be embedded (.csv file with tab delimiter, no header, no index). | - |
+| `--input` | str | Path to the multilayer edge list of the network to be embedded (csv file with no index). | - |
+| `--sep` | str | Delimiter of the input csv edge list. | "\t" |
+| `--header` | store_true | Pass this argument if the input csv edge list has a header. | - |
+| `--output-name` | str | Name of the output .csv file (without suffix). | "embeddings" |
 | `--is-directed` | store_true | Pass this argument if the network is directed. | - |
 | `--edges-are-distances` | store_true | Pass this argument if edge weights indicate distance between nodes (opposed to weight/similarity). | - |
 | `--output_dir` | str | Path of the output directory where the embedding files will be saved. | - |
 | `--dimensions` | int | The dimensionality of the embeddings. | 128 |
 | `--walk-length` | int | Length of each random walk. | 20 |
-| `--num-walks` | int | Number of randwom walks to simulate for each node. | 10 |
+| `--num-walks` | int | Number of random walks to simulate for each node. | 10 |
 | `--p` | float | Return parameter `p` from the node2vec algorithm. | 1.0 |
-| `--q` | float | In-out parameter `q` from the node2vec algoritym. | 0.5 |
+| `--q` | float | In-out parameter `q` from the node2vec algorithm. | 0.5 |
 | `--s` | float | Default switching parameter for layer pairs which are not specified in the `--s-dict` argument. | 1.0 |
-| `--s-dict` | list | Switching parameters for specific layer pairs in a dict-like manner. Pass the names of layer pairs followed by their switching parameters, separated by whitespaces. E.g., if the switching parameter from `layer1` to `layer2` is `0.5` and the switching parameter from `layer2` to `layer1` is `0.7`, you would pass `layer1 layer2 0.5 layer2 layer1 0.7`. Note that layer pairs are directed. For all layer pairs which are not specified here, the default parameter `--s` is adopted. | empty list |
+| `--s-dict` | list | Switching parameters for specific layer pairs in a dict-like manner. Pass the names of layer pairs followed by their switching parameters, separated by white spaces. E.g., if the switching parameter from `layer1` to `layer2` is `0.5` and the switching parameter from `layer2` to `layer1` is `0.7`, you would pass `layer1 layer2 0.5 layer2 layer1 0.7`. Note that layer pairs are directed. For all layer pairs which are not specified here, the default parameter `--s` is adopted. | empty list |
 | `--window-size` | int | Context size for the word2vec optimization. | 10 |
 | `--epochs` | int | Number of epochs in SGD. | 1 |
 | `--workers` | int | Number of parallel workers (threads). | 8 |
```

### Comparing `henhoe2vec-1.0.0/pyproject.toml` & `henhoe2vec-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "henhoe2vec"
-version = "1.0.0"
+version = "1.0.1"
 description = "Implementation of the HeNHoE-2vec algorithm by Valentini et al. (2021)."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 authors = [
     {name = "Robert Giesler", email = "robert.giesler@rwth-aachen.de"}
 ]
```

### Comparing `henhoe2vec-1.0.0/src/henhoe2vec/alias_sampling.py` & `henhoe2vec-1.0.1/src/henhoe2vec/alias_sampling.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-1.0.0/src/henhoe2vec/henhoe2vec.py` & `henhoe2vec-1.0.1/src/henhoe2vec/henhoe2vec.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,20 +11,39 @@
     """
     parser = argparse.ArgumentParser(description="Run HeNHoE-2vec.")
 
     parser.add_argument(
         "--input",
         type=str,
         help=(
-            "Path to the multilayer edge list of the network to be embedded (.csv file"
-            " with tab delimiter, no header, no index)."
+            "Path to the multilayer edge list of the network to be embedded (csv file"
+            " with no index)."
         ),
     )
 
     parser.add_argument(
+        "--sep", type=str, help=("Delimiter of the input csv edge list."), default="\t"
+    )
+
+    parser.add_argument(
+        "--header",
+        type="store_true",
+        help=("Pass this argument if the input csv edge list has a header."),
+    )
+
+    parser.add_argument(
+        "--output-name",
+        type=str,
+        help=(
+            "Name of the output .csv file (without suffix). Default is 'embeddings'."
+        ),
+        default="embeddings",
+    )
+
+    parser.add_argument(
         "--is-directed",
         action="store_true",
         help="Pass this argument if the network is directed.",
     )
 
     parser.add_argument(
         "--edges-are-distance",
@@ -32,15 +51,15 @@
         help=(
             "Pass this argument if edge weights indicate distance between nodes"
             " (opposed to weight/similarity)."
         ),
     )
 
     parser.add_argument(
-        "--output_dir",
+        "--output-dir",
         type=str,
         help="Path of the output directory where the embedding files will be saved.",
     )
 
     parser.add_argument(
         "--dimensions",
         type=int,
@@ -163,14 +182,17 @@
 
     return switching_dict
 
 
 def run(
     input_csv,
     output_dir,
+    sep="\t",
+    header=False,
+    output_name="embeddings",
     is_directed=False,
     edges_are_distance=False,
     dims=128,
     walk_length=20,
     num_walks=10,
     p=1.0,
     q=0.5,
@@ -184,17 +206,23 @@
     Main method to embed the nodes of a HeNHoE (multilayer) network using the
     HeNHoE-2vec algorithm. Results are saved as .emb and .csv files.
 
     Parameters
     ----------
     input_csv : str
         Path to the multilayer edge list of the network to be embedded (csv file with
-        tab delimiter, no header, no index).
+        no index).
     output_dir : str
         Path of the output directory where the embedding files will be saved.
+    sep : str
+        Delimiter of the input csv edge list. Default is "\\t".
+    header : bool
+        Whether the input csv edge list has a header. Default is False.
+    output_name : str
+        Name of the output .csv file (without suffix). Default is "embeddings".
     is_directed : bool
         Whether the network is directed. Default is False.
     edges_are_distance : bool
         Whether edge weights indicate distance between nodes (opposed to
         weight/similarity). Default is False.
     dims : int
         The dimensionality of the embeddings. Default is 128.
@@ -232,15 +260,15 @@
     """
     start = time.time()
     # Parse multilayer network
     if verbose:
         N_nx = utils.timed_invoke(
             "parsing edgelist",
             lambda: utils.parse_multilayer_edgelist(
-                input_csv, is_directed, edges_are_distance
+                input_csv, is_directed, edges_are_distance, sep=sep, header=header
             ),
         )
     else:
         N_nx = utils.parse_multilayer_edgelist(
             input_csv, is_directed, edges_are_distance
         )
 
@@ -266,20 +294,34 @@
         walks = hh2v.simulate_walks(num_walks, walk_length)
 
     # Learn and save embeddings
     if verbose:
         utils.timed_invoke(
             "learning and saving embeddings",
             lambda: embeddings.generate_embeddings(
-                walks, output_dir, dims, window_size, epochs, workers, verbose
+                walks,
+                output_dir,
+                output_name,
+                dims,
+                window_size,
+                epochs,
+                workers,
+                verbose,
             ),
         )
     else:
         embeddings.generate_embeddings(
-            walks, output_dir, dims, window_size, epochs, workers, verbose
+            walks,
+            output_dir,
+            output_name,
+            dims,
+            window_size,
+            epochs,
+            workers,
+            verbose,
         )
 
     finish = time.time()
     if verbose:
         print(
             f"Completed multilayer network embedding in {finish - start} seconds."
             f" See results in {output_dir}."
@@ -290,14 +332,17 @@
     if __name__ == "__main__":
         args = parse_args()
         # Parse arguments s and s-dict
         s = parse_switching_param(args.s, args.s_dict)
         run(
             input_csv=args.input,
             output_dir=args.output_dir,
+            sep=args.sep,
+            header=args.header,
+            output_name=args.output_name,
             is_directed=args.is_directed,
             edges_are_distance=args.edges_are_distance,
             dims=args.dimensions,
             walk_length=args.walk_length,
             num_walks=args.num_walks,
             p=args.p,
             q=args.q,
```

### Comparing `henhoe2vec-1.0.0/src/henhoe2vec/henhoe2vec_walks.py` & `henhoe2vec-1.0.1/src/henhoe2vec/henhoe2vec_walks.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-1.0.0/src/henhoe2vec/napkin.py` & `henhoe2vec-1.0.1/src/henhoe2vec/napkin.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-1.0.0/src/henhoe2vec/utils.py` & `henhoe2vec-1.0.1/src/henhoe2vec/utils.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-1.0.0/src/henhoe2vec.egg-info/PKG-INFO` & `henhoe2vec-1.0.1/src/henhoe2vec.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: henhoe2vec
-Version: 1.0.0
+Version: 1.0.1
 Summary: Implementation of the HeNHoE-2vec algorithm by Valentini et al. (2021).
 Author-email: Robert Giesler <robert.giesler@rwth-aachen.de>
 License: MIT License
         
         Copyright (c) 2023 Robert Giesler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,14 +36,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+![PyPI](https://img.shields.io/pypi/v/henhoe2vec)
 [![Tests](https://github.com/Bertr0/HeNHoE-2vec/actions/workflows/tests.yml/badge.svg)](https://github.com/Bertr0/HeNHoE-2vec/actions/workflows/tests.yml)
 
 # HeNHoE-2vec
 A Python implementation of the HeNHoE-2vec algorithm by [Valentini et al.](https://arxiv.org/abs/2101.01425) for the embedding of networks with heterogeneous nodes and homogeneous edges (HeNHoE).
 
 _Note_: HeNHoE networks are analogous to multilayer networks: in HeNHoE networks, each node has a distinct node type, and in multilayer networks, each node belongs to a distinct layer. The terms `type` and `layer` may therefore be regarded synonymous. Throughout the code and for the remainder of this documentation, we will use the terms `multilayer network` and `layer` as opposed to `HeNHoE network` and `type`.
 
@@ -72,40 +73,43 @@
 The many individual steps of HeNHoE-2vec are accumulated in a single `run()` method in the `henhoe2vec.henhoe2vec` module. HeNHoE-2vec can be run from start to finish as follows:
 ```python
 import henho2vec as hh2v
 
 hh2v.henhoe2vec.run(input_csv, output_dir)
 ```
 
-`input_csv` is the path to the multilayer edge list of the network to be embedded (csv file with tab delimiter, no header, no index). `output_dir` is the path to the output directory where the embedding files will be saved. The `run()` method takes a bunch of other optional parameters which can be used to configure HeNHoE-2vec. A comprehensive overview of parameters can be found in the code documentation.
+`input_csv` is the path to the multilayer edge list of the network to be embedded (csv file with no index). `output_dir` is the path to the output directory where the embedding files will be saved. The `run()` method takes a bunch of other optional parameters which can be used to configure HeNHoE-2vec. A comprehensive overview of parameters can be found in the code documentation.
 
 ### As a Python Script
-To run HeNHoE-2vec as a script, clone this repositiory using
+To run HeNHoE-2vec as a script, clone this repository using
 ```
 $ git clone git@github.com:Bertr0/HeNHoE-2vec.git
 ```
 , install the requirements found in `requirements.txt` and run the following command from the root of the repository:
 ```
 $ python3 -m src.henhoe2vec.henhoe2vec --input <input_path> --output_dir <output_dir_path>
 ```
 
-This will generate node embedddings for the nodes of the network specified by the mutlilayer edge list saved at `<input_path>` and saves the embedding files in `<output_dir>`.
+This will generate node embeddings for the nodes of the network specified by the multilayer edge list saved at `<input_path>` and saves the embedding files in `<output_dir>`.
 
 Run `python3 -m src.henhoe2vec.henhoe2vec --help` from the root of the repository to show an overview of all arguments taken by the script. The following table also shows an overview of all arguments:
 
 #### Script Arguments
 | Argument | Type | Description | Default Value |
 | -------- | ---- | ----------- | ------------- |
-| `--input` | str | Path to the multilayer edge list of the network to be embedded (.csv file with tab delimiter, no header, no index). | - |
+| `--input` | str | Path to the multilayer edge list of the network to be embedded (csv file with no index). | - |
+| `--sep` | str | Delimiter of the input csv edge list. | "\t" |
+| `--header` | store_true | Pass this argument if the input csv edge list has a header. | - |
+| `--output-name` | str | Name of the output .csv file (without suffix). | "embeddings" |
 | `--is-directed` | store_true | Pass this argument if the network is directed. | - |
 | `--edges-are-distances` | store_true | Pass this argument if edge weights indicate distance between nodes (opposed to weight/similarity). | - |
 | `--output_dir` | str | Path of the output directory where the embedding files will be saved. | - |
 | `--dimensions` | int | The dimensionality of the embeddings. | 128 |
 | `--walk-length` | int | Length of each random walk. | 20 |
-| `--num-walks` | int | Number of randwom walks to simulate for each node. | 10 |
+| `--num-walks` | int | Number of random walks to simulate for each node. | 10 |
 | `--p` | float | Return parameter `p` from the node2vec algorithm. | 1.0 |
-| `--q` | float | In-out parameter `q` from the node2vec algoritym. | 0.5 |
+| `--q` | float | In-out parameter `q` from the node2vec algorithm. | 0.5 |
 | `--s` | float | Default switching parameter for layer pairs which are not specified in the `--s-dict` argument. | 1.0 |
-| `--s-dict` | list | Switching parameters for specific layer pairs in a dict-like manner. Pass the names of layer pairs followed by their switching parameters, separated by whitespaces. E.g., if the switching parameter from `layer1` to `layer2` is `0.5` and the switching parameter from `layer2` to `layer1` is `0.7`, you would pass `layer1 layer2 0.5 layer2 layer1 0.7`. Note that layer pairs are directed. For all layer pairs which are not specified here, the default parameter `--s` is adopted. | empty list |
+| `--s-dict` | list | Switching parameters for specific layer pairs in a dict-like manner. Pass the names of layer pairs followed by their switching parameters, separated by white spaces. E.g., if the switching parameter from `layer1` to `layer2` is `0.5` and the switching parameter from `layer2` to `layer1` is `0.7`, you would pass `layer1 layer2 0.5 layer2 layer1 0.7`. Note that layer pairs are directed. For all layer pairs which are not specified here, the default parameter `--s` is adopted. | empty list |
 | `--window-size` | int | Context size for the word2vec optimization. | 10 |
 | `--epochs` | int | Number of epochs in SGD. | 1 |
 | `--workers` | int | Number of parallel workers (threads). | 8 |
```

### Comparing `henhoe2vec-1.0.0/src/henhoe2vec.egg-info/SOURCES.txt` & `henhoe2vec-1.0.1/src/henhoe2vec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `henhoe2vec-1.0.0/tests/test_alias_sampling.py` & `henhoe2vec-1.0.1/tests/test_alias_sampling.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-1.0.0/tests/test_embeddings.py` & `henhoe2vec-1.0.1/tests/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-1.0.0/tests/test_henhoe2vec.py` & `henhoe2vec-1.0.1/tests/test_henhoe2vec.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-1.0.0/tests/test_henhoe2vec_walks.py` & `henhoe2vec-1.0.1/tests/test_henhoe2vec_walks.py`

 * *Files identical despite different names*

### Comparing `henhoe2vec-1.0.0/tests/test_utils.py` & `henhoe2vec-1.0.1/tests/test_utils.py`

 * *Files identical despite different names*

