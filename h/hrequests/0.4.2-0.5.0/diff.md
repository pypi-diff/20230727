# Comparing `tmp/hrequests-0.4.2.tar.gz` & `tmp/hrequests-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hrequests-0.4.2.tar", max compression
+gzip compressed data, was "hrequests-0.5.0.tar", max compression
```

## Comparing `hrequests-0.4.2.tar` & `hrequests-0.5.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0      327 2023-07-08 02:07:11.571269 hrequests-0.4.2/hrequests/__init__.py
--rw-r--r--   0        0        0      143 2023-07-16 09:31:33.373549 hrequests-0.4.2/hrequests/__version__.py
--rw-r--r--   0        0        0        0 2023-07-02 20:20:07.221972 hrequests-0.4.2/hrequests/bin/__init__.py
--rw-r--r--   0        0        0     1688 2023-07-02 20:40:17.715874 hrequests-0.4.2/hrequests/bin/LICENSE.txt
--rw-r--r--   0        0        0    23808 2023-07-16 05:24:15.767500 hrequests-0.4.2/hrequests/browser.py
--rw-r--r--   0        0        0     2771 2023-07-07 18:22:10.146220 hrequests-0.4.2/hrequests/cffi.py
--rw-r--r--   0        0        0    13695 2023-07-16 05:38:20.704288 hrequests-0.4.2/hrequests/client.py
--rw-r--r--   0        0        0    16415 2023-07-07 01:06:32.804013 hrequests-0.4.2/hrequests/cookies.py
--rw-r--r--   0        0        0      723 2023-07-09 08:14:06.945274 hrequests-0.4.2/hrequests/exceptions.py
--rw-r--r--   0        0        0    19506 2023-07-16 09:26:40.532017 hrequests-0.4.2/hrequests/parser.py
--rw-r--r--   0        0        0      374 2023-07-08 02:07:11.641927 hrequests-0.4.2/hrequests/playwright_mock/__init__.py
--rw-r--r--   0        0        0     1163 2023-06-23 03:19:47.973633 hrequests-0.4.2/hrequests/playwright_mock/context.py
--rw-r--r--   0        0        0    12246 2023-07-07 18:42:04.730618 hrequests-0.4.2/hrequests/playwright_mock/element_handle.py
--rw-r--r--   0        0        0     2208 2023-07-08 02:07:11.715693 hrequests-0.4.2/hrequests/playwright_mock/faker.py
--rw-r--r--   0        0        0    16099 2023-07-08 02:07:11.935959 hrequests-0.4.2/hrequests/playwright_mock/frame.py
--rw-r--r--   0        0        0     1579 2023-06-17 22:56:39.629341 hrequests-0.4.2/hrequests/playwright_mock/frame_locator.py
--rw-r--r--   0        0        0      354 2023-06-17 22:56:39.629341 hrequests-0.4.2/hrequests/playwright_mock/js_handle.py
--rw-r--r--   0        0        0     6919 2023-06-18 03:47:56.370585 hrequests-0.4.2/hrequests/playwright_mock/locale.json
--rw-r--r--   0        0        0    12140 2023-06-18 03:49:17.047181 hrequests-0.4.2/hrequests/playwright_mock/locator.py
--rw-r--r--   0        0        0     3454 2023-06-17 23:01:35.605590 hrequests-0.4.2/hrequests/playwright_mock/mouse.py
--rw-r--r--   0        0        0    17529 2023-07-16 04:06:21.948435 hrequests-0.4.2/hrequests/playwright_mock/page.py
--rw-r--r--   0        0        0     1823 2023-07-08 02:07:11.739522 hrequests-0.4.2/hrequests/playwright_mock/playwright_mock.py
--rw-r--r--   0        0        0     3910 2023-07-08 02:07:11.800614 hrequests-0.4.2/hrequests/playwright_mock/proxy_manager.py
--rw-r--r--   0        0        0    13769 2023-07-20 02:12:07.392826 hrequests-0.4.2/hrequests/reqs.py
--rw-r--r--   0        0        0     8576 2023-07-20 02:10:18.786226 hrequests-0.4.2/hrequests/response.py
--rw-r--r--   0        0        0    11917 2023-07-12 07:00:19.769672 hrequests-0.4.2/hrequests/session.py
--rw-r--r--   0        0        0     4715 2023-07-11 01:15:09.826071 hrequests-0.4.2/hrequests/toolbelt.py
--rw-r--r--   0        0        0    11357 2023-07-06 18:41:32.923322 hrequests-0.4.2/LICENSE
--rw-r--r--   0        0        0     1022 2023-07-16 09:31:45.416726 hrequests-0.4.2/pyproject.toml
--rw-r--r--   0        0        0    33032 2023-07-16 09:29:15.958671 hrequests-0.4.2/README.md
--rw-r--r--   0        0        0    33452 1970-01-01 00:00:00.000000 hrequests-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      327 2023-07-08 02:07:11.571269 hrequests-0.5.0/hrequests/__init__.py
+-rw-r--r--   0        0        0      143 2023-07-27 05:36:46.339796 hrequests-0.5.0/hrequests/__version__.py
+-rw-r--r--   0        0        0        0 2023-07-02 20:20:07.221972 hrequests-0.5.0/hrequests/bin/__init__.py
+-rw-r--r--   0        0        0     1688 2023-07-02 20:40:17.715874 hrequests-0.5.0/hrequests/bin/LICENSE.txt
+-rw-r--r--   0        0        0    24019 2023-07-27 04:11:05.106287 hrequests-0.5.0/hrequests/browser.py
+-rw-r--r--   0        0        0     2766 2023-07-27 05:28:27.582549 hrequests-0.5.0/hrequests/cffi.py
+-rw-r--r--   0        0        0    13695 2023-07-16 05:38:20.704288 hrequests-0.5.0/hrequests/client.py
+-rw-r--r--   0        0        0    16943 2023-07-27 04:00:00.788929 hrequests-0.5.0/hrequests/cookies.py
+-rw-r--r--   0        0        0      832 2023-07-26 03:24:32.884562 hrequests-0.5.0/hrequests/exceptions.py
+-rw-r--r--   0        0        0     3521 2023-07-26 02:48:16.215913 hrequests-0.5.0/hrequests/extensions.py
+-rw-r--r--   0        0        0    19506 2023-07-16 09:26:40.532017 hrequests-0.5.0/hrequests/parser.py
+-rw-r--r--   0        0        0      374 2023-07-08 02:07:11.641927 hrequests-0.5.0/hrequests/playwright_mock/__init__.py
+-rw-r--r--   0        0        0     1163 2023-07-26 16:42:30.741872 hrequests-0.5.0/hrequests/playwright_mock/context.py
+-rw-r--r--   0        0        0    12246 2023-07-07 18:42:04.730618 hrequests-0.5.0/hrequests/playwright_mock/element_handle.py
+-rw-r--r--   0        0        0     2208 2023-07-08 02:07:11.715693 hrequests-0.5.0/hrequests/playwright_mock/faker.py
+-rw-r--r--   0        0        0    16099 2023-07-08 02:07:11.935959 hrequests-0.5.0/hrequests/playwright_mock/frame.py
+-rw-r--r--   0        0        0     1579 2023-06-17 22:56:39.629341 hrequests-0.5.0/hrequests/playwright_mock/frame_locator.py
+-rw-r--r--   0        0        0      354 2023-06-17 22:56:39.629341 hrequests-0.5.0/hrequests/playwright_mock/js_handle.py
+-rw-r--r--   0        0        0     6919 2023-06-18 03:47:56.370585 hrequests-0.5.0/hrequests/playwright_mock/locale.json
+-rw-r--r--   0        0        0    12140 2023-06-18 03:49:17.047181 hrequests-0.5.0/hrequests/playwright_mock/locator.py
+-rw-r--r--   0        0        0     3454 2023-06-17 23:01:35.605590 hrequests-0.5.0/hrequests/playwright_mock/mouse.py
+-rw-r--r--   0        0        0    17529 2023-07-16 04:06:21.948435 hrequests-0.5.0/hrequests/playwright_mock/page.py
+-rw-r--r--   0        0        0     2226 2023-07-27 03:05:33.657481 hrequests-0.5.0/hrequests/playwright_mock/playwright_mock.py
+-rw-r--r--   0        0        0     3910 2023-07-08 02:07:11.800614 hrequests-0.5.0/hrequests/playwright_mock/proxy_manager.py
+-rw-r--r--   0        0        0    13769 2023-07-20 02:12:07.392826 hrequests-0.5.0/hrequests/reqs.py
+-rw-r--r--   0        0        0     8645 2023-07-27 03:19:59.329126 hrequests-0.5.0/hrequests/response.py
+-rw-r--r--   0        0        0    11917 2023-07-12 07:00:19.769672 hrequests-0.5.0/hrequests/session.py
+-rw-r--r--   0        0        0     4715 2023-07-26 07:07:38.574046 hrequests-0.5.0/hrequests/toolbelt.py
+-rw-r--r--   0        0        0    11357 2023-07-06 18:41:32.923322 hrequests-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1062 2023-07-27 05:36:54.131069 hrequests-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    35059 2023-07-27 05:38:31.115281 hrequests-0.5.0/README.md
+-rw-r--r--   0        0        0    35450 1970-01-01 00:00:00.000000 hrequests-0.5.0/PKG-INFO
```

### Comparing `hrequests-0.4.2/hrequests/bin/LICENSE.txt` & `hrequests-0.5.0/hrequests/bin/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.2/hrequests/browser.py` & `hrequests-0.5.0/hrequests/browser.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 import asyncio
+import os
 from functools import partial
 from random import choice
 from threading import Thread
