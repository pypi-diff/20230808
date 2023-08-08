# Comparing `tmp/vocode_api-0.0.5a5.tar.gz` & `tmp/vocode_api-0.0.5a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocode_api-0.0.5a5.tar", max compression
+gzip compressed data, was "vocode_api-0.0.5a6.tar", max compression
```

## Comparing `vocode_api-0.0.5a5.tar` & `vocode_api-0.0.5a6.tar`

### file list

```diff
@@ -1,110 +1,126 @@
--rw-r--r--   0        0        0     2777 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/README.md
--rw-r--r--   0        0        0      379 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/pyproject.toml
--rw-r--r--   0        0        0     4780 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/__init__.py
--rw-r--r--   0        0        0     2074 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/client.py
--rw-r--r--   0        0        0      348 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/core/__init__.py
--rw-r--r--   0        0        0      426 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      170 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/errors/__init__.py
--rw-r--r--   0        0        0      313 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/py.typed
--rw-r--r--   0        0        0      220 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/resources/actions/__init__.py
--rw-r--r--   0        0        0     9264 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/resources/actions/client.py
--rw-r--r--   0        0        0       65 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/resources/agents/__init__.py
--rw-r--r--   0        0        0     8814 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/resources/agents/client.py
--rw-r--r--   0        0        0       65 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/resources/calls/__init__.py
--rw-r--r--   0        0        0    10806 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/resources/calls/client.py
--rw-r--r--   0        0        0       65 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/resources/numbers/__init__.py
--rw-r--r--   0        0        0    10759 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/resources/numbers/client.py
--rw-r--r--   0        0        0       65 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/resources/usage/__init__.py
--rw-r--r--   0        0        0     2159 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/resources/usage/client.py
--rw-r--r--   0        0        0       65 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/resources/voices/__init__.py
--rw-r--r--   0        0        0     9214 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/resources/voices/client.py
--rw-r--r--   0        0        0       65 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/resources/webhooks/__init__.py
--rw-r--r--   0        0        0     8808 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/resources/webhooks/client.py
--rw-r--r--   0        0        0     7085 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/__init__.py
--rw-r--r--   0        0        0      837 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/action_type.py
--rw-r--r--   0        0        0     1029 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/agent.py
--rw-r--r--   0        0        0      316 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/agent_actions_item.py
--rw-r--r--   0        0        0     1096 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/agent_params.py
--rw-r--r--   0        0        0      384 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/agent_params_actions_item.py
--rw-r--r--   0        0        0      332 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/agent_params_voice.py
--rw-r--r--   0        0        0      177 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/agent_params_webhook.py
--rw-r--r--   0        0        0     1360 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/agent_update_params.py
--rw-r--r--   0        0        0      368 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/agent_update_params_actions.py
--rw-r--r--   0        0        0      477 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/agent_update_params_actions_agent_update_params_actions_item.py
--rw-r--r--   0        0        0      177 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/agent_update_params_initial_message.py
--rw-r--r--   0        0        0      169 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/agent_update_params_prompt.py
--rw-r--r--   0        0        0      445 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/agent_update_params_voice.py
--rw-r--r--   0        0        0      246 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/agent_update_params_webhook.py
--rw-r--r--   0        0        0      264 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/agent_voice.py
--rw-r--r--   0        0        0      913 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/azure_voice.py
--rw-r--r--   0        0        0      873 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/azure_voice_params.py
--rw-r--r--   0        0        0     1197 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/azure_voice_update_params.py
--rw-r--r--   0        0        0      173 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/azure_voice_update_params_pitch.py
--rw-r--r--   0        0        0      172 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/azure_voice_update_params_rate.py
--rw-r--r--   0        0        0      177 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/azure_voice_update_params_voice_name.py
--rw-r--r--   0        0        0     1035 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/call.py
--rw-r--r--   0        0        0      832 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/call_status.py
--rw-r--r--   0        0        0      376 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/create_action_request.py
--rw-r--r--   0        0        0      320 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/create_action_response.py
--rw-r--r--   0        0        0      175 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/create_call_request_agent.py
--rw-r--r--   0        0        0      329 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/create_voice_request.py
--rw-r--r--   0        0        0      273 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/create_voice_response.py
--rw-r--r--   0        0        0      931 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/dtmf_action.py
--rw-r--r--   0        0        0      891 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/dtmf_action_params.py
--rw-r--r--   0        0        0      932 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/dtmf_action_update_params.py
--rw-r--r--   0        0        0      239 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/dtmf_action_update_params_config.py
--rw-r--r--   0        0        0      953 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/eleven_labs_voice.py
--rw-r--r--   0        0        0      913 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/eleven_labs_voice_params.py
--rw-r--r--   0        0        0     1455 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/eleven_labs_voice_update_params.py
--rw-r--r--   0        0        0      179 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/eleven_labs_voice_update_params_api_key.py
--rw-r--r--   0        0        0      190 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/eleven_labs_voice_update_params_similarity_boost.py
--rw-r--r--   0        0        0      184 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/eleven_labs_voice_update_params_stability.py
--rw-r--r--   0        0        0      180 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/eleven_labs_voice_update_params_voice_id.py
--rw-r--r--   0        0        0      736 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/empty_action_config.py
--rw-r--r--   0        0        0      942 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/end_conversation_action.py
--rw-r--r--   0        0        0      902 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/end_conversation_action_params.py
--rw-r--r--   0        0        0      977 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/end_conversation_action_update_params.py
--rw-r--r--   0        0        0      250 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/end_conversation_action_update_params_config.py
--rw-r--r--   0        0        0     1395 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/event_type.py
--rw-r--r--   0        0        0      317 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/get_action_response.py
--rw-r--r--   0        0        0      270 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/get_voice_response.py
--rw-r--r--   0        0        0      466 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/http_method.py
--rw-r--r--   0        0        0      843 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/http_validation_error.py
--rw-r--r--   0        0        0      323 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/list_actions_response_item.py
--rw-r--r--   0        0        0      276 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/list_voices_response_item.py
--rw-r--r--   0        0        0      901 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/normalized_agent.py
--rw-r--r--   0        0        0     1018 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/normalized_call.py
--rw-r--r--   0        0        0      843 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/normalized_phone_number.py
--rw-r--r--   0        0        0      860 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/phone_number.py
--rw-r--r--   0        0        0      674 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/plan_type.py
--rw-r--r--   0        0        0      846 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/rime_voice.py
--rw-r--r--   0        0        0      806 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/rime_voice_params.py
--rw-r--r--   0        0        0      929 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/rime_voice_update_params.py
--rw-r--r--   0        0        0      174 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/rime_voice_update_params_speaker.py
--rw-r--r--   0        0        0      925 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/transfer_call_action.py
--rw-r--r--   0        0        0      885 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/transfer_call_action_params.py
--rw-r--r--   0        0        0      965 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/transfer_call_action_update_params.py
--rw-r--r--   0        0        0      250 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/transfer_call_action_update_params_config.py
--rw-r--r--   0        0        0      760 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/transfer_call_config.py
--rw-r--r--   0        0        0      728 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/undefined.py
--rw-r--r--   0        0        0      443 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/update_action_request_body.py
--rw-r--r--   0        0        0      320 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/update_action_response.py
--rw-r--r--   0        0        0      203 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/update_number_request_inbound_agent.py
--rw-r--r--   0        0        0      390 2023-07-25 00:32:52.145558 vocode_api-0.0.5a5/src/vocode/types/update_voice_request_body.py
--rw-r--r--   0        0        0      273 2023-07-25 00:32:52.149558 vocode_api-0.0.5a5/src/vocode/types/update_voice_response.py
--rw-r--r--   0        0        0      866 2023-07-25 00:32:52.149558 vocode_api-0.0.5a5/src/vocode/types/usage.py
--rw-r--r--   0        0        0      869 2023-07-25 00:32:52.149558 vocode_api-0.0.5a5/src/vocode/types/validation_error.py
--rw-r--r--   0        0        0      128 2023-07-25 00:32:52.149558 vocode_api-0.0.5a5/src/vocode/types/validation_error_loc_item.py
--rw-r--r--   0        0        0      907 2023-07-25 00:32:52.149558 vocode_api-0.0.5a5/src/vocode/types/voice_type.py
--rw-r--r--   0        0        0      921 2023-07-25 00:32:52.149558 vocode_api-0.0.5a5/src/vocode/types/webhook.py
--rw-r--r--   0        0        0      898 2023-07-25 00:32:52.149558 vocode_api-0.0.5a5/src/vocode/types/webhook_params.py
--rw-r--r--   0        0        0     1124 2023-07-25 00:32:52.149558 vocode_api-0.0.5a5/src/vocode/types/webhook_update_params.py
--rw-r--r--   0        0        0      214 2023-07-25 00:32:52.149558 vocode_api-0.0.5a5/src/vocode/types/webhook_update_params_method.py
--rw-r--r--   0        0        0      231 2023-07-25 00:32:52.149558 vocode_api-0.0.5a5/src/vocode/types/webhook_update_params_subscriptions.py
--rw-r--r--   0        0        0      168 2023-07-25 00:32:52.149558 vocode_api-0.0.5a5/src/vocode/types/webhook_update_params_url.py
--rw-r--r--   0        0        0     3187 1970-01-01 00:00:00.000000 vocode_api-0.0.5a5/PKG-INFO
+-rw-r--r--   0        0        0     2777 2023-08-08 21:10:39.979218 vocode_api-0.0.5a6/README.md
+-rw-r--r--   0        0        0      379 2023-08-08 21:10:39.979218 vocode_api-0.0.5a6/pyproject.toml
+-rw-r--r--   0        0        0     5878 2023-08-08 21:10:39.979218 vocode_api-0.0.5a6/src/vocode/__init__.py
+-rw-r--r--   0        0        0     2388 2023-08-08 21:10:39.979218 vocode_api-0.0.5a6/src/vocode/client.py
+-rw-r--r--   0        0        0      348 2023-08-08 21:10:39.979218 vocode_api-0.0.5a6/src/vocode/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-08-08 21:10:39.979218 vocode_api-0.0.5a6/src/vocode/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-08-08 21:10:39.979218 vocode_api-0.0.5a6/src/vocode/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-08-08 21:10:39.979218 vocode_api-0.0.5a6/src/vocode/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-08-08 21:10:39.979218 vocode_api-0.0.5a6/src/vocode/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      170 2023-08-08 21:10:39.979218 vocode_api-0.0.5a6/src/vocode/errors/__init__.py
+-rw-r--r--   0        0        0      313 2023-08-08 21:10:39.979218 vocode_api-0.0.5a6/src/vocode/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2023-08-08 21:10:39.979218 vocode_api-0.0.5a6/src/vocode/py.typed
+-rw-r--r--   0        0        0      240 2023-08-08 21:10:39.979218 vocode_api-0.0.5a6/src/vocode/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-08-08 21:10:39.979218 vocode_api-0.0.5a6/src/vocode/resources/actions/__init__.py
+-rw-r--r--   0        0        0     9715 2023-08-08 21:10:39.979218 vocode_api-0.0.5a6/src/vocode/resources/actions/client.py
+-rw-r--r--   0        0        0       65 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/resources/agents/__init__.py
+-rw-r--r--   0        0        0    11883 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/resources/agents/client.py
+-rw-r--r--   0        0        0       65 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/resources/calls/__init__.py
+-rw-r--r--   0        0        0    11313 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/resources/calls/client.py
+-rw-r--r--   0        0        0       65 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/resources/numbers/__init__.py
+-rw-r--r--   0        0        0    12026 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/resources/numbers/client.py
+-rw-r--r--   0        0        0       65 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/resources/payment/__init__.py
+-rw-r--r--   0        0        0     3921 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/resources/payment/client.py
+-rw-r--r--   0        0        0       65 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/resources/usage/__init__.py
+-rw-r--r--   0        0        0     2221 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/resources/usage/client.py
+-rw-r--r--   0        0        0       65 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/resources/voices/__init__.py
+-rw-r--r--   0        0        0     9671 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/resources/voices/client.py
+-rw-r--r--   0        0        0       65 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/resources/webhooks/__init__.py
+-rw-r--r--   0        0        0     9395 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/resources/webhooks/client.py
+-rw-r--r--   0        0        0     8780 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/__init__.py
+-rw-r--r--   0        0        0      837 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/action_type.py
+-rw-r--r--   0        0        0     1343 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/agent.py
+-rw-r--r--   0        0        0      316 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/agent_actions_item.py
+-rw-r--r--   0        0        0      384 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/agent_params_actions_item.py
+-rw-r--r--   0        0        0      231 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/agent_params_vector_database.py
+-rw-r--r--   0        0        0      332 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/agent_params_voice.py
+-rw-r--r--   0        0        0      177 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/agent_params_webhook.py
+-rw-r--r--   0        0        0     1811 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/agent_update_params.py
+-rw-r--r--   0        0        0      368 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/agent_update_params_actions.py
+-rw-r--r--   0        0        0      477 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/agent_update_params_actions_agent_update_params_actions_item.py
+-rw-r--r--   0        0        0      177 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/agent_update_params_initial_message.py
+-rw-r--r--   0        0        0      256 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/agent_update_params_interrupt_sensitivity.py
+-rw-r--r--   0        0        0      207 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/agent_update_params_language.py
+-rw-r--r--   0        0        0      169 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/agent_update_params_prompt.py
+-rw-r--r--   0        0        0      300 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/agent_update_params_vector_database.py
+-rw-r--r--   0        0        0      445 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/agent_update_params_voice.py
+-rw-r--r--   0        0        0      246 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/agent_update_params_webhook.py
+-rw-r--r--   0        0        0      264 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/agent_voice.py
+-rw-r--r--   0        0        0      913 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/azure_voice.py
+-rw-r--r--   0        0        0      873 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/azure_voice_params.py
+-rw-r--r--   0        0        0     1197 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/azure_voice_update_params.py
+-rw-r--r--   0        0        0      173 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/azure_voice_update_params_pitch.py
+-rw-r--r--   0        0        0      172 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/azure_voice_update_params_rate.py
+-rw-r--r--   0        0        0      177 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/azure_voice_update_params_voice_name.py
+-rw-r--r--   0        0        0     1035 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/call.py
+-rw-r--r--   0        0        0      832 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/call_status.py
+-rw-r--r--   0        0        0      376 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/create_action_request.py
+-rw-r--r--   0        0        0      320 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/create_action_response.py
+-rw-r--r--   0        0        0     1575 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/create_call_agent_params.py
+-rw-r--r--   0        0        0      400 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/create_call_agent_params_actions_item.py
+-rw-r--r--   0        0        0      241 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/create_call_agent_params_vector_database.py
+-rw-r--r--   0        0        0      342 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/create_call_agent_params_voice.py
+-rw-r--r--   0        0        0      187 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/create_call_agent_params_webhook.py
+-rw-r--r--   0        0        0      207 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/create_call_request_agent.py
+-rw-r--r--   0        0        0      329 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/create_voice_request.py
+-rw-r--r--   0        0        0      273 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/create_voice_response.py
+-rw-r--r--   0        0        0      931 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/dtmf_action.py
+-rw-r--r--   0        0        0      891 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/dtmf_action_params.py
+-rw-r--r--   0        0        0      932 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/dtmf_action_update_params.py
+-rw-r--r--   0        0        0      239 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/dtmf_action_update_params_config.py
+-rw-r--r--   0        0        0      953 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/eleven_labs_voice.py
+-rw-r--r--   0        0        0      913 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/eleven_labs_voice_params.py
+-rw-r--r--   0        0        0     1455 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/eleven_labs_voice_update_params.py
+-rw-r--r--   0        0        0      179 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/eleven_labs_voice_update_params_api_key.py
+-rw-r--r--   0        0        0      190 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/eleven_labs_voice_update_params_similarity_boost.py
+-rw-r--r--   0        0        0      184 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/eleven_labs_voice_update_params_stability.py
+-rw-r--r--   0        0        0      180 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/eleven_labs_voice_update_params_voice_id.py
+-rw-r--r--   0        0        0      736 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/empty_action_config.py
+-rw-r--r--   0        0        0      942 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/end_conversation_action.py
+-rw-r--r--   0        0        0      902 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/end_conversation_action_params.py
+-rw-r--r--   0        0        0      977 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/end_conversation_action_update_params.py
+-rw-r--r--   0        0        0      250 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/end_conversation_action_update_params_config.py
+-rw-r--r--   0        0        0     1395 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/event_type.py
+-rw-r--r--   0        0        0      317 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/get_action_response.py
+-rw-r--r--   0        0        0      270 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/get_voice_response.py
+-rw-r--r--   0        0        0      466 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/http_method.py
+-rw-r--r--   0        0        0      843 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/http_validation_error.py
+-rw-r--r--   0        0        0      496 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/interrupt_sensitivity.py
+-rw-r--r--   0        0        0      564 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/language.py
+-rw-r--r--   0        0        0      806 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/page.py
+-rw-r--r--   0        0        0      892 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/phone_number.py
+-rw-r--r--   0        0        0      927 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/pinecone_vector_database.py
+-rw-r--r--   0        0        0      887 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/pinecone_vector_database_params.py
+-rw-r--r--   0        0        0     1378 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/pinecone_vector_database_update_params.py
+-rw-r--r--   0        0        0      194 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/pinecone_vector_database_update_params_api_environment.py
+-rw-r--r--   0        0        0      186 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/pinecone_vector_database_update_params_api_key.py
+-rw-r--r--   0        0        0      185 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/pinecone_vector_database_update_params_index.py
+-rw-r--r--   0        0        0      674 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/plan_type.py
+-rw-r--r--   0        0        0      846 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/rime_voice.py
+-rw-r--r--   0        0        0      806 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/rime_voice_params.py
+-rw-r--r--   0        0        0      929 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/rime_voice_update_params.py
+-rw-r--r--   0        0        0      174 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/rime_voice_update_params_speaker.py
+-rw-r--r--   0        0        0      925 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/transfer_call_action.py
+-rw-r--r--   0        0        0      885 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/transfer_call_action_params.py
+-rw-r--r--   0        0        0      965 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/transfer_call_action_update_params.py
+-rw-r--r--   0        0        0      250 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/transfer_call_action_update_params_config.py
+-rw-r--r--   0        0        0      760 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/transfer_call_config.py
+-rw-r--r--   0        0        0      728 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/undefined.py
+-rw-r--r--   0        0        0      443 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/update_action_request_body.py
+-rw-r--r--   0        0        0      320 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/update_action_response.py
+-rw-r--r--   0        0        0      247 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/update_number_request_inbound_agent.py
+-rw-r--r--   0        0        0      170 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/update_number_request_label.py
+-rw-r--r--   0        0        0      390 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/update_voice_request_body.py
+-rw-r--r--   0        0        0      273 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/update_voice_response.py
+-rw-r--r--   0        0        0      866 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/usage.py
+-rw-r--r--   0        0        0      869 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/validation_error.py
+-rw-r--r--   0        0        0      128 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0      166 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/vector_database_type.py
+-rw-r--r--   0        0        0      753 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/voice_type.py
+-rw-r--r--   0        0        0      921 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/webhook.py
+-rw-r--r--   0        0        0      898 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/webhook_params.py
+-rw-r--r--   0        0        0     1124 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/webhook_update_params.py
+-rw-r--r--   0        0        0      214 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/webhook_update_params_method.py
+-rw-r--r--   0        0        0      231 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/webhook_update_params_subscriptions.py
+-rw-r--r--   0        0        0      168 2023-08-08 21:10:39.983218 vocode_api-0.0.5a6/src/vocode/types/webhook_update_params_url.py
+-rw-r--r--   0        0        0     3187 1970-01-01 00:00:00.000000 vocode_api-0.0.5a6/PKG-INFO
```

### Comparing `vocode_api-0.0.5a5/README.md` & `vocode_api-0.0.5a6/README.md`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a5/src/vocode/__init__.py` & `vocode_api-0.0.5a6/src/vocode/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,45 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .errors import UnprocessableEntityError
-from .resources import actions, agents, calls, numbers, usage, voices, webhooks
+from .resources import actions, agents, calls, numbers, payment, usage, voices, webhooks
 from .types import (
     ActionType,
     Agent,
     AgentActionsItem,
-    AgentParams,
     AgentParamsActionsItem,
+    AgentParamsVectorDatabase,
     AgentParamsVoice,
     AgentParamsWebhook,
     AgentUpdateParams,
     AgentUpdateParamsActions,
     AgentUpdateParamsActionsAgentUpdateParamsActionsItem,
     AgentUpdateParamsInitialMessage,
+    AgentUpdateParamsInterruptSensitivity,
+    AgentUpdateParamsLanguage,
     AgentUpdateParamsPrompt,
+    AgentUpdateParamsVectorDatabase,
     AgentUpdateParamsVoice,
     AgentUpdateParamsWebhook,
     AgentVoice,
     AzureVoice,
     AzureVoiceParams,
     AzureVoiceUpdateParams,
     AzureVoiceUpdateParamsPitch,
     AzureVoiceUpdateParamsRate,
     AzureVoiceUpdateParamsVoiceName,
     Call,
     CallStatus,
     CreateActionRequest,
     CreateActionResponse,
+    CreateCallAgentParams,
+    CreateCallAgentParamsActionsItem,
+    CreateCallAgentParamsVectorDatabase,
+    CreateCallAgentParamsVoice,
+    CreateCallAgentParamsWebhook,
     CreateCallRequestAgent,
     CreateVoiceRequest,
     CreateVoiceResponse,
     DtmfAction,
     DtmfActionParams,
     DtmfActionUpdateParams,
     DtmfActionUpdateParamsConfig,
@@ -48,74 +56,88 @@
     EndConversationActionUpdateParams,
     EndConversationActionUpdateParamsConfig,
     EventType,
     GetActionResponse,
     GetVoiceResponse,
     HttpMethod,
     HttpValidationError,
-    ListActionsResponseItem,
-    ListVoicesResponseItem,
-    NormalizedAgent,
-    NormalizedCall,
-    NormalizedPhoneNumber,
+    InterruptSensitivity,
+    Language,
+    Page,
     PhoneNumber,
+    PineconeVectorDatabase,
+    PineconeVectorDatabaseParams,
+    PineconeVectorDatabaseUpdateParams,
+    PineconeVectorDatabaseUpdateParamsApiEnvironment,
+    PineconeVectorDatabaseUpdateParamsApiKey,
+    PineconeVectorDatabaseUpdateParamsIndex,
     PlanType,
     RimeVoice,
     RimeVoiceParams,
     RimeVoiceUpdateParams,
     RimeVoiceUpdateParamsSpeaker,
     TransferCallAction,
     TransferCallActionParams,
     TransferCallActionUpdateParams,
     TransferCallActionUpdateParamsConfig,
     TransferCallConfig,
     Undefined,
     UpdateActionRequestBody,
     UpdateActionResponse,
     UpdateNumberRequestInboundAgent,
+    UpdateNumberRequestLabel,
     UpdateVoiceRequestBody,
     UpdateVoiceResponse,
     Usage,
     ValidationError,
     ValidationErrorLocItem,
+    VectorDatabaseType,
     VoiceType,
     Webhook,
     WebhookParams,
     WebhookUpdateParams,
     WebhookUpdateParamsMethod,
     WebhookUpdateParamsSubscriptions,
     WebhookUpdateParamsUrl,
 )
 
 __all__ = [
     "ActionType",
     "Agent",
     "AgentActionsItem",
-    "AgentParams",
     "AgentParamsActionsItem",
+    "AgentParamsVectorDatabase",
     "AgentParamsVoice",
     "AgentParamsWebhook",
     "AgentUpdateParams",
     "AgentUpdateParamsActions",
     "AgentUpdateParamsActionsAgentUpdateParamsActionsItem",
     "AgentUpdateParamsInitialMessage",
+    "AgentUpdateParamsInterruptSensitivity",
+    "AgentUpdateParamsLanguage",
     "AgentUpdateParamsPrompt",
+    "AgentUpdateParamsVectorDatabase",
     "AgentUpdateParamsVoice",
     "AgentUpdateParamsWebhook",
     "AgentVoice",
     "AzureVoice",
     "AzureVoiceParams",
     "AzureVoiceUpdateParams",
     "AzureVoiceUpdateParamsPitch",
     "AzureVoiceUpdateParamsRate",
     "AzureVoiceUpdateParamsVoiceName",
     "Call",
     "CallStatus",
     "CreateActionRequest",
     "CreateActionResponse",
+    "CreateCallAgentParams",
+    "CreateCallAgentParamsActionsItem",
+    "CreateCallAgentParamsVectorDatabase",
+    "CreateCallAgentParamsVoice",
+    "CreateCallAgentParamsWebhook",
     "CreateCallRequestAgent",
     "CreateVoiceRequest",
     "CreateVoiceResponse",
     "DtmfAction",
     "DtmfActionParams",
     "DtmfActionUpdateParams",
     "DtmfActionUpdateParamsConfig",
@@ -132,20 +154,24 @@
     "EndConversationActionUpdateParams",
     "EndConversationActionUpdateParamsConfig",
     "EventType",
     "GetActionResponse",
     "GetVoiceResponse",
     "HttpMethod",
     "HttpValidationError",
-    "ListActionsResponseItem",
-    "ListVoicesResponseItem",
-    "NormalizedAgent",
-    "NormalizedCall",
-    "NormalizedPhoneNumber",
+    "InterruptSensitivity",
+    "Language",
+    "Page",
     "PhoneNumber",
+    "PineconeVectorDatabase",
+    "PineconeVectorDatabaseParams",
+    "PineconeVectorDatabaseUpdateParams",
+    "PineconeVectorDatabaseUpdateParamsApiEnvironment",
+    "PineconeVectorDatabaseUpdateParamsApiKey",
+    "PineconeVectorDatabaseUpdateParamsIndex",
     "PlanType",
     "RimeVoice",
     "RimeVoiceParams",
     "RimeVoiceUpdateParams",
     "RimeVoiceUpdateParamsSpeaker",
     "TransferCallAction",
     "TransferCallActionParams",
@@ -153,27 +179,30 @@
     "TransferCallActionUpdateParamsConfig",
     "TransferCallConfig",
     "Undefined",
     "UnprocessableEntityError",
     "UpdateActionRequestBody",
     "UpdateActionResponse",
     "UpdateNumberRequestInboundAgent",
+    "UpdateNumberRequestLabel",
     "UpdateVoiceRequestBody",
     "UpdateVoiceResponse",
     "Usage",
     "ValidationError",
     "ValidationErrorLocItem",
+    "VectorDatabaseType",
     "VoiceType",
     "Webhook",
     "WebhookParams",
     "WebhookUpdateParams",
     "WebhookUpdateParamsMethod",
     "WebhookUpdateParamsSubscriptions",
     "WebhookUpdateParamsUrl",
     "actions",
     "agents",
     "calls",
     "numbers",
+    "payment",
     "usage",
     "voices",
     "webhooks",
 ]
```

