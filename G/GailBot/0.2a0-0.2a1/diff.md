# Comparing `tmp/GailBot-0.2a0.tar.gz` & `tmp/GailBot-0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GailBot-0.2a0.tar", last modified: Mon Aug  7 17:10:49 2023, max compression
+gzip compressed data, was "GailBot-0.2a1.tar", last modified: Mon Aug  7 17:13:44 2023, max compression
```

## Comparing `GailBot-0.2a0.tar` & `GailBot-0.2a1.tar`

### file list

```diff
@@ -1,285 +1,285 @@
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.864391 GailBot-0.2a0/
--rw-r--r--   0 jasonycwu   (501) staff       (20)     1066 2023-08-07 03:38:06.000000 GailBot-0.2a0/LICENSE
--rw-r--r--   0 jasonycwu   (501) staff       (20)       49 2023-08-07 03:38:06.000000 GailBot-0.2a0/MANIFEST.in
--rw-r--r--   0 jasonycwu   (501) staff       (20)    10630 2023-08-07 17:10:49.863930 GailBot-0.2a0/PKG-INFO
--rw-r--r--   0 jasonycwu   (501) staff       (20)     8546 2023-08-07 03:48:15.000000 GailBot-0.2a0/README.md
--rw-r--r--   0 jasonycwu   (501) staff       (20)     1412 2023-08-07 17:07:14.000000 GailBot-0.2a0/pyproject.toml
--rw-r--r--   0 jasonycwu   (501) staff       (20)     5014 2023-08-07 03:38:06.000000 GailBot-0.2a0/requirements.txt
--rw-r--r--   0 jasonycwu   (501) staff       (20)       38 2023-08-07 17:10:49.864447 GailBot-0.2a0/setup.cfg
--rw-r--r--   0 jasonycwu   (501) staff       (20)      251 2023-08-07 03:38:06.000000 GailBot-0.2a0/setup.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.813331 GailBot-0.2a0/src/
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.820170 GailBot-0.2a0/src/.idea/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      176 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/.idea/.gitignore
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.820621 GailBot-0.2a0/src/.idea/inspectionProfiles/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      574 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 jasonycwu   (501) staff       (20)      174 2023-08-07 02:22:24.000000 GailBot-0.2a0/src/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 jasonycwu   (501) staff       (20)      181 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/.idea/misc.xml
--rw-r--r--   0 jasonycwu   (501) staff       (20)      258 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/.idea/modules.xml
--rw-r--r--   0 jasonycwu   (501) staff       (20)      226 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/.idea/src.iml
--rw-r--r--   0 jasonycwu   (501) staff       (20)      183 2023-08-07 02:22:24.000000 GailBot-0.2a0/src/.idea/vcs.xml
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.821393 GailBot-0.2a0/src/GailBot.egg-info/
--rw-r--r--   0 jasonycwu   (501) staff       (20)    10630 2023-08-07 17:10:49.000000 GailBot-0.2a0/src/GailBot.egg-info/PKG-INFO
--rw-r--r--   0 jasonycwu   (501) staff       (20)     9006 2023-08-07 17:10:49.000000 GailBot-0.2a0/src/GailBot.egg-info/SOURCES.txt
--rw-r--r--   0 jasonycwu   (501) staff       (20)        1 2023-08-07 17:10:49.000000 GailBot-0.2a0/src/GailBot.egg-info/dependency_links.txt
--rw-r--r--   0 jasonycwu   (501) staff       (20)     5075 2023-08-07 17:10:49.000000 GailBot-0.2a0/src/GailBot.egg-info/requires.txt
--rw-r--r--   0 jasonycwu   (501) staff       (20)       23 2023-08-07 17:10:49.000000 GailBot-0.2a0/src/GailBot.egg-info/top_level.txt
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.821672 GailBot-0.2a0/src/config_backend/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      230 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/config_backend/__init__.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.812947 GailBot-0.2a0/src/config_backend/engines/
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.821830 GailBot-0.2a0/src/config_backend/engines/google/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      549 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/config_backend/engines/google/google_config.toml
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.821999 GailBot-0.2a0/src/config_backend/engines/watson/
--rw-r--r--   0 jasonycwu   (501) staff       (20)     2196 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/config_backend/engines/watson/watson_config.toml
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.822169 GailBot-0.2a0/src/config_backend/engines/whisper/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      929 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/config_backend/engines/whisper/whisper_config.toml
--rw-r--r--   0 jasonycwu   (501) staff       (20)      546 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/config_backend/paths.toml
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.822409 GailBot-0.2a0/src/config_backend/plugin/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      142 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/config_backend/plugin/valid_plugin.toml
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.823342 GailBot-0.2a0/src/config_backend/services/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      407 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/config_backend/services/default_setting.toml
--rw-r--r--   0 jasonycwu   (501) staff       (20)     1119 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/config_backend/services/format.md
--rw-r--r--   0 jasonycwu   (501) staff       (20)      448 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/config_backend/services/service.toml
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.823670 GailBot-0.2a0/src/config_backend/settings/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      272 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/config_backend/settings/default.toml
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.824086 GailBot-0.2a0/src/config_backend/toplevel/
--rw-r--r--   0 jasonycwu   (501) staff       (20)     1040 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/config_backend/toplevel/ws_config.toml
--rw-r--r--   0 jasonycwu   (501) staff       (20)       40 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/config_backend/toplevel/ws_root.toml
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.824265 GailBot-0.2a0/src/config_backend/util/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      163 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/config_backend/util/log.toml
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.824643 GailBot-0.2a0/src/gailbot/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      380 2023-08-07 17:09:46.000000 GailBot-0.2a0/src/gailbot/__init__.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)    22765 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/api.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.824930 GailBot-0.2a0/src/gailbot/configs/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      459 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/configs/__init__.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.825420 GailBot-0.2a0/src/gailbot/configs/confs/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      162 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/configs/confs/__init__.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     1163 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/configs/confs/paths.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.825661 GailBot-0.2a0/src/gailbot/configs/interfaces/
--rw-r--r--   0 jasonycwu   (501) staff       (20)     1767 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/configs/interfaces/__init__.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.825828 GailBot-0.2a0/src/gailbot/configs/interfaces/config/
--rw-r--r--   0 jasonycwu   (501) staff       (20)     4839 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/configs/interfaces/config/ws_config.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.813833 GailBot-0.2a0/src/gailbot/configs/interfaces/core/
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.826329 GailBot-0.2a0/src/gailbot/configs/interfaces/core/engines/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      834 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/configs/interfaces/core/engines/google.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)      889 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/configs/interfaces/core/engines/watson.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     2111 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/configs/interfaces/core/engines/whisper.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.826488 GailBot-0.2a0/src/gailbot/configs/interfaces/core/setting/
--rw-r--r--   0 jasonycwu   (501) staff       (20)     1030 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/configs/interfaces/core/setting/defaults.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.826657 GailBot-0.2a0/src/gailbot/configs/interfaces/core/util/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      540 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/configs/interfaces/core/util/logger.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.827175 GailBot-0.2a0/src/gailbot/configs/interfaces/plugin/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      244 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/configs/interfaces/plugin/__init__.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     1061 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/configs/interfaces/plugin/pluginsuite.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)      229 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/configs/interfaces/plugin/validstructure.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.827657 GailBot-0.2a0/src/gailbot/configs/interfaces/services/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      220 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/configs/interfaces/services/__init__.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     1921 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/configs/interfaces/services/service.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.827806 GailBot-0.2a0/src/gailbot/core/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      156 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/__init__.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.828565 GailBot-0.2a0/src/gailbot/core/engines/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      363 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/__init__.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     1560 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/engine.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)      976 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/engineManager.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     2361 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/exception.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.829041 GailBot-0.2a0/src/gailbot/core/engines/google/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      184 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/google/__init__.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)    12266 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/google/core.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     2578 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/google/google.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.830613 GailBot-0.2a0/src/gailbot/core/engines/watson/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      260 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/watson/__init__.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)    11756 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/watson/am.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)      367 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/watson/codes.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)    12605 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/watson/core.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)    16999 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/watson/lm.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)    13203 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/watson/recognition_results.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     5085 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/watson/recognize_callback.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     4907 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/watson/watson.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.831198 GailBot-0.2a0/src/gailbot/core/engines/whisperEngine/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      203 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/whisperEngine/__init__.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     5643 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/whisperEngine/core.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.831460 GailBot-0.2a0/src/gailbot/core/engines/whisperEngine/diarization/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      199 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/whisperEngine/diarization/__init__.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     3460 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/whisperEngine/diarization/utils.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     2846 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/whisperEngine/parsers.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     2100 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/whisperEngine/whisperEngine.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.831753 GailBot-0.2a0/src/gailbot/core/engines/whisperX/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      156 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/whisperX/__init__.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     2960 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/engines/whisperX/whisperX.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.832192 GailBot-0.2a0/src/gailbot/core/pipeline/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      259 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/pipeline/__init__.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     1046 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/pipeline/component.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)    10631 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/pipeline/pipeline.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.833427 GailBot-0.2a0/src/gailbot/core/utils/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      163 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/utils/__init__.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     2630 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/utils/download.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)    14143 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/utils/general.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     1535 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/utils/logger.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)    27791 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/utils/media.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)    14816 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/core/utils/threads.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.834036 GailBot-0.2a0/src/gailbot/plugins/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      264 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/plugins/__init__.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.834658 GailBot-0.2a0/src/gailbot/plugins/loader/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      303 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/plugins/loader/__init__.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     9172 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/plugins/loader/directoryloader.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)      824 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/plugins/loader/pluginLoader.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)    10696 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/plugins/loader/urlloader.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)    10435 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/plugins/manager.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     1364 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/plugins/plugin.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     7744 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/plugins/suite.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.834959 GailBot-0.2a0/src/gailbot/services/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      267 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/__init__.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)    23896 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/controller.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.835480 GailBot-0.2a0/src/gailbot/services/converter/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      334 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/converter/__init__.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     2740 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/converter/converter.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.836464 GailBot-0.2a0/src/gailbot/services/converter/payload/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      458 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/converter/payload/__init__.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     3184 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/converter/payload/audioPayload.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     3745 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/converter/payload/conversationDirectoryPayload.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)    13064 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/converter/payload/payloadObject.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     3926 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/converter/payload/transcribedDirPayload.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     2224 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/converter/payload/videoPayload.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.836756 GailBot-0.2a0/src/gailbot/services/converter/plugin/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      237 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/converter/plugin/__init__.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     5744 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/converter/plugin/pluginMethod.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.837699 GailBot-0.2a0/src/gailbot/services/converter/result/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      398 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/converter/result/__init__.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     1406 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/converter/result/analysis.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     1673 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/converter/result/format.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)      479 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/converter/result/processingStatus.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     1936 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/converter/result/resultInterface.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     5590 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/converter/result/transcribe.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.838022 GailBot-0.2a0/src/gailbot/services/organizer/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      368 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/__init__.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)    18452 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/organizer.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.838468 GailBot-0.2a0/src/gailbot/services/organizer/settings/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      261 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/settings/__init__.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.839770 GailBot-0.2a0/src/gailbot/services/organizer/settings/interface/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      425 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/settings/interface/__init__.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)      665 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/settings/interface/engineSettingInterface.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     2853 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/settings/interface/googleInterface.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)      480 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/settings/interface/pluginSettingsInterface.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     2681 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/settings/interface/watsonInterface.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     2172 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/settings/interface/whisperInterface.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     2105 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/settings/interface/whisperXInterface.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.840352 GailBot-0.2a0/src/gailbot/services/organizer/settings/objects/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      293 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/settings/objects/__init__.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     4067 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/settings/objects/engineObject.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)      339 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/settings/objects/pluginObject.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     3539 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/settings/objects/settingObject.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)    19968 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/settings/settingManager.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.840846 GailBot-0.2a0/src/gailbot/services/organizer/source/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      238 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/source/__init__.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     8415 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/source/source_manager.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     3330 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/organizer/source/source_object.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.841161 GailBot-0.2a0/src/gailbot/services/pipeline/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      275 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/pipeline/__init__.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.841983 GailBot-0.2a0/src/gailbot/services/pipeline/components/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      146 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/pipeline/components/__init__.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     6078 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/pipeline/components/analysisComponent.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     2150 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/pipeline/components/formatComponent.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)      506 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/pipeline/components/progress.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)    10230 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/pipeline/components/transcribeComponent.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     1949 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/services/pipeline/pipeline.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.842704 GailBot-0.2a0/src/gailbot/workspace/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      275 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/workspace/__init__.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     5567 2023-08-07 03:38:06.000000 GailBot-0.2a0/src/gailbot/workspace/manager.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.844093 GailBot-0.2a0/tests/
--rw-r--r--   0 jasonycwu   (501) staff       (20)     1602 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/README
--rw-r--r--   0 jasonycwu   (501) staff       (20)     5448 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/UPDATELOG
--rw-r--r--   0 jasonycwu   (501) staff       (20)      172 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/__init__.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.844730 GailBot-0.2a0/tests/configs/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      156 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/configs/__init__.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)        0 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/configs/configs_test_configs.toml
--rw-r--r--   0 jasonycwu   (501) staff       (20)     1301 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/configs/test_config.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.844920 GailBot-0.2a0/tests/core/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      156 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/core/__init__.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.846176 GailBot-0.2a0/tests/core/engines/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      156 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/core/engines/__init__.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     2493 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/core/engines/data.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     5456 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/core/engines/test_google_engine.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     1562 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/core/engines/test_watson_am.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     6491 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/core/engines/test_watson_core.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     2787 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/core/engines/test_watson_lm.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     5372 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/core/engines/test_whisper.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     1168 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/core/engines/test_whisperx.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.846554 GailBot-0.2a0/tests/core/pipeline/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      156 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/core/pipeline/__init__.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     4398 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/core/pipeline/test_pipeline.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.847409 GailBot-0.2a0/tests/core/utils/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      156 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/core/utils/__init__.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)       72 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/core/utils/test.csv
--rw-r--r--   0 jasonycwu   (501) staff       (20)    14074 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/core/utils/test_general.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     8668 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/core/utils/test_media.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     9413 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/core/utils/test_thread.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.848447 GailBot-0.2a0/tests/plugins/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      237 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/plugins/__init__.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)      484 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/plugins/plugin_data.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     5731 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/plugins/plugin_data_old.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     6026 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/plugins/test_plugin.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     6072 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/plugins/test_plugins_old.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.849948 GailBot-0.2a0/tests/small-test/
--rw-r--r--   0 jasonycwu   (501) staff       (20)     2371 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/gailbot_key.json
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.852379 GailBot-0.2a0/tests/small-test/hello-dir/
--rw-r--r--   0 jasonycwu   (501) staff       (20)   135260 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/hello-dir/hello1.wav
--rw-r--r--   0 jasonycwu   (501) staff       (20)   135260 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/hello-dir/hello2.wav
--rw-r--r--   0 jasonycwu   (501) staff       (20)   135260 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/hello-dir/hello3.wav
--rw-r--r--   0 jasonycwu   (501) staff       (20)   135260 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/hello-dir/hello4.wav
--rw-r--r--   0 jasonycwu   (501) staff       (20)   135260 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/hello1.wav
--rw-r--r--   0 jasonycwu   (501) staff       (20)   135260 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/hello2.wav
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.852879 GailBot-0.2a0/tests/small-test/invalidFile/
--rw-r--r--   0 jasonycwu   (501) staff       (20)        0 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/invalidFile/invalidfile1
--rw-r--r--   0 jasonycwu   (501) staff       (20)        0 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/invalidFile/invalidfile2
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.853368 GailBot-0.2a0/tests/small-test/transcribed-input/
--rw-r--r--   0 jasonycwu   (501) staff       (20)        6 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/transcribed-input/.gailbot
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.817287 GailBot-0.2a0/tests/small-test/transcribed-input/Analysis/
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.856479 GailBot-0.2a0/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      102 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/conversation.S.ca
--rw-r--r--   0 jasonycwu   (501) staff       (20)      102 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/conversation.cha
--rw-r--r--   0 jasonycwu   (501) staff       (20)       63 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/conversation.csv
--rw-r--r--   0 jasonycwu   (501) staff       (20)      601 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/conversation.gailbot.xml
--rw-r--r--   0 jasonycwu   (501) staff       (20)      324 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/conversation.talkbank.xml
--rw-r--r--   0 jasonycwu   (501) staff       (20)       28 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/conversation.txt
--rw-r--r--   0 jasonycwu   (501) staff       (20)     2803 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/format.md
--rw-r--r--   0 jasonycwu   (501) staff       (20)   135212 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/merged.wav
--rw-r--r--   0 jasonycwu   (501) staff       (20)       60 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/words.csv
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.817491 GailBot-0.2a0/tests/small-test/transcribed-input/Raw/
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.857290 GailBot-0.2a0/tests/small-test/transcribed-input/Raw/Media/
--rw-r--r--   0 jasonycwu   (501) staff       (20)   135260 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/transcribed-input/Raw/Media/hello1.wav
--rw-r--r--   0 jasonycwu   (501) staff       (20)   135212 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/transcribed-input/Raw/Media/merged.wav
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.857891 GailBot-0.2a0/tests/small-test/transcribed-input/Raw/Transcript/
--rw-r--r--   0 jasonycwu   (501) staff       (20)       43 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/transcribed-input/Raw/Transcript/hello1.csv
--rw-r--r--   0 jasonycwu   (501) staff       (20)     1119 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/transcribed-input/format.md
--rw-r--r--   0 jasonycwu   (501) staff       (20)      899 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/small-test/transcribed-input/meta.json
--rw-r--r--   0 jasonycwu   (501) staff       (20)    17736 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_api.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.859774 GailBot-0.2a0/tests/test_data/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      328 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/__init__.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)      785 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/data.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     5863 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/path.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     2058 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/payload_obj.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)      471 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/result_data.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.859973 GailBot-0.2a0/tests/test_data/sample_suite/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      371 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/sample_suite/config.toml
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.817809 GailBot-0.2a0/tests/test_data/sample_suite/src/
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.860163 GailBot-0.2a0/tests/test_data/sample_suite/src/sample_dir/
--rw-r--r--   0 jasonycwu   (501) staff       (20)     1341 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/sample_suite/src/sample_dir/sample_module1.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.860352 GailBot-0.2a0/tests/test_data/sample_suite/src/sample_dir2/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      854 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/sample_suite/src/sample_dir2/sample_module2.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     2966 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/setting_data.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.860752 GailBot-0.2a0/tests/test_data/test_suite/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      237 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/test_suite/__init__.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)      893 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/test_suite/config.toml
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.861097 GailBot-0.2a0/tests/test_data/test_suite/src/
--rw-r--r--   0 jasonycwu   (501) staff       (20)        0 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/test_suite/src/__init__.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.862862 GailBot-0.2a0/tests/test_data/test_suite/src/folder1/
--rw-r--r--   0 jasonycwu   (501) staff       (20)      237 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/test_suite/src/folder1/__init__.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)      570 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/test_suite/src/folder1/test_fail1.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)      507 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/test_suite/src/folder1/test_fail2.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)      980 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/test_suite/src/folder1/test_succ1.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)      493 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/test_suite/src/folder1/test_succ2.py
-drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:10:49.863664 GailBot-0.2a0/tests/test_data/test_suite/src/folder2/
--rw-r--r--   0 jasonycwu   (501) staff       (20)        0 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/test_suite/src/folder2/__init__.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)      680 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/test_suite/src/folder2/test_succ3.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)      680 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/test_suite/src/folder2/test_succ4.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)      281 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_data/workspace.py
--rw-r--r--   0 jasonycwu   (501) staff       (20)     3335 2023-08-07 03:38:06.000000 GailBot-0.2a0/tests/test_small.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.081028 GailBot-0.2a1/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1066 2023-08-07 03:38:06.000000 GailBot-0.2a1/LICENSE
+-rw-r--r--   0 jasonycwu   (501) staff       (20)       49 2023-08-07 03:38:06.000000 GailBot-0.2a1/MANIFEST.in
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    10629 2023-08-07 17:13:44.080820 GailBot-0.2a1/PKG-INFO
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     8545 2023-08-07 17:12:20.000000 GailBot-0.2a1/README.md
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1412 2023-08-07 17:07:14.000000 GailBot-0.2a1/pyproject.toml
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     5014 2023-08-07 03:38:06.000000 GailBot-0.2a1/requirements.txt
+-rw-r--r--   0 jasonycwu   (501) staff       (20)       38 2023-08-07 17:13:44.081067 GailBot-0.2a1/setup.cfg
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      251 2023-08-07 03:38:06.000000 GailBot-0.2a1/setup.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.035683 GailBot-0.2a1/src/
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.041688 GailBot-0.2a1/src/.idea/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      176 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/.idea/.gitignore
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.042590 GailBot-0.2a1/src/.idea/inspectionProfiles/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      574 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      174 2023-08-07 02:22:24.000000 GailBot-0.2a1/src/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      181 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/.idea/misc.xml
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      258 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/.idea/modules.xml
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      226 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/.idea/src.iml
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      183 2023-08-07 02:22:24.000000 GailBot-0.2a1/src/.idea/vcs.xml
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.043311 GailBot-0.2a1/src/GailBot.egg-info/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    10629 2023-08-07 17:13:43.000000 GailBot-0.2a1/src/GailBot.egg-info/PKG-INFO
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     9006 2023-08-07 17:13:44.000000 GailBot-0.2a1/src/GailBot.egg-info/SOURCES.txt
+-rw-r--r--   0 jasonycwu   (501) staff       (20)        1 2023-08-07 17:13:43.000000 GailBot-0.2a1/src/GailBot.egg-info/dependency_links.txt
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     5075 2023-08-07 17:13:43.000000 GailBot-0.2a1/src/GailBot.egg-info/requires.txt
+-rw-r--r--   0 jasonycwu   (501) staff       (20)       23 2023-08-07 17:13:43.000000 GailBot-0.2a1/src/GailBot.egg-info/top_level.txt
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.043560 GailBot-0.2a1/src/config_backend/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      230 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/config_backend/__init__.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.035294 GailBot-0.2a1/src/config_backend/engines/
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.043701 GailBot-0.2a1/src/config_backend/engines/google/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      549 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/config_backend/engines/google/google_config.toml
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.043838 GailBot-0.2a1/src/config_backend/engines/watson/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2196 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/config_backend/engines/watson/watson_config.toml
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.043970 GailBot-0.2a1/src/config_backend/engines/whisper/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      929 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/config_backend/engines/whisper/whisper_config.toml
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      546 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/config_backend/paths.toml
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.044109 GailBot-0.2a1/src/config_backend/plugin/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      142 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/config_backend/plugin/valid_plugin.toml
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.044537 GailBot-0.2a1/src/config_backend/services/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      407 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/config_backend/services/default_setting.toml
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1119 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/config_backend/services/format.md
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      448 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/config_backend/services/service.toml
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.044743 GailBot-0.2a1/src/config_backend/settings/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      272 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/config_backend/settings/default.toml
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.045115 GailBot-0.2a1/src/config_backend/toplevel/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1040 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/config_backend/toplevel/ws_config.toml
+-rw-r--r--   0 jasonycwu   (501) staff       (20)       40 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/config_backend/toplevel/ws_root.toml
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.045287 GailBot-0.2a1/src/config_backend/util/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      163 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/config_backend/util/log.toml
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.045807 GailBot-0.2a1/src/gailbot/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      380 2023-08-07 17:12:40.000000 GailBot-0.2a1/src/gailbot/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    22765 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/api.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.046076 GailBot-0.2a1/src/gailbot/configs/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      459 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/configs/__init__.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.046525 GailBot-0.2a1/src/gailbot/configs/confs/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      162 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/configs/confs/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1163 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/configs/confs/paths.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.046776 GailBot-0.2a1/src/gailbot/configs/interfaces/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1767 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/configs/interfaces/__init__.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.046956 GailBot-0.2a1/src/gailbot/configs/interfaces/config/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     4839 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/configs/interfaces/config/ws_config.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.036190 GailBot-0.2a1/src/gailbot/configs/interfaces/core/
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.047486 GailBot-0.2a1/src/gailbot/configs/interfaces/core/engines/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      834 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/configs/interfaces/core/engines/google.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      889 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/configs/interfaces/core/engines/watson.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2111 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/configs/interfaces/core/engines/whisper.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.047641 GailBot-0.2a1/src/gailbot/configs/interfaces/core/setting/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1030 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/configs/interfaces/core/setting/defaults.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.047802 GailBot-0.2a1/src/gailbot/configs/interfaces/core/util/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      540 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/configs/interfaces/core/util/logger.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.048245 GailBot-0.2a1/src/gailbot/configs/interfaces/plugin/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      244 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/configs/interfaces/plugin/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1061 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/configs/interfaces/plugin/pluginsuite.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      229 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/configs/interfaces/plugin/validstructure.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.048560 GailBot-0.2a1/src/gailbot/configs/interfaces/services/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      220 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/configs/interfaces/services/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1921 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/configs/interfaces/services/service.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.048707 GailBot-0.2a1/src/gailbot/core/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      156 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/core/__init__.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.049296 GailBot-0.2a1/src/gailbot/core/engines/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      363 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/core/engines/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1560 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/core/engines/engine.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      976 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/core/engines/engineManager.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2361 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/core/engines/exception.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.049873 GailBot-0.2a1/src/gailbot/core/engines/google/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      184 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/core/engines/google/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    12266 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/core/engines/google/core.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2578 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/core/engines/google/google.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.051840 GailBot-0.2a1/src/gailbot/core/engines/watson/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      260 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/core/engines/watson/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    11756 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/core/engines/watson/am.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      367 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/core/engines/watson/codes.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    12605 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/core/engines/watson/core.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    16999 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/core/engines/watson/lm.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    13203 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/core/engines/watson/recognition_results.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     5085 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/core/engines/watson/recognize_callback.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     4907 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/core/engines/watson/watson.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.052441 GailBot-0.2a1/src/gailbot/core/engines/whisperEngine/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      203 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/core/engines/whisperEngine/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     5643 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/core/engines/whisperEngine/core.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.052734 GailBot-0.2a1/src/gailbot/core/engines/whisperEngine/diarization/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      199 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/core/engines/whisperEngine/diarization/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     3460 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/core/engines/whisperEngine/diarization/utils.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2846 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/core/engines/whisperEngine/parsers.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2100 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/core/engines/whisperEngine/whisperEngine.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.053038 GailBot-0.2a1/src/gailbot/core/engines/whisperX/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      156 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/core/engines/whisperX/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2960 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/core/engines/whisperX/whisperX.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.053455 GailBot-0.2a1/src/gailbot/core/pipeline/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      259 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/core/pipeline/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1046 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/core/pipeline/component.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    10631 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/core/pipeline/pipeline.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.054576 GailBot-0.2a1/src/gailbot/core/utils/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      163 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/core/utils/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2630 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/core/utils/download.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    14143 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/core/utils/general.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1535 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/core/utils/logger.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    27791 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/core/utils/media.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    14816 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/core/utils/threads.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.055212 GailBot-0.2a1/src/gailbot/plugins/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      264 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/plugins/__init__.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.055811 GailBot-0.2a1/src/gailbot/plugins/loader/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      303 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/plugins/loader/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     9172 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/plugins/loader/directoryloader.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      824 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/plugins/loader/pluginLoader.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    10696 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/plugins/loader/urlloader.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    10435 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/plugins/manager.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1364 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/plugins/plugin.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     7744 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/plugins/suite.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.056105 GailBot-0.2a1/src/gailbot/services/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      267 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    23896 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/controller.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.056630 GailBot-0.2a1/src/gailbot/services/converter/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      334 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/converter/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2740 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/converter/converter.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.057579 GailBot-0.2a1/src/gailbot/services/converter/payload/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      458 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/converter/payload/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     3184 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/converter/payload/audioPayload.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     3745 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/converter/payload/conversationDirectoryPayload.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    13064 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/converter/payload/payloadObject.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     3926 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/converter/payload/transcribedDirPayload.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2224 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/converter/payload/videoPayload.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.057887 GailBot-0.2a1/src/gailbot/services/converter/plugin/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      237 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/converter/plugin/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     5744 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/converter/plugin/pluginMethod.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.058744 GailBot-0.2a1/src/gailbot/services/converter/result/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      398 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/converter/result/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1406 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/converter/result/analysis.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1673 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/converter/result/format.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      479 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/converter/result/processingStatus.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1936 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/converter/result/resultInterface.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     5590 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/converter/result/transcribe.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.059030 GailBot-0.2a1/src/gailbot/services/organizer/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      368 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/organizer/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    18452 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/organizer/organizer.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.059578 GailBot-0.2a1/src/gailbot/services/organizer/settings/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      261 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/organizer/settings/__init__.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.060993 GailBot-0.2a1/src/gailbot/services/organizer/settings/interface/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      425 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/organizer/settings/interface/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      665 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/organizer/settings/interface/engineSettingInterface.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2853 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/organizer/settings/interface/googleInterface.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      480 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/organizer/settings/interface/pluginSettingsInterface.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2681 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/organizer/settings/interface/watsonInterface.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2172 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/organizer/settings/interface/whisperInterface.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2105 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/organizer/settings/interface/whisperXInterface.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.061626 GailBot-0.2a1/src/gailbot/services/organizer/settings/objects/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      293 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/organizer/settings/objects/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     4067 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/organizer/settings/objects/engineObject.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      339 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/organizer/settings/objects/pluginObject.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     3539 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/organizer/settings/objects/settingObject.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    19968 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/organizer/settings/settingManager.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.062063 GailBot-0.2a1/src/gailbot/services/organizer/source/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      238 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/organizer/source/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     8415 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/organizer/source/source_manager.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     3330 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/organizer/source/source_object.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.062333 GailBot-0.2a1/src/gailbot/services/pipeline/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      275 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/pipeline/__init__.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.063012 GailBot-0.2a1/src/gailbot/services/pipeline/components/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      146 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/pipeline/components/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     6078 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/pipeline/components/analysisComponent.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2150 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/pipeline/components/formatComponent.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      506 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/pipeline/components/progress.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    10230 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/pipeline/components/transcribeComponent.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1949 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/services/pipeline/pipeline.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.063386 GailBot-0.2a1/src/gailbot/workspace/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      275 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/workspace/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     5567 2023-08-07 03:38:06.000000 GailBot-0.2a1/src/gailbot/workspace/manager.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.065062 GailBot-0.2a1/tests/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1602 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/README
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     5448 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/UPDATELOG
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      172 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/__init__.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.065648 GailBot-0.2a1/tests/configs/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      156 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/configs/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)        0 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/configs/configs_test_configs.toml
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1301 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/configs/test_config.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.065825 GailBot-0.2a1/tests/core/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      156 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/core/__init__.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.067376 GailBot-0.2a1/tests/core/engines/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      156 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/core/engines/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2493 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/core/engines/data.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     5456 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/core/engines/test_google_engine.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1562 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/core/engines/test_watson_am.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     6491 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/core/engines/test_watson_core.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2787 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/core/engines/test_watson_lm.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     5372 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/core/engines/test_whisper.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1168 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/core/engines/test_whisperx.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.067721 GailBot-0.2a1/tests/core/pipeline/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      156 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/core/pipeline/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     4398 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/core/pipeline/test_pipeline.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.068663 GailBot-0.2a1/tests/core/utils/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      156 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/core/utils/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)       72 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/core/utils/test.csv
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    14074 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/core/utils/test_general.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     8668 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/core/utils/test_media.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     9413 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/core/utils/test_thread.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.069724 GailBot-0.2a1/tests/plugins/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      237 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/plugins/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      484 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/plugins/plugin_data.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     5731 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/plugins/plugin_data_old.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     6026 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/plugins/test_plugin.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     6072 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/plugins/test_plugins_old.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.071144 GailBot-0.2a1/tests/small-test/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2371 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/small-test/gailbot_key.json
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.073331 GailBot-0.2a1/tests/small-test/hello-dir/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)   135260 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/small-test/hello-dir/hello1.wav
+-rw-r--r--   0 jasonycwu   (501) staff       (20)   135260 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/small-test/hello-dir/hello2.wav
+-rw-r--r--   0 jasonycwu   (501) staff       (20)   135260 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/small-test/hello-dir/hello3.wav
+-rw-r--r--   0 jasonycwu   (501) staff       (20)   135260 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/small-test/hello-dir/hello4.wav
+-rw-r--r--   0 jasonycwu   (501) staff       (20)   135260 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/small-test/hello1.wav
+-rw-r--r--   0 jasonycwu   (501) staff       (20)   135260 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/small-test/hello2.wav
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.073809 GailBot-0.2a1/tests/small-test/invalidFile/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)        0 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/small-test/invalidFile/invalidfile1
+-rw-r--r--   0 jasonycwu   (501) staff       (20)        0 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/small-test/invalidFile/invalidfile2
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.074300 GailBot-0.2a1/tests/small-test/transcribed-input/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)        6 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/small-test/transcribed-input/.gailbot
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.039178 GailBot-0.2a1/tests/small-test/transcribed-input/Analysis/
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.076567 GailBot-0.2a1/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      102 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/conversation.S.ca
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      102 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/conversation.cha
+-rw-r--r--   0 jasonycwu   (501) staff       (20)       63 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/conversation.csv
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      601 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/conversation.gailbot.xml
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      324 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/conversation.talkbank.xml
+-rw-r--r--   0 jasonycwu   (501) staff       (20)       28 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/conversation.txt
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2803 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/format.md
+-rw-r--r--   0 jasonycwu   (501) staff       (20)   135212 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/merged.wav
+-rw-r--r--   0 jasonycwu   (501) staff       (20)       60 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/words.csv
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.039367 GailBot-0.2a1/tests/small-test/transcribed-input/Raw/
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.077245 GailBot-0.2a1/tests/small-test/transcribed-input/Raw/Media/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)   135260 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/small-test/transcribed-input/Raw/Media/hello1.wav
+-rw-r--r--   0 jasonycwu   (501) staff       (20)   135212 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/small-test/transcribed-input/Raw/Media/merged.wav
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.077574 GailBot-0.2a1/tests/small-test/transcribed-input/Raw/Transcript/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)       43 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/small-test/transcribed-input/Raw/Transcript/hello1.csv
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1119 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/small-test/transcribed-input/format.md
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      899 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/small-test/transcribed-input/meta.json
+-rw-r--r--   0 jasonycwu   (501) staff       (20)    17736 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/test_api.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.078673 GailBot-0.2a1/tests/test_data/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      328 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/test_data/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      785 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/test_data/data.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     5863 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/test_data/path.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2058 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/test_data/payload_obj.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      471 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/test_data/result_data.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.078808 GailBot-0.2a1/tests/test_data/sample_suite/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      371 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/test_data/sample_suite/config.toml
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.039684 GailBot-0.2a1/tests/test_data/sample_suite/src/
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.078939 GailBot-0.2a1/tests/test_data/sample_suite/src/sample_dir/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     1341 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/test_data/sample_suite/src/sample_dir/sample_module1.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.079070 GailBot-0.2a1/tests/test_data/sample_suite/src/sample_dir2/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      854 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/test_data/sample_suite/src/sample_dir2/sample_module2.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     2966 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/test_data/setting_data.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.079388 GailBot-0.2a1/tests/test_data/test_suite/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      237 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/test_data/test_suite/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      893 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/test_data/test_suite/config.toml
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.079525 GailBot-0.2a1/tests/test_data/test_suite/src/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)        0 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/test_data/test_suite/src/__init__.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.080208 GailBot-0.2a1/tests/test_data/test_suite/src/folder1/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      237 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/test_data/test_suite/src/folder1/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      570 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/test_data/test_suite/src/folder1/test_fail1.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      507 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/test_data/test_suite/src/folder1/test_fail2.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      980 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/test_data/test_suite/src/folder1/test_succ1.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      493 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/test_data/test_suite/src/folder1/test_succ2.py
+drwxr-xr-x   0 jasonycwu   (501) staff       (20)        0 2023-08-07 17:13:44.080582 GailBot-0.2a1/tests/test_data/test_suite/src/folder2/
+-rw-r--r--   0 jasonycwu   (501) staff       (20)        0 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/test_data/test_suite/src/folder2/__init__.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      680 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/test_data/test_suite/src/folder2/test_succ3.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      680 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/test_data/test_suite/src/folder2/test_succ4.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)      281 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/test_data/workspace.py
+-rw-r--r--   0 jasonycwu   (501) staff       (20)     3335 2023-08-07 03:38:06.000000 GailBot-0.2a1/tests/test_small.py
```

### Comparing `GailBot-0.2a0/LICENSE` & `GailBot-0.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/PKG-INFO` & `GailBot-0.2a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GailBot
-Version: 0.2a0
+Version: 0.2a1
 Summary: GailBot API
 Author-email: Muhammad Umair <muhammad.umair@tufts.edu>
 Maintainer-email: Human Interaction Lab - Tufts University <hilab-dev@elist.tufts.edu>
 License: MIT License
         
         Copyright (c) 2023 jasonycwu
         
