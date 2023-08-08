# Comparing `tmp/mantium_spec-1.0.518.post1.tar.gz` & `tmp/mantium_spec-1.0.624.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mantium_spec-1.0.518.post1.tar", max compression
+gzip compressed data, was "mantium_spec-1.0.624.tar", max compression
```

## Comparing `mantium_spec-1.0.518.post1.tar` & `mantium_spec-1.0.624.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0     4975 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/README.md
--rw-r--r--   0        0        0     3201 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/__init__.py
--rw-r--r--   0        0        0      149 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/api/__init__.py
--rw-r--r--   0        0        0    21610 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/api/applications_api.py
--rw-r--r--   0        0        0    27714 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/api_client.py
--rw-r--r--   0        0        0    16336 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/configuration.py
--rw-r--r--   0        0        0     5062 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/exceptions.py
--rw-r--r--   0        0        0     2663 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/models/__init__.py
--rw-r--r--   0        0        0     8048 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/models/answer.py
--rw-r--r--   0        0        0     3653 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/models/answer_meta.py
--rw-r--r--   0        0        0     4610 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/models/application_credential.py
--rw-r--r--   0        0        0    11532 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/models/application_detail_response.py
--rw-r--r--   0        0        0     5453 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/models/application_query_request.py
--rw-r--r--   0        0        0     7116 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/models/application_query_response.py
--rw-r--r--   0        0        0     8430 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/models/application_response.py
--rw-r--r--   0        0        0     3166 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/models/application_status.py
--rw-r--r--   0        0        0    22881 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/models/chat_gpt_plugin_application_detail_response.py
--rw-r--r--   0        0        0     5764 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/models/content_creation_template_options.py
--rw-r--r--   0        0        0     3115 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/models/content_type.py
--rw-r--r--   0        0        0     3376 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/models/credential_type.py
--rw-r--r--   0        0        0     5855 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/models/cursor_datamodel_page_application_response.py
--rw-r--r--   0        0        0     8294 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/models/custom_template_options.py
--rw-r--r--   0        0        0     5764 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/models/customer_support_template_options.py
--rw-r--r--   0        0        0     6158 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/models/document.py
--rw-r--r--   0        0        0     3905 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/models/document_metadata.py
--rw-r--r--   0        0        0     5728 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/models/event_planning_template_options.py
--rw-r--r--   0        0        0     3695 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/models/http_validation_error.py
--rw-r--r--   0        0        0     5746 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/models/legal_documents_template_options.py
--rw-r--r--   0        0        0     2965 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/models/location_inner.py
--rw-r--r--   0        0        0     5692 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/models/meeting_info_template_options.py
--rw-r--r--   0        0        0     5982 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/models/personal_knowledge_management_template_options.py
--rw-r--r--   0        0        0     5854 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/models/product_documentation_template_options.py
--rw-r--r--   0        0        0     5782 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/models/recipe_management_template_options.py
--rw-r--r--   0        0        0    22121 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/models/response_get_application_detail.py
--rw-r--r--   0        0        0     5618 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/models/shopify_template_options.py
--rw-r--r--   0        0        0     4337 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/models/span.py
--rw-r--r--   0        0        0     7930 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/models/template.py
--rw-r--r--   0        0        0     5221 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/models/validation_error.py
--rw-r--r--   0        0        0    12591 2023-07-26 23:25:15.000000 mantium_spec-1.0.518.post1/mantium_spec/rest.py
--rw-r--r--   0        0        0      374 2023-07-26 23:25:31.564378 mantium_spec-1.0.518.post1/pyproject.toml
--rw-r--r--   0        0        0     5804 1970-01-01 00:00:00.000000 mantium_spec-1.0.518.post1/setup.py
--rw-r--r--   0        0        0     5544 1970-01-01 00:00:00.000000 mantium_spec-1.0.518.post1/PKG-INFO
+-rw-r--r--   0        0        0     5013 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/README.md
+-rw-r--r--   0        0        0     3259 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/__init__.py
+-rw-r--r--   0        0        0      149 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/api/__init__.py
+-rw-r--r--   0        0        0    21604 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/api/applications_api.py
+-rw-r--r--   0        0        0    27708 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/api_client.py
+-rw-r--r--   0        0        0    16324 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/configuration.py
+-rw-r--r--   0        0        0     5056 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/exceptions.py
+-rw-r--r--   0        0        0     2721 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/models/__init__.py
+-rw-r--r--   0        0        0     7239 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/models/answer.py
+-rw-r--r--   0        0        0     3647 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/models/answer_meta.py
+-rw-r--r--   0        0        0     4604 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/models/application_credential.py
+-rw-r--r--   0        0        0    14386 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/models/application_detail_response.py
+-rw-r--r--   0        0        0     5447 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/models/application_query_request.py
+-rw-r--r--   0        0        0     7110 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/models/application_query_response.py
+-rw-r--r--   0        0        0    11212 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/models/application_response.py
+-rw-r--r--   0        0        0     3160 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/models/application_status.py
+-rw-r--r--   0        0        0    25729 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/models/chat_gpt_plugin_application_detail_response.py
+-rw-r--r--   0        0        0     5758 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/models/content_creation_template_options.py
+-rw-r--r--   0        0        0     3109 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/models/content_type.py
+-rw-r--r--   0        0        0     3370 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/models/credential_type.py
+-rw-r--r--   0        0        0     5849 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/models/cursor_datamodel_page_application_response.py
+-rw-r--r--   0        0        0     8288 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/models/custom_template_options.py
+-rw-r--r--   0        0        0     5758 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/models/customer_support_template_options.py
+-rw-r--r--   0        0        0     3562 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/models/data_source_type.py
+-rw-r--r--   0        0        0     6152 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/models/document.py
+-rw-r--r--   0        0        0     3899 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/models/document_metadata.py
+-rw-r--r--   0        0        0     5722 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/models/event_planning_template_options.py
+-rw-r--r--   0        0        0     3689 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/models/http_validation_error.py
+-rw-r--r--   0        0        0     5740 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/models/legal_documents_template_options.py
+-rw-r--r--   0        0        0     2959 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/models/location_inner.py
+-rw-r--r--   0        0        0     5686 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/models/meeting_info_template_options.py
+-rw-r--r--   0        0        0     5976 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/models/personal_knowledge_management_template_options.py
+-rw-r--r--   0        0        0     5848 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/models/product_documentation_template_options.py
+-rw-r--r--   0        0        0     5776 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/models/recipe_management_template_options.py
+-rw-r--r--   0        0        0    24849 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/models/response_get_application_detail.py
+-rw-r--r--   0        0        0     5612 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/models/shopify_template_options.py
+-rw-r--r--   0        0        0     4331 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/models/span.py
+-rw-r--r--   0        0        0     7924 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/models/template.py
+-rw-r--r--   0        0        0     5215 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/models/validation_error.py
+-rw-r--r--   0        0        0    12585 2023-08-08 18:40:10.000000 mantium_spec-1.0.624/mantium_spec/rest.py
+-rw-r--r--   0        0        0      368 2023-08-08 18:40:30.292247 mantium_spec-1.0.624/pyproject.toml
+-rw-r--r--   0        0        0     5837 1970-01-01 00:00:00.000000 mantium_spec-1.0.624/setup.py
+-rw-r--r--   0        0        0     5576 1970-01-01 00:00:00.000000 mantium_spec-1.0.624/PKG-INFO
```

### Comparing `mantium_spec-1.0.518.post1/README.md` & `mantium_spec-1.0.624/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # mantium-spec
 Mantium API Documentation
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0.518.post1
+- API version: 1.0.624
 - Package version: 1.0.0
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
@@ -109,14 +109,15 @@
  - [ChatGPTPluginApplicationDetailResponse](docs/ChatGPTPluginApplicationDetailResponse.md)
  - [ContentCreationTemplateOptions](docs/ContentCreationTemplateOptions.md)
  - [ContentType](docs/ContentType.md)
  - [CredentialType](docs/CredentialType.md)
  - [CursorDatamodelPageApplicationResponse](docs/CursorDatamodelPageApplicationResponse.md)
  - [CustomTemplateOptions](docs/CustomTemplateOptions.md)
  - [CustomerSupportTemplateOptions](docs/CustomerSupportTemplateOptions.md)
