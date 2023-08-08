# Comparing `tmp/license_manager_cli-2.3.2.tar.gz` & `tmp/license_manager_cli-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "license_manager_cli-2.3.2.tar", max compression
+gzip compressed data, was "license_manager_cli-3.0.0.tar", max compression
```

## Comparing `license_manager_cli-2.3.2.tar` & `license_manager_cli-3.0.0.tar`

### file list

```diff
@@ -1,20 +1,23 @@
--rw-r--r--   0        0        0     1082 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/LICENSE
--rw-r--r--   0        0        0     7574 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/README.rst
--rw-r--r--   0        0        0        0 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/lm_cli/__init__.py
--rw-r--r--   0        0        0    10990 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/lm_cli/auth.py
--rw-r--r--   0        0        0     2937 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/lm_cli/config.py
--rw-r--r--   0        0        0      299 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/lm_cli/constants.py
--rw-r--r--   0        0        0     2569 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/lm_cli/exceptions.py
--rw-r--r--   0        0        0      675 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/lm_cli/logs.py
--rw-r--r--   0        0        0     5684 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/lm_cli/main.py
--rw-r--r--   0        0        0     4560 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/lm_cli/render.py
--rw-r--r--   0        0        0     7100 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/lm_cli/requests.py
--rw-r--r--   0        0        0     3716 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/lm_cli/schemas.py
--rw-r--r--   0        0        0        0 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/lm_cli/subapps/__init__.py
--rw-r--r--   0        0        0     1734 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/lm_cli/subapps/bookings.py
--rw-r--r--   0        0        0     5971 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/lm_cli/subapps/configurations.py
--rw-r--r--   0        0        0     1680 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/lm_cli/subapps/licenses.py
--rw-r--r--   0        0        0     1147 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/lm_cli/text_tools.py
--rw-r--r--   0        0        0     3516 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/lm_cli/time_loop.py
--rw-r--r--   0        0        0     1833 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/pyproject.toml
--rw-r--r--   0        0        0     8868 1970-01-01 00:00:00.000000 license_manager_cli-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-08-08 21:22:41.335960 license_manager_cli-3.0.0/LICENSE
+-rw-r--r--   0        0        0     7574 2023-08-08 21:22:41.335960 license_manager_cli-3.0.0/README.rst
+-rw-r--r--   0        0        0        0 2023-08-08 21:22:41.335960 license_manager_cli-3.0.0/lm_cli/__init__.py
+-rw-r--r--   0        0        0    10456 2023-08-08 21:22:41.335960 license_manager_cli-3.0.0/lm_cli/auth.py
+-rw-r--r--   0        0        0     2897 2023-08-08 21:22:41.335960 license_manager_cli-3.0.0/lm_cli/config.py
+-rw-r--r--   0        0        0      565 2023-08-08 21:22:41.335960 license_manager_cli-3.0.0/lm_cli/constants.py
+-rw-r--r--   0        0        0     2569 2023-08-08 21:22:41.335960 license_manager_cli-3.0.0/lm_cli/exceptions.py
+-rw-r--r--   0        0        0      675 2023-08-08 21:22:41.335960 license_manager_cli-3.0.0/lm_cli/logs.py
+-rw-r--r--   0        0        0     5998 2023-08-08 21:22:41.335960 license_manager_cli-3.0.0/lm_cli/main.py
+-rw-r--r--   0        0        0     4560 2023-08-08 21:22:41.335960 license_manager_cli-3.0.0/lm_cli/render.py
+-rw-r--r--   0        0        0     7143 2023-08-08 21:22:41.335960 license_manager_cli-3.0.0/lm_cli/requests.py
+-rw-r--r--   0        0        0     1760 2023-08-08 21:22:41.335960 license_manager_cli-3.0.0/lm_cli/schemas.py
+-rw-r--r--   0        0        0        0 2023-08-08 21:22:41.335960 license_manager_cli-3.0.0/lm_cli/subapps/__init__.py
+-rw-r--r--   0        0        0     1625 2023-08-08 21:22:41.335960 license_manager_cli-3.0.0/lm_cli/subapps/bookings.py
+-rw-r--r--   0        0        0     5603 2023-08-08 21:22:41.335960 license_manager_cli-3.0.0/lm_cli/subapps/configurations.py
+-rw-r--r--   0        0        0     5364 2023-08-08 21:22:41.335960 license_manager_cli-3.0.0/lm_cli/subapps/features.py
+-rw-r--r--   0        0        0     2203 2023-08-08 21:22:41.335960 license_manager_cli-3.0.0/lm_cli/subapps/jobs.py
+-rw-r--r--   0        0        0     4329 2023-08-08 21:22:41.335960 license_manager_cli-3.0.0/lm_cli/subapps/license_servers.py
+-rw-r--r--   0        0        0     3907 2023-08-08 21:22:41.335960 license_manager_cli-3.0.0/lm_cli/subapps/products.py
+-rw-r--r--   0        0        0     1147 2023-08-08 21:22:41.335960 license_manager_cli-3.0.0/lm_cli/text_tools.py
+-rw-r--r--   0        0        0     3516 2023-08-08 21:22:41.335960 license_manager_cli-3.0.0/lm_cli/time_loop.py
+-rw-r--r--   0        0        0     1833 2023-08-08 21:22:41.339959 license_manager_cli-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     8868 1970-01-01 00:00:00.000000 license_manager_cli-3.0.0/PKG-INFO
```

### Comparing `license_manager_cli-2.3.2/LICENSE` & `license_manager_cli-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `license_manager_cli-2.3.2/README.rst` & `license_manager_cli-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `license_manager_cli-2.3.2/lm_cli/auth.py` & `license_manager_cli-3.0.0/lm_cli/auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 """
 Utilities for handling auth in lm-cli.
 """
 
 from time import sleep
 from typing import Dict, Optional, cast
 
