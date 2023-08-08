# Comparing `tmp/discord-py-interactions-5.8.0.tar.gz` & `tmp/discord-py-interactions-5.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-py-interactions-5.8.0.tar", last modified: Thu Jul 13 19:03:24 2023, max compression
+gzip compressed data, was "discord-py-interactions-5.9.0.tar", last modified: Tue Aug  8 15:17:55 2023, max compression
```

## Comparing `discord-py-interactions-5.8.0.tar` & `discord-py-interactions-5.9.0.tar`

### file list

```diff
@@ -1,197 +1,198 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.496833 discord-py-interactions-5.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-07-13 19:03:24.496833 discord-py-interactions-5.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.468833 discord-py-interactions-5.8.0/discord_py_interactions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-07-13 19:03:24.000000 discord-py-interactions-5.8.0/discord_py_interactions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-07-13 19:03:24.000000 discord-py-interactions-5.8.0/discord_py_interactions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 19:03:24.000000 discord-py-interactions-5.8.0/discord_py_interactions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-13 19:03:24.000000 discord-py-interactions-5.8.0/discord_py_interactions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-13 19:03:24.000000 discord-py-interactions-5.8.0/discord_py_interactions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.468833 discord-py-interactions-5.8.0/interactions/
--rw-r--r--   0 runner    (1001) docker     (123)    15634 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.468833 discord-py-interactions-5.8.0/interactions/api/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.468833 discord-py-interactions-5.8.0/interactions/api/events/
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23953 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/discord.py
--rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.472833 discord-py-interactions-5.8.0/interactions/api/events/processors/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/processors/_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/processors/_template.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/processors/auto_mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/processors/channel_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/processors/guild_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/processors/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/processors/member_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/processors/message_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/processors/reaction_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/processors/role_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/processors/stage_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/processors/thread_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/processors/user_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/events/processors/voice_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.472833 discord-py-interactions-5.8.0/interactions/api/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13569 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/gateway/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/gateway/state.py
--rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/gateway/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.472833 discord-py-interactions-5.8.0/interactions/api/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/http/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.472833 discord-py-interactions-5.8.0/interactions/api/http/http_requests/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/http/http_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/http/http_requests/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)    22816 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/http/http_requests/channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/http/http_requests/emojis.py
--rw-r--r--   0 runner    (1001) docker     (123)    35309 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/http/http_requests/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/http/http_requests/interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/http/http_requests/members.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/http/http_requests/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/http/http_requests/reactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/http/http_requests/scheduled_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/http/http_requests/stickers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/http/http_requests/threads.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/http/http_requests/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/http/http_requests/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/http/route.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.476833 discord-py-interactions-5.8.0/interactions/api/voice/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/voice/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/voice/audio_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/voice/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/voice/opus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/voice/player.py
--rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/voice/recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15285 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/api/voice/voice_gateway.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.476833 discord-py-interactions-5.8.0/interactions/bin/
--rw-r--r--   0 runner    (1001) docker     (123)   441856 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/bin/opus-x64.dll
--rw-r--r--   0 runner    (1001) docker     (123)   366080 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/bin/opus-x86.dll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.476833 discord-py-interactions-5.8.0/interactions/client/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/auto_shard_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    92213 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    13209 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.476833 discord-py-interactions-5.8.0/interactions/client/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/mixins/modal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/mixins/send.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/mixins/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)    31356 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/smart_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.480833 discord-py-interactions-5.8.0/interactions/client/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/utils/attr_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/utils/attr_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/utils/attr_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/utils/deserialise_app_cmds.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/utils/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/utils/input_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/utils/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/client/utils/text_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.480833 discord-py-interactions-5.8.0/interactions/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/console.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.480833 discord-py-interactions-5.8.0/interactions/ext/debug_extension/
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/debug_extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/debug_extension/debug_application_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/debug_extension/debug_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/debug_extension/debug_exts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/debug_extension/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.480833 discord-py-interactions-5.8.0/interactions/ext/hybrid_commands/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/hybrid_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/hybrid_commands/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    23266 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/hybrid_commands/hybrid_slash.py
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/hybrid_commands/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/jurigged.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.484833 discord-py-interactions-5.8.0/interactions/ext/mypy/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/mypy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16002 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/paginators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.484833 discord-py-interactions-5.8.0/interactions/ext/prefixed_commands/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/prefixed_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27881 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/prefixed_commands/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/prefixed_commands/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/prefixed_commands/help.py
--rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/prefixed_commands/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/prefixed_commands/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/ext/sentry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.484833 discord-py-interactions-5.8.0/interactions/models/
--rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.488834 discord-py-interactions-5.8.0/interactions/models/discord/
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/app_perms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    13612 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/auto_mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   103722 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/color.py
--rw-r--r--   0 runner    (1001) docker     (123)    24769 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    16484 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)    31037 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    96356 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/invite.py
--rw-r--r--   0 runner    (1001) docker     (123)    38408 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/modal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/scheduled_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/stage_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/team.py
--rw-r--r--   0 runner    (1001) docker     (123)     8875 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)    26138 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/user.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/voice_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/discord/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.492833 discord-py-interactions-5.8.0/interactions/models/internal/
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/active_voice_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.492833 discord-py-interactions-5.8.0/interactions/models/internal/annotations/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/annotations/slash.py
--rw-r--r--   0 runner    (1001) docker     (123)    55760 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/application_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/auto_defer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    36628 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    19351 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    17655 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/cooldowns.py
--rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/localisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.492833 discord-py-interactions-5.8.0/interactions/models/internal/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/tasks/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/tasks/triggers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/internal/wait.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.496833 discord-py-interactions-5.8.0/interactions/models/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/misc/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/models/misc/iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/interactions/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-13 19:03:24.496833 discord-py-interactions-5.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-13 19:03:17.000000 discord-py-interactions-5.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:24.496833 discord-py-interactions-5.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/tests/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/tests/test_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/tests/test_contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/tests/test_cooldowns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/tests/test_emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-13 19:03:07.000000 discord-py-interactions-5.8.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:17:55.849075 discord-py-interactions-5.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-08-08 15:17:55.849075 discord-py-interactions-5.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:17:55.797074 discord-py-interactions-5.9.0/discord_py_interactions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-08-08 15:17:55.000000 discord-py-interactions-5.9.0/discord_py_interactions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-08-08 15:17:55.000000 discord-py-interactions-5.9.0/discord_py_interactions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 15:17:55.000000 discord-py-interactions-5.9.0/discord_py_interactions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-08-08 15:17:55.000000 discord-py-interactions-5.9.0/discord_py_interactions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-08 15:17:55.000000 discord-py-interactions-5.9.0/discord_py_interactions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:17:55.801074 discord-py-interactions-5.9.0/interactions/
+-rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:17:55.801074 discord-py-interactions-5.9.0/interactions/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:17:55.801074 discord-py-interactions-5.9.0/interactions/api/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/events/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26535 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/events/discord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/events/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:17:55.805075 discord-py-interactions-5.9.0/interactions/api/events/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/events/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/events/processors/_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/events/processors/_template.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/events/processors/auto_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/events/processors/channel_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/events/processors/guild_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/events/processors/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/events/processors/member_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/events/processors/message_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/events/processors/reaction_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/events/processors/role_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/events/processors/scheduled_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/events/processors/stage_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/events/processors/thread_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/events/processors/user_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/events/processors/voice_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:17:55.805075 discord-py-interactions-5.9.0/interactions/api/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13569 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/gateway/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/gateway/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/gateway/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:17:55.805075 discord-py-interactions-5.9.0/interactions/api/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/http/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:17:55.809074 discord-py-interactions-5.9.0/interactions/api/http/http_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/http/http_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/http/http_requests/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22907 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/http/http_requests/channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/http/http_requests/emojis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35309 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/http/http_requests/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12056 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/http/http_requests/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/http/http_requests/members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/http/http_requests/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/http/http_requests/reactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/http/http_requests/scheduled_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/http/http_requests/stickers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/http/http_requests/threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/http/http_requests/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/http/http_requests/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/http/route.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:17:55.813074 discord-py-interactions-5.9.0/interactions/api/voice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/voice/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/voice/audio_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/voice/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/voice/opus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/voice/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7782 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/voice/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15285 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/api/voice/voice_gateway.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:17:55.813074 discord-py-interactions-5.9.0/interactions/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)   441856 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/bin/opus-x64.dll
+-rw-r--r--   0 runner    (1001) docker     (123)   366080 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/bin/opus-x86.dll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:17:55.817074 discord-py-interactions-5.9.0/interactions/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/client/auto_shard_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93178 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/client/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13239 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/client/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:17:55.817074 discord-py-interactions-5.9.0/interactions/client/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/client/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/client/mixins/modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/client/mixins/send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/client/mixins/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32858 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/client/smart_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:17:55.817074 discord-py-interactions-5.9.0/interactions/client/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/client/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/client/utils/attr_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/client/utils/attr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/client/utils/attr_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/client/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/client/utils/deserialise_app_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/client/utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/client/utils/input_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/client/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/client/utils/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/client/utils/text_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:17:55.821075 discord-py-interactions-5.9.0/interactions/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/ext/console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:17:55.821075 discord-py-interactions-5.9.0/interactions/ext/debug_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/ext/debug_extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/ext/debug_extension/debug_application_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/ext/debug_extension/debug_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/ext/debug_extension/debug_exts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/ext/debug_extension/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:17:55.821075 discord-py-interactions-5.9.0/interactions/ext/hybrid_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/ext/hybrid_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13057 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/ext/hybrid_commands/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24128 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/ext/hybrid_commands/hybrid_slash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/ext/hybrid_commands/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/ext/jurigged.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:17:55.821075 discord-py-interactions-5.9.0/interactions/ext/mypy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/ext/mypy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16002 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/ext/paginators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:17:55.825075 discord-py-interactions-5.9.0/interactions/ext/prefixed_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/ext/prefixed_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29438 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/ext/prefixed_commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/ext/prefixed_commands/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/ext/prefixed_commands/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/ext/prefixed_commands/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/ext/prefixed_commands/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/ext/sentry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:17:55.825075 discord-py-interactions-5.9.0/interactions/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    12637 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:17:55.833075 discord-py-interactions-5.9.0/interactions/models/discord/
+-rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/discord/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/discord/app_perms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/discord/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/discord/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13612 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/discord/auto_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/discord/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104644 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/discord/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/discord/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24776 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/discord/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16484 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/discord/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/discord/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31332 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/discord/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/discord/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96566 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/discord/guild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/discord/invite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38476 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/discord/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/discord/modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/discord/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/discord/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/discord/scheduled_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/discord/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/discord/stage_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/discord/sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/discord/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8875 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/discord/thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/discord/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26138 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/discord/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/discord/user.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/discord/voice_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/discord/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:17:55.837075 discord-py-interactions-5.9.0/interactions/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/internal/active_voice_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:17:55.841075 discord-py-interactions-5.9.0/interactions/models/internal/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/internal/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/internal/annotations/slash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57623 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/internal/application_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/internal/auto_defer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/internal/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/internal/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/internal/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36926 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/internal/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19643 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/internal/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17655 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/internal/cooldowns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/internal/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/internal/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/internal/localisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/internal/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:17:55.841075 discord-py-interactions-5.9.0/interactions/models/internal/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/internal/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/internal/tasks/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/internal/tasks/triggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/internal/wait.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:17:55.845075 discord-py-interactions-5.9.0/interactions/models/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/misc/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/models/misc/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/interactions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-08 15:17:55.849075 discord-py-interactions-5.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-08-08 15:17:47.000000 discord-py-interactions-5.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:17:55.849075 discord-py-interactions-5.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/tests/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16999 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/tests/test_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/tests/test_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/tests/test_cooldowns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/tests/test_emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-08-08 15:17:30.000000 discord-py-interactions-5.9.0/tests/utils.py
```

### Comparing `discord-py-interactions-5.8.0/LICENSE` & `discord-py-interactions-5.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/PKG-INFO` & `discord-py-interactions-5.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-py-interactions
-Version: 5.8.0
+Version: 5.9.0
 Summary: Easy, simple, scalable and modular: a Python API wrapper for interactions.
 Home-page: https://github.com/interactions-py/interactions.py
 Author: LordOfPolls
 Author-email: dev@lordofpolls.com
 Project-URL: Discord, https://discord.gg/KkgMBVuEkx
 Project-URL: Documentation, https://naff-docs.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `discord-py-interactions-5.8.0/README.md` & `discord-py-interactions-5.9.0/README.md`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/discord_py_interactions.egg-info/PKG-INFO` & `discord-py-interactions-5.9.0/discord_py_interactions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-py-interactions
-Version: 5.8.0
+Version: 5.9.0
 Summary: Easy, simple, scalable and modular: a Python API wrapper for interactions.
 Home-page: https://github.com/interactions-py/interactions.py
 Author: LordOfPolls
 Author-email: dev@lordofpolls.com
 Project-URL: Discord, https://discord.gg/KkgMBVuEkx
 Project-URL: Documentation, https://naff-docs.readthedocs.io/en/latest/
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `discord-py-interactions-5.8.0/discord_py_interactions.egg-info/SOURCES.txt` & `discord-py-interactions-5.9.0/discord_py_interactions.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 interactions/api/events/processors/channel_events.py
 interactions/api/events/processors/guild_events.py
 interactions/api/events/processors/integrations.py
 interactions/api/events/processors/member_events.py
 interactions/api/events/processors/message_events.py
 interactions/api/events/processors/reaction_events.py
 interactions/api/events/processors/role_events.py
+interactions/api/events/processors/scheduled_events.py
 interactions/api/events/processors/stage_events.py
 interactions/api/events/processors/thread_events.py
 interactions/api/events/processors/user_events.py
 interactions/api/events/processors/voice_events.py
 interactions/api/gateway/__init__.py
 interactions/api/gateway/gateway.py
 interactions/api/gateway/state.py
```

### Comparing `discord-py-interactions-5.8.0/discord_py_interactions.egg-info/requires.txt` & `discord-py-interactions-5.9.0/discord_py_interactions.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/__init__.py` & `discord-py-interactions-5.9.0/interactions/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,15 @@
     COLOR_TYPES,
     Colour,
     CommandType,
     component_callback,
     ComponentCommand,
     ComponentContext,
     ComponentType,
+    ConsumeRest,
     context_menu,
     ContextMenu,
     ContextMenuContext,
     Converter,
     cooldown,
     Cooldown,
     CooldownSystem,
@@ -334,14 +335,15 @@
     WebhookMixin,
     WebhookTypes,
     WebSocketOPCode,
     SlidingWindowSystem,
     ExponentialBackoffSystem,
     LeakyBucketSystem,
     TokenBucketSystem,
