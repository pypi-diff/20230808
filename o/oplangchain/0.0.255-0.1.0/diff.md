# Comparing `tmp/oplangchain-0.0.255.tar.gz` & `tmp/oplangchain-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oplangchain-0.0.255.tar", max compression
+gzip compressed data, was "oplangchain-0.1.0.tar", max compression
```

## Comparing `oplangchain-0.0.255.tar` & `oplangchain-0.1.0.tar`

### file list

```diff
@@ -1,972 +1,972 @@
--rw-r--r--   0        0        0     3074 2023-08-07 21:21:40.388154 oplangchain-0.0.255/oplangchain/__init__.py
--rw-r--r--   0        0        0     3396 2023-08-07 21:21:40.388154 oplangchain-0.0.255/oplangchain/agents/__init__.py
--rw-r--r--   0        0        0    41297 2023-08-07 21:21:40.389154 oplangchain-0.0.255/oplangchain/agents/agent.py
--rw-r--r--   0        0        0    18325 2023-08-07 21:21:40.389154 oplangchain-0.0.255/oplangchain/agents/agent_iterator.py
--rw-r--r--   0        0        0     3464 2023-08-07 21:21:40.390154 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/__init__.py
--rw-r--r--   0        0        0      873 2023-08-07 21:21:40.391155 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/amadeus/toolkit.py
--rw-r--r--   0        0        0      919 2023-08-07 21:21:40.391155 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/azure_cognitive_services.py
--rw-r--r--   0        0        0      369 2023-08-07 21:21:40.392155 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/base.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.393154 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/conversational_retrieval/__init__.py
--rw-r--r--   0        0        0     3377 2023-08-07 21:21:40.393154 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/conversational_retrieval/openai_functions.py
--rw-r--r--   0        0        0      730 2023-08-07 21:21:40.393154 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/conversational_retrieval/tool.py
--rw-r--r--   0        0        0       19 2023-08-07 21:21:40.394154 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/csv/__init__.py
--rw-r--r--   0        0        0     1148 2023-08-07 21:21:40.395155 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/csv/base.py
--rw-r--r--   0        0        0      174 2023-08-07 21:21:40.395155 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/file_management/__init__.py
--rw-r--r--   0        0        0     2074 2023-08-07 21:21:40.396155 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/file_management/toolkit.py
--rw-r--r--   0        0        0       22 2023-08-07 21:21:40.396155 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/github/__init__.py
--rw-r--r--   0        0        0     2484 2023-08-07 21:21:40.397154 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/github/toolkit.py
--rw-r--r--   0        0        0       21 2023-08-07 21:21:40.398154 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/gmail/__init__.py
--rw-r--r--   0        0        0     1567 2023-08-07 21:21:40.398154 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/gmail/toolkit.py
--rw-r--r--   0        0        0       20 2023-08-07 21:21:40.399153 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/jira/__init__.py
--rw-r--r--   0        0        0     1919 2023-08-07 21:21:40.399153 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/jira/toolkit.py
--rw-r--r--   0        0        0       18 2023-08-07 21:21:40.400153 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/json/__init__.py
--rw-r--r--   0        0        0     1713 2023-08-07 21:21:40.401154 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/json/base.py
--rw-r--r--   0        0        0     1819 2023-08-07 21:21:40.401154 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/json/prompt.py
--rw-r--r--   0        0        0      555 2023-08-07 21:21:40.401154 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/json/toolkit.py
--rw-r--r--   0        0        0       23 2023-08-07 21:21:40.402153 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/multion/__init__.py
--rw-r--r--   0        0        0      660 2023-08-07 21:21:40.402153 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/multion/toolkit.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.403154 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/nla/__init__.py
--rw-r--r--   0        0        0     1937 2023-08-07 21:21:40.404153 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/nla/tool.py
--rw-r--r--   0        0        0     3765 2023-08-07 21:21:40.404153 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/nla/toolkit.py
--rw-r--r--   0        0        0       25 2023-08-07 21:21:40.405154 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/office365/__init__.py
--rw-r--r--   0        0        0     1171 2023-08-07 21:21:40.405154 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/office365/toolkit.py
--rw-r--r--   0        0        0       26 2023-08-07 21:21:40.406154 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/openapi/__init__.py
--rw-r--r--   0        0        0     2140 2023-08-07 21:21:40.406154 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/openapi/base.py
--rw-r--r--   0        0        0    11233 2023-08-07 21:21:40.407153 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/openapi/planner.py
--rw-r--r--   0        0        0    10460 2023-08-07 21:21:40.407153 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/openapi/planner_prompt.py
--rw-r--r--   0        0        0     1743 2023-08-07 21:21:40.407153 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/openapi/prompt.py
--rw-r--r--   0        0        0     3835 2023-08-07 21:21:40.408153 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/openapi/spec.py
--rw-r--r--   0        0        0     2374 2023-08-07 21:21:40.408153 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/openapi/toolkit.py
--rw-r--r--   0        0        0       22 2023-08-07 21:21:40.409153 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/pandas/__init__.py
--rw-r--r--   0        0        0    11518 2023-08-07 21:21:40.410153 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/pandas/base.py
--rw-r--r--   0        0        0     1113 2023-08-07 21:21:40.410153 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/pandas/prompt.py
--rw-r--r--   0        0        0      162 2023-08-07 21:21:40.411153 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/playwright/__init__.py
--rw-r--r--   0        0        0     3014 2023-08-07 21:21:40.411153 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/playwright/toolkit.py
--rw-r--r--   0        0        0       22 2023-08-07 21:21:40.412153 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/powerbi/__init__.py
--rw-r--r--   0        0        0     2322 2023-08-07 21:21:40.412153 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/powerbi/base.py
--rw-r--r--   0        0        0     2489 2023-08-07 21:21:40.413154 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/powerbi/chat_base.py
--rw-r--r--   0        0        0     2773 2023-08-07 21:21:40.413154 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/powerbi/prompt.py
--rw-r--r--   0        0        0     3217 2023-08-07 21:21:40.413154 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/powerbi/toolkit.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.414153 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/python/__init__.py
--rw-r--r--   0        0        0     2200 2023-08-07 21:21:40.415153 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/python/base.py
--rw-r--r--   0        0        0      513 2023-08-07 21:21:40.415153 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/python/prompt.py
--rw-r--r--   0        0        0       20 2023-08-07 21:21:40.416154 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/spark/__init__.py
--rw-r--r--   0        0        0     2734 2023-08-07 21:21:40.416154 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/spark/base.py
--rw-r--r--   0        0        0      295 2023-08-07 21:21:40.416154 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/spark/prompt.py
--rw-r--r--   0        0        0       23 2023-08-07 21:21:40.417153 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/spark_sql/__init__.py
--rw-r--r--   0        0        0     2072 2023-08-07 21:21:40.418154 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/spark_sql/base.py
--rw-r--r--   0        0        0     1202 2023-08-07 21:21:40.418154 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/spark_sql/prompt.py
--rw-r--r--   0        0        0     1034 2023-08-07 21:21:40.418154 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/spark_sql/toolkit.py
--rw-r--r--   0        0        0       17 2023-08-07 21:21:40.419153 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/sql/__init__.py
--rw-r--r--   0        0        0     3434 2023-08-07 21:21:40.420153 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/sql/base.py
--rw-r--r--   0        0        0     1428 2023-08-07 21:21:40.420153 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/sql/prompt.py
--rw-r--r--   0        0        0     2816 2023-08-07 21:21:40.420153 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/sql/toolkit.py
--rw-r--r--   0        0        0       56 2023-08-07 21:21:40.421153 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/vectorstore/__init__.py
--rw-r--r--   0        0        0     2408 2023-08-07 21:21:40.422154 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/vectorstore/base.py
--rw-r--r--   0        0        0      834 2023-08-07 21:21:40.422154 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/vectorstore/prompt.py
--rw-r--r--   0        0        0     2961 2023-08-07 21:21:40.422154 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/vectorstore/toolkit.py
--rw-r--r--   0        0        0       23 2023-08-07 21:21:40.423153 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/xorbits/__init__.py
--rw-r--r--   0        0        0     3105 2023-08-07 21:21:40.424153 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/xorbits/base.py
--rw-r--r--   0        0        0     1070 2023-08-07 21:21:40.424153 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/xorbits/prompt.py
--rw-r--r--   0        0        0       22 2023-08-07 21:21:40.425154 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/zapier/__init__.py
--rw-r--r--   0        0        0     1609 2023-08-07 21:21:40.425154 oplangchain-0.0.255/oplangchain/agents/agent_toolkits/zapier/toolkit.py
--rw-r--r--   0        0        0      688 2023-08-07 21:21:40.426153 oplangchain-0.0.255/oplangchain/agents/agent_types.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.426153 oplangchain-0.0.255/oplangchain/agents/chat/__init__.py
--rw-r--r--   0        0        0     4908 2023-08-07 21:21:40.427153 oplangchain-0.0.255/oplangchain/agents/chat/base.py
--rw-r--r--   0        0        0     1706 2023-08-07 21:21:40.427153 oplangchain-0.0.255/oplangchain/agents/chat/output_parser.py
--rw-r--r--   0        0        0     1158 2023-08-07 21:21:40.427153 oplangchain-0.0.255/oplangchain/agents/chat/prompt.py
--rw-r--r--   0        0        0       75 2023-08-07 21:21:40.428154 oplangchain-0.0.255/oplangchain/agents/conversational/__init__.py
--rw-r--r--   0        0        0     4820 2023-08-07 21:21:40.429153 oplangchain-0.0.255/oplangchain/agents/conversational/base.py
--rw-r--r--   0        0        0     1150 2023-08-07 21:21:40.429153 oplangchain-0.0.255/oplangchain/agents/conversational/output_parser.py
--rw-r--r--   0        0        0     1859 2023-08-07 21:21:40.429153 oplangchain-0.0.255/oplangchain/agents/conversational/prompt.py
--rw-r--r--   0        0        0       75 2023-08-07 21:21:40.430153 oplangchain-0.0.255/oplangchain/agents/conversational_chat/__init__.py
--rw-r--r--   0        0        0     4977 2023-08-07 21:21:40.431155 oplangchain-0.0.255/oplangchain/agents/conversational_chat/base.py
--rw-r--r--   0        0        0     2256 2023-08-07 21:21:40.431155 oplangchain-0.0.255/oplangchain/agents/conversational_chat/output_parser.py
--rw-r--r--   0        0        0     2757 2023-08-07 21:21:40.431155 oplangchain-0.0.255/oplangchain/agents/conversational_chat/prompt.py
--rw-r--r--   0        0        0     2995 2023-08-07 21:21:40.432153 oplangchain-0.0.255/oplangchain/agents/initialize.py
--rw-r--r--   0        0        0    17319 2023-08-07 21:21:40.432153 oplangchain-0.0.255/oplangchain/agents/load_tools.py
--rw-r--r--   0        0        0     4371 2023-08-07 21:21:40.433153 oplangchain-0.0.255/oplangchain/agents/loading.py
--rw-r--r--   0        0        0       86 2023-08-07 21:21:40.433153 oplangchain-0.0.255/oplangchain/agents/mrkl/__init__.py
--rw-r--r--   0        0        0     7097 2023-08-07 21:21:40.434153 oplangchain-0.0.255/oplangchain/agents/mrkl/base.py
--rw-r--r--   0        0        0     2706 2023-08-07 21:21:40.434153 oplangchain-0.0.255/oplangchain/agents/mrkl/output_parser.py
--rw-r--r--   0        0        0      641 2023-08-07 21:21:40.435153 oplangchain-0.0.255/oplangchain/agents/mrkl/prompt.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.435153 oplangchain-0.0.255/oplangchain/agents/openai_functions_agent/__init__.py
--rw-r--r--   0        0        0     2527 2023-08-07 21:21:40.436153 oplangchain-0.0.255/oplangchain/agents/openai_functions_agent/agent_token_buffer_memory.py
--rw-r--r--   0        0        0    11896 2023-08-07 21:21:40.436153 oplangchain-0.0.255/oplangchain/agents/openai_functions_agent/base.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.437154 oplangchain-0.0.255/oplangchain/agents/openai_functions_multi_agent/__init__.py
--rw-r--r--   0        0        0    13337 2023-08-07 21:21:40.437154 oplangchain-0.0.255/oplangchain/agents/openai_functions_multi_agent/base.py
--rw-r--r--   0        0        0       76 2023-08-07 21:21:40.438153 oplangchain-0.0.255/oplangchain/agents/react/__init__.py
--rw-r--r--   0        0        0     5664 2023-08-07 21:21:40.439154 oplangchain-0.0.255/oplangchain/agents/react/base.py
--rw-r--r--   0        0        0     1188 2023-08-07 21:21:40.439154 oplangchain-0.0.255/oplangchain/agents/react/output_parser.py
--rw-r--r--   0        0        0     1901 2023-08-07 21:21:40.439154 oplangchain-0.0.255/oplangchain/agents/react/textworld_prompt.py
--rw-r--r--   0        0        0     6122 2023-08-07 21:21:40.440153 oplangchain-0.0.255/oplangchain/agents/react/wiki_prompt.py
--rw-r--r--   0        0        0     1085 2023-08-07 21:21:40.440153 oplangchain-0.0.255/oplangchain/agents/schema.py
--rw-r--r--   0        0        0      106 2023-08-07 21:21:40.441153 oplangchain-0.0.255/oplangchain/agents/self_ask_with_search/__init__.py
--rw-r--r--   0        0        0     3094 2023-08-07 21:21:40.441153 oplangchain-0.0.255/oplangchain/agents/self_ask_with_search/base.py
--rw-r--r--   0        0        0      962 2023-08-07 21:21:40.442155 oplangchain-0.0.255/oplangchain/agents/self_ask_with_search/output_parser.py
--rw-r--r--   0        0        0     1921 2023-08-07 21:21:40.442155 oplangchain-0.0.255/oplangchain/agents/self_ask_with_search/prompt.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.443153 oplangchain-0.0.255/oplangchain/agents/structured_chat/__init__.py
--rw-r--r--   0        0        0     5144 2023-08-07 21:21:40.443153 oplangchain-0.0.255/oplangchain/agents/structured_chat/base.py
--rw-r--r--   0        0        0     3452 2023-08-07 21:21:40.444153 oplangchain-0.0.255/oplangchain/agents/structured_chat/output_parser.py
--rw-r--r--   0        0        0      992 2023-08-07 21:21:40.444153 oplangchain-0.0.255/oplangchain/agents/structured_chat/prompt.py
--rw-r--r--   0        0        0     1402 2023-08-07 21:21:40.445153 oplangchain-0.0.255/oplangchain/agents/tools.py
--rw-r--r--   0        0        0     1475 2023-08-07 21:21:40.445153 oplangchain-0.0.255/oplangchain/agents/types.py
--rw-r--r--   0        0        0      384 2023-08-07 21:21:40.445153 oplangchain-0.0.255/oplangchain/agents/utils.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.446153 oplangchain-0.0.255/oplangchain/agents/xml/__init__.py
--rw-r--r--   0        0        0     3887 2023-08-07 21:21:40.447154 oplangchain-0.0.255/oplangchain/agents/xml/base.py
--rw-r--r--   0        0        0      749 2023-08-07 21:21:40.447154 oplangchain-0.0.255/oplangchain/agents/xml/prompt.py
--rw-r--r--   0        0        0      218 2023-08-07 21:21:40.447154 oplangchain-0.0.255/oplangchain/base_language.py
--rw-r--r--   0        0        0    24769 2023-08-07 21:21:40.448153 oplangchain-0.0.255/oplangchain/cache.py
--rw-r--r--   0        0        0     2839 2023-08-07 21:21:40.449154 oplangchain-0.0.255/oplangchain/callbacks/__init__.py
--rw-r--r--   0        0        0    14484 2023-08-07 21:21:40.449154 oplangchain-0.0.255/oplangchain/callbacks/aim_callback.py
--rw-r--r--   0        0        0    13719 2023-08-07 21:21:40.450154 oplangchain-0.0.255/oplangchain/callbacks/argilla_callback.py
--rw-r--r--   0        0        0     7503 2023-08-07 21:21:40.450154 oplangchain-0.0.255/oplangchain/callbacks/arize_callback.py
--rw-r--r--   0        0        0    11343 2023-08-07 21:21:40.451154 oplangchain-0.0.255/oplangchain/callbacks/arthur_callback.py
--rw-r--r--   0        0        0    15174 2023-08-07 21:21:40.451154 oplangchain-0.0.255/oplangchain/callbacks/base.py
--rw-r--r--   0        0        0    18496 2023-08-07 21:21:40.452155 oplangchain-0.0.255/oplangchain/callbacks/clearml_callback.py
--rw-r--r--   0        0        0    23238 2023-08-07 21:21:40.452155 oplangchain-0.0.255/oplangchain/callbacks/comet_ml_callback.py
--rw-r--r--   0        0        0     6424 2023-08-07 21:21:40.453153 oplangchain-0.0.255/oplangchain/callbacks/context_callback.py
--rw-r--r--   0        0        0     2561 2023-08-07 21:21:40.453153 oplangchain-0.0.255/oplangchain/callbacks/file.py
--rw-r--r--   0        0        0    13157 2023-08-07 21:21:40.454154 oplangchain-0.0.255/oplangchain/callbacks/flyte_callback.py
--rw-r--r--   0        0        0     1410 2023-08-07 21:21:40.454154 oplangchain-0.0.255/oplangchain/callbacks/human.py
--rw-r--r--   0        0        0     5570 2023-08-07 21:21:40.454154 oplangchain-0.0.255/oplangchain/callbacks/infino_callback.py
--rw-r--r--   0        0        0    53773 2023-08-07 21:21:40.455153 oplangchain-0.0.255/oplangchain/callbacks/manager.py
--rw-r--r--   0        0        0    24163 2023-08-07 21:21:40.455153 oplangchain-0.0.255/oplangchain/callbacks/mlflow_callback.py
--rw-r--r--   0        0        0     5348 2023-08-07 21:21:40.456153 oplangchain-0.0.255/oplangchain/callbacks/openai_info.py
--rw-r--r--   0        0        0     5523 2023-08-07 21:21:40.456153 oplangchain-0.0.255/oplangchain/callbacks/promptlayer_callback.py
--rw-r--r--   0        0        0     8823 2023-08-07 21:21:40.457154 oplangchain-0.0.255/oplangchain/callbacks/sagemaker_callback.py
--rw-r--r--   0        0        0     3203 2023-08-07 21:21:40.457154 oplangchain-0.0.255/oplangchain/callbacks/stdout.py
--rw-r--r--   0        0        0     2436 2023-08-07 21:21:40.457154 oplangchain-0.0.255/oplangchain/callbacks/streaming_aiter.py
--rw-r--r--   0        0        0     3364 2023-08-07 21:21:40.458154 oplangchain-0.0.255/oplangchain/callbacks/streaming_aiter_final_only.py
--rw-r--r--   0        0        0     2170 2023-08-07 21:21:40.458154 oplangchain-0.0.255/oplangchain/callbacks/streaming_stdout.py
--rw-r--r--   0        0        0     3368 2023-08-07 21:21:40.459153 oplangchain-0.0.255/oplangchain/callbacks/streaming_stdout_final_only.py
--rw-r--r--   0        0        0     3190 2023-08-07 21:21:40.459153 oplangchain-0.0.255/oplangchain/callbacks/streamlit/__init__.py
--rw-r--r--   0        0        0     5435 2023-08-07 21:21:40.460153 oplangchain-0.0.255/oplangchain/callbacks/streamlit/mutable_expander.py
--rw-r--r--   0        0        0    15671 2023-08-07 21:21:40.461154 oplangchain-0.0.255/oplangchain/callbacks/streamlit/streamlit_callback_handler.py
--rw-r--r--   0        0        0      502 2023-08-07 21:21:40.461154 oplangchain-0.0.255/oplangchain/callbacks/tracers/__init__.py
--rw-r--r--   0        0        0    17018 2023-08-07 21:21:40.462154 oplangchain-0.0.255/oplangchain/callbacks/tracers/base.py
--rw-r--r--   0        0        0     4858 2023-08-07 21:21:40.462154 oplangchain-0.0.255/oplangchain/callbacks/tracers/evaluation.py
--rw-r--r--   0        0        0     8055 2023-08-07 21:21:40.463154 oplangchain-0.0.255/oplangchain/callbacks/tracers/langchain.py
--rw-r--r--   0        0        0     7362 2023-08-07 21:21:40.463154 oplangchain-0.0.255/oplangchain/callbacks/tracers/langchain_v1.py
--rw-r--r--   0        0        0     1537 2023-08-07 21:21:40.464154 oplangchain-0.0.255/oplangchain/callbacks/tracers/run_collector.py
--rw-r--r--   0        0        0     3456 2023-08-07 21:21:40.464154 oplangchain-0.0.255/oplangchain/callbacks/tracers/schemas.py
--rw-r--r--   0        0        0     6027 2023-08-07 21:21:40.464154 oplangchain-0.0.255/oplangchain/callbacks/tracers/stdout.py
--rw-r--r--   0        0        0    18983 2023-08-07 21:21:40.465154 oplangchain-0.0.255/oplangchain/callbacks/tracers/wandb.py
--rw-r--r--   0        0        0     8505 2023-08-07 21:21:40.465154 oplangchain-0.0.255/oplangchain/callbacks/utils.py
--rw-r--r--   0        0        0    20659 2023-08-07 21:21:40.466154 oplangchain-0.0.255/oplangchain/callbacks/wandb_callback.py
--rw-r--r--   0        0        0     8062 2023-08-07 21:21:40.466154 oplangchain-0.0.255/oplangchain/callbacks/whylabs_callback.py
--rw-r--r--   0        0        0     5294 2023-08-07 21:21:40.467154 oplangchain-0.0.255/oplangchain/chains/__init__.py
--rw-r--r--   0        0        0       84 2023-08-07 21:21:40.468155 oplangchain-0.0.255/oplangchain/chains/api/__init__.py
--rw-r--r--   0        0        0     5334 2023-08-07 21:21:40.468155 oplangchain-0.0.255/oplangchain/chains/api/base.py
--rw-r--r--   0        0        0     2452 2023-08-07 21:21:40.469154 oplangchain-0.0.255/oplangchain/chains/api/news_docs.py
--rw-r--r--   0        0        0     3399 2023-08-07 21:21:40.469154 oplangchain-0.0.255/oplangchain/chains/api/open_meteo_docs.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.470153 oplangchain-0.0.255/oplangchain/chains/api/openapi/__init__.py
--rw-r--r--   0        0        0     8750 2023-08-07 21:21:40.471154 oplangchain-0.0.255/oplangchain/chains/api/openapi/chain.py
--rw-r--r--   0        0        0     1791 2023-08-07 21:21:40.471154 oplangchain-0.0.255/oplangchain/chains/api/openapi/prompts.py
--rw-r--r--   0        0        0     1877 2023-08-07 21:21:40.471154 oplangchain-0.0.255/oplangchain/chains/api/openapi/requests_chain.py
--rw-r--r--   0        0        0     1749 2023-08-07 21:21:40.472154 oplangchain-0.0.255/oplangchain/chains/api/openapi/response_chain.py
--rw-r--r--   0        0        0     1920 2023-08-07 21:21:40.472154 oplangchain-0.0.255/oplangchain/chains/api/podcast_docs.py
--rw-r--r--   0        0        0     1026 2023-08-07 21:21:40.473154 oplangchain-0.0.255/oplangchain/chains/api/prompt.py
--rw-r--r--   0        0        0     1537 2023-08-07 21:21:40.473154 oplangchain-0.0.255/oplangchain/chains/api/tmdb_docs.py
--rw-r--r--   0        0        0    24814 2023-08-07 21:21:40.474154 oplangchain-0.0.255/oplangchain/chains/base.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.474154 oplangchain-0.0.255/oplangchain/chains/chat_vector_db/__init__.py
--rw-r--r--   0        0        0      689 2023-08-07 21:21:40.475154 oplangchain-0.0.255/oplangchain/chains/chat_vector_db/prompts.py
--rw-r--r--   0        0        0       43 2023-08-07 21:21:40.475154 oplangchain-0.0.255/oplangchain/chains/combine_documents/__init__.py
--rw-r--r--   0        0        0     6390 2023-08-07 21:21:40.476154 oplangchain-0.0.255/oplangchain/chains/combine_documents/base.py
--rw-r--r--   0        0        0    11149 2023-08-07 21:21:40.476154 oplangchain-0.0.255/oplangchain/chains/combine_documents/map_reduce.py
--rw-r--r--   0        0        0     8368 2023-08-07 21:21:40.477154 oplangchain-0.0.255/oplangchain/chains/combine_documents/map_rerank.py
--rw-r--r--   0        0        0    11004 2023-08-07 21:21:40.477154 oplangchain-0.0.255/oplangchain/chains/combine_documents/reduce.py
--rw-r--r--   0        0        0     9075 2023-08-07 21:21:40.478154 oplangchain-0.0.255/oplangchain/chains/combine_documents/refine.py
--rw-r--r--   0        0        0     7658 2023-08-07 21:21:40.478154 oplangchain-0.0.255/oplangchain/chains/combine_documents/stuff.py
--rw-r--r--   0        0        0      107 2023-08-07 21:21:40.479154 oplangchain-0.0.255/oplangchain/chains/constitutional_ai/__init__.py
--rw-r--r--   0        0        0     6328 2023-08-07 21:21:40.479154 oplangchain-0.0.255/oplangchain/chains/constitutional_ai/base.py
--rw-r--r--   0        0        0      265 2023-08-07 21:21:40.480154 oplangchain-0.0.255/oplangchain/chains/constitutional_ai/models.py
--rw-r--r--   0        0        0    21738 2023-08-07 21:21:40.480154 oplangchain-0.0.255/oplangchain/chains/constitutional_ai/principles.py
--rw-r--r--   0        0        0     8656 2023-08-07 21:21:40.481155 oplangchain-0.0.255/oplangchain/chains/constitutional_ai/prompts.py
--rw-r--r--   0        0        0       71 2023-08-07 21:21:40.482154 oplangchain-0.0.255/oplangchain/chains/conversation/__init__.py
--rw-r--r--   0        0        0     2174 2023-08-07 21:21:40.482154 oplangchain-0.0.255/oplangchain/chains/conversation/base.py
--rw-r--r--   0        0        0      856 2023-08-07 21:21:40.482154 oplangchain-0.0.255/oplangchain/chains/conversation/memory.py
--rw-r--r--   0        0        0      908 2023-08-07 21:21:40.483153 oplangchain-0.0.255/oplangchain/chains/conversation/prompt.py
--rw-r--r--   0        0        0       49 2023-08-07 21:21:40.484154 oplangchain-0.0.255/oplangchain/chains/conversational_retrieval/__init__.py
--rw-r--r--   0        0        0    16705 2023-08-07 21:21:40.484154 oplangchain-0.0.255/oplangchain/chains/conversational_retrieval/base.py
--rw-r--r--   0        0        0      715 2023-08-07 21:21:40.485153 oplangchain-0.0.255/oplangchain/chains/conversational_retrieval/prompts.py
--rw-r--r--   0        0        0      126 2023-08-07 21:21:40.485153 oplangchain-0.0.255/oplangchain/chains/elasticsearch_database/__init__.py
--rw-r--r--   0        0        0     8166 2023-08-07 21:21:40.486154 oplangchain-0.0.255/oplangchain/chains/elasticsearch_database/base.py
--rw-r--r--   0        0        0     1420 2023-08-07 21:21:40.486154 oplangchain-0.0.255/oplangchain/chains/elasticsearch_database/prompts.py
--rw-r--r--   0        0        0      731 2023-08-07 21:21:40.487153 oplangchain-0.0.255/oplangchain/chains/example_generator.py
--rw-r--r--   0        0        0       51 2023-08-07 21:21:40.487153 oplangchain-0.0.255/oplangchain/chains/flare/__init__.py
--rw-r--r--   0        0        0     8765 2023-08-07 21:21:40.488154 oplangchain-0.0.255/oplangchain/chains/flare/base.py
--rw-r--r--   0        0        0     1453 2023-08-07 21:21:40.488154 oplangchain-0.0.255/oplangchain/chains/flare/prompts.py
--rw-r--r--   0        0        0       49 2023-08-07 21:21:40.489153 oplangchain-0.0.255/oplangchain/chains/graph_qa/__init__.py
--rw-r--r--   0        0        0     7676 2023-08-07 21:21:40.489153 oplangchain-0.0.255/oplangchain/chains/graph_qa/arangodb.py
--rw-r--r--   0        0        0     2970 2023-08-07 21:21:40.490153 oplangchain-0.0.255/oplangchain/chains/graph_qa/base.py
--rw-r--r--   0        0        0     4586 2023-08-07 21:21:40.490153 oplangchain-0.0.255/oplangchain/chains/graph_qa/cypher.py
--rw-r--r--   0        0        0     3019 2023-08-07 21:21:40.490153 oplangchain-0.0.255/oplangchain/chains/graph_qa/hugegraph.py
--rw-r--r--   0        0        0     3019 2023-08-07 21:21:40.491153 oplangchain-0.0.255/oplangchain/chains/graph_qa/kuzu.py
--rw-r--r--   0        0        0     2994 2023-08-07 21:21:40.491153 oplangchain-0.0.255/oplangchain/chains/graph_qa/nebulagraph.py
--rw-r--r--   0        0        0     4479 2023-08-07 21:21:40.492154 oplangchain-0.0.255/oplangchain/chains/graph_qa/neptune_cypher.py
--rw-r--r--   0        0        0    13728 2023-08-07 21:21:40.492154 oplangchain-0.0.255/oplangchain/chains/graph_qa/prompts.py
--rw-r--r--   0        0        0     4771 2023-08-07 21:21:40.493153 oplangchain-0.0.255/oplangchain/chains/graph_qa/sparql.py
--rw-r--r--   0        0        0       75 2023-08-07 21:21:40.493153 oplangchain-0.0.255/oplangchain/chains/hyde/__init__.py
--rw-r--r--   0        0        0     2831 2023-08-07 21:21:40.494154 oplangchain-0.0.255/oplangchain/chains/hyde/base.py
--rw-r--r--   0        0        0     1908 2023-08-07 21:21:40.494154 oplangchain-0.0.255/oplangchain/chains/hyde/prompts.py
--rw-r--r--   0        0        0    12141 2023-08-07 21:21:40.495154 oplangchain-0.0.255/oplangchain/chains/llm.py
--rw-r--r--   0        0        0       88 2023-08-07 21:21:40.495154 oplangchain-0.0.255/oplangchain/chains/llm_bash/__init__.py
--rw-r--r--   0        0        0     4165 2023-08-07 21:21:40.496153 oplangchain-0.0.255/oplangchain/chains/llm_bash/base.py
--rw-r--r--   0        0        0     1937 2023-08-07 21:21:40.496153 oplangchain-0.0.255/oplangchain/chains/llm_bash/prompt.py
--rw-r--r--   0        0        0      139 2023-08-07 21:21:40.497153 oplangchain-0.0.255/oplangchain/chains/llm_checker/__init__.py
--rw-r--r--   0        0        0     6090 2023-08-07 21:21:40.497153 oplangchain-0.0.255/oplangchain/chains/llm_checker/base.py
--rw-r--r--   0        0        0     1120 2023-08-07 21:21:40.498153 oplangchain-0.0.255/oplangchain/chains/llm_checker/prompt.py
--rw-r--r--   0        0        0      143 2023-08-07 21:21:40.499153 oplangchain-0.0.255/oplangchain/chains/llm_math/__init__.py
--rw-r--r--   0        0        0     6372 2023-08-07 21:21:40.499153 oplangchain-0.0.255/oplangchain/chains/llm_math/base.py
--rw-r--r--   0        0        0      863 2023-08-07 21:21:40.499153 oplangchain-0.0.255/oplangchain/chains/llm_math/prompt.py
--rw-r--r--   0        0        0     2877 2023-08-07 21:21:40.500154 oplangchain-0.0.255/oplangchain/chains/llm_requests.py
--rw-r--r--   0        0        0      352 2023-08-07 21:21:40.500154 oplangchain-0.0.255/oplangchain/chains/llm_summarization_checker/__init__.py
--rw-r--r--   0        0        0     6606 2023-08-07 21:21:40.501153 oplangchain-0.0.255/oplangchain/chains/llm_summarization_checker/base.py
--rw-r--r--   0        0        0      654 2023-08-07 21:21:40.502153 oplangchain-0.0.255/oplangchain/chains/llm_summarization_checker/prompts/are_all_true_prompt.txt
--rw-r--r--   0        0        0      377 2023-08-07 21:21:40.502153 oplangchain-0.0.255/oplangchain/chains/llm_summarization_checker/prompts/check_facts.txt
--rw-r--r--   0        0        0      128 2023-08-07 21:21:40.503153 oplangchain-0.0.255/oplangchain/chains/llm_summarization_checker/prompts/create_facts.txt
--rw-r--r--   0        0        0      416 2023-08-07 21:21:40.503153 oplangchain-0.0.255/oplangchain/chains/llm_summarization_checker/prompts/revise_summary.txt
--rw-r--r--   0        0        0      126 2023-08-07 21:21:40.504153 oplangchain-0.0.255/oplangchain/chains/llm_symbolic_math/__init__.py
--rw-r--r--   0        0        0     5555 2023-08-07 21:21:40.504153 oplangchain-0.0.255/oplangchain/chains/llm_symbolic_math/base.py
--rw-r--r--   0        0        0     1087 2023-08-07 21:21:40.505153 oplangchain-0.0.255/oplangchain/chains/llm_symbolic_math/prompt.py
--rw-r--r--   0        0        0    23945 2023-08-07 21:21:40.505153 oplangchain-0.0.255/oplangchain/chains/loading.py
--rw-r--r--   0        0        0     3715 2023-08-07 21:21:40.505153 oplangchain-0.0.255/oplangchain/chains/mapreduce.py
--rw-r--r--   0        0        0     3050 2023-08-07 21:21:40.506153 oplangchain-0.0.255/oplangchain/chains/moderation.py
--rw-r--r--   0        0        0       96 2023-08-07 21:21:40.507154 oplangchain-0.0.255/oplangchain/chains/natbot/__init__.py
--rw-r--r--   0        0        0     4179 2023-08-07 21:21:40.507154 oplangchain-0.0.255/oplangchain/chains/natbot/base.py
--rw-r--r--   0        0        0    15466 2023-08-07 21:21:40.508154 oplangchain-0.0.255/oplangchain/chains/natbot/crawler.py
--rw-r--r--   0        0        0     4984 2023-08-07 21:21:40.508154 oplangchain-0.0.255/oplangchain/chains/natbot/prompt.py
--rw-r--r--   0        0        0      948 2023-08-07 21:21:40.509153 oplangchain-0.0.255/oplangchain/chains/openai_functions/__init__.py
--rw-r--r--   0        0        0    14608 2023-08-07 21:21:40.509153 oplangchain-0.0.255/oplangchain/chains/openai_functions/base.py
--rw-r--r--   0        0        0     3506 2023-08-07 21:21:40.510153 oplangchain-0.0.255/oplangchain/chains/openai_functions/citation_fuzzy_match.py
--rw-r--r--   0        0        0     3338 2023-08-07 21:21:40.510153 oplangchain-0.0.255/oplangchain/chains/openai_functions/extraction.py
--rw-r--r--   0        0        0    11162 2023-08-07 21:21:40.511155 oplangchain-0.0.255/oplangchain/chains/openai_functions/openapi.py
--rw-r--r--   0        0        0     3709 2023-08-07 21:21:40.511155 oplangchain-0.0.255/oplangchain/chains/openai_functions/qa_with_structure.py
--rw-r--r--   0        0        0     2653 2023-08-07 21:21:40.512154 oplangchain-0.0.255/oplangchain/chains/openai_functions/tagging.py
--rw-r--r--   0        0        0     1257 2023-08-07 21:21:40.512154 oplangchain-0.0.255/oplangchain/chains/openai_functions/utils.py
--rw-r--r--   0        0        0     1961 2023-08-07 21:21:40.512154 oplangchain-0.0.255/oplangchain/chains/prompt_selector.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.513154 oplangchain-0.0.255/oplangchain/chains/qa_generation/__init__.py
--rw-r--r--   0        0        0     2444 2023-08-07 21:21:40.514154 oplangchain-0.0.255/oplangchain/chains/qa_generation/base.py
--rw-r--r--   0        0        0     1865 2023-08-07 21:21:40.514154 oplangchain-0.0.255/oplangchain/chains/qa_generation/prompt.py
--rw-r--r--   0        0        0      173 2023-08-07 21:21:40.515154 oplangchain-0.0.255/oplangchain/chains/qa_with_sources/__init__.py
--rw-r--r--   0        0        0     7717 2023-08-07 21:21:40.515154 oplangchain-0.0.255/oplangchain/chains/qa_with_sources/base.py
--rw-r--r--   0        0        0     6803 2023-08-07 21:21:40.516154 oplangchain-0.0.255/oplangchain/chains/qa_with_sources/loading.py
--rw-r--r--   0        0        0     6966 2023-08-07 21:21:40.516154 oplangchain-0.0.255/oplangchain/chains/qa_with_sources/map_reduce_prompt.py
--rw-r--r--   0        0        0     1313 2023-08-07 21:21:40.517154 oplangchain-0.0.255/oplangchain/chains/qa_with_sources/refine_prompts.py
--rw-r--r--   0        0        0     2344 2023-08-07 21:21:40.517154 oplangchain-0.0.255/oplangchain/chains/qa_with_sources/retrieval.py
--rw-r--r--   0        0        0     6576 2023-08-07 21:21:40.518154 oplangchain-0.0.255/oplangchain/chains/qa_with_sources/stuff_prompt.py
--rw-r--r--   0        0        0     2799 2023-08-07 21:21:40.518154 oplangchain-0.0.255/oplangchain/chains/qa_with_sources/vector_db.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.519154 oplangchain-0.0.255/oplangchain/chains/query_constructor/__init__.py
--rw-r--r--   0        0        0     5808 2023-08-07 21:21:40.519154 oplangchain-0.0.255/oplangchain/chains/query_constructor/base.py
--rw-r--r--   0        0        0     3129 2023-08-07 21:21:40.520154 oplangchain-0.0.255/oplangchain/chains/query_constructor/ir.py
--rw-r--r--   0        0        0     4752 2023-08-07 21:21:40.520154 oplangchain-0.0.255/oplangchain/chains/query_constructor/parser.py
--rw-r--r--   0        0        0     6446 2023-08-07 21:21:40.520154 oplangchain-0.0.255/oplangchain/chains/query_constructor/prompt.py
--rw-r--r--   0        0        0      303 2023-08-07 21:21:40.521153 oplangchain-0.0.255/oplangchain/chains/query_constructor/schema.py
--rw-r--r--   0        0        0     8552 2023-08-07 21:21:40.522154 oplangchain-0.0.255/oplangchain/chains/question_answering/__init__.py
--rw-r--r--   0        0        0     8003 2023-08-07 21:21:40.522154 oplangchain-0.0.255/oplangchain/chains/question_answering/map_reduce_prompt.py
--rw-r--r--   0        0        0     1617 2023-08-07 21:21:40.523154 oplangchain-0.0.255/oplangchain/chains/question_answering/map_rerank_prompt.py
--rw-r--r--   0        0        0     2726 2023-08-07 21:21:40.523154 oplangchain-0.0.255/oplangchain/chains/question_answering/refine_prompts.py
--rw-r--r--   0        0        0     1135 2023-08-07 21:21:40.524154 oplangchain-0.0.255/oplangchain/chains/question_answering/stuff_prompt.py
--rw-r--r--   0        0        0       62 2023-08-07 21:21:40.524154 oplangchain-0.0.255/oplangchain/chains/retrieval_qa/__init__.py
--rw-r--r--   0        0        0     9762 2023-08-07 21:21:40.525154 oplangchain-0.0.255/oplangchain/chains/retrieval_qa/base.py
--rw-r--r--   0        0        0      394 2023-08-07 21:21:40.525154 oplangchain-0.0.255/oplangchain/chains/retrieval_qa/prompt.py
--rw-r--r--   0        0        0      407 2023-08-07 21:21:40.526154 oplangchain-0.0.255/oplangchain/chains/router/__init__.py
--rw-r--r--   0        0        0     4556 2023-08-07 21:21:40.526154 oplangchain-0.0.255/oplangchain/chains/router/base.py
--rw-r--r--   0        0        0     1970 2023-08-07 21:21:40.527154 oplangchain-0.0.255/oplangchain/chains/router/embedding_router.py
--rw-r--r--   0        0        0     4185 2023-08-07 21:21:40.527154 oplangchain-0.0.255/oplangchain/chains/router/llm_router.py
--rw-r--r--   0        0        0     2562 2023-08-07 21:21:40.528154 oplangchain-0.0.255/oplangchain/chains/router/multi_prompt.py
--rw-r--r--   0        0        0     1123 2023-08-07 21:21:40.528154 oplangchain-0.0.255/oplangchain/chains/router/multi_prompt_prompt.py
--rw-r--r--   0        0        0     1079 2023-08-07 21:21:40.528154 oplangchain-0.0.255/oplangchain/chains/router/multi_retrieval_prompt.py
--rw-r--r--   0        0        0     3635 2023-08-07 21:21:40.529154 oplangchain-0.0.255/oplangchain/chains/router/multi_retrieval_qa.py
--rw-r--r--   0        0        0     7481 2023-08-07 21:21:40.529154 oplangchain-0.0.255/oplangchain/chains/sequential.py
--rw-r--r--   0        0        0       47 2023-08-07 21:21:40.530154 oplangchain-0.0.255/oplangchain/chains/sql_database/__init__.py
--rw-r--r--   0        0        0    14202 2023-08-07 21:21:40.530154 oplangchain-0.0.255/oplangchain/chains/sql_database/prompt.py
--rw-r--r--   0        0        0     2066 2023-08-07 21:21:40.531154 oplangchain-0.0.255/oplangchain/chains/sql_database/query.py
--rw-r--r--   0        0        0     5695 2023-08-07 21:21:40.532154 oplangchain-0.0.255/oplangchain/chains/summarize/__init__.py
--rw-r--r--   0        0        0      233 2023-08-07 21:21:40.532154 oplangchain-0.0.255/oplangchain/chains/summarize/map_reduce_prompt.py
--rw-r--r--   0        0        0      805 2023-08-07 21:21:40.532154 oplangchain-0.0.255/oplangchain/chains/summarize/refine_prompts.py
--rw-r--r--   0        0        0      233 2023-08-07 21:21:40.533154 oplangchain-0.0.255/oplangchain/chains/summarize/stuff_prompt.py
--rw-r--r--   0        0        0     2233 2023-08-07 21:21:40.533154 oplangchain-0.0.255/oplangchain/chains/transform.py
--rw-r--r--   0        0        0     1354 2023-08-07 21:21:40.534154 oplangchain-0.0.255/oplangchain/chat_models/__init__.py
--rw-r--r--   0        0        0     6988 2023-08-07 21:21:40.535154 oplangchain-0.0.255/oplangchain/chat_models/anthropic.py
--rw-r--r--   0        0        0     4707 2023-08-07 21:21:40.535154 oplangchain-0.0.255/oplangchain/chat_models/azure_openai.py
--rw-r--r--   0        0        0     5396 2023-08-07 21:21:40.536154 oplangchain-0.0.255/oplangchain/chat_models/azureml_endpoint.py
--rw-r--r--   0        0        0    23270 2023-08-07 21:21:40.536154 oplangchain-0.0.255/oplangchain/chat_models/base.py
--rw-r--r--   0        0        0     1040 2023-08-07 21:21:40.537154 oplangchain-0.0.255/oplangchain/chat_models/fake.py
--rw-r--r--   0        0        0    11127 2023-08-07 21:21:40.537154 oplangchain-0.0.255/oplangchain/chat_models/google_palm.py
--rw-r--r--   0        0        0     4017 2023-08-07 21:21:40.537154 oplangchain-0.0.255/oplangchain/chat_models/human.py
--rw-r--r--   0        0        0    15223 2023-08-07 21:21:40.538154 oplangchain-0.0.255/oplangchain/chat_models/jinachat.py
--rw-r--r--   0        0        0     6855 2023-08-07 21:21:40.538154 oplangchain-0.0.255/oplangchain/chat_models/mlflow_ai_gateway.py
--rw-r--r--   0        0        0    22364 2023-08-07 21:21:40.539155 oplangchain-0.0.255/oplangchain/chat_models/openai.py
--rw-r--r--   0        0        0     5164 2023-08-07 21:21:40.539155 oplangchain-0.0.255/oplangchain/chat_models/promptlayer_openai.py
--rw-r--r--   0        0        0     6006 2023-08-07 21:21:40.540154 oplangchain-0.0.255/oplangchain/chat_models/vertexai.py
--rw-r--r--   0        0        0      685 2023-08-07 21:21:40.540154 oplangchain-0.0.255/oplangchain/docker-compose.yaml
--rw-r--r--   0        0        0      519 2023-08-07 21:21:40.541154 oplangchain-0.0.255/oplangchain/docstore/__init__.py
--rw-r--r--   0        0        0     1071 2023-08-07 21:21:40.541154 oplangchain-0.0.255/oplangchain/docstore/arbitrary_fn.py
--rw-r--r--   0        0        0      836 2023-08-07 21:21:40.542154 oplangchain-0.0.255/oplangchain/docstore/base.py
--rw-r--r--   0        0        0       62 2023-08-07 21:21:40.542154 oplangchain-0.0.255/oplangchain/docstore/document.py
--rw-r--r--   0        0        0     1602 2023-08-07 21:21:40.543154 oplangchain-0.0.255/oplangchain/docstore/in_memory.py
--rw-r--r--   0        0        0     1479 2023-08-07 21:21:40.543154 oplangchain-0.0.255/oplangchain/docstore/wikipedia.py
--rw-r--r--   0        0        0    12884 2023-08-07 21:21:40.544154 oplangchain-0.0.255/oplangchain/document_loaders/__init__.py
--rw-r--r--   0        0        0     2847 2023-08-07 21:21:40.544154 oplangchain-0.0.255/oplangchain/document_loaders/acreom.py
--rw-r--r--   0        0        0      839 2023-08-07 21:21:40.545154 oplangchain-0.0.255/oplangchain/document_loaders/airbyte_json.py
--rw-r--r--   0        0        0     1273 2023-08-07 21:21:40.545154 oplangchain-0.0.255/oplangchain/document_loaders/airtable.py
--rw-r--r--   0        0        0     2716 2023-08-07 21:21:40.546153 oplangchain-0.0.255/oplangchain/document_loaders/apify_dataset.py
--rw-r--r--   0        0        0     1138 2023-08-07 21:21:40.546153 oplangchain-0.0.255/oplangchain/document_loaders/arxiv.py
--rw-r--r--   0        0        0     4861 2023-08-07 21:21:40.546153 oplangchain-0.0.255/oplangchain/document_loaders/async_html.py
--rw-r--r--   0        0        0      576 2023-08-07 21:21:40.547154 oplangchain-0.0.255/oplangchain/document_loaders/azlyrics.py
--rw-r--r--   0        0        0     1612 2023-08-07 21:21:40.547154 oplangchain-0.0.255/oplangchain/document_loaders/azure_blob_storage_container.py
--rw-r--r--   0        0        0     1631 2023-08-07 21:21:40.548154 oplangchain-0.0.255/oplangchain/document_loaders/azure_blob_storage_file.py
--rw-r--r--   0        0        0     3041 2023-08-07 21:21:40.548154 oplangchain-0.0.255/oplangchain/document_loaders/base.py
--rw-r--r--   0        0        0     3928 2023-08-07 21:21:40.549154 oplangchain-0.0.255/oplangchain/document_loaders/bibtex.py
--rw-r--r--   0        0        0     3147 2023-08-07 21:21:40.549154 oplangchain-0.0.255/oplangchain/document_loaders/bigquery.py
--rw-r--r--   0        0        0     2722 2023-08-07 21:21:40.549154 oplangchain-0.0.255/oplangchain/document_loaders/bilibili.py
--rw-r--r--   0        0        0    10089 2023-08-07 21:21:40.550154 oplangchain-0.0.255/oplangchain/document_loaders/blackboard.py
--rw-r--r--   0        0        0      326 2023-08-07 21:21:40.551154 oplangchain-0.0.255/oplangchain/document_loaders/blob_loaders/__init__.py
--rw-r--r--   0        0        0     4279 2023-08-07 21:21:40.551154 oplangchain-0.0.255/oplangchain/document_loaders/blob_loaders/file_system.py
--rw-r--r--   0        0        0     5765 2023-08-07 21:21:40.551154 oplangchain-0.0.255/oplangchain/document_loaders/blob_loaders/schema.py
--rw-r--r--   0        0        0     1506 2023-08-07 21:21:40.552154 oplangchain-0.0.255/oplangchain/document_loaders/blob_loaders/youtube_audio.py
--rw-r--r--   0        0        0     5728 2023-08-07 21:21:40.552154 oplangchain-0.0.255/oplangchain/document_loaders/blockchain.py
--rw-r--r--   0        0        0     1068 2023-08-07 21:21:40.553154 oplangchain-0.0.255/oplangchain/document_loaders/brave_search.py
--rw-r--r--   0        0        0     2132 2023-08-07 21:21:40.553154 oplangchain-0.0.255/oplangchain/document_loaders/browserless.py
--rw-r--r--   0        0        0     2026 2023-08-07 21:21:40.554154 oplangchain-0.0.255/oplangchain/document_loaders/chatgpt.py
--rw-r--r--   0        0        0      552 2023-08-07 21:21:40.554154 oplangchain-0.0.255/oplangchain/document_loaders/college_confidential.py
--rw-r--r--   0        0        0     2143 2023-08-07 21:21:40.554154 oplangchain-0.0.255/oplangchain/document_loaders/concurrent.py
--rw-r--r--   0        0        0    25397 2023-08-07 21:21:40.555154 oplangchain-0.0.255/oplangchain/document_loaders/confluence.py
--rw-r--r--   0        0        0     1068 2023-08-07 21:21:40.556154 oplangchain-0.0.255/oplangchain/document_loaders/conllu.py
--rw-r--r--   0        0        0     4195 2023-08-07 21:21:40.556154 oplangchain-0.0.255/oplangchain/document_loaders/csv_loader.py
--rw-r--r--   0        0        0     5901 2023-08-07 21:21:40.556154 oplangchain-0.0.255/oplangchain/document_loaders/cube_semantic.py
--rw-r--r--   0        0        0     4993 2023-08-07 21:21:40.557154 oplangchain-0.0.255/oplangchain/document_loaders/datadog_logs.py
--rw-r--r--   0        0        0     1325 2023-08-07 21:21:40.557154 oplangchain-0.0.255/oplangchain/document_loaders/dataframe.py
--rw-r--r--   0        0        0     2110 2023-08-07 21:21:40.558154 oplangchain-0.0.255/oplangchain/document_loaders/diffbot.py
--rw-r--r--   0        0        0     5094 2023-08-07 21:21:40.558154 oplangchain-0.0.255/oplangchain/document_loaders/directory.py
--rw-r--r--   0        0        0     1261 2023-08-07 21:21:40.558154 oplangchain-0.0.255/oplangchain/document_loaders/discord.py
--rw-r--r--   0        0        0    13216 2023-08-07 21:21:40.559154 oplangchain-0.0.255/oplangchain/document_loaders/docugami.py
--rw-r--r--   0        0        0     6089 2023-08-07 21:21:40.559154 oplangchain-0.0.255/oplangchain/document_loaders/dropbox.py
--rw-r--r--   0        0        0     3181 2023-08-07 21:21:40.560154 oplangchain-0.0.255/oplangchain/document_loaders/duckdb_loader.py
--rw-r--r--   0        0        0     3782 2023-08-07 21:21:40.560154 oplangchain-0.0.255/oplangchain/document_loaders/email.py
--rw-r--r--   0        0        0     8933 2023-08-07 21:21:40.561154 oplangchain-0.0.255/oplangchain/document_loaders/embaas.py
--rw-r--r--   0        0        0     1510 2023-08-07 21:21:40.561154 oplangchain-0.0.255/oplangchain/document_loaders/epub.py
--rw-r--r--   0        0        0     7808 2023-08-07 21:21:40.562154 oplangchain-0.0.255/oplangchain/document_loaders/etherscan.py
--rw-r--r--   0        0        0     5744 2023-08-07 21:21:40.562154 oplangchain-0.0.255/oplangchain/document_loaders/evernote.py
--rw-r--r--   0        0        0     1664 2023-08-07 21:21:40.562154 oplangchain-0.0.255/oplangchain/document_loaders/excel.py
--rw-r--r--   0        0        0     1298 2023-08-07 21:21:40.563154 oplangchain-0.0.255/oplangchain/document_loaders/facebook_chat.py
--rw-r--r--   0        0        0     2241 2023-08-07 21:21:40.563154 oplangchain-0.0.255/oplangchain/document_loaders/fauna.py
--rw-r--r--   0        0        0     1569 2023-08-07 21:21:40.564154 oplangchain-0.0.255/oplangchain/document_loaders/figma.py
--rw-r--r--   0        0        0     1573 2023-08-07 21:21:40.564154 oplangchain-0.0.255/oplangchain/document_loaders/gcs_directory.py
--rw-r--r--   0        0        0     1731 2023-08-07 21:21:40.565154 oplangchain-0.0.255/oplangchain/document_loaders/gcs_file.py
--rw-r--r--   0        0        0     4527 2023-08-07 21:21:40.565154 oplangchain-0.0.255/oplangchain/document_loaders/generic.py
--rw-r--r--   0        0        0     1682 2023-08-07 21:21:40.565154 oplangchain-0.0.255/oplangchain/document_loaders/geodataframe.py
--rw-r--r--   0        0        0     4138 2023-08-07 21:21:40.566154 oplangchain-0.0.255/oplangchain/document_loaders/git.py
--rw-r--r--   0        0        0     3106 2023-08-07 21:21:40.566154 oplangchain-0.0.255/oplangchain/document_loaders/gitbook.py
--rw-r--r--   0        0        0     6868 2023-08-07 21:21:40.567154 oplangchain-0.0.255/oplangchain/document_loaders/github.py
--rw-r--r--   0        0        0    13926 2023-08-07 21:21:40.567154 oplangchain-0.0.255/oplangchain/document_loaders/googledrive.py
--rw-r--r--   0        0        0      969 2023-08-07 21:21:40.568154 oplangchain-0.0.255/oplangchain/document_loaders/gutenberg.py
--rw-r--r--   0        0        0     1559 2023-08-07 21:21:40.568154 oplangchain-0.0.255/oplangchain/document_loaders/helpers.py
--rw-r--r--   0        0        0     2061 2023-08-07 21:21:40.569154 oplangchain-0.0.255/oplangchain/document_loaders/hn.py
--rw-r--r--   0        0        0     1204 2023-08-07 21:21:40.569154 oplangchain-0.0.255/oplangchain/document_loaders/html.py
--rw-r--r--   0        0        0     2118 2023-08-07 21:21:40.569154 oplangchain-0.0.255/oplangchain/document_loaders/html_bs.py
--rw-r--r--   0        0        0     3025 2023-08-07 21:21:40.570153 oplangchain-0.0.255/oplangchain/document_loaders/hugging_face_dataset.py
--rw-r--r--   0        0        0     7648 2023-08-07 21:21:40.570153 oplangchain-0.0.255/oplangchain/document_loaders/ifixit.py
--rw-r--r--   0        0        0     1186 2023-08-07 21:21:40.571153 oplangchain-0.0.255/oplangchain/document_loaders/image.py
--rw-r--r--   0        0        0     3099 2023-08-07 21:21:40.571153 oplangchain-0.0.255/oplangchain/document_loaders/image_captions.py
--rw-r--r--   0        0        0      487 2023-08-07 21:21:40.571153 oplangchain-0.0.255/oplangchain/document_loaders/imsdb.py
--rw-r--r--   0        0        0     1734 2023-08-07 21:21:40.572153 oplangchain-0.0.255/oplangchain/document_loaders/iugu.py
--rw-r--r--   0        0        0     3699 2023-08-07 21:21:40.572153 oplangchain-0.0.255/oplangchain/document_loaders/joplin.py
--rw-r--r--   0        0        0     5487 2023-08-07 21:21:40.573154 oplangchain-0.0.255/oplangchain/document_loaders/json_loader.py
--rw-r--r--   0        0        0     2052 2023-08-07 21:21:40.573154 oplangchain-0.0.255/oplangchain/document_loaders/larksuite.py
--rw-r--r--   0        0        0     1828 2023-08-07 21:21:40.574154 oplangchain-0.0.255/oplangchain/document_loaders/markdown.py
--rw-r--r--   0        0        0     3130 2023-08-07 21:21:40.574154 oplangchain-0.0.255/oplangchain/document_loaders/mastodon.py
--rw-r--r--   0        0        0     3293 2023-08-07 21:21:40.575154 oplangchain-0.0.255/oplangchain/document_loaders/max_compute.py
--rw-r--r--   0        0        0     3479 2023-08-07 21:21:40.575154 oplangchain-0.0.255/oplangchain/document_loaders/mediawikidump.py
--rw-r--r--   0        0        0      838 2023-08-07 21:21:40.575154 oplangchain-0.0.255/oplangchain/document_loaders/merge.py
--rw-r--r--   0        0        0     2600 2023-08-07 21:21:40.576154 oplangchain-0.0.255/oplangchain/document_loaders/mhtml.py
--rw-r--r--   0        0        0     3131 2023-08-07 21:21:40.576154 oplangchain-0.0.255/oplangchain/document_loaders/modern_treasury.py
--rw-r--r--   0        0        0     4287 2023-08-07 21:21:40.577155 oplangchain-0.0.255/oplangchain/document_loaders/news.py
--rw-r--r--   0        0        0     4281 2023-08-07 21:21:40.577155 oplangchain-0.0.255/oplangchain/document_loaders/notebook.py
--rw-r--r--   0        0        0      741 2023-08-07 21:21:40.578154 oplangchain-0.0.255/oplangchain/document_loaders/notion.py
--rw-r--r--   0        0        0     5892 2023-08-07 21:21:40.578154 oplangchain-0.0.255/oplangchain/document_loaders/notiondb.py
--rw-r--r--   0        0        0     1084 2023-08-07 21:21:40.578154 oplangchain-0.0.255/oplangchain/document_loaders/nuclia.py
--rw-r--r--   0        0        0     3594 2023-08-07 21:21:40.579154 oplangchain-0.0.255/oplangchain/document_loaders/obs_directory.py
--rw-r--r--   0        0        0     4745 2023-08-07 21:21:40.579154 oplangchain-0.0.255/oplangchain/document_loaders/obs_file.py
--rw-r--r--   0        0        0     2537 2023-08-07 21:21:40.580154 oplangchain-0.0.255/oplangchain/document_loaders/obsidian.py
--rw-r--r--   0        0        0     1793 2023-08-07 21:21:40.580154 oplangchain-0.0.255/oplangchain/document_loaders/odt.py
--rw-r--r--   0        0        0     8635 2023-08-07 21:21:40.581154 oplangchain-0.0.255/oplangchain/document_loaders/onedrive.py
--rw-r--r--   0        0        0     1108 2023-08-07 21:21:40.581154 oplangchain-0.0.255/oplangchain/document_loaders/onedrive_file.py
--rw-r--r--   0        0        0     1322 2023-08-07 21:21:40.582154 oplangchain-0.0.255/oplangchain/document_loaders/open_city_data.py
--rw-r--r--   0        0        0     1765 2023-08-07 21:21:40.582154 oplangchain-0.0.255/oplangchain/document_loaders/org_mode.py
--rw-r--r--   0        0        0      645 2023-08-07 21:21:40.583155 oplangchain-0.0.255/oplangchain/document_loaders/parsers/__init__.py
--rw-r--r--   0        0        0     6083 2023-08-07 21:21:40.583155 oplangchain-0.0.255/oplangchain/document_loaders/parsers/audio.py
--rw-r--r--   0        0        0     2466 2023-08-07 21:21:40.584154 oplangchain-0.0.255/oplangchain/document_loaders/parsers/generic.py
--rw-r--r--   0        0        0     5759 2023-08-07 21:21:40.584154 oplangchain-0.0.255/oplangchain/document_loaders/parsers/grobid.py
--rw-r--r--   0        0        0       99 2023-08-07 21:21:40.585154 oplangchain-0.0.255/oplangchain/document_loaders/parsers/html/__init__.py
--rw-r--r--   0        0        0     1602 2023-08-07 21:21:40.585154 oplangchain-0.0.255/oplangchain/document_loaders/parsers/html/bs4.py
--rw-r--r--   0        0        0      117 2023-08-07 21:21:40.586154 oplangchain-0.0.255/oplangchain/document_loaders/parsers/language/__init__.py
--rw-r--r--   0        0        0      499 2023-08-07 21:21:40.586154 oplangchain-0.0.255/oplangchain/document_loaders/parsers/language/code_segmenter.py
--rw-r--r--   0        0        0     2088 2023-08-07 21:21:40.587154 oplangchain-0.0.255/oplangchain/document_loaders/parsers/language/javascript.py
--rw-r--r--   0        0        0     4670 2023-08-07 21:21:40.587154 oplangchain-0.0.255/oplangchain/document_loaders/parsers/language/language_parser.py
--rw-r--r--   0        0        0     1662 2023-08-07 21:21:40.588154 oplangchain-0.0.255/oplangchain/document_loaders/parsers/language/python.py
--rw-r--r--   0        0        0     8801 2023-08-07 21:21:40.588154 oplangchain-0.0.255/oplangchain/document_loaders/parsers/pdf.py
--rw-r--r--   0        0        0      912 2023-08-07 21:21:40.589154 oplangchain-0.0.255/oplangchain/document_loaders/parsers/registry.py
--rw-r--r--   0        0        0      476 2023-08-07 21:21:40.589154 oplangchain-0.0.255/oplangchain/document_loaders/parsers/txt.py
--rw-r--r--   0        0        0    20543 2023-08-07 21:21:40.589154 oplangchain-0.0.255/oplangchain/document_loaders/pdf.py
--rw-r--r--   0        0        0     2517 2023-08-07 21:21:40.590154 oplangchain-0.0.255/oplangchain/document_loaders/powerpoint.py
--rw-r--r--   0        0        0     1412 2023-08-07 21:21:40.590154 oplangchain-0.0.255/oplangchain/document_loaders/psychic.py
--rw-r--r--   0        0        0     3418 2023-08-07 21:21:40.591154 oplangchain-0.0.255/oplangchain/document_loaders/pyspark_dataframe.py
--rw-r--r--   0        0        0      525 2023-08-07 21:21:40.591154 oplangchain-0.0.255/oplangchain/document_loaders/python.py
--rw-r--r--   0        0        0     3526 2023-08-07 21:21:40.592154 oplangchain-0.0.255/oplangchain/document_loaders/readthedocs.py
--rw-r--r--   0        0        0    12428 2023-08-07 21:21:40.592154 oplangchain-0.0.255/oplangchain/document_loaders/recursive_url_loader.py
--rw-r--r--   0        0        0     4605 2023-08-07 21:21:40.592154 oplangchain-0.0.255/oplangchain/document_loaders/reddit.py
--rw-r--r--   0        0        0      722 2023-08-07 21:21:40.593154 oplangchain-0.0.255/oplangchain/document_loaders/roam.py
--rw-r--r--   0        0        0     4433 2023-08-07 21:21:40.593154 oplangchain-0.0.255/oplangchain/document_loaders/rocksetdb.py
--rw-r--r--   0        0        0     4930 2023-08-07 21:21:40.594154 oplangchain-0.0.255/oplangchain/document_loaders/rss.py
--rw-r--r--   0        0        0     1821 2023-08-07 21:21:40.594154 oplangchain-0.0.255/oplangchain/document_loaders/rst.py
--rw-r--r--   0        0        0     2050 2023-08-07 21:21:40.595154 oplangchain-0.0.255/oplangchain/document_loaders/rtf.py
--rw-r--r--   0        0        0     1225 2023-08-07 21:21:40.595154 oplangchain-0.0.255/oplangchain/document_loaders/s3_directory.py
--rw-r--r--   0        0        0     1316 2023-08-07 21:21:40.595154 oplangchain-0.0.255/oplangchain/document_loaders/s3_file.py
--rw-r--r--   0        0        0     5008 2023-08-07 21:21:40.596154 oplangchain-0.0.255/oplangchain/document_loaders/sitemap.py
--rw-r--r--   0        0        0     4180 2023-08-07 21:21:40.596154 oplangchain-0.0.255/oplangchain/document_loaders/slack_directory.py
--rw-r--r--   0        0        0     4826 2023-08-07 21:21:40.597154 oplangchain-0.0.255/oplangchain/document_loaders/snowflake_loader.py
--rw-r--r--   0        0        0     2059 2023-08-07 21:21:40.597154 oplangchain-0.0.255/oplangchain/document_loaders/spreedly.py
--rw-r--r--   0        0        0      887 2023-08-07 21:21:40.598155 oplangchain-0.0.255/oplangchain/document_loaders/srt.py
--rw-r--r--   0        0        0     1855 2023-08-07 21:21:40.598155 oplangchain-0.0.255/oplangchain/document_loaders/stripe.py
--rw-r--r--   0        0        0     9041 2023-08-07 21:21:40.599154 oplangchain-0.0.255/oplangchain/document_loaders/telegram.py
--rw-r--r--   0        0        0     1840 2023-08-07 21:21:40.599154 oplangchain-0.0.255/oplangchain/document_loaders/tencent_cos_directory.py
--rw-r--r--   0        0        0     1752 2023-08-07 21:21:40.600154 oplangchain-0.0.255/oplangchain/document_loaders/tencent_cos_file.py
--rw-r--r--   0        0        0     1993 2023-08-07 21:21:40.600154 oplangchain-0.0.255/oplangchain/document_loaders/text.py
--rw-r--r--   0        0        0      994 2023-08-07 21:21:40.600154 oplangchain-0.0.255/oplangchain/document_loaders/tomarkdown.py
--rw-r--r--   0        0        0     1649 2023-08-07 21:21:40.601154 oplangchain-0.0.255/oplangchain/document_loaders/toml.py
--rw-r--r--   0        0        0     6596 2023-08-07 21:21:40.601154 oplangchain-0.0.255/oplangchain/document_loaders/trello.py
--rw-r--r--   0        0        0     1278 2023-08-07 21:21:40.602154 oplangchain-0.0.255/oplangchain/document_loaders/tsv.py
--rw-r--r--   0        0        0     3454 2023-08-07 21:21:40.602154 oplangchain-0.0.255/oplangchain/document_loaders/twitter.py
--rw-r--r--   0        0        0    13877 2023-08-07 21:21:40.603154 oplangchain-0.0.255/oplangchain/document_loaders/unstructured.py
--rw-r--r--   0        0        0     6011 2023-08-07 21:21:40.603154 oplangchain-0.0.255/oplangchain/document_loaders/url.py
--rw-r--r--   0        0        0     4947 2023-08-07 21:21:40.603154 oplangchain-0.0.255/oplangchain/document_loaders/url_playwright.py
--rw-r--r--   0        0        0     5221 2023-08-07 21:21:40.604153 oplangchain-0.0.255/oplangchain/document_loaders/url_selenium.py
--rw-r--r--   0        0        0     1633 2023-08-07 21:21:40.604153 oplangchain-0.0.255/oplangchain/document_loaders/weather.py
--rw-r--r--   0        0        0     8011 2023-08-07 21:21:40.605154 oplangchain-0.0.255/oplangchain/document_loaders/web_base.py
--rw-r--r--   0        0        0     1761 2023-08-07 21:21:40.605154 oplangchain-0.0.255/oplangchain/document_loaders/whatsapp_chat.py
--rw-r--r--   0        0        0     2182 2023-08-07 21:21:40.606153 oplangchain-0.0.255/oplangchain/document_loaders/wikipedia.py
--rw-r--r--   0        0        0     4553 2023-08-07 21:21:40.606153 oplangchain-0.0.255/oplangchain/document_loaders/word_document.py
--rw-r--r--   0        0        0     1479 2023-08-07 21:21:40.607154 oplangchain-0.0.255/oplangchain/document_loaders/xml.py
--rw-r--r--   0        0        0     1623 2023-08-07 21:21:40.607154 oplangchain-0.0.255/oplangchain/document_loaders/xorbits.py
--rw-r--r--   0        0        0    14670 2023-08-07 21:21:40.608153 oplangchain-0.0.255/oplangchain/document_loaders/youtube.py
--rw-r--r--   0        0        0     1436 2023-08-07 21:21:40.609153 oplangchain-0.0.255/oplangchain/document_transformers/__init__.py
--rw-r--r--   0        0        0     3446 2023-08-07 21:21:40.609153 oplangchain-0.0.255/oplangchain/document_transformers/doctran_text_extract.py
--rw-r--r--   0        0        0     2170 2023-08-07 21:21:40.610154 oplangchain-0.0.255/oplangchain/document_transformers/doctran_text_qa.py
--rw-r--r--   0        0        0     2314 2023-08-07 21:21:40.610154 oplangchain-0.0.255/oplangchain/document_transformers/doctran_text_translate.py
--rw-r--r--   0        0        0     8078 2023-08-07 21:21:40.611154 oplangchain-0.0.255/oplangchain/document_transformers/embeddings_redundant_filter.py
--rw-r--r--   0        0        0     1293 2023-08-07 21:21:40.611154 oplangchain-0.0.255/oplangchain/document_transformers/html2text.py
--rw-r--r--   0        0        0     1374 2023-08-07 21:21:40.611154 oplangchain-0.0.255/oplangchain/document_transformers/long_context_reorder.py
--rw-r--r--   0        0        0     1469 2023-08-07 21:21:40.612154 oplangchain-0.0.255/oplangchain/document_transformers/nuclia_text_transform.py
--rw-r--r--   0        0        0     6198 2023-08-07 21:21:40.612154 oplangchain-0.0.255/oplangchain/document_transformers/openai_functions.py
--rw-r--r--   0        0        0     4604 2023-08-07 21:21:40.613153 oplangchain-0.0.255/oplangchain/embeddings/__init__.py
--rw-r--r--   0        0        0     9592 2023-08-07 21:21:40.614153 oplangchain-0.0.255/oplangchain/embeddings/aleph_alpha.py
--rw-r--r--   0        0        0     1631 2023-08-07 21:21:40.614153 oplangchain-0.0.255/oplangchain/embeddings/awa.py
--rw-r--r--   0        0        0      655 2023-08-07 21:21:40.614153 oplangchain-0.0.255/oplangchain/embeddings/base.py
--rw-r--r--   0        0        0     5480 2023-08-07 21:21:40.615154 oplangchain-0.0.255/oplangchain/embeddings/bedrock.py
--rw-r--r--   0        0        0     6547 2023-08-07 21:21:40.615154 oplangchain-0.0.255/oplangchain/embeddings/clarifai.py
--rw-r--r--   0        0        0     3377 2023-08-07 21:21:40.616154 oplangchain-0.0.255/oplangchain/embeddings/cohere.py
--rw-r--r--   0        0        0     4882 2023-08-07 21:21:40.616154 oplangchain-0.0.255/oplangchain/embeddings/dashscope.py
--rw-r--r--   0        0        0     4394 2023-08-07 21:21:40.617154 oplangchain-0.0.255/oplangchain/embeddings/deepinfra.py
--rw-r--r--   0        0        0     2792 2023-08-07 21:21:40.617154 oplangchain-0.0.255/oplangchain/embeddings/edenai.py
--rw-r--r--   0        0        0     8376 2023-08-07 21:21:40.618155 oplangchain-0.0.255/oplangchain/embeddings/elasticsearch.py
--rw-r--r--   0        0        0     4786 2023-08-07 21:21:40.618155 oplangchain-0.0.255/oplangchain/embeddings/embaas.py
--rw-r--r--   0        0        0     1495 2023-08-07 21:21:40.619154 oplangchain-0.0.255/oplangchain/embeddings/fake.py
--rw-r--r--   0        0        0     2682 2023-08-07 21:21:40.619154 oplangchain-0.0.255/oplangchain/embeddings/google_palm.py
--rw-r--r--   0        0        0     1637 2023-08-07 21:21:40.619154 oplangchain-0.0.255/oplangchain/embeddings/gpt4all.py
--rw-r--r--   0        0        0     6034 2023-08-07 21:21:40.620154 oplangchain-0.0.255/oplangchain/embeddings/huggingface.py
--rw-r--r--   0        0        0     3680 2023-08-07 21:21:40.620154 oplangchain-0.0.255/oplangchain/embeddings/huggingface_hub.py
--rw-r--r--   0        0        0     3445 2023-08-07 21:21:40.621154 oplangchain-0.0.255/oplangchain/embeddings/jina.py
--rw-r--r--   0        0        0     4021 2023-08-07 21:21:40.621154 oplangchain-0.0.255/oplangchain/embeddings/llamacpp.py
--rw-r--r--   0        0        0    12073 2023-08-07 21:21:40.622154 oplangchain-0.0.255/oplangchain/embeddings/localai.py
--rw-r--r--   0        0        0     4684 2023-08-07 21:21:40.622154 oplangchain-0.0.255/oplangchain/embeddings/minimax.py
--rw-r--r--   0        0        0     2240 2023-08-07 21:21:40.623153 oplangchain-0.0.255/oplangchain/embeddings/mlflow_gateway.py
--rw-r--r--   0        0        0     2357 2023-08-07 21:21:40.623153 oplangchain-0.0.255/oplangchain/embeddings/modelscope_hub.py
--rw-r--r--   0        0        0     5877 2023-08-07 21:21:40.624154 oplangchain-0.0.255/oplangchain/embeddings/mosaicml.py
--rw-r--r--   0        0        0     2170 2023-08-07 21:21:40.624154 oplangchain-0.0.255/oplangchain/embeddings/nlpcloud.py
--rw-r--r--   0        0        0     3398 2023-08-07 21:21:40.624154 oplangchain-0.0.255/oplangchain/embeddings/octoai_embeddings.py
--rw-r--r--   0        0        0    19937 2023-08-07 21:21:40.625156 oplangchain-0.0.255/oplangchain/embeddings/openai.py
--rw-r--r--   0        0        0     7102 2023-08-07 21:21:40.626153 oplangchain-0.0.255/oplangchain/embeddings/sagemaker_endpoint.py
--rw-r--r--   0        0        0     3747 2023-08-07 21:21:40.626153 oplangchain-0.0.255/oplangchain/embeddings/self_hosted.py
--rw-r--r--   0        0        0     6546 2023-08-07 21:21:40.626153 oplangchain-0.0.255/oplangchain/embeddings/self_hosted_hugging_face.py
--rw-r--r--   0        0        0      179 2023-08-07 21:21:40.627153 oplangchain-0.0.255/oplangchain/embeddings/sentence_transformer.py
--rw-r--r--   0        0        0     3726 2023-08-07 21:21:40.627153 oplangchain-0.0.255/oplangchain/embeddings/spacy_embeddings.py
--rw-r--r--   0        0        0     2386 2023-08-07 21:21:40.628153 oplangchain-0.0.255/oplangchain/embeddings/tensorflow_hub.py
--rw-r--r--   0        0        0     1875 2023-08-07 21:21:40.628153 oplangchain-0.0.255/oplangchain/embeddings/vertexai.py
--rw-r--r--   0        0        0     3305 2023-08-07 21:21:40.629153 oplangchain-0.0.255/oplangchain/embeddings/xinference.py
--rw-r--r--   0        0        0      476 2023-08-07 21:21:40.629153 oplangchain-0.0.255/oplangchain/env.py
--rw-r--r--   0        0        0     5042 2023-08-07 21:21:40.630153 oplangchain-0.0.255/oplangchain/evaluation/__init__.py
--rw-r--r--   0        0        0      165 2023-08-07 21:21:40.630153 oplangchain-0.0.255/oplangchain/evaluation/agents/__init__.py
--rw-r--r--   0        0        0    13153 2023-08-07 21:21:40.631153 oplangchain-0.0.255/oplangchain/evaluation/agents/trajectory_eval_chain.py
--rw-r--r--   0        0        0     5935 2023-08-07 21:21:40.631153 oplangchain-0.0.255/oplangchain/evaluation/agents/trajectory_eval_prompt.py
--rw-r--r--   0        0        0     1398 2023-08-07 21:21:40.632153 oplangchain-0.0.255/oplangchain/evaluation/comparison/__init__.py
--rw-r--r--   0        0        0    15043 2023-08-07 21:21:40.633154 oplangchain-0.0.255/oplangchain/evaluation/comparison/eval_chain.py
--rw-r--r--   0        0        0     2175 2023-08-07 21:21:40.633154 oplangchain-0.0.255/oplangchain/evaluation/comparison/prompt.py
--rw-r--r--   0        0        0     1628 2023-08-07 21:21:40.634153 oplangchain-0.0.255/oplangchain/evaluation/criteria/__init__.py
--rw-r--r--   0        0        0    20294 2023-08-07 21:21:40.634153 oplangchain-0.0.255/oplangchain/evaluation/criteria/eval_chain.py
--rw-r--r--   0        0        0     1751 2023-08-07 21:21:40.635153 oplangchain-0.0.255/oplangchain/evaluation/criteria/prompt.py
--rw-r--r--   0        0        0      323 2023-08-07 21:21:40.635153 oplangchain-0.0.255/oplangchain/evaluation/embedding_distance/__init__.py
--rw-r--r--   0        0        0    15475 2023-08-07 21:21:40.636153 oplangchain-0.0.255/oplangchain/evaluation/embedding_distance/base.py
--rw-r--r--   0        0        0     5192 2023-08-07 21:21:40.636153 oplangchain-0.0.255/oplangchain/evaluation/loading.py
--rw-r--r--   0        0        0      344 2023-08-07 21:21:40.637153 oplangchain-0.0.255/oplangchain/evaluation/qa/__init__.py
--rw-r--r--   0        0        0     9987 2023-08-07 21:21:40.637153 oplangchain-0.0.255/oplangchain/evaluation/qa/eval_chain.py
--rw-r--r--   0        0        0     3906 2023-08-07 21:21:40.638154 oplangchain-0.0.255/oplangchain/evaluation/qa/eval_prompt.py
--rw-r--r--   0        0        0      956 2023-08-07 21:21:40.638154 oplangchain-0.0.255/oplangchain/evaluation/qa/generate_chain.py
--rw-r--r--   0        0        0      601 2023-08-07 21:21:40.639153 oplangchain-0.0.255/oplangchain/evaluation/qa/generate_prompt.py
--rw-r--r--   0        0        0    16800 2023-08-07 21:21:40.639153 oplangchain-0.0.255/oplangchain/evaluation/schema.py
--rw-r--r--   0        0        0      285 2023-08-07 21:21:40.640154 oplangchain-0.0.255/oplangchain/evaluation/string_distance/__init__.py
--rw-r--r--   0        0        0    13996 2023-08-07 21:21:40.640154 oplangchain-0.0.255/oplangchain/evaluation/string_distance/base.py
--rw-r--r--   0        0        0      141 2023-08-07 21:21:40.641153 oplangchain-0.0.255/oplangchain/example_generator.py
--rw-r--r--   0        0        0      162 2023-08-07 21:21:40.641153 oplangchain-0.0.255/oplangchain/formatting.py
--rw-r--r--   0        0        0      751 2023-08-07 21:21:40.642153 oplangchain-0.0.255/oplangchain/graphs/__init__.py
--rw-r--r--   0        0        0     6198 2023-08-07 21:21:40.642153 oplangchain-0.0.255/oplangchain/graphs/arangodb_graph.py
--rw-r--r--   0        0        0     1841 2023-08-07 21:21:40.643153 oplangchain-0.0.255/oplangchain/graphs/hugegraph.py
--rw-r--r--   0        0        0     3559 2023-08-07 21:21:40.643153 oplangchain-0.0.255/oplangchain/graphs/kuzu_graph.py
--rw-r--r--   0        0        0      713 2023-08-07 21:21:40.644153 oplangchain-0.0.255/oplangchain/graphs/memgraph_graph.py
--rw-r--r--   0        0        0     7362 2023-08-07 21:21:40.644153 oplangchain-0.0.255/oplangchain/graphs/nebula_graph.py
--rw-r--r--   0        0        0     3625 2023-08-07 21:21:40.645154 oplangchain-0.0.255/oplangchain/graphs/neo4j_graph.py
--rw-r--r--   0        0        0     6553 2023-08-07 21:21:40.645154 oplangchain-0.0.255/oplangchain/graphs/neptune_graph.py
--rw-r--r--   0        0        0     5877 2023-08-07 21:21:40.646154 oplangchain-0.0.255/oplangchain/graphs/networkx_graph.py
--rw-r--r--   0        0        0     9461 2023-08-07 21:21:40.646154 oplangchain-0.0.255/oplangchain/graphs/rdf_graph.py
--rw-r--r--   0        0        0      207 2023-08-07 21:21:40.647153 oplangchain-0.0.255/oplangchain/indexes/__init__.py
--rw-r--r--   0        0        0     1712 2023-08-07 21:21:40.647153 oplangchain-0.0.255/oplangchain/indexes/graph.py
--rw-r--r--   0        0        0       49 2023-08-07 21:21:40.648155 oplangchain-0.0.255/oplangchain/indexes/prompts/__init__.py
--rw-r--r--   0        0        0     1947 2023-08-07 21:21:40.648155 oplangchain-0.0.255/oplangchain/indexes/prompts/entity_extraction.py
--rw-r--r--   0        0        0     1152 2023-08-07 21:21:40.649155 oplangchain-0.0.255/oplangchain/indexes/prompts/entity_summarization.py
--rw-r--r--   0        0        0     1584 2023-08-07 21:21:40.649155 oplangchain-0.0.255/oplangchain/indexes/prompts/knowledge_triplet_extraction.py
--rw-r--r--   0        0        0     3048 2023-08-07 21:21:40.650154 oplangchain-0.0.255/oplangchain/indexes/vectorstore.py
--rw-r--r--   0        0        0      277 2023-08-07 21:21:40.650154 oplangchain-0.0.255/oplangchain/input.py
--rw-r--r--   0        0        0     6388 2023-08-07 21:21:40.651155 oplangchain-0.0.255/oplangchain/llms/__init__.py
--rw-r--r--   0        0        0     4996 2023-08-07 21:21:40.651155 oplangchain-0.0.255/oplangchain/llms/ai21.py
--rw-r--r--   0        0        0    11352 2023-08-07 21:21:40.652154 oplangchain-0.0.255/oplangchain/llms/aleph_alpha.py
--rw-r--r--   0        0        0     3021 2023-08-07 21:21:40.652154 oplangchain-0.0.255/oplangchain/llms/amazon_api_gateway.py
--rw-r--r--   0        0        0    11164 2023-08-07 21:21:40.653154 oplangchain-0.0.255/oplangchain/llms/anthropic.py
--rw-r--r--   0        0        0     4657 2023-08-07 21:21:40.653154 oplangchain-0.0.255/oplangchain/llms/anyscale.py
--rw-r--r--   0        0        0     5365 2023-08-07 21:21:40.654154 oplangchain-0.0.255/oplangchain/llms/aviary.py
--rw-r--r--   0        0        0    10218 2023-08-07 21:21:40.654154 oplangchain-0.0.255/oplangchain/llms/azureml_endpoint.py
--rw-r--r--   0        0        0     4309 2023-08-07 21:21:40.655155 oplangchain-0.0.255/oplangchain/llms/bananadev.py
--rw-r--r--   0        0        0    34723 2023-08-07 21:21:40.655155 oplangchain-0.0.255/oplangchain/llms/base.py
--rw-r--r--   0        0        0     2359 2023-08-07 21:21:40.656154 oplangchain-0.0.255/oplangchain/llms/baseten.py
--rw-r--r--   0        0        0     9064 2023-08-07 21:21:40.656154 oplangchain-0.0.255/oplangchain/llms/beam.py
--rw-r--r--   0        0        0     6690 2023-08-07 21:21:40.657155 oplangchain-0.0.255/oplangchain/llms/bedrock.py
--rw-r--r--   0        0        0     3773 2023-08-07 21:21:40.657155 oplangchain-0.0.255/oplangchain/llms/cerebriumai.py
--rw-r--r--   0        0        0     3937 2023-08-07 21:21:40.658154 oplangchain-0.0.255/oplangchain/llms/chatglm.py
--rw-r--r--   0        0        0     5802 2023-08-07 21:21:40.658154 oplangchain-0.0.255/oplangchain/llms/clarifai.py
--rw-r--r--   0        0        0     7303 2023-08-07 21:21:40.659154 oplangchain-0.0.255/oplangchain/llms/cohere.py
--rw-r--r--   0        0        0     4187 2023-08-07 21:21:40.659154 oplangchain-0.0.255/oplangchain/llms/ctransformers.py
--rw-r--r--   0        0        0    12068 2023-08-07 21:21:40.660154 oplangchain-0.0.255/oplangchain/llms/databricks.py
--rw-r--r--   0        0        0     3755 2023-08-07 21:21:40.660154 oplangchain-0.0.255/oplangchain/llms/deepinfra.py
--rw-r--r--   0        0        0     7445 2023-08-07 21:21:40.661153 oplangchain-0.0.255/oplangchain/llms/edenai.py
--rw-r--r--   0        0        0     1335 2023-08-07 21:21:40.661153 oplangchain-0.0.255/oplangchain/llms/fake.py
--rw-r--r--   0        0        0    13035 2023-08-07 21:21:40.661153 oplangchain-0.0.255/oplangchain/llms/fireworks.py
--rw-r--r--   0        0        0     3651 2023-08-07 21:21:40.662153 oplangchain-0.0.255/oplangchain/llms/forefrontai.py
--rw-r--r--   0        0        0     5733 2023-08-07 21:21:40.662153 oplangchain-0.0.255/oplangchain/llms/google_palm.py
--rw-r--r--   0        0        0     5122 2023-08-07 21:21:40.663154 oplangchain-0.0.255/oplangchain/llms/gooseai.py
--rw-r--r--   0        0        0     6312 2023-08-07 21:21:40.663154 oplangchain-0.0.255/oplangchain/llms/gpt4all.py
--rw-r--r--   0        0        0     5452 2023-08-07 21:21:40.664153 oplangchain-0.0.255/oplangchain/llms/huggingface_endpoint.py
--rw-r--r--   0        0        0     4603 2023-08-07 21:21:40.664153 oplangchain-0.0.255/oplangchain/llms/huggingface_hub.py
--rw-r--r--   0        0        0     6566 2023-08-07 21:21:40.665154 oplangchain-0.0.255/oplangchain/llms/huggingface_pipeline.py
--rw-r--r--   0        0        0     9715 2023-08-07 21:21:40.665154 oplangchain-0.0.255/oplangchain/llms/huggingface_text_gen_inference.py
--rw-r--r--   0        0        0     2541 2023-08-07 21:21:40.665154 oplangchain-0.0.255/oplangchain/llms/human.py
--rw-r--r--   0        0        0     5065 2023-08-07 21:21:40.666154 oplangchain-0.0.255/oplangchain/llms/koboldai.py
--rw-r--r--   0        0        0    10889 2023-08-07 21:21:40.666154 oplangchain-0.0.255/oplangchain/llms/llamacpp.py
--rw-r--r--   0        0        0     1249 2023-08-07 21:21:40.667154 oplangchain-0.0.255/oplangchain/llms/loading.py
--rw-r--r--   0        0        0     1874 2023-08-07 21:21:40.667154 oplangchain-0.0.255/oplangchain/llms/manifest.py
--rw-r--r--   0        0        0     5154 2023-08-07 21:21:40.668154 oplangchain-0.0.255/oplangchain/llms/minimax.py
--rw-r--r--   0        0        0     2919 2023-08-07 21:21:40.668154 oplangchain-0.0.255/oplangchain/llms/mlflow_ai_gateway.py
--rw-r--r--   0        0        0     3239 2023-08-07 21:21:40.669154 oplangchain-0.0.255/oplangchain/llms/modal.py
--rw-r--r--   0        0        0     6742 2023-08-07 21:21:40.669154 oplangchain-0.0.255/oplangchain/llms/mosaicml.py
--rw-r--r--   0        0        0     5442 2023-08-07 21:21:40.669154 oplangchain-0.0.255/oplangchain/llms/nlpcloud.py
--rw-r--r--   0        0        0     3804 2023-08-07 21:21:40.670154 oplangchain-0.0.255/oplangchain/llms/octoai_endpoint.py
--rw-r--r--   0        0        0    34722 2023-08-07 21:21:40.670154 oplangchain-0.0.255/oplangchain/llms/openai.py
--rw-r--r--   0        0        0     9922 2023-08-07 21:21:40.671153 oplangchain-0.0.255/oplangchain/llms/openllm.py
--rw-r--r--   0        0        0      794 2023-08-07 21:21:40.671153 oplangchain-0.0.255/oplangchain/llms/openlm.py
--rw-r--r--   0        0        0     5263 2023-08-07 21:21:40.672153 oplangchain-0.0.255/oplangchain/llms/petals.py
--rw-r--r--   0        0        0     4013 2023-08-07 21:21:40.672153 oplangchain-0.0.255/oplangchain/llms/pipelineai.py
--rw-r--r--   0        0        0     1527 2023-08-07 21:21:40.673154 oplangchain-0.0.255/oplangchain/llms/predibase.py
--rw-r--r--   0        0        0     4364 2023-08-07 21:21:40.673154 oplangchain-0.0.255/oplangchain/llms/predictionguard.py
--rw-r--r--   0        0        0     8682 2023-08-07 21:21:40.674155 oplangchain-0.0.255/oplangchain/llms/promptlayer_openai.py
--rw-r--r--   0        0        0     5160 2023-08-07 21:21:40.674299 oplangchain-0.0.255/oplangchain/llms/replicate.py
--rw-r--r--   0        0        0     7335 2023-08-07 21:21:40.675155 oplangchain-0.0.255/oplangchain/llms/rwkv.py
--rw-r--r--   0        0        0     8811 2023-08-07 21:21:40.675155 oplangchain-0.0.255/oplangchain/llms/sagemaker_endpoint.py
--rw-r--r--   0        0        0     7673 2023-08-07 21:21:40.675155 oplangchain-0.0.255/oplangchain/llms/self_hosted.py
--rw-r--r--   0        0        0     7689 2023-08-07 21:21:40.676153 oplangchain-0.0.255/oplangchain/llms/self_hosted_hugging_face.py
--rw-r--r--   0        0        0     4563 2023-08-07 21:21:40.676153 oplangchain-0.0.255/oplangchain/llms/stochasticai.py
--rw-r--r--   0        0        0     7579 2023-08-07 21:21:40.677154 oplangchain-0.0.255/oplangchain/llms/textgen.py
--rw-r--r--   0        0        0     7872 2023-08-07 21:21:40.677154 oplangchain-0.0.255/oplangchain/llms/tongyi.py
--rw-r--r--   0        0        0      246 2023-08-07 21:21:40.678154 oplangchain-0.0.255/oplangchain/llms/utils.py
--rw-r--r--   0        0        0     7709 2023-08-07 21:21:40.678154 oplangchain-0.0.255/oplangchain/llms/vertexai.py
--rw-r--r--   0        0        0     3978 2023-08-07 21:21:40.678154 oplangchain-0.0.255/oplangchain/llms/vllm.py
--rw-r--r--   0        0        0     4909 2023-08-07 21:21:40.679154 oplangchain-0.0.255/oplangchain/llms/writer.py
--rw-r--r--   0        0        0     6011 2023-08-07 21:21:40.679154 oplangchain-0.0.255/oplangchain/llms/xinference.py
--rw-r--r--   0        0        0       41 2023-08-07 21:21:40.680153 oplangchain-0.0.255/oplangchain/load/__init__.py
--rw-r--r--   0        0        0      753 2023-08-07 21:21:40.680153 oplangchain-0.0.255/oplangchain/load/dump.py
--rw-r--r--   0        0        0     4037 2023-08-07 21:21:40.681154 oplangchain-0.0.255/oplangchain/load/load.py
--rw-r--r--   0        0        0     4618 2023-08-07 21:21:40.681154 oplangchain-0.0.255/oplangchain/load/serializable.py
--rw-r--r--   0        0        0     2844 2023-08-07 21:21:40.682154 oplangchain-0.0.255/oplangchain/memory/__init__.py
--rw-r--r--   0        0        0     3068 2023-08-07 21:21:40.683153 oplangchain-0.0.255/oplangchain/memory/buffer.py
--rw-r--r--   0        0        0     1228 2023-08-07 21:21:40.683153 oplangchain-0.0.255/oplangchain/memory/buffer_window.py
--rw-r--r--   0        0        0     1612 2023-08-07 21:21:40.683153 oplangchain-0.0.255/oplangchain/memory/chat_memory.py
--rw-r--r--   0        0        0     1566 2023-08-07 21:21:40.684153 oplangchain-0.0.255/oplangchain/memory/chat_message_histories/__init__.py
--rw-r--r--   0        0        0     2367 2023-08-07 21:21:40.685154 oplangchain-0.0.255/oplangchain/memory/chat_message_histories/cassandra.py
--rw-r--r--   0        0        0     6493 2023-08-07 21:21:40.685154 oplangchain-0.0.255/oplangchain/memory/chat_message_histories/cosmos_db.py
--rw-r--r--   0        0        0     2881 2023-08-07 21:21:40.686153 oplangchain-0.0.255/oplangchain/memory/chat_message_histories/dynamodb.py
--rw-r--r--   0        0        0     1362 2023-08-07 21:21:40.686153 oplangchain-0.0.255/oplangchain/memory/chat_message_histories/file.py
--rw-r--r--   0        0        0     3332 2023-08-07 21:21:40.687154 oplangchain-0.0.255/oplangchain/memory/chat_message_histories/firestore.py
--rw-r--r--   0        0        0      584 2023-08-07 21:21:40.687154 oplangchain-0.0.255/oplangchain/memory/chat_message_histories/in_memory.py
--rw-r--r--   0        0        0     6829 2023-08-07 21:21:40.687154 oplangchain-0.0.255/oplangchain/memory/chat_message_histories/momento.py
--rw-r--r--   0        0        0     2719 2023-08-07 21:21:40.688154 oplangchain-0.0.255/oplangchain/memory/chat_message_histories/mongodb.py
--rw-r--r--   0        0        0     2644 2023-08-07 21:21:40.688154 oplangchain-0.0.255/oplangchain/memory/chat_message_histories/postgres.py
--rw-r--r--   0        0        0     1945 2023-08-07 21:21:40.689154 oplangchain-0.0.255/oplangchain/memory/chat_message_histories/redis.py
--rw-r--r--   0        0        0     2897 2023-08-07 21:21:40.690157 oplangchain-0.0.255/oplangchain/memory/chat_message_histories/sql.py
--rw-r--r--   0        0        0     1176 2023-08-07 21:21:40.690617 oplangchain-0.0.255/oplangchain/memory/chat_message_histories/streamlit.py
--rw-r--r--   0        0        0     6402 2023-08-07 21:21:40.691155 oplangchain-0.0.255/oplangchain/memory/chat_message_histories/zep.py
--rw-r--r--   0        0        0     2889 2023-08-07 21:21:40.691155 oplangchain-0.0.255/oplangchain/memory/combined.py
--rw-r--r--   0        0        0    12982 2023-08-07 21:21:40.692156 oplangchain-0.0.255/oplangchain/memory/entity.py
--rw-r--r--   0        0        0     5017 2023-08-07 21:21:40.692156 oplangchain-0.0.255/oplangchain/memory/kg.py
--rw-r--r--   0        0        0     3098 2023-08-07 21:21:40.693154 oplangchain-0.0.255/oplangchain/memory/motorhead_memory.py
--rw-r--r--   0        0        0     8176 2023-08-07 21:21:40.694155 oplangchain-0.0.255/oplangchain/memory/prompt.py
--rw-r--r--   0        0        0      789 2023-08-07 21:21:40.694155 oplangchain-0.0.255/oplangchain/memory/readonly.py
--rw-r--r--   0        0        0      756 2023-08-07 21:21:40.695154 oplangchain-0.0.255/oplangchain/memory/simple.py
--rw-r--r--   0        0        0     3342 2023-08-07 21:21:40.695154 oplangchain-0.0.255/oplangchain/memory/summary.py
--rw-r--r--   0        0        0     2933 2023-08-07 21:21:40.695154 oplangchain-0.0.255/oplangchain/memory/summary_buffer.py
--rw-r--r--   0        0        0     1915 2023-08-07 21:21:40.696155 oplangchain-0.0.255/oplangchain/memory/token_buffer.py
--rw-r--r--   0        0        0      687 2023-08-07 21:21:40.696155 oplangchain-0.0.255/oplangchain/memory/utils.py
--rw-r--r--   0        0        0     2976 2023-08-07 21:21:40.697154 oplangchain-0.0.255/oplangchain/memory/vectorstore.py
--rw-r--r--   0        0        0     5067 2023-08-07 21:21:40.697154 oplangchain-0.0.255/oplangchain/memory/zep_memory.py
--rw-r--r--   0        0        0     3236 2023-08-07 21:21:40.698155 oplangchain-0.0.255/oplangchain/model_laboratory.py
--rw-r--r--   0        0        0     1588 2023-08-07 21:21:40.699156 oplangchain-0.0.255/oplangchain/output_parsers/__init__.py
--rw-r--r--   0        0        0     1071 2023-08-07 21:21:40.699156 oplangchain-0.0.255/oplangchain/output_parsers/boolean.py
--rw-r--r--   0        0        0     1763 2023-08-07 21:21:40.700155 oplangchain-0.0.255/oplangchain/output_parsers/combining.py
--rw-r--r--   0        0        0     1817 2023-08-07 21:21:40.700155 oplangchain-0.0.255/oplangchain/output_parsers/datetime.py
--rw-r--r--   0        0        0     1138 2023-08-07 21:21:40.701154 oplangchain-0.0.255/oplangchain/output_parsers/enum.py
--rw-r--r--   0        0        0     1805 2023-08-07 21:21:40.701154 oplangchain-0.0.255/oplangchain/output_parsers/fix.py
--rw-r--r--   0        0        0      810 2023-08-07 21:21:40.702154 oplangchain-0.0.255/oplangchain/output_parsers/format_instructions.py
--rw-r--r--   0        0        0     2209 2023-08-07 21:21:40.702154 oplangchain-0.0.255/oplangchain/output_parsers/json.py
--rw-r--r--   0        0        0      939 2023-08-07 21:21:40.702154 oplangchain-0.0.255/oplangchain/output_parsers/list.py
--rw-r--r--   0        0        0      702 2023-08-07 21:21:40.703154 oplangchain-0.0.255/oplangchain/output_parsers/loading.py
--rw-r--r--   0        0        0     3350 2023-08-07 21:21:40.703154 oplangchain-0.0.255/oplangchain/output_parsers/openai_functions.py
--rw-r--r--   0        0        0      503 2023-08-07 21:21:40.704153 oplangchain-0.0.255/oplangchain/output_parsers/prompts.py
--rw-r--r--   0        0        0     1731 2023-08-07 21:21:40.704153 oplangchain-0.0.255/oplangchain/output_parsers/pydantic.py
--rw-r--r--   0        0        0     3165 2023-08-07 21:21:40.705154 oplangchain-0.0.255/oplangchain/output_parsers/rail_parser.py
--rw-r--r--   0        0        0     1196 2023-08-07 21:21:40.705154 oplangchain-0.0.255/oplangchain/output_parsers/regex.py
--rw-r--r--   0        0        0     1696 2023-08-07 21:21:40.705154 oplangchain-0.0.255/oplangchain/output_parsers/regex_dict.py
--rw-r--r--   0        0        0     4709 2023-08-07 21:21:40.706153 oplangchain-0.0.255/oplangchain/output_parsers/retry.py
--rw-r--r--   0        0        0     3070 2023-08-07 21:21:40.706153 oplangchain-0.0.255/oplangchain/output_parsers/structured.py
--rw-r--r--   0        0        0     2744 2023-08-07 21:21:40.707597 oplangchain-0.0.255/oplangchain/prompts/__init__.py
--rw-r--r--   0        0        0     3671 2023-08-07 21:21:40.708154 oplangchain-0.0.255/oplangchain/prompts/base.py
--rw-r--r--   0        0        0    21563 2023-08-07 21:21:40.708154 oplangchain-0.0.255/oplangchain/prompts/chat.py
--rw-r--r--   0        0        0      553 2023-08-07 21:21:40.709154 oplangchain-0.0.255/oplangchain/prompts/example_selector/__init__.py
--rw-r--r--   0        0        0      526 2023-08-07 21:21:40.709154 oplangchain-0.0.255/oplangchain/prompts/example_selector/base.py
--rw-r--r--   0        0        0     2433 2023-08-07 21:21:40.710153 oplangchain-0.0.255/oplangchain/prompts/example_selector/length_based.py
--rw-r--r--   0        0        0     3798 2023-08-07 21:21:40.710153 oplangchain-0.0.255/oplangchain/prompts/example_selector/ngram_overlap.py
--rw-r--r--   0        0        0     6848 2023-08-07 21:21:40.711153 oplangchain-0.0.255/oplangchain/prompts/example_selector/semantic_similarity.py
--rw-r--r--   0        0        0    11737 2023-08-07 21:21:40.711153 oplangchain-0.0.255/oplangchain/prompts/few_shot.py
--rw-r--r--   0        0        0     5423 2023-08-07 21:21:40.712154 oplangchain-0.0.255/oplangchain/prompts/few_shot_with_templates.py
--rw-r--r--   0        0        0     5507 2023-08-07 21:21:40.712154 oplangchain-0.0.255/oplangchain/prompts/loading.py
--rw-r--r--   0        0        0     2254 2023-08-07 21:21:40.713154 oplangchain-0.0.255/oplangchain/prompts/pipeline.py
--rw-r--r--   0        0        0     8136 2023-08-07 21:21:40.713154 oplangchain-0.0.255/oplangchain/prompts/prompt.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.713154 oplangchain-0.0.255/oplangchain/py.typed
--rw-r--r--   0        0        0      111 2023-08-07 21:21:40.714153 oplangchain-0.0.255/oplangchain/python.py
--rw-r--r--   0        0        0      212 2023-08-07 21:21:40.714153 oplangchain-0.0.255/oplangchain/requests.py
--rw-r--r--   0        0        0     3614 2023-08-07 21:21:40.715154 oplangchain-0.0.255/oplangchain/retrievers/__init__.py
--rw-r--r--   0        0        0      582 2023-08-07 21:21:40.716155 oplangchain-0.0.255/oplangchain/retrievers/arxiv.py
--rw-r--r--   0        0        0     4042 2023-08-07 21:21:40.716155 oplangchain-0.0.255/oplangchain/retrievers/azure_cognitive_search.py
--rw-r--r--   0        0        0     3653 2023-08-07 21:21:40.717154 oplangchain-0.0.255/oplangchain/retrievers/bm25.py
--rw-r--r--   0        0        0     2649 2023-08-07 21:21:40.717154 oplangchain-0.0.255/oplangchain/retrievers/chaindesk.py
--rw-r--r--   0        0        0     2998 2023-08-07 21:21:40.718154 oplangchain-0.0.255/oplangchain/retrievers/chatgpt_plugin_retriever.py
--rw-r--r--   0        0        0     2255 2023-08-07 21:21:40.718154 oplangchain-0.0.255/oplangchain/retrievers/contextual_compression.py
--rw-r--r--   0        0        0     2303 2023-08-07 21:21:40.719154 oplangchain-0.0.255/oplangchain/retrievers/databerry.py
--rw-r--r--   0        0        0     6730 2023-08-07 21:21:40.719154 oplangchain-0.0.255/oplangchain/retrievers/docarray.py
--rw-r--r--   0        0        0      591 2023-08-07 21:21:40.720154 oplangchain-0.0.255/oplangchain/retrievers/document_compressors/__init__.py
--rw-r--r--   0        0        0     3658 2023-08-07 21:21:40.720154 oplangchain-0.0.255/oplangchain/retrievers/document_compressors/base.py
--rw-r--r--   0        0        0     3813 2023-08-07 21:21:40.721154 oplangchain-0.0.255/oplangchain/retrievers/document_compressors/chain_extract.py
--rw-r--r--   0        0        0      366 2023-08-07 21:21:40.721154 oplangchain-0.0.255/oplangchain/retrievers/document_compressors/chain_extract_prompt.py
--rw-r--r--   0        0        0     2965 2023-08-07 21:21:40.722154 oplangchain-0.0.255/oplangchain/retrievers/document_compressors/chain_filter.py
--rw-r--r--   0        0        0      231 2023-08-07 21:21:40.722154 oplangchain-0.0.255/oplangchain/retrievers/document_compressors/chain_filter_prompt.py
--rw-r--r--   0        0        0     2961 2023-08-07 21:21:40.723154 oplangchain-0.0.255/oplangchain/retrievers/document_compressors/cohere_rerank.py
--rw-r--r--   0        0        0     3139 2023-08-07 21:21:40.723154 oplangchain-0.0.255/oplangchain/retrievers/document_compressors/embeddings_filter.py
--rw-r--r--   0        0        0     4658 2023-08-07 21:21:40.724154 oplangchain-0.0.255/oplangchain/retrievers/elastic_search_bm25.py
--rw-r--r--   0        0        0     5793 2023-08-07 21:21:40.724154 oplangchain-0.0.255/oplangchain/retrievers/ensemble.py
--rw-r--r--   0        0        0     7430 2023-08-07 21:21:40.724154 oplangchain-0.0.255/oplangchain/retrievers/google_cloud_enterprise_search.py
--rw-r--r--   0        0        0    12601 2023-08-07 21:21:40.725154 oplangchain-0.0.255/oplangchain/retrievers/kendra.py
--rw-r--r--   0        0        0     2527 2023-08-07 21:21:40.725154 oplangchain-0.0.255/oplangchain/retrievers/knn.py
--rw-r--r--   0        0        0     3022 2023-08-07 21:21:40.726154 oplangchain-0.0.255/oplangchain/retrievers/llama_index.py
--rw-r--r--   0        0        0     3373 2023-08-07 21:21:40.726154 oplangchain-0.0.255/oplangchain/retrievers/merger_retriever.py
--rw-r--r--   0        0        0     1439 2023-08-07 21:21:40.727154 oplangchain-0.0.255/oplangchain/retrievers/metal.py
--rw-r--r--   0        0        0     2377 2023-08-07 21:21:40.727154 oplangchain-0.0.255/oplangchain/retrievers/milvus.py
--rw-r--r--   0        0        0     4834 2023-08-07 21:21:40.728154 oplangchain-0.0.255/oplangchain/retrievers/multi_query.py
--rw-r--r--   0        0        0     5436 2023-08-07 21:21:40.728154 oplangchain-0.0.255/oplangchain/retrievers/pinecone_hybrid_search.py
--rw-r--r--   0        0        0      592 2023-08-07 21:21:40.729153 oplangchain-0.0.255/oplangchain/retrievers/pubmed.py
--rw-r--r--   0        0        0       94 2023-08-07 21:21:40.729153 oplangchain-0.0.255/oplangchain/retrievers/pupmed.py
--rw-r--r--   0        0        0     2601 2023-08-07 21:21:40.730154 oplangchain-0.0.255/oplangchain/retrievers/re_phraser.py
--rw-r--r--   0        0        0     1903 2023-08-07 21:21:40.730154 oplangchain-0.0.255/oplangchain/retrievers/remote_retriever.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.731154 oplangchain-0.0.255/oplangchain/retrievers/self_query/__init__.py
--rw-r--r--   0        0        0     5945 2023-08-07 21:21:40.731154 oplangchain-0.0.255/oplangchain/retrievers/self_query/base.py
--rw-r--r--   0        0        0     1442 2023-08-07 21:21:40.732154 oplangchain-0.0.255/oplangchain/retrievers/self_query/chroma.py
--rw-r--r--   0        0        0     2592 2023-08-07 21:21:40.732154 oplangchain-0.0.255/oplangchain/retrievers/self_query/deeplake.py
--rw-r--r--   0        0        0     3595 2023-08-07 21:21:40.732154 oplangchain-0.0.255/oplangchain/retrievers/self_query/myscale.py
--rw-r--r--   0        0        0     1448 2023-08-07 21:21:40.733154 oplangchain-0.0.255/oplangchain/retrievers/self_query/pinecone.py
--rw-r--r--   0        0        0     2811 2023-08-07 21:21:40.733154 oplangchain-0.0.255/oplangchain/retrievers/self_query/qdrant.py
--rw-r--r--   0        0        0     1501 2023-08-07 21:21:40.734154 oplangchain-0.0.255/oplangchain/retrievers/self_query/weaviate.py
--rw-r--r--   0        0        0     3657 2023-08-07 21:21:40.734154 oplangchain-0.0.255/oplangchain/retrievers/svm.py
--rw-r--r--   0        0        0     4035 2023-08-07 21:21:40.735154 oplangchain-0.0.255/oplangchain/retrievers/tfidf.py
--rw-r--r--   0        0        0     5812 2023-08-07 21:21:40.735154 oplangchain-0.0.255/oplangchain/retrievers/time_weighted_retriever.py
--rw-r--r--   0        0        0     4597 2023-08-07 21:21:40.736154 oplangchain-0.0.255/oplangchain/retrievers/vespa_retriever.py
--rw-r--r--   0        0        0     4053 2023-08-07 21:21:40.736154 oplangchain-0.0.255/oplangchain/retrievers/weaviate_hybrid_search.py
--rw-r--r--   0        0        0     8276 2023-08-07 21:21:40.737154 oplangchain-0.0.255/oplangchain/retrievers/web_research.py
--rw-r--r--   0        0        0      605 2023-08-07 21:21:40.737154 oplangchain-0.0.255/oplangchain/retrievers/wikipedia.py
--rw-r--r--   0        0        0     3071 2023-08-07 21:21:40.738154 oplangchain-0.0.255/oplangchain/retrievers/zep.py
--rw-r--r--   0        0        0     2671 2023-08-07 21:21:40.738154 oplangchain-0.0.255/oplangchain/retrievers/zilliz.py
--rw-r--r--   0        0        0     1718 2023-08-07 21:21:40.739154 oplangchain-0.0.255/oplangchain/schema/__init__.py
--rw-r--r--   0        0        0      643 2023-08-07 21:21:40.739154 oplangchain-0.0.255/oplangchain/schema/agent.py
--rw-r--r--   0        0        0     2656 2023-08-07 21:21:40.740154 oplangchain-0.0.255/oplangchain/schema/document.py
--rw-r--r--   0        0        0    10169 2023-08-07 21:21:40.740346 oplangchain-0.0.255/oplangchain/schema/language_model.py
--rw-r--r--   0        0        0     4095 2023-08-07 21:21:40.741154 oplangchain-0.0.255/oplangchain/schema/memory.py
--rw-r--r--   0        0        0     7482 2023-08-07 21:21:40.741154 oplangchain-0.0.255/oplangchain/schema/messages.py
--rw-r--r--   0        0        0     5447 2023-08-07 21:21:40.742154 oplangchain-0.0.255/oplangchain/schema/output.py
--rw-r--r--   0        0        0     7782 2023-08-07 21:21:40.742154 oplangchain-0.0.255/oplangchain/schema/output_parser.py
--rw-r--r--   0        0        0      634 2023-08-07 21:21:40.742154 oplangchain-0.0.255/oplangchain/schema/prompt.py
--rw-r--r--   0        0        0     6865 2023-08-07 21:21:40.743154 oplangchain-0.0.255/oplangchain/schema/prompt_template.py
--rw-r--r--   0        0        0    10045 2023-08-07 21:21:40.743154 oplangchain-0.0.255/oplangchain/schema/retriever.py
--rw-r--r--   0        0        0    40366 2023-08-07 21:21:40.744154 oplangchain-0.0.255/oplangchain/schema/runnable.py
--rw-r--r--   0        0        0      120 2023-08-07 21:21:40.744154 oplangchain-0.0.255/oplangchain/serpapi.py
--rw-r--r--   0        0        0      533 2023-08-07 21:21:40.745154 oplangchain-0.0.255/oplangchain/server.py
--rw-r--r--   0        0        0     3561 2023-08-07 21:21:40.745154 oplangchain-0.0.255/oplangchain/smith/__init__.py
--rw-r--r--   0        0        0     2189 2023-08-07 21:21:40.746154 oplangchain-0.0.255/oplangchain/smith/evaluation/__init__.py
--rw-r--r--   0        0        0     8567 2023-08-07 21:21:40.747154 oplangchain-0.0.255/oplangchain/smith/evaluation/config.py
--rw-r--r--   0        0        0    51494 2023-08-07 21:21:40.747154 oplangchain-0.0.255/oplangchain/smith/evaluation/runner_utils.py
--rw-r--r--   0        0        0    15807 2023-08-07 21:21:40.748154 oplangchain-0.0.255/oplangchain/smith/evaluation/string_run_evaluator.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.748154 oplangchain-0.0.255/oplangchain/smith/evaluation/utils.py
--rw-r--r--   0        0        0      129 2023-08-07 21:21:40.749154 oplangchain-0.0.255/oplangchain/sql_database.py
--rw-r--r--   0        0        0    38439 2023-08-07 21:21:40.749154 oplangchain-0.0.255/oplangchain/text_splitter.py
--rw-r--r--   0        0        0     6594 2023-08-07 21:21:40.750153 oplangchain-0.0.255/oplangchain/tools/__init__.py
--rw-r--r--   0        0        0      237 2023-08-07 21:21:40.751154 oplangchain-0.0.255/oplangchain/tools/amadeus/__init__.py
--rw-r--r--   0        0        0      407 2023-08-07 21:21:40.751154 oplangchain-0.0.255/oplangchain/tools/amadeus/base.py
--rw-r--r--   0        0        0     1974 2023-08-07 21:21:40.752153 oplangchain-0.0.255/oplangchain/tools/amadeus/closest_airport.py
--rw-r--r--   0        0        0     5557 2023-08-07 21:21:40.752153 oplangchain-0.0.255/oplangchain/tools/amadeus/flight_search.py
--rw-r--r--   0        0        0     1123 2023-08-07 21:21:40.753154 oplangchain-0.0.255/oplangchain/tools/amadeus/utils.py
--rw-r--r--   0        0        0       25 2023-08-07 21:21:40.753154 oplangchain-0.0.255/oplangchain/tools/arxiv/__init__.py
--rw-r--r--   0        0        0     1000 2023-08-07 21:21:40.754154 oplangchain-0.0.255/oplangchain/tools/arxiv/tool.py
--rw-r--r--   0        0        0      595 2023-08-07 21:21:40.755154 oplangchain-0.0.255/oplangchain/tools/azure_cognitive_services/__init__.py
--rw-r--r--   0        0        0     5326 2023-08-07 21:21:40.755154 oplangchain-0.0.255/oplangchain/tools/azure_cognitive_services/form_recognizer.py
--rw-r--r--   0        0        0     5255 2023-08-07 21:21:40.756153 oplangchain-0.0.255/oplangchain/tools/azure_cognitive_services/image_analysis.py
--rw-r--r--   0        0        0     4296 2023-08-07 21:21:40.756153 oplangchain-0.0.255/oplangchain/tools/azure_cognitive_services/speech2text.py
--rw-r--r--   0        0        0     3646 2023-08-07 21:21:40.757154 oplangchain-0.0.255/oplangchain/tools/azure_cognitive_services/text2speech.py
--rw-r--r--   0        0        0      776 2023-08-07 21:21:40.757154 oplangchain-0.0.255/oplangchain/tools/azure_cognitive_services/utils.py
--rw-r--r--   0        0        0    26843 2023-08-07 21:21:40.757154 oplangchain-0.0.255/oplangchain/tools/base.py
--rw-r--r--   0        0        0      160 2023-08-07 21:21:40.758154 oplangchain-0.0.255/oplangchain/tools/bing_search/__init__.py
--rw-r--r--   0        0        0     1435 2023-08-07 21:21:40.759154 oplangchain-0.0.255/oplangchain/tools/bing_search/tool.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.759154 oplangchain-0.0.255/oplangchain/tools/brave_search/__init__.py
--rw-r--r--   0        0        0     1336 2023-08-07 21:21:40.760154 oplangchain-0.0.255/oplangchain/tools/brave_search/tool.py
--rw-r--r--   0        0        0     1736 2023-08-07 21:21:40.760154 oplangchain-0.0.255/oplangchain/tools/convert_to_openai.py
--rw-r--r--   0        0        0      258 2023-08-07 21:21:40.761154 oplangchain-0.0.255/oplangchain/tools/dataforseo_api_search/__init__.py
--rw-r--r--   0        0        0     2176 2023-08-07 21:21:40.761154 oplangchain-0.0.255/oplangchain/tools/dataforseo_api_search/tool.py
--rw-r--r--   0        0        0      137 2023-08-07 21:21:40.762154 oplangchain-0.0.255/oplangchain/tools/ddg_search/__init__.py
--rw-r--r--   0        0        0     2315 2023-08-07 21:21:40.763154 oplangchain-0.0.255/oplangchain/tools/ddg_search/tool.py
--rw-r--r--   0        0        0      653 2023-08-07 21:21:40.763154 oplangchain-0.0.255/oplangchain/tools/file_management/__init__.py
--rw-r--r--   0        0        0     1724 2023-08-07 21:21:40.764155 oplangchain-0.0.255/oplangchain/tools/file_management/copy.py
--rw-r--r--   0        0        0     1320 2023-08-07 21:21:40.764155 oplangchain-0.0.255/oplangchain/tools/file_management/delete.py
--rw-r--r--   0        0        0     1940 2023-08-07 21:21:40.765154 oplangchain-0.0.255/oplangchain/tools/file_management/file_search.py
--rw-r--r--   0        0        0     1407 2023-08-07 21:21:40.765154 oplangchain-0.0.255/oplangchain/tools/file_management/list_dir.py
--rw-r--r--   0        0        0     1864 2023-08-07 21:21:40.766154 oplangchain-0.0.255/oplangchain/tools/file_management/move.py
--rw-r--r--   0        0        0     1315 2023-08-07 21:21:40.766154 oplangchain-0.0.255/oplangchain/tools/file_management/read.py
--rw-r--r--   0        0        0     1708 2023-08-07 21:21:40.767154 oplangchain-0.0.255/oplangchain/tools/file_management/utils.py
--rw-r--r--   0        0        0     1589 2023-08-07 21:21:40.767154 oplangchain-0.0.255/oplangchain/tools/file_management/write.py
--rw-r--r--   0        0        0       20 2023-08-07 21:21:40.768154 oplangchain-0.0.255/oplangchain/tools/github/__init__.py
--rw-r--r--   0        0        0     3438 2023-08-07 21:21:40.769155 oplangchain-0.0.255/oplangchain/tools/github/prompt.py
--rw-r--r--   0        0        0      921 2023-08-07 21:21:40.769155 oplangchain-0.0.255/oplangchain/tools/github/tool.py
--rw-r--r--   0        0        0      541 2023-08-07 21:21:40.770154 oplangchain-0.0.255/oplangchain/tools/gmail/__init__.py
--rw-r--r--   0        0        0      976 2023-08-07 21:21:40.770154 oplangchain-0.0.255/oplangchain/tools/gmail/base.py
--rw-r--r--   0        0        0     2539 2023-08-07 21:21:40.771154 oplangchain-0.0.255/oplangchain/tools/gmail/create_draft.py
--rw-r--r--   0        0        0     1727 2023-08-07 21:21:40.771154 oplangchain-0.0.255/oplangchain/tools/gmail/get_message.py
--rw-r--r--   0        0        0     1535 2023-08-07 21:21:40.772154 oplangchain-0.0.255/oplangchain/tools/gmail/get_thread.py
--rw-r--r--   0        0        0     4363 2023-08-07 21:21:40.772154 oplangchain-0.0.255/oplangchain/tools/gmail/search.py
--rw-r--r--   0        0        0     2847 2023-08-07 21:21:40.773153 oplangchain-0.0.255/oplangchain/tools/gmail/send_message.py
--rw-r--r--   0        0        0     4528 2023-08-07 21:21:40.773153 oplangchain-0.0.255/oplangchain/tools/gmail/utils.py
--rw-r--r--   0        0        0      126 2023-08-07 21:21:40.774156 oplangchain-0.0.255/oplangchain/tools/golden_query/__init__.py
--rw-r--r--   0        0        0     1090 2023-08-07 21:21:40.774156 oplangchain-0.0.255/oplangchain/tools/golden_query/tool.py
--rw-r--r--   0        0        0      130 2023-08-07 21:21:40.775227 oplangchain-0.0.255/oplangchain/tools/google_places/__init__.py
--rw-r--r--   0        0        0     1106 2023-08-07 21:21:40.775227 oplangchain-0.0.255/oplangchain/tools/google_places/tool.py
--rw-r--r--   0        0        0      172 2023-08-07 21:21:40.776153 oplangchain-0.0.255/oplangchain/tools/google_search/__init__.py
--rw-r--r--   0        0        0     1461 2023-08-07 21:21:40.777153 oplangchain-0.0.255/oplangchain/tools/google_search/tool.py
--rw-r--r--   0        0        0      220 2023-08-07 21:21:40.777153 oplangchain-0.0.255/oplangchain/tools/google_serper/__init__.py
--rw-r--r--   0        0        0     2076 2023-08-07 21:21:40.778154 oplangchain-0.0.255/oplangchain/tools/google_serper/tool.py
--rw-r--r--   0        0        0       47 2023-08-07 21:21:40.778154 oplangchain-0.0.255/oplangchain/tools/graphql/__init__.py
--rw-r--r--   0        0        0     1186 2023-08-07 21:21:40.779153 oplangchain-0.0.255/oplangchain/tools/graphql/tool.py
--rw-r--r--   0        0        0      122 2023-08-07 21:21:40.779153 oplangchain-0.0.255/oplangchain/tools/human/__init__.py
--rw-r--r--   0        0        0      959 2023-08-07 21:21:40.780154 oplangchain-0.0.255/oplangchain/tools/human/tool.py
--rw-r--r--   0        0        0     2290 2023-08-07 21:21:40.780154 oplangchain-0.0.255/oplangchain/tools/ifttt.py
--rw-r--r--   0        0        0       43 2023-08-07 21:21:40.781153 oplangchain-0.0.255/oplangchain/tools/interaction/__init__.py
--rw-r--r--   0        0        0      454 2023-08-07 21:21:40.782154 oplangchain-0.0.255/oplangchain/tools/interaction/tool.py
--rw-r--r--   0        0        0       17 2023-08-07 21:21:40.782154 oplangchain-0.0.255/oplangchain/tools/jira/__init__.py
--rw-r--r--   0        0        0     3170 2023-08-07 21:21:40.783154 oplangchain-0.0.255/oplangchain/tools/jira/prompt.py
--rw-r--r--   0        0        0     1569 2023-08-07 21:21:40.783154 oplangchain-0.0.255/oplangchain/tools/jira/tool.py
--rw-r--r--   0        0        0       46 2023-08-07 21:21:40.784153 oplangchain-0.0.255/oplangchain/tools/json/__init__.py
--rw-r--r--   0        0        0     4087 2023-08-07 21:21:40.784153 oplangchain-0.0.255/oplangchain/tools/json/tool.py
--rw-r--r--   0        0        0      144 2023-08-07 21:21:40.785153 oplangchain-0.0.255/oplangchain/tools/metaphor_search/__init__.py
--rw-r--r--   0        0        0     2672 2023-08-07 21:21:40.785153 oplangchain-0.0.255/oplangchain/tools/metaphor_search/tool.py
--rw-r--r--   0        0        0      237 2023-08-07 21:21:40.786154 oplangchain-0.0.255/oplangchain/tools/multion/__init__.py
--rw-r--r--   0        0        0     1577 2023-08-07 21:21:40.787153 oplangchain-0.0.255/oplangchain/tools/multion/create_session.py
--rw-r--r--   0        0        0     2116 2023-08-07 21:21:40.787153 oplangchain-0.0.255/oplangchain/tools/multion/update_session.py
--rw-r--r--   0        0        0      101 2023-08-07 21:21:40.788153 oplangchain-0.0.255/oplangchain/tools/nuclia/__init__.py
--rw-r--r--   0        0        0     7575 2023-08-07 21:21:40.788153 oplangchain-0.0.255/oplangchain/tools/nuclia/tool.py
--rw-r--r--   0        0        0      585 2023-08-07 21:21:40.789153 oplangchain-0.0.255/oplangchain/tools/office365/__init__.py
--rw-r--r--   0        0        0      480 2023-08-07 21:21:40.789153 oplangchain-0.0.255/oplangchain/tools/office365/base.py
--rw-r--r--   0        0        0     1832 2023-08-07 21:21:40.790153 oplangchain-0.0.255/oplangchain/tools/office365/create_draft_message.py
--rw-r--r--   0        0        0     4846 2023-08-07 21:21:40.790153 oplangchain-0.0.255/oplangchain/tools/office365/events_search.py
--rw-r--r--   0        0        0     4160 2023-08-07 21:21:40.791154 oplangchain-0.0.255/oplangchain/tools/office365/messages_search.py
--rw-r--r--   0        0        0     2830 2023-08-07 21:21:40.791154 oplangchain-0.0.255/oplangchain/tools/office365/send_event.py
--rw-r--r--   0        0        0     1763 2023-08-07 21:21:40.792153 oplangchain-0.0.255/oplangchain/tools/office365/send_message.py
--rw-r--r--   0        0        0     2136 2023-08-07 21:21:40.792153 oplangchain-0.0.255/oplangchain/tools/office365/utils.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.793153 oplangchain-0.0.255/oplangchain/tools/openapi/__init__.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.793153 oplangchain-0.0.255/oplangchain/tools/openapi/utils/__init__.py
--rw-r--r--   0        0        0    20553 2023-08-07 21:21:40.794153 oplangchain-0.0.255/oplangchain/tools/openapi/utils/api_models.py
--rw-r--r--   0        0        0      156 2023-08-07 21:21:40.794153 oplangchain-0.0.255/oplangchain/tools/openapi/utils/openapi_utils.py
--rw-r--r--   0        0        0      152 2023-08-07 21:21:40.795153 oplangchain-0.0.255/oplangchain/tools/openweathermap/__init__.py
--rw-r--r--   0        0        0      916 2023-08-07 21:21:40.795153 oplangchain-0.0.255/oplangchain/tools/openweathermap/tool.py
--rw-r--r--   0        0        0      684 2023-08-07 21:21:40.796153 oplangchain-0.0.255/oplangchain/tools/playwright/__init__.py
--rw-r--r--   0        0        0     2118 2023-08-07 21:21:40.796153 oplangchain-0.0.255/oplangchain/tools/playwright/base.py
--rw-r--r--   0        0        0     3048 2023-08-07 21:21:40.797153 oplangchain-0.0.255/oplangchain/tools/playwright/click.py
--rw-r--r--   0        0        0     1292 2023-08-07 21:21:40.797153 oplangchain-0.0.255/oplangchain/tools/playwright/current_page.py
--rw-r--r--   0        0        0     3003 2023-08-07 21:21:40.798153 oplangchain-0.0.255/oplangchain/tools/playwright/extract_hyperlinks.py
--rw-r--r--   0        0        0     2335 2023-08-07 21:21:40.798153 oplangchain-0.0.255/oplangchain/tools/playwright/extract_text.py
--rw-r--r--   0        0        0     3695 2023-08-07 21:21:40.799155 oplangchain-0.0.255/oplangchain/tools/playwright/get_elements.py
--rw-r--r--   0        0        0     1756 2023-08-07 21:21:40.799155 oplangchain-0.0.255/oplangchain/tools/playwright/navigate.py
--rw-r--r--   0        0        0     1891 2023-08-07 21:21:40.799155 oplangchain-0.0.255/oplangchain/tools/playwright/navigate_back.py
--rw-r--r--   0        0        0     2813 2023-08-07 21:21:40.800154 oplangchain-0.0.255/oplangchain/tools/playwright/utils.py
--rw-r--r--   0        0        0     2888 2023-08-07 21:21:40.800154 oplangchain-0.0.255/oplangchain/tools/plugin.py
--rw-r--r--   0        0        0       52 2023-08-07 21:21:40.801153 oplangchain-0.0.255/oplangchain/tools/powerbi/__init__.py
--rw-r--r--   0        0        0     7339 2023-08-07 21:21:40.802153 oplangchain-0.0.255/oplangchain/tools/powerbi/prompt.py
--rw-r--r--   0        0        0    11057 2023-08-07 21:21:40.802153 oplangchain-0.0.255/oplangchain/tools/powerbi/tool.py
--rw-r--r--   0        0        0       26 2023-08-07 21:21:40.803153 oplangchain-0.0.255/oplangchain/tools/pubmed/__init__.py
--rw-r--r--   0        0        0     1010 2023-08-07 21:21:40.803153 oplangchain-0.0.255/oplangchain/tools/pubmed/tool.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.804154 oplangchain-0.0.255/oplangchain/tools/python/__init__.py
--rw-r--r--   0        0        0     4313 2023-08-07 21:21:40.804154 oplangchain-0.0.255/oplangchain/tools/python/tool.py
--rw-r--r--   0        0        0       52 2023-08-07 21:21:40.805154 oplangchain-0.0.255/oplangchain/tools/requests/__init__.py
--rw-r--r--   0        0        0     6248 2023-08-07 21:21:40.805154 oplangchain-0.0.255/oplangchain/tools/requests/tool.py
--rw-r--r--   0        0        0       31 2023-08-07 21:21:40.806153 oplangchain-0.0.255/oplangchain/tools/scenexplain/__init__.py
--rw-r--r--   0        0        0     1065 2023-08-07 21:21:40.806153 oplangchain-0.0.255/oplangchain/tools/scenexplain/tool.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.807153 oplangchain-0.0.255/oplangchain/tools/searx_search/__init__.py
--rw-r--r--   0        0        0     2216 2023-08-07 21:21:40.808154 oplangchain-0.0.255/oplangchain/tools/searx_search/tool.py
--rw-r--r--   0        0        0       93 2023-08-07 21:21:40.808154 oplangchain-0.0.255/oplangchain/tools/shell/__init__.py
--rw-r--r--   0        0        0     2384 2023-08-07 21:21:40.809153 oplangchain-0.0.255/oplangchain/tools/shell/tool.py
--rw-r--r--   0        0        0       18 2023-08-07 21:21:40.809153 oplangchain-0.0.255/oplangchain/tools/sleep/__init__.py
--rw-r--r--   0        0        0     1205 2023-08-07 21:21:40.810153 oplangchain-0.0.255/oplangchain/tools/sleep/tool.py
--rw-r--r--   0        0        0       44 2023-08-07 21:21:40.811153 oplangchain-0.0.255/oplangchain/tools/spark_sql/__init__.py
--rw-r--r--   0        0        0      550 2023-08-07 21:21:40.811153 oplangchain-0.0.255/oplangchain/tools/spark_sql/prompt.py
--rw-r--r--   0        0        0     4512 2023-08-07 21:21:40.812153 oplangchain-0.0.255/oplangchain/tools/spark_sql/tool.py
--rw-r--r--   0        0        0       49 2023-08-07 21:21:40.812153 oplangchain-0.0.255/oplangchain/tools/sql_database/__init__.py
--rw-r--r--   0        0        0      597 2023-08-07 21:21:40.813154 oplangchain-0.0.255/oplangchain/tools/sql_database/prompt.py
--rw-r--r--   0        0        0     4574 2023-08-07 21:21:40.813154 oplangchain-0.0.255/oplangchain/tools/sql_database/tool.py
--rw-r--r--   0        0        0      167 2023-08-07 21:21:40.814153 oplangchain-0.0.255/oplangchain/tools/steamship_image_generation/__init__.py
--rw-r--r--   0        0        0     3327 2023-08-07 21:21:40.814153 oplangchain-0.0.255/oplangchain/tools/steamship_image_generation/tool.py
--rw-r--r--   0        0        0     1395 2023-08-07 21:21:40.815153 oplangchain-0.0.255/oplangchain/tools/steamship_image_generation/utils.py
--rw-r--r--   0        0        0       51 2023-08-07 21:21:40.815153 oplangchain-0.0.255/oplangchain/tools/vectorstore/__init__.py
--rw-r--r--   0        0        0     3243 2023-08-07 21:21:40.816153 oplangchain-0.0.255/oplangchain/tools/vectorstore/tool.py
--rw-r--r--   0        0        0       29 2023-08-07 21:21:40.817153 oplangchain-0.0.255/oplangchain/tools/wikipedia/__init__.py
--rw-r--r--   0        0        0      849 2023-08-07 21:21:40.817153 oplangchain-0.0.255/oplangchain/tools/wikipedia/tool.py
--rw-r--r--   0        0        0      146 2023-08-07 21:21:40.818153 oplangchain-0.0.255/oplangchain/tools/wolfram_alpha/__init__.py
--rw-r--r--   0        0        0      869 2023-08-07 21:21:40.818153 oplangchain-0.0.255/oplangchain/tools/wolfram_alpha/tool.py
--rw-r--r--   0        0        0        0 2023-08-07 21:21:40.819153 oplangchain-0.0.255/oplangchain/tools/youtube/__init__.py
--rw-r--r--   0        0        0     1661 2023-08-07 21:21:40.819153 oplangchain-0.0.255/oplangchain/tools/youtube/search.py
--rw-r--r--   0        0        0      170 2023-08-07 21:21:40.820154 oplangchain-0.0.255/oplangchain/tools/zapier/__init__.py
--rw-r--r--   0        0        0     1182 2023-08-07 21:21:40.820154 oplangchain-0.0.255/oplangchain/tools/zapier/prompt.py
--rw-r--r--   0        0        0     7065 2023-08-07 21:21:40.821156 oplangchain-0.0.255/oplangchain/tools/zapier/tool.py
--rw-r--r--   0        0        0     2868 2023-08-07 21:21:40.821156 oplangchain-0.0.255/oplangchain/utilities/__init__.py
--rw-r--r--   0        0        0     6386 2023-08-07 21:21:40.822153 oplangchain-0.0.255/oplangchain/utilities/arxiv.py
--rw-r--r--   0        0        0      274 2023-08-07 21:21:40.822153 oplangchain-0.0.255/oplangchain/utilities/asyncio.py
--rw-r--r--   0        0        0     2419 2023-08-07 21:21:40.823154 oplangchain-0.0.255/oplangchain/utilities/awslambda.py
--rw-r--r--   0        0        0     5703 2023-08-07 21:21:40.823154 oplangchain-0.0.255/oplangchain/utilities/bash.py
--rw-r--r--   0        0        0     2481 2023-08-07 21:21:40.824154 oplangchain-0.0.255/oplangchain/utilities/bibtex.py
--rw-r--r--   0        0        0     3333 2023-08-07 21:21:40.824154 oplangchain-0.0.255/oplangchain/utilities/bing_search.py
--rw-r--r--   0        0        0     2326 2023-08-07 21:21:40.825153 oplangchain-0.0.255/oplangchain/utilities/brave_search.py
--rw-r--r--   0        0        0     7832 2023-08-07 21:21:40.825153 oplangchain-0.0.255/oplangchain/utilities/dataforseo_api_search.py
--rw-r--r--   0        0        0     3764 2023-08-07 21:21:40.825153 oplangchain-0.0.255/oplangchain/utilities/duckduckgo_search.py
--rw-r--r--   0        0        0    11594 2023-08-07 21:21:40.826153 oplangchain-0.0.255/oplangchain/utilities/github.py
--rw-r--r--   0        0        0     1836 2023-08-07 21:21:40.826153 oplangchain-0.0.255/oplangchain/utilities/golden_query.py
--rw-r--r--   0        0        0     4065 2023-08-07 21:21:40.827153 oplangchain-0.0.255/oplangchain/utilities/google_places_api.py
--rw-r--r--   0        0        0     5094 2023-08-07 21:21:40.827153 oplangchain-0.0.255/oplangchain/utilities/google_search.py
--rw-r--r--   0        0        0     6503 2023-08-07 21:21:40.828153 oplangchain-0.0.255/oplangchain/utilities/google_serper.py
--rw-r--r--   0        0        0     1885 2023-08-07 21:21:40.828153 oplangchain-0.0.255/oplangchain/utilities/graphql.py
--rw-r--r--   0        0        0     6173 2023-08-07 21:21:40.828153 oplangchain-0.0.255/oplangchain/utilities/jira.py
--rw-r--r--   0        0        0     1972 2023-08-07 21:21:40.829153 oplangchain-0.0.255/oplangchain/utilities/loading.py
--rw-r--r--   0        0        0     2642 2023-08-07 21:21:40.829153 oplangchain-0.0.255/oplangchain/utilities/max_compute.py
--rw-r--r--   0        0        0     6705 2023-08-07 21:21:40.830153 oplangchain-0.0.255/oplangchain/utilities/metaphor_search.py
--rw-r--r--   0        0        0    10299 2023-08-07 21:21:40.830153 oplangchain-0.0.255/oplangchain/utilities/openapi.py
--rw-r--r--   0        0        0     2440 2023-08-07 21:21:40.831154 oplangchain-0.0.255/oplangchain/utilities/openweathermap.py
--rw-r--r--   0        0        0     2198 2023-08-07 21:21:40.831154 oplangchain-0.0.255/oplangchain/utilities/portkey.py
--rw-r--r--   0        0        0    11237 2023-08-07 21:21:40.832154 oplangchain-0.0.255/oplangchain/utilities/powerbi.py
--rw-r--r--   0        0        0     5627 2023-08-07 21:21:40.832154 oplangchain-0.0.255/oplangchain/utilities/pupmed.py
--rw-r--r--   0        0        0     2141 2023-08-07 21:21:40.833154 oplangchain-0.0.255/oplangchain/utilities/python.py
--rw-r--r--   0        0        0     5435 2023-08-07 21:21:40.833154 oplangchain-0.0.255/oplangchain/utilities/redis.py
--rw-r--r--   0        0        0     7120 2023-08-07 21:21:40.834153 oplangchain-0.0.255/oplangchain/utilities/requests.py
--rw-r--r--   0        0        0     2198 2023-08-07 21:21:40.834153 oplangchain-0.0.255/oplangchain/utilities/scenexplain.py
--rw-r--r--   0        0        0    16529 2023-08-07 21:21:40.835153 oplangchain-0.0.255/oplangchain/utilities/searx_search.py
--rw-r--r--   0        0        0     6025 2023-08-07 21:21:40.835153 oplangchain-0.0.255/oplangchain/utilities/serpapi.py
--rw-r--r--   0        0        0     6964 2023-08-07 21:21:40.836153 oplangchain-0.0.255/oplangchain/utilities/spark_sql.py
--rw-r--r--   0        0        0    18263 2023-08-07 21:21:40.836153 oplangchain-0.0.255/oplangchain/utilities/sql_database.py
--rw-r--r--   0        0        0     3409 2023-08-07 21:21:40.837154 oplangchain-0.0.255/oplangchain/utilities/twilio.py
--rw-r--r--   0        0        0     1457 2023-08-07 21:21:40.837154 oplangchain-0.0.255/oplangchain/utilities/vertexai.py
--rw-r--r--   0        0        0     3920 2023-08-07 21:21:40.838153 oplangchain-0.0.255/oplangchain/utilities/wikipedia.py
--rw-r--r--   0        0        0     1989 2023-08-07 21:21:40.838153 oplangchain-0.0.255/oplangchain/utilities/wolfram_alpha.py
--rw-r--r--   0        0        0    11560 2023-08-07 21:21:40.838153 oplangchain-0.0.255/oplangchain/utilities/zapier.py
--rw-r--r--   0        0        0     1149 2023-08-07 21:21:40.839153 oplangchain-0.0.255/oplangchain/utils/__init__.py
--rw-r--r--   0        0        0      873 2023-08-07 21:21:40.840155 oplangchain-0.0.255/oplangchain/utils/env.py
--rw-r--r--   0        0        0     1237 2023-08-07 21:21:40.840155 oplangchain-0.0.255/oplangchain/utils/formatting.py
--rw-r--r--   0        0        0     1289 2023-08-07 21:21:40.841153 oplangchain-0.0.255/oplangchain/utils/input.py
--rw-r--r--   0        0        0     2016 2023-08-07 21:21:40.841153 oplangchain-0.0.255/oplangchain/utils/math.py
--rw-r--r--   0        0        0      908 2023-08-07 21:21:40.842153 oplangchain-0.0.255/oplangchain/utils/strings.py
--rw-r--r--   0        0        0     5606 2023-08-07 21:21:40.842153 oplangchain-0.0.255/oplangchain/utils/utils.py
--rw-r--r--   0        0        0     4003 2023-08-07 21:21:40.843153 oplangchain-0.0.255/oplangchain/vectorstores/__init__.py
--rw-r--r--   0        0        0     2025 2023-08-07 21:21:40.844154 oplangchain-0.0.255/oplangchain/vectorstores/_pgvector_data_models.py
--rw-r--r--   0        0        0    13535 2023-08-07 21:21:40.845153 oplangchain-0.0.255/oplangchain/vectorstores/alibabacloud_opensearch.py
--rw-r--r--   0        0        0    15792 2023-08-07 21:21:40.845153 oplangchain-0.0.255/oplangchain/vectorstores/analyticdb.py
--rw-r--r--   0        0        0    16575 2023-08-07 21:21:40.846155 oplangchain-0.0.255/oplangchain/vectorstores/annoy.py
--rw-r--r--   0        0        0    12133 2023-08-07 21:21:40.846155 oplangchain-0.0.255/oplangchain/vectorstores/atlas.py
--rw-r--r--   0        0        0    21220 2023-08-07 21:21:40.847154 oplangchain-0.0.255/oplangchain/vectorstores/awadb.py
--rw-r--r--   0        0        0    20714 2023-08-07 21:21:40.848154 oplangchain-0.0.255/oplangchain/vectorstores/azuresearch.py
--rw-r--r--   0        0        0    22433 2023-08-07 21:21:40.848154 oplangchain-0.0.255/oplangchain/vectorstores/base.py
--rw-r--r--   0        0        0    13392 2023-08-07 21:21:40.849154 oplangchain-0.0.255/oplangchain/vectorstores/cassandra.py
--rw-r--r--   0        0        0    23808 2023-08-07 21:21:40.849154 oplangchain-0.0.255/oplangchain/vectorstores/chroma.py
--rw-r--r--   0        0        0    12729 2023-08-07 21:21:40.850154 oplangchain-0.0.255/oplangchain/vectorstores/clarifai.py
--rw-r--r--   0        0        0    17811 2023-08-07 21:21:40.850154 oplangchain-0.0.255/oplangchain/vectorstores/clickhouse.py
--rw-r--r--   0        0        0    34968 2023-08-07 21:21:40.851154 oplangchain-0.0.255/oplangchain/vectorstores/deeplake.py
--rw-r--r--   0        0        0      216 2023-08-07 21:21:40.851154 oplangchain-0.0.255/oplangchain/vectorstores/docarray/__init__.py
--rw-r--r--   0        0        0     6871 2023-08-07 21:21:40.852153 oplangchain-0.0.255/oplangchain/vectorstores/docarray/base.py
--rw-r--r--   0        0        0     4057 2023-08-07 21:21:40.852153 oplangchain-0.0.255/oplangchain/vectorstores/docarray/hnsw.py
--rw-r--r--   0        0        0     2411 2023-08-07 21:21:40.853153 oplangchain-0.0.255/oplangchain/vectorstores/docarray/in_memory.py
--rw-r--r--   0        0        0    27775 2023-08-07 21:21:40.853153 oplangchain-0.0.255/oplangchain/vectorstores/elastic_vector_search.py
--rw-r--r--   0        0        0    29115 2023-08-07 21:21:40.854153 oplangchain-0.0.255/oplangchain/vectorstores/faiss.py
--rw-r--r--   0        0        0    16399 2023-08-07 21:21:40.854153 oplangchain-0.0.255/oplangchain/vectorstores/hologres.py
--rw-r--r--   0        0        0     4236 2023-08-07 21:21:40.855153 oplangchain-0.0.255/oplangchain/vectorstores/lancedb.py
--rw-r--r--   0        0        0    17152 2023-08-07 21:21:40.855153 oplangchain-0.0.255/oplangchain/vectorstores/marqo.py
--rw-r--r--   0        0        0    15176 2023-08-07 21:21:40.856154 oplangchain-0.0.255/oplangchain/vectorstores/matching_engine.py
--rw-r--r--   0        0        0    10421 2023-08-07 21:21:40.856154 oplangchain-0.0.255/oplangchain/vectorstores/meilisearch.py
--rw-r--r--   0        0        0    31468 2023-08-07 21:21:40.857154 oplangchain-0.0.255/oplangchain/vectorstores/milvus.py
--rw-r--r--   0        0        0    12345 2023-08-07 21:21:40.857154 oplangchain-0.0.255/oplangchain/vectorstores/mongodb_atlas.py
--rw-r--r--   0        0        0    16539 2023-08-07 21:21:40.858154 oplangchain-0.0.255/oplangchain/vectorstores/myscale.py
--rw-r--r--   0        0        0    27686 2023-08-07 21:21:40.870155 oplangchain-0.0.255/oplangchain/vectorstores/opensearch_vector_search.py
--rw-r--r--   0        0        0    17344 2023-08-07 21:21:40.871154 oplangchain-0.0.255/oplangchain/vectorstores/pgembedding.py
--rw-r--r--   0        0        0    21251 2023-08-07 21:21:40.871154 oplangchain-0.0.255/oplangchain/vectorstores/pgvector.py
--rw-r--r--   0        0        0    14905 2023-08-07 21:21:40.872154 oplangchain-0.0.255/oplangchain/vectorstores/pinecone.py
--rw-r--r--   0        0        0    68527 2023-08-07 21:21:40.872154 oplangchain-0.0.255/oplangchain/vectorstores/qdrant.py
--rw-r--r--   0        0        0    23138 2023-08-07 21:21:40.873155 oplangchain-0.0.255/oplangchain/vectorstores/redis.py
--rw-r--r--   0        0        0    12186 2023-08-07 21:21:40.873155 oplangchain-0.0.255/oplangchain/vectorstores/rocksetdb.py
--rw-r--r--   0        0        0    19511 2023-08-07 21:21:40.874154 oplangchain-0.0.255/oplangchain/vectorstores/scann.py
--rw-r--r--   0        0        0    18252 2023-08-07 21:21:40.874154 oplangchain-0.0.255/oplangchain/vectorstores/singlestoredb.py
--rw-r--r--   0        0        0    12385 2023-08-07 21:21:40.875154 oplangchain-0.0.255/oplangchain/vectorstores/sklearn.py
--rw-r--r--   0        0        0    17219 2023-08-07 21:21:40.875154 oplangchain-0.0.255/oplangchain/vectorstores/starrocks.py
--rw-r--r--   0        0        0    14233 2023-08-07 21:21:40.876155 oplangchain-0.0.255/oplangchain/vectorstores/supabase.py
--rw-r--r--   0        0        0     8878 2023-08-07 21:21:40.876155 oplangchain-0.0.255/oplangchain/vectorstores/tair.py
--rw-r--r--   0        0        0     4878 2023-08-07 21:21:40.877154 oplangchain-0.0.255/oplangchain/vectorstores/tigris.py
--rw-r--r--   0        0        0     9728 2023-08-07 21:21:40.877154 oplangchain-0.0.255/oplangchain/vectorstores/typesense.py
--rw-r--r--   0        0        0     1790 2023-08-07 21:21:40.879153 oplangchain-0.0.255/oplangchain/vectorstores/utils.py
--rw-r--r--   0        0        0    15857 2023-08-07 21:21:40.880157 oplangchain-0.0.255/oplangchain/vectorstores/vectara.py
--rw-r--r--   0        0        0    16875 2023-08-07 21:21:40.881156 oplangchain-0.0.255/oplangchain/vectorstores/weaviate.py
--rw-r--r--   0        0        0     7559 2023-08-07 21:21:40.881156 oplangchain-0.0.255/oplangchain/vectorstores/zilliz.py
--rw-r--r--   0        0        0    13302 2023-08-07 22:19:02.788154 oplangchain-0.0.255/pyproject.toml
--rw-r--r--   0        0        0     5724 2023-08-07 21:21:40.386154 oplangchain-0.0.255/README.md
--rw-r--r--   0        0        0    14950 1970-01-01 00:00:00.000000 oplangchain-0.0.255/PKG-INFO
+-rw-r--r--   0        0        0     3074 2023-08-07 14:51:51.064476 oplangchain-0.1.0/oplangchain/__init__.py
+-rw-r--r--   0        0        0     3396 2023-08-07 14:51:51.065474 oplangchain-0.1.0/oplangchain/agents/__init__.py
+-rw-r--r--   0        0        0    41297 2023-08-07 14:51:51.065474 oplangchain-0.1.0/oplangchain/agents/agent.py
+-rw-r--r--   0        0        0    18325 2023-08-07 14:51:51.066475 oplangchain-0.1.0/oplangchain/agents/agent_iterator.py
+-rw-r--r--   0        0        0     3464 2023-08-07 14:51:51.067476 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/__init__.py
+-rw-r--r--   0        0        0      873 2023-08-07 14:51:51.067476 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/amadeus/toolkit.py
+-rw-r--r--   0        0        0      919 2023-08-07 14:51:51.068473 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/azure_cognitive_services.py
+-rw-r--r--   0        0        0      369 2023-08-07 14:51:51.068473 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/base.py
+-rw-r--r--   0        0        0        0 2023-08-07 14:51:51.069473 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/conversational_retrieval/__init__.py
+-rw-r--r--   0        0        0     3377 2023-08-07 14:51:51.070474 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/conversational_retrieval/openai_functions.py
+-rw-r--r--   0        0        0      730 2023-08-07 14:51:51.070474 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/conversational_retrieval/tool.py
+-rw-r--r--   0        0        0       19 2023-08-07 14:51:51.071474 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/csv/__init__.py
+-rw-r--r--   0        0        0     1148 2023-08-07 14:51:51.071474 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/csv/base.py
+-rw-r--r--   0        0        0      174 2023-08-07 14:51:51.072475 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/file_management/__init__.py
+-rw-r--r--   0        0        0     2074 2023-08-07 14:51:51.074475 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/file_management/toolkit.py
+-rw-r--r--   0        0        0       22 2023-08-07 14:51:51.075476 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/github/__init__.py
+-rw-r--r--   0        0        0     2484 2023-08-07 14:51:51.075476 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/github/toolkit.py
+-rw-r--r--   0        0        0       21 2023-08-07 14:51:51.076475 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/gmail/__init__.py
+-rw-r--r--   0        0        0     1567 2023-08-07 14:51:51.077473 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/gmail/toolkit.py
+-rw-r--r--   0        0        0       20 2023-08-07 14:51:51.077473 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/jira/__init__.py
+-rw-r--r--   0        0        0     1919 2023-08-07 14:51:51.078473 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/jira/toolkit.py
+-rw-r--r--   0        0        0       18 2023-08-07 14:51:51.079473 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/json/__init__.py
+-rw-r--r--   0        0        0     1713 2023-08-07 14:51:51.079473 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/json/base.py
+-rw-r--r--   0        0        0     1819 2023-08-07 14:51:51.080474 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/json/prompt.py
+-rw-r--r--   0        0        0      555 2023-08-07 14:51:51.081474 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/json/toolkit.py
+-rw-r--r--   0        0        0       23 2023-08-07 14:51:51.081474 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/multion/__init__.py
+-rw-r--r--   0        0        0      660 2023-08-07 14:51:51.082473 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/multion/toolkit.py
+-rw-r--r--   0        0        0        0 2023-08-07 14:51:51.082473 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/nla/__init__.py
+-rw-r--r--   0        0        0     1937 2023-08-07 14:51:51.083474 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/nla/tool.py
+-rw-r--r--   0        0        0     3765 2023-08-07 14:51:51.084474 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/nla/toolkit.py
+-rw-r--r--   0        0        0       25 2023-08-07 14:51:51.084474 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/office365/__init__.py
+-rw-r--r--   0        0        0     1171 2023-08-07 14:51:51.085475 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/office365/toolkit.py
+-rw-r--r--   0        0        0       26 2023-08-07 14:51:51.086474 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/openapi/__init__.py
+-rw-r--r--   0        0        0     2140 2023-08-07 14:51:51.086474 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/openapi/base.py
+-rw-r--r--   0        0        0    11233 2023-08-07 14:51:51.087474 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/openapi/planner.py
+-rw-r--r--   0        0        0    10460 2023-08-07 14:51:51.088474 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/openapi/planner_prompt.py
+-rw-r--r--   0        0        0     1743 2023-08-07 14:51:51.088474 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/openapi/prompt.py
+-rw-r--r--   0        0        0     3835 2023-08-07 14:51:51.089476 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/openapi/spec.py
+-rw-r--r--   0        0        0     2374 2023-08-07 14:51:51.090474 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/openapi/toolkit.py
+-rw-r--r--   0        0        0       22 2023-08-07 14:51:51.091474 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/pandas/__init__.py
+-rw-r--r--   0        0        0    11518 2023-08-07 14:51:51.091474 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/pandas/base.py
+-rw-r--r--   0        0        0     1113 2023-08-07 14:51:51.092475 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/pandas/prompt.py
+-rw-r--r--   0        0        0      162 2023-08-07 14:51:51.092475 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/playwright/__init__.py
+-rw-r--r--   0        0        0     3014 2023-08-07 14:51:51.093473 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/playwright/toolkit.py
+-rw-r--r--   0        0        0       22 2023-08-07 14:51:51.094473 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/powerbi/__init__.py
+-rw-r--r--   0        0        0     2322 2023-08-07 14:51:51.094473 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/powerbi/base.py
+-rw-r--r--   0        0        0     2489 2023-08-07 14:51:51.095474 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/powerbi/chat_base.py
+-rw-r--r--   0        0        0     2773 2023-08-07 14:51:51.095474 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/powerbi/prompt.py
+-rw-r--r--   0        0        0     3217 2023-08-07 14:51:51.096473 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/powerbi/toolkit.py
+-rw-r--r--   0        0        0        0 2023-08-07 14:51:51.096473 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/python/__init__.py
+-rw-r--r--   0        0        0     2200 2023-08-07 14:51:51.097476 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/python/base.py
+-rw-r--r--   0        0        0      513 2023-08-07 14:51:51.098475 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/python/prompt.py
+-rw-r--r--   0        0        0       20 2023-08-07 14:51:51.098475 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/spark/__init__.py
+-rw-r--r--   0        0        0     2734 2023-08-07 14:51:51.099473 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/spark/base.py
+-rw-r--r--   0        0        0      295 2023-08-07 14:51:51.099473 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/spark/prompt.py
+-rw-r--r--   0        0        0       23 2023-08-07 14:51:51.100475 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/spark_sql/__init__.py
+-rw-r--r--   0        0        0     2072 2023-08-07 14:51:51.100475 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/spark_sql/base.py
+-rw-r--r--   0        0        0     1202 2023-08-07 14:51:51.101474 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/spark_sql/prompt.py
+-rw-r--r--   0        0        0     1034 2023-08-07 14:51:51.101474 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/spark_sql/toolkit.py
+-rw-r--r--   0        0        0       17 2023-08-07 14:51:51.102474 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/sql/__init__.py
+-rw-r--r--   0        0        0     3434 2023-08-07 14:51:51.102474 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/sql/base.py
+-rw-r--r--   0        0        0     1428 2023-08-07 14:51:51.103474 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/sql/prompt.py
+-rw-r--r--   0        0        0     2816 2023-08-07 14:51:51.103474 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/sql/toolkit.py
+-rw-r--r--   0        0        0       56 2023-08-07 14:51:51.104474 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/vectorstore/__init__.py
+-rw-r--r--   0        0        0     2408 2023-08-07 14:51:51.105474 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/vectorstore/base.py
+-rw-r--r--   0        0        0      834 2023-08-07 14:51:51.105474 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/vectorstore/prompt.py
+-rw-r--r--   0        0        0     2961 2023-08-07 14:51:51.106474 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/vectorstore/toolkit.py
+-rw-r--r--   0        0        0       23 2023-08-07 14:51:51.107474 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/xorbits/__init__.py
+-rw-r--r--   0        0        0     3105 2023-08-07 14:51:51.107474 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/xorbits/base.py
+-rw-r--r--   0        0        0     1070 2023-08-07 14:51:51.107474 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/xorbits/prompt.py
+-rw-r--r--   0        0        0       22 2023-08-07 14:51:51.108474 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/zapier/__init__.py
+-rw-r--r--   0        0        0     1609 2023-08-07 14:51:51.109473 oplangchain-0.1.0/oplangchain/agents/agent_toolkits/zapier/toolkit.py
+-rw-r--r--   0        0        0      688 2023-08-07 14:51:51.109473 oplangchain-0.1.0/oplangchain/agents/agent_types.py
+-rw-r--r--   0        0        0        0 2023-08-07 14:51:51.110474 oplangchain-0.1.0/oplangchain/agents/chat/__init__.py
+-rw-r--r--   0        0        0     4908 2023-08-07 14:51:51.110474 oplangchain-0.1.0/oplangchain/agents/chat/base.py
+-rw-r--r--   0        0        0     1706 2023-08-07 14:51:51.111474 oplangchain-0.1.0/oplangchain/agents/chat/output_parser.py
+-rw-r--r--   0        0        0     1158 2023-08-07 14:51:51.111474 oplangchain-0.1.0/oplangchain/agents/chat/prompt.py
+-rw-r--r--   0        0        0       75 2023-08-07 14:51:51.112474 oplangchain-0.1.0/oplangchain/agents/conversational/__init__.py
+-rw-r--r--   0        0        0     4820 2023-08-07 14:51:51.113475 oplangchain-0.1.0/oplangchain/agents/conversational/base.py
+-rw-r--r--   0        0        0     1150 2023-08-07 14:51:51.113475 oplangchain-0.1.0/oplangchain/agents/conversational/output_parser.py
+-rw-r--r--   0        0        0     1859 2023-08-07 14:51:51.114475 oplangchain-0.1.0/oplangchain/agents/conversational/prompt.py
+-rw-r--r--   0        0        0       75 2023-08-07 14:51:51.114475 oplangchain-0.1.0/oplangchain/agents/conversational_chat/__init__.py
+-rw-r--r--   0        0        0     4977 2023-08-07 14:51:51.115474 oplangchain-0.1.0/oplangchain/agents/conversational_chat/base.py
+-rw-r--r--   0        0        0     2256 2023-08-07 14:51:51.115474 oplangchain-0.1.0/oplangchain/agents/conversational_chat/output_parser.py
+-rw-r--r--   0        0        0     2757 2023-08-07 14:51:51.116474 oplangchain-0.1.0/oplangchain/agents/conversational_chat/prompt.py
+-rw-r--r--   0        0        0     2995 2023-08-07 14:51:51.116474 oplangchain-0.1.0/oplangchain/agents/initialize.py
+-rw-r--r--   0        0        0    17319 2023-08-07 14:51:51.117475 oplangchain-0.1.0/oplangchain/agents/load_tools.py
+-rw-r--r--   0        0        0     4371 2023-08-07 14:51:51.117475 oplangchain-0.1.0/oplangchain/agents/loading.py
+-rw-r--r--   0        0        0       86 2023-08-07 14:51:51.118474 oplangchain-0.1.0/oplangchain/agents/mrkl/__init__.py
+-rw-r--r--   0        0        0     7097 2023-08-07 14:51:51.119474 oplangchain-0.1.0/oplangchain/agents/mrkl/base.py
+-rw-r--r--   0        0        0     2706 2023-08-07 14:51:51.119474 oplangchain-0.1.0/oplangchain/agents/mrkl/output_parser.py
+-rw-r--r--   0        0        0      641 2023-08-07 14:51:51.119474 oplangchain-0.1.0/oplangchain/agents/mrkl/prompt.py
+-rw-r--r--   0        0        0        0 2023-08-07 14:51:51.120474 oplangchain-0.1.0/oplangchain/agents/openai_functions_agent/__init__.py
+-rw-r--r--   0        0        0     2527 2023-08-07 14:51:51.121473 oplangchain-0.1.0/oplangchain/agents/openai_functions_agent/agent_token_buffer_memory.py
+-rw-r--r--   0        0        0    11896 2023-08-07 14:51:51.121473 oplangchain-0.1.0/oplangchain/agents/openai_functions_agent/base.py
+-rw-r--r--   0        0        0        0 2023-08-07 14:51:51.122475 oplangchain-0.1.0/oplangchain/agents/openai_functions_multi_agent/__init__.py
+-rw-r--r--   0        0        0    13337 2023-08-07 14:51:51.122475 oplangchain-0.1.0/oplangchain/agents/openai_functions_multi_agent/base.py
+-rw-r--r--   0        0        0       76 2023-08-07 14:51:51.123474 oplangchain-0.1.0/oplangchain/agents/react/__init__.py
+-rw-r--r--   0        0        0     5664 2023-08-07 14:51:51.124474 oplangchain-0.1.0/oplangchain/agents/react/base.py
+-rw-r--r--   0        0        0     1188 2023-08-07 14:51:51.124474 oplangchain-0.1.0/oplangchain/agents/react/output_parser.py
+-rw-r--r--   0        0        0     1901 2023-08-07 14:51:51.125474 oplangchain-0.1.0/oplangchain/agents/react/textworld_prompt.py
+-rw-r--r--   0        0        0     6122 2023-08-07 14:51:51.125474 oplangchain-0.1.0/oplangchain/agents/react/wiki_prompt.py
+-rw-r--r--   0        0        0     1085 2023-08-07 14:51:51.126475 oplangchain-0.1.0/oplangchain/agents/schema.py
+-rw-r--r--   0        0        0      106 2023-08-07 14:51:51.127474 oplangchain-0.1.0/oplangchain/agents/self_ask_with_search/__init__.py
+-rw-r--r--   0        0        0     3094 2023-08-07 14:51:51.127474 oplangchain-0.1.0/oplangchain/agents/self_ask_with_search/base.py
+-rw-r--r--   0        0        0      962 2023-08-07 14:51:51.128474 oplangchain-0.1.0/oplangchain/agents/self_ask_with_search/output_parser.py
+-rw-r--r--   0        0        0     1921 2023-08-07 14:51:51.128474 oplangchain-0.1.0/oplangchain/agents/self_ask_with_search/prompt.py
+-rw-r--r--   0        0        0        0 2023-08-07 14:51:51.129475 oplangchain-0.1.0/oplangchain/agents/structured_chat/__init__.py
+-rw-r--r--   0        0        0     5144 2023-08-07 14:51:51.129475 oplangchain-0.1.0/oplangchain/agents/structured_chat/base.py
+-rw-r--r--   0        0        0     3452 2023-08-07 14:51:51.130474 oplangchain-0.1.0/oplangchain/agents/structured_chat/output_parser.py
+-rw-r--r--   0        0        0      992 2023-08-07 14:51:51.130474 oplangchain-0.1.0/oplangchain/agents/structured_chat/prompt.py
+-rw-r--r--   0        0        0     1402 2023-08-07 14:51:51.131474 oplangchain-0.1.0/oplangchain/agents/tools.py
+-rw-r--r--   0        0        0     1475 2023-08-07 14:51:51.131474 oplangchain-0.1.0/oplangchain/agents/types.py
+-rw-r--r--   0        0        0      384 2023-08-07 14:51:51.132475 oplangchain-0.1.0/oplangchain/agents/utils.py
+-rw-r--r--   0        0        0        0 2023-08-07 14:51:51.132475 oplangchain-0.1.0/oplangchain/agents/xml/__init__.py
+-rw-r--r--   0        0        0     3887 2023-08-07 14:51:51.133474 oplangchain-0.1.0/oplangchain/agents/xml/base.py
+-rw-r--r--   0        0        0      749 2023-08-07 14:51:51.133474 oplangchain-0.1.0/oplangchain/agents/xml/prompt.py
+-rw-r--r--   0        0        0      218 2023-08-07 14:51:51.134474 oplangchain-0.1.0/oplangchain/base_language.py
+-rw-r--r--   0        0        0    24769 2023-08-07 14:51:51.134474 oplangchain-0.1.0/oplangchain/cache.py
+-rw-r--r--   0        0        0     2839 2023-08-07 14:51:51.135474 oplangchain-0.1.0/oplangchain/callbacks/__init__.py
+-rw-r--r--   0        0        0    14484 2023-08-07 14:51:51.136474 oplangchain-0.1.0/oplangchain/callbacks/aim_callback.py
+-rw-r--r--   0        0        0    13719 2023-08-07 14:51:51.136474 oplangchain-0.1.0/oplangchain/callbacks/argilla_callback.py
+-rw-r--r--   0        0        0     7503 2023-08-07 14:51:51.137474 oplangchain-0.1.0/oplangchain/callbacks/arize_callback.py
+-rw-r--r--   0        0        0    11343 2023-08-07 14:51:51.137474 oplangchain-0.1.0/oplangchain/callbacks/arthur_callback.py
+-rw-r--r--   0        0        0    15174 2023-08-07 14:51:51.138475 oplangchain-0.1.0/oplangchain/callbacks/base.py
+-rw-r--r--   0        0        0    18496 2023-08-07 14:51:51.139474 oplangchain-0.1.0/oplangchain/callbacks/clearml_callback.py
+-rw-r--r--   0        0        0    23238 2023-08-07 14:51:51.139474 oplangchain-0.1.0/oplangchain/callbacks/comet_ml_callback.py
+-rw-r--r--   0        0        0     6424 2023-08-07 14:51:51.140475 oplangchain-0.1.0/oplangchain/callbacks/context_callback.py
+-rw-r--r--   0        0        0     2561 2023-08-07 14:51:51.140475 oplangchain-0.1.0/oplangchain/callbacks/file.py
+-rw-r--r--   0        0        0    13157 2023-08-07 14:51:51.141475 oplangchain-0.1.0/oplangchain/callbacks/flyte_callback.py
+-rw-r--r--   0        0        0     1410 2023-08-07 14:51:51.141475 oplangchain-0.1.0/oplangchain/callbacks/human.py
+-rw-r--r--   0        0        0     5570 2023-08-07 14:51:51.142475 oplangchain-0.1.0/oplangchain/callbacks/infino_callback.py
+-rw-r--r--   0        0        0    53773 2023-08-07 14:51:51.142475 oplangchain-0.1.0/oplangchain/callbacks/manager.py
+-rw-r--r--   0        0        0    24163 2023-08-07 14:51:51.143474 oplangchain-0.1.0/oplangchain/callbacks/mlflow_callback.py
+-rw-r--r--   0        0        0     5348 2023-08-07 14:51:51.143474 oplangchain-0.1.0/oplangchain/callbacks/openai_info.py
+-rw-r--r--   0        0        0     5523 2023-08-07 14:51:51.144475 oplangchain-0.1.0/oplangchain/callbacks/promptlayer_callback.py
+-rw-r--r--   0        0        0     8823 2023-08-07 14:51:51.144475 oplangchain-0.1.0/oplangchain/callbacks/sagemaker_callback.py
+-rw-r--r--   0        0        0     3203 2023-08-07 14:51:51.145474 oplangchain-0.1.0/oplangchain/callbacks/stdout.py
+-rw-r--r--   0        0        0     2436 2023-08-07 14:51:51.145474 oplangchain-0.1.0/oplangchain/callbacks/streaming_aiter.py
+-rw-r--r--   0        0        0     3364 2023-08-07 14:51:51.145474 oplangchain-0.1.0/oplangchain/callbacks/streaming_aiter_final_only.py
+-rw-r--r--   0        0        0     2170 2023-08-07 14:51:51.146474 oplangchain-0.1.0/oplangchain/callbacks/streaming_stdout.py
+-rw-r--r--   0        0        0     3368 2023-08-07 14:51:51.147474 oplangchain-0.1.0/oplangchain/callbacks/streaming_stdout_final_only.py
+-rw-r--r--   0        0        0     3190 2023-08-07 14:51:51.147474 oplangchain-0.1.0/oplangchain/callbacks/streamlit/__init__.py
+-rw-r--r--   0        0        0     5435 2023-08-07 14:51:51.148474 oplangchain-0.1.0/oplangchain/callbacks/streamlit/mutable_expander.py
+-rw-r--r--   0        0        0    15671 2023-08-07 14:51:51.149474 oplangchain-0.1.0/oplangchain/callbacks/streamlit/streamlit_callback_handler.py
+-rw-r--r--   0        0        0      502 2023-08-07 14:51:51.150474 oplangchain-0.1.0/oplangchain/callbacks/tracers/__init__.py
+-rw-r--r--   0        0        0    17018 2023-08-07 14:51:51.150474 oplangchain-0.1.0/oplangchain/callbacks/tracers/base.py
+-rw-r--r--   0        0        0     4858 2023-08-07 14:51:51.151474 oplangchain-0.1.0/oplangchain/callbacks/tracers/evaluation.py
+-rw-r--r--   0        0        0     8055 2023-08-07 14:51:51.151474 oplangchain-0.1.0/oplangchain/callbacks/tracers/langchain.py
+-rw-r--r--   0        0        0     7362 2023-08-07 14:51:51.152474 oplangchain-0.1.0/oplangchain/callbacks/tracers/langchain_v1.py
+-rw-r--r--   0        0        0     1537 2023-08-07 14:51:51.152474 oplangchain-0.1.0/oplangchain/callbacks/tracers/run_collector.py
+-rw-r--r--   0        0        0     3456 2023-08-07 14:51:51.152474 oplangchain-0.1.0/oplangchain/callbacks/tracers/schemas.py
+-rw-r--r--   0        0        0     6027 2023-08-07 14:51:51.153474 oplangchain-0.1.0/oplangchain/callbacks/tracers/stdout.py
+-rw-r--r--   0        0        0    18983 2023-08-07 14:51:51.153474 oplangchain-0.1.0/oplangchain/callbacks/tracers/wandb.py
+-rw-r--r--   0        0        0     8505 2023-08-07 14:51:51.154474 oplangchain-0.1.0/oplangchain/callbacks/utils.py
+-rw-r--r--   0        0        0    20659 2023-08-07 14:51:51.154474 oplangchain-0.1.0/oplangchain/callbacks/wandb_callback.py
+-rw-r--r--   0        0        0     8062 2023-08-07 14:51:51.155475 oplangchain-0.1.0/oplangchain/callbacks/whylabs_callback.py
+-rw-r--r--   0        0        0     5294 2023-08-07 14:51:51.156475 oplangchain-0.1.0/oplangchain/chains/__init__.py
+-rw-r--r--   0        0        0       84 2023-08-07 14:51:51.157475 oplangchain-0.1.0/oplangchain/chains/api/__init__.py
+-rw-r--r--   0        0        0     5334 2023-08-07 14:51:51.158475 oplangchain-0.1.0/oplangchain/chains/api/base.py
+-rw-r--r--   0        0        0     2452 2023-08-07 14:51:51.159474 oplangchain-0.1.0/oplangchain/chains/api/news_docs.py
+-rw-r--r--   0        0        0     3399 2023-08-07 14:51:51.159474 oplangchain-0.1.0/oplangchain/chains/api/open_meteo_docs.py
+-rw-r--r--   0        0        0        0 2023-08-07 14:51:51.160475 oplangchain-0.1.0/oplangchain/chains/api/openapi/__init__.py
+-rw-r--r--   0        0        0     8750 2023-08-07 14:51:51.161475 oplangchain-0.1.0/oplangchain/chains/api/openapi/chain.py
+-rw-r--r--   0        0        0     1791 2023-08-07 14:51:51.161475 oplangchain-0.1.0/oplangchain/chains/api/openapi/prompts.py
+-rw-r--r--   0        0        0     1877 2023-08-07 14:51:51.162474 oplangchain-0.1.0/oplangchain/chains/api/openapi/requests_chain.py
+-rw-r--r--   0        0        0     1749 2023-08-07 14:51:51.162474 oplangchain-0.1.0/oplangchain/chains/api/openapi/response_chain.py
+-rw-r--r--   0        0        0     1920 2023-08-07 14:51:51.163474 oplangchain-0.1.0/oplangchain/chains/api/podcast_docs.py
+-rw-r--r--   0        0        0     1026 2023-08-07 14:51:51.163474 oplangchain-0.1.0/oplangchain/chains/api/prompt.py
+-rw-r--r--   0        0        0     1537 2023-08-07 14:51:51.164475 oplangchain-0.1.0/oplangchain/chains/api/tmdb_docs.py
+-rw-r--r--   0        0        0    24814 2023-08-07 14:51:51.164475 oplangchain-0.1.0/oplangchain/chains/base.py
+-rw-r--r--   0        0        0        0 2023-08-07 14:51:51.165475 oplangchain-0.1.0/oplangchain/chains/chat_vector_db/__init__.py
+-rw-r--r--   0        0        0      689 2023-08-07 14:51:51.165475 oplangchain-0.1.0/oplangchain/chains/chat_vector_db/prompts.py
+-rw-r--r--   0        0        0       43 2023-08-07 14:51:51.166474 oplangchain-0.1.0/oplangchain/chains/combine_documents/__init__.py
+-rw-r--r--   0        0        0     6390 2023-08-07 14:51:51.167474 oplangchain-0.1.0/oplangchain/chains/combine_documents/base.py
+-rw-r--r--   0        0        0    11149 2023-08-07 14:51:51.167474 oplangchain-0.1.0/oplangchain/chains/combine_documents/map_reduce.py
+-rw-r--r--   0        0        0     8368 2023-08-07 14:51:51.168475 oplangchain-0.1.0/oplangchain/chains/combine_documents/map_rerank.py
+-rw-r--r--   0        0        0    11004 2023-08-07 14:51:51.168475 oplangchain-0.1.0/oplangchain/chains/combine_documents/reduce.py
+-rw-r--r--   0        0        0     9075 2023-08-07 14:51:51.169474 oplangchain-0.1.0/oplangchain/chains/combine_documents/refine.py
+-rw-r--r--   0        0        0     7658 2023-08-07 14:51:51.169474 oplangchain-0.1.0/oplangchain/chains/combine_documents/stuff.py
+-rw-r--r--   0        0        0      107 2023-08-07 14:51:51.170474 oplangchain-0.1.0/oplangchain/chains/constitutional_ai/__init__.py
+-rw-r--r--   0        0        0     6328 2023-08-07 14:51:51.170474 oplangchain-0.1.0/oplangchain/chains/constitutional_ai/base.py
+-rw-r--r--   0        0        0      265 2023-08-07 14:51:51.171474 oplangchain-0.1.0/oplangchain/chains/constitutional_ai/models.py
+-rw-r--r--   0        0        0    21738 2023-08-07 14:51:51.171474 oplangchain-0.1.0/oplangchain/chains/constitutional_ai/principles.py
+-rw-r--r--   0        0        0     8656 2023-08-07 14:51:51.172475 oplangchain-0.1.0/oplangchain/chains/constitutional_ai/prompts.py
+-rw-r--r--   0        0        0       71 2023-08-07 14:51:51.173476 oplangchain-0.1.0/oplangchain/chains/conversation/__init__.py
+-rw-r--r--   0        0        0     2174 2023-08-07 14:51:51.173476 oplangchain-0.1.0/oplangchain/chains/conversation/base.py
+-rw-r--r--   0        0        0      856 2023-08-07 14:51:51.174476 oplangchain-0.1.0/oplangchain/chains/conversation/memory.py
+-rw-r--r--   0        0        0      908 2023-08-07 14:51:51.174476 oplangchain-0.1.0/oplangchain/chains/conversation/prompt.py
+-rw-r--r--   0        0        0       49 2023-08-07 14:51:51.175475 oplangchain-0.1.0/oplangchain/chains/conversational_retrieval/__init__.py
+-rw-r--r--   0        0        0    16705 2023-08-07 14:51:51.176476 oplangchain-0.1.0/oplangchain/chains/conversational_retrieval/base.py
+-rw-r--r--   0        0        0      715 2023-08-07 14:51:51.176476 oplangchain-0.1.0/oplangchain/chains/conversational_retrieval/prompts.py
+-rw-r--r--   0        0        0      126 2023-08-07 14:51:51.177475 oplangchain-0.1.0/oplangchain/chains/elasticsearch_database/__init__.py
+-rw-r--r--   0        0        0     8166 2023-08-07 14:51:51.177475 oplangchain-0.1.0/oplangchain/chains/elasticsearch_database/base.py
+-rw-r--r--   0        0        0     1420 2023-08-07 14:51:51.178474 oplangchain-0.1.0/oplangchain/chains/elasticsearch_database/prompts.py
+-rw-r--r--   0        0        0      731 2023-08-07 14:51:51.178474 oplangchain-0.1.0/oplangchain/chains/example_generator.py
+-rw-r--r--   0        0        0       51 2023-08-07 14:51:51.179474 oplangchain-0.1.0/oplangchain/chains/flare/__init__.py
+-rw-r--r--   0        0        0     8765 2023-08-07 14:51:51.180476 oplangchain-0.1.0/oplangchain/chains/flare/base.py
+-rw-r--r--   0        0        0     1453 2023-08-07 14:51:51.180476 oplangchain-0.1.0/oplangchain/chains/flare/prompts.py
+-rw-r--r--   0        0        0       49 2023-08-07 14:51:51.181476 oplangchain-0.1.0/oplangchain/chains/graph_qa/__init__.py
+-rw-r--r--   0        0        0     7676 2023-08-07 14:51:51.182475 oplangchain-0.1.0/oplangchain/chains/graph_qa/arangodb.py
+-rw-r--r--   0        0        0     2970 2023-08-07 14:51:51.182475 oplangchain-0.1.0/oplangchain/chains/graph_qa/base.py
+-rw-r--r--   0        0        0     4586 2023-08-07 14:51:51.183475 oplangchain-0.1.0/oplangchain/chains/graph_qa/cypher.py
+-rw-r--r--   0        0        0     3019 2023-08-07 14:51:51.183475 oplangchain-0.1.0/oplangchain/chains/graph_qa/hugegraph.py
+-rw-r--r--   0        0        0     3019 2023-08-07 14:51:51.184473 oplangchain-0.1.0/oplangchain/chains/graph_qa/kuzu.py
+-rw-r--r--   0        0        0     2994 2023-08-07 14:51:51.184473 oplangchain-0.1.0/oplangchain/chains/graph_qa/nebulagraph.py
+-rw-r--r--   0        0        0     4479 2023-08-07 14:51:51.185474 oplangchain-0.1.0/oplangchain/chains/graph_qa/neptune_cypher.py
+-rw-r--r--   0        0        0    13728 2023-08-07 14:51:51.185474 oplangchain-0.1.0/oplangchain/chains/graph_qa/prompts.py
+-rw-r--r--   0        0        0     4771 2023-08-07 14:51:51.186474 oplangchain-0.1.0/oplangchain/chains/graph_qa/sparql.py
+-rw-r--r--   0        0        0       75 2023-08-07 14:51:51.187475 oplangchain-0.1.0/oplangchain/chains/hyde/__init__.py
+-rw-r--r--   0        0        0     2831 2023-08-07 14:51:51.187475 oplangchain-0.1.0/oplangchain/chains/hyde/base.py
+-rw-r--r--   0        0        0     1908 2023-08-07 14:51:51.188474 oplangchain-0.1.0/oplangchain/chains/hyde/prompts.py
+-rw-r--r--   0        0        0    12141 2023-08-07 14:51:51.188474 oplangchain-0.1.0/oplangchain/chains/llm.py
+-rw-r--r--   0        0        0       88 2023-08-07 14:51:51.189475 oplangchain-0.1.0/oplangchain/chains/llm_bash/__init__.py
+-rw-r--r--   0        0        0     4165 2023-08-07 14:51:51.190475 oplangchain-0.1.0/oplangchain/chains/llm_bash/base.py
+-rw-r--r--   0        0        0     1937 2023-08-07 14:51:51.191475 oplangchain-0.1.0/oplangchain/chains/llm_bash/prompt.py
+-rw-r--r--   0        0        0      139 2023-08-07 14:51:51.191475 oplangchain-0.1.0/oplangchain/chains/llm_checker/__init__.py
+-rw-r--r--   0        0        0     6090 2023-08-07 14:51:51.192474 oplangchain-0.1.0/oplangchain/chains/llm_checker/base.py
+-rw-r--r--   0        0        0     1120 2023-08-07 14:51:51.192474 oplangchain-0.1.0/oplangchain/chains/llm_checker/prompt.py
+-rw-r--r--   0        0        0      143 2023-08-07 14:51:51.193472 oplangchain-0.1.0/oplangchain/chains/llm_math/__init__.py
+-rw-r--r--   0        0        0     6372 2023-08-07 14:51:51.194476 oplangchain-0.1.0/oplangchain/chains/llm_math/base.py
+-rw-r--r--   0        0        0      863 2023-08-07 14:51:51.194476 oplangchain-0.1.0/oplangchain/chains/llm_math/prompt.py
+-rw-r--r--   0        0        0     2877 2023-08-07 14:51:51.195474 oplangchain-0.1.0/oplangchain/chains/llm_requests.py
+-rw-r--r--   0        0        0      352 2023-08-07 14:51:51.196474 oplangchain-0.1.0/oplangchain/chains/llm_summarization_checker/__init__.py
+-rw-r--r--   0        0        0     6606 2023-08-07 14:51:51.196474 oplangchain-0.1.0/oplangchain/chains/llm_summarization_checker/base.py
+-rw-r--r--   0        0        0      654 2023-08-07 14:51:51.241473 oplangchain-0.1.0/oplangchain/chains/llm_summarization_checker/prompts/are_all_true_prompt.txt
+-rw-r--r--   0        0        0      377 2023-08-07 14:51:51.242473 oplangchain-0.1.0/oplangchain/chains/llm_summarization_checker/prompts/check_facts.txt
+-rw-r--r--   0        0        0      128 2023-08-07 14:51:51.244473 oplangchain-0.1.0/oplangchain/chains/llm_summarization_checker/prompts/create_facts.txt
+-rw-r--r--   0        0        0      416 2023-08-07 14:51:51.245474 oplangchain-0.1.0/oplangchain/chains/llm_summarization_checker/prompts/revise_summary.txt
+-rw-r--r--   0        0        0      126 2023-08-07 14:51:51.245474 oplangchain-0.1.0/oplangchain/chains/llm_symbolic_math/__init__.py
+-rw-r--r--   0        0        0     5555 2023-08-07 14:51:51.246475 oplangchain-0.1.0/oplangchain/chains/llm_symbolic_math/base.py
+-rw-r--r--   0        0        0     1087 2023-08-07 14:51:51.246475 oplangchain-0.1.0/oplangchain/chains/llm_symbolic_math/prompt.py
+-rw-r--r--   0        0        0    23945 2023-08-07 14:51:51.277473 oplangchain-0.1.0/oplangchain/chains/loading.py
+-rw-r--r--   0        0        0     3715 2023-08-07 14:51:51.278475 oplangchain-0.1.0/oplangchain/chains/mapreduce.py
+-rw-r--r--   0        0        0     3050 2023-08-07 14:51:51.279473 oplangchain-0.1.0/oplangchain/chains/moderation.py
+-rw-r--r--   0        0        0       96 2023-08-07 14:51:51.279473 oplangchain-0.1.0/oplangchain/chains/natbot/__init__.py
+-rw-r--r--   0        0        0     4179 2023-08-07 14:51:51.280474 oplangchain-0.1.0/oplangchain/chains/natbot/base.py
+-rw-r--r--   0        0        0    15466 2023-08-07 14:51:51.280474 oplangchain-0.1.0/oplangchain/chains/natbot/crawler.py
+-rw-r--r--   0        0        0     4984 2023-08-07 14:51:51.281475 oplangchain-0.1.0/oplangchain/chains/natbot/prompt.py
+-rw-r--r--   0        0        0      948 2023-08-07 14:51:51.310473 oplangchain-0.1.0/oplangchain/chains/openai_functions/__init__.py
+-rw-r--r--   0        0        0    14608 2023-08-07 14:51:51.311474 oplangchain-0.1.0/oplangchain/chains/openai_functions/base.py
+-rw-r--r--   0        0        0     3506 2023-08-07 14:51:51.312483 oplangchain-0.1.0/oplangchain/chains/openai_functions/citation_fuzzy_match.py
+-rw-r--r--   0        0        0     3338 2023-08-07 14:51:51.343475 oplangchain-0.1.0/oplangchain/chains/openai_functions/extraction.py
+-rw-r--r--   0        0        0    11184 2023-08-07 16:16:46.596551 oplangchain-0.1.0/oplangchain/chains/openai_functions/openapi.py
+-rw-r--r--   0        0        0     3709 2023-08-07 14:51:51.344474 oplangchain-0.1.0/oplangchain/chains/openai_functions/qa_with_structure.py
+-rw-r--r--   0        0        0     2653 2023-08-07 14:51:51.345474 oplangchain-0.1.0/oplangchain/chains/openai_functions/tagging.py
+-rw-r--r--   0        0        0     1257 2023-08-07 14:51:51.345474 oplangchain-0.1.0/oplangchain/chains/openai_functions/utils.py
+-rw-r--r--   0        0        0     1961 2023-08-07 14:51:51.346475 oplangchain-0.1.0/oplangchain/chains/prompt_selector.py
+-rw-r--r--   0        0        0        0 2023-08-07 14:51:51.346475 oplangchain-0.1.0/oplangchain/chains/qa_generation/__init__.py
+-rw-r--r--   0        0        0     2444 2023-08-07 14:51:51.347474 oplangchain-0.1.0/oplangchain/chains/qa_generation/base.py
+-rw-r--r--   0        0        0     1865 2023-08-07 14:51:51.347474 oplangchain-0.1.0/oplangchain/chains/qa_generation/prompt.py
+-rw-r--r--   0        0        0      173 2023-08-07 14:51:51.348474 oplangchain-0.1.0/oplangchain/chains/qa_with_sources/__init__.py
+-rw-r--r--   0        0        0     7717 2023-08-07 14:51:51.348474 oplangchain-0.1.0/oplangchain/chains/qa_with_sources/base.py
+-rw-r--r--   0        0        0     6803 2023-08-07 14:51:51.349474 oplangchain-0.1.0/oplangchain/chains/qa_with_sources/loading.py
+-rw-r--r--   0        0        0     6966 2023-08-07 14:51:51.350474 oplangchain-0.1.0/oplangchain/chains/qa_with_sources/map_reduce_prompt.py
+-rw-r--r--   0        0        0     1313 2023-08-07 14:51:51.377473 oplangchain-0.1.0/oplangchain/chains/qa_with_sources/refine_prompts.py
+-rw-r--r--   0        0        0     2344 2023-08-07 14:51:51.378473 oplangchain-0.1.0/oplangchain/chains/qa_with_sources/retrieval.py
+-rw-r--r--   0        0        0     6576 2023-08-07 14:51:51.378473 oplangchain-0.1.0/oplangchain/chains/qa_with_sources/stuff_prompt.py
+-rw-r--r--   0        0        0     2799 2023-08-07 14:51:51.378473 oplangchain-0.1.0/oplangchain/chains/qa_with_sources/vector_db.py
+-rw-r--r--   0        0        0        0 2023-08-07 14:51:51.379473 oplangchain-0.1.0/oplangchain/chains/query_constructor/__init__.py
+-rw-r--r--   0        0        0     5808 2023-08-07 14:51:51.380475 oplangchain-0.1.0/oplangchain/chains/query_constructor/base.py
+-rw-r--r--   0        0        0     3129 2023-08-07 14:51:51.380475 oplangchain-0.1.0/oplangchain/chains/query_constructor/ir.py
+-rw-r--r--   0        0        0     4752 2023-08-07 14:51:51.381474 oplangchain-0.1.0/oplangchain/chains/query_constructor/parser.py
+-rw-r--r--   0        0        0     6446 2023-08-07 14:51:51.381474 oplangchain-0.1.0/oplangchain/chains/query_constructor/prompt.py
+-rw-r--r--   0        0        0      303 2023-08-07 14:51:51.383473 oplangchain-0.1.0/oplangchain/chains/query_constructor/schema.py
+-rw-r--r--   0        0        0     8552 2023-08-07 14:51:51.384474 oplangchain-0.1.0/oplangchain/chains/question_answering/__init__.py
+-rw-r--r--   0        0        0     8003 2023-08-07 14:51:51.384474 oplangchain-0.1.0/oplangchain/chains/question_answering/map_reduce_prompt.py
+-rw-r--r--   0        0        0     1617 2023-08-07 14:51:51.416474 oplangchain-0.1.0/oplangchain/chains/question_answering/map_rerank_prompt.py
+-rw-r--r--   0        0        0     2726 2023-08-07 14:51:51.417476 oplangchain-0.1.0/oplangchain/chains/question_answering/refine_prompts.py
+-rw-r--r--   0        0        0     1135 2023-08-07 14:51:51.417476 oplangchain-0.1.0/oplangchain/chains/question_answering/stuff_prompt.py
+-rw-r--r--   0        0        0       62 2023-08-07 14:51:51.418473 oplangchain-0.1.0/oplangchain/chains/retrieval_qa/__init__.py
+-rw-r--r--   0        0        0     9762 2023-08-07 14:51:51.419475 oplangchain-0.1.0/oplangchain/chains/retrieval_qa/base.py
+-rw-r--r--   0        0        0      394 2023-08-07 14:51:51.419475 oplangchain-0.1.0/oplangchain/chains/retrieval_qa/prompt.py
+-rw-r--r--   0        0        0      407 2023-08-07 14:51:51.420474 oplangchain-0.1.0/oplangchain/chains/router/__init__.py
+-rw-r--r--   0        0        0     4556 2023-08-07 14:51:51.420474 oplangchain-0.1.0/oplangchain/chains/router/base.py
+-rw-r--r--   0        0        0     1970 2023-08-07 14:51:51.421474 oplangchain-0.1.0/oplangchain/chains/router/embedding_router.py
+-rw-r--r--   0        0        0     4185 2023-08-07 14:51:51.421474 oplangchain-0.1.0/oplangchain/chains/router/llm_router.py
+-rw-r--r--   0        0        0     2562 2023-08-07 14:51:51.447474 oplangchain-0.1.0/oplangchain/chains/router/multi_prompt.py
+-rw-r--r--   0        0        0     1123 2023-08-07 14:51:51.448481 oplangchain-0.1.0/oplangchain/chains/router/multi_prompt_prompt.py
+-rw-r--r--   0        0        0     1079 2023-08-07 14:51:51.449476 oplangchain-0.1.0/oplangchain/chains/router/multi_retrieval_prompt.py
+-rw-r--r--   0        0        0     3635 2023-08-07 14:51:51.449476 oplangchain-0.1.0/oplangchain/chains/router/multi_retrieval_qa.py
+-rw-r--r--   0        0        0     7481 2023-08-07 14:51:51.450475 oplangchain-0.1.0/oplangchain/chains/sequential.py
+-rw-r--r--   0        0        0       47 2023-08-07 14:51:51.450475 oplangchain-0.1.0/oplangchain/chains/sql_database/__init__.py
+-rw-r--r--   0        0        0    14202 2023-08-07 14:51:51.451476 oplangchain-0.1.0/oplangchain/chains/sql_database/prompt.py
+-rw-r--r--   0        0        0     2066 2023-08-07 14:51:51.451476 oplangchain-0.1.0/oplangchain/chains/sql_database/query.py
+-rw-r--r--   0        0        0     5695 2023-08-07 14:51:51.480846 oplangchain-0.1.0/oplangchain/chains/summarize/__init__.py
+-rw-r--r--   0        0        0      233 2023-08-07 14:51:51.481847 oplangchain-0.1.0/oplangchain/chains/summarize/map_reduce_prompt.py
+-rw-r--r--   0        0        0      805 2023-08-07 14:51:51.481847 oplangchain-0.1.0/oplangchain/chains/summarize/refine_prompts.py
+-rw-r--r--   0        0        0      233 2023-08-07 14:51:51.513090 oplangchain-0.1.0/oplangchain/chains/summarize/stuff_prompt.py
+-rw-r--r--   0        0        0     2233 2023-08-07 14:51:51.513090 oplangchain-0.1.0/oplangchain/chains/transform.py
+-rw-r--r--   0        0        0     1354 2023-08-07 14:51:51.514100 oplangchain-0.1.0/oplangchain/chat_models/__init__.py
+-rw-r--r--   0        0        0     6988 2023-08-07 14:51:51.515099 oplangchain-0.1.0/oplangchain/chat_models/anthropic.py
+-rw-r--r--   0        0        0     4707 2023-08-07 14:51:51.515099 oplangchain-0.1.0/oplangchain/chat_models/azure_openai.py
+-rw-r--r--   0        0        0     5396 2023-08-07 14:51:51.518098 oplangchain-0.1.0/oplangchain/chat_models/azureml_endpoint.py
+-rw-r--r--   0        0        0    23270 2023-08-07 14:51:51.519100 oplangchain-0.1.0/oplangchain/chat_models/base.py
+-rw-r--r--   0        0        0     1040 2023-08-07 14:51:51.519100 oplangchain-0.1.0/oplangchain/chat_models/fake.py
+-rw-r--r--   0        0        0    11127 2023-08-07 14:51:51.520100 oplangchain-0.1.0/oplangchain/chat_models/google_palm.py
+-rw-r--r--   0        0        0     4017 2023-08-07 14:51:51.520100 oplangchain-0.1.0/oplangchain/chat_models/human.py
+-rw-r--r--   0        0        0    15223 2023-08-07 14:51:51.521099 oplangchain-0.1.0/oplangchain/chat_models/jinachat.py
+-rw-r--r--   0        0        0     6855 2023-08-07 14:51:51.521099 oplangchain-0.1.0/oplangchain/chat_models/mlflow_ai_gateway.py
+-rw-r--r--   0        0        0    22364 2023-08-07 14:51:51.522100 oplangchain-0.1.0/oplangchain/chat_models/openai.py
+-rw-r--r--   0        0        0     5164 2023-08-07 14:51:51.522100 oplangchain-0.1.0/oplangchain/chat_models/promptlayer_openai.py
+-rw-r--r--   0        0        0     6006 2023-08-07 14:51:51.523098 oplangchain-0.1.0/oplangchain/chat_models/vertexai.py
+-rw-r--r--   0        0        0      685 2023-08-07 14:51:51.523098 oplangchain-0.1.0/oplangchain/docker-compose.yaml
+-rw-r--r--   0        0        0      519 2023-08-07 14:51:51.524099 oplangchain-0.1.0/oplangchain/docstore/__init__.py
+-rw-r--r--   0        0        0     1071 2023-08-07 14:51:51.524099 oplangchain-0.1.0/oplangchain/docstore/arbitrary_fn.py
+-rw-r--r--   0        0        0      836 2023-08-07 14:51:51.525100 oplangchain-0.1.0/oplangchain/docstore/base.py
+-rw-r--r--   0        0        0       62 2023-08-07 14:51:51.525100 oplangchain-0.1.0/oplangchain/docstore/document.py
+-rw-r--r--   0        0        0     1602 2023-08-07 14:51:51.550662 oplangchain-0.1.0/oplangchain/docstore/in_memory.py
+-rw-r--r--   0        0        0     1479 2023-08-07 14:51:51.551661 oplangchain-0.1.0/oplangchain/docstore/wikipedia.py
+-rw-r--r--   0        0        0    12884 2023-08-07 14:51:51.552662 oplangchain-0.1.0/oplangchain/document_loaders/__init__.py
+-rw-r--r--   0        0        0     2847 2023-08-07 14:51:51.552662 oplangchain-0.1.0/oplangchain/document_loaders/acreom.py
+-rw-r--r--   0        0        0      839 2023-08-07 14:51:51.553664 oplangchain-0.1.0/oplangchain/document_loaders/airbyte_json.py
+-rw-r--r--   0        0        0     1273 2023-08-07 14:51:51.553664 oplangchain-0.1.0/oplangchain/document_loaders/airtable.py
+-rw-r--r--   0        0        0     2716 2023-08-07 14:51:51.582945 oplangchain-0.1.0/oplangchain/document_loaders/apify_dataset.py
+-rw-r--r--   0        0        0     1138 2023-08-07 14:51:51.582945 oplangchain-0.1.0/oplangchain/document_loaders/arxiv.py
+-rw-r--r--   0        0        0     4861 2023-08-07 14:51:51.583960 oplangchain-0.1.0/oplangchain/document_loaders/async_html.py
+-rw-r--r--   0        0        0      576 2023-08-07 14:51:51.583960 oplangchain-0.1.0/oplangchain/document_loaders/azlyrics.py
+-rw-r--r--   0        0        0     1612 2023-08-07 14:51:51.584953 oplangchain-0.1.0/oplangchain/document_loaders/azure_blob_storage_container.py
+-rw-r--r--   0        0        0     1631 2023-08-07 14:51:51.584953 oplangchain-0.1.0/oplangchain/document_loaders/azure_blob_storage_file.py
+-rw-r--r--   0        0        0     3041 2023-08-07 14:51:51.585951 oplangchain-0.1.0/oplangchain/document_loaders/base.py
+-rw-r--r--   0        0        0     3928 2023-08-07 14:51:51.585951 oplangchain-0.1.0/oplangchain/document_loaders/bibtex.py
+-rw-r--r--   0        0        0     3147 2023-08-07 14:51:51.586951 oplangchain-0.1.0/oplangchain/document_loaders/bigquery.py
+-rw-r--r--   0        0        0     2722 2023-08-07 14:51:51.586951 oplangchain-0.1.0/oplangchain/document_loaders/bilibili.py
+-rw-r--r--   0        0        0    10089 2023-08-07 14:51:51.587951 oplangchain-0.1.0/oplangchain/document_loaders/blackboard.py
+-rw-r--r--   0        0        0      326 2023-08-07 14:51:51.587951 oplangchain-0.1.0/oplangchain/document_loaders/blob_loaders/__init__.py
+-rw-r--r--   0        0        0     4279 2023-08-07 14:51:51.588952 oplangchain-0.1.0/oplangchain/document_loaders/blob_loaders/file_system.py
+-rw-r--r--   0        0        0     5765 2023-08-07 14:51:51.588952 oplangchain-0.1.0/oplangchain/document_loaders/blob_loaders/schema.py
+-rw-r--r--   0        0        0     1506 2023-08-07 14:51:51.615001 oplangchain-0.1.0/oplangchain/document_loaders/blob_loaders/youtube_audio.py
+-rw-r--r--   0        0        0     5728 2023-08-07 14:51:51.615001 oplangchain-0.1.0/oplangchain/document_loaders/blockchain.py
+-rw-r--r--   0        0        0     1068 2023-08-07 14:51:51.616031 oplangchain-0.1.0/oplangchain/document_loaders/brave_search.py
+-rw-r--r--   0        0        0     2132 2023-08-07 14:51:51.616031 oplangchain-0.1.0/oplangchain/document_loaders/browserless.py
+-rw-r--r--   0        0        0     2026 2023-08-07 14:51:51.617013 oplangchain-0.1.0/oplangchain/document_loaders/chatgpt.py
+-rw-r--r--   0        0        0      552 2023-08-07 14:51:51.617013 oplangchain-0.1.0/oplangchain/document_loaders/college_confidential.py
+-rw-r--r--   0        0        0     2143 2023-08-07 14:51:51.618013 oplangchain-0.1.0/oplangchain/document_loaders/concurrent.py
+-rw-r--r--   0        0        0    25397 2023-08-07 14:51:51.619013 oplangchain-0.1.0/oplangchain/document_loaders/confluence.py
+-rw-r--r--   0        0        0     1068 2023-08-07 14:51:51.646792 oplangchain-0.1.0/oplangchain/document_loaders/conllu.py
+-rw-r--r--   0        0        0     4195 2023-08-07 14:51:51.646792 oplangchain-0.1.0/oplangchain/document_loaders/csv_loader.py
+-rw-r--r--   0        0        0     5901 2023-08-07 14:51:51.647825 oplangchain-0.1.0/oplangchain/document_loaders/cube_semantic.py
+-rw-r--r--   0        0        0     4993 2023-08-07 14:51:51.648805 oplangchain-0.1.0/oplangchain/document_loaders/datadog_logs.py
+-rw-r--r--   0        0        0     1325 2023-08-07 14:51:51.648805 oplangchain-0.1.0/oplangchain/document_loaders/dataframe.py
+-rw-r--r--   0        0        0     2110 2023-08-07 14:51:51.648805 oplangchain-0.1.0/oplangchain/document_loaders/diffbot.py
+-rw-r--r--   0        0        0     5094 2023-08-07 14:51:51.649807 oplangchain-0.1.0/oplangchain/document_loaders/directory.py
+-rw-r--r--   0        0        0     1261 2023-08-07 14:51:51.649807 oplangchain-0.1.0/oplangchain/document_loaders/discord.py
+-rw-r--r--   0        0        0    13216 2023-08-07 14:51:51.650804 oplangchain-0.1.0/oplangchain/document_loaders/docugami.py
+-rw-r--r--   0        0        0     6089 2023-08-07 14:51:51.650804 oplangchain-0.1.0/oplangchain/document_loaders/dropbox.py
+-rw-r--r--   0        0        0     3181 2023-08-07 14:51:51.651804 oplangchain-0.1.0/oplangchain/document_loaders/duckdb_loader.py
+-rw-r--r--   0        0        0     3782 2023-08-07 14:51:51.651804 oplangchain-0.1.0/oplangchain/document_loaders/email.py
+-rw-r--r--   0        0        0     8933 2023-08-07 14:51:51.652806 oplangchain-0.1.0/oplangchain/document_loaders/embaas.py
+-rw-r--r--   0        0        0     1510 2023-08-07 14:51:51.652806 oplangchain-0.1.0/oplangchain/document_loaders/epub.py
+-rw-r--r--   0        0        0     7808 2023-08-07 14:51:51.653805 oplangchain-0.1.0/oplangchain/document_loaders/etherscan.py
+-rw-r--r--   0        0        0     5744 2023-08-07 14:51:51.653805 oplangchain-0.1.0/oplangchain/document_loaders/evernote.py
+-rw-r--r--   0        0        0     1664 2023-08-07 14:51:51.654807 oplangchain-0.1.0/oplangchain/document_loaders/excel.py
+-rw-r--r--   0        0        0     1298 2023-08-07 14:51:51.654807 oplangchain-0.1.0/oplangchain/document_loaders/facebook_chat.py
+-rw-r--r--   0        0        0     2241 2023-08-07 14:51:51.655804 oplangchain-0.1.0/oplangchain/document_loaders/fauna.py
+-rw-r--r--   0        0        0     1569 2023-08-07 14:51:51.655804 oplangchain-0.1.0/oplangchain/document_loaders/figma.py
+-rw-r--r--   0        0        0     1573 2023-08-07 14:51:51.656804 oplangchain-0.1.0/oplangchain/document_loaders/gcs_directory.py
+-rw-r--r--   0        0        0     1731 2023-08-07 14:51:51.656804 oplangchain-0.1.0/oplangchain/document_loaders/gcs_file.py
+-rw-r--r--   0        0        0     4527 2023-08-07 14:51:51.657804 oplangchain-0.1.0/oplangchain/document_loaders/generic.py
+-rw-r--r--   0        0        0     1682 2023-08-07 14:51:51.657804 oplangchain-0.1.0/oplangchain/document_loaders/geodataframe.py
+-rw-r--r--   0        0        0     4138 2023-08-07 14:51:51.657804 oplangchain-0.1.0/oplangchain/document_loaders/git.py
+-rw-r--r--   0        0        0     3106 2023-08-07 14:51:51.658804 oplangchain-0.1.0/oplangchain/document_loaders/gitbook.py
+-rw-r--r--   0        0        0     6868 2023-08-07 14:51:51.658804 oplangchain-0.1.0/oplangchain/document_loaders/github.py
+-rw-r--r--   0        0        0    13926 2023-08-07 14:51:51.659804 oplangchain-0.1.0/oplangchain/document_loaders/googledrive.py
+-rw-r--r--   0        0        0      969 2023-08-07 14:51:51.660541 oplangchain-0.1.0/oplangchain/document_loaders/gutenberg.py
+-rw-r--r--   0        0        0     1559 2023-08-07 14:51:51.660541 oplangchain-0.1.0/oplangchain/document_loaders/helpers.py
+-rw-r--r--   0        0        0     2061 2023-08-07 14:51:51.661555 oplangchain-0.1.0/oplangchain/document_loaders/hn.py
+-rw-r--r--   0        0        0     1204 2023-08-07 14:51:51.661555 oplangchain-0.1.0/oplangchain/document_loaders/html.py
+-rw-r--r--   0        0        0     2118 2023-08-07 14:51:51.661555 oplangchain-0.1.0/oplangchain/document_loaders/html_bs.py
+-rw-r--r--   0        0        0     3025 2023-08-07 14:51:51.662553 oplangchain-0.1.0/oplangchain/document_loaders/hugging_face_dataset.py
+-rw-r--r--   0        0        0     7648 2023-08-07 14:51:51.662553 oplangchain-0.1.0/oplangchain/document_loaders/ifixit.py
+-rw-r--r--   0        0        0     1186 2023-08-07 14:51:51.663554 oplangchain-0.1.0/oplangchain/document_loaders/image.py
+-rw-r--r--   0        0        0     3099 2023-08-07 14:51:51.663554 oplangchain-0.1.0/oplangchain/document_loaders/image_captions.py
+-rw-r--r--   0        0        0      487 2023-08-07 14:51:51.664553 oplangchain-0.1.0/oplangchain/document_loaders/imsdb.py
+-rw-r--r--   0        0        0     1734 2023-08-07 14:51:51.664553 oplangchain-0.1.0/oplangchain/document_loaders/iugu.py
+-rw-r--r--   0        0        0     3699 2023-08-07 14:51:51.665554 oplangchain-0.1.0/oplangchain/document_loaders/joplin.py
+-rw-r--r--   0        0        0     5487 2023-08-07 14:51:51.665554 oplangchain-0.1.0/oplangchain/document_loaders/json_loader.py
+-rw-r--r--   0        0        0     2052 2023-08-07 14:51:51.665554 oplangchain-0.1.0/oplangchain/document_loaders/larksuite.py
+-rw-r--r--   0        0        0     1828 2023-08-07 14:51:51.666553 oplangchain-0.1.0/oplangchain/document_loaders/markdown.py
+-rw-r--r--   0        0        0     3130 2023-08-07 14:51:51.666553 oplangchain-0.1.0/oplangchain/document_loaders/mastodon.py
+-rw-r--r--   0        0        0     3293 2023-08-07 14:51:51.667553 oplangchain-0.1.0/oplangchain/document_loaders/max_compute.py
+-rw-r--r--   0        0        0     3479 2023-08-07 14:51:51.667553 oplangchain-0.1.0/oplangchain/document_loaders/mediawikidump.py
+-rw-r--r--   0        0        0      838 2023-08-07 14:51:51.668553 oplangchain-0.1.0/oplangchain/document_loaders/merge.py
+-rw-r--r--   0        0        0     2600 2023-08-07 14:51:51.668553 oplangchain-0.1.0/oplangchain/document_loaders/mhtml.py
+-rw-r--r--   0        0        0     3131 2023-08-07 14:51:51.669553 oplangchain-0.1.0/oplangchain/document_loaders/modern_treasury.py
+-rw-r--r--   0        0        0     4287 2023-08-07 14:51:51.669553 oplangchain-0.1.0/oplangchain/document_loaders/news.py
+-rw-r--r--   0        0        0     4281 2023-08-07 14:51:51.669553 oplangchain-0.1.0/oplangchain/document_loaders/notebook.py
+-rw-r--r--   0        0        0      741 2023-08-07 14:51:51.670553 oplangchain-0.1.0/oplangchain/document_loaders/notion.py
+-rw-r--r--   0        0        0     5892 2023-08-07 14:51:51.670553 oplangchain-0.1.0/oplangchain/document_loaders/notiondb.py
+-rw-r--r--   0        0        0     1084 2023-08-07 14:51:51.671554 oplangchain-0.1.0/oplangchain/document_loaders/nuclia.py
+-rw-r--r--   0        0        0     3594 2023-08-07 14:51:51.671554 oplangchain-0.1.0/oplangchain/document_loaders/obs_directory.py
+-rw-r--r--   0        0        0     4745 2023-08-07 14:51:51.672555 oplangchain-0.1.0/oplangchain/document_loaders/obs_file.py
+-rw-r--r--   0        0        0     2537 2023-08-07 14:51:51.672555 oplangchain-0.1.0/oplangchain/document_loaders/obsidian.py
+-rw-r--r--   0        0        0     1793 2023-08-07 14:51:51.673554 oplangchain-0.1.0/oplangchain/document_loaders/odt.py
+-rw-r--r--   0        0        0     8635 2023-08-07 14:51:51.673554 oplangchain-0.1.0/oplangchain/document_loaders/onedrive.py
+-rw-r--r--   0        0        0     1108 2023-08-07 14:51:51.674553 oplangchain-0.1.0/oplangchain/document_loaders/onedrive_file.py
+-rw-r--r--   0        0        0     1322 2023-08-07 14:51:51.674553 oplangchain-0.1.0/oplangchain/document_loaders/open_city_data.py
+-rw-r--r--   0        0        0     1765 2023-08-07 14:51:51.675557 oplangchain-0.1.0/oplangchain/document_loaders/org_mode.py
+-rw-r--r--   0        0        0      645 2023-08-07 14:51:51.676554 oplangchain-0.1.0/oplangchain/document_loaders/parsers/__init__.py
+-rw-r--r--   0        0        0     6083 2023-08-07 14:51:51.676554 oplangchain-0.1.0/oplangchain/document_loaders/parsers/audio.py
+-rw-r--r--   0        0        0     2466 2023-08-07 14:51:51.677553 oplangchain-0.1.0/oplangchain/document_loaders/parsers/generic.py
+-rw-r--r--   0        0        0     5759 2023-08-07 14:51:51.677553 oplangchain-0.1.0/oplangchain/document_loaders/parsers/grobid.py
+-rw-r--r--   0        0        0       99 2023-08-07 14:51:51.678553 oplangchain-0.1.0/oplangchain/document_loaders/parsers/html/__init__.py
+-rw-r--r--   0        0        0     1602 2023-08-07 14:51:51.678553 oplangchain-0.1.0/oplangchain/document_loaders/parsers/html/bs4.py
+-rw-r--r--   0        0        0      117 2023-08-07 14:51:51.679553 oplangchain-0.1.0/oplangchain/document_loaders/parsers/language/__init__.py
+-rw-r--r--   0        0        0      499 2023-08-07 14:51:51.679553 oplangchain-0.1.0/oplangchain/document_loaders/parsers/language/code_segmenter.py
+-rw-r--r--   0        0        0     2088 2023-08-07 14:51:51.680556 oplangchain-0.1.0/oplangchain/document_loaders/parsers/language/javascript.py
+-rw-r--r--   0        0        0     4670 2023-08-07 14:51:51.680556 oplangchain-0.1.0/oplangchain/document_loaders/parsers/language/language_parser.py
+-rw-r--r--   0        0        0     1662 2023-08-07 14:51:51.681553 oplangchain-0.1.0/oplangchain/document_loaders/parsers/language/python.py
+-rw-r--r--   0        0        0     8801 2023-08-07 14:51:51.681553 oplangchain-0.1.0/oplangchain/document_loaders/parsers/pdf.py
+-rw-r--r--   0        0        0      912 2023-08-07 14:51:51.682556 oplangchain-0.1.0/oplangchain/document_loaders/parsers/registry.py
+-rw-r--r--   0        0        0      476 2023-08-07 14:51:51.682556 oplangchain-0.1.0/oplangchain/document_loaders/parsers/txt.py
+-rw-r--r--   0        0        0    20543 2023-08-07 14:51:51.683555 oplangchain-0.1.0/oplangchain/document_loaders/pdf.py
+-rw-r--r--   0        0        0     2517 2023-08-07 14:51:51.683555 oplangchain-0.1.0/oplangchain/document_loaders/powerpoint.py
+-rw-r--r--   0        0        0     1412 2023-08-07 14:51:51.684554 oplangchain-0.1.0/oplangchain/document_loaders/psychic.py
+-rw-r--r--   0        0        0     3418 2023-08-07 14:51:51.684554 oplangchain-0.1.0/oplangchain/document_loaders/pyspark_dataframe.py
+-rw-r--r--   0        0        0      525 2023-08-07 14:51:51.684554 oplangchain-0.1.0/oplangchain/document_loaders/python.py
+-rw-r--r--   0        0        0     3526 2023-08-07 14:51:51.685553 oplangchain-0.1.0/oplangchain/document_loaders/readthedocs.py
+-rw-r--r--   0        0        0    12428 2023-08-07 14:51:51.685553 oplangchain-0.1.0/oplangchain/document_loaders/recursive_url_loader.py
+-rw-r--r--   0        0        0     4605 2023-08-07 14:51:51.686554 oplangchain-0.1.0/oplangchain/document_loaders/reddit.py
+-rw-r--r--   0        0        0      722 2023-08-07 14:51:51.686554 oplangchain-0.1.0/oplangchain/document_loaders/roam.py
+-rw-r--r--   0        0        0     4433 2023-08-07 14:51:51.687553 oplangchain-0.1.0/oplangchain/document_loaders/rocksetdb.py
+-rw-r--r--   0        0        0     4930 2023-08-07 14:51:51.687553 oplangchain-0.1.0/oplangchain/document_loaders/rss.py
+-rw-r--r--   0        0        0     1821 2023-08-07 14:51:51.688553 oplangchain-0.1.0/oplangchain/document_loaders/rst.py
+-rw-r--r--   0        0        0     2050 2023-08-07 14:51:51.688553 oplangchain-0.1.0/oplangchain/document_loaders/rtf.py
+-rw-r--r--   0        0        0     1225 2023-08-07 14:51:51.689554 oplangchain-0.1.0/oplangchain/document_loaders/s3_directory.py
+-rw-r--r--   0        0        0     1316 2023-08-07 14:51:51.689554 oplangchain-0.1.0/oplangchain/document_loaders/s3_file.py
+-rw-r--r--   0        0        0     5008 2023-08-07 14:51:51.690554 oplangchain-0.1.0/oplangchain/document_loaders/sitemap.py
+-rw-r--r--   0        0        0     4180 2023-08-07 14:51:51.690554 oplangchain-0.1.0/oplangchain/document_loaders/slack_directory.py
+-rw-r--r--   0        0        0     4826 2023-08-07 14:51:51.691555 oplangchain-0.1.0/oplangchain/document_loaders/snowflake_loader.py
+-rw-r--r--   0        0        0     2059 2023-08-07 14:51:51.691555 oplangchain-0.1.0/oplangchain/document_loaders/spreedly.py
+-rw-r--r--   0        0        0      887 2023-08-07 14:51:51.692555 oplangchain-0.1.0/oplangchain/document_loaders/srt.py
+-rw-r--r--   0        0        0     1855 2023-08-07 14:51:51.692555 oplangchain-0.1.0/oplangchain/document_loaders/stripe.py
+-rw-r--r--   0        0        0     9041 2023-08-07 14:51:51.693553 oplangchain-0.1.0/oplangchain/document_loaders/telegram.py
+-rw-r--r--   0        0        0     1840 2023-08-07 14:51:51.693553 oplangchain-0.1.0/oplangchain/document_loaders/tencent_cos_directory.py
+-rw-r--r--   0        0        0     1752 2023-08-07 14:51:51.694554 oplangchain-0.1.0/oplangchain/document_loaders/tencent_cos_file.py
+-rw-r--r--   0        0        0     1993 2023-08-07 14:51:51.694554 oplangchain-0.1.0/oplangchain/document_loaders/text.py
+-rw-r--r--   0        0        0      994 2023-08-07 14:51:51.695553 oplangchain-0.1.0/oplangchain/document_loaders/tomarkdown.py
+-rw-r--r--   0        0        0     1649 2023-08-07 14:51:51.695553 oplangchain-0.1.0/oplangchain/document_loaders/toml.py
+-rw-r--r--   0        0        0     6596 2023-08-07 14:51:51.696553 oplangchain-0.1.0/oplangchain/document_loaders/trello.py
+-rw-r--r--   0        0        0     1278 2023-08-07 14:51:51.696553 oplangchain-0.1.0/oplangchain/document_loaders/tsv.py
+-rw-r--r--   0        0        0     3454 2023-08-07 14:51:51.697556 oplangchain-0.1.0/oplangchain/document_loaders/twitter.py
+-rw-r--r--   0        0        0    13877 2023-08-07 14:51:51.697556 oplangchain-0.1.0/oplangchain/document_loaders/unstructured.py
+-rw-r--r--   0        0        0     6011 2023-08-07 14:51:51.698554 oplangchain-0.1.0/oplangchain/document_loaders/url.py
+-rw-r--r--   0        0        0     4947 2023-08-07 14:51:51.698554 oplangchain-0.1.0/oplangchain/document_loaders/url_playwright.py
+-rw-r--r--   0        0        0     5221 2023-08-07 14:51:51.699553 oplangchain-0.1.0/oplangchain/document_loaders/url_selenium.py
+-rw-r--r--   0        0        0     1633 2023-08-07 14:51:51.699553 oplangchain-0.1.0/oplangchain/document_loaders/weather.py
+-rw-r--r--   0        0        0     8011 2023-08-07 14:51:51.699553 oplangchain-0.1.0/oplangchain/document_loaders/web_base.py
+-rw-r--r--   0        0        0     1761 2023-08-07 14:51:51.700553 oplangchain-0.1.0/oplangchain/document_loaders/whatsapp_chat.py
+-rw-r--r--   0        0        0     2182 2023-08-07 14:51:51.700553 oplangchain-0.1.0/oplangchain/document_loaders/wikipedia.py
+-rw-r--r--   0        0        0     4553 2023-08-07 14:51:51.701553 oplangchain-0.1.0/oplangchain/document_loaders/word_document.py
+-rw-r--r--   0        0        0     1479 2023-08-07 14:51:51.701553 oplangchain-0.1.0/oplangchain/document_loaders/xml.py
+-rw-r--r--   0        0        0     1623 2023-08-07 14:51:51.702554 oplangchain-0.1.0/oplangchain/document_loaders/xorbits.py
+-rw-r--r--   0        0        0    14670 2023-08-07 14:51:51.702554 oplangchain-0.1.0/oplangchain/document_loaders/youtube.py
+-rw-r--r--   0        0        0     1436 2023-08-07 14:51:51.703553 oplangchain-0.1.0/oplangchain/document_transformers/__init__.py
+-rw-r--r--   0        0        0     3446 2023-08-07 14:51:51.704554 oplangchain-0.1.0/oplangchain/document_transformers/doctran_text_extract.py
+-rw-r--r--   0        0        0     2170 2023-08-07 14:51:51.704554 oplangchain-0.1.0/oplangchain/document_transformers/doctran_text_qa.py
+-rw-r--r--   0        0        0     2314 2023-08-07 14:51:51.705558 oplangchain-0.1.0/oplangchain/document_transformers/doctran_text_translate.py
+-rw-r--r--   0        0        0     8078 2023-08-07 14:51:51.705558 oplangchain-0.1.0/oplangchain/document_transformers/embeddings_redundant_filter.py
+-rw-r--r--   0        0        0     1293 2023-08-07 14:51:51.706556 oplangchain-0.1.0/oplangchain/document_transformers/html2text.py
+-rw-r--r--   0        0        0     1374 2023-08-07 14:51:51.706556 oplangchain-0.1.0/oplangchain/document_transformers/long_context_reorder.py
+-rw-r--r--   0        0        0     1469 2023-08-07 14:51:51.707557 oplangchain-0.1.0/oplangchain/document_transformers/nuclia_text_transform.py
+-rw-r--r--   0        0        0     6198 2023-08-07 14:51:51.707557 oplangchain-0.1.0/oplangchain/document_transformers/openai_functions.py
+-rw-r--r--   0        0        0     4604 2023-08-07 14:51:51.708556 oplangchain-0.1.0/oplangchain/embeddings/__init__.py
+-rw-r--r--   0        0        0     9592 2023-08-07 14:51:51.708556 oplangchain-0.1.0/oplangchain/embeddings/aleph_alpha.py
+-rw-r--r--   0        0        0     1631 2023-08-07 14:51:51.709556 oplangchain-0.1.0/oplangchain/embeddings/awa.py
+-rw-r--r--   0        0        0      655 2023-08-07 14:51:51.709556 oplangchain-0.1.0/oplangchain/embeddings/base.py
+-rw-r--r--   0        0        0     5480 2023-08-07 14:51:51.710557 oplangchain-0.1.0/oplangchain/embeddings/bedrock.py
+-rw-r--r--   0        0        0     6547 2023-08-07 14:51:51.710557 oplangchain-0.1.0/oplangchain/embeddings/clarifai.py
+-rw-r--r--   0        0        0     3377 2023-08-07 14:51:51.711555 oplangchain-0.1.0/oplangchain/embeddings/cohere.py
+-rw-r--r--   0        0        0     4882 2023-08-07 14:51:51.711555 oplangchain-0.1.0/oplangchain/embeddings/dashscope.py
+-rw-r--r--   0        0        0     4394 2023-08-07 14:51:51.712552 oplangchain-0.1.0/oplangchain/embeddings/deepinfra.py
+-rw-r--r--   0        0        0     2792 2023-08-07 14:51:51.712552 oplangchain-0.1.0/oplangchain/embeddings/edenai.py
+-rw-r--r--   0        0        0     8376 2023-08-07 14:51:51.713557 oplangchain-0.1.0/oplangchain/embeddings/elasticsearch.py
+-rw-r--r--   0        0        0     4786 2023-08-07 14:51:51.713557 oplangchain-0.1.0/oplangchain/embeddings/embaas.py
+-rw-r--r--   0        0        0     1495 2023-08-07 14:51:51.714556 oplangchain-0.1.0/oplangchain/embeddings/fake.py
+-rw-r--r--   0        0        0     2682 2023-08-07 14:51:51.714556 oplangchain-0.1.0/oplangchain/embeddings/google_palm.py
+-rw-r--r--   0        0        0     1637 2023-08-07 14:51:51.715554 oplangchain-0.1.0/oplangchain/embeddings/gpt4all.py
+-rw-r--r--   0        0        0     6034 2023-08-07 14:51:51.715554 oplangchain-0.1.0/oplangchain/embeddings/huggingface.py
+-rw-r--r--   0        0        0     3680 2023-08-07 14:51:51.716553 oplangchain-0.1.0/oplangchain/embeddings/huggingface_hub.py
+-rw-r--r--   0        0        0     3445 2023-08-07 14:51:51.716553 oplangchain-0.1.0/oplangchain/embeddings/jina.py
+-rw-r--r--   0        0        0     4021 2023-08-07 14:51:51.717553 oplangchain-0.1.0/oplangchain/embeddings/llamacpp.py
+-rw-r--r--   0        0        0    12073 2023-08-07 14:51:51.717553 oplangchain-0.1.0/oplangchain/embeddings/localai.py
+-rw-r--r--   0        0        0     4684 2023-08-07 14:51:51.717553 oplangchain-0.1.0/oplangchain/embeddings/minimax.py
+-rw-r--r--   0        0        0     2240 2023-08-07 14:51:51.718553 oplangchain-0.1.0/oplangchain/embeddings/mlflow_gateway.py
+-rw-r--r--   0        0        0     2357 2023-08-07 14:51:51.718553 oplangchain-0.1.0/oplangchain/embeddings/modelscope_hub.py
+-rw-r--r--   0        0        0     5877 2023-08-07 14:51:51.719553 oplangchain-0.1.0/oplangchain/embeddings/mosaicml.py
+-rw-r--r--   0        0        0     2170 2023-08-07 14:51:51.719553 oplangchain-0.1.0/oplangchain/embeddings/nlpcloud.py
+-rw-r--r--   0        0        0     3398 2023-08-07 14:51:51.720554 oplangchain-0.1.0/oplangchain/embeddings/octoai_embeddings.py
+-rw-r--r--   0        0        0    19937 2023-08-07 14:51:51.720554 oplangchain-0.1.0/oplangchain/embeddings/openai.py
+-rw-r--r--   0        0        0     7102 2023-08-07 14:51:51.721553 oplangchain-0.1.0/oplangchain/embeddings/sagemaker_endpoint.py
+-rw-r--r--   0        0        0     3747 2023-08-07 14:51:51.721553 oplangchain-0.1.0/oplangchain/embeddings/self_hosted.py
+-rw-r--r--   0        0        0     6546 2023-08-07 14:51:51.722557 oplangchain-0.1.0/oplangchain/embeddings/self_hosted_hugging_face.py
+-rw-r--r--   0        0        0      179 2023-08-07 14:51:51.722557 oplangchain-0.1.0/oplangchain/embeddings/sentence_transformer.py
+-rw-r--r--   0        0        0     3726 2023-08-07 14:51:51.722557 oplangchain-0.1.0/oplangchain/embeddings/spacy_embeddings.py
+-rw-r--r--   0        0        0     2386 2023-08-07 14:51:51.723554 oplangchain-0.1.0/oplangchain/embeddings/tensorflow_hub.py
+-rw-r--r--   0        0        0     1875 2023-08-07 14:51:51.723554 oplangchain-0.1.0/oplangchain/embeddings/vertexai.py
+-rw-r--r--   0        0        0     3305 2023-08-07 14:51:51.724554 oplangchain-0.1.0/oplangchain/embeddings/xinference.py
+-rw-r--r--   0        0        0      476 2023-08-07 14:51:51.724554 oplangchain-0.1.0/oplangchain/env.py
+-rw-r--r--   0        0        0     5042 2023-08-07 14:51:51.725558 oplangchain-0.1.0/oplangchain/evaluation/__init__.py
+-rw-r--r--   0        0        0      165 2023-08-07 14:51:51.726553 oplangchain-0.1.0/oplangchain/evaluation/agents/__init__.py
+-rw-r--r--   0        0        0    13153 2023-08-07 14:51:51.727554 oplangchain-0.1.0/oplangchain/evaluation/agents/trajectory_eval_chain.py
+-rw-r--r--   0        0        0     5935 2023-08-07 14:51:51.727554 oplangchain-0.1.0/oplangchain/evaluation/agents/trajectory_eval_prompt.py
+-rw-r--r--   0        0        0     1398 2023-08-07 14:51:51.728554 oplangchain-0.1.0/oplangchain/evaluation/comparison/__init__.py
+-rw-r--r--   0        0        0    15043 2023-08-07 14:51:51.728554 oplangchain-0.1.0/oplangchain/evaluation/comparison/eval_chain.py
+-rw-r--r--   0        0        0     2175 2023-08-07 14:51:51.729554 oplangchain-0.1.0/oplangchain/evaluation/comparison/prompt.py
+-rw-r--r--   0        0        0     1628 2023-08-07 14:51:51.729554 oplangchain-0.1.0/oplangchain/evaluation/criteria/__init__.py
+-rw-r--r--   0        0        0    20294 2023-08-07 14:51:51.730554 oplangchain-0.1.0/oplangchain/evaluation/criteria/eval_chain.py
+-rw-r--r--   0        0        0     1751 2023-08-07 14:51:51.731554 oplangchain-0.1.0/oplangchain/evaluation/criteria/prompt.py
+-rw-r--r--   0        0        0      323 2023-08-07 14:51:51.732554 oplangchain-0.1.0/oplangchain/evaluation/embedding_distance/__init__.py
+-rw-r--r--   0        0        0    15475 2023-08-07 14:51:51.732554 oplangchain-0.1.0/oplangchain/evaluation/embedding_distance/base.py
+-rw-r--r--   0        0        0     5192 2023-08-07 14:51:51.733553 oplangchain-0.1.0/oplangchain/evaluation/loading.py
+-rw-r--r--   0        0        0      344 2023-08-07 14:51:51.733553 oplangchain-0.1.0/oplangchain/evaluation/qa/__init__.py
+-rw-r--r--   0        0        0     9987 2023-08-07 14:51:51.734557 oplangchain-0.1.0/oplangchain/evaluation/qa/eval_chain.py
+-rw-r--r--   0        0        0     3906 2023-08-07 14:51:51.734557 oplangchain-0.1.0/oplangchain/evaluation/qa/eval_prompt.py
+-rw-r--r--   0        0        0      956 2023-08-07 14:51:51.735557 oplangchain-0.1.0/oplangchain/evaluation/qa/generate_chain.py
+-rw-r--r--   0        0        0      601 2023-08-07 14:51:51.735557 oplangchain-0.1.0/oplangchain/evaluation/qa/generate_prompt.py
+-rw-r--r--   0        0        0    16800 2023-08-07 14:51:51.736556 oplangchain-0.1.0/oplangchain/evaluation/schema.py
+-rw-r--r--   0        0        0      285 2023-08-07 14:51:51.736556 oplangchain-0.1.0/oplangchain/evaluation/string_distance/__init__.py
+-rw-r--r--   0        0        0    13996 2023-08-07 14:51:51.737553 oplangchain-0.1.0/oplangchain/evaluation/string_distance/base.py
+-rw-r--r--   0        0        0      141 2023-08-07 14:51:51.737553 oplangchain-0.1.0/oplangchain/example_generator.py
+-rw-r--r--   0        0        0      162 2023-08-07 14:51:51.738557 oplangchain-0.1.0/oplangchain/formatting.py
+-rw-r--r--   0        0        0      751 2023-08-07 14:51:51.739554 oplangchain-0.1.0/oplangchain/graphs/__init__.py
+-rw-r--r--   0        0        0     6198 2023-08-07 14:51:51.739554 oplangchain-0.1.0/oplangchain/graphs/arangodb_graph.py
+-rw-r--r--   0        0        0     1841 2023-08-07 14:51:51.739554 oplangchain-0.1.0/oplangchain/graphs/hugegraph.py
+-rw-r--r--   0        0        0     3559 2023-08-07 14:51:51.740556 oplangchain-0.1.0/oplangchain/graphs/kuzu_graph.py
+-rw-r--r--   0        0        0      713 2023-08-07 14:51:51.740556 oplangchain-0.1.0/oplangchain/graphs/memgraph_graph.py
+-rw-r--r--   0        0        0     7362 2023-08-07 14:51:51.741553 oplangchain-0.1.0/oplangchain/graphs/nebula_graph.py
+-rw-r--r--   0        0        0     3625 2023-08-07 14:51:51.741553 oplangchain-0.1.0/oplangchain/graphs/neo4j_graph.py
+-rw-r--r--   0        0        0     6553 2023-08-07 14:51:51.742553 oplangchain-0.1.0/oplangchain/graphs/neptune_graph.py
+-rw-r--r--   0        0        0     5877 2023-08-07 14:51:51.742553 oplangchain-0.1.0/oplangchain/graphs/networkx_graph.py
+-rw-r--r--   0        0        0     9461 2023-08-07 14:51:51.743553 oplangchain-0.1.0/oplangchain/graphs/rdf_graph.py
+-rw-r--r--   0        0        0      207 2023-08-07 14:51:51.743553 oplangchain-0.1.0/oplangchain/indexes/__init__.py
+-rw-r--r--   0        0        0     1712 2023-08-07 14:51:51.744553 oplangchain-0.1.0/oplangchain/indexes/graph.py
+-rw-r--r--   0        0        0       49 2023-08-07 14:51:51.745553 oplangchain-0.1.0/oplangchain/indexes/prompts/__init__.py
+-rw-r--r--   0        0        0     1947 2023-08-07 14:51:51.745553 oplangchain-0.1.0/oplangchain/indexes/prompts/entity_extraction.py
+-rw-r--r--   0        0        0     1152 2023-08-07 14:51:51.746553 oplangchain-0.1.0/oplangchain/indexes/prompts/entity_summarization.py
+-rw-r--r--   0        0        0     1584 2023-08-07 14:51:51.746553 oplangchain-0.1.0/oplangchain/indexes/prompts/knowledge_triplet_extraction.py
+-rw-r--r--   0        0        0     3048 2023-08-07 14:51:51.747555 oplangchain-0.1.0/oplangchain/indexes/vectorstore.py
+-rw-r--r--   0        0        0      277 2023-08-07 14:51:51.747555 oplangchain-0.1.0/oplangchain/input.py
+-rw-r--r--   0        0        0     6388 2023-08-07 14:51:51.748554 oplangchain-0.1.0/oplangchain/llms/__init__.py
+-rw-r--r--   0        0        0     4996 2023-08-07 14:51:51.749553 oplangchain-0.1.0/oplangchain/llms/ai21.py
+-rw-r--r--   0        0        0    11352 2023-08-07 14:51:51.749553 oplangchain-0.1.0/oplangchain/llms/aleph_alpha.py
+-rw-r--r--   0        0        0     3021 2023-08-07 14:51:51.749553 oplangchain-0.1.0/oplangchain/llms/amazon_api_gateway.py
+-rw-r--r--   0        0        0    11164 2023-08-07 14:51:51.750554 oplangchain-0.1.0/oplangchain/llms/anthropic.py
+-rw-r--r--   0        0        0     4657 2023-08-07 14:51:51.750554 oplangchain-0.1.0/oplangchain/llms/anyscale.py
+-rw-r--r--   0        0        0     5365 2023-08-07 14:51:51.751553 oplangchain-0.1.0/oplangchain/llms/aviary.py
+-rw-r--r--   0        0        0    10218 2023-08-07 14:51:51.751553 oplangchain-0.1.0/oplangchain/llms/azureml_endpoint.py
+-rw-r--r--   0        0        0     4309 2023-08-07 14:51:51.752555 oplangchain-0.1.0/oplangchain/llms/bananadev.py
+-rw-r--r--   0        0        0    34723 2023-08-07 14:51:51.752555 oplangchain-0.1.0/oplangchain/llms/base.py
+-rw-r--r--   0        0        0     2359 2023-08-07 14:51:51.753553 oplangchain-0.1.0/oplangchain/llms/baseten.py
+-rw-r--r--   0        0        0     9064 2023-08-07 14:51:51.753553 oplangchain-0.1.0/oplangchain/llms/beam.py
+-rw-r--r--   0        0        0     6690 2023-08-07 14:51:51.754553 oplangchain-0.1.0/oplangchain/llms/bedrock.py
+-rw-r--r--   0        0        0     3773 2023-08-07 14:51:51.754553 oplangchain-0.1.0/oplangchain/llms/cerebriumai.py
+-rw-r--r--   0        0        0     3937 2023-08-07 14:51:51.755560 oplangchain-0.1.0/oplangchain/llms/chatglm.py
+-rw-r--r--   0        0        0     5802 2023-08-07 14:51:51.755560 oplangchain-0.1.0/oplangchain/llms/clarifai.py
+-rw-r--r--   0        0        0     7303 2023-08-07 14:51:51.756555 oplangchain-0.1.0/oplangchain/llms/cohere.py
+-rw-r--r--   0        0        0     4187 2023-08-07 14:51:51.756555 oplangchain-0.1.0/oplangchain/llms/ctransformers.py
+-rw-r--r--   0        0        0    12068 2023-08-07 14:51:51.757555 oplangchain-0.1.0/oplangchain/llms/databricks.py
+-rw-r--r--   0        0        0     3755 2023-08-07 14:51:51.757555 oplangchain-0.1.0/oplangchain/llms/deepinfra.py
+-rw-r--r--   0        0        0     7445 2023-08-07 14:51:51.758555 oplangchain-0.1.0/oplangchain/llms/edenai.py
+-rw-r--r--   0        0        0     1335 2023-08-07 14:51:51.758555 oplangchain-0.1.0/oplangchain/llms/fake.py
+-rw-r--r--   0        0        0    13035 2023-08-07 14:51:51.758555 oplangchain-0.1.0/oplangchain/llms/fireworks.py
+-rw-r--r--   0        0        0     3651 2023-08-07 14:51:51.759554 oplangchain-0.1.0/oplangchain/llms/forefrontai.py
+-rw-r--r--   0        0        0     5733 2023-08-07 14:51:51.759554 oplangchain-0.1.0/oplangchain/llms/google_palm.py
+-rw-r--r--   0        0        0     5122 2023-08-07 14:51:51.760553 oplangchain-0.1.0/oplangchain/llms/gooseai.py
+-rw-r--r--   0        0        0     6312 2023-08-07 14:51:51.760553 oplangchain-0.1.0/oplangchain/llms/gpt4all.py
+-rw-r--r--   0        0        0     5452 2023-08-07 14:51:51.761553 oplangchain-0.1.0/oplangchain/llms/huggingface_endpoint.py
+-rw-r--r--   0        0        0     4603 2023-08-07 14:51:51.761553 oplangchain-0.1.0/oplangchain/llms/huggingface_hub.py
+-rw-r--r--   0        0        0     6566 2023-08-07 14:51:51.762553 oplangchain-0.1.0/oplangchain/llms/huggingface_pipeline.py
+-rw-r--r--   0        0        0     9715 2023-08-07 14:51:51.762553 oplangchain-0.1.0/oplangchain/llms/huggingface_text_gen_inference.py
+-rw-r--r--   0        0        0     2541 2023-08-07 14:51:51.763557 oplangchain-0.1.0/oplangchain/llms/human.py
+-rw-r--r--   0        0        0     5065 2023-08-07 14:51:51.763557 oplangchain-0.1.0/oplangchain/llms/koboldai.py
+-rw-r--r--   0        0        0    10889 2023-08-07 14:51:51.763557 oplangchain-0.1.0/oplangchain/llms/llamacpp.py
+-rw-r--r--   0        0        0     1249 2023-08-07 14:51:51.764557 oplangchain-0.1.0/oplangchain/llms/loading.py
+-rw-r--r--   0        0        0     1874 2023-08-07 14:51:51.764557 oplangchain-0.1.0/oplangchain/llms/manifest.py
+-rw-r--r--   0        0        0     5154 2023-08-07 14:51:51.765556 oplangchain-0.1.0/oplangchain/llms/minimax.py
+-rw-r--r--   0        0        0     2919 2023-08-07 14:51:51.765556 oplangchain-0.1.0/oplangchain/llms/mlflow_ai_gateway.py
+-rw-r--r--   0        0        0     3239 2023-08-07 14:51:51.766557 oplangchain-0.1.0/oplangchain/llms/modal.py
+-rw-r--r--   0        0        0     6742 2023-08-07 14:51:51.766557 oplangchain-0.1.0/oplangchain/llms/mosaicml.py
+-rw-r--r--   0        0        0     5442 2023-08-07 14:51:51.767556 oplangchain-0.1.0/oplangchain/llms/nlpcloud.py
+-rw-r--r--   0        0        0     3804 2023-08-07 14:51:51.767556 oplangchain-0.1.0/oplangchain/llms/octoai_endpoint.py
+-rw-r--r--   0        0        0    34722 2023-08-07 14:51:51.768558 oplangchain-0.1.0/oplangchain/llms/openai.py
+-rw-r--r--   0        0        0     9922 2023-08-07 14:51:51.768558 oplangchain-0.1.0/oplangchain/llms/openllm.py
+-rw-r--r--   0        0        0      794 2023-08-07 14:51:51.769556 oplangchain-0.1.0/oplangchain/llms/openlm.py
+-rw-r--r--   0        0        0     5263 2023-08-07 14:51:51.769556 oplangchain-0.1.0/oplangchain/llms/petals.py
+-rw-r--r--   0        0        0     4013 2023-08-07 14:51:51.770556 oplangchain-0.1.0/oplangchain/llms/pipelineai.py
+-rw-r--r--   0        0        0     1527 2023-08-07 14:51:51.770556 oplangchain-0.1.0/oplangchain/llms/predibase.py
+-rw-r--r--   0        0        0     4364 2023-08-07 14:51:51.771554 oplangchain-0.1.0/oplangchain/llms/predictionguard.py
+-rw-r--r--   0        0        0     8682 2023-08-07 14:51:51.771554 oplangchain-0.1.0/oplangchain/llms/promptlayer_openai.py
+-rw-r--r--   0        0        0     5160 2023-08-07 14:51:51.772556 oplangchain-0.1.0/oplangchain/llms/replicate.py
+-rw-r--r--   0        0        0     7335 2023-08-07 14:51:51.772556 oplangchain-0.1.0/oplangchain/llms/rwkv.py
+-rw-r--r--   0        0        0     8811 2023-08-07 14:51:51.773554 oplangchain-0.1.0/oplangchain/llms/sagemaker_endpoint.py
+-rw-r--r--   0        0        0     7673 2023-08-07 14:51:51.773554 oplangchain-0.1.0/oplangchain/llms/self_hosted.py
+-rw-r--r--   0        0        0     7689 2023-08-07 14:51:51.774553 oplangchain-0.1.0/oplangchain/llms/self_hosted_hugging_face.py
+-rw-r--r--   0        0        0     4563 2023-08-07 14:51:51.774553 oplangchain-0.1.0/oplangchain/llms/stochasticai.py
+-rw-r--r--   0        0        0     7579 2023-08-07 14:51:51.775557 oplangchain-0.1.0/oplangchain/llms/textgen.py
+-rw-r--r--   0        0        0     7872 2023-08-07 14:51:51.775557 oplangchain-0.1.0/oplangchain/llms/tongyi.py
+-rw-r--r--   0        0        0      246 2023-08-07 14:51:51.776555 oplangchain-0.1.0/oplangchain/llms/utils.py
+-rw-r--r--   0        0        0     7709 2023-08-07 14:51:51.776555 oplangchain-0.1.0/oplangchain/llms/vertexai.py
+-rw-r--r--   0        0        0     3978 2023-08-07 14:51:51.777553 oplangchain-0.1.0/oplangchain/llms/vllm.py
+-rw-r--r--   0        0        0     4909 2023-08-07 14:51:51.777553 oplangchain-0.1.0/oplangchain/llms/writer.py
+-rw-r--r--   0        0        0     6011 2023-08-07 14:51:51.777553 oplangchain-0.1.0/oplangchain/llms/xinference.py
+-rw-r--r--   0        0        0       41 2023-08-07 14:51:51.778553 oplangchain-0.1.0/oplangchain/load/__init__.py
+-rw-r--r--   0        0        0      753 2023-08-07 14:51:51.779553 oplangchain-0.1.0/oplangchain/load/dump.py
+-rw-r--r--   0        0        0     4037 2023-08-07 14:51:51.779553 oplangchain-0.1.0/oplangchain/load/load.py
+-rw-r--r--   0        0        0     4618 2023-08-07 14:51:51.779553 oplangchain-0.1.0/oplangchain/load/serializable.py
+-rw-r--r--   0        0        0     2844 2023-08-07 14:51:51.780558 oplangchain-0.1.0/oplangchain/memory/__init__.py
+-rw-r--r--   0        0        0     3068 2023-08-07 14:51:51.781555 oplangchain-0.1.0/oplangchain/memory/buffer.py
+-rw-r--r--   0        0        0     1228 2023-08-07 14:51:51.781555 oplangchain-0.1.0/oplangchain/memory/buffer_window.py
+-rw-r--r--   0        0        0     1612 2023-08-07 14:51:51.782555 oplangchain-0.1.0/oplangchain/memory/chat_memory.py
+-rw-r--r--   0        0        0     1566 2023-08-07 14:51:51.783553 oplangchain-0.1.0/oplangchain/memory/chat_message_histories/__init__.py
+-rw-r--r--   0        0        0     2367 2023-08-07 14:51:51.783553 oplangchain-0.1.0/oplangchain/memory/chat_message_histories/cassandra.py
+-rw-r--r--   0        0        0     6493 2023-08-07 14:51:51.784555 oplangchain-0.1.0/oplangchain/memory/chat_message_histories/cosmos_db.py
+-rw-r--r--   0        0        0     2881 2023-08-07 14:51:51.784555 oplangchain-0.1.0/oplangchain/memory/chat_message_histories/dynamodb.py
+-rw-r--r--   0        0        0     1362 2023-08-07 14:51:51.785553 oplangchain-0.1.0/oplangchain/memory/chat_message_histories/file.py
+-rw-r--r--   0        0        0     3332 2023-08-07 14:51:51.785553 oplangchain-0.1.0/oplangchain/memory/chat_message_histories/firestore.py
+-rw-r--r--   0        0        0      584 2023-08-07 14:51:51.785553 oplangchain-0.1.0/oplangchain/memory/chat_message_histories/in_memory.py
+-rw-r--r--   0        0        0     6829 2023-08-07 14:51:51.786554 oplangchain-0.1.0/oplangchain/memory/chat_message_histories/momento.py
+-rw-r--r--   0        0        0     2719 2023-08-07 14:51:51.786554 oplangchain-0.1.0/oplangchain/memory/chat_message_histories/mongodb.py
+-rw-r--r--   0        0        0     2644 2023-08-07 14:51:51.787553 oplangchain-0.1.0/oplangchain/memory/chat_message_histories/postgres.py
+-rw-r--r--   0        0        0     1945 2023-08-07 14:51:51.787553 oplangchain-0.1.0/oplangchain/memory/chat_message_histories/redis.py
+-rw-r--r--   0        0        0     2897 2023-08-07 14:51:51.788555 oplangchain-0.1.0/oplangchain/memory/chat_message_histories/sql.py
+-rw-r--r--   0        0        0     1176 2023-08-07 14:51:51.788555 oplangchain-0.1.0/oplangchain/memory/chat_message_histories/streamlit.py
+-rw-r--r--   0        0        0     6402 2023-08-07 14:51:51.789557 oplangchain-0.1.0/oplangchain/memory/chat_message_histories/zep.py
+-rw-r--r--   0        0        0     2889 2023-08-07 14:51:51.789557 oplangchain-0.1.0/oplangchain/memory/combined.py
+-rw-r--r--   0        0        0    12982 2023-08-07 14:51:51.790555 oplangchain-0.1.0/oplangchain/memory/entity.py
+-rw-r--r--   0        0        0     5017 2023-08-07 14:51:51.790555 oplangchain-0.1.0/oplangchain/memory/kg.py
+-rw-r--r--   0        0        0     3098 2023-08-07 14:51:51.790555 oplangchain-0.1.0/oplangchain/memory/motorhead_memory.py
+-rw-r--r--   0        0        0     8176 2023-08-07 14:51:51.791553 oplangchain-0.1.0/oplangchain/memory/prompt.py
+-rw-r--r--   0        0        0      789 2023-08-07 14:51:51.791553 oplangchain-0.1.0/oplangchain/memory/readonly.py
+-rw-r--r--   0        0        0      756 2023-08-07 14:51:51.792554 oplangchain-0.1.0/oplangchain/memory/simple.py
+-rw-r--r--   0        0        0     3342 2023-08-07 14:51:51.792554 oplangchain-0.1.0/oplangchain/memory/summary.py
+-rw-r--r--   0        0        0     2933 2023-08-07 14:51:51.793554 oplangchain-0.1.0/oplangchain/memory/summary_buffer.py
+-rw-r--r--   0        0        0     1915 2023-08-07 14:51:51.793554 oplangchain-0.1.0/oplangchain/memory/token_buffer.py
+-rw-r--r--   0        0        0      687 2023-08-07 14:51:51.793554 oplangchain-0.1.0/oplangchain/memory/utils.py
+-rw-r--r--   0        0        0     2976 2023-08-07 14:51:51.794553 oplangchain-0.1.0/oplangchain/memory/vectorstore.py
+-rw-r--r--   0        0        0     5067 2023-08-07 14:51:51.794553 oplangchain-0.1.0/oplangchain/memory/zep_memory.py
+-rw-r--r--   0        0        0     3236 2023-08-07 14:51:51.795553 oplangchain-0.1.0/oplangchain/model_laboratory.py
+-rw-r--r--   0        0        0     1588 2023-08-07 14:51:51.795553 oplangchain-0.1.0/oplangchain/output_parsers/__init__.py
+-rw-r--r--   0        0        0     1071 2023-08-07 14:51:51.796553 oplangchain-0.1.0/oplangchain/output_parsers/boolean.py
+-rw-r--r--   0        0        0     1763 2023-08-07 14:51:51.797557 oplangchain-0.1.0/oplangchain/output_parsers/combining.py
+-rw-r--r--   0        0        0     1817 2023-08-07 14:51:51.797557 oplangchain-0.1.0/oplangchain/output_parsers/datetime.py
+-rw-r--r--   0        0        0     1138 2023-08-07 14:51:51.798554 oplangchain-0.1.0/oplangchain/output_parsers/enum.py
+-rw-r--r--   0        0        0     1805 2023-08-07 14:51:51.798554 oplangchain-0.1.0/oplangchain/output_parsers/fix.py
+-rw-r--r--   0        0        0      810 2023-08-07 14:51:51.799553 oplangchain-0.1.0/oplangchain/output_parsers/format_instructions.py
+-rw-r--r--   0        0        0     2209 2023-08-07 14:51:51.799553 oplangchain-0.1.0/oplangchain/output_parsers/json.py
+-rw-r--r--   0        0        0      939 2023-08-07 14:51:51.800554 oplangchain-0.1.0/oplangchain/output_parsers/list.py
+-rw-r--r--   0        0        0      702 2023-08-07 14:51:51.800554 oplangchain-0.1.0/oplangchain/output_parsers/loading.py
+-rw-r--r--   0        0        0     3350 2023-08-07 14:51:51.801553 oplangchain-0.1.0/oplangchain/output_parsers/openai_functions.py
+-rw-r--r--   0        0        0      503 2023-08-07 14:51:51.801553 oplangchain-0.1.0/oplangchain/output_parsers/prompts.py
+-rw-r--r--   0        0        0     1731 2023-08-07 14:51:51.802553 oplangchain-0.1.0/oplangchain/output_parsers/pydantic.py
+-rw-r--r--   0        0        0     3165 2023-08-07 14:51:51.802553 oplangchain-0.1.0/oplangchain/output_parsers/rail_parser.py
+-rw-r--r--   0        0        0     1196 2023-08-07 14:51:51.803553 oplangchain-0.1.0/oplangchain/output_parsers/regex.py
+-rw-r--r--   0        0        0     1696 2023-08-07 14:51:51.803553 oplangchain-0.1.0/oplangchain/output_parsers/regex_dict.py
+-rw-r--r--   0        0        0     4709 2023-08-07 14:51:51.803553 oplangchain-0.1.0/oplangchain/output_parsers/retry.py
+-rw-r--r--   0        0        0     3070 2023-08-07 14:51:51.804553 oplangchain-0.1.0/oplangchain/output_parsers/structured.py
+-rw-r--r--   0        0        0     2744 2023-08-07 14:51:51.805554 oplangchain-0.1.0/oplangchain/prompts/__init__.py
+-rw-r--r--   0        0        0     3671 2023-08-07 14:51:51.805554 oplangchain-0.1.0/oplangchain/prompts/base.py
+-rw-r--r--   0        0        0    21563 2023-08-07 14:51:51.806555 oplangchain-0.1.0/oplangchain/prompts/chat.py
+-rw-r--r--   0        0        0      553 2023-08-07 14:51:51.806555 oplangchain-0.1.0/oplangchain/prompts/example_selector/__init__.py
+-rw-r--r--   0        0        0      526 2023-08-07 14:51:51.807553 oplangchain-0.1.0/oplangchain/prompts/example_selector/base.py
+-rw-r--r--   0        0        0     2433 2023-08-07 14:51:51.808556 oplangchain-0.1.0/oplangchain/prompts/example_selector/length_based.py
+-rw-r--r--   0        0        0     3798 2023-08-07 14:51:51.808556 oplangchain-0.1.0/oplangchain/prompts/example_selector/ngram_overlap.py
+-rw-r--r--   0        0        0     6848 2023-08-07 14:51:51.809554 oplangchain-0.1.0/oplangchain/prompts/example_selector/semantic_similarity.py
+-rw-r--r--   0        0        0    11737 2023-08-07 14:51:51.809554 oplangchain-0.1.0/oplangchain/prompts/few_shot.py
+-rw-r--r--   0        0        0     5423 2023-08-07 14:51:51.810553 oplangchain-0.1.0/oplangchain/prompts/few_shot_with_templates.py
+-rw-r--r--   0        0        0     5507 2023-08-07 14:51:51.810553 oplangchain-0.1.0/oplangchain/prompts/loading.py
+-rw-r--r--   0        0        0     2254 2023-08-07 14:51:51.811553 oplangchain-0.1.0/oplangchain/prompts/pipeline.py
+-rw-r--r--   0        0        0     8136 2023-08-07 14:51:51.811553 oplangchain-0.1.0/oplangchain/prompts/prompt.py
+-rw-r--r--   0        0        0        0 2023-08-07 14:51:51.811553 oplangchain-0.1.0/oplangchain/py.typed
+-rw-r--r--   0        0        0      111 2023-08-07 14:51:51.812554 oplangchain-0.1.0/oplangchain/python.py
+-rw-r--r--   0        0        0      212 2023-08-07 14:51:51.812554 oplangchain-0.1.0/oplangchain/requests.py
+-rw-r--r--   0        0        0     3614 2023-08-07 14:51:51.813554 oplangchain-0.1.0/oplangchain/retrievers/__init__.py
+-rw-r--r--   0        0        0      582 2023-08-07 14:51:51.814556 oplangchain-0.1.0/oplangchain/retrievers/arxiv.py
+-rw-r--r--   0        0        0     4042 2023-08-07 14:51:51.814556 oplangchain-0.1.0/oplangchain/retrievers/azure_cognitive_search.py
+-rw-r--r--   0        0        0     3653 2023-08-07 14:51:51.815554 oplangchain-0.1.0/oplangchain/retrievers/bm25.py
+-rw-r--r--   0        0        0     2649 2023-08-07 14:51:51.815554 oplangchain-0.1.0/oplangchain/retrievers/chaindesk.py
+-rw-r--r--   0        0        0     2998 2023-08-07 14:51:51.816554 oplangchain-0.1.0/oplangchain/retrievers/chatgpt_plugin_retriever.py
+-rw-r--r--   0        0        0     2255 2023-08-07 14:51:51.816554 oplangchain-0.1.0/oplangchain/retrievers/contextual_compression.py
+-rw-r--r--   0        0        0     2303 2023-08-07 14:51:51.817555 oplangchain-0.1.0/oplangchain/retrievers/databerry.py
+-rw-r--r--   0        0        0     6730 2023-08-07 14:51:51.817555 oplangchain-0.1.0/oplangchain/retrievers/docarray.py
+-rw-r--r--   0        0        0      591 2023-08-07 14:51:51.818556 oplangchain-0.1.0/oplangchain/retrievers/document_compressors/__init__.py
+-rw-r--r--   0        0        0     3658 2023-08-07 14:51:51.819555 oplangchain-0.1.0/oplangchain/retrievers/document_compressors/base.py
+-rw-r--r--   0        0        0     3813 2023-08-07 14:51:51.819555 oplangchain-0.1.0/oplangchain/retrievers/document_compressors/chain_extract.py
+-rw-r--r--   0        0        0      366 2023-08-07 14:51:51.820553 oplangchain-0.1.0/oplangchain/retrievers/document_compressors/chain_extract_prompt.py
+-rw-r--r--   0        0        0     2965 2023-08-07 14:51:51.820553 oplangchain-0.1.0/oplangchain/retrievers/document_compressors/chain_filter.py
+-rw-r--r--   0        0        0      231 2023-08-07 14:51:51.821553 oplangchain-0.1.0/oplangchain/retrievers/document_compressors/chain_filter_prompt.py
+-rw-r--r--   0        0        0     2961 2023-08-07 14:51:51.821553 oplangchain-0.1.0/oplangchain/retrievers/document_compressors/cohere_rerank.py
+-rw-r--r--   0        0        0     3139 2023-08-07 14:51:51.822559 oplangchain-0.1.0/oplangchain/retrievers/document_compressors/embeddings_filter.py
+-rw-r--r--   0        0        0     4658 2023-08-07 14:51:51.822559 oplangchain-0.1.0/oplangchain/retrievers/elastic_search_bm25.py
+-rw-r--r--   0        0        0     5793 2023-08-07 14:51:51.822559 oplangchain-0.1.0/oplangchain/retrievers/ensemble.py
+-rw-r--r--   0        0        0     7430 2023-08-07 14:51:51.823557 oplangchain-0.1.0/oplangchain/retrievers/google_cloud_enterprise_search.py
+-rw-r--r--   0        0        0    12601 2023-08-07 14:51:51.823557 oplangchain-0.1.0/oplangchain/retrievers/kendra.py
+-rw-r--r--   0        0        0     2527 2023-08-07 14:51:51.824556 oplangchain-0.1.0/oplangchain/retrievers/knn.py
+-rw-r--r--   0        0        0     3022 2023-08-07 14:51:51.824556 oplangchain-0.1.0/oplangchain/retrievers/llama_index.py
+-rw-r--r--   0        0        0     3373 2023-08-07 14:51:51.825559 oplangchain-0.1.0/oplangchain/retrievers/merger_retriever.py
+-rw-r--r--   0        0        0     1439 2023-08-07 14:51:51.825559 oplangchain-0.1.0/oplangchain/retrievers/metal.py
+-rw-r--r--   0        0        0     2377 2023-08-07 14:51:51.826554 oplangchain-0.1.0/oplangchain/retrievers/milvus.py
+-rw-r--r--   0        0        0     4834 2023-08-07 14:51:51.826554 oplangchain-0.1.0/oplangchain/retrievers/multi_query.py
+-rw-r--r--   0        0        0     5436 2023-08-07 14:51:51.827554 oplangchain-0.1.0/oplangchain/retrievers/pinecone_hybrid_search.py
+-rw-r--r--   0        0        0      592 2023-08-07 14:51:51.827554 oplangchain-0.1.0/oplangchain/retrievers/pubmed.py
+-rw-r--r--   0        0        0       94 2023-08-07 14:51:51.827554 oplangchain-0.1.0/oplangchain/retrievers/pupmed.py
+-rw-r--r--   0        0        0     2601 2023-08-07 14:51:51.828554 oplangchain-0.1.0/oplangchain/retrievers/re_phraser.py
+-rw-r--r--   0        0        0     1903 2023-08-07 14:51:51.829553 oplangchain-0.1.0/oplangchain/retrievers/remote_retriever.py
+-rw-r--r--   0        0        0        0 2023-08-07 14:51:51.829553 oplangchain-0.1.0/oplangchain/retrievers/self_query/__init__.py
+-rw-r--r--   0        0        0     5945 2023-08-07 14:51:51.830554 oplangchain-0.1.0/oplangchain/retrievers/self_query/base.py
+-rw-r--r--   0        0        0     1442 2023-08-07 14:51:51.830554 oplangchain-0.1.0/oplangchain/retrievers/self_query/chroma.py
+-rw-r--r--   0        0        0     2592 2023-08-07 14:51:51.831553 oplangchain-0.1.0/oplangchain/retrievers/self_query/deeplake.py
+-rw-r--r--   0        0        0     3595 2023-08-07 14:51:51.831553 oplangchain-0.1.0/oplangchain/retrievers/self_query/myscale.py
+-rw-r--r--   0        0        0     1448 2023-08-07 14:51:51.832554 oplangchain-0.1.0/oplangchain/retrievers/self_query/pinecone.py
+-rw-r--r--   0        0        0     2811 2023-08-07 14:51:51.832554 oplangchain-0.1.0/oplangchain/retrievers/self_query/qdrant.py
+-rw-r--r--   0        0        0     1501 2023-08-07 14:51:51.833553 oplangchain-0.1.0/oplangchain/retrievers/self_query/weaviate.py
+-rw-r--r--   0        0        0     3657 2023-08-07 14:51:51.833553 oplangchain-0.1.0/oplangchain/retrievers/svm.py
+-rw-r--r--   0        0        0     4035 2023-08-07 14:51:51.834553 oplangchain-0.1.0/oplangchain/retrievers/tfidf.py
+-rw-r--r--   0        0        0     5812 2023-08-07 14:51:51.834553 oplangchain-0.1.0/oplangchain/retrievers/time_weighted_retriever.py
+-rw-r--r--   0        0        0     4597 2023-08-07 14:51:51.834553 oplangchain-0.1.0/oplangchain/retrievers/vespa_retriever.py
+-rw-r--r--   0        0        0     4053 2023-08-07 14:51:51.835553 oplangchain-0.1.0/oplangchain/retrievers/weaviate_hybrid_search.py
+-rw-r--r--   0        0        0     8276 2023-08-07 14:51:51.835553 oplangchain-0.1.0/oplangchain/retrievers/web_research.py
+-rw-r--r--   0        0        0      605 2023-08-07 14:51:51.836553 oplangchain-0.1.0/oplangchain/retrievers/wikipedia.py
+-rw-r--r--   0        0        0     3071 2023-08-07 14:51:51.836553 oplangchain-0.1.0/oplangchain/retrievers/zep.py
+-rw-r--r--   0        0        0     2671 2023-08-07 14:51:51.837553 oplangchain-0.1.0/oplangchain/retrievers/zilliz.py
+-rw-r--r--   0        0        0     1718 2023-08-07 14:51:51.837553 oplangchain-0.1.0/oplangchain/schema/__init__.py
+-rw-r--r--   0        0        0      643 2023-08-07 14:51:51.838554 oplangchain-0.1.0/oplangchain/schema/agent.py
+-rw-r--r--   0        0        0     2656 2023-08-07 14:51:51.838554 oplangchain-0.1.0/oplangchain/schema/document.py
+-rw-r--r--   0        0        0    10169 2023-08-07 14:51:51.839555 oplangchain-0.1.0/oplangchain/schema/language_model.py
+-rw-r--r--   0        0        0     4095 2023-08-07 14:51:51.839555 oplangchain-0.1.0/oplangchain/schema/memory.py
+-rw-r--r--   0        0        0     7482 2023-08-07 14:51:51.840555 oplangchain-0.1.0/oplangchain/schema/messages.py
+-rw-r--r--   0        0        0     5447 2023-08-07 14:51:51.840555 oplangchain-0.1.0/oplangchain/schema/output.py
+-rw-r--r--   0        0        0     7782 2023-08-07 14:51:51.841553 oplangchain-0.1.0/oplangchain/schema/output_parser.py
+-rw-r--r--   0        0        0      634 2023-08-07 14:51:51.841553 oplangchain-0.1.0/oplangchain/schema/prompt.py
+-rw-r--r--   0        0        0     6865 2023-08-07 14:51:51.841553 oplangchain-0.1.0/oplangchain/schema/prompt_template.py
+-rw-r--r--   0        0        0    10045 2023-08-07 14:51:51.842553 oplangchain-0.1.0/oplangchain/schema/retriever.py
+-rw-r--r--   0        0        0    40366 2023-08-07 14:51:51.842553 oplangchain-0.1.0/oplangchain/schema/runnable.py
+-rw-r--r--   0        0        0      120 2023-08-07 14:51:51.843553 oplangchain-0.1.0/oplangchain/serpapi.py
+-rw-r--r--   0        0        0      533 2023-08-07 14:51:51.843553 oplangchain-0.1.0/oplangchain/server.py
+-rw-r--r--   0        0        0     3561 2023-08-07 14:51:51.844553 oplangchain-0.1.0/oplangchain/smith/__init__.py
+-rw-r--r--   0        0        0     2189 2023-08-07 14:51:51.845553 oplangchain-0.1.0/oplangchain/smith/evaluation/__init__.py
+-rw-r--r--   0        0        0     8567 2023-08-07 14:51:51.845553 oplangchain-0.1.0/oplangchain/smith/evaluation/config.py
+-rw-r--r--   0        0        0    51494 2023-08-07 14:51:51.846553 oplangchain-0.1.0/oplangchain/smith/evaluation/runner_utils.py
+-rw-r--r--   0        0        0    15807 2023-08-07 14:51:51.847555 oplangchain-0.1.0/oplangchain/smith/evaluation/string_run_evaluator.py
+-rw-r--r--   0        0        0        0 2023-08-07 14:51:51.847555 oplangchain-0.1.0/oplangchain/smith/evaluation/utils.py
+-rw-r--r--   0        0        0      129 2023-08-07 14:51:51.848554 oplangchain-0.1.0/oplangchain/sql_database.py
+-rw-r--r--   0        0        0    38439 2023-08-07 14:51:51.848554 oplangchain-0.1.0/oplangchain/text_splitter.py
+-rw-r--r--   0        0        0     6594 2023-08-07 14:51:51.849553 oplangchain-0.1.0/oplangchain/tools/__init__.py
+-rw-r--r--   0        0        0      237 2023-08-07 14:51:51.850553 oplangchain-0.1.0/oplangchain/tools/amadeus/__init__.py
+-rw-r--r--   0        0        0      407 2023-08-07 14:51:51.850553 oplangchain-0.1.0/oplangchain/tools/amadeus/base.py
+-rw-r--r--   0        0        0     1974 2023-08-07 14:51:51.850553 oplangchain-0.1.0/oplangchain/tools/amadeus/closest_airport.py
+-rw-r--r--   0        0        0     5557 2023-08-07 14:51:51.851553 oplangchain-0.1.0/oplangchain/tools/amadeus/flight_search.py
+-rw-r--r--   0        0        0     1123 2023-08-07 14:51:51.851553 oplangchain-0.1.0/oplangchain/tools/amadeus/utils.py
+-rw-r--r--   0        0        0       25 2023-08-07 14:51:51.852553 oplangchain-0.1.0/oplangchain/tools/arxiv/__init__.py
+-rw-r--r--   0        0        0     1000 2023-08-07 14:51:51.853554 oplangchain-0.1.0/oplangchain/tools/arxiv/tool.py
+-rw-r--r--   0        0        0      595 2023-08-07 14:51:51.853554 oplangchain-0.1.0/oplangchain/tools/azure_cognitive_services/__init__.py
+-rw-r--r--   0        0        0     5326 2023-08-07 14:51:51.854554 oplangchain-0.1.0/oplangchain/tools/azure_cognitive_services/form_recognizer.py
+-rw-r--r--   0        0        0     5255 2023-08-07 14:51:51.854554 oplangchain-0.1.0/oplangchain/tools/azure_cognitive_services/image_analysis.py
+-rw-r--r--   0        0        0     4296 2023-08-07 14:51:51.855557 oplangchain-0.1.0/oplangchain/tools/azure_cognitive_services/speech2text.py
+-rw-r--r--   0        0        0     3646 2023-08-07 14:51:51.855557 oplangchain-0.1.0/oplangchain/tools/azure_cognitive_services/text2speech.py
+-rw-r--r--   0        0        0      776 2023-08-07 14:51:51.856554 oplangchain-0.1.0/oplangchain/tools/azure_cognitive_services/utils.py
+-rw-r--r--   0        0        0    26843 2023-08-07 14:51:51.856554 oplangchain-0.1.0/oplangchain/tools/base.py
+-rw-r--r--   0        0        0      160 2023-08-07 14:51:51.857554 oplangchain-0.1.0/oplangchain/tools/bing_search/__init__.py
+-rw-r--r--   0        0        0     1435 2023-08-07 14:51:51.858553 oplangchain-0.1.0/oplangchain/tools/bing_search/tool.py
+-rw-r--r--   0        0        0        0 2023-08-07 14:51:51.858553 oplangchain-0.1.0/oplangchain/tools/brave_search/__init__.py
+-rw-r--r--   0        0        0     1336 2023-08-07 14:51:51.859554 oplangchain-0.1.0/oplangchain/tools/brave_search/tool.py
+-rw-r--r--   0        0        0     1736 2023-08-07 14:51:51.859554 oplangchain-0.1.0/oplangchain/tools/convert_to_openai.py
+-rw-r--r--   0        0        0      258 2023-08-07 14:51:51.860553 oplangchain-0.1.0/oplangchain/tools/dataforseo_api_search/__init__.py
+-rw-r--r--   0        0        0     2176 2023-08-07 14:51:51.860553 oplangchain-0.1.0/oplangchain/tools/dataforseo_api_search/tool.py
+-rw-r--r--   0        0        0      137 2023-08-07 14:51:51.861553 oplangchain-0.1.0/oplangchain/tools/ddg_search/__init__.py
+-rw-r--r--   0        0        0     2315 2023-08-07 14:51:51.862553 oplangchain-0.1.0/oplangchain/tools/ddg_search/tool.py
+-rw-r--r--   0        0        0      653 2023-08-07 14:51:51.862553 oplangchain-0.1.0/oplangchain/tools/file_management/__init__.py
+-rw-r--r--   0        0        0     1724 2023-08-07 14:51:51.863557 oplangchain-0.1.0/oplangchain/tools/file_management/copy.py
+-rw-r--r--   0        0        0     1320 2023-08-07 14:51:51.863557 oplangchain-0.1.0/oplangchain/tools/file_management/delete.py
+-rw-r--r--   0        0        0     1940 2023-08-07 14:51:51.864555 oplangchain-0.1.0/oplangchain/tools/file_management/file_search.py
+-rw-r--r--   0        0        0     1407 2023-08-07 14:51:51.865554 oplangchain-0.1.0/oplangchain/tools/file_management/list_dir.py
+-rw-r--r--   0        0        0     1864 2023-08-07 14:51:51.865554 oplangchain-0.1.0/oplangchain/tools/file_management/move.py
+-rw-r--r--   0        0        0     1315 2023-08-07 14:51:51.866553 oplangchain-0.1.0/oplangchain/tools/file_management/read.py
+-rw-r--r--   0        0        0     1708 2023-08-07 14:51:51.866553 oplangchain-0.1.0/oplangchain/tools/file_management/utils.py
+-rw-r--r--   0        0        0     1589 2023-08-07 14:51:51.866553 oplangchain-0.1.0/oplangchain/tools/file_management/write.py
+-rw-r--r--   0        0        0       20 2023-08-07 14:51:51.867553 oplangchain-0.1.0/oplangchain/tools/github/__init__.py
+-rw-r--r--   0        0        0     3438 2023-08-07 14:51:51.868553 oplangchain-0.1.0/oplangchain/tools/github/prompt.py
+-rw-r--r--   0        0        0      921 2023-08-07 14:51:51.868553 oplangchain-0.1.0/oplangchain/tools/github/tool.py
+-rw-r--r--   0        0        0      541 2023-08-07 14:51:51.869554 oplangchain-0.1.0/oplangchain/tools/gmail/__init__.py
+-rw-r--r--   0        0        0      976 2023-08-07 14:51:51.869554 oplangchain-0.1.0/oplangchain/tools/gmail/base.py
+-rw-r--r--   0        0        0     2539 2023-08-07 14:51:51.870553 oplangchain-0.1.0/oplangchain/tools/gmail/create_draft.py
+-rw-r--r--   0        0        0     1727 2023-08-07 14:51:51.870553 oplangchain-0.1.0/oplangchain/tools/gmail/get_message.py
+-rw-r--r--   0        0        0     1535 2023-08-07 14:51:51.871553 oplangchain-0.1.0/oplangchain/tools/gmail/get_thread.py
+-rw-r--r--   0        0        0     4363 2023-08-07 14:51:51.871553 oplangchain-0.1.0/oplangchain/tools/gmail/search.py
+-rw-r--r--   0        0        0     2847 2023-08-07 14:51:51.872555 oplangchain-0.1.0/oplangchain/tools/gmail/send_message.py
+-rw-r--r--   0        0        0     4528 2023-08-07 14:51:51.872555 oplangchain-0.1.0/oplangchain/tools/gmail/utils.py
+-rw-r--r--   0        0        0      126 2023-08-07 14:51:51.873555 oplangchain-0.1.0/oplangchain/tools/golden_query/__init__.py
+-rw-r--r--   0        0        0     1090 2023-08-07 14:51:51.873555 oplangchain-0.1.0/oplangchain/tools/golden_query/tool.py
+-rw-r--r--   0        0        0      130 2023-08-07 14:51:51.874554 oplangchain-0.1.0/oplangchain/tools/google_places/__init__.py
+-rw-r--r--   0        0        0     1106 2023-08-07 14:51:51.875555 oplangchain-0.1.0/oplangchain/tools/google_places/tool.py
+-rw-r--r--   0        0        0      172 2023-08-07 14:51:51.875555 oplangchain-0.1.0/oplangchain/tools/google_search/__init__.py
+-rw-r--r--   0        0        0     1461 2023-08-07 14:51:51.876553 oplangchain-0.1.0/oplangchain/tools/google_search/tool.py
+-rw-r--r--   0        0        0      220 2023-08-07 14:51:51.877554 oplangchain-0.1.0/oplangchain/tools/google_serper/__init__.py
+-rw-r--r--   0        0        0     2076 2023-08-07 14:51:51.877554 oplangchain-0.1.0/oplangchain/tools/google_serper/tool.py
+-rw-r--r--   0        0        0       47 2023-08-07 14:51:51.878556 oplangchain-0.1.0/oplangchain/tools/graphql/__init__.py
+-rw-r--r--   0        0        0     1186 2023-08-07 14:51:51.878556 oplangchain-0.1.0/oplangchain/tools/graphql/tool.py
+-rw-r--r--   0        0        0      122 2023-08-07 14:51:51.879554 oplangchain-0.1.0/oplangchain/tools/human/__init__.py
+-rw-r--r--   0        0        0      959 2023-08-07 14:51:51.880557 oplangchain-0.1.0/oplangchain/tools/human/tool.py
+-rw-r--r--   0        0        0     2290 2023-08-07 14:51:51.880557 oplangchain-0.1.0/oplangchain/tools/ifttt.py
+-rw-r--r--   0        0        0       43 2023-08-07 14:51:51.881555 oplangchain-0.1.0/oplangchain/tools/interaction/__init__.py
+-rw-r--r--   0        0        0      454 2023-08-07 14:51:51.881555 oplangchain-0.1.0/oplangchain/tools/interaction/tool.py
+-rw-r--r--   0        0        0       17 2023-08-07 14:51:51.882557 oplangchain-0.1.0/oplangchain/tools/jira/__init__.py
+-rw-r--r--   0        0        0     3170 2023-08-07 14:51:51.883554 oplangchain-0.1.0/oplangchain/tools/jira/prompt.py
+-rw-r--r--   0        0        0     1569 2023-08-07 14:51:51.883554 oplangchain-0.1.0/oplangchain/tools/jira/tool.py
+-rw-r--r--   0        0        0       46 2023-08-07 14:51:51.884555 oplangchain-0.1.0/oplangchain/tools/json/__init__.py
+-rw-r--r--   0        0        0     4087 2023-08-07 14:51:51.885554 oplangchain-0.1.0/oplangchain/tools/json/tool.py
+-rw-r--r--   0        0        0      144 2023-08-07 14:51:51.886555 oplangchain-0.1.0/oplangchain/tools/metaphor_search/__init__.py
+-rw-r--r--   0        0        0     2672 2023-08-07 14:51:51.886555 oplangchain-0.1.0/oplangchain/tools/metaphor_search/tool.py
+-rw-r--r--   0        0        0      237 2023-08-07 14:51:51.887554 oplangchain-0.1.0/oplangchain/tools/multion/__init__.py
+-rw-r--r--   0        0        0     1577 2023-08-07 14:51:51.888554 oplangchain-0.1.0/oplangchain/tools/multion/create_session.py
+-rw-r--r--   0        0        0     2116 2023-08-07 14:51:51.888554 oplangchain-0.1.0/oplangchain/tools/multion/update_session.py
+-rw-r--r--   0        0        0      101 2023-08-07 14:51:51.889554 oplangchain-0.1.0/oplangchain/tools/nuclia/__init__.py
+-rw-r--r--   0        0        0     7575 2023-08-07 14:51:51.890557 oplangchain-0.1.0/oplangchain/tools/nuclia/tool.py
+-rw-r--r--   0        0        0      585 2023-08-07 14:51:51.890557 oplangchain-0.1.0/oplangchain/tools/office365/__init__.py
+-rw-r--r--   0        0        0      480 2023-08-07 14:51:51.891554 oplangchain-0.1.0/oplangchain/tools/office365/base.py
+-rw-r--r--   0        0        0     1832 2023-08-07 14:51:51.891554 oplangchain-0.1.0/oplangchain/tools/office365/create_draft_message.py
+-rw-r--r--   0        0        0     4846 2023-08-07 14:51:51.892556 oplangchain-0.1.0/oplangchain/tools/office365/events_search.py
+-rw-r--r--   0        0        0     4160 2023-08-07 14:51:51.892556 oplangchain-0.1.0/oplangchain/tools/office365/messages_search.py
+-rw-r--r--   0        0        0     2830 2023-08-07 14:51:51.893556 oplangchain-0.1.0/oplangchain/tools/office365/send_event.py
+-rw-r--r--   0        0        0     1763 2023-08-07 14:51:51.893556 oplangchain-0.1.0/oplangchain/tools/office365/send_message.py
+-rw-r--r--   0        0        0     2136 2023-08-07 14:51:51.894556 oplangchain-0.1.0/oplangchain/tools/office365/utils.py
+-rw-r--r--   0        0        0        0 2023-08-07 14:51:51.894556 oplangchain-0.1.0/oplangchain/tools/openapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 14:51:51.895553 oplangchain-0.1.0/oplangchain/tools/openapi/utils/__init__.py
+-rw-r--r--   0        0        0    20553 2023-08-07 14:51:51.896553 oplangchain-0.1.0/oplangchain/tools/openapi/utils/api_models.py
+-rw-r--r--   0        0        0      156 2023-08-07 14:51:51.896553 oplangchain-0.1.0/oplangchain/tools/openapi/utils/openapi_utils.py
+-rw-r--r--   0        0        0      152 2023-08-07 14:51:51.897555 oplangchain-0.1.0/oplangchain/tools/openweathermap/__init__.py
+-rw-r--r--   0        0        0      916 2023-08-07 14:51:51.897555 oplangchain-0.1.0/oplangchain/tools/openweathermap/tool.py
+-rw-r--r--   0        0        0      684 2023-08-07 14:51:51.898554 oplangchain-0.1.0/oplangchain/tools/playwright/__init__.py
+-rw-r--r--   0        0        0     2118 2023-08-07 14:51:51.899555 oplangchain-0.1.0/oplangchain/tools/playwright/base.py
+-rw-r--r--   0        0        0     3048 2023-08-07 14:51:51.899555 oplangchain-0.1.0/oplangchain/tools/playwright/click.py
+-rw-r--r--   0        0        0     1292 2023-08-07 14:51:51.900556 oplangchain-0.1.0/oplangchain/tools/playwright/current_page.py
+-rw-r--r--   0        0        0     3003 2023-08-07 14:51:51.901555 oplangchain-0.1.0/oplangchain/tools/playwright/extract_hyperlinks.py
+-rw-r--r--   0        0        0     2335 2023-08-07 14:51:51.901555 oplangchain-0.1.0/oplangchain/tools/playwright/extract_text.py
+-rw-r--r--   0        0        0     3695 2023-08-07 14:51:51.902555 oplangchain-0.1.0/oplangchain/tools/playwright/get_elements.py
+-rw-r--r--   0        0        0     1756 2023-08-07 14:51:51.902555 oplangchain-0.1.0/oplangchain/tools/playwright/navigate.py
+-rw-r--r--   0        0        0     1891 2023-08-07 14:51:51.902555 oplangchain-0.1.0/oplangchain/tools/playwright/navigate_back.py
+-rw-r--r--   0        0        0     2813 2023-08-07 14:51:51.903555 oplangchain-0.1.0/oplangchain/tools/playwright/utils.py
+-rw-r--r--   0        0        0     2888 2023-08-07 14:51:51.903555 oplangchain-0.1.0/oplangchain/tools/plugin.py
+-rw-r--r--   0        0        0       52 2023-08-07 14:51:51.904555 oplangchain-0.1.0/oplangchain/tools/powerbi/__init__.py
+-rw-r--r--   0        0        0     7339 2023-08-07 14:51:51.905557 oplangchain-0.1.0/oplangchain/tools/powerbi/prompt.py
+-rw-r--r--   0        0        0    11057 2023-08-07 14:51:51.905557 oplangchain-0.1.0/oplangchain/tools/powerbi/tool.py
+-rw-r--r--   0        0        0       26 2023-08-07 14:51:51.906554 oplangchain-0.1.0/oplangchain/tools/pubmed/__init__.py
+-rw-r--r--   0        0        0     1010 2023-08-07 14:51:51.907554 oplangchain-0.1.0/oplangchain/tools/pubmed/tool.py
+-rw-r--r--   0        0        0        0 2023-08-07 14:51:51.907554 oplangchain-0.1.0/oplangchain/tools/python/__init__.py
+-rw-r--r--   0        0        0     4313 2023-08-07 14:51:51.908554 oplangchain-0.1.0/oplangchain/tools/python/tool.py
+-rw-r--r--   0        0        0       52 2023-08-07 14:51:51.909554 oplangchain-0.1.0/oplangchain/tools/requests/__init__.py
+-rw-r--r--   0        0        0     6248 2023-08-07 14:51:51.909554 oplangchain-0.1.0/oplangchain/tools/requests/tool.py
+-rw-r--r--   0        0        0       31 2023-08-07 14:51:51.910555 oplangchain-0.1.0/oplangchain/tools/scenexplain/__init__.py
+-rw-r--r--   0        0        0     1065 2023-08-07 14:51:51.910555 oplangchain-0.1.0/oplangchain/tools/scenexplain/tool.py
+-rw-r--r--   0        0        0        0 2023-08-07 14:51:51.911554 oplangchain-0.1.0/oplangchain/tools/searx_search/__init__.py
+-rw-r--r--   0        0        0     2216 2023-08-07 14:51:51.912556 oplangchain-0.1.0/oplangchain/tools/searx_search/tool.py
+-rw-r--r--   0        0        0       93 2023-08-07 14:51:51.913554 oplangchain-0.1.0/oplangchain/tools/shell/__init__.py
+-rw-r--r--   0        0        0     2384 2023-08-07 14:51:51.914556 oplangchain-0.1.0/oplangchain/tools/shell/tool.py
+-rw-r--r--   0        0        0       18 2023-08-07 14:51:51.915554 oplangchain-0.1.0/oplangchain/tools/sleep/__init__.py
+-rw-r--r--   0        0        0     1205 2023-08-07 14:51:51.915554 oplangchain-0.1.0/oplangchain/tools/sleep/tool.py
+-rw-r--r--   0        0        0       44 2023-08-07 14:51:51.916553 oplangchain-0.1.0/oplangchain/tools/spark_sql/__init__.py
+-rw-r--r--   0        0        0      550 2023-08-07 14:51:51.917554 oplangchain-0.1.0/oplangchain/tools/spark_sql/prompt.py
+-rw-r--r--   0        0        0     4512 2023-08-07 14:51:51.917554 oplangchain-0.1.0/oplangchain/tools/spark_sql/tool.py
+-rw-r--r--   0        0        0       49 2023-08-07 14:51:51.918557 oplangchain-0.1.0/oplangchain/tools/sql_database/__init__.py
+-rw-r--r--   0        0        0      597 2023-08-07 14:51:51.918557 oplangchain-0.1.0/oplangchain/tools/sql_database/prompt.py
+-rw-r--r--   0        0        0     4574 2023-08-07 14:51:51.919553 oplangchain-0.1.0/oplangchain/tools/sql_database/tool.py
+-rw-r--r--   0        0        0      167 2023-08-07 14:51:51.919553 oplangchain-0.1.0/oplangchain/tools/steamship_image_generation/__init__.py
+-rw-r--r--   0        0        0     3327 2023-08-07 14:51:51.920553 oplangchain-0.1.0/oplangchain/tools/steamship_image_generation/tool.py
+-rw-r--r--   0        0        0     1395 2023-08-07 14:51:51.920553 oplangchain-0.1.0/oplangchain/tools/steamship_image_generation/utils.py
+-rw-r--r--   0        0        0       51 2023-08-07 14:51:51.921553 oplangchain-0.1.0/oplangchain/tools/vectorstore/__init__.py
+-rw-r--r--   0        0        0     3243 2023-08-07 14:51:51.922557 oplangchain-0.1.0/oplangchain/tools/vectorstore/tool.py
+-rw-r--r--   0        0        0       29 2023-08-07 14:51:51.922557 oplangchain-0.1.0/oplangchain/tools/wikipedia/__init__.py
+-rw-r--r--   0        0        0      849 2023-08-07 14:51:51.923555 oplangchain-0.1.0/oplangchain/tools/wikipedia/tool.py
+-rw-r--r--   0        0        0      146 2023-08-07 14:51:51.924555 oplangchain-0.1.0/oplangchain/tools/wolfram_alpha/__init__.py
+-rw-r--r--   0        0        0      869 2023-08-07 14:51:51.924555 oplangchain-0.1.0/oplangchain/tools/wolfram_alpha/tool.py
+-rw-r--r--   0        0        0        0 2023-08-07 14:51:51.925557 oplangchain-0.1.0/oplangchain/tools/youtube/__init__.py
+-rw-r--r--   0        0        0     1661 2023-08-07 14:51:51.925557 oplangchain-0.1.0/oplangchain/tools/youtube/search.py
+-rw-r--r--   0        0        0      170 2023-08-07 14:51:51.926554 oplangchain-0.1.0/oplangchain/tools/zapier/__init__.py
+-rw-r--r--   0        0        0     1182 2023-08-07 14:51:51.927554 oplangchain-0.1.0/oplangchain/tools/zapier/prompt.py
+-rw-r--r--   0        0        0     7065 2023-08-07 14:51:51.927554 oplangchain-0.1.0/oplangchain/tools/zapier/tool.py
+-rw-r--r--   0        0        0     2868 2023-08-07 14:51:51.928554 oplangchain-0.1.0/oplangchain/utilities/__init__.py
+-rw-r--r--   0        0        0     6386 2023-08-07 14:51:51.928554 oplangchain-0.1.0/oplangchain/utilities/arxiv.py
+-rw-r--r--   0        0        0      274 2023-08-07 14:51:51.929553 oplangchain-0.1.0/oplangchain/utilities/asyncio.py
+-rw-r--r--   0        0        0     2419 2023-08-07 14:51:51.929553 oplangchain-0.1.0/oplangchain/utilities/awslambda.py
+-rw-r--r--   0        0        0     5703 2023-08-07 14:51:51.930559 oplangchain-0.1.0/oplangchain/utilities/bash.py
+-rw-r--r--   0        0        0     2481 2023-08-07 14:51:51.930559 oplangchain-0.1.0/oplangchain/utilities/bibtex.py
+-rw-r--r--   0        0        0     3333 2023-08-07 14:51:51.931554 oplangchain-0.1.0/oplangchain/utilities/bing_search.py
+-rw-r--r--   0        0        0     2326 2023-08-07 14:51:51.931554 oplangchain-0.1.0/oplangchain/utilities/brave_search.py
+-rw-r--r--   0        0        0     7832 2023-08-07 14:51:51.932554 oplangchain-0.1.0/oplangchain/utilities/dataforseo_api_search.py
+-rw-r--r--   0        0        0     3764 2023-08-07 14:51:51.932554 oplangchain-0.1.0/oplangchain/utilities/duckduckgo_search.py
+-rw-r--r--   0        0        0    11594 2023-08-07 14:51:51.933556 oplangchain-0.1.0/oplangchain/utilities/github.py
+-rw-r--r--   0        0        0     1836 2023-08-07 14:51:51.933556 oplangchain-0.1.0/oplangchain/utilities/golden_query.py
+-rw-r--r--   0        0        0     4065 2023-08-07 14:51:51.934557 oplangchain-0.1.0/oplangchain/utilities/google_places_api.py
+-rw-r--r--   0        0        0     5094 2023-08-07 14:51:51.934557 oplangchain-0.1.0/oplangchain/utilities/google_search.py
+-rw-r--r--   0        0        0     6503 2023-08-07 14:51:51.935556 oplangchain-0.1.0/oplangchain/utilities/google_serper.py
+-rw-r--r--   0        0        0     1885 2023-08-07 14:51:51.935556 oplangchain-0.1.0/oplangchain/utilities/graphql.py
+-rw-r--r--   0        0        0     6173 2023-08-07 14:51:51.936557 oplangchain-0.1.0/oplangchain/utilities/jira.py
+-rw-r--r--   0        0        0     1972 2023-08-07 14:51:51.937557 oplangchain-0.1.0/oplangchain/utilities/loading.py
+-rw-r--r--   0        0        0     2642 2023-08-07 14:51:51.937557 oplangchain-0.1.0/oplangchain/utilities/max_compute.py
+-rw-r--r--   0        0        0     6705 2023-08-07 14:51:51.938555 oplangchain-0.1.0/oplangchain/utilities/metaphor_search.py
+-rw-r--r--   0        0        0    10299 2023-08-07 14:51:51.939558 oplangchain-0.1.0/oplangchain/utilities/openapi.py
+-rw-r--r--   0        0        0     2440 2023-08-07 14:51:51.940557 oplangchain-0.1.0/oplangchain/utilities/openweathermap.py
+-rw-r--r--   0        0        0     2198 2023-08-07 14:51:51.940557 oplangchain-0.1.0/oplangchain/utilities/portkey.py
+-rw-r--r--   0        0        0    11237 2023-08-07 14:51:51.941556 oplangchain-0.1.0/oplangchain/utilities/powerbi.py
+-rw-r--r--   0        0        0     5627 2023-08-07 14:51:51.942556 oplangchain-0.1.0/oplangchain/utilities/pupmed.py
+-rw-r--r--   0        0        0     2141 2023-08-07 14:51:51.942556 oplangchain-0.1.0/oplangchain/utilities/python.py
+-rw-r--r--   0        0        0     5435 2023-08-07 14:51:51.943556 oplangchain-0.1.0/oplangchain/utilities/redis.py
+-rw-r--r--   0        0        0     7120 2023-08-07 14:51:51.944557 oplangchain-0.1.0/oplangchain/utilities/requests.py
+-rw-r--r--   0        0        0     2198 2023-08-07 14:51:51.944557 oplangchain-0.1.0/oplangchain/utilities/scenexplain.py
+-rw-r--r--   0        0        0    16529 2023-08-07 14:51:51.945556 oplangchain-0.1.0/oplangchain/utilities/searx_search.py
+-rw-r--r--   0        0        0     6025 2023-08-07 14:51:51.945556 oplangchain-0.1.0/oplangchain/utilities/serpapi.py
+-rw-r--r--   0        0        0     6964 2023-08-07 14:51:51.945556 oplangchain-0.1.0/oplangchain/utilities/spark_sql.py
+-rw-r--r--   0        0        0    18263 2023-08-07 14:51:51.946554 oplangchain-0.1.0/oplangchain/utilities/sql_database.py
+-rw-r--r--   0        0        0     3409 2023-08-07 14:51:51.946554 oplangchain-0.1.0/oplangchain/utilities/twilio.py
+-rw-r--r--   0        0        0     1457 2023-08-07 14:51:51.947558 oplangchain-0.1.0/oplangchain/utilities/vertexai.py
+-rw-r--r--   0        0        0     3920 2023-08-07 14:51:51.947558 oplangchain-0.1.0/oplangchain/utilities/wikipedia.py
+-rw-r--r--   0        0        0     1989 2023-08-07 14:51:51.948557 oplangchain-0.1.0/oplangchain/utilities/wolfram_alpha.py
+-rw-r--r--   0        0        0    11560 2023-08-07 14:51:51.948557 oplangchain-0.1.0/oplangchain/utilities/zapier.py
+-rw-r--r--   0        0        0     1149 2023-08-07 14:51:51.949556 oplangchain-0.1.0/oplangchain/utils/__init__.py
+-rw-r--r--   0        0        0      873 2023-08-07 14:51:51.950555 oplangchain-0.1.0/oplangchain/utils/env.py
+-rw-r--r--   0        0        0     1237 2023-08-07 14:51:51.950555 oplangchain-0.1.0/oplangchain/utils/formatting.py
+-rw-r--r--   0        0        0     1289 2023-08-07 14:51:51.951556 oplangchain-0.1.0/oplangchain/utils/input.py
+-rw-r--r--   0        0        0     2016 2023-08-07 14:51:51.952556 oplangchain-0.1.0/oplangchain/utils/math.py
+-rw-r--r--   0        0        0      908 2023-08-07 14:51:51.952556 oplangchain-0.1.0/oplangchain/utils/strings.py
+-rw-r--r--   0        0        0     5606 2023-08-07 14:51:51.953554 oplangchain-0.1.0/oplangchain/utils/utils.py
+-rw-r--r--   0        0        0     4003 2023-08-07 14:51:51.953554 oplangchain-0.1.0/oplangchain/vectorstores/__init__.py
+-rw-r--r--   0        0        0     2025 2023-08-07 14:51:51.954555 oplangchain-0.1.0/oplangchain/vectorstores/_pgvector_data_models.py
+-rw-r--r--   0        0        0    13535 2023-08-07 14:51:51.955557 oplangchain-0.1.0/oplangchain/vectorstores/alibabacloud_opensearch.py
+-rw-r--r--   0        0        0    15792 2023-08-07 14:51:51.955557 oplangchain-0.1.0/oplangchain/vectorstores/analyticdb.py
+-rw-r--r--   0        0        0    16575 2023-08-07 14:51:51.956557 oplangchain-0.1.0/oplangchain/vectorstores/annoy.py
+-rw-r--r--   0        0        0    12133 2023-08-07 14:51:51.956557 oplangchain-0.1.0/oplangchain/vectorstores/atlas.py
+-rw-r--r--   0        0        0    21220 2023-08-07 14:51:51.957556 oplangchain-0.1.0/oplangchain/vectorstores/awadb.py
+-rw-r--r--   0        0        0    20714 2023-08-07 14:51:51.957556 oplangchain-0.1.0/oplangchain/vectorstores/azuresearch.py
+-rw-r--r--   0        0        0    22433 2023-08-07 14:51:51.958557 oplangchain-0.1.0/oplangchain/vectorstores/base.py
+-rw-r--r--   0        0        0    13392 2023-08-07 14:51:51.958557 oplangchain-0.1.0/oplangchain/vectorstores/cassandra.py
+-rw-r--r--   0        0        0    23808 2023-08-07 14:51:51.959557 oplangchain-0.1.0/oplangchain/vectorstores/chroma.py
+-rw-r--r--   0        0        0    12729 2023-08-07 14:51:51.959557 oplangchain-0.1.0/oplangchain/vectorstores/clarifai.py
+-rw-r--r--   0        0        0    17811 2023-08-07 14:51:51.960557 oplangchain-0.1.0/oplangchain/vectorstores/clickhouse.py
+-rw-r--r--   0        0        0    34968 2023-08-07 14:51:51.961556 oplangchain-0.1.0/oplangchain/vectorstores/deeplake.py
+-rw-r--r--   0        0        0      216 2023-08-07 14:51:51.961556 oplangchain-0.1.0/oplangchain/vectorstores/docarray/__init__.py
+-rw-r--r--   0        0        0     6871 2023-08-07 14:51:51.962554 oplangchain-0.1.0/oplangchain/vectorstores/docarray/base.py
+-rw-r--r--   0        0        0     4057 2023-08-07 14:51:51.962554 oplangchain-0.1.0/oplangchain/vectorstores/docarray/hnsw.py
+-rw-r--r--   0        0        0     2411 2023-08-07 14:51:51.963557 oplangchain-0.1.0/oplangchain/vectorstores/docarray/in_memory.py
+-rw-r--r--   0        0        0    27775 2023-08-07 14:51:51.963557 oplangchain-0.1.0/oplangchain/vectorstores/elastic_vector_search.py
+-rw-r--r--   0        0        0    29115 2023-08-07 14:51:51.964557 oplangchain-0.1.0/oplangchain/vectorstores/faiss.py
+-rw-r--r--   0        0        0    16399 2023-08-07 14:51:51.965557 oplangchain-0.1.0/oplangchain/vectorstores/hologres.py
+-rw-r--r--   0        0        0     4236 2023-08-07 14:51:51.965557 oplangchain-0.1.0/oplangchain/vectorstores/lancedb.py
+-rw-r--r--   0        0        0    17152 2023-08-07 14:51:51.966557 oplangchain-0.1.0/oplangchain/vectorstores/marqo.py
+-rw-r--r--   0        0        0    15176 2023-08-07 14:51:51.966557 oplangchain-0.1.0/oplangchain/vectorstores/matching_engine.py
+-rw-r--r--   0        0        0    10421 2023-08-07 14:51:51.967557 oplangchain-0.1.0/oplangchain/vectorstores/meilisearch.py
+-rw-r--r--   0        0        0    31468 2023-08-07 14:51:51.967557 oplangchain-0.1.0/oplangchain/vectorstores/milvus.py
+-rw-r--r--   0        0        0    12345 2023-08-07 14:51:51.968557 oplangchain-0.1.0/oplangchain/vectorstores/mongodb_atlas.py
+-rw-r--r--   0        0        0    16539 2023-08-07 14:51:51.968557 oplangchain-0.1.0/oplangchain/vectorstores/myscale.py
+-rw-r--r--   0        0        0    27686 2023-08-07 14:51:51.969557 oplangchain-0.1.0/oplangchain/vectorstores/opensearch_vector_search.py
+-rw-r--r--   0        0        0    17344 2023-08-07 14:51:51.969557 oplangchain-0.1.0/oplangchain/vectorstores/pgembedding.py
+-rw-r--r--   0        0        0    21251 2023-08-07 14:51:51.970556 oplangchain-0.1.0/oplangchain/vectorstores/pgvector.py
+-rw-r--r--   0        0        0    14905 2023-08-07 14:51:51.971554 oplangchain-0.1.0/oplangchain/vectorstores/pinecone.py
+-rw-r--r--   0        0        0    68527 2023-08-07 14:51:51.971554 oplangchain-0.1.0/oplangchain/vectorstores/qdrant.py
+-rw-r--r--   0        0        0    23138 2023-08-07 14:51:51.972558 oplangchain-0.1.0/oplangchain/vectorstores/redis.py
+-rw-r--r--   0        0        0    12186 2023-08-07 14:51:51.972558 oplangchain-0.1.0/oplangchain/vectorstores/rocksetdb.py
+-rw-r--r--   0        0        0    19511 2023-08-07 14:51:51.973555 oplangchain-0.1.0/oplangchain/vectorstores/scann.py
+-rw-r--r--   0        0        0    18252 2023-08-07 14:51:51.973555 oplangchain-0.1.0/oplangchain/vectorstores/singlestoredb.py
+-rw-r--r--   0        0        0    12385 2023-08-07 14:51:51.974557 oplangchain-0.1.0/oplangchain/vectorstores/sklearn.py
+-rw-r--r--   0        0        0    17219 2023-08-07 14:51:51.974557 oplangchain-0.1.0/oplangchain/vectorstores/starrocks.py
+-rw-r--r--   0        0        0    14233 2023-08-07 14:51:51.975557 oplangchain-0.1.0/oplangchain/vectorstores/supabase.py
+-rw-r--r--   0        0        0     8878 2023-08-07 14:51:51.976555 oplangchain-0.1.0/oplangchain/vectorstores/tair.py
+-rw-r--r--   0        0        0     4878 2023-08-07 14:51:51.977554 oplangchain-0.1.0/oplangchain/vectorstores/tigris.py
+-rw-r--r--   0        0        0     9728 2023-08-07 14:51:51.977554 oplangchain-0.1.0/oplangchain/vectorstores/typesense.py
+-rw-r--r--   0        0        0     1790 2023-08-07 14:51:51.978555 oplangchain-0.1.0/oplangchain/vectorstores/utils.py
+-rw-r--r--   0        0        0    15857 2023-08-07 14:51:51.978555 oplangchain-0.1.0/oplangchain/vectorstores/vectara.py
+-rw-r--r--   0        0        0    16875 2023-08-07 14:51:51.979557 oplangchain-0.1.0/oplangchain/vectorstores/weaviate.py
+-rw-r--r--   0        0        0     7559 2023-08-07 14:51:51.980557 oplangchain-0.1.0/oplangchain/vectorstores/zilliz.py
+-rw-r--r--   0        0        0    13280 2023-08-07 16:53:14.384679 oplangchain-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5724 2023-08-07 14:51:51.062474 oplangchain-0.1.0/README.md
+-rw-r--r--   0        0        0    14928 1970-01-01 00:00:00.000000 oplangchain-0.1.0/PKG-INFO
```

### Comparing `oplangchain-0.0.255/oplangchain/__init__.py` & `oplangchain-0.1.0/oplangchain/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/__init__.py` & `oplangchain-0.1.0/oplangchain/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent.py` & `oplangchain-0.1.0/oplangchain/agents/agent.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_iterator.py` & `oplangchain-0.1.0/oplangchain/agents/agent_iterator.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/__init__.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/amadeus/toolkit.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/amadeus/toolkit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/azure_cognitive_services.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/azure_cognitive_services.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/conversational_retrieval/openai_functions.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/conversational_retrieval/openai_functions.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/conversational_retrieval/tool.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/conversational_retrieval/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/csv/base.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/csv/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/file_management/toolkit.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/file_management/toolkit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/github/toolkit.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/github/toolkit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/gmail/toolkit.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/gmail/toolkit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/jira/toolkit.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/jira/toolkit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/json/base.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/json/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/json/prompt.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/json/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/json/toolkit.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/json/toolkit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/multion/toolkit.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/multion/toolkit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/nla/tool.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/nla/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/nla/toolkit.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/nla/toolkit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/office365/toolkit.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/office365/toolkit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/openapi/base.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/openapi/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/openapi/planner.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/openapi/planner.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/openapi/planner_prompt.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/openapi/planner_prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/openapi/prompt.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/openapi/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/openapi/spec.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/openapi/spec.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/openapi/toolkit.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/openapi/toolkit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/pandas/base.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/pandas/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/pandas/prompt.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/pandas/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/playwright/toolkit.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/playwright/toolkit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/powerbi/base.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/powerbi/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/powerbi/chat_base.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/powerbi/chat_base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/powerbi/prompt.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/powerbi/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/powerbi/toolkit.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/powerbi/toolkit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/python/base.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/python/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/python/prompt.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/python/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/spark/base.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/spark/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/spark_sql/base.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/spark_sql/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/spark_sql/prompt.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/spark_sql/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/spark_sql/toolkit.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/spark_sql/toolkit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/sql/base.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/sql/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/sql/prompt.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/sql/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/sql/toolkit.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/sql/toolkit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/vectorstore/base.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/vectorstore/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/vectorstore/prompt.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/vectorstore/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/vectorstore/toolkit.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/vectorstore/toolkit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/xorbits/base.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/xorbits/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/xorbits/prompt.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/xorbits/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_toolkits/zapier/toolkit.py` & `oplangchain-0.1.0/oplangchain/agents/agent_toolkits/zapier/toolkit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/agent_types.py` & `oplangchain-0.1.0/oplangchain/agents/agent_types.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/chat/base.py` & `oplangchain-0.1.0/oplangchain/agents/chat/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/chat/output_parser.py` & `oplangchain-0.1.0/oplangchain/agents/chat/output_parser.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/chat/prompt.py` & `oplangchain-0.1.0/oplangchain/agents/chat/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/conversational/base.py` & `oplangchain-0.1.0/oplangchain/agents/conversational/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/conversational/output_parser.py` & `oplangchain-0.1.0/oplangchain/agents/conversational/output_parser.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/conversational/prompt.py` & `oplangchain-0.1.0/oplangchain/agents/conversational/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/conversational_chat/base.py` & `oplangchain-0.1.0/oplangchain/agents/conversational_chat/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/conversational_chat/output_parser.py` & `oplangchain-0.1.0/oplangchain/agents/conversational_chat/output_parser.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/conversational_chat/prompt.py` & `oplangchain-0.1.0/oplangchain/agents/conversational_chat/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/initialize.py` & `oplangchain-0.1.0/oplangchain/agents/initialize.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/load_tools.py` & `oplangchain-0.1.0/oplangchain/agents/load_tools.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/loading.py` & `oplangchain-0.1.0/oplangchain/agents/loading.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/mrkl/base.py` & `oplangchain-0.1.0/oplangchain/agents/mrkl/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/mrkl/output_parser.py` & `oplangchain-0.1.0/oplangchain/agents/mrkl/output_parser.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/mrkl/prompt.py` & `oplangchain-0.1.0/oplangchain/agents/mrkl/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/openai_functions_agent/agent_token_buffer_memory.py` & `oplangchain-0.1.0/oplangchain/agents/openai_functions_agent/agent_token_buffer_memory.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/openai_functions_agent/base.py` & `oplangchain-0.1.0/oplangchain/agents/openai_functions_agent/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/openai_functions_multi_agent/base.py` & `oplangchain-0.1.0/oplangchain/agents/openai_functions_multi_agent/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/react/base.py` & `oplangchain-0.1.0/oplangchain/agents/react/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/react/output_parser.py` & `oplangchain-0.1.0/oplangchain/agents/react/output_parser.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/react/textworld_prompt.py` & `oplangchain-0.1.0/oplangchain/agents/react/textworld_prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/react/wiki_prompt.py` & `oplangchain-0.1.0/oplangchain/agents/react/wiki_prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/schema.py` & `oplangchain-0.1.0/oplangchain/agents/schema.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/self_ask_with_search/base.py` & `oplangchain-0.1.0/oplangchain/agents/self_ask_with_search/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/self_ask_with_search/output_parser.py` & `oplangchain-0.1.0/oplangchain/agents/self_ask_with_search/output_parser.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/self_ask_with_search/prompt.py` & `oplangchain-0.1.0/oplangchain/agents/self_ask_with_search/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/structured_chat/base.py` & `oplangchain-0.1.0/oplangchain/agents/structured_chat/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/structured_chat/output_parser.py` & `oplangchain-0.1.0/oplangchain/agents/structured_chat/output_parser.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/structured_chat/prompt.py` & `oplangchain-0.1.0/oplangchain/agents/structured_chat/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/tools.py` & `oplangchain-0.1.0/oplangchain/agents/tools.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/types.py` & `oplangchain-0.1.0/oplangchain/agents/types.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/xml/base.py` & `oplangchain-0.1.0/oplangchain/agents/xml/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/agents/xml/prompt.py` & `oplangchain-0.1.0/oplangchain/agents/xml/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/cache.py` & `oplangchain-0.1.0/oplangchain/cache.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/__init__.py` & `oplangchain-0.1.0/oplangchain/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/aim_callback.py` & `oplangchain-0.1.0/oplangchain/callbacks/aim_callback.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/argilla_callback.py` & `oplangchain-0.1.0/oplangchain/callbacks/argilla_callback.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/arize_callback.py` & `oplangchain-0.1.0/oplangchain/callbacks/arize_callback.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/arthur_callback.py` & `oplangchain-0.1.0/oplangchain/callbacks/arthur_callback.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/base.py` & `oplangchain-0.1.0/oplangchain/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/clearml_callback.py` & `oplangchain-0.1.0/oplangchain/callbacks/clearml_callback.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/comet_ml_callback.py` & `oplangchain-0.1.0/oplangchain/callbacks/comet_ml_callback.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/context_callback.py` & `oplangchain-0.1.0/oplangchain/callbacks/context_callback.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/file.py` & `oplangchain-0.1.0/oplangchain/callbacks/file.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/flyte_callback.py` & `oplangchain-0.1.0/oplangchain/callbacks/flyte_callback.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/human.py` & `oplangchain-0.1.0/oplangchain/callbacks/human.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/infino_callback.py` & `oplangchain-0.1.0/oplangchain/callbacks/infino_callback.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/manager.py` & `oplangchain-0.1.0/oplangchain/callbacks/manager.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/mlflow_callback.py` & `oplangchain-0.1.0/oplangchain/callbacks/mlflow_callback.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/openai_info.py` & `oplangchain-0.1.0/oplangchain/callbacks/openai_info.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/promptlayer_callback.py` & `oplangchain-0.1.0/oplangchain/callbacks/promptlayer_callback.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/sagemaker_callback.py` & `oplangchain-0.1.0/oplangchain/callbacks/sagemaker_callback.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/stdout.py` & `oplangchain-0.1.0/oplangchain/callbacks/stdout.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/streaming_aiter.py` & `oplangchain-0.1.0/oplangchain/callbacks/streaming_aiter.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/streaming_aiter_final_only.py` & `oplangchain-0.1.0/oplangchain/callbacks/streaming_aiter_final_only.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/streaming_stdout.py` & `oplangchain-0.1.0/oplangchain/callbacks/streaming_stdout.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/streaming_stdout_final_only.py` & `oplangchain-0.1.0/oplangchain/callbacks/streaming_stdout_final_only.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/streamlit/__init__.py` & `oplangchain-0.1.0/oplangchain/callbacks/streamlit/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/streamlit/mutable_expander.py` & `oplangchain-0.1.0/oplangchain/callbacks/streamlit/mutable_expander.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/streamlit/streamlit_callback_handler.py` & `oplangchain-0.1.0/oplangchain/callbacks/streamlit/streamlit_callback_handler.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/tracers/base.py` & `oplangchain-0.1.0/oplangchain/callbacks/tracers/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/tracers/evaluation.py` & `oplangchain-0.1.0/oplangchain/callbacks/tracers/evaluation.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/tracers/langchain.py` & `oplangchain-0.1.0/oplangchain/callbacks/tracers/langchain.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/tracers/langchain_v1.py` & `oplangchain-0.1.0/oplangchain/callbacks/tracers/langchain_v1.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/tracers/run_collector.py` & `oplangchain-0.1.0/oplangchain/callbacks/tracers/run_collector.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/tracers/schemas.py` & `oplangchain-0.1.0/oplangchain/callbacks/tracers/schemas.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/tracers/stdout.py` & `oplangchain-0.1.0/oplangchain/callbacks/tracers/stdout.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/tracers/wandb.py` & `oplangchain-0.1.0/oplangchain/callbacks/tracers/wandb.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/utils.py` & `oplangchain-0.1.0/oplangchain/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/wandb_callback.py` & `oplangchain-0.1.0/oplangchain/callbacks/wandb_callback.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/callbacks/whylabs_callback.py` & `oplangchain-0.1.0/oplangchain/callbacks/whylabs_callback.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/__init__.py` & `oplangchain-0.1.0/oplangchain/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/api/base.py` & `oplangchain-0.1.0/oplangchain/chains/api/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/api/news_docs.py` & `oplangchain-0.1.0/oplangchain/chains/api/news_docs.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/api/open_meteo_docs.py` & `oplangchain-0.1.0/oplangchain/chains/api/open_meteo_docs.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/api/openapi/chain.py` & `oplangchain-0.1.0/oplangchain/chains/api/openapi/chain.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/api/openapi/prompts.py` & `oplangchain-0.1.0/oplangchain/chains/api/openapi/prompts.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/api/openapi/requests_chain.py` & `oplangchain-0.1.0/oplangchain/chains/api/openapi/requests_chain.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/api/openapi/response_chain.py` & `oplangchain-0.1.0/oplangchain/chains/api/openapi/response_chain.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/api/podcast_docs.py` & `oplangchain-0.1.0/oplangchain/chains/api/podcast_docs.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/api/prompt.py` & `oplangchain-0.1.0/oplangchain/chains/api/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/api/tmdb_docs.py` & `oplangchain-0.1.0/oplangchain/chains/api/tmdb_docs.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/base.py` & `oplangchain-0.1.0/oplangchain/chains/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/chat_vector_db/prompts.py` & `oplangchain-0.1.0/oplangchain/chains/chat_vector_db/prompts.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/combine_documents/base.py` & `oplangchain-0.1.0/oplangchain/chains/combine_documents/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/combine_documents/map_reduce.py` & `oplangchain-0.1.0/oplangchain/chains/combine_documents/map_reduce.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/combine_documents/map_rerank.py` & `oplangchain-0.1.0/oplangchain/chains/combine_documents/map_rerank.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/combine_documents/reduce.py` & `oplangchain-0.1.0/oplangchain/chains/combine_documents/reduce.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/combine_documents/refine.py` & `oplangchain-0.1.0/oplangchain/chains/combine_documents/refine.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/combine_documents/stuff.py` & `oplangchain-0.1.0/oplangchain/chains/combine_documents/stuff.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/constitutional_ai/base.py` & `oplangchain-0.1.0/oplangchain/chains/constitutional_ai/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/constitutional_ai/principles.py` & `oplangchain-0.1.0/oplangchain/chains/constitutional_ai/principles.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/constitutional_ai/prompts.py` & `oplangchain-0.1.0/oplangchain/chains/constitutional_ai/prompts.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/conversation/base.py` & `oplangchain-0.1.0/oplangchain/chains/conversation/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/conversation/memory.py` & `oplangchain-0.1.0/oplangchain/chains/conversation/memory.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/conversation/prompt.py` & `oplangchain-0.1.0/oplangchain/chains/conversation/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/conversational_retrieval/base.py` & `oplangchain-0.1.0/oplangchain/chains/conversational_retrieval/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/conversational_retrieval/prompts.py` & `oplangchain-0.1.0/oplangchain/chains/conversational_retrieval/prompts.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/elasticsearch_database/base.py` & `oplangchain-0.1.0/oplangchain/chains/elasticsearch_database/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/elasticsearch_database/prompts.py` & `oplangchain-0.1.0/oplangchain/chains/elasticsearch_database/prompts.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/example_generator.py` & `oplangchain-0.1.0/oplangchain/chains/example_generator.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/flare/base.py` & `oplangchain-0.1.0/oplangchain/chains/flare/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/flare/prompts.py` & `oplangchain-0.1.0/oplangchain/chains/flare/prompts.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/graph_qa/arangodb.py` & `oplangchain-0.1.0/oplangchain/chains/graph_qa/arangodb.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/graph_qa/base.py` & `oplangchain-0.1.0/oplangchain/chains/graph_qa/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/graph_qa/cypher.py` & `oplangchain-0.1.0/oplangchain/chains/graph_qa/cypher.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/graph_qa/hugegraph.py` & `oplangchain-0.1.0/oplangchain/chains/graph_qa/hugegraph.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/graph_qa/kuzu.py` & `oplangchain-0.1.0/oplangchain/chains/graph_qa/kuzu.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/graph_qa/nebulagraph.py` & `oplangchain-0.1.0/oplangchain/chains/graph_qa/nebulagraph.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/graph_qa/neptune_cypher.py` & `oplangchain-0.1.0/oplangchain/chains/graph_qa/neptune_cypher.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/graph_qa/prompts.py` & `oplangchain-0.1.0/oplangchain/chains/graph_qa/prompts.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/graph_qa/sparql.py` & `oplangchain-0.1.0/oplangchain/chains/graph_qa/sparql.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/hyde/base.py` & `oplangchain-0.1.0/oplangchain/chains/hyde/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/hyde/prompts.py` & `oplangchain-0.1.0/oplangchain/chains/hyde/prompts.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/llm.py` & `oplangchain-0.1.0/oplangchain/chains/llm.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/llm_bash/base.py` & `oplangchain-0.1.0/oplangchain/chains/llm_bash/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/llm_bash/prompt.py` & `oplangchain-0.1.0/oplangchain/chains/llm_bash/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/llm_checker/base.py` & `oplangchain-0.1.0/oplangchain/chains/llm_checker/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/llm_checker/prompt.py` & `oplangchain-0.1.0/oplangchain/chains/llm_checker/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/llm_math/base.py` & `oplangchain-0.1.0/oplangchain/chains/llm_math/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/llm_math/prompt.py` & `oplangchain-0.1.0/oplangchain/chains/llm_math/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/llm_requests.py` & `oplangchain-0.1.0/oplangchain/chains/llm_requests.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/llm_summarization_checker/base.py` & `oplangchain-0.1.0/oplangchain/chains/llm_summarization_checker/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/llm_summarization_checker/prompts/are_all_true_prompt.txt` & `oplangchain-0.1.0/oplangchain/chains/llm_summarization_checker/prompts/are_all_true_prompt.txt`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/llm_symbolic_math/base.py` & `oplangchain-0.1.0/oplangchain/chains/llm_symbolic_math/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/llm_symbolic_math/prompt.py` & `oplangchain-0.1.0/oplangchain/chains/llm_symbolic_math/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/loading.py` & `oplangchain-0.1.0/oplangchain/chains/loading.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/mapreduce.py` & `oplangchain-0.1.0/oplangchain/chains/mapreduce.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/moderation.py` & `oplangchain-0.1.0/oplangchain/chains/moderation.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/natbot/base.py` & `oplangchain-0.1.0/oplangchain/chains/natbot/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/natbot/crawler.py` & `oplangchain-0.1.0/oplangchain/chains/natbot/crawler.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/natbot/prompt.py` & `oplangchain-0.1.0/oplangchain/chains/natbot/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/openai_functions/__init__.py` & `oplangchain-0.1.0/oplangchain/chains/openai_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/openai_functions/base.py` & `oplangchain-0.1.0/oplangchain/chains/openai_functions/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/openai_functions/citation_fuzzy_match.py` & `oplangchain-0.1.0/oplangchain/chains/openai_functions/citation_fuzzy_match.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/openai_functions/extraction.py` & `oplangchain-0.1.0/oplangchain/chains/openai_functions/extraction.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/openai_functions/openapi.py` & `oplangchain-0.1.0/oplangchain/chains/openai_functions/openapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,14 +240,15 @@
     request_chain: Optional[Chain] = None,
     llm_chain_kwargs: Optional[Dict] = None,
     verbose: bool = False,
     headers: Optional[Dict] = None,
     params: Optional[Dict] = None,
     **kwargs: Any,
 ) -> SequentialChain:
+    print("STARTING")
     """Create a chain for querying an API from a OpenAPI spec.
 
     Args:
         spec: OpenAPISpec or url/file/text string corresponding to one.
         llm: language model, should be an OpenAI function-calling model, e.g.
             `ChatOpenAI(model="gpt-3.5-turbo-0613")`.
         prompt: Main prompt template to use.
```

### Comparing `oplangchain-0.0.255/oplangchain/chains/openai_functions/qa_with_structure.py` & `oplangchain-0.1.0/oplangchain/chains/openai_functions/qa_with_structure.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/openai_functions/tagging.py` & `oplangchain-0.1.0/oplangchain/chains/openai_functions/tagging.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/openai_functions/utils.py` & `oplangchain-0.1.0/oplangchain/chains/openai_functions/utils.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/prompt_selector.py` & `oplangchain-0.1.0/oplangchain/chains/prompt_selector.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/qa_generation/base.py` & `oplangchain-0.1.0/oplangchain/chains/qa_generation/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/qa_generation/prompt.py` & `oplangchain-0.1.0/oplangchain/chains/qa_generation/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/qa_with_sources/base.py` & `oplangchain-0.1.0/oplangchain/chains/qa_with_sources/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/qa_with_sources/loading.py` & `oplangchain-0.1.0/oplangchain/chains/qa_with_sources/loading.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/qa_with_sources/map_reduce_prompt.py` & `oplangchain-0.1.0/oplangchain/chains/qa_with_sources/map_reduce_prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/qa_with_sources/refine_prompts.py` & `oplangchain-0.1.0/oplangchain/chains/qa_with_sources/refine_prompts.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/qa_with_sources/retrieval.py` & `oplangchain-0.1.0/oplangchain/chains/qa_with_sources/retrieval.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/qa_with_sources/stuff_prompt.py` & `oplangchain-0.1.0/oplangchain/chains/qa_with_sources/stuff_prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/qa_with_sources/vector_db.py` & `oplangchain-0.1.0/oplangchain/chains/qa_with_sources/vector_db.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/query_constructor/base.py` & `oplangchain-0.1.0/oplangchain/chains/query_constructor/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/query_constructor/ir.py` & `oplangchain-0.1.0/oplangchain/chains/query_constructor/ir.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/query_constructor/parser.py` & `oplangchain-0.1.0/oplangchain/chains/query_constructor/parser.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/query_constructor/prompt.py` & `oplangchain-0.1.0/oplangchain/chains/query_constructor/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/question_answering/__init__.py` & `oplangchain-0.1.0/oplangchain/chains/question_answering/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/question_answering/map_reduce_prompt.py` & `oplangchain-0.1.0/oplangchain/chains/question_answering/map_reduce_prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/question_answering/map_rerank_prompt.py` & `oplangchain-0.1.0/oplangchain/chains/question_answering/map_rerank_prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/question_answering/refine_prompts.py` & `oplangchain-0.1.0/oplangchain/chains/question_answering/refine_prompts.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/question_answering/stuff_prompt.py` & `oplangchain-0.1.0/oplangchain/chains/question_answering/stuff_prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/retrieval_qa/base.py` & `oplangchain-0.1.0/oplangchain/chains/retrieval_qa/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/router/base.py` & `oplangchain-0.1.0/oplangchain/chains/router/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/router/embedding_router.py` & `oplangchain-0.1.0/oplangchain/chains/router/embedding_router.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/router/llm_router.py` & `oplangchain-0.1.0/oplangchain/chains/router/llm_router.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/router/multi_prompt.py` & `oplangchain-0.1.0/oplangchain/chains/router/multi_prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/router/multi_prompt_prompt.py` & `oplangchain-0.1.0/oplangchain/chains/router/multi_prompt_prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/router/multi_retrieval_prompt.py` & `oplangchain-0.1.0/oplangchain/chains/router/multi_retrieval_prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/router/multi_retrieval_qa.py` & `oplangchain-0.1.0/oplangchain/chains/router/multi_retrieval_qa.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/sequential.py` & `oplangchain-0.1.0/oplangchain/chains/sequential.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/sql_database/prompt.py` & `oplangchain-0.1.0/oplangchain/chains/sql_database/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/sql_database/query.py` & `oplangchain-0.1.0/oplangchain/chains/sql_database/query.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/summarize/__init__.py` & `oplangchain-0.1.0/oplangchain/chains/summarize/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/summarize/refine_prompts.py` & `oplangchain-0.1.0/oplangchain/chains/summarize/refine_prompts.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chains/transform.py` & `oplangchain-0.1.0/oplangchain/chains/transform.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chat_models/__init__.py` & `oplangchain-0.1.0/oplangchain/chat_models/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chat_models/anthropic.py` & `oplangchain-0.1.0/oplangchain/chat_models/anthropic.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chat_models/azure_openai.py` & `oplangchain-0.1.0/oplangchain/chat_models/azure_openai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chat_models/azureml_endpoint.py` & `oplangchain-0.1.0/oplangchain/chat_models/azureml_endpoint.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chat_models/base.py` & `oplangchain-0.1.0/oplangchain/chat_models/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chat_models/fake.py` & `oplangchain-0.1.0/oplangchain/chat_models/fake.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chat_models/google_palm.py` & `oplangchain-0.1.0/oplangchain/chat_models/google_palm.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chat_models/human.py` & `oplangchain-0.1.0/oplangchain/chat_models/human.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chat_models/jinachat.py` & `oplangchain-0.1.0/oplangchain/chat_models/jinachat.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chat_models/mlflow_ai_gateway.py` & `oplangchain-0.1.0/oplangchain/chat_models/mlflow_ai_gateway.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chat_models/openai.py` & `oplangchain-0.1.0/oplangchain/chat_models/openai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chat_models/promptlayer_openai.py` & `oplangchain-0.1.0/oplangchain/chat_models/promptlayer_openai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/chat_models/vertexai.py` & `oplangchain-0.1.0/oplangchain/chat_models/vertexai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/docker-compose.yaml` & `oplangchain-0.1.0/oplangchain/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/docstore/__init__.py` & `oplangchain-0.1.0/oplangchain/docstore/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/docstore/arbitrary_fn.py` & `oplangchain-0.1.0/oplangchain/docstore/arbitrary_fn.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/docstore/base.py` & `oplangchain-0.1.0/oplangchain/docstore/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/docstore/in_memory.py` & `oplangchain-0.1.0/oplangchain/docstore/in_memory.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/docstore/wikipedia.py` & `oplangchain-0.1.0/oplangchain/docstore/wikipedia.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/__init__.py` & `oplangchain-0.1.0/oplangchain/document_loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/acreom.py` & `oplangchain-0.1.0/oplangchain/document_loaders/acreom.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/airbyte_json.py` & `oplangchain-0.1.0/oplangchain/document_loaders/airbyte_json.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/airtable.py` & `oplangchain-0.1.0/oplangchain/document_loaders/airtable.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/apify_dataset.py` & `oplangchain-0.1.0/oplangchain/document_loaders/apify_dataset.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/arxiv.py` & `oplangchain-0.1.0/oplangchain/document_loaders/arxiv.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/async_html.py` & `oplangchain-0.1.0/oplangchain/document_loaders/async_html.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/azlyrics.py` & `oplangchain-0.1.0/oplangchain/document_loaders/azlyrics.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/azure_blob_storage_container.py` & `oplangchain-0.1.0/oplangchain/document_loaders/azure_blob_storage_container.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/azure_blob_storage_file.py` & `oplangchain-0.1.0/oplangchain/document_loaders/azure_blob_storage_file.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/base.py` & `oplangchain-0.1.0/oplangchain/document_loaders/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/bibtex.py` & `oplangchain-0.1.0/oplangchain/document_loaders/bibtex.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/bigquery.py` & `oplangchain-0.1.0/oplangchain/document_loaders/bigquery.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/bilibili.py` & `oplangchain-0.1.0/oplangchain/document_loaders/bilibili.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/blackboard.py` & `oplangchain-0.1.0/oplangchain/document_loaders/blackboard.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/blob_loaders/file_system.py` & `oplangchain-0.1.0/oplangchain/document_loaders/blob_loaders/file_system.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/blob_loaders/schema.py` & `oplangchain-0.1.0/oplangchain/document_loaders/blob_loaders/schema.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/blob_loaders/youtube_audio.py` & `oplangchain-0.1.0/oplangchain/document_loaders/blob_loaders/youtube_audio.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/blockchain.py` & `oplangchain-0.1.0/oplangchain/document_loaders/blockchain.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/brave_search.py` & `oplangchain-0.1.0/oplangchain/document_loaders/brave_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/browserless.py` & `oplangchain-0.1.0/oplangchain/document_loaders/browserless.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/chatgpt.py` & `oplangchain-0.1.0/oplangchain/document_loaders/chatgpt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/college_confidential.py` & `oplangchain-0.1.0/oplangchain/document_loaders/college_confidential.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/concurrent.py` & `oplangchain-0.1.0/oplangchain/document_loaders/concurrent.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/confluence.py` & `oplangchain-0.1.0/oplangchain/document_loaders/confluence.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/conllu.py` & `oplangchain-0.1.0/oplangchain/document_loaders/conllu.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/csv_loader.py` & `oplangchain-0.1.0/oplangchain/document_loaders/csv_loader.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/cube_semantic.py` & `oplangchain-0.1.0/oplangchain/document_loaders/cube_semantic.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/datadog_logs.py` & `oplangchain-0.1.0/oplangchain/document_loaders/datadog_logs.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/dataframe.py` & `oplangchain-0.1.0/oplangchain/document_loaders/dataframe.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/diffbot.py` & `oplangchain-0.1.0/oplangchain/document_loaders/diffbot.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/directory.py` & `oplangchain-0.1.0/oplangchain/document_loaders/directory.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/discord.py` & `oplangchain-0.1.0/oplangchain/document_loaders/discord.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/docugami.py` & `oplangchain-0.1.0/oplangchain/document_loaders/docugami.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/dropbox.py` & `oplangchain-0.1.0/oplangchain/document_loaders/dropbox.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/duckdb_loader.py` & `oplangchain-0.1.0/oplangchain/document_loaders/duckdb_loader.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/email.py` & `oplangchain-0.1.0/oplangchain/document_loaders/email.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/embaas.py` & `oplangchain-0.1.0/oplangchain/document_loaders/embaas.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/epub.py` & `oplangchain-0.1.0/oplangchain/document_loaders/epub.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/etherscan.py` & `oplangchain-0.1.0/oplangchain/document_loaders/etherscan.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/evernote.py` & `oplangchain-0.1.0/oplangchain/document_loaders/evernote.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/excel.py` & `oplangchain-0.1.0/oplangchain/document_loaders/excel.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/facebook_chat.py` & `oplangchain-0.1.0/oplangchain/document_loaders/facebook_chat.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/fauna.py` & `oplangchain-0.1.0/oplangchain/document_loaders/fauna.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/figma.py` & `oplangchain-0.1.0/oplangchain/document_loaders/figma.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/gcs_directory.py` & `oplangchain-0.1.0/oplangchain/document_loaders/gcs_directory.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/gcs_file.py` & `oplangchain-0.1.0/oplangchain/document_loaders/gcs_file.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/generic.py` & `oplangchain-0.1.0/oplangchain/document_loaders/generic.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/geodataframe.py` & `oplangchain-0.1.0/oplangchain/document_loaders/geodataframe.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/git.py` & `oplangchain-0.1.0/oplangchain/document_loaders/git.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/gitbook.py` & `oplangchain-0.1.0/oplangchain/document_loaders/gitbook.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/github.py` & `oplangchain-0.1.0/oplangchain/document_loaders/github.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/googledrive.py` & `oplangchain-0.1.0/oplangchain/document_loaders/googledrive.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/gutenberg.py` & `oplangchain-0.1.0/oplangchain/document_loaders/gutenberg.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/helpers.py` & `oplangchain-0.1.0/oplangchain/document_loaders/helpers.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/hn.py` & `oplangchain-0.1.0/oplangchain/document_loaders/hn.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/html.py` & `oplangchain-0.1.0/oplangchain/document_loaders/html.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/html_bs.py` & `oplangchain-0.1.0/oplangchain/document_loaders/html_bs.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/hugging_face_dataset.py` & `oplangchain-0.1.0/oplangchain/document_loaders/hugging_face_dataset.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/ifixit.py` & `oplangchain-0.1.0/oplangchain/document_loaders/ifixit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/image.py` & `oplangchain-0.1.0/oplangchain/document_loaders/image.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/image_captions.py` & `oplangchain-0.1.0/oplangchain/document_loaders/image_captions.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/iugu.py` & `oplangchain-0.1.0/oplangchain/document_loaders/iugu.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/joplin.py` & `oplangchain-0.1.0/oplangchain/document_loaders/joplin.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/json_loader.py` & `oplangchain-0.1.0/oplangchain/document_loaders/json_loader.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/larksuite.py` & `oplangchain-0.1.0/oplangchain/document_loaders/larksuite.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/markdown.py` & `oplangchain-0.1.0/oplangchain/document_loaders/markdown.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/mastodon.py` & `oplangchain-0.1.0/oplangchain/document_loaders/mastodon.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/max_compute.py` & `oplangchain-0.1.0/oplangchain/document_loaders/max_compute.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/mediawikidump.py` & `oplangchain-0.1.0/oplangchain/document_loaders/mediawikidump.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/merge.py` & `oplangchain-0.1.0/oplangchain/document_loaders/merge.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/mhtml.py` & `oplangchain-0.1.0/oplangchain/document_loaders/mhtml.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/modern_treasury.py` & `oplangchain-0.1.0/oplangchain/document_loaders/modern_treasury.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/news.py` & `oplangchain-0.1.0/oplangchain/document_loaders/news.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/notebook.py` & `oplangchain-0.1.0/oplangchain/document_loaders/notebook.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/notion.py` & `oplangchain-0.1.0/oplangchain/document_loaders/notion.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/notiondb.py` & `oplangchain-0.1.0/oplangchain/document_loaders/notiondb.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/nuclia.py` & `oplangchain-0.1.0/oplangchain/document_loaders/nuclia.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/obs_directory.py` & `oplangchain-0.1.0/oplangchain/document_loaders/obs_directory.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/obs_file.py` & `oplangchain-0.1.0/oplangchain/document_loaders/obs_file.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/obsidian.py` & `oplangchain-0.1.0/oplangchain/document_loaders/obsidian.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/odt.py` & `oplangchain-0.1.0/oplangchain/document_loaders/odt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/onedrive.py` & `oplangchain-0.1.0/oplangchain/document_loaders/onedrive.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/onedrive_file.py` & `oplangchain-0.1.0/oplangchain/document_loaders/onedrive_file.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/open_city_data.py` & `oplangchain-0.1.0/oplangchain/document_loaders/open_city_data.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/org_mode.py` & `oplangchain-0.1.0/oplangchain/document_loaders/org_mode.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/parsers/__init__.py` & `oplangchain-0.1.0/oplangchain/document_loaders/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/parsers/audio.py` & `oplangchain-0.1.0/oplangchain/document_loaders/parsers/audio.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/parsers/generic.py` & `oplangchain-0.1.0/oplangchain/document_loaders/parsers/generic.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/parsers/grobid.py` & `oplangchain-0.1.0/oplangchain/document_loaders/parsers/grobid.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/parsers/html/bs4.py` & `oplangchain-0.1.0/oplangchain/document_loaders/parsers/html/bs4.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/parsers/language/javascript.py` & `oplangchain-0.1.0/oplangchain/document_loaders/parsers/language/javascript.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/parsers/language/language_parser.py` & `oplangchain-0.1.0/oplangchain/document_loaders/parsers/language/language_parser.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/parsers/language/python.py` & `oplangchain-0.1.0/oplangchain/document_loaders/parsers/language/python.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/parsers/pdf.py` & `oplangchain-0.1.0/oplangchain/document_loaders/parsers/pdf.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/parsers/registry.py` & `oplangchain-0.1.0/oplangchain/document_loaders/parsers/registry.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/pdf.py` & `oplangchain-0.1.0/oplangchain/document_loaders/pdf.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/powerpoint.py` & `oplangchain-0.1.0/oplangchain/document_loaders/powerpoint.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/psychic.py` & `oplangchain-0.1.0/oplangchain/document_loaders/psychic.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/pyspark_dataframe.py` & `oplangchain-0.1.0/oplangchain/document_loaders/pyspark_dataframe.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/python.py` & `oplangchain-0.1.0/oplangchain/document_loaders/python.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/readthedocs.py` & `oplangchain-0.1.0/oplangchain/document_loaders/readthedocs.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/recursive_url_loader.py` & `oplangchain-0.1.0/oplangchain/document_loaders/recursive_url_loader.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/reddit.py` & `oplangchain-0.1.0/oplangchain/document_loaders/reddit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/roam.py` & `oplangchain-0.1.0/oplangchain/document_loaders/roam.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/rocksetdb.py` & `oplangchain-0.1.0/oplangchain/document_loaders/rocksetdb.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/rss.py` & `oplangchain-0.1.0/oplangchain/document_loaders/rss.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/rst.py` & `oplangchain-0.1.0/oplangchain/document_loaders/rst.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/rtf.py` & `oplangchain-0.1.0/oplangchain/document_loaders/rtf.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/s3_directory.py` & `oplangchain-0.1.0/oplangchain/document_loaders/s3_directory.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/s3_file.py` & `oplangchain-0.1.0/oplangchain/document_loaders/s3_file.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/sitemap.py` & `oplangchain-0.1.0/oplangchain/document_loaders/sitemap.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/slack_directory.py` & `oplangchain-0.1.0/oplangchain/document_loaders/slack_directory.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/snowflake_loader.py` & `oplangchain-0.1.0/oplangchain/document_loaders/snowflake_loader.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/spreedly.py` & `oplangchain-0.1.0/oplangchain/document_loaders/spreedly.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/srt.py` & `oplangchain-0.1.0/oplangchain/document_loaders/srt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/stripe.py` & `oplangchain-0.1.0/oplangchain/document_loaders/stripe.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/telegram.py` & `oplangchain-0.1.0/oplangchain/document_loaders/telegram.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/tencent_cos_directory.py` & `oplangchain-0.1.0/oplangchain/document_loaders/tencent_cos_directory.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/tencent_cos_file.py` & `oplangchain-0.1.0/oplangchain/document_loaders/tencent_cos_file.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/text.py` & `oplangchain-0.1.0/oplangchain/document_loaders/text.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/tomarkdown.py` & `oplangchain-0.1.0/oplangchain/document_loaders/tomarkdown.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/toml.py` & `oplangchain-0.1.0/oplangchain/document_loaders/toml.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/trello.py` & `oplangchain-0.1.0/oplangchain/document_loaders/trello.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/tsv.py` & `oplangchain-0.1.0/oplangchain/document_loaders/tsv.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/twitter.py` & `oplangchain-0.1.0/oplangchain/document_loaders/twitter.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/unstructured.py` & `oplangchain-0.1.0/oplangchain/document_loaders/unstructured.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/url.py` & `oplangchain-0.1.0/oplangchain/document_loaders/url.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/url_playwright.py` & `oplangchain-0.1.0/oplangchain/document_loaders/url_playwright.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/url_selenium.py` & `oplangchain-0.1.0/oplangchain/document_loaders/url_selenium.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/weather.py` & `oplangchain-0.1.0/oplangchain/document_loaders/weather.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/web_base.py` & `oplangchain-0.1.0/oplangchain/document_loaders/web_base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/whatsapp_chat.py` & `oplangchain-0.1.0/oplangchain/document_loaders/whatsapp_chat.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/wikipedia.py` & `oplangchain-0.1.0/oplangchain/document_loaders/wikipedia.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/word_document.py` & `oplangchain-0.1.0/oplangchain/document_loaders/word_document.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/xml.py` & `oplangchain-0.1.0/oplangchain/document_loaders/xml.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/xorbits.py` & `oplangchain-0.1.0/oplangchain/document_loaders/xorbits.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_loaders/youtube.py` & `oplangchain-0.1.0/oplangchain/document_loaders/youtube.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_transformers/__init__.py` & `oplangchain-0.1.0/oplangchain/document_transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_transformers/doctran_text_extract.py` & `oplangchain-0.1.0/oplangchain/document_transformers/doctran_text_extract.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_transformers/doctran_text_qa.py` & `oplangchain-0.1.0/oplangchain/document_transformers/doctran_text_qa.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_transformers/doctran_text_translate.py` & `oplangchain-0.1.0/oplangchain/document_transformers/doctran_text_translate.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_transformers/embeddings_redundant_filter.py` & `oplangchain-0.1.0/oplangchain/document_transformers/embeddings_redundant_filter.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_transformers/html2text.py` & `oplangchain-0.1.0/oplangchain/document_transformers/html2text.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_transformers/long_context_reorder.py` & `oplangchain-0.1.0/oplangchain/document_transformers/long_context_reorder.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_transformers/nuclia_text_transform.py` & `oplangchain-0.1.0/oplangchain/document_transformers/nuclia_text_transform.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/document_transformers/openai_functions.py` & `oplangchain-0.1.0/oplangchain/document_transformers/openai_functions.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/embeddings/__init__.py` & `oplangchain-0.1.0/oplangchain/embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/embeddings/aleph_alpha.py` & `oplangchain-0.1.0/oplangchain/embeddings/aleph_alpha.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/embeddings/awa.py` & `oplangchain-0.1.0/oplangchain/embeddings/awa.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/embeddings/base.py` & `oplangchain-0.1.0/oplangchain/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/embeddings/bedrock.py` & `oplangchain-0.1.0/oplangchain/embeddings/bedrock.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/embeddings/clarifai.py` & `oplangchain-0.1.0/oplangchain/embeddings/clarifai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/embeddings/cohere.py` & `oplangchain-0.1.0/oplangchain/embeddings/cohere.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/embeddings/dashscope.py` & `oplangchain-0.1.0/oplangchain/embeddings/dashscope.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/embeddings/deepinfra.py` & `oplangchain-0.1.0/oplangchain/embeddings/deepinfra.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/embeddings/edenai.py` & `oplangchain-0.1.0/oplangchain/embeddings/edenai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/embeddings/elasticsearch.py` & `oplangchain-0.1.0/oplangchain/embeddings/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/embeddings/embaas.py` & `oplangchain-0.1.0/oplangchain/embeddings/embaas.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/embeddings/fake.py` & `oplangchain-0.1.0/oplangchain/embeddings/fake.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/embeddings/google_palm.py` & `oplangchain-0.1.0/oplangchain/embeddings/google_palm.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/embeddings/gpt4all.py` & `oplangchain-0.1.0/oplangchain/embeddings/gpt4all.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/embeddings/huggingface.py` & `oplangchain-0.1.0/oplangchain/embeddings/huggingface.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/embeddings/huggingface_hub.py` & `oplangchain-0.1.0/oplangchain/embeddings/huggingface_hub.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/embeddings/jina.py` & `oplangchain-0.1.0/oplangchain/embeddings/jina.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/embeddings/llamacpp.py` & `oplangchain-0.1.0/oplangchain/embeddings/llamacpp.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/embeddings/localai.py` & `oplangchain-0.1.0/oplangchain/embeddings/localai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/embeddings/minimax.py` & `oplangchain-0.1.0/oplangchain/embeddings/minimax.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/embeddings/mlflow_gateway.py` & `oplangchain-0.1.0/oplangchain/embeddings/mlflow_gateway.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/embeddings/modelscope_hub.py` & `oplangchain-0.1.0/oplangchain/embeddings/modelscope_hub.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/embeddings/mosaicml.py` & `oplangchain-0.1.0/oplangchain/embeddings/mosaicml.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/embeddings/nlpcloud.py` & `oplangchain-0.1.0/oplangchain/embeddings/nlpcloud.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/embeddings/octoai_embeddings.py` & `oplangchain-0.1.0/oplangchain/embeddings/octoai_embeddings.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/embeddings/openai.py` & `oplangchain-0.1.0/oplangchain/embeddings/openai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/embeddings/sagemaker_endpoint.py` & `oplangchain-0.1.0/oplangchain/embeddings/sagemaker_endpoint.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/embeddings/self_hosted.py` & `oplangchain-0.1.0/oplangchain/embeddings/self_hosted.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/embeddings/self_hosted_hugging_face.py` & `oplangchain-0.1.0/oplangchain/embeddings/self_hosted_hugging_face.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/embeddings/spacy_embeddings.py` & `oplangchain-0.1.0/oplangchain/embeddings/spacy_embeddings.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/embeddings/tensorflow_hub.py` & `oplangchain-0.1.0/oplangchain/embeddings/tensorflow_hub.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/embeddings/vertexai.py` & `oplangchain-0.1.0/oplangchain/embeddings/vertexai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/embeddings/xinference.py` & `oplangchain-0.1.0/oplangchain/embeddings/xinference.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/evaluation/__init__.py` & `oplangchain-0.1.0/oplangchain/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/evaluation/agents/trajectory_eval_chain.py` & `oplangchain-0.1.0/oplangchain/evaluation/agents/trajectory_eval_chain.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/evaluation/agents/trajectory_eval_prompt.py` & `oplangchain-0.1.0/oplangchain/evaluation/agents/trajectory_eval_prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/evaluation/comparison/__init__.py` & `oplangchain-0.1.0/oplangchain/evaluation/comparison/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/evaluation/comparison/eval_chain.py` & `oplangchain-0.1.0/oplangchain/evaluation/comparison/eval_chain.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/evaluation/comparison/prompt.py` & `oplangchain-0.1.0/oplangchain/evaluation/comparison/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/evaluation/criteria/__init__.py` & `oplangchain-0.1.0/oplangchain/evaluation/criteria/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/evaluation/criteria/eval_chain.py` & `oplangchain-0.1.0/oplangchain/evaluation/criteria/eval_chain.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/evaluation/criteria/prompt.py` & `oplangchain-0.1.0/oplangchain/evaluation/criteria/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/evaluation/embedding_distance/base.py` & `oplangchain-0.1.0/oplangchain/evaluation/embedding_distance/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/evaluation/loading.py` & `oplangchain-0.1.0/oplangchain/evaluation/loading.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/evaluation/qa/eval_chain.py` & `oplangchain-0.1.0/oplangchain/evaluation/qa/eval_chain.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/evaluation/qa/eval_prompt.py` & `oplangchain-0.1.0/oplangchain/evaluation/qa/eval_prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/evaluation/qa/generate_chain.py` & `oplangchain-0.1.0/oplangchain/evaluation/qa/generate_chain.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/evaluation/qa/generate_prompt.py` & `oplangchain-0.1.0/oplangchain/evaluation/qa/generate_prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/evaluation/schema.py` & `oplangchain-0.1.0/oplangchain/evaluation/schema.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/evaluation/string_distance/base.py` & `oplangchain-0.1.0/oplangchain/evaluation/string_distance/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/graphs/__init__.py` & `oplangchain-0.1.0/oplangchain/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/graphs/arangodb_graph.py` & `oplangchain-0.1.0/oplangchain/graphs/arangodb_graph.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/graphs/hugegraph.py` & `oplangchain-0.1.0/oplangchain/graphs/hugegraph.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/graphs/kuzu_graph.py` & `oplangchain-0.1.0/oplangchain/graphs/kuzu_graph.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/graphs/memgraph_graph.py` & `oplangchain-0.1.0/oplangchain/graphs/memgraph_graph.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/graphs/nebula_graph.py` & `oplangchain-0.1.0/oplangchain/graphs/nebula_graph.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/graphs/neo4j_graph.py` & `oplangchain-0.1.0/oplangchain/graphs/neo4j_graph.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/graphs/neptune_graph.py` & `oplangchain-0.1.0/oplangchain/graphs/neptune_graph.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/graphs/networkx_graph.py` & `oplangchain-0.1.0/oplangchain/graphs/networkx_graph.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/graphs/rdf_graph.py` & `oplangchain-0.1.0/oplangchain/graphs/rdf_graph.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/indexes/graph.py` & `oplangchain-0.1.0/oplangchain/indexes/graph.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/indexes/prompts/entity_extraction.py` & `oplangchain-0.1.0/oplangchain/indexes/prompts/entity_extraction.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/indexes/prompts/entity_summarization.py` & `oplangchain-0.1.0/oplangchain/indexes/prompts/entity_summarization.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/indexes/prompts/knowledge_triplet_extraction.py` & `oplangchain-0.1.0/oplangchain/indexes/prompts/knowledge_triplet_extraction.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/indexes/vectorstore.py` & `oplangchain-0.1.0/oplangchain/indexes/vectorstore.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/__init__.py` & `oplangchain-0.1.0/oplangchain/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/ai21.py` & `oplangchain-0.1.0/oplangchain/llms/ai21.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/aleph_alpha.py` & `oplangchain-0.1.0/oplangchain/llms/aleph_alpha.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/amazon_api_gateway.py` & `oplangchain-0.1.0/oplangchain/llms/amazon_api_gateway.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/anthropic.py` & `oplangchain-0.1.0/oplangchain/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/anyscale.py` & `oplangchain-0.1.0/oplangchain/llms/anyscale.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/aviary.py` & `oplangchain-0.1.0/oplangchain/llms/aviary.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/azureml_endpoint.py` & `oplangchain-0.1.0/oplangchain/llms/azureml_endpoint.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/bananadev.py` & `oplangchain-0.1.0/oplangchain/llms/bananadev.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/base.py` & `oplangchain-0.1.0/oplangchain/llms/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/baseten.py` & `oplangchain-0.1.0/oplangchain/llms/baseten.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/beam.py` & `oplangchain-0.1.0/oplangchain/llms/beam.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/bedrock.py` & `oplangchain-0.1.0/oplangchain/llms/bedrock.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/cerebriumai.py` & `oplangchain-0.1.0/oplangchain/llms/cerebriumai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/chatglm.py` & `oplangchain-0.1.0/oplangchain/llms/chatglm.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/clarifai.py` & `oplangchain-0.1.0/oplangchain/llms/clarifai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/cohere.py` & `oplangchain-0.1.0/oplangchain/llms/cohere.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/ctransformers.py` & `oplangchain-0.1.0/oplangchain/llms/ctransformers.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/databricks.py` & `oplangchain-0.1.0/oplangchain/llms/databricks.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/deepinfra.py` & `oplangchain-0.1.0/oplangchain/llms/deepinfra.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/edenai.py` & `oplangchain-0.1.0/oplangchain/llms/edenai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/fake.py` & `oplangchain-0.1.0/oplangchain/llms/fake.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/fireworks.py` & `oplangchain-0.1.0/oplangchain/llms/fireworks.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/forefrontai.py` & `oplangchain-0.1.0/oplangchain/llms/forefrontai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/google_palm.py` & `oplangchain-0.1.0/oplangchain/llms/google_palm.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/gooseai.py` & `oplangchain-0.1.0/oplangchain/llms/gooseai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/gpt4all.py` & `oplangchain-0.1.0/oplangchain/llms/gpt4all.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/huggingface_endpoint.py` & `oplangchain-0.1.0/oplangchain/llms/huggingface_endpoint.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/huggingface_hub.py` & `oplangchain-0.1.0/oplangchain/llms/huggingface_hub.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/huggingface_pipeline.py` & `oplangchain-0.1.0/oplangchain/llms/huggingface_pipeline.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/huggingface_text_gen_inference.py` & `oplangchain-0.1.0/oplangchain/llms/huggingface_text_gen_inference.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/human.py` & `oplangchain-0.1.0/oplangchain/llms/human.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/koboldai.py` & `oplangchain-0.1.0/oplangchain/llms/koboldai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/llamacpp.py` & `oplangchain-0.1.0/oplangchain/llms/llamacpp.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/loading.py` & `oplangchain-0.1.0/oplangchain/llms/loading.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/manifest.py` & `oplangchain-0.1.0/oplangchain/llms/manifest.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/minimax.py` & `oplangchain-0.1.0/oplangchain/llms/minimax.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/mlflow_ai_gateway.py` & `oplangchain-0.1.0/oplangchain/llms/mlflow_ai_gateway.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/modal.py` & `oplangchain-0.1.0/oplangchain/llms/modal.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/mosaicml.py` & `oplangchain-0.1.0/oplangchain/llms/mosaicml.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/nlpcloud.py` & `oplangchain-0.1.0/oplangchain/llms/nlpcloud.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/octoai_endpoint.py` & `oplangchain-0.1.0/oplangchain/llms/octoai_endpoint.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/openai.py` & `oplangchain-0.1.0/oplangchain/llms/openai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/openllm.py` & `oplangchain-0.1.0/oplangchain/llms/openllm.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/openlm.py` & `oplangchain-0.1.0/oplangchain/llms/openlm.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/petals.py` & `oplangchain-0.1.0/oplangchain/llms/petals.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/pipelineai.py` & `oplangchain-0.1.0/oplangchain/llms/pipelineai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/predibase.py` & `oplangchain-0.1.0/oplangchain/llms/predibase.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/predictionguard.py` & `oplangchain-0.1.0/oplangchain/llms/predictionguard.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/promptlayer_openai.py` & `oplangchain-0.1.0/oplangchain/llms/promptlayer_openai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/replicate.py` & `oplangchain-0.1.0/oplangchain/llms/replicate.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/rwkv.py` & `oplangchain-0.1.0/oplangchain/llms/rwkv.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/sagemaker_endpoint.py` & `oplangchain-0.1.0/oplangchain/llms/sagemaker_endpoint.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/self_hosted.py` & `oplangchain-0.1.0/oplangchain/llms/self_hosted.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/self_hosted_hugging_face.py` & `oplangchain-0.1.0/oplangchain/llms/self_hosted_hugging_face.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/stochasticai.py` & `oplangchain-0.1.0/oplangchain/llms/stochasticai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/textgen.py` & `oplangchain-0.1.0/oplangchain/llms/textgen.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/tongyi.py` & `oplangchain-0.1.0/oplangchain/llms/tongyi.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/vertexai.py` & `oplangchain-0.1.0/oplangchain/llms/vertexai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/vllm.py` & `oplangchain-0.1.0/oplangchain/llms/vllm.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/writer.py` & `oplangchain-0.1.0/oplangchain/llms/writer.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/llms/xinference.py` & `oplangchain-0.1.0/oplangchain/llms/xinference.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/load/dump.py` & `oplangchain-0.1.0/oplangchain/load/dump.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/load/load.py` & `oplangchain-0.1.0/oplangchain/load/load.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/load/serializable.py` & `oplangchain-0.1.0/oplangchain/load/serializable.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/memory/__init__.py` & `oplangchain-0.1.0/oplangchain/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/memory/buffer.py` & `oplangchain-0.1.0/oplangchain/memory/buffer.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/memory/buffer_window.py` & `oplangchain-0.1.0/oplangchain/memory/buffer_window.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/memory/chat_memory.py` & `oplangchain-0.1.0/oplangchain/memory/chat_memory.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/memory/chat_message_histories/__init__.py` & `oplangchain-0.1.0/oplangchain/memory/chat_message_histories/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/memory/chat_message_histories/cassandra.py` & `oplangchain-0.1.0/oplangchain/memory/chat_message_histories/cassandra.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/memory/chat_message_histories/cosmos_db.py` & `oplangchain-0.1.0/oplangchain/memory/chat_message_histories/cosmos_db.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/memory/chat_message_histories/dynamodb.py` & `oplangchain-0.1.0/oplangchain/memory/chat_message_histories/dynamodb.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/memory/chat_message_histories/file.py` & `oplangchain-0.1.0/oplangchain/memory/chat_message_histories/file.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/memory/chat_message_histories/firestore.py` & `oplangchain-0.1.0/oplangchain/memory/chat_message_histories/firestore.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/memory/chat_message_histories/in_memory.py` & `oplangchain-0.1.0/oplangchain/memory/chat_message_histories/in_memory.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/memory/chat_message_histories/momento.py` & `oplangchain-0.1.0/oplangchain/memory/chat_message_histories/momento.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/memory/chat_message_histories/mongodb.py` & `oplangchain-0.1.0/oplangchain/memory/chat_message_histories/mongodb.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/memory/chat_message_histories/postgres.py` & `oplangchain-0.1.0/oplangchain/memory/chat_message_histories/postgres.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/memory/chat_message_histories/redis.py` & `oplangchain-0.1.0/oplangchain/memory/chat_message_histories/redis.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/memory/chat_message_histories/sql.py` & `oplangchain-0.1.0/oplangchain/memory/chat_message_histories/sql.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/memory/chat_message_histories/streamlit.py` & `oplangchain-0.1.0/oplangchain/memory/chat_message_histories/streamlit.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/memory/chat_message_histories/zep.py` & `oplangchain-0.1.0/oplangchain/memory/chat_message_histories/zep.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/memory/combined.py` & `oplangchain-0.1.0/oplangchain/memory/combined.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/memory/entity.py` & `oplangchain-0.1.0/oplangchain/memory/entity.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/memory/kg.py` & `oplangchain-0.1.0/oplangchain/memory/kg.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/memory/motorhead_memory.py` & `oplangchain-0.1.0/oplangchain/memory/motorhead_memory.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/memory/prompt.py` & `oplangchain-0.1.0/oplangchain/memory/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/memory/readonly.py` & `oplangchain-0.1.0/oplangchain/memory/readonly.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/memory/simple.py` & `oplangchain-0.1.0/oplangchain/memory/simple.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/memory/summary.py` & `oplangchain-0.1.0/oplangchain/memory/summary.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/memory/summary_buffer.py` & `oplangchain-0.1.0/oplangchain/memory/summary_buffer.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/memory/token_buffer.py` & `oplangchain-0.1.0/oplangchain/memory/token_buffer.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/memory/utils.py` & `oplangchain-0.1.0/oplangchain/memory/utils.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/memory/vectorstore.py` & `oplangchain-0.1.0/oplangchain/memory/vectorstore.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/memory/zep_memory.py` & `oplangchain-0.1.0/oplangchain/memory/zep_memory.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/model_laboratory.py` & `oplangchain-0.1.0/oplangchain/model_laboratory.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/output_parsers/__init__.py` & `oplangchain-0.1.0/oplangchain/output_parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/output_parsers/boolean.py` & `oplangchain-0.1.0/oplangchain/output_parsers/boolean.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/output_parsers/combining.py` & `oplangchain-0.1.0/oplangchain/output_parsers/combining.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/output_parsers/datetime.py` & `oplangchain-0.1.0/oplangchain/output_parsers/datetime.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/output_parsers/enum.py` & `oplangchain-0.1.0/oplangchain/output_parsers/enum.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/output_parsers/fix.py` & `oplangchain-0.1.0/oplangchain/output_parsers/fix.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/output_parsers/format_instructions.py` & `oplangchain-0.1.0/oplangchain/output_parsers/format_instructions.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/output_parsers/json.py` & `oplangchain-0.1.0/oplangchain/output_parsers/json.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/output_parsers/list.py` & `oplangchain-0.1.0/oplangchain/output_parsers/list.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/output_parsers/loading.py` & `oplangchain-0.1.0/oplangchain/output_parsers/loading.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/output_parsers/openai_functions.py` & `oplangchain-0.1.0/oplangchain/output_parsers/openai_functions.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/output_parsers/pydantic.py` & `oplangchain-0.1.0/oplangchain/output_parsers/pydantic.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/output_parsers/rail_parser.py` & `oplangchain-0.1.0/oplangchain/output_parsers/rail_parser.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/output_parsers/regex.py` & `oplangchain-0.1.0/oplangchain/output_parsers/regex.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/output_parsers/regex_dict.py` & `oplangchain-0.1.0/oplangchain/output_parsers/regex_dict.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/output_parsers/retry.py` & `oplangchain-0.1.0/oplangchain/output_parsers/retry.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/output_parsers/structured.py` & `oplangchain-0.1.0/oplangchain/output_parsers/structured.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/prompts/__init__.py` & `oplangchain-0.1.0/oplangchain/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/prompts/base.py` & `oplangchain-0.1.0/oplangchain/prompts/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/prompts/chat.py` & `oplangchain-0.1.0/oplangchain/prompts/chat.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/prompts/example_selector/__init__.py` & `oplangchain-0.1.0/oplangchain/prompts/example_selector/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/prompts/example_selector/base.py` & `oplangchain-0.1.0/oplangchain/prompts/example_selector/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/prompts/example_selector/length_based.py` & `oplangchain-0.1.0/oplangchain/prompts/example_selector/length_based.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/prompts/example_selector/ngram_overlap.py` & `oplangchain-0.1.0/oplangchain/prompts/example_selector/ngram_overlap.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/prompts/example_selector/semantic_similarity.py` & `oplangchain-0.1.0/oplangchain/prompts/example_selector/semantic_similarity.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/prompts/few_shot.py` & `oplangchain-0.1.0/oplangchain/prompts/few_shot.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/prompts/few_shot_with_templates.py` & `oplangchain-0.1.0/oplangchain/prompts/few_shot_with_templates.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/prompts/loading.py` & `oplangchain-0.1.0/oplangchain/prompts/loading.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/prompts/pipeline.py` & `oplangchain-0.1.0/oplangchain/prompts/pipeline.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/prompts/prompt.py` & `oplangchain-0.1.0/oplangchain/prompts/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/__init__.py` & `oplangchain-0.1.0/oplangchain/retrievers/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/arxiv.py` & `oplangchain-0.1.0/oplangchain/retrievers/arxiv.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/azure_cognitive_search.py` & `oplangchain-0.1.0/oplangchain/retrievers/azure_cognitive_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/bm25.py` & `oplangchain-0.1.0/oplangchain/retrievers/bm25.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/chaindesk.py` & `oplangchain-0.1.0/oplangchain/retrievers/chaindesk.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/chatgpt_plugin_retriever.py` & `oplangchain-0.1.0/oplangchain/retrievers/chatgpt_plugin_retriever.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/contextual_compression.py` & `oplangchain-0.1.0/oplangchain/retrievers/contextual_compression.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/databerry.py` & `oplangchain-0.1.0/oplangchain/retrievers/databerry.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/docarray.py` & `oplangchain-0.1.0/oplangchain/retrievers/docarray.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/document_compressors/__init__.py` & `oplangchain-0.1.0/oplangchain/retrievers/document_compressors/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/document_compressors/base.py` & `oplangchain-0.1.0/oplangchain/retrievers/document_compressors/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/document_compressors/chain_extract.py` & `oplangchain-0.1.0/oplangchain/retrievers/document_compressors/chain_extract.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/document_compressors/chain_filter.py` & `oplangchain-0.1.0/oplangchain/retrievers/document_compressors/chain_filter.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/document_compressors/cohere_rerank.py` & `oplangchain-0.1.0/oplangchain/retrievers/document_compressors/cohere_rerank.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/document_compressors/embeddings_filter.py` & `oplangchain-0.1.0/oplangchain/retrievers/document_compressors/embeddings_filter.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/elastic_search_bm25.py` & `oplangchain-0.1.0/oplangchain/retrievers/elastic_search_bm25.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/ensemble.py` & `oplangchain-0.1.0/oplangchain/retrievers/ensemble.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/google_cloud_enterprise_search.py` & `oplangchain-0.1.0/oplangchain/retrievers/google_cloud_enterprise_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/kendra.py` & `oplangchain-0.1.0/oplangchain/retrievers/kendra.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/knn.py` & `oplangchain-0.1.0/oplangchain/retrievers/knn.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/llama_index.py` & `oplangchain-0.1.0/oplangchain/retrievers/llama_index.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/merger_retriever.py` & `oplangchain-0.1.0/oplangchain/retrievers/merger_retriever.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/metal.py` & `oplangchain-0.1.0/oplangchain/retrievers/metal.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/milvus.py` & `oplangchain-0.1.0/oplangchain/retrievers/milvus.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/multi_query.py` & `oplangchain-0.1.0/oplangchain/retrievers/multi_query.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/pinecone_hybrid_search.py` & `oplangchain-0.1.0/oplangchain/retrievers/pinecone_hybrid_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/pubmed.py` & `oplangchain-0.1.0/oplangchain/retrievers/pubmed.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/re_phraser.py` & `oplangchain-0.1.0/oplangchain/retrievers/re_phraser.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/remote_retriever.py` & `oplangchain-0.1.0/oplangchain/retrievers/remote_retriever.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/self_query/base.py` & `oplangchain-0.1.0/oplangchain/retrievers/self_query/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/self_query/chroma.py` & `oplangchain-0.1.0/oplangchain/retrievers/self_query/chroma.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/self_query/deeplake.py` & `oplangchain-0.1.0/oplangchain/retrievers/self_query/deeplake.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/self_query/myscale.py` & `oplangchain-0.1.0/oplangchain/retrievers/self_query/myscale.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/self_query/pinecone.py` & `oplangchain-0.1.0/oplangchain/retrievers/self_query/pinecone.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/self_query/qdrant.py` & `oplangchain-0.1.0/oplangchain/retrievers/self_query/qdrant.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/self_query/weaviate.py` & `oplangchain-0.1.0/oplangchain/retrievers/self_query/weaviate.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/svm.py` & `oplangchain-0.1.0/oplangchain/retrievers/svm.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/tfidf.py` & `oplangchain-0.1.0/oplangchain/retrievers/tfidf.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/time_weighted_retriever.py` & `oplangchain-0.1.0/oplangchain/retrievers/time_weighted_retriever.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/vespa_retriever.py` & `oplangchain-0.1.0/oplangchain/retrievers/vespa_retriever.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/weaviate_hybrid_search.py` & `oplangchain-0.1.0/oplangchain/retrievers/weaviate_hybrid_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/web_research.py` & `oplangchain-0.1.0/oplangchain/retrievers/web_research.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/wikipedia.py` & `oplangchain-0.1.0/oplangchain/retrievers/wikipedia.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/zep.py` & `oplangchain-0.1.0/oplangchain/retrievers/zep.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/retrievers/zilliz.py` & `oplangchain-0.1.0/oplangchain/retrievers/zilliz.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/schema/__init__.py` & `oplangchain-0.1.0/oplangchain/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/schema/agent.py` & `oplangchain-0.1.0/oplangchain/schema/agent.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/schema/document.py` & `oplangchain-0.1.0/oplangchain/schema/document.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/schema/language_model.py` & `oplangchain-0.1.0/oplangchain/schema/language_model.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/schema/memory.py` & `oplangchain-0.1.0/oplangchain/schema/memory.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/schema/messages.py` & `oplangchain-0.1.0/oplangchain/schema/messages.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/schema/output.py` & `oplangchain-0.1.0/oplangchain/schema/output.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/schema/output_parser.py` & `oplangchain-0.1.0/oplangchain/schema/output_parser.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/schema/prompt.py` & `oplangchain-0.1.0/oplangchain/schema/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/schema/prompt_template.py` & `oplangchain-0.1.0/oplangchain/schema/prompt_template.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/schema/retriever.py` & `oplangchain-0.1.0/oplangchain/schema/retriever.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/schema/runnable.py` & `oplangchain-0.1.0/oplangchain/schema/runnable.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/server.py` & `oplangchain-0.1.0/oplangchain/server.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/smith/__init__.py` & `oplangchain-0.1.0/oplangchain/smith/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/smith/evaluation/__init__.py` & `oplangchain-0.1.0/oplangchain/smith/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/smith/evaluation/config.py` & `oplangchain-0.1.0/oplangchain/smith/evaluation/config.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/smith/evaluation/runner_utils.py` & `oplangchain-0.1.0/oplangchain/smith/evaluation/runner_utils.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/smith/evaluation/string_run_evaluator.py` & `oplangchain-0.1.0/oplangchain/smith/evaluation/string_run_evaluator.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/text_splitter.py` & `oplangchain-0.1.0/oplangchain/text_splitter.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/__init__.py` & `oplangchain-0.1.0/oplangchain/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/amadeus/closest_airport.py` & `oplangchain-0.1.0/oplangchain/tools/amadeus/closest_airport.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/amadeus/flight_search.py` & `oplangchain-0.1.0/oplangchain/tools/amadeus/flight_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/amadeus/utils.py` & `oplangchain-0.1.0/oplangchain/tools/amadeus/utils.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/arxiv/tool.py` & `oplangchain-0.1.0/oplangchain/tools/arxiv/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/azure_cognitive_services/__init__.py` & `oplangchain-0.1.0/oplangchain/tools/azure_cognitive_services/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/azure_cognitive_services/form_recognizer.py` & `oplangchain-0.1.0/oplangchain/tools/azure_cognitive_services/form_recognizer.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/azure_cognitive_services/image_analysis.py` & `oplangchain-0.1.0/oplangchain/tools/azure_cognitive_services/image_analysis.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/azure_cognitive_services/speech2text.py` & `oplangchain-0.1.0/oplangchain/tools/azure_cognitive_services/speech2text.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/azure_cognitive_services/text2speech.py` & `oplangchain-0.1.0/oplangchain/tools/azure_cognitive_services/text2speech.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/azure_cognitive_services/utils.py` & `oplangchain-0.1.0/oplangchain/tools/azure_cognitive_services/utils.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/base.py` & `oplangchain-0.1.0/oplangchain/tools/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/bing_search/tool.py` & `oplangchain-0.1.0/oplangchain/tools/bing_search/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/brave_search/tool.py` & `oplangchain-0.1.0/oplangchain/tools/brave_search/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/convert_to_openai.py` & `oplangchain-0.1.0/oplangchain/tools/convert_to_openai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/dataforseo_api_search/tool.py` & `oplangchain-0.1.0/oplangchain/tools/dataforseo_api_search/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/ddg_search/tool.py` & `oplangchain-0.1.0/oplangchain/tools/ddg_search/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/file_management/__init__.py` & `oplangchain-0.1.0/oplangchain/tools/file_management/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/file_management/copy.py` & `oplangchain-0.1.0/oplangchain/tools/file_management/copy.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/file_management/delete.py` & `oplangchain-0.1.0/oplangchain/tools/file_management/delete.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/file_management/file_search.py` & `oplangchain-0.1.0/oplangchain/tools/file_management/file_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/file_management/list_dir.py` & `oplangchain-0.1.0/oplangchain/tools/file_management/list_dir.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/file_management/move.py` & `oplangchain-0.1.0/oplangchain/tools/file_management/move.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/file_management/read.py` & `oplangchain-0.1.0/oplangchain/tools/file_management/read.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/file_management/utils.py` & `oplangchain-0.1.0/oplangchain/tools/file_management/utils.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/file_management/write.py` & `oplangchain-0.1.0/oplangchain/tools/file_management/write.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/github/prompt.py` & `oplangchain-0.1.0/oplangchain/tools/github/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/github/tool.py` & `oplangchain-0.1.0/oplangchain/tools/github/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/gmail/__init__.py` & `oplangchain-0.1.0/oplangchain/tools/gmail/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/gmail/base.py` & `oplangchain-0.1.0/oplangchain/tools/gmail/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/gmail/create_draft.py` & `oplangchain-0.1.0/oplangchain/tools/gmail/create_draft.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/gmail/get_message.py` & `oplangchain-0.1.0/oplangchain/tools/gmail/get_message.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/gmail/get_thread.py` & `oplangchain-0.1.0/oplangchain/tools/gmail/get_thread.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/gmail/search.py` & `oplangchain-0.1.0/oplangchain/tools/gmail/search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/gmail/send_message.py` & `oplangchain-0.1.0/oplangchain/tools/gmail/send_message.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/gmail/utils.py` & `oplangchain-0.1.0/oplangchain/tools/gmail/utils.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/golden_query/tool.py` & `oplangchain-0.1.0/oplangchain/tools/golden_query/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/google_places/tool.py` & `oplangchain-0.1.0/oplangchain/tools/google_places/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/google_search/tool.py` & `oplangchain-0.1.0/oplangchain/tools/google_search/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/google_serper/tool.py` & `oplangchain-0.1.0/oplangchain/tools/google_serper/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/graphql/tool.py` & `oplangchain-0.1.0/oplangchain/tools/graphql/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/human/tool.py` & `oplangchain-0.1.0/oplangchain/tools/human/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/ifttt.py` & `oplangchain-0.1.0/oplangchain/tools/ifttt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/jira/prompt.py` & `oplangchain-0.1.0/oplangchain/tools/jira/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/jira/tool.py` & `oplangchain-0.1.0/oplangchain/tools/jira/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/json/tool.py` & `oplangchain-0.1.0/oplangchain/tools/json/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/metaphor_search/tool.py` & `oplangchain-0.1.0/oplangchain/tools/metaphor_search/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/multion/create_session.py` & `oplangchain-0.1.0/oplangchain/tools/multion/create_session.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/multion/update_session.py` & `oplangchain-0.1.0/oplangchain/tools/multion/update_session.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/nuclia/tool.py` & `oplangchain-0.1.0/oplangchain/tools/nuclia/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/office365/__init__.py` & `oplangchain-0.1.0/oplangchain/tools/office365/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/office365/create_draft_message.py` & `oplangchain-0.1.0/oplangchain/tools/office365/create_draft_message.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/office365/events_search.py` & `oplangchain-0.1.0/oplangchain/tools/office365/events_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/office365/messages_search.py` & `oplangchain-0.1.0/oplangchain/tools/office365/messages_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/office365/send_event.py` & `oplangchain-0.1.0/oplangchain/tools/office365/send_event.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/office365/send_message.py` & `oplangchain-0.1.0/oplangchain/tools/office365/send_message.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/office365/utils.py` & `oplangchain-0.1.0/oplangchain/tools/office365/utils.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/openapi/utils/api_models.py` & `oplangchain-0.1.0/oplangchain/tools/openapi/utils/api_models.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/openweathermap/tool.py` & `oplangchain-0.1.0/oplangchain/tools/openweathermap/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/playwright/__init__.py` & `oplangchain-0.1.0/oplangchain/tools/playwright/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/playwright/base.py` & `oplangchain-0.1.0/oplangchain/tools/playwright/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/playwright/click.py` & `oplangchain-0.1.0/oplangchain/tools/playwright/click.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/playwright/current_page.py` & `oplangchain-0.1.0/oplangchain/tools/playwright/current_page.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/playwright/extract_hyperlinks.py` & `oplangchain-0.1.0/oplangchain/tools/playwright/extract_hyperlinks.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/playwright/extract_text.py` & `oplangchain-0.1.0/oplangchain/tools/playwright/extract_text.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/playwright/get_elements.py` & `oplangchain-0.1.0/oplangchain/tools/playwright/get_elements.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/playwright/navigate.py` & `oplangchain-0.1.0/oplangchain/tools/playwright/navigate.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/playwright/navigate_back.py` & `oplangchain-0.1.0/oplangchain/tools/playwright/navigate_back.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/playwright/utils.py` & `oplangchain-0.1.0/oplangchain/tools/playwright/utils.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/plugin.py` & `oplangchain-0.1.0/oplangchain/tools/plugin.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/powerbi/prompt.py` & `oplangchain-0.1.0/oplangchain/tools/powerbi/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/powerbi/tool.py` & `oplangchain-0.1.0/oplangchain/tools/powerbi/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/pubmed/tool.py` & `oplangchain-0.1.0/oplangchain/tools/pubmed/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/python/tool.py` & `oplangchain-0.1.0/oplangchain/tools/python/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/requests/tool.py` & `oplangchain-0.1.0/oplangchain/tools/requests/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/scenexplain/tool.py` & `oplangchain-0.1.0/oplangchain/tools/scenexplain/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/searx_search/tool.py` & `oplangchain-0.1.0/oplangchain/tools/searx_search/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/shell/tool.py` & `oplangchain-0.1.0/oplangchain/tools/shell/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/sleep/tool.py` & `oplangchain-0.1.0/oplangchain/tools/sleep/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/spark_sql/prompt.py` & `oplangchain-0.1.0/oplangchain/tools/spark_sql/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/spark_sql/tool.py` & `oplangchain-0.1.0/oplangchain/tools/spark_sql/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/sql_database/prompt.py` & `oplangchain-0.1.0/oplangchain/tools/sql_database/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/sql_database/tool.py` & `oplangchain-0.1.0/oplangchain/tools/sql_database/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/steamship_image_generation/tool.py` & `oplangchain-0.1.0/oplangchain/tools/steamship_image_generation/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/steamship_image_generation/utils.py` & `oplangchain-0.1.0/oplangchain/tools/steamship_image_generation/utils.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/vectorstore/tool.py` & `oplangchain-0.1.0/oplangchain/tools/vectorstore/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/wikipedia/tool.py` & `oplangchain-0.1.0/oplangchain/tools/wikipedia/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/wolfram_alpha/tool.py` & `oplangchain-0.1.0/oplangchain/tools/wolfram_alpha/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/youtube/search.py` & `oplangchain-0.1.0/oplangchain/tools/youtube/search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/zapier/prompt.py` & `oplangchain-0.1.0/oplangchain/tools/zapier/prompt.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/tools/zapier/tool.py` & `oplangchain-0.1.0/oplangchain/tools/zapier/tool.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/__init__.py` & `oplangchain-0.1.0/oplangchain/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/arxiv.py` & `oplangchain-0.1.0/oplangchain/utilities/arxiv.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/awslambda.py` & `oplangchain-0.1.0/oplangchain/utilities/awslambda.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/bash.py` & `oplangchain-0.1.0/oplangchain/utilities/bash.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/bibtex.py` & `oplangchain-0.1.0/oplangchain/utilities/bibtex.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/bing_search.py` & `oplangchain-0.1.0/oplangchain/utilities/bing_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/brave_search.py` & `oplangchain-0.1.0/oplangchain/utilities/brave_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/dataforseo_api_search.py` & `oplangchain-0.1.0/oplangchain/utilities/dataforseo_api_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/duckduckgo_search.py` & `oplangchain-0.1.0/oplangchain/utilities/duckduckgo_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/github.py` & `oplangchain-0.1.0/oplangchain/utilities/github.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/golden_query.py` & `oplangchain-0.1.0/oplangchain/utilities/golden_query.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/google_places_api.py` & `oplangchain-0.1.0/oplangchain/utilities/google_places_api.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/google_search.py` & `oplangchain-0.1.0/oplangchain/utilities/google_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/google_serper.py` & `oplangchain-0.1.0/oplangchain/utilities/google_serper.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/graphql.py` & `oplangchain-0.1.0/oplangchain/utilities/graphql.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/jira.py` & `oplangchain-0.1.0/oplangchain/utilities/jira.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/loading.py` & `oplangchain-0.1.0/oplangchain/utilities/loading.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/max_compute.py` & `oplangchain-0.1.0/oplangchain/utilities/max_compute.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/metaphor_search.py` & `oplangchain-0.1.0/oplangchain/utilities/metaphor_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/openapi.py` & `oplangchain-0.1.0/oplangchain/utilities/openapi.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/openweathermap.py` & `oplangchain-0.1.0/oplangchain/utilities/openweathermap.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/portkey.py` & `oplangchain-0.1.0/oplangchain/utilities/portkey.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/powerbi.py` & `oplangchain-0.1.0/oplangchain/utilities/powerbi.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/pupmed.py` & `oplangchain-0.1.0/oplangchain/utilities/pupmed.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/python.py` & `oplangchain-0.1.0/oplangchain/utilities/python.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/redis.py` & `oplangchain-0.1.0/oplangchain/utilities/redis.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/requests.py` & `oplangchain-0.1.0/oplangchain/utilities/requests.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/scenexplain.py` & `oplangchain-0.1.0/oplangchain/utilities/scenexplain.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/searx_search.py` & `oplangchain-0.1.0/oplangchain/utilities/searx_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/serpapi.py` & `oplangchain-0.1.0/oplangchain/utilities/serpapi.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/spark_sql.py` & `oplangchain-0.1.0/oplangchain/utilities/spark_sql.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/sql_database.py` & `oplangchain-0.1.0/oplangchain/utilities/sql_database.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/twilio.py` & `oplangchain-0.1.0/oplangchain/utilities/twilio.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/vertexai.py` & `oplangchain-0.1.0/oplangchain/utilities/vertexai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/wikipedia.py` & `oplangchain-0.1.0/oplangchain/utilities/wikipedia.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/wolfram_alpha.py` & `oplangchain-0.1.0/oplangchain/utilities/wolfram_alpha.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utilities/zapier.py` & `oplangchain-0.1.0/oplangchain/utilities/zapier.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utils/__init__.py` & `oplangchain-0.1.0/oplangchain/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utils/env.py` & `oplangchain-0.1.0/oplangchain/utils/env.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utils/formatting.py` & `oplangchain-0.1.0/oplangchain/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utils/input.py` & `oplangchain-0.1.0/oplangchain/utils/input.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utils/math.py` & `oplangchain-0.1.0/oplangchain/utils/math.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utils/strings.py` & `oplangchain-0.1.0/oplangchain/utils/strings.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/utils/utils.py` & `oplangchain-0.1.0/oplangchain/utils/utils.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/__init__.py` & `oplangchain-0.1.0/oplangchain/vectorstores/__init__.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/_pgvector_data_models.py` & `oplangchain-0.1.0/oplangchain/vectorstores/_pgvector_data_models.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/alibabacloud_opensearch.py` & `oplangchain-0.1.0/oplangchain/vectorstores/alibabacloud_opensearch.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/analyticdb.py` & `oplangchain-0.1.0/oplangchain/vectorstores/analyticdb.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/annoy.py` & `oplangchain-0.1.0/oplangchain/vectorstores/annoy.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/atlas.py` & `oplangchain-0.1.0/oplangchain/vectorstores/atlas.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/awadb.py` & `oplangchain-0.1.0/oplangchain/vectorstores/awadb.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/azuresearch.py` & `oplangchain-0.1.0/oplangchain/vectorstores/azuresearch.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/base.py` & `oplangchain-0.1.0/oplangchain/vectorstores/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/cassandra.py` & `oplangchain-0.1.0/oplangchain/vectorstores/cassandra.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/chroma.py` & `oplangchain-0.1.0/oplangchain/vectorstores/chroma.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/clarifai.py` & `oplangchain-0.1.0/oplangchain/vectorstores/clarifai.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/clickhouse.py` & `oplangchain-0.1.0/oplangchain/vectorstores/clickhouse.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/deeplake.py` & `oplangchain-0.1.0/oplangchain/vectorstores/deeplake.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/docarray/base.py` & `oplangchain-0.1.0/oplangchain/vectorstores/docarray/base.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/docarray/hnsw.py` & `oplangchain-0.1.0/oplangchain/vectorstores/docarray/hnsw.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/docarray/in_memory.py` & `oplangchain-0.1.0/oplangchain/vectorstores/docarray/in_memory.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/elastic_vector_search.py` & `oplangchain-0.1.0/oplangchain/vectorstores/elastic_vector_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/faiss.py` & `oplangchain-0.1.0/oplangchain/vectorstores/faiss.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/hologres.py` & `oplangchain-0.1.0/oplangchain/vectorstores/hologres.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/lancedb.py` & `oplangchain-0.1.0/oplangchain/vectorstores/lancedb.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/marqo.py` & `oplangchain-0.1.0/oplangchain/vectorstores/marqo.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/matching_engine.py` & `oplangchain-0.1.0/oplangchain/vectorstores/matching_engine.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/meilisearch.py` & `oplangchain-0.1.0/oplangchain/vectorstores/meilisearch.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/milvus.py` & `oplangchain-0.1.0/oplangchain/vectorstores/milvus.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/mongodb_atlas.py` & `oplangchain-0.1.0/oplangchain/vectorstores/mongodb_atlas.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/myscale.py` & `oplangchain-0.1.0/oplangchain/vectorstores/myscale.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/opensearch_vector_search.py` & `oplangchain-0.1.0/oplangchain/vectorstores/opensearch_vector_search.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/pgembedding.py` & `oplangchain-0.1.0/oplangchain/vectorstores/pgembedding.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/pgvector.py` & `oplangchain-0.1.0/oplangchain/vectorstores/pgvector.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/pinecone.py` & `oplangchain-0.1.0/oplangchain/vectorstores/pinecone.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/qdrant.py` & `oplangchain-0.1.0/oplangchain/vectorstores/qdrant.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/redis.py` & `oplangchain-0.1.0/oplangchain/vectorstores/redis.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/rocksetdb.py` & `oplangchain-0.1.0/oplangchain/vectorstores/rocksetdb.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/scann.py` & `oplangchain-0.1.0/oplangchain/vectorstores/scann.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/singlestoredb.py` & `oplangchain-0.1.0/oplangchain/vectorstores/singlestoredb.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/sklearn.py` & `oplangchain-0.1.0/oplangchain/vectorstores/sklearn.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/starrocks.py` & `oplangchain-0.1.0/oplangchain/vectorstores/starrocks.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/supabase.py` & `oplangchain-0.1.0/oplangchain/vectorstores/supabase.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/tair.py` & `oplangchain-0.1.0/oplangchain/vectorstores/tair.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/tigris.py` & `oplangchain-0.1.0/oplangchain/vectorstores/tigris.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/typesense.py` & `oplangchain-0.1.0/oplangchain/vectorstores/typesense.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/utils.py` & `oplangchain-0.1.0/oplangchain/vectorstores/utils.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/vectara.py` & `oplangchain-0.1.0/oplangchain/vectorstores/vectara.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/weaviate.py` & `oplangchain-0.1.0/oplangchain/vectorstores/weaviate.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/oplangchain/vectorstores/zilliz.py` & `oplangchain-0.1.0/oplangchain/vectorstores/zilliz.py`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/pyproject.toml` & `oplangchain-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "oplangchain"
-version = "0.0.255"
-description = "Building applications with LLMs through composability"
+version = "0.1.0"
+description = "langchain modified for OpenPlugin"
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://www.github.com/hwchase17/langchain"
 
 [tool.poetry.scripts]
 langchain-server = "langchain.server:main"
```

### Comparing `oplangchain-0.0.255/README.md` & `oplangchain-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `oplangchain-0.0.255/PKG-INFO` & `oplangchain-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: oplangchain
-Version: 0.0.255
-Summary: Building applications with LLMs through composability
+Version: 0.1.0
+Summary: langchain modified for OpenPlugin
 Home-page: https://www.github.com/hwchase17/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

