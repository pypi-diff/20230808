# Comparing `tmp/jps_api_wrapper-1.7.0.tar.gz` & `tmp/jps_api_wrapper-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jps_api_wrapper-1.7.0.tar", last modified: Thu Jul 20 17:43:15 2023, max compression
+gzip compressed data, was "jps_api_wrapper-1.8.0.tar", last modified: Tue Aug  8 15:05:31 2023, max compression
```

## Comparing `jps_api_wrapper-1.7.0.tar` & `jps_api_wrapper-1.8.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 17:43:15.314837 jps_api_wrapper-1.7.0/
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-07-20 17:34:54.000000 jps_api_wrapper-1.7.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8112 2023-07-20 17:43:15.314837 jps_api_wrapper-1.7.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6635 2023-07-20 17:34:54.000000 jps_api_wrapper-1.7.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      136 2023-07-20 17:34:54.000000 jps_api_wrapper-1.7.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      757 2023-07-20 17:43:15.314837 jps_api_wrapper-1.7.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 17:43:15.310837 jps_api_wrapper-1.7.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 17:43:15.312837 jps_api_wrapper-1.7.0/src/jps_api_wrapper/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 17:42:45.000000 jps_api_wrapper-1.7.0/src/jps_api_wrapper/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   262861 2023-07-20 17:34:54.000000 jps_api_wrapper-1.7.0/src/jps_api_wrapper/classic.py
--rw-rw-rw-   0 root         (0) root         (0)   318985 2023-07-20 17:34:54.000000 jps_api_wrapper-1.7.0/src/jps_api_wrapper/pro.py
--rw-rw-rw-   0 root         (0) root         (0)    13172 2023-07-20 17:34:54.000000 jps_api_wrapper-1.7.0/src/jps_api_wrapper/request_builder.py
--rw-rw-rw-   0 root         (0) root         (0)     6752 2023-07-20 17:34:54.000000 jps_api_wrapper-1.7.0/src/jps_api_wrapper/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 17:43:15.313837 jps_api_wrapper-1.7.0/src/jps_api_wrapper.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8112 2023-07-20 17:43:15.000000 jps_api_wrapper-1.7.0/src/jps_api_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      454 2023-07-20 17:43:15.000000 jps_api_wrapper-1.7.0/src/jps_api_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 17:43:15.000000 jps_api_wrapper-1.7.0/src/jps_api_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-07-20 17:43:15.000000 jps_api_wrapper-1.7.0/src/jps_api_wrapper.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-20 17:43:15.000000 jps_api_wrapper-1.7.0/src/jps_api_wrapper.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 17:43:15.313837 jps_api_wrapper-1.7.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)   290397 2023-07-20 17:34:54.000000 jps_api_wrapper-1.7.0/tests/test_classic.py
--rw-rw-rw-   0 root         (0) root         (0)   212692 2023-07-20 17:34:54.000000 jps_api_wrapper-1.7.0/tests/test_pro.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:05:31.481794 jps_api_wrapper-1.8.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-07-20 17:34:54.000000 jps_api_wrapper-1.8.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8112 2023-08-08 15:05:31.481794 jps_api_wrapper-1.8.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6635 2023-07-20 17:34:54.000000 jps_api_wrapper-1.8.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      136 2023-07-20 17:34:54.000000 jps_api_wrapper-1.8.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      757 2023-08-08 15:05:31.482794 jps_api_wrapper-1.8.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:05:31.477794 jps_api_wrapper-1.8.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:05:31.479794 jps_api_wrapper-1.8.0/src/jps_api_wrapper/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 15:05:04.000000 jps_api_wrapper-1.8.0/src/jps_api_wrapper/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   262861 2023-07-20 17:34:54.000000 jps_api_wrapper-1.8.0/src/jps_api_wrapper/classic.py
+-rw-rw-rw-   0 root         (0) root         (0)   324202 2023-08-08 14:46:46.000000 jps_api_wrapper-1.8.0/src/jps_api_wrapper/pro.py
+-rw-rw-rw-   0 root         (0) root         (0)    13172 2023-07-20 17:34:54.000000 jps_api_wrapper-1.8.0/src/jps_api_wrapper/request_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)     6752 2023-08-08 14:53:58.000000 jps_api_wrapper-1.8.0/src/jps_api_wrapper/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:05:31.480794 jps_api_wrapper-1.8.0/src/jps_api_wrapper.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8112 2023-08-08 15:05:31.000000 jps_api_wrapper-1.8.0/src/jps_api_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      454 2023-08-08 15:05:31.000000 jps_api_wrapper-1.8.0/src/jps_api_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 15:05:31.000000 jps_api_wrapper-1.8.0/src/jps_api_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-08-08 15:05:31.000000 jps_api_wrapper-1.8.0/src/jps_api_wrapper.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-08-08 15:05:31.000000 jps_api_wrapper-1.8.0/src/jps_api_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:05:31.481794 jps_api_wrapper-1.8.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)   290397 2023-07-20 17:34:54.000000 jps_api_wrapper-1.8.0/tests/test_classic.py
+-rw-rw-rw-   0 root         (0) root         (0)   216898 2023-08-08 14:46:46.000000 jps_api_wrapper-1.8.0/tests/test_pro.py
```

### Comparing `jps_api_wrapper-1.7.0/LICENSE` & `jps_api_wrapper-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jps_api_wrapper-1.7.0/PKG-INFO` & `jps_api_wrapper-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jps_api_wrapper
-Version: 1.7.0
+Version: 1.8.0
 Summary: Jamf Pro Server API Python wrapper
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.6
```

### Comparing `jps_api_wrapper-1.7.0/README.md` & `jps_api_wrapper-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `jps_api_wrapper-1.7.0/setup.cfg` & `jps_api_wrapper-1.8.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = jps_api_wrapper
-version = 1.7.0
+version = 1.8.0
 description = Jamf Pro Server API Python wrapper
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 readme = README.md
 license = MIT
 classifiers = 
 	License :: OSI Approved :: MIT License
```

