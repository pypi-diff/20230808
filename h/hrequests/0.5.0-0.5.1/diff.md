# Comparing `tmp/hrequests-0.5.0.tar.gz` & `tmp/hrequests-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hrequests-0.5.0.tar", max compression
+gzip compressed data, was "hrequests-0.5.1.tar", max compression
```

## Comparing `hrequests-0.5.0.tar` & `hrequests-0.5.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      327 2023-07-08 02:07:11.571269 hrequests-0.5.0/hrequests/__init__.py
--rw-r--r--   0        0        0      143 2023-07-27 05:36:46.339796 hrequests-0.5.0/hrequests/__version__.py
--rw-r--r--   0        0        0        0 2023-07-02 20:20:07.221972 hrequests-0.5.0/hrequests/bin/__init__.py
--rw-r--r--   0        0        0     1688 2023-07-02 20:40:17.715874 hrequests-0.5.0/hrequests/bin/LICENSE.txt
--rw-r--r--   0        0        0    24019 2023-07-27 04:11:05.106287 hrequests-0.5.0/hrequests/browser.py
--rw-r--r--   0        0        0     2766 2023-07-27 05:28:27.582549 hrequests-0.5.0/hrequests/cffi.py
--rw-r--r--   0        0        0    13695 2023-07-16 05:38:20.704288 hrequests-0.5.0/hrequests/client.py
--rw-r--r--   0        0        0    16943 2023-07-27 04:00:00.788929 hrequests-0.5.0/hrequests/cookies.py
--rw-r--r--   0        0        0      832 2023-07-26 03:24:32.884562 hrequests-0.5.0/hrequests/exceptions.py
--rw-r--r--   0        0        0     3521 2023-07-26 02:48:16.215913 hrequests-0.5.0/hrequests/extensions.py
--rw-r--r--   0        0        0    19506 2023-07-16 09:26:40.532017 hrequests-0.5.0/hrequests/parser.py
--rw-r--r--   0        0        0      374 2023-07-08 02:07:11.641927 hrequests-0.5.0/hrequests/playwright_mock/__init__.py
--rw-r--r--   0        0        0     1163 2023-07-26 16:42:30.741872 hrequests-0.5.0/hrequests/playwright_mock/context.py
--rw-r--r--   0        0        0    12246 2023-07-07 18:42:04.730618 hrequests-0.5.0/hrequests/playwright_mock/element_handle.py
--rw-r--r--   0        0        0     2208 2023-07-08 02:07:11.715693 hrequests-0.5.0/hrequests/playwright_mock/faker.py
--rw-r--r--   0        0        0    16099 2023-07-08 02:07:11.935959 hrequests-0.5.0/hrequests/playwright_mock/frame.py
--rw-r--r--   0        0        0     1579 2023-06-17 22:56:39.629341 hrequests-0.5.0/hrequests/playwright_mock/frame_locator.py
--rw-r--r--   0        0        0      354 2023-06-17 22:56:39.629341 hrequests-0.5.0/hrequests/playwright_mock/js_handle.py
--rw-r--r--   0        0        0     6919 2023-06-18 03:47:56.370585 hrequests-0.5.0/hrequests/playwright_mock/locale.json
--rw-r--r--   0        0        0    12140 2023-06-18 03:49:17.047181 hrequests-0.5.0/hrequests/playwright_mock/locator.py
--rw-r--r--   0        0        0     3454 2023-06-17 23:01:35.605590 hrequests-0.5.0/hrequests/playwright_mock/mouse.py
--rw-r--r--   0        0        0    17529 2023-07-16 04:06:21.948435 hrequests-0.5.0/hrequests/playwright_mock/page.py
--rw-r--r--   0        0        0     2226 2023-07-27 03:05:33.657481 hrequests-0.5.0/hrequests/playwright_mock/playwright_mock.py
--rw-r--r--   0        0        0     3910 2023-07-08 02:07:11.800614 hrequests-0.5.0/hrequests/playwright_mock/proxy_manager.py
--rw-r--r--   0        0        0    13769 2023-07-20 02:12:07.392826 hrequests-0.5.0/hrequests/reqs.py
--rw-r--r--   0        0        0     8645 2023-07-27 03:19:59.329126 hrequests-0.5.0/hrequests/response.py
--rw-r--r--   0        0        0    11917 2023-07-12 07:00:19.769672 hrequests-0.5.0/hrequests/session.py
--rw-r--r--   0        0        0     4715 2023-07-26 07:07:38.574046 hrequests-0.5.0/hrequests/toolbelt.py
--rw-r--r--   0        0        0    11357 2023-07-06 18:41:32.923322 hrequests-0.5.0/LICENSE
--rw-r--r--   0        0        0     1062 2023-07-27 05:36:54.131069 hrequests-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    35059 2023-07-27 05:38:31.115281 hrequests-0.5.0/README.md
--rw-r--r--   0        0        0    35450 1970-01-01 00:00:00.000000 hrequests-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      327 2023-07-08 02:07:11.571269 hrequests-0.5.1/hrequests/__init__.py
+-rw-r--r--   0        0        0      143 2023-08-04 18:30:02.012594 hrequests-0.5.1/hrequests/__version__.py
+-rw-r--r--   0        0        0        0 2023-07-02 20:20:07.221972 hrequests-0.5.1/hrequests/bin/__init__.py
+-rw-r--r--   0        0        0     1688 2023-07-02 20:40:17.715874 hrequests-0.5.1/hrequests/bin/LICENSE.txt
+-rw-r--r--   0        0        0    24019 2023-07-27 04:11:05.106287 hrequests-0.5.1/hrequests/browser.py
+-rw-r--r--   0        0        0     2766 2023-07-27 05:28:27.582549 hrequests-0.5.1/hrequests/cffi.py
+-rw-r--r--   0        0        0    13695 2023-07-16 05:38:20.704288 hrequests-0.5.1/hrequests/client.py
+-rw-r--r--   0        0        0    16943 2023-07-27 04:00:00.788929 hrequests-0.5.1/hrequests/cookies.py
+-rw-r--r--   0        0        0      832 2023-07-26 03:24:32.884562 hrequests-0.5.1/hrequests/exceptions.py
+-rw-r--r--   0        0        0     3521 2023-07-26 02:48:16.215913 hrequests-0.5.1/hrequests/extensions.py
+-rw-r--r--   0        0        0    19506 2023-07-16 09:26:40.532017 hrequests-0.5.1/hrequests/parser.py
+-rw-r--r--   0        0        0      374 2023-07-08 02:07:11.641927 hrequests-0.5.1/hrequests/playwright_mock/__init__.py
+-rw-r--r--   0        0        0     1163 2023-07-26 16:42:30.741872 hrequests-0.5.1/hrequests/playwright_mock/context.py
+-rw-r--r--   0        0        0    12246 2023-07-07 18:42:04.730618 hrequests-0.5.1/hrequests/playwright_mock/element_handle.py
+-rw-r--r--   0        0        0     2208 2023-07-08 02:07:11.715693 hrequests-0.5.1/hrequests/playwright_mock/faker.py
+-rw-r--r--   0        0        0    16099 2023-07-08 02:07:11.935959 hrequests-0.5.1/hrequests/playwright_mock/frame.py
+-rw-r--r--   0        0        0     1579 2023-06-17 22:56:39.629341 hrequests-0.5.1/hrequests/playwright_mock/frame_locator.py
+-rw-r--r--   0        0        0      354 2023-06-17 22:56:39.629341 hrequests-0.5.1/hrequests/playwright_mock/js_handle.py
+-rw-r--r--   0        0        0     6919 2023-06-18 03:47:56.370585 hrequests-0.5.1/hrequests/playwright_mock/locale.json
+-rw-r--r--   0        0        0    12140 2023-06-18 03:49:17.047181 hrequests-0.5.1/hrequests/playwright_mock/locator.py
+-rw-r--r--   0        0        0     3454 2023-06-17 23:01:35.605590 hrequests-0.5.1/hrequests/playwright_mock/mouse.py
+-rw-r--r--   0        0        0    17529 2023-07-16 04:06:21.948435 hrequests-0.5.1/hrequests/playwright_mock/page.py
+-rw-r--r--   0        0        0     2226 2023-07-27 03:05:33.657481 hrequests-0.5.1/hrequests/playwright_mock/playwright_mock.py
+-rw-r--r--   0        0        0     3910 2023-07-08 02:07:11.800614 hrequests-0.5.1/hrequests/playwright_mock/proxy_manager.py
+-rw-r--r--   0        0        0    13769 2023-08-02 01:58:49.061559 hrequests-0.5.1/hrequests/reqs.py
+-rw-r--r--   0        0        0     9568 2023-08-02 04:34:43.306666 hrequests-0.5.1/hrequests/response.py
+-rw-r--r--   0        0        0    11919 2023-08-02 04:49:24.344756 hrequests-0.5.1/hrequests/session.py
+-rw-r--r--   0        0        0     4715 2023-07-26 07:07:38.574046 hrequests-0.5.1/hrequests/toolbelt.py
+-rw-r--r--   0        0        0    11357 2023-07-06 18:41:32.923322 hrequests-0.5.1/LICENSE
+-rw-r--r--   0        0        0     1062 2023-08-04 18:29:54.155287 hrequests-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0    35095 2023-07-27 16:55:04.722183 hrequests-0.5.1/README.md
+-rw-r--r--   0        0        0    35485 1970-01-01 00:00:00.000000 hrequests-0.5.1/PKG-INFO
```

### Comparing `hrequests-0.5.0/hrequests/bin/LICENSE.txt` & `hrequests-0.5.1/hrequests/bin/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hrequests-0.5.0/hrequests/browser.py` & `hrequests-0.5.1/hrequests/browser.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.5.0/hrequests/cffi.py` & `hrequests-0.5.1/hrequests/cffi.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.5.0/hrequests/client.py` & `hrequests-0.5.1/hrequests/client.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.5.0/hrequests/cookies.py` & `hrequests-0.5.1/hrequests/cookies.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.5.0/hrequests/exceptions.py` & `hrequests-0.5.1/hrequests/exceptions.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.5.0/hrequests/extensions.py` & `hrequests-0.5.1/hrequests/extensions.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.5.0/hrequests/parser.py` & `hrequests-0.5.1/hrequests/parser.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.5.0/hrequests/playwright_mock/context.py` & `hrequests-0.5.1/hrequests/playwright_mock/context.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.5.0/hrequests/playwright_mock/element_handle.py` & `hrequests-0.5.1/hrequests/playwright_mock/element_handle.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.5.0/hrequests/playwright_mock/faker.py` & `hrequests-0.5.1/hrequests/playwright_mock/faker.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.5.0/hrequests/playwright_mock/frame.py` & `hrequests-0.5.1/hrequests/playwright_mock/frame.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.5.0/hrequests/playwright_mock/frame_locator.py` & `hrequests-0.5.1/hrequests/playwright_mock/frame_locator.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.5.0/hrequests/playwright_mock/locale.json` & `hrequests-0.5.1/hrequests/playwright_mock/locale.json`

 * *Files identical despite different names*

### Comparing `hrequests-0.5.0/hrequests/playwright_mock/locator.py` & `hrequests-0.5.1/hrequests/playwright_mock/locator.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.5.0/hrequests/playwright_mock/mouse.py` & `hrequests-0.5.1/hrequests/playwright_mock/mouse.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.5.0/hrequests/playwright_mock/page.py` & `hrequests-0.5.1/hrequests/playwright_mock/page.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.5.0/hrequests/playwright_mock/playwright_mock.py` & `hrequests-0.5.1/hrequests/playwright_mock/playwright_mock.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.5.0/hrequests/playwright_mock/proxy_manager.py` & `hrequests-0.5.1/hrequests/playwright_mock/proxy_manager.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.5.0/hrequests/reqs.py` & `hrequests-0.5.1/hrequests/reqs.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.5.0/hrequests/response.py` & `hrequests-0.5.1/hrequests/response.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,25 +8,26 @@
 import orjson
 
 import hrequests
 from hrequests.exceptions import ClientException
 
 from .cookies import RequestsCookieJar
 from .toolbelt import CaseInsensitiveDict, FileUtils
