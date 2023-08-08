# Comparing `tmp/vertex_protocol-1.1.6.tar.gz` & `tmp/vertex_protocol-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vertex_protocol-1.1.6.tar", max compression
+gzip compressed data, was "vertex_protocol-1.1.7.tar", max compression
```

## Comparing `vertex_protocol-1.1.6.tar` & `vertex_protocol-1.1.7.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     3337 2023-08-02 20:23:25.909049 vertex_protocol-1.1.6/README.md
--rw-r--r--   0        0        0     1664 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/__init__.py
--rw-r--r--   0        0        0     6634 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/client/__init__.py
--rw-r--r--   0        0        0      580 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/client/apis/__init__.py
--rw-r--r--   0        0        0     1394 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/client/apis/base.py
--rw-r--r--   0        0        0     1108 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/client/apis/market/__init__.py
--rw-r--r--   0        0        0     3516 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/client/apis/market/execute.py
--rw-r--r--   0        0        0    10439 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/client/apis/market/query.py
--rw-r--r--   0        0        0      746 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/client/apis/perp/__init__.py
--rw-r--r--   0        0        0     1438 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/client/apis/perp/query.py
--rw-r--r--   0        0        0     1027 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/client/apis/spot/__init__.py
--rw-r--r--   0        0        0     1191 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/client/apis/spot/base.py
--rw-r--r--   0        0        0     4782 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/client/apis/spot/execute.py
--rw-r--r--   0        0        0     2964 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/client/apis/spot/query.py
--rw-r--r--   0        0        0     1307 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/client/apis/subaccount/__init__.py
--rw-r--r--   0        0        0     2023 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/client/apis/subaccount/execute.py
--rw-r--r--   0        0        0     3669 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/client/apis/subaccount/query.py
--rw-r--r--   0        0        0     2554 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/client/context.py
--rw-r--r--   0        0        0     8786 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/contracts/__init__.py
--rw-r--r--   0        0        0    13215 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/contracts/abis/Endpoint.json
--rw-r--r--   0        0        0    55374 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/contracts/abis/FQuerier.json
--rw-r--r--   0        0        0    17205 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/contracts/abis/IClearinghouse.json
--rw-r--r--   0        0        0     3385 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/contracts/abis/IERC20.json
--rw-r--r--   0        0        0     5677 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/contracts/abis/IEndpoint.json
--rw-r--r--   0        0        0    13112 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/contracts/abis/IOffchainBook.json
--rw-r--r--   0        0        0    19201 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/contracts/abis/IPerpEngine.json
--rw-r--r--   0        0        0     6291 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/contracts/abis/IProductEngine.json
--rw-r--r--   0        0        0    16739 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/contracts/abis/ISpotEngine.json
--rw-r--r--   0        0        0     5698 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/contracts/abis/MockERC20.json
--rw-r--r--   0        0        0     1013 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/contracts/deployments/deployment.arbitrumGoerli.json
--rw-r--r--   0        0        0      993 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/contracts/deployments/deployment.arbitrumOne.json
--rw-r--r--   0        0        0      908 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/contracts/deployments/deployment.test.json
--rw-r--r--   0        0        0      426 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/contracts/eip712/__init__.py
--rw-r--r--   0        0        0     1189 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/contracts/eip712/domain.py
--rw-r--r--   0        0        0     2484 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/contracts/eip712/sign.py
--rw-r--r--   0        0        0     4636 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/contracts/eip712/types.py
--rw-r--r--   0        0        0     1526 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/contracts/loader.py
--rw-r--r--   0        0        0     2914 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/contracts/types.py
--rw-r--r--   0        0        0     1127 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/engine_client/__init__.py
--rw-r--r--   0        0        0    18741 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/engine_client/execute.py
--rw-r--r--   0        0        0    12030 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/engine_client/query.py
--rw-r--r--   0        0        0     5739 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/engine_client/types/__init__.py
--rw-r--r--   0        0        0    18756 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/engine_client/types/execute.py
--rw-r--r--   0        0        0     3505 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/engine_client/types/models.py
--rw-r--r--   0        0        0     9927 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/engine_client/types/query.py
--rw-r--r--   0        0        0      926 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/indexer_client/__init__.py
--rw-r--r--   0        0        0    11793 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/indexer_client/query.py
--rw-r--r--   0        0        0     3077 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/indexer_client/types/__init__.py
--rw-r--r--   0        0        0     5656 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/indexer_client/types/models.py
--rw-r--r--   0        0        0    12832 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/indexer_client/types/query.py
--rw-r--r--   0        0        0      933 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/utils/__init__.py
--rw-r--r--   0        0        0      341 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/utils/backend.py
--rw-r--r--   0        0        0     5301 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/utils/bytes32.py
--rw-r--r--   0        0        0       99 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/utils/enum.py
--rw-r--r--   0        0        0     1136 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/utils/exceptions.py
--rw-r--r--   0        0        0     1094 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/utils/expiration.py
--rw-r--r--   0        0        0     1020 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/utils/math.py
--rw-r--r--   0        0        0     2089 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/utils/model.py
--rw-r--r--   0        0        0      863 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/utils/nonce.py
--rw-r--r--   0        0        0      503 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/utils/subaccount.py
--rw-r--r--   0        0        0     4119 1970-01-01 00:00:00.000000 vertex_protocol-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0     3337 2023-08-08 03:56:13.241867 vertex_protocol-1.1.7/README.md
+-rw-r--r--   0        0        0     1663 2023-08-08 03:56:13.241867 vertex_protocol-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/__init__.py
+-rw-r--r--   0        0        0     6634 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/client/__init__.py
+-rw-r--r--   0        0        0      580 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/client/apis/__init__.py
+-rw-r--r--   0        0        0     1394 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/client/apis/base.py
+-rw-r--r--   0        0        0     1108 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/client/apis/market/__init__.py
+-rw-r--r--   0        0        0     4258 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/client/apis/market/execute.py
+-rw-r--r--   0        0        0    10439 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/client/apis/market/query.py
+-rw-r--r--   0        0        0      746 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/client/apis/perp/__init__.py
+-rw-r--r--   0        0        0     1438 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/client/apis/perp/query.py
+-rw-r--r--   0        0        0     1027 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/client/apis/spot/__init__.py
+-rw-r--r--   0        0        0     1191 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/client/apis/spot/base.py
+-rw-r--r--   0        0        0     4782 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/client/apis/spot/execute.py
+-rw-r--r--   0        0        0     2964 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/client/apis/spot/query.py
+-rw-r--r--   0        0        0     1307 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/client/apis/subaccount/__init__.py
+-rw-r--r--   0        0        0     2023 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/client/apis/subaccount/execute.py
+-rw-r--r--   0        0        0     3669 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/client/apis/subaccount/query.py
+-rw-r--r--   0        0        0     2554 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/client/context.py
+-rw-r--r--   0        0        0     8786 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/contracts/__init__.py
+-rw-r--r--   0        0        0    13215 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/contracts/abis/Endpoint.json
+-rw-r--r--   0        0        0    55374 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/contracts/abis/FQuerier.json
+-rw-r--r--   0        0        0    17205 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/contracts/abis/IClearinghouse.json
+-rw-r--r--   0        0        0     3385 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/contracts/abis/IERC20.json
+-rw-r--r--   0        0        0     5677 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/contracts/abis/IEndpoint.json
+-rw-r--r--   0        0        0    13112 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/contracts/abis/IOffchainBook.json
+-rw-r--r--   0        0        0    19201 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/contracts/abis/IPerpEngine.json
+-rw-r--r--   0        0        0     6291 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/contracts/abis/IProductEngine.json
+-rw-r--r--   0        0        0    16739 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/contracts/abis/ISpotEngine.json
+-rw-r--r--   0        0        0     5698 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/contracts/abis/MockERC20.json
+-rw-r--r--   0        0        0     1013 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/contracts/deployments/deployment.arbitrumGoerli.json
+-rw-r--r--   0        0        0      993 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/contracts/deployments/deployment.arbitrumOne.json
+-rw-r--r--   0        0        0      908 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/contracts/deployments/deployment.test.json
+-rw-r--r--   0        0        0      426 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/contracts/eip712/__init__.py
+-rw-r--r--   0        0        0     1189 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/contracts/eip712/domain.py
+-rw-r--r--   0        0        0     2484 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/contracts/eip712/sign.py
+-rw-r--r--   0        0        0     4636 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/contracts/eip712/types.py
+-rw-r--r--   0        0        0     1526 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/contracts/loader.py
+-rw-r--r--   0        0        0     2914 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/contracts/types.py
+-rw-r--r--   0        0        0     1127 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/engine_client/__init__.py
+-rw-r--r--   0        0        0    21167 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/engine_client/execute.py
+-rw-r--r--   0        0        0    12030 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/engine_client/query.py
+-rw-r--r--   0        0        0     5739 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/engine_client/types/__init__.py
+-rw-r--r--   0        0        0    18756 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/engine_client/types/execute.py
+-rw-r--r--   0        0        0     3505 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/engine_client/types/models.py
+-rw-r--r--   0        0        0     9927 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/engine_client/types/query.py
+-rw-r--r--   0        0        0      926 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/indexer_client/__init__.py
+-rw-r--r--   0        0        0    11793 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/indexer_client/query.py
+-rw-r--r--   0        0        0     3077 2023-08-08 03:56:13.245868 vertex_protocol-1.1.7/vertex_protocol/indexer_client/types/__init__.py
+-rw-r--r--   0        0        0     5656 2023-08-08 03:56:13.249868 vertex_protocol-1.1.7/vertex_protocol/indexer_client/types/models.py
+-rw-r--r--   0        0        0    12832 2023-08-08 03:56:13.249868 vertex_protocol-1.1.7/vertex_protocol/indexer_client/types/query.py
+-rw-r--r--   0        0        0      933 2023-08-08 03:56:13.249868 vertex_protocol-1.1.7/vertex_protocol/utils/__init__.py
+-rw-r--r--   0        0        0      341 2023-08-08 03:56:13.249868 vertex_protocol-1.1.7/vertex_protocol/utils/backend.py
+-rw-r--r--   0        0        0     5301 2023-08-08 03:56:13.249868 vertex_protocol-1.1.7/vertex_protocol/utils/bytes32.py
+-rw-r--r--   0        0        0       99 2023-08-08 03:56:13.249868 vertex_protocol-1.1.7/vertex_protocol/utils/enum.py
+-rw-r--r--   0        0        0     1136 2023-08-08 03:56:13.249868 vertex_protocol-1.1.7/vertex_protocol/utils/exceptions.py
+-rw-r--r--   0        0        0     1094 2023-08-08 03:56:13.249868 vertex_protocol-1.1.7/vertex_protocol/utils/expiration.py
+-rw-r--r--   0        0        0     1290 2023-08-08 03:56:13.249868 vertex_protocol-1.1.7/vertex_protocol/utils/math.py
+-rw-r--r--   0        0        0     2089 2023-08-08 03:56:13.249868 vertex_protocol-1.1.7/vertex_protocol/utils/model.py
+-rw-r--r--   0        0        0      863 2023-08-08 03:56:13.249868 vertex_protocol-1.1.7/vertex_protocol/utils/nonce.py
+-rw-r--r--   0        0        0      503 2023-08-08 03:56:13.249868 vertex_protocol-1.1.7/vertex_protocol/utils/subaccount.py
+-rw-r--r--   0        0        0     4119 1970-01-01 00:00:00.000000 vertex_protocol-1.1.7/PKG-INFO
```

### Comparing `vertex_protocol-1.1.6/README.md` & `vertex_protocol-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/pyproject.toml` & `vertex_protocol-1.1.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vertex-protocol"
-version = "1.1.6"
+version = "1.1.7"
 description = "Vertex Protocol SDK"
 authors = ["Jeury Mejia <jeury@vertexprotocol.com>"]
 homepage = "https://vertexprotocol.com/"
 maintainers = [
   "Frank Jia <frank@vertexprotocol.com>",
   "Clark Oh-Willeke <clark@vertexprotocol.com>"
 ]
