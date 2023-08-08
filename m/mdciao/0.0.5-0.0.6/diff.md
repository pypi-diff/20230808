# Comparing `tmp/mdciao-0.0.5.tar.gz` & `tmp/mdciao-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdciao-0.0.5.tar", last modified: Mon Jul 11 18:30:14 2022, max compression
+gzip compressed data, was "mdciao-0.0.6.tar", last modified: Tue Aug  8 14:37:48 2023, max compression
```

## Comparing `mdciao-0.0.5.tar` & `mdciao-0.0.6.tar`

### file list

```diff
@@ -1,97 +1,182 @@
-drwxrwxr-x   0 guille    (1000) guille    (1000)        0 2022-07-11 18:30:14.340096 mdciao-0.0.5/
--rw-rw-r--   0 guille    (1000) guille    (1000)     7652 2020-07-27 18:29:42.000000 mdciao-0.0.5/LICENSE.txt
--rw-rw-r--   0 guille    (1000) guille    (1000)     8874 2022-07-11 18:30:14.340096 mdciao-0.0.5/PKG-INFO
--rw-rw-r--   0 guille    (1000) guille    (1000)     8047 2022-07-11 15:28:50.000000 mdciao-0.0.5/README.rst
-drwxrwxr-x   0 guille    (1000) guille    (1000)        0 2022-07-11 18:30:14.332096 mdciao-0.0.5/mdciao/
--rw-rw-r--   0 guille    (1000) guille    (1000)      424 2022-06-11 17:35:24.000000 mdciao-0.0.5/mdciao/__init__.py
-drwxrwxr-x   0 guille    (1000) guille    (1000)        0 2022-07-11 18:30:14.332096 mdciao-0.0.5/mdciao/cli/
--rw-rw-r--   0 guille    (1000) guille    (1000)      247 2022-06-11 17:35:24.000000 mdciao-0.0.5/mdciao/cli/__init__.py
--rw-rw-r--   0 guille    (1000) guille    (1000)   108858 2022-07-11 15:28:50.000000 mdciao-0.0.5/mdciao/cli/cli.py
-drwxrwxr-x   0 guille    (1000) guille    (1000)        0 2022-07-11 18:30:14.332096 mdciao-0.0.5/mdciao/contacts/
--rw-rw-r--   0 guille    (1000) guille    (1000)     1115 2022-06-11 17:35:24.000000 mdciao-0.0.5/mdciao/contacts/__init__.py
--rw-rw-r--   0 guille    (1000) guille    (1000)    12939 2022-06-11 17:35:24.000000 mdciao-0.0.5/mdciao/contacts/_md_compute_contacts.py
--rw-rw-r--   0 guille    (1000) guille    (1000)   249790 2022-07-11 15:28:50.000000 mdciao-0.0.5/mdciao/contacts/contacts.py
--rw-rw-r--   0 guille    (1000) guille    (1000)    24459 2022-06-11 17:35:24.000000 mdciao-0.0.5/mdciao/dihedrals.py
-drwxrwxr-x   0 guille    (1000) guille    (1000)        0 2022-07-11 18:30:14.336096 mdciao-0.0.5/mdciao/examples/
--rw-rw-r--   0 guille    (1000) guille    (1000)    35957 2022-07-11 15:28:50.000000 mdciao-0.0.5/mdciao/examples/Comparing_CGs_Bars.ipynb
--rw-rw-r--   0 guille    (1000) guille    (1000)    38800 2022-07-11 15:28:50.000000 mdciao-0.0.5/mdciao/examples/Comparing_CGs_Flares.ipynb
--rw-rw-r--   0 guille    (1000) guille    (1000)    13581 2022-07-11 15:28:50.000000 mdciao-0.0.5/mdciao/examples/EGFR_Kinase_Inhibitors.ipynb
--rw-rw-r--   0 guille    (1000) guille    (1000)    24788 2022-07-11 15:28:50.000000 mdciao-0.0.5/mdciao/examples/Flareplot_Schemes.ipynb
--rw-rw-r--   0 guille    (1000) guille    (1000)     7053 2022-07-11 15:28:50.000000 mdciao-0.0.5/mdciao/examples/Manuscript.ipynb
--rw-rw-r--   0 guille    (1000) guille    (1000)    21077 2022-07-11 15:28:50.000000 mdciao-0.0.5/mdciao/examples/Missing_Contacts.ipynb
--rw-rw-r--   0 guille    (1000) guille    (1000)    30833 2022-07-11 15:28:50.000000 mdciao-0.0.5/mdciao/examples/Tutorial.ipynb
--rw-rw-r--   0 guille    (1000) guille    (1000)      431 2022-06-11 17:35:24.000000 mdciao-0.0.5/mdciao/examples/__init__.py
--rw-rw-r--   0 guille    (1000) guille    (1000)    22275 2022-07-11 15:28:50.000000 mdciao-0.0.5/mdciao/examples/examples.py
-drwxrwxr-x   0 guille    (1000) guille    (1000)        0 2022-07-11 18:30:14.336096 mdciao-0.0.5/mdciao/filenames/
--rw-rw-r--   0 guille    (1000) guille    (1000)      120 2022-06-11 17:35:24.000000 mdciao-0.0.5/mdciao/filenames/__init__.py
--rw-rw-r--   0 guille    (1000) guille    (1000)     5221 2022-06-11 17:35:24.000000 mdciao-0.0.5/mdciao/filenames/filenames.py
-drwxrwxr-x   0 guille    (1000) guille    (1000)        0 2022-07-11 18:30:14.336096 mdciao-0.0.5/mdciao/flare/
--rw-rw-r--   0 guille    (1000) guille    (1000)     1520 2022-06-11 17:35:24.000000 mdciao-0.0.5/mdciao/flare/__init__.py
--rw-rw-r--   0 guille    (1000) guille    (1000)     8995 2022-06-11 17:35:24.000000 mdciao-0.0.5/mdciao/flare/_textutils.py
--rw-rw-r--   0 guille    (1000) guille    (1000)    47836 2022-07-11 15:28:43.000000 mdciao-0.0.5/mdciao/flare/_utils.py
--rw-rw-r--   0 guille    (1000) guille    (1000)    49435 2022-07-11 15:28:50.000000 mdciao-0.0.5/mdciao/flare/flare.py
-drwxrwxr-x   0 guille    (1000) guille    (1000)        0 2022-07-11 18:30:14.336096 mdciao-0.0.5/mdciao/fragments/
--rw-rw-r--   0 guille    (1000) guille    (1000)      570 2022-06-11 17:35:24.000000 mdciao-0.0.5/mdciao/fragments/__init__.py
--rw-rw-r--   0 guille    (1000) guille    (1000)    51478 2022-07-11 15:28:43.000000 mdciao-0.0.5/mdciao/fragments/fragments.py
-drwxrwxr-x   0 guille    (1000) guille    (1000)        0 2022-07-11 18:30:14.336096 mdciao-0.0.5/mdciao/nomenclature/
--rw-rw-r--   0 guille    (1000) guille    (1000)     5870 2022-07-11 15:28:43.000000 mdciao-0.0.5/mdciao/nomenclature/__init__.py
--rw-rw-r--   0 guille    (1000) guille    (1000)     7267 2022-06-11 17:35:24.000000 mdciao-0.0.5/mdciao/nomenclature/_md_from_dataframe.py
--rw-rw-r--   0 guille    (1000) guille    (1000)   125377 2022-07-11 15:28:50.000000 mdciao-0.0.5/mdciao/nomenclature/nomenclature.py
--rw-rw-r--   0 guille    (1000) guille    (1000)   126451 2022-07-01 08:54:25.000000 mdciao-0.0.5/mdciao/nomenclature/nomenclature_BACKUP_374783.py
--rw-------   0 guille    (1000) guille    (1000)   110016 2022-07-01 08:54:28.000000 mdciao-0.0.5/mdciao/nomenclature/nomenclature_BASE_374783.py
--rw-------   0 guille    (1000) guille    (1000)   125320 2022-07-01 08:54:28.000000 mdciao-0.0.5/mdciao/nomenclature/nomenclature_LOCAL_374783.py
--rw-------   0 guille    (1000) guille    (1000)   110614 2022-07-01 08:54:28.000000 mdciao-0.0.5/mdciao/nomenclature/nomenclature_REMOTE_374783.py
--rw-rw-r--   0 guille    (1000) guille    (1000)    44215 2022-07-11 15:28:43.000000 mdciao-0.0.5/mdciao/parsers.py
-drwxrwxr-x   0 guille    (1000) guille    (1000)        0 2022-07-11 18:30:14.336096 mdciao-0.0.5/mdciao/pdb/
--rw-rw-r--   0 guille    (1000) guille    (1000)      362 2022-07-11 15:28:50.000000 mdciao-0.0.5/mdciao/pdb/__init__.py
--rw-rw-r--   0 guille    (1000) guille    (1000)     5169 2022-07-11 15:28:50.000000 mdciao-0.0.5/mdciao/pdb/pdb.py
-drwxrwxr-x   0 guille    (1000) guille    (1000)        0 2022-07-11 18:30:14.336096 mdciao-0.0.5/mdciao/plots/
--rw-rw-r--   0 guille    (1000) guille    (1000)      235 2022-06-11 17:35:24.000000 mdciao-0.0.5/mdciao/plots/__init__.py
--rw-rw-r--   0 guille    (1000) guille    (1000)    82255 2022-07-11 15:28:43.000000 mdciao-0.0.5/mdciao/plots/plots.py
-drwxrwxr-x   0 guille    (1000) guille    (1000)        0 2022-07-11 18:30:14.336096 mdciao-0.0.5/mdciao/sites/
--rw-rw-r--   0 guille    (1000) guille    (1000)     4069 2022-06-11 17:35:24.000000 mdciao-0.0.5/mdciao/sites/__init__.py
--rw-rw-r--   0 guille    (1000) guille    (1000)    11340 2022-06-11 17:35:24.000000 mdciao-0.0.5/mdciao/sites/siteIO.py
-drwxrwxr-x   0 guille    (1000) guille    (1000)        0 2022-07-11 18:30:14.336096 mdciao-0.0.5/mdciao/utils/
--rw-rw-r--   0 guille    (1000) guille    (1000)     2532 2020-07-31 08:19:22.000000 mdciao-0.0.5/mdciao/utils/COM.py
--rw-rw-r--   0 guille    (1000) guille    (1000)      519 2020-07-10 09:57:07.000000 mdciao-0.0.5/mdciao/utils/__init__.py
--rw-rw-r--   0 guille    (1000) guille    (1000)     9225 2022-06-11 17:35:24.000000 mdciao-0.0.5/mdciao/utils/bonds.py
--rw-rw-r--   0 guille    (1000) guille    (1000)    10351 2022-06-11 17:35:24.000000 mdciao-0.0.5/mdciao/utils/contact_matrix.py
--rw-rw-r--   0 guille    (1000) guille    (1000)    21993 2022-06-11 17:35:24.000000 mdciao-0.0.5/mdciao/utils/lists.py
--rw-rw-r--   0 guille    (1000) guille    (1000)    28445 2022-07-11 15:28:43.000000 mdciao-0.0.5/mdciao/utils/residue_and_atom.py
--rw-rw-r--   0 guille    (1000) guille    (1000)    18000 2022-07-11 15:28:43.000000 mdciao-0.0.5/mdciao/utils/sequence.py
--rw-rw-r--   0 guille    (1000) guille    (1000)    41905 2022-07-11 15:28:43.000000 mdciao-0.0.5/mdciao/utils/str_and_dict.py
-drwxrwxr-x   0 guille    (1000) guille    (1000)        0 2022-07-11 18:30:14.332096 mdciao-0.0.5/mdciao.egg-info/
--rw-rw-r--   0 guille    (1000) guille    (1000)     8874 2022-07-11 18:30:14.000000 mdciao-0.0.5/mdciao.egg-info/PKG-INFO
--rw-rw-r--   0 guille    (1000) guille    (1000)     2168 2022-07-11 18:30:14.000000 mdciao-0.0.5/mdciao.egg-info/SOURCES.txt
--rw-rw-r--   0 guille    (1000) guille    (1000)        1 2022-07-11 18:30:14.000000 mdciao-0.0.5/mdciao.egg-info/dependency_links.txt
--rw-rw-r--   0 guille    (1000) guille    (1000)      339 2022-07-11 18:30:14.000000 mdciao-0.0.5/mdciao.egg-info/requires.txt
--rw-rw-r--   0 guille    (1000) guille    (1000)        7 2022-07-11 18:30:14.000000 mdciao-0.0.5/mdciao.egg-info/top_level.txt
-drwxrwxr-x   0 guille    (1000) guille    (1000)        0 2022-07-11 18:30:14.336096 mdciao-0.0.5/scripts/
--rwxrwxr-x   0 guille    (1000) guille    (1000)     1211 2020-07-29 07:52:47.000000 mdciao-0.0.5/scripts/mdc_CGN_overview.py
--rwxrwxr-x   0 guille    (1000) guille    (1000)     1216 2022-06-11 17:35:24.000000 mdciao-0.0.5/scripts/mdc_GPCR_overview.py
--rwxrwxr-x   0 guille    (1000) guille    (1000)     1248 2022-06-11 17:35:24.000000 mdciao-0.0.5/scripts/mdc_KLIFS_overview.py
--rwxrwxr-x   0 guille    (1000) guille    (1000)     2627 2022-06-11 17:35:24.000000 mdciao-0.0.5/scripts/mdc_compare.py
--rwxrwxr-x   0 guille    (1000) guille    (1000)     1795 2022-06-11 17:35:24.000000 mdciao-0.0.5/scripts/mdc_examples.py
--rwxrwxr-x   0 guille    (1000) guille    (1000)     1265 2021-04-23 10:19:35.000000 mdciao-0.0.5/scripts/mdc_fragments.py
--rwxrwxr-x   0 guille    (1000) guille    (1000)     1642 2022-06-11 17:35:24.000000 mdciao-0.0.5/scripts/mdc_interface.py
--rwxrwxr-x   0 guille    (1000) guille    (1000)     1581 2022-06-11 17:35:24.000000 mdciao-0.0.5/scripts/mdc_neighborhoods.py
--rwxrwxr-x   0 guille    (1000) guille    (1000)     1319 2022-06-11 17:35:24.000000 mdciao-0.0.5/scripts/mdc_notebooks.py
--rwxrwxr-x   0 guille    (1000) guille    (1000)     1251 2022-06-11 17:35:24.000000 mdciao-0.0.5/scripts/mdc_pdb.py
--rwxrwxr-x   0 guille    (1000) guille    (1000)     1448 2022-06-11 17:35:24.000000 mdciao-0.0.5/scripts/mdc_residues.py
--rwxrwxr-x   0 guille    (1000) guille    (1000)     1510 2021-01-11 11:10:22.000000 mdciao-0.0.5/scripts/mdc_sites.py
--rw-rw-r--   0 guille    (1000) guille    (1000)       38 2022-07-11 18:30:14.340096 mdciao-0.0.5/setup.cfg
--rw-rw-r--   0 guille    (1000) guille    (1000)     4381 2022-07-11 18:00:13.000000 mdciao-0.0.5/setup.py
-drwxrwxr-x   0 guille    (1000) guille    (1000)        0 2022-07-11 18:30:14.332096 mdciao-0.0.5/tests/
-drwxrwxr-x   0 guille    (1000) guille    (1000)        0 2022-07-11 18:30:14.332096 mdciao-0.0.5/tests/data/
-drwxrwxr-x   0 guille    (1000) guille    (1000)        0 2022-07-11 18:30:14.336096 mdciao-0.0.5/tests/data/RCSB_pdb/
--rw-rw-r--   0 guille    (1000) guille    (1000)   459941 2022-06-11 17:35:24.000000 mdciao-0.0.5/tests/data/RCSB_pdb/3SN6.pdb.gz
-drwxrwxr-x   0 guille    (1000) guille    (1000)        0 2022-07-11 18:30:14.340096 mdciao-0.0.5/tests/data/examples/
--rw-rw-r--   0 guille    (1000) guille    (1000)   662530 2020-07-10 09:57:07.000000 mdciao-0.0.5/tests/data/examples/gs-b2ar.noH.pdb
--rw-rw-r--   0 guille    (1000) guille    (1000)  1807612 2021-01-11 15:06:08.000000 mdciao-0.0.5/tests/data/examples/gs-b2ar.noH.stride.5.xtc
-drwxrwxr-x   0 guille    (1000) guille    (1000)        0 2022-07-11 18:30:14.340096 mdciao-0.0.5/tests/data/json/
--rw-rw-r--   0 guille    (1000) guille    (1000)      221 2022-06-11 17:35:24.000000 mdciao-0.0.5/tests/data/json/tip.json
-drwxrwxr-x   0 guille    (1000) guille    (1000)        0 2022-07-11 18:30:14.340096 mdciao-0.0.5/tests/data/nomenclature/
--rw-rw-r--   0 guille    (1000) guille    (1000)     5798 2020-07-10 09:57:07.000000 mdciao-0.0.5/tests/data/nomenclature/CGN_3SN6.txt
--rw-rw-r--   0 guille    (1000) guille    (1000)   453607 2022-07-11 15:28:43.000000 mdciao-0.0.5/tests/data/nomenclature/KLIFS_P31751.xlsx
--rw-rw-r--   0 guille    (1000) guille    (1000)    31299 2022-06-11 17:35:24.000000 mdciao-0.0.5/tests/data/nomenclature/adrb2_human.xlsx
--rw-rw-r--   0 guille    (1000) guille    (1000)    30491 2022-06-11 17:35:24.000000 mdciao-0.0.5/tests/data/nomenclature/nomenclature.bib
+drwxrwxr-x   0 perezheg  (1000) perezheg  (1000)        0 2023-08-08 14:37:48.684129 mdciao-0.0.6/
+drwxrwxr-x   0 perezheg  (1000) perezheg  (1000)        0 2023-08-08 14:37:48.604128 mdciao-0.0.6/.github/
+drwxrwxr-x   0 perezheg  (1000) perezheg  (1000)        0 2023-08-08 14:37:48.608128 mdciao-0.0.6/.github/workflows/
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     2457 2023-08-08 11:42:57.000000 mdciao-0.0.6/.github/workflows/python-package.yml
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)        6 2021-07-04 10:18:28.000000 mdciao-0.0.6/.gitignore
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     7652 2021-10-18 15:27:23.000000 mdciao-0.0.6/LICENSE.txt
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     8874 2023-08-08 14:37:48.684129 mdciao-0.0.6/PKG-INFO
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     8047 2023-08-08 11:42:57.000000 mdciao-0.0.6/README.rst
+drwxrwxr-x   0 perezheg  (1000) perezheg  (1000)        0 2023-08-08 14:37:48.608128 mdciao-0.0.6/doc/
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)      194 2022-05-31 09:08:14.000000 mdciao-0.0.6/doc/FAQ.rst
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)      634 2021-07-04 10:18:28.000000 mdciao-0.0.6/doc/Makefile
+drwxrwxr-x   0 perezheg  (1000) perezheg  (1000)        0 2023-08-08 14:37:48.612129 mdciao-0.0.6/doc/api/
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)       84 2022-05-31 09:08:14.000000 mdciao-0.0.6/doc/api/api.rst
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)      702 2023-08-08 11:42:57.000000 mdciao-0.0.6/doc/api_stub.rst
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     3565 2022-05-31 09:08:14.000000 mdciao-0.0.6/doc/basic_usage.rst
+drwxrwxr-x   0 perezheg  (1000) perezheg  (1000)        0 2023-08-08 14:37:48.612129 mdciao-0.0.6/doc/cli_cli/
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     1258 2022-05-31 09:08:14.000000 mdciao-0.0.6/doc/cli_cli/cli_cli.rst
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)      149 2021-07-04 10:18:28.000000 mdciao-0.0.6/doc/cli_cli/mdc_CGN_overview.rst
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)      152 2022-05-31 09:08:14.000000 mdciao-0.0.6/doc/cli_cli/mdc_GPCR_overview.rst
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)      157 2021-07-04 10:18:28.000000 mdciao-0.0.6/doc/cli_cli/mdc_compare.rst
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)      151 2021-07-04 10:18:28.000000 mdciao-0.0.6/doc/cli_cli/mdc_fragments.rst
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)      140 2021-07-04 10:18:28.000000 mdciao-0.0.6/doc/cli_cli/mdc_interface.rst
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)      146 2021-07-04 10:18:28.000000 mdciao-0.0.6/doc/cli_cli/mdc_neighborhoods.rst
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)      136 2022-05-31 09:08:14.000000 mdciao-0.0.6/doc/cli_cli/mdc_notebooks.rst
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)      117 2021-10-18 15:27:23.000000 mdciao-0.0.6/doc/cli_cli/mdc_pdb.rst
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)      132 2022-05-31 09:08:14.000000 mdciao-0.0.6/doc/cli_cli/mdc_residues.rst
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)      120 2021-07-04 10:18:28.000000 mdciao-0.0.6/doc/cli_cli/mdc_sites.rst
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     2229 2022-05-31 09:08:14.000000 mdciao-0.0.6/doc/cli_stub.rst
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     3279 2023-08-08 11:42:57.000000 mdciao-0.0.6/doc/conf.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    19918 2023-08-08 11:42:57.000000 mdciao-0.0.6/doc/highlights.rst
+drwxrwxr-x   0 perezheg  (1000) perezheg  (1000)        0 2023-08-08 14:37:48.660128 mdciao-0.0.6/doc/imgs/
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)   275220 2021-10-18 15:27:23.000000 mdciao-0.0.6/doc/imgs/banner.png
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     3411 2021-10-18 15:27:23.000000 mdciao-0.0.6/doc/imgs/banner.svg
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)   407656 2021-10-18 15:27:23.000000 mdciao-0.0.6/doc/imgs/bars_and_PDF.png
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    76482 2021-10-18 15:27:23.000000 mdciao-0.0.6/doc/imgs/bars_and_PDF.svg
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)   276980 2022-05-31 09:08:14.000000 mdciao-0.0.6/doc/imgs/distro_and_violin.png
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)   179227 2022-05-31 09:08:14.000000 mdciao-0.0.6/doc/imgs/distro_and_violin.svg
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)   285007 2021-10-18 15:27:23.000000 mdciao-0.0.6/doc/imgs/flare_inset.svg.zip
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    34924 2022-05-31 09:08:14.000000 mdciao-0.0.6/doc/imgs/freq_comparison.png
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)   973443 2021-10-18 15:27:23.000000 mdciao-0.0.6/doc/imgs/interface.combined.png
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     2988 2021-10-18 15:27:23.000000 mdciao-0.0.6/doc/imgs/interface.combined.svg
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)   318564 2021-10-18 15:27:23.000000 mdciao-0.0.6/doc/imgs/interface.flare@3.5_Ang.small.png
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)   425661 2021-10-18 15:27:23.000000 mdciao-0.0.6/doc/imgs/interface.matrix@3.5_Ang.Fig.4.png
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)   908553 2021-10-18 15:27:23.000000 mdciao-0.0.6/doc/imgs/interface.overall@3.5_Ang.Fig.5.png
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)   451151 2021-10-18 15:27:23.000000 mdciao-0.0.6/doc/imgs/interface_BRG.png
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)   428687 2021-10-18 15:27:23.000000 mdciao-0.0.6/doc/imgs/neighborhoods.LEU394.time_trace@3.5_Ang.Fig.2.png
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)   436918 2021-10-18 15:27:23.000000 mdciao-0.0.6/doc/imgs/neighborhoods.LEU394@G.H5.26.time_trace@3.5_Ang.Fig.2.consensus.png
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)   107497 2021-10-18 15:27:23.000000 mdciao-0.0.6/doc/imgs/neighborhoods.overall.distro.@3.5_Ang.Fig.4.png
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    90906 2021-10-18 15:27:23.000000 mdciao-0.0.6/doc/imgs/neighborhoods.overall@3.5_Ang.Fig.1.consensus.png
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    58973 2022-05-31 09:08:14.000000 mdciao-0.0.6/doc/imgs/neighborhoods.overall@3.5_Ang.Fig.1.png
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    86326 2021-07-04 10:18:28.000000 mdciao-0.0.6/doc/imgs/neighborhoods.overall@3.5_Ang.Fig.3.png
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    69641 2021-10-18 15:27:23.000000 mdciao-0.0.6/doc/imgs/sites.overall@3.5_Ang.Fig.6.png
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    47223 2021-10-18 15:27:23.000000 mdciao-0.0.6/doc/imgs/table_screenshot.png
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     4961 2023-08-08 11:42:57.000000 mdciao-0.0.6/doc/index.rst
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     5835 2023-08-08 12:17:06.000000 mdciao-0.0.6/doc/installation.rst
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)      139 2022-05-31 09:08:14.000000 mdciao-0.0.6/doc/overview.rst
+drwxrwxr-x   0 perezheg  (1000) perezheg  (1000)        0 2023-08-08 14:37:48.660128 mdciao-0.0.6/doc/utils/
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)       44 2021-07-04 10:18:28.000000 mdciao-0.0.6/doc/utils/utils.rst
+drwxrwxr-x   0 perezheg  (1000) perezheg  (1000)        0 2023-08-08 14:37:48.660128 mdciao-0.0.6/mdciao/
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)      424 2022-05-31 09:08:14.000000 mdciao-0.0.6/mdciao/__init__.py
+drwxrwxr-x   0 perezheg  (1000) perezheg  (1000)        0 2023-08-08 14:37:48.660128 mdciao-0.0.6/mdciao/cli/
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)      247 2022-05-31 09:08:14.000000 mdciao-0.0.6/mdciao/cli/__init__.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)   108859 2023-08-08 11:42:57.000000 mdciao-0.0.6/mdciao/cli/cli.py
+drwxrwxr-x   0 perezheg  (1000) perezheg  (1000)        0 2023-08-08 14:37:48.664129 mdciao-0.0.6/mdciao/contacts/
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     1115 2022-05-31 09:08:14.000000 mdciao-0.0.6/mdciao/contacts/__init__.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    13977 2023-08-08 11:42:57.000000 mdciao-0.0.6/mdciao/contacts/_md_compute_contacts.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)   249783 2023-08-08 11:42:57.000000 mdciao-0.0.6/mdciao/contacts/contacts.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    24459 2022-05-31 09:08:14.000000 mdciao-0.0.6/mdciao/dihedrals.py
+drwxrwxr-x   0 perezheg  (1000) perezheg  (1000)        0 2023-08-08 14:37:48.664129 mdciao-0.0.6/mdciao/examples/
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    35957 2022-08-17 09:56:51.000000 mdciao-0.0.6/mdciao/examples/Comparing_CGs_Bars.ipynb
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    38800 2022-08-17 09:56:51.000000 mdciao-0.0.6/mdciao/examples/Comparing_CGs_Flares.ipynb
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    13581 2023-08-08 11:42:57.000000 mdciao-0.0.6/mdciao/examples/EGFR_Kinase_Inhibitors.ipynb
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    24788 2023-08-08 11:42:57.000000 mdciao-0.0.6/mdciao/examples/Flareplot_Schemes.ipynb
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     7053 2023-08-08 11:42:57.000000 mdciao-0.0.6/mdciao/examples/Manuscript.ipynb
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    21077 2022-08-17 09:56:51.000000 mdciao-0.0.6/mdciao/examples/Missing_Contacts.ipynb
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    30833 2023-08-08 11:42:57.000000 mdciao-0.0.6/mdciao/examples/Tutorial.ipynb
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)      431 2023-08-08 11:42:57.000000 mdciao-0.0.6/mdciao/examples/__init__.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    22275 2023-08-08 11:42:57.000000 mdciao-0.0.6/mdciao/examples/examples.py
+drwxrwxr-x   0 perezheg  (1000) perezheg  (1000)        0 2023-08-08 14:37:48.664129 mdciao-0.0.6/mdciao/filenames/
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)      120 2022-05-31 09:08:14.000000 mdciao-0.0.6/mdciao/filenames/__init__.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     5221 2023-08-08 11:42:57.000000 mdciao-0.0.6/mdciao/filenames/filenames.py
+drwxrwxr-x   0 perezheg  (1000) perezheg  (1000)        0 2023-08-08 14:37:48.668129 mdciao-0.0.6/mdciao/flare/
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     1520 2022-05-31 09:08:14.000000 mdciao-0.0.6/mdciao/flare/__init__.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     8995 2022-05-31 09:08:14.000000 mdciao-0.0.6/mdciao/flare/_textutils.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    47899 2023-08-08 11:42:57.000000 mdciao-0.0.6/mdciao/flare/_utils.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    49435 2023-08-08 11:42:57.000000 mdciao-0.0.6/mdciao/flare/flare.py
+drwxrwxr-x   0 perezheg  (1000) perezheg  (1000)        0 2023-08-08 14:37:48.668129 mdciao-0.0.6/mdciao/fragments/
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)      570 2023-08-08 11:42:57.000000 mdciao-0.0.6/mdciao/fragments/__init__.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    51593 2023-08-08 11:42:57.000000 mdciao-0.0.6/mdciao/fragments/fragments.py
+drwxrwxr-x   0 perezheg  (1000) perezheg  (1000)        0 2023-08-08 14:37:48.668129 mdciao-0.0.6/mdciao/nomenclature/
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     5870 2022-08-17 09:56:51.000000 mdciao-0.0.6/mdciao/nomenclature/__init__.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     7267 2022-05-31 09:08:14.000000 mdciao-0.0.6/mdciao/nomenclature/_md_from_dataframe.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)   125377 2023-08-08 11:42:57.000000 mdciao-0.0.6/mdciao/nomenclature/nomenclature.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    44215 2023-08-08 11:42:57.000000 mdciao-0.0.6/mdciao/parsers.py
+drwxrwxr-x   0 perezheg  (1000) perezheg  (1000)        0 2023-08-08 14:37:48.668129 mdciao-0.0.6/mdciao/pdb/
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)      362 2023-08-08 11:42:57.000000 mdciao-0.0.6/mdciao/pdb/__init__.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     5169 2022-08-17 09:56:51.000000 mdciao-0.0.6/mdciao/pdb/pdb.py
+drwxrwxr-x   0 perezheg  (1000) perezheg  (1000)        0 2023-08-08 14:37:48.668129 mdciao-0.0.6/mdciao/plots/
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)      235 2022-05-31 09:08:14.000000 mdciao-0.0.6/mdciao/plots/__init__.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    82255 2023-08-08 11:42:57.000000 mdciao-0.0.6/mdciao/plots/plots.py
+drwxrwxr-x   0 perezheg  (1000) perezheg  (1000)        0 2023-08-08 14:37:48.668129 mdciao-0.0.6/mdciao/sites/
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     4069 2022-05-31 09:08:14.000000 mdciao-0.0.6/mdciao/sites/__init__.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    11340 2023-08-08 11:42:57.000000 mdciao-0.0.6/mdciao/sites/siteIO.py
+drwxrwxr-x   0 perezheg  (1000) perezheg  (1000)        0 2023-08-08 14:37:48.672129 mdciao-0.0.6/mdciao/utils/
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     2532 2021-10-18 15:27:23.000000 mdciao-0.0.6/mdciao/utils/COM.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)      519 2021-07-04 10:18:28.000000 mdciao-0.0.6/mdciao/utils/__init__.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     9225 2022-08-17 09:56:51.000000 mdciao-0.0.6/mdciao/utils/bonds.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    10351 2022-05-31 09:08:14.000000 mdciao-0.0.6/mdciao/utils/contact_matrix.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    21993 2023-08-08 11:47:20.000000 mdciao-0.0.6/mdciao/utils/lists.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    28445 2023-08-08 11:42:57.000000 mdciao-0.0.6/mdciao/utils/residue_and_atom.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    20648 2023-08-08 11:42:57.000000 mdciao-0.0.6/mdciao/utils/sequence.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    41905 2023-08-08 11:42:57.000000 mdciao-0.0.6/mdciao/utils/str_and_dict.py
+drwxrwxr-x   0 perezheg  (1000) perezheg  (1000)        0 2023-08-08 14:37:48.660128 mdciao-0.0.6/mdciao.egg-info/
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     8874 2023-08-08 14:37:48.000000 mdciao-0.0.6/mdciao.egg-info/PKG-INFO
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     4511 2023-08-08 14:37:48.000000 mdciao-0.0.6/mdciao.egg-info/SOURCES.txt
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)        1 2023-08-08 14:37:48.000000 mdciao-0.0.6/mdciao.egg-info/dependency_links.txt
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)      480 2023-08-08 14:37:48.000000 mdciao-0.0.6/mdciao.egg-info/requires.txt
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)        7 2023-08-08 14:37:48.000000 mdciao-0.0.6/mdciao.egg-info/top_level.txt
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)      124 2023-08-08 11:42:57.000000 mdciao-0.0.6/requirements.txt
+drwxrwxr-x   0 perezheg  (1000) perezheg  (1000)        0 2023-08-08 14:37:48.672129 mdciao-0.0.6/scripts/
+-rwxrwxr-x   0 perezheg  (1000) perezheg  (1000)     1211 2021-10-18 15:27:23.000000 mdciao-0.0.6/scripts/mdc_CGN_overview.py
+-rwxrwxr-x   0 perezheg  (1000) perezheg  (1000)     1216 2022-05-31 09:08:14.000000 mdciao-0.0.6/scripts/mdc_GPCR_overview.py
+-rwxrwxr-x   0 perezheg  (1000) perezheg  (1000)     1248 2022-05-31 09:08:14.000000 mdciao-0.0.6/scripts/mdc_KLIFS_overview.py
+-rwxrwxr-x   0 perezheg  (1000) perezheg  (1000)     2627 2022-05-31 09:08:14.000000 mdciao-0.0.6/scripts/mdc_compare.py
+-rwxrwxr-x   0 perezheg  (1000) perezheg  (1000)     1795 2022-05-31 09:08:14.000000 mdciao-0.0.6/scripts/mdc_examples.py
+-rwxrwxr-x   0 perezheg  (1000) perezheg  (1000)     1265 2021-10-18 15:27:23.000000 mdciao-0.0.6/scripts/mdc_fragments.py
+-rwxrwxr-x   0 perezheg  (1000) perezheg  (1000)     1642 2022-05-31 09:08:14.000000 mdciao-0.0.6/scripts/mdc_interface.py
+-rwxrwxr-x   0 perezheg  (1000) perezheg  (1000)     1581 2022-05-31 09:08:14.000000 mdciao-0.0.6/scripts/mdc_neighborhoods.py
+-rwxrwxr-x   0 perezheg  (1000) perezheg  (1000)     1319 2022-05-31 09:08:14.000000 mdciao-0.0.6/scripts/mdc_notebooks.py
+-rwxrwxr-x   0 perezheg  (1000) perezheg  (1000)     1251 2022-05-31 09:08:14.000000 mdciao-0.0.6/scripts/mdc_pdb.py
+-rwxrwxr-x   0 perezheg  (1000) perezheg  (1000)     1448 2022-05-31 09:08:14.000000 mdciao-0.0.6/scripts/mdc_residues.py
+-rwxrwxr-x   0 perezheg  (1000) perezheg  (1000)     1510 2021-10-18 15:27:23.000000 mdciao-0.0.6/scripts/mdc_sites.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)       38 2023-08-08 14:37:48.684129 mdciao-0.0.6/setup.cfg
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     4622 2023-08-08 12:31:31.000000 mdciao-0.0.6/setup.py
+drwxrwxr-x   0 perezheg  (1000) perezheg  (1000)        0 2023-08-08 14:37:48.676128 mdciao-0.0.6/tests/
+drwxrwxr-x   0 perezheg  (1000) perezheg  (1000)        0 2023-08-08 14:37:48.608128 mdciao-0.0.6/tests/data/
+drwxrwxr-x   0 perezheg  (1000) perezheg  (1000)        0 2023-08-08 14:37:48.676128 mdciao-0.0.6/tests/data/RCSB_pdb/
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)   459941 2022-05-31 09:08:14.000000 mdciao-0.0.6/tests/data/RCSB_pdb/3SN6.pdb.gz
+drwxrwxr-x   0 perezheg  (1000) perezheg  (1000)        0 2023-08-08 14:37:48.680128 mdciao-0.0.6/tests/data/bogus_pdb/
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    34545 2021-07-04 10:18:28.000000 mdciao-0.0.6/tests/data/bogus_pdb/2_3AA_chains_and_two_ligs_dimer.pdb
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    17326 2021-07-04 10:18:28.000000 mdciao-0.0.6/tests/data/bogus_pdb/2_3AA_chains_and_two_ligs_monomer.LYS29toLYS99.pdb
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     9621 2021-07-04 10:18:28.000000 mdciao-0.0.6/tests/data/bogus_pdb/2_3AA_chains_and_two_ligs_monomer.gro
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    17265 2021-07-04 10:18:28.000000 mdciao-0.0.6/tests/data/bogus_pdb/2_3AA_chains_and_two_ligs_monomer.pdb
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    12243 2021-07-04 10:18:28.000000 mdciao-0.0.6/tests/data/bogus_pdb/file_no_bonds.pdb
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     1583 2022-05-31 09:08:14.000000 mdciao-0.0.6/tests/data/bogus_pdb/water_and_ions.pdb.gz
+drwxrwxr-x   0 perezheg  (1000) perezheg  (1000)        0 2023-08-08 14:37:48.684129 mdciao-0.0.6/tests/data/examples/
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)   662530 2021-07-04 10:18:28.000000 mdciao-0.0.6/tests/data/examples/gs-b2ar.noH.pdb
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)   451248 2021-07-04 10:18:28.000000 mdciao-0.0.6/tests/data/examples/gs-b2ar.noH.stride.20.xtc
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)  1807612 2021-10-18 15:27:23.000000 mdciao-0.0.6/tests/data/examples/gs-b2ar.noH.stride.5.xtc
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)   258474 2021-07-04 10:18:28.000000 mdciao-0.0.6/tests/data/examples/prot1.pdb.gz
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)      362 2022-05-31 09:08:14.000000 mdciao-0.0.6/tests/data/examples/two_empty_files.zip
+drwxrwxr-x   0 perezheg  (1000) perezheg  (1000)        0 2023-08-08 14:37:48.684129 mdciao-0.0.6/tests/data/json/
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)      131 2022-05-31 09:08:14.000000 mdciao-0.0.6/tests/data/json/GDP.json
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)      152 2022-05-31 09:08:14.000000 mdciao-0.0.6/tests/data/json/GDP_name_XXX.json
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)      101 2022-05-31 09:08:14.000000 mdciao-0.0.6/tests/data/json/tip.dat
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)      221 2022-05-31 09:08:14.000000 mdciao-0.0.6/tests/data/json/tip.json
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)       86 2022-05-31 09:08:14.000000 mdciao-0.0.6/tests/data/json/tip_residx.dat
+drwxrwxr-x   0 perezheg  (1000) perezheg  (1000)        0 2023-08-08 14:37:48.684129 mdciao-0.0.6/tests/data/nomenclature/
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)   459946 2021-07-04 10:18:28.000000 mdciao-0.0.6/tests/data/nomenclature/3SN6_GLU10GLX.pdb.gz
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     5798 2023-08-08 11:42:57.000000 mdciao-0.0.6/tests/data/nomenclature/CGN_3SN6.txt
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     5670 2022-05-31 09:08:14.000000 mdciao-0.0.6/tests/data/nomenclature/GPCRmd_B2AR_nomenclature_test.xlsx
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)   453607 2022-08-17 09:56:51.000000 mdciao-0.0.6/tests/data/nomenclature/KLIFS_P31751.xlsx
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    31299 2022-05-31 09:08:14.000000 mdciao-0.0.6/tests/data/nomenclature/adrb2_human.xlsx
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    30491 2022-05-31 09:08:14.000000 mdciao-0.0.6/tests/data/nomenclature/nomenclature.bib
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     1859 2022-05-31 09:08:14.000000 mdciao-0.0.6/tests/test_COM_utils.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    10000 2022-05-31 09:08:14.000000 mdciao-0.0.6/tests/test_bonds_utils.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    38782 2023-08-08 11:42:57.000000 mdciao-0.0.6/tests/test_cli.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)   142579 2023-08-08 11:42:57.000000 mdciao-0.0.6/tests/test_contacts.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     8244 2023-08-08 11:42:57.000000 mdciao-0.0.6/tests/test_examples.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     9060 2022-08-17 09:56:51.000000 mdciao-0.0.6/tests/test_flare.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    28261 2023-08-08 11:42:57.000000 mdciao-0.0.6/tests/test_flare_utils.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    34304 2023-08-08 11:42:57.000000 mdciao-0.0.6/tests/test_fragments.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    12715 2022-05-31 09:08:14.000000 mdciao-0.0.6/tests/test_lists_utils.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    63121 2023-08-08 11:42:57.000000 mdciao-0.0.6/tests/test_nomenclature.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)      895 2022-05-31 09:08:14.000000 mdciao-0.0.6/tests/test_parsers.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     1313 2023-08-08 11:42:57.000000 mdciao-0.0.6/tests/test_pdb.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    30235 2023-08-08 11:42:57.000000 mdciao-0.0.6/tests/test_plots.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    28430 2023-08-08 11:42:57.000000 mdciao-0.0.6/tests/test_residue_and_atom_utils.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)     3639 2023-08-08 11:42:57.000000 mdciao-0.0.6/tests/test_scripts.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    10069 2023-08-08 11:42:57.000000 mdciao-0.0.6/tests/test_sequence.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    12691 2023-08-08 11:42:57.000000 mdciao-0.0.6/tests/test_siteIO.py
+-rw-rw-r--   0 perezheg  (1000) perezheg  (1000)    33781 2022-05-31 09:08:14.000000 mdciao-0.0.6/tests/test_str_and_dict_utils.py
```

### Comparing `mdciao-0.0.5/LICENSE.txt` & `mdciao-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/PKG-INFO` & `mdciao-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdciao
-Version: 0.0.5
+Version: 0.0.6
 Summary: mdciao: Analysis of Molecular Dynamics Simulations Using Residue Neighborhoods
 Home-page: https://github.com/gph82/mdciao
 Author-email: guillermo.perez@charite.de
 Project-URL: docs, http://proteinformatics.org/mdciao
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `mdciao-0.0.5/README.rst` & `mdciao-0.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/mdciao/cli/cli.py` & `mdciao-0.0.6/mdciao/cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -2013,15 +2013,15 @@
     writer.sheets[sheet2_name] = workbook.add_worksheet(sheet2_name)
     writer.sheets[sheet2_name].write_string(offset, 0, 'pairs by contact frequency')
     _DF.from_dict(freqs).round({"freq": 2, "sum": 2}).to_excel(writer,
                                                                sheet_name=sheet2_name,
                                                                startrow=offset,
                                                                startcol=0,
                                                                )
-    writer.save()
+    writer.close()
     print(fname_excel)
     if pop:
         myfig.tight_layout()
         _plt.show()
 
     return myfig, freqs, plotted_freqs
```

