# Comparing `tmp/canonicalwebteam_store_base-0.0.5.tar.gz` & `tmp/canonicalwebteam_store_base-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canonicalwebteam_store_base-0.0.5.tar", max compression
+gzip compressed data, was "canonicalwebteam_store_base-0.0.6.tar", max compression
```

## Comparing `canonicalwebteam_store_base-0.0.5.tar` & `canonicalwebteam_store_base-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35149 2023-07-13 16:59:42.819586 canonicalwebteam_store_base-0.0.5/LICENSE
--rw-r--r--   0        0        0     1304 2023-07-13 16:59:42.819586 canonicalwebteam_store_base-0.0.5/README.md
--rw-r--r--   0        0        0        0 2023-07-13 16:59:42.819586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/__init__.py
--rw-r--r--   0        0        0     1424 2023-07-13 16:59:42.819586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/app.py
--rw-r--r--   0        0        0        0 2023-07-13 16:59:42.819586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/auth/__init__.py
--rw-r--r--   0        0        0      385 2023-07-13 16:59:42.819586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/auth/authentication.py
--rw-r--r--   0        0        0     1656 2023-07-13 16:59:42.819586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/auth/logic.py
--rw-r--r--   0        0        0     3723 2023-07-13 16:59:42.819586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/auth/views.py
--rw-r--r--   0        0        0    27069 2023-07-13 16:59:42.819586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/data/licenses.json
--rw-r--r--   0        0        0     2745 2023-07-13 16:59:42.819586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/handlers.py
--rw-r--r--   0        0        0        0 2023-07-13 16:59:42.819586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/packages/__init__.py
--rw-r--r--   0        0        0    11998 2023-07-13 16:59:42.819586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/packages/logic.py
--rw-r--r--   0        0        0     2665 2023-07-13 16:59:42.819586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/packages/views.py
--rw-r--r--   0        0        0      201 2023-07-13 16:59:42.823586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/sample_blueprint/views.py
--rw-r--r--   0        0        0        0 2023-07-13 16:59:42.823586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/utils/__init__.py
--rw-r--r--   0        0        0     1094 2023-07-13 16:59:42.823586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/utils/config.py
--rw-r--r--   0        0        0      166 2023-07-13 16:59:42.823586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/utils/constants.py
--rw-r--r--   0        0        0      433 2023-07-13 16:59:42.823586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/utils/decorators.py
--rw-r--r--   0        0        0       61 2023-07-13 16:59:42.823586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/utils/extensions.py
--rw-r--r--   0        0        0     4608 2023-07-13 16:59:42.823586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/utils/helpers.py
--rw-r--r--   0        0        0       25 2023-07-13 16:59:42.823586 canonicalwebteam_store_base-0.0.5/canonicalwebteam/templates/storebase.html
--rw-r--r--   0        0        0     1050 2023-07-13 16:59:42.823586 canonicalwebteam_store_base-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 canonicalwebteam_store_base-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-08 14:33:39.059889 canonicalwebteam_store_base-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1304 2023-08-08 14:33:39.063889 canonicalwebteam_store_base-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2023-08-08 14:33:39.063889 canonicalwebteam_store_base-0.0.6/canonicalwebteam/store_base/__init__.py
+-rw-r--r--   0        0        0     1424 2023-08-08 14:33:39.063889 canonicalwebteam_store_base-0.0.6/canonicalwebteam/store_base/app.py
+-rw-r--r--   0        0        0        0 2023-08-08 14:33:39.063889 canonicalwebteam_store_base-0.0.6/canonicalwebteam/store_base/auth/__init__.py
+-rw-r--r--   0        0        0      385 2023-08-08 14:33:39.063889 canonicalwebteam_store_base-0.0.6/canonicalwebteam/store_base/auth/authentication.py
+-rw-r--r--   0        0        0     1656 2023-08-08 14:33:39.063889 canonicalwebteam_store_base-0.0.6/canonicalwebteam/store_base/auth/logic.py
+-rw-r--r--   0        0        0     3723 2023-08-08 14:33:39.063889 canonicalwebteam_store_base-0.0.6/canonicalwebteam/store_base/auth/views.py
+-rw-r--r--   0        0        0    27069 2023-08-08 14:33:39.063889 canonicalwebteam_store_base-0.0.6/canonicalwebteam/store_base/data/licenses.json
+-rw-r--r--   0        0        0     2745 2023-08-08 14:33:39.063889 canonicalwebteam_store_base-0.0.6/canonicalwebteam/store_base/handlers.py
+-rw-r--r--   0        0        0        0 2023-08-08 14:33:39.063889 canonicalwebteam_store_base-0.0.6/canonicalwebteam/store_base/packages/__init__.py
+-rw-r--r--   0        0        0    13375 2023-08-08 14:33:39.063889 canonicalwebteam_store_base-0.0.6/canonicalwebteam/store_base/packages/logic.py
+-rw-r--r--   0        0        0     2980 2023-08-08 14:33:39.063889 canonicalwebteam_store_base-0.0.6/canonicalwebteam/store_base/packages/views.py
+-rw-r--r--   0        0        0      201 2023-08-08 14:33:39.063889 canonicalwebteam_store_base-0.0.6/canonicalwebteam/store_base/sample_blueprint/views.py
+-rw-r--r--   0        0        0        0 2023-08-08 14:33:39.063889 canonicalwebteam_store_base-0.0.6/canonicalwebteam/store_base/utils/__init__.py
+-rw-r--r--   0        0        0     1094 2023-08-08 14:33:39.063889 canonicalwebteam_store_base-0.0.6/canonicalwebteam/store_base/utils/config.py
+-rw-r--r--   0        0        0      166 2023-08-08 14:33:39.063889 canonicalwebteam_store_base-0.0.6/canonicalwebteam/store_base/utils/constants.py
+-rw-r--r--   0        0        0      433 2023-08-08 14:33:39.063889 canonicalwebteam_store_base-0.0.6/canonicalwebteam/store_base/utils/decorators.py
+-rw-r--r--   0        0        0       61 2023-08-08 14:33:39.063889 canonicalwebteam_store_base-0.0.6/canonicalwebteam/store_base/utils/extensions.py
+-rw-r--r--   0        0        0     4608 2023-08-08 14:33:39.063889 canonicalwebteam_store_base-0.0.6/canonicalwebteam/store_base/utils/helpers.py
+-rw-r--r--   0        0        0       25 2023-08-08 14:33:39.063889 canonicalwebteam_store_base-0.0.6/canonicalwebteam/templates/storebase.html
+-rw-r--r--   0        0        0     1050 2023-08-08 14:33:39.067890 canonicalwebteam_store_base-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 canonicalwebteam_store_base-0.0.6/PKG-INFO
```

### Comparing `canonicalwebteam_store_base-0.0.5/LICENSE` & `canonicalwebteam_store_base-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.5/README.md` & `canonicalwebteam_store_base-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/app.py` & `canonicalwebteam_store_base-0.0.6/canonicalwebteam/store_base/app.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/auth/logic.py` & `canonicalwebteam_store_base-0.0.6/canonicalwebteam/store_base/auth/logic.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/auth/views.py` & `canonicalwebteam_store_base-0.0.6/canonicalwebteam/store_base/auth/views.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/data/licenses.json` & `canonicalwebteam_store_base-0.0.6/canonicalwebteam/store_base/data/licenses.json`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/handlers.py` & `canonicalwebteam_store_base-0.0.6/canonicalwebteam/store_base/handlers.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/packages/logic.py` & `canonicalwebteam_store_base-0.0.6/canonicalwebteam/store_base/packages/logic.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,25 +8,34 @@
 from typing import List, Dict, TypedDict, Any
 
 from canonicalwebteam.store_api.exceptions import StoreApiError
 
 from canonicalwebteam.store_base.utils import helpers
 
 
-Package = TypedDict(
-    "Package_type",
+Packages = TypedDict(
+    "Packages_type",
     {
         "packages": List[
             Dict[str, Dict[str, str or List[str]] or List[Dict[str, str]]]
         ]
     },
 )
 
+Package = TypedDict(
+    "Package_type",
+    {
+        "package": Dict[
+            str, Dict[str, str or List[str]] or List[Dict[str, str]]
+        ]
+    },
+)
+
 
-def fetch_packages(store_api, fields: List[str]) -> Package:
+def fetch_packages(store_api, fields: List[str]) -> Packages:
     """
     Fetches packages from the store API based on the specified fields.
 
     :param: store_api: The specific store API object.
     :param: fields (List[str]): A list of fields to include in the package
     data.
 
@@ -37,14 +46,34 @@
     store = store_api(talisker.requests.get_session())
     packages = store.find(fields=fields).get("results", [])
     response = make_response({"packages": packages})
     response.cache_control.max_age = 3600
     return response.json
 
 
+def fetch_package(store_api, package_name: str, fields: List[str]) -> Package:
+    """
+    Fetches a package from the store API based on the specified package name.
+
+    :param: store_api: The specific store API object.
+    :param: package_name (str): The name of the package to fetch.
+    :param: fields (List[str]): A list of fields to include in the package
+
+    :returns: a dictionary containing the fetched package.
+    """
+    store = store_api(talisker.requests.get_session())
+    package = store.get_item_details(
+        name=package_name,
+        fields=fields,
+    )
+    response = make_response({"package": package})
+    response.cache_control.max_age = 3600
+    return response.json
+
+
 def get_bundle_charms(charm_apps):
     result = []
 
     if charm_apps:
         for app_name, data in charm_apps.items():
             # Charm names could be with the old prefix/suffix
             # Like: cs:~charmed-osm/mariadb-k8s-35
@@ -148,20 +177,20 @@
             package["snap"]["media"]
         )
 
     return resp
 
 
 def paginate(
-    packages: List[Package], page: int, size: int, total_pages: int
-) -> List[Package]:
+    packages: List[Packages], page: int, size: int, total_pages: int
+) -> List[Packages]:
     """
     Paginates a list of packages based on the specified page and size.
 
-    :param: packages (List[Package]): The list of packages to paginate.
+    :param: packages (List[Packages]): The list of packages to paginate.
     :param: page (int): The current page number.
     :param: size (int): The number of packages to include in each page.
     :param: total_pages (int): The total number of pages.
     :returns: a list of paginated packages.
 
     note:
         - If the provided page exceeds the total number of pages, the last
@@ -228,15 +257,15 @@
             )
         res = parsed_packages
 
     return {"packages": res, "total_pages": total_pages}
 
 
 def filter_packages(
-    packages: List[Package], filter_params: Dict[str, List[str]]
+    packages: List[Packages], filter_params: Dict[str, List[str]]
 ):
     """
     Filters the list of packages based on the specified filter parameters.
 
     :param packages: the list of packages to filter.
     :param filter_params: The filter parameters
     :returns: the filtered list of packages.
@@ -371,7 +400,24 @@
             if abs((revision_since - now).days) < 30 and (
                 not revisions[0]["channels"]
                 or revisions[0]["channels"][0] == "edge"
             ):
                 snap_info["is_new"] = True
 
     return user_snaps, registered_snaps
+
+
+def get_package(
+    store, store_name: str, package_name: str, fields: List[str]
+) -> Package:
+    """Get a package by name
+
+    :param store: The store object.
+    :param store_name: The name of the store.
+    :param package_name: The name of the package.
+    :param fields: The fields to fetch.
+
+    :return: A dictionary containing the package.
+    """
+    package = fetch_package(store, package_name, fields).get("package", {})
+
+    return {"package": parse_package_for_card(package, store_name, store)}
```