### Comparing `vocode_api-0.0.5a5/src/vocode/client.py` & `vocode_api-0.0.5a6/src/vocode/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 # This file was auto-generated by Fern from our API Definition.
 
+import typing
+
 from .resources.actions.client import ActionsClient, AsyncActionsClient
 from .resources.agents.client import AgentsClient, AsyncAgentsClient
 from .resources.calls.client import AsyncCallsClient, CallsClient
 from .resources.numbers.client import AsyncNumbersClient, NumbersClient
+from .resources.payment.client import AsyncPaymentClient, PaymentClient
 from .resources.usage.client import AsyncUsageClient, UsageClient
 from .resources.voices.client import AsyncVoicesClient, VoicesClient
 from .resources.webhooks.client import AsyncWebhooksClient, WebhooksClient
 
 
 class Vocode:
-    def __init__(self, *, environment: str, token: str):
+    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
         self._token = token
         self.numbers = NumbersClient(environment=self._environment, token=self._token)
         self.calls = CallsClient(environment=self._environment, token=self._token)
         self.usage = UsageClient(environment=self._environment, token=self._token)
         self.actions = ActionsClient(environment=self._environment, token=self._token)
         self.agents = AgentsClient(environment=self._environment, token=self._token)
         self.voices = VoicesClient(environment=self._environment, token=self._token)
         self.webhooks = WebhooksClient(environment=self._environment, token=self._token)