@@ -47,15 +47,15 @@
 Researchers studying human interaction, such as conversation analysts, psychologists, and linguists all rely on detailed transcriptions of language use. Ideally, these should include so-called paralinguistic features of talk, such as overlaps, prosody, and intonation, as they convey important information. However, transcribing these features by hand requires substantial amounts of time by trained transcribers. There are currently no Speech to Text (STT) systems that are able to annotate these features. To reduce the resources needed to create transcripts that include paralinguistic features, we developed a program called GailBot. GailBot combines STT services with plugins to automatically generate first drafts of conversation analytic transcripts. It also enables researchers to add new plugins to transcribe additional features, or to improve the plugins it currently uses. We argue that despite its limitations, GailBot represents a substantial improvement over existing dialogue transcription software.
 
 Find the full paper published by Dialogue and Discourse [here](https://journals.uic.edu/ojs/index.php/dad/article/view/11392).
 
 
 ## Status
 
-GailBot version: 0.1a11 (Pre-release)
+GailBot version: 0.2a1 (Pre-release)
 Release type: API
 
 
 ## Installation
 
 GailBot and the necessary dependencies can be installed using pip with the following commands:
 ```
```

### Comparing `GailBot-0.2a0/README.md` & `GailBot-0.2a1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Researchers studying human interaction, such as conversation analysts, psychologists, and linguists all rely on detailed transcriptions of language use. Ideally, these should include so-called paralinguistic features of talk, such as overlaps, prosody, and intonation, as they convey important information. However, transcribing these features by hand requires substantial amounts of time by trained transcribers. There are currently no Speech to Text (STT) systems that are able to annotate these features. To reduce the resources needed to create transcripts that include paralinguistic features, we developed a program called GailBot. GailBot combines STT services with plugins to automatically generate first drafts of conversation analytic transcripts. It also enables researchers to add new plugins to transcribe additional features, or to improve the plugins it currently uses. We argue that despite its limitations, GailBot represents a substantial improvement over existing dialogue transcription software.
 
 Find the full paper published by Dialogue and Discourse [here](https://journals.uic.edu/ojs/index.php/dad/article/view/11392).
 
 
 ## Status
 
-GailBot version: 0.1a11 (Pre-release)
+GailBot version: 0.2a1 (Pre-release)
 Release type: API
 
 
 ## Installation
 
 GailBot and the necessary dependencies can be installed using pip with the following commands:
 ```
```

### Comparing `GailBot-0.2a0/pyproject.toml` & `GailBot-0.2a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/requirements.txt` & `GailBot-0.2a1/requirements.txt`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/.idea/inspectionProfiles/Project_Default.xml` & `GailBot-0.2a1/src/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/GailBot.egg-info/PKG-INFO` & `GailBot-0.2a1/src/GailBot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GailBot
-Version: 0.2a0
+Version: 0.2a1
 Summary: GailBot API
 Author-email: Muhammad Umair <muhammad.umair@tufts.edu>
 Maintainer-email: Human Interaction Lab - Tufts University <hilab-dev@elist.tufts.edu>
 License: MIT License
         
         Copyright (c) 2023 jasonycwu
         
@@ -47,15 +47,15 @@
 Researchers studying human interaction, such as conversation analysts, psychologists, and linguists all rely on detailed transcriptions of language use. Ideally, these should include so-called paralinguistic features of talk, such as overlaps, prosody, and intonation, as they convey important information. However, transcribing these features by hand requires substantial amounts of time by trained transcribers. There are currently no Speech to Text (STT) systems that are able to annotate these features. To reduce the resources needed to create transcripts that include paralinguistic features, we developed a program called GailBot. GailBot combines STT services with plugins to automatically generate first drafts of conversation analytic transcripts. It also enables researchers to add new plugins to transcribe additional features, or to improve the plugins it currently uses. We argue that despite its limitations, GailBot represents a substantial improvement over existing dialogue transcription software.
 
 Find the full paper published by Dialogue and Discourse [here](https://journals.uic.edu/ojs/index.php/dad/article/view/11392).
 
 
 ## Status
 
-GailBot version: 0.1a11 (Pre-release)
+GailBot version: 0.2a1 (Pre-release)
 Release type: API
 
 
 ## Installation
 
 GailBot and the necessary dependencies can be installed using pip with the following commands:
 ```
```

### Comparing `GailBot-0.2a0/src/GailBot.egg-info/SOURCES.txt` & `GailBot-0.2a1/src/GailBot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/GailBot.egg-info/requires.txt` & `GailBot-0.2a1/src/GailBot.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/config_backend/engines/google/google_config.toml` & `GailBot-0.2a1/src/config_backend/engines/google/google_config.toml`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/config_backend/engines/watson/watson_config.toml` & `GailBot-0.2a1/src/config_backend/engines/watson/watson_config.toml`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/config_backend/engines/whisper/whisper_config.toml` & `GailBot-0.2a1/src/config_backend/engines/whisper/whisper_config.toml`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/config_backend/paths.toml` & `GailBot-0.2a1/src/config_backend/paths.toml`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/config_backend/services/format.md` & `GailBot-0.2a1/src/config_backend/services/format.md`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/config_backend/toplevel/ws_config.toml` & `GailBot-0.2a1/src/config_backend/toplevel/ws_config.toml`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/api.py` & `GailBot-0.2a1/src/gailbot/api.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/configs/confs/paths.py` & `GailBot-0.2a1/src/gailbot/configs/confs/paths.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/configs/interfaces/__init__.py` & `GailBot-0.2a1/src/gailbot/configs/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/configs/interfaces/config/ws_config.py` & `GailBot-0.2a1/src/gailbot/configs/interfaces/config/ws_config.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/configs/interfaces/core/engines/google.py` & `GailBot-0.2a1/src/gailbot/configs/interfaces/core/engines/google.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/configs/interfaces/core/engines/watson.py` & `GailBot-0.2a1/src/gailbot/configs/interfaces/core/engines/watson.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/configs/interfaces/core/engines/whisper.py` & `GailBot-0.2a1/src/gailbot/configs/interfaces/core/engines/whisper.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/configs/interfaces/core/setting/defaults.py` & `GailBot-0.2a1/src/gailbot/configs/interfaces/core/setting/defaults.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/configs/interfaces/core/util/logger.py` & `GailBot-0.2a1/src/gailbot/configs/interfaces/core/util/logger.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/configs/interfaces/plugin/pluginsuite.py` & `GailBot-0.2a1/src/gailbot/configs/interfaces/plugin/pluginsuite.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/configs/interfaces/services/service.py` & `GailBot-0.2a1/src/gailbot/configs/interfaces/services/service.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/core/engines/engine.py` & `GailBot-0.2a1/src/gailbot/core/engines/engine.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/core/engines/engineManager.py` & `GailBot-0.2a1/src/gailbot/core/engines/engineManager.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/core/engines/exception.py` & `GailBot-0.2a1/src/gailbot/core/engines/exception.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/core/engines/google/core.py` & `GailBot-0.2a1/src/gailbot/core/engines/google/core.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/core/engines/google/google.py` & `GailBot-0.2a1/src/gailbot/core/engines/google/google.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/core/engines/watson/am.py` & `GailBot-0.2a1/src/gailbot/core/engines/watson/am.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/core/engines/watson/core.py` & `GailBot-0.2a1/src/gailbot/core/engines/watson/core.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/core/engines/watson/lm.py` & `GailBot-0.2a1/src/gailbot/core/engines/watson/lm.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/core/engines/watson/recognition_results.py` & `GailBot-0.2a1/src/gailbot/core/engines/watson/recognition_results.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/core/engines/watson/recognize_callback.py` & `GailBot-0.2a1/src/gailbot/core/engines/watson/recognize_callback.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/core/engines/watson/watson.py` & `GailBot-0.2a1/src/gailbot/core/engines/watson/watson.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/core/engines/whisperEngine/core.py` & `GailBot-0.2a1/src/gailbot/core/engines/whisperEngine/core.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/core/engines/whisperEngine/diarization/utils.py` & `GailBot-0.2a1/src/gailbot/core/engines/whisperEngine/diarization/utils.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/core/engines/whisperEngine/parsers.py` & `GailBot-0.2a1/src/gailbot/core/engines/whisperEngine/parsers.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/core/engines/whisperEngine/whisperEngine.py` & `GailBot-0.2a1/src/gailbot/core/engines/whisperEngine/whisperEngine.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/core/engines/whisperX/whisperX.py` & `GailBot-0.2a1/src/gailbot/core/engines/whisperX/whisperX.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/core/pipeline/component.py` & `GailBot-0.2a1/src/gailbot/core/pipeline/component.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/core/pipeline/pipeline.py` & `GailBot-0.2a1/src/gailbot/core/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/core/utils/download.py` & `GailBot-0.2a1/src/gailbot/core/utils/download.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/core/utils/general.py` & `GailBot-0.2a1/src/gailbot/core/utils/general.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/core/utils/logger.py` & `GailBot-0.2a1/src/gailbot/core/utils/logger.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/core/utils/media.py` & `GailBot-0.2a1/src/gailbot/core/utils/media.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/core/utils/threads.py` & `GailBot-0.2a1/src/gailbot/core/utils/threads.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/plugins/loader/directoryloader.py` & `GailBot-0.2a1/src/gailbot/plugins/loader/directoryloader.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/plugins/loader/pluginLoader.py` & `GailBot-0.2a1/src/gailbot/plugins/loader/pluginLoader.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/plugins/loader/urlloader.py` & `GailBot-0.2a1/src/gailbot/plugins/loader/urlloader.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/plugins/manager.py` & `GailBot-0.2a1/src/gailbot/plugins/manager.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/plugins/plugin.py` & `GailBot-0.2a1/src/gailbot/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/plugins/suite.py` & `GailBot-0.2a1/src/gailbot/plugins/suite.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/services/controller.py` & `GailBot-0.2a1/src/gailbot/services/controller.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/services/converter/converter.py` & `GailBot-0.2a1/src/gailbot/services/converter/converter.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/services/converter/payload/audioPayload.py` & `GailBot-0.2a1/src/gailbot/services/converter/payload/audioPayload.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/services/converter/payload/conversationDirectoryPayload.py` & `GailBot-0.2a1/src/gailbot/services/converter/payload/conversationDirectoryPayload.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/services/converter/payload/payloadObject.py` & `GailBot-0.2a1/src/gailbot/services/converter/payload/payloadObject.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/services/converter/payload/transcribedDirPayload.py` & `GailBot-0.2a1/src/gailbot/services/converter/payload/transcribedDirPayload.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/services/converter/payload/videoPayload.py` & `GailBot-0.2a1/src/gailbot/services/converter/payload/videoPayload.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/services/converter/plugin/pluginMethod.py` & `GailBot-0.2a1/src/gailbot/services/converter/plugin/pluginMethod.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/services/converter/result/analysis.py` & `GailBot-0.2a1/src/gailbot/services/converter/result/analysis.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/services/converter/result/format.py` & `GailBot-0.2a1/src/gailbot/services/converter/result/format.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/services/converter/result/resultInterface.py` & `GailBot-0.2a1/src/gailbot/services/converter/result/resultInterface.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/services/converter/result/transcribe.py` & `GailBot-0.2a1/src/gailbot/services/converter/result/transcribe.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/services/organizer/organizer.py` & `GailBot-0.2a1/src/gailbot/services/organizer/organizer.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/services/organizer/settings/interface/engineSettingInterface.py` & `GailBot-0.2a1/src/gailbot/services/organizer/settings/interface/engineSettingInterface.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/services/organizer/settings/interface/googleInterface.py` & `GailBot-0.2a1/src/gailbot/services/organizer/settings/interface/googleInterface.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/services/organizer/settings/interface/watsonInterface.py` & `GailBot-0.2a1/src/gailbot/services/organizer/settings/interface/watsonInterface.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/services/organizer/settings/interface/whisperInterface.py` & `GailBot-0.2a1/src/gailbot/services/organizer/settings/interface/whisperInterface.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/services/organizer/settings/interface/whisperXInterface.py` & `GailBot-0.2a1/src/gailbot/services/organizer/settings/interface/whisperXInterface.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/services/organizer/settings/objects/engineObject.py` & `GailBot-0.2a1/src/gailbot/services/organizer/settings/objects/engineObject.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/services/organizer/settings/objects/settingObject.py` & `GailBot-0.2a1/src/gailbot/services/organizer/settings/objects/settingObject.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/services/organizer/settings/settingManager.py` & `GailBot-0.2a1/src/gailbot/services/organizer/settings/settingManager.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/services/organizer/source/source_manager.py` & `GailBot-0.2a1/src/gailbot/services/organizer/source/source_manager.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/services/organizer/source/source_object.py` & `GailBot-0.2a1/src/gailbot/services/organizer/source/source_object.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/services/pipeline/components/analysisComponent.py` & `GailBot-0.2a1/src/gailbot/services/pipeline/components/analysisComponent.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/services/pipeline/components/formatComponent.py` & `GailBot-0.2a1/src/gailbot/services/pipeline/components/formatComponent.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/services/pipeline/components/transcribeComponent.py` & `GailBot-0.2a1/src/gailbot/services/pipeline/components/transcribeComponent.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/services/pipeline/pipeline.py` & `GailBot-0.2a1/src/gailbot/services/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/src/gailbot/workspace/manager.py` & `GailBot-0.2a1/src/gailbot/workspace/manager.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/README` & `GailBot-0.2a1/tests/README`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/UPDATELOG` & `GailBot-0.2a1/tests/UPDATELOG`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/configs/test_config.py` & `GailBot-0.2a1/tests/configs/test_config.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/core/engines/data.py` & `GailBot-0.2a1/tests/core/engines/data.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/core/engines/test_google_engine.py` & `GailBot-0.2a1/tests/core/engines/test_google_engine.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/core/engines/test_watson_am.py` & `GailBot-0.2a1/tests/core/engines/test_watson_am.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/core/engines/test_watson_core.py` & `GailBot-0.2a1/tests/core/engines/test_watson_core.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/core/engines/test_watson_lm.py` & `GailBot-0.2a1/tests/core/engines/test_watson_lm.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/core/engines/test_whisper.py` & `GailBot-0.2a1/tests/core/engines/test_whisper.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/core/engines/test_whisperx.py` & `GailBot-0.2a1/tests/core/engines/test_whisperx.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/core/pipeline/test_pipeline.py` & `GailBot-0.2a1/tests/core/pipeline/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/core/utils/test_general.py` & `GailBot-0.2a1/tests/core/utils/test_general.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/core/utils/test_media.py` & `GailBot-0.2a1/tests/core/utils/test_media.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/core/utils/test_thread.py` & `GailBot-0.2a1/tests/core/utils/test_thread.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/plugins/plugin_data_old.py` & `GailBot-0.2a1/tests/plugins/plugin_data_old.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/plugins/test_plugin.py` & `GailBot-0.2a1/tests/plugins/test_plugin.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/plugins/test_plugins_old.py` & `GailBot-0.2a1/tests/plugins/test_plugins_old.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/small-test/gailbot_key.json` & `GailBot-0.2a1/tests/small-test/gailbot_key.json`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/small-test/hello-dir/hello1.wav` & `GailBot-0.2a1/tests/small-test/hello-dir/hello1.wav`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/small-test/hello-dir/hello2.wav` & `GailBot-0.2a1/tests/small-test/hello-dir/hello2.wav`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/small-test/hello-dir/hello3.wav` & `GailBot-0.2a1/tests/small-test/hello-dir/hello3.wav`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/small-test/hello-dir/hello4.wav` & `GailBot-0.2a1/tests/small-test/hello-dir/hello4.wav`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/small-test/hello1.wav` & `GailBot-0.2a1/tests/small-test/hello1.wav`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/small-test/hello2.wav` & `GailBot-0.2a1/tests/small-test/hello2.wav`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/conversation.gailbot.xml` & `GailBot-0.2a1/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/conversation.gailbot.xml`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/format.md` & `GailBot-0.2a1/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/format.md`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/merged.wav` & `GailBot-0.2a1/tests/small-test/transcribed-input/Analysis/gb_hilab_suite/merged.wav`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/small-test/transcribed-input/Raw/Media/hello1.wav` & `GailBot-0.2a1/tests/small-test/transcribed-input/Raw/Media/hello1.wav`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/small-test/transcribed-input/Raw/Media/merged.wav` & `GailBot-0.2a1/tests/small-test/transcribed-input/Raw/Media/merged.wav`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/small-test/transcribed-input/format.md` & `GailBot-0.2a1/tests/small-test/transcribed-input/format.md`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/small-test/transcribed-input/meta.json` & `GailBot-0.2a1/tests/small-test/transcribed-input/meta.json`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/test_api.py` & `GailBot-0.2a1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/test_data/data.py` & `GailBot-0.2a1/tests/test_data/data.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/test_data/path.py` & `GailBot-0.2a1/tests/test_data/path.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/test_data/payload_obj.py` & `GailBot-0.2a1/tests/test_data/payload_obj.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/test_data/sample_suite/src/sample_dir/sample_module1.py` & `GailBot-0.2a1/tests/test_data/sample_suite/src/sample_dir/sample_module1.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/test_data/sample_suite/src/sample_dir2/sample_module2.py` & `GailBot-0.2a1/tests/test_data/sample_suite/src/sample_dir2/sample_module2.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/test_data/setting_data.py` & `GailBot-0.2a1/tests/test_data/setting_data.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/test_data/test_suite/config.toml` & `GailBot-0.2a1/tests/test_data/test_suite/config.toml`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/test_data/test_suite/src/folder1/test_fail1.py` & `GailBot-0.2a1/tests/test_data/test_suite/src/folder1/test_fail1.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/test_data/test_suite/src/folder1/test_succ1.py` & `GailBot-0.2a1/tests/test_data/test_suite/src/folder1/test_succ1.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/test_data/test_suite/src/folder2/test_succ3.py` & `GailBot-0.2a1/tests/test_data/test_suite/src/folder2/test_succ3.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/test_data/test_suite/src/folder2/test_succ4.py` & `GailBot-0.2a1/tests/test_data/test_suite/src/folder2/test_succ4.py`

 * *Files identical despite different names*

### Comparing `GailBot-0.2a0/tests/test_small.py` & `GailBot-0.2a1/tests/test_small.py`

 * *Files identical despite different names*