### Comparing `canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/packages/views.py` & `canonicalwebteam_store_base-0.0.6/canonicalwebteam/store_base/packages/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     session,
     make_response,
     current_app as app,
 )
 
 from canonicalwebteam.store_base.packages.logic import (
     get_packages,
+    get_package,
     get_snaps_account_info,
 )
 from canonicalwebteam.store_base.utils.config import PACKAGE_PARAMS
 
 from canonicalwebteam.store_base.utils.decorators import login_required
 
 store_packages = Blueprint(
@@ -21,15 +22,14 @@
     __name__,
 )
 
 
 @store_packages.route("/store.json")
 def get_store_packages():
     app_name = app.name
-
     filters = dict(request.args)
     filters.pop("page", {})
     params = PACKAGE_PARAMS[app_name]
     store, fields, size = params["store"], params["fields"], params["size"]
 
     page = int(request.args.get("page", 1))
 
@@ -91,7 +91,18 @@
                 "snaps": user_snaps,
                 "current_user": flask_user["nickname"],
                 "registered_snaps": registered_snaps,
             }
         )
 
         return response
+
+
+@store_packages.route("/<package_name>/card.json")
+def get_store_package(package_name):
+    app_name = app.name
+
+    params = PACKAGE_PARAMS[app_name]
+    store, fields = params["store"], params["fields"]
+
+    res = make_response(get_package(store, app_name, package_name, fields))
+    return res
```

### Comparing `canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/utils/config.py` & `canonicalwebteam_store_base-0.0.6/canonicalwebteam/store_base/utils/config.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.5/canonicalwebteam/store_base/utils/helpers.py` & `canonicalwebteam_store_base-0.0.6/canonicalwebteam/store_base/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_base-0.0.5/pyproject.toml` & `canonicalwebteam_store_base-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "canonicalwebteam-store-base"
-version = "0.0.5"
+version = "0.0.6"
 description = "An application base for all stores"
 authors = ["Canonical Webteam <webteam@canonical.com>"]
 license = "GPL3"
 readme = "README.md"
 packages = [{include = "canonicalwebteam"}]
 
 [tool.poetry.dependencies]
```

### Comparing `canonicalwebteam_store_base-0.0.5/PKG-INFO` & `canonicalwebteam_store_base-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canonicalwebteam-store-base
-Version: 0.0.5
+Version: 0.0.6
 Summary: An application base for all stores
 License: GPL3
 Author: Canonical Webteam
 Author-email: webteam@canonical.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

