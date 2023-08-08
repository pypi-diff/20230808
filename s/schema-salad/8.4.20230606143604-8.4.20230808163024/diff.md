# Comparing `tmp/schema-salad-8.4.20230606143604.tar.gz` & `tmp/schema-salad-8.4.20230808163024.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schema-salad-8.4.20230606143604.tar", last modified: Tue Jun  6 15:39:12 2023, max compression
+gzip compressed data, was "schema-salad-8.4.20230808163024.tar", last modified: Tue Aug  8 16:40:33 2023, max compression
```

## Comparing `schema-salad-8.4.20230606143604.tar` & `schema-salad-8.4.20230808163024.tar`

### file list

```diff
@@ -1,450 +1,450 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.990679 schema-salad-8.4.20230606143604/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.946678 schema-salad-8.4.20230606143604/.circleci/
--rw-r--r--   0 michael   (1000) michael   (1000)     3370 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/.circleci/config.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      324 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/.coveragerc
--rw-r--r--   0 michael   (1000) michael   (1000)      304 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/.dockerignore
--rw-r--r--   0 michael   (1000) michael   (1000)      282 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/.flake8
--rw-r--r--   0 michael   (1000) michael   (1000)      229 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/.git-blame-ignore-revs
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.946678 schema-salad-8.4.20230606143604/.github/
--rw-r--r--   0 michael   (1000) michael   (1000)      603 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/.github/dependabot.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.946678 schema-salad-8.4.20230606143604/.github/workflows/
--rw-r--r--   0 michael   (1000) michael   (1000)     3859 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/.github/workflows/ci-tests.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      835 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1090 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/.github/workflows/quay-publish.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      169 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/.github/workflows/wheel-prep.sh
--rw-r--r--   0 michael   (1000) michael   (1000)     5664 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/.github/workflows/wheels.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      219 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/.gitignore
--rw-r--r--   0 michael   (1000) michael   (1000)      113 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/.isort.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)      585 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/.mergify.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    21223 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/.pylintrc
--rw-r--r--   0 michael   (1000) michael   (1000)      558 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/.readthedocs.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1643 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/CONTRIBUTING.md
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      680 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/MANIFEST.in
--rw-r--r--   0 michael   (1000) michael   (1000)     8324 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/Makefile
--rw-r--r--   0 michael   (1000) michael   (1000)    15861 2023-06-06 15:39:12.990679 schema-salad-8.4.20230606143604/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)    14703 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/README.rst
--rwxr-xr-x   0 michael   (1000) michael   (1000)      438 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/build-schema_salad-docker.sh
--rw-r--r--   0 michael   (1000) michael   (1000)      209 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/dev-requirements.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.946678 schema-salad-8.4.20230606143604/docs/
--rw-r--r--   0 michael   (1000) michael   (1000)      634 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/docs/Makefile
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.946678 schema-salad-8.4.20230606143604/docs/_static/
--rw-r--r--   0 michael   (1000) michael   (1000)    15086 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/docs/_static/favicon.ico
--rw-r--r--   0 michael   (1000) michael   (1000)      200 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/docs/cli.rst
--rw-r--r--   0 michael   (1000) michael   (1000)     3461 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/docs/conf.py
--rw-r--r--   0 michael   (1000) michael   (1000)      220 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/docs/index.rst
--rw-r--r--   0 michael   (1000) michael   (1000)      795 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/docs/make.bat
--rw-r--r--   0 michael   (1000) michael   (1000)      656 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/docs/typeshed.rst
--rw-r--r--   0 michael   (1000) michael   (1000)      325 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/lgtm.yml
--rwxr-xr-x   0 michael   (1000) michael   (1000)      819 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/manual_wheel_publish.sh
--rw-r--r--   0 michael   (1000) michael   (1000)      122 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-requirements.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.938678 schema-salad-8.4.20230606143604/mypy-stubs/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.946678 schema-salad-8.4.20230606143604/mypy-stubs/cachecontrol/
--rw-r--r--   0 michael   (1000) michael   (1000)      219 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/cachecontrol/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      226 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/cachecontrol/cache.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.946678 schema-salad-8.4.20230606143604/mypy-stubs/cachecontrol/caches/
--rw-r--r--   0 michael   (1000) michael   (1000)      273 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/cachecontrol/caches/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      873 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/cachecontrol/caches/file_cache.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      169 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/cachecontrol/compat.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      470 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/cachecontrol/controller.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      532 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/cachecontrol/wrapper.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.950678 schema-salad-8.4.20230606143604/mypy-stubs/mistune/
--rw-r--r--   0 michael   (1000) michael   (1000)      922 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/mistune/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      168 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/mistune/_types.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     5480 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/mistune/block_parser.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2848 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/mistune/inline_parser.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1535 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/mistune/markdown.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.950678 schema-salad-8.4.20230606143604/mypy-stubs/mistune/plugins/
--rw-r--r--   0 michael   (1000) michael   (1000)      458 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/mistune/plugins/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      566 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/mistune/plugins/table.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     4159 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/mistune/renderers.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1870 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/mistune/scanner.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      191 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/mistune/util.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.950678 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/
--rw-r--r--   0 michael   (1000) michael   (1000)     1292 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      674 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/collection.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      231 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/compare.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/exceptions.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     8337 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/graph.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.954678 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/
--rw-r--r--   0 michael   (1000) michael   (1000)     2010 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_CSVW.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_DC.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1034 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_DCAT.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2361 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_DCTERMS.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1109 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_DOAP.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1847 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_FOAF.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     4691 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_ODRL2.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1259 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_ORG.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2260 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_OWL.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      441 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_PROF.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     4520 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_PROV.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1105 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_QB.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      620 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_RDF.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      519 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_RDFS.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)    41401 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_SDO.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     4965 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_SH.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      943 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_SKOS.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1075 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_SOSA.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      680 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_SSN.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2462 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_TIME.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      927 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_VOID.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1742 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_XSD.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2282 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      131 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/parser.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      724 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/paths.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      893 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/plugin.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.954678 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/plugins/
--rw-r--r--   0 michael   (1000) michael   (1000)      118 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/plugins/__init__.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.954678 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/plugins/parsers/
--rw-r--r--   0 michael   (1000) michael   (1000)      126 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/plugins/parsers/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)       34 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/plugins/parsers/notation3.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1354 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/query.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1370 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/resource.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1337 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/term.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      115 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/rdflib/util.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.954678 schema-salad-8.4.20230606143604/mypy-stubs/ruamel/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy-stubs/ruamel/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      137 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/mypy.ini
--rw-r--r--   0 michael   (1000) michael   (1000)     1097 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/pyproject.toml
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3512 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/release-test.sh
--rw-r--r--   0 michael   (1000) michael   (1000)      376 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/requirements.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.954678 schema-salad-8.4.20230606143604/schema_salad/
--rw-r--r--   0 michael   (1000) michael   (1000)      395 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      110 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/__main__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      186 2023-06-06 15:39:12.000000 schema-salad-8.4.20230606143604/schema_salad/_version.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.958678 schema-salad-8.4.20230606143604/schema_salad/avro/
--rw-r--r--   0 michael   (1000) michael   (1000)    11359 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/avro/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)      166 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/avro/NOTICE
--rw-r--r--   0 michael   (1000) michael   (1000)      802 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/avro/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    23815 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/avro/schema.py
--rw-r--r--   0 michael   (1000) michael   (1000)     7237 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4412 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/codegen_base.py
--rw-r--r--   0 michael   (1000) michael   (1000)    19604 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/cpp_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)    10930 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dlang_codegen.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.958678 schema-salad-8.4.20230606143604/schema_salad/dotnet/
--rw-r--r--   0 michael   (1000) michael   (1000)       82 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/AssemblyInfo.cs
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.958678 schema-salad-8.4.20230606143604/schema_salad/dotnet/DocFx/
--rw-r--r--   0 michael   (1000) michael   (1000)      445 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/DocFx/filterConfig.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       22 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/DocFx/index.md
--rw-r--r--   0 michael   (1000) michael   (1000)       71 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/DocFx/toc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    11356 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)     1442 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Project.csproj.template
--rw-r--r--   0 michael   (1000) michael   (1000)       40 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1788 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Solution.sln
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.958678 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.958678 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/data/
--rw-r--r--   0 michael   (1000) michael   (1000)        4 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/data/test.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      333 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/runsettings.xml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.958678 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/
--rw-r--r--   0 michael   (1000) michael   (1000)      207 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/ExampleTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     2173 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/FetcherTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1151 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/UtilitiesTests.cs
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.958678 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/
--rw-r--r--   0 michael   (1000) michael   (1000)     1027 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/AnyLoaderTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1321 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/ArrayLoaderTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     2429 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/EnumLoaderTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      749 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/ExpressionLoaderTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1742 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/IdMapLoaderTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      766 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/NullLoaderTests.cs
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.962678 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/
--rw-r--r--   0 michael   (1000) michael   (1000)     1435 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderDoubleTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1431 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderFloatTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1393 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderIntTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1246 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderStringTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1087 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/UnionLoaderTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1188 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/Test.csproj.template
--rw-r--r--   0 michael   (1000) michael   (1000)     1459 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/docfx.json
--rw-r--r--   0 michael   (1000) michael   (1000)    11383 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/editorconfig
--rw-r--r--   0 michael   (1000) michael   (1000)     6894 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/gitignore
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.962678 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/
--rw-r--r--   0 michael   (1000) michael   (1000)     2262 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Fetcher.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      167 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/LoaderInstances.cs
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.962678 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/
--rw-r--r--   0 michael   (1000) michael   (1000)      338 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/AnyLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1754 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/ArrayLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      905 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/EnumLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      646 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/ExpressionLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     2168 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/IdMapLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     4481 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/Loader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      362 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/NullLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      745 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/PrimitiveLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      734 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/RecordLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1674 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/RootLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     3984 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/SecondaryDSLLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     3056 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/TypeDSLLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      793 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/UnionLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1656 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/UriLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     5215 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/LoadingOptions.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     4595 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Saveable.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1490 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/ScalarNodeTypeResolver.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      501 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/UriExtensions.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1624 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Utilities.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1913 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/ValidationException.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Vocabs.cs
--rw-r--r--   0 michael   (1000) michael   (1000)    33304 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/dotnet_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4175 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/exceptions.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8025 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/fetcher.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.962678 schema-salad-8.4.20230606143604/schema_salad/java/
--rw-r--r--   0 michael   (1000) michael   (1000)       61 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/MANIFEST.MF
--rw-r--r--   0 michael   (1000) michael   (1000)      993 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)        8 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/gitignore
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.966678 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/
--rw-r--r--   0 michael   (1000) michael   (1000)      335 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/AnyLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1248 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/ArrayLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      296 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/ConstantMaps.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1521 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/DefaultFetcher.java
--rw-r--r--   0 michael   (1000) michael   (1000)      984 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/EnumLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      416 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/ExpressionLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      186 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/Fetcher.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1697 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/IdMapLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     4613 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/Loader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      125 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/LoaderInstances.java
--rw-r--r--   0 michael   (1000) michael   (1000)     3815 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/LoadingOptions.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1944 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/LoadingOptionsBuilder.java
--rw-r--r--   0 michael   (1000) michael   (1000)      332 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/NullLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1113 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/OneOrListOf.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1050 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/OneOrListOfLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      543 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/OptionalLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      384 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/PrimitiveLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1175 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/RecordLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     3734 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/RootLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      180 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/Saveable.java
--rw-r--r--   0 michael   (1000) michael   (1000)      177 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/SaveableImpl.java
--rw-r--r--   0 michael   (1000) michael   (1000)     3035 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/SecondaryFilesDslLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     2555 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/TypeDslLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      866 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/UnionLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1511 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/UriLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     3293 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/Uris.java
--rw-r--r--   0 michael   (1000) michael   (1000)     2254 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/ValidationException.java
--rw-r--r--   0 michael   (1000) michael   (1000)      789 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/Validator.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1025 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/YamlUtils.java
--rw-r--r--   0 michael   (1000) michael   (1000)      131 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/main_utils/package.html
--rw-r--r--   0 michael   (1000) michael   (1000)      237 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/overview.html
--rw-r--r--   0 michael   (1000) michael   (1000)      187 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/package.html
--rw-r--r--   0 michael   (1000) michael   (1000)     5467 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/pom.xml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.966678 schema-salad-8.4.20230606143604/schema_salad/java/test_utils/
--rw-r--r--   0 michael   (1000) michael   (1000)     1347 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/test_utils/DefaultFetcherTest.java
--rw-r--r--   0 michael   (1000) michael   (1000)       74 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/test_utils/ExamplesTest.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1134 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/test_utils/ShortnameTest.java
--rw-r--r--   0 michael   (1000) michael   (1000)      402 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java/test_utils/YamlUtilsTest.java
--rw-r--r--   0 michael   (1000) michael   (1000)    32358 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/java_codegen.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     8476 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/jsonld_context.py
--rw-r--r--   0 michael   (1000) michael   (1000)    14154 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/main.py
--rw-r--r--   0 michael   (1000) michael   (1000)    33109 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/makedoc.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.970678 schema-salad-8.4.20230606143604/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1327 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      283 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2442 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      473 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      437 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3322 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1804 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      932 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      183 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       90 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    12751 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3940 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    13461 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      882 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/sfdsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      367 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/sfdsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/sfdsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      190 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/sfdsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      830 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      846 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema/vocab_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)   130989 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/metaschema.py
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/py.typed
--rw-r--r--   0 michael   (1000) michael   (1000)    23034 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/python_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)    28705 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/python_codegen_support.py
--rw-r--r--   0 michael   (1000) michael   (1000)    46746 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/ref_resolver.py
--rw-r--r--   0 michael   (1000) michael   (1000)    29944 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/schema.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9031 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/sourceline.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.978679 schema-salad-8.4.20230606143604/schema_salad/tests/
--rw-r--r--   0 michael   (1000) michael   (1000)  2615816 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/EDAM.owl
--rw-r--r--   0 michael   (1000) michael   (1000)      827 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      125 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/bad_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       65 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/bad_schema2.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      140 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/basket.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1267 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/basket_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      590 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/class_field_test.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      452 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/conftest.py
--rw-r--r--   0 michael   (1000) michael   (1000)   126068 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/cwl-pre.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.978679 schema-salad-8.4.20230606143604/schema_salad/tests/docimp/
--rw-r--r--   0 michael   (1000) michael   (1000)      155 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/docimp/d1.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        7 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/docimp/d2.md
--rw-r--r--   0 michael   (1000) michael   (1000)       42 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/docimp/d3.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       42 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/docimp/d4.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       18 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/docimp/d5.md
--rw-r--r--   0 michael   (1000) michael   (1000)      320 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/docimp/dpre.json
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.982679 schema-salad-8.4.20230606143604/schema_salad/tests/foreign/
--rwxr-xr-x   0 michael   (1000) michael   (1000)      347 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/foreign/foreign_prop1.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      302 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/foreign/foreign_prop2.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      436 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/foreign/foreign_prop3.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      390 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/foreign/foreign_prop4.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      428 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/foreign/foreign_prop5.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      294 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/foreign/foreign_prop6.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      292 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/foreign/foreign_prop7.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/formattest2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       41 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/frag.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       13 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/hello.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       71 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/hellofield.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      946 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/inherited-attributes.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       17 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/inject-id1.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        9 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/inject-id2.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       32 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/inject-id3.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       25 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/list.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1241 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/matcher.py
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/memory-leak-check.py
--rw-r--r--   0 michael   (1000) michael   (1000)    61394 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/metaschema-pre.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      208 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/missing_step_name.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       18 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/mixin.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      154 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/multidoc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      900 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/pt.yml
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1466 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/revtool_bad_schema.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_avro_names.py
--rw-r--r--   0 michael   (1000) michael   (1000)     7342 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_cg.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1146 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_cli_args.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1144 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_cpp_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2420 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_cwl11.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1071 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_dlang_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3366 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_dotnet_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)    15614 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_errors.py
--rw-r--r--   0 michael   (1000) michael   (1000)    19849 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_examples.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2660 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_fetch.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1603 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_fp.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1868 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_java_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9277 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_makedoc.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1334 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_misc.py
--rw-r--r--   0 michael   (1000) michael   (1000)      818 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_pickling.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6218 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_print_oneline.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4547 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_python_codegen.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.982679 schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.982679 schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/
--rw-r--r--   0 michael   (1000) michael   (1000)      227 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/PreprocessedFilesType.yaml
--rw-r--r--   0 michael   (1000) michael   (1000)      912 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_util.js
--rwxr-xr-x   0 michael   (1000) michael   (1000)    11901 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_vcf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      148 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/vcf_merge_util.js
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.982679 schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/bio-cwl-tools/
--rwxr-xr-x   0 michael   (1000) michael   (1000)     4732 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     4701 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats_invalid_schema_ref.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     5757 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/bio-cwl-tools/picard_CreateSequenceDictionary.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.982679 schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/h3agatk/
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1905 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/h3agatk/GATK-Sub-Workflow-h3abionet-snp.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)    10910 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/h3agatk/GATK-complete-WES-Workflow-h3abionet.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1122 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/tabs_rna_seq_workflow.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.982679 schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/topmed/
--rwxr-xr-x   0 michael   (1000) michael   (1000)     5976 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/topmed/topmed_variant_calling_pipeline.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     2231 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9625 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_ref_resolver.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.986679 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/
--rw-r--r--   0 michael   (1000) michael   (1000)    30591 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      209 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    25402 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    20107 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      453 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/avro_naming.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      529 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/avro_naming_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      529 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/avro_subtype.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      524 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/avro_subtype_bad.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)      514 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/cwltest-schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/invocation.md
--rw-r--r--   0 michael   (1000) michael   (1000)     3933 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      514 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/misc_schema_v1.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      575 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/misc_schema_v2.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/no_field_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       70 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/one_line_primary_doc.yml
--rwxr-xr-x   0 michael   (1000) michael   (1000)       42 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test1.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      157 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test10.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      147 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test11.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      299 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test12.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      302 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test13.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      208 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test14.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      247 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test15.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      274 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test16.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      238 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test17.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      241 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test18.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      269 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test19.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)       43 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test2.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)       98 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test3.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)       93 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test4.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)       99 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test5.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)       83 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test6.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      154 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test7.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      152 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test8.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      151 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/test9.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1233 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schema.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1536 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_schemas_directive.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3545 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_subtypes.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3412 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/test_typescript_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1613 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/tests/util.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.986679 schema-salad-8.4.20230606143604/schema_salad/typescript/
--rw-r--r--   0 michael   (1000) michael   (1000)     1617 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/.gitignore
--rw-r--r--   0 michael   (1000) michael   (1000)    11357 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)      138 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/index.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1082 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/package.json
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.986679 schema-salad-8.4.20230606143604/schema_salad/typescript/test/
--rw-r--r--   0 michael   (1000) michael   (1000)      879 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/test/AnyLoader.spec.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      147 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/test/ExampleTest.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     3118 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/test/Fetcher.spec.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1390 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/test/IdMap.spec.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     3265 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/test/Typeguards.spec.ts
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.986679 schema-salad-8.4.20230606143604/schema_salad/typescript/test/data/
--rw-r--r--   0 michael   (1000) michael   (1000)       70 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/test/data/hellofield.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        5 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/test/data/test.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     1418 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/test/utilities.spec.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      541 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/tsconfig.json
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.990679 schema-salad-8.4.20230606143604/schema_salad/typescript/util/
--rw-r--r--   0 michael   (1000) michael   (1000)       60 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/Dict.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     2336 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/Fetcher.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      860 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/Internal.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      282 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/LoaderInstances.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1554 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/LoadingOptions.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     3536 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/Saveable.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      593 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/Typeguards.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1406 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/ValidationException.ts
--rw-r--r--   0 michael   (1000) michael   (1000)       74 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/Vocabs.ts
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.990679 schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/AnyLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1005 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/ArrayLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      481 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/EnumLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      350 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/ExpressionLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1180 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/IdMapLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     3228 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/Loader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      497 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/PrimitiveLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      721 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/RecordLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     2508 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/RootLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     2421 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/SecondaryDSLLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1776 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/TypeDSLLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      789 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/UnionLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1043 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/UriLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)    29355 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/typescript_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3672 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/utils.py
--rw-r--r--   0 michael   (1000) michael   (1000)    15648 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad/validate.py
--rw-r--r--   0 michael   (1000) michael   (1000)      836 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/schema_salad.Dockerfile
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-06 15:39:12.958678 schema-salad-8.4.20230606143604/schema_salad.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)    15861 2023-06-06 15:39:12.000000 schema-salad-8.4.20230606143604/schema_salad.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)    15666 2023-06-06 15:39:12.000000 schema-salad-8.4.20230606143604/schema_salad.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-06-06 15:39:12.000000 schema-salad-8.4.20230606143604/schema_salad.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      106 2023-06-06 15:39:12.000000 schema-salad-8.4.20230606143604/schema_salad.egg-info/entry_points.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      465 2023-06-06 15:39:12.000000 schema-salad-8.4.20230606143604/schema_salad.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       13 2023-06-06 15:39:12.000000 schema-salad-8.4.20230606143604/schema_salad.egg-info/top_level.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-06-06 15:30:50.000000 schema-salad-8.4.20230606143604/schema_salad.egg-info/zip-safe
--rw-r--r--   0 michael   (1000) michael   (1000)      189 2023-06-06 15:39:12.990679 schema-salad-8.4.20230606143604/setup.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)     5828 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/setup.py
--rw-r--r--   0 michael   (1000) michael   (1000)       45 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/test-requirements.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     2735 2023-06-06 15:30:34.000000 schema-salad-8.4.20230606143604/tox.ini
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.441424 schema-salad-8.4.20230808163024/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.393423 schema-salad-8.4.20230808163024/.circleci/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3370 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/.circleci/config.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      324 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/.coveragerc
+-rw-r--r--   0 michael   (1000) michael   (1000)      310 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/.dockerignore
+-rw-r--r--   0 michael   (1000) michael   (1000)      282 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/.flake8
+-rw-r--r--   0 michael   (1000) michael   (1000)      229 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/.git-blame-ignore-revs
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.393423 schema-salad-8.4.20230808163024/.github/
+-rw-r--r--   0 michael   (1000) michael   (1000)      603 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/.github/dependabot.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.393423 schema-salad-8.4.20230808163024/.github/workflows/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3977 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/.github/workflows/ci-tests.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      835 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1090 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/.github/workflows/quay-publish.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      169 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/.github/workflows/wheel-prep.sh
+-rw-r--r--   0 michael   (1000) michael   (1000)     5664 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/.github/workflows/wheels.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      219 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/.gitignore
+-rw-r--r--   0 michael   (1000) michael   (1000)      113 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/.isort.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)      585 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/.mergify.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    21223 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/.pylintrc
+-rw-r--r--   0 michael   (1000) michael   (1000)      558 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/.readthedocs.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1643 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/CONTRIBUTING.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      680 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/MANIFEST.in
+-rw-r--r--   0 michael   (1000) michael   (1000)     8283 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/Makefile
+-rw-r--r--   0 michael   (1000) michael   (1000)    15862 2023-08-08 16:40:33.441424 schema-salad-8.4.20230808163024/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)    14703 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/README.rst
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      449 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/build-schema_salad-docker.sh
+-rw-r--r--   0 michael   (1000) michael   (1000)      209 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/dev-requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.393423 schema-salad-8.4.20230808163024/docs/
+-rw-r--r--   0 michael   (1000) michael   (1000)      634 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/docs/Makefile
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.393423 schema-salad-8.4.20230808163024/docs/_static/
+-rw-r--r--   0 michael   (1000) michael   (1000)    15086 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/docs/_static/favicon.ico
+-rw-r--r--   0 michael   (1000) michael   (1000)      200 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/docs/cli.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)     3461 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/docs/conf.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      220 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/docs/index.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      795 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/docs/make.bat
+-rw-r--r--   0 michael   (1000) michael   (1000)      656 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/docs/typeshed.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      325 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/lgtm.yml
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      819 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/manual_wheel_publish.sh
+-rw-r--r--   0 michael   (1000) michael   (1000)      122 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.385423 schema-salad-8.4.20230808163024/mypy-stubs/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.397423 schema-salad-8.4.20230808163024/mypy-stubs/cachecontrol/
+-rw-r--r--   0 michael   (1000) michael   (1000)      219 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/cachecontrol/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      226 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/cachecontrol/cache.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.397423 schema-salad-8.4.20230808163024/mypy-stubs/cachecontrol/caches/
+-rw-r--r--   0 michael   (1000) michael   (1000)      273 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/cachecontrol/caches/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      873 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/cachecontrol/caches/file_cache.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      169 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/cachecontrol/compat.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      470 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/cachecontrol/controller.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      532 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/cachecontrol/wrapper.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.397423 schema-salad-8.4.20230808163024/mypy-stubs/mistune/
+-rw-r--r--   0 michael   (1000) michael   (1000)      922 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/mistune/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      168 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/mistune/_types.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     5480 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/mistune/block_parser.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2848 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/mistune/inline_parser.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1535 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/mistune/markdown.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.397423 schema-salad-8.4.20230808163024/mypy-stubs/mistune/plugins/
+-rw-r--r--   0 michael   (1000) michael   (1000)      458 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/mistune/plugins/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      566 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/mistune/plugins/table.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4159 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/mistune/renderers.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1870 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/mistune/scanner.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      191 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/mistune/util.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.397423 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1292 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      674 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/collection.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      231 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/compare.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/exceptions.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     8337 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/graph.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.401423 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2010 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_CSVW.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_DC.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1034 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_DCAT.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2361 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_DCTERMS.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1109 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_DOAP.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1847 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_FOAF.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4691 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_ODRL2.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1259 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_ORG.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2260 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_OWL.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      441 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_PROF.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4520 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_PROV.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1105 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_QB.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      620 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_RDF.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      519 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_RDFS.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)    41401 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_SDO.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4965 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_SH.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      943 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_SKOS.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1075 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_SOSA.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      680 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_SSN.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2462 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_TIME.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      927 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_VOID.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1742 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_XSD.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2282 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      131 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/parser.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      724 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/paths.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      893 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/plugin.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.401423 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/plugins/
+-rw-r--r--   0 michael   (1000) michael   (1000)      118 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/plugins/__init__.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.401423 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/plugins/parsers/
+-rw-r--r--   0 michael   (1000) michael   (1000)      126 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/plugins/parsers/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)       34 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/plugins/parsers/notation3.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1354 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/query.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1370 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/resource.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1337 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/term.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      115 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/rdflib/util.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.401423 schema-salad-8.4.20230808163024/mypy-stubs/ruamel/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy-stubs/ruamel/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      137 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/mypy.ini
+-rw-r--r--   0 michael   (1000) michael   (1000)     1157 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/pyproject.toml
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3512 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/release-test.sh
+-rw-r--r--   0 michael   (1000) michael   (1000)      471 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.405423 schema-salad-8.4.20230808163024/schema_salad/
+-rw-r--r--   0 michael   (1000) michael   (1000)      395 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      110 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/__main__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      186 2023-08-08 16:40:33.000000 schema-salad-8.4.20230808163024/schema_salad/_version.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.405423 schema-salad-8.4.20230808163024/schema_salad/avro/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11359 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/avro/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)      166 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/avro/NOTICE
+-rw-r--r--   0 michael   (1000) michael   (1000)      802 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/avro/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    23815 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/avro/schema.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     7384 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4412 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/codegen_base.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    19604 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/cpp_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    11181 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dlang_codegen.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.409423 schema-salad-8.4.20230808163024/schema_salad/dotnet/
+-rw-r--r--   0 michael   (1000) michael   (1000)       82 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/AssemblyInfo.cs
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.409423 schema-salad-8.4.20230808163024/schema_salad/dotnet/DocFx/
+-rw-r--r--   0 michael   (1000) michael   (1000)      445 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/DocFx/filterConfig.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       22 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/DocFx/index.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       71 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/DocFx/toc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    11356 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)     1442 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/Project.csproj.template
+-rw-r--r--   0 michael   (1000) michael   (1000)       40 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1788 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/Solution.sln
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.409423 schema-salad-8.4.20230808163024/schema_salad/dotnet/Test/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.409423 schema-salad-8.4.20230808163024/schema_salad/dotnet/Test/data/
+-rw-r--r--   0 michael   (1000) michael   (1000)        4 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/Test/data/test.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      333 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/Test/runsettings.xml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.409423 schema-salad-8.4.20230808163024/schema_salad/dotnet/Test/src/
+-rw-r--r--   0 michael   (1000) michael   (1000)      207 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/Test/src/ExampleTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     2173 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/Test/src/FetcherTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1151 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/Test/src/UtilitiesTests.cs
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.409423 schema-salad-8.4.20230808163024/schema_salad/dotnet/Test/src/loaders/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1027 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/Test/src/loaders/AnyLoaderTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1321 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/Test/src/loaders/ArrayLoaderTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     2429 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/Test/src/loaders/EnumLoaderTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      749 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/Test/src/loaders/ExpressionLoaderTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1742 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/Test/src/loaders/IdMapLoaderTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      766 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/Test/src/loaders/NullLoaderTests.cs
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.409423 schema-salad-8.4.20230808163024/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1435 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderDoubleTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1431 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderFloatTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1393 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderIntTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1246 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderStringTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1087 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/Test/src/loaders/UnionLoaderTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1188 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/Test.csproj.template
+-rw-r--r--   0 michael   (1000) michael   (1000)     1459 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/docfx.json
+-rw-r--r--   0 michael   (1000) michael   (1000)    11383 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/editorconfig
+-rw-r--r--   0 michael   (1000) michael   (1000)     6894 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/gitignore
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.409423 schema-salad-8.4.20230808163024/schema_salad/dotnet/util/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2262 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/util/Fetcher.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      167 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/util/LoaderInstances.cs
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.413423 schema-salad-8.4.20230808163024/schema_salad/dotnet/util/Loaders/
+-rw-r--r--   0 michael   (1000) michael   (1000)      338 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/util/Loaders/AnyLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1754 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/util/Loaders/ArrayLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      905 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/util/Loaders/EnumLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      646 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/util/Loaders/ExpressionLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     2168 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/util/Loaders/IdMapLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     4481 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/util/Loaders/Loader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      362 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/util/Loaders/NullLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      745 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/util/Loaders/PrimitiveLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      734 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/util/Loaders/RecordLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1674 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/util/Loaders/RootLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     3984 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/util/Loaders/SecondaryDSLLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     3056 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/util/Loaders/TypeDSLLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      793 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/util/Loaders/UnionLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1656 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/util/Loaders/UriLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     5215 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/util/LoadingOptions.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     4595 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/util/Saveable.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1490 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/util/ScalarNodeTypeResolver.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      501 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/util/UriExtensions.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1624 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/util/Utilities.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1913 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/util/ValidationException.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet/util/Vocabs.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)    33179 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/dotnet_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4175 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/exceptions.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8025 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/fetcher.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.413423 schema-salad-8.4.20230808163024/schema_salad/java/
+-rw-r--r--   0 michael   (1000) michael   (1000)       61 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/MANIFEST.MF
+-rw-r--r--   0 michael   (1000) michael   (1000)      993 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)        8 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/gitignore
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.417423 schema-salad-8.4.20230808163024/schema_salad/java/main_utils/
+-rw-r--r--   0 michael   (1000) michael   (1000)      335 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/main_utils/AnyLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1248 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/main_utils/ArrayLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      296 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/main_utils/ConstantMaps.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1521 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/main_utils/DefaultFetcher.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      984 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/main_utils/EnumLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      416 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/main_utils/ExpressionLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      186 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/main_utils/Fetcher.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1697 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/main_utils/IdMapLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     4613 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/main_utils/Loader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      125 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/main_utils/LoaderInstances.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     3815 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/main_utils/LoadingOptions.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1944 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/main_utils/LoadingOptionsBuilder.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      332 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/main_utils/NullLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1113 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/main_utils/OneOrListOf.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1050 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/main_utils/OneOrListOfLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      543 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/main_utils/OptionalLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      384 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/main_utils/PrimitiveLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1175 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/main_utils/RecordLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     3734 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/main_utils/RootLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      180 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/main_utils/Saveable.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      177 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/main_utils/SaveableImpl.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     3035 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/main_utils/SecondaryFilesDslLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     2555 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/main_utils/TypeDslLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      866 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/main_utils/UnionLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1511 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/main_utils/UriLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     3293 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/main_utils/Uris.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     2254 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/main_utils/ValidationException.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      789 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/main_utils/Validator.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1025 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/main_utils/YamlUtils.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      131 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/main_utils/package.html
+-rw-r--r--   0 michael   (1000) michael   (1000)      237 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/overview.html
+-rw-r--r--   0 michael   (1000) michael   (1000)      187 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/package.html
+-rw-r--r--   0 michael   (1000) michael   (1000)     5467 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/pom.xml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.417423 schema-salad-8.4.20230808163024/schema_salad/java/test_utils/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1347 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/test_utils/DefaultFetcherTest.java
+-rw-r--r--   0 michael   (1000) michael   (1000)       74 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/test_utils/ExamplesTest.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1134 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/test_utils/ShortnameTest.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      402 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java/test_utils/YamlUtilsTest.java
+-rw-r--r--   0 michael   (1000) michael   (1000)    32321 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/java_codegen.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     8476 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/jsonld_context.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    14321 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/main.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    33109 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/makedoc.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.421423 schema-salad-8.4.20230808163024/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1327 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      283 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2442 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      473 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      437 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3322 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1804 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      932 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      183 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       90 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    12751 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     4074 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    13461 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      882 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/metaschema/sfdsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      367 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/metaschema/sfdsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      289 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/metaschema/sfdsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      190 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/metaschema/sfdsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1273 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      846 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/metaschema/vocab_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)   131239 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/metaschema.py
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/py.typed
+-rw-r--r--   0 michael   (1000) michael   (1000)    23137 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/python_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    28911 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/python_codegen_support.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    47501 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/ref_resolver.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    29935 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/schema.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9031 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/sourceline.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.429423 schema-salad-8.4.20230808163024/schema_salad/tests/
+-rw-r--r--   0 michael   (1000) michael   (1000)  2615816 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/EDAM.owl
+-rw-r--r--   0 michael   (1000) michael   (1000)      827 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      125 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/bad_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       65 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/bad_schema2.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      140 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/basket.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1267 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/basket_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      590 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/class_field_test.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      452 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/conftest.py
+-rw-r--r--   0 michael   (1000) michael   (1000)   126068 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/cwl-pre.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.429423 schema-salad-8.4.20230808163024/schema_salad/tests/docimp/
+-rw-r--r--   0 michael   (1000) michael   (1000)      155 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/docimp/d1.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        7 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/docimp/d2.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       42 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/docimp/d3.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       42 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/docimp/d4.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       18 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/docimp/d5.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      320 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/docimp/dpre.json
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.429423 schema-salad-8.4.20230808163024/schema_salad/tests/foreign/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      347 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/foreign/foreign_prop1.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      302 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/foreign/foreign_prop2.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      436 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/foreign/foreign_prop3.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      390 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/foreign/foreign_prop4.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      428 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/foreign/foreign_prop5.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      294 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/foreign/foreign_prop6.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      292 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/foreign/foreign_prop7.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/formattest2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       41 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/frag.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       13 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/hello.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       71 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/hellofield.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      946 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/inherited-attributes.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       17 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/inject-id1.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        9 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/inject-id2.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       32 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/inject-id3.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       25 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/list.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1241 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/matcher.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/memory-leak-check.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    61956 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/metaschema-pre.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      208 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/missing_step_name.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       18 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/mixin.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      154 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/multidoc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      900 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/pt.yml
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1466 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/revtool_bad_schema.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_avro_names.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     7342 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_cg.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1146 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_cli_args.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1144 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_cpp_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2420 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_cwl11.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1071 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_dlang_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3366 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_dotnet_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    15614 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_errors.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    20512 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_examples.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2660 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_fetch.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1603 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_fp.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1868 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_java_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9277 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_makedoc.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1334 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_misc.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      818 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_pickling.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6218 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_print_oneline.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4547 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_python_codegen.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.429423 schema-salad-8.4.20230808163024/schema_salad/tests/test_real_cwl/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.433423 schema-salad-8.4.20230808163024/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/
+-rw-r--r--   0 michael   (1000) michael   (1000)      227 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/PreprocessedFilesType.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)      912 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_util.js
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    11901 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_vcf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      148 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/vcf_merge_util.js
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.433423 schema-salad-8.4.20230808163024/schema_salad/tests/test_real_cwl/bio-cwl-tools/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4732 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4701 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats_invalid_schema_ref.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     5757 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_real_cwl/bio-cwl-tools/picard_CreateSequenceDictionary.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.433423 schema-salad-8.4.20230808163024/schema_salad/tests/test_real_cwl/h3agatk/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1905 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_real_cwl/h3agatk/GATK-Sub-Workflow-h3abionet-snp.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    10910 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_real_cwl/h3agatk/GATK-complete-WES-Workflow-h3abionet.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1122 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_real_cwl/tabs_rna_seq_workflow.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.433423 schema-salad-8.4.20230808163024/schema_salad/tests/test_real_cwl/topmed/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     5976 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_real_cwl/topmed/topmed_variant_calling_pipeline.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     2231 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_real_cwl.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9625 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_ref_resolver.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.437424 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/
+-rw-r--r--   0 michael   (1000) michael   (1000)    30591 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      209 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    25402 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    20107 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      453 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/avro_naming.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      529 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/avro_naming_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      529 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/avro_subtype.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      524 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/avro_subtype_bad.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      514 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/cwltest-schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/invocation.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     3933 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      514 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/misc_schema_v1.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      575 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/misc_schema_v2.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       54 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/no_field_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       70 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/one_line_primary_doc.yml
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       42 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/test1.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      157 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/test10.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      147 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/test11.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      299 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/test12.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      302 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/test13.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      208 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/test14.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      247 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/test15.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      274 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/test16.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      238 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/test17.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      241 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/test18.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      269 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/test19.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       43 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/test2.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       98 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/test3.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       93 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/test4.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       99 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/test5.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       83 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/test6.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      154 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/test7.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      152 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/test8.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      151 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/test9.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1233 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schema.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1536 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_schemas_directive.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3545 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_subtypes.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3412 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/test_typescript_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1613 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/tests/util.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.437424 schema-salad-8.4.20230808163024/schema_salad/typescript/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1617 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/.gitignore
+-rw-r--r--   0 michael   (1000) michael   (1000)    11357 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)      138 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/index.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1082 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/package.json
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.437424 schema-salad-8.4.20230808163024/schema_salad/typescript/test/
+-rw-r--r--   0 michael   (1000) michael   (1000)      879 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/test/AnyLoader.spec.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      147 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/test/ExampleTest.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     3118 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/test/Fetcher.spec.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1390 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/test/IdMap.spec.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     3265 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/test/Typeguards.spec.ts
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.437424 schema-salad-8.4.20230808163024/schema_salad/typescript/test/data/
+-rw-r--r--   0 michael   (1000) michael   (1000)       70 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/test/data/hellofield.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        5 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/test/data/test.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     1418 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/test/utilities.spec.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      541 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/tsconfig.json
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.437424 schema-salad-8.4.20230808163024/schema_salad/typescript/util/
+-rw-r--r--   0 michael   (1000) michael   (1000)       60 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/util/Dict.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     2336 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/util/Fetcher.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      860 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/util/Internal.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      282 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/util/LoaderInstances.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1554 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/util/LoadingOptions.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     3536 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/util/Saveable.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      593 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/util/Typeguards.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1406 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/util/ValidationException.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)       74 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/util/Vocabs.ts
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.441424 schema-salad-8.4.20230808163024/schema_salad/typescript/util/loaders/
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/util/loaders/AnyLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1005 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/util/loaders/ArrayLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      481 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/util/loaders/EnumLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      350 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/util/loaders/ExpressionLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1180 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/util/loaders/IdMapLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     3228 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/util/loaders/Loader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      497 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/util/loaders/PrimitiveLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      721 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/util/loaders/RecordLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     2508 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/util/loaders/RootLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     2421 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/util/loaders/SecondaryDSLLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1776 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/util/loaders/TypeDSLLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      789 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/util/loaders/UnionLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1043 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript/util/loaders/UriLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)    29256 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/typescript_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3672 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/utils.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    15648 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad/validate.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      841 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/schema_salad.Dockerfile
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-08-08 16:40:33.405423 schema-salad-8.4.20230808163024/schema_salad.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)    15862 2023-08-08 16:40:33.000000 schema-salad-8.4.20230808163024/schema_salad.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)    15666 2023-08-08 16:40:33.000000 schema-salad-8.4.20230808163024/schema_salad.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-08-08 16:40:33.000000 schema-salad-8.4.20230808163024/schema_salad.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      106 2023-08-08 16:40:33.000000 schema-salad-8.4.20230808163024/schema_salad.egg-info/entry_points.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      539 2023-08-08 16:40:33.000000 schema-salad-8.4.20230808163024/schema_salad.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       13 2023-08-08 16:40:33.000000 schema-salad-8.4.20230808163024/schema_salad.egg-info/top_level.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-08-08 16:34:38.000000 schema-salad-8.4.20230808163024/schema_salad.egg-info/zip-safe
+-rw-r--r--   0 michael   (1000) michael   (1000)      189 2023-08-08 16:40:33.441424 schema-salad-8.4.20230808163024/setup.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)     5942 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/setup.py
+-rw-r--r--   0 michael   (1000) michael   (1000)       75 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/test-requirements.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     2644 2023-08-08 16:34:28.000000 schema-salad-8.4.20230808163024/tox.ini
```

### Comparing `schema-salad-8.4.20230606143604/.circleci/config.yml` & `schema-salad-8.4.20230808163024/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/.github/dependabot.yml` & `schema-salad-8.4.20230808163024/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/.github/workflows/ci-tests.yml` & `schema-salad-8.4.20230808163024/.github/workflows/ci-tests.yml`

 * *Files 6% similar despite different names*

```diff
@@ -16,38 +16,42 @@
     name: CI tests via Tox
 
     runs-on: ubuntu-20.04  # 22.04 doesn't support Python 3.6
 
     strategy:
       matrix:
         py-ver-major: [3]