+from urllib.parse import urlparse, ParseResult
 
 
 class ProcessResponse:
     def __init__(
         self,
         session,
         method: str,
         url: str,
         files: Optional[dict] = None,
         allow_redirects: bool = True,
-        chain: bool = False,
+        history: bool = False,
         cookies: Optional[Union[RequestsCookieJar, dict, list]] = None,
         **kwargs,
     ) -> None:
         self.session: 'hrequests.session.TLSSession' = session
         self.method: str = method
         self.url: str = url
         self.allow_redirects: bool = allow_redirects
@@ -45,25 +46,25 @@
                 headers = self.session.headers.copy()
             # else if headers were provided, append Content-Type to those
             elif isinstance(headers, dict):
                 headers = CaseInsensitiveDict(headers)
             headers['Content-Type'] = content_type
             kwargs['headers'] = headers
 
-        self.chain: bool = chain
+        self.history: bool = history
         self.cookies: Optional[Union[RequestsCookieJar, dict, list]] = cookies
         self.kwargs: dict = kwargs
         self.response: Response
 
     def send(self) -> None:
         time: datetime = datetime.now()
-        if self.chain:
-            resp_chain = list(self.generate_chain())
-            self.response = resp_chain[-1]
-            self.response.history = resp_chain[:-1]
+        if self.history:
+            resp_history = list(self.generate_history())
+            self.response = resp_history[-1]
+            self.response.history = resp_history[:-1]
         else:
             self.response = self.execute_request()
         self.response.elapsed = datetime.now() - time
 
     def execute_request(self, redirect: Optional[bool] = None) -> 'Response':
         if redirect is None:
             redirect = self.allow_redirects
