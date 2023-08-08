# Comparing `tmp/langflow-0.4.1.tar.gz` & `tmp/langflow-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langflow-0.4.1.tar", max compression
+gzip compressed data, was "langflow-0.4.2.tar", max compression
```

## Comparing `langflow-0.4.1.tar` & `langflow-0.4.2.tar`

### file list

```diff
@@ -1,160 +1,160 @@
--rw-r--r--   0        0        0     1065 2023-08-04 19:07:30.184463 langflow-0.4.1/LICENSE
--rw-r--r--   0        0        0    15764 2023-08-04 19:07:30.184463 langflow-0.4.1/README.md
--rw-r--r--   0        0        0     3072 2023-08-04 19:07:30.700469 langflow-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      514 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/__init__.py
--rw-r--r--   0        0        0     9339 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/__main__.py
--rw-r--r--   0        0        0       61 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/api/__init__.py
--rw-r--r--   0        0        0      485 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/api/router.py
--rw-r--r--   0        0        0     2380 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/api/utils.py
--rw-r--r--   0        0        0      526 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/api/v1/__init__.py
--rw-r--r--   0        0        0     4486 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/api/v1/base.py
--rw-r--r--   0        0        0     4979 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/api/v1/callback.py
--rw-r--r--   0        0        0     7300 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/api/v1/chat.py
--rw-r--r--   0        0        0     2534 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/api/v1/components.py
--rw-r--r--   0        0        0     4129 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/api/v1/endpoints.py
--rw-r--r--   0        0        0     2691 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/api/v1/flow_styles.py
--rw-r--r--   0        0        0     3868 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/api/v1/flows.py
--rw-r--r--   0        0        0     2625 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/api/v1/schemas.py
--rw-r--r--   0        0        0     4439 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/api/v1/validate.py
--rw-r--r--   0        0        0      152 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/cache/__init__.py
--rw-r--r--   0        0        0     1815 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/cache/base.py
--rw-r--r--   0        0        0     4554 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/cache/flow.py
--rw-r--r--   0        0        0     4481 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/cache/manager.py
--rw-r--r--   0        0        0     5062 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/cache/utils.py
--rw-r--r--   0        0        0        0 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/chat/__init__.py
--rw-r--r--   0        0        0       45 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/chat/config.py
--rw-r--r--   0        0        0     8554 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/chat/manager.py
--rw-r--r--   0        0        0     1272 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/chat/utils.py
--rw-r--r--   0        0        0      103 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/components/__init__.py
--rw-r--r--   0        0        0        0 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/components/chains/__init__.py
--rw-r--r--   0        0        0     1003 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/components/chains/prompt_runner.py
--rw-r--r--   0        0        0    13474 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/config.yaml
--rw-r--r--   0        0        0        0 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/custom/__init__.py
--rw-r--r--   0        0        0     1733 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/custom/customs.py
--rw-r--r--   0        0        0        0 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/database/__init__.py
--rw-r--r--   0        0        0     2387 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/database/base.py
--rw-r--r--   0        0        0        0 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/database/models/__init__.py
--rw-r--r--   0        0        0      363 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/database/models/base.py
--rw-r--r--   0        0        0     1120 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/database/models/component.py
--rw-r--r--   0        0        0     1705 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/database/models/flow.py
--rw-r--r--   0        0        0      831 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/database/models/flow_style.py
--rw-r--r--   0        0        0   206379 2023-08-04 19:08:57.784855 langflow-0.4.1/src/backend/langflow/frontend/assets/index-c3be492f.css
--rw-r--r--   0        0        0  4229497 2023-08-04 19:08:57.788855 langflow-0.4.1/src/backend/langflow/frontend/assets/index-f45528ab.js
--rw-r--r--   0        0        0    23161 2023-08-04 19:08:57.784855 langflow-0.4.1/src/backend/langflow/frontend/assets/male-technologist-d2e7de57.png
--rw-r--r--   0        0        0    26806 2023-08-04 19:08:57.784855 langflow-0.4.1/src/backend/langflow/frontend/assets/robot-95e1b00d.png
--rw-r--r--   0        0        0     4310 2023-08-04 19:08:57.784855 langflow-0.4.1/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js
--rw-r--r--   0        0        0   104188 2023-08-04 19:08:57.784855 langflow-0.4.1/src/backend/langflow/frontend/favicon.ico
--rw-r--r--   0        0        0      724 2023-08-04 19:08:57.784855 langflow-0.4.1/src/backend/langflow/frontend/index.html
--rw-r--r--   0        0        0      764 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/graph/__init__.py
--rw-r--r--   0        0        0        0 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/graph/edge/__init__.py
--rw-r--r--   0        0        0     2349 2023-08-04 19:07:30.700469 langflow-0.4.1/src/backend/langflow/graph/edge/base.py
--rw-r--r--   0        0        0        0 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/graph/graph/__init__.py
--rw-r--r--   0        0        0     7854 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/graph/graph/base.py
--rw-r--r--   0        0        0     2165 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/graph/graph/constants.py
--rw-r--r--   0        0        0        0 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/graph/graph/utils.py
--rw-r--r--   0        0        0      642 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/graph/utils.py
--rw-r--r--   0        0        0        0 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/graph/vertex/__init__.py
--rw-r--r--   0        0        0    10167 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/graph/vertex/base.py
--rw-r--r--   0        0        0        1 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/graph/vertex/constants.py
--rw-r--r--   0        0        0     8689 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/graph/vertex/types.py
--rw-r--r--   0        0        0        0 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/__init__.py
--rw-r--r--   0        0        0       84 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/agents/__init__.py
--rw-r--r--   0        0        0     2423 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/agents/base.py
--rw-r--r--   0        0        0    10224 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/agents/custom.py
--rw-r--r--   0        0        0     1447 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/agents/prebuilt.py
--rw-r--r--   0        0        0     4690 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/base.py
--rw-r--r--   0        0        0       84 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/chains/__init__.py
--rw-r--r--   0        0        0     3006 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/chains/base.py
--rw-r--r--   0        0        0     4843 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/chains/custom.py
--rw-r--r--   0        0        0      194 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/custom/__init__.py
--rw-r--r--   0        0        0     1594 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/custom/base.py
--rw-r--r--   0        0        0     8937 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/custom/code_parser.py
--rw-r--r--   0        0        0     2122 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/custom/component.py
--rw-r--r--   0        0        0     1788 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/custom/constants.py
--rw-r--r--   0        0        0     6572 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/custom/custom_component.py
--rw-r--r--   0        0        0     9279 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/custom/directory_reader.py
--rw-r--r--   0        0        0      529 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/custom/schema.py
--rw-r--r--   0        0        0     2306 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/custom_lists.py
--rw-r--r--   0        0        0        0 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/document_loaders/__init__.py
--rw-r--r--   0        0        0     1479 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/document_loaders/base.py
--rw-r--r--   0        0        0        0 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/embeddings/__init__.py
--rw-r--r--   0        0        0     1445 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/embeddings/base.py
--rw-r--r--   0        0        0      171 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/importing/__init__.py
--rw-r--r--   0        0        0     6105 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/importing/utils.py
--rw-r--r--   0        0        0        0 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/initialize/__init__.py
--rw-r--r--   0        0        0      385 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/initialize/llm.py
--rw-r--r--   0        0        0    18948 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/initialize/loading.py
--rw-r--r--   0        0        0     3772 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/initialize/utils.py
--rw-r--r--   0        0        0     7704 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/initialize/vector_store.py
--rw-r--r--   0        0        0     2048 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/listing.py
--rw-r--r--   0        0        0       78 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/llms/__init__.py
--rw-r--r--   0        0        0     1355 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/llms/base.py
--rw-r--r--   0        0        0       88 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/memories/__init__.py
--rw-r--r--   0        0        0     2135 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/memories/base.py
--rw-r--r--   0        0        0        0 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/output_parsers/__init__.py
--rw-r--r--   0        0        0     2355 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/output_parsers/base.py
--rw-r--r--   0        0        0       87 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/prompts/__init__.py
--rw-r--r--   0        0        0     2459 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/prompts/base.py
--rw-r--r--   0        0        0     2483 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/prompts/custom.py
--rw-r--r--   0        0        0        0 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/retrievers/__init__.py
--rw-r--r--   0        0        0     2086 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/retrievers/base.py
--rw-r--r--   0        0        0     2764 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/run.py
--rw-r--r--   0        0        0      106 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/text_splitters/__init__.py
--rw-r--r--   0        0        0     1450 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/text_splitters/base.py
--rw-r--r--   0        0        0        0 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/toolkits/__init__.py
--rw-r--r--   0        0        0     2598 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/toolkits/base.py
--rw-r--r--   0        0        0        0 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/toolkits/custom.py
--rw-r--r--   0        0        0       81 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/tools/__init__.py
--rw-r--r--   0        0        0     5418 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/tools/base.py
--rw-r--r--   0        0        0      913 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/tools/constants.py
--rw-r--r--   0        0        0     1269 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/tools/custom.py
--rw-r--r--   0        0        0     4328 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/tools/util.py
--rw-r--r--   0        0        0    14759 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/types.py
--rw-r--r--   0        0        0        0 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/utilities/__init__.py
--rw-r--r--   0        0        0     2294 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/utilities/base.py
--rw-r--r--   0        0        0     2645 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/utils.py
--rw-r--r--   0        0        0        0 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/vector_store/__init__.py
--rw-r--r--   0        0        0     1813 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/vector_store/base.py
--rw-r--r--   0        0        0        0 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/wrappers/__init__.py
--rw-r--r--   0        0        0     1500 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/interface/wrappers/base.py
--rw-r--r--   0        0        0       29 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/jcloud.yml
--rw-r--r--   0        0        0      428 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/lcserve.py
--rw-r--r--   0        0        0     2556 2023-08-04 19:07:30.704469 langflow-0.4.1/src/backend/langflow/main.py
--rw-r--r--   0        0        0        0 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/processing/__init__.py
--rw-r--r--   0        0        0     2013 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/processing/base.py
--rw-r--r--   0        0        0     8650 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/processing/process.py
--rw-r--r--   0        0        0      579 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/server.py
--rw-r--r--   0        0        0     6451 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/settings.py
--rw-r--r--   0        0        0        0 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/template/__init__.py
--rw-r--r--   0        0        0        0 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/template/field/__init__.py
--rw-r--r--   0        0        0     2571 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/template/field/base.py
--rw-r--r--   0        0        0      423 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/template/frontend_node/__init__.py
--rw-r--r--   0        0        0     7033 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/template/frontend_node/agents.py
--rw-r--r--   0        0        0     9840 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/template/frontend_node/base.py
--rw-r--r--   0        0        0     7796 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/template/frontend_node/chains.py
--rw-r--r--   0        0        0     1694 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/template/frontend_node/constants.py
--rw-r--r--   0        0        0      998 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/template/frontend_node/custom_components.py
--rw-r--r--   0        0        0     8636 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/template/frontend_node/documentloaders.py
--rw-r--r--   0        0        0     1680 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/template/frontend_node/embeddings.py
--rw-r--r--   0        0        0        0 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/template/frontend_node/formatter/__init__.py
--rw-r--r--   0        0        0      297 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/template/frontend_node/formatter/base.py
--rw-r--r--   0        0        0     5569 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/template/frontend_node/formatter/field_formatters.py
--rw-r--r--   0        0        0     5370 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/template/frontend_node/llms.py
--rw-r--r--   0        0        0     6559 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/template/frontend_node/memories.py
--rw-r--r--   0        0        0      364 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/template/frontend_node/output_parsers.py
--rw-r--r--   0        0        0     3540 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/template/frontend_node/prompts.py
--rw-r--r--   0        0        0      523 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/template/frontend_node/retrievers.py
--rw-r--r--   0        0        0     2355 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/template/frontend_node/textsplitters.py
--rw-r--r--   0        0        0     4016 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/template/frontend_node/tools.py
--rw-r--r--   0        0        0      823 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/template/frontend_node/utilities.py
--rw-r--r--   0        0        0     9428 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/template/frontend_node/vectorstores.py
--rw-r--r--   0        0        0        0 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/template/template/__init__.py
--rw-r--r--   0        0        0     1181 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/template/template/base.py
--rw-r--r--   0        0        0        0 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/utils/__init__.py
--rw-r--r--   0        0        0     1792 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/utils/constants.py
--rw-r--r--   0        0        0      915 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/utils/logger.py
--rw-r--r--   0        0        0     3169 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/utils/payload.py
--rw-r--r--   0        0        0       23 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/utils/types.py
--rw-r--r--   0        0        0    13928 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/utils/util.py
--rw-r--r--   0        0        0     7665 2023-08-04 19:07:30.708469 langflow-0.4.1/src/backend/langflow/utils/validate.py
--rw-r--r--   0        0        0    18838 1970-01-01 00:00:00.000000 langflow-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-08 18:01:13.450185 langflow-0.4.2/LICENSE
+-rw-r--r--   0        0        0    15764 2023-08-08 18:01:13.450185 langflow-0.4.2/README.md
+-rw-r--r--   0        0        0     3072 2023-08-08 18:01:13.862196 langflow-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      514 2023-08-08 18:01:13.862196 langflow-0.4.2/src/backend/langflow/__init__.py
+-rw-r--r--   0        0        0     9339 2023-08-08 18:01:13.862196 langflow-0.4.2/src/backend/langflow/__main__.py
+-rw-r--r--   0        0        0       61 2023-08-08 18:01:13.862196 langflow-0.4.2/src/backend/langflow/api/__init__.py
+-rw-r--r--   0        0        0      485 2023-08-08 18:01:13.862196 langflow-0.4.2/src/backend/langflow/api/router.py
+-rw-r--r--   0        0        0     3203 2023-08-08 18:01:13.862196 langflow-0.4.2/src/backend/langflow/api/utils.py
+-rw-r--r--   0        0        0      526 2023-08-08 18:01:13.862196 langflow-0.4.2/src/backend/langflow/api/v1/__init__.py
+-rw-r--r--   0        0        0     4486 2023-08-08 18:01:13.862196 langflow-0.4.2/src/backend/langflow/api/v1/base.py
+-rw-r--r--   0        0        0     4979 2023-08-08 18:01:13.862196 langflow-0.4.2/src/backend/langflow/api/v1/callback.py
+-rw-r--r--   0        0        0     7300 2023-08-08 18:01:13.862196 langflow-0.4.2/src/backend/langflow/api/v1/chat.py
+-rw-r--r--   0        0        0     2534 2023-08-08 18:01:13.862196 langflow-0.4.2/src/backend/langflow/api/v1/components.py
+-rw-r--r--   0        0        0     4429 2023-08-08 18:01:13.862196 langflow-0.4.2/src/backend/langflow/api/v1/endpoints.py
+-rw-r--r--   0        0        0     2691 2023-08-08 18:01:13.862196 langflow-0.4.2/src/backend/langflow/api/v1/flow_styles.py
+-rw-r--r--   0        0        0     3868 2023-08-08 18:01:13.862196 langflow-0.4.2/src/backend/langflow/api/v1/flows.py
+-rw-r--r--   0        0        0     2625 2023-08-08 18:01:13.862196 langflow-0.4.2/src/backend/langflow/api/v1/schemas.py
+-rw-r--r--   0        0        0     4439 2023-08-08 18:01:13.862196 langflow-0.4.2/src/backend/langflow/api/v1/validate.py
+-rw-r--r--   0        0        0      152 2023-08-08 18:01:13.862196 langflow-0.4.2/src/backend/langflow/cache/__init__.py
+-rw-r--r--   0        0        0     1815 2023-08-08 18:01:13.862196 langflow-0.4.2/src/backend/langflow/cache/base.py
+-rw-r--r--   0        0        0     4554 2023-08-08 18:01:13.862196 langflow-0.4.2/src/backend/langflow/cache/flow.py
+-rw-r--r--   0        0        0     4481 2023-08-08 18:01:13.862196 langflow-0.4.2/src/backend/langflow/cache/manager.py
+-rw-r--r--   0        0        0     5062 2023-08-08 18:01:13.862196 langflow-0.4.2/src/backend/langflow/cache/utils.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:01:13.862196 langflow-0.4.2/src/backend/langflow/chat/__init__.py
+-rw-r--r--   0        0        0       45 2023-08-08 18:01:13.862196 langflow-0.4.2/src/backend/langflow/chat/config.py
+-rw-r--r--   0        0        0     8554 2023-08-08 18:01:13.862196 langflow-0.4.2/src/backend/langflow/chat/manager.py
+-rw-r--r--   0        0        0     1272 2023-08-08 18:01:13.862196 langflow-0.4.2/src/backend/langflow/chat/utils.py
+-rw-r--r--   0        0        0      103 2023-08-08 18:01:13.862196 langflow-0.4.2/src/backend/langflow/components/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:01:13.862196 langflow-0.4.2/src/backend/langflow/components/chains/__init__.py
+-rw-r--r--   0        0        0     1003 2023-08-08 18:01:13.862196 langflow-0.4.2/src/backend/langflow/components/chains/prompt_runner.py
+-rw-r--r--   0        0        0    13474 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/config.yaml
+-rw-r--r--   0        0        0        0 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/custom/__init__.py
+-rw-r--r--   0        0        0     1733 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/custom/customs.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/database/__init__.py
+-rw-r--r--   0        0        0     2387 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/database/base.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/database/models/__init__.py
+-rw-r--r--   0        0        0      363 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/database/models/base.py
+-rw-r--r--   0        0        0     1120 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/database/models/component.py
+-rw-r--r--   0        0        0     1705 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/database/models/flow.py
+-rw-r--r--   0        0        0      831 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/database/models/flow_style.py
+-rw-r--r--   0        0        0  4229512 2023-08-08 18:02:20.467846 langflow-0.4.2/src/backend/langflow/frontend/assets/index-52958152.js
+-rw-r--r--   0        0        0   206379 2023-08-08 18:02:20.463846 langflow-0.4.2/src/backend/langflow/frontend/assets/index-c3be492f.css
+-rw-r--r--   0        0        0    23161 2023-08-08 18:02:20.463846 langflow-0.4.2/src/backend/langflow/frontend/assets/male-technologist-d2e7de57.png
+-rw-r--r--   0        0        0    26806 2023-08-08 18:02:20.463846 langflow-0.4.2/src/backend/langflow/frontend/assets/robot-95e1b00d.png
+-rw-r--r--   0        0        0     4310 2023-08-08 18:02:20.463846 langflow-0.4.2/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js
+-rw-r--r--   0        0        0   104188 2023-08-08 18:02:20.463846 langflow-0.4.2/src/backend/langflow/frontend/favicon.ico
+-rw-r--r--   0        0        0      724 2023-08-08 18:02:20.467846 langflow-0.4.2/src/backend/langflow/frontend/index.html
+-rw-r--r--   0        0        0      764 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/graph/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/graph/edge/__init__.py
+-rw-r--r--   0        0        0     2349 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/graph/edge/base.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/graph/graph/__init__.py
+-rw-r--r--   0        0        0     7854 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/graph/graph/base.py
+-rw-r--r--   0        0        0     2165 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/graph/graph/constants.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/graph/graph/utils.py
+-rw-r--r--   0        0        0      642 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/graph/utils.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/graph/vertex/__init__.py
+-rw-r--r--   0        0        0    10167 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/graph/vertex/base.py
+-rw-r--r--   0        0        0        1 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/graph/vertex/constants.py
+-rw-r--r--   0        0        0     8689 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/graph/vertex/types.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/__init__.py
+-rw-r--r--   0        0        0       84 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/agents/__init__.py
+-rw-r--r--   0        0        0     2423 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/agents/base.py
+-rw-r--r--   0        0        0    10224 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/agents/custom.py
+-rw-r--r--   0        0        0     1447 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/agents/prebuilt.py
+-rw-r--r--   0        0        0     4690 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/base.py
+-rw-r--r--   0        0        0       84 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/chains/__init__.py
+-rw-r--r--   0        0        0     3006 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/chains/base.py
+-rw-r--r--   0        0        0     4843 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/chains/custom.py
+-rw-r--r--   0        0        0      194 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/custom/__init__.py
+-rw-r--r--   0        0        0     1594 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/custom/base.py
+-rw-r--r--   0        0        0     8937 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/custom/code_parser.py
+-rw-r--r--   0        0        0     2122 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/custom/component.py
+-rw-r--r--   0        0        0     1788 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/custom/constants.py
+-rw-r--r--   0        0        0     6572 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/custom/custom_component.py
+-rw-r--r--   0        0        0     9279 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/custom/directory_reader.py
+-rw-r--r--   0        0        0      529 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/custom/schema.py
+-rw-r--r--   0        0        0     2306 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/custom_lists.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/document_loaders/__init__.py
+-rw-r--r--   0        0        0     1479 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/document_loaders/base.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/embeddings/__init__.py
+-rw-r--r--   0        0        0     1445 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/embeddings/base.py
+-rw-r--r--   0        0        0      171 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/importing/__init__.py
+-rw-r--r--   0        0        0     6105 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/importing/utils.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/initialize/__init__.py
+-rw-r--r--   0        0        0      385 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/initialize/llm.py
+-rw-r--r--   0        0        0    18948 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/initialize/loading.py
+-rw-r--r--   0        0        0     3772 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/initialize/utils.py
+-rw-r--r--   0        0        0     8309 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/initialize/vector_store.py
+-rw-r--r--   0        0        0     2048 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/listing.py
+-rw-r--r--   0        0        0       78 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/llms/__init__.py
+-rw-r--r--   0        0        0     1355 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/llms/base.py
+-rw-r--r--   0        0        0       88 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/memories/__init__.py
+-rw-r--r--   0        0        0     2135 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/memories/base.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/output_parsers/__init__.py
+-rw-r--r--   0        0        0     2355 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/output_parsers/base.py
+-rw-r--r--   0        0        0       87 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/prompts/__init__.py
+-rw-r--r--   0        0        0     2459 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/prompts/base.py
+-rw-r--r--   0        0        0     2483 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/prompts/custom.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/retrievers/__init__.py
+-rw-r--r--   0        0        0     2086 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/retrievers/base.py
+-rw-r--r--   0        0        0     2764 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/run.py
+-rw-r--r--   0        0        0      106 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/text_splitters/__init__.py
+-rw-r--r--   0        0        0     1450 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/text_splitters/base.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/toolkits/__init__.py
+-rw-r--r--   0        0        0     2598 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/toolkits/base.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/toolkits/custom.py
+-rw-r--r--   0        0        0       81 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/tools/__init__.py
+-rw-r--r--   0        0        0     5418 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/tools/base.py
+-rw-r--r--   0        0        0      913 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/tools/constants.py
+-rw-r--r--   0        0        0     1269 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/tools/custom.py
+-rw-r--r--   0        0        0     4328 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/tools/util.py
+-rw-r--r--   0        0        0    14787 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/types.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/utilities/__init__.py
+-rw-r--r--   0        0        0     2294 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/utilities/base.py
+-rw-r--r--   0        0        0     2645 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/utils.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/vector_store/__init__.py
+-rw-r--r--   0        0        0     1813 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/vector_store/base.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/wrappers/__init__.py
+-rw-r--r--   0        0        0     1500 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/interface/wrappers/base.py
+-rw-r--r--   0        0        0       29 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/jcloud.yml
+-rw-r--r--   0        0        0      428 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/lcserve.py
+-rw-r--r--   0        0        0     2556 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/main.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/processing/__init__.py
+-rw-r--r--   0        0        0     2013 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/processing/base.py
+-rw-r--r--   0        0        0     8650 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/processing/process.py
+-rw-r--r--   0        0        0      579 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/server.py
+-rw-r--r--   0        0        0     6451 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/settings.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/template/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/template/field/__init__.py
+-rw-r--r--   0        0        0     2571 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/template/field/base.py
+-rw-r--r--   0        0        0      423 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/template/frontend_node/__init__.py
+-rw-r--r--   0        0        0     7033 2023-08-08 18:01:13.866196 langflow-0.4.2/src/backend/langflow/template/frontend_node/agents.py
+-rw-r--r--   0        0        0     9840 2023-08-08 18:01:13.870196 langflow-0.4.2/src/backend/langflow/template/frontend_node/base.py
+-rw-r--r--   0        0        0     7796 2023-08-08 18:01:13.870196 langflow-0.4.2/src/backend/langflow/template/frontend_node/chains.py
+-rw-r--r--   0        0        0     1694 2023-08-08 18:01:13.870196 langflow-0.4.2/src/backend/langflow/template/frontend_node/constants.py
+-rw-r--r--   0        0        0      998 2023-08-08 18:01:13.870196 langflow-0.4.2/src/backend/langflow/template/frontend_node/custom_components.py
+-rw-r--r--   0        0        0     8636 2023-08-08 18:01:13.870196 langflow-0.4.2/src/backend/langflow/template/frontend_node/documentloaders.py
+-rw-r--r--   0        0        0     1680 2023-08-08 18:01:13.870196 langflow-0.4.2/src/backend/langflow/template/frontend_node/embeddings.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:01:13.870196 langflow-0.4.2/src/backend/langflow/template/frontend_node/formatter/__init__.py
+-rw-r--r--   0        0        0      297 2023-08-08 18:01:13.870196 langflow-0.4.2/src/backend/langflow/template/frontend_node/formatter/base.py
+-rw-r--r--   0        0        0     5569 2023-08-08 18:01:13.870196 langflow-0.4.2/src/backend/langflow/template/frontend_node/formatter/field_formatters.py
+-rw-r--r--   0        0        0     5370 2023-08-08 18:01:13.870196 langflow-0.4.2/src/backend/langflow/template/frontend_node/llms.py
+-rw-r--r--   0        0        0     6559 2023-08-08 18:01:13.870196 langflow-0.4.2/src/backend/langflow/template/frontend_node/memories.py
+-rw-r--r--   0        0        0      364 2023-08-08 18:01:13.870196 langflow-0.4.2/src/backend/langflow/template/frontend_node/output_parsers.py
+-rw-r--r--   0        0        0     3540 2023-08-08 18:01:13.870196 langflow-0.4.2/src/backend/langflow/template/frontend_node/prompts.py
+-rw-r--r--   0        0        0      523 2023-08-08 18:01:13.870196 langflow-0.4.2/src/backend/langflow/template/frontend_node/retrievers.py
+-rw-r--r--   0        0        0     2355 2023-08-08 18:01:13.870196 langflow-0.4.2/src/backend/langflow/template/frontend_node/textsplitters.py
+-rw-r--r--   0        0        0     4016 2023-08-08 18:01:13.870196 langflow-0.4.2/src/backend/langflow/template/frontend_node/tools.py
+-rw-r--r--   0        0        0     1029 2023-08-08 18:01:13.870196 langflow-0.4.2/src/backend/langflow/template/frontend_node/utilities.py
+-rw-r--r--   0        0        0    11001 2023-08-08 18:01:13.870196 langflow-0.4.2/src/backend/langflow/template/frontend_node/vectorstores.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:01:13.870196 langflow-0.4.2/src/backend/langflow/template/template/__init__.py
+-rw-r--r--   0        0        0     1181 2023-08-08 18:01:13.870196 langflow-0.4.2/src/backend/langflow/template/template/base.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:01:13.870196 langflow-0.4.2/src/backend/langflow/utils/__init__.py
+-rw-r--r--   0        0        0     1792 2023-08-08 18:01:13.870196 langflow-0.4.2/src/backend/langflow/utils/constants.py
+-rw-r--r--   0        0        0      915 2023-08-08 18:01:13.870196 langflow-0.4.2/src/backend/langflow/utils/logger.py
+-rw-r--r--   0        0        0     3169 2023-08-08 18:01:13.870196 langflow-0.4.2/src/backend/langflow/utils/payload.py
+-rw-r--r--   0        0        0       23 2023-08-08 18:01:13.870196 langflow-0.4.2/src/backend/langflow/utils/types.py
+-rw-r--r--   0        0        0    13928 2023-08-08 18:01:13.870196 langflow-0.4.2/src/backend/langflow/utils/util.py
+-rw-r--r--   0        0        0     7665 2023-08-08 18:01:13.870196 langflow-0.4.2/src/backend/langflow/utils/validate.py
+-rw-r--r--   0        0        0    18838 1970-01-01 00:00:00.000000 langflow-0.4.2/PKG-INFO
```

### Comparing `langflow-0.4.1/LICENSE` & `langflow-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/README.md` & `langflow-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/pyproject.toml` & `langflow-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langflow"
-version = "0.4.1"
+version = "0.4.2"
 description = "A Python package with a built-in web application"
 authors = ["Logspace <contact@logspace.ai>"]
 maintainers = [
     "Carlos Coelho <carlos@logspace.ai>",
     "Cristhian Zanforlin <cristhian.lousa@gmail.com>",
     "Gabriel Almeida <gabriel@logspace.ai>",
     "Gustavo Schaedler <gustavopoa@gmail.com>",
@@ -29,15 +29,15 @@
 fastapi = "^0.100.0"
 uvicorn = "^0.22.0"
 beautifulsoup4 = "^4.12.2"
 google-search-results = "^2.4.1"
 google-api-python-client = "^2.79.0"
 typer = "^0.9.0"
 gunicorn = "^21.1.0"
-langchain = "^0.0.250"
+langchain = "^0.0.256"
 openai = "^0.27.8"
 pandas = "^2.0.0"
 chromadb = "^0.3.21"
 huggingface-hub = { version = "^0.16.0", extras = ["inference"] }
 rich = "^13.4.2"
 llama-cpp-python = { version = "~0.1.0", optional = true }
 networkx = "^3.1"
```

### Comparing `langflow-0.4.1/src/backend/langflow/__init__.py` & `langflow-0.4.2/src/backend/langflow/__init__.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/__main__.py` & `langflow-0.4.2/src/backend/langflow/__main__.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/api/utils.py` & `langflow-0.4.2/src/backend/langflow/api/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -62,7 +62,34 @@
 def merge_nested_dicts(dict1, dict2):
     for key, value in dict2.items():
         if isinstance(value, dict) and isinstance(dict1.get(key), dict):
             dict1[key] = merge_nested_dicts(dict1[key], value)
         else:
             dict1[key] = value
     return dict1
+
+
+def merge_nested_dicts_with_renaming(dict1, dict2):
+    for key, value in dict2.items():
+        if (
+            key in dict1
+            and isinstance(value, dict)
+            and isinstance(dict1.get(key), dict)
+        ):
+            for sub_key, sub_value in value.items():
+                if sub_key in dict1[key]:
+                    new_key = get_new_key(dict1[key], sub_key)
+                    dict1[key][new_key] = sub_value
+                else:
+                    dict1[key][sub_key] = sub_value
+        else:
+            dict1[key] = value
+    return dict1
+
+
+def get_new_key(dictionary, original_key):
+    counter = 1
+    new_key = original_key + " (" + str(counter) + ")"
+    while new_key in dictionary:
+        counter += 1
+        new_key = original_key + " (" + str(counter) + ")"
+    return new_key
```

### Comparing `langflow-0.4.1/src/backend/langflow/api/v1/__init__.py` & `langflow-0.4.2/src/backend/langflow/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/api/v1/base.py` & `langflow-0.4.2/src/backend/langflow/api/v1/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/api/v1/callback.py` & `langflow-0.4.2/src/backend/langflow/api/v1/callback.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/api/v1/chat.py` & `langflow-0.4.2/src/backend/langflow/api/v1/chat.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/api/v1/components.py` & `langflow-0.4.2/src/backend/langflow/api/v1/components.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/api/v1/endpoints.py` & `langflow-0.4.2/src/backend/langflow/api/v1/endpoints.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from langflow.api.v1.schemas import (
     ProcessResponse,
     UploadFileResponse,
     CustomComponentCode,
 )
 
-from langflow.api.utils import merge_nested_dicts
+from langflow.api.utils import merge_nested_dicts_with_renaming
 
 from langflow.interface.types import (
     build_langchain_types_dict,
     build_langchain_template_custom_component,
     build_langchain_custom_component_list_from_path,
 )
 
@@ -42,22 +42,29 @@
     custom_components_from_file = {}
     if settings.COMPONENTS_PATH:
         logger.info(f"Building custom components from {settings.COMPONENTS_PATH}")
         custom_component_dicts = [
             build_langchain_custom_component_list_from_path(str(path))
             for path in settings.COMPONENTS_PATH
         ]
-        logger.info(f"Loading {len(custom_component_dicts)} custom components")
-
+        logger.info(f"Loading {len(custom_component_dicts)} category(ies)")
         for custom_component_dict in custom_component_dicts:
-            custom_components_from_file = merge_nested_dicts(
+            # custom_component_dict is a dict of dicts
+            category = list(custom_component_dict.keys())[0]
+            logger.info(
+                f"Loading {len(custom_component_dict[category])} component(s) from category {category}"
+            )
+            logger.debug(custom_component_dict)
+            custom_components_from_file = merge_nested_dicts_with_renaming(
                 custom_components_from_file, custom_component_dict
             )
-            logger.info(f"Loaded {custom_component_dict}")
-    return merge_nested_dicts(native_components, custom_components_from_file)
+
+    return merge_nested_dicts_with_renaming(
+        native_components, custom_components_from_file
+    )
 
 
 # For backwards compatibility we will keep the old endpoint
 @router.post("/predict/{flow_id}", response_model=ProcessResponse)
 @router.post("/process/{flow_id}", response_model=ProcessResponse)
 async def process_flow(
     flow_id: str,
```

### Comparing `langflow-0.4.1/src/backend/langflow/api/v1/flow_styles.py` & `langflow-0.4.2/src/backend/langflow/api/v1/flow_styles.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/api/v1/flows.py` & `langflow-0.4.2/src/backend/langflow/api/v1/flows.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/api/v1/schemas.py` & `langflow-0.4.2/src/backend/langflow/api/v1/schemas.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/api/v1/validate.py` & `langflow-0.4.2/src/backend/langflow/api/v1/validate.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/cache/base.py` & `langflow-0.4.2/src/backend/langflow/cache/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/cache/flow.py` & `langflow-0.4.2/src/backend/langflow/cache/flow.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/cache/manager.py` & `langflow-0.4.2/src/backend/langflow/cache/manager.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/cache/utils.py` & `langflow-0.4.2/src/backend/langflow/cache/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/chat/manager.py` & `langflow-0.4.2/src/backend/langflow/chat/manager.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/chat/utils.py` & `langflow-0.4.2/src/backend/langflow/chat/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/components/chains/prompt_runner.py` & `langflow-0.4.2/src/backend/langflow/components/chains/prompt_runner.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/config.yaml` & `langflow-0.4.2/src/backend/langflow/config.yaml`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/custom/customs.py` & `langflow-0.4.2/src/backend/langflow/custom/customs.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/database/base.py` & `langflow-0.4.2/src/backend/langflow/database/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/database/models/component.py` & `langflow-0.4.2/src/backend/langflow/database/models/component.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/database/models/flow.py` & `langflow-0.4.2/src/backend/langflow/database/models/flow.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/database/models/flow_style.py` & `langflow-0.4.2/src/backend/langflow/database/models/flow_style.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/frontend/assets/index-c3be492f.css` & `langflow-0.4.2/src/backend/langflow/frontend/assets/index-c3be492f.css`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/frontend/assets/index-f45528ab.js` & `langflow-0.4.2/src/backend/langflow/frontend/assets/index-52958152.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -143657,15 +143657,15 @@
             name: "Python Code",
             mode: "python",
             image: "https://cdn-icons-png.flaticon.com/512/5968/5968350.png",
             language: "py",
             code: T
         }, {
             name: "Chat Widget HTML",
-            description: "Insert this code anywhere in your &lt;body&gt; tag. To use with react and other libs, check our <a class='link-color' href='https://langflow.org/guidelines/widget'>documentation</a>.",
+            description: "Insert this code anywhere in your &lt;body&gt; tag. To use with react and other libs, check our <a class='link-color' href='https://docs.langflow.org/guidelines/widget'>documentation</a>.",
             mode: "html",
             image: "https://cdn-icons-png.flaticon.com/512/5968/5968350.png",
             language: "py",
             code: Q
         }]);
 
         function x() {
@@ -143694,15 +143694,15 @@
                 name: "Python Code",
                 mode: "python",
                 language: "py",
                 image: "https://cdn-icons-png.flaticon.com/512/5968/5968350.png",
                 code: T
             }, {
                 name: "Chat Widget HTML",
-                description: "Insert this code anywhere in your &lt;body&gt; tag. To use with react and other libs, check our <a class='link-color' href='https://langflow.org/guidelines/widget'>documentation</a>.",
+                description: "Insert this code anywhere in your &lt;body&gt; tag. To use with react and other libs, check our <a class='link-color' href='https://docs.langflow.org/guidelines/widget'>documentation</a>.",
                 mode: "html",
                 image: "https://cdn-icons-png.flaticon.com/512/5968/5968350.png",
                 language: "py",
                 code: Q
             }, {
                 name: "Tweaks",
                 mode: "python",
@@ -143725,15 +143725,15 @@
                 name: "Python Code",
                 mode: "python",
                 image: "https://cdn-icons-png.flaticon.com/512/5968/5968350.png",
                 language: "py",
                 code: T
             }, {
                 name: "Chat Widget HTML",
-                description: "Insert this code anywhere in your &lt;body&gt; tag. To use with react and other libs, check our <a class='link-color' href='https://langflow.org/guidelines/widget'>documentation</a>.",
+                description: "Insert this code anywhere in your &lt;body&gt; tag. To use with react and other libs, check our <a class='link-color' href='https://docs.langflow.org/guidelines/widget'>documentation</a>.",
                 mode: "html",
                 image: "https://cdn-icons-png.flaticon.com/512/5968/5968350.png",
                 language: "py",
                 code: Q
             }])
         }, [e.data.nodes, i]);
