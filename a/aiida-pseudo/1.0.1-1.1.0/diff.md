# Comparing `tmp/aiida-pseudo-1.0.1.tar.gz` & `tmp/aiida_pseudo-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida-pseudo-1.0.1.tar", last modified: Mon May  8 09:08:03 2023, max compression
+gzip compressed data, was "aiida_pseudo-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiida-pseudo-1.0.1.tar` & `aiida_pseudo-1.1.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1188 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/.gitignore
--rw-r--r--   0        0        0     1078 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      230 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/.readthedocs.yml
--rw-r--r--   0        0        0    13321 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/CHANGELOG.md
--rw-r--r--   0        0        0     1073 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0     8871 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/README.md
--rw-r--r--   0        0        0     3245 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      113 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/src/aiida_pseudo/__init__.py
--rw-r--r--   0        0        0      250 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/src/aiida_pseudo/cli/__init__.py
--rw-r--r--   0        0        0     3848 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/src/aiida_pseudo/cli/family.py
--rw-r--r--   0        0        0    19578 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/src/aiida_pseudo/cli/install.py
--rw-r--r--   0        0        0     2226 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/src/aiida_pseudo/cli/list.py
--rw-r--r--   0        0        0      202 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/src/aiida_pseudo/cli/params/__init__.py
--rw-r--r--   0        0        0      370 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/src/aiida_pseudo/cli/params/arguments.py
--rw-r--r--   0        0        0     3635 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/src/aiida_pseudo/cli/params/options.py
--rw-r--r--   0        0        0     7303 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/src/aiida_pseudo/cli/params/types.py
--rw-r--r--   0        0        0     1031 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/src/aiida_pseudo/cli/root.py
--rw-r--r--   0        0        0     2663 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/src/aiida_pseudo/cli/utils.py
--rw-r--r--   0        0        0       60 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/src/aiida_pseudo/common/__init__.py
--rw-r--r--   0        0        0      245 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/src/aiida_pseudo/common/units.py
--rw-r--r--   0        0        0      105 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/src/aiida_pseudo/data/__init__.py
--rw-r--r--   0        0        0      382 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/src/aiida_pseudo/data/pseudo/__init__.py
--rw-r--r--   0        0        0     2886 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/src/aiida_pseudo/data/pseudo/jthxml.py
--rw-r--r--   0        0        0     7954 2023-05-08 09:07:56.713072 aiida-pseudo-1.0.1/src/aiida_pseudo/data/pseudo/pseudo.py
--rw-r--r--   0        0        0     2742 2023-05-08 09:07:56.717072 aiida-pseudo-1.0.1/src/aiida_pseudo/data/pseudo/psf.py
--rw-r--r--   0        0        0     4519 2023-05-08 09:07:56.717072 aiida-pseudo-1.0.1/src/aiida_pseudo/data/pseudo/psml.py
--rw-r--r--   0        0        0     3076 2023-05-08 09:07:56.717072 aiida-pseudo-1.0.1/src/aiida_pseudo/data/pseudo/psp8.py
--rw-r--r--   0        0        0     4707 2023-05-08 09:07:56.717072 aiida-pseudo-1.0.1/src/aiida_pseudo/data/pseudo/upf.py
--rw-r--r--   0        0        0     6686 2023-05-08 09:07:56.717072 aiida-pseudo-1.0.1/src/aiida_pseudo/data/pseudo/vps.py
--rw-r--r--   0        0        0      102 2023-05-08 09:07:56.717072 aiida-pseudo-1.0.1/src/aiida_pseudo/groups/__init__.py
--rw-r--r--   0        0        0      308 2023-05-08 09:07:56.717072 aiida-pseudo-1.0.1/src/aiida_pseudo/groups/family/__init__.py
--rw-r--r--   0        0        0      545 2023-05-08 09:07:56.717072 aiida-pseudo-1.0.1/src/aiida_pseudo/groups/family/cutoffs.py
--rw-r--r--   0        0        0    15544 2023-05-08 09:07:56.717072 aiida-pseudo-1.0.1/src/aiida_pseudo/groups/family/pseudo.py
--rw-r--r--   0        0        0    18127 2023-05-08 09:07:56.717072 aiida-pseudo-1.0.1/src/aiida_pseudo/groups/family/pseudo_dojo.py
--rw-r--r--   0        0        0     3973 2023-05-08 09:07:56.717072 aiida-pseudo-1.0.1/src/aiida_pseudo/groups/family/sssp.py
--rw-r--r--   0        0        0      178 2023-05-08 09:07:56.717072 aiida-pseudo-1.0.1/src/aiida_pseudo/groups/mixins/__init__.py
--rw-r--r--   0        0        0    14194 2023-05-08 09:07:56.717072 aiida-pseudo-1.0.1/src/aiida_pseudo/groups/mixins/cutoffs.py
--rw-r--r--   0        0        0    10527 1970-01-01 00:00:00.000000 aiida-pseudo-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1188 2023-06-20 12:04:54.486973 aiida_pseudo-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1078 2023-06-20 12:04:54.486973 aiida_pseudo-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      230 2023-06-20 12:04:54.486973 aiida_pseudo-1.1.0/.readthedocs.yml
+-rw-r--r--   0        0        0    13493 2023-06-20 12:04:54.486973 aiida_pseudo-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1073 2023-06-20 12:04:54.486973 aiida_pseudo-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     8871 2023-06-20 12:04:54.486973 aiida_pseudo-1.1.0/README.md
+-rw-r--r--   0        0        0     3245 2023-06-20 12:04:54.490973 aiida_pseudo-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      113 2023-06-20 12:04:54.490973 aiida_pseudo-1.1.0/src/aiida_pseudo/__init__.py
+-rw-r--r--   0        0        0      250 2023-06-20 12:04:54.490973 aiida_pseudo-1.1.0/src/aiida_pseudo/cli/__init__.py
+-rw-r--r--   0        0        0     3848 2023-06-20 12:04:54.490973 aiida_pseudo-1.1.0/src/aiida_pseudo/cli/family.py
+-rw-r--r--   0        0        0    19745 2023-06-20 12:04:54.490973 aiida_pseudo-1.1.0/src/aiida_pseudo/cli/install.py
+-rw-r--r--   0        0        0     2226 2023-06-20 12:04:54.490973 aiida_pseudo-1.1.0/src/aiida_pseudo/cli/list.py
+-rw-r--r--   0        0        0      202 2023-06-20 12:04:54.490973 aiida_pseudo-1.1.0/src/aiida_pseudo/cli/params/__init__.py
+-rw-r--r--   0        0        0      370 2023-06-20 12:04:54.490973 aiida_pseudo-1.1.0/src/aiida_pseudo/cli/params/arguments.py
+-rw-r--r--   0        0        0     3635 2023-06-20 12:04:54.490973 aiida_pseudo-1.1.0/src/aiida_pseudo/cli/params/options.py
+-rw-r--r--   0        0        0     7303 2023-06-20 12:04:54.490973 aiida_pseudo-1.1.0/src/aiida_pseudo/cli/params/types.py
+-rw-r--r--   0        0        0     1031 2023-06-20 12:04:54.490973 aiida_pseudo-1.1.0/src/aiida_pseudo/cli/root.py
+-rw-r--r--   0        0        0     2663 2023-06-20 12:04:54.490973 aiida_pseudo-1.1.0/src/aiida_pseudo/cli/utils.py
+-rw-r--r--   0        0        0       60 2023-06-20 12:04:54.490973 aiida_pseudo-1.1.0/src/aiida_pseudo/common/__init__.py
+-rw-r--r--   0        0        0      245 2023-06-20 12:04:54.490973 aiida_pseudo-1.1.0/src/aiida_pseudo/common/units.py
+-rw-r--r--   0        0        0      105 2023-06-20 12:04:54.490973 aiida_pseudo-1.1.0/src/aiida_pseudo/data/__init__.py
+-rw-r--r--   0        0        0      382 2023-06-20 12:04:54.490973 aiida_pseudo-1.1.0/src/aiida_pseudo/data/pseudo/__init__.py
+-rw-r--r--   0        0        0     2886 2023-06-20 12:04:54.490973 aiida_pseudo-1.1.0/src/aiida_pseudo/data/pseudo/jthxml.py
+-rw-r--r--   0        0        0     7954 2023-06-20 12:04:54.490973 aiida_pseudo-1.1.0/src/aiida_pseudo/data/pseudo/pseudo.py
+-rw-r--r--   0        0        0     2742 2023-06-20 12:04:54.490973 aiida_pseudo-1.1.0/src/aiida_pseudo/data/pseudo/psf.py
+-rw-r--r--   0        0        0     4519 2023-06-20 12:04:54.490973 aiida_pseudo-1.1.0/src/aiida_pseudo/data/pseudo/psml.py
+-rw-r--r--   0        0        0     3076 2023-06-20 12:04:54.490973 aiida_pseudo-1.1.0/src/aiida_pseudo/data/pseudo/psp8.py
+-rw-r--r--   0        0        0     4707 2023-06-20 12:04:54.490973 aiida_pseudo-1.1.0/src/aiida_pseudo/data/pseudo/upf.py
+-rw-r--r--   0        0        0     6686 2023-06-20 12:04:54.490973 aiida_pseudo-1.1.0/src/aiida_pseudo/data/pseudo/vps.py
+-rw-r--r--   0        0        0      102 2023-06-20 12:04:54.490973 aiida_pseudo-1.1.0/src/aiida_pseudo/groups/__init__.py
+-rw-r--r--   0        0        0      308 2023-06-20 12:04:54.490973 aiida_pseudo-1.1.0/src/aiida_pseudo/groups/family/__init__.py
+-rw-r--r--   0        0        0      545 2023-06-20 12:04:54.490973 aiida_pseudo-1.1.0/src/aiida_pseudo/groups/family/cutoffs.py
+-rw-r--r--   0        0        0    15544 2023-06-20 12:04:54.490973 aiida_pseudo-1.1.0/src/aiida_pseudo/groups/family/pseudo.py
+-rw-r--r--   0        0        0    18127 2023-06-20 12:04:54.490973 aiida_pseudo-1.1.0/src/aiida_pseudo/groups/family/pseudo_dojo.py
+-rw-r--r--   0        0        0     4197 2023-06-20 12:04:54.490973 aiida_pseudo-1.1.0/src/aiida_pseudo/groups/family/sssp.py
+-rw-r--r--   0        0        0      178 2023-06-20 12:04:54.490973 aiida_pseudo-1.1.0/src/aiida_pseudo/groups/mixins/__init__.py
+-rw-r--r--   0        0        0    14194 2023-06-20 12:04:54.490973 aiida_pseudo-1.1.0/src/aiida_pseudo/groups/mixins/cutoffs.py
+-rw-r--r--   0        0        0    10527 1970-01-01 00:00:00.000000 aiida_pseudo-1.1.0/PKG-INFO
```

### Comparing `aiida-pseudo-1.0.1/.gitignore` & `aiida_pseudo-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.1/.pre-commit-config.yaml` & `aiida_pseudo-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.1/CHANGELOG.md` & `aiida_pseudo-1.1.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Change log
 
