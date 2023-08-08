# Comparing `tmp/license_manager_agent-2.3.2.tar.gz` & `tmp/license_manager_agent-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "license_manager_agent-2.3.2.tar", max compression
+gzip compressed data, was "license_manager_agent-3.0.0.tar", max compression
```

## Comparing `license_manager_agent-2.3.2.tar` & `license_manager_agent-3.0.0.tar`

### file list

```diff
@@ -1,32 +1,35 @@
--rw-r--r--   0        0        0       23 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/README.rst
--rw-r--r--   0        0        0        0 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/__init__.py
--rw-r--r--   0        0        0    10818 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/backend_utils.py
--rw-r--r--   0        0        0     3473 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/config.py
--rw-r--r--   0        0        0     1048 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/exceptions.py
--rw-r--r--   0        0        0     4032 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/license_report.py
--rw-r--r--   0        0        0     2000 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/logs.py
--rw-r--r--   0        0        0        0 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/parsing/__init__.py
--rw-r--r--   0        0        0     1732 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/parsing/flexlm.py
--rw-r--r--   0        0        0     3537 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/parsing/lmx.py
--rw-r--r--   0        0        0     4416 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/parsing/lsdyna.py
--rw-r--r--   0        0        0     4758 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/parsing/olicense.py
--rw-r--r--   0        0        0     2197 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/parsing/rlm.py
--rwxr-xr-x   0        0        0     1048 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/reconcile.py
--rw-r--r--   0        0        0    10660 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/reconciliation.py
--rw-r--r--   0        0        0        0 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/server_interfaces/__init__.py
--rw-r--r--   0        0        0     2904 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/server_interfaces/flexlm.py
--rw-r--r--   0        0        0     1665 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/server_interfaces/license_server_interface.py
--rw-r--r--   0        0        0     2751 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/server_interfaces/lmx.py
--rw-r--r--   0        0        0     2727 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/server_interfaces/lsdyna.py
--rw-r--r--   0        0        0     2719 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/server_interfaces/olicense.py
--rw-r--r--   0        0        0     3739 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/server_interfaces/rlm.py
--rw-r--r--   0        0        0     1251 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/utils.py
--rw-r--r--   0        0        0        0 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/workload_managers/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 19:49:38.907070 license_manager_agent-2.3.2/lm_agent/workload_managers/slurm/__init__.py
--rw-r--r--   0        0        0     8376 2023-06-08 19:49:38.911070 license_manager_agent-2.3.2/lm_agent/workload_managers/slurm/cmd_utils.py
--rw-r--r--   0        0        0     1036 2023-06-08 19:49:38.911070 license_manager_agent-2.3.2/lm_agent/workload_managers/slurm/common.py
--rw-r--r--   0        0        0     3732 2023-06-08 19:49:38.911070 license_manager_agent-2.3.2/lm_agent/workload_managers/slurm/reservations.py
--rw-r--r--   0        0        0     1728 2023-06-08 19:49:38.911070 license_manager_agent-2.3.2/lm_agent/workload_managers/slurm/slurmctld_epilog.py
--rw-r--r--   0        0        0     3923 2023-06-08 19:49:38.911070 license_manager_agent-2.3.2/lm_agent/workload_managers/slurm/slurmctld_prolog.py
--rw-r--r--   0        0        0     2050 2023-06-08 19:49:38.911070 license_manager_agent-2.3.2/pyproject.toml
--rw-r--r--   0        0        0     1053 1970-01-01 00:00:00.000000 license_manager_agent-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0       23 2023-08-08 21:22:40.775421 license_manager_agent-3.0.0/README.rst
+-rw-r--r--   0        0        0        0 2023-08-08 21:22:40.775421 license_manager_agent-3.0.0/lm_agent/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 21:22:40.775421 license_manager_agent-3.0.0/lm_agent/backend_utils/__init__.py
+-rw-r--r--   0        0        0      288 2023-08-08 21:22:40.775421 license_manager_agent-3.0.0/lm_agent/backend_utils/constants.py
+-rw-r--r--   0        0        0     1808 2023-08-08 21:22:40.779421 license_manager_agent-3.0.0/lm_agent/backend_utils/models.py
+-rw-r--r--   0        0        0    10196 2023-08-08 21:22:40.779421 license_manager_agent-3.0.0/lm_agent/backend_utils/utils.py
+-rw-r--r--   0        0        0     3473 2023-08-08 21:22:40.779421 license_manager_agent-3.0.0/lm_agent/config.py
+-rw-r--r--   0        0        0     1150 2023-08-08 21:22:40.779421 license_manager_agent-3.0.0/lm_agent/exceptions.py
+-rw-r--r--   0        0        0     4161 2023-08-08 21:22:40.779421 license_manager_agent-3.0.0/lm_agent/license_report.py
+-rw-r--r--   0        0        0     2519 2023-08-08 21:22:40.779421 license_manager_agent-3.0.0/lm_agent/logs.py
+-rw-r--r--   0        0        0        0 2023-08-08 21:22:40.779421 license_manager_agent-3.0.0/lm_agent/parsing/__init__.py
+-rw-r--r--   0        0        0     1732 2023-08-08 21:22:40.779421 license_manager_agent-3.0.0/lm_agent/parsing/flexlm.py
+-rw-r--r--   0        0        0     3537 2023-08-08 21:22:40.779421 license_manager_agent-3.0.0/lm_agent/parsing/lmx.py
+-rw-r--r--   0        0        0     4416 2023-08-08 21:22:40.779421 license_manager_agent-3.0.0/lm_agent/parsing/lsdyna.py
+-rw-r--r--   0        0        0     4758 2023-08-08 21:22:40.779421 license_manager_agent-3.0.0/lm_agent/parsing/olicense.py
+-rw-r--r--   0        0        0     2197 2023-08-08 21:22:40.779421 license_manager_agent-3.0.0/lm_agent/parsing/rlm.py
+-rwxr-xr-x   0        0        0     1054 2023-08-08 21:22:40.779421 license_manager_agent-3.0.0/lm_agent/reconcile.py
+-rw-r--r--   0        0        0     8097 2023-08-08 21:22:40.779421 license_manager_agent-3.0.0/lm_agent/reconciliation.py
+-rw-r--r--   0        0        0        0 2023-08-08 21:22:40.779421 license_manager_agent-3.0.0/lm_agent/server_interfaces/__init__.py
+-rw-r--r--   0        0        0     2844 2023-08-08 21:22:40.779421 license_manager_agent-3.0.0/lm_agent/server_interfaces/flexlm.py
+-rw-r--r--   0        0        0     1620 2023-08-08 21:22:40.779421 license_manager_agent-3.0.0/lm_agent/server_interfaces/license_server_interface.py
+-rw-r--r--   0        0        0     2745 2023-08-08 21:22:40.779421 license_manager_agent-3.0.0/lm_agent/server_interfaces/lmx.py
+-rw-r--r--   0        0        0     2711 2023-08-08 21:22:40.779421 license_manager_agent-3.0.0/lm_agent/server_interfaces/lsdyna.py
+-rw-r--r--   0        0        0     2703 2023-08-08 21:22:40.779421 license_manager_agent-3.0.0/lm_agent/server_interfaces/olicense.py
+-rw-r--r--   0        0        0     3091 2023-08-08 21:22:40.779421 license_manager_agent-3.0.0/lm_agent/server_interfaces/rlm.py
+-rw-r--r--   0        0        0     1251 2023-08-08 21:22:40.779421 license_manager_agent-3.0.0/lm_agent/utils.py
+-rw-r--r--   0        0        0        0 2023-08-08 21:22:40.779421 license_manager_agent-3.0.0/lm_agent/workload_managers/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 21:22:40.779421 license_manager_agent-3.0.0/lm_agent/workload_managers/slurm/__init__.py
+-rw-r--r--   0        0        0     8204 2023-08-08 21:22:40.779421 license_manager_agent-3.0.0/lm_agent/workload_managers/slurm/cmd_utils.py
+-rw-r--r--   0        0        0     1036 2023-08-08 21:22:40.779421 license_manager_agent-3.0.0/lm_agent/workload_managers/slurm/common.py
+-rw-r--r--   0        0        0     3732 2023-08-08 21:22:40.779421 license_manager_agent-3.0.0/lm_agent/workload_managers/slurm/reservations.py
+-rw-r--r--   0        0        0     1524 2023-08-08 21:22:40.779421 license_manager_agent-3.0.0/lm_agent/workload_managers/slurm/slurmctld_epilog.py
+-rw-r--r--   0        0        0     3921 2023-08-08 21:22:40.779421 license_manager_agent-3.0.0/lm_agent/workload_managers/slurm/slurmctld_prolog.py
+-rw-r--r--   0        0        0     2050 2023-08-08 21:22:40.779421 license_manager_agent-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1053 1970-01-01 00:00:00.000000 license_manager_agent-3.0.0/PKG-INFO
```

### Comparing `license_manager_agent-2.3.2/lm_agent/backend_utils.py` & `license_manager_agent-3.0.0/lm_agent/backend_utils/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,19 +2,29 @@
 Provide utilities that communicate with the backend.
 """
 import getpass
 from typing import Dict, List, Optional, Union
 
 import httpx
 import jwt
-from pydantic import BaseModel, Field, ValidationError
 
-from lm_agent.config import PRODUCT_FEATURE_RX, settings
-from lm_agent.exceptions import LicenseManagerAuthTokenError, LicenseManagerBackendConnectionError
-from lm_agent.logs import logger
+from lm_agent.backend_utils.models import (
+    BookingSchema,
+    ConfigurationSchema,
+    FeatureSchema,
+    JobSchema,
+    LicenseBookingRequest,
+)
+from lm_agent.config import settings
+from lm_agent.exceptions import (
+    LicenseManagerAuthTokenError,
+    LicenseManagerBackendConnectionError,
+    LicenseManagerParseError,
+)
+from lm_agent.logs import log_error, logger
 
 USER_NAME = getpass.getuser()
 TOKEN_FILE_NAME = f"{USER_NAME}.token"
 
 
 def _load_token_from_cache() -> Union[str, None]:
     """
