# Comparing `tmp/metador_core-0.0.2.tar.gz` & `tmp/metador_core-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metador_core-0.0.2.tar", max compression
+gzip compressed data, was "metador_core-0.1.0.tar", max compression
```

## Comparing `metador_core-0.0.2.tar` & `metador_core-0.1.0.tar`

### file list

```diff
@@ -1,61 +1,152 @@
--rw-r--r--   0        0        0     1190 2022-12-12 13:34:25.100274 metador_core-0.0.2/LICENSE
--rw-r--r--   0        0        0     4689 2022-12-12 13:34:25.100274 metador_core-0.0.2/README.md
--rw-r--r--   0        0        0      232 2022-12-12 13:34:25.100274 metador_core-0.0.2/metador_core/__init__.py
--rw-r--r--   0        0        0     4637 2022-12-12 13:34:25.100274 metador_core-0.0.2/metador_core/container/__init__.py
--rw-r--r--   0        0        0     1756 2022-12-12 13:34:25.100274 metador_core-0.0.2/metador_core/container/drivers.py
--rw-r--r--   0        0        0    33450 2022-12-12 13:34:25.100274 metador_core-0.0.2/metador_core/container/interface.py
--rw-r--r--   0        0        0     2544 2022-12-12 13:34:25.100274 metador_core-0.0.2/metador_core/container/provider.py
--rw-r--r--   0        0        0     3746 2022-12-12 13:34:25.100274 metador_core-0.0.2/metador_core/container/types.py
--rw-r--r--   0        0        0     2892 2022-12-12 13:34:25.100274 metador_core-0.0.2/metador_core/container/utils.py
--rw-r--r--   0        0        0    22502 2022-12-12 13:34:25.100274 metador_core-0.0.2/metador_core/container/wrappers.py
--rw-r--r--   0        0        0    13590 2022-12-12 13:34:25.100274 metador_core-0.0.2/metador_core/harvester/__init__.py
--rw-r--r--   0        0        0     1380 2022-12-12 13:34:25.100274 metador_core-0.0.2/metador_core/harvester/common.py
--rw-r--r--   0        0        0    12010 2022-12-12 13:34:25.100274 metador_core-0.0.2/metador_core/ih5/PATCH_THEORY.md
--rw-r--r--   0        0        0     2204 2022-12-12 13:34:25.100274 metador_core-0.0.2/metador_core/ih5/__init__.py
--rw-r--r--   0        0        0      296 2022-12-12 13:34:25.100274 metador_core-0.0.2/metador_core/ih5/container.py
--rw-r--r--   0        0        0    12562 2022-12-12 13:34:25.100274 metador_core-0.0.2/metador_core/ih5/manifest.py
--rw-r--r--   0        0        0    27653 2022-12-12 13:34:25.100274 metador_core-0.0.2/metador_core/ih5/overlay.py
--rw-r--r--   0        0        0    25812 2022-12-12 13:34:25.100274 metador_core-0.0.2/metador_core/ih5/record.py
--rw-r--r--   0        0        0     3688 2022-12-12 13:34:25.100274 metador_core-0.0.2/metador_core/ih5/skeleton.py
--rw-r--r--   0        0        0    13595 2022-12-12 13:34:25.100274 metador_core-0.0.2/metador_core/packer/__init__.py
--rw-r--r--   0        0        0     5538 2022-12-12 13:34:25.100274 metador_core-0.0.2/metador_core/packer/example.py
--rw-r--r--   0        0        0     1270 2022-12-12 13:34:25.100274 metador_core-0.0.2/metador_core/packer/types.py
--rw-r--r--   0        0        0     3643 2022-12-12 13:34:25.100274 metador_core-0.0.2/metador_core/packer/utils.py
--rw-r--r--   0        0        0       50 2022-12-12 13:34:25.100274 metador_core-0.0.2/metador_core/plugin/__init__.py
--rw-r--r--   0        0        0     2488 2022-12-12 13:34:25.100274 metador_core-0.0.2/metador_core/plugin/entrypoints.py
--rw-r--r--   0        0        0    15954 2022-12-12 13:34:25.100274 metador_core-0.0.2/metador_core/plugin/interface.py
--rw-r--r--   0        0        0     4708 2022-12-12 13:34:25.100274 metador_core-0.0.2/metador_core/plugin/metaclass.py
--rw-r--r--   0        0        0     4267 2022-12-12 13:34:25.100274 metador_core-0.0.2/metador_core/plugin/types.py
--rw-r--r--   0        0        0     3021 2022-12-12 13:34:25.100274 metador_core-0.0.2/metador_core/plugin/util.py
--rw-r--r--   0        0        0     3462 2022-12-12 13:34:25.100274 metador_core-0.0.2/metador_core/plugins.py
--rw-r--r--   0        0        0       87 2022-12-12 13:34:25.100274 metador_core-0.0.2/metador_core/schema/__init__.py
--rw-r--r--   0        0        0     3812 2022-12-12 13:34:25.100274 metador_core-0.0.2/metador_core/schema/base.py
--rw-r--r--   0        0        0     4675 2022-12-12 13:34:25.104275 metador_core-0.0.2/metador_core/schema/common/__init__.py
--rw-r--r--   0        0        0     2876 2022-12-12 13:34:25.104275 metador_core-0.0.2/metador_core/schema/common/rocrate.py
--rw-r--r--   0        0        0     6523 2022-12-12 13:34:25.104275 metador_core-0.0.2/metador_core/schema/common/schemaorg.py
--rw-r--r--   0        0        0    17395 2022-12-12 13:34:25.104275 metador_core-0.0.2/metador_core/schema/core.py
--rw-r--r--   0        0        0     4606 2022-12-12 13:34:25.104275 metador_core-0.0.2/metador_core/schema/decorators.py
--rw-r--r--   0        0        0     3069 2022-12-12 13:34:25.104275 metador_core-0.0.2/metador_core/schema/encoder.py
--rw-r--r--   0        0        0     6189 2022-12-12 13:34:25.104275 metador_core-0.0.2/metador_core/schema/inspect.py
--rw-r--r--   0        0        0     8590 2022-12-12 13:34:25.104275 metador_core-0.0.2/metador_core/schema/jsonschema.py
--rw-r--r--   0        0        0     2766 2022-12-12 13:34:25.104275 metador_core-0.0.2/metador_core/schema/ld.py
--rw-r--r--   0        0        0     3402 2022-12-12 13:34:25.104275 metador_core-0.0.2/metador_core/schema/parser.py
--rw-r--r--   0        0        0    17384 2022-12-12 13:34:25.104275 metador_core-0.0.2/metador_core/schema/partial.py
--rw-r--r--   0        0        0     8155 2022-12-12 13:34:25.104275 metador_core-0.0.2/metador_core/schema/pg.py
--rw-r--r--   0        0        0     6088 2022-12-12 13:34:25.104275 metador_core-0.0.2/metador_core/schema/plugins.py
--rw-r--r--   0        0        0     4741 2022-12-12 13:34:25.104275 metador_core-0.0.2/metador_core/schema/types.py
--rw-r--r--   0        0        0      490 2022-12-12 13:34:25.104275 metador_core-0.0.2/metador_core/util/__init__.py
--rw-r--r--   0        0        0     9178 2022-12-12 13:34:25.104275 metador_core-0.0.2/metador_core/util/diff.py
--rw-r--r--   0        0        0     3269 2022-12-12 13:34:25.104275 metador_core-0.0.2/metador_core/util/hashsums.py
--rw-r--r--   0        0        0     1899 2022-12-12 13:34:25.104275 metador_core-0.0.2/metador_core/util/models.py
--rw-r--r--   0        0        0      510 2022-12-12 13:34:25.104275 metador_core-0.0.2/metador_core/util/pytest.py
--rw-r--r--   0        0        0     5874 2022-12-12 13:34:25.104275 metador_core-0.0.2/metador_core/util/typing.py
--rw-r--r--   0        0        0     8461 2022-12-12 13:34:25.104275 metador_core-0.0.2/metador_core/widget/__init__.py
--rw-r--r--   0        0        0     6254 2022-12-12 13:34:25.104275 metador_core-0.0.2/metador_core/widget/common.py
--rw-r--r--   0        0        0    11447 2022-12-12 13:34:25.104275 metador_core-0.0.2/metador_core/widget/dashboard.py
--rw-r--r--   0        0        0      893 2022-12-12 13:34:25.104275 metador_core-0.0.2/metador_core/widget/jupyter/__init__.py
--rw-r--r--   0        0        0     2830 2022-12-12 13:34:25.104275 metador_core-0.0.2/metador_core/widget/jupyter/standalone.py
--rw-r--r--   0        0        0     8740 2022-12-12 13:34:25.104275 metador_core-0.0.2/metador_core/widget/server/__init__.py
--rw-r--r--   0        0        0     4206 2022-12-12 13:34:25.104275 metador_core-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     8806 1970-01-01 00:00:00.000000 metador_core-0.0.2/setup.py
--rw-r--r--   0        0        0     6712 1970-01-01 00:00:00.000000 metador_core-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      872 2023-08-08 10:30:28.119934 metador_core-0.1.0/.reuse/dep5
+-rw-r--r--   0        0        0      876 2023-08-08 10:30:28.119934 metador_core-0.1.0/AUTHORS.md
+-rw-r--r--   0        0        0      762 2023-08-08 10:30:28.119934 metador_core-0.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0      726 2023-08-08 10:30:28.119934 metador_core-0.1.0/CITATION.cff
+-rw-r--r--   0        0        0     5446 2023-08-08 10:30:28.119934 metador_core-0.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2269 2023-08-08 10:30:28.119934 metador_core-0.1.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1190 2023-08-08 10:30:28.119934 metador_core-0.1.0/LICENSE
+drwxr-xr-x   0        0        0        0 2023-08-08 10:30:28.119934 metador_core-0.1.0/LICENSES/
+-rw-r--r--   0        0        0     7048 2023-08-08 10:30:28.119934 metador_core-0.1.0/LICENSES/CC0-1.0.txt
+-rw-r--r--   0        0        0     1078 2023-08-08 10:30:28.119934 metador_core-0.1.0/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     4119 2023-08-08 10:30:28.119934 metador_core-0.1.0/README.md
+-rw-r--r--   0        0        0     5613 2023-08-08 10:30:28.119934 metador_core-0.1.0/codemeta.json
+-rw-r--r--   0        0        0       22 2023-08-08 10:30:28.119934 metador_core-0.1.0/docs/changelog.md
+-rw-r--r--   0        0        0       28 2023-08-08 10:30:28.119934 metador_core-0.1.0/docs/code_of_conduct.md
+-rw-r--r--   0        0        0       25 2023-08-08 10:30:28.119934 metador_core-0.1.0/docs/contributing.md
+-rw-r--r--   0        0        0       20 2023-08-08 10:30:28.119934 metador_core-0.1.0/docs/credits.md
+-rw-r--r--   0        0        0      182 2023-08-08 10:30:28.119934 metador_core-0.1.0/docs/css/style.css
+-rw-r--r--   0        0        0    13595 2023-08-08 10:30:28.119934 metador_core-0.1.0/docs/dev_guide.md
+-rw-r--r--   0        0        0      179 2023-08-08 10:30:28.119934 metador_core-0.1.0/docs/index.md
+-rw-r--r--   0        0        0      473 2023-08-08 10:30:28.119934 metador_core-0.1.0/docs/license.md
+-rw-r--r--   0        0        0      278 2023-08-08 10:30:28.119934 metador_core-0.1.0/docs/logo.svg
+-rw-r--r--   0        0        0    69142 2023-08-08 10:30:28.119934 metador_core-0.1.0/docs/notebooks/01_MetadorContainer.ipynb
+-rw-r--r--   0        0        0    21785 2023-08-08 10:30:28.119934 metador_core-0.1.0/docs/notebooks/02_YourFirstMetadorPlugin.ipynb
+-rw-r--r--   0        0        0    76533 2023-08-08 10:30:28.119934 metador_core-0.1.0/docs/notebooks/03_Schemas.ipynb
+-rw-r--r--   0        0        0    23840 2023-08-08 10:30:28.123934 metador_core-0.1.0/docs/notebooks/03b_SemanticsInteroperability.ipynb
+-rw-r--r--   0        0        0      571 2023-08-08 10:30:28.123934 metador_core-0.1.0/docs/notebooks/04_Harvesters.ipynb
+-rw-r--r--   0        0        0   120852 2023-08-08 10:30:28.123934 metador_core-0.1.0/docs/notebooks/05_Widgets.ipynb
+-rw-r--r--   0        0        0      808 2023-08-08 10:30:28.123934 metador_core-0.1.0/docs/notebooks/about.md
+-rw-r--r--   0        0        0      218 2023-08-08 10:30:28.123934 metador_core-0.1.0/docs/notebooks/files/test.bibmeta.yaml
+-rw-r--r--   0        0        0       90 2023-08-08 10:30:28.123934 metador_core-0.1.0/docs/notebooks/files/test.html
+-rw-r--r--   0        0        0       31 2023-08-08 10:30:28.123934 metador_core-0.1.0/docs/notebooks/files/test.json
+-rw-r--r--   0        0        0       37 2023-08-08 10:30:28.123934 metador_core-0.1.0/docs/notebooks/files/test.md
+-rw-r--r--   0        0        0    14812 2023-08-08 10:30:28.123934 metador_core-0.1.0/docs/notebooks/files/test.pdf
+-rw-r--r--   0        0        0    10102 2023-08-08 10:30:28.123934 metador_core-0.1.0/docs/notebooks/files/test.png
+-rw-r--r--   0        0        0     8083 2023-08-08 10:30:28.123934 metador_core-0.1.0/docs/notebooks/schema_flowchart.dot
+-rw-r--r--   0        0        0   368924 2023-08-08 10:30:28.123934 metador_core-0.1.0/docs/notebooks/schema_flowchart.png
+-rw-r--r--   0        0        0      229 2023-08-08 10:30:28.123934 metador_core-0.1.0/docs/overrides/main.html
+-rw-r--r--   0        0        0      699 2023-08-08 10:30:28.123934 metador_core-0.1.0/docs/overrides/partials/copyright.html
+-rw-r--r--   0        0        0       29 2023-08-08 10:30:28.123934 metador_core-0.1.0/docs/quickstart.md
+-rw-r--r--   0        0        0     1218 2023-08-08 10:30:28.123934 metador_core-0.1.0/docs/scripts/coverage_status.py
+-rw-r--r--   0        0        0      994 2023-08-08 10:30:28.123934 metador_core-0.1.0/docs/scripts/gen_ref_pages.py
+-rw-r--r--   0        0        0     5814 2023-08-08 10:30:28.123934 metador_core-0.1.0/mkdocs.yml
+-rw-r--r--   0        0        0     6328 2023-08-08 10:30:28.127934 metador_core-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      235 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/__init__.py
+-rw-r--r--   0        0        0     4637 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/container/__init__.py
+-rw-r--r--   0        0        0     2748 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/container/drivers.py
+-rw-r--r--   0        0        0    37053 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/container/interface.py
+-rw-r--r--   0        0        0     3979 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/container/protocols.py
+-rw-r--r--   0        0        0     3364 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/container/provider.py
+-rw-r--r--   0        0        0     2891 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/container/utils.py
+-rw-r--r--   0        0        0    23140 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/container/wrappers.py
+-rw-r--r--   0        0        0    13575 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/harvester/__init__.py
+-rw-r--r--   0        0        0     1380 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/harvester/common.py
+-rw-r--r--   0        0        0    12010 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/ih5/PATCH_THEORY.md
+-rw-r--r--   0        0        0     2204 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/ih5/__init__.py
+-rw-r--r--   0        0        0      370 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/ih5/container.py
+-rw-r--r--   0        0        0    12626 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/ih5/manifest.py
+-rw-r--r--   0        0        0    27352 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/ih5/overlay.py
+-rw-r--r--   0        0        0    26125 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/ih5/record.py
+-rw-r--r--   0        0        0     3659 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/ih5/skeleton.py
+-rw-r--r--   0        0        0    13592 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/packer/__init__.py
+-rw-r--r--   0        0        0     5536 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/packer/example.py
+-rw-r--r--   0        0        0     1270 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/packer/types.py
+-rw-r--r--   0        0        0     3633 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/packer/utils.py
+-rw-r--r--   0        0        0       50 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/plugin/__init__.py
+-rw-r--r--   0        0        0     2480 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/plugin/entrypoints.py
+-rw-r--r--   0        0        0    15890 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/plugin/interface.py
+-rw-r--r--   0        0        0     4748 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/plugin/metaclass.py
+-rw-r--r--   0        0        0     4397 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/plugin/types.py
+-rw-r--r--   0        0        0     3021 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/plugin/util.py
+-rw-r--r--   0        0        0     3647 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/plugins.py
+-rw-r--r--   0        0        0      119 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/rdf/__init__.py
+-rw-r--r--   0        0        0     3326 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/rdf/lib.py
+-rw-r--r--   0        0        0     5392 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/rdf/skos.py
+-rw-r--r--   0        0        0       87 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/schema/__init__.py
+-rw-r--r--   0        0        0     3495 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/schema/base.py
+-rw-r--r--   0        0        0     4675 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/schema/common/__init__.py
+-rw-r--r--   0        0        0     3043 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/schema/common/rocrate.py
+-rw-r--r--   0        0        0    10677 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/schema/common/schemaorg.py
+-rw-r--r--   0        0        0    17502 2023-08-08 10:30:28.127934 metador_core-0.1.0/src/metador_core/schema/core.py
+-rw-r--r--   0        0        0     5926 2023-08-08 10:30:28.131934 metador_core-0.1.0/src/metador_core/schema/decorators.py
+-rw-r--r--   0        0        0     3069 2023-08-08 10:30:28.131934 metador_core-0.1.0/src/metador_core/schema/encoder.py
+-rw-r--r--   0        0        0     6189 2023-08-08 10:30:28.131934 metador_core-0.1.0/src/metador_core/schema/inspect.py
+-rw-r--r--   0        0        0     8746 2023-08-08 10:30:28.131934 metador_core-0.1.0/src/metador_core/schema/jsonschema.py
+-rw-r--r--   0        0        0     2946 2023-08-08 10:30:28.131934 metador_core-0.1.0/src/metador_core/schema/ld.py
+-rw-r--r--   0        0        0     3584 2023-08-08 10:30:28.131934 metador_core-0.1.0/src/metador_core/schema/parser.py
+-rw-r--r--   0        0        0    17590 2023-08-08 10:30:28.131934 metador_core-0.1.0/src/metador_core/schema/partial.py
+-rw-r--r--   0        0        0     8433 2023-08-08 10:30:28.131934 metador_core-0.1.0/src/metador_core/schema/pg.py
+-rw-r--r--   0        0        0     6088 2023-08-08 10:30:28.131934 metador_core-0.1.0/src/metador_core/schema/plugins.py
+-rw-r--r--   0        0        0     4741 2023-08-08 10:30:28.131934 metador_core-0.1.0/src/metador_core/schema/types.py
+-rw-r--r--   0        0        0      659 2023-08-08 10:30:28.131934 metador_core-0.1.0/src/metador_core/util/__init__.py
+-rw-r--r--   0        0        0     9178 2023-08-08 10:30:28.131934 metador_core-0.1.0/src/metador_core/util/diff.py
+-rw-r--r--   0        0        0     2269 2023-08-08 10:30:28.131934 metador_core-0.1.0/src/metador_core/util/enum.py
+-rw-r--r--   0        0        0     3263 2023-08-08 10:30:28.131934 metador_core-0.1.0/src/metador_core/util/hashsums.py
+-rw-r--r--   0        0        0     1936 2023-08-08 10:30:28.131934 metador_core-0.1.0/src/metador_core/util/models.py
+-rw-r--r--   0        0        0      530 2023-08-08 10:30:28.131934 metador_core-0.1.0/src/metador_core/util/pytest.py
+-rw-r--r--   0        0        0     6441 2023-08-08 10:30:28.131934 metador_core-0.1.0/src/metador_core/util/typing.py
+-rw-r--r--   0        0        0     9304 2023-08-08 10:30:28.131934 metador_core-0.1.0/src/metador_core/widget/__init__.py
+-rw-r--r--   0        0        0     7009 2023-08-08 10:30:28.131934 metador_core-0.1.0/src/metador_core/widget/common.py
+-rw-r--r--   0        0        0    14981 2023-08-08 10:30:28.131934 metador_core-0.1.0/src/metador_core/widget/dashboard.py
+-rw-r--r--   0        0        0      838 2023-08-08 10:30:28.131934 metador_core-0.1.0/src/metador_core/widget/jupyter/__init__.py
+-rw-r--r--   0        0        0     2882 2023-08-08 10:30:28.131934 metador_core-0.1.0/src/metador_core/widget/jupyter/standalone.py
+-rw-r--r--   0        0        0    12221 2023-08-08 10:30:28.131934 metador_core-0.1.0/src/metador_core/widget/server/__init__.py
+-rw-r--r--   0        0        0       28 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     2867 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/conftest.py
+-rw-r--r--   0        0        0     1005 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/container/conftest.py
+-rw-r--r--   0        0        0    15720 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/container/test_container_interface.py
+-rw-r--r--   0        0        0     6944 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/container/test_container_protocols_drivers.py
+-rw-r--r--   0        0        0      741 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/container/test_container_provider.py
+-rw-r--r--   0        0        0     2106 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/container/test_container_utils.py
+-rw-r--r--   0        0        0       18 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/data/dirdiff2/_meta.yaml
+-rw-r--r--   0        0        0       14 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/data/dirdiff2/a/b
+-rw-r--r--   0        0        0        9 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/data/dirdiff2/e/g
+-rw-r--r--   0        0        0       12 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/data/dirdiff2/f
+-rw-r--r--   0        0        0        9 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/data/dirdiff2/h
+-rw-r--r--   0        0        0        0 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/data/dirdiff2/z
+-rw-r--r--   0        0        0     1995 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/examples/test_mixed_files_container.py
+-rw-r--r--   0        0        0    19714 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/ih5/test_ih5_overlay.py
+-rw-r--r--   0        0        0    18003 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/ih5/test_ih5_record.py
+-rw-r--r--   0        0        0     6174 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/ih5/test_ih5_skeleton_stub.py
+-rw-r--r--   0        0        0     7204 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/ih5/test_ih5mf_record.py
+-rw-r--r--   0        0        0     1037 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/packer/test_example_packer.py
+-rw-r--r--   0        0        0     3043 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/packer/test_packer_interface.py
+-rw-r--r--   0        0        0        0 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/plugin/__init__.py
+-rw-r--r--   0        0        0     3105 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/plugin/dummy_plugins.py
+-rw-r--r--   0        0        0    10992 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/plugin/test_interface.py
+-rw-r--r--   0        0        0     1723 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/plugin/test_metaclass.py
+-rw-r--r--   0        0        0      702 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/plugin/test_plugins_import.py
+-rw-r--r--   0        0        0     3214 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/plugin/test_types.py
+-rw-r--r--   0        0        0     1947 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/plugin/test_util.py
+-rw-r--r--   0        0        0        0 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/schema/__init__.py
+-rw-r--r--   0        0        0      124 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/schema/conftest.py
+-rw-r--r--   0        0        0     2115 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/schema/test_base.py
+-rw-r--r--   0        0        0     5774 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/schema/test_core.py
+-rw-r--r--   0        0        0     5519 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/schema/test_decorators.py
+-rw-r--r--   0        0        0     1422 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/schema/test_default_schemas.py
+-rw-r--r--   0        0        0     1433 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/schema/test_inspect.py
+-rw-r--r--   0        0        0     3698 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/schema/test_jsonschema.py
+-rw-r--r--   0        0        0     3943 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/schema/test_ld.py
+-rw-r--r--   0        0        0     4689 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/schema/test_parser_encoder.py
+-rw-r--r--   0        0        0     4584 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/schema/test_partial.py
+-rw-r--r--   0        0        0     1301 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/schema/test_plugingroup.py
+-rw-r--r--   0        0        0     2886 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/schema/test_plugins_schemas.py
+-rw-r--r--   0        0        0      113 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/schema/test_schema_invariants.py
+-rw-r--r--   0        0        0     5920 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/schema/test_types.py
+-rw-r--r--   0        0        0        0 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/util/__init__.py
+-rw-r--r--   0        0        0     3686 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/util/test_dirdiff.py
+-rw-r--r--   0        0        0      463 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/util/test_hashsums.py
+-rw-r--r--   0        0        0     1001 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/util/test_misc.py
+-rw-r--r--   0        0        0     2770 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/util/test_models.py
+-rw-r--r--   0        0        0     6647 2023-08-08 10:30:28.131934 metador_core-0.1.0/tests/util/test_typing.py
+-rw-r--r--   0        0        0     6189 1970-01-01 00:00:00.000000 metador_core-0.1.0/PKG-INFO
```

### Comparing `metador_core-0.0.2/LICENSE` & `metador_core-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metador_core-0.0.2/metador_core/container/__init__.py` & `metador_core-0.1.0/src/metador_core/container/__init__.py`

 * *Files identical despite different names*

### Comparing `metador_core-0.0.2/metador_core/container/interface.py` & `metador_core-0.1.0/src/metador_core/container/interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import json
 from dataclasses import dataclass
