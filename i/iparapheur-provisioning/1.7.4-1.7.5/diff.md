# Comparing `tmp/iparapheur-provisioning-1.7.4.tar.gz` & `tmp/iparapheur-provisioning-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iparapheur-provisioning-1.7.4.tar", last modified: Mon Aug  7 13:53:21 2023, max compression
+gzip compressed data, was "iparapheur-provisioning-1.7.5.tar", last modified: Tue Aug  8 14:52:03 2023, max compression
```

## Comparing `iparapheur-provisioning-1.7.4.tar` & `iparapheur-provisioning-1.7.5.tar`

### file list

```diff
@@ -1,332 +1,332 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.860828 iparapheur-provisioning-1.7.4/
--rw-r--r--   0 root         (0) root         (0)     1111 2023-08-07 13:53:03.000000 iparapheur-provisioning-1.7.4/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      421 2023-08-07 13:53:21.864828 iparapheur-provisioning-1.7.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    21776 2023-08-07 13:53:02.000000 iparapheur-provisioning-1.7.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.796826 iparapheur-provisioning-1.7.4/iparapheur_provisioning/
--rw-r--r--   0 root         (0) root         (0)      907 2023-08-07 13:53:02.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58620 2023-08-07 13:53:02.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.808827 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/
--rw-r--r--   0 root         (0) root         (0)      214 2023-08-07 13:53:03.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8048 2023-08-07 13:53:02.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/path_to_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.808827 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/paths/
--rw-r--r--   0 root         (0) root         (0)      250 2023-08-07 13:53:02.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/paths/__init__.py
--rw-r--r--   0 root         (0) root         (0)      261 2023-08-07 13:52:56.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-08-07 13:52:56.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id.py
--rw-r--r--   0 root         (0) root         (0)      303 2023-08-07 13:52:51.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-08-07 13:52:51.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id.py
--rw-r--r--   0 root         (0) root         (0)      315 2023-08-07 13:52:53.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata.py
--rw-r--r--   0 root         (0) root         (0)      490 2023-08-07 13:52:53.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id.py
--rw-r--r--   0 root         (0) root         (0)      338 2023-08-07 13:52:54.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate.py
--rw-r--r--   0 root         (0) root         (0)      552 2023-08-07 13:52:54.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id.py
--rw-r--r--   0 root         (0) root         (0)      643 2023-08-07 13:52:55.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type.py
--rw-r--r--   0 root         (0) root         (0)      329 2023-08-07 13:53:01.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type.py
--rw-r--r--   0 root         (0) root         (0)      493 2023-08-07 13:53:01.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id.py
--rw-r--r--   0 root         (0) root         (0)      374 2023-08-07 13:53:01.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype.py
--rw-r--r--   0 root         (0) root         (0)      566 2023-08-07 13:53:01.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py
--rw-r--r--   0 root         (0) root         (0)      303 2023-08-07 13:52:58.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-08-07 13:52:58.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id.py
--rw-r--r--   0 root         (0) root         (0)      210 2023-08-07 13:53:02.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition.py
--rw-r--r--   0 root         (0) root         (0)      264 2023-08-07 13:53:02.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key.py
--rw-r--r--   0 root         (0) root         (0)      150 2023-08-07 13:52:50.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user.py
--rw-r--r--   0 root         (0) root         (0)      393 2023-08-07 13:52:50.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user_user_id.py
--rw-r--r--   0 root         (0) root         (0)     1929 2023-08-07 13:53:02.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/tag_to_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.812826 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/tags/
--rw-r--r--   0 root         (0) root         (0)      659 2023-08-07 13:53:02.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/tags/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1031 2023-08-07 13:52:50.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/tags/admin_all_users_api.py
--rw-r--r--   0 root         (0) root         (0)     1131 2023-08-07 13:52:51.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/tags/admin_desk_api.py
--rw-r--r--   0 root         (0) root         (0)     1195 2023-08-07 13:52:53.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/tags/admin_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)     1336 2023-08-07 13:52:54.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/tags/admin_seal_certificate_api.py
--rw-r--r--   0 root         (0) root         (0)     1138 2023-08-07 13:52:55.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/tags/admin_template_api.py
--rw-r--r--   0 root         (0) root         (0)     1074 2023-08-07 13:52:56.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/tags/admin_tenant_api.py
--rw-r--r--   0 root         (0) root         (0)     1139 2023-08-07 13:52:58.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py
--rw-r--r--   0 root         (0) root         (0)     1959 2023-08-07 13:53:01.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/tags/admin_typology_api.py
--rw-r--r--   0 root         (0) root         (0)      863 2023-08-07 13:53:02.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/tags/admin_workflow_definition_api.py
--rw-r--r--   0 root         (0) root         (0)    15677 2023-08-07 13:53:02.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/configuration.py
--rw-r--r--   0 root         (0) root         (0)     4598 2023-08-07 13:53:02.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.820827 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/
--rw-r--r--   0 root         (0) root         (0)      357 2023-08-07 13:53:03.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6643 2023-08-07 13:52:42.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/certificate_informations.py
--rw-r--r--   0 root         (0) root         (0)     1426 2023-08-07 13:52:42.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/delegation_sort_by.py
--rw-r--r--   0 root         (0) root         (0)    24041 2023-08-07 13:52:43.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/desk_dto.py
--rw-r--r--   0 root         (0) root         (0)     3809 2023-08-07 13:52:43.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/desk_representation.py
--rw-r--r--   0 root         (0) root         (0)     4553 2023-08-07 13:52:44.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/error_response.py
--rw-r--r--   0 root         (0) root         (0)     4971 2023-08-07 13:52:44.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/external_signature_config_representation.py
--rw-r--r--   0 root         (0) root         (0)     1399 2023-08-07 13:52:44.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/external_signature_config_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1455 2023-08-07 13:52:44.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/external_signature_provider.py
--rw-r--r--   0 root         (0) root         (0)     2680 2023-08-07 13:52:44.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/folder_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     2656 2023-08-07 13:52:44.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/internal_metadata.py
--rw-r--r--   0 root         (0) root         (0)     3284 2023-08-07 13:52:44.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/layer_representation.py
--rw-r--r--   0 root         (0) root         (0)     1141 2023-08-07 13:52:44.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/layer_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     7908 2023-08-07 13:52:44.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)     5805 2023-08-07 13:52:44.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/metadata_representation.py
--rw-r--r--   0 root         (0) root         (0)     1356 2023-08-07 13:52:44.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/metadata_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1598 2023-08-07 13:52:44.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/metadata_type.py
--rw-r--r--   0 root         (0) root         (0)     9105 2023-08-07 13:52:45.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/page_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)     9141 2023-08-07 13:52:45.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/page_metadata_representation.py
--rw-r--r--   0 root         (0) root         (0)     9205 2023-08-07 13:52:45.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/page_seal_certificate_representation.py
--rw-r--r--   0 root         (0) root         (0)     9132 2023-08-07 13:52:45.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/page_subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)     9123 2023-08-07 13:52:45.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/page_tenant_representation.py
--rw-r--r--   0 root         (0) root         (0)     9105 2023-08-07 13:52:45.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/page_type_representation.py
--rw-r--r--   0 root         (0) root         (0)     9105 2023-08-07 13:52:46.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/page_user_representation.py
--rw-r--r--   0 root         (0) root         (0)     9232 2023-08-07 13:52:46.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/page_workflow_definition_representation.py
--rw-r--r--   0 root         (0) root         (0)     5251 2023-08-07 13:52:46.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/pageable_object.py
--rw-r--r--   0 root         (0) root         (0)     3524 2023-08-07 13:52:46.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/pdf_signature_position.py
--rw-r--r--   0 root         (0) root         (0)     8300 2023-08-07 13:52:46.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/seal_certificate_dto.py
--rw-r--r--   0 root         (0) root         (0)     4500 2023-08-07 13:52:46.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/seal_certificate_representation.py
--rw-r--r--   0 root         (0) root         (0)     1301 2023-08-07 13:52:46.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/seal_certificate_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1527 2023-08-07 13:52:46.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/signature_format.py
--rw-r--r--   0 root         (0) root         (0)     1273 2023-08-07 13:52:46.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/signature_protocol.py
--rw-r--r--   0 root         (0) root         (0)     3524 2023-08-07 13:52:46.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/sort_object.py
--rw-r--r--   0 root         (0) root         (0)    29448 2023-08-07 13:52:47.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/subtype_dto.py
--rw-r--r--   0 root         (0) root         (0)     1307 2023-08-07 13:52:47.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/subtype_layer_association.py
--rw-r--r--   0 root         (0) root         (0)     3930 2023-08-07 13:52:47.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/subtype_layer_dto.py
--rw-r--r--   0 root         (0) root         (0)     5468 2023-08-07 13:52:47.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/subtype_metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)     3288 2023-08-07 13:52:47.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)     3082 2023-08-07 13:52:47.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/template_type.py
--rw-r--r--   0 root         (0) root         (0)     3274 2023-08-07 13:52:47.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/tenant_dto.py
--rw-r--r--   0 root         (0) root         (0)     3286 2023-08-07 13:52:48.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/tenant_representation.py
--rw-r--r--   0 root         (0) root         (0)     1142 2023-08-07 13:52:48.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/tenant_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     9365 2023-08-07 13:52:48.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/type_dto.py
--rw-r--r--   0 root         (0) root         (0)     4044 2023-08-07 13:52:48.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/type_representation.py
--rw-r--r--   0 root         (0) root         (0)     1144 2023-08-07 13:52:48.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/typology_sort_by.py
--rw-r--r--   0 root         (0) root         (0)    29666 2023-08-07 13:52:48.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/user_dto.py
--rw-r--r--   0 root         (0) root         (0)     1471 2023-08-07 13:52:49.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/user_privilege.py
--rw-r--r--   0 root         (0) root         (0)     6504 2023-08-07 13:52:49.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/user_representation.py
--rw-r--r--   0 root         (0) root         (0)     1522 2023-08-07 13:52:49.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/user_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     4499 2023-08-07 13:52:49.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/workflow_definition_representation.py
--rw-r--r--   0 root         (0) root         (0)     1256 2023-08-07 13:52:49.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/workflow_definition_sort_by.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.820827 iparapheur-provisioning-1.7.4/iparapheur_provisioning/models/
--rw-r--r--   0 root         (0) root         (0)     4525 2023-08-07 13:53:03.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.820827 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/
--rw-r--r--   0 root         (0) root         (0)     2703 2023-08-07 13:53:02.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.820827 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/
--rw-r--r--   0 root         (0) root         (0)      369 2023-08-07 13:52:56.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13070 2023-08-07 13:52:56.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/get.py
--rw-r--r--   0 root         (0) root         (0)    13629 2023-08-07 13:52:55.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.820827 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/
--rw-r--r--   0 root         (0) root         (0)      389 2023-08-07 13:52:56.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11083 2023-08-07 13:52:56.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11332 2023-08-07 13:52:56.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py
--rw-r--r--   0 root         (0) root         (0)    15808 2023-08-07 13:52:56.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.824827 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/
--rw-r--r--   0 root         (0) root         (0)      399 2023-08-07 13:52:51.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15034 2023-08-07 13:52:51.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py
--rw-r--r--   0 root         (0) root         (0)    16302 2023-08-07 13:52:50.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.824827 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
--rw-r--r--   0 root         (0) root         (0)      415 2023-08-07 13:52:51.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11337 2023-08-07 13:52:50.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11677 2023-08-07 13:52:51.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py
--rw-r--r--   0 root         (0) root         (0)    16545 2023-08-07 13:52:51.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.824827 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/
--rw-r--r--   0 root         (0) root         (0)      407 2023-08-07 13:52:53.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15486 2023-08-07 13:52:52.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/get.py
--rw-r--r--   0 root         (0) root         (0)    16907 2023-08-07 13:52:52.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.824827 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/
--rw-r--r--   0 root         (0) root         (0)      431 2023-08-07 13:52:53.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11413 2023-08-07 13:52:52.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11668 2023-08-07 13:52:52.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/get.py
--rw-r--r--   0 root         (0) root         (0)    16979 2023-08-07 13:52:53.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.824827 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/
--rw-r--r--   0 root         (0) root         (0)      423 2023-08-07 13:52:54.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14894 2023-08-07 13:52:54.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/get.py
--rw-r--r--   0 root         (0) root         (0)    19934 2023-08-07 13:52:53.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.824827 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/
--rw-r--r--   0 root         (0) root         (0)      463 2023-08-07 13:52:54.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12091 2023-08-07 13:52:53.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    12371 2023-08-07 13:52:53.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/get.py
--rw-r--r--   0 root         (0) root         (0)    20252 2023-08-07 13:52:54.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.828827 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/
--rw-r--r--   0 root         (0) root         (0)      437 2023-08-07 13:52:55.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11569 2023-08-07 13:52:55.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/delete.py
--rw-r--r--   0 root         (0) root         (0)    11613 2023-08-07 13:52:55.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/get.py
--rw-r--r--   0 root         (0) root         (0)    15581 2023-08-07 13:52:54.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/post.py
--rw-r--r--   0 root         (0) root         (0)    15574 2023-08-07 13:52:55.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.828827 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/
--rw-r--r--   0 root         (0) root         (0)      417 2023-08-07 13:53:01.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14728 2023-08-07 13:53:00.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py
--rw-r--r--   0 root         (0) root         (0)    15777 2023-08-07 13:52:58.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.828827 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
--rw-r--r--   0 root         (0) root         (0)      433 2023-08-07 13:53:01.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11337 2023-08-07 13:52:59.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11590 2023-08-07 13:52:59.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py
--rw-r--r--   0 root         (0) root         (0)    15521 2023-08-07 13:53:01.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.836827 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
--rw-r--r--   0 root         (0) root         (0)      449 2023-08-07 13:53:01.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15050 2023-08-07 13:53:00.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py
--rw-r--r--   0 root         (0) root         (0)    16640 2023-08-07 13:52:58.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.836827 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
--rw-r--r--   0 root         (0) root         (0)      471 2023-08-07 13:53:01.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11672 2023-08-07 13:52:59.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11934 2023-08-07 13:52:59.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py
--rw-r--r--   0 root         (0) root         (0)    16645 2023-08-07 13:53:00.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.836827 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/
--rw-r--r--   0 root         (0) root         (0)      399 2023-08-07 13:52:58.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15944 2023-08-07 13:52:57.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py
--rw-r--r--   0 root         (0) root         (0)    16306 2023-08-07 13:52:57.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.840827 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
--rw-r--r--   0 root         (0) root         (0)      415 2023-08-07 13:52:58.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11932 2023-08-07 13:52:57.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11580 2023-08-07 13:52:57.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py
--rw-r--r--   0 root         (0) root         (0)    16046 2023-08-07 13:52:58.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.840827 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/
--rw-r--r--   0 root         (0) root         (0)      429 2023-08-07 13:53:02.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15256 2023-08-07 13:53:02.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.840827 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/
--rw-r--r--   0 root         (0) root         (0)      477 2023-08-07 13:53:02.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11623 2023-08-07 13:53:02.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/delete.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.840827 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/
--rw-r--r--   0 root         (0) root         (0)      365 2023-08-07 13:52:50.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13222 2023-08-07 13:52:50.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.840827 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/
--rw-r--r--   0 root         (0) root         (0)      381 2023-08-07 13:52:50.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11207 2023-08-07 13:52:49.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11978 2023-08-07 13:52:49.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py
--rw-r--r--   0 root         (0) root         (0)    15946 2023-08-07 13:52:50.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py
--rw-r--r--   0 root         (0) root         (0)    10635 2023-08-07 13:53:02.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/rest.py
--rw-r--r--   0 root         (0) root         (0)    97752 2023-08-07 13:53:03.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.800826 iparapheur-provisioning-1.7.4/iparapheur_provisioning.egg-info/
--rw-r--r--   0 root         (0) root         (0)      421 2023-08-07 13:53:21.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    20426 2023-08-07 13:53:21.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-07 13:53:21.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      118 2023-08-07 13:53:21.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-08-07 13:53:21.000000 iparapheur-provisioning-1.7.4/iparapheur_provisioning.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-08-07 13:53:21.864828 iparapheur-provisioning-1.7.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1322 2023-08-07 13:53:02.000000 iparapheur-provisioning-1.7.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.796826 iparapheur-provisioning-1.7.4/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.852827 iparapheur-provisioning-1.7.4/test/test_models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 13:53:02.000000 iparapheur-provisioning-1.7.4/test/test_models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      709 2023-08-07 13:52:42.000000 iparapheur-provisioning-1.7.4/test/test_models/test_certificate_informations.py
--rw-r--r--   0 root         (0) root         (0)      682 2023-08-07 13:52:42.000000 iparapheur-provisioning-1.7.4/test/test_models/test_delegation_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      645 2023-08-07 13:52:43.000000 iparapheur-provisioning-1.7.4/test/test_models/test_desk_dto.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-08-07 13:52:43.000000 iparapheur-provisioning-1.7.4/test/test_models/test_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-08-07 13:52:44.000000 iparapheur-provisioning-1.7.4/test/test_models/test_error_response.py
--rw-r--r--   0 root         (0) root         (0)      767 2023-08-07 13:52:44.000000 iparapheur-provisioning-1.7.4/test/test_models/test_external_signature_config_representation.py
--rw-r--r--   0 root         (0) root         (0)      736 2023-08-07 13:52:44.000000 iparapheur-provisioning-1.7.4/test/test_models/test_external_signature_config_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      718 2023-08-07 13:52:44.000000 iparapheur-provisioning-1.7.4/test/test_models/test_external_signature_provider.py
--rw-r--r--   0 root         (0) root         (0)      666 2023-08-07 13:52:44.000000 iparapheur-provisioning-1.7.4/test/test_models/test_folder_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      681 2023-08-07 13:52:44.000000 iparapheur-provisioning-1.7.4/test/test_models/test_internal_metadata.py
--rw-r--r--   0 root         (0) root         (0)      693 2023-08-07 13:52:44.000000 iparapheur-provisioning-1.7.4/test/test_models/test_layer_representation.py
--rw-r--r--   0 root         (0) root         (0)      662 2023-08-07 13:52:44.000000 iparapheur-provisioning-1.7.4/test/test_models/test_layer_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      661 2023-08-07 13:52:44.000000 iparapheur-provisioning-1.7.4/test/test_models/test_metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)      705 2023-08-07 13:52:44.000000 iparapheur-provisioning-1.7.4/test/test_models/test_metadata_representation.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-08-07 13:52:44.000000 iparapheur-provisioning-1.7.4/test/test_models/test_metadata_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      665 2023-08-07 13:52:44.000000 iparapheur-provisioning-1.7.4/test/test_models/test_metadata_type.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-08-07 13:52:45.000000 iparapheur-provisioning-1.7.4/test/test_models/test_page_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)      722 2023-08-07 13:52:45.000000 iparapheur-provisioning-1.7.4/test/test_models/test_page_metadata_representation.py
--rw-r--r--   0 root         (0) root         (0)      751 2023-08-07 13:52:45.000000 iparapheur-provisioning-1.7.4/test/test_models/test_page_seal_certificate_representation.py
--rw-r--r--   0 root         (0) root         (0)      718 2023-08-07 13:52:45.000000 iparapheur-provisioning-1.7.4/test/test_models/test_page_subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)      714 2023-08-07 13:52:45.000000 iparapheur-provisioning-1.7.4/test/test_models/test_page_tenant_representation.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-08-07 13:52:45.000000 iparapheur-provisioning-1.7.4/test/test_models/test_page_type_representation.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-08-07 13:52:46.000000 iparapheur-provisioning-1.7.4/test/test_models/test_page_user_representation.py
--rw-r--r--   0 root         (0) root         (0)      763 2023-08-07 13:52:46.000000 iparapheur-provisioning-1.7.4/test/test_models/test_page_workflow_definition_representation.py
--rw-r--r--   0 root         (0) root         (0)      673 2023-08-07 13:52:46.000000 iparapheur-provisioning-1.7.4/test/test_models/test_pageable_object.py
--rw-r--r--   0 root         (0) root         (0)      698 2023-08-07 13:52:46.000000 iparapheur-provisioning-1.7.4/test/test_models/test_pdf_signature_position.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-08-07 13:52:46.000000 iparapheur-provisioning-1.7.4/test/test_models/test_seal_certificate_dto.py
--rw-r--r--   0 root         (0) root         (0)      734 2023-08-07 13:52:46.000000 iparapheur-provisioning-1.7.4/test/test_models/test_seal_certificate_representation.py
--rw-r--r--   0 root         (0) root         (0)      703 2023-08-07 13:52:46.000000 iparapheur-provisioning-1.7.4/test/test_models/test_seal_certificate_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      677 2023-08-07 13:52:46.000000 iparapheur-provisioning-1.7.4/test/test_models/test_signature_format.py
--rw-r--r--   0 root         (0) root         (0)      685 2023-08-07 13:52:46.000000 iparapheur-provisioning-1.7.4/test/test_models/test_signature_protocol.py
--rw-r--r--   0 root         (0) root         (0)      657 2023-08-07 13:52:46.000000 iparapheur-provisioning-1.7.4/test/test_models/test_sort_object.py
--rw-r--r--   0 root         (0) root         (0)      657 2023-08-07 13:52:47.000000 iparapheur-provisioning-1.7.4/test/test_models/test_subtype_dto.py
--rw-r--r--   0 root         (0) root         (0)      710 2023-08-07 13:52:47.000000 iparapheur-provisioning-1.7.4/test/test_models/test_subtype_layer_association.py
--rw-r--r--   0 root         (0) root         (0)      678 2023-08-07 13:52:47.000000 iparapheur-provisioning-1.7.4/test/test_models/test_subtype_layer_dto.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-08-07 13:52:47.000000 iparapheur-provisioning-1.7.4/test/test_models/test_subtype_metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)      701 2023-08-07 13:52:47.000000 iparapheur-provisioning-1.7.4/test/test_models/test_subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)      665 2023-08-07 13:52:47.000000 iparapheur-provisioning-1.7.4/test/test_models/test_template_type.py
--rw-r--r--   0 root         (0) root         (0)      653 2023-08-07 13:52:47.000000 iparapheur-provisioning-1.7.4/test/test_models/test_tenant_dto.py
--rw-r--r--   0 root         (0) root         (0)      697 2023-08-07 13:52:48.000000 iparapheur-provisioning-1.7.4/test/test_models/test_tenant_representation.py
--rw-r--r--   0 root         (0) root         (0)      666 2023-08-07 13:52:48.000000 iparapheur-provisioning-1.7.4/test/test_models/test_tenant_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      645 2023-08-07 13:52:48.000000 iparapheur-provisioning-1.7.4/test/test_models/test_type_dto.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-08-07 13:52:48.000000 iparapheur-provisioning-1.7.4/test/test_models/test_type_representation.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-08-07 13:52:48.000000 iparapheur-provisioning-1.7.4/test/test_models/test_typology_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      645 2023-08-07 13:52:48.000000 iparapheur-provisioning-1.7.4/test/test_models/test_user_dto.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-08-07 13:52:49.000000 iparapheur-provisioning-1.7.4/test/test_models/test_user_privilege.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-08-07 13:52:49.000000 iparapheur-provisioning-1.7.4/test/test_models/test_user_representation.py
--rw-r--r--   0 root         (0) root         (0)      658 2023-08-07 13:52:49.000000 iparapheur-provisioning-1.7.4/test/test_models/test_user_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      746 2023-08-07 13:52:49.000000 iparapheur-provisioning-1.7.4/test/test_models/test_workflow_definition_representation.py
--rw-r--r--   0 root         (0) root         (0)      715 2023-08-07 13:52:49.000000 iparapheur-provisioning-1.7.4/test/test_models/test_workflow_definition_sort_by.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.852827 iparapheur-provisioning-1.7.4/test/test_paths/
--rw-r--r--   0 root         (0) root         (0)     1995 2023-08-07 13:53:02.000000 iparapheur-provisioning-1.7.4/test/test_paths/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.852827 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 13:52:56.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant/__init__.py
--rw-r--r--   0 root         (0) root         (0)      887 2023-08-07 13:52:56.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant/test_get.py
--rw-r--r--   0 root         (0) root         (0)      899 2023-08-07 13:52:56.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.852827 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 13:52:56.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)      946 2023-08-07 13:52:56.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      930 2023-08-07 13:52:56.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      916 2023-08-07 13:52:56.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.852827 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 13:52:51.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
--rw-r--r--   0 root         (0) root         (0)      924 2023-08-07 13:52:51.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py
--rw-r--r--   0 root         (0) root         (0)      932 2023-08-07 13:52:51.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.852827 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 13:52:51.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)      977 2023-08-07 13:52:51.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-08-07 13:52:51.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      947 2023-08-07 13:52:51.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.856828 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 13:52:53.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)      970 2023-08-07 13:52:53.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_get.py
--rw-r--r--   0 root         (0) root         (0)      948 2023-08-07 13:52:53.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.856828 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 13:52:53.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1005 2023-08-07 13:52:53.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      989 2023-08-07 13:52:53.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      975 2023-08-07 13:52:53.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.856828 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 13:52:54.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/__init__.py
--rw-r--r--   0 root         (0) root         (0)      970 2023-08-07 13:52:54.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/test_get.py
--rw-r--r--   0 root         (0) root         (0)      976 2023-08-07 13:52:54.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.856828 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 13:52:54.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1064 2023-08-07 13:52:54.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)     1051 2023-08-07 13:52:54.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)     1025 2023-08-07 13:52:54.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.856828 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 13:52:55.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1021 2023-08-07 13:52:55.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      988 2023-08-07 13:52:55.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/test_get.py
--rw-r--r--   0 root         (0) root         (0)     1017 2023-08-07 13:52:55.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/test_post.py
--rw-r--r--   0 root         (0) root         (0)     1014 2023-08-07 13:52:55.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.856828 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 13:53:01.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
--rw-r--r--   0 root         (0) root         (0)      949 2023-08-07 13:53:01.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py
--rw-r--r--   0 root         (0) root         (0)      957 2023-08-07 13:53:01.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.860828 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 13:53:01.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-08-07 13:53:01.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      996 2023-08-07 13:53:01.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-08-07 13:53:01.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.860828 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 13:53:01.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
--rw-r--r--   0 root         (0) root         (0)      993 2023-08-07 13:53:01.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-08-07 13:53:01.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.860828 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 13:53:01.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1056 2023-08-07 13:53:01.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)     1050 2023-08-07 13:53:01.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-08-07 13:53:01.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.860828 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 13:52:58.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-08-07 13:52:58.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py
--rw-r--r--   0 root         (0) root         (0)      936 2023-08-07 13:52:58.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.860828 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 13:52:58.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1047 2023-08-07 13:52:58.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-08-07 13:52:58.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      947 2023-08-07 13:52:58.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.860828 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 13:53:02.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/__init__.py
--rw-r--r--   0 root         (0) root         (0)      982 2023-08-07 13:53:02.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.860828 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 13:53:02.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1081 2023-08-07 13:53:02.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/test_delete.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.860828 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_user/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 13:52:50.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)      899 2023-08-07 13:52:50.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-07 13:53:21.860828 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_user_user_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-07 13:52:50.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)      932 2023-08-07 13:52:50.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      919 2023-08-07 13:52:50.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      902 2023-08-07 13:52:50.000000 iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.754397 iparapheur-provisioning-1.7.5/
+-rw-r--r--   0 root         (0) root         (0)     1111 2023-08-08 14:51:26.000000 iparapheur-provisioning-1.7.5/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      421 2023-08-08 14:52:03.754397 iparapheur-provisioning-1.7.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    21776 2023-08-08 14:51:26.000000 iparapheur-provisioning-1.7.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.702396 iparapheur-provisioning-1.7.5/iparapheur_provisioning/
+-rw-r--r--   0 root         (0) root         (0)      907 2023-08-08 14:51:26.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58620 2023-08-08 14:51:26.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.702396 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/
+-rw-r--r--   0 root         (0) root         (0)      214 2023-08-08 14:51:26.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8048 2023-08-08 14:51:26.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/path_to_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.706396 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/paths/
+-rw-r--r--   0 root         (0) root         (0)      250 2023-08-08 14:51:26.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/paths/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      261 2023-08-08 14:51:17.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-08-08 14:51:17.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id.py
+-rw-r--r--   0 root         (0) root         (0)      303 2023-08-08 14:51:06.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-08-08 14:51:06.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id.py
+-rw-r--r--   0 root         (0) root         (0)      315 2023-08-08 14:51:09.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata.py
+-rw-r--r--   0 root         (0) root         (0)      490 2023-08-08 14:51:09.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id.py
+-rw-r--r--   0 root         (0) root         (0)      338 2023-08-08 14:51:12.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate.py
+-rw-r--r--   0 root         (0) root         (0)      552 2023-08-08 14:51:12.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id.py
+-rw-r--r--   0 root         (0) root         (0)      643 2023-08-08 14:51:14.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type.py
+-rw-r--r--   0 root         (0) root         (0)      329 2023-08-08 14:51:24.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type.py
+-rw-r--r--   0 root         (0) root         (0)      493 2023-08-08 14:51:24.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id.py
+-rw-r--r--   0 root         (0) root         (0)      374 2023-08-08 14:51:24.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype.py
+-rw-r--r--   0 root         (0) root         (0)      566 2023-08-08 14:51:24.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py
+-rw-r--r--   0 root         (0) root         (0)      303 2023-08-08 14:51:19.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-08-08 14:51:19.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id.py
+-rw-r--r--   0 root         (0) root         (0)      210 2023-08-08 14:51:26.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition.py
+-rw-r--r--   0 root         (0) root         (0)      264 2023-08-08 14:51:26.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key.py
+-rw-r--r--   0 root         (0) root         (0)      150 2023-08-08 14:51:04.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user.py
+-rw-r--r--   0 root         (0) root         (0)      393 2023-08-08 14:51:04.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user_user_id.py
+-rw-r--r--   0 root         (0) root         (0)     1929 2023-08-08 14:51:26.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/tag_to_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.710396 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/tags/
+-rw-r--r--   0 root         (0) root         (0)      659 2023-08-08 14:51:26.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/tags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-08-08 14:51:04.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/tags/admin_all_users_api.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-08-08 14:51:07.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/tags/admin_desk_api.py
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-08-08 14:51:09.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/tags/admin_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)     1336 2023-08-08 14:51:12.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/tags/admin_seal_certificate_api.py
+-rw-r--r--   0 root         (0) root         (0)     1138 2023-08-08 14:51:14.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/tags/admin_template_api.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-08-08 14:51:17.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/tags/admin_tenant_api.py
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-08-08 14:51:19.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-08-08 14:51:24.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/tags/admin_typology_api.py
+-rw-r--r--   0 root         (0) root         (0)      863 2023-08-08 14:51:26.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/tags/admin_workflow_definition_api.py
+-rw-r--r--   0 root         (0) root         (0)    15677 2023-08-08 14:51:26.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     4598 2023-08-08 14:51:26.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.718397 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/
+-rw-r--r--   0 root         (0) root         (0)      357 2023-08-08 14:51:26.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6643 2023-08-08 14:50:46.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/certificate_informations.py
+-rw-r--r--   0 root         (0) root         (0)     1426 2023-08-08 14:50:47.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/delegation_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)    24041 2023-08-08 14:50:48.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/desk_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3809 2023-08-08 14:50:50.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)     4553 2023-08-08 14:50:50.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/error_response.py
+-rw-r--r--   0 root         (0) root         (0)     4971 2023-08-08 14:50:50.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/external_signature_config_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-08-08 14:50:51.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/external_signature_config_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1455 2023-08-08 14:50:51.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/external_signature_provider.py
+-rw-r--r--   0 root         (0) root         (0)     2680 2023-08-08 14:50:51.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/folder_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     2656 2023-08-08 14:50:51.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/internal_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     3284 2023-08-08 14:50:51.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/layer_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-08-08 14:50:51.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/layer_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     7908 2023-08-08 14:50:52.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5805 2023-08-08 14:50:52.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/metadata_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-08-08 14:50:52.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/metadata_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1598 2023-08-08 14:50:52.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/metadata_type.py
+-rw-r--r--   0 root         (0) root         (0)     9105 2023-08-08 14:50:52.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/page_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9141 2023-08-08 14:50:53.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/page_metadata_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9205 2023-08-08 14:50:53.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/page_seal_certificate_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9132 2023-08-08 14:50:53.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/page_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9123 2023-08-08 14:50:54.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/page_tenant_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9105 2023-08-08 14:50:54.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/page_type_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9105 2023-08-08 14:50:54.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/page_user_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9232 2023-08-08 14:50:55.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/page_workflow_definition_representation.py
+-rw-r--r--   0 root         (0) root         (0)     5251 2023-08-08 14:50:55.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/pageable_object.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-08-08 14:50:55.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/pdf_signature_position.py
+-rw-r--r--   0 root         (0) root         (0)     8300 2023-08-08 14:50:56.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/seal_certificate_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4500 2023-08-08 14:50:56.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/seal_certificate_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-08-08 14:50:56.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/seal_certificate_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-08-08 14:50:56.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/signature_format.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-08-08 14:50:56.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/signature_protocol.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-08-08 14:50:56.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/sort_object.py
+-rw-r--r--   0 root         (0) root         (0)    29448 2023-08-08 14:50:57.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/subtype_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1307 2023-08-08 14:50:58.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/subtype_layer_association.py
+-rw-r--r--   0 root         (0) root         (0)     3930 2023-08-08 14:50:58.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/subtype_layer_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5468 2023-08-08 14:50:58.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/subtype_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3288 2023-08-08 14:50:58.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)     3082 2023-08-08 14:50:58.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/template_type.py
+-rw-r--r--   0 root         (0) root         (0)     3274 2023-08-08 14:50:58.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/tenant_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3286 2023-08-08 14:50:59.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/tenant_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-08-08 14:50:59.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/tenant_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     9365 2023-08-08 14:50:59.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/type_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4044 2023-08-08 14:50:59.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/type_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1144 2023-08-08 14:50:59.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/typology_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)    29666 2023-08-08 14:51:00.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/user_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-08-08 14:51:01.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/user_privilege.py
+-rw-r--r--   0 root         (0) root         (0)     6504 2023-08-08 14:51:01.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/user_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2023-08-08 14:51:01.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/user_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     4499 2023-08-08 14:51:01.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/workflow_definition_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1256 2023-08-08 14:51:01.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/workflow_definition_sort_by.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.718397 iparapheur-provisioning-1.7.5/iparapheur_provisioning/models/
+-rw-r--r--   0 root         (0) root         (0)     4525 2023-08-08 14:51:26.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.718397 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/
+-rw-r--r--   0 root         (0) root         (0)     2703 2023-08-08 14:51:26.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.722396 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/
+-rw-r--r--   0 root         (0) root         (0)      369 2023-08-08 14:51:17.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13070 2023-08-08 14:51:16.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/get.py
+-rw-r--r--   0 root         (0) root         (0)    13629 2023-08-08 14:51:15.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.722396 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/
+-rw-r--r--   0 root         (0) root         (0)      389 2023-08-08 14:51:17.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11083 2023-08-08 14:51:15.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11332 2023-08-08 14:51:16.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    15808 2023-08-08 14:51:17.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.722396 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-08-08 14:51:06.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15034 2023-08-08 14:51:06.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py
+-rw-r--r--   0 root         (0) root         (0)    16302 2023-08-08 14:51:05.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.722396 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-08-08 14:51:06.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11337 2023-08-08 14:51:05.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11677 2023-08-08 14:51:06.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16545 2023-08-08 14:51:05.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.722396 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/
+-rw-r--r--   0 root         (0) root         (0)      407 2023-08-08 14:51:09.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15486 2023-08-08 14:51:08.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/get.py
+-rw-r--r--   0 root         (0) root         (0)    16907 2023-08-08 14:51:07.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.722396 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/
+-rw-r--r--   0 root         (0) root         (0)      431 2023-08-08 14:51:09.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11413 2023-08-08 14:51:08.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11668 2023-08-08 14:51:08.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16979 2023-08-08 14:51:09.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.726397 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/
+-rw-r--r--   0 root         (0) root         (0)      423 2023-08-08 14:51:12.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14894 2023-08-08 14:51:11.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/get.py
+-rw-r--r--   0 root         (0) root         (0)    19934 2023-08-08 14:51:10.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.726397 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/
+-rw-r--r--   0 root         (0) root         (0)      463 2023-08-08 14:51:12.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12091 2023-08-08 14:51:11.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    12371 2023-08-08 14:51:11.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    20252 2023-08-08 14:51:12.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.726397 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/
+-rw-r--r--   0 root         (0) root         (0)      437 2023-08-08 14:51:14.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11569 2023-08-08 14:51:13.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11613 2023-08-08 14:51:14.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/get.py
+-rw-r--r--   0 root         (0) root         (0)    15581 2023-08-08 14:51:13.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/post.py
+-rw-r--r--   0 root         (0) root         (0)    15574 2023-08-08 14:51:14.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.726397 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/
+-rw-r--r--   0 root         (0) root         (0)      417 2023-08-08 14:51:24.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14728 2023-08-08 14:51:23.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py
+-rw-r--r--   0 root         (0) root         (0)    15777 2023-08-08 14:51:21.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.726397 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
+-rw-r--r--   0 root         (0) root         (0)      433 2023-08-08 14:51:24.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11337 2023-08-08 14:51:21.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11590 2023-08-08 14:51:22.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    15521 2023-08-08 14:51:24.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.730397 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
+-rw-r--r--   0 root         (0) root         (0)      449 2023-08-08 14:51:24.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15050 2023-08-08 14:51:22.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py
+-rw-r--r--   0 root         (0) root         (0)    16640 2023-08-08 14:51:20.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.730397 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
+-rw-r--r--   0 root         (0) root         (0)      471 2023-08-08 14:51:24.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11672 2023-08-08 14:51:21.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11934 2023-08-08 14:51:22.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16645 2023-08-08 14:51:23.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.730397 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-08-08 14:51:19.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15944 2023-08-08 14:51:18.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py
+-rw-r--r--   0 root         (0) root         (0)    16306 2023-08-08 14:51:17.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.730397 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-08-08 14:51:19.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11932 2023-08-08 14:51:19.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11580 2023-08-08 14:51:18.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16046 2023-08-08 14:51:19.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.730397 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/
+-rw-r--r--   0 root         (0) root         (0)      429 2023-08-08 14:51:26.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15256 2023-08-08 14:51:26.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.730397 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/
+-rw-r--r--   0 root         (0) root         (0)      477 2023-08-08 14:51:26.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11623 2023-08-08 14:51:25.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/delete.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.730397 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/
+-rw-r--r--   0 root         (0) root         (0)      365 2023-08-08 14:51:04.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13222 2023-08-08 14:51:03.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.734397 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)      381 2023-08-08 14:51:04.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11207 2023-08-08 14:51:02.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11978 2023-08-08 14:51:03.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    15946 2023-08-08 14:51:04.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py
+-rw-r--r--   0 root         (0) root         (0)    10635 2023-08-08 14:51:26.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/rest.py
+-rw-r--r--   0 root         (0) root         (0)    97752 2023-08-08 14:51:26.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.702396 iparapheur-provisioning-1.7.5/iparapheur_provisioning.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      421 2023-08-08 14:52:03.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    20426 2023-08-08 14:52:03.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 14:52:03.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      118 2023-08-08 14:52:03.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-08-08 14:52:03.000000 iparapheur-provisioning-1.7.5/iparapheur_provisioning.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-08-08 14:52:03.754397 iparapheur-provisioning-1.7.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-08-08 14:51:26.000000 iparapheur-provisioning-1.7.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.698396 iparapheur-provisioning-1.7.5/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.742397 iparapheur-provisioning-1.7.5/test/test_models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 14:51:26.000000 iparapheur-provisioning-1.7.5/test/test_models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      709 2023-08-08 14:50:46.000000 iparapheur-provisioning-1.7.5/test/test_models/test_certificate_informations.py
+-rw-r--r--   0 root         (0) root         (0)      682 2023-08-08 14:50:47.000000 iparapheur-provisioning-1.7.5/test/test_models/test_delegation_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      645 2023-08-08 14:50:49.000000 iparapheur-provisioning-1.7.5/test/test_models/test_desk_dto.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-08-08 14:50:50.000000 iparapheur-provisioning-1.7.5/test/test_models/test_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-08-08 14:50:50.000000 iparapheur-provisioning-1.7.5/test/test_models/test_error_response.py
+-rw-r--r--   0 root         (0) root         (0)      767 2023-08-08 14:50:51.000000 iparapheur-provisioning-1.7.5/test/test_models/test_external_signature_config_representation.py
+-rw-r--r--   0 root         (0) root         (0)      736 2023-08-08 14:50:51.000000 iparapheur-provisioning-1.7.5/test/test_models/test_external_signature_config_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      718 2023-08-08 14:50:51.000000 iparapheur-provisioning-1.7.5/test/test_models/test_external_signature_provider.py
+-rw-r--r--   0 root         (0) root         (0)      666 2023-08-08 14:50:51.000000 iparapheur-provisioning-1.7.5/test/test_models/test_folder_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      681 2023-08-08 14:50:51.000000 iparapheur-provisioning-1.7.5/test/test_models/test_internal_metadata.py
+-rw-r--r--   0 root         (0) root         (0)      693 2023-08-08 14:50:51.000000 iparapheur-provisioning-1.7.5/test/test_models/test_layer_representation.py
+-rw-r--r--   0 root         (0) root         (0)      662 2023-08-08 14:50:51.000000 iparapheur-provisioning-1.7.5/test/test_models/test_layer_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      661 2023-08-08 14:50:52.000000 iparapheur-provisioning-1.7.5/test/test_models/test_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)      705 2023-08-08 14:50:52.000000 iparapheur-provisioning-1.7.5/test/test_models/test_metadata_representation.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-08-08 14:50:52.000000 iparapheur-provisioning-1.7.5/test/test_models/test_metadata_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      665 2023-08-08 14:50:52.000000 iparapheur-provisioning-1.7.5/test/test_models/test_metadata_type.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-08-08 14:50:52.000000 iparapheur-provisioning-1.7.5/test/test_models/test_page_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)      722 2023-08-08 14:50:53.000000 iparapheur-provisioning-1.7.5/test/test_models/test_page_metadata_representation.py
+-rw-r--r--   0 root         (0) root         (0)      751 2023-08-08 14:50:53.000000 iparapheur-provisioning-1.7.5/test/test_models/test_page_seal_certificate_representation.py
+-rw-r--r--   0 root         (0) root         (0)      718 2023-08-08 14:50:53.000000 iparapheur-provisioning-1.7.5/test/test_models/test_page_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)      714 2023-08-08 14:50:54.000000 iparapheur-provisioning-1.7.5/test/test_models/test_page_tenant_representation.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-08-08 14:50:54.000000 iparapheur-provisioning-1.7.5/test/test_models/test_page_type_representation.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-08-08 14:50:55.000000 iparapheur-provisioning-1.7.5/test/test_models/test_page_user_representation.py
+-rw-r--r--   0 root         (0) root         (0)      763 2023-08-08 14:50:55.000000 iparapheur-provisioning-1.7.5/test/test_models/test_page_workflow_definition_representation.py
+-rw-r--r--   0 root         (0) root         (0)      673 2023-08-08 14:50:55.000000 iparapheur-provisioning-1.7.5/test/test_models/test_pageable_object.py
+-rw-r--r--   0 root         (0) root         (0)      698 2023-08-08 14:50:55.000000 iparapheur-provisioning-1.7.5/test/test_models/test_pdf_signature_position.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-08-08 14:50:56.000000 iparapheur-provisioning-1.7.5/test/test_models/test_seal_certificate_dto.py
+-rw-r--r--   0 root         (0) root         (0)      734 2023-08-08 14:50:56.000000 iparapheur-provisioning-1.7.5/test/test_models/test_seal_certificate_representation.py
+-rw-r--r--   0 root         (0) root         (0)      703 2023-08-08 14:50:56.000000 iparapheur-provisioning-1.7.5/test/test_models/test_seal_certificate_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      677 2023-08-08 14:50:56.000000 iparapheur-provisioning-1.7.5/test/test_models/test_signature_format.py
+-rw-r--r--   0 root         (0) root         (0)      685 2023-08-08 14:50:56.000000 iparapheur-provisioning-1.7.5/test/test_models/test_signature_protocol.py
+-rw-r--r--   0 root         (0) root         (0)      657 2023-08-08 14:50:56.000000 iparapheur-provisioning-1.7.5/test/test_models/test_sort_object.py
+-rw-r--r--   0 root         (0) root         (0)      657 2023-08-08 14:50:57.000000 iparapheur-provisioning-1.7.5/test/test_models/test_subtype_dto.py
+-rw-r--r--   0 root         (0) root         (0)      710 2023-08-08 14:50:58.000000 iparapheur-provisioning-1.7.5/test/test_models/test_subtype_layer_association.py
+-rw-r--r--   0 root         (0) root         (0)      678 2023-08-08 14:50:58.000000 iparapheur-provisioning-1.7.5/test/test_models/test_subtype_layer_dto.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-08-08 14:50:58.000000 iparapheur-provisioning-1.7.5/test/test_models/test_subtype_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)      701 2023-08-08 14:50:58.000000 iparapheur-provisioning-1.7.5/test/test_models/test_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)      665 2023-08-08 14:50:58.000000 iparapheur-provisioning-1.7.5/test/test_models/test_template_type.py
+-rw-r--r--   0 root         (0) root         (0)      653 2023-08-08 14:50:58.000000 iparapheur-provisioning-1.7.5/test/test_models/test_tenant_dto.py
+-rw-r--r--   0 root         (0) root         (0)      697 2023-08-08 14:50:59.000000 iparapheur-provisioning-1.7.5/test/test_models/test_tenant_representation.py
+-rw-r--r--   0 root         (0) root         (0)      666 2023-08-08 14:50:59.000000 iparapheur-provisioning-1.7.5/test/test_models/test_tenant_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      645 2023-08-08 14:50:59.000000 iparapheur-provisioning-1.7.5/test/test_models/test_type_dto.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-08-08 14:50:59.000000 iparapheur-provisioning-1.7.5/test/test_models/test_type_representation.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-08-08 14:50:59.000000 iparapheur-provisioning-1.7.5/test/test_models/test_typology_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      645 2023-08-08 14:51:00.000000 iparapheur-provisioning-1.7.5/test/test_models/test_user_dto.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-08-08 14:51:01.000000 iparapheur-provisioning-1.7.5/test/test_models/test_user_privilege.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-08-08 14:51:01.000000 iparapheur-provisioning-1.7.5/test/test_models/test_user_representation.py
+-rw-r--r--   0 root         (0) root         (0)      658 2023-08-08 14:51:01.000000 iparapheur-provisioning-1.7.5/test/test_models/test_user_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      746 2023-08-08 14:51:01.000000 iparapheur-provisioning-1.7.5/test/test_models/test_workflow_definition_representation.py
+-rw-r--r--   0 root         (0) root         (0)      715 2023-08-08 14:51:01.000000 iparapheur-provisioning-1.7.5/test/test_models/test_workflow_definition_sort_by.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.742397 iparapheur-provisioning-1.7.5/test/test_paths/
+-rw-r--r--   0 root         (0) root         (0)     1995 2023-08-08 14:51:26.000000 iparapheur-provisioning-1.7.5/test/test_paths/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.742397 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 14:51:17.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      887 2023-08-08 14:51:17.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      899 2023-08-08 14:51:17.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.742397 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 14:51:17.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      925 2023-08-08 14:51:17.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      930 2023-08-08 14:51:17.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      916 2023-08-08 14:51:17.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.742397 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 14:51:07.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      924 2023-08-08 14:51:07.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-08-08 14:51:06.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.746397 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 14:51:06.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      956 2023-08-08 14:51:06.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-08-08 14:51:06.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      947 2023-08-08 14:51:06.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.746397 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 14:51:09.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      970 2023-08-08 14:51:09.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      948 2023-08-08 14:51:09.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.746397 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 14:51:09.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      984 2023-08-08 14:51:09.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      989 2023-08-08 14:51:09.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      975 2023-08-08 14:51:09.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.746397 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 14:51:12.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      970 2023-08-08 14:51:12.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      976 2023-08-08 14:51:12.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.746397 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 14:51:12.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-08-08 14:51:12.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)     1051 2023-08-08 14:51:12.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-08-08 14:51:12.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.746397 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 14:51:14.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1000 2023-08-08 14:51:14.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      988 2023-08-08 14:51:14.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      996 2023-08-08 14:51:14.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/test_post.py
+-rw-r--r--   0 root         (0) root         (0)      993 2023-08-08 14:51:14.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.750397 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 14:51:24.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      949 2023-08-08 14:51:24.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      957 2023-08-08 14:51:24.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.750397 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 14:51:24.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      981 2023-08-08 14:51:24.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      996 2023-08-08 14:51:24.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-08-08 14:51:24.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.750397 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 14:51:24.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      993 2023-08-08 14:51:24.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-08-08 14:51:24.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.750397 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 14:51:24.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1035 2023-08-08 14:51:24.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)     1050 2023-08-08 14:51:24.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-08-08 14:51:24.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.750397 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 14:51:19.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-08-08 14:51:19.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      936 2023-08-08 14:51:19.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.750397 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 14:51:19.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-08-08 14:51:19.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-08-08 14:51:19.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      947 2023-08-08 14:51:19.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.750397 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 14:51:26.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      982 2023-08-08 14:51:26.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.750397 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 14:51:26.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1060 2023-08-08 14:51:26.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/test_delete.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.754397 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_user/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 14:51:04.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      899 2023-08-08 14:51:04.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 14:52:03.754397 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 14:51:04.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      911 2023-08-08 14:51:04.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      919 2023-08-08 14:51:04.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      902 2023-08-08 14:51:04.000000 iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py
```

### Comparing `iparapheur-provisioning-1.7.4/LICENSE.md` & `iparapheur-provisioning-1.7.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/README.md` & `iparapheur-provisioning-1.7.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 The main link between every sub-services, integrating business code logic.
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: DEVELOP
-- Package version: 1.7.4
+- Package version: 1.7.5
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://libriciel.fr](https://libriciel.fr)
 
 ## Requirements.
 
 Python &gt;&#x3D;3.7
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/__init__.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     iparapheur v5.x main core application.  The main link between every sub-services, integrating business code logic.   # noqa: E501
 
     The version of the OpenAPI document: DEVELOP
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
-__version__ = "1.7.4"
+__version__ = "1.7.5"
 
 # import ApiClient
 from iparapheur_provisioning.api_client import ApiClient
 
 # import Configuration
 from iparapheur_provisioning.configuration import Configuration
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/api_client.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1000,15 +1000,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = HTTPHeaderDict()
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.7.4/python'
+        self.user_agent = 'OpenAPI-Generator/1.7.5/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/path_to_api.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/tag_to_api.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/tag_to_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/tags/__init__.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/tags/admin_all_users_api.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/tags/admin_all_users_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/tags/admin_desk_api.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/tags/admin_desk_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/tags/admin_metadata_api.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/tags/admin_metadata_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/tags/admin_seal_certificate_api.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/tags/admin_seal_certificate_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/tags/admin_template_api.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/tags/admin_template_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/tags/admin_tenant_api.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/tags/admin_tenant_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/tags/admin_typology_api.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/tags/admin_typology_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/apis/tags/admin_workflow_definition_api.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/apis/tags/admin_workflow_definition_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/configuration.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,15 +365,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: DEVELOP\n"\
-               "SDK Package Version: 1.7.4".\
+               "SDK Package Version: 1.7.5".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/exceptions.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/exceptions.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/certificate_informations.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/certificate_informations.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/delegation_sort_by.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/delegation_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/desk_dto.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/desk_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/desk_representation.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/error_response.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/error_response.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/external_signature_config_representation.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/external_signature_config_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/external_signature_config_sort_by.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/external_signature_config_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/external_signature_provider.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/external_signature_provider.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/folder_sort_by.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/folder_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/internal_metadata.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/internal_metadata.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/layer_representation.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/layer_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/layer_sort_by.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/layer_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/metadata_dto.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/metadata_representation.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/metadata_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/metadata_sort_by.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/metadata_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/metadata_type.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/metadata_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/page_desk_representation.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/page_desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/page_metadata_representation.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/page_metadata_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/page_seal_certificate_representation.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/page_seal_certificate_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/page_subtype_representation.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/page_subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/page_tenant_representation.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/page_tenant_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/page_type_representation.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/page_type_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/page_user_representation.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/page_user_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/page_workflow_definition_representation.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/page_workflow_definition_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/pageable_object.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/pageable_object.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/pdf_signature_position.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/pdf_signature_position.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/seal_certificate_dto.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/seal_certificate_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/seal_certificate_representation.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/seal_certificate_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/seal_certificate_sort_by.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/seal_certificate_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/signature_format.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/signature_format.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/signature_protocol.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/signature_protocol.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/sort_object.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/sort_object.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/subtype_dto.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/subtype_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/subtype_layer_association.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/subtype_layer_association.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/subtype_layer_dto.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/subtype_layer_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/subtype_metadata_dto.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/subtype_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/subtype_representation.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/template_type.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/template_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/tenant_dto.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/tenant_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/tenant_representation.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/tenant_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/tenant_sort_by.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/tenant_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/type_dto.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/type_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/type_representation.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/type_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/typology_sort_by.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/typology_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/user_dto.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/user_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/user_privilege.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/user_privilege.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/user_representation.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/user_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/user_sort_by.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/user_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/workflow_definition_representation.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/workflow_definition_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/model/workflow_definition_sort_by.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/model/workflow_definition_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/models/__init__.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/models/__init__.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/__init__.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/get.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -117,69 +117,69 @@
     style=api_client.ParameterStyle.FORM,
     schema=SearchTermSchema,
     explode=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = PageTenantRepresentation
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageTenantRepresentation
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -194,17 +194,17 @@
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '200': _response_for_200,
     '403': _response_for_403,
     '400': _response_for_400,