+        self.payment = PaymentClient(environment=self._environment, token=self._token)
 
 
 class AsyncVocode:
-    def __init__(self, *, environment: str, token: str):
+    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
         self._token = token
         self.numbers = AsyncNumbersClient(environment=self._environment, token=self._token)
         self.calls = AsyncCallsClient(environment=self._environment, token=self._token)
         self.usage = AsyncUsageClient(environment=self._environment, token=self._token)
         self.actions = AsyncActionsClient(environment=self._environment, token=self._token)
         self.agents = AsyncAgentsClient(environment=self._environment, token=self._token)
         self.voices = AsyncVoicesClient(environment=self._environment, token=self._token)
         self.webhooks = AsyncWebhooksClient(environment=self._environment, token=self._token)
+        self.payment = AsyncPaymentClient(environment=self._environment, token=self._token)
```

### Comparing `vocode_api-0.0.5a5/src/vocode/core/datetime_utils.py` & `vocode_api-0.0.5a6/src/vocode/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a5/src/vocode/core/jsonable_encoder.py` & `vocode_api-0.0.5a6/src/vocode/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a5/src/vocode/resources/actions/client.py` & `vocode_api-0.0.5a6/src/vocode/resources/actions/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.create_action_request import CreateActionRequest
 from ...types.create_action_response import CreateActionResponse
 from ...types.get_action_response import GetActionResponse
 from ...types.http_validation_error import HttpValidationError
