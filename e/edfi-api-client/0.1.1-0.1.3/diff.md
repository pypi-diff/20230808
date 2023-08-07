# Comparing `tmp/edfi_api_client-0.1.1-py3-none-any.whl.zip` & `tmp/edfi_api_client-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 21333 bytes, number of entries: 10
--rw-r--r--  2.0 unx      125 b- defN 22-Dec-01 21:28 edfi_api_client/__init__.py
--rw-r--r--  2.0 unx    14310 b- defN 22-Dec-01 21:28 edfi_api_client/edfi_client.py
--rw-r--r--  2.0 unx    19147 b- defN 23-Jan-27 18:48 edfi_api_client/edfi_endpoint.py
--rw-r--r--  2.0 unx     5491 b- defN 22-Dec-01 21:28 edfi_api_client/edfi_params.py
--rw-r--r--  2.0 unx     1635 b- defN 22-Dec-01 21:28 edfi_api_client/util.py
--rwxrwxrwx  2.0 unx    11357 b- defN 23-Jan-27 18:48 edfi_api_client-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    20004 b- defN 23-Jan-27 18:48 edfi_api_client-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-27 18:48 edfi_api_client-0.1.1.dist-info/WHEEL
--rwxrwxrwx  2.0 unx       16 b- defN 23-Jan-27 18:48 edfi_api_client-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      856 b- defN 23-Jan-27 18:48 edfi_api_client-0.1.1.dist-info/RECORD
-10 files, 73033 bytes uncompressed, 19869 bytes compressed:  72.8%
+Zip file size: 22578 bytes, number of entries: 10
+-rwxrwxrwx  2.0 unx      125 b- defN 22-Nov-04 14:42 edfi_api_client/__init__.py
+-rwxrwxrwx  2.0 unx    14310 b- defN 23-Feb-24 22:20 edfi_api_client/edfi_client.py
+-rwxrwxrwx  2.0 unx    21870 b- defN 23-Mar-10 20:51 edfi_api_client/edfi_endpoint.py
+-rwxrwxrwx  2.0 unx     6210 b- defN 23-Mar-10 20:51 edfi_api_client/edfi_params.py
+-rwxrwxrwx  2.0 unx     1635 b- defN 22-Nov-04 14:42 edfi_api_client/util.py
+-rwxrwxrwx  2.0 unx    11357 b- defN 23-Mar-10 21:29 edfi_api_client-0.1.3.dist-info/LICENSE
+-rwxrwxrwx  2.0 unx    21994 b- defN 23-Mar-10 21:29 edfi_api_client-0.1.3.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Mar-10 21:29 edfi_api_client-0.1.3.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx       16 b- defN 23-Mar-10 21:29 edfi_api_client-0.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      856 b- defN 23-Mar-06 17:38 edfi_api_client-0.1.3.dist-info/RECORD
+10 files, 78465 bytes uncompressed, 21114 bytes compressed:  73.1%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: edfi_api_client/edfi_params.py
 Comment: 
 
 Filename: edfi_api_client/util.py
 Comment: 
 
-Filename: edfi_api_client-0.1.1.dist-info/LICENSE
+Filename: edfi_api_client-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: edfi_api_client-0.1.1.dist-info/METADATA
+Filename: edfi_api_client-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: edfi_api_client-0.1.1.dist-info/WHEEL
+Filename: edfi_api_client-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: edfi_api_client-0.1.1.dist-info/top_level.txt
+Filename: edfi_api_client-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: edfi_api_client-0.1.1.dist-info/RECORD
+Filename: edfi_api_client-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## edfi_api_client/edfi_endpoint.py

