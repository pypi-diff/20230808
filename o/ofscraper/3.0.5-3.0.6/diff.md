# Comparing `tmp/ofscraper-3.0.5.tar.gz` & `tmp/ofscraper-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-3.0.5.tar", max compression
+gzip compressed data, was "ofscraper-3.0.6.tar", max compression
```

## Comparing `ofscraper-3.0.5.tar` & `ofscraper-3.0.6.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     1067 2023-08-07 13:27:44.367449 ofscraper-3.0.5/LICENSE
--rw-r--r--   0        0        0     2863 2023-08-07 13:27:44.367449 ofscraper-3.0.5/README.md
--rwxr-xr-x   0        0        0      254 2023-08-07 13:27:44.375449 ofscraper-3.0.5/ofscraper/__main__.py
--rw-r--r--   0        0        0     1016 2023-08-07 13:27:44.375449 ofscraper-3.0.5/ofscraper/__version__.py
--rw-r--r--   0        0        0      999 2023-08-07 13:27:44.375449 ofscraper-3.0.5/ofscraper/__version__.pye
--rw-r--r--   0        0        0     8736 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/api/archive.py
--rw-r--r--   0        0        0     9895 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/api/highlights.py
--rw-r--r--   0        0        0     1029 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/api/init.py
--rw-r--r--   0        0        0     7568 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/api/labels.py
--rw-r--r--   0        0        0     2946 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/api/me.py
--rw-r--r--   0        0        0     9518 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/api/messages.py
--rw-r--r--   0        0        0     9687 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/api/paid.py
--rw-r--r--   0        0        0     5730 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/api/pinned.py
--rw-r--r--   0        0        0     4497 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/api/profile.py
--rw-r--r--   0        0        0     3384 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/api/subscriptions.py
--rw-r--r--   0        0        0     9312 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/api/timeline.py
--rw-r--r--   0        0        0      804 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/classes/labels.py
--rw-r--r--   0        0        0     8779 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/classes/media.py
--rw-r--r--   0        0        0     1795 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/classes/multiprocessprogress.py
--rw-r--r--   0        0        0     8068 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/classes/placeholder.py
--rw-r--r--   0        0        0     3734 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/classes/posts.py
--rw-r--r--   0        0        0     4849 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/classes/sessionbuilder.py
--rw-r--r--   0        0        0    29784 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/classes/table.py
--rw-r--r--   0        0        0    14816 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/commands/check.py
--rw-r--r--   0        0        0     5347 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/commands/manual.py
--rwxr-xr-x   0        0        0    15354 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/commands/scraper.py
--rw-r--r--   0        0        0     7246 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/constants.py
--rw-r--r--   0        0        0        1 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/db/__init__.py
--rw-r--r--   0        0        0    10129 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/db/operations.py
--rw-r--r--   0        0        0     3576 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/db/queries.py
--rw-r--r--   0        0        0        1 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/interaction/__init__.py
--rw-r--r--   0        0        0     4851 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/interaction/like.py
--rw-r--r--   0        0        0      773 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/prompts/keybindings.py
--rw-r--r--   0        0        0     6241 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/prompts/promptConvert.py
--rw-r--r--   0        0        0     7227 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/prompts/prompt_strings.py
--rw-r--r--   0        0        0     7848 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/prompts/prompt_validators.py
--rw-r--r--   0        0        0    30812 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/prompts/prompts.py
--rw-r--r--   0        0        0     3430 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/start.py
--rw-r--r--   0        0        0        1 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/utils/__init__.py
--rw-r--r--   0        0        0    14095 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/utils/args.py
--rw-r--r--   0        0        0    10632 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/utils/auth.py
--rw-r--r--   0        0        0     8977 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/utils/binaries.py
--rw-r--r--   0        0        0    14736 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/utils/config.py
--rw-r--r--   0        0        0      395 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/utils/console.py
--rw-r--r--   0        0        0     1080 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/utils/dates.py
--rw-r--r--   0        0        0    41373 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/utils/download.py
--rw-r--r--   0        0        0      609 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/utils/encoding.py
--rw-r--r--   0        0        0     3386 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/utils/exit.py
--rw-r--r--   0        0        0     5665 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/utils/filters.py
--rw-r--r--   0        0        0    11133 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/utils/logger.py
--rw-r--r--   0        0        0      189 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/utils/misc.py
--rw-r--r--   0        0        0    10913 2023-08-07 13:27:44.379449 ofscraper-3.0.5/ofscraper/utils/of.py
--rw-r--r--   0        0        0     7251 2023-08-07 13:27:44.383449 ofscraper-3.0.5/ofscraper/utils/paths.py
--rw-r--r--   0        0        0     4221 2023-08-07 13:27:44.383449 ofscraper-3.0.5/ofscraper/utils/profiles.py
--rw-r--r--   0        0        0      399 2023-08-07 13:27:44.383449 ofscraper-3.0.5/ofscraper/utils/semaphoreDelayed.py
--rw-r--r--   0        0        0     1215 2023-08-07 13:27:44.383449 ofscraper-3.0.5/ofscraper/utils/separate.py
--rw-r--r--   0        0        0      893 2023-08-07 13:27:44.383449 ofscraper-3.0.5/ofscraper/utils/stdout.py
--rw-r--r--   0        0        0     5773 2023-08-07 13:27:44.383449 ofscraper-3.0.5/ofscraper/utils/userselector.py
--rw-r--r--   0        0        0     2073 2023-08-07 13:28:22.887609 ofscraper-3.0.5/pyproject.toml
--rw-r--r--   0        0        0     4720 1970-01-01 00:00:00.000000 ofscraper-3.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-07 21:53:00.131458 ofscraper-3.0.6/LICENSE
+-rw-r--r--   0        0        0     2863 2023-08-07 21:53:00.131458 ofscraper-3.0.6/README.md
+-rwxr-xr-x   0        0        0      291 2023-08-07 21:53:00.139458 ofscraper-3.0.6/ofscraper/__main__.py
+-rw-r--r--   0        0        0     1016 2023-08-07 21:53:00.139458 ofscraper-3.0.6/ofscraper/__version__.py
+-rw-r--r--   0        0        0      999 2023-08-07 21:53:00.139458 ofscraper-3.0.6/ofscraper/__version__.pye
+-rw-r--r--   0        0        0     8736 2023-08-07 21:53:00.139458 ofscraper-3.0.6/ofscraper/api/archive.py
+-rw-r--r--   0        0        0     9895 2023-08-07 21:53:00.139458 ofscraper-3.0.6/ofscraper/api/highlights.py
+-rw-r--r--   0        0        0     1029 2023-08-07 21:53:00.139458 ofscraper-3.0.6/ofscraper/api/init.py
+-rw-r--r--   0        0        0     7568 2023-08-07 21:53:00.139458 ofscraper-3.0.6/ofscraper/api/labels.py
+-rw-r--r--   0        0        0     2946 2023-08-07 21:53:00.139458 ofscraper-3.0.6/ofscraper/api/me.py
+-rw-r--r--   0        0        0     9518 2023-08-07 21:53:00.139458 ofscraper-3.0.6/ofscraper/api/messages.py
+-rw-r--r--   0        0        0     9687 2023-08-07 21:53:00.139458 ofscraper-3.0.6/ofscraper/api/paid.py
+-rw-r--r--   0        0        0     5730 2023-08-07 21:53:00.139458 ofscraper-3.0.6/ofscraper/api/pinned.py
+-rw-r--r--   0        0        0     4497 2023-08-07 21:53:00.139458 ofscraper-3.0.6/ofscraper/api/profile.py
+-rw-r--r--   0        0        0     3384 2023-08-07 21:53:00.139458 ofscraper-3.0.6/ofscraper/api/subscriptions.py
+-rw-r--r--   0        0        0     9312 2023-08-07 21:53:00.139458 ofscraper-3.0.6/ofscraper/api/timeline.py
+-rw-r--r--   0        0        0      804 2023-08-07 21:53:00.139458 ofscraper-3.0.6/ofscraper/classes/labels.py
+-rw-r--r--   0        0        0     8779 2023-08-07 21:53:00.139458 ofscraper-3.0.6/ofscraper/classes/media.py
+-rw-r--r--   0        0        0     1795 2023-08-07 21:53:00.139458 ofscraper-3.0.6/ofscraper/classes/multiprocessprogress.py
+-rw-r--r--   0        0        0     8068 2023-08-07 21:53:00.139458 ofscraper-3.0.6/ofscraper/classes/placeholder.py
+-rw-r--r--   0        0        0     3734 2023-08-07 21:53:00.139458 ofscraper-3.0.6/ofscraper/classes/posts.py
+-rw-r--r--   0        0        0     4849 2023-08-07 21:53:00.139458 ofscraper-3.0.6/ofscraper/classes/sessionbuilder.py
+-rw-r--r--   0        0        0    29784 2023-08-07 21:53:00.139458 ofscraper-3.0.6/ofscraper/classes/table.py
+-rw-r--r--   0        0        0    14816 2023-08-07 21:53:00.139458 ofscraper-3.0.6/ofscraper/commands/check.py
+-rw-r--r--   0        0        0     5347 2023-08-07 21:53:00.139458 ofscraper-3.0.6/ofscraper/commands/manual.py
+-rwxr-xr-x   0        0        0    15354 2023-08-07 21:53:00.139458 ofscraper-3.0.6/ofscraper/commands/scraper.py
+-rw-r--r--   0        0        0     7246 2023-08-07 21:53:00.139458 ofscraper-3.0.6/ofscraper/constants.py
+-rw-r--r--   0        0        0        1 2023-08-07 21:53:00.139458 ofscraper-3.0.6/ofscraper/db/__init__.py
+-rw-r--r--   0        0        0    10129 2023-08-07 21:53:00.139458 ofscraper-3.0.6/ofscraper/db/operations.py
+-rw-r--r--   0        0        0     3576 2023-08-07 21:53:00.139458 ofscraper-3.0.6/ofscraper/db/queries.py
+-rw-r--r--   0        0        0        1 2023-08-07 21:53:00.139458 ofscraper-3.0.6/ofscraper/interaction/__init__.py
+-rw-r--r--   0        0        0     4851 2023-08-07 21:53:00.139458 ofscraper-3.0.6/ofscraper/interaction/like.py
+-rw-r--r--   0        0        0      773 2023-08-07 21:53:00.139458 ofscraper-3.0.6/ofscraper/prompts/keybindings.py
+-rw-r--r--   0        0        0     6241 2023-08-07 21:53:00.139458 ofscraper-3.0.6/ofscraper/prompts/promptConvert.py
+-rw-r--r--   0        0        0     7227 2023-08-07 21:53:00.139458 ofscraper-3.0.6/ofscraper/prompts/prompt_strings.py
+-rw-r--r--   0        0        0     7848 2023-08-07 21:53:00.143458 ofscraper-3.0.6/ofscraper/prompts/prompt_validators.py
+-rw-r--r--   0        0        0    30812 2023-08-07 21:53:00.143458 ofscraper-3.0.6/ofscraper/prompts/prompts.py
+-rw-r--r--   0        0        0     3752 2023-08-07 21:53:00.143458 ofscraper-3.0.6/ofscraper/start.py
+-rw-r--r--   0        0        0        1 2023-08-07 21:53:00.143458 ofscraper-3.0.6/ofscraper/utils/__init__.py
+-rw-r--r--   0        0        0    14095 2023-08-07 21:53:00.143458 ofscraper-3.0.6/ofscraper/utils/args.py
+-rw-r--r--   0        0        0    10673 2023-08-07 21:53:00.143458 ofscraper-3.0.6/ofscraper/utils/auth.py
+-rw-r--r--   0        0        0     8977 2023-08-07 21:53:00.143458 ofscraper-3.0.6/ofscraper/utils/binaries.py
+-rw-r--r--   0        0        0    14736 2023-08-07 21:53:00.143458 ofscraper-3.0.6/ofscraper/utils/config.py
+-rw-r--r--   0        0        0      395 2023-08-07 21:53:00.143458 ofscraper-3.0.6/ofscraper/utils/console.py
+-rw-r--r--   0        0        0     1080 2023-08-07 21:53:00.143458 ofscraper-3.0.6/ofscraper/utils/dates.py
+-rw-r--r--   0        0        0    41393 2023-08-07 21:53:00.143458 ofscraper-3.0.6/ofscraper/utils/download.py
+-rw-r--r--   0        0        0      609 2023-08-07 21:53:00.143458 ofscraper-3.0.6/ofscraper/utils/encoding.py
+-rw-r--r--   0        0        0     3386 2023-08-07 21:53:00.143458 ofscraper-3.0.6/ofscraper/utils/exit.py
+-rw-r--r--   0        0        0     5665 2023-08-07 21:53:00.143458 ofscraper-3.0.6/ofscraper/utils/filters.py
+-rw-r--r--   0        0        0    11133 2023-08-07 21:53:00.143458 ofscraper-3.0.6/ofscraper/utils/logger.py
+-rw-r--r--   0        0        0      189 2023-08-07 21:53:00.143458 ofscraper-3.0.6/ofscraper/utils/misc.py
+-rw-r--r--   0        0        0    10913 2023-08-07 21:53:00.143458 ofscraper-3.0.6/ofscraper/utils/of.py
+-rw-r--r--   0        0        0     7251 2023-08-07 21:53:00.143458 ofscraper-3.0.6/ofscraper/utils/paths.py
+-rw-r--r--   0        0        0     4221 2023-08-07 21:53:00.143458 ofscraper-3.0.6/ofscraper/utils/profiles.py
+-rw-r--r--   0        0        0      399 2023-08-07 21:53:00.143458 ofscraper-3.0.6/ofscraper/utils/semaphoreDelayed.py
+-rw-r--r--   0        0        0     1215 2023-08-07 21:53:00.143458 ofscraper-3.0.6/ofscraper/utils/separate.py
+-rw-r--r--   0        0        0      893 2023-08-07 21:53:00.143458 ofscraper-3.0.6/ofscraper/utils/stdout.py
+-rw-r--r--   0        0        0     5773 2023-08-07 21:53:00.143458 ofscraper-3.0.6/ofscraper/utils/userselector.py
+-rw-r--r--   0        0        0     2073 2023-08-07 21:53:32.303791 ofscraper-3.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4720 1970-01-01 00:00:00.000000 ofscraper-3.0.6/PKG-INFO
```

### Comparing `ofscraper-3.0.5/LICENSE` & `ofscraper-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/README.md` & `ofscraper-3.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/__version__.py` & `ofscraper-3.0.6/ofscraper/__version__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/__version__.pye` & `ofscraper-3.0.6/ofscraper/__version__.pye`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/api/archive.py` & `ofscraper-3.0.6/ofscraper/api/archive.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/api/highlights.py` & `ofscraper-3.0.6/ofscraper/api/highlights.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/api/init.py` & `ofscraper-3.0.6/ofscraper/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/api/labels.py` & `ofscraper-3.0.6/ofscraper/api/labels.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/api/me.py` & `ofscraper-3.0.6/ofscraper/api/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/api/messages.py` & `ofscraper-3.0.6/ofscraper/api/messages.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/api/paid.py` & `ofscraper-3.0.6/ofscraper/api/paid.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/api/pinned.py` & `ofscraper-3.0.6/ofscraper/api/pinned.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/api/profile.py` & `ofscraper-3.0.6/ofscraper/api/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/api/subscriptions.py` & `ofscraper-3.0.6/ofscraper/api/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/api/timeline.py` & `ofscraper-3.0.6/ofscraper/api/timeline.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/classes/labels.py` & `ofscraper-3.0.6/ofscraper/classes/labels.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/classes/media.py` & `ofscraper-3.0.6/ofscraper/classes/media.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/classes/multiprocessprogress.py` & `ofscraper-3.0.6/ofscraper/classes/multiprocessprogress.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/classes/placeholder.py` & `ofscraper-3.0.6/ofscraper/classes/placeholder.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/classes/posts.py` & `ofscraper-3.0.6/ofscraper/classes/posts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/classes/sessionbuilder.py` & `ofscraper-3.0.6/ofscraper/classes/sessionbuilder.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/classes/table.py` & `ofscraper-3.0.6/ofscraper/classes/table.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/commands/check.py` & `ofscraper-3.0.6/ofscraper/commands/check.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/commands/manual.py` & `ofscraper-3.0.6/ofscraper/commands/manual.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/commands/scraper.py` & `ofscraper-3.0.6/ofscraper/commands/scraper.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/constants.py` & `ofscraper-3.0.6/ofscraper/constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/db/operations.py` & `ofscraper-3.0.6/ofscraper/db/operations.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/db/queries.py` & `ofscraper-3.0.6/ofscraper/db/queries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/interaction/like.py` & `ofscraper-3.0.6/ofscraper/interaction/like.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/prompts/keybindings.py` & `ofscraper-3.0.6/ofscraper/prompts/keybindings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/prompts/promptConvert.py` & `ofscraper-3.0.6/ofscraper/prompts/promptConvert.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/prompts/prompt_strings.py` & `ofscraper-3.0.6/ofscraper/prompts/prompt_strings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/prompts/prompt_validators.py` & `ofscraper-3.0.6/ofscraper/prompts/prompt_validators.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/prompts/prompts.py` & `ofscraper-3.0.6/ofscraper/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/start.py` & `ofscraper-3.0.6/ofscraper/start.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+
 import sys
+import os
 import time
 import ssl
 import platform
 import certifi
+import multiprocessing
 from threading import Event
 import ofscraper.utils.logger as logger
 import ofscraper.utils.args as args_
 import ofscraper.commands.scraper as scraper
 import ofscraper.commands.check as check
 import ofscraper.commands.manual as manual
 import ofscraper.utils.config as config_
@@ -79,21 +82,28 @@
     args=args_.getargs()
     log=logger.get_shared_logger()
     logger.updateSenstiveDict(f"/{paths_.get_username()}/","/your_username/")
     logger.updateSenstiveDict(f"\\{paths_.get_username()}\\","\\\\your_username\\\\")
 
     #print info
     log.debug(args)
+    log.debug(platform.platform())
     log.debug(config_.read_config())
     log.info(f"config path: {str(paths_.get_config_path())}")
     log.info(f"profile path: {str(paths_.get_profile_path())}")
     log.info(f"log folder: {str(paths_.get_config_home()/'logging')}")
     log.debug(f"ssl {ssl.get_default_verify_paths()}")
     log.debug(f"python version {platform. python_version()}" )
     log.debug(f"certifi {certifi.where()}")
 
 def discord_warning():
     if args_.getargs().discord=="DEBUG":
         console_.get_shared_console().print("[bold red]Warning Discord with DEBUG is not recommended\nAs processing messages is much slower compared to other[/bold red]")
 
 
-
+def set_mulitproc_start_type():
+    plat=platform.system()
+    if plat == "Darwin" or plat=="Windows":
+        multiprocessing.set_start_method('spawn')
+        os.environ['no_proxy'] = '*'
+    else:
+        multiprocessing.set_startDarwin_method('fork')
```

