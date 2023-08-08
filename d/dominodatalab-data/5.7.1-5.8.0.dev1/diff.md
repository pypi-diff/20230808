# Comparing `tmp/dominodatalab_data-5.7.1.tar.gz` & `tmp/dominodatalab_data-5.8.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dominodatalab_data-5.7.1.tar", max compression
+gzip compressed data, was "dominodatalab_data-5.8.0.dev1.tar", max compression
```

## Comparing `dominodatalab_data-5.7.1.tar` & `dominodatalab_data-5.8.0.dev1.tar`

### file list

```diff
@@ -1,115 +1,115 @@
--rw-r--r--   0        0        0    10891 2022-12-13 21:08:46.883572 dominodatalab_data-5.7.1/LICENSE
--rw-r--r--   0        0        0     5982 2023-07-20 22:48:08.992771 dominodatalab_data-5.7.1/README.md
--rw-r--r--   0        0        0      102 2022-12-13 21:08:46.888200 dominodatalab_data-5.7.1/datasource_api_client/__init__.py
--rw-r--r--   0        0        0       47 2022-12-13 21:08:46.888449 dominodatalab_data-5.7.1/datasource_api_client/api/__init__.py
--rw-r--r--   0        0        0        0 2022-12-13 21:08:46.888635 dominodatalab_data-5.7.1/datasource_api_client/api/datasource/__init__.py
--rw-r--r--   0        0        0     4143 2023-07-25 21:18:01.766650 dominodatalab_data-5.7.1/datasource_api_client/api/datasource/get_datasource_by_name.py
--rw-r--r--   0        0        0        0 2022-12-13 21:08:46.889007 dominodatalab_data-5.7.1/datasource_api_client/api/proxy/__init__.py
--rw-r--r--   0        0        0     3381 2023-07-25 21:18:01.766907 dominodatalab_data-5.7.1/datasource_api_client/api/proxy/get_key_url.py
--rw-r--r--   0        0        0     3434 2023-07-25 21:18:01.767159 dominodatalab_data-5.7.1/datasource_api_client/api/proxy/list_keys.py
--rw-r--r--   0        0        0     2204 2023-07-25 21:18:01.767451 dominodatalab_data-5.7.1/datasource_api_client/api/proxy/log_metric.py
--rw-r--r--   0        0        0     1661 2023-07-25 21:18:01.767728 dominodatalab_data-5.7.1/datasource_api_client/client.py
--rw-r--r--   0        0        0      695 2022-12-13 21:08:46.889828 dominodatalab_data-5.7.1/datasource_api_client/models/__init__.py
--rw-r--r--   0        0        0     1173 2022-12-13 21:08:46.890343 dominodatalab_data-5.7.1/datasource_api_client/models/datasource_config.py
--rw-r--r--   0        0        0     4708 2022-12-13 21:08:46.890492 dominodatalab_data-5.7.1/datasource_api_client/models/datasource_dto.py
--rw-r--r--   0        0        0     1199 2022-12-13 21:08:46.890641 dominodatalab_data-5.7.1/datasource_api_client/models/datasource_dto_added_by.py
--rw-r--r--   0        0        0      428 2023-07-20 22:48:08.995331 dominodatalab_data-5.7.1/datasource_api_client/models/datasource_dto_auth_type.py
--rw-r--r--   0        0        0      712 2023-07-25 21:18:01.768820 dominodatalab_data-5.7.1/datasource_api_client/models/datasource_dto_data_source_type.py
--rw-r--r--   0        0        0      170 2022-12-13 21:08:46.891095 dominodatalab_data-5.7.1/datasource_api_client/models/datasource_dto_status.py
--rw-r--r--   0        0        0     1905 2022-12-13 21:08:46.891294 dominodatalab_data-5.7.1/datasource_api_client/models/datasource_owner_info.py
--rw-r--r--   0        0        0     1498 2022-12-13 21:08:46.891428 dominodatalab_data-5.7.1/datasource_api_client/models/error_response.py
--rw-r--r--   0        0        0     3569 2022-12-13 21:08:46.891567 dominodatalab_data-5.7.1/datasource_api_client/models/key_request.py
--rw-r--r--   0        0        0     3880 2023-07-25 21:18:01.769075 dominodatalab_data-5.7.1/datasource_api_client/models/list_request.py
--rw-r--r--   0        0        0      153 2022-12-13 21:08:46.891858 dominodatalab_data-5.7.1/datasource_api_client/models/log_metric_m.py
--rw-r--r--   0        0        0      239 2022-12-13 21:08:46.891994 dominodatalab_data-5.7.1/datasource_api_client/models/log_metric_t.py
--rw-r--r--   0        0        0     2084 2022-12-13 21:08:46.892129 dominodatalab_data-5.7.1/datasource_api_client/models/proxy_error_response.py
--rw-r--r--   0        0        0      939 2023-07-20 22:48:08.996991 dominodatalab_data-5.7.1/datasource_api_client/types.py
--rw-r--r--   0        0        0      369 2022-12-13 21:08:46.893659 dominodatalab_data-5.7.1/domino_data/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 22:48:08.998268 dominodatalab_data-5.7.1/domino_data/_feature_store/__init__.py
--rw-r--r--   0        0        0     3801 2023-07-20 22:48:08.998880 dominodatalab_data-5.7.1/domino_data/_feature_store/client.py
--rw-r--r--   0        0        0      684 2023-07-20 22:48:08.999044 dominodatalab_data-5.7.1/domino_data/_feature_store/exceptions.py
--rw-r--r--   0        0        0     2966 2023-07-20 22:48:08.999763 dominodatalab_data-5.7.1/domino_data/_feature_store/git.py
--rw-r--r--   0        0        0      683 2023-07-20 22:48:09.000218 dominodatalab_data-5.7.1/domino_data/_feature_store/logging.py
--rw-r--r--   0        0        0     1223 2023-07-20 22:48:09.000513 dominodatalab_data-5.7.1/domino_data/_feature_store/run.py
--rw-r--r--   0        0        0     8180 2023-07-20 22:48:09.000922 dominodatalab_data-5.7.1/domino_data/_feature_store/sync.py
--rw-r--r--   0        0        0     4527 2023-07-20 22:48:09.001175 dominodatalab_data-5.7.1/domino_data/auth.py
--rw-r--r--   0        0        0    10464 2023-07-25 21:18:01.770172 dominodatalab_data-5.7.1/domino_data/configuration_gen.py
--rw-r--r--   0        0        0    27063 2023-07-25 21:18:01.771520 dominodatalab_data-5.7.1/domino_data/data_sources.py
--rw-r--r--   0        0        0      894 2023-01-04 19:29:57.409242 dominodatalab_data-5.7.1/domino_data/logging.py
--rw-r--r--   0        0        0        0 2022-12-13 21:08:46.895616 dominodatalab_data-5.7.1/domino_data/py.typed
--rw-r--r--   0        0        0        0 2022-12-13 21:08:46.895810 dominodatalab_data-5.7.1/domino_data/training_sets/__init__.py
--rw-r--r--   0        0        0    13955 2023-07-20 22:48:09.003049 dominodatalab_data-5.7.1/domino_data/training_sets/client.py
--rw-r--r--   0        0        0     3588 2022-12-13 21:08:46.896143 dominodatalab_data-5.7.1/domino_data/training_sets/model.py
--rw-r--r--   0        0        0     2566 2023-07-25 17:05:35.878259 dominodatalab_data-5.7.1/domino_data/transfer.py
--rw-r--r--   0        0        0      104 2023-07-20 22:48:09.003666 dominodatalab_data-5.7.1/feature_store_api_client/__init__.py
--rw-r--r--   0        0        0       47 2023-07-20 22:48:09.003784 dominodatalab_data-5.7.1/feature_store_api_client/api/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 22:48:09.003861 dominodatalab_data-5.7.1/feature_store_api_client/api/default/__init__.py
--rw-r--r--   0        0        0     2657 2023-07-20 22:48:09.003992 dominodatalab_data-5.7.1/feature_store_api_client/api/default/get.py
--rw-r--r--   0        0        0     2861 2023-07-20 22:48:09.004103 dominodatalab_data-5.7.1/feature_store_api_client/api/default/get_feature_view_name_store.py
--rw-r--r--   0        0        0     3383 2023-07-20 22:48:09.004198 dominodatalab_data-5.7.1/feature_store_api_client/api/default/post.py
--rw-r--r--   0        0        0     1870 2023-07-20 22:48:09.004458 dominodatalab_data-5.7.1/feature_store_api_client/api/default/post_featureview.py
--rw-r--r--   0        0        0     3215 2023-07-20 22:48:09.004596 dominodatalab_data-5.7.1/feature_store_api_client/api/default/post_lock.py
--rw-r--r--   0        0        0     3144 2023-07-20 22:48:09.004720 dominodatalab_data-5.7.1/feature_store_api_client/api/default/post_unlock.py
--rw-r--r--   0        0        0     1822 2023-07-20 22:48:09.004825 dominodatalab_data-5.7.1/feature_store_api_client/client.py
--rw-r--r--   0        0        0     1443 2023-07-20 22:48:09.005377 dominodatalab_data-5.7.1/feature_store_api_client/models/__init__.py
--rw-r--r--   0        0        0     2002 2023-07-20 22:48:09.005624 dominodatalab_data-5.7.1/feature_store_api_client/models/auth_config.py
--rw-r--r--   0        0        0     1513 2023-07-20 22:48:09.005775 dominodatalab_data-5.7.1/feature_store_api_client/models/auth_config_fields.py
--rw-r--r--   0        0        0     1166 2023-07-20 22:48:09.005907 dominodatalab_data-5.7.1/feature_store_api_client/models/auth_config_meta.py
--rw-r--r--   0        0        0      170 2023-07-20 22:48:09.006010 dominodatalab_data-5.7.1/feature_store_api_client/models/auth_field_name.py
--rw-r--r--   0        0        0      197 2023-07-20 22:48:09.006118 dominodatalab_data-5.7.1/feature_store_api_client/models/auth_type.py
--rw-r--r--   0        0        0      668 2023-07-20 22:48:09.006253 dominodatalab_data-5.7.1/feature_store_api_client/models/config_field_name.py
--rw-r--r--   0        0        0     2987 2023-07-20 22:48:09.006367 dominodatalab_data-5.7.1/feature_store_api_client/models/create_feature_store_request.py
--rw-r--r--   0        0        0     1323 2023-07-20 22:48:09.006521 dominodatalab_data-5.7.1/feature_store_api_client/models/create_feature_store_request_offline_store_config.py
--rw-r--r--   0        0        0     1832 2023-07-20 22:48:09.006662 dominodatalab_data-5.7.1/feature_store_api_client/models/entity.py
--rw-r--r--   0        0        0     1721 2023-07-20 22:48:09.007150 dominodatalab_data-5.7.1/feature_store_api_client/models/feature.py
--rw-r--r--   0        0        0     3878 2023-07-20 22:48:09.007262 dominodatalab_data-5.7.1/feature_store_api_client/models/feature_store.py
--rw-r--r--   0        0        0     1252 2023-07-20 22:48:09.007374 dominodatalab_data-5.7.1/feature_store_api_client/models/feature_store_offline_store_config.py
--rw-r--r--   0        0        0      175 2023-07-20 22:48:09.007477 dominodatalab_data-5.7.1/feature_store_api_client/models/feature_store_sync_result.py
--rw-r--r--   0        0        0     1148 2023-07-20 22:48:09.007807 dominodatalab_data-5.7.1/feature_store_api_client/models/feature_tags.py
--rw-r--r--   0        0        0     3863 2023-07-20 22:48:09.007951 dominodatalab_data-5.7.1/feature_store_api_client/models/feature_view.py
--rw-r--r--   0        0        0     3261 2023-07-20 22:48:09.008381 dominodatalab_data-5.7.1/feature_store_api_client/models/feature_view_request.py
--rw-r--r--   0        0        0     1209 2023-07-20 22:48:09.008486 dominodatalab_data-5.7.1/feature_store_api_client/models/feature_view_request_tags.py
--rw-r--r--   0        0        0     1171 2023-07-20 22:48:09.008653 dominodatalab_data-5.7.1/feature_store_api_client/models/feature_view_tags.py
--rw-r--r--   0        0        0     2968 2023-07-20 22:48:09.008787 dominodatalab_data-5.7.1/feature_store_api_client/models/field.py
--rw-r--r--   0        0        0      340 2023-07-20 22:48:09.008914 dominodatalab_data-5.7.1/feature_store_api_client/models/git_provider_name.py
--rw-r--r--   0        0        0     2405 2023-07-20 22:48:09.009041 dominodatalab_data-5.7.1/feature_store_api_client/models/lock_feature_store_request.py
--rw-r--r--   0        0        0     1750 2023-07-20 22:48:09.009149 dominodatalab_data-5.7.1/feature_store_api_client/models/metadata.py
--rw-r--r--   0        0        0     2552 2023-07-20 22:48:09.009252 dominodatalab_data-5.7.1/feature_store_api_client/models/offline_store_config.py
--rw-r--r--   0        0        0     1556 2023-07-20 22:48:09.009349 dominodatalab_data-5.7.1/feature_store_api_client/models/offline_store_config_fields.py
--rw-r--r--   0        0        0      219 2023-07-20 22:48:09.009470 dominodatalab_data-5.7.1/feature_store_api_client/models/offline_store_type.py
--rw-r--r--   0        0        0     1895 2023-07-20 22:48:09.009577 dominodatalab_data-5.7.1/feature_store_api_client/models/unlock_feature_store_request.py
--rw-r--r--   0        0        0     2459 2023-07-20 22:48:09.009897 dominodatalab_data-5.7.1/feature_store_api_client/models/upsert_feature_views_request.py
--rw-r--r--   0        0        0      939 2023-07-20 22:48:09.009999 dominodatalab_data-5.7.1/feature_store_api_client/types.py
--rw-r--r--   0        0        0     3858 2023-07-25 22:13:15.765438 dominodatalab_data-5.7.1/pyproject.toml
--rw-r--r--   0        0        0      103 2022-12-13 21:08:46.910476 dominodatalab_data-5.7.1/training_set_api_client/__init__.py
--rw-r--r--   0        0        0       47 2022-12-13 21:08:46.910619 dominodatalab_data-5.7.1/training_set_api_client/api/__init__.py
--rw-r--r--   0        0        0        0 2022-12-13 21:08:46.910785 dominodatalab_data-5.7.1/training_set_api_client/api/default/__init__.py
--rw-r--r--   0        0        0     1441 2022-12-13 21:08:46.910908 dominodatalab_data-5.7.1/training_set_api_client/api/default/delete_training_set_name.py
--rw-r--r--   0        0        0     1576 2022-12-13 21:08:46.911013 dominodatalab_data-5.7.1/training_set_api_client/api/default/delete_training_set_name_number.py
--rw-r--r--   0        0        0     2242 2022-12-13 21:08:46.911099 dominodatalab_data-5.7.1/training_set_api_client/api/default/get_training_set_name.py
--rw-r--r--   0        0        0     2525 2022-12-13 21:08:46.911182 dominodatalab_data-5.7.1/training_set_api_client/api/default/get_training_set_name_number.py
--rw-r--r--   0        0        0     3679 2022-12-13 21:08:46.911276 dominodatalab_data-5.7.1/training_set_api_client/api/default/post_find.py
--rw-r--r--   0        0        0     2832 2022-12-13 21:08:46.911364 dominodatalab_data-5.7.1/training_set_api_client/api/default/post_training_set_name.py
--rw-r--r--   0        0        0     3801 2022-12-13 21:08:46.911452 dominodatalab_data-5.7.1/training_set_api_client/api/default/post_version_find.py
--rw-r--r--   0        0        0     2716 2022-12-13 21:08:46.911584 dominodatalab_data-5.7.1/training_set_api_client/api/default/put_training_set_name.py
--rw-r--r--   0        0        0     3049 2022-12-13 21:08:46.911684 dominodatalab_data-5.7.1/training_set_api_client/api/default/put_training_set_name_number.py
--rw-r--r--   0        0        0     1661 2022-12-13 21:08:46.911774 dominodatalab_data-5.7.1/training_set_api_client/client.py
--rw-r--r--   0        0        0     1139 2022-12-13 21:08:46.911917 dominodatalab_data-5.7.1/training_set_api_client/models/__init__.py
--rw-r--r--   0        0        0     3301 2022-12-13 21:08:46.912007 dominodatalab_data-5.7.1/training_set_api_client/models/create_training_set_version_request.py
--rw-r--r--   0        0        0     1280 2022-12-13 21:08:46.912105 dominodatalab_data-5.7.1/training_set_api_client/models/create_training_set_version_request_meta.py
--rw-r--r--   0        0        0     1995 2022-12-13 21:08:46.912303 dominodatalab_data-5.7.1/training_set_api_client/models/monitoring_meta.py
--rw-r--r--   0        0        0     2411 2022-12-13 21:08:46.912407 dominodatalab_data-5.7.1/training_set_api_client/models/training_set.py
--rw-r--r--   0        0        0     2010 2022-12-13 21:08:46.912513 dominodatalab_data-5.7.1/training_set_api_client/models/training_set_filter.py
--rw-r--r--   0        0        0     1204 2022-12-13 21:08:46.912628 dominodatalab_data-5.7.1/training_set_api_client/models/training_set_filter_meta.py
--rw-r--r--   0        0        0     1171 2022-12-13 21:08:46.912764 dominodatalab_data-5.7.1/training_set_api_client/models/training_set_meta.py
--rw-r--r--   0        0        0     4472 2022-12-13 21:08:46.912863 dominodatalab_data-5.7.1/training_set_api_client/models/training_set_version.py
--rw-r--r--   0        0        0     2545 2022-12-13 21:08:46.912963 dominodatalab_data-5.7.1/training_set_api_client/models/training_set_version_filter.py
--rw-r--r--   0        0        0     1242 2022-12-13 21:08:46.913081 dominodatalab_data-5.7.1/training_set_api_client/models/training_set_version_filter_meta.py
--rw-r--r--   0        0        0     1303 2022-12-13 21:08:46.913192 dominodatalab_data-5.7.1/training_set_api_client/models/training_set_version_filter_training_set_meta.py
--rw-r--r--   0        0        0     1209 2022-12-13 21:08:46.913297 dominodatalab_data-5.7.1/training_set_api_client/models/training_set_version_meta.py
--rw-r--r--   0        0        0     1844 2022-12-13 21:08:46.913396 dominodatalab_data-5.7.1/training_set_api_client/models/update_training_set_request.py
--rw-r--r--   0        0        0     1242 2022-12-13 21:08:46.913504 dominodatalab_data-5.7.1/training_set_api_client/models/update_training_set_request_meta.py
--rw-r--r--   0        0        0     3070 2022-12-13 21:08:46.913600 dominodatalab_data-5.7.1/training_set_api_client/models/update_training_set_version_request.py
--rw-r--r--   0        0        0     1280 2022-12-13 21:08:46.913689 dominodatalab_data-5.7.1/training_set_api_client/models/update_training_set_version_request_meta.py
--rw-r--r--   0        0        0      984 2022-12-13 21:08:46.913773 dominodatalab_data-5.7.1/training_set_api_client/types.py
--rw-r--r--   0        0        0     7352 1970-01-01 00:00:00.000000 dominodatalab_data-5.7.1/PKG-INFO
+-rw-r--r--   0        0        0    10891 2022-06-17 19:33:52.493061 dominodatalab_data-5.8.0.dev1/LICENSE
+-rw-r--r--   0        0        0     5982 2022-06-17 19:33:52.493416 dominodatalab_data-5.8.0.dev1/README.md
+-rw-r--r--   0        0        0      102 2023-08-04 21:09:45.118077 dominodatalab_data-5.8.0.dev1/datasource_api_client/__init__.py
+-rw-r--r--   0        0        0       47 2023-08-04 21:09:45.206350 dominodatalab_data-5.8.0.dev1/datasource_api_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-04 21:09:45.255371 dominodatalab_data-5.8.0.dev1/datasource_api_client/api/datasource/__init__.py
+-rw-r--r--   0        0        0     4162 2023-08-04 21:10:19.805373 dominodatalab_data-5.8.0.dev1/datasource_api_client/api/datasource/get_datasource_by_name.py
+-rw-r--r--   0        0        0        0 2023-08-04 21:09:45.222556 dominodatalab_data-5.8.0.dev1/datasource_api_client/api/proxy/__init__.py
+-rw-r--r--   0        0        0     3389 2023-08-04 21:10:19.778411 dominodatalab_data-5.8.0.dev1/datasource_api_client/api/proxy/get_key_url.py
+-rw-r--r--   0        0        0     3442 2023-08-04 21:10:19.785898 dominodatalab_data-5.8.0.dev1/datasource_api_client/api/proxy/list_keys.py
+-rw-r--r--   0        0        0     2212 2023-08-04 21:10:19.761325 dominodatalab_data-5.8.0.dev1/datasource_api_client/api/proxy/log_metric.py
+-rw-r--r--   0        0        0     1822 2023-08-04 21:10:19.735375 dominodatalab_data-5.8.0.dev1/datasource_api_client/client.py
+-rw-r--r--   0        0        0      695 2023-08-04 21:09:45.203366 dominodatalab_data-5.8.0.dev1/datasource_api_client/models/__init__.py
+-rw-r--r--   0        0        0     1173 2023-08-04 21:10:19.712263 dominodatalab_data-5.8.0.dev1/datasource_api_client/models/datasource_config.py
+-rw-r--r--   0        0        0     4708 2023-08-04 21:10:19.823414 dominodatalab_data-5.8.0.dev1/datasource_api_client/models/datasource_dto.py
+-rw-r--r--   0        0        0     1199 2023-08-04 21:10:19.729974 dominodatalab_data-5.8.0.dev1/datasource_api_client/models/datasource_dto_added_by.py
+-rw-r--r--   0        0        0      428 2023-08-04 21:10:18.329537 dominodatalab_data-5.8.0.dev1/datasource_api_client/models/datasource_dto_auth_type.py
+-rw-r--r--   0        0        0     1156 2023-08-08 18:47:59.935595 dominodatalab_data-5.8.0.dev1/datasource_api_client/models/datasource_dto_data_source_type.py
+-rw-r--r--   0        0        0      170 2023-08-04 21:10:18.305647 dominodatalab_data-5.8.0.dev1/datasource_api_client/models/datasource_dto_status.py
+-rw-r--r--   0        0        0     1905 2023-08-04 21:10:19.771308 dominodatalab_data-5.8.0.dev1/datasource_api_client/models/datasource_owner_info.py
+-rw-r--r--   0        0        0     1498 2023-08-04 21:10:19.759530 dominodatalab_data-5.8.0.dev1/datasource_api_client/models/error_response.py
+-rw-r--r--   0        0        0     3569 2023-08-04 21:10:19.817850 dominodatalab_data-5.8.0.dev1/datasource_api_client/models/key_request.py
+-rw-r--r--   0        0        0     3583 2023-08-04 21:10:19.821109 dominodatalab_data-5.8.0.dev1/datasource_api_client/models/list_request.py
+-rw-r--r--   0        0        0      153 2023-08-04 21:10:18.316235 dominodatalab_data-5.8.0.dev1/datasource_api_client/models/log_metric_m.py
+-rw-r--r--   0        0        0      239 2023-08-04 21:10:18.319372 dominodatalab_data-5.8.0.dev1/datasource_api_client/models/log_metric_t.py
+-rw-r--r--   0        0        0     2084 2023-08-04 21:10:19.813863 dominodatalab_data-5.8.0.dev1/datasource_api_client/models/proxy_error_response.py
+-rw-r--r--   0        0        0      939 2023-08-04 21:10:19.779199 dominodatalab_data-5.8.0.dev1/datasource_api_client/types.py
+-rw-r--r--   0        0        0      369 2022-06-17 19:33:52.498752 dominodatalab_data-5.8.0.dev1/domino_data/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-01 18:54:53.831027 dominodatalab_data-5.8.0.dev1/domino_data/_feature_store/__init__.py
+-rw-r--r--   0        0        0     3801 2023-04-03 15:43:18.645563 dominodatalab_data-5.8.0.dev1/domino_data/_feature_store/client.py
+-rw-r--r--   0        0        0      684 2022-12-01 18:54:53.832478 dominodatalab_data-5.8.0.dev1/domino_data/_feature_store/exceptions.py
+-rw-r--r--   0        0        0     2966 2023-01-04 16:07:48.401852 dominodatalab_data-5.8.0.dev1/domino_data/_feature_store/git.py
+-rw-r--r--   0        0        0      683 2023-01-04 16:07:48.403057 dominodatalab_data-5.8.0.dev1/domino_data/_feature_store/logging.py
+-rw-r--r--   0        0        0     1223 2023-01-04 16:07:48.405079 dominodatalab_data-5.8.0.dev1/domino_data/_feature_store/run.py
+-rw-r--r--   0        0        0     8180 2023-04-03 15:43:18.647140 dominodatalab_data-5.8.0.dev1/domino_data/_feature_store/sync.py
+-rw-r--r--   0        0        0     4527 2022-11-01 18:48:22.635731 dominodatalab_data-5.8.0.dev1/domino_data/auth.py
+-rw-r--r--   0        0        0    14312 2023-08-08 18:47:59.936750 dominodatalab_data-5.8.0.dev1/domino_data/configuration_gen.py
+-rw-r--r--   0        0        0    27235 2023-07-31 21:24:56.045465 dominodatalab_data-5.8.0.dev1/domino_data/data_sources.py
+-rw-r--r--   0        0        0      894 2023-01-04 16:07:48.407684 dominodatalab_data-5.8.0.dev1/domino_data/logging.py
+-rw-r--r--   0        0        0        0 2022-06-17 19:33:52.499858 dominodatalab_data-5.8.0.dev1/domino_data/py.typed
+-rw-r--r--   0        0        0        0 2022-06-17 19:33:52.500015 dominodatalab_data-5.8.0.dev1/domino_data/training_sets/__init__.py
+-rw-r--r--   0        0        0    13955 2022-11-01 18:48:22.638301 dominodatalab_data-5.8.0.dev1/domino_data/training_sets/client.py
+-rw-r--r--   0        0        0     3588 2022-06-17 19:33:52.500395 dominodatalab_data-5.8.0.dev1/domino_data/training_sets/model.py
+-rw-r--r--   0        0        0     2566 2023-07-25 18:20:36.202155 dominodatalab_data-5.8.0.dev1/domino_data/transfer.py
+-rw-r--r--   0        0        0      104 2023-03-22 20:55:07.504701 dominodatalab_data-5.8.0.dev1/feature_store_api_client/__init__.py
+-rw-r--r--   0        0        0       47 2023-03-22 20:55:07.608604 dominodatalab_data-5.8.0.dev1/feature_store_api_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-22 20:55:07.642166 dominodatalab_data-5.8.0.dev1/feature_store_api_client/api/default/__init__.py
+-rw-r--r--   0        0        0     2657 2023-03-22 20:55:43.492057 dominodatalab_data-5.8.0.dev1/feature_store_api_client/api/default/get.py
+-rw-r--r--   0        0        0     2861 2023-03-22 20:55:43.484056 dominodatalab_data-5.8.0.dev1/feature_store_api_client/api/default/get_feature_view_name_store.py
+-rw-r--r--   0        0        0     3383 2023-03-22 20:55:43.517321 dominodatalab_data-5.8.0.dev1/feature_store_api_client/api/default/post.py
+-rw-r--r--   0        0        0     1870 2023-03-22 20:55:43.459031 dominodatalab_data-5.8.0.dev1/feature_store_api_client/api/default/post_featureview.py
+-rw-r--r--   0        0        0     3215 2023-03-22 20:55:43.522840 dominodatalab_data-5.8.0.dev1/feature_store_api_client/api/default/post_lock.py
+-rw-r--r--   0        0        0     3144 2023-03-22 20:55:43.523213 dominodatalab_data-5.8.0.dev1/feature_store_api_client/api/default/post_unlock.py
+-rw-r--r--   0        0        0     1822 2023-03-22 20:55:43.469889 dominodatalab_data-5.8.0.dev1/feature_store_api_client/client.py
+-rw-r--r--   0        0        0     1443 2023-03-22 20:55:42.273428 dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/__init__.py
+-rw-r--r--   0        0        0     2002 2023-03-22 20:55:43.488903 dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/auth_config.py
+-rw-r--r--   0        0        0     1513 2023-03-22 20:55:43.471506 dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/auth_config_fields.py
+-rw-r--r--   0        0        0     1166 2023-03-22 20:55:43.485806 dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/auth_config_meta.py
+-rw-r--r--   0        0        0      170 2023-03-22 20:55:42.266939 dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/auth_field_name.py
+-rw-r--r--   0        0        0      197 2023-03-22 20:55:42.238844 dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/auth_type.py
+-rw-r--r--   0        0        0      668 2023-03-22 20:55:42.288884 dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/config_field_name.py
+-rw-r--r--   0        0        0     2987 2023-03-22 20:55:43.591807 dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/create_feature_store_request.py
+-rw-r--r--   0        0        0     1323 2023-03-22 20:55:43.538533 dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/create_feature_store_request_offline_store_config.py
+-rw-r--r--   0        0        0     1832 2023-03-22 20:55:43.581484 dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/entity.py
+-rw-r--r--   0        0        0     1721 2023-03-22 20:55:43.578194 dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/feature.py
+-rw-r--r--   0        0        0     3878 2023-03-22 20:55:43.649694 dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/feature_store.py
+-rw-r--r--   0        0        0     1252 2023-03-22 20:55:43.558771 dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/feature_store_offline_store_config.py
+-rw-r--r--   0        0        0      175 2023-03-22 20:55:42.320963 dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/feature_store_sync_result.py
+-rw-r--r--   0        0        0     1148 2023-03-22 20:55:43.562270 dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/feature_tags.py
+-rw-r--r--   0        0        0     3863 2023-03-22 20:55:43.690892 dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/feature_view.py
+-rw-r--r--   0        0        0     3261 2023-03-22 20:55:43.682470 dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/feature_view_request.py
+-rw-r--r--   0        0        0     1209 2023-03-22 20:55:43.591240 dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/feature_view_request_tags.py
+-rw-r--r--   0        0        0     1171 2023-03-22 20:55:43.590373 dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/feature_view_tags.py
+-rw-r--r--   0        0        0     2968 2023-03-22 20:55:43.689231 dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/field.py
+-rw-r--r--   0        0        0      340 2023-03-22 20:55:42.291611 dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/git_provider_name.py
+-rw-r--r--   0        0        0     2405 2023-03-22 20:55:43.681639 dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/lock_feature_store_request.py
+-rw-r--r--   0        0        0     1750 2023-03-22 20:55:43.658307 dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/metadata.py
+-rw-r--r--   0        0        0     2552 2023-03-22 20:55:43.688892 dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/offline_store_config.py
+-rw-r--r--   0        0        0     1556 2023-03-22 20:55:43.672272 dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/offline_store_config_fields.py
+-rw-r--r--   0        0        0      219 2023-03-22 20:55:42.310466 dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/offline_store_type.py
+-rw-r--r--   0        0        0     1895 2023-03-22 20:55:43.683506 dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/unlock_feature_store_request.py
+-rw-r--r--   0        0        0     2459 2023-04-03 15:43:18.647763 dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/upsert_feature_views_request.py
+-rw-r--r--   0        0        0      939 2023-03-22 20:55:43.653052 dominodatalab_data-5.8.0.dev1/feature_store_api_client/types.py
+-rw-r--r--   0        0        0     3862 2023-07-25 18:20:36.206005 dominodatalab_data-5.8.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0      103 2022-06-17 19:33:52.511546 dominodatalab_data-5.8.0.dev1/training_set_api_client/__init__.py
+-rw-r--r--   0        0        0       47 2022-06-17 19:33:52.511807 dominodatalab_data-5.8.0.dev1/training_set_api_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2022-06-17 19:33:52.511995 dominodatalab_data-5.8.0.dev1/training_set_api_client/api/default/__init__.py
+-rw-r--r--   0        0        0     1441 2022-06-17 19:33:52.512214 dominodatalab_data-5.8.0.dev1/training_set_api_client/api/default/delete_training_set_name.py
+-rw-r--r--   0        0        0     1576 2022-06-17 19:33:52.512390 dominodatalab_data-5.8.0.dev1/training_set_api_client/api/default/delete_training_set_name_number.py
+-rw-r--r--   0        0        0     2242 2022-06-17 19:33:52.512565 dominodatalab_data-5.8.0.dev1/training_set_api_client/api/default/get_training_set_name.py
+-rw-r--r--   0        0        0     2525 2022-06-17 19:33:52.512716 dominodatalab_data-5.8.0.dev1/training_set_api_client/api/default/get_training_set_name_number.py
+-rw-r--r--   0        0        0     3679 2022-06-17 19:33:52.512881 dominodatalab_data-5.8.0.dev1/training_set_api_client/api/default/post_find.py
+-rw-r--r--   0        0        0     2832 2022-06-17 19:33:52.513035 dominodatalab_data-5.8.0.dev1/training_set_api_client/api/default/post_training_set_name.py
+-rw-r--r--   0        0        0     3801 2022-06-17 19:33:52.513198 dominodatalab_data-5.8.0.dev1/training_set_api_client/api/default/post_version_find.py
+-rw-r--r--   0        0        0     2716 2022-06-17 19:33:52.513339 dominodatalab_data-5.8.0.dev1/training_set_api_client/api/default/put_training_set_name.py
+-rw-r--r--   0        0        0     3049 2022-06-17 19:33:52.513478 dominodatalab_data-5.8.0.dev1/training_set_api_client/api/default/put_training_set_name_number.py
+-rw-r--r--   0        0        0     1661 2022-06-17 19:33:52.513626 dominodatalab_data-5.8.0.dev1/training_set_api_client/client.py
+-rw-r--r--   0        0        0     1139 2022-06-17 19:33:52.513861 dominodatalab_data-5.8.0.dev1/training_set_api_client/models/__init__.py
+-rw-r--r--   0        0        0     3301 2022-06-17 19:33:52.514040 dominodatalab_data-5.8.0.dev1/training_set_api_client/models/create_training_set_version_request.py
+-rw-r--r--   0        0        0     1280 2022-06-17 19:33:52.514213 dominodatalab_data-5.8.0.dev1/training_set_api_client/models/create_training_set_version_request_meta.py
+-rw-r--r--   0        0        0     1995 2022-06-17 19:33:52.514387 dominodatalab_data-5.8.0.dev1/training_set_api_client/models/monitoring_meta.py
+-rw-r--r--   0        0        0     2411 2022-06-17 19:33:52.514750 dominodatalab_data-5.8.0.dev1/training_set_api_client/models/training_set.py
+-rw-r--r--   0        0        0     2010 2022-06-17 19:33:52.515025 dominodatalab_data-5.8.0.dev1/training_set_api_client/models/training_set_filter.py
+-rw-r--r--   0        0        0     1204 2022-06-17 19:33:52.515206 dominodatalab_data-5.8.0.dev1/training_set_api_client/models/training_set_filter_meta.py
+-rw-r--r--   0        0        0     1171 2022-06-17 19:33:52.515360 dominodatalab_data-5.8.0.dev1/training_set_api_client/models/training_set_meta.py
+-rw-r--r--   0        0        0     4472 2022-06-17 19:33:52.515516 dominodatalab_data-5.8.0.dev1/training_set_api_client/models/training_set_version.py
+-rw-r--r--   0        0        0     2545 2022-06-17 19:33:52.515673 dominodatalab_data-5.8.0.dev1/training_set_api_client/models/training_set_version_filter.py
+-rw-r--r--   0        0        0     1242 2022-06-17 19:33:52.515825 dominodatalab_data-5.8.0.dev1/training_set_api_client/models/training_set_version_filter_meta.py
+-rw-r--r--   0        0        0     1303 2022-06-17 19:33:52.515970 dominodatalab_data-5.8.0.dev1/training_set_api_client/models/training_set_version_filter_training_set_meta.py
+-rw-r--r--   0        0        0     1209 2022-06-17 19:33:52.516132 dominodatalab_data-5.8.0.dev1/training_set_api_client/models/training_set_version_meta.py
+-rw-r--r--   0        0        0     1844 2022-06-17 19:33:52.516276 dominodatalab_data-5.8.0.dev1/training_set_api_client/models/update_training_set_request.py
+-rw-r--r--   0        0        0     1242 2022-06-17 19:33:52.516430 dominodatalab_data-5.8.0.dev1/training_set_api_client/models/update_training_set_request_meta.py
+-rw-r--r--   0        0        0     3070 2022-06-17 19:33:52.516575 dominodatalab_data-5.8.0.dev1/training_set_api_client/models/update_training_set_version_request.py
+-rw-r--r--   0        0        0     1280 2022-06-17 19:33:52.516715 dominodatalab_data-5.8.0.dev1/training_set_api_client/models/update_training_set_version_request_meta.py
+-rw-r--r--   0        0        0      984 2022-06-17 19:33:52.516851 dominodatalab_data-5.8.0.dev1/training_set_api_client/types.py
+-rw-r--r--   0        0        0     7366 1970-01-01 00:00:00.000000 dominodatalab_data-5.8.0.dev1/PKG-INFO
```

### Comparing `dominodatalab_data-5.7.1/LICENSE` & `dominodatalab_data-5.8.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/README.md` & `dominodatalab_data-5.8.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/datasource_api_client/api/datasource/get_datasource_by_name.py` & `dominodatalab_data-5.8.0.dev1/datasource_api_client/api/datasource/get_datasource_by_name.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 def _get_kwargs(
     name: str,
     *,
     client: Client,
     run_id: Union[Unset, None, str] = UNSET,
 ) -> Dict[str, Any]:
-    url = f"{client.base_url}/datasource/name/{name}"
+    url = "{}/datasource/name/{name}".format(client.base_url, name=name)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
     params["runId"] = run_id
```

### Comparing `dominodatalab_data-5.7.1/datasource_api_client/api/proxy/get_key_url.py` & `dominodatalab_data-5.8.0.dev1/datasource_api_client/api/proxy/get_key_url.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 def _get_kwargs(
     *,
     client: Client,
     json_body: KeyRequest,
 ) -> Dict[str, Any]:
-    url = f"{client.base_url}/objectstore/key"
+    url = "{}/objectstore/key".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     json_json_body = json_body.to_dict()
 
     return {
```

### Comparing `dominodatalab_data-5.7.1/datasource_api_client/api/proxy/list_keys.py` & `dominodatalab_data-5.8.0.dev1/datasource_api_client/api/proxy/list_keys.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 def _get_kwargs(
     *,
     client: Client,
     json_body: ListRequest,
 ) -> Dict[str, Any]:
-    url = f"{client.base_url}/objectstore/list"
+    url = "{}/objectstore/list".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     json_json_body = json_body.to_dict()
 
     return {
```

### Comparing `dominodatalab_data-5.7.1/datasource_api_client/api/proxy/log_metric.py` & `dominodatalab_data-5.8.0.dev1/datasource_api_client/api/proxy/log_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 def _get_kwargs(
     *,
     client: Client,
     t: LogMetricT,
     b: int,
     m: LogMetricM,
 ) -> Dict[str, Any]:
-    url = f"{client.base_url}/objectstore/metric"
+    url = "{}/objectstore/metric".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
     json_t = t.value
```

### Comparing `dominodatalab_data-5.7.1/datasource_api_client/client.py` & `dominodatalab_data-5.8.0.dev1/training_set_api_client/client.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/datasource_api_client/models/__init__.py` & `dominodatalab_data-5.8.0.dev1/datasource_api_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/datasource_api_client/models/datasource_config.py` & `dominodatalab_data-5.8.0.dev1/datasource_api_client/models/datasource_config.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/datasource_api_client/models/datasource_dto.py` & `dominodatalab_data-5.8.0.dev1/datasource_api_client/models/datasource_dto.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/datasource_api_client/models/datasource_dto_added_by.py` & `dominodatalab_data-5.8.0.dev1/datasource_api_client/models/datasource_dto_added_by.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/datasource_api_client/models/datasource_owner_info.py` & `dominodatalab_data-5.8.0.dev1/datasource_api_client/models/datasource_owner_info.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/datasource_api_client/models/error_response.py` & `dominodatalab_data-5.8.0.dev1/datasource_api_client/models/error_response.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/datasource_api_client/models/key_request.py` & `dominodatalab_data-5.8.0.dev1/datasource_api_client/models/key_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/datasource_api_client/models/list_request.py` & `dominodatalab_data-5.8.0.dev1/datasource_api_client/models/list_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,63 +10,62 @@
 
 @attr.s(auto_attribs=True)
 class ListRequest:
     """
     Attributes:
         datasource_id (str):
         prefix (str):
-        page_size (int):
         config_overwrites (Union[Unset, DatasourceConfig]):
         credential_overwrites (Union[Unset, DatasourceConfig]):
+        page_size (Union[Unset, int]):
     """
 
     datasource_id: str
     prefix: str
-    page_size: int
     config_overwrites: Union[Unset, DatasourceConfig] = UNSET
     credential_overwrites: Union[Unset, DatasourceConfig] = UNSET
+    page_size: Union[Unset, int] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         datasource_id = self.datasource_id
         prefix = self.prefix
-        page_size = self.page_size
         config_overwrites: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.config_overwrites, Unset):
             config_overwrites = self.config_overwrites.to_dict()
 
         credential_overwrites: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.credential_overwrites, Unset):
             credential_overwrites = self.credential_overwrites.to_dict()
 