```

### Comparing `langflow-0.4.1/src/backend/langflow/frontend/assets/male-technologist-d2e7de57.png` & `langflow-0.4.2/src/backend/langflow/frontend/assets/male-technologist-d2e7de57.png`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/frontend/assets/robot-95e1b00d.png` & `langflow-0.4.2/src/backend/langflow/frontend/assets/robot-95e1b00d.png`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js` & `langflow-0.4.2/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/frontend/favicon.ico` & `langflow-0.4.2/src/backend/langflow/frontend/favicon.ico`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/frontend/index.html` & `langflow-0.4.2/src/backend/langflow/frontend/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 <head>
     <meta charset="UTF-8">
     <meta http-equiv="X-UA-Compatible" content="IE=edge">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <link rel="icon" href="/favicon.ico" />
     <script src="/node_modules/ace-builds/src-min-noconflict/ace.js" type="text/javascript"></script>
     <title>Langflow</title>
-  <script type="module" crossorigin src="/assets/index-f45528ab.js"></script>
+  <script type="module" crossorigin src="/assets/index-52958152.js"></script>
   <link rel="stylesheet" href="/assets/index-c3be492f.css">
 </head>
 <body id='body' style="width: 100%; height:100%">
     <noscript>You need to enable JavaScript to run this app.</noscript>
     <div style="width: 100vw; height:100vh" id='root'></div>
     
 </body>
```

