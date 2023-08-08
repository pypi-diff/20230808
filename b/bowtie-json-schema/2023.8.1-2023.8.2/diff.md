# Comparing `tmp/bowtie_json_schema-2023.8.1.tar.gz` & `tmp/bowtie_json_schema-2023.8.2.tar.gz`

## Comparing `bowtie_json_schema-2023.8.1.tar` & `bowtie_json_schema-2023.8.2.tar`

### file list

```diff
@@ -1,83 +1,84 @@
--rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/.readthedocs.yaml
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/action.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/io-schema.json -> bowtie/schemas/io-schema.json
--rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/noxfile.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/test-requirements.in
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/test-requirements.txt
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/.github/SECURITY.md
--rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/.github/release.yml
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/.github/workflows/build-frontend.yml
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/.github/workflows/dependabot-merge.yml
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/.github/workflows/deploy-frontend.yml
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/.github/workflows/documentation-links.yml
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/.github/workflows/images.yml
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/.github/workflows/report.yml
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/bowtie/__init__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/bowtie/__main__.py
--rw-r--r--   0        0        0    32694 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/bowtie/_cli.py
--rw-r--r--   0        0        0     8673 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/bowtie/_commands.py
--rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/bowtie/_core.py
--rw-r--r--   0        0        0    13733 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/bowtie/_report.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/bowtie/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/bowtie/schemas/__init__.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/docs/Makefile
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/docs/cli.rst
--rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/docs/conf.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/docs/contributing.rst
--rw-r--r--   0        0        0    34142 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/docs/implementers.rst
--rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/docs/index.rst
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/docs/requirements.in
--rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/docs/requirements.txt
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0   629179 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/docs/_static/dreamed.png
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/.eslintrc.js
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/index.html
--rw-r--r--   0        0        0   165159 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/package-lock.json
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/package.json
--rw-r--r--   0        0        0    93868 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/pnpm-lock.yaml
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/tsconfig.json
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/vite.config.js
--rw-r--r--   0        0        0   130217 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/public/favicon.ico
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/MainContainer.jsx
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/ReportDataHandler.jsx
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/ReportView.jsx
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/index.jsx
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/components/CopyToClipboard.jsx
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/components/LoadingAnimation.jsx
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/components/NavBar.jsx
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/components/Cases/AccordionItem.jsx
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/components/Cases/AccordionSvg.jsx
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/components/Cases/CasesSection.jsx
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/components/Cases/SchemaDisplay.jsx
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/components/DragAndDrop/DragAndDrop.css
--rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/components/DragAndDrop/DragAndDrop.jsx
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/components/Modals/DetailsButtonModal.jsx
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/components/Modals/RunTimeInfoModal.jsx
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/components/RunInfo/RunInfoSection.jsx
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/components/Summary/ImplementationRow.css
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/components/Summary/ImplementationRow.jsx
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/components/Summary/SummarySection.jsx
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/components/Summary/SummaryTable.jsx
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/context/BowtieVersionContext.jsx
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/context/ThemeContext.jsx
--rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/frontend/src/data/parseReportData.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/tests/__init__.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/tests/conftest.py
--rw-r--r--   0        0        0    23976 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/tests/test_integration.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/tests/fauxmplementations/badsonschema/Dockerfile
--rwxr-xr-x   0        0        0     1832 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/tests/fauxmplementations/badsonschema/badsonschema
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/tests/fauxmplementations/envsonschema/Dockerfile
--rwxr-xr-x   0        0        0     4529 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/tests/fauxmplementations/envsonschema/envsonschema
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/tests/fauxmplementations/lintsonschema/Dockerfile
--rw-r--r--   0        0        0    12345 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/tests/fauxmplementations/lintsonschema/io-schema.json
--rwxr-xr-x   0        0        0     3190 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/tests/fauxmplementations/lintsonschema/lintsonschema
--rw-r--r--   0        0        0    28309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/bowtie/templates/report.html.j2
--rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/bowtie/schemas/io-schema.json
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/LICENSE
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/README.rst
--rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/pyproject.toml
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.1/PKG-INFO
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/.non-pre-commit-ci.yaml
+-rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/.readthedocs.yaml
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/action.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/io-schema.json -> bowtie/schemas/io-schema.json
+-rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/noxfile.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/test-requirements.in
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/test-requirements.txt
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/.github/SECURITY.md
+-rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/.github/release.yml
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/.github/workflows/build-frontend.yml
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/.github/workflows/dependabot-merge.yml
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/.github/workflows/deploy-frontend.yml
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/.github/workflows/documentation-links.yml
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/.github/workflows/images.yml
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/.github/workflows/report.yml
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/bowtie/__init__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/bowtie/__main__.py
+-rw-r--r--   0        0        0    32694 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/bowtie/_cli.py
+-rw-r--r--   0        0        0     8673 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/bowtie/_commands.py
+-rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/bowtie/_core.py
+-rw-r--r--   0        0        0    13733 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/bowtie/_report.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/bowtie/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/bowtie/schemas/__init__.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/docs/Makefile
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/docs/cli.rst
+-rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/docs/conf.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/docs/contributing.rst
+-rw-r--r--   0        0        0    34142 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/docs/implementers.rst
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/docs/index.rst
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/docs/requirements.in
+-rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/docs/requirements.txt
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0   629179 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/docs/_static/dreamed.png
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/frontend/.eslintrc.js
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/frontend/index.html
+-rw-r--r--   0        0        0   165765 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/frontend/package-lock.json
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/frontend/package.json
+-rw-r--r--   0        0        0    93868 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/frontend/pnpm-lock.yaml
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/frontend/tsconfig.json
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/frontend/vite.config.js
+-rw-r--r--   0        0        0   130217 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/frontend/public/favicon.ico
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/frontend/src/MainContainer.jsx
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/frontend/src/ReportDataHandler.jsx
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/frontend/src/ReportView.jsx
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/frontend/src/index.jsx
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/frontend/src/components/CopyToClipboard.jsx
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/frontend/src/components/LoadingAnimation.jsx
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/frontend/src/components/NavBar.jsx
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/frontend/src/components/Cases/AccordionItem.jsx
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/frontend/src/components/Cases/AccordionSvg.jsx
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/frontend/src/components/Cases/CasesSection.jsx
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/frontend/src/components/Cases/SchemaDisplay.jsx
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/frontend/src/components/DragAndDrop/DragAndDrop.css
+-rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/frontend/src/components/DragAndDrop/DragAndDrop.jsx
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/frontend/src/components/Modals/DetailsButtonModal.jsx
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/frontend/src/components/Modals/RunTimeInfoModal.jsx
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/frontend/src/components/RunInfo/RunInfoSection.jsx
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/frontend/src/components/Summary/ImplementationRow.css
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/frontend/src/components/Summary/ImplementationRow.jsx
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/frontend/src/components/Summary/SummarySection.jsx
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/frontend/src/components/Summary/SummaryTable.jsx
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/frontend/src/context/BowtieVersionContext.jsx
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/frontend/src/context/ThemeContext.jsx
+-rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/frontend/src/data/parseReportData.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/tests/__init__.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/tests/conftest.py
+-rw-r--r--   0        0        0    23976 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/tests/test_integration.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/tests/fauxmplementations/badsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     1832 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/tests/fauxmplementations/badsonschema/badsonschema
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/tests/fauxmplementations/envsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     4529 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/tests/fauxmplementations/envsonschema/envsonschema
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/tests/fauxmplementations/lintsonschema/Dockerfile
+-rw-r--r--   0        0        0    12345 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/tests/fauxmplementations/lintsonschema/io-schema.json
+-rwxr-xr-x   0        0        0     3190 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/tests/fauxmplementations/lintsonschema/lintsonschema
+-rw-r--r--   0        0        0    28309 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/bowtie/templates/report.html.j2
+-rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/bowtie/schemas/io-schema.json
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/LICENSE
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/README.rst
+-rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/pyproject.toml
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 bowtie_json_schema-2023.8.2/PKG-INFO
```

