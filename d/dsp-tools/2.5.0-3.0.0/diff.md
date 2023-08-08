# Comparing `tmp/dsp_tools-2.5.0.tar.gz` & `tmp/dsp_tools-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsp_tools-2.5.0.tar", max compression
+gzip compressed data, was "dsp_tools-3.0.0.tar", max compression
```

## Comparing `dsp_tools-2.5.0.tar` & `dsp_tools-3.0.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0    35149 2023-07-28 08:19:29.730879 dsp_tools-2.5.0/LICENSE
--rw-r--r--   0        0        0     4602 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/docs/index.md
--rw-r--r--   0        0        0     5007 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/__init__.py
--rw-r--r--   0        0        0    24318 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/dsp_tools.py
--rw-r--r--   0        0        0    89253 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/excel2xml.py
--rw-r--r--   0        0        0        0 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/fast_xmlupload/__init__.py
--rw-r--r--   0        0        0    38361 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/fast_xmlupload/process_files.py
--rw-r--r--   0        0        0    14344 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/fast_xmlupload/upload_files.py
--rw-r--r--   0        0        0     4185 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/fast_xmlupload/upload_xml.py
--rw-r--r--   0        0        0        0 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/models/__init__.py
--rw-r--r--   0        0        0     1059 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/models/bitstream.py
--rw-r--r--   0        0        0     8718 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/models/connection.py
--rw-r--r--   0        0        0     3325 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/models/exceptions.py
--rw-r--r--   0        0        0     8851 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/models/group.py
--rw-r--r--   0        0        0    16528 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/models/helpers.py
--rw-r--r--   0        0        0     8979 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/models/langstring.py
--rw-r--r--   0        0        0    20524 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/models/listnode.py
--rw-r--r--   0        0        0      463 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/models/model.py
--rw-r--r--   0        0        0    14896 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/models/ontology.py
--rw-r--r--   0        0        0     2350 2023-07-28 08:19:29.750879 dsp_tools-2.5.0/src/dsp_tools/models/permission.py
--rw-r--r--   0        0        0    16761 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/models/project.py
--rw-r--r--   0        0        0     1744 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/models/projectContext.py
--rw-r--r--   0        0        0    18840 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/models/propertyclass.py
--rw-r--r--   0        0        0     1930 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/models/propertyelement.py
--rw-r--r--   0        0        0    20694 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/models/resource.py
--rw-r--r--   0        0        0    29833 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/models/resourceclass.py
--rw-r--r--   0        0        0      496 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/models/set_encoder.py
--rw-r--r--   0        0        0     1087 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/models/sipi.py
--rw-r--r--   0        0        0    25439 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/models/user.py
--rw-r--r--   0        0        0    33397 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/models/value.py
--rw-r--r--   0        0        0     1971 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/models/xmlallow.py
--rw-r--r--   0        0        0      594 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/models/xmlbitstream.py
--rw-r--r--   0        0        0     1504 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/models/xmlpermission.py
--rw-r--r--   0        0        0     2172 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/models/xmlproperty.py
--rw-r--r--   0        0        0     8720 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/models/xmlresource.py
--rw-r--r--   0        0        0     2141 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/models/xmlvalue.py
--rw-r--r--   0        0        0        0 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/py.typed
--rw-r--r--   0        0        0     1488 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/resources/0100-template-repo/template.json
--rw-r--r--   0        0        0     1036 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/resources/0100-template-repo/template.xml
--rw-r--r--   0        0        0    23808 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/resources/schema/data.xsd
--rw-r--r--   0        0        0     2770 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/resources/schema/lists-only.json
--rw-r--r--   0        0        0    42584 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/resources/schema/project.json
--rw-r--r--   0        0        0    32171 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/resources/schema/properties-only.json
--rw-r--r--   0        0        0     4341 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/resources/schema/resources-only.json
--rw-r--r--   0        0        0       61 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/resources/start-stack/docker-compose.override.yml
--rw-r--r--   0        0        0     2460 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/resources/start-stack/docker-compose.yml
--rw-r--r--   0        0        0      164 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/resources/start-stack/start-stack-config.yml
--rw-r--r--   0        0        0        0 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/utils/__init__.py
--rw-r--r--   0        0        0    15142 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/utils/excel_to_json_lists.py
--rw-r--r--   0        0        0     4912 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/utils/excel_to_json_project.py
--rw-r--r--   0        0        0     8237 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/utils/excel_to_json_properties.py
--rw-r--r--   0        0        0    10530 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/utils/excel_to_json_resources.py
--rw-r--r--   0        0        0     1170 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/utils/generate_templates.py
--rw-r--r--   0        0        0     3189 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/utils/id_to_iri.py
--rw-r--r--   0        0        0     1424 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/utils/logging.py
--rw-r--r--   0        0        0    42361 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/utils/project_create.py
--rw-r--r--   0        0        0     8373 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/utils/project_create_lists.py
--rw-r--r--   0        0        0     4694 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/utils/project_get.py
--rw-r--r--   0        0        0    18815 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/utils/project_validate.py
--rw-r--r--   0        0        0     4259 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/utils/rosetta.py
--rw-r--r--   0        0        0    13326 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/utils/shared.py
--rw-r--r--   0        0        0    13872 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/utils/stack_handling.py
--rw-r--r--   0        0        0    52419 2023-07-28 08:19:29.754879 dsp_tools-2.5.0/src/dsp_tools/utils/xml_upload.py
--rw-r--r--   0        0        0     5940 1970-01-01 00:00:00.000000 dsp_tools-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-08 15:17:48.912974 dsp_tools-3.0.0/LICENSE
+-rw-r--r--   0        0        0     5058 2023-08-08 15:17:48.932975 dsp_tools-3.0.0/docs/index.md
+-rw-r--r--   0        0        0     5007 2023-08-08 15:17:48.932975 dsp_tools-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-08 15:17:48.932975 dsp_tools-3.0.0/src/dsp_tools/__init__.py
+-rw-r--r--   0        0        0    24014 2023-08-08 15:17:48.932975 dsp_tools-3.0.0/src/dsp_tools/dsp_tools.py
+-rw-r--r--   0        0        0    89253 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/excel2xml.py
+-rw-r--r--   0        0        0        0 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/fast_xmlupload/__init__.py
+-rw-r--r--   0        0        0    38501 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/fast_xmlupload/process_files.py
+-rw-r--r--   0        0        0    14418 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/fast_xmlupload/upload_files.py
+-rw-r--r--   0        0        0     4230 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/fast_xmlupload/upload_xml.py
+-rw-r--r--   0        0        0        0 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/models/__init__.py
+-rw-r--r--   0        0        0     1059 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/models/bitstream.py
+-rw-r--r--   0        0        0     8718 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/models/connection.py
+-rw-r--r--   0        0        0     3325 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/models/exceptions.py
+-rw-r--r--   0        0        0     8851 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/models/group.py
+-rw-r--r--   0        0        0    16528 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/models/helpers.py
+-rw-r--r--   0        0        0     8979 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/models/langstring.py
+-rw-r--r--   0        0        0    20524 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/models/listnode.py
+-rw-r--r--   0        0        0      463 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/models/model.py
+-rw-r--r--   0        0        0    14896 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/models/ontology.py
+-rw-r--r--   0        0        0     2350 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/models/permission.py
+-rw-r--r--   0        0        0    16761 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/models/project.py
+-rw-r--r--   0        0        0     1744 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/models/projectContext.py
+-rw-r--r--   0        0        0    18840 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/models/propertyclass.py
+-rw-r--r--   0        0        0     1930 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/models/propertyelement.py
+-rw-r--r--   0        0        0    20694 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/models/resource.py
+-rw-r--r--   0        0        0    29833 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/models/resourceclass.py
+-rw-r--r--   0        0        0      496 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/models/set_encoder.py
+-rw-r--r--   0        0        0     1201 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/models/sipi.py
+-rw-r--r--   0        0        0    25439 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/models/user.py
+-rw-r--r--   0        0        0    33397 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/models/value.py
+-rw-r--r--   0        0        0     1971 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/models/xmlallow.py
+-rw-r--r--   0        0        0      594 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/models/xmlbitstream.py
+-rw-r--r--   0        0        0     1504 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/models/xmlpermission.py
+-rw-r--r--   0        0        0     2172 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/models/xmlproperty.py
+-rw-r--r--   0        0        0     8720 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/models/xmlresource.py
+-rw-r--r--   0        0        0     2141 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/models/xmlvalue.py
+-rw-r--r--   0        0        0        0 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/py.typed
+-rw-r--r--   0        0        0     1488 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/resources/0100-template-repo/template.json
+-rw-r--r--   0        0        0     1036 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/resources/0100-template-repo/template.xml
+-rw-r--r--   0        0        0    23808 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/resources/schema/data.xsd
+-rw-r--r--   0        0        0     2770 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/resources/schema/lists-only.json
+-rw-r--r--   0        0        0    41377 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/resources/schema/project.json
+-rw-r--r--   0        0        0    30964 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/resources/schema/properties-only.json
+-rw-r--r--   0        0        0     4341 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/resources/schema/resources-only.json
+-rw-r--r--   0        0        0       61 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/resources/start-stack/docker-compose.override.yml
+-rw-r--r--   0        0        0     2459 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/resources/start-stack/docker-compose.yml
+-rw-r--r--   0        0        0      164 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/resources/start-stack/start-stack-config.yml
+-rw-r--r--   0        0        0        0 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/utils/__init__.py
+-rw-r--r--   0        0        0    15142 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/utils/excel_to_json_lists.py
+-rw-r--r--   0        0        0     4912 2023-08-08 15:17:48.936975 dsp_tools-3.0.0/src/dsp_tools/utils/excel_to_json_project.py
+-rw-r--r--   0        0        0     8237 2023-08-08 15:17:48.940975 dsp_tools-3.0.0/src/dsp_tools/utils/excel_to_json_properties.py
+-rw-r--r--   0        0        0    10530 2023-08-08 15:17:48.940975 dsp_tools-3.0.0/src/dsp_tools/utils/excel_to_json_resources.py
+-rw-r--r--   0        0        0     1170 2023-08-08 15:17:48.940975 dsp_tools-3.0.0/src/dsp_tools/utils/generate_templates.py
+-rw-r--r--   0        0        0     3189 2023-08-08 15:17:48.940975 dsp_tools-3.0.0/src/dsp_tools/utils/id_to_iri.py
+-rw-r--r--   0        0        0     1424 2023-08-08 15:17:48.940975 dsp_tools-3.0.0/src/dsp_tools/utils/logging.py
+-rw-r--r--   0        0        0    45760 2023-08-08 15:17:48.940975 dsp_tools-3.0.0/src/dsp_tools/utils/project_create.py
+-rw-r--r--   0        0        0     8373 2023-08-08 15:17:48.940975 dsp_tools-3.0.0/src/dsp_tools/utils/project_create_lists.py
+-rw-r--r--   0        0        0     4694 2023-08-08 15:17:48.940975 dsp_tools-3.0.0/src/dsp_tools/utils/project_get.py
+-rw-r--r--   0        0        0    18815 2023-08-08 15:17:48.940975 dsp_tools-3.0.0/src/dsp_tools/utils/project_validate.py
+-rw-r--r--   0        0        0     4259 2023-08-08 15:17:48.940975 dsp_tools-3.0.0/src/dsp_tools/utils/rosetta.py
+-rw-r--r--   0        0        0    15582 2023-08-08 15:17:48.940975 dsp_tools-3.0.0/src/dsp_tools/utils/shared.py
+-rw-r--r--   0        0        0    14325 2023-08-08 15:17:48.940975 dsp_tools-3.0.0/src/dsp_tools/utils/stack_handling.py
+-rw-r--r--   0        0        0    52419 2023-08-08 15:17:48.940975 dsp_tools-3.0.0/src/dsp_tools/utils/xml_upload.py
+-rw-r--r--   0        0        0     6396 1970-01-01 00:00:00.000000 dsp_tools-3.0.0/PKG-INFO
```

### Comparing `dsp_tools-2.5.0/LICENSE` & `dsp_tools-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/docs/index.md` & `dsp_tools-3.0.0/docs/index.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,16 @@
-[![PyPI version](https://badge.fury.io/py/dsp-tools.svg)](https://badge.fury.io/py/dsp-tools)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
+[![](https://badge.fury.io/py/dsp-tools.svg)](https://badge.fury.io/py/dsp-tools) 
+[![](https://img.shields.io/pypi/pyversions/dsp-tools.svg)](https://pypi.org/project/dsp-tools/) 
+[![](https://img.shields.io/badge/Python%20code%20style-black-000000.svg)](https://github.com/psf/black) 
+[![](https://img.shields.io/badge/Python%20linting-pylint-darkgreen)](https://github.com/pylint-dev/pylint) 
+[![](https://img.shields.io/badge/Python%20typing-mypy-darkgreen)](https://github.com/python/mypy) 
+[![](https://img.shields.io/badge/Markdown%20linting-markdownlint-darkgreen)](
+  https://github.com/igorshubovych/markdownlint-cli) 
+[![](https://img.shields.io/badge/Link%20validation-markdown%20link%20validator-darkgreen)](
+  https://www.npmjs.com/package/markdown-link-validator)
 
 # DSP-TOOLS documentation
 
 DSP-TOOLS is a Python package with a command line interface 
 that helps you interact with a DSP server. 
 A DSP server is a remote server or a local machine 
 where the [DSP-API](https://github.com/dasch-swiss/dsp-api) is running on.
```

### Comparing `dsp_tools-2.5.0/pyproject.toml` & `dsp_tools-3.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # See https://packaging.python.org/en/latest/specifications/declaring-project-metadata
 
 [tool.poetry]
 name = "dsp-tools"
-version = "2.5.0"
+version = "3.0.0"
 description = "DSP-TOOLS is a Python package with a command line interface that helps you interact with a DaSCH service platform (DSP) server."
 authors = ["DaSCH - Swiss National Data and Service Center for the Humanities <info@dasch.swiss>"]
 readme = "docs/index.md"
 license = "GPL-3.0-only"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `dsp_tools-2.5.0/src/dsp_tools/dsp_tools.py` & `dsp_tools-3.0.0/src/dsp_tools/dsp_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,28 +140,26 @@
 
     # upload-files
     parser_upload_files = subparsers.add_parser(
         name="upload-files",
         help="For internal use only: upload already processed files",
     )
     parser_upload_files.set_defaults(action="upload-files")
-    parser_upload_files.add_argument("-f", "--pkl-file", help="path to pickle file written by 'process-files'")
     parser_upload_files.add_argument("-d", "--processed-dir", help="path to the directory with the processed files")
     parser_upload_files.add_argument("-n", "--nthreads", type=int, default=4, help="number of threads to use")
     parser_upload_files.add_argument("-s", "--server", default=default_dsp_api_url, help=dsp_server_text)
     parser_upload_files.add_argument("-u", "--user", default=root_user_email, help=username_text)
     parser_upload_files.add_argument("-p", "--password", default=root_user_pw, help=password_text)
 
     # fast-xmlupload
     parser_fast_xmlupload_files = subparsers.add_parser(
         name="fast-xmlupload",
         help="For internal use only: create resources with already uploaded files",
     )
     parser_fast_xmlupload_files.set_defaults(action="fast-xmlupload")
-    parser_fast_xmlupload_files.add_argument("-f", "--pkl-file", help="path to pickle file written by 'process-files'")
     parser_fast_xmlupload_files.add_argument("-s", "--server", default=default_dsp_api_url, help=dsp_server_text)
     parser_fast_xmlupload_files.add_argument("-u", "--user", default=root_user_email, help=username_text)
     parser_fast_xmlupload_files.add_argument("-p", "--password", default=root_user_pw, help=password_text)
     parser_fast_xmlupload_files.add_argument("xml_file", help="path to XML file containing the data")
 
     # excel2json
     parser_excel2json = subparsers.add_parser(
@@ -472,26 +470,24 @@
             output_dir=args.output_dir,
             xml_file=args.xml_file,
             nthreads=args.nthreads,
             batch_size=args.batchsize,
         )
     elif args.action == "upload-files":
         success = upload_files(
-            pkl_file=args.pkl_file,
             dir_with_processed_files=args.processed_dir,
             nthreads=args.nthreads,
             user=args.user,
             password=args.password,
             dsp_url=args.server,
             sipi_url=args.sipi_url,
         )
     elif args.action == "fast-xmlupload":
         success = fast_xmlupload(
             xml_file=args.xml_file,
-            pkl_file=args.pkl_file,
             user=args.user,
             password=args.password,
             dsp_url=args.server,
             sipi_url=args.sipi_url,
         )
     elif args.action == "excel2json":
         success = excel2json(
```

### Comparing `dsp_tools-2.5.0/src/dsp_tools/excel2xml.py` & `dsp_tools-3.0.0/src/dsp_tools/excel2xml.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/fast_xmlupload/process_files.py` & `dsp_tools-3.0.0/src/dsp_tools/fast_xmlupload/process_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,31 +16,34 @@
 import requests
 from docker.models.containers import Container
 from lxml import etree
 
 from dsp_tools.models.exceptions import UserError
 from dsp_tools.utils.logging import get_logger
 
+from dsp_tools.utils.shared import http_call_with_retry
+
 logger = get_logger(__name__, filesize_mb=100, backupcount=36)
 sipi_container: Optional[Container] = None
 export_moving_image_frames_script: Optional[Path] = None
 
 
 def _get_export_moving_image_frames_script() -> None:
     """
     Downloads the shell script that is used to extract the preview image from a video.
     """
     user_folder = Path.home() / Path(".dsp-tools/fast-xmlupload")
     user_folder.mkdir(parents=True, exist_ok=True)
     global export_moving_image_frames_script
     export_moving_image_frames_script = user_folder / "export-moving-image-frames.sh"
-    script_text = requests.get(
-        "https://github.com/dasch-swiss/dsp-api/raw/main/sipi/scripts/export-moving-image-frames.sh",
-        timeout=10,
-    ).text
+    script_text_response = http_call_with_retry(
+        action=requests.get,
+        url="https://github.com/dasch-swiss/dsp-api/raw/main/sipi/scripts/export-moving-image-frames.sh",
+    )
+    script_text = script_text_response.text
     with open(export_moving_image_frames_script, "w", encoding="utf-8") as f:
         f.write(script_text)
 
 
 def _determine_success_status_and_exit_code(
     files_to_process: list[Path],
     processed_files: list[tuple[Path, Optional[Path]]],
@@ -140,15 +143,16 @@
 
     Args:
         processed_files: the result of the file processing
 
     Raises:
         UserError if the file could not be written
     """
-    filename = f"processing_result_{datetime.now().strftime('%Y%m%d_%H%M%S')}.pkl"
+    filename = Path(f"processing_result_{datetime.now().strftime('%Y-%m-%d_%H.%M.%S.%f')}.pkl")
+
     try:
         with open(filename, "wb") as pkl_file:
             pickle.dump(processed_files, pkl_file)
         print(f"{datetime.now()}: The result was written to: {filename}")
     except OSError:
         err_msg = f"An error occurred while writing the result to the pickle file. Content of file: {processed_files}"
         logger.error(err_msg, exc_info=True)
```

### Comparing `dsp_tools-2.5.0/src/dsp_tools/fast_xmlupload/upload_files.py` & `dsp_tools-3.0.0/src/dsp_tools/fast_xmlupload/upload_files.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,21 +5,81 @@
 from pathlib import Path
 from typing import Optional
 
 import requests
 from regex import regex
 
 from dsp_tools.models.connection import Connection
-from dsp_tools.models.exceptions import BaseError
+from dsp_tools.models.exceptions import UserError
 from dsp_tools.utils.logging import get_logger
-from dsp_tools.utils.shared import login
+from dsp_tools.utils.shared import http_call_with_retry, login
 
 logger = get_logger(__name__)
 
 
+def _check_processed_dir(dir_with_processed_files: str) -> Path:
+    """
+    Checks the input parameter provided by the user and transforms it into a Path.
+
+    Args:
+        processed_dir: the directory where the processed files have been written to
+
+    Raises:
+        UserError: if the directory does not exist
+
+    Returns:
+        Path object of the directory
+    """
+    dir_with_processed_files_path = Path(dir_with_processed_files)
+    if not dir_with_processed_files_path.is_dir():
+        raise UserError(f"The folder with the processed files is invalid: {dir_with_processed_files}")
+    return dir_with_processed_files_path
+
+
+def get_pkl_files() -> list[Path]:
+    """
+    Get all pickle files starting with "processing_result_" in the current working directory.
+
+    Raises:
+        UserError: If no pickle file was found
+
+    Returns:
+        list of pickle files
+    """
+    pkl_file_paths = [Path(x) for x in glob.glob("processing_result_*.pkl")]
+    if len(pkl_file_paths) == 0:
+        raise UserError("No pickle file found. Please run the processing step first.")
+    return pkl_file_paths
+
+
+def _get_paths_from_pkl_files(pkl_files: list[Path]) -> list[Path]:
+    """
+    Read the pickle file(s) returned by the processing step.
+
+    Args:
+        pkl_files: pickle file(s) returned by the processing step
+
+    Returns:
+        list of file paths of the processed files (uuid filenames)
+    """
+    orig_paths_2_processed_paths: list[tuple[Path, Optional[Path]]] = []
+    for pkl_file in pkl_files:
+        orig_paths_2_processed_paths.extend(pickle.loads(pkl_file.read_bytes()))
+
+    processed_paths: list[Path] = []
+    for orig_path, processed_path in orig_paths_2_processed_paths:
+        if processed_path:
+            processed_paths.append(processed_path)
+        else:
+            print(f"{datetime.now()}: WARNING: There is no processed file for {orig_path}")
+            logger.warning(f"There is no processed file for {orig_path}")
+
+    return processed_paths
+
+
 def _get_upload_candidates(
     dir_with_processed_files: Path,
     internal_filename_of_processed_file: Path,
 ) -> list[Path]:
     """
     Based on the base derivate file, get all files based on the same uuid.
     For example, if the base derivate file is tmp/1f/fb/1ffbbb30-77e8-414c-94ff-7e1c060f9146.jp2,
@@ -106,19 +166,20 @@
 
     Returns:
         True if the file could be uploaded, False if an exception occurred.
     """
     try:
         with open(file, "rb") as bitstream:
             try:
-                response_upload = requests.post(
+                response_upload = http_call_with_retry(
+                    action=requests.post,
+                    initial_timeout=8 * 60,
                     url=f"{regex.sub(r'/$', '', sipi_url)}/upload_without_processing",
                     headers={"Authorization": f"Bearer {con.get_token()}"},
                     files={"file": bitstream},
-                    timeout=8 * 60,
                 )
             except Exception:  # pylint: disable=broad-exception-caught
                 err_msg = f"An exception was raised while calling the /upload_without_processing route for {file}"
                 print(f"{datetime.now()}: ERROR: {err_msg}")
                 logger.error(err_msg, exc_info=True)
                 return False
     except Exception:  # pylint: disable=broad-exception-caught
@@ -185,65 +246,14 @@
         logger.error(f"Could not upload all files for {internal_filename_of_processed_file}.")
         return internal_filename_of_processed_file, False
     else:
         logger.info(f"Successfully uploaded all files for {internal_filename_of_processed_file}.")
         return internal_filename_of_processed_file, True
 
 
-def _get_paths_from_pkl_file(pkl_file: Path) -> list[Path]:
-    """
-    Read the pickle file returned by the processing step.
-
-    Args:
-        pkl_file: pickle file returned by the processing step
-
-    Returns:
-        list of uuid file paths
-    """
-    with open(pkl_file, "rb") as file:
-        orig_paths_2_processed_paths: list[tuple[Path, Optional[Path]]] = pickle.load(file)
-
-    processed_paths: list[Path] = []
-    for orig_processed in orig_paths_2_processed_paths:
-        if orig_processed[1]:
-            processed_paths.append(orig_processed[1])
-        else:
-            print(f"{datetime.now()}: WARNING: There is no processed file for {orig_processed[0]}")
-            logger.warning(f"There is no processed file for {orig_processed[0]}")
-
-    return processed_paths
-
-
-def _check_params(
-    pkl_file: str,
-    dir_with_processed_files: str,
-) -> Optional[tuple[Path, Path]]:
-    """
-    Checks the input parameters provided by the user and transforms them into the expected types.
-
-    Args:
-        pkl_file: the XML file the paths are extracted from
-        processed_dir: the output directory where the created files should be written to
-
-    Returns:
-        A tuple with the Path objects of the input strings
-    """
-    pkl_file_path = Path(pkl_file)
-    dir_with_processed_files_path = Path(dir_with_processed_files)
-
-    if not pkl_file_path.is_file():
-        print(f"{pkl_file} is not a file")
-        return None
-    if not dir_with_processed_files_path.is_dir():
-        print(f"{dir_with_processed_files} is not a directory")
-        return None
-
-    return pkl_file_path, dir_with_processed_files_path
-
-
 def _upload_files_in_parallel(
     dir_with_processed_files: Path,
     internal_filenames_of_processed_files: list[Path],
     sipi_url: str,
     con: Connection,
     nthreads: int,
 ) -> list[tuple[Path, bool]]:
@@ -309,51 +319,42 @@
             print(f" - {path} could not be uploaded.")
             logger.error(f"{path} could not be uploaded.")
 
     return success
 
 
 def upload_files(
-    pkl_file: str,
     dir_with_processed_files: str,
     nthreads: int,
     user: str,
     password: str,
     dsp_url: str,
     sipi_url: str,
 ) -> bool:
     """
     Uploads the processed files to the DSP server, using multithreading.
     Before using this method, the files must be processed by the processing step.
 
     Args:
-        pkl_file: pickle file containing the mapping between the original files and the processed files,
         e.g. Path('multimedia/nested/subfolder/test.tif'), Path('tmp/0b/22/0b22570d-515f-4c3d-a6af-e42b458e7b2b.jp2').
         dir_with_processed_files: path to the directory where the processed files are located
         nthreads: number of threads to use for uploading (optimum depends on the number of CPUs on the server)
         user: the user's e-mail for login into DSP
         password: the user's password for login into DSP
         dsp_url: URL to the DSP server
         sipi_url: URL to the Sipi server
 
     Returns:
         success status
     """
-    # check the input parameters
-    param_check_result = _check_params(
-        pkl_file=pkl_file,
-        dir_with_processed_files=dir_with_processed_files,
-    )
-    if param_check_result:
-        pkl_file_path, dir_with_processed_files_path = param_check_result
-    else:
-        raise BaseError("Error reading the input parameters. Please check them.")
+    dir_with_processed_files_path = _check_processed_dir(dir_with_processed_files)
+    pkl_file_paths = get_pkl_files()
 
     # read paths from pkl file
-    internal_filenames_of_processed_files = _get_paths_from_pkl_file(pkl_file=pkl_file_path)
+    internal_filenames_of_processed_files = _get_paths_from_pkl_files(pkl_files=pkl_file_paths)
     print(f"{datetime.now()}: Found {len(internal_filenames_of_processed_files)} files to upload...")
     logger.info(f"Found {len(internal_filenames_of_processed_files)} files to upload...")
 
     # create connection to DSP
     con = login(
         server=dsp_url,
         user=user,
```

### Comparing `dsp_tools-2.5.0/src/dsp_tools/fast_xmlupload/upload_xml.py` & `dsp_tools-3.0.0/src/dsp_tools/fast_xmlupload/upload_xml.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,83 +1,85 @@
 import pickle
 from datetime import datetime
 from pathlib import Path
-from typing import Optional
+from typing import Optional, cast
 
 from lxml import etree
 
-from dsp_tools.models.exceptions import BaseError
+from dsp_tools.models.exceptions import UserError
 from dsp_tools.utils.logging import get_logger
 from dsp_tools.utils.xml_upload import xml_upload
 
+from dsp_tools.fast_xmlupload.upload_files import get_pkl_files
+
 logger = get_logger(__name__)
 
 
-def _get_paths_from_pkl_file(pkl_file: Path) -> dict[str, str]:
+def _get_paths_from_pkl_files(pkl_files: list[Path]) -> dict[str, str]:
     """
-    Read the pickle file returned by the processing step.
+    Read the pickle file(s) returned by the processing step.
 
     Args:
-        pkl_file: pickle file returned by the processing step
+        pkl_files: pickle file(s) returned by the processing step
+
+    Raises:
+        UserError: If for a file, no derivative was found
 
     Returns:
         dict of original paths to uuid filenames
     """
-    with open(pkl_file, "rb") as file:
-        orig_path_2_processed_path: list[tuple[Path, Optional[Path]]] = pickle.load(file)
+    orig_path_2_processed_path: list[tuple[Path, Optional[Path]]] = []
+    for pkl_file in pkl_files:
+        orig_path_2_processed_path.extend(pickle.loads(pkl_file.read_bytes()))
 
     orig_path_2_uuid_filename: dict[str, str] = {}
     for orig_path, processed_path in orig_path_2_processed_path:
         if processed_path:
             orig_path_2_uuid_filename[str(orig_path)] = str(processed_path.name)
         else:
-            raise BaseError(
+            raise UserError(
                 f"There is no processed file for {orig_path}. The fast xmlupload cannot be started, "
                 "because the resource that uses this file would fail."
             )
 
     return orig_path_2_uuid_filename
 
 
 def replace_bitstream_paths(
     xml_tree: "etree._ElementTree[etree._Element]",
     orig_path_2_uuid_filename: dict[str, str],
 ) -> "etree._ElementTree[etree._Element]":
     """
-    Replace the original filepaths in the <bitstream> Tags by the uuid filenames of the processed files.
+    Replace the original filepaths in the <bitstream> gags by the uuid filenames of the processed files.
 
     Args:
         xml_tree: The parsed original XML tree
         orig_path_2_uuid_filename: Mapping from original filenames to uuid filenames (from the pickle file)
 
     Raises:
-        BaseError: If for a file, no derivative was found
+        UserError: If for a file, no derivative was found
 
     Returns:
         The XML tree with the replaced filepaths (modified in place)
     """
     for elem in xml_tree.iter():
         if etree.QName(elem).localname.endswith("bitstream"):
             if elem.text in orig_path_2_uuid_filename:
                 elem.text = orig_path_2_uuid_filename[elem.text]
             else:
-                res_id = ""
-                res = elem.getparent()
-                if res:
-                    res_id = f"Resource {res.attrib['id']}: "
-                raise BaseError(
-                    f"{res_id}Cannot find processed derivatives for {elem.text}. The fast xmlupload cannot be started, "
-                    "because the resource that uses this file would fail."
+                res_id = cast("etree._Element", elem.getparent()).attrib.get("id")
+                raise UserError(
+                    f"Resource {res_id}: Cannot find processed derivatives for {elem.text}. "
+                    "The fast xmlupload cannot be started, because the resource that uses this file would fail."
                 )
     return xml_tree
 
 
 def fast_xmlupload(
     xml_file: str,
-    pkl_file: str,
     user: str,
     password: str,
     dsp_url: str,
     sipi_url: str,
 ) -> bool:
     """
     This function reads an XML file
@@ -85,26 +87,26 @@
     using the fast XML upload method.
     Before using this method,
     the original files must be processed by the processing step,
     and uploaded by the upoad step.
 
     Args:
         xml_file: path to XML file containing the resources
-        pkl_file: pickle file containing the mapping between the original files and the processed files,
         e.g. Path('multimedia/nested/subfolder/test.tif'), Path('tmp/0b/22/0b22570d-515f-4c3d-a6af-e42b458e7b2b.jp2')
         user: the user's e-mail for login into DSP
         password: the user's password for login into DSP
         dsp_url: URL to the DSP server
         sipi_url: URL to the Sipi server
 
     Returns:
         success status
     """
     xml_tree_orig = etree.parse(xml_file)
-    orig_path_2_uuid_filename = _get_paths_from_pkl_file(pkl_file=Path(pkl_file))
+    pkl_files = get_pkl_files()
+    orig_path_2_uuid_filename = _get_paths_from_pkl_files(pkl_files)
     xml_tree_replaced = replace_bitstream_paths(
         xml_tree=xml_tree_orig,
         orig_path_2_uuid_filename=orig_path_2_uuid_filename,
     )
 
     start_time = datetime.now()
     print(f"{start_time}: Start with fast XML upload...")
```

### Comparing `dsp_tools-2.5.0/src/dsp_tools/models/bitstream.py` & `dsp_tools-3.0.0/src/dsp_tools/models/bitstream.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/models/connection.py` & `dsp_tools-3.0.0/src/dsp_tools/models/connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         credentials = {"email": email, "password": password}
         jsondata = json.dumps(credentials)
 
         response = requests.post(
             self._server + "/v2/authentication",
             headers={"Content-Type": "application/json; charset=UTF-8"},
             data=jsondata,
-            timeout=10,
+            timeout=20,
         )
         check_for_api_error(response)
         result = response.json()
         self._token = result["token"]
 
     def get_token(self) -> str:
         """
@@ -101,15 +101,15 @@
         :return: None
         """
 
         if self._token is not None:
             response = requests.delete(
                 self._server + "/v2/authentication",
                 headers={"Authorization": "Bearer " + self._token},
-                timeout=10,
+                timeout=20,
             )
             check_for_api_error(response)
             self._token = None
 
     def __del__(self):
         pass
         # self.logout()
@@ -188,27 +188,27 @@
         :return: Response from server
         """
 
         if path[0] != "/":
             path = "/" + path
         if not self._token:
             if not headers:
-                response = requests.get(self._server + path, timeout=10)
+                response = requests.get(self._server + path, timeout=20)
             else:
-                response = requests.get(self._server + path, headers, timeout=10)
+                response = requests.get(self._server + path, headers, timeout=20)
         else:
             if not headers:
                 response = requests.get(
                     self._server + path,
                     headers={"Authorization": "Bearer " + self._token},
-                    timeout=10,
+                    timeout=20,
                 )
             else:
                 headers["Authorization"] = "Bearer " + self._token
-                response = requests.get(self._server + path, headers, timeout=10)
+                response = requests.get(self._server + path, headers, timeout=20)
 
         check_for_api_error(response)
         json_response = response.json()
         return json_response
 
     def put(self, path: str, jsondata: Optional[str] = None, content_type: str = "application/json"):
         """
@@ -221,22 +221,22 @@
 
         if path[0] != "/":
             path = "/" + path
         if jsondata is None:
             response = requests.put(
                 self._server + path,
                 headers={"Authorization": "Bearer " + self._token},
-                timeout=10,
+                timeout=20,
             )
         else:
             response = requests.put(
                 self._server + path,
                 headers={"Content-Type": content_type + "; charset=UTF-8", "Authorization": "Bearer " + self._token},
                 data=jsondata,
-                timeout=10,
+                timeout=20,
             )
         check_for_api_error(response)
         result = response.json()
         return result
 
     def delete(self, path: str, params: Optional[any] = None):
         """
@@ -248,19 +248,19 @@
         if path[0] != "/":
             path = "/" + path
         if params is not None:
             response = requests.delete(
                 self._server + path,
                 headers={"Authorization": "Bearer " + self._token},
                 params=params,
-                timeout=10,
+                timeout=20,
             )
 
         else:
             response = requests.delete(
                 self._server + path,
                 headers={"Authorization": "Bearer " + self._token},
-                timeout=10,
+                timeout=20,
             )
         check_for_api_error(response)
         result = response.json()
         return result
```

### Comparing `dsp_tools-2.5.0/src/dsp_tools/models/exceptions.py` & `dsp_tools-3.0.0/src/dsp_tools/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/models/group.py` & `dsp_tools-3.0.0/src/dsp_tools/models/group.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/models/helpers.py` & `dsp_tools-3.0.0/src/dsp_tools/models/helpers.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/models/langstring.py` & `dsp_tools-3.0.0/src/dsp_tools/models/langstring.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/models/listnode.py` & `dsp_tools-3.0.0/src/dsp_tools/models/listnode.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/models/ontology.py` & `dsp_tools-3.0.0/src/dsp_tools/models/ontology.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/models/permission.py` & `dsp_tools-3.0.0/src/dsp_tools/models/permission.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/models/project.py` & `dsp_tools-3.0.0/src/dsp_tools/models/project.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/models/projectContext.py` & `dsp_tools-3.0.0/src/dsp_tools/models/projectContext.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/models/propertyclass.py` & `dsp_tools-3.0.0/src/dsp_tools/models/propertyclass.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/models/propertyelement.py` & `dsp_tools-3.0.0/src/dsp_tools/models/propertyelement.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/models/resource.py` & `dsp_tools-3.0.0/src/dsp_tools/models/resource.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/models/resourceclass.py` & `dsp_tools-3.0.0/src/dsp_tools/models/resourceclass.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/models/user.py` & `dsp_tools-3.0.0/src/dsp_tools/models/user.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/models/value.py` & `dsp_tools-3.0.0/src/dsp_tools/models/value.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/models/xmlallow.py` & `dsp_tools-3.0.0/src/dsp_tools/models/xmlallow.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/models/xmlbitstream.py` & `dsp_tools-3.0.0/src/dsp_tools/models/xmlbitstream.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/models/xmlpermission.py` & `dsp_tools-3.0.0/src/dsp_tools/models/xmlpermission.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/models/xmlproperty.py` & `dsp_tools-3.0.0/src/dsp_tools/models/xmlproperty.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/models/xmlresource.py` & `dsp_tools-3.0.0/src/dsp_tools/models/xmlresource.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/models/xmlvalue.py` & `dsp_tools-3.0.0/src/dsp_tools/models/xmlvalue.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/resources/0100-template-repo/template.json` & `dsp_tools-3.0.0/src/dsp_tools/resources/0100-template-repo/template.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/resources/0100-template-repo/template.xml` & `dsp_tools-3.0.0/src/dsp_tools/resources/0100-template-repo/template.xml`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/resources/schema/data.xsd` & `dsp_tools-3.0.0/src/dsp_tools/resources/schema/data.xsd`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/resources/schema/lists-only.json` & `dsp_tools-3.0.0/src/dsp_tools/resources/schema/lists-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/resources/schema/project.json` & `dsp_tools-3.0.0/src/dsp_tools/resources/schema/project.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999970561594203%*

 * *Differences: {"'definitions'": "{'gui_element': {'enum': {delete: [11]}}, 'property': {'allOf': {7: {'then': "*

 * *                  "{'properties': {'gui_element': {'enum': {insert: [(0, 'Spinbox')], delete: "*

 * *                  "[0]}}}}}, 12: {'then': {'properties': {'gui_element': {replace: "*

 * *                  "OrderedDict([('const', 'Interval')])}}}}, delete: [18]}}}"}*

```diff
@@ -132,15 +132,14 @@
                 "Interval",
                 "List",
                 "Radio",
                 "Pulldown",
                 "Richtext",
                 "Searchbox",
                 "SimpleText",
-                "Slider",
                 "Spinbox",
                 "Textarea",
                 "TimeStamp"
             ],
             "type": "string"
         },
         "langstring": {
@@ -442,15 +441,15 @@
                             }
                         }
                     },
                     "then": {
                         "properties": {
                             "gui_element": {
                                 "enum": [
-                                    "Slider",
+                                    "Spinbox",
                                     "SimpleText"
                                 ]
                             },
                             "super": {
                                 "items": {
                                     "oneOf": [
                                         {
@@ -608,18 +607,15 @@
                                 "const": "IntervalValue"
                             }
                         }
                     },
                     "then": {
                         "properties": {
                             "gui_element": {
-                                "enum": [
-                                    "Interval",
-                                    "SimpleText"
-                                ]
+                                "const": "Interval"
                             },
                             "super": {
                                 "items": {
                                     "oneOf": [
                                         {
                                             "enum": [
                                                 "hasSequenceBounds"
@@ -770,42 +766,14 @@
                         }
                     }
                 },
                 {
                     "if": {
                         "properties": {
                             "gui_element": {
-                                "const": "Slider"
-                            }
-                        }
-                    },
-                    "then": {
-                        "properties": {
-                            "gui_attributes": {
-                                "additionalProperties": false,
-                                "properties": {
-                                    "max": {
-                                        "type": "number"
-                                    },
-                                    "min": {
-                                        "type": "number"
-                                    }
-                                },
-                                "type": "object"
-                            }
-                        },
-                        "required": [
-                            "gui_attributes"
-                        ]
-                    }
-                },
-                {
-                    "if": {
-                        "properties": {
-                            "gui_element": {
                                 "const": "Spinbox"
                             }
                         }
                     },
                     "then": {
                         "properties": {
                             "gui_attributes": {
```

### Comparing `dsp_tools-2.5.0/src/dsp_tools/resources/schema/properties-only.json` & `dsp_tools-3.0.0/src/dsp_tools/resources/schema/properties-only.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999158902691512%*

 * *Differences: {"'definitions'": "{'gui_element': {'enum': {delete: [11]}}, 'property': {'allOf': {7: {'then': "*

 * *                  "{'properties': {'gui_element': {'enum': {insert: [(0, 'Spinbox')], delete: "*

 * *                  "[0]}}}}}, 12: {'then': {'properties': {'gui_element': {replace: "*

 * *                  "OrderedDict([('const', 'Interval')])}}}}, delete: [18]}}}"}*

```diff
@@ -56,15 +56,14 @@
                 "Interval",
                 "List",
                 "Radio",
                 "Pulldown",
                 "Richtext",
                 "Searchbox",
                 "SimpleText",
-                "Slider",
                 "Spinbox",
                 "Textarea",
                 "TimeStamp"
             ],
             "type": "string"
         },
         "langstring": {
@@ -301,15 +300,15 @@
                             }
                         }
                     },
                     "then": {
                         "properties": {
                             "gui_element": {
                                 "enum": [
-                                    "Slider",
+                                    "Spinbox",
                                     "SimpleText"
                                 ]
                             },
                             "super": {
                                 "items": {
                                     "oneOf": [
                                         {
@@ -467,18 +466,15 @@
                                 "const": "IntervalValue"
                             }
                         }
                     },
                     "then": {
                         "properties": {
                             "gui_element": {
-                                "enum": [
-                                    "Interval",
-                                    "SimpleText"
-                                ]
+                                "const": "Interval"
                             },
                             "super": {
                                 "items": {
                                     "oneOf": [
                                         {
                                             "enum": [
                                                 "hasSequenceBounds"
@@ -629,42 +625,14 @@
                         }
                     }
                 },
                 {
                     "if": {
                         "properties": {
                             "gui_element": {
-                                "const": "Slider"
-                            }
-                        }
-                    },
-                    "then": {
-                        "properties": {
-                            "gui_attributes": {
-                                "additionalProperties": false,
-                                "properties": {
-                                    "max": {
-                                        "type": "number"
-                                    },
-                                    "min": {
-                                        "type": "number"
-                                    }
-                                },
-                                "type": "object"
-                            }
-                        },
-                        "required": [
-                            "gui_attributes"
-                        ]
-                    }
-                },
-                {
-                    "if": {
-                        "properties": {
-                            "gui_element": {
                                 "const": "Spinbox"
                             }
                         }
                     },
                     "then": {
                         "properties": {
                             "gui_attributes": {
```

### Comparing `dsp_tools-2.5.0/src/dsp_tools/resources/schema/resources-only.json` & `dsp_tools-3.0.0/src/dsp_tools/resources/schema/resources-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/resources/start-stack/docker-compose.yml` & `dsp_tools-3.0.0/src/dsp_tools/resources/start-stack/docker-compose.yml`

 * *Files 4% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 version: '3.7'
 
 services:
 
   app:
     # on the verge of every deployment (fortnightly), update the "image" value from the "app" value of
     # https://github.com/dasch-swiss/ops-deploy/blob/main/roles/dsp-deploy/files/RELEASE.json
-    image: daschswiss/dsp-app:v10.23.0
+    image: daschswiss/dsp-app:v10.23.1
     ports:
       - "4200:4200"
     networks:
       - knora-net
 
   db:
     # on the verge of every deployment (fortnightly), update the "image" value from the "db" value of
     # https://github.com/dasch-swiss/ops-deploy/blob/main/roles/dsp-deploy/files/RELEASE.json
-    image: daschswiss/apache-jena-fuseki:2.0.11
+    image: daschswiss/apache-jena-fuseki:2.1.0
     ports:
       - "3030:3030"
     networks:
       - knora-net
     environment:
       - TZ=Europe/Zurich
       - ADMIN_PASSWORD=test
       - JVM_ARGS=-Xmx3G
 
   sipi:
     # on the verge of every deployment (fortnightly), take the same tag as DSP-API
-    image: daschswiss/knora-sipi:29.1.1
+    image: daschswiss/knora-sipi:29.1.2
     ports:
       - "1024:1024"
     volumes:
       - .:/docker
     networks:
       - knora-net
     environment:
@@ -45,15 +45,15 @@
       - KNORA_WEBAPI_KNORA_API_EXTERNAL_HOST=0.0.0.0
       - KNORA_WEBAPI_KNORA_API_EXTERNAL_PORT=3333
     command: --config=/docker/sipi.docker-config.lua
 
   api:
     # on the verge of every deployment (fortnightly), update the "image" value from the "api" value of
     # https://github.com/dasch-swiss/ops-deploy/blob/main/roles/dsp-deploy/files/RELEASE.json
-    image: daschswiss/knora-api:29.1.1
+    image: daschswiss/knora-api:29.1.2
     depends_on:
       - sipi
       - db
     ports:
       - "3333:3333"
     networks:
       - knora-net
```

### Comparing `dsp_tools-2.5.0/src/dsp_tools/utils/excel_to_json_lists.py` & `dsp_tools-3.0.0/src/dsp_tools/utils/excel_to_json_lists.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/utils/excel_to_json_project.py` & `dsp_tools-3.0.0/src/dsp_tools/utils/excel_to_json_project.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/utils/excel_to_json_properties.py` & `dsp_tools-3.0.0/src/dsp_tools/utils/excel_to_json_properties.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/utils/excel_to_json_resources.py` & `dsp_tools-3.0.0/src/dsp_tools/utils/excel_to_json_resources.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/utils/generate_templates.py` & `dsp_tools-3.0.0/src/dsp_tools/utils/generate_templates.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/utils/id_to_iri.py` & `dsp_tools-3.0.0/src/dsp_tools/utils/id_to_iri.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/utils/logging.py` & `dsp_tools-3.0.0/src/dsp_tools/utils/logging.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/utils/project_create.py` & `dsp_tools-3.0.0/src/dsp_tools/utils/project_create.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,102 +20,119 @@
 from dsp_tools.utils.project_validate import validate_project
 from dsp_tools.utils.shared import login, parse_json_input, try_network_action
 
 logger = get_logger(__name__)
 
 
 def _create_project_on_server(
-    project_definition: dict[str, Any],
+    shortcode: str,
+    shortname: str,
+    longname: str,
+    descriptions: Optional[dict[str, str]],
+    keywords: Optional[list[str]],
     con: Connection,
     verbose: bool,
 ) -> tuple[Project, bool]:
     """
     Create the project on the DSP server.
     If it already exists: update its longname, description and keywords.
 
     Args:
-        project_definition: parsed JSON project definition
+        shortcode: shortcode of the project
+        shortname: shortname of the project
+        longname: longname of the project
+        descriptions: descriptions of the project in different languages
+        keywords: keywords of the project
         con: connection to the DSP server
         verbose: verbose switch
 
     Raises:
         UserError: if the project cannot be created on the DSP server
 
     Returns:
         a tuple of the remote project and the success status (True if everything went smoothly, False otherwise)
     """
     try:
         # the normal, expected case is that this try block fails
-        project_local = Project(con=con, shortcode=project_definition["project"]["shortcode"])
+        project_local = Project(con=con, shortcode=shortcode)
         project_remote: Project = try_network_action(project_local.read)
         proj_designation = f"'{project_remote.shortname}' ({project_remote.shortcode})"
         msg = f"Project {proj_designation} already exists on the DSP server. Updating it..."
         print(f"\tWARNING: {msg}")
         logger.warning(msg)
         # try to update the basic info
         project_remote, _ = _update_basic_info_of_project(
-            project=project_remote, project_definition=project_definition, verbose=verbose
+            project=project_remote,
+            shortcode=shortcode,
+            shortname=shortname,
+            longname=longname,
+            descriptions=descriptions,
+            keywords=keywords,
+            verbose=verbose,
         )
         # It doesn't matter if the update is successful or not: continue anyway, because success is anyways false.
         # There are other things from this file that can be created on the server,
         # e.g. the groups and users, so the process must continue.
         return project_remote, False
     except BaseError:
         pass
 
     success = True
     project_local = Project(
         con=con,
-        shortcode=project_definition["project"]["shortcode"],
-        shortname=project_definition["project"]["shortname"],
-        longname=project_definition["project"]["longname"],
-        description=LangString(project_definition["project"].get("descriptions")),
-        keywords=set(project_definition["project"].get("keywords")),
+        shortcode=shortcode,
+        shortname=shortname,
+        longname=longname,
+        description=LangString(descriptions),  # type: ignore[arg-type]
+        keywords=set(keywords) if keywords else None,
         selfjoin=False,
         status=True,
     )
     try:
         project_remote = try_network_action(project_local.create)
     except BaseError:
-        err_msg = (
-            f"Cannot create project '{project_definition['project']['shortname']}' "
-            f"({project_definition['project']['shortcode']}) on DSP server."
-        )
+        err_msg = f"Cannot create project '{shortname}' ({shortcode}) on DSP server."
         logger.error(err_msg, exc_info=True)
         raise UserError(err_msg) from None
     print(f"\tCreated project '{project_remote.shortname}' ({project_remote.shortcode}).")
     return project_remote, success
 
 
 def _update_basic_info_of_project(
     project: Project,
-    project_definition: dict[str, Any],
+    shortcode: str,
+    shortname: str,
+    longname: str,
+    descriptions: Optional[dict[str, str]],
+    keywords: Optional[list[str]],
     verbose: bool,
 ) -> tuple[Project, bool]:
     """
     Updates the longname, description and keywords of a project on a DSP server.
     Returns the updated project (or the unchanged project if not successful)
     and a boolean saying if the update was successful or not.
     If the update was not successful, an error message is printed to stdout.
 
     Args:
         project: the project to be updated (must exist on the DSP server)
-        project_definition: a parsed JSON project file with the same shortname and shortcode than the existing project
+        shortcode: shortcode of the project (must be the same as in the existing project)
+        shortname: shortname of the project (must be the same as in the existing project)
+        longname: longname of the project
+        descriptions: descriptions of the project in different languages
+        keywords: keywords of the project
+        verbose: verbose switch
 
     Returns:
         tuple of (updated project, success status)
     """
-    # store in variables for convenience
-    shortcode = project_definition["project"]["shortcode"]
-    shortname = project_definition["project"]["shortname"]
 
     # update the local "project" object
-    project.longname = project_definition["project"]["longname"]
-    project.description = project_definition["project"].get("descriptions")
-    project.keywords = project_definition["project"].get("keywords")
+    project.longname = longname
+    project.description = LangString(descriptions)  # type: ignore[arg-type]
+    project.keywords = set(keywords) if keywords else set()
 
     # make the call to DSP-API
     try:
         project_remote: Project = try_network_action(project.update)
         if verbose:
             print(f"\tUpdated project '{shortname}' ({shortcode}).")
         logger.info(f"Updated project '{shortname}' ({shortcode}).")
@@ -497,62 +514,66 @@
                 sorted_prop_classes.append(prop)
                 ok_propclass_names.append(prop_name)
                 prop_classes_to_sort.remove(prop)
     return sorted_prop_classes
 
 
 def _create_ontology(
-    ontology_definition: dict[str, Any],
+    onto_name: str,
+    onto_label: str,
+    onto_comment: Optional[str],
     project_ontologies: list[Ontology],
     con: Connection,
     project_remote: Project,
     context: Context,
     verbose: bool,
 ) -> Optional[Ontology]:
     """
     Create an ontology on the DSP server,
     and add the prefixes defined in the JSON file to its context.
     If the ontology already exists on the DSP server, it is skipped.
 
     Args:
-        ontology_definition: one ontology from the "ontologies" section of a parsed JSON project file
+        onto_name: name of the ontology
+        onto_label: label of the ontology
+        onto_comment: comment of the ontology
         project_ontologies: ontologies existing on the DSP server
         con: Connection to the DSP server
         project_remote: representation of the project on the DSP server
         context: prefixes and the ontology IRIs they stand for
         verbose: verbose switch
 
     Raises:
         UserError: if the ontology cannot be created on the DSP server
 
     Returns:
         representation of the created ontology on the DSP server, or None if it already existed
     """
     # skip if it already exists on the DSP server
-    if ontology_definition["name"] in [onto.name for onto in project_ontologies]:
-        print(f"\tWARNING: Ontology '{ontology_definition['name']}' already exists on the DSP server. Skipping...")
+    if onto_name in [onto.name for onto in project_ontologies]:
+        print(f"\tWARNING: Ontology '{onto_name}' already exists on the DSP server. Skipping...")
         return None
 
-    print(f"Create ontology '{ontology_definition['name']}'...")
+    print(f"Create ontology '{onto_name}'...")
     ontology_local = Ontology(
         con=con,
         project=project_remote,
-        label=ontology_definition["label"],
-        name=ontology_definition["name"],
-        comment=ontology_definition.get("comment"),
+        label=onto_label,
+        name=onto_name,
+        comment=onto_comment,
     )
     try:
         ontology_remote: Ontology = try_network_action(ontology_local.create)
     except BaseError:
         # if ontology cannot be created, let the error escalate
-        logger.error(f"ERROR while trying to create ontology '{ontology_definition['name']}'.", exc_info=True)
-        raise UserError(f"ERROR while trying to create ontology '{ontology_definition['name']}'.") from None
+        logger.error(f"ERROR while trying to create ontology '{onto_name}'.", exc_info=True)
+        raise UserError(f"ERROR while trying to create ontology '{onto_name}'.") from None
 
     if verbose:
-        print(f"\tCreated ontology '{ontology_definition['name']}'.")
+        print(f"\tCreated ontology '{onto_name}'.")
 
     context.add_context(
         ontology_remote.name,
         ontology_remote.iri + ("#" if not ontology_remote.iri.endswith("#") else ""),
     )
 
     # add the prefixes defined in the JSON file
@@ -564,30 +585,30 @@
     return ontology_remote
 
 
 def _create_ontologies(
     con: Connection,
     context: Context,
     knora_api_prefix: str,
-    list_root_nodes: dict[str, Any],
-    project_definition: dict[str, Any],
+    names_and_iris_of_list_nodes: dict[str, Any],
+    ontology_definitions: list[dict[str, Any]],
     project_remote: Project,
     verbose: bool,
 ) -> bool:
     """
     Iterates over the ontologies in a JSON project file and creates the ontologies that don't exist on the DSP server
     yet. For every ontology, it first creates the resource classes, then the properties, and then adds the cardinalities
     to the resource classes.
 
     Args:
         con: Connection to the DSP server
         context: prefixes and the ontology IRIs they stand for
         knora_api_prefix: the prefix that stands for the knora-api ontology
-        list_root_nodes: the IRIs of the list nodes that were already created and are now available on the DSP server
-        project_definition: the parsed JSON project file
+        names_and_iris_of_list_nodes: IRIs of list nodes that were already created and are available on the DSP server
+        ontology_definitions: the "ontologies" section of the parsed JSON project file
         project_remote: representation of the project on the DSP server
         verbose: verbose switch
 
     Raises:
         UserError if an error occurs during the creation of an ontology.
         All other errors are printed, the process continues, but the success status will be false.
 
@@ -604,97 +625,102 @@
         )
     except BaseError:
         err_msg = "Unable to retrieve remote ontologies. Cannot check if your ontology already exists."
         print("WARNING: {err_msg}")
         logger.warning(err_msg, exc_info=True)
         project_ontologies = []
 
-    for ontology_definition in project_definition.get("project", {}).get("ontologies", {}):
-        ontology_definition = cast(dict[str, Any], ontology_definition)
+    for ontology_definition in ontology_definitions:
         ontology_remote = _create_ontology(
-            ontology_definition=ontology_definition,
+            onto_name=ontology_definition["name"],
+            onto_label=ontology_definition["label"],
+            onto_comment=ontology_definition.get("comment"),
             project_ontologies=project_ontologies,
             con=con,
             project_remote=project_remote,
             context=context,
             verbose=verbose,
         )
         if not ontology_remote:
             overall_success = False
             continue
 
         # add the empty resource classes to the remote ontology
         last_modification_date, remote_res_classes, success = _add_resource_classes_to_remote_ontology(
-            ontology_definition=ontology_definition,
+            onto_name=ontology_definition["name"],
+            resclass_definitions=ontology_definition.get("resources", []),
             ontology_remote=ontology_remote,
             con=con,
             last_modification_date=ontology_remote.lastModificationDate,
             verbose=verbose,
         )
         if not success:
             overall_success = False
 
         # add the property classes to the remote ontology
         last_modification_date, success = _add_property_classes_to_remote_ontology(
-            ontology_definition=ontology_definition,
+            onto_name=ontology_definition["name"],
+            property_definitions=ontology_definition.get("properties", []),
             ontology_remote=ontology_remote,
-            list_root_nodes=list_root_nodes,
+            names_and_iris_of_list_nodes=names_and_iris_of_list_nodes,
             con=con,
             last_modification_date=last_modification_date,
             knora_api_prefix=knora_api_prefix,
             verbose=verbose,
         )
         if not success:
             overall_success = False
 
         # Add cardinalities to class
         success = _add_cardinalities_to_resource_classes(
-            ontology_definition=ontology_definition,
+            resclass_definitions=ontology_definition.get("resources", []),
             ontology_remote=ontology_remote,
             remote_res_classes=remote_res_classes,
             last_modification_date=last_modification_date,
             knora_api_prefix=knora_api_prefix,
             verbose=verbose,
         )
         if not success:
             overall_success = False
 
     return overall_success
 
 
 def _add_resource_classes_to_remote_ontology(
-    ontology_definition: dict[str, Any],
+    onto_name: str,
+    resclass_definitions: list[dict[str, Any]],
     ontology_remote: Ontology,
     con: Connection,
     last_modification_date: DateTimeStamp,
     verbose: bool,
 ) -> tuple[DateTimeStamp, dict[str, ResourceClass], bool]:
     """
     Creates the resource classes (without cardinalities) defined in the "resources" section of an ontology. The
     containing project and the containing ontology must already be existing on the DSP server.
     If an error occurs during creation of a resource class, it is printed out, the process continues, but the success
     status will be false.
 
     Args:
-        ontology_definition: the part of the parsed JSON project file that contains the current ontology
+        onto_name: name of the current ontology
+        resclass_definitions: the part of the parsed JSON project file that contains the resources of the current onto
         ontology_remote: representation of the current ontology on the DSP server
         con: connection to the DSP server
         last_modification_date: last modification date of the ontology on the DSP server
         verbose: verbose switch
 
     Returns:
         last modification date of the ontology,
         new resource classes,
         success status
     """
 
     overall_success = True
     print("\tCreate resource classes...")
     new_res_classes: dict[str, ResourceClass] = {}
-    sorted_resources = _sort_resources(ontology_definition["resources"], ontology_definition["name"])
+    sorted_resources = _sort_resources(resclass_definitions, onto_name)
     for res_class in sorted_resources:
         super_classes = res_class["super"]
         if isinstance(super_classes, str):
             super_classes = [super_classes]
         res_class_local = ResourceClass(
             con=con,
             context=ontology_remote.context,
@@ -718,43 +744,45 @@
             logger.warning(f"Unable to create resource class '{res_class['name']}'.", exc_info=True)
             overall_success = False
 
     return last_modification_date, new_res_classes, overall_success
 
 
 def _add_property_classes_to_remote_ontology(
-    ontology_definition: dict[str, Any],
+    onto_name: str,
+    property_definitions: list[dict[str, Any]],
     ontology_remote: Ontology,
-    list_root_nodes: dict[str, Any],
+    names_and_iris_of_list_nodes: dict[str, Any],
     con: Connection,
     last_modification_date: DateTimeStamp,
     knora_api_prefix: str,
     verbose: bool,
 ) -> tuple[DateTimeStamp, bool]:
     """
     Creates the property classes defined in the "properties" section of an ontology. The
     containing project and the containing ontology must already be existing on the DSP server.
     If an error occurs during creation of a property class, it is printed out, the process continues, but the success
     status will be false.
 
     Args:
-        ontology_definition: the part of the parsed JSON project file that contains the current ontology
+        onto_name: name of the current ontology
+        property_definitions: the part of the parsed JSON project file that contains the properties of the current onto
         ontology_remote: representation of the current ontology on the DSP server
-        list_root_nodes: the IRIs of the list nodes that were already created and are now available on the DSP server
+        names_and_iris_of_list_nodes: IRIs of list nodes that were already created and are available on the DSP server
         con: connection to the DSP server
         last_modification_date: last modification date of the ontology on the DSP server
         knora_api_prefix: the prefix that stands for the knora-api ontology
         verbose: verbose switch
 
     Returns:
         a tuple consisting of the last modification date of the ontology, and the success status
     """
     overall_success = True
     print("\tCreate property classes...")
-    sorted_prop_classes = _sort_prop_classes(ontology_definition["properties"], ontology_definition["name"])
+    sorted_prop_classes = _sort_prop_classes(property_definitions, onto_name)
     for prop_class in sorted_prop_classes:
         # get the super-property/ies, valid forms are:
         #   - "prefix:super-property" : fully qualified name of property in another ontology. The prefix has to be
         #     defined in the prefixes part.
         #   - ":super-property" : super-property defined in current ontology
         #   - "super-property" : super-property defined in the knora-api ontology
         #   - if omitted, "knora-api:hasValue" is assumed
@@ -775,17 +803,19 @@
         #   - "object_name" : The object is defined in "knora-api"
         if ":" in prop_class["object"]:
             prefix, _object = prop_class["object"].split(":")
             prop_object = f"{prefix}:{_object}" if prefix else f"{ontology_remote.name}:{_object}"
         else:
             prop_object = knora_api_prefix + prop_class["object"]
 
+        # get the gui_attributes
         gui_attributes = prop_class.get("gui_attributes")
         if gui_attributes and gui_attributes.get("hlist"):
-            gui_attributes["hlist"] = "<" + list_root_nodes[gui_attributes["hlist"]]["id"] + ">"
+            list_iri = names_and_iris_of_list_nodes[gui_attributes["hlist"]]["id"]
+            gui_attributes["hlist"] = f"<{list_iri}>"
 
         # create the property class
         prop_class_local = PropertyClass(
             con=con,
             context=ontology_remote.context,
             label=LangString(prop_class.get("labels")),
             name=prop_class["name"],
@@ -807,29 +837,29 @@
             logger.warning(f"Unable to create property class '{prop_class['name']}'.", exc_info=True)
             overall_success = False
 
     return last_modification_date, overall_success
 
 
 def _add_cardinalities_to_resource_classes(
-    ontology_definition: dict[str, Any],
+    resclass_definitions: list[dict[str, Any]],
     ontology_remote: Ontology,
     remote_res_classes: dict[str, ResourceClass],
     last_modification_date: DateTimeStamp,
     knora_api_prefix: str,
     verbose: bool,
 ) -> bool:
     """
     Iterates over the resource classes of an ontology of a JSON project definition, and adds the cardinalities to each
     resource class. The resource classes and the properties must already be existing on the DSP server.
     If an error occurs during creation of a cardinality, it is printed out, the process continues, but the success
     status will be false.
 
     Args:
-        ontology_definition: the part of the parsed JSON project file that contains the current ontology
+        resclass_definitions: the part of the parsed JSON project file that contains the resources of the current onto
         ontology_remote: representation of the current ontology on the DSP server
         remote_res_classes: representations of the resource classes on the DSP server
         last_modification_date: last modification date of the ontology on the DSP server
         knora_api_prefix: the prefix that stands for the knora-api ontology
         verbose: verbose switch
 
     Returns:
@@ -839,15 +869,15 @@
     print("\tAdd cardinalities to resource classes...")
     switcher = {
         "1": Cardinality.C_1,
         "0-1": Cardinality.C_0_1,
         "0-n": Cardinality.C_0_n,
         "1-n": Cardinality.C_1_n,
     }
-    for res_class in ontology_definition.get("resources", []):
+    for res_class in resclass_definitions:
         res_class_remote = remote_res_classes.get(ontology_remote.iri + "#" + res_class["name"])
         if not res_class_remote:
             print(
                 f"WARNING: Unable to add cardinalities to resource class '{res_class['name']}': "
                 f"This class doesn't exist on the DSP server."
             )
             overall_success = False
@@ -876,14 +906,70 @@
                 overall_success = False
 
             ontology_remote.lastModificationDate = last_modification_date
 
     return overall_success
 
 
+def _rectify_hlist_of_properties(
+    lists: list[dict[str, Any]],
+    properties: list[dict[str, Any]],
+) -> list[dict[str, Any]]:
+    """
+    Check the "hlist" of the "gui_attributes" of the properties.
+    If they don't refer to an existing list name,
+    check if there is a label of a list that corresponds to the "hlist".
+    If so, rectify the "hlist" to refer to the name of the list instead of the label.
+
+    Args:
+        lists: "lists" section of the JSON project definition
+        properties: "properties" section of one of the ontologies of the JSON project definition
+
+    Raises:
+        UserError: if the "hlist" refers to no existing list name or label
+
+    Returns:
+        the rectified "properties" section
+    """
+
+    if not lists or not properties:
+        return properties
+
+    existing_list_names = [l["name"] for l in lists]
+
+    for prop in properties:
+        if not prop.get("gui_attributes"):
+            continue
+        if not prop["gui_attributes"].get("hlist"):
+            continue
+        list_name = prop["gui_attributes"]["hlist"] if prop["gui_attributes"]["hlist"] in existing_list_names else None
+        if list_name:
+            continue
+
+        deduced_list_name = None
+        for root_node in lists:
+            if prop["gui_attributes"]["hlist"] in root_node["labels"].values():
+                deduced_list_name = cast(str, root_node["name"])
+        if deduced_list_name:
+            msg = (
+                f"INFO: Property '{prop['name']}' references the list '{prop['gui_attributes']['hlist']}' "
+                f"which is not a valid list name. "
+                f"Assuming that you meant '{deduced_list_name}' instead."
+            )
+            logger.warning(msg)
+            print(msg)
+        else:
+            msg = f"Property '{prop['name']}' references an unknown list: '{prop['gui_attributes']['hlist']}'"
+            logger.error(msg)
+            raise UserError(f"ERROR: {msg}")
+        prop["gui_attributes"]["hlist"] = deduced_list_name
+
+    return properties
+
+
 def create_project(
     project_file_as_path_or_parsed: Union[str, Path, dict[str, Any]],
     server: str,
     user_mail: str,
     password: str,
     verbose: bool,
     dump: bool,
@@ -929,35 +1015,47 @@
     new_lists = expand_lists_from_excel(project_definition.get("project", {}).get("lists", []))
     if new_lists:
         project_definition["project"]["lists"] = new_lists
 
     # validate against JSON schema
     validate_project(project_definition, expand_lists=False)
     print("\tJSON project file is syntactically correct and passed validation.")
-    print(f"Create project '{proj_shortname}' ({proj_shortcode})...")
+
+    # rectify the "hlist" of the "gui_attributes" of the properties
+    for onto in project_definition["project"]["ontologies"]:
+        if onto.get("properties"):
+            onto["properties"] = _rectify_hlist_of_properties(
+                lists=project_definition["project"].get("lists", []),
+                properties=onto["properties"],
+            )
 
     # establish connection to DSP server
     con = login(server=server, user=user_mail, password=password)
     if dump:
         con.start_logging()
 
     # create project on DSP server
+    print(f"Create project '{proj_shortname}' ({proj_shortcode})...")
     project_remote, success = _create_project_on_server(
-        project_definition=project_definition,
+        shortcode=project_definition["project"]["shortcode"],
+        shortname=project_definition["project"]["shortname"],
+        longname=project_definition["project"]["longname"],
+        descriptions=project_definition["project"].get("descriptions"),
+        keywords=project_definition["project"].get("keywords"),
         con=con,
         verbose=verbose,
     )
     if not success:
         overall_success = False
 
     # create the lists
-    list_root_nodes: dict[str, Any] = {}
+    names_and_iris_of_list_nodes: dict[str, Any] = {}
     if project_definition["project"].get("lists"):
         print("Create lists...")
-        list_root_nodes, success = create_lists_on_server(
+        names_and_iris_of_list_nodes, success = create_lists_on_server(
             lists_to_create=project_definition["project"]["lists"],
             con=con,
             project_remote=project_remote,
         )
         if not success:
             overall_success = False
 
@@ -987,16 +1085,16 @@
             overall_success = False
 
     # create the ontologies
     success = _create_ontologies(
         con=con,
         context=context,
         knora_api_prefix=knora_api_prefix,
-        list_root_nodes=list_root_nodes,
-        project_definition=project_definition,
+        names_and_iris_of_list_nodes=names_and_iris_of_list_nodes,
+        ontology_definitions=project_definition["project"]["ontologies"],
         project_remote=project_remote,
         verbose=verbose,
     )
     if not success:
         overall_success = False
 
     # final steps
```

### Comparing `dsp_tools-2.5.0/src/dsp_tools/utils/project_create_lists.py` & `dsp_tools-3.0.0/src/dsp_tools/utils/project_create_lists.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/utils/project_get.py` & `dsp_tools-3.0.0/src/dsp_tools/utils/project_get.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/utils/project_validate.py` & `dsp_tools-3.0.0/src/dsp_tools/utils/project_validate.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/utils/rosetta.py` & `dsp_tools-3.0.0/src/dsp_tools/utils/rosetta.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/src/dsp_tools/utils/shared.py` & `dsp_tools-3.0.0/src/dsp_tools/utils/shared.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 import copy
 import importlib.resources
 import json
 import time
 import unicodedata
 from datetime import datetime
 from pathlib import Path
-from typing import Any, Callable, Optional, Union
+from typing import Any, Callable, Optional, Union, cast
 
 import pandas as pd
 import regex
 from lxml import etree
 from requests import ReadTimeout, RequestException
+import requests
+from urllib3.exceptions import ReadTimeoutError
 
 from dsp_tools.models.connection import Connection
 from dsp_tools.models.exceptions import BaseError, UserError
 from dsp_tools.models.propertyelement import PropertyElement
 from dsp_tools.utils.logging import get_logger
 
 logger = get_logger(__name__)
@@ -48,22 +50,74 @@
         try_network_action(lambda: con.login(email=user, password=password))
     except BaseError:
         logger.error("Cannot login to DSP server", exc_info=True)
         raise UserError("Cannot login to DSP server") from None
     return con
 
 
+def http_call_with_retry(
+    action: Callable[..., Any],
+    *args: Any,
+    initial_timeout: int = 10,
+    **kwargs: Any,
+) -> requests.Response:
+    """
+    Function that tries 7 times to execute an HTTP request.
+    Timeouts (and only timeouts) are catched, and the request is retried after a waiting time.
+    The waiting times are 1, 2, 4, 8, 16, 32, 64 seconds.
+    Every time, the previous timeout is increased by 10 seconds.
+    Use this only for actions that can be retried without side effects.
+
+    Args:
+        action: one of requests.get(), requests.post(), requests.put(), requests.delete()
+        initial_timeout: Timeout to start with. Defaults to 10 seconds.
+
+    Raises:
+        errors from the requests library that are not timeouts
+
+    Returns:
+        response of the HTTP request
+    """
+    if action not in (requests.get, requests.post, requests.put, requests.delete):
+        raise BaseError(
+            "This function can only be used with the methods get, post, put, and delete of the Python requests library."
+        )
+    action_as_str = f"action='{action}', args='{args}', kwargs='{kwargs}'"
+    timeout = initial_timeout
+    for i in range(7):
+        try:
+            if args and not kwargs:
+                result = action(*args, timeout=timeout)
+            elif kwargs and not args:
+                result = action(**kwargs, timeout=timeout)
+            elif args and kwargs:
+                result = action(*args, **kwargs, timeout=timeout)
+            else:
+                result = action(timeout=timeout)
+            return cast(requests.Response, result)
+        except (TimeoutError, ReadTimeout, ReadTimeoutError):
+            timeout += 10
+            msg = f"Timeout Error: Retry request with timeout {timeout} in {2 ** i} seconds..."
+            print(f"{datetime.now().isoformat()}: {msg}")
+            logger.error(f"{msg} {action_as_str} (retry-counter i={i})", exc_info=True)
+            time.sleep(2**i)
+            continue
+
+    logger.error("Permanently unable to execute the API call. See logs for more details.")
+    raise BaseError("Permanently unable to execute the API call. See logs for more details.")
+
+
 def try_network_action(
     action: Callable[..., Any],
     *args: Any,
     **kwargs: Any,
 ) -> Any:
     """
     Helper method that tries 7 times to execute an action.
-    If a ConnectionError, a requests.exceptions.RequestException, or a non-permanent BaseError occors,
+    If a timeout error, a ConnectionError, a requests.exceptions.RequestException, or a non-permanent BaseError occors,
     it waits and retries.
     The waiting times are 1, 2, 4, 8, 16, 32, 64 seconds.
     If another exception occurs, it escalates.
 
     Args:
         action: a lambda with the code to be executed, or a function
         args: positional arguments for the action
```

### Comparing `dsp_tools-2.5.0/src/dsp_tools/utils/stack_handling.py` & `dsp_tools-3.0.0/src/dsp_tools/utils/stack_handling.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 import requests
 import yaml
 
 from dsp_tools.models.exceptions import UserError
 from dsp_tools.utils.logging import get_logger
 
+from dsp_tools.utils.shared import http_call_with_retry
+
 logger = get_logger(__name__)
 
 
 @dataclass
 class StackConfiguration:
     """
     Groups together configuration information for the StackHandler.
@@ -117,15 +119,19 @@
         """
         Retrieve the config file sipi.docker-config.lua from the DSP-API repository,
         and set the max_file_size parameter if necessary.
 
         Raises:
             UserError: if max_file_size is set but cannot be injected into sipi.docker-config.lua
         """
-        docker_config_lua_text = requests.get(f"{self.__url_prefix}sipi/config/sipi.docker-config.lua", timeout=10).text
+        docker_config_lua_response = http_call_with_retry(
+            action=requests.get,
+            url=f"{self.__url_prefix}sipi/config/sipi.docker-config.lua",
+        )
+        docker_config_lua_text = docker_config_lua_response.text
         if self.__stack_configuration.max_file_size:
             max_post_size_regex = r"max_post_size ?= ?[\'\"]\d+M[\'\"]"
             if not re.search(max_post_size_regex, docker_config_lua_text):
                 raise UserError("Unable to set max_file_size. Please try again without this flag.")
             docker_config_lua_text = re.sub(
                 max_post_size_regex,
                 f"max_post_size = '{self.__stack_configuration.max_file_size}M'",
@@ -155,39 +161,45 @@
     def _wait_for_fuseki(self) -> None:
         """
         Wait up to 6 minutes, until the fuseki database is up and running.
         This function imitates the behaviour of the script dsp-api/webapi/scripts/wait-for-db.sh.
         """
         for _ in range(6 * 60):
             try:
-                response = requests.get(url="http://0.0.0.0:3030/$/server", auth=("admin", "test"), timeout=10)
+                response = http_call_with_retry(
+                    action=requests.get,
+                    url="http://0.0.0.0:3030/$/server",
+                    auth=("admin", "test"),
+                )
                 if response.ok:
                     break
             except Exception:  # pylint: disable=broad-exception-caught
                 time.sleep(1)
             time.sleep(1)
 
     def _create_knora_test_repo(self) -> None:
         """
         Inside fuseki, create the "knora-test" repository.
         This function imitates the behaviour of the script dsp-api/webapi/scripts/fuseki-init-knora-test.sh.
 
         Raises:
             UserError: in case of failure
         """
-        repo_template = requests.get(
-            f"{self.__url_prefix}webapi/scripts/fuseki-repository-config.ttl.template",
-            timeout=10,
-        ).text
+        repo_template_response = http_call_with_retry(
+            action=requests.get,
+            url=f"{self.__url_prefix}webapi/scripts/fuseki-repository-config.ttl.template",
+        )
+        repo_template = repo_template_response.text
         repo_template = repo_template.replace("@REPOSITORY@", "knora-test")
-        response = requests.post(
+        response = http_call_with_retry(
+            action=requests.post,
+            initial_timeout=10,
             url="http://0.0.0.0:3030/$/datasets",
             files={"file": ("file.ttl", repo_template, "text/turtle; charset=utf8")},
             auth=("admin", "test"),
-            timeout=10,
         )
         if not response.ok:
             msg = (
                 "Cannot start DSP-API: Error when creating the 'knora-test' repository. "
                 "Is DSP-API perhaps running already?"
             )
             logger.error(f"{msg}. response = {vars(response)}")
@@ -211,25 +223,26 @@
             ("knora-ontologies/salsah-gui.ttl", "http://www.knora.org/ontology/salsah-gui"),
             ("test_data/project_data/admin-data.ttl", "http://www.knora.org/data/admin"),
             ("test_data/project_data/permissions-data.ttl", "http://www.knora.org/data/permissions"),
             ("test_data/project_ontologies/anything-onto.ttl", "http://www.knora.org/ontology/0001/anything"),
             ("test_data/project_data/anything-data.ttl", "http://www.knora.org/data/0001/anything"),
         ]
         for ttl_file, graph in ttl_files:
-            ttl_text_response = requests.get(self.__url_prefix + ttl_file, timeout=10)
-            if not ttl_text_response.ok:
+            ttl_response = http_call_with_retry(action=requests.get, url=self.__url_prefix + ttl_file)
+            if not ttl_response.ok:
                 msg = f"Cannot start DSP-API: Error when retrieving '{self.__url_prefix + ttl_file}'"
-                logger.error(f"{msg}'. response = {vars(ttl_text_response)}")
+                logger.error(f"{msg}'. response = {vars(ttl_response)}")
                 raise UserError(msg)
-            ttl_text = ttl_text_response.text
-            response = requests.post(
+            ttl_text = ttl_response.text
+            response = http_call_with_retry(
+                action=requests.post,
+                initial_timeout=10,
                 url=graph_prefix + graph,
                 files={"file": ("file.ttl", ttl_text, "text/turtle; charset: utf-8")},
                 auth=("admin", "test"),
-                timeout=10,
             )
             if not response.ok:
                 logger.error(f"Cannot start DSP-API: Error when creating graph '{graph}'. response = {vars(response)}")
                 raise UserError(f"Cannot start DSP-API: Error when creating graph '{graph}'")
 
     def _initialize_fuseki(self) -> None:
         """
```

### Comparing `dsp_tools-2.5.0/src/dsp_tools/utils/xml_upload.py` & `dsp_tools-3.0.0/src/dsp_tools/utils/xml_upload.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-2.5.0/PKG-INFO` & `dsp_tools-3.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsp-tools
-Version: 2.5.0
+Version: 3.0.0
 Summary: DSP-TOOLS is a Python package with a command line interface that helps you interact with a DaSCH service platform (DSP) server.
 Home-page: https://www.dasch.swiss/
 License: GPL-3.0-only
 Author: DaSCH - Swiss National Data and Service Center for the Humanities
 Author-email: info@dasch.swiss
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -24,17 +24,23 @@
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: regex (>=2023.5.5,<2024.0.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
 Project-URL: Documentation, https://docs.dasch.swiss/latest/DSP-TOOLS/
 Project-URL: Repository, https://github.com/dasch-swiss/dsp-tools
 Description-Content-Type: text/markdown
 
-[![PyPI version](https://badge.fury.io/py/dsp-tools.svg)](https://badge.fury.io/py/dsp-tools)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
+[![](https://badge.fury.io/py/dsp-tools.svg)](https://badge.fury.io/py/dsp-tools) 
+[![](https://img.shields.io/pypi/pyversions/dsp-tools.svg)](https://pypi.org/project/dsp-tools/) 
+[![](https://img.shields.io/badge/Python%20code%20style-black-000000.svg)](https://github.com/psf/black) 
+[![](https://img.shields.io/badge/Python%20linting-pylint-darkgreen)](https://github.com/pylint-dev/pylint) 
+[![](https://img.shields.io/badge/Python%20typing-mypy-darkgreen)](https://github.com/python/mypy) 
+[![](https://img.shields.io/badge/Markdown%20linting-markdownlint-darkgreen)](
+  https://github.com/igorshubovych/markdownlint-cli) 
+[![](https://img.shields.io/badge/Link%20validation-markdown%20link%20validator-darkgreen)](
+  https://www.npmjs.com/package/markdown-link-validator)
 
 # DSP-TOOLS documentation
 
 DSP-TOOLS is a Python package with a command line interface 
 that helps you interact with a DSP server. 
 A DSP server is a remote server or a local machine 
 where the [DSP-API](https://github.com/dasch-swiss/dsp-api) is running on.
```