### Comparing `jps_api_wrapper-1.7.0/src/jps_api_wrapper/classic.py` & `jps_api_wrapper-1.8.0/src/jps_api_wrapper/classic.py`

 * *Files identical despite different names*

### Comparing `jps_api_wrapper-1.7.0/src/jps_api_wrapper/pro.py` & `jps_api_wrapper-1.8.0/src/jps_api_wrapper/pro.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,14 +232,261 @@
         :returns: API authentication information in JSON
         """
         endpoint = "/api/v1/auth"
 
         return self._get(endpoint)
 
     """
+    api-integrations
+    """
+
+    def get_api_integrations(
+        self,
+        page: int = None,
+        page_size: int = None,
+        sort: List[str] = ["id:asc"],
+        filter: str = None,
+    ) -> dict:
+        """
+        Returns all Jamf Pro API integrations with search criteria in JSON
+
+        :param page: Page to return, default page is 0.
+        :param page_size: Page size to return, default page-size is 100.
+        :param sort:
+            Sorting criteria in the format: property:asc/desc. Default sort is
+            ["id:asc"]. Multiple sort criteria are supported and must be
+            separated with a comma.
+
+            Options: id, displayName.
+
+            Example: ["id:desc", "displayName:asc"]
+
+        :param filter:
+            Query in the RSQL format, allowing to filter app titles collection.
+            Default filter is empty query - returning all results for the
+            requested page.
+
+            Options: id, displayName
+
+            Example: 'displayName=="IntegrationName"'
+
+        :returns: All Jamf Pro API integrations in JSON
+        """
+        endpoint = "/api/v1/api-integrations"
+        params = remove_empty_params(
+            {"page": page, "page-size": page_size, "sort": sort, "filter": filter}
+        )
+
+        return self._get(endpoint, params=params)
+
+    def get_api_integration(self, id: Union[int, str]) -> dict:
+        """
+        Returns specified API integration by ID
+
+        :param id: API integration ID
+
+        :returns: API integration information in JSON
+        """
+        endpoint = f"/api/v1/api-integrations/{id}"
+
+        return self._get(endpoint)
+
+    def create_api_integration(self, data: dict) -> dict:
+        """
+        Creates API integration with JSON data
+
+        :param data:
+            JSON data to create API integration with. For syntax information
+            view `Jamf's documentation.
+            <https://developer.jamf.com/jamf-pro/reference/postcreateapiintegration>`__
+
+        :returns: New API integration information in JSON
+        """
+        endpoint = "/api/v1/api-integrations"
+
+        return self._post(endpoint, data)
+
+    def create_api_integration_client_credentials(self, id: Union[int, str]) -> dict:
+        """
+        Creates client credentials for the specified API integration with JSON
+        data
+
+        :param id: API integration ID
+
+        :returns: New API integration client credentials in JSON
+        """
+        endpoint = f"/api/v1/api-integrations/{id}/client-credentials"
+
+        return self._post(endpoint)
+
+    def update_api_integration(self, data: dict, id: Union[int, str]) -> dict:
+        """
+        Updates specified API integrations with JSON data by ID
+
+        :param data:
+            JSON data to update API integration with. For syntax information
+            view `Jamf's documentation.
+            <https://developer.jamf.com/jamf-pro/reference/putupdateapiintegration>`__
+        :param id: API integration ID
+
+        :returns: Updated API integration information in JSON
+        """
+        endpoint = f"/api/v1/api-integrations/{id}"
+
+        return self._put(endpoint, data)
+
+    def delete_api_integration(self, id: Union[int, str]) -> str:
+        """
+        Deletes specified API integration by ID
+
+        :param id: API integration ID
+
+        :returns: Success message stating that the API integration was deleted
+        """
+        endpoint = f"/api/v1/api-integrations/{id}"
+
+        return self._delete(
+            endpoint, success_message=f"API integration {id} successfully deleted."
+        )
+
+    """
+    api-role-privileges
+    """
+
+    def get_api_role_privileges(self) -> dict:
+        """
+        Returns all API role privileges in JSON
+
+        :returns: All API role privileges in JSON
+        """
+        endpoint = "/api/v1/api-role-privileges"
+
+        return self._get(endpoint)
+
+    def get_api_role_privileges_search(self, name: str, limit: int = None) -> dict:
+        """
+        Returns the results of the search of the API role privileges in JSON
+
+        :param name:
+            The partial or complete API role privilege name we are searching
+            for
+        :param limit:
+            Number to limit the results to, defaults to 15
+
+        :returns: List of matching results of the API role privileges in JSON
+        """
+        params = remove_empty_params(
+            {
+                "name": name,
+                "limit": limit,
+            }
+        )
+        endpoint = "/api/v1/api-role-privileges/search"
+
+        return self._get(endpoint, params=params)
+
+    """
+    api-roles
+    """
+
+    def get_api_roles(
+        self,
+        page: int = None,
+        page_size: int = None,
+        sort: List[str] = ["id:asc"],
+        filter: str = None,
+    ) -> dict:
+        """
+        Returns all API roles in JSON
+
+        :param page: Page to return, default page is 0.
+        :param page_size: Page size to return, default page-size is 100.
+        :param sort:
+            Sorting criteria in the format: property:asc/desc. Default sort is
+            ["id:asc"]. Multiple sort criteria are supported and must be
+            separated with a comma.
+
+            Options: id, displayName
+
+            Example: ["id:desc", "displayName:asc"]
+
+        :param filter:
+            Query in the RSQL format, allowing to filter app titles collection.
+            Default filter is empty query - returning all results for the
+            requested page.
+
+            Options: id, displayName
+
+            Example: 'displayName=="myRole"'
+        """
+        endpoint = "/api/v1/api-roles"
+        params = remove_empty_params(
+            {"page": page, "page-size": page_size, "sort": sort, "filter": filter}
+        )
+
+        return self._get(endpoint, params=params)
+
+    def get_api_role(self, id: Union[int, str]) -> dict:
+        """
+        Returns specific API role in JSON by ID
+
+        :param id: API role ID
+
+        :returns: API role information in JSON
+        """
+        endpoint = f"/api/v1/api-roles/{id}"
+
+        return self._get(endpoint)
+
+    def create_api_role(self, data: dict) -> dict:
+        """
+        Creates a new API role with JSON data
+
+        :param data:
+            JSON data to create API role with. For syntax information view
+            `Jamf's documentation.
+            <https://developer.jamf.com/jamf-pro/reference/postcreateapirole>`__
+
+        :returns: New API role information in JSON
+        """
+        endpoint = "/api/v1/api-roles"
+
+        return self._post(endpoint, data)
+
+    def update_api_role(self, data: dict, id: Union[int, str]) -> dict:
+        """
+        Updates specific API role with JSON data by ID
+
+        :param data:
+            JSON data to update API role with. For syntax information view
+            `Jamf's documentation.
+            <https://developer.jamf.com/jamf-pro/reference/putupdateapirole>`__
+        :param id: API role ID
+
+        :returns: Updated API role information in JSON
+        """
+        endpoint = f"/api/v1/api-roles/{id}"
+
+        return self._put(endpoint, data)
+
+    def delete_api_role(self, id: Union[int, str]) -> dict:
+        """
+        Deletes specific API role by ID
+
+        :param id: API role ID
+
+        :returns: Success message str stating that the API role was deleted
+        """
+        endpoint = f"/api/v1/api-roles/{id}"
+
+        return self._delete(
+            endpoint, success_message=f"API role {id} successfully deleted."
+        )
+
+    """
     app-request-preview
     """
 
     def get_app_request_settings(self) -> dict:
         """
         Returns the app request settings in JSON
 