-        py-ver-minor: [6, 7, 8, 9, 10, 11]
+        py-ver-minor: [6, 8, 9, 10, 11, 12]
         step: [lint, bandit, unit, mypy, memleak]
         exclude:
           - py-ver-major: 3
             py-ver-minor: 6
             step: mypy
           - py-ver-major: 3
             py-ver-minor: 6
             step: memleak
           - py-ver-major: 3
             py-ver-minor: 6
             step: lint
+          - py-ver-major: 3
+            py-ver-minor: 12
+            step: memleak
 
     env:
       py-semver: ${{ format('{0}.{1}', matrix.py-ver-major, matrix.py-ver-minor) }}
       TOXENV: ${{ format('py{0}{1}-{2}', matrix.py-ver-major, matrix.py-ver-minor, matrix.step) }}
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ env.py-semver }}
+          allow-prereleases: true
           cache: pip
           cache-dependency-path: |
             requirements.txt
             tox.ini
 
       - name: Upgrade setuptools and install tox
         run: |
```

### Comparing `schema-salad-8.4.20230606143604/.github/workflows/codeql-analysis.yml` & `schema-salad-8.4.20230808163024/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/.github/workflows/quay-publish.yml` & `schema-salad-8.4.20230808163024/.github/workflows/quay-publish.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/.github/workflows/wheels.yml` & `schema-salad-8.4.20230808163024/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/.mergify.yml` & `schema-salad-8.4.20230808163024/.mergify.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/.pylintrc` & `schema-salad-8.4.20230808163024/.pylintrc`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/.readthedocs.yml` & `schema-salad-8.4.20230808163024/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/CONTRIBUTING.md` & `schema-salad-8.4.20230808163024/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/LICENSE.txt` & `schema-salad-8.4.20230808163024/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/MANIFEST.in` & `schema-salad-8.4.20230808163024/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/Makefile` & `schema-salad-8.4.20230808163024/Makefile`

 * *Files 3% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 	pylint --msg-template="{path}:{line}: [{msg_id}({symbol}), {obj}] {msg}" \
 		$^ -j0> $@ || true
 
 diff_pylint_report: pylint_report.txt
 	diff-quality --compare-branch=main --violations=pylint pylint_report.txt
 
 .coverage:
-	python setup.py test --addopts "--cov --cov-config=.coveragerc --cov-report= ${PYTEST_EXTRA}"
+	pytest --cov --cov-config=.coveragerc --cov-report= ${PYTEST_EXTRA}
 	$(COVBASE) -m schema_salad.main \
 		--print-jsonld-context schema_salad/metaschema/metaschema.yml \
 		> /dev/null
 	$(COVBASE) -m schema_salad.main \
 		--print-rdfs schema_salad/metaschema/metaschema.yml \
 		> /dev/null
 	$(COVBASE) -m schema_salad.main \
@@ -157,15 +157,15 @@
 
 ## test                   : run the schema-salad test suite
 test: $(PYSOURCES)
 	python -m pytest -rs ${PYTEST_EXTRA}
 
 ## testcov                : run the schema-salad test suite and collect coverage
 testcov: $(PYSOURCES)
-	python setup.py test --addopts "--cov" ${PYTEST_EXTRA}
+	pytest --cov ${PYTEST_EXTRA}
 
 sloccount.sc: $(PYSOURCES) Makefile
 	sloccount --duplicates --wide --details $^ > $@
 
 ## sloccount              : count lines of code
 sloccount: $(PYSOURCES) Makefile
 	sloccount $^
@@ -178,15 +178,16 @@
 mypy: $(filter-out setup.py,$(PYSOURCES))
 	MYPYPATH=$$MYPYPATH:mypy-stubs mypy $^
 
 mypy_3.6: $(filter-out setup.py,$(PYSOURCES))
 	MYPYPATH=$$MYPYPATH:mypy-stubs mypy --python-version 3.6 $^
 
 mypyc: $(PYSOURCES)
