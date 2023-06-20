# Comparing `tmp/flake8-noqa-1.3.1.tar.gz` & `tmp/flake8-noqa-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-noqa-1.3.1.tar", last modified: Tue Mar 14 03:56:31 2023, max compression
+gzip compressed data, was "flake8-noqa-1.3.2.tar", last modified: Tue Jun 20 21:35:02 2023, max compression
```

## Comparing `flake8-noqa-1.3.1.tar` & `flake8-noqa-1.3.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 03:56:31.189546 flake8-noqa-1.3.1/
--rw-rw-rw-   0 root         (0) root         (0)      326 2022-11-24 19:30:44.000000 flake8-noqa-1.3.1/.editorconfig
--rw-rw-rw-   0 root         (0) root         (0)      258 2022-11-24 19:30:44.000000 flake8-noqa-1.3.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)       88 2022-11-24 19:30:44.000000 flake8-noqa-1.3.1/.gitlab-ci.env
--rw-rw-rw-   0 root         (0) root         (0)     2058 2022-11-24 19:49:28.000000 flake8-noqa-1.3.1/.gitlab-ci.yaml
--rw-rw-rw-   0 root         (0) root         (0)      260 2022-11-24 19:30:44.000000 flake8-noqa-1.3.1/.yamllint.yaml
--rw-rw-rw-   0 root         (0) root         (0)     7652 2022-11-24 19:30:44.000000 flake8-noqa-1.3.1/COPYING.LESSER
--rw-rw-rw-   0 root         (0) root         (0)    35149 2022-11-24 19:30:44.000000 flake8-noqa-1.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5970 2023-03-14 03:56:31.189546 flake8-noqa-1.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4891 2022-11-24 19:30:44.000000 flake8-noqa-1.3.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      169 2022-11-24 19:30:44.000000 flake8-noqa-1.3.1/flake8-noqa.sublime-project
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 03:56:31.185546 flake8-noqa-1.3.1/flake8_noqa/
--rw-rw-rw-   0 root         (0) root         (0)      173 2022-11-24 19:30:44.000000 flake8-noqa-1.3.1/flake8_noqa/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6364 2022-11-24 19:30:44.000000 flake8-noqa-1.3.1/flake8_noqa/noqa_checker.py
--rw-rw-rw-   0 root         (0) root         (0)     3477 2022-11-24 19:30:44.000000 flake8-noqa-1.3.1/flake8_noqa/noqa_comment.py
--rw-rw-rw-   0 root         (0) root         (0)     7375 2023-03-14 03:55:00.000000 flake8-noqa-1.3.1/flake8_noqa/noqa_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 03:56:31.189546 flake8-noqa-1.3.1/flake8_noqa.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5970 2023-03-14 03:56:31.000000 flake8-noqa-1.3.1/flake8_noqa.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      473 2023-03-14 03:56:31.000000 flake8-noqa-1.3.1/flake8_noqa.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-14 03:56:31.000000 flake8-noqa-1.3.1/flake8_noqa.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-03-14 03:56:31.000000 flake8-noqa-1.3.1/flake8_noqa.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      490 2023-03-14 03:56:31.000000 flake8-noqa-1.3.1/flake8_noqa.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-03-14 03:56:31.000000 flake8-noqa-1.3.1/flake8_noqa.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     2278 2022-11-24 19:30:44.000000 flake8-noqa-1.3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-14 03:56:31.189546 flake8-noqa-1.3.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     6238 2023-03-14 03:56:29.000000 flake8-noqa-1.3.1/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 21:35:02.380688 flake8-noqa-1.3.2/
+-rw-rw-rw-   0 root         (0) root         (0)      326 2022-11-24 19:30:44.000000 flake8-noqa-1.3.2/.editorconfig
+-rw-rw-rw-   0 root         (0) root         (0)      258 2022-11-24 19:30:44.000000 flake8-noqa-1.3.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)       88 2022-11-24 19:30:44.000000 flake8-noqa-1.3.2/.gitlab-ci.env
+-rw-rw-rw-   0 root         (0) root         (0)     2058 2022-11-24 19:49:28.000000 flake8-noqa-1.3.2/.gitlab-ci.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      260 2022-11-24 19:30:44.000000 flake8-noqa-1.3.2/.yamllint.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2022-11-24 19:30:44.000000 flake8-noqa-1.3.2/COPYING.LESSER
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2022-11-24 19:30:44.000000 flake8-noqa-1.3.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5999 2023-06-20 21:35:02.380688 flake8-noqa-1.3.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4891 2022-11-24 19:30:44.000000 flake8-noqa-1.3.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      169 2022-11-24 19:30:44.000000 flake8-noqa-1.3.2/flake8-noqa.sublime-project
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 21:35:02.376688 flake8-noqa-1.3.2/flake8_noqa/
+-rw-rw-rw-   0 root         (0) root         (0)      173 2022-11-24 19:30:44.000000 flake8-noqa-1.3.2/flake8_noqa/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6364 2022-11-24 19:30:44.000000 flake8-noqa-1.3.2/flake8_noqa/noqa_checker.py
+-rw-rw-rw-   0 root         (0) root         (0)     3477 2022-11-24 19:30:44.000000 flake8-noqa-1.3.2/flake8_noqa/noqa_comment.py
+-rw-rw-rw-   0 root         (0) root         (0)     7380 2023-06-20 21:30:54.000000 flake8-noqa-1.3.2/flake8_noqa/noqa_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 21:35:02.380688 flake8-noqa-1.3.2/flake8_noqa.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5999 2023-06-20 21:35:02.000000 flake8-noqa-1.3.2/flake8_noqa.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      473 2023-06-20 21:35:02.000000 flake8-noqa-1.3.2/flake8_noqa.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 21:35:02.000000 flake8-noqa-1.3.2/flake8_noqa.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-20 21:35:02.000000 flake8-noqa-1.3.2/flake8_noqa.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      490 2023-06-20 21:35:02.000000 flake8-noqa-1.3.2/flake8_noqa.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-20 21:35:02.000000 flake8-noqa-1.3.2/flake8_noqa.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2278 2022-11-24 19:30:44.000000 flake8-noqa-1.3.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 21:35:02.380688 flake8-noqa-1.3.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     6238 2023-06-20 21:35:00.000000 flake8-noqa-1.3.2/test.py
```

### Comparing `flake8-noqa-1.3.1/.gitlab-ci.yaml` & `flake8-noqa-1.3.2/.gitlab-ci.yaml`

 * *Files identical despite different names*

### Comparing `flake8-noqa-1.3.1/COPYING.LESSER` & `flake8-noqa-1.3.2/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `flake8-noqa-1.3.1/LICENSE` & `flake8-noqa-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-noqa-1.3.1/PKG-INFO` & `flake8-noqa-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-noqa
-Version: 1.3.1
+Version: 1.3.2
 Summary: Flake8 noqa comment validation
 Author-email: Peter Linss <pypi@linss.com>
 License: GNU Lesser General Public License v3
 Project-URL: homepage, https://github.com/plinss/flake8-noqa
 Keywords: flake8,noqa
 Classifier: Framework :: Flake8
 Classifier: Environment :: Console
@@ -20,14 +20,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
+License-File: COPYING.LESSER
 
 [flake8-noqa](https://github.com/plinss/flake8-noqa)
 ==========
 
 flake8 plugin to validate `# noqa` comments.
 
 flake8 is very particular about formatting of `# noqa` comments.