@@ -110,229 +120,188 @@
     def _inject_token(self, request: httpx.Request) -> httpx.Request:
         if self._token is None:
             self._token = acquire_token()
         request.headers["authorization"] = f"Bearer {self._token}"
         return request
 
 
-class SyncBackendClient(httpx.Client):
+async def check_backend_health():
     """
-    Extends the synchronous httpx.Client class with automatic token acquisition for requests.
-    The token is acquired lazily on the first httpx request issued.
-
-    This client should be used only for the CLI tools.
+    Hit the API's health-check endpoint to make sure the API is available.
     """
-
-    _token: Optional[str]
-
-    def __init__(self):
-        self._token = None
-        super().__init__(base_url=settings.BACKEND_BASE_URL, auth=self._inject_token)
-
-    def _inject_token(self, request: httpx.Request) -> httpx.Request:
-        if self._token is None:
-            self._token = acquire_token()
-        request.headers["authorization"] = f"Bearer {self._token}"
-        return request
-
-
-async def check_backend_health():
-    """Hit the API's health-check endpoint to make sure the API is available."""
     async with AsyncBackendClient() as backend_client:
         resp = await backend_client.get("/lm/health")
     if resp.status_code != 204:
-        logger.error("license-manager-backend health-check failed.")
+        logger.error(f"Backend health-check request failed with status code: {resp.status_code}")
         raise LicenseManagerBackendConnectionError("Could not connect to the backend health-check endpoint")
 
 
-class BackendConfigurationRow(BaseModel):
+async def get_cluster_jobs_from_backend() -> List[JobSchema]:
     """
-    NOTE: This is a copy of the schema from the backend.
-          If the schema changes upstream in a non-reverse-compatible way, this schema should cause errors
-          in deserialization.
+    Get all jobs for the cluster with its bookings from the backend.
     """
+    async with AsyncBackendClient() as backend_client:
+        resp = await backend_client.get("/lm/jobs/by_client_id")
+
+        LicenseManagerBackendConnectionError.require_condition(
+            resp.status_code == 200, f"Could not get job data from the backend: {resp.text}"
+        )
+
+    parsed_resp: List = resp.json()
 
-    class Config:
-        extra = "ignore"
+    with LicenseManagerParseError.handle_errors(
+        "Could not parse job data returned from the backend", do_except=log_error
+    ):
+        jobs = [JobSchema.parse_obj(job) for job in parsed_resp]
 
-    id: Optional[int] = None
-    product: str
-    features: dict
-    license_servers: List[str]
-    license_server_type: str
-    grace_time: int
-    client_id: str
+    return jobs
 
 
-class BackendBookingRow(BaseModel):
+async def get_cluster_configs_from_backend() -> List[ConfigurationSchema]:
     """
-    NOTE: This is a copy of the schema from the backend.
-          If the schema changes upstream in a non-reverse-compatible
-          way, this schema should cause errors in deserialization.
+    Get all configs from the backend for the cluster.
     """
+    async with AsyncBackendClient() as backend_client:
+        resp = await backend_client.get("/lm/configurations/by_client_id")
 
-    class Config:
-        extra = "ignore"
+        LicenseManagerBackendConnectionError.require_condition(
+            resp.status_code == 200, f"Could not get configuration data from the backend: {resp.text}"
+        )
 
-    job_id: str
-    product_feature: str
-    booked: int
-    config_id: int
-    lead_host: str
-    user_name: str
-    cluster_name: str
+    parsed_resp: List = resp.json()
 
+    with LicenseManagerParseError.handle_errors(
+        "Could not parse configuration data returned from the backend", do_except=log_error
+    ):
+        configurations = [ConfigurationSchema.parse_obj(configuration) for configuration in parsed_resp]
 
-class LicenseBooking(BaseModel):
-    """
-    Structure to represent a license booking.
-    """
+    return configurations
 
-    product_feature: str = Field(..., regex=PRODUCT_FEATURE_RX)
-    tokens: int
-    license_server_type: Union[None, str]
 
-
-class LicenseBookingRequest(BaseModel):
+async def get_cluster_grace_times() -> Dict[int, int]:
     """
-    Structure to represent a list of license bookings.
+    Get the grace time for each feature_id in the cluster.
     """
+    cluster_configurations = await get_cluster_configs_from_backend()
 
-    job_id: int
-    bookings: Union[List, List[LicenseBooking]]
-    user_name: str
-    lead_host: str
-    cluster_name: str
-
+    grace_times = {
+        feature.id: configuration.grace_time
+        for configuration in cluster_configurations
+        for feature in configuration.features
+    }
 
-async def get_bookings_from_backend(
-    cluster_name: Optional[str] = None,
-) -> List[BackendBookingRow]:
-    bookings: List = []
-    try:
-        async with AsyncBackendClient() as backend_client:
-            if cluster_name:
-                resp = await backend_client.get(f"/lm/api/v1/booking/all?cluster_name={cluster_name}")
-            else:
-                resp = await backend_client.get("/lm/api/v1/booking/all")
-    except httpx.ConnectError as e:
-        logger.error(f"Connection failed to backend: {e}")
-        return bookings
-    for booking in resp.json():
-        try:
-            bookings.append(BackendBookingRow.parse_obj(booking))
-        except ValidationError as err:
-            logger.error(f"Wrong format for booking: {str(err)}")
-    return bookings
+    return grace_times
 
 
-async def get_config_id_from_backend(product_feature: str) -> int:
-    """Given the product_feature return return the config id."""
-    path = "/lm/api/v1/config/"
+async def make_feature_update(feature: str, total: int, used: int):
+    """
+    Update the feature with its current counters.
+    """
     async with AsyncBackendClient() as backend_client:
-        resp = await backend_client.get(path, params={"product_feature": product_feature})
-    return resp.json()
+        feature_response = await backend_client.put(
+            "/lm/features/by_client_id",
+            json={
+                "name": feature,
+                "total": total,
+                "used": used,
+            },
+        )
+        LicenseManagerBackendConnectionError.require_condition(
+            feature_response.status_code == 200, f"Failed to update feature: {feature_response.text}"
+        )
 
 
-async def get_config_from_backend() -> List[BackendConfigurationRow]:
-    """Get all config rows from the backend."""
-    path = "/lm/api/v1/config/agent/all"
+async def make_booking_request(lbr: LicenseBookingRequest) -> bool:
+    """
+    Create a job and its bookings on the backend for each license booked.
+    """
+    async with AsyncBackendClient() as backend_client:
+        job_response = await backend_client.post(
+            "/lm/jobs",
+            json=lbr.dict(),
+        )
+        if job_response.status_code != 201:
+            logger.error(f"Failed to create booking: {job_response.text}")
+            return False
 
-    try:
-        async with AsyncBackendClient() as backend_client:
-            resp = await backend_client.get(path)
-    except httpx.ConnectError as e:
-        logger.error(f"Connection failed to backend: {backend_client.base_url}{path}: {e}")
-        return []
-
-    configs = []
-    for (i, config_row) in enumerate(resp.json()):
-        try:
-            configs.append(BackendConfigurationRow.parse_obj(config_row))
-        except ValidationError as err:
-            logger.error(f"Could not validate config entry at row {i}: {str(err)}")
-    return configs
+    logger.debug("##### Booking completed successfully #####")
+    return True
 
 
-async def make_booking_request(lbr: LicenseBookingRequest) -> bool:
-    """Book the feature tokens."""
+async def remove_job_by_slurm_job_id(slurm_job_id: str):
+    """
+    Remove the job with its bookings for the given slurm_job_id in the cluster.
+    """
+    async with AsyncBackendClient() as backend_client:
+        resp = await backend_client.delete(f"lm/jobs/slurm_job_id/{slurm_job_id}")
 
