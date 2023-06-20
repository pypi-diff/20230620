# Comparing `tmp/polyswarm-3.2.1.tar.gz` & `tmp/polyswarm-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyswarm-3.2.1.tar", last modified: Tue May 30 22:09:01 2023, max compression
+gzip compressed data, was "polyswarm-3.3.0.tar", last modified: Tue Jun 20 20:14:41 2023, max compression
```

## Comparing `polyswarm-3.2.1.tar` & `polyswarm-3.3.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 22:09:01.136853 polyswarm-3.2.1/
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-05-30 22:08:39.000000 polyswarm-3.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2804 2023-05-30 22:09:01.136853 polyswarm-3.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2011 2023-05-30 22:08:39.000000 polyswarm-3.2.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 22:09:01.136853 polyswarm-3.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1658 2023-05-30 22:08:39.000000 polyswarm-3.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 22:09:01.132853 polyswarm-3.2.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 22:09:01.132853 polyswarm-3.2.1/src/polyswarm/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      526 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 22:09:01.136853 polyswarm-3.2.1/src/polyswarm/client/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2160 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/client/download.py
--rw-rw-rw-   0 root         (0) root         (0)     3734 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/client/engine.py
--rw-rw-rw-   0 root         (0) root         (0)     1489 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/client/families.py
--rw-rw-rw-   0 root         (0) root         (0)     4528 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/client/historical.py
--rw-rw-rw-   0 root         (0) root         (0)     2430 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/client/links.py
--rw-rw-rw-   0 root         (0) root         (0)     2310 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/client/live.py
--rw-rw-rw-   0 root         (0) root         (0)     1567 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/client/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     6130 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/client/polyswarm.py
--rw-rw-rw-   0 root         (0) root         (0)     2163 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/client/rules.py
--rw-rw-rw-   0 root         (0) root         (0)     1495 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/client/sandbox.py
--rw-rw-rw-   0 root         (0) root         (0)     6349 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/client/scan.py
--rw-rw-rw-   0 root         (0) root         (0)     5916 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/client/search.py
--rw-rw-rw-   0 root         (0) root         (0)     1070 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/client/tags.py
--rw-rw-rw-   0 root         (0) root         (0)     2736 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/client/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      389 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 22:09:01.136853 polyswarm-3.2.1/src/polyswarm/formatters/
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/formatters/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1276 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/formatters/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2153 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/formatters/hashes.py
--rw-rw-rw-   0 root         (0) root         (0)     5618 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/formatters/json.py
--rw-rw-rw-   0 root         (0) root         (0)    22994 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/formatters/text.py
--rw-rw-rw-   0 root         (0) root         (0)     9994 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/polyswarm.py
--rw-rw-rw-   0 root         (0) root         (0)     3760 2023-05-30 22:08:39.000000 polyswarm-3.2.1/src/polyswarm/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 22:09:01.132853 polyswarm-3.2.1/src/polyswarm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2804 2023-05-30 22:09:01.000000 polyswarm-3.2.1/src/polyswarm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1023 2023-05-30 22:09:01.000000 polyswarm-3.2.1/src/polyswarm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 22:09:01.000000 polyswarm-3.2.1/src/polyswarm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-05-30 22:09:01.000000 polyswarm-3.2.1/src/polyswarm.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      164 2023-05-30 22:09:01.000000 polyswarm-3.2.1/src/polyswarm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-30 22:09:01.000000 polyswarm-3.2.1/src/polyswarm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:14:41.561974 polyswarm-3.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-06-20 20:13:59.000000 polyswarm-3.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2664 2023-06-20 20:14:41.561974 polyswarm-3.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2011 2023-06-20 20:13:59.000000 polyswarm-3.3.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 20:14:41.561974 polyswarm-3.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1467 2023-06-20 20:13:59.000000 polyswarm-3.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:14:41.557974 polyswarm-3.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:14:41.557974 polyswarm-3.3.0/src/polyswarm/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      526 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:14:41.561974 polyswarm-3.3.0/src/polyswarm/client/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2716 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/client/download.py
+-rw-rw-rw-   0 root         (0) root         (0)     3734 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/client/engine.py
+-rw-rw-rw-   0 root         (0) root         (0)     1489 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/client/families.py
+-rw-rw-rw-   0 root         (0) root         (0)     4528 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/client/historical.py
+-rw-rw-rw-   0 root         (0) root         (0)     2430 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/client/links.py
+-rw-rw-rw-   0 root         (0) root         (0)     2310 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/client/live.py
+-rw-rw-rw-   0 root         (0) root         (0)     1567 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/client/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     6156 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/client/polyswarm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2163 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/client/rules.py
+-rw-rw-rw-   0 root         (0) root         (0)     4000 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/client/sandbox.py
+-rw-rw-rw-   0 root         (0) root         (0)     6349 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/client/scan.py
+-rw-rw-rw-   0 root         (0) root         (0)     5916 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/client/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/client/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/client/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      389 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:14:41.561974 polyswarm-3.3.0/src/polyswarm/formatters/
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/formatters/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/formatters/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2153 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/formatters/hashes.py
+-rw-rw-rw-   0 root         (0) root         (0)     5722 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/formatters/json.py
+-rw-rw-rw-   0 root         (0) root         (0)    24719 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/formatters/text.py
+-rw-rw-rw-   0 root         (0) root         (0)    10475 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/polyswarm.py
+-rw-rw-rw-   0 root         (0) root         (0)     3760 2023-06-20 20:13:59.000000 polyswarm-3.3.0/src/polyswarm/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:14:41.557974 polyswarm-3.3.0/src/polyswarm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2664 2023-06-20 20:14:41.000000 polyswarm-3.3.0/src/polyswarm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-06-20 20:14:41.000000 polyswarm-3.3.0/src/polyswarm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 20:14:41.000000 polyswarm-3.3.0/src/polyswarm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-06-20 20:14:41.000000 polyswarm-3.3.0/src/polyswarm.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      124 2023-06-20 20:14:41.000000 polyswarm-3.3.0/src/polyswarm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-20 20:14:41.000000 polyswarm-3.3.0/src/polyswarm.egg-info/top_level.txt
```

### Comparing `polyswarm-3.2.1/LICENSE` & `polyswarm-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.1/PKG-INFO` & `polyswarm-3.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: polyswarm
-Version: 3.2.1
+Version: 3.3.0
 Summary: CLI for using the PolySwarm Customer APIs
 Home-page: https://github.com/polyswarm/polyswarm-cli
 Author: PolySwarm Developers
 Author-email: info@polyswarm.io
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,<4
+Requires-Python: >=3.5,<4
 Description-Content-Type: text/markdown
 Provides-Extra: yara
 License-File: LICENSE
 
 
 # Polyswarm Customer CLI