+    ForumSortOrder,
 )
 from .api import events
 from . import ext
 
 __all__ = (
     "__api_version__",
     "__py_version__",
@@ -409,14 +411,15 @@
     "COLOR_TYPES",
     "Colour",
     "CommandType",
     "component_callback",
     "ComponentCommand",
     "ComponentContext",
     "ComponentType",
+    "ConsumeRest",
     "const",
     "context_menu",
     "CONTEXT_MENU_NAME_LENGTH",
     "ContextMenu",
     "ContextMenuContext",
     "Converter",
     "cooldown",
@@ -454,14 +457,15 @@
     "events",
     "ExplicitContentFilterLevel",
     "ext",
     "Extension",
     "File",
     "FlatUIColors",
     "FlatUIColours",
+    "ForumSortOrder",
     "ForumLayoutType",
     "get_components_ids",
     "get_logger",
     "global_autocomplete",
     "GLOBAL_SCOPE",
     "GlobalAutoComplete",
     "GlobalScope",
```

### Comparing `discord-py-interactions-5.8.0/interactions/api/events/__init__.py` & `discord-py-interactions-5.9.0/interactions/api/events/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,19 @@
     ChannelUpdate,
     GuildAuditLogEntryCreate,
     GuildAvailable,
     GuildEmojisUpdate,
     GuildJoin,
     GuildLeft,
     GuildMembersChunk,
+    GuildScheduledEventCreate,
+    GuildScheduledEventUpdate,
+    GuildScheduledEventDelete,
+    GuildScheduledEventUserAdd,
+    GuildScheduledEventUserRemove,
     GuildStickersUpdate,
     GuildUnavailable,
     GuildUpdate,
     IntegrationCreate,
     IntegrationDelete,
     IntegrationUpdate,
     InteractionCreate,
@@ -122,14 +127,19 @@
     "GuildAuditLogEntryCreate",
     "GuildAvailable",
     "GuildEmojisUpdate",
     "GuildEvent",
     "GuildJoin",
     "GuildLeft",
     "GuildMembersChunk",
+    "GuildScheduledEventCreate",
+    "GuildScheduledEventUpdate",
+    "GuildScheduledEventDelete",
+    "GuildScheduledEventUserAdd",
+    "GuildScheduledEventUserRemove",
     "GuildStickersUpdate",
     "GuildUnavailable",
     "GuildUpdate",
     "IntegrationCreate",
     "IntegrationDelete",
     "IntegrationUpdate",
     "InteractionCreate",
```

### Comparing `discord-py-interactions-5.8.0/interactions/api/events/base.py` & `discord-py-interactions-5.9.0/interactions/api/events/base.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/api/events/discord.py` & `discord-py-interactions-5.9.0/interactions/api/events/discord.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,19 @@
     "ChannelPinsUpdate",
     "ChannelUpdate",
     "GuildAuditLogEntryCreate",
     "GuildEmojisUpdate",
     "GuildJoin",
     "GuildLeft",
     "GuildMembersChunk",
+    "GuildScheduledEventCreate",
+    "GuildScheduledEventUpdate",
+    "GuildScheduledEventDelete",
+    "GuildScheduledEventUserAdd",
+    "GuildScheduledEventUserRemove",
     "GuildStickersUpdate",
     "GuildAvailable",
     "GuildUnavailable",
     "GuildUpdate",
     "IntegrationCreate",
     "IntegrationDelete",
     "IntegrationUpdate",
@@ -105,14 +110,15 @@
     from interactions.models.discord.role import Role
     from interactions.models.discord.sticker import Sticker
     from interactions.models.discord.voice_state import VoiceState
     from interactions.models.discord.stage_instance import StageInstance
     from interactions.models.discord.auto_mod import AutoModerationAction, AutoModRule
     from interactions.models.discord.reaction import Reaction
     from interactions.models.discord.app_perms import ApplicationCommandPermission
+    from interactions.models.discord.scheduled_event import ScheduledEvent
 
 
 @attrs.define(eq=False, order=False, hash=False, kw_only=False)
 class AutoModExec(BaseEvent):
     """Dispatched when an auto modation action is executed"""
 
     execution: "AutoModerationAction" = attrs.field(repr=False, metadata=docs("The executed auto mod action"))
@@ -138,14 +144,15 @@
     """Dispatched when an auto mod rule is deleted"""
 
     ...
 
 
 @attrs.define(eq=False, order=False, hash=False, kw_only=False)
 class ApplicationCommandPermissionsUpdate(BaseEvent):
+    id: "Snowflake_Type" = attrs.field(repr=False, metadata=docs("The ID of the command permissions were updated for"))
     guild_id: "Snowflake_Type" = attrs.field(
         repr=False, metadata=docs("The guild the command permissions were updated in")
     )
     application_id: "Snowflake_Type" = attrs.field(
         repr=False, metadata=docs("The application the command permissions were updated for")
     )
     permissions: List["ApplicationCommandPermission"] = attrs.field(
@@ -244,28 +251,33 @@
     member: "Member" = attrs.field(
         repr=False,
     )
     """The member who was added"""
 
 
 @attrs.define(eq=False, order=False, hash=False, kw_only=False)
-class ThreadMembersUpdate(BaseEvent):
+class ThreadMembersUpdate(GuildEvent):
     """Dispatched when anyone is added or removed from a thread."""
 
     id: "Snowflake_Type" = attrs.field(
         repr=False,
     )
     """The ID of the thread"""
     member_count: int = attrs.field(repr=False, default=50)
     """the approximate number of members in the thread, capped at 50"""
     added_members: List["Member"] = attrs.field(repr=False, factory=list)
     """Users added to the thread"""
     removed_member_ids: List["Snowflake_Type"] = attrs.field(repr=False, factory=list)
     """Users removed from the thread"""
 
+    @property
+    def channel(self) -> Optional["TYPE_THREAD_CHANNEL"]:
+        """The thread channel this event is dispatched from"""
+        return self.client.get_channel(self.id)
+
 
 @attrs.define(eq=False, order=False, hash=False, kw_only=False)
 class GuildJoin(GuildEvent):
     """
     Dispatched when a guild is joined, created, or becomes available.
 
     !!! note
@@ -746,7 +758,60 @@
 
 @attrs.define(eq=False, order=False, hash=False, kw_only=False)
 class GuildAuditLogEntryCreate(GuildEvent):
     """Dispatched when audit log entry is created"""
 
     audit_log_entry: interactions.models.AuditLogEntry = attrs.field(repr=False)
     """The audit log entry object"""
+
+
+@attrs.define(eq=False, order=False, hash=False, kw_only=False)
+class GuildScheduledEventCreate(BaseEvent):
+    """Dispatched when scheduled event is created"""
+
+    scheduled_event: "ScheduledEvent" = attrs.field(repr=True)
+    """The scheduled event object"""
+
+
+@attrs.define(eq=False, order=False, hash=False, kw_only=False)
+class GuildScheduledEventUpdate(BaseEvent):
+    """Dispatched when scheduled event is updated"""
+
+    before: Absent["ScheduledEvent"] = attrs.field(repr=True)
+    """The scheduled event before this event was created"""
+    after: "ScheduledEvent" = attrs.field(repr=True)
+    """The scheduled event after this event was created"""
+
+
+@attrs.define(eq=False, order=False, hash=False, kw_only=False)
+class GuildScheduledEventDelete(GuildScheduledEventCreate):
+    """Dispatched when scheduled event is deleted"""
+
+
+@attrs.define(eq=False, order=False, hash=False, kw_only=False)
+class GuildScheduledEventUserAdd(GuildEvent):
+    """Dispatched when scheduled event is created"""
+
+    scheduled_event_id: "Snowflake_Type" = attrs.field(repr=True)
+    """The ID of the scheduled event"""
+    user_id: "Snowflake_Type" = attrs.field(repr=True)
+    """The ID of the user that has been added/removed from scheduled event"""
+
+    @property
+    def scheduled_event(self) -> Optional["ScheduledEvent"]:
+        """The scheduled event object if cached"""
+        return self.client.get_scheduled_event(self.scheduled_event_id)
+
+    @property
+    def user(self) -> Optional["User"]:
+        """The user that has been added/removed from scheduled event if cached"""
+        return self.client.get_user(self.user_id)
+
+    @property
+    def member(self) -> Optional["Member"]:
+        """The guild member that has been added/removed from scheduled event if cached"""
+        return self.client.get_member(self.guild_id, self.user.id)
+
+
+@attrs.define(eq=False, order=False, hash=False, kw_only=False)
+class GuildScheduledEventUserRemove(GuildScheduledEventUserAdd):
+    """Dispatched when scheduled event is removed"""
```

### Comparing `discord-py-interactions-5.8.0/interactions/api/events/internal.py` & `discord-py-interactions-5.9.0/interactions/api/events/internal.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/api/events/processors/__init__.py` & `discord-py-interactions-5.9.0/interactions/api/events/processors/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from .channel_events import ChannelEvents
 from .guild_events import GuildEvents
 from .integrations import IntegrationEvents
 from .member_events import MemberEvents
 from .message_events import MessageEvents
 from .reaction_events import ReactionEvents
 from .role_events import RoleEvents
+from .scheduled_events import ScheduledEvents
 from .stage_events import StageEvents
 from .thread_events import ThreadEvents
 from .user_events import UserEvents
 from .voice_events import VoiceEvents
 from ._template import Processor
 from .auto_mod import AutoModEvents
 
@@ -16,14 +17,15 @@
     "ChannelEvents",
     "GuildEvents",
     "IntegrationEvents",
     "MemberEvents",
     "MessageEvents",
     "ReactionEvents",
     "RoleEvents",
+    "ScheduledEvents",
     "StageEvents",
     "ThreadEvents",
     "UserEvents",
     "VoiceEvents",
     "Processor",
     "AutoModEvents",
 )
```

### Comparing `discord-py-interactions-5.8.0/interactions/api/events/processors/_template.py` & `discord-py-interactions-5.9.0/interactions/api/events/processors/_template.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/api/events/processors/auto_mod.py` & `discord-py-interactions-5.9.0/interactions/api/events/processors/auto_mod.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/api/events/processors/channel_events.py` & `discord-py-interactions-5.9.0/interactions/api/events/processors/channel_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/api/events/processors/guild_events.py` & `discord-py-interactions-5.9.0/interactions/api/events/processors/guild_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/api/events/processors/integrations.py` & `discord-py-interactions-5.9.0/interactions/api/events/processors/integrations.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/api/events/processors/member_events.py` & `discord-py-interactions-5.9.0/interactions/api/events/processors/member_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/api/events/processors/message_events.py` & `discord-py-interactions-5.9.0/interactions/api/events/processors/message_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/api/events/processors/reaction_events.py` & `discord-py-interactions-5.9.0/interactions/api/events/processors/reaction_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/api/events/processors/role_events.py` & `discord-py-interactions-5.9.0/interactions/api/events/processors/role_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/api/events/processors/stage_events.py` & `discord-py-interactions-5.9.0/interactions/api/events/processors/stage_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/api/events/processors/thread_events.py` & `discord-py-interactions-5.9.0/interactions/api/events/processors/thread_events.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,13 +39,14 @@
         self.dispatch(events.ThreadListSync(channel_ids, threads, members))
 
     @Processor.define()
     async def _on_raw_thread_members_update(self, event: "RawGatewayEvent") -> None:
         g_id = event.data.get("guild_id")
         self.dispatch(
             events.ThreadMembersUpdate(
+                g_id,
                 event.data.get("id"),
                 event.data.get("member_count"),
                 [await self.cache.fetch_member(g_id, m["user_id"]) for m in event.data.get("added_members", [])],
                 event.data.get("removed_member_ids", []),
             )
         )
```

### Comparing `discord-py-interactions-5.8.0/interactions/api/events/processors/user_events.py` & `discord-py-interactions-5.9.0/interactions/api/events/processors/user_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/api/events/processors/voice_events.py` & `discord-py-interactions-5.9.0/interactions/api/events/processors/voice_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/api/gateway/gateway.py` & `discord-py-interactions-5.9.0/interactions/api/gateway/gateway.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/api/gateway/state.py` & `discord-py-interactions-5.9.0/interactions/api/gateway/state.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/api/gateway/websocket.py` & `discord-py-interactions-5.9.0/interactions/api/gateway/websocket.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/api/http/http_client.py` & `discord-py-interactions-5.9.0/interactions/api/http/http_client.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/api/http/http_requests/__init__.py` & `discord-py-interactions-5.9.0/interactions/api/http/http_requests/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/api/http/http_requests/bot.py` & `discord-py-interactions-5.9.0/interactions/api/http/http_requests/bot.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/api/http/http_requests/channels.py` & `discord-py-interactions-5.9.0/interactions/api/http/http_requests/channels.py`

 * *Files 0% similar despite different names*

```diff
@@ -440,15 +440,20 @@
         Args:
             channel_id: The ID of the channel.
             overwrite_id: The ID of the overwrite
             reason: An optional reason for the audit log
 
         """
         await self.request(
-            Route("DELETE", "/channels/{channel_id}/{overwrite_id}", channel_id=channel_id, overwrite_id=overwrite_id),
+            Route(
+                "DELETE",
+                "/channels/{channel_id}/permissions/{overwrite_id}",
+                channel_id=channel_id,
+                overwrite_id=overwrite_id,
+            ),
             reason=reason,
         )
 
     async def follow_news_channel(
         self, channel_id: "Snowflake_Type", webhook_channel_id: "Snowflake_Type"
     ) -> discord_typings.FollowedChannelData:
         """
```

### Comparing `discord-py-interactions-5.8.0/interactions/api/http/http_requests/emojis.py` & `discord-py-interactions-5.9.0/interactions/api/http/http_requests/emojis.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/api/http/http_requests/guild.py` & `discord-py-interactions-5.9.0/interactions/api/http/http_requests/guild.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/api/http/http_requests/interactions.py` & `discord-py-interactions-5.9.0/interactions/api/http/http_requests/interactions.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/api/http/http_requests/members.py` & `discord-py-interactions-5.9.0/interactions/api/http/http_requests/members.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/api/http/http_requests/messages.py` & `discord-py-interactions-5.9.0/interactions/api/http/http_requests/messages.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/api/http/http_requests/reactions.py` & `discord-py-interactions-5.9.0/interactions/api/http/http_requests/reactions.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/api/http/http_requests/scheduled_events.py` & `discord-py-interactions-5.9.0/interactions/api/http/http_requests/scheduled_events.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/api/http/http_requests/stickers.py` & `discord-py-interactions-5.9.0/interactions/api/http/http_requests/stickers.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/api/http/http_requests/threads.py` & `discord-py-interactions-5.9.0/interactions/api/http/http_requests/threads.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
         """
         return await self.request(Route("GET", "/channels/{thread_id}/thread-members", thread_id=thread_id))
 
     async def list_public_archived_threads(
         self,
         channel_id: "Snowflake_Type",
-        limit: int = None,
+        limit: int | None = None,
         before: Optional["Snowflake_Type"] = None,
     ) -> discord_typings.ListThreadsData:
         """
         Get a list of archived public threads in a channel.
 
         Args:
             channel_id: The channel to get threads from
@@ -104,15 +104,15 @@
         return await self.request(
             Route("GET", "/channels/{channel_id}/threads/archived/public", channel_id=channel_id), params=payload
         )
 
     async def list_private_archived_threads(
         self,
         channel_id: "Snowflake_Type",
-        limit: int = None,
+        limit: int | None = None,
         before: Optional["Snowflake_Type"] = None,
     ) -> discord_typings.ListThreadsData:
         """
         Get a list of archived private threads in a channel.
 
         Args:
             channel_id: The channel to get threads from
@@ -131,15 +131,15 @@
         return await self.request(
             Route("GET", "/channels/{channel_id}/threads/archived/private", channel_id=channel_id), params=payload
         )
 
     async def list_joined_private_archived_threads(
         self,
         channel_id: "Snowflake_Type",
-        limit: int = None,
+        limit: int | None = None,
         before: Optional["Snowflake_Type"] = None,
     ) -> discord_typings.ListThreadsData:
         """
         Get a list of archived private threads in a channel that you have joined.
 
         Args:
             channel_id: The channel to get threads from
@@ -225,15 +225,15 @@
 
     async def create_forum_thread(
         self,
         channel_id: "Snowflake_Type",
         name: str,
         auto_archive_duration: int,
         message: dict | FormData,
-        applied_tags: List[str] = None,
+        applied_tags: List[str] | None = None,
         rate_limit_per_user: Absent[int] = MISSING,
         files: Absent["UPLOADABLE_TYPE"] = MISSING,
         reason: Absent[str] = MISSING,
     ) -> dict:
         """
         Create a thread within a forum channel.
```

### Comparing `discord-py-interactions-5.8.0/interactions/api/http/http_requests/users.py` & `discord-py-interactions-5.9.0/interactions/api/http/http_requests/users.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         return await self.request(Route("GET", "/users/@me/connections"))
 
     async def group_dm_add_recipient(
         self,
         channel_id: "Snowflake_Type",
         user_id: "Snowflake_Type",
         access_token: str,
-        nick: str = None,
+        nick: str | None = None,
     ) -> None:
         """
         Adds a recipient to a Group DM using their access token.
 
         Args:
             channel_id: The ID of the group dm
             user_id: The ID of the user to add
@@ -126,15 +126,15 @@
             user_id: The ID of the user to remove
 
         """
         return await self.request(
             Route("DELETE", "/channels/{channel_id}/recipients/{user_id}", channel_id=channel_id, user_id=user_id)
         )
 
-    async def modify_current_user_nick(self, guild_id: "Snowflake_Type", nickname: str = None) -> None:
+    async def modify_current_user_nick(self, guild_id: "Snowflake_Type", nickname: str | None = None) -> None:
         """
         Modifies the nickname of the current user in a guild.
 
         Args:
             guild_id: The ID of the guild
             nickname: The new nickname to use
```

### Comparing `discord-py-interactions-5.8.0/interactions/api/http/http_requests/webhooks.py` & `discord-py-interactions-5.9.0/interactions/api/http/http_requests/webhooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,17 @@
 
         Returns:
             List of webhook objects
 
         """
         return await self.request(Route("GET", "/guilds/{guild_id}/webhooks", guild_id=guild_id))
 
-    async def get_webhook(self, webhook_id: "Snowflake_Type", webhook_token: str = None) -> discord_typings.WebhookData:
+    async def get_webhook(
+        self, webhook_id: "Snowflake_Type", webhook_token: str | None = None
+    ) -> discord_typings.WebhookData:
         """
         Return the new webhook object for the given id.
 
         Args:
             webhook_id: The ID of the webhook to get
             webhook_token: The token for the webhook
 
@@ -77,15 +79,15 @@
 
     async def modify_webhook(
         self,
         webhook_id: "Snowflake_Type",
         name: str,
         avatar: Any,
         channel_id: "Snowflake_Type",
-        webhook_token: str = None,
+        webhook_token: str | None = None,
     ) -> discord_typings.WebhookData:
         """
         Modify a webhook.
 
         Args:
             name: the default name of the webhook
             avatar: image for the default webhook avatar
@@ -97,15 +99,15 @@
         endpoint = "/webhooks/{webhook_id}" + f"/{webhook_token}" if webhook_token else ""
 
         return await self.request(
             Route("PATCH", endpoint, webhook_id=webhook_id, webhook_token=webhook_token),
             payload={"name": name, "avatar": avatar, "channel_id": channel_id},
         )
 
-    async def delete_webhook(self, webhook_id: "Snowflake_Type", webhook_token: str = None) -> None:
+    async def delete_webhook(self, webhook_id: "Snowflake_Type", webhook_token: str | None = None) -> None:
         """
         Delete a webhook.
 
         Args:
             webhook_id: The ID of the webhook to delete
             webhook_token: The token for the webhook
```

### Comparing `discord-py-interactions-5.8.0/interactions/api/http/route.py` & `discord-py-interactions-5.9.0/interactions/api/http/route.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/api/voice/audio.py` & `discord-py-interactions-5.9.0/interactions/api/voice/audio.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/api/voice/audio_writer.py` & `discord-py-interactions-5.9.0/interactions/api/voice/audio_writer.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/api/voice/encryption.py` & `discord-py-interactions-5.9.0/interactions/api/voice/encryption.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/api/voice/opus.py` & `discord-py-interactions-5.9.0/interactions/api/voice/opus.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/api/voice/player.py` & `discord-py-interactions-5.9.0/interactions/api/voice/player.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/api/voice/recorder.py` & `discord-py-interactions-5.9.0/interactions/api/voice/recorder.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 __all__ = ("Recorder",)
 
 log = logging.getLogger(logger_name)
 
 
 class Recorder(threading.Thread):
-    def __init__(self, v_state, loop, *, output_dir: str = None) -> None:
+    def __init__(self, v_state, loop, *, output_dir: str | None = None) -> None:
         super().__init__()
         self.daemon = True
 
         self.state: "ActiveVoiceState" = v_state
         self.loop: AbstractEventLoop = loop
         self.decrypter: Decryption = Decryption(self.state.ws.secret)
         self._decoders: dict[str, Decoder] = defaultdict(Decoder)
```

### Comparing `discord-py-interactions-5.8.0/interactions/api/voice/voice_gateway.py` & `discord-py-interactions-5.9.0/interactions/api/voice/voice_gateway.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/bin/opus-x64.dll` & `discord-py-interactions-5.9.0/interactions/bin/opus-x64.dll`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/bin/opus-x86.dll` & `discord-py-interactions-5.9.0/interactions/bin/opus-x86.dll`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/client/__init__.py` & `discord-py-interactions-5.9.0/interactions/client/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/client/auto_shard_client.py` & `discord-py-interactions-5.9.0/interactions/client/auto_shard_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import time
+from datetime import datetime
 from collections import defaultdict
 from typing import TYPE_CHECKING, Optional
 
 import interactions.api.events as events
 from interactions.api.events import ShardConnect
 from interactions.api.gateway.state import ConnectionState
 from interactions.client.client import Client
@@ -64,14 +65,24 @@
         Return a dictionary of latencies for all shards.
 
         Returns:
             {shard_id: latency}
         """
         return {state.shard_id: state.latency for state in self._connection_states}
 
+    @property
+    def start_time(self) -> datetime:
+        """The start time of the first shard of the bot."""
+        return next((state.start_time for state in self._connection_states), MISSING)  # type: ignore
+
+    @property
+    def start_times(self) -> dict[int, datetime]:
+        """The start times of all shards of the bot, keyed by each shard ID."""
+        return {state.shard_id: state.start_time for state in self._connection_states}  # type: ignore
+
     async def stop(self) -> None:
         """Shutdown the bot."""
         self.logger.debug("Stopping the bot.")
         self._ready.clear()
         await self.http.close()
         await asyncio.gather(*(state.stop() for state in self._connection_states))
```

### Comparing `discord-py-interactions-5.8.0/interactions/client/client.py` & `discord-py-interactions-5.9.0/interactions/client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,14 +169,20 @@
     events.MessageDeleteBulk: [Intents.GUILD_MESSAGES],
     # Intents.AUTO_MODERATION_CONFIGURATION
     events.AutoModExec: [Intents.AUTO_MODERATION_EXECUTION, Intents.AUTO_MOD],
     # Intents.AUTO_MODERATION_CONFIGURATION
     events.AutoModCreated: [Intents.AUTO_MODERATION_CONFIGURATION, Intents.AUTO_MOD],
     events.AutoModUpdated: [Intents.AUTO_MODERATION_CONFIGURATION, Intents.AUTO_MOD],
     events.AutoModDeleted: [Intents.AUTO_MODERATION_CONFIGURATION, Intents.AUTO_MOD],
+    # Intents.GUILD_SCHEDULED_EVENTS
+    events.GuildScheduledEventCreate: [Intents.GUILD_SCHEDULED_EVENTS],
+    events.GuildScheduledEventUpdate: [Intents.GUILD_SCHEDULED_EVENTS],
+    events.GuildScheduledEventDelete: [Intents.GUILD_SCHEDULED_EVENTS],
+    events.GuildScheduledEventUserAdd: [Intents.GUILD_SCHEDULED_EVENTS],
+    events.GuildScheduledEventUserRemove: [Intents.GUILD_SCHEDULED_EVENTS],
     # multiple intents
     events.ThreadMembersUpdate: [Intents.GUILDS, Intents.GUILD_MEMBERS],
     events.TypingStart: [
         Intents.GUILD_MESSAGE_TYPING,
         Intents.DIRECT_MESSAGE_TYPING,
         Intents.TYPING,
     ],
@@ -207,14 +213,15 @@
     processors.ChannelEvents,
     processors.GuildEvents,
     processors.IntegrationEvents,
     processors.MemberEvents,
     processors.MessageEvents,
     processors.ReactionEvents,
     processors.RoleEvents,
+    processors.ScheduledEvents,
     processors.StageEvents,
     processors.ThreadEvents,
     processors.UserEvents,
     processors.VoiceEvents,
 ):
     """
 
@@ -1107,15 +1114,15 @@
             Union[
                 List[List[Union["BaseComponent", dict]]],
                 List[Union["BaseComponent", dict]],
                 "BaseComponent",
                 dict,
             ]
         ] = None,
-        check: Absent[Optional[Union[Callable[..., bool], Callable[..., Awaitable[bool]]]]] = None,
+        check: Absent[Optional[Union[Callable[..., bool], Callable[..., Awaitable[bool]]]]] | None = None,
         timeout: Optional[float] = None,
     ) -> "events.Component":
         """
         Waits for a component to be sent to the bot.
 
         Args:
             messages: The message object to check for.
@@ -2278,18 +2285,37 @@
 
         Returns:
             The scheduled event if found, otherwise None
 
         """
         try:
             scheduled_event_data = await self.http.get_scheduled_event(guild_id, scheduled_event_id, with_user_count)
-            return ScheduledEvent.from_dict(scheduled_event_data, self)
+            return self.cache.place_scheduled_event_data(scheduled_event_data)
         except NotFound:
             return None
 
+    def get_scheduled_event(
+        self,
+        scheduled_event_id: "Snowflake_Type",
+    ) -> Optional["ScheduledEvent"]:
+        """
+        Get a scheduled event by id.
+
+        !!! note
+            This method is an alias for the cache which will return a cached object.
+
+        Args:
+            scheduled_event_id: The ID of the scheduled event to get
+
+        Returns:
+            The scheduled event if found, otherwise None
+
+        """
+        return self.cache.get_scheduled_event(scheduled_event_id)
+
     async def fetch_custom_emoji(
         self, emoji_id: "Snowflake_Type", guild_id: "Snowflake_Type", *, force: bool = False
     ) -> Optional[CustomEmoji]:
         """
         Fetch a custom emoji by id.
 
         Args:
```

### Comparing `discord-py-interactions-5.8.0/interactions/client/const.py` & `discord-py-interactions-5.9.0/interactions/client/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 """
 import inspect
 import logging
 import os
 import sys
 from collections import defaultdict
 from importlib.metadata import version as _v, PackageNotFoundError
-from typing import TypeVar, Union, Callable, Coroutine
+from typing import TypeVar, Union, Callable, Coroutine, ClassVar
 
 __all__ = (
     "__version__",
     "__repo_url__",
     "__py_version__",
     "__api_version__",
     "get_logger",
@@ -127,15 +127,15 @@
 EMBED_MAX_DESC_LENGTH = 4096
 EMBED_MAX_FIELDS = 25
 EMBED_TOTAL_MAX = 6000
 EMBED_FIELD_VALUE_LENGTH = 1024
 
 
 class Singleton(type):
-    _instances = {}
+    _instances: ClassVar[dict] = {}
 
     def __call__(self, *args, **kwargs) -> "Singleton":
         if self not in self._instances:
             self._instances[self] = super(Singleton, self).__call__(*args, **kwargs)
         return self._instances[self]
```

### Comparing `discord-py-interactions-5.8.0/interactions/client/errors.py` & `discord-py-interactions-5.9.0/interactions/client/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Any, TYPE_CHECKING, Callable, Coroutine, List, Optional, SupportsInt, Union
+from typing import Dict, Any, TYPE_CHECKING, Callable, Coroutine, ClassVar, List, Optional, SupportsInt, Union
 
 import aiohttp
 
 from interactions.client.utils.misc_utils import escape_mentions
 from . import const
 
 if TYPE_CHECKING:
@@ -197,15 +197,15 @@
     """You have changed something too frequently."""
 
 
 class WebSocketClosed(LibraryException):
     """The websocket was closed."""
 
     code: int = 0
-    codes: Dict[int, str] = {
+    codes: ClassVar[Dict[int, str]] = {
         1000: "Normal Closure",
         4000: "Unknown Error",
         4001: "Unknown OpCode",
         4002: "Decode Error",
         4003: "Not Authenticated",
         4004: "Authentication Failed",
         4005: "Already Authenticated",
@@ -224,15 +224,15 @@
         super().__init__(f"The Websocket closed with code: {code} - {self.codes.get(code, 'Unknown Error')}")
 
 
 class VoiceWebSocketClosed(LibraryException):
     """The voice websocket was closed."""
 
     code: int = 0
-    codes: Dict[int, str] = {
+    codes: ClassVar[Dict[int, str]] = {
         1000: "Normal Closure",
         4000: "Unknown Error",
         4001: "Unknown OpCode",
         4002: "Decode Error",
         4003: "Not Authenticated",
         4004: "Authentication Failed",
         4005: "Already Authenticated",
```

### Comparing `discord-py-interactions-5.8.0/interactions/client/mixins/modal.py` & `discord-py-interactions-5.9.0/interactions/client/mixins/modal.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/client/mixins/send.py` & `discord-py-interactions-5.9.0/interactions/client/mixins/send.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/client/mixins/serialization.py` & `discord-py-interactions-5.9.0/interactions/client/mixins/serialization.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/client/smart_cache.py` & `discord-py-interactions-5.9.0/interactions/client/smart_cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from interactions.models.discord.channel import BaseChannel, GuildChannel, ThreadChannel
 from interactions.models.discord.emoji import CustomEmoji
 from interactions.models.discord.guild import Guild
 from interactions.models.discord.message import Message
 from interactions.models.discord.role import Role
 from interactions.models.discord.snowflake import to_snowflake, to_optional_snowflake
 from interactions.models.discord.user import Member, User
+from interactions.models.discord.scheduled_event import ScheduledEvent
 from interactions.models.internal.active_voice_state import ActiveVoiceState
 
 __all__ = ("GlobalCache", "create_cache")
 
 
 if TYPE_CHECKING:
     from interactions.client import Client
@@ -66,14 +67,15 @@
     )
 
     # Non expiring discord objects cache
     user_cache: dict = attrs.field(repr=False, factory=dict)  # key: user_id
     member_cache: dict = attrs.field(repr=False, factory=dict)  # key: (guild_id, user_id)
     channel_cache: dict = attrs.field(repr=False, factory=dict)  # key: channel_id
     guild_cache: dict = attrs.field(repr=False, factory=dict)  # key: guild_id
+    scheduled_events_cache: dict = attrs.field(repr=False, factory=dict)  # key: guild_scheduled_event_id
 
     # Expiring discord objects cache
     message_cache: TTLCache = attrs.field(repr=False, factory=TTLCache)  # key: (channel_id, message_id)
     role_cache: TTLCache = attrs.field(repr=False, factory=dict)  # key: role_id
     voice_state_cache: TTLCache = attrs.field(repr=False, factory=dict)  # key: user_id
     bot_voice_state_cache: dict = attrs.field(repr=False, factory=dict)  # key: guild_id
 
@@ -899,7 +901,47 @@
         Args:
             emoji_id: The ID of the emoji
         """
         if self.emoji_cache is not None:
             self.emoji_cache.pop(to_snowflake(emoji_id), None)
 
     # endregion Emoji cache
+
+    # region ScheduledEvents cache
+
+    def get_scheduled_event(self, scheduled_event_id: "Snowflake_Type") -> Optional["ScheduledEvent"]:
+        """
+        Get a scheduled event based on the scheduled event ID.
+
+        Args:
+            scheduled_event_id: The ID of the scheduled event
+
+        Returns:
+            The ScheduledEvent if found
+        """
+        return self.scheduled_events_cache.get(to_snowflake(scheduled_event_id))
+
+    def place_scheduled_event_data(self, data: discord_typings.GuildScheduledEventData) -> "ScheduledEvent":
+        """
+        Take json data representing a scheduled event, process it, and cache it.
+
+        Args:
+            data: json representation of the scheduled event
+
+        Returns:
+            The processed scheduled event
+        """
+        scheduled_event = ScheduledEvent.from_dict(data, self._client)
+        self.scheduled_events_cache[scheduled_event.id] = scheduled_event
+
+        return scheduled_event
+
+    def delete_scheduled_event(self, scheduled_event_id: "Snowflake_Type") -> None:
+        """
+        Delete a scheduled event from the cache.
+
+        Args:
+            scheduled_event_id: The ID of the scheduled event
+        """
+        self.scheduled_events_cache.pop(to_snowflake(scheduled_event_id), None)
+
+    # endregion ScheduledEvents cache
```

### Comparing `discord-py-interactions-5.8.0/interactions/client/utils/__init__.py` & `discord-py-interactions-5.9.0/interactions/client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/client/utils/attr_converters.py` & `discord-py-interactions-5.9.0/interactions/client/utils/attr_converters.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/client/utils/attr_utils.py` & `discord-py-interactions-5.9.0/interactions/client/utils/attr_utils.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/client/utils/attr_utils.pyi` & `discord-py-interactions-5.9.0/interactions/client/utils/attr_utils.pyi`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/client/utils/cache.py` & `discord-py-interactions-5.9.0/interactions/client/utils/cache.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/client/utils/deserialise_app_cmds.py` & `discord-py-interactions-5.9.0/interactions/client/utils/deserialise_app_cmds.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/client/utils/formatting.py` & `discord-py-interactions-5.9.0/interactions/client/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/client/utils/input_utils.py` & `discord-py-interactions-5.9.0/interactions/client/utils/input_utils.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/client/utils/misc_utils.py` & `discord-py-interactions-5.9.0/interactions/client/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/client/utils/serializer.py` & `discord-py-interactions-5.9.0/interactions/client/utils/serializer.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/client/utils/text_utils.py` & `discord-py-interactions-5.9.0/interactions/client/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/ext/console.py` & `discord-py-interactions-5.9.0/interactions/ext/console.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/ext/debug_extension/__init__.py` & `discord-py-interactions-5.9.0/interactions/ext/debug_extension/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 import platform
 import tracemalloc
+from typing import ClassVar
 
 from interactions import (
     Client,
     Extension,
     listen,
     slash_command,
     InteractionContext,
@@ -24,15 +25,15 @@
 
 class DebugExtension(DebugExec, DebugAppCMD, DebugExts, Extension):
     class Metadata(Extension.Metadata):
         name = "Debug Extension"
         description = "Debugging utilities for interactions.py"
         version = "1.0.0"
         url = "https://github.com/interactions-py/interactions.py"
-        requirements = ["interactions>=5.0.0"]
+        requirements: ClassVar[list] = ["interactions>=5.0.0"]
 
     def __init__(self, bot: Client) -> None:
         bot.logger.info("Debug Extension is mounting!")
 
         super().__init__(bot)
         self.add_ext_check(checks.is_owner())
```

### Comparing `discord-py-interactions-5.8.0/interactions/ext/debug_extension/debug_application_cmd.py` & `discord-py-interactions-5.9.0/interactions/ext/debug_extension/debug_application_cmd.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/ext/debug_extension/debug_exec.py` & `discord-py-interactions-5.9.0/interactions/ext/debug_extension/debug_exec.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/ext/debug_extension/debug_exts.py` & `discord-py-interactions-5.9.0/interactions/ext/debug_extension/debug_exts.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/ext/debug_extension/utils.py` & `discord-py-interactions-5.9.0/interactions/ext/debug_extension/utils.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/ext/hybrid_commands/context.py` & `discord-py-interactions-5.9.0/interactions/ext/hybrid_commands/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,14 +114,16 @@
     def from_prefixed_context(cls, ctx: prefixed.PrefixedContext) -> Self:
         # this is a "best guess" on what the permissions are
         # this may or may not be totally accurate
         if hasattr(ctx.channel, "permissions_for"):
             app_permissions = ctx.channel.permissions_for(ctx.guild.me)  # type: ignore
         elif ctx.channel.type in {10, 11, 12}:  # it's a thread
             app_permissions = ctx.channel.parent_channel.permissions_for(ctx.guild.me)  # type: ignore
+        else:
+            app_permissions = Permissions(0)
 
         self = cls(ctx.client)
         self.guild_id = ctx.guild_id
         self.channel_id = ctx.channel_id
         self.author_id = ctx.author_id
         self.message_id = ctx.message_id
         self._message = ctx.message
```

### Comparing `discord-py-interactions-5.8.0/interactions/ext/hybrid_commands/hybrid_slash.py` & `discord-py-interactions-5.9.0/interactions/ext/hybrid_commands/hybrid_slash.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import asyncio
 import inspect
-from typing import Any, Callable, List, Optional, Union, TYPE_CHECKING, Awaitable
+from typing import Any, Callable, List, Optional, Union, TYPE_CHECKING, Awaitable, Annotated, get_origin, get_args
 
 import attrs
 from interactions import (
     BaseContext,
     Converter,
+    ConsumeRest,
     NoArgumentConverter,
     Attachment,
     SlashCommandChoice,
     OptionType,
     BaseChannelConverter,
     ChannelType,
     BaseChannel,
@@ -27,15 +28,15 @@
     Permissions,
 )
 from interactions.client.const import AsyncCallable, GLOBAL_SCOPE
 from interactions.client.utils.serializer import no_export_meta
 from interactions.client.utils.misc_utils import maybe_coroutine, get_object_name
 from interactions.client.errors import BadArgument
 from interactions.ext.prefixed_commands import PrefixedCommand, PrefixedContext
-from interactions.models.internal.converters import _LiteralConverter
+from interactions.models.internal.converters import _LiteralConverter, CONSUME_REST_MARKER
 from interactions.models.internal.checks import guild_only
 
 if TYPE_CHECKING:
     from .context import HybridContext
 
 __all__ = ("HybridSlashCommand", "hybrid_slash_command", "hybrid_slash_subcommand")
 
@@ -234,15 +235,15 @@
 
     async def __call__(self, context: SlashContext, *args, **kwargs) -> None:
         new_ctx = context.client.hybrid.hybrid_context.from_slash_context(context)
         await super().__call__(new_ctx, *args, **kwargs)
 
     def group(
         self,
-        name: str = None,
+        name: str | None = None,
         description: str = "No Description Set",
         inherit_checks: bool = True,
         aliases: list[str] | None = None,
     ) -> "HybridSlashCommand":
         self._dummy_base = True
         return HybridSlashCommand(
             name=self.name,
@@ -258,15 +259,15 @@
 
     def subcommand(
         self,
         sub_cmd_name: Absent[LocalisedName | str] = MISSING,
         group_name: LocalisedName | str = None,
         sub_cmd_description: Absent[LocalisedDesc | str] = MISSING,
         group_description: Absent[LocalisedDesc | str] = MISSING,
-        options: List[Union[SlashCommandOption, dict]] = None,
+        options: List[Union[SlashCommandOption, dict]] | None = None,
         nsfw: bool = False,
         inherit_checks: bool = True,
         aliases: list[str] | None = None,
         silence_autocomplete_errors: bool = True,
     ) -> Callable[..., "HybridSlashCommand"]:
         def wrapper(call: AsyncCallable) -> "HybridSlashCommand":
             nonlocal sub_cmd_name, sub_cmd_description
@@ -346,25 +347,37 @@
             # makes my life easier
             option = SlashCommandOption(**option)
 
         if option.autocomplete and not cmd._silence_autocomplete_errors:
             # there isn't much we can do here
             raise ValueError("Autocomplete is unsupported in hybrid commands.")
 
-        name = str(option.name)
+        name = option.argument_name or str(option.name)
         annotation = inspect.Parameter.empty
         default = inspect.Parameter.empty
         kind = inspect.Parameter.POSITIONAL_ONLY if cmd._uses_arg else inspect.Parameter.POSITIONAL_OR_KEYWORD
 
+        consume_rest: bool = False
+
         if slash_param := cmd.parameters.get(name):
             kind = slash_param.kind
 
             if kind == inspect.Parameter.KEYWORD_ONLY:  # work around prefixed cmd parsing
                 kind = inspect.Parameter.POSITIONAL_OR_KEYWORD
 
+            # here come the hacks - these allow ConsumeRest (the class) to be passed through
+            if get_origin(slash_param.type) == Annotated:
+                args = get_args(slash_param.type)
+                # ComsumeRest[str] or Annotated[ConsumeRest[str], Converter] support
+                # by all means, the second isn't allowed in prefixed commands, but we'll ignore that for converter support for slash cmds
+                if args[1] is CONSUME_REST_MARKER or (
+                    args[0] == Annotated and get_args(args[0])[1] is CONSUME_REST_MARKER
+                ):
+                    consume_rest = True
+
             if slash_param.converter:
                 annotation = slash_param.converter
             if slash_param.default is not MISSING:
                 default = slash_param.default
 
         if option.choices:
             option_anno = ChoicesConverter(option.choices)
@@ -383,14 +396,17 @@
             annotation = ChainNoArgConverter(option_anno, annotation, name)
         else:
             annotation = ChainConverter(option_anno, annotation, name)
 
         if not option.required and default == inspect.Parameter.empty:
             default = None
 
+        if consume_rest:
+            annotation = ConsumeRest[annotation]
+
         actual_param = inspect.Parameter(
             name=name,
             kind=kind,
             default=default,
             annotation=annotation,
         )
         fake_sig_parameters.append(actual_param)
@@ -521,16 +537,16 @@
     description: Absent[str | LocalisedDesc] = MISSING,
     base_description: Optional[str | LocalisedDesc] = None,
     base_desc: Optional[str | LocalisedDesc] = None,
     base_default_member_permissions: Optional["Permissions"] = None,
     base_dm_permission: bool = True,
     subcommand_group_description: Optional[str | LocalisedDesc] = None,
     sub_group_desc: Optional[str | LocalisedDesc] = None,
-    scopes: List["Snowflake_Type"] = None,
-    options: List[dict] = None,
+    scopes: List["Snowflake_Type"] | None = None,
+    options: List[dict] | None = None,
     nsfw: bool = False,
     silence_autocomplete_errors: bool = False,
 ) -> Callable[[AsyncCallable], HybridSlashCommand]:
     """
     A decorator specifically tailored for creating hybrid slash subcommands.
 
     Args:
```

### Comparing `discord-py-interactions-5.8.0/interactions/ext/hybrid_commands/manager.py` & `discord-py-interactions-5.9.0/interactions/ext/hybrid_commands/manager.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/ext/jurigged.py` & `discord-py-interactions-5.9.0/interactions/ext/jurigged.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/ext/mypy/__init__.py` & `discord-py-interactions-5.9.0/interactions/ext/mypy/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/ext/paginators.py` & `discord-py-interactions-5.9.0/interactions/ext/paginators.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/ext/prefixed_commands/__init__.py` & `discord-py-interactions-5.9.0/interactions/ext/prefixed_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/ext/prefixed_commands/command.py` & `discord-py-interactions-5.9.0/interactions/ext/prefixed_commands/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,23 +14,24 @@
     Type,
     TypeGuard,
 )
 
 import attrs
 from typing_extensions import Self
 
-from interactions.client.const import MISSING
+from interactions.client.const import MISSING, T
 from interactions.client.errors import BadArgument
 from interactions.client.utils.input_utils import _quotes
 from interactions.client.utils.misc_utils import get_object_name, maybe_coroutine
 from interactions.models.internal.command import BaseCommand
 from interactions.models.internal.converters import (
     _LiteralConverter,
     NoArgumentConverter,
     Greedy,
+    CONSUME_REST_MARKER,
     MODEL_TO_CONVERTER,
 )
 from interactions.models.internal.protocols import Converter
 from ...client.utils.attr_utils import docs
 
 if TYPE_CHECKING:
     from .context import PrefixedContext
@@ -58,14 +59,15 @@
         "type",
         "kind",
         "converters",
         "greedy",
         "union",
         "variable",
         "consume_rest",
+        "consume_rest_class",
         "no_argument",
     )
 
     name: str
     "The name of the parameter."
     default: Any
     "The default value of the parameter."
@@ -86,15 +88,15 @@
     no_argument: bool
     "Does this parameter have a converter that subclasses `NoArgumentConverter`?"
 
     def __init__(
         self,
         name: str,
         default: Any = MISSING,
-        type: Type = None,
+        type: Type | None = None,
         kind: inspect._ParameterKind = inspect._ParameterKind.POSITIONAL_OR_KEYWORD,
         converters: Optional[list[Callable[["PrefixedContext", str], Any]]] = None,
         greedy: bool = False,
         union: bool = False,
         variable: bool = False,
         consume_rest: bool = False,
         no_argument: bool = False,
@@ -495,21 +497,47 @@
         for name, param in params.items():
             if finished_params:
                 raise ValueError("Cannot have multiple keyword-only or variable arguments.")
 
             cmd_param = PrefixedCommandParameter.from_param(param)
             anno = param.annotation
 
+            # this is ugly, ik
+            if typing.get_origin(anno) == Annotated and typing.get_args(anno)[1] is CONSUME_REST_MARKER:
+                cmd_param.consume_rest = True
+                finished_params = True
+                anno = typing.get_args(anno)[0]
+
+                if anno == T:
+                    # someone forgot to typehint
+                    anno = inspect._empty
+
+            if typing.get_origin(anno) == Annotated:
+                anno = _get_from_anno_type(anno)
+
             if typing.get_origin(anno) == Greedy:
+                if finished_params:
+                    raise ValueError("Consume rest arguments cannot be Greedy.")
+
                 anno, default = _greedy_parse(anno, param)
 
                 if default is not param.empty:
                     cmd_param.default = default
                 cmd_param.greedy = True
 
+            if typing.get_origin(anno) == tuple:
+                if cmd_param.optional:
+                    # there's a lot of parser ambiguities here, so i'd rather not
+                    raise ValueError("Variable arguments cannot have default values or be Optional.")
+                cmd_param.variable = True
+                finished_params = True
+
+                # use empty if the typehint is just "tuple"
+                anno = typing.get_args(anno)[0] if typing.get_args(anno) else inspect._empty
+
             if typing.get_origin(anno) in {Union, UnionType}:
                 cmd_param.union = True
                 for arg in typing.get_args(anno):
                     if _check_for_no_arg(anno):
                         cmd_param.no_argument = True
 
                     if arg != NoneType:
@@ -520,30 +548,31 @@
             else:
                 if _check_for_no_arg(anno):
                     cmd_param.no_argument = True
 
                 converter = _get_converter(anno, name)
                 cmd_param.converters.append(converter)
 
-            match param.kind:
-                case param.KEYWORD_ONLY:
-                    if cmd_param.greedy:
-                        raise ValueError("Keyword-only arguments cannot be Greedy.")
-
-                    cmd_param.consume_rest = True
-                    finished_params = True
-                case param.VAR_POSITIONAL:
-                    if cmd_param.optional:
-                        # there's a lot of parser ambiguities here, so i'd rather not
-                        raise ValueError("Variable arguments cannot have default values or be Optional.")
-                    if cmd_param.greedy:
-                        raise ValueError("Variable arguments cannot be Greedy.")
+            if not finished_params:
+                match param.kind:
+                    case param.KEYWORD_ONLY:
+                        if cmd_param.greedy:
+                            raise ValueError("Consume rest arguments cannot be Greedy.")
+
+                        cmd_param.consume_rest = True
+                        finished_params = True
+                    case param.VAR_POSITIONAL:
+                        if cmd_param.optional:
+                            # there's a lot of parser ambiguities here, so i'd rather not
+                            raise ValueError("Variable arguments cannot have default values or be Optional.")
+                        if cmd_param.greedy:
+                            raise ValueError("Variable arguments cannot be Greedy.")
 
-                    cmd_param.variable = True
-                    finished_params = True
+                        cmd_param.variable = True
+                        finished_params = True
 
             self.parameters.append(cmd_param)
 
         # we need to deal with subcommands too
         for command in self.all_subcommands:
             command._parse_parameters()
 
@@ -694,15 +723,22 @@
                 if param.consume_rest:
                     arg = args.consume_rest()
 
                 if param.variable:
                     args_to_convert = args.get_rest_of_args()
                     new_arg = [await _convert(param, ctx, arg) for arg in args_to_convert]
                     new_arg = tuple(arg[0] for arg in new_arg)
-                    new_args.extend(new_arg)
+
+                    if param.kind == inspect.Parameter.VAR_POSITIONAL:
+                        new_args.extend(new_arg)
+                    elif param.kind == inspect.Parameter.POSITIONAL_ONLY:
+                        new_args.append(new_arg)
+                    else:
+                        kwargs[param.name] = new_arg
+
                     param_index += 1
                     break
 
                 if param.greedy:
                     greedy_args, broke_off = await _greedy_convert(param, ctx, args)
 
                     new_args.append(greedy_args)
```

### Comparing `discord-py-interactions-5.8.0/interactions/ext/prefixed_commands/context.py` & `discord-py-interactions-5.9.0/interactions/ext/prefixed_commands/context.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import TYPE_CHECKING, Any, Iterable, Optional, Union
 
 from typing_extensions import Self
 
 from interactions.client.client import Client
 from interactions.client.mixins.send import SendMixin
+from interactions.models.discord.channel import TYPE_MESSAGEABLE_CHANNEL
 from interactions.models.discord.embed import Embed
 from interactions.models.discord.file import UPLOADABLE_TYPE
 from interactions.models.discord.message import Message
 from interactions.models.internal.context import BaseContext
 from interactions.models.misc.context_manager import Typing
 
 if TYPE_CHECKING:
@@ -59,14 +60,19 @@
 
     @property
     def message(self) -> Message:
         """The message that invoked this context."""
         return self._message
 
     @property
+    def channel(self) -> TYPE_MESSAGEABLE_CHANNEL:
+        """The channel this context was invoked in."""
+        return self.message.channel
+
+    @property
     def invoke_target(self) -> str:
         """The name of the command to be invoked."""
         return self.command.name
 
     @property
     def typing(self) -> Typing:
         """A context manager to send a typing state to the context's channel as long as the wrapped operation takes."""
```

### Comparing `discord-py-interactions-5.8.0/interactions/ext/prefixed_commands/help.py` & `discord-py-interactions-5.9.0/interactions/ext/prefixed_commands/help.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/ext/prefixed_commands/manager.py` & `discord-py-interactions-5.9.0/interactions/ext/prefixed_commands/manager.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/ext/prefixed_commands/utils.py` & `discord-py-interactions-5.9.0/interactions/ext/prefixed_commands/utils.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/ext/sentry.py` & `discord-py-interactions-5.9.0/interactions/ext/sentry.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
             scope.set_tag("iteration", self.iteration)
             sentry_sdk.capture_exception(error)
 
 
 def setup(
     bot: Client,
-    token: str = None,
+    token: str | None = None,
     filter: Optional[Callable[[dict[str, Any], dict[str, Any]], Optional[dict[str, Any]]]] = None,
     **kwargs,
 ) -> None:
     if not token:
         bot.logger.error("Cannot enable sentry integration, no token provided")
         return
     if filter is None:
```

### Comparing `discord-py-interactions-5.8.0/interactions/models/__init__.py` & `discord-py-interactions-5.9.0/interactions/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,14 +183,15 @@
     VideoQualityMode,
     VoiceRegion,
     VoiceState,
     Webhook,
     WebhookMixin,
     WebhookTypes,
     WebSocketOPCode,
+    ForumSortOrder,
 )
 from .internal import (
     ActiveVoiceState,
     application_commands_to_dict,
     auto_defer,
     AutocompleteContext,
     AutoDefer,
@@ -206,14 +207,15 @@
     check,
     component_callback,
     ComponentCommand,
     ComponentContext,
     context_menu,
     user_context_menu,
     message_context_menu,
+    ConsumeRest,
     ContextMenu,
     ContextMenuContext,
     Converter,
     cooldown,
     Cooldown,
     CooldownSystem,
     SlidingWindowSystem,
@@ -358,14 +360,15 @@
     "COLOR_TYPES",
     "Colour",
     "CommandType",
     "component_callback",
     "ComponentCommand",
     "ComponentContext",
     "ComponentType",
+    "ConsumeRest",
     "context_menu",
     "ContextMenu",
     "ContextMenuContext",
     "Converter",
     "cooldown",
     "Cooldown",
     "CooldownSystem",
@@ -392,14 +395,15 @@
     "EmbedFooter",
     "EmbedProvider",
     "ExplicitContentFilterLevel",
     "Extension",
     "File",
     "FlatUIColors",
     "FlatUIColours",
+    "ForumSortOrder",
     "ForumLayoutType",
     "get_components_ids",
     "global_autocomplete",
     "GlobalAutoComplete",
     "Greedy",
     "Guild",
     "guild_only",
```

### Comparing `discord-py-interactions-5.8.0/interactions/models/discord/__init__.py` & `discord-py-interactions-5.9.0/interactions/models/discord/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,15 @@
     StickerTypes,
     SystemChannelFlags,
     TeamMembershipState,
     UserFlags,
     VerificationLevel,
     VideoQualityMode,
     WebSocketOPCode,
+    ForumSortOrder,
 )
 from .file import File, open_file, UPLOADABLE_TYPE
 from .guild import (
     AuditLog,
     AuditLogChange,
     AuditLogEntry,
     AuditLogHistory,
@@ -222,14 +223,15 @@
     "EmbedField",
     "EmbedFooter",
     "EmbedProvider",
     "ExplicitContentFilterLevel",
     "File",
     "FlatUIColors",
     "FlatUIColours",
+    "ForumSortOrder",
     "ForumLayoutType",
     "get_components_ids",
     "Guild",
     "GuildBan",
     "GuildCategory",
     "GuildChannel",
     "GuildForum",
```

### Comparing `discord-py-interactions-5.8.0/interactions/models/discord/activity.py` & `discord-py-interactions-5.9.0/interactions/models/discord/activity.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/discord/app_perms.py` & `discord-py-interactions-5.9.0/interactions/models/discord/app_perms.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/discord/application.py` & `discord-py-interactions-5.9.0/interactions/models/discord/application.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/discord/asset.py` & `discord-py-interactions-5.9.0/interactions/models/discord/asset.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/discord/auto_mod.py` & `discord-py-interactions-5.9.0/interactions/models/discord/auto_mod.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/discord/base.py` & `discord-py-interactions-5.9.0/interactions/models/discord/base.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/discord/channel.py` & `discord-py-interactions-5.9.0/interactions/models/discord/channel.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,16 @@
     OverwriteType,
     Permissions,
     VideoQualityMode,
     AutoArchiveDuration,
     StagePrivacyLevel,
     MessageFlags,
     InviteTargetType,
+    ForumSortOrder,
+    ForumLayoutType,
 )
 
 if TYPE_CHECKING:
     from aiohttp import FormData
     from interactions import Client, Embed, BaseComponent, AllowedMentions, Sticker, Message
     from interactions.models.internal.active_voice_state import ActiveVoiceState
 