```diff
@@ -355,86 +355,141 @@
         page_size: int = 100,
 
         retry_on_failure: bool = False,
         max_retries: int = 5,
         max_wait: int = 500,
 
         step_change_version: bool = False,
-        change_version_step_size: int = 50000
+        change_version_step_size: int = 50000,
+        reverse_paging: bool = True,
     ) -> Iterator[List[dict]]:
         """
         This method completes a series of GET requests, paginating params as necessary based on endpoint.
         Rows are returned as a generator.
 
         :param page_size:
         :param retry_on_failure:
         :param max_retries:
         :param max_wait:
         :param step_change_version:
         :param change_version_step_size:
+        :param reverse_paging:
         :return:
         """
+        self.client.verbose_log(f"[Paged Get Resource] Endpoint  : {self.url}")
+
         # Reset pagination parameters
         paged_params = self.params.copy()
-        paged_params.init_page_by_offset(page_size)
 
-        if step_change_version:
+        ### Prepare pagination variables, depending on type of pagination being used
+        if step_change_version and reverse_paging:
+            self.client.verbose_log(
+                f"[Paged Get Resource] Pagination Method: Change Version Stepping with Reverse-Offset Pagination"
+            )
             paged_params.init_page_by_change_version_step(change_version_step_size)
+            total_count = self._get_total_count(paged_params)
+            paged_params.init_reverse_page_by_offset(total_count, page_size)
 
-        # Begin pagination-loop
-        self.client.verbose_log(f"[Paged Get Resource] Endpoint  : {self.url}")
+        elif step_change_version:
+            self.client.verbose_log(
+                f"[Paged Get Resource] Pagination Method: Change Version Stepping with Offset Pagination"
+            )
+            paged_params.init_page_by_offset(page_size)
+            paged_params.init_page_by_change_version_step(change_version_step_size)
+
+        else:
+            self.client.verbose_log(
+                f"[Paged Get Resource] Pagination Method: Offset Pagination"
+            )
+            paged_params.init_page_by_offset(page_size)
 
+        # Begin pagination-loop
         while True:
+
+            ### GET from the API and yield the resulting JSON payload
             self.client.verbose_log(f"[Paged Get Resource] Parameters: {paged_params}")
 
             if retry_on_failure:
                 res = self._get_response_with_exponential_backoff(
                     self.url, params=paged_params,
                     max_retries=max_retries, max_wait=max_wait
                 )
             else:
                 res = self._get_response(self.url, params=paged_params)
 
-            # If no rows are returned, end pagination.
-            if len(res.json()) == 0:
+            self.client.verbose_log(f"[Paged Get Resource] Retrieved {len(res.json())} rows.")
+            yield res.json()
 
-                if step_change_version:
+            ### Paginate, depending on the method specified in arguments
+            # Reverse offset pagination is only applicable during change-version stepping.
+            if step_change_version and reverse_paging:
+                self.client.verbose_log("[Paged Get Resource] @ Reverse-paginating offset...")
+                try:
+                    paged_params.reverse_page_by_offset()
+                except StopIteration:
+                    self.client.verbose_log(
+                        f"[Paged Get Resource] @ Reverse-paginated into negatives. Stepping change version..."
+                    )
                     try:
-                        self.client.verbose_log(f"[Paged Get Resource] @ Retrieved zero rows. Stepping change version...")
-                        paged_params.page_by_change_version_step()
-                        # This raises a StopIteration if max change version is exceeded.
+                        paged_params.page_by_change_version_step()  # This raises a StopIteration if max change version is exceeded.
+                        total_count = self._get_total_count(paged_params)
+                        paged_params.init_reverse_page_by_offset(total_count, page_size)
                     except StopIteration:
-                        self.client.verbose_log(f"[Paged Get Resource] @ Change version exceeded max. Ending pagination.")
+                        self.client.verbose_log(
+                            f"[Paged Get Resource] @ Change version exceeded max. Ending pagination."
+                        )
                         break
-                else:
-                    self.client.verbose_log(f"[Paged Get Resource] @ Retrieved zero rows. Ending pagination.")
-                    break
 
-            # Otherwise, paginate offset.
             else:
-                self.client.verbose_log(f"[Paged Get Resource] @ Retrieved {len(res.json())} rows. Paging offset...")
-                yield res.json()
-                paged_params.page_by_offset()
+                # If no rows are returned, end pagination.
+                if len(res.json()) == 0:
+
+                    if step_change_version:
+                        try:
+                            self.client.verbose_log(f"[Paged Get Resource] @ Stepping change version...")
+                            paged_params.page_by_change_version_step()  # This raises a StopIteration if max change version is exceeded.
+                        except StopIteration:
+                            self.client.verbose_log(f"[Paged Get Resource] @ Change version exceeded max. Ending pagination.")
+                            break
+                    else:
+                        self.client.verbose_log(f"[Paged Get Resource] @ Retrieved zero rows. Ending pagination.")
+                        break
+
+                # Otherwise, paginate offset.
+                else:
+                    self.client.verbose_log(f"@ Paginating offset...")
+                    paged_params.page_by_offset()
 
 
     def total_count(self):
         """
         Ed-Fi 3 resources/descriptors can be fed an optional 'totalCount' parameter in GETs.
         This returns a 'Total-Count' in the response headers that gives the total number of rows for that resource with the specified params.
         Non-pagination params (i.e., offset and limit) have no impact on the returned total.
 
         :return:
         """
         params = self.params.copy()
-        params['totalCount'] = True
-        params['limit'] = 0
+        return self._get_total_count(params)
 
-        res = self._get_response(self.url, params=params)
-        return int(res.headers.get('Total-Count'))
 
+    def _get_total_count(self, params: EdFiParams):
+        """
+        `total_count()` is accessible by the user and during reverse offset-pagination.
+        This internal helper method prevents code needing to be defined twice.
+
+        :param params:
+        :return:
+        """
+        _params = params.copy()
+        _params['totalCount'] = True
+        _params['limit'] = 0
+
+        res = self._get_response(self.url, params=_params)
+        return int(res.headers.get('Total-Count'))
 
 
 
 class EdFiComposite(EdFiEndpoint):
     """
 
     """
@@ -549,17 +604,18 @@
 
         :param page_size:
         :param retry_on_failure:
         :param max_retries:
         :param max_wait:
         :return:
         """
-        if 'step_change_version' in kwargs or 'change_version_step_size' in kwargs:
+        if 'step_change_version' in kwargs or 'change_version_step_size' in kwargs or 'reverse_paging' in kwargs:
             raise KeyError(
-                "Change versions are not implemented in composites! Remove `step_change_version` and `change_version_step_size` from arguments."
+                "Change versions are not implemented in composites!\n"
+                "Remove `step_change_version`, `change_version_step_size`, and/or `reverse_paging` from arguments."
             )
 
         # Reset pagination parameters
         paged_params = self.params.copy()
         paged_params.init_page_by_offset(page_size)
 
         # Begin pagination-loop
```

