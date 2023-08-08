# Comparing `tmp/pharus-0.8.6.tar.gz` & `tmp/pharus-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pharus-0.8.6.tar", last modified: Tue May  2 19:51:02 2023, max compression
+gzip compressed data, was "pharus-0.8.7.tar", last modified: Tue Aug  8 16:34:14 2023, max compression
```

## Comparing `pharus-0.8.6.tar` & `pharus-0.8.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 anaconda  (1001) anaconda   (101)        0 2023-05-02 19:51:02.345365 pharus-0.8.6/
--rw-r--r--   0 anaconda  (1001) anaconda   (101)     1079 2023-05-02 19:50:07.000000 pharus-0.8.6/LICENSE
--rw-r--r--   0 anaconda  (1001) anaconda   (101)     1799 2023-05-02 19:51:02.345365 pharus-0.8.6/PKG-INFO
--rw-r--r--   0 anaconda  (1001) anaconda   (101)     1422 2023-05-02 19:50:07.000000 pharus-0.8.6/README.rst
-drwxr-xr-x   0 anaconda  (1001) anaconda   (101)        0 2023-05-02 19:51:02.341365 pharus-0.8.6/pharus/
--rw-r--r--   0 anaconda  (1001) anaconda   (101)      368 2023-05-02 19:50:07.000000 pharus-0.8.6/pharus/__init__.py
--rw-r--r--   0 anaconda  (1001) anaconda   (101)    22314 2023-05-02 19:50:07.000000 pharus-0.8.6/pharus/component_interface.py
--rw-r--r--   0 anaconda  (1001) anaconda   (101)    11118 2023-05-02 19:50:07.000000 pharus-0.8.6/pharus/dynamic_api_gen.py
--rw-r--r--   0 anaconda  (1001) anaconda   (101)      276 2023-05-02 19:50:07.000000 pharus-0.8.6/pharus/error.py
--rw-r--r--   0 anaconda  (1001) anaconda   (101)    19519 2023-05-02 19:50:07.000000 pharus-0.8.6/pharus/interface.py
--rw-r--r--   0 anaconda  (1001) anaconda   (101)    41895 2023-05-02 19:50:07.000000 pharus-0.8.6/pharus/server.py
--rw-r--r--   0 anaconda  (1001) anaconda   (101)       46 2023-05-02 19:50:07.000000 pharus-0.8.6/pharus/version.py
-drwxr-xr-x   0 anaconda  (1001) anaconda   (101)        0 2023-05-02 19:51:02.345365 pharus-0.8.6/pharus.egg-info/
--rw-r--r--   0 anaconda  (1001) anaconda   (101)     1799 2023-05-02 19:51:02.000000 pharus-0.8.6/pharus.egg-info/PKG-INFO
--rw-r--r--   0 anaconda  (1001) anaconda   (101)      355 2023-05-02 19:51:02.000000 pharus-0.8.6/pharus.egg-info/SOURCES.txt
--rw-r--r--   0 anaconda  (1001) anaconda   (101)        1 2023-05-02 19:51:02.000000 pharus-0.8.6/pharus.egg-info/dependency_links.txt
--rw-r--r--   0 anaconda  (1001) anaconda   (101)       45 2023-05-02 19:51:02.000000 pharus-0.8.6/pharus.egg-info/entry_points.txt
--rw-r--r--   0 anaconda  (1001) anaconda   (101)      146 2023-05-02 19:51:02.000000 pharus-0.8.6/pharus.egg-info/requires.txt
--rw-r--r--   0 anaconda  (1001) anaconda   (101)        7 2023-05-02 19:51:02.000000 pharus-0.8.6/pharus.egg-info/top_level.txt
--rw-r--r--   0 anaconda  (1001) anaconda   (101)       38 2023-05-02 19:51:02.345365 pharus-0.8.6/setup.cfg
--rw-r--r--   0 anaconda  (1001) anaconda   (101)     1277 2023-05-02 19:50:07.000000 pharus-0.8.6/setup.py
+drwxr-xr-x   0 anaconda  (1001) anaconda   (101)        0 2023-08-08 16:34:14.977429 pharus-0.8.7/
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)     1079 2023-08-08 16:33:26.000000 pharus-0.8.7/LICENSE
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)     1799 2023-08-08 16:34:14.977429 pharus-0.8.7/PKG-INFO
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)     1422 2023-08-08 16:33:26.000000 pharus-0.8.7/README.rst
+drwxr-xr-x   0 anaconda  (1001) anaconda   (101)        0 2023-08-08 16:34:14.973429 pharus-0.8.7/pharus/
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)      368 2023-08-08 16:33:26.000000 pharus-0.8.7/pharus/__init__.py
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)    22314 2023-08-08 16:33:26.000000 pharus-0.8.7/pharus/component_interface.py
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)    11118 2023-08-08 16:33:26.000000 pharus-0.8.7/pharus/dynamic_api_gen.py
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)      276 2023-08-08 16:33:26.000000 pharus-0.8.7/pharus/error.py
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)    18642 2023-08-08 16:33:26.000000 pharus-0.8.7/pharus/interface.py
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)    37292 2023-08-08 16:33:26.000000 pharus-0.8.7/pharus/server.py
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)       46 2023-08-08 16:33:26.000000 pharus-0.8.7/pharus/version.py
+drwxr-xr-x   0 anaconda  (1001) anaconda   (101)        0 2023-08-08 16:34:14.977429 pharus-0.8.7/pharus.egg-info/
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)     1799 2023-08-08 16:34:14.000000 pharus-0.8.7/pharus.egg-info/PKG-INFO
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)      355 2023-08-08 16:34:14.000000 pharus-0.8.7/pharus.egg-info/SOURCES.txt
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)        1 2023-08-08 16:34:14.000000 pharus-0.8.7/pharus.egg-info/dependency_links.txt
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)       45 2023-08-08 16:34:14.000000 pharus-0.8.7/pharus.egg-info/entry_points.txt
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)      146 2023-08-08 16:34:14.000000 pharus-0.8.7/pharus.egg-info/requires.txt
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)        7 2023-08-08 16:34:14.000000 pharus-0.8.7/pharus.egg-info/top_level.txt
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)       38 2023-08-08 16:34:14.977429 pharus-0.8.7/setup.cfg
+-rw-r--r--   0 anaconda  (1001) anaconda   (101)     1277 2023-08-08 16:33:26.000000 pharus-0.8.7/setup.py
```

### Comparing `pharus-0.8.6/LICENSE` & `pharus-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pharus-0.8.6/PKG-INFO` & `pharus-0.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pharus
-Version: 0.8.6
+Version: 0.8.7
 Summary: A generic REST API server backend for DataJoint pipelines.
 Home-page: https://github.com/datajoint/pharus
 Author: DataJoint Neuro
 Author-email: support@vathes.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/x-rst
