# Comparing `tmp/ntia_conformance_checker-0.4.0.tar.gz` & `tmp/ntia_conformance_checker-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntia_conformance_checker-0.4.0.tar", last modified: Thu Jul 27 17:32:59 2023, max compression
+gzip compressed data, was "ntia_conformance_checker-0.5.0.tar", last modified: Tue Aug  8 18:54:07 2023, max compression
```

## Comparing `ntia_conformance_checker-0.4.0.tar` & `ntia_conformance_checker-0.5.0.tar`

### file list

```diff
@@ -1,192 +1,192 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:32:59.403746 ntia_conformance_checker-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:32:59.335744 ntia_conformance_checker-0.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:32:59.335744 ntia_conformance_checker-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/.github/workflows/bandit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:32:59.339744 ntia_conformance_checker-0.4.0/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/.idea/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:32:59.339744 ntia_conformance_checker-0.4.0/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/.idea/ntia-conformance-checker.iml
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/FAQ.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-07-27 17:32:59.403746 ntia_conformance_checker-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/bandit.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:32:59.339744 ntia_conformance_checker-0.4.0/ntia_conformance_checker/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/ntia_conformance_checker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/ntia_conformance_checker/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    12701 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/ntia_conformance_checker/sbom_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:32:59.339744 ntia_conformance_checker-0.4.0/ntia_conformance_checker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-07-27 17:32:59.000000 ntia_conformance_checker-0.4.0/ntia_conformance_checker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-07-27 17:32:59.000000 ntia_conformance_checker-0.4.0/ntia_conformance_checker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 17:32:59.000000 ntia_conformance_checker-0.4.0/ntia_conformance_checker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-27 17:32:59.000000 ntia_conformance_checker-0.4.0/ntia_conformance_checker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-27 17:32:59.000000 ntia_conformance_checker-0.4.0/ntia_conformance_checker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 17:32:59.000000 ntia_conformance_checker-0.4.0/ntia_conformance_checker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 17:32:59.403746 ntia_conformance_checker-0.4.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      164 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:32:59.339744 ntia_conformance_checker-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:32:59.331744 ntia_conformance_checker-0.4.0/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:32:59.343744 ntia_conformance_checker-0.4.0/tests/data/SPDXSBOMExampleTests/
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingAuthorName.spdx.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingComponentName.spdx.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingComponentVersion.spdx.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingDependencyRelationships.spdx.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingSupplierName.spdx.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingUniqueIdentifiers.spdx.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/SPDXSBOMExampleTests/alpine.spdx
--rw-r--r--   0 runner    (1001) docker     (123)    25506 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/SPDXSBOMExampleTests/bom-alpine-3.15.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)    27752 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/SPDXSBOMExampleTests/photon.spdx.tag
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:32:59.347744 ntia_conformance_checker-0.4.0/tests/data/missing_author_name/
--rw-r--r--   0 runner    (1001) docker     (123)    19246 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/missing_author_name/SPDXJSONExample-v2.3.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)    35758 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/missing_author_name/SPDXRdfExample-v2.3.spdx.rdf.xml
--rw-r--r--   0 runner    (1001) docker     (123)    16603 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/missing_author_name/SPDXTagExample-v2.3.spdx
--rw-r--r--   0 runner    (1001) docker     (123)    21925 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/missing_author_name/SPDXXMLExample-v2.3.spdx.xml
--rw-r--r--   0 runner    (1001) docker     (123)    18436 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/missing_author_name/SPDXYAMLExample-v2.3.spdx.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:32:59.347744 ntia_conformance_checker-0.4.0/tests/data/missing_component_name/
--rw-r--r--   0 runner    (1001) docker     (123)    17427 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/missing_component_name/SPDXJsonExample.json
--rw-r--r--   0 runner    (1001) docker     (123)    17744 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/missing_component_name/SPDXRdfExample.rdf
--rw-r--r--   0 runner    (1001) docker     (123)    15054 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/missing_component_name/SPDXXmlExample.xml
--rw-r--r--   0 runner    (1001) docker     (123)    13726 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/missing_component_name/SPDXYamlExample.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:32:59.347744 ntia_conformance_checker-0.4.0/tests/data/missing_component_version/
--rw-r--r--   0 runner    (1001) docker     (123)    19301 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/missing_component_version/SPDXJSONExample-v2.3.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)    36044 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/missing_component_version/SPDXRdfExample-v2.3.spdx.rdf.xml
--rw-r--r--   0 runner    (1001) docker     (123)    16670 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/missing_component_version/SPDXTagExample-v2.3.spdx
--rw-r--r--   0 runner    (1001) docker     (123)    22006 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/missing_component_version/SPDXXMLExample-v2.3.spdx.xml
--rw-r--r--   0 runner    (1001) docker     (123)    18504 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/missing_component_version/SPDXYAMLExample-v2.3.spdx.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:32:59.351744 ntia_conformance_checker-0.4.0/tests/data/missing_dependency_relationships/
--rw-r--r--   0 runner    (1001) docker     (123)    18333 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/missing_dependency_relationships/SPDXJSONExample-v2.3.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)    15463 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/missing_dependency_relationships/SPDXRdfExample-v2.3.spdx.rdf.xml
--rw-r--r--   0 runner    (1001) docker     (123)    16304 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/missing_dependency_relationships/SPDXTagExample-v2.3.spdx
--rw-r--r--   0 runner    (1001) docker     (123)    20074 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/missing_dependency_relationships/SPDXXMLExample-v2.3.spdx.xml
--rw-r--r--   0 runner    (1001) docker     (123)    17453 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/missing_dependency_relationships/SPDXYAMLExample-v2.3.spdx.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:32:59.351744 ntia_conformance_checker-0.4.0/tests/data/missing_supplier_name/
--rw-r--r--   0 runner    (1001) docker     (123)    20983 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/missing_supplier_name/SPDXJSONExample-v2.3.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)    40234 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/missing_supplier_name/SPDXRdfExample-v2.3.spdx.rdf.xml
--rw-r--r--   0 runner    (1001) docker     (123)    17892 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/missing_supplier_name/SPDXTagExample-v2.3.spdx
--rw-r--r--   0 runner    (1001) docker     (123)    24068 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/missing_supplier_name/SPDXXMLExample-v2.3.spdx.xml
--rw-r--r--   0 runner    (1001) docker     (123)    19863 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/missing_supplier_name/SPDXYAMLExample-v2.3.spdx.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:32:59.355744 ntia_conformance_checker-0.4.0/tests/data/missing_timestamp/
--rw-r--r--   0 runner    (1001) docker     (123)    19312 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/missing_timestamp/SPDXJSONExample-v2.3.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)    35921 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/missing_timestamp/SPDXRdfExample-v2.3.spdx.rdf.xml
--rw-r--r--   0 runner    (1001) docker     (123)    16672 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/missing_timestamp/SPDXTagExample-v2.3.spdx
--rw-r--r--   0 runner    (1001) docker     (123)    22022 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/missing_timestamp/SPDXXMLExample-v2.3.spdx.xml
--rw-r--r--   0 runner    (1001) docker     (123)    18503 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/missing_timestamp/SPDXYAMLExample-v2.3.spdx.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:32:59.355744 ntia_conformance_checker-0.4.0/tests/data/missing_unique_identifiers/
--rw-r--r--   0 runner    (1001) docker     (123)    19298 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/missing_unique_identifiers/SPDXJSONExample-v2.3.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)    34397 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/missing_unique_identifiers/SPDXRdfExample-v2.3.spdx.rdf.xml
--rw-r--r--   0 runner    (1001) docker     (123)    16654 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/missing_unique_identifiers/SPDXTagExample-v2.3.spdx
--rw-r--r--   0 runner    (1001) docker     (123)    21947 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/missing_unique_identifiers/SPDXXMLExample-v2.3.spdx.xml
--rw-r--r--   0 runner    (1001) docker     (123)    18448 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/missing_unique_identifiers/SPDXYAMLExample-v2.3.spdx.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:32:59.355744 ntia_conformance_checker-0.4.0/tests/data/no_elements_missing/
--rw-r--r--   0 runner    (1001) docker     (123)    19332 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/no_elements_missing/SPDXJSONExample-v2.3.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)    35941 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/no_elements_missing/SPDXRdfExample-v2.3.spdx.rdf.xml
--rw-r--r--   0 runner    (1001) docker     (123)    16693 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/no_elements_missing/SPDXTagExample-v2.3.spdx
--rw-r--r--   0 runner    (1001) docker     (123)    22042 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/no_elements_missing/SPDXXMLExample-v2.3.spdx.xml
--rw-r--r--   0 runner    (1001) docker     (123)    18526 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/no_elements_missing/SPDXYAMLExample-v2.3.spdx.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:32:59.355744 ntia_conformance_checker-0.4.0/tests/data/other_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/other_tests/SPDXSBOMExample.spdx.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/data/other_tests/SPDXSimpleTag.tag
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:32:59.331744 ntia_conformance_checker-0.4.0/tests/doc_fest/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:32:59.359744 ntia_conformance_checker-0.4.0/tests/doc_fest/FOSSology/
--rw-r--r--   0 runner    (1001) docker     (123)   265354 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/FOSSology/SPDX2TV_PyYAML-6.0.tar.gz.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (123)   265322 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/FOSSology/SPDX2TV_PyYAML-6.0.tar.gz_v2 (1).spdx.tag
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:32:59.371745 ntia_conformance_checker-0.4.0/tests/doc_fest/Kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/Kubernetes/kubernetes-appbomination.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (123)    25724 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/Kubernetes/kubernetes-frederick-serve.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (123) 10020640 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/Kubernetes/kubernetes-keycloak.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (123)    58486 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/Kubernetes/kubernetes-pyyaml.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (123)   177744 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/Kubernetes/kubernetes-time.spdx.tag
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:32:59.371745 ntia_conformance_checker-0.4.0/tests/doc_fest/MetaSpdxscanner/
--rw-r--r--   0 runner    (1001) docker     (123)    31194 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/MetaSpdxscanner/app-bom-ination-1.0.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (123)   298947 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/MetaSpdxscanner/python3-pyyaml-6.0.spdx.tag
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:32:59.379745 ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/python3-pyyaml-dbg.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/python3-pyyaml-dev.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/python3-pyyaml-src.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)    42218 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/python3-pyyaml.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)   440190 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/recipe-python3-pyyaml.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)   112550 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/recipe-time.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/runtime-python3-pyyaml-dbg.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/runtime-python3-pyyaml-dev.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/runtime-python3-pyyaml-src.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/runtime-python3-pyyaml.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/runtime-time-dbg.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/runtime-time-dev.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/runtime-time-doc.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/runtime-time-src.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/runtime-time.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/time-dbg.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/time-dev.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/time-doc.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/time-src.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/time.spdx.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:32:59.379745 ntia_conformance_checker-0.4.0/tests/doc_fest/Philips/
--rw-r--r--   0 runner    (1001) docker     (123)   243446 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/Philips/keyclock_sbom.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:32:59.379745 ntia_conformance_checker-0.4.0/tests/doc_fest/REA/
--rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/REA/AppBOM-inationSBOM.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (123)    10486 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/REA/AppBOM-inationVDR.xml
--rw-r--r--   0 runner    (1001) docker     (123)   191631 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/REA/PyYamlSBOM.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (123)   230822 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/REA/PyYamlVDR.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:32:59.387745 ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/
--rw-r--r--   0 runner    (1001) docker     (123)    13577 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceAndDependency.spdx (1).json
--rw-r--r--   0 runner    (1001) docker     (123)   250152 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceAndDependency.spdx.rdf.xml
--rw-r--r--   0 runner    (1001) docker     (123)    10205 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceAndDependency.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceAndDependency.spdx.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9821 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceOnly.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)   190258 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceOnly.spdx.rdf.xml
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceOnly.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceOnly.spdx.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   182863 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/SourceAuditor-time-1.9.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)   754185 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/SourceAuditor-time-1.9.spdx.rdf.xml
--rw-r--r--   0 runner    (1001) docker     (123)   140277 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/SourceAuditor-time-1.9.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (123)   162052 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/SourceAuditor-time-1.9.spdx.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   272289 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)   706941 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.rdf.xml
--rw-r--r--   0 runner    (1001) docker     (123)   976785 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.rdf.xml.orig
--rw-r--r--   0 runner    (1001) docker     (123)   184179 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (123)   217286 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:32:59.391745 ntia_conformance_checker-0.4.0/tests/doc_fest/SynopsysBlackDuck/
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/SynopsysBlackDuck/time-1.9-3.el8.x8664.rpm.spdx.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:32:59.391745 ntia_conformance_checker-0.4.0/tests/doc_fest/Tern/
--rw-r--r--   0 runner    (1001) docker     (123)    52051 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/Tern/appbomination_container.spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)   994639 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/Tern/tern-pyyaml-spdx.json
--rw-r--r--   0 runner    (1001) docker     (123)   965989 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/Tern/tern-pyyaml-spdx.spdx.tag
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:32:59.395745 ntia_conformance_checker-0.4.0/tests/doc_fest/ZephyrWest/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/ZephyrWest/app (1).spdx.tag
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/ZephyrWest/app.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (123)   514309 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/ZephyrWest/build (1).spdx.tag
--rw-r--r--   0 runner    (1001) docker     (123)    57063 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/ZephyrWest/build-corrected.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (123)    53845 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/ZephyrWest/build.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (123)    16876 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/ZephyrWest/sdk.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (123)   140247 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/ZephyrWest/zephyr (1).spdx.tag
--rw-r--r--   0 runner    (1001) docker     (123)    40468 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/ZephyrWest/zephyr.spdx.tag
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:32:59.395745 ntia_conformance_checker-0.4.0/tests/doc_fest/metaeffekt/
--rw-r--r--   0 runner    (1001) docker     (123)  3246600 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/metaeffekt/jboss-keycloak-15.0.0-container.spdx.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:32:59.403746 ntia_conformance_checker-0.4.0/tests/doc_fest/nexB/
--rw-r--r--   0 runner    (1001) docker     (123)    36870 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/nexB/App-BOM-ination.json
--rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/nexB/App-BOM-ination.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (123)   363611 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/nexB/LibreSolar-v21.0-Source.json
--rw-r--r--   0 runner    (1001) docker     (123)    44486 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/nexB/LibreSolar-v21.0-Source.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (123)   744585 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/nexB/gnu_time-v1.9.json
--rw-r--r--   0 runner    (1001) docker     (123)    74530 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/nexB/gnu_time-v1.9.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (123)    25719 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/nexB/serve-1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/doc_fest/nexB/serve-1.0.0.spdx.tag
--rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-07-27 17:32:47.000000 ntia_conformance_checker-0.4.0/tests/test_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:54:07.645019 ntia_conformance_checker-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:54:07.553018 ntia_conformance_checker-0.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:54:07.557018 ntia_conformance_checker-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/.github/workflows/bandit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:54:07.557018 ntia_conformance_checker-0.5.0/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/.idea/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:54:07.557018 ntia_conformance_checker-0.5.0/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/.idea/ntia-conformance-checker.iml
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/FAQ.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-08-08 18:54:07.645019 ntia_conformance_checker-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/bandit.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:54:07.561018 ntia_conformance_checker-0.5.0/ntia_conformance_checker/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/ntia_conformance_checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/ntia_conformance_checker/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12805 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/ntia_conformance_checker/sbom_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:54:07.561018 ntia_conformance_checker-0.5.0/ntia_conformance_checker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-08-08 18:54:07.000000 ntia_conformance_checker-0.5.0/ntia_conformance_checker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-08-08 18:54:07.000000 ntia_conformance_checker-0.5.0/ntia_conformance_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 18:54:07.000000 ntia_conformance_checker-0.5.0/ntia_conformance_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-08 18:54:07.000000 ntia_conformance_checker-0.5.0/ntia_conformance_checker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-08 18:54:07.000000 ntia_conformance_checker-0.5.0/ntia_conformance_checker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-08 18:54:07.000000 ntia_conformance_checker-0.5.0/ntia_conformance_checker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 18:54:07.645019 ntia_conformance_checker-0.5.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      164 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:54:07.561018 ntia_conformance_checker-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:54:07.545018 ntia_conformance_checker-0.5.0/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:54:07.565018 ntia_conformance_checker-0.5.0/tests/data/SPDXSBOMExampleTests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingAuthorName.spdx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingComponentName.spdx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingComponentVersion.spdx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingDependencyRelationships.spdx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingSupplierName.spdx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingUniqueIdentifiers.spdx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/SPDXSBOMExampleTests/alpine.spdx
+-rw-r--r--   0 runner    (1001) docker     (123)    25506 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/SPDXSBOMExampleTests/bom-alpine-3.15.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)    27752 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/SPDXSBOMExampleTests/photon.spdx.tag
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:54:07.569018 ntia_conformance_checker-0.5.0/tests/data/missing_author_name/
+-rw-r--r--   0 runner    (1001) docker     (123)    19246 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/missing_author_name/SPDXJSONExample-v2.3.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35758 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/missing_author_name/SPDXRdfExample-v2.3.spdx.rdf.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    16603 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/missing_author_name/SPDXTagExample-v2.3.spdx
+-rw-r--r--   0 runner    (1001) docker     (123)    21925 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/missing_author_name/SPDXXMLExample-v2.3.spdx.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    18436 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/missing_author_name/SPDXYAMLExample-v2.3.spdx.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:54:07.573018 ntia_conformance_checker-0.5.0/tests/data/missing_component_name/
+-rw-r--r--   0 runner    (1001) docker     (123)    17427 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/missing_component_name/SPDXJsonExample.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17744 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/missing_component_name/SPDXRdfExample.rdf
+-rw-r--r--   0 runner    (1001) docker     (123)    15054 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/missing_component_name/SPDXXmlExample.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    13726 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/missing_component_name/SPDXYamlExample.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:54:07.573018 ntia_conformance_checker-0.5.0/tests/data/missing_component_version/
+-rw-r--r--   0 runner    (1001) docker     (123)    19301 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/missing_component_version/SPDXJSONExample-v2.3.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)    36044 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/missing_component_version/SPDXRdfExample-v2.3.spdx.rdf.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    16670 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/missing_component_version/SPDXTagExample-v2.3.spdx
+-rw-r--r--   0 runner    (1001) docker     (123)    22006 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/missing_component_version/SPDXXMLExample-v2.3.spdx.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    18504 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/missing_component_version/SPDXYAMLExample-v2.3.spdx.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:54:07.577018 ntia_conformance_checker-0.5.0/tests/data/missing_dependency_relationships/
+-rw-r--r--   0 runner    (1001) docker     (123)    18333 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/missing_dependency_relationships/SPDXJSONExample-v2.3.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15463 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/missing_dependency_relationships/SPDXRdfExample-v2.3.spdx.rdf.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    16304 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/missing_dependency_relationships/SPDXTagExample-v2.3.spdx
+-rw-r--r--   0 runner    (1001) docker     (123)    20074 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/missing_dependency_relationships/SPDXXMLExample-v2.3.spdx.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    17453 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/missing_dependency_relationships/SPDXYAMLExample-v2.3.spdx.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:54:07.577018 ntia_conformance_checker-0.5.0/tests/data/missing_supplier_name/
+-rw-r--r--   0 runner    (1001) docker     (123)    20983 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/missing_supplier_name/SPDXJSONExample-v2.3.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)    40234 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/missing_supplier_name/SPDXRdfExample-v2.3.spdx.rdf.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    17892 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/missing_supplier_name/SPDXTagExample-v2.3.spdx
+-rw-r--r--   0 runner    (1001) docker     (123)    24068 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/missing_supplier_name/SPDXXMLExample-v2.3.spdx.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    19863 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/missing_supplier_name/SPDXYAMLExample-v2.3.spdx.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:54:07.581018 ntia_conformance_checker-0.5.0/tests/data/missing_timestamp/
+-rw-r--r--   0 runner    (1001) docker     (123)    19312 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/missing_timestamp/SPDXJSONExample-v2.3.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35921 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/missing_timestamp/SPDXRdfExample-v2.3.spdx.rdf.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    16672 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/missing_timestamp/SPDXTagExample-v2.3.spdx
+-rw-r--r--   0 runner    (1001) docker     (123)    22022 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/missing_timestamp/SPDXXMLExample-v2.3.spdx.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    18503 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/missing_timestamp/SPDXYAMLExample-v2.3.spdx.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:54:07.585018 ntia_conformance_checker-0.5.0/tests/data/missing_unique_identifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)    19298 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/missing_unique_identifiers/SPDXJSONExample-v2.3.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34397 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/missing_unique_identifiers/SPDXRdfExample-v2.3.spdx.rdf.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    16654 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/missing_unique_identifiers/SPDXTagExample-v2.3.spdx
+-rw-r--r--   0 runner    (1001) docker     (123)    21947 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/missing_unique_identifiers/SPDXXMLExample-v2.3.spdx.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    18448 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/missing_unique_identifiers/SPDXYAMLExample-v2.3.spdx.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:54:07.585018 ntia_conformance_checker-0.5.0/tests/data/no_elements_missing/
+-rw-r--r--   0 runner    (1001) docker     (123)    19332 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/no_elements_missing/SPDXJSONExample-v2.3.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35941 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/no_elements_missing/SPDXRdfExample-v2.3.spdx.rdf.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    16693 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/no_elements_missing/SPDXTagExample-v2.3.spdx
+-rw-r--r--   0 runner    (1001) docker     (123)    22042 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/no_elements_missing/SPDXXMLExample-v2.3.spdx.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    18526 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/no_elements_missing/SPDXYAMLExample-v2.3.spdx.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:54:07.585018 ntia_conformance_checker-0.5.0/tests/data/other_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/other_tests/SPDXSBOMExample.spdx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/data/other_tests/SPDXSimpleTag.tag
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:54:07.549018 ntia_conformance_checker-0.5.0/tests/doc_fest/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:54:07.589018 ntia_conformance_checker-0.5.0/tests/doc_fest/FOSSology/
+-rw-r--r--   0 runner    (1001) docker     (123)   265354 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/FOSSology/SPDX2TV_PyYAML-6.0.tar.gz.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (123)   265322 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/FOSSology/SPDX2TV_PyYAML-6.0.tar.gz_v2 (1).spdx.tag
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:54:07.601018 ntia_conformance_checker-0.5.0/tests/doc_fest/Kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/Kubernetes/kubernetes-appbomination.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (123)    25724 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/Kubernetes/kubernetes-frederick-serve.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (123) 10020640 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/Kubernetes/kubernetes-keycloak.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (123)    58486 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/Kubernetes/kubernetes-pyyaml.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (123)   177744 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/Kubernetes/kubernetes-time.spdx.tag
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:54:07.601018 ntia_conformance_checker-0.5.0/tests/doc_fest/MetaSpdxscanner/
+-rw-r--r--   0 runner    (1001) docker     (123)    31194 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/MetaSpdxscanner/app-bom-ination-1.0.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (123)   298947 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/MetaSpdxscanner/python3-pyyaml-6.0.spdx.tag
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:54:07.613019 ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/python3-pyyaml-dbg.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/python3-pyyaml-dev.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/python3-pyyaml-src.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)    42218 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/python3-pyyaml.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)   440190 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/recipe-python3-pyyaml.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)   112550 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/recipe-time.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/runtime-python3-pyyaml-dbg.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/runtime-python3-pyyaml-dev.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/runtime-python3-pyyaml-src.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/runtime-python3-pyyaml.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/runtime-time-dbg.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/runtime-time-dev.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/runtime-time-doc.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/runtime-time-src.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/runtime-time.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/time-dbg.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/time-dev.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/time-doc.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/time-src.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/time.spdx.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:54:07.613019 ntia_conformance_checker-0.5.0/tests/doc_fest/Philips/
+-rw-r--r--   0 runner    (1001) docker     (123)   243446 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/Philips/keyclock_sbom.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:54:07.613019 ntia_conformance_checker-0.5.0/tests/doc_fest/REA/
+-rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/REA/AppBOM-inationSBOM.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (123)    10486 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/REA/AppBOM-inationVDR.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   191631 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/REA/PyYamlSBOM.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (123)   230822 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/REA/PyYamlVDR.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:54:07.625019 ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/
+-rw-r--r--   0 runner    (1001) docker     (123)    13577 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceAndDependency.spdx (1).json
+-rw-r--r--   0 runner    (1001) docker     (123)   250152 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceAndDependency.spdx.rdf.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    10205 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceAndDependency.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceAndDependency.spdx.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9821 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceOnly.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)   190258 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceOnly.spdx.rdf.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceOnly.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceOnly.spdx.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   182863 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/SourceAuditor-time-1.9.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)   754185 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/SourceAuditor-time-1.9.spdx.rdf.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   140277 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/SourceAuditor-time-1.9.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (123)   162052 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/SourceAuditor-time-1.9.spdx.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   272289 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)   706941 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.rdf.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   976785 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.rdf.xml.orig
+-rw-r--r--   0 runner    (1001) docker     (123)   184179 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (123)   217286 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:54:07.629019 ntia_conformance_checker-0.5.0/tests/doc_fest/SynopsysBlackDuck/
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/SynopsysBlackDuck/time-1.9-3.el8.x8664.rpm.spdx.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:54:07.629019 ntia_conformance_checker-0.5.0/tests/doc_fest/Tern/
+-rw-r--r--   0 runner    (1001) docker     (123)    52051 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/Tern/appbomination_container.spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)   994639 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/Tern/tern-pyyaml-spdx.json
+-rw-r--r--   0 runner    (1001) docker     (123)   965989 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/Tern/tern-pyyaml-spdx.spdx.tag
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:54:07.637019 ntia_conformance_checker-0.5.0/tests/doc_fest/ZephyrWest/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/ZephyrWest/app (1).spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/ZephyrWest/app.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (123)   514309 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/ZephyrWest/build (1).spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (123)    57063 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/ZephyrWest/build-corrected.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (123)    53845 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/ZephyrWest/build.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (123)    16876 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/ZephyrWest/sdk.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (123)   140247 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/ZephyrWest/zephyr (1).spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (123)    40468 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/ZephyrWest/zephyr.spdx.tag
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:54:07.637019 ntia_conformance_checker-0.5.0/tests/doc_fest/metaeffekt/
+-rw-r--r--   0 runner    (1001) docker     (123)  3246600 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/metaeffekt/jboss-keycloak-15.0.0-container.spdx.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 18:54:07.645019 ntia_conformance_checker-0.5.0/tests/doc_fest/nexB/
+-rw-r--r--   0 runner    (1001) docker     (123)    36870 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/nexB/App-BOM-ination.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/nexB/App-BOM-ination.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (123)   363611 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/nexB/LibreSolar-v21.0-Source.json
+-rw-r--r--   0 runner    (1001) docker     (123)    44486 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/nexB/LibreSolar-v21.0-Source.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (123)   744585 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/nexB/gnu_time-v1.9.json
+-rw-r--r--   0 runner    (1001) docker     (123)    74530 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/nexB/gnu_time-v1.9.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (123)    25719 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/nexB/serve-1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/doc_fest/nexB/serve-1.0.0.spdx.tag
+-rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-08-08 18:53:53.000000 ntia_conformance_checker-0.5.0/tests/test_checker.py
```

### Comparing `ntia_conformance_checker-0.4.0/.github/workflows/build.yml` & `ntia_conformance_checker-0.5.0/.github/workflows/build.yml`

 * *Files 7% similar despite different names*

```diff
@@ -27,12 +27,7 @@
       env:
           # This token is provided by Actions,
           # you do not need to create your own token
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
       run: |
         pipenv run coverage run -m pytest
         pipenv run coverage xml -o coverage/python.xml
