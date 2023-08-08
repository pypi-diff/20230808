# Comparing `tmp/semantic_kernel-0.3.6.dev0.tar.gz` & `tmp/semantic_kernel-0.3.7.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_kernel-0.3.6.dev0.tar", max compression
+gzip compressed data, was "semantic_kernel-0.3.7.dev0.tar", max compression
```

## Comparing `semantic_kernel-0.3.6.dev0.tar` & `semantic_kernel-0.3.7.dev0.tar`

### file list

```diff
@@ -1,123 +1,124 @@
--rw-r--r--   0        0        0     1186 2023-05-08 23:38:10.000000 semantic_kernel-0.3.6.dev0/pip/README.md
--rw-r--r--   0        0        0     1577 2023-08-07 16:13:48.135392 semantic_kernel-0.3.6.dev0/pyproject.toml
--rw-r--r--   0        0        0     1375 2023-07-12 19:14:40.912511 semantic_kernel-0.3.6.dev0/semantic_kernel/__init__.py
--rw-r--r--   0        0        0      719 2023-05-25 17:48:21.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/__init__.py
--rw-r--r--   0        0        0     1647 2023-04-30 18:57:02.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/ai_exception.py
--rw-r--r--   0        0        0     1792 2023-06-12 17:06:53.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py
--rw-r--r--   0        0        0     1321 2023-07-14 16:57:26.312407 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/chat_request_settings.py
--rw-r--r--   0        0        0     1484 2023-07-14 16:57:26.312942 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/complete_request_settings.py
--rw-r--r--   0        0        0      282 2023-04-30 18:57:02.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
--rw-r--r--   0        0        0      352 2023-04-30 18:57:02.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/hugging_face/__init__.py
--rw-r--r--   0        0        0     6190 2023-08-07 16:13:48.138206 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
--rw-r--r--   0        0        0     2317 2023-05-08 23:38:10.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
--rw-r--r--   0        0        0      892 2023-04-30 18:57:02.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py
--rw-r--r--   0        0        0     2615 2023-05-15 18:12:57.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
--rw-r--r--   0        0        0     2607 2023-05-15 18:12:57.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
--rw-r--r--   0        0        0     2602 2023-05-15 18:12:57.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
--rw-r--r--   0        0        0     8903 2023-07-16 00:59:27.692753 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
--rw-r--r--   0        0        0     5788 2023-07-16 00:59:27.693316 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
--rw-r--r--   0        0        0     3007 2023-08-07 16:13:48.139150 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
--rw-r--r--   0        0        0     1616 2023-06-12 17:06:53.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py
--rw-r--r--   0        0        0      242 2023-07-21 00:24:52.991872 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/__init__.py
--rw-r--r--   0        0        0    15609 2023-07-21 00:24:52.992413 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py
--rw-r--r--   0        0        0     8224 2023-07-21 00:24:52.992894 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py
--rw-r--r--   0        0        0      182 2023-05-18 17:32:52.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/chroma/__init__.py
--rw-r--r--   0        0        0    15093 2023-08-02 21:24:01.722277 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
--rw-r--r--   0        0        0     4426 2023-07-16 00:58:38.000353 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/chroma/utils.py
--rw-r--r--   0        0        0      133 2023-07-21 00:24:52.995551 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/milvus/__init__.py
--rw-r--r--   0        0        0    16859 2023-07-21 00:24:52.995917 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py
--rw-r--r--   0        0        0      190 2023-07-06 22:13:35.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/pinecone/__init__.py
--rw-r--r--   0        0        0    14928 2023-07-12 19:14:40.913001 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py
--rw-r--r--   0        0        0     1154 2023-07-06 22:13:35.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/pinecone/utils.py
--rw-r--r--   0        0        0      190 2023-07-12 19:14:40.913420 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/postgres/__init__.py
--rw-r--r--   0        0        0    20480 2023-07-12 19:14:40.913726 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py
--rw-r--r--   0        0        0      182 2023-08-02 21:24:01.723071 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/qdrant/__init__.py
--rw-r--r--   0        0        0    11910 2023-08-02 21:24:01.723452 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py
--rw-r--r--   0        0        0    11295 2023-06-12 17:06:53.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py
--rw-r--r--   0        0        0      126 2023-08-07 16:13:48.139679 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/openapi/__init__.py
--rw-r--r--   0        0        0    11132 2023-08-07 16:13:48.140037 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/openapi/sk_openapi.py
--rw-r--r--   0        0        0      265 2023-08-02 21:24:01.724044 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/search_engine/__init__.py
--rw-r--r--   0        0        0     2891 2023-08-02 21:24:01.724670 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/search_engine/bing_connector.py
--rw-r--r--   0        0        0      254 2023-08-02 21:24:01.725238 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/search_engine/connector.py
--rw-r--r--   0        0        0     3268 2023-08-02 21:24:01.725609 semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/search_engine/google_connector.py
--rw-r--r--   0        0        0      804 2023-07-17 21:15:24.599960 semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/__init__.py
--rw-r--r--   0        0        0     2553 2023-08-07 16:13:48.140835 semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/conversation_summary_skill.py
--rw-r--r--   0        0        0     2200 2023-08-07 16:13:48.141276 semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/file_io_skill.py
--rw-r--r--   0        0        0     3823 2023-08-07 16:13:48.141662 semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/http_skill.py
--rw-r--r--   0        0        0     3264 2023-08-07 16:13:48.142147 semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/math_skill.py
--rw-r--r--   0        0        0     4710 2023-08-07 16:13:48.142825 semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/text_memory_skill.py
--rw-r--r--   0        0        0     2531 2023-08-07 16:13:48.143278 semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/text_skill.py
--rw-r--r--   0        0        0     7978 2023-08-07 16:13:48.143817 semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/time_skill.py
--rw-r--r--   0        0        0      747 2023-08-07 16:13:48.144413 semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/wait_skill.py
--rw-r--r--   0        0        0     1950 2023-07-17 21:15:24.600357 semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/web_search_engine_skill.py
--rw-r--r--   0        0        0    31084 2023-08-07 16:13:48.145351 semantic_kernel-0.3.6.dev0/semantic_kernel/kernel.py
--rw-r--r--   0        0        0     1726 2023-07-16 00:59:27.695868 semantic_kernel-0.3.6.dev0/semantic_kernel/kernel_exception.py
--rw-r--r--   0        0        0      160 2023-04-13 23:12:46.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/memory/__init__.py
--rw-r--r--   0        0        0     2544 2023-06-08 17:22:29.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/memory/memory_query_result.py
--rw-r--r--   0        0        0     3912 2023-07-12 19:14:40.914195 semantic_kernel-0.3.6.dev0/semantic_kernel/memory/memory_record.py
--rw-r--r--   0        0        0     7272 2023-08-02 21:24:01.726940 semantic_kernel-0.3.6.dev0/semantic_kernel/memory/memory_store_base.py
--rw-r--r--   0        0        0     1666 2023-08-02 21:24:01.727814 semantic_kernel-0.3.6.dev0/semantic_kernel/memory/null_memory.py
--rw-r--r--   0        0        0     6354 2023-07-16 00:42:59.250269 semantic_kernel-0.3.6.dev0/semantic_kernel/memory/semantic_text_memory.py
--rw-r--r--   0        0        0     3418 2023-08-02 21:24:01.728381 semantic_kernel-0.3.6.dev0/semantic_kernel/memory/semantic_text_memory_base.py
--rw-r--r--   0        0        0    12032 2023-05-15 18:12:57.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/memory/volatile_memory_store.py
--rw-r--r--   0        0        0     2361 2023-04-22 04:06:40.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/orchestration/context_variables.py
--rw-r--r--   0        0        0     5079 2023-04-14 00:51:57.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/orchestration/delegate_handlers.py
--rw-r--r--   0        0        0     9005 2023-05-19 23:02:13.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/orchestration/delegate_inference.py
--rw-r--r--   0        0        0      638 2023-04-13 23:12:46.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/orchestration/delegate_types.py
--rw-r--r--   0        0        0     7514 2023-04-14 00:52:05.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/orchestration/sk_context.py
--rw-r--r--   0        0        0    21047 2023-08-07 16:13:48.146463 semantic_kernel-0.3.6.dev0/semantic_kernel/orchestration/sk_function.py
--rw-r--r--   0        0        0     6289 2023-08-07 16:13:48.147317 semantic_kernel-0.3.6.dev0/semantic_kernel/orchestration/sk_function_base.py
--rw-r--r--   0        0        0      408 2023-08-02 21:24:01.729218 semantic_kernel-0.3.6.dev0/semantic_kernel/planning/__init__.py
--rw-r--r--   0        0        0    12946 2023-08-07 16:13:48.148064 semantic_kernel-0.3.6.dev0/semantic_kernel/planning/action_planner/action_planner.py
--rw-r--r--   0        0        0      355 2023-08-02 21:24:01.730504 semantic_kernel-0.3.6.dev0/semantic_kernel/planning/action_planner/skprompt.txt
--rw-r--r--   0        0        0     7536 2023-08-07 16:13:48.149023 semantic_kernel-0.3.6.dev0/semantic_kernel/planning/basic_planner.py
--rw-r--r--   0        0        0    16641 2023-08-07 16:13:48.149664 semantic_kernel-0.3.6.dev0/semantic_kernel/planning/plan.py
--rw-r--r--   0        0        0     1198 2023-08-02 21:24:01.731437 semantic_kernel-0.3.6.dev0/semantic_kernel/planning/planning_exception.py
--rw-r--r--   0        0        0      723 2023-08-02 21:24:01.732600 semantic_kernel-0.3.6.dev0/semantic_kernel/planning/sequential_planner/Skills/SequentialPlanning/config.json
--rw-r--r--   0        0        0     3005 2023-08-02 21:24:01.732891 semantic_kernel-0.3.6.dev0/semantic_kernel/planning/sequential_planner/Skills/SequentialPlanning/skprompt.txt
--rw-r--r--   0        0        0      142 2023-08-02 21:24:01.733143 semantic_kernel-0.3.6.dev0/semantic_kernel/planning/sequential_planner/__init__.py
--rw-r--r--   0        0        0     5761 2023-08-02 21:24:01.733497 semantic_kernel-0.3.6.dev0/semantic_kernel/planning/sequential_planner/sequential_planner.py
--rw-r--r--   0        0        0     1147 2023-08-02 21:24:01.733879 semantic_kernel-0.3.6.dev0/semantic_kernel/planning/sequential_planner/sequential_planner_config.py
--rw-r--r--   0        0        0     8636 2023-08-07 16:13:48.150305 semantic_kernel-0.3.6.dev0/semantic_kernel/planning/sequential_planner/sequential_planner_extensions.py
--rw-r--r--   0        0        0     5515 2023-08-02 21:24:01.734840 semantic_kernel-0.3.6.dev0/semantic_kernel/planning/sequential_planner/sequential_planner_parser.py
--rw-r--r--   0        0        0     1001 2023-08-07 16:13:48.151163 semantic_kernel-0.3.6.dev0/semantic_kernel/reliability/pass_through_without_retry.py
--rw-r--r--   0        0        0      694 2023-06-05 21:39:19.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/reliability/retry_mechanism_base.py
--rw-r--r--   0        0        0     2101 2023-04-13 23:12:46.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py
--rw-r--r--   0        0        0     2332 2023-04-14 00:51:57.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/semantic_functions/prompt_template.py
--rw-r--r--   0        0        0      506 2023-04-13 23:12:46.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/semantic_functions/prompt_template_base.py
--rw-r--r--   0        0        0     4525 2023-06-12 17:06:53.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/semantic_functions/prompt_template_config.py
--rw-r--r--   0        0        0      671 2023-04-14 00:51:57.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/semantic_functions/semantic_function_config.py
--rw-r--r--   0        0        0     2793 2023-08-07 16:13:48.151449 semantic_kernel-0.3.6.dev0/semantic_kernel/sk_pydantic.py
--rw-r--r--   0        0        0      322 2023-04-14 00:51:57.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/skill_definition/__init__.py
--rw-r--r--   0        0        0      958 2023-08-07 16:13:48.152176 semantic_kernel-0.3.6.dev0/semantic_kernel/skill_definition/function_view.py
--rw-r--r--   0        0        0     2323 2023-08-07 16:13:48.152617 semantic_kernel-0.3.6.dev0/semantic_kernel/skill_definition/functions_view.py
--rw-r--r--   0        0        0      506 2023-08-07 16:13:48.153078 semantic_kernel-0.3.6.dev0/semantic_kernel/skill_definition/parameter_view.py
--rw-r--r--   0        0        0     4821 2023-08-07 16:13:48.153598 semantic_kernel-0.3.6.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py
--rw-r--r--   0        0        0     1415 2023-08-07 16:13:48.154182 semantic_kernel-0.3.6.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py
--rw-r--r--   0        0        0      817 2023-08-07 16:13:48.155067 semantic_kernel-0.3.6.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py
--rw-r--r--   0        0        0      840 2023-08-07 16:13:48.155620 semantic_kernel-0.3.6.dev0/semantic_kernel/skill_definition/sk_function_decorator.py
--rw-r--r--   0        0        0     4945 2023-08-07 16:13:48.156191 semantic_kernel-0.3.6.dev0/semantic_kernel/skill_definition/skill_collection.py
--rw-r--r--   0        0        0      959 2023-08-07 16:13:48.156737 semantic_kernel-0.3.6.dev0/semantic_kernel/skill_definition/skill_collection_base.py
--rw-r--r--   0        0        0     1115 2023-04-13 23:12:46.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/README.md
--rw-r--r--   0        0        0      918 2023-08-07 16:13:48.157561 semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/blocks/block.py
--rw-r--r--   0        0        0      228 2023-04-14 00:51:57.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/blocks/block_types.py
--rw-r--r--   0        0        0     4606 2023-08-07 16:13:48.157992 semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/blocks/code_block.py
--rw-r--r--   0        0        0     3053 2023-08-07 16:13:48.158688 semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/blocks/function_id_block.py
--rw-r--r--   0        0        0      276 2023-04-13 23:12:46.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/blocks/symbols.py
--rw-r--r--   0        0        0     1519 2023-08-07 16:13:48.159110 semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/blocks/text_block.py
--rw-r--r--   0        0        0     2311 2023-08-07 16:13:48.159574 semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/blocks/val_block.py
--rw-r--r--   0        0        0     2637 2023-08-07 16:13:48.159998 semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/blocks/var_block.py
--rw-r--r--   0        0        0     6604 2023-08-07 16:13:48.160845 semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/code_tokenizer.py
--rw-r--r--   0        0        0     6035 2023-08-07 16:13:48.161444 semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/prompt_template_engine.py
--rw-r--r--   0        0        0      532 2023-04-13 23:12:46.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/protocols/code_renderer.py
--rw-r--r--   0        0        0     3081 2023-08-07 16:13:48.162236 semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py
--rw-r--r--   0        0        0      596 2023-04-13 23:12:46.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/protocols/text_renderer.py
--rw-r--r--   0        0        0     7856 2023-08-07 16:13:48.162888 semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/template_tokenizer.py
--rw-r--r--   0        0        0      473 2023-04-30 18:57:03.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/text/__init__.py
--rw-r--r--   0        0        0      667 2023-04-30 18:57:03.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/text/function_extension.py
--rw-r--r--   0        0        0     8568 2023-07-16 00:58:38.006510 semantic_kernel-0.3.6.dev0/semantic_kernel/text/text_chunker.py
--rw-r--r--   0        0        0      403 2023-04-13 23:12:46.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/utils/null_logger.py
--rw-r--r--   0        0        0     2570 2023-08-07 16:13:48.163472 semantic_kernel-0.3.6.dev0/semantic_kernel/utils/settings.py
--rw-r--r--   0        0        0      221 2023-04-13 23:12:46.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/utils/static_property.py
--rw-r--r--   0        0        0     2198 2023-04-13 23:12:46.000000 semantic_kernel-0.3.6.dev0/semantic_kernel/utils/validation.py
--rw-r--r--   0        0        0     1965 1970-01-01 00:00:00.000000 semantic_kernel-0.3.6.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1186 2023-05-08 23:38:10.000000 semantic_kernel-0.3.7.dev0/pip/README.md
+-rw-r--r--   0        0        0     1577 2023-08-08 16:41:25.443291 semantic_kernel-0.3.7.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1375 2023-07-12 19:14:40.912511 semantic_kernel-0.3.7.dev0/semantic_kernel/__init__.py
+-rw-r--r--   0        0        0       48 2023-08-08 16:41:25.443978 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/__init__.py
+-rw-r--r--   0        0        0      719 2023-05-25 17:48:21.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/ai/__init__.py
+-rw-r--r--   0        0        0     1647 2023-04-30 18:57:02.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/ai/ai_exception.py
+-rw-r--r--   0        0        0     1792 2023-06-12 17:06:53.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py
+-rw-r--r--   0        0        0     1321 2023-07-14 16:57:26.312407 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/ai/chat_request_settings.py
+-rw-r--r--   0        0        0     1484 2023-07-14 16:57:26.312942 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/ai/complete_request_settings.py
+-rw-r--r--   0        0        0      282 2023-04-30 18:57:02.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
+-rw-r--r--   0        0        0      352 2023-04-30 18:57:02.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/ai/hugging_face/__init__.py
+-rw-r--r--   0        0        0     6190 2023-08-07 16:13:48.138206 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
+-rw-r--r--   0        0        0     2317 2023-05-08 23:38:10.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
+-rw-r--r--   0        0        0      892 2023-04-30 18:57:02.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py
+-rw-r--r--   0        0        0     2615 2023-05-15 18:12:57.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
+-rw-r--r--   0        0        0     2607 2023-05-15 18:12:57.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
+-rw-r--r--   0        0        0     2602 2023-05-15 18:12:57.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
+-rw-r--r--   0        0        0     8903 2023-07-16 00:59:27.692753 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
+-rw-r--r--   0        0        0     5788 2023-07-16 00:59:27.693316 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
+-rw-r--r--   0        0        0     3007 2023-08-07 16:13:48.139150 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
+-rw-r--r--   0        0        0     1616 2023-06-12 17:06:53.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py
+-rw-r--r--   0        0        0      242 2023-07-21 00:24:52.991872 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/__init__.py
+-rw-r--r--   0        0        0    15609 2023-07-21 00:24:52.992413 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py
+-rw-r--r--   0        0        0     8224 2023-07-21 00:24:52.992894 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py
+-rw-r--r--   0        0        0      182 2023-05-18 17:32:52.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/memory/chroma/__init__.py
+-rw-r--r--   0        0        0    15093 2023-08-02 21:24:01.722277 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
+-rw-r--r--   0        0        0     4426 2023-07-16 00:58:38.000353 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/memory/chroma/utils.py
+-rw-r--r--   0        0        0      133 2023-07-21 00:24:52.995551 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/memory/milvus/__init__.py
+-rw-r--r--   0        0        0    16859 2023-07-21 00:24:52.995917 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py
+-rw-r--r--   0        0        0      190 2023-07-06 22:13:35.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/memory/pinecone/__init__.py
+-rw-r--r--   0        0        0    14928 2023-07-12 19:14:40.913001 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py
+-rw-r--r--   0        0        0     1154 2023-07-06 22:13:35.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/memory/pinecone/utils.py
+-rw-r--r--   0        0        0      190 2023-07-12 19:14:40.913420 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/memory/postgres/__init__.py
+-rw-r--r--   0        0        0    20480 2023-07-12 19:14:40.913726 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py
+-rw-r--r--   0        0        0      182 2023-08-02 21:24:01.723071 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/memory/qdrant/__init__.py
+-rw-r--r--   0        0        0    11910 2023-08-02 21:24:01.723452 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py
+-rw-r--r--   0        0        0    11295 2023-06-12 17:06:53.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py
+-rw-r--r--   0        0        0      126 2023-08-07 16:13:48.139679 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/openapi/__init__.py
+-rw-r--r--   0        0        0    11132 2023-08-07 16:13:48.140037 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/openapi/sk_openapi.py
+-rw-r--r--   0        0        0      265 2023-08-02 21:24:01.724044 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/search_engine/__init__.py
+-rw-r--r--   0        0        0     2891 2023-08-02 21:24:01.724670 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/search_engine/bing_connector.py
+-rw-r--r--   0        0        0      254 2023-08-02 21:24:01.725238 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/search_engine/connector.py
+-rw-r--r--   0        0        0     3268 2023-08-02 21:24:01.725609 semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/search_engine/google_connector.py
+-rw-r--r--   0        0        0      804 2023-07-17 21:15:24.599960 semantic_kernel-0.3.7.dev0/semantic_kernel/core_skills/__init__.py
+-rw-r--r--   0        0        0     2553 2023-08-07 16:13:48.140835 semantic_kernel-0.3.7.dev0/semantic_kernel/core_skills/conversation_summary_skill.py
+-rw-r--r--   0        0        0     2200 2023-08-07 16:13:48.141276 semantic_kernel-0.3.7.dev0/semantic_kernel/core_skills/file_io_skill.py
+-rw-r--r--   0        0        0     3823 2023-08-07 16:13:48.141662 semantic_kernel-0.3.7.dev0/semantic_kernel/core_skills/http_skill.py
+-rw-r--r--   0        0        0     3264 2023-08-07 16:13:48.142147 semantic_kernel-0.3.7.dev0/semantic_kernel/core_skills/math_skill.py
+-rw-r--r--   0        0        0     4710 2023-08-07 16:13:48.142825 semantic_kernel-0.3.7.dev0/semantic_kernel/core_skills/text_memory_skill.py
+-rw-r--r--   0        0        0     2531 2023-08-07 16:13:48.143278 semantic_kernel-0.3.7.dev0/semantic_kernel/core_skills/text_skill.py
+-rw-r--r--   0        0        0     7978 2023-08-07 16:13:48.143817 semantic_kernel-0.3.7.dev0/semantic_kernel/core_skills/time_skill.py
+-rw-r--r--   0        0        0      747 2023-08-07 16:13:48.144413 semantic_kernel-0.3.7.dev0/semantic_kernel/core_skills/wait_skill.py
+-rw-r--r--   0        0        0     1950 2023-07-17 21:15:24.600357 semantic_kernel-0.3.7.dev0/semantic_kernel/core_skills/web_search_engine_skill.py
+-rw-r--r--   0        0        0    31084 2023-08-07 16:13:48.145351 semantic_kernel-0.3.7.dev0/semantic_kernel/kernel.py
+-rw-r--r--   0        0        0     1726 2023-07-16 00:59:27.695868 semantic_kernel-0.3.7.dev0/semantic_kernel/kernel_exception.py
+-rw-r--r--   0        0        0      160 2023-04-13 23:12:46.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/memory/__init__.py
+-rw-r--r--   0        0        0     2544 2023-06-08 17:22:29.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/memory/memory_query_result.py
+-rw-r--r--   0        0        0     3912 2023-07-12 19:14:40.914195 semantic_kernel-0.3.7.dev0/semantic_kernel/memory/memory_record.py
+-rw-r--r--   0        0        0     7272 2023-08-02 21:24:01.726940 semantic_kernel-0.3.7.dev0/semantic_kernel/memory/memory_store_base.py
+-rw-r--r--   0        0        0     1666 2023-08-02 21:24:01.727814 semantic_kernel-0.3.7.dev0/semantic_kernel/memory/null_memory.py
+-rw-r--r--   0        0        0     6354 2023-07-16 00:42:59.250269 semantic_kernel-0.3.7.dev0/semantic_kernel/memory/semantic_text_memory.py
+-rw-r--r--   0        0        0     3418 2023-08-02 21:24:01.728381 semantic_kernel-0.3.7.dev0/semantic_kernel/memory/semantic_text_memory_base.py
+-rw-r--r--   0        0        0    12032 2023-05-15 18:12:57.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/memory/volatile_memory_store.py
+-rw-r--r--   0        0        0     2361 2023-04-22 04:06:40.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/orchestration/context_variables.py
+-rw-r--r--   0        0        0     5079 2023-04-14 00:51:57.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/orchestration/delegate_handlers.py
+-rw-r--r--   0        0        0     9005 2023-05-19 23:02:13.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/orchestration/delegate_inference.py
+-rw-r--r--   0        0        0      638 2023-04-13 23:12:46.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/orchestration/delegate_types.py
+-rw-r--r--   0        0        0     7514 2023-04-14 00:52:05.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/orchestration/sk_context.py
+-rw-r--r--   0        0        0    21047 2023-08-07 16:13:48.146463 semantic_kernel-0.3.7.dev0/semantic_kernel/orchestration/sk_function.py
+-rw-r--r--   0        0        0     6289 2023-08-07 16:13:48.147317 semantic_kernel-0.3.7.dev0/semantic_kernel/orchestration/sk_function_base.py
+-rw-r--r--   0        0        0      408 2023-08-02 21:24:01.729218 semantic_kernel-0.3.7.dev0/semantic_kernel/planning/__init__.py
+-rw-r--r--   0        0        0    12946 2023-08-07 16:13:48.148064 semantic_kernel-0.3.7.dev0/semantic_kernel/planning/action_planner/action_planner.py
+-rw-r--r--   0        0        0      355 2023-08-02 21:24:01.730504 semantic_kernel-0.3.7.dev0/semantic_kernel/planning/action_planner/skprompt.txt
+-rw-r--r--   0        0        0     7860 2023-08-08 16:41:25.444667 semantic_kernel-0.3.7.dev0/semantic_kernel/planning/basic_planner.py
+-rw-r--r--   0        0        0    16641 2023-08-07 16:13:48.149664 semantic_kernel-0.3.7.dev0/semantic_kernel/planning/plan.py
+-rw-r--r--   0        0        0     1198 2023-08-02 21:24:01.731437 semantic_kernel-0.3.7.dev0/semantic_kernel/planning/planning_exception.py
+-rw-r--r--   0        0        0      723 2023-08-02 21:24:01.732600 semantic_kernel-0.3.7.dev0/semantic_kernel/planning/sequential_planner/Skills/SequentialPlanning/config.json
+-rw-r--r--   0        0        0     3005 2023-08-02 21:24:01.732891 semantic_kernel-0.3.7.dev0/semantic_kernel/planning/sequential_planner/Skills/SequentialPlanning/skprompt.txt
+-rw-r--r--   0        0        0      142 2023-08-02 21:24:01.733143 semantic_kernel-0.3.7.dev0/semantic_kernel/planning/sequential_planner/__init__.py
+-rw-r--r--   0        0        0     5761 2023-08-02 21:24:01.733497 semantic_kernel-0.3.7.dev0/semantic_kernel/planning/sequential_planner/sequential_planner.py
+-rw-r--r--   0        0        0     1147 2023-08-02 21:24:01.733879 semantic_kernel-0.3.7.dev0/semantic_kernel/planning/sequential_planner/sequential_planner_config.py
+-rw-r--r--   0        0        0     8636 2023-08-07 16:13:48.150305 semantic_kernel-0.3.7.dev0/semantic_kernel/planning/sequential_planner/sequential_planner_extensions.py
+-rw-r--r--   0        0        0     5515 2023-08-02 21:24:01.734840 semantic_kernel-0.3.7.dev0/semantic_kernel/planning/sequential_planner/sequential_planner_parser.py
+-rw-r--r--   0        0        0     1001 2023-08-07 16:13:48.151163 semantic_kernel-0.3.7.dev0/semantic_kernel/reliability/pass_through_without_retry.py
+-rw-r--r--   0        0        0      694 2023-06-05 21:39:19.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/reliability/retry_mechanism_base.py
+-rw-r--r--   0        0        0     2101 2023-04-13 23:12:46.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py
+-rw-r--r--   0        0        0     2332 2023-04-14 00:51:57.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/semantic_functions/prompt_template.py
+-rw-r--r--   0        0        0      506 2023-04-13 23:12:46.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/semantic_functions/prompt_template_base.py
+-rw-r--r--   0        0        0     4525 2023-06-12 17:06:53.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/semantic_functions/prompt_template_config.py
+-rw-r--r--   0        0        0      671 2023-04-14 00:51:57.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/semantic_functions/semantic_function_config.py
+-rw-r--r--   0        0        0     2793 2023-08-07 16:13:48.151449 semantic_kernel-0.3.7.dev0/semantic_kernel/sk_pydantic.py
+-rw-r--r--   0        0        0      322 2023-04-14 00:51:57.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/skill_definition/__init__.py
+-rw-r--r--   0        0        0      958 2023-08-07 16:13:48.152176 semantic_kernel-0.3.7.dev0/semantic_kernel/skill_definition/function_view.py
+-rw-r--r--   0        0        0     2323 2023-08-07 16:13:48.152617 semantic_kernel-0.3.7.dev0/semantic_kernel/skill_definition/functions_view.py
+-rw-r--r--   0        0        0      506 2023-08-07 16:13:48.153078 semantic_kernel-0.3.7.dev0/semantic_kernel/skill_definition/parameter_view.py
+-rw-r--r--   0        0        0     4821 2023-08-07 16:13:48.153598 semantic_kernel-0.3.7.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py
+-rw-r--r--   0        0        0     1415 2023-08-07 16:13:48.154182 semantic_kernel-0.3.7.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py
+-rw-r--r--   0        0        0      817 2023-08-07 16:13:48.155067 semantic_kernel-0.3.7.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py
+-rw-r--r--   0        0        0      840 2023-08-07 16:13:48.155620 semantic_kernel-0.3.7.dev0/semantic_kernel/skill_definition/sk_function_decorator.py
+-rw-r--r--   0        0        0     4945 2023-08-07 16:13:48.156191 semantic_kernel-0.3.7.dev0/semantic_kernel/skill_definition/skill_collection.py
+-rw-r--r--   0        0        0      959 2023-08-07 16:13:48.156737 semantic_kernel-0.3.7.dev0/semantic_kernel/skill_definition/skill_collection_base.py
+-rw-r--r--   0        0        0     1115 2023-04-13 23:12:46.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/template_engine/README.md
+-rw-r--r--   0        0        0      918 2023-08-07 16:13:48.157561 semantic_kernel-0.3.7.dev0/semantic_kernel/template_engine/blocks/block.py
+-rw-r--r--   0        0        0      228 2023-04-14 00:51:57.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/template_engine/blocks/block_types.py
+-rw-r--r--   0        0        0     4606 2023-08-07 16:13:48.157992 semantic_kernel-0.3.7.dev0/semantic_kernel/template_engine/blocks/code_block.py
+-rw-r--r--   0        0        0     3053 2023-08-07 16:13:48.158688 semantic_kernel-0.3.7.dev0/semantic_kernel/template_engine/blocks/function_id_block.py
+-rw-r--r--   0        0        0      276 2023-04-13 23:12:46.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/template_engine/blocks/symbols.py
+-rw-r--r--   0        0        0     1519 2023-08-07 16:13:48.159110 semantic_kernel-0.3.7.dev0/semantic_kernel/template_engine/blocks/text_block.py
+-rw-r--r--   0        0        0     2311 2023-08-07 16:13:48.159574 semantic_kernel-0.3.7.dev0/semantic_kernel/template_engine/blocks/val_block.py
+-rw-r--r--   0        0        0     2637 2023-08-07 16:13:48.159998 semantic_kernel-0.3.7.dev0/semantic_kernel/template_engine/blocks/var_block.py
+-rw-r--r--   0        0        0     6604 2023-08-07 16:13:48.160845 semantic_kernel-0.3.7.dev0/semantic_kernel/template_engine/code_tokenizer.py
+-rw-r--r--   0        0        0     6035 2023-08-07 16:13:48.161444 semantic_kernel-0.3.7.dev0/semantic_kernel/template_engine/prompt_template_engine.py
+-rw-r--r--   0        0        0      532 2023-04-13 23:12:46.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/template_engine/protocols/code_renderer.py
+-rw-r--r--   0        0        0     3081 2023-08-07 16:13:48.162236 semantic_kernel-0.3.7.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py
+-rw-r--r--   0        0        0      596 2023-04-13 23:12:46.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/template_engine/protocols/text_renderer.py
+-rw-r--r--   0        0        0     7856 2023-08-07 16:13:48.162888 semantic_kernel-0.3.7.dev0/semantic_kernel/template_engine/template_tokenizer.py
+-rw-r--r--   0        0        0      473 2023-04-30 18:57:03.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/text/__init__.py
+-rw-r--r--   0        0        0      667 2023-04-30 18:57:03.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/text/function_extension.py
+-rw-r--r--   0        0        0     8568 2023-07-16 00:58:38.006510 semantic_kernel-0.3.7.dev0/semantic_kernel/text/text_chunker.py
+-rw-r--r--   0        0        0      403 2023-04-13 23:12:46.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/utils/null_logger.py
+-rw-r--r--   0        0        0     2570 2023-08-07 16:13:48.163472 semantic_kernel-0.3.7.dev0/semantic_kernel/utils/settings.py
+-rw-r--r--   0        0        0      221 2023-04-13 23:12:46.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/utils/static_property.py
+-rw-r--r--   0        0        0     2198 2023-04-13 23:12:46.000000 semantic_kernel-0.3.7.dev0/semantic_kernel/utils/validation.py
+-rw-r--r--   0        0        0     1965 1970-01-01 00:00:00.000000 semantic_kernel-0.3.7.dev0/PKG-INFO
```

### Comparing `semantic_kernel-0.3.6.dev0/pip/README.md` & `semantic_kernel-0.3.7.dev0/pip/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/pyproject.toml` & `semantic_kernel-0.3.7.dev0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "semantic-kernel"
-version = "0.3.6.dev"
+version = "0.3.7.dev"
 description = ""
 authors = ["Microsoft <SK-Support@microsoft.com>"]
 readme = "pip/README.md"
 packages = [{include = "semantic_kernel"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/__init__.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/__init__.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/ai/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/ai_exception.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/ai/ai_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/chat_request_settings.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/ai/chat_request_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/complete_request_settings.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/ai/complete_request_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/chroma/utils.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/memory/chroma/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/pinecone/utils.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/memory/pinecone/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/openapi/sk_openapi.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/openapi/sk_openapi.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/search_engine/bing_connector.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/search_engine/bing_connector.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/connectors/search_engine/google_connector.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/connectors/search_engine/google_connector.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/__init__.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/core_skills/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/conversation_summary_skill.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/core_skills/conversation_summary_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/file_io_skill.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/core_skills/file_io_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/http_skill.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/core_skills/http_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/math_skill.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/core_skills/math_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/text_memory_skill.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/core_skills/text_memory_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/text_skill.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/core_skills/text_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/time_skill.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/core_skills/time_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/wait_skill.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/core_skills/wait_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/core_skills/web_search_engine_skill.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/core_skills/web_search_engine_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/kernel.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/kernel.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/kernel_exception.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/kernel_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/memory/memory_query_result.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/memory/memory_query_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/memory/memory_record.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/memory/memory_record.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/memory/memory_store_base.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/memory/memory_store_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/memory/null_memory.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/memory/null_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/memory/semantic_text_memory.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/memory/semantic_text_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/memory/semantic_text_memory_base.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/memory/semantic_text_memory_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/memory/volatile_memory_store.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/memory/volatile_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/orchestration/context_variables.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/orchestration/context_variables.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/orchestration/delegate_handlers.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/orchestration/delegate_handlers.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/orchestration/delegate_inference.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/orchestration/delegate_inference.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/orchestration/delegate_types.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/orchestration/delegate_types.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/orchestration/sk_context.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/orchestration/sk_context.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/orchestration/sk_function.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/orchestration/sk_function.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/orchestration/sk_function_base.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/orchestration/sk_function_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/planning/action_planner/action_planner.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/planning/action_planner/action_planner.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/planning/basic_planner.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/planning/basic_planner.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,30 @@
 """A basic JSON-based planner for the Python Semantic Kernel"""
 import json
 
 import regex
 
 from semantic_kernel.kernel import Kernel
 from semantic_kernel.orchestration.context_variables import ContextVariables
-from semantic_kernel.planning.plan import Plan
+
+
+class Plan:
+    """A simple plan object for the Semantic Kernel"""
+
+    def __init__(self, prompt: str, goal: str, plan: str):
+        self.prompt = prompt
+        self.goal = goal
+        self.generated_plan = plan
+
+    def __str__(self):
+        return f"Prompt: {self.prompt}\nGoal: {self.goal}\nPlan: {self.plan}"
+
+    def __repr__(self):
+        return str(self)
+
 
 PROMPT = """
 You are a planner for the Semantic Kernel.
 Your job is to create a properly formatted JSON plan step by step, to satisfy the goal given.
 Create a list of subtasks based off the [GOAL] provided.
 Each subtask must be from within the [AVAILABLE FUNCTIONS] list. Do not use any functions that are not in the list.
 Base your decisions on which functions to use from the description and the name of the function.
```

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/planning/plan.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/planning/plan.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/planning/planning_exception.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/planning/planning_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/planning/sequential_planner/Skills/SequentialPlanning/config.json` & `semantic_kernel-0.3.7.dev0/semantic_kernel/planning/sequential_planner/Skills/SequentialPlanning/config.json`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/planning/sequential_planner/Skills/SequentialPlanning/skprompt.txt` & `semantic_kernel-0.3.7.dev0/semantic_kernel/planning/sequential_planner/Skills/SequentialPlanning/skprompt.txt`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/planning/sequential_planner/sequential_planner.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/planning/sequential_planner/sequential_planner.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/planning/sequential_planner/sequential_planner_config.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/planning/sequential_planner/sequential_planner_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/planning/sequential_planner/sequential_planner_extensions.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/planning/sequential_planner/sequential_planner_extensions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/planning/sequential_planner/sequential_planner_parser.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/planning/sequential_planner/sequential_planner_parser.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/reliability/pass_through_without_retry.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/reliability/pass_through_without_retry.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/reliability/retry_mechanism_base.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/reliability/retry_mechanism_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/semantic_functions/prompt_template.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/semantic_functions/prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/semantic_functions/prompt_template_config.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/semantic_functions/prompt_template_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/semantic_functions/semantic_function_config.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/semantic_functions/semantic_function_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/sk_pydantic.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/sk_pydantic.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/skill_definition/function_view.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/skill_definition/function_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/skill_definition/functions_view.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/skill_definition/functions_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/skill_definition/sk_function_decorator.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/skill_definition/sk_function_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/skill_definition/skill_collection.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/skill_definition/skill_collection.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/skill_definition/skill_collection_base.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/skill_definition/skill_collection_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/README.md` & `semantic_kernel-0.3.7.dev0/semantic_kernel/template_engine/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/blocks/block.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/template_engine/blocks/block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/blocks/code_block.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/template_engine/blocks/code_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/blocks/function_id_block.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/template_engine/blocks/function_id_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/blocks/text_block.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/template_engine/blocks/text_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/blocks/val_block.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/template_engine/blocks/val_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/blocks/var_block.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/template_engine/blocks/var_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/code_tokenizer.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/template_engine/code_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/prompt_template_engine.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/template_engine/prompt_template_engine.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/protocols/code_renderer.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/template_engine/protocols/code_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/protocols/text_renderer.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/template_engine/protocols/text_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/template_engine/template_tokenizer.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/template_engine/template_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/text/function_extension.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/text/function_extension.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/text/text_chunker.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/text/text_chunker.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/utils/settings.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/utils/settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/semantic_kernel/utils/validation.py` & `semantic_kernel-0.3.7.dev0/semantic_kernel/utils/validation.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.6.dev0/PKG-INFO` & `semantic_kernel-0.3.7.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-kernel
-Version: 0.3.6.dev0
+Version: 0.3.7.dev0
 Summary: 
 Author: Microsoft
 Author-email: SK-Support@microsoft.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