-from ...types.list_actions_response_item import ListActionsResponseItem
+from ...types.page import Page
 from ...types.update_action_request_body import UpdateActionRequestBody
 from ...types.update_action_response import UpdateActionResponse
 
 
 class ActionsClient:
-    def __init__(self, *, environment: str, token: str):
+    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
         self._token = token
 
     def get_action(self, *, id: str) -> GetActionResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "v1/actions"),
@@ -41,25 +41,28 @@
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def list_actions(self) -> typing.List[ListActionsResponseItem]:
+    def list_actions(self, *, page: typing.Optional[int] = None, size: typing.Optional[int] = None) -> Page:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "v1/actions/list"),
+            params={"page": page, "size": size},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[ListActionsResponseItem], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Page, _response.json())  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create_action(self, *, request: CreateActionRequest) -> CreateActionResponse:
@@ -101,15 +104,15 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncActionsClient:
-    def __init__(self, *, environment: str, token: str):
+    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
         self._token = token
 
     async def get_action(self, *, id: str) -> GetActionResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
@@ -126,26 +129,29 @@
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def list_actions(self) -> typing.List[ListActionsResponseItem]:
+    async def list_actions(self, *, page: typing.Optional[int] = None, size: typing.Optional[int] = None) -> Page:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "v1/actions/list"),
+                params={"page": page, "size": size},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[ListActionsResponseItem], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Page, _response.json())  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create_action(self, *, request: CreateActionRequest) -> CreateActionResponse:
```

### Comparing `vocode_api-0.0.5a5/src/vocode/resources/agents/client.py` & `vocode_api-0.0.5a6/src/vocode/resources/voices/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,184 +7,192 @@
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
-from ...types.agent import Agent
-from ...types.agent_params import AgentParams
-from ...types.agent_update_params import AgentUpdateParams
+from ...types.create_voice_request import CreateVoiceRequest
+from ...types.create_voice_response import CreateVoiceResponse
+from ...types.get_voice_response import GetVoiceResponse
 from ...types.http_validation_error import HttpValidationError
-from ...types.normalized_agent import NormalizedAgent
+from ...types.page import Page
+from ...types.update_voice_request_body import UpdateVoiceRequestBody
+from ...types.update_voice_response import UpdateVoiceResponse
 
 
-class AgentsClient:
-    def __init__(self, *, environment: str, token: str):
+class VoicesClient:
+    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
         self._token = token
 