-    - name: Report python coverage
-      uses: orgoro/coverage@v3
-      with:
-        coverageFile: coverage/python.xml
-        token: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `ntia_conformance_checker-0.4.0/.github/workflows/codeql.yml` & `ntia_conformance_checker-0.5.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/.github/workflows/pylint.yml` & `ntia_conformance_checker-0.5.0/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/.github/workflows/python-publish.yml` & `ntia_conformance_checker-0.5.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/.gitignore` & `ntia_conformance_checker-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/CONTRIBUTING.md` & `ntia_conformance_checker-0.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/LICENSE` & `ntia_conformance_checker-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/PKG-INFO` & `ntia_conformance_checker-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntia_conformance_checker
-Version: 0.4.0
+Version: 0.5.0
 Summary: Check SPDX SBOM for NTIA minimum elements
 Author-email: Josh Lin <linynjosh@gmail.com>, John Speed Meyers <johnmeyersster@gmail.com>
 Maintainer-email: John Speed Meyers <johnmeyersster@gmail.com>, Gary O'Neall <gary@sourceauditor.com>, Josh Lin <linynjosh@gmail.com>, SPDX group at the Linux Foundation and others <spdx-implementers+owner@lists.spdx.org>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/spdx/ntia-conformance-checker
 Keywords: spdx,sbom,ntia
 Classifier: Intended Audience :: Developers
```