## edfi_api_client/edfi_params.py

```diff
@@ -1,8 +1,9 @@
 import logging
+import math
 
 from typing import List, Optional
 
 from edfi_api_client import util
 
 
 class EdFiParams(dict):
@@ -90,30 +91,30 @@
             final_params[util.snake_to_camel(key)] = val
 
         return final_params
 
 
 
     ### Methods for preparing params for pagination and completing pagination
-    def init_page_by_offset(self, page_size: int = 100):
+    def init_page_by_offset(self, page_size: int):
         """
 
         :param page_size:
         :return:
         """
         self.page_size = page_size
 
         if 'limit' in self or 'offset' in self:
             logging.warning("The previously-defined limit and offset will be reset for paging.")
 
         self['limit'] = self.page_size
         self['offset'] = 0
 
 
-    def init_page_by_change_version_step(self, change_version_step_size: int = 50000):
+    def init_page_by_change_version_step(self, change_version_step_size: int):
         """
 
         :param change_version_step_size:
         :return:
         """
         self.change_version_step_size = change_version_step_size
 
@@ -156,7 +157,36 @@
             self['maxChangeVersion'] = min(
                 self['maxChangeVersion'] + self.change_version_step_size,
                 self.max_change_version
             )
 
             # Reset the offset counter for the next window of change versions.
             self['offset'] = 0
+
+
+    def init_reverse_page_by_offset(self, total_count: int, page_size: int):
+        """
+
+        :param total_count:
+        :param page_size:
+        :return:
+        """
+        self.page_size = page_size
+
+        self['limit'] = self.page_size
+        self['offset'] = math.floor(total_count / self.page_size) * self.page_size
+
+
+    def reverse_page_by_offset(self):
+        """
+
+        :return:
+        """
+        if self.page_size is None:
+            raise ValueError(
+                "To reverse-paginate by offset, you must first prepare the class using `init_reverse_page_by_offset()`!"
+            )
+
+        self['offset'] -= self.page_size
+
+        if self['offset'] < 0:
+            raise StopIteration
```