### Comparing `bowtie_json_schema-2023.8.1/.pre-commit-config.yaml` & `bowtie_json_schema-2023.8.2/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -17,29 +17,29 @@
     hooks:
       - id: isort
   - repo: https://github.com/asottile/pyupgrade
     rev: v3.10.1
     hooks:
       - id: pyupgrade
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.0.281"
+    rev: "v0.0.282"
     hooks:
       - id: ruff
   - repo: https://github.com/Riverside-Healthcare/djLint
     rev: v1.32.1
     hooks:
       - id: djlint-jinja
   - repo: https://github.com/psf/black
     rev: 23.7.0
     hooks:
       - name: black (python implementations & bowtie internals)
         id: black
         args: ["--line-length", "79"]
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v3.0.0"
+    rev: "v3.0.1"
     hooks:
       - name: prettier (javascript implementations & bowtie internals)
         exclude: frontend/pnpm-lock.yaml
         id: prettier
   - repo: https://github.com/doublify/pre-commit-rust
     rev: "v1.0"
     hooks:
@@ -88,7 +88,26 @@
         id: eslint
         files: ^frontend/src/.*\.jsx?$
         types: [file]
         additional_dependencies:
           - eslint@8.43.0
           - eslint-plugin-react@7.32.2
           - eslint-plugin-react-hooks@4.6.0
