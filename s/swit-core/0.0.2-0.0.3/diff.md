# Comparing `tmp/swit_core-0.0.2.tar.gz` & `tmp/swit_core-0.0.3.tar.gz`

## Comparing `swit_core-0.0.2.tar` & `swit_core-0.0.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 swit_core-0.0.2/.DS_Store
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 swit_core-0.0.2/.flake8
--rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 swit_core-0.0.2/build.sh
--rwxr-xr-x   0        0        0       54 2020-02-02 00:00:00.000000 swit_core-0.0.2/run_tests.sh
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 swit_core-0.0.2/.idea/.gitignore
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 swit_core-0.0.2/.idea/core.iml
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 swit_core-0.0.2/.idea/misc.xml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 swit_core-0.0.2/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 swit_core-0.0.2/.idea/vcs.xml
--rw-r--r--   0        0        0    24979 2020-02-02 00:00:00.000000 swit_core-0.0.2/.idea/workspace.xml
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 swit_core-0.0.2/.idea/httpRequests/2023-08-08T143300.405.json
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 swit_core-0.0.2/.idea/httpRequests/2023-08-08T143308.500.json
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 swit_core-0.0.2/.idea/httpRequests/http-client.cookies
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 swit_core-0.0.2/.idea/httpRequests/http-requests-log.http
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 swit_core-0.0.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 swit_core-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/__init__.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/constants.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/logger.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/lokalise.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/type.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/action/__init__.py
--rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/action/activity_handler_abc.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/action/activity_router.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/action/dependencies.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/action/exceptions.py
--rw-r--r--   0        0        0     6309 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/action/schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/auth/__init__.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/auth/constants.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/auth/dependencies.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/auth/exception.py
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/auth/models.py
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/auth/oauth2.py
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/auth/repository.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/auth/router.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/auth/schemas.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/auth/signature_verification.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/auth/utils.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/Icon.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/__init__.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/button.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/collection_entry.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/container.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/divider.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/file.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/header.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/html_frame.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/image.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/input.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/select.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/select_item.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/signIn_page.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/static_action.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/tabs.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/text_paragraph.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/textarea.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 swit_core-0.0.2/tests/test_oauth2.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 swit_core-0.0.2/tests/test_path_resolver.py
--rw-r--r--   0        0        0     9030 2020-02-02 00:00:00.000000 swit_core-0.0.2/tests/test_router.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 swit_core-0.0.2/tests/test_signature_verification.py
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 swit_core-0.0.2/tests/utils.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 swit_core-0.0.2/.gitignore
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swit_core-0.0.2/README.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 swit_core-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 swit_core-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 swit_core-0.0.3/.DS_Store
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 swit_core-0.0.3/.flake8
+-rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 swit_core-0.0.3/build.sh
+-rwxr-xr-x   0        0        0       54 2020-02-02 00:00:00.000000 swit_core-0.0.3/run_tests.sh
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 swit_core-0.0.3/.idea/.gitignore
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 swit_core-0.0.3/.idea/core.iml
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 swit_core-0.0.3/.idea/misc.xml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 swit_core-0.0.3/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 swit_core-0.0.3/.idea/vcs.xml
+-rw-r--r--   0        0        0    26025 2020-02-02 00:00:00.000000 swit_core-0.0.3/.idea/workspace.xml
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 swit_core-0.0.3/.idea/httpRequests/2023-08-08T143300.405.json
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 swit_core-0.0.3/.idea/httpRequests/2023-08-08T143308.500.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 swit_core-0.0.3/.idea/httpRequests/http-client.cookies
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 swit_core-0.0.3/.idea/httpRequests/http-requests-log.http
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 swit_core-0.0.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 swit_core-0.0.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/__init__.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/constants.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/logger.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/lokalise.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/type.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/action/__init__.py
+-rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/action/activity_handler_abc.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/action/activity_router.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/action/dependencies.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/action/exceptions.py
+-rw-r--r--   0        0        0     6309 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/action/schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/auth/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/auth/constants.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/auth/dependencies.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/auth/exception.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/auth/models.py
+-rw-r--r--   0        0        0     4230 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/auth/oauth2.py
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/auth/repository.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/auth/router.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/auth/schemas.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/auth/signature_verification.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/auth/utils.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/ui/Icon.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/ui/__init__.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/ui/button.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/ui/collection_entry.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/ui/container.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/ui/divider.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/ui/file.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/ui/header.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/ui/html_frame.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/ui/image.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/ui/input.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/ui/select.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/ui/select_item.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/ui/signIn_page.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/ui/static_action.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/ui/tabs.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/ui/text_paragraph.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 swit_core-0.0.3/switcore/ui/textarea.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 swit_core-0.0.3/tests/test_oauth2.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 swit_core-0.0.3/tests/test_path_resolver.py
+-rw-r--r--   0        0        0     9030 2020-02-02 00:00:00.000000 swit_core-0.0.3/tests/test_router.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 swit_core-0.0.3/tests/test_signature_verification.py
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 swit_core-0.0.3/tests/utils.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 swit_core-0.0.3/.gitignore
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swit_core-0.0.3/README.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 swit_core-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 swit_core-0.0.3/PKG-INFO
```

### Comparing `swit_core-0.0.2/.DS_Store` & `swit_core-0.0.3/.DS_Store`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.2/.idea/workspace.xml` & `swit_core-0.0.3/.idea/workspace.xml`

 * *Files 2% similar despite different names*