-	MYPYPATH=mypy-stubs SCHEMA_SALAD_USE_MYPYC=1 python setup.py test --addopts "${PYTEST_EXTRA}"
+	MYPYPATH=mypy-stubs SCHEMA_SALAD_USE_MYPYC=1 pip install --verbose -e . \
+		 && pytest "${PYTEST_EXTRA}"
 
 mypyi:
 	MYPYPATH=mypy-stubs SCHEMA_SALAD_USE_MYPYC=1 pip install .${EXTRAS}
 
 check-metaschema-diff:
 	docker run \
 		-v "$(realpath ${MODULE}/metaschema/):/tmp/:ro" \
```

### Comparing `schema-salad-8.4.20230606143604/PKG-INFO` & `schema-salad-8.4.20230808163024/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: schema-salad
-Version: 8.4.20230606143604
+Version: 8.4.20230808163024
 Summary: Schema Annotations for Linked Avro Data (SALAD)
 Home-page: https://github.com/common-workflow-language/schema_salad
 Download-URL: https://github.com/common-workflow-language/schema_salad/releases
 Author: Common workflow language working group
 Author-email: common-workflow-language@googlegroups.com
 License: Apache 2.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
-Requires-Python: >=3.6,<3.12
+Requires-Python: >=3.6,<3.13
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: pycodegen
 License-File: LICENSE.txt
 
 |Linux Build Status| |Code coverage| |Documentation Status| |CII Best Practices|
```

### Comparing `schema-salad-8.4.20230606143604/README.rst` & `schema-salad-8.4.20230808163024/README.rst`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/docs/Makefile` & `schema-salad-8.4.20230808163024/docs/Makefile`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/docs/_static/favicon.ico` & `schema-salad-8.4.20230808163024/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/docs/conf.py` & `schema-salad-8.4.20230808163024/docs/conf.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/docs/make.bat` & `schema-salad-8.4.20230808163024/docs/make.bat`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/docs/typeshed.rst` & `schema-salad-8.4.20230808163024/docs/typeshed.rst`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/manual_wheel_publish.sh` & `schema-salad-8.4.20230808163024/manual_wheel_publish.sh`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/cachecontrol/caches/file_cache.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/cachecontrol/caches/file_cache.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/cachecontrol/wrapper.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/cachecontrol/wrapper.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/mistune/__init__.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/mistune/__init__.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/mistune/block_parser.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/mistune/block_parser.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/mistune/inline_parser.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/mistune/inline_parser.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/mistune/markdown.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/mistune/markdown.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/mistune/plugins/table.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/mistune/plugins/table.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/mistune/renderers.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/mistune/renderers.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/mistune/scanner.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/mistune/scanner.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/__init__.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/rdflib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/collection.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/rdflib/collection.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/graph.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/rdflib/graph.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_CSVW.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_CSVW.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_DCAT.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_DCAT.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_DCTERMS.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_DCTERMS.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_DOAP.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_DOAP.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_FOAF.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_FOAF.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_ODRL2.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_ODRL2.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_ORG.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_ORG.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_OWL.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_OWL.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_PROV.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_PROV.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_QB.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_QB.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_RDF.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_RDF.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_RDFS.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_RDFS.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_SDO.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_SDO.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_SH.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_SH.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_SKOS.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_SKOS.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_SOSA.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_SOSA.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_SSN.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_SSN.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_TIME.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_TIME.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_VOID.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_VOID.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/_XSD.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/_XSD.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/namespace/__init__.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/rdflib/namespace/__init__.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/paths.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/rdflib/paths.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/plugin.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/rdflib/plugin.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/query.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/rdflib/query.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/resource.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/rdflib/resource.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/mypy-stubs/rdflib/term.pyi` & `schema-salad-8.4.20230808163024/mypy-stubs/rdflib/term.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/pyproject.toml` & `schema-salad-8.4.20230808163024/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [build-system]
 requires = [
     "setuptools>=45",
     "setuptools_scm[toml]>=6.2",
     'mypy==0.971; python_version == "3.6"',  # last version for Python 3.6
-    'mypy==1.3.0; python_version >= "3.7"',  # update mypy-requirements as well
+    'mypy==1.4.1; python_version >= "3.7"',  # update mypy-requirements as well
     "black>=19.10b0",
     "types-pkg_resources",
     "types-requests",
     "types-dataclasses",
+    "importlib_resources>=1.4",  # equivalent to Python 3.9
     "ruamel.yaml>= 0.12.4, != 0.16.6, < 0.18",
     "types-setuptools"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 write_to = "schema_salad/_version.py"
```

### Comparing `schema-salad-8.4.20230606143604/release-test.sh` & `schema-salad-8.4.20230808163024/release-test.sh`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/avro/LICENSE` & `schema-salad-8.4.20230808163024/schema_salad/avro/LICENSE`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/avro/__init__.py` & `schema-salad-8.4.20230808163024/schema_salad/avro/__init__.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/avro/schema.py` & `schema-salad-8.4.20230808163024/schema_salad/avro/schema.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/codegen.py` & `schema-salad-8.4.20230808163024/schema_salad/codegen.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,14 +53,16 @@
     sp = urlsplit(base)
     pkg = (
         package
         if package
         else ".".join(list(reversed(sp.netloc.split("."))) + sp.path.strip("/").split("/"))
     )
     info = parser_info or pkg
+    salad_version = schema_metadata.get("saladVersion", "v1.1")
+
     if lang in set(["python", "cpp", "dlang"]):
         if target:
             dest: Union[TextIOWrapper, TextIO] = open(target, mode="w", encoding="utf-8")
         else:
             dest = sys.stdout
         if lang == "cpp":
             gen = CppCodeGen(
@@ -76,18 +78,21 @@
             gen = DlangCodeGen(
                 base,
                 dest,
                 examples,
                 pkg,
                 copyright,
                 info,
+                salad_version,
             )
             gen.parse(j)
             return
-        gen = PythonCodeGen(dest, copyright=copyright, parser_info=info)
+        gen = PythonCodeGen(
+            dest, copyright=copyright, parser_info=info, salad_version=salad_version
+        )
 
     elif lang == "java":
         gen = JavaCodeGen(
             base,
             target=target,
             examples=examples,
             package=pkg,
```

### Comparing `schema-salad-8.4.20230606143604/schema_salad/codegen_base.py` & `schema-salad-8.4.20230808163024/schema_salad/codegen_base.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/cpp_codegen.py` & `schema-salad-8.4.20230808163024/schema_salad/cpp_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dlang_codegen.py` & `schema-salad-8.4.20230808163024/schema_salad/dlang_codegen.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,23 +18,25 @@
         self,
         base: str,
         target: IO[str],
         examples: Optional[str],
         package: str,
         copyright_: Optional[str],
         parser_info: Optional[str],
+        salad_version: str,
     ) -> None:
         """Initialize the D codegen."""
         super().__init__()
         self.base_uri = base
         self.examples = examples
         self.target = target
         self.package = package
         self.copyright = copyright_
         self.parser_info = parser_info
+        self.salad_version = salad_version
         self.doc_root_types: List[str] = []
 
     def prologue(self) -> None:
         """Trigger to generate the prolouge code."""
         module_comment = []
 
         if self.parser_info:
@@ -56,33 +58,44 @@
         ]
 
         self.target.write(self.to_doc_comment(module_comment))
         self.target.write(
             f"""module {self.package};
 
 import salad.meta.dumper : genDumper;
-import salad.meta.impl : genCtor, genIdentifier, genOpEq;
+import salad.meta.impl : genCtor_, genIdentifier, genOpEq;
 import salad.meta.parser : import_ = importFromURI;
 import salad.meta.uda : documentRoot, id, idMap, link, LinkResolver, secondaryFilesDSL, typeDSL;
 import salad.primitives : SchemaBase;
-import salad.type : None, Either;
+import salad.type : None, Union;
 
 """
         )
         if self.parser_info:
             self.target.write(
                 f"""/// parser information
 enum parserInfo = "{self.parser_info}";
 """  # noqa: B907
             )
 
+        self.target.write(
+            f"""
+enum saladVersion = "{self.salad_version}";
+
+mixin template genCtor()
+{{
+    mixin genCtor_!saladVersion;
+}}
+"""  # noqa: B907
+        )
+
     def epilogue(self, root_loader: TypeDef) -> None:
         """Trigger to generate the epilouge code."""
         doc_root_type_str = ", ".join(self.doc_root_types)
