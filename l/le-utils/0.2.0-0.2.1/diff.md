# Comparing `tmp/le-utils-0.2.0.tar.gz` & `tmp/le-utils-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/le-utils-0.2.0.tar", last modified: Mon Jun 12 04:14:36 2023, max compression
+gzip compressed data, was "le-utils-0.2.1.tar", last modified: Tue Aug  8 16:42:25 2023, max compression
```

## Comparing `le-utils-0.2.0.tar` & `le-utils-0.2.1.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 04:14:36.000000 le-utils-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-12 04:14:19.000000 le-utils-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-06-12 04:14:19.000000 le-utils-0.2.0/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 04:14:36.000000 le-utils-0.2.0/le_utils/
--rw-r--r--   0 runner    (1001) docker     (122)     7165 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/humanhash.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 04:14:36.000000 le-utils-0.2.0/le_utils/constants/
--rw-r--r--   0 runner    (1001) docker     (122)     4532 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/constants/format_presets.py
--rw-r--r--   0 runner    (1001) docker     (122)     2631 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/constants/file_formats.py
--rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/constants/file_types.py
--rw-r--r--   0 runner    (1001) docker     (122)      369 2023-06-12 04:14:34.000000 le-utils-0.2.0/le_utils/constants/modalities.py
--rw-r--r--   0 runner    (1001) docker     (122)     1393 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/constants/content_kinds.py
--rw-r--r--   0 runner    (1001) docker     (122)     9300 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/constants/languages.py
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/constants/exercises.py
--rw-r--r--   0 runner    (1001) docker     (122)      126 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/constants/roles.py
--rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/constants/licenses.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1982 2023-06-12 04:14:34.000000 le-utils-0.2.0/le_utils/constants/completion_criteria.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 04:14:36.000000 le-utils-0.2.0/le_utils/constants/labels/
--rw-r--r--   0 runner    (1001) docker     (122)     5735 2023-06-12 04:14:34.000000 le-utils-0.2.0/le_utils/constants/labels/subjects.py
--rw-r--r--   0 runner    (1001) docker     (122)      873 2023-06-12 04:14:34.000000 le-utils-0.2.0/le_utils/constants/labels/levels.py
--rw-r--r--   0 runner    (1001) docker     (122)      574 2023-06-12 04:14:34.000000 le-utils-0.2.0/le_utils/constants/labels/learning_activities.py
--rw-r--r--   0 runner    (1001) docker     (122)      696 2023-06-12 04:14:34.000000 le-utils-0.2.0/le_utils/constants/labels/accessibility_categories.py
--rw-r--r--   0 runner    (1001) docker     (122)      955 2023-06-12 04:14:34.000000 le-utils-0.2.0/le_utils/constants/labels/needs.py
--rw-r--r--   0 runner    (1001) docker     (122)      212 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/constants/labels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      752 2023-06-12 04:14:34.000000 le-utils-0.2.0/le_utils/constants/labels/resource_type.py
--rw-r--r--   0 runner    (1001) docker     (122)     1750 2023-06-12 04:14:34.000000 le-utils-0.2.0/le_utils/constants/mastery_criteria.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 04:14:36.000000 le-utils-0.2.0/le_utils/resources/
--rw-r--r--   0 runner    (1001) docker     (122)     8183 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/resources/presetlookup.json
--rw-r--r--   0 runner    (1001) docker     (122)      347 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/resources/kindlookup.json
--rw-r--r--   0 runner    (1001) docker     (122)    21338 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/resources/languagelookup.json
--rw-r--r--   0 runner    (1001) docker     (122)     1483 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/resources/licenselookup.json
--rw-r--r--   0 runner    (1001) docker     (122)      710 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/resources/formatlookup.json
--rw-r--r--   0 runner    (1001) docker     (122)     2851 2023-06-12 04:14:19.000000 le-utils-0.2.0/le_utils/proquint.py
--rw-r--r--   0 runner    (1001) docker     (122)    12733 2023-06-12 04:14:36.000000 le-utils-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      260 2023-06-12 04:14:36.000000 le-utils-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1226 2023-06-12 04:14:19.000000 le-utils-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-12 04:14:36.000000 le-utils-0.2.0/le_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-12 04:14:36.000000 le-utils-0.2.0/le_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-12 04:14:36.000000 le-utils-0.2.0/le_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    12733 2023-06-12 04:14:36.000000 le-utils-0.2.0/le_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1163 2023-06-12 04:14:36.000000 le-utils-0.2.0/le_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-06-12 04:14:36.000000 le-utils-0.2.0/le_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)    10228 2023-06-12 04:14:19.000000 le-utils-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:42:25.175387 le-utils-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-08 16:41:50.000000 le-utils-0.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-08 16:41:50.000000 le-utils-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-08-08 16:42:25.175387 le-utils-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10228 2023-08-08 16:41:50.000000 le-utils-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:42:25.171386 le-utils-0.2.1/le_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:41:50.000000 le-utils-0.2.1/le_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:42:25.175387 le-utils-0.2.1/le_utils/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 16:41:50.000000 le-utils-0.2.1/le_utils/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-08-08 16:42:24.000000 le-utils-0.2.1/le_utils/constants/completion_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-08-08 16:41:50.000000 le-utils-0.2.1/le_utils/constants/content_kinds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-08-08 16:41:50.000000 le-utils-0.2.1/le_utils/constants/exercises.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-08-08 16:41:50.000000 le-utils-0.2.1/le_utils/constants/file_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-08 16:41:50.000000 le-utils-0.2.1/le_utils/constants/file_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-08-08 16:41:50.000000 le-utils-0.2.1/le_utils/constants/format_presets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:42:25.175387 le-utils-0.2.1/le_utils/constants/labels/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-08 16:41:50.000000 le-utils-0.2.1/le_utils/constants/labels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-08 16:42:06.000000 le-utils-0.2.1/le_utils/constants/labels/accessibility_categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-08-08 16:42:06.000000 le-utils-0.2.1/le_utils/constants/labels/learning_activities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-08-08 16:42:06.000000 le-utils-0.2.1/le_utils/constants/labels/levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-08 16:42:06.000000 le-utils-0.2.1/le_utils/constants/labels/needs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-08-08 16:42:06.000000 le-utils-0.2.1/le_utils/constants/labels/resource_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-08-08 16:42:24.000000 le-utils-0.2.1/le_utils/constants/labels/subjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-08-08 16:41:50.000000 le-utils-0.2.1/le_utils/constants/languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-08-08 16:41:50.000000 le-utils-0.2.1/le_utils/constants/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-08-08 16:42:24.000000 le-utils-0.2.1/le_utils/constants/mastery_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-08 16:42:06.000000 le-utils-0.2.1/le_utils/constants/modalities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-08 16:41:50.000000 le-utils-0.2.1/le_utils/constants/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-08 16:42:24.000000 le-utils-0.2.1/le_utils/constants/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-08-08 16:41:50.000000 le-utils-0.2.1/le_utils/humanhash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-08-08 16:41:50.000000 le-utils-0.2.1/le_utils/proquint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:42:25.175387 le-utils-0.2.1/le_utils/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-08 16:41:50.000000 le-utils-0.2.1/le_utils/resources/formatlookup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-08 16:41:50.000000 le-utils-0.2.1/le_utils/resources/kindlookup.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21338 2023-08-08 16:41:50.000000 le-utils-0.2.1/le_utils/resources/languagelookup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-08-08 16:41:50.000000 le-utils-0.2.1/le_utils/resources/licenselookup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-08-08 16:41:50.000000 le-utils-0.2.1/le_utils/resources/presetlookup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-08-08 16:41:50.000000 le-utils-0.2.1/le_utils/uuidv5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 16:42:25.175387 le-utils-0.2.1/le_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11028 2023-08-08 16:42:25.000000 le-utils-0.2.1/le_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-08 16:42:25.000000 le-utils-0.2.1/le_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 16:42:25.000000 le-utils-0.2.1/le_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-08 16:42:25.000000 le-utils-0.2.1/le_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 16:42:25.000000 le-utils-0.2.1/le_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-08 16:42:25.175387 le-utils-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-08-08 16:41:50.000000 le-utils-0.2.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `le-utils-0.2.0/LICENSE.txt` & `le-utils-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `le-utils-0.2.0/le_utils/humanhash.py` & `le-utils-0.2.1/le_utils/humanhash.py`

 * *Files identical despite different names*

### Comparing `le-utils-0.2.0/le_utils/constants/format_presets.py` & `le-utils-0.2.1/le_utils/constants/format_presets.py`

 * *Files identical despite different names*

### Comparing `le-utils-0.2.0/le_utils/constants/file_formats.py` & `le-utils-0.2.1/le_utils/constants/file_formats.py`

 * *Files identical despite different names*

### Comparing `le-utils-0.2.0/le_utils/constants/file_types.py` & `le-utils-0.2.1/le_utils/constants/file_types.py`

 * *Files identical despite different names*

### Comparing `le-utils-0.2.0/le_utils/constants/content_kinds.py` & `le-utils-0.2.1/le_utils/constants/content_kinds.py`

 * *Files identical despite different names*

### Comparing `le-utils-0.2.0/le_utils/constants/languages.py` & `le-utils-0.2.1/le_utils/constants/languages.py`

 * *Files identical despite different names*

### Comparing `le-utils-0.2.0/le_utils/constants/exercises.py` & `le-utils-0.2.1/le_utils/constants/exercises.py`

 * *Files identical despite different names*

### Comparing `le-utils-0.2.0/le_utils/constants/licenses.py` & `le-utils-0.2.1/le_utils/constants/licenses.py`

 * *Files identical despite different names*

### Comparing `le-utils-0.2.0/le_utils/constants/labels/subjects.py` & `le-utils-0.2.1/le_utils/constants/labels/subjects.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,15 +82,18 @@
     (DRAMA, "Drama"),
     (EARTH_SCIENCE, "Earth Science"),
     (ENTREPRENEURSHIP, "Entrepreneurship"),
     (ENVIRONMENT, "Environment"),
     (FINANCIAL_LITERACY, "Financial Literacy"),
     (FOR_TEACHERS, "For Teachers"),
     (FOUNDATIONS, "Foundations"),
