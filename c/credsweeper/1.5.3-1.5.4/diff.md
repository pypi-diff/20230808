# Comparing `tmp/credsweeper-1.5.3.tar.gz` & `tmp/credsweeper-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "credsweeper-1.5.3.tar", last modified: Thu Jul 20 16:15:42 2023, max compression
+gzip compressed data, was "credsweeper-1.5.4.tar", last modified: Tue Aug  8 08:03:01 2023, max compression
```

## Comparing `credsweeper-1.5.3.tar` & `credsweeper-1.5.4.tar`

### file list

```diff
@@ -1,160 +1,162 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.589390 credsweeper-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-20 16:15:24.000000 credsweeper-1.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-07-20 16:15:42.589390 credsweeper-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-07-20 16:15:24.000000 credsweeper-1.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.565388 credsweeper-1.5.3/credsweeper/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15134 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17086 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.565388 credsweeper-1.5.3/credsweeper/common/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/common/keyword_checklist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/common/keyword_checklist.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/common/morpheme_checklist.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.565388 credsweeper-1.5.3/credsweeper/config/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.569389 credsweeper-1.5.3/credsweeper/credentials/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/credentials/augment_candidates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/credentials/candidate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/credentials/candidate_group_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/credentials/candidate_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/credentials/credential_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/credentials/line_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.573389 credsweeper-1.5.3/credsweeper/deep_scanner/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/deep_scanner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/deep_scanner/abstract_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/deep_scanner/byte_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/deep_scanner/bzip2_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/deep_scanner/deep_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/deep_scanner/encoder_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/deep_scanner/gzip_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/deep_scanner/html_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/deep_scanner/lang_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/deep_scanner/pdf_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/deep_scanner/tar_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/deep_scanner/xml_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/deep_scanner/zip_scanner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.573389 credsweeper-1.5.3/credsweeper/file_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/file_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/file_handler/analysis_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/file_handler/byte_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/file_handler/content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/file_handler/data_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/file_handler/descriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/file_handler/diff_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/file_handler/file_path_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/file_handler/files_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/file_handler/patch_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/file_handler/string_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/file_handler/struct_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/file_handler/text_content_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/file_handler/text_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.581390 credsweeper-1.5.3/credsweeper/filters/
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/cred_card_number_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.585390 credsweeper-1.5.3/credsweeper/filters/group/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/group/general_keyword.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/group/general_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/group/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/group/password_keyword.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/group/structured_token.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/group/token_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/group/url_credentials_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/group/weird_base36_token.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/group/weird_base64_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/line_specific_key_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/separator_unusual_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_allowlist_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_array_dictionary_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_base32_data_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_base64_data_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_blocklist_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_camel_case_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_couple_keyword_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_dictionary_keyword_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_dictionary_value_length_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_entropy_base32_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_entropy_base36_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_entropy_base64_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_file_path_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_first_word_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_grafana_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_json_web_token_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_last_word_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_length_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_method_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_not_allowed_pattern_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_not_part_encoded_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_number_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_pattern_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_pattern_length_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_pem_pattern_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_similarity_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_split_keyword_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_string_type_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_structured_token_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_token_base32_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_token_base36_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_token_base64_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_token_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/value_useless_word_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/filters/variable_not_allowed_pattern_check.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.585390 credsweeper-1.5.3/credsweeper/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/logger/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.585390 credsweeper-1.5.3/credsweeper/ml_model/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/ml_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/ml_model/features.py
--rw-r--r--   0 runner    (1001) docker     (123)   165415 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/ml_model/ml_model.onnx
--rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/ml_model/ml_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/ml_model/model_config.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.585390 credsweeper-1.5.3/credsweeper/rules/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17558 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/rules/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/rules/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.585390 credsweeper-1.5.3/credsweeper/scanner/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/scanner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.585390 credsweeper-1.5.3/credsweeper/scanner/scan_type/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/scanner/scan_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/scanner/scan_type/multi_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/scanner/scan_type/pem_key_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/scanner/scan_type/scan_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/scanner/scan_type/single_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/scanner/scanner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.589390 credsweeper-1.5.3/credsweeper/secret/
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/secret/config.json
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/secret/log.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.589390 credsweeper-1.5.3/credsweeper/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/utils/entropy_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21745 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/utils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.589390 credsweeper-1.5.3/credsweeper/validations/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/validations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/validations/apply_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/validations/github_token_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/validations/google_api_key_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/validations/google_multi_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/validations/mailchimp_key_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/validations/slack_token_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/validations/square_access_token_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/validations/square_client_id_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/validations/stripe_api_key_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-20 16:15:24.000000 credsweeper-1.5.3/credsweeper/validations/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.565388 credsweeper-1.5.3/credsweeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-07-20 16:15:42.000000 credsweeper-1.5.3/credsweeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5732 2023-07-20 16:15:42.000000 credsweeper-1.5.3/credsweeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 16:15:42.000000 credsweeper-1.5.3/credsweeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-20 16:15:42.000000 credsweeper-1.5.3/credsweeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-20 16:15:42.000000 credsweeper-1.5.3/credsweeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 16:15:42.000000 credsweeper-1.5.3/credsweeper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-20 16:15:42.593391 credsweeper-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-20 16:15:24.000000 credsweeper-1.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:15:42.589390 credsweeper-1.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    30988 2023-07-20 16:15:24.000000 credsweeper-1.5.3/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    43734 2023-07-20 16:15:24.000000 credsweeper-1.5.3/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:03:01.449074 credsweeper-1.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-08 08:02:43.000000 credsweeper-1.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-08-08 08:03:01.449074 credsweeper-1.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-08-08 08:02:43.000000 credsweeper-1.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:03:01.413075 credsweeper-1.5.4/credsweeper/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15134 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17589 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:03:01.413075 credsweeper-1.5.4/credsweeper/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/common/keyword_checklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/common/keyword_checklist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8696 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/common/morpheme_checklist.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:03:01.417075 credsweeper-1.5.4/credsweeper/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:03:01.417075 credsweeper-1.5.4/credsweeper/credentials/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/credentials/augment_candidates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/credentials/candidate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/credentials/candidate_group_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/credentials/candidate_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/credentials/credential_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/credentials/line_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:03:01.421074 credsweeper-1.5.4/credsweeper/deep_scanner/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/deep_scanner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/deep_scanner/abstract_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/deep_scanner/byte_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/deep_scanner/bzip2_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/deep_scanner/deep_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/deep_scanner/encoder_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/deep_scanner/gzip_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/deep_scanner/html_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/deep_scanner/lang_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/deep_scanner/pdf_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/deep_scanner/tar_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/deep_scanner/xml_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/deep_scanner/zip_scanner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:03:01.425074 credsweeper-1.5.4/credsweeper/file_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/file_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/file_handler/analysis_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/file_handler/byte_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/file_handler/content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/file_handler/data_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/file_handler/descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/file_handler/diff_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/file_handler/file_path_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/file_handler/files_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/file_handler/patch_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/file_handler/string_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/file_handler/struct_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/file_handler/text_content_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/file_handler/text_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:03:01.433074 credsweeper-1.5.4/credsweeper/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:03:01.437074 credsweeper-1.5.4/credsweeper/filters/group/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/group/general_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/group/general_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/group/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/group/password_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/group/structured_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/group/token_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/group/url_credentials_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/group/weird_base36_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/group/weird_base64_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/line_specific_key_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/separator_unusual_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_allowlist_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_array_dictionary_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_base32_data_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_base64_data_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_blocklist_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_camel_case_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_card_number_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_couple_keyword_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_dictionary_keyword_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_dictionary_value_length_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_entropy_base32_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_entropy_base36_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_entropy_base64_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_file_path_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_first_word_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_grafana_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_iban_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_json_web_token_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_last_word_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_length_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_method_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_not_allowed_pattern_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_not_part_encoded_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_number_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_pattern_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_pattern_length_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_pem_pattern_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_similarity_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_split_keyword_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_string_type_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_structured_token_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_token_base32_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_token_base36_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_token_base64_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_token_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_useless_word_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/value_vin_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/filters/variable_not_allowed_pattern_check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:03:01.437074 credsweeper-1.5.4/credsweeper/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/logger/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:03:01.441074 credsweeper-1.5.4/credsweeper/ml_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/ml_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/ml_model/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)   165415 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/ml_model/ml_model.onnx
+-rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/ml_model/ml_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/ml_model/model_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:03:01.441074 credsweeper-1.5.4/credsweeper/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18514 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/rules/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/rules/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:03:01.441074 credsweeper-1.5.4/credsweeper/scanner/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/scanner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:03:01.441074 credsweeper-1.5.4/credsweeper/scanner/scan_type/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/scanner/scan_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/scanner/scan_type/multi_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/scanner/scan_type/pem_key_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/scanner/scan_type/scan_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/scanner/scan_type/single_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/scanner/scanner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:03:01.445074 credsweeper-1.5.4/credsweeper/secret/
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/secret/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/secret/log.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:03:01.445074 credsweeper-1.5.4/credsweeper/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/utils/entropy_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21745 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/utils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:03:01.449074 credsweeper-1.5.4/credsweeper/validations/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/validations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/validations/apply_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/validations/github_token_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/validations/google_api_key_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/validations/google_multi_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/validations/mailchimp_key_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/validations/slack_token_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/validations/square_access_token_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/validations/square_client_id_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/validations/stripe_api_key_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-08-08 08:02:43.000000 credsweeper-1.5.4/credsweeper/validations/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:03:01.413075 credsweeper-1.5.4/credsweeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-08-08 08:03:01.000000 credsweeper-1.5.4/credsweeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-08-08 08:03:01.000000 credsweeper-1.5.4/credsweeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 08:03:01.000000 credsweeper-1.5.4/credsweeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-08 08:03:01.000000 credsweeper-1.5.4/credsweeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-08-08 08:03:01.000000 credsweeper-1.5.4/credsweeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-08 08:03:01.000000 credsweeper-1.5.4/credsweeper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-08 08:03:01.449074 credsweeper-1.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-08-08 08:02:43.000000 credsweeper-1.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:03:01.449074 credsweeper-1.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    30888 2023-08-08 08:02:43.000000 credsweeper-1.5.4/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43603 2023-08-08 08:02:43.000000 credsweeper-1.5.4/tests/test_main.py
```

### Comparing `credsweeper-1.5.3/LICENSE` & `credsweeper-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/PKG-INFO` & `credsweeper-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: credsweeper
-Version: 1.5.3
+Version: 1.5.4
 Summary: Credential Sweeper
 Home-page: https://github.com/Samsung/CredSweeper
 Project-URL: Bug Tracker, https://github.com/Samsung/CredSweeper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `credsweeper-1.5.3/README.md` & `credsweeper-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/__init__.py` & `credsweeper-1.5.4/credsweeper/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
     'MlValidator',  #
     'StringContentProvider',  #
     'TextContentProvider',  #
     'ThresholdPreset',  #
     '__version__'
 ]
 
