# Comparing `tmp/swit_core-0.0.1.tar.gz` & `tmp/swit_core-0.0.2.tar.gz`

## Comparing `swit_core-0.0.1.tar` & `swit_core-0.0.2.tar`

### file list

```diff
@@ -1,62 +1,66 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 swit_core-0.0.1/.DS_Store
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 swit_core-0.0.1/.flake8
--rwxr-xr-x   0        0        0       85 2020-02-02 00:00:00.000000 swit_core-0.0.1/build.sh
--rwxr-xr-x   0        0        0       54 2020-02-02 00:00:00.000000 swit_core-0.0.1/run_tests.sh
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 swit_core-0.0.1/.idea/.gitignore
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 swit_core-0.0.1/.idea/core.iml
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 swit_core-0.0.1/.idea/misc.xml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 swit_core-0.0.1/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 swit_core-0.0.1/.idea/vcs.xml
--rw-r--r--   0        0        0    25899 2020-02-02 00:00:00.000000 swit_core-0.0.1/.idea/workspace.xml
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 swit_core-0.0.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 swit_core-0.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/__init__.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/constants.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/logger.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/lokalise.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/type.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/action/__init__.py
--rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/action/activity_handler_abc.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/action/activity_router.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/action/dependencies.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/action/exceptions.py
--rw-r--r--   0        0        0     6309 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/action/schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/auth/__init__.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/auth/constants.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/auth/dependencies.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/auth/exception.py
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/auth/models.py
--rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/auth/oauth2.py
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/auth/repository.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/auth/router.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/auth/schemas.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/auth/signature_verification.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/auth/utils.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/ui/Icon.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/ui/__init__.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/ui/button.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/ui/collection_entry.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/ui/container.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/ui/divider.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/ui/file.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/ui/header.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/ui/html_frame.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/ui/image.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/ui/input.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/ui/select.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/ui/select_item.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/ui/signIn_page.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/ui/static_action.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/ui/tabs.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/ui/text_paragraph.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 swit_core-0.0.1/switcore/ui/textarea.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 swit_core-0.0.1/tests/test_oauth2.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 swit_core-0.0.1/tests/test_path_resolver.py
--rw-r--r--   0        0        0     9030 2020-02-02 00:00:00.000000 swit_core-0.0.1/tests/test_router.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 swit_core-0.0.1/tests/test_signature_verification.py
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 swit_core-0.0.1/tests/utils.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 swit_core-0.0.1/.gitignore
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swit_core-0.0.1/README.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 swit_core-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 swit_core-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 swit_core-0.0.2/.DS_Store
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 swit_core-0.0.2/.flake8
+-rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 swit_core-0.0.2/build.sh
+-rwxr-xr-x   0        0        0       54 2020-02-02 00:00:00.000000 swit_core-0.0.2/run_tests.sh
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 swit_core-0.0.2/.idea/.gitignore
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 swit_core-0.0.2/.idea/core.iml
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 swit_core-0.0.2/.idea/misc.xml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 swit_core-0.0.2/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 swit_core-0.0.2/.idea/vcs.xml
+-rw-r--r--   0        0        0    24979 2020-02-02 00:00:00.000000 swit_core-0.0.2/.idea/workspace.xml
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 swit_core-0.0.2/.idea/httpRequests/2023-08-08T143300.405.json
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 swit_core-0.0.2/.idea/httpRequests/2023-08-08T143308.500.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 swit_core-0.0.2/.idea/httpRequests/http-client.cookies
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 swit_core-0.0.2/.idea/httpRequests/http-requests-log.http
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 swit_core-0.0.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 swit_core-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/__init__.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/constants.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/logger.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/lokalise.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/type.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/action/__init__.py
+-rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/action/activity_handler_abc.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/action/activity_router.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/action/dependencies.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/action/exceptions.py
+-rw-r--r--   0        0        0     6309 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/action/schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/auth/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/auth/constants.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/auth/dependencies.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/auth/exception.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/auth/models.py
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/auth/oauth2.py
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/auth/repository.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/auth/router.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/auth/schemas.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/auth/signature_verification.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/auth/utils.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/Icon.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/__init__.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/button.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/collection_entry.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/container.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/divider.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/file.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/header.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/html_frame.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/image.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/input.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/select.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/select_item.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/signIn_page.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/static_action.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/tabs.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/text_paragraph.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 swit_core-0.0.2/switcore/ui/textarea.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swit_core-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 swit_core-0.0.2/tests/test_oauth2.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 swit_core-0.0.2/tests/test_path_resolver.py
+-rw-r--r--   0        0        0     9030 2020-02-02 00:00:00.000000 swit_core-0.0.2/tests/test_router.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 swit_core-0.0.2/tests/test_signature_verification.py
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 swit_core-0.0.2/tests/utils.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 swit_core-0.0.2/.gitignore
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swit_core-0.0.2/README.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 swit_core-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 swit_core-0.0.2/PKG-INFO
```