-import pydantic
 from jose import jwt
 from jose.exceptions import ExpiredSignatureError
 from loguru import logger
 
 from lm_cli.config import settings
 from lm_cli.exceptions import Abort, LicenseManagerCliError
 from lm_cli.render import terminal_message
 from lm_cli.requests import make_request
-from lm_cli.schemas import DeviceCodeData, IdentityData, LicenseManagerContext, Persona, TokenSet
+from lm_cli.schemas import DeviceCodeData, LicenseManagerContext, Persona, TokenSet
 from lm_cli.text_tools import unwrap
 from lm_cli.time_loop import TimeLoop
 
 
-def validate_token_and_extract_identity(token_set: TokenSet) -> IdentityData:
+def validate_token_and_extract_identity(token_set: TokenSet) -> str:
     """
     Validate the access_token from a TokenSet and extract the identity data.
 
     Validations:
         * Checks if access_token is not empty.
         * Checks timestamp on the access token.
         * Checks for identity data.
@@ -69,38 +68,26 @@
             subject="Invalid access token.",
             support=True,
             log_message=f"Unknown error while validating access access token: {err}.",
             original_error=err,
         )
 
     logger.debug("Extracting identity data from the access token.")
-    user_email = token_data.get(settings.IDENTITY_CLAIMS_KEY)
-    identity_claims = {"user_email": user_email}
+    user_email = token_data.get("email")
 
     Abort.require_condition(
-        identity_claims,
+        user_email,
         "No identity data found in access token data.",
         raise_kwargs=dict(
             subject="No identity found.",
             support=True,
         ),
     )
-    try:
-        return IdentityData.parse_obj(identity_claims)
-    except pydantic.ValidationError as err:
-        raise Abort(
-            """
-            The identity data in the access token is malformed or incomplete.
 
-            Please try logging in again.
-            """,
-            subject="Invalid identity data.",
-            support=True,
-            log_message=f"Identity data is incomplete: {err}.",
-        )
+    return user_email
 
 
 def load_tokens_from_cache() -> TokenSet:
     """
     Load an access token (and a refresh token if one exists) from the cache.
     """
 
@@ -170,36 +157,36 @@
 
     Returns the persona.
     """
     if token_set is None:
         token_set = load_tokens_from_cache()
 
     try:
-        identity_data = validate_token_and_extract_identity(token_set)
+        user_email = validate_token_and_extract_identity(token_set)
     except ExpiredSignatureError:
         Abort.require_condition(
             token_set.refresh_token is not None,
             "The auth token is expired. Please retrieve a new and log in again.",
             raise_kwargs=dict(
                 subject="Expired access token.",
                 support=True,
             ),
         )
 
         logger.debug("The access token is expired. Attempting to refresh token.")
         refresh_access_token(ctx, token_set)