### Comparing `mdciao-0.0.5/mdciao/contacts/__init__.py` & `mdciao-0.0.6/mdciao/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/mdciao/contacts/_md_compute_contacts.py` & `mdciao-0.0.6/mdciao/contacts/_md_compute_contacts.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #    Please note: The following method "compute_contacts" is a
 #    modified version of the one found in the original MDTraj
 #    Python Library, whose original authors and copyright
 #    holders are listed below.
 
 #    The modifications consist in including the indices
 #    of the closest atom-pairs in the returned values. The
-#    modified lines are 212, 243, 244, and 255
+#    modified lines are 141-143, 260, 264, 265, and 276
 ##############################################################################
 
 
 ##############################################################################
 # MDTraj: A Python Library for Loading, Saving, and Manipulating
 #         Molecular Dynamics Trajectories.
 # Copyright 2012-2013 Stanford University and the Authors
@@ -58,21 +58,31 @@
 # https://github.com/mdtraj/mdtraj/issues/1569
 # Further reading
 # https://www.oreilly.com/library/view/understanding-open-source/0596005814/ch03.html
 # https://tldrlegal.com/license/gnu-lesser-general-public-license-v3-(lgpl-3)
 # http://oss-watch.ac.uk/resources/lgpl
 #https://www.gnu.org/licenses/gpl-faq.html#AllCompatibility
 