## Comparing `edfi_api_client-0.1.1.dist-info/LICENSE` & `edfi_api_client-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `edfi_api_client-0.1.1.dist-info/METADATA` & `edfi_api_client-0.1.3.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: edfi-api-client
-Version: 0.1.1
+Version: 0.1.3
 Summary: Ed-Fi API client and tools
 Home-page: https://github.com/edanalytics/edfi_api_client
 Author: Erik Joranlien, Jay Kaiser
 Author-email: ejoranlien@edanalytics.org, jkaiser@edanalytics.org
+License: UNKNOWN
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: requests
 
 # Ed-Fi API Client Python Package
 
 ## Quick Guide
 
 ```python
@@ -28,15 +29,15 @@
 for row in staffs.get_rows(page_size=500):
     pass
 
 # Pull all rows for the 'studentStaffAssociations' resource as pages (retrying when given authentication-timeout errors)
 ssa = api.resource('studentStaffAssociations')  # OR 'student_staff_associations'
 for page in ssa.get_pages(retry_on_failure=True):
     pass
-    
+
 # Pull all rows for the enrollment students composite, filtering by section ID
 enrollment_students = api.composite('students', filter_type='sections', filter_id='12345')
 for row in enrollment_students.get_rows():
     pass
 ```
 
 ------
@@ -425,15 +426,15 @@
 
 ```python
 >>> student_rows = students.get_rows(
         page_size=500,           # The limit to pass to the parameters. Overwrites parameter if already defined.
         retry_on_failure=False,  # Reconnect session if request fails and reattempt (e.g., if authentication expires).
         max_retries=5,           # If `retry_on_failure is True`, how many attempts before giving up.
         max_wait=500,            # If `retry_on_failure is True`, max wait time for exponential backoff before giving up.
-    
+
         step_change_version=False,       # Only available for resources/descriptors. See [Change Version Stepping] below.
         change_version_step_size=50000,  # Only available for resources/descriptors. See [Change Version Stepping] below.
     )
 <generator object EdFiEndpoint.get_rows at 0x7f7472650f90>
 
 >>> list(student_rows)
 [Paged Get Resource] Endpoint  : {BASE_URL}/data/v3/ed-fi/students
@@ -575,7 +576,47 @@
 
 **Things to note when using change version stepping:** 
 * Change version stepping usually results in more requests made to the API; however, they are far less likely to overwhelm it as with high offsets.
 * Using change version stepping requires both `min_change_version` and `max_change_version` be defined within either the resource's `params` or `kwargs`.
 If either are undefined, an error is raised.
 * The default `change_version_step_size` is set to `50000`.
 This value is not optimized. Try raising it to send fewer requests to the API.
+
+
+**Important Caveat: API De-synchronization when Change-Version Stepping**
+
+There is a known problem that can occur when pulling from the API using change-version limits and without snapshotting.
+If any rows within the change-version window are updated mid-pull, their change-version is updated and they escape the window.
+When this occurs, all other rows in the window shift to fill the place of the missing row, resulting in rows entering previously-pulled offset-windows and being missed in subsequent calls to the API.
+This leads to a gradual de-synchronization between the API and datalakes built from the API.
+
+
+
+We have added a new offset-pagination method to counteract this bug, known as "reverse paging."
+By default, when `step_change_version=True` in resource pulls, requests are made to the API starting at the greatest offset and iterating backwards until offset zero.
+If a row is updated and a shift occurs mid-pull, one or more rows in the change version may be ingested multiple times, but no rows will be lost altogether.
+
+<details>
+<summary>For example:</summary>
+
+-----
+
+Say there are 15 rows in the `students` resource with change versions between 0 and 20.
+We pull these rows using a page-size of 4.
+
+![EdFiDesync1](https://github.com/edanalytics/edfi_api_client/raw/main/images/changeversion_desync1.png)
+
+Say that before our fourth (and final) API call, record number 6 is updated and leaves the change-version window.
+Records 7 through 15 will shift to fill its place.
+When this occurs, record number 13 will shift from page 4 into a page that has already been ingested.
+Therefore, it will be missed from the final output.
+
+![EdFiDesync2](https://github.com/edanalytics/edfi_api_client/raw/main/images/changeversion_desync2.png)
+
+Using reverse-paging, page 4 will be ingested first. When record number 6 is updated and the rows shift, record 13 will move into page 3 and will be ingested a second time.
+However, this row will not be lost.
+
+-----
+
+</details>
+
+
```