-        doc_root_type = f"Either!({doc_root_type_str})"
+        doc_root_type = f"Union!({doc_root_type_str})"
         self.target.write(
             f"""
 ///
 alias DocumentRootType = {doc_root_type};
 
 ///
 alias importFromURI = import_!DocumentRootType;
@@ -181,15 +194,15 @@
             elif stype == "null":
                 type_str = "None"
             else:
                 type_str = stype
         elif isinstance(type_, list):
             t_str = [self.parse_record_field_type(t, None)[1] for t in type_]
             union_types = ", ".join(t_str)
-            type_str = f"Either!({union_types})"
+            type_str = f"Union!({union_types})"
         elif shortname(type_["type"]) == "array":
             item_type = self.parse_record_field_type(type_["items"], None)[1]
             type_str = f"{item_type}[]"
         elif shortname(type_["type"]) == "record":
             return annotate_str, shortname(type_.get("name", "record"))
         elif shortname(type_["type"]) == "enum":
             return annotate_str, "'not yet implemented'"
```

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/LICENSE` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/LICENSE`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/Project.csproj.template` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/Project.csproj.template`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/Solution.sln` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/Solution.sln`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/FetcherTests.cs` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/Test/src/FetcherTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/UtilitiesTests.cs` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/Test/src/UtilitiesTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/AnyLoaderTests.cs` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/Test/src/loaders/AnyLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/ArrayLoaderTests.cs` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/Test/src/loaders/ArrayLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/EnumLoaderTests.cs` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/Test/src/loaders/EnumLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/ExpressionLoaderTests.cs` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/Test/src/loaders/ExpressionLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/IdMapLoaderTests.cs` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/Test/src/loaders/IdMapLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/NullLoaderTests.cs` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/Test/src/loaders/NullLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderDoubleTests.cs` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderDoubleTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderFloatTests.cs` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderFloatTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderIntTests.cs` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderIntTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderStringTests.cs` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderStringTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/Test/src/loaders/UnionLoaderTests.cs` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/Test/src/loaders/UnionLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/Test.csproj.template` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/Test.csproj.template`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/docfx.json` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/docfx.json`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/editorconfig` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/editorconfig`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/gitignore` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/gitignore`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Fetcher.cs` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/util/Fetcher.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/ArrayLoader.cs` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/util/Loaders/ArrayLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/EnumLoader.cs` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/util/Loaders/EnumLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/ExpressionLoader.cs` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/util/Loaders/ExpressionLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/IdMapLoader.cs` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/util/Loaders/IdMapLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/Loader.cs` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/util/Loaders/Loader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/PrimitiveLoader.cs` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/util/Loaders/PrimitiveLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/RecordLoader.cs` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/util/Loaders/RecordLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/RootLoader.cs` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/util/Loaders/RootLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/SecondaryDSLLoader.cs` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/util/Loaders/SecondaryDSLLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/TypeDSLLoader.cs` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/util/Loaders/TypeDSLLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/UnionLoader.cs` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/util/Loaders/UnionLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Loaders/UriLoader.cs` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/util/Loaders/UriLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/LoadingOptions.cs` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/util/LoadingOptions.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Saveable.cs` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/util/Saveable.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/ScalarNodeTypeResolver.cs` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/util/ScalarNodeTypeResolver.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/Utilities.cs` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/util/Utilities.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet/util/ValidationException.cs` & `schema-salad-8.4.20230808163024/schema_salad/dotnet/util/ValidationException.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/dotnet_codegen.py` & `schema-salad-8.4.20230808163024/schema_salad/dotnet_codegen.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     MutableSequence,
     Optional,
     Set,
     Union,
 )
 from xml.sax.saxutils import escape  # nosec
 
-import pkg_resources
+from importlib_resources import files
 
 from . import _logger, schema
 from .codegen_base import CodeGenBase, TypeDef
 from .exceptions import SchemaException
 from .java_codegen import _ensure_directory_and_write, _safe_makedirs
 from .schema import shortname
 
@@ -851,23 +851,21 @@
         template_vars: MutableMapping[str, str] = dict(
             project_name=self.package,
             version="0.0.1-SNAPSHOT",
             project_description=pd,
             license_name="Apache License, Version 2.0",
         )
 
-        def template_from_resource(resource: str) -> string.Template:
-            template_str = pkg_resources.resource_string(__name__, f"dotnet/{resource}").decode(
-                "utf-8"
-            )
+        def template_from_resource(resource: Path) -> string.Template:
+            template_str = resource.read_text("utf-8")
             template = string.Template(template_str)
             return template
 
         def expand_resource_template_to(resource: str, path: Path) -> None:
-            template = template_from_resource(resource)
+            template = template_from_resource(files("schema_salad").joinpath(f"dotnet/{resource}"))
             src = template.safe_substitute(template_vars)
             _ensure_directory_and_write(path, src)
 
         expand_resource_template_to("editorconfig", self.target_dir / ".editorconfig")
         expand_resource_template_to("gitignore", self.target_dir / ".gitignore")
         expand_resource_template_to("LICENSE", self.target_dir / "LICENSE")
         expand_resource_template_to("README.md", self.target_dir / "README.md")
@@ -940,21 +938,20 @@
         util_src_dirs = {
             "util": self.main_src_dir / "util",
             "Test": self.test_src_dir,
             "DocFx": self.target_dir / "DocFx",
         }
 
         def copy_utils_recursive(util_src: str, util_target: Path) -> None:
-            for util in pkg_resources.resource_listdir(__name__, f"dotnet/{util_src}"):
-                template_path = os.path.join(util_src, util)
-                if pkg_resources.resource_isdir(__name__, f"dotnet/{template_path}"):
-                    copy_utils_recursive(os.path.join(util_src, util), util_target / util)
+            for util in files("schema_salad").joinpath(f"dotnet/{util_src}").iterdir():
+                if util.is_dir():
+                    copy_utils_recursive(os.path.join(util_src, util.name), util_target / util.name)
                     continue
-                src_path = util_target / util
-                src_template = template_from_resource(template_path)
+                src_path = util_target / util.name
+                src_template = template_from_resource(util)
                 src = src_template.safe_substitute(template_args)
                 _ensure_directory_and_write(src_path, src)
 
         for util_src, util_target in util_src_dirs.items():
             copy_utils_recursive(util_src, util_target)
 
     def secondaryfilesdsl_loader(self, inner: TypeDef) -> TypeDef:
```

### Comparing `schema-salad-8.4.20230606143604/schema_salad/exceptions.py` & `schema-salad-8.4.20230808163024/schema_salad/exceptions.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/fetcher.py` & `schema-salad-8.4.20230808163024/schema_salad/fetcher.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/java/README.md` & `schema-salad-8.4.20230808163024/schema_salad/java/README.md`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/ArrayLoader.java` & `schema-salad-8.4.20230808163024/schema_salad/java/main_utils/ArrayLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/DefaultFetcher.java` & `schema-salad-8.4.20230808163024/schema_salad/java/main_utils/DefaultFetcher.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/EnumLoader.java` & `schema-salad-8.4.20230808163024/schema_salad/java/main_utils/EnumLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/IdMapLoader.java` & `schema-salad-8.4.20230808163024/schema_salad/java/main_utils/IdMapLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/Loader.java` & `schema-salad-8.4.20230808163024/schema_salad/java/main_utils/Loader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/LoadingOptions.java` & `schema-salad-8.4.20230808163024/schema_salad/java/main_utils/LoadingOptions.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/LoadingOptionsBuilder.java` & `schema-salad-8.4.20230808163024/schema_salad/java/main_utils/LoadingOptionsBuilder.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/OneOrListOf.java` & `schema-salad-8.4.20230808163024/schema_salad/java/main_utils/OneOrListOf.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/OneOrListOfLoader.java` & `schema-salad-8.4.20230808163024/schema_salad/java/main_utils/OneOrListOfLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/OptionalLoader.java` & `schema-salad-8.4.20230808163024/schema_salad/java/main_utils/OptionalLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/RecordLoader.java` & `schema-salad-8.4.20230808163024/schema_salad/java/main_utils/RecordLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/RootLoader.java` & `schema-salad-8.4.20230808163024/schema_salad/java/main_utils/RootLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/SecondaryFilesDslLoader.java` & `schema-salad-8.4.20230808163024/schema_salad/java/main_utils/SecondaryFilesDslLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/TypeDslLoader.java` & `schema-salad-8.4.20230808163024/schema_salad/java/main_utils/TypeDslLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/UnionLoader.java` & `schema-salad-8.4.20230808163024/schema_salad/java/main_utils/UnionLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/UriLoader.java` & `schema-salad-8.4.20230808163024/schema_salad/java/main_utils/UriLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/Uris.java` & `schema-salad-8.4.20230808163024/schema_salad/java/main_utils/Uris.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/ValidationException.java` & `schema-salad-8.4.20230808163024/schema_salad/java/main_utils/ValidationException.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/Validator.java` & `schema-salad-8.4.20230808163024/schema_salad/java/main_utils/Validator.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/java/main_utils/YamlUtils.java` & `schema-salad-8.4.20230808163024/schema_salad/java/main_utils/YamlUtils.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/java/pom.xml` & `schema-salad-8.4.20230808163024/schema_salad/java/pom.xml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/java/test_utils/DefaultFetcherTest.java` & `schema-salad-8.4.20230808163024/schema_salad/java/test_utils/DefaultFetcherTest.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/java/test_utils/ShortnameTest.java` & `schema-salad-8.4.20230808163024/schema_salad/java/test_utils/ShortnameTest.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/java_codegen.py` & `schema-salad-8.4.20230808163024/schema_salad/java_codegen.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     MutableMapping,
     MutableSequence,
     Optional,
     Set,
     Union,
 )
 
-import pkg_resources
+from importlib_resources import files
 
 from . import _logger, schema
 from .codegen_base import CodeGenBase, TypeDef
 from .exceptions import SchemaException
 from .schema import shortname
 
 # experiment at providing more typed objects building a optional type that allows
@@ -784,23 +784,21 @@
             version="0.0.1-SNAPSHOT",
             project_name=self.package,
             project_description=pd,
             license_name="Apache License, Version 2.0",
             license_url="https://www.apache.org/licenses/LICENSE-2.0.txt",
         )
 
-        def template_from_resource(resource: str) -> string.Template:
-            template_str = pkg_resources.resource_string(__name__, f"java/{resource}").decode(
-                "utf-8"
-            )
+        def template_from_resource(resource: Path) -> string.Template:
+            template_str = resource.read_text("utf-8")
             template = string.Template(template_str)
             return template
 
         def expand_resource_template_to(resource: str, path: Path) -> None:
-            template = template_from_resource(resource)
+            template = template_from_resource(files("schema_salad").joinpath(f"java/{resource}"))
             src = template.safe_substitute(template_vars)
             _ensure_directory_and_write(path, src)
 
         expand_resource_template_to("pom.xml", self.target_dir / "pom.xml")
         expand_resource_template_to("gitignore", self.target_dir / ".gitignore")
         expand_resource_template_to("package.html", self.main_src_dir / "package.html")
         expand_resource_template_to(
@@ -876,17 +874,17 @@
         )
 
         util_src_dirs = {
             "main_utils": self.main_src_dir,
             "test_utils": self.test_src_dir,
         }
         for util_src, util_target in util_src_dirs.items():
-            for util in pkg_resources.resource_listdir(__name__, f"java/{util_src}"):
-                src_path = util_target / "utils" / util
-                src_template = template_from_resource(os.path.join(util_src, util))
+            for util in files("schema_salad").joinpath(f"java/{util_src}").iterdir():
+                src_path = util_target / "utils" / util.name
+                src_template = template_from_resource(util)
                 src = src_template.safe_substitute(template_args)
                 _ensure_directory_and_write(src_path, src)
 
     def secondaryfilesdsl_loader(self, inner: TypeDef) -> TypeDef:
         instance_type = inner.instance_type or "Object"
         return self.declare_type(
             TypeDef(
```

### Comparing `schema-salad-8.4.20230606143604/schema_salad/jsonld_context.py` & `schema-salad-8.4.20230808163024/schema_salad/jsonld_context.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/main.py` & `schema-salad-8.4.20230808163024/schema_salad/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,29 +3,33 @@
 import argparse
 import logging
 import os
 import sys
 from typing import Any, Dict, List, Mapping, MutableSequence, Optional, Union, cast
 from urllib.parse import urlparse
 
-import pkg_resources  # part of setuptools
 from rdflib import __version__ as rdflib_version
 from rdflib.parser import Parser
 from rdflib.plugin import register
 from ruamel.yaml.comments import CommentedMap, CommentedSeq
 
 from . import codegen, jsonld_context, schema
 from .avro.schema import SchemaParseException
 from .exceptions import ValidationException, to_one_line_messages
 from .makedoc import makedoc
 from .ref_resolver import Loader, file_uri
 from .utils import json_dump, stdout
 
 if int(rdflib_version.split(".", maxsplit=1)[0]) < 6:
     register("json-ld", Parser, "rdflib_jsonld.parser", "JsonLDParser")
+
+if sys.version_info >= (3, 8):
+    import importlib.metadata as importlib_metadata
+else:
+    import importlib_metadata
 _logger = logging.getLogger("salad")
 
 
 def printrdf(
     workflow: str,
     wf: Union[CommentedMap, CommentedSeq],
     ctx: Dict[str, Any],
@@ -217,20 +221,20 @@
         return 1
 
     if args.quiet:
         _logger.setLevel(logging.WARN)
     if args.debug:
         _logger.setLevel(logging.DEBUG)
 
-    pkg = pkg_resources.require("schema_salad")
+    pkg = importlib_metadata.version("schema_salad")
     if pkg:
         if args.version:
-            print(f"{sys.argv[0]} Current version: {pkg[0].version}")
+            print(f"{sys.argv[0]} Current version: {pkg}")
             return 0
-        _logger.info("%s Current version: %s", sys.argv[0], pkg[0].version)
+        _logger.info("%s Current version: %s", sys.argv[0], pkg)
 
     # Get the metaschema to validate the schema
     metaschema_names, metaschema_doc, metaschema_loader = schema.get_metaschema()
 
     # Load schema document and resolve refs
 
     schema_uri = args.schema
@@ -295,15 +299,18 @@
         metactx["@base"] = schema_metadata["$base"]
     if isinstance(schema_doc, CommentedSeq):
         (schema_ctx, rdfs) = jsonld_context.salad_to_jsonld_context(schema_doc, metactx)
     else:
         raise ValidationException(f"Expected a CommentedSeq, got {type(schema_doc)}: {schema_doc}.")
 
     # Create the loader that will be used to load the target document.
-    document_loader = Loader(schema_ctx, skip_schemas=args.skip_schemas)
+    schema_version = schema_metadata.get("saladVersion", None)
+    document_loader = Loader(
+        schema_ctx, skip_schemas=args.skip_schemas, salad_version=schema_version
+    )
 
     if args.codegen:
         codegen.codegen(
             args.codegen,
             cast(List[Dict[str, Any]], schema_doc),
             schema_metadata,
             document_loader,
```

### Comparing `schema-salad-8.4.20230606143604/schema_salad/makedoc.py` & `schema-salad-8.4.20230808163024/schema_salad/makedoc.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/metaschema/field_name.yml` & `schema-salad-8.4.20230808163024/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/metaschema/ident_res.yml` & `schema-salad-8.4.20230808163024/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/metaschema/import_include.md` & `schema-salad-8.4.20230808163024/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/metaschema/link_res.yml` & `schema-salad-8.4.20230808163024/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/metaschema/map_res.yml` & `schema-salad-8.4.20230808163024/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/metaschema/map_res_schema.yml` & `schema-salad-8.4.20230808163024/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/metaschema/metaschema.yml` & `schema-salad-8.4.20230808163024/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/metaschema/metaschema_base.yml` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/metaschema_base.yml`

 * *Files 2% similar despite different names*

```diff
@@ -35,17 +35,16 @@
     - "xsd:int"
     - "xsd:long"
     - "xsd:float"
     - "xsd:double"
     - "xsd:string"
   doc:
     - |
-      Names of salad data types (based on Avro schema declarations).
-
-      Refer to the [Avro schema declaration documentation](https://avro.apache.org/docs/current/spec.html#schemas) for
+      Salad data types are based on Avro schema declarations.  Refer to the
+      [Avro schema declaration documentation](https://avro.apache.org/docs/current/spec.html#schemas) for
       detailed information.
     - "null: no value"
     - "boolean: a binary value"
     - "int: 32-bit signed integer"
     - "long: 64-bit signed integer"
     - "float: single precision (32-bit) IEEE 754 floating-point number"
     - "double: double precision (64-bit) IEEE 754 floating-point number"
```

### Comparing `schema-salad-8.4.20230606143604/schema_salad/metaschema/salad.md` & `schema-salad-8.4.20230808163024/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/metaschema/sfdsl_res.yml` & `schema-salad-8.4.20230808163024/schema_salad/metaschema/sfdsl_res.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/metaschema/typedsl_res.yml` & `schema-salad-8.4.20230808163024/schema_salad/metaschema/typedsl_res.yml`

 * *Files 27% similar despite different names*

```diff
@@ -2,17 +2,22 @@
   ## Domain Specific Language for types
 
   Fields may be tagged `typeDSL: true` in `jsonldPredicate`.  If so, the field is expanded using the
   following micro-DSL for schema salad types:
 
   * If the type ends with a question mark `?`, the question mark is stripped off and the type is expanded to a union with `null`
   * If the type ends with square brackets `[]` it is expanded to an array with items of the preceding type symbol
-  * The type may end with both `[]?` to indicate it is an optional array.
+  * The type may end with both square brackets with one question mark (`[]?`) to indicate it is an optional array.
   * Identifier resolution is applied after type DSL expansion.
 
+  Starting with Schema Salad version 1.3, fields tagged with `typeDSL: true` in `jsonldPredicate` have the following additional behavior:
+
+  * Square brackes `[]` can be repeated to indicate 2, 3, or more dimensional array types.
+  * These multi-dimensional arrays, like 1-dimensional arrays, can be combined with `?` (for example, `[][]?`) to indicate that it is an optional multi-dimensional array.
+
   ### Type DSL example
 
   Given the following schema:
 
   ```
 - $include: typedsl_res_schema.yml
 - |
```

### Comparing `schema-salad-8.4.20230606143604/schema_salad/metaschema/vocab_res.yml` & `schema-salad-8.4.20230808163024/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/metaschema.py` & `schema-salad-8.4.20230808163024/schema_salad/metaschema.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # This file was autogenerated using schema-salad-tool --codegen=python
 # The code itself is released under the Apache 2.0 license and the help text is
 # subject to the license of the original schema.
 import copy
 import logging
 import os
 import pathlib
-import re
 import tempfile
 import uuid as _uuid__  # pylint: disable=unused-import # noqa: F401
 import xml.sax  # nosec
 from abc import ABC, abstractmethod
 from io import StringIO
 from typing import (
     Any,
@@ -570,49 +569,55 @@
                 self.vocab_term,
                 self.scoped_ref,
             )
         return self.inner.load(doc, baseuri, loadingOptions)
 
 
 class _TypeDSLLoader(_Loader):
-    typeDSLregex = re.compile(r"^([^[?]+)(\[\])?(\?)?$")
-
-    def __init__(self, inner, refScope):
-        # type: (_Loader, Union[int, None]) -> None
+    def __init__(self, inner, refScope, salad_version):
+        # type: (_Loader, Union[int, None], str) -> None
         self.inner = inner
         self.refScope = refScope
+        self.salad_version = salad_version
 
     def resolve(
         self,
         doc,  # type: str
         baseuri,  # type: str
         loadingOptions,  # type: LoadingOptions
     ):
-        # type: (...) -> Union[List[Union[Dict[str, str], str]], Dict[str, str], str]
-        m = self.typeDSLregex.match(doc)
-        if m:
-            group1 = m.group(1)
-            assert group1 is not None  # nosec
-            first = expand_url(group1, baseuri, loadingOptions, False, True, self.refScope)
-            second = third = None
-            if bool(m.group(2)):
-                second = {"type": "array", "items": first}
-                # second = CommentedMap((("type", "array"),
-                #                       ("items", first)))
-                # second.lc.add_kv_line_col("type", lc)
-                # second.lc.add_kv_line_col("items", lc)
-                # second.lc.filename = filename
-            if bool(m.group(3)):
-                third = ["null", second or first]
-                # third = CommentedSeq(["null", second or first])
-                # third.lc.add_kv_line_col(0, lc)
-                # third.lc.add_kv_line_col(1, lc)
-                # third.lc.filename = filename
-            return third or second or first
-        return doc
+        # type: (...) -> Union[List[Union[Dict[str, Any], str]], Dict[str, Any], str]
+        doc_ = doc
+        optional = False
+        if doc_.endswith("?"):
+            optional = True
+            doc_ = doc_[0:-1]
+
+        if doc_.endswith("[]"):
+            salad_versions = [int(v) for v in self.salad_version[1:].split(".")]
+            items = ""  # type: Union[List[Union[Dict[str, Any], str]], Dict[str, Any], str]
+            rest = doc_[0:-2]
+            if salad_versions < [1, 3]:
+                if rest.endswith("[]"):
+                    # To show the error message with the original type
+                    return doc
+                else:
+                    items = expand_url(rest, baseuri, loadingOptions, False, True, self.refScope)
+            else:
+                items = self.resolve(rest, baseuri, loadingOptions)
+                if isinstance(items, str):
+                    items = expand_url(items, baseuri, loadingOptions, False, True, self.refScope)
+            expanded = {"type": "array", "items": items}  # type: Union[Dict[str, Any], str]
+        else:
+            expanded = expand_url(doc_, baseuri, loadingOptions, False, True, self.refScope)
+
+        if optional:
+            return ["null", expanded]
+        else:
+            return expanded
 
     def load(self, doc, baseuri, loadingOptions, docRoot=None):
         # type: (Any, str, LoadingOptions, Optional[str]) -> Any
         if isinstance(doc, MutableSequence):
             r = []  # type: List[Any]
             for d in doc:
                 if isinstance(d, str):
@@ -3572,47 +3577,48 @@
         strtype,
         array_of_union_of_PrimitiveTypeLoader_or_RecordSchemaLoader_or_EnumSchemaLoader_or_ArraySchemaLoader_or_strtype,
     )
 )
 typedsl_union_of_PrimitiveTypeLoader_or_RecordSchemaLoader_or_EnumSchemaLoader_or_ArraySchemaLoader_or_strtype_or_array_of_union_of_PrimitiveTypeLoader_or_RecordSchemaLoader_or_EnumSchemaLoader_or_ArraySchemaLoader_or_strtype_2 = _TypeDSLLoader(
     union_of_PrimitiveTypeLoader_or_RecordSchemaLoader_or_EnumSchemaLoader_or_ArraySchemaLoader_or_strtype_or_array_of_union_of_PrimitiveTypeLoader_or_RecordSchemaLoader_or_EnumSchemaLoader_or_ArraySchemaLoader_or_strtype,
     2,
+    "v1.1",
 )
 array_of_RecordFieldLoader = _ArrayLoader(RecordFieldLoader)
 union_of_None_type_or_array_of_RecordFieldLoader = _UnionLoader(
     (
         None_type,
         array_of_RecordFieldLoader,
     )
 )
 idmap_fields_union_of_None_type_or_array_of_RecordFieldLoader = _IdMapLoader(
     union_of_None_type_or_array_of_RecordFieldLoader, "name", "type"
 )
 Record_nameLoader = _EnumLoader(("record",), "Record_name")
-typedsl_Record_nameLoader_2 = _TypeDSLLoader(Record_nameLoader, 2)
+typedsl_Record_nameLoader_2 = _TypeDSLLoader(Record_nameLoader, 2, "v1.1")
 union_of_None_type_or_strtype = _UnionLoader(
     (
         None_type,
         strtype,
     )
 )
 uri_union_of_None_type_or_strtype_True_False_None = _URILoader(
     union_of_None_type_or_strtype, True, False, None
 )
 uri_array_of_strtype_True_False_None = _URILoader(array_of_strtype, True, False, None)
 Enum_nameLoader = _EnumLoader(("enum",), "Enum_name")
-typedsl_Enum_nameLoader_2 = _TypeDSLLoader(Enum_nameLoader, 2)
+typedsl_Enum_nameLoader_2 = _TypeDSLLoader(Enum_nameLoader, 2, "v1.1")
 uri_union_of_PrimitiveTypeLoader_or_RecordSchemaLoader_or_EnumSchemaLoader_or_ArraySchemaLoader_or_strtype_or_array_of_union_of_PrimitiveTypeLoader_or_RecordSchemaLoader_or_EnumSchemaLoader_or_ArraySchemaLoader_or_strtype_False_True_2 = _URILoader(
     union_of_PrimitiveTypeLoader_or_RecordSchemaLoader_or_EnumSchemaLoader_or_ArraySchemaLoader_or_strtype_or_array_of_union_of_PrimitiveTypeLoader_or_RecordSchemaLoader_or_EnumSchemaLoader_or_ArraySchemaLoader_or_strtype,
     False,
     True,
     2,
 )
 Array_nameLoader = _EnumLoader(("array",), "Array_name")
-typedsl_Array_nameLoader_2 = _TypeDSLLoader(Array_nameLoader, 2)
+typedsl_Array_nameLoader_2 = _TypeDSLLoader(Array_nameLoader, 2, "v1.1")
 union_of_None_type_or_booltype = _UnionLoader(
     (
         None_type,
         booltype,
     )
 )
 union_of_None_type_or_inttype = _UnionLoader(
@@ -3661,15 +3667,15 @@
         array_of_SpecializeDefLoader,
     )
 )
 idmap_specialize_union_of_None_type_or_array_of_SpecializeDefLoader = _IdMapLoader(
     union_of_None_type_or_array_of_SpecializeDefLoader, "specializeFrom", "specializeTo"
 )
 Documentation_nameLoader = _EnumLoader(("documentation",), "Documentation_name")
-typedsl_Documentation_nameLoader_2 = _TypeDSLLoader(Documentation_nameLoader, 2)
+typedsl_Documentation_nameLoader_2 = _TypeDSLLoader(Documentation_nameLoader, 2, "v1.1")
 union_of_SaladRecordSchemaLoader_or_SaladEnumSchemaLoader_or_DocumentationLoader = (
     _UnionLoader(
         (
             SaladRecordSchemaLoader,
             SaladEnumSchemaLoader,
             DocumentationLoader,
         )
```

### Comparing `schema-salad-8.4.20230606143604/schema_salad/python_codegen.py` & `schema-salad-8.4.20230808163024/schema_salad/python_codegen.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 )
 
 try:
     import black
 except ModuleNotFoundError:
     black = None  # type: ignore[assignment]
 
-from pkg_resources import resource_stream
+from importlib_resources import files
 
 from . import schema
 from .codegen_base import CodeGenBase, TypeDef
 from .exceptions import SchemaException
 from .schema import shortname
 
 _string_type_def = TypeDef("strtype", "_PrimitiveLoader(str)")
@@ -78,22 +78,24 @@
     """Generation of Python code for a given Schema Salad definition."""
 
     def __init__(
         self,
         out: IO[str],
         copyright: Optional[str],
         parser_info: str,
+        salad_version: str,
     ) -> None:
         super().__init__()
         self.out = out
         self.current_class_is_abstract = False
         self.serializer = StringIO()
         self.idfield = ""
         self.copyright = copyright
         self.parser_info = parser_info
+        self.salad_version = salad_version
 
     @staticmethod
     def safe_name(name: str) -> str:
         """Generate a safe version of the given name."""
         avn = schema.avro_field_name(name)
         if avn.startswith("anon."):
             avn = avn[5:]
@@ -119,18 +121,18 @@
 #
 # The original schema is {copyright}.
 """.format(
                     copyright=self.copyright
                 )
             )
 
