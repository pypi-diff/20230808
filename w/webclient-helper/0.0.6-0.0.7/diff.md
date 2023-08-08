# Comparing `tmp/webclient_helper-0.0.6-py3-none-any.whl.zip` & `tmp/webclient_helper-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 8476 bytes, number of entries: 7
+Zip file size: 8812 bytes, number of entries: 7
 -rw-rw-r--  2.0 unx     7367 b- defN 22-Aug-18 15:47 webclient_helper/__init__.py
--rw-rw-r--  2.0 unx    10132 b- defN 21-Sep-28 13:06 webclient_helper/client.py
--rw-rw-r--  2.0 unx      608 b- defN 23-Jul-10 04:46 webclient_helper-0.0.6.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx     8516 b- defN 23-Jul-10 04:46 webclient_helper-0.0.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-10 04:46 webclient_helper-0.0.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx       17 b- defN 23-Jul-10 04:46 webclient_helper-0.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      603 b- defN 23-Jul-10 04:46 webclient_helper-0.0.6.dist-info/RECORD
-7 files, 27335 bytes uncompressed, 7398 bytes compressed:  72.9%
+-rw-rw-r--  2.0 unx    13990 b- defN 23-Aug-08 10:48 webclient_helper/client.py
+-rw-rw-r--  2.0 unx      608 b- defN 23-Aug-08 11:05 webclient_helper-0.0.7.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx     9451 b- defN 23-Aug-08 11:05 webclient_helper-0.0.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Aug-08 11:05 webclient_helper-0.0.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       17 b- defN 23-Aug-08 11:05 webclient_helper-0.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      603 b- defN 23-Aug-08 11:05 webclient_helper-0.0.7.dist-info/RECORD
+7 files, 32128 bytes uncompressed, 7734 bytes compressed:  75.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: webclient_helper/__init__.py
 Comment: 
 
 Filename: webclient_helper/client.py
 Comment: 
 
-Filename: webclient_helper-0.0.6.dist-info/LICENSE.txt
+Filename: webclient_helper-0.0.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: webclient_helper-0.0.6.dist-info/METADATA
+Filename: webclient_helper-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: webclient_helper-0.0.6.dist-info/WHEEL
+Filename: webclient_helper-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: webclient_helper-0.0.6.dist-info/top_level.txt
+Filename: webclient_helper-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: webclient_helper-0.0.6.dist-info/RECORD
+Filename: webclient_helper-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## webclient_helper/client.py