### Comparing `swit_core-0.0.1/.DS_Store` & `swit_core-0.0.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.1/.idea/workspace.xml` & `swit_core-0.0.2/.idea/workspace.xml`

 * *Files 6% similar despite different names*

#### Comparing `swit_core-0.0.1/.idea/workspace.xml` & `swit_core-0.0.2/.idea/workspace.xml`

```diff
@@ -3,16 +3,16 @@
   <component name="AnalysisUIOptions">
     <option name="SHOW_STRUCTURE" value="true"/>
   </component>
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="7747ff4f-b6a5-4206-b1a9-45990956cc9c" name="Changes" comment="add signature_verification">
-      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
+    <list default="true" id="7747ff4f-b6a5-4206-b1a9-45990956cc9c" name="Changes" comment="add get_authorization_url">
+      <change beforePath="$PROJECT_DIR$/build.sh" beforeDir="false" afterPath="$PROJECT_DIR$/build.sh" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
@@ -42,15 +42,15 @@
   </component>
   <component name="PropertiesComponent"><![CDATA[{
   "keyToString": {
     "RunOnceActivity.OpenProjectViewOnStart": "true",
     "RunOnceActivity.ShowReadmeOnStart": "true",
     "TODO_SCOPE": "All Places",
     "WebServerToolWindowFactoryState": "false",
-    "com.google.cloudcode.ide_session_index": "20230807_0005",
+    "com.google.cloudcode.ide_session_index": "20230808_0002",
     "git-widget-placeholder": "main",
     "last_opened_file_path": "/Users/el/Library/Application Support/JetBrains/PyCharm2023.2/scratches",
     "node.js.detected.package.eslint": "true",
     "node.js.detected.package.tslint": "true",
     "node.js.selected.package.eslint": "(autodetect)",
     "node.js.selected.package.tslint": "(autodetect)",
     "nodejs_package_manager_path": "npm",
@@ -70,35 +70,16 @@
     <key name="MoveFile.RECENT_KEYS">
       <recent name="$PROJECT_DIR$/switcore"/>
       <recent name="$PROJECT_DIR$/apis/v1"/>
       <recent name="$PROJECT_DIR$"/>
       <recent name="$PROJECT_DIR$/switbuilder-core"/>
     </key>
   </component>
-  <component name="RunManager" selected="Python tests.Python tests for test_signature_verification.SignatureVerifierTest">
-    <configuration name="aa" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
-      <module name="core"/>
-      <option name="INTERPRETER_OPTIONS" value=""/>
-      <option name="PARENT_ENVS" value="true"/>
-      <envs>
-        <env name="PYTHONUNBUFFERED" value="1"/>
-      </envs>
-      <option name="SDK_HOME" value=""/>
-      <option name="WORKING_DIRECTORY" value="$APPLICATION_CONFIG_DIR$/scratches"/>
-      <option name="IS_MODULE_SDK" value="false"/>
-      <option name="ADD_CONTENT_ROOTS" value="true"/>
-      <option name="ADD_SOURCE_ROOTS" value="true"/>
-      <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
-      <option name="SCRIPT_NAME" value="$APPLICATION_CONFIG_DIR$/scratches/aa.py"/>
-      <option name="PARAMETERS" value=""/>
-      <option name="SHOW_COMMAND_LINE" value="false"/>
-      <option name="EMULATE_TERMINAL" value="false"/>
-      <option name="MODULE_MODE" value="false"/>
-      <option name="REDIRECT_INPUT" value="false"/>
-      <option name="INPUT_FILE" value=""/>
+  <component name="RunManager" selected="HTTP Request.test | #1">
+    <configuration name="test | #1" type="HttpClient.HttpRequestRunConfigurationType" factoryName="HTTP Request" temporary="true" nameIsGenerated="true" path="$APPLICATION_CONFIG_DIR$/scratches/test.http" requestIdentifier="#1" runType="Run single request">
       <method v="2"/>
     </configuration>
     <configuration name="main" type="PythonConfigurationType" factoryName="Python" nameIsGenerated="true">
       <module name="core"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs>
@@ -115,86 +96,71 @@
       <option name="SHOW_COMMAND_LINE" value="false"/>
       <option name="EMULATE_TERMINAL" value="false"/>
       <option name="MODULE_MODE" value="false"/>
       <option name="REDIRECT_INPUT" value="false"/>
       <option name="INPUT_FILE" value=""/>
       <method v="2"/>
     </configuration>
-    <configuration name="Python tests for test_signature_verification.SignatureVerifierTest" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+    <configuration name="Python tests for test_oauth2.OAuth2Test" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="core"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;test_signature_verification.SignatureVerifierTest&quot;"/>
+      <option name="_new_target" value="&quot;test_oauth2.OAuth2Test&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="Python tests for test_signature_verification.SignatureVerifierTest.test_verification_failure_due_to_invalid_signing_secret" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+    <configuration name="Python tests for test_router.RouterTest" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="core"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;test_signature_verification.SignatureVerifierTest.test_verification_failure_due_to_invalid_signing_secret&quot;"/>
+      <option name="_new_target" value="&quot;test_router.RouterTest&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="Python tests for test_signature_verification.SignatureVerifierTest.test_verification_failure_due_to_time" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+    <configuration name="Python tests for test_signature_verification.SignatureVerifierTest" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="core"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;test_signature_verification.SignatureVerifierTest.test_verification_failure_due_to_time&quot;"/>
+      <option name="_new_target" value="&quot;test_signature_verification.SignatureVerifierTest&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="Python tests for test_signature_verification.SignatureVerifierTest.test_verification_success" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+    <configuration name="Python tests for test_signature_verification.SignatureVerifierTest.test_verification_failure_due_to_invalid_signing_secret" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="core"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;test_signature_verification.SignatureVerifierTest.test_verification_success&quot;"/>
-      <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
-      <method v="2"/>
-    </configuration>
-    <configuration name="Python tests for tests.Test" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
-      <module name="core"/>
-      <option name="INTERPRETER_OPTIONS" value=""/>
-      <option name="PARENT_ENVS" value="true"/>
-      <option name="SDK_HOME" value=""/>
-      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/switbuilder-core/ui/header"/>
-      <option name="IS_MODULE_SDK" value="true"/>
-      <option name="ADD_CONTENT_ROOTS" value="true"/>
-      <option name="ADD_SOURCE_ROOTS" value="true"/>
-      <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
-      <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;tests.Test&quot;"/>
+      <option name="_new_target" value="&quot;test_signature_verification.SignatureVerifierTest.test_verification_failure_due_to_invalid_signing_secret&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
     <configuration name="Python tests for tests.Test" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="core"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
@@ -222,19 +188,19 @@
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
       <option name="_new_target" value="&quot;tests.Test&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
     <recent_temporary>
       <list>
+        <item itemvalue="HTTP Request.test | #1"/>
+        <item itemvalue="Python tests.Python tests for test_oauth2.OAuth2Test"/>
+        <item itemvalue="Python tests.Python tests for test_router.RouterTest"/>
         <item itemvalue="Python tests.Python tests for test_signature_verification.SignatureVerifierTest"/>
         <item itemvalue="Python tests.Python tests for test_signature_verification.SignatureVerifierTest.test_verification_failure_due_to_invalid_signing_secret"/>
-        <item itemvalue="Python tests.Python tests for test_signature_verification.SignatureVerifierTest.test_verification_failure_due_to_time"/>
-        <item itemvalue="Python tests.Python tests for test_signature_verification.SignatureVerifierTest.test_verification_success"/>
-        <item itemvalue="Python.aa"/>
       </list>
     </recent_temporary>
   </component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="7747ff4f-b6a5-4206-b1a9-45990956cc9c" name="Changes" comment=""/>
@@ -285,15 +251,18 @@
       <workItem from="1690768201250" duration="10490000"/>
       <workItem from="1690785105649" duration="1898000"/>
       <workItem from="1690846288216" duration="8036000"/>
       <workItem from="1691019825770" duration="14837000"/>
       <workItem from="1691044078888" duration="5651000"/>
       <workItem from="1691125780639" duration="1692000"/>
       <workItem from="1691364671466" duration="7395000"/>
-      <workItem from="1691382310184" duration="295000"/>
+      <workItem from="1691382310184" duration="805000"/>
+      <workItem from="1691383125458" duration="566000"/>
+      <workItem from="1691384565572" duration="7184000"/>
+      <workItem from="1691476703720" duration="789000"/>
     </task>
     <task id="LOCAL-00001" summary="first commit">
       <option name="closed" value="true"/>
       <created>1689566168015</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
@@ -455,15 +424,31 @@
       <option name="closed" value="true"/>
       <created>1691042699521</created>
       <option name="number" value="00021"/>
       <option name="presentableId" value="LOCAL-00021"/>
       <option name="project" value="LOCAL"/>
       <updated>1691042699521</updated>
     </task>
-    <option name="localTasksCounter" value="22"/>
+    <task id="LOCAL-00022" summary="프로젝트 정보 변경">
+      <option name="closed" value="true"/>
+      <created>1691477099421</created>
+      <option name="number" value="00022"/>
+      <option name="presentableId" value="LOCAL-00022"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1691477099421</updated>
+    </task>
+    <task id="LOCAL-00023" summary="add get_authorization_url">
+      <option name="closed" value="true"/>
+      <created>1691477176892</created>
+      <option name="number" value="00023"/>
+      <option name="presentableId" value="LOCAL-00023"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1691477176892</updated>
+    </task>
+    <option name="localTasksCounter" value="24"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
@@ -479,31 +464,38 @@
   <component name="VcsManagerConfiguration">
     <MESSAGE value="first commit"/>
     <MESSAGE value="escape 추가"/>
     <MESSAGE value="add signature_verification.py"/>
     <MESSAGE value="add args, kwargs"/>
     <MESSAGE value="add get_or_create"/>
     <MESSAGE value="add signature_verification"/>
-    <option name="LAST_COMMIT_MESSAGE" value="add signature_verification"/>
+    <MESSAGE value="프로젝트 정보 변경"/>
+    <MESSAGE value="add get_authorization_url"/>
+    <option name="LAST_COMMIT_MESSAGE" value="add get_authorization_url"/>
   </component>
   <component name="XDebuggerManager">
     <breakpoint-manager>
       <breakpoints>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/venv/lib/python3.10/site-packages/httpx_oauth/oauth2.py</url>
           <line>47</line>
           <option name="timeStamp" value="28"/>
         </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/switcore/auth/router.py</url>
+          <line>27</line>
+          <option name="timeStamp" value="29"/>
+        </line-breakpoint>
       </breakpoints>
     </breakpoint-manager>
     <watches-manager>
       <configuration name="tests">
         <watch expression="unquote(response.headers[&quot;location&quot;])" language="Python"/>
       </configuration>
     </watches-manager>
   </component>
   <component name="com.intellij.coverage.CoverageDataManagerImpl">
     <SUITE FILE_PATH="coverage/core$aa.coverage" NAME="aa Coverage Results" MODIFIED="1690410103760" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$APPLICATION_CONFIG_DIR$/scratches"/>
-    <SUITE FILE_PATH="coverage/core$.coverage" NAME=" Coverage Results" MODIFIED="1691027116387" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tests"/>
+    <SUITE FILE_PATH="coverage/core$.coverage" NAME=" Coverage Results" MODIFIED="1691388445257" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tests"/>
     <SUITE FILE_PATH="coverage/core$main.coverage" NAME="main Coverage Results" MODIFIED="1690246417369" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
   </component>
 </project>
```

