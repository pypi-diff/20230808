# Comparing `tmp/langflow-0.4.3.tar.gz` & `tmp/langflow-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langflow-0.4.3.tar", max compression
+gzip compressed data, was "langflow-0.4.4.tar", max compression
```

## Comparing `langflow-0.4.3.tar` & `langflow-0.4.4.tar`

### file list

```diff
@@ -1,160 +1,160 @@
--rw-r--r--   0        0        0     1065 2023-08-08 18:14:45.130529 langflow-0.4.3/LICENSE
--rw-r--r--   0        0        0    15764 2023-08-08 18:14:45.130529 langflow-0.4.3/README.md
--rw-r--r--   0        0        0     3072 2023-08-08 18:14:45.578527 langflow-0.4.3/pyproject.toml
--rw-r--r--   0        0        0      514 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/__init__.py
--rw-r--r--   0        0        0     9339 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/__main__.py
--rw-r--r--   0        0        0       61 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/api/__init__.py
--rw-r--r--   0        0        0      485 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/api/router.py
--rw-r--r--   0        0        0     3203 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/api/utils.py
--rw-r--r--   0        0        0      526 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/api/v1/__init__.py
--rw-r--r--   0        0        0     4486 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/api/v1/base.py
--rw-r--r--   0        0        0     4979 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/api/v1/callback.py
--rw-r--r--   0        0        0     7302 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/api/v1/chat.py
--rw-r--r--   0        0        0     2534 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/api/v1/components.py
--rw-r--r--   0        0        0     4429 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/api/v1/endpoints.py
--rw-r--r--   0        0        0     2691 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/api/v1/flow_styles.py
--rw-r--r--   0        0        0     3868 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/api/v1/flows.py
--rw-r--r--   0        0        0     2625 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/api/v1/schemas.py
--rw-r--r--   0        0        0     4439 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/api/v1/validate.py
--rw-r--r--   0        0        0      152 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/cache/__init__.py
--rw-r--r--   0        0        0     1815 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/cache/base.py
--rw-r--r--   0        0        0     4554 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/cache/flow.py
--rw-r--r--   0        0        0     4481 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/cache/manager.py
--rw-r--r--   0        0        0     5062 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/cache/utils.py
--rw-r--r--   0        0        0        0 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/chat/__init__.py
--rw-r--r--   0        0        0       45 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/chat/config.py
--rw-r--r--   0        0        0     8554 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/chat/manager.py
--rw-r--r--   0        0        0     1261 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/chat/utils.py
--rw-r--r--   0        0        0      103 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/components/__init__.py
--rw-r--r--   0        0        0        0 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/components/chains/__init__.py
--rw-r--r--   0        0        0     1003 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/components/chains/prompt_runner.py
--rw-r--r--   0        0        0    13474 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/config.yaml
--rw-r--r--   0        0        0        0 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/custom/__init__.py
--rw-r--r--   0        0        0     1733 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/custom/customs.py
--rw-r--r--   0        0        0        0 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/database/__init__.py
--rw-r--r--   0        0        0     2387 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/database/base.py
--rw-r--r--   0        0        0        0 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/database/models/__init__.py
--rw-r--r--   0        0        0      363 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/database/models/base.py
--rw-r--r--   0        0        0     1120 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/database/models/component.py
--rw-r--r--   0        0        0     1705 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/database/models/flow.py
--rw-r--r--   0        0        0      831 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/database/models/flow_style.py
--rw-r--r--   0        0        0   206379 2023-08-08 18:15:45.098354 langflow-0.4.3/src/backend/langflow/frontend/assets/index-c3be492f.css
--rw-r--r--   0        0        0  4229777 2023-08-08 18:15:45.102354 langflow-0.4.3/src/backend/langflow/frontend/assets/index-c9011122.js
--rw-r--r--   0        0        0    23161 2023-08-08 18:15:45.098354 langflow-0.4.3/src/backend/langflow/frontend/assets/male-technologist-d2e7de57.png
--rw-r--r--   0        0        0    26806 2023-08-08 18:15:45.098354 langflow-0.4.3/src/backend/langflow/frontend/assets/robot-95e1b00d.png
--rw-r--r--   0        0        0     4310 2023-08-08 18:15:45.098354 langflow-0.4.3/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js
--rw-r--r--   0        0        0   104188 2023-08-08 18:15:45.098354 langflow-0.4.3/src/backend/langflow/frontend/favicon.ico
--rw-r--r--   0        0        0      724 2023-08-08 18:15:45.102354 langflow-0.4.3/src/backend/langflow/frontend/index.html
--rw-r--r--   0        0        0      764 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/graph/__init__.py
--rw-r--r--   0        0        0        0 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/graph/edge/__init__.py
--rw-r--r--   0        0        0     2349 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/graph/edge/base.py
--rw-r--r--   0        0        0        0 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/graph/graph/__init__.py
--rw-r--r--   0        0        0     7854 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/graph/graph/base.py
--rw-r--r--   0        0        0     2165 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/graph/graph/constants.py
--rw-r--r--   0        0        0        0 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/graph/graph/utils.py
--rw-r--r--   0        0        0      642 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/graph/utils.py
--rw-r--r--   0        0        0        0 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/graph/vertex/__init__.py
--rw-r--r--   0        0        0    10167 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/graph/vertex/base.py
--rw-r--r--   0        0        0        1 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/graph/vertex/constants.py
--rw-r--r--   0        0        0     8689 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/graph/vertex/types.py
--rw-r--r--   0        0        0        0 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/interface/__init__.py
--rw-r--r--   0        0        0       84 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/interface/agents/__init__.py
--rw-r--r--   0        0        0     2423 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/interface/agents/base.py
--rw-r--r--   0        0        0    10224 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/interface/agents/custom.py
--rw-r--r--   0        0        0     1447 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/interface/agents/prebuilt.py
--rw-r--r--   0        0        0     4690 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/interface/base.py
--rw-r--r--   0        0        0       84 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/interface/chains/__init__.py
--rw-r--r--   0        0        0     3006 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/interface/chains/base.py
--rw-r--r--   0        0        0     4843 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/interface/chains/custom.py
--rw-r--r--   0        0        0      194 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/interface/custom/__init__.py
--rw-r--r--   0        0        0     1594 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/interface/custom/base.py
--rw-r--r--   0        0        0     8937 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/interface/custom/code_parser.py
--rw-r--r--   0        0        0     2122 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/interface/custom/component.py
--rw-r--r--   0        0        0     1788 2023-08-08 18:14:45.578527 langflow-0.4.3/src/backend/langflow/interface/custom/constants.py
--rw-r--r--   0        0        0     6572 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/custom/custom_component.py
--rw-r--r--   0        0        0     9279 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/custom/directory_reader.py
--rw-r--r--   0        0        0      529 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/custom/schema.py
--rw-r--r--   0        0        0     2306 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/custom_lists.py
--rw-r--r--   0        0        0        0 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/document_loaders/__init__.py
--rw-r--r--   0        0        0     1479 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/document_loaders/base.py
--rw-r--r--   0        0        0        0 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/embeddings/__init__.py
--rw-r--r--   0        0        0     1445 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/embeddings/base.py
--rw-r--r--   0        0        0      171 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/importing/__init__.py
--rw-r--r--   0        0        0     6105 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/importing/utils.py
--rw-r--r--   0        0        0        0 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/initialize/__init__.py
--rw-r--r--   0        0        0      385 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/initialize/llm.py
--rw-r--r--   0        0        0    18948 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/initialize/loading.py
--rw-r--r--   0        0        0     3772 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/initialize/utils.py
--rw-r--r--   0        0        0     8362 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/initialize/vector_store.py
--rw-r--r--   0        0        0     2048 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/listing.py
--rw-r--r--   0        0        0       78 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/llms/__init__.py
--rw-r--r--   0        0        0     1355 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/llms/base.py
--rw-r--r--   0        0        0       88 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/memories/__init__.py
--rw-r--r--   0        0        0     2135 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/memories/base.py
--rw-r--r--   0        0        0        0 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/output_parsers/__init__.py
--rw-r--r--   0        0        0     2355 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/output_parsers/base.py
--rw-r--r--   0        0        0       87 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/prompts/__init__.py
--rw-r--r--   0        0        0     2459 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/prompts/base.py
--rw-r--r--   0        0        0     2483 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/prompts/custom.py
--rw-r--r--   0        0        0        0 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/retrievers/__init__.py
--rw-r--r--   0        0        0     2086 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/retrievers/base.py
--rw-r--r--   0        0        0     2764 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/run.py
--rw-r--r--   0        0        0      106 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/text_splitters/__init__.py
--rw-r--r--   0        0        0     1450 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/text_splitters/base.py
--rw-r--r--   0        0        0        0 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/toolkits/__init__.py
--rw-r--r--   0        0        0     2598 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/toolkits/base.py
--rw-r--r--   0        0        0        0 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/toolkits/custom.py
--rw-r--r--   0        0        0       81 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/tools/__init__.py
--rw-r--r--   0        0        0     5418 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/tools/base.py
--rw-r--r--   0        0        0      913 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/tools/constants.py
--rw-r--r--   0        0        0     1269 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/tools/custom.py
--rw-r--r--   0        0        0     4328 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/tools/util.py
--rw-r--r--   0        0        0    14787 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/types.py
--rw-r--r--   0        0        0        0 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/utilities/__init__.py
--rw-r--r--   0        0        0     2294 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/utilities/base.py
--rw-r--r--   0        0        0     2645 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/utils.py
--rw-r--r--   0        0        0        0 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/vector_store/__init__.py
--rw-r--r--   0        0        0     1813 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/vector_store/base.py
--rw-r--r--   0        0        0        0 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/wrappers/__init__.py
--rw-r--r--   0        0        0     1500 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/interface/wrappers/base.py
--rw-r--r--   0        0        0       29 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/jcloud.yml
--rw-r--r--   0        0        0      428 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/lcserve.py
--rw-r--r--   0        0        0     2556 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/main.py
--rw-r--r--   0        0        0        0 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/processing/__init__.py
--rw-r--r--   0        0        0     2013 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/processing/base.py
--rw-r--r--   0        0        0     8650 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/processing/process.py
--rw-r--r--   0        0        0      579 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/server.py
--rw-r--r--   0        0        0     6451 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/settings.py
--rw-r--r--   0        0        0        0 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/template/__init__.py
--rw-r--r--   0        0        0        0 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/template/field/__init__.py
--rw-r--r--   0        0        0     2571 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/template/field/base.py
--rw-r--r--   0        0        0      423 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/template/frontend_node/__init__.py
--rw-r--r--   0        0        0     7033 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/template/frontend_node/agents.py
--rw-r--r--   0        0        0     9840 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/template/frontend_node/base.py
--rw-r--r--   0        0        0     7796 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/template/frontend_node/chains.py
--rw-r--r--   0        0        0     1694 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/template/frontend_node/constants.py
--rw-r--r--   0        0        0      998 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/template/frontend_node/custom_components.py
--rw-r--r--   0        0        0     8636 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/template/frontend_node/documentloaders.py
--rw-r--r--   0        0        0     1680 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/template/frontend_node/embeddings.py
--rw-r--r--   0        0        0        0 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/template/frontend_node/formatter/__init__.py
--rw-r--r--   0        0        0      297 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/template/frontend_node/formatter/base.py
--rw-r--r--   0        0        0     5569 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/template/frontend_node/formatter/field_formatters.py
--rw-r--r--   0        0        0     5370 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/template/frontend_node/llms.py
--rw-r--r--   0        0        0     6559 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/template/frontend_node/memories.py
--rw-r--r--   0        0        0      364 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/template/frontend_node/output_parsers.py
--rw-r--r--   0        0        0     3540 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/template/frontend_node/prompts.py
--rw-r--r--   0        0        0      523 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/template/frontend_node/retrievers.py
--rw-r--r--   0        0        0     2355 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/template/frontend_node/textsplitters.py
--rw-r--r--   0        0        0     4016 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/template/frontend_node/tools.py
--rw-r--r--   0        0        0     1029 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/template/frontend_node/utilities.py
--rw-r--r--   0        0        0    11001 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/template/frontend_node/vectorstores.py
--rw-r--r--   0        0        0        0 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/template/template/__init__.py
--rw-r--r--   0        0        0     1181 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/template/template/base.py
--rw-r--r--   0        0        0        0 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/utils/__init__.py
--rw-r--r--   0        0        0     1792 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/utils/constants.py
--rw-r--r--   0        0        0      915 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/utils/logger.py
--rw-r--r--   0        0        0     3169 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/utils/payload.py
--rw-r--r--   0        0        0       23 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/utils/types.py
--rw-r--r--   0        0        0    13928 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/utils/util.py
--rw-r--r--   0        0        0     7665 2023-08-08 18:14:45.582527 langflow-0.4.3/src/backend/langflow/utils/validate.py
--rw-r--r--   0        0        0    18838 1970-01-01 00:00:00.000000 langflow-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-08 19:56:05.003479 langflow-0.4.4/LICENSE
+-rw-r--r--   0        0        0    15764 2023-08-08 19:56:05.003479 langflow-0.4.4/README.md
+-rw-r--r--   0        0        0     3072 2023-08-08 19:56:05.411483 langflow-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0      514 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/__init__.py
+-rw-r--r--   0        0        0     9339 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/__main__.py
+-rw-r--r--   0        0        0       61 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/api/__init__.py
+-rw-r--r--   0        0        0      485 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/api/router.py
+-rw-r--r--   0        0        0     3203 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/api/utils.py
+-rw-r--r--   0        0        0      526 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/api/v1/__init__.py
+-rw-r--r--   0        0        0     4486 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/api/v1/base.py
+-rw-r--r--   0        0        0     4979 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/api/v1/callback.py
+-rw-r--r--   0        0        0     7302 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/api/v1/chat.py
+-rw-r--r--   0        0        0     2534 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/api/v1/components.py
+-rw-r--r--   0        0        0     4429 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/api/v1/endpoints.py
+-rw-r--r--   0        0        0     2691 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/api/v1/flow_styles.py
+-rw-r--r--   0        0        0     3868 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/api/v1/flows.py
+-rw-r--r--   0        0        0     2625 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/api/v1/schemas.py
+-rw-r--r--   0        0        0     4439 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/api/v1/validate.py
+-rw-r--r--   0        0        0      152 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/cache/__init__.py
+-rw-r--r--   0        0        0     1815 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/cache/base.py
+-rw-r--r--   0        0        0     4554 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/cache/flow.py
+-rw-r--r--   0        0        0     4481 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/cache/manager.py
+-rw-r--r--   0        0        0     5062 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/cache/utils.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/chat/__init__.py
+-rw-r--r--   0        0        0       45 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/chat/config.py
+-rw-r--r--   0        0        0     8554 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/chat/manager.py
+-rw-r--r--   0        0        0     1261 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/chat/utils.py
+-rw-r--r--   0        0        0      103 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/components/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/components/chains/__init__.py
+-rw-r--r--   0        0        0     1003 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/components/chains/prompt_runner.py
+-rw-r--r--   0        0        0    13474 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/config.yaml
+-rw-r--r--   0        0        0        0 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/custom/__init__.py
+-rw-r--r--   0        0        0     1733 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/custom/customs.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/database/__init__.py
+-rw-r--r--   0        0        0     2387 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/database/base.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/database/models/__init__.py
+-rw-r--r--   0        0        0      363 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/database/models/base.py
+-rw-r--r--   0        0        0     1120 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/database/models/component.py
+-rw-r--r--   0        0        0     1705 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/database/models/flow.py
+-rw-r--r--   0        0        0      831 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/database/models/flow_style.py
+-rw-r--r--   0        0        0   206379 2023-08-08 19:57:10.992282 langflow-0.4.4/src/backend/langflow/frontend/assets/index-c3be492f.css
+-rw-r--r--   0        0        0  4229777 2023-08-08 19:57:10.992282 langflow-0.4.4/src/backend/langflow/frontend/assets/index-c9011122.js
+-rw-r--r--   0        0        0    23161 2023-08-08 19:57:10.992282 langflow-0.4.4/src/backend/langflow/frontend/assets/male-technologist-d2e7de57.png
+-rw-r--r--   0        0        0    26806 2023-08-08 19:57:10.992282 langflow-0.4.4/src/backend/langflow/frontend/assets/robot-95e1b00d.png
+-rw-r--r--   0        0        0     4310 2023-08-08 19:57:10.992282 langflow-0.4.4/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js
+-rw-r--r--   0        0        0   104188 2023-08-08 19:57:10.988282 langflow-0.4.4/src/backend/langflow/frontend/favicon.ico
+-rw-r--r--   0        0        0      724 2023-08-08 19:57:10.992282 langflow-0.4.4/src/backend/langflow/frontend/index.html
+-rw-r--r--   0        0        0      764 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/graph/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/graph/edge/__init__.py
+-rw-r--r--   0        0        0     2349 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/graph/edge/base.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/graph/graph/__init__.py
+-rw-r--r--   0        0        0     7854 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/graph/graph/base.py
+-rw-r--r--   0        0        0     2165 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/graph/graph/constants.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/graph/graph/utils.py
+-rw-r--r--   0        0        0      642 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/graph/utils.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/graph/vertex/__init__.py
+-rw-r--r--   0        0        0    10167 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/graph/vertex/base.py
+-rw-r--r--   0        0        0        1 2023-08-08 19:56:05.411483 langflow-0.4.4/src/backend/langflow/graph/vertex/constants.py
+-rw-r--r--   0        0        0     8689 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/graph/vertex/types.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/__init__.py
+-rw-r--r--   0        0        0       84 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/agents/__init__.py
+-rw-r--r--   0        0        0     2423 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/agents/base.py
+-rw-r--r--   0        0        0    10224 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/agents/custom.py
+-rw-r--r--   0        0        0     1447 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/agents/prebuilt.py
+-rw-r--r--   0        0        0     4690 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/base.py
+-rw-r--r--   0        0        0       84 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/chains/__init__.py
+-rw-r--r--   0        0        0     3006 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/chains/base.py
+-rw-r--r--   0        0        0     4843 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/chains/custom.py
+-rw-r--r--   0        0        0      194 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/custom/__init__.py
+-rw-r--r--   0        0        0     1594 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/custom/base.py
+-rw-r--r--   0        0        0     8937 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/custom/code_parser.py
+-rw-r--r--   0        0        0     2122 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/custom/component.py
+-rw-r--r--   0        0        0     1788 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/custom/constants.py
+-rw-r--r--   0        0        0     6572 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/custom/custom_component.py
+-rw-r--r--   0        0        0     9279 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/custom/directory_reader.py
+-rw-r--r--   0        0        0      529 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/custom/schema.py
+-rw-r--r--   0        0        0     2306 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/custom_lists.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/document_loaders/__init__.py
+-rw-r--r--   0        0        0     1479 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/document_loaders/base.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/embeddings/__init__.py
+-rw-r--r--   0        0        0     1445 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/embeddings/base.py
+-rw-r--r--   0        0        0      171 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/importing/__init__.py
+-rw-r--r--   0        0        0     6105 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/importing/utils.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/initialize/__init__.py
+-rw-r--r--   0        0        0      385 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/initialize/llm.py
+-rw-r--r--   0        0        0    18948 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/initialize/loading.py
+-rw-r--r--   0        0        0     3772 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/initialize/utils.py
+-rw-r--r--   0        0        0     8362 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/initialize/vector_store.py
+-rw-r--r--   0        0        0     2048 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/listing.py
+-rw-r--r--   0        0        0       78 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/llms/__init__.py
+-rw-r--r--   0        0        0     1355 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/llms/base.py
+-rw-r--r--   0        0        0       88 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/memories/__init__.py
+-rw-r--r--   0        0        0     2135 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/memories/base.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/output_parsers/__init__.py
+-rw-r--r--   0        0        0     2355 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/output_parsers/base.py
+-rw-r--r--   0        0        0       87 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/prompts/__init__.py
+-rw-r--r--   0        0        0     2459 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/prompts/base.py
+-rw-r--r--   0        0        0     2483 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/prompts/custom.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/retrievers/__init__.py
+-rw-r--r--   0        0        0     2086 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/retrievers/base.py
+-rw-r--r--   0        0        0     2764 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/run.py
+-rw-r--r--   0        0        0      106 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/text_splitters/__init__.py
+-rw-r--r--   0        0        0     1450 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/text_splitters/base.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/toolkits/__init__.py
+-rw-r--r--   0        0        0     2598 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/toolkits/base.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/toolkits/custom.py
+-rw-r--r--   0        0        0       81 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/tools/__init__.py
+-rw-r--r--   0        0        0     5418 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/tools/base.py
+-rw-r--r--   0        0        0      913 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/tools/constants.py
+-rw-r--r--   0        0        0     1269 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/tools/custom.py
+-rw-r--r--   0        0        0     4328 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/tools/util.py
+-rw-r--r--   0        0        0    14787 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/types.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/utilities/__init__.py
+-rw-r--r--   0        0        0     2294 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/utilities/base.py
+-rw-r--r--   0        0        0     2645 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/utils.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/vector_store/__init__.py
+-rw-r--r--   0        0        0     1813 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/vector_store/base.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/wrappers/__init__.py
+-rw-r--r--   0        0        0     1500 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/interface/wrappers/base.py
+-rw-r--r--   0        0        0       29 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/jcloud.yml
+-rw-r--r--   0        0        0      428 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/lcserve.py
+-rw-r--r--   0        0        0     2556 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/main.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/processing/__init__.py
+-rw-r--r--   0        0        0     2013 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/processing/base.py
+-rw-r--r--   0        0        0     8650 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/processing/process.py
+-rw-r--r--   0        0        0      579 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/server.py
+-rw-r--r--   0        0        0     6451 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/settings.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/template/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/template/field/__init__.py
+-rw-r--r--   0        0        0     2571 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/template/field/base.py
+-rw-r--r--   0        0        0      423 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/template/frontend_node/__init__.py
+-rw-r--r--   0        0        0     7033 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/template/frontend_node/agents.py
+-rw-r--r--   0        0        0     9840 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/template/frontend_node/base.py
+-rw-r--r--   0        0        0     7796 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/template/frontend_node/chains.py
+-rw-r--r--   0        0        0     1694 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/template/frontend_node/constants.py
+-rw-r--r--   0        0        0      998 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/template/frontend_node/custom_components.py
+-rw-r--r--   0        0        0     8636 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/template/frontend_node/documentloaders.py
+-rw-r--r--   0        0        0     1680 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/template/frontend_node/embeddings.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/template/frontend_node/formatter/__init__.py
+-rw-r--r--   0        0        0      297 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/template/frontend_node/formatter/base.py
+-rw-r--r--   0        0        0     5569 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/template/frontend_node/formatter/field_formatters.py
+-rw-r--r--   0        0        0     5370 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/template/frontend_node/llms.py
+-rw-r--r--   0        0        0     6559 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/template/frontend_node/memories.py
+-rw-r--r--   0        0        0      364 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/template/frontend_node/output_parsers.py
+-rw-r--r--   0        0        0     3540 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/template/frontend_node/prompts.py
+-rw-r--r--   0        0        0      523 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/template/frontend_node/retrievers.py
+-rw-r--r--   0        0        0     2355 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/template/frontend_node/textsplitters.py
+-rw-r--r--   0        0        0     4016 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/template/frontend_node/tools.py
+-rw-r--r--   0        0        0     1029 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/template/frontend_node/utilities.py
+-rw-r--r--   0        0        0    11001 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/template/frontend_node/vectorstores.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/template/template/__init__.py
+-rw-r--r--   0        0        0     1181 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/template/template/base.py
+-rw-r--r--   0        0        0        0 2023-08-08 19:56:05.415483 langflow-0.4.4/src/backend/langflow/utils/__init__.py
+-rw-r--r--   0        0        0     1792 2023-08-08 19:56:05.419484 langflow-0.4.4/src/backend/langflow/utils/constants.py
+-rw-r--r--   0        0        0      915 2023-08-08 19:56:05.419484 langflow-0.4.4/src/backend/langflow/utils/logger.py
+-rw-r--r--   0        0        0     3169 2023-08-08 19:56:05.419484 langflow-0.4.4/src/backend/langflow/utils/payload.py
+-rw-r--r--   0        0        0       23 2023-08-08 19:56:05.419484 langflow-0.4.4/src/backend/langflow/utils/types.py
+-rw-r--r--   0        0        0    13928 2023-08-08 19:56:05.419484 langflow-0.4.4/src/backend/langflow/utils/util.py
+-rw-r--r--   0        0        0     7665 2023-08-08 19:56:05.419484 langflow-0.4.4/src/backend/langflow/utils/validate.py
+-rw-r--r--   0        0        0    18831 1970-01-01 00:00:00.000000 langflow-0.4.4/PKG-INFO
```

### Comparing `langflow-0.4.3/LICENSE` & `langflow-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/README.md` & `langflow-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/pyproject.toml` & `langflow-0.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langflow"
-version = "0.4.3"
+version = "0.4.4"
 description = "A Python package with a built-in web application"
 authors = ["Logspace <contact@logspace.ai>"]
 maintainers = [
     "Carlos Coelho <carlos@logspace.ai>",
     "Cristhian Zanforlin <cristhian.lousa@gmail.com>",
     "Gabriel Almeida <gabriel@logspace.ai>",
     "Gustavo Schaedler <gustavopoa@gmail.com>",
@@ -59,15 +59,16 @@
 sentence-transformers = { version = "^2.2.2", optional = true }
 ctransformers = { version = "^0.2.10", optional = true }
 cohere = "^4.11.0"
 python-multipart = "^0.0.6"
 sqlmodel = "^0.0.8"
 faiss-cpu = "^1.7.4"
 anthropic = "^0.3.0"
-orjson = "^3.9.1"
+
+orjson = "3.9.3"
 multiprocess = "^0.70.14"
 cachetools = "^5.3.1"
 types-cachetools = "^5.3.0.5"
 appdirs = "^1.4.4"
 pinecone-client = "^2.2.2"
 supabase = "^1.0.3"
 pymongo = "^4.4.0"
```

### Comparing `langflow-0.4.3/src/backend/langflow/__init__.py` & `langflow-0.4.4/src/backend/langflow/__init__.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/__main__.py` & `langflow-0.4.4/src/backend/langflow/__main__.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/api/utils.py` & `langflow-0.4.4/src/backend/langflow/api/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/api/v1/__init__.py` & `langflow-0.4.4/src/backend/langflow/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/api/v1/base.py` & `langflow-0.4.4/src/backend/langflow/api/v1/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/api/v1/callback.py` & `langflow-0.4.4/src/backend/langflow/api/v1/callback.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/api/v1/chat.py` & `langflow-0.4.4/src/backend/langflow/api/v1/chat.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/api/v1/components.py` & `langflow-0.4.4/src/backend/langflow/api/v1/components.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/api/v1/endpoints.py` & `langflow-0.4.4/src/backend/langflow/api/v1/endpoints.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/api/v1/flow_styles.py` & `langflow-0.4.4/src/backend/langflow/api/v1/flow_styles.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/api/v1/flows.py` & `langflow-0.4.4/src/backend/langflow/api/v1/flows.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/api/v1/schemas.py` & `langflow-0.4.4/src/backend/langflow/api/v1/schemas.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/api/v1/validate.py` & `langflow-0.4.4/src/backend/langflow/api/v1/validate.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/cache/base.py` & `langflow-0.4.4/src/backend/langflow/cache/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/cache/flow.py` & `langflow-0.4.4/src/backend/langflow/cache/flow.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/cache/manager.py` & `langflow-0.4.4/src/backend/langflow/cache/manager.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/cache/utils.py` & `langflow-0.4.4/src/backend/langflow/cache/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/chat/manager.py` & `langflow-0.4.4/src/backend/langflow/chat/manager.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/chat/utils.py` & `langflow-0.4.4/src/backend/langflow/chat/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/components/chains/prompt_runner.py` & `langflow-0.4.4/src/backend/langflow/components/chains/prompt_runner.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/config.yaml` & `langflow-0.4.4/src/backend/langflow/config.yaml`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/custom/customs.py` & `langflow-0.4.4/src/backend/langflow/custom/customs.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/database/base.py` & `langflow-0.4.4/src/backend/langflow/database/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/database/models/component.py` & `langflow-0.4.4/src/backend/langflow/database/models/component.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/database/models/flow.py` & `langflow-0.4.4/src/backend/langflow/database/models/flow.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/database/models/flow_style.py` & `langflow-0.4.4/src/backend/langflow/database/models/flow_style.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/frontend/assets/index-c3be492f.css` & `langflow-0.4.4/src/backend/langflow/frontend/assets/index-c3be492f.css`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/frontend/assets/index-c9011122.js` & `langflow-0.4.4/src/backend/langflow/frontend/assets/index-c9011122.js`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/frontend/assets/male-technologist-d2e7de57.png` & `langflow-0.4.4/src/backend/langflow/frontend/assets/male-technologist-d2e7de57.png`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/frontend/assets/robot-95e1b00d.png` & `langflow-0.4.4/src/backend/langflow/frontend/assets/robot-95e1b00d.png`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js` & `langflow-0.4.4/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/frontend/favicon.ico` & `langflow-0.4.4/src/backend/langflow/frontend/favicon.ico`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/frontend/index.html` & `langflow-0.4.4/src/backend/langflow/frontend/index.html`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/graph/__init__.py` & `langflow-0.4.4/src/backend/langflow/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/graph/edge/base.py` & `langflow-0.4.4/src/backend/langflow/graph/edge/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/graph/graph/base.py` & `langflow-0.4.4/src/backend/langflow/graph/graph/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/graph/graph/constants.py` & `langflow-0.4.4/src/backend/langflow/graph/graph/constants.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/graph/utils.py` & `langflow-0.4.4/src/backend/langflow/graph/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/graph/vertex/base.py` & `langflow-0.4.4/src/backend/langflow/graph/vertex/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/graph/vertex/types.py` & `langflow-0.4.4/src/backend/langflow/graph/vertex/types.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/agents/base.py` & `langflow-0.4.4/src/backend/langflow/interface/agents/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/agents/custom.py` & `langflow-0.4.4/src/backend/langflow/interface/agents/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/agents/prebuilt.py` & `langflow-0.4.4/src/backend/langflow/interface/agents/prebuilt.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/base.py` & `langflow-0.4.4/src/backend/langflow/interface/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/chains/base.py` & `langflow-0.4.4/src/backend/langflow/interface/chains/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/chains/custom.py` & `langflow-0.4.4/src/backend/langflow/interface/chains/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/custom/base.py` & `langflow-0.4.4/src/backend/langflow/interface/custom/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/custom/code_parser.py` & `langflow-0.4.4/src/backend/langflow/interface/custom/code_parser.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/custom/component.py` & `langflow-0.4.4/src/backend/langflow/interface/custom/component.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/custom/constants.py` & `langflow-0.4.4/src/backend/langflow/interface/custom/constants.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/custom/custom_component.py` & `langflow-0.4.4/src/backend/langflow/interface/custom/custom_component.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/custom/directory_reader.py` & `langflow-0.4.4/src/backend/langflow/interface/custom/directory_reader.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/custom/schema.py` & `langflow-0.4.4/src/backend/langflow/interface/custom/schema.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/custom_lists.py` & `langflow-0.4.4/src/backend/langflow/interface/custom_lists.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/document_loaders/base.py` & `langflow-0.4.4/src/backend/langflow/interface/document_loaders/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/embeddings/base.py` & `langflow-0.4.4/src/backend/langflow/interface/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/importing/utils.py` & `langflow-0.4.4/src/backend/langflow/interface/importing/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/initialize/loading.py` & `langflow-0.4.4/src/backend/langflow/interface/initialize/loading.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/initialize/utils.py` & `langflow-0.4.4/src/backend/langflow/interface/initialize/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/initialize/vector_store.py` & `langflow-0.4.4/src/backend/langflow/interface/initialize/vector_store.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/listing.py` & `langflow-0.4.4/src/backend/langflow/interface/listing.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/llms/base.py` & `langflow-0.4.4/src/backend/langflow/interface/llms/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/memories/base.py` & `langflow-0.4.4/src/backend/langflow/interface/memories/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/output_parsers/base.py` & `langflow-0.4.4/src/backend/langflow/interface/output_parsers/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/prompts/base.py` & `langflow-0.4.4/src/backend/langflow/interface/prompts/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/prompts/custom.py` & `langflow-0.4.4/src/backend/langflow/interface/prompts/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/retrievers/base.py` & `langflow-0.4.4/src/backend/langflow/interface/retrievers/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/run.py` & `langflow-0.4.4/src/backend/langflow/interface/run.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/text_splitters/base.py` & `langflow-0.4.4/src/backend/langflow/interface/text_splitters/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/toolkits/base.py` & `langflow-0.4.4/src/backend/langflow/interface/toolkits/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/tools/base.py` & `langflow-0.4.4/src/backend/langflow/interface/tools/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/tools/constants.py` & `langflow-0.4.4/src/backend/langflow/interface/tools/constants.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/tools/custom.py` & `langflow-0.4.4/src/backend/langflow/interface/tools/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/tools/util.py` & `langflow-0.4.4/src/backend/langflow/interface/tools/util.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/types.py` & `langflow-0.4.4/src/backend/langflow/interface/types.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/utilities/base.py` & `langflow-0.4.4/src/backend/langflow/interface/utilities/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/utils.py` & `langflow-0.4.4/src/backend/langflow/interface/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/vector_store/base.py` & `langflow-0.4.4/src/backend/langflow/interface/vector_store/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/interface/wrappers/base.py` & `langflow-0.4.4/src/backend/langflow/interface/wrappers/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/main.py` & `langflow-0.4.4/src/backend/langflow/main.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/processing/base.py` & `langflow-0.4.4/src/backend/langflow/processing/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/processing/process.py` & `langflow-0.4.4/src/backend/langflow/processing/process.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/server.py` & `langflow-0.4.4/src/backend/langflow/server.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/settings.py` & `langflow-0.4.4/src/backend/langflow/settings.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/template/field/base.py` & `langflow-0.4.4/src/backend/langflow/template/field/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/template/frontend_node/agents.py` & `langflow-0.4.4/src/backend/langflow/template/frontend_node/agents.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/template/frontend_node/base.py` & `langflow-0.4.4/src/backend/langflow/template/frontend_node/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/template/frontend_node/chains.py` & `langflow-0.4.4/src/backend/langflow/template/frontend_node/chains.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/template/frontend_node/constants.py` & `langflow-0.4.4/src/backend/langflow/template/frontend_node/constants.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/template/frontend_node/custom_components.py` & `langflow-0.4.4/src/backend/langflow/template/frontend_node/custom_components.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/template/frontend_node/documentloaders.py` & `langflow-0.4.4/src/backend/langflow/template/frontend_node/documentloaders.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/template/frontend_node/embeddings.py` & `langflow-0.4.4/src/backend/langflow/template/frontend_node/embeddings.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/template/frontend_node/formatter/field_formatters.py` & `langflow-0.4.4/src/backend/langflow/template/frontend_node/formatter/field_formatters.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/template/frontend_node/llms.py` & `langflow-0.4.4/src/backend/langflow/template/frontend_node/llms.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/template/frontend_node/memories.py` & `langflow-0.4.4/src/backend/langflow/template/frontend_node/memories.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/template/frontend_node/prompts.py` & `langflow-0.4.4/src/backend/langflow/template/frontend_node/prompts.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/template/frontend_node/retrievers.py` & `langflow-0.4.4/src/backend/langflow/template/frontend_node/retrievers.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/template/frontend_node/textsplitters.py` & `langflow-0.4.4/src/backend/langflow/template/frontend_node/textsplitters.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/template/frontend_node/tools.py` & `langflow-0.4.4/src/backend/langflow/template/frontend_node/tools.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/template/frontend_node/utilities.py` & `langflow-0.4.4/src/backend/langflow/template/frontend_node/utilities.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/template/frontend_node/vectorstores.py` & `langflow-0.4.4/src/backend/langflow/template/frontend_node/vectorstores.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/template/template/base.py` & `langflow-0.4.4/src/backend/langflow/template/template/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/utils/constants.py` & `langflow-0.4.4/src/backend/langflow/utils/constants.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/utils/logger.py` & `langflow-0.4.4/src/backend/langflow/utils/logger.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/utils/payload.py` & `langflow-0.4.4/src/backend/langflow/utils/payload.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/utils/util.py` & `langflow-0.4.4/src/backend/langflow/utils/util.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/src/backend/langflow/utils/validate.py` & `langflow-0.4.4/src/backend/langflow/utils/validate.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.3/PKG-INFO` & `langflow-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langflow
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Python package with a built-in web application
 Home-page: https://github.com/logspace-ai/langflow
 License: MIT
 Keywords: nlp,langchain,openai,gpt,gui
 Author: Logspace
 Author-email: contact@logspace.ai
 Maintainer: Carlos Coelho
@@ -40,15 +40,15 @@
 Requires-Dist: langchain-experimental (>=0.0.8,<0.0.9)
 Requires-Dist: langchain-serve (>0.0.51) ; extra == "deploy"
 Requires-Dist: llama-cpp-python (>=0.1.0,<0.2.0) ; extra == "local"
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: multiprocess (>=0.70.14,<0.71.0)
 Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
-Requires-Dist: orjson (>=3.9.1,<4.0.0)
+Requires-Dist: orjson (==3.9.3)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: pinecone-client (>=2.2.2,<3.0.0)
 Requires-Dist: psycopg (>=3.1.9,<4.0.0)
 Requires-Dist: psycopg-binary (>=3.1.9,<4.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0)
 Requires-Dist: pyarrow (>=12.0.0,<13.0.0)
 Requires-Dist: pymongo (>=4.4.0,<5.0.0)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: langflow Version: 0.4.3 Summary: A Python package
+Metadata-Version: 2.1 Name: langflow Version: 0.4.4 Summary: A Python package
 with a built-in web application Home-page: https://github.com/logspace-ai/
 langflow License: MIT Keywords: nlp,langchain,openai,gpt,gui Author: Logspace
 Author-email: contact@logspace.ai Maintainer: Carlos Coelho Maintainer-email:
 carlos@logspace.ai Requires-Python: >=3.9,<3.11 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Provides-Extra: all Provides-Extra: deploy Provides-
@@ -19,15 +19,15 @@
 (>=2.4.1,<3.0.0) Requires-Dist: gunicorn (>=21.1.0,<22.0.0) Requires-Dist:
 huggingface-hub[inference] (>=0.16.0,<0.17.0) Requires-Dist: jina (==3.15.2)
 Requires-Dist: langchain (>=0.0.256,<0.0.257) Requires-Dist: langchain-
 experimental (>=0.0.8,<0.0.9) Requires-Dist: langchain-serve (>0.0.51) ; extra
 == "deploy" Requires-Dist: llama-cpp-python (>=0.1.0,<0.2.0) ; extra == "local"
 Requires-Dist: lxml (>=4.9.2,<5.0.0) Requires-Dist: multiprocess
 (>=0.70.14,<0.71.0) Requires-Dist: networkx (>=3.1,<4.0) Requires-Dist: openai
-(>=0.27.8,<0.28.0) Requires-Dist: orjson (>=3.9.1,<4.0.0) Requires-Dist: pandas
+(>=0.27.8,<0.28.0) Requires-Dist: orjson (==3.9.3) Requires-Dist: pandas
 (>=2.0.0,<3.0.0) Requires-Dist: pinecone-client (>=2.2.2,<3.0.0) Requires-Dist:
 psycopg (>=3.1.9,<4.0.0) Requires-Dist: psycopg-binary (>=3.1.9,<4.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0) Requires-Dist: pyarrow
 (>=12.0.0,<13.0.0) Requires-Dist: pymongo (>=4.4.0,<5.0.0) Requires-Dist: pypdf
 (>=3.11.0,<4.0.0) Requires-Dist: pysrt (>=1.1.2,<2.0.0) Requires-Dist: python-
 multipart (>=0.0.6,<0.0.7) Requires-Dist: qdrant-client (>=1.3.0,<2.0.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0) Requires-Dist: sentence-transformers
```

