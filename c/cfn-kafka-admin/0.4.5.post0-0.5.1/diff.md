# Comparing `tmp/cfn_kafka_admin-0.4.5.post0.tar.gz` & `tmp/cfn_kafka_admin-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfn_kafka_admin-0.4.5.post0.tar", max compression
+gzip compressed data, was "cfn_kafka_admin-0.5.1.tar", max compression
```

## Comparing `cfn_kafka_admin-0.4.5.post0.tar` & `cfn_kafka_admin-0.5.1.tar`

### file list

```diff
@@ -1,27 +1,26 @@
--rw-r--r--   0        0        0    16725 2022-03-22 06:17:38.518532 cfn_kafka_admin-0.4.5.post0/LICENSE
--rw-r--r--   0        0        0     2314 2022-05-11 06:55:41.690789 cfn_kafka_admin-0.4.5.post0/README.rst
--rw-r--r--   0        0        0      227 2023-03-22 11:05:01.084425 cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/__init__.py
--rw-r--r--   0        0        0    21940 2023-03-22 11:01:31.193882 cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/cfn_kafka_admin.py
--rw-r--r--   0        0        0      652 2023-03-22 11:01:31.193882 cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/cfn_resources_definitions/__init__.py
--rw-r--r--   0        0        0     1905 2023-03-22 11:01:31.193882 cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/cfn_resources_definitions/custom.py
--rw-r--r--   0        0        0     1793 2023-03-22 11:01:31.194882 cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/cfn_resources_definitions/resource.py
--rw-r--r--   0        0        0     1852 2023-03-22 11:01:31.194882 cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/cli.py
--rw-r--r--   0        0        0     1651 2023-03-22 11:01:31.194882 cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/common.py
--rw-r--r--   0        0        0      118 2023-03-22 11:01:31.194882 cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/kafka/__init__.py
--rw-r--r--   0        0        0     3334 2022-03-22 06:17:38.519532 cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/kafka/acls_management.py
--rw-r--r--   0        0        0     5104 2023-03-22 11:01:31.195882 cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/kafka/topics_management.py
--rw-r--r--   0        0        0      118 2023-03-22 11:01:31.195882 cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/lambda_functions/__init__.py
--rw-r--r--   0        0        0     4861 2023-03-22 11:01:31.195882 cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/lambda_functions/acls.py
--rw-r--r--   0        0        0     6363 2023-03-22 11:01:31.195882 cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/lambda_functions/schemas.py
--rw-r--r--   0        0        0     6614 2023-03-22 11:01:31.195882 cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/lambda_functions/topics.py
--rw-r--r--   0        0        0      118 2023-03-22 11:01:31.196882 cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/models/__init__.py
--rw-r--r--   0        0        0    12345 2023-03-22 11:01:31.196882 cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/models/admin.py
--rw-r--r--   0        0        0      118 2023-03-22 11:01:31.196882 cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/specs/__init__.py
--rw-r--r--   0        0        0     2990 2023-03-22 11:05:01.702432 cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/specs/aws-cfn-kafka-admin-provider-schema.json
--rw-r--r--   0        0        0     2466 2023-03-22 11:05:01.702432 cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/specs/ews-kafka-acl.json
--rw-r--r--   0        0        0     2386 2023-03-22 11:05:01.701433 cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/specs/ews-kafka-parameters.json
--rw-r--r--   0        0        0     2130 2023-03-22 11:05:01.702432 cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/specs/ews-kafka-schema.json
--rw-r--r--   0        0        0     7084 2023-03-22 11:05:01.702432 cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/specs/ews-kafka-topic.json
--rw-r--r--   0        0        0     2469 2023-03-22 11:05:01.084425 cfn_kafka_admin-0.4.5.post0/pyproject.toml
--rw-r--r--   0        0        0     3663 1970-01-01 00:00:00.000000 cfn_kafka_admin-0.4.5.post0/setup.py
--rw-r--r--   0        0        0     3802 1970-01-01 00:00:00.000000 cfn_kafka_admin-0.4.5.post0/PKG-INFO
+-rw-r--r--   0        0        0    16725 2022-03-22 06:17:38.518532 cfn_kafka_admin-0.5.1/LICENSE
+-rw-r--r--   0        0        0     2314 2022-05-11 06:55:41.690789 cfn_kafka_admin-0.5.1/README.rst
+-rw-r--r--   0        0        0      221 2023-08-08 05:19:36.860624 cfn_kafka_admin-0.5.1/cfn_kafka_admin/__init__.py
+-rw-r--r--   0        0        0    21939 2023-04-24 12:49:19.847982 cfn_kafka_admin-0.5.1/cfn_kafka_admin/cfn_kafka_admin.py
+-rw-r--r--   0        0        0      652 2023-04-24 12:49:19.847982 cfn_kafka_admin-0.5.1/cfn_kafka_admin/cfn_resources_definitions/__init__.py
+-rw-r--r--   0        0        0     1905 2023-04-24 12:49:19.847982 cfn_kafka_admin-0.5.1/cfn_kafka_admin/cfn_resources_definitions/custom.py
+-rw-r--r--   0        0        0     1793 2023-04-24 12:49:19.847982 cfn_kafka_admin-0.5.1/cfn_kafka_admin/cfn_resources_definitions/resource.py
+-rw-r--r--   0        0        0     1852 2023-04-24 12:49:19.848981 cfn_kafka_admin-0.5.1/cfn_kafka_admin/cli.py
+-rw-r--r--   0        0        0     2949 2023-05-05 09:04:48.510208 cfn_kafka_admin-0.5.1/cfn_kafka_admin/common.py
+-rw-r--r--   0        0        0      136 2023-06-08 12:02:54.094616 cfn_kafka_admin-0.5.1/cfn_kafka_admin/kafka_resources/__init__.py
+-rw-r--r--   0        0        0     3309 2023-04-24 12:49:19.848981 cfn_kafka_admin-0.5.1/cfn_kafka_admin/kafka_resources/acls_management.py
+-rw-r--r--   0        0        0     4672 2023-08-08 05:11:41.636003 cfn_kafka_admin-0.5.1/cfn_kafka_admin/kafka_resources/topics_management.py
+-rw-r--r--   0        0        0      136 2023-04-24 12:49:19.849982 cfn_kafka_admin-0.5.1/cfn_kafka_admin/lambda_functions/__init__.py
+-rw-r--r--   0        0        0     4869 2023-06-08 12:02:54.095616 cfn_kafka_admin-0.5.1/cfn_kafka_admin/lambda_functions/acls.py
+-rw-r--r--   0        0        0     6357 2023-04-24 12:49:19.849982 cfn_kafka_admin-0.5.1/cfn_kafka_admin/lambda_functions/schemas.py
+-rw-r--r--   0        0        0     8762 2023-06-08 12:02:54.095616 cfn_kafka_admin-0.5.1/cfn_kafka_admin/lambda_functions/topics.py
+-rw-r--r--   0        0        0      118 2023-04-24 12:49:19.850982 cfn_kafka_admin-0.5.1/cfn_kafka_admin/models/__init__.py
+-rw-r--r--   0        0        0    12373 2023-08-08 05:11:41.833005 cfn_kafka_admin-0.5.1/cfn_kafka_admin/models/admin.py
+-rw-r--r--   0        0        0      118 2023-04-24 12:49:19.850982 cfn_kafka_admin-0.5.1/cfn_kafka_admin/specs/__init__.py
+-rw-r--r--   0        0        0     2990 2023-08-08 05:19:37.448631 cfn_kafka_admin-0.5.1/cfn_kafka_admin/specs/aws-cfn-kafka-admin-provider-schema.json
+-rw-r--r--   0        0        0     2466 2023-08-08 05:19:37.448631 cfn_kafka_admin-0.5.1/cfn_kafka_admin/specs/ews-kafka-acl.json
+-rw-r--r--   0        0        0     2386 2023-08-08 05:19:37.448631 cfn_kafka_admin-0.5.1/cfn_kafka_admin/specs/ews-kafka-parameters.json
+-rw-r--r--   0        0        0     2130 2023-08-08 05:19:37.448631 cfn_kafka_admin-0.5.1/cfn_kafka_admin/specs/ews-kafka-schema.json
+-rw-r--r--   0        0        0     7084 2023-08-08 05:19:37.448631 cfn_kafka_admin-0.5.1/cfn_kafka_admin/specs/ews-kafka-topic.json
+-rw-r--r--   0        0        0     2449 2023-08-08 05:19:36.860624 cfn_kafka_admin-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3581 1970-01-01 00:00:00.000000 cfn_kafka_admin-0.5.1/PKG-INFO
```

### Comparing `cfn_kafka_admin-0.4.5.post0/LICENSE` & `cfn_kafka_admin-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.4.5.post0/README.rst` & `cfn_kafka_admin-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/cfn_kafka_admin.py` & `cfn_kafka_admin-0.5.1/cfn_kafka_admin/cfn_kafka_admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -307,15 +307,14 @@
         registry_password,
         registry_userinfo,
         schema_class,
         attribute: TopicSchemaDef,
         subject_suffix: str,
         deletion_policy,
     ):
