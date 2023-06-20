# Comparing `tmp/tqdm_loggable-0.1.3.tar.gz` & `tmp/tqdm_loggable-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tqdm_loggable-0.1.3.tar", max compression
+gzip compressed data, was "tqdm_loggable-0.1.4.tar", max compression
```

## Comparing `tqdm_loggable-0.1.3.tar` & `tqdm_loggable-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     7660 2022-11-29 10:07:25.339524 tqdm_loggable-0.1.3/README.md
--rw-r--r--   0        0        0      848 2023-01-26 17:57:52.925490 tqdm_loggable-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2022-09-20 20:31:08.634217 tqdm_loggable-0.1.3/tqdm_loggable/__init__.py
--rw-r--r--   0        0        0      236 2022-12-09 08:59:14.033580 tqdm_loggable-0.1.3/tqdm_loggable/auto.py
--rw-r--r--   0        0        0     1398 2022-09-21 10:15:04.851282 tqdm_loggable-0.1.3/tqdm_loggable/manual_tests.py
--rw-r--r--   0        0        0     5916 2023-01-26 17:57:32.829295 tqdm_loggable-0.1.3/tqdm_loggable/tqdm_logging.py
--rw-r--r--   0        0        0     1756 2022-11-29 10:04:15.518725 tqdm_loggable-0.1.3/tqdm_loggable/utils.py
--rw-r--r--   0        0        0     8687 1970-01-01 00:00:00.000000 tqdm_loggable-0.1.3/setup.py
--rw-r--r--   0        0        0     8476 1970-01-01 00:00:00.000000 tqdm_loggable-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     7913 2023-06-20 08:43:11.123043 tqdm_loggable-0.1.4/README.md
+-rw-r--r--   0        0        0      848 2023-06-20 08:43:44.164335 tqdm_loggable-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-09-20 20:31:08.634217 tqdm_loggable-0.1.4/tqdm_loggable/__init__.py
+-rw-r--r--   0        0        0      379 2023-06-20 08:40:47.694326 tqdm_loggable-0.1.4/tqdm_loggable/auto.py
+-rw-r--r--   0        0        0     1398 2022-09-21 10:15:04.851282 tqdm_loggable-0.1.4/tqdm_loggable/manual_tests.py
+-rw-r--r--   0        0        0     5916 2023-01-26 17:57:32.829295 tqdm_loggable-0.1.4/tqdm_loggable/tqdm_logging.py
+-rw-r--r--   0        0        0     2310 2023-06-20 08:40:47.694871 tqdm_loggable-0.1.4/tqdm_loggable/utils.py
+-rw-r--r--   0        0        0     8729 1970-01-01 00:00:00.000000 tqdm_loggable-0.1.4/PKG-INFO
```

### Comparing `tqdm_loggable-0.1.3/README.md` & `tqdm_loggable-0.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 tqdm-loggable
 =============
 