-    (FOUNDATIONS_LOGIC_AND_CRITICAL_THINKING, "Foundations Logic And Critical Thinking"),
+    (
+        FOUNDATIONS_LOGIC_AND_CRITICAL_THINKING,
+        "Foundations Logic And Critical Thinking",
+    ),
     (GEOMETRY, "Geometry"),
     (GUIDES, "Guides"),
     (HISTORY, "History"),
     (INDUSTRY_AND_SECTOR_SPECIFIC, "Industry And Sector Specific"),
     (LANGUAGE_LEARNING, "Language Learning"),
     (LEARNING_SKILLS, "Learning Skills"),
     (LESSON_PLANS, "Lesson Plans"),
```

### Comparing `le-utils-0.2.0/le_utils/constants/labels/levels.py` & `le-utils-0.2.1/le_utils/constants/labels/levels.py`

 * *Files identical despite different names*

### Comparing `le-utils-0.2.0/le_utils/constants/labels/learning_activities.py` & `le-utils-0.2.1/le_utils/constants/labels/learning_activities.py`

 * *Files identical despite different names*

### Comparing `le-utils-0.2.0/le_utils/constants/labels/accessibility_categories.py` & `le-utils-0.2.1/le_utils/constants/labels/accessibility_categories.py`

 * *Files identical despite different names*

### Comparing `le-utils-0.2.0/le_utils/constants/labels/needs.py` & `le-utils-0.2.1/le_utils/constants/labels/needs.py`

 * *Files identical despite different names*

### Comparing `le-utils-0.2.0/le_utils/constants/labels/resource_type.py` & `le-utils-0.2.1/le_utils/constants/labels/resource_type.py`

 * *Files identical despite different names*

### Comparing `le-utils-0.2.0/le_utils/resources/presetlookup.json` & `le-utils-0.2.1/le_utils/resources/presetlookup.json`

 * *Files identical despite different names*

### Comparing `le-utils-0.2.0/le_utils/resources/languagelookup.json` & `le-utils-0.2.1/le_utils/resources/languagelookup.json`

 * *Files identical despite different names*

### Comparing `le-utils-0.2.0/le_utils/resources/licenselookup.json` & `le-utils-0.2.1/le_utils/resources/licenselookup.json`

 * *Files identical despite different names*

### Comparing `le-utils-0.2.0/le_utils/resources/formatlookup.json` & `le-utils-0.2.1/le_utils/resources/formatlookup.json`

 * *Files identical despite different names*

### Comparing `le-utils-0.2.0/le_utils/proquint.py` & `le-utils-0.2.1/le_utils/proquint.py`

 * *Files identical despite different names*

### Comparing `le-utils-0.2.0/PKG-INFO` & `le-utils-0.2.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,234 +1,237 @@
 Metadata-Version: 2.1
 Name: le-utils
-Version: 0.2.0
+Version: 0.2.1
 Summary: LE-Utils contains shared constants used in Kolibri, Ricecooker, and Kolibri Studio.
 Home-page: https://github.com/learningequality/le-utils
 Author: Learning Equality
 Author-email: info@learningequality.org
 License: MIT
 Download-URL: https://github.com/learningequality/le-utils/releases