@@ -236,14 +238,16 @@
     """The id of the last message sent in this channel (may not point to an existing or valid message)"""
     default_auto_archive_duration: int = attrs.field(repr=False, default=AutoArchiveDuration.ONE_DAY)
     """Default duration that the clients (not the API) will use for newly created threads, in minutes, to automatically archive the thread after recent activity"""
     last_pin_timestamp: Optional["models.Timestamp"] = attrs.field(
         repr=False, default=None, converter=optional_c(timestamp_converter)
     )
     """When the last pinned message was pinned. This may be None when a message is not pinned."""
+    rate_limit_per_user: int = attrs.field(repr=False, default=0)
+    """Amount of seconds a user has to wait before sending another message (0-21600)"""
 
     async def _send_http_request(
         self, message_payload: Union[dict, "FormData"], files: list["UPLOADABLE_TYPE"] | None = None
     ) -> dict:
         return await self._client.http.create_message(message_payload, self.id, files=files)
 
     async def fetch_message(self, message_id: Snowflake_Type, *, force: bool = False) -> Optional["models.Message"]:
@@ -383,15 +387,15 @@
 
         if len(message_ids) == 1:
             # bulk delete messages will throw a http error if only 1 message is passed
             await self.delete_message(message_ids[0], reason)
         else:
             await self._client.http.bulk_delete_messages(self.id, message_ids, reason)
 