+##############################################################################
+# Imports
+##############################################################################
+
+from __future__ import print_function, division
 import numpy as _np
 import mdtraj as _md
 from mdtraj.utils import ensure_type
 import itertools
 from mdtraj.utils.six import string_types
 from mdtraj.utils.six.moves import xrange
 from mdtraj.core import element
+
+##############################################################################
+# Code
+##############################################################################
+
 def compute_contacts(traj, contacts='all', scheme='closest-heavy', ignore_nonprotein=True, periodic=True,
                      soft_min=False, soft_min_beta=20):
     """Compute the distance between pairs of residues in a trajectory.
 
     Parameters
     ----------
     traj : md.Trajectory
@@ -124,28 +134,31 @@
         gives the actual residue pairs resolved from `all`. Furthermore,
         when scheme=='ca', any contact pair supplied as input corresponding
         to a residue without an alpha carbon (e.g. HOH) is ignored from the
         input contacts list, meanings that the indexing of the
         output `distances` may not match up with the indexing of the input
         `contacts`. But the indexing of `distances` *will* match up with
         the indexing of `residue_pairs`
+    atom_pairs :  np.ndarray, shape=(n_pairs, 2), dtype=int
+        Each row of this return value gives the indices of the atoms
+        involved in the contact.
 
     Examples
     --------
     >>> # To compute the contact distance between residue 0 and 10 and
     >>> # residues 0 and 11
-    >>> _md.compute_contacts(t, [[0, 10], [0, 11]])
+    >>> md.compute_contacts(t, [[0, 10], [0, 11]])
 
     >>> # the itertools library can be useful to generate the arrays of indices
     >>> group_1 = [0, 1, 2]
     >>> group_2 = [10, 11]
     >>> pairs = list(itertools.product(group_1, group_2))
     >>> print(pairs)
     [(0, 10), (0, 11), (1, 10), (1, 11), (2, 10), (2, 11)]
-    >>> _md.compute_contacts(t, pairs)
+    >>> md.compute_contacts(t, pairs)
 
     See Also
     --------
     mdtraj.geometry.squareform : turn the result from this function
         into a square "contact map"
     Topology.residue : Get residues from the topology by index
     """
