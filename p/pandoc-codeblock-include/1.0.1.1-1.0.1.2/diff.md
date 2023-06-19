# Comparing `tmp/pandoc_codeblock_include-1.0.1.1.tar.gz` & `tmp/pandoc_codeblock_include-1.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandoc_codeblock_include-1.0.1.1.tar", max compression
+gzip compressed data, was "pandoc_codeblock_include-1.0.1.2.tar", max compression
```

## Comparing `pandoc_codeblock_include-1.0.1.1.tar` & `pandoc_codeblock_include-1.0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1521 2023-06-18 12:42:26.913752 pandoc_codeblock_include-1.0.1.1/LICENSE
--rw-r--r--   0        0        0     9286 2023-06-18 12:42:26.913752 pandoc_codeblock_include-1.0.1.1/README.md
--rw-r--r--   0        0        0     4225 2023-06-18 12:42:26.917752 pandoc_codeblock_include-1.0.1.1/pandoc_codeblock_include.py
--rw-r--r--   0        0        0     2934 2023-06-18 12:42:26.917752 pandoc_codeblock_include-1.0.1.1/pyproject.toml
--rw-r--r--   0        0        0    10398 1970-01-01 00:00:00.000000 pandoc_codeblock_include-1.0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1521 2023-06-19 22:36:37.060857 pandoc_codeblock_include-1.0.1.2/LICENSE
+-rw-r--r--   0        0        0     9378 2023-06-19 22:36:37.060857 pandoc_codeblock_include-1.0.1.2/README.md
+-rw-r--r--   0        0        0     4225 2023-06-19 22:36:37.064857 pandoc_codeblock_include-1.0.1.2/pandoc_codeblock_include.py
+-rw-r--r--   0        0        0     2940 2023-06-19 22:36:37.064857 pandoc_codeblock_include-1.0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    10490 1970-01-01 00:00:00.000000 pandoc_codeblock_include-1.0.1.2/PKG-INFO
```

### Comparing `pandoc_codeblock_include-1.0.1.1/LICENSE` & `pandoc_codeblock_include-1.0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pandoc_codeblock_include-1.0.1.1/README.md` & `pandoc_codeblock_include-1.0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Installation
 ============
 