-    async def delete_message(self, message: Union[Snowflake_Type, "models.Message"], reason: str = None) -> None:
+    async def delete_message(self, message: Union[Snowflake_Type, "models.Message"], reason: str | None = None) -> None:
         """
         Delete a single message from a channel.
 
         Args:
             message: The message to delete
             reason: The reason for this action
 
@@ -557,15 +561,15 @@
         self,
         name: str,
         message: Absent[Snowflake_Type] = MISSING,
         thread_type: Absent[ChannelType] = MISSING,
         invitable: Absent[bool] = MISSING,
         rate_limit_per_user: Absent[int] = MISSING,
         auto_archive_duration: AutoArchiveDuration = AutoArchiveDuration.ONE_DAY,
-        reason: Absent[str] = None,
+        reason: Absent[str] | None = None,
     ) -> "TYPE_THREAD_CHANNEL":
         """
         Creates a new thread in this channel. If a message is provided, it will be used as the initial message.
 
         Args:
             name: 1-100 character thread name
             message: The message to connect this thread to. Required for news channel.
@@ -597,15 +601,15 @@
             auto_archive_duration=auto_archive_duration,
             message_id=to_optional_snowflake(message),
             reason=reason,
         )
         return self._client.cache.place_channel_data(thread_data)
 
     async def fetch_public_archived_threads(
-        self, limit: int = None, before: Optional["models.Timestamp"] = None
+        self, limit: int | None = None, before: Optional["models.Timestamp"] = None
     ) -> "models.ThreadList":
         """
         Get a `ThreadList` of archived **public** threads available in this channel.
 
         Args:
             limit: optional maximum number of threads to return
             before: Returns threads before this timestamp
@@ -617,15 +621,15 @@
         threads_data = await self._client.http.list_public_archived_threads(
             channel_id=self.id, limit=limit, before=before
         )
         threads_data["id"] = self.id
         return models.ThreadList.from_dict(threads_data, self._client)
 
     async def fetch_private_archived_threads(
-        self, limit: int = None, before: Optional["models.Timestamp"] = None
+        self, limit: int | None = None, before: Optional["models.Timestamp"] = None
     ) -> "models.ThreadList":
         """
         Get a `ThreadList` of archived **private** threads available in this channel.
 
         Args:
             limit: optional maximum number of threads to return
             before: Returns threads before this timestamp