+from enum import Enum, auto
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     ItemsView,
     Iterator,
     KeysView,
@@ -33,22 +34,46 @@
 from .drivers import (
     METADOR_DRIVERS,
     MetadorDriver,
     MetadorDriverEnum,
     get_driver_type,
     get_source,
 )
-from .types import H5DatasetLike, H5FileLike, H5GroupLike
+from .protocols import H5DatasetLike, H5FileLike, H5GroupLike
 
 if TYPE_CHECKING:
     from .wrappers import MetadorContainer, MetadorNode
 
 S = TypeVar("S", bound=MetadataSchema)
 
 
+class NodeAcl(Enum):
+    """Metador node soft access control flags.
+
+    Soft means - they can be bypassed, it is about trying to prevent errors.
+
+    Group nodes inherit their ACL flags to child nodes.
+    """
+
+    # NOTE: maybe refactor this to IntFlag? Then e.g. restrict() interface can be like:
+    # node.restrict(acl=NodeAcl.read_only | NodeAcl.local_only)
+
+    read_only = auto()
+    """Forbid calling methods mutating contents of (meta)data."""
+
+    local_only = auto()
+    """Forbid access to parents beyond the initial local node."""
+
+    skel_only = auto()
+    """Forbid reading datasets and metadata, only existence can be checked."""
+
+
+NodeAclFlags: TypeAlias = Dict[NodeAcl, bool]
+
+
 @dataclass
 class StoredMetadata:
     """Information about a metadata schema instance stored at a node."""
 
     uuid: UUID
     """UUID identifying the metadata object in the container.
 
@@ -58,20 +83,25 @@
     schema: PluginRef
     """Schema the object is an instance of."""
 
     node: H5DatasetLike
     """Node with serialized metadata object."""
 
     def to_path(self):
+        """Return path of metadata object.
+
+        (E.g. to return canonical path for copying TOC link nodes)
+        """
         prefix = self.node.parent.name
         ep_name = to_ep_name(self.schema.name, self.schema.version)
         return f"{prefix}/{ep_name}={self.uuid}"
 
     @staticmethod
     def from_node(obj: H5DatasetLike) -> StoredMetadata:
+        """Instantiate info about a stored metadata node."""
         path = obj.name
         segs = path.lstrip("/").split("/")
         ep_name, uuid_str = segs.pop().split("=")
         s_name, s_vers = from_ep_name(EPName(ep_name))
         uuid = UUID(uuid_str)
         s_ref = schemas.PluginRef(name=s_name, version=s_vers)
         return StoredMetadata(uuid=uuid, schema=s_ref, node=obj)
@@ -217,19 +247,19 @@
         """Return names of explicitly attached metadata objects.
 
         Transitive parent schemas are not included.
         """
         return self._objs.keys()
 
     def values(self) -> ValuesView[StoredMetadata]:
-        self._node._guard_skel_only()
+        self._node._guard_acl(NodeAcl.skel_only)
         return self._objs.values()
 
     def items(self) -> ItemsView[str, StoredMetadata]:
-        self._node._guard_skel_only()
+        self._node._guard_acl(NodeAcl.skel_only)
         return self._objs.items()
 
     # ----
 
     def __len__(self) -> int:
         """Return number of explicitly attached metadata objects.
 
@@ -244,48 +274,60 @@
         """
         return iter(self.keys())
 
     # ----
 
     def query(
         self,
-        schema: Union[str, Type[MetadataSchema]] = "",
+        schema: Union[
+            str, Tuple[str, Optional[SemVerTuple]], PluginRef, Type[MetadataSchema]
+        ] = "",
         version: Optional[SemVerTuple] = None,
     ) -> Iterator[PluginRef]:
         """Return schema names for which objects at this node are compatible with passed schema.
 
         Will also consider compatible child schema instances.
 
         Returned iterator will yield passed schema first, if an object is available.
-        Otherwise, the order is not specified.
+        Apart from this, the order is not specified.
         """
         schema_name, schema_ver = plugin_args(schema, version)
-        # no schema selected -> anything goes
+        # no schema selected -> list everything
         if not schema_name:
             for obj in self.values():
                 yield obj.schema
             return
 
         # try exact schema (in any compatible version, if version specified)
         if obj := self._get_raw(schema_name, schema_ver):
             yield obj.schema
 
-        # next, try schemas compatible with any child schemas
-        compat = self._mc.metador.schemas.children(schema_name, schema_ver)
+        # next, try compatible child schemas of compatible versions of requested schema
+        compat = set().union(
+            *(
+                self._mc.metador.schemas.children(ref)
+                for ref in self._mc.metador.schemas.versions(schema_name, schema_ver)
+            )
+        )
         avail = {self._get_raw(s).schema for s in self.keys()}
         for s_ref in avail.intersection(compat):
             yield s_ref
 
-    def __contains__(self, schema: Union[str, MetadataSchema]) -> bool:
+    def __contains__(
+        self,
+        schema: Union[
+            str, Tuple[str, Optional[SemVerTuple]], PluginRef, Type[MetadataSchema]
+        ],
+    ) -> bool:
         """Check whether a compatible metadata object for given schema exists.
 
         Will also consider compatible child schema instances.
         """
-        if schema == "":
-            return False
+        if schema == "" or isinstance(schema, tuple) and schema[0] == "":
+            return False  # empty query lists everything, here the logic is inverted!
         return next(self.query(schema), None) is not None
 
     @overload
     def __getitem__(self, schema: str) -> MetadataSchema:
         ...
 
     @overload
@@ -313,21 +355,25 @@
     def get(
         self, schema: Union[str, Type[S]], version: Optional[SemVerTuple] = None
     ) -> Optional[Union[MetadataSchema, S]]:
         """Get a parsed metadata object matching the given schema (if it exists).
 
         Will also consider compatible child schema instances.
         """
-        self._node._guard_skel_only()
+        self._node._guard_acl(NodeAcl.skel_only)
+
+        # normalize arguments
         schema_name, schema_ver = plugin_args(schema, version)
 
+        # get a compatible schema instance that is available at this node
         compat_schema = next(self.query(schema_name, schema_ver), None)
         if not compat_schema:
-            return None
+            return None  # not found
 
+        # get class of schema and parse object
         schema_class = self._require_schema(schema_name, schema_ver)
         if obj := self._get_raw(compat_schema.name, compat_schema.version):
             return cast(S, self._parse_obj(schema_class, obj.node[()]))
         return None
 
     def __setitem__(
         self, schema: Union[str, Type[S]], value: Union[Dict[str, Any], MetadataSchema]
@@ -338,15 +384,15 @@
 
         Raises TypeError if passed schema is marked auxiliary.
 
         Raises ValueError if an object for the schema already exists.
 
         Raises ValidationError if passed object is not valid for the schema.
         """
-        self._node._guard_read_only()
+        self._node._guard_acl(NodeAcl.read_only)
         schema_name, schema_ver = plugin_args(schema)
 
         # if self.get(schema_name, schema_ver):  # <- also subclass schemas
         # NOTE: for practical reasons let's be more lenient here and allow redundancy
         # hence only check if exact schema (modulo version) is already there
         if self._get_raw(schema_name):  # <- only same schema
             msg = f"Metadata object for schema {schema_name} already exists!"
@@ -360,15 +406,15 @@
         """Delete metadata object explicitly stored for the passed schema.
 
         If a schema class is passed, its version is ignored,
         as each node may contain at most one explicit instance per schema.
 
         Raises KeyError if no metadata object for that schema exists.
         """
-        self._node._guard_read_only()
+        self._node._guard_acl(NodeAcl.read_only)
         schema_name, _ = plugin_args(schema)
 
         if self._get_raw(schema_name) is None:
             raise KeyError(schema_name)  # no (explicit) metadata object
 
         self._del_raw(schema_name)
 
@@ -492,15 +538,20 @@
     def find_missing(self, path: H5GroupLike) -> List[H5DatasetLike]:
         """Return list of metadata objects not listed in TOC."""
         missing = []
 
         def collect_missing(_, node):
             if not M.is_internal_path(node.name, M.METADOR_META_PREF):
                 return  # not a metador metadata path
+            if M.is_meta_base_path(node.name):
+                # top dir, not a "link dataset",
+                # e.g. /.../foo/metador_meta_ or /.../metador_meta_foo
+                return
 
+            # now we assume we have a path to a metadata link object in the group
             obj = StoredMetadata.from_node(node)
             known = obj.uuid in self._toc_path
             # check UUID collision: i.e., used in TOC, but points elsewhere
             # (requires fixing up the name of this object / new UUID)
             # implies that THIS object IS missing in the TOC
             collision = known and self.resolve(obj.uuid) != node.name
             if not known or collision:
@@ -518,17 +569,21 @@
         for node in missing:
             obj = StoredMetadata.from_node(node)
             if update and obj.uuid in self._toc_path:
                 # update target of existing link (e.g. for move)
                 self.update(obj.uuid, node.name)
             else:
                 # assign new UUID (e.g. for copy)
+                # (copied metadata node refers to some other uuid in the name)
                 obj.uuid = self.fresh_uuid()
                 new_path = obj.to_path()
+                # rename the metadata node to point to the new UUID
                 self._raw.move(node.name, new_path)
+                obj.node = cast(H5DatasetLike, self._raw[new_path])
+                # register the object with the new UUID in the TOC
                 self.register(obj)
 
 
 class TOCSchemas:
     """Schema management for schemas used in the container.
 
     Interface is made to mimic PGSchema wherever it makes sense.
@@ -631,15 +686,15 @@
         self._raw: H5FileLike = raw_cont
         """Raw underlying container (for quick access)."""
 
         self._pkgs = toc_packages
         """TOC package metadata manager object."""
 
         self._schemas: Set[PluginRef] = set()
-        """Stored JSON Schemas of used schemas."""
+        """Stored JSON Schemas of actually used schemas."""
 
         self._parents: Dict[PluginRef, List[PluginRef]] = {}
         """Parents of a used json schema (i.e. other partially compatible schemas)."""
 
         self._children: Dict[PluginRef, Set[PluginRef]] = {}
         """Children of a used json schema (i.e. other fully compatible schemas)."""
 
@@ -682,23 +737,43 @@
         self, schema, version: Optional[SemVerTuple] = None
     ) -> List[PluginRef]:
         """Like PGSchema.parent_path, but with respect to container deps."""
         name, vers = plugin_args(schema, version, require_version=True)
         s_ref = schemas.PluginRef(name=name, version=vers)
         return self._parents[s_ref]
 
+    def versions(
+        self, p_name: str, version: Optional[SemVerTuple] = None
+    ) -> List[PluginRef]:
+        """Like PGSchema.versions, but with respect to container deps."""
+        # NOTE: using _children instead of _schemas because some are only listed
+        # due to their appearance in the parent_path of some actually used schema
+        # but we need them here for "parent compatibility" to work right.
+        refs = list(filter(lambda s: s.name == p_name, self._children))
+
+        if version is None:
+            return refs
+        # filter plugins for compatible version
+        requested = schemas.PluginRef(name=p_name, version=version)
+        # NOTE: here "supports" arguments are reversed (compared to "plugin versions")!
+        # because its about instances (that must be "below" the requested schema version)
+        return [ref for ref in refs if requested.supports(ref)]
+
     def children(self, schema, version: Optional[SemVerTuple] = None) -> Set[PluginRef]:
         """Like PGSchema.children, but with respect to container deps."""
         name, vers = plugin_args(schema, version)
         if vers is not None:
             s_refs = [schemas.PluginRef(name=name, version=vers)]
         else:
             # if no version is given, collect all possibilities
             s_refs = [ref for ref in self._children.keys() if ref.name == name]
-        return set.union(set(), *map(self._children.__getitem__, s_refs))
+        # return all that can be actually retrieved
+        return set().union(
+            *filter(lambda x: x is not None, map(self._children.get, s_refs))
+        )
 
     # ----
 
     def __len__(self):
         return len(self._schemas)
 
     def __iter__(self):
@@ -706,15 +781,15 @@
 
     def __contains__(self, schema_ref: PluginRef):
         return schema_ref in self._schemas
 
     def __getitem__(self, schema_ref: PluginRef):
         node_path = self._jsonschema_path_for(schema_ref)
         assert node_path in self._raw
-        return self._load_json(self._raw.require_dataset(node_path))
+        return self._load_json(cast(H5DatasetLike, self._raw[node_path]))
 
     def get(self, schema_ref: PluginRef):
         try:
             self[schema_ref]
         except KeyError:
             return None
 
@@ -820,26 +895,28 @@
     """Interface to the Metador metadata index (table of contents) of a container."""
 
     def __init__(self, container: MetadorContainer):
         self._container = container
         self._raw = self._container.__wrapped__
 
         ver = self.spec_version if M.METADOR_VERSION_PATH in self._raw else None
-        if ver is None and self._container.mode == "r":
-            msg = "Container is read-only and does not look like a Metador container! "
-            msg += "Please open in writable mode to initialize Metador structures!"
-            raise ValueError(msg)
-        if ver is not None and ver >= [2]:
-            msg = f"Unsupported Metador container version: {ver}"
-            raise ValueError(msg)
+        if ver:
+            if ver >= [2]:
+                msg = f"Unsupported Metador container version: {ver}"
+                raise ValueError(msg)
+        else:
+            if self._container.acl[NodeAcl.read_only]:
+                msg = "Container is read-only and does not look like a Metador container! "
+                msg += "Please open in writable mode to initialize Metador structures!"
+                raise ValueError(msg)
 
-        # writable + no version = fresh (for metador), initialize it
-        if ver is None:
+            # writable + no version = fresh (for metador), initialize it
             self._raw[M.METADOR_VERSION_PATH] = M.METADOR_SPEC_VERSION
             self._raw[M.METADOR_UUID_PATH] = str(uuid1())
+
         # if we're here, we have a prepared container TOC structure
 
         # proceed to initialize TOC
         self._driver_type: MetadorDriverEnum = get_driver_type(self._raw)
 
         self._packages = TOCPackages(self._raw)
         self._schemas = TOCSchemas(self._raw, self._packages)
@@ -878,34 +955,42 @@
         return list(map(int, ver[()].decode("utf-8").split(".")))
 
     @property
     def schemas(self):
         """Information about all schemas used for metadata objects in this container."""
         return self._schemas
 
-    @overload
     def query(
-        self, schema: str, version: Optional[SemVerTuple] = None
-    ) -> Dict[MetadorNode, MetadataSchema]:
-        ...
+        self,
+        schema: Union[str, Type[S]],
+        version: Optional[SemVerTuple] = None,
+        *,
+        node: Optional[MetadorNode] = None,
+    ) -> Iterator[MetadorNode]:
+        """Return nodes that contain a metadata object compatible with the given schema."""
+        schema_name, schema_ver = plugin_args(schema, version)
+        if not schema_name:  # could be e.g. empty string
+            msg = "A schema name, plugin reference or class must be provided!"
+            raise ValueError(msg)
 
-    @overload
-    def query(
-        self, schema: Type[S], version: Optional[SemVerTuple] = None
-    ) -> Dict[MetadorNode, S]:
-        ...
+        start_node: MetadorNode = node or self._container["/"]
 
-    def query(
-        self, schema: Union[str, Type[S]] = "", version: Optional[SemVerTuple] = None
-    ) -> Dict[MetadorNode, Union[MetadataSchema, S]]:
-        """Return nodes that contain a metadata object valid for the given schema."""
-        schema_name, schema_ver = plugin_args(schema, version)
-        ret: Dict[MetadorNode, Union[MetadataSchema, S]] = {}
-        if obj := self._container.meta.get(schema_name, schema_ver):
-            ret[self._container["/"]] = obj
+        # check start node metadata explicitly
+        if (schema_name, schema_ver) in start_node.meta:
+            yield start_node
+
+        if not isinstance(start_node, H5GroupLike):
+            return  # the node is not group-like, cannot be traversed down
+
+        # collect nodes below start node recursively
+        # NOTE: yielding from the collect_nodes does not work :'(
+        # so we have to actually materialize the list >.<
+        # but we expose only the generator interface anyway (better design)
+        # (maybe consider replacing visititems with a custom traversal here)
+        ret: List[MetadorNode] = []
 
         def collect_nodes(_, node: MetadorNode):
-            if obj := node.meta.get(schema_name, schema_ver):
-                ret[node] = obj
+            if (schema_name, schema_ver) in node.meta:
+                ret.append(node)
 
-        self._container.visititems(collect_nodes)
-        return ret
+        start_node.visititems(collect_nodes)
+        yield from iter(ret)
```

### Comparing `metador_core-0.0.2/metador_core/container/provider.py` & `metador_core-0.1.0/src/metador_core/container/provider.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Abstract Metador container provider interface."""
-from typing import Any, Dict, Generic, Optional, Protocol, Tuple, Type, TypeVar
+from typing import Any, Dict, Generic, Optional, Protocol, Tuple, Type, TypeVar, Union
 
 from .wrappers import MetadorContainer, MetadorDriver
 
 T = TypeVar("T")
 
 
 class ContainerProxy(Protocol[T]):
@@ -21,30 +21,38 @@
     container-centric Flask blueprints, so they can be easier reused in
     different backends and services.
 
     Note that only containment and retrieval are possible - on purpose.
     Knowing and iterating over all containers in a system is not always possible.
     """
 
+    def __contains__(self, key: T) -> bool:
+        """Return whether a resource key is known to the proxy."""
+        # return self.get(key) is not None
+
     def get(self, key: T) -> Optional[MetadorContainer]:
-        ...
+        """Get a container instance, if resource key is known to the proxy.
 
-    def __contains__(self, key: T) -> bool:
-        return self.get(key) is None
+        Implement this method in subclasses to support the minimal interface.
+        """
 
     def __getitem__(self, key: T) -> T:
+        """Get a container instance, if resource key is known to the proxy.
+
+        Default implementation is in terms of `get`.
+        """
         if ret := self.get(key):
             return ret
         raise KeyError(key)
 
 
 ContainerArgs = Tuple[Type[MetadorDriver], Any]
 """Pair of (driver class, suitable driver arguments).
 
-Must be such that `MetadorContainer(driver(source))` yields a container.
+Must be such that `MetadorContainer(driver(source))` yields a working container.
 """
 
 
 class SimpleContainerProvider(Generic[T], ContainerProxy[T]):
     """Dict-backed container proxy.
 
     It is a minimal reasonable implementation for the interface that can be
@@ -54,24 +62,32 @@
 
     _known: Dict[T, ContainerArgs]
     """Mapping from container identifier to MetadorContainer constructor args."""
 
     def __init__(self):
         self._known = {}
 
+    def __contains__(self, key: T) -> bool:
+        return key in self._known
+
     def get(self, key: T) -> Optional[MetadorContainer]:
         """Get an open container file to access data and metadata, if it exists."""
         if key not in self._known:
             return None
         driver, source = self._known[key]
         return MetadorContainer(driver(source))
 
     # ----
 
     def __delitem__(self, key: T):
         del self._known[key]
 
-    def __setitem__(self, key: T, value: ContainerArgs):
-        self._known[key] = value
+    def __setitem__(self, key: T, value: Union[ContainerArgs, MetadorContainer]):
+        # NOTE: can't do instance check here, because MetadorContainer is a wrapper itself
+        # so we check if a container is passed by presence of the .metador attribute
+        if container_toc := getattr(value, "metador", None):
+            self._known[key] = (container_toc.driver, container_toc.source)
+        else:
+            self._known[key] = value
 
     def keys(self):
         return self._known.keys()
