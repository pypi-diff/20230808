# Comparing `tmp/azure-search-documents-11.4.0b6.zip` & `tmp/azure-search-documents-11.4.0b7.zip`

## zipinfo {}

```diff
@@ -1,200 +1,200 @@
-Zip file size: 425691 bytes, number of entries: 198
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 22:23 azure-search-documents-11.4.0b6/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 22:23 azure-search-documents-11.4.0b6/tests/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 22:23 azure-search-documents-11.4.0b6/azure/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 22:23 azure-search-documents-11.4.0b6/samples/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 22:23 azure-search-documents-11.4.0b6/azure_search_documents.egg-info/
--rw-rw-r--  2.0 unx    22754 b- defN 23-Jul-11 22:23 azure-search-documents-11.4.0b6/PKG-INFO
--rw-rw-r--  2.0 unx    10696 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/CHANGELOG.md
--rw-rw-r--  2.0 unx    21853 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/README.md
--rw-rw-r--  2.0 unx     4081 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/TROUBLESHOOTING.md
--rw-rw-r--  2.0 unx     1073 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/LICENSE
--rw-rw-r--  2.0 unx       38 b- defN 23-Jul-11 22:23 azure-search-documents-11.4.0b6/setup.cfg
--rw-rw-r--  2.0 unx       52 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/pyproject.toml
--rw-rw-r--  2.0 unx     2365 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/setup.py
--rw-rw-r--  2.0 unx      193 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/MANIFEST.in
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 22:23 azure-search-documents-11.4.0b6/tests/async_tests/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 22:23 azure-search-documents-11.4.0b6/tests/perfstress_tests/
--rw-rw-r--  2.0 unx     6841 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/test_search_index_client_data_source_live.py
--rw-rw-r--  2.0 unx     4976 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/test_search_client_search_live.py
--rw-rw-r--  2.0 unx     5734 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/test_search_index_client_synonym_map_live.py
--rw-rw-r--  2.0 unx     4583 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/test_regex_flags.py
--rw-rw-r--  2.0 unx     6365 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/test_buffered_sender.py
--rw-rw-r--  2.0 unx     7246 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/test_search_index_client_live.py
--rw-rw-r--  2.0 unx     2164 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/test_index_documents_batch.py
--rw-rw-r--  2.0 unx    11683 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/test_search_index_client_skillset_live.py
--rw-rw-r--  2.0 unx     3103 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/test_index_field_helpers.py
--rw-rw-r--  2.0 unx     5887 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/test_queries.py
--rw-rw-r--  2.0 unx     1227 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/conftest.py
--rw-rw-r--  2.0 unx    29355 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/search_service_preparer.py
--rw-rw-r--  2.0 unx    14512 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/test_search_client.py
--rw-rw-r--  2.0 unx     7372 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/test_search_indexer_client_live.py
--rw-rw-r--  2.0 unx     6740 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/test_search_client_buffered_sender_live.py
--rw-rw-r--  2.0 unx     6583 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/test_search_client_index_document_live.py
--rw-rw-r--  2.0 unx     4068 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/test_search_index_client_alias_live.py
--rw-rw-r--  2.0 unx     4980 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/test_search_index_client.py
--rw-rw-r--  2.0 unx     1938 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/test_search_client_basic_live.py
--rw-rw-r--  2.0 unx     6902 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/async_tests/test_search_client_index_document_live_async.py
--rw-rw-r--  2.0 unx     6087 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/async_tests/test_search_index_client_synonym_map_live_async.py
--rw-rw-r--  2.0 unx     4392 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/async_tests/test_search_index_client_alias_live_async.py
--rw-rw-r--  2.0 unx     6298 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/async_tests/test_search_index_client_data_source_live_async.py
--rw-rw-r--  2.0 unx     1364 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/async_tests/test_search_client_async.py
--rw-rw-r--  2.0 unx     2157 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/async_tests/test_search_client_basic_live_async.py
--rw-rw-r--  2.0 unx     7177 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/async_tests/test_search_client_buffered_sender_live_async.py
--rw-rw-r--  2.0 unx    10245 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/async_tests/test_search_index_client_skillset_live_async.py
--rw-rw-r--  2.0 unx     7689 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/async_tests/test_search_index_client_live_async.py
--rw-rw-r--  2.0 unx     3942 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/async_tests/test_search_index_client_async.py
--rw-rw-r--  2.0 unx     7955 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/async_tests/test_search_indexer_client_live_async.py
--rw-rw-r--  2.0 unx     6255 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/async_tests/test_search_client_search_live_async.py
--rw-rw-r--  2.0 unx     6385 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/async_tests/test_buffered_sender_async.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/perfstress_tests/__init__.py
--rw-rw-r--  2.0 unx     2247 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/perfstress_tests/search_documents.py
--rw-rw-r--  2.0 unx     2287 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/perfstress_tests/autocomplete.py
--rw-rw-r--  2.0 unx     2252 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/tests/perfstress_tests/suggest.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 22:23 azure-search-documents-11.4.0b6/azure/search/
--rw-rw-r--  2.0 unx      264 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 22:23 azure-search-documents-11.4.0b6/azure/search/documents/
--rw-rw-r--  2.0 unx      264 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 22:23 azure-search-documents-11.4.0b6/azure/search/documents/indexes/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 22:23 azure-search-documents-11.4.0b6/azure/search/documents/models/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 22:23 azure-search-documents-11.4.0b6/azure/search/documents/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 22:23 azure-search-documents-11.4.0b6/azure/search/documents/_generated/
--rw-rw-r--  2.0 unx      769 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/_headers_mixin.py
--rw-rw-r--  2.0 unx      498 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/_api_versions.py
--rw-rw-r--  2.0 unx    36112 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/_search_client.py
--rw-rw-r--  2.0 unx      252 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/_version.py
--rw-rw-r--  2.0 unx     3518 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/_queries.py
--rw-rw-r--  2.0 unx     1822 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/__init__.py
--rw-rw-r--  2.0 unx      491 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/_search_documents_error.py
--rw-rw-r--  2.0 unx    14785 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/_search_indexing_buffered_sender.py
--rw-rw-r--  2.0 unx     1825 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/_utils.py
--rw-rw-r--  2.0 unx     6063 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/_index_documents_batch.py
--rw-rw-r--  2.0 unx     2087 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/_search_indexing_buffered_sender_base.py
--rw-rw-r--  2.0 unx     5590 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/_paging.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/py.typed
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 22:23 azure-search-documents-11.4.0b6/azure/search/documents/indexes/models/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 22:23 azure-search-documents-11.4.0b6/azure/search/documents/indexes/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 22:23 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/
--rw-rw-r--  2.0 unx    26062 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_search_index_client.py
--rw-rw-r--  2.0 unx    30990 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_search_indexer_client.py
--rw-rw-r--  2.0 unx     1479 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/__init__.py
--rw-rw-r--  2.0 unx     3140 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_utils.py
--rw-rw-r--  2.0 unx    44098 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/models/_models.py
--rw-rw-r--  2.0 unx    43360 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/models/_index.py
--rw-rw-r--  2.0 unx    10333 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/models/__init__.py
--rw-rw-r--  2.0 unx      624 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/models/_edm.py
--rw-rw-r--  2.0 unx    27028 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/aio/_search_index_client.py
--rw-rw-r--  2.0 unx    30044 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/aio/_search_indexer_client.py
--rw-rw-r--  2.0 unx     1479 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/aio/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 22:23 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/models/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 22:23 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 22:23 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/operations/
--rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/_patch.py
--rw-rw-r--  2.0 unx    78836 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/_serialization.py
--rw-rw-r--  2.0 unx     2467 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/_configuration.py
--rw-rw-r--  2.0 unx      742 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/__init__.py
--rw-rw-r--  2.0 unx     5032 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/_search_service_client.py
--rw-rw-r--  2.0 unx     1720 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/_vendor.py
--rw-rw-r--  2.0 unx    70564 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/models/_search_service_client_enums.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/models/_patch.py
--rw-rw-r--  2.0 unx    16331 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/models/__init__.py
--rw-rw-r--  2.0 unx   490136 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/models/_models_py3.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 22:23 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/operations/
--rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/_patch.py
--rw-rw-r--  2.0 unx     2477 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/_configuration.py
--rw-rw-r--  2.0 unx      742 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/__init__.py
--rw-rw-r--  2.0 unx     5161 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/_search_service_client.py
--rw-rw-r--  2.0 unx      955 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/_vendor.py
--rw-rw-r--  2.0 unx    27236 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/operations/_synonym_maps_operations.py
--rw-rw-r--  2.0 unx     4160 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/operations/_search_service_client_operations.py
--rw-rw-r--  2.0 unx    40542 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/operations/_indexes_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/operations/_patch.py
--rw-rw-r--  2.0 unx     1220 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/operations/__init__.py
--rw-rw-r--  2.0 unx    35901 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/operations/_skillsets_operations.py
--rw-rw-r--  2.0 unx    28599 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/operations/_data_sources_operations.py
--rw-rw-r--  2.0 unx    28586 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/operations/_aliases_operations.py
--rw-rw-r--  2.0 unx    45076 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/operations/_indexers_operations.py
--rw-rw-r--  2.0 unx    33802 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/operations/_synonym_maps_operations.py
--rw-rw-r--  2.0 unx     5049 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/operations/_search_service_client_operations.py
--rw-rw-r--  2.0 unx    49565 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/operations/_indexes_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/operations/_patch.py
--rw-rw-r--  2.0 unx     1220 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/operations/__init__.py
--rw-rw-r--  2.0 unx    44430 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/operations/_skillsets_operations.py
--rw-rw-r--  2.0 unx    35474 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/operations/_data_sources_operations.py
--rw-rw-r--  2.0 unx    34800 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/operations/_aliases_operations.py
--rw-rw-r--  2.0 unx    57126 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/operations/_indexers_operations.py
--rw-rw-r--  2.0 unx     2012 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/models/__init__.py
--rw-rw-r--  2.0 unx    15161 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/aio/_search_indexing_buffered_sender_async.py
--rw-rw-r--  2.0 unx    37001 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/aio/_search_client_async.py
--rw-rw-r--  2.0 unx     1553 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/aio/__init__.py
--rw-rw-r--  2.0 unx      673 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/aio/_timer.py
--rw-rw-r--  2.0 unx     5886 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/aio/_index_documents_batch_async.py
--rw-rw-r--  2.0 unx     5174 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/aio/_paging.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 22:23 azure-search-documents-11.4.0b6/azure/search/documents/_generated/models/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 22:23 azure-search-documents-11.4.0b6/azure/search/documents/_generated/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 22:23 azure-search-documents-11.4.0b6/azure/search/documents/_generated/operations/
--rw-rw-r--  2.0 unx     3793 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/_generated/_search_index_client.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/_generated/_patch.py
--rw-rw-r--  2.0 unx    78836 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/_generated/_serialization.py
--rw-rw-r--  2.0 unx     2699 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/_generated/_configuration.py
--rw-rw-r--  2.0 unx      736 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/_generated/__init__.py
--rw-rw-r--  2.0 unx     1200 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/_generated/_vendor.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/_generated/models/_patch.py
--rw-rw-r--  2.0 unx    15706 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/_generated/models/_search_index_client_enums.py
--rw-rw-r--  2.0 unx     3704 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/_generated/models/__init__.py
--rw-rw-r--  2.0 unx   103482 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/_generated/models/_models_py3.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 22:23 azure-search-documents-11.4.0b6/azure/search/documents/_generated/aio/operations/
--rw-rw-r--  2.0 unx     3902 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/_generated/aio/_search_index_client.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/_generated/aio/_patch.py
--rw-rw-r--  2.0 unx     2709 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/_generated/aio/_configuration.py
--rw-rw-r--  2.0 unx      736 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/_generated/aio/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/_generated/aio/operations/_patch.py
--rw-rw-r--  2.0 unx    51145 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/_generated/aio/operations/_documents_operations.py
--rw-rw-r--  2.0 unx      687 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/_generated/aio/operations/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/_generated/operations/_patch.py
--rw-rw-r--  2.0 unx    68985 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/_generated/operations/_documents_operations.py
--rw-rw-r--  2.0 unx      687 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/azure/search/documents/_generated/operations/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 22:23 azure-search-documents-11.4.0b6/samples/async_samples/
--rw-rw-r--  2.0 unx     2823 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/sample_data_source_operations.py
--rw-rw-r--  2.0 unx     2246 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/sample_authentication.py
--rw-rw-r--  2.0 unx     3875 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/sample_indexers_operations.py
--rw-rw-r--  2.0 unx     2899 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/sample_synonym_map_operations.py
--rw-rw-r--  2.0 unx     1785 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/sample_buffered_sender.py
--rw-rw-r--  2.0 unx     1587 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/sample_get_document.py
--rw-rw-r--  2.0 unx     1557 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/sample_analyze_text.py
--rw-rw-r--  2.0 unx     6100 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/README.md
--rw-rw-r--  2.0 unx     2373 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/sample_semantic_search.py
--rw-rw-r--  2.0 unx     3272 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/sample_index_alias_crud_operations.py
--rw-rw-r--  2.0 unx     1759 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/sample_filter_query.py
--rw-rw-r--  2.0 unx     3648 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/sample_index_crud_operations.py
--rw-rw-r--  2.0 unx     1561 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/sample_autocomplete.py
--rw-rw-r--  2.0 unx     5964 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/sample_indexer_datasource_skillset.py
--rw-rw-r--  2.0 unx     1581 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/sample_simple_query.py
--rw-rw-r--  2.0 unx     1583 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/sample_facet_query.py
--rw-rw-r--  2.0 unx     6707 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/sample_vector_search.py
--rw-rw-r--  2.0 unx     1627 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/sample_suggestions.py
--rw-rw-r--  2.0 unx     2163 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/sample_crud_operations.py
--rw-rw-r--  2.0 unx     2347 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/async_samples/sample_semantic_search_async.py
--rw-rw-r--  2.0 unx     2361 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/async_samples/sample_crud_operations_async.py
--rw-rw-r--  2.0 unx     4350 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/async_samples/sample_indexers_operations_async.py
--rw-rw-r--  2.0 unx     1708 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/async_samples/sample_facet_query_async.py
--rw-rw-r--  2.0 unx     1656 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/async_samples/sample_analyze_text_async.py
--rw-rw-r--  2.0 unx     3498 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/async_samples/sample_index_alias_crud_operations_async.py
--rw-rw-r--  2.0 unx     1753 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/async_samples/sample_suggestions_async.py
--rw-rw-r--  2.0 unx     1702 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/async_samples/sample_simple_query_async.py
--rw-rw-r--  2.0 unx     1896 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/async_samples/sample_buffered_sender_async.py
--rw-rw-r--  2.0 unx     2385 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/async_samples/sample_authentication_async.py
--rw-rw-r--  2.0 unx     3870 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/async_samples/sample_index_crud_operations_async.py
--rw-rw-r--  2.0 unx     2544 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/async_samples/sample_synonym_map_operations_async.py
--rw-rw-r--  2.0 unx     7109 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/async_samples/sample_vector_search_async.py
--rw-rw-r--  2.0 unx     1900 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/async_samples/sample_filter_query_async.py
--rw-rw-r--  2.0 unx     3080 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/async_samples/sample_data_source_operations_async.py
--rw-rw-r--  2.0 unx     1676 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/async_samples/sample_autocomplete_async.py
--rw-rw-r--  2.0 unx     1718 b- defN 23-Jul-11 22:21 azure-search-documents-11.4.0b6/samples/async_samples/sample_get_document_async.py
--rw-rw-r--  2.0 unx    22754 b- defN 23-Jul-11 22:23 azure-search-documents-11.4.0b6/azure_search_documents.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx       59 b- defN 23-Jul-11 22:23 azure-search-documents-11.4.0b6/azure_search_documents.egg-info/requires.txt
--rw-rw-r--  2.0 unx     8510 b- defN 23-Jul-11 22:23 azure-search-documents-11.4.0b6/azure_search_documents.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Jul-11 22:23 azure-search-documents-11.4.0b6/azure_search_documents.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx        6 b- defN 23-Jul-11 22:23 azure-search-documents-11.4.0b6/azure_search_documents.egg-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Jul-11 22:23 azure-search-documents-11.4.0b6/azure_search_documents.egg-info/dependency_links.txt
-198 files, 2268223 bytes uncompressed, 379703 bytes compressed:  83.3%
+Zip file size: 426033 bytes, number of entries: 198
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 23:22 azure-search-documents-11.4.0b7/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 23:22 azure-search-documents-11.4.0b7/azure/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 23:22 azure-search-documents-11.4.0b7/tests/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 23:22 azure-search-documents-11.4.0b7/samples/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 23:22 azure-search-documents-11.4.0b7/azure_search_documents.egg-info/
+-rw-rw-r--  2.0 unx    21923 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/README.md
+-rw-rw-r--  2.0 unx       52 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/pyproject.toml
+-rw-rw-r--  2.0 unx    11178 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/CHANGELOG.md
+-rw-rw-r--  2.0 unx     1073 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/LICENSE
+-rw-rw-r--  2.0 unx       38 b- defN 23-Aug-07 23:22 azure-search-documents-11.4.0b7/setup.cfg
+-rw-rw-r--  2.0 unx     4081 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/TROUBLESHOOTING.md
+-rw-rw-r--  2.0 unx      193 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/MANIFEST.in
+-rw-rw-r--  2.0 unx    22824 b- defN 23-Aug-07 23:22 azure-search-documents-11.4.0b7/PKG-INFO
+-rw-rw-r--  2.0 unx     2365 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/setup.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 23:22 azure-search-documents-11.4.0b7/azure/search/
+-rw-rw-r--  2.0 unx      264 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 23:22 azure-search-documents-11.4.0b7/azure/search/documents/
+-rw-rw-r--  2.0 unx      264 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 23:22 azure-search-documents-11.4.0b7/azure/search/documents/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 23:22 azure-search-documents-11.4.0b7/azure/search/documents/_generated/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 23:22 azure-search-documents-11.4.0b7/azure/search/documents/indexes/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 23:22 azure-search-documents-11.4.0b7/azure/search/documents/aio/
+-rw-rw-r--  2.0 unx      252 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/_version.py
+-rw-rw-r--  2.0 unx     3518 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/_queries.py
+-rw-rw-r--  2.0 unx     2087 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/_search_indexing_buffered_sender_base.py
+-rw-rw-r--  2.0 unx     5590 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/_paging.py
+-rw-rw-r--  2.0 unx    14785 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/_search_indexing_buffered_sender.py
+-rw-rw-r--  2.0 unx    35616 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/_search_client.py
+-rw-rw-r--  2.0 unx     1822 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/__init__.py
+-rw-rw-r--  2.0 unx      498 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/_api_versions.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/py.typed
+-rw-rw-r--  2.0 unx     1825 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/_utils.py
+-rw-rw-r--  2.0 unx     6063 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/_index_documents_batch.py
+-rw-rw-r--  2.0 unx      769 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/_headers_mixin.py
+-rw-rw-r--  2.0 unx      491 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/_search_documents_error.py
+-rw-rw-r--  2.0 unx     2012 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/models/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 23:22 azure-search-documents-11.4.0b7/azure/search/documents/_generated/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 23:22 azure-search-documents-11.4.0b7/azure/search/documents/_generated/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 23:22 azure-search-documents-11.4.0b7/azure/search/documents/_generated/aio/
+-rw-rw-r--  2.0 unx      674 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/_generated/_patch.py
+-rw-rw-r--  2.0 unx    79289 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/_generated/_serialization.py
+-rw-rw-r--  2.0 unx      735 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/_generated/__init__.py
+-rw-rw-r--  2.0 unx      675 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/_generated/_vendor.py
+-rw-rw-r--  2.0 unx     3792 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/_generated/_search_index_client.py
+-rw-rw-r--  2.0 unx     2698 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/_generated/_configuration.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/_generated/models/_patch.py
+-rw-rw-r--  2.0 unx    15705 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/_generated/models/_search_index_client_enums.py
+-rw-rw-r--  2.0 unx   103914 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/_generated/models/_models_py3.py
+-rw-rw-r--  2.0 unx     3703 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/_generated/models/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/_generated/operations/_patch.py
+-rw-rw-r--  2.0 unx      686 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/_generated/operations/__init__.py
+-rw-rw-r--  2.0 unx    68740 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/_generated/operations/_documents_operations.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 23:22 azure-search-documents-11.4.0b7/azure/search/documents/_generated/aio/operations/
+-rw-rw-r--  2.0 unx      674 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/_generated/aio/_patch.py
+-rw-rw-r--  2.0 unx      735 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/_generated/aio/__init__.py
+-rw-rw-r--  2.0 unx     3901 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/_generated/aio/_search_index_client.py
+-rw-rw-r--  2.0 unx     2708 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/_generated/aio/_configuration.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/_generated/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx      686 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/_generated/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx    50935 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/_generated/aio/operations/_documents_operations.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 23:22 azure-search-documents-11.4.0b7/azure/search/documents/indexes/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 23:22 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 23:22 azure-search-documents-11.4.0b7/azure/search/documents/indexes/aio/
+-rw-rw-r--  2.0 unx    30990 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_search_indexer_client.py
+-rw-rw-r--  2.0 unx     1479 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/__init__.py
+-rw-rw-r--  2.0 unx     3140 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_utils.py
+-rw-rw-r--  2.0 unx    26062 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_search_index_client.py
+-rw-rw-r--  2.0 unx      624 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/models/_edm.py
+-rw-rw-r--  2.0 unx    10333 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/models/__init__.py
+-rw-rw-r--  2.0 unx    43360 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/models/_index.py
+-rw-rw-r--  2.0 unx    44098 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/models/_models.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 23:22 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 23:22 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 23:22 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/
+-rw-rw-r--  2.0 unx      674 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/_patch.py
+-rw-rw-r--  2.0 unx    79289 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/_serialization.py
+-rw-rw-r--  2.0 unx      741 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/__init__.py
+-rw-rw-r--  2.0 unx     1214 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/_vendor.py
+-rw-rw-r--  2.0 unx     5031 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/_search_service_client.py
+-rw-rw-r--  2.0 unx     2466 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/_configuration.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/models/_patch.py
+-rw-rw-r--  2.0 unx    70652 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/models/_search_service_client_enums.py
+-rw-rw-r--  2.0 unx   492151 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/models/_models_py3.py
+-rw-rw-r--  2.0 unx    16440 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/models/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/operations/_patch.py
+-rw-rw-r--  2.0 unx    33738 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/operations/_synonym_maps_operations.py
+-rw-rw-r--  2.0 unx    34736 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/operations/_aliases_operations.py
+-rw-rw-r--  2.0 unx    49473 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/operations/_indexes_operations.py
+-rw-rw-r--  2.0 unx     1219 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/operations/__init__.py
+-rw-rw-r--  2.0 unx    44352 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/operations/_skillsets_operations.py
+-rw-rw-r--  2.0 unx    57006 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/operations/_indexers_operations.py
+-rw-rw-r--  2.0 unx     5048 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/operations/_search_service_client_operations.py
+-rw-rw-r--  2.0 unx    35410 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/operations/_data_sources_operations.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 23:22 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/operations/
+-rw-rw-r--  2.0 unx      674 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/_patch.py
+-rw-rw-r--  2.0 unx      741 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/__init__.py
+-rw-rw-r--  2.0 unx      954 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/_vendor.py
+-rw-rw-r--  2.0 unx     5160 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/_search_service_client.py
+-rw-rw-r--  2.0 unx     2476 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/_configuration.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx    27235 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/operations/_synonym_maps_operations.py
+-rw-rw-r--  2.0 unx    28585 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/operations/_aliases_operations.py
+-rw-rw-r--  2.0 unx    40541 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/operations/_indexes_operations.py
+-rw-rw-r--  2.0 unx     1219 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx    35900 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/operations/_skillsets_operations.py
+-rw-rw-r--  2.0 unx    45075 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/operations/_indexers_operations.py
+-rw-rw-r--  2.0 unx     4159 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/operations/_search_service_client_operations.py
+-rw-rw-r--  2.0 unx    28598 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/operations/_data_sources_operations.py
+-rw-rw-r--  2.0 unx    30044 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/aio/_search_indexer_client.py
+-rw-rw-r--  2.0 unx     1479 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/aio/__init__.py
+-rw-rw-r--  2.0 unx    27028 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/indexes/aio/_search_index_client.py
+-rw-rw-r--  2.0 unx     5886 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/aio/_index_documents_batch_async.py
+-rw-rw-r--  2.0 unx     5174 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/aio/_paging.py
+-rw-rw-r--  2.0 unx    15161 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/aio/_search_indexing_buffered_sender_async.py
+-rw-rw-r--  2.0 unx      673 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/aio/_timer.py
+-rw-rw-r--  2.0 unx     1553 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/aio/__init__.py
+-rw-rw-r--  2.0 unx    36505 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/azure/search/documents/aio/_search_client_async.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 23:22 azure-search-documents-11.4.0b7/tests/async_tests/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 23:22 azure-search-documents-11.4.0b7/tests/perfstress_tests/
+-rw-rw-r--  2.0 unx    11708 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/test_search_index_client_skillset_live.py
+-rw-rw-r--  2.0 unx     6608 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/test_search_client_index_document_live.py
+-rw-rw-r--  2.0 unx     5005 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/test_search_index_client.py
+-rw-rw-r--  2.0 unx     5001 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/test_search_client_search_live.py
+-rw-rw-r--  2.0 unx     4583 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/test_regex_flags.py
+-rw-rw-r--  2.0 unx     3103 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/test_index_field_helpers.py
+-rw-rw-r--  2.0 unx    14512 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/test_search_client.py
+-rw-rw-r--  2.0 unx     7354 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/test_search_index_client_live.py
+-rw-rw-r--  2.0 unx     6365 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/test_buffered_sender.py
+-rw-rw-r--  2.0 unx     4093 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/test_search_index_client_alias_live.py
+-rw-rw-r--  2.0 unx     2013 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/test_search_client_basic_live.py
+-rw-rw-r--  2.0 unx     2164 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/test_index_documents_batch.py
+-rw-rw-r--  2.0 unx    29548 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/search_service_preparer.py
+-rw-rw-r--  2.0 unx     6866 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/test_search_index_client_data_source_live.py
+-rw-rw-r--  2.0 unx     5759 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/test_search_index_client_synonym_map_live.py
+-rw-rw-r--  2.0 unx     7422 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/test_search_indexer_client_live.py
+-rw-rw-r--  2.0 unx     5887 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/test_queries.py
+-rw-rw-r--  2.0 unx     6790 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/test_search_client_buffered_sender_live.py
+-rw-rw-r--  2.0 unx     1227 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/conftest.py
+-rw-rw-r--  2.0 unx     6323 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/async_tests/test_search_index_client_data_source_live_async.py
+-rw-rw-r--  2.0 unx     8005 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/async_tests/test_search_indexer_client_live_async.py
+-rw-rw-r--  2.0 unx     2157 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/async_tests/test_search_client_basic_live_async.py
+-rw-rw-r--  2.0 unx     6927 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/async_tests/test_search_client_index_document_live_async.py
+-rw-rw-r--  2.0 unx     4417 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/async_tests/test_search_index_client_alias_live_async.py
+-rw-rw-r--  2.0 unx     6112 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/async_tests/test_search_index_client_synonym_map_live_async.py
+-rw-rw-r--  2.0 unx     1364 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/async_tests/test_search_client_async.py
+-rw-rw-r--  2.0 unx    10270 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/async_tests/test_search_index_client_skillset_live_async.py
+-rw-rw-r--  2.0 unx     7797 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/async_tests/test_search_index_client_live_async.py
+-rw-rw-r--  2.0 unx     7227 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/async_tests/test_search_client_buffered_sender_live_async.py
+-rw-rw-r--  2.0 unx     6385 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/async_tests/test_buffered_sender_async.py
+-rw-rw-r--  2.0 unx     3942 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/async_tests/test_search_index_client_async.py
+-rw-rw-r--  2.0 unx     6280 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/async_tests/test_search_client_search_live_async.py
+-rw-rw-r--  2.0 unx     2252 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/perfstress_tests/suggest.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/perfstress_tests/__init__.py
+-rw-rw-r--  2.0 unx     2287 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/perfstress_tests/autocomplete.py
+-rw-rw-r--  2.0 unx     2247 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/tests/perfstress_tests/search_documents.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-07 23:22 azure-search-documents-11.4.0b7/samples/async_samples/
+-rw-rw-r--  2.0 unx     6100 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/README.md
+-rw-rw-r--  2.0 unx     2899 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/sample_synonym_map_operations.py
+-rw-rw-r--  2.0 unx     1583 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/sample_facet_query.py
+-rw-rw-r--  2.0 unx     1581 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/sample_simple_query.py
+-rw-rw-r--  2.0 unx     1627 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/sample_suggestions.py
+-rw-rw-r--  2.0 unx     2163 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/sample_crud_operations.py
+-rw-rw-r--  2.0 unx     3873 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/sample_index_crud_operations.py
+-rw-rw-r--  2.0 unx     2373 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/sample_semantic_search.py
+-rw-rw-r--  2.0 unx     6783 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/sample_vector_search.py
+-rw-rw-r--  2.0 unx     1557 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/sample_analyze_text.py
+-rw-rw-r--  2.0 unx     5964 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/sample_indexer_datasource_skillset.py
+-rw-rw-r--  2.0 unx     3875 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/sample_indexers_operations.py
+-rw-rw-r--  2.0 unx     1587 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/sample_get_document.py
+-rw-rw-r--  2.0 unx     2823 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/sample_data_source_operations.py
+-rw-rw-r--  2.0 unx     1785 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/sample_buffered_sender.py
+-rw-rw-r--  2.0 unx     1759 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/sample_filter_query.py
+-rw-rw-r--  2.0 unx     1561 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/sample_autocomplete.py
+-rw-rw-r--  2.0 unx     3272 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/sample_index_alias_crud_operations.py
+-rw-rw-r--  2.0 unx     3353 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/sample_authentication.py
+-rw-rw-r--  2.0 unx     3498 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/async_samples/sample_index_alias_crud_operations_async.py
+-rw-rw-r--  2.0 unx     3579 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/async_samples/sample_authentication_async.py
+-rw-rw-r--  2.0 unx     2361 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/async_samples/sample_crud_operations_async.py
+-rw-rw-r--  2.0 unx     2544 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/async_samples/sample_synonym_map_operations_async.py
+-rw-rw-r--  2.0 unx     1702 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/async_samples/sample_simple_query_async.py
+-rw-rw-r--  2.0 unx     1753 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/async_samples/sample_suggestions_async.py
+-rw-rw-r--  2.0 unx     1708 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/async_samples/sample_facet_query_async.py
+-rw-rw-r--  2.0 unx     4170 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/async_samples/sample_index_crud_operations_async.py
+-rw-rw-r--  2.0 unx     1896 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/async_samples/sample_buffered_sender_async.py
+-rw-rw-r--  2.0 unx     1900 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/async_samples/sample_filter_query_async.py
+-rw-rw-r--  2.0 unx     1676 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/async_samples/sample_autocomplete_async.py
+-rw-rw-r--  2.0 unx     3080 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/async_samples/sample_data_source_operations_async.py
+-rw-rw-r--  2.0 unx     2347 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/async_samples/sample_semantic_search_async.py
+-rw-rw-r--  2.0 unx     7135 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/async_samples/sample_vector_search_async.py
+-rw-rw-r--  2.0 unx     4350 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/async_samples/sample_indexers_operations_async.py
+-rw-rw-r--  2.0 unx     1718 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/async_samples/sample_get_document_async.py
+-rw-rw-r--  2.0 unx     1656 b- defN 23-Aug-07 23:21 azure-search-documents-11.4.0b7/samples/async_samples/sample_analyze_text_async.py
+-rw-rw-r--  2.0 unx        1 b- defN 23-Aug-07 23:22 azure-search-documents-11.4.0b7/azure_search_documents.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx        6 b- defN 23-Aug-07 23:22 azure-search-documents-11.4.0b7/azure_search_documents.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Aug-07 23:22 azure-search-documents-11.4.0b7/azure_search_documents.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx       59 b- defN 23-Aug-07 23:22 azure-search-documents-11.4.0b7/azure_search_documents.egg-info/requires.txt
+-rw-rw-r--  2.0 unx     8510 b- defN 23-Aug-07 23:22 azure-search-documents-11.4.0b7/azure_search_documents.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx    22824 b- defN 23-Aug-07 23:22 azure-search-documents-11.4.0b7/azure_search_documents.egg-info/PKG-INFO
+198 files, 2273415 bytes uncompressed, 380045 bytes compressed:  83.3%
```