+ - [DataSourceType](docs/DataSourceType.md)
  - [Document](docs/Document.md)
  - [DocumentMetadata](docs/DocumentMetadata.md)
  - [EventPlanningTemplateOptions](docs/EventPlanningTemplateOptions.md)
  - [HTTPValidationError](docs/HTTPValidationError.md)
  - [LegalDocumentsTemplateOptions](docs/LegalDocumentsTemplateOptions.md)
  - [LocationInner](docs/LocationInner.md)
  - [MeetingInfoTemplateOptions](docs/MeetingInfoTemplateOptions.md)
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/__init__.py` & `mantium_spec-1.0.624/mantium_spec/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # flake8: noqa
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 __version__ = "1.0.0"
@@ -40,14 +40,15 @@
 from mantium_spec.models.chat_gpt_plugin_application_detail_response import ChatGPTPluginApplicationDetailResponse
 from mantium_spec.models.content_creation_template_options import ContentCreationTemplateOptions
 from mantium_spec.models.content_type import ContentType
 from mantium_spec.models.credential_type import CredentialType
 from mantium_spec.models.cursor_datamodel_page_application_response import CursorDatamodelPageApplicationResponse
 from mantium_spec.models.custom_template_options import CustomTemplateOptions
 from mantium_spec.models.customer_support_template_options import CustomerSupportTemplateOptions
+from mantium_spec.models.data_source_type import DataSourceType
 from mantium_spec.models.document import Document
 from mantium_spec.models.document_metadata import DocumentMetadata
 from mantium_spec.models.event_planning_template_options import EventPlanningTemplateOptions
 from mantium_spec.models.http_validation_error import HTTPValidationError
 from mantium_spec.models.legal_documents_template_options import LegalDocumentsTemplateOptions
 from mantium_spec.models.location_inner import LocationInner
 from mantium_spec.models.meeting_info_template_options import MeetingInfoTemplateOptions
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/api/applications_api.py` & `mantium_spec-1.0.624/mantium_spec/api/applications_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/api_client.py` & `mantium_spec-1.0.624/mantium_spec/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
 import datetime
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/configuration.py` & `mantium_spec-1.0.624/mantium_spec/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import copy
@@ -384,15 +384,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.0.518.post1\n"\
+               "Version of the API: 1.0.624\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/exceptions.py` & `mantium_spec-1.0.624/mantium_spec/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/models/__init__.py` & `mantium_spec-1.0.624/mantium_spec/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 # import models into model package
@@ -25,14 +25,15 @@
 from mantium_spec.models.chat_gpt_plugin_application_detail_response import ChatGPTPluginApplicationDetailResponse
 from mantium_spec.models.content_creation_template_options import ContentCreationTemplateOptions
 from mantium_spec.models.content_type import ContentType
 from mantium_spec.models.credential_type import CredentialType
 from mantium_spec.models.cursor_datamodel_page_application_response import CursorDatamodelPageApplicationResponse
 from mantium_spec.models.custom_template_options import CustomTemplateOptions
 from mantium_spec.models.customer_support_template_options import CustomerSupportTemplateOptions
+from mantium_spec.models.data_source_type import DataSourceType
 from mantium_spec.models.document import Document
 from mantium_spec.models.document_metadata import DocumentMetadata
 from mantium_spec.models.event_planning_template_options import EventPlanningTemplateOptions
 from mantium_spec.models.http_validation_error import HTTPValidationError
 from mantium_spec.models.legal_documents_template_options import LegalDocumentsTemplateOptions
 from mantium_spec.models.location_inner import LocationInner
 from mantium_spec.models.meeting_info_template_options import MeetingInfoTemplateOptions
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/models/answer.py` & `mantium_spec-1.0.624/mantium_spec/models/answer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
@@ -64,19 +64,24 @@
         self._context = None
         self._offsets_in_document = None
         self._offsets_in_context = None
         self._meta = None
         self.discriminator = None
 
         self.answer = answer
-        self.score = score
-        self.context = context
-        self.offsets_in_document = offsets_in_document
-        self.offsets_in_context = offsets_in_context
-        self.meta = meta
+        if score is not None:
+            self.score = score
+        if context is not None:
+            self.context = context
+        if offsets_in_document is not None:
+            self.offsets_in_document = offsets_in_document
+        if offsets_in_context is not None:
+            self.offsets_in_context = offsets_in_context
+        if meta is not None:
+            self.meta = meta
 
     @property
     def answer(self):
         """Gets the answer of this Answer.  # noqa: E501
 
 
         :return: The answer of this Answer.  # noqa: E501
@@ -111,16 +116,14 @@
     def score(self, score):
         """Sets the score of this Answer.
 
 
         :param score: The score of this Answer.  # noqa: E501
         :type score: float
         """
-        if self.local_vars_configuration.client_side_validation and score is None:  # noqa: E501
-            raise ValueError("Invalid value for `score`, must not be `None`")  # noqa: E501
 
         self._score = score
 
     @property
     def context(self):
         """Gets the context of this Answer.  # noqa: E501
 
@@ -134,16 +137,14 @@
     def context(self, context):
         """Sets the context of this Answer.
 
 
         :param context: The context of this Answer.  # noqa: E501
         :type context: str
         """