+  - repo: https://github.com/dustinsand/pre-commit-jvm
+    rev: v0.8.0
+    hooks:
+      - name: ktlint
+        id: ktlint
+        args:
+          [
+            "--format",
+            "implementations/kotlin-kmp-json-schema-validator/**/*.kt",
+            "implementations/kotlin-kmp-json-schema-validator/*.kts",
+          ]
+      - name: detekt
+        id: detekt
+        args:
+          [
+            "--build-upon-default-config",
+            "--input",
+            "implementations/kotlin-kmp-json-schema-validator",
+          ]
```

### Comparing `bowtie_json_schema-2023.8.1/noxfile.py` & `bowtie_json_schema-2023.8.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/test-requirements.txt` & `bowtie_json_schema-2023.8.2/test-requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     # via
     #   aiohttp
     #   requests
 click==8.1.6
     # via
     #   bowtie-json-schema
     #   trogon
-cryptography==41.0.2
+cryptography==41.0.3
     # via pyjwt
 frozenlist==1.4.0
     # via
     #   aiohttp
     #   aiosignal
 github3-py==4.0.1
     # via bowtie-json-schema
@@ -48,15 +48,15 @@
     #   yarl
 importlib-metadata==6.8.0
     # via textual
 iniconfig==2.0.0
     # via pytest
 jinja2==3.1.2
     # via bowtie-json-schema
-jsonschema==4.18.4
+jsonschema==4.18.6
     # via bowtie-json-schema
 jsonschema-specifications==2023.7.1
     # via jsonschema
 linkify-it-py==2.0.2
     # via markdown-it-py
 markdown-it-py[linkify,plugins]==3.0.0
     # via
@@ -98,27 +98,27 @@
     # via github3-py
 referencing==0.30.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via github3-py
-rich==13.4.2
+rich==13.5.2
     # via
     #   bowtie-json-schema
     #   textual
 rpds-py==0.9.2
     # via
     #   jsonschema
     #   referencing
 six==1.16.0
     # via python-dateutil
 structlog==23.1.0
     # via bowtie-json-schema
-textual==0.30.0
+textual==0.31.0
     # via trogon
 trogon==0.5.0
     # via bowtie-json-schema
 typing-extensions==4.7.1
     # via
     #   aiodocker
     #   textual