-        stream = resource_stream(__name__, "python_codegen_support.py")
-        python_codegen_support = stream.read().decode("UTF-8")
+        python_codegen_support = (
+            files("schema_salad").joinpath("python_codegen_support.py").read_text("UTF-8")
+        )
         self.out.write(python_codegen_support[python_codegen_support.find("\n") + 1 :])
-        stream.close()
         self.out.write("\n\n")
 
         self.out.write(
             f"""def parser_info() -> str:
     return "{self.parser_info}"
 
 
@@ -625,15 +627,16 @@
         )
 
     def typedsl_loader(self, inner: TypeDef, ref_scope: Optional[int]) -> TypeDef:
         """Construct the TypeDef for the given DSL loader."""
         return self.declare_type(
             TypeDef(
                 f"typedsl_{self.safe_name(inner.name)}_{ref_scope}",
-                f"_TypeDSLLoader({self.safe_name(inner.name)}, {ref_scope})",
+                f"_TypeDSLLoader({self.safe_name(inner.name)}, {ref_scope}, "  # noqa: B907
+                f"'{self.salad_version}')",
             )
         )
 
     def secondaryfilesdsl_loader(self, inner: TypeDef) -> TypeDef:
         """Construct the TypeDef for secondary files."""
         return self.declare_type(
             TypeDef(
```

### Comparing `schema-salad-8.4.20230606143604/schema_salad/python_codegen_support.py` & `schema-salad-8.4.20230808163024/schema_salad/python_codegen_support.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Template code used by python_codegen.py."""
 import copy
 import logging
 import os
 import pathlib
-import re
 import tempfile
 import uuid as _uuid__  # pylint: disable=unused-import # noqa: F401
 import xml.sax  # nosec
 from abc import ABC, abstractmethod
 from io import StringIO
 from typing import (
     Any,
@@ -567,49 +566,55 @@
                 self.vocab_term,
                 self.scoped_ref,
             )
         return self.inner.load(doc, baseuri, loadingOptions)
 
 
 class _TypeDSLLoader(_Loader):
-    typeDSLregex = re.compile(r"^([^[?]+)(\[\])?(\?)?$")
-
-    def __init__(self, inner, refScope):
-        # type: (_Loader, Union[int, None]) -> None
+    def __init__(self, inner, refScope, salad_version):
+        # type: (_Loader, Union[int, None], str) -> None
         self.inner = inner
         self.refScope = refScope
+        self.salad_version = salad_version
 
     def resolve(
         self,
         doc,  # type: str
         baseuri,  # type: str
         loadingOptions,  # type: LoadingOptions
     ):
-        # type: (...) -> Union[List[Union[Dict[str, str], str]], Dict[str, str], str]
-        m = self.typeDSLregex.match(doc)
-        if m:
-            group1 = m.group(1)
-            assert group1 is not None  # nosec
-            first = expand_url(group1, baseuri, loadingOptions, False, True, self.refScope)
-            second = third = None
-            if bool(m.group(2)):
-                second = {"type": "array", "items": first}
-                # second = CommentedMap((("type", "array"),
-                #                       ("items", first)))
-                # second.lc.add_kv_line_col("type", lc)
-                # second.lc.add_kv_line_col("items", lc)
-                # second.lc.filename = filename
-            if bool(m.group(3)):
-                third = ["null", second or first]
-                # third = CommentedSeq(["null", second or first])
-                # third.lc.add_kv_line_col(0, lc)
-                # third.lc.add_kv_line_col(1, lc)
-                # third.lc.filename = filename
-            return third or second or first
-        return doc
+        # type: (...) -> Union[List[Union[Dict[str, Any], str]], Dict[str, Any], str]
+        doc_ = doc
+        optional = False
+        if doc_.endswith("?"):
+            optional = True
+            doc_ = doc_[0:-1]
+
+        if doc_.endswith("[]"):
+            salad_versions = [int(v) for v in self.salad_version[1:].split(".")]
+            items = ""  # type: Union[List[Union[Dict[str, Any], str]], Dict[str, Any], str]
+            rest = doc_[0:-2]
+            if salad_versions < [1, 3]:
+                if rest.endswith("[]"):
+                    # To show the error message with the original type
+                    return doc
+                else:
+                    items = expand_url(rest, baseuri, loadingOptions, False, True, self.refScope)
+            else:
+                items = self.resolve(rest, baseuri, loadingOptions)
+                if isinstance(items, str):
+                    items = expand_url(items, baseuri, loadingOptions, False, True, self.refScope)
+            expanded = {"type": "array", "items": items}  # type: Union[Dict[str, Any], str]
+        else:
+            expanded = expand_url(doc_, baseuri, loadingOptions, False, True, self.refScope)
+
+        if optional:
+            return ["null", expanded]
+        else:
+            return expanded
 
     def load(self, doc, baseuri, loadingOptions, docRoot=None):
         # type: (Any, str, LoadingOptions, Optional[str]) -> Any
         if isinstance(doc, MutableSequence):
             r = []  # type: List[Any]
             for d in doc:
                 if isinstance(d, str):
```

### Comparing `schema-salad-8.4.20230606143604/schema_salad/ref_resolver.py` & `schema-salad-8.4.20230808163024/schema_salad/ref_resolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     ResolveType,
     aslist,
     onWindows,
     yaml_no_ts,
 )
 
 _logger = logging.getLogger("salad")
-typeDSLregex = re.compile(r"^([^[?]+)(\[\])?(\?)?$")
 
 
 def file_uri(path: str, split_frag: bool = False) -> str:
     if path.startswith("file://"):
         return path
     if split_frag:
         pathsp = path.split("#", 2)
@@ -137,14 +136,15 @@
         idx=loader.idx,
         cache=loader.cache,
         fetcher_constructor=loader.fetcher_constructor,
         skip_schemas=loader.skip_schemas,
         url_fields=loader.url_fields,
         allow_attachments=loader.allow_attachments,
         session=loader.session,
+        salad_version=loader.salad_version,
     )
 
 
 class Loader:
     def __init__(
         self,
         ctx: ContextType,
@@ -154,14 +154,15 @@
         cache: Optional[CacheType] = None,
         session: Optional[requests.sessions.Session] = None,
         fetcher_constructor: Optional[FetcherCallableType] = None,
         skip_schemas: Optional[bool] = None,
         url_fields: Optional[Set[str]] = None,
         allow_attachments: Optional[AttachmentsType] = None,
         doc_cache: Union[str, bool] = True,
+        salad_version: Optional[str] = None,
     ) -> None:
         self.idx: IdxType = (
             NormDict(lambda url: urllib.parse.urlsplit(url).geturl()) if idx is None else idx
         )
 
         self.ctx: ContextType = {}
         self.graph = schemagraph if schemagraph is not None else Graph()