### Comparing `ofscraper-3.0.5/ofscraper/utils/args.py` & `ofscraper-3.0.6/ofscraper/utils/args.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/utils/auth.py` & `ofscraper-3.0.6/ofscraper/utils/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,14 +150,15 @@
     else:
         console.print("You'll need to go to onlyfans.com and retrive header information\nGo to https://github.com/datawhores/OF-Scraper and find the section named 'Getting Your Auth Info'\nYou only need to retrive the x-bc header,the user-agent, and cookie information",style="yellow")
         auth['auth'].update(prompts.auth_prompt(auth['auth']))
     for key,item in auth["auth"].items():
         newitem=item.strip()
         newitem=re.sub("^ +","",newitem)
         newitem=re.sub(" +$","",newitem)
+        newitem=re.sub("\n+","",newitem)
         auth["auth"][key]=newitem
     console.print(f"{auth}\nWriting to {authFile}",style="yellow")
     with open(authFile, 'w') as f:
         f.write(json.dumps(auth, indent=4))
```

### Comparing `ofscraper-3.0.5/ofscraper/utils/binaries.py` & `ofscraper-3.0.6/ofscraper/utils/binaries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/utils/config.py` & `ofscraper-3.0.6/ofscraper/utils/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/utils/dates.py` & `ofscraper-3.0.6/ofscraper/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/utils/download.py` & `ofscraper-3.0.6/ofscraper/utils/download.py`

 * *Files 0% similar despite different names*

```diff
@@ -853,14 +853,15 @@
         cache.set(ele.postid ,True)
         cache.close()
 
 
 def addGlobalDir(path):
     dirSet.add(path.resolve().parent)
 def setDirectoriesDate():