```

### Comparing `bowtie_json_schema-2023.8.1/.github/SECURITY.md` & `bowtie_json_schema-2023.8.2/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/.github/dependabot.yml` & `bowtie_json_schema-2023.8.2/.github/dependabot.yml`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,19 @@
       interval: "daily"
 
   - package-ecosystem: "gradle"
     directory: "implementations/java-json-schema-validator"
     schedule:
       interval: "daily"
 
+  - package-ecosystem: "gradle"
+    directory: "implementations/kmp-json-schema-validator"
+    schedule:
+      interval: "daily"
+
   # Dependabot for Dockerfiles
   # --------------------------
 
   # See dependabot/dependabot-core#1015 or dependabot/dependabot-core#2178,
   # this doesn't happen automatically, so hooray, manual list.
 
   - package-ecosystem: "docker"
```

### Comparing `bowtie_json_schema-2023.8.1/.github/workflows/build-frontend.yml` & `bowtie_json_schema-2023.8.2/.github/workflows/build-frontend.yml`

 * *Files 12% similar despite different names*

```diff
@@ -14,13 +14,13 @@
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-node@v3
         with:
           node-version: 18.x
       - run: npm ci
         working-directory: ./frontend
-      - run: npm run build
+      - run: npm run build -- --base=${{ vars.BOWTIE_BASE_URL || '/bowtie' }}
         working-directory: ./frontend
       - uses: actions/upload-artifact@v3
         with:
           name: frontend-build
           path: frontend/build
```

### Comparing `bowtie_json_schema-2023.8.1/.github/workflows/ci.yml` & `bowtie_json_schema-2023.8.2/.github/workflows/ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -17,16 +17,18 @@
   pre-commit:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: "3.x"
-      - uses: pre-commit/action@v3.0.0
-
+      - name: Run pre-commit action
+        uses: pre-commit/action@v3.0.0
+        with:
+          extra_args: --config .non-pre-commit-ci.yaml --all-files
   list:
     runs-on: ubuntu-latest
     outputs:
       noxenvs: ${{ steps.noxenvs-matrix.outputs.noxenvs }}
     steps:
       - uses: actions/checkout@v3
       - name: Set up nox
```

### Comparing `bowtie_json_schema-2023.8.1/.github/workflows/dependabot-merge.yml` & `bowtie_json_schema-2023.8.2/.github/workflows/dependabot-merge.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/.github/workflows/deploy-frontend.yml` & `bowtie_json_schema-2023.8.2/.github/workflows/deploy-frontend.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/.github/workflows/images.yml` & `bowtie_json_schema-2023.8.2/.github/workflows/images.yml`

 * *Files 1% similar despite different names*

```diff
@@ -83,13 +83,13 @@
           tags: ${{ steps.build_image.outputs.tags }}
           registry: ghcr.io/${{ github.repository_owner }}
           username: ${{ github.actor }}
           password: ${{ github.token }}
         if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags')
 
       - name: Install Bowtie