@@ -42,15 +42,14 @@
 client-sanity = "sanity.vertex_client:run"
 
 [[tool.poetry.source]]
 name = "private"
 url = "https://github.com/vertex-protocol/vertex-python-sdk"
 priority = "primary"
 
-
 [[tool.poetry.source]]
 name = "PyPI"
 priority = "primary"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `vertex_protocol-1.1.6/vertex_protocol/client/__init__.py` & `vertex_protocol-1.1.7/vertex_protocol/client/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/client/apis/__init__.py` & `vertex_protocol-1.1.7/vertex_protocol/client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/client/apis/base.py` & `vertex_protocol-1.1.7/vertex_protocol/client/apis/base.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/client/apis/market/__init__.py` & `vertex_protocol-1.1.7/vertex_protocol/client/apis/market/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/client/apis/market/execute.py` & `vertex_protocol-1.1.7/vertex_protocol/client/apis/market/execute.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from vertex_protocol.engine_client.types.execute import (
     BurnLpParams,
     CancelOrdersParams,
     CancelProductOrdersParams,
     ExecuteResponse,
     MintLpParams,
-    PlaceOrderParams, CancelOrdersResponse,
+    PlaceOrderParams,
+    CancelOrdersResponse,
 )
 from vertex_protocol.client.apis.base import VertexBaseAPI
+from vertex_protocol.utils.subaccount import Subaccount
 
 
 class MarketExecuteAPI(VertexBaseAPI):
     """
     Provides functionality to interact with the Vertex's market execution APIs.
     This class contains methods that allow clients to execute operations such as minting LP tokens, burning LP tokens,
     placing and cancelling orders on the Vertex market.
@@ -79,22 +81,40 @@
 
         Raises:
             Exception: If there is an error during the execution or the response status is not "success".
         """
         return self.context.engine_client.cancel_orders(params)
 
     def cancel_product_orders(
-            self, params: CancelProductOrdersParams
+        self, params: CancelProductOrdersParams
     ) -> ExecuteResponse:
         """
         Cancels all orders for provided products through the engine.
 
         Args:
             params (CancelProductOrdersParams): Parameters required to cancel product orders.
 
         Returns:
             CancelOrdersResponse: A data class object containing information about the canceled product orders.
 
         Raises:
             Exception: If there is an error during the execution or the response status is not "success".
         """
         return self.context.engine_client.cancel_product_orders(params)
+
+    def close_position(
+        self, subaccount: Subaccount, product_id: int
+    ) -> ExecuteResponse:
+        """
+        Places an order through the engine to close a position for the provided `product_id`.
+
+        Attributes:
+            subaccount (Subaccount): The subaccount to close position for.
+            product_id (int): The ID of the product to close position for.
+
+         Returns:
+            ExecuteResponse: The response from the engine execution.
+
+        Raises:
+            Exception: If there is an error during the execution or the response status is not "success".
+        """
+        return self.context.engine_client.close_position(subaccount, product_id)
```