@@ -637,15 +641,15 @@
         threads_data = await self._client.http.list_private_archived_threads(
             channel_id=self.id, limit=limit, before=before
         )
         threads_data["id"] = self.id
         return models.ThreadList.from_dict(threads_data, self._client)
 
     async def fetch_archived_threads(
-        self, limit: int = None, before: Optional["models.Timestamp"] = None
+        self, limit: int | None = None, before: Optional["models.Timestamp"] = None
     ) -> "models.ThreadList":
         """
         Get a `ThreadList` of archived threads available in this channel.
 
         Args:
             limit: optional maximum number of threads to return
             before: Returns threads before this timestamp
@@ -660,15 +664,15 @@
         threads_data.update(
             await self._client.http.list_public_archived_threads(channel_id=self.id, limit=limit, before=before)
         )
         threads_data["id"] = self.id
         return models.ThreadList.from_dict(threads_data, self._client)
 
     async def fetch_joined_private_archived_threads(
-        self, limit: int = None, before: Optional["models.Timestamp"] = None
+        self, limit: int | None = None, before: Optional["models.Timestamp"] = None
     ) -> "models.ThreadList":
         """
         Get a `ThreadList` of threads the bot is a participant of in this channel.
 
         Args:
             limit: optional maximum number of threads to return
             before: Returns threads before this timestamp
@@ -1216,15 +1220,15 @@
         use_external_stickers: bool | None = None,
         use_private_threads: bool | None = None,
         use_public_threads: bool | None = None,
         use_vad: bool | None = None,
         view_audit_log: bool | None = None,
         view_channel: bool | None = None,
         view_guild_insights: bool | None = None,
-        reason: str = None,
+        reason: str | None = None,
     ) -> None:
         """
         Set the Permission Overwrites for a given target.
 
         Args:
             target: The target to set permission overwrites for
             add_reactions: Allows for the addition of reactions to messages
@@ -1660,15 +1664,15 @@
         await self._client.http.follow_news_channel(self.id, webhook_channel_id)
 
     async def create_thread_from_message(
         self,
         name: str,
         message: Snowflake_Type,
         auto_archive_duration: AutoArchiveDuration = AutoArchiveDuration.ONE_DAY,
-        reason: Absent[str] = None,
+        reason: Absent[str] | None = None,
     ) -> "GuildNewsThread":
         """
         Creates a new news thread in this channel.
 
         Args:
             name: 1-100 character thread name.
             message: The message to connect this thread to.
@@ -1687,16 +1691,14 @@
         )
 
 
 @attrs.define(eq=False, order=False, hash=False, kw_only=True)
 class GuildText(GuildChannel, MessageableMixin, InvitableMixin, ThreadableMixin, WebhookMixin):
     topic: Optional[str] = attrs.field(repr=False, default=None)
     """The channel topic (0-1024 characters)"""