-__version__ = "1.5.3"
+__version__ = "1.5.4"
```

### Comparing `credsweeper-1.5.3/credsweeper/__main__.py` & `credsweeper-1.5.4/credsweeper/__main__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/app.py` & `credsweeper-1.5.4/credsweeper/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,18 @@
 
         return config_dict  # type: ignore
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def _use_ml_validation(self) -> bool:
         if isinstance(self.ml_threshold, (float, int)) and 0 >= self.ml_threshold:
+            logger.info("ML validation is disabled")
+            return False
+        if not self.credential_manager.candidates:
+            logger.info("Skipping ML validation due to no candidates found")
             return False
         return True
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     # the import cannot be done on top due
     # TypeError: cannot pickle 'onnxruntime.capi.onnxruntime_pybind11_state.InferenceSession' object
@@ -315,15 +319,15 @@
         return candidates
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def post_processing(self) -> None:
         """Machine learning validation for received credential candidates."""
         if self._use_ml_validation():
-            logger.info(f"Run ML Validation for {len(self.credential_manager.candidates)} candidates")
+            logger.info(f"Grouping {len(self.credential_manager.candidates)} candidates")
             new_cred_list = []
             cred_groups = self.credential_manager.group_credentials()
             ml_cred_groups = []
             for group_key, group_candidates in cred_groups.items():
                 # Analyze with ML if all candidates in group require ML
                 for candidate in group_candidates:
                     if not candidate.use_ml:
@@ -332,21 +336,26 @@
                     ml_cred_groups.append((group_key.value, group_candidates))
                     continue
                 # If at least one of credentials in the group do not require ML - automatically report to user
                 for candidate in group_candidates:
                     candidate.ml_validation = KeyValidationOption.NOT_AVAILABLE
                 new_cred_list += group_candidates
 