-    def get_agent(self, *, id: str) -> Agent:
+    def get_voice(self, *, id: str) -> GetVoiceResponse:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/agents"),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/voices"),
             params={"id": id},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(Agent, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(GetVoiceResponse, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def list_agents(self) -> typing.List[NormalizedAgent]:
+    def list_voices(self, *, page: typing.Optional[int] = None, size: typing.Optional[int] = None) -> Page:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/agents/list"),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/voices/list"),
+            params={"page": page, "size": size},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[NormalizedAgent], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Page, _response.json())  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def create_agent(self, *, request: AgentParams) -> Agent:
+    def create_voice(self, *, request: CreateVoiceRequest) -> CreateVoiceResponse:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/agents/create"),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/voices/create"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(Agent, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(CreateVoiceResponse, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def update_agent(self, *, id: str, request: AgentUpdateParams) -> Agent:
+    def update_voice(self, *, id: str, request: UpdateVoiceRequestBody) -> UpdateVoiceResponse:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/agents/update"),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/voices/update"),
             params={"id": id},
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(Agent, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(UpdateVoiceResponse, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncAgentsClient:
-    def __init__(self, *, environment: str, token: str):
+class AsyncVoicesClient:
+    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
         self._token = token
 
-    async def get_agent(self, *, id: str) -> Agent:
+    async def get_voice(self, *, id: str) -> GetVoiceResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/agents"),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/voices"),
                 params={"id": id},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(Agent, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(GetVoiceResponse, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def list_agents(self) -> typing.List[NormalizedAgent]:
+    async def list_voices(self, *, page: typing.Optional[int] = None, size: typing.Optional[int] = None) -> Page:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/agents/list"),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/voices/list"),
+                params={"page": page, "size": size},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[NormalizedAgent], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Page, _response.json())  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def create_agent(self, *, request: AgentParams) -> Agent:
+    async def create_voice(self, *, request: CreateVoiceRequest) -> CreateVoiceResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/agents/create"),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/voices/create"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(Agent, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(CreateVoiceResponse, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def update_agent(self, *, id: str, request: AgentUpdateParams) -> Agent:
+    async def update_voice(self, *, id: str, request: UpdateVoiceRequestBody) -> UpdateVoiceResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/agents/update"),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/voices/update"),
                 params={"id": id},
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(Agent, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(UpdateVoiceResponse, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `vocode_api-0.0.5a5/src/vocode/resources/calls/client.py` & `vocode_api-0.0.5a6/src/vocode/resources/calls/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,33 +10,36 @@
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.call import Call
 from ...types.create_call_request_agent import CreateCallRequestAgent
 from ...types.http_validation_error import HttpValidationError
-from ...types.normalized_call import NormalizedCall
+from ...types.page import Page
 
 
 class CallsClient:
-    def __init__(self, *, environment: str, token: str):
+    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
         self._token = token
 
-    def list_calls(self) -> typing.List[NormalizedCall]:
+    def list_calls(self, *, page: typing.Optional[int] = None, size: typing.Optional[int] = None) -> Page:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "v1/calls/list"),
+            params={"page": page, "size": size},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[NormalizedCall], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Page, _response.json())  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_call(self, *, id: str) -> Call:
@@ -117,30 +120,33 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncCallsClient:
-    def __init__(self, *, environment: str, token: str):
+    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
         self._token = token
 
-    async def list_calls(self) -> typing.List[NormalizedCall]:
+    async def list_calls(self, *, page: typing.Optional[int] = None, size: typing.Optional[int] = None) -> Page:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "v1/calls/list"),
+                params={"page": page, "size": size},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[NormalizedCall], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Page, _response.json())  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_call(self, *, id: str) -> Call:
```

### Comparing `vocode_api-0.0.5a5/src/vocode/resources/numbers/client.py` & `vocode_api-0.0.5a6/src/vocode/resources/numbers/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,35 +8,42 @@
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.http_validation_error import HttpValidationError
-from ...types.normalized_phone_number import NormalizedPhoneNumber
+from ...types.page import Page
 from ...types.phone_number import PhoneNumber
 from ...types.update_number_request_inbound_agent import UpdateNumberRequestInboundAgent
+from ...types.update_number_request_label import UpdateNumberRequestLabel
+
+# this is used as the default value for optional parameters
+OMIT = typing.cast(typing.Any, ...)
 
 
 class NumbersClient:
-    def __init__(self, *, environment: str, token: str):
+    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
         self._token = token
 
-    def list_numbers(self) -> typing.List[NormalizedPhoneNumber]:
+    def list_numbers(self, *, page: typing.Optional[int] = None, size: typing.Optional[int] = None) -> Page:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "v1/numbers/list"),
+            params={"page": page, "size": size},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[NormalizedPhoneNumber], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Page, _response.json())  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_number(self, *, phone_number: str) -> PhoneNumber:
@@ -72,20 +79,31 @@
             return pydantic.parse_obj_as(PhoneNumber, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def update_number(self, *, phone_number: str, inbound_agent: UpdateNumberRequestInboundAgent) -> PhoneNumber:
+    def update_number(
+        self,
+        *,
+        phone_number: str,
+        label: typing.Optional[UpdateNumberRequestLabel] = OMIT,
+        inbound_agent: typing.Optional[UpdateNumberRequestInboundAgent] = OMIT,
+    ) -> PhoneNumber:
+        _request: typing.Dict[str, typing.Any] = {}
+        if label is not OMIT:
+            _request["label"] = label
+        if inbound_agent is not OMIT:
+            _request["inbound_agent"] = inbound_agent
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment}/", "v1/numbers/update"),
             params={"phone_number": phone_number},
-            json=jsonable_encoder({"inbound_agent": inbound_agent}),
+            json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PhoneNumber, _response.json())  # type: ignore
@@ -115,30 +133,33 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncNumbersClient:
-    def __init__(self, *, environment: str, token: str):
+    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
         self._token = token
 
-    async def list_numbers(self) -> typing.List[NormalizedPhoneNumber]:
+    async def list_numbers(self, *, page: typing.Optional[int] = None, size: typing.Optional[int] = None) -> Page:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment}/", "v1/numbers/list"),
+                params={"page": page, "size": size},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[NormalizedPhoneNumber], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Page, _response.json())  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_number(self, *, phone_number: str) -> PhoneNumber:
@@ -176,21 +197,32 @@
             return pydantic.parse_obj_as(PhoneNumber, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def update_number(self, *, phone_number: str, inbound_agent: UpdateNumberRequestInboundAgent) -> PhoneNumber:
+    async def update_number(
+        self,
+        *,
+        phone_number: str,
+        label: typing.Optional[UpdateNumberRequestLabel] = OMIT,
+        inbound_agent: typing.Optional[UpdateNumberRequestInboundAgent] = OMIT,
+    ) -> PhoneNumber:
+        _request: typing.Dict[str, typing.Any] = {}
+        if label is not OMIT:
+            _request["label"] = label
+        if inbound_agent is not OMIT:
+            _request["inbound_agent"] = inbound_agent
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment}/", "v1/numbers/update"),
                 params={"phone_number": phone_number},
-                json=jsonable_encoder({"inbound_agent": inbound_agent}),
+                json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(PhoneNumber, _response.json())  # type: ignore
```

### Comparing `vocode_api-0.0.5a5/src/vocode/resources/usage/client.py` & `vocode_api-0.0.5a6/src/vocode/resources/usage/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
+import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...types.usage import Usage
 
 
 class UsageClient:
-    def __init__(self, *, environment: str, token: str):
+    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
         self._token = token
 
     def get_usage(self) -> Usage:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment}/", "v1/usage"),
@@ -31,15 +32,15 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncUsageClient:
-    def __init__(self, *, environment: str, token: str):
+    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
         self._token = token
 
     async def get_usage(self) -> Usage:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
```

### Comparing `vocode_api-0.0.5a5/src/vocode/resources/voices/client.py` & `vocode_api-0.0.5a6/src/vocode/resources/webhooks/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,186 +7,190 @@
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
-from ...types.create_voice_request import CreateVoiceRequest
-from ...types.create_voice_response import CreateVoiceResponse
-from ...types.get_voice_response import GetVoiceResponse
 from ...types.http_validation_error import HttpValidationError
-from ...types.list_voices_response_item import ListVoicesResponseItem
-from ...types.update_voice_request_body import UpdateVoiceRequestBody
-from ...types.update_voice_response import UpdateVoiceResponse
+from ...types.page import Page
+from ...types.webhook import Webhook
+from ...types.webhook_params import WebhookParams
+from ...types.webhook_update_params import WebhookUpdateParams
 
 
-class VoicesClient:
-    def __init__(self, *, environment: str, token: str):
+class WebhooksClient:
+    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
         self._token = token
 
-    def get_voice(self, *, id: str) -> GetVoiceResponse:
+    def get_webhook(self, *, id: str) -> Webhook:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/voices"),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/webhooks"),
             params={"id": id},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GetVoiceResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Webhook, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def list_voices(self) -> typing.List[ListVoicesResponseItem]:
+    def list_webhooks(self, *, page: typing.Optional[int] = None, size: typing.Optional[int] = None) -> Page:
         _response = httpx.request(
             "GET",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/voices/list"),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/webhooks/list"),