-    rate_limit_per_user: int = attrs.field(repr=False, default=0)
-    """Amount of seconds a user has to wait before sending another message (0-21600)"""
 
     async def edit(
         self,
         *,
         name: Absent[str] = MISSING,
         position: Absent[int] = MISSING,
         permission_overwrites: Absent[
@@ -1745,15 +1747,15 @@
         )
 
     async def create_public_thread(
         self,
         name: str,
         auto_archive_duration: AutoArchiveDuration = AutoArchiveDuration.ONE_DAY,
         rate_limit_per_user: Absent[int] = MISSING,
-        reason: Absent[str] = None,
+        reason: Absent[str] | None = None,
     ) -> "GuildPublicThread":
         """
         Creates a new public thread in this channel.
 
         Args:
             name: 1-100 character thread name.
             auto_archive_duration: Time before the thread will be automatically archived. Note 3 day and 7 day archive durations require the server to be boosted.
@@ -1774,15 +1776,15 @@
 
     async def create_private_thread(
         self,
         name: str,
         invitable: Absent[bool] = MISSING,
         auto_archive_duration: AutoArchiveDuration = AutoArchiveDuration.ONE_DAY,
         rate_limit_per_user: Absent[int] = MISSING,
-        reason: Absent[str] = None,
+        reason: Absent[str] | None = None,
     ) -> "GuildPrivateThread":
         """
         Creates a new private thread in this channel.
 
         Args:
             name: 1-100 character thread name.
             invitable: Whether non-moderators can add other non-moderators to a thread.
@@ -1804,15 +1806,15 @@
         )
 
     async def create_thread_from_message(
         self,
         name: str,
         message: Snowflake_Type,
         auto_archive_duration: AutoArchiveDuration = AutoArchiveDuration.ONE_DAY,
-        reason: Absent[str] = None,
+        reason: Absent[str] | None = None,
     ) -> "GuildPublicThread":
         """
         Creates a new public thread in this channel.
 
         Args:
             name: 1-100 character thread name.
             message: The message to connect this thread to.
@@ -2390,29 +2392,39 @@
 class GuildForum(GuildChannel):
     available_tags: List[ThreadTag] = attrs.field(repr=False, factory=list)
     """A list of tags available to assign to threads"""
     default_reaction_emoji: Optional[DefaultReaction] = attrs.field(repr=False, default=None)
     """The default emoji to react with for posts"""
     last_message_id: Optional[Snowflake_Type] = attrs.field(repr=False, default=None)
     # TODO: Implement "template" once the API supports them
+    rate_limit_per_user: int = attrs.field(repr=False, default=0)
+    """Amount of seconds a user has to wait before sending another message (0-21600)"""
+    default_sort_order: Optional[ForumSortOrder] = attrs.field(
+        repr=False, default=None, converter=ForumSortOrder.converter
+    )
+    """the default sort order type used to order posts in GUILD_FORUM channels. Defaults to null, which indicates a preferred sort order hasn't been set by a channel admin"""
+    default_forum_layout: ForumLayoutType = attrs.field(
+        repr=False, default=ForumLayoutType.NOT_SET, converter=ForumLayoutType
+    )
+    """The default forum layout view used to display posts in GUILD_FORUM channels. Defaults to 0, which indicates a layout view has not been set by a channel admin"""
 
     @classmethod
     def _process_dict(cls, data: Dict[str, Any], client: "Client") -> Dict[str, Any]:
         data = super()._process_dict(data, client)
         data["available_tags"] = [
             ThreadTag.from_dict(tag_data | {"parent_channel_id": data["id"]}, client)
             for tag_data in data.get("available_tags", [])
         ]
         return data
 
     async def create_post(
         self,
         name: str,
         content: str | None,
-        applied_tags: Optional[List[Union["Snowflake_Type", "ThreadTag", str]]] = MISSING,
+        applied_tags: Absent[List[Union["Snowflake_Type", "ThreadTag", str]]] = MISSING,
         *,
         auto_archive_duration: AutoArchiveDuration = AutoArchiveDuration.ONE_DAY,
         rate_limit_per_user: Absent[int] = MISSING,
         embeds: Optional[Union[List[Union["Embed", dict]], Union["Embed", dict]]] = None,
         embed: Optional[Union["Embed", dict]] = None,
         components: Optional[
             Union[
@@ -2447,15 +2459,15 @@
             file: Files to send, the path, bytes or File() instance, defaults to None. You may have up to 10 files.
             tts: Should this message use Text To Speech.
             reason: The reason for creating this post
 
         Returns:
             A GuildForumPost object representing the created post.
         """
-        if applied_tags != MISSING:
+        if applied_tags is not MISSING:
             processed = []
             for tag in applied_tags:
                 if isinstance(tag, ThreadTag):
                     tag = tag.id
                 elif isinstance(tag, (str, int)):
                     tag = self.get_tag(tag, case_insensitive=True)
                     if not tag:
@@ -2552,20 +2564,21 @@
         Args:
             value: The name or ID of the tag to get
             case_insensitive: Whether to ignore case when searching for the tag
 
         Returns:
             A ThreadTag object representing the tag.
         """
+        value = str(value)
 
         def maybe_insensitive(string: str) -> str:
             return string.lower() if case_insensitive else string
 
         def predicate(tag: ThreadTag) -> Optional["ThreadTag"]:
-            if str(tag.id) == str(value):
+            if str(tag.id) == value:
                 return tag
             if maybe_insensitive(tag.name) == maybe_insensitive(value):
                 return tag
 
         return next((tag for tag in self.available_tags if predicate(tag)), None)
 
     async def create_tag(self, name: str, emoji: Union["models.PartialEmoji", dict, str, None] = None) -> "ThreadTag":
@@ -2595,15 +2608,15 @@
                 payload["emoji_id"] = emoji.id
             else:
                 payload["emoji_name"] = emoji.name
 
         data = await self._client.http.create_tag(**payload)
 
         channel_data = self._client.cache.place_channel_data(data)
-        return [tag for tag in channel_data.available_tags if tag.name == name][0]
+        return next(tag for tag in channel_data.available_tags if tag.name == name)
 
     async def edit_tag(
         self,
         tag_id: "Snowflake_Type",
         *,
         name: str | None = None,
         emoji: Union["models.PartialEmoji", dict, str, None] = None,
@@ -2623,15 +2636,15 @@
 
         if emoji.id:
             data = await self._client.http.edit_tag(self.id, tag_id, name, emoji_id=emoji.id)
         else:
             data = await self._client.http.edit_tag(self.id, tag_id, name, emoji_name=emoji.name)
 
         channel_data = self._client.cache.place_channel_data(data)
-        return [tag for tag in channel_data.available_tags if tag.name == name][0]
+        return next(tag for tag in channel_data.available_tags if tag.name == name)
 
     async def delete_tag(self, tag_id: "Snowflake_Type") -> None:
         """
         Delete a tag for this forum.
 
         Args:
             tag_id: The ID of the tag to delete
```

### Comparing `discord-py-interactions-5.8.0/interactions/models/discord/color.py` & `discord-py-interactions-5.9.0/interactions/models/discord/color.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/discord/components.py` & `discord-py-interactions-5.9.0/interactions/models/discord/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,15 @@
 
     def __init__(
         self,
         *,
         style: ButtonStyle | int,
         label: str | None = None,
         emoji: "PartialEmoji | None | str" = None,
-        custom_id: str = None,
+        custom_id: str | None = None,
         url: str | None = None,
         disabled: bool = False,
     ) -> None:
         self.style: ButtonStyle = ButtonStyle(style)
         self.label: str | None = label
         self.emoji: "PartialEmoji | None" = emoji
         self.custom_id: str | None = custom_id
```

### Comparing `discord-py-interactions-5.8.0/interactions/models/discord/embed.py` & `discord-py-interactions-5.9.0/interactions/models/discord/embed.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/discord/emoji.py` & `discord-py-interactions-5.9.0/interactions/models/discord/emoji.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/discord/enums.py` & `discord-py-interactions-5.9.0/interactions/models/discord/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from enum import Enum, EnumMeta, IntEnum, IntFlag
 from functools import reduce
 from operator import or_
-from typing import Iterator, Tuple, TypeVar, Type
+from typing import Iterator, Tuple, TypeVar, Type, Optional
 
 from interactions.client.const import get_logger
 
 __all__ = (
     "ActivityFlag",
     "ActivityType",
     "ApplicationFlags",
@@ -15,14 +15,15 @@
     "ChannelFlags",
     "ChannelType",
     "CommandType",
     "ComponentType",
     "DefaultNotificationLevel",
     "ExplicitContentFilterLevel",
     "ForumLayoutType",
+    "ForumSortOrder",
     "IntegrationExpireBehaviour",
     "Intents",
     "InteractionPermissionTypes",
     "InteractionType",
     "InviteTargetType",
     "MemberFlags",
     "MentionType",
@@ -1042,7 +1043,18 @@
 
 class ForumLayoutType(CursedIntEnum):
     """The layout of a forum channel."""
 
     NOT_SET = 0
     LIST = 1
     GALLERY = 2
+
+
+class ForumSortOrder(CursedIntEnum):
+    """The order of a forum channel."""
+
+    LATEST_ACTIVITY = 0
+    CREATION_DATE = 1
+
+    @classmethod
+    def converter(cls, value: Optional[int]) -> "ForumSortOrder":
+        return None if value is None else cls(value)
```

### Comparing `discord-py-interactions-5.8.0/interactions/models/discord/file.py` & `discord-py-interactions-5.9.0/interactions/models/discord/file.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/discord/guild.py` & `discord-py-interactions-5.9.0/interactions/models/discord/guild.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     MFALevel,
     NSFWLevel,
     Permissions,
     ScheduledEventPrivacyLevel,
     ScheduledEventType,
     SystemChannelFlags,
     VerificationLevel,
+    ForumSortOrder,
 )
 from .snowflake import (
     Snowflake_Type,
     to_optional_snowflake,
     to_snowflake,
     to_snowflake_list,
 )
@@ -1019,14 +1020,15 @@
         ] = MISSING,
         category: Union[Snowflake_Type, "models.GuildCategory"] = None,
         nsfw: bool = False,
         rate_limit_per_user: int = 0,
         default_reaction_emoji: Absent[Union[dict, "models.PartialEmoji", "models.DefaultReaction", str]] = MISSING,
         available_tags: Absent["list[dict | models.ThreadTag] | dict | models.ThreadTag"] = MISSING,
         layout: ForumLayoutType = ForumLayoutType.NOT_SET,
+        sort_order: Absent[ForumSortOrder] = MISSING,
         reason: Absent[Optional[str]] = MISSING,
     ) -> "models.GuildForum":
         """
         Create a forum channel in this guild.
 
         Args:
             name: The name of the forum channel
@@ -1035,14 +1037,15 @@
             permission_overwrites: Permission overwrites to apply to the forum channel
             category: The category this forum channel should be within
             nsfw: Should this forum be marked nsfw
             rate_limit_per_user: The time users must wait between sending messages
             default_reaction_emoji: The default emoji to react with when creating a thread
             available_tags: The available tags for this forum channel
             layout: The layout of the forum channel
+            sort_order: The sort order of the forum channel
             reason: The reason for creating this channel
 
         Returns:
            The newly created forum channel.
 
         """
         return await self.create_channel(
@@ -1053,14 +1056,15 @@
             permission_overwrites=permission_overwrites,
             category=category,
             nsfw=nsfw,
             rate_limit_per_user=rate_limit_per_user,
             default_reaction_emoji=models.process_default_reaction(default_reaction_emoji),
             available_tags=list_converter(models.process_thread_tag)(available_tags) if available_tags else MISSING,
             default_forum_layout=layout,
+            default_sort_order=sort_order,
             reason=reason,
         )
 
     async def create_news_channel(
         self,
         name: str,
         topic: Absent[Optional[str]] = MISSING,
@@ -1213,15 +1217,15 @@
             name=name,
             position=position,
             permission_overwrites=permission_overwrites,
             reason=reason,
         )
 
     async def delete_channel(
-        self, channel: Union["models.TYPE_GUILD_CHANNEL", Snowflake_Type], reason: str = None
+        self, channel: Union["models.TYPE_GUILD_CHANNEL", Snowflake_Type], reason: str | None = None
     ) -> None:
         """
         Delete the given channel, can handle either a snowflake or channel object.
 
         This is effectively just an alias for `channel.delete()`
 
         Args:
@@ -1245,15 +1249,15 @@
         List all scheduled events in this guild.
 
         Returns:
             A list of scheduled events.
 
         """
         scheduled_events_data = await self._client.http.list_schedules_events(self.id, with_user_count)
-        return models.ScheduledEvent.from_list(scheduled_events_data, self._client)
+        return [self._client.cache.place_scheduled_event_data(data) for data in scheduled_events_data]
 
     async def fetch_scheduled_event(
         self, scheduled_event_id: Snowflake_Type, with_user_count: bool = False
     ) -> Optional["models.ScheduledEvent"]:
         """
         Get a scheduled event by id.
 
@@ -1267,15 +1271,15 @@
         """
         try:
             scheduled_event_data = await self._client.http.get_scheduled_event(
                 self.id, scheduled_event_id, with_user_count
             )
         except NotFound:
             return None
-        return models.ScheduledEvent.from_dict(scheduled_event_data, self._client)
+        return self._client.cache.place_scheduled_event_data(scheduled_event_data)
 
     async def create_scheduled_event(
         self,
         name: str,
         event_type: ScheduledEventType,
         start_time: "models.Timestamp",
         end_time: Absent[Optional["models.Timestamp"]] = MISSING,
@@ -1331,15 +1335,15 @@
             "channel_id": channel_id,
             "entity_metadata": entity_metadata,
             "privacy_level": privacy_level,
             "image": to_image_data(cover_image) if cover_image else MISSING,
         }
 
         scheduled_event_data = await self._client.http.create_scheduled_event(self.id, payload, reason)
-        return models.ScheduledEvent.from_dict(scheduled_event_data, self._client)
+        return self._client.cache.place_scheduled_event_data(scheduled_event_data)
 
     async def create_custom_sticker(
         self,
         name: str,
         file: UPLOADABLE_TYPE,
         tags: list[str],
         description: Absent[Optional[str]] = MISSING,
@@ -1867,15 +1871,15 @@
         Args:
             user: The user to unban
             reason: The reason for the ban
 
         """
         await self._client.http.remove_guild_ban(self.id, to_snowflake(user), reason=reason)
 
-    async def fetch_widget_image(self, style: str = None) -> str:
+    async def fetch_widget_image(self, style: str | None = None) -> str:
         """
         Fetch a guilds widget image.
 
         For a list of styles, look here: https://discord.com/developers/docs/resources/guild#get-guild-widget-image-widget-style-options
 
         Args:
             style: The style to use for the widget image
```

### Comparing `discord-py-interactions-5.8.0/interactions/models/discord/invite.py` & `discord-py-interactions-5.9.0/interactions/models/discord/invite.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,73 +11,79 @@
 from interactions.models.discord.snowflake import to_snowflake
 from interactions.models.discord.stage_instance import StageInstance
 from interactions.models.discord.timestamp import Timestamp
 from .base import ClientObject
 
 if TYPE_CHECKING:
     from interactions.client import Client
-    from interactions.models import TYPE_GUILD_CHANNEL
+    from interactions.models import TYPE_GUILD_CHANNEL, Guild
     from interactions.models.discord.user import User
     from interactions.models.discord.snowflake import Snowflake_Type
 
 __all__ = ("Invite",)
 
 
 @attrs.define(eq=False, order=False, hash=False, kw_only=True)
 class Invite(ClientObject):
     code: str = attrs.field(repr=True)
-    """the invite code (unique ID)"""
+    """The invite code (unique ID)"""
 
     # metadata
     uses: int = attrs.field(default=0, repr=True)
-    """the guild this invite is for"""
+    """How many times this invite has been used"""
     max_uses: int = attrs.field(repr=False, default=0)
-    """max number of times this invite can be used"""
+    """Max number of times this invite can be used"""
     max_age: int = attrs.field(repr=False, default=0)
-    """duration (in seconds) after which the invite expires"""
+    """Duration (in seconds) after which the invite expires"""
     created_at: Timestamp = attrs.field(default=MISSING, converter=optional_c(timestamp_converter), repr=True)
-    """when this invite was created"""
+    """When this invite was created"""
     temporary: bool = attrs.field(default=False, repr=True)
-    """whether this invite only grants temporary membership"""
+    """Whether this invite only grants temporary membership"""
 
     # target data
     target_type: Optional[Union[InviteTargetType, int]] = attrs.field(
         default=None, converter=optional_c(InviteTargetType), repr=True
     )
-    """the type of target for this voice channel invite"""
+    """The type of target for this voice channel invite"""
     approximate_presence_count: Optional[int] = attrs.field(repr=False, default=MISSING)
-    """approximate count of online members, returned from the `GET /invites/<code>` endpoint when `with_counts` is `True`"""
+    """Approximate count of online members, returned when fetching invites with `with_counts` set as `True`"""
     approximate_member_count: Optional[int] = attrs.field(repr=False, default=MISSING)
-    """approximate count of total members, returned from the `GET /invites/<code>` endpoint when `with_counts` is `True`"""
+    """Approximate count of total members, returned when fetching invites with `with_counts` set as `True`"""
     scheduled_event: Optional["Snowflake_Type"] = attrs.field(
         default=None, converter=optional_c(to_snowflake), repr=True
     )
-    """guild scheduled event data, only included if `guild_scheduled_event_id` contains a valid guild scheduled event id"""
+    """Guild scheduled event data, only included if `guild_scheduled_event_id` contains a valid guild scheduled event id"""
     expires_at: Optional[Timestamp] = attrs.field(default=None, converter=optional_c(timestamp_converter), repr=True)
-    """the expiration date of this invite, returned from the `GET /invites/<code>` endpoint when `with_expiration` is `True`"""
+    """The expiration date of this invite, returned when fetching invites with `with_expiration` set as `True`"""
     stage_instance: Optional[StageInstance] = attrs.field(repr=False, default=None)
-    """stage instance data if there is a public Stage instance in the Stage channel this invite is for (deprecated)"""
+    """Stage instance data if there is a public Stage instance in the Stage channel this invite is for (deprecated)"""
     target_application: Optional[dict] = attrs.field(repr=False, default=None)
-    """the embedded application to open for this voice channel embedded application invite"""
+    """The embedded application to open for this voice channel embedded application invite"""
     guild_preview: Optional[GuildPreview] = attrs.field(repr=False, default=MISSING)
-    """the guild this invite is for"""
+    """The guild this invite is for - not given in invite events"""
 
     # internal for props
     _channel_id: "Snowflake_Type" = attrs.field(converter=to_snowflake, repr=True)
+    _guild_id: Optional["Snowflake_Type"] = attrs.field(default=None, converter=optional_c(to_snowflake), repr=True)
     _inviter_id: Optional["Snowflake_Type"] = attrs.field(default=None, converter=optional_c(to_snowflake), repr=True)
     _target_user_id: Optional["Snowflake_Type"] = attrs.field(
         repr=False, default=None, converter=optional_c(to_snowflake)
     )
 
     @property
-    def channel(self) -> "TYPE_GUILD_CHANNEL":
-        """The channel the invite is for."""
+    def channel(self) -> Optional["TYPE_GUILD_CHANNEL"]:
+        """The cached channel the invite is for."""
         return self._client.cache.get_channel(self._channel_id)
 
     @property
+    def guild(self) -> Optional["Guild"]:
+        """The cached guild the invite is."""
+        return self._client.cache.get_guild(self._guild_id) if self._guild_id else None
+
+    @property
     def inviter(self) -> Optional["User"]:
         """The user that created the invite or None."""
         return self._client.cache.get_user(self._inviter_id) if self._inviter_id else None
 
     @property
     def target_user(self) -> Optional["User"]:
         """The user whose stream to display for this voice channel stream invite or None."""
@@ -91,24 +97,31 @@
         if "target_application" in data:
             data["target_application"] = Application.from_dict(data, client)
 
         if "target_event_id" in data:
             data["scheduled_event"] = data["target_event_id"]
 
         if channel := data.pop("channel", None):
-            # invite metadata does not contain enough info to create a channel object
+            client.cache.place_channel_data(channel)
             data["channel_id"] = channel["id"]
 
         if guild := data.pop("guild", None):
             data["guild_preview"] = GuildPreview.from_dict(guild, client)
+            data["guild_id"] = guild["id"]
+        elif guild_id := data.pop("guild_id", None):
+            data["guild_id"] = guild_id
 
         if inviter := data.pop("inviter", None):
             inviter = client.cache.place_user_data(inviter)
             data["inviter_id"] = inviter.id
 
+        if target_user := data.pop("target_user", None):
+            target_user = client.cache.place_user_data(target_user)
+            data["target_user_id"] = target_user.id
+
         return data
 
     def __str__(self) -> str:
         return self.link
 
     @property
     def link(self) -> str:
```

### Comparing `discord-py-interactions-5.8.0/interactions/models/discord/message.py` & `discord-py-interactions-5.9.0/interactions/models/discord/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from interactions.client.const import GUILD_WELCOME_MESSAGES, MISSING, Absent
 from interactions.client.errors import ThreadOutsideOfGuild, NotFound
 from interactions.client.mixins.serialization import DictSerializationMixin
 from interactions.client.utils.attr_converters import optional as optional_c
 from interactions.client.utils.attr_converters import timestamp_converter
 from interactions.client.utils.serializer import dict_filter_none
 from interactions.client.utils.text_utils import mentions
-from interactions.models.discord.channel import BaseChannel
+from interactions.models.discord.channel import BaseChannel, GuildChannel
 from interactions.models.discord.emoji import process_emoji_req_format
 from interactions.models.discord.file import UPLOADABLE_TYPE
 from interactions.models.discord.embed import process_embeds
 from .base import DiscordObject
 from .enums import (
     ChannelType,
     InteractionType,
@@ -105,15 +105,15 @@
         if waveform := data.pop("waveform", None):
             data["waveform"] = bytearray(base64.b64decode(waveform))
         return data
 
 
 @attrs.define(eq=False, order=False, hash=False, kw_only=True)
 class ChannelMention(DiscordObject):
-    guild_id: "Snowflake_Type" = attrs.field(
+    guild_id: "Snowflake_Type | None" = attrs.field(
         repr=False,
     )
     """id of the guild containing the channel"""
     type: ChannelType = attrs.field(repr=False, converter=ChannelType)
     """the type of channel"""
     name: str = attrs.field(
         repr=False,
@@ -462,15 +462,15 @@
                 mention_channels.append(ChannelMention.from_dict(channel_data, client))
                 found_ids.append(channel_data["id"])
         if "content" in data:
             for channel_id in channel_mention.findall(data["content"]):
                 if channel_id not in found_ids and (channel := client.get_channel(channel_id)):
                     channel_data = {
                         "id": channel.id,
-                        "guild_id": channel._guild_id,
+                        "guild_id": channel._guild_id if isinstance(channel, GuildChannel) else None,
                         "type": channel.type,
                         "name": channel.name,
                     }
                     mention_channels.append(ChannelMention.from_dict(channel_data, client))
         if mention_channels:
             data["mention_channels"] = mention_channels
```

### Comparing `discord-py-interactions-5.8.0/interactions/models/discord/modal.py` & `discord-py-interactions-5.9.0/interactions/models/discord/modal.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/discord/reaction.py` & `discord-py-interactions-5.9.0/interactions/models/discord/reaction.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/discord/role.py` & `discord-py-interactions-5.9.0/interactions/models/discord/role.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/discord/scheduled_event.py` & `discord-py-interactions-5.9.0/interactions/models/discord/scheduled_event.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/discord/snowflake.py` & `discord-py-interactions-5.9.0/interactions/models/discord/snowflake.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/discord/stage_instance.py` & `discord-py-interactions-5.9.0/interactions/models/discord/stage_instance.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/discord/sticker.py` & `discord-py-interactions-5.9.0/interactions/models/discord/sticker.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/discord/team.py` & `discord-py-interactions-5.9.0/interactions/models/discord/team.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/discord/thread.py` & `discord-py-interactions-5.9.0/interactions/models/discord/thread.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/discord/timestamp.py` & `discord-py-interactions-5.9.0/interactions/models/discord/timestamp.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/discord/user.py` & `discord-py-interactions-5.9.0/interactions/models/discord/user.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/discord/user.pyi` & `discord-py-interactions-5.9.0/interactions/models/discord/user.pyi`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/discord/voice_state.py` & `discord-py-interactions-5.9.0/interactions/models/discord/voice_state.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/discord/webhooks.py` & `discord-py-interactions-5.9.0/interactions/models/discord/webhooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,16 +185,16 @@
         allowed_mentions: Optional[Union["AllowedMentions", dict]] = None,
         reply_to: Optional[Union["MessageReference", "Message", dict, "Snowflake_Type"]] = None,
         files: Optional[Union["UPLOADABLE_TYPE", List["UPLOADABLE_TYPE"]]] = None,
         file: Optional["UPLOADABLE_TYPE"] = None,
         tts: bool = False,
         suppress_embeds: bool = False,
         flags: Optional[Union[int, "MessageFlags"]] = None,
-        username: str = None,
-        avatar_url: str = None,
+        username: str | None = None,
+        avatar_url: str | None = None,
         wait: bool = False,
         thread: "Snowflake_Type" = None,
         **kwargs,
     ) -> Optional["Message"]:
         """
         Send a message as this webhook.
```

### Comparing `discord-py-interactions-5.8.0/interactions/models/internal/__init__.py` & `discord-py-interactions-5.9.0/interactions/models/internal/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     slash_mentionable_option,
     slash_role_option,
     slash_str_option,
     slash_user_option,
 )
 from .callback import CallbackObject
 from .active_voice_state import ActiveVoiceState
+from .auto_defer import AutoDefer  # purposely out of order to make sure auto_defer comes out as the deco
 from .application_commands import (
     application_commands_to_dict,
     auto_defer,
     CallbackType,
     component_callback,
     ComponentCommand,
     context_menu,
@@ -37,15 +38,14 @@
     SlashCommand,
     SlashCommandChoice,
     SlashCommandOption,
     SlashCommandParameter,
     subcommand,
     sync_needed,
 )
-from .auto_defer import AutoDefer
 from .checks import dm_only, guild_only, has_any_role, has_id, has_role, is_owner
 from .command import BaseCommand, check, cooldown, max_concurrency
 from .context import (
     AutocompleteContext,
     BaseContext,
     BaseInteractionContext,
     ComponentContext,
@@ -54,14 +54,15 @@
     ModalContext,
     Resolved,
     SlashContext,
 )
 from .converters import (
     BaseChannelConverter,
     ChannelConverter,
+    ConsumeRest,
     CustomEmojiConverter,
     DMChannelConverter,
     DMConverter,
     DMGroupConverter,
     Greedy,
     GuildCategoryConverter,
     GuildChannelConverter,
@@ -120,14 +121,15 @@
     "check",
     "component_callback",
     "ComponentCommand",
     "ComponentContext",
     "context_menu",
     "user_context_menu",
     "message_context_menu",
+    "ConsumeRest",
     "ContextMenu",
     "ContextMenuContext",
     "Converter",
     "cooldown",
     "Cooldown",
     "CooldownSystem",
     "SlidingWindowSystem",
```

### Comparing `discord-py-interactions-5.8.0/interactions/models/internal/active_voice_state.py` & `discord-py-interactions-5.9.0/interactions/models/internal/active_voice_state.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/internal/annotations/slash.py` & `discord-py-interactions-5.9.0/interactions/models/internal/annotations/slash.py`

 * *Files 19% similar despite different names*

```diff
@@ -28,241 +28,259 @@
     )
 
 
 def slash_str_option(
     description: str,
     required: bool = False,
     autocomplete: bool = False,
-    choices: List[Union["SlashCommandChoice", dict]] = None,
+    choices: List[Union["SlashCommandChoice", dict]] | None = None,
     min_length: Optional[int] = None,
     max_length: Optional[int] = None,
+    name: Optional[str] = None,
 ) -> Type[str]:
     """
     Annotates an argument as a string type slash command option.
 
     Args:
         description: The description of your option
         required: Is this option required?
         autocomplete: Use autocomplete for this option
         choices: The choices allowed by this command
         min_length: The minimum length of text a user can input.
         max_length: The maximum length of text a user can input.
+        name: The name of the option. Defaults to the name of the argument
 
     """
     return SlashCommandOption(
-        name="placeholder",
+        name=name,
         description=description,
         required=required,
         autocomplete=autocomplete,
         choices=choices or [],
         max_length=max_length,
         min_length=min_length,
         type=models.OptionType.STRING,
     )
 
 
 def slash_float_option(
     description: str,
     required: bool = False,
     autocomplete: bool = False,
-    choices: List[Union["SlashCommandChoice", dict]] = None,
+    choices: List[Union["SlashCommandChoice", dict]] | None = None,
     min_value: Optional[float] = None,
     max_value: Optional[float] = None,
+    name: Optional[str] = None,
 ) -> Type[float]:
     """
     Annotates an argument as a float type slash command option.
 
     Args:
         description: The description of your option
         required: Is this option required?
         autocomplete: Use autocomplete for this option
         choices: The choices allowed by this command
         min_value: The minimum number allowed
         max_value: The maximum number allowed
+        name: The name of the option. Defaults to the name of the argument
 
     """
     return SlashCommandOption(
-        name="placeholder",
+        name=name,
         description=description,
         required=required,
         autocomplete=autocomplete,
         choices=choices or [],
         max_value=max_value,
         min_value=min_value,
         type=models.OptionType.NUMBER,
     )
 
 
 def slash_int_option(
     description: str,
     required: bool = False,
     autocomplete: bool = False,
-    choices: List[Union["SlashCommandChoice", dict]] = None,
+    choices: List[Union["SlashCommandChoice", dict]] | None = None,
     min_value: Optional[float] = None,
     max_value: Optional[float] = None,
+    name: Optional[str] = None,
 ) -> Type[int]:
     """
     Annotates an argument as a integer type slash command option.
 
     Args:
         description: The description of your option
         required: Is this option required?
         autocomplete: Use autocomplete for this option
         choices: The choices allowed by this command
         min_value: The minimum number allowed
         max_value: The maximum number allowed
+        name: The name of the option. Defaults to the name of the argument
 
     """
     return SlashCommandOption(
-        name="placeholder",
+        name=name,
         description=description,
         required=required,
         autocomplete=autocomplete,
         choices=choices or [],
         max_value=max_value,
         min_value=min_value,
         type=models.OptionType.INTEGER,
     )
 
 
 def slash_bool_option(
     description: str,
     required: bool = False,
+    name: Optional[str] = None,
 ) -> Type[bool]:
     """
     Annotates an argument as a boolean type slash command option.
 
     Args:
         description: The description of your option
         required: Is this option required?
+        name: The name of the option. Defaults to the name of the argument
 
     """
     return SlashCommandOption(
-        name="placeholder",
+        name=name,
         description=description,
         required=required,
         type=models.OptionType.BOOLEAN,
     )
 
 
 def slash_user_option(
     description: str,
     required: bool = False,
     autocomplete: bool = False,
+    name: Optional[str] = None,
 ) -> Type[Union["User", "Member"]]:
     """
     Annotates an argument as a user type slash command option.
 
     Args:
         description: The description of your option
         required: Is this option required?
         autocomplete: Use autocomplete for this option
+        name: The name of the option. Defaults to the name of the argument
 
     """
     return SlashCommandOption(
-        name="placeholder",
+        name=name,
         description=description,
         required=required,
         autocomplete=autocomplete,
         type=models.OptionType.USER,
     )
 
 
 def slash_channel_option(
     description: str,
     required: bool = False,
     autocomplete: bool = False,
-    choices: List[Union["SlashCommandChoice", dict]] = None,
+    choices: List[Union["SlashCommandChoice", dict]] | None = None,
     channel_types: Optional[list[Union["ChannelType", int]]] = None,
+    name: Optional[str] = None,
 ) -> Type["BaseChannel"]:
     """
     Annotates an argument as a channel type slash command option.
 
     Args:
         description: The description of your option
         required: Is this option required?
         autocomplete: Use autocomplete for this option
         choices: The choices allowed by this command
         channel_types: The types of channel allowed by this option
+        name: The name of the option. Defaults to the name of the argument
 
     """
     return SlashCommandOption(
-        name="placeholder",
+        name=name,
         description=description,
         required=required,
         autocomplete=autocomplete,
         choices=choices or [],
         channel_types=channel_types,
         type=models.OptionType.CHANNEL,
     )
 
 
 def slash_role_option(
     description: str,
     required: bool = False,
     autocomplete: bool = False,
-    choices: List[Union["SlashCommandChoice", dict]] = None,
+    choices: List[Union["SlashCommandChoice", dict]] | None = None,
+    name: Optional[str] = None,
 ) -> Type["Role"]:
     """
     Annotates an argument as a role type slash command option.
 
     Args:
         description: The description of your option
         required: Is this option required?
         autocomplete: Use autocomplete for this option
         choices: The choices allowed by this command
+        name: The name of the option. Defaults to the name of the argument
 
     """
     return SlashCommandOption(
-        name="placeholder",
+        name=name,
         description=description,
         required=required,
         autocomplete=autocomplete,
         choices=choices or [],
         type=models.OptionType.ROLE,
     )
 
 
 def slash_mentionable_option(
     description: str,
     required: bool = False,
     autocomplete: bool = False,
-    choices: List[Union["SlashCommandChoice", dict]] = None,
+    choices: List[Union["SlashCommandChoice", dict]] | None = None,
+    name: Optional[str] = None,
 ) -> Type[Union["Role", "BaseChannel", "User", "Member"]]:
     """
     Annotates an argument as a mentionable type slash command option.
 
     Args:
         description: The description of your option
         required: Is this option required?
         autocomplete: Use autocomplete for this option
         choices: The choices allowed by this command
+        name: The name of the option. Defaults to the name of the argument
 
     """
     return SlashCommandOption(
-        name="placeholder",
+        name=name,
         description=description,
         required=required,
         autocomplete=autocomplete,
         choices=choices or [],
         type=models.OptionType.MENTIONABLE,
     )
 
 
 def slash_attachment_option(
     description: str,
     required: bool = False,
+    name: Optional[str] = None,
 ) -> Type["Attachment"]:
     """
     Annotates an argument as an attachment type slash command option.
 
     Args:
         description: The description of your option
         required: Is this option required?
+        name: The name of the option. Defaults to the name of the argument
 
     """
     return SlashCommandOption(
-        name="placeholder",
+        name=name,
         description=description,
         required=required,
         type=models.OptionType.ATTACHMENT,
     )
```

### Comparing `discord-py-interactions-5.8.0/interactions/models/internal/application_commands.py` & `discord-py-interactions-5.9.0/interactions/models/internal/application_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,15 +271,15 @@
 
         Returns:
             The markdown mention.
         """
         if scope:
             cmd_id = self.get_cmd_id(scope=scope)
         else:
-            cmd_id = list(self.cmd_id.values())[0]
+            cmd_id = next(iter(self.cmd_id.values()))
 
         return f"</{self.resolved_name}:{cmd_id}>"
 
     @property
     def resolved_name(self) -> str:
         """A representation of this interaction's name."""
         return str(self.name)
@@ -396,14 +396,15 @@
         required: "This option must be filled to use the command"
         choices: A list of choices the user has to pick between
         channel_types: The channel types permitted. The option needs to be a channel
         min_value: The minimum value permitted. The option needs to be an integer or float
         max_value: The maximum value permitted. The option needs to be an integer or float
         min_length: The minimum length of text a user can input. The option needs to be a string
         max_length: The maximum length of text a user can input. The option needs to be a string
+        argument_name: The name of the argument to be used in the function. If not given, assumed to be the same as the name of the option
 
     """
 
     name: LocalisedName | str = attrs.field(repr=False, converter=LocalisedName.converter)
     type: Union[OptionType, int] = attrs.field(
         repr=False,
     )
@@ -414,14 +415,15 @@
     autocomplete: bool = attrs.field(repr=False, default=False)
     choices: List[Union[SlashCommandChoice, Dict]] = attrs.field(repr=False, factory=list)
     channel_types: Optional[list[Union[ChannelType, int]]] = attrs.field(repr=False, default=None)
     min_value: Optional[float] = attrs.field(repr=False, default=None)
     max_value: Optional[float] = attrs.field(repr=False, default=None)
     min_length: Optional[int] = attrs.field(repr=False, default=None)
     max_length: Optional[int] = attrs.field(repr=False, default=None)
+    argument_name: Optional[str] = attrs.field(repr=False, default=None)
 
     @type.validator
     def _type_validator(self, attribute: str, value: int) -> None:
         if value in (OptionType.SUB_COMMAND, OptionType.SUB_COMMAND_GROUP):
             raise ValueError(
                 "Options cannot be SUB_COMMAND or SUB_COMMAND_GROUP. If you want to use subcommands, "
                 "see the @sub_command() decorator."
@@ -484,14 +486,15 @@
                 raise ValueError("`min_length` needs to be <= than `max_length`")
 
             if self.max_length < 1:
                 raise ValueError("`max_length` needs to be >= 1")
 
     def as_dict(self) -> dict:
         data = attrs.asdict(self)
+        data.pop("argument_name", None)
         data["name"] = str(self.name)
         data["description"] = str(self.description)
         data["choices"] = [
             choice.as_dict() if isinstance(choice, SlashCommandChoice) else choice for choice in self.choices
         ]
         data["name_localizations"] = self.name.to_locale_dict()
         data["description_localizations"] = self.description.to_locale_dict()
@@ -502,14 +505,19 @@
 @attrs.define()
 class SlashCommandParameter:
     name: str = attrs.field()
     type: typing.Any = attrs.field()
     kind: inspect._ParameterKind = attrs.field()
     default: typing.Any = attrs.field(default=MISSING)
     converter: typing.Optional[typing.Callable] = attrs.field(default=None)
+    _option_name: typing.Optional[str] = attrs.field(default=None)
+
+    @property
+    def option_name(self) -> str:
+        return self._option_name or self.name
 
 
 def _get_option_from_annotated(annotated: Annotated) -> SlashCommandOption | None:
     args = typing.get_args(annotated)
     return next((a for a in args if isinstance(a, SlashCommandOption)), None)
 
 
@@ -597,18 +605,22 @@
 
         super().__attrs_post_init__()
 
     def _add_option_from_anno_method(self, name: str, option: SlashCommandOption) -> None:
         if not self.options:
             self.options = []
 
-        option.name = name
+        if option.name is None:
+            option.name = name
+        else:
+            option.argument_name = name
+
         self.options.append(option)
 
-    def _parse_parameters(self) -> None:
+    def _parse_parameters(self) -> None:  # noqa: C901
         """
         Parses the parameters that this command has into a form i.py can use.
 
         This is purposely separated like this to allow "lazy parsing" - parsing
         as the command is added to a bot rather than being parsed immediately.
         This allows variables like "self" to be filtered out, and is useful for
         potential future additions.
@@ -661,14 +673,28 @@
                     converter = _get_converter_from_annotated(anno)
 
                 if converter:
                     our_param.converter = self._get_converter_function(converter, our_param.name)
 
             self.parameters[param.name] = our_param
 
+        if self.options:
+            for option in self.options:
+                maybe_argument_name = (
+                    option.argument_name if isinstance(option, SlashCommandOption) else option.get("argument_name")
+                )
+                if maybe_argument_name:
+                    name = option.name if isinstance(option, SlashCommandOption) else option["name"]
+                    try:
+                        self.parameters[maybe_argument_name]._option_name = str(name)
+                    except KeyError:
+                        raise ValueError(
+                            f'Argument name "{maybe_argument_name}" for "{name}" does not match any parameter in {self.resolved_name}\'s function.'
+                        ) from None
+
     def to_dict(self) -> dict:
         data = super().to_dict()
 
         if self.is_subcommand:
             data["name"] = str(self.sub_cmd_name)
             data["description"] = str(self.sub_cmd_description)
             data["name_localizations"] = self.sub_cmd_name.to_locale_dict()
@@ -713,15 +739,15 @@
 
             return call
 
         option_name = option_name.lower()
         return wrapper
 
     def group(
-        self, name: str = None, description: str = "No Description Set", inherit_checks: bool = True
+        self, name: str | None = None, description: str = "No Description Set", inherit_checks: bool = True
     ) -> "SlashCommand":
         return SlashCommand(
             name=self.name,
             description=self.description,
             group_name=name,
             group_description=description,
             scopes=self.scopes,
@@ -732,15 +758,15 @@
 
     def subcommand(
         self,
         sub_cmd_name: Absent[LocalisedName | str] = MISSING,
         group_name: LocalisedName | str = None,
         sub_cmd_description: Absent[LocalisedDesc | str] = MISSING,
         group_description: Absent[LocalisedDesc | str] = MISSING,
-        options: List[Union[SlashCommandOption, Dict]] = None,
+        options: List[Union[SlashCommandOption, Dict]] | None = None,
         nsfw: bool = False,
         inherit_checks: bool = True,
     ) -> Callable[..., "SlashCommand"]:
         def wrapper(call: Callable[..., Coroutine]) -> "SlashCommand":
             nonlocal sub_cmd_name, sub_cmd_description
 
             if not asyncio.iscoroutinefunction(call):
@@ -776,26 +802,26 @@
             return await self.call_with_binding(callback, ctx)
 
         kwargs_copy = ctx.kwargs.copy()
 
         new_args = []
         new_kwargs = {}
 
-        for name, param in self.parameters.items():
-            value = kwargs_copy.pop(name, MISSING)
+        for param in self.parameters.values():
+            value = kwargs_copy.pop(param.option_name, MISSING)
             if value is MISSING:
                 continue
 
             if converter := param.converter:
                 value = await maybe_coroutine(converter, ctx, value)
 
             if param.kind == inspect.Parameter.POSITIONAL_ONLY:
                 new_args.append(value)
             else:
-                new_kwargs[name] = value
+                new_kwargs[param.name] = value
 
         # i do want to address one thing: what happens if you have both *args and **kwargs
         # in your argument?
         # i would say passing in values for both makes sense... but they're very likely
         # going to overlap and cause issues and confusion
         # for the sake of simplicty, i.py assumes kwargs takes priority over args
         if kwargs_copy:
@@ -957,16 +983,16 @@
     description: Absent[str | LocalisedDesc] = MISSING,
     base_description: Optional[str | LocalisedDesc] = None,
     base_desc: Optional[str | LocalisedDesc] = None,
     base_default_member_permissions: Optional["Permissions"] = None,
     base_dm_permission: bool = True,
     subcommand_group_description: Optional[str | LocalisedDesc] = None,
     sub_group_desc: Optional[str | LocalisedDesc] = None,
-    scopes: List["Snowflake_Type"] = None,
-    options: List[dict] = None,
+    scopes: List["Snowflake_Type"] | None = None,
+    options: List[dict] | None = None,
     nsfw: bool = False,
 ) -> Callable[[AsyncCallable], SlashCommand]:
     """
     A decorator specifically tailored for creating subcommands.
 
     Args:
         base: The name of the base command
@@ -1132,22 +1158,26 @@
     """
     Register a coroutine as a component callback.
 
     Component callbacks work the same way as commands, just using components as a way of invoking, instead of messages.
     Your callback will be given a single argument, `ComponentContext`
 
     Note:
-        This can optionally take a regex pattern, which will be used to match against the custom ID of the component
+        This can optionally take a regex pattern, which will be used to match against the custom ID of the component.
+
+        If you do not supply a `custom_id`, the name of the coroutine will be used instead.
 
     Args:
         *custom_id: The custom ID of the component to wait for
 
     """
 
     def wrapper(func: AsyncCallable) -> ComponentCommand:
+        custom_id = custom_id or [func.__name__]  # noqa: F823
+
         if not asyncio.iscoroutinefunction(func):
             raise ValueError("Commands must be coroutines")
 
         return ComponentCommand(name=f"ComponentCallback::{custom_id}", callback=func, listeners=custom_id)
 
     custom_id = _unpack_helper(custom_id)
     custom_ids_validator(*custom_id)
@@ -1158,22 +1188,26 @@
     """
     Register a coroutine as a modal callback.
 
     Modal callbacks work the same way as commands, just using modals as a way of invoking, instead of messages.
     Your callback will be given a single argument, `ModalContext`
 
     Note:
-        This can optionally take a regex pattern, which will be used to match against the custom ID of the modal
+        This can optionally take a regex pattern, which will be used to match against the custom ID of the modal.
+
+        If you do not supply a `custom_id`, the name of the coroutine will be used instead.
 
 
     Args:
         *custom_id: The custom ID of the modal to wait for
     """
 
     def wrapper(func: AsyncCallable) -> ModalCommand:
+        custom_id = custom_id or [func.__name__]  # noqa: F823
+
         if not asyncio.iscoroutinefunction(func):
             raise ValueError("Commands must be coroutines")
 
         return ModalCommand(name=f"ModalCallback::{custom_id}", callback=func, listeners=custom_id)
 
     custom_id = _unpack_helper(custom_id)
     custom_ids_validator(*custom_id)
@@ -1186,20 +1220,21 @@
 
 def slash_option(
     name: str,
     description: str,
     opt_type: Union[OptionType, int],
     required: bool = False,
     autocomplete: bool = False,
-    choices: List[Union[SlashCommandChoice, dict]] = None,
+    choices: List[Union[SlashCommandChoice, dict]] | None = None,
     channel_types: Optional[list[Union[ChannelType, int]]] = None,
     min_value: Optional[float] = None,
     max_value: Optional[float] = None,
     min_length: Optional[int] = None,
     max_length: Optional[int] = None,
+    argument_name: Optional[str] = None,
 ) -> Callable[[SlashCommandT], SlashCommandT]:
     r"""
     A decorator to add an option to a slash command.
 
     Args:
         name: 1-32 lowercase character name matching ^[\w-]{1,32}$
         opt_type: The type of option
@@ -1208,14 +1243,15 @@
         autocomplete: If autocomplete interactions are enabled for this STRING, INTEGER, or NUMBER type option
         choices: A list of choices the user has to pick between (max 25)
         channel_types: The channel types permitted. The option needs to be a channel
         min_value: The minimum value permitted. The option needs to be an integer or float
         max_value: The maximum value permitted. The option needs to be an integer or float
         min_length: The minimum length of text a user can input. The option needs to be a string
         max_length: The maximum length of text a user can input. The option needs to be a string
+        argument_name: The name of the argument to be used in the function. If not given, assumed to be the same as the name of the option
     """
 
     def wrapper(func: SlashCommandT) -> SlashCommandT:
         if hasattr(func, "cmd_id"):
             raise ValueError("slash_option decorators must be positioned under a slash_command decorator")
 
         option = SlashCommandOption(
@@ -1226,14 +1262,15 @@
             autocomplete=autocomplete,
             choices=choices or [],
             channel_types=channel_types,
             min_value=min_value,
             max_value=max_value,
             min_length=min_length,
             max_length=max_length,
+            argument_name=argument_name,
         )
         if not hasattr(func, "options"):
             func.options = []
         func.options.insert(0, option)
         return func
 
     return wrapper
```

### Comparing `discord-py-interactions-5.8.0/interactions/models/internal/auto_defer.py` & `discord-py-interactions-5.9.0/interactions/models/internal/auto_defer.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/internal/callback.py` & `discord-py-interactions-5.9.0/interactions/models/internal/callback.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/internal/checks.py` & `discord-py-interactions-5.9.0/interactions/models/internal/checks.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/internal/command.py` & `discord-py-interactions-5.9.0/interactions/models/internal/command.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/internal/context.py` & `discord-py-interactions-5.9.0/interactions/models/internal/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,14 +280,17 @@
         instance.permission_map = {client.app.id: Permissions(payload.get("app_permissions", 0))}
         instance.locale = payload["locale"]
         instance.guild_locale = payload.get("guild_locale", instance.locale)
         instance._context_type = payload.get("type", 0)
         instance.resolved = Resolved.from_dict(client, payload["data"].get("resolved", {}), payload.get("guild_id"))
 
         instance.channel_id = Snowflake(payload["channel_id"])
+        if channel := payload.get("channel"):
+            client.cache.place_channel_data(channel)
+
         if member := payload.get("member"):
             instance.author_id = Snowflake(member["user"]["id"])
             instance.guild_id = Snowflake(payload["guild_id"])
             client.cache.place_member_data(instance.guild_id, member)
         else:
             instance.author_id = Snowflake(payload["user"]["id"])
             client.cache.place_user_data(payload["user"])
@@ -540,26 +543,28 @@
             delete_after=delete_after,
             pass_self_into_delete=True,
             **kwargs,
         )
 
     respond = send
 
-    async def delete(self, message: "Snowflake_Type") -> None:
+    async def delete(self, message: "Snowflake_Type" = "@original") -> None:
         """
         Delete a message sent in response to this interaction.
 
         Args:
-            message: The message to delete
+            message: The message to delete. Defaults to @original which represents the initial response message.
         """
-        await self.client.http.delete_interaction_message(self.client.app.id, self.token, to_snowflake(message))
+        await self.client.http.delete_interaction_message(
+            self.client.app.id, self.token, to_snowflake(message) if message != "@original" else message
+        )
 
     async def edit(
         self,
-        message: "Snowflake_Type",
+        message: "Snowflake_Type" = "@original",
         *,
         content: typing.Optional[str] = None,
         embeds: typing.Optional[
             typing.Union[typing.Iterable[typing.Union["Embed", dict]], typing.Union["Embed", dict]]
         ] = None,
         embed: typing.Optional[typing.Union["Embed", dict]] = None,
         components: typing.Optional[
@@ -587,15 +592,15 @@
 
         if file:
             files = [file, *files] if files else [file]
         message_data = await self.client.http.edit_interaction_message(
             payload=message_payload,
             application_id=self.client.app.id,
             token=self.token,
-            message_id=to_snowflake(message),
+            message_id=to_snowflake(message) if message != "@original" else message,
             files=files,
         )
         if message_data:
             return self.client.cache.place_message_data(message_data)
 
 
 class SlashContext(InteractionContext, ModalMixin):
```

### Comparing `discord-py-interactions-5.8.0/interactions/models/internal/converters.py` & `discord-py-interactions-5.9.0/interactions/models/internal/converters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 import typing
-from typing import Any, Optional, List
+from typing import Any, Optional, List, Annotated
 
-from interactions.client.const import T, T_co
+from interactions.client.const import T, T_co, Sentinel
 from interactions.client.errors import BadArgument
 from interactions.client.errors import Forbidden, HTTPException
 from interactions.models.discord.channel import (
     BaseChannel,
     DMChannel,
     DM,
     DMGroup,
@@ -62,14 +62,15 @@
     "MessageableChannelConverter",
     "RoleConverter",
     "GuildConverter",
     "PartialEmojiConverter",
     "CustomEmojiConverter",
     "MessageConverter",
     "Greedy",
+    "ConsumeRest",
     "MODEL_TO_CONVERTER",
 )
 
 
 class NoArgumentConverter(Converter[T_co]):
     """
     An indicator class for special type of converters that only uses the Context.
@@ -568,14 +569,23 @@
         return result
 
 
 class Greedy(List[T]):
     """A special marker class to mark an argument in a prefixed command to repeatedly convert until it fails to convert an argument."""
 
 
+class ConsumeRestMarker(Sentinel):
+    pass
+
+
+CONSUME_REST_MARKER = ConsumeRestMarker()
+
+ConsumeRest = Annotated[T, CONSUME_REST_MARKER]
+"""A special marker type alias to mark an argument in a prefixed command to consume the rest of the arguments."""
+
 MODEL_TO_CONVERTER: dict[type, type[Converter]] = {
     SnowflakeObject: SnowflakeConverter,
     BaseChannel: BaseChannelConverter,
     DMChannel: DMChannelConverter,
     DM: DMConverter,
     DMGroup: DMGroupConverter,
     GuildChannel: GuildChannelConverter,
```

### Comparing `discord-py-interactions-5.8.0/interactions/models/internal/cooldowns.py` & `discord-py-interactions-5.9.0/interactions/models/internal/cooldowns.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/internal/extension.py` & `discord-py-interactions-5.9.0/interactions/models/internal/extension.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/internal/listener.py` & `discord-py-interactions-5.9.0/interactions/models/internal/listener.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
             # discard the first parameter, which is the class instance
             self._params = list(self._params.values())[1:]
 
         self.pass_event_object = len(self._params) != 0
 
 
 def listen(
-    event_name: Absent[str | BaseEvent] = MISSING,
+    event_name: Absent[str | type[BaseEvent]] = MISSING,
     *,
     delay_until_ready: bool = False,
     is_default_listener: bool = False,
     disable_default_listeners: bool = False,
 ) -> Callable[[AsyncCallable], Listener]:
     """
     Decorator to make a function an event listener.
```

### Comparing `discord-py-interactions-5.8.0/interactions/models/internal/localisation.py` & `discord-py-interactions-5.9.0/interactions/models/internal/localisation.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/internal/protocols.py` & `discord-py-interactions-5.9.0/interactions/models/internal/protocols.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/internal/tasks/task.py` & `discord-py-interactions-5.9.0/interactions/models/internal/tasks/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,68 +71,68 @@
         """A dummy method for interactions.ext.sentry to hook"""
 
     def on_error(self, error: Exception) -> None:
         """Error handler for this task. Called when an exception is raised during execution of the task."""
         self.on_error_sentry_hook(error)
         interactions.Client.default_error_handler("Task", error)
 
-    async def __call__(self) -> None:
+    async def __call__(self, *args, **kwargs) -> None:
         try:
             if inspect.iscoroutinefunction(self.callback):
-                val = await self.callback()
+                val = await self.callback(*args, **kwargs)
             else:
-                val = self.callback()
+                val = self.callback(*args, **kwargs)
 
             if isinstance(val, BaseTrigger):
                 self.reschedule(val)
         except Exception as e:
             self.on_error(e)
 
-    def _fire(self, fire_time: datetime) -> None:
+    def _fire(self, fire_time: datetime, *args, **kwargs) -> None:
         """Called when the task is being fired."""
         self.trigger.set_last_call_time(fire_time)
-        _ = asyncio.create_task(self())
+        _ = asyncio.create_task(self(*args, **kwargs))
         self.iteration += 1
 
-    async def _task_loop(self) -> None:
+    async def _task_loop(self, *args, **kwargs) -> None:
         """The main task loop to fire the task at the specified time based on triggers configured."""
         while not self._stop.is_set():
             fire_time = self.trigger.next_fire()
             if fire_time is None:
                 return self.stop()
 
             future = asyncio.create_task(self._stop.wait())
             timeout = (fire_time - datetime.now()).total_seconds()
             done, _ = await asyncio.wait([future], timeout=timeout, return_when=asyncio.FIRST_COMPLETED)
             if future in done:
                 return None
 
-            self._fire(fire_time)
+            self._fire(fire_time, *args, **kwargs)
 
-    def start(self) -> None:
+    def start(self, *args, **kwargs) -> None:
         """Start this task."""
         try:
             self.trigger.reschedule()
             self._stop.clear()
-            self.task = asyncio.create_task(self._task_loop())
+            self.task = asyncio.create_task(self._task_loop(*args, **kwargs))
         except RuntimeError:
             get_logger().error(
                 "Unable to start task without a running event loop! We recommend starting tasks within an `on_startup` event."
             )
 
     def stop(self) -> None:
         """End this task."""
         self._stop.set()
         if self.task:
             self.task.cancel()
 
-    def restart(self) -> None:
+    def restart(self, *args, **kwargs) -> None:
         """Restart this task."""
         self.stop()
-        self.start()
+        self.start(*args, **kwargs)
 
     def reschedule(self, trigger: BaseTrigger) -> None:
         """
         Change the trigger being used by this task.
 
         Args:
             trigger: The new Trigger to use
```

### Comparing `discord-py-interactions-5.8.0/interactions/models/internal/tasks/triggers.py` & `discord-py-interactions-5.9.0/interactions/models/internal/tasks/triggers.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/internal/wait.py` & `discord-py-interactions-5.9.0/interactions/models/internal/wait.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/misc/context_manager.py` & `discord-py-interactions-5.9.0/interactions/models/misc/context_manager.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/interactions/models/misc/iterator.py` & `discord-py-interactions-5.9.0/interactions/models/misc/iterator.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/pyproject.toml` & `discord-py-interactions-5.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "interactions.py"
-version = "5.8.0"
+version = "5.9.0"
 description = "Easy, simple, scalable and modular: a Python API wrapper for interactions."
 authors = [
     "LordOfPolls <dev@lordofpolls.com>",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
```

### Comparing `discord-py-interactions-5.8.0/setup.py` & `discord-py-interactions-5.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/tests/consts.py` & `discord-py-interactions-5.9.0/tests/consts.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/tests/test_bot.py` & `discord-py-interactions-5.9.0/tests/test_bot.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/tests/test_cache.py` & `discord-py-interactions-5.9.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/tests/test_contexts.py` & `discord-py-interactions-5.9.0/tests/test_contexts.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/tests/test_cooldowns.py` & `discord-py-interactions-5.9.0/tests/test_cooldowns.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/tests/test_emoji.py` & `discord-py-interactions-5.9.0/tests/test_emoji.py`

 * *Files identical despite different names*

### Comparing `discord-py-interactions-5.8.0/tests/utils.py` & `discord-py-interactions-5.9.0/tests/utils.py`

 * *Files identical despite different names*