+        page_size = self.page_size
+
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "datasourceId": datasource_id,
                 "prefix": prefix,
-                "page_size": page_size,
             }
         )
         if config_overwrites is not UNSET:
             field_dict["configOverwrites"] = config_overwrites
         if credential_overwrites is not UNSET:
             field_dict["credentialOverwrites"] = credential_overwrites
+        if page_size is not UNSET:
+            field_dict["pageSize"] = page_size
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         datasource_id = d.pop("datasourceId")
+
         prefix = d.pop("prefix")
-        if "page_size" in d:
-            page_size = d.pop("page_size")
-        else:
-            page_size = None
 
         _config_overwrites = d.pop("configOverwrites", UNSET)
         config_overwrites: Union[Unset, DatasourceConfig]
         if isinstance(_config_overwrites, Unset):
             config_overwrites = UNSET
         else:
             config_overwrites = DatasourceConfig.from_dict(_config_overwrites)
@@ -74,29 +73,23 @@
         _credential_overwrites = d.pop("credentialOverwrites", UNSET)
         credential_overwrites: Union[Unset, DatasourceConfig]
         if isinstance(_credential_overwrites, Unset):
             credential_overwrites = UNSET
         else:
             credential_overwrites = DatasourceConfig.from_dict(_credential_overwrites)
 