+            params={"page": page, "size": size},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[ListVoicesResponseItem], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Page, _response.json())  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def create_voice(self, *, request: CreateVoiceRequest) -> CreateVoiceResponse:
+    def create_webhook(self, *, request: WebhookParams) -> Webhook:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/voices/create"),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/webhooks/create"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CreateVoiceResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Webhook, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def update_voice(self, *, id: str, request: UpdateVoiceRequestBody) -> UpdateVoiceResponse:
+    def update_webhook(self, *, id: str, request: WebhookUpdateParams) -> Webhook:
         _response = httpx.request(
             "POST",
-            urllib.parse.urljoin(f"{self._environment}/", "v1/voices/update"),
+            urllib.parse.urljoin(f"{self._environment}/", "v1/webhooks/update"),
             params={"id": id},
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(UpdateVoiceResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Webhook, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncVoicesClient:
-    def __init__(self, *, environment: str, token: str):
+class AsyncWebhooksClient:
+    def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
         self._token = token
 
-    async def get_voice(self, *, id: str) -> GetVoiceResponse:
+    async def get_webhook(self, *, id: str) -> Webhook:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/voices"),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/webhooks"),
                 params={"id": id},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(GetVoiceResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Webhook, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def list_voices(self) -> typing.List[ListVoicesResponseItem]:
+    async def list_webhooks(self, *, page: typing.Optional[int] = None, size: typing.Optional[int] = None) -> Page:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/voices/list"),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/webhooks/list"),
+                params={"page": page, "size": size},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[ListVoicesResponseItem], _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Page, _response.json())  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def create_voice(self, *, request: CreateVoiceRequest) -> CreateVoiceResponse:
+    async def create_webhook(self, *, request: WebhookParams) -> Webhook:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/voices/create"),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/webhooks/create"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(CreateVoiceResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Webhook, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def update_voice(self, *, id: str, request: UpdateVoiceRequestBody) -> UpdateVoiceResponse:
+    async def update_webhook(self, *, id: str, request: WebhookUpdateParams) -> Webhook:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
-                urllib.parse.urljoin(f"{self._environment}/", "v1/voices/update"),
+                urllib.parse.urljoin(f"{self._environment}/", "v1/webhooks/update"),
                 params={"id": id},
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(UpdateVoiceResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Webhook, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `vocode_api-0.0.5a5/src/vocode/types/__init__.py` & `vocode_api-0.0.5a6/src/vocode/types/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .action_type import ActionType
 from .agent import Agent
 from .agent_actions_item import AgentActionsItem
-from .agent_params import AgentParams
 from .agent_params_actions_item import AgentParamsActionsItem
+from .agent_params_vector_database import AgentParamsVectorDatabase
 from .agent_params_voice import AgentParamsVoice
 from .agent_params_webhook import AgentParamsWebhook
 from .agent_update_params import AgentUpdateParams
 from .agent_update_params_actions import AgentUpdateParamsActions
 from .agent_update_params_actions_agent_update_params_actions_item import (
     AgentUpdateParamsActionsAgentUpdateParamsActionsItem,
 )
 from .agent_update_params_initial_message import AgentUpdateParamsInitialMessage
+from .agent_update_params_interrupt_sensitivity import AgentUpdateParamsInterruptSensitivity
+from .agent_update_params_language import AgentUpdateParamsLanguage
 from .agent_update_params_prompt import AgentUpdateParamsPrompt
+from .agent_update_params_vector_database import AgentUpdateParamsVectorDatabase
 from .agent_update_params_voice import AgentUpdateParamsVoice
 from .agent_update_params_webhook import AgentUpdateParamsWebhook
 from .agent_voice import AgentVoice
 from .azure_voice import AzureVoice
 from .azure_voice_params import AzureVoiceParams
 from .azure_voice_update_params import AzureVoiceUpdateParams
 from .azure_voice_update_params_pitch import AzureVoiceUpdateParamsPitch
 from .azure_voice_update_params_rate import AzureVoiceUpdateParamsRate
 from .azure_voice_update_params_voice_name import AzureVoiceUpdateParamsVoiceName
 from .call import Call
 from .call_status import CallStatus
 from .create_action_request import CreateActionRequest
 from .create_action_response import CreateActionResponse
+from .create_call_agent_params import CreateCallAgentParams
+from .create_call_agent_params_actions_item import CreateCallAgentParamsActionsItem
+from .create_call_agent_params_vector_database import CreateCallAgentParamsVectorDatabase
+from .create_call_agent_params_voice import CreateCallAgentParamsVoice
+from .create_call_agent_params_webhook import CreateCallAgentParamsWebhook
 from .create_call_request_agent import CreateCallRequestAgent
 from .create_voice_request import CreateVoiceRequest
 from .create_voice_response import CreateVoiceResponse
 from .dtmf_action import DtmfAction
 from .dtmf_action_params import DtmfActionParams
 from .dtmf_action_update_params import DtmfActionUpdateParams
 from .dtmf_action_update_params_config import DtmfActionUpdateParamsConfig
@@ -47,73 +55,87 @@
 from .end_conversation_action_update_params import EndConversationActionUpdateParams
 from .end_conversation_action_update_params_config import EndConversationActionUpdateParamsConfig
 from .event_type import EventType
 from .get_action_response import GetActionResponse
 from .get_voice_response import GetVoiceResponse
 from .http_method import HttpMethod
 from .http_validation_error import HttpValidationError
-from .list_actions_response_item import ListActionsResponseItem
-from .list_voices_response_item import ListVoicesResponseItem
-from .normalized_agent import NormalizedAgent
-from .normalized_call import NormalizedCall
-from .normalized_phone_number import NormalizedPhoneNumber
+from .interrupt_sensitivity import InterruptSensitivity
+from .language import Language
+from .page import Page
 from .phone_number import PhoneNumber
+from .pinecone_vector_database import PineconeVectorDatabase
+from .pinecone_vector_database_params import PineconeVectorDatabaseParams
+from .pinecone_vector_database_update_params import PineconeVectorDatabaseUpdateParams
+from .pinecone_vector_database_update_params_api_environment import PineconeVectorDatabaseUpdateParamsApiEnvironment
+from .pinecone_vector_database_update_params_api_key import PineconeVectorDatabaseUpdateParamsApiKey
+from .pinecone_vector_database_update_params_index import PineconeVectorDatabaseUpdateParamsIndex
 from .plan_type import PlanType
 from .rime_voice import RimeVoice
 from .rime_voice_params import RimeVoiceParams
 from .rime_voice_update_params import RimeVoiceUpdateParams
 from .rime_voice_update_params_speaker import RimeVoiceUpdateParamsSpeaker
 from .transfer_call_action import TransferCallAction
 from .transfer_call_action_params import TransferCallActionParams
 from .transfer_call_action_update_params import TransferCallActionUpdateParams
 from .transfer_call_action_update_params_config import TransferCallActionUpdateParamsConfig
 from .transfer_call_config import TransferCallConfig
 from .undefined import Undefined
 from .update_action_request_body import UpdateActionRequestBody
 from .update_action_response import UpdateActionResponse
 from .update_number_request_inbound_agent import UpdateNumberRequestInboundAgent
+from .update_number_request_label import UpdateNumberRequestLabel
 from .update_voice_request_body import UpdateVoiceRequestBody
 from .update_voice_response import UpdateVoiceResponse
 from .usage import Usage
 from .validation_error import ValidationError
 from .validation_error_loc_item import ValidationErrorLocItem
+from .vector_database_type import VectorDatabaseType
 from .voice_type import VoiceType
 from .webhook import Webhook
 from .webhook_params import WebhookParams
 from .webhook_update_params import WebhookUpdateParams
 from .webhook_update_params_method import WebhookUpdateParamsMethod
 from .webhook_update_params_subscriptions import WebhookUpdateParamsSubscriptions
 from .webhook_update_params_url import WebhookUpdateParamsUrl
 
 __all__ = [
     "ActionType",
     "Agent",
     "AgentActionsItem",
-    "AgentParams",
     "AgentParamsActionsItem",
+    "AgentParamsVectorDatabase",
     "AgentParamsVoice",
     "AgentParamsWebhook",
     "AgentUpdateParams",
     "AgentUpdateParamsActions",
     "AgentUpdateParamsActionsAgentUpdateParamsActionsItem",
     "AgentUpdateParamsInitialMessage",
+    "AgentUpdateParamsInterruptSensitivity",
+    "AgentUpdateParamsLanguage",
     "AgentUpdateParamsPrompt",
+    "AgentUpdateParamsVectorDatabase",
     "AgentUpdateParamsVoice",
     "AgentUpdateParamsWebhook",
     "AgentVoice",
     "AzureVoice",
     "AzureVoiceParams",
     "AzureVoiceUpdateParams",
     "AzureVoiceUpdateParamsPitch",
     "AzureVoiceUpdateParamsRate",
     "AzureVoiceUpdateParamsVoiceName",
     "Call",
     "CallStatus",
     "CreateActionRequest",
     "CreateActionResponse",
+    "CreateCallAgentParams",
+    "CreateCallAgentParamsActionsItem",
+    "CreateCallAgentParamsVectorDatabase",
+    "CreateCallAgentParamsVoice",
+    "CreateCallAgentParamsWebhook",
     "CreateCallRequestAgent",
     "CreateVoiceRequest",
     "CreateVoiceResponse",
     "DtmfAction",
     "DtmfActionParams",
     "DtmfActionUpdateParams",
     "DtmfActionUpdateParamsConfig",
@@ -130,39 +152,45 @@
     "EndConversationActionUpdateParams",
     "EndConversationActionUpdateParamsConfig",
     "EventType",
     "GetActionResponse",
     "GetVoiceResponse",
     "HttpMethod",
     "HttpValidationError",
-    "ListActionsResponseItem",
-    "ListVoicesResponseItem",
-    "NormalizedAgent",
-    "NormalizedCall",
-    "NormalizedPhoneNumber",
+    "InterruptSensitivity",
+    "Language",
+    "Page",
     "PhoneNumber",
+    "PineconeVectorDatabase",
+    "PineconeVectorDatabaseParams",
+    "PineconeVectorDatabaseUpdateParams",
+    "PineconeVectorDatabaseUpdateParamsApiEnvironment",
+    "PineconeVectorDatabaseUpdateParamsApiKey",
+    "PineconeVectorDatabaseUpdateParamsIndex",
     "PlanType",
     "RimeVoice",
     "RimeVoiceParams",
     "RimeVoiceUpdateParams",
     "RimeVoiceUpdateParamsSpeaker",
     "TransferCallAction",
     "TransferCallActionParams",
     "TransferCallActionUpdateParams",
     "TransferCallActionUpdateParamsConfig",
     "TransferCallConfig",
     "Undefined",
     "UpdateActionRequestBody",
     "UpdateActionResponse",
     "UpdateNumberRequestInboundAgent",
+    "UpdateNumberRequestLabel",
     "UpdateVoiceRequestBody",
     "UpdateVoiceResponse",
     "Usage",
     "ValidationError",
     "ValidationErrorLocItem",
+    "VectorDatabaseType",
     "VoiceType",
     "Webhook",
     "WebhookParams",
     "WebhookUpdateParams",
     "WebhookUpdateParamsMethod",
     "WebhookUpdateParamsSubscriptions",
     "WebhookUpdateParamsUrl",
```

### Comparing `vocode_api-0.0.5a5/src/vocode/types/action_type.py` & `vocode_api-0.0.5a6/src/vocode/types/action_type.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a5/src/vocode/types/agent.py` & `vocode_api-0.0.5a6/src/vocode/types/usage.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,27 +2,22 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .agent_actions_item import AgentActionsItem
-from .agent_voice import AgentVoice
-from .webhook import Webhook
+from .plan_type import PlanType
 
 
-class Agent(pydantic.BaseModel):
-    id: str
+class Usage(pydantic.BaseModel):
     user_id: str
-    prompt: str
-    actions: typing.List[AgentActionsItem]
-    voice: AgentVoice
-    initial_message: typing.Optional[str]
-    webhook: typing.Optional[Webhook]
+    plan_type: PlanType
+    monthly_usage_minutes: int
+    monthly_usage_limit_minutes: int
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vocode_api-0.0.5a5/src/vocode/types/agent_params.py` & `vocode_api-0.0.5a6/src/vocode/types/transfer_call_action.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,25 +2,23 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .agent_params_actions_item import AgentParamsActionsItem
-from .agent_params_voice import AgentParamsVoice
-from .agent_params_webhook import AgentParamsWebhook
+from .action_type import ActionType
+from .transfer_call_config import TransferCallConfig
 
 
-class AgentParams(pydantic.BaseModel):
-    prompt: str
-    actions: typing.Optional[typing.List[AgentParamsActionsItem]]
-    voice: AgentParamsVoice
-    initial_message: typing.Optional[str]
-    webhook: typing.Optional[AgentParamsWebhook]
+class TransferCallAction(pydantic.BaseModel):
+    id: str
+    user_id: str
+    type: typing.Optional[ActionType]
+    config: TransferCallConfig
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vocode_api-0.0.5a5/src/vocode/types/agent_update_params.py` & `vocode_api-0.0.5a6/src/vocode/types/agent_update_params.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,25 +4,31 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 from .agent_update_params_actions import AgentUpdateParamsActions
 from .agent_update_params_initial_message import AgentUpdateParamsInitialMessage
+from .agent_update_params_interrupt_sensitivity import AgentUpdateParamsInterruptSensitivity
+from .agent_update_params_language import AgentUpdateParamsLanguage
 from .agent_update_params_prompt import AgentUpdateParamsPrompt
+from .agent_update_params_vector_database import AgentUpdateParamsVectorDatabase
 from .agent_update_params_voice import AgentUpdateParamsVoice
 from .agent_update_params_webhook import AgentUpdateParamsWebhook
 
 
 class AgentUpdateParams(pydantic.BaseModel):
     prompt: typing.Optional[AgentUpdateParamsPrompt]
+    language: typing.Optional[AgentUpdateParamsLanguage]
     actions: typing.Optional[AgentUpdateParamsActions]
     voice: typing.Optional[AgentUpdateParamsVoice]
     initial_message: typing.Optional[AgentUpdateParamsInitialMessage]
     webhook: typing.Optional[AgentUpdateParamsWebhook]
+    vector_database: typing.Optional[AgentUpdateParamsVectorDatabase]
+    interrupt_sensitivity: typing.Optional[AgentUpdateParamsInterruptSensitivity]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vocode_api-0.0.5a5/src/vocode/types/azure_voice.py` & `vocode_api-0.0.5a6/src/vocode/types/azure_voice.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a5/src/vocode/types/azure_voice_params.py` & `vocode_api-0.0.5a6/src/vocode/types/azure_voice_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a5/src/vocode/types/azure_voice_update_params.py` & `vocode_api-0.0.5a6/src/vocode/types/azure_voice_update_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a5/src/vocode/types/call.py` & `vocode_api-0.0.5a6/src/vocode/types/call.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a5/src/vocode/types/call_status.py` & `vocode_api-0.0.5a6/src/vocode/types/call_status.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a5/src/vocode/types/dtmf_action.py` & `vocode_api-0.0.5a6/src/vocode/types/dtmf_action.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a5/src/vocode/types/dtmf_action_params.py` & `vocode_api-0.0.5a6/src/vocode/types/dtmf_action_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a5/src/vocode/types/dtmf_action_update_params.py` & `vocode_api-0.0.5a6/src/vocode/types/dtmf_action_update_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a5/src/vocode/types/eleven_labs_voice.py` & `vocode_api-0.0.5a6/src/vocode/types/eleven_labs_voice.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a5/src/vocode/types/eleven_labs_voice_params.py` & `vocode_api-0.0.5a6/src/vocode/types/eleven_labs_voice_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a5/src/vocode/types/eleven_labs_voice_update_params.py` & `vocode_api-0.0.5a6/src/vocode/types/eleven_labs_voice_update_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a5/src/vocode/types/empty_action_config.py` & `vocode_api-0.0.5a6/src/vocode/types/empty_action_config.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a5/src/vocode/types/end_conversation_action.py` & `vocode_api-0.0.5a6/src/vocode/types/end_conversation_action.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a5/src/vocode/types/end_conversation_action_params.py` & `vocode_api-0.0.5a6/src/vocode/types/end_conversation_action_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a5/src/vocode/types/end_conversation_action_update_params.py` & `vocode_api-0.0.5a6/src/vocode/types/end_conversation_action_update_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a5/src/vocode/types/event_type.py` & `vocode_api-0.0.5a6/src/vocode/types/event_type.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a5/src/vocode/types/http_validation_error.py` & `vocode_api-0.0.5a6/src/vocode/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a5/src/vocode/types/normalized_agent.py` & `vocode_api-0.0.5a6/src/vocode/types/phone_number.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
+from .agent import Agent
 
 
-class NormalizedAgent(pydantic.BaseModel):
+class PhoneNumber(pydantic.BaseModel):
     id: str
     user_id: str
-    prompt: str
-    actions: typing.List[str]
-    voice: str
-    initial_message: typing.Optional[str]
-    webhook: typing.Optional[str]
+    active: typing.Optional[bool]
+    label: typing.Optional[str]
+    inbound_agent: Agent
+    number: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vocode_api-0.0.5a5/src/vocode/types/normalized_call.py` & `vocode_api-0.0.5a6/src/vocode/types/agent.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,27 +2,33 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .call_status import CallStatus
+from .agent_actions_item import AgentActionsItem
+from .agent_voice import AgentVoice
+from .interrupt_sensitivity import InterruptSensitivity
+from .language import Language
+from .pinecone_vector_database import PineconeVectorDatabase
+from .webhook import Webhook
 
 
-class NormalizedCall(pydantic.BaseModel):
+class Agent(pydantic.BaseModel):
     id: str
     user_id: str
-    status: typing.Optional[CallStatus]
-    error_message: typing.Optional[str]
-    recording_available: typing.Optional[bool]
-    transcript: typing.Optional[str]
-    to_number: str
-    from_number: str
-    agent: str
+    prompt: str
+    language: typing.Optional[Language]
+    actions: typing.List[AgentActionsItem]
+    voice: AgentVoice
+    initial_message: typing.Optional[str]
+    webhook: typing.Optional[Webhook]
+    vector_database: typing.Optional[PineconeVectorDatabase]
+    interrupt_sensitivity: typing.Optional[InterruptSensitivity]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vocode_api-0.0.5a5/src/vocode/types/normalized_phone_number.py` & `vocode_api-0.0.5a6/src/vocode/types/webhook_params.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
+from .event_type import EventType
+from .http_method import HttpMethod
 
 
-class NormalizedPhoneNumber(pydantic.BaseModel):
-    id: str
-    user_id: str
-    active: typing.Optional[bool]
-    inbound_agent: str
-    number: str
+class WebhookParams(pydantic.BaseModel):
+    subscriptions: typing.List[EventType]
+    url: str
+    method: typing.Optional[HttpMethod]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vocode_api-0.0.5a5/src/vocode/types/phone_number.py` & `vocode_api-0.0.5a6/src/vocode/types/rime_voice_params.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,23 +2,20 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .agent import Agent
+from .voice_type import VoiceType
 
 
-class PhoneNumber(pydantic.BaseModel):
-    id: str
-    user_id: str
-    active: typing.Optional[bool]
-    inbound_agent: Agent
-    number: str
+class RimeVoiceParams(pydantic.BaseModel):
+    type: VoiceType
+    speaker: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vocode_api-0.0.5a5/src/vocode/types/plan_type.py` & `vocode_api-0.0.5a6/src/vocode/types/plan_type.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a5/src/vocode/types/rime_voice.py` & `vocode_api-0.0.5a6/src/vocode/types/rime_voice.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a5/src/vocode/types/rime_voice_params.py` & `vocode_api-0.0.5a6/src/vocode/types/pinecone_vector_database_params.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .voice_type import VoiceType
+from .vector_database_type import VectorDatabaseType
 
 
-class RimeVoiceParams(pydantic.BaseModel):
-    type: VoiceType
-    speaker: str
+class PineconeVectorDatabaseParams(pydantic.BaseModel):
+    type: VectorDatabaseType
+    index: str
+    api_key: str
+    api_environment: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vocode_api-0.0.5a5/src/vocode/types/rime_voice_update_params.py` & `vocode_api-0.0.5a6/src/vocode/types/rime_voice_update_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a5/src/vocode/types/transfer_call_action.py` & `vocode_api-0.0.5a6/src/vocode/types/transfer_call_action_update_params.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,22 +3,20 @@
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 from .action_type import ActionType
-from .transfer_call_config import TransferCallConfig
+from .transfer_call_action_update_params_config import TransferCallActionUpdateParamsConfig
 
 
-class TransferCallAction(pydantic.BaseModel):
-    id: str
-    user_id: str
-    type: typing.Optional[ActionType]
-    config: TransferCallConfig
+class TransferCallActionUpdateParams(pydantic.BaseModel):
+    type: ActionType
+    config: typing.Optional[TransferCallActionUpdateParamsConfig]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vocode_api-0.0.5a5/src/vocode/types/transfer_call_action_params.py` & `vocode_api-0.0.5a6/src/vocode/types/transfer_call_action_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a5/src/vocode/types/transfer_call_action_update_params.py` & `vocode_api-0.0.5a6/src/vocode/types/pinecone_vector_database.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,21 +2,24 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .action_type import ActionType
-from .transfer_call_action_update_params_config import TransferCallActionUpdateParamsConfig
+from .vector_database_type import VectorDatabaseType
 
 
-class TransferCallActionUpdateParams(pydantic.BaseModel):
-    type: ActionType
-    config: typing.Optional[TransferCallActionUpdateParamsConfig]
+class PineconeVectorDatabase(pydantic.BaseModel):
+    id: str
+    user_id: str
+    type: typing.Optional[VectorDatabaseType]
+    index: str
+    api_key: str
+    api_environment: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vocode_api-0.0.5a5/src/vocode/types/transfer_call_config.py` & `vocode_api-0.0.5a6/src/vocode/types/transfer_call_config.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a5/src/vocode/types/undefined.py` & `vocode_api-0.0.5a6/src/vocode/types/undefined.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.5a5/src/vocode/types/usage.py` & `vocode_api-0.0.5a6/src/vocode/types/validation_error.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .plan_type import PlanType
+from .validation_error_loc_item import ValidationErrorLocItem
 
 
-class Usage(pydantic.BaseModel):
-    user_id: str
-    plan_type: PlanType
-    monthly_usage_minutes: int
-    monthly_usage_limit_minutes: int
+class ValidationError(pydantic.BaseModel):
+    loc: typing.List[ValidationErrorLocItem]
+    msg: str
+    type: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vocode_api-0.0.5a5/src/vocode/types/validation_error.py` & `vocode_api-0.0.5a6/src/vocode/types/webhook.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,21 +2,24 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .validation_error_loc_item import ValidationErrorLocItem
+from .event_type import EventType
+from .http_method import HttpMethod
 
 
-class ValidationError(pydantic.BaseModel):
-    loc: typing.List[ValidationErrorLocItem]
-    msg: str
-    type: str
+class Webhook(pydantic.BaseModel):
+    id: str
+    user_id: str
+    subscriptions: typing.List[EventType]
+    url: str
+    method: typing.Optional[HttpMethod]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vocode_api-0.0.5a5/src/vocode/types/voice_type.py` & `vocode_api-0.0.5a6/src/vocode/types/voice_type.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,27 +7,23 @@
 
 
 class VoiceType(str, enum.Enum):
     """
     An enumeration.
     """
 
-    VOICE_BASE = "voice_base"
     VOICE_AZURE = "voice_azure"
     VOICE_RIME = "voice_rime"
     VOICE_ELEVEN_LABS = "voice_eleven_labs"
 
     def visit(
         self,
-        voice_base: typing.Callable[[], T_Result],
         voice_azure: typing.Callable[[], T_Result],
         voice_rime: typing.Callable[[], T_Result],
         voice_eleven_labs: typing.Callable[[], T_Result],
     ) -> T_Result:
-        if self is VoiceType.VOICE_BASE:
-            return voice_base()
         if self is VoiceType.VOICE_AZURE:
             return voice_azure()
         if self is VoiceType.VOICE_RIME:
             return voice_rime()
         if self is VoiceType.VOICE_ELEVEN_LABS:
             return voice_eleven_labs()
```

### Comparing `vocode_api-0.0.5a5/src/vocode/types/webhook_params.py` & `vocode_api-0.0.5a6/src/vocode/types/webhook_update_params.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .event_type import EventType
-from .http_method import HttpMethod
+from .webhook_update_params_method import WebhookUpdateParamsMethod
+from .webhook_update_params_subscriptions import WebhookUpdateParamsSubscriptions
+from .webhook_update_params_url import WebhookUpdateParamsUrl
 
 
-class WebhookParams(pydantic.BaseModel):
-    subscriptions: typing.List[EventType]
-    url: str
-    method: typing.Optional[HttpMethod]
+class WebhookUpdateParams(pydantic.BaseModel):
+    subscriptions: typing.Optional[WebhookUpdateParamsSubscriptions]
+    url: typing.Optional[WebhookUpdateParamsUrl]
+    method: typing.Optional[WebhookUpdateParamsMethod]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vocode_api-0.0.5a5/src/vocode/types/webhook_update_params.py` & `vocode_api-0.0.5a6/src/vocode/types/pinecone_vector_database_update_params.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .webhook_update_params_method import WebhookUpdateParamsMethod
-from .webhook_update_params_subscriptions import WebhookUpdateParamsSubscriptions
-from .webhook_update_params_url import WebhookUpdateParamsUrl
+from .pinecone_vector_database_update_params_api_environment import PineconeVectorDatabaseUpdateParamsApiEnvironment
+from .pinecone_vector_database_update_params_api_key import PineconeVectorDatabaseUpdateParamsApiKey
+from .pinecone_vector_database_update_params_index import PineconeVectorDatabaseUpdateParamsIndex
+from .vector_database_type import VectorDatabaseType
 
 
-class WebhookUpdateParams(pydantic.BaseModel):
-    subscriptions: typing.Optional[WebhookUpdateParamsSubscriptions]
-    url: typing.Optional[WebhookUpdateParamsUrl]
-    method: typing.Optional[WebhookUpdateParamsMethod]
+class PineconeVectorDatabaseUpdateParams(pydantic.BaseModel):
+    type: VectorDatabaseType
+    index: typing.Optional[PineconeVectorDatabaseUpdateParamsIndex]
+    api_key: typing.Optional[PineconeVectorDatabaseUpdateParamsApiKey]
+    api_environment: typing.Optional[PineconeVectorDatabaseUpdateParamsApiEnvironment]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vocode_api-0.0.5a5/PKG-INFO` & `vocode_api-0.0.5a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vocode-api
-Version: 0.0.5a5
+Version: 0.0.5a6
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