```

### Comparing `polyswarm-3.2.1/README.md` & `polyswarm-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.1/setup.py` & `polyswarm-3.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,47 +5,44 @@
 # The README.md will be used as the content for the PyPi package details page on the Python Package Index.
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 
 setup(
     name='polyswarm',
-    version='3.2.1',
+    version='3.3.0',
     description='CLI for using the PolySwarm Customer APIs',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='PolySwarm Developers',
     author_email='info@polyswarm.io',
     url='https://github.com/polyswarm/polyswarm-cli',
     license='MIT',
-    python_requires='>=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,<4',
+    python_requires='>=3.5,<4',
     install_requires=[
-        'polyswarm-api~=3.1',
+        'polyswarm-api~=3.3.2',
         'click~=7.0',
         'colorama~=0.4.3',
         'future~=0.18.2',
         'click-log~=0.3.2',
         'pygments~=2.5.2',
     ],
     extras_require={
-        ':python_version < "3.0"': ['futures~=3.3.0'],
         'yara': ['yara-python==3.11.0'],
     },
     include_package_data=True,
     packages=find_packages('src'),
     package_dir={'': 'src'},
     entry_points={
         'console_scripts': [
             'polyswarm=polyswarm.__main__:polyswarm_cli',
         ],
     },
     classifiers=[
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: Implementation :: PyPy',
     ],
 )
```

### Comparing `polyswarm-3.2.1/src/polyswarm/__main__.py` & `polyswarm-3.3.0/src/polyswarm/__main__.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.1/src/polyswarm/client/download.py` & `polyswarm-3.3.0/src/polyswarm/client/download.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,14 +29,29 @@
     api = ctx.obj['api']
     out = ctx.obj['output']
     hashes = utils.parse_hashes(hash_value, hash_file=hash_file)
     for result in api.download_multiple(hashes, destination, hash_type):
         out.local_artifact(result)
 
 
+@click.command('download-id', short_help='Download file(s).')
+@click.option('-d', '--destination', type=click.Path(file_okay=False),
+              help='Path where to store the downloaded files.', default=os.getcwd())
+@click.argument('instance_id', nargs=-1, type=click.INT)
+@click.pass_context
+def download_id(ctx, destination, instance_id):
+    """
+    Download files from instance ids
+    """
+    api = ctx.obj['api']
+    out = ctx.obj['output']
+    for result in api.download_id_multiple(instance_id, destination):
+        out.local_artifact(result)
+
+
 @click.command('stream', short_help='Access the polyswarm file stream.')
 @click.option('-s', '--since', type=click.IntRange(1, 2880), default=1440,
               help='Request archives X minutes into the past. Default: 1440, Max: 2880.')
 @click.argument('destination', nargs=1, type=click.Path(file_okay=False))
 @click.pass_context
 def stream(ctx, since, destination):
     api = ctx.obj['api']