```

### Comparing `flake8-noqa-1.3.1/README.md` & `flake8-noqa-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `flake8-noqa-1.3.1/flake8_noqa/noqa_checker.py` & `flake8-noqa-1.3.2/flake8_noqa/noqa_checker.py`

 * *Files identical despite different names*

### Comparing `flake8-noqa-1.3.1/flake8_noqa/noqa_comment.py` & `flake8-noqa-1.3.2/flake8_noqa/noqa_comment.py`

 * *Files identical despite different names*

### Comparing `flake8-noqa-1.3.1/flake8_noqa/noqa_filter.py` & `flake8-noqa-1.3.2/flake8_noqa/noqa_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
 
 				pass
 			else:  # blanket noqa
 				if (reports):
 					if (self.require_code):
 						yield self._message(comment.token, Message.NOQA_REQUIRE_CODE,
 						                    comment=comment.text, noqa_strip=comment.noqa.strip(),
-						                    codes=', '.join(sorted(reports)))
+						                    codes=', '.join(sorted(set(reports))))
 
 				else:
 					yield self._message(comment.token, Message.NOQA_NO_VIOLATIONS, comment=comment.text)
 
 
 class Violation(flake8.style_guide.Violation):
 	"""Replacement for flake8's Violation class."""
```

### Comparing `flake8-noqa-1.3.1/flake8_noqa.egg-info/PKG-INFO` & `flake8-noqa-1.3.2/flake8_noqa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-noqa
-Version: 1.3.1
+Version: 1.3.2
 Summary: Flake8 noqa comment validation
 Author-email: Peter Linss <pypi@linss.com>
 License: GNU Lesser General Public License v3
 Project-URL: homepage, https://github.com/plinss/flake8-noqa
 Keywords: flake8,noqa
 Classifier: Framework :: Flake8
 Classifier: Environment :: Console
@@ -20,14 +20,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
+License-File: COPYING.LESSER
 
 [flake8-noqa](https://github.com/plinss/flake8-noqa)
 ==========
 
 flake8 plugin to validate `# noqa` comments.
 
 flake8 is very particular about formatting of `# noqa` comments.
```

### Comparing `flake8-noqa-1.3.1/pyproject.toml` & `flake8-noqa-1.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flake8-noqa-1.3.1/test.py` & `flake8-noqa-1.3.2/test.py`

 * *Files identical despite different names*