### Comparing `vertex_protocol-1.1.6/vertex_protocol/client/apis/market/query.py` & `vertex_protocol-1.1.7/vertex_protocol/client/apis/market/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/client/apis/perp/__init__.py` & `vertex_protocol-1.1.7/vertex_protocol/client/apis/perp/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/client/apis/perp/query.py` & `vertex_protocol-1.1.7/vertex_protocol/client/apis/perp/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/client/apis/spot/__init__.py` & `vertex_protocol-1.1.7/vertex_protocol/client/apis/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/client/apis/spot/base.py` & `vertex_protocol-1.1.7/vertex_protocol/client/apis/spot/base.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/client/apis/spot/execute.py` & `vertex_protocol-1.1.7/vertex_protocol/client/apis/spot/execute.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/client/apis/spot/query.py` & `vertex_protocol-1.1.7/vertex_protocol/client/apis/spot/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/client/apis/subaccount/__init__.py` & `vertex_protocol-1.1.7/vertex_protocol/client/apis/subaccount/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/client/apis/subaccount/execute.py` & `vertex_protocol-1.1.7/vertex_protocol/client/apis/subaccount/execute.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/client/apis/subaccount/query.py` & `vertex_protocol-1.1.7/vertex_protocol/client/apis/subaccount/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/client/context.py` & `vertex_protocol-1.1.7/vertex_protocol/client/context.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/contracts/__init__.py` & `vertex_protocol-1.1.7/vertex_protocol/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/contracts/abis/Endpoint.json` & `vertex_protocol-1.1.7/vertex_protocol/contracts/abis/Endpoint.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/contracts/abis/FQuerier.json` & `vertex_protocol-1.1.7/vertex_protocol/contracts/abis/FQuerier.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/contracts/abis/IClearinghouse.json` & `vertex_protocol-1.1.7/vertex_protocol/contracts/abis/IClearinghouse.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/contracts/abis/IERC20.json` & `vertex_protocol-1.1.7/vertex_protocol/contracts/abis/IERC20.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/contracts/abis/IEndpoint.json` & `vertex_protocol-1.1.7/vertex_protocol/contracts/abis/IEndpoint.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/contracts/abis/IOffchainBook.json` & `vertex_protocol-1.1.7/vertex_protocol/contracts/abis/IOffchainBook.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/contracts/abis/IPerpEngine.json` & `vertex_protocol-1.1.7/vertex_protocol/contracts/abis/IPerpEngine.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/contracts/abis/IProductEngine.json` & `vertex_protocol-1.1.7/vertex_protocol/contracts/abis/IProductEngine.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/contracts/abis/ISpotEngine.json` & `vertex_protocol-1.1.7/vertex_protocol/contracts/abis/ISpotEngine.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/contracts/abis/MockERC20.json` & `vertex_protocol-1.1.7/vertex_protocol/contracts/abis/MockERC20.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/contracts/deployments/deployment.arbitrumGoerli.json` & `vertex_protocol-1.1.7/vertex_protocol/contracts/deployments/deployment.arbitrumGoerli.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/contracts/deployments/deployment.arbitrumOne.json` & `vertex_protocol-1.1.7/vertex_protocol/contracts/deployments/deployment.arbitrumOne.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/contracts/deployments/deployment.test.json` & `vertex_protocol-1.1.7/vertex_protocol/contracts/deployments/deployment.test.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/contracts/eip712/domain.py` & `vertex_protocol-1.1.7/vertex_protocol/contracts/eip712/domain.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/contracts/eip712/sign.py` & `vertex_protocol-1.1.7/vertex_protocol/contracts/eip712/sign.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/contracts/eip712/types.py` & `vertex_protocol-1.1.7/vertex_protocol/contracts/eip712/types.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/contracts/loader.py` & `vertex_protocol-1.1.7/vertex_protocol/contracts/loader.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/contracts/types.py` & `vertex_protocol-1.1.7/vertex_protocol/contracts/types.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/engine_client/__init__.py` & `vertex_protocol-1.1.7/vertex_protocol/engine_client/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/engine_client/execute.py` & `vertex_protocol-1.1.7/vertex_protocol/engine_client/execute.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from copy import deepcopy
+import time
 import requests
 from functools import singledispatchmethod
 
 from typing import Optional, Type, Union
 from eth_account.signers.local import LocalAccount
 from vertex_protocol.contracts.eip712.sign import (
     get_eip712_typed_data_digest,
@@ -27,26 +28,29 @@
     OrderParams,
     PlaceOrderParams,
     WithdrawCollateralParams,
     to_execute_request,
     CancelOrdersResponse,
 )
 from vertex_protocol.contracts.types import VertexExecuteType