### Comparing `langflow-0.4.1/src/backend/langflow/graph/__init__.py` & `langflow-0.4.2/src/backend/langflow/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/graph/edge/base.py` & `langflow-0.4.2/src/backend/langflow/graph/edge/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/graph/graph/base.py` & `langflow-0.4.2/src/backend/langflow/graph/graph/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/graph/graph/constants.py` & `langflow-0.4.2/src/backend/langflow/graph/graph/constants.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/graph/utils.py` & `langflow-0.4.2/src/backend/langflow/graph/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/graph/vertex/base.py` & `langflow-0.4.2/src/backend/langflow/graph/vertex/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/graph/vertex/types.py` & `langflow-0.4.2/src/backend/langflow/graph/vertex/types.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/agents/base.py` & `langflow-0.4.2/src/backend/langflow/interface/agents/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/agents/custom.py` & `langflow-0.4.2/src/backend/langflow/interface/agents/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/agents/prebuilt.py` & `langflow-0.4.2/src/backend/langflow/interface/agents/prebuilt.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/base.py` & `langflow-0.4.2/src/backend/langflow/interface/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/chains/base.py` & `langflow-0.4.2/src/backend/langflow/interface/chains/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/chains/custom.py` & `langflow-0.4.2/src/backend/langflow/interface/chains/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/custom/base.py` & `langflow-0.4.2/src/backend/langflow/interface/custom/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/custom/code_parser.py` & `langflow-0.4.2/src/backend/langflow/interface/custom/code_parser.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/custom/component.py` & `langflow-0.4.2/src/backend/langflow/interface/custom/component.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/custom/constants.py` & `langflow-0.4.2/src/backend/langflow/interface/custom/constants.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/custom/custom_component.py` & `langflow-0.4.2/src/backend/langflow/interface/custom/custom_component.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/custom/directory_reader.py` & `langflow-0.4.2/src/backend/langflow/interface/custom/directory_reader.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/custom/schema.py` & `langflow-0.4.2/src/backend/langflow/interface/custom/schema.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/custom_lists.py` & `langflow-0.4.2/src/backend/langflow/interface/custom_lists.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/document_loaders/base.py` & `langflow-0.4.2/src/backend/langflow/interface/document_loaders/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/embeddings/base.py` & `langflow-0.4.2/src/backend/langflow/interface/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/importing/utils.py` & `langflow-0.4.2/src/backend/langflow/interface/importing/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/initialize/loading.py` & `langflow-0.4.2/src/backend/langflow/interface/initialize/loading.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/initialize/utils.py` & `langflow-0.4.2/src/backend/langflow/interface/initialize/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/initialize/vector_store.py` & `langflow-0.4.2/src/backend/langflow/interface/initialize/vector_store.py`

 * *Files 7% similar despite different names*