-`tqdm-loggable` is petite Python package providing logging friendly TQDM progress bars.
+`tqdm-loggable` is a petite Python package providing logging friendly TQDM progress bars.
 
 If your Python application has [tqdm](https://tqdm.github.io/) progress bars and you use them in a non-interactive session like... 
 
 - Background worker
 - Docker container
 - Edge computing
 - [Logstash](https://www.elastic.co/logstash/), [Sentry](https://docs.sentry.io/platforms/python/), [Datadog](https://docs.datadoghq.com/logs/log_collection/python/?tab=jsonlogformatter) or other external log tools
@@ -17,15 +17,14 @@
 application is having`tqdm` progress ongoing. If the progress bar'ed operation takes few minutes your appliaction
 may appear frozen. This is  fixed by `tqdm-logging` by sending a regular reports about your progress to logging backend like files and log monitoring
 tools.
 
 In these situations `tqdm-loggable` will automatically turn your `tqdm` progress bars to loggable progress messages
 that can be read in headless systems.
 
-
 `tqdm-loggable`... 
 
 - Is a drop-in replacement for the normal `tqdm` - nothing changes unless non-interactive session is detected
 - Uses Python [logging](https://docs.python.org/3/library/logging.html) subsystem to report status instead of terminal
 - Print a log line for every X seconds
 - [The logging messages are structured](https://docs.python.org/3/howto/logging-cookbook.html#implementing-structured-logging), so they work with Sentry, LogStash, etc. rich logging services
   which provide advanced searching and tagging by variables
@@ -108,14 +107,17 @@
 ```
 
 `tqdm_loggable` will detect non-interactive sessions.
 If the application is running without a proper terminal, non-interactive progress messages will be used.
 Otherwise progress bar is delegated `tqdm.auto` module to maintain the compatibility
 with any `tqdm` system without any changes to code.
 
+`tqdm_loggable` has also progress bar workarounds for [Jupyter Notebook environments](https://jupyter.org/)
+like [Datalore](https://www.jetbrains.com/datalore/) which [are not 100% compatible](https://jupyter.org/) with the original Jupyter Notebook.
+
 The Python logger instance used to log the messages is named `tqqm_loggable.tqm_logging`.
 
 Development
 -----------
 
 You can use [tqdm_loggable/manual_tests.py](./tqdm_loggable/manual_tests.py) to run the various checks 
 to see what different interactive and non-interactive sessions give for you.
```

### Comparing `tqdm_loggable-0.1.3/pyproject.toml` & `tqdm_loggable-0.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tqdm-loggable"
-version = "0.1.3"
+version = "0.1.4"
 description = "TQDM progress bar friendliness for non-interactive terminals and logging output"
 authors = ["Mikko Ohtamaa <mikko@opensourcehacker.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "tqdm_loggable"}]
 homepage = "https://tradingstrategy.ai"
 repository = "https://github.com/tradingstrategy-ai/tqdm-loggable"
```

### Comparing `tqdm_loggable-0.1.3/tqdm_loggable/manual_tests.py` & `tqdm_loggable-0.1.4/tqdm_loggable/manual_tests.py`

 * *Files identical despite different names*

### Comparing `tqdm_loggable-0.1.3/tqdm_loggable/tqdm_logging.py` & `tqdm_loggable-0.1.4/tqdm_loggable/tqdm_logging.py`

 * *Files identical despite different names*

### Comparing `tqdm_loggable-0.1.3/setup.py` & `tqdm_loggable-0.1.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,218 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: tqdm-loggable
+Version: 0.1.4
+Summary: TQDM progress bar friendliness for non-interactive terminals and logging output
+Home-page: https://tradingstrategy.ai
+License: MIT
+Keywords: logging,tqdm,sentry,logstash,progress bar,datadog,new relic
+Author: Mikko Ohtamaa
+Author-email: mikko@opensourcehacker.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: tqdm (>=4.64.1,<5.0.0)
+Project-URL: Repository, https://github.com/tradingstrategy-ai/tqdm-loggable
+Description-Content-Type: text/markdown
 
-packages = \
-['tqdm_loggable']
+tqdm-loggable
+=============
 
-package_data = \
-{'': ['*']}
+`tqdm-loggable` is a petite Python package providing logging friendly TQDM progress bars.
 
-install_requires = \
-['tqdm>=4.64.1,<5.0.0']
-
-entry_points = \
-{'console_scripts': ['manual-tests = tqdm_loggable.manual_tests:main']}
-
-setup_kwargs = {
-    'name': 'tqdm-loggable',
-    'version': '0.1.3',
-    'description': 'TQDM progress bar friendliness for non-interactive terminals and logging output',
-    'long_description': 'tqdm-loggable\n=============\n\n`tqdm-loggable` is petite Python package providing logging friendly TQDM progress bars.\n\nIf your Python application has [tqdm](https://tqdm.github.io/) progress bars and you use them in a non-interactive session like... \n\n- Background worker\n- Docker container\n- Edge computing\n- [Logstash](https://www.elastic.co/logstash/), [Sentry](https://docs.sentry.io/platforms/python/), [Datadog](https://docs.datadoghq.com/logs/log_collection/python/?tab=jsonlogformatter) or other external log tools\n- Long-running machine learning tasks\n- ...or [stdout](https://en.wikipedia.org/wiki/Standard_streams) stream is otherwise not available or redirected\n\n...you cannot have interactive progress bar. What happens is that if you are observing\nyour application using monitoring tools, you usually do not see anything happening while your\napplication is having`tqdm` progress ongoing. If the progress bar\'ed operation takes few minutes your appliaction\nmay appear frozen. This is  fixed by `tqdm-logging` by sending a regular reports about your progress to logging backend like files and log monitoring\ntools.\n\nIn these situations `tqdm-loggable` will automatically turn your `tqdm` progress bars to loggable progress messages\nthat can be read in headless systems.\n\n\n`tqdm-loggable`... \n\n- Is a drop-in replacement for the normal `tqdm` - nothing changes unless non-interactive session is detected\n- Uses Python [logging](https://docs.python.org/3/library/logging.html) subsystem to report status instead of terminal\n- Print a log line for every X seconds\n- [The logging messages are structured](https://docs.python.org/3/howto/logging-cookbook.html#implementing-structured-logging), so they work with Sentry, LogStash, etc. rich logging services\n  which provide advanced searching and tagging by variables\n- Special support for Github Actions and other continous integration environments\n\nHere is a sample `tqdm` log message output in plain text logs:\n\n```\ntqdm_logging.py     :139  2022-09-21 12:13:44,138 Progress on:Progress bar without total -/- rate:- remaining:? elapsed:00:00 postfix:-\ntqdm_logging.py     :139  2022-09-21 12:13:46,225 Progress on:Progress bar without total 10000/- rate:- remaining:? elapsed:00:02 postfix:-\n\ntqdm_logging.py     :139  2022-09-21 12:13:46,225 Progress on:Sample progress -/60000 rate:- remaining:? elapsed:00:00 postfix:-\ntqdm_logging.py     :139  2022-09-21 12:13:56,307 Progress on:Sample progress 21.0kit/60.0kit rate:1,982.9it/s remaining:00:19 elapsed:00:10 postfix:Current time=2022-09-21 10:13:55.801787\ntqdm_logging.py     :139  2022-09-21 12:14:06,392 Progress on:Sample progress 41.0kit/60.0kit rate:1,984.1it/s remaining:00:09 elapsed:00:20 postfix:Current time=2022-09-21 10:14:05.890220\n```\n\nNote that `tqdm-loggable` is not to be confused with [tqdm.contrib.logging](https://tqdm.github.io/docs/contrib.logging/) \nthat is very different approach for a different problem.\n\nInstallation\n------------\n\nThe package name is `tqdm-loggable.` [Read Python packaging manual](https://packaging.python.org/en/latest/) on how to install packages\non your system.\n\nUsage\n-----\n\nThe only things you need to do\n\n- Make sure your [Python logging system is properly configured](https://docs.python.org/3/howto/logging.html)\n- Change import from `from tqdm.auto import tqdm` to `from tqdm_loggable.auto import tqdm`\n- Optionally call `tqdm_logging.set_level()` at the init of your application\n- Optionally call `tqdm_logging.set_log_rate()` at the init of your application\n\nSearch and replace instructions for your Python codebase:\n\n```\nfrom tqdm import tqdm -> from tqdm_loggable.auto import tqdm \nfrom tqdm.auto import tqdm -> from tqdm_loggable.auto import tqdm\n```\n\nHere is [an example script](./tqdm_loggable/manual_tests.py):\n\n```python\nimport datetime\nimport logging\nimport time\n\nfrom tqdm_loggable.auto import tqdm\nfrom tqdm_loggable.tqdm_logging import tqdm_logging\n\n\nlogger = logging.getLogger(__name__)\n\n\ndef main():\n    fmt = f"%(filename)-20s:%(lineno)-4d %(asctime)s %(message)s"\n    logging.basicConfig(level=logging.INFO, format=fmt, handlers=[logging.StreamHandler()])\n\n    # Set the log level to all tqdm-logging progress bars.\n    # Defaults to info - no need to set if you do not want to change the level\n    tqdm_logging.set_level(logging.INFO)\n    \n    # Set the rate how often we update logs\n    # Defaults to 10 seconds - optional\n    tqdm_logging.set_log_rate(datetime.timedelta(seconds=10))    \n\n    logger.info("This is an INFO test message using Python logging")\n\n    with tqdm(total=60_000, desc="Sample progress", unit_scale=True) as progress_bar:\n        for i in range(60_000):\n            progress_bar.update(1000)\n\n            # Test postfix output\n            progress_bar.set_postfix({"Current time": datetime.datetime.utcnow()})\n\n            time.sleep(0.5)\n\n```\n\n`tqdm_loggable` will detect non-interactive sessions.\nIf the application is running without a proper terminal, non-interactive progress messages will be used.\nOtherwise progress bar is delegated `tqdm.auto` module to maintain the compatibility\nwith any `tqdm` system without any changes to code.\n\nThe Python logger instance used to log the messages is named `tqqm_loggable.tqm_logging`.\n\nDevelopment\n-----------\n\nYou can use [tqdm_loggable/manual_tests.py](./tqdm_loggable/manual_tests.py) to run the various checks \nto see what different interactive and non-interactive sessions give for you.\n\n```shell\n# Normal interactive terminal run\npoetry run manual-tests \n```\n\nBecause this is a normal shell session you will get a normal progress bar:\n\n```\nSample progress:  20%|████████▏                                | 12.0k/60.0k [00:05<00:24, 1.98kit/s, Current time=2022-09-21 15:40:24.274670]\n```\n\n...then test without without a proper [TERM environment variable](https://unix.stackexchange.com/questions/528323/what-uses-the-term-variable):\n\n```shell\n# Disable interactive terminal by fiddling with TERM environment variable\nTERM=dumb poetry run manual-tests \n```\n\nYou get log messages:\n\n```\ntqdm_logging.py     :139  2022-09-21 17:41:20,720 Progress on:Sample progress -/60000 rate:- remaining:? elapsed:00:00 postfix:-\ntqdm_logging.py     :139  2022-09-21 17:41:30,803 Progress on:Sample progress 21.0kit/60.0kit rate:1,984.7it/s remaining:00:19 elapsed:00:10 postfix:Current time=2022-09-21 15:41:30.300714\n```\n\n...or with different Docker sessions:\n\n```shell\n# This will display process as log messages\ndocker build -t manual-tests . && docker run manual-tests\n\n# This will allocate a terminal and display progress as a normal tqdm progress bar\ndocker build -t manual-tests . && docker run -ti manual-tests\n```\n\nor with redirected stdout:\n\n```shell\npoetry run manual-tests > output.txt\ncat output.txt\n```\n\nThese will output our terminal detection info and draw a progress bar, total 30 seconds.\n\n```\ntqdm-loggable manual tests\nsys.stdout.isatty(): False\nTERM: -\nis_interactive_session(): False\n```\n\nand further progress bar or progress messages will follow depending\nif you run the manual test interactively or not.\n\nSee also\n--------\n\nSee other relevant logging packages:\n\n- [tqdm-loggable on PyPi](https://pypi.org/project/tqdm-loggable/)\n- [python-discord-logging-handler](https://github.com/tradingstrategy-ai/python-logging-discord-handler)\n- [python-logstash](https://github.com/tradingstrategy-ai/python-logstash)\n\nKudos\n-----\n\nOriginally build for [Trading Strategy blockchain trade automation](https://tradingstrategy.ai/docs/).\n\n[See the original StackOverflow question](https://stackoverflow.com/questions/73433322/tqdm-progress-bar-with-docker-logs).\n\nLicense\n-------\n\nMIT',
-    'author': 'Mikko Ohtamaa',
-    'author_email': 'mikko@opensourcehacker.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://tradingstrategy.ai',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+If your Python application has [tqdm](https://tqdm.github.io/) progress bars and you use them in a non-interactive session like... 
 
+- Background worker
+- Docker container
+- Edge computing
+- [Logstash](https://www.elastic.co/logstash/), [Sentry](https://docs.sentry.io/platforms/python/), [Datadog](https://docs.datadoghq.com/logs/log_collection/python/?tab=jsonlogformatter) or other external log tools
+- Long-running machine learning tasks
+- ...or [stdout](https://en.wikipedia.org/wiki/Standard_streams) stream is otherwise not available or redirected
 
-setup(**setup_kwargs)
+...you cannot have interactive progress bar. What happens is that if you are observing
+your application using monitoring tools, you usually do not see anything happening while your
+application is having`tqdm` progress ongoing. If the progress bar'ed operation takes few minutes your appliaction
+may appear frozen. This is  fixed by `tqdm-logging` by sending a regular reports about your progress to logging backend like files and log monitoring
+tools.
+
+In these situations `tqdm-loggable` will automatically turn your `tqdm` progress bars to loggable progress messages
+that can be read in headless systems.
+
+`tqdm-loggable`... 
+
+- Is a drop-in replacement for the normal `tqdm` - nothing changes unless non-interactive session is detected
+- Uses Python [logging](https://docs.python.org/3/library/logging.html) subsystem to report status instead of terminal
+- Print a log line for every X seconds
+- [The logging messages are structured](https://docs.python.org/3/howto/logging-cookbook.html#implementing-structured-logging), so they work with Sentry, LogStash, etc. rich logging services
+  which provide advanced searching and tagging by variables
+- Special support for Github Actions and other continous integration environments
+
+Here is a sample `tqdm` log message output in plain text logs:
+
+```
+tqdm_logging.py     :139  2022-09-21 12:13:44,138 Progress on:Progress bar without total -/- rate:- remaining:? elapsed:00:00 postfix:-
+tqdm_logging.py     :139  2022-09-21 12:13:46,225 Progress on:Progress bar without total 10000/- rate:- remaining:? elapsed:00:02 postfix:-
+
+tqdm_logging.py     :139  2022-09-21 12:13:46,225 Progress on:Sample progress -/60000 rate:- remaining:? elapsed:00:00 postfix:-
+tqdm_logging.py     :139  2022-09-21 12:13:56,307 Progress on:Sample progress 21.0kit/60.0kit rate:1,982.9it/s remaining:00:19 elapsed:00:10 postfix:Current time=2022-09-21 10:13:55.801787
+tqdm_logging.py     :139  2022-09-21 12:14:06,392 Progress on:Sample progress 41.0kit/60.0kit rate:1,984.1it/s remaining:00:09 elapsed:00:20 postfix:Current time=2022-09-21 10:14:05.890220
+```
+
+Note that `tqdm-loggable` is not to be confused with [tqdm.contrib.logging](https://tqdm.github.io/docs/contrib.logging/) 
+that is very different approach for a different problem.
+
+Installation
+------------
+
+The package name is `tqdm-loggable.` [Read Python packaging manual](https://packaging.python.org/en/latest/) on how to install packages
+on your system.
+
+Usage
+-----
+
+The only things you need to do
+
+- Make sure your [Python logging system is properly configured](https://docs.python.org/3/howto/logging.html)
+- Change import from `from tqdm.auto import tqdm` to `from tqdm_loggable.auto import tqdm`
+- Optionally call `tqdm_logging.set_level()` at the init of your application
+- Optionally call `tqdm_logging.set_log_rate()` at the init of your application
+
+Search and replace instructions for your Python codebase:
+
+```
+from tqdm import tqdm -> from tqdm_loggable.auto import tqdm 
+from tqdm.auto import tqdm -> from tqdm_loggable.auto import tqdm
+```
+
+Here is [an example script](./tqdm_loggable/manual_tests.py):
+
+```python
+import datetime
+import logging
+import time
+
+from tqdm_loggable.auto import tqdm
+from tqdm_loggable.tqdm_logging import tqdm_logging
+
+
+logger = logging.getLogger(__name__)
+
+
+def main():
+    fmt = f"%(filename)-20s:%(lineno)-4d %(asctime)s %(message)s"
+    logging.basicConfig(level=logging.INFO, format=fmt, handlers=[logging.StreamHandler()])
+
+    # Set the log level to all tqdm-logging progress bars.
+    # Defaults to info - no need to set if you do not want to change the level
+    tqdm_logging.set_level(logging.INFO)
+    
+    # Set the rate how often we update logs
+    # Defaults to 10 seconds - optional
+    tqdm_logging.set_log_rate(datetime.timedelta(seconds=10))    
+
+    logger.info("This is an INFO test message using Python logging")
+
+    with tqdm(total=60_000, desc="Sample progress", unit_scale=True) as progress_bar:
+        for i in range(60_000):
+            progress_bar.update(1000)
+
+            # Test postfix output
+            progress_bar.set_postfix({"Current time": datetime.datetime.utcnow()})
+
+            time.sleep(0.5)
+
+```
+
+`tqdm_loggable` will detect non-interactive sessions.
+If the application is running without a proper terminal, non-interactive progress messages will be used.
+Otherwise progress bar is delegated `tqdm.auto` module to maintain the compatibility
+with any `tqdm` system without any changes to code.
+
+`tqdm_loggable` has also progress bar workarounds for [Jupyter Notebook environments](https://jupyter.org/)
+like [Datalore](https://www.jetbrains.com/datalore/) which [are not 100% compatible](https://jupyter.org/) with the original Jupyter Notebook.
+
+The Python logger instance used to log the messages is named `tqqm_loggable.tqm_logging`.
+
+Development
+-----------
+
+You can use [tqdm_loggable/manual_tests.py](./tqdm_loggable/manual_tests.py) to run the various checks 
+to see what different interactive and non-interactive sessions give for you.
+
+```shell
+# Normal interactive terminal run
+poetry run manual-tests 
+```
+
+Because this is a normal shell session you will get a normal progress bar:
+
+```
+Sample progress:  20%|████████▏                                | 12.0k/60.0k [00:05<00:24, 1.98kit/s, Current time=2022-09-21 15:40:24.274670]
+```
+
+...then test without without a proper [TERM environment variable](https://unix.stackexchange.com/questions/528323/what-uses-the-term-variable):
+
+```shell
+# Disable interactive terminal by fiddling with TERM environment variable
+TERM=dumb poetry run manual-tests 
+```
+
+You get log messages:
+
+```
+tqdm_logging.py     :139  2022-09-21 17:41:20,720 Progress on:Sample progress -/60000 rate:- remaining:? elapsed:00:00 postfix:-
+tqdm_logging.py     :139  2022-09-21 17:41:30,803 Progress on:Sample progress 21.0kit/60.0kit rate:1,984.7it/s remaining:00:19 elapsed:00:10 postfix:Current time=2022-09-21 15:41:30.300714
+```
+
+...or with different Docker sessions:
+
+```shell
+# This will display process as log messages
+docker build -t manual-tests . && docker run manual-tests
+
+# This will allocate a terminal and display progress as a normal tqdm progress bar
+docker build -t manual-tests . && docker run -ti manual-tests
+```
+
+or with redirected stdout:
+
+```shell
+poetry run manual-tests > output.txt
+cat output.txt
+```
+
+These will output our terminal detection info and draw a progress bar, total 30 seconds.
+
+```
+tqdm-loggable manual tests
+sys.stdout.isatty(): False
+TERM: -
+is_interactive_session(): False
+```
+
+and further progress bar or progress messages will follow depending
+if you run the manual test interactively or not.
+
+See also
+--------
+
+See other relevant logging packages:
+
+- [tqdm-loggable on PyPi](https://pypi.org/project/tqdm-loggable/)
+- [python-discord-logging-handler](https://github.com/tradingstrategy-ai/python-logging-discord-handler)
+- [python-logstash](https://github.com/tradingstrategy-ai/python-logstash)
+
+Kudos
+-----
+
+Originally build for [Trading Strategy blockchain trade automation](https://tradingstrategy.ai/docs/).
+
+[See the original StackOverflow question](https://stackoverflow.com/questions/73433322/tqdm-progress-bar-with-docker-logs).
+
+License
+-------
+
+MIT
```