@@ -203,14 +204,19 @@
         self.idmap: Dict[str, str] = {}
         self.mapPredicate: Dict[str, str] = {}
         self.type_dsl_fields: Set[str] = set()
         self.subscopes: Dict[str, str] = {}
         self.secondaryFile_dsl_fields: Set[str] = set()
         self.allow_attachments = allow_attachments
 
+        if salad_version:
+            self.salad_version = salad_version
+        else:
+            self.salad_version = "v1.1"
+
         self.add_context(ctx)
 
     def expand_url(
         self,
         url: str,
         base_url: str,
         scoped_id: bool = False,
@@ -627,31 +633,49 @@
         t: Union[str, CommentedMap, CommentedSeq],
         lc: LineCol,
         filename: str,
     ) -> Union[str, CommentedMap, CommentedSeq]:
         if not isinstance(t, str):
             return t
 
-        m = typeDSLregex.match(t)
-        if not m:
-            return t
-        first = m.group(1)
-        assert first  # nosec
-        second = third = None
-        if bool(m.group(2)):
-            second = CommentedMap((("type", "array"), ("items", first)))
-            second.lc.add_kv_line_col("type", lc)
-            second.lc.add_kv_line_col("items", lc)
-            second.lc.filename = filename
-        if bool(m.group(3)):
-            third = CommentedSeq(["null", second or first])
-            third.lc.add_kv_line_col(0, lc)
-            third.lc.add_kv_line_col(1, lc)
-            third.lc.filename = filename
-        return third or second or first
+        t_ = t
+        optional = False
+        if t_.endswith("?"):
+            optional = True
+            t_ = t_[0:-1]
+
+        if t_.endswith("[]"):
+            salad_versions = [int(v) for v in self.salad_version[1:].split(".")]
+            rest = t_[0:-2]
+            if salad_versions < [1, 3]:
+                if rest.endswith("[]"):
+                    # To show the error message with the original type
+                    return t
+                else:
+                    cmap = CommentedMap((("type", "array"), ("items", rest)))
+            else:
+                items = self._type_dsl(rest, lc, filename)
+                cmap = CommentedMap((("type", "array"), ("items", items)))
+            cmap.lc.add_kv_line_col("type", lc)
+            cmap.lc.add_kv_line_col("items", lc)
+            cmap.lc.filename = filename
+            expanded: Union[str, CommentedMap, CommentedSeq] = cmap
+        else:
+            expanded = t_
+
+        if optional:
+            cs = CommentedSeq(["null", expanded])
+            cs.lc.add_kv_line_col(0, lc)
+            cs.lc.add_kv_line_col(1, lc)
+            cs.lc.filename = filename
+            ret: Union[str, CommentedMap, CommentedSeq] = cs
+        else:
+            ret = expanded
+
+        return ret
 
     def _secondaryFile_dsl(
         self,
         t: Union[str, CommentedMap, CommentedSeq],
         lc: LineCol,
         filename: str,
     ) -> Union[str, CommentedMap, CommentedSeq]:
```

### Comparing `schema-salad-8.4.20230606143604/schema_salad/schema.py` & `schema-salad-8.4.20230808163024/schema_salad/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     Tuple,
     TypeVar,
     Union,
     cast,
 )
 from urllib.parse import urlparse
 
-from pkg_resources import resource_stream
+from importlib_resources import files
 from ruamel.yaml.comments import CommentedMap, CommentedSeq
 
 from schema_salad.utils import (
     CacheType,
     ResolveType,
     add_dictlist,
     aslist,
@@ -173,23 +173,26 @@
                 "@id": saladp + "type",
                 "@type": "@vocab",
                 "refScope": 2,
                 "typeDSL": True,
             },
             "typeDSL": saladp + "JsonldPredicate/typeDSL",
             "xsd": "http://www.w3.org/2001/XMLSchema#",
-        }
+        },
+        salad_version="v1.3",
     )
 
     for salad in SALAD_FILES:
-        with resource_stream("schema_salad", "metaschema/" + salad) as stream:
-            loader.cache["https://w3id.org/cwl/" + salad] = stream.read().decode("UTF-8")
+        loader.cache["https://w3id.org/cwl/" + salad] = (
+            files("schema_salad").joinpath("metaschema/" + salad).read_text("UTF-8")
+        )
 
-    with resource_stream("schema_salad", "metaschema/metaschema.yml") as stream:
-        loader.cache["https://w3id.org/cwl/salad"] = stream.read().decode("UTF-8")
+    loader.cache["https://w3id.org/cwl/salad"] = (
+        files("schema_salad").joinpath("metaschema/metaschema.yml").read_text("UTF-8")
+    )
 
     yaml = yaml_no_ts()
     j = yaml.load(loader.cache["https://w3id.org/cwl/salad"])
     add_lc_filename(j, "metaschema.yml")
     j2 = loader.resolve_all(j, saladp)[0]
 
     if not isinstance(j2, list):
```

### Comparing `schema-salad-8.4.20230606143604/schema_salad/sourceline.py` & `schema-salad-8.4.20230808163024/schema_salad/sourceline.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/EDAM.owl` & `schema-salad-8.4.20230808163024/schema_salad/tests/EDAM.owl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/Process.yml` & `schema-salad-8.4.20230808163024/schema_salad/tests/Process.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/basket_schema.yml` & `schema-salad-8.4.20230808163024/schema_salad/tests/basket_schema.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/class_field_test.yml` & `schema-salad-8.4.20230808163024/schema_salad/tests/class_field_test.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/cwl-pre.yml` & `schema-salad-8.4.20230808163024/schema_salad/tests/cwl-pre.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/inherited-attributes.yml` & `schema-salad-8.4.20230808163024/schema_salad/tests/inherited-attributes.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/matcher.py` & `schema-salad-8.4.20230808163024/schema_salad/tests/matcher.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/metaschema-pre.yml` & `schema-salad-8.4.20230808163024/schema_salad/tests/metaschema-pre.yml`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993669871794871%*

 * *Differences: {'0': "{'doc': {insert: [(37, '## Domain Specific Language for types\\n\\nFields may be tagged "*

 * *      '`typeDSL: true` in `jsonldPredicate`.  If so, the field is expanded using the\\nfollowing '*

 * *      'micro-DSL for schema salad types:\\n\\n* If the type ends with a question mark `?`, the '*

 * *      'question mark is stripped off and the type is expanded to a union with `null`\\n* If the '*

 * *      'type ends with square brackets `[]` it is expanded to an array with items of the preceding '*

 * *      'type symbol\\n […]*

```diff
@@ -34,15 +34,15 @@
             "## Identifier maps\n\nThe schema may designate certain fields as having a `mapSubject`.  If the\nvalue of the field is a JSON object, it must be transformed into an array of\nJSON objects.  Each key-value pair from the source JSON object is a list\nitem, each list item must be a JSON object, and the value of the key is\nassigned to the field specified by `mapSubject`.\n\nFields which have `mapSubject` specified may also supply a `mapPredicate`.\nIf the value of a map item is not a JSON object, the item is transformed to a\nJSON object with the key assigned to the field specified by `mapSubject` and\nthe value assigned to the field specified by `mapPredicate`.\n\n### Identifier map example\n\nGiven the following schema:\n\n```\n",
             "{\n  \"$graph\": [{\n    \"name\": \"MappedType\",\n    \"type\": \"record\",\n    \"documentRoot\": true,\n    \"fields\": [{\n      \"name\": \"mapped\",\n      \"type\": {\n        \"type\": \"array\",\n        \"items\": \"ExampleRecord\"\n      },\n      \"jsonldPredicate\": {\n        \"mapSubject\": \"key\",\n        \"mapPredicate\": \"value\"\n      }\n    }],\n  },\n  {\n    \"name\": \"ExampleRecord\",\n    \"type\": \"record\",\n    \"fields\": [{\n      \"name\": \"key\",\n      \"type\": \"string\"\n      }, {\n      \"name\": \"value\",\n      \"type\": \"string\"\n      }\n    ]\n  }]\n}\n",
             "```\n\nProcess the following example:\n\n```\n",
             "{\n  \"mapped\": {\n    \"shaggy\": {\n      \"value\": \"scooby\"\n    },\n    \"fred\": \"daphne\"\n  }\n}\n",
             "```\n\nThis becomes:\n\n```\n",
             "{\n    \"mapped\": [\n        {\n            \"value\": \"daphne\",\n            \"key\": \"fred\"\n        },\n        {\n            \"value\": \"scooby\",\n            \"key\": \"shaggy\"\n        }\n    ]\n}\n",
             "```\n",
-            "## Domain Specific Language for types\n\nFields may be tagged `typeDSL: true` in `jsonldPredicate`.  If so, the field is expanded using the\nfollowing micro-DSL for schema salad types:\n\n* If the type ends with a question mark `?`, the question mark is stripped off and the type is expanded to a union with `null`\n* If the type ends with square brackets `[]` it is expanded to an array with items of the preceding type symbol\n* The type may end with both `[]?` to indicate it is an optional array.\n* Identifier resolution is applied after type DSL expansion.\n\n### Type DSL example\n\nGiven the following schema:\n\n```\n",
+            "## Domain Specific Language for types\n\nFields may be tagged `typeDSL: true` in `jsonldPredicate`.  If so, the field is expanded using the\nfollowing micro-DSL for schema salad types:\n\n* If the type ends with a question mark `?`, the question mark is stripped off and the type is expanded to a union with `null`\n* If the type ends with square brackets `[]` it is expanded to an array with items of the preceding type symbol\n* The type may end with both square brackets with one question mark (`[]?`) to indicate it is an optional array.\n* Identifier resolution is applied after type DSL expansion.\n\nStarting with Schema Salad version 1.3, fields tagged with `typeDSL: true` in `jsonldPredicate` have the following additional behavior:\n\n* Square brackes `[]` can be repeated to indicate 2, 3, or more dimensional array types.\n* These multi-dimensional arrays, like 1-dimensional arrays, can be combined with `?` (for example, `[][]?`) to indicate that it is an optional multi-dimensional array.\n\n### Type DSL example\n\nGiven the following schema:\n\n```\n",
             "{\n  \"$graph\": [\n  {\"$import\": \"metaschema_base.yml\"},\n  {\n    \"name\": \"TypeDSLExample\",\n    \"type\": \"record\",\n    \"documentRoot\": true,\n    \"fields\": [{\n      \"name\": \"extype\",\n      \"type\": \"string\",\n      \"jsonldPredicate\": {\n        _type: \"@vocab\",\n        \"typeDSL\": true\n      }\n    }]\n  }]\n}\n",
             "```\n\nProcess the following example:\n\n```\n",
             "[{\n  \"extype\": \"string\"\n}, {\n  \"extype\": \"string?\"\n}, {\n  \"extype\": \"string[]\"\n}, {\n  \"extype\": \"string[]?\"\n}]\n",
             "```\n\nThis becomes:\n\n```\n",
             "[\n    {\n        \"extype\": \"string\"\n    }, \n    {\n        \"extype\": [\n            \"null\", \n            \"string\"\n        ]\n    }, \n    {\n        \"extype\": {\n            \"type\": \"array\", \n            \"items\": \"string\"\n        }\n    }, \n    {\n        \"extype\": [\n            \"null\", \n            {\n                \"type\": \"array\", \n                \"items\": \"string\"\n            }\n        ]\n    }\n]\n",
             "```\n",
             "## Domain Specific Language for secondary files\n\nFields may be tagged `secondaryFilesDSL: true` in `jsonldPredicate`.  If so, the field is expanded using the\nfollowing micro-DSL for secondary files:\n\n* If the value is a string, it is transformed to an object with two fields `pattern` and `required`\n* By default, the value of `required` is `null` (this indicates default behavior, which may be based on the context)\n* If the value ends with a question mark `?` the question mark is\n  stripped off and the value of the field `required` is set to `False`\n* The remaining value is assigned to the field `pattern`\n\n### Type DSL example\n\nGiven the following schema:\n\n```\n",