```diff
@@ -54,28 +54,29 @@
         self._extra_headers = extra_headers
         self._history = []
         self.set_session()
 
     def login(self):
         pass
 
+    @property
     def is_login_defined(self):
         """Return True if a login method is defined"""
         return inspect.getsource(self.login) != '    def login(self):\n        pass\n'
 
     def _set_auth_header(self):
         """Add "Authorization" header on session if self._token is set"""
         if self._token:
             self.session.headers.update({
                 'Authorization': '{} {}'.format(self._token_type, self._token)
             })
 
     def set_session(self):
         """Get a new session object for self.session and invoke login method"""
-        if self.is_login_defined():
+        if self.is_login_defined:
             self.session = wh.new_requests_session(
                 user_agent=self._user_agent,
                 content_type=self._content_type,
                 extra_headers=self._extra_headers
             )
             self.login()
         else:
@@ -86,185 +87,302 @@
                 content_type=self._content_type,
                 extra_headers=self._extra_headers
             )
         if self._token:
             assert self._token_type is not None, "self._token is set, but not self._token_type"
         self._set_auth_header()
 
-    def OPTIONS(self, url, headers=None, debug=False, **kwargs):
+    def OPTIONS(self, url, headers=None, debug=False, retry=False, **kwargs):
         """Send a OPTIONS request and return response object
 
         - url: url/endpoint
         - headers: dict of headers to update on the session before making request
         - debug: if True, enter debugger before returning
+        - retry: if True and initial response is "401 Unauthorized", call
+          self.set_session() and try again
 
         Other kwargs are passed to webclient_helper.session_method
         """
+        if url.startswith('/') and self._base_url:
+            url = self._base_url + url
+
         response = wh.session_method(
             'options',
             url,
             session=self.session,
             headers=headers,
             debug=debug,
             **kwargs
         )
+        if retry and response.status_code == 401:
+            self.set_session()
+            response = wh.session_method(
+                'options',
+                url,
+                session=self.session,
+                headers=headers,
+                debug=debug,
+                **kwargs
+            )
+
         self._history.append({
             'caller': inspect.getouterframes(inspect.currentframe(), 2)[1][3],
             'summary': wh.get_summary_from_response(response),
             'response': response
         })
         return response
 
-    def HEAD(self, url, headers=None, debug=False, **kwargs):
+    def HEAD(self, url, headers=None, debug=False, retry=False, **kwargs):
         """Send a HEAD request and return response object
 
         - url: url/endpoint
         - headers: dict of headers to update on the session before making request
         - debug: if True, enter debugger before returning
+        - retry: if True and initial response is "401 Unauthorized", call
+          self.set_session() and try again
 
         Other kwargs are passed to webclient_helper.session_method
         """
+        if url.startswith('/') and self._base_url:
+            url = self._base_url + url
+
         response = wh.session_method(
             'head',
             url,
             session=self.session,
             headers=headers,
             debug=debug,
             **kwargs
         )
+        if retry and response.status_code == 401:
+            self.set_session()
+            response = wh.session_method(
+                'head',
+                url,
+                session=self.session,
+                headers=headers,
+                debug=debug,
+                **kwargs
+            )
+
         self._history.append({
             'caller': inspect.getouterframes(inspect.currentframe(), 2)[1][3],
             'summary': wh.get_summary_from_response(response),
             'response': response
         })
         return response
 
-    def GET(self, url, headers=None, params=None, debug=False, **kwargs):
+    def GET(self, url, headers=None, params=None, debug=False, retry=False, **kwargs):
         """Send a GET request and return response object
 
         - url: url/endpoint
         - headers: dict of headers to update on the session before making request
         - params: a dict with query string vars and values
         - debug: if True, enter debugger before returning
+        - retry: if True and initial response is "401 Unauthorized", call
+          self.set_session() and try again
 
         Other kwargs are passed to webclient_helper.session_method
         """
+        if url.startswith('/') and self._base_url:
+            url = self._base_url + url
+
         response = wh.session_method(
             'get',
             url,
             session=self.session,
             headers=headers,
             params=params,
             debug=debug,
             **kwargs
         )
+        if retry and response.status_code == 401:
+            self.set_session()
+            response = wh.session_method(
+                'get',
+                url,
+                session=self.session,
+                headers=headers,
+                params=params,
+                debug=debug,
+                **kwargs
+            )
+
         self._history.append({
             'caller': inspect.getouterframes(inspect.currentframe(), 2)[1][3],
             'summary': wh.get_summary_from_response(response),
             'response': response
         })
         return response
 
-    def POST(self, url, headers=None, data=None, json=None, debug=False, **kwargs):
+    def POST(self, url, headers=None, data=None, json=None, debug=False, retry=False, **kwargs):
         """Send a POST request and return response object
 
         - url: url/endpoint
         - headers: dict of headers to update on the session before making request
         - data: a dict to send in the body (non-JSON)
         - json: a dict to send in the body
         - debug: if True, enter debugger before returning
+        - retry: if True and initial response is "401 Unauthorized", call
+          self.set_session() and try again
 
         Other kwargs are passed to webclient_helper.session_method
         """
+        if url.startswith('/') and self._base_url:
+            url = self._base_url + url
+
         response = wh.session_method(
             'post',
             url,
             session=self.session,
             headers=headers,
             data=data,
             json=json,
             debug=debug,
             **kwargs
         )
+        if retry and response.status_code == 401:
+            self.set_session()
+            response = wh.session_method(
+                'post',
+                url,
+                session=self.session,
+                headers=headers,
+                data=data,
+                json=json,
+                debug=debug,
+                **kwargs
+            )
+
         self._history.append({
             'caller': inspect.getouterframes(inspect.currentframe(), 2)[1][3],
             'summary': wh.get_summary_from_response(response),
             'response': response
         })
         return response
 
-    def PUT(self, url, headers=None, data=None, debug=False, **kwargs):
+    def PUT(self, url, headers=None, data=None, debug=False, retry=False, **kwargs):
         """Send a PUT request and return response object
 
         - url: url/endpoint
         - headers: dict of headers to update on the session before making request
         - data: a dict to send in the body (non-JSON)
         - debug: if True, enter debugger before returning
+        - retry: if True and initial response is "401 Unauthorized", call
+          self.set_session() and try again
 
         Other kwargs are passed to webclient_helper.session_method
         """
+        if url.startswith('/') and self._base_url:
+            url = self._base_url + url
+
         response = wh.session_method(
             'put',
             url,
             session=self.session,
             headers=headers,
             data=data,
             debug=debug,
             **kwargs
         )
+        if retry and response.status_code == 401:
+            self.set_session()
+            response = wh.session_method(
+                'put',
+                url,
+                session=self.session,
+                headers=headers,
+                data=data,
+                debug=debug,
+                **kwargs
+            )
+
         self._history.append({
             'caller': inspect.getouterframes(inspect.currentframe(), 2)[1][3],
             'summary': wh.get_summary_from_response(response),
             'response': response
         })
         return response
 
-    def PATCH(self, url, headers=None, data=None, debug=False, **kwargs):
+    def PATCH(self, url, headers=None, data=None, debug=False, retry=False, **kwargs):
         """Send a PATCH request and return response object
 
         - url: url/endpoint
         - headers: dict of headers to update on the session before making request
         - data: a dict to send in the body (non-JSON)
         - debug: if True, enter debugger before returning
+        - retry: if True and initial response is "401 Unauthorized", call
+          self.set_session() and try again
 
         Other kwargs are passed to webclient_helper.session_method
         """
+        if url.startswith('/') and self._base_url:
+            url = self._base_url + url
+
         response = wh.session_method(
             'patch',
             url,
             session=self.session,
             headers=headers,
             data=data,
             debug=debug,
             **kwargs
         )
+        if retry and response.status_code == 401:
+            self.set_session()
+            response = wh.session_method(
+                'patch',
+                url,
+                session=self.session,
+                headers=headers,
+                data=data,
+                debug=debug,
+                **kwargs
+            )
+
         self._history.append({
             'caller': inspect.getouterframes(inspect.currentframe(), 2)[1][3],
             'summary': wh.get_summary_from_response(response),
             'response': response
         })
         return response
 
-    def DELETE(self, url, headers=None, debug=False, **kwargs):
+    def DELETE(self, url, headers=None, debug=False, retry=False, **kwargs):
         """Send a DELETE request and return response object
 
         - url: url/endpoint
         - headers: dict of headers to update on the session before making request
         - debug: if True, enter debugger before returning
+        - retry: if True and initial response is "401 Unauthorized", call
+          self.set_session() and try again
 
         Other kwargs are passed to webclient_helper.session_method
         """
+        if url.startswith('/') and self._base_url:
+            url = self._base_url + url
+
         response = wh.session_method(
             'delete',
             url,
             session=self.session,
             headers=headers,
             debug=debug,
             **kwargs
         )
+        if retry and response.status_code == 401:
+            self.set_session()
+            response = wh.session_method(
+                'delete',
+                url,
+                session=self.session,
+                headers=headers,
+                debug=debug,
+                **kwargs
+            )
+
         self._history.append({
             'caller': inspect.getouterframes(inspect.currentframe(), 2)[1][3],
             'summary': wh.get_summary_from_response(response),
             'response': response
         })
         return response
```