```

### Comparing `metador_core-0.0.2/metador_core/container/types.py` & `metador_core-0.1.0/src/metador_core/container/protocols.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-"""
-Protocol roughly formalizing the overlap of h5py.File and IH5Record API.
+"""Protocol roughly formalizing the overlap of h5py.File and IH5Record API.
 
 We build the MetadorContainer interface assuming only these methods.
 """
 from __future__ import annotations
 
 from typing import (
     Any,
     Callable,
     ItemsView,
     Iterable,
     KeysView,
+    Literal,
     MutableMapping,
     Optional,
     Protocol,
     TypeVar,
     Union,
     ValuesView,
     runtime_checkable,
 )
 
-from typing_extensions import Literal
-
-from ..ih5.record import OpenMode
+from typing_extensions import get_args
 
 
 @runtime_checkable
-class H5NodeLike(Protocol):
+class H5NodeLike(Protocol):  # pragma: no cover
     """HDF5 Files, Groups and Datasets are all Nodes."""
 
     @property
     def name(self) -> str:
         """Absolute path of the node."""
 
     @property
@@ -43,15 +41,15 @@
 
     @property
     def file(self) -> H5FileLike:
         """Original file-like object this node belongs to."""
 
 
 @runtime_checkable
-class H5DatasetLike(H5NodeLike, Protocol):
+class H5DatasetLike(H5NodeLike, Protocol):  # pragma: no cover
     """Datasets provide numpy-style indexing into data.
 
     Metador containers use it for storing bytes,
     and for getting bytes out again using [()].
     """
 
     def __getitem__(self, key: Any) -> Any:
@@ -63,21 +61,20 @@
     # needed to distinguish from other types:
     @property
     def ndim(self) -> int:
         """Numpy-style dimensionality."""
 
 
 CallbackResult = TypeVar("CallbackResult")
-VisititemsCallback = Callable[[str, H5NodeLike], Optional[CallbackResult]]
 VisitCallback = Callable[[str], Optional[CallbackResult]]
+VisititemsCallback = Callable[[str, H5NodeLike], Optional[CallbackResult]]
 
 
 @runtime_checkable
-class H5GroupLike(H5NodeLike, Protocol):
-
+class H5GroupLike(H5NodeLike, Protocol):  # pragma: no cover
     # MutableMapping-like
 
     def __getitem__(self, name: str) -> Union[H5GroupLike, H5DatasetLike]:
         ...
 
     def __setitem__(self, name: str, obj) -> None:
         ...
@@ -108,19 +105,19 @@
         ...
 
     def get(self, name: str, *args, **kwargs) -> Union[H5GroupLike, H5DatasetLike]:
         ...
 
     # h5py specific
 
-    def visititems(self, func: VisititemsCallback) -> CallbackResult:
+    def visititems(self, func: VisititemsCallback) -> Optional[CallbackResult]:
         # returns value returned from callback
         ...
 
-    def visit(self, func: VisitCallback) -> CallbackResult:
+    def visit(self, func: VisitCallback) -> Optional[CallbackResult]:
         # returns value returned from callback
         ...
 
     def create_dataset(self, path, *args, **kwargs) -> H5DatasetLike:
         # returns original passed-in data
         ...
 
@@ -137,16 +134,21 @@
     def move(self, source: str, dest: str) -> None:
         ...
 
     def copy(self, source, dest, **kwargs) -> None:
         ...
 
 
+OpenMode = Literal["r", "r+", "a", "w", "w-", "x"]
+"""User open modes that can be passed during initialization."""
+_OPEN_MODES = list(get_args(OpenMode))
+
+
 @runtime_checkable
-class H5FileLike(H5GroupLike, Protocol):
+class H5FileLike(H5GroupLike, Protocol):  # pragma: no cover
     """A HDF5 File acts like the root group and has some extra features."""
 
     @property
     def mode(self) -> Literal["r", "r+"]:
         """Return 'r' if container is immutable, otherwise 'r+'."""
 
     def close(self) -> None:
```

### Comparing `metador_core-0.0.2/metador_core/container/utils.py` & `metador_core-0.1.0/src/metador_core/container/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-Constants and helper functions.
+"""Constants and helper functions.
 
 Provides syntactic path transformations to implement the Metador container layout.
 """
 
 from typing_extensions import Final
 
 METADOR_SPEC_VERSION: Final[str] = "1.0"
```

### Comparing `metador_core-0.0.2/metador_core/container/wrappers.py` & `metador_core-0.1.0/src/metador_core/container/wrappers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,90 +1,111 @@
 from __future__ import annotations
 
 from itertools import takewhile
 from typing import Any, Dict, MutableMapping, Optional, Set, Type, Union
 
 import h5py
 import wrapt
-from typing_extensions import Final
 
-from ..ih5.overlay import H5Type, node_h5type
 from . import utils as M
 from .drivers import MetadorDriver, to_h5filelike
-from .interface import MetadorContainerTOC, MetadorMeta
-from .types import H5DatasetLike, H5FileLike, H5GroupLike, H5NodeLike, OpenMode
-
-RO_FLAG: Final[str] = "read_only"
-LO_FLAG: Final[str] = "local_only"
-SO_FLAG: Final[str] = "skel_only"
+from .interface import MetadorContainerTOC, MetadorMeta, NodeAcl, NodeAclFlags
+from .protocols import H5DatasetLike, H5FileLike, H5GroupLike, H5NodeLike, OpenMode
 
 
 class UnsupportedOperationError(AttributeError):
     """Subclass to distinguish between actually missing attribute and unsupported one."""
 
 
 class WrappedAttributeManager(wrapt.ObjectProxy):
     """Wrapper for AttributeManager-like objects to prevent mutation (read-only) or inspection (skel-only)."""
 
     __wrapped__: MutableMapping
 
-    _self_ro: bool
-    _self_so: bool
+    _self_acl: NodeAclFlags
+    _self_acl_whitelist: Dict[NodeAcl, Set[str]] = {
+        NodeAcl.skel_only: {"keys"},
+        NodeAcl.read_only: {"keys", "values", "items", "get"},
+    }
     _self_allowed: Set[str]
 
-    def __init__(self, obj, **kwargs):
+    def __init__(self, obj, acl: NodeAclFlags):
         super().__init__(obj)
+        # initialize whitelist based on passed ACL flags
+        self._self_acl = acl
+        allowed: Optional[Set[str]] = None
+        for flag, value in acl.items():
+            if not value or flag not in self._self_acl_whitelist:
+                continue
+            if allowed is None:
+                allowed = self._self_acl_whitelist[flag]
+            else:
+                allowed = allowed.intersection(self._self_acl_whitelist[flag])
+        self._self_allowed = allowed or set()
 
-        self._self_ro = kwargs.get(RO_FLAG, False)
-        self._self_so = kwargs.get(SO_FLAG, False)
-        if self._self_so:
-            self._self_allowed = {"keys"}
-        elif self._self_ro:
-            self._self_allowed = {"keys", "values", "items", "get"}
-        else:
-            self._self_allowed = set()  # this means everything is allowed
-
-    def _raise_illegal_op(self, flag: str):
+    def _raise_illegal_op(self, flag_info: str):
         raise UnsupportedOperationError(
-            f"This attribute set belongs to a node marked as {flag}!"
+            f"This attribute set belongs to a node marked as {flag_info}!"
         )
 
     def __getattr__(self, key: str):
-        # NOTE: this will not restrict __contains__ because its a special method, which is desired behavior.
+        # NOTE: this will not restrict __contains__ because its a special method
+        # (which is desired behavior).
         if (
             hasattr(self.__wrapped__, key)
             and self._self_allowed
             and key not in self._self_allowed
         ):
-            msg = f"{RO_FLAG}={self._self_ro} and {SO_FLAG}={self._self_so}"
-            self._raise_illegal_op(msg)
+            self._raise_illegal_op(str(self._self_acl))
         return getattr(self.__wrapped__, key)
 
     # this is not intercepted by getattr
     def __getitem__(self, key: str):
-        if self._self_so:
-            self._raise_illegal_op(SO_FLAG)
+        if self._self_acl[NodeAcl.skel_only]:
+            self._raise_illegal_op(NodeAcl.skel_only.name)
         return self.__wrapped__.__getitem__(key)
 
     # this is not intercepted by getattr
     def __setitem__(self, key: str, value):
-        if self._self_ro:
-            self._raise_illegal_op(RO_FLAG)
+        if self._self_acl[NodeAcl.read_only]:
+            self._raise_illegal_op(NodeAcl.read_only.name)
         return self.__wrapped__.__setitem__(key, value)
 
     # this is not intercepted by getattr
     def __delitem__(self, key: str):
-        if self._self_ro:
-            self._raise_illegal_op(RO_FLAG)
+        if self._self_acl[NodeAcl.read_only]:
+            self._raise_illegal_op(NodeAcl.read_only.name)
         return self.__wrapped__.__delitem__(key)
 
     def __repr__(self) -> str:
         return repr(self.__wrapped__)
 
 
+class WithDefaultQueryStartNode(wrapt.ObjectProxy):
+    """Cosmetic wrapper to search metadata below a H5LikeGroup.
+
+    Used to make sure that:
+        `group.metador.query(...)`
+    is equivalent to:
+        `container.metador.query(..., node=group)`
+
+    (without it, the default node will be the root "/" if not specified).
+    """
+
+    __wrapped__: MetadorContainerTOC
+
+    def __init__(self, obj: MetadorContainerTOC, def_start_node):
+        super().__init__(obj)
+        self._self_query_start_node = def_start_node
+
+    def query(self, schema, version=None, *, node=None):
+        node = node or self._self_query_start_node
+        return self.__wrapped__.query(schema, version, node=node)
+
+
 class MetadorNode(wrapt.ObjectProxy):
     """Wrapper for h5py and IH5 Groups and Datasets providing Metador-specific features.
 
     In addition to the Metadata management, also provides helpers to reduce possible
     mistakes in implementing interfaces by allowing to mark nodes as
 
     * read_only (regardless of the writability of the underlying opened container) and
@@ -92,112 +113,85 @@
 
     Note that these are "soft" restrictions to prevent errors and can be bypassed.
     """
 
     __wrapped__: H5NodeLike
 
     @staticmethod
-    def _parse_access_flags(kwargs):
-        # NOTE: mutating, removes keys that are inspected!
-        return {
-            LO_FLAG: kwargs.pop(LO_FLAG, False),
-            RO_FLAG: kwargs.pop(RO_FLAG, False),
-            SO_FLAG: kwargs.pop(SO_FLAG, False),
-        }
+    def _parse_access_flags(kwargs) -> NodeAclFlags:
+        # NOTE: mutating kwargs, removes keys that are inspected!
+        return {flag: kwargs.pop(flag.name, False) for flag in iter(NodeAcl)}
 
     def __init__(self, mc: MetadorContainer, node: H5NodeLike, **kwargs):
         flags = self._parse_access_flags(kwargs)
         lp = kwargs.pop("local_parent", None)
         if kwargs:
             raise ValueError(f"Unknown keyword arguments: {kwargs}")
 
         super().__init__(node)
         self._self_container: MetadorContainer = mc
 
-        self._self_flags: Dict[str, bool] = flags
+        self._self_flags: NodeAclFlags = flags
         self._self_local_parent: Optional[MetadorGroup] = lp
 
     def _child_node_kwargs(self):
         """Return kwargs to be passed to a child node.
 
         Ensures that {read,skel,local}_only status is passed down correctly.
         """
-        return {"local_parent": self if self.local_only else None, **self._self_flags}
+        return {
+            "local_parent": self if self.acl[NodeAcl.local_only] else None,
+            **{k.name: v for k, v in self.acl.items() if v},
+        }
 
     def restrict(self, **kwargs) -> MetadorNode:
         """Restrict this object to be local_only or read_only.
 
         Pass local_only=True and/or read_only=True to enable the restriction.
 
         local_only means that the node may not access the parent or file objects.
         read_only means that mutable actions cannot be done (even if container is mutable).
         """
-        # can only set, but not unset! (unless doing it on purpose with the attributes)
         added_flags = self._parse_access_flags(kwargs)
+        if added_flags[NodeAcl.local_only]:
+            # was set as local explicitly for this node ->
+            self._self_local_parent = None  # remove its ability to go up
+
+        # can only set, but not unset!
+        self._self_flags.update({k: True for k, v in added_flags.items() if v})
         if kwargs:
             raise ValueError(f"Unknown keyword arguments: {kwargs}")
 
-        self._self_flags.update(added_flags)
-        if added_flags[LO_FLAG]:  # was set as local explicitly ->
-            self._self_local_parent = None  # remove its ability to go up
         return self
 
     @property
-    def local_only(self) -> bool:
-        """Return whether this node is local-only.
-
-        If True, it is not possible to access parents beyond the initial local node.
-        If this is a Group, will inherit this status to children.
-        """
-        return self._self_flags[LO_FLAG]
-
-    @property
-    def read_only(self) -> bool:
-        """Return whether this node is read-only.
-
-        If True, no mutating methods should be called and will be prevented if possible.
-        If this is a Group, will inherit this status to children.
-        """
-        return self._self_flags[RO_FLAG]
-
-    @property
-    def skel_only(self) -> bool:
-        """Return whether this node is skel-only.
-
-        If True, then attributes, datasets and metadata cannot be retrieved, only listed.
-        If this is a Group, will inherit this status to children.
-        """
-        return self._self_flags[SO_FLAG]
+    def acl(self) -> Dict[NodeAcl, bool]:
+        """Return ACL flags of current node."""
+        return dict(self._self_flags)
 
     def _guard_path(self, path: str):
         if M.is_internal_path(path):
             msg = f"Trying to use a Metador-internal path: '{path}'"
             raise ValueError(msg)
-        if self.local_only and path[0] == "/":
+        if self.acl[NodeAcl.local_only] and path[0] == "/":
             msg = f"Node is marked as local_only, cannot use absolute path '{path}'!"
             raise ValueError(msg)
 
-    def _guard_read_only(self, method: str = "this method"):
-        if self.read_only:
-            msg = f"Cannot use {method}, the node is marked as read_only!"
-            raise UnsupportedOperationError(msg)
-
-    def _guard_skel_only(self, method: str = "this method"):
-        if self.skel_only:
-            msg = f"Cannot use {method}, the node is marked as skel_only!"
+    def _guard_acl(self, flag: NodeAcl, method: str = "this method"):
+        if self.acl[flag]:
+            msg = f"Cannot use {method}, the node is marked as {flag.name}!"
             raise UnsupportedOperationError(msg)
 
     # helpers
 
     def _wrap_if_node(self, val):
         """Wrap value into a metador node wrapper, if it is a suitable group or dataset."""
-        ntype = node_h5type(val)
-        if ntype == H5Type.group:
+        if isinstance(val, H5GroupLike):
             return MetadorGroup(self._self_container, val, **self._child_node_kwargs())
-        elif ntype == H5Type.dataset:
+        elif isinstance(val, H5DatasetLike):
             return MetadorDataset(
                 self._self_container, val, **self._child_node_kwargs()
             )
         else:
             return val
 
     def _destroy_meta(self, _unlink: bool = True):
@@ -226,83 +220,78 @@
     def meta(self) -> MetadorMeta:
         """Access the interface to metadata attached to this node."""
         return MetadorMeta(self)
 
     @property
     def metador(self) -> MetadorContainerTOC:
         """Access the info about the container this node belongs to."""
-        return self._self_container.metador
+        return WithDefaultQueryStartNode(self._self_container.metador, self)
 
     # wrap existing methods as needed
 
     @property
     def name(self) -> str:
         return self.__wrapped__.name  # just for type checker not to complain
 
     @property
     def attrs(self):
-        if self.read_only or self.skel_only:
-            return WrappedAttributeManager(
-                self.__wrapped__.attrs,
-                **{
-                    RO_FLAG: self.read_only,
-                    SO_FLAG: self.skel_only,
-                },
-            )
+        if self.acl[NodeAcl.read_only] or self.acl[NodeAcl.skel_only]:
+            return WrappedAttributeManager(self.__wrapped__.attrs, self.acl)
         return self.__wrapped__.attrs
 
     @property
     def parent(self) -> MetadorGroup:
-        if self.local_only:
+        if self.acl[NodeAcl.local_only]:
             # allow child nodes of local-only nodes to go up to the marked parent
             # (or it is None, if this is the local root)
-            # see https://github.com/GrahamDumpleton/wrapt/issues/215
-            return self._self_local_parent
+            if lp := self._self_local_parent:
+                return lp
+            else:
+                # raise exception (illegal non-local access)
+                self._guard_acl(NodeAcl.local_only, "parent")
 
         return MetadorGroup(
             self._self_container,
             self.__wrapped__.parent,
             **self._child_node_kwargs(),
         )
 
     @property
     def file(self) -> MetadorContainer:
-        if self.local_only:
-            # see https://github.com/GrahamDumpleton/wrapt/issues/215
-            return None  # type: ignore
+        if self.acl[NodeAcl.local_only]:
+            # raise exception (illegal non-local access)
+            self._guard_acl(NodeAcl.local_only, "parent")
         return self._self_container
 
 
 class MetadorDataset(MetadorNode):
     """Metador wrapper for a HDF5 Dataset."""
 
     __wrapped__: H5DatasetLike
 
     # manually assembled from public methods which h5py.Dataset provides
     _self_RO_FORBIDDEN = {"resize", "make_scale", "write_direct", "flush"}
 
     def __getattr__(self, key):
-        if self.read_only and key in self._self_RO_FORBIDDEN:
-            self._guard_read_only(key)
-        if self.skel_only and key == "get":
-            self._guard_skel_only(key)
+        if self.acl[NodeAcl.read_only] and key in self._self_RO_FORBIDDEN:
+            self._guard_acl(NodeAcl.read_only, key)
+        if self.acl[NodeAcl.skel_only] and key == "get":
+            self._guard_acl(NodeAcl.skel_only, key)
 
         return getattr(self.__wrapped__, key)
 
     # prevent getter of node if marked as skel_only
     def __getitem__(self, *args, **kwargs):
-        self._guard_skel_only("__getitem__")
-
+        self._guard_acl(NodeAcl.skel_only, "__getitem__")
         return self.__wrapped__.__getitem__(*args, **kwargs)
 
     # prevent mutating method calls of node is marked as read_only
 
     def __setitem__(self, *args, **kwargs):
-        self._guard_read_only("__setitem__")
-
+        self._guard_acl(NodeAcl.read_only, "__setitem__")
         return self.__wrapped__.__setitem__(*args, **kwargs)
 
 
 # TODO: can this be done somehow with wrapt.decorator but still without boilerplate?
 # problem is it wants a function, but we need to look it up by name first
 # so we hand-roll the decorator for now.
 def _wrap_method(method: str, is_read_only_method: bool = False):
@@ -314,15 +303,15 @@
     If is_read_only=False and the object is read_only, refuses to call the method.
     """
 
     def wrapped_method(obj, name, *args, **kwargs):
         # obj will be the self of the wrapper instance
         obj._guard_path(name)
         if not is_read_only_method:
-            obj._guard_read_only(method)
+            obj._guard_acl(NodeAcl.read_only, method)
         ret = getattr(obj.__wrapped__, method)(name, *args, **kwargs)  # RAW
         return obj._wrap_if_node(ret)
 
     return wrapped_method
 
 
 # classes of h5py reference-like types (we don't support that)
@@ -376,19 +365,21 @@
 
         return self.visititems(wrapped_func)
 
     # following also depend on the filtered sequence, directly
     # filter the items, derive other related functions based on that
 
     def items(self):
-        return (
-            (k, self._wrap_if_node(v))
-            for k, v in self.__wrapped__.items()  # RAW
-            if not M.is_internal_path(v.name)
-        )
+        for k, v in self.__wrapped__.items():
+            if v is None:
+                # NOTE: e.g. when nodes are deleted/moved during iteration,
+                # v can suddenly be None -> we need to catch this case!
+                continue
+            if not M.is_internal_path(v.name):
+                yield (k, self._wrap_if_node(v))
 
     def values(self):
         return map(lambda x: x[1], self.items())
 
     def keys(self):
         return map(lambda x: x[0], self.items())
 
@@ -410,25 +401,25 @@
             if nxt := self.get(segs[0]):
                 return "/".join(segs[1:]) in nxt
             return False
 
     # these we can take care of but are a bit more tricky to think through
 
     def __delitem__(self, name: str):
-        self._guard_read_only("__delitem__")
+        self._guard_acl(NodeAcl.read_only, "__delitem__")
         self._guard_path(name)
 
         node = self[name]
         # clean up metadata (recursively, if a group)
         node._destroy_meta()
         # kill the actual data
         return _wrap_method("__delitem__")(self, name)
 
     def move(self, source: str, dest: str):
-        self._guard_read_only("move")
+        self._guard_acl(NodeAcl.read_only, "move")
         self._guard_path(source)
         self._guard_path(dest)
 
         src_metadir = self[source].meta._base_dir
         # if actual data move fails, an exception will prevent the rest
         self.__wrapped__.move(source, dest)  # RAW
 
@@ -453,15 +444,15 @@
 
     def copy(
         self,
         source: Union[str, MetadorGroup, MetadorDataset],
         dest: Union[str, MetadorGroup],
         **kwargs,
     ):
-        self._guard_read_only("copy")
+        self._guard_acl(NodeAcl.read_only, "copy")
 
         # get source node and its name without the path and its type
         src_node: MetadorNode
         if isinstance(source, str):
             self._guard_path(source)
             src_node = self[source]
         elif isinstance(source, MetadorNode):
@@ -498,23 +489,25 @@
             "expand_refs": True,
             "without_attrs": without_attrs,
         }
         self.__wrapped__.copy(source, dst_path, **copy_kwargs)  # RAW
         dst_node = self[dst_path]  # exists now
 
         if src_is_dataset and not without_meta:
-            # because metadata lives in parallel group, need to copy separately
+            # because metadata lives in parallel group, need to copy separately:
             src_meta: str = src_node.meta._base_dir
-            dst_meta: str = dst_node.meta._base_dir  # will not exist yet
+            dst_meta: str = dst_node.meta._base_dir  # node will not exist yet
             self.__wrapped__.copy(src_meta, dst_meta, **copy_kwargs)  # RAW
-            # register in TOC
+
+            # register in TOC:
             dst_meta_node = self.__wrapped__[dst_meta]
             assert isinstance(dst_meta_node, H5GroupLike)
             missing = self._self_container.metador._links.find_missing(dst_meta_node)
             self._self_container.metador._links.repair_missing(missing)
+
         if not src_is_dataset:
             if without_meta:
                 # need to destroy copied metadata copied with the source group
                 # but keep TOC links (they point to original copy!)
                 dst_node._destroy_meta(_unlink=False)
             else:
                 # register copied metadata objects under new uuids
@@ -556,19 +549,26 @@
     def metador(self) -> MetadorContainerTOC:
         """Access interface to Metador metadata object index."""
         return self._self_toc
 
     def __init__(
         self,
         name_or_obj: Union[MetadorDriver, Any],
-        mode: OpenMode = "r",
+        mode: Optional[OpenMode] = "r",
         *,
         # NOTE: driver takes class instead of enum to also allow subclasses
         driver: Optional[Type[MetadorDriver]] = None,
     ):