-        identity_data = validate_token_and_extract_identity(token_set)
+        user_email = validate_token_and_extract_identity(token_set)
 
-    logger.debug(f"Persona created with identity data: {identity_data}.")
+    logger.debug(f"Persona created with identity data: {user_email}.")
 
     save_tokens_to_cache(token_set)
 
     return Persona(
         token_set=token_set,
-        identity_data=identity_data,
+        user_email=user_email,
     )
 
 
 def refresh_access_token(ctx: LicenseManagerContext, token_set: TokenSet):
     """
     Attempt to fetch a new access token given a refresh token in a token_set.
```

### Comparing `license_manager_cli-2.3.2/lm_cli/config.py` & `license_manager_cli-3.0.0/lm_cli/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,14 @@
     # OIDC config for machine-to-machine security
     OIDC_DOMAIN: str
     OIDC_LOGIN_DOMAIN: Optional[str]
     OIDC_AUDIENCE: str
     OIDC_CLIENT_ID: str
     OIDC_MAX_POLL_TIME: int = 5 * 60  # 5 Minutes
 
-    IDENTITY_CLAIMS_KEY: str = "email"
-
     @root_validator(skip_on_failure=True)
     def compute_extra_settings(cls, values):
         """
         Compute settings values that are based on other settings values.
         """
         cache_dir = values["LM_CACHE_DIR"]
         cache_dir.mkdir(exist_ok=True, parents=True)
```

### Comparing `license_manager_cli-2.3.2/lm_cli/exceptions.py` & `license_manager_cli-3.0.0/lm_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-2.3.2/lm_cli/logs.py` & `license_manager_cli-3.0.0/lm_cli/logs.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-2.3.2/lm_cli/main.py` & `license_manager_cli-3.0.0/lm_cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,23 +13,29 @@
 from lm_cli.config import settings
 from lm_cli.exceptions import Abort, handle_abort
 from lm_cli.logs import init_logs
 from lm_cli.render import render_json, terminal_message
 from lm_cli.schemas import LicenseManagerContext, Persona, TokenSet
 from lm_cli.subapps.bookings import app as bookings_app
 from lm_cli.subapps.configurations import app as configurations_app
-from lm_cli.subapps.licenses import app as licenses_app
+from lm_cli.subapps.features import app as features_app
+from lm_cli.subapps.jobs import app as jobs_app
+from lm_cli.subapps.license_servers import app as license_servers_app
+from lm_cli.subapps.products import app as products_app
 from lm_cli.text_tools import conjoin, copy_to_clipboard
 
 
 app = typer.Typer()
 
-app.add_typer(licenses_app, name="licenses")
 app.add_typer(bookings_app, name="bookings")
 app.add_typer(configurations_app, name="configurations")
+app.add_typer(features_app, name="features")
+app.add_typer(jobs_app, name="jobs")
+app.add_typer(license_servers_app, name="license-servers")
+app.add_typer(products_app, name="products")
 
 
 @app.callback(invoke_without_command=True)
 @handle_abort
 def main(
     ctx: typer.Context,
     verbose: bool = typer.Option(False, help="Enable verbose logging to the terminal"),
@@ -37,15 +43,15 @@
 ):
     """
     Welcome to the License Manager CLI!
 
     More information can be shown for each command listed below by running it with the --help option.
     """
     if version:
-        typer.echo(importlib_metadata.version("lm-cli"))
+        typer.echo(importlib_metadata.version("license-manager-cli"))
         raise typer.Exit()
 
     if ctx.invoked_subcommand is None:
         terminal_message(
             conjoin(
                 "No command provided. Please check the [bold magenta]usage[/bold magenta] and add a command",
                 "",
@@ -80,15 +86,15 @@
 def login(ctx: typer.Context):
     """
     Log in to the lm-cli by storing the supplied token argument in the cache.
     """
     token_set: TokenSet = fetch_auth_tokens(ctx.obj)
     persona: Persona = init_persona(ctx.obj, token_set)
     terminal_message(
-        f"User was logged in with email '{persona.identity_data.user_email}'",
+        f"User was logged in with email '{persona.user_email}'",
         subject="Logged in!",
     )
 
 
 @app.command()
 @handle_abort
 def logout():
```

### Comparing `license_manager_cli-2.3.2/lm_cli/render.py` & `license_manager_cli-3.0.0/lm_cli/render.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-2.3.2/lm_cli/requests.py` & `license_manager_cli-3.0.0/lm_cli/requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
             original_error=err,
         )
 
     if expected_status is not None and response.status_code != expected_status:
         try:
             error_message_text = response.json()["detail"]
         except Exception:
-            error_message_text = response.text
+            error_message_text = f"{response.text} | status code: {response.status_code}"
 
         raise Abort(
             unwrap(
                 f"""
                 {abort_message}: Received an error response. Error message: [red]{error_message_text}[/red].
                 """
             ),
```

### Comparing `license_manager_cli-2.3.2/lm_cli/subapps/bookings.py` & `license_manager_cli-3.0.0/lm_cli/subapps/bookings.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,20 +12,16 @@
 from lm_cli.requests import make_request, parse_query_params
 from lm_cli.schemas import LicenseManagerContext
 
 
 style_mapper = StyleMapper(
     id="blue",
     job_id="white",
-    product_feature="green",
-    booked="cyan",
-    config_id="magenta",
-    lead_host="white",
-    user_name="red",
-    cluster_name="yellow",
+    feature_id="green",
+    quantity="cyan",
 )
 
 
 app = typer.Typer(help="Commands to interact with bookings.")
 
 
 @app.command("list")
@@ -47,15 +43,15 @@
 
     params = parse_query_params(search=search, sort_order=sort_order, sort_field=sort_field)
 
     data = cast(
         List,
         make_request(
             lm_ctx.client,
-            "/lm/api/v1/booking/all",
+            "/lm/bookings",
             "GET",
             expected_status=200,
             abort_message="Couldn't retrieve booking list from API",
             support=True,
             params=params,
         ),
     )
```

### Comparing `license_manager_cli-2.3.2/lm_cli/subapps/configurations.py` & `license_manager_cli-3.0.0/lm_cli/subapps/configurations.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,37 +2,60 @@
 A ``typer`` app that can interact with Configurations data in a cruddy manner.
 """
 
 from typing import Dict, List, Optional, cast
 
 import typer
 
