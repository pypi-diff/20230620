# Comparing `tmp/vedro-playwright-1.1.0.tar.gz` & `tmp/vedro-playwright-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vedro-playwright-1.1.0.tar", last modified: Wed Jul 20 12:16:18 2022, max compression
+gzip compressed data, was "vedro-playwright-1.2.0.tar", last modified: Wed Nov 23 14:23:30 2022, max compression
```

## Comparing `vedro-playwright-1.1.0.tar` & `vedro-playwright-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 12:16:18.079259 vedro-playwright-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-07-20 12:16:09.000000 vedro-playwright-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3442 2022-07-20 12:16:18.079259 vedro-playwright-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2889 2022-07-20 12:16:09.000000 vedro-playwright-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      704 2022-07-20 12:16:18.083258 vedro-playwright-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-07-20 12:16:09.000000 vedro-playwright-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 12:16:18.079259 vedro-playwright-1.1.0/vedro_playwright/
--rw-r--r--   0 runner    (1001) docker     (121)      596 2022-07-20 12:16:09.000000 vedro-playwright-1.1.0/vedro_playwright/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-07-20 12:16:09.000000 vedro-playwright-1.1.0/vedro_playwright/_browser_engine.py
--rw-r--r--   0 runner    (1001) docker     (121)      512 2022-07-20 12:16:09.000000 vedro-playwright-1.1.0/vedro_playwright/_browser_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)     1689 2022-07-20 12:16:09.000000 vedro-playwright-1.1.0/vedro_playwright/_browsers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-07-20 12:16:09.000000 vedro-playwright-1.1.0/vedro_playwright/_screenshot_path.py
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-07-20 12:16:09.000000 vedro-playwright-1.1.0/vedro_playwright/_screenshots_mode.py
--rw-r--r--   0 runner    (1001) docker     (121)     6782 2022-07-20 12:16:09.000000 vedro-playwright-1.1.0/vedro_playwright/_vedro_playwright.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 12:16:09.000000 vedro-playwright-1.1.0/vedro_playwright/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 12:16:18.079259 vedro-playwright-1.1.0/vedro_playwright.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3442 2022-07-20 12:16:18.000000 vedro-playwright-1.1.0/vedro_playwright.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-07-20 12:16:18.000000 vedro-playwright-1.1.0/vedro_playwright.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-20 12:16:18.000000 vedro-playwright-1.1.0/vedro_playwright.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-20 12:16:18.000000 vedro-playwright-1.1.0/vedro_playwright.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-07-20 12:16:18.000000 vedro-playwright-1.1.0/vedro_playwright.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 14:23:30.130700 vedro-playwright-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-11-23 14:23:16.000000 vedro-playwright-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     3266 2022-11-23 14:23:30.130700 vedro-playwright-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2713 2022-11-23 14:23:16.000000 vedro-playwright-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      704 2022-11-23 14:23:30.130700 vedro-playwright-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-11-23 14:23:16.000000 vedro-playwright-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 14:23:30.130700 vedro-playwright-1.2.0/vedro_playwright/
+-rw-r--r--   0 runner    (1001) docker     (121)      596 2022-11-23 14:23:16.000000 vedro-playwright-1.2.0/vedro_playwright/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2022-11-23 14:23:16.000000 vedro-playwright-1.2.0/vedro_playwright/_browser_engine.py
+-rw-r--r--   0 runner    (1001) docker     (121)      512 2022-11-23 14:23:16.000000 vedro-playwright-1.2.0/vedro_playwright/_browser_registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1602 2022-11-23 14:23:16.000000 vedro-playwright-1.2.0/vedro_playwright/_browsers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1411 2022-11-23 14:23:16.000000 vedro-playwright-1.2.0/vedro_playwright/_screenshot_path.py
+-rw-r--r--   0 runner    (1001) docker     (121)      254 2022-11-23 14:23:16.000000 vedro-playwright-1.2.0/vedro_playwright/_screenshots_mode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6886 2022-11-23 14:23:16.000000 vedro-playwright-1.2.0/vedro_playwright/_vedro_playwright.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-23 14:23:16.000000 vedro-playwright-1.2.0/vedro_playwright/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 14:23:30.130700 vedro-playwright-1.2.0/vedro_playwright.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3266 2022-11-23 14:23:30.000000 vedro-playwright-1.2.0/vedro_playwright.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      507 2022-11-23 14:23:30.000000 vedro-playwright-1.2.0/vedro_playwright.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-23 14:23:30.000000 vedro-playwright-1.2.0/vedro_playwright.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-23 14:23:30.000000 vedro-playwright-1.2.0/vedro_playwright.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-23 14:23:30.000000 vedro-playwright-1.2.0/vedro_playwright.egg-info/top_level.txt
```

### Comparing `vedro-playwright-1.1.0/LICENSE` & `vedro-playwright-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vedro-playwright-1.1.0/PKG-INFO` & `vedro-playwright-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vedro-playwright
-Version: 1.1.0
+Version: 1.2.0
 Summary: Vedro + playwright
 Home-page: https://github.com/2gis-test-labs/vedro-playwright
 Author: 2GIS Test Labs
 Author-email: test-labs@2gis.ru
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
@@ -13,15 +13,14 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Vedro Playwright Plugin
 