### Comparing `ntia_conformance_checker-0.4.0/Pipfile.lock` & `ntia_conformance_checker-0.5.0/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/README.md` & `ntia_conformance_checker-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/ntia_conformance_checker/main.py` & `ntia_conformance_checker-0.5.0/ntia_conformance_checker/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 def get_parsed_args():
     """Parse command line arguments"""
     parser = argparse.ArgumentParser(
         prog="ntia-checker",
         description="Check if SPDX SBOM complies with NTIA minimum elements",
     )
-    parser.add_argument("--file", help="Filepath for SPDX SBOM")
+    parser.add_argument("--file", required=True, help="Filepath for SPDX SBOM")
     parser.add_argument(
         "--output",
         choices=["print", "json", "html", "quiet"],
         default="print",
         help="Specify type of output",
     )
     parser.add_argument(
@@ -31,28 +31,35 @@
         "--output_path", help="Specify whether output should be verbose"
     )
     parser.add_argument(
         "--version",
         action="store_true",
         help="Display version of ntia-conformance-checker",
     )
+    parser.add_argument(
+        "--skip-validation",
+        action="store_true",
+        default=False,
+        help="Display version of ntia-conformance-checker",
+    )
+
     args = parser.parse_args()
     return args
 
 
 def main():
     """Entrypoint for CLI application."""
 
     args = get_parsed_args()
 
     if args.version:
         print(version("ntia-conformance-checker"))
         sys.exit(0)
 