-        if page_size is None:
-            list_request = cls(
-                datasource_id=datasource_id,
-                prefix=prefix,
-                config_overwrites=config_overwrites,
-                credential_overwrites=credential_overwrites,
-            )
-        else:
-            list_request = cls(
-                datasource_id=datasource_id,
-                prefix=prefix,
-                page_size=page_size,
-                config_overwrites=config_overwrites,
-                credential_overwrites=credential_overwrites,
-            )
+        page_size = d.pop("pageSize", UNSET)
+
+        list_request = cls(
+            datasource_id=datasource_id,
+            prefix=prefix,
+            config_overwrites=config_overwrites,
+            credential_overwrites=credential_overwrites,
+            page_size=page_size,
+        )
 
         list_request.additional_properties = d
         return list_request
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
```

### Comparing `dominodatalab_data-5.7.1/datasource_api_client/models/proxy_error_response.py` & `dominodatalab_data-5.8.0.dev1/datasource_api_client/models/proxy_error_response.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/datasource_api_client/types.py` & `dominodatalab_data-5.8.0.dev1/datasource_api_client/types.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/domino_data/_feature_store/client.py` & `dominodatalab_data-5.8.0.dev1/domino_data/_feature_store/client.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/domino_data/_feature_store/exceptions.py` & `dominodatalab_data-5.8.0.dev1/domino_data/_feature_store/exceptions.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/domino_data/_feature_store/git.py` & `dominodatalab_data-5.8.0.dev1/domino_data/_feature_store/git.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/domino_data/_feature_store/logging.py` & `dominodatalab_data-5.8.0.dev1/domino_data/_feature_store/logging.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/domino_data/_feature_store/run.py` & `dominodatalab_data-5.8.0.dev1/domino_data/_feature_store/run.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/domino_data/_feature_store/sync.py` & `dominodatalab_data-5.8.0.dev1/domino_data/_feature_store/sync.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/domino_data/auth.py` & `dominodatalab_data-5.8.0.dev1/domino_data/auth.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/domino_data/configuration_gen.py` & `dominodatalab_data-5.8.0.dev1/domino_data/configuration_gen.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Code generated by gen.py; DO NOT EDIT.
 This file was generated by robots at