@@ -131,15 +131,15 @@
             {
                 "doc": "The name of the field\n",
                 "jsonldPredicate": "@id",
                 "name": "https://w3id.org/cwl/salad#RecordField/name",
                 "type": "string"
             },
             {
-                "doc": "The field type\n",
+                "doc": "The field type. If it is an array, it indicates\nthat the field type is a union type of its elements.\nIts elements may be duplicated.\n",
                 "jsonldPredicate": {
                     "_id": "https://w3id.org/cwl/salad#type",
                     "_type": "@vocab",
                     "refScope": 2,
                     "typeDSL": true
                 },
                 "name": "https://w3id.org/cwl/salad#RecordField/type",
```

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/pt.yml` & `schema-salad-8.4.20230808163024/schema_salad/tests/pt.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/revtool_bad_schema.cwl` & `schema-salad-8.4.20230808163024/schema_salad/tests/revtool_bad_schema.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_avro_names.py` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_avro_names.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_cg.py` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_cg.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_cli_args.py` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_cli_args.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_cpp_codegen.py` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_cpp_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_cwl11.py` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_cwl11.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_dlang_codegen.py` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_dlang_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_dotnet_codegen.py` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_dotnet_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_errors.py` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_examples.py` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Any, Dict, cast
 
 import pytest
 from ruamel.yaml.comments import CommentedMap, CommentedSeq
 
 import schema_salad.main
 import schema_salad.schema
+from schema_salad.exceptions import ValidationException
 from schema_salad.jsonld_context import makerdf
 from schema_salad.ref_resolver import Loader, file_uri, uri_file_path
 from schema_salad.sourceline import SourceLine, cmap
 from schema_salad.utils import ContextType, stdout, yaml_no_ts
 
 from .util import get_data
 
@@ -329,15 +330,15 @@
 
 
 def test_yaml_float_test() -> None:
     assert yaml_no_ts().load("float-test: 2e-10")["float-test"] == 2e-10
 
 
 def test_typedsl_ref() -> None:
-    ldr = Loader({})
+    ldr = Loader({}, salad_version="v1.1")
     ldr.add_context(
         {
             "File": "http://example.com/File",
             "null": "http://example.com/null",
             "array": "http://example.com/array",
             "type": {"@type": "@vocab", "typeDSL": True},
         }
@@ -351,14 +352,32 @@
 
     ra, _ = ldr.resolve_all(cmap({"type": "File[]"}), "")
     assert {"type": {"items": "File", "type": "array"}} == ra
 
     ra, _ = ldr.resolve_all(cmap({"type": "File[]?"}), "")
     assert {"type": ["null", {"items": "File", "type": "array"}]} == ra
 
+    with pytest.raises(ValidationException):
+        ldr.resolve_all(cmap({"type": "File[][]"}), "")
+
+
+def test_nested_typedsl_ref() -> None:
+    ldr = Loader({}, salad_version="v1.3")
+    ldr.add_context(
+        {
+            "File": "http://example.com/File",
+            "null": "http://example.com/null",
+            "array": "http://example.com/array",
+            "type": {"@type": "@vocab", "typeDSL": True},
+        }
+    )
+
+    ra, _ = ldr.resolve_all(cmap({"type": "File[][]"}), "")
+    assert {"type": {"items": {"items": "File", "type": "array"}, "type": "array"}} == ra
+
 
 def test_secondaryFile_dsl_ref() -> None:
     ldr = Loader({})
     ldr.add_context({"secondaryFiles": {"secondaryFilesDSL": True}})
 
     ra, _ = ldr.resolve_all(cmap({"secondaryFiles": ".foo"}), "")
     assert {"secondaryFiles": {"pattern": ".foo", "required": None}} == ra
```

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_fetch.py` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_fp.py` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_fp.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_java_codegen.py` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_java_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_makedoc.py` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_makedoc.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,9 +235,9 @@
     # 6. If the changes are agreeable, then update the hash below
     hasher = hashlib.sha256()
     hasher.update(metaschema_doc.encode("utf-8"))
     result = tmp_path / "result.html"
     with open(result, "w") as h:
         h.write(metaschema_doc)
     assert (
-        hasher.hexdigest() == "4e67cb0a28829f9e14ecce93183fcf89fedb2446ae6cd717ccb2966609fe76a2"
+        hasher.hexdigest() == "400bd8b4f3af31ffaeeb04b7780a140b0d26151645016e49a1a375964b67ea7e"
     ), result
```

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_misc.py` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_pickling.py` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_print_oneline.py` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_print_oneline.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_python_codegen.py` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_python_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_util.js` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_util.js`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_vcf.cwl` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_vcf.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats.cwl` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats_invalid_schema_ref.cwl` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats_invalid_schema_ref.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/bio-cwl-tools/picard_CreateSequenceDictionary.cwl` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_real_cwl/bio-cwl-tools/picard_CreateSequenceDictionary.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/h3agatk/GATK-Sub-Workflow-h3abionet-snp.cwl` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_real_cwl/h3agatk/GATK-Sub-Workflow-h3abionet-snp.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/h3agatk/GATK-complete-WES-Workflow-h3abionet.cwl` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_real_cwl/h3agatk/GATK-complete-WES-Workflow-h3abionet.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/tabs_rna_seq_workflow.cwl` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_real_cwl/tabs_rna_seq_workflow.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl/topmed/topmed_variant_calling_pipeline.cwl` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_real_cwl/topmed/topmed_variant_calling_pipeline.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_real_cwl.py` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_real_cwl.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_ref_resolver.py` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_ref_resolver.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/CommandLineTool.yml` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/Process.yml` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/Process.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/Workflow.yml` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/Workflow.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/avro_naming_base.yml` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/avro_naming_base.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/avro_subtype.yml` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/avro_subtype.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/avro_subtype_bad.yml` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/avro_subtype_bad.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/cwltest-schema.yml` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/cwltest-schema.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/metaschema_base.yml` & `schema-salad-8.4.20230808163024/schema_salad/metaschema/metaschema_base.yml`

 * *Files 6% similar despite different names*

```diff
@@ -35,16 +35,17 @@
     - "xsd:int"
     - "xsd:long"
     - "xsd:float"
     - "xsd:double"
     - "xsd:string"
   doc:
     - |
-      Salad data types are based on Avro schema declarations.  Refer to the
-      [Avro schema declaration documentation](https://avro.apache.org/docs/current/spec.html#schemas) for
+      Names of salad data types (based on Avro schema declarations).
+
+      Refer to the [Avro schema declaration documentation](https://avro.apache.org/docs/current/spec.html#schemas) for
       detailed information.
     - "null: no value"
     - "boolean: a binary value"
     - "int: 32-bit signed integer"
     - "long: 64-bit signed integer"
     - "float: single precision (32-bit) IEEE 754 floating-point number"
     - "double: double precision (64-bit) IEEE 754 floating-point number"
@@ -86,15 +87,17 @@
             - string
       jsonldPredicate:
         _id: sld:type
         _type: "@vocab"
         typeDSL: true
         refScope: 2
       doc: |
-        The field type
+        The field type. If it is an array, it indicates
+        that the field type is a union type of its elements.
+        Its elements may be duplicated.
 
 
 - name: RecordSchema
   type: record
   fields:
     type:
       doc: "Must be `record`"
```

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/misc_schema_v1.yml` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/misc_schema_v1.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_schema/misc_schema_v2.yml` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_schema/misc_schema_v2.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_schema.py` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_schemas_directive.py` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_schemas_directive.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_subtypes.py` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_subtypes.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/test_typescript_codegen.py` & `schema-salad-8.4.20230808163024/schema_salad/tests/test_typescript_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/tests/util.py` & `schema-salad-8.4.20230808163024/schema_salad/tests/util.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/typescript/.gitignore` & `schema-salad-8.4.20230808163024/schema_salad/typescript/.gitignore`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/typescript/LICENSE` & `schema-salad-8.4.20230808163024/schema_salad/typescript/LICENSE`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/typescript/package.json` & `schema-salad-8.4.20230808163024/schema_salad/typescript/package.json`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/typescript/test/AnyLoader.spec.ts` & `schema-salad-8.4.20230808163024/schema_salad/typescript/test/AnyLoader.spec.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/typescript/test/Fetcher.spec.ts` & `schema-salad-8.4.20230808163024/schema_salad/typescript/test/Fetcher.spec.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/typescript/test/IdMap.spec.ts` & `schema-salad-8.4.20230808163024/schema_salad/typescript/test/IdMap.spec.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/typescript/test/Typeguards.spec.ts` & `schema-salad-8.4.20230808163024/schema_salad/typescript/test/Typeguards.spec.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/typescript/test/utilities.spec.ts` & `schema-salad-8.4.20230808163024/schema_salad/typescript/test/utilities.spec.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/typescript/tsconfig.json` & `schema-salad-8.4.20230808163024/schema_salad/typescript/tsconfig.json`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/typescript/util/Fetcher.ts` & `schema-salad-8.4.20230808163024/schema_salad/typescript/util/Fetcher.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/typescript/util/Internal.ts` & `schema-salad-8.4.20230808163024/schema_salad/typescript/util/Internal.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/typescript/util/LoadingOptions.ts` & `schema-salad-8.4.20230808163024/schema_salad/typescript/util/LoadingOptions.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/typescript/util/Saveable.ts` & `schema-salad-8.4.20230808163024/schema_salad/typescript/util/Saveable.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/typescript/util/Typeguards.ts` & `schema-salad-8.4.20230808163024/schema_salad/typescript/util/Typeguards.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/typescript/util/ValidationException.ts` & `schema-salad-8.4.20230808163024/schema_salad/typescript/util/ValidationException.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/ArrayLoader.ts` & `schema-salad-8.4.20230808163024/schema_salad/typescript/util/loaders/ArrayLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/IdMapLoader.ts` & `schema-salad-8.4.20230808163024/schema_salad/typescript/util/loaders/IdMapLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/Loader.ts` & `schema-salad-8.4.20230808163024/schema_salad/typescript/util/loaders/Loader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/RecordLoader.ts` & `schema-salad-8.4.20230808163024/schema_salad/typescript/util/loaders/RecordLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/RootLoader.ts` & `schema-salad-8.4.20230808163024/schema_salad/typescript/util/loaders/RootLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/SecondaryDSLLoader.ts` & `schema-salad-8.4.20230808163024/schema_salad/typescript/util/loaders/SecondaryDSLLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/TypeDSLLoader.ts` & `schema-salad-8.4.20230808163024/schema_salad/typescript/util/loaders/TypeDSLLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/UnionLoader.ts` & `schema-salad-8.4.20230808163024/schema_salad/typescript/util/loaders/UnionLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/typescript/util/loaders/UriLoader.ts` & `schema-salad-8.4.20230808163024/schema_salad/typescript/util/loaders/UriLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/typescript_codegen.py` & `schema-salad-8.4.20230808163024/schema_salad/typescript_codegen.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     MutableMapping,
     MutableSequence,
     Optional,
     Set,
     Union,
 )
 
-import pkg_resources
+from importlib_resources import files
 
 from . import _logger, schema
 from .codegen_base import CodeGenBase, TypeDef
 from .exceptions import SchemaException
 from .java_codegen import _ensure_directory_and_write, _safe_makedirs
 from .schema import shortname
 
@@ -727,23 +727,23 @@
             project_name=self.package,
             version="0.0.1-SNAPSHOT",
             project_description=pd,
             license_name="Apache License, Version 2.0",
             generated_class_imports=generated_class_imports,
         )
 
-        def template_from_resource(resource: str) -> string.Template:
-            template_str = pkg_resources.resource_string(__name__, f"typescript/{resource}").decode(
-                "utf-8"
-            )
+        def template_from_resource(resource: Path) -> string.Template:
+            template_str = resource.read_text("utf-8")
             template = string.Template(template_str)
             return template
 
         def expand_resource_template_to(resource: str, path: Path) -> None:
-            template = template_from_resource(resource)
+            template = template_from_resource(
+                files("schema_salad").joinpath(f"typescript/{resource}")
+            )
             src = template.safe_substitute(template_vars)
             _ensure_directory_and_write(path, src)
 
         expand_resource_template_to("package.json", self.target_dir / "package.json")
         expand_resource_template_to(".gitignore", self.target_dir / ".gitignore")
         expand_resource_template_to("LICENSE", self.target_dir / "LICENSE")
         expand_resource_template_to("tsconfig.json", self.target_dir / "tsconfig.json")
@@ -802,21 +802,20 @@
 
         util_src_dirs = {
             "util": self.main_src_dir / "util",
             "test": self.main_src_dir / "test",
         }
 
         def copy_utils_recursive(util_src: str, util_target: Path) -> None:
-            for util in pkg_resources.resource_listdir(__name__, f"typescript/{util_src}"):
-                template_path = os.path.join(util_src, util)
-                if pkg_resources.resource_isdir(__name__, f"typescript/{template_path}"):
-                    copy_utils_recursive(os.path.join(util_src, util), util_target / util)
+            for util in files("schema_salad").joinpath(f"typescript/{util_src}").iterdir():
+                if util.is_dir():
+                    copy_utils_recursive(os.path.join(util_src, util.name), util_target / util.name)
                     continue
-                src_path = util_target / util
-                src_template = template_from_resource(template_path)
+                src_path = util_target / util.name
+                src_template = template_from_resource(util)
                 src = src_template.safe_substitute(template_args)
                 _ensure_directory_and_write(src_path, src)
 
         for util_src, util_target in util_src_dirs.items():
             copy_utils_recursive(util_src, util_target)
 
     def secondaryfilesdsl_loader(self, inner: TypeDef) -> TypeDef:
```

### Comparing `schema-salad-8.4.20230606143604/schema_salad/utils.py` & `schema-salad-8.4.20230808163024/schema_salad/utils.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad/validate.py` & `schema-salad-8.4.20230808163024/schema_salad/validate.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/schema_salad.Dockerfile` & `schema-salad-8.4.20230808163024/schema_salad.Dockerfile`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 WORKDIR /schema_salad
 COPY . .
 
 RUN python3 -m venv env3
 RUN source env3/bin/activate && python3 -m pip install -U pip setuptools wheel build
 RUN export SETUPTOOLS_SCM_PRETEND_VERSION=$(grep __version__ schema_salad/_version.py  | awk -F\' '{ print $2 }') ; source env3/bin/activate && SCHEMA_SALAD_USE_MYPYC=1 MYPYPATH=mypy-stubs python3 -m build --wheel --outdir=/wheels
 RUN source env3/bin/activate && python3 -m pip wheel -r requirements.txt --wheel-dir=/wheels
-RUN source env3/bin/activate && python3 -m pip install --force-reinstall --no-index --no-warn-script-location --root=/pythonroot/ /wheels/*.whl
+RUN source env3/bin/activate && python3 -m pip install --force-reinstall --no-index --no-warn-script-location --prefix=/pythonroot/usr /wheels/*.whl
 
 FROM alpine:latest as module
 LABEL maintainer peter.amstutz@curoverse.com
 
 RUN apk add --no-cache py3-six
 
 COPY --from=builder /pythonroot/ /
```

### Comparing `schema-salad-8.4.20230606143604/schema_salad.egg-info/PKG-INFO` & `schema-salad-8.4.20230808163024/schema_salad.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: schema-salad
-Version: 8.4.20230606143604
+Version: 8.4.20230808163024
 Summary: Schema Annotations for Linked Avro Data (SALAD)
 Home-page: https://github.com/common-workflow-language/schema_salad
 Download-URL: https://github.com/common-workflow-language/schema_salad/releases
 Author: Common workflow language working group
 Author-email: common-workflow-language@googlegroups.com
 License: Apache 2.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
-Requires-Python: >=3.6,<3.12
+Requires-Python: >=3.6,<3.13
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 Provides-Extra: pycodegen
 License-File: LICENSE.txt
 
 |Linux Build Status| |Code coverage| |Documentation Status| |CII Best Practices|
```

### Comparing `schema-salad-8.4.20230606143604/schema_salad.egg-info/SOURCES.txt` & `schema-salad-8.4.20230808163024/schema_salad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schema-salad-8.4.20230606143604/setup.py` & `schema-salad-8.4.20230808163024/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,20 +87,22 @@
     "rdflib < 6.0.0;python_version<='3.6'",
     "rdflib-jsonld>=0.4.0, <= 0.6.1;python_version<='3.6'",
     "mistune>=2.0.3,<2.1",
     "CacheControl[filecache] >= 0.11.7, < 0.14",
     "CacheControl[filecache] < 0.13;python_version<='3.6'",
     "urllib3<2;python_version<='3.6'",
     "mypy_extensions",
+    "importlib_resources>=1.4",  # equivalent to Python 3.9,
+    "importlib_metadata;python_version<'3.8'",
 ]
 
 extras_require = {
     "docs": [
         "sphinx >= 2.2",
-        "sphinx-rtd-theme",
+        "sphinx-rtd-theme >= 1",
         "pytest < 8",
         "sphinx-autoapi",
         "sphinx-autodoc-typehints",
         "typed_ast;python_version<'3.8'",
         "sphinxcontrib-autoprogram",
     ],
     "pycodegen": ["black"],
@@ -114,15 +116,15 @@
     long_description_content_type="text/x-rst",
     author="Common workflow language working group",
     author_email="common-workflow-language@googlegroups.com",
     url="https://github.com/common-workflow-language/schema_salad",
     download_url="https://github.com/common-workflow-language/schema_salad/releases",
     ext_modules=ext_modules,
     license="Apache 2.0",
-    python_requires=">=3.6,<3.12",
+    python_requires=">=3.6,<3.13",
     setup_requires=pytest_runner + ["setuptools_scm"],
     packages=["schema_salad", "schema_salad.tests", "schema_salad.avro"],
     package_data={
         "schema_salad": [
             "metaschema/*",
             "py.typed",
             "dotnet/*",
@@ -163,16 +165,16 @@
         "Environment :: Console",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: POSIX",
         "Operating System :: MacOS :: MacOS X",
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Typing :: Typed",
     ],
     use_scm_version=True,
 )
```