-            is_cred, probability = self.ml_validator.validate_groups(ml_cred_groups, self.ml_batch_size)
-            for i, (_, group_candidates) in enumerate(ml_cred_groups):
-                if is_cred[i]:
-                    for candidate in group_candidates:
-                        candidate.ml_validation = KeyValidationOption.VALIDATED_KEY
-                        candidate.ml_probability = probability[i]
-                    new_cred_list += group_candidates
+            # prevent extra ml_validator creation if ml_cred_groups is empty
+            if ml_cred_groups:
+                logger.info(f"Run ML Validation for {len(ml_cred_groups)} groups")
+                is_cred, probability = self.ml_validator.validate_groups(ml_cred_groups, self.ml_batch_size)
+                for i, (_, group_candidates) in enumerate(ml_cred_groups):
+                    if is_cred[i]:
+                        for candidate in group_candidates:
+                            candidate.ml_validation = KeyValidationOption.VALIDATED_KEY
+                            candidate.ml_probability = probability[i]
+                        new_cred_list += group_candidates
+            else:
+                logger.info("Skipping ML validation due not applicable")
 
             self.credential_manager.set_credentials(new_cred_list)
 
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def export_results(self) -> None:
         """Save credential candidates to json file or print them to a console."""
```

### Comparing `credsweeper-1.5.3/credsweeper/common/constants.py` & `credsweeper-1.5.4/credsweeper/common/constants.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/common/keyword_checklist.py` & `credsweeper-1.5.4/credsweeper/common/keyword_checklist.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/common/keyword_checklist.txt` & `credsweeper-1.5.4/credsweeper/common/keyword_checklist.txt`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/common/morpheme_checklist.txt` & `credsweeper-1.5.4/credsweeper/common/morpheme_checklist.txt`

 * *Files 1% similar despite different names*

```diff
@@ -989,14 +989,15 @@
 pale
 panel
 par
 pass
 patch
 path
 patte
+paw
 pci
 pcmcia
 peer
 penalt
 pend
 people
 per
```

### Comparing `credsweeper-1.5.3/credsweeper/config/config.py` & `credsweeper-1.5.4/credsweeper/config/config.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/credentials/augment_candidates.py` & `credsweeper-1.5.4/credsweeper/credentials/augment_candidates.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/credentials/candidate.py` & `credsweeper-1.5.4/credsweeper/credentials/candidate.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/credentials/candidate_group_generator.py` & `credsweeper-1.5.4/credsweeper/credentials/candidate_group_generator.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/credentials/candidate_key.py` & `credsweeper-1.5.4/credsweeper/credentials/candidate_key.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/credentials/credential_manager.py` & `credsweeper-1.5.4/credsweeper/credentials/credential_manager.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/credentials/line_data.py` & `credsweeper-1.5.4/credsweeper/credentials/line_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,17 @@
             # If variable name starts with `-` (usual case for args in CLI)
             #  and value can be split by bash special characters
             if len(value_spl) > 1 and self.variable.startswith("-"):
                 self.value = value_spl[0]
 
     def sanitize_variable(self) -> None:
         """Remove trailing spaces, dashes and quotations around the variable."""
-        if self.variable:
+        sanitized_var_len = 0
+        while self.variable and sanitized_var_len != len(self.variable):
+            sanitized_var_len = len(self.variable)
             # Remove trailing \s. Can happen if there are \s between variable and `=` character
             self.variable = self.variable.strip()
             # Remove trailing `-` at the variable name start. Usual case for CLI commands
             self.variable = self.variable.strip("-")
             # Remove trailing `'"`. Usual case for JSON data
             self.variable = self.variable.strip('"')
             self.variable = self.variable.strip("'")