@@ -3040,15 +3287,15 @@
 
     def get_enrollment_settings(self) -> dict:
         """
         Returns Enrollment object and re-enrollment settings
 
         :returns: Enrollment settings information in JSON
         """
-        endpoint = "/api/v2/enrollment"
+        endpoint = "/api/v3/enrollment"
 
         return self._get(endpoint)
 
     def get_enrollment_history(
         self, page: int = None, page_size: int = None, sort: List[str] = None
     ) -> dict:
         """
@@ -3301,15 +3548,15 @@
         :param data:
             JSON data to update the enrollment settings with. For syntax
             information view `Jamf's documentation.
             <https://developer.jamf.com/jamf-pro/reference/put_v2-enrollment>`__
 
         :returns: Updated enrollment settings in JSON
         """
-        endpoint = "/api/v2/enrollment"
+        endpoint = "/api/v3/enrollment"
 
         return self._put(endpoint, data)
 
     def update_enrollment_adue_session_token_settings(self, data: dict) -> dict:
         """
         Updates the account driven user enrollment session token settings
 
@@ -5066,50 +5313,82 @@
 
         :returns: Local Admin Password auto-deploy information in JSON
         """
         endpoint = "/api/v2/local-admin-password/settings"
 
         return self._get(endpoint)
 