+    '200': _response_for_200,
     '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -40,115 +40,115 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor201ResponseBodyApplicationJson = TenantDto
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor201(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor201ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_201 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor201,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor201ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor201ResponseBodyApplicationJson = TenantDto
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor201(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor201ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_201 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '507': _response_for_507,
-    '201': _response_for_201,
     '403': _response_for_403,
     '400': _response_for_400,
     '401': _response_for_401,
+    '201': _response_for_201,
+    '507': _response_for_507,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -54,26 +54,14 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-
-
-@dataclass
-class ApiResponseFor204(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: schemas.Unset = schemas.unset
-    headers: schemas.Unset = schemas.unset
-
-
-_response_for_204 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor204,
-)
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
@@ -85,32 +73,25 @@
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor204(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
-    ]
+    body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
-    },
+_response_for_204 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor204,
 )
 SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
@@ -123,19 +104,38 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+
+
+@dataclass
+class ApiResponseFor401(api_client.ApiResponse):
+    response: urllib3.HTTPResponse
+    body: typing.Union[
+        SchemaFor401ResponseBodyApplicationJson,
+    ]
+    headers: schemas.Unset = schemas.unset
+
+
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaFor401ResponseBodyApplicationJson),
+    },
+)
 _status_code_to_response = {
-    '204': _response_for_204,
     '403': _response_for_403,
-    '401': _response_for_401,
+    '204': _response_for_204,
     '404': _response_for_404,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -55,95 +55,95 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = TenantDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = TenantDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '200': _response_for_200,
     '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '200': _response_for_200,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,115 +66,115 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = TenantDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = TenantDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '200': _response_for_200,
     '403': _response_for_403,
     '400': _response_for_400,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '200': _response_for_200,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -143,69 +143,69 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = PageDeskRepresentation
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageDeskRepresentation
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -220,17 +220,17 @@
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '200': _response_for_200,
     '403': _response_for_403,
     '400': _response_for_400,
+    '200': _response_for_200,
     '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,135 +66,135 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor201ResponseBodyApplicationJson = DeskDto
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor201(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor201ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_201 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor201,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor201ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor201ResponseBodyApplicationJson = DeskDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor201(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor201ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_201 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '507': _response_for_507,
-    '409': _response_for_409,
-    '201': _response_for_201,
     '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '401': _response_for_401,
+    '201': _response_for_201,
+    '507': _response_for_507,
+    '409': _response_for_409,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -62,26 +62,14 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=DeskIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-
-
-@dataclass
-class ApiResponseFor204(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: schemas.Unset = schemas.unset
-    headers: schemas.Unset = schemas.unset
-
-
-_response_for_204 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor204,
-)
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
@@ -93,32 +81,25 @@
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor204(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
-    ]
+    body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
-    },
+_response_for_204 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor204,
 )
 SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
@@ -131,19 +112,38 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+
+
+@dataclass
+class ApiResponseFor401(api_client.ApiResponse):
+    response: urllib3.HTTPResponse
+    body: typing.Union[
+        SchemaFor401ResponseBodyApplicationJson,
+    ]
+    headers: schemas.Unset = schemas.unset
+
+
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaFor401ResponseBodyApplicationJson),
+    },
+)
 _status_code_to_response = {
-    '204': _response_for_204,
     '403': _response_for_403,
-    '401': _response_for_401,
+    '204': _response_for_204,
     '404': _response_for_404,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -63,95 +63,95 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=DeskIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = DeskDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = DeskDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '200': _response_for_200,
     '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '200': _response_for_200,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,50 +74,50 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 SchemaFor200ResponseBodyApplicationJson = DeskDto
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
@@ -131,78 +131,78 @@
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '507': _response_for_507,
-    '409': _response_for_409,
-    '200': _response_for_200,
     '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '200': _response_for_200,
+    '401': _response_for_401,
+    '507': _response_for_507,
+    '409': _response_for_409,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/get.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -151,95 +151,95 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = PageMetadataRepresentation
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageMetadataRepresentation
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '200': _response_for_200,
     '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '200': _response_for_200,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/post.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,155 +66,155 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor201ResponseBodyApplicationJson = MetadataDto
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor201(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor201ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_201 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor201,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor201ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor201ResponseBodyApplicationJson = MetadataDto
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor201(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor201ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_201 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '507': _response_for_507,
-    '409': _response_for_409,
-    '201': _response_for_201,
     '403': _response_for_403,
     '400': _response_for_400,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '401': _response_for_401,
+    '201': _response_for_201,
+    '507': _response_for_507,
+    '409': _response_for_409,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/delete.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/delete.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -62,26 +62,14 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=MetadataIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-
-
-@dataclass
-class ApiResponseFor204(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: schemas.Unset = schemas.unset
-    headers: schemas.Unset = schemas.unset
-
-
-_response_for_204 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor204,
-)
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
@@ -93,32 +81,25 @@
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor204(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
-    ]
+    body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
-    },
+_response_for_204 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor204,
 )
 SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
@@ -131,19 +112,38 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+
+
+@dataclass
+class ApiResponseFor401(api_client.ApiResponse):
+    response: urllib3.HTTPResponse
+    body: typing.Union[
+        SchemaFor401ResponseBodyApplicationJson,
+    ]
+    headers: schemas.Unset = schemas.unset
+
+
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaFor401ResponseBodyApplicationJson),
+    },
+)
 _status_code_to_response = {
-    '204': _response_for_204,
     '403': _response_for_403,
-    '401': _response_for_401,
+    '204': _response_for_204,
     '404': _response_for_404,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/get.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -63,95 +63,95 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=MetadataIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = MetadataDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = MetadataDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '200': _response_for_200,
     '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '200': _response_for_200,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/put.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,82 +74,82 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: schemas.Unset = schemas.unset
+    body: typing.Union[
+        SchemaFor400ResponseBodyApplicationJson,
+    ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaFor400ResponseBodyApplicationJson),
+    },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
-    ]
+    body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
-    },
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
@@ -181,41 +181,41 @@
 _response_for_406 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor406,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor406ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '507': _response_for_507,