## zipnote {}

```diff
@@ -1,595 +1,595 @@
-Filename: azure-search-documents-11.4.0b6/
+Filename: azure-search-documents-11.4.0b7/
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/
+Filename: azure-search-documents-11.4.0b7/azure/
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/
+Filename: azure-search-documents-11.4.0b7/tests/
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/
+Filename: azure-search-documents-11.4.0b7/samples/
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure_search_documents.egg-info/
+Filename: azure-search-documents-11.4.0b7/azure_search_documents.egg-info/
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/PKG-INFO
+Filename: azure-search-documents-11.4.0b7/README.md
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/CHANGELOG.md
+Filename: azure-search-documents-11.4.0b7/pyproject.toml
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/README.md
+Filename: azure-search-documents-11.4.0b7/CHANGELOG.md
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/TROUBLESHOOTING.md
+Filename: azure-search-documents-11.4.0b7/LICENSE
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/LICENSE
+Filename: azure-search-documents-11.4.0b7/setup.cfg
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/setup.cfg
+Filename: azure-search-documents-11.4.0b7/TROUBLESHOOTING.md
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/pyproject.toml
+Filename: azure-search-documents-11.4.0b7/MANIFEST.in
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/setup.py
+Filename: azure-search-documents-11.4.0b7/PKG-INFO
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/MANIFEST.in
+Filename: azure-search-documents-11.4.0b7/setup.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/async_tests/
+Filename: azure-search-documents-11.4.0b7/azure/search/
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/perfstress_tests/
+Filename: azure-search-documents-11.4.0b7/azure/__init__.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/test_search_index_client_data_source_live.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/test_search_client_search_live.py
+Filename: azure-search-documents-11.4.0b7/azure/search/__init__.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/test_search_index_client_synonym_map_live.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/models/
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/test_regex_flags.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_generated/
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/test_buffered_sender.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/test_search_index_client_live.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/aio/
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/test_index_documents_batch.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_version.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/test_search_index_client_skillset_live.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_queries.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/test_index_field_helpers.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_search_indexing_buffered_sender_base.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/test_queries.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_paging.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/conftest.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_search_indexing_buffered_sender.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/search_service_preparer.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_search_client.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/test_search_client.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/__init__.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/test_search_indexer_client_live.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_api_versions.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/test_search_client_buffered_sender_live.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/py.typed
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/test_search_client_index_document_live.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_utils.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/test_search_index_client_alias_live.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_index_documents_batch.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/test_search_index_client.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_headers_mixin.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/test_search_client_basic_live.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_search_documents_error.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/async_tests/test_search_client_index_document_live_async.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/models/__init__.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/async_tests/test_search_index_client_synonym_map_live_async.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_generated/models/
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/async_tests/test_search_index_client_alias_live_async.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_generated/operations/
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/async_tests/test_search_index_client_data_source_live_async.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_generated/aio/
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/async_tests/test_search_client_async.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_generated/_patch.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/async_tests/test_search_client_basic_live_async.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_generated/_serialization.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/async_tests/test_search_client_buffered_sender_live_async.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_generated/__init__.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/async_tests/test_search_index_client_skillset_live_async.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_generated/_vendor.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/async_tests/test_search_index_client_live_async.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_generated/_search_index_client.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/async_tests/test_search_index_client_async.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_generated/_configuration.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/async_tests/test_search_indexer_client_live_async.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_generated/models/_patch.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/async_tests/test_search_client_search_live_async.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_generated/models/_search_index_client_enums.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/async_tests/test_buffered_sender_async.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_generated/models/_models_py3.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/perfstress_tests/__init__.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_generated/models/__init__.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/perfstress_tests/search_documents.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_generated/operations/_patch.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/perfstress_tests/autocomplete.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_generated/operations/__init__.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/tests/perfstress_tests/suggest.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_generated/operations/_documents_operations.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_generated/aio/operations/
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/__init__.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_generated/aio/_patch.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_generated/aio/__init__.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/__init__.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_generated/aio/_search_index_client.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_generated/aio/_configuration.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/models/
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_generated/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/aio/
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_generated/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_generated/
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/_generated/aio/operations/_documents_operations.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_headers_mixin.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/models/
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_api_versions.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_search_client.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/aio/
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_version.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_search_indexer_client.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_queries.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/__init__.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/__init__.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_utils.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_search_documents_error.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_search_index_client.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_search_indexing_buffered_sender.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/models/_edm.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_utils.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/models/__init__.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_index_documents_batch.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/models/_index.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_search_indexing_buffered_sender_base.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/models/_models.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_paging.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/models/
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/py.typed
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/operations/
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/models/
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/aio/
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/_patch.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/_serialization.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_search_index_client.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/__init__.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_search_indexer_client.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/_vendor.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/__init__.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/_search_service_client.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_utils.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/_configuration.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/models/_models.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/models/_patch.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/models/_index.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/models/_search_service_client_enums.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/models/__init__.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/models/_models_py3.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/models/_edm.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/models/__init__.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/aio/_search_index_client.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/operations/_patch.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/aio/_search_indexer_client.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/operations/_synonym_maps_operations.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/aio/__init__.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/operations/_aliases_operations.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/models/
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/operations/_indexes_operations.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/operations/__init__.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/operations/
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/operations/_skillsets_operations.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/_patch.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/operations/_indexers_operations.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/_serialization.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/operations/_search_service_client_operations.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/_configuration.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/operations/_data_sources_operations.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/__init__.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/operations/
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/_search_service_client.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/_patch.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/_vendor.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/__init__.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/models/_search_service_client_enums.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/_vendor.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/models/_patch.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/_search_service_client.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/models/__init__.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/_configuration.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/models/_models_py3.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/operations/
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/operations/_synonym_maps_operations.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/_patch.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/operations/_aliases_operations.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/_configuration.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/operations/_indexes_operations.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/__init__.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/_search_service_client.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/operations/_skillsets_operations.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/_vendor.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/operations/_indexers_operations.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/operations/_synonym_maps_operations.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/operations/_search_service_client_operations.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/operations/_search_service_client_operations.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/operations/_data_sources_operations.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/operations/_indexes_operations.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/aio/_search_indexer_client.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/operations/_patch.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/aio/__init__.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/operations/__init__.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/indexes/aio/_search_index_client.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/operations/_skillsets_operations.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/aio/_index_documents_batch_async.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/operations/_data_sources_operations.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/aio/_paging.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/operations/_aliases_operations.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/aio/_search_indexing_buffered_sender_async.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/operations/_indexers_operations.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/aio/_timer.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/operations/_synonym_maps_operations.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/aio/__init__.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/operations/_search_service_client_operations.py
+Filename: azure-search-documents-11.4.0b7/azure/search/documents/aio/_search_client_async.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/operations/_indexes_operations.py
+Filename: azure-search-documents-11.4.0b7/tests/async_tests/
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/operations/_patch.py
+Filename: azure-search-documents-11.4.0b7/tests/perfstress_tests/
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/operations/__init__.py
+Filename: azure-search-documents-11.4.0b7/tests/test_search_index_client_skillset_live.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/operations/_skillsets_operations.py
+Filename: azure-search-documents-11.4.0b7/tests/test_search_client_index_document_live.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/operations/_data_sources_operations.py
+Filename: azure-search-documents-11.4.0b7/tests/test_search_index_client.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/operations/_aliases_operations.py
+Filename: azure-search-documents-11.4.0b7/tests/test_search_client_search_live.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/operations/_indexers_operations.py
+Filename: azure-search-documents-11.4.0b7/tests/test_regex_flags.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/models/__init__.py
+Filename: azure-search-documents-11.4.0b7/tests/test_index_field_helpers.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/aio/_search_indexing_buffered_sender_async.py
+Filename: azure-search-documents-11.4.0b7/tests/test_search_client.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/aio/_search_client_async.py
+Filename: azure-search-documents-11.4.0b7/tests/test_search_index_client_live.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/aio/__init__.py
+Filename: azure-search-documents-11.4.0b7/tests/test_buffered_sender.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/aio/_timer.py
+Filename: azure-search-documents-11.4.0b7/tests/test_search_index_client_alias_live.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/aio/_index_documents_batch_async.py
+Filename: azure-search-documents-11.4.0b7/tests/test_search_client_basic_live.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/aio/_paging.py
+Filename: azure-search-documents-11.4.0b7/tests/test_index_documents_batch.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_generated/models/
+Filename: azure-search-documents-11.4.0b7/tests/search_service_preparer.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_generated/aio/
+Filename: azure-search-documents-11.4.0b7/tests/test_search_index_client_data_source_live.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_generated/operations/
+Filename: azure-search-documents-11.4.0b7/tests/test_search_index_client_synonym_map_live.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_generated/_search_index_client.py
+Filename: azure-search-documents-11.4.0b7/tests/test_search_indexer_client_live.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_generated/_patch.py
+Filename: azure-search-documents-11.4.0b7/tests/test_queries.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_generated/_serialization.py
+Filename: azure-search-documents-11.4.0b7/tests/test_search_client_buffered_sender_live.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_generated/_configuration.py
+Filename: azure-search-documents-11.4.0b7/tests/conftest.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_generated/__init__.py
+Filename: azure-search-documents-11.4.0b7/tests/async_tests/test_search_index_client_data_source_live_async.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_generated/_vendor.py
+Filename: azure-search-documents-11.4.0b7/tests/async_tests/test_search_indexer_client_live_async.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_generated/models/_patch.py
+Filename: azure-search-documents-11.4.0b7/tests/async_tests/test_search_client_basic_live_async.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_generated/models/_search_index_client_enums.py
+Filename: azure-search-documents-11.4.0b7/tests/async_tests/test_search_client_index_document_live_async.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_generated/models/__init__.py
+Filename: azure-search-documents-11.4.0b7/tests/async_tests/test_search_index_client_alias_live_async.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_generated/models/_models_py3.py
+Filename: azure-search-documents-11.4.0b7/tests/async_tests/test_search_index_client_synonym_map_live_async.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_generated/aio/operations/
+Filename: azure-search-documents-11.4.0b7/tests/async_tests/test_search_client_async.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_generated/aio/_search_index_client.py
+Filename: azure-search-documents-11.4.0b7/tests/async_tests/test_search_index_client_skillset_live_async.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_generated/aio/_patch.py
+Filename: azure-search-documents-11.4.0b7/tests/async_tests/test_search_index_client_live_async.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_generated/aio/_configuration.py
+Filename: azure-search-documents-11.4.0b7/tests/async_tests/test_search_client_buffered_sender_live_async.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_generated/aio/__init__.py
+Filename: azure-search-documents-11.4.0b7/tests/async_tests/test_buffered_sender_async.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_generated/aio/operations/_patch.py
+Filename: azure-search-documents-11.4.0b7/tests/async_tests/test_search_index_client_async.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_generated/aio/operations/_documents_operations.py
+Filename: azure-search-documents-11.4.0b7/tests/async_tests/test_search_client_search_live_async.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_generated/aio/operations/__init__.py
+Filename: azure-search-documents-11.4.0b7/tests/perfstress_tests/suggest.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_generated/operations/_patch.py
+Filename: azure-search-documents-11.4.0b7/tests/perfstress_tests/__init__.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_generated/operations/_documents_operations.py
+Filename: azure-search-documents-11.4.0b7/tests/perfstress_tests/autocomplete.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure/search/documents/_generated/operations/__init__.py
+Filename: azure-search-documents-11.4.0b7/tests/perfstress_tests/search_documents.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/async_samples/
+Filename: azure-search-documents-11.4.0b7/samples/async_samples/
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/sample_data_source_operations.py
+Filename: azure-search-documents-11.4.0b7/samples/README.md
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/sample_authentication.py
+Filename: azure-search-documents-11.4.0b7/samples/sample_synonym_map_operations.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/sample_indexers_operations.py
+Filename: azure-search-documents-11.4.0b7/samples/sample_facet_query.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/sample_synonym_map_operations.py
+Filename: azure-search-documents-11.4.0b7/samples/sample_simple_query.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/sample_buffered_sender.py
+Filename: azure-search-documents-11.4.0b7/samples/sample_suggestions.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/sample_get_document.py
+Filename: azure-search-documents-11.4.0b7/samples/sample_crud_operations.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/sample_analyze_text.py
+Filename: azure-search-documents-11.4.0b7/samples/sample_index_crud_operations.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/README.md
+Filename: azure-search-documents-11.4.0b7/samples/sample_semantic_search.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/sample_semantic_search.py
+Filename: azure-search-documents-11.4.0b7/samples/sample_vector_search.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/sample_index_alias_crud_operations.py
+Filename: azure-search-documents-11.4.0b7/samples/sample_analyze_text.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/sample_filter_query.py
+Filename: azure-search-documents-11.4.0b7/samples/sample_indexer_datasource_skillset.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/sample_index_crud_operations.py
+Filename: azure-search-documents-11.4.0b7/samples/sample_indexers_operations.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/sample_autocomplete.py
+Filename: azure-search-documents-11.4.0b7/samples/sample_get_document.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/sample_indexer_datasource_skillset.py
+Filename: azure-search-documents-11.4.0b7/samples/sample_data_source_operations.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/sample_simple_query.py
+Filename: azure-search-documents-11.4.0b7/samples/sample_buffered_sender.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/sample_facet_query.py
+Filename: azure-search-documents-11.4.0b7/samples/sample_filter_query.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/sample_vector_search.py
+Filename: azure-search-documents-11.4.0b7/samples/sample_autocomplete.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/sample_suggestions.py
+Filename: azure-search-documents-11.4.0b7/samples/sample_index_alias_crud_operations.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/sample_crud_operations.py
+Filename: azure-search-documents-11.4.0b7/samples/sample_authentication.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/async_samples/sample_semantic_search_async.py
+Filename: azure-search-documents-11.4.0b7/samples/async_samples/sample_index_alias_crud_operations_async.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/async_samples/sample_crud_operations_async.py
+Filename: azure-search-documents-11.4.0b7/samples/async_samples/sample_authentication_async.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/async_samples/sample_indexers_operations_async.py
+Filename: azure-search-documents-11.4.0b7/samples/async_samples/sample_crud_operations_async.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/async_samples/sample_facet_query_async.py
+Filename: azure-search-documents-11.4.0b7/samples/async_samples/sample_synonym_map_operations_async.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/async_samples/sample_analyze_text_async.py
+Filename: azure-search-documents-11.4.0b7/samples/async_samples/sample_simple_query_async.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/async_samples/sample_index_alias_crud_operations_async.py
+Filename: azure-search-documents-11.4.0b7/samples/async_samples/sample_suggestions_async.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/async_samples/sample_suggestions_async.py
+Filename: azure-search-documents-11.4.0b7/samples/async_samples/sample_facet_query_async.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/async_samples/sample_simple_query_async.py
+Filename: azure-search-documents-11.4.0b7/samples/async_samples/sample_index_crud_operations_async.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/async_samples/sample_buffered_sender_async.py
+Filename: azure-search-documents-11.4.0b7/samples/async_samples/sample_buffered_sender_async.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/async_samples/sample_authentication_async.py
+Filename: azure-search-documents-11.4.0b7/samples/async_samples/sample_filter_query_async.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/async_samples/sample_index_crud_operations_async.py
+Filename: azure-search-documents-11.4.0b7/samples/async_samples/sample_autocomplete_async.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/async_samples/sample_synonym_map_operations_async.py
+Filename: azure-search-documents-11.4.0b7/samples/async_samples/sample_data_source_operations_async.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/async_samples/sample_vector_search_async.py
+Filename: azure-search-documents-11.4.0b7/samples/async_samples/sample_semantic_search_async.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/async_samples/sample_filter_query_async.py
+Filename: azure-search-documents-11.4.0b7/samples/async_samples/sample_vector_search_async.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/async_samples/sample_data_source_operations_async.py
+Filename: azure-search-documents-11.4.0b7/samples/async_samples/sample_indexers_operations_async.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/async_samples/sample_autocomplete_async.py
+Filename: azure-search-documents-11.4.0b7/samples/async_samples/sample_get_document_async.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/samples/async_samples/sample_get_document_async.py
+Filename: azure-search-documents-11.4.0b7/samples/async_samples/sample_analyze_text_async.py
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure_search_documents.egg-info/PKG-INFO
+Filename: azure-search-documents-11.4.0b7/azure_search_documents.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure_search_documents.egg-info/requires.txt
+Filename: azure-search-documents-11.4.0b7/azure_search_documents.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure_search_documents.egg-info/SOURCES.txt
+Filename: azure-search-documents-11.4.0b7/azure_search_documents.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure_search_documents.egg-info/not-zip-safe
+Filename: azure-search-documents-11.4.0b7/azure_search_documents.egg-info/requires.txt
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure_search_documents.egg-info/top_level.txt
+Filename: azure-search-documents-11.4.0b7/azure_search_documents.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-search-documents-11.4.0b6/azure_search_documents.egg-info/dependency_links.txt
+Filename: azure-search-documents-11.4.0b7/azure_search_documents.egg-info/PKG-INFO
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-search-documents-11.4.0b6/PKG-INFO` & `azure-search-documents-11.4.0b7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-search-documents
-Version: 11.4.0b6
+Version: 11.4.0b7
 Summary: Microsoft Azure Cognitive Search Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/search/azure-search-documents
 Author: Microsoft Corporation
 Author-email: ascl@microsoft.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -261,14 +261,15 @@
 You can use the `SearchIndexClient` to create a search index. Fields can be
 defined using convenient `SimpleField`, `SearchableField`, or `ComplexField`
 models. Indexes can also define suggesters, lexical analyzers, and more.
 
 <!-- SNIPPET:sample_index_crud_operations.create_index -->
 
 ```python