-    sbom = SbomChecker(args.file)
+    sbom = SbomChecker(args.file, validate=not args.skip_validation)
     if args.output == "print":
         sbom.print_table_output()
         if args.verbose:
             sbom.print_components_missing_info()
     if args.output == "json":
         result_dict = sbom.output_json()
         if args.output_path:
```

### Comparing `ntia_conformance_checker-0.4.0/ntia_conformance_checker/sbom_checker.py` & `ntia_conformance_checker-0.5.0/ntia_conformance_checker/sbom_checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,22 +12,24 @@
 from spdx_tools.spdx.validation.document_validator import validate_full_spdx_document
 
 
 # pylint: disable=too-many-instance-attributes
 class SbomChecker:
     """SBOM minimum elements check."""
 
-    def __init__(self, file):
+    def __init__(self, file, validate=True):
         self.file = file
         self.parsing_error = []
         self.doc = self.parse_file()
         if not self.doc:
             self.ntia_mininum_elements_compliant = False
         else:
-            self.validation_messages = validate_full_spdx_document(self.doc)
+            self.validation_messages = None
+            if validate:
+                self.validation_messages = validate_full_spdx_document(self.doc)
             self.sbom_name = self.doc.creation_info.name
             self.doc_version = self.check_doc_version()
             self.doc_author = True
             self.doc_timestamp = True
             self.dependency_relationships = self.check_dependency_relationships()
             self.components_without_names = self.get_components_without_names()
             self.components_without_versions = self.get_components_without_versions()