```

### Comparing `credsweeper-1.5.3/credsweeper/deep_scanner/abstract_scanner.py` & `credsweeper-1.5.4/credsweeper/deep_scanner/abstract_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/deep_scanner/byte_scanner.py` & `credsweeper-1.5.4/credsweeper/deep_scanner/byte_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/deep_scanner/bzip2_scanner.py` & `credsweeper-1.5.4/credsweeper/deep_scanner/bzip2_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/deep_scanner/deep_scanner.py` & `credsweeper-1.5.4/credsweeper/deep_scanner/deep_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/deep_scanner/encoder_scanner.py` & `credsweeper-1.5.4/credsweeper/deep_scanner/encoder_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/deep_scanner/gzip_scanner.py` & `credsweeper-1.5.4/credsweeper/deep_scanner/gzip_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/deep_scanner/html_scanner.py` & `credsweeper-1.5.4/credsweeper/deep_scanner/html_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/deep_scanner/lang_scanner.py` & `credsweeper-1.5.4/credsweeper/deep_scanner/lang_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/deep_scanner/pdf_scanner.py` & `credsweeper-1.5.4/credsweeper/deep_scanner/pdf_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/deep_scanner/tar_scanner.py` & `credsweeper-1.5.4/credsweeper/deep_scanner/tar_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/deep_scanner/xml_scanner.py` & `credsweeper-1.5.4/credsweeper/deep_scanner/xml_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/deep_scanner/zip_scanner.py` & `credsweeper-1.5.4/credsweeper/deep_scanner/zip_scanner.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/file_handler/__init__.py` & `credsweeper-1.5.4/credsweeper/file_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/file_handler/analysis_target.py` & `credsweeper-1.5.4/credsweeper/file_handler/analysis_target.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/file_handler/byte_content_provider.py` & `credsweeper-1.5.4/credsweeper/file_handler/byte_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/file_handler/content_provider.py` & `credsweeper-1.5.4/credsweeper/file_handler/content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/file_handler/data_content_provider.py` & `credsweeper-1.5.4/credsweeper/file_handler/data_content_provider.py`

 * *Files 10% similar despite different names*

```diff
@@ -73,29 +73,43 @@
         Return True if some structure found
         """
         try:
             if MIN_DATA_LEN > len(self.__text):
                 return False
         except Exception:
             return False
-        # JSON
-        try:
-            if "{" in self.__text:
+        # JSON & NDJSON
+        if "{" in self.__text and "}" in self.__text and "\"" in self.__text and ":" in self.__text:
+            try:
                 self.structure = json.loads(self.__text)
                 logger.debug("CONVERTED from json")
+            except Exception as exc:
+                logger.debug("Cannot parse as json:%s %s", exc, self.data)
             else:
-                logger.debug("Data do not contain { - weak JSON")
-        except Exception as exc:
-            logger.debug("Cannot parse as json:%s %s", exc, self.data)
+                if self.__is_structure():
+                    return True
+            try:
+                self.structure = []
+                for line in self.__text.splitlines():
+                    self.structure.append(json.loads(line))
+                else:
+                    logger.debug("CONVERTED from ndjson")
+            except Exception as exc:
+                logger.debug("Cannot parse as ndjson:%s %s", exc, self.data)
+                self.structure = None
+            else:
+                if self.__is_structure():
+                    return True
         else:
-            if self.__is_structure():
-                return True
+            logger.debug("Data do not contain { - weak JSON")
+
         # # # Python
         try:
-            if ";" in self.__text or 2 < self.__text.count("\n"):
+            # search only in sources with strings
+            if (";" in self.__text or 2 < self.__text.count("\n")) and ("\"" in self.__text or "'" in self.__text):
                 self.structure = Util.parse_python(self.__text)
                 logger.debug("CONVERTED from Python")
             else:
                 logger.debug("Data do not contain line feed - weak PYTHON")
         except Exception as exc:
             logger.debug("Cannot parse as Python:%s %s", exc, self.data)
         else:
@@ -134,14 +148,25 @@
                 return False
         except Exception as exc:
             logger.debug("Cannot parse as XML:%s %s", exc, self.data)
         else:
             return bool(self.lines and self.line_numbers)
         return False
 
+    def _extend_lines_with_text(self, text: str, line_num: int) -> bool:
+        """multiline cell will be analysed as text"""
+        lines = text.splitlines()
+        if 1 >= len(lines):
+            return False
+        for line in lines:
+            if stripped_line := line.strip():
+                self.line_numbers.append(line_num)
+                self.lines.append(stripped_line)
+        return True
+
     def represent_as_html(self) -> bool:
         """Tries to read data as html
 
         Return:
              True if reading was successful
 
         """
@@ -161,41 +186,55 @@
                     if line:
                         self.line_numbers.append(line_number + 1)
                         self.lines.append(line)
 
                 # transform table if table cell is assigned to header cell
                 # make from cells a chain like next is assigned to previous
                 for table in html.find_all('table'):
-                    table_header = None
+                    table_header: Optional[List[Optional[str]]] = None
                     for tr in table.find_all('tr'):
-                        record_line = ""
-                        if table_header:
-                            for th, td in zip(table_header.find_all(['td', 'th']), tr.find_all('td')):
-                                th_text = th.get_text(strip=True)
-                                td_text = td.get_text(strip=True)
-                                if not record_line:
-                                    record_line = f'"{td_text}"'
+                        record_numbers = []
+                        record_lines = []
+                        record_leading = ""
+                        if table_header is None:
+                            table_header = []
+                            # first row in table may be a header with <td> and a style, but search <th> too
+                            for cell in tr.find_all(['th', 'td']):
+                                td_text = cell.get_text(strip=True)
+                                if not td_text or self._extend_lines_with_text(td_text, cell.sourceline):
+                                    table_header.append(None)
+                                    continue
+                                table_header.append(td_text)
+                                if not record_leading:
+                                    record_leading = td_text
                                 else:
-                                    record_line += f' = "{td_text}"'
-                                self.line_numbers.append(td.sourceline)
-                                self.lines.append(f'{th_text} = "{td_text}"')
-                            self.line_numbers.append(tr.sourceline)
-                            self.lines.append(record_line)
+                                    record_numbers.append(cell.sourceline)
+                                    record_lines.append(f"{record_leading} = {td_text}")
+                                # add single text to lines for analysis
+                                self.line_numbers.append(cell.sourceline)
+                                self.lines.append(td_text)
                         else:
-                            for td in tr.find_all(['td', 'th']):
-                                td_text = td.get_text(strip=True)
-                                if not record_line:
-                                    record_line = f'"{td_text}"'
+                            # not a first line in table - may be combined with a header
+                            for header_pos, cell in enumerate(tr.find_all('td')):
+                                td_text = cell.get_text(strip=True)
+                                if not td_text or self._extend_lines_with_text(td_text, cell.sourceline):
+                                    continue
+                                if not record_leading:
+                                    record_leading = td_text
                                 else:
-                                    record_line += f' = "{td_text}"'
-                                self.line_numbers.append(td.sourceline)
-                                self.lines.append(td_text)
-                            self.line_numbers.append(tr.sourceline)
-                            self.lines.append(record_line)
-                            table_header = tr
+                                    record_numbers.append(cell.sourceline)
+                                    record_lines.append(f"{record_leading} = {td_text}")
+                                if header_pos < len(table_header):
+                                    if header_text := table_header[header_pos]:
+                                        self.line_numbers.append(cell.sourceline)
+                                        self.lines.append(f"{header_text} = {td_text}")
+                        if record_lines:
+                            # add combinations with left column
+                            self.line_numbers.extend(record_numbers)
+                            self.lines.extend(record_lines)
 
                 logger.debug("CONVERTED from html")
             else:
                 logger.debug("Data do not contain specific tags - weak HTML")
         except Exception as exc:
             logger.debug("Cannot parse as HTML:%s %s", exc, self.data)
         else:
```

### Comparing `credsweeper-1.5.3/credsweeper/file_handler/diff_content_provider.py` & `credsweeper-1.5.4/credsweeper/file_handler/diff_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/file_handler/file_path_extractor.py` & `credsweeper-1.5.4/credsweeper/file_handler/file_path_extractor.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/file_handler/files_provider.py` & `credsweeper-1.5.4/credsweeper/file_handler/files_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/file_handler/patch_provider.py` & `credsweeper-1.5.4/credsweeper/file_handler/patch_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/file_handler/string_content_provider.py` & `credsweeper-1.5.4/credsweeper/file_handler/string_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/file_handler/struct_content_provider.py` & `credsweeper-1.5.4/credsweeper/file_handler/struct_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/file_handler/text_content_provider.py` & `credsweeper-1.5.4/credsweeper/file_handler/text_content_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/file_handler/text_provider.py` & `credsweeper-1.5.4/credsweeper/file_handler/text_provider.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/__init__.py` & `credsweeper-1.5.4/credsweeper/filters/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from credsweeper.filters.filter import Filter  # isort:skip
 
-from credsweeper.filters.cred_card_number_check import CreditCardNumberCheck
 from credsweeper.filters.line_specific_key_check import LineSpecificKeyCheck
 from credsweeper.filters.separator_unusual_check import SeparatorUnusualCheck
 from credsweeper.filters.value_allowlist_check import ValueAllowlistCheck
 from credsweeper.filters.value_array_dictionary_check import ValueArrayDictionaryCheck
 from credsweeper.filters.value_base32_data_check import ValueBase32DataCheck
 from credsweeper.filters.value_base64_data_check import ValueBase64DataCheck
 from credsweeper.filters.value_blocklist_check import ValueBlocklistCheck
 from credsweeper.filters.value_camel_case_check import ValueCamelCaseCheck
+from credsweeper.filters.value_card_number_check import ValueCardNumberCheck
 from credsweeper.filters.value_couple_keyword_check import ValueCoupleKeywordCheck
 from credsweeper.filters.value_dictionary_keyword_check import ValueDictionaryKeywordCheck
 from credsweeper.filters.value_dictionary_value_length_check import ValueDictionaryValueLengthCheck
 from credsweeper.filters.value_entropy_base32_check import ValueEntropyBase32Check
 from credsweeper.filters.value_entropy_base36_check import ValueEntropyBase36Check
 from credsweeper.filters.value_entropy_base64_check import ValueEntropyBase64Check
 from credsweeper.filters.value_file_path_check import ValueFilePathCheck
 from credsweeper.filters.value_first_word_check import ValueFirstWordCheck
 from credsweeper.filters.value_grafana_check import ValueGrafanaCheck
+from credsweeper.filters.value_iban_check import ValueIbanCheck
 from credsweeper.filters.value_json_web_token_check import ValueJsonWebTokenCheck
 from credsweeper.filters.value_last_word_check import ValueLastWordCheck
 from credsweeper.filters.value_length_check import ValueLengthCheck
 from credsweeper.filters.value_method_check import ValueMethodCheck
 from credsweeper.filters.value_not_allowed_pattern_check import ValueNotAllowedPatternCheck
 from credsweeper.filters.value_not_part_encoded_check import ValueNotPartEncodedCheck
 from credsweeper.filters.value_number_check import ValueNumberCheck
@@ -33,8 +34,9 @@
 from credsweeper.filters.value_string_type_check import ValueStringTypeCheck
 from credsweeper.filters.value_structured_token_check import ValueStructuredTokenCheck
 from credsweeper.filters.value_token_base32_check import ValueTokenBase32Check
 from credsweeper.filters.value_token_base36_check import ValueTokenBase36Check
 from credsweeper.filters.value_token_base64_check import ValueTokenBase64Check
 from credsweeper.filters.value_token_check import ValueTokenCheck
 from credsweeper.filters.value_useless_word_check import ValueUselessWordCheck
+from credsweeper.filters.value_vin_check import ValueVinCheck
 from credsweeper.filters.variable_not_allowed_pattern_check import VariableNotAllowedPatternCheck
```

### Comparing `credsweeper-1.5.3/credsweeper/filters/cred_card_number_check.py` & `credsweeper-1.5.4/credsweeper/filters/value_card_number_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from credsweeper.config import Config
 from credsweeper.credentials import LineData
 from credsweeper.file_handler.analysis_target import AnalysisTarget
 from credsweeper.filters import Filter
 
 
-class CreditCardNumberCheck(Filter):
+class ValueCardNumberCheck(Filter):
     """Check that value is a credit card number."""
 
     def __init__(self, config: Config = None) -> None:
         pass
 
     def run(self, line_data: LineData, target: AnalysisTarget) -> bool:
         """Run filter checks on received credential candidate data 'line_data'.