### Comparing `swit_core-0.0.1/.idea/inspectionProfiles/Project_Default.xml` & `swit_core-0.0.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.1/switcore/logger.py` & `swit_core-0.0.2/switcore/logger.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.1/switcore/lokalise.py` & `swit_core-0.0.2/switcore/lokalise.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.1/switcore/action/activity_handler_abc.py` & `swit_core-0.0.2/switcore/action/activity_handler_abc.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.1/switcore/action/activity_router.py` & `swit_core-0.0.2/switcore/action/activity_router.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.1/switcore/action/dependencies.py` & `swit_core-0.0.2/switcore/action/dependencies.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.1/switcore/action/schemas.py` & `swit_core-0.0.2/switcore/action/schemas.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.1/switcore/auth/dependencies.py` & `swit_core-0.0.2/switcore/auth/dependencies.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.1/switcore/auth/exception.py` & `swit_core-0.0.2/switcore/auth/exception.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.1/switcore/auth/models.py` & `swit_core-0.0.2/switcore/auth/models.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.1/switcore/auth/oauth2.py` & `swit_core-0.0.2/switcore/auth/oauth2.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,14 +44,36 @@
         }
 
         if state is not None:
             params["state"] = state
 
         return f"{self.authorize_endpoint}?{urlencode(params)}"
 
