# Comparing `tmp/nbtopy-1.0.tar.gz` & `tmp/nbtopy-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbtopy-1.0.tar", last modified: Tue Oct 25 04:54:45 2022, max compression
+gzip compressed data, was "nbtopy-1.1.tar", last modified: Mon Jun 19 22:32:30 2023, max compression
```

## Comparing `nbtopy-1.0.tar` & `nbtopy-1.1.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-10-25 04:54:45.512643 nbtopy-1.0/
--rw-r--r--   0 mark      (1000) mark      (1000)     6256 2022-10-25 04:54:45.512643 nbtopy-1.0/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)     5844 2022-10-19 23:19:32.000000 nbtopy-1.0/README.md
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-10-25 04:54:45.512643 nbtopy-1.0/nbtopy.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     6256 2022-10-25 04:54:45.000000 nbtopy-1.0/nbtopy.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      181 2022-10-25 04:54:45.000000 nbtopy-1.0/nbtopy.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2022-10-25 04:54:45.000000 nbtopy-1.0/nbtopy.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       39 2022-10-25 04:54:45.000000 nbtopy-1.0/nbtopy.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        7 2022-10-25 04:54:45.000000 nbtopy-1.0/nbtopy.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)     8335 2022-10-25 04:43:35.000000 nbtopy-1.0/nbtopy.py
--rw-r--r--   0 mark      (1000) mark      (1000)       38 2022-10-25 04:54:45.512643 nbtopy-1.0/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)      948 2022-07-13 23:41:24.000000 nbtopy-1.0/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-06-19 22:32:30.088621 nbtopy-1.1/
+-rw-r--r--   0 mark      (1000) mark      (1000)       74 2023-06-13 08:11:33.000000 nbtopy-1.1/.flake8
+-rw-r--r--   0 mark      (1000) mark      (1000)       54 2022-09-02 08:06:01.000000 nbtopy-1.1/.gitignore
+-rw-r--r--   0 mark      (1000) mark      (1000)      386 2023-06-19 22:19:15.000000 nbtopy-1.1/Makefile
+-rw-r--r--   0 mark      (1000) mark      (1000)     6054 2023-06-19 22:32:30.088621 nbtopy-1.1/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)     5641 2023-06-19 22:29:25.000000 nbtopy-1.1/README.md
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-06-19 22:32:30.088621 nbtopy-1.1/nbtopy.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     6054 2023-06-19 22:32:30.000000 nbtopy-1.1/nbtopy.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      244 2023-06-19 22:32:30.000000 nbtopy-1.1/nbtopy.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-06-19 22:32:30.000000 nbtopy-1.1/nbtopy.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       39 2023-06-19 22:32:30.000000 nbtopy-1.1/nbtopy.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       46 2023-06-19 22:32:30.000000 nbtopy-1.1/nbtopy.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        7 2023-06-19 22:32:30.000000 nbtopy-1.1/nbtopy.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)     8855 2023-06-19 22:28:18.000000 nbtopy-1.1/nbtopy.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      993 2023-06-19 22:31:06.000000 nbtopy-1.1/pyproject.toml
+-rw-r--r--   0 mark      (1000) mark      (1000)       38 2023-06-19 22:32:30.088621 nbtopy-1.1/setup.cfg
```

### Comparing `nbtopy-1.0/PKG-INFO` & `nbtopy-1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: nbtopy
-Version: 1.0
-Summary: Converts Jupyter notebook file[s] to Python (interactive) file[s].
-Home-page: https://github.com/bulletmark/nbtopy
-Author: Mark Blakeney
-Author-email: mark.blakeney@bullet-systems.net
-License: GPLv3
-Keywords: jupyter notebook nbconvert vscode
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 ## NBTOPY - Converts Jupyter notebook files to Python files
 [![PyPi](https://img.shields.io/pypi/v/nbtopy)](https://pypi.org/project/nbtopy/)
 [![AUR](https://img.shields.io/aur/version/nbtopy)](https://aur.archlinux.org/packages/nbtopy/)
 
 [nbtopy](http://github.com/bulletmark/nbtopy) is a Linux command line
 utility to convert one or more [Jupyter](https://jupyter.org/) notebook
 files (`.ipynb`) to Python files (`.py`). My primary purpose for
@@ -75,58 +62,49 @@
 
     ```
     $ nbtopy -r -d $PWD/pyfiles .
     ```
 
 ## Installation or Upgrade
 
-Arch users can install [nbtopy from the AUR](https://aur.archlinux.org/packages/nbtopy/).
+Arch users can install [nbtopy from the
+AUR](https://aur.archlinux.org/packages/nbtopy/).
 
 Python 3.6 or later is required. Note [nbtopy is on
 PyPI](https://pypi.org/project/nbtopy/) so just ensure that
-`python3-pip` and `python3-wheel` are installed then type the following
-to install (or upgrade):
-
-```
-$ sudo pip3 install -U nbtopy
-```
-
-Or, to install from this source repository:
+[`pipx`](https://pypa.github.io/pipx/) is installed then type the
+following:
 
 ```
-$ git clone http://github.com/bulletmark/nbtopy
-$ cd nbtopy
-$ sudo pip3 install -U .
+$ pipx install nbtopy
 ```
 
-To upgrade from the source repository:
+To upgrade:
 
 ```
-$ cd nbtopy # i.e. to git source dir above
-$ git pull
-$ sudo pip3 install -U .
+$ pipx upgrade nbtopy
 ```
 
 This program runs on pure Python. No 3rd party packages are required.
 Note that this program does not require Jupyter's
 [nbconvert](https://nbconvert.readthedocs.io/) tool.
 
 ## Command Line Options
 
 Type `nbtopy -h` to view the usage summary:
 
 ```
 usage: nbtopy [-h] [-m] [-M] [-c] [-e] [-x] [-f] [-r] [-p] [-q] [-w]
-                 [-o OUT] [-d DIR]
-                 ipynb_path [ipynb_path ...]
+                 [-o OUT] [-d DIR] [-V]
+                 [ipynb_path ...]
 
 Converts Jupyter notebook file[s] to Python (interactive) file[s].
 
 positional arguments:
-  ipynb_path            input ipynb file (dir for *.ipynb files)
+  ipynb_path            input ipynb file[s] (or dir for all *.ipynb files)
 
 options:
   -h, --help            show this help message and exit
   -m, --no-markdown-tag
                         do not add markdown tag on markdown cells
   -M, --no-markdown     do not output markdown cells at all
   -c, --no-code-tag     do not add code tag on code cells
@@ -137,14 +115,15 @@
   -r, --recurse         recursively process files in all sub-directories
   -p, --purge           just purge associated output file[s]
   -q, --quiet           suppress messages about processed file[s]
   -w, --no-warnings     suppress warning messages about processed file[s]
   -o OUT, --out OUT     alternative output file name, or '-' for stdout
   -d DIR, --dir DIR     output directory, default = ".". Specify absolute path
                         to create separate tree of output files
+  -V, --version         show nbtopy version
 
 Note you can set default options in ~/.config/nbtopy-flags.conf.
 ```
 
 ## Default Options
 
 You can add default options to a personal configuration file
```

### Comparing `nbtopy-1.0/README.md` & `nbtopy-1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: nbtopy
+Version: 1.1
+Summary: Converts Jupyter notebook files to Python (interactive) files
+Author-email: Mark Blakeney <mark.blakeney@bullet-systems.net>
+License: GPLv3
+Project-URL: Homepage, https://github.com/bulletmark/nbtopy
+Keywords: jupyter,notebook,nbconvert,vscode
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 ## NBTOPY - Converts Jupyter notebook files to Python files
 [![PyPi](https://img.shields.io/pypi/v/nbtopy)](https://pypi.org/project/nbtopy/)
 [![AUR](https://img.shields.io/aur/version/nbtopy)](https://aur.archlinux.org/packages/nbtopy/)
 
 [nbtopy](http://github.com/bulletmark/nbtopy) is a Linux command line
 utility to convert one or more [Jupyter](https://jupyter.org/) notebook
 files (`.ipynb`) to Python files (`.py`). My primary purpose for
@@ -62,58 +74,49 @@
 
     ```
     $ nbtopy -r -d $PWD/pyfiles .
     ```
 
 ## Installation or Upgrade
 
-Arch users can install [nbtopy from the AUR](https://aur.archlinux.org/packages/nbtopy/).
+Arch users can install [nbtopy from the
+AUR](https://aur.archlinux.org/packages/nbtopy/).
 
 Python 3.6 or later is required. Note [nbtopy is on
 PyPI](https://pypi.org/project/nbtopy/) so just ensure that
-`python3-pip` and `python3-wheel` are installed then type the following
-to install (or upgrade):
-
-```
-$ sudo pip3 install -U nbtopy
-```
-
-Or, to install from this source repository:
+[`pipx`](https://pypa.github.io/pipx/) is installed then type the
+following:
 
 ```
-$ git clone http://github.com/bulletmark/nbtopy
-$ cd nbtopy
-$ sudo pip3 install -U .
+$ pipx install nbtopy
 ```
 
-To upgrade from the source repository:
+To upgrade:
 
 ```
-$ cd nbtopy # i.e. to git source dir above
-$ git pull
-$ sudo pip3 install -U .
+$ pipx upgrade nbtopy
 ```
 
 This program runs on pure Python. No 3rd party packages are required.
 Note that this program does not require Jupyter's
 [nbconvert](https://nbconvert.readthedocs.io/) tool.
 
 ## Command Line Options
 
 Type `nbtopy -h` to view the usage summary:
 
 ```
 usage: nbtopy [-h] [-m] [-M] [-c] [-e] [-x] [-f] [-r] [-p] [-q] [-w]
-                 [-o OUT] [-d DIR]
-                 ipynb_path [ipynb_path ...]
+                 [-o OUT] [-d DIR] [-V]
+                 [ipynb_path ...]
 
 Converts Jupyter notebook file[s] to Python (interactive) file[s].
 
 positional arguments:
-  ipynb_path            input ipynb file (dir for *.ipynb files)
+  ipynb_path            input ipynb file[s] (or dir for all *.ipynb files)
 
 options:
   -h, --help            show this help message and exit
   -m, --no-markdown-tag
                         do not add markdown tag on markdown cells
   -M, --no-markdown     do not output markdown cells at all
   -c, --no-code-tag     do not add code tag on code cells
@@ -124,14 +127,15 @@
   -r, --recurse         recursively process files in all sub-directories
   -p, --purge           just purge associated output file[s]
   -q, --quiet           suppress messages about processed file[s]
   -w, --no-warnings     suppress warning messages about processed file[s]
   -o OUT, --out OUT     alternative output file name, or '-' for stdout
   -d DIR, --dir DIR     output directory, default = ".". Specify absolute path
                         to create separate tree of output files
+  -V, --version         show nbtopy version
 
 Note you can set default options in ~/.config/nbtopy-flags.conf.
 ```
 
 ## Default Options
 
 You can add default options to a personal configuration file
```

### Comparing `nbtopy-1.0/nbtopy.egg-info/PKG-INFO` & `nbtopy-1.1/nbtopy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: nbtopy
-Version: 1.0
-Summary: Converts Jupyter notebook file[s] to Python (interactive) file[s].
-Home-page: https://github.com/bulletmark/nbtopy
-Author: Mark Blakeney
-Author-email: mark.blakeney@bullet-systems.net
+Version: 1.1
+Summary: Converts Jupyter notebook files to Python (interactive) files
+Author-email: Mark Blakeney <mark.blakeney@bullet-systems.net>
 License: GPLv3
-Keywords: jupyter notebook nbconvert vscode
+Project-URL: Homepage, https://github.com/bulletmark/nbtopy
+Keywords: jupyter,notebook,nbconvert,vscode
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 ## NBTOPY - Converts Jupyter notebook files to Python files
 [![PyPi](https://img.shields.io/pypi/v/nbtopy)](https://pypi.org/project/nbtopy/)
 [![AUR](https://img.shields.io/aur/version/nbtopy)](https://aur.archlinux.org/packages/nbtopy/)
@@ -75,58 +74,49 @@
 
     ```
     $ nbtopy -r -d $PWD/pyfiles .
     ```
 
 ## Installation or Upgrade
 
-Arch users can install [nbtopy from the AUR](https://aur.archlinux.org/packages/nbtopy/).
+Arch users can install [nbtopy from the
+AUR](https://aur.archlinux.org/packages/nbtopy/).
 
 Python 3.6 or later is required. Note [nbtopy is on
 PyPI](https://pypi.org/project/nbtopy/) so just ensure that
-`python3-pip` and `python3-wheel` are installed then type the following
-to install (or upgrade):
+[`pipx`](https://pypa.github.io/pipx/) is installed then type the
+following:
 
 ```
-$ sudo pip3 install -U nbtopy
+$ pipx install nbtopy
 ```
 
-Or, to install from this source repository:
+To upgrade:
 
 ```
-$ git clone http://github.com/bulletmark/nbtopy
-$ cd nbtopy
-$ sudo pip3 install -U .
-```
-
-To upgrade from the source repository:
-
-```
-$ cd nbtopy # i.e. to git source dir above
-$ git pull
-$ sudo pip3 install -U .
+$ pipx upgrade nbtopy
 ```
 
 This program runs on pure Python. No 3rd party packages are required.
 Note that this program does not require Jupyter's
 [nbconvert](https://nbconvert.readthedocs.io/) tool.
 
 ## Command Line Options
 
 Type `nbtopy -h` to view the usage summary:
 
 ```
 usage: nbtopy [-h] [-m] [-M] [-c] [-e] [-x] [-f] [-r] [-p] [-q] [-w]
-                 [-o OUT] [-d DIR]
-                 ipynb_path [ipynb_path ...]
+                 [-o OUT] [-d DIR] [-V]
+                 [ipynb_path ...]
 
 Converts Jupyter notebook file[s] to Python (interactive) file[s].
 
 positional arguments:
-  ipynb_path            input ipynb file (dir for *.ipynb files)
+  ipynb_path            input ipynb file[s] (or dir for all *.ipynb files)
 
 options:
   -h, --help            show this help message and exit
   -m, --no-markdown-tag
                         do not add markdown tag on markdown cells
   -M, --no-markdown     do not output markdown cells at all
   -c, --no-code-tag     do not add code tag on code cells
@@ -137,14 +127,15 @@
   -r, --recurse         recursively process files in all sub-directories
   -p, --purge           just purge associated output file[s]
   -q, --quiet           suppress messages about processed file[s]
   -w, --no-warnings     suppress warning messages about processed file[s]
   -o OUT, --out OUT     alternative output file name, or '-' for stdout
   -d DIR, --dir DIR     output directory, default = ".". Specify absolute path
                         to create separate tree of output files
+  -V, --version         show nbtopy version
 
 Note you can set default options in ~/.config/nbtopy-flags.conf.
 ```
 
 ## Default Options
 
 You can add default options to a personal configuration file
```

### Comparing `nbtopy-1.0/nbtopy.py` & `nbtopy-1.1/nbtopy.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,16 +25,20 @@
         return False
 
     with opath.open('w') as fp:
         fp.write(out)
 
     return True if exists else None
 
+convert_first = True
+
 def convert_file(ipath: Path, dirout: Path, args: Namespace) -> bool:
     'Convert given input file'
+    global convert_first
+
     if args.out:
         if args.out == '-':
             opath = None
         else:
             opath = dirout / args.out
     else:
         if not dirout.is_absolute():
@@ -70,17 +74,17 @@
             js = json.load(fp)
     except Exception:
         if not args.no_warnings:
             print(f'Skipping {ipath} : is malformed.', file=sys.stderr)
         return False
 
     out = []
-    if not args.out or convert_file.first:
+    if not args.out or convert_first:
         out.append('#!/usr/bin/env python3')
-        convert_file.first = False
+        convert_first = False
 
     out.append(f'\n## Built from {ipath} by {PROG} ##\n')
 
     cellist = js.get('cells')
 
     # Handle older format notebooks
     if cellist is None:
@@ -163,16 +167,14 @@
             print(msg)
 
     else:
         sys.stdout.write(outbuf)
 
     return True
 
-convert_file.first = True
-
 def convert_dir(ipath: Path, dirout: Path, args: Namespace) -> int:
     'Convert files in given input dir'
     count = 0
     for path in ipath.iterdir():
         if path.is_dir():
             if args.recurse:
                 count += convert_dir(path, dirout, args)
@@ -206,28 +208,48 @@
     opt.add_argument('-w', '--no-warnings', action='store_true',
             help='suppress warning messages about processed file[s]')
     opt.add_argument('-o', '--out',
             help='alternative output file name, or \'-\' for stdout')
     opt.add_argument('-d', '--dir', default='.',
             help='output directory, default = ".". Specify absolute path '
             'to create separate tree of output files')
-    opt.add_argument('ipynb_path', nargs='+',
+    opt.add_argument('-V', '--version', action='store_true',
+            help=f'show {PROG} version')
+    opt.add_argument('ipynb_path', nargs='*',
             help='input ipynb file[s] (or dir for all *.ipynb files)')
 
     # Merge in default args from user config file. Then parse the
     # command line.
-    cnflines = ''
     cnffile = CNFFILE.expanduser()
     if cnffile.exists():
         with cnffile.open() as fp:
-            cnflines = [re.sub(r'#.*$', '', line).strip() for line in fp]
-        cnflines = ' '.join(cnflines).strip()
+            lines = [re.sub(r'#.*$', '', line).strip() for line in fp]
+        cnflines = ' '.join(lines).strip()
+    else:
+        cnflines = ''
 
     args = opt.parse_args(shlex.split(cnflines) + sys.argv[1:])
 
+    if args.version:
+        if sys.version_info >= (3, 8):
+            from importlib.metadata import version
+        else:
+            from importlib_metadata import version
+
+        try:
+            ver = version(PROG)
+        except Exception:
+            ver = 'unknown'
+
+        print(ver)
+        return
+
+    if not args.ipynb_path:
+        opt.error('Must specify one or more ipynb files')
+
     dirout = Path(args.dir)
 
     if args.out:
         if args.out == '-':
             args.quiet = True
         else:
             path = dirout / args.out
```