```diff
@@ -166,14 +166,30 @@
     if "texts" in params:
         params["documents"] = params.pop("texts")
     return class_object.from_documents(**params)
 
 
 def initialize_chroma(class_object: Type[Chroma], params: dict):
     """Initialize a ChromaDB object from the params"""
+    if (  # type: ignore
+        "chroma_server_host" in params
+        or "chroma_server_http_port" in params
+        or "chroma_server_ssl_enabled" in params
+        or "chroma_server_grpc_port" in params
+        or "chroma_server_cors_allow_origins" in params
+    ):
+        import chromadb  # type: ignore
+
+        settings_params = {
+            key: params[key]
+            for key, value_ in params.items()
+            if key.startswith("chroma_server_") and value_
+        }
+        chroma_settings = chromadb.config.Settings(**settings_params)
+        params["client_settings"] = chroma_settings
     persist = params.pop("persist", False)
     if not docs_in_params(params):
         params.pop("documents", None)
         params.pop("texts", None)
         params["embedding_function"] = params.pop("embedding")
         chromadb = class_object(**params)
     else:
```

### Comparing `langflow-0.4.1/src/backend/langflow/interface/listing.py` & `langflow-0.4.2/src/backend/langflow/interface/listing.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/llms/base.py` & `langflow-0.4.2/src/backend/langflow/interface/llms/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/memories/base.py` & `langflow-0.4.2/src/backend/langflow/interface/memories/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/output_parsers/base.py` & `langflow-0.4.2/src/backend/langflow/interface/output_parsers/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/prompts/base.py` & `langflow-0.4.2/src/backend/langflow/interface/prompts/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/prompts/custom.py` & `langflow-0.4.2/src/backend/langflow/interface/prompts/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/retrievers/base.py` & `langflow-0.4.2/src/backend/langflow/interface/retrievers/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/run.py` & `langflow-0.4.2/src/backend/langflow/interface/run.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/text_splitters/base.py` & `langflow-0.4.2/src/backend/langflow/interface/text_splitters/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/toolkits/base.py` & `langflow-0.4.2/src/backend/langflow/interface/toolkits/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/tools/base.py` & `langflow-0.4.2/src/backend/langflow/interface/tools/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/tools/constants.py` & `langflow-0.4.2/src/backend/langflow/interface/tools/constants.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/tools/custom.py` & `langflow-0.4.2/src/backend/langflow/interface/tools/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/tools/util.py` & `langflow-0.4.2/src/backend/langflow/interface/tools/util.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/types.py` & `langflow-0.4.2/src/backend/langflow/interface/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import ast
 import contextlib
 from typing import Any