@@ -169,16 +182,16 @@
                     residue_pairs.append((i, j))
 
         residue_pairs = _np.array(residue_pairs)
         if len(residue_pairs) == 0:
             raise ValueError('No acceptable residue pairs found')
 
     else:
-        residue_pairs = ensure_type(_np.asarray(contacts), dtype=_np.int, ndim=2, name='contacts',
-                                    shape=(None, 2), warn_on_cast=False)
+        residue_pairs = ensure_type(_np.asarray(contacts), dtype=int, ndim=2, name='contacts',
+                               shape=(None, 2), warn_on_cast=False)
         if not _np.all((residue_pairs >= 0) * (residue_pairs < traj.n_residues)):
             raise ValueError('contacts requests a residue that is not in the permitted range')
 
     # now the bulk of the function. This will calculate atom distances and then
     # re-work them in the required scheme to get residue distances
     scheme = scheme.lower()
     if scheme not in ['ca', 'closest', 'closest-heavy', 'sidechain', 'sidechain-heavy']:
@@ -220,15 +233,20 @@
             residue_membership = [[atom.index for atom in residue.atoms if not (atom.element == element.hydrogen)]
                                   for residue in traj.topology.residues]
         elif scheme == 'sidechain':
             residue_membership = [[atom.index for atom in residue.atoms if atom.is_sidechain]
                                   for residue in traj.topology.residues]
         elif scheme == 'sidechain-heavy':
             # then remove the hydrogens from the above list
