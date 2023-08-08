# Comparing `tmp/offchain-0.1.4.tar.gz` & `tmp/offchain-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "offchain-0.1.4.tar", max compression
+gzip compressed data, was "offchain-0.1.5.tar", max compression
```

## Comparing `offchain-0.1.4.tar` & `offchain-0.1.5.tar`

### file list

```diff
@@ -1,68 +1,67 @@
--rw-r--r--   0        0        0     1066 2023-01-31 19:05:23.364203 offchain-0.1.4/LICENSE
--rw-r--r--   0        0        0     2805 2023-01-31 19:05:23.364203 offchain-0.1.4/README.md
--rw-r--r--   0        0        0      163 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/__init__.py
--rw-r--r--   0        0        0        0 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/base/__init__.py
--rw-r--r--   0        0        0       45 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/base/base_model.py
--rw-r--r--   0        0        0      454 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/base/types.py
--rw-r--r--   0        0        0     1676 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/concurrency.py
--rw-r--r--   0        0        0        0 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/constants/__init__.py
--rw-r--r--   0        0        0     1061 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/constants/addresses.py
--rw-r--r--   0        0        0      183 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/constants/providers.py
--rw-r--r--   0        0        0        0 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/logger/__init__.py
--rw-r--r--   0        0        0      384 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/logger/logging.py
--rw-r--r--   0        0        0      217 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/__init__.py
--rw-r--r--   0        0        0      194 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/adapters/__init__.py
--rw-r--r--   0        0        0     1906 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/adapters/arweave.py
--rw-r--r--   0        0        0     1055 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/adapters/base_adapter.py
--rw-r--r--   0        0        0     1209 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/adapters/data_uri.py
--rw-r--r--   0        0        0      317 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/adapters/http_adapter.py
--rw-r--r--   0        0        0     3618 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/adapters/ipfs.py
--rw-r--r--   0        0        0        0 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/constants/__init__.py
--rw-r--r--   0        0        0      359 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/constants/autoglyphs.py
--rw-r--r--   0        0        0     7181 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/constants/nouns.py
--rw-r--r--   0        0        0       84 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/fetchers/__init__.py
--rw-r--r--   0        0        0     1725 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/fetchers/base_fetcher.py
--rw-r--r--   0        0        0     3410 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/fetchers/metadata_fetcher.py
--rw-r--r--   0        0        0      612 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/get_token_metadata.py
--rw-r--r--   0        0        0      225 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/models/__init__.py
--rw-r--r--   0        0        0     3488 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/models/metadata.py
--rw-r--r--   0        0        0      800 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/models/metadata_processing_error.py
--rw-r--r--   0        0        0     1049 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/models/token.py
--rw-r--r--   0        0        0      867 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/parsers/__init__.py
--rw-r--r--   0        0        0     1622 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/parsers/base_parser.py
--rw-r--r--   0        0        0        0 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/parsers/catchall/__init__.py
--rw-r--r--   0        0        0      568 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/parsers/catchall/catchall_parser.py
--rw-r--r--   0        0        0     6049 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/parsers/catchall/default_catchall.py
--rw-r--r--   0        0        0        0 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/parsers/collection/__init__.py
--rw-r--r--   0        0        0    10245 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/parsers/collection/artblocks.py
--rw-r--r--   0        0        0     4840 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/parsers/collection/autoglyphs.py
--rw-r--r--   0        0        0     1448 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/parsers/collection/chainrunners.py
--rw-r--r--   0        0        0     1930 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/parsers/collection/collection_parser.py
--rw-r--r--   0        0        0     2692 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/parsers/collection/decentraland.py
--rw-r--r--   0        0        0     4465 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/parsers/collection/ens.py
--rw-r--r--   0        0        0     1143 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/parsers/collection/foundation.py
--rw-r--r--   0        0        0     3253 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/parsers/collection/hashmasks.py
--rw-r--r--   0        0        0     2968 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/parsers/collection/loot.py
--rw-r--r--   0        0        0     2509 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/parsers/collection/makersplace.py
--rw-r--r--   0        0        0     3618 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/parsers/collection/nouns.py
--rw-r--r--   0        0        0     3707 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/parsers/collection/punks.py
--rw-r--r--   0        0        0     3589 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/parsers/collection/superrare.py
--rw-r--r--   0        0        0     3061 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/parsers/collection/zora.py
--rw-r--r--   0        0        0        0 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/parsers/schema/__init__.py
--rw-r--r--   0        0        0     5167 2023-01-31 19:05:23.364203 offchain-0.1.4/offchain/metadata/parsers/schema/opensea.py
--rw-r--r--   0        0        0      653 2023-01-31 19:05:23.368203 offchain-0.1.4/offchain/metadata/parsers/schema/schema_parser.py
--rw-r--r--   0        0        0       88 2023-01-31 19:05:23.368203 offchain-0.1.4/offchain/metadata/pipelines/__init__.py
--rw-r--r--   0        0        0      216 2023-01-31 19:05:23.368203 offchain-0.1.4/offchain/metadata/pipelines/base_pipeline.py
--rw-r--r--   0        0        0     9511 2023-01-31 19:05:23.368203 offchain-0.1.4/offchain/metadata/pipelines/metadata_pipeline.py
--rw-r--r--   0        0        0        0 2023-01-31 19:05:23.368203 offchain-0.1.4/offchain/metadata/registries/__init__.py
--rw-r--r--   0        0        0      891 2023-01-31 19:05:23.368203 offchain-0.1.4/offchain/metadata/registries/adapter_registry.py
--rw-r--r--   0        0        0     1386 2023-01-31 19:05:23.368203 offchain-0.1.4/offchain/metadata/registries/base_registry.py
--rw-r--r--   0        0        0      741 2023-01-31 19:05:23.368203 offchain-0.1.4/offchain/metadata/registries/fetcher_registry.py
--rw-r--r--   0        0        0     2287 2023-01-31 19:05:23.368203 offchain-0.1.4/offchain/metadata/registries/parser_registry.py
--rw-r--r--   0        0        0        0 2023-01-31 19:05:23.368203 offchain-0.1.4/offchain/web3/__init__.py
--rw-r--r--   0        0        0     6709 2023-01-31 19:05:23.368203 offchain-0.1.4/offchain/web3/contract_caller.py
--rw-r--r--   0        0        0      487 2023-01-31 19:05:23.368203 offchain-0.1.4/offchain/web3/contract_utils.py
--rw-r--r--   0        0        0     3179 2023-01-31 19:05:23.368203 offchain-0.1.4/offchain/web3/jsonrpc.py
--rw-r--r--   0        0        0      677 2023-01-31 19:05:23.368203 offchain-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4105 1970-01-01 00:00:00.000000 offchain-0.1.4/setup.py
--rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 offchain-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-08-08 15:18:41.040844 offchain-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2805 2023-08-08 15:18:41.040844 offchain-0.1.5/README.md
+-rw-r--r--   0        0        0      163 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/base/__init__.py
+-rw-r--r--   0        0        0       45 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/base/base_model.py
+-rw-r--r--   0        0        0      454 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/base/types.py
+-rw-r--r--   0        0        0     1676 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/concurrency.py
+-rw-r--r--   0        0        0        0 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/constants/__init__.py
+-rw-r--r--   0        0        0     1061 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/constants/addresses.py
+-rw-r--r--   0        0        0      183 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/constants/providers.py
+-rw-r--r--   0        0        0        0 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/logger/__init__.py
+-rw-r--r--   0        0        0      384 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/logger/logging.py
+-rw-r--r--   0        0        0      217 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/__init__.py
+-rw-r--r--   0        0        0      194 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/adapters/__init__.py
+-rw-r--r--   0        0        0     1906 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/adapters/arweave.py
+-rw-r--r--   0        0        0     1055 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/adapters/base_adapter.py
+-rw-r--r--   0        0        0     1209 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/adapters/data_uri.py
+-rw-r--r--   0        0        0      317 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/adapters/http_adapter.py
+-rw-r--r--   0        0        0     3618 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/adapters/ipfs.py
+-rw-r--r--   0        0        0        0 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/constants/__init__.py
+-rw-r--r--   0        0        0      359 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/constants/autoglyphs.py
+-rw-r--r--   0        0        0     7181 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/constants/nouns.py
+-rw-r--r--   0        0        0       84 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/fetchers/__init__.py
+-rw-r--r--   0        0        0     1725 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/fetchers/base_fetcher.py
+-rw-r--r--   0        0        0     3410 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/fetchers/metadata_fetcher.py
+-rw-r--r--   0        0        0      612 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/get_token_metadata.py
+-rw-r--r--   0        0        0      225 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/models/__init__.py
+-rw-r--r--   0        0        0     3488 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/models/metadata.py
+-rw-r--r--   0        0        0      800 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/models/metadata_processing_error.py
+-rw-r--r--   0        0        0     1049 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/models/token.py
+-rw-r--r--   0        0        0      867 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/parsers/__init__.py
+-rw-r--r--   0        0        0     1622 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/parsers/base_parser.py
+-rw-r--r--   0        0        0        0 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/parsers/catchall/__init__.py
+-rw-r--r--   0        0        0      568 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/parsers/catchall/catchall_parser.py
+-rw-r--r--   0        0        0     6049 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/parsers/catchall/default_catchall.py
+-rw-r--r--   0        0        0        0 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/parsers/collection/__init__.py
+-rw-r--r--   0        0        0    10245 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/parsers/collection/artblocks.py
+-rw-r--r--   0        0        0     4840 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/parsers/collection/autoglyphs.py
+-rw-r--r--   0        0        0     1448 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/parsers/collection/chainrunners.py
+-rw-r--r--   0        0        0     1938 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/parsers/collection/collection_parser.py
+-rw-r--r--   0        0        0     2692 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/parsers/collection/decentraland.py
+-rw-r--r--   0        0        0     4465 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/parsers/collection/ens.py
+-rw-r--r--   0        0        0     1143 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/parsers/collection/foundation.py
+-rw-r--r--   0        0        0     3253 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/parsers/collection/hashmasks.py
+-rw-r--r--   0        0        0     2968 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/parsers/collection/loot.py
+-rw-r--r--   0        0        0     2509 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/parsers/collection/makersplace.py
+-rw-r--r--   0        0        0     3618 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/parsers/collection/nouns.py
+-rw-r--r--   0        0        0     3707 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/parsers/collection/punks.py
+-rw-r--r--   0        0        0     3589 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/parsers/collection/superrare.py
+-rw-r--r--   0        0        0     3095 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/parsers/collection/zora.py
+-rw-r--r--   0        0        0        0 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/parsers/schema/__init__.py
+-rw-r--r--   0        0        0     5167 2023-08-08 15:18:41.040844 offchain-0.1.5/offchain/metadata/parsers/schema/opensea.py
+-rw-r--r--   0        0        0      653 2023-08-08 15:18:41.044844 offchain-0.1.5/offchain/metadata/parsers/schema/schema_parser.py
+-rw-r--r--   0        0        0       88 2023-08-08 15:18:41.044844 offchain-0.1.5/offchain/metadata/pipelines/__init__.py
+-rw-r--r--   0        0        0      216 2023-08-08 15:18:41.044844 offchain-0.1.5/offchain/metadata/pipelines/base_pipeline.py
+-rw-r--r--   0        0        0     9511 2023-08-08 15:18:41.044844 offchain-0.1.5/offchain/metadata/pipelines/metadata_pipeline.py
+-rw-r--r--   0        0        0        0 2023-08-08 15:18:41.044844 offchain-0.1.5/offchain/metadata/registries/__init__.py
+-rw-r--r--   0        0        0      891 2023-08-08 15:18:41.044844 offchain-0.1.5/offchain/metadata/registries/adapter_registry.py
+-rw-r--r--   0        0        0     1386 2023-08-08 15:18:41.044844 offchain-0.1.5/offchain/metadata/registries/base_registry.py
+-rw-r--r--   0        0        0      741 2023-08-08 15:18:41.044844 offchain-0.1.5/offchain/metadata/registries/fetcher_registry.py
+-rw-r--r--   0        0        0     2287 2023-08-08 15:18:41.044844 offchain-0.1.5/offchain/metadata/registries/parser_registry.py
+-rw-r--r--   0        0        0        0 2023-08-08 15:18:41.044844 offchain-0.1.5/offchain/web3/__init__.py
+-rw-r--r--   0        0        0     6709 2023-08-08 15:18:41.044844 offchain-0.1.5/offchain/web3/contract_caller.py
+-rw-r--r--   0        0        0      487 2023-08-08 15:18:41.044844 offchain-0.1.5/offchain/web3/contract_utils.py
+-rw-r--r--   0        0        0     3179 2023-08-08 15:18:41.044844 offchain-0.1.5/offchain/web3/jsonrpc.py
+-rw-r--r--   0        0        0      680 2023-08-08 15:18:41.044844 offchain-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3537 1970-01-01 00:00:00.000000 offchain-0.1.5/PKG-INFO
```

### Comparing `offchain-0.1.4/LICENSE` & `offchain-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/README.md` & `offchain-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/concurrency.py` & `offchain-0.1.5/offchain/concurrency.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/constants/addresses.py` & `offchain-0.1.5/offchain/constants/addresses.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/metadata/adapters/arweave.py` & `offchain-0.1.5/offchain/metadata/adapters/arweave.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/metadata/adapters/base_adapter.py` & `offchain-0.1.5/offchain/metadata/adapters/base_adapter.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/metadata/adapters/data_uri.py` & `offchain-0.1.5/offchain/metadata/adapters/data_uri.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/metadata/adapters/ipfs.py` & `offchain-0.1.5/offchain/metadata/adapters/ipfs.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/metadata/constants/nouns.py` & `offchain-0.1.5/offchain/metadata/constants/nouns.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/metadata/fetchers/base_fetcher.py` & `offchain-0.1.5/offchain/metadata/fetchers/base_fetcher.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/metadata/fetchers/metadata_fetcher.py` & `offchain-0.1.5/offchain/metadata/fetchers/metadata_fetcher.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/metadata/get_token_metadata.py` & `offchain-0.1.5/offchain/metadata/get_token_metadata.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/metadata/models/metadata.py` & `offchain-0.1.5/offchain/metadata/models/metadata.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/metadata/models/metadata_processing_error.py` & `offchain-0.1.5/offchain/metadata/models/metadata_processing_error.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/metadata/models/token.py` & `offchain-0.1.5/offchain/metadata/models/token.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/metadata/parsers/__init__.py` & `offchain-0.1.5/offchain/metadata/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/metadata/parsers/base_parser.py` & `offchain-0.1.5/offchain/metadata/parsers/base_parser.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/metadata/parsers/catchall/catchall_parser.py` & `offchain-0.1.5/offchain/metadata/parsers/catchall/catchall_parser.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/metadata/parsers/catchall/default_catchall.py` & `offchain-0.1.5/offchain/metadata/parsers/catchall/default_catchall.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/metadata/parsers/collection/artblocks.py` & `offchain-0.1.5/offchain/metadata/parsers/collection/artblocks.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/metadata/parsers/collection/autoglyphs.py` & `offchain-0.1.5/offchain/metadata/parsers/collection/autoglyphs.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/metadata/parsers/collection/chainrunners.py` & `offchain-0.1.5/offchain/metadata/parsers/collection/chainrunners.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/metadata/parsers/collection/collection_parser.py` & `offchain-0.1.5/offchain/metadata/parsers/collection/collection_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,8 +36,8 @@
 
         Args:
             token (Token): the token whose metadata needs to be parsed.
 
         Returns:
             bool: whether or not the collection parser handles this token.
         """
-        return token.collection_address in [address.lower() for address in self._COLLECTION_ADDRESSES]
+        return token.collection_address.lower() in [address.lower() for address in self._COLLECTION_ADDRESSES]
```

### Comparing `offchain-0.1.4/offchain/metadata/parsers/collection/decentraland.py` & `offchain-0.1.5/offchain/metadata/parsers/collection/decentraland.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/metadata/parsers/collection/ens.py` & `offchain-0.1.5/offchain/metadata/parsers/collection/ens.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/metadata/parsers/collection/foundation.py` & `offchain-0.1.5/offchain/metadata/parsers/collection/foundation.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/metadata/parsers/collection/hashmasks.py` & `offchain-0.1.5/offchain/metadata/parsers/collection/hashmasks.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/metadata/parsers/collection/loot.py` & `offchain-0.1.5/offchain/metadata/parsers/collection/loot.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/metadata/parsers/collection/makersplace.py` & `offchain-0.1.5/offchain/metadata/parsers/collection/makersplace.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/metadata/parsers/collection/nouns.py` & `offchain-0.1.5/offchain/metadata/parsers/collection/nouns.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/metadata/parsers/collection/punks.py` & `offchain-0.1.5/offchain/metadata/parsers/collection/punks.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/metadata/parsers/collection/superrare.py` & `offchain-0.1.5/offchain/metadata/parsers/collection/superrare.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/metadata/parsers/collection/zora.py` & `offchain-0.1.5/offchain/metadata/parsers/collection/zora.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             return MediaDetails(uri=uri, size=size, sha256=None, mime_type=content_type)
         except Exception:
             pass
 
         return None
 
     def parse_metadata(self, token: Token, raw_data: Optional[dict], *args, **kwargs) -> Optional[Metadata]:
-        if token.uri is None or raw_data is None:
+        if token.uri is None or raw_data is None or not isinstance(raw_data, dict):
             token.uri = self.get_uri(token.token_id)
             raw_data = self.fetcher.fetch_content(token.uri)
 
         metadata = DefaultCatchallParser(self.fetcher).parse_metadata(token=token, raw_data=raw_data)
 
         content_uri = self.get_content_uri(token.token_id)
         content = self.get_content_details(content_uri)
```

### Comparing `offchain-0.1.4/offchain/metadata/parsers/schema/opensea.py` & `offchain-0.1.5/offchain/metadata/parsers/schema/opensea.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/metadata/parsers/schema/schema_parser.py` & `offchain-0.1.5/offchain/metadata/parsers/schema/schema_parser.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/metadata/pipelines/metadata_pipeline.py` & `offchain-0.1.5/offchain/metadata/pipelines/metadata_pipeline.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/metadata/registries/adapter_registry.py` & `offchain-0.1.5/offchain/metadata/registries/adapter_registry.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/metadata/registries/base_registry.py` & `offchain-0.1.5/offchain/metadata/registries/base_registry.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/metadata/registries/fetcher_registry.py` & `offchain-0.1.5/offchain/metadata/registries/fetcher_registry.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/metadata/registries/parser_registry.py` & `offchain-0.1.5/offchain/metadata/registries/parser_registry.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/web3/contract_caller.py` & `offchain-0.1.5/offchain/web3/contract_caller.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/offchain/web3/jsonrpc.py` & `offchain-0.1.5/offchain/web3/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `offchain-0.1.4/pyproject.toml` & `offchain-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "offchain"
-version = "0.1.4"
+version = "0.1.5"
 description = "Open source metadata processing framework"
 authors = ["Zora eng <eng@zora.co>"]
 readme = "README.md"
 documentation = "https://ourzora.github.io/offchain"
 
 [tool.poetry.dependencies]
-python = ">=3.9"
+python = ">=3.9 <4"
 requests = "^2.28.1"
 pydantic = "^1.9.2"
 python-json-logger = "^2.0.4"
 urllib3 = "^1.26.11"
 web3 = "^5.30.0"
 tenacity = "^8.0.1"
```

### Comparing `offchain-0.1.4/PKG-INFO` & `offchain-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: offchain
-Version: 0.1.4
+Version: 0.1.5
 Summary: Open source metadata processing framework
 Author: Zora eng
 Author-email: eng@zora.co
-Requires-Python: >=3.9
+Requires-Python: >=3.9,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.9.2,<2.0.0)
 Requires-Dist: python-json-logger (>=2.0.4,<3.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
```