-
         definition = self.define_schema_definition_path(
             topic_name, subject_suffix, attribute
         )
         topic_schema_r = schema_class(
             f"{topic_name}{SerializerDef[attribute.Serializer.name].value}{subject_suffix}Schema",
             DeletionPolicy=deletion_policy,
             SerializeAttribute=subject_suffix,
```

### Comparing `cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/cfn_resources_definitions/__init__.py` & `cfn_kafka_admin-0.5.1/cfn_kafka_admin/cfn_resources_definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/cfn_resources_definitions/custom.py` & `cfn_kafka_admin-0.5.1/cfn_kafka_admin/cfn_resources_definitions/custom.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/cfn_resources_definitions/resource.py` & `cfn_kafka_admin-0.5.1/cfn_kafka_admin/cfn_resources_definitions/resource.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/cli.py` & `cfn_kafka_admin-0.5.1/cfn_kafka_admin/cli.py`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/kafka/acls_management.py` & `cfn_kafka_admin-0.5.1/cfn_kafka_admin/kafka_resources/acls_management.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#  -*- coding: utf-8 -*-
 # SPDX-License-Identifier: MPL-2.0
 # Copyright 2021 John Mille<john@ews-network.net>
 
 """
 Module to handle Kafka topics management.
 """
```

### Comparing `cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/kafka/topics_management.py` & `cfn_kafka_admin-0.5.1/cfn_kafka_admin/kafka_resources/topics_management.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,124 +1,122 @@
-#  -*- coding: utf-8 -*-
 # SPDX-License-Identifier: MPL-2.0
 # Copyright 2021 John Mille<john@ews-network.net>
 
 """
 Module to handle Kafka topics management.
 """
 
+import logging
+from os import environ
+from random import randint
+
 from kafka import KafkaConsumer, errors
 from kafka.admin import (
     ConfigResource,
     ConfigResourceType,
     KafkaAdminClient,
     NewPartitions,
     NewTopic,
 )
+from retry import retry
+
+from cfn_kafka_admin.common import KAFKA_LOG, setup_logging
+
+LOG = setup_logging(__file__)
+
+KAFKA_LOG.setLevel(logging.WARNING)
+KAFKA_DEBUG = environ.get("DEBUG_KAFKA_CLIENT", False)
+if KAFKA_DEBUG:
+    KAFKA_LOG.setLevel(logging.DEBUG)
+    KAFKA_LOG.handlers[0].setLevel(logging.DEBUG)
 
+RETRY_ATTEMPTS = max(abs(int(environ.get("CREATE_RETRY_ATTEMPTS", 3))), 5)
+RETRY_JITTER = randint(1, 5)
 
+
+@retry(
+    (errors.KafkaError,),
+    tries=RETRY_ATTEMPTS,
+    jitter=RETRY_JITTER,
+    logger=LOG,
+)
 def create_new_kafka_topic(
     name,
-    partitions,
-    cluster_info,
-    replication_factor=None,
-    settings=None,
+    partitions: int,
+    cluster_info: dict,
+    replication_factor: int,
+    settings: dict = None,
 ):
     """
     Function to create new Kafka topic
 
     :param str name:
     :param int partitions:
     :param dict cluster_info: Dictionary with the Kafka information
     :param int replication_factor: Replication factor. Defaults to 3
     :param dict settings: Additional topics new_settings
     """
-    if not replication_factor:
-        replication_factor = 1
+    if replication_factor < 0:
+        raise ValueError("Topic partitions must be >= 1")
+    LOG.debug(f"CREATE_RETRY_ATTEMPTS: {RETRY_ATTEMPTS} - JITTER: {RETRY_JITTER}")
+    LOG.info(
+        "Attempting to create topic:(partitions/replication/settings): {}: {}/{}/{}".format(
+            name, partitions, replication_factor, settings
+        )
+    )
+    cluster_info.update(
+        {
+            "client_id": "CREATE_TOPICS"
+            + environ.get("AWS_LAMBDA_FUNCTION_NAME", "cfn-kafka-Topics")
+        }
+    )
     try:
         admin_client = KafkaAdminClient(**cluster_info)
         topic = NewTopic(name, partitions, replication_factor, topic_configs=settings)
         admin_client.create_topics([topic])
+        LOG.info(
+            "Successfully created topic:(partitions/replication): {}: {}/{}".format(
+                name, partitions, replication_factor
+            )
+        )
         return name
-    except errors.TopicAlreadyExistsError:
+    except errors.TopicAlreadyExistsError as error:
+        LOG.exception(error)
+        LOG.error(
+            LOG.info(
+                "Failed to create topic:(partitions/replication): {}: {}/{}".format(
+                    name, partitions, replication_factor
+                )
+            )
+        )
         raise errors.TopicAlreadyExistsError(f"Topic {name} already exists")
 
 
 def delete_topic(name, cluster_info):
     """
     Function to delete kafka topic
 
     :param name: name of the topic to delete
     :param cluster_info: cluster information
     :return:
     """
+    cluster_info.update(
+        {
+            "client_id": "DELETE_TOPICS"
+            + environ.get("AWS_LAMBDA_FUNCTION_NAME", "cfn-kafka-Topics")
+        }
+    )
     admin_client = KafkaAdminClient(**cluster_info)
-    admin_client.delete_topics([name])
-
-
-def validate_cleanup_policy(new_value: str, old_value: str, name: str) -> None:
-    """
-    Validates that the update for cleanup.policy does not go from delete to compact, which is invalid.
-
-    :param str new_value:
-    :param str old_value:
-    :param str name:
-    :raises: ValueError when changing from `delete` to `compact`
-    """
-    if old_value == "delete" and new_value == "compact":
-        raise ValueError(
-            name, "You cannot change cleanup.policy from delete to cleanup."
-        )
-
-
-def kafka_update_rules(topic_configs: tuple, new_settings: dict, name: str):
-    """
-    Ensures update is possible
-
-    :param tuple(str, str, list) topic_configs:
-    :param dict new_settings:
-    :param str name:
-    :return:
-    """
-    properties = {
-        "cleanup.policy": (True, validate_cleanup_policy),
-        "compression.type": (False, None),
-        "connection.failed.authentication.delay.ms": (False, None),
-        "default.replication.factor": (False, None),
-        "delete.retention.ms": (True, None),
-        "file.delete.delay.ms": (False, None),
-        "flush.messages": (False, None),
-        "flush.ms": (False, None),
-        "group.max.session.timeout.ms": (False, None),
-        "index.interval.bytes": (False, None),
-        "max.message.bytes": (True, None),
-        "max.compaction.lag.ms": (True, None),
-        "message.timestamp.type": (True, None),
-        "min.cleanable.dirty.ratio": (False, None),
-        "min.compaction.lag.ms": (True, None),
-        "min.insync.replicas": (True, None),
-        "retention.bytes": (True, None),
-        "retention.ms": (True, None),
-    }
-    current_settings = topic_configs[2]
-    c_settings_map = {}
-    for c_setting in current_settings:
-        c_settings_map[c_setting[0]] = c_setting[1]
-
-    for key, new_value in new_settings.items():
-        set_value = topic_configs[key]
-        if set_value == new_value:
-            continue
-        else:
-            if key not in properties:
-                continue
-            if not properties[key][0]:
-                raise ValueError(name, "Value for", key, "is immutable")
-            elif properties[key][0] and properties[key][1]:
-                properties[key][1](new_value, set_value, name)
+    LOG.info(f"Deleting Topic {name}")
+    try:
+        admin_client.delete_topics([name])
+        LOG.debug(f"Successfully deleted topic:(partitions/replication): {name}")
+    except Exception as error:
+        LOG.exception(error)
+        raise
 
 
 def update_kafka_topic(
     name: str, partitions: int, cluster_info: dict, settings: dict
 ) -> None:
     """
     Function to update existing Kafka topic
@@ -130,15 +128,14 @@
     :return:
     """
     consumer_client = KafkaConsumer(**cluster_info)
     admin_client = KafkaAdminClient(**cluster_info)
     configs = admin_client.describe_configs(
         config_resources=[ConfigResource(ConfigResourceType.TOPIC, name)]
     )
-    kafka_update_rules(configs, settings, name)
     curr_partitions = consumer_client.partitions_for_topic(name)
     if curr_partitions:
         curr_partitions_count = len(curr_partitions)
     else:
         raise LookupError(
             f"Failed to retrieve the current number of partitions for {name}"
         )
```

### Comparing `cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/lambda_functions/acls.py` & `cfn_kafka_admin-0.5.1/cfn_kafka_admin/lambda_functions/acls.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-#  -*- coding: utf-8 -*-
 # SPDX-License-Identifier: MPL-2.0
 # Copyright 2021 John Mille<john@ews-network.net>
 
 """Main module."""
+
+from __future__ import annotations
+
 import uuid
 
 from aws_cfn_custom_resource_resolve_parser import handle
 from cfn_resource_provider import ResourceProvider
 from compose_x_common.compose_x_common import keyisset, keypresent
 
 from cfn_kafka_admin.common import setup_logging
-from cfn_kafka_admin.kafka.acls_management import (
+from cfn_kafka_admin.kafka_resources.acls_management import (
     create_new_acls,
     delete_acls,
     differentiate_old_new_acls,
 )
 from cfn_kafka_admin.models.admin import EwsKafkaAcl
 
 LOG = setup_logging()
@@ -22,15 +24,15 @@
 
 class KafkaACL(ResourceProvider):
     def __init__(self):
         """
         Init method
         """
         self.cluster_info = {}
-        super(KafkaACL, self).__init__()
+        super().__init__()
         self.request_schema = EwsKafkaAcl.schema()
 
     def convert_property_types(self):
         int_props = []
         boolean_props = []
         for prop in int_props:
             if keypresent(prop, self.properties) and isinstance(
```

### Comparing `cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/lambda_functions/schemas.py` & `cfn_kafka_admin-0.5.1/cfn_kafka_admin/lambda_functions/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-#  -*- coding: utf-8 -*-
 # SPDX-License-Identifier: MPL-2.0
 # Copyright 2021 John Mille<john@ews-network.net>
 
 """Module to handle the custom resource for Schemas"""
 
+from __future__ import annotations
+
 import json
 import logging
 import re
 
 from aws_cfn_custom_resource_resolve_parser import handle
 from boto3.session import Session
 from cfn_resource_provider import ResourceProvider
@@ -61,15 +62,15 @@
 class KafkaSchema(ResourceProvider):
     """
     Class for custom resource to handle a Kafka Schema
     """
 
     def __init__(self):
         self.cluster_info = {}
-        super(KafkaSchema, self).__init__()
+        super().__init__()
         self.request_schema = EwsKafkaSchema.schema()
 
     def try_replace_from_secret(self, param):
         if (
             isinstance(self.get(param), str)
             and self.get(param).find("resolve:secretsmanager") >= 0
         ):
```

### Comparing `cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/models/admin.py` & `cfn_kafka_admin-0.5.1/cfn_kafka_admin/models/admin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  aws-cfn-kafka-admin-provider-schema.json
-#   timestamp: 2022-05-12T15:39:14+00:00
+#   timestamp: 2023-08-08T05:11:20+00:00
 
 from __future__ import annotations
 
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
 from pydantic import BaseModel, Extra, Field, confloat, conint, constr
@@ -40,15 +40,15 @@
     JSON = "JSON"
     PROTOBUF = "PROTOBUF"
 
 
 class TopicSchemaDef(BaseModel):
     Serializer: SerializerDef
     Definition: Optional[Union[str, Dict[str, Any]]] = None
-    CompatibilityMode: Optional[CompatibilityMode] = None
+    CompatibilityMode: Optional[CompatibilityMode] = "NONE"
 
 
 class BootstrapServers(BaseModel):
     __root__: str = Field(
         ..., description="Endpoint URL of the Kafka cluster in the format hostname:port"
     )
 
@@ -270,15 +270,15 @@
     RegistryUrl: Optional[RegistryUrl] = None
     RegistryUsername: Optional[RegistryUsername] = None
     RegistryPassword: Optional[RegistryPassword] = None
     RegistryUserInfo: Optional[RegistryUserInfo] = None
     Subject: Optional[str] = None
     Serializer: Optional[SerializerDef] = None
     Definition: Optional[Union[str, Dict[str, Any]]] = None
-    CompatibilityMode: Optional[CompatibilityMode] = None
+    CompatibilityMode: Optional[CompatibilityMode] = "NONE"
     ServiceToken: Optional[str] = Field(None, description="The Lambda Function ARN")
     PermanentlyDelete: Optional[bool] = Field(
         False,
         description="If set to true, the Schema is set to hard delete. Use carefully",
     )
 
 
@@ -290,41 +290,41 @@
     FunctionName: Optional[str] = Field(
         None, description="Name or ARN of the Schema Registry function to use"
     )
     RegistryUrl: Optional[str] = None
     RegistryUsername: Optional[RegistryUsername] = None
     RegistryPassword: Optional[RegistryPassword] = None
     RegistryUserInfo: Optional[RegistryUserInfo] = None
-    CompatibilityMode: Optional[CompatibilityMode] = None
+    CompatibilityMode: Optional[CompatibilityMode] = "NONE"
     DeletionPolicy: Optional[DeletionPolicy] = Field(
         "Retain",
         description="When set, overrides the DeletionPolicy set as default for all schemas",
     )
     S3Store: Optional[S3Store] = None
 
 
 class EwsKafkaParameters(BaseModel):
     BootstrapServers: Optional[BootstrapServers] = None
-    SecurityProtocol: Optional[SecurityProtocol] = None
-    SASLMechanism: Optional[SASLMechanism] = None
+    SecurityProtocol: Optional[SecurityProtocol] = "PLAINTEXT"
+    SASLMechanism: Optional[SASLMechanism] = "PLAIN"
     SASLUsername: Optional[SASLUsername] = None
     SASLPassword: Optional[SASLPassword] = None
     RegistryUrl: Optional[RegistryUrl] = None
     RegistryUsername: Optional[RegistryUsername] = None
     RegistryPassword: Optional[RegistryPassword] = None
-    CompatibilityMode: Optional[CompatibilityMode] = None
+    CompatibilityMode: Optional[CompatibilityMode] = "NONE"
 
 
 class EwsKafkaTopic(BaseModel):
     Name: Name
     PartitionsCount: PartitionsCount
     ReplicationFactor: Optional[ReplicationFactor] = None
     BootstrapServers: Optional[BootstrapServers] = None
-    SecurityProtocol: Optional[SecurityProtocol] = None
-    SASLMechanism: Optional[SASLMechanism] = None
+    SecurityProtocol: Optional[SecurityProtocol] = "PLAINTEXT"
+    SASLMechanism: Optional[SASLMechanism] = "PLAIN"
     SASLUsername: Optional[SASLUsername] = None
     SASLPassword: Optional[SASLPassword] = None
     Schema: Optional[TopicSchemas] = None
     Settings: Optional[TopicsSettings] = None
 
 
 class Policies(BaseModel):
```

### Comparing `cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/specs/aws-cfn-kafka-admin-provider-schema.json` & `cfn_kafka_admin-0.5.1/cfn_kafka_admin/specs/aws-cfn-kafka-admin-provider-schema.json`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/specs/ews-kafka-acl.json` & `cfn_kafka_admin-0.5.1/cfn_kafka_admin/specs/ews-kafka-acl.json`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/specs/ews-kafka-parameters.json` & `cfn_kafka_admin-0.5.1/cfn_kafka_admin/specs/ews-kafka-parameters.json`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/specs/ews-kafka-schema.json` & `cfn_kafka_admin-0.5.1/cfn_kafka_admin/specs/ews-kafka-schema.json`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.4.5.post0/cfn_kafka_admin/specs/ews-kafka-topic.json` & `cfn_kafka_admin-0.5.1/cfn_kafka_admin/specs/ews-kafka-topic.json`

 * *Files identical despite different names*

### Comparing `cfn_kafka_admin-0.4.5.post0/pyproject.toml` & `cfn_kafka_admin-0.5.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,68 +1,70 @@
 [tool.poetry]
 name = "cfn_kafka_admin"
-version = "0.4.5.post0"
+version = "0.5.1"
 description = "AWS CloudFormation Resources to manage Kafka"
-authors = ["johnpreston <john@compose-x.io>"]
-license = "MPL-2.0"
+authors = ["John Mille <john@compose-x.io>"]
 classifiers = [
   "Natural Language :: English",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
 ]
+
 readme = "README.rst"
+license = "LICENSE"
+
 [tool.poetry.urls]
 "Source" = "https://github.com/compose-x/cfn-kafka-admin"
 "Bug Tracker" = "https://github.com/compose-x/cfn-kafka-admin/issues"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-compose-x-common = "^0.5.0"
-jsonschema = "^4.5.1"
-importlib-resources = "^5.7.1"
+compose-x-common = "^1.2"
+jsonschema = "4.17.3"
+importlib-resources = "^6.0"
 PyYAML = "^6.0"
-troposphere = "^4.0.1"
-kafka-schema-registry-admin = "^0.1.0"
-datamodel-code-generator = {extras = ["http"], version = "^0.12"}
+troposphere = "^4.3"
+kafka-schema-registry-admin = "^0.2.5"
+datamodel-code-generator = { extras = ["http"], version = "^0.18" }
 aws-cfn-custom-resource-resolve-parser = "^0.2.1"
 kafka-python = "^2.0.2"
 cfn-resource-provider = "^1.0.7"
+retry2 = "^0.9.5"
+
+[tool.poetry.scripts]
+aws-cfn-kafka-admin-provider = "cfn_kafka_admin.cli:main"
 
-[tool.poetry.dev-dependencies]
-black = "^22.3.0"
-isort = "^5.10.1"
-flake8 = "^3.9.2"
+[tool.poetry.group.dev.dependencies]
+black = "^23.7"
+isort = "^5.10"
 coverage = "^5.5"
 pytest = "^6.2.5"
 pre-commit = "^2.19.0"
 tbump = "^6.8.0"
 cleanpy = "^0.3.1"
 Sphinx = "^4.5.0"
 sphinx-material = "^0.0.35"
 sphinx-jsonschema = "^1.19.1"
-pyupgrade = "^2.32.1"
-
-[tool.poetry.scripts]
-aws-cfn-kafka-admin-provider = "cfn_kafka_admin.cli:main"
+pyupgrade = "^3.3.1"
 
 [tool.datamodel-codegen]
 input = "cfn_kafka_admin/specs/aws-cfn-kafka-admin-provider-schema.json"
 input-file-type = "jsonschema"
 output = "cfn_kafka_admin/models/admin.py"
 reuse-model = "true"
-target-python-version = "3.7"
+target-python-version = "3.8"
 
 [tool.tbump]
 github_url = "https://github.com/compose-x/cfn-kafka-admin"
 
 [tool.tbump.version]
-current = "0.4.5.post0"
+current = "0.5.1"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
@@ -100,9 +102,9 @@
 ]
 [tool.coverage.run]
 omit = [
   "*/cli.py"
 ]
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cfn_kafka_admin-0.4.5.post0/PKG-INFO` & `cfn_kafka_admin-0.5.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 Metadata-Version: 2.1
 Name: cfn-kafka-admin
-Version: 0.4.5.post0
+Version: 0.5.1
 Summary: AWS CloudFormation Resources to manage Kafka
-License: MPL-2.0
-Author: johnpreston
+License: LICENSE
+Author: John Mille
 Author-email: john@compose-x.io
 Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved
+Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: aws-cfn-custom-resource-resolve-parser (>=0.2.1,<0.3.0)
 Requires-Dist: cfn-resource-provider (>=1.0.7,<2.0.0)
-Requires-Dist: compose-x-common (>=0.5.0,<0.6.0)
-Requires-Dist: datamodel-code-generator[http] (>=0.12,<0.13)
-Requires-Dist: importlib-resources (>=5.7.1,<6.0.0)
-Requires-Dist: jsonschema (>=4.5.1,<5.0.0)
+Requires-Dist: compose-x-common (>=1.2,<2.0)
+Requires-Dist: datamodel-code-generator[http] (>=0.18,<0.19)
+Requires-Dist: importlib-resources (>=6.0,<7.0)
+Requires-Dist: jsonschema (==4.17.3)
 Requires-Dist: kafka-python (>=2.0.2,<3.0.0)
-Requires-Dist: kafka-schema-registry-admin (>=0.1.0,<0.2.0)
-Requires-Dist: troposphere (>=4.0.1,<5.0.0)
+Requires-Dist: kafka-schema-registry-admin (>=0.2.5,<0.3.0)
+Requires-Dist: retry2 (>=0.9.5,<0.10.0)
+Requires-Dist: troposphere (>=4.3,<5.0)
 Project-URL: Bug Tracker, https://github.com/compose-x/cfn-kafka-admin/issues
 Project-URL: Source, https://github.com/compose-x/cfn-kafka-admin
 Description-Content-Type: text/x-rst
 
 ===============
 cfn-kafka-admin
 ===============
```