## Comparing `edfi_api_client-0.1.1.dist-info/RECORD` & `edfi_api_client-0.1.3.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 edfi_api_client/__init__.py,sha256=JnJMJ0DCcKxZ7Quufh1m4TFa2H3cgYIpwfFBPVANF1A,125
 edfi_api_client/edfi_client.py,sha256=LrCdHy_YrdASvh5XUWM3wPIu1L9btLhWMOJfjBv5ny0,14310
-edfi_api_client/edfi_endpoint.py,sha256=GL0ubmrfBnnpKyWNdolbBg3Ge18WGji7qsTlJ55IfKg,19147
-edfi_api_client/edfi_params.py,sha256=ZHvJvdvJ2JLWupMSqxWIDSBbJtWxvJB9hFyy0sZDcdo,5491
+edfi_api_client/edfi_endpoint.py,sha256=39li0mHtyk5AetvXnur4XmomhWiHgkrDHhqxrECcBYo,21870
+edfi_api_client/edfi_params.py,sha256=A7HD9KTho1DW9zEVRPz0J_aYYDQADNxQUf_2bfN3Lg8,6210
 edfi_api_client/util.py,sha256=m1IRdDRE-EriL1XYQW7Lsi9Dnp-lXBq6xMs-FRb8fJA,1635
-edfi_api_client-0.1.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-edfi_api_client-0.1.1.dist-info/METADATA,sha256=fboYgESvXBBaWLVQW7HN6ZFMUqwfz7yRKfbMf3OGhSM,20004
-edfi_api_client-0.1.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-edfi_api_client-0.1.1.dist-info/top_level.txt,sha256=I0RTU6qPcDdmlDR1HmAcZnSymrkKcL_ZeWsbUViiKhQ,16
-edfi_api_client-0.1.1.dist-info/RECORD,,
+edfi_api_client-0.1.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+edfi_api_client-0.1.3.dist-info/METADATA,sha256=RyVUv9mu-ca-Wcr4RdqMEJSuSmvLXjOaA_pnzttGd38,21994
+edfi_api_client-0.1.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+edfi_api_client-0.1.3.dist-info/top_level.txt,sha256=I0RTU6qPcDdmlDR1HmAcZnSymrkKcL_ZeWsbUViiKhQ,16
+edfi_api_client-0.1.3.dist-info/RECORD,,
```