+client = SearchIndexClient(service_endpoint, AzureKeyCredential(key))
 name = "hotels"
 fields = [
     SimpleField(name="hotelId", type=SearchFieldDataType.String, key=True),
     SimpleField(name="baseRate", type=SearchFieldDataType.Double),
     SearchableField(name="description", type=SearchFieldDataType.String, collection=True),
     ComplexField(
         name="address",
@@ -295,19 +296,19 @@
 [a few special rules for merging](https://docs.microsoft.com/rest/api/searchservice/addupdate-or-delete-documents#document-actions)
 to be aware of.
 
 <!-- SNIPPET:sample_crud_operations.upload_document -->
 
 ```python
 DOCUMENT = {
-    "Category": "Hotel",
-    "HotelId": "1000",
-    "Rating": 4.0,
-    "Rooms": [],
-    "HotelName": "Azure Inn",
+    "category": "Hotel",
+    "hotelId": "1000",
+    "rating": 4.0,
+    "rooms": [],
+    "hotelName": "Azure Inn",
 }
 
 result = search_client.upload_documents(documents=[DOCUMENT])
 
 print("Upload of new document succeeded: {}".format(result[0].succeeded))
 ```
 
@@ -348,17 +349,17 @@
 from azure.search.documents import SearchClient
 
 search_client = SearchClient(service_endpoint, index_name, AzureKeyCredential(key))
 
 result = search_client.get_document(key="23")
 
 print("Details for hotel '23' are:")
-print("        Name: {}".format(result["HotelName"]))
-print("      Rating: {}".format(result["Rating"]))
-print("    Category: {}".format(result["Category"]))
+print("        Name: {}".format(result["hotelName"]))
+print("      Rating: {}".format(result["rating"]))
+print("    Category: {}".format(result["category"]))
 ```
 
 <!-- END SNIPPET -->
 
 ### Async APIs
 
 This library includes a complete async API. To use it, you must
@@ -376,15 +377,15 @@
 search_client = SearchClient(service_endpoint, index_name, AzureKeyCredential(key))
 
 async with search_client:
     results = await search_client.search(search_text="spa")
 
     print("Hotels containing 'spa' in the name (or other fields):")
     async for result in results:
-        print("    Name: {} (rating {})".format(result["HotelName"], result["Rating"]))
+        print("    Name: {} (rating {})".format(result["hotelName"], result["rating"]))
 ```
 
 <!-- END SNIPPET -->
 
 ## Troubleshooting
 
 ### General
```

## Comparing `azure-search-documents-11.4.0b6/CHANGELOG.md` & `azure-search-documents-11.4.0b7/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 # Release History
 
+## 11.4.0b7 (2023-08-08)
+
+### Features Added
+
+- Added multi-vector search support. Now instead of passing in `vector`, `top_k` and `vector_fields`, search method accepts `vectors` which is a list of `Vector` object.
+
+### Breaking Changes
+
+> These changes do not impact the API of stable versions such as 11.3.0.
+> Only code written against a beta version such as 11.4.0b6 may be affected.
+- Stopped supporting `vector`, `top_k` and `vector_fields` in `SearchClient.search` method.
+
 ## 11.4.0b6 (2023-07-11)
 
 ### Features Added
 
 - Added `top_k` support for `VectorSearch`.
 
 ## 11.4.0b5 (2023-07-11)
```

## Comparing `azure-search-documents-11.4.0b6/README.md` & `azure-search-documents-11.4.0b7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -239,14 +239,15 @@
 You can use the `SearchIndexClient` to create a search index. Fields can be
 defined using convenient `SimpleField`, `SearchableField`, or `ComplexField`
 models. Indexes can also define suggesters, lexical analyzers, and more.
 
 <!-- SNIPPET:sample_index_crud_operations.create_index -->
 
 ```python
+client = SearchIndexClient(service_endpoint, AzureKeyCredential(key))
 name = "hotels"
 fields = [
     SimpleField(name="hotelId", type=SearchFieldDataType.String, key=True),
     SimpleField(name="baseRate", type=SearchFieldDataType.Double),
     SearchableField(name="description", type=SearchFieldDataType.String, collection=True),
     ComplexField(
         name="address",
@@ -273,19 +274,19 @@
 [a few special rules for merging](https://docs.microsoft.com/rest/api/searchservice/addupdate-or-delete-documents#document-actions)
 to be aware of.
 
 <!-- SNIPPET:sample_crud_operations.upload_document -->
 
 ```python
 DOCUMENT = {
-    "Category": "Hotel",
-    "HotelId": "1000",
-    "Rating": 4.0,
-    "Rooms": [],
-    "HotelName": "Azure Inn",
+    "category": "Hotel",
+    "hotelId": "1000",
+    "rating": 4.0,
+    "rooms": [],
+    "hotelName": "Azure Inn",
 }
 
 result = search_client.upload_documents(documents=[DOCUMENT])
 
 print("Upload of new document succeeded: {}".format(result[0].succeeded))
 ```
 
@@ -326,17 +327,17 @@
 from azure.search.documents import SearchClient
 
 search_client = SearchClient(service_endpoint, index_name, AzureKeyCredential(key))
 
 result = search_client.get_document(key="23")
 
 print("Details for hotel '23' are:")
-print("        Name: {}".format(result["HotelName"]))
-print("      Rating: {}".format(result["Rating"]))
-print("    Category: {}".format(result["Category"]))
+print("        Name: {}".format(result["hotelName"]))
+print("      Rating: {}".format(result["rating"]))
+print("    Category: {}".format(result["category"]))
 ```
 
 <!-- END SNIPPET -->
 
 ### Async APIs
 
 This library includes a complete async API. To use it, you must
@@ -354,15 +355,15 @@
 search_client = SearchClient(service_endpoint, index_name, AzureKeyCredential(key))
 
 async with search_client:
     results = await search_client.search(search_text="spa")
 
     print("Hotels containing 'spa' in the name (or other fields):")
     async for result in results:
-        print("    Name: {} (rating {})".format(result["HotelName"], result["Rating"]))
+        print("    Name: {} (rating {})".format(result["hotelName"], result["rating"]))
 ```
 
 <!-- END SNIPPET -->
 
 ## Troubleshooting
 
 ### General
```

## Comparing `azure-search-documents-11.4.0b6/TROUBLESHOOTING.md` & `azure-search-documents-11.4.0b7/TROUBLESHOOTING.md`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/LICENSE` & `azure-search-documents-11.4.0b7/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/setup.py` & `azure-search-documents-11.4.0b7/setup.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/tests/test_search_index_client_data_source_live.py` & `azure-search-documents-11.4.0b7/tests/test_search_index_client_data_source_live.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         return data_source_connection
 
     @SearchEnvVarPreparer()
     @search_decorator(schema="hotel_schema.json", index_batch="hotel_small.json")
     @recorded_by_proxy
     def test_data_source(self, endpoint, api_key, **kwargs):
         storage_cs = kwargs.get("search_storage_connection_string")
-        client = SearchIndexerClient(endpoint, api_key)
+        client = SearchIndexerClient(endpoint, api_key, retry_backoff_factor=60)
         self._test_create_datasource(client, storage_cs)
         self._test_delete_datasource(client, storage_cs)
         self._test_get_datasource(client, storage_cs)
         self._test_list_datasources(client, storage_cs)
         self._test_create_or_update_datasource(client, storage_cs)
         self._test_create_or_update_datasource_if_unchanged(client, storage_cs)
         self._test_delete_datasource_if_unchanged(client, storage_cs)
```

## Comparing `azure-search-documents-11.4.0b6/tests/test_search_client_search_live.py` & `azure-search-documents-11.4.0b7/tests/test_search_client_search_live.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 class TestSearchClient(AzureRecordedTestCase):
     @SearchEnvVarPreparer()
     @search_decorator(schema="hotel_schema.json", index_batch="hotel_small.json")
     @recorded_by_proxy
     def test_search_client(self, endpoint, api_key, index_name):
-        client = SearchClient(endpoint, index_name, api_key)
+        client = SearchClient(endpoint, index_name, api_key, retry_backoff_factor=60)
         self._test_get_search_simple(client)
         self._test_get_search_simple_with_top(client)
         self._test_get_search_filter(client)
         self._test_get_search_filter_array(client)
         self._test_get_search_counts(client)
         self._test_get_search_coverage(client)
         self._test_get_search_facets_none(client)
```

## Comparing `azure-search-documents-11.4.0b6/tests/test_search_index_client_synonym_map_live.py` & `azure-search-documents-11.4.0b7/tests/test_search_index_client_synonym_map_live.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 class TestSearchClientSynonymMaps(AzureRecordedTestCase):
     @SearchEnvVarPreparer()
     @search_decorator(schema="hotel_schema.json", index_batch="hotel_small.json")
     @recorded_by_proxy
     def test_synonym_map(self, endpoint, api_key):
-        client = SearchIndexClient(endpoint, api_key)
+        client = SearchIndexClient(endpoint, api_key, retry_backoff_factor=60)
         self._test_create_synonym_map(client)
         self._test_delete_synonym_map(client)
         self._test_delete_synonym_map_if_unchanged(client)
         self._test_get_synonym_map(client)
         self._test_get_synonym_maps(client)
         self._test_create_or_update_synonym_map(client)
```

## Comparing `azure-search-documents-11.4.0b6/tests/test_regex_flags.py` & `azure-search-documents-11.4.0b7/tests/test_regex_flags.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/tests/test_buffered_sender.py` & `azure-search-documents-11.4.0b7/tests/test_buffered_sender.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,25 +54,25 @@
         with SearchIndexingBufferedSender("endpoint", "index name", CREDENTIAL, auto_flush=False) as client:
             client.upload_documents(["upload1"])
             client.delete_documents(["delete1", "delete2"])
         assert mock_cleanup.called
 
     def test_flush(self):
         DOCUMENT = {
-            "Category": "Hotel",
-            "HotelId": "1000",
-            "Rating": 4.0,
-            "Rooms": [],
-            "HotelName": "Azure Inn",
+            "category": "Hotel",
+            "hotelId": "1000",
+            "rating": 4.0,
+            "rooms": [],
+            "hotelName": "Azure Inn",
         }
         with mock.patch.object(
             SearchIndexingBufferedSender, "_index_documents_actions", side_effect=HttpResponseError("Error")
         ):
             with SearchIndexingBufferedSender("endpoint", "index name", CREDENTIAL, auto_flush=False) as client:
-                client._index_key = "HotelId"
+                client._index_key = "hotelId"
                 client.upload_documents([DOCUMENT])
                 client.flush()
                 assert len(client.actions) == 0
 
     def test_callback_new(self):
         on_new = mock.Mock()
         with SearchIndexingBufferedSender(
```

## Comparing `azure-search-documents-11.4.0b6/tests/test_search_index_client_live.py` & `azure-search-documents-11.4.0b7/tests/test_search_index_client_live.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 class TestSearchIndexClient(AzureRecordedTestCase):
     @SearchEnvVarPreparer()
     @search_decorator(schema=None, index_batch=None)
     @recorded_by_proxy
     def test_search_index_client(self, api_key, endpoint, index_name):
-        client = SearchIndexClient(endpoint, api_key)
+        client = SearchIndexClient(endpoint, api_key, retry_backoff_factor=60)
         index_name = "hotels"
         self._test_get_service_statistics(client)
         self._test_list_indexes_empty(client)
         self._test_create_index(client, index_name)
         self._test_list_indexes(client, index_name)
         self._test_get_index(client, index_name)
         self._test_get_index_statistics(client, index_name)
@@ -59,15 +59,18 @@
 
     def _test_get_index(self, client, index_name):
         result = client.get_index(index_name)
         assert result.name == index_name
 
     def _test_get_index_statistics(self, client, index_name):
         result = client.get_index_statistics(index_name)
-        assert set(result.keys()) == {"document_count", "storage_size"}
+        keys = set(result.keys())
+        assert "document_count" in keys
+        assert "storage_size" in keys
+        assert "vector_index_size" in keys
 
     def _test_create_index(self, client, index_name):
         fields = [
             SimpleField(name="hotelId", type=SearchFieldDataType.String, key=True),
             SimpleField(name="baseRate", type=SearchFieldDataType.Double),
         ]
         scoring_profile = ScoringProfile(name="MyProfile")
```

## Comparing `azure-search-documents-11.4.0b6/tests/test_index_documents_batch.py` & `azure-search-documents-11.4.0b7/tests/test_index_documents_batch.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/tests/test_search_index_client_skillset_live.py` & `azure-search-documents-11.4.0b7/tests/test_search_index_client_skillset_live.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 class TestSearchSkillset(AzureRecordedTestCase):
     @pytest.mark.skip("The skills are deprecated")
     @SearchEnvVarPreparer()
     @search_decorator(schema="hotel_schema.json", index_batch="hotel_small.json")
     @recorded_by_proxy
     def test_skillset_crud(self, api_key, endpoint):
-        client = SearchIndexerClient(endpoint, api_key)
+        client = SearchIndexerClient(endpoint, api_key, retry_backoff_factor=60)
         self._test_create_skillset_validation()
         self._test_create_skillset(client)
         self._test_get_skillset(client)
         self._test_get_skillsets(client)
         self._test_create_or_update_skillset(client)
         self._test_create_or_update_skillset_if_unchanged(client)
         self._test_create_or_update_skillset_inplace(client)
```

## Comparing `azure-search-documents-11.4.0b6/tests/test_index_field_helpers.py` & `azure-search-documents-11.4.0b7/tests/test_index_field_helpers.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/tests/test_queries.py` & `azure-search-documents-11.4.0b7/tests/test_queries.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/tests/conftest.py` & `azure-search-documents-11.4.0b7/tests/conftest.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/tests/search_service_preparer.py` & `azure-search-documents-11.4.0b7/tests/search_service_preparer.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import requests
 import wrapt
 
 from devtools_testutils import EnvironmentVariableLoader
 from azure_devtools.scenario_tests.exceptions import AzureTestError
 
 from azure.core.credentials import AzureKeyCredential
-from azure.core.exceptions import ResourceNotFoundError
+from azure.core.exceptions import HttpResponseError
 
 SERVICE_URL_FMT = "https://{}.{}/indexes?api-version=2021-04-30-Preview"
 TIME_TO_SLEEP = 3
 SEARCH_ENDPOINT_SUFFIX = environ.get("SEARCH_ENDPOINT_SUFFIX", "search.windows.net")
 
 SearchEnvVarPreparer = functools.partial(
     EnvironmentVariableLoader,
@@ -73,16 +73,22 @@
     from azure.search.documents.indexes import SearchIndexerClient
 
     client = SearchIndexerClient(endpoint, AzureKeyCredential(api_key), retry_backoff_factor=60)
     for indexer in client.get_indexers():
         client.delete_indexer(indexer)
     for datasource in client.get_data_source_connection_names():
         client.delete_data_source_connection(datasource)
-    for skillset in client.get_skillset_names():
-        client.delete_skillset(skillset)
+    try:
+        for skillset in client.get_skillset_names():
+            client.delete_skillset(skillset)
+    except HttpResponseError as ex:
+        if "skillset related operations are not enabled in this region" in ex.message.lower():
+            pass
+        else:
+            raise
 
 
 def _set_up_index(service_name, endpoint, api_key, schema, index_batch):
     from azure.core.credentials import AzureKeyCredential
     from azure.search.documents import SearchClient
     from azure.search.documents._generated.models import IndexBatch
```

## Comparing `azure-search-documents-11.4.0b6/tests/test_search_client.py` & `azure-search-documents-11.4.0b7/tests/test_search_client.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/tests/test_search_indexer_client_live.py` & `azure-search-documents-11.4.0b7/tests/test_search_indexer_client_live.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 class TestSearchIndexerClientTest(AzureRecordedTestCase):
     @SearchEnvVarPreparer()
     @search_decorator(schema="hotel_schema.json", index_batch="hotel_small.json")
     @recorded_by_proxy
     def test_search_indexers(self, endpoint, api_key, **kwargs):
         storage_cs = kwargs.get("search_storage_connection_string")
         container_name = kwargs.get("search_storage_container_name")
-        client = SearchIndexerClient(endpoint, api_key)
-        index_client = SearchIndexClient(endpoint, api_key)
+        client = SearchIndexerClient(endpoint, api_key, retry_backoff_factor=60)
+        index_client = SearchIndexClient(endpoint, api_key, retry_backoff_factor=60)
         self._test_create_indexer(client, index_client, storage_cs, container_name)
         self._test_delete_indexer(client, index_client, storage_cs, container_name)
         self._test_get_indexer(client, index_client, storage_cs, container_name)
         self._test_list_indexer(client, index_client, storage_cs, container_name)
         self._test_create_or_update_indexer(client, index_client, storage_cs, container_name)
         self._test_reset_indexer(client, index_client, storage_cs, container_name)
         self._test_run_indexer(client, index_client, storage_cs, container_name)
```

## Comparing `azure-search-documents-11.4.0b6/tests/test_search_client_buffered_sender_live.py` & `azure-search-documents-11.4.0b7/tests/test_search_client_buffered_sender_live.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 
 class TestSearchIndexingBufferedSender(AzureRecordedTestCase):
     @SearchEnvVarPreparer()
     @search_decorator(schema="hotel_schema.json", index_batch="hotel_small.json")
     @recorded_by_proxy
     def test_search_client_index_buffered_sender(self, endpoint, api_key, index_name):
-        client = SearchClient(endpoint, index_name, api_key)
-        batch_client = SearchIndexingBufferedSender(endpoint, index_name, api_key)
+        client = SearchClient(endpoint, index_name, api_key, retry_backoff_factor=60)
+        batch_client = SearchIndexingBufferedSender(endpoint, index_name, api_key, retry_backoff_factor=60)
         try:
             doc_count = 10
             doc_count = self._test_upload_documents_new(client, batch_client, doc_count)
             doc_count = self._test_upload_documents_existing(client, batch_client, doc_count)
             doc_count = self._test_delete_documents_existing(client, batch_client, doc_count)
             doc_count = self._test_delete_documents_missing(client, batch_client, doc_count)
             doc_count = self._test_merge_documents_existing(client, batch_client, doc_count)
```

## Comparing `azure-search-documents-11.4.0b6/tests/test_search_client_index_document_live.py` & `azure-search-documents-11.4.0b7/tests/test_search_client_index_document_live.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 class TestSearchClientIndexDocument(AzureRecordedTestCase):
     @SearchEnvVarPreparer()
     @search_decorator(schema="hotel_schema.json", index_batch="hotel_small.json")
     @recorded_by_proxy
     def test_search_client_index_document(self, endpoint, api_key, index_name):
-        client = SearchClient(endpoint, index_name, api_key)
+        client = SearchClient(endpoint, index_name, api_key, retry_backoff_factor=60)
         doc_count = 10
         doc_count = self._test_upload_documents_new(client, doc_count)
         doc_count = self._test_upload_documents_existing(client, doc_count)
         doc_count = self._test_delete_documents_existing(client, doc_count)
         doc_count = self._test_delete_documents_missing(client, doc_count)
         doc_count = self._test_merge_documents_existing(client, doc_count)
         doc_count = self._test_merge_documents_missing(client, doc_count)
```

## Comparing `azure-search-documents-11.4.0b6/tests/test_search_index_client_alias_live.py` & `azure-search-documents-11.4.0b7/tests/test_search_index_client_alias_live.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 
 class TestSearchClientAlias(AzureRecordedTestCase):
     @SearchEnvVarPreparer()
     @search_decorator(schema="hotel_schema.json", index_batch="hotel_small.json")
     @recorded_by_proxy
     def test_alias(self, endpoint, api_key):
-        client = SearchIndexClient(endpoint, api_key)
+        client = SearchIndexClient(endpoint, api_key, retry_backoff_factor=60)
         aliases = ["resort", "motel"]
         index_name = next(client.list_index_names())
         self._test_list_aliases_empty(client)
         self._test_create_alias(client, aliases[0], index_name)
 
         self._test_create_or_update_alias(client, aliases[1], index_name)
```

## Comparing `azure-search-documents-11.4.0b6/tests/test_search_index_client.py` & `azure-search-documents-11.4.0b7/tests/test_search_index_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         assert client._headers == {
             "api-key": "test_api_key",
             "Accept": "application/json;odata.metadata=minimal",
         }
 
     def test_index_credential_roll(self):
         credential = AzureKeyCredential(key="old_api_key")
-        client = SearchIndexClient("endpoint", credential)
+        client = SearchIndexClient("endpoint", credential, retry_backoff_factor=60)
         assert client._headers == {
             "api-key": "old_api_key",
             "Accept": "application/json;odata.metadata=minimal",
         }
         credential.update("new_api_key")
         assert client._headers == {
             "api-key": "new_api_key",
```

## Comparing `azure-search-documents-11.4.0b6/tests/test_search_client_basic_live.py` & `azure-search-documents-11.4.0b7/tests/async_tests/test_search_client_basic_live_async.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
 import pytest
-
 from azure.core.exceptions import HttpResponseError
-from azure.search.documents import SearchClient
-from devtools_testutils import AzureRecordedTestCase, recorded_by_proxy
+from azure.search.documents.aio import SearchClient
+from devtools_testutils.aio import recorded_by_proxy_async
+from devtools_testutils import AzureRecordedTestCase
 
 from search_service_preparer import SearchEnvVarPreparer, search_decorator
 
 
-class TestSearchClient(AzureRecordedTestCase):
+class TestSearchClientAsync(AzureRecordedTestCase):
     @SearchEnvVarPreparer()
     @search_decorator(schema="hotel_schema.json", index_batch="hotel_small.json")
-    @recorded_by_proxy
-    def test_get_document_count(self, endpoint, api_key, index_name):
+    @recorded_by_proxy_async
+    async def test_get_document_count(self, endpoint, api_key, index_name):
         client = SearchClient(endpoint, index_name, api_key)
-        assert client.get_document_count() == 10
+        async with client:
+            assert await client.get_document_count() == 10
 
     @SearchEnvVarPreparer()
     @search_decorator(schema="hotel_schema.json", index_batch="hotel_small.json")
-    @recorded_by_proxy
-    def test_get_document(self, endpoint, api_key, index_name, index_batch):
+    @recorded_by_proxy_async
+    async def test_get_document(self, endpoint, api_key, index_name, index_batch):
         client = SearchClient(endpoint, index_name, api_key)
-        for hotel_id in range(1, 11):
-            result = client.get_document(key=str(hotel_id))
-            expected = index_batch["value"][hotel_id - 1]
-            assert result.get("hotelId") == expected.get("hotelId")
-            assert result.get("hotelName") == expected.get("hotelName")
-            assert result.get("description") == expected.get("description")
+        async with client:
+            for hotel_id in range(1, 11):
+                result = await client.get_document(key=str(hotel_id))
+                expected = index_batch["value"][hotel_id - 1]
+                assert result.get("hotelId") == expected.get("hotelId")
+                assert result.get("hotelName") == expected.get("hotelName")
+                assert result.get("description") == expected.get("description")
 
     @SearchEnvVarPreparer()
     @search_decorator(schema="hotel_schema.json", index_batch="hotel_small.json")
-    @recorded_by_proxy
-    def test_get_document_missing(self, endpoint, api_key, index_name):
+    @recorded_by_proxy_async
+    async def test_get_document_missing(self, endpoint, api_key, index_name):
         client = SearchClient(endpoint, index_name, api_key)
-        with pytest.raises(HttpResponseError):
-            client.get_document(key="1000")
+        async with client:
+            with pytest.raises(HttpResponseError):
+                await client.get_document(key="1000")
```

## Comparing `azure-search-documents-11.4.0b6/tests/async_tests/test_search_client_index_document_live_async.py` & `azure-search-documents-11.4.0b7/tests/async_tests/test_search_client_index_document_live_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 class TestSearchClientDocumentsAsync(AzureRecordedTestCase):
     @SearchEnvVarPreparer()
     @search_decorator(schema="hotel_schema.json", index_batch="hotel_small.json")
     @recorded_by_proxy_async
     async def test_search_client_index_document(self, endpoint, api_key, index_name):
-        client = SearchClient(endpoint, index_name, api_key)
+        client = SearchClient(endpoint, index_name, api_key, retry_backoff_factor=60)
         doc_count = 10
         async with client:
             doc_count = await self._test_upload_documents_new(client, doc_count)
             doc_count = await self._test_upload_documents_existing(client, doc_count)
             doc_count = await self._test_delete_documents_existing(client, doc_count)
             doc_count = await self._test_delete_documents_missing(client, doc_count)
             doc_count = await self._test_merge_documents_existing(client, doc_count)
```

## Comparing `azure-search-documents-11.4.0b6/tests/async_tests/test_search_index_client_synonym_map_live_async.py` & `azure-search-documents-11.4.0b7/tests/async_tests/test_search_index_client_synonym_map_live_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 class TestSearchClientSynonymMaps(AzureRecordedTestCase):
     @SearchEnvVarPreparer()
     @search_decorator(schema="hotel_schema.json", index_batch="hotel_small.json")
     @recorded_by_proxy_async
     async def test_synonym_map(self, endpoint, api_key):
-        client = SearchIndexClient(endpoint, api_key)
+        client = SearchIndexClient(endpoint, api_key, retry_backoff_factor=60)
         async with client:
             await self._test_create_synonym_map(client)
             await self._test_delete_synonym_map(client)
             await self._test_delete_synonym_map_if_unchanged(client)
             await self._test_get_synonym_map(client)
             await self._test_get_synonym_maps(client)
             await self._test_create_or_update_synonym_map(client)
```

## Comparing `azure-search-documents-11.4.0b6/tests/async_tests/test_search_index_client_alias_live_async.py` & `azure-search-documents-11.4.0b7/tests/async_tests/test_search_index_client_alias_live_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 
 class TestSearchClientAlias(AzureRecordedTestCase):
     @SearchEnvVarPreparer()
     @search_decorator(schema="hotel_schema.json", index_batch="hotel_small.json")
     @recorded_by_proxy_async
     async def test_alias(self, endpoint, api_key):
-        client = SearchIndexClient(endpoint, api_key)
+        client = SearchIndexClient(endpoint, api_key, retry_backoff_factor=60)
         aliases = ["resort", "motel"]
 
         async with client:
             index_name = await client.list_index_names().__anext__()
             await self._test_list_aliases_empty(client)
             await self._test_create_alias(client, aliases[0], index_name)
```

## Comparing `azure-search-documents-11.4.0b6/tests/async_tests/test_search_index_client_data_source_live_async.py` & `azure-search-documents-11.4.0b7/tests/async_tests/test_search_index_client_data_source_live_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         return data_source_connection
 
     @SearchEnvVarPreparer()
     @search_decorator(schema="hotel_schema.json", index_batch="hotel_small.json")
     @recorded_by_proxy_async
     async def test_data_source(self, endpoint, api_key, **kwargs):
         storage_cs = kwargs.get("search_storage_connection_string")
-        client = SearchIndexerClient(endpoint, api_key)
+        client = SearchIndexerClient(endpoint, api_key, retry_backoff_factor=60)
         async with client:
             await self._test_create_datasource(client, storage_cs)
             await self._test_delete_datasource(client, storage_cs)
             await self._test_get_datasource(client, storage_cs)
             await self._test_list_datasources(client, storage_cs)
             await self._test_create_or_update_datasource(client, storage_cs)
             await self._test_create_or_update_datasource_if_unchanged(client, storage_cs)
```

## Comparing `azure-search-documents-11.4.0b6/tests/async_tests/test_search_client_async.py` & `azure-search-documents-11.4.0b7/tests/async_tests/test_search_client_async.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/tests/async_tests/test_search_client_basic_live_async.py` & `azure-search-documents-11.4.0b7/tests/test_search_client_basic_live.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,42 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
 import pytest
+
 from azure.core.exceptions import HttpResponseError
-from azure.search.documents.aio import SearchClient
-from devtools_testutils.aio import recorded_by_proxy_async
-from devtools_testutils import AzureRecordedTestCase
+from azure.search.documents import SearchClient
+from devtools_testutils import AzureRecordedTestCase, recorded_by_proxy
 
 from search_service_preparer import SearchEnvVarPreparer, search_decorator
 
 
-class TestSearchClientAsync(AzureRecordedTestCase):
+class TestSearchClient(AzureRecordedTestCase):
     @SearchEnvVarPreparer()
     @search_decorator(schema="hotel_schema.json", index_batch="hotel_small.json")
-    @recorded_by_proxy_async
-    async def test_get_document_count(self, endpoint, api_key, index_name):
-        client = SearchClient(endpoint, index_name, api_key)
-        async with client:
-            assert await client.get_document_count() == 10
+    @recorded_by_proxy
+    def test_get_document_count(self, endpoint, api_key, index_name):
+        client = SearchClient(endpoint, index_name, api_key, retry_backoff_factor=60)
+        assert client.get_document_count() == 10
 
     @SearchEnvVarPreparer()
     @search_decorator(schema="hotel_schema.json", index_batch="hotel_small.json")
-    @recorded_by_proxy_async
-    async def test_get_document(self, endpoint, api_key, index_name, index_batch):
-        client = SearchClient(endpoint, index_name, api_key)
-        async with client:
-            for hotel_id in range(1, 11):
-                result = await client.get_document(key=str(hotel_id))
-                expected = index_batch["value"][hotel_id - 1]
-                assert result.get("hotelId") == expected.get("hotelId")
-                assert result.get("hotelName") == expected.get("hotelName")
-                assert result.get("description") == expected.get("description")
+    @recorded_by_proxy
+    def test_get_document(self, endpoint, api_key, index_name, index_batch):
+        client = SearchClient(endpoint, index_name, api_key, retry_backoff_factor=60)
+        for hotel_id in range(1, 11):
+            result = client.get_document(key=str(hotel_id))
+            expected = index_batch["value"][hotel_id - 1]
+            assert result.get("hotelId") == expected.get("hotelId")
+            assert result.get("hotelName") == expected.get("hotelName")
+            assert result.get("description") == expected.get("description")
 
     @SearchEnvVarPreparer()
     @search_decorator(schema="hotel_schema.json", index_batch="hotel_small.json")
-    @recorded_by_proxy_async
-    async def test_get_document_missing(self, endpoint, api_key, index_name):
-        client = SearchClient(endpoint, index_name, api_key)
-        async with client:
-            with pytest.raises(HttpResponseError):
-                await client.get_document(key="1000")
+    @recorded_by_proxy
+    def test_get_document_missing(self, endpoint, api_key, index_name):
+        client = SearchClient(endpoint, index_name, api_key, retry_backoff_factor=60)
+        with pytest.raises(HttpResponseError):
+            client.get_document(key="1000")
```

## Comparing `azure-search-documents-11.4.0b6/tests/async_tests/test_search_client_buffered_sender_live_async.py` & `azure-search-documents-11.4.0b7/tests/async_tests/test_search_client_buffered_sender_live_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 
 class TestSearchIndexingBufferedSenderAsync(AzureRecordedTestCase):
     @SearchEnvVarPreparer()
     @search_decorator(schema="hotel_schema.json", index_batch="hotel_small.json")
     @recorded_by_proxy_async
     async def test_search_client_index_buffered_sender(self, endpoint, api_key, index_name):
-        client = SearchClient(endpoint, index_name, api_key)
-        batch_client = SearchIndexingBufferedSender(endpoint, index_name, api_key)
+        client = SearchClient(endpoint, index_name, api_key, retry_backoff_factor=60)
+        batch_client = SearchIndexingBufferedSender(endpoint, index_name, api_key, retry_backoff_factor=60)
         try:
             async with client:
                 async with batch_client:
                     doc_count = 10
                     doc_count = await self._test_upload_documents_new(client, batch_client, doc_count)
                     doc_count = await self._test_upload_documents_existing(client, batch_client, doc_count)
                     doc_count = await self._test_delete_documents_existing(client, batch_client, doc_count)
```

## Comparing `azure-search-documents-11.4.0b6/tests/async_tests/test_search_index_client_skillset_live_async.py` & `azure-search-documents-11.4.0b7/tests/async_tests/test_search_index_client_skillset_live_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 class TestSearchClientSkillsets(AzureRecordedTestCase):
     @pytest.mark.skip("The skills are deprecated")
     @SearchEnvVarPreparer()
     @search_decorator(schema="hotel_schema.json", index_batch="hotel_small.json")
     @recorded_by_proxy_async
     async def test_skillset_crud(self, api_key, endpoint):
-        client = SearchIndexerClient(endpoint, api_key)
+        client = SearchIndexerClient(endpoint, api_key, retry_backoff_factor=60)
         async with client:
             await self._test_create_skillset(client)
             await self._test_get_skillset(client)
             await self._test_get_skillsets(client)
             await self._test_create_or_update_skillset(client)
             await self._test_create_or_update_skillset_if_unchanged(client)
             await self._test_create_or_update_skillset_inplace(client)
```

## Comparing `azure-search-documents-11.4.0b6/tests/async_tests/test_search_index_client_live_async.py` & `azure-search-documents-11.4.0b7/tests/async_tests/test_search_index_client_live_async.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 class TestSearchIndexClientAsync(AzureRecordedTestCase):
     @SearchEnvVarPreparer()
     @search_decorator(schema=None, index_batch=None)
     @recorded_by_proxy_async
     async def test_search_index_client(self, api_key, endpoint, index_name):
-        client = SearchIndexClient(endpoint, api_key)
+        client = SearchIndexClient(endpoint, api_key, retry_backoff_factor=60)
         index_name = "hotels"
         async with client:
             await self._test_get_service_statistics(client)
             await self._test_list_indexes_empty(client)
             await self._test_create_index(client, index_name)
             await self._test_list_indexes(client, index_name)
             await self._test_get_index(client, index_name)
@@ -80,15 +80,18 @@
 
     async def _test_get_index(self, client, index_name):
         result = await client.get_index(index_name)
         assert result.name == index_name
 
     async def _test_get_index_statistics(self, client, index_name):
         result = await client.get_index_statistics(index_name)
-        assert set(result.keys()) == {"document_count", "storage_size"}
+        keys = set(result.keys())
+        assert "document_count" in keys
+        assert "storage_size" in keys
+        assert "vector_index_size" in keys
 
     async def _test_delete_indexes_if_unchanged(self, client):
         # First create an index
         name = "hotels-del-unchanged"
         fields = [
             {"name": "hotelId", "type": "Edm.String", "key": True, "searchable": False},
             {"name": "baseRate", "type": "Edm.Double"},
```

## Comparing `azure-search-documents-11.4.0b6/tests/async_tests/test_search_index_client_async.py` & `azure-search-documents-11.4.0b7/tests/async_tests/test_search_index_client_async.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/tests/async_tests/test_search_indexer_client_live_async.py` & `azure-search-documents-11.4.0b7/tests/async_tests/test_search_indexer_client_live_async.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 class TestSearchIndexerClientTestAsync(AzureRecordedTestCase):
     @SearchEnvVarPreparer()
     @search_decorator(schema="hotel_schema.json", index_batch="hotel_small.json")
     @recorded_by_proxy_async
     async def test_search_indexers(self, endpoint, api_key, **kwargs):
         storage_cs = kwargs.get("search_storage_connection_string")
         container_name = kwargs.get("search_storage_container_name")
-        client = SearchIndexerClient(endpoint, api_key)
-        index_client = SearchIndexClient(endpoint, api_key)
+        client = SearchIndexerClient(endpoint, api_key, retry_backoff_factor=60)
+        index_client = SearchIndexClient(endpoint, api_key, retry_backoff_factor=60)
         async with client:
             async with index_client:
                 await self._test_create_indexer(client, index_client, storage_cs, container_name)
                 await self._test_delete_indexer(client, index_client, storage_cs, container_name)
                 await self._test_get_indexer(client, index_client, storage_cs, container_name)
                 await self._test_list_indexer(client, index_client, storage_cs, container_name)
                 await self._test_create_or_update_indexer(client, index_client, storage_cs, container_name)
```

## Comparing `azure-search-documents-11.4.0b6/tests/async_tests/test_search_client_search_live_async.py` & `azure-search-documents-11.4.0b7/tests/async_tests/test_search_client_search_live_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 class TestClientTestAsync(AzureRecordedTestCase):
     @SearchEnvVarPreparer()
     @search_decorator(schema="hotel_schema.json", index_batch="hotel_small.json")
     @recorded_by_proxy_async
     async def test_search_client(self, endpoint, api_key, index_name):
-        client = SearchClient(endpoint, index_name, api_key)
+        client = SearchClient(endpoint, index_name, api_key, retry_backoff_factor=60)
         async with client:
             await self._test_get_search_simple(client)
             await self._test_get_search_simple_with_top(client)
             await self._test_get_search_filter(client)
             await self._test_get_search_filter_array(client)
             await self._test_get_search_counts(client)
             await self._test_get_search_coverage(client)
```

## Comparing `azure-search-documents-11.4.0b6/tests/async_tests/test_buffered_sender_async.py` & `azure-search-documents-11.4.0b7/tests/async_tests/test_buffered_sender_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,25 +51,25 @@
         async with SearchIndexingBufferedSender("endpoint", "index name", CREDENTIAL, auto_flush=False) as client:
             await client.upload_documents(["upload1"])
             await client.delete_documents(["delete1", "delete2"])
         assert mock_cleanup.called
 
     async def test_flush(self):
         DOCUMENT = {
-            "Category": "Hotel",
-            "HotelId": "1000",
-            "Rating": 4.0,
-            "Rooms": [],
-            "HotelName": "Azure Inn",
+            "category": "Hotel",
+            "hotelId": "1000",
+            "rating": 4.0,
+            "rooms": [],
+            "hotelName": "Azure Inn",
         }
         with mock.patch.object(
             SearchIndexingBufferedSender, "_index_documents_actions", side_effect=HttpResponseError("Error")
         ):
             async with SearchIndexingBufferedSender("endpoint", "index name", CREDENTIAL, auto_flush=False) as client:
-                client._index_key = "HotelId"
+                client._index_key = "hotelId"
                 await client.upload_documents([DOCUMENT])
                 await client.flush()
                 assert len(client.actions) == 0
 
     async def test_callback_new(self):
         on_new = mock.AsyncMock()
         async with SearchIndexingBufferedSender(
```

## Comparing `azure-search-documents-11.4.0b6/tests/perfstress_tests/search_documents.py` & `azure-search-documents-11.4.0b7/tests/perfstress_tests/search_documents.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/tests/perfstress_tests/autocomplete.py` & `azure-search-documents-11.4.0b7/tests/perfstress_tests/autocomplete.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/tests/perfstress_tests/suggest.py` & `azure-search-documents-11.4.0b7/tests/perfstress_tests/suggest.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/_headers_mixin.py` & `azure-search-documents-11.4.0b7/azure/search/documents/_headers_mixin.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/_search_client.py` & `azure-search-documents-11.4.0b7/azure/search/documents/_search_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,17 +158,15 @@
         semantic_fields: Optional[List[str]] = None,
         semantic_configuration_name: Optional[str] = None,
         select: Optional[List[str]] = None,
         skip: Optional[int] = None,
         top: Optional[int] = None,
         scoring_statistics: Optional[Union[str, ScoringStatistics]] = None,
         session_id: Optional[str] = None,
-        vector: Optional[List[float]] = None,
-        top_k: Optional[int] = None,
-        vector_fields: Optional[str] = None,
+        vectors: Optional[List[Vector]] = None,
         semantic_error_handling: Optional[Union[str, SemanticErrorHandling]] = None,
         semantic_max_wait_in_milliseconds: Optional[int] = None,
         debug: Optional[Union[str, QueryDebugMode]] = None,
         **kwargs: Any
     ) -> SearchItemPaged[Dict]:
         # pylint:disable=too-many-locals, disable=redefined-builtin
         """Search the Azure search index for documents.
@@ -271,21 +269,16 @@
          "partial" and "fail".
         :paramtype semantic_error_handling: str or ~azure.search.documents.models.SemanticErrorHandling
         :keyword int semantic_max_wait_in_milliseconds: Allows the user to set an upper bound on the amount of
          time it takes for semantic enrichment to finish processing before the request fails.
         :keyword debug: Enables a debugging tool that can be used to further explore your Semantic search
          results. Known values are: "disabled", "speller", "semantic", and "all".
         :paramtype debug: str or ~azure.search.documents.models.QueryDebugMode
-        :keyword vector: The vector representation of a search query.
-        :paramtype vector: List[float]
-        :keyword top_k: Number of nearest neighbors to return as top hits.
-        :paramtype top_k: int
-        :keyword vector_fields: Vector Fields of type Collection(Edm.Single) to be included in the vector
-          searched.
-        :paramtype vector_fields: str
+        :keyword vectors: The query parameters for multi-vector search queries.
+        :paramtype vectors: list[Vector]
         :rtype:  SearchItemPaged[Dict]
 
         .. admonition:: Example:
 
             .. literalinclude:: ../samples/sample_simple_query.py
                 :start-after: [START simple_query]
                 :end-before: [END simple_query]
@@ -321,17 +314,14 @@
         captions = (
             query_caption
             if not query_caption_highlight
             else "{}|highlight-{}".format(query_caption, query_caption_highlight)
         )
 
         semantic_configuration = semantic_configuration_name
-        vector_option = None
-        if vector or top_k or vector_fields:
-            vector_option = Vector(value=vector, k=top_k, fields=vector_fields)
 
         query = SearchQuery(
             search_text=search_text,
             include_total_result_count=include_total_result_count,
             facets=facets,
             filter=filter_arg,
             highlight_fields=highlight_fields,
@@ -351,15 +341,15 @@
             semantic_fields=",".join(semantic_fields) if semantic_fields else None,
             semantic_configuration=semantic_configuration,
             select=select if isinstance(select, str) else None,
             skip=skip,
             top=top,
             session_id=session_id,
             scoring_statistics=scoring_statistics,
-            vector=vector_option,
+            vectors=vectors,
             semantic_error_handling=semantic_error_handling,
             semantic_max_wait_in_milliseconds=semantic_max_wait_in_milliseconds,
             debug=debug,
         )
         if isinstance(select, list):
             query.select(select)
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/_queries.py` & `azure-search-documents-11.4.0b7/azure/search/documents/_queries.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/__init__.py` & `azure-search-documents-11.4.0b7/azure/search/documents/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/_search_indexing_buffered_sender.py` & `azure-search-documents-11.4.0b7/azure/search/documents/_search_indexing_buffered_sender.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/_utils.py` & `azure-search-documents-11.4.0b7/azure/search/documents/_utils.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/_index_documents_batch.py` & `azure-search-documents-11.4.0b7/azure/search/documents/_index_documents_batch.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/_search_indexing_buffered_sender_base.py` & `azure-search-documents-11.4.0b7/azure/search/documents/_search_indexing_buffered_sender_base.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/_paging.py` & `azure-search-documents-11.4.0b7/azure/search/documents/_paging.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_search_index_client.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_search_index_client.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_search_indexer_client.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_search_indexer_client.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/__init__.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_utils.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_utils.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/models/_models.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/models/_models.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/models/_index.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/models/_index.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/models/__init__.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/models/_edm.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/models/_edm.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/aio/_search_index_client.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/aio/_search_index_client.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/aio/_search_indexer_client.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/aio/_search_indexer_client.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/aio/__init__.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/_patch.py` & `azure-search-documents-11.4.0b7/azure/search/documents/_generated/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/_serialization.py` & `azure-search-documents-11.4.0b7/azure/search/documents/_generated/_serialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -658,16 +658,17 @@
                         _new_attr = new_attr
                         _serialized = serialized
                         for k in keys:  # type: ignore
                             if k not in _serialized:
                                 _serialized.update(_new_attr)  # type: ignore
                             _new_attr = _new_attr[k]  # type: ignore
                             _serialized = _serialized[k]
-                except ValueError:
-                    continue
+                except ValueError as err:
+                    if isinstance(err, SerializationError):
+                        raise
 
         except (AttributeError, KeyError, TypeError) as err:
             msg = "Attribute {} in object {} cannot be serialized.\n{}".format(attr_name, class_name, str(target_obj))
             raise_with_traceback(SerializationError, msg, err)
         else:
             return serialized
 
@@ -737,26 +738,26 @@
             return output
 
     def query(self, name, data, data_type, **kwargs):
         """Serialize data intended for a URL query.
 
         :param data: The data to be serialized.
         :param str data_type: The type to be serialized from.
+        :keyword bool skip_quote: Whether to skip quote the serialized result.
+        Defaults to False.
         :rtype: str
         :raises: TypeError if serialization fails.
         :raises: ValueError if data is None
         """
         try:
             # Treat the list aside, since we don't want to encode the div separator
             if data_type.startswith("["):
                 internal_data_type = data_type[1:-1]
-                data = [self.serialize_data(d, internal_data_type, **kwargs) if d is not None else "" for d in data]
-                if not kwargs.get("skip_quote", False):
-                    data = [quote(str(d), safe="") for d in data]
-                return str(self.serialize_iter(data, internal_data_type, **kwargs))
+                do_quote = not kwargs.get("skip_quote", False)
+                return str(self.serialize_iter(data, internal_data_type, do_quote=do_quote, **kwargs))
 
             # Not a list, regular serialization
             output = self.serialize_data(data, data_type, **kwargs)
             if data_type == "bool":
                 output = json.dumps(output)
             if kwargs.get("skip_quote") is True:
                 output = str(output)
@@ -887,29 +888,36 @@
 
         :param list attr: Object to be serialized.
         :param str iter_type: Type of object in the iterable.
         :param bool required: Whether the objects in the iterable must
          not be None or empty.
         :param str div: If set, this str will be used to combine the elements
          in the iterable into a combined string. Default is 'None'.
+        :keyword bool do_quote: Whether to quote the serialized result of each iterable element.
+        Defaults to False.
         :rtype: list, str
         """
         if isinstance(data, str):
             raise SerializationError("Refuse str type as a valid iter type.")
 
         serialization_ctxt = kwargs.get("serialization_ctxt", {})
         is_xml = kwargs.get("is_xml", False)
 
         serialized = []
         for d in data:
             try:
                 serialized.append(self.serialize_data(d, iter_type, **kwargs))
-            except ValueError:
+            except ValueError as err:
+                if isinstance(err, SerializationError):
+                    raise
                 serialized.append(None)
 
+        if kwargs.get("do_quote", False):
+            serialized = ["" if s is None else quote(str(s), safe="") for s in serialized]
+
         if div:
             serialized = ["" if s is None else str(s) for s in serialized]
             serialized = div.join(serialized)
 
         if "xml" in serialization_ctxt or is_xml:
             # XML serialization is more complicated
             xml_desc = serialization_ctxt.get("xml", {})
@@ -946,15 +954,17 @@
         :rtype: dict
         """
         serialization_ctxt = kwargs.get("serialization_ctxt", {})
         serialized = {}
         for key, value in attr.items():
             try:
                 serialized[self.serialize_unicode(key)] = self.serialize_data(value, dict_type, **kwargs)
-            except ValueError:
+            except ValueError as err:
+                if isinstance(err, SerializationError):
+                    raise
                 serialized[self.serialize_unicode(key)] = None
 
         if "xml" in serialization_ctxt:
             # XML serialization is more complicated
             xml_desc = serialization_ctxt["xml"]
             xml_name = xml_desc["name"]
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/_configuration.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/__init__.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._search_service_client import SearchServiceClient
 
 try:
     from ._patch import __all__ as _patch_all
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/_search_service_client.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/_search_service_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
 from typing import Any
 
 from azure.core import PipelineClient
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/models/_search_service_client_enums.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/models/_search_service_client_enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from enum import Enum
 from azure.core import CaseInsensitiveEnumMeta
 
 
@@ -145,15 +145,15 @@
     URL = "url"
     """Entities describing a URL."""
     EMAIL = "email"
     """Entities describing an email address."""
 
 
 class EntityRecognitionSkillLanguage(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """The language codes supported for input text by EntityRecognitionSkill."""
+    """Deprecated. The language codes supported for input text by EntityRecognitionSkill."""
 
     AR = "ar"
     """Arabic"""
     CS = "cs"
     """Czech"""
     ZH_HANS = "zh-Hans"
     """Chinese-Simplified"""
@@ -1339,15 +1339,16 @@
     """Indicates that a field contains a date/time value, including timezone information."""
     GEOGRAPHY_POINT = "Edm.GeographyPoint"
     """Indicates that a field contains a geo-location in terms of longitude and latitude."""
     COMPLEX = "Edm.ComplexType"
     """Indicates that a field contains one or more complex objects that in turn have sub-fields of
     #: other types."""
     SINGLE = "Edm.Single"
-    """Indicates that a field contains a single-precision floating point number."""
+    """Indicates that a field contains a single-precision floating point number. This is only valid
+    #: when used with Collection(Edm.Single)."""
 
 
 class SearchIndexerDataSourceType(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Defines the type of a datasource."""
 
     AZURE_SQL = "azuresql"
     """Indicates an Azure SQL datasource."""
@@ -1360,15 +1361,15 @@
     MY_SQL = "mysql"
     """Indicates a MySql datasource."""
     ADLS_GEN2 = "adlsgen2"
     """Indicates an ADLS Gen2 datasource."""
 
 
 class SentimentSkillLanguage(str, Enum, metaclass=CaseInsensitiveEnumMeta):
-    """The language codes supported for input text by SentimentSkill."""
+    """Deprecated. The language codes supported for input text by SentimentSkill."""
 
     DA = "da"
     """Danish"""
     NL = "nl"
     """Dutch"""
     EN = "en"
     """English"""
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/models/_patch.py` & `azure-search-documents-11.4.0b7/azure/search/documents/_generated/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/models/__init__.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._models_py3 import AnalyzeRequest
 from ._models_py3 import AnalyzeResult
 from ._models_py3 import AnalyzedTokenInfo
 from ._models_py3 import AsciiFoldingTokenFilter
@@ -44,14 +44,15 @@
 from ._models_py3 import FieldMapping
 from ._models_py3 import FieldMappingFunction
 from ._models_py3 import FreshnessScoringFunction
 from ._models_py3 import FreshnessScoringParameters
 from ._models_py3 import GetIndexStatisticsResult
 from ._models_py3 import HighWaterMarkChangeDetectionPolicy
 from ._models_py3 import HnswParameters
+from ._models_py3 import HnswVectorSearchAlgorithmConfiguration
 from ._models_py3 import ImageAnalysisSkill
 from ._models_py3 import IndexerCurrentState
 from ._models_py3 import IndexerExecutionResult
 from ._models_py3 import IndexingParameters
 from ._models_py3 import IndexingParametersConfiguration
 from ._models_py3 import IndexingSchedule
 from ._models_py3 import InputFieldMappingEntry
@@ -249,14 +250,15 @@
     "FieldMapping",
     "FieldMappingFunction",
     "FreshnessScoringFunction",
     "FreshnessScoringParameters",
     "GetIndexStatisticsResult",
     "HighWaterMarkChangeDetectionPolicy",
     "HnswParameters",
+    "HnswVectorSearchAlgorithmConfiguration",
     "ImageAnalysisSkill",
     "IndexerCurrentState",
     "IndexerExecutionResult",
     "IndexingParameters",
     "IndexingParametersConfiguration",
     "IndexingSchedule",
     "InputFieldMappingEntry",
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/models/_models_py3.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/models/_models_py3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,22 @@
 # coding=utf-8
 # pylint: disable=too-many-lines
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 import datetime
-import sys
 from typing import Any, Dict, List, Optional, TYPE_CHECKING, Union
 
 from .. import _serialization
 
-if sys.version_info >= (3, 9):
-    from collections.abc import MutableMapping
-else:
-    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
-
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from .. import models as _models
-JSON = MutableMapping[str, Any]  # pylint: disable=unsubscriptable-object
 
 
 class AnalyzedTokenInfo(_serialization.Model):
     """Information about a token returned by an analyzer.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
@@ -2140,15 +2133,15 @@
     :vartype outputs: list[~search_service_client.models.OutputFieldMappingEntry]
     :ivar parsing_mode: The parsingMode for the skill. Will be set to 'default' if not defined.
     :vartype parsing_mode: str
     :ivar data_to_extract: The type of data to be extracted for the skill. Will be set to
      'contentAndMetadata' if not defined.
     :vartype data_to_extract: str
     :ivar configuration: A dictionary of configurations for the skill.
-    :vartype configuration: dict[str, JSON]
+    :vartype configuration: dict[str, any]
     """
 
     _validation = {
         "odata_type": {"required": True},
         "inputs": {"required": True},
         "outputs": {"required": True},
     }
@@ -2171,15 +2164,15 @@
         inputs: List["_models.InputFieldMappingEntry"],
         outputs: List["_models.OutputFieldMappingEntry"],
         name: Optional[str] = None,
         description: Optional[str] = None,
         context: Optional[str] = None,
         parsing_mode: Optional[str] = None,
         data_to_extract: Optional[str] = None,
-        configuration: Optional[Dict[str, JSON]] = None,
+        configuration: Optional[Dict[str, Any]] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword name: The name of the skill which uniquely identifies it within the skillset. A skill
          with no name defined will be given a default name of its 1-based index in the skills array,
          prefixed with the character '#'.
         :paramtype name: str
@@ -2198,15 +2191,15 @@
         :paramtype outputs: list[~search_service_client.models.OutputFieldMappingEntry]
         :keyword parsing_mode: The parsingMode for the skill. Will be set to 'default' if not defined.
         :paramtype parsing_mode: str
         :keyword data_to_extract: The type of data to be extracted for the skill. Will be set to
          'contentAndMetadata' if not defined.
         :paramtype data_to_extract: str
         :keyword configuration: A dictionary of configurations for the skill.
-        :paramtype configuration: dict[str, JSON]
+        :paramtype configuration: dict[str, any]
         """
         super().__init__(name=name, description=description, context=context, inputs=inputs, outputs=outputs, **kwargs)
         self.odata_type: str = "#Microsoft.Skills.Util.DocumentExtractionSkill"
         self.parsing_mode = parsing_mode
         self.data_to_extract = data_to_extract
         self.configuration = configuration
 
@@ -2581,15 +2574,15 @@
         self.odata_type: str = "#Microsoft.Skills.Text.V3.EntityLinkingSkill"
         self.default_language_code = default_language_code
         self.minimum_precision = minimum_precision
         self.model_version = model_version
 
 
 class EntityRecognitionSkill(SearchIndexerSkill):
-    """Text analytics entity recognition.
+    """This skill is deprecated. Use the V3.EntityRecognitionSkill instead.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar odata_type: Identifies the concrete type of the skill. Required.
     :vartype odata_type: str
     :ivar name: The name of the skill which uniquely identifies it within the skillset. A skill
      with no name defined will be given a default name of its 1-based index in the skills array,
@@ -2863,33 +2856,33 @@
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar name: The name of the field mapping function. Required.
     :vartype name: str
     :ivar parameters: A dictionary of parameter name/value pairs to pass to the function. Each
      value must be of a primitive type.
-    :vartype parameters: dict[str, JSON]
+    :vartype parameters: dict[str, any]
     """
 
     _validation = {
         "name": {"required": True},
     }
 
     _attribute_map = {
         "name": {"key": "name", "type": "str"},
         "parameters": {"key": "parameters", "type": "{object}"},
     }
 
-    def __init__(self, *, name: str, parameters: Optional[Dict[str, JSON]] = None, **kwargs: Any) -> None:
+    def __init__(self, *, name: str, parameters: Optional[Dict[str, Any]] = None, **kwargs: Any) -> None:
         """
         :keyword name: The name of the field mapping function. Required.
         :paramtype name: str
         :keyword parameters: A dictionary of parameter name/value pairs to pass to the function. Each
          value must be of a primitive type.
-        :paramtype parameters: dict[str, JSON]
+        :paramtype parameters: dict[str, any]
         """
         super().__init__(**kwargs)
         self.name = name
         self.parameters = parameters
 
 
 class FreshnessScoringFunction(ScoringFunction):
@@ -2991,31 +2984,36 @@
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar document_count: The number of documents in the index. Required.
     :vartype document_count: int
     :ivar storage_size: The amount of storage in bytes consumed by the index. Required.
     :vartype storage_size: int
+    :ivar vector_index_size: The amount of memory in bytes consumed by vectors in the index.
+    :vartype vector_index_size: int
     """
 
     _validation = {
         "document_count": {"required": True, "readonly": True},
         "storage_size": {"required": True, "readonly": True},
+        "vector_index_size": {"readonly": True},
     }
 
     _attribute_map = {
         "document_count": {"key": "documentCount", "type": "int"},
         "storage_size": {"key": "storageSize", "type": "int"},
+        "vector_index_size": {"key": "vectorIndexSize", "type": "int"},
     }
 
     def __init__(self, **kwargs: Any) -> None:
         """ """
         super().__init__(**kwargs)
         self.document_count = None
         self.storage_size = None
+        self.vector_index_size = None
 
 
 class HighWaterMarkChangeDetectionPolicy(DataChangeDetectionPolicy):
     """Defines a data change detection policy that captures changes based on the value of a high water
     mark column.
 
     All required parameters must be populated in order to send to Azure.
@@ -3112,14 +3110,89 @@
         super().__init__(**kwargs)
         self.m = m
         self.ef_construction = ef_construction
         self.ef_search = ef_search
         self.metric = metric
 
 
+class VectorSearchAlgorithmConfiguration(_serialization.Model):
+    """Contains configuration options specific to the algorithm used during indexing time.
+
+    You probably want to use the sub-classes and not this class directly. Known sub-classes are:
+    HnswVectorSearchAlgorithmConfiguration
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar name: The name to associate with this particular configuration. Required.
+    :vartype name: str
+    :ivar kind: The name of the kind of algorithm being configured for use with vector search. Only
+     ``hnsw`` is supported in the current preview. Required.
+    :vartype kind: str
+    """
+
+    _validation = {
+        "name": {"required": True},
+        "kind": {"required": True},
+    }
+
+    _attribute_map = {
+        "name": {"key": "name", "type": "str"},
+        "kind": {"key": "kind", "type": "str"},
+    }
+
+    _subtype_map = {"kind": {"hnsw": "HnswVectorSearchAlgorithmConfiguration"}}
+
+    def __init__(self, *, name: str, **kwargs: Any) -> None:
+        """
+        :keyword name: The name to associate with this particular configuration. Required.
+        :paramtype name: str
+        """
+        super().__init__(**kwargs)
+        self.name = name
+        self.kind: Optional[str] = None
+
+
+class HnswVectorSearchAlgorithmConfiguration(VectorSearchAlgorithmConfiguration):
+    """Contains configuration options specific to the hnsw approximate nearest neighbors algorithm
+    used during indexing time.
+
+    All required parameters must be populated in order to send to Azure.
+
+    :ivar name: The name to associate with this particular configuration. Required.
+    :vartype name: str
+    :ivar kind: The name of the kind of algorithm being configured for use with vector search. Only
+     ``hnsw`` is supported in the current preview. Required.
+    :vartype kind: str
+    :ivar parameters: Contains the parameters specific to hnsw algorithm.
+    :vartype parameters: ~search_service_client.models.HnswParameters
+    """
+
+    _validation = {
+        "name": {"required": True},
+        "kind": {"required": True},
+    }
+
+    _attribute_map = {
+        "name": {"key": "name", "type": "str"},
+        "kind": {"key": "kind", "type": "str"},
+        "parameters": {"key": "hnswParameters", "type": "HnswParameters"},
+    }
+
+    def __init__(self, *, name: str, parameters: Optional["_models.HnswParameters"] = None, **kwargs: Any) -> None:
+        """
+        :keyword name: The name to associate with this particular configuration. Required.
+        :paramtype name: str
+        :keyword parameters: Contains the parameters specific to hnsw algorithm.
+        :paramtype parameters: ~search_service_client.models.HnswParameters
+        """
+        super().__init__(name=name, **kwargs)
+        self.kind: str = "hnsw"
+        self.parameters = parameters
+
+
 class ImageAnalysisSkill(SearchIndexerSkill):
     """A skill that analyzes image files. It extracts a rich set of visual features based on the image
     content.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar odata_type: Identifies the concrete type of the skill. Required.
@@ -3423,15 +3496,15 @@
 
 class IndexingParametersConfiguration(_serialization.Model):  # pylint: disable=too-many-instance-attributes
     """A dictionary of indexer-specific configuration properties. Each name is the name of a specific
     property. Each value must be of a primitive type.
 
     :ivar additional_properties: Unmatched properties from the message are deserialized to this
      collection.
-    :vartype additional_properties: dict[str, JSON]
+    :vartype additional_properties: dict[str, any]
     :ivar parsing_mode: Represents the parsing mode for indexing from an Azure blob data source.
      Known values are: "default", "text", "delimitedText", "json", "jsonArray", and "jsonLines".
     :vartype parsing_mode: str or ~search_service_client.models.BlobIndexerParsingMode
     :ivar excluded_file_name_extensions: Comma-delimited list of filename extensions to ignore when
      processing from Azure blob storage.  For example, you could exclude ".png, .mp4" to skip over
      those files during indexing.
     :vartype excluded_file_name_extensions: str
@@ -3514,15 +3587,15 @@
         "execution_environment": {"key": "executionEnvironment", "type": "str"},
         "query_timeout": {"key": "queryTimeout", "type": "str"},
     }
 
     def __init__(
         self,
         *,
-        additional_properties: Optional[Dict[str, JSON]] = None,
+        additional_properties: Optional[Dict[str, Any]] = None,
         parsing_mode: Union[str, "_models.BlobIndexerParsingMode"] = "default",
         excluded_file_name_extensions: str = "",
         indexed_file_name_extensions: str = "",
         fail_on_unsupported_content_type: bool = False,
         fail_on_unprocessable_document: bool = False,
         index_storage_metadata_only_for_oversized_documents: bool = False,
         delimited_text_headers: Optional[str] = None,
@@ -3536,15 +3609,15 @@
         execution_environment: Union[str, "_models.IndexerExecutionEnvironment"] = "standard",
         query_timeout: str = "00:05:00",
         **kwargs: Any
     ) -> None:
         """
         :keyword additional_properties: Unmatched properties from the message are deserialized to this
          collection.
-        :paramtype additional_properties: dict[str, JSON]
+        :paramtype additional_properties: dict[str, any]
         :keyword parsing_mode: Represents the parsing mode for indexing from an Azure blob data source.
          Known values are: "default", "text", "delimitedText", "json", "jsonArray", and "jsonLines".
         :paramtype parsing_mode: str or ~search_service_client.models.BlobIndexerParsingMode
         :keyword excluded_file_name_extensions: Comma-delimited list of filename extensions to ignore
          when processing from Azure blob storage.  For example, you could exclude ".png, .mp4" to skip
          over those files during indexing.
         :paramtype excluded_file_name_extensions: str
@@ -7838,16 +7911,16 @@
         super().__init__(**kwargs)
         self.field_name = field_name
 
 
 class SemanticSettings(_serialization.Model):
     """Defines parameters for a search index that influence semantic capabilities.
 
-    :ivar default_configuration: Allows you to set a default semantic configuration in your index,
-     making it optional to pass it on as a query parameter every time.
+    :ivar default_configuration: Allows you to set the name of a default semantic configuration in
+     your index, making it optional to pass it on as a query parameter every time.
     :vartype default_configuration: str
     :ivar configurations: The semantic configurations for the index.
     :vartype configurations: list[~search_service_client.models.SemanticConfiguration]
     """
 
     _attribute_map = {
         "default_configuration": {"key": "defaultConfiguration", "type": "str"},
@@ -7858,28 +7931,27 @@
         self,
         *,
         default_configuration: Optional[str] = None,
         configurations: Optional[List["_models.SemanticConfiguration"]] = None,
         **kwargs: Any
     ) -> None:
         """
-        :keyword default_configuration: Allows you to set a default semantic configuration in your
-         index, making it optional to pass it on as a query parameter every time.
+        :keyword default_configuration: Allows you to set the name of a default semantic configuration
+         in your index, making it optional to pass it on as a query parameter every time.
         :paramtype default_configuration: str
         :keyword configurations: The semantic configurations for the index.
         :paramtype configurations: list[~search_service_client.models.SemanticConfiguration]
         """
         super().__init__(**kwargs)
         self.default_configuration = default_configuration
         self.configurations = configurations
 
 
 class SentimentSkill(SearchIndexerSkill):
-    """Text analytics positive-negative sentiment analysis, scored as a floating point value in a
-    range of zero to 1.
+    """This skill is deprecated. Use the V3.SentimentSkill instead.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar odata_type: Identifies the concrete type of the skill. Required.
     :vartype odata_type: str
     :ivar name: The name of the skill which uniquely identifies it within the skillset. A skill
      with no name defined will be given a default name of its 1-based index in the skills array,
@@ -8063,93 +8135,105 @@
 
 
 class ServiceCounters(_serialization.Model):
     """Represents service-level resource counters and quotas.
 
     All required parameters must be populated in order to send to Azure.
 
-    :ivar alias_counter: Total number of aliases.
+    :ivar alias_counter: Total number of aliases. Required.
     :vartype alias_counter: ~search_service_client.models.ResourceCounter
     :ivar document_counter: Total number of documents across all indexes in the service. Required.
     :vartype document_counter: ~search_service_client.models.ResourceCounter
     :ivar index_counter: Total number of indexes. Required.
     :vartype index_counter: ~search_service_client.models.ResourceCounter
     :ivar indexer_counter: Total number of indexers. Required.
     :vartype indexer_counter: ~search_service_client.models.ResourceCounter
     :ivar data_source_counter: Total number of data sources. Required.
     :vartype data_source_counter: ~search_service_client.models.ResourceCounter
     :ivar storage_size_counter: Total size of used storage in bytes. Required.
     :vartype storage_size_counter: ~search_service_client.models.ResourceCounter
     :ivar synonym_map_counter: Total number of synonym maps. Required.
     :vartype synonym_map_counter: ~search_service_client.models.ResourceCounter
-    :ivar skillset_counter: Total number of skillsets.
+    :ivar skillset_counter: Total number of skillsets. Required.
     :vartype skillset_counter: ~search_service_client.models.ResourceCounter
+    :ivar vector_index_size_counter: Total memory consumption of all vector indexes within the
+     service, in bytes. Required.
+    :vartype vector_index_size_counter: ~search_service_client.models.ResourceCounter
     """
 
     _validation = {
+        "alias_counter": {"required": True},
         "document_counter": {"required": True},
         "index_counter": {"required": True},
         "indexer_counter": {"required": True},
         "data_source_counter": {"required": True},
         "storage_size_counter": {"required": True},
         "synonym_map_counter": {"required": True},
+        "skillset_counter": {"required": True},
+        "vector_index_size_counter": {"required": True},
     }
 
     _attribute_map = {
         "alias_counter": {"key": "aliasesCount", "type": "ResourceCounter"},
         "document_counter": {"key": "documentCount", "type": "ResourceCounter"},
         "index_counter": {"key": "indexesCount", "type": "ResourceCounter"},
         "indexer_counter": {"key": "indexersCount", "type": "ResourceCounter"},
         "data_source_counter": {"key": "dataSourcesCount", "type": "ResourceCounter"},
         "storage_size_counter": {"key": "storageSize", "type": "ResourceCounter"},
         "synonym_map_counter": {"key": "synonymMaps", "type": "ResourceCounter"},
         "skillset_counter": {"key": "skillsetCount", "type": "ResourceCounter"},
+        "vector_index_size_counter": {"key": "vectorIndexSize", "type": "ResourceCounter"},
     }
 
     def __init__(
         self,
         *,
+        alias_counter: "_models.ResourceCounter",
         document_counter: "_models.ResourceCounter",
         index_counter: "_models.ResourceCounter",
         indexer_counter: "_models.ResourceCounter",
         data_source_counter: "_models.ResourceCounter",
         storage_size_counter: "_models.ResourceCounter",
         synonym_map_counter: "_models.ResourceCounter",
-        alias_counter: Optional["_models.ResourceCounter"] = None,
-        skillset_counter: Optional["_models.ResourceCounter"] = None,
+        skillset_counter: "_models.ResourceCounter",
+        vector_index_size_counter: "_models.ResourceCounter",
         **kwargs: Any
     ) -> None:
         """
-        :keyword alias_counter: Total number of aliases.
+        :keyword alias_counter: Total number of aliases. Required.
         :paramtype alias_counter: ~search_service_client.models.ResourceCounter
         :keyword document_counter: Total number of documents across all indexes in the service.
          Required.
         :paramtype document_counter: ~search_service_client.models.ResourceCounter
         :keyword index_counter: Total number of indexes. Required.
         :paramtype index_counter: ~search_service_client.models.ResourceCounter
         :keyword indexer_counter: Total number of indexers. Required.
         :paramtype indexer_counter: ~search_service_client.models.ResourceCounter
         :keyword data_source_counter: Total number of data sources. Required.
         :paramtype data_source_counter: ~search_service_client.models.ResourceCounter
         :keyword storage_size_counter: Total size of used storage in bytes. Required.
         :paramtype storage_size_counter: ~search_service_client.models.ResourceCounter
         :keyword synonym_map_counter: Total number of synonym maps. Required.
         :paramtype synonym_map_counter: ~search_service_client.models.ResourceCounter
-        :keyword skillset_counter: Total number of skillsets.
+        :keyword skillset_counter: Total number of skillsets. Required.
         :paramtype skillset_counter: ~search_service_client.models.ResourceCounter
+        :keyword vector_index_size_counter: Total memory consumption of all vector indexes within the
+         service, in bytes. Required.
+        :paramtype vector_index_size_counter: ~search_service_client.models.ResourceCounter
         """
         super().__init__(**kwargs)
         self.alias_counter = alias_counter
         self.document_counter = document_counter
         self.index_counter = index_counter
         self.indexer_counter = indexer_counter
         self.data_source_counter = data_source_counter
         self.storage_size_counter = storage_size_counter
         self.synonym_map_counter = synonym_map_counter
         self.skillset_counter = skillset_counter
+        self.vector_index_size_counter = vector_index_size_counter
 
 
 class ServiceLimits(_serialization.Model):
     """Represents various service level limits.
 
     :ivar max_fields_per_index: The maximum allowed fields per index.
     :vartype max_fields_per_index: int
@@ -9481,57 +9565,14 @@
         :paramtype algorithm_configurations:
          list[~search_service_client.models.VectorSearchAlgorithmConfiguration]
         """
         super().__init__(**kwargs)
         self.algorithm_configurations = algorithm_configurations
 
 
-class VectorSearchAlgorithmConfiguration(_serialization.Model):
-    """Contains configuration options specific to the algorithm used during indexing time.
-
-    All required parameters must be populated in order to send to Azure.
-
-    :ivar name: The name to associate with this particular configuration. Required.
-    :vartype name: str
-    :ivar kind: The name of the kind of algorithm being configured for use with vector search.
-     Required.
-    :vartype kind: str
-    :ivar hnsw_parameters: Contains the parameters specific to hnsw algorithm.
-    :vartype hnsw_parameters: ~search_service_client.models.HnswParameters
-    """
-
-    _validation = {
-        "name": {"required": True},
-        "kind": {"required": True},
-    }
-
-    _attribute_map = {
-        "name": {"key": "name", "type": "str"},
-        "kind": {"key": "kind", "type": "str"},
-        "hnsw_parameters": {"key": "hnswParameters", "type": "HnswParameters"},
-    }
-
-    def __init__(
-        self, *, name: str, kind: str, hnsw_parameters: Optional["_models.HnswParameters"] = None, **kwargs: Any
-    ) -> None:
-        """
-        :keyword name: The name to associate with this particular configuration. Required.
-        :paramtype name: str
-        :keyword kind: The name of the kind of algorithm being configured for use with vector search.
-         Required.
-        :paramtype kind: str
-        :keyword hnsw_parameters: Contains the parameters specific to hnsw algorithm.
-        :paramtype hnsw_parameters: ~search_service_client.models.HnswParameters
-        """
-        super().__init__(**kwargs)
-        self.name = name
-        self.kind = kind
-        self.hnsw_parameters = hnsw_parameters
-
-
 class WebApiSkill(SearchIndexerSkill):  # pylint: disable=too-many-instance-attributes
     """A skill that can call a Web API endpoint, allowing you to extend a skillset by having it call
     your custom code.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar odata_type: Identifies the concrete type of the skill. Required.
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/_patch.py` & `azure-search-documents-11.4.0b7/azure/search/documents/_generated/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/_configuration.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/__init__.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._search_service_client import SearchServiceClient
 
 try:
     from ._patch import __all__ as _patch_all
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/_search_service_client.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/_search_service_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
 from typing import Any, Awaitable
 
 from azure.core import AsyncPipelineClient
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/_vendor.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/_vendor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from abc import ABC
 from typing import TYPE_CHECKING
 
 from azure.core.pipeline.transport import HttpRequest
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/operations/_synonym_maps_operations.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/operations/_synonym_maps_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=too-many-lines
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/operations/_search_service_client_operations.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/operations/_search_service_client_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=too-many-lines
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from typing import Any, Callable, Dict, Optional, TypeVar
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/operations/_indexes_operations.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/operations/_indexes_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=too-many-lines
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/operations/_patch.py` & `azure-search-documents-11.4.0b7/azure/search/documents/_generated/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/operations/__init__.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/operations/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._data_sources_operations import DataSourcesOperations
 from ._indexers_operations import IndexersOperations
 from ._skillsets_operations import SkillsetsOperations
 from ._synonym_maps_operations import SynonymMapsOperations
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/operations/_skillsets_operations.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/operations/_skillsets_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=too-many-lines
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/operations/_data_sources_operations.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/operations/_data_sources_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=too-many-lines
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/operations/_aliases_operations.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/operations/_aliases_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=too-many-lines
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
 from typing import Any, AsyncIterable, Callable, Dict, IO, Optional, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/aio/operations/_indexers_operations.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/operations/_indexers_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=too-many-lines
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/operations/_synonym_maps_operations.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/operations/_synonym_maps_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=too-many-lines
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
@@ -19,15 +19,15 @@
 from azure.core.pipeline.transport import HttpResponse
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 
 from .. import models as _models
 from .._serialization import Serializer
-from .._vendor import SearchServiceClientMixinABC, _convert_request, _format_url_section
+from .._vendor import SearchServiceClientMixinABC, _convert_request
 
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
@@ -50,15 +50,15 @@
 
     # Construct URL
     _url = kwargs.pop("template_url", "/synonymmaps('{synonymMapName}')")
     path_format_arguments = {
         "synonymMapName": _SERIALIZER.url("synonym_map_name", synonym_map_name, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if x_ms_client_request_id is not None:
         _headers["x-ms-client-request-id"] = _SERIALIZER.header("x_ms_client_request_id", x_ms_client_request_id, "str")
@@ -90,15 +90,15 @@
 
     # Construct URL
     _url = kwargs.pop("template_url", "/synonymmaps('{synonymMapName}')")
     path_format_arguments = {
         "synonymMapName": _SERIALIZER.url("synonym_map_name", synonym_map_name, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if x_ms_client_request_id is not None:
         _headers["x-ms-client-request-id"] = _SERIALIZER.header("x_ms_client_request_id", x_ms_client_request_id, "str")
@@ -122,15 +122,15 @@
 
     # Construct URL
     _url = kwargs.pop("template_url", "/synonymmaps('{synonymMapName}')")
     path_format_arguments = {
         "synonymMapName": _SERIALIZER.url("synonym_map_name", synonym_map_name, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if x_ms_client_request_id is not None:
         _headers["x-ms-client-request-id"] = _SERIALIZER.header("x_ms_client_request_id", x_ms_client_request_id, "str")
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/operations/_search_service_client_operations.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/operations/_search_service_client_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=too-many-lines
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from typing import Any, Callable, Dict, Optional, TypeVar
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/operations/_indexes_operations.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/operations/_indexes_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=too-many-lines
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.exceptions import (
@@ -21,15 +21,15 @@
 from azure.core.pipeline.transport import HttpResponse
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 
 from .. import models as _models
 from .._serialization import Serializer
-from .._vendor import SearchServiceClientMixinABC, _convert_request, _format_url_section
+from .._vendor import SearchServiceClientMixinABC, _convert_request
 
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
@@ -102,15 +102,15 @@
 
     # Construct URL
     _url = kwargs.pop("template_url", "/indexes('{indexName}')")
     path_format_arguments = {
         "indexName": _SERIALIZER.url("index_name", index_name, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     if allow_index_downtime is not None:
         _params["allowIndexDowntime"] = _SERIALIZER.query("allow_index_downtime", allow_index_downtime, "bool")
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
@@ -144,15 +144,15 @@
 
     # Construct URL
     _url = kwargs.pop("template_url", "/indexes('{indexName}')")
     path_format_arguments = {
         "indexName": _SERIALIZER.url("index_name", index_name, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if x_ms_client_request_id is not None:
         _headers["x-ms-client-request-id"] = _SERIALIZER.header("x_ms_client_request_id", x_ms_client_request_id, "str")
@@ -174,15 +174,15 @@
 
     # Construct URL
     _url = kwargs.pop("template_url", "/indexes('{indexName}')")
     path_format_arguments = {
         "indexName": _SERIALIZER.url("index_name", index_name, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if x_ms_client_request_id is not None:
         _headers["x-ms-client-request-id"] = _SERIALIZER.header("x_ms_client_request_id", x_ms_client_request_id, "str")
@@ -202,15 +202,15 @@
 
     # Construct URL
     _url = kwargs.pop("template_url", "/indexes('{indexName}')/search.stats")
     path_format_arguments = {
         "indexName": _SERIALIZER.url("index_name", index_name, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if x_ms_client_request_id is not None:
         _headers["x-ms-client-request-id"] = _SERIALIZER.header("x_ms_client_request_id", x_ms_client_request_id, "str")
@@ -231,15 +231,15 @@
 
     # Construct URL
     _url = kwargs.pop("template_url", "/indexes('{indexName}')/search.analyze")
     path_format_arguments = {
         "indexName": _SERIALIZER.url("index_name", index_name, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if x_ms_client_request_id is not None:
         _headers["x-ms-client-request-id"] = _SERIALIZER.header("x_ms_client_request_id", x_ms_client_request_id, "str")
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/operations/_patch.py` & `azure-search-documents-11.4.0b7/azure/search/documents/_generated/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/operations/__init__.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/operations/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._data_sources_operations import DataSourcesOperations
 from ._indexers_operations import IndexersOperations
 from ._skillsets_operations import SkillsetsOperations
 from ._synonym_maps_operations import SynonymMapsOperations
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/operations/_skillsets_operations.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/operations/_skillsets_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=too-many-lines
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
@@ -19,15 +19,15 @@
 from azure.core.pipeline.transport import HttpResponse
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 
 from .. import models as _models
 from .._serialization import Serializer
-from .._vendor import SearchServiceClientMixinABC, _convert_request, _format_url_section
+from .._vendor import SearchServiceClientMixinABC, _convert_request
 
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
@@ -52,15 +52,15 @@
 
     # Construct URL
     _url = kwargs.pop("template_url", "/skillsets('{skillsetName}')")
     path_format_arguments = {
         "skillsetName": _SERIALIZER.url("skillset_name", skillset_name, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
     if skip_indexer_reset_requirement_for_cache is not None:
         _params["ignoreResetRequirements"] = _SERIALIZER.query(
             "skip_indexer_reset_requirement_for_cache", skip_indexer_reset_requirement_for_cache, "bool"
         )
@@ -100,15 +100,15 @@
 
     # Construct URL
     _url = kwargs.pop("template_url", "/skillsets('{skillsetName}')")
     path_format_arguments = {
         "skillsetName": _SERIALIZER.url("skillset_name", skillset_name, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if x_ms_client_request_id is not None:
         _headers["x-ms-client-request-id"] = _SERIALIZER.header("x_ms_client_request_id", x_ms_client_request_id, "str")
@@ -132,15 +132,15 @@
 
     # Construct URL
     _url = kwargs.pop("template_url", "/skillsets('{skillsetName}')")
     path_format_arguments = {
         "skillsetName": _SERIALIZER.url("skillset_name", skillset_name, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if x_ms_client_request_id is not None:
         _headers["x-ms-client-request-id"] = _SERIALIZER.header("x_ms_client_request_id", x_ms_client_request_id, "str")
@@ -210,15 +210,15 @@
 
     # Construct URL
     _url = kwargs.pop("template_url", "/skillsets('{skillsetName}')/search.resetskills")
     path_format_arguments = {
         "skillsetName": _SERIALIZER.url("skillset_name", skillset_name, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if x_ms_client_request_id is not None:
         _headers["x-ms-client-request-id"] = _SERIALIZER.header("x_ms_client_request_id", x_ms_client_request_id, "str")
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/operations/_data_sources_operations.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/operations/_data_sources_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=too-many-lines
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
@@ -19,15 +19,15 @@
 from azure.core.pipeline.transport import HttpResponse
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 
 from .. import models as _models
 from .._serialization import Serializer
-from .._vendor import SearchServiceClientMixinABC, _convert_request, _format_url_section
+from .._vendor import SearchServiceClientMixinABC, _convert_request
 
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
@@ -51,15 +51,15 @@
 
     # Construct URL
     _url = kwargs.pop("template_url", "/datasources('{dataSourceName}')")
     path_format_arguments = {
         "dataSourceName": _SERIALIZER.url("data_source_name", data_source_name, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
     if skip_indexer_reset_requirement_for_cache is not None:
         _params["ignoreResetRequirements"] = _SERIALIZER.query(
             "skip_indexer_reset_requirement_for_cache", skip_indexer_reset_requirement_for_cache, "bool"
         )
@@ -95,15 +95,15 @@
 
     # Construct URL
     _url = kwargs.pop("template_url", "/datasources('{dataSourceName}')")
     path_format_arguments = {
         "dataSourceName": _SERIALIZER.url("data_source_name", data_source_name, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if x_ms_client_request_id is not None:
         _headers["x-ms-client-request-id"] = _SERIALIZER.header("x_ms_client_request_id", x_ms_client_request_id, "str")
@@ -127,15 +127,15 @@
 
     # Construct URL
     _url = kwargs.pop("template_url", "/datasources('{dataSourceName}')")
     path_format_arguments = {
         "dataSourceName": _SERIALIZER.url("data_source_name", data_source_name, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if x_ms_client_request_id is not None:
         _headers["x-ms-client-request-id"] = _SERIALIZER.header("x_ms_client_request_id", x_ms_client_request_id, "str")
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/operations/_aliases_operations.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/operations/_aliases_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=too-many-lines
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
 from typing import Any, Callable, Dict, IO, Iterable, Optional, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.exceptions import (
@@ -21,15 +21,15 @@
 from azure.core.pipeline.transport import HttpResponse
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 
 from .. import models as _models
 from .._serialization import Serializer
-from .._vendor import SearchServiceClientMixinABC, _convert_request, _format_url_section
+from .._vendor import SearchServiceClientMixinABC, _convert_request
 
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
@@ -97,15 +97,15 @@
 
     # Construct URL
     _url = kwargs.pop("template_url", "/aliases('{aliasName}')")
     path_format_arguments = {
         "aliasName": _SERIALIZER.url("alias_name", alias_name, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if x_ms_client_request_id is not None:
         _headers["x-ms-client-request-id"] = _SERIALIZER.header("x_ms_client_request_id", x_ms_client_request_id, "str")
@@ -137,15 +137,15 @@
 
     # Construct URL
     _url = kwargs.pop("template_url", "/aliases('{aliasName}')")
     path_format_arguments = {
         "aliasName": _SERIALIZER.url("alias_name", alias_name, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if x_ms_client_request_id is not None:
         _headers["x-ms-client-request-id"] = _SERIALIZER.header("x_ms_client_request_id", x_ms_client_request_id, "str")
@@ -167,15 +167,15 @@
 
     # Construct URL
     _url = kwargs.pop("template_url", "/aliases('{aliasName}')")
     path_format_arguments = {
         "aliasName": _SERIALIZER.url("alias_name", alias_name, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if x_ms_client_request_id is not None:
         _headers["x-ms-client-request-id"] = _SERIALIZER.header("x_ms_client_request_id", x_ms_client_request_id, "str")
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/indexes/_generated/operations/_indexers_operations.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/operations/_indexers_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=too-many-lines
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
 from typing import Any, Callable, Dict, IO, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
@@ -19,15 +19,15 @@
 from azure.core.pipeline.transport import HttpResponse
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 
 from .. import models as _models
 from .._serialization import Serializer
-from .._vendor import SearchServiceClientMixinABC, _convert_request, _format_url_section
+from .._vendor import SearchServiceClientMixinABC, _convert_request
 
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
@@ -43,15 +43,15 @@
 
     # Construct URL
     _url = kwargs.pop("template_url", "/indexers('{indexerName}')/search.reset")
     path_format_arguments = {
         "indexerName": _SERIALIZER.url("indexer_name", indexer_name, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if x_ms_client_request_id is not None:
         _headers["x-ms-client-request-id"] = _SERIALIZER.header("x_ms_client_request_id", x_ms_client_request_id, "str")
@@ -72,15 +72,15 @@
 
     # Construct URL
     _url = kwargs.pop("template_url", "/indexers('{indexerName}')/search.resetdocs")
     path_format_arguments = {
         "indexerName": _SERIALIZER.url("indexer_name", indexer_name, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     if overwrite is not None:
         _params["overwrite"] = _SERIALIZER.query("overwrite", overwrite, "bool")
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
@@ -102,15 +102,15 @@
 
     # Construct URL
     _url = kwargs.pop("template_url", "/indexers('{indexerName}')/search.run")
     path_format_arguments = {
         "indexerName": _SERIALIZER.url("indexer_name", indexer_name, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if x_ms_client_request_id is not None:
         _headers["x-ms-client-request-id"] = _SERIALIZER.header("x_ms_client_request_id", x_ms_client_request_id, "str")
@@ -139,15 +139,15 @@
 
     # Construct URL
     _url = kwargs.pop("template_url", "/indexers('{indexerName}')")
     path_format_arguments = {
         "indexerName": _SERIALIZER.url("indexer_name", indexer_name, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
     if skip_indexer_reset_requirement_for_cache is not None:
         _params["ignoreResetRequirements"] = _SERIALIZER.query(
             "skip_indexer_reset_requirement_for_cache", skip_indexer_reset_requirement_for_cache, "bool"
         )
@@ -187,15 +187,15 @@
 
     # Construct URL
     _url = kwargs.pop("template_url", "/indexers('{indexerName}')")
     path_format_arguments = {
         "indexerName": _SERIALIZER.url("indexer_name", indexer_name, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if x_ms_client_request_id is not None:
         _headers["x-ms-client-request-id"] = _SERIALIZER.header("x_ms_client_request_id", x_ms_client_request_id, "str")
@@ -217,15 +217,15 @@
 
     # Construct URL
     _url = kwargs.pop("template_url", "/indexers('{indexerName}')")
     path_format_arguments = {
         "indexerName": _SERIALIZER.url("indexer_name", indexer_name, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if x_ms_client_request_id is not None:
         _headers["x-ms-client-request-id"] = _SERIALIZER.header("x_ms_client_request_id", x_ms_client_request_id, "str")
@@ -294,15 +294,15 @@
 
     # Construct URL
     _url = kwargs.pop("template_url", "/indexers('{indexerName}')/search.status")
     path_format_arguments = {
         "indexerName": _SERIALIZER.url("indexer_name", indexer_name, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     if x_ms_client_request_id is not None:
         _headers["x-ms-client-request-id"] = _SERIALIZER.header("x_ms_client_request_id", x_ms_client_request_id, "str")
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/models/__init__.py` & `azure-search-documents-11.4.0b7/azure/search/documents/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/aio/_search_indexing_buffered_sender_async.py` & `azure-search-documents-11.4.0b7/azure/search/documents/aio/_search_indexing_buffered_sender_async.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/aio/_search_client_async.py` & `azure-search-documents-11.4.0b7/azure/search/documents/aio/_search_client_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,17 +164,15 @@
         semantic_fields: Optional[List[str]] = None,
         semantic_configuration_name: Optional[str] = None,
         select: Optional[List[str]] = None,
         skip: Optional[int] = None,
         top: Optional[int] = None,
         scoring_statistics: Optional[Union[str, ScoringStatistics]] = None,
         session_id: Optional[str] = None,
-        vector: Optional[List[float]] = None,
-        top_k: Optional[int] = None,
-        vector_fields: Optional[str] = None,
+        vectors: Optional[List[Vector]] = None,
         semantic_error_handling: Optional[Union[str, SemanticErrorHandling]] = None,
         semantic_max_wait_in_milliseconds: Optional[int] = None,
         debug: Optional[Union[str, QueryDebugMode]] = None,
         **kwargs
     ) -> AsyncSearchItemPaged[Dict]:
         # pylint:disable=too-many-locals, disable=redefined-builtin
         """Search the Azure search index for documents.
@@ -278,21 +276,16 @@
          "partial" and "fail".
         :paramtype semantic_error_handling: str or ~azure.search.documents.models.SemanticErrorHandling
         :keyword int semantic_max_wait_in_milliseconds: Allows the user to set an upper bound on the amount of
          time it takes for semantic enrichment to finish processing before the request fails.
         :keyword debug: Enables a debugging tool that can be used to further explore your Semantic search
          results. Known values are: "disabled", "speller", "semantic", and "all".
         :paramtype debug: str or ~azure.search.documents.models.QueryDebugMode
-        :keyword vector: The vector representation of a search query.
-        :paramtype vector: list[float]
-        :keyword top_k: Number of nearest neighbors to return as top hits.
-        :paramtype top_k: int
-        :keyword vector_fields: Vector Fields of type Collection(Edm.Single) to be included in the vector
-          searched.
-        :paramtype vector_fields: str
+        :keyword vectors: The query parameters for multi-vector search queries.
+        :paramtype vectors: list[Vector]
         :return: A list of documents (dicts) matching the specified search criteria.
         :rtype:  AsyncSearchItemPaged[dict]
 
         .. admonition:: Example:
 
             .. literalinclude:: ../samples/async_samples/sample_simple_query_async.py
                 :start-after: [START simple_query_async]
@@ -326,17 +319,14 @@
         answers = answers if not query_answer_threshold else "{}|threshold-{}".format(answers, query_answer_threshold)
         captions = (
             query_caption
             if not query_caption_highlight
             else "{}|highlight-{}".format(query_caption, query_caption_highlight)
         )
         semantic_configuration = semantic_configuration_name
-        vector_option = None
-        if vector or top_k or vector_fields:
-            vector_option = Vector(value=vector, k=top_k, fields=vector_fields)
 
         query = SearchQuery(
             search_text=search_text,
             include_total_result_count=include_total_result_count,
             facets=facets,
             filter=filter_arg,
             highlight_fields=highlight_fields,
@@ -356,15 +346,15 @@
             semantic_fields=",".join(semantic_fields) if semantic_fields else None,
             semantic_configuration=semantic_configuration,
             select=select if isinstance(select, str) else None,
             skip=skip,
             top=top,
             session_id=session_id,
             scoring_statistics=scoring_statistics,
-            vector=vector_option,
+            vectors=vectors,
             semantic_error_handling=semantic_error_handling,
             semantic_max_wait_in_milliseconds=semantic_max_wait_in_milliseconds,
             debug=debug,
         )
         if isinstance(select, list):
             query.select(select)
         kwargs["headers"] = self._merge_client_headers(kwargs.get("headers"))
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/aio/__init__.py` & `azure-search-documents-11.4.0b7/azure/search/documents/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/aio/_timer.py` & `azure-search-documents-11.4.0b7/azure/search/documents/aio/_timer.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/aio/_index_documents_batch_async.py` & `azure-search-documents-11.4.0b7/azure/search/documents/aio/_index_documents_batch_async.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/aio/_paging.py` & `azure-search-documents-11.4.0b7/azure/search/documents/aio/_paging.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/_generated/_search_index_client.py` & `azure-search-documents-11.4.0b7/azure/search/documents/_generated/_search_index_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
 from typing import Any
 
 from azure.core import PipelineClient
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/_generated/_patch.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/_generated/_serialization.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/_serialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -658,16 +658,17 @@
                         _new_attr = new_attr
                         _serialized = serialized
                         for k in keys:  # type: ignore
                             if k not in _serialized:
                                 _serialized.update(_new_attr)  # type: ignore
                             _new_attr = _new_attr[k]  # type: ignore
                             _serialized = _serialized[k]
-                except ValueError:
-                    continue
+                except ValueError as err:
+                    if isinstance(err, SerializationError):
+                        raise
 
         except (AttributeError, KeyError, TypeError) as err:
             msg = "Attribute {} in object {} cannot be serialized.\n{}".format(attr_name, class_name, str(target_obj))
             raise_with_traceback(SerializationError, msg, err)
         else:
             return serialized
 
@@ -737,26 +738,26 @@
             return output
 
     def query(self, name, data, data_type, **kwargs):
         """Serialize data intended for a URL query.
 
         :param data: The data to be serialized.
         :param str data_type: The type to be serialized from.
+        :keyword bool skip_quote: Whether to skip quote the serialized result.
+        Defaults to False.
         :rtype: str
         :raises: TypeError if serialization fails.
         :raises: ValueError if data is None
         """
         try:
             # Treat the list aside, since we don't want to encode the div separator
             if data_type.startswith("["):
                 internal_data_type = data_type[1:-1]
-                data = [self.serialize_data(d, internal_data_type, **kwargs) if d is not None else "" for d in data]
-                if not kwargs.get("skip_quote", False):
-                    data = [quote(str(d), safe="") for d in data]
-                return str(self.serialize_iter(data, internal_data_type, **kwargs))
+                do_quote = not kwargs.get("skip_quote", False)
+                return str(self.serialize_iter(data, internal_data_type, do_quote=do_quote, **kwargs))
 
             # Not a list, regular serialization
             output = self.serialize_data(data, data_type, **kwargs)
             if data_type == "bool":
                 output = json.dumps(output)
             if kwargs.get("skip_quote") is True:
                 output = str(output)
@@ -887,29 +888,36 @@
 
         :param list attr: Object to be serialized.
         :param str iter_type: Type of object in the iterable.
         :param bool required: Whether the objects in the iterable must
          not be None or empty.
         :param str div: If set, this str will be used to combine the elements
          in the iterable into a combined string. Default is 'None'.
+        :keyword bool do_quote: Whether to quote the serialized result of each iterable element.
+        Defaults to False.
         :rtype: list, str
         """
         if isinstance(data, str):
             raise SerializationError("Refuse str type as a valid iter type.")
 
         serialization_ctxt = kwargs.get("serialization_ctxt", {})
         is_xml = kwargs.get("is_xml", False)
 
         serialized = []
         for d in data:
             try:
                 serialized.append(self.serialize_data(d, iter_type, **kwargs))
-            except ValueError:
+            except ValueError as err:
+                if isinstance(err, SerializationError):
+                    raise
                 serialized.append(None)
 
+        if kwargs.get("do_quote", False):
+            serialized = ["" if s is None else quote(str(s), safe="") for s in serialized]
+
         if div:
             serialized = ["" if s is None else str(s) for s in serialized]
             serialized = div.join(serialized)
 
         if "xml" in serialization_ctxt or is_xml:
             # XML serialization is more complicated
             xml_desc = serialization_ctxt.get("xml", {})
@@ -946,15 +954,17 @@
         :rtype: dict
         """
         serialization_ctxt = kwargs.get("serialization_ctxt", {})
         serialized = {}
         for key, value in attr.items():
             try:
                 serialized[self.serialize_unicode(key)] = self.serialize_data(value, dict_type, **kwargs)
-            except ValueError:
+            except ValueError as err:
+                if isinstance(err, SerializationError):
+                    raise
                 serialized[self.serialize_unicode(key)] = None
 
         if "xml" in serialization_ctxt:
             # XML serialization is more complicated
             xml_desc = serialization_ctxt["xml"]
             xml_name = xml_desc["name"]
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/_generated/_configuration.py` & `azure-search-documents-11.4.0b7/azure/search/documents/_generated/_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/_generated/__init__.py` & `azure-search-documents-11.4.0b7/azure/search/documents/_generated/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._search_index_client import SearchIndexClient
 
 try:
     from ._patch import __all__ as _patch_all
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/_generated/models/_patch.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/_generated/models/_search_index_client_enums.py` & `azure-search-documents-11.4.0b7/azure/search/documents/_generated/models/_search_index_client_enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from enum import Enum
 from azure.core import CaseInsensitiveEnumMeta
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/_generated/models/__init__.py` & `azure-search-documents-11.4.0b7/azure/search/documents/_generated/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._models_py3 import AnswerResult
 from ._models_py3 import AutocompleteItem
 from ._models_py3 import AutocompleteOptions
 from ._models_py3 import AutocompleteRequest
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/_generated/models/_models_py3.py` & `azure-search-documents-11.4.0b7/azure/search/documents/_generated/models/_models_py3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding=utf-8
 # pylint: disable=too-many-lines
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any, Dict, List, Optional, TYPE_CHECKING, Union
 
 from .. import _serialization
 
@@ -1229,14 +1229,16 @@
     :ivar captions: A value that specifies whether captions should be returned as part of the
      search response. Known values are: "none" and "extractive".
     :vartype captions: str or ~search_index_client.models.QueryCaptionType
     :ivar semantic_fields: The comma-separated list of field names used for semantic search.
     :vartype semantic_fields: str
     :ivar vector: The query parameters for vector and hybrid search queries.
     :vartype vector: ~search_index_client.models.Vector
+    :ivar vectors: The query parameters for multi-vector search queries.
+    :vartype vectors: list[~search_index_client.models.Vector]
     """
 
     _validation = {
         "semantic_max_wait_in_milliseconds": {"minimum": 700},
     }
 
     _attribute_map = {
@@ -1265,14 +1267,15 @@
         "answers": {"key": "answers", "type": "str"},
         "select": {"key": "select", "type": "str"},
         "skip": {"key": "skip", "type": "int"},
         "top": {"key": "top", "type": "int"},
         "captions": {"key": "captions", "type": "str"},
         "semantic_fields": {"key": "semanticFields", "type": "str"},
         "vector": {"key": "vector", "type": "Vector"},
+        "vectors": {"key": "vectors", "type": "[Vector]"},
     }
 
     def __init__(  # pylint: disable=too-many-locals
         self,
         *,
         include_total_result_count: Optional[bool] = None,
         facets: Optional[List[str]] = None,
@@ -1299,14 +1302,15 @@
         answers: Optional[Union[str, "_models.QueryAnswerType"]] = None,
         select: Optional[str] = None,
         skip: Optional[int] = None,
         top: Optional[int] = None,
         captions: Optional[Union[str, "_models.QueryCaptionType"]] = None,
         semantic_fields: Optional[str] = None,
         vector: Optional["_models.Vector"] = None,
+        vectors: Optional[List["_models.Vector"]] = None,
         **kwargs: Any
     ) -> None:
         """
         :keyword include_total_result_count: A value that specifies whether to fetch the total count of
          results. Default is false. Setting this value to true may have a performance impact. Note that
          the count returned is an approximation.
         :paramtype include_total_result_count: bool
@@ -1417,14 +1421,16 @@
         :keyword captions: A value that specifies whether captions should be returned as part of the
          search response. Known values are: "none" and "extractive".
         :paramtype captions: str or ~search_index_client.models.QueryCaptionType
         :keyword semantic_fields: The comma-separated list of field names used for semantic search.
         :paramtype semantic_fields: str
         :keyword vector: The query parameters for vector and hybrid search queries.
         :paramtype vector: ~search_index_client.models.Vector
+        :keyword vectors: The query parameters for multi-vector search queries.
+        :paramtype vectors: list[~search_index_client.models.Vector]
         """
         super().__init__(**kwargs)
         self.include_total_result_count = include_total_result_count
         self.facets = facets
         self.filter = filter
         self.highlight_fields = highlight_fields
         self.highlight_post_tag = highlight_post_tag
@@ -1448,14 +1454,15 @@
         self.answers = answers
         self.select = select
         self.skip = skip
         self.top = top
         self.captions = captions
         self.semantic_fields = semantic_fields
         self.vector = vector
+        self.vectors = vectors
 
 
 class SearchResult(_serialization.Model):
     """Contains a document found by a search query, plus associated metadata.
 
     Variables are only populated by the server, and will be ignored when sending a request.
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/_generated/aio/_search_index_client.py` & `azure-search-documents-11.4.0b7/azure/search/documents/_generated/aio/_search_index_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
 from typing import Any, Awaitable
 
 from azure.core import AsyncPipelineClient
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/_generated/aio/_patch.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/_generated/aio/_configuration.py` & `azure-search-documents-11.4.0b7/azure/search/documents/_generated/aio/_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/_generated/aio/__init__.py` & `azure-search-documents-11.4.0b7/azure/search/documents/_generated/aio/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._search_index_client import SearchIndexClient
 
 try:
     from ._patch import __all__ as _patch_all
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/_generated/aio/operations/_patch.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/_generated/aio/operations/_documents_operations.py` & `azure-search-documents-11.4.0b7/azure/search/documents/_generated/aio/operations/_documents_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # pylint: disable=too-many-lines
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-import sys
 from typing import Any, Callable, Dict, IO, List, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -32,19 +31,14 @@
     build_index_request,
     build_search_get_request,
     build_search_post_request,
     build_suggest_get_request,
     build_suggest_post_request,
 )
 
-if sys.version_info >= (3, 9):
-    from collections.abc import MutableMapping
-else:
-    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
-JSON = MutableMapping[str, Any]  # pylint: disable=unsubscriptable-object
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
 class DocumentsOperations:
     """
     .. warning::
@@ -438,45 +432,45 @@
     @distributed_trace_async
     async def get(
         self,
         key: str,
         selected_fields: Optional[List[str]] = None,
         request_options: Optional[_models.RequestOptions] = None,
         **kwargs: Any
-    ) -> JSON:
+    ) -> Dict[str, Any]:
         """Retrieves a document from the index.
 
         .. seealso::
            - https://docs.microsoft.com/rest/api/searchservice/lookup-document
 
         :param key: The key of the document to retrieve. Required.
         :type key: str
         :param selected_fields: List of field names to retrieve for the document; Any field not
          retrieved will be missing from the returned document. Default value is None.
         :type selected_fields: list[str]
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~search_index_client.models.RequestOptions
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: JSON or the result of cls(response)
-        :rtype: JSON
+        :return: dict mapping str to any or the result of cls(response)
+        :rtype: dict[str, any]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[JSON] = kwargs.pop("cls", None)
+        cls: ClsType[Dict[str, Any]] = kwargs.pop("cls", None)
 
         _x_ms_client_request_id = None
         if request_options is not None:
             _x_ms_client_request_id = request_options.x_ms_client_request_id
 
         request = build_get_request(
             key=key,
@@ -502,15 +496,15 @@
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.SearchError, pipeline_response)
             raise HttpResponseError(response=response, model=error)
 
-        deserialized = self._deserialize("object", pipeline_response)
+        deserialized = self._deserialize("{object}", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
     get.metadata = {"url": "/docs('{key}')"}
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/_generated/aio/operations/__init__.py` & `azure-search-documents-11.4.0b7/azure/search/documents/_generated/operations/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._documents_operations import DocumentsOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/_generated/operations/_patch.py` & `azure-search-documents-11.4.0b7/azure/search/documents/indexes/_generated/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/_generated/operations/_documents_operations.py` & `azure-search-documents-11.4.0b7/azure/search/documents/_generated/operations/_documents_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # pylint: disable=too-many-lines
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 from io import IOBase
-import sys
 from typing import Any, Callable, Dict, IO, List, Optional, TypeVar, Union, overload
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -20,21 +19,16 @@
 from azure.core.pipeline.transport import HttpResponse
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 
 from .. import models as _models
 from .._serialization import Serializer
-from .._vendor import _convert_request, _format_url_section
+from .._vendor import _convert_request
 
-if sys.version_info >= (3, 9):
-    from collections.abc import MutableMapping
-else:
-    from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
-JSON = MutableMapping[str, Any]  # pylint: disable=unsubscriptable-object
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
@@ -211,15 +205,15 @@
 
     # Construct URL
     _url = kwargs.pop("template_url", "/docs('{key}')")
     path_format_arguments = {
         "key": _SERIALIZER.url("key", key, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct parameters
     if selected_fields is not None:
         _params["$select"] = _SERIALIZER.query("selected_fields", selected_fields, "[str]", div=",")
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
@@ -804,45 +798,45 @@
     @distributed_trace
     def get(
         self,
         key: str,
         selected_fields: Optional[List[str]] = None,
         request_options: Optional[_models.RequestOptions] = None,
         **kwargs: Any
-    ) -> JSON:
+    ) -> Dict[str, Any]:
         """Retrieves a document from the index.
 
         .. seealso::
            - https://docs.microsoft.com/rest/api/searchservice/lookup-document
 
         :param key: The key of the document to retrieve. Required.
         :type key: str
         :param selected_fields: List of field names to retrieve for the document; Any field not
          retrieved will be missing from the returned document. Default value is None.
         :type selected_fields: list[str]
         :param request_options: Parameter group. Default value is None.
         :type request_options: ~search_index_client.models.RequestOptions
         :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: JSON or the result of cls(response)
-        :rtype: JSON
+        :return: dict mapping str to any or the result of cls(response)
+        :rtype: dict[str, any]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[JSON] = kwargs.pop("cls", None)
+        cls: ClsType[Dict[str, Any]] = kwargs.pop("cls", None)
 
         _x_ms_client_request_id = None
         if request_options is not None:
             _x_ms_client_request_id = request_options.x_ms_client_request_id
 
         request = build_get_request(
             key=key,
@@ -868,15 +862,15 @@
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.SearchError, pipeline_response)
             raise HttpResponseError(response=response, model=error)
 
-        deserialized = self._deserialize("object", pipeline_response)
+        deserialized = self._deserialize("{object}", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})
 
         return deserialized
 
     get.metadata = {"url": "/docs('{key}')"}
```

## Comparing `azure-search-documents-11.4.0b6/azure/search/documents/_generated/operations/__init__.py` & `azure-search-documents-11.4.0b7/azure/search/documents/_generated/aio/operations/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.5, generator: @autorest/python@6.4.11)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.7.1)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._documents_operations import DocumentsOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
```

## Comparing `azure-search-documents-11.4.0b6/samples/sample_data_source_operations.py` & `azure-search-documents-11.4.0b7/samples/sample_data_source_operations.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/samples/sample_authentication.py` & `azure-search-documents-11.4.0b7/samples/sample_authentication.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,25 +34,56 @@
     key = os.getenv("AZURE_SEARCH_API_KEY")
 
     search_client = SearchClient(service_endpoint, index_name, AzureKeyCredential(key))
     # [END create_search_client_with_key]
 
     result = search_client.get_document_count()
 
-    print("There are {} documents in the {} search index.".format(result, repr(index_name)))
+    print("There are {} documents in the {} search index.".format(result, index_name))
 
 
 def authentication_service_client_with_api_key_credential():
     # [START create_search_service_client_with_key]
     from azure.core.credentials import AzureKeyCredential
     from azure.search.documents.indexes import SearchIndexClient
 
     service_endpoint = os.getenv("AZURE_SEARCH_SERVICE_ENDPOINT")
     key = os.getenv("AZURE_SEARCH_API_KEY")
 
     search_client = SearchIndexClient(service_endpoint, AzureKeyCredential(key))
     # [END create_search_service_client_with_key]
 
 
+def authentication_with_aad():
+    # [START authentication_with_aad]
+    from azure.identity import DefaultAzureCredential
+    from azure.search.documents import SearchClient
+
+    service_endpoint = os.getenv("AZURE_SEARCH_SERVICE_ENDPOINT")
+    index_name = os.getenv("AZURE_SEARCH_INDEX_NAME")
+    credential = DefaultAzureCredential()
+
+    search_client = SearchClient(service_endpoint, index_name, credential)
+    # [END authentication_with_aad]
+
+    result = search_client.get_document_count()
+
+    print("There are {} documents in the {} search index.".format(result, index_name))
+
+
+def authentication_service_client_with_aad():
+    # [START authentication_service_client_with_aad]
+    from azure.identity import DefaultAzureCredential
+    from azure.search.documents.indexes import SearchIndexClient
+
+    service_endpoint = os.getenv("AZURE_SEARCH_SERVICE_ENDPOINT")
+    credential = DefaultAzureCredential()
+
+    search_client = SearchIndexClient(service_endpoint, credential)
+    # [END authentication_service_client_with_aad]
+
+
 if __name__ == "__main__":
     authentication_with_api_key_credential()
     authentication_service_client_with_api_key_credential()
+    authentication_with_aad()
+    authentication_service_client_with_aad()
```

## Comparing `azure-search-documents-11.4.0b6/samples/sample_indexers_operations.py` & `azure-search-documents-11.4.0b7/samples/sample_indexers_operations.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/samples/sample_synonym_map_operations.py` & `azure-search-documents-11.4.0b7/samples/sample_synonym_map_operations.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/samples/sample_buffered_sender.py` & `azure-search-documents-11.4.0b7/samples/sample_buffered_sender.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,25 +27,25 @@
 
 from azure.core.credentials import AzureKeyCredential
 from azure.search.documents import SearchIndexingBufferedSender
 
 
 def sample_batching_client():
     DOCUMENT = {
-        "Category": "Hotel",
-        "HotelId": "1000",
-        "Rating": 4.0,
-        "Rooms": [],
-        "HotelName": "Azure Inn",
+        "category": "Hotel",
+        "hotelId": "1000",
+        "rating": 4.0,
+        "rooms": [],
+        "hotelName": "Azure Inn",
     }
 
     with SearchIndexingBufferedSender(service_endpoint, index_name, AzureKeyCredential(key)) as batch_client:
         # add upload actions
         batch_client.upload_documents(documents=[DOCUMENT])
         # add merge actions
-        batch_client.merge_documents(documents=[{"HotelId": "1000", "Rating": 4.5}])
+        batch_client.merge_documents(documents=[{"hotelId": "1000", "rating": 4.5}])
         # add delete actions
-        batch_client.delete_documents(documents=[{"HotelId": "1000"}])
+        batch_client.delete_documents(documents=[{"hotelId": "1000"}])
 
 
 if __name__ == "__main__":
     sample_batching_client()
```

## Comparing `azure-search-documents-11.4.0b6/samples/sample_get_document.py` & `azure-search-documents-11.4.0b7/samples/sample_get_document.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     from azure.search.documents import SearchClient
 
     search_client = SearchClient(service_endpoint, index_name, AzureKeyCredential(key))
 
     result = search_client.get_document(key="23")
 
     print("Details for hotel '23' are:")
-    print("        Name: {}".format(result["HotelName"]))
-    print("      Rating: {}".format(result["Rating"]))
-    print("    Category: {}".format(result["Category"]))
+    print("        Name: {}".format(result["hotelName"]))
+    print("      Rating: {}".format(result["rating"]))
+    print("    Category: {}".format(result["category"]))
     # [END get_document]
 
 
 if __name__ == "__main__":
     get_document()
```

## Comparing `azure-search-documents-11.4.0b6/samples/sample_analyze_text.py` & `azure-search-documents-11.4.0b7/samples/sample_analyze_text.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/samples/README.md` & `azure-search-documents-11.4.0b7/samples/README.md`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/samples/sample_semantic_search.py` & `azure-search-documents-11.4.0b7/samples/sample_semantic_search.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     api_key = os.getenv("AZURE_SEARCH_API_KEY")
 
     credential = AzureKeyCredential(api_key)
     client = SearchClient(endpoint=endpoint, index_name=index_name, credential=credential)
     results = list(client.search(search_text="luxury", query_language="en-us", query_speller="lexicon"))
 
     for result in results:
-        print("{}\n{}\n)".format(result["HotelId"], result["HotelName"]))
+        print("{}\n{}\n)".format(result["hotelId"], result["hotelName"]))
     # [END speller]
 
 
 def semantic_ranking():
     # [START semantic_ranking]
     from azure.core.credentials import AzureKeyCredential
     from azure.search.documents import SearchClient
@@ -57,14 +57,14 @@
             query_type="semantic",
             semantic_configuration_name="semantic_config_name",
             query_language="en-us",
         )
     )
 
     for result in results:
-        print("{}\n{}\n)".format(result["HotelId"], result["HotelName"]))
+        print("{}\n{}\n)".format(result["hotelId"], result["hotelName"]))
     # [END semantic_ranking]
 
 
 if __name__ == "__main__":
     speller()
     semantic_ranking()
```

## Comparing `azure-search-documents-11.4.0b6/samples/sample_index_alias_crud_operations.py` & `azure-search-documents-11.4.0b7/samples/sample_index_alias_crud_operations.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/samples/sample_filter_query.py` & `azure-search-documents-11.4.0b7/samples/sample_filter_query.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,23 +30,23 @@
 def filter_query():
     # [START filter_query]
     from azure.core.credentials import AzureKeyCredential
     from azure.search.documents import SearchClient
 
     search_client = SearchClient(service_endpoint, index_name, AzureKeyCredential(key))
 
-    select = ("HotelName", "Rating")
+    select = ("hotelName", "rating")
     results = search_client.search(
         search_text="WiFi",
         filter="Address/StateProvince eq 'FL' and Address/Country eq 'USA'",
         select=",".join(select),
-        order_by="Rating desc",
+        order_by="rating desc",
     )
 
     print("Florida hotels containing 'WiFi', sorted by Rating:")
     for result in results:
-        print("    Name: {} (rating {})".format(result["HotelName"], result["Rating"]))
+        print("    Name: {} (rating {})".format(result["hotelName"], result["rating"]))
     # [END filter_query]
 
 
 if __name__ == "__main__":
     filter_query()
```

## Comparing `azure-search-documents-11.4.0b6/samples/sample_index_crud_operations.py` & `azure-search-documents-11.4.0b7/samples/sample_index_crud_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,19 +32,18 @@
     SearchIndex,
     ScoringProfile,
     SearchFieldDataType,
     SimpleField,
     SearchableField,
 )
 
-client = SearchIndexClient(service_endpoint, AzureKeyCredential(key))
-
 
 def create_index():
     # [START create_index]
+    client = SearchIndexClient(service_endpoint, AzureKeyCredential(key))
     name = "hotels"
     fields = [
         SimpleField(name="hotelId", type=SearchFieldDataType.String, key=True),
         SimpleField(name="baseRate", type=SearchFieldDataType.Double),
         SearchableField(name="description", type=SearchFieldDataType.String, collection=True),
         ComplexField(
             name="address",
@@ -61,21 +60,23 @@
 
     result = client.create_index(index)
     # [END create_index]
 
 
 def get_index():
     # [START get_index]
+    client = SearchIndexClient(service_endpoint, AzureKeyCredential(key))
     name = "hotels"
     result = client.get_index(name)
     # [END get_index]
 
 
 def update_index():
     # [START update_index]
+    client = SearchIndexClient(service_endpoint, AzureKeyCredential(key))
     name = "hotels"
     fields = [
         SimpleField(name="hotelId", type=SearchFieldDataType.String, key=True),
         SimpleField(name="baseRate", type=SearchFieldDataType.Double),
         SearchableField(name="description", type=SearchFieldDataType.String, collection=True),
         SearchableField(name="hotelName", type=SearchFieldDataType.String),
         ComplexField(
@@ -96,14 +97,15 @@
 
     result = client.create_or_update_index(index=index)
     # [END update_index]
 
 
 def delete_index():
     # [START delete_index]
+    client = SearchIndexClient(service_endpoint, AzureKeyCredential(key))
     name = "hotels"
     client.delete_index(name)
     # [END delete_index]
 
 
 if __name__ == "__main__":
     create_index()
```

## Comparing `azure-search-documents-11.4.0b6/samples/sample_autocomplete.py` & `azure-search-documents-11.4.0b7/samples/sample_autocomplete.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/samples/sample_indexer_datasource_skillset.py` & `azure-search-documents-11.4.0b7/samples/sample_indexer_datasource_skillset.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/samples/sample_simple_query.py` & `azure-search-documents-11.4.0b7/samples/sample_simple_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,13 +34,13 @@
 
     search_client = SearchClient(service_endpoint, index_name, AzureKeyCredential(key))
 
     results = search_client.search(search_text="spa")
 
     print("Hotels containing 'spa' in the name (or other fields):")
     for result in results:
-        print("    Name: {} (rating {})".format(result["HotelName"], result["Rating"]))
+        print("    Name: {} (rating {})".format(result["hotelName"], result["rating"]))
     # [END simple_query]
 
 
 if __name__ == "__main__":
     simple_text_query()
```

## Comparing `azure-search-documents-11.4.0b6/samples/sample_facet_query.py` & `azure-search-documents-11.4.0b7/samples/sample_facet_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 def filter_query():
     # [START facet_query]
     from azure.core.credentials import AzureKeyCredential
     from azure.search.documents import SearchClient
 
     search_client = SearchClient(service_endpoint, index_name, AzureKeyCredential(key))
 
-    results = search_client.search(search_text="WiFi", facets=["Category,count:3", "ParkingIncluded"])
+    results = search_client.search(search_text="WiFi", facets=["category,count:3", "parkingIncluded"])
 
     facets = results.get_facets()
 
     print("Catgory facet counts for hotels:")
-    for facet in facets["Category"]:
+    for facet in facets["category"]:
         print("    {}".format(facet))
     # [END facet_query]
 
 
 if __name__ == "__main__":
     filter_query()
```

## Comparing `azure-search-documents-11.4.0b6/samples/sample_vector_search.py` & `azure-search-documents-11.4.0b7/samples/sample_vector_search.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,23 +21,25 @@
 """
 
 import os
 
 from azure.core.credentials import AzureKeyCredential
 from azure.search.documents import SearchClient
 from azure.search.documents.indexes import SearchIndexClient
+from azure.search.documents.models import Vector
 
 service_endpoint = os.getenv("AZURE_SEARCH_SERVICE_ENDPOINT")
 index_name = os.getenv("AZURE_SEARCH_INDEX_NAME")
 key = os.getenv("AZURE_SEARCH_API_KEY")
 
 
 def get_embeddings(text: str):
     # There are a few ways to get embeddings. This is just one example.
     import openai
+
     open_ai_endpoint = os.getenv("OpenAIEndpoint")
     open_ai_key = os.getenv("OpenAIKey")
 
     openai.api_version = "2022-12-01"
     openai.api_base = open_ai_endpoint
     openai.api_type = "azure"
     openai.api_key = open_ai_key
@@ -80,103 +82,100 @@
 
 def get_hotel_documents():
     docs = [
         {
             "hotelId": "1",
             "hotelName": "Fancy Stay",
             "description": "Best hotel in town if you like luxury hotels.",
-            "DescriptionVector": get_embeddings("Best hotel in town if you like luxury hotels."),
+            "descriptionVector": get_embeddings("Best hotel in town if you like luxury hotels."),
             "category": "Luxury",
         },
         {
-            "HotelId": "2",
-            "HotelName": "Roach Motel",
-            "Description": "Cheapest hotel in town. Infact, a motel.",
-            "DescriptionVector": get_embeddings("Cheapest hotel in town. Infact, a motel."),
-            "Category": "Budget",
+            "hotelId": "2",
+            "hotelName": "Roach Motel",
+            "description": "Cheapest hotel in town. Infact, a motel.",
+            "descriptionVector": get_embeddings("Cheapest hotel in town. Infact, a motel."),
+            "category": "Budget",
         },
         {
-            "HotelId": "3",
-            "HotelName": "EconoStay",
-            "Description": "Very popular hotel in town.",
-            "DescriptionVector": get_embeddings("Very popular hotel in town."),
-            "Category": "Budget",
+            "hotelId": "3",
+            "hotelName": "EconoStay",
+            "description": "Very popular hotel in town.",
+            "descriptionVector": get_embeddings("Very popular hotel in town."),
+            "category": "Budget",
         },
         {
-            "HotelId": "4",
-            "HotelName": "Modern Stay",
-            "Description": "Modern architecture, very polite staff and very clean. Also very affordable.",
-            "DescriptionVector": get_embeddings(
+            "hotelId": "4",
+            "hotelName": "Modern Stay",
+            "description": "Modern architecture, very polite staff and very clean. Also very affordable.",
+            "descriptionVector": get_embeddings(
                 "Modern architecture, very polite staff and very clean. Also very affordable."
             ),
-            "Category": "Luxury",
+            "category": "Luxury",
         },
         {
-            "HotelId": "5",
-            "HotelName": "Secret Point",
-            "Description": "One of the best hotel in town. The hotel is ideally located on the main commercial artery of the city in the heart of New York.",
-            "DescriptionVector": get_embeddings(
+            "hotelId": "5",
+            "hotelName": "Secret Point",
+            "description": "One of the best hotel in town. The hotel is ideally located on the main commercial artery of the city in the heart of New York.",
+            "descriptionVector": get_embeddings(
                 "One of the best hotel in town. The hotel is ideally located on the main commercial artery of the city in the heart of New York."
             ),
-            "Category": "Boutique",
+            "category": "Boutique",
         },
     ]
     return docs
 
 
 def single_vector_search():
     # [START single_vector_search]
     query = "Top hotels in town"
 
     search_client = SearchClient(service_endpoint, index_name, AzureKeyCredential(key))
+    vector = Vector(value=get_embeddings(query), k=3, fields="descriptionVector")
 
     results = search_client.search(
         search_text="",
-        vector=get_embeddings(query),
-        top_k=3,
-        vector_fields="descriptionVector",
+        vectors=[vector],
         select=["hotelId", "hotelName"],
     )
 
     for result in results:
         print(result)
     # [END single_vector_search]
 
 
 def single_vector_search_with_filter():
     # [START single_vector_search_with_filter]
     query = "Top hotels in town"
 
     search_client = SearchClient(service_endpoint, index_name, AzureKeyCredential(key))
+    vector = Vector(value=get_embeddings(query), k=3, fields="descriptionVector")
 
     results = search_client.search(
         search_text="",
-        vector=get_embeddings(query),
-        top_k=3,
-        vector_fields="descriptionVector",
+        vectors=[vector],
         filter="category eq 'Luxury'",
         select=["hotelId", "hotelName"],
     )
 
     for result in results:
         print(result)
     # [END single_vector_search_with_filter]
 
 
 def simple_hybrid_search():
     # [START simple_hybrid_search]
     query = "Top hotels in town"
 
     search_client = SearchClient(service_endpoint, index_name, AzureKeyCredential(key))
+    vector = Vector(value=get_embeddings(query), k=3, fields="descriptionVector")
 
     results = search_client.search(
         search_text=query,
-        vector=get_embeddings(query),
-        top_k=3,
-        vector_fields="descriptionVector",
+        vectors=[vector],
         select=["hotelId", "hotelName"],
     )
     print(results.get_answers())
     for result in results:
         print(result)
     # [END simple_hybrid_search]
 
@@ -185,11 +184,11 @@
     credential = AzureKeyCredential(key)
     index_client = SearchIndexClient(service_endpoint, credential)
     index = get_hotel_index(index_name)
     index_client.create_index(index)
     client = SearchClient(service_endpoint, index_name, credential)
     hotel_docs = get_hotel_documents()
     client.upload_documents(documents=hotel_docs)
-    
+
     single_vector_search()
     single_vector_search_with_filter()
     simple_hybrid_search()
```

## Comparing `azure-search-documents-11.4.0b6/samples/sample_suggestions.py` & `azure-search-documents-11.4.0b7/samples/sample_suggestions.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,14 @@
 
     search_client = SearchClient(service_endpoint, index_name, AzureKeyCredential(key))
 
     results = search_client.suggest(search_text="coffee", suggester_name="sg")
 
     print("Search suggestions for 'coffee'")
     for result in results:
-        hotel = search_client.get_document(key=result["HotelId"])
-        print("    Text: {} for Hotel: {}".format(repr(result["text"]), hotel["HotelName"]))
+        hotel = search_client.get_document(key=result["hotelId"])
+        print("    Text: {} for Hotel: {}".format(repr(result["text"]), hotel["hotelName"]))
     # [END suggest_query]
 
 
 if __name__ == "__main__":
     suggest_query()
```

## Comparing `azure-search-documents-11.4.0b6/samples/sample_crud_operations.py` & `azure-search-documents-11.4.0b7/samples/sample_crud_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,38 +31,38 @@
 
 search_client = SearchClient(service_endpoint, index_name, AzureKeyCredential(key))
 
 
 def upload_document():
     # [START upload_document]
     DOCUMENT = {
-        "Category": "Hotel",
-        "HotelId": "1000",
-        "Rating": 4.0,
-        "Rooms": [],
-        "HotelName": "Azure Inn",
+        "category": "Hotel",
+        "hotelId": "1000",
+        "rating": 4.0,
+        "rooms": [],
+        "hotelName": "Azure Inn",
     }
 
     result = search_client.upload_documents(documents=[DOCUMENT])
 
     print("Upload of new document succeeded: {}".format(result[0].succeeded))
     # [END upload_document]
 
 
 def merge_document():
     # [START merge_document]
-    result = search_client.merge_documents(documents=[{"HotelId": "1000", "Rating": 4.5}])
+    result = search_client.merge_documents(documents=[{"hotelId": "1000", "rating": 4.5}])
 
     print("Merge into new document succeeded: {}".format(result[0].succeeded))
     # [END merge_document]
 
 
 def delete_document():
     # [START delete_document]
-    result = search_client.delete_documents(documents=[{"HotelId": "1000"}])
+    result = search_client.delete_documents(documents=[{"hotelId": "1000"}])
 
     print("Delete new document succeeded: {}".format(result[0].succeeded))
     # [END delete_document]
 
 
 if __name__ == "__main__":
     upload_document()
```

## Comparing `azure-search-documents-11.4.0b6/samples/async_samples/sample_semantic_search_async.py` & `azure-search-documents-11.4.0b7/samples/async_samples/sample_semantic_search_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     api_key = os.getenv("AZURE_SEARCH_API_KEY")
 
     credential = AzureKeyCredential(api_key)
     client = SearchClient(endpoint=endpoint, index_name=index_name, credential=credential)
     results = await client.search(search_text="luxury", query_language="en-us", query_speller="lexicon")
 
     async for result in results:
-        print("{}\n{}\n)".format(result["HotelId"], result["HotelName"]))
+        print("{}\n{}\n)".format(result["hotelId"], result["hotelName"]))
     # [END speller_async]
 
 
 async def semantic_ranking():
     # [START semantic_ranking_async]
     from azure.core.credentials import AzureKeyCredential
     from azure.search.documents import SearchClient
@@ -51,14 +51,14 @@
     api_key = os.getenv("AZURE_SEARCH_API_KEY")
 
     credential = AzureKeyCredential(api_key)
     client = SearchClient(endpoint=endpoint, index_name=index_name, credential=credential)
     results = list(client.search(search_text="luxury", query_type="semantic", query_language="en-us"))
 
     for result in results:
-        print("{}\n{}\n)".format(result["HotelId"], result["HotelName"]))
+        print("{}\n{}\n)".format(result["hotelId"], result["hotelName"]))
     # [END semantic_ranking_async]
 
 
 if __name__ == "__main__":
     asyncio.run(speller())
     asyncio.run(semantic_ranking())
```

## Comparing `azure-search-documents-11.4.0b6/samples/async_samples/sample_crud_operations_async.py` & `azure-search-documents-11.4.0b7/samples/async_samples/sample_crud_operations_async.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,38 +32,38 @@
 
 search_client = SearchClient(service_endpoint, index_name, AzureKeyCredential(key))
 
 
 async def upload_document():
     # [START upload_document_async]
     DOCUMENT = {
-        "Category": "Hotel",
-        "HotelId": "1000",
-        "Rating": 4.0,
-        "Rooms": [],
-        "HotelName": "Azure Inn",
+        "category": "Hotel",
+        "hotelId": "1000",
+        "rating": 4.0,
+        "rooms": [],
+        "hotelName": "Azure Inn",
     }
 
     result = await search_client.upload_documents(documents=[DOCUMENT])
 
     print("Upload of new document succeeded: {}".format(result[0].succeeded))
     # [END upload_document_async]
 
 
 async def merge_document():
     # [START merge_document_async]
-    result = await search_client.upload_documents(documents=[{"HotelId": "1000", "Rating": 4.5}])
+    result = await search_client.upload_documents(documents=[{"hotelId": "1000", "rating": 4.5}])
 
     print("Merge into new document succeeded: {}".format(result[0].succeeded))
     # [END merge_document_async]
 
 
 async def delete_document():
     # [START delete_document_async]
-    result = await search_client.upload_documents(documents=[{"HotelId": "1000"}])
+    result = await search_client.upload_documents(documents=[{"hotelId": "1000"}])
 
     print("Delete new document succeeded: {}".format(result[0].succeeded))
     # [END delete_document_async]
 
 
 async def main():
     await upload_document()
```

## Comparing `azure-search-documents-11.4.0b6/samples/async_samples/sample_indexers_operations_async.py` & `azure-search-documents-11.4.0b7/samples/async_samples/sample_indexers_operations_async.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/samples/async_samples/sample_facet_query_async.py` & `azure-search-documents-11.4.0b7/samples/async_samples/sample_facet_query_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,19 +33,19 @@
     # [START facet_query_async]
     from azure.core.credentials import AzureKeyCredential
     from azure.search.documents.aio import SearchClient
 
     search_client = SearchClient(service_endpoint, index_name, AzureKeyCredential(key))
 
     async with search_client:
-        results = await search_client.search(search_text="WiFi", facets=["Category,count:3", "ParkingIncluded"])
+        results = await search_client.search(search_text="WiFi", facets=["category,count:3", "parkingIncluded"])
 
         facets = await results.get_facets()
 
         print("Catgory facet counts for hotels:")
-        for facet in facets["Category"]:
+        for facet in facets["category"]:
             print("    {}".format(facet))
     # [END facet_query_async]
 
 
 if __name__ == "__main__":
     asyncio.run(filter_query())
```

## Comparing `azure-search-documents-11.4.0b6/samples/async_samples/sample_analyze_text_async.py` & `azure-search-documents-11.4.0b7/samples/async_samples/sample_analyze_text_async.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/samples/async_samples/sample_index_alias_crud_operations_async.py` & `azure-search-documents-11.4.0b7/samples/async_samples/sample_index_alias_crud_operations_async.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/samples/async_samples/sample_suggestions_async.py` & `azure-search-documents-11.4.0b7/samples/async_samples/sample_suggestions_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,14 @@
     search_client = SearchClient(service_endpoint, index_name, AzureKeyCredential(key))
 
     async with search_client:
         results = await search_client.suggest(search_text="coffee", suggester_name="sg")
 
         print("Search suggestions for 'coffee'")
         for result in results:
-            hotel = await search_client.get_document(key=result["HotelId"])
-            print("    Text: {} for Hotel: {}".format(repr(result["text"]), hotel["HotelName"]))
+            hotel = await search_client.get_document(key=result["hotelId"])
+            print("    Text: {} for Hotel: {}".format(repr(result["text"]), hotel["hotelName"]))
     # [END suggest_query_async]
 
 
 if __name__ == "__main__":
     asyncio.run(suggest_query())
```

## Comparing `azure-search-documents-11.4.0b6/samples/async_samples/sample_simple_query_async.py` & `azure-search-documents-11.4.0b7/samples/async_samples/sample_simple_query_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,13 +37,13 @@
     search_client = SearchClient(service_endpoint, index_name, AzureKeyCredential(key))
 
     async with search_client:
         results = await search_client.search(search_text="spa")
 
         print("Hotels containing 'spa' in the name (or other fields):")
         async for result in results:
-            print("    Name: {} (rating {})".format(result["HotelName"], result["Rating"]))
+            print("    Name: {} (rating {})".format(result["hotelName"], result["rating"]))
     # [END simple_query_async]
 
 
 if __name__ == "__main__":
     asyncio.run(simple_text_query())
```

## Comparing `azure-search-documents-11.4.0b6/samples/async_samples/sample_buffered_sender_async.py` & `azure-search-documents-11.4.0b7/samples/async_samples/sample_buffered_sender_async.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,28 +28,28 @@
 
 from azure.core.credentials import AzureKeyCredential
 from azure.search.documents.aio import SearchIndexingBufferedSender
 
 
 async def sample_batching_client():
     DOCUMENT = {
-        "Category": "Hotel",
-        "HotelId": "1000",
-        "Rating": 4.0,
-        "Rooms": [],
-        "HotelName": "Azure Inn",
+        "category": "Hotel",
+        "hotelId": "1000",
+        "rating": 4.0,
+        "rooms": [],
+        "hotelName": "Azure Inn",
     }
 
     async with SearchIndexingBufferedSender(service_endpoint, index_name, AzureKeyCredential(key)) as batch_client:
         # add upload actions
         await batch_client.upload_documents(documents=[DOCUMENT])
         # add merge actions
-        await batch_client.merge_documents(documents=[{"HotelId": "1000", "Rating": 4.5}])
+        await batch_client.merge_documents(documents=[{"hotelId": "1000", "rating": 4.5}])
         # add delete actions
-        await batch_client.delete_documents(documents=[{"HotelId": "1000"}])
+        await batch_client.delete_documents(documents=[{"hotelId": "1000"}])
 
 
 async def main():
     await sample_batching_client()
 
 
 if __name__ == "__main__":
```

## Comparing `azure-search-documents-11.4.0b6/samples/async_samples/sample_index_crud_operations_async.py` & `azure-search-documents-11.4.0b7/samples/async_samples/sample_index_crud_operations_async.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,19 +33,18 @@
     SearchIndex,
     ScoringProfile,
     SearchFieldDataType,
     SimpleField,
     SearchableField,
 )
 
-client = SearchIndexClient(service_endpoint, AzureKeyCredential(key))
-
 
 async def create_index():
     # [START create_index_async]
+    client = SearchIndexClient(service_endpoint, AzureKeyCredential(key))
     name = "hotels"
     fields = [
         SimpleField(name="hotelId", type=SearchFieldDataType.String, key=True),
         SimpleField(name="baseRate", type=SearchFieldDataType.Double),
         SearchableField(name="description", type=SearchFieldDataType.String, collection=True),
         ComplexField(
             name="address",
@@ -58,26 +57,30 @@
     ]
 
     cors_options = CorsOptions(allowed_origins=["*"], max_age_in_seconds=60)
     scoring_profiles = []
     index = SearchIndex(name=name, fields=fields, scoring_profiles=scoring_profiles, cors_options=cors_options)
 
     result = await client.create_index(index)
+    await client.close()
     # [END create_index_async]
 
 
 async def get_index():
     # [START get_index_async]
+    client = SearchIndexClient(service_endpoint, AzureKeyCredential(key))
     name = "hotels"
     result = await client.get_index(name)
+    await client.close()
     # [END get_index_async]
 
 
 async def update_index():
     # [START update_index_async]
+    client = SearchIndexClient(service_endpoint, AzureKeyCredential(key))
     name = "hotels"
     fields = [
         SimpleField(name="hotelId", type=SearchFieldDataType.String, key=True),
         SimpleField(name="baseRate", type=SearchFieldDataType.Double),
         SearchableField(name="description", type=SearchFieldDataType.String, collection=True),
         SearchableField(name="hotelName", type=SearchFieldDataType.String),
         ComplexField(
@@ -94,27 +97,29 @@
     cors_options = CorsOptions(allowed_origins=["*"], max_age_in_seconds=60)
     scoring_profile = ScoringProfile(name="MyProfile")
     scoring_profiles = []
     scoring_profiles.append(scoring_profile)
     index = SearchIndex(name=name, fields=fields, scoring_profiles=scoring_profiles, cors_options=cors_options)
 
     result = await client.create_or_update_index(index=index)
+    await client.close()
     # [END update_index_async]
 
 
 async def delete_index():
     # [START delete_index_async]
+    client = SearchIndexClient(service_endpoint, AzureKeyCredential(key))
     name = "hotels"
     await client.delete_index(name)
+    await client.close()
     # [END delete_index_async]
 
 
 async def main():
     await create_index()
     await get_index()
     await update_index()
     await delete_index()
-    await client.close()
 
 
 if __name__ == "__main__":
     asyncio.run(main())
```

## Comparing `azure-search-documents-11.4.0b6/samples/async_samples/sample_synonym_map_operations_async.py` & `azure-search-documents-11.4.0b7/samples/async_samples/sample_synonym_map_operations_async.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/samples/async_samples/sample_vector_search_async.py` & `azure-search-documents-11.4.0b7/samples/async_samples/sample_vector_search_async.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,23 +22,25 @@
 
 import os
 import asyncio
 
 from azure.core.credentials import AzureKeyCredential
 from azure.search.documents.aio import SearchClient
 from azure.search.documents.indexes import SearchIndexClient
+from azure.search.documents.models import Vector
 
 service_endpoint = os.getenv("AZURE_SEARCH_SERVICE_ENDPOINT")
 index_name = os.getenv("AZURE_SEARCH_INDEX_NAME")
 key = os.getenv("AZURE_SEARCH_API_KEY")
 
 
 def get_embeddings(text: str):
     # There are a few ways to get embeddings. This is just one example.
     import openai
+
     open_ai_endpoint = os.getenv("OpenAIEndpoint")
     open_ai_key = os.getenv("OpenAIKey")
 
     openai.api_version = "2022-12-01"
     openai.api_base = open_ai_endpoint
     openai.api_type = "azure"
     openai.api_key = open_ai_key
@@ -81,121 +83,120 @@
 
 def get_hotel_documents():
     docs = [
         {
             "hotelId": "1",
             "hotelName": "Fancy Stay",
             "description": "Best hotel in town if you like luxury hotels.",
-            "DescriptionVector": get_embeddings("Best hotel in town if you like luxury hotels."),
+            "descriptionVector": get_embeddings("Best hotel in town if you like luxury hotels."),
             "category": "Luxury",
         },
         {
-            "HotelId": "2",
-            "HotelName": "Roach Motel",
-            "Description": "Cheapest hotel in town. Infact, a motel.",
-            "DescriptionVector": get_embeddings("Cheapest hotel in town. Infact, a motel."),
-            "Category": "Budget",
+            "hotelId": "2",
+            "hotelName": "Roach Motel",
+            "descrdescriptioniption": "Cheapest hotel in town. Infact, a motel.",
+            "descriptionVector": get_embeddings("Cheapest hotel in town. Infact, a motel."),
+            "category": "Budget",
         },
         {
-            "HotelId": "3",
-            "HotelName": "EconoStay",
-            "Description": "Very popular hotel in town.",
-            "DescriptionVector": get_embeddings("Very popular hotel in town."),
-            "Category": "Budget",
+            "hotelId": "3",
+            "hotelName": "EconoStay",
+            "description": "Very popular hotel in town.",
+            "descriptionVector": get_embeddings("Very popular hotel in town."),
+            "category": "Budget",
         },
         {
-            "HotelId": "4",
-            "HotelName": "Modern Stay",
-            "Description": "Modern architecture, very polite staff and very clean. Also very affordable.",
-            "DescriptionVector": get_embeddings(
+            "hotelId": "4",
+            "hotelName": "Modern Stay",
+            "description": "Modern architecture, very polite staff and very clean. Also very affordable.",
+            "descriptionVector": get_embeddings(
                 "Modern architecture, very polite staff and very clean. Also very affordable."
             ),
-            "Category": "Luxury",
+            "category": "Luxury",
         },
         {
-            "HotelId": "5",
-            "HotelName": "Secret Point",
-            "Description": "One of the best hotel in town. The hotel is ideally located on the main commercial artery of the city in the heart of New York.",
-            "DescriptionVector": get_embeddings(
+            "hotelId": "5",
+            "hotelName": "Secret Point",
+            "description": "One of the best hotel in town. The hotel is ideally located on the main commercial artery of the city in the heart of New York.",
+            "descriptionVector": get_embeddings(
                 "One of the best hotel in town. The hotel is ideally located on the main commercial artery of the city in the heart of New York."
             ),
-            "Category": "Boutique",
+            "category": "Boutique",
         },
     ]
     return docs
 
 
 async def single_vector_search():
     # [START single_vector_search]
     query = "Top hotels in town"
 
     search_client = SearchClient(service_endpoint, index_name, AzureKeyCredential(key))
+    vector = Vector(value=get_embeddings(query), k=3, fields="descriptionVector")
 
     async with search_client:
         results = await search_client.search(
             search_text="",
-            vector=get_embeddings(query),
-            top_k=3,
-            vector_fields="descriptionVector",
+            vectors=[vector],
             select=["hotelId", "hotelName"],
         )
 
         async for result in results:
             print(result)
     # [END single_vector_search]
 
 
 async def single_vector_search_with_filter():
     # [START single_vector_search_with_filter]
     query = "Top hotels in town"
 
     search_client = SearchClient(service_endpoint, index_name, AzureKeyCredential(key))
+    vector = Vector(value=get_embeddings(query), k=3, fields="descriptionVector")
 
     async with search_client:
         results = await search_client.search(
             search_text="",
-            vector=get_embeddings(query),
-            top_k=3,
-            vector_fields="descriptionVector",
+            vectors=[vector],
             filter="category eq 'Luxury'",
             select=["hotelId", "hotelName"],
         )
 
         async for result in results:
             print(result)
     # [END single_vector_search_with_filter]
 
 
 async def simple_hybrid_search():
     # [START simple_hybrid_search]
     query = "Top hotels in town"
 
     search_client = SearchClient(service_endpoint, index_name, AzureKeyCredential(key))
+    vector = Vector(value=get_embeddings(query), k=3, fields="descriptionVector")
 
     async with search_client:
         results = await search_client.search(
             search_text=query,
-            vector=get_embeddings(query),
-            top_k=3,
-            vector_fields="descriptionVector",
+            vectors=[vector],
             select=["hotelId", "hotelName"],
         )
         print(await results.get_answers())
         async for result in results:
             print(result)
     # [END simple_hybrid_search]
 
 
-if __name__ == "__main__":
+async def main():
     credential = AzureKeyCredential(key)
     index_client = SearchIndexClient(service_endpoint, credential)
     index = get_hotel_index(index_name)
     index_client.create_index(index)
     client = SearchClient(service_endpoint, index_name, credential)
     hotel_docs = get_hotel_documents()
-    client.upload_documents(documents=hotel_docs)
-    
-    single_vector_search()
-    single_vector_search_with_filter()
-    asyncio.run(single_vector_search())
-    asyncio.run(single_vector_search_with_filter())
-    asyncio.run(simple_hybrid_search())
+    await client.upload_documents(documents=hotel_docs)
+
+    await single_vector_search()
+    await single_vector_search_with_filter()
+    await simple_hybrid_search()
+
+
+if __name__ == "__main__":
+    asyncio.run(main())
```

## Comparing `azure-search-documents-11.4.0b6/samples/async_samples/sample_filter_query_async.py` & `azure-search-documents-11.4.0b7/samples/async_samples/sample_filter_query_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,24 +32,24 @@
 async def filter_query():
     # [START filter_query_async]
     from azure.core.credentials import AzureKeyCredential
     from azure.search.documents.aio import SearchClient
 
     search_client = SearchClient(service_endpoint, index_name, AzureKeyCredential(key))
 
-    select = ("HotelName", "Rating")
+    select = ("hotelName", "rating")
     async with search_client:
         results = await search_client.search(
             search_text="WiFi",
             filter="Address/StateProvince eq 'FL' and Address/Country eq 'USA'",
             select=",".join(select),
-            order_by="Rating desc",
+            order_by="rating desc",
         )
 
         print("Florida hotels containing 'WiFi', sorted by Rating:")
         async for result in results:
-            print("    Name: {} (rating {})".format(result["HotelName"], result["Rating"]))
+            print("    Name: {} (rating {})".format(result["hotelName"], result["rating"]))
     # [END filter_query_async]
 
 
 if __name__ == "__main__":
     asyncio.run(filter_query())
```

## Comparing `azure-search-documents-11.4.0b6/samples/async_samples/sample_data_source_operations_async.py` & `azure-search-documents-11.4.0b7/samples/async_samples/sample_data_source_operations_async.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/samples/async_samples/sample_autocomplete_async.py` & `azure-search-documents-11.4.0b7/samples/async_samples/sample_autocomplete_async.py`

 * *Files identical despite different names*

## Comparing `azure-search-documents-11.4.0b6/samples/async_samples/sample_get_document_async.py` & `azure-search-documents-11.4.0b7/samples/async_samples/sample_get_document_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
     search_client = SearchClient(service_endpoint, index_name, AzureKeyCredential(key))
 
     async with search_client:
         result = await search_client.get_document(key="23")
 
         print("Details for hotel '23' are:")
-        print("        Name: {}".format(result["HotelName"]))
-        print("      Rating: {}".format(result["Rating"]))
-        print("    Category: {}".format(result["Category"]))
+        print("        Name: {}".format(result["hotelName"]))
+        print("      Rating: {}".format(result["rating"]))
+        print("    Category: {}".format(result["category"]))
     # [END get_document_async]
 
 
 if __name__ == "__main__":
     asyncio.run(autocomplete_query())
```

## Comparing `azure-search-documents-11.4.0b6/azure_search_documents.egg-info/PKG-INFO` & `azure-search-documents-11.4.0b7/azure_search_documents.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-search-documents
-Version: 11.4.0b6
+Version: 11.4.0b7
 Summary: Microsoft Azure Cognitive Search Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/search/azure-search-documents
 Author: Microsoft Corporation
 Author-email: ascl@microsoft.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -261,14 +261,15 @@
 You can use the `SearchIndexClient` to create a search index. Fields can be
 defined using convenient `SimpleField`, `SearchableField`, or `ComplexField`
 models. Indexes can also define suggesters, lexical analyzers, and more.
 
 <!-- SNIPPET:sample_index_crud_operations.create_index -->
 
 ```python
+client = SearchIndexClient(service_endpoint, AzureKeyCredential(key))
 name = "hotels"
 fields = [
     SimpleField(name="hotelId", type=SearchFieldDataType.String, key=True),
     SimpleField(name="baseRate", type=SearchFieldDataType.Double),
     SearchableField(name="description", type=SearchFieldDataType.String, collection=True),
     ComplexField(
         name="address",
@@ -295,19 +296,19 @@
 [a few special rules for merging](https://docs.microsoft.com/rest/api/searchservice/addupdate-or-delete-documents#document-actions)
 to be aware of.
 
 <!-- SNIPPET:sample_crud_operations.upload_document -->
 
 ```python
 DOCUMENT = {
-    "Category": "Hotel",
-    "HotelId": "1000",
-    "Rating": 4.0,
-    "Rooms": [],
-    "HotelName": "Azure Inn",
+    "category": "Hotel",
+    "hotelId": "1000",
+    "rating": 4.0,
+    "rooms": [],
+    "hotelName": "Azure Inn",
 }
 
 result = search_client.upload_documents(documents=[DOCUMENT])
 
 print("Upload of new document succeeded: {}".format(result[0].succeeded))
 ```
 
@@ -348,17 +349,17 @@
 from azure.search.documents import SearchClient
 
 search_client = SearchClient(service_endpoint, index_name, AzureKeyCredential(key))
 
 result = search_client.get_document(key="23")
 
 print("Details for hotel '23' are:")
-print("        Name: {}".format(result["HotelName"]))
-print("      Rating: {}".format(result["Rating"]))
-print("    Category: {}".format(result["Category"]))
+print("        Name: {}".format(result["hotelName"]))
+print("      Rating: {}".format(result["rating"]))
+print("    Category: {}".format(result["category"]))
 ```
 
 <!-- END SNIPPET -->
 
 ### Async APIs
 
 This library includes a complete async API. To use it, you must
@@ -376,15 +377,15 @@
 search_client = SearchClient(service_endpoint, index_name, AzureKeyCredential(key))
 
 async with search_client:
     results = await search_client.search(search_text="spa")
 
     print("Hotels containing 'spa' in the name (or other fields):")
     async for result in results:
-        print("    Name: {} (rating {})".format(result["HotelName"], result["Rating"]))
+        print("    Name: {} (rating {})".format(result["hotelName"], result["rating"]))
 ```
 
 <!-- END SNIPPET -->
 
 ## Troubleshooting
 
 ### General
```

## Comparing `azure-search-documents-11.4.0b6/azure_search_documents.egg-info/SOURCES.txt` & `azure-search-documents-11.4.0b7/azure_search_documents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