-    '200': _response_for_200,
     '403': _response_for_403,
     '400': _response_for_400,
+    '404': _response_for_404,
+    '200': _response_for_200,
     '401': _response_for_401,
     '406': _response_for_406,
-    '404': _response_for_404,
+    '507': _response_for_507,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/get.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -135,95 +135,95 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = PageSealCertificateRepresentation
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageSealCertificateRepresentation
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '200': _response_for_200,
     '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '200': _response_for_200,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/post.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -144,115 +144,115 @@
         'multipart/form-data': api_client.MediaType(
             schema=SchemaForRequestBodyMultipartFormData),
     },
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor201ResponseBodyApplicationJson = SealCertificateDto
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor201(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor201ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_201 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor201,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor201ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor201ResponseBodyApplicationJson = SealCertificateDto
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor201(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor201ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_201 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '507': _response_for_507,
-    '201': _response_for_201,
     '403': _response_for_403,
     '400': _response_for_400,
     '401': _response_for_401,
+    '201': _response_for_201,
+    '507': _response_for_507,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/delete.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -62,43 +62,62 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=SealCertificateIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+
+
+@dataclass
+class ApiResponseFor403(api_client.ApiResponse):
+    response: urllib3.HTTPResponse
+    body: typing.Union[
+        SchemaFor403ResponseBodyApplicationJson,
+    ]
+    headers: schemas.Unset = schemas.unset
+
+
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaFor403ResponseBodyApplicationJson),
+    },
+)
 
 
 @dataclass
 class ApiResponseFor204(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -131,39 +150,20 @@
 _response_for_406 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor406,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor406ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
-
-
-@dataclass
-class ApiResponseFor404(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
-    ]
-    headers: schemas.Unset = schemas.unset
-
-
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
-    },
-)
 _status_code_to_response = {
-    '204': _response_for_204,
     '403': _response_for_403,
+    '204': _response_for_204,
+    '404': _response_for_404,
     '401': _response_for_401,
     '406': _response_for_406,
-    '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/get.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -63,115 +63,115 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=SealCertificateIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = SealCertificateDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = SealCertificateDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '200': _response_for_200,
     '403': _response_for_403,
     '400': _response_for_400,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '200': _response_for_200,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/put.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/put.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -150,115 +150,115 @@
         'multipart/form-data': api_client.MediaType(
             schema=SchemaForRequestBodyMultipartFormData),
     },
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = SealCertificateDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = SealCertificateDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '200': _response_for_200,
     '403': _response_for_403,
     '400': _response_for_400,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '200': _response_for_200,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/delete.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/delete.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -63,26 +63,14 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TemplateTypeSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-