-        if self.local_vars_configuration.client_side_validation and context is None:  # noqa: E501
-            raise ValueError("Invalid value for `context`, must not be `None`")  # noqa: E501
 
         self._context = context
 
     @property
     def offsets_in_document(self):
         """Gets the offsets_in_document of this Answer.  # noqa: E501
 
@@ -157,16 +158,14 @@
     def offsets_in_document(self, offsets_in_document):
         """Sets the offsets_in_document of this Answer.
 
 
         :param offsets_in_document: The offsets_in_document of this Answer.  # noqa: E501
         :type offsets_in_document: list[Span]
         """
-        if self.local_vars_configuration.client_side_validation and offsets_in_document is None:  # noqa: E501
-            raise ValueError("Invalid value for `offsets_in_document`, must not be `None`")  # noqa: E501
 
         self._offsets_in_document = offsets_in_document
 
     @property
     def offsets_in_context(self):
         """Gets the offsets_in_context of this Answer.  # noqa: E501
 
@@ -180,16 +179,14 @@
     def offsets_in_context(self, offsets_in_context):
         """Sets the offsets_in_context of this Answer.
 
 
         :param offsets_in_context: The offsets_in_context of this Answer.  # noqa: E501
         :type offsets_in_context: list[Span]
         """
-        if self.local_vars_configuration.client_side_validation and offsets_in_context is None:  # noqa: E501
-            raise ValueError("Invalid value for `offsets_in_context`, must not be `None`")  # noqa: E501
 
         self._offsets_in_context = offsets_in_context
 
     @property
     def meta(self):
         """Gets the meta of this Answer.  # noqa: E501
 
@@ -203,16 +200,14 @@
     def meta(self, meta):
         """Sets the meta of this Answer.
 
 
         :param meta: The meta of this Answer.  # noqa: E501
         :type meta: AnswerMeta
         """
-        if self.local_vars_configuration.client_side_validation and meta is None:  # noqa: E501
-            raise ValueError("Invalid value for `meta`, must not be `None`")  # noqa: E501
 
         self._meta = meta
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/models/answer_meta.py` & `mantium_spec-1.0.624/mantium_spec/models/answer_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/models/application_credential.py` & `mantium_spec-1.0.624/mantium_spec/models/application_credential.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/models/application_detail_response.py` & `mantium_spec-1.0.624/mantium_spec/models/application_detail_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
@@ -38,54 +38,69 @@
     openapi_types = {
         'id': 'str',
         'created_at': 'datetime',
         'name': 'str',
         'description': 'str',
         'top_k': 'int',
         'status': 'ApplicationStatus',
+        'last_synced': 'datetime',
+        'storage_size': 'int',
+        'data_sources': 'list[DataSourceType]',
         'destination_id': 'str',
         'embedding_count': 'int',
         'template': 'Template'
     }
 
     attribute_map = {
         'id': 'id',
         'created_at': 'created_at',
         'name': 'name',
         'description': 'description',
         'top_k': 'top_k',
         'status': 'status',
+        'last_synced': 'last_synced',
+        'storage_size': 'storage_size',
+        'data_sources': 'data_sources',
         'destination_id': 'destination_id',
         'embedding_count': 'embedding_count',
         'template': 'template'
     }
 
-    def __init__(self, id=None, created_at=None, name=None, description=None, top_k=None, status=None, destination_id=None, embedding_count=0, template=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, created_at=None, name=None, description=None, top_k=None, status=None, last_synced=None, storage_size=0, data_sources=[], destination_id=None, embedding_count=0, template=None, local_vars_configuration=None):  # noqa: E501
         """ApplicationDetailResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._created_at = None
         self._name = None
         self._description = None
         self._top_k = None
         self._status = None
+        self._last_synced = None
+        self._storage_size = None
+        self._data_sources = None
         self._destination_id = None
         self._embedding_count = None
         self._template = None
         self.discriminator = None
 
         self.id = id
         self.created_at = created_at
         self.name = name
         self.description = description
         self.top_k = top_k
         self.status = status
+        if last_synced is not None:
+            self.last_synced = last_synced
+        if storage_size is not None:
+            self.storage_size = storage_size
+        if data_sources is not None:
+            self.data_sources = data_sources
         if destination_id is not None:
             self.destination_id = destination_id
         if embedding_count is not None:
             self.embedding_count = embedding_count
         if template is not None:
             self.template = template
 
@@ -234,14 +249,83 @@
         """
         if self.local_vars_configuration.client_side_validation and status is None:  # noqa: E501
             raise ValueError("Invalid value for `status`, must not be `None`")  # noqa: E501
 
         self._status = status
 
     @property
+    def last_synced(self):
+        """Gets the last_synced of this ApplicationDetailResponse.  # noqa: E501
+
+        The last time a DatasetUpdate job ran for the application  # noqa: E501
+
+        :return: The last_synced of this ApplicationDetailResponse.  # noqa: E501
+        :rtype: datetime
+        """
+        return self._last_synced
+
+    @last_synced.setter
+    def last_synced(self, last_synced):
+        """Sets the last_synced of this ApplicationDetailResponse.
+
+        The last time a DatasetUpdate job ran for the application  # noqa: E501
+
+        :param last_synced: The last_synced of this ApplicationDetailResponse.  # noqa: E501
+        :type last_synced: datetime
+        """
+
+        self._last_synced = last_synced
+
+    @property
+    def storage_size(self):
+        """Gets the storage_size of this ApplicationDetailResponse.  # noqa: E501
+
+        current file storage size for the application  # noqa: E501
+
+        :return: The storage_size of this ApplicationDetailResponse.  # noqa: E501
+        :rtype: int
+        """
+        return self._storage_size
+
+    @storage_size.setter
+    def storage_size(self, storage_size):
+        """Sets the storage_size of this ApplicationDetailResponse.
+
+        current file storage size for the application  # noqa: E501
+
+        :param storage_size: The storage_size of this ApplicationDetailResponse.  # noqa: E501
+        :type storage_size: int
+        """
+
+        self._storage_size = storage_size
+
+    @property
+    def data_sources(self):
+        """Gets the data_sources of this ApplicationDetailResponse.  # noqa: E501
+
+        Data sources used by the application  # noqa: E501
+
+        :return: The data_sources of this ApplicationDetailResponse.  # noqa: E501
+        :rtype: list[DataSourceType]
+        """
+        return self._data_sources
+
+    @data_sources.setter
+    def data_sources(self, data_sources):
+        """Sets the data_sources of this ApplicationDetailResponse.
+
+        Data sources used by the application  # noqa: E501
+
+        :param data_sources: The data_sources of this ApplicationDetailResponse.  # noqa: E501
+        :type data_sources: list[DataSourceType]
+        """
+
+        self._data_sources = data_sources
+
+    @property
     def destination_id(self):
         """Gets the destination_id of this ApplicationDetailResponse.  # noqa: E501
 
         Destination identifier  # noqa: E501
 
         :return: The destination_id of this ApplicationDetailResponse.  # noqa: E501
         :rtype: str
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/models/application_query_request.py` & `mantium_spec-1.0.624/mantium_spec/models/application_query_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/models/application_query_response.py` & `mantium_spec-1.0.624/mantium_spec/models/application_query_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/models/application_response.py` & `mantium_spec-1.0.624/mantium_spec/models/application_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
@@ -37,46 +37,61 @@
     """
     openapi_types = {
         'id': 'str',
         'created_at': 'datetime',
         'name': 'str',
         'description': 'str',
         'top_k': 'int',
-        'status': 'ApplicationStatus'
+        'status': 'ApplicationStatus',
+        'last_synced': 'datetime',
+        'storage_size': 'int',
+        'data_sources': 'list[DataSourceType]'
     }
 
     attribute_map = {
         'id': 'id',
         'created_at': 'created_at',
         'name': 'name',
         'description': 'description',
         'top_k': 'top_k',
-        'status': 'status'
+        'status': 'status',
+        'last_synced': 'last_synced',
+        'storage_size': 'storage_size',
+        'data_sources': 'data_sources'
     }
 
-    def __init__(self, id=None, created_at=None, name=None, description=None, top_k=None, status=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, created_at=None, name=None, description=None, top_k=None, status=None, last_synced=None, storage_size=0, data_sources=[], local_vars_configuration=None):  # noqa: E501
         """ApplicationResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._created_at = None
         self._name = None
         self._description = None
         self._top_k = None
         self._status = None