+        """Initialize a MetadorContainer instance from file(s) or a supported object.
+
+        The `mode` argument is ignored when simply wrapping an object.
+
+        If a data source such as a path is passed, will instantiate the object first,
+        using the default H5File driver or the passed `driver` keyword argument.
+        """
         # wrap the h5file-like object (will set self.__wrapped__)
         super().__init__(self, to_h5filelike(name_or_obj, mode, driver=driver))
         # initialize metador-specific stuff
         self._self_toc = MetadorContainerTOC(self)
 
     # not clear if we want these in the public interface. keep this private for now:
```

### Comparing `metador_core-0.0.2/metador_core/harvester/__init__.py` & `metador_core-0.1.0/src/metador_core/harvester/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Plugin group for metadata harvesters."""
 from __future__ import annotations
 
 from abc import ABC, ABCMeta, abstractmethod
 from pathlib import Path
 from typing import (
     TYPE_CHECKING,
+    Any,
     Callable,
     ClassVar,
     Dict,
     Iterable,
     Set,
     Type,
     TypeVar,
@@ -73,35 +74,32 @@
 class Harvester(ABC, metaclass=HarvesterMeta):
     """Base class for metadata harvesters.
 
     A harvester is a class that can be instantiated to extract
     metadata according to some schema plugin (the returned schema
     must be defined as the `Plugin.returns` attribute)
 
-    Override the inner `Args` class with a subclass to add arguments.
+    Override the inner `Harvester.Args` class with a subclass to add arguments.
     This works exactly like schema definition and is simply
     another pydantic model, so you can use both field and root
     validators to check whether the arguments are making sense.
 
     If all you need is getting a file path, consider using
     `FileHarvester`, which already defines a `filepath` argument.
 
     Override the `run()` method to implement the metadata harvesting
     based on a validated configuration located at `self.args`.
     """
 
     Plugin: ClassVar[HarvesterPlugin]
 
-    if TYPE_CHECKING:
-        Args: TypeAlias = HarvesterArgs
-    else:
-        Args = HarvesterArgs
-        """Arguments to be passed to the harvester."""
+    Args: TypeAlias = HarvesterArgs
+    """Arguments to be passed to the harvester."""
 
-    args: Union[Args, HarvesterArgsPartial]
+    args: Union[Harvester.Args, HarvesterArgsPartial]
 
     @property
     def schema(self):
         """Partial schema class returned by this harvester.
 
         Provided for implementation convenience.
         """
@@ -136,15 +134,15 @@
             raise ValueError(msg)
         return self.run()
 
     # ----
     # to be overridden
 
     @abstractmethod
-    def run(self):
+    def run(self) -> MetadataSchema:
         """Do the harvesting according to instance configuration and return metadata.
 
         Override this method with your custom metadata harvesting logic, based
         on configuration provided in `self.args`.
 
         All actual, possibly time-intensive harvesting computations (accessing
         resources, running external code, etc.) MUST be performed in this method.
@@ -155,15 +153,14 @@
         ensure that these are managed, fresh and cleaned up when you are done
         (e.g. if you need to run external processes that dump outputs to a
         file).
 
         Returns:
             A fresh instance of type `self.schema` containing harvested metadata.
         """
-        raise NotImplementedError
 
 
 class FileHarvester(Harvester):
     """Harvester for processing a single file path.
 
     The file path is not provided or set during __init__,
     but instead is passed during harvest_file.
@@ -337,28 +334,29 @@
     """Given a sequence of harvesters, configure them all at once.
 
     Can be used to set the same parameter in all of them easily.
     """
     return (h(**kwargs) for h in harvesters)
 
 
-def file_harvester_pipeline(*args: Union[FileHarvester, Type[FileHarvester]]):
+def file_harvester_pipeline(
+    *hvs: Union[FileHarvester, Type[FileHarvester]]
+) -> Callable[[Path], Any]:
     """Generate a harvesting pipeline for a file.
 
     Args:
-        FileHarvester classes or pre-configured instances to use.
-
-        The passed objects must be preconfigured as needed,
-        except for fixing a filepath (it will be overwritten).
+        hvs: FileHarvester classes or pre-configured instances to use.
+            The passed objects must be preconfigured as needed,
+            except for fixing a filepath (it will be overwritten).
 
     Returns:
         Function that takes a file path and will return
         the harvesters configured for the passed path.
     """