-        uses: bowtie-json-schema/bowtie@v2023.07.10
+        uses: bowtie-json-schema/bowtie@v2023.08.1
         if: steps.changes.outputs.impl == 'true' || (github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags'))
 
       - name: Smoke Test
         run: bowtie smoke -i "${{ steps.build_image.outputs.image-with-tag }}"
         if: steps.changes.outputs.impl == 'true' || (github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags'))
```

### Comparing `bowtie_json_schema-2023.8.1/.github/workflows/report.yml` & `bowtie_json_schema-2023.8.2/.github/workflows/report.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/bowtie/_cli.py` & `bowtie_json_schema-2023.8.2/bowtie/_cli.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/bowtie/_commands.py` & `bowtie_json_schema-2023.8.2/bowtie/_commands.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/bowtie/_core.py` & `bowtie_json_schema-2023.8.2/bowtie/_core.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/bowtie/_report.py` & `bowtie_json_schema-2023.8.2/bowtie/_report.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/bowtie/exceptions.py` & `bowtie_json_schema-2023.8.2/bowtie/exceptions.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/docs/Makefile` & `bowtie_json_schema-2023.8.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/docs/cli.rst` & `bowtie_json_schema-2023.8.2/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/docs/conf.py` & `bowtie_json_schema-2023.8.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/docs/contributing.rst` & `bowtie_json_schema-2023.8.2/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/docs/implementers.rst` & `bowtie_json_schema-2023.8.2/docs/implementers.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/docs/index.rst` & `bowtie_json_schema-2023.8.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/docs/requirements.txt` & `bowtie_json_schema-2023.8.2/docs/requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -37,23 +37,23 @@
 click==8.1.6
     # via
     #   bowtie-json-schema
     #   sphinx-click
     #   trogon
 contourpy==1.1.0
     # via matplotlib
-cryptography==41.0.2
+cryptography==41.0.3
     # via pyjwt
 cycler==0.11.0
     # via matplotlib
 docutils==0.20.1
     # via
     #   sphinx
     #   sphinx-click
-fonttools==4.41.1
+fonttools==4.42.0
     # via matplotlib
 frozenlist==1.4.0
     # via
     #   aiohttp
     #   aiosignal
 furo==2023.7.26
     # via -r docs/requirements.in
@@ -67,15 +67,15 @@
     # via sphinx
 importlib-metadata==6.8.0
     # via textual
 jinja2==3.1.2
     # via
     #   bowtie-json-schema
     #   sphinx
-jsonschema==4.18.4
+jsonschema==4.18.6
     # via bowtie-json-schema
 jsonschema-specifications==2023.7.1
     # via jsonschema
 kiwisolver==1.4.4
     # via matplotlib
 linkify-it-py==2.0.2
     # via markdown-it-py
@@ -94,15 +94,15 @@
     # via markdown-it-py
 mdurl==0.1.2
     # via markdown-it-py
 multidict==6.0.4
     # via
     #   aiohttp
     #   yarl
-numpy==1.25.1
+numpy==1.25.2
     # via
     #   contourpy
     #   matplotlib
 packaging==23.1
     # via
     #   matplotlib
     #   sphinx
@@ -132,29 +132,29 @@
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via
     #   github3-py
     #   sphinx
-rich==13.4.2
+rich==13.5.2
     # via
     #   bowtie-json-schema
     #   textual
 rpds-py==0.9.2
     # via
     #   jsonschema
     #   referencing
 six==1.16.0
     # via python-dateutil
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.4.1
     # via beautifulsoup4
-sphinx==7.1.1
+sphinx==7.1.2
     # via
     #   -r docs/requirements.in
     #   furo
     #   sphinx-basic-ng
     #   sphinx-click
     #   sphinx-copybutton
     #   sphinx-json-schema-spec
@@ -162,15 +162,15 @@
     #   sphinxext-opengraph
 sphinx-basic-ng==1.0.0b2
     # via furo
 sphinx-click==4.4.0
     # via -r docs/requirements.in
 sphinx-copybutton==0.5.2
     # via -r docs/requirements.in
-sphinx-json-schema-spec==2023.7.2
+sphinx-json-schema-spec==2023.8.1
     # via -r docs/requirements.in
 sphinxcontrib-applehelp==1.0.4
     # via sphinx
 sphinxcontrib-devhelp==1.0.2
     # via sphinx
 sphinxcontrib-htmlhelp==2.0.1
     # via sphinx
@@ -182,15 +182,15 @@
     # via sphinx
 sphinxcontrib-spelling==8.0.0
     # via -r docs/requirements.in
 sphinxext-opengraph==0.8.2
     # via -r docs/requirements.in
 structlog==23.1.0
     # via bowtie-json-schema
-textual==0.30.0
+textual==0.31.0
     # via trogon
 trogon==0.5.0
     # via bowtie-json-schema
 typing-extensions==4.7.1
     # via
     #   aiodocker
     #   textual
```

### Comparing `bowtie_json_schema-2023.8.1/docs/_static/dreamed.png` & `bowtie_json_schema-2023.8.2/docs/_static/dreamed.png`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/frontend/package-lock.json` & `bowtie_json_schema-2023.8.2/frontend/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994482020547946%*

 * *Differences: {"'packages'": "{'': {'dependencies': {'urijs': '^1.19.11'}, 'devDependencies': {'@types/urijs': "*

 * *               "'^1.19.19'}}, 'node_modules/@types/urijs': OrderedDict([('version', '1.19.19'), "*

 * *               "('resolved', 'https://registry.npmjs.org/@types/urijs/-/urijs-1.19.19.tgz'), "*

 * *               "('integrity', "*

 * *               "'sha512-FDJNkyhmKLw7uEvTxx5tSXfPeQpO0iy73Ry+PmYZJvQy0QIWX8a7kJ4kLWRf+EbTPJEPDSgPXHaM7pzr5lmvCg=='), "*

 * *               "('dev', True)]), 'node_modules/urijs': OrderedDict([(' […]*

```diff
@@ -6,19 +6,21 @@
             "dependencies": {
                 "bootstrap": "^5.3.0",
                 "moment": "^2.29.4",
                 "react": "^18.2.0",
                 "react-bootstrap": "^2.8.0",
                 "react-bootstrap-icons": "^1.10.3",
                 "react-dom": "^18.2.0",
-                "react-router-dom": "^6.14.1"
+                "react-router-dom": "^6.14.1",
+                "urijs": "^1.19.11"
             },
             "devDependencies": {
                 "@types/react": "^18.2.14",
                 "@types/react-dom": "^18.2.6",
+                "@types/urijs": "^1.19.19",
                 "@vitejs/plugin-react": "^4.0.3",
                 "eslint": "8.43.0",
                 "eslint-plugin-react": "7.32.2",
                 "eslint-plugin-react-hooks": "4.6.0",
                 "ts-loader": "^9.4.4",
                 "typescript": "^5.1.6",
                 "vite": "^4.4.2"
@@ -1104,14 +1106,20 @@
             "version": "4.4.6"
         },
         "node_modules/@types/scheduler": {
             "integrity": "sha512-5cJ8CB4yAx7BH1oMvdU0Jh9lrEXyPkar6F9G/ERswkCuvP4KQZfZkSjcMbAICCpQTN4OuZn8tz0HiKv9TGZgrQ==",
             "resolved": "https://registry.npmjs.org/@types/scheduler/-/scheduler-0.16.3.tgz",
             "version": "0.16.3"
         },
+        "node_modules/@types/urijs": {
+            "dev": true,
+            "integrity": "sha512-FDJNkyhmKLw7uEvTxx5tSXfPeQpO0iy73Ry+PmYZJvQy0QIWX8a7kJ4kLWRf+EbTPJEPDSgPXHaM7pzr5lmvCg==",
+            "resolved": "https://registry.npmjs.org/@types/urijs/-/urijs-1.19.19.tgz",
+            "version": "1.19.19"
+        },
         "node_modules/@types/warning": {
             "integrity": "sha512-t/Tvs5qR47OLOr+4E9ckN8AmP2Tf16gWq+/qA4iUGS/OOyHVO8wv2vjJuX8SNOUTJyWb+2t7wJm6cXILFnOROA==",
             "resolved": "https://registry.npmjs.org/@types/warning/-/warning-3.0.0.tgz",
             "version": "3.0.0"
         },
         "node_modules/@vitejs/plugin-react": {
             "dependencies": {
@@ -4339,14 +4347,19 @@
                 "punycode": "^2.1.0"
             },
             "dev": true,
             "integrity": "sha512-7rKUyy33Q1yc98pQ1DAmLtwX109F7TIfWlW1Ydo8Wl1ii1SeHieeh0HHfPeL2fMXK6z0s8ecKs9frCuLJvndBg==",
             "resolved": "https://registry.npmjs.org/uri-js/-/uri-js-4.4.1.tgz",
             "version": "4.4.1"
         },
+        "node_modules/urijs": {
+            "integrity": "sha512-HXgFDgDommxn5/bIv0cnQZsPhHDA90NPHD6+c/v21U5+Sx5hoP8+dP9IZXBU1gIfvdRfhG8cel9QNPeionfcCQ==",
+            "resolved": "https://registry.npmjs.org/urijs/-/urijs-1.19.11.tgz",
+            "version": "1.19.11"
+        },
         "node_modules/vite": {
             "bin": {
                 "vite": "bin/vite.js"
             },
             "dependencies": {
                 "esbuild": "^0.18.10",
                 "postcss": "^8.4.24",
```

### Comparing `bowtie_json_schema-2023.8.1/frontend/pnpm-lock.yaml` & `bowtie_json_schema-2023.8.2/frontend/pnpm-lock.yaml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/frontend/public/favicon.ico` & `bowtie_json_schema-2023.8.2/frontend/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/frontend/src/ReportDataHandler.jsx` & `bowtie_json_schema-2023.8.2/frontend/src/ReportDataHandler.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/frontend/src/index.jsx` & `bowtie_json_schema-2023.8.2/frontend/src/index.jsx`

 * *Files 5% similar despite different names*

```diff
@@ -5,30 +5,37 @@
 import ReportDataHandler from "./ReportDataHandler";
 import { createHashRouter, RouterProvider } from "react-router-dom";
 import ThemeContextProvider from "./context/ThemeContext";
 import { MainContainer } from "./MainContainer";
 import { BowtieVersionContextProvider } from "./context/BowtieVersionContext";
 import { DragAndDrop } from "./components/DragAndDrop/DragAndDrop";
 import { parseReportData } from "./data/parseReportData";
+import URI from "urijs";
+
+const reportHost =
+  import.meta.env.MODE === "development"
+    ? "https://bowtie.report"
+    : window.location.href;
+const reportUri = new URI(reportHost).directory(import.meta.env.BASE_URL);
 
-const reportUrl = "https://bowtie.report";
 const titleTag = document.getElementsByTagName("title")[0];
 const dialectToName = {
   "draft2020-12": "Draft 2020-12",
   "draft2019-09": "Draft 2019-09",
   draft7: "Draft 7",
   draft6: "Draft 6",
   draft4: "Draft 4",
   draft3: "Draft 3",
 };
 
 const fetchReportData = async (dialect) => {
   const dialectName = dialectToName[dialect] ?? dialect;
   titleTag.textContent = `Bowtie - ${dialectName}`;
-  const response = await fetch(`${reportUrl}/${dialect}.json`);
+  const url = reportUri.clone().filename(dialect).suffix("json").href();
+  const response = await fetch(url);
   const jsonl = await response.text();
   const lines = jsonl
     .trim()
     .split(/\r?\n/)
     .map((line) => JSON.parse(line));
   return parseReportData(lines);
 };
```

### Comparing `bowtie_json_schema-2023.8.1/frontend/src/components/CopyToClipboard.jsx` & `bowtie_json_schema-2023.8.2/frontend/src/components/CopyToClipboard.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/frontend/src/components/LoadingAnimation.jsx` & `bowtie_json_schema-2023.8.2/frontend/src/components/LoadingAnimation.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/frontend/src/components/NavBar.jsx` & `bowtie_json_schema-2023.8.2/frontend/src/components/NavBar.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/frontend/src/components/Cases/AccordionItem.jsx` & `bowtie_json_schema-2023.8.2/frontend/src/components/Cases/AccordionItem.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/frontend/src/components/Cases/AccordionSvg.jsx` & `bowtie_json_schema-2023.8.2/frontend/src/components/Cases/AccordionSvg.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/frontend/src/components/Cases/CasesSection.jsx` & `bowtie_json_schema-2023.8.2/frontend/src/components/Cases/CasesSection.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/frontend/src/components/Cases/SchemaDisplay.jsx` & `bowtie_json_schema-2023.8.2/frontend/src/components/Cases/SchemaDisplay.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/frontend/src/components/DragAndDrop/DragAndDrop.jsx` & `bowtie_json_schema-2023.8.2/frontend/src/components/DragAndDrop/DragAndDrop.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/frontend/src/components/Modals/DetailsButtonModal.jsx` & `bowtie_json_schema-2023.8.2/frontend/src/components/Modals/DetailsButtonModal.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/frontend/src/components/Modals/RunTimeInfoModal.jsx` & `bowtie_json_schema-2023.8.2/frontend/src/components/Modals/RunTimeInfoModal.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/frontend/src/components/RunInfo/RunInfoSection.jsx` & `bowtie_json_schema-2023.8.2/frontend/src/components/RunInfo/RunInfoSection.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/frontend/src/components/Summary/ImplementationRow.css` & `bowtie_json_schema-2023.8.2/frontend/src/components/Summary/ImplementationRow.css`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/frontend/src/components/Summary/ImplementationRow.jsx` & `bowtie_json_schema-2023.8.2/frontend/src/components/Summary/ImplementationRow.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/frontend/src/components/Summary/SummarySection.jsx` & `bowtie_json_schema-2023.8.2/frontend/src/components/Summary/SummarySection.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/frontend/src/components/Summary/SummaryTable.jsx` & `bowtie_json_schema-2023.8.2/frontend/src/components/Summary/SummaryTable.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/frontend/src/context/ThemeContext.jsx` & `bowtie_json_schema-2023.8.2/frontend/src/context/ThemeContext.jsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/frontend/src/data/parseReportData.ts` & `bowtie_json_schema-2023.8.2/frontend/src/data/parseReportData.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/tests/test_integration.py` & `bowtie_json_schema-2023.8.2/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/tests/fauxmplementations/badsonschema/badsonschema` & `bowtie_json_schema-2023.8.2/tests/fauxmplementations/badsonschema/badsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/tests/fauxmplementations/envsonschema/envsonschema` & `bowtie_json_schema-2023.8.2/tests/fauxmplementations/envsonschema/envsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/tests/fauxmplementations/lintsonschema/io-schema.json` & `bowtie_json_schema-2023.8.2/tests/fauxmplementations/lintsonschema/io-schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/tests/fauxmplementations/lintsonschema/lintsonschema` & `bowtie_json_schema-2023.8.2/tests/fauxmplementations/lintsonschema/lintsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/bowtie/templates/report.html.j2` & `bowtie_json_schema-2023.8.2/bowtie/templates/report.html.j2`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/bowtie/schemas/io-schema.json` & `bowtie_json_schema-2023.8.2/bowtie/schemas/io-schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/.gitignore` & `bowtie_json_schema-2023.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/LICENSE` & `bowtie_json_schema-2023.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/README.rst` & `bowtie_json_schema-2023.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/pyproject.toml` & `bowtie_json_schema-2023.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2023.8.1/PKG-INFO` & `bowtie_json_schema-2023.8.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bowtie-json-schema
-Version: 2023.8.1
+Version: 2023.8.2
 Summary: A meta-validator for the JSON Schema specification.
 Project-URL: Documentation, https://bowtie-json-schema.readthedocs.io/
 Project-URL: Homepage, https://github.com/bowtie-json-schema/bowtie
 Project-URL: Issues, https://github.com/bowtie-json-schema/bowtie/issues/
 Project-URL: Source, https://github.com/bowtie-json-schema/bowtie
 Author: Julian Berman
 Author-email: Julian+bowtie@GrayVines.com
```