+from langflow.api.utils import merge_nested_dicts_with_renaming
 from langflow.interface.agents.base import agent_creator
 from langflow.interface.chains.base import chain_creator
 from langflow.interface.custom.constants import CUSTOM_COMPONENT_SUPPORTED_TYPES
 from langflow.interface.document_loaders.base import documentloader_creator
 from langflow.interface.embeddings.base import embedding_creator
 from langflow.interface.importing.utils import get_function_custom
 from langflow.interface.llms.base import llm_creator
@@ -26,15 +27,14 @@
     CustomComponentFrontendNode,
 )
 from langflow.interface.retrievers.base import retriever_creator
 
 from langflow.interface.custom.directory_reader import DirectoryReader
 from langflow.utils.logger import logger
 from langflow.utils.util import get_base_classes
-from langflow.api.utils import merge_nested_dicts
 
 import re
 import warnings
 import traceback
 from fastapi import HTTPException
 
 
@@ -419,8 +419,8 @@
     valid_components, invalid_components = build_and_validate_all_files(
         reader, file_list
     )
 
     valid_menu = build_valid_menu(valid_components)
     invalid_menu = build_invalid_menu(invalid_components)
 
-    return merge_nested_dicts(valid_menu, invalid_menu)
+    return merge_nested_dicts_with_renaming(valid_menu, invalid_menu)
```

### Comparing `langflow-0.4.1/src/backend/langflow/interface/utilities/base.py` & `langflow-0.4.2/src/backend/langflow/interface/utilities/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/utils.py` & `langflow-0.4.2/src/backend/langflow/interface/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/vector_store/base.py` & `langflow-0.4.2/src/backend/langflow/interface/vector_store/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/interface/wrappers/base.py` & `langflow-0.4.2/src/backend/langflow/interface/wrappers/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/main.py` & `langflow-0.4.2/src/backend/langflow/main.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/processing/base.py` & `langflow-0.4.2/src/backend/langflow/processing/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/processing/process.py` & `langflow-0.4.2/src/backend/langflow/processing/process.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/server.py` & `langflow-0.4.2/src/backend/langflow/server.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/settings.py` & `langflow-0.4.2/src/backend/langflow/settings.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/template/field/base.py` & `langflow-0.4.2/src/backend/langflow/template/field/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/template/frontend_node/agents.py` & `langflow-0.4.2/src/backend/langflow/template/frontend_node/agents.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/template/frontend_node/base.py` & `langflow-0.4.2/src/backend/langflow/template/frontend_node/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/template/frontend_node/chains.py` & `langflow-0.4.2/src/backend/langflow/template/frontend_node/chains.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/template/frontend_node/constants.py` & `langflow-0.4.2/src/backend/langflow/template/frontend_node/constants.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/template/frontend_node/custom_components.py` & `langflow-0.4.2/src/backend/langflow/template/frontend_node/custom_components.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/template/frontend_node/documentloaders.py` & `langflow-0.4.2/src/backend/langflow/template/frontend_node/documentloaders.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/template/frontend_node/embeddings.py` & `langflow-0.4.2/src/backend/langflow/template/frontend_node/embeddings.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/template/frontend_node/formatter/field_formatters.py` & `langflow-0.4.2/src/backend/langflow/template/frontend_node/formatter/field_formatters.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/template/frontend_node/llms.py` & `langflow-0.4.2/src/backend/langflow/template/frontend_node/llms.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/template/frontend_node/memories.py` & `langflow-0.4.2/src/backend/langflow/template/frontend_node/memories.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/template/frontend_node/prompts.py` & `langflow-0.4.2/src/backend/langflow/template/frontend_node/prompts.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/template/frontend_node/retrievers.py` & `langflow-0.4.2/src/backend/langflow/template/frontend_node/retrievers.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/template/frontend_node/textsplitters.py` & `langflow-0.4.2/src/backend/langflow/template/frontend_node/textsplitters.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/template/frontend_node/tools.py` & `langflow-0.4.2/src/backend/langflow/template/frontend_node/tools.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/template/frontend_node/utilities.py` & `langflow-0.4.2/src/backend/langflow/template/frontend_node/utilities.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 
 class UtilitiesFrontendNode(FrontendNode):
     @staticmethod
     def format_field(field: TemplateField, name: Optional[str] = None) -> None:
         FrontendNode.format_field(field, name)
         # field.field_type could be "Literal['news', 'search', 'places', 'images']
         # we need to convert it to a list