-
-@dataclass
-class ApiResponseFor200(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: schemas.Unset = schemas.unset
-    headers: schemas.Unset = schemas.unset
-
-
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
-)
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
@@ -94,57 +82,69 @@
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
+    response: urllib3.HTTPResponse
+    body: schemas.Unset = schemas.unset
+    headers: schemas.Unset = schemas.unset
+
+
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
+)
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+
+
+@dataclass
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '200': _response_for_200,
     '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '200': _response_for_200,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/get.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -63,97 +63,97 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TemplateTypeSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        schemas.Unset,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+        'text/plain': api_client.MediaType(),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        schemas.Unset,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
-        'text/plain': api_client.MediaType(),
+        'application/json': api_client.MediaType(
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '403': _response_for_403,
-    '401': _response_for_401,
     '200': _response_for_200,
+    '403': _response_for_403,
     '404': _response_for_404,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
-    'application/json',
     'text/plain',
+    'application/json',
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
     def _get_custom_template_oapg(
         self,
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/post.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,26 +74,14 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-
-
-@dataclass
-class ApiResponseFor200(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: schemas.Unset = schemas.unset
-    headers: schemas.Unset = schemas.unset
-
-
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
-)
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
@@ -105,57 +93,69 @@
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
+    response: urllib3.HTTPResponse
+    body: schemas.Unset = schemas.unset
+    headers: schemas.Unset = schemas.unset
+
+
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
+)
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+
+
+@dataclass
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '200': _response_for_200,
     '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '200': _response_for_200,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/put.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,26 +74,14 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-
-
-@dataclass
-class ApiResponseFor200(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: schemas.Unset = schemas.unset
-    headers: schemas.Unset = schemas.unset
-
-
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
-)
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
@@ -105,57 +93,69 @@
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
+    response: urllib3.HTTPResponse
+    body: schemas.Unset = schemas.unset
+    headers: schemas.Unset = schemas.unset
+
+
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
+)
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+
+
+@dataclass
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '200': _response_for_200,
     '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '200': _response_for_200,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -135,95 +135,95 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = PageTypeRepresentation
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageTypeRepresentation
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '200': _response_for_200,
     '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '200': _response_for_200,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,50 +66,50 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 SchemaFor201ResponseBodyApplicationJson = TypeDto
 
 
 @dataclass
 class ApiResponseFor201(api_client.ApiResponse):