-[![Codecov](https://img.shields.io/codecov/c/github/nikitanovosibirsk/vedro-playwright/master.svg?style=flat-square)](https://codecov.io/gh/nikitanovosibirsk/vedro-playwright)
 [![PyPI](https://img.shields.io/pypi/v/vedro-playwright.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-playwright/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/vedro-playwright?style=flat-square)](https://pypi.python.org/pypi/vedro-playwright/)
 [![Python Version](https://img.shields.io/pypi/pyversions/vedro-playwright.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-playwright/)
 
 [Vedro](https://vedro.io/) + [playwright](https://playwright.dev/python/)
 
 (forked from [vedro-pyppeteer](https://github.com/nikitanovosibirsk/vedro-pyppeteer))
```

### Comparing `vedro-playwright-1.1.0/README.md` & `vedro-playwright-1.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # Vedro Playwright Plugin
 
-[![Codecov](https://img.shields.io/codecov/c/github/nikitanovosibirsk/vedro-playwright/master.svg?style=flat-square)](https://codecov.io/gh/nikitanovosibirsk/vedro-playwright)
 [![PyPI](https://img.shields.io/pypi/v/vedro-playwright.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-playwright/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/vedro-playwright?style=flat-square)](https://pypi.python.org/pypi/vedro-playwright/)
 [![Python Version](https://img.shields.io/pypi/pyversions/vedro-playwright.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-playwright/)
 
 [Vedro](https://vedro.io/) + [playwright](https://playwright.dev/python/)
 
 (forked from [vedro-pyppeteer](https://github.com/nikitanovosibirsk/vedro-pyppeteer))
```

### Comparing `vedro-playwright-1.1.0/setup.cfg` & `vedro-playwright-1.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.0
+current_version = 1.2.0
 message = bump version → {new_version}
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
```

### Comparing `vedro-playwright-1.1.0/setup.py` & `vedro-playwright-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 def find_dev_required():
     with open("requirements-dev.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="vedro-playwright",
-    version="1.1.0",
+    version="1.2.0",
     description="Vedro + playwright",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="2GIS Test Labs",
     author_email="test-labs@2gis.ru",
     python_requires=">=3.8",
     url="https://github.com/2gis-test-labs/vedro-playwright",
     license="Apache-2.0",
-    packages=find_packages(exclude=("tests",)),
+    packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"vedro_playwright": ["py.typed"]},
     install_requires=find_required(),
     tests_require=find_dev_required(),
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

### Comparing `vedro-playwright-1.1.0/vedro_playwright/__init__.py` & `vedro-playwright-1.2.0/vedro_playwright/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,13 +5,13 @@
     opened_firefox,
     opened_firefox_page,
     opened_webkit,
     opened_webkit_page,
 )
 from ._vedro_playwright import Playwright, PlaywrightPlugin, opened_browser, opened_browser_page
 
-__version__ = "1.1.0"
+__version__ = "1.2.0"
 __all__ = ("Playwright", "PlaywrightPlugin", "BrowserEngine",
            "opened_browser", "opened_browser_page",
            "opened_chromium", "opened_chromium_page",
            "opened_firefox", "opened_firefox_page",
            "opened_webkit", "opened_webkit_page",)
```

### Comparing `vedro-playwright-1.1.0/vedro_playwright/_browser_registry.py` & `vedro-playwright-1.2.0/vedro_playwright/_browser_registry.py`

 * *Files identical despite different names*

### Comparing `vedro-playwright-1.1.0/vedro_playwright/_browsers.py` & `vedro-playwright-1.2.0/vedro_playwright/_browsers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Optional, cast
+from typing import Any, Dict, Optional
 
 import vedro
 from playwright.async_api import Browser, Page
 
 from ._browser_engine import BrowserEngine
 from ._vedro_playwright import opened_browser, opened_browser_page
 
@@ -12,48 +12,48 @@
 
 
 # chromium
 
 @vedro.context
 async def opened_chromium(options: Optional[Dict[str, Any]] = None) -> Browser:
     browser = await opened_browser(BrowserEngine.CHROMIUM, options)
-    return cast(Browser, browser)
+    return browser
 
 
 @vedro.context
 async def opened_chromium_page(browser: Optional[Browser] = None) -> Page:
     if browser is None:
         browser = await opened_chromium()
     page = await opened_browser_page(browser)
-    return cast(Page, page)
+    return page
 
 
 # firefox
 
 @vedro.context
 async def opened_firefox(options: Optional[Dict[str, Any]] = None) -> Browser:
     browser = await opened_browser(BrowserEngine.FIREFOX, options)
-    return cast(Browser, browser)
+    return browser
 
 
 @vedro.context
 async def opened_firefox_page(browser: Optional[Browser] = None) -> Page:
     if browser is None:
         browser = await opened_firefox()
     page = await opened_browser_page(browser)
-    return cast(Page, page)
+    return page
 
 
 # webkit
 
 @vedro.context
 async def opened_webkit(options: Optional[Dict[str, Any]] = None) -> Browser:
     browser = await opened_browser(BrowserEngine.WEBKIT, options)
-    return cast(Browser, browser)
+    return browser
 
 
 @vedro.context
 async def opened_webkit_page(browser: Optional[Browser] = None) -> Page:
     if browser is None:
         browser = await opened_webkit()
     page = await opened_browser_page(browser)
-    return cast(Page, page)
+    return page
```

### Comparing `vedro-playwright-1.1.0/vedro_playwright/_screenshot_path.py` & `vedro-playwright-1.2.0/vedro_playwright/_screenshot_path.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 __all__ = ("ScreenshotPath",)
 
 
 class ScreenshotPath:
     def __init__(self, dir_: Path) -> None:
         self.dir = dir_
-        self.rerun: Union[int, None] = None
         self.timestamp: Union[int, None] = None
         self.scenario_path: Union[Path, None] = None
         self.scenario_subject: Union[str, None] = None
         self.step_name: Union[str, None] = None
         self.tab_index: Union[int, None] = None
         self.context_index: Union[int, None] = None
 
@@ -22,17 +21,14 @@
             rel_path = self.scenario_path.relative_to(cwd)
             dir_path = self.dir.joinpath(rel_path.with_suffix(""))
 
         file_path = "screenshot"
         if self.scenario_subject is not None:
             file_path = self.scenario_subject
 
-        if self.rerun is not None:
-            file_path = f"[{self.rerun}]{file_path}"
-
         if self.timestamp is not None:
             file_path += f"__{self.timestamp}"
 
         if self.step_name is not None:
             file_path += f"__{self.step_name}"
 
         if self.tab_index is not None:
```

### Comparing `vedro-playwright-1.1.0/vedro_playwright/_vedro_playwright.py` & `vedro-playwright-1.2.0/vedro_playwright/_vedro_playwright.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,27 +48,26 @@
 
 @vedro.context
 async def opened_browser_page(browser: Optional[Browser] = None) -> Page:
     if browser is None:
         browser = await opened_browser()
 
     context: BrowserContext = await browser.new_context()
-    # context available via page.context
+    # context available via `page.context`
     page = await context.new_page()
     return page
 
 
 class PlaywrightPlugin(Plugin):
     def __init__(self, config: Type["Playwright"], *,
                  browser_registry: BrowserRegistry = _browser_registry) -> None:
         super().__init__(config)
         self._browser_registry = browser_registry
         self._mode = ScreenshotsMode.DISABLED
         self._dir = Path()
-        self._reruns = 0
         self._step_buffer: Dict[str, List[Tuple[bytes, Path]]] = {}
 
     def subscribe(self, dispatcher: Dispatcher) -> None:
         dispatcher.listen(ArgParseEvent, self.on_arg_parse) \
                   .listen(ArgParsedEvent, self.on_arg_parsed) \
                   .listen(StartupEvent, self.on_startup) \
                   .listen(ScenarioRunEvent, self.on_scenario_run) \
@@ -88,32 +87,31 @@
         help_message = f"Set directory for screenshots (default: '{default_dir}')"
         group.add_argument("--playwright-screenshots-dir",
                            default=default_dir, help=help_message)
 
     def on_arg_parsed(self, event: ArgParsedEvent) -> None:
         self._mode = event.args.playwright_screenshots
         self._dir = Path(event.args.playwright_screenshots_dir).resolve()
-        self._reruns = event.args.reruns
 
     def on_startup(self, event: StartupEvent) -> None:
         if self._mode != ScreenshotsMode.DISABLED and self._dir.exists():
             rmtree(self._dir)
 
     def on_scenario_run(self, event: ScenarioRunEvent) -> None:
         if self._mode == ScreenshotsMode.DISABLED:
             return
         self._path = ScreenshotPath(self._dir)
         self._path.scenario_path = event.scenario_result.scenario.path
         self._path.scenario_subject = event.scenario_result.scenario.subject
-        if self._reruns > 0:
-            self._path.rerun = event.scenario_result.rerun
         self._step_buffer = {}
 
-    def _save_screenshot(self,
-                         screenshot: bytes, path: Path) -> None:
+    async def _create_screenshot(self, page: Page) -> bytes:
+        return await page.screenshot()
+
+    async def _save_screenshot(self, screenshot: bytes, path: Path) -> None:
         if not path.parent.exists():
             path.parent.mkdir(parents=True)
         path.write_bytes(screenshot)
 
     def _attach_screenshot_to_step_result(self,
                                           step_result: StepResult,
                                           screenshot_path: Path,
@@ -135,32 +133,36 @@
                 self._path.step_name = event.step_result.step_name
                 if len(browser.contexts) > 1:
                     self._path.context_index = context_idx
                 if len(context.pages) > 1:
                     self._path.tab_index = page_idx
 
                 path = self._path.resolve()
-                screenshot = await page.screenshot()
                 if self._mode == ScreenshotsMode.EVERY_STEP:
-                    self._save_screenshot(screenshot, path)
+                    screenshot = await self._create_screenshot(page)
+                    await self._save_screenshot(screenshot, path)
                     self._attach_screenshot_to_step_result(event.step_result, path)
+
                 elif self._mode == ScreenshotsMode.ON_FAIL:
                     if event.step_result.step_name not in self._step_buffer:
                         self._step_buffer[event.step_result.step_name] = []
+                    screenshot = await self._create_screenshot(page)
                     self._step_buffer[event.step_result.step_name].append((screenshot, path))
+
                 elif (self._mode == ScreenshotsMode.ONLY_FAILED) and event.step_result.is_failed():
-                    self._save_screenshot(screenshot, path)
+                    screenshot = await self._create_screenshot(page)
+                    await self._save_screenshot(screenshot, path)
                     self._attach_screenshot_to_step_result(event.step_result, path)
 
     async def on_scenario_failed(self, event: ScenarioFailedEvent) -> None:
         for step_result in event.scenario_result.step_results:
             if step_result.step_name not in self._step_buffer:
                 continue
             screenshots = self._step_buffer[step_result.step_name]
             while len(screenshots) > 0:
                 screenshot, path = screenshots.pop(0)
-                self._save_screenshot(screenshot, path)
+                await self._save_screenshot(screenshot, path)
                 self._attach_screenshot_to_step_result(step_result, path)
 
 
 class Playwright(PluginConfig):
     plugin = PlaywrightPlugin
```

### Comparing `vedro-playwright-1.1.0/vedro_playwright.egg-info/PKG-INFO` & `vedro-playwright-1.2.0/vedro_playwright.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vedro-playwright
-Version: 1.1.0
+Version: 1.2.0
 Summary: Vedro + playwright
 Home-page: https://github.com/2gis-test-labs/vedro-playwright
 Author: 2GIS Test Labs
 Author-email: test-labs@2gis.ru
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
@@ -13,15 +13,14 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Vedro Playwright Plugin
 
-[![Codecov](https://img.shields.io/codecov/c/github/nikitanovosibirsk/vedro-playwright/master.svg?style=flat-square)](https://codecov.io/gh/nikitanovosibirsk/vedro-playwright)
 [![PyPI](https://img.shields.io/pypi/v/vedro-playwright.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-playwright/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/vedro-playwright?style=flat-square)](https://pypi.python.org/pypi/vedro-playwright/)
 [![Python Version](https://img.shields.io/pypi/pyversions/vedro-playwright.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-playwright/)
 
 [Vedro](https://vedro.io/) + [playwright](https://playwright.dev/python/)
 
 (forked from [vedro-pyppeteer](https://github.com/nikitanovosibirsk/vedro-pyppeteer))
```