@@ -241,15 +243,15 @@
                 "nonconformantComponents"
             ] = self.components_without_suppliers
             result["componentSuppliers"][
                 "allProvided"
             ] = not self.components_without_suppliers
             result["totalNumberComponents"] = self.get_total_number_components()
             if self.validation_messages:
-                result["validationMessages"] = self.validation_messages
+                result["validationMessages"] = list(map(str, self.validation_messages))
         else:
             result["parsingError"] = self.parsing_error
 
         result["isNtiaConformant"] = self.ntia_mininum_elements_compliant
 
         return result
```

### Comparing `ntia_conformance_checker-0.4.0/ntia_conformance_checker.egg-info/PKG-INFO` & `ntia_conformance_checker-0.5.0/ntia_conformance_checker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntia-conformance-checker
-Version: 0.4.0
+Version: 0.5.0
 Summary: Check SPDX SBOM for NTIA minimum elements
 Author-email: Josh Lin <linynjosh@gmail.com>, John Speed Meyers <johnmeyersster@gmail.com>
 Maintainer-email: John Speed Meyers <johnmeyersster@gmail.com>, Gary O'Neall <gary@sourceauditor.com>, Josh Lin <linynjosh@gmail.com>, SPDX group at the Linux Foundation and others <spdx-implementers+owner@lists.spdx.org>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/spdx/ntia-conformance-checker
 Keywords: spdx,sbom,ntia
 Classifier: Intended Audience :: Developers