@@ -123,58 +123,58 @@
 _response_for_201 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '507': _response_for_507,
-    '409': _response_for_409,
-    '201': _response_for_201,
     '403': _response_for_403,
     '401': _response_for_401,
+    '201': _response_for_201,
+    '507': _response_for_507,
+    '409': _response_for_409,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -62,26 +62,14 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TypeIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-
-
-@dataclass
-class ApiResponseFor204(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: schemas.Unset = schemas.unset
-    headers: schemas.Unset = schemas.unset
-
-
-_response_for_204 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor204,
-)
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
@@ -93,32 +81,25 @@
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor204(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
-    ]
+    body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
-    },
+_response_for_204 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor204,
 )
 SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
@@ -131,19 +112,38 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+
+
+@dataclass
+class ApiResponseFor401(api_client.ApiResponse):
+    response: urllib3.HTTPResponse
+    body: typing.Union[
+        SchemaFor401ResponseBodyApplicationJson,
+    ]
+    headers: schemas.Unset = schemas.unset
+
+
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaFor401ResponseBodyApplicationJson),
+    },
+)
 _status_code_to_response = {
-    '204': _response_for_204,
     '403': _response_for_403,
-    '401': _response_for_401,
+    '204': _response_for_204,
     '404': _response_for_404,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -63,95 +63,95 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TypeIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = TypeDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = TypeDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '200': _response_for_200,
     '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '200': _response_for_200,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,95 +74,95 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = TypeDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = TypeDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '200': _response_for_200,
     '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '200': _response_for_200,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -143,95 +143,95 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TypeIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = PageSubtypeRepresentation
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageSubtypeRepresentation
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '200': _response_for_200,
     '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '200': _response_for_200,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,135 +74,135 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor201ResponseBodyApplicationJson = SubtypeDto
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor201(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor201ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_201 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor201,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor201ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor201ResponseBodyApplicationJson = SubtypeDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor201(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor201ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_201 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '507': _response_for_507,
-    '409': _response_for_409,
-    '201': _response_for_201,
     '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '401': _response_for_401,
+    '201': _response_for_201,
+    '507': _response_for_507,
+    '409': _response_for_409,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -70,26 +70,14 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=SubtypeIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-
-
-@dataclass
-class ApiResponseFor204(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: schemas.Unset = schemas.unset
-    headers: schemas.Unset = schemas.unset
-
-
-_response_for_204 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor204,
-)
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
@@ -101,32 +89,25 @@
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor204(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
-    ]
+    body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
-    },
+_response_for_204 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor204,
 )
 SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
@@ -139,19 +120,38 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+
+
+@dataclass
+class ApiResponseFor401(api_client.ApiResponse):
+    response: urllib3.HTTPResponse
+    body: typing.Union[
+        SchemaFor401ResponseBodyApplicationJson,
+    ]
+    headers: schemas.Unset = schemas.unset
+
+
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaFor401ResponseBodyApplicationJson),
+    },
+)
 _status_code_to_response = {
-    '204': _response_for_204,
     '403': _response_for_403,
-    '401': _response_for_401,
+    '204': _response_for_204,
     '404': _response_for_404,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -71,95 +71,95 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=SubtypeIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = SubtypeDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = SubtypeDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '200': _response_for_200,
     '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '200': _response_for_200,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -82,88 +82,88 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor204ResponseBodyApplicationJson = SubtypeDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor204(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor204ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_204 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor204,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor204ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor204ResponseBodyApplicationJson = SubtypeDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor204(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor204ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_204 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor204,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor204ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 SchemaFor200ResponseBodyApplicationJson = SubtypeDto
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
@@ -178,18 +178,18 @@
     response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '204': _response_for_204,
     '403': _response_for_403,
-    '401': _response_for_401,
+    '204': _response_for_204,
     '404': _response_for_404,
+    '401': _response_for_401,
     '200': _response_for_200,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -151,115 +151,115 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = PageUserRepresentation
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageUserRepresentation
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '200': _response_for_200,
     '403': _response_for_403,
     '400': _response_for_400,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '200': _response_for_200,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,135 +66,135 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor201ResponseBodyApplicationJson = UserDto
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor201(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor201ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_201 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor201,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor201ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor201ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor201(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor201ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_201 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '507': _response_for_507,
-    '409': _response_for_409,
-    '201': _response_for_201,
     '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '401': _response_for_401,
+    '201': _response_for_201,
+    '507': _response_for_507,
+    '409': _response_for_409,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -62,43 +62,62 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=UserIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+
+
+@dataclass
+class ApiResponseFor403(api_client.ApiResponse):
+    response: urllib3.HTTPResponse
+    body: typing.Union[
+        SchemaFor403ResponseBodyApplicationJson,
+    ]
+    headers: schemas.Unset = schemas.unset
+
+
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaFor403ResponseBodyApplicationJson),
+    },
+)
 
 
 @dataclass
 class ApiResponseFor204(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -131,39 +150,20 @@
 _response_for_406 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor406,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor406ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
-
-
-@dataclass
-class ApiResponseFor404(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
-    ]
-    headers: schemas.Unset = schemas.unset
-
-
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
-    },
-)
 _status_code_to_response = {
-    '204': _response_for_204,
     '403': _response_for_403,
+    '204': _response_for_204,
+    '404': _response_for_404,
     '401': _response_for_401,
     '406': _response_for_406,
-    '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -63,95 +63,95 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=UserIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = UserDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '200': _response_for_200,
     '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '200': _response_for_200,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,115 +74,115 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = UserDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor406ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor406(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor406ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_406 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor406,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor406ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor406ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor406(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor406ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_406 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor406,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor406ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '200': _response_for_200,
     '403': _response_for_403,
+    '404': _response_for_404,
+    '200': _response_for_200,
     '401': _response_for_401,
     '406': _response_for_406,
-    '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/get.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -143,33 +143,14 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = PageWorkflowDefinitionRepresentation
-
-
-@dataclass
-class ApiResponseFor200(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
-    ]
-    headers: schemas.Unset = schemas.unset
-
-
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
-    },
-)
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
@@ -219,19 +200,38 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
+SchemaFor200ResponseBodyApplicationJson = PageWorkflowDefinitionRepresentation
+
+
+@dataclass
+class ApiResponseFor200(api_client.ApiResponse):
+    response: urllib3.HTTPResponse
+    body: typing.Union[
+        SchemaFor200ResponseBodyApplicationJson,
+    ]
+    headers: schemas.Unset = schemas.unset
+
+
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaFor200ResponseBodyApplicationJson),
+    },
+)
 _status_code_to_response = {
-    '200': _response_for_200,
     '403': _response_for_403,
     '400': _response_for_400,
     '404': _response_for_404,
+    '200': _response_for_200,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/delete.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -62,26 +62,14 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=WorkflowDefinitionKeySchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-
-
-@dataclass
-class ApiResponseFor204(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: schemas.Unset = schemas.unset
-    headers: schemas.Unset = schemas.unset
-
-
-_response_for_204 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor204,
-)
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
@@ -93,32 +81,25 @@
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor204(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
-    ]
+    body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
-    },
+_response_for_204 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor204,
 )
 SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
