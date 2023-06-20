# Comparing `tmp/logbt-0.1.0.tar.gz` & `tmp/logbt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logbt-0.1.0.tar", max compression
+gzip compressed data, was "logbt-0.2.0.tar", max compression
```

## Comparing `logbt-0.1.0.tar` & `logbt-0.2.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       25 2023-06-11 14:41:49.464192 logbt-0.1.0/README.md
--rw-r--r--   0        0        0     1271 2023-06-11 14:51:38.812956 logbt-0.1.0/logbt/__init__.py
--rw-r--r--   0        0        0      276 2023-06-12 15:18:47.624881 logbt-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      636 1970-01-01 00:00:00.000000 logbt-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      317 2023-06-20 17:52:55.693151 logbt-0.2.0/README.md
+-rw-r--r--   0        0        0     1368 2023-06-20 17:52:22.316515 logbt-0.2.0/logbt/__init__.py
+-rw-r--r--   0        0        0      276 2023-06-20 17:52:33.088720 logbt-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      928 1970-01-01 00:00:00.000000 logbt-0.2.0/PKG-INFO
```

### Comparing `logbt-0.1.0/logbt/__init__.py` & `logbt-0.2.0/logbt/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -50,20 +50,24 @@
 
 def colorize(record):
     record["level"].name = f'[{record["level"].name}]'.ljust(10)
     record["module"] = random_color(f'[{record["module"]}]'.ljust(15))
     record["function"] = f'[{record["function"]}]'.ljust(10)
 
 
-loguru.logger.remove()
-logger = loguru.logger.patch(colorize)
+def config(level="INFO"):
+    splitter = " " * 3
+    logger.add(
+        sys.stdout,
+        colorize=True,
+        level=level,
+        format="SPLITTER[{time:YYYY-MM-DD HH:mm:ss}]"
+        "SPLITTER<level>{level}</level>"
+        "SPLITTER{module}"
+        "SPLITTER{function}"
+        "SPLITTER{message} :: ({file}:{line})".replace("SPLITTER", splitter),
+    )
 
-splitter = " " * 3
-logger.add(
-    sys.stdout,
-    colorize=True,
-    format="SPLITTER[{time:YYYY-MM-DD HH:mm:ss}]"
-    "SPLITTER<level>{level}</level>"
-    "SPLITTER{module}"
-    "SPLITTER{function}"
-    "SPLITTER{message} :: ({file}:{line})".replace("SPLITTER", splitter),
-)
+
+logger = loguru.logger
+logger.remove()
+logger = logger.patch(colorize)
```

### Comparing `logbt-0.1.0/PKG-INFO` & `logbt-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logbt
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: SmsS4
 Author-email: smss.lite@gmail.com
 Requires-Python: >=3.5
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
@@ -14,7 +14,32 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 Configuration for Loguru
 
+# Install
+
+```shell
+poetry add logbt
+```
+
+# Usage
+
+```python
+from logbt import config
+from logbt import logger
+
+config(level="DEBUG")
+
+
+def f():
+    logger.info("INSIDE function")
+
+
+logger.debug("YOU SHOULD NOT SEE THIS")
+logger.info("THIS IS INFO")
+logger.error("THIS IS NOT INFO")
+f()
+```
+
```