@@ -76,20 +77,39 @@
                 **self.kwargs,
             )
         except IOError as e:
             raise ClientException('Connection error') from e
         resp.session = None if self.session.temp else self.session
         return resp
 
-    def generate_chain(self):
+    @staticmethod
+    def _merge_relative(src_url, redir_url):
+        '''merges the netloc of a source url with the path/params/query/fragment of a redirect url'''
+        parsed_red = urlparse(redir_url)
+        # if the redirect url already has a domain and scheme, return with no change
+        if parsed_red.netloc and parsed_red.scheme:
+            return redir_url
+        # parse the source url
+        parsed_src = urlparse(src_url)
+        # rebuild with missing netloc and scheme
+        return ParseResult(
+            scheme=parsed_red.scheme or parsed_src.scheme,
+            netloc=parsed_red.netloc or parsed_src.netloc,
+            path=parsed_red.path,
+            params=parsed_red.params,
+            query=parsed_red.query,
+            fragment=parsed_red.fragment
+        ).geturl()
+
+    def generate_history(self):
         while True:
             resp = self.execute_request(redirect=False)  # don't allow redirects
             yield resp
             if self.allow_redirects and resp.status_code in range(300, 400):
-                self.url = resp.headers['Location']
+                self.url = self._merge_relative(resp.url, resp.headers['Location'])
             else:
                 break
 
 
 @dataclass
 class Response:
     """
```

### Comparing `hrequests-0.5.0/hrequests/session.py` & `hrequests-0.5.1/hrequests/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,15 @@
             url=url,
             data=data,
             files=files,
             headers=headers,
             cookies=cookies,
             json=json,
             allow_redirects=allow_redirects,
-            chain=history,
+            history=history,
             verify=self.verify if verify is None else verify,
             timeout=self.timeout if timeout is None else timeout,
             proxy=proxies,
         )
         proc.send()
         return proc.response
```

### Comparing `hrequests-0.5.0/hrequests/toolbelt.py` & `hrequests-0.5.1/hrequests/toolbelt.py`

 * *Files identical despite different names*

### Comparing `hrequests-0.5.0/LICENSE` & `hrequests-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hrequests-0.5.0/pyproject.toml` & `hrequests-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hrequests"
-version = "0.5.0"
+version = "0.5.1"
 description = "Hrequests (human requests) is a simple, configurable, feature-rich, replacement for the Python requests library."
 authors = ["daijro <daijro.dev@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/daijro/hrequests"
 keywords = ["tls", "client", "http", "scraping", "requests", "humans", "playwright"]
 classifiers = [
```

### Comparing `hrequests-0.5.0/README.md` & `hrequests-0.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 - Realistic browser header generation 🚀
 - JSON serializing up to 10x faster than the standard library 🚀
 
 ### 💻 Browser crawling
 
 - Simple & uncomplicated browser automation
 - Human-like cursor movement and typing
+- Chrome extension support
 - Full page screenshots
 - Headless and headful support
 - No CORS restrictions
 
 ### ⚡ More
 - High performance ✨
 - Minimal dependence on the python standard libraries
@@ -992,15 +993,15 @@
     with resp.render(extensions='C:\\extentions'):
     ```
     Note that these need to be *unpacked* extensions. You can unpack a `.crx` file by changing the file extension to `.zip` and extracting the contents.
 
 Here is an usage example of using a captcha solver:
 
 ```py
->>> with hrequests.render('https://accounts.hcaptcha.com/demo', extensions=['C:\\extentions\\hektcaptcha']):
+>>> with hrequests.render('https://accounts.hcaptcha.com/demo', extensions=['C:\\extentions\\hektcaptcha']) as page:
 ...     page.awaitSelector('.hcaptcha-success')  # wait for captcha to finish
 ...     page.click('input[type=submit]')
 ```
 
 ### Requests & Responses
 
 Requests can also be sent within browser sessions. These operate the same as the standard `hrequests.request`, and will use the browser's cookies and headers. The `BrowserSession` cookies will be updated with each request.
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_phtnlv1a_/tmpjd4w31wc_TarContainer/0/30.md", line 1078, column 3: CDATA terminal not found*

 * *File "/tmp/diffoscope_phtnlv1a_/tmpjd4w31wc_TarContainer/0/30.md", line 1078, column 3: CDATA terminal not found*

```diff
@@ -7,26 +7,26 @@
  configurable, feature-rich, replacement for the Python requests library. ***
 ### â¨ Features - Seamless transition between HTTP and headless browsing ð»
 - Integrated fast HTML parser ð - High performance concurrency with gevent
 (*without monkey-patching!*) ð - Replication of browser TLS fingerprints
 ð - JavaScript rendering ð - Supports HTTP/2 ð - Realistic browser
 header generation ð - JSON serializing up to 10x faster than the standard
 library ð ### ð» Browser crawling - Simple & uncomplicated browser
-automation - Human-like cursor movement and typing - Full page screenshots -
-Headless and headful support - No CORS restrictions ### â¡ More - High
-performance â¨ - Minimal dependence on the python standard libraries - Written
-with type safety - 100% threadsafe â¤ï¸ --- # Installation Install via pip:
-```bash pip install -U hrequests python -m playwright install chromium ```
-Other depedencies will be downloaded on the first import: ```py >>> import
-hrequests ``` --- # Documentation 1. [Simple Usage](https://github.com/daijro/
-hrequests#simple-usage) 2. [Sessions](https://github.com/daijro/
-hrequests#sessions) 3. [Concurrent & Lazy Requests](https://github.com/daijro/
-hrequests#concurrent--lazy-requests) 4. [HTML Parsing](https://github.com/
-daijro/hrequests#html-parsing) 5. [Browser Automation](https://github.com/
-daijro/hrequests#browser-automation)
+automation - Human-like cursor movement and typing - Chrome extension support -
+Full page screenshots - Headless and headful support - No CORS restrictions ###
+â¡ More - High performance â¨ - Minimal dependence on the python standard
+libraries - Written with type safety - 100% threadsafe â¤ï¸ --- #
+Installation Install via pip: ```bash pip install -U hrequests python -
+m playwright install chromium ``` Other depedencies will be downloaded on the
+first import: ```py >>> import hrequests ``` --- # Documentation 1. [Simple
+Usage](https://github.com/daijro/hrequests#simple-usage) 2. [Sessions](https://
+github.com/daijro/hrequests#sessions) 3. [Concurrent & Lazy Requests](https://
+github.com/daijro/hrequests#concurrent--lazy-requests) 4. [HTML Parsing](https:
+//github.com/daijro/hrequests#html-parsing) 5. [Browser Automation](https://
+github.com/daijro/hrequests#browser-automation)
 ===============================================================================
 ## Simple Usage Here is an example of a simple `get` request: ```py >>> resp =
 hrequests.get('https://www.google.com/') ``` Requests are sent through
 [bogdanfinn's tls-client](https://github.com/bogdanfinn/tls-client) to spoof
 the TLS client fingerprint. This is done automatically, and is completely
 transparent to the user. Other request methods include `post`, `put`, `delete`,
 `head`, `options`, and `patch`. The `Response` object is a near 1:1 replica of
```

### Comparing `hrequests-0.5.0/PKG-INFO` & `hrequests-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hrequests
-Version: 0.5.0
+Version: 0.5.1
 Summary: Hrequests (human requests) is a simple, configurable, feature-rich, replacement for the Python requests library.
 Home-page: https://github.com/daijro/hrequests
 License: Apache-2.0
 Keywords: tls,client,http,scraping,requests,humans,playwright
 Author: daijro
 Author-email: daijro.dev@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -79,14 +79,15 @@
 - Realistic browser header generation 🚀
 - JSON serializing up to 10x faster than the standard library 🚀
 
 ### 💻 Browser crawling
 
 - Simple & uncomplicated browser automation
 - Human-like cursor movement and typing
+- Chrome extension support
 - Full page screenshots
 - Headless and headful support
 - No CORS restrictions
 
 ### ⚡ More
 - High performance ✨
 - Minimal dependence on the python standard libraries
@@ -1032,15 +1033,15 @@
     with resp.render(extensions='C:\\extentions'):
     ```
     Note that these need to be *unpacked* extensions. You can unpack a `.crx` file by changing the file extension to `.zip` and extracting the contents.
 
 Here is an usage example of using a captcha solver:
 
 ```py
->>> with hrequests.render('https://accounts.hcaptcha.com/demo', extensions=['C:\\extentions\\hektcaptcha']):
+>>> with hrequests.render('https://accounts.hcaptcha.com/demo', extensions=['C:\\extentions\\hektcaptcha']) as page:
 ...     page.awaitSelector('.hcaptcha-success')  # wait for captcha to finish
 ...     page.click('input[type=submit]')
 ```
 
 ### Requests & Responses
 
 Requests can also be sent within browser sessions. These operate the same as the standard `hrequests.request`, and will use the browser's cookies and headers. The `BrowserSession` cookies will be updated with each request.
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_phtnlv1a_/tmpjd4w31wc_TarContainer/0/31", line 1119, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_phtnlv1a_/tmpjd4w31wc_TarContainer/0/31", line 1119, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hrequests Version: 0.5.0 Summary: Hrequests (human
+Metadata-Version: 2.1 Name: hrequests Version: 0.5.1 Summary: Hrequests (human
 requests) is a simple, configurable, feature-rich, replacement for the Python
 requests library. Home-page: https://github.com/daijro/hrequests License:
 Apache-2.0 Keywords: tls,client,http,scraping,requests,humans,playwright
 Author: daijro Author-email: daijro.dev@gmail.com Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
@@ -26,26 +26,26 @@
  configurable, feature-rich, replacement for the Python requests library. ***
 ### â¨ Features - Seamless transition between HTTP and headless browsing ð»
 - Integrated fast HTML parser ð - High performance concurrency with gevent
 (*without monkey-patching!*) ð - Replication of browser TLS fingerprints
 ð - JavaScript rendering ð - Supports HTTP/2 ð - Realistic browser
 header generation ð - JSON serializing up to 10x faster than the standard
 library ð ### ð» Browser crawling - Simple & uncomplicated browser
-automation - Human-like cursor movement and typing - Full page screenshots -
-Headless and headful support - No CORS restrictions ### â¡ More - High
-performance â¨ - Minimal dependence on the python standard libraries - Written
-with type safety - 100% threadsafe â¤ï¸ --- # Installation Install via pip:
-```bash pip install -U hrequests python -m playwright install chromium ```
-Other depedencies will be downloaded on the first import: ```py >>> import
-hrequests ``` --- # Documentation 1. [Simple Usage](https://github.com/daijro/
-hrequests#simple-usage) 2. [Sessions](https://github.com/daijro/
-hrequests#sessions) 3. [Concurrent & Lazy Requests](https://github.com/daijro/
-hrequests#concurrent--lazy-requests) 4. [HTML Parsing](https://github.com/
-daijro/hrequests#html-parsing) 5. [Browser Automation](https://github.com/
-daijro/hrequests#browser-automation)
+automation - Human-like cursor movement and typing - Chrome extension support -
+Full page screenshots - Headless and headful support - No CORS restrictions ###
+â¡ More - High performance â¨ - Minimal dependence on the python standard
+libraries - Written with type safety - 100% threadsafe â¤ï¸ --- #
+Installation Install via pip: ```bash pip install -U hrequests python -
+m playwright install chromium ``` Other depedencies will be downloaded on the
+first import: ```py >>> import hrequests ``` --- # Documentation 1. [Simple
+Usage](https://github.com/daijro/hrequests#simple-usage) 2. [Sessions](https://
+github.com/daijro/hrequests#sessions) 3. [Concurrent & Lazy Requests](https://
+github.com/daijro/hrequests#concurrent--lazy-requests) 4. [HTML Parsing](https:
+//github.com/daijro/hrequests#html-parsing) 5. [Browser Automation](https://
+github.com/daijro/hrequests#browser-automation)
 ===============================================================================
 ## Simple Usage Here is an example of a simple `get` request: ```py >>> resp =
 hrequests.get('https://www.google.com/') ``` Requests are sent through
 [bogdanfinn's tls-client](https://github.com/bogdanfinn/tls-client) to spoof
 the TLS client fingerprint. This is done automatically, and is completely
 transparent to the user. Other request methods include `post`, `put`, `delete`,
 `head`, `options`, and `patch`. The `Response` object is a near 1:1 replica of
```