@@ -131,19 +112,38 @@
 _response_for_404 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+
+
+@dataclass
+class ApiResponseFor401(api_client.ApiResponse):
+    response: urllib3.HTTPResponse
+    body: typing.Union[
+        SchemaFor401ResponseBodyApplicationJson,
+    ]
+    headers: schemas.Unset = schemas.unset
+
+
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaFor401ResponseBodyApplicationJson),
+    },
+)
 _status_code_to_response = {
-    '204': _response_for_204,
     '403': _response_for_403,
-    '401': _response_for_401,
+    '204': _response_for_204,
     '404': _response_for_404,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -117,69 +117,69 @@
     style=api_client.ParameterStyle.FORM,
     schema=SearchTermSchema,
     explode=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = PageUserRepresentation
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageUserRepresentation
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -194,17 +194,17 @@
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '200': _response_for_200,
     '403': _response_for_403,
     '400': _response_for_400,
+    '200': _response_for_200,
     '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -54,26 +54,14 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=UserIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-
-
-@dataclass
-class ApiResponseFor204(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: schemas.Unset = schemas.unset
-    headers: schemas.Unset = schemas.unset
-
-
-_response_for_204 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor204,
-)
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
@@ -104,14 +92,26 @@
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
+
+
+@dataclass
+class ApiResponseFor204(api_client.ApiResponse):
+    response: urllib3.HTTPResponse
+    body: schemas.Unset = schemas.unset
+    headers: schemas.Unset = schemas.unset
+
+
+_response_for_204 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor204,
+)
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
@@ -124,17 +124,17 @@
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '204': _response_for_204,
     '403': _response_for_403,
     '400': _response_for_400,