-    features = [
-        {
-            "product_feature": license_booking.product_feature,
-            "booked": license_booking.tokens,
-        }
-        for license_booking in lbr.bookings
-    ]
+        LicenseManagerBackendConnectionError.require_condition(
+            resp.status_code == 200, f"Failed to remove job: {resp.text}"
+        )
+
+    logger.debug("##### Job removed successfully #####")
 
-    logger.debug(f"features: {features}")
-    logger.debug(f"lbr: {lbr}")
 
+async def get_bookings_for_job_id(slurm_job_id: str) -> List[BookingSchema]:
+    """
+    Return the job with its bookings for the given job_id in the cluster.
+    """
     async with AsyncBackendClient() as backend_client:
-        resp = await backend_client.put(
-            "/lm/api/v1/booking/book",
-            json={
-                "job_id": lbr.job_id,
-                "features": features,
-                "user_name": lbr.user_name,
-                "lead_host": lbr.lead_host,
-                "cluster_name": lbr.cluster_name,
-            },
-        )
+        job_response = await backend_client.get(f"/lm/jobs/slurm_job_id/{slurm_job_id}")
 
-    if resp.status_code == 200:
-        logger.debug("##### Booking completed successfully #####")
-        return True
-    logger.debug(f"##### Booking failed: {str(resp.content)} #####")
-    return False
+        LicenseManagerBackendConnectionError.require_condition(
+            job_response.status_code == 200, f"Failed to get job: {job_response.text}"
+        )
 
+        with LicenseManagerParseError.handle_errors(""):
+            parsed_resp: List = job_response.json()["bookings"]
 
-async def remove_booking_for_job_id(job_id: str) -> bool:
-    """Remove token bookings used by job."""
+    with LicenseManagerParseError.handle_errors(
+        "Could not parse booking data returned from the backend", do_except=log_error
+    ):
+        bookings = [BookingSchema.parse_obj(booking) for booking in parsed_resp]
 
-    # Remove the booking for the job.
-    async with AsyncBackendClient() as backend_client:
-        resp = await backend_client.delete(f"lm/api/v1/booking/book/{job_id}")
-    # Return True if the request to delete the booking was successful.
-    if resp.status_code == 200:
-        return True
-    logger.error(f"{job_id} could not be deleted.")
-    logger.debug(f"response from delete: {resp.__dict__}")
-    return False
+    return bookings
 
 
-async def get_all_grace_times() -> Dict[int, int]:
+async def get_all_features_from_backend() -> List[FeatureSchema]:
     """
-    Send GET to /lm/api/v1/config/all.
+    Return the job with its bookings for the given job_id in the cluster.
     """
     async with AsyncBackendClient() as backend_client:
-        response = await backend_client.get("/lm/api/v1/config/all")
-    configs = response.json()
-    grace_times = {config["id"]: config["grace_time"] for config in configs}
-    return grace_times
+        feature_response = await backend_client.get("/lm/features")
 
+        LicenseManagerBackendConnectionError.require_condition(
+            feature_response.status_code == 200, f"Failed to get features: {feature_response.text}"
+        )
 
-async def get_booking_for_job_id(job_id: str) -> Dict:
-    """
-    Return the booking row for the given job_id.
-    """
-    async with AsyncBackendClient() as backend_client:
-        response = await backend_client.get(f"/lm/api/v1/booking/job/{job_id}")
-    return response.json()
+        with LicenseManagerParseError.handle_errors(""):
+            parsed_resp: List = feature_response.json()
 
+    with LicenseManagerParseError.handle_errors(
+        "Could not parse feature data returned from the backend", do_except=log_error
+    ):
+        features = [FeatureSchema.parse_obj(feature) for feature in parsed_resp]
 
-async def get_bookings_sum_per_cluster(product_feature: str) -> Dict[str, int]:
-    """
-    Get booking sum for a license's bookings in each cluster.
+    return features
+
+
+async def get_feature_bookings_sum(product_feature: str) -> int:
     """
-    async with AsyncBackendClient() as backend_client:
-        response = await backend_client.get("/lm/api/v1/booking/all")
-    bookings = response.json()
+    Get booking sum for a license's bookings in all clusters.
 
-    booking_sum: Dict[str, int] = {}
+    Note: a license can be configured in multiple clusters,
+    having the same name but different configurations.
+
+    The booking sum is the sum of all bookings for a license in all clusters.
+    """
+    # get all features
+    features = await get_all_features_from_backend()
 
-    for booking in bookings:
-        cluster_name = booking["cluster_name"]
-        if booking["product_feature"] == product_feature:
-            booking_sum[cluster_name] = booking_sum.get(cluster_name, 0) + booking["booked"]
+    # sum bookings for each feature with the same name
+    booking_sum = sum(
+        feature.booked_total
+        for feature in features
+        if f"{feature.product.name}.{feature.name}" == product_feature
+    )
 
     return booking_sum
```

### Comparing `license_manager_agent-2.3.2/lm_agent/config.py` & `license_manager_agent-3.0.0/lm_agent/config.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.2/lm_agent/exceptions.py` & `license_manager_agent-3.0.0/lm_agent/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,18 @@
     """Exception for backend connection issues."""
 
 
 class LicenseManagerBackendConnectionError(Buzz):
     """Exception for backend connection issues."""
 
 
+class LicenseManagerParseError(Buzz):
+    """Exception for error during parsing of backend data."""
+
+
 class LicenseManagerBackendVersionError(Buzz):
     """Exception for backend/agent version mismatches."""
 
 
 class LicenseManagerEmptyReportError(Buzz):
     """Exception for empty report when no licenses added in backend."""
```

### Comparing `license_manager_agent-2.3.2/lm_agent/license_report.py` & `license_manager_agent-3.0.0/lm_agent/license_report.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 """
 Invoke license stat tools to build a view of license token counts.
 """
 import asyncio
 import typing
 
-from lm_agent.backend_utils import BackendConfigurationRow, get_config_from_backend
+from lm_agent.backend_utils.models import ConfigurationSchema
+from lm_agent.backend_utils.utils import get_cluster_configs_from_backend
 from lm_agent.exceptions import LicenseManagerNonSupportedServerTypeError
 from lm_agent.logs import logger
 from lm_agent.server_interfaces.flexlm import FlexLMLicenseServer
-from lm_agent.server_interfaces.license_server_interface import LicenseServerInterface
+from lm_agent.server_interfaces.license_server_interface import LicenseReportItem, LicenseServerInterface
 from lm_agent.server_interfaces.lmx import LMXLicenseServer
 from lm_agent.server_interfaces.lsdyna import LSDynaLicenseServer
 from lm_agent.server_interfaces.olicense import OLicenseLicenseServer
 from lm_agent.server_interfaces.rlm import RLMLicenseServer
 from lm_agent.workload_managers.slurm.cmd_utils import get_all_product_features_from_cluster
 
 
 def get_local_license_configurations(
-    license_configurations: typing.List[BackendConfigurationRow], local_licenses: typing.List[str]
-) -> typing.List[BackendConfigurationRow]:
+    license_configurations: typing.List[ConfigurationSchema], local_licenses: typing.List[str]
+) -> typing.List[ConfigurationSchema]:
     """
     Return the license configurations from the backend that are configured on the cluster.
     """
     filtered_entries = []
 
     for entry in license_configurations:
-        for feature in entry.features.keys():
-            if f"{entry.product}.{feature}" in local_licenses:
+        for feature in entry.features:
+            feature_name = feature.name
+            product_name = feature.product.name
+            if f"{product_name}.{feature_name}" in local_licenses:
                 filtered_entries.append(entry)
                 break
     return filtered_entries
 
 
-async def report() -> typing.List[dict]:
+async def report() -> typing.List[LicenseReportItem]:
     """
     Get stat counts using a license stat tool.
 
     This function iterates over the available license_servers and associated
     features configured via LICENSE_SERVER_FEATURES and generates
     a report by requesting license information from the license_server_type.
 