-Description: LE Utils
-        ========
-        The `le-utils` package contains shared constants used by Ricecooker, Kolibri, and
-        Kolibri Studio. This package is not meant to be installed or used directly, but
-        plays an important role in all Learning Equality products.
-        
-        
-        Constants
-        =========
-        The Python files in the [le_utils/constants/](./le_utils/constants) are used to
-        define constants (usually in `ALL_CAPS` form) to be used from Python code.
-        The same constants and naming conventions are also provided in JSON format in the
-        folder [le_utils/resources/](le_utils/resources) for use in frontend code.
-        This means, adding a new constant may require editing multiple files: the Python
-        constant-defining file, the JSON-file, and any associated tests.
-        
-        
-        Languages
-        ---------
-        The file [le_utils/constants/languages.py](./le_utils/constants/languages.py) and
-        the lookup table in [le_utils/resources/languagelookup.json](./le_utils/resources/languagelookup.json)
-        define the internal representation for languages codes used by Ricecooker, Kolibri,
-        and Kolibri Studio to identify educational content in different languages.
-        
-        The internal representation uses a mixture of two-letter codes (e.g. `en`),
-        two-letter-and-country code (e.g. `pt-BR` for Brazilian Portuguese),
-        and three-letter codes (e.g., `zul` for Zulu).
-        
-        In order to make sure you have the correct language code when interfacing with
-        the Kolibri ecosystem (e.g. when uploading new content to Kolibri Studio), you
-        must lookup the language object using the helper method `getlang`:
-        
-        ```
-        >>> from le_utils.constants.languages import getlang
-        >>> language_obj = getlang('en')       # lookup language using language code
-        >>> language_obj
-        Language(native_name='English', primary_code='en', subcode=None, name='English', ka_name=None)
-        ```
-        The function `getlang` will return `None` if the lookup fails. In such cases, you
-        can try lookup by name or lookup by alpha2 code (ISO_639-1) methods defined below.
-        
-        Once you've successfully looked up the language object, you can obtain the internal
-        representation language code from the language object's `code` attribute:
-        ```
-        >>> language_obj.code
-        'en'
-        ```
-        The Ricecooker API expects these internal representation language codes will be
-        supplied for all `language` attributes (channel language, node language, and files language).
-        
-        
-        
-        ### More lookup helper methods
-        The helper method `getlang_by_name` allows you to lookup a language by name:
-        ```
-        >>> from le_utils.constants.languages import getlang_by_name
-        >>> language_obj = getlang_by_name('English')  # lookup language by name
-        >>> language_obj
-        Language(native_name='English', primary_code='en', subcode=None, name='English', ka_name=None)
-        ```
-        
-        The module `le_utils.constants.languages` defines two other language lookup methods:
-          - Use `getlang_by_native_name` for lookup up names by native language name,
-            e.g., you look for 'Français' to find French.
-         -  Use `getlang_by_alpha2` to perform lookups using the standard two-letter codes
-            defined in [ISO_639-1](https://en.wikipedia.org/wiki/ISO_639-1) that are
-            supported by the `pycountries` library.
-        
-        
-        #### Useful links
-        
-        The following websites are useful for researching language codes:
-        
-          - https://www.ethnologue.com/
-          - https://en.wikipedia.org/wiki/List_of_ISO_639-2_codes
-        
-        
-        
-        Licenses
-        --------
-        All content nodes within Kolibri and Kolibri Studio must have a license. The file
-        [le_utils/constants/licenses.py](./le_utils/constants/licenses.py) contains the
-        constants used to identify the license types. These constants are meant to be
-        used in conjunction with the helper method `ricecooker.classes.licenses.get_license`
-        to create `Licence` objects.
-        
-        To initialize a license object, you must specify the license type and the
-        `copyright_holder` (str) which identifies a person or an organization. For example:
-        ```
-        from ricecooker.classes.licenses import get_license
-        from le_utils.constants import licenses
-        license = get_license(licenses.CC_BY, copyright_holder="Khan Academy")
-        ```
-        
-        Note: The `copyright_holder` field is required for all License types except for
-        the public domain license for which `copyright_holder` can be None.
-        
-        
-        
-        
-        Content kinds (ContentNode subclasses)
-        --------------------------------------
-        Content items throughout the Kolibri ecosystem come in several kinds. The `kind`
-        attribute of each object can be one of ("topic", "video", "audio", "exercise"
-        "document", or "html5".
-        See [constants/content_kinds.py](https://github.com/learningequality/le-utils/blob/master/le_utils/constants/content_kinds.py#L11-L17) for latest list.
-        
-        The currently supported content kinds are:
-          - Topic node (folder)
-          - Video content nodes backed by a video files and subtitles
-          - Audio content nodes backed by an audio files
-          - Document content nodes backed by a document files (PDF or ePub)
-          - HTML5 app content nodes backed by a HTML5 zip files
-          - Slideshow content nodes
-          - Exercise content nodes
-        
-        The `kind` attribute identifies a subclass of the base content node class within
-        the data model, which differs on Ricecooker, Studio, and Kolibri:
-          - [ricecooker.classes.nodes.ContentNode](https://github.com/learningequality/ricecooker/blob/master/ricecooker/classes/nodes.py#L428-L506):
-            in-memory content node used to store metadata needed to upload new content to Kolibri  Studio
-          - [contentcuration.contentcuration.models.ContentNode](https://github.com/learningequality/studio/blob/develop/contentcuration/contentcuration/models.py#L775):
-            node within one of the trees associated with a Kolibri Studio channel.
-          - [kolibri.core.content.models.ContentNode](https://github.com/learningequality/kolibri/blob/develop/kolibri/core/content/models.py#L175):
-            node within tree for a particular version of a channel on Kolibri.
-        
-        For a detailed description of the common and different model attributes available
-        on content nodes in each part of the platform see [this doc](https://docs.google.com/spreadsheets/d/181hSEwJ7yVmMh7LEwaHENqQetYSsbSDwybHTO_0zZM0/edit#gid=1640972430).
-        
-        
-        
-        File formats (extensions)
-        -------------------------
-        These are low-level constant that represents what type of file and are essentially
-        synonymous with file extensions. The file format `MP4` is simply a convenient
-        proxy for the file extension `mp4`.
-        See [file_formats.py](https://github.com/learningequality/le-utils/blob/master/le_utils/constants/file_formats.py)
-        and [resourcces/formatlookup.json](https://github.com/nucleogenesis/le-utils/blob/master/le_utils/resources/formatlookup.json).
-        
-        
-        
-        Format presets (ContentNode-File relation)
-        ------------------------------------------
-        Every `ContentNode` is associated with one or more `File` objects and nature of
-        this association is represented though the `format_preset` attribute of the file.
-        The `format_preset` is the role the file is playing in the content node,
-        e.g., thumbnail, high resolution video, or low resolution video.
-        Note that format presets are represented redundantly as python string in
-        [constants/format_presets.py](https://github.com/learningequality/le-utils/blob/master/le_utils/constants/format_presets.py)
-        and as json [resources/presetlookup.json](https://github.com/learningequality/le-utils/blob/master/le_utils/resources/presetlookup.json).
-        
-        You can think of the different format presets on a content node as different "slots"
-        to be filled in by files, with certain slots being required while other optional.
-        For examples, for a VideoNode (kind=`video`) to be a valid content node, it must
-        have at least one video file associated with it filling either the `high_res_video`
-        slot or the `low_res_video` slot. Certain slots can have multiple files in them,
-        like the `video_subtitle` preset, since a VideoNode can have multiple subtitles
-        associated with it for different languages.
-        
-        
-        The figure below illustrates the structure between content nodes, files, and format presets.
-        
-        ![Illustration of the relationships between content kinds (nodes), files, and format presets.](docs/img/le-utils_constants_and_mapping.png)
-        
-        In the Sample shown, the Video Node is of content kind `video` and has three
-        files associated with it:
-          - The first file has file format `mp4` and format preset `high_res_video`
-          - The second file is also in `mp4` format but the relation to the content node
-            is that `low_res_video`
-          - A third file with format `vtt` is associated with the content node with a
-            format preset of `video_subtitle`.
-        
-        Format presets play a crucial role throughout the Kolibri content ecosystem and
-        govern such things as content validation rules applied by Ricecooker, Kolibri Studio
-        edit rules, and the rendering logic on Kolibri.
-        
-        
-        File types (ricecooker.files.File subclasses)
-        ---------------------------------------------
-        Used on Ricecooker as identifiers to represents what type of file when serializing
-        things to JSON as part of the content import process. Note that file types constants
-        are internal to ricecooker operations and are not used in Kolibri Studio or Kolibri.
-        
-        
-        
-        Exercises
-        ---------
-        The file [le_utils/constants/exercises.py](./le_utils/constants/exercises.py)
-        contains identifiers for different question types and mastery models.
-        
-        
-        
-        Proquint Channel Tokens
-        -----------------------
-        The file [le_utils/proquint.py](./le_utils/proquint.py) contains helper methods
-        for generating proquint identifiers for content channels. These are short strings
-        that are easy to enter on devices without a full keyboard, e.g. `sutul-hakuh`.
-        
-        
-        Roles
-        -----
-        The `role` constants are used for Role-based access control (RBAC) within the
-        Kolibri platform. Currently, only two levels of visibility are supported:
-          - `learner` (default): content nodes are visible to all Kolibri users
-          - `coach`: content nodes are only visible to Kolibri coaches and administrators
-        
-        
-        Metadata labels
-        ---------------
-        
-        These are encoded in spec/labels-v*.json. Once a spec has been finalized it will be
-        added to finalized_specs.yml to ensure that CI will fail any future modifications
-        to this specification. This ensures that the resulting built code has consistent
-        ordering so that generated bits for bitmasks are stable across releases.
-        We also require that all names in the specs be globally unique to minimize confusion
-        and reduce the chance of collisions in translations of these terms for users.
-        
 Keywords: le-utils le_utils LE utils kolibri studio ricecooker content curation
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Utilities
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*,  <3.12
 Description-Content-Type: text/markdown
 Provides-Extra: lang_utils
+License-File: LICENSE.txt
+
+LE Utils
+========
+The `le-utils` package contains shared constants used by Ricecooker, Kolibri, and
+Kolibri Studio. This package is not meant to be installed or used directly, but
+plays an important role in all Learning Equality products.
+
+
+Constants
+=========
+The Python files in the [le_utils/constants/](./le_utils/constants) are used to
+define constants (usually in `ALL_CAPS` form) to be used from Python code.
+The same constants and naming conventions are also provided in JSON format in the
+folder [le_utils/resources/](le_utils/resources) for use in frontend code.
+This means, adding a new constant may require editing multiple files: the Python
+constant-defining file, the JSON-file, and any associated tests.
+
+
+Languages
+---------
+The file [le_utils/constants/languages.py](./le_utils/constants/languages.py) and
+the lookup table in [le_utils/resources/languagelookup.json](./le_utils/resources/languagelookup.json)
+define the internal representation for languages codes used by Ricecooker, Kolibri,
+and Kolibri Studio to identify educational content in different languages.
+
+The internal representation uses a mixture of two-letter codes (e.g. `en`),
+two-letter-and-country code (e.g. `pt-BR` for Brazilian Portuguese),
+and three-letter codes (e.g., `zul` for Zulu).
+
+In order to make sure you have the correct language code when interfacing with
+the Kolibri ecosystem (e.g. when uploading new content to Kolibri Studio), you
+must lookup the language object using the helper method `getlang`:
+
+```
+>>> from le_utils.constants.languages import getlang
+>>> language_obj = getlang('en')       # lookup language using language code
+>>> language_obj
+Language(native_name='English', primary_code='en', subcode=None, name='English', ka_name=None)
+```
+The function `getlang` will return `None` if the lookup fails. In such cases, you
+can try lookup by name or lookup by alpha2 code (ISO_639-1) methods defined below.
+
+Once you've successfully looked up the language object, you can obtain the internal
+representation language code from the language object's `code` attribute:
+```
+>>> language_obj.code
+'en'
+```
+The Ricecooker API expects these internal representation language codes will be
+supplied for all `language` attributes (channel language, node language, and files language).
+
+
+
+### More lookup helper methods
+The helper method `getlang_by_name` allows you to lookup a language by name:
+```
+>>> from le_utils.constants.languages import getlang_by_name
+>>> language_obj = getlang_by_name('English')  # lookup language by name
+>>> language_obj
+Language(native_name='English', primary_code='en', subcode=None, name='English', ka_name=None)
+```
+
+The module `le_utils.constants.languages` defines two other language lookup methods:
+  - Use `getlang_by_native_name` for lookup up names by native language name,
+    e.g., you look for 'Français' to find French.
+ -  Use `getlang_by_alpha2` to perform lookups using the standard two-letter codes
+    defined in [ISO_639-1](https://en.wikipedia.org/wiki/ISO_639-1) that are
+    supported by the `pycountries` library.
+
+
+#### Useful links
+
+The following websites are useful for researching language codes:
+
+  - https://www.ethnologue.com/
+  - https://en.wikipedia.org/wiki/List_of_ISO_639-2_codes
+
+
+
+Licenses
+--------
+All content nodes within Kolibri and Kolibri Studio must have a license. The file
+[le_utils/constants/licenses.py](./le_utils/constants/licenses.py) contains the
+constants used to identify the license types. These constants are meant to be
+used in conjunction with the helper method `ricecooker.classes.licenses.get_license`
+to create `Licence` objects.
+
+To initialize a license object, you must specify the license type and the
+`copyright_holder` (str) which identifies a person or an organization. For example:
+```
+from ricecooker.classes.licenses import get_license
+from le_utils.constants import licenses
+license = get_license(licenses.CC_BY, copyright_holder="Khan Academy")
+```
+
+Note: The `copyright_holder` field is required for all License types except for
+the public domain license for which `copyright_holder` can be None.
+
+
+
+
+Content kinds (ContentNode subclasses)
+--------------------------------------
+Content items throughout the Kolibri ecosystem come in several kinds. The `kind`
+attribute of each object can be one of ("topic", "video", "audio", "exercise"
+"document", or "html5".
+See [constants/content_kinds.py](https://github.com/learningequality/le-utils/blob/master/le_utils/constants/content_kinds.py#L11-L17) for latest list.
+
+The currently supported content kinds are:
+  - Topic node (folder)
+  - Video content nodes backed by a video files and subtitles
+  - Audio content nodes backed by an audio files
+  - Document content nodes backed by a document files (PDF or ePub)
+  - HTML5 app content nodes backed by a HTML5 zip files
+  - Slideshow content nodes
+  - Exercise content nodes
+
+The `kind` attribute identifies a subclass of the base content node class within
+the data model, which differs on Ricecooker, Studio, and Kolibri:
+  - [ricecooker.classes.nodes.ContentNode](https://github.com/learningequality/ricecooker/blob/master/ricecooker/classes/nodes.py#L428-L506):
+    in-memory content node used to store metadata needed to upload new content to Kolibri  Studio
+  - [contentcuration.contentcuration.models.ContentNode](https://github.com/learningequality/studio/blob/develop/contentcuration/contentcuration/models.py#L775):
+    node within one of the trees associated with a Kolibri Studio channel.
+  - [kolibri.core.content.models.ContentNode](https://github.com/learningequality/kolibri/blob/develop/kolibri/core/content/models.py#L175):
+    node within tree for a particular version of a channel on Kolibri.
+
+For a detailed description of the common and different model attributes available
+on content nodes in each part of the platform see [this doc](https://docs.google.com/spreadsheets/d/181hSEwJ7yVmMh7LEwaHENqQetYSsbSDwybHTO_0zZM0/edit#gid=1640972430).
+
+
+
+File formats (extensions)
+-------------------------
+These are low-level constant that represents what type of file and are essentially
+synonymous with file extensions. The file format `MP4` is simply a convenient
+proxy for the file extension `mp4`.
+See [file_formats.py](https://github.com/learningequality/le-utils/blob/master/le_utils/constants/file_formats.py)
+and [resourcces/formatlookup.json](https://github.com/nucleogenesis/le-utils/blob/master/le_utils/resources/formatlookup.json).
+
+
+
+Format presets (ContentNode-File relation)
+------------------------------------------
+Every `ContentNode` is associated with one or more `File` objects and nature of
+this association is represented though the `format_preset` attribute of the file.
+The `format_preset` is the role the file is playing in the content node,
+e.g., thumbnail, high resolution video, or low resolution video.
+Note that format presets are represented redundantly as python string in
+[constants/format_presets.py](https://github.com/learningequality/le-utils/blob/master/le_utils/constants/format_presets.py)
+and as json [resources/presetlookup.json](https://github.com/learningequality/le-utils/blob/master/le_utils/resources/presetlookup.json).
+
+You can think of the different format presets on a content node as different "slots"
+to be filled in by files, with certain slots being required while other optional.
+For examples, for a VideoNode (kind=`video`) to be a valid content node, it must
+have at least one video file associated with it filling either the `high_res_video`
+slot or the `low_res_video` slot. Certain slots can have multiple files in them,
+like the `video_subtitle` preset, since a VideoNode can have multiple subtitles
+associated with it for different languages.
+
+
+The figure below illustrates the structure between content nodes, files, and format presets.
+
+![Illustration of the relationships between content kinds (nodes), files, and format presets.](docs/img/le-utils_constants_and_mapping.png)
+
+In the Sample shown, the Video Node is of content kind `video` and has three
+files associated with it:
+  - The first file has file format `mp4` and format preset `high_res_video`
+  - The second file is also in `mp4` format but the relation to the content node
+    is that `low_res_video`
+  - A third file with format `vtt` is associated with the content node with a
+    format preset of `video_subtitle`.
+
+Format presets play a crucial role throughout the Kolibri content ecosystem and
+govern such things as content validation rules applied by Ricecooker, Kolibri Studio
+edit rules, and the rendering logic on Kolibri.
+
+
+File types (ricecooker.files.File subclasses)
+---------------------------------------------
+Used on Ricecooker as identifiers to represents what type of file when serializing
+things to JSON as part of the content import process. Note that file types constants
+are internal to ricecooker operations and are not used in Kolibri Studio or Kolibri.
+
+
+
+Exercises
+---------
+The file [le_utils/constants/exercises.py](./le_utils/constants/exercises.py)
+contains identifiers for different question types and mastery models.
+
+
+
+Proquint Channel Tokens
+-----------------------
+The file [le_utils/proquint.py](./le_utils/proquint.py) contains helper methods
+for generating proquint identifiers for content channels. These are short strings
+that are easy to enter on devices without a full keyboard, e.g. `sutul-hakuh`.
+
+
+Roles
+-----
+The `role` constants are used for Role-based access control (RBAC) within the
+Kolibri platform. Currently, only two levels of visibility are supported:
+  - `learner` (default): content nodes are visible to all Kolibri users
+  - `coach`: content nodes are only visible to Kolibri coaches and administrators
+
+
+Metadata labels
+---------------
+
+These are encoded in spec/labels-v*.json. Once a spec has been finalized it will be
+added to finalized_specs.yml to ensure that CI will fail any future modifications
+to this specification. This ensures that the resulting built code has consistent
+ordering so that generated bits for bitmasks are stable across releases.
+We also require that all names in the specs be globally unique to minimize confusion
+and reduce the chance of collisions in translations of these terms for users.
+
+
```

### Comparing `le-utils-0.2.0/setup.py` & `le-utils-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 lang_utils_requirements = [
     "pycountry==17.5.14",
 ]
 
 setup(
     name="le-utils",
     packages=find_packages(),
-    version="0.2.0",
+    version="0.2.1",
     description="LE-Utils contains shared constants used in Kolibri, Ricecooker, and Kolibri Studio.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[],
     extras_require={"lang_utils": lang_utils_requirements},
     license="MIT",
     url="https://github.com/learningequality/le-utils",
```

### Comparing `le-utils-0.2.0/le_utils.egg-info/PKG-INFO` & `le-utils-0.2.1/le_utils.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,234 +1,237 @@
 Metadata-Version: 2.1
 Name: le-utils
-Version: 0.2.0
+Version: 0.2.1
 Summary: LE-Utils contains shared constants used in Kolibri, Ricecooker, and Kolibri Studio.
 Home-page: https://github.com/learningequality/le-utils
 Author: Learning Equality
 Author-email: info@learningequality.org
 License: MIT
 Download-URL: https://github.com/learningequality/le-utils/releases
-Description: LE Utils
-        ========
-        The `le-utils` package contains shared constants used by Ricecooker, Kolibri, and
-        Kolibri Studio. This package is not meant to be installed or used directly, but
-        plays an important role in all Learning Equality products.
-        
-        
-        Constants
-        =========
-        The Python files in the [le_utils/constants/](./le_utils/constants) are used to
-        define constants (usually in `ALL_CAPS` form) to be used from Python code.
-        The same constants and naming conventions are also provided in JSON format in the
-        folder [le_utils/resources/](le_utils/resources) for use in frontend code.
-        This means, adding a new constant may require editing multiple files: the Python
-        constant-defining file, the JSON-file, and any associated tests.
-        
-        
-        Languages
-        ---------
-        The file [le_utils/constants/languages.py](./le_utils/constants/languages.py) and
-        the lookup table in [le_utils/resources/languagelookup.json](./le_utils/resources/languagelookup.json)
-        define the internal representation for languages codes used by Ricecooker, Kolibri,
-        and Kolibri Studio to identify educational content in different languages.
-        
-        The internal representation uses a mixture of two-letter codes (e.g. `en`),
-        two-letter-and-country code (e.g. `pt-BR` for Brazilian Portuguese),
-        and three-letter codes (e.g., `zul` for Zulu).
-        
-        In order to make sure you have the correct language code when interfacing with
-        the Kolibri ecosystem (e.g. when uploading new content to Kolibri Studio), you
-        must lookup the language object using the helper method `getlang`:
-        
-        ```
-        >>> from le_utils.constants.languages import getlang
-        >>> language_obj = getlang('en')       # lookup language using language code
-        >>> language_obj
-        Language(native_name='English', primary_code='en', subcode=None, name='English', ka_name=None)
-        ```
-        The function `getlang` will return `None` if the lookup fails. In such cases, you
-        can try lookup by name or lookup by alpha2 code (ISO_639-1) methods defined below.
-        
-        Once you've successfully looked up the language object, you can obtain the internal
-        representation language code from the language object's `code` attribute:
-        ```
-        >>> language_obj.code
-        'en'
-        ```
-        The Ricecooker API expects these internal representation language codes will be
-        supplied for all `language` attributes (channel language, node language, and files language).
-        
-        
-        
-        ### More lookup helper methods
-        The helper method `getlang_by_name` allows you to lookup a language by name:
-        ```
-        >>> from le_utils.constants.languages import getlang_by_name
-        >>> language_obj = getlang_by_name('English')  # lookup language by name
-        >>> language_obj
-        Language(native_name='English', primary_code='en', subcode=None, name='English', ka_name=None)
-        ```
-        
-        The module `le_utils.constants.languages` defines two other language lookup methods:
-          - Use `getlang_by_native_name` for lookup up names by native language name,
-            e.g., you look for 'Français' to find French.
-         -  Use `getlang_by_alpha2` to perform lookups using the standard two-letter codes
-            defined in [ISO_639-1](https://en.wikipedia.org/wiki/ISO_639-1) that are
-            supported by the `pycountries` library.
-        
-        
-        #### Useful links
-        
-        The following websites are useful for researching language codes:
-        
-          - https://www.ethnologue.com/
-          - https://en.wikipedia.org/wiki/List_of_ISO_639-2_codes
-        
-        
-        
-        Licenses
-        --------
-        All content nodes within Kolibri and Kolibri Studio must have a license. The file
-        [le_utils/constants/licenses.py](./le_utils/constants/licenses.py) contains the
-        constants used to identify the license types. These constants are meant to be
-        used in conjunction with the helper method `ricecooker.classes.licenses.get_license`
-        to create `Licence` objects.
-        
-        To initialize a license object, you must specify the license type and the
-        `copyright_holder` (str) which identifies a person or an organization. For example:
-        ```
-        from ricecooker.classes.licenses import get_license
-        from le_utils.constants import licenses
-        license = get_license(licenses.CC_BY, copyright_holder="Khan Academy")
-        ```
-        
-        Note: The `copyright_holder` field is required for all License types except for
-        the public domain license for which `copyright_holder` can be None.
-        
-        
-        
-        
-        Content kinds (ContentNode subclasses)
-        --------------------------------------
-        Content items throughout the Kolibri ecosystem come in several kinds. The `kind`
-        attribute of each object can be one of ("topic", "video", "audio", "exercise"
-        "document", or "html5".
-        See [constants/content_kinds.py](https://github.com/learningequality/le-utils/blob/master/le_utils/constants/content_kinds.py#L11-L17) for latest list.
-        
-        The currently supported content kinds are:
-          - Topic node (folder)
-          - Video content nodes backed by a video files and subtitles
-          - Audio content nodes backed by an audio files
-          - Document content nodes backed by a document files (PDF or ePub)
-          - HTML5 app content nodes backed by a HTML5 zip files
-          - Slideshow content nodes
-          - Exercise content nodes
-        
-        The `kind` attribute identifies a subclass of the base content node class within
-        the data model, which differs on Ricecooker, Studio, and Kolibri:
-          - [ricecooker.classes.nodes.ContentNode](https://github.com/learningequality/ricecooker/blob/master/ricecooker/classes/nodes.py#L428-L506):
-            in-memory content node used to store metadata needed to upload new content to Kolibri  Studio
-          - [contentcuration.contentcuration.models.ContentNode](https://github.com/learningequality/studio/blob/develop/contentcuration/contentcuration/models.py#L775):
-            node within one of the trees associated with a Kolibri Studio channel.
-          - [kolibri.core.content.models.ContentNode](https://github.com/learningequality/kolibri/blob/develop/kolibri/core/content/models.py#L175):
-            node within tree for a particular version of a channel on Kolibri.
-        
-        For a detailed description of the common and different model attributes available
-        on content nodes in each part of the platform see [this doc](https://docs.google.com/spreadsheets/d/181hSEwJ7yVmMh7LEwaHENqQetYSsbSDwybHTO_0zZM0/edit#gid=1640972430).
-        
-        
-        
-        File formats (extensions)
-        -------------------------
-        These are low-level constant that represents what type of file and are essentially
-        synonymous with file extensions. The file format `MP4` is simply a convenient
-        proxy for the file extension `mp4`.
-        See [file_formats.py](https://github.com/learningequality/le-utils/blob/master/le_utils/constants/file_formats.py)
-        and [resourcces/formatlookup.json](https://github.com/nucleogenesis/le-utils/blob/master/le_utils/resources/formatlookup.json).
-        
-        
-        
-        Format presets (ContentNode-File relation)
-        ------------------------------------------
-        Every `ContentNode` is associated with one or more `File` objects and nature of
-        this association is represented though the `format_preset` attribute of the file.
-        The `format_preset` is the role the file is playing in the content node,
-        e.g., thumbnail, high resolution video, or low resolution video.
-        Note that format presets are represented redundantly as python string in
-        [constants/format_presets.py](https://github.com/learningequality/le-utils/blob/master/le_utils/constants/format_presets.py)
-        and as json [resources/presetlookup.json](https://github.com/learningequality/le-utils/blob/master/le_utils/resources/presetlookup.json).
-        
-        You can think of the different format presets on a content node as different "slots"
-        to be filled in by files, with certain slots being required while other optional.
-        For examples, for a VideoNode (kind=`video`) to be a valid content node, it must
-        have at least one video file associated with it filling either the `high_res_video`
-        slot or the `low_res_video` slot. Certain slots can have multiple files in them,
-        like the `video_subtitle` preset, since a VideoNode can have multiple subtitles
-        associated with it for different languages.
-        
-        
-        The figure below illustrates the structure between content nodes, files, and format presets.
-        
-        ![Illustration of the relationships between content kinds (nodes), files, and format presets.](docs/img/le-utils_constants_and_mapping.png)
-        
-        In the Sample shown, the Video Node is of content kind `video` and has three
-        files associated with it:
-          - The first file has file format `mp4` and format preset `high_res_video`
-          - The second file is also in `mp4` format but the relation to the content node
-            is that `low_res_video`
-          - A third file with format `vtt` is associated with the content node with a
-            format preset of `video_subtitle`.
-        
-        Format presets play a crucial role throughout the Kolibri content ecosystem and
-        govern such things as content validation rules applied by Ricecooker, Kolibri Studio
-        edit rules, and the rendering logic on Kolibri.
-        
-        
-        File types (ricecooker.files.File subclasses)
-        ---------------------------------------------
-        Used on Ricecooker as identifiers to represents what type of file when serializing
-        things to JSON as part of the content import process. Note that file types constants
-        are internal to ricecooker operations and are not used in Kolibri Studio or Kolibri.
-        
-        
-        
-        Exercises
-        ---------
-        The file [le_utils/constants/exercises.py](./le_utils/constants/exercises.py)
-        contains identifiers for different question types and mastery models.
-        
-        
-        
-        Proquint Channel Tokens
-        -----------------------
-        The file [le_utils/proquint.py](./le_utils/proquint.py) contains helper methods
-        for generating proquint identifiers for content channels. These are short strings
-        that are easy to enter on devices without a full keyboard, e.g. `sutul-hakuh`.
-        
-        
-        Roles
-        -----
-        The `role` constants are used for Role-based access control (RBAC) within the
-        Kolibri platform. Currently, only two levels of visibility are supported:
-          - `learner` (default): content nodes are visible to all Kolibri users
-          - `coach`: content nodes are only visible to Kolibri coaches and administrators
-        
-        
-        Metadata labels
-        ---------------
-        
-        These are encoded in spec/labels-v*.json. Once a spec has been finalized it will be
-        added to finalized_specs.yml to ensure that CI will fail any future modifications
-        to this specification. This ensures that the resulting built code has consistent
-        ordering so that generated bits for bitmasks are stable across releases.
-        We also require that all names in the specs be globally unique to minimize confusion
-        and reduce the chance of collisions in translations of these terms for users.
-        
 Keywords: le-utils le_utils LE utils kolibri studio ricecooker content curation
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Utilities
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*,  <3.12
 Description-Content-Type: text/markdown
 Provides-Extra: lang_utils
+License-File: LICENSE.txt
+
+LE Utils
+========
+The `le-utils` package contains shared constants used by Ricecooker, Kolibri, and
+Kolibri Studio. This package is not meant to be installed or used directly, but
+plays an important role in all Learning Equality products.
+
+
+Constants
+=========
+The Python files in the [le_utils/constants/](./le_utils/constants) are used to
+define constants (usually in `ALL_CAPS` form) to be used from Python code.
+The same constants and naming conventions are also provided in JSON format in the
+folder [le_utils/resources/](le_utils/resources) for use in frontend code.
+This means, adding a new constant may require editing multiple files: the Python
+constant-defining file, the JSON-file, and any associated tests.
+
+
+Languages
+---------
+The file [le_utils/constants/languages.py](./le_utils/constants/languages.py) and
+the lookup table in [le_utils/resources/languagelookup.json](./le_utils/resources/languagelookup.json)
+define the internal representation for languages codes used by Ricecooker, Kolibri,
+and Kolibri Studio to identify educational content in different languages.
+
+The internal representation uses a mixture of two-letter codes (e.g. `en`),
+two-letter-and-country code (e.g. `pt-BR` for Brazilian Portuguese),
+and three-letter codes (e.g., `zul` for Zulu).
+
+In order to make sure you have the correct language code when interfacing with
+the Kolibri ecosystem (e.g. when uploading new content to Kolibri Studio), you
+must lookup the language object using the helper method `getlang`:
+
+```
+>>> from le_utils.constants.languages import getlang
+>>> language_obj = getlang('en')       # lookup language using language code
+>>> language_obj
+Language(native_name='English', primary_code='en', subcode=None, name='English', ka_name=None)
+```
+The function `getlang` will return `None` if the lookup fails. In such cases, you
+can try lookup by name or lookup by alpha2 code (ISO_639-1) methods defined below.
+
+Once you've successfully looked up the language object, you can obtain the internal
+representation language code from the language object's `code` attribute:
+```
+>>> language_obj.code
+'en'
+```
+The Ricecooker API expects these internal representation language codes will be
+supplied for all `language` attributes (channel language, node language, and files language).
+
+
+
+### More lookup helper methods
+The helper method `getlang_by_name` allows you to lookup a language by name:
+```
+>>> from le_utils.constants.languages import getlang_by_name
+>>> language_obj = getlang_by_name('English')  # lookup language by name
+>>> language_obj
+Language(native_name='English', primary_code='en', subcode=None, name='English', ka_name=None)
+```
+
+The module `le_utils.constants.languages` defines two other language lookup methods:
+  - Use `getlang_by_native_name` for lookup up names by native language name,
+    e.g., you look for 'Français' to find French.
+ -  Use `getlang_by_alpha2` to perform lookups using the standard two-letter codes
+    defined in [ISO_639-1](https://en.wikipedia.org/wiki/ISO_639-1) that are
+    supported by the `pycountries` library.
+
+
+#### Useful links
+
+The following websites are useful for researching language codes:
+
+  - https://www.ethnologue.com/
+  - https://en.wikipedia.org/wiki/List_of_ISO_639-2_codes
+
+
+
+Licenses
+--------
+All content nodes within Kolibri and Kolibri Studio must have a license. The file
+[le_utils/constants/licenses.py](./le_utils/constants/licenses.py) contains the
+constants used to identify the license types. These constants are meant to be
+used in conjunction with the helper method `ricecooker.classes.licenses.get_license`
+to create `Licence` objects.
+
+To initialize a license object, you must specify the license type and the
+`copyright_holder` (str) which identifies a person or an organization. For example:
+```
+from ricecooker.classes.licenses import get_license
+from le_utils.constants import licenses
+license = get_license(licenses.CC_BY, copyright_holder="Khan Academy")
+```
+
+Note: The `copyright_holder` field is required for all License types except for
+the public domain license for which `copyright_holder` can be None.
+
+
+
+
+Content kinds (ContentNode subclasses)
+--------------------------------------
+Content items throughout the Kolibri ecosystem come in several kinds. The `kind`
+attribute of each object can be one of ("topic", "video", "audio", "exercise"
+"document", or "html5".
+See [constants/content_kinds.py](https://github.com/learningequality/le-utils/blob/master/le_utils/constants/content_kinds.py#L11-L17) for latest list.
+
+The currently supported content kinds are:
+  - Topic node (folder)
+  - Video content nodes backed by a video files and subtitles
+  - Audio content nodes backed by an audio files
+  - Document content nodes backed by a document files (PDF or ePub)
+  - HTML5 app content nodes backed by a HTML5 zip files
+  - Slideshow content nodes
+  - Exercise content nodes
+
+The `kind` attribute identifies a subclass of the base content node class within
+the data model, which differs on Ricecooker, Studio, and Kolibri:
+  - [ricecooker.classes.nodes.ContentNode](https://github.com/learningequality/ricecooker/blob/master/ricecooker/classes/nodes.py#L428-L506):
+    in-memory content node used to store metadata needed to upload new content to Kolibri  Studio
+  - [contentcuration.contentcuration.models.ContentNode](https://github.com/learningequality/studio/blob/develop/contentcuration/contentcuration/models.py#L775):
+    node within one of the trees associated with a Kolibri Studio channel.
+  - [kolibri.core.content.models.ContentNode](https://github.com/learningequality/kolibri/blob/develop/kolibri/core/content/models.py#L175):
+    node within tree for a particular version of a channel on Kolibri.
+
+For a detailed description of the common and different model attributes available
+on content nodes in each part of the platform see [this doc](https://docs.google.com/spreadsheets/d/181hSEwJ7yVmMh7LEwaHENqQetYSsbSDwybHTO_0zZM0/edit#gid=1640972430).
+
+
+
+File formats (extensions)
+-------------------------
+These are low-level constant that represents what type of file and are essentially
+synonymous with file extensions. The file format `MP4` is simply a convenient
+proxy for the file extension `mp4`.
+See [file_formats.py](https://github.com/learningequality/le-utils/blob/master/le_utils/constants/file_formats.py)
+and [resourcces/formatlookup.json](https://github.com/nucleogenesis/le-utils/blob/master/le_utils/resources/formatlookup.json).
+
+
+
+Format presets (ContentNode-File relation)
+------------------------------------------
+Every `ContentNode` is associated with one or more `File` objects and nature of
+this association is represented though the `format_preset` attribute of the file.
+The `format_preset` is the role the file is playing in the content node,
+e.g., thumbnail, high resolution video, or low resolution video.
+Note that format presets are represented redundantly as python string in
+[constants/format_presets.py](https://github.com/learningequality/le-utils/blob/master/le_utils/constants/format_presets.py)
+and as json [resources/presetlookup.json](https://github.com/learningequality/le-utils/blob/master/le_utils/resources/presetlookup.json).
+
+You can think of the different format presets on a content node as different "slots"
+to be filled in by files, with certain slots being required while other optional.
+For examples, for a VideoNode (kind=`video`) to be a valid content node, it must
+have at least one video file associated with it filling either the `high_res_video`
+slot or the `low_res_video` slot. Certain slots can have multiple files in them,
+like the `video_subtitle` preset, since a VideoNode can have multiple subtitles
+associated with it for different languages.
+
+
+The figure below illustrates the structure between content nodes, files, and format presets.
+
+![Illustration of the relationships between content kinds (nodes), files, and format presets.](docs/img/le-utils_constants_and_mapping.png)
+
+In the Sample shown, the Video Node is of content kind `video` and has three
+files associated with it:
+  - The first file has file format `mp4` and format preset `high_res_video`
+  - The second file is also in `mp4` format but the relation to the content node
+    is that `low_res_video`
+  - A third file with format `vtt` is associated with the content node with a
+    format preset of `video_subtitle`.
+
+Format presets play a crucial role throughout the Kolibri content ecosystem and
+govern such things as content validation rules applied by Ricecooker, Kolibri Studio
+edit rules, and the rendering logic on Kolibri.
+
+
+File types (ricecooker.files.File subclasses)
+---------------------------------------------
+Used on Ricecooker as identifiers to represents what type of file when serializing
+things to JSON as part of the content import process. Note that file types constants
+are internal to ricecooker operations and are not used in Kolibri Studio or Kolibri.
+
+
+
+Exercises
+---------
+The file [le_utils/constants/exercises.py](./le_utils/constants/exercises.py)
+contains identifiers for different question types and mastery models.
+
+
+
+Proquint Channel Tokens
+-----------------------
+The file [le_utils/proquint.py](./le_utils/proquint.py) contains helper methods
+for generating proquint identifiers for content channels. These are short strings
+that are easy to enter on devices without a full keyboard, e.g. `sutul-hakuh`.
+
+
+Roles
+-----
+The `role` constants are used for Role-based access control (RBAC) within the
+Kolibri platform. Currently, only two levels of visibility are supported:
+  - `learner` (default): content nodes are visible to all Kolibri users
+  - `coach`: content nodes are only visible to Kolibri coaches and administrators
+
+
+Metadata labels
+---------------
+
+These are encoded in spec/labels-v*.json. Once a spec has been finalized it will be
+added to finalized_specs.yml to ensure that CI will fail any future modifications
+to this specification. This ensures that the resulting built code has consistent
+ordering so that generated bits for bitmasks are stable across releases.
+We also require that all names in the specs be globally unique to minimize confusion
+and reduce the chance of collisions in translations of these terms for users.
+
+
```

### Comparing `le-utils-0.2.0/le_utils.egg-info/SOURCES.txt` & `le-utils-0.2.1/le_utils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 le_utils/__init__.py
 le_utils/humanhash.py
 le_utils/proquint.py
+le_utils/uuidv5.py
 le_utils.egg-info/PKG-INFO
 le_utils.egg-info/SOURCES.txt
 le_utils.egg-info/dependency_links.txt
 le_utils.egg-info/requires.txt
 le_utils.egg-info/top_level.txt
 le_utils/constants/__init__.py
 le_utils/constants/completion_criteria.py
@@ -19,14 +20,15 @@
 le_utils/constants/file_types.py
 le_utils/constants/format_presets.py
 le_utils/constants/languages.py
 le_utils/constants/licenses.py
 le_utils/constants/mastery_criteria.py
 le_utils/constants/modalities.py
 le_utils/constants/roles.py
+le_utils/constants/uuid.py
 le_utils/constants/labels/__init__.py
 le_utils/constants/labels/accessibility_categories.py
 le_utils/constants/labels/learning_activities.py
 le_utils/constants/labels/levels.py
 le_utils/constants/labels/needs.py
 le_utils/constants/labels/resource_type.py
 le_utils/constants/labels/subjects.py
```

### Comparing `le-utils-0.2.0/README.md` & `le-utils-0.2.1/README.md`

 * *Files identical despite different names*