-2022-12-21 20:33:45.427061"""
+2023-08-04 21:24:25.982748"""
 from typing import Any, Dict, Optional, Union
 
 from enum import Enum
 from importlib import import_module
 
 import attr
 
@@ -69,14 +69,15 @@
     HOST = "host"
     PORT = "port"
     PROJECT = "project"
     REGION = "region"
     ROLE = "role"
     SCHEMA = "schema"
     WAREHOUSE = "warehouse"
+    CATALOGCODE = "catalogCode"
 
 
 class CredElem(Enum):
     """Enumeration of valid credential elements."""
 
     ACCESSKEY = "accessKey"
     ACCESSKEYID = "accessKeyID"
@@ -123,35 +124,91 @@
 
     gcp_project_id: Optional[str] = _config(elem=ConfigElem.PROJECT)
 
     private_key_json: Optional[str] = _cred(elem=CredElem.PRIVATEKEY)
 
 
 @attr.s(auto_attribs=True)
+class ClickHouseConfig(Config):
+    """ClickHouseConfig datasource configuration."""
+
+    username: Optional[str] = _cred(elem=CredElem.USERNAME)
+    password: Optional[str] = _cred(elem=CredElem.PASSWORD)
+
+
+@attr.s(auto_attribs=True)
+class DB2Config(Config):
+    """DB2Config datasource configuration."""
+
+    username: Optional[str] = _cred(elem=CredElem.USERNAME)
+    password: Optional[str] = _cred(elem=CredElem.PASSWORD)
+
+
+@attr.s(auto_attribs=True)
+class DruidConfig(Config):
+    """DruidConfig datasource configuration."""
+
+    username: Optional[str] = _cred(elem=CredElem.USERNAME)
+    password: Optional[str] = _cred(elem=CredElem.PASSWORD)
+
+
+@attr.s(auto_attribs=True)
 class GCSConfig(Config):
     """GCSConfig datasource configuration."""
 
     bucket: Optional[str] = _config(elem=ConfigElem.BUCKET)
 
     private_key_json: Optional[str] = _cred(elem=CredElem.PRIVATEKEY)
 
 
 @attr.s(auto_attribs=True)