@@ -44,15 +47,17 @@
     view of what features are available with what actually exists in the
     license server database.
     """
     report_items = []
     get_report_awaitables = []
     product_features_awaited = []
 
-    license_configurations = await get_config_from_backend()
+    # Get cluster configuration
+    license_configurations = await get_cluster_configs_from_backend()
+
     local_licenses = await get_all_product_features_from_cluster()
     filtered_entries = get_local_license_configurations(license_configurations, local_licenses)
 
     logger.debug("#### Getting reconciliation report ####")
     logger.debug("### Licenses in the backend: ")
     logger.debug(license_configurations)
     logger.debug("### Licenses in the cluster: ")
@@ -66,22 +71,22 @@
         lsdyna=LSDynaLicenseServer,
         lmx=LMXLicenseServer,
         olicense=OLicenseLicenseServer,
     )
 
     for entry in filtered_entries:
         product_features_to_check = []
-        for feature in entry.features.keys():
-            product_feature = f"{entry.product}.{feature}"
+        for feature in entry.features:
+            product_feature = f"{feature.product.name}.{feature.name}"
             product_features_to_check.append(product_feature)
 
         logger.debug("### Features to check: ")
         logger.debug(product_features_to_check)
 
-        server_type = server_type_map.get(entry.license_server_type)
+        server_type = server_type_map.get(entry.type)
 
         if server_type is None:
             raise LicenseManagerNonSupportedServerTypeError("License server type not supported.")
 
         license_server_interface = server_type(entry.license_servers)
 
         for product_feature in product_features_to_check:
@@ -92,12 +97,11 @@
 
     for result, product_feature in zip(results, product_features_awaited):
         if isinstance(result, Exception):
             logger.error(f"#### Report for feature {product_feature} failed with: {result} ####")
         else:
             report_items.append(result)
 
-    reconciliation = [item.dict() for item in report_items]
     logger.debug("#### Reconciliation items:")
-    logger.debug(reconciliation)
+    logger.debug(report_items)
 
-    return reconciliation
+    return report_items
```

### Comparing `license_manager_agent-2.3.2/lm_agent/parsing/flexlm.py` & `license_manager_agent-3.0.0/lm_agent/parsing/flexlm.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.2/lm_agent/parsing/lmx.py` & `license_manager_agent-3.0.0/lm_agent/parsing/lmx.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.2/lm_agent/parsing/lsdyna.py` & `license_manager_agent-3.0.0/lm_agent/parsing/lsdyna.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.2/lm_agent/parsing/olicense.py` & `license_manager_agent-3.0.0/lm_agent/parsing/olicense.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.2/lm_agent/parsing/rlm.py` & `license_manager_agent-3.0.0/lm_agent/parsing/rlm.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.2/lm_agent/reconcile.py` & `license_manager_agent-3.0.0/lm_agent/reconcile.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 import asyncio
 import logging
 import typing
 
 import sentry_sdk
 
-from lm_agent.backend_utils import check_backend_health
+from lm_agent.backend_utils.utils import check_backend_health
 from lm_agent.config import settings
 from lm_agent.logs import init_logging, logger
 from lm_agent.reconciliation import reconcile
 
 if settings.SENTRY_DSN:
     sentry_sdk.init(
         dsn=settings.SENTRY_DSN,
```

### Comparing `license_manager_agent-2.3.2/lm_agent/reconciliation.py` & `license_manager_agent-3.0.0/lm_agent/reconciliation.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,132 +1,116 @@
 #!/usr/bin/env python3
 """
 Reconciliation functionality live here.
 """
 import asyncio
 from typing import Dict, List
 
-from httpx import ConnectError
-
-from lm_agent.backend_utils import (
-    AsyncBackendClient,
-    get_all_grace_times,
-    get_booking_for_job_id,
-    get_bookings_from_backend,
-    get_bookings_sum_per_cluster,
-    get_config_id_from_backend,
-    remove_booking_for_job_id,
-)
-from lm_agent.exceptions import (
-    LicenseManagerBackendConnectionError,
-    LicenseManagerEmptyReportError,
-    LicenseManagerFeatureConfigurationIncorrect,
-    LicenseManagerReservationFailure,
+from lm_agent.backend_utils.models import BookingSchema
+from lm_agent.backend_utils.utils import (
+    get_bookings_for_job_id,
+    get_cluster_configs_from_backend,
+    get_cluster_grace_times,
+    get_cluster_jobs_from_backend,
+    get_feature_bookings_sum,
+    make_feature_update,
+    remove_job_by_slurm_job_id,
 )
+from lm_agent.exceptions import LicenseManagerEmptyReportError, LicenseManagerReservationFailure
 from lm_agent.license_report import report
 from lm_agent.logs import logger
+from lm_agent.server_interfaces.license_server_interface import LicenseReportItem
 from lm_agent.workload_managers.slurm.cmd_utils import (
-    get_all_product_features_from_cluster,
-    get_cluster_name,
     get_tokens_for_license,
     return_formatted_squeue_out,
     squeue_parser,
 )
 from lm_agent.workload_managers.slurm.reservations import (
     scontrol_create_reservation,
     scontrol_delete_reservation,
     scontrol_show_reservation,
     scontrol_update_reservation,
 )
 
-RECONCILE_URL_PATH = "/lm/api/v1/license/reconcile"
-
 
-def get_greatest_grace_time(job_id: str, grace_times: Dict[int, int], booking_rows: List) -> int:
+def get_greatest_grace_time_for_job(grace_times: Dict[int, int], job_bookings: List[BookingSchema]) -> int:
     """
-    Find the greatest grace_time for the given job_id.
+    Find the greatest grace_time among the features booked by the given job_id.
     """
-    greatest_grace_time = -1
-    for book in booking_rows:
-        if not book:
-            continue
-        for inner_book in book:
-            if str(inner_book["job_id"]) != str(job_id):
-                continue
-            config_id_for_grace_times = inner_book["config_id"]
-            greatest_grace_time = max(greatest_grace_time, grace_times[config_id_for_grace_times])
-    return greatest_grace_time
+    greatest_booking_feature = max(
+        job_bookings, default=None, key=lambda job_booking: grace_times[job_booking.feature_id]
+    )
+    if not greatest_booking_feature:
+        return -1
+    return grace_times[greatest_booking_feature.feature_id]
 
 
 def get_running_jobs(squeue_result: List) -> List:
     return [j for j in squeue_result if j["state"] == "RUNNING"]
 
 
-async def clean_booked_grace_time():
+async def clean_jobs_by_grace_time():
     """
-    Clean the booked licenses if the job's running time is greater than the grace_time.
+    Clean the jobs where running time is greater than the grace_time.
     """
     logger.debug("GRACE_TIME START")
+
     formatted_squeue_output = return_formatted_squeue_out()
-    cluster_name = await get_cluster_name()
     if not formatted_squeue_output:
         logger.debug("GRACE_TIME no squeue")
-        await clean_bookings(None, cluster_name)
+        await clean_jobs(None)
         logger.debug("GRACE_TIME cleaned bookings that are not in the queue")
         return
+
     squeue_result = squeue_parser(formatted_squeue_output)
     squeue_running_jobs = get_running_jobs(squeue_result)
 
-    grace_times = await get_all_grace_times()
-    get_booked_call = []
-    for job in squeue_running_jobs:
-        job_id = job["job_id"]
-        get_booked_call.append(get_booking_for_job_id(job_id))
+    get_bookings_call = [get_bookings_for_job_id(job["job_id"]) for job in squeue_running_jobs]
+    results = await asyncio.gather(*get_bookings_call)
+    bookings_for_running_jobs = {job["job_id"]: result for job, result in zip(squeue_running_jobs, results)}
 
-    booking_rows_for_running_jobs = await asyncio.gather(*get_booked_call)
+    grace_times = await get_cluster_grace_times()
 
-    # get the greatest grace_time for each job
+    # get the grace_time for each job
     for job in squeue_running_jobs:
-        job_id = job["job_id"]
-        greatest_grace_time = get_greatest_grace_time(job_id, grace_times, booking_rows_for_running_jobs)
+        slurm_job_id = job["job_id"]
+        greatest_grace_time = get_greatest_grace_time_for_job(
+            grace_times, bookings_for_running_jobs[slurm_job_id]
+        )
         # if the running_time is greater than the greatest grace_time, delete the booking for it
         if job["run_time_in_seconds"] > greatest_grace_time and greatest_grace_time != -1:
-            logger.debug(f"GRACE_TIME: {greatest_grace_time}, {job_id}")
-            await remove_booking_for_job_id(job_id)
-    await clean_bookings(squeue_result, cluster_name)
+            logger.debug(f"GRACE_TIME: {greatest_grace_time}, {slurm_job_id}")
+            await remove_job_by_slurm_job_id(slurm_job_id)
+
+    await clean_jobs(squeue_result)
+
 
+async def clean_jobs(squeue_result):
+    """Clean the jobs that aren't running along with its bookings."""
+    logger.debug("CLEAN_JOBS: start")
 
-async def clean_bookings(squeue_result, cluster_name):
-    logger.debug("CLEAN_BOOKINGS: start")
-    cluster_bookings = [str(booking.job_id) for booking in await get_bookings_from_backend(cluster_name)]
+    cluster_jobs = [job.slurm_job_id for job in await get_cluster_jobs_from_backend()]
     if squeue_result is None:
         squeue_result = []
+
     jobs_not_running = [str(job["job_id"]) for job in squeue_result if job["state"] != "RUNNING"]
     all_jobs_squeue = [str(job["job_id"]) for job in squeue_result]
-    delete_booking_call = []
-    logger.debug("CLEAN_BOOKINGS: after building lists")
-    for job_id in cluster_bookings:
-        if job_id in jobs_not_running or job_id not in all_jobs_squeue:
-            delete_booking_call.append(remove_booking_for_job_id(job_id))
-    logger.debug(f"CLEAN_BOOKINGS: {cluster_bookings}, {jobs_not_running}, {all_jobs_squeue}")
-    if not delete_booking_call:
-        logger.debug("CLEAN_BOOKINGS: no need to clean")
-        return
-    await asyncio.gather(*delete_booking_call)
+    logger.debug("CLEAN_JOBS: after building lists")
+
+    delete_job_call = []
 