```

### Comparing `credsweeper-1.5.3/credsweeper/filters/filter.py` & `credsweeper-1.5.4/credsweeper/filters/filter.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/group/__init__.py` & `credsweeper-1.5.4/credsweeper/filters/group/__init__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/group/group.py` & `credsweeper-1.5.4/credsweeper/filters/group/group.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/group/token_pattern.py` & `credsweeper-1.5.4/credsweeper/filters/group/token_pattern.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/group/url_credentials_group.py` & `credsweeper-1.5.4/credsweeper/filters/group/url_credentials_group.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/group/weird_base36_token.py` & `credsweeper-1.5.4/credsweeper/filters/group/weird_base36_token.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/group/weird_base64_token.py` & `credsweeper-1.5.4/credsweeper/filters/group/weird_base64_token.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/line_specific_key_check.py` & `credsweeper-1.5.4/credsweeper/filters/line_specific_key_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/separator_unusual_check.py` & `credsweeper-1.5.4/credsweeper/filters/separator_unusual_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/value_allowlist_check.py` & `credsweeper-1.5.4/credsweeper/filters/value_allowlist_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/value_array_dictionary_check.py` & `credsweeper-1.5.4/credsweeper/filters/value_array_dictionary_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/value_base32_data_check.py` & `credsweeper-1.5.4/credsweeper/filters/value_base32_data_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/value_base64_data_check.py` & `credsweeper-1.5.4/credsweeper/filters/value_base64_data_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/value_blocklist_check.py` & `credsweeper-1.5.4/credsweeper/filters/value_blocklist_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/value_camel_case_check.py` & `credsweeper-1.5.4/credsweeper/filters/value_camel_case_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/value_couple_keyword_check.py` & `credsweeper-1.5.4/credsweeper/filters/value_couple_keyword_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/value_dictionary_keyword_check.py` & `credsweeper-1.5.4/credsweeper/filters/value_dictionary_keyword_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/value_dictionary_value_length_check.py` & `credsweeper-1.5.4/credsweeper/filters/value_dictionary_value_length_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/value_entropy_base32_check.py` & `credsweeper-1.5.4/credsweeper/filters/value_entropy_base32_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/value_entropy_base36_check.py` & `credsweeper-1.5.4/credsweeper/filters/value_entropy_base36_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/value_entropy_base64_check.py` & `credsweeper-1.5.4/credsweeper/filters/value_entropy_base64_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/value_file_path_check.py` & `credsweeper-1.5.4/credsweeper/filters/value_file_path_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/value_first_word_check.py` & `credsweeper-1.5.4/credsweeper/filters/value_first_word_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/value_grafana_check.py` & `credsweeper-1.5.4/credsweeper/filters/value_grafana_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/value_json_web_token_check.py` & `credsweeper-1.5.4/credsweeper/filters/value_json_web_token_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/value_last_word_check.py` & `credsweeper-1.5.4/credsweeper/filters/value_last_word_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/value_length_check.py` & `credsweeper-1.5.4/credsweeper/filters/value_length_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/value_method_check.py` & `credsweeper-1.5.4/credsweeper/filters/value_method_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/value_not_allowed_pattern_check.py` & `credsweeper-1.5.4/credsweeper/filters/value_not_allowed_pattern_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/value_not_part_encoded_check.py` & `credsweeper-1.5.4/credsweeper/filters/value_not_part_encoded_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/value_number_check.py` & `credsweeper-1.5.4/credsweeper/filters/value_number_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/value_pattern_check.py` & `credsweeper-1.5.4/credsweeper/filters/value_pattern_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/value_pem_pattern_check.py` & `credsweeper-1.5.4/credsweeper/filters/value_pem_pattern_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/value_similarity_check.py` & `credsweeper-1.5.4/credsweeper/filters/value_similarity_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/value_split_keyword_check.py` & `credsweeper-1.5.4/credsweeper/filters/value_split_keyword_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/value_string_type_check.py` & `credsweeper-1.5.4/credsweeper/filters/value_string_type_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/value_structured_token_check.py` & `credsweeper-1.5.4/credsweeper/filters/value_structured_token_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/value_token_base32_check.py` & `credsweeper-1.5.4/credsweeper/filters/value_token_base32_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/value_token_base36_check.py` & `credsweeper-1.5.4/credsweeper/filters/value_token_base36_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/value_token_base64_check.py` & `credsweeper-1.5.4/credsweeper/filters/value_token_base64_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/value_token_check.py` & `credsweeper-1.5.4/credsweeper/filters/value_token_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/value_useless_word_check.py` & `credsweeper-1.5.4/credsweeper/filters/value_useless_word_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/filters/variable_not_allowed_pattern_check.py` & `credsweeper-1.5.4/credsweeper/filters/variable_not_allowed_pattern_check.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/logger/logger.py` & `credsweeper-1.5.4/credsweeper/logger/logger.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/ml_model/features.py` & `credsweeper-1.5.4/credsweeper/ml_model/features.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/ml_model/ml_model.onnx` & `credsweeper-1.5.4/credsweeper/ml_model/ml_model.onnx`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/ml_model/ml_validator.py` & `credsweeper-1.5.4/credsweeper/ml_model/ml_validator.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/ml_model/model_config.json` & `credsweeper-1.5.4/credsweeper/ml_model/model_config.json`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/rules/config.yaml` & `credsweeper-1.5.4/credsweeper/rules/config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,39 @@
+- name: VIN
+  severity: info
+  type: pattern
+  values:
+    - (^|[^0-9A-Za-z])(?P<value>[A-HJ-NPR-Z0-9]{17})([^=0-9A-Za-z]|$)
+  filter_type:
+    - ValueVinCheck
+    - ValuePatternCheck
+  min_line_len: 16
+  required_regex: "[a-zA-Z0-9_/+-]{15,}"
+  doc_available: false
+
 - name: Credit card number
   severity: info
   type: pattern
   values:
     - (?<!([0-9]\.|[=*+\/\-] |.[=*+\/\-]))((?<![0-9A-Za-z_=*+\-\/.])(?P<value>[0-9]{16})(?![0-9A-Za-z_=*+\-\/.]))(?!(\.[0-9]| [=*+\/\-]|.[=*+\/\-]))
   filter_type:
-    - CreditCardNumberCheck
+    - ValueCardNumberCheck
   min_line_len: 16
+  required_regex: "[a-zA-Z0-9_/+-]{15,}"
+  doc_available: false
+
+- name: IBAN
+  severity: info
+  type: pattern
+  values:
+    - (^|[^0-9A-Za-z])(?P<value>[A-Z]{2}[0-9]{2}[A-Z0-9]{12,30})([^=0-9A-Za-z]|$)
+  filter_type:
+    - ValueIbanCheck
+  min_line_len: 16
+  required_regex: "[a-zA-Z0-9_/+-]{15,}"
   doc_available: false
 
 - name: API
   severity: medium
   type: keyword
   values:
     - api
@@ -26,14 +50,15 @@
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>(ABIA|ACCA|AGPA|AIDA|AIPA|AKIA|ANPA|ANVA|AROA|APKA|ASCA|ASIA)[0-9A-Z]{16,17})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - A
   min_line_len: 20
+  required_regex: "[a-zA-Z0-9_/+-]{15,}"
 
 - name: AWS Multi
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>(AKIA|ASIA)[0-9A-Z]{16,17})([^=0-9A-Za-z_/+-]|$)
     - (?P<value>[0-9a-zA-Z/+]{40})
@@ -140,15 +165,15 @@
     - ya29.
   min_line_len: 27
 
 - name: Heroku API Key
   severity: high
   type: pattern
   values:
-    - (?P<value>(?i)heroku(.{0,20})?[0-9a-f]{8}(-[0-9a-f]{4})+-[0-9a-f]{12})([^=0-9A-Za-z_/+-]|$)
+    - (?i)(?P<value>heroku(.{0,20})?[0-9a-f]{8}(-[0-9a-f]{4})+-[0-9a-f]{12})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
   use_ml: true
   required_substrings:
     - heroku
   min_line_len: 24
 
 - name: Instagram Access Token
@@ -197,21 +222,22 @@
     - key-
   min_line_len: 36
 
 - name: Password
   severity: medium
   type: keyword
   values:
-    - pass|pw(d|\b)
+    - (?<!by)pass(?!ed|ing|es)|pw(d|\b)
   filter_type: PasswordKeyword
   use_ml: true
   min_line_len: 10
   required_substrings:
     - pass
     - pw
+  doc_available: false
 
 - name: PayPal Braintree Access Token
   severity: high
   type: pattern
   values:
     - (?P<value>access_token\$production\$[0-9a-z]{16}\$[0-9a-z]{32})([^=0-9A-Za-z_/+-]|$)
   filter_type: GeneralPattern
@@ -582,42 +608,46 @@
 - name: Bitbucket Client ID
   severity: info
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>[a-zA-Z0-9]{18}([a-zA-Z0-9]{14})?)([^0-9A-Za-z.$_/+-]|$)
   filter_type: WeirdBase64Token
   min_line_len: 18
+  required_regex: "[a-zA-Z0-9_/+-]{15,}"
 
 - name: Bitbucket Client Secret
   severity: info
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>([a-zA-Z0-9_-]{32}){1,2})([^0-9A-Za-z.$_/+-]|$)
   filter_type: WeirdBase64Token
   min_line_len: 32
+  required_regex: "[a-zA-Z0-9_/+-]{15,}"
 
 - name: Jira / Confluence PAT token
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>[NMO][ADgjQTwz][a-zA-Z0-9+/]{42})([^=0-9A-Za-z_/+-]|$)
   filter_type: StructuredToken
   min_line_len: 44
   required_substrings:
     - M
     - N
     - O
+  required_regex: "[a-zA-Z0-9_/+-]{15,}"
 
 - name: Atlassian Old PAT token
   severity: info
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>[a-zA-Z0-9]{24})([^=0-9A-Za-z.$_/+-]|$)
   filter_type: WeirdBase64Token
   min_line_len: 24