```

### Comparing `pharus-0.8.6/README.rst` & `pharus-0.8.7/README.rst`

 * *Files identical despite different names*

### Comparing `pharus-0.8.6/pharus/component_interface.py` & `pharus-0.8.7/pharus/component_interface.py`

 * *Files identical despite different names*

### Comparing `pharus-0.8.6/pharus/dynamic_api_gen.py` & `pharus-0.8.7/pharus/dynamic_api_gen.py`

 * *Files identical despite different names*

### Comparing `pharus-0.8.6/pharus/interface.py` & `pharus-0.8.7/pharus/interface.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,19 +16,20 @@
     """Primary connector that communicates with a DataJoint database server."""
 
     @staticmethod
     def _list_schemas(connection: dj.Connection) -> list:
         """
         List all schemas under the database.
 
-        :param connection: User's DataJoint connection object
-        :type connection: dj.Connection
-        :return: List of schemas names in alphabetical order (excludes ``information_schema``,
+        Args:
+            connection (dj.Connection): User's DataJoint connection object
+
+        Returns:
+            List of schemas names in alphabetical order (excludes ``information_schema``,
             ``sys``, ``performance_schema``, ``mysql``)
-        :rtype: list
         """
 
         # Attempt to connect return true if successful, false is failed
         return [
             row[0]
             for row in connection.query(
                 """
@@ -45,21 +46,21 @@
     def _list_tables(
         connection: dj.Connection,
         schema_name: str,
     ) -> dict:
         """
         List all tables and their type given a schema.
 
-        :param connection: User's DataJoint connection object
-        :type connection: dj.Connection
-        :param schema_name: Name of schema to list all tables from
-        :type schema_name: str
-        :return: Contains a key for each table type where values are the respective list of
-            table names
-        :rtype: dict
+        Args:
+            connection (dj.Connection): User's DataJoint connection object
+            schema_name (str): Name of schema to list all tables from
+
+        Returns:
+            Contains a key for each table type where values are the respective
+                list of table names
         """
 
         # Get list of tables names
         tables_name = dj.Schema(
             schema_name, create_schema=False, connection=connection
         ).list_tables()
         # Dict to store list of table name for each type
@@ -96,31 +97,31 @@
         limit: int = 1000,
         page: int = 1,
         order=None,
         fetch_blobs=False,
         fetch_args=[],
     ) -> tuple:
         """
-        Get records from query.
+        Get records from the query.
 
-        :param query: any datajoint object related to QueryExpression
-        :type query: datajoint ``QueryExpression`` or related object
-        :param restriction: Sequence of filters as ``dict`` with ``attributeName``,
-            ``operation``, ``value`` keys defined, defaults to ``[]``
-        :type restriction: list, optional
-        :param limit: Max number of records to return, defaults to ``1000``
-        :type limit: int, optional
-        :param page: Page number to return, defaults to ``1``
-        :type page: int, optional
-        :param order: Sequence to order records, defaults to ``['KEY ASC']``. See
-            :class:`~datajoint.fetch.Fetch` for more info.
-        :type order: list, optional
-        :return: Attribute headers, records in dict form, and the total number of records that
-            can be paged
-        :rtype: tuple
+        Args:
+            query: Any datajoint object related to QueryExpression.
+            restriction (optional): Sequence of filters as ``dict`` with ``attributeName``,
+                ``operation``, ``value`` keys defined, defaults to ``[]``.
+            limit (optional): Max number of records to return, defaults to ``1000``.
+            page (optional): Page number to return, defaults to ``1``.
+            order (optional): Sequence to order records, defaults to ``['KEY ASC']``. See
+                :class:`~datajoint.fetch.Fetch` for more info.
+
+        Returns:
+            A tuple containing:
+
+                - Attribute headers
+                - Records in dictionary form
+                - The total number of records that can be paged
         """
 
         # Get table object from name
         attributes = query.heading.attributes
         # Fetch tuples without blobs as dict to be used to create a
         #   list of tuples for returning
         query_restricted = query & dj.AndList(
@@ -207,24 +208,27 @@
         return list(attributes.keys()), rows, len(query_restricted)
 
     @staticmethod
     def _get_attributes(query, include_unique_values=False) -> dict:
         """
         Method to get primary and secondary attributes of a query.
 
-        :param query: any datajoint object related to QueryExpression
-        :type query: datajoint ``QueryExpression`` or related object
-        :param include_unique_values: boolean that determines if the unique values are
-            included as part of the returned attributes
-        :type include_unique_values: boolean, optional
-        :return: Dict with keys ``attribute_headers`` and ``attributes`` containing
-            ``primary``, ``secondary`` which each contain a
-            ``list`` of ``tuples`` specifying: ``attribute_name``, ``type``, ``nullable``,
-            ``default``, ``autoincrement``.
-        :rtype: dict
+        Args:
+            query: Any datajoint object related to QueryExpression.
+            include_unique_values (optional): Boolean that determines if the unique values are
+                included as part of the returned attributes.
+
+        Returns:
+            A dictionary with keys ``attribute_headers`` and ``attributes`` containing
+                ``primary``, ``secondary``, each of which is a list of tuples specifying:
+
+                - ``attribute_name``
+                - ``nullable``
+                - ``default``
+                - ``autoincrement``
         """
 
         query_attributes = dict(primary=[], secondary=[])
         for attribute_name, attribute_info in query.heading.attributes.items():
             if attribute_info.in_key:
                 query_attributes["primary"].append(
                     (
@@ -268,22 +272,21 @@
         connection: dj.Connection,
         schema_name: str,
         table_name: str,
     ) -> str:
         """
         Get the table definition.
 
-        :param connection: User's DataJoint connection object
-        :type connection: dj.Connection
-        :param schema_name: Name of schema
-        :type schema_name: str
-        :param table_name: Table name under the given schema; must be in camel case
-        :type table_name: str
-        :return: Definition of the table
-        :rtype: str
+        Args:
+            connection: User's DataJoint connection object.
+            schema_name: Name of the schema.
+            table_name: Table name under the given schema; must be in camel case.
+
+        Returns:
+            Definition of the table as a string.
         """
 
         local_values = locals()
         local_values[schema_name] = dj.VirtualModule(
             schema_name, schema_name, connection=connection
         )
         return getattr(local_values[schema_name], table_name).describe()
@@ -294,22 +297,19 @@
         schema_name: str,
         table_name: str,
         tuple_to_insert: dict,
     ):
         """
         Insert record as tuple into table.
 
-        :param connection: User's DataJoint connection object
-        :type connection: dj.Connection
-        :param schema_name: Name of schema
-        :type schema_name: str
-        :param table_name: Table name under the given schema; must be in camel case
-        :type table_name: str
-        :param tuple_to_insert: Record to be inserted
-        :type tuple_to_insert: dict
+        Args:
+            connection: User's DataJoint connection object.
+            schema_name: Name of the schema.
+            table_name: Table name under the given schema; must be in camel case.
+            tuple_to_insert: Record to be inserted as a dictionary.
         """
 
         schema_virtual_module = dj.VirtualModule(
             schema_name, schema_name, connection=connection
         )
         getattr(schema_virtual_module, table_name).insert(tuple_to_insert)
 
@@ -318,27 +318,25 @@
         connection: dj.Connection,
         schema_name: str,
         table_name: str,
         restriction: list = [],
     ) -> list:
         """
         Return summary of dependencies associated with a restricted table. Will only show
-        dependencies that user has access to.
+        dependencies that the user has access to.
 
-        :param connection: User's DataJoint connection object
-        :type connection: dj.Connection
-        :param schema_name: Name of schema
-        :type schema_name: str
-        :param table_name: Table name under the given schema; must be in camel case
-        :type table_name: str
-        :param restriction: Sequence of filters as ``dict`` with ``attributeName``,
-            ``operation``, ``value`` keys defined, defaults to ``[]``
-        :type restriction: list
-        :return: Tables that are dependent on specific records.
-        :rtype: list
+        Args:
+            connection: User's DataJoint connection object.
+            schema_name: Name of the schema.
+            table_name: Table name under the given schema; must be in camel case.
+            restriction: Sequence of filters as a list of dictionaries with keys
+                "attributeName", "operation", and "value" defined, defaults to [].
+
+        Returns:
+            List of tables that are dependent on specific records.
         """
 
         virtual_module = dj.VirtualModule(
             schema_name, schema_name, connection=connection
         )
         table = getattr(virtual_module, table_name)
         attributes = table.heading.attributes
@@ -372,24 +370,22 @@
     def _update_tuple(
         connection: dj.Connection,
         schema_name: str,
         table_name: str,
         tuple_to_update: dict,
     ):
         """
-        Update record as tuple into table.
+        Update record as a tuple into the table.
+
+        Args:
+            connection: User's DataJoint connection object.
+            schema_name: Name of the schema.
+            table_name: Table name under the given schema; must be in camel case.
+            tuple_to_update: Record to be updated.
 
-        :param connection: User's DataJoint connection object
-        :type connection: dj.Connection
-        :param schema_name: Name of schema
-        :type schema_name: str
-        :param table_name: Table name under the given schema; must be in camel case
-        :type table_name: str
-        :param tuple_to_update: Record to be updated
-        :type tuple_to_update: dict
         """
 
         schema_virtual_module = dj.VirtualModule(
             schema_name, schema_name, connection=connection
         )
         with connection.transaction:
             [
@@ -402,27 +398,23 @@
         connection: dj.Connection,
         schema_name: str,
         table_name: str,
         restriction: list = [],
         cascade: bool = False,
     ):
         """
-        Delete a specific record based on the restriction given.
+        Delete a specific record based on the given restriction.
 
-        :param connection: User's DataJoint connection object
-        :type connection: dj.Connection
-        :param schema_name: Name of schema
-        :type schema_name: str
-        :param table_name: Table name under the given schema; must be in camel case
-        :type table_name: str
-        :param restriction: Sequence of filters as ``dict`` with ``attributeName``,
-            ``operation``, ``value`` keys defined, defaults to ``[]``
-        :type restriction: list, optional
-        :param cascade: Allow for cascading delete, defaults to ``False``
-        :type cascade: bool, optional
+        Args:
+            connection: User's DataJoint connection object.
+            schema_name: Name of the schema.
+            table_name: Table name under the given schema; must be in camel case.
+            restriction: Sequence of filters as a list of dictionaries with keys
+                         ``attributeName``, ``operation``, and ``value``, defaults to ``[]``.
+            cascade: Allow for cascading delete, defaults to ``False``.
         """
 
         schema_virtual_module = dj.VirtualModule(
             schema_name, schema_name, connection=connection
         )
 
         # Get table object from name
@@ -443,45 +435,49 @@
         query.delete(safemode=False) if cascade else query.delete_quick()
 
     @staticmethod
     def _get_table_object(
         schema_virtual_module: VirtualModule, table_name: str
     ) -> UserTable:
         """
-        Helper method for getting the table object based on the table name provided.
+        Helper method for getting the table object based on the provided table name.
 
-        :param schema_virtual_module: Virtual module for accesing the schema
-        :type schema_virtual_module: :class:`~datajoint.schemas.VirtualModule`
-        :param table_name: Name of the table; for part it should be ``Parent.Part``
-        :type table_name: str
-        :return: DataJoint table object.
-        :rtype: :class:`~datajoint.user_tables.UserTable`
+        Args:
+            schema_virtual_module: Virtual module for accessing the schema.
+            table_name: Name of the table; for part tables, it should
+                be in the format ``Parent.Part``.
+
+        Returns:
+            DataJoint table object of the specified table.
         """
+
         # Split the table name by '.' for dealing with part tables
         table_name_parts = table_name.split(".")
         if len(table_name_parts) == 2:
             return getattr(
                 getattr(schema_virtual_module, table_name_parts[0]), table_name_parts[1]
             )
         else:
             return getattr(schema_virtual_module, table_name_parts[0])
 
     @staticmethod
     def _filter_to_restriction(attribute_filter: dict, attribute_type: str) -> str:
         """
-        Convert attribute filter to a restriction.
+        Converts an attribute filter to a DataJoint-compatible restriction.
 
-        :param attribute_filter: A filter as ``dict`` with ``attributeName``, ``operation``,
-            ``value`` keys defined, defaults to ``[]``
-        :type attribute_filter: dict
-        :param attribute_type: Attribute type
-        :type attribute_type: str
-        :return: DataJoint-compatible restriction
-        :rtype: str
+        Args:
+            attribute_filter (dict): A filter as a dictionary with keys
+                ``attributeName``, ``operation``, and ``value`` defined.
+                Defaults to an empty dictionary.
+            attribute_type (str): Attribute type.
+
+        Returns:
+            DataJoint-compatible restriction.
         """
+
         if attribute_filter["operation"] in (">", "<", ">=", "<="):
             operation = attribute_filter["operation"]
         elif attribute_filter["value"] is None:
             operation = " IS " if attribute_filter["operation"] == "=" else " IS NOT "
         else:
             operation = attribute_filter["operation"]
```

### Comparing `pharus-0.8.6/pharus/server.py` & `pharus-0.8.7/pharus/server.py`

 * *Files 24% similar despite different names*

```diff
@@ -53,19 +53,19 @@
     )
 
 
 def protected_route(function: Callable) -> Callable:
     """
     Protected route function decorator which authenticates requests.
 
-    :param function: Function to decorate, typically routes
-    :type function: :class:`~typing.Callable`
-    :return: Function output if JWT authetication is successful, otherwise return error
-        message
-    :rtype: :class:`~typing.Callable`
+    Args:
+        function: Function to decorate, typically routes
+
+    Returns:
+        Function's output if JWT authetication is successful, otherwise return error message
     """
 
     @wraps(function)
     def wrapper(**kwargs):
         try:
             if "database_host" in request.args:
                 encoded_jwt = request.headers.get("Authorization").split()[1]
@@ -101,116 +101,122 @@
 
 
 @app.route(f"{environ.get('PHARUS_PREFIX', '')}/version", methods=["GET"])
 def api_version() -> str:
     """
     Handler for ``/version`` route.
 
-    :return: API version
-    :rtype: str
-
-    .. http:get:: /version
+    Returns:
+        API version
 
-        Route to check server health returning the API version.
+    ## GET /version
 
-        **Example request**:
+    Route to check server health returning the API version.
 
-        .. sourcecode:: http
+    ### Example request:
 
-            GET /version HTTP/1.1
-            Host: fakeservices.datajoint.io
+    ```http
+    GET /version HTTP/1.1
+    Host: fakeservices.datajoint.io
+    ```
 
-        **Example response**:
+    ### Example response:
 
-        .. sourcecode:: http
+    ```http
+    HTTP/1.1 200 OK
+    Vary: Accept
+    Content-Type: application/json
 
-            HTTP/1.1 200 OK
-            Vary: Accept
-            Content-Type: application/json
-
-            {
-                "version": "0.7.3"
-            }
+    {
+        "version": "0.8.7"
+    }
+    ```
 
-        :statuscode 200: No error.
+    #### Status Codes
+    * 200 OK: No error.
     """
     if request.method in {"GET", "HEAD"}:
         return dict(version=version)
 
 
 @app.route(f"{environ.get('PHARUS_PREFIX', '')}/login", methods=["POST"])
 def login() -> dict:
     """
-    **WARNING**: Currently, this implementation exposes user database credentials as plain
-    text in POST body once and stores it within a bearer token as Base64 encoded for
-    subsequent requests. That is how the server is able to submit queries on user's behalf.
-    Due to this, it is required that remote hosts expose the server only under HTTPS to ensure
-    end-to-end encryption. Sending passwords in plain text over HTTPS in POST request body is
-    common and utilized by companies such as GitHub (2021) and Chase Bank (2021). On server
-    side, there is no caching, logging, or storage of received passwords or tokens and thus
-    available only briefly in memory. This means the primary vulnerable point is client side.
-    Users should be responsible with their passwords and bearer tokens treating them as
-    one-in-the-same. Be aware that if your client system happens to be compromised, a bad
-    actor could monitor your outgoing network requests and capture/log your credentials.
-    However, in such a terrible scenario, a bad actor would not only collect credentials for
-    your DataJoint database but also other sites such as github.com, chase.com, etc. Please be
-    responsible and vigilant with credentials and tokens on client side systems. Improvements
-    to the above strategy is currently being tracked in
-    https://github.com/datajoint/pharus/issues/82.
-
     Handler for ``/login`` route.
 
-    :return: Function output is an encoded JWT if successful, otherwise return error message
-    :rtype: dict
-
-    .. http:post:: /login
-
-        Route to generate an authentication token.
-
-        **Example request**:
-
-        .. sourcecode:: http
-
-            POST /login HTTP/1.1
-            Host: fakeservices.datajoint.io
-            Accept: application/json
-
-            {
-                "databaseAddress": "tutorial-db.datajoint.io",
-                "username": "user1",
-                "password": "password1"
-            }
-
-        **Example successful response**:
-
-        .. sourcecode:: http
-
-            HTTP/1.1 200 OK
-            Vary: Accept
-            Content-Type: application/json
-
-            {
-                "jwt": "<token>"
-            }
-
-
-        **Example unexpected response**:
-
-        .. sourcecode:: http
-
-            HTTP/1.1 500 Internal Server Error
-            Vary: Accept
-            Content-Type: text/plain
-
-            400 Bad Request: The browser (or proxy) sent a request that this server could not
-                understand.
-
-        :resheader Content-Type: text/plain, application/json
-        :statuscode 200: No error.
-        :statuscode 500: Unexpected error encountered. Returns the error message as a string.
+    Warning:
+        Currently, this implementation exposes user database credentials as plain text in
+        POST body once and stores it within a bearer token as Base64 encoded for
+        subsequent requests. That is how the server is able to submit queries on user's
+        behalf. Due to this, it is required that remote hosts expose the server only
+        under HTTPS to ensure end-to-end encryption. Sending passwords in plain text over
+        HTTPS in POST request body is common and utilized by companies such as GitHub
+        (2021) and Chase Bank (2021). On server side, there is no caching, logging, or
+        storage of received passwords or tokens and thus available only briefly in
+        memory. This means the primary vulnerable point is client side. Users should be
+        responsible with their passwords and bearer tokens treating them as
+        one-in-the-same. Be aware that if your client system happens to be compromised,
+        a bad actor could monitor your outgoing network requests and capture/log your
+        credentials. However, in such a terrible scenario, a bad actor would not only
+        collect credentials for your DataJoint database but also other sites such as
+        github.com, chase.com, etc. Please be responsible and vigilant with credentials
+        and tokens on client side systems. Improvements to the above strategy is
+        currently being tracked in https://github.com/datajoint/pharus/issues/82.
+
+    Returns:
+        Function output is an encoded JWT if successful, otherwise return error message
+
+    ## POST /login
+
+    Route to generate an authentication token.
+
+    ### Example request:
+
+    ```http
+    POST /login HTTP/1.1
+    Host: fakeservices.datajoint.io
+    Accept: application/json
+
+    {
+        "databaseAddress": "tutorial-db.datajoint.io",
+        "username": "user1",
+        "password": "password1"
+    }
+    ```
+
+    ### Example successful response:
+
+    ```http
+    HTTP/1.1 200 OK
+    Vary: Accept
+    Content-Type: application/json
+
+    {
+        "jwt": "<token>"
+    }
+    ```
+
+    ### Example unexpected response:
+
+    ```http
+    HTTP/1.1 500 Internal Server Error
+    Vary: Accept
+    Content-Type: text/plain
+
+    400 Bad Request: The browser (or proxy) sent a request that this server could not
+        understand.
+    ```
+
+    #### Response Headers
+    * Content-Type: text/plain, application/json
+
+    #### Status Codes
+    * 200 OK: No error.
+    * 500 Internal Server Error: Unexpected error encountered.
+        Returns the error message as a string.
     """
     if request.method == "POST":
         # Try to login in with the database connection info, if true then create jwt key
         try:
             if "database_host" in request.args:
                 # Oidc token exchange
 
@@ -291,61 +297,69 @@
 
 @app.route(f"{environ.get('PHARUS_PREFIX', '')}/schema", methods=["GET"])
 @protected_route
 def schema(connection: dj.Connection) -> dict:
     """
     Handler for ``/schema`` route.
 
-    :param connection: User's DataJoint connection object
-    :type connection: dj.Connection
-    :return: If successful then sends back a list of schemas names otherwise returns error.
-    :rtype: dict
+    Args:
+        connection (dj.Connection): User's DataJoint connection object
 
-    .. http:get:: /schema
+    Returns:
+        If successful, then sends back a list of schema names; otherwise, returns an error.
 
-        Route to get list of schemas.
+    ## GET /schema
 
-        **Example request**:
+    Route to get a list of schemas.
 
-        .. sourcecode:: http
+    ### Example request:
 
-            GET /schema HTTP/1.1
-            Host: fakeservices.datajoint.io
-            Authorization: Bearer <token>
+    ```http
+    GET /schema HTTP/1.1
+    Host: fakeservices.datajoint.io
+    Authorization: Bearer <token>
+    ```
 
-        **Example successful response**:
+    ### Example successful response:
 
-        .. sourcecode:: http
+    ```http
+    HTTP/1.1 200 OK
+    Vary: Accept
+    Content-Type: application/json
 
-            HTTP/1.1 200 OK
-            Vary: Accept
-            Content-Type: application/json
+    {
+        "schemaNames": [
+            "alpha_company"
+        ]
+    }
+    ```
 
-            {
-                "schemaNames": [
-                    "alpha_company"
-                ]
-            }
+    ### Example unexpected response:
 
-        **Example unexpected response**:
+    ```http
+    HTTP/1.1 500 Internal Server Error
+    Vary: Accept
+    Content-Type: text/plain
 
-        .. sourcecode:: http
+    400 Bad Request: The browser (or proxy) sent a request that this server could not
+        understand.
+    ```
 
-            HTTP/1.1 500 Internal Server Error
-            Vary: Accept
-            Content-Type: text/plain
+    #### Request Headers
+    * Authorization: Bearer <OAuth2_token\>
 
-            400 Bad Request: The browser (or proxy) sent a request that this server could not
-                understand.
+    #### Response Headers
+    * Content-Type: text/plain, application/json
 
-        :reqheader Authorization: Bearer <OAuth2_token>
-        :resheader Content-Type: text/plain, application/json
-        :statuscode 200: No error.
-        :statuscode 500: Unexpected error encountered. Returns the error message as a string.
+    #### Status Codes
+    * 200 OK: No error.
+    * 500 Internal Server Error: Unexpected error encountered.
+        Returns the error message as a string.
     """
+
     if request.method in {"GET", "HEAD"}:
         # Get all the schemas
         try:
             schemas_name = _DJConnector._list_schemas(connection)
             return dict(schemaNames=schemas_name)
         except Exception:
             return traceback.format_exc(), 500
@@ -358,71 +372,79 @@
 def table(
     connection: dj.Connection,
     schema_name: str,
 ) -> dict:
     """
     Handler for ``/schema/{schema_name}/table`` route.
 
-    :param connection: User's DataJoint connection object
-    :type connection: dj.Connection
-    :param schema_name: Schema name.
-    :type schema_name: str
-    :return: If successful then sends back a list of table names otherwise returns error.
-    :rtype: dict
-
-    .. http:get:: /schema/{schema_name}/table
-
-        Route to get tables within a schema.
-
-        **Example request**:
-
-        .. sourcecode:: http
-
-            GET /schema/alpha_company/table HTTP/1.1
-            Host: fakeservices.datajoint.io
-            Authorization: Bearer <token>
-
-        **Example successful response**:
-
-        .. sourcecode:: http
-
-            HTTP/1.1 200 OK
-            Vary: Accept
-            Content-Type: application/json
-
-            {
-                "tableTypes": {
-                    "computed": [],
-                    "imported": [],
-                    "lookup": [
-                        "Employee"
-                    ],
-                    "manual": [
-                        "Computer"
-                    ],
-                    "part": []
-                }
-            }
-
-        **Example unexpected response**:
-
-        .. sourcecode:: http
-
-            HTTP/1.1 500 Internal Server Error
-            Vary: Accept
-            Content-Type: text/plain
-
-            400 Bad Request: The browser (or proxy) sent a request that this server could not
-                understand.
-
-        :query schema_name: Schema name.
-        :reqheader Authorization: Bearer <OAuth2_token>
-        :resheader Content-Type: text/plain, application/json
-        :statuscode 200: No error.
-        :statuscode 500: Unexpected error encountered. Returns the error message as a string.
+    Args:
+        connection (dj.Connection): User's DataJoint connection object
+        schema_name (str): Schema name.
+
+    Returns:
+        If successful, then sends back a list of table names; otherwise, returns an error.
+
+    ## GET /schema/{schema_name}/table
+
+    Route to get tables within a schema.
+
+    ### Example request:
+
+    ```http
+    GET /schema/alpha_company/table HTTP/1.1
+    Host: fakeservices.datajoint.io
+    Authorization: Bearer <token>
+    ```
+
+    ### Example successful response:
+
+    ```http
+    HTTP/1.1 200 OK
+    Vary: Accept
+    Content-Type: application/json
+
+    {
+        "tableTypes": {
+            "computed": [],
+            "imported": [],
+            "lookup": [
+                "Employee"
+            ],
+            "manual": [
+                "Computer"
+            ],
+            "part": []
+        }
+    }
+    ```
+
+    ### Example unexpected response:
+
+    ```http
+    HTTP/1.1 500 Internal Server Error
+    Vary: Accept
+    Content-Type: text/plain
+
+    400 Bad Request: The browser (or proxy) sent a request that this server could not
+        understand.
+    ```
+
+    #### Query Parameters
+    * schema_name: Schema name.
+
+    #### Request Headers
+    * Authorization: Bearer <OAuth2_token\>
+
+    #### Response Headers
+    * Content-Type: text/plain, application/json
+
+    #### Status Codes
+    * 200 OK: No error.
+    * 500 Internal Server Error: Unexpected error encountered.
+        Returns the error message as a string.
     """
     if request.method in {"GET", "HEAD"}:
         try:
             tables_dict_list = _DJConnector._list_tables(connection, schema_name)
             return dict(tableTypes=tables_dict_list)
         except Exception:
             return traceback.format_exc(), 500
@@ -436,301 +458,322 @@
 def record(
     connection: dj.Connection,
     schema_name: str,
     table_name: str,
 ) -> Union[dict, str, tuple]:
     (
         """
-        Handler for ``/schema/{schema_name}/table/{table_name}/record`` route.
+    Handler for ``/schema/{schema_name}/table/{table_name}/record`` route.
 
-        :param connection: User's DataJoint connection object
-        :type connection: dj.Connection
-        :param schema_name: Schema name.
-        :type schema_name: str
-        :param table_name: Table name.
-        :type table_name: str
-        :return: If successful performs desired operation based on HTTP method, otherwise
-            returns error.
-        :rtype: :class:`~typing.Union[dict, str, tuple]`
-
-        .. http:get:: /schema/{schema_name}/table/{table_name}/record
-
-            Route to fetch records.
-
-            **Example request**:
-
-            .. sourcecode:: http
-
-                GET /schema/alpha_company/table/Computer/record?limit=1&page=2&"""
-        "order=computer_id%20DESC&restriction=W3siYXR0cmlidXRlTmFtZSI6ICJjb21wdXRlcl9tZW1vcnk"
-        "iLCAib3BlcmF0aW9uIjogIj49IiwgInZhbHVlIjogMTZ9XQo="
-        """ HTTP/1.1
-                Host: fakeservices.datajoint.io
-                Authorization: Bearer <token>
-
-            **Example successful response**:
-
-            .. sourcecode:: http
-
-                HTTP/1.1 200 OK
-                Vary: Accept
-                Content-Type: application/json
-
-                {
-                    "recordHeader": [
-                        "computer_id",
-                        "computer_serial",
-                        "computer_brand",
-                        "computer_built",
-                        "computer_processor",
-                        "computer_memory",
-                        "computer_weight",
-                        "computer_cost",
-                        "computer_preowned",
-                        "computer_purchased",
-                        "computer_updates",
-                        "computer_accessories"
-                    ],
-                    "records": [
-                        [
-                            "4e41491a-86d5-4af7-a013-89bde75528bd",
-                            "DJS1JA17G",
-                            "Dell",
-                            1590364800,
-                            2.2,
-                            16,
-                            4.4,
-                            "700.99",
-                            0,
-                            1603181061,
-                            null,
-                            "=BLOB="
-                        ]
-                    ],
-                    "totalCount": 2
-                }
-
-            **Example unexpected response**:
-
-            .. sourcecode:: http
-
-                HTTP/1.1 500 Internal Server Error
-                Vary: Accept
-                Content-Type: text/plain
-
-                400 Bad Request: The browser (or proxy) sent a request that this server could
-                    not understand.
-
-            :query schema_name: Schema name.
-            :query table_name: Table name.
-            :query limit: Limit of how many records per page. Defaults to ``1000``.
-            :query page: Page requested. Defaults to ``1``.
-            :query order: Sort order. Defaults to ``KEY ASC``.
-            :query restriction: Base64-encoded ``AND`` sequence of restrictions. For example,
-                you could restrict as ``[{"attributeName": "computer_memory", "operation": ``-
-                ``">=", "value": 16}]`` with this param set as
-                ``W3siYXR0cmlidXRlTmFtZSI6ICJjb21wdXRlcl9tZW1vcnkiLCAib3Bl``-
-                ``cmF0aW9uIjogIj49IiwgInZhbHVlIjogMTZ9XQo=``. Defaults to no restriction.
-            :reqheader Authorization: Bearer <OAuth2_token>
-            :resheader Content-Type: text/plain, application/json
-            :statuscode 200: No error.
-            :statuscode 500: Unexpected error encountered. Returns the error message as a
-                string.
-
-        .. http:post:: /schema/{schema_name}/table/{table_name}/record
-
-            Route to insert a record. Omitted attributes utilize the default if set.
-
-            **Example request**:
-
-            .. sourcecode:: http
-
-                POST /schema/alpha_company/table/Computer/record HTTP/1.1
-                Host: fakeservices.datajoint.io
-                Accept: application/json
-                Authorization: Bearer <token>
-
-                {
-                    "records": [
-                        {
-                            "computer_id": "ffffffff-86d5-4af7-a013-89bde75528bd",
-                            "computer_serial": "ZYXWVEISJ",
-                            "computer_brand": "HP",
-                            "computer_built": "2021-01-01",
-                            "computer_processor": 2.7,
-                            "computer_memory": 32,
-                            "computer_weight": 3.7,
-                            "computer_cost": 599.99,
-                            "computer_preowned": 0,
-                            "computer_purchased": "2021-02-01 13:00:00",
-                            "computer_updates": 0
-                        }
-                    ]
-                }
-
-            **Example successful response**:
-
-            .. sourcecode:: http
-
-                HTTP/1.1 200 OK
-                Vary: Accept
-                Content-Type: text/plain
-
-                {
-                    "response": "Insert Successful"
-                }
-
-            **Example unexpected response**:
-
-            .. sourcecode:: http
-
-                HTTP/1.1 500 Internal Server Error
-                Vary: Accept
-                Content-Type: text/plain
-
-                400 Bad Request: The browser (or proxy) sent a request that this server could
-                    not understand.
-
-            :reqheader Authorization: Bearer <OAuth2_token>
-            :resheader Content-Type: text/plain
-            :statuscode 200: No error.
-            :statuscode 500: Unexpected error encountered. Returns the error message as a
-                string.
-
-        .. http:patch:: /schema/{schema_name}/table/{table_name}/record
-
-            Route to update a record. Omitted attributes utilize the default if set.
-
-            **Example request**:
-
-            .. sourcecode:: http
-
-                PATCH /schema/alpha_company/table/Computer/record HTTP/1.1
-                Host: fakeservices.datajoint.io
-                Accept: application/json
-                Authorization: Bearer <token>
-
-                {
-                    "records": [
-                        {
-                            "computer_id": "ffffffff-86d5-4af7-a013-89bde75528bd",
-                            "computer_serial": "ZYXWVEISJ",
-                            "computer_brand": "HP",
-                            "computer_built": "2021-01-01",
-                            "computer_processor": 2.7,
-                            "computer_memory": 32,
-                            "computer_weight": 3.7,
-                            "computer_cost": 601.01,
-                            "computer_preowned": 0,
-                            "computer_purchased": "2021-02-01 13:00:00",
-                            "computer_updates": 0
-                        }
-                    ]
-                }
+    Args:
+        connection (dj.Connection): User's DataJoint connection object
+        schema_name (str): Schema name.
+        table_name (str): Table name.
+
+    Returns:
+        If successful, then sends back the desired operation based on the HTTP method;
+            otherwise, returns an error.
+
+    ## GET /schema/{schema_name}/table/{table_name}/record
+
+    Route to fetch records.
+
+    ### Example request:
+
+    ```http
+    GET /schema/alpha_company/table/Computer/record?limit=1&page=2&order=computer_id%20DESC&
+        restriction=W3siYXR0cmlidXRlTmFtZSI6ICJjb21wdXRlcl9tZW1vcnkiLCAib3BlcmF0aW9uIjogIj49I
+        iwgInZhbHVlIjogMTZ9XQo= HTTP/1.1
+    Host: fakeservices.datajoint.io
+    Authorization: Bearer <token>
+    ```
+
+    ### Example successful response:
+
+    ```http
+    HTTP/1.1 200 OK
+    Vary: Accept
+    Content-Type: application/json
+
+    {
+        "recordHeader": [
+            "computer_id",
+            "computer_serial",
+            "computer_brand",
+            "computer_built",
+            "computer_processor",
+            "computer_memory",
+            "computer_weight",
+            "computer_cost",
+            "computer_preowned",
+            "computer_purchased",
+            "computer_updates",
+            "computer_accessories"
+        ],
+        "records": [
+            [
+                "4e41491a-86d5-4af7-a013-89bde75528bd",
+                "DJS1JA17G",
+                "Dell",
+                1590364800,
+                2.2,
+                16,
+                4.4,
+                "700.99",
+                0,
+                1603181061,
+                null,
+                "=BLOB="
+            ]
+        ],
+        "totalCount": 2
+    }
+    ```
+
+    ### Example unexpected response:
+
+    ```http
+    HTTP/1.1 500 Internal Server Error
+    Vary: Accept
+    Content-Type: text/plain
+
+    400 Bad Request: The browser (or proxy) sent a request that this server could
+        not understand.
+    ```
+
+    #### Query Parameters
+    * schema_name: Schema name.
+    * table_name: Table name.
+    * limit: Limit of how many records per page. Defaults to `1000`.
+    * page: Page requested. Defaults to `1`.
+    * order: Sort order. Defaults to `KEY ASC`.
+    * restriction: Base64-encoded `AND` sequence of restrictions. For example, you could
+        restrict as `[{"attributeName": "computer_memory", "operation": ">=", "value": 16}]`
+        with this param set as `W3siYXR0cmlidXRlTmFtZSI6ICJjb21wdXRlcl9tZW1vcnkiLCAib3BlcmF0a
+        W9uIjogIj49IiwgInZhbHVlIjogMTZ9XQo=`. Defaults to no restriction.
+
+    #### Request Headers
+    * Authorization: Bearer <OAuth2_token\>
+
+    #### Response Headers
+    * Content-Type: text/plain, application/json
+
+    #### Status Codes
+    * 200 OK: No error.
+    * 500 Internal Server Error: Unexpected error encountered. Returns the error message as a
+        string.
+
+    ## POST /schema/{schema_name}/table/{table_name}/record
+
+    Route to insert a record. Omitted attributes utilize the default if set.
+
+    ### Example request:
+
+    ```http
+    POST /schema/alpha_company/table/Computer/record HTTP/1.1
+    Host: fakeservices.datajoint.io
+    Accept: application/json
+    Authorization: Bearer <token>
 
-            **Example successful response**:
-
-            .. sourcecode:: http
-
-                HTTP/1.1 200 OK
-                Vary: Accept
-                Content-Type: text/plain
-
-                {
-                    "response": "Update Successful"
-                }
-
-            **Example unexpected response**:
-
-            .. sourcecode:: http
-
-                HTTP/1.1 500 Internal Server Error
-                Vary: Accept
-                Content-Type: text/plain
-
-                400 Bad Request: The browser (or proxy) sent a request that this server could
-                    not understand.
+    {
+        "records": [
+            {
+                "computer_id": "ffffffff-86d5-4af7-a013-89bde75528bd",
+                "computer_serial": "ZYXWVEISJ",
+                "computer_brand": "HP",
+                "computer_built": "2021-01-01",
+                "computer_processor": 2.7,
+                "computer_memory": 32,
+                "computer_weight": 3.7,
+                "computer_cost": 599.99,
+                "computer_preowned": 0,
+                "computer_purchased": "2021-02-01 13:00:00",
+                "computer_updates": 0
+            }
+        ]
+    }
+    ```
 
-            :reqheader Authorization: Bearer <OAuth2_token>
-            :resheader Content-Type: text/plain
-            :statuscode 200: No error.
-            :statuscode 500: Unexpected error encountered. Returns the error message as a
-                string.
+    ### Example successful response:
 
-        .. http:delete:: /schema/{schema_name}/table/{table_name}/record
+    ```http
+    HTTP/1.1 200 OK
+    Vary: Accept
+    Content-Type: text/plain
 
-            Route to delete a specific record.
+    {
+        "response": "Insert Successful"
+    }
+    ```
 
-            **Example request**:
+    ### Example unexpected response:
 
-            .. sourcecode:: http
+    ```http
+    HTTP/1.1 500 Internal Server Error
+    Vary: Accept
+    Content-Type: text/plain
 
-                DELETE /schema/alpha_company/table/Computer/record?cascade=false&"""
-        "restriction=W3siYXR0cmlidXRlTmFtZSI6ICJjb21wdXRlcl9tZW1vcnkiLCAib3BlcmF0aW9uIjogIj49"
-        "IiwgInZhbHVlIjogMTZ9XQo="
-        """ HTTP/1.1
-                Host: fakeservices.datajoint.io
-                Authorization: Bearer <token>
+    400 Bad Request: The browser (or proxy) sent a request that this server could
+        not understand.
+    ```
 
-            **Example successful response**:
+    #### Request Headers
+    * Authorization: Bearer <OAuth2_token\>
 
-            .. sourcecode:: http
+    #### Response Headers
+    * Content-Type: text/plain
 
-                HTTP/1.1 200 OK
-                Vary: Accept
-                Content-Type: text/plain
+    #### Status Codes
+    * 200 OK: No error.
+    * 500 Internal Server Error: Unexpected error encountered. Returns the error message as a
+        string.
 
-                {
-                    "response": "Delete Successful"
-                }
+    ## PATCH /schema/{schema_name}/table/{table_name}/record
 
-            **Example conflict response**:
+    Route to update a record. Omitted attributes utilize the default if set.
 
-            .. sourcecode:: http
+    ### Example request:
 
-                HTTP/1.1 409 Conflict
-                Vary: Accept
-                Content-Type: application/json
-
-                {
-                    "error": "IntegrityError",
-                    "error_msg": "Cannot delete or update a parent row: a foreign key
-                        constraint fails (`alpha_company`.`#employee`, CONSTRAINT
-                        `#employee_ibfk_1` FOREIGN KEY (`computer_id`) REFERENCES `computer`
-                        (`computer_id`) ON DELETE RESTRICT ON UPDATE CASCADE",
-                    "child_schema": "alpha_company",
-                    "child_table": "Employee"
-                }
+    ```http
+    PATCH /schema/alpha_company/table/Computer/record HTTP/1.1
+    Host: fakeservices.datajoint.io
+    Accept: application/json
+    Authorization: Bearer <token>
 
-            **Example unexpected response**:
-
-            .. sourcecode:: http
+    {
+        "records": [
+            {
+                "computer_id": "ffffffff-86d5-4af7-a013-89bde75528bd",
+                "computer_serial": "ZYXWVEISJ",
+                "computer_brand": "HP",
+                "computer_built": "2021-01-01",
+                "computer_processor": 2.7,
+                "computer_memory": 32,
+                "computer_weight": 3.7,
+                "computer_cost": 601.01,
+                "computer_preowned": 0,
+                "computer_purchased": "2021-02-01 13:00:00",
+                "computer_updates": 0
+            }
+        ]
+    }
+    ```
+
+    ### Example successful response:
+
+    ```http
+    HTTP/1.1 200 OK
+    Vary: Accept
+    Content-Type: text/plain
+
+    {
+        "response": "Update Successful"
+    }
+    ```
+
+    ### Example unexpected response:
+
+    ```http
+    HTTP/1.1 500 Internal Server Error
+    Vary: Accept
+    Content-Type: text/plain
+
+    400 Bad Request: The browser (or proxy) sent a request that this server could
+        not understand.
+    ```
+
+    #### Request Headers
+    * Authorization: Bearer <OAuth2_token\>
+
+    #### Response Headers
+    * Content-Type: text/plain
+
+    #### Status Codes
+    * 200 OK: No error.
+    * 500 Internal Server Error: Unexpected error encountered. Returns the error message as a
+        string.
+
+    ## DELETE /schema/{schema_name}/table/{table_name}/record
+
+    Route to delete a specific record.
+
+    ### Example request:
+
+    ```http
+    DELETE /schema/alpha_company/table/Computer/record?cascade=false&restriction=
+        W3siYXR0cmlidXRlTmFtZSI6ICJjb21wdXRlcl9tZW1vcnkiLCAib3BlcmF0aW9uIjogIj49IiwgInZhbHVlI
+        jogMTZ9XQo= HTTP/1.1
+    Host: fakeservices.datajoint.io
+    Authorization: Bearer <token>
+    ```
+
+    ### Example successful response:
+
+    ```http
+    HTTP/1.1 200 OK
+    Vary: Accept
+    Content-Type: text/plain
+
+    {
+        "response": "Delete Successful"
+    }
+    ```
+
+    ### Example conflict response:
+
+    ```http
+    HTTP/1.1 409 Conflict
+    Vary: Accept
+    Content-Type: application/json
+
+    {
+        "error": "IntegrityError",
+        "error_msg": "Cannot delete or update a parent row: a foreign key
+            constraint fails (`alpha_company`.`#employee`, CONSTRAINT
+            `#employee_ibfk_1` FOREIGN KEY (`computer_id`) REFERENCES `computer`
+            (`computer_id`) ON DELETE RESTRICT ON UPDATE CASCADE",
+        "child_schema": "alpha_company",
+        "child_table": "Employee"
+    }
+    ```
+
+    ### Example unexpected response:
+
+    ```http
+    HTTP/1.1 500 Internal Server Error
+    Vary: Accept
+    Content-Type: text/plain
+
+    400 Bad Request: The browser (or proxy) sent a request that this server could
+        not understand.
+    ```
+
+    #### Query Parameters
+    * cascade: Enable cascading delete. Accepts ``true`` or ``false``. Defaults to
+        ``false``.
+    * restriction: Base64-encoded ``AND`` sequence of restrictions. For example,
+        you could restrict as ``[{"attributeName": "computer_memory", "operation": ">=",
+        "value": 16}]`` with this param set as
+        ``W3siYXR0cmlidXRlTmFtZSI6ICJjb21wdXRlcl9tZW1vcnkiLCAib3BlcmF0aW9uIjogIj49
+        IiwgInZhbHVlIjogMTZ9XQo=``. Defaults to no restriction.
+
+    #### Request Headers
+    * Authorization: Bearer <OAuth2_token\>
+
+    #### Response Headers
+    * Content-Type: text/plain, application/json
+
+    #### Status Codes
+    * 200 OK: No error.
+    * 409 Conflict: Attempting to delete a record with dependents while ``cascade``
+        set to ``false``.
+    * 500 Internal Server Error: Unexpected error encountered. Returns the error message as a
+        string.
 
-                HTTP/1.1 500 Internal Server Error
-                Vary: Accept
-                Content-Type: text/plain
-
-                400 Bad Request: The browser (or proxy) sent a request that this server could
-                    not understand.
-
-            :query cascade: Enable cascading delete. Accepts ``true`` or ``false``.
-                Defaults to ``false``.
-            :query restriction: Base64-encoded ``AND`` sequence of restrictions. For example,
-                you could restrict as ``[{"attributeName": "computer_memory", "operation": ``-
-                ``">=", "value": 16}]`` with this param set as
-                ``W3siYXR0cmlidXRlTmFtZSI6ICJjb21wdXRlcl9tZW1vcnkiLCAib3Bl``-
-                ``cmF0aW9uIjogIj49IiwgInZhbHVlIjogMTZ9XQo=``. Defaults to no restriction.
-            :reqheader Authorization: Bearer <OAuth2_token>
-            :resheader Content-Type: text/plain, application/json
-            :statuscode 200: No error.
-            :statuscode 409: Attempting to delete a record with dependents while ``cascade``
-                set to ``false``.
-            :statuscode 500: Unexpected error encountered. Returns the error message as a
-                string.
-        """
+    """
     )
     if request.method in {"GET", "HEAD"}:
         try:
             schema_virtual_module = dj.VirtualModule(
                 schema_name, schema_name, connection=connection
             )
 
@@ -812,74 +855,81 @@
     connection: dj.Connection,
     schema_name: str,
     table_name: str,
 ) -> str:
     """
     Handler for ``/schema/{schema_name}/table/{table_name}/definition`` route.
 
-    :param connection: User's DataJoint connection object
-    :type connection: dj.Connection
-    :param schema_name: Schema name.
-    :type schema_name: str
-    :param table_name: Table name.
-    :type table_name: str
-    :return: If successful then sends back definition for table otherwise returns error.
-    :rtype: str
-
-    .. http:get:: /schema/{schema_name}/table/{table_name}/definition
-
-        Route to get DataJoint table definition.
-
-        **Example request**:
-
-        .. sourcecode:: http
-
-            GET /schema/alpha_company/table/Computer/definition HTTP/1.1
-            Host: fakeservices.datajoint.io
-            Authorization: Bearer <token>
-
-        **Example successful response**:
-
-        .. sourcecode:: http
-
-            HTTP/1.1 200 OK
-            Vary: Accept
-            Content-Type: text/plain
-
-            # Computers that belong to the company
-            computer_id          : uuid                      # unique id
-            ---
-            computer_serial="ABC101" : varchar(9)            # manufacturer serial number
-            computer_brand       : enum('HP','Dell')         # manufacturer brand
-            computer_built       : date                      # manufactured date
-            computer_processor   : double                    # processing power in GHz
-            computer_memory      : int                       # RAM in GB
-            computer_weight      : float                     # weight in lbs
-            computer_cost        : decimal(6,2)              # purchased price
-            computer_preowned    : tinyint                   # purchased as new or used
-            computer_purchased   : datetime                  # purchased date and time
-            computer_updates=null : time                     # scheduled daily update timeslot
-            computer_accessories=null : longblob             # included additional accessories
-
-        **Example unexpected response**:
-
-        .. sourcecode:: http
-
-            HTTP/1.1 500 Internal Server Error
-            Vary: Accept
-            Content-Type: text/plain
-
-            400 Bad Request: The browser (or proxy) sent a request that this server could not
-                understand.
-
-        :reqheader Authorization: Bearer <OAuth2_token>
-        :resheader Content-Type: text/plain
-        :statuscode 200: No error.
-        :statuscode 500: Unexpected error encountered. Returns the error message as a string.
+    Args:
+        connection (dj.Connection): User's DataJoint connection object
+        schema_name (str): Schema name.
+        table_name (str): Table name.
+
+    Returns:
+        If successful, then sends back the definition for the table; otherwise,
+            returns an error.
+
+    ## GET /schema/{schema_name}/table/{table_name}/definition
+
+    Route to get DataJoint table definition.
+
+    ### Example request:
+
+    ```http
+    GET /schema/alpha_company/table/Computer/definition HTTP/1.1
+    Host: fakeservices.datajoint.io
+    Authorization: Bearer <token>
+    ```
+
+    ### Example successful response:
+
+    ```http
+    HTTP/1.1 200 OK
+    Vary: Accept
+    Content-Type: text/plain
+
+    # Computers that belong to the company
+    computer_id          : uuid                      # unique id
+    ---
+    computer_serial="ABC101" : varchar(9)            # manufacturer serial number
+    computer_brand       : enum('HP','Dell')         # manufacturer brand
+    computer_built       : date                      # manufactured date
+    computer_processor   : double                    # processing power in GHz
+    computer_memory      : int                       # RAM in GB
+    computer_weight      : float                     # weight in lbs
+    computer_cost        : decimal(6,2)              # purchased price
+    computer_preowned    : tinyint                   # purchased as new or used
+    computer_purchased   : datetime                  # purchased date and time
+    computer_updates=null : time                     # scheduled daily update timeslot
+    computer_accessories=null : longblob             # included additional accessories
+    ```
+
+    ### Example unexpected response:
+
+    ```http
+    HTTP/1.1 500 Internal Server Error
+    Vary: Accept
+    Content-Type: text/plain
+
+    400 Bad Request: The browser (or proxy) sent a request that this server could not
+        understand.
+    ```
+
+    #### Request Headers
+    * Authorization: Bearer <OAuth2_token\>
+
+    #### Response Headers
+    * Content-Type: text/plain
+
+    #### Status Codes
+    * 200 OK: No error.
+    * 500 Internal Server Error: Unexpected error encountered. Returns the error message as a
+        string.
     """
+
     if request.method in {"GET", "HEAD"}:
         try:
             table_definition = _DJConnector._get_table_definition(
                 connection, schema_name, table_name
             )
             return table_definition
         except Exception:
@@ -895,159 +945,166 @@
     connection: dj.Connection,
     schema_name: str,
     table_name: str,
 ) -> dict:
     """
     Handler for ``/schema/{schema_name}/table/{table_name}/attribute`` route.
 
-    :param connection: User's DataJoint connection object
-    :type connection: dj.Connection
-    :param schema_name: Schema name.
-    :type schema_name: str
-    :param table_name: Table name.
-    :type table_name: str
-    :return: If successful then sends back dict of table attributes otherwise returns error.
-    :rtype: dict
-
-    .. http:GET:: /schema/{schema_name}/table/{table_name}/attribute
-
-        Route to get metadata on table attributes.
-
-        **Example request**:
-
-        .. sourcecode:: http
-
-            GET /schema/alpha_company/table/Computer/attribute HTTP/1.1
-            Host: fakeservices.datajoint.io
-            Authorization: Bearer <token>
-
-        **Example successful response**:
-
-        .. sourcecode:: http
-
-            HTTP/1.1 200 OK
-            Vary: Accept
-            Content-Type: application/json
-
-            {
-                "attributeHeader": [
-                    "name",
-                    "type",
-                    "nullable",
-                    "default",
-                    "autoincrement"
+    Args:
+        connection (dj.Connection): User's DataJoint connection object
+        schema_name (str): Schema name.
+        table_name (str): Table name.
+
+    Returns:
+        If successful, then sends back a dictionary of table attributes; otherwise,
+            returns an error.
+
+    ## GET /schema/{schema_name}/table/{table_name}/attribute
+
+    Route to get metadata on table attributes.
+
+    ### Example request:
+
+    ```http
+    GET /schema/alpha_company/table/Computer/attribute HTTP/1.1
+    Host: fakeservices.datajoint.io
+    Authorization: Bearer <token>
+    ```
+
+    ### Example successful response:
+
+    ```http
+    HTTP/1.1 200 OK
+    Vary: Accept
+    Content-Type: application/json
+
+    {
+        "attributeHeader": [
+            "name",
+            "type",
+            "nullable",
+            "default",
+            "autoincrement"
+        ],
+        "attributes": {
+            "primary": [
+                [
+                    "computer_id",
+                    "uuid",
+                    false,
+                    null,
+                    false
+                ]
+            ],
+            "secondary": [
+                [
+                    "computer_serial",
+                    "varchar(9)",
+                    false,
+                    ""ABC101"",
+                    false
                 ],
-                "attributes": {
-                    "primary": [
-                        [
-                            "computer_id",
-                            "uuid",
-                            false,
-                            null,
-                            false
-                        ]
-                    ],
-                    "secondary": [
-                        [
-                            "computer_serial",
-                            "varchar(9)",
-                            false,
-                            "\"ABC101\"",
-                            false
-                        ],
-                        [
-                            "computer_brand",
-                            "enum('HP','Dell')",
-                            false,
-                            null,
-                            false
-                        ],
-                        [
-                            "computer_built",
-                            "date",
-                            false,
-                            null,
-                            false
-                        ],
-                        [
-                            "computer_processor",
-                            "double",
-                            false,
-                            null,
-                            false
-                        ],
-                        [
-                            "computer_memory",
-                            "int",
-                            false,
-                            null,
-                            false
-                        ],
-                        [
-                            "computer_weight",
-                            "float",
-                            false,
-                            null,
-                            false
-                        ],
-                        [
-                            "computer_cost",
-                            "decimal(6,2)",
-                            false,
-                            null,
-                            false
-                        ],
-                        [
-                            "computer_preowned",
-                            "tinyint",
-                            false,
-                            null,
-                            false
-                        ],
-                        [
-                            "computer_purchased",
-                            "datetime",
-                            false,
-                            null,
-                            false
-                        ],
-                        [
-                            "computer_updates",
-                            "time",
-                            true,
-                            "null",
-                            false
-                        ],
-                        [
-                            "computer_accessories",
-                            "longblob",
-                            true,
-                            "null",
-                            false
-                        ]
-                    ]
-                }
-            }
-
-        **Example unexpected response**:
-
-        .. sourcecode:: http
-
-            HTTP/1.1 500 Internal Server Error
-            Vary: Accept
-            Content-Type: text/plain
-
-            400 Bad Request: The browser (or proxy) sent a request that this server could not
-                understand.
-
-        :reqheader Authorization: Bearer <OAuth2_token>
-        :resheader Content-Type: text/plain, application/json
-        :statuscode 200: No error.
-        :statuscode 500: Unexpected error encountered. Returns the error message as a string.
+                [
+                    "computer_brand",
+                    "enum('HP','Dell')",
+                    false,
+                    null,
+                    false
+                ],
+                [
+                    "computer_built",
+                    "date",
+                    false,
+                    null,
+                    false
+                ],
+                [
+                    "computer_processor",
+                    "double",
+                    false,
+                    null,
+                    false
+                ],
+                [
+                    "computer_memory",
+                    "int",
+                    false,
+                    null,
+                    false
+                ],
+                [
+                    "computer_weight",
+                    "float",
+                    false,
+                    null,
+                    false
+                ],
+                [
+                    "computer_cost",
+                    "decimal(6,2)",
+                    false,
+                    null,
+                    false
+                ],
+                [
+                    "computer_preowned",
+                    "tinyint",
+                    false,
+                    null,
+                    false
+                ],
+                [
+                    "computer_purchased",
+                    "datetime",
+                    false,
+                    null,
+                    false
+                ],
+                [
+                    "computer_updates",
+                    "time",
+                    true,
+                    "null",
+                    false
+                ],
+                [
+                    "computer_accessories",
+                    "longblob",
+                    true,
+                    "null",
+                    false
+                ]
+            ]
+        }
+    }
+    ```
+
+    ### Example unexpected response:
+
+    ```http
+    HTTP/1.1 500 Internal Server Error
+    Vary: Accept
+    Content-Type: text/plain
+
+    400 Bad Request: The browser (or proxy) sent a request that this server could not
+        understand.
+    ```
+
+    #### Request Headers
+    * Authorization: Bearer <OAuth2_token\>
+
+    #### Response Headers
+    * Content-Type: text/plain, application/json
+
+    #### Status Codes
+    * 200 OK: No error.
+    * 500 Internal Server Error: Unexpected error encountered. Returns the error message as a
+        string.
     """
+
     if request.method in {"GET", "HEAD"}:
         try:
             local_values = locals()
             local_values[schema_name] = dj.VirtualModule(
                 schema_name, schema_name, connection=connection
             )
 
@@ -1099,90 +1156,95 @@
 def dependency(
     connection: dj.Connection,
     schema_name: str,
     table_name: str,
 ) -> dict:
     (
         """
-        Handler for ``/schema/{schema_name}/table/{table_name}/dependency`` route.
+    Handler for ``/schema/{schema_name}/table/{table_name}/dependency`` route.
 
-        :param connection: User's DataJoint connection object
-        :type connection: dj.Connection
-        :param schema_name: Schema name.
-        :type schema_name: str
-        :param table_name: Table name.
-        :type table_name: str
-        :return: If sucessfuly sends back a list of dependencies otherwise returns error.
-        :rtype: dict
-
-        .. http:get:: /schema/{schema_name}/table/{table_name}/dependency
-
-            Route to get the metadata in relation to the dependent records associated with """
-        """a restricted subset of a table.
-
-            **Example request**:
-
-            .. sourcecode:: http
-
-                GET /schema/alpha_company/table/Computer/dependency?restriction=W3siYXR0cml"""
-        "idXRlTmFtZSI6ICJjb21wdXRlcl9tZW1vcnkiLCAib3BlcmF0aW9uIjogIj49IiwgInZhbHVlIjogMTZ9XQo"
-        "="
-        """ HTTP/1.1
-                Host: fakeservices.datajoint.io
-                Authorization: Bearer <token>
-
-            **Example successful response**:
-
-            .. sourcecode:: http
-
-                HTTP/1.1 200 OK
-                Vary: Accept
-                Content-Type: application/json
-
-                {
-                    "dependencies": [
-                        {
-                            "accessible": true,
-                            "count": 2,
-                            "schema": "alpha_company",
-                            "table": "computer"
-                        },
-                        {
-                            "accessible": true,
-                            "count": 2,
-                            "schema": "alpha_company",
-                            "table": "#employee"
-                        }
-                    ]
-                }
+    Args:
+        connection (dj.Connection): User's DataJoint connection object
+        schema_name (str): Schema name.
+        table_name (str): Table name.
 
-            **Example unexpected response**:
+    Returns:
+        If successful, then sends back a list of dependencies; otherwise, returns an error.
 
-            .. sourcecode:: http
+    ## GET /schema/{schema_name}/table/{table_name}/dependency
 
-                HTTP/1.1 500 Internal Server Error
-                Vary: Accept
-                Content-Type: text/plain
-
-                400 Bad Request: The browser (or proxy) sent a request that this server could
-                    not understand.
-
-            :query schema_name: Schema name.
-            :query table_name: Table name.
-            :query restriction: Base64-encoded ``AND`` sequence of restrictions. For example,
-                you could restrict as ``[{"attributeName": "computer_memory", "operation": ``-
-                ``">=", "value": 16}]`` with this param set as
-                ``W3siYXR0cmlidXRlTmFtZSI6ICJjb21wdXRlcl9tZW1vcnkiLCAib3Bl``-
-                ``cmF0aW9uIjogIj49IiwgInZhbHVlIjogMTZ9XQo=``. Defaults to no restriction.
-            :reqheader Authorization: Bearer <OAuth2_token>
-            :resheader Content-Type: text/plain, application/json
-            :statuscode 200: No error.
-            :statuscode 500: Unexpected error encountered. Returns the error message as a
-                string.
-        """
+    Route to get the metadata in relation to the dependent records associated with a
+        restricted subset of a table.
+
+    ### Example request:
+
+    ```http
+    GET /schema/alpha_company/table/Computer/dependency?restriction=
+        W3siYXR0cmlidXRlTmFtZSI6ICJjb21wdXRlcl9tZW1vcnkiLCAib3BlcmF0aW9uIjogIj49IiwgInZ=
+        HTTP/1.1
+    Host: fakeservices.datajoint.io
+    Authorization: Bearer <token>
+    ```
+
+    ### Example successful response:
+
+    ```http
+    HTTP/1.1 200 OK
+    Vary: Accept
+    Content-Type: application/json
+
+    {
+        "dependencies": [
+            {
+                "accessible": true,
+                "count": 2,
+                "schema": "alpha_company",
+                "table": "computer"
+            },
+            {
+                "accessible": true,
+                "count": 2,
+                "schema": "alpha_company",
+                "table": "#employee"
+            }
+        ]
+    }
+    ```
+
+    ### Example unexpected response:
+
+    ```http
+    HTTP/1.1 500 Internal Server Error
+    Vary: Accept
+    Content-Type: text/plain
+
+    400 Bad Request: The browser (or proxy) sent a request that this server could not
+        understand.
+    ```
+
+    #### Query Parameters
+    * schema_name: Schema name.
+    * table_name: Table name.
+    * restriction: Base64-encoded ``AND`` sequence of restrictions. For example, you could
+        restrict as ``[{"attributeName": "computer_memory", "operation": ">=", "value": 16}]``
+        with this param set as
+        ``W3siYXR0cmlidXRlTmFtZSI6ICJjb21wdXRlcl9tZW1vcnkiLCAib3BlcmF0aW9uIjogIj49IiwgInZ=``.
+        Defaults to no restriction.
+
+    #### Request Headers
+    * Authorization: Bearer <OAuth2_token\>
+
+    #### Response Headers
+    * Content-Type: text/plain, application/json
+
+    #### Status Codes
+    * 200 OK: No error.
+    * 500 Internal Server Error: Unexpected error encountered. Returns the error message as a
+        string.
+    """
     )
     if request.method in {"GET", "HEAD"}:
         # Get dependencies
         try:
             dependencies = _DJConnector._record_dependency(
                 connection,
                 schema_name,
```

### Comparing `pharus-0.8.6/pharus.egg-info/PKG-INFO` & `pharus-0.8.7/pharus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pharus
-Version: 0.8.6
+Version: 0.8.7
 Summary: A generic REST API server backend for DataJoint pipelines.
 Home-page: https://github.com/datajoint/pharus
 Author: DataJoint Neuro
 Author-email: support@vathes.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/x-rst
```

### Comparing `pharus-0.8.6/setup.py` & `pharus-0.8.7/setup.py`

 * *Files identical despite different names*