+class GenericJDBCConfig(Config):
+    """GenericJDBCConfig datasource configuration."""
+
+    username: Optional[str] = _cred(elem=CredElem.USERNAME)
+    password: Optional[str] = _cred(elem=CredElem.PASSWORD)
+
+
+@attr.s(auto_attribs=True)
 class GenericS3Config(Config):
     """GenericS3Config datasource configuration."""
 
     bucket: Optional[str] = _config(elem=ConfigElem.BUCKET)
     host: Optional[str] = _config(elem=ConfigElem.HOST)
     region: Optional[str] = _config(elem=ConfigElem.REGION)
 
     aws_access_key_id: Optional[str] = _cred(elem=CredElem.ACCESSKEYID)
     aws_secret_access_key: Optional[str] = _cred(elem=CredElem.SECRETACCESSKEY)
 
 
 @attr.s(auto_attribs=True)
+class GreenplumConfig(Config):
+    """GreenplumConfig datasource configuration."""
+
+    username: Optional[str] = _cred(elem=CredElem.USERNAME)
+    password: Optional[str] = _cred(elem=CredElem.PASSWORD)
+
+
+@attr.s(auto_attribs=True)
+class IgniteConfig(Config):
+    """IgniteConfig datasource configuration."""
+
+    username: Optional[str] = _cred(elem=CredElem.USERNAME)
+    password: Optional[str] = _cred(elem=CredElem.PASSWORD)
+
+
+@attr.s(auto_attribs=True)
+class MariaDBConfig(Config):
+    """MariaDBConfig datasource configuration."""
+
+    username: Optional[str] = _cred(elem=CredElem.USERNAME)
+    password: Optional[str] = _cred(elem=CredElem.PASSWORD)
+
+
+@attr.s(auto_attribs=True)
 class MongoDBConfig(Config):
     """MongoDBConfig datasource configuration."""
 
     username: Optional[str] = _cred(elem=CredElem.USERNAME)
     password: Optional[str] = _cred(elem=CredElem.PASSWORD)
 
 
@@ -166,24 +223,40 @@
     password: Optional[str] = _cred(elem=CredElem.PASSWORD)
     aws_access_key_id: Optional[str] = _cred(elem=CredElem.ACCESSKEYID)
     aws_secret_access_key: Optional[str] = _cred(elem=CredElem.SECRETACCESSKEY)
     aws_session_token: Optional[str] = _cred(elem=CredElem.SESSIONTOKEN)
 
 
 @attr.s(auto_attribs=True)
+class NetezzaConfig(Config):
+    """NetezzaConfig datasource configuration."""
+
+    username: Optional[str] = _cred(elem=CredElem.USERNAME)
+    password: Optional[str] = _cred(elem=CredElem.PASSWORD)
+
+
+@attr.s(auto_attribs=True)
 class OracleConfig(Config):
     """OracleConfig datasource configuration."""
 
     database: Optional[str] = _config(elem=ConfigElem.DATABASE)
 
     username: Optional[str] = _cred(elem=CredElem.USERNAME)
     password: Optional[str] = _cred(elem=CredElem.PASSWORD)
 
 
 @attr.s(auto_attribs=True)
+class PalantirConfig(Config):
+    """PalantirConfig datasource configuration."""
+
+    client_id: Optional[str] = _cred(elem=CredElem.CLIENTID)
+    client_secret: Optional[str] = _cred(elem=CredElem.CLIENTSECRET)
+
+
+@attr.s(auto_attribs=True)
 class PostgreSQLConfig(Config):
     """PostgreSQLConfig datasource configuration."""
 
     database: Optional[str] = _config(elem=ConfigElem.DATABASE)
     region: Optional[str] = _config(elem=ConfigElem.REGION)
 
     username: Optional[str] = _cred(elem=CredElem.USERNAME)
@@ -216,14 +289,30 @@
 
     aws_access_key_id: Optional[str] = _cred(elem=CredElem.ACCESSKEYID)
     aws_secret_access_key: Optional[str] = _cred(elem=CredElem.SECRETACCESSKEY)
     aws_session_token: Optional[str] = _cred(elem=CredElem.SESSIONTOKEN)
 
 
 @attr.s(auto_attribs=True)
+class SAPHanaConfig(Config):
+    """SAPHanaConfig datasource configuration."""
+
+    username: Optional[str] = _cred(elem=CredElem.USERNAME)
+    password: Optional[str] = _cred(elem=CredElem.PASSWORD)
+
+
+@attr.s(auto_attribs=True)
+class SingleStoreConfig(Config):
+    """SingleStoreConfig datasource configuration."""
+
+    username: Optional[str] = _cred(elem=CredElem.USERNAME)
+    password: Optional[str] = _cred(elem=CredElem.PASSWORD)
+
+
+@attr.s(auto_attribs=True)
 class SQLServerConfig(Config):
     """SQLServerConfig datasource configuration."""
 
     database: Optional[str] = _config(elem=ConfigElem.DATABASE)
 
     username: Optional[str] = _cred(elem=CredElem.USERNAME)
     password: Optional[str] = _cred(elem=CredElem.PASSWORD)
@@ -240,14 +329,22 @@
 
     username: Optional[str] = _cred(elem=CredElem.USERNAME)
     password: Optional[str] = _cred(elem=CredElem.PASSWORD)
     token: Optional[str] = _cred(elem=CredElem.TOKEN)
 
 
 @attr.s(auto_attribs=True)
+class SynapseConfig(Config):
+    """SynapseConfig datasource configuration."""
+
+    username: Optional[str] = _cred(elem=CredElem.USERNAME)
+    password: Optional[str] = _cred(elem=CredElem.PASSWORD)
+
+
+@attr.s(auto_attribs=True)
 class TabularS3GlueConfig(Config):
     """TabularS3GlueConfig datasource configuration."""
 
     database: Optional[str] = _config(elem=ConfigElem.DATABASE)
     region: Optional[str] = _config(elem=ConfigElem.REGION)
 
 
@@ -267,58 +364,82 @@
     schema: Optional[str] = _config(elem=ConfigElem.SCHEMA)
 
     username: Optional[str] = _cred(elem=CredElem.USERNAME)
     password: Optional[str] = _cred(elem=CredElem.PASSWORD)
 
 
 @attr.s(auto_attribs=True)