+    def get_local_admin_password_pending_rotations(self) -> dict:
+        """
+        Returns information about all devices and usernames currently in the
+        state of a pending LAPS rotation
+
+        :returns: Pending rotations information in JSON
+        """
+        endpoint = "/api/v2/local-admin-password/pending-rotations"
+
+        return self._get(endpoint)
+
     def get_local_admin_password_accounts(self, clientManagementId: str) -> dict:
         """
         Returns a full list of admin accounts that are LAPS capable
 
         :param clientManagementId: Client management ID of target device
 
         :returns:
             All LAPS capable accounts for the device in JSON
         """
         endpoint = f"/api/v2/local-admin-password/{clientManagementId}/accounts"
 
         return self._get(endpoint)
 
-    def get_local_admin_password_user_history(
+    def get_local_admin_password_user_audit(
         self, clientManagementId: str, username: str
     ) -> dict:
         """
         Returns full history of all local admin passwords for a specific
         username on a target device. History will include password, who viewed
         the password and when it was viewed. Get audit history by using the
         client management id and username as the path parameters.
 
         :param clientManagementId: Client management ID of target device
         :param username: Username to view audit information for
 
         :returns:
-            Full history of all local admin passwords used for user on device
-            in JSON
+            LAPS password viewed history for the device and username in jSON
         """
         endpoint = (
             f"/api/v2/local-admin-password/{clientManagementId}/account/"
             f"{username}/audit"
         )
 
         return self._get(endpoint)
 
+    def get_local_admin_password_user_history(
+        self, clientManagementId: str, username: str
+    ) -> dict:
+        """
+        Returns the full history of all for a specific username on a target
+        device. History will include date created, date last seen, expiration
+        time, and rotational status. Get audit history by using the client
+        management id and username as the path parameters.
+
+        :param clientManagementId: Client management ID of target device
+        :param username: Username to view audit information for
+
+        :returns:
+            LAPS historical records for the device and username in JSON
+        """
+        endpoint = (
+            f"/api/v2/local-admin-password/{clientManagementId}/account/"
+            f"{username}/history"
+        )
+
+        return self._get(endpoint)
+
     def get_local_admin_password_user_current(
         self, clientManagementId: str, username: str
     ) -> dict:
         """
         Returns current LAPS password for specified client by using the client
         management id and username as the path parameters. Once the password is
         viewed it will be rotated out with a new password based on the rotation
@@ -5422,14 +5701,37 @@
         """
         params = {"verbose": verbose}
         endpoint = "/api/v1/deploy-package"
 
         return self._post(endpoint, data, params=params)
 
     """
+    mobile-device-apps
+    """
+
+    def create_mobile_device_app_reinstall_config(self, data: dict) -> str:
+        """
+        Creates a redeploy of the managed app configuration for a specific app
+        on a specific device using the $APP_CONFIG_REINSTALL_CODE generated
+        during deployment
+
+        :param data:
+            JSON data to create the redeploy with. For syntax information view
+            `Jamf's documentation.
+            <https://developer.jamf.com/jamf-pro/reference/post_v1-mobile-device-apps-reinstall-app-config>`__
+
+        :returns: Success message stating the app config was redeployed
+        """
+        endpoint = "/api/v1/mobile-device-apps/reinstall-app-config"
+
+        return self._post(
+            endpoint, data, success_message="Mobile device app config redeployed."
+        )
+
+    """
     mobile-device-enrollment-profile
     """
 
     def get_mobile_device_enrollment_profile(self, id: Union[int, str]) -> dict:
         """
         Downloads the MDM enrollment profile to the current users Downloads
         folder by ID
@@ -6419,97 +6721,14 @@
         endpoint = f"/api/v2/patch-policies/{id}/dashboard"
 
         return self._delete(
             endpoint, success_message=f"Patch policy {id} removed from dashboard."
         )
 
     """
-    patch-policies-preview
-    """
-
-    def get_patch_policy_dashboard(self, id: Union[int, str]) -> dict:
-        """
-        .. deprecated:: 1.3.0
-            Use :func:`get_patch_policy_dashboard_v2` instead.
-
-        Returns whether or not the requested patch policy is on the dashboard
-        by ID
-
-        :param id: Patch policy ID
-
-        :returns:
-            Whether or no the request patch policy is on the dashboard in JSON
-        """
-        warnings.warn(
-            (
-                "Pro.get_patch_policy_dashboard has been deprecated by Jamf Pro "
-                "v10.44.0. Use Pro.get_patch_policy_v2() instead."
-            ),
-            category=DeprecationWarning,
-        )
-
-        endpoint = f"/api/patch/patch-policies/{id}/dashboard"
-
-        return self._get(endpoint)
-
-    def create_patch_policy_dashboard(self, id: Union[int, str]) -> str:
-        """
-        .. deprecated:: 1.3.0
-            Use :func:`create_patch_policy_dashboard_v2` instead.
-
-        Adds a patch policy to the dashboard by ID
-
-        :param id: Patch policy ID
-
-        :returns:
-            Success message stating that the patch policy was added to the
-            dashboard
-        """
-        warnings.warn(
-            (
-                "Pro.create_patch_policy_dashboard has been deprecated by Jamf Pro "
-                "v10.44.0. Use Pro.create_patch_policy_v2() instead."
-            ),
-            category=DeprecationWarning,
-        )
-
-        endpoint = f"/api/patch/patch-policies/{id}/dashboard"
-
-        return self._post(
-            endpoint, success_message=f"Patch policy {id} added to dashboard."
-        )
-
-    def delete_patch_policy_dashboard(self, id: Union[int, str]) -> str:
-        """
-        .. deprecated:: 1.3.0
-            Use :func:`delete_patch_policy_dashboard_v2` instead.
-
-        Removes a patch policy from the dashboard by ID
-
-        :param id: Patch policy ID
-
-        :returns:
-            Success message stating that the patch policy was removed from the
-            dashboard
-        """
-        warnings.warn(
-            (
-                "Pro.delete_patch_policy_dashboard has been deprecated by Jamf Pro "
-                "v10.44.0. Use Pro.delete_patch_policy_v2() instead."
-            ),
-            category=DeprecationWarning,
-        )
-
-        endpoint = f"/api/patch/patch-policies/{id}/dashboard"
-
-        return self._delete(
-            endpoint, success_message=f"Patch policy {id} removed from dashboard."
-        )
-
-    """
     patch-policy-logs
     """
 
     def get_patch_policy_logs(
         self,
         id: Union[int, str],
         page: int = None,
@@ -7078,81 +7297,14 @@
             endpoint,
             success_message=(
                 f"Patch software title configuration {id} removed from dashboard."
             ),
         )
 
     """
-    patches-preview
-    """
-
-    def get_patch_dashboards(self) -> dict:
-        """
-        .. deprecated:: 1.3.0
-
-        Returns list of patch IDs on dashboard
-
-        :returns: All patch IDs on the dashboard in JSON
-        """
-        warnings.warn(
-            ("Pro.get_patch_dashboards has been deprecated by Jamf Pro v10.44.0."),
-            category=DeprecationWarning,
-        )
-
-        endpoint = "/api/patch/onDashboard"
-
-        return self._get(endpoint)
-
-    def get_patch_software_title_configuration_id(self, id: Union[int, str]) -> dict:
-        """
-        .. deprecated:: 1.3.0
-
-        Returns the software title configuration ID for the given patch policy
-        by ID
-
-        :param ID: Policy ID
-
-        :returns: Software title configuration for the patch policy in JSON
-        """
-        warnings.warn(
-            (
-                "Pro.get_patch_software_title_configuration_id has been deprecated by "
-                "Jamf Pro v10.44.0."
-            ),
-            category=DeprecationWarning,
-        )
-
-        endpoint = f"/api/patch/obj/policy/{id}/softwareTitleConfigurationId"
-
-        return self._get(endpoint)
-
-    def create_patch_disclaimer_accept(self) -> str:
-        """
-        .. deprecated:: 1.3.0
-
-        Accepts patch reporting disclaimer
-
-        :returns:
-            Success message stating the patch reporting disclaimer was accepted
-        """
-        warnings.warn(
-            (
-                "Pro.create_patch_disclaimer_accept has been deprecated by Jamf Pro "
-                "v10.44.0."
-            ),
-            category=DeprecationWarning,
-        )
-
-        endpoint = "/api/patch/disclaimerAgree"
-
-        return self._post(
-            endpoint, success_message="Patch reporting disclaimer accepted."
-        )
-
-    """
     policies-preview
     """
 
     def get_policy_properties(self) -> dict:
         """
         Returns policy properties
```

### Comparing `jps_api_wrapper-1.7.0/src/jps_api_wrapper/request_builder.py` & `jps_api_wrapper-1.8.0/src/jps_api_wrapper/request_builder.py`

 * *Files identical despite different names*

### Comparing `jps_api_wrapper-1.7.0/src/jps_api_wrapper/utils.py` & `jps_api_wrapper-1.8.0/src/jps_api_wrapper/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     :param params: Supplied parameter values
     :param param_options: List of valid parameter options
 
     :raises InvalidParameterOptions:
         The values that were passed to this parameter do not match the valid
         options.
     """
-    if type(params) == str:
+    if type(params) is str:
         params = [params]
     for param in params:
         if param not in param_options:
             raise InvalidParameterOptions(
                 "The values that were passed to this parameter do not match "
                 "the following valid options:\n"
                 f"{param_options}"
```

### Comparing `jps_api_wrapper-1.7.0/src/jps_api_wrapper.egg-info/PKG-INFO` & `jps_api_wrapper-1.8.0/src/jps_api_wrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jps-api-wrapper
-Version: 1.7.0
+Version: 1.8.0
 Summary: Jamf Pro Server API Python wrapper
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.6
```

### Comparing `jps_api_wrapper-1.7.0/tests/test_classic.py` & `jps_api_wrapper-1.8.0/tests/test_classic.py`

 * *Files identical despite different names*

### Comparing `jps_api_wrapper-1.7.0/tests/test_pro.py` & `jps_api_wrapper-1.8.0/tests/test_pro.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,14 +295,195 @@
     Ensures that get_api_authentication returns JSON data when used
     """
     responses.add(response_builder("GET", jps_url("/api/v1/auth")))
     assert pro.get_api_authentication() == EXPECTED_JSON
 
 
 """
+api-integrations
+"""
+
+
+@responses.activate
+def test_get_api_integrations(pro):
+    """
+    Ensures that get_api_integrations returns JSON data when used without
+    optional params
+    """
+    responses.add(response_builder("GET", jps_url("/api/v1/api-integrations")))
+    assert pro.get_api_integrations() == EXPECTED_JSON
+
+
+@responses.activate
+def test_get_api_integrations_optional_params(pro):
+    """
+    Ensures that get_api_integrations returns JSON data when used with all
+    optional params
+    """
+    responses.add(response_builder("GET", jps_url("/api/v1/api-integrations")))
+    assert (
+        pro.get_api_integrations(
+            0, 100, ["id:desc", "displayName:asc"], 'displayName=="IntegrationName"'
+        )
+        == EXPECTED_JSON
+    )
+
+
+@responses.activate
+def test_get_api_integration(pro):
+    """
+    Ensures that get_api_integration returns JSON data when used
+    """
+    responses.add(response_builder("GET", jps_url("/api/v1/api-integrations/1001")))
+    assert pro.get_api_integration(1001) == EXPECTED_JSON
+
+
+@responses.activate
+def test_create_api_integration(pro):
+    """
+    Ensures that create_api_integration returns JSON data when used
+    """
+    responses.add(response_builder("POST", jps_url("/api/v1/api-integrations")))
+    assert pro.create_api_integration(EXPECTED_JSON) == EXPECTED_JSON
+
+
+@responses.activate
+def test_create_api_integration_client_credentials(pro):
+    """
+    Ensures that create_api_integration_client_credentials returns JSON when
+    used
+    """
+    responses.add(
+        response_builder(
+            "POST", jps_url("/api/v1/api-integrations/1001/client-credentials")
+        )
+    )
+    assert pro.create_api_integration_client_credentials(1001) == EXPECTED_JSON
+
+
+@responses.activate
+def test_update_api_integration(pro):
+    """
+    Ensures that update_api_integration returns JSON when used
+    """
+    responses.add(response_builder("PUT", jps_url("/api/v1/api-integrations/1001")))
+    assert pro.update_api_integration(EXPECTED_JSON, 1001) == EXPECTED_JSON
+
+
+@responses.activate
+def test_delete_api_integration(pro):
+    """
+    Ensures that delete_api_integration returns a success message when used
+    """
+    responses.add(response_builder("DELETE", jps_url("/api/v1/api-integrations/1001")))
+    assert (
+        pro.delete_api_integration(1001) == "API integration 1001 successfully deleted."
+    )
+
+
+"""
+api-role-privileges
+"""
+
+
+@responses.activate
+def test_get_api_role_privileges(pro):
+    """
+    Ensures that get_api_role_privileges returns JSON when used
+    """
+    responses.add(response_builder("GET", jps_url("/api/v1/api-role-privileges")))
+    assert pro.get_api_role_privileges() == EXPECTED_JSON
+
+
+@responses.activate
+def test_get_api_role_privileges_search(pro):
+    """
+    Ensures that get_api_role_privileges_search returns JSON when used without
+    optional params
+    """
+    responses.add(
+        response_builder("GET", jps_url("/api/v1/api-role-privileges/search"))
+    )
+    assert pro.get_api_role_privileges_search("Read") == EXPECTED_JSON
+
+
+@responses.activate
+def test_get_api_role_privileges_search_optional_params(pro):
+    """
+    Ensures that get_api_role_privileges_search returns JSON when used with all
+    optional params
+    """
+    responses.add(
+        response_builder("GET", jps_url("/api/v1/api-role-privileges/search"))
+    )
+    assert pro.get_api_role_privileges_search("Read", 10) == EXPECTED_JSON
+
+
+"""
+api-roles
+"""
+
+
+@responses.activate
+def test_get_api_roles(pro):
+    """
+    Ensures that get_api_roles returns JSON when used without optional params
+    """
+    responses.add(response_builder("GET", jps_url("/api/v1/api-roles")))
+    assert pro.get_api_roles() == EXPECTED_JSON
+
+
+@responses.activate
+def test_get_api_roles_optional_params(pro):
+    """
+    Ensures that get_api_roles returns JSON with all optional params
+    """
+    responses.add(response_builder("GET", jps_url("/api/v1/api-roles")))
+    assert pro.get_api_roles(
+        0, 100, ["id:desc", "displayName:asc"], 'displayName=="myRole"'
+    )
+
+
+@responses.activate
+def test_get_api_role(pro):
+    """
+    Ensures that get_api_role returns JSON when used
+    """
+    responses.add(response_builder("GET", jps_url("/api/v1/api-roles/1001")))
+    assert pro.get_api_role(1001) == EXPECTED_JSON
+
+
+@responses.activate
+def test_create_api_role(pro):
+    """
+    Ensures that create_api_role returns JSON when used
+    """
+    responses.add(response_builder("POST", jps_url("/api/v1/api-roles")))
+    assert pro.create_api_role(EXPECTED_JSON) == EXPECTED_JSON
+
+
+@responses.activate
+def test_update_api_role(pro):
+    """
+    Ensures that update_api_role returns JSON when used
+    """
+    responses.add(response_builder("PUT", jps_url("/api/v1/api-roles/1001")))
+    assert pro.update_api_role(EXPECTED_JSON, 1001) == EXPECTED_JSON
+
+
+@responses.activate
+def test_delete_api_roles(pro):
+    """
+    Ensures that delete_api_role returns a success message when used
+    """
+    responses.add(response_builder("DELETE", jps_url("/api/v1/api-roles/1001")))
+    assert pro.delete_api_role(1001) == "API role 1001 successfully deleted."
+
+
+"""
 app-request-preview
 """
 
 
 @responses.activate
 def test_get_app_request_settings(pro):
     """
@@ -2383,15 +2564,15 @@
 
 
 @responses.activate
 def test_get_enrollment_settings(pro):
     """
     Ensures that get_enrollment_settings returns JSON when used
     """
-    responses.add(response_builder("GET", jps_url("/api/v2/enrollment")))
+    responses.add(response_builder("GET", jps_url("/api/v3/enrollment")))
     assert pro.get_enrollment_settings() == EXPECTED_JSON
 
 
 @responses.activate
 def test_get_enrollment_history(pro):
     """
     Ensures that get_enrollment_history returns JSON when used without
@@ -2559,15 +2740,15 @@
 
 @responses.activate
 def test_update_enrollment_settings(pro):
     """
     Ensures that update_enrollment_settings returns JSON when used with
     required params
     """
-    responses.add(response_builder("PUT", jps_url("/api/v2/enrollment")))
+    responses.add(response_builder("PUT", jps_url("/api/v3/enrollment")))
     assert pro.update_enrollment_settings(EXPECTED_JSON) == EXPECTED_JSON
 
 
 @responses.activate
 def test_update_enrollment_adue_session_token_settings(pro):
     """
     Ensures that update_enrollment_adue_session_token_Settings returns JSON
@@ -4016,43 +4197,75 @@
     responses.add(
         response_builder("GET", jps_url("/api/v2/local-admin-password/settings"))
     )
     assert pro.get_local_admin_password_settings() == EXPECTED_JSON
 
 
 @responses.activate
-def test_get_local_admin_password_user_history(pro):
+def test_get_local_admin_password_pending_rotation(pro):
     """
-    Ensures that get_local_admin_password_user_history returns JSON when used
+    Ensures that get_local_admin_password_pending_rotation returns JSON when
+    used
+    """
+    responses.add(
+        response_builder(
+            "GET", jps_url("/api/v2/local-admin-password/pending-rotations")
+        )
+    )
+    assert pro.get_local_admin_password_pending_rotations() == EXPECTED_JSON
+
+
+@responses.activate
+def test_get_local_admin_password_accounts(pro):
+    """
+    Ensures that get_local_admin_password_accounts returns JSON when used with
+    required params
+    """
+    responses.add(
+        response_builder(
+            "GET", jps_url("/api/v2/local-admin-password/1a2b-3c4d/accounts")
+        )
+    )
+    assert pro.get_local_admin_password_accounts("1a2b-3c4d") == EXPECTED_JSON
+
+
+@responses.activate
+def test_get_local_admin_password_user_audit(pro):
+    """
+    Ensures that get_local_admin_password_user_audit returns JSON when used
     with required params
     """
     responses.add(
         response_builder(
             "GET",
             jps_url("/api/v2/local-admin-password/1a2b-3c4d/account/testuser/audit"),
         )
     )
     assert (
-        pro.get_local_admin_password_user_history("1a2b-3c4d", "testuser")
+        pro.get_local_admin_password_user_audit("1a2b-3c4d", "testuser")
         == EXPECTED_JSON
     )
 
 
 @responses.activate
-def test_get_local_admin_password_accounts(pro):
+def test_get_local_admin_password_user_history(pro):
     """
-    Ensures that get_local_admin_password_accounts returns JSON when used with
-    required params
+    Ensures that get_local_admin_password_user_history returns JSON when used
+    with required params
     """
     responses.add(
         response_builder(
-            "GET", jps_url("/api/v2/local-admin-password/1a2b-3c4d/accounts")
+            "GET",
+            jps_url("/api/v2/local-admin-password/1a2b-3c4d/account/testuser/history"),
         )
     )
-    assert pro.get_local_admin_password_accounts("1a2b-3c4d") == EXPECTED_JSON
+    assert (
+        pro.get_local_admin_password_user_history("1a2b-3c4d", "testuser")
+        == EXPECTED_JSON
+    )
 
 
 @responses.activate
 def test_get_local_admin_password_user_current(pro):
     """
     Ensures that get_local_admin_password_user_current returns JSON when used
     with required params
@@ -4321,14 +4534,35 @@
     optional params
     """
     responses.add(response_builder("POST", jps_url("/api/v1/deploy-package")))
     assert pro.create_mdm_deploy_package(EXPECTED_JSON, True) == EXPECTED_JSON
 
 
 """
+mobile-device-apps
+"""
+
+
+@responses.activate
+def test_create_mobile_device_app_reinstall_config(pro):
+    """
+    Ensures that create_mobile_app_reinstall_config returns JSON when used
+    """
+    responses.add(
+        response_builder(
+            "POST", jps_url("/api/v1/mobile-device-apps/reinstall-app-config")
+        )
+    )
+    assert (
+        pro.create_mobile_device_app_reinstall_config(EXPECTED_JSON)
+        == "Mobile device app config redeployed."
+    )
+
+
+"""
 mobile-device-enrollment-profile
 """
 
 
 @responses.activate
 def test_get_mobile_device_enrollment_profile_NotFound(pro):
     """
@@ -5042,61 +5276,14 @@
     assert (
         pro.delete_patch_policy_dashboard_v2(1001)
         == "Patch policy 1001 removed from dashboard."
     )
 
 
 """
-patch-policies-preview
-"""
-
-
-@responses.activate
-def test_get_patch_policy_dashboard(pro):
-    """
-    Ensures that get_patch_policy_dashboard returns JSON when used with
-    required params
-    """
-    responses.add(
-        response_builder("GET", jps_url("/api/patch/patch-policies/1001/dashboard"))
-    )
-    assert pro.get_patch_policy_dashboard(1001) == EXPECTED_JSON
-
-
-@responses.activate
-def test_create_patch_policy_dashboard(pro):
-    """
-    Ensures that create_patch_policy_dashboard returns JSON when used with
-    required params
-    """
-    responses.add(
-        response_builder("POST", jps_url("/api/patch/patch-policies/1001/dashboard"))
-    )
-    assert (
-        pro.create_patch_policy_dashboard(1001)
-        == "Patch policy 1001 added to dashboard."
-    )
-
-
-@responses.activate
-def test_delete_patch_policy_dashboard(pro):
-    """
-    Ensures that delete_patch_policy_dashboard returns a success message str
-    when used with required params
-    """
-    responses.add(
-        response_builder("DELETE", jps_url("/api/patch/patch-policies/1001/dashboard"))
-    )
-    assert (
-        pro.delete_patch_policy_dashboard(1001)
-        == "Patch policy 1001 removed from dashboard."
-    )
-
-
-"""
 patch-policy-logs
 """
 
 
 @responses.activate
 def test_get_patch_policy_logs(pro):
     """
@@ -5555,53 +5742,14 @@
     assert (
         pro.delete_patch_software_title_configuration_dashboard(1001)
         == "Patch software title configuration 1001 removed from dashboard."
     )
 
 
 """
-patches-preview
-"""
-
-
-@responses.activate
-def test_get_patch_dashboards(pro):
-    """
-    Ensures that get_patch_dashboards returns JSON when used
-    """
-    responses.add(response_builder("GET", jps_url("/api/patch/onDashboard")))
-    assert pro.get_patch_dashboards() == EXPECTED_JSON
-
-
-@responses.activate
-def test_get_patch_software_title_configuration_id(pro):
-    """
-    Ensures that get_patch_software_title_configuration_id returns JSON when
-    used with required params
-    """
-    responses.add(
-        response_builder(
-            "GET", jps_url("/api/patch/obj/policy/1001/softwareTitleConfigurationId")
-        )
-    )
-    assert pro.get_patch_software_title_configuration_id(1001) == EXPECTED_JSON
-
-
-@responses.activate
-def test_create_patch_disclaimer_accept(pro):
-    """
-    Ensures that create_patch_disclaimer_accept returns JSON when used
-    """
-    responses.add(response_builder("POST", jps_url("/api/patch/disclaimerAgree")))
-    assert (
-        pro.create_patch_disclaimer_accept() == "Patch reporting disclaimer accepted."
-    )
-
-
-"""
 policies-preview
 """
 
 
 @responses.activate
 def test_get_policy_properties(pro):
     """
```