+    async def get_authorization_url(
+            self,
+            redirect_uri: str,
+            state: str | None,
+            scope: str,
+            **extras_params: dict[str, str],
+    ) -> str:
+        params = {
+            "response_type": "code",
+            "client_id": self.client_id,
+            "redirect_uri": redirect_uri,
+            "scope": scope,
+        }
+
+        if state is not None:
+            params["state"] = state
+
+        if extras_params is not None:
+            params = {**params, **extras_params}
+
+        return f"{self.authorize_endpoint}?{urlencode(params)}"
+
     async def get_access_token(self, code: str, redirect_uri: str) -> SwitToken:
         async with httpx.AsyncClient() as client:
             data = {
                 "grant_type": "authorization_code",
                 "code": code,
                 "redirect_uri": redirect_uri,
                 "client_id": self.client_id,
```

### Comparing `swit_core-0.0.1/switcore/auth/repository.py` & `swit_core-0.0.2/switcore/auth/repository.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.1/switcore/auth/router.py` & `swit_core-0.0.2/switcore/auth/router.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.1/switcore/auth/signature_verification.py` & `swit_core-0.0.2/switcore/auth/signature_verification.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.1/switcore/auth/utils.py` & `swit_core-0.0.2/switcore/auth/utils.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.1/switcore/ui/collection_entry.py` & `swit_core-0.0.2/switcore/ui/collection_entry.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.1/switcore/ui/file.py` & `swit_core-0.0.2/switcore/ui/file.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.1/tests/test_oauth2.py` & `swit_core-0.0.2/tests/test_oauth2.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.1/tests/test_path_resolver.py` & `swit_core-0.0.2/tests/test_path_resolver.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.1/tests/test_router.py` & `swit_core-0.0.2/tests/test_router.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.1/tests/test_signature_verification.py` & `swit_core-0.0.2/tests/test_signature_verification.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.1/tests/utils.py` & `swit_core-0.0.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `swit_core-0.0.1/pyproject.toml` & `swit_core-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "swit-core"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name = "ur-team", email = "developers@swit.io" },
 ]
 description = "this is a switbuilder core package"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `swit_core-0.0.1/PKG-INFO` & `swit_core-0.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swit-core
-Version: 0.0.1
+Version: 0.0.2
 Summary: this is a switbuilder core package
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: ur-team <developers@swit.io>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