## Comparing `webclient_helper-0.0.6.dist-info/LICENSE.txt` & `webclient_helper-0.0.7.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `webclient_helper-0.0.6.dist-info/METADATA` & `webclient_helper-0.0.7.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: webclient-helper
-Version: 0.0.6
+Version: 0.0.7
 Summary: Helpful WebClient class to interact with APIs on the web
 Home-page: https://github.com/kenjyco/webclient-helper
 Author: Ken
 Author-email: kenjyco@gmail.com
 License: MIT
-Download-URL: https://github.com/kenjyco/webclient-helper/tarball/v0.0.6
+Download-URL: https://github.com/kenjyco/webclient-helper/tarball/v0.0.7
 Keywords: webclient,api,requests,soup,beautifulsoup,lxml,http,rest,helper,kenjyco
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -103,79 +103,93 @@
            - user_agent: if specified, set "User-Agent" header
            - content_type: content type for requests
            - extra_headers: a dict of extra headers to set on the session
 
            If no login method is defined, any supplied username/password will be
            passed to new_requests_session (for basic auth)
 
-       OPTIONS(self, url, headers=None, debug=False, **kwargs)
+       OPTIONS(self, url, headers=None, debug=False, retry=False, **kwargs)
            Send a OPTIONS request and return response object
 
            - url: url/endpoint
            - headers: dict of headers to update on the session before making request
            - debug: if True, enter debugger before returning
+           - retry: if True and initial response is "401 Unauthorized", call
+             self.set_session() and try again
 
            Other kwargs are passed to webclient_helper.session_method
 
-       HEAD(self, url, headers=None, debug=False, **kwargs)
+       HEAD(self, url, headers=None, debug=False, retry=False, **kwargs)
            Send a HEAD request and return response object
 
            - url: url/endpoint
            - headers: dict of headers to update on the session before making request
            - debug: if True, enter debugger before returning
+           - retry: if True and initial response is "401 Unauthorized", call
+             self.set_session() and try again
 
            Other kwargs are passed to webclient_helper.session_method
 
-       GET(self, url, headers=None, params=None, debug=False, **kwargs)
+       GET(self, url, headers=None, params=None, debug=False, retry=False, **kwargs)
            Send a GET request and return response object
 
            - url: url/endpoint
            - headers: dict of headers to update on the session before making request
            - params: a dict with query string vars and values
            - debug: if True, enter debugger before returning
