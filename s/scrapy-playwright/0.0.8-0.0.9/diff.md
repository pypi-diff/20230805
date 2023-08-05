# Comparing `tmp/scrapy-playwright-0.0.8.tar.gz` & `tmp/scrapy-playwright-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy-playwright-0.0.8.tar", last modified: Thu Jan 13 23:04:28 2022, max compression
+gzip compressed data, was "scrapy-playwright-0.0.9.tar", last modified: Thu Jan 27 16:26:16 2022, max compression
```

## Comparing `scrapy-playwright-0.0.8.tar` & `scrapy-playwright-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 23:04:28.410819 scrapy-playwright-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1461 2022-01-13 23:04:19.000000 scrapy-playwright-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    14594 2022-01-13 23:04:28.410819 scrapy-playwright-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13654 2022-01-13 23:04:19.000000 scrapy-playwright-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-01-13 23:04:19.000000 scrapy-playwright-0.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 23:04:28.410819 scrapy-playwright-0.0.8/scrapy_playwright/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-01-13 23:04:19.000000 scrapy-playwright-0.0.8/scrapy_playwright/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11735 2022-01-13 23:04:19.000000 scrapy-playwright-0.0.8/scrapy_playwright/handler.py
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-01-13 23:04:19.000000 scrapy-playwright-0.0.8/scrapy_playwright/page.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 23:04:28.410819 scrapy-playwright-0.0.8/scrapy_playwright.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14594 2022-01-13 23:04:28.000000 scrapy-playwright-0.0.8/scrapy_playwright.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-01-13 23:04:28.000000 scrapy-playwright-0.0.8/scrapy_playwright.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-13 23:04:28.000000 scrapy-playwright-0.0.8/scrapy_playwright.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-01-13 23:04:28.000000 scrapy-playwright-0.0.8/scrapy_playwright.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-01-13 23:04:28.000000 scrapy-playwright-0.0.8/scrapy_playwright.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-01-13 23:04:28.410819 scrapy-playwright-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1263 2022-01-13 23:04:19.000000 scrapy-playwright-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 16:26:16.110779 scrapy-playwright-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1461 2022-01-27 16:25:57.000000 scrapy-playwright-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    16098 2022-01-27 16:26:16.110779 scrapy-playwright-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    15158 2022-01-27 16:25:57.000000 scrapy-playwright-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-01-27 16:25:57.000000 scrapy-playwright-0.0.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 16:26:16.110779 scrapy-playwright-0.0.9/scrapy_playwright/
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-01-27 16:25:57.000000 scrapy-playwright-0.0.9/scrapy_playwright/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11844 2022-01-27 16:25:57.000000 scrapy-playwright-0.0.9/scrapy_playwright/handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1529 2022-01-27 16:25:57.000000 scrapy-playwright-0.0.9/scrapy_playwright/headers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      448 2022-01-27 16:25:57.000000 scrapy-playwright-0.0.9/scrapy_playwright/page.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 16:26:16.110779 scrapy-playwright-0.0.9/scrapy_playwright.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    16098 2022-01-27 16:26:16.000000 scrapy-playwright-0.0.9/scrapy_playwright.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2022-01-27 16:26:16.000000 scrapy-playwright-0.0.9/scrapy_playwright.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-27 16:26:16.000000 scrapy-playwright-0.0.9/scrapy_playwright.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2022-01-27 16:26:16.000000 scrapy-playwright-0.0.9/scrapy_playwright.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-01-27 16:26:16.000000 scrapy-playwright-0.0.9/scrapy_playwright.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-01-27 16:26:16.114779 scrapy-playwright-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1263 2022-01-27 16:25:57.000000 scrapy-playwright-0.0.9/setup.py
```

### Comparing `scrapy-playwright-0.0.8/LICENSE` & `scrapy-playwright-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapy-playwright-0.0.8/PKG-INFO` & `scrapy-playwright-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-playwright
-Version: 0.0.8
+Version: 0.0.9
 Summary: Playwright integration for Scrapy
 Home-page: https://github.com/scrapy-plugins/scrapy-playwright
 Author: Eugenio Lacuesta
 Author-email: eugenio.lacuesta@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -123,14 +123,33 @@
 
 * `PLAYWRIGHT_DEFAULT_NAVIGATION_TIMEOUT` (type `Optional[float]`, default `None`)
 
     The timeout used when requesting pages by Playwright. If `None` or unset,
     the default value will be used (30000 ms at the time of writing this).
     See the docs for [BrowserContext.set_default_navigation_timeout](https://playwright.dev/python/docs/api/class-browsercontext#browser_contextset_default_navigation_timeouttimeout).
 
+* `PLAYWRIGHT_PROCESS_REQUEST_HEADERS` (type `str`, default `scrapy_playwright.headers.use_scrapy_headers`)
+
+    The path to a coroutine function (`async def`) that processes headers for a given request
+    and returns a dictionary with the headers to be used (note that, depending on the browser,
+    additional default headers will be sent as well).
+
+    The function must return a `dict` object, and receives the following keyword arguments:
+
+    ```python
+    browser_type: str, playwright_request: playwright.async_api.Request, scrapy_headers: scrapy.http.headers.Headers
+    ```
+
+    The default value (`scrapy_playwright.headers.use_scrapy_headers`) tries to emulate Scrapy's
+    behaviour for navigation requests, i.e. overriding headers with their values from the Scrapy request.
+    For non-navigation requests (e.g. images, stylesheets, scripts, etc), only the `User-Agent` header
+    is overriden, for consistency.
+
+    There is nother function available: `scrapy_playwright.headers.use_playwright_headers`,
+    which will return the headers from the Playwright request without any changes.
 
 ## Basic usage
 
 Set the `playwright` [Request.meta](https://docs.scrapy.org/en/latest/topics/request-response.html#scrapy.http.Request.meta)
 key to download a request using Playwright:
 
 ```python
@@ -155,16 +174,16 @@
 ```
 
 ### Notes about the User-Agent header
 
 By default, outgoing requests include the `User-Agent` set by Scrapy (either with the
 `USER_AGENT` or `DEFAULT_REQUEST_HEADERS` settings or via the `Request.headers` attribute).
 This could cause some sites to react in unexpected ways, for instance if the user agent
-does not match the Browser being used. If you prefer to send the `User-Agent` from the Browser,
-set the Scrapy user agent to `None`.
+does not match the running Browser. If you prefer the `User-Agent` sent by
+default by the specific browser you're using, set the Scrapy user agent to `None`.
 
 
 ## Receiving the Page object in the callback
 
 Specifying a non-False value for the `playwright_include_page` `meta` key for a
 request will result in the corresponding `playwright.async_api.Page` object
 being available in the `playwright_page` meta key in the request callback.
@@ -401,7 +420,16 @@
         return {"quote_count": len(response.css("div.quote"))}  # quotes from several pages
 ```
 
 
 For more examples, please see the scripts in the [examples](examples) directory.
 
 
+## Known limitations
+
+* Currently, `scrapy-plawright` does not work natively on Windows. See
+  [this comment](https://github.com/scrapy-plugins/scrapy-playwright/issues/7#issuecomment-808824121)
+  for more infomation. Additionally, please see
+  [this comment](https://github.com/scrapy-plugins/scrapy-playwright/issues/7#issuecomment-817394494)
+  for a possible workaround.
+
+
```

### Comparing `scrapy-playwright-0.0.8/README.md` & `scrapy-playwright-0.0.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -99,14 +99,33 @@
 
 * `PLAYWRIGHT_DEFAULT_NAVIGATION_TIMEOUT` (type `Optional[float]`, default `None`)
 
     The timeout used when requesting pages by Playwright. If `None` or unset,
     the default value will be used (30000 ms at the time of writing this).
     See the docs for [BrowserContext.set_default_navigation_timeout](https://playwright.dev/python/docs/api/class-browsercontext#browser_contextset_default_navigation_timeouttimeout).
 
+* `PLAYWRIGHT_PROCESS_REQUEST_HEADERS` (type `str`, default `scrapy_playwright.headers.use_scrapy_headers`)
+
+    The path to a coroutine function (`async def`) that processes headers for a given request
+    and returns a dictionary with the headers to be used (note that, depending on the browser,
+    additional default headers will be sent as well).
+
+    The function must return a `dict` object, and receives the following keyword arguments:
+
+    ```python
+    browser_type: str, playwright_request: playwright.async_api.Request, scrapy_headers: scrapy.http.headers.Headers
+    ```
+
+    The default value (`scrapy_playwright.headers.use_scrapy_headers`) tries to emulate Scrapy's
+    behaviour for navigation requests, i.e. overriding headers with their values from the Scrapy request.
+    For non-navigation requests (e.g. images, stylesheets, scripts, etc), only the `User-Agent` header
+    is overriden, for consistency.
+
+    There is nother function available: `scrapy_playwright.headers.use_playwright_headers`,
+    which will return the headers from the Playwright request without any changes.
 
 ## Basic usage
 
 Set the `playwright` [Request.meta](https://docs.scrapy.org/en/latest/topics/request-response.html#scrapy.http.Request.meta)
 key to download a request using Playwright:
 
 ```python
@@ -131,16 +150,16 @@
 ```
 
 ### Notes about the User-Agent header
 
 By default, outgoing requests include the `User-Agent` set by Scrapy (either with the
 `USER_AGENT` or `DEFAULT_REQUEST_HEADERS` settings or via the `Request.headers` attribute).
 This could cause some sites to react in unexpected ways, for instance if the user agent
-does not match the Browser being used. If you prefer to send the `User-Agent` from the Browser,
-set the Scrapy user agent to `None`.
+does not match the running Browser. If you prefer the `User-Agent` sent by
+default by the specific browser you're using, set the Scrapy user agent to `None`.
 
 
 ## Receiving the Page object in the callback
 
 Specifying a non-False value for the `playwright_include_page` `meta` key for a
 request will result in the corresponding `playwright.async_api.Page` object
 being available in the `playwright_page` meta key in the request callback.
@@ -375,7 +394,16 @@
         await page.screenshot(path="quotes.png", fullPage=True)
         await page.close()
         return {"quote_count": len(response.css("div.quote"))}  # quotes from several pages
 ```
 
 
 For more examples, please see the scripts in the [examples](examples) directory.
+
+
+## Known limitations
+
+* Currently, `scrapy-plawright` does not work natively on Windows. See
+  [this comment](https://github.com/scrapy-plugins/scrapy-playwright/issues/7#issuecomment-808824121)
+  for more infomation. Additionally, please see
+  [this comment](https://github.com/scrapy-plugins/scrapy-playwright/issues/7#issuecomment-817394494)
+  for a possible workaround.
```

### Comparing `scrapy-playwright-0.0.8/scrapy_playwright/handler.py` & `scrapy-playwright-0.0.9/scrapy_playwright/handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import asyncio
 import logging
 import warnings
 from collections import defaultdict
 from contextlib import suppress
 from time import time
 from typing import Callable, Dict, Optional, Type, TypeVar
-from urllib.parse import urlparse
 
 from playwright.async_api import (
     BrowserContext,
     Page,
     PlaywrightContextManager,
     Request as PlaywrightRequest,
     Response as PlaywrightResponse,
@@ -18,17 +17,19 @@
 from scrapy import Spider, signals
 from scrapy.core.downloader.handlers.http import HTTPDownloadHandler
 from scrapy.crawler import Crawler
 from scrapy.http import Request, Response
 from scrapy.http.headers import Headers
 from scrapy.responsetypes import responsetypes
 from scrapy.utils.defer import deferred_from_coro
+from scrapy.utils.misc import load_object
 from scrapy.utils.reactor import verify_installed_reactor
 from twisted.internet.defer import Deferred, inlineCallbacks
 
+from scrapy_playwright.headers import use_scrapy_headers
 from scrapy_playwright.page import PageCoroutine
 
 
 __all__ = ["ScrapyPlaywrightDownloadHandler"]
 
 
 PlaywrightHandler = TypeVar("PlaywrightHandler", bound="ScrapyPlaywrightDownloadHandler")
@@ -62,21 +63,29 @@
         super().__init__(settings=crawler.settings, crawler=crawler)
         verify_installed_reactor("twisted.internet.asyncioreactor.AsyncioSelectorReactor")
         crawler.signals.connect(self._engine_started, signals.engine_started)
         self.stats = crawler.stats
 
         self.browser_type: str = crawler.settings.get("PLAYWRIGHT_BROWSER_TYPE") or "chromium"
         self.launch_options: dict = crawler.settings.getdict("PLAYWRIGHT_LAUNCH_OPTIONS") or {}
+
         self.default_navigation_timeout: Optional[float] = None
         if "PLAYWRIGHT_DEFAULT_NAVIGATION_TIMEOUT" in crawler.settings:
             with suppress(TypeError, ValueError):
                 self.default_navigation_timeout = float(
                     crawler.settings.get("PLAYWRIGHT_DEFAULT_NAVIGATION_TIMEOUT")
                 )
 
+        if crawler.settings.get("PLAYWRIGHT_PROCESS_REQUEST_HEADERS"):
+            self.process_request_headers = load_object(
+                crawler.settings["PLAYWRIGHT_PROCESS_REQUEST_HEADERS"]
+            )
+        else:
+            self.process_request_headers = use_scrapy_headers
+
         default_context_kwargs: dict = {}
         if "PLAYWRIGHT_CONTEXT_ARGS" in crawler.settings:
             default_context_kwargs = crawler.settings.getdict("PLAYWRIGHT_CONTEXT_ARGS")
             warnings.warn(
                 "The PLAYWRIGHT_CONTEXT_ARGS setting is deprecated, please use"
                 " PLAYWRIGHT_CONTEXTS instead. Keyword arguments defined in"
                 " PLAYWRIGHT_CONTEXT_ARGS will be used when creating the 'default' context",
@@ -176,17 +185,16 @@
                         f" ignoring handler for event '{event}'"
                     )
 
         await page.unroute("**")
         await page.route(
             "**",
             self._make_request_handler(
-                url=request.url,
                 method=request.method,
-                headers=request.headers.to_unicode_dict(),
+                scrapy_headers=request.headers,
                 body=request.body,
                 encoding=getattr(request, "encoding", None),
             ),
         )
 
         try:
             result = await self._download_request_with_page(request, page)
@@ -245,27 +253,28 @@
             logger.debug("Browser context closed: '%s'", name)
             if name in self.contexts:
                 self.contexts.pop(name)
 
         return close_browser_context_callback
 
     def _make_request_handler(
-        self, url: str, method: str, headers: dict, body: Optional[bytes], encoding: str = "utf8"
+        self, method: str, scrapy_headers: Headers, body: Optional[bytes], encoding: str = "utf8"
     ) -> Callable:
-        def request_handler(route: Route, pw_request: PlaywrightRequest) -> None:
+        async def _request_handler(route: Route, playwright_request: PlaywrightRequest) -> None:
             """Override request headers, method and body."""
-            headers.setdefault("user-agent", pw_request.headers.get("user-agent"))
-            if pw_request.url == url:
-                overrides: dict = {"method": method, "headers": headers}
+            processed_headers = await self.process_request_headers(
+                self.browser_type, playwright_request, scrapy_headers
+            )
+
+            # the request that reaches the callback should contain the headers that were sent
+            scrapy_headers.clear()
+            scrapy_headers.update(processed_headers)
+
+            overrides: dict = {"headers": processed_headers}
+            if playwright_request.is_navigation_request():
+                overrides["method"] = method
                 if body is not None:
                     overrides["post_data"] = body.decode(encoding)
-                if self.browser_type == "firefox":
-                    # otherwise this fails with playwright.helper.Error: NS_ERROR_NET_RESET
-                    overrides["headers"]["host"] = urlparse(pw_request.url).netloc
-            else:
-                overrides = {"headers": pw_request.headers.copy()}
-                # override user agent, for consistency with other requests
-                if headers.get("user-agent"):
-                    overrides["headers"]["user-agent"] = headers["user-agent"]
-            asyncio.create_task(route.continue_(**overrides))
 
-        return request_handler
+            await route.continue_(**overrides)
+
+        return _request_handler
```

### Comparing `scrapy-playwright-0.0.8/scrapy_playwright.egg-info/PKG-INFO` & `scrapy-playwright-0.0.9/scrapy_playwright.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-playwright
-Version: 0.0.8
+Version: 0.0.9
 Summary: Playwright integration for Scrapy
 Home-page: https://github.com/scrapy-plugins/scrapy-playwright
 Author: Eugenio Lacuesta
 Author-email: eugenio.lacuesta@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -123,14 +123,33 @@
 
 * `PLAYWRIGHT_DEFAULT_NAVIGATION_TIMEOUT` (type `Optional[float]`, default `None`)
 
     The timeout used when requesting pages by Playwright. If `None` or unset,
     the default value will be used (30000 ms at the time of writing this).
     See the docs for [BrowserContext.set_default_navigation_timeout](https://playwright.dev/python/docs/api/class-browsercontext#browser_contextset_default_navigation_timeouttimeout).
 
+* `PLAYWRIGHT_PROCESS_REQUEST_HEADERS` (type `str`, default `scrapy_playwright.headers.use_scrapy_headers`)
+
+    The path to a coroutine function (`async def`) that processes headers for a given request
+    and returns a dictionary with the headers to be used (note that, depending on the browser,
+    additional default headers will be sent as well).
+
+    The function must return a `dict` object, and receives the following keyword arguments:
+
+    ```python
+    browser_type: str, playwright_request: playwright.async_api.Request, scrapy_headers: scrapy.http.headers.Headers
+    ```
+
+    The default value (`scrapy_playwright.headers.use_scrapy_headers`) tries to emulate Scrapy's
+    behaviour for navigation requests, i.e. overriding headers with their values from the Scrapy request.
+    For non-navigation requests (e.g. images, stylesheets, scripts, etc), only the `User-Agent` header
+    is overriden, for consistency.
+
+    There is nother function available: `scrapy_playwright.headers.use_playwright_headers`,
+    which will return the headers from the Playwright request without any changes.
 
 ## Basic usage
 
 Set the `playwright` [Request.meta](https://docs.scrapy.org/en/latest/topics/request-response.html#scrapy.http.Request.meta)
 key to download a request using Playwright:
 
 ```python
@@ -155,16 +174,16 @@
 ```
 
 ### Notes about the User-Agent header
 
 By default, outgoing requests include the `User-Agent` set by Scrapy (either with the
 `USER_AGENT` or `DEFAULT_REQUEST_HEADERS` settings or via the `Request.headers` attribute).
 This could cause some sites to react in unexpected ways, for instance if the user agent
-does not match the Browser being used. If you prefer to send the `User-Agent` from the Browser,
-set the Scrapy user agent to `None`.
+does not match the running Browser. If you prefer the `User-Agent` sent by
+default by the specific browser you're using, set the Scrapy user agent to `None`.
 
 
 ## Receiving the Page object in the callback
 
 Specifying a non-False value for the `playwright_include_page` `meta` key for a
 request will result in the corresponding `playwright.async_api.Page` object
 being available in the `playwright_page` meta key in the request callback.
@@ -401,7 +420,16 @@
         return {"quote_count": len(response.css("div.quote"))}  # quotes from several pages
 ```
 
 
 For more examples, please see the scripts in the [examples](examples) directory.
 
 
+## Known limitations
+
+* Currently, `scrapy-plawright` does not work natively on Windows. See
+  [this comment](https://github.com/scrapy-plugins/scrapy-playwright/issues/7#issuecomment-808824121)
+  for more infomation. Additionally, please see
+  [this comment](https://github.com/scrapy-plugins/scrapy-playwright/issues/7#issuecomment-817394494)
+  for a possible workaround.
+
+
```

### Comparing `scrapy-playwright-0.0.8/setup.py` & `scrapy-playwright-0.0.9/setup.py`

 * *Files identical despite different names*