+        self._last_synced = None
+        self._storage_size = None
+        self._data_sources = None
         self.discriminator = None
 
         self.id = id
         self.created_at = created_at
         self.name = name
         self.description = description
         self.top_k = top_k
         self.status = status
+        if last_synced is not None:
+            self.last_synced = last_synced
+        if storage_size is not None:
+            self.storage_size = storage_size
+        if data_sources is not None:
+            self.data_sources = data_sources
 
     @property
     def id(self):
         """Gets the id of this ApplicationResponse.  # noqa: E501
 
         A unique identifier  # noqa: E501
 
@@ -218,14 +233,83 @@
         :type status: ApplicationStatus
         """
         if self.local_vars_configuration.client_side_validation and status is None:  # noqa: E501
             raise ValueError("Invalid value for `status`, must not be `None`")  # noqa: E501
 
         self._status = status
 
+    @property
+    def last_synced(self):
+        """Gets the last_synced of this ApplicationResponse.  # noqa: E501
+
+        The last time a DatasetUpdate job ran for the application  # noqa: E501
+
+        :return: The last_synced of this ApplicationResponse.  # noqa: E501
+        :rtype: datetime
+        """
+        return self._last_synced
+
+    @last_synced.setter
+    def last_synced(self, last_synced):
+        """Sets the last_synced of this ApplicationResponse.
+
+        The last time a DatasetUpdate job ran for the application  # noqa: E501
+
+        :param last_synced: The last_synced of this ApplicationResponse.  # noqa: E501
+        :type last_synced: datetime
+        """
+
+        self._last_synced = last_synced
+
+    @property
+    def storage_size(self):
+        """Gets the storage_size of this ApplicationResponse.  # noqa: E501
+
+        current file storage size for the application  # noqa: E501
+
+        :return: The storage_size of this ApplicationResponse.  # noqa: E501
+        :rtype: int
+        """
+        return self._storage_size
+
+    @storage_size.setter
+    def storage_size(self, storage_size):
+        """Sets the storage_size of this ApplicationResponse.
+
+        current file storage size for the application  # noqa: E501
+
+        :param storage_size: The storage_size of this ApplicationResponse.  # noqa: E501
+        :type storage_size: int
+        """
+
+        self._storage_size = storage_size
+
+    @property
+    def data_sources(self):
+        """Gets the data_sources of this ApplicationResponse.  # noqa: E501
+
+        Data sources used by the application  # noqa: E501
+
+        :return: The data_sources of this ApplicationResponse.  # noqa: E501
+        :rtype: list[DataSourceType]
+        """
+        return self._data_sources
+
+    @data_sources.setter
+    def data_sources(self, data_sources):
+        """Sets the data_sources of this ApplicationResponse.
+
+        Data sources used by the application  # noqa: E501
+
+        :param data_sources: The data_sources of this ApplicationResponse.  # noqa: E501
+        :type data_sources: list[DataSourceType]
+        """
+
+        self._data_sources = data_sources
+
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
                 args = getfullargspec(x.to_dict).args
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/models/application_status.py` & `mantium_spec-1.0.624/mantium_spec/models/application_status.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/models/chat_gpt_plugin_application_detail_response.py` & `mantium_spec-1.0.624/mantium_spec/models/chat_gpt_plugin_application_detail_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
@@ -38,14 +38,17 @@
     openapi_types = {
         'id': 'str',
         'created_at': 'datetime',
         'name': 'str',
         'description': 'str',
         'top_k': 'int',
         'status': 'ApplicationStatus',
+        'last_synced': 'datetime',
+        'storage_size': 'int',
+        'data_sources': 'list[DataSourceType]',
         'destination_id': 'str',
         'embedding_count': 'int',
         'template': 'Template',
         'chatgpt_name': 'str',
         'chatgpt_description': 'str',
         'chatgpt_query_description': 'str',
         'chatgpt_info_description': 'str',
@@ -59,40 +62,46 @@
     attribute_map = {
         'id': 'id',
         'created_at': 'created_at',
         'name': 'name',
         'description': 'description',
         'top_k': 'top_k',
         'status': 'status',
+        'last_synced': 'last_synced',
+        'storage_size': 'storage_size',
+        'data_sources': 'data_sources',
         'destination_id': 'destination_id',
         'embedding_count': 'embedding_count',
         'template': 'template',
         'chatgpt_name': 'chatgpt_name',
         'chatgpt_description': 'chatgpt_description',
         'chatgpt_query_description': 'chatgpt_query_description',
         'chatgpt_info_description': 'chatgpt_info_description',
         'logo_url': 'logo_url',
         'contact_email_address': 'contact_email_address',
         'legal_info_url': 'legal_info_url',
         'access_token': 'access_token',
         'saved_response_enabled': 'saved_response_enabled'
     }
 
-    def __init__(self, id=None, created_at=None, name=None, description=None, top_k=None, status=None, destination_id=None, embedding_count=0, template=None, chatgpt_name=None, chatgpt_description=None, chatgpt_query_description=None, chatgpt_info_description=None, logo_url=None, contact_email_address=None, legal_info_url=None, access_token=None, saved_response_enabled=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, created_at=None, name=None, description=None, top_k=None, status=None, last_synced=None, storage_size=0, data_sources=[], destination_id=None, embedding_count=0, template=None, chatgpt_name=None, chatgpt_description=None, chatgpt_query_description=None, chatgpt_info_description=None, logo_url=None, contact_email_address=None, legal_info_url=None, access_token=None, saved_response_enabled=None, local_vars_configuration=None):  # noqa: E501
         """ChatGPTPluginApplicationDetailResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._created_at = None
         self._name = None
         self._description = None
         self._top_k = None
         self._status = None
+        self._last_synced = None
+        self._storage_size = None
+        self._data_sources = None
         self._destination_id = None
         self._embedding_count = None
         self._template = None
         self._chatgpt_name = None
         self._chatgpt_description = None
         self._chatgpt_query_description = None
         self._chatgpt_info_description = None
@@ -105,14 +114,20 @@
 
         self.id = id
         self.created_at = created_at
         self.name = name
         self.description = description
         self.top_k = top_k
         self.status = status
+        if last_synced is not None:
+            self.last_synced = last_synced
+        if storage_size is not None:
+            self.storage_size = storage_size
+        if data_sources is not None:
+            self.data_sources = data_sources
         if destination_id is not None:
             self.destination_id = destination_id
         if embedding_count is not None:
             self.embedding_count = embedding_count
         if template is not None:
             self.template = template
         if chatgpt_name is not None:
@@ -122,15 +137,16 @@
         if chatgpt_query_description is not None:
             self.chatgpt_query_description = chatgpt_query_description
         if chatgpt_info_description is not None:
             self.chatgpt_info_description = chatgpt_info_description
         self.logo_url = logo_url
         self.contact_email_address = contact_email_address
         self.legal_info_url = legal_info_url
-        self.access_token = access_token
+        if access_token is not None:
+            self.access_token = access_token
         self.saved_response_enabled = saved_response_enabled
 
     @property
     def id(self):
         """Gets the id of this ChatGPTPluginApplicationDetailResponse.  # noqa: E501
 
         A unique identifier  # noqa: E501
@@ -274,14 +290,83 @@
         """
         if self.local_vars_configuration.client_side_validation and status is None:  # noqa: E501
             raise ValueError("Invalid value for `status`, must not be `None`")  # noqa: E501
 
         self._status = status
 
     @property
+    def last_synced(self):
+        """Gets the last_synced of this ChatGPTPluginApplicationDetailResponse.  # noqa: E501
+
+        The last time a DatasetUpdate job ran for the application  # noqa: E501
+
+        :return: The last_synced of this ChatGPTPluginApplicationDetailResponse.  # noqa: E501
+        :rtype: datetime
+        """
+        return self._last_synced
+
+    @last_synced.setter
+    def last_synced(self, last_synced):
+        """Sets the last_synced of this ChatGPTPluginApplicationDetailResponse.
+
+        The last time a DatasetUpdate job ran for the application  # noqa: E501
+
+        :param last_synced: The last_synced of this ChatGPTPluginApplicationDetailResponse.  # noqa: E501
+        :type last_synced: datetime
+        """
+
+        self._last_synced = last_synced
+
+    @property
+    def storage_size(self):
+        """Gets the storage_size of this ChatGPTPluginApplicationDetailResponse.  # noqa: E501
+
+        current file storage size for the application  # noqa: E501
+
+        :return: The storage_size of this ChatGPTPluginApplicationDetailResponse.  # noqa: E501
+        :rtype: int
+        """
+        return self._storage_size
+
+    @storage_size.setter
+    def storage_size(self, storage_size):
+        """Sets the storage_size of this ChatGPTPluginApplicationDetailResponse.
+
+        current file storage size for the application  # noqa: E501
+
+        :param storage_size: The storage_size of this ChatGPTPluginApplicationDetailResponse.  # noqa: E501
+        :type storage_size: int
+        """
+
+        self._storage_size = storage_size
+
+    @property
+    def data_sources(self):
+        """Gets the data_sources of this ChatGPTPluginApplicationDetailResponse.  # noqa: E501
+
+        Data sources used by the application  # noqa: E501
+
+        :return: The data_sources of this ChatGPTPluginApplicationDetailResponse.  # noqa: E501
+        :rtype: list[DataSourceType]
+        """
+        return self._data_sources
+
+    @data_sources.setter
+    def data_sources(self, data_sources):
+        """Sets the data_sources of this ChatGPTPluginApplicationDetailResponse.
+
+        Data sources used by the application  # noqa: E501
+
+        :param data_sources: The data_sources of this ChatGPTPluginApplicationDetailResponse.  # noqa: E501
+        :type data_sources: list[DataSourceType]
+        """
+
+        self._data_sources = data_sources
+
+    @property
     def destination_id(self):
         """Gets the destination_id of this ChatGPTPluginApplicationDetailResponse.  # noqa: E501
 
         Destination identifier  # noqa: E501
 
         :return: The destination_id of this ChatGPTPluginApplicationDetailResponse.  # noqa: E501
         :rtype: str
@@ -530,16 +615,14 @@
         """Sets the access_token of this ChatGPTPluginApplicationDetailResponse.
 
         Access token for the plugin  # noqa: E501
 
         :param access_token: The access_token of this ChatGPTPluginApplicationDetailResponse.  # noqa: E501
         :type access_token: str
         """
-        if self.local_vars_configuration.client_side_validation and access_token is None:  # noqa: E501
-            raise ValueError("Invalid value for `access_token`, must not be `None`")  # noqa: E501
 
         self._access_token = access_token
 
     @property
     def saved_response_enabled(self):
         """Gets the saved_response_enabled of this ChatGPTPluginApplicationDetailResponse.  # noqa: E501
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/models/content_creation_template_options.py` & `mantium_spec-1.0.624/mantium_spec/models/content_creation_template_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/models/content_type.py` & `mantium_spec-1.0.624/mantium_spec/models/content_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/models/credential_type.py` & `mantium_spec-1.0.624/mantium_spec/models/credential_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/models/cursor_datamodel_page_application_response.py` & `mantium_spec-1.0.624/mantium_spec/models/cursor_datamodel_page_application_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/models/custom_template_options.py` & `mantium_spec-1.0.624/mantium_spec/models/custom_template_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/models/customer_support_template_options.py` & `mantium_spec-1.0.624/mantium_spec/models/customer_support_template_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/models/document.py` & `mantium_spec-1.0.624/mantium_spec/models/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/models/document_metadata.py` & `mantium_spec-1.0.624/mantium_spec/models/document_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/models/event_planning_template_options.py` & `mantium_spec-1.0.624/mantium_spec/models/event_planning_template_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/models/http_validation_error.py` & `mantium_spec-1.0.624/mantium_spec/models/http_validation_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/models/legal_documents_template_options.py` & `mantium_spec-1.0.624/mantium_spec/models/legal_documents_template_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/models/location_inner.py` & `mantium_spec-1.0.624/mantium_spec/models/location_inner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/models/meeting_info_template_options.py` & `mantium_spec-1.0.624/mantium_spec/models/meeting_info_template_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/models/personal_knowledge_management_template_options.py` & `mantium_spec-1.0.624/mantium_spec/models/personal_knowledge_management_template_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/models/product_documentation_template_options.py` & `mantium_spec-1.0.624/mantium_spec/models/product_documentation_template_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/models/recipe_management_template_options.py` & `mantium_spec-1.0.624/mantium_spec/models/recipe_management_template_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/models/response_get_application_detail.py` & `mantium_spec-1.0.624/mantium_spec/models/response_get_application_detail.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
@@ -38,14 +38,17 @@
     openapi_types = {
         'id': 'str',
         'created_at': 'datetime',
         'name': 'str',
         'description': 'str',
         'top_k': 'int',
         'status': 'ApplicationStatus',
+        'last_synced': 'datetime',
+        'storage_size': 'int',
+        'data_sources': 'list[DataSourceType]',
         'destination_id': 'str',
         'embedding_count': 'int',
         'template': 'Template',
         'chatgpt_name': 'str',
         'chatgpt_description': 'str',
         'chatgpt_query_description': 'str',
         'chatgpt_info_description': 'str',
@@ -59,40 +62,46 @@
     attribute_map = {
         'id': 'id',
         'created_at': 'created_at',
         'name': 'name',
         'description': 'description',
         'top_k': 'top_k',
         'status': 'status',
+        'last_synced': 'last_synced',
+        'storage_size': 'storage_size',
+        'data_sources': 'data_sources',
         'destination_id': 'destination_id',
         'embedding_count': 'embedding_count',
         'template': 'template',
         'chatgpt_name': 'chatgpt_name',
         'chatgpt_description': 'chatgpt_description',
         'chatgpt_query_description': 'chatgpt_query_description',
         'chatgpt_info_description': 'chatgpt_info_description',
         'logo_url': 'logo_url',
         'contact_email_address': 'contact_email_address',
         'legal_info_url': 'legal_info_url',
         'access_token': 'access_token',
         'saved_response_enabled': 'saved_response_enabled'
     }
 
-    def __init__(self, id=None, created_at=None, name=None, description=None, top_k=None, status=None, destination_id=None, embedding_count=0, template=None, chatgpt_name=None, chatgpt_description=None, chatgpt_query_description=None, chatgpt_info_description=None, logo_url=None, contact_email_address=None, legal_info_url=None, access_token=None, saved_response_enabled=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, created_at=None, name=None, description=None, top_k=None, status=None, last_synced=None, storage_size=0, data_sources=[], destination_id=None, embedding_count=0, template=None, chatgpt_name=None, chatgpt_description=None, chatgpt_query_description=None, chatgpt_info_description=None, logo_url=None, contact_email_address=None, legal_info_url=None, access_token=None, saved_response_enabled=None, local_vars_configuration=None):  # noqa: E501
         """ResponseGetApplicationDetail - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._created_at = None
         self._name = None
         self._description = None
         self._top_k = None
         self._status = None
+        self._last_synced = None
+        self._storage_size = None
+        self._data_sources = None
         self._destination_id = None
         self._embedding_count = None
         self._template = None
         self._chatgpt_name = None
         self._chatgpt_description = None
         self._chatgpt_query_description = None
         self._chatgpt_info_description = None
@@ -105,14 +114,20 @@
 
         self.id = id
         self.created_at = created_at
         self.name = name
         self.description = description
         self.top_k = top_k
         self.status = status
+        if last_synced is not None:
+            self.last_synced = last_synced
+        if storage_size is not None:
+            self.storage_size = storage_size
+        if data_sources is not None:
+            self.data_sources = data_sources
         if destination_id is not None:
             self.destination_id = destination_id
         if embedding_count is not None:
             self.embedding_count = embedding_count
         if template is not None:
             self.template = template
         if chatgpt_name is not None:
@@ -122,15 +137,16 @@
         if chatgpt_query_description is not None:
             self.chatgpt_query_description = chatgpt_query_description
         if chatgpt_info_description is not None:
             self.chatgpt_info_description = chatgpt_info_description
         self.logo_url = logo_url
         self.contact_email_address = contact_email_address
         self.legal_info_url = legal_info_url
-        self.access_token = access_token
+        if access_token is not None:
+            self.access_token = access_token
         self.saved_response_enabled = saved_response_enabled
 
     @property
     def id(self):
         """Gets the id of this ResponseGetApplicationDetail.  # noqa: E501
 
         A unique identifier  # noqa: E501
@@ -274,14 +290,83 @@
         """
         if self.local_vars_configuration.client_side_validation and status is None:  # noqa: E501
             raise ValueError("Invalid value for `status`, must not be `None`")  # noqa: E501
 
         self._status = status
 
     @property
+    def last_synced(self):
+        """Gets the last_synced of this ResponseGetApplicationDetail.  # noqa: E501
+
+        The last time a DatasetUpdate job ran for the application  # noqa: E501
+
+        :return: The last_synced of this ResponseGetApplicationDetail.  # noqa: E501
+        :rtype: datetime
+        """
+        return self._last_synced
+
+    @last_synced.setter
+    def last_synced(self, last_synced):
+        """Sets the last_synced of this ResponseGetApplicationDetail.
+
+        The last time a DatasetUpdate job ran for the application  # noqa: E501
+
+        :param last_synced: The last_synced of this ResponseGetApplicationDetail.  # noqa: E501
+        :type last_synced: datetime
+        """
+
+        self._last_synced = last_synced
+
+    @property
+    def storage_size(self):
+        """Gets the storage_size of this ResponseGetApplicationDetail.  # noqa: E501
+
+        current file storage size for the application  # noqa: E501
+
+        :return: The storage_size of this ResponseGetApplicationDetail.  # noqa: E501
+        :rtype: int
+        """
+        return self._storage_size
+
+    @storage_size.setter
+    def storage_size(self, storage_size):
+        """Sets the storage_size of this ResponseGetApplicationDetail.
+
+        current file storage size for the application  # noqa: E501
+
+        :param storage_size: The storage_size of this ResponseGetApplicationDetail.  # noqa: E501
+        :type storage_size: int
+        """
+
+        self._storage_size = storage_size
+
+    @property
+    def data_sources(self):
+        """Gets the data_sources of this ResponseGetApplicationDetail.  # noqa: E501
+
+        Data sources used by the application  # noqa: E501
+
+        :return: The data_sources of this ResponseGetApplicationDetail.  # noqa: E501
+        :rtype: list[DataSourceType]
+        """
+        return self._data_sources
+
+    @data_sources.setter
+    def data_sources(self, data_sources):
+        """Sets the data_sources of this ResponseGetApplicationDetail.
+
+        Data sources used by the application  # noqa: E501
+
+        :param data_sources: The data_sources of this ResponseGetApplicationDetail.  # noqa: E501
+        :type data_sources: list[DataSourceType]
+        """
+
+        self._data_sources = data_sources
+
+    @property
     def destination_id(self):
         """Gets the destination_id of this ResponseGetApplicationDetail.  # noqa: E501
 
         Destination identifier  # noqa: E501
 
         :return: The destination_id of this ResponseGetApplicationDetail.  # noqa: E501
         :rtype: str
@@ -530,16 +615,14 @@
         """Sets the access_token of this ResponseGetApplicationDetail.
 
         Access token for the plugin  # noqa: E501
 
         :param access_token: The access_token of this ResponseGetApplicationDetail.  # noqa: E501
         :type access_token: str
         """
-        if self.local_vars_configuration.client_side_validation and access_token is None:  # noqa: E501
-            raise ValueError("Invalid value for `access_token`, must not be `None`")  # noqa: E501
 
         self._access_token = access_token
 
     @property
     def saved_response_enabled(self):
         """Gets the saved_response_enabled of this ResponseGetApplicationDetail.  # noqa: E501
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/models/shopify_template_options.py` & `mantium_spec-1.0.624/mantium_spec/models/shopify_template_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/models/span.py` & `mantium_spec-1.0.624/mantium_spec/models/span.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/models/template.py` & `mantium_spec-1.0.624/mantium_spec/models/template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/models/validation_error.py` & `mantium_spec-1.0.624/mantium_spec/models/validation_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
 except ImportError:
```

### Comparing `mantium_spec-1.0.518.post1/mantium_spec/rest.py` & `mantium_spec-1.0.624/mantium_spec/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mantium API
 
     Mantium API Documentation  # noqa: E501
 
-    The version of the OpenAPI document: 1.0.518.post1
+    The version of the OpenAPI document: 1.0.624
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import io
```

### Comparing `mantium_spec-1.0.518.post1/setup.py` & `mantium_spec-1.0.624/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['openapi-client>=1.1.7,<2.0.0']
 
 setup_kwargs = {
     'name': 'mantium-spec',
-    'version': '1.0.518.post1',
+    'version': '1.0.624',
     'description': 'OpenAPI-generated Python client',
-    'long_description': '# mantium-spec\nMantium API Documentation\n\nThis Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:\n\n- API version: 1.0.518.post1\n- Package version: 1.0.0\n- Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen\n\n## Requirements.\n\nPython 2.7 and 3.4+\n\n## Installation & Usage\n### pip install\n\nIf the python package is hosted on a repository, you can install directly using:\n\n```sh\npip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git\n```\n(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)\n\nThen import the package:\n```python\nimport mantium_spec\n```\n\n### Setuptools\n\nInstall via [Setuptools](http://pypi.python.org/pypi/setuptools).\n\n```sh\npython setup.py install --user\n```\n(or `sudo python setup.py install` to install the package for all users)\n\nThen import the package:\n```python\nimport mantium_spec\n```\n\n## Getting Started\n\nPlease follow the [installation procedure](#installation--usage) and then run the following:\n\n```python\nfrom __future__ import print_function\n\nimport time\nimport mantium_spec\nfrom mantium_spec.rest import ApiException\nfrom pprint import pprint\n\n# Defining the host is optional and defaults to http://localhost\n# See configuration.py for a list of all supported configuration parameters.\nconfiguration = mantium_spec.Configuration(\n    host = "http://localhost"\n)\n\n# The client must configure the authentication and authorization parameters\n# in accordance with the API server security policy.\n# Examples for each auth method are provided below, use the example that\n# satisfies your auth use case.\n\n# Configure Bearer authorization: HTTPBearer\nconfiguration = mantium_spec.Configuration(\n    access_token = \'YOUR_BEARER_TOKEN\'\n)\n\n\n# Enter a context with an instance of the API client\nwith mantium_spec.ApiClient(configuration) as api_client:\n    # Create an instance of the API class\n    api_instance = mantium_spec.ApplicationsApi(api_client)\n    application_id = \'application_id_example\' # str | \nbody = None # object |  (optional)\n\n    try:\n        # Get application detail.\n        api_response = api_instance.get_application_detail(application_id, body=body)\n        pprint(api_response)\n    except ApiException as e:\n        print("Exception when calling ApplicationsApi->get_application_detail: %s\\n" % e)\n    \n```\n\n## Documentation for API Endpoints\n\nAll URIs are relative to *http://localhost*\n\nClass | Method | HTTP request | Description\n------------ | ------------- | ------------- | -------------\n*ApplicationsApi* | [**get_application_detail**](docs/ApplicationsApi.md#get_application_detail) | **GET** /applications/{application_id} | Get application detail.\n*ApplicationsApi* | [**list_applications**](docs/ApplicationsApi.md#list_applications) | **GET** /applications/ | List applications.\n*ApplicationsApi* | [**query_application**](docs/ApplicationsApi.md#query_application) | **POST** /applications/{application_id}/query | Interact with an application.\n\n\n## Documentation For Models\n\n - [Answer](docs/Answer.md)\n - [AnswerMeta](docs/AnswerMeta.md)\n - [ApplicationCredential](docs/ApplicationCredential.md)\n - [ApplicationDetailResponse](docs/ApplicationDetailResponse.md)\n - [ApplicationQueryRequest](docs/ApplicationQueryRequest.md)\n - [ApplicationQueryResponse](docs/ApplicationQueryResponse.md)\n - [ApplicationResponse](docs/ApplicationResponse.md)\n - [ApplicationStatus](docs/ApplicationStatus.md)\n - [ChatGPTPluginApplicationDetailResponse](docs/ChatGPTPluginApplicationDetailResponse.md)\n - [ContentCreationTemplateOptions](docs/ContentCreationTemplateOptions.md)\n - [ContentType](docs/ContentType.md)\n - [CredentialType](docs/CredentialType.md)\n - [CursorDatamodelPageApplicationResponse](docs/CursorDatamodelPageApplicationResponse.md)\n - [CustomTemplateOptions](docs/CustomTemplateOptions.md)\n - [CustomerSupportTemplateOptions](docs/CustomerSupportTemplateOptions.md)\n - [Document](docs/Document.md)\n - [DocumentMetadata](docs/DocumentMetadata.md)\n - [EventPlanningTemplateOptions](docs/EventPlanningTemplateOptions.md)\n - [HTTPValidationError](docs/HTTPValidationError.md)\n - [LegalDocumentsTemplateOptions](docs/LegalDocumentsTemplateOptions.md)\n - [LocationInner](docs/LocationInner.md)\n - [MeetingInfoTemplateOptions](docs/MeetingInfoTemplateOptions.md)\n - [PersonalKnowledgeManagementTemplateOptions](docs/PersonalKnowledgeManagementTemplateOptions.md)\n - [ProductDocumentationTemplateOptions](docs/ProductDocumentationTemplateOptions.md)\n - [RecipeManagementTemplateOptions](docs/RecipeManagementTemplateOptions.md)\n - [ResponseGetApplicationDetail](docs/ResponseGetApplicationDetail.md)\n - [ShopifyTemplateOptions](docs/ShopifyTemplateOptions.md)\n - [Span](docs/Span.md)\n - [Template](docs/Template.md)\n - [ValidationError](docs/ValidationError.md)\n\n\n## Documentation For Authorization\n\n\n## HTTPBearer\n\n- **Type**: Bearer authentication\n\n\n## Author\n\n\n\n\n',
+    'long_description': '# mantium-spec\nMantium API Documentation\n\nThis Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:\n\n- API version: 1.0.624\n- Package version: 1.0.0\n- Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen\n\n## Requirements.\n\nPython 2.7 and 3.4+\n\n## Installation & Usage\n### pip install\n\nIf the python package is hosted on a repository, you can install directly using:\n\n```sh\npip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git\n```\n(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)\n\nThen import the package:\n```python\nimport mantium_spec\n```\n\n### Setuptools\n\nInstall via [Setuptools](http://pypi.python.org/pypi/setuptools).\n\n```sh\npython setup.py install --user\n```\n(or `sudo python setup.py install` to install the package for all users)\n\nThen import the package:\n```python\nimport mantium_spec\n```\n\n## Getting Started\n\nPlease follow the [installation procedure](#installation--usage) and then run the following:\n\n```python\nfrom __future__ import print_function\n\nimport time\nimport mantium_spec\nfrom mantium_spec.rest import ApiException\nfrom pprint import pprint\n\n# Defining the host is optional and defaults to http://localhost\n# See configuration.py for a list of all supported configuration parameters.\nconfiguration = mantium_spec.Configuration(\n    host = "http://localhost"\n)\n\n# The client must configure the authentication and authorization parameters\n# in accordance with the API server security policy.\n# Examples for each auth method are provided below, use the example that\n# satisfies your auth use case.\n\n# Configure Bearer authorization: HTTPBearer\nconfiguration = mantium_spec.Configuration(\n    access_token = \'YOUR_BEARER_TOKEN\'\n)\n\n\n# Enter a context with an instance of the API client\nwith mantium_spec.ApiClient(configuration) as api_client:\n    # Create an instance of the API class\n    api_instance = mantium_spec.ApplicationsApi(api_client)\n    application_id = \'application_id_example\' # str | \nbody = None # object |  (optional)\n\n    try:\n        # Get application detail.\n        api_response = api_instance.get_application_detail(application_id, body=body)\n        pprint(api_response)\n    except ApiException as e:\n        print("Exception when calling ApplicationsApi->get_application_detail: %s\\n" % e)\n    \n```\n\n## Documentation for API Endpoints\n\nAll URIs are relative to *http://localhost*\n\nClass | Method | HTTP request | Description\n------------ | ------------- | ------------- | -------------\n*ApplicationsApi* | [**get_application_detail**](docs/ApplicationsApi.md#get_application_detail) | **GET** /applications/{application_id} | Get application detail.\n*ApplicationsApi* | [**list_applications**](docs/ApplicationsApi.md#list_applications) | **GET** /applications/ | List applications.\n*ApplicationsApi* | [**query_application**](docs/ApplicationsApi.md#query_application) | **POST** /applications/{application_id}/query | Interact with an application.\n\n\n## Documentation For Models\n\n - [Answer](docs/Answer.md)\n - [AnswerMeta](docs/AnswerMeta.md)\n - [ApplicationCredential](docs/ApplicationCredential.md)\n - [ApplicationDetailResponse](docs/ApplicationDetailResponse.md)\n - [ApplicationQueryRequest](docs/ApplicationQueryRequest.md)\n - [ApplicationQueryResponse](docs/ApplicationQueryResponse.md)\n - [ApplicationResponse](docs/ApplicationResponse.md)\n - [ApplicationStatus](docs/ApplicationStatus.md)\n - [ChatGPTPluginApplicationDetailResponse](docs/ChatGPTPluginApplicationDetailResponse.md)\n - [ContentCreationTemplateOptions](docs/ContentCreationTemplateOptions.md)\n - [ContentType](docs/ContentType.md)\n - [CredentialType](docs/CredentialType.md)\n - [CursorDatamodelPageApplicationResponse](docs/CursorDatamodelPageApplicationResponse.md)\n - [CustomTemplateOptions](docs/CustomTemplateOptions.md)\n - [CustomerSupportTemplateOptions](docs/CustomerSupportTemplateOptions.md)\n - [DataSourceType](docs/DataSourceType.md)\n - [Document](docs/Document.md)\n - [DocumentMetadata](docs/DocumentMetadata.md)\n - [EventPlanningTemplateOptions](docs/EventPlanningTemplateOptions.md)\n - [HTTPValidationError](docs/HTTPValidationError.md)\n - [LegalDocumentsTemplateOptions](docs/LegalDocumentsTemplateOptions.md)\n - [LocationInner](docs/LocationInner.md)\n - [MeetingInfoTemplateOptions](docs/MeetingInfoTemplateOptions.md)\n - [PersonalKnowledgeManagementTemplateOptions](docs/PersonalKnowledgeManagementTemplateOptions.md)\n - [ProductDocumentationTemplateOptions](docs/ProductDocumentationTemplateOptions.md)\n - [RecipeManagementTemplateOptions](docs/RecipeManagementTemplateOptions.md)\n - [ResponseGetApplicationDetail](docs/ResponseGetApplicationDetail.md)\n - [ShopifyTemplateOptions](docs/ShopifyTemplateOptions.md)\n - [Span](docs/Span.md)\n - [Template](docs/Template.md)\n - [ValidationError](docs/ValidationError.md)\n\n\n## Documentation For Authorization\n\n\n## HTTPBearer\n\n- **Type**: Bearer authentication\n\n\n## Author\n\n\n\n\n',
     'author': 'Mantium',
     'author_email': 'support@mantiumai.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `mantium_spec-1.0.518.post1/PKG-INFO` & `mantium_spec-1.0.624/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mantium-spec
-Version: 1.0.518.post1
+Version: 1.0.624
 Summary: OpenAPI-generated Python client
 Author: Mantium
 Author-email: support@mantiumai.com
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -15,15 +15,15 @@
 Description-Content-Type: text/markdown
 
 # mantium-spec
 Mantium API Documentation
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.0.518.post1
+- API version: 1.0.624
 - Package version: 1.0.0
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
@@ -125,14 +125,15 @@
  - [ChatGPTPluginApplicationDetailResponse](docs/ChatGPTPluginApplicationDetailResponse.md)
  - [ContentCreationTemplateOptions](docs/ContentCreationTemplateOptions.md)
  - [ContentType](docs/ContentType.md)
  - [CredentialType](docs/CredentialType.md)
  - [CursorDatamodelPageApplicationResponse](docs/CursorDatamodelPageApplicationResponse.md)
  - [CustomTemplateOptions](docs/CustomTemplateOptions.md)
  - [CustomerSupportTemplateOptions](docs/CustomerSupportTemplateOptions.md)
+ - [DataSourceType](docs/DataSourceType.md)
  - [Document](docs/Document.md)
  - [DocumentMetadata](docs/DocumentMetadata.md)
  - [EventPlanningTemplateOptions](docs/EventPlanningTemplateOptions.md)
  - [HTTPValidationError](docs/HTTPValidationError.md)
  - [LegalDocumentsTemplateOptions](docs/LegalDocumentsTemplateOptions.md)
  - [LocationInner](docs/LocationInner.md)
  - [MeetingInfoTemplateOptions](docs/MeetingInfoTemplateOptions.md)
```