+        # It seems it could also be like "typing_extensions.['news', 'search', 'places', 'images']"
         if "Literal" in field.field_type:
-            field.options = ast.literal_eval(field.field_type.replace("Literal", ""))
+            field_type = field.field_type.replace("typing_extensions.", "")
+            field_type = field_type.replace("Literal", "")
+            field.options = ast.literal_eval(field_type)
             field.is_list = True
             field.field_type = "str"
 
         if isinstance(field.value, dict):
             field.field_type = "code"
             field.value = json.dumps(field.value, indent=4)
```

### Comparing `langflow-0.4.1/src/backend/langflow/template/frontend_node/vectorstores.py` & `langflow-0.4.2/src/backend/langflow/template/frontend_node/vectorstores.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,59 @@
 from typing import List, Optional
 
 from langflow.template.field.base import TemplateField
 from langflow.template.frontend_node.base import FrontendNode
 
 
+BASIC_FIELDS = [
+    "work_dir",
+    "collection_name",
+    "api_key",
+    "location",
+    "persist_directory",
+    "persist",
+    "weaviate_url",
+    "index_name",
+    "namespace",
+    "folder_path",
+    "table_name",
+    "query_name",
+    "supabase_url",
+    "supabase_service_key",
+    "mongodb_atlas_cluster_uri",
+    "collection_name",
+    "db_name",
+]
+ADVANCED_FIELDS = [
+    "n_dim",
+    "key",
+    "prefix",
+    "distance_func",
+    "content_payload_key",
+    "metadata_payload_key",
+    "timeout",
+    "host",
+    "path",
+    "url",
+    "port",
+    "https",
+    "prefer_grpc",
+    "grpc_port",
+    "pinecone_api_key",
+    "pinecone_env",
+    "client_kwargs",
+    "search_kwargs",
+    "chroma_server_host",
+    "chroma_server_http_port",
+    "chroma_server_ssl_enabled",
+    "chroma_server_grpc_port",
+    "chroma_server_cors_allow_origins",
+]
+
+
 class VectorStoreFrontendNode(FrontendNode):
     def add_extra_fields(self) -> None:
         extra_fields: List[TemplateField] = []
         # Add search_kwargs field
         extra_field = TemplateField(
             name="search_kwargs",
             field_type="code",
@@ -41,24 +87,70 @@
                 multiline=False,
                 value="{}",
             )
             extra_fields.extend((extra_field, extra_field2))
 
         elif self.template.type_name == "Chroma":
             # New bool field for persist parameter