-class PalantirConfig(Config):
-    """PalantirConfig datasource configuration."""
+class VerticaConfig(Config):
+    """VerticaConfig datasource configuration."""
 
-    client_id: Optional[str] = _cred(elem=CredElem.CLIENTID)
-    client_secret: Optional[str] = _cred(elem=CredElem.CLIENTSECRET)
+    username: Optional[str] = _cred(elem=CredElem.USERNAME)
+    password: Optional[str] = _cred(elem=CredElem.PASSWORD)
 
 
 DatasourceConfig = Union[
     ADLSConfig,
     BigQueryConfig,
+    ClickHouseConfig,
+    DB2Config,
+    DruidConfig,
     GCSConfig,
+    GenericJDBCConfig,
     GenericS3Config,
+    GreenplumConfig,
+    IgniteConfig,
+    MariaDBConfig,
     MongoDBConfig,
     MySQLConfig,
+    NetezzaConfig,
     OracleConfig,
+    PalantirConfig,
     PostgreSQLConfig,
     RedshiftConfig,
     S3Config,
+    SAPHanaConfig,
+    SingleStoreConfig,
     SQLServerConfig,
     SnowflakeConfig,
+    SynapseConfig,
     TabularS3GlueConfig,
     TeradataConfig,
     TrinoConfig,
-    PalantirConfig,
+    VerticaConfig,
     Config,
 ]
 
 DATASOURCES = {
     DatasourceDtoDataSourceType.ADLSCONFIG: "ObjectStoreDatasource",
     DatasourceDtoDataSourceType.BIGQUERYCONFIG: "TabularDatasource",
+    DatasourceDtoDataSourceType.CLICKHOUSECONFIG: "TabularDatasource",
+    DatasourceDtoDataSourceType.DB2CONFIG: "TabularDatasource",
+    DatasourceDtoDataSourceType.DRUIDCONFIG: "TabularDatasource",
     DatasourceDtoDataSourceType.GCSCONFIG: "ObjectStoreDatasource",
+    DatasourceDtoDataSourceType.GENERICJDBCCONFIG: "TabularDatasource",
     DatasourceDtoDataSourceType.GENERICS3CONFIG: "ObjectStoreDatasource",
+    DatasourceDtoDataSourceType.GREENPLUMCONFIG: "TabularDatasource",
+    DatasourceDtoDataSourceType.IGNITECONFIG: "TabularDatasource",
+    DatasourceDtoDataSourceType.MARIADBCONFIG: "TabularDatasource",
     DatasourceDtoDataSourceType.MONGODBCONFIG: "TabularDatasource",
     DatasourceDtoDataSourceType.MYSQLCONFIG: "TabularDatasource",
+    DatasourceDtoDataSourceType.NETEZZACONFIG: "TabularDatasource",
     DatasourceDtoDataSourceType.ORACLECONFIG: "TabularDatasource",
+    DatasourceDtoDataSourceType.PALANTIRCONFIG: "TabularDatasource",
     DatasourceDtoDataSourceType.POSTGRESQLCONFIG: "TabularDatasource",
     DatasourceDtoDataSourceType.REDSHIFTCONFIG: "TabularDatasource",
     DatasourceDtoDataSourceType.S3CONFIG: "ObjectStoreDatasource",
+    DatasourceDtoDataSourceType.SAPHANACONFIG: "TabularDatasource",
+    DatasourceDtoDataSourceType.SINGLESTORECONFIG: "TabularDatasource",
     DatasourceDtoDataSourceType.SQLSERVERCONFIG: "TabularDatasource",
     DatasourceDtoDataSourceType.SNOWFLAKECONFIG: "TabularDatasource",
+    DatasourceDtoDataSourceType.SYNAPSECONFIG: "TabularDatasource",
     DatasourceDtoDataSourceType.TABULARS3GLUECONFIG: "TabularDatasource",
     DatasourceDtoDataSourceType.TERADATACONFIG: "TabularDatasource",
     DatasourceDtoDataSourceType.TRINOCONFIG: "TabularDatasource",
-    DatasourceDtoDataSourceType.PALANTIRCONFIG: "TabularDatasource",
+    DatasourceDtoDataSourceType.VERTICACONFIG: "TabularDatasource",
 }
 
 
 def find_datasource_klass(datasource_type: DatasourceDtoDataSourceType) -> Any:
     """Find according datasource class."""
     mod = import_module("domino_data.data_sources")
     return getattr(mod, DATASOURCES[datasource_type])