+    global dir_lock
     split_log.info( f" {pid_log_helper()} Setting Date for modified directories")
     output=set()
     rootDir=pathlib.Path(config_.get_save_location(config_.read_config())).resolve()
     for ele in dirSet:
         output.add(ele)
         while ele!=rootDir and ele.parent!=rootDir:
             split_log.debug(f"{pid_log_helper()} Setting Dates ele:{ele} rootDir:{rootDir}")
```

### Comparing `ofscraper-3.0.5/ofscraper/utils/encoding.py` & `ofscraper-3.0.6/ofscraper/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/utils/exit.py` & `ofscraper-3.0.6/ofscraper/utils/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/utils/filters.py` & `ofscraper-3.0.6/ofscraper/utils/filters.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/utils/logger.py` & `ofscraper-3.0.6/ofscraper/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/utils/of.py` & `ofscraper-3.0.6/ofscraper/utils/of.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/utils/paths.py` & `ofscraper-3.0.6/ofscraper/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/utils/profiles.py` & `ofscraper-3.0.6/ofscraper/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/utils/separate.py` & `ofscraper-3.0.6/ofscraper/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/utils/stdout.py` & `ofscraper-3.0.6/ofscraper/utils/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/ofscraper/utils/userselector.py` & `ofscraper-3.0.6/ofscraper/utils/userselector.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.0.5/pyproject.toml` & `ofscraper-3.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "3.0.5"
+version = "3.0.6"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">3.7.0,<3.12"
 httpx = {extras = ["http2"], version = "^0.23.3"}
```

### Comparing `ofscraper-3.0.5/PKG-INFO` & `ofscraper-3.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 3.0.5
+Version: 3.0.6
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >3.7.0,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