+    '204': _response_for_204,
     '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -55,115 +55,115 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=UserIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = UserDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '200': _response_for_200,
     '403': _response_for_403,
     '400': _response_for_400,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '200': _response_for_200,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,115 +66,115 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = UserDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '200': _response_for_200,
     '403': _response_for_403,
     '400': _response_for_400,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '200': _response_for_200,
+    '401': _response_for_401,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/rest.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/rest.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning/schemas.py` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning/schemas.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/iparapheur_provisioning.egg-info/SOURCES.txt` & `iparapheur-provisioning-1.7.5/iparapheur_provisioning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/setup.py` & `iparapheur-provisioning-1.7.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "iparapheur-provisioning"
-VERSION = "1.7.4"
+VERSION = "1.7.5"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_certificate_informations.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_certificate_informations.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_delegation_sort_by.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_delegation_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_desk_dto.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_desk_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_desk_representation.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_error_response.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_error_response.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_external_signature_config_representation.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_external_signature_config_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_external_signature_config_sort_by.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_external_signature_config_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_external_signature_provider.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_external_signature_provider.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_folder_sort_by.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_folder_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_internal_metadata.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_internal_metadata.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_layer_representation.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_layer_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_layer_sort_by.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_layer_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_metadata_dto.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_metadata_representation.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_metadata_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_metadata_sort_by.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_metadata_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_metadata_type.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_metadata_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_page_desk_representation.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_page_desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_page_metadata_representation.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_page_metadata_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_page_seal_certificate_representation.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_page_seal_certificate_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_page_subtype_representation.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_page_subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_page_tenant_representation.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_page_tenant_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_page_type_representation.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_page_type_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_page_user_representation.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_page_user_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_page_workflow_definition_representation.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_page_workflow_definition_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_pageable_object.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_pageable_object.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_pdf_signature_position.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_pdf_signature_position.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_seal_certificate_dto.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_seal_certificate_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_seal_certificate_representation.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_seal_certificate_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_seal_certificate_sort_by.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_seal_certificate_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_signature_format.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_signature_format.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_signature_protocol.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_signature_protocol.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_sort_object.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_sort_object.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_subtype_dto.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_subtype_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_subtype_layer_association.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_subtype_layer_association.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_subtype_layer_dto.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_subtype_layer_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_subtype_metadata_dto.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_subtype_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_subtype_representation.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_template_type.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_template_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_tenant_dto.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_tenant_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_tenant_representation.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_tenant_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_tenant_sort_by.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_tenant_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_type_dto.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_type_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_type_representation.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_type_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_typology_sort_by.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_typology_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_user_dto.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_user_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_user_privilege.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_user_privilege.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_user_representation.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_user_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_user_sort_by.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_user_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_workflow_definition_representation.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_workflow_definition_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_models/test_workflow_definition_sort_by.py` & `iparapheur-provisioning-1.7.5/test/test_models/test_workflow_definition_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/__init__.py` & `iparapheur-provisioning-1.7.5/test/test_paths/__init__.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant/test_get.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant/test_get.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_post.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant import post  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_metadata import post  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenant(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdMetadata(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenant unit test stubs
-        Create a new tenant  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdMetadata unit test stubs
+        Create a metadata  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 507
+    response_status = 403
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,33 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id import delete  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id import delete  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdDeskDeskId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantId unit test stubs
-        Delete a tenant  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdDeskDeskId unit test stubs
+        Delete a desk  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 204
-    response_body = ''
+    response_status = 403
+
+
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 403
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 507
+    response_status = 403
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,33 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id import delete  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
 class TestApiProvisioningV1AdminTenantTenantIdDeskDeskId(ApiTestMixin, unittest.TestCase):
     """
     ApiProvisioningV1AdminTenantTenantIdDeskDeskId unit test stubs
-        Delete a desk  # noqa: E501
+        Get a full desk description  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 204
-    response_body = ''
+    response_status = 403
+
+
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdDeskDeskId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdDeskDeskId unit test stubs
-        Get a full desk description  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
+        Get a full user description  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_put.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id import put  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id import put  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdDeskDeskId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdMetadataMetadataId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdDeskDeskId unit test stubs
-        Edit a desk  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdMetadataMetadataId unit test stubs
+        Edit a metadata  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 507
+    response_status = 403
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_get.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_metadata import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdMetadata(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdUser(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdMetadata unit test stubs
-        List all metadata associated with the tenant  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdUser unit test stubs
+        List all users associated with the tenant  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_post.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_metadata import post  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import put  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdMetadata(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdMetadata unit test stubs
-        Create a metadata  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
+        Edit a user  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 507
+    response_status = 403
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_delete.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_get.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,33 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id import delete  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_metadata import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdMetadataMetadataId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdMetadata(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdMetadataMetadataId unit test stubs
-        Delete a metadata  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdMetadata unit test stubs
+        List all metadata associated with the tenant  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 204
-    response_body = ''
+    response_status = 403
+
+
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_get.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_get.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_put.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_delete.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,36 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id import put  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id import delete  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
 class TestApiProvisioningV1AdminTenantTenantIdMetadataMetadataId(ApiTestMixin, unittest.TestCase):
     """
     ApiProvisioningV1AdminTenantTenantIdMetadataMetadataId unit test stubs
-        Edit a metadata  # noqa: E501
+        Delete a metadata  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 507
-
-
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/test_get.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/test_get.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/test_post.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/test_post.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 507
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_delete.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_delete.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,13 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 204
-    response_body = ''
+    response_status = 403
+
+
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_get.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_get.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_put.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_put.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/test_delete.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/test_get.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,33 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_templates_template_type import delete  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_templates_template_type import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
 class TestApiProvisioningV1AdminTenantTenantIdTemplatesTemplateType(ApiTestMixin, unittest.TestCase):
     """
     ApiProvisioningV1AdminTenantTenantIdTemplatesTemplateType unit test stubs
-        Delete a custom template  # noqa: E501
+        Get a custom template  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
     response_status = 200
-    response_body = ''
+
+
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/test_get.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/test_post.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,34 +8,36 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_templates_template_type import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_templates_template_type import post  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
 class TestApiProvisioningV1AdminTenantTenantIdTemplatesTemplateType(ApiTestMixin, unittest.TestCase):
     """
     ApiProvisioningV1AdminTenantTenantIdTemplatesTemplateType unit test stubs
-        Get a custom template  # noqa: E501
+        Create a custom template  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
     response_status = 403
 
 
 
 
+
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/test_post.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/test_put.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,35 +8,36 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_templates_template_type import post  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_templates_template_type import put  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
 class TestApiProvisioningV1AdminTenantTenantIdTemplatesTemplateType(ApiTestMixin, unittest.TestCase):
     """
     ApiProvisioningV1AdminTenantTenantIdTemplatesTemplateType unit test stubs
-        Create a custom template  # noqa: E501
+        Update a custom template  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
-    response_body = ''
+    response_status = 403
+
+
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/test_put.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,35 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_templates_template_type import put  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import delete  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdTemplatesTemplateType(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdTemplatesTemplateType unit test stubs
-        Update a custom template  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
+        Remove the given user from the tenant, deleting it if it was the last tenant linked  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
-    response_body = ''
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type import post  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user import post  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdTypologyType(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdUser(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdTypologyType unit test stubs
-        Create a type  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdUser unit test stubs
+        Create a new user  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 507
+    response_status = 403
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,33 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id import delete  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtype(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeId unit test stubs
-        Delete a type  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtype unit test stubs
+        Get subtypes  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 204
-    response_body = ''
+    response_status = 403
+
+
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 403
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,34 +8,36 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype import post  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
 class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtype(ApiTestMixin, unittest.TestCase):
     """
     ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtype unit test stubs
-        Get subtypes  # noqa: E501
+        Create a subtype  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 403
+
+
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,36 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype import post  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtype(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtype unit test stubs
-        Create a subtype  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeId unit test stubs
+        Get a subtype with every information set  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 507
-
-
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,13 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 204
-    response_body = ''
+    response_status = 403
+
+
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,34 +8,36 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id import put  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
 class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeId(ApiTestMixin, unittest.TestCase):
     """
     ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeId unit test stubs
-        Get a subtype with every information set  # noqa: E501
+        Edit a subtype  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 403
+
+
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,36 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id import put  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id import delete  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeId unit test stubs
-        Edit a subtype  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeId unit test stubs
+        Delete a type  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 204
-
-
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,34 +8,36 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type import post  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdUser(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdTypologyType(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdUser unit test stubs
-        List all users associated with the tenant  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdTypologyType unit test stubs
+        Create a type  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 403
+
+
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user import post  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id import put  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdUser(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdDeskDeskId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdUser unit test stubs
-        Create a new user  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdDeskDeskId unit test stubs
+        Edit a desk  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 507
+    response_status = 403
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,33 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import delete  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import delete  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminUserUserId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
-        Remove the given user from the tenant, deleting it if it was the last tenant linked  # noqa: E501
+    ApiProvisioningV1AdminUserUserId unit test stubs
+        Delete a user  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 204
-    response_body = ''
+    response_status = 403
+
+
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminUserUserId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
-        Get a full user description  # noqa: E501
+    ApiProvisioningV1AdminUserUserId unit test stubs
+        Get a full user representation  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,36 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import put  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id import delete  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
-        Edit a user  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantId unit test stubs
+        Delete a tenant  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
-
-
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/test_get.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/test_get.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/test_delete.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/test_delete.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,13 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 204
-    response_body = ''
+    response_status = 403
+
+
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,33 +8,36 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import delete  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant import post  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminUserUserId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenant(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminUserUserId unit test stubs
-        Delete a user  # noqa: E501
+    ApiProvisioningV1AdminTenant unit test stubs
+        Create a new tenant  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
+        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 204
-    response_body = ''
+    response_status = 403
+
+
+
+
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,34 +8,36 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import put  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
 class TestApiProvisioningV1AdminUserUserId(ApiTestMixin, unittest.TestCase):
     """
     ApiProvisioningV1AdminUserUserId unit test stubs
-        Get a full user representation  # noqa: E501
+        Edit a user  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 403
+
+
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.7.4/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py` & `iparapheur-provisioning-1.7.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/test_delete.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,36 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import put  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_templates_template_type import delete  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminUserUserId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdTemplatesTemplateType(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminUserUserId unit test stubs
-        Edit a user  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdTemplatesTemplateType unit test stubs
+        Delete a custom template  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
-
-
+    response_status = 403
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