+           - retry: if True and initial response is "401 Unauthorized", call
+             self.set_session() and try again
 
            Other kwargs are passed to webclient_helper.session_method
 
-       POST(self, url, headers=None, data=None, json=None, debug=False, **kwargs)
+       POST(self, url, headers=None, data=None, json=None, debug=False, retry=False, **kwargs)
            Send a POST request and return response object
 
            - url: url/endpoint
            - headers: dict of headers to update on the session before making request
            - data: a dict to send in the body (non-JSON)
            - json: a dict to send in the body
            - debug: if True, enter debugger before returning
+           - retry: if True and initial response is "401 Unauthorized", call
+             self.set_session() and try again
 
            Other kwargs are passed to webclient_helper.session_method
 
-       PUT(self, url, headers=None, data=None, debug=False, **kwargs)
+       PUT(self, url, headers=None, data=None, debug=False, retry=False, **kwargs)
            Send a PUT request and return response object
 
            - url: url/endpoint
            - headers: dict of headers to update on the session before making request
            - data: a dict to send in the body (non-JSON)
            - debug: if True, enter debugger before returning
+           - retry: if True and initial response is "401 Unauthorized", call
+             self.set_session() and try again
 
            Other kwargs are passed to webclient_helper.session_method
 
-       PATCH(self, url, headers=None, data=None, debug=False, **kwargs)
+       PATCH(self, url, headers=None, data=None, debug=False, retry=False, **kwargs)
            Send a PATCH request and return response object
 
            - url: url/endpoint
            - headers: dict of headers to update on the session before making request
            - data: a dict to send in the body (non-JSON)
            - debug: if True, enter debugger before returning
+           - retry: if True and initial response is "401 Unauthorized", call
+             self.set_session() and try again
 
            Other kwargs are passed to webclient_helper.session_method
 
-       DELETE(self, url, headers=None, debug=False, **kwargs)
+       DELETE(self, url, headers=None, debug=False, retry=False, **kwargs)
            Send a DELETE request and return response object
 
            - url: url/endpoint
            - headers: dict of headers to update on the session before making request
            - debug: if True, enter debugger before returning
+           - retry: if True and initial response is "401 Unauthorized", call
+             self.set_session() and try again
 
            Other kwargs are passed to webclient_helper.session_method
 
        history_explorer(self, return_selections=False)
            Select responses from history to explore in ipython (if ipython installed)
 
            - return_selections: if True, return the selections from history
@@ -225,15 +239,15 @@
                json=data
            )
            self._token = response.json().get('access_token')
            self._token_type = 'Bearer'
 
        def get_something(self, params=None, debug=False):
            return self.GET(
-               self._base_url + '/api/something',
+               '/api/something',
                params=params,
                debug=debug
            )
 
 
    some_client = SomeClient(
        username='myuser',
```

## Comparing `webclient_helper-0.0.6.dist-info/RECORD` & `webclient_helper-0.0.7.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 webclient_helper/__init__.py,sha256=cRkOx_vpF8ZOYD_kXmXH39gYwNAZvqWKPEHvjeyg8GQ,7367
-webclient_helper/client.py,sha256=QnRGhKWHIpob-kllmQ4LQ9I7uasDqIfHZPvH_zmyQIg,10132
-webclient_helper-0.0.6.dist-info/LICENSE.txt,sha256=INpf6xK6c1YT-PmCXwO_CNA-XdHaEbLGX4UWX2mIHHk,608
-webclient_helper-0.0.6.dist-info/METADATA,sha256=6zAlIJO6Q-F5mxfK8kUCq6InsfdGQKCv25pBKX573bA,8516
-webclient_helper-0.0.6.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-webclient_helper-0.0.6.dist-info/top_level.txt,sha256=Khq9ECpPecSzsRYLSD2ub0wdFIVCWkX9w72iEMK28Zg,17
-webclient_helper-0.0.6.dist-info/RECORD,,
+webclient_helper/client.py,sha256=pI86JXy7llO8FnrE9i7wgTKGO2ACTnHWIwBJTZYxLQ0,13990
+webclient_helper-0.0.7.dist-info/LICENSE.txt,sha256=INpf6xK6c1YT-PmCXwO_CNA-XdHaEbLGX4UWX2mIHHk,608
+webclient_helper-0.0.7.dist-info/METADATA,sha256=W53kOAyNi1mfYAD7TF7pqRqYQh-lwYNcQ-2ppoikHHw,9451
+webclient_helper-0.0.7.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+webclient_helper-0.0.7.dist-info/top_level.txt,sha256=Khq9ECpPecSzsRYLSD2ub0wdFIVCWkX9w72iEMK28Zg,17
+webclient_helper-0.0.7.dist-info/RECORD,,
```