+## `1.1.0` - 2023-06-20
+
+### Features
+
+- Add support for SSSP v1.3 [[5709f27]](https://github.com/aiidateam/aiida-pseudo/commit/5709f275d217d2f509dcac6fb24436bc29bcd53a)
+
+
 ## `1.0.1` - 2023-05-08
 
 ### Fixes
 - CLI: Change `Critical` to `Report` if family exists in `install` command [[3887762]](https://github.com/aiidateam/aiida-pseudo/commit/38877622cb658d7b37fd0f93fbdd649256146aa2)
 
 ### Dependencies
 - Update pre-commit requirement `isort==5.12.0` [[d3b494e]](https://github.com/aiidateam/aiida-pseudo/commit/d3b494e68444b68f200f8f01a3673b8d028ffa3e)
```

### Comparing `aiida-pseudo-1.0.1/LICENSE.txt` & `aiida_pseudo-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.1/README.md` & `aiida_pseudo-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.1/pyproject.toml` & `aiida_pseudo-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.1/src/aiida_pseudo/cli/family.py` & `aiida_pseudo-1.1.0/src/aiida_pseudo/cli/family.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.1/src/aiida_pseudo/cli/install.py` & `aiida_pseudo-1.1.0/src/aiida_pseudo/cli/install.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,14 +105,16 @@
     :param traceback: boolean, if true, print the traceback when an exception occurs.
     :return: Latest patch version of the requested minor version
     """
     from aiida_pseudo.groups.family import SsspFamily
 
     from .utils import attempt
 
+    # The ``parent_id=19`` points to the SSSP entry on the Materials Cloud. Using ``parent_id`` will fetch the latest
+    # version of the SSSP archive record.
     url_template = 'https://archive.materialscloud.org/record/file?filename={filename}&parent_id=19'
 
     # Download the dictionary mapping of the minor versions to the latest corresponding patch versions. Since patch
     # releases of the SSSP only contain bug fixes, there is no reason to have the user install an outdated patch
     # version. So, the latest patch version of the minor version that is specified by the user is always installed.
     with attempt('downloading patch versions information... ', include_traceback=traceback):
         response = requests.get(url_template.format(filename='versions.yaml'), timeout=30)
@@ -179,15 +181,15 @@
         response.raise_for_status()
         with open(filepath_metadata, 'wb') as handle:
             handle.write(response.content)
             handle.flush()
 
 
 @cmd_install.command('sssp')
-@options.VERSION(type=click.Choice(['1.0', '1.1', '1.2']), default='1.2', show_default=True)
+@options.VERSION(type=click.Choice(['1.0', '1.1', '1.2', '1.3']), default='1.3', show_default=True)
 @options.FUNCTIONAL(type=click.Choice(['PBE', 'PBEsol']), default='PBE', show_default=True)
 @options.PROTOCOL(type=click.Choice(['efficiency', 'precision']), default='efficiency', show_default=True)
 @options.DOWNLOAD_ONLY()
 @options.TRACEBACK()
 @decorators.with_dbenv()
 def cmd_install_sssp(version, functional, protocol, download_only, traceback):
     """Install an SSSP configuration.
```

### Comparing `aiida-pseudo-1.0.1/src/aiida_pseudo/cli/list.py` & `aiida_pseudo-1.1.0/src/aiida_pseudo/cli/list.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.1/src/aiida_pseudo/cli/params/options.py` & `aiida_pseudo-1.1.0/src/aiida_pseudo/cli/params/options.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.1/src/aiida_pseudo/cli/params/types.py` & `aiida_pseudo-1.1.0/src/aiida_pseudo/cli/params/types.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.1/src/aiida_pseudo/cli/root.py` & `aiida_pseudo-1.1.0/src/aiida_pseudo/cli/root.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.1/src/aiida_pseudo/cli/utils.py` & `aiida_pseudo-1.1.0/src/aiida_pseudo/cli/utils.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.1/src/aiida_pseudo/data/pseudo/jthxml.py` & `aiida_pseudo-1.1.0/src/aiida_pseudo/data/pseudo/jthxml.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.1/src/aiida_pseudo/data/pseudo/pseudo.py` & `aiida_pseudo-1.1.0/src/aiida_pseudo/data/pseudo/pseudo.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.1/src/aiida_pseudo/data/pseudo/psf.py` & `aiida_pseudo-1.1.0/src/aiida_pseudo/data/pseudo/psf.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.1/src/aiida_pseudo/data/pseudo/psml.py` & `aiida_pseudo-1.1.0/src/aiida_pseudo/data/pseudo/psml.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.1/src/aiida_pseudo/data/pseudo/psp8.py` & `aiida_pseudo-1.1.0/src/aiida_pseudo/data/pseudo/psp8.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.1/src/aiida_pseudo/data/pseudo/upf.py` & `aiida_pseudo-1.1.0/src/aiida_pseudo/data/pseudo/upf.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.1/src/aiida_pseudo/data/pseudo/vps.py` & `aiida_pseudo-1.1.0/src/aiida_pseudo/data/pseudo/vps.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.1/src/aiida_pseudo/groups/family/cutoffs.py` & `aiida_pseudo-1.1.0/src/aiida_pseudo/groups/family/cutoffs.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.1/src/aiida_pseudo/groups/family/pseudo.py` & `aiida_pseudo-1.1.0/src/aiida_pseudo/groups/family/pseudo.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.1/src/aiida_pseudo/groups/family/pseudo_dojo.py` & `aiida_pseudo-1.1.0/src/aiida_pseudo/groups/family/pseudo_dojo.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.1/src/aiida_pseudo/groups/family/sssp.py` & `aiida_pseudo-1.1.0/src/aiida_pseudo/groups/family/sssp.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,14 +41,18 @@
         SsspConfiguration('1.1', 'PBE', 'precision'),
         SsspConfiguration('1.1', 'PBEsol', 'efficiency'),
         SsspConfiguration('1.1', 'PBEsol', 'precision'),
         SsspConfiguration('1.2', 'PBE', 'efficiency'),
         SsspConfiguration('1.2', 'PBE', 'precision'),
         SsspConfiguration('1.2', 'PBEsol', 'efficiency'),
         SsspConfiguration('1.2', 'PBEsol', 'precision'),
+        SsspConfiguration('1.3', 'PBE', 'efficiency'),
+        SsspConfiguration('1.3', 'PBE', 'precision'),
+        SsspConfiguration('1.3', 'PBEsol', 'efficiency'),
+        SsspConfiguration('1.3', 'PBEsol', 'precision'),
     )
 
     @classmethod
     def get_valid_labels(cls) -> Sequence[str]:
         """Return the tuple of labels of all valid SSSP configurations."""
         return tuple(cls.format_configuration_label(configuration) for configuration in cls.valid_configurations)
```

### Comparing `aiida-pseudo-1.0.1/src/aiida_pseudo/groups/mixins/cutoffs.py` & `aiida_pseudo-1.1.0/src/aiida_pseudo/groups/mixins/cutoffs.py`

 * *Files identical despite different names*

### Comparing `aiida-pseudo-1.0.1/PKG-INFO` & `aiida_pseudo-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-pseudo
-Version: 1.0.1
+Version: 1.1.0
 Summary: AiiDA plugin that simplifies working with pseudo potentials.
 Keywords: aiida,pseudopotentials
 Author-email: "Sebastiaan P. Huber" <mail@sphuber.net>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AiiDA
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aiida-pseudo Version: 1.0.1 Summary: AiiDA plugin
+Metadata-Version: 2.1 Name: aiida-pseudo Version: 1.1.0 Summary: AiiDA plugin
 that simplifies working with pseudo potentials. Keywords:
 aiida,pseudopotentials Author-email: "Sebastiaan P. Huber"
 sphuber.net> Requires-Python: >=3.8 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable Classifier: Framework
 :: AiiDA Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: POSIX :: Linux Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Programming Language :: Python Classifier: Programming
```