+  required_regex: "[a-zA-Z0-9_/+-]{15,}"
 
 - name: Atlassian PAT token
   severity: high
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>ATATT3xFfGF0[a-zA-Z0-9-_]{171}=[A-F0-9]{8})([^=0-9A-Za-z_/+-]|$)
   filter_type: TokenPattern
@@ -740,37 +770,40 @@
 - name: Dropbox App secret
   severity: info
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>[a-z0-9]{15})([^=0-9A-Za-z_/+-]|$)
   filter_type: WeirdBase36Token
   min_line_len: 15
+  required_regex: "[a-zA-Z0-9_/+-]{15,}"
 
 - name: Gitlab Incoming Email Token
   severity: info
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>[a-z0-9]{24,25})([^=0-9A-Za-z_/+-]|$)
   filter_type: WeirdBase36Token
   min_line_len: 24
+  required_regex: "[a-zA-Z0-9_/+-]{15,}"
 
 - name: Gitlab Feed Token
   severity: info
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>[a-zA-Z0-9_-]{20})([^=0-9A-Za-z_/+-]|$)
   filter_type: WeirdBase64Token
   min_line_len: 20
+  required_regex: "[a-zA-Z0-9_/+-]{15,}"
 
 - name: Jira 2FA
   severity: info
   type: pattern
   values:
     - (^|[^.0-9A-Za-z_/+-])(?P<value>[A-Z2-7]{16})([^=0-9A-Za-z_/+-]|$)
   filter_type:
     - ValueCoupleKeywordCheck
     - ValuePatternCheck
     - ValueEntropyBase32Check
     - ValueBase32DataCheck
     - ValueTokenBase32Check
   min_line_len: 16
-  doc_available: true
+  required_regex: "[a-zA-Z0-9_/+-]{15,}"
```

### Comparing `credsweeper-1.5.3/credsweeper/rules/rule.py` & `credsweeper-1.5.4/credsweeper/rules/rule.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/scanner/scan_type/multi_pattern.py` & `credsweeper-1.5.4/credsweeper/scanner/scan_type/multi_pattern.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/scanner/scan_type/pem_key_pattern.py` & `credsweeper-1.5.4/credsweeper/scanner/scan_type/pem_key_pattern.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/scanner/scan_type/scan_type.py` & `credsweeper-1.5.4/credsweeper/scanner/scan_type/scan_type.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/scanner/scan_type/single_pattern.py` & `credsweeper-1.5.4/credsweeper/scanner/scan_type/single_pattern.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/scanner/scanner.py` & `credsweeper-1.5.4/credsweeper/scanner/scanner.py`

 * *Files 9% similar despite different names*

```diff
@@ -87,29 +87,14 @@
         for rule, scanner in self.rules_scanners:
             if line_len >= rule.min_line_len \
                     and (RuleType.PATTERN == rule.rule_type and matched_pattern
                          or RuleType.KEYWORD == rule.rule_type and matched_keyword
                          or RuleType.PEM_KEY == rule.rule_type and matched_pem_key):
                 yield rule, scanner
 