-            residue_membership = [[atom.index for atom in residue.atoms if atom.is_sidechain and not (atom.element == element.hydrogen)]
+            if 'GLY' in [residue.name for residue in traj.topology.residues]:
+              import warnings
+              warnings.warn('selected topology includes at least one glycine residue, which has no heavy atoms in its sidechain. The distances involving glycine residues '
+                            'will be computed using the sidechain hydrogen instead.')
+            residue_membership = [[atom.index for atom in residue.atoms if atom.is_sidechain and not (atom.element == element.hydrogen)] if not residue.name == 'GLY'
+                                  else [atom.index for atom in residue.atoms if atom.is_sidechain]
                                   for residue in traj.topology.residues]
 
         residue_lens = [len(ainds) for ainds in residue_membership]
 
         atom_pairs = []
         n_atom_pairs_per_residue_pair = []
         for pair in residue_pairs:
```

### Comparing `mdciao-0.0.5/mdciao/contacts/contacts.py` & `mdciao-0.0.6/mdciao/contacts/contacts.py`

 * *Files 0% similar despite different names*

```diff
@@ -3370,15 +3370,15 @@
                                                              startcol=2+1,
                                                              columns=[
                                                          "label",
                                                          "freq"],
                                                              index=False
                                                              )
 
-        writer.save()
+        writer.close()
 
     def frequency_str_ASCII_file(self, idf,
                                  ascii_file=None):
         r"""
         Create a string with the frequencies from a :obj:`~pandas.DataFrame`
 
         Parameters
@@ -6215,15 +6215,15 @@
 
     """
     m = -1 / switch_off
     b = 1 + (cutoff / switch_off)
     res = m * _np.array(d) + b
     res[d < cutoff] = 1
     res[d > (cutoff + switch_off)] = 0
