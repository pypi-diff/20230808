# Comparing `tmp/mentat-ai-0.1.8.tar.gz` & `tmp/mentat-ai-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentat-ai-0.1.8.tar", last modified: Mon Jul 31 20:29:29 2023, max compression
+gzip compressed data, was "mentat-ai-0.1.9.tar", last modified: Tue Aug  1 05:22:43 2023, max compression
```

## Comparing `mentat-ai-0.1.8.tar` & `mentat-ai-0.1.9.tar`

### file list

```diff
@@ -1,51 +1,53 @@
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-31 20:29:29.150919 mentat-ai-0.1.8/
--rw-r--r--   0 biobootloader   (501) staff       (20)    11357 2023-07-08 00:24:17.000000 mentat-ai-0.1.8/LICENSE
--rw-r--r--   0 biobootloader   (501) staff       (20)     4108 2023-07-31 20:29:29.150785 mentat-ai-0.1.8/PKG-INFO
--rw-r--r--   0 biobootloader   (501) staff       (20)     3898 2023-07-31 14:40:12.000000 mentat-ai-0.1.8/README.md
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-31 20:29:29.140954 mentat-ai-0.1.8/mentat/
--rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-07-12 23:06:24.000000 mentat-ai-0.1.8/mentat/__init__.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      342 2023-07-28 22:38:12.000000 mentat-ai-0.1.8/mentat/__main__.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     6949 2023-07-31 14:40:12.000000 mentat-ai-0.1.8/mentat/app.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     4175 2023-07-22 22:55:34.000000 mentat-ai-0.1.8/mentat/change_conflict_resolution.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     5095 2023-07-22 22:55:34.000000 mentat-ai-0.1.8/mentat/code_change.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     4283 2023-07-22 22:55:34.000000 mentat-ai-0.1.8/mentat/code_change_display.py
--rw-r--r--   0 biobootloader   (501) staff       (20)    10455 2023-07-31 14:40:12.000000 mentat-ai-0.1.8/mentat/code_file_manager.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     3422 2023-07-30 05:21:38.000000 mentat-ai-0.1.8/mentat/config_manager.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     1728 2023-07-28 22:38:12.000000 mentat-ai-0.1.8/mentat/conversation.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      293 2023-07-30 05:20:49.000000 mentat-ai-0.1.8/mentat/default_config.json
--rw-r--r--   0 biobootloader   (501) staff       (20)     2603 2023-07-31 20:17:16.000000 mentat-ai-0.1.8/mentat/git_handler.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     4547 2023-07-31 20:26:16.000000 mentat-ai-0.1.8/mentat/llm_api.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     1696 2023-07-22 22:55:34.000000 mentat-ai-0.1.8/mentat/logging_config.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     8169 2023-07-27 16:52:26.000000 mentat-ai-0.1.8/mentat/parsing.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     3559 2023-07-15 05:21:35.000000 mentat-ai-0.1.8/mentat/prompts.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     1452 2023-07-21 00:32:22.000000 mentat-ai-0.1.8/mentat/streaming_printer.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     3193 2023-07-21 00:32:22.000000 mentat-ai-0.1.8/mentat/user_input_manager.py
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-31 20:29:29.141593 mentat-ai-0.1.8/mentat_ai.egg-info/
--rw-r--r--   0 biobootloader   (501) staff       (20)     4108 2023-07-31 20:29:29.000000 mentat-ai-0.1.8/mentat_ai.egg-info/PKG-INFO
--rw-r--r--   0 biobootloader   (501) staff       (20)     1068 2023-07-31 20:29:29.000000 mentat-ai-0.1.8/mentat_ai.egg-info/SOURCES.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)        1 2023-07-31 20:29:29.000000 mentat-ai-0.1.8/mentat_ai.egg-info/dependency_links.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)       46 2023-07-31 20:29:29.000000 mentat-ai-0.1.8/mentat_ai.egg-info/entry_points.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)      764 2023-07-31 20:29:29.000000 mentat-ai-0.1.8/mentat_ai.egg-info/requires.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)       21 2023-07-31 20:29:29.000000 mentat-ai-0.1.8/mentat_ai.egg-info/top_level.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)       91 2023-07-21 00:32:22.000000 mentat-ai-0.1.8/pyproject.toml
--rw-r--r--   0 biobootloader   (501) staff       (20)       38 2023-07-31 20:29:29.150964 mentat-ai-0.1.8/setup.cfg
--rw-r--r--   0 biobootloader   (501) staff       (20)      853 2023-07-31 20:29:10.000000 mentat-ai-0.1.8/setup.py
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-31 20:29:29.142530 mentat-ai-0.1.8/testbed/
--rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-05-31 00:08:09.000000 mentat-ai-0.1.8/testbed/__init__.py
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-31 20:29:29.145171 mentat-ai-0.1.8/testbed/multifile_calculator/
--rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-05-31 00:07:36.000000 mentat-ai-0.1.8/testbed/multifile_calculator/__init__.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      580 2023-07-18 20:17:52.000000 mentat-ai-0.1.8/testbed/multifile_calculator/calculator.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      179 2023-07-18 20:17:50.000000 mentat-ai-0.1.8/testbed/multifile_calculator/operations.py
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-31 20:29:29.150474 mentat-ai-0.1.8/tests/
--rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-07-12 22:56:07.000000 mentat-ai-0.1.8/tests/__init__.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     4010 2023-07-21 00:32:22.000000 mentat-ai-0.1.8/tests/benchmark_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     7024 2023-07-31 14:40:12.000000 mentat-ai-0.1.8/tests/code_file_manager_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     7515 2023-07-31 14:40:12.000000 mentat-ai-0.1.8/tests/codechange_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     1549 2023-07-30 05:20:49.000000 mentat-ai-0.1.8/tests/config_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     3992 2023-07-30 05:20:49.000000 mentat-ai-0.1.8/tests/conftest.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      826 2023-07-30 05:20:49.000000 mentat-ai-0.1.8/tests/git_handler_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     1270 2023-07-30 05:20:49.000000 mentat-ai-0.1.8/tests/license_check.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     1467 2023-07-12 22:02:48.000000 mentat-ai-0.1.8/tests/measure_api_speed.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     2605 2023-07-25 13:33:37.000000 mentat-ai-0.1.8/tests/record_benchmark.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     2924 2023-07-30 14:54:58.000000 mentat-ai-0.1.8/tests/system_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      825 2023-07-21 00:32:22.000000 mentat-ai-0.1.8/tests/ui_test.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-08-01 05:22:43.206486 mentat-ai-0.1.9/
+-rw-r--r--   0 biobootloader   (501) staff       (20)    11357 2023-07-08 00:24:17.000000 mentat-ai-0.1.9/LICENSE
+-rw-r--r--   0 biobootloader   (501) staff       (20)     4126 2023-08-01 05:22:43.206364 mentat-ai-0.1.9/PKG-INFO
+-rw-r--r--   0 biobootloader   (501) staff       (20)     3916 2023-08-01 05:21:29.000000 mentat-ai-0.1.9/README.md
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-08-01 05:22:43.202509 mentat-ai-0.1.9/mentat/
+-rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-07-12 23:06:24.000000 mentat-ai-0.1.9/mentat/__init__.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      342 2023-07-28 22:38:12.000000 mentat-ai-0.1.9/mentat/__main__.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     5559 2023-08-01 05:21:29.000000 mentat-ai-0.1.9/mentat/app.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     4175 2023-07-22 22:55:34.000000 mentat-ai-0.1.9/mentat/change_conflict_resolution.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     5675 2023-08-01 05:21:29.000000 mentat-ai-0.1.9/mentat/code_change.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     4283 2023-07-22 22:55:34.000000 mentat-ai-0.1.9/mentat/code_change_display.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)    10573 2023-08-01 05:21:29.000000 mentat-ai-0.1.9/mentat/code_file_manager.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     3422 2023-07-30 05:21:38.000000 mentat-ai-0.1.9/mentat/config_manager.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1728 2023-08-01 05:20:26.000000 mentat-ai-0.1.9/mentat/conversation.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      293 2023-07-30 05:20:49.000000 mentat-ai-0.1.9/mentat/default_config.json
+-rw-r--r--   0 biobootloader   (501) staff       (20)     2603 2023-08-01 04:54:47.000000 mentat-ai-0.1.9/mentat/git_handler.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     4547 2023-08-01 05:21:29.000000 mentat-ai-0.1.9/mentat/llm_api.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1772 2023-08-01 05:21:29.000000 mentat-ai-0.1.9/mentat/logging_config.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      274 2023-08-01 05:21:29.000000 mentat-ai-0.1.9/mentat/model_error.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)    11180 2023-08-01 05:21:29.000000 mentat-ai-0.1.9/mentat/parsing.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     3559 2023-07-15 05:21:35.000000 mentat-ai-0.1.9/mentat/prompts.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1452 2023-07-21 00:32:22.000000 mentat-ai-0.1.9/mentat/streaming_printer.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     3193 2023-07-21 00:32:22.000000 mentat-ai-0.1.9/mentat/user_input_manager.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-08-01 05:22:43.203148 mentat-ai-0.1.9/mentat_ai.egg-info/
+-rw-r--r--   0 biobootloader   (501) staff       (20)     4126 2023-08-01 05:22:43.000000 mentat-ai-0.1.9/mentat_ai.egg-info/PKG-INFO
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1117 2023-08-01 05:22:43.000000 mentat-ai-0.1.9/mentat_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)        1 2023-08-01 05:22:43.000000 mentat-ai-0.1.9/mentat_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)       46 2023-08-01 05:22:43.000000 mentat-ai-0.1.9/mentat_ai.egg-info/entry_points.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)      764 2023-08-01 05:22:43.000000 mentat-ai-0.1.9/mentat_ai.egg-info/requires.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)       21 2023-08-01 05:22:43.000000 mentat-ai-0.1.9/mentat_ai.egg-info/top_level.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)       91 2023-07-21 00:32:22.000000 mentat-ai-0.1.9/pyproject.toml
+-rw-r--r--   0 biobootloader   (501) staff       (20)       38 2023-08-01 05:22:43.206517 mentat-ai-0.1.9/setup.cfg
+-rw-r--r--   0 biobootloader   (501) staff       (20)      853 2023-08-01 05:22:27.000000 mentat-ai-0.1.9/setup.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-08-01 05:22:43.203240 mentat-ai-0.1.9/testbed/
+-rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-05-31 00:08:09.000000 mentat-ai-0.1.9/testbed/__init__.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-08-01 05:22:43.203785 mentat-ai-0.1.9/testbed/multifile_calculator/
+-rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-05-31 00:07:36.000000 mentat-ai-0.1.9/testbed/multifile_calculator/__init__.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      580 2023-07-18 20:17:52.000000 mentat-ai-0.1.9/testbed/multifile_calculator/calculator.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      179 2023-07-18 20:17:50.000000 mentat-ai-0.1.9/testbed/multifile_calculator/operations.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-08-01 05:22:43.206082 mentat-ai-0.1.9/tests/
+-rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-07-12 22:56:07.000000 mentat-ai-0.1.9/tests/__init__.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     4010 2023-07-21 00:32:22.000000 mentat-ai-0.1.9/tests/benchmark_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     7515 2023-08-01 05:21:29.000000 mentat-ai-0.1.9/tests/code_change_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     7637 2023-08-01 05:21:29.000000 mentat-ai-0.1.9/tests/code_file_manager_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1549 2023-07-30 05:20:49.000000 mentat-ai-0.1.9/tests/config_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     3992 2023-07-30 05:20:49.000000 mentat-ai-0.1.9/tests/conftest.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      826 2023-07-30 05:20:49.000000 mentat-ai-0.1.9/tests/git_handler_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1270 2023-07-30 05:20:49.000000 mentat-ai-0.1.9/tests/license_check.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1467 2023-07-12 22:02:48.000000 mentat-ai-0.1.9/tests/measure_api_speed.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     7789 2023-08-01 05:21:29.000000 mentat-ai-0.1.9/tests/model_error_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     2605 2023-07-25 13:33:37.000000 mentat-ai-0.1.9/tests/record_benchmark.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     4239 2023-08-01 05:21:29.000000 mentat-ai-0.1.9/tests/system_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      825 2023-07-21 00:32:22.000000 mentat-ai-0.1.9/tests/ui_test.py
```

### Comparing `mentat-ai-0.1.8/LICENSE` & `mentat-ai-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.8/PKG-INFO` & `mentat-ai-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mentat-ai
-Version: 0.1.8
+Version: 0.1.9
 Summary: AI coding assistant on your command line
 License: Apache-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Twitter Follow](https://img.shields.io/twitter/follow/bio_bootloader?style=social)](https://twitter.com/bio_bootloader)
@@ -90,9 +90,9 @@
 
 ## Options
 
 ### Exclude Files
 
 Exclude given paths, directories, or [glob patterns](https://docs.python.org/3/library/glob.html) from Mentat's context. Takes precedence over included file paths.
 ```
-mentat --exclude exclude_me.py dir1/dir2 **/*.ts
+mentat path/to/directory --exclude exclude_me.py dir1/dir2 **/*.ts
 ```
```

### Comparing `mentat-ai-0.1.8/README.md` & `mentat-ai-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -81,9 +81,9 @@
 
 ## Options
 
 ### Exclude Files
 
 Exclude given paths, directories, or [glob patterns](https://docs.python.org/3/library/glob.html) from Mentat's context. Takes precedence over included file paths.
 ```
-mentat --exclude exclude_me.py dir1/dir2 **/*.ts
+mentat path/to/directory --exclude exclude_me.py dir1/dir2 **/*.ts
 ```
```

### Comparing `mentat-ai-0.1.8/mentat/app.py` & `mentat-ai-0.1.9/mentat/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import glob
 import logging
 import os
 from typing import Iterable, Optional
 
 from termcolor import cprint
 
-from .code_change import CodeChange, CodeChangeAction
+from .code_change import CodeChange
 from .code_change_display import print_change
 from .code_file_manager import CodeFileManager
 from .config_manager import ConfigManager, mentat_dir_path
 from .conversation import Conversation
 from .git_handler import get_shared_git_root_for_paths
 from .llm_api import CostTracker, count_tokens, setup_api_key
 from .logging_config import setup_logging
@@ -85,60 +85,23 @@
     cprint("What can I do for you?", color="light_blue")
     need_user_request = True
     while True:
         if need_user_request:
             user_response = user_input_manager.collect_user_input()
             conv.add_user_message(user_response)
         explanation, code_changes = conv.get_model_response(code_file_manager, config)
-        warn_user_wrong_files(code_file_manager, code_changes, git_root)
 
         if code_changes:
             need_user_request = get_user_feedback_on_changes(
                 config, conv, user_input_manager, code_file_manager, code_changes
             )
         else:
             need_user_request = True
 
 
-def warn_user_wrong_files(
-    code_file_manager: CodeFileManager,
-    code_changes: Iterable[CodeChange],
-    git_root: str,
-):
-    warned = set()
-    for change in code_changes:
-        if change.action == CodeChangeAction.CreateFile and os.path.exists(change.file):
-            logging.info("Model tried to create a file that already exists")
-            cprint(
-                f"Error: tried to create {change.file}, but file already existed!",
-                color="red",
-            )
-            raise KeyboardInterrupt
-        elif change.action == CodeChangeAction.DeleteFile and not os.path.exists(
-            change.file
-        ):
-            logging.info("Model tried to delete a file that didn't exist")
-            cprint(
-                f"Error: tried to delete {change.file}, but file doesn't exist!",
-                color="red",
-            )
-            raise KeyboardInterrupt
-
-        if (
-            os.path.join(git_root, change.file) not in code_file_manager.file_paths
-            and change.action != CodeChangeAction.CreateFile
-            and change.file not in warned
-        ):
-            warned.add(change.file)
-            cprint(
-                f"Change in {change.file} does not match original files!",
-                color="light_yellow",
-            )
-
-
 def get_user_feedback_on_changes(
     config: ConfigManager,
     conv: Conversation,
     user_input_manager: UserInputManager,
     code_file_manager: CodeFileManager,
     code_changes: Iterable[CodeChange],
 ) -> bool:
```

### Comparing `mentat-ai-0.1.8/mentat/change_conflict_resolution.py` & `mentat-ai-0.1.9/mentat/change_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.8/mentat/code_change_display.py` & `mentat-ai-0.1.9/mentat/code_change_display.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.8/mentat/code_file_manager.py` & `mentat-ai-0.1.9/mentat/code_file_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,22 +176,28 @@
             self.file_lines[abs_path] = self._read_file(abs_path)
 
     def get_code_message(self):
         self._read_all_file_lines()
         code_message = ["Code Files:\n"]
         for abs_path in self.file_paths:
             rel_path = os.path.relpath(abs_path, self.git_root)
-            code_message.append(rel_path)
+
+            # We always want to give GPT posix paths
+            posix_rel_path = Path(rel_path).as_posix()
+            code_message.append(posix_rel_path)
+
             for i, line in enumerate(self.file_lines[abs_path], start=1):
                 code_message.append(f"{i}:{line}")
             code_message.append("")
+
             git_diff_output = get_git_diff_for_path(self.git_root, rel_path)
             if git_diff_output:
                 code_message.append("Current git diff for this file:")
                 code_message.append(f"{git_diff_output}")
+
         return "\n".join(code_message)
 
     def _handle_delete(self, delete_change):
         file_path = os.path.join(self.git_root, delete_change.file)
         if not os.path.exists(file_path):
             logging.error(f"Path {file_path} non-existent on delete")
             return
```

### Comparing `mentat-ai-0.1.8/mentat/config_manager.py` & `mentat-ai-0.1.9/mentat/config_manager.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.8/mentat/conversation.py` & `mentat-ai-0.1.9/mentat/conversation.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.8/mentat/git_handler.py` & `mentat-ai-0.1.9/mentat/git_handler.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.8/mentat/llm_api.py` & `mentat-ai-0.1.9/mentat/llm_api.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.8/mentat/logging_config.py` & `mentat-ai-0.1.9/mentat/logging_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 def setup_logging():
     logs_dir = "logs"
     if "PYTEST_CURRENT_TEST" in os.environ:
         logs_dir += "/test_logs"
     logs_path = os.path.join(mentat_dir_path, logs_dir)
 
     logging.getLogger("openai").setLevel(logging.WARNING)
-    logging.getLogger("asyncio").setLevel(logging.WARNING)
+    # Breaking out of async generator when model messes up causes an error
+    logging.getLogger("asyncio").setLevel(logging.CRITICAL)
     formatter = logging.Formatter("%(asctime)s - %(levelname)s - %(message)s")
 
     console_handler = logging.StreamHandler()
     console_handler.setFormatter(formatter)
     # Only log warnings and higher to console
     console_handler.setLevel(logging.WARNING)
```

### Comparing `mentat-ai-0.1.8/mentat/prompts.py` & `mentat-ai-0.1.9/mentat/prompts.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.8/mentat/streaming_printer.py` & `mentat-ai-0.1.9/mentat/streaming_printer.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.8/mentat/user_input_manager.py` & `mentat-ai-0.1.9/mentat/user_input_manager.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.8/mentat_ai.egg-info/PKG-INFO` & `mentat-ai-0.1.9/mentat_ai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mentat-ai
-Version: 0.1.8
+Version: 0.1.9
 Summary: AI coding assistant on your command line
 License: Apache-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Twitter Follow](https://img.shields.io/twitter/follow/bio_bootloader?style=social)](https://twitter.com/bio_bootloader)
@@ -90,9 +90,9 @@
 
 ## Options
 
 ### Exclude Files
 
 Exclude given paths, directories, or [glob patterns](https://docs.python.org/3/library/glob.html) from Mentat's context. Takes precedence over included file paths.
 ```
-mentat --exclude exclude_me.py dir1/dir2 **/*.ts
+mentat path/to/directory --exclude exclude_me.py dir1/dir2 **/*.ts
 ```
```

### Comparing `mentat-ai-0.1.8/mentat_ai.egg-info/SOURCES.txt` & `mentat-ai-0.1.9/mentat_ai.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 mentat/code_file_manager.py
 mentat/config_manager.py
 mentat/conversation.py
 mentat/default_config.json
 mentat/git_handler.py
 mentat/llm_api.py
 mentat/logging_config.py
+mentat/model_error.py
 mentat/parsing.py
 mentat/prompts.py
 mentat/streaming_printer.py
 mentat/user_input_manager.py
 mentat_ai.egg-info/PKG-INFO
 mentat_ai.egg-info/SOURCES.txt
 mentat_ai.egg-info/dependency_links.txt
@@ -27,17 +28,18 @@
 mentat_ai.egg-info/top_level.txt
 testbed/__init__.py
 testbed/multifile_calculator/__init__.py
 testbed/multifile_calculator/calculator.py
 testbed/multifile_calculator/operations.py
 tests/__init__.py
 tests/benchmark_test.py
+tests/code_change_test.py
 tests/code_file_manager_test.py
-tests/codechange_test.py
 tests/config_test.py
 tests/conftest.py
 tests/git_handler_test.py
 tests/license_check.py
 tests/measure_api_speed.py
+tests/model_error_test.py
 tests/record_benchmark.py
 tests/system_test.py
 tests/ui_test.py
```

### Comparing `mentat-ai-0.1.8/mentat_ai.egg-info/requires.txt` & `mentat-ai-0.1.9/mentat_ai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.8/setup.py` & `mentat-ai-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 readme_path = os.path.join(Path(__file__).parent, "README.md")
 with open(readme_path, "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="mentat-ai",
-    version="0.1.8",
+    version="0.1.9",
     python_requires=">=3.10",
     packages=find_packages(),
     install_requires=read_requirements("requirements.txt"),
     package_data={
         "mentat": ["default_config.json"],
     },
     entry_points={
```

### Comparing `mentat-ai-0.1.8/testbed/multifile_calculator/calculator.py` & `mentat-ai-0.1.9/testbed/multifile_calculator/calculator.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.8/tests/benchmark_test.py` & `mentat-ai-0.1.9/tests/benchmark_test.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.8/tests/code_file_manager_test.py` & `mentat-ai-0.1.9/tests/code_file_manager_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -176,7 +176,26 @@
             paths,
             [],
             user_input_manager=None,
             config=mock_config,
             git_root=temp_testbed,
         )
     assert e_info.type == KeyboardInterrupt
+
+
+# Make sure we always give posix paths to GPT
+def test_posix_paths(temp_testbed, mock_config):
+    dir_name = "dir"
+    file_name = "file.txt"
+    file_path = os.path.join(dir_name, file_name)
+    os.makedirs(dir_name, exist_ok=True)
+    with open(file_path, "w") as file_file:
+        file_file.write("I am a file")
+    code_file_manager = CodeFileManager(
+        [file_path],
+        [],
+        user_input_manager=None,
+        config=mock_config,
+        git_root=temp_testbed,
+    )
+    code_message = code_file_manager.get_code_message()
+    assert dir_name + "/" + file_name in code_message.split("\n")
```

### Comparing `mentat-ai-0.1.8/tests/codechange_test.py` & `mentat-ai-0.1.9/tests/code_change_test.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.8/tests/config_test.py` & `mentat-ai-0.1.9/tests/config_test.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.8/tests/conftest.py` & `mentat-ai-0.1.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.8/tests/git_handler_test.py` & `mentat-ai-0.1.9/tests/git_handler_test.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.8/tests/license_check.py` & `mentat-ai-0.1.9/tests/license_check.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.8/tests/measure_api_speed.py` & `mentat-ai-0.1.9/tests/measure_api_speed.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.8/tests/record_benchmark.py` & `mentat-ai-0.1.9/tests/record_benchmark.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.8/tests/ui_test.py` & `mentat-ai-0.1.9/tests/ui_test.py`

 * *Files identical despite different names*