+    for slurm_job_id in cluster_jobs:
+        if slurm_job_id in jobs_not_running or slurm_job_id not in all_jobs_squeue:
+            delete_job_call.append(remove_job_by_slurm_job_id(slurm_job_id))
 
-async def filter_cluster_update_licenses(licenses_to_update: List) -> List:
-    """Get the licenses in the cluster to filter the cluster update response."""
-    local_licenses = await get_all_product_features_from_cluster()
-
-    filtered_licenses = []
-    for license in licenses_to_update:
-        if license["product_feature"] in local_licenses:
-            filtered_licenses.append(license)
-    return filtered_licenses
+    if not delete_job_call:
+        logger.debug("CLEAN_JOBS: no need to clean")
+        return
+
+    await asyncio.gather(*delete_job_call)
 
 
 async def create_or_update_reservation(reservation_data):
     """
     Create the reservation if it doesn't exist, otherwise update it.
     If the reservation cannot be updated, delete it and create a new one.
     """
@@ -143,123 +127,89 @@
         created = await scontrol_create_reservation(reservation_data, "30:00")
         LicenseManagerReservationFailure.require_condition(created, "Could not create reservation.")
 
 
 async def reconcile():
     """Generate the report and reconcile the license feature token usage."""
     logger.debug("Starting reconciliation")
+
+    # Get cluster data
+    configurations = await get_cluster_configs_from_backend()
+
     # Delete bookings for jobs that reached the grace time
-    logger.debug("Cleaning bookings by grace time")
-    await clean_booked_grace_time()
-    logger.debug("Bookings cleaned by grace time")
+    logger.debug("Cleaning jobs by grace time")
+    await clean_jobs_by_grace_time()
+    logger.debug("Jobs cleaned by grace time")
 
     # Generate report and update the backend
     logger.debug("Reconciling licenses in the backend")
-    await update_report()
+    license_usage_info = await update_features()
     logger.debug("Backend licenses reconciliated")
 
-    # Fetch from backend the licenses usage information
-    logger.debug("Fetching licenses usage information from backend")
-    async with AsyncBackendClient() as backend_client:
-        response = await backend_client.get("/lm/api/v1/license/cluster_update")
-    licenses_usage_info = response.json()
-    logger.debug("Licenses usage information fetched from backend")
-
-    # Filter the licenses to update
-    licenses_to_update = await filter_cluster_update_licenses(licenses_usage_info)
-    logger.debug(f"Licenses to update: {licenses_to_update}")
-
     reservation_data = []
 
     # Calculate how many licenses should be reserved for each license
-    for license_data in licenses_to_update:
-        # Get license usage from backend
-        product_feature = license_data["product_feature"]
-        product, feature = product_feature.split(".")
-        server_used = license_data["license_used"]
-
-        cluster_name = await get_cluster_name()
-
-        bookings_per_cluster = await get_bookings_sum_per_cluster(product_feature)
-        cluster_booking_sum = bookings_per_cluster.get(cluster_name, 0)
-        other_cluster_booking_sum = sum(
-            [booking for cluster, booking in bookings_per_cluster.items() if cluster != cluster_name]
-        )
-
-        # Get license configuration from backend
-        config_id = await get_config_id_from_backend(product_feature)
-        async with AsyncBackendClient() as backend_client:
-            config = await backend_client.get(f"/lm/api/v1/config/{config_id}")
-        config = config.json()
-
-        license_server_type = config["license_server_type"]
-        # Use feature name to get total and limit from feature data in the license config
-        try:
-            # Get total from new feature format
-            total = config["features"][feature].get("total", 0)
-            LicenseManagerFeatureConfigurationIncorrect.require_condition(
-                total,
-                f"The configuration for {feature} is incorrect. Please include the total amount of licenses.",
-            )
-        except AttributeError:
-            # Fallback to get the total from the old feature format
-            total = config["features"][feature]
-
-        try:
-            # Get limit from new feature format. If not specified, use the total as the limit
-            limit = config["features"][feature].get("limit", total)
-        except AttributeError:
-            # Fallback to use the total as the limit for the old feature format
-            limit = total
+    for license_data in license_usage_info:
+        # Get license usage from license report
+        product_feature = license_data.product_feature
+        server_used = license_data.used
+        total = license_data.total
+
+        # Get booking information from backend
+        booking_sum = await get_feature_bookings_sum(product_feature)
+
+        # Get license server type and reserved from the configuration in the backend
+        for configuration in configurations:
+            for feature in configuration.features:
+                if f"{feature.product.name}.{feature.name}" == product_feature:
+                    license_server_type = configuration.type
+                    reserved = feature.reserved
 
         # Get license usage from the cluster
         slurm_used = await get_tokens_for_license(f"{product_feature}@{license_server_type}", "Used")
 
         """
         The reserved amount represents how many licenses are already in use:
         Either in the license server or booked for a job (bookings from other cluster as well).
-        If the license has a limit, the amount of licenses past the limit should be reserved too.
+        If the license has a reserved value, it should be reserved too.
 
         The reservation is not meant to be used by any user, it's a way to block usage of licenses
         """
 
-        reserved = (
-            server_used - (slurm_used - cluster_booking_sum) + other_cluster_booking_sum + (total - limit)
-        )
+        reservation_amount = server_used - slurm_used + booking_sum + reserved
 
-        if reserved < 0:
-            reserved = 0
+        if reservation_amount < 0:
+            reservation_amount = 0
 
-        if reserved > total:
-            reserved = total
+        if reservation_amount > total:
+            reservation_amount = total
 
-        if reserved:
-            reservation_data.append(f"{product_feature}@{license_server_type}:{reserved}")
+        if reservation_amount:
+            reservation_data.append(f"{product_feature}@{license_server_type}:{reservation_amount}")
 
-    # Create the reservation or update the existing one
-    logger.debug(f"Reservation data: {reservation_data}")
-    await create_or_update_reservation(",".join(reservation_data))
+        if reservation_data:
+            logger.debug(f"Reservation data: {reservation_data}")
 
-    logger.debug("Reconciliation done")
+            # Create the reservation or update the existing one
+            await create_or_update_reservation(",".join(reservation_data))
+        else:
+            logger.debug("No reservation needed")
 
+        logger.debug("Reconciliation done")
 
-async def update_report():
-    logger.info("Beginning forced reconciliation process")
-    rep = await report()
-    if not rep:
+
+async def update_features() -> List[LicenseReportItem]:
+    """Send the license data collected from the cluster to the backend."""
+    license_report = await report()
+
+    if not license_report:
         logger.error(
             "No license data could be collected, check that tools are installed "
             "correctly and the right hosts/ports are configured in settings"
         )
         raise LicenseManagerEmptyReportError("Got an empty response from the license server")
-    try:
-        async with AsyncBackendClient() as backend_client:
-            r = await backend_client.patch(RECONCILE_URL_PATH, json=rep)
-    except ConnectError as e:
-        logger.error(f"{backend_client.base_url}{RECONCILE_URL_PATH}: {e}")
-        raise LicenseManagerBackendConnectionError("Failed to connect to the backend")
-
-    if r.status_code != 200:
-        logger.error(f"{r.url}: {r.status_code}!: {r.text}")
-        raise LicenseManagerBackendConnectionError(f"Unexpected status code from report: {r.status_code}")
 
-    logger.info(f"Forced reconciliation succeeded. backend updated: {len(rep)} feature(s)")
+    for license in license_report:
+        product, feature = license.product_feature.split(".")
+        await make_feature_update(feature=feature, total=license.total, used=license.used)
+
+    return license_report
```

### Comparing `license_manager_agent-2.3.2/lm_agent/server_interfaces/flexlm.py` & `license_manager_agent-3.0.0/lm_agent/server_interfaces/flexlm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """FlexLM license server interface."""
 import typing
 
+from lm_agent.backend_utils.models import LicenseServerSchema
 from lm_agent.config import settings
 from lm_agent.exceptions import LicenseManagerBadServerOutput
 from lm_agent.parsing import flexlm
 from lm_agent.server_interfaces.license_server_interface import LicenseReportItem, LicenseServerInterface
 from lm_agent.utils import run_command
 
 
 class FlexLMLicenseServer(LicenseServerInterface):
     """Extract license information from FlexLM license server."""
 
-    def __init__(self, license_servers: typing.List[str]):
+    def __init__(self, license_servers: typing.List[LicenseServerSchema]):
         self.license_servers = license_servers
         self.parser = flexlm.parse
 
     def get_commands_list(self) -> typing.List[typing.List[str]]:
         """Generate a list of commands with the available license server hosts."""
 
-        host_ports = [(server.split(":")[1:]) for server in self.license_servers]
         commands_to_run = []
-        for host, port in host_ports:
+        for license_server in self.license_servers:
             command_line = [
                 f"{settings.LMUTIL_PATH}",
                 "lmstat",
                 "-c",
-                f"{port}@{host}",
+                f"{license_server.port}@{license_server.host}",
                 "-f",
             ]
             commands_to_run.append(command_line)
         return commands_to_run
 
     async def get_output_from_server(self, product_feature: str):
         """Override abstract method to get output from FlexLM license server."""