-from typing import Any, Callable, Dict, Literal, Optional, Pattern, Union, List
+from typing import Any, Callable, Dict, Iterable, List, Literal, Optional, Pattern, Union
 
 from aioprocessing import Queue
 from fake_headers import Headers
 from playwright._impl._api_types import Error as PlaywrightError
 from playwright._impl._api_types import TimeoutError as PlaywrightTimeoutError
 
 import hrequests
 from hrequests.client import CaseInsensitiveDict
 from hrequests.cookies import cookiejar_to_list, list_to_cookiejar
-from hrequests.exceptions import BrowserException, BrowserTimeoutException
+from hrequests.exceptions import BrowserException, BrowserTimeoutException, JavascriptException
 from hrequests.response import Response
 
 from .cookies import RequestsCookieJar
+from .extensions import BuildExtensions, Extension, activate_exts
 
 
 class BrowserSession:
     """
     Args:
         headless (bool, optional): Whether to run the browser in headless mode. Defaults to True.
         session (hrequests.session.TLSSession, optional): Session to use for headers, cookies, etc.
         resp (hrequests.response.Response, optional): Response to update with cookies, headers, etc.
         proxy_ip (str, optional): Proxy to use for the browser. Example: 123.123.123
         mock_human (bool, optional): Whether to emulate human behavior. Defaults to False.
-        allow_styling (bool, optional): Allow loading images, fonts, styles, etc. Defaults to True
         browser (Literal['firefox', 'chrome', 'opera'], optional): Generate useragent headers for a specific browser
         os (Literal['win', 'mac', 'lin'], optional): Generate headers for a specific OS
+        extensions (Union[str, Iterable[str]], optional): Path to a folder of unpacked extensions, or a list of paths to unpacked extensions
 
     Attributes:
         url (str): Get the page url
         headers (dict): Get the browser headers (User-Agent)
         content (dict): Get the current page content
         cookies (RequestsCookieJar): Get the browser cookies
 
@@ -69,17 +71,17 @@
         self,
         *,
         headless: bool = True,
         session: Optional[hrequests.session.TLSSession] = None,
         resp: Optional[hrequests.response.Response] = None,
         proxy_ip: Optional[str] = None,
         mock_human: bool = False,
-        allow_styling: bool = True,
         browser: Optional[Literal['firefox', 'chrome', 'opera']] = None,
         os: Optional[Literal['win', 'mac', 'lin']] = None,
+        extensions: Optional[Union[str, Iterable[str]]] = None,
     ) -> None:
         # uses asyncio queues to communicate with the asyncio loop from any thread
         # _in is for calls from other threads
         self._in: Queue = Queue()
         # _out is for responses from the asyncio loop
         self._out: Queue = Queue()
         # remember session and resp to clone cookies back to when closing
@@ -96,68 +98,66 @@
             self.browser: str = browser or choice(('firefox', 'chrome', 'opera'))
             self.ua: str = Headers(browser=self.browser, os=os).generate()['User-Agent']
         # proxy variables
         self.proxy_ip: Optional[str] = proxy_ip
         # browser config
         self.mock_human: bool = mock_human
         self.headless: bool = headless
+        self.extensions: Optional[List[Extension]] = (
+            BuildExtensions(extensions).list if extensions else None
+        )
         # bool to indicate browser was closed
         self._closed: bool = False
-        # boolean to disable loading images, fonts, styles, etc
-        self.allow_styling: bool = allow_styling
         # spawn asyncio loop
         thread: Thread = Thread(target=self.spawn_main, daemon=True)
         thread.start()
 
     def spawn_main(self) -> None:
         asyncio.new_event_loop().run_until_complete(self.main())
 
     async def main(self) -> None:
         # build the playwright instance
-        self.client = await hrequests.PlaywrightMock(headless=self.headless)
+        self.client = await hrequests.PlaywrightMock(
+            headless=self.headless, extensions=self.extensions
+        )
         self.context = await self.client.new_context(
             browser_name=self.browser,
             user_agent=self.ua,
             proxy=self.proxy_ip,
             mock_human=self.mock_human,
         )
         # create a new page
         self.page = await self.context.new_page()
-        # route all requests through handle_request to kill unnessecary requests
-        await self.page.route("**/*", self.handle_request)
-        # run the main loop:
-        # 1. listen for calls to _in
-        # 2. handle the call within the asyncio loop
-        # 3. put the call response in _out.
-        # this is used as a work around to make playwright work across threads
+        # activate extensions
+        if self.extensions:
+            await activate_exts(self.page, self.extensions)
+        '''
+        run the main loop
+        '''
         while True:
             try:
+                # listen for calls to _in
                 call: partial = self._in.get()
+                # handle the call within the asyncio loop
+                # this is used as a workaround to make playwright work across threads
                 out = await call()
             except PlaywrightTimeoutError as e:
+                # if a timeout error is raised, mark as closed and put the error in _out
                 self._closed = True
                 self._out.put(BrowserTimeoutException(e))
             except PlaywrightError as e:
+                # if a playwright error is raised, mark as closed and put the error in _out
                 self._closed = True
                 self._out.put(BrowserException(e))
             except BrowserException as e:
                 self._out.put(e)
             else:
+                # put the call response in _out
                 self._out.put(out)
 
-    # unnessecary resource requests to kill
-    _excluded_resources = {'font', 'image', 'stylesheet', 'media'}
-
-    async def handle_request(self, route) -> None:
-        # kill unnessecary requests
-        if not self.allow_styling and route.request.resource_type in self._excluded_resources:
-            await route.abort()
-        else:
-            await route.continue_()
-
     async def shutdown(self) -> None:
         self._closed = True
         await self.client.stop()
 
     def __enter__(self) -> 'BrowserSession':
         return self
 
@@ -173,15 +173,15 @@
         if isinstance(out, Exception):
             raise out
         return out
 
     def __getattr__(self, name) -> Any:
         # sourcery skip: raise-from-previous-error
         if self._closed:
-            raise BrowserException('Browser was closed. Attribute call failed: ' + name)
+            raise BrowserException(f'Browser was closed. Attribute call failed: {name}')
         # forwards unknown attribute calls to _call_wrapper
         try:
             # check if the attribute (with a leading _) exists
             attr = self.__getattribute__(f'_{name}')
         except AttributeError:
             # if it doesnt, raise an error
             raise AttributeError(
@@ -231,29 +231,29 @@
         '''
         Wait for a selector to exist
 
         Parameters:
             selector (str): Selector to wait for
             timeout (float, optional): Timeout in seconds. Defaults to 30.
         '''
-        return await self.page.wait_for_function(
+        await self.page.wait_for_function(
             "selector => !!document.querySelector(selector)",
             arg=selector,
             timeout=int(timeout * 1e3),
         )
 
     async def _awaitEnabled(self, selector, *, timeout: float = 30):
         '''
         Wait for a selector to be enabled
 
         Parameters:
             selector (str): Selector to wait for
             timeout (float, optional): Timeout in seconds. Defaults to 30.
         '''
-        return await self.page.wait_for_function(
+        await self.page.wait_for_function(
             "selector => !document.querySelector(selector).disabled",
             arg=selector,
             timeout=int(timeout * 1e3),
         )
 
     async def _isVisible(self, selector: str) -> bool:
         '''
@@ -372,15 +372,18 @@
         '''
         Evaluate and return javascript
 
         Parameters:
             script (str): Javascript to evaluate in the page
             arg (str, optional): Argument to pass into the javascript function
         '''
-        return await self.page.evaluate(script, arg=arg)
+        try:
+            return await self.page.evaluate(script, arg=arg)
+        except PlaywrightError as e:
+            raise JavascriptException('Javascript eval exception') from e
 
     async def _screenshot(self, path: str, full_page: bool = False):
         '''
         Take a screenshot of the page
 
         Parameters:
             path (str): Path to save screenshot to
@@ -578,26 +581,26 @@
 def render(
     url: str = None,
     headless: bool = True,
     proxy: dict = None,
     response: hrequests.response.Response = None,
     session: hrequests.session.TLSSession = None,
     mock_human: bool = False,
-    allow_styling: bool = True,
+    extensions: Optional[Union[str, Iterable[str]]] = None,
 ):
     assert any((url, session, response)), 'Must provide a url or an existing session, response'
     if proxy:
         proxy = list(proxy.values())[0]
     render_session = BrowserSession(
         session=session,
         resp=response,
         proxy_ip=proxy,
         headless=headless,
         mock_human=mock_human,
-        allow_styling=allow_styling,
+        extensions=extensions,
     )
     # include headers from session if a TLSSession is provided
     if session and isinstance(session, hrequests.session.TLSSession):
         render_session.setHeaders(session.headers)
     # include merged cookies from session or from response
     if req_src := session or response:
         render_session.setCookies(req_src.cookies)
```

### Comparing `hrequests-0.4.2/hrequests/cffi.py` & `hrequests-0.5.0/hrequests/cffi.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,18 +30,18 @@
                 return r'.*windows\-64\-.*\.dll'
             else:
                 return r'.*windows\-32\-.*\.dll'
         if machine() == "aarch64":
             return r'.*arm64\-.*\.so'
         if platform == 'linux':
             # check if alpine
-            os_name_dat = os.popen('cat /etc/os-release').read()
+            os_name_dat = open('/etc/os-release', 'r').read()
             if not os_name_dat:
                 return r'.*ubuntu\-amd64\-.*\.so'
-            os_name = re.search(r'NAME="(\w+)"', os_name_dat)[1]
+            os_name = re.search(r'\sID=(\w+)', os_name_dat)[1]
             if os_name.lower() == 'alpine':
                 return r'.*alpine\-amd64\-.*\.so'
         return r'.*ubuntu\-amd64\-.*\.so'
 
     def check_library(self):
         for file in os.listdir(self.parent_path):
             if self.file_regex.match(file):
```

### Comparing `hrequests-0.4.2/hrequests/client.py` & `hrequests-0.5.0/hrequests/client.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.2/hrequests/cookies.py` & `hrequests-0.5.0/hrequests/cookies.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,499 +1,499 @@
-import copy
-from http.client import HTTPMessage
-from http.cookiejar import Cookie, CookieJar
-from typing import Any, MutableMapping, Union
-from urllib.parse import urlparse, urlunparse
-
-import hrequests
-
-try:
-    import threading
-except ImportError:
-    import dummy_threading as threading
-
-
-class MockRequest:
-    """
-    Origin: requests library (https://github.com/psf/requests)
-    Mimic a urllib2.Request to get the correct cookie string for the request.
-    """
-
-    def __init__(self, request_url: str, request_headers: 'hrequests.client.CaseInsensitiveDict'):
-        self.request_url = request_url
-        self.request_headers = request_headers
-        self._new_headers = {}
-        self.type = urlparse(self.request_url).scheme
-
-    def get_type(self):
-        return self.type
-
-    def get_host(self):
-        return urlparse(self.request_url).netloc
-
-    def get_origin_req_host(self):
-        return self.get_host()
-
-    def get_full_url(self):
-        # Only return the response's URL if the user hadn't set the Host
-        # header
-        if not self.request_headers.get("Host"):
-            return self.request_url
-        # If they did set it, retrieve it and reconstruct the expected domain
-        host = self.request_headers["Host"]
-        parsed = urlparse(self.request_url)
-        # Reconstruct the URL as we expect it
-        return urlunparse(
-            [
-                parsed.scheme,
-                host,
-                parsed.path,
-                parsed.params,
-                parsed.query,
-                parsed.fragment,
-            ]
-        )
-
-    def is_unverifiable(self):
-        return True
-
-    def has_header(self, name):
-        return name in self.request_headers or name in self._new_headers
-
-    def get_header(self, name, default=None):
-        return self.request_headers.get(name, self._new_headers.get(name, default))
-
-    def add_unredirected_header(self, name, value):
-        self._new_headers[name] = value
-
-    def get_new_headers(self):
-        return self._new_headers
-
-    @property
-    def unverifiable(self):
-        return self.is_unverifiable()
-
-    @property
-    def origin_req_host(self):
-        return self.get_origin_req_host()
-
-    @property
-    def host(self):
-        return self.get_host()
-
-
-class MockResponse:
-    """
-    Wraps a httplib.HTTPMessage to mimic a urllib.addinfourl.
-    The objective is to retrieve the response cookies correctly.
-    """
-
-    def __init__(self, headers):
-        self._headers = headers
-
-    def info(self):
-        return self._headers
-
-    def getheaders(self, name):
-        self._headers.getheaders(name)
-
-
-class CookieConflictError(RuntimeError):
-    """
-    There are two cookies that meet the criteria specified in the cookie jar.
-    Use .get and .set and include domain and path args in order to be more specific.
-    """
-
-
-class RequestsCookieJar(CookieJar, MutableMapping):
-    """
-    Origin: requests library (https://github.com/psf/requests)
-    Compatibility class; is a cookielib.CookieJar, but exposes a dict
-    interface.
-
-    This is the CookieJar we create by default for requests and sessions that
-    don't specify one, since some clients may expect response.cookies and
-    session.cookies to support dict operations.
-
-    Requests does not use the dict interface internally; it's just for
-    compatibility with external client code. All requests code should work
-    out of the box with externally provided instances of ``CookieJar``, e.g.
-    ``LWPCookieJar`` and ``FileCookieJar``.
-
-    Unlike a regular CookieJar, this class is pickleable.
-
-    .. warning:: dictionary operations that are normally O(1) may be O(n).
-    """
-
-    def get(self, name, default=None, domain=None, path=None):
-        """Dict-like get() that also supports optional domain and path args in
-        order to resolve naming collisions from using one cookie jar over
-        multiple domains.
-
-        .. warning:: operation is O(n), not O(1).
-        """
-        try:
-            return self._find_no_duplicates(name, domain, path)
-        except KeyError:
-            return default
-
-    def set(self, name, value, **kwargs):
-        """Dict-like set() that also supports optional domain and path args in
-        order to resolve naming collisions from using one cookie jar over
-        multiple domains.
-        """
-        # support client code that unsets cookies by assignment of a None value:
-        if value is None:
-            remove_cookie_by_name(self, name, domain=kwargs.get("domain"), path=kwargs.get("path"))
-            return
-
-        c = create_cookie(name, value, **kwargs)
-        self.set_cookie(c)
-        return c
-
-    def iterkeys(self):
-        """Dict-like iterkeys() that returns an iterator of names of cookies
-        from the jar.
-
-        .. seealso:: itervalues() and iteritems().
-        """
-        for cookie in iter(self):
-            yield cookie.name
-
-    def keys(self):
-        """Dict-like keys() that returns a list of names of cookies from the
-        jar.
-
-        .. seealso:: values() and items().
-        """
-        return list(self.iterkeys())
-
-    def itervalues(self):
-        """Dict-like itervalues() that returns an iterator of values of cookies
-        from the jar.
-
-        .. seealso:: iterkeys() and iteritems().
-        """
-        for cookie in iter(self):
-            yield cookie.value
-
-    def values(self):
-        """Dict-like values() that returns a list of values of cookies from the
-        jar.
-
-        .. seealso:: keys() and items().
-        """
-        return list(self.itervalues())
-
-    def iteritems(self):
-        """Dict-like iteritems() that returns an iterator of name-value tuples
-        from the jar.
-
-        .. seealso:: iterkeys() and itervalues().
-        """
-        for cookie in iter(self):
-            yield cookie.name, cookie.value
-
-    def items(self):
-        """Dict-like items() that returns a list of name-value tuples from the
-        jar. Allows client-code to call ``dict(RequestsCookieJar)`` and get a
-        vanilla python dict of key value pairs.
-
-        .. seealso:: keys() and values().
-        """
-        return list(self.iteritems())
-
-    def list_domains(self):
-        """Utility method to list all the domains in the jar."""
-        domains = []
-        for cookie in iter(self):
-            if cookie.domain not in domains:
-                domains.append(cookie.domain)
-        return domains
-
-    def list_paths(self):
-        """Utility method to list all the paths in the jar."""
-        paths = []
-        for cookie in iter(self):
-            if cookie.path not in paths:
-                paths.append(cookie.path)
-        return paths
-
-    def multiple_domains(self):
-        """Returns True if there are multiple domains in the jar.
-        Returns False otherwise.
-
-        :rtype: bool
-        """
-        domains = []
-        for cookie in iter(self):
-            if cookie.domain is not None and cookie.domain in domains:
-                return True
-            domains.append(cookie.domain)
-        return False  # there is only one domain in jar
-
-    def get_dict(self, domain=None, path=None):
-        """Takes as an argument an optional domain and path and returns a plain
-        old Python dict of name-value pairs of cookies that meet the
-        requirements.
-
-        :rtype: dict
-        """
-        dictionary = {}
-        for cookie in iter(self):
-            if (domain is None or cookie.domain == domain) and (
-                path is None or cookie.path == path
-            ):
-                dictionary[cookie.name] = cookie.value
-        return dictionary
-
-    def __contains__(self, name):
-        try:
-            return super().__contains__(name)
-        except CookieConflictError:
-            return True
-
-    def __getitem__(self, name):
-        """Dict-like __getitem__() for compatibility with client code. Throws
-        exception if there are more than one cookie with name. In that case,
-        use the more explicit get() method instead.
-
-        .. warning:: operation is O(n), not O(1).
-        """
-        return self._find_no_duplicates(name)
-
-    def __setitem__(self, name, value):
-        """Dict-like __setitem__ for compatibility with client code. Throws
-        exception if there is already a cookie of that name in the jar. In that
-        case, use the more explicit set() method instead.
-        """
-        self.set(name, value)
-
-    def __delitem__(self, name):
-        """Deletes a cookie given a name. Wraps ``cookielib.CookieJar``'s
-        ``remove_cookie_by_name()``.
-        """
-        remove_cookie_by_name(self, name)
-
-    def set_cookie(self, cookie, *args, **kwargs):
-        if (
-            hasattr(cookie.value, "startswith")
-            and cookie.value.startswith('"')
-            and cookie.value.endswith('"')
-        ):
-            cookie.value = cookie.value.replace('\\"', "")
-        return super().set_cookie(cookie, *args, **kwargs)
-
-    def update(self, other):
-        """Updates this jar with cookies from another CookieJar or dict-like"""
-        if isinstance(other, CookieJar):
-            for cookie in other:
-                self.set_cookie(copy.copy(cookie))
-        else:
-            super().update(other)
-
-    def _find(self, name, domain=None, path=None):
-        """Requests uses this method internally to get cookie values.
-
-        If there are conflicting cookies, _find arbitrarily chooses one.
-        See _find_no_duplicates if you want an exception thrown if there are
-        conflicting cookies.
-
-        :param name: a string containing name of cookie
-        :param domain: (optional) string containing domain of cookie
-        :param path: (optional) string containing path of cookie
-        :return: cookie.value
-        """
-        for cookie in iter(self):
-            if cookie.name == name:
-                if domain is None or cookie.domain == domain:
-                    if path is None or cookie.path == path:
-                        return cookie.value
-
-        raise KeyError(f"name={name!r}, domain={domain!r}, path={path!r}")
-
-    def _find_no_duplicates(self, name, domain=None, path=None):
-        """Both ``__get_item__`` and ``get`` call this function: it's never
-        used elsewhere in Requests.
-
-        :param name: a string containing name of cookie
-        :param domain: (optional) string containing domain of cookie
-        :param path: (optional) string containing path of cookie
-        :raises KeyError: if cookie is not found
-        :raises CookieConflictError: if there are multiple cookies
-            that match name and optionally domain and path
-        :return: cookie.value
-        """
-        toReturn = None
-        for cookie in iter(self):
-            if cookie.name == name:
-                if domain is None or cookie.domain == domain:
-                    if path is None or cookie.path == path:
-                        if toReturn is not None:
-                            # if there are multiple cookies that meet passed in criteria
-                            raise CookieConflictError(
-                                f"There are multiple cookies with name, {name!r}"
-                            )
-                        # we will eventually return this as long as no cookie conflict
-                        toReturn = cookie.value
-
-        if toReturn:
-            return toReturn
-        raise KeyError(f"name={name!r}, domain={domain!r}, path={path!r}")
-
-    def __getstate__(self):
-        """Unlike a normal CookieJar, this class is pickleable."""
-        state = self.__dict__.copy()
-        # remove the unpickleable RLock object
-        state.pop("_cookies_lock")
-        return state
-
-    def __setstate__(self, state):
-        """Unlike a normal CookieJar, this class is pickleable."""
-        self.__dict__.update(state)
-        if "_cookies_lock" not in self.__dict__:
-            self._cookies_lock = threading.RLock()
-
-    def copy(self):
-        """Return a copy of this RequestsCookieJar."""
-        new_cj = RequestsCookieJar()
-        new_cj.set_policy(self.get_policy())
-        new_cj.update(self)
-        return new_cj
-
-    def get_policy(self):
-        """Return the CookiePolicy instance used."""
-        return self._policy
-
-
-def remove_cookie_by_name(
-    cookiejar: RequestsCookieJar, name: str, domain: str = None, path: str = None
-):
-    """Removes a cookie by name, by default over all domains and paths."""
-    clearables = []
-    for cookie in cookiejar:
-        if cookie.name != name:
-            continue
-        if domain is not None and domain != cookie.domain:
-            continue
-        if path is not None and path != cookie.path:
-            continue
-        clearables.append((cookie.domain, cookie.path, cookie.name))
-
-    for domain, path, name in clearables:
-        cookiejar.clear(domain, path, name)
-
-
-def create_cookie(name: str, value: str, **kwargs: Any) -> Cookie:
-    """Make a cookie from underspecified parameters."""
-    result = {
-        "version": 0,
-        "name": name,
-        "value": value,
-        "port": None,
-        "domain": "",
-        "path": "/",
-        "secure": False,
-        "expires": None,
-        "discard": True,
-        "comment": None,
-        "comment_url": None,
-        "rest": {"HttpOnly": None},
-        "rfc2109": False,
-    }
-
-    badargs = set(kwargs) - set(result)
-    if badargs:
-        raise TypeError(f"create_cookie() got unexpected keyword arguments: {list(badargs)}")
-
-    result.update(kwargs)
-    result["port_specified"] = bool(result["port"])
-    result["domain_specified"] = bool(result["domain"])
-    result["domain_initial_dot"] = result["domain"].startswith(".")
-    result["path_specified"] = bool(result["path"])
-
-    return Cookie(**result)
-
-
-def cookiejar_from_dict(cookie_dict: dict) -> RequestsCookieJar:
-    """transform a dict to CookieJar"""
-    cookie_jar = RequestsCookieJar()
-    if cookie_dict is not None:
-        for name, value in cookie_dict.items():
-            cookie_jar.set_cookie(create_cookie(name=name, value=value))
-    return cookie_jar
-
-
-def merge_cookies(
-    cookiejar: RequestsCookieJar, cookies: Union[dict, RequestsCookieJar]
-) -> RequestsCookieJar:
-    """Merge cookies in session and cookies provided in request"""
-    if type(cookies) is dict:
-        cookies = cookiejar_from_dict(cookies)
-
-    for cookie in cookies:
-        cookiejar.set_cookie(cookie)
-
-    return cookiejar
-
-
-def get_cookie_header(
-    request_url: str,
-    request_headers: 'hrequests.client.CaseInsensitiveDict',
-    cookie_jar: RequestsCookieJar,
-) -> str:
-    r = MockRequest(request_url, request_headers)
-    cookie_jar.add_cookie_header(r)
-    return r.get_new_headers().get("Cookie")
-
-
-def extract_cookies_to_jar(
-    request_url: str,
-    request_headers: 'hrequests.client.CaseInsensitiveDict',
-    cookie_jar: RequestsCookieJar,
-    response_headers: dict,
-) -> RequestsCookieJar:
-    response_cookie_jar = cookiejar_from_dict({})
-
-    req = MockRequest(request_url, request_headers)
-    # mimic HTTPMessage
-    http_message = HTTPMessage()
-    http_message._headers = []
-    for header_name, header_values in response_headers.items():
-        http_message._headers.extend((header_name, header_value) for header_value in header_values)
-    res = MockResponse(http_message)
-    response_cookie_jar.extract_cookies(res, req)
-
-    merge_cookies(cookie_jar, response_cookie_jar)
-    return response_cookie_jar
-
-
-'''
-Utilities to convert Playwright cookies to RequestsCookieJar and vice versa
-'''
-
-cookie_keys: tuple = ('name', 'value', 'port', 'domain', 'path', 'expires', 'secure', 'discard')
-
-
-def list_to_cookiejar(browser_cookies: list) -> RequestsCookieJar:
-    cookiejar: RequestsCookieJar = RequestsCookieJar()
-    for br_cookie in browser_cookies:
-        # swap "session" parameter to "discard"
-        if 'session' in br_cookie:
-            br_cookie['discard'] = br_cookie['session']
-            del br_cookie['session']
-        # create a cookie object
-        cookiejar.set_cookie(
-            create_cookie(**{key: value for key, value in br_cookie.items() if key in cookie_keys})
-        )
-    return cookiejar
-
-
-def cookiejar_to_list(cookiejar: RequestsCookieJar) -> list:
-    return [
-        {
-            'session' if key == 'discard' else key: getattr(cookie, key)
-            for key in cookie_keys
-            if key in cookie.__dict__
-        }
-        for cookie in cookiejar
-    ]
+import copy
+from http.client import HTTPMessage
+from http.cookiejar import Cookie, CookieJar
+from typing import Any, MutableMapping, Union
+from urllib.parse import urlparse, urlunparse
+
+import hrequests
+
+try:
+    import threading
+except ImportError:
+    import dummy_threading as threading
+
+
+class MockRequest:
+    """
+    Origin: requests library (https://github.com/psf/requests)
+    Mimic a urllib2.Request to get the correct cookie string for the request.
+    """
+
+    def __init__(self, request_url: str, request_headers: 'hrequests.client.CaseInsensitiveDict'):
+        self.request_url = request_url
+        self.request_headers = request_headers
+        self._new_headers = {}
+        self.type = urlparse(self.request_url).scheme
+
+    def get_type(self):
+        return self.type
+
+    def get_host(self):
+        return urlparse(self.request_url).netloc
+
+    def get_origin_req_host(self):
+        return self.get_host()
+
+    def get_full_url(self):
+        # Only return the response's URL if the user hadn't set the Host
+        # header
+        if not self.request_headers.get("Host"):
+            return self.request_url
+        # If they did set it, retrieve it and reconstruct the expected domain
+        host = self.request_headers["Host"]
+        parsed = urlparse(self.request_url)
+        # Reconstruct the URL as we expect it
+        return urlunparse(
+            [
+                parsed.scheme,
+                host,
+                parsed.path,
+                parsed.params,
+                parsed.query,
+                parsed.fragment,
+            ]
+        )
+
+    def is_unverifiable(self):
+        return True
+
+    def has_header(self, name):
+        return name in self.request_headers or name in self._new_headers
+
+    def get_header(self, name, default=None):
+        return self.request_headers.get(name, self._new_headers.get(name, default))
+
+    def add_unredirected_header(self, name, value):
+        self._new_headers[name] = value
+
+    def get_new_headers(self):
+        return self._new_headers
+
+    @property
+    def unverifiable(self):
+        return self.is_unverifiable()
+
+    @property
+    def origin_req_host(self):
+        return self.get_origin_req_host()
+
+    @property
+    def host(self):
+        return self.get_host()
+
+
+class MockResponse:
+    """
+    Wraps a httplib.HTTPMessage to mimic a urllib.addinfourl.
+    The objective is to retrieve the response cookies correctly.
+    """
+
+    def __init__(self, headers):
+        self._headers = headers
+
+    def info(self):
+        return self._headers
+
+    def getheaders(self, name):
+        self._headers.getheaders(name)
+
+
+class CookieConflictError(RuntimeError):
+    """
+    There are two cookies that meet the criteria specified in the cookie jar.
+    Use .get and .set and include domain and path args in order to be more specific.
+    """
+
+
+class RequestsCookieJar(CookieJar, MutableMapping):
+    """
+    Origin: requests library (https://github.com/psf/requests)
+    Compatibility class; is a cookielib.CookieJar, but exposes a dict
+    interface.
+
+    This is the CookieJar we create by default for requests and sessions that
+    don't specify one, since some clients may expect response.cookies and
+    session.cookies to support dict operations.
+
+    Requests does not use the dict interface internally; it's just for
+    compatibility with external client code. All requests code should work
+    out of the box with externally provided instances of ``CookieJar``, e.g.
+    ``LWPCookieJar`` and ``FileCookieJar``.
+
+    Unlike a regular CookieJar, this class is pickleable.
+
+    .. warning:: dictionary operations that are normally O(1) may be O(n).
+    """
+
+    def get(self, name, default=None, domain=None, path=None):
+        """Dict-like get() that also supports optional domain and path args in
+        order to resolve naming collisions from using one cookie jar over
+        multiple domains.
+
+        .. warning:: operation is O(n), not O(1).
+        """
+        try:
+            return self._find_no_duplicates(name, domain, path)
+        except KeyError:
+            return default
+
+    def set(self, name, value, **kwargs):
+        """Dict-like set() that also supports optional domain and path args in
+        order to resolve naming collisions from using one cookie jar over
+        multiple domains.
+        """
+        # support client code that unsets cookies by assignment of a None value:
+        if value is None:
+            remove_cookie_by_name(self, name, domain=kwargs.get("domain"), path=kwargs.get("path"))
+            return
+
+        c = create_cookie(name, value, **kwargs)
+        self.set_cookie(c)
+        return c
+
+    def iterkeys(self):
+        """Dict-like iterkeys() that returns an iterator of names of cookies
+        from the jar.
+
+        .. seealso:: itervalues() and iteritems().
+        """
+        for cookie in iter(self):
+            yield cookie.name
+
+    def keys(self):
+        """Dict-like keys() that returns a list of names of cookies from the
+        jar.
+
+        .. seealso:: values() and items().
+        """
+        return list(self.iterkeys())
+
+    def itervalues(self):
+        """Dict-like itervalues() that returns an iterator of values of cookies
+        from the jar.
+
+        .. seealso:: iterkeys() and iteritems().
+        """
+        for cookie in iter(self):
+            yield cookie.value
+
+    def values(self):
+        """Dict-like values() that returns a list of values of cookies from the
+        jar.
+
+        .. seealso:: keys() and items().
+        """
+        return list(self.itervalues())
+
+    def iteritems(self):
+        """Dict-like iteritems() that returns an iterator of name-value tuples
+        from the jar.
+
+        .. seealso:: iterkeys() and itervalues().
+        """
+        for cookie in iter(self):
+            yield cookie.name, cookie.value
+
+    def items(self):
+        """Dict-like items() that returns a list of name-value tuples from the
+        jar. Allows client-code to call ``dict(RequestsCookieJar)`` and get a
+        vanilla python dict of key value pairs.
+
+        .. seealso:: keys() and values().
+        """
+        return list(self.iteritems())
+
+    def list_domains(self):
+        """Utility method to list all the domains in the jar."""
+        domains = []
+        for cookie in iter(self):
+            if cookie.domain not in domains:
+                domains.append(cookie.domain)
+        return domains
+
+    def list_paths(self):
+        """Utility method to list all the paths in the jar."""
+        paths = []
+        for cookie in iter(self):
+            if cookie.path not in paths:
+                paths.append(cookie.path)
+        return paths
+
+    def multiple_domains(self):
+        """Returns True if there are multiple domains in the jar.
+        Returns False otherwise.
+
+        :rtype: bool
+        """
+        domains = []
+        for cookie in iter(self):
+            if cookie.domain is not None and cookie.domain in domains:
+                return True
+            domains.append(cookie.domain)
+        return False  # there is only one domain in jar
+
+    def get_dict(self, domain=None, path=None):
+        """Takes as an argument an optional domain and path and returns a plain
+        old Python dict of name-value pairs of cookies that meet the
+        requirements.
+
+        :rtype: dict
+        """
+        dictionary = {}
+        for cookie in iter(self):
+            if (domain is None or cookie.domain == domain) and (
+                path is None or cookie.path == path
+            ):
+                dictionary[cookie.name] = cookie.value
+        return dictionary
+
+    def __contains__(self, name):
+        try:
+            return super().__contains__(name)
+        except CookieConflictError:
+            return True
+
+    def __getitem__(self, name):
+        """Dict-like __getitem__() for compatibility with client code. Throws
+        exception if there are more than one cookie with name. In that case,
+        use the more explicit get() method instead.
+
+        .. warning:: operation is O(n), not O(1).
+        """
+        return self._find_no_duplicates(name)
+
+    def __setitem__(self, name, value):
+        """Dict-like __setitem__ for compatibility with client code. Throws
+        exception if there is already a cookie of that name in the jar. In that
+        case, use the more explicit set() method instead.
+        """
+        self.set(name, value)
+
+    def __delitem__(self, name):
+        """Deletes a cookie given a name. Wraps ``cookielib.CookieJar``'s
+        ``remove_cookie_by_name()``.
+        """
+        remove_cookie_by_name(self, name)
+
+    def set_cookie(self, cookie, *args, **kwargs):
+        if (
+            hasattr(cookie.value, "startswith")
+            and cookie.value.startswith('"')
+            and cookie.value.endswith('"')
+        ):
+            cookie.value = cookie.value.replace('\\"', "")
+        return super().set_cookie(cookie, *args, **kwargs)
+
+    def update(self, other):
+        """Updates this jar with cookies from another CookieJar or dict-like"""
+        if isinstance(other, CookieJar):
+            for cookie in other:
+                self.set_cookie(copy.copy(cookie))
+        else:
+            super().update(other)
+
+    def _find(self, name, domain=None, path=None):
+        """Requests uses this method internally to get cookie values.
+
+        If there are conflicting cookies, _find arbitrarily chooses one.
+        See _find_no_duplicates if you want an exception thrown if there are
+        conflicting cookies.
+
+        :param name: a string containing name of cookie
+        :param domain: (optional) string containing domain of cookie
+        :param path: (optional) string containing path of cookie
+        :return: cookie.value
+        """
+        for cookie in iter(self):
+            if cookie.name == name:
+                if domain is None or cookie.domain == domain:
+                    if path is None or cookie.path == path:
+                        return cookie.value
+
+        raise KeyError(f"name={name!r}, domain={domain!r}, path={path!r}")
+
+    def _find_no_duplicates(self, name, domain=None, path=None):
+        """Both ``__get_item__`` and ``get`` call this function: it's never
+        used elsewhere in Requests.
+
+        :param name: a string containing name of cookie
+        :param domain: (optional) string containing domain of cookie
+        :param path: (optional) string containing path of cookie
+        :raises KeyError: if cookie is not found
+        :raises CookieConflictError: if there are multiple cookies
+            that match name and optionally domain and path
+        :return: cookie.value
+        """
+        toReturn = None
+        for cookie in iter(self):
+            if cookie.name == name:
+                if domain is None or cookie.domain == domain:
+                    if path is None or cookie.path == path:
+                        if toReturn is not None:
+                            # if there are multiple cookies that meet passed in criteria
+                            raise CookieConflictError(
+                                f"There are multiple cookies with name, {name!r}"
+                            )
+                        # we will eventually return this as long as no cookie conflict
+                        toReturn = cookie.value
+
+        if toReturn:
+            return toReturn
+        raise KeyError(f"name={name!r}, domain={domain!r}, path={path!r}")
+
+    def __getstate__(self):
+        """Unlike a normal CookieJar, this class is pickleable."""
+        state = self.__dict__.copy()
+        # remove the unpickleable RLock object
+        state.pop("_cookies_lock")
+        return state
+
+    def __setstate__(self, state):
+        """Unlike a normal CookieJar, this class is pickleable."""
+        self.__dict__.update(state)
+        if "_cookies_lock" not in self.__dict__:
+            self._cookies_lock = threading.RLock()
+
+    def copy(self):
+        """Return a copy of this RequestsCookieJar."""
+        new_cj = RequestsCookieJar()
+        new_cj.set_policy(self.get_policy())
+        new_cj.update(self)
+        return new_cj
+
+    def get_policy(self):
+        """Return the CookiePolicy instance used."""
+        return self._policy
+
+
+def remove_cookie_by_name(
+    cookiejar: RequestsCookieJar, name: str, domain: str = None, path: str = None
+):
+    """Removes a cookie by name, by default over all domains and paths."""
+    clearables = []
+    for cookie in cookiejar:
+        if cookie.name != name:
+            continue
+        if domain is not None and domain != cookie.domain:
+            continue
+        if path is not None and path != cookie.path:
+            continue
+        clearables.append((cookie.domain, cookie.path, cookie.name))
+
+    for domain, path, name in clearables:
+        cookiejar.clear(domain, path, name)
+
+
+def create_cookie(name: str, value: str, **kwargs: Any) -> Cookie:
+    """Make a cookie from underspecified parameters."""
+    result = {
+        "version": 0,
+        "name": name,
+        "value": value,
+        "port": None,
+        "domain": "",
+        "path": "/",
+        "secure": False,
+        "expires": None,
+        "discard": True,
+        "comment": None,
+        "comment_url": None,
+        "rest": {"HttpOnly": None},
+        "rfc2109": False,
+    }
+
+    badargs = set(kwargs) - set(result)
+    if badargs:
+        raise TypeError(f"create_cookie() got unexpected keyword arguments: {list(badargs)}")
+
+    result.update(kwargs)
+    result["port_specified"] = bool(result["port"])
+    result["domain_specified"] = bool(result["domain"])
+    result["domain_initial_dot"] = result["domain"].startswith(".")
+    result["path_specified"] = bool(result["path"])
+
+    return Cookie(**result)
+
+
+def cookiejar_from_dict(cookie_dict: dict) -> RequestsCookieJar:
+    """transform a dict to CookieJar"""
+    cookie_jar = RequestsCookieJar()
+    if cookie_dict is not None:
+        for name, value in cookie_dict.items():
+            cookie_jar.set_cookie(create_cookie(name=name, value=value))
+    return cookie_jar
+
+
+def merge_cookies(
+    cookiejar: RequestsCookieJar, cookies: Union[dict, RequestsCookieJar]
+) -> RequestsCookieJar:
+    """Merge cookies in session and cookies provided in request"""
+    if type(cookies) is dict:
+        cookies = cookiejar_from_dict(cookies)
+
+    for cookie in cookies:
+        cookiejar.set_cookie(cookie)
+
+    return cookiejar
+
+
+def get_cookie_header(
+    request_url: str,
+    request_headers: 'hrequests.client.CaseInsensitiveDict',
+    cookie_jar: RequestsCookieJar,
+) -> str:
+    r = MockRequest(request_url, request_headers)
+    cookie_jar.add_cookie_header(r)
+    return r.get_new_headers().get("Cookie")
+
+
+def extract_cookies_to_jar(
+    request_url: str,
+    request_headers: 'hrequests.client.CaseInsensitiveDict',
+    cookie_jar: RequestsCookieJar,
+    response_headers: dict,
+) -> RequestsCookieJar:
+    response_cookie_jar = cookiejar_from_dict({})
+
+    req = MockRequest(request_url, request_headers)
+    # mimic HTTPMessage
+    http_message = HTTPMessage()
+    http_message._headers = []
+    for header_name, header_values in response_headers.items():
+        http_message._headers.extend((header_name, header_value) for header_value in header_values)
+    res = MockResponse(http_message)
+    response_cookie_jar.extract_cookies(res, req)
+
+    merge_cookies(cookie_jar, response_cookie_jar)
+    return response_cookie_jar
+
+
+'''
+Utilities to convert Playwright cookies to RequestsCookieJar and vice versa
+'''
+
+cookie_keys: tuple = ('name', 'value', 'port', 'domain', 'path', 'expires', 'secure', 'discard')
+
+
+def list_to_cookiejar(browser_cookies: list) -> RequestsCookieJar:
+    cookiejar: RequestsCookieJar = RequestsCookieJar()
+    for br_cookie in browser_cookies:
+        # swap "session" parameter to "discard"
+        if 'session' in br_cookie:
+            br_cookie['discard'] = br_cookie['session']
+            del br_cookie['session']
+        # create a cookie object
+        cookiejar.set_cookie(
+            create_cookie(**{key: value for key, value in br_cookie.items() if key in cookie_keys})
+        )
+    return cookiejar
+
+
+def cookiejar_to_list(cookiejar: RequestsCookieJar) -> list:
+    return [
+        {
+            'session' if key == 'discard' else key: val
+            for key in cookie_keys
+            if key in cookie.__dict__ and (val := getattr(cookie, key)) is not None
+        }
+        for cookie in cookiejar
+    ]
```

### Comparing `hrequests-0.4.2/hrequests/exceptions.py` & `hrequests-0.5.0/hrequests/exceptions.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,7 +16,11 @@
 
 class NoPauseRuntimeException(RuntimeError):
     '''Exception raised when a request with no_pause=True is called from a different thread than it was created in'''
 
 
 class NotRenderedException(Exception):
     '''Raise when the user tries to interact with an element that is not in a BrowserSession'''
+
+
+class JavascriptException(BrowserException):
+    '''Exception raised when a javascript error occurs'''
```

### Comparing `hrequests-0.4.2/hrequests/parser.py` & `hrequests-0.5.0/hrequests/parser.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.2/hrequests/playwright_mock/context.py` & `hrequests-0.5.0/hrequests/playwright_mock/context.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.2/hrequests/playwright_mock/element_handle.py` & `hrequests-0.5.0/hrequests/playwright_mock/element_handle.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.2/hrequests/playwright_mock/faker.py` & `hrequests-0.5.0/hrequests/playwright_mock/faker.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.2/hrequests/playwright_mock/frame.py` & `hrequests-0.5.0/hrequests/playwright_mock/frame.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.2/hrequests/playwright_mock/frame_locator.py` & `hrequests-0.5.0/hrequests/playwright_mock/frame_locator.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.2/hrequests/playwright_mock/locale.json` & `hrequests-0.5.0/hrequests/playwright_mock/locale.json`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.2/hrequests/playwright_mock/locator.py` & `hrequests-0.5.0/hrequests/playwright_mock/locator.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.2/hrequests/playwright_mock/mouse.py` & `hrequests-0.5.0/hrequests/playwright_mock/mouse.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.2/hrequests/playwright_mock/page.py` & `hrequests-0.5.0/hrequests/playwright_mock/page.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.2/hrequests/playwright_mock/playwright_mock.py` & `hrequests-0.5.0/hrequests/playwright_mock/playwright_mock.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,49 @@
+from typing import List, Tuple
+
 from async_class import AsyncObject
 from hrequests.playwright_mock import Faker, ProxyManager, context
 from playwright.async_api import async_playwright
 
 
 class PlaywrightMock(AsyncObject):
-    async def __ainit__(self, headless=False, scroll_into_view=True):
+    async def __ainit__(
+        self,
+        headless: bool = False,
+        scroll_into_view: bool = True,
+        extensions=None,
+    ):
         # setting values
         self.scroll_into_view = scroll_into_view
+        self.extensions = extensions
         # starting Playwright
         self.playwright = await async_playwright().start()
         # launching chromium
-        self.main_browser = await self.launch_browser(client=self.playwright, headless=headless)
+        self.main_browser = await self.launch_browser(headless=headless)
 
-    args = [
+    args: Tuple[str] = (
         '--disable-blink-features=AutomationControlled',
         '--disable-web-security',
         '--disable-site-isolation-trials',
         '--disable-features=CrossSiteDocumentBlockingIfIsolating,'
         'CrossSiteDocumentBlockingAlways,'
         'IsolateOrigins,'
         'site-per-process,'
         'SharedArrayBuffer',
-    ]
+    )  # type: ignore
 
-    @staticmethod
-    async def launch_browser(client, headless=False):
-        return await client.chromium.launch(
-            headless=headless,
-            args=PlaywrightMock.args + (['--headless=new'] if headless else []),
-        )
+    async def launch_browser(self, headless: bool = False):
+        args: List[str] = list(PlaywrightMock.args)
+        if headless:
+            args.append('--headless=new')
+        if self.extensions:
+            paths = [ext.path for ext in self.extensions]
+            args.extend(f'--load-extension={ext}' for ext in paths)
+            args.append(f'--disable-extensions-except={",".join(paths)}')
+        return await self.playwright.chromium.launch(headless=headless, args=args)
 
     async def stop(self):
         await self.main_browser.close()
         await self.playwright.stop()
 
     async def new_context(self, browser_name: str, user_agent: str, proxy=None, **launch_args):
         # calling proxyManager and faker
```

### Comparing `hrequests-0.4.2/hrequests/playwright_mock/proxy_manager.py` & `hrequests-0.5.0/hrequests/playwright_mock/proxy_manager.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.2/hrequests/reqs.py` & `hrequests-0.5.0/hrequests/reqs.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.2/hrequests/response.py` & `hrequests-0.5.0/hrequests/response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 from http.client import responses as status_codes
 from json import detect_encoding
-from typing import List, Optional, Union
+from typing import List, Optional, Union, Iterable
 
 import orjson
 
 import hrequests
 from hrequests.exceptions import ClientException
 
 from .cookies import RequestsCookieJar
@@ -182,23 +182,27 @@
         return resolved_links
 
     def __bool__(self) -> bool:
         '''Returns True if :attr:`status_code` is less than 400'''
         return self.ok
 
     def render(
-        self, *, headless: bool = True, mock_human: bool = False, allow_styling: bool = True
+        self,
+        *,
+        headless: bool = True,
+        mock_human: bool = False,
+        extensions: Optional[Union[str, Iterable[str]]] = None,
     ) -> 'hrequests.browser.BrowserSession':
         return hrequests.browser.render(
             response=self,
             session=self.session,
             proxy=self.session.proxies if self.session else None,
             headless=headless,
             mock_human=mock_human,
-            allow_styling=allow_styling,
+            extensions=extensions,
         )
 
     def __enter__(self):
         return self
 
     def __repr__(self):
         return f"<Response [{self.status_code}]>"
```

### Comparing `hrequests-0.4.2/hrequests/session.py` & `hrequests-0.5.0/hrequests/session.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.2/hrequests/toolbelt.py` & `hrequests-0.5.0/hrequests/toolbelt.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.2/LICENSE` & `hrequests-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hrequests-0.4.2/pyproject.toml` & `hrequests-0.5.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hrequests"
-version = "0.4.2"
+version = "0.5.0"
 description = "Hrequests (human requests) is a simple, configurable, feature-rich, replacement for the Python requests library."
 authors = ["daijro <daijro.dev@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/daijro/hrequests"
 keywords = ["tls", "client", "http", "scraping", "requests", "humans", "playwright"]
 classifiers = [
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: Browsers",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.7"
 orjson = "*"
 httpx = "*"
-playwright = "*"
+urllib3 = "*"
+playwright = "1.34.0"
 playwright-stealth = "*"
 wget = "*"
 async-class = "*"
 aioprocessing = "*"
 numpy = "*"
 fake-headers = "*"
+pycryptodome = "*"
 lxml = "*"
 parse = "*"
 pyquery = "*"
 w3lib = "*"
 gevent = "*"
 msvc-runtime = {version = "*", markers = "sys_platform == 'win32'"}
```

### Comparing `hrequests-0.4.2/README.md` & `hrequests-0.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 <h4 align="center">
 <p align="center">
     <a href="https://github.com/daijro/hrequests/blob/main/LICENSE">
         <img src="https://img.shields.io/github/license/daijro/hrequests.svg">
     </a>
     <a href="https://python.org/">
-        <img src="https://img.shields.io/badge/python-3.6&#8208;3.11-blue">
+        <img src="https://img.shields.io/badge/python-3.7&#8208;3.11-blue">
     </a>
     <a href="https://pypi.org/project/hrequests/">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/hrequests.svg">
     </a>
     <a href="https://pepy.tech/project/hrequests">
         <img alt="PyPI" src="https://pepy.tech/badge/hrequests">
     </a>
@@ -56,16 +56,16 @@
 ---
 
 # Installation
 
 Install via pip:
 
 ```bash
-pip install hrequests
-playwright install
+pip install -U hrequests
+python -m playwright install chromium
 ```
 
 Other depedencies will be downloaded on the first import:
 
 ```py
 >>> import hrequests
 ```
@@ -636,14 +636,30 @@
 
 You can spawn a `BrowserSession` instance by calling it:
 
 ```py
 >>> page = hrequests.BrowserSession()  # headless=True by default
 ```
 
+<details>
+<summary>Parameters</summary>
+
+```
+Parameters:
+    headless (bool, optional): Whether to run the browser in headless mode. Defaults to True.
+    session (hrequests.session.TLSSession, optional): Session to use for headers, cookies, etc.
+    resp (hrequests.response.Response, optional): Response to update with cookies, headers, etc.
+    proxy_ip (str, optional): Proxy to use for the browser. Example: 123.123.123
+    mock_human (bool, optional): Whether to emulate human behavior. Defaults to False.
+    browser (Literal['firefox', 'chrome', 'opera'], optional): Generate useragent headers for a specific browser
+    os (Literal['win', 'mac', 'lin'], optional): Generate headers for a specific OS
+    extensions (Union[str, Iterable[str]], optional): Path to a folder of unpacked extensions, or a list of paths to unpacked extensions
+```
+</details>
+
 `BrowserSession` is entirely safe to use across threads.
 
 ### Render an existing Response
 
 Responses have a `.render()` method. This will render the contents of the response in a browser page.
 
 Once the page is closed, the Response content and the Response's session cookies will be updated.
@@ -679,35 +695,29 @@
 <details>
 <summary>Parameters</summary>
 
 ```
 Parameters:
     headless (bool, optional): Whether to run the browser in headless mode. Defaults to False.
     mock_human (bool, optional): Whether to emulate human behavior. Defaults to False.
-    allow_styling (bool, optional): Allow loading images, fonts, styles, etc. Defaults to True
+    extensions (Union[str, Iterable[str]], optional): Path to a folder of unpacked extensions, or a list of paths to unpacked extensions
 ```
 </details>
 
 ### Properties
 
 Cookies are inherited from the session:
 
 ```py
 >>> page.cookies: RequestsCookieJar  # cookies are inherited from the session
 <RequestsCookieJar[Cookie(version=0, name='1P_JAR', value='2023-07-05-20', port=None, port_specified=False, domain='.somewebsite.com', domain_specified=True...
 ```
 
-Toggle loading unnessecary resources such as images, fonts, styles, etc:
-```py
-page.allow_styling: bool = False
-```
-
 ### Pulling page data
 
-
 Get current page url:
 
 ```py
 >>> page.url: str
 https://www.somewebsite.com/
 ```
 
@@ -956,14 +966,45 @@
     timeout (float, optional): Timeout in seconds. Defaults to 30.
 
 Throws:
     hrequests.exceptions.BrowserTimeoutException: If timeout is reached
 ```
 </details>
 
+### Adding Chrome extensions
+
+Chrome extensions can be easily imported into a browser session. Some potentially useful extensions include:
+
+- [hektCaptcha](https://github.com/Wikidepia/hektCaptcha-extension) - Hcaptcha solver
+
+- [uBlock Origin](https://github.com/gorhill/uBlock) - Ad & popup blocker
+
+- [FastForward](https://fastforward.team/) - Bypass & skip link redirects
+
+Extensions are added with the `extensions` parameter.
+
+- This can be an list of absolute paths to unpacked extensions:
+    ```py
+    with resp.render(extensions=['C:\\extentions\\hektcaptcha', 'C:\\extentions\\ublockorigin']):
+    ```
+
+- Or a folder containing the unpacked extensions:
+    ```py
+    with resp.render(extensions='C:\\extentions'):
+    ```
+    Note that these need to be *unpacked* extensions. You can unpack a `.crx` file by changing the file extension to `.zip` and extracting the contents.
+
+Here is an usage example of using a captcha solver:
+
+```py
+>>> with hrequests.render('https://accounts.hcaptcha.com/demo', extensions=['C:\\extentions\\hektcaptcha']):
+...     page.awaitSelector('.hcaptcha-success')  # wait for captcha to finish
+...     page.click('input[type=submit]')
+```
+
 ### Requests & Responses
 
 Requests can also be sent within browser sessions. These operate the same as the standard `hrequests.request`, and will use the browser's cookies and headers. The `BrowserSession` cookies will be updated with each request.
 
 This returns a normal `Response` object:
 ```py
 >>> resp = page.get('https://duckduckgo.com')
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_frgzxwnw_/tmpi9d3ogst_TarContainer/0/29.md", line 1037, column 3: CDATA terminal not found*

 * *File "/tmp/diffoscope_frgzxwnw_/tmpi9d3ogst_TarContainer/0/29.md", line 1037, column 3: CDATA terminal not found*

```diff
@@ -1,32 +1,32 @@
 [https://i.imgur.com/r8GcQW1.png]
                              ***** hrequests *****
   *** [https://img.shields.io/github/license/daijro/hrequests.svg] [https://
-   img.shields.io/badge/python-3.6&#8208;3.11-blue] [PyPI] [PyPI] [https://
+   img.shields.io/badge/python-3.7&#8208;3.11-blue] [PyPI] [PyPI] [https://
   img.shields.io/badge/code%20style-black-black.svg] [https://img.shields.io/
     badge/imports-isort-yellow.svg]Hrequests (human requests) is a simple,
  configurable, feature-rich, replacement for the Python requests library. ***
 ### â¨ Features - Seamless transition between HTTP and headless browsing ð»
 - Integrated fast HTML parser ð - High performance concurrency with gevent
 (*without monkey-patching!*) ð - Replication of browser TLS fingerprints
 ð - JavaScript rendering ð - Supports HTTP/2 ð - Realistic browser
 header generation ð - JSON serializing up to 10x faster than the standard
 library ð ### ð» Browser crawling - Simple & uncomplicated browser
 automation - Human-like cursor movement and typing - Full page screenshots -
 Headless and headful support - No CORS restrictions ### â¡ More - High
 performance â¨ - Minimal dependence on the python standard libraries - Written
 with type safety - 100% threadsafe â¤ï¸ --- # Installation Install via pip:
-```bash pip install hrequests playwright install ``` Other depedencies will be
-downloaded on the first import: ```py >>> import hrequests ``` --- #
-Documentation 1. [Simple Usage](https://github.com/daijro/hrequests#simple-
-usage) 2. [Sessions](https://github.com/daijro/hrequests#sessions) 3.
-[Concurrent & Lazy Requests](https://github.com/daijro/hrequests#concurrent--
-lazy-requests) 4. [HTML Parsing](https://github.com/daijro/hrequests#html-
-parsing) 5. [Browser Automation](https://github.com/daijro/hrequests#browser-
-automation)
+```bash pip install -U hrequests python -m playwright install chromium ```
+Other depedencies will be downloaded on the first import: ```py >>> import
+hrequests ``` --- # Documentation 1. [Simple Usage](https://github.com/daijro/
+hrequests#simple-usage) 2. [Sessions](https://github.com/daijro/
+hrequests#sessions) 3. [Concurrent & Lazy Requests](https://github.com/daijro/
+hrequests#concurrent--lazy-requests) 4. [HTML Parsing](https://github.com/
+daijro/hrequests#html-parsing) 5. [Browser Automation](https://github.com/
+daijro/hrequests#browser-automation)
 ===============================================================================
 ## Simple Usage Here is an example of a simple `get` request: ```py >>> resp =
 hrequests.get('https://www.google.com/') ``` Requests are sent through
 [bogdanfinn's tls-client](https://github.com/bogdanfinn/tls-client) to spoof
 the TLS client fingerprint. This is done automatically, and is completely
 transparent to the user. Other request methods include `post`, `put`, `delete`,
 `head`, `options`, and `patch`. The `Response` object is a near 1:1 replica of
```

### Comparing `hrequests-0.4.2/PKG-INFO` & `hrequests-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: hrequests
-Version: 0.4.2
+Version: 0.5.0
 Summary: Hrequests (human requests) is a simple, configurable, feature-rich, replacement for the Python requests library.
 Home-page: https://github.com/daijro/hrequests
 License: Apache-2.0
 Keywords: tls,client,http,scraping,requests,humans,playwright
 Author: daijro
 Author-email: daijro.dev@gmail.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Browsers
@@ -25,17 +24,19 @@
 Requires-Dist: gevent
 Requires-Dist: httpx
 Requires-Dist: lxml
 Requires-Dist: msvc-runtime ; sys_platform == "win32"
 Requires-Dist: numpy
 Requires-Dist: orjson
 Requires-Dist: parse
-Requires-Dist: playwright
+Requires-Dist: playwright (==1.34.0)
 Requires-Dist: playwright-stealth
+Requires-Dist: pycryptodome
 Requires-Dist: pyquery
+Requires-Dist: urllib3
 Requires-Dist: w3lib
 Requires-Dist: wget
 Project-URL: Repository, https://github.com/daijro/hrequests
 Description-Content-Type: text/markdown
 
 <img src="https://i.imgur.com/r8GcQW1.png" align="center">
 </img>
@@ -45,15 +46,15 @@
 
 <h4 align="center">
 <p align="center">
     <a href="https://github.com/daijro/hrequests/blob/main/LICENSE">
         <img src="https://img.shields.io/github/license/daijro/hrequests.svg">
     </a>
     <a href="https://python.org/">
-        <img src="https://img.shields.io/badge/python-3.6&#8208;3.11-blue">
+        <img src="https://img.shields.io/badge/python-3.7&#8208;3.11-blue">
     </a>
     <a href="https://pypi.org/project/hrequests/">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/hrequests.svg">
     </a>
     <a href="https://pepy.tech/project/hrequests">
         <img alt="PyPI" src="https://pepy.tech/badge/hrequests">
     </a>
@@ -95,16 +96,16 @@
 ---
 
 # Installation
 
 Install via pip:
 
 ```bash
-pip install hrequests
-playwright install
+pip install -U hrequests
+python -m playwright install chromium
 ```
 
 Other depedencies will be downloaded on the first import:
 
 ```py
 >>> import hrequests
 ```
@@ -675,14 +676,30 @@
 
 You can spawn a `BrowserSession` instance by calling it:
 
 ```py
 >>> page = hrequests.BrowserSession()  # headless=True by default
 ```
 
+<details>
+<summary>Parameters</summary>
+
+```
+Parameters:
+    headless (bool, optional): Whether to run the browser in headless mode. Defaults to True.
+    session (hrequests.session.TLSSession, optional): Session to use for headers, cookies, etc.
+    resp (hrequests.response.Response, optional): Response to update with cookies, headers, etc.
+    proxy_ip (str, optional): Proxy to use for the browser. Example: 123.123.123
+    mock_human (bool, optional): Whether to emulate human behavior. Defaults to False.
+    browser (Literal['firefox', 'chrome', 'opera'], optional): Generate useragent headers for a specific browser
+    os (Literal['win', 'mac', 'lin'], optional): Generate headers for a specific OS
+    extensions (Union[str, Iterable[str]], optional): Path to a folder of unpacked extensions, or a list of paths to unpacked extensions
+```
+</details>
+
 `BrowserSession` is entirely safe to use across threads.
 
 ### Render an existing Response
 
 Responses have a `.render()` method. This will render the contents of the response in a browser page.
 
 Once the page is closed, the Response content and the Response's session cookies will be updated.
@@ -718,35 +735,29 @@
 <details>
 <summary>Parameters</summary>
 
 ```
 Parameters:
     headless (bool, optional): Whether to run the browser in headless mode. Defaults to False.
     mock_human (bool, optional): Whether to emulate human behavior. Defaults to False.
-    allow_styling (bool, optional): Allow loading images, fonts, styles, etc. Defaults to True
+    extensions (Union[str, Iterable[str]], optional): Path to a folder of unpacked extensions, or a list of paths to unpacked extensions
 ```
 </details>
 
 ### Properties
 
 Cookies are inherited from the session:
 
 ```py
 >>> page.cookies: RequestsCookieJar  # cookies are inherited from the session
 <RequestsCookieJar[Cookie(version=0, name='1P_JAR', value='2023-07-05-20', port=None, port_specified=False, domain='.somewebsite.com', domain_specified=True...
 ```
 
-Toggle loading unnessecary resources such as images, fonts, styles, etc:
-```py
-page.allow_styling: bool = False
-```
-
 ### Pulling page data
 
-
 Get current page url:
 
 ```py
 >>> page.url: str
 https://www.somewebsite.com/
 ```
 
@@ -995,14 +1006,45 @@
     timeout (float, optional): Timeout in seconds. Defaults to 30.
 
 Throws:
     hrequests.exceptions.BrowserTimeoutException: If timeout is reached
 ```
 </details>
 
+### Adding Chrome extensions
+
+Chrome extensions can be easily imported into a browser session. Some potentially useful extensions include:
+
+- [hektCaptcha](https://github.com/Wikidepia/hektCaptcha-extension) - Hcaptcha solver
+
+- [uBlock Origin](https://github.com/gorhill/uBlock) - Ad & popup blocker
+
+- [FastForward](https://fastforward.team/) - Bypass & skip link redirects
+
+Extensions are added with the `extensions` parameter.
+
+- This can be an list of absolute paths to unpacked extensions:
+    ```py
+    with resp.render(extensions=['C:\\extentions\\hektcaptcha', 'C:\\extentions\\ublockorigin']):
+    ```
+
+- Or a folder containing the unpacked extensions:
+    ```py
+    with resp.render(extensions='C:\\extentions'):
+    ```
+    Note that these need to be *unpacked* extensions. You can unpack a `.crx` file by changing the file extension to `.zip` and extracting the contents.
+
+Here is an usage example of using a captcha solver:
+
+```py
+>>> with hrequests.render('https://accounts.hcaptcha.com/demo', extensions=['C:\\extentions\\hektcaptcha']):
+...     page.awaitSelector('.hcaptcha-success')  # wait for captcha to finish
+...     page.click('input[type=submit]')
+```
+
 ### Requests & Responses
 
 Requests can also be sent within browser sessions. These operate the same as the standard `hrequests.request`, and will use the browser's cookies and headers. The `BrowserSession` cookies will be updated with each request.
 
 This returns a normal `Response` object:
 ```py
 >>> resp = page.get('https://duckduckgo.com')
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_frgzxwnw_/tmpi9d3ogst_TarContainer/0/30", line 1077, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_frgzxwnw_/tmpi9d3ogst_TarContainer/0/30", line 1077, column 0: CDATA terminal not found*

```diff
@@ -1,51 +1,51 @@
-Metadata-Version: 2.1 Name: hrequests Version: 0.4.2 Summary: Hrequests (human
+Metadata-Version: 2.1 Name: hrequests Version: 0.5.0 Summary: Hrequests (human
 requests) is a simple, configurable, feature-rich, replacement for the Python
 requests library. Home-page: https://github.com/daijro/hrequests License:
 Apache-2.0 Keywords: tls,client,http,scraping,requests,humans,playwright
-Author: daijro Author-email: daijro.dev@gmail.com Requires-Python: >=3.6,<4.0
+Author: daijro Author-email: daijro.dev@gmail.com Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Topic :: Internet :: WWW/
-HTTP Classifier: Topic :: Internet :: WWW/HTTP :: Browsers Classifier: Topic ::
-Software Development :: Libraries :: Python Modules Requires-Dist:
-aioprocessing Requires-Dist: async-class Requires-Dist: fake-headers Requires-
-Dist: gevent Requires-Dist: httpx Requires-Dist: lxml Requires-Dist: msvc-
-runtime ; sys_platform == "win32" Requires-Dist: numpy Requires-Dist: orjson
-Requires-Dist: parse Requires-Dist: playwright Requires-Dist: playwright-
-stealth Requires-Dist: pyquery Requires-Dist: w3lib Requires-Dist: wget
+:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Topic :: Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP ::
+Browsers Classifier: Topic :: Software Development :: Libraries :: Python
+Modules Requires-Dist: aioprocessing Requires-Dist: async-class Requires-Dist:
+fake-headers Requires-Dist: gevent Requires-Dist: httpx Requires-Dist: lxml
+Requires-Dist: msvc-runtime ; sys_platform == "win32" Requires-Dist: numpy
+Requires-Dist: orjson Requires-Dist: parse Requires-Dist: playwright (==1.34.0)
+Requires-Dist: playwright-stealth Requires-Dist: pycryptodome Requires-Dist:
+pyquery Requires-Dist: urllib3 Requires-Dist: w3lib Requires-Dist: wget
 Project-URL: Repository, https://github.com/daijro/hrequests Description-
 Content-Type: text/markdown [https://i.imgur.com/r8GcQW1.png]
                              ***** hrequests *****
   *** [https://img.shields.io/github/license/daijro/hrequests.svg] [https://
-   img.shields.io/badge/python-3.6&#8208;3.11-blue] [PyPI] [PyPI] [https://
+   img.shields.io/badge/python-3.7&#8208;3.11-blue] [PyPI] [PyPI] [https://
   img.shields.io/badge/code%20style-black-black.svg] [https://img.shields.io/
     badge/imports-isort-yellow.svg]Hrequests (human requests) is a simple,
  configurable, feature-rich, replacement for the Python requests library. ***
 ### â¨ Features - Seamless transition between HTTP and headless browsing ð»
 - Integrated fast HTML parser ð - High performance concurrency with gevent
 (*without monkey-patching!*) ð - Replication of browser TLS fingerprints
 ð - JavaScript rendering ð - Supports HTTP/2 ð - Realistic browser
 header generation ð - JSON serializing up to 10x faster than the standard
 library ð ### ð» Browser crawling - Simple & uncomplicated browser
 automation - Human-like cursor movement and typing - Full page screenshots -
 Headless and headful support - No CORS restrictions ### â¡ More - High
 performance â¨ - Minimal dependence on the python standard libraries - Written
 with type safety - 100% threadsafe â¤ï¸ --- # Installation Install via pip:
-```bash pip install hrequests playwright install ``` Other depedencies will be
-downloaded on the first import: ```py >>> import hrequests ``` --- #
-Documentation 1. [Simple Usage](https://github.com/daijro/hrequests#simple-
-usage) 2. [Sessions](https://github.com/daijro/hrequests#sessions) 3.
-[Concurrent & Lazy Requests](https://github.com/daijro/hrequests#concurrent--
-lazy-requests) 4. [HTML Parsing](https://github.com/daijro/hrequests#html-
-parsing) 5. [Browser Automation](https://github.com/daijro/hrequests#browser-
-automation)
+```bash pip install -U hrequests python -m playwright install chromium ```
+Other depedencies will be downloaded on the first import: ```py >>> import
+hrequests ``` --- # Documentation 1. [Simple Usage](https://github.com/daijro/
+hrequests#simple-usage) 2. [Sessions](https://github.com/daijro/
+hrequests#sessions) 3. [Concurrent & Lazy Requests](https://github.com/daijro/
+hrequests#concurrent--lazy-requests) 4. [HTML Parsing](https://github.com/
+daijro/hrequests#html-parsing) 5. [Browser Automation](https://github.com/
+daijro/hrequests#browser-automation)
 ===============================================================================
 ## Simple Usage Here is an example of a simple `get` request: ```py >>> resp =
 hrequests.get('https://www.google.com/') ``` Requests are sent through
 [bogdanfinn's tls-client](https://github.com/bogdanfinn/tls-client) to spoof
 the TLS client fingerprint. This is done automatically, and is completely
 transparent to the user. Other request methods include `post`, `put`, `delete`,
 `head`, `options`, and `patch`. The `Response` object is a near 1:1 replica of
```