-    return _np.array(res,dtype=_np.float)
+    return _np.array(res,dtype=float)
 
 def _quadratic_switchoff(d, cutoff, switch_off):
     r"""
     Returns 1 for d<=cutoff, 0 for d>cutoff+switch and a quaratic value [1,0[ between both
 
     d, cutoff, and switch_off have to be in the same units
     Parameters
@@ -6240,15 +6240,15 @@
     """
     # y = k(d-cutoff)^2+c
     c = 1
     k= -1/(switch_off**2)
     res = k*(d-cutoff)**2+c
     res[d < cutoff] = 1
     res[d > (cutoff + switch_off)] = 0
-    return _np.array(res,dtype=_np.float)
+    return _np.array(res,dtype=float)
 
 def _sum_ctc_freqs_by_atom_type(atom_pairs, counts):
     r"""
     Starting from a list of atom pairs and an associated list of counts
     representing a contact frequency, aggregate the frequencies by
     type of contact into "BB-BB", "SC-SC", "SC-BB", "BB-SC" depending
     on the atom-types involved in the contact.
```

### Comparing `mdciao-0.0.5/mdciao/dihedrals.py` & `mdciao-0.0.6/mdciao/dihedrals.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/mdciao/examples/Comparing_CGs_Bars.ipynb` & `mdciao-0.0.6/mdciao/examples/Comparing_CGs_Bars.ipynb`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/mdciao/examples/Comparing_CGs_Flares.ipynb` & `mdciao-0.0.6/mdciao/examples/Comparing_CGs_Flares.ipynb`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/mdciao/examples/EGFR_Kinase_Inhibitors.ipynb` & `mdciao-0.0.6/mdciao/examples/EGFR_Kinase_Inhibitors.ipynb`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/mdciao/examples/Flareplot_Schemes.ipynb` & `mdciao-0.0.6/mdciao/examples/Flareplot_Schemes.ipynb`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/mdciao/examples/Manuscript.ipynb` & `mdciao-0.0.6/mdciao/examples/Manuscript.ipynb`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/mdciao/examples/Missing_Contacts.ipynb` & `mdciao-0.0.6/mdciao/examples/Missing_Contacts.ipynb`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/mdciao/examples/Tutorial.ipynb` & `mdciao-0.0.6/mdciao/examples/Tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/mdciao/examples/examples.py` & `mdciao-0.0.6/mdciao/examples/examples.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/mdciao/filenames/filenames.py` & `mdciao-0.0.6/mdciao/filenames/filenames.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/mdciao/flare/__init__.py` & `mdciao-0.0.6/mdciao/flare/__init__.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/mdciao/flare/_textutils.py` & `mdciao-0.0.6/mdciao/flare/_textutils.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/mdciao/flare/_utils.py` & `mdciao-0.0.6/mdciao/flare/_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -948,14 +948,15 @@
     mute_fragments : list, default is None
         In case this was passed as not None initially
         a re-indexing needs to happen here
 
     Returns
     -------
     residues_as_fragments, anchor_fragments, mute_fragments
+    residues_as_fragmetns : list of lists
     """
     res_idxs = _np.unique(res_idxs_pairs)
     if sparse_fragments:
         assert sparse_residues is False
     if fragments is None:
         if isinstance(sparse_residues, bool):
             if sparse_residues:
@@ -998,15 +999,15 @@
             if len(am_frags)==0:
                 am_frags = None
         else:
             pass
         re_indexed.append(am_frags)
     anchor_fragments, mute_fragments = re_indexed
 
-    return residues_as_fragments, anchor_fragments, mute_fragments
+    return [list(rr) for rr in residues_as_fragments], anchor_fragments, mute_fragments
 
 
 def fontsize_get(iax):
     r"""
     Scan text elements and return a dictionary with fontsizes
     Parameters
     ----------
```

### Comparing `mdciao-0.0.5/mdciao/flare/flare.py` & `mdciao-0.0.6/mdciao/flare/flare.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/mdciao/fragments/__init__.py` & `mdciao-0.0.6/mdciao/fragments/__init__.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/mdciao/fragments/fragments.py` & `mdciao-0.0.6/mdciao/fragments/fragments.py`

 * *Files 2% similar despite different names*

```diff
@@ -1272,17 +1272,17 @@
         False, the missing residues
         have been deleted
     """
     #TODO very related to utils.lists.find_parent_list, perhaps merge?
     _mdcu.lists.assert_no_intersection(fragments, word="fragments")
     frag_idxs = _mdcu.lists.in_what_N_fragments(res_idxs, fragments)
     orphans = _np.flatnonzero([len(par) == 0 for par in frag_idxs])
-    frag_idxs = _np.squeeze(frag_idxs)
+    frag_idxs = [[int(ii) if len(ii)>0 else ii][0] for ii in frag_idxs]
     if len(orphans)>0:
         if raise_on_missing:
             raise ValueError("residues %s don't appear in any 'fragments'. "
                              "If you're OK with this, set 'check_if_subset=False'" % (_np.array(res_idxs)[orphans]))
         else:
-            res_idxs = _np.delete(res_idxs, orphans)
-            frag_idxs = _np.delete(frag_idxs, orphans)
+            res_idxs = _np.array([ri for ii, ri in enumerate(res_idxs) if ii not in orphans])
+            frag_idxs = _np.array([ri for ii, ri in enumerate(frag_idxs) if ii not in orphans])
 
     return frag_idxs, res_idxs
```

### Comparing `mdciao-0.0.5/mdciao/nomenclature/__init__.py` & `mdciao-0.0.6/mdciao/nomenclature/__init__.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/mdciao/nomenclature/_md_from_dataframe.py` & `mdciao-0.0.6/mdciao/nomenclature/_md_from_dataframe.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/mdciao/nomenclature/nomenclature.py` & `mdciao-0.0.6/mdciao/nomenclature/nomenclature.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/mdciao/parsers.py` & `mdciao-0.0.6/mdciao/parsers.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/mdciao/pdb/pdb.py` & `mdciao-0.0.6/mdciao/pdb/pdb.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/mdciao/plots/plots.py` & `mdciao-0.0.6/mdciao/plots/plots.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/mdciao/sites/__init__.py` & `mdciao-0.0.6/mdciao/sites/__init__.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/mdciao/sites/siteIO.py` & `mdciao-0.0.6/mdciao/sites/siteIO.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/mdciao/utils/COM.py` & `mdciao-0.0.6/mdciao/utils/COM.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/mdciao/utils/__init__.py` & `mdciao-0.0.6/mdciao/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/mdciao/utils/bonds.py` & `mdciao-0.0.6/mdciao/utils/bonds.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/mdciao/utils/contact_matrix.py` & `mdciao-0.0.6/mdciao/utils/contact_matrix.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/mdciao/utils/lists.py` & `mdciao-0.0.6/mdciao/utils/lists.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/mdciao/utils/residue_and_atom.py` & `mdciao-0.0.6/mdciao/utils/residue_and_atom.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/mdciao/utils/sequence.py` & `mdciao-0.0.6/mdciao/utils/sequence.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,18 +15,19 @@
 
 .. autosummary::
    :toctree: generated/
 
 """
 import numpy as _np
 from pandas import DataFrame as _DF
-from Bio.pairwise2 import align as _Bioalign
 from .lists import contiguous_ranges as _cranges
 import pandas as _pd
 from IPython.display import display as _display
+from collections import namedtuple as _namedtuple
+from Bio import Align as _BioAlign
 
 
 # See "Define original properties" https://pandas.pydata.org/pandas-docs/stable/development/extending.html#define-original-properties
 class _ADF(_DF):
     r"""
     Sub-class of an :obj:`~pandas.DataFrame` to include the alignment_score as metadata.
 
@@ -97,73 +98,111 @@
     seq : str of len top.n_residues
     """
     assert len(replacement_letter)==1
 
     return ''.join([str(rr.code).replace("None",replacement_letter) for rr in top.residues])
 
 def my_bioalign(seq1, seq2,
-                method="globalms",
-                argstuple=(1,0,-1,-.05),
-                kwargs = {"penalize_end_gaps":False}):
+                method="global",
+                match=1, mismatch=0, open_gap_score=-1, extend_gap_score=-0.05,
+                n_max=1000
+                ):
     r"""
-    Align two sequences using a method of :obj:`Bioalign`
+    Align two sequences using :obj:`Bio.Align.PairwiseAligner`
 
     Note
     ----
-    This is a one-liner wrapper around whatever method
-    of :obj:`Bioalign` has been chosen, typically
-    pairwise2.align.globalms
-
     The intention is to only use *this* method throughout
     mdciao, and change *here* any alignment parameters s.t.
     alignment is done using *always* the same parameters.
 
-    The exposed arguments `method` and `argstuple`
-    are there for future development but will raise
-    NotImplementedErrors if changed.
-
-    See https://biopython.org/DIST/docs/api/Bio.pairwise2-module.html
+    See https://biopython.org/docs/1.75/api/Bio.Align.html?#Bio.Align.PairwiseAligner
     for more info
 
     Parameters
     ----------
     seq1 : str, any length
     seq2 : str, any length
-    method : str, default is "globalms"
-    argstuple : tuple, default is (-1,0,-1,-.05)
-        The tuple controlling penalties for:
-        * matches
-        * mismatches
-        * opening a gap
-        * extending the gap
+    method : str, default is "global"
+        Gets passed as argument "mode" to
+        the underlying :obj:~`Bio.Align.PairwiseAligner`
+        At the moment, any other value will raise NotImplementedError.
+    match : int or float, default is 1
+        Score value for a match.
+        At the moment, any other value will raise NotImplementedError.
+    mismatch : int or float, default is 0
+        Penalty value (non-positve score) for a mismatch.
+        At the moment, any other value will raise NotImplementedError.
+    open_gap_score : int or float, default is -1
+        Penalty value (non-positve score) for opening a gap.
+        At the moment, any other value will raise NotImplementedError.
+    extend_gap_score : int or float, default is 0.05
+        Penalty value (non-positve score) for extending a gap.
+        At the moment, any other value will raise NotImplementedError.
+    n_max : int, default is 1000
+        The maximum number of returned alignments.
 
     Returns
     -------
     alignments : list