@@ -57,20 +57,18 @@
         parsed_output = self.parser(server_output)
 
         # raise exception if parser didn't output license information
         if parsed_output.get("total") is None or any(
             [
                 parsed_output.get("total", {}).get("used") is None,
                 parsed_output.get("total", {}).get("total") is None,
-                parsed_output.get("uses") is None,
             ]
         ):
             raise LicenseManagerBadServerOutput("Invalid data returned from parser.")
 
         report_item = LicenseReportItem(
             product_feature=product_feature,
             used=parsed_output["total"]["used"],
             total=parsed_output["total"]["total"],
-            used_licenses=parsed_output["uses"],
         )
 
         return report_item
```

### Comparing `license_manager_agent-2.3.2/lm_agent/server_interfaces/license_server_interface.py` & `license_manager_agent-3.0.0/lm_agent/server_interfaces/license_server_interface.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Module for license server interface abstract base class."""
 import abc
-import typing
 
 from pydantic import BaseModel, Field
 
 from lm_agent.config import PRODUCT_FEATURE_RX
 
 
 class LicenseServerInterface(metaclass=abc.ABCMeta):
@@ -47,8 +46,7 @@
     """
     An item in a LicenseReport, a count of tokens for one product/feature.
     """
 
     product_feature: str = Field(..., regex=PRODUCT_FEATURE_RX)
     used: int
     total: int
-    used_licenses: typing.List
```

### Comparing `license_manager_agent-2.3.2/lm_agent/server_interfaces/lmx.py` & `license_manager_agent-3.0.0/lm_agent/server_interfaces/lsdyna.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,61 +1,59 @@
-"""LM-X license server interface."""
+"""LS-Dyna license server interface."""
 import typing
 
+from lm_agent.backend_utils.models import LicenseServerSchema
 from lm_agent.config import settings
 from lm_agent.exceptions import LicenseManagerBadServerOutput
-from lm_agent.parsing import lmx
+from lm_agent.parsing import lsdyna
 from lm_agent.server_interfaces.license_server_interface import LicenseReportItem, LicenseServerInterface
 from lm_agent.utils import run_command
 
 
-class LMXLicenseServer(LicenseServerInterface):
-    """Extract license information from LM-X license server."""
+class LSDynaLicenseServer(LicenseServerInterface):
+    """Extract license information from LS-Dyna license server."""
 
-    def __init__(self, license_servers: typing.List[str]):
+    def __init__(self, license_servers: typing.List[LicenseServerSchema]):
         """Initialize the license server instance with the license server host and parser."""
         self.license_servers = license_servers
-        self.parser = lmx.parse
+        self.parser = lsdyna.parse
 
     def get_commands_list(self) -> typing.List[typing.List[str]]:
         """Generate a list of commands with the available license server hosts."""
 
-        host_ports = [(server.split(":")[1:]) for server in self.license_servers]
         commands_to_run = []
-        for host, port in host_ports:
+        for license_server in self.license_servers:
             command_line = [
-                f"{settings.LMXENDUTIL_PATH}",
-                "-licstat",
-                "-host",
-                host,
-                "-port",
-                port,
+                f"{settings.LSDYNA_PATH}",
+                "-s",
+                f"{license_server.port}@{license_server.host}",
+                "-R",
             ]
             commands_to_run.append(command_line)
         return commands_to_run
 
     async def get_output_from_server(self):
-        """Override abstract method to get output from LM-X license server."""
+        """Override abstract method to get output from Ls-Dyna license server."""
 
         # get the list of commands for each license server host
         commands_to_run = self.get_commands_list()
 
         # run each command in the list, one at a time, until one succeds
         for cmd in commands_to_run:
             output = await run_command(cmd)
 
             # try the next server if the previous didn't return the expected data
             if not output:
                 continue
             return output
 
-        raise RuntimeError("None of the checks for LM-X succeeded!")
+        raise RuntimeError("None of the checks for LS-Dyna succeeded!")
 
     async def get_report_item(self, product_feature: str):
-        """Override abstract method to parse LM-X license server output into License Report Item."""
+        """Override abstract method to parse LS-Dyna license server output into License Report Item."""
 
         server_output = await self.get_output_from_server()
         parsed_output = self.parser(server_output)
 
         (_, feature) = product_feature.split(".")
 
         current_feature_item = parsed_output.get(feature)
@@ -64,11 +62,10 @@
         if current_feature_item is None:
             raise LicenseManagerBadServerOutput("Invalid data returned from parser.")
 
         report_item = LicenseReportItem(
             product_feature=product_feature,
             used=current_feature_item["used"],
             total=current_feature_item["total"],
-            used_licenses=current_feature_item["uses"],
         )
 
         return report_item
```

### Comparing `license_manager_agent-2.3.2/lm_agent/server_interfaces/lsdyna.py` & `license_manager_agent-3.0.0/lm_agent/server_interfaces/rlm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,82 @@
-"""LS-Dyna license server interface."""
+"""RLM license server interface."""
 import typing
 
+from lm_agent.backend_utils.models import LicenseServerSchema
 from lm_agent.config import settings
 from lm_agent.exceptions import LicenseManagerBadServerOutput
-from lm_agent.parsing import lsdyna
+from lm_agent.parsing import rlm
 from lm_agent.server_interfaces.license_server_interface import LicenseReportItem, LicenseServerInterface
 from lm_agent.utils import run_command
 
 
-class LSDynaLicenseServer(LicenseServerInterface):
-    """Extract license information from LS-Dyna license server."""
+class RLMLicenseServer(LicenseServerInterface):
+    """Extract license information from RLM license server."""
 
-    def __init__(self, license_servers: typing.List[str]):
-        """Initialize the license server instance with the license server host and parser."""
+    def __init__(self, license_servers: typing.List[LicenseServerSchema]):
         self.license_servers = license_servers
-        self.parser = lsdyna.parse
+        self.parser = rlm.parse
 
     def get_commands_list(self) -> typing.List[typing.List[str]]:
         """Generate a list of commands with the available license server hosts."""
 
-        host_ports = [(server.split(":")[1:]) for server in self.license_servers]
         commands_to_run = []
-        for host, port in host_ports:
+        for license_server in self.license_servers:
             command_line = [
-                f"{settings.LSDYNA_PATH}",
-                "-s",
-                f"{port}@{host}",
-                "-R",
+                f"{settings.RLMUTIL_PATH}",
+                "rlmstat",
+                "-c",
+                f"{license_server.port}@{license_server.host}",
+                "-a",
+                "-p",
             ]
             commands_to_run.append(command_line)
         return commands_to_run
 
     async def get_output_from_server(self):
-        """Override abstract method to get output from Ls-Dyna license server."""
+        """Override abstract method to get output from RLM license server."""
 
         # get the list of commands for each license server host
         commands_to_run = self.get_commands_list()
 
         # run each command in the list, one at a time, until one succeds
         for cmd in commands_to_run:
             output = await run_command(cmd)
 
             # try the next server if the previous didn't return the expected data
             if not output:
                 continue
             return output
 
-        raise RuntimeError("None of the checks for LS-Dyna succeeded!")
+        raise RuntimeError("None of the checks for RLM succeeded!")
 
     async def get_report_item(self, product_feature: str):
-        """Override abstract method to parse LS-Dyna license server output into License Report Item."""
+        """Override abstract method to parse RLM license server output into License Report Item."""
 
         server_output = await self.get_output_from_server()
         parsed_output = self.parser(server_output)
 
         (_, feature) = product_feature.split(".")
 
-        current_feature_item = parsed_output.get(feature)
+        current_feature_item = self._filter_current_feature(parsed_output["total"], feature)
 
         # raise exception if parser didn't output license information
         if current_feature_item is None:
             raise LicenseManagerBadServerOutput("Invalid data returned from parser.")
 
         report_item = LicenseReportItem(
             product_feature=product_feature,
             used=current_feature_item["used"],
             total=current_feature_item["total"],
-            used_licenses=current_feature_item["uses"],
         )
 
         return report_item
+
+    def _filter_current_feature(self, parsed_list, feature):
+        """
+        The output from the RLM server returns information about all the licenses
+        in the server. This function filters the output to return only the information
+        about the feature we want.
+        """
+        for feature_item in parsed_list:
+            if feature_item["feature"] == feature:
+                return feature_item
```

### Comparing `license_manager_agent-2.3.2/lm_agent/server_interfaces/olicense.py` & `license_manager_agent-3.0.0/lm_agent/server_interfaces/lmx.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,61 @@
-"""OLicense license server interface."""
+"""LM-X license server interface."""
 import typing
 
+from lm_agent.backend_utils.models import LicenseServerSchema
 from lm_agent.config import settings
 from lm_agent.exceptions import LicenseManagerBadServerOutput
-from lm_agent.parsing import olicense
+from lm_agent.parsing import lmx
 from lm_agent.server_interfaces.license_server_interface import LicenseReportItem, LicenseServerInterface
 from lm_agent.utils import run_command
 
 
-class OLicenseLicenseServer(LicenseServerInterface):
-    """Extract license information from OLicense license server."""
+class LMXLicenseServer(LicenseServerInterface):
+    """Extract license information from LM-X license server."""
 
-    def __init__(self, license_servers: typing.List[str]):
+    def __init__(self, license_servers: typing.List[LicenseServerSchema]):
         """Initialize the license server instance with the license server host and parser."""
         self.license_servers = license_servers
-        self.parser = olicense.parse
+        self.parser = lmx.parse
 
     def get_commands_list(self) -> typing.List[typing.List[str]]:
         """Generate a list of commands with the available license server hosts."""
 
-        host_ports = [(server.split(":")[1:]) for server in self.license_servers]
         commands_to_run = []
-        for host, port in host_ports:
+        for license_server in self.license_servers:
             command_line = [
-                f"{settings.OLIXTOOL_PATH}",
-                "-sv",
-                f"{host}:{port}",
+                f"{settings.LMXENDUTIL_PATH}",
+                "-licstat",
+                "-host",
+                f"{license_server.host}",
+                "-port",
+                f"{license_server.port}",
             ]
             commands_to_run.append(command_line)
         return commands_to_run
 
     async def get_output_from_server(self):
-        """Override abstract method to get output from OLicense license server."""
+        """Override abstract method to get output from LM-X license server."""
 
         # get the list of commands for each license server host
         commands_to_run = self.get_commands_list()
 
         # run each command in the list, one at a time, until one succeds
         for cmd in commands_to_run:
             output = await run_command(cmd)
 
             # try the next server if the previous didn't return the expected data
             if not output:
                 continue
             return output
 
-        raise RuntimeError("None of the checks for OLicense succeeded!")
+        raise RuntimeError("None of the checks for LM-X succeeded!")
 
     async def get_report_item(self, product_feature: str):
-        """Override abstract method to parse OLicense license server output into License Report Item."""
+        """Override abstract method to parse LM-X license server output into License Report Item."""
 
         server_output = await self.get_output_from_server()
         parsed_output = self.parser(server_output)
 
         (_, feature) = product_feature.split(".")
 
         current_feature_item = parsed_output.get(feature)
@@ -61,11 +64,10 @@
         if current_feature_item is None:
             raise LicenseManagerBadServerOutput("Invalid data returned from parser.")
 
         report_item = LicenseReportItem(
             product_feature=product_feature,
             used=current_feature_item["used"],
             total=current_feature_item["total"],
-            used_licenses=current_feature_item["uses"],
         )
 
         return report_item
```

### Comparing `license_manager_agent-2.3.2/lm_agent/server_interfaces/rlm.py` & `license_manager_agent-3.0.0/lm_agent/server_interfaces/olicense.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,94 +1,70 @@
-"""RLM license server interface."""
+"""OLicense license server interface."""
 import typing
 
+from lm_agent.backend_utils.models import LicenseServerSchema
 from lm_agent.config import settings
 from lm_agent.exceptions import LicenseManagerBadServerOutput
-from lm_agent.parsing import rlm
+from lm_agent.parsing import olicense
 from lm_agent.server_interfaces.license_server_interface import LicenseReportItem, LicenseServerInterface
 from lm_agent.utils import run_command
 
 
-class RLMLicenseServer(LicenseServerInterface):
-    """Extract license information from RLM license server."""
+class OLicenseLicenseServer(LicenseServerInterface):
+    """Extract license information from OLicense license server."""
 
-    def __init__(self, license_servers: typing.List[str]):
+    def __init__(self, license_servers: typing.List[LicenseServerSchema]):
+        """Initialize the license server instance with the license server host and parser."""
         self.license_servers = license_servers
-        self.parser = rlm.parse
+        self.parser = olicense.parse
 
     def get_commands_list(self) -> typing.List[typing.List[str]]:
         """Generate a list of commands with the available license server hosts."""
 
-        host_ports = [(server.split(":")[1:]) for server in self.license_servers]
         commands_to_run = []
-        for host, port in host_ports:
-            command_line = [f"{settings.RLMUTIL_PATH}", "rlmstat", "-c", f"{port}@{host}", "-a", "-p"]
+        for license_server in self.license_servers:
+            command_line = [
+                f"{settings.OLIXTOOL_PATH}",
+                "-sv",
+                f"{license_server.host}:{license_server.port}",
+            ]
             commands_to_run.append(command_line)
         return commands_to_run
 
     async def get_output_from_server(self):
-        """Override abstract method to get output from RLM license server."""
+        """Override abstract method to get output from OLicense license server."""
 
         # get the list of commands for each license server host
         commands_to_run = self.get_commands_list()
 
         # run each command in the list, one at a time, until one succeds
         for cmd in commands_to_run:
             output = await run_command(cmd)
 
             # try the next server if the previous didn't return the expected data
             if not output:
                 continue
             return output
 
-        raise RuntimeError("None of the checks for RLM succeeded!")
+        raise RuntimeError("None of the checks for OLicense succeeded!")
 
     async def get_report_item(self, product_feature: str):
-        """Override abstract method to parse RLM license server output into License Report Item."""
+        """Override abstract method to parse OLicense license server output into License Report Item."""
 
         server_output = await self.get_output_from_server()
         parsed_output = self.parser(server_output)
 
         (_, feature) = product_feature.split(".")
 
-        current_feature_item = self._filter_current_feature(parsed_output["total"], feature)
-        used_licenses = self._filter_used_features(parsed_output["uses"], feature)
+        current_feature_item = parsed_output.get(feature)
 
         # raise exception if parser didn't output license information
-        if current_feature_item is None or used_licenses is None:
+        if current_feature_item is None:
             raise LicenseManagerBadServerOutput("Invalid data returned from parser.")
 
         report_item = LicenseReportItem(
             product_feature=product_feature,
             used=current_feature_item["used"],
             total=current_feature_item["total"],
-            used_licenses=used_licenses,
         )
 
         return report_item
-
-    def _filter_current_feature(self, parsed_list, feature):
-        """
-        The output from the RLM server returns information about all the licenses
-        in the server. This function filters the output to return only the information
-        about the feature we want.
-        """
-        for feature_item in parsed_list:
-            if feature_item["feature"] == feature:
-                return feature_item
-
-    def _filter_used_features(self, parsed_list, feature):
-        """
-        The output from the RLM server returns information about all the licenses
-        that are in use. This function filters the output to return only the information
-        about the usage of the feature we want.
-        """
-        used_licenses = []
-        for feature_booked in parsed_list:
-            if feature_booked["feature"] == feature:
-                used_licenses.append(feature_booked)
-
-        for license in used_licenses:
-            # remove the feature key, since we already handled it.
-            del license["feature"]
-
-        return used_licenses
```

### Comparing `license_manager_agent-2.3.2/lm_agent/utils.py` & `license_manager_agent-3.0.0/lm_agent/utils.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.2/lm_agent/workload_managers/slurm/cmd_utils.py` & `license_manager_agent-3.0.0/lm_agent/workload_managers/slurm/cmd_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Utilities that interact with slurm."""
 import asyncio
 import re
 import shlex
 import subprocess
 from typing import List, Optional, Union
 