#### Comparing `swit_core-0.0.2/.idea/workspace.xml` & `swit_core-0.0.3/.idea/workspace.xml`

```diff
@@ -3,16 +3,17 @@
   <component name="AnalysisUIOptions">
     <option name="SHOW_STRUCTURE" value="true"/>
   </component>
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="7747ff4f-b6a5-4206-b1a9-45990956cc9c" name="Changes" comment="add get_authorization_url">
+    <list default="true" id="7747ff4f-b6a5-4206-b1a9-45990956cc9c" name="Changes" comment="state default value None">
       <change beforePath="$PROJECT_DIR$/build.sh" beforeDir="false" afterPath="$PROJECT_DIR$/build.sh" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
@@ -42,15 +43,15 @@
   </component>
   <component name="PropertiesComponent"><![CDATA[{
   "keyToString": {
     "RunOnceActivity.OpenProjectViewOnStart": "true",
     "RunOnceActivity.ShowReadmeOnStart": "true",
     "TODO_SCOPE": "All Places",
     "WebServerToolWindowFactoryState": "false",
-    "com.google.cloudcode.ide_session_index": "20230808_0002",
+    "com.google.cloudcode.ide_session_index": "20230808_0008",
     "git-widget-placeholder": "main",
     "last_opened_file_path": "/Users/el/Library/Application Support/JetBrains/PyCharm2023.2/scratches",
     "node.js.detected.package.eslint": "true",
     "node.js.detected.package.tslint": "true",
     "node.js.selected.package.eslint": "(autodetect)",
     "node.js.selected.package.tslint": "(autodetect)",
     "nodejs_package_manager_path": "npm",
@@ -254,15 +255,17 @@
       <workItem from="1691019825770" duration="14837000"/>
       <workItem from="1691044078888" duration="5651000"/>
       <workItem from="1691125780639" duration="1692000"/>
       <workItem from="1691364671466" duration="7395000"/>
       <workItem from="1691382310184" duration="805000"/>
       <workItem from="1691383125458" duration="566000"/>
       <workItem from="1691384565572" duration="7184000"/>
-      <workItem from="1691476703720" duration="789000"/>
+      <workItem from="1691476703720" duration="2636000"/>
+      <workItem from="1691479933649" duration="1390000"/>
+      <workItem from="1691485960914" duration="92000"/>
     </task>
     <task id="LOCAL-00001" summary="first commit">
       <option name="closed" value="true"/>
       <created>1689566168015</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
@@ -440,15 +443,31 @@
       <option name="closed" value="true"/>
       <created>1691477176892</created>
       <option name="number" value="00023"/>
       <option name="presentableId" value="LOCAL-00023"/>
       <option name="project" value="LOCAL"/>
       <updated>1691477176892</updated>
     </task>
-    <option name="localTasksCounter" value="24"/>
+    <task id="LOCAL-00024" summary="extras_params 타입 변경">
+      <option name="closed" value="true"/>
+      <created>1691480197633</created>
+      <option name="number" value="00024"/>
+      <option name="presentableId" value="LOCAL-00024"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1691480197633</updated>
+    </task>
+    <task id="LOCAL-00025" summary="state default value None">
+      <option name="closed" value="true"/>
+      <created>1691486015746</created>
+      <option name="number" value="00025"/>
+      <option name="presentableId" value="LOCAL-00025"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1691486015746</updated>
+    </task>
+    <option name="localTasksCounter" value="26"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
@@ -466,15 +485,17 @@
     <MESSAGE value="escape 추가"/>
     <MESSAGE value="add signature_verification.py"/>
     <MESSAGE value="add args, kwargs"/>
     <MESSAGE value="add get_or_create"/>
     <MESSAGE value="add signature_verification"/>
     <MESSAGE value="프로젝트 정보 변경"/>
     <MESSAGE value="add get_authorization_url"/>
-    <option name="LAST_COMMIT_MESSAGE" value="add get_authorization_url"/>
+    <MESSAGE value="extras_params 타입 변경"/>
+    <MESSAGE value="state default value None"/>
+    <option name="LAST_COMMIT_MESSAGE" value="state default value None"/>
   </component>
   <component name="XDebuggerManager">
     <breakpoint-manager>
       <breakpoints>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/venv/lib/python3.10/site-packages/httpx_oauth/oauth2.py</url>
           <line>47</line>
```