-    return lambda path: configure(*args, filepath=path)
+    return lambda path: configure(*hvs, filepath=path)
 
 
 def harvest(
     schema: Type[S],
     sources: Iterable[Union[Path, Harvester]],
     *,
     ignore_invalid: bool = False,
```

### Comparing `metador_core-0.0.2/metador_core/harvester/common.py` & `metador_core-0.1.0/src/metador_core/harvester/common.py`

 * *Files identical despite different names*

### Comparing `metador_core-0.0.2/metador_core/ih5/PATCH_THEORY.md` & `metador_core-0.1.0/src/metador_core/ih5/PATCH_THEORY.md`

 * *Files identical despite different names*

### Comparing `metador_core-0.0.2/metador_core/ih5/__init__.py` & `metador_core-0.1.0/src/metador_core/ih5/__init__.py`

 * *Files identical despite different names*

### Comparing `metador_core-0.0.2/metador_core/ih5/manifest.py` & `metador_core-0.1.0/src/metador_core/ih5/manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,18 @@
     user_block: IH5UserBlock  # copy of user block (without the manifest extension part)
 
     skeleton: IH5Skeleton  # computed with IH5Skeleton, used to create a stub
 
     manifest_exts: Dict[str, Any]  # Arbitrary extensions, similar to IH5UserBlock
 
     @classmethod
-    def from_userblock(cls, ub: IH5UserBlock, skeleton={}, exts={}) -> IH5Manifest:
+    def from_userblock(cls, ub: IH5UserBlock, skeleton=None, exts=None) -> IH5Manifest:
         """Create a manifest file based on a user block."""
+        skeleton = skeleton or {}
+        exts = exts or {}
         ub_copy = ub.copy()
         # only keep other extensions (otherwise its circular)
         ub_copy.ub_exts = {
             k: v for k, v in ub.ub_exts.items() if k != IH5UBExtManifest.ext_name()
         }
         return cls(
             manifest_uuid=uuid1(),
```

### Comparing `metador_core-0.0.2/metador_core/ih5/overlay.py` & `metador_core-0.1.0/src/metador_core/ih5/overlay.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-r"""
-Overlay wrappers to access a virtual record consisting of a base container + patches.
+"""Overlay wrappers to access a virtual record consisting of a base container + patches.
 
 The wrappers take care of dispatching requests to records,
 groups and attributes to the correct path.
 """
 from __future__ import annotations
 
 import re
@@ -15,20 +14,24 @@
     Callable,
     Dict,
     List,
     Optional,
     Type,
     TypeVar,
     Union,
+    cast,
 )
 
 import h5py
 import numpy as np
 
+from ..container.protocols import H5DatasetLike
+
 if TYPE_CHECKING:
+    from ..container.protocols import H5GroupLike
     from .record import IH5Record
 else:
     IH5Record = Any
 
 
 # dataset value marking a deleted group, dataset or attribute
 DEL_VALUE = np.void(b"\x7f")  # ASCII DELETE
@@ -79,15 +82,15 @@
     this node will not consider containers with smaller index than that.
     """
 
     def __post_init__(self):
         """Instantiate an overlay node."""
         if not self._gpath or self._gpath[0] != "/":
             raise ValueError("Path must be absolute!")
-        if not (0 <= self._cidx):
+        if self._cidx < 0:
             raise ValueError("Creation index must be non-negative!")
 
     @property
     def _files(self) -> List[h5py.File]:
         return self._record.__files__
 
     def __hash__(self):
@@ -95,15 +98,15 @@
 
         Two nodes are equivalent if they are linked to the same
         open record and address the same entity.
         """
         return hash((id(self._record), self._gpath, self._cidx))
 
     def __bool__(self) -> bool:
-        return bool(self._files) and bool(all(map(bool, self._files)))
+        return bool(self._files) and all(map(bool, self._files))
 
     @property
     def _last_idx(self):
         """Index of the latest container."""
         return len(self._files) - 1
 
     @property
@@ -193,15 +196,15 @@
 
     @property
     def _is_attrs(self) -> bool:
         return self.__is_attrs__
 
     def __init__(
         self,
-        record,  # IH5Record
+        record: IH5Record,
         gpath: str,
         creation_idx: int,
         attrs: bool = False,
     ):
         """See `IH5Node` constructor.
 
         This variant represents an "overlay container", of which there are two types -
@@ -260,15 +263,15 @@
         for i in reversed(range(self._cidx, len(self._files))):
             if self._gpath not in self._files[i]:
                 continue
 
             obj = self._files[i][self._gpath]
             if self._is_attrs:
                 obj = obj.attrs
-            assert isinstance(obj, h5py.Group) or isinstance(obj, h5py.AttributeManager)
+            assert isinstance(obj, (h5py.Group, h5py.AttributeManager))
 
             # keep most recent version of child node / attribute
             for k in obj.keys():
                 if k not in children:
                     is_virtual[k] = _node_is_virtual(self._get_child_raw(k, i))
                     children[k] = i
                 elif is_virtual[k]:  # .. and k in children!
@@ -277,15 +280,15 @@
 
         # return resulting child nodes / attributes (without the deleted ones)
         # in alphabetical order,
         # in case of attributes, also excludes special SUBST marker attribute
         return {
             k: idx
             for k, idx in sorted(children.items(), key=lambda x: x[0])
-            if (not self._is_attrs or not k == SUBST_KEY)
+            if (not self._is_attrs or k != SUBST_KEY)
             and not _node_is_del_mark(self._get_child_raw(k, idx))
         }
 
     def _get_children(self) -> List[Any]:
         """Get alphabetically ordered list of child nodes."""
         return [
             self._get_child(self._abs_path(k), idx)
@@ -403,26 +406,31 @@
 
     # h5py-like interface
     @property
     def name(self) -> str:
         return self._gpath
 
     @property
-    def file(self):  # -> IH5Record
+    def file(self) -> IH5Record:
         return self._record
 
     @property
     def parent(self) -> IH5Group:
         return self._record[self._parent_path()]
 
     @property
-    def attrs(self):
+    def attrs(self) -> IH5AttributeManager:
         self._guard_open()
         return IH5AttributeManager(self._record, self._gpath, self._cidx)
 
+    # this one is also needed to work with H5DatasetLike
+    @property
+    def ndim(self) -> int:
+        return self._files[self._cidx][self._gpath].ndim  # type: ignore
+
     # for a dataset, instead of paths the numpy data is indexed. at this level
     # the patching mechanism ends, so it's just passing through to h5py
 
     def __getitem__(self, key):
         # just pass through dataset indexing to underlying dataset
         self._guard_open()
         return self._files[self._cidx][self._gpath][key]  # type: ignore
@@ -572,23 +580,22 @@
         self, path: str, shape=None, dtype=None, data=None, **kwargs
     ) -> IH5Dataset:
         self._guard_open()
         self._guard_read_only()
         self._guard_key(path)
         self._guard_value(data)
 
-        unknown_kwargs = set(kwargs.keys()) - set(["compression", "compression_opts"])
-        if unknown_kwargs:
+        if unknown_kwargs := set(kwargs.keys()) - {"compression", "compression_opts"}:
             raise ValueError(f"Unkown kwargs: {unknown_kwargs}")
 
         path = self._abs_path(path)
         fidx = self._find(path)
         if fidx is not None:
             prev_val = self._get_child(path, fidx)
-            if isinstance(prev_val, IH5Group) or isinstance(prev_val, IH5Dataset):
+            if isinstance(prev_val, (IH5Group, IH5Dataset)):
                 raise ValueError("Path exists, in order to replace - delete first!")
 
         if path in self._files[-1] and _node_is_del_mark(
             self._get_child_raw(path, self._last_idx)
         ):
             # remove deletion marker in latest patch, if set
             del self._files[-1][path]
@@ -621,17 +628,20 @@
         if isinstance(dest, str):
             # if dest is a path, ignore inferred/passed name
             segs = self._abs_path(dest).split("/")
             dst_group = self.require_group("/".join(segs[:-1]) or "/")
             dst_name = segs[-1]
         else:
             # given dest is a group node, use inferred/passed name
-            dst_group = dest
+
+            dst_group = dest if dest.name != "/" else dest["/"]  # *
+            # * ugly workaround for treating files as groups in the copy method
+
             dst_name = name
-        return h5_copy_from_to(src_node, dst_group, dst_name, **kwargs)
+        return h5_copy_from_to(src_node, cast(Any, dst_group), dst_name, **kwargs)
 
     def move(self, source: str, dest: str):
         self.copy(source, dest)
         del self[source]
 
     def visititems(self, func: Callable[[str, object], Optional[Any]]) -> Any:
         self._guard_open()
@@ -673,32 +683,20 @@
     attribute_set = "attribute-set"  # = not further nested, dict-like
     attribute = "attribute"  # = unwrapped data
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}.{self.value}"
 
 
-_h5types = {
-    # normal h5py files
-    h5py.Group: H5Type.group,
-    h5py.Dataset: H5Type.dataset,
-    h5py.AttributeManager: H5Type.attribute_set,
-    # IH5 datasets
-    IH5Group: H5Type.group,
-    IH5Dataset: H5Type.dataset,
-    IH5AttributeManager: H5Type.attribute_set,
-}
-
-
-def node_h5type(node):
-    """Return whether node is Group, Dataset or AttributeManager (or None)."""
-    return _h5types.get(type(node))
-
-
-def h5_copy_from_to(source_node, target_group, target_path: str, **kwargs):
+def h5_copy_from_to(
+    source_node: Union[H5DatasetLike, H5GroupLike],
+    target_group: H5GroupLike,
+    target_path: str,
+    **kwargs,
+):
     """Copy a dataset or group from one container to a fresh location.
 
     This works also between HDF5 and IH5.
 
     Source node must be group or dataset object.
     Target node must be an existing group object.
     Target path must be fresh path relative to target node.
@@ -707,45 +705,38 @@
     shallow: bool = kwargs.pop("shallow", False)
     for arg in ["expand_soft", "expand_external", "expand_refs"]:
         if not kwargs.pop(arg, True):
             raise ValueError("IH5 does not support keeping references!")
     if kwargs:
         raise ValueError(f"Unknown keyword arguments: {kwargs}")
 
-    src_type = node_h5type(source_node)
-    if src_type is None or src_type == H5Type.attribute_set:
-        raise ValueError("Can only copy from a group or dataset!")
-    if node_h5type(target_group) != H5Type.group:
-        raise ValueError("Copy target must be a group!")
-
     if not target_path or target_path[0] == "/":
         raise ValueError("Target path must be non-empty and relative!")
     if target_path in target_group:
         raise ValueError(f"Target path {target_path} already exists in target group!")
 
     def copy_attrs(src_node, trg_node):
         if not without_attrs:
             trg_atrs = trg_node.attrs
             for k, v in src_node.attrs.items():
                 trg_atrs[k] = v
 
-    if src_type == H5Type.dataset:
+    if isinstance(source_node, H5DatasetLike):
         node = target_group.create_dataset(target_path, data=source_node[()])
         copy_attrs(source_node, node)  # copy dataset attributes
     else:
         trg_root = target_group.create_group(target_path)
         copy_attrs(source_node, trg_root)  # copy source node attributes
 
         def copy_children(name, src_child):
             # name is relative to source root -> can use it
-            ntype = node_h5type(src_child)
-            if ntype == H5Type.group:
-                trg_root.create_group(name)
-            elif ntype == H5Type.dataset:
+            if isinstance(src_child, H5DatasetLike):
                 trg_root[name] = src_child[()]
+            else:  # must be grouplike
+                trg_root.create_group(name)
             copy_attrs(src_child, trg_root[name])
 
         if shallow:  # only immediate children
             for name, src_child in source_node.items():
                 copy_children(name, src_child)
         else:  # recursive copy
             source_node.visititems(copy_children)
```

### Comparing `metador_core-0.0.2/metador_core/ih5/record.py` & `metador_core-0.1.0/src/metador_core/ih5/record.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-Immutable HDF5 container records.
+"""Immutable HDF5 container records.
 
 A record consists of a base container and a number of patch containers.
 This allows a record to work in settings where files are immutable, but still
 provide a structured way of updating data stored inside.
 
 Both base containers and patches are HDF5 files that are linked together
 by some special attributes in the container root.
@@ -13,21 +12,22 @@
 * transparent access to data in the record (possibly spanning multiple files)
 """
 from __future__ import annotations
 
 import json
 import re
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Tuple, Type, TypeVar, Union, get_args
+from typing import Any, Dict, List, Literal, Optional, Tuple, Type, TypeVar, Union
 from uuid import UUID, uuid1
 
 import h5py
 from pydantic import BaseModel, Field, PrivateAttr
-from typing_extensions import Annotated, Final, Literal
+from typing_extensions import Annotated, Final
 
+from ..container.protocols import _OPEN_MODES, OpenMode
 from ..schema.types import QualHashsumStr
 from ..util.hashsums import qualified_hashsum
 from .overlay import IH5Group, h5_copy_from_to
 
 # the magic string we use to identify a valid container
 FORMAT_MAGIC_STR: Final[str] = "ih5_v01"
 """Magic value at the beginning of the file to detect that an HDF5 file is valid IH5."""
@@ -146,23 +146,16 @@
             if check == b"\x89HDF":
                 raise ValueError(f"{filename}: no user block reserved, can't write!")
             f.seek(0)
             f.write(data)
             f.write(b"\x00")  # mark end of the data
 
 
-OpenMode = Literal["r", "r+", "a", "w", "w-", "x"]
-"""User open modes that can be passed during initialization."""
-
-_OPEN_MODES = list(get_args(OpenMode))
-
-
 class IH5Record(IH5Group):
-    """
-    Class representing a record, which consists of a collection of immutable files.
+    """Class representing a record, which consists of a collection of immutable files.
 
     One file is a base container (with no linked predecessor state),
     the remaining files are a linear sequence of patch containers.
 
     Runtime invariants to be upheld before/after each method call (after __init__):
 
     * all files of an instance are open for reading (until `close()` is called)
@@ -194,15 +187,17 @@
     def __new__(cls, *args, **kwargs):
         ret = super().__new__(cls)
         ret._allow_patching = True
         ret.__files__ = []
         return ret
 
     def __eq__(self, o) -> bool:
-        return self.__files__ == o.__files__
+        if not isinstance(o, IH5Group):
+            return False
+        return self._record._files == o._record._files
 
     @property
     def _has_writable(self):
         """Return True iff an uncommitted patch exists."""
         if not self.__files__:
             return False
         f = self.__files__[-1]
@@ -446,49 +441,59 @@
         if not dir.is_dir():
             raise ValueError(f"'{dir}' is not a directory")
 
         ret = []
         namepat = f"[{cls._ALLOWED_NAME_CHARS}]+(?=[^{cls._ALLOWED_NAME_CHARS}])"
         for p in dir.glob(f"*{cls._FILE_EXT}"):
             if m := re.match(namepat, p.name):
-                ret.append(m.group(0))
+                ret.append(m[0])
         return list(map(lambda name: dir / name, set(ret)))
 
-    def __init__(self, record: Union[str, Path], mode: OpenMode = "r", **kwargs):
+    def __init__(
+        self, record: Union[str, Path, List[Path]], mode: OpenMode = "r", **kwargs
+    ):
         """Open or create a record.
 
         This method uses `find_files` to infer the correct set of files syntactically.
 
         The open mode semantics are the same as for h5py.File.
 
         If the mode is 'r', then creating, committing or discarding patches is disabled.
 
         If the mode is 'a' or 'r+', then a new patch will be created in case the latest
         patch has already been committed.
         """
         super().__init__(self)
 
-        record = Path(record)
+        if isinstance(record, list):
+            if mode[0] == "w" or mode == "x":
+                raise ValueError("Pass a prefix path for creating or overwriting!")
+            paths = record
+        else:
+            paths = None
+            path: Path = Path(record)
+
         if mode not in _OPEN_MODES:
             raise ValueError(f"Unknown file open mode: {mode}")
 
         if mode[0] == "w" or mode == "x":
             # create new or overwrite to get new
-            ret = self._create(record, truncate=(mode == "w"))
+            ret = self._create(path, truncate=(mode == "w"))
             self.__dict__.update(ret.__dict__)
             return
 
         if mode == "a" or mode[0] == "r":
-            paths = self.find_files(record)
+            if not paths:  # user passed a path prefix -> find files
+                paths = self.find_files(path)  # type: ignore
 
-            if not paths:
+            if not paths:  # no files were found
                 if mode != "a":  # r/r+ need existing containers
-                    raise FileNotFoundError(f"No files found for record: {record}")
-                else:  # a means create new if not existing (will be writable)
-                    ret = self._create(record, truncate=False)
+                    raise FileNotFoundError(f"No files found for record: {path}")
+                else:  # 'a' means create new if not existing (will be writable)
+                    ret = self._create(path, truncate=False)
                     self.__dict__.update(ret.__dict__)
                     return
 
             # open existing (will be ro if everything is fine, writable if latest patch was uncommitted)
             want_rw = mode != "r"
             ret = self._open(paths, reopen_incomplete_patch=want_rw, **kwargs)
             self.__dict__.update(ret.__dict__)
@@ -592,15 +597,14 @@
 
         The passed userblock is a prepared userblock with updated HDF5 hashsum for the
         merged container and adapted prev_patch field, as will it be written to the file.
         Additional changes done to it in-place will be included.
 
         The passed filename can be used to perform additional necessary actions.
         """
-        pass
 
     def merge_files(self, target: Path) -> Path:
         """Given a path with a record name, merge current record into new container.
 
         Returns new resulting container.
         """
         self._expect_open()
```

### Comparing `metador_core-0.0.2/metador_core/ih5/skeleton.py` & `metador_core-0.1.0/src/metador_core/ih5/skeleton.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 
 A skeleton is documenting the tree structure of a HDF5-like container,
 ignoring the actual data content (attribute values and datasets).
 
 This can be used to implement manifest file and support "patching in thin air",
 i.e. without having the actual container.
 """
-from typing import Dict, Union
+from typing import Dict, Literal, Union
 
 import h5py
 from pydantic import BaseModel
-from typing_extensions import Literal
 
 from .overlay import H5Type, IH5Dataset, IH5Group
 from .record import IH5Record, IH5UserBlock
 
 
 class SkeletonNodeInfo(BaseModel):
     node_type: Literal[H5Type.group, H5Type.dataset]
```

### Comparing `metador_core-0.0.2/metador_core/packer/__init__.py` & `metador_core-0.1.0/src/metador_core/packer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """Definition of HDF5 packer plugin interface."""
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from io import UnsupportedOperation
 from pathlib import Path
-from typing import Tuple, Type
+from typing import Callable, Tuple, Type
 
 import wrapt
 from overrides import EnforceOverrides, overrides
 
-from metador_core.ih5.manifest import IH5MFRecord
-from metador_core.plugins import plugingroups
-
 from ..container import MetadorContainer
+from ..ih5.manifest import IH5MFRecord
 from ..plugin import interface as pg
+from ..plugins import plugingroups
 from ..schema.core import MetadataSchema
 from ..schema.plugins import PluginPkgMeta
 from ..util.diff import DirDiff
 from ..util.hashsums import DirHashsums, dir_hashsums
 from .types import DirValidationErrors
 
 
@@ -143,15 +142,15 @@
 
         The `diff` structure contains information about changed paths.
 
         If not implemented, updates will be created by clearing the provided
         container and using `pack` on it.
 
         Args:
-            container: Metador IH5 record to pack the data into or update
+            mc: Metador IH5 record to pack the data into or update
             data_dir: Directory containing all the data to be packed
             diff: Diff tree of dirs and files in data_dir compared to a previous state
         """
         # default fallback implementation using pack
         for obj in [mc, mc.attrs, mc.meta]:
             for key in obj.keys():
                 del obj[key]
@@ -166,15 +165,15 @@
 
         The `data_dir` is assumed to be suitable (according to `check_dir`).
 
         If not implemented, initial packing is done using `update`
         with an empty container and a diff containing all the files.
 
         Args:
-            container: Metador IH5 record to pack the data into or update
+            mc: Metador IH5 record to pack the data into or update
             data_dir: Directory containing all the data to be packed
         """
         # default fallback implementation using update
         return cls.update(mc, data_dir, DirDiff.compare({}, dir_hashsums(data_dir)))
 
 
 class PackerInfo(MetadataSchema):
@@ -259,15 +258,17 @@
         Raises an exception if packer is not found or `packer.check_dir` fails.
         """
         packer = self[pname]
         if errs := packer.check_dir(srcdir):
             raise errs
         return (packer, dir_hashsums(srcdir))
 
-    def pack(self, packer_name: str, data_dir: Path, target: Path, h5like_cls):
+    def pack(
+        self, packer_name: str, data_dir: Path, target: Path, h5like_cls: Callable
+    ):
         """Pack a directory into a container using an installed packer.
 
         `packer_name` must be an installed packer plugin.
 
         `data_dir` must be an existing directory suitable for the packer.
 
         `target` must be a non-existing path and will be passed into `h5like_cls` as-is.
```

### Comparing `metador_core-0.0.2/metador_core/packer/example.py` & `metador_core-0.1.0/src/metador_core/packer/example.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-This is an example packer plugin for simple general data types.
+"""This is an example packer plugin for simple general data types.
 
 A packer plugin implements use-case specific container-related
 functionality for Metador containers.
 
 To develop your own packer plugin, implement a class deriving from
 `Packer` and register the class as an entrypoint of your package
 (see the `pyproject.toml` of this package, where `GenericPacker`
@@ -117,15 +116,14 @@
             elif path.is_file():
                 if path.name.endswith(cls.META_SUFFIX):
                     if key == cls.META_SUFFIX:
                         # update root meta
                         print("CREATE:", path, "->", key, "(biblio metadata)")
                         mc.meta["common_biblio"] = BibMeta.parse_file(path)
                 else:
-
                     if path.name.lower().endswith(".csv"):
                         # embed CSV as numpy array with table metadata
                         print("CREATE:", path, "->", key, "(table)")
 
                         mc[key] = pandas.read_csv(path).to_numpy()  # type: ignore
                         mc[key].meta["common_table"] = TableMeta.for_file(
                             cls.sidecar_for(path)
```

### Comparing `metador_core-0.0.2/metador_core/packer/types.py` & `metador_core-0.1.0/src/metador_core/packer/types.py`

 * *Files identical despite different names*

### Comparing `metador_core-0.0.2/metador_core/packer/utils.py` & `metador_core-0.1.0/src/metador_core/packer/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,16 +61,16 @@
     metadata: Optional[MetadataSchema] = None,
 ) -> MetadorDataset:
     """Embed a file, adding minimal generic metadata to it.
 
     Will also ensure that the attached metadata has RO-Crate compatible @id set correctly.
 
     Args:
-        container: Container where to embed the file contents
-        container_path: Fresh path in container where to place the file
+        node: Container where to embed the file contents
+        node_path: Fresh path in container where to place the file
         file_path: Path of an existing file to be embedded
         metadata: If provided, will attach this instead of harvesting defaults.
 
     Returns:
         Dataset of new embedded file.
     """
     file_path = Path(file_path)
```

### Comparing `metador_core-0.0.2/metador_core/plugin/entrypoints.py` & `metador_core-0.1.0/src/metador_core/plugin/entrypoints.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,30 +4,34 @@
 import re
 from dataclasses import dataclass
 from typing import Any, Dict, List, Optional, Tuple
 
 from importlib_metadata import Distribution, entry_points
 
 from ..schema.plugins import PluginPkgMeta, SemVerTuple
-from .types import from_ep_group_name, is_metador_ep_group, to_ep_group_name
+from .types import (
+    EPGroupName,
+    from_ep_group_name,
+    is_metador_ep_group,
+    to_ep_group_name,
+)
 
 _eps = entry_points()
 """All entry points."""
 
 pkg_meta = {}
 """Collected infos about packages that provide plugins (filled by get_group)."""
 
 
 def get_group(group_name: str) -> Dict[str, Any]:
     """Get a dict of all available entrypoints for a Metador plugin group."""
     ep_grp = to_ep_group_name(group_name)
     plugins: Dict[str, Any] = {}
 
     for ep in _eps.select(group=ep_grp):
-
         if ep.name in plugins:
             # TODO: will importlib_metadata even return colliding packages?
             # should be figured out (quite important to know)
             msg = f"{group_name}: a plugin named '{ep.name}' is already registered!"
             raise TypeError(msg)
 
         plugins[ep.name] = ep
@@ -58,26 +62,23 @@
 
     # parse entry point groups
     epgs = filter(
         is_metador_ep_group,
         dist.entry_points.groups,
     )
     eps = {
-        from_ep_group_name(epg): list(
+        from_ep_group_name(EPGroupName(epg)): list(
             map(lambda x: x.name, dist.entry_points.select(group=epg))
         )
         for epg in epgs
     }
 
-    def is_repo_url(kv):
-        return kv[0] == "Project-URL" and kv[1].startswith("Repository,")
-
     repo_url: Optional[str] = None
     try:
-        url = next(filter(is_repo_url, dist.metadata.items()))
-        url = url[1].split()[1]  # from "Repository, http://..."
-        repo_url = url
+        urls = dist.metadata.get_all("Project-URL")
+        url = next(filter(lambda u: u.startswith("Repository,"), urls or []))
+        repo_url = url.split()[1]  # from "Repository, http://..."
     except StopIteration:
         pass
     return DistMeta(
         name=dist.name, version=parsed_ver, plugins=eps, repository_url=repo_url
     )
```

### Comparing `metador_core-0.0.2/metador_core/plugin/interface.py` & `metador_core-0.1.0/src/metador_core/plugin/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,19 +134,19 @@
         self._ENTRY_POINTS[ep_name] = ep_obj
 
         if ep_name not in self._VERSIONS:
             self._VERSIONS[name] = []
         self._VERSIONS[name].append(p_ref)
         self._VERSIONS[name].sort()  # should be cheap
 
-    def __init__(self, entrypoints):
+    def __init__(self, entrypoints: Dict[str, EntryPoint]):
         self._ENTRY_POINTS = {}
         self._VERSIONS = {}
 
-        for k, v in entrypoints.values():
+        for k, v in entrypoints.items():
             self._add_ep(k, v)
 
         self._LOADED_PLUGINS = {}
         self.__post_init__()
 
     def __post_init__(self):
         if type(self) is PluginGroup:
@@ -198,19 +198,15 @@
             return self.provider(self.resolve("schema"))
 
         ep_name = util.to_ep_name(ref.name, ref.version)
         ep = self._ENTRY_POINTS[ep_name]
         return self._PKG_META[cast(Any, ep).dist.name]
 
     def is_plugin(self, p_cls):
-        """Return whether this class is a (possibly marked) installed plugin.
-
-        Args:
-            p_cls: class to be checked
-        """
+        """Return whether this class is a (possibly marked) installed plugin."""
         if not isinstance(p_cls, type) or not issubclass(
             p_cls, self.Plugin.plugin_class
         ):
             return False
 
         c = UndefVersion._unwrap(p_cls) or p_cls  # get real underlying class
         # check its exactly a registered plugin, if it has a Plugin section
@@ -242,17 +238,16 @@
     # dict-like interface will provide latest versions of plugins by default
 
     def __contains__(self, key) -> bool:
         name, version = plugin_args(key)
         if pg_versions := self._VERSIONS.get(name):
             if not version:
                 return True
-            else:
-                pg = self.PluginRef(name=name, version=version)
-                return pg in pg_versions
+            pg = self.PluginRef(name=name, version=version)
+            return pg in pg_versions
         return False
 
     def __getitem__(self, key) -> Type[T]:
         if key not in self:
             raise KeyError(f"{self.name} not found: {key}")
         return self.get(key)
 
@@ -376,15 +371,15 @@
         """Perform plugin group specific checks on a registered plugin.
 
         Raises a TypeError with message in case of failure.
 
         To be overridden in subclasses for plugin group specific checks.
 
         Args:
-            name: Declared entrypoint name.
+            ep_name: Declared entrypoint name.
             plugin: Object the entrypoint is pointing to.
         """
         # NOTE: following cannot happen as long as we enforce
         # overriding check_plugin.
         # keep that here for now, in case we loosen this
         # if type(self) is not PluginGroup:
         #    return  # is not the "plugingroup" group itself
```

### Comparing `metador_core-0.0.2/metador_core/plugin/metaclass.py` & `metador_core-0.1.0/src/metador_core/plugin/metaclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     @classmethod
     def _mark_class(cls, c):
         """Mark a class with this marker mixin."""
         if cls._is_marked(c):
             raise TypeError(f"{c} already marked by {cls}!")
 
         ret = c.__class__(c.__name__, (cls, c), {})
+        # ret.__module__ = c.__module__
         setattr(ret, cls._fieldname(), c)
 
         # NOTE: discouraged!
         # https://docs.python.org/3/howto/annotations.html#annotations-howto
         # ----
         # anns = getattr(ret, "__annotations__", {})
         # anns[unw_field] = ClassVar[Type]
```

### Comparing `metador_core-0.0.2/metador_core/plugin/types.py` & `metador_core-0.1.0/src/metador_core/plugin/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,18 @@
     Helper for function argument parsing.
     """
     name: str = ""
     vers: Optional[SemVerTuple] = version
 
     if isinstance(plugin, str):
         name = plugin
+    if isinstance(plugin, tuple) and len(plugin) == 2:
+        name = plugin[0]
+        if not vers:
+            vers = plugin[1]
     elif isinstance(plugin, HasNameVersion):
         name = plugin.name
         if not vers:
             vers = plugin.version
     elif pgi := getattr(plugin, "Plugin", None):
         if isinstance(pgi, HasNameVersion):
             return plugin_args(pgi, version, require_version=require_version)
```

### Comparing `metador_core-0.0.2/metador_core/plugin/util.py` & `metador_core-0.1.0/src/metador_core/plugin/util.py`

 * *Files identical despite different names*

### Comparing `metador_core-0.0.2/metador_core/plugins.py` & `metador_core-0.1.0/src/metador_core/plugins.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,30 @@
-"""Central place to access all plugin groups."""
+"""Central place for convenient access to all registered plugin groups.
+
+For example, to access the `schema` plugingroup, you can use:
+
+`from metador_core.plugins import schemas`
+"""
 from typing import TYPE_CHECKING, Dict, List, TypeVar, cast
 
 import wrapt
 
 from .plugin.interface import PG_GROUP_NAME, AnyPluginRef, PluginGroup, plugin_args
 
 S = TypeVar("S", bound=PluginGroup)
 
 
 class PGPluginGroup(wrapt.ObjectProxy):
     """PluginGroup plugin group.
 
     This wrapper returns instances of other loaded plugin groups.
 
-    To access the actual plugingroup class that gives out *classes*
-    instead of instances (like all other plugingroups),
-    request the "plugingroup" plugingroup.
+    In the esoteric case that you need to access the actual plugingroup class
+    that gives out *classes* instead of instances (like all other plugingroups),
+    request the "plugingroup" plugingroup. But usually you will not want this.
     """
 
     _self_groups: Dict[AnyPluginRef, PluginGroup]
 
     def __reset__(self):
         self._self_groups.clear()
         self.__init__()
@@ -67,15 +72,14 @@
     def is_plugin(self, obj):
         return obj in self.values()
 
 
 # access to available plugin groups:
 
 plugingroups: PGPluginGroup = PGPluginGroup()
-plugingroup_classes = plugingroups.__wrapped__
 
 # help mypy (obviously only for groups in this package):
 # NOTE: this would be better: https://github.com/python/mypy/issues/13643
 if TYPE_CHECKING:  # pragma: no cover
     from .harvester import PGHarvester
     from .packer import PGPacker
     from .schema.pg import PGSchema
@@ -91,21 +95,21 @@
 # this allows to import like: from metador_core.plugins import schemas
 
 # define what to import with *
 __all__ = list(sorted(map(lambda ref: f"{ref.name}s", plugingroups.keys())))
 
 
 def __dir__() -> List[str]:
-    # show the existing plugin groups for tab completion
+    # show the existing plugin groups for tab completion in e.g. ipython
     return __all__
 
 
 def __getattr__(key: str):
-    # get desired plugin group and add as module attribute
-    # (i.e. this is called once per group)
+    # get desired plugin group and add it as module attribute
+    # (i.e. this is called at most once per group)
     if not isinstance(key, str) or key[-1] != "s":
         raise AttributeError(key)
     if group := plugingroups.get(key[:-1]):
         globals()["__annotations__"][key] = type(group)
         globals()[key] = group
         return group
     raise AttributeError(key)
```

### Comparing `metador_core-0.0.2/metador_core/schema/base.py` & `metador_core-0.1.0/src/metador_core/schema/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 import json
-from typing import Optional, cast
+from pathlib import Path
+from typing import Union
 
-from pydantic import BaseModel, Extra
-from pydantic_yaml import YamlModelMixin
-from pydantic_yaml.mixin import YamlModelMixinConfig, YamlStyle
+from pydantic import BaseModel, Extra, ValidationError
+from pydantic_yaml import parse_yaml_file_as, parse_yaml_raw_as, to_yaml_str
 
 from .encoder import DynEncoderModelMetaclass
 from .parser import ParserMixin
 
 
 def _mod_def_dump_args(kwargs):
     """Set `by_alias=True` in given kwargs dict, if not set explicitly."""
     if "by_alias" not in kwargs:
         kwargs["by_alias"] = True  # e.g. so we get correct @id, etc fields
     if "exclude_none" not in kwargs:
         kwargs["exclude_none"] = True  # we treat None as "missing" so leave it out
     return kwargs
 
 
-class BaseModelPlus(
-    ParserMixin, YamlModelMixin, BaseModel, metaclass=DynEncoderModelMetaclass
-):
+class BaseModelPlus(ParserMixin, BaseModel, metaclass=DynEncoderModelMetaclass):
     """Extended pydantic BaseModel with some good defaults.
 
     Used as basis for various entities, including:
     * Metadata schemas
     * Harvester arguments
     """
 
@@ -64,38 +62,31 @@
     def json_dict(self, **kwargs):
         """Return a JSON-compatible dict.
 
         Uses round-trip through JSON serialization.
         """
         return json.loads(self.json(**kwargs))
 
-    def yaml(
-        self,
-        *,
-        # sort_keys: bool = False,
-        default_flow_style: bool = False,
-        default_style: Optional[YamlStyle] = None,
-        indent: Optional[bool] = None,
-        encoding: Optional[str] = None,
-        **kwargs,
-    ) -> str:
+    def yaml(self, **kwargs) -> str:
         """Return serialized YAML as string."""
         # Current way: use round trip through JSON to kick out non-JSON entities
         # (more elegant: allow ruamel yaml to reuse defined custom JSON dumpers)
-        tmp = self.json_dict(**_mod_def_dump_args(kwargs))
-        # NOTE: yaml_dumps is defined by the used yaml mixin in the config
-        cfg = cast(YamlModelMixinConfig, self.__config__)
-        return cfg.yaml_dumps(
-            tmp,
-            # sort_keys=sort_keys, # does not work for some weird arg passing reason
-            default_flow_style=default_flow_style,
-            default_style=default_style,
-            encoding=encoding,
-            indent=indent,
-        )
+        # tmp = self.json_dict(**_mod_def_dump_args(kwargs))
+        return to_yaml_str(self)
+
+    @classmethod
+    def parse_file(cls, path: Union[str, Path]):
+        return parse_yaml_file_as(cls, path)
+
+    @classmethod
+    def parse_raw(cls, dat: Union[str, bytes], **kwargs):
+        try:
+            return super().parse_raw(dat, **kwargs)
+        except ValidationError:
+            return parse_yaml_raw_as(cls, dat)
 
     def __bytes__(self) -> bytes:
         """Serialize to JSON and return UTF-8 encoded bytes to be written in a file."""
         # add a newline, as otherwise behaviour with text editors will be confusing
         # (e.g. vim automatically adds a trailing newline that it hides)
         # https://stackoverflow.com/questions/729692/why-should-text-files-end-with-a-newline
         return (self.json() + "\n").encode(encoding="utf-8")
```

### Comparing `metador_core-0.0.2/metador_core/schema/common/__init__.py` & `metador_core-0.1.0/src/metador_core/schema/common/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
                 if cls.require_unit:
                     raise ValueError(f"Value '{v}' must have a unit!")
                 val = parse_obj_as(Number, arr[0])
                 # return with inferred unit
                 return tcls.construct(value=val, unitText=cls.infer_unit)
 
             val = parse_obj_as(Tuple[Number, str], arr)
-            if cls.allowed_units and not val[1] in cls.allowed_units:
+            if cls.allowed_units and val[1] not in cls.allowed_units:
                 msg = (
                     f"Invalid unit '{val[1]}', unit must be one of {cls.allowed_units}"
                 )
                 raise ValueError(msg)
             return tcls.construct(value=val[0], unitText=val[1])
```

### Comparing `metador_core-0.0.2/metador_core/schema/common/rocrate.py` & `metador_core-0.1.0/src/metador_core/schema/common/rocrate.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,22 +75,26 @@
         )
         if has_given_or_additional and not values.get("familyName"):
             msg = "givenName and additionalName require also familyName to be provided!"
             raise ValueError(msg)
         return values
 
     @root_validator
-    def infer_name(cls, values):
+    def ensure_name(cls, values):
         missing_name = values.get("name") is None
         if missing_name:
             parts = []
             for k in ["givenName", "additionalName", "familyName"]:
                 if v := values.get(k):
                     parts.append(v)
-            values["name"] = " ".join(parts)
+            fullname = " ".join(parts)
+            if not fullname:
+                msg = "A Person must have name or familyName set!"
+                raise ValueError(msg)
+            values["name"] = fullname
         return values
 
 
 # required self-description of RO-Crate file
 rocrate_self_meta = {
     "@type": "CreativeWork",
     "@id": "ro-crate-metadata.json",
```

### Comparing `metador_core-0.0.2/metador_core/schema/core.py` & `metador_core-0.1.0/src/metador_core/schema/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Core Metadata schemas for Metador that are essential for the container API."""
 
+
 from __future__ import annotations
 
+import contextlib
 from collections import ChainMap
 from functools import partial
 from typing import Any, ClassVar, Dict, Optional, Set, Type, cast
 
 import wrapt
 from pydantic import Extra, root_validator
 
@@ -25,28 +27,27 @@
 from .inspect import (
     FieldInspector,
     LiftedRODict,
     WrappedLiftedDict,
     lift_dict,
     make_field_inspector,
 )
-from .jsonschema import finalize_schema_extra, schema_of
+
+# from .jsonschema import finalize_schema_extra, schema_of
 from .partial import PartialFactory, is_mergeable_type
 from .types import to_semver_str
 
 
 def add_missing_field_descriptions(schema, model):
     """Add missing field descriptions from own Fields info, if possible."""
     for fname, fjsdef in schema.get("properties", {}).items():
         if not fjsdef.get("description"):
-            try:
+            with contextlib.suppress(KeyError):
                 if desc := model.Fields[fname].description:
                     fjsdef["description"] = desc
-            except KeyError:
-                pass  # no field info for that field
 
 
 KEY_SCHEMA_PG = "$metador_plugin"
 """Key in JSON schema to put metador plugin name an version."""
 
 KEY_SCHEMA_CONSTFLDS = "$metador_constants"
 """Key in JSON schema to put metador 'constant fields'."""
@@ -83,21 +84,22 @@
                 schema[KEY_SCHEMA_CONSTFLDS] = {}
                 for cname, cval in model.__constants__.items():
                     # list them (so they are not rejected even with additionalProperties=False)
                     schema["properties"][cname] = True
                     # store the constant alongside the schema
                     schema[KEY_SCHEMA_CONSTFLDS][cname] = cval
 
-            # do magic
-            finalize_schema_extra(schema, model, base_model=MetadataSchema)
+            # do magic (TODO: fix/rewrite)
+            # finalize_schema_extra(schema, model, base_model=MetadataSchema)
 
-    @classmethod
-    def schema(cls, *args, **kwargs):
-        """Return customized JSONSchema for this model."""
-        return schema_of(UndefVersion._unwrap(cls) or cls, *args, **kwargs)
+    # NOTE: custom JSON schema feature is broken
+    # @classmethod
+    # def schema(cls, *args, **kwargs):
+    #    """Return customized JSONSchema for this model."""
+    #    return schema_of(UndefVersion._unwrap(cls) or cls, *args, **kwargs)
 
     @root_validator(pre=True)
     def override_consts(cls, values):
         """Override/add defined schema constants.
 
         They must be present on dump, but are ignored on load.
         """
@@ -187,21 +189,21 @@
 
         # "constant fields" are inherited, but copied - not shared
         self.__constants__ = {}
         for b in bases:
             self.__constants__.update(getattr(b, "__constants__", {}))
 
     @property  # type: ignore
-    @cache
+    @cache  # noqa: B019
     def _typehints(self):
         """Return typehints of this class."""
         return get_type_hints(self)
 
     @property  # type: ignore
-    @cache
+    @cache  # noqa: B019
     def _base_typehints(self):
         """Return typehints accumulated from base class chain."""
         return ChainMap(
             *(b._typehints for b in self.__bases__ if issubclass(b, SchemaBase))
         )
 
     # ---- for public use ----
@@ -247,15 +249,15 @@
 
 
 # ----
 
 
 def _indent_text(txt, prefix="\t"):
     """Add indentation at new lines in given string."""
-    return "\n".join(map(lambda l: f"{prefix}{l}", txt.split("\n")))
+    return "\n".join(map(lambda line: f"{prefix}{line}", txt.split("\n")))
 
 
 class SchemaFieldInspector(FieldInspector):
     """MetadataSchema-specific field inspector.
 
     It adds a user-friendly repr and access to nested subschemas.
     """
@@ -342,31 +344,33 @@
             if k not in obj.__constants__
         )
 
     # override to add some fixes to partials
     @classmethod
     def _create_partial(cls, mcls, *, typehints=...):
         th = getattr(mcls, "_typehints", None)
-        ret, nested = super()._create_partial(mcls, typehints=th)
+        unw = UndefVersion._unwrap(mcls) or mcls
+        ret, nested = super()._create_partial(unw, typehints=th)
         # attach constant field list for field filtering
-        setattr(ret, "__constants__", getattr(mcls, "__constants__", set()))
+        ret.__constants__ = getattr(mcls, "__constants__", set())
         # copy custom parser to partial
         # (otherwise partial can't parse correctly with parser mixin)
         if parser := getattr(mcls, "Parser", None):
-            setattr(ret, "Parser", parser)
+            ret.Parser = parser
         return (ret, nested)
 
 
 # --- delayed checks (triggered during schema loading) ---
 # if we do it earlier, might lead to problems with forward refs and circularity
 
 
 def check_types(schema: Type[MetadataSchema], *, recheck: bool = False):
     if schema is MetadataSchema or schema.__types_checked__ and not recheck:
         return
+    schema.__types_checked__ = True
 
     # recursively check compositional and inheritance dependencies
     for b in schema.__bases__:
         if issubclass(b, MetadataSchema):
             check_types(b, recheck=recheck)
 
     schemaFields = cast(Any, schema.Fields)
@@ -375,16 +379,14 @@
             s = schemaFields[f].schemas[sname]
             if s is not schema and issubclass(s, MetadataSchema):
                 check_types(s, recheck=recheck)
 
     check_allowed_types(schema)
     check_overrides(schema)
 
-    schema.__types_checked__ = True
-
 
 def check_allowed_types(schema: Type[MetadataSchema]):
     """Check that shape of defined fields is suitable for deep merging."""
     hints = cast(Any, schema._typehints)
     for field, hint in hints.items():
         if not is_public_name(field):
             continue  # private field
```

### Comparing `metador_core-0.0.2/metador_core/schema/decorators.py` & `metador_core-0.1.0/src/metador_core/schema/decorators.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import Any, Dict, Optional
+from typing import Any, Dict, Literal, Optional
 
 from pydantic.fields import ModelField
 
 from ..util import is_public_name
 from ..util.models import field_parent_type
-from ..util.typing import get_annotations, unoptional
+from ..util.typing import get_annotations, is_enum, is_literal, is_subtype, unoptional
 from .core import MetadataSchema
 
 
 def _expect_schema_class(mcls):
     if not issubclass(mcls, MetadataSchema):
         raise TypeError("This decorator is for MetadataSchema subclasses!")
 
@@ -31,15 +31,14 @@
     # but is this good? defaults are implicit optionality -> we discourage it, so no.
     _check_names_public(names)
 
     def make_fields_mandatory(mcls):
         _expect_schema_class(mcls)
 
         for name in names:
-
             if name not in mcls.__fields__:
                 raise ValueError(f"{mcls.__name__} has no field named '{name}'!")
             if name in get_annotations(mcls):
                 raise ValueError(
                     f"{mcls.__name__} already defines '{name}', cannot use decorator!"
                 )
 
@@ -71,20 +70,42 @@
 
     def add_fields(mcls):
         _expect_schema_class(mcls)
 
         # hacking it in-place approach:
         overridden = set()
         for name, value in consts.items():
-
-            if name in mcls.__fields__:
-                if not override:
-                    msg = f"{mcls} already has a field '{name}'! (override={override})"
+            if field_def := mcls.__fields__.get(name):  # overriding a field
+                # we allow to silently override of enum/literal types with suitable values
+                # to support a schema design pattern of marked subclasses
+                # but check that it is actually used correctly.
+                enum_specialization = is_enum(field_def.type_)
+                literal_specialization = is_literal(field_def.type_)
+
+                valid_specialization = False
+                if enum_specialization:
+                    valid_specialization = isinstance(value, field_def.type_)
+                elif literal_specialization:
+                    lit_const = Literal[value]  # type: ignore
+                    valid_specialization = is_subtype(lit_const, field_def.type_)
+
+                if (
+                    enum_specialization or literal_specialization
+                ) and not valid_specialization:
+                    msg = f"{mcls.__name__}.{name} cannot be overriden with '{value}', "
+                    msg += f"because it is not a valid value of {field_def.type_}!"
+                    raise TypeError(msg)
+
+                # reject if not force override or allowed special cases
+                if not (override or enum_specialization or literal_specialization):
+                    msg = f"{mcls.__name__} already has a field '{name}'!"
+                    msg += f" (override={override})"
                     raise ValueError(msg)
-                else:
+
+                else:  # new field
                     overridden.add(name)
 
             # this would force the exact constant on load
             # but this breaks parent compatibility if consts overridden!
             # ----
             # val = value.default if isinstance(value, FieldInfo) else value
             # ctype = Optional[make_literal(val)]  # type: ignore
```

### Comparing `metador_core-0.0.2/metador_core/schema/encoder.py` & `metador_core-0.1.0/src/metador_core/schema/encoder.py`

 * *Files identical despite different names*

### Comparing `metador_core-0.0.2/metador_core/schema/inspect.py` & `metador_core-0.1.0/src/metador_core/schema/inspect.py`

 * *Files identical despite different names*

### Comparing `metador_core-0.0.2/metador_core/schema/jsonschema.py` & `metador_core-0.1.0/src/metador_core/schema/jsonschema.py`

 * *Files 3% similar despite different names*

```diff
@@ -146,14 +146,15 @@
         if new_name := defmap.get(refstr[plen:]):
             return f"#/{KEY_SCHEMA_DEFS}/{new_name}"
     return refstr
 
 
 def update_refs(defmap, obj):
     """Recursively update `$ref` in `obj` based on defmap."""
+    print("update", obj)
     if isinstance(obj, (type(None), bool, int, float, str)):
         return obj
     elif isinstance(obj, list):
         return list(map(partial(update_refs, defmap), obj))
     elif isinstance(obj, dict):
         return {
             k: (update_refs(defmap, v) if k != "$ref" else map_ref(defmap, v))
@@ -193,14 +194,15 @@
 def schema_of(model: Type[BaseModel], *args, **kwargs):
     """Return JSON Schema for a model.
 
     Improved version of `pydantic.schema_of`, returns result
     in $defs normal form, with $ref pointing to the model.
     """
     schema = pyd_schema_of(model, *args, **kwargs)
+    print(type(schema), schema)
     schema.pop("title", None)
     fixup_jsonschema(schema)
     return schema
 
 
 def schemas(models: Iterable[Type[BaseModel]], *args, **kwargs):
     """Return JSON Schema for multiple models.
@@ -260,14 +262,16 @@
     base_model: Type[BaseModel] = None,
 ) -> None:
     """Perform custom JSON Schema postprocessing.
 
     To be called as last action in custom schema_extra method in the used base model.
 
     Arguments:
+        schema: The JSON object containing the schema
+        model: The underlying pydantic model
         base_model: The custom base model that this function is called for.
     """
     base_model = base_model or BaseModel
     assert issubclass(model, base_model)
 
     # a schema should have a specified standard
     schema["$schema"] = "https://json-schema.org/draft/2020-12/schema"
```

### Comparing `metador_core-0.0.2/metador_core/schema/ld.py` & `metador_core-0.1.0/src/metador_core/schema/ld.py`

 * *Files 9% similar despite different names*

```diff
@@ -81,12 +81,19 @@
 
     @property
     def is_ld_ref(self):
         return True
 
 
 T = TypeVar("T", bound=LDSchema)
+
 LDOrRef: TypeAlias = Union[LDIdRef, T]
 """LDOrRef[T] is either an object of LD Schema T, or a reference to an object.
 
 An LD reference is just an object with an @id.
 """
+
+LDRef: TypeAlias = LDIdRef  # Annotated[LDIdRef, T]  # <- does not work :(
+"""LDRef[T] is a reference to an object of type T.
+
+An LD reference is just an object with an @id.
+"""
```

### Comparing `metador_core-0.0.2/metador_core/schema/parser.py` & `metador_core-0.1.0/src/metador_core/schema/parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """Simplify creation of custom parsers for pydantic models."""
-from functools import partial
 from typing import Any, ClassVar, Dict, Type, TypeVar
 
 from pydantic import BaseModel
 
 T = TypeVar("T")
 
 
 class BaseParser:
     """Parsers that work with the ParserMixin must inherit from this class."""
 
     schema_info: Dict[str, Any] = {}
     strict: bool = True
 
     @classmethod
-    def parse(cls, tcls: Type[T], v: Any) -> T:
+    def parse(cls, target: Type[T], v: Any) -> T:
         """Override and implement this method for custom parsing.
 
         The default implementation will simply pass through
         any instances of `tcls` unchanged and fail on anything else.
 
         Make sure that the parser can also handle any object that itself
         produces as an input.
@@ -27,28 +26,29 @@
         i.e. produce an instance of `tcls`, any other returned type
         will lead to an exception.
 
         If you know what you are doing, set `strict=False` to
         disable this behavior.
 
         Args:
-            tcls: target class whose instance should be returned
+            target: class the value should be parsed into
             v: value to be parsed
         """
-        if not isinstance(v, tcls):
-            raise TypeError(f"Expected {tcls.__name__}, but got {type(v).__name__}!")
+        if target is not None and not isinstance(v, target):
+            raise TypeError(f"Expected {target.__name__}, but got {type(v).__name__}!")
         return v
 
 
-def run_parser(cls: Type[BaseParser], tcls: Type, v: Any):
+def run_parser(cls: Type[BaseParser], target: Type[T], value: Any):
     """Parse and validate passed value."""
-    # print("call parser", cls, "into", tcls, "on", v, ":", type(v))
-    ret = cls.parse(tcls, v)
-    if cls.strict and not isinstance(ret, tcls):
-        msg = f"Parser returned:  {type(ret)}, expected: {tcls} (strict=True)"
+    # print("call parser", cls, "from", tcls, "on", value, ":", type(value))
+    ret = cls.parse(target, value)
+    if cls.strict and not isinstance(ret, target):
+        msg = f"Parser returned: {type(ret).__name__}, "
+        msg += f"expected: {target.__name__} (strict=True)"
         raise RuntimeError(msg)
     return ret
 
 
 def get_parser(cls):
     """Return inner Parser class, or None.
 
@@ -77,27 +77,31 @@
     """
 
     Parser: ClassVar[Type[BaseParser]]
 
     @classmethod
     def __get_validators__(cls):
         pfunc = cls.__dict__.get("__parser_func__")
-
         if pfunc is None:
             if parser := get_parser(cls):
-                pfunc = partial(run_parser, parser, cls)
+
+                def wrapper_func(cls, value, values=None, config=None, field=None):
+                    return run_parser(parser, field.type_, value)
+
+                pfunc = wrapper_func
             else:
                 pfunc = NoParserDefined
             cls.__parser_func__ = pfunc  # cache it
 
         if pfunc is not NoParserDefined:  # return cached parser function
-            # print("yield custom parser", pfunc)
             yield pfunc
 
-        # important: if no parser is given, return the default validate function of the model!
+        # important: if no parser is given
+        # and class is a model,
+        # also return the default validate function of the model!
         if issubclass(cls, BaseModel):
             yield cls.validate
 
     @classmethod
     def __modify_schema__(cls, schema):
         if parser := get_parser(cls):
             if schema_info := parser.schema_info:
```

### Comparing `metador_core-0.0.2/metador_core/schema/partial.py` & `metador_core-0.1.0/src/metador_core/schema/partial.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,28 +199,29 @@
         Otherwise, will call `to_partial`.
         """
         if isinstance(obj, cls):
             return obj
         return cls.to_partial(obj, ignore_invalid=ignore_invalid)
 
     def _update_field(
-        cls,
+        self,
         v_old,
         v_new,
         *,
-        path: List[str] = [],
+        path: List[str] = None,
         allow_overwrite: bool = False,
     ):
         """Return merged result of the two passed arguments.
 
         None is always overwritten by a non-None value,
         lists are concatenated, sets are unionized,
         partial models are recursively merged,
         otherwise the new value overwrites the old one.
         """
+        path = path or []
         # None -> missing value -> just use new value (shortcut)
         if v_old is None or v_new is None:
             return v_new or v_old
 
         # list -> new one must also be a list -> concatenate
         if isinstance(v_old, list):
             return v_old + v_new
@@ -228,19 +229,19 @@
         # set -> new one must also be a set -> set union
         if isinstance(v_old, set):
             # NOTE: we could try being smarter for sets of partial models
             # https://github.com/Materials-Data-Science-and-Informatics/metador-core/issues/20
             return v_old.union(v_new)  # set union
 
         # another model -> recursive merge of partials, if compatible
-        old_is_model = isinstance(v_old, cls.__partial_fac__.base_model)
-        new_is_model = isinstance(v_new, cls.__partial_fac__.base_model)
+        old_is_model = isinstance(v_old, self.__partial_fac__.base_model)
+        new_is_model = isinstance(v_new, self.__partial_fac__.base_model)
         if old_is_model and new_is_model:
-            v_old_p = cls.__partial_fac__.get_partial(type(v_old)).cast(v_old)
-            v_new_p = cls.__partial_fac__.get_partial(type(v_new)).cast(v_new)
+            v_old_p = self.__partial_fac__.get_partial(type(v_old)).cast(v_old)
+            v_new_p = self.__partial_fac__.get_partial(type(v_new)).cast(v_new)
             new_subclass_old = issubclass(type(v_new_p), type(v_old_p))
             old_subclass_new = issubclass(type(v_old_p), type(v_new_p))
             if new_subclass_old or old_subclass_new:
                 try:
                     return v_old_p.merge_with(
                         v_new_p, allow_overwrite=allow_overwrite, _path=path
                     )
@@ -260,23 +261,24 @@
 
     def merge_with(
         self,
         obj,
         *,
         ignore_invalid: bool = False,
         allow_overwrite: bool = False,
-        _path: List[str] = [],
+        _path: List[str] = None,
     ):
         """Return a new partial model with updated fields (without validation).
 
         Raises `ValidationError` if passed `obj` is not suitable,
         unless `ignore_invalid` is set to `True`.
 
         Raises `ValueError` if `allow_overwrite=False` and a value would be overwritten.
         """
+        _path = _path or []
         obj = self.cast(obj, ignore_invalid=ignore_invalid)  # raises on failure
 
         ret = self.copy()  # type: ignore
         for f_name, v_new in self.__partial_fac__._get_field_vals(obj):
             v_old = ret.__dict__.get(f_name)
             v_merged = self._update_field(
                 v_old, v_new, path=_path + [f_name], allow_overwrite=allow_overwrite
@@ -470,15 +472,18 @@
         if partial := _partials[cls].get(mcls):
             return partial  # already have a partial
         else:  # block the spot (to break recursion)
             _partials[cls][mcls] = None
 
         # ----
         # create a partial for a model:
-        mcls.update_forward_refs()  # to be sure
+        # localns = {cls._partial_forwardref_name(k): v for k,v in _partials[cls].items() if v}
+        localns: Dict[str, Any] = {}
+        mcls.update_forward_refs(**localns)  # to be sure
+
         partial, nested = cls._create_partial(mcls, typehints=typehints)
         partial_ref = cls._partial_forwardref_name(mcls)
         # store result
         _forwardrefs[cls][partial_ref] = partial
         _partials[cls][mcls] = partial
         # create partials for nested models
         for model in nested:
```

### Comparing `metador_core-0.0.2/metador_core/schema/pg.py` & `metador_core-0.1.0/src/metador_core/schema/pg.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,14 +142,23 @@
         ] = {}
         self._subschemas: Dict[MetadataSchema, Set[MetadataSchema]] = {}
 
         # partial schema classes
         self._partials: Dict[MetadataSchema, PartialModel] = {}
         self._forwardrefs: Dict[str, MetadataSchema] = {}
 
+    def plugin_deps(self, plugin) -> Set[AnyPluginRef]:
+        self._parent_schema[plugin] = infer_parent(plugin)
+        if pcls := self._parent_schema[plugin]:
+            # make sure a parent schema plugin is initialized before the child
+            info = pcls.Plugin
+            return {self.PluginRef(name=info.name, version=info.version)}
+        else:
+            return set()
+
     def check_plugin(self, name: str, plugin: Type[MetadataSchema]):
         check_types(plugin)  # ensure that (overrides of) fields are valid
 
     def _compute_parent_path(self, plugin: Type[MetadataSchema]) -> List[AnyPluginRef]:
         ref = plugin.Plugin.ref()
         ret = [ref]
         curr = plugin
@@ -160,17 +169,14 @@
             curr = self._get_unsafe(p_ref.name, p_ref.version)
             parent = self._parent_schema[curr]
 
         ret.reverse()
         return ret
 
     def init_plugin(self, plugin):
-        # infer the parent schema plugin, if any
-        self._parent_schema[plugin] = infer_parent(plugin)
-
         # pre-compute parent schema path
         ref = plugin.Plugin.ref()
         self._parents[ref] = self._compute_parent_path(plugin)
         if ref not in self._children:
             self._children[ref] = set()
 
         # collect children schema set for all parents
```

### Comparing `metador_core-0.0.2/metador_core/schema/plugins.py` & `metador_core-0.1.0/src/metador_core/schema/plugins.py`

 * *Files identical despite different names*

### Comparing `metador_core-0.0.2/metador_core/schema/types.py` & `metador_core-0.1.0/src/metador_core/schema/types.py`

 * *Files identical despite different names*

### Comparing `metador_core-0.0.2/metador_core/util/diff.py` & `metador_core-0.1.0/src/metador_core/util/diff.py`

 * *Files identical despite different names*

### Comparing `metador_core-0.0.2/metador_core/util/hashsums.py` & `metador_core-0.1.0/src/metador_core/util/hashsums.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,25 +44,23 @@
 
 def file_hashsum(path: Path, alg: str = DEF_HASH_ALG):
     with open(path, "rb") as f:
         return qualified_hashsum(f, alg)
 
 
 DirHashsums = Dict[str, Any]
-"""
-Nested dict representing a directory.
+"""Nested dict representing a directory.
 
 str values represent files (checksum) or symlinks (target path),
 dict values represent sub-directories.
 """
 
 
 def rel_symlink(base: Path, dir: Path) -> Optional[Path]:
-    """
-    From base path and a symlink path, normalize it to be relative to base.
+    """From base path and a symlink path, normalize it to be relative to base.
 
     Mainly used to eliminate .. in paths.
 
     If path points outside base, returns None.
     """
     path = dir.parent / os.readlink(str(dir))
     try:
```

### Comparing `metador_core-0.0.2/metador_core/util/models.py` & `metador_core-0.1.0/src/metador_core/util/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,16 +28,17 @@
     return filter(is_subclass_of(bound), traverse_typehint(mf.type_))
 
 
 def atomic_types(m: BaseModel, *, bound=object) -> Dict[str, Set[Type]]:
     """Return dict from field name to model classes referenced in the field definition.
 
     Args:
-        bound: If provided, will be used to filter results to
-          contain only subclasses of the bound.
+        m: Pydantic model
+        bound (object): If provided, will be used to filter results to
+            contain only subclasses of the bound.
     """
     return {k: set(field_atomic_types(v, bound=bound)) for k, v in m.__fields__.items()}
 
 
 def field_parent_type(m: Type[BaseModel], name: str) -> Type[BaseModel]:
     """Return type of field assigned in the next parent that provides a type hint."""
     b = next(filter(lambda x: x is not m, field_origins(m, name)), None)
```

### Comparing `metador_core-0.0.2/metador_core/util/typing.py` & `metador_core-0.1.0/src/metador_core/util/typing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,28 @@
+import enum
 from collections import ChainMap
-from typing import Any, Callable, Dict, Iterable, List, Mapping, Set, Tuple, Type, Union
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Iterable,
+    List,
+    Literal,
+    Mapping,
+    Set,
+    Tuple,
+    Type,
+    Union,
+)
 
 import typing_extensions as te
-import typing_utils
-from typing_extensions import Annotated, ClassVar, Literal, TypedDict
+
+# import typing_utils  # for issubtype
+from runtype import validation as rv  # for is_subtype
+from typing_extensions import Annotated, ClassVar, TypedDict
 
 get_args = te.get_args  # re-export get_args
 
 TypeHint: Any
 """For documentation purposes - to mark type hint arguments."""
 
 
@@ -58,14 +73,18 @@
     return get_origin(hint) is ClassVar
 
 
 def is_annotated(hint):
     return get_origin(hint) is Annotated
 
 
+def is_literal(hint):
+    return get_origin(hint) is Literal
+
+
 NoneType = type(None)
 
 
 def is_nonetype(hint):
     return hint is NoneType
 
 
@@ -102,30 +121,34 @@
 
     Sets and floats are not supported.
     """
     if val is None:
         return type(None)
     elif isinstance(val, (bool, int, str)):
         return make_typehint(LIT, val)
+    elif issubclass(val.__class__, enum.Enum):
+        return make_typehint(LIT, val.value)
     elif isinstance(val, (tuple, list)):
         args = tuple(map(make_literal, val))
         return make_typehint(TUP, *args)
     elif isinstance(val, dict):
         d = {k: make_literal(v) for k, v in val.items()}
         # NOTE: the TypedDict must be from typing_extensions for 3.8!
         return TypedDict("AnonConstDict", d)  # type: ignore
     raise ValueError(f"Unsupported value: {val}")
 
 
 def make_tree_traversal(succ_func: Callable[[Any], Iterable]):
     """Return generator to traverse nodes of a tree-shaped object.
 
+    Returned function has a boolean keyword argument `post_order`.
+    If True, will emit the parent node after children instead of before.
+
     Args:
-        child_func: Function to be called on each node returning Iterable of children
-        post_order: If True, will emit the parent node after children instead of before
+        succ_func: Function to be called on each node returning Iterable of children
     """
 
     def traverse(obj, *, post_order: bool = False):
         if not post_order:
             yield obj
         for t in succ_func(obj):
             yield from traverse(t, post_order=post_order)
@@ -135,15 +158,15 @@
     return traverse
 
 
 traverse_typehint = make_tree_traversal(get_args)
 """Perform depth-first pre-order traversal of a type annotation.
 
 Args:
-    th: type hint object to be traversed
+    th (object): type hint object to be traversed
 """
 
 
 def make_tree_mapper(node_constructor, succ_func):
     def map_func(obj, leaf_map_func):
         if children := succ_func(obj):
             mcs = (map_func(c, leaf_map_func) for c in children)
@@ -177,23 +200,26 @@
 
 
 # ----
 
 
 def is_subtype(sub, base):
     # add hack to ignore pydantic Annotated FieldInfo
+    # add hacky fix for literals
     # NOTE: this is only superficial, actually issubtype must be fixed
-    # or it won't work with nested Annotated types
+    # or it won't work with nested Annotated types or complicated stuff
     ann_sub, ann_base = is_annotated(sub), is_annotated(base)
-    if ann_sub != ann_base:
+    lit_sub, lit_base = is_literal(sub), is_literal(base)
+    if ann_sub != ann_base or lit_sub != lit_base:
         return False  # not equal on annotated wrapping status
 
     if not ann_sub:
         # proceed as usual
-        return typing_utils.issubtype(sub, base)
+        return rv.is_subtype(sub, base)
+        # return typing_utils.issubtype(sub, base)
     else:
         sub_args, base_args = get_args(sub), get_args(base)
         # NOTE: FieldInfo of pydantic is not comparable :( so we ignore it
         # same_ann = list(sub_args)[1:] == list(base_args)[1:]
         return is_subtype(sub_args[0], base_args[0])  # and same_ann
 
 
@@ -206,7 +232,10 @@
     """Return a predicate to check isinstance for a given type."""
     return lambda obj: isinstance(obj, t)
 
 
 def is_subclass_of(t: Any) -> Callable[[Any], bool]:
     """Return a predicate to check issubclass for a given type."""
     return lambda obj: isinstance(obj, type) and issubclass(obj, t)
+
+
+is_enum = is_subclass_of(enum.Enum)
```

### Comparing `metador_core-0.0.2/metador_core/widget/__init__.py` & `metador_core-0.1.0/src/metador_core/widget/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Pluggable widgets for Metador."""
+"""Interface of Metador widget plugins."""
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import (
     TYPE_CHECKING,
     Any,
     ClassVar,
@@ -48,30 +48,34 @@
     def __init__(
         self,
         node: MetadorNode,
         schema_name: str = "",
         schema_version: Optional[SemVerTuple] = None,
         *,
         server: Optional[WidgetServer] = None,
+        container_id: Optional[str] = None,
         metadata: Optional[MetadataSchema] = None,
         max_width: Optional[int] = None,
         max_height: Optional[int] = None,
+        keep_ratio: bool = False,
     ):
         """Instantiate a widget for a node.
 
         If no schema name is provided, the widget will try to pick the first metadata object
         from the node that is an instance of a supported schema, in the listed order.
 
         If no server is provided, a stand-alone server is started (e.g. for use in a notebook).
 
         If a metadata object is passed explicitly, it will be used instead of trying to
         retrieve one from the node.
         """
         # NOTE: we restrict the node so that widgets don't try to escape their scope
         self._node = node.restrict(read_only=True, local_only=True)
+        # NOTE: if no container_id is passed, we assume its jupyter mode (based on the metador UUIDs)
+        self._container_id = container_id or str(node.metador.container_uuid)
 
         # if no server passed, we're in Jupyter mode - use standalone
         srv: WidgetServer
         if server is not None:
             srv = server
         else:
             from .jupyter.standalone import running, widget_server
@@ -79,18 +83,14 @@
             if not running():
                 raise ValueError(
                     "No widget server passed and standalone server not running!"
                 )
             srv = widget_server()
         self._server = srv
 
-        # maximal width and height to use / try to fill
-        self._w = max_width
-        self._h = max_height
-
         # setup correct metadata
         if metadata is not None:
             if not self.supports_meta(metadata):
                 msg = "Passed metadata is not instance of a supported schema!"
                 raise ValueError(msg)
             self._meta = metadata
         else:
@@ -103,14 +103,27 @@
                 raise ValueError("The node does not contain any suitable metadata!")
 
             if metadata := node.meta.get(schema_name, schema_version):
                 self._meta = metadata
             else:
                 raise ValueError("The node does not contain '{schema_name}' metadata!")
 
+        # maximum width and height that can be used (if None, unlimited)
+        self._w: Optional[int] = max_width
+        self._h: Optional[int] = max_height
+
+        # recalibrate maximum width and height of widgets to preserve ration, if possible + desired
+        can_scale = self._meta.width is not None and self._meta.height is not None
+        if keep_ratio and can_scale:
+            scale_factor = min(
+                self._h / self._meta.height.value, self._w / self._meta.width.value
+            )
+            self._w = int(self._meta.width.value * scale_factor)
+            self._h = int(self._meta.height.value * scale_factor)
+
         # widget-specific setup hook
         self.setup()
 
     def file_data(self, node: Optional[MetadorDataset] = None) -> bytes:
         """Return data at passed dataset node as bytes.
 
         If no node passed, will use the widget root node (if it is a dataset).
@@ -128,23 +141,23 @@
         If no node passed, will use the widget root node (if it is a dataset).
         """
         node = node or self._node
         if not isinstance(node, MetadorDataset):
             raise ValueError(
                 f"Passed node {node.name} does not look like a dataset node!"
             )
-        return self._server.file_url_for(node)
+        return self._server.file_url_for(self._container_id, node)
 
     @classmethod
     def supports(cls, *schemas: PluginRef) -> bool:
         """Return whether any (exact) schema is supported (version-compatible) by widget."""
-        for schema in schemas:
-            if any(map(lambda sref: sref.supports(schema), cls.Plugin.supports)):
-                return True
-        return False
+        return any(
+            any(map(lambda sref: sref.supports(schema), cls.Plugin.supports))
+            for schema in schemas
+        )
 
     @classmethod
     def supports_meta(cls, obj: MetadataSchema) -> bool:
         """Return whether widget supports the specific metadata object.
 
         The passed object is assumed to be of one of the supported schema types.
 
@@ -153,15 +166,15 @@
         Override to constrain further (e.g. check field values).
 
         This method affects the dashboard widget selection process and is used
         to check a metadata object if directly passed to `__init__`.
         """
         return cls.supports(type(obj).Plugin.ref())
 
-    def setup(self):
+    def setup(self):  # noqa: B027  # implementing it is not mandatory
         """Check that passed node is valid and do preparations.
 
         If multiple supported schemas are listed, case splitting based on the
         schema type should be done here to minimize logic in the rendering.
 
         Everything that instances can reuse, especially if it is computationally
         expensive, should also be done here.
```

### Comparing `metador_core-0.0.2/metador_core/widget/common.py` & `metador_core-0.1.0/src/metador_core/widget/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-"""Common widgets."""
+"""Common generic widgets.
+
+These basically integrate many default widgets provided by panel/bokeh into Metador.
+"""
 
 import json
 from typing import List, Set, Type
 
 import panel as pn
 from overrides import overrides
 from panel.viewable import Viewable
@@ -167,14 +170,16 @@
     @overrides
     def show(self) -> Viewable:
         return pn.pane.JSON(
             json.loads(self.file_data()),
             name=self.title,
             max_width=self._w,
             max_height=self._h,
+            hover_preview=True,
+            depth=-1,
         )
 
 
 # pass URL:
 
 
 class PDFWidget(FileWidget):
@@ -201,35 +206,51 @@
         "image/gif": pn.pane.GIF,
         "image/svg+xml": pn.pane.SVG,
     }
 
     @overrides
     def show(self) -> Viewable:
         return self.PANEL_WIDGET[self._meta.encodingFormat](
-            self.file_url(), width=self._w, height=self._h
+            self.file_url(),
+            width=self._w,
+            height=self._h,
+            alt_text="Sorry. Something went wrong while loading the resource",
         )
 
 
+# NOTE: Panel based widget does not work.
+# see - https://github.com/holoviz/panel/issues/3203
+# using HTML based audio & video panes for the audio and video widgets respectively
 class AudioWidget(FileWidget):
     class Plugin(FileWidget.Plugin):
         name = "core.file.audio"
         version = (0, 1, 0)
 
     MIME_TYPES = {"audio/mpeg", "audio/ogg", "audio/webm"}
 
     @overrides
     def show(self) -> Viewable:
-        return pn.pane.Audio(self.file_url(), name=self.title)
+        return pn.pane.HTML(
+            f"""
+                <audio controls>
+                    <source src={self.file_url()} type={self._meta.encodingFormat}>
+                </audio>
+            """,
+        )
 
 
 class VideoWidget(FileWidget):
     class Plugin(FileWidget.Plugin):
         name = "core.file.video"
         version = (0, 1, 0)
 
     MIME_TYPES = {"video/mp4", "video/ogg", "video/webm"}
 
     @overrides
     def show(self) -> Viewable:
-        return pn.pane.Video(
-            self.file_url(), name=self.title, max_width=self._w, max_height=self._h
+        return pn.pane.HTML(
+            f"""
+                <video width={self._w} height={self._h} controls style="object-position: center; object-fit:cover;">
+                <source src={self.file_url()} type={self._meta.encodingFormat}>
+                </video>
+            """,
         )
```

### Comparing `metador_core-0.0.2/metador_core/widget/dashboard.py` & `metador_core-0.1.0/src/metador_core/widget/server/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,321 +1,302 @@
-from __future__ import annotations
-
-from functools import partial
-from itertools import groupby
-from typing import Dict, Iterable, List, Optional, Tuple
-
-import panel as pn
+"""The Metador widget server."""
+import io
+from typing import Dict, List, Literal, Optional, Union
+
+import numpy as np
+from bokeh.application import Application
+from bokeh.application.handlers.function import FunctionHandler
+from bokeh.document import Document
+from bokeh.embed import server_document
+from bokeh.server.server import Server
+from flask import Blueprint, request, send_file
 from panel.viewable import Viewable
-from phantom.interval import Open
-
-from ..container import MetadorContainer, MetadorNode
-from ..plugins import schemas, widgets
-from ..schema import MetadataSchema
-from ..schema.plugins import PluginRef
-from ..schema.types import NonEmptyStr, SemVerTuple
-
-
-class DashboardPriority(int, Open, low=1, high=10):
-    ...
-
-
-class DashboardGroup(int, Open, low=1):
-    ...
-
-
-class DashboardWidgetMeta(MetadataSchema):
-    """Configuration for a widget in the dashboard."""
-
-    priority: Optional[DashboardPriority] = DashboardPriority(1)
-    """Priority of the widget (1-10), higher priority nodes are shown first."""
-
-    group: Optional[DashboardGroup]
-    """Dashboard group of the widget.
-
-    Groups are presented in ascending order.
-    Widgets are ordered by priority within a group.
-    All widgets in a group are shown in a single row.
-
-    Widgets without an assigned group come last.
-    """
-
-    schema_name: Optional[NonEmptyStr]
-    """Name of schema of an metadata object at the current node to be visualized.
+from tornado.ioloop import IOLoop
+from werkzeug.exceptions import BadRequest, NotFound
 
-    If not given, any suitable presentable object will be used.
-    """
-
-    schema_version: Optional[SemVerTuple]
-
-    widget_name: Optional[str]
-    """Name of widget to be used to present the (meta)data.
-
-    If not given, any suitable will be used.
-    """
+from metador_core.container import ContainerProxy, MetadorContainer, MetadorNode
 
-    widget_version: Optional[SemVerTuple]
 
+class WidgetServer:
+    """Server backing the instances of Metador widgets (and dashboard).
 
-class DashboardMeta(MetadataSchema):
-    """Schema describing dashboard configuration for a node in a container.
+    Metador widgets depend on a `WidgetServer` to:
+    * get data from Metador containers (via special flask API, provided as a mountable blueprint)
+    * wire up the information flow with a bokeh server instance (requirement for interactive bokeh widgets)
 
-    Instantiating without passing a list of widget configurations will
-    return an instance that will show an arbitrary suitable widget, i.e.
-    is equivalent to `DashboardMeta.show()`
-    """
-
-    class Plugin:
-        name = "core.dashboard"
-        version = (0, 1, 0)
-
-    widgets: List[DashboardWidgetMeta] = [DashboardWidgetMeta()]
-    """Widgets to present for this node in the dashboard.
-
-    If left empty, will try present any widget usable for this node.
+    For information on running a bokeh server see:
+    https://docs.bokeh.org/en/latest/docs/user_guide/server.html#embedding-bokeh-server-as-a-library
     """
 
     @classmethod
-    def widget(cls, **kwargs) -> DashboardWidgetMeta:
-        # for convenience
-        return DashboardWidgetMeta(**kwargs)
+    def _get_widget_arg(cls, args: Dict[str, List[bytes]], name: str) -> Optional[str]:
+        """Extract argument from bokeh server request argument dict."""
+        return args[name][0].decode("utf-8") if name in args and args[name] else None
 
     @classmethod
-    def show(cls, _arg: List[DashboardWidgetMeta] = None, **kwargs):
-        """Return an instance of dashboard configuration metadata.
-
-        Convenience method to construct a configuration for the node
-        for one or multiple widgets.
+    def _get_widget_args(cls, doc: Document):
+        """Extract arguments from bokeh server request parameters."""
+        args = doc.session_context.request.arguments
+        return dict(
+            container_id=cls._get_widget_arg(args, "id"),
+            container_path=cls._get_widget_arg(args, "path"),
+        )
 
-        For one widget, pass the widget config (if any) as keyword arguments,
-        e.g.  `DashboardMeta.show(group=1)`.
+    @classmethod
+    def _make_widget_args(
+        cls, container_id: str, container_path: Optional[str]
+    ) -> Dict[str, str]:
+        """Construct dict to be passed through bokeh request into widget."""
+        req_args = {"id": container_id}
+        if container_path:
+            req_args["path"] = container_path
+        return req_args
+
+    def _get_bokeh_widget_name(
+        self,
+        viewable_type: Literal["widget", "dashboard"],
+        name: str,
+    ) -> str:
+        """Return mapped name of a registered widget or dashboard (bokeh server endpoint).
 
-        For multiple widgets, instantiate widget configurations with `widget(...)`,
-        and pass them to `show`, e.g.:
-        `DashboardMeta.show([DashboardMeta.widget(), DashboardMeta.widget(group=2)])`.
+        Raises NotFound exception if widget has not been found.
         """
-        if _arg and kwargs:
-            msg = "Pass widget config arguments or list of widget configs - not both!"
-            raise ValueError(msg)
+        if viewable_type not in {"widget", "dashboard"}:
+            msg = f"Invalid type: {viewable_type}. Must be widget or dashboard!"
+            raise NotFound(msg)
+        known = self._reg_widgets if viewable_type == "widget" else self._reg_dashboards
+        if name not in known:
+            raise NotFound(f"Bokeh {viewable_type} not found: '{name}'")
+        return known[name]
+
+    def _get_container_node(
+        self, container_id: str, container_path: Optional[str] = None
+    ) -> Optional[Union[MetadorContainer, MetadorNode]]:
+        """Retrieve desired container (and target path, if provided).
 
-        if _arg is None:
-            # kwargs have config for a singleton widget
-            widgets = [cls.widget(**kwargs)]
-        else:
-            # multiple widgets, preconfigured
-            widgets = list(_arg)
-        return cls(widgets=widgets)
+        If `path` is provided in the query parameters,
+        will return the container node, otherwise returns the full container.
 
+        Raises NotFound exception if container or path in container do not exist.
+        """
+        try:
+            container = self._containers.get(container_id)
+        except KeyError as e:
+            raise NotFound(f"Container not found: '{container_id}'") from e
+
+        if container_path is None:
+            return container
+        if node := container.get(container_path):
+            return node.restrict(read_only=True, local_only=True)
+
+        raise NotFound(f"Path not found in container: {container_path}")
+
+    # ----
+
+    def __init__(
+        self,
+        containers: ContainerProxy[str],
+        *,
+        bokeh_endpoint: Optional[str] = None,
+        flask_endpoint: Optional[str] = None,
+        populate: bool = True,
+    ):
+        """Widget server to serve widget- and dashboard-like bokeh entities.
+
+        Args:
+            containers: `ContainerProxy` to retrieve containers by some container id string.
+            bokeh_endpoint: Endpoint where the bokeh server will run (`WidgetServer.run()`)
+            flask_endpoint: Endpoint where Widget API is mounted (`WidgetServer.get_flask_blueprint()`)
+            populate: If true (default), load and serve all installed widgets and generic dashboard
+        """
+        self._containers = containers
+        self._bokeh_apps: Dict[str, Application] = {}
+        self._reg_widgets: Dict[str, str] = {}
+        self._reg_dashboards: Dict[str, str] = {}
+
+        # these can be set after launching the server threads
+        # (e.g. in case of dynamic port selection)
+        self._flask_endpoint = flask_endpoint or ""
+        self._bokeh_endpoint = bokeh_endpoint or ""
+
+        if populate:
+            self.register_installed()
+
+    def register_installed(self) -> None:
+        """Register installed widgets and the generic dashboard."""
+        # NOTE: do imports here, otherwise circular imports.
+        from metador_core.plugins import widgets
+
+        from ..dashboard import Dashboard
+
+        self.register_dashboard("generic", self.make_bokeh_app(Dashboard))
+        for wclass in widgets.values():
+            self.register_widget(
+                wclass.Plugin.plugin_string(), self.make_bokeh_app(wclass)
+            )
 
-# ----
-
-NodeWidgetPair = Tuple[MetadorNode, DashboardWidgetMeta]
-"""A container node paired up with a widget configuration."""
-
-NodeWidgetRow = List[NodeWidgetPair]
-"""Sorted list of NodeWidgetPairs.
+    def register_widget(self, name: str, bokeh_app: Application) -> None:
+        """Register a new widget application."""
+        mapped_name = f"w-{name}"
+        self._bokeh_apps[f"/{mapped_name}"] = bokeh_app
+        self._reg_widgets[name] = mapped_name
+
+    def register_dashboard(self, name: str, bokeh_app: Application) -> None:
+        """Register a new dashboard application."""
+        mapped_name = f"d-{name}"
+        self._bokeh_apps[f"/{mapped_name}"] = bokeh_app
+        self._reg_dashboards[name] = mapped_name
+
+    def make_bokeh_app(self, viewable_class: Viewable) -> Application:
+        def handler(doc: Document) -> None:
+            """Return bokeh app for Metador widget.
+
+            In this context, a suitable class must satisfy the interface
+            of being initialized with a metador node or container,
+            and having a `show()` method returning a panel `Viewable`.
+
+            The app will understand take `id` and optionally a `path` as query params.
+            These are parsed and used to look up the correct container (node).
+            """
+            w_args = self._get_widget_args(doc)
+            if c_obj := self._get_container_node(**w_args):
+                # if we retrieved container / node, instantiate a widget and show it
+                widget = viewable_class(
+                    c_obj, server=self, container_id=w_args["container_id"]
+                ).show()
+                doc.add_root(widget.get_root(doc))
+
+        return Application(FunctionHandler(handler, trap_exceptions=True))
+
+    @property
+    def flask_endpoint(self) -> str:
+        """Get configured endpoint where WidgetServer API is mounted."""
+        return self._flask_endpoint
+
+    @flask_endpoint.setter
+    def flask_endpoint(self, uri: str):
+        """Set URI where the blueprint from `get_flask_blueprint` is mounted."""
+        self._flask_endpoint = uri.rstrip("/")
+
+    @property
+    def bokeh_endpoint(self) -> str:
+        """Get URI where the bokeh server is running."""
+        return self._bokeh_endpoint
+
+    @bokeh_endpoint.setter
+    def bokeh_endpoint(self, uri: str):
+        """Set URI where the bokeh server is running."""
+        self._bokeh_endpoint = uri.rstrip("/")
+
+    def run(self, **kwargs):
+        """Run bokeh server with the registered apps (will block the current process)."""
+        # kwargs["io_loop"] = kwargs.get("io_loop") or IOLoop()
+        # server = pn.io.server.get_server(self._bokeh_apps, **kwargs)
+
+        kwargs["loop"] = kwargs.get("io_loop") or IOLoop()
+        server = Server(self._bokeh_apps, **kwargs)
+
+        server.start()
+        server.io_loop.start()
 
-Ordered first by descending priority, then by ascending node path.
-"""
+    # ----
+    # Helper functions exposed to widgets
 
+    def file_url_for(self, container_id: str, node: MetadorNode) -> str:
+        """Return URL for given container ID and file at Metador Container node.
 
-def sorted_widgets(
-    widgets: Iterable[NodeWidgetPair],
-) -> Tuple[Dict[int, NodeWidgetRow], NodeWidgetRow]:
-    """Return widgets in groups, ordered by priority and node path.
+        To be used by widgets that need direct access to files in the container.
+        """
+        if not self._flask_endpoint:
+            raise RuntimeError("missing flask endpoint!")
+        return f"{self._flask_endpoint}/file/{container_id}{node.name}"
 
-    Returns tuple with dict of groups and a remainder of ungrouped widgets.
-    """
+    # ----
+    # Functions making up the WidgetServer API
 
-    def nwp_group(tup: NodeWidgetPair) -> int:
-        return tup[1].group or 0
+    def index(self):
+        """Return information about current Metador environment.
 
-    def nwp_prio(tup: NodeWidgetPair) -> int:
-        return -tup[1].priority or 0  # in descending order of priority
+        Response includes an overview of metador-related Python packages,
+        Metador plugins, and the known widgets (nodes) and dashboards (containers).
+        """
+        from metador_core.plugin.types import to_ep_name
+        from metador_core.plugins import plugingroups
 
-    def sorted_group(ws: Iterable[NodeWidgetPair]) -> NodeWidgetRow:
-        """Sort first on priority, and for same priority on container node."""
-        return list(sorted(sorted(ws, key=lambda x: x[0].name), key=nwp_prio))
-
-    # dict, sorted in ascending group order (but ungrouped are 0)
-    ret = dict(
-        sorted(
-            {
-                k: sorted_group(v)
-                for k, v in groupby(sorted(widgets, key=nwp_group), key=nwp_group)
-            }.items()
+        # build dict with all available metador plugins
+        pgs = {to_ep_name(x.name, x.version): x.dict() for x in plugingroups.keys()}
+        groups = {plugingroups.Plugin.name: pgs}
+        for pg in plugingroups.values():
+            groups[pg.Plugin.name] = {
+                to_ep_name(x.name, x.version): x.dict() for x in pg.keys()
+            }
+
+        return {
+            "widgets": list(self._reg_widgets),
+            "dashboards": list(self._reg_dashboards),
+            "plugins": groups,
+        }
+
+    def download(self, container_id: str, container_path: str):
+        """Return file download stream of a file embedded in the container."""
+        node = self._get_container_node(container_id, container_path)
+        # get data out of container
+        obj = node[()]
+        bs = obj.tolist() if isinstance(obj, np.void) else obj
+        if not isinstance(bs, bytes):
+            raise BadRequest(f"Path not a bytes object: /{container_path}")
+
+        # construct a default file name based on path in container
+        def_name = f"{container_id}_{container_path.replace('/', '__')}"
+        # if object has attached file metadata, use it to serve data:
+        filemeta = node.meta.get("core.file")
+        name = filemeta.id_ if filemeta else def_name
+        mime = filemeta.encodingFormat if filemeta else None
+
+        # requested as explicit file download?
+        dl = bool(request.args.get("download", False))
+        # return file download stream with download metadata
+        return send_file(
+            io.BytesIO(bs), download_name=name, mimetype=mime, as_attachment=dl
         )
-    )
-    ungrp = ret.pop(0, [])  # separate out the ungrouped (were mapped to 0)
-    return ret, ungrp
-
-
-# ----
-
-
-def _resolve_schema(node: MetadorNode, wmeta: DashboardWidgetMeta) -> PluginRef:
-    """Return usable schema+version pair for the node based on widget metadata.
-
-    If a schema name or schema version is missing, will complete these values.
-
-    Usable schema means that:
-    * there exists a compatible installed schema
-    * there exists a compatible metadata object at given node
-
-    Raises ValueError on failure to find a suitable schema.
-    """
-    if wmeta.schema_name is None:
-        # if no schema selected -> pick any schema for which we have:
-        #   * a schema instance at the current node
-        #   * installed widget(s) that support it
-        for obj_schema in node.meta.query():
-            if next(widgets.widgets_for(obj_schema), None):
-                return obj_schema
-
-        msg = f"Cannot find suitable schema for a widget at node: {node.name}"
-        raise ValueError(msg)
-
-    # check that a node object is compatible with the one requested
-    req_ver = wmeta.schema_version if wmeta.schema_version else "any"
-    req_schema = f"{wmeta.schema_name} ({req_ver})"
-    s_ref = next(node.meta.query(wmeta.schema_name, wmeta.schema_version), None)
-    if s_ref is None:
-        msg = f"Dashboard wants metadata compatible with {req_schema}, but node"
-        if nrf := next(node.meta.query(wmeta.schema_name), None):
-            nobj_schema = f"{nrf.name} {nrf.version}"
-            msg += f"only has incompatible object: {nobj_schema}"
-        else:
-            msg += "has no suitable object"
-        raise ValueError(msg)
-
-    # if no version is specified, pick the one actually present at the node
-    version = wmeta.schema_version or s_ref.version
-    s_ref = schemas.PluginRef(name=wmeta.schema_name, version=version)
-
-    # ensure there is an installed schema compatible with the one requested
-    # (NOTE: if child schemas exist, the parents do too - no need to check)
-    installed_schema = schemas.get(s_ref.name, s_ref.version)
-    if installed_schema is None:
-        msg = f"No installed schema is compatible with {req_schema}"
-        raise ValueError(msg)
-
-    return s_ref
-
 
-def _widget_suitable_for(m_obj: MetadataSchema, w_ref: PluginRef) -> bool:
-    """Granular check whether the widget actually works with the metadata object.
-
-    Assumes that the passed object is known to be one of the supported schemas.
-    """
-    w_cls = widgets._get_unsafe(w_ref.name, w_ref.version)
-    return w_cls.Plugin.primary and w_cls.supports_meta(m_obj)
-
-
-def _resolve_widget(
-    node: MetadorNode,
-    s_ref: PluginRef,
-    w_name: Optional[str],
-    w_version: Optional[SemVerTuple],
-) -> PluginRef:
-    """Return suitable widget for the node based on given dashboard metadata."""
-    if w_name is None:
-        # get candidate widgets in alphabetic order (all that claim to work with schema)
-        cand_widgets = sorted(widgets.widgets_for(s_ref))
-        is_suitable = partial(_widget_suitable_for, node.meta[s_ref.name])
-        # filter out the ones that ACTUALLY can handle the object and are eligible
-        if w_ref := next(filter(is_suitable, cand_widgets), None):
-            return w_ref
-        else:
-            msg = f"Could not find suitable widget for {w_name} at node {node.name}"
-            raise ValueError(msg)
-
-    # now we have a widget name (and possibly version) - check it
-    widget_class = widgets._get_unsafe(w_name, w_version)
-    if widget_class is None:
-        raise ValueError(f"Could not find compatible widget: {w_name} {w_version}")
-    if not widget_class.supports(*schemas.parent_path(s_ref.name, s_ref.version)):
-        msg = f"Widget {widget_class.Plugin.ref()} does not support {s_ref}"
-        raise ValueError(msg)
-
-    w_ref = widget_class.Plugin.ref()
-    return w_ref
-
-
-# ----
-
-
-class Dashboard:
-    """The dashboard presents a view of all marked nodes in a container.
-
-    To be included in the dashboard, a node must be marked by a DashboardMeta
-    object that has show=True and contains possibly additional directives.
-    """
-
-    def __init__(self, container: MetadorContainer, *, server=None):
-        self._container: MetadorContainer = container
-        self._server = server
-
-        # figure out what schemas to show and what widgets to use and collect
-        ws: List[NodeWidgetPair] = []
-        for node, dbmeta in self._container.metador.query(DashboardMeta).items():
-            restr_node = node.restrict(read_only=True, local_only=True)
-            for wmeta in dbmeta.widgets:
-                ws.append((restr_node, self._resolve_node(node, wmeta)))
-
-        grps, ungrp = sorted_widgets(ws)
-        self._groups = grps
-        self._ungrouped = ungrp
-
-    def _resolve_node(
-        self, node: MetadorNode, wmeta: DashboardWidgetMeta
-    ) -> DashboardWidgetMeta:
-        """Check and resolve widget dashboard metadata for a node."""
-        wmeta = wmeta.copy()  # use copy, abandon original
-
-        s_ref: PluginRef = _resolve_schema(node, wmeta)
-        wmeta.schema_name = s_ref.name
-        wmeta.schema_version = s_ref.version
+    def get_script(
+        self,
+        viewable_type: Literal["widget", "dashboard"],
+        name: str,
+        container_id: str,
+        container_path: Optional[str] = None,
+    ) -> str:
+        """Return a script tag that will auto-load the desired widget for selected container."""
+        if not self._bokeh_endpoint:
+            raise RuntimeError("missing bokeh endpoint!")
+        if viewable_type == "dashboard" and container_path:
+            raise BadRequest("Dashboards do not accept a container path!")
+
+        return server_document(
+            f"{self._bokeh_endpoint}/{self._get_bokeh_widget_name(viewable_type, name)}",
+            arguments=self._make_widget_args(container_id, container_path),
+        )
 
-        w_ref: PluginRef = _resolve_widget(
-            node, s_ref, wmeta.widget_name, wmeta.widget_version
+    def get_flask_blueprint(self, *args):
+        """Return a Flask blueprint with the Metador container and widget API."""
+        api = Blueprint(*args)
+
+        api.route("/")(self.index)
+        api.route("/file/<container_id>/<path:container_path>")(self.download)
+        api.route("/<viewable_type>/<name>/<container_id>/")(
+            api.route("/<viewable_type>/<name>/<container_id>/<path:container_path>")(
+                self.get_script
+            )
         )
-        wmeta.widget_name = w_ref.name
-        wmeta.widget_version = w_ref.version
 
-        return wmeta
+        return api
 
-    def show(self) -> Viewable:
-        """Instantiate widgets for container and return resulting dashboard."""
-        w_width, w_height = 640, 480  # max size of a widget tile
-        db_height = int(3.5 * w_height)  # max size of the dashboard
-        db_width = int(2.5 * w_width)
-
-        # Outermost element: The Dashboard is a column of widget groups
-        db = pn.Column(scroll=True, height=db_height, width=db_width)
-
-        # helper, to fill widget instances into row or flexbox
-        def add_widgets(w_grp, ui_row):
-            for node, wmeta in w_grp:
-                w_cls = widgets.get(wmeta.widget_name, wmeta.widget_version)
-                label = pn.pane.Str(f"{node.name}:")
-                w_obj = w_cls(
-                    node,
-                    wmeta.schema_name,
-                    wmeta.schema_version,
-                    server=self._server,
-                    max_width=w_width,
-                    max_height=w_height,
-                )
-                ui_row.append(pn.Column(label, w_obj.show()))
-            return ui_row
-
-        # instantiate each widget group as row (those are non-wrapping)
-        for widget_group in self._groups.values():
-            db.append(
-                add_widgets(
-                    widget_group,
-                    pn.Row(width=db_width, height=int(1.2 * w_height), scroll=True),
-                )
-            )
-        # dump remaining ungrouped widgets into flexbox (auto-wrapping)
-        db.append(add_widgets(self._ungrouped, pn.FlexBox()))
-        return db
+
+# NOTE: snippet to make script tag not evaluate by default
+# it can be used to prevent the auto-loading during DOM injection, if needed for some reason
+#     # disable self-evaluation (save call in variable, call when requested)
+#     sc_id = re.match(r"\s*<script id=\"(.*)\">", script).group(1)
+#     script = script.replace("(function", f"w{sc_id} = (function").replace(
+#         "})();", "});"
+#     )
+#     return f'{script}<button type="button" onclick="w{sc_id}()">Load widget</button>'
```

### Comparing `metador_core-0.0.2/metador_core/widget/jupyter/standalone.py` & `metador_core-0.1.0/src/metador_core/widget/jupyter/standalone.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""
-Ad-hoc standalone dashboard/widget server for use within Jupyter notebooks.
+"""Ad-hoc standalone dashboard/widget server for use within Jupyter notebooks.
 
-Runs everything needed to see a dashboard or widget in threads.
+It runs everything needed to see a dashboard or widget in threads.
 
 This is mostly intended for convenient local use (e.g. by a researcher),
 or could be adapted for a containerized (in the Docker-sense) environment, e.g.
 where the user has metador libraries available and can inspect containers.
+
+**Do not use this to deploy a widget server backing the widgets on a website.**
 """
 import logging
 import socket
 from threading import Thread
 from typing import List, Optional
-from uuid import UUID
 
 import panel as pn
 from flask import Flask
 
 from ...container.provider import SimpleContainerProvider
 from ..server import WidgetServer
 
@@ -41,23 +41,23 @@
 # this should be not a problem ("serious" servers are implemented elsewhere!).
 
 DEFAULT_PANEL_EXTS = ["ace"]
 
 host: str = "127.0.0.1"
 port: int = -1
 
-_known_containers: SimpleContainerProvider[UUID] = SimpleContainerProvider[UUID]()
+_known_containers: SimpleContainerProvider[str] = SimpleContainerProvider[str]()
 _widget_server: WidgetServer = WidgetServer(_known_containers)
 
 
 def widget_server() -> WidgetServer:
     return _widget_server
 
 
-def container_provider() -> SimpleContainerProvider[UUID]:
+def container_provider() -> SimpleContainerProvider[str]:
     return _known_containers
 
 
 def running() -> bool:
     return port > 0
 
 
@@ -79,16 +79,16 @@
     def run_bokeh():
         _widget_server.run(
             host=host, port=bokeh_port, allowed_websocket_origin=[f"{host}:{port}"]
         )
 
     # prepare flask server
     flask_app = Flask(__name__)
-    _widget_server.set_bokeh_endpoint(bokeh_base)
-    _widget_server.set_flask_endpoint(flask_base)
+    _widget_server.bokeh_endpoint = bokeh_base
+    _widget_server.flask_endpoint = flask_base
     flask_bokeh = _widget_server.get_flask_blueprint("widget-api", __name__)
     flask_app.register_blueprint(flask_bokeh)
 
     def run_flask():
         flask_app.run(host=host, port=port)
 
     # launch
```

### Comparing `metador_core-0.0.2/PKG-INFO` & `metador_core-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,153 +1,149 @@
 Metadata-Version: 2.1
 Name: metador-core
-Version: 0.0.2
+Version: 0.1.0
 Summary: Core of Metador, the metadata-first research data management framework.
 Home-page: https://github.com/Materials-Data-Science-and-Informatics/metador-core
 License: MIT
-Keywords: metadata,rdm,FAIR,framework
+Keywords: metadata,rdm,FAIR,framework,python
 Author: Anton Pirogov
 Author-email: a.pirogov@fz-juelich.de
+Maintainer: Anton Pirogov
+Maintainer-email: a.pirogov@fz-juelich.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Typing :: Typed
 Requires-Dist: Flask (>=2.1.3,<3.0.0)
 Requires-Dist: Pillow (>=9.1.1,<10.0.0)
-Requires-Dist: Pint (>=0.18,<0.19)
-Requires-Dist: frozendict (>=2.3.4,<3.0.0)
-Requires-Dist: h5py (>=3.6.0,<4.0.0)
+Requires-Dist: Pint (>=0.21,<0.22)
+Requires-Dist: h5py (>=3.8.0,<4.0.0)
 Requires-Dist: importlib-metadata (>=4.11.4,<5.0.0)
 Requires-Dist: isodate (>=0.6.1,<0.7.0)
-Requires-Dist: jsonschema (>=4.4.0,<5.0.0)
 Requires-Dist: overrides (>=7.0.0,<8.0.0)
 Requires-Dist: pandas (>=1.4.1,<2.0.0)
 Requires-Dist: panel (>=0.14.0,<0.15.0)
-Requires-Dist: phantom-types (>=0.17.1,<0.18.0)
-Requires-Dist: pydantic (>=1.10.2,<2.0.0)
-Requires-Dist: pydantic-yaml[ruamel] (>=0.6.3,<0.7.0)
+Requires-Dist: phantom-types (>=2.1.0,<3.0.0)
+Requires-Dist: pydantic (>=1.10.12,<2.0.0)
+Requires-Dist: pydantic-yaml (>=1.1.1,<2.0.0)
 Requires-Dist: python-magic (>=0.4.25,<0.5.0)
+Requires-Dist: rdflib (>=6.2.0,<7.0.0)
+Requires-Dist: runtype (>=0.3.5,<0.4.0)
 Requires-Dist: simple-parsing (>=0.0.20,<0.0.21)
-Requires-Dist: toml (>=0.10.2,<0.11.0)
-Requires-Dist: typing-extensions (>=4.1.1,<5.0.0)
-Requires-Dist: typing-utils (>=0.1.0,<0.2.0)
+Requires-Dist: typing-extensions (>=4.6.0,<5.0.0)
 Requires-Dist: wrapt (>=1.14.1,<2.0.0)
 Project-URL: Documentation, https://github.com/Materials-Data-Science-and-Informatics/metador-core
 Project-URL: Repository, https://github.com/Materials-Data-Science-and-Informatics/metador-core
 Description-Content-Type: text/markdown
 
-# metador-core
-
-![Project status](https://img.shields.io/badge/project%20status-alpha-%23ff8000)
 [
-![Test](https://img.shields.io/github/workflow/status/Materials-Data-Science-and-Informatics/metador-core/test?label=test)
-](https://github.com/Materials-Data-Science-and-Informatics/metador-core/actions?query=workflow:test)
+![Docs](https://img.shields.io/badge/read-docs-success)
+](https://materials-data-science-and-informatics.github.io/metador-core)
+[
+![CI](https://img.shields.io/github/actions/workflow/status/Materials-Data-Science-and-Informatics/metador-core/ci.yml?branch=main&label=ci)
+](https://github.com/Materials-Data-Science-and-Informatics/metador-core/actions/workflows/ci.yml)
 [
-![Coverage](https://img.shields.io/codecov/c/gh/Materials-Data-Science-and-Informatics/metador-core?token=4JU2SZFZDZ)
-](https://app.codecov.io/gh/Materials-Data-Science-and-Informatics/metador-core)
+![Test Coverage](https://materials-data-science-and-informatics.github.io/metador-core/main/coverage_badge.svg)
+](https://materials-data-science-and-informatics.github.io/metador-core/main/coverage)
 [
-![Docs](https://img.shields.io/badge/read-docs-success)
-](https://materials-data-science-and-informatics.github.io/metador-core/)
+![PyPIPkgVersion](https://img.shields.io/pypi/v/metador-core)
+](https://pypi.org/project/metador-core/)
+[
+![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7174/badge)
+](https://bestpractices.coreinfrastructure.org/projects/7174)
 
-Core library of the Metador platform. It provides:
+<!-- --8<-- [start:abstract] -->
+# metador-core
+
+The core library of the Metador framework. It provides:
 
 * an interface for managing structured and validated metadata (`MetadorContainer`)
 * an API to manage immutable (but still "patchable") HDF5 files (`IH5Record`)
-* an extensible entry-points based plugin system defining plugin groups and plugins
-* core plugin group interfaces (schemas, packers, widgets, ...)
-* general semantically aligned schemas that should be used and extended
+* an extensible entry-points based plugin system for defining plugin groups and plugins
+* core plugin group types and interfaces (schemas, packers, widgets, ...)
+* general semantically aligned schemas that can be used and extended
 * visualization widgets for common data types based on Bokeh and Panel
 * generic dashboard presenting (meta)data for which suitable widgets are installed
 
-## Getting Started
+<!-- --8<-- [end:abstract] -->
+<!-- --8<-- [start:quickstart] -->
 
-This library is not a batteries-included solution, it is intended for people interested in
-using and extending the Metador ecosystem and who are willing to write their own plugins
-to adapt Metador to their use-case and provide services based on it.
-
-Please check out the tutorials that explain general concepts,
-interfaces and specific plugin development topics are provided [here](./tutorial).
-
-For a first taste, you can install this package just as any other package into your
-current Python environment using:
-
-<!--
-old install link based on https:
-metador-core@git+https://github.com/Materials-Data-Science-and-Informatics/metador-core.git
--->
+## Installation
+
+You can install the current stable version of Metador from PyPI:
 
 ```
-$ pip install git+ssh://git@github.com:Materials-Data-Science-and-Informatics/metador-core.git
+pip install metador-core
 ```
 
-or if you are adding it as a dependency into your poetry project:
+## Getting Started
 
-```
-$ poetry add git+ssh://git@github.com:Materials-Data-Science-and-Informatics/metador-core.git
-```
+If you successfully installed the package, check out the
+[tutorial notebooks](https://materials-data-science-and-informatics.github.io/metador-core/main/notebooks/about/).
 
-As usual, it is highly recommended that you use a
-[virtual environment](https://stackoverflow.com/questions/41573587/what-is-the-difference-between-venv-pyvenv-pyenv-virtualenv-virtualenvwrappe)
-to ensure isolation of dependencies between unrelated projects.
+These are intended to showcase what Metador has to offer and get you started with usage
+and development of your own schemas, widgets or other plugins.
 
-If you want to write or extend plugins, such as metadata schemas or widgets,
-the provided tutorials will get you started.
+To explore the notebooks interactively, clone this repo, install it, and then run:
 
-If you want to contribute to the actual core, see further below.
+```
+pip install notebook
+jupyter notebook ./docs/notebooks
+```
 
-## Compatibility and Known Issues
+You can use the
+[metador-extension-cookiecutter](https://github.com/Materials-Data-Science-and-Informatics/metador-extension-cookiecutter)
+template to generate a well-structured Python package repository that you can use to
+quickly get started with Metador plugin development.
 
-This package supports Python `>=3.8`.
+## Compatibility and Known Issues
 
-There was a mysterious bug when using inside Jupyter `6.4.6`,
-but there are no known problems when upgrading to Jupyter `6.4.10`.
+Currently this package supports Python `>=3.8`.
 
-If you encounter any problems, ensure that your bug is reproducible in a simple and
-minimal standalone Python script that is runnable in a venv with this package installed
-and can demonstrate your issue.
+We will try to support all still officially updated versions of Python,
+unless forced to drop it for technical reasons.
 
-## Development
+<!-- --8<-- [end:quickstart] -->
 
-This project uses [Poetry](https://python-poetry.org/) for dependency
-management, so you will need to have poetry
-[installed](https://python-poetry.org/docs/master/#installing-with-the-official-installer)
-in order to contribute.
+**You can find more information on using and contributing to this repository in the
+[documentation](https://materials-data-science-and-informatics.github.io/metador-core/main).**
 
-Then you can run the following lines to setup the project and install the package:
-```
-$ git clone git@github.com:Materials-Data-Science-and-Informatics/metador-core.git
-$ cd metador-core
-$ poetry install
-```
+<!-- --8<-- [start:citation] -->
 
-Run `pre-commit install` (see [https://pre-commit.com](https://pre-commit.com))
-after cloning. This enables pre-commit to enforce the required linting hooks.
+## How to Cite
 
-Run `pytest` (see [https://docs.pytest.org](https://docs.pytest.org)) before
-merging your changes to make sure you did not break anything. To check
-coverage, use `pytest --cov`.
+If you want to cite this project in your scientific work,
+please use the [citation file](https://citation-file-format.github.io/)
+in the [repository](https://github.com/Materials-Data-Science-and-Informatics/metador-core/blob/main/CITATION.cff).
 
-To generate local documentation (as the one linked above), run
-`pdoc -o docs metador_core` (see [https://pdoc.dev](https://pdoc.dev)).
+<!-- --8<-- [end:citation] -->
+<!-- --8<-- [start:acknowledgements] -->
 
 ## Acknowledgements
 
+We kindly thank all
+[authors and contributors](https://materials-data-science-and-informatics.github.io/metador-core/latest/credits).
+
 <div>
 <img style="vertical-align: middle;" alt="HMC Logo" src="https://github.com/Materials-Data-Science-and-Informatics/Logos/raw/main/HMC/HMC_Logo_M.png" width=50% height=50% />
 &nbsp;&nbsp;
 <img style="vertical-align: middle;" alt="FZJ Logo" src="https://github.com/Materials-Data-Science-and-Informatics/Logos/raw/main/FZJ/FZJ.png" width=30% height=30% />
 </div>
 <br />
 
 This project was developed at the Institute for Materials Data Science and Informatics
 (IAS-9) of the Jülich Research Center and funded by the Helmholtz Metadata Collaboration
 (HMC), an incubator-platform of the Helmholtz Association within the framework of the
 Information and Data Science strategic initiative.
 
+<!-- --8<-- [end:acknowledgements] -->
+
```