```

### Comparing `polyswarm-3.2.1/src/polyswarm/client/engine.py` & `polyswarm-3.3.0/src/polyswarm/client/engine.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.1/src/polyswarm/client/families.py` & `polyswarm-3.3.0/src/polyswarm/client/families.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.1/src/polyswarm/client/historical.py` & `polyswarm-3.3.0/src/polyswarm/client/historical.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.1/src/polyswarm/client/links.py` & `polyswarm-3.3.0/src/polyswarm/client/links.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.1/src/polyswarm/client/live.py` & `polyswarm-3.3.0/src/polyswarm/client/live.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.1/src/polyswarm/client/metadata.py` & `polyswarm-3.3.0/src/polyswarm/client/metadata.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.1/src/polyswarm/client/polyswarm.py` & `polyswarm-3.3.0/src/polyswarm/client/polyswarm.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from polyswarm.polyswarm import Polyswarm
 from polyswarm.formatters import formatters
 from polyswarm.client.utils import validate_key
 from polyswarm.client.live import live
 from polyswarm.client.historical import historical
 from polyswarm.client.scan import scan, lookup, wait, rescan, rescan_id
 from polyswarm.client.sandbox import sandbox, sandbox_list
-from polyswarm.client.download import download, cat, stream
+from polyswarm.client.download import download, cat, stream, download_id
 from polyswarm.client.search import known, search
 from polyswarm.client.rules import rules
 from polyswarm.client.links import link
 from polyswarm.client.tags import tag
 from polyswarm.client.families import family
 from polyswarm.client.metadata import metadata
 from polyswarm.client.engine import engine
@@ -139,14 +139,14 @@
 
     ctx.obj['api'] = Polyswarm(api_key, uri=api_uri, community=community, parallel=parallel, verify=verify)
     ctx.obj['output'] = formatters[output_format](color=color, output=output_file)
 
 
 commands = [
     scan, wait, lookup, search, live, historical,
-    download, cat, stream, rescan, rescan_id,
+    download, download_id, cat, stream, rescan, rescan_id,
     rules, link, tag, family, metadata,
     engine, known, sandbox, sandbox_list
 ]
 
 for command in commands:
     polyswarm_cli.add_command(command)
```

### Comparing `polyswarm-3.2.1/src/polyswarm/client/rules.py` & `polyswarm-3.3.0/src/polyswarm/client/rules.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.1/src/polyswarm/client/scan.py` & `polyswarm-3.3.0/src/polyswarm/client/scan.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.1/src/polyswarm/client/search.py` & `polyswarm-3.3.0/src/polyswarm/client/search.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.1/src/polyswarm/client/tags.py` & `polyswarm-3.3.0/src/polyswarm/client/tags.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.1/src/polyswarm/client/utils.py` & `polyswarm-3.3.0/src/polyswarm/client/utils.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.1/src/polyswarm/formatters/base.py` & `polyswarm-3.3.0/src/polyswarm/formatters/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -47,7 +47,13 @@
         raise NotImplementedError
 
     def artifact_metadata(self, result, only=None):
         raise NotImplementedError
 
     def sandbox_list(self, result):
         raise NotImplementedError
+
+    def sandbox_task(self, result):
+        raise NotImplementedError
+
+    def sandbox_tasks(self, results):
+        raise NotImplementedError
```

### Comparing `polyswarm-3.2.1/src/polyswarm/formatters/hashes.py` & `polyswarm-3.3.0/src/polyswarm/formatters/hashes.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.1/src/polyswarm/formatters/json.py` & `polyswarm-3.3.0/src/polyswarm/formatters/json.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,18 @@
 
     def known_host(self, result):
         click.echo(self._to_json(result.json), file=self.out)
 
     def artifact_metadata(self, result, only=None):
         click.echo(self._to_json(result.json), file=self.out)
 
-    def sandbox_list(self, result):
+    def sandbox_providers(self, result):
+        click.echo(self._to_json(result.json), file=self.out)
+
+    def sandbox_task(self, result):
         click.echo(self._to_json(result.json), file=self.out)
 
 
 class PrettyJSONOutput(JSONOutput):
     name = 'pretty-json'
 
     def __init__(self, output, color, **kwargs):
```

### Comparing `polyswarm-3.2.1/src/polyswarm/formatters/text.py` & `polyswarm-3.3.0/src/polyswarm/formatters/text.py`

 * *Files 4% similar despite different names*

```diff
@@ -333,18 +333,53 @@
             if only is None or metadata['tool'] in only:
                 tool = self._white(metadata['tool'].rjust(max_len))
                 output.append('%s: Updated at %s' % (tool, pretty_print_datetime(metadata['updated'])))
         self._close_group()
 
         return self._output(output, write)
 