### Comparing `swit_core-0.0.2/.idea/httpRequests/2023-08-08T143308.500.json` & `swit_core-0.0.3/.idea/httpRequests/2023-08-08T143308.500.json`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.2/.idea/httpRequests/http-requests-log.http` & `swit_core-0.0.3/.idea/httpRequests/http-requests-log.http`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.2/.idea/inspectionProfiles/Project_Default.xml` & `swit_core-0.0.3/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.2/switcore/logger.py` & `swit_core-0.0.3/switcore/logger.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.2/switcore/lokalise.py` & `swit_core-0.0.3/switcore/lokalise.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.2/switcore/action/activity_handler_abc.py` & `swit_core-0.0.3/switcore/action/activity_handler_abc.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.2/switcore/action/activity_router.py` & `swit_core-0.0.3/switcore/action/activity_router.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.2/switcore/action/dependencies.py` & `swit_core-0.0.3/switcore/action/dependencies.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.2/switcore/action/schemas.py` & `swit_core-0.0.3/switcore/action/schemas.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.2/switcore/auth/dependencies.py` & `swit_core-0.0.3/switcore/auth/dependencies.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.2/switcore/auth/exception.py` & `swit_core-0.0.3/switcore/auth/exception.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.2/switcore/auth/models.py` & `swit_core-0.0.3/switcore/auth/models.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.2/switcore/auth/oauth2.py` & `swit_core-0.0.3/switcore/auth/oauth2.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,17 +47,17 @@
             params["state"] = state
 
         return f"{self.authorize_endpoint}?{urlencode(params)}"
 
     async def get_authorization_url(
             self,
             redirect_uri: str,
-            state: str | None,
             scope: str,
-            **extras_params: dict[str, str],
+            state: str | None = None,
+            **extras_params,
     ) -> str:
         params = {
             "response_type": "code",
             "client_id": self.client_id,
             "redirect_uri": redirect_uri,
             "scope": scope,
         }
```

### Comparing `swit_core-0.0.2/switcore/auth/repository.py` & `swit_core-0.0.3/switcore/auth/repository.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.2/switcore/auth/router.py` & `swit_core-0.0.3/switcore/auth/router.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.2/switcore/auth/signature_verification.py` & `swit_core-0.0.3/switcore/auth/signature_verification.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.2/switcore/auth/utils.py` & `swit_core-0.0.3/switcore/auth/utils.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.2/switcore/ui/collection_entry.py` & `swit_core-0.0.3/switcore/ui/collection_entry.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.2/switcore/ui/file.py` & `swit_core-0.0.3/switcore/ui/file.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.2/tests/test_oauth2.py` & `swit_core-0.0.3/tests/test_oauth2.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.2/tests/test_path_resolver.py` & `swit_core-0.0.3/tests/test_path_resolver.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.2/tests/test_router.py` & `swit_core-0.0.3/tests/test_router.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.2/tests/test_signature_verification.py` & `swit_core-0.0.3/tests/test_signature_verification.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.2/tests/utils.py` & `swit_core-0.0.3/tests/utils.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.2/pyproject.toml` & `swit_core-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "swit-core"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name = "ur-team", email = "developers@swit.io" },
 ]
 description = "this is a switbuilder core package"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `swit_core-0.0.2/PKG-INFO` & `swit_core-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swit-core
-Version: 0.0.2
+Version: 0.0.3
 Summary: this is a switbuilder core package
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: ur-team <developers@swit.io>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