-    @staticmethod
-    def _required_substrings_not_present(required_substrings: List[str], line: str) -> bool:
-        """ returns True if required substring absent in line """
-        for substring in required_substrings:
-            if substring in line:
-                return False
-        return True
-
-    @staticmethod
-    def _required_regex_not_matched(required_regex: re.Pattern, line: str) -> bool:
-        """ returns True if line does not matched required_regex """
-        if required_regex.match(line):
-            return False
-        return True
-
     def scan(self, provider: ContentProvider) -> List[Candidate]:
         """Run scanning of list of target lines from 'targets' with set of rule from 'self.rules'.
 
         Args:
             provider: objects with data to analyze: line, line number,
               filepath and all lines in file
```

### Comparing `credsweeper-1.5.3/credsweeper/secret/config.json` & `credsweeper-1.5.4/credsweeper/secret/config.json`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/secret/log.yaml` & `credsweeper-1.5.4/credsweeper/secret/log.yaml`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/utils/entropy_validator.py` & `credsweeper-1.5.4/credsweeper/utils/entropy_validator.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/utils/util.py` & `credsweeper-1.5.4/credsweeper/utils/util.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/validations/__init__.py` & `credsweeper-1.5.4/credsweeper/validations/__init__.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/validations/apply_validation.py` & `credsweeper-1.5.4/credsweeper/validations/apply_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/validations/github_token_validation.py` & `credsweeper-1.5.4/credsweeper/validations/github_token_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/validations/google_api_key_validation.py` & `credsweeper-1.5.4/credsweeper/validations/google_api_key_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/validations/google_multi_validation.py` & `credsweeper-1.5.4/credsweeper/validations/google_multi_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/validations/mailchimp_key_validation.py` & `credsweeper-1.5.4/credsweeper/validations/mailchimp_key_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/validations/slack_token_validation.py` & `credsweeper-1.5.4/credsweeper/validations/slack_token_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/validations/square_access_token_validation.py` & `credsweeper-1.5.4/credsweeper/validations/square_access_token_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/validations/square_client_id_validation.py` & `credsweeper-1.5.4/credsweeper/validations/square_client_id_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/validations/stripe_api_key_validation.py` & `credsweeper-1.5.4/credsweeper/validations/stripe_api_key_validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper/validations/validation.py` & `credsweeper-1.5.4/credsweeper/validations/validation.py`

 * *Files identical despite different names*

### Comparing `credsweeper-1.5.3/credsweeper.egg-info/PKG-INFO` & `credsweeper-1.5.4/credsweeper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: credsweeper
-Version: 1.5.3
+Version: 1.5.4
 Summary: Credential Sweeper
 Home-page: https://github.com/Samsung/CredSweeper
 Project-URL: Bug Tracker, https://github.com/Samsung/CredSweeper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `credsweeper-1.5.3/credsweeper.egg-info/SOURCES.txt` & `credsweeper-1.5.4/credsweeper.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -50,33 +50,34 @@
 credsweeper/file_handler/files_provider.py
 credsweeper/file_handler/patch_provider.py
 credsweeper/file_handler/string_content_provider.py
 credsweeper/file_handler/struct_content_provider.py
 credsweeper/file_handler/text_content_provider.py
 credsweeper/file_handler/text_provider.py
 credsweeper/filters/__init__.py
-credsweeper/filters/cred_card_number_check.py
 credsweeper/filters/filter.py
 credsweeper/filters/line_specific_key_check.py
 credsweeper/filters/separator_unusual_check.py
 credsweeper/filters/value_allowlist_check.py
 credsweeper/filters/value_array_dictionary_check.py
 credsweeper/filters/value_base32_data_check.py
 credsweeper/filters/value_base64_data_check.py
 credsweeper/filters/value_blocklist_check.py
 credsweeper/filters/value_camel_case_check.py
+credsweeper/filters/value_card_number_check.py
 credsweeper/filters/value_couple_keyword_check.py
 credsweeper/filters/value_dictionary_keyword_check.py
 credsweeper/filters/value_dictionary_value_length_check.py
 credsweeper/filters/value_entropy_base32_check.py
 credsweeper/filters/value_entropy_base36_check.py
 credsweeper/filters/value_entropy_base64_check.py
 credsweeper/filters/value_file_path_check.py
 credsweeper/filters/value_first_word_check.py
 credsweeper/filters/value_grafana_check.py
+credsweeper/filters/value_iban_check.py
 credsweeper/filters/value_json_web_token_check.py
 credsweeper/filters/value_last_word_check.py
 credsweeper/filters/value_length_check.py
 credsweeper/filters/value_method_check.py
 credsweeper/filters/value_not_allowed_pattern_check.py
 credsweeper/filters/value_not_part_encoded_check.py
 credsweeper/filters/value_number_check.py
@@ -88,14 +89,15 @@
 credsweeper/filters/value_string_type_check.py
 credsweeper/filters/value_structured_token_check.py
 credsweeper/filters/value_token_base32_check.py
 credsweeper/filters/value_token_base36_check.py
 credsweeper/filters/value_token_base64_check.py
 credsweeper/filters/value_token_check.py
 credsweeper/filters/value_useless_word_check.py
+credsweeper/filters/value_vin_check.py
 credsweeper/filters/variable_not_allowed_pattern_check.py
 credsweeper/filters/group/__init__.py
 credsweeper/filters/group/general_keyword.py
 credsweeper/filters/group/general_pattern.py
 credsweeper/filters/group/group.py
 credsweeper/filters/group/password_keyword.py
 credsweeper/filters/group/structured_token.py
```

### Comparing `credsweeper-1.5.3/setup.py` & `credsweeper-1.5.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     "openpyxl",  #
     "pandas",  #
     "password-strength",  #
     "pdfminer.six",  #
     "PyYAML",  #
     "requests",  #
     "scipy",  #
+    "schwifty",  #
     "typing_extensions",  #
     "whatthepatch",  #
     "numpy",  #
     "scikit-learn",  #
     "onnxruntime",  #
 ]
```

### Comparing `credsweeper-1.5.3/tests/test_app.py` & `credsweeper-1.5.4/tests/test_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -586,16 +586,14 @@
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_rules_ml_p(self) -> None:
         # checks whether all rules have positive test samples with almost the same arguments during benchmark
         with tempfile.TemporaryDirectory() as tmp_dir:
             json_filename = os.path.join(tmp_dir, f"{__name__}.json")
             _stdout, _stderr = self._m_credsweeper([
-                "--log",
-                "debug",
                 "--path",
                 str(SAMPLES_PATH),
                 "--save-json",
                 json_filename,
             ])
             self.assertEqual(0, len(_stderr))
             report = Util.json_load(json_filename)
@@ -610,16 +608,14 @@
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_rules_ml_n(self) -> None:
         # checks whether all rules have test samples which detected without ML
         with tempfile.TemporaryDirectory() as tmp_dir:
             json_filename = os.path.join(tmp_dir, f"{__name__}.json")
             _stdout, _stderr = self._m_credsweeper([
-                "--log",
-                "debug",
                 "--path",
                 str(SAMPLES_PATH),
                 "--ml_threshold",
                 "0",
                 "--save-json",
                 json_filename,
             ])
```

### Comparing `credsweeper-1.5.3/tests/test_main.py` & `credsweeper-1.5.4/tests/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -609,20 +609,20 @@
         # test for finding credentials in html
         content_provider: FilesProvider = TextProvider([SAMPLES_PATH / "test.html"])
         cred_sweeper = CredSweeper(depth=5)
         cred_sweeper.run(content_provider=content_provider)
         found_credentials = cred_sweeper.credential_manager.get_credentials()
         expected_credential_lines = [
             "508627689:AAEuLPKs-EhrjrYGnz60bnYNZqakf6HJxc0",
-            'secret = "Ndjbwu88s22ygavsdhgt5454v3h1x"',
-            'password = "Cr3DeHTbIal"',
-            'password = "0dm1nk0"',
-            '"password" = "p@$$w0Rd42"',
-            'secret = "BNbNbws73bdhss329ssakKhds120384"',
-            '"token" = "H72gsdv2dswPneHduwhfd"',
+            "secret = Ndjbwu88s22ygavsdhgt5454v3h1x",
+            "password = Cr3DeHTbIal",
+            "password = 0dm1nk0",
+            "password = p@$$w0Rd42",
+            "secret = BNbNbws73bdhss329ssakKhds120384",
+            "token = H72gsdv2dswPneHduwhfd",
         ]
         self.assertEqual(len(expected_credential_lines), len(found_credentials))
         for cred in found_credentials:
             self.assertEqual(1, len(cred.line_data_list))
             self.assertIn(cred.line_data_list[0].line, expected_credential_lines)
             expected_credential_lines.remove(cred.line_data_list[0].line)
         self.assertEqual(0, len(expected_credential_lines))
@@ -695,18 +695,15 @@
     # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #
 
     def test_doc_p(self) -> None:
         content_provider: FilesProvider = TextProvider([SAMPLES_PATH / "test.html"])
         cred_sweeper = CredSweeper(doc=True)
         cred_sweeper.run(content_provider=content_provider)
         found_credentials = cred_sweeper.credential_manager.get_credentials()
-        expected_credential_lines = [
-            "508627689:AAEuLPKs-EhrjrYGnz60bnYNZqakf6HJxc0", 'password = "0dm1nk0"', 'password = "Cr3DeHTbIal"',
-            '"password" = "p@$$w0Rd42"'
-        ]
+        expected_credential_lines = ["508627689:AAEuLPKs-EhrjrYGnz60bnYNZqakf6HJxc0"]
         self.assertEqual(len(expected_credential_lines), len(found_credentials))
         for cred in found_credentials:
             self.assertEqual(1, len(cred.line_data_list))
             self.assertIn(cred.line_data_list[0].line, expected_credential_lines)
             expected_credential_lines.remove(cred.line_data_list[0].line)
         self.assertEqual(0, len(expected_credential_lines))
```