-    def sandbox_list(self, result, write=True):
+    def sandbox_providers(self, result, write=True):
         output = []
-        output.append(self._white('============================= Sandboxes ============================='))
-        output.append(self._white('result: {}'.format(result.json['result'])))
+        output.append(self._white('============================= Providers ============================='))
+        for provider in result.json['result']:
+            output.append(self._white('name: {}'.format(provider['name'])))
+        return self._output(output, write)
+    
+    def sandbox_task(self, task, write=True):
+        output = []
+        output.append(self._white('============================= Sandbox Task ============================='))
+        output.append(self._blue('id: {}'.format(task.id)))
+        output.append(self._blue('sha256: {}'.format(task.sha256)))
+        output.append(self._blue('sandbox: {}'.format(task.sandbox)))
+        output.append(self._white('created: {}'.format(task.created)))
+        output.append(self._white('community: {}'.format(task.community)))
+        output.append(self._white('instance id: {}'.format(task.instance_id)))
+        output.append(self._white('status: {}'.format(task.status)))
+
+        if task.account_number:
+            output.append(self._white('account number: {}'.format(task.account_number)))
+        if task.team_account_number:
+            output.append(self._white('team account number: {}'.format(task.team_account_number)))
+
+        if task.sandbox_artifacts:
+            output.append(self._white('sandbox artifacts:'))
+        self._open_group()
+        for artifact in task.sandbox_artifacts:
+            output_string = '{}: '.format(artifact.type)
+            if artifact.name:
+                output_string += '{}, '.format(artifact.name)
+            if artifact.mimetype:
+                output_string += '{}, '.format(artifact.mimetype)
+            output_string += 'instance id: {}'.format(artifact.instance_id)
+            output.append(self._white(output_string))
+        self._close_group()
+
+        if task.report:
+            output.append(self._white('report: use `--fmt pretty-json` to see report content'))
+
         return self._output(output, write)
 
     def metadata(self, instance, write=True):
         output = []
         output.append(self._white('============================= Metadata ============================='))
         output.append(self._blue('Artifact id: {}'.format(instance.id)))
         output.append(self._white('Created: {}'.format(instance.created)))
```

### Comparing `polyswarm-3.2.1/src/polyswarm/polyswarm.py` & `polyswarm-3.3.0/src/polyswarm/polyswarm.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,14 +165,27 @@
         """
         args = [(destination, h) for h in hashes]
 
         for result in utils.parallel_executor(self.download, args_list=args,
                                               kwargs_list=[{'hash_type': hash_type}]*len(args)):
             yield result
 
+    def download_id_multiple(self, instance_id, destination):
+        """
+        Download files from matching instance ids.
+
+        :param instance_id: A list of instance ids to download.
+        :param destination: Folder where to download the files to.
+        :return: An iterator of local artifacts.
+        """
+        args = [(destination, h) for h in instance_id]
+
+        for result in utils.parallel_executor(self.download_id, args_list=args):
+            yield result
+
     def download_stream(self, destination, since=1440):
         """
         Access the polyswarm file stream.
 
         :param destination: Folder where to download the files to.
         :param since: Request archives X minutes into the past. Default: 1440, Max: 2880.
         :return: An iterator of local artifacts.
@@ -222,13 +235,13 @@
                 args_list=args,
                 kwargs_list=kwargs,
         ):
             yield tag_link
 
     def sandbox_instances(self, instance_ids, **kwargs):
         """
-        Send a file to be sandboxed by sha256 hash.
+        Send a file to be sandboxed by instance id.
         """
         args = [(u,) for u in instance_ids]
         kwargs = [kwargs] * len(args)
         for result in utils.parallel_executor(self.sandbox, args_list=args, kwargs_list=kwargs):
             yield result
```

### Comparing `polyswarm-3.2.1/src/polyswarm/utils.py` & `polyswarm-3.3.0/src/polyswarm/utils.py`

 * *Files identical despite different names*

### Comparing `polyswarm-3.2.1/src/polyswarm.egg-info/PKG-INFO` & `polyswarm-3.3.0/src/polyswarm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: polyswarm
-Version: 3.2.1
+Version: 3.3.0
 Summary: CLI for using the PolySwarm Customer APIs
 Home-page: https://github.com/polyswarm/polyswarm-cli
 Author: PolySwarm Developers
 Author-email: info@polyswarm.io
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,<4
+Requires-Python: >=3.5,<4
 Description-Content-Type: text/markdown
 Provides-Extra: yara
 License-File: LICENSE
 
 
 # Polyswarm Customer CLI
```

### Comparing `polyswarm-3.2.1/src/polyswarm.egg-info/SOURCES.txt` & `polyswarm-3.3.0/src/polyswarm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