```

### Comparing `dominodatalab_data-5.7.1/domino_data/data_sources.py` & `dominodatalab_data-5.8.0.dev1/domino_data/data_sources.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,15 +247,14 @@
     """
     token_url = os.getenv("DOMINO_API_PROXY", "")
     if token_url:
         try:
             jwt = get_jwt_token(token_url)
         except httpx.HTTPStatusError:
             logger.opt(exception=True).warning("Failed to get token from sidecar container API")
-            pass
         else:
             return {CredElem.TOKEN.value: jwt}
 
     location = os.getenv("DOMINO_TOKEN_FILE", DOMINO_TOKEN_DEFAULT_LOCATION)
     try:
         with open(location, encoding="ascii") as token_file:
             return {CredElem.TOKEN.value: token_file.readline().rstrip()}
@@ -635,15 +634,20 @@
         if response.status_code == 200:
             datasource_dto = cast(DatasourceDto, response.parsed)
             datasource_klass = cast(
                 Datasource, find_datasource_klass(datasource_dto.data_source_type)
             )
             return datasource_klass.from_dto(self, datasource_dto)
 
-        message = cast(ErrorResponse, response.parsed).message
+        error_response = cast(ErrorResponse, response.parsed)
+        message = (
+            f"Received unexpected response while getting data source: {response}"
+            if error_response is None
+            else error_response.message
+        )
         logger.exception(message)
         raise Exception(message)
 
     @backoff.on_exception(backoff.expo, UnauthenticatedError, max_time=60)
     def list_keys(
         self,
         datasource_id: str,
```

### Comparing `dominodatalab_data-5.7.1/domino_data/logging.py` & `dominodatalab_data-5.8.0.dev1/domino_data/logging.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/domino_data/training_sets/client.py` & `dominodatalab_data-5.8.0.dev1/domino_data/training_sets/client.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/domino_data/training_sets/model.py` & `dominodatalab_data-5.8.0.dev1/domino_data/training_sets/model.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/domino_data/transfer.py` & `dominodatalab_data-5.8.0.dev1/domino_data/transfer.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/feature_store_api_client/api/default/get.py` & `dominodatalab_data-5.8.0.dev1/feature_store_api_client/api/default/get.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/feature_store_api_client/api/default/get_feature_view_name_store.py` & `dominodatalab_data-5.8.0.dev1/feature_store_api_client/api/default/get_feature_view_name_store.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/feature_store_api_client/api/default/post.py` & `dominodatalab_data-5.8.0.dev1/feature_store_api_client/api/default/post.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/feature_store_api_client/api/default/post_featureview.py` & `dominodatalab_data-5.8.0.dev1/feature_store_api_client/api/default/post_featureview.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/feature_store_api_client/api/default/post_lock.py` & `dominodatalab_data-5.8.0.dev1/feature_store_api_client/api/default/post_lock.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/feature_store_api_client/api/default/post_unlock.py` & `dominodatalab_data-5.8.0.dev1/feature_store_api_client/api/default/post_unlock.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/feature_store_api_client/client.py` & `dominodatalab_data-5.8.0.dev1/datasource_api_client/client.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/feature_store_api_client/models/__init__.py` & `dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/feature_store_api_client/models/auth_config.py` & `dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/auth_config.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/feature_store_api_client/models/auth_config_fields.py` & `dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/auth_config_fields.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/feature_store_api_client/models/auth_config_meta.py` & `dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/auth_config_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/feature_store_api_client/models/config_field_name.py` & `dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/config_field_name.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/feature_store_api_client/models/create_feature_store_request.py` & `dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/create_feature_store_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/feature_store_api_client/models/create_feature_store_request_offline_store_config.py` & `dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/create_feature_store_request_offline_store_config.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/feature_store_api_client/models/entity.py` & `dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/entity.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/feature_store_api_client/models/feature.py` & `dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/feature.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/feature_store_api_client/models/feature_store.py` & `dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/feature_store.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/feature_store_api_client/models/feature_store_offline_store_config.py` & `dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/feature_store_offline_store_config.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/feature_store_api_client/models/feature_tags.py` & `dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/feature_tags.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/feature_store_api_client/models/feature_view.py` & `dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/feature_view.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/feature_store_api_client/models/feature_view_request.py` & `dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/feature_view_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/feature_store_api_client/models/feature_view_request_tags.py` & `dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/feature_view_request_tags.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/feature_store_api_client/models/feature_view_tags.py` & `dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/feature_view_tags.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/feature_store_api_client/models/field.py` & `dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/field.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/feature_store_api_client/models/lock_feature_store_request.py` & `dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/lock_feature_store_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/feature_store_api_client/models/metadata.py` & `dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/metadata.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/feature_store_api_client/models/offline_store_config.py` & `dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/offline_store_config.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/feature_store_api_client/models/offline_store_config_fields.py` & `dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/offline_store_config_fields.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/feature_store_api_client/models/unlock_feature_store_request.py` & `dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/unlock_feature_store_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/feature_store_api_client/models/upsert_feature_views_request.py` & `dominodatalab_data-5.8.0.dev1/feature_store_api_client/models/upsert_feature_views_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/feature_store_api_client/types.py` & `dominodatalab_data-5.8.0.dev1/feature_store_api_client/types.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/pyproject.toml` & `dominodatalab_data-5.8.0.dev1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dominodatalab-data"
-version = "5.7.1"
+version = "5.8.0dev1"
 description = "Domino Data API for interacting with Domino Data features"
 readme = "README.md"
 authors = [
     "Gabriel Haim <gabriel.haim@dominodatalab.com>",
     "Aaron Read <aaron.read@dominodatalab.com>",
 ]
 license = "Apache Software License 2.0"
@@ -38,31 +38,31 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pandas = ">=1.3.0"
+pandas = "^1.3.0"
 httpx = "^0.23.0"
 attrs = ">=20.1.0,<22.0.0"
 python-dateutil = "^2.8.0"
-pyarrow = "^8.0.0"
+pyarrow = "^10.0.0"
 loguru = "^0.5.3"
 backoff = "^1.11.1"
 bson = "^0.5.10"
 urllib3 = "^1.26.16"
 
 [tool.poetry.group.dev.dependencies]
 Sphinx = "^5.3.0"
 bandit = "^1.7.5"
 black = {version = "^22.12.0", allow-prereleases = true}
 darglint = "^1.8.1"
 flake8 = "^4.0.1"
-grpcio = "^1.56.0"
+grpcio = "^1.56.2"
 isort = {extras = ["colors"], version = "^5.12.0"}
 mypy = "^1.4.1"
 mypy-extensions = "^1.0.0"
 openapi-python-client = "^0.11.6"
 pdbpp = "^0.10.3"
 pre-commit = "^2.21.0"
 pydocstyle = "^6.3.0"
@@ -75,16 +75,16 @@
 safety = "^2.3.5"
 sphinx-rtd-theme = "^1.2.2"
 types-PyYAML = "^6.0.12.11"
 types-python-dateutil = "^2.8.19.14"
 vcrpy = "^5.0.0"
 
 [tool.poetry.group.featurestore.dependencies]
-feast = "^0.29.0"
-GitPython = "^3.1.31"
+feast = "^0.31.1"
+GitPython = "^3.1.32"
 
 [tool.black]
 # https://github.com/psf/black
 target-version = ["py38"]
 line-length = 100
 color = true
```

### Comparing `dominodatalab_data-5.7.1/training_set_api_client/api/default/delete_training_set_name.py` & `dominodatalab_data-5.8.0.dev1/training_set_api_client/api/default/delete_training_set_name.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/training_set_api_client/api/default/delete_training_set_name_number.py` & `dominodatalab_data-5.8.0.dev1/training_set_api_client/api/default/delete_training_set_name_number.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/training_set_api_client/api/default/get_training_set_name.py` & `dominodatalab_data-5.8.0.dev1/training_set_api_client/api/default/get_training_set_name.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/training_set_api_client/api/default/get_training_set_name_number.py` & `dominodatalab_data-5.8.0.dev1/training_set_api_client/api/default/get_training_set_name_number.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/training_set_api_client/api/default/post_find.py` & `dominodatalab_data-5.8.0.dev1/training_set_api_client/api/default/post_find.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/training_set_api_client/api/default/post_training_set_name.py` & `dominodatalab_data-5.8.0.dev1/training_set_api_client/api/default/post_training_set_name.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/training_set_api_client/api/default/post_version_find.py` & `dominodatalab_data-5.8.0.dev1/training_set_api_client/api/default/post_version_find.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/training_set_api_client/api/default/put_training_set_name.py` & `dominodatalab_data-5.8.0.dev1/training_set_api_client/api/default/put_training_set_name.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/training_set_api_client/api/default/put_training_set_name_number.py` & `dominodatalab_data-5.8.0.dev1/training_set_api_client/api/default/put_training_set_name_number.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/training_set_api_client/client.py` & `dominodatalab_data-5.8.0.dev1/feature_store_api_client/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,11 +39,14 @@
 
 
 @attr.s(auto_attribs=True)
 class AuthenticatedClient(Client):
     """A Client which has been authenticated for use on secured endpoints"""
 
     token: str
+    prefix: str = "Bearer"
+    auth_header_name: str = "Authorization"
 
     def get_headers(self) -> Dict[str, str]:
+        auth_header_value = f"{self.prefix} {self.token}" if self.prefix else self.token
         """Get headers to be used in authenticated endpoints"""
-        return {"Authorization": f"Bearer {self.token}", **self.headers}
+        return {self.auth_header_name: auth_header_value, **self.headers}
```

### Comparing `dominodatalab_data-5.7.1/training_set_api_client/models/__init__.py` & `dominodatalab_data-5.8.0.dev1/training_set_api_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/training_set_api_client/models/create_training_set_version_request.py` & `dominodatalab_data-5.8.0.dev1/training_set_api_client/models/create_training_set_version_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/training_set_api_client/models/create_training_set_version_request_meta.py` & `dominodatalab_data-5.8.0.dev1/training_set_api_client/models/create_training_set_version_request_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/training_set_api_client/models/monitoring_meta.py` & `dominodatalab_data-5.8.0.dev1/training_set_api_client/models/monitoring_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/training_set_api_client/models/training_set.py` & `dominodatalab_data-5.8.0.dev1/training_set_api_client/models/training_set.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/training_set_api_client/models/training_set_filter.py` & `dominodatalab_data-5.8.0.dev1/training_set_api_client/models/training_set_filter.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/training_set_api_client/models/training_set_filter_meta.py` & `dominodatalab_data-5.8.0.dev1/training_set_api_client/models/training_set_filter_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/training_set_api_client/models/training_set_meta.py` & `dominodatalab_data-5.8.0.dev1/training_set_api_client/models/training_set_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/training_set_api_client/models/training_set_version.py` & `dominodatalab_data-5.8.0.dev1/training_set_api_client/models/training_set_version.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/training_set_api_client/models/training_set_version_filter.py` & `dominodatalab_data-5.8.0.dev1/training_set_api_client/models/training_set_version_filter.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/training_set_api_client/models/training_set_version_filter_meta.py` & `dominodatalab_data-5.8.0.dev1/training_set_api_client/models/training_set_version_filter_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/training_set_api_client/models/training_set_version_filter_training_set_meta.py` & `dominodatalab_data-5.8.0.dev1/training_set_api_client/models/training_set_version_filter_training_set_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/training_set_api_client/models/training_set_version_meta.py` & `dominodatalab_data-5.8.0.dev1/training_set_api_client/models/training_set_version_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/training_set_api_client/models/update_training_set_request.py` & `dominodatalab_data-5.8.0.dev1/training_set_api_client/models/update_training_set_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/training_set_api_client/models/update_training_set_request_meta.py` & `dominodatalab_data-5.8.0.dev1/training_set_api_client/models/update_training_set_request_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/training_set_api_client/models/update_training_set_version_request.py` & `dominodatalab_data-5.8.0.dev1/training_set_api_client/models/update_training_set_version_request.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/training_set_api_client/models/update_training_set_version_request_meta.py` & `dominodatalab_data-5.8.0.dev1/training_set_api_client/models/update_training_set_version_request_meta.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/training_set_api_client/types.py` & `dominodatalab_data-5.8.0.dev1/training_set_api_client/types.py`

 * *Files identical despite different names*

### Comparing `dominodatalab_data-5.7.1/PKG-INFO` & `dominodatalab_data-5.8.0.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dominodatalab-data
-Version: 5.7.1
+Version: 5.8.0.dev1
 Summary: Domino Data API for interacting with Domino Data features
 Home-page: https://github.com/dominodatalab/domino-data
 License: Apache Software License 2.0
 Author: Gabriel Haim
 Author-email: gabriel.haim@dominodatalab.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,16 +19,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: attrs (>=20.1.0,<22.0.0)
 Requires-Dist: backoff (>=1.11.1,<2.0.0)
 Requires-Dist: bson (>=0.5.10,<0.6.0)
 Requires-Dist: httpx (>=0.23.0,<0.24.0)
 Requires-Dist: loguru (>=0.5.3,<0.6.0)
-Requires-Dist: pandas (>=1.3.0)
-Requires-Dist: pyarrow (>=8.0.0,<9.0.0)
+Requires-Dist: pandas (>=1.3.0,<2.0.0)
+Requires-Dist: pyarrow (>=10.0.0,<11.0.0)
 Requires-Dist: python-dateutil (>=2.8.0,<3.0.0)
 Requires-Dist: urllib3 (>=1.26.16,<2.0.0)
 Project-URL: Repository, https://github.com/dominodatalab/domino-data
 Description-Content-Type: text/markdown
 
 # Domino Data API
```