-![Python package](https://github.com/chdemko/pandoc-codeblock-include/workflows/Python%20package/badge.svg?branch=develop)
+[![Python package](https://github.com/chdemko/pandoc-codeblock-include/workflows/Python%20package/badge.svg?branch=develop)](https://github.com/chdemko/pandoc-codeblock-include/actions/workflows/python-package.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-codeblock-include/develop.svg?logo=Codecov&logoColor=white)](https://coveralls.io/github/chdemko/pandoc-codeblock-include?branch=develop)
 [![Code Climate](https://codeclimate.com/github/chdemko/pandoc-codeblock-include/badges/gpa.svg)](https://codeclimate.com/github/chdemko/pandoc-codeblock-include/)
 [![Code Beat](https://codebeat.co/badges/c0e680bd-9c47-4180-8d3f-b706905d0e73)](https://codebeat.co/projects/github-com-chdemko-pandoc-codeblock-include-develop/)
 [![Codacy](https://img.shields.io/codacy/grade/26716ef242ba4089aff55eff7ca592a9.svg?logo=codacy&logoColor=white)](https://app.codacy.com/gh/chdemko/pandoc-codeblock-include/)
 [![PyPI version](https://img.shields.io/pypi/v/pandoc-codeblock-include.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-codeblock-include/)
 [![PyPI format](https://img.shields.io/pypi/format/pandoc-codeblock-include.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiYw92eBNAAAAgJJREFUeNrt3T1WwkAUgNH31Br3ogWptdAlgyvQxYgHeh0LKKxI+PHAzNyvRo8xlxl5CZKllBIaax0Rr5n53tqB3Ti3k7qPiEUpZQAAggEACAYAIBgAgGAAoG8Ey9oRAHBas9oR5NgcIDOz5TN4pjnIJiJeapwTWAFGfMR2CDRlJViUUuYAtAfgOSK+Jv5N8FbddlBGav4M7+9795jHUsqqTGtdFQIAxgE0jQCAaQCaRQDAdABNIgDgMADNIQDgcAB/EHxWjwCA4wDsvvahegQAHA+gCQQAnAagegQAnA6gagQAnAdArQhcDdx//D+ZeXvg95tHxDK21wbG2mTm/SWP38Wgcz+jMj8i4ikiVhMePrv0z3vnlO1/grS+DVoBehfuVwCAABAAAkAAqLO6nwP896Tz2ucIVgBbgAAQAAJAAAgAASAABIAAEAACQAAIADXZyfcD9P55A7W/c8oKYAsQAAJAAAgAASBzgJ5eB1sBBIAAEAACQAAIAJkDTM/9AO4HEAACQAAIAAEgANTPHMD9AFYAASAABIAAEAACQP3MAWq/H6D3OYYVwBYgAASAABAAAkDmAF5HWwEEgAAQAAJAAAgAASAABIAAEAACQAAIAAEgAASAABAAAkAACAABIAAEgAAQAAJAAAgAXVWj/x+g988FtAIIAAEgAASAABAAaqhfB1BFkJjdTNQAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-codeblock-include/)
 [![License](https://img.shields.io/pypi/l/pandoc-codeblock-include.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAABmCAYAAAADI5lUAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiQKA106BAAABUNJREFUeNrtnV2IFlUYx3/P625qbrGlpWmWdaMVKau2EmpCrSDqxRpUUkr0SYVEFyFRUXQhfUAihTdCESVpKpKQpLZBsghltn605VVKpmZgGYvmbhpPFzMbWu3LO7szO1//H+zN7sw5c57nd8685+zMeY0quLsB04FW4A7gWmAMMAyRRbqBE8BRYCfwMfCNmXlfJ1iV5LcAbwBNimuu+Q54xcw21iSAuzcA7wOLFLtCsQl4yMxO9ymAu48HtgK3Kl6F5ACw0Mx++o8AYc/fBUxWnArN98DtZtYFULngDx8o+aXgZuDdi0YAd58fDv2iPMwzs+0WTvX2qfeXjv1Ak7n7DOBLxaOU3FYhWOQR5aS1AsxWHErLnArB8q4oJ+PM3buBoRFO6gJ2K3aZpBm4PMLxPXh09ijO2cTd90RNZkVhKzcSQAIICSAkgJAAQgIICSAkgJAAQgIICSAKT91gVOLui4EVKbZzvZm9kGD7rgHmEbw9NRoYCTQCvwInCd7UaQPaep/GLZUABP+ivDHFdo5KKPHTgNeAu6jyllXIk8A5d/8QeN7MjusWkGPcfRnBs5QtNSS/l3rgQaDT3e+UAPlN/iPA2wMYQa8APnH3ZgmQv+SPBlbGUNRw4D13r5MA+WIF0R67qsZNwMMSID+9vwF4IOZin5AA+WE+8W+O0eTuN0iAfNCSs3IlQMxMSqjciRIgH0wsmgCDNQU5CKxJMXHtMXwAHAJcndD1jSu0AGbWHkcSUmZEgmVfqltA9kkySQ0SIPsMyWnZEiAm/kiw7DMSIPt0AecSKvukBMg4ZvYXcCSh4g9LgHzwVc7KzcY00N0XAM+kmLitZrYqhnLagPsTuL7PCy0AwUJHS4oCHMpwok4AnboF5ONzwJFwFIiTd6pt5y4BssebMZbVA6xOszESIDrbiW+TrDVm9rMEyNdtwIHHgPMDLOoX4KW02yMB+ifBAWCgs4qnzex3CZBfXgS+7ee568xsQxYaIQH6Pwr0ELzk8WfEU48Dy7LSDgkwMAn2Eu2dRwceNbPfJEBxeD3s1bWwzcw+zdLFD9ZK4DHiX0CJwsEkbwXuvrrGkWBl5vTVXsGxxHBaDXE76+71CV+H9gpOiRM1HHPKzM5l7cIlQDxcX8Mxo9x9uAQoJktqOKYeuE8CFO/+P5NgabgWXnX3sRKgOMmfDWyJMJsaA+xw9wkSIN+Jr7j7U+HUdmTE028Bdrv73NKsA4Q9ZUmK7Ww3s7UxtaUZeAuYMYBirgpHgg3AcjP7sdACEOyE8XjKsq8dSI8H5gLPEu+jbfcCi9x9PbDKzDqKKkBeh/rpwN0Eu4Jcl1A19cBSYKm77wXWAZvN7AcJkG7ypwBfD3K1TeHPy+7eaGbnk65QHwL7ZlKKdY8AxmsWkC5XlqF+CdA3jWWoXwL0TUPK9V8mAdLlkpTrr5cA6VInAcpNfRnqHyzLu4jvBc3+0J8NGE6lfM1nB6UWPRJWHPRImNBnACEBhAQQEkBIACEBhAQQEkBIACEBhAQQ/8bcvRsYGuGcLuLbJ0/ESzPRvtW0x9z9MDBBsSslhyoE27eIcnKsAuxUHErLFxWC15tFOdli7m7AXmCK4lEq9gFTK+Hmx88pHqVjuZkFj4SZ2TZgs2JSGjaa2WcA1vsbd28AdgGTFZ9Csx+YaWZn4IKVQDM7DSwIDxDFve8v7E3+RQKEEhwFZgGbFKvC8REwK8wx/ytA70hgZvcQbInSobjlns6w1y++sOf/k+9qZ4ZTxKlAKzCH4OvfxgLDFNdM0k2wc/lRggW+LUBHtW8l+xuWwqBw5I0ApAAAAABJRU5ErkJggg==)](https://raw.githubusercontent.com/chdemko/pandoc-codeblock-include/develop/LICENSE)
```

### Comparing `pandoc_codeblock_include-1.0.1.1/pandoc_codeblock_include.py` & `pandoc_codeblock_include-1.0.1.2/pandoc_codeblock_include.py`

 * *Files identical despite different names*

### Comparing `pandoc_codeblock_include-1.0.1.1/pyproject.toml` & `pandoc_codeblock_include-1.0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
     requires = ["poetry-core>=1.2"]
     build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
     name = "pandoc-codeblock-include"
-    version = "1.0.1.1"
+    version = "1.0.1.2"
     description="A pandoc filter for including file in block code"
     authors = ["Christophe Demko <chdemko@gmail.com>"]
     license = "BSD-3-Clause"
     readme = "README.md"
     homepage="https://github.com/chdemko/pandoc-codeblock-include"
     keywords=["pandoc", "filters", "codeblock", "include"]
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
@@ -81,9 +81,9 @@
     ruff = "^0.0.254"
     darglint = "^1.8.1"
     teyit = {version = "^0.4.3", python = ">=3.9"}
     slotscheck = "^0.16.5"
     refurb = {version = "^1.16.0", python = ">=3.10"}
     
 [tool.poetry.scripts]
-   -codeblock-include = "pandoc_codeblock_include:main"
+   pandoc-codeblock-include = "pandoc_codeblock_include:main"
```

### Comparing `pandoc_codeblock_include-1.0.1.1/PKG-INFO` & `pandoc_codeblock_include-1.0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandoc-codeblock-include
-Version: 1.0.1.1
+Version: 1.0.1.2
 Summary: A pandoc filter for including file in block code
 Home-page: https://github.com/chdemko/pandoc-codeblock-include
 License: BSD-3-Clause
 Keywords: pandoc,filters,codeblock,include
 Author: Christophe Demko
 Author-email: chdemko@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -24,15 +24,15 @@
 Classifier: Topic :: Text Processing :: Filters
 Requires-Dist: panflute (>=2.3.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 Installation
 ============
 
-![Python package](https://github.com/chdemko/pandoc-codeblock-include/workflows/Python%20package/badge.svg?branch=develop)
+[![Python package](https://github.com/chdemko/pandoc-codeblock-include/workflows/Python%20package/badge.svg?branch=develop)](https://github.com/chdemko/pandoc-codeblock-include/actions/workflows/python-package.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/chdemko/pandoc-codeblock-include/develop.svg?logo=Codecov&logoColor=white)](https://coveralls.io/github/chdemko/pandoc-codeblock-include?branch=develop)
 [![Code Climate](https://codeclimate.com/github/chdemko/pandoc-codeblock-include/badges/gpa.svg)](https://codeclimate.com/github/chdemko/pandoc-codeblock-include/)
 [![Code Beat](https://codebeat.co/badges/c0e680bd-9c47-4180-8d3f-b706905d0e73)](https://codebeat.co/projects/github-com-chdemko-pandoc-codeblock-include-develop/)
 [![Codacy](https://img.shields.io/codacy/grade/26716ef242ba4089aff55eff7ca592a9.svg?logo=codacy&logoColor=white)](https://app.codacy.com/gh/chdemko/pandoc-codeblock-include/)
 [![PyPI version](https://img.shields.io/pypi/v/pandoc-codeblock-include.svg?logo=Python&logoColor=white)](https://pypi.org/project/pandoc-codeblock-include/)
 [![PyPI format](https://img.shields.io/pypi/format/pandoc-codeblock-include.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAACACAYAAADDPmHLAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiYw92eBNAAAAgJJREFUeNrt3T1WwkAUgNH31Br3ogWptdAlgyvQxYgHeh0LKKxI+PHAzNyvRo8xlxl5CZKllBIaax0Rr5n53tqB3Ti3k7qPiEUpZQAAggEACAYAIBgAgGAAoG8Ey9oRAHBas9oR5NgcIDOz5TN4pjnIJiJeapwTWAFGfMR2CDRlJViUUuYAtAfgOSK+Jv5N8FbddlBGav4M7+9795jHUsqqTGtdFQIAxgE0jQCAaQCaRQDAdABNIgDgMADNIQDgcAB/EHxWjwCA4wDsvvahegQAHA+gCQQAnAagegQAnA6gagQAnAdArQhcDdx//D+ZeXvg95tHxDK21wbG2mTm/SWP38Wgcz+jMj8i4ikiVhMePrv0z3vnlO1/grS+DVoBehfuVwCAABAAAkAAqLO6nwP896Tz2ucIVgBbgAAQAAJAAAgAASAABIAAEAACQAAIADXZyfcD9P55A7W/c8oKYAsQAAJAAAgAASBzgJ5eB1sBBIAAEAACQAAIAJkDTM/9AO4HEAACQAAIAAEgANTPHMD9AFYAASAABIAAEAACQP3MAWq/H6D3OYYVwBYgAASAABAAAkDmAF5HWwEEgAAQAAJAAAgAASAABIAAEAACQAAIAAEgAASAABAAAkAACAABIAAEgAAQAAJAAAgAXVWj/x+g988FtAIIAAEgAASAABAAaqhfB1BFkJjdTNQAAAAASUVORK5CYII=)](https://pypi.org/project/pandoc-codeblock-include/)
 [![License](https://img.shields.io/pypi/l/pandoc-codeblock-include.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIAAAABmCAYAAAADI5lUAAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA3XAAAN1wFCKJt4AAAAB3RJTUUH4gwPFiQKA106BAAABUNJREFUeNrtnV2IFlUYx3/P625qbrGlpWmWdaMVKau2EmpCrSDqxRpUUkr0SYVEFyFRUXQhfUAihTdCESVpKpKQpLZBsghltn605VVKpmZgGYvmbhpPFzMbWu3LO7szO1//H+zN7sw5c57nd8685+zMeY0quLsB04FW4A7gWmAMMAyRRbqBE8BRYCfwMfCNmXlfJ1iV5LcAbwBNimuu+Q54xcw21iSAuzcA7wOLFLtCsQl4yMxO9ymAu48HtgK3Kl6F5ACw0Mx++o8AYc/fBUxWnArN98DtZtYFULngDx8o+aXgZuDdi0YAd58fDv2iPMwzs+0WTvX2qfeXjv1Ak7n7DOBLxaOU3FYhWOQR5aS1AsxWHErLnArB8q4oJ+PM3buBoRFO6gJ2K3aZpBm4PMLxPXh09ijO2cTd90RNZkVhKzcSQAIICSAkgJAAQgIICSAkgJAAQgIICSAKT91gVOLui4EVKbZzvZm9kGD7rgHmEbw9NRoYCTQCvwInCd7UaQPaep/GLZUABP+ivDHFdo5KKPHTgNeAu6jyllXIk8A5d/8QeN7MjusWkGPcfRnBs5QtNSS/l3rgQaDT3e+UAPlN/iPA2wMYQa8APnH3ZgmQv+SPBlbGUNRw4D13r5MA+WIF0R67qsZNwMMSID+9vwF4IOZin5AA+WE+8W+O0eTuN0iAfNCSs3IlQMxMSqjciRIgH0wsmgCDNQU5CKxJMXHtMXwAHAJcndD1jSu0AGbWHkcSUmZEgmVfqltA9kkySQ0SIPsMyWnZEiAm/kiw7DMSIPt0AecSKvukBMg4ZvYXcCSh4g9LgHzwVc7KzcY00N0XAM+kmLitZrYqhnLagPsTuL7PCy0AwUJHS4oCHMpwok4AnboF5ONzwJFwFIiTd6pt5y4BssebMZbVA6xOszESIDrbiW+TrDVm9rMEyNdtwIHHgPMDLOoX4KW02yMB+ifBAWCgs4qnzex3CZBfXgS+7ee568xsQxYaIQH6Pwr0ELzk8WfEU48Dy7LSDgkwMAn2Eu2dRwceNbPfJEBxeD3s1bWwzcw+zdLFD9ZK4DHiX0CJwsEkbwXuvrrGkWBl5vTVXsGxxHBaDXE76+71CV+H9gpOiRM1HHPKzM5l7cIlQDxcX8Mxo9x9uAQoJktqOKYeuE8CFO/+P5NgabgWXnX3sRKgOMmfDWyJMJsaA+xw9wkSIN+Jr7j7U+HUdmTE028Bdrv73NKsA4Q9ZUmK7Ww3s7UxtaUZeAuYMYBirgpHgg3AcjP7sdACEOyE8XjKsq8dSI8H5gLPEu+jbfcCi9x9PbDKzDqKKkBeh/rpwN0Eu4Jcl1A19cBSYKm77wXWAZvN7AcJkG7ypwBfD3K1TeHPy+7eaGbnk65QHwL7ZlKKdY8AxmsWkC5XlqF+CdA3jWWoXwL0TUPK9V8mAdLlkpTrr5cA6VInAcpNfRnqHyzLu4jvBc3+0J8NGE6lfM1nB6UWPRJWHPRImNBnACEBhAQQEkBIACEBhAQQEkBIACEBhAQQ/8bcvRsYGuGcLuLbJ0/ESzPRvtW0x9z9MDBBsSslhyoE27eIcnKsAuxUHErLFxWC15tFOdli7m7AXmCK4lEq9gFTK+Hmx88pHqVjuZkFj4SZ2TZgs2JSGjaa2WcA1vsbd28AdgGTFZ9Csx+YaWZn4IKVQDM7DSwIDxDFve8v7E3+RQKEEhwFZgGbFKvC8REwK8wx/ytA70hgZvcQbInSobjlns6w1y++sOf/k+9qZ4ZTxKlAKzCH4OvfxgLDFNdM0k2wc/lRggW+LUBHtW8l+xuWwqBw5I0ApAAAAABJRU5ErkJggg==)](https://raw.githubusercontent.com/chdemko/pandoc-codeblock-include/develop/LICENSE)
```