```

### Comparing `ntia_conformance_checker-0.4.0/ntia_conformance_checker.egg-info/SOURCES.txt` & `ntia_conformance_checker-0.5.0/ntia_conformance_checker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/pyproject.toml` & `ntia_conformance_checker-0.5.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2", "setuptools_scm[toml]>=3.4.3"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ntia_conformance_checker"
-version = "0.4.0"
+version = "0.5.0"
 authors = [
     {name = "Josh Lin", email = "linynjosh@gmail.com"},
     {name = "John Speed Meyers", email = "johnmeyersster@gmail.com"}
 ]
 maintainers = [
     {name = "John Speed Meyers", email = "johnmeyersster@gmail.com"},
     {name = "Gary O'Neall", email = "gary@sourceauditor.com"},
```

### Comparing `ntia_conformance_checker-0.4.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingAuthorName.spdx.yml` & `ntia_conformance_checker-0.5.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingAuthorName.spdx.yml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingComponentName.spdx.yml` & `ntia_conformance_checker-0.5.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingComponentName.spdx.yml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingComponentVersion.spdx.yml` & `ntia_conformance_checker-0.5.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingComponentVersion.spdx.yml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingDependencyRelationships.spdx.yml` & `ntia_conformance_checker-0.5.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingDependencyRelationships.spdx.yml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingSupplierName.spdx.yml` & `ntia_conformance_checker-0.5.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingSupplierName.spdx.yml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingUniqueIdentifiers.spdx.yml` & `ntia_conformance_checker-0.5.0/tests/data/SPDXSBOMExampleTests/SPDXSBOMExampleMissingUniqueIdentifiers.spdx.yml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/SPDXSBOMExampleTests/alpine.spdx` & `ntia_conformance_checker-0.5.0/tests/data/SPDXSBOMExampleTests/alpine.spdx`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/SPDXSBOMExampleTests/bom-alpine-3.15.spdx.json` & `ntia_conformance_checker-0.5.0/tests/data/SPDXSBOMExampleTests/bom-alpine-3.15.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/SPDXSBOMExampleTests/photon.spdx.tag` & `ntia_conformance_checker-0.5.0/tests/data/SPDXSBOMExampleTests/photon.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/missing_author_name/SPDXJSONExample-v2.3.spdx.json` & `ntia_conformance_checker-0.5.0/tests/data/missing_author_name/SPDXJSONExample-v2.3.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/missing_author_name/SPDXRdfExample-v2.3.spdx.rdf.xml` & `ntia_conformance_checker-0.5.0/tests/data/missing_author_name/SPDXRdfExample-v2.3.spdx.rdf.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/missing_author_name/SPDXTagExample-v2.3.spdx` & `ntia_conformance_checker-0.5.0/tests/data/missing_author_name/SPDXTagExample-v2.3.spdx`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/missing_author_name/SPDXXMLExample-v2.3.spdx.xml` & `ntia_conformance_checker-0.5.0/tests/data/missing_author_name/SPDXXMLExample-v2.3.spdx.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/missing_author_name/SPDXYAMLExample-v2.3.spdx.yaml` & `ntia_conformance_checker-0.5.0/tests/data/missing_author_name/SPDXYAMLExample-v2.3.spdx.yaml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/missing_component_name/SPDXJsonExample.json` & `ntia_conformance_checker-0.5.0/tests/data/missing_component_name/SPDXJsonExample.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/missing_component_name/SPDXRdfExample.rdf` & `ntia_conformance_checker-0.5.0/tests/data/missing_component_name/SPDXRdfExample.rdf`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/missing_component_name/SPDXXmlExample.xml` & `ntia_conformance_checker-0.5.0/tests/data/missing_component_name/SPDXXmlExample.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/missing_component_name/SPDXYamlExample.yaml` & `ntia_conformance_checker-0.5.0/tests/data/missing_component_name/SPDXYamlExample.yaml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/missing_component_version/SPDXJSONExample-v2.3.spdx.json` & `ntia_conformance_checker-0.5.0/tests/data/missing_component_version/SPDXJSONExample-v2.3.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/missing_component_version/SPDXRdfExample-v2.3.spdx.rdf.xml` & `ntia_conformance_checker-0.5.0/tests/data/missing_component_version/SPDXRdfExample-v2.3.spdx.rdf.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/missing_component_version/SPDXTagExample-v2.3.spdx` & `ntia_conformance_checker-0.5.0/tests/data/missing_component_version/SPDXTagExample-v2.3.spdx`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/missing_component_version/SPDXXMLExample-v2.3.spdx.xml` & `ntia_conformance_checker-0.5.0/tests/data/missing_component_version/SPDXXMLExample-v2.3.spdx.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/missing_component_version/SPDXYAMLExample-v2.3.spdx.yaml` & `ntia_conformance_checker-0.5.0/tests/data/missing_component_version/SPDXYAMLExample-v2.3.spdx.yaml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/missing_dependency_relationships/SPDXJSONExample-v2.3.spdx.json` & `ntia_conformance_checker-0.5.0/tests/data/missing_dependency_relationships/SPDXJSONExample-v2.3.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/missing_dependency_relationships/SPDXRdfExample-v2.3.spdx.rdf.xml` & `ntia_conformance_checker-0.5.0/tests/data/missing_dependency_relationships/SPDXRdfExample-v2.3.spdx.rdf.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/missing_dependency_relationships/SPDXTagExample-v2.3.spdx` & `ntia_conformance_checker-0.5.0/tests/data/missing_dependency_relationships/SPDXTagExample-v2.3.spdx`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/missing_dependency_relationships/SPDXXMLExample-v2.3.spdx.xml` & `ntia_conformance_checker-0.5.0/tests/data/missing_dependency_relationships/SPDXXMLExample-v2.3.spdx.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/missing_dependency_relationships/SPDXYAMLExample-v2.3.spdx.yaml` & `ntia_conformance_checker-0.5.0/tests/data/missing_dependency_relationships/SPDXYAMLExample-v2.3.spdx.yaml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/missing_supplier_name/SPDXJSONExample-v2.3.spdx.json` & `ntia_conformance_checker-0.5.0/tests/data/missing_supplier_name/SPDXJSONExample-v2.3.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/missing_supplier_name/SPDXRdfExample-v2.3.spdx.rdf.xml` & `ntia_conformance_checker-0.5.0/tests/data/missing_supplier_name/SPDXRdfExample-v2.3.spdx.rdf.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/missing_supplier_name/SPDXTagExample-v2.3.spdx` & `ntia_conformance_checker-0.5.0/tests/data/missing_supplier_name/SPDXTagExample-v2.3.spdx`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/missing_supplier_name/SPDXXMLExample-v2.3.spdx.xml` & `ntia_conformance_checker-0.5.0/tests/data/missing_supplier_name/SPDXXMLExample-v2.3.spdx.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/missing_supplier_name/SPDXYAMLExample-v2.3.spdx.yaml` & `ntia_conformance_checker-0.5.0/tests/data/missing_supplier_name/SPDXYAMLExample-v2.3.spdx.yaml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/missing_timestamp/SPDXJSONExample-v2.3.spdx.json` & `ntia_conformance_checker-0.5.0/tests/data/missing_timestamp/SPDXJSONExample-v2.3.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/missing_timestamp/SPDXRdfExample-v2.3.spdx.rdf.xml` & `ntia_conformance_checker-0.5.0/tests/data/missing_timestamp/SPDXRdfExample-v2.3.spdx.rdf.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/missing_timestamp/SPDXTagExample-v2.3.spdx` & `ntia_conformance_checker-0.5.0/tests/data/missing_timestamp/SPDXTagExample-v2.3.spdx`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/missing_timestamp/SPDXXMLExample-v2.3.spdx.xml` & `ntia_conformance_checker-0.5.0/tests/data/missing_timestamp/SPDXXMLExample-v2.3.spdx.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/missing_timestamp/SPDXYAMLExample-v2.3.spdx.yaml` & `ntia_conformance_checker-0.5.0/tests/data/missing_timestamp/SPDXYAMLExample-v2.3.spdx.yaml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/missing_unique_identifiers/SPDXJSONExample-v2.3.spdx.json` & `ntia_conformance_checker-0.5.0/tests/data/missing_unique_identifiers/SPDXJSONExample-v2.3.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/missing_unique_identifiers/SPDXRdfExample-v2.3.spdx.rdf.xml` & `ntia_conformance_checker-0.5.0/tests/data/missing_unique_identifiers/SPDXRdfExample-v2.3.spdx.rdf.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/missing_unique_identifiers/SPDXTagExample-v2.3.spdx` & `ntia_conformance_checker-0.5.0/tests/data/missing_unique_identifiers/SPDXTagExample-v2.3.spdx`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/missing_unique_identifiers/SPDXXMLExample-v2.3.spdx.xml` & `ntia_conformance_checker-0.5.0/tests/data/missing_unique_identifiers/SPDXXMLExample-v2.3.spdx.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/missing_unique_identifiers/SPDXYAMLExample-v2.3.spdx.yaml` & `ntia_conformance_checker-0.5.0/tests/data/missing_unique_identifiers/SPDXYAMLExample-v2.3.spdx.yaml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/no_elements_missing/SPDXJSONExample-v2.3.spdx.json` & `ntia_conformance_checker-0.5.0/tests/data/no_elements_missing/SPDXJSONExample-v2.3.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/no_elements_missing/SPDXRdfExample-v2.3.spdx.rdf.xml` & `ntia_conformance_checker-0.5.0/tests/data/no_elements_missing/SPDXRdfExample-v2.3.spdx.rdf.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/no_elements_missing/SPDXTagExample-v2.3.spdx` & `ntia_conformance_checker-0.5.0/tests/data/no_elements_missing/SPDXTagExample-v2.3.spdx`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/no_elements_missing/SPDXXMLExample-v2.3.spdx.xml` & `ntia_conformance_checker-0.5.0/tests/data/no_elements_missing/SPDXXMLExample-v2.3.spdx.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/no_elements_missing/SPDXYAMLExample-v2.3.spdx.yaml` & `ntia_conformance_checker-0.5.0/tests/data/no_elements_missing/SPDXYAMLExample-v2.3.spdx.yaml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/other_tests/SPDXSBOMExample.spdx.yml` & `ntia_conformance_checker-0.5.0/tests/data/other_tests/SPDXSBOMExample.spdx.yml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/data/other_tests/SPDXSimpleTag.tag` & `ntia_conformance_checker-0.5.0/tests/data/other_tests/SPDXSimpleTag.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/FOSSology/SPDX2TV_PyYAML-6.0.tar.gz.spdx.tag` & `ntia_conformance_checker-0.5.0/tests/doc_fest/FOSSology/SPDX2TV_PyYAML-6.0.tar.gz.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/FOSSology/SPDX2TV_PyYAML-6.0.tar.gz_v2 (1).spdx.tag` & `ntia_conformance_checker-0.5.0/tests/doc_fest/FOSSology/SPDX2TV_PyYAML-6.0.tar.gz_v2 (1).spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/Kubernetes/kubernetes-appbomination.spdx.tag` & `ntia_conformance_checker-0.5.0/tests/doc_fest/Kubernetes/kubernetes-appbomination.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/Kubernetes/kubernetes-frederick-serve.spdx.tag` & `ntia_conformance_checker-0.5.0/tests/doc_fest/Kubernetes/kubernetes-frederick-serve.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/Kubernetes/kubernetes-keycloak.spdx.tag` & `ntia_conformance_checker-0.5.0/tests/doc_fest/Kubernetes/kubernetes-keycloak.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/Kubernetes/kubernetes-pyyaml.spdx.tag` & `ntia_conformance_checker-0.5.0/tests/doc_fest/Kubernetes/kubernetes-pyyaml.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/Kubernetes/kubernetes-time.spdx.tag` & `ntia_conformance_checker-0.5.0/tests/doc_fest/Kubernetes/kubernetes-time.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/MetaSpdxscanner/app-bom-ination-1.0.spdx.tag` & `ntia_conformance_checker-0.5.0/tests/doc_fest/MetaSpdxscanner/app-bom-ination-1.0.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/MetaSpdxscanner/python3-pyyaml-6.0.spdx.tag` & `ntia_conformance_checker-0.5.0/tests/doc_fest/MetaSpdxscanner/python3-pyyaml-6.0.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/python3-pyyaml-dbg.spdx.json` & `ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/python3-pyyaml-dbg.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/python3-pyyaml-dev.spdx.json` & `ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/python3-pyyaml-dev.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/python3-pyyaml-src.spdx.json` & `ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/python3-pyyaml-src.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/python3-pyyaml.spdx.json` & `ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/python3-pyyaml.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/recipe-python3-pyyaml.spdx.json` & `ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/recipe-python3-pyyaml.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/recipe-time.spdx.json` & `ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/recipe-time.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/runtime-python3-pyyaml-dbg.spdx.json` & `ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/runtime-python3-pyyaml-dbg.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/runtime-python3-pyyaml-dev.spdx.json` & `ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/runtime-python3-pyyaml-dev.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/runtime-python3-pyyaml-src.spdx.json` & `ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/runtime-python3-pyyaml-src.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/runtime-python3-pyyaml.spdx.json` & `ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/runtime-python3-pyyaml.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/runtime-time-dbg.spdx.json` & `ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/runtime-time-dbg.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/runtime-time-dev.spdx.json` & `ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/runtime-time-dev.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/runtime-time-doc.spdx.json` & `ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/runtime-time-doc.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/runtime-time-src.spdx.json` & `ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/runtime-time-src.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/runtime-time.spdx.json` & `ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/runtime-time.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/time-dbg.spdx.json` & `ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/time-dbg.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/time-dev.spdx.json` & `ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/time-dev.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/time-doc.spdx.json` & `ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/time-doc.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/time-src.spdx.json` & `ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/time-src.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/OpenEmbedded/time.spdx.json` & `ntia_conformance_checker-0.5.0/tests/doc_fest/OpenEmbedded/time.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/Philips/keyclock_sbom.json` & `ntia_conformance_checker-0.5.0/tests/doc_fest/Philips/keyclock_sbom.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/REA/AppBOM-inationSBOM.spdx.tag` & `ntia_conformance_checker-0.5.0/tests/doc_fest/REA/AppBOM-inationSBOM.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/REA/AppBOM-inationVDR.xml` & `ntia_conformance_checker-0.5.0/tests/doc_fest/REA/AppBOM-inationVDR.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/REA/PyYamlSBOM.spdx.tag` & `ntia_conformance_checker-0.5.0/tests/doc_fest/REA/PyYamlSBOM.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/REA/PyYamlVDR.xml` & `ntia_conformance_checker-0.5.0/tests/doc_fest/REA/PyYamlVDR.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceAndDependency.spdx (1).json` & `ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceAndDependency.spdx (1).json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceAndDependency.spdx.rdf.xml` & `ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceAndDependency.spdx.rdf.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceAndDependency.spdx.tag` & `ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceAndDependency.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceAndDependency.spdx.yaml` & `ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceAndDependency.spdx.yaml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceOnly.spdx.json` & `ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceOnly.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceOnly.spdx.rdf.xml` & `ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceOnly.spdx.rdf.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceOnly.spdx.tag` & `ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceOnly.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceOnly.spdx.yaml` & `ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/AppBomInation-SourceOnly.spdx.yaml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/SourceAuditor-time-1.9.spdx.json` & `ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/SourceAuditor-time-1.9.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/SourceAuditor-time-1.9.spdx.rdf.xml` & `ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/SourceAuditor-time-1.9.spdx.rdf.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/SourceAuditor-time-1.9.spdx.tag` & `ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/SourceAuditor-time-1.9.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/SourceAuditor-time-1.9.spdx.yaml` & `ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/SourceAuditor-time-1.9.spdx.yaml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.json` & `ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.rdf.xml` & `ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.rdf.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.rdf.xml.orig` & `ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.rdf.xml.orig`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.tag` & `ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.yaml` & `ntia_conformance_checker-0.5.0/tests/doc_fest/SourceAuditor/pyyamll-6.spdx.yaml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/SynopsysBlackDuck/time-1.9-3.el8.x8664.rpm.spdx.json` & `ntia_conformance_checker-0.5.0/tests/doc_fest/SynopsysBlackDuck/time-1.9-3.el8.x8664.rpm.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/Tern/appbomination_container.spdx.json` & `ntia_conformance_checker-0.5.0/tests/doc_fest/Tern/appbomination_container.spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/Tern/tern-pyyaml-spdx.json` & `ntia_conformance_checker-0.5.0/tests/doc_fest/Tern/tern-pyyaml-spdx.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/Tern/tern-pyyaml-spdx.spdx.tag` & `ntia_conformance_checker-0.5.0/tests/doc_fest/Tern/tern-pyyaml-spdx.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/ZephyrWest/app (1).spdx.tag` & `ntia_conformance_checker-0.5.0/tests/doc_fest/ZephyrWest/app (1).spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/ZephyrWest/app.spdx.tag` & `ntia_conformance_checker-0.5.0/tests/doc_fest/ZephyrWest/app.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/ZephyrWest/build (1).spdx.tag` & `ntia_conformance_checker-0.5.0/tests/doc_fest/ZephyrWest/build (1).spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/ZephyrWest/build-corrected.spdx.tag` & `ntia_conformance_checker-0.5.0/tests/doc_fest/ZephyrWest/build-corrected.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/ZephyrWest/build.spdx.tag` & `ntia_conformance_checker-0.5.0/tests/doc_fest/ZephyrWest/build.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/ZephyrWest/sdk.spdx.tag` & `ntia_conformance_checker-0.5.0/tests/doc_fest/ZephyrWest/sdk.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/ZephyrWest/zephyr (1).spdx.tag` & `ntia_conformance_checker-0.5.0/tests/doc_fest/ZephyrWest/zephyr (1).spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/ZephyrWest/zephyr.spdx.tag` & `ntia_conformance_checker-0.5.0/tests/doc_fest/ZephyrWest/zephyr.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/metaeffekt/jboss-keycloak-15.0.0-container.spdx.xml` & `ntia_conformance_checker-0.5.0/tests/doc_fest/metaeffekt/jboss-keycloak-15.0.0-container.spdx.xml`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/nexB/App-BOM-ination.json` & `ntia_conformance_checker-0.5.0/tests/doc_fest/nexB/App-BOM-ination.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/nexB/App-BOM-ination.spdx.tag` & `ntia_conformance_checker-0.5.0/tests/doc_fest/nexB/App-BOM-ination.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/nexB/LibreSolar-v21.0-Source.json` & `ntia_conformance_checker-0.5.0/tests/doc_fest/nexB/LibreSolar-v21.0-Source.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/nexB/LibreSolar-v21.0-Source.spdx.tag` & `ntia_conformance_checker-0.5.0/tests/doc_fest/nexB/LibreSolar-v21.0-Source.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/nexB/gnu_time-v1.9.json` & `ntia_conformance_checker-0.5.0/tests/doc_fest/nexB/gnu_time-v1.9.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/nexB/gnu_time-v1.9.spdx.tag` & `ntia_conformance_checker-0.5.0/tests/doc_fest/nexB/gnu_time-v1.9.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/nexB/serve-1.0.0.json` & `ntia_conformance_checker-0.5.0/tests/doc_fest/nexB/serve-1.0.0.json`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/doc_fest/nexB/serve-1.0.0.spdx.tag` & `ntia_conformance_checker-0.5.0/tests/doc_fest/nexB/serve-1.0.0.spdx.tag`

 * *Files identical despite different names*

### Comparing `ntia_conformance_checker-0.4.0/tests/test_checker.py` & `ntia_conformance_checker-0.5.0/tests/test_checker.py`

 * *Files identical despite different names*