+from vertex_protocol.utils.bytes32 import subaccount_to_hex
 
 from vertex_protocol.utils.exceptions import (
     BadStatusCodeException,
     ExecuteFailedException,
 )
+from vertex_protocol.utils.expiration import OrderType, get_expiration_timestamp
+from vertex_protocol.utils.math import mul_x18, round_x18, to_x18
 from vertex_protocol.utils.model import (
     VertexBaseModel,
     is_instance_of_union,
     ensure_data_type,
 )
 from vertex_protocol.utils.nonce import gen_order_nonce
-from vertex_protocol.utils.subaccount import SubaccountParams
+from vertex_protocol.utils.subaccount import Subaccount, SubaccountParams
 
 
 class EngineExecuteClient:
     """
     Client class for executing operations against the off-chain engine.
     """
 
@@ -116,16 +120,17 @@
             recv_time_ms (int, optional): Received time in milliseconds.
 
         Returns:
             int: The generated order nonce.
         """
         return gen_order_nonce(recv_time_ms)
 
-    def prepare_execute_params(self, params: Type[BaseParams], use_order_nonce: bool) -> Type[
-        BaseParams]:  # type: ignore
+    def prepare_execute_params(
+        self, params: Type[BaseParams], use_order_nonce: bool
+    ) -> Type[BaseParams]:  # type: ignore
         """
         Prepares the parameters for execution by ensuring that both owner and nonce are correctly set.
 
         Args:
             params (Type[BaseParams]): The original parameters.
 
         Returns:
@@ -528,7 +533,62 @@
         """
         params = self.prepare_execute_params(LinkSignerParams.parse_obj(params), False)  # type: ignore
         params.signature = params.signature or self._sign(
             VertexExecuteType.LINK_SIGNER,
             params.dict(),
         )
         return self.execute(params)
+
+    def close_position(
+        self, subaccount: Subaccount, product_id: int
+    ) -> ExecuteResponse:
+        """
+        Execute a place order operation to close a position for the provided `product_id`.
+
+        Attributes:
+            subaccount (Subaccount): The subaccount to close position for.
+            product_id (int): The ID of the product to close position for.
+
+        Returns:
+            ExecuteResponse: Response of the execution, including status and potential error message.
+        """
+        subaccount = subaccount_to_hex(subaccount)
+        summary = self._querier.get_subaccount_info(subaccount)
+        try:
+            balance = [
+                balance
+                for balance in summary.spot_balances + summary.perp_balances
+                if balance.product_id == product_id
+            ][0]
+            product = [
+                product
+                for product in summary.spot_products + summary.perp_products
+                if product.product_id == product_id
+            ][0]
+        except Exception as e:
+            raise Exception(f"Invalid product id provided {product_id}. Error: {e}")
+        closing_spread_x18 = to_x18(0.005)
+        closing_price_x18 = (
+            mul_x18(product.oracle_price_x18, to_x18(1) - closing_spread_x18)
+            if int(balance.balance.amount) > 0
+            else mul_x18(product.oracle_price_x18, to_x18(1) + closing_spread_x18)
+        )
+        return self.place_order(
+            PlaceOrderParams(  # type: ignore
+                product_id=product_id,
+                order=OrderParams(  # type: ignore
+                    sender=subaccount,
+                    amount=-round_x18(
+                        balance.balance.amount,
+                        product.book_info.size_increment,
+                    ),
+                    priceX18=round_x18(
+                        closing_price_x18,
+                        product.book_info.price_increment_x18,
+                    ),
+                    expiration=get_expiration_timestamp(
+                        OrderType.FOK,
+                        int(time.time()) + 1000,
+                    ),
+                ),
+            )
+        )
```

### Comparing `vertex_protocol-1.1.6/vertex_protocol/engine_client/query.py` & `vertex_protocol-1.1.7/vertex_protocol/engine_client/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/engine_client/types/__init__.py` & `vertex_protocol-1.1.7/vertex_protocol/engine_client/types/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/engine_client/types/execute.py` & `vertex_protocol-1.1.7/vertex_protocol/engine_client/types/execute.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/engine_client/types/models.py` & `vertex_protocol-1.1.7/vertex_protocol/engine_client/types/models.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/engine_client/types/query.py` & `vertex_protocol-1.1.7/vertex_protocol/engine_client/types/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/indexer_client/__init__.py` & `vertex_protocol-1.1.7/vertex_protocol/indexer_client/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/indexer_client/query.py` & `vertex_protocol-1.1.7/vertex_protocol/indexer_client/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/indexer_client/types/__init__.py` & `vertex_protocol-1.1.7/vertex_protocol/indexer_client/types/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/indexer_client/types/models.py` & `vertex_protocol-1.1.7/vertex_protocol/indexer_client/types/models.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/indexer_client/types/query.py` & `vertex_protocol-1.1.7/vertex_protocol/indexer_client/types/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/utils/__init__.py` & `vertex_protocol-1.1.7/vertex_protocol/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/utils/bytes32.py` & `vertex_protocol-1.1.7/vertex_protocol/utils/bytes32.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/utils/exceptions.py` & `vertex_protocol-1.1.7/vertex_protocol/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/utils/expiration.py` & `vertex_protocol-1.1.7/vertex_protocol/utils/expiration.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/utils/model.py` & `vertex_protocol-1.1.7/vertex_protocol/utils/model.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/vertex_protocol/utils/nonce.py` & `vertex_protocol-1.1.7/vertex_protocol/utils/nonce.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.6/PKG-INFO` & `vertex_protocol-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vertex-protocol
-Version: 1.1.6
+Version: 1.1.7
 Summary: Vertex Protocol SDK
 Home-page: https://vertexprotocol.com/
 Keywords: vertex protocol,vertex sdk,vertex protocol api
 Author: Jeury Mejia
 Author-email: jeury@vertexprotocol.com
 Maintainer: Frank Jia
 Maintainer-email: frank@vertexprotocol.com
```