-        A list of tuples, each containing seq1,seq2,score.
-        See https://biopython.org/DIST/docs/api/Bio.pairwise2-module.html
-        for more info
-
+        A list of namedtuples, each containing seq1,seq2,score.
 
     """
-    # This is to be able to raise the NotImplemented but also to hard-code the only allowEd method here
-    allowed_method="globalms"
-    allowed_tuple = (1, 0, -1, -.05)
+    _my_alg = _namedtuple("NamedTuplePairwiseAlignments", ["seq1", "seq2", "score"])
+
+    # This is to be able to raise the NotImplemented but also to hard-code the only allowed method here
+    allowed_method="global"
+    end_gap_score = 0 # equivalent to the old "penalize_end_gaps": False in pairwise2
     if method!=allowed_method:
         raise (NotImplementedError("At the moment only %s is "
                                    "allowed as alignment method"%method))
 
+    allowed_kwargs = {"match": 1, "mismatch": 0, "open_gap_score": -1, "extend_gap_score": -0.05}
+
+    provided_kwargs = {key : val for key, val in locals().items() if key in allowed_kwargs}
+    if allowed_kwargs == provided_kwargs:
+        a = _BioAlign.PairwiseAligner(mode=method,
+                                      match=match, mismatch=mismatch, open_gap_score=open_gap_score,
+                                      extend_gap_score=extend_gap_score, end_gap_score=end_gap_score)
+        alignments = [a for __, a in zip(range(n_max), a.align(seq1,seq2))]
+        scores = _np.array([a.score for a in alignments])
+
+        # Some edge cases in the tests produce alignments with no overlap at all, i.e. with an empty a.aligned attribute,
+        # that are equally scored with other alignments, e.g.
+        # ---X       --X
+        # ----  vs   ---
+        # IWN-       IWN
+        # have the same scores b.c. mismatches are valued with 0
+
+        # These alignments are badly scored alignments in "guess" mode that can be discarded safely
+        # Hence, we mark the start of the alignment as _np.inf s.t. they sink
+        # to the bottom the list of equally (badly) scored alignments
+        starting_alignment_idxs = [[a.aligned[1][0][0] if len(a.aligned[1])>0 else _np.inf][0] for a in alignments]
+
+        # TODO
+        # Then comes this very interim solution, to not touch the test-suite ATM, checkout
+        # this issue to find out why this reordering https://github.com/biopython/biopython/issues/4360
+
+        # In each block of equally scored alignments, sort by ascending order
+        # of first match-index for sequence 2
+        order = _np.lexsort((starting_alignment_idxs, -scores))
+        # reorder
+        alignments = [alignments[ii] for ii in order[:n_max]]
+        scores = [a.score for a in alignments] #reorder scores
+        if hasattr(alignments[0],"sequences"): # some more backward compatibility
+            seqs = [a._format_generalized().replace(" ","").splitlines() for a in alignments]
+        else:
+            seqs = [a.format().splitlines() for a in alignments]
 
-    if tuple(argstuple) == tuple(allowed_tuple):
-        return getattr(_Bioalign, method)(seq1, seq2, *argstuple, **kwargs)
+        algs = [_my_alg(s[0],s[-1],score) for s,score in zip(seqs,scores)]
+        return algs
     else:
-        raise NotImplementedError("At the moment only %s is "
-                                   "allowed as argument tuple, got"
-                                   "instead %s"%(str(allowed_tuple),
-                                                    str(argstuple)))
+        raise NotImplementedError(f"At the moment, the keyword arguments {list(allowed_kwargs.keys()) }are exposed"
+                                  f"to make them highly visible, but their values can't be changed from {allowed_kwargs}."
+                                  f"The input was instead {provided_kwargs}")
 
 
 
 def alignment_result_to_list_of_dicts(ialg,
                                       seq_0_res_idxs,
                                       seq_1_res_idxs,
                                       topology_0=None,
@@ -174,29 +213,28 @@
                                       key_idx_seq_0="idx_0",
                                       key_idx_seq_1="idx_1",
                                       key_full_resname_seq_0='fullname_0',
                                       key_full_resname_seq_1='fullname_1',
                                       verbose=False,
                                       ):
     r"""
-    Input an alignment result (:obj:`ialg`) and return it as
+    Input an alignment result `ialg` and return it as
     a list of per-residue dictionaries with other complementary keys.
 
     This list of dictionaries is very suitable for further operations
     with :obj:`pandas.DataFrame`.
 
     TODO
     ----
     Decide whether we need key_resSeq_1 or not
 
     Parameters
     ----------
-    ialg: list
-        list with four entries, see obj:`my_bioalign`
-        and https://biopython.org/DIST/docs/api/Bio.pairwise2-module.html
+    ialg: namedtuple
+        See return value of obj:`my_bioalign`
         for more info
     topology_0: :obj:`mdtraj.Topology` object
     seq_0_res_idxs:
         Zero-indexed residue indices of whatever was in seq_0
     seq_1_res_idxs:
         Zero-indexed residue indices of whatever was in seq_1
     key_AA_code_seq_0 : str, default is AA_0
```

### Comparing `mdciao-0.0.5/mdciao/utils/str_and_dict.py` & `mdciao-0.0.6/mdciao/utils/str_and_dict.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/mdciao.egg-info/PKG-INFO` & `mdciao-0.0.6/mdciao.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdciao
-Version: 0.0.5
+Version: 0.0.6
 Summary: mdciao: Analysis of Molecular Dynamics Simulations Using Residue Neighborhoods
 Home-page: https://github.com/gph82/mdciao
 Author-email: guillermo.perez@charite.de
 Project-URL: docs, http://proteinformatics.org/mdciao
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `mdciao-0.0.5/scripts/mdc_CGN_overview.py` & `mdciao-0.0.6/scripts/mdc_CGN_overview.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/scripts/mdc_GPCR_overview.py` & `mdciao-0.0.6/scripts/mdc_GPCR_overview.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/scripts/mdc_KLIFS_overview.py` & `mdciao-0.0.6/scripts/mdc_KLIFS_overview.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/scripts/mdc_compare.py` & `mdciao-0.0.6/scripts/mdc_compare.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/scripts/mdc_examples.py` & `mdciao-0.0.6/scripts/mdc_examples.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/scripts/mdc_fragments.py` & `mdciao-0.0.6/scripts/mdc_fragments.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/scripts/mdc_interface.py` & `mdciao-0.0.6/scripts/mdc_interface.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/scripts/mdc_neighborhoods.py` & `mdciao-0.0.6/scripts/mdc_neighborhoods.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/scripts/mdc_notebooks.py` & `mdciao-0.0.6/scripts/mdc_notebooks.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/scripts/mdc_pdb.py` & `mdciao-0.0.6/scripts/mdc_pdb.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/scripts/mdc_residues.py` & `mdciao-0.0.6/scripts/mdc_residues.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/scripts/mdc_sites.py` & `mdciao-0.0.6/scripts/mdc_sites.py`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/setup.py` & `mdciao-0.0.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 from setuptools import setup, find_packages
 import os
 os.environ["BEZIER_NO_EXTENSION"]="true" # Check https://github.com/dhermes/bezier/releases/tag/2020.2.3
 
 with open("README.rst", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
@@ -47,18 +47,22 @@
                     "cython",
                     "numpy>=1.18.1",
                     "mdtraj",
                     "astunparse; python_version!='3.8'",
                     "astunparse<1.6.3; python_version=='3.8'",
                     "pandas",
                     "matplotlib",
+                    "matplotlib<=3.5.3; python_version<'3.8'",
+                    "scipy<=1.9.0; python_version<='3.8'",
                     "scipy",
                     "joblib",
                     "openpyxl",
                     "biopython>=1.77",
+                    "ipython<=8.12; python_version<='3.8'",
+                    "ipython==7.*; python_version=='3.7'",
                     "ipython",
                     "XlsxWriter",
                     "requests",
                     "tqdm",
                     "natsort",
                     "bezier; python_version!='3.6'",
                     "bezier<2020.2.3; python_version=='3.6'",
```

### Comparing `mdciao-0.0.5/tests/data/RCSB_pdb/3SN6.pdb.gz` & `mdciao-0.0.6/tests/data/RCSB_pdb/3SN6.pdb.gz`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/tests/data/examples/gs-b2ar.noH.pdb` & `mdciao-0.0.6/tests/data/examples/gs-b2ar.noH.pdb`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/tests/data/examples/gs-b2ar.noH.stride.5.xtc` & `mdciao-0.0.6/tests/data/examples/gs-b2ar.noH.stride.5.xtc`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/tests/data/nomenclature/CGN_3SN6.txt` & `mdciao-0.0.6/tests/data/nomenclature/CGN_3SN6.txt`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/tests/data/nomenclature/KLIFS_P31751.xlsx` & `mdciao-0.0.6/tests/data/nomenclature/KLIFS_P31751.xlsx`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/tests/data/nomenclature/adrb2_human.xlsx` & `mdciao-0.0.6/tests/data/nomenclature/adrb2_human.xlsx`

 * *Files identical despite different names*

### Comparing `mdciao-0.0.5/tests/data/nomenclature/nomenclature.bib` & `mdciao-0.0.6/tests/data/nomenclature/nomenclature.bib`

 * *Files identical despite different names*