-from lm_cli.constants import SortOrder
+from lm_cli.constants import LicenseServerType, SortOrder
 from lm_cli.exceptions import handle_abort
 from lm_cli.render import StyleMapper, render_list_results, render_single_result, terminal_message
 from lm_cli.requests import make_request, parse_query_params
-from lm_cli.schemas import ConfigurationCreateRequestData, LicenseManagerContext
-from lm_cli.text_tools import dedent
+from lm_cli.schemas import ConfigurationCreateSchema, LicenseManagerContext
 
 
 style_mapper = StyleMapper(
     id="blue",
     name="green",
-    product="cyan",
-    features="magenta",
-    license_servers="yellow",
-    license_server_type="white",
-    grace_time="red",
-    client_id="black",
+    cluster_client_id="cyan",
+    features="red",
+    license_servers="white",
+    grace_time="magenta",
+    type="yellow",
 )
 
 
 app = typer.Typer(help="Commands to interact with configurations.")
 
 
+def format_data(data):
+    """Return data in the correct format for printing."""
+    formatted_data = []
+
+    for configuration in data:
+        new_data = {}
+
+        new_data["id"] = configuration["id"]
+        new_data["name"] = configuration["name"]
+        new_data["cluster_client_id"] = configuration["cluster_client_id"]
+        new_data["features"] = ", ".join([feature["name"] for feature in configuration["features"]])
+        new_data["license_servers"] = ", ".join(
+            [
+                f"{license_server['host']}:{license_server['port']}"
+                for license_server in configuration["license_servers"]
+            ]
+        )
+        new_data["grace_time"] = f"{configuration['grace_time']} (seconds)"
+        new_data["type"] = configuration["type"]
+
+        formatted_data.append(new_data)
+
+    return formatted_data
+
+
 @app.command("list")
 @handle_abort
 def list_all(
     ctx: typer.Context,
     search: Optional[str] = typer.Option(None, help="Apply a search term to results."),
     sort_order: SortOrder = typer.Option(SortOrder.UNSORTED, help="Specify sort order."),
     sort_field: Optional[str] = typer.Option(None, help="The field by which results should be sorted."),
@@ -48,30 +71,27 @@
 
     params = parse_query_params(search=search, sort_order=sort_order, sort_field=sort_field)
 
     data = cast(
         List,
         make_request(
             lm_ctx.client,
-            "/lm/api/v1/config/all",
+            "/lm/configurations",
             "GET",
             expected_status=200,
             abort_message="Couldn't retrieve configuration list from API",
             support=True,
             params=params,
         ),
     )
 
-    # Add grace time measure unit to the results before printing
-    for configuration in data:
-        grace_time = str(configuration["grace_time"]) + " (seconds)"
-        configuration["grace_time"] = grace_time
+    formatted_data = format_data(data)
 
     render_list_results(
-        data,
+        formatted_data,
         title="Configurations List",
         style_mapper=style_mapper,
     )
 
 
 @app.command("get-one")
 @handle_abort
@@ -88,96 +108,67 @@
     assert lm_ctx is not None
     assert lm_ctx.client is not None
 
     result = cast(
         Dict,
         make_request(
             lm_ctx.client,
-            f"/lm/api/v1/config/{id}",
+            f"/lm/configurations/{id}",
             "GET",
             expected_status=200,
             abort_message="Couldn't get the configuration from the API",
             support=True,
         ),
     )
 
-    # Add grace time measure unit to the results before printing
-    grace_time = str(result["grace_time"]) + " (seconds)"
-    result["grace_time"] = grace_time
+    formatted_result = format_data([result])
 
     render_single_result(
-        result,
+        formatted_result[0],
         title=f"Configuration id {id}",
     )
 
 
 @app.command()
 @handle_abort
 def create(
     ctx: typer.Context,
     name: str = typer.Option(
         ...,
         help="The name of configuration to create.",
     ),
-    product: str = typer.Option(
+    cluster_client_id: str = typer.Option(
         ...,
-        help="The name of the product of the license.",
+        help="The cluster OIDC client_id of the cluster where the configuration is being added.",
     ),
-    features: str = typer.Option(
-        ...,
-        help=dedent(
-            """
-            The features of the license, with total quantity and limit.
-            Must be a string with a valid JSON object serialized.
-            Example: '{"feature1": {"total": 10, "limit": 10}, "feature2": {"total": 20, "limit": 10}}'
-            """
-        ),
-    ),
-    license_servers: str = typer.Option(
-        ...,
-        help=dedent(
-            """
-            The list of license servers connection strings, in order of preference.
-            Must be in the format <license_server_type>:<hostname>:<port>.
-            Use commas to concatenate in case there's more than one entry.
-            """
-        ),
-    ),
-    license_server_type: str = typer.Option(..., help="The license server type."),
     grace_time: int = typer.Option(
         ...,
         help="The grace time for jobs using the license. Must be in seconds.",
     ),
-    client_id: str = typer.Option(
-        ...,
-        help="The identification (client_id) of the cluster where the license is configured.",
-    ),
+    license_server_type: LicenseServerType = typer.Option(..., help="The license server type."),
 ):
     """
     Create a new configuration.
     """
     lm_ctx: LicenseManagerContext = ctx.obj
 
     # Make static type checkers happy
     assert lm_ctx is not None
     assert lm_ctx.client is not None
 
-    request_data = ConfigurationCreateRequestData(
+    request_data = ConfigurationCreateSchema(
         name=name,
-        product=product,
-        features=features,
-        license_servers=license_servers,
-        license_server_type=license_server_type,
+        cluster_client_id=cluster_client_id,
         grace_time=grace_time,
-        client_id=client_id,
+        type=license_server_type,
     )
 
     make_request(
         lm_ctx.client,
-        "/lm/api/v1/config/",
+        "/lm/configurations",
         "POST",
         expected_status=201,
         abort_message="Configuration creation failed",
         support=True,
         request_model=request_data,
     )
 
@@ -203,15 +194,15 @@
 
     # Make static type checkers happy
     assert lm_ctx is not None
     assert lm_ctx.client is not None
 
     make_request(
         lm_ctx.client,
-        f"/lm/api/v1/config/{id}",
+        f"/lm/configurations/{id}",
         "DELETE",
         expected_status=200,
         abort_message="Request to delete configuration was not accepted by the API",
         support=True,
     )
     terminal_message(
         "The configuration was deleted successfully.",
```

### Comparing `license_manager_cli-2.3.2/lm_cli/subapps/licenses.py` & `license_manager_cli-3.0.0/lm_cli/subapps/jobs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,80 @@
 """
-A ``typer`` app that can interact with Licenses endpoint to list data.
+A ``typer`` app that can interact with Jobs endpoint to list data.
 """
 
 from typing import List, Optional, cast
 
 import typer
 
 from lm_cli.constants import SortOrder
 from lm_cli.exceptions import handle_abort
 from lm_cli.render import StyleMapper, render_list_results
 from lm_cli.requests import make_request, parse_query_params
 from lm_cli.schemas import LicenseManagerContext
 
 
 style_mapper = StyleMapper(
-    product_feature="green",
-    used="cyan",
-    total="magenta",
-    booked="blue",
-    available="yellow",
+    id="blue",
+    slurm_job_id="white",
+    cluster_client_id="green",
+    username="cyan",
+    lead_host="magenta",
+    bookings="purple",
 )
 
 
-app = typer.Typer(help="Commands to interact with licenses.")
+app = typer.Typer(help="Commands to interact with jobs.")
 
 
 @app.command("list")
 @handle_abort
 def list_all(
     ctx: typer.Context,
     search: Optional[str] = typer.Option(None, help="Apply a search term to results."),
     sort_order: SortOrder = typer.Option(SortOrder.UNSORTED, help="Specify sort order."),
     sort_field: Optional[str] = typer.Option(None, help="The field by which results should be sorted."),
 ):
     """
-    Show license usage information.
+    Show job information.
     """
     lm_ctx: LicenseManagerContext = ctx.obj
 
     # Make static type checkers happy
     assert lm_ctx is not None
     assert lm_ctx.client is not None
 
     params = parse_query_params(search=search, sort_order=sort_order, sort_field=sort_field)
 
     data = cast(
         List,
         make_request(
             lm_ctx.client,
-            "/lm/api/v1/license/complete/all",
+            "/lm/jobs",
             "GET",
             expected_status=200,
-            abort_message="Couldn't retrieve license list from API",
+            abort_message="Couldn't retrieve job list from API",
             support=True,
             params=params,
         ),
     )
 
+    formatted_data = []
+
+    for job in data:
+        new_data = {}
+        new_data["id"] = job["id"]
+        new_data["slurm_job_id"] = job["slurm_job_id"]
+        new_data["cluster_client_id"] = job["cluster_client_id"]
+        new_data["username"] = job["username"]
+        new_data["lead_host"] = job["lead_host"]
+        new_data["bookings"] = " | ".join(
+            [f"feature_id: {booking['feature_id']}, quantity: {booking['quantity']}" for booking in job["bookings"]]
+        )
+
+        formatted_data.append(new_data)
+
     render_list_results(
-        data,
-        title="Licenses List",
+        formatted_data,
+        title="Jobs List",
         style_mapper=style_mapper,
     )
```

### Comparing `license_manager_cli-2.3.2/lm_cli/text_tools.py` & `license_manager_cli-3.0.0/lm_cli/text_tools.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-2.3.2/lm_cli/time_loop.py` & `license_manager_cli-3.0.0/lm_cli/time_loop.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-2.3.2/pyproject.toml` & `license_manager_cli-3.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "license-manager-cli"
-version = "2.3.2"
+version = "3.0.0"
 description = "License Manager CLI Client"
 authors = ["Omnivector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/omnivector-solutions/license-manager"
 documentation = "https://omnivector-solutions.github.io/license-manager/"
 packages = [ { include = "lm_cli" } ]
```

### Comparing `license_manager_cli-2.3.2/PKG-INFO` & `license_manager_cli-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: license-manager-cli
-Version: 2.3.2
+Version: 3.0.0
 Summary: License Manager CLI Client
 Home-page: https://github.com/omnivector-solutions/license-manager
 License: MIT
 Author: Omnivector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.6.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