-from lm_agent.backend_utils import LicenseBooking
+from lm_agent.backend_utils.models import LicenseBooking
 from lm_agent.logs import logger
 from lm_agent.workload_managers.slurm.common import (
     CMD_TIMEOUT,
     ENCODING,
     SACCTMGR_PATH,
     SCONTROL_PATH,
     SQUEUE_PATH,
@@ -67,21 +67,20 @@
         return required_licenses
 
     for requested_license in license_array:
         matched_license_items = _match_requested_license(requested_license)
         if not matched_license_items:
             continue
         product_feature = matched_license_items["product_feature"]
-        license_server_type = matched_license_items["server_type"]
-        tokens = matched_license_items["tokens"]
+        booked = matched_license_items["tokens"]
+
         # Create the license booking
         license_booking = LicenseBooking(
             product_feature=product_feature,
-            tokens=tokens,
-            license_server_type=license_server_type,
+            quantity=booked,
         )
         required_licenses.append(license_booking)
 
     return required_licenses
 
 
 async def get_tokens_for_license(
@@ -131,28 +130,26 @@
     proc = await asyncio.create_subprocess_shell(
         shlex.join(cmd), stdout=asyncio.subprocess.PIPE, stderr=asyncio.subprocess.STDOUT
     )
 
     stdout, _ = await asyncio.wait_for(proc.communicate(), CMD_TIMEOUT)
     output = str(stdout, encoding=ENCODING)
     logger.debug("##### scontrol show lic #####")
-    logger.debug(output)
     return output
 
 
 async def get_cluster_name() -> str:
     cmd = [
         SACCTMGR_PATH,
         "list",
         "cluster",
         "-nP",
         "format=Cluster",
     ]
     logger.debug("##### sacctmgr get cluster name cmd #####")
-    logger.debug(f"{' '.join(cmd)}")
 
     sacctmgr_modify_resource = await asyncio.create_subprocess_shell(
         shlex.join(cmd),
         stdout=asyncio.subprocess.PIPE,
         stderr=asyncio.subprocess.STDOUT,
     )
```

### Comparing `license_manager_agent-2.3.2/lm_agent/workload_managers/slurm/common.py` & `license_manager_agent-3.0.0/lm_agent/workload_managers/slurm/common.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.2/lm_agent/workload_managers/slurm/reservations.py` & `license_manager_agent-3.0.0/lm_agent/workload_managers/slurm/reservations.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.2/lm_agent/workload_managers/slurm/slurmctld_epilog.py` & `license_manager_agent-3.0.0/lm_agent/workload_managers/slurm/slurmctld_epilog.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python3
 """
 The EpilogSlurmctld executable.
 """
 import asyncio
 import sys
 
-from lm_agent.backend_utils import remove_booking_for_job_id
+from lm_agent.backend_utils.utils import remove_job_by_slurm_job_id
 from lm_agent.config import settings
 from lm_agent.logs import init_logging, logger
-from lm_agent.reconciliation import update_report
+from lm_agent.reconciliation import update_features
 from lm_agent.workload_managers.slurm.cmd_utils import get_required_licenses_for_job
 from lm_agent.workload_managers.slurm.common import get_job_context
 
 
 async def epilog():
     # Initialize the logger
     init_logging("slurmctld-epilog")
@@ -20,15 +20,15 @@
     job_id = job_context["job_id"]
     job_licenses = job_context["job_licenses"]
 
     # Check if reconciliation should be triggered.
     if settings.USE_RECONCILE_IN_PROLOG_EPILOG:
         # Force a reconciliation before we attempt to remove bookings.
         try:
-            await update_report()
+            await update_features()
         except Exception as e:
             logger.error(f"Failed to call reconcile with {e}")
             sys.exit(1)
 
     try:
         required_licenses = get_required_licenses_for_job(job_licenses)
     except Exception as e:
@@ -36,20 +36,16 @@
         sys.exit(1)
 
     if not required_licenses:
         logger.debug("No licenses required, exiting!")
         sys.exit(0)
 
     if len(required_licenses) > 0:
-        # Attempt to remove the booking and log the result.
-        booking_removed = await remove_booking_for_job_id(job_id)
-        if booking_removed:
-            logger.debug(f"Booking for job id: {job_id} successfully deleted.")
-        else:
-            logger.debug(f"Booking for job id: {job_id} not removed.")
+        # Attempt to remove the job with its bookings.
+        await remove_job_by_slurm_job_id(job_id)
 
 
 def main():
     asyncio.run(epilog())
 
 
 if __name__ == "__main__":
```

### Comparing `license_manager_agent-2.3.2/lm_agent/workload_managers/slurm/slurmctld_prolog.py` & `license_manager_agent-3.0.0/lm_agent/workload_managers/slurm/slurmctld_prolog.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,83 +9,84 @@
 Executing this script will result in either an exit(0) or exit(1). Slurm will
 proceed with scheduling the job if the exit status is 0, and will not proceed
 if the exit status is anything other then 0, e.g. 1.
 """
 import asyncio
 import sys
 
-from lm_agent.backend_utils import LicenseBookingRequest, get_config_from_backend, make_booking_request
+from lm_agent.backend_utils.models import LicenseBookingRequest
+from lm_agent.backend_utils.utils import get_cluster_configs_from_backend, make_booking_request
 from lm_agent.config import settings
 from lm_agent.logs import init_logging, logger
-from lm_agent.reconciliation import update_report
+from lm_agent.reconciliation import update_features
 from lm_agent.workload_managers.slurm.cmd_utils import get_required_licenses_for_job
 from lm_agent.workload_managers.slurm.common import get_job_context
 
 
 async def prolog():
     """The PrologSlurmctld for the license-manager-agent."""
     # Initialize the logger
     init_logging("slurmctld-prolog")
     # Acqure the job context
     job_context = get_job_context()
     job_id = job_context.get("job_id", "")
     user_name = job_context.get("user_name")
     lead_host = job_context.get("lead_host")
-    cluster_name = job_context.get("cluster_name")
     job_licenses = job_context.get("job_licenses")
 
     logger.info(f"Prolog started for job id: {job_id}")
 
     try:
         required_licenses = get_required_licenses_for_job(job_licenses)
-        logger.debug(f"Required licenses: {required_licenses}")
     except Exception as e:
         logger.error(f"Failed to call get_required_licenses_for_job with {e}")
         sys.exit(1)
 
     if not required_licenses:
         logger.debug("No licenses required, exiting!")
         sys.exit(0)
 
+    logger.debug(f"Required licenses: {required_licenses}")
+
     tracked_licenses = list()
-    # Create a list of tracked licenses in the form <product>.<feature>
 
+    # Create a list of tracked licenses in the form <product>.<feature>
     if len(required_licenses) > 0:
         # Create a list of tracked licenses in the form <product>.<feature>
         try:
-            entries = await get_config_from_backend()
+            entries = await get_cluster_configs_from_backend()
         except Exception as e:
             logger.error(f"Failed to call get_config_from_backend with {e}")
             sys.exit(1)
+
         for entry in entries:
             for feature in entry.features:
-                tracked_licenses.append(f"{entry.product}.{feature}")
+                tracked_licenses.append(f"{feature.product.name}.{feature.name}")
     logger.debug(f"Tracked licenses: {tracked_licenses}")
 
     # Create a tracked LicenseBookingRequest for licenses that we actually
     # track. These tracked licenses are what we will check feature token
     # availability for.
     tracked_license_booking_request = LicenseBookingRequest(
-        job_id=job_id,
-        bookings=[],
-        user_name=user_name,
+        slurm_job_id=job_id,
+        username=user_name,
         lead_host=lead_host,
-        cluster_name=cluster_name,
+        bookings=[],
     )
     for booking in required_licenses:
         if booking.product_feature in tracked_licenses:
             tracked_license_booking_request.bookings.append(booking)
     logger.debug(f"Tracked license bookings: {tracked_license_booking_request}")
 
     if len(tracked_license_booking_request.bookings) > 0:
         # Check if reconciliation should be triggered.
         if settings.USE_RECONCILE_IN_PROLOG_EPILOG:
             # Force a reconciliation before we check the feature token availability.
             try:
-                await update_report()
+                await update_features()
             except Exception as e:
                 logger.error(f"Failed to call reconcile with {e}")
                 sys.exit(1)
 
         booking_request = await make_booking_request(tracked_license_booking_request)
         if not booking_request:
             logger.debug("Booking request unsuccessful, not enough licenses.")
```

### Comparing `license_manager_agent-2.3.2/pyproject.toml` & `license_manager_agent-3.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "license-manager-agent"
-version = "2.3.2"
+version = "3.0.0"
 description = "Provides an agent for interacting with license manager"
 authors = ["OmniVector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/omnivector-solutions/license-manager"
 documentation = "https://omnivector-solutions.github.io/license-manager/"
 packages = [{ include = "lm_agent" }]
@@ -15,15 +15,15 @@
 PyJWT = "^2.4.0"
 typer = "^0.3.2"
 pydantic = {version = "^1.8.2", extras = ["dotenv"]}
 requests = "^2.26.0"
 tabulate = "^0.8.9"
 boto3 = "^1.18.17"
 sentry-sdk = "^1.3.1"
-py-buzz = "^2.1.3"
+py-buzz = "^3.2.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.4"
 pytest-asyncio = "^0.15.1"
 pytest-cov = "^2.12.1"
 pytest-env = "^0.6.2"
 respx = "^0.17.1"
```

### Comparing `license_manager_agent-2.3.2/PKG-INFO` & `license_manager_agent-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: license-manager-agent
-Version: 2.3.2
+Version: 3.0.0
 Summary: Provides an agent for interacting with license manager
 Home-page: https://github.com/omnivector-solutions/license-manager
 License: MIT
 Author: OmniVector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.8,<3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: PyJWT (>=2.4.0,<3.0.0)
 Requires-Dist: boto3 (>=1.18.17,<2.0.0)
 Requires-Dist: httpx (>=0.18.2,<0.19.0)
-Requires-Dist: py-buzz (>=2.1.3,<3.0.0)
+Requires-Dist: py-buzz (>=3.2.1,<4.0.0)
 Requires-Dist: pydantic[dotenv] (>=1.8.2,<2.0.0)
 Requires-Dist: requests (>=2.26.0,<3.0.0)
 Requires-Dist: sentry-sdk (>=1.3.1,<2.0.0)
 Requires-Dist: tabulate (>=0.8.9,<0.9.0)
 Requires-Dist: typer (>=0.3.2,<0.4.0)
 Project-URL: Documentation, https://omnivector-solutions.github.io/license-manager/
 Project-URL: Repository, https://github.com/omnivector-solutions/license-manager
```