-            extra_field = TemplateField(
-                name="persist",
-                field_type="bool",
-                required=False,
-                show=True,
-                advanced=False,
-                value=False,
-                display_name="Persist",
-            )
-            extra_fields.append(extra_field)
+            chroma_fields = [
+                TemplateField(
+                    name="persist",
+                    field_type="bool",
+                    required=False,
+                    show=True,
+                    advanced=False,
+                    value=False,
+                    display_name="Persist",
+                ),
+                # chroma_server_grpc_port: str | None = None,
+                TemplateField(
+                    name="chroma_server_host",
+                    field_type="str",
+                    required=False,
+                    show=True,
+                    advanced=True,
+                    display_name="Chroma Server Host",
+                ),
+                TemplateField(
+                    name="chroma_server_http_port",
+                    field_type="str",
+                    required=False,
+                    show=True,
+                    advanced=True,
+                    display_name="Chroma Server HTTP Port",
+                ),
+                TemplateField(
+                    name="chroma_server_ssl_enabled",
+                    field_type="bool",
+                    required=False,
+                    show=True,
+                    advanced=True,
+                    value=False,
+                    display_name="Chroma Server SSL Enabled",
+                ),
+                TemplateField(
+                    name="chroma_server_grpc_port",
+                    field_type="str",
+                    required=False,
+                    show=True,
+                    advanced=True,
+                    display_name="Chroma Server GRPC Port",
+                ),
+                TemplateField(
+                    name="chroma_server_cors_allow_origins",
+                    field_type="str",
+                    required=False,
+                    is_list=True,
+                    show=True,
+                    advanced=True,
+                    display_name="Chroma Server CORS Allow Origins",
+                ),
+            ]
+
+            extra_fields.extend(chroma_fields)
         elif self.template.type_name == "Pinecone":
             # add pinecone_api_key and pinecone_env
             extra_field = TemplateField(
                 name="pinecone_api_key",
                 field_type="str",
                 required=False,
                 placeholder="",
@@ -204,53 +296,14 @@
     def add_extra_base_classes(self) -> None:
         self.base_classes.extend(("BaseRetriever", "VectorStoreRetriever"))
 
     @staticmethod
     def format_field(field: TemplateField, name: Optional[str] = None) -> None:
         FrontendNode.format_field(field, name)
         # Define common field attributes
-        basic_fields = [
-            "work_dir",
-            "collection_name",
-            "api_key",
-            "location",
-            "persist_directory",
-            "persist",
-            "weaviate_url",
-            "index_name",
-            "namespace",
-            "folder_path",
-            "table_name",
-            "query_name",
-            "supabase_url",
-            "supabase_service_key",
-            "mongodb_atlas_cluster_uri",
-            "collection_name",
-            "db_name",
-        ]
-        advanced_fields = [
-            "n_dim",
-            "key",
-            "prefix",
-            "distance_func",
-            "content_payload_key",
-            "metadata_payload_key",
-            "timeout",
-            "host",
-            "path",
-            "url",
-            "port",
-            "https",
-            "prefer_grpc",
-            "grpc_port",
-            "pinecone_api_key",
-            "pinecone_env",
-            "client_kwargs",
-            "search_kwargs",
-        ]
 
         # Check and set field attributes
         if field.name == "texts":
             # if field.name is "texts" it has to be replaced
             # when instantiating the vectorstores
             field.name = "documents"
 
@@ -265,25 +318,25 @@
             field.name = "embedding"
             field.required = True
             field.show = True
             field.advanced = False
             field.display_name = "Embedding"
             field.field_type = "Embeddings"
 
-        elif field.name in basic_fields:
+        elif field.name in BASIC_FIELDS:
             field.show = True
             field.advanced = False
             if field.name == "api_key":
                 field.display_name = "API Key"
                 field.password = True
             elif field.name == "location":
                 field.value = ":memory:"
                 field.placeholder = ":memory:"
 
-        elif field.name in advanced_fields:
+        elif field.name in ADVANCED_FIELDS:
             field.show = True
             field.advanced = True
             if "key" in field.name:
                 field.password = False
 
         elif field.name == "text_key":
             field.show = False
```

### Comparing `langflow-0.4.1/src/backend/langflow/template/template/base.py` & `langflow-0.4.2/src/backend/langflow/template/template/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/utils/constants.py` & `langflow-0.4.2/src/backend/langflow/utils/constants.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/utils/logger.py` & `langflow-0.4.2/src/backend/langflow/utils/logger.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/utils/payload.py` & `langflow-0.4.2/src/backend/langflow/utils/payload.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/utils/util.py` & `langflow-0.4.2/src/backend/langflow/utils/util.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/src/backend/langflow/utils/validate.py` & `langflow-0.4.2/src/backend/langflow/utils/validate.py`

 * *Files identical despite different names*

### Comparing `langflow-0.4.1/PKG-INFO` & `langflow-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langflow
-Version: 0.4.1
+Version: 0.4.2
 Summary: A Python package with a built-in web application
 Home-page: https://github.com/logspace-ai/langflow
 License: MIT
 Keywords: nlp,langchain,openai,gpt,gui
 Author: Logspace
 Author-email: contact@logspace.ai
 Maintainer: Carlos Coelho
@@ -32,15 +32,15 @@
 Requires-Dist: fastavro (>=1.8.0,<2.0.0)
 Requires-Dist: google-api-python-client (>=2.79.0,<3.0.0)
 Requires-Dist: google-cloud-aiplatform (>=1.26.1,<2.0.0)
 Requires-Dist: google-search-results (>=2.4.1,<3.0.0)
 Requires-Dist: gunicorn (>=21.1.0,<22.0.0)
 Requires-Dist: huggingface-hub[inference] (>=0.16.0,<0.17.0)
 Requires-Dist: jina (==3.15.2)
-Requires-Dist: langchain (>=0.0.250,<0.0.251)
+Requires-Dist: langchain (>=0.0.256,<0.0.257)
 Requires-Dist: langchain-experimental (>=0.0.8,<0.0.9)
 Requires-Dist: langchain-serve (>0.0.51) ; extra == "deploy"
 Requires-Dist: llama-cpp-python (>=0.1.0,<0.2.0) ; extra == "local"
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: multiprocess (>=0.70.14,<0.71.0)
 Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: langflow Version: 0.4.1 Summary: A Python package
+Metadata-Version: 2.1 Name: langflow Version: 0.4.2 Summary: A Python package
 with a built-in web application Home-page: https://github.com/logspace-ai/
 langflow License: MIT Keywords: nlp,langchain,openai,gpt,gui Author: Logspace
 Author-email: contact@logspace.ai Maintainer: Carlos Coelho Maintainer-email:
 carlos@logspace.ai Requires-Python: >=3.9,<3.11 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Provides-Extra: all Provides-Extra: deploy Provides-
@@ -14,15 +14,15 @@
 "local" Requires-Dist: docstring-parser (>=0.15,<0.16) Requires-Dist: faiss-cpu
 (>=1.7.4,<2.0.0) Requires-Dist: fake-useragent (>=1.1.3,<2.0.0) Requires-Dist:
 fastapi (>=0.100.0,<0.101.0) Requires-Dist: fastavro (>=1.8.0,<2.0.0) Requires-
 Dist: google-api-python-client (>=2.79.0,<3.0.0) Requires-Dist: google-cloud-
 aiplatform (>=1.26.1,<2.0.0) Requires-Dist: google-search-results
 (>=2.4.1,<3.0.0) Requires-Dist: gunicorn (>=21.1.0,<22.0.0) Requires-Dist:
 huggingface-hub[inference] (>=0.16.0,<0.17.0) Requires-Dist: jina (==3.15.2)
-Requires-Dist: langchain (>=0.0.250,<0.0.251) Requires-Dist: langchain-
+Requires-Dist: langchain (>=0.0.256,<0.0.257) Requires-Dist: langchain-
 experimental (>=0.0.8,<0.0.9) Requires-Dist: langchain-serve (>0.0.51) ; extra
 == "deploy" Requires-Dist: llama-cpp-python (>=0.1.0,<0.2.0) ; extra == "local"
 Requires-Dist: lxml (>=4.9.2,<5.0.0) Requires-Dist: multiprocess
 (>=0.70.14,<0.71.0) Requires-Dist: networkx (>=3.1,<4.0) Requires-Dist: openai
 (>=0.27.8,<0.28.0) Requires-Dist: orjson (>=3.9.1,<4.0.0) Requires-Dist: pandas
 (>=2.0.0,<3.0.0) Requires-Dist: pinecone-client (>=2.2.2,<3.0.0) Requires-Dist:
 psycopg (>=3.1.9,<4.0.0) Requires-Dist: psycopg-binary (>=3.1.9,<4.0.0)
```

