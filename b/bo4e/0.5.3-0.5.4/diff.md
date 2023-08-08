# Comparing `tmp/bo4e-0.5.3.tar.gz` & `tmp/bo4e-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bo4e-0.5.3.tar", last modified: Wed Jul 26 05:42:14 2023, max compression
+gzip compressed data, was "bo4e-0.5.4.tar", last modified: Tue Aug  8 07:09:27 2023, max compression
```

## Comparing `bo4e-0.5.3.tar` & `bo4e-0.5.4.tar`

### file list

```diff
@@ -1,448 +1,448 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:42:14.222693 bo4e-0.5.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:42:14.186692 bo4e-0.5.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:42:14.186692 bo4e-0.5.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-26 05:42:02.000000 bo4e-0.5.3/.github/ISSUE_TEMPLATE/funktionale-anforderung-an-den-bo4e-standard.md
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-26 05:42:02.000000 bo4e-0.5.3/.github/ISSUE_TEMPLATE/technisches-problem---python-specific-problem.md
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-26 05:42:02.000000 bo4e-0.5.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:42:14.186692 bo4e-0.5.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-26 05:42:02.000000 bo4e-0.5.3/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-26 05:42:02.000000 bo4e-0.5.3/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-26 05:42:02.000000 bo4e-0.5.3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-26 05:42:02.000000 bo4e-0.5.3/.github/workflows/formatting.yml
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-26 05:42:02.000000 bo4e-0.5.3/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-26 05:42:02.000000 bo4e-0.5.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-26 05:42:02.000000 bo4e-0.5.3/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-26 05:42:02.000000 bo4e-0.5.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-26 05:42:02.000000 bo4e-0.5.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    17193 2023-07-26 05:42:02.000000 bo4e-0.5.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-26 05:42:02.000000 bo4e-0.5.3/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:42:14.186692 bo4e-0.5.3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-26 05:42:02.000000 bo4e-0.5.3/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-26 05:42:02.000000 bo4e-0.5.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-26 05:42:02.000000 bo4e-0.5.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-07-26 05:42:02.000000 bo4e-0.5.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-26 05:42:02.000000 bo4e-0.5.3/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 05:42:02.000000 bo4e-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-26 05:42:14.222693 bo4e-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-26 05:42:02.000000 bo4e-0.5.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:42:14.186692 bo4e-0.5.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-07-26 05:42:02.000000 bo4e-0.5.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:42:14.186692 bo4e-0.5.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-26 05:42:02.000000 bo4e-0.5.3/docs/_static/bo4e-python-favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-07-26 05:42:02.000000 bo4e-0.5.3/docs/_static/bo4e-python-favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-07-26 05:42:02.000000 bo4e-0.5.3/docs/_static/bo4e-python-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    26543 2023-07-26 05:42:02.000000 bo4e-0.5.3/docs/_static/bo4e-python-logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:42:14.186692 bo4e-0.5.3/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-07-26 05:42:02.000000 bo4e-0.5.3/docs/api/bo4e.bo.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10343 2023-07-26 05:42:02.000000 bo4e-0.5.3/docs/api/bo4e.com.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12407 2023-07-26 05:42:02.000000 bo4e-0.5.3/docs/api/bo4e.enum.rst
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-26 05:42:02.000000 bo4e-0.5.3/docs/api/bo4e.rst
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-26 05:42:02.000000 bo4e-0.5.3/docs/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-26 05:42:02.000000 bo4e-0.5.3/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-26 05:42:02.000000 bo4e-0.5.3/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-07-26 05:42:02.000000 bo4e-0.5.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-26 05:42:02.000000 bo4e-0.5.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-26 05:42:02.000000 bo4e-0.5.3/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-26 05:42:02.000000 bo4e-0.5.3/docs/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-26 05:42:02.000000 bo4e-0.5.3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-26 05:42:02.000000 bo4e-0.5.3/docs/test_uml.py
--rw-r--r--   0 runner    (1001) docker     (123)    28380 2023-07-26 05:42:02.000000 bo4e-0.5.3/docs/uml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:42:14.186692 bo4e-0.5.3/json_schemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:42:14.190693 bo4e-0.5.3/json_schemas/bo/
--rw-r--r--   0 runner    (1001) docker     (123)    51662 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/bo/Angebot.json
--rw-r--r--   0 runner    (1001) docker     (123)    20861 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/bo/Ansprechpartner.json
--rw-r--r--   0 runner    (1001) docker     (123)    30039 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/bo/Ausschreibung.json
--rw-r--r--   0 runner    (1001) docker     (123)    31018 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/bo/Buendelvertrag.json
--rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/bo/Energiemenge.json
--rw-r--r--   0 runner    (1001) docker     (123)    18226 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/bo/Fremdkosten.json
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/bo/Geschaeftsobjekt.json
--rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/bo/Geschaeftspartner.json
--rw-r--r--   0 runner    (1001) docker     (123)    17575 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/bo/Kosten.json
--rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/bo/Lastgang.json
--rw-r--r--   0 runner    (1001) docker     (123)    10704 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/bo/LastgangKompakt.json
--rw-r--r--   0 runner    (1001) docker     (123)    24248 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/bo/Marktlokation.json
--rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/bo/Marktteilnehmer.json
--rw-r--r--   0 runner    (1001) docker     (123)    30665 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/bo/Messlokation.json
--rw-r--r--   0 runner    (1001) docker     (123)    35920 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/bo/Netznutzungsrechnung.json
--rw-r--r--   0 runner    (1001) docker     (123)    31358 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/bo/Preisblatt.json
--rw-r--r--   0 runner    (1001) docker     (123)    37279 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/bo/PreisblattDienstleistung.json
--rw-r--r--   0 runner    (1001) docker     (123)    37788 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/bo/PreisblattHardware.json
--rw-r--r--   0 runner    (1001) docker     (123)    31923 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/bo/PreisblattKonzessionsabgabe.json
--rw-r--r--   0 runner    (1001) docker     (123)    37797 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/bo/PreisblattMessung.json
--rw-r--r--   0 runner    (1001) docker     (123)    32989 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/bo/PreisblattNetznutzung.json
--rw-r--r--   0 runner    (1001) docker     (123)    34002 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/bo/Rechnung.json
--rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/bo/Region.json
--rw-r--r--   0 runner    (1001) docker     (123)    63902 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/bo/Regionaltarif.json
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/bo/Standorteigenschaften.json
--rw-r--r--   0 runner    (1001) docker     (123)    61162 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/bo/Tarif.json
--rw-r--r--   0 runner    (1001) docker     (123)    30304 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/bo/Tarifinfo.json
--rw-r--r--   0 runner    (1001) docker     (123)    43186 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/bo/Tarifkosten.json
--rw-r--r--   0 runner    (1001) docker     (123)    57802 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/bo/Tarifpreisblatt.json
--rw-r--r--   0 runner    (1001) docker     (123)    27127 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/bo/Vertrag.json
--rw-r--r--   0 runner    (1001) docker     (123)    19710 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/bo/Zaehler.json
--rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/bo/Zeitreihe.json
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/bo/_LastgangBody.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:42:14.198693 bo4e-0.5.3/json_schemas/com/
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Adresse.json
--rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Angebotsposition.json
--rw-r--r--   0 runner    (1001) docker     (123)    38449 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Angebotsteil.json
--rw-r--r--   0 runner    (1001) docker     (123)    40573 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Angebotsvariante.json
--rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/AufAbschlag.json
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/AufAbschlagProOrt.json
--rw-r--r--   0 runner    (1001) docker     (123)    28916 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/AufAbschlagRegional.json
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/AufAbschlagstaffelProOrt.json
--rw-r--r--   0 runner    (1001) docker     (123)    13809 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Ausschreibungsdetail.json
--rw-r--r--   0 runner    (1001) docker     (123)    18479 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Ausschreibungslos.json
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Betrag.json
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/COM.json
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Dienstleistung.json
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Energieherkunft.json
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Energiemix.json
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/ExterneReferenz.json
--rw-r--r--   0 runner    (1001) docker     (123)    11326 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Fremdkostenblock.json
--rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Fremdkostenposition.json
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Geokoordinaten.json
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Geraet.json
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Geraeteeigenschaften.json
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Hardware.json
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Katasteradresse.json
--rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Kostenblock.json
--rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Kostenposition.json
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/KriteriumWert.json
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/MarktgebietInfo.json
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Menge.json
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Messlokationszuordnung.json
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/PositionsAufAbschlag.json
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Preis.json
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Preisgarantie.json
--rw-r--r--   0 runner    (1001) docker     (123)    11150 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Preisposition.json
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Preisstaffel.json
--rw-r--r--   0 runner    (1001) docker     (123)    12985 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Rechnungsposition.json
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/RegionaleGueltigkeit.json
--rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/RegionalePreisgarantie.json
--rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/RegionalePreisstaffel.json
--rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/RegionaleTarifpreisposition.json
--rw-r--r--   0 runner    (1001) docker     (123)    32018 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/RegionalerAufAbschlag.json
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Regionskriterium.json
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Rufnummer.json
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Sigmoidparameter.json
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/StandorteigenschaftenAllgemein.json
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/StandorteigenschaftenGas.json
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/StandorteigenschaftenStrom.json
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Steuerbetrag.json
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Tagesvektor.json
--rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Tarifberechnungsparameter.json
--rw-r--r--   0 runner    (1001) docker     (123)     9076 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Tarifeinschraenkung.json
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Tarifpreis.json
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Tarifpreisposition.json
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/TarifpreispositionProOrt.json
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/TarifpreisstaffelProOrt.json
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Unterschrift.json
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Verbrauch.json
--rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Vertragskonditionen.json
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Vertragsteil.json
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Zaehlwerk.json
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Zeitintervall.json
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Zeitraum.json
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Zeitreihenwert.json
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Zeitreihenwertkompakt.json
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/com/Zustaendigkeit.json
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-26 05:42:02.000000 bo4e-0.5.3/json_schemas/generate_json_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-26 05:42:02.000000 bo4e-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-26 05:42:02.000000 bo4e-0.5.3/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-26 05:42:02.000000 bo4e-0.5.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-26 05:42:14.226693 bo4e-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-26 05:42:02.000000 bo4e-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:42:14.182692 bo4e-0.5.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:42:14.198693 bo4e-0.5.3/src/bo4e/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:42:14.202693 bo4e-0.5.3/src/bo4e/bo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/bo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/bo/angebot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/bo/ansprechpartner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/bo/ausschreibung.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/bo/buendelvertrag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/bo/energiemenge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/bo/fremdkosten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/bo/geschaeftsobjekt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/bo/geschaeftspartner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/bo/kosten.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/bo/lastgang.py
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/bo/marktlokation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/bo/marktteilnehmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/bo/messlokation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/bo/netznutzungsrechnung.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/bo/preisblatt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/bo/preisblattdienstleistung.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/bo/preisblatthardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/bo/preisblattkonzessionsabgabe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/bo/preisblattmessung.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/bo/preisblattnetznutzung.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/bo/rechnung.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/bo/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/bo/regionaltarif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/bo/standorteigenschaften.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/bo/tarif.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/bo/tarifinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/bo/tarifkosten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/bo/tarifpreisblatt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/bo/vertrag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/bo/zaehler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/bo/zeitreihe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:42:14.206693 bo4e-0.5.3/src/bo4e/com/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/adresse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/angebotsposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/angebotsteil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/angebotsvariante.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/aufabschlag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/aufabschlagproort.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/aufabschlagregional.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/aufabschlagstaffelproort.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/ausschreibungsdetail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/ausschreibungslos.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/betrag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/com.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/dienstleistung.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/energieherkunft.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/energiemix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/externereferenz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/fremdkostenblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/fremdkostenposition.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/geokoordinaten.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/geraet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/geraeteeigenschaften.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/katasteradresse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/kostenblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/kostenposition.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/kriteriumwert.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/marktgebietinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/menge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/messlokationszuordnung.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/positionsaufabschlag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/preis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/preisgarantie.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/preisposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/preisstaffel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/rechnungsposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/regionalegueltigkeit.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/regionalepreisgarantie.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/regionalepreisstaffel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/regionaleraufabschlag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/regionaletarifpreisposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/regionskriterium.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/rufnummer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/sigmoidparameter.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/standorteigenschaftengas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/standorteigenschaftenstrom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/steuerbetrag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/tagesvektor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/tarifberechnungsparameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/tarifeinschraenkung.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/tarifpreis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/tarifpreisposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/tarifpreispositionproort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/tarifpreisstaffelproort.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/unterschrift.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/verbrauch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/vertragskonditionen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/vertragsteil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/zaehlwerk.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/zeitintervall.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/zeitraum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/zeitreihenwert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/zeitreihenwertkompakt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/com/zustaendigkeit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:42:14.214693 bo4e-0.5.3/src/bo4e/enum/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/angebotsstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/anrede.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/arithmetische_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/artikelid.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/aufabschlagstyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/aufabschlagsziel.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/ausschreibungsportal.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/ausschreibungsstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/ausschreibungstyp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/bdewartikelnummer.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/bemessungsgroesse.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/bilanzierungsmethode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/botyp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/dienstleistungstyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/energierichtung.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/erzeugungsart.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/gasqualitaet.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/gebiettyp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/geraetemerkmal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/geraetetyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/geschaeftspartnerrolle.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/gueltigkeitstyp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/kalkulationsmethode.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/kontaktart.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/kostenklasse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/kundengruppe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/kundengruppeka.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/kundentyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/landescode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/leistungstyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/lokationstyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/marktrolle.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/medium.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/mengeneinheit.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/mengenoperator.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/messart.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/messgroesse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/messpreistyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/messwertstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/messwertstatuszusatz.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/netzebene.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/nnrechnungsart.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/nnrechnungstyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/oekolabel.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/oekozertifikat.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/preisgarantietyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/preismodell.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/preisstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/preistyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/rechnungslegung.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/rechnungsstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/rechnungstyp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/regionskriteriumtyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/rollencodetyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/rufnummernart.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/sparte.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/steuerkennzeichen.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/strenum.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/tarifart.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/tarifkalkulationsmethode.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/tarifmerkmal.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/tarifregionskriterium.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/tariftyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/tarifzeit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/themengebiet.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/titel.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/verbrauchsart.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/vertragsart.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/vertragsform.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/vertragsstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/voraussetzungen.py
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/waehrungscode.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/waehrungseinheit.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/wertermittlungsverfahren.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/zaehlerauspraegung.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/zaehlertyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/enum/zeiteinheit.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:42:14.214693 bo4e-0.5.3/src/bo4e/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-07-26 05:42:02.000000 bo4e-0.5.3/src/bo4e/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:42:14.198693 bo4e-0.5.3/src/bo4e.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-26 05:42:14.000000 bo4e-0.5.3/src/bo4e.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13420 2023-07-26 05:42:14.000000 bo4e-0.5.3/src/bo4e.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 05:42:14.000000 bo4e-0.5.3/src/bo4e.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 05:42:14.000000 bo4e-0.5.3/src/bo4e.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-26 05:42:14.000000 bo4e-0.5.3/src/bo4e.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-26 05:42:14.000000 bo4e-0.5.3/src/bo4e.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:42:14.222693 bo4e-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/serialization_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_adresse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_angebot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_angebotsposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_angebotsteil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_angebotsvariante.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_ansprechpartner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_aufabschlag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_aufabschlagproort.py
--rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_aufabschlagregional.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_aufabschlagstaffelproort.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_ausschreibung.py
--rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_ausschreibungsdetail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_ausschreibungslos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_betrag.py
--rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_buendelvertrag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_bypassing_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:42:14.182692 bo4e-0.5.3/tests/test_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 05:42:14.222693 bo4e-0.5.3/tests/test_data/test_data_adresse/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_data/test_data_adresse/test_data_adresse_missing_plz.json
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_data/test_data_adresse/test_data_adresse_only_required_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_data/test_data_adresse/test_data_adresse_with_all_possible_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_doc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_energieherkunft.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_energiemenge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_energiemix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_externe_referenz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_fremdkosten.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_fremdkostenblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_fremdkostenposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_geokoordinaten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_geraet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_geraeteeigenschaften.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_geschaeftsobjekt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_geschaeftspartner.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_katasteradresse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_kosten.py
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_kostenblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_kostenposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_kriteriumswert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_lastgang.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_lastgangkompakt.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_marktgebietinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_marktlokation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_marktteilnehmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_menge.py
--rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_messlokation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_messlokationszuordnung.py
--rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_netznutzungsrechnung.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_positionsaufabschlag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_preis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_preisblatt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_preisblatt_dienstleistung.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_preisblatt_hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_preisblatt_konzessionsabgabe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_preisblatt_messung.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_preisblattnetznutzung.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_preisgarantie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_preisposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_preisstaffel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_rechnung.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_rechnungsposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_regionalegueltigkeit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_regionalepreisgarantie.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_regionalepreisstaffel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_regionaleraufabschlag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_regionaletarifpreisposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_regionaltarif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_regionskriterium.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_sigmoidparameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_standorteigenschaften.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_standorteigenschaftengas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_standorteigenschaftenstrom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_steuerbetrag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_tagesvektor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_tarif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_tarifberechnungsparameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_tarifeinschraenkung.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_tarifinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_tarifkosten.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_tarifpreis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_tarifpreisblatt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_tarifpreisposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_tarifpreispositionproort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_tarifpreisstaffelproort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_unterschrift.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_verbrauch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_vertrag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_vertragskonditionen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_vertragsteil.py
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_zaehler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_zeitintervall.py
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_zeitraum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_zeitreihe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_zeitreihenwert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/test_zeitreihenwertkompakt.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-26 05:42:02.000000 bo4e-0.5.3/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-26 05:42:02.000000 bo4e-0.5.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:09:27.907184 bo4e-0.5.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:09:27.867183 bo4e-0.5.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:09:27.867183 bo4e-0.5.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-08-08 07:09:16.000000 bo4e-0.5.4/.github/ISSUE_TEMPLATE/funktionale-anforderung-an-den-bo4e-standard.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-08-08 07:09:16.000000 bo4e-0.5.4/.github/ISSUE_TEMPLATE/technisches-problem---python-specific-problem.md
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-08 07:09:16.000000 bo4e-0.5.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:09:27.867183 bo4e-0.5.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-08-08 07:09:16.000000 bo4e-0.5.4/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-08 07:09:16.000000 bo4e-0.5.4/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-08 07:09:16.000000 bo4e-0.5.4/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-08-08 07:09:16.000000 bo4e-0.5.4/.github/workflows/formatting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-08 07:09:16.000000 bo4e-0.5.4/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-08-08 07:09:16.000000 bo4e-0.5.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-08-08 07:09:16.000000 bo4e-0.5.4/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-08-08 07:09:16.000000 bo4e-0.5.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-08-08 07:09:16.000000 bo4e-0.5.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    17193 2023-08-08 07:09:16.000000 bo4e-0.5.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-08 07:09:16.000000 bo4e-0.5.4/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:09:27.867183 bo4e-0.5.4/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-08-08 07:09:16.000000 bo4e-0.5.4/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-08 07:09:16.000000 bo4e-0.5.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-08 07:09:16.000000 bo4e-0.5.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-08-08 07:09:16.000000 bo4e-0.5.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-08-08 07:09:16.000000 bo4e-0.5.4/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 07:09:16.000000 bo4e-0.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-08-08 07:09:27.907184 bo4e-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-08-08 07:09:16.000000 bo4e-0.5.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:09:27.871183 bo4e-0.5.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-08-08 07:09:16.000000 bo4e-0.5.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:09:27.871183 bo4e-0.5.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-08-08 07:09:16.000000 bo4e-0.5.4/docs/_static/bo4e-python-favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-08-08 07:09:16.000000 bo4e-0.5.4/docs/_static/bo4e-python-favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-08-08 07:09:16.000000 bo4e-0.5.4/docs/_static/bo4e-python-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26543 2023-08-08 07:09:16.000000 bo4e-0.5.4/docs/_static/bo4e-python-logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:09:27.871183 bo4e-0.5.4/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-08-08 07:09:16.000000 bo4e-0.5.4/docs/api/bo4e.bo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10343 2023-08-08 07:09:16.000000 bo4e-0.5.4/docs/api/bo4e.com.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12407 2023-08-08 07:09:16.000000 bo4e-0.5.4/docs/api/bo4e.enum.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-08 07:09:16.000000 bo4e-0.5.4/docs/api/bo4e.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-08 07:09:16.000000 bo4e-0.5.4/docs/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-08 07:09:16.000000 bo4e-0.5.4/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-08 07:09:16.000000 bo4e-0.5.4/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-08-08 07:09:16.000000 bo4e-0.5.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-08-08 07:09:16.000000 bo4e-0.5.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-08 07:09:16.000000 bo4e-0.5.4/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-08 07:09:16.000000 bo4e-0.5.4/docs/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-08 07:09:16.000000 bo4e-0.5.4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-08-08 07:09:16.000000 bo4e-0.5.4/docs/test_uml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28380 2023-08-08 07:09:16.000000 bo4e-0.5.4/docs/uml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:09:27.871183 bo4e-0.5.4/json_schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:09:27.875183 bo4e-0.5.4/json_schemas/bo/
+-rw-r--r--   0 runner    (1001) docker     (123)    51662 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/bo/Angebot.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20861 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/bo/Ansprechpartner.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30039 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/bo/Ausschreibung.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31018 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/bo/Buendelvertrag.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/bo/Energiemenge.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18226 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/bo/Fremdkosten.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/bo/Geschaeftsobjekt.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/bo/Geschaeftspartner.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17575 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/bo/Kosten.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/bo/Lastgang.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10704 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/bo/LastgangKompakt.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24248 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/bo/Marktlokation.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/bo/Marktteilnehmer.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30665 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/bo/Messlokation.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35920 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/bo/Netznutzungsrechnung.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31358 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/bo/Preisblatt.json
+-rw-r--r--   0 runner    (1001) docker     (123)    37279 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/bo/PreisblattDienstleistung.json
+-rw-r--r--   0 runner    (1001) docker     (123)    37788 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/bo/PreisblattHardware.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31923 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/bo/PreisblattKonzessionsabgabe.json
+-rw-r--r--   0 runner    (1001) docker     (123)    37797 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/bo/PreisblattMessung.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32989 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/bo/PreisblattNetznutzung.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34002 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/bo/Rechnung.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/bo/Region.json
+-rw-r--r--   0 runner    (1001) docker     (123)    63902 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/bo/Regionaltarif.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/bo/Standorteigenschaften.json
+-rw-r--r--   0 runner    (1001) docker     (123)    61162 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/bo/Tarif.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30304 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/bo/Tarifinfo.json
+-rw-r--r--   0 runner    (1001) docker     (123)    43186 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/bo/Tarifkosten.json
+-rw-r--r--   0 runner    (1001) docker     (123)    57802 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/bo/Tarifpreisblatt.json
+-rw-r--r--   0 runner    (1001) docker     (123)    27127 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/bo/Vertrag.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19710 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/bo/Zaehler.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9718 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/bo/Zeitreihe.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/bo/_LastgangBody.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:09:27.879183 bo4e-0.5.4/json_schemas/com/
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Adresse.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Angebotsposition.json
+-rw-r--r--   0 runner    (1001) docker     (123)    38449 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Angebotsteil.json
+-rw-r--r--   0 runner    (1001) docker     (123)    40573 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Angebotsvariante.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8864 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/AufAbschlag.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/AufAbschlagProOrt.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28916 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/AufAbschlagRegional.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/AufAbschlagstaffelProOrt.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13809 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Ausschreibungsdetail.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18479 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Ausschreibungslos.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Betrag.json
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/COM.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Dienstleistung.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Energieherkunft.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Energiemix.json
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/ExterneReferenz.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11326 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Fremdkostenblock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Fremdkostenposition.json
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Geokoordinaten.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Geraet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Geraeteeigenschaften.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Hardware.json
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Katasteradresse.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Kostenblock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Kostenposition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/KriteriumWert.json
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/MarktgebietInfo.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Menge.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Messlokationszuordnung.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/PositionsAufAbschlag.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Preis.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Preisgarantie.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11150 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Preisposition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Preisstaffel.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12985 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Rechnungsposition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/RegionaleGueltigkeit.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/RegionalePreisgarantie.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/RegionalePreisstaffel.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/RegionaleTarifpreisposition.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32018 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/RegionalerAufAbschlag.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Regionskriterium.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Rufnummer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Sigmoidparameter.json
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/StandorteigenschaftenAllgemein.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/StandorteigenschaftenGas.json
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/StandorteigenschaftenStrom.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Steuerbetrag.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Tagesvektor.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Tarifberechnungsparameter.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9076 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Tarifeinschraenkung.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Tarifpreis.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Tarifpreisposition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/TarifpreispositionProOrt.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/TarifpreisstaffelProOrt.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Unterschrift.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Verbrauch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Vertragskonditionen.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Vertragsteil.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Zaehlwerk.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Zeitintervall.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Zeitraum.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Zeitreihenwert.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Zeitreihenwertkompakt.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/com/Zustaendigkeit.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-08-08 07:09:16.000000 bo4e-0.5.4/json_schemas/generate_json_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-08-08 07:09:16.000000 bo4e-0.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-08 07:09:16.000000 bo4e-0.5.4/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-08-08 07:09:16.000000 bo4e-0.5.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-08-08 07:09:27.907184 bo4e-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-08 07:09:16.000000 bo4e-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:09:27.867183 bo4e-0.5.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:09:27.883183 bo4e-0.5.4/src/bo4e/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:09:27.883183 bo4e-0.5.4/src/bo4e/bo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/bo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/bo/angebot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/bo/ansprechpartner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/bo/ausschreibung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/bo/buendelvertrag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/bo/energiemenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/bo/fremdkosten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/bo/geschaeftsobjekt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/bo/geschaeftspartner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/bo/kosten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/bo/lastgang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/bo/marktlokation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/bo/marktteilnehmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/bo/messlokation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/bo/netznutzungsrechnung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/bo/preisblatt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/bo/preisblattdienstleistung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/bo/preisblatthardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/bo/preisblattkonzessionsabgabe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/bo/preisblattmessung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/bo/preisblattnetznutzung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/bo/rechnung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/bo/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/bo/regionaltarif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/bo/standorteigenschaften.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/bo/tarif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/bo/tarifinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/bo/tarifkosten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/bo/tarifpreisblatt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/bo/vertrag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/bo/zaehler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/bo/zeitreihe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:09:27.891183 bo4e-0.5.4/src/bo4e/com/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/adresse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/angebotsposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/angebotsteil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/angebotsvariante.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/aufabschlag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/aufabschlagproort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/aufabschlagregional.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/aufabschlagstaffelproort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/ausschreibungsdetail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/ausschreibungslos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/betrag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/com.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/dienstleistung.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/energieherkunft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/energiemix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/externereferenz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/fremdkostenblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/fremdkostenposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/geokoordinaten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/geraet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/geraeteeigenschaften.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/katasteradresse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/kostenblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/kostenposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/kriteriumwert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/marktgebietinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/menge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/messlokationszuordnung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/positionsaufabschlag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/preis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/preisgarantie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/preisposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/preisstaffel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/rechnungsposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/regionalegueltigkeit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/regionalepreisgarantie.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/regionalepreisstaffel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/regionaleraufabschlag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/regionaletarifpreisposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/regionskriterium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/rufnummer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/sigmoidparameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/standorteigenschaftengas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/standorteigenschaftenstrom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/steuerbetrag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/tagesvektor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/tarifberechnungsparameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/tarifeinschraenkung.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/tarifpreis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/tarifpreisposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/tarifpreispositionproort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/tarifpreisstaffelproort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/unterschrift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/verbrauch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/vertragskonditionen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/vertragsteil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/zaehlwerk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/zeitintervall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/zeitraum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/zeitreihenwert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/zeitreihenwertkompakt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/com/zustaendigkeit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:09:27.899184 bo4e-0.5.4/src/bo4e/enum/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/angebotsstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/anrede.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/arithmetische_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/artikelid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/aufabschlagstyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/aufabschlagsziel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/ausschreibungsportal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/ausschreibungsstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/ausschreibungstyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/bdewartikelnummer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/bemessungsgroesse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/bilanzierungsmethode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/botyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/dienstleistungstyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/energierichtung.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/erzeugungsart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/gasqualitaet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/gebiettyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/geraetemerkmal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/geraetetyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/geschaeftspartnerrolle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/gueltigkeitstyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/kalkulationsmethode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/kontaktart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/kostenklasse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/kundengruppe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/kundengruppeka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/kundentyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/landescode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/leistungstyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/lokationstyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/marktrolle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/mengeneinheit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/mengenoperator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/messart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/messgroesse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/messpreistyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/messwertstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/messwertstatuszusatz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/netzebene.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/nnrechnungsart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/nnrechnungstyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/oekolabel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/oekozertifikat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/preisgarantietyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/preismodell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/preisstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/preistyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/rechnungslegung.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/rechnungsstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/rechnungstyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/regionskriteriumtyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/rollencodetyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/rufnummernart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/sparte.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/steuerkennzeichen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/strenum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/tarifart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/tarifkalkulationsmethode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/tarifmerkmal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/tarifregionskriterium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/tariftyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/tarifzeit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/themengebiet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/titel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/verbrauchsart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/vertragsart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/vertragsform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/vertragsstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/voraussetzungen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/waehrungscode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/waehrungseinheit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/wertermittlungsverfahren.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/zaehlerauspraegung.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/zaehlertyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/enum/zeiteinheit.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:09:27.899184 bo4e-0.5.4/src/bo4e/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-08-08 07:09:16.000000 bo4e-0.5.4/src/bo4e/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:09:27.883183 bo4e-0.5.4/src/bo4e.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-08-08 07:09:27.000000 bo4e-0.5.4/src/bo4e.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13420 2023-08-08 07:09:27.000000 bo4e-0.5.4/src/bo4e.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 07:09:27.000000 bo4e-0.5.4/src/bo4e.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 07:09:27.000000 bo4e-0.5.4/src/bo4e.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-08 07:09:27.000000 bo4e-0.5.4/src/bo4e.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-08 07:09:27.000000 bo4e-0.5.4/src/bo4e.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:09:27.907184 bo4e-0.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/serialization_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_adresse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_angebot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_angebotsposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_angebotsteil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_angebotsvariante.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_ansprechpartner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_aufabschlag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_aufabschlagproort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_aufabschlagregional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_aufabschlagstaffelproort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_ausschreibung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_ausschreibungsdetail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_ausschreibungslos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_betrag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_buendelvertrag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_bypassing_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:09:27.867183 bo4e-0.5.4/tests/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 07:09:27.907184 bo4e-0.5.4/tests/test_data/test_data_adresse/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_data/test_data_adresse/test_data_adresse_missing_plz.json
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_data/test_data_adresse/test_data_adresse_only_required_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_data/test_data_adresse/test_data_adresse_with_all_possible_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_doc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_energieherkunft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_energiemenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_energiemix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_externe_referenz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_fremdkosten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_fremdkostenblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_fremdkostenposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_geokoordinaten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_geraet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_geraeteeigenschaften.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_geschaeftsobjekt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_geschaeftspartner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_katasteradresse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_kosten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_kostenblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_kostenposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_kriteriumswert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_lastgang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_lastgangkompakt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_marktgebietinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_marktlokation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_marktteilnehmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_menge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_messlokation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_messlokationszuordnung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_netznutzungsrechnung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_positionsaufabschlag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_preis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_preisblatt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_preisblatt_dienstleistung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_preisblatt_hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_preisblatt_konzessionsabgabe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_preisblatt_messung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_preisblattnetznutzung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_preisgarantie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_preisposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_preisstaffel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_rechnung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_rechnungsposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_regionalegueltigkeit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_regionalepreisgarantie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_regionalepreisstaffel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_regionaleraufabschlag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_regionaletarifpreisposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_regionaltarif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_regionskriterium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_sigmoidparameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_standorteigenschaften.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_standorteigenschaftengas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_standorteigenschaftenstrom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_steuerbetrag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_tagesvektor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_tarif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_tarifberechnungsparameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_tarifeinschraenkung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_tarifinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_tarifkosten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_tarifpreis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_tarifpreisblatt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_tarifpreisposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_tarifpreispositionproort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_tarifpreisstaffelproort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_unterschrift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_verbrauch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_vertrag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_vertragskonditionen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_vertragsteil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_zaehler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_zeitintervall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_zeitraum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_zeitreihe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_zeitreihenwert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/test_zeitreihenwertkompakt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-08-08 07:09:16.000000 bo4e-0.5.4/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-08-08 07:09:16.000000 bo4e-0.5.4/tox.ini
```

### Comparing `bo4e-0.5.3/.github/ISSUE_TEMPLATE/funktionale-anforderung-an-den-bo4e-standard.md` & `bo4e-0.5.4/.github/ISSUE_TEMPLATE/funktionale-anforderung-an-den-bo4e-standard.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ---
 name: Funktionale Anforderung an den BO4E Standard
 about: Eine Anforderung die so noch nicht vom BO4E Standard abgedeckt ist und/oder
   ein Vorschlag, wie sie abzubilden wäre
 title: 'Ein aussagekräftiger Titel: Hunde- und Katzentarife können nicht abgebildet
   werden'
 labels: BO4E Enhancement Proposal
-assignees: ''
+assignees: '@bo4e/the-gremium'
 
 ---
 
 Bitte **möglichst kleinteilig** pro Problem oder Anmerkung genau ein Ticket eröffnen anstatt alle Probleme, Gedanken oder Verbesserungsvorschläge in ein Mega-Ticket zu verpacken. Das erleichtert die Umsetzung und Diskussion ganz massiv.
 
 **Die fachliche Anforderung**
```

### Comparing `bo4e-0.5.3/.github/ISSUE_TEMPLATE/technisches-problem---python-specific-problem.md` & `bo4e-0.5.4/.github/ISSUE_TEMPLATE/technisches-problem---python-specific-problem.md`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/.github/dependabot.yml` & `bo4e-0.5.4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/.github/workflows/codeql-analysis.yml` & `bo4e-0.5.4/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/.github/workflows/coverage.yml` & `bo4e-0.5.4/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/.github/workflows/docs.yml` & `bo4e-0.5.4/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/.github/workflows/formatting.yml` & `bo4e-0.5.4/.github/workflows/formatting.yml`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/.github/workflows/linting.yml` & `bo4e-0.5.4/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/.github/workflows/python-publish.yml` & `bo4e-0.5.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/.github/workflows/tests.yml` & `bo4e-0.5.4/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/.gitignore` & `bo4e-0.5.4/.gitignore`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/.pre-commit-config.yaml` & `bo4e-0.5.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/.pylintrc` & `bo4e-0.5.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/.readthedocs.yaml` & `bo4e-0.5.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/CONTRIBUTING.md` & `bo4e-0.5.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/LICENSE.rst` & `bo4e-0.5.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/PKG-INFO` & `bo4e-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bo4e
-Version: 0.5.3
+Version: 0.5.4
 Summary: Python Library that implements the BO4E Standard.
 Home-page: https://github.com/Hochfrequenz/BO4E-python
 Author: Kevin Krechan
 Author-email: kevin.krechan@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://bo4e-python.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/Hochfrequenz/BO4E-python
```

### Comparing `bo4e-0.5.3/README.rst` & `bo4e-0.5.4/README.rst`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/docs/Makefile` & `bo4e-0.5.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/docs/_static/bo4e-python-favicon.png` & `bo4e-0.5.4/docs/_static/bo4e-python-favicon.png`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/docs/_static/bo4e-python-favicon.svg` & `bo4e-0.5.4/docs/_static/bo4e-python-favicon.svg`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/docs/_static/bo4e-python-logo.png` & `bo4e-0.5.4/docs/_static/bo4e-python-logo.png`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/docs/_static/bo4e-python-logo.svg` & `bo4e-0.5.4/docs/_static/bo4e-python-logo.svg`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/docs/api/bo4e.bo.rst` & `bo4e-0.5.4/docs/api/bo4e.bo.rst`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/docs/api/bo4e.com.rst` & `bo4e-0.5.4/docs/api/bo4e.com.rst`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/docs/api/bo4e.enum.rst` & `bo4e-0.5.4/docs/api/bo4e.enum.rst`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/docs/conf.py` & `bo4e-0.5.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/docs/index.rst` & `bo4e-0.5.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/docs/uml.py` & `bo4e-0.5.4/docs/uml.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/bo/Angebot.json` & `bo4e-0.5.4/json_schemas/bo/Angebot.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/bo/Ansprechpartner.json` & `bo4e-0.5.4/json_schemas/bo/Ansprechpartner.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/bo/Ausschreibung.json` & `bo4e-0.5.4/json_schemas/bo/Ausschreibung.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/bo/Buendelvertrag.json` & `bo4e-0.5.4/json_schemas/bo/Buendelvertrag.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/bo/Energiemenge.json` & `bo4e-0.5.4/json_schemas/bo/Energiemenge.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/bo/Fremdkosten.json` & `bo4e-0.5.4/json_schemas/bo/Fremdkosten.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/bo/Geschaeftsobjekt.json` & `bo4e-0.5.4/json_schemas/bo/Geschaeftsobjekt.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/bo/Geschaeftspartner.json` & `bo4e-0.5.4/json_schemas/bo/Geschaeftspartner.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/bo/Kosten.json` & `bo4e-0.5.4/json_schemas/bo/Kosten.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/bo/Lastgang.json` & `bo4e-0.5.4/json_schemas/bo/Lastgang.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/bo/LastgangKompakt.json` & `bo4e-0.5.4/json_schemas/bo/LastgangKompakt.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/bo/Marktlokation.json` & `bo4e-0.5.4/json_schemas/bo/Marktlokation.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/bo/Marktteilnehmer.json` & `bo4e-0.5.4/json_schemas/bo/Marktteilnehmer.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/bo/Messlokation.json` & `bo4e-0.5.4/json_schemas/bo/Messlokation.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/bo/Netznutzungsrechnung.json` & `bo4e-0.5.4/json_schemas/bo/Netznutzungsrechnung.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/bo/Preisblatt.json` & `bo4e-0.5.4/json_schemas/bo/Preisblatt.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/bo/PreisblattDienstleistung.json` & `bo4e-0.5.4/json_schemas/bo/PreisblattDienstleistung.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/bo/PreisblattHardware.json` & `bo4e-0.5.4/json_schemas/bo/PreisblattHardware.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/bo/PreisblattKonzessionsabgabe.json` & `bo4e-0.5.4/json_schemas/bo/PreisblattKonzessionsabgabe.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/bo/PreisblattMessung.json` & `bo4e-0.5.4/json_schemas/bo/PreisblattMessung.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/bo/PreisblattNetznutzung.json` & `bo4e-0.5.4/json_schemas/bo/PreisblattNetznutzung.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/bo/Rechnung.json` & `bo4e-0.5.4/json_schemas/bo/Rechnung.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/bo/Region.json` & `bo4e-0.5.4/json_schemas/bo/Region.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/bo/Regionaltarif.json` & `bo4e-0.5.4/json_schemas/bo/Regionaltarif.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/bo/Standorteigenschaften.json` & `bo4e-0.5.4/json_schemas/bo/Standorteigenschaften.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/bo/Tarif.json` & `bo4e-0.5.4/json_schemas/bo/Tarif.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/bo/Tarifinfo.json` & `bo4e-0.5.4/json_schemas/bo/Tarifinfo.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/bo/Tarifkosten.json` & `bo4e-0.5.4/json_schemas/bo/Tarifkosten.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/bo/Tarifpreisblatt.json` & `bo4e-0.5.4/json_schemas/bo/Tarifpreisblatt.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/bo/Vertrag.json` & `bo4e-0.5.4/json_schemas/bo/Vertrag.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/bo/Zaehler.json` & `bo4e-0.5.4/json_schemas/bo/Zaehler.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/bo/Zeitreihe.json` & `bo4e-0.5.4/json_schemas/bo/Zeitreihe.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/bo/_LastgangBody.json` & `bo4e-0.5.4/json_schemas/bo/_LastgangBody.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Adresse.json` & `bo4e-0.5.4/json_schemas/com/Adresse.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Angebotsposition.json` & `bo4e-0.5.4/json_schemas/com/Angebotsposition.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Angebotsteil.json` & `bo4e-0.5.4/json_schemas/com/Angebotsteil.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Angebotsvariante.json` & `bo4e-0.5.4/json_schemas/com/Angebotsvariante.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/AufAbschlag.json` & `bo4e-0.5.4/json_schemas/com/AufAbschlag.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/AufAbschlagProOrt.json` & `bo4e-0.5.4/json_schemas/com/AufAbschlagProOrt.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/AufAbschlagRegional.json` & `bo4e-0.5.4/json_schemas/com/AufAbschlagRegional.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/AufAbschlagstaffelProOrt.json` & `bo4e-0.5.4/json_schemas/com/AufAbschlagstaffelProOrt.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Ausschreibungsdetail.json` & `bo4e-0.5.4/json_schemas/com/Ausschreibungsdetail.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Ausschreibungslos.json` & `bo4e-0.5.4/json_schemas/com/Ausschreibungslos.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Betrag.json` & `bo4e-0.5.4/json_schemas/com/Betrag.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Dienstleistung.json` & `bo4e-0.5.4/json_schemas/com/Dienstleistung.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Energieherkunft.json` & `bo4e-0.5.4/json_schemas/com/Energieherkunft.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Energiemix.json` & `bo4e-0.5.4/json_schemas/com/Energiemix.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/ExterneReferenz.json` & `bo4e-0.5.4/json_schemas/com/ExterneReferenz.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Fremdkostenblock.json` & `bo4e-0.5.4/json_schemas/com/Fremdkostenblock.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Fremdkostenposition.json` & `bo4e-0.5.4/json_schemas/com/Fremdkostenposition.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Geokoordinaten.json` & `bo4e-0.5.4/json_schemas/com/Geokoordinaten.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Geraet.json` & `bo4e-0.5.4/json_schemas/com/Geraet.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Geraeteeigenschaften.json` & `bo4e-0.5.4/json_schemas/com/Geraeteeigenschaften.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Hardware.json` & `bo4e-0.5.4/json_schemas/com/Hardware.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Katasteradresse.json` & `bo4e-0.5.4/json_schemas/com/Katasteradresse.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Kostenblock.json` & `bo4e-0.5.4/json_schemas/com/Kostenblock.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Kostenposition.json` & `bo4e-0.5.4/json_schemas/com/Kostenposition.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/KriteriumWert.json` & `bo4e-0.5.4/json_schemas/com/KriteriumWert.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/MarktgebietInfo.json` & `bo4e-0.5.4/json_schemas/com/MarktgebietInfo.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Menge.json` & `bo4e-0.5.4/json_schemas/com/Menge.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Messlokationszuordnung.json` & `bo4e-0.5.4/json_schemas/com/Messlokationszuordnung.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/PositionsAufAbschlag.json` & `bo4e-0.5.4/json_schemas/com/PositionsAufAbschlag.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Preis.json` & `bo4e-0.5.4/json_schemas/com/Preis.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Preisgarantie.json` & `bo4e-0.5.4/json_schemas/com/Preisgarantie.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Preisposition.json` & `bo4e-0.5.4/json_schemas/com/Preisposition.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Preisstaffel.json` & `bo4e-0.5.4/json_schemas/com/Preisstaffel.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Rechnungsposition.json` & `bo4e-0.5.4/json_schemas/com/Rechnungsposition.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/RegionaleGueltigkeit.json` & `bo4e-0.5.4/json_schemas/com/RegionaleGueltigkeit.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/RegionalePreisgarantie.json` & `bo4e-0.5.4/json_schemas/com/RegionalePreisgarantie.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/RegionalePreisstaffel.json` & `bo4e-0.5.4/json_schemas/com/RegionalePreisstaffel.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/RegionaleTarifpreisposition.json` & `bo4e-0.5.4/json_schemas/com/RegionaleTarifpreisposition.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/RegionalerAufAbschlag.json` & `bo4e-0.5.4/json_schemas/com/RegionalerAufAbschlag.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Regionskriterium.json` & `bo4e-0.5.4/json_schemas/com/Regionskriterium.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Rufnummer.json` & `bo4e-0.5.4/json_schemas/com/Rufnummer.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Sigmoidparameter.json` & `bo4e-0.5.4/json_schemas/com/Sigmoidparameter.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/StandorteigenschaftenAllgemein.json` & `bo4e-0.5.4/json_schemas/com/StandorteigenschaftenAllgemein.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/StandorteigenschaftenGas.json` & `bo4e-0.5.4/json_schemas/com/StandorteigenschaftenGas.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/StandorteigenschaftenStrom.json` & `bo4e-0.5.4/json_schemas/com/StandorteigenschaftenStrom.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Steuerbetrag.json` & `bo4e-0.5.4/json_schemas/com/Steuerbetrag.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Tagesvektor.json` & `bo4e-0.5.4/json_schemas/com/Tagesvektor.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Tarifberechnungsparameter.json` & `bo4e-0.5.4/json_schemas/com/Tarifberechnungsparameter.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Tarifeinschraenkung.json` & `bo4e-0.5.4/json_schemas/com/Tarifeinschraenkung.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Tarifpreis.json` & `bo4e-0.5.4/json_schemas/com/Tarifpreis.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Tarifpreisposition.json` & `bo4e-0.5.4/json_schemas/com/Tarifpreisposition.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/TarifpreispositionProOrt.json` & `bo4e-0.5.4/json_schemas/com/TarifpreispositionProOrt.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/TarifpreisstaffelProOrt.json` & `bo4e-0.5.4/json_schemas/com/TarifpreisstaffelProOrt.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Unterschrift.json` & `bo4e-0.5.4/json_schemas/com/Unterschrift.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Verbrauch.json` & `bo4e-0.5.4/json_schemas/com/Verbrauch.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Vertragskonditionen.json` & `bo4e-0.5.4/json_schemas/com/Vertragskonditionen.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Vertragsteil.json` & `bo4e-0.5.4/json_schemas/com/Vertragsteil.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Zaehlwerk.json` & `bo4e-0.5.4/json_schemas/com/Zaehlwerk.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Zeitintervall.json` & `bo4e-0.5.4/json_schemas/com/Zeitintervall.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Zeitraum.json` & `bo4e-0.5.4/json_schemas/com/Zeitraum.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Zeitreihenwert.json` & `bo4e-0.5.4/json_schemas/com/Zeitreihenwert.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Zeitreihenwertkompakt.json` & `bo4e-0.5.4/json_schemas/com/Zeitreihenwertkompakt.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/com/Zustaendigkeit.json` & `bo4e-0.5.4/json_schemas/com/Zustaendigkeit.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/json_schemas/generate_json_schemas.py` & `bo4e-0.5.4/json_schemas/generate_json_schemas.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/pyproject.toml` & `bo4e-0.5.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/setup.cfg` & `bo4e-0.5.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/bo/angebot.py` & `bo4e-0.5.4/src/bo4e/bo/angebot.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/bo/ansprechpartner.py` & `bo4e-0.5.4/src/bo4e/bo/ansprechpartner.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/bo/ausschreibung.py` & `bo4e-0.5.4/src/bo4e/bo/ausschreibung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/bo/buendelvertrag.py` & `bo4e-0.5.4/src/bo4e/bo/buendelvertrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/bo/energiemenge.py` & `bo4e-0.5.4/src/bo4e/bo/energiemenge.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/bo/fremdkosten.py` & `bo4e-0.5.4/src/bo4e/bo/fremdkosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/bo/geschaeftsobjekt.py` & `bo4e-0.5.4/src/bo4e/bo/geschaeftsobjekt.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/bo/geschaeftspartner.py` & `bo4e-0.5.4/src/bo4e/bo/geschaeftspartner.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/bo/kosten.py` & `bo4e-0.5.4/src/bo4e/bo/kosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/bo/lastgang.py` & `bo4e-0.5.4/src/bo4e/bo/lastgang.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/bo/marktlokation.py` & `bo4e-0.5.4/src/bo4e/bo/marktlokation.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/bo/marktteilnehmer.py` & `bo4e-0.5.4/src/bo4e/bo/marktteilnehmer.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/bo/messlokation.py` & `bo4e-0.5.4/src/bo4e/bo/messlokation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Contains Messlokation class
 and corresponding marshmallow schema for de-/serialization
 """
 import re
-from typing import Annotated, List, Optional
+from typing import Annotated, Any, List, Optional
 
 from iso3166 import countries
 from pydantic import Field, field_validator, model_validator
 
 from bo4e.bo.geschaeftsobjekt import Geschaeftsobjekt
 from bo4e.bo.zaehler import Zaehler
 from bo4e.com.adresse import Adresse
@@ -114,14 +114,18 @@
             (0, 0, 0),
         },
         custom_error_message="More than one address information is given.",
     )
     "Checks that if an address is given, that there is only one valid address given"
 
     # pylint: disable=no-self-argument
-    @model_validator(mode="after")  # type:ignore[arg-type]
+    @model_validator(mode="before")
     @classmethod
-    def validate_grundzustaendiger_x_codenr(cls, model: "Messlokation") -> "Messlokation":
+    def validate_grundzustaendiger_x_codenr(cls, data: Any) -> dict[str, Any]:
         """Checks that if a codenr is given, that there is only one valid codenr given."""
-        if model.grundzustaendiger_msb_codenr is not None and model.grundzustaendiger_msbim_codenr is not None:
+        assert isinstance(data, dict), "data is not a dict"
+        if (
+            data.get("grundzustaendiger_msb_codenr", None) is not None
+            and data.get("grundzustaendiger_msbim_codenr", None) is not None
+        ):
             raise ValueError("More than one codenr is given.")
-        return model
+        return data
```

### Comparing `bo4e-0.5.3/src/bo4e/bo/netznutzungsrechnung.py` & `bo4e-0.5.4/src/bo4e/bo/netznutzungsrechnung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/bo/preisblatt.py` & `bo4e-0.5.4/src/bo4e/bo/preisblatt.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/bo/preisblattdienstleistung.py` & `bo4e-0.5.4/src/bo4e/bo/preisblattdienstleistung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/bo/preisblatthardware.py` & `bo4e-0.5.4/src/bo4e/bo/preisblatthardware.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/bo/preisblattkonzessionsabgabe.py` & `bo4e-0.5.4/src/bo4e/bo/preisblattkonzessionsabgabe.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/bo/preisblattmessung.py` & `bo4e-0.5.4/src/bo4e/bo/preisblattmessung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/bo/preisblattnetznutzung.py` & `bo4e-0.5.4/src/bo4e/bo/preisblattnetznutzung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/bo/rechnung.py` & `bo4e-0.5.4/src/bo4e/bo/rechnung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/bo/region.py` & `bo4e-0.5.4/src/bo4e/bo/region.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/bo/regionaltarif.py` & `bo4e-0.5.4/src/bo4e/bo/regionaltarif.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/bo/standorteigenschaften.py` & `bo4e-0.5.4/src/bo4e/bo/standorteigenschaften.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/bo/tarif.py` & `bo4e-0.5.4/src/bo4e/bo/tarif.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/bo/tarifinfo.py` & `bo4e-0.5.4/src/bo4e/bo/tarifinfo.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/bo/tarifkosten.py` & `bo4e-0.5.4/src/bo4e/bo/tarifkosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/bo/tarifpreisblatt.py` & `bo4e-0.5.4/src/bo4e/bo/tarifpreisblatt.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/bo/vertrag.py` & `bo4e-0.5.4/src/bo4e/bo/vertrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/bo/zaehler.py` & `bo4e-0.5.4/src/bo4e/bo/zaehler.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/bo/zeitreihe.py` & `bo4e-0.5.4/src/bo4e/bo/zeitreihe.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/adresse.py` & `bo4e-0.5.4/src/bo4e/com/adresse.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/angebotsposition.py` & `bo4e-0.5.4/src/bo4e/com/angebotsposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/angebotsteil.py` & `bo4e-0.5.4/src/bo4e/com/angebotsteil.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/angebotsvariante.py` & `bo4e-0.5.4/src/bo4e/com/angebotsvariante.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/aufabschlag.py` & `bo4e-0.5.4/src/bo4e/com/aufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/aufabschlagproort.py` & `bo4e-0.5.4/src/bo4e/com/aufabschlagproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/aufabschlagregional.py` & `bo4e-0.5.4/src/bo4e/com/aufabschlagregional.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/aufabschlagstaffelproort.py` & `bo4e-0.5.4/src/bo4e/com/aufabschlagstaffelproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/ausschreibungsdetail.py` & `bo4e-0.5.4/src/bo4e/com/ausschreibungsdetail.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/ausschreibungslos.py` & `bo4e-0.5.4/src/bo4e/com/ausschreibungslos.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/betrag.py` & `bo4e-0.5.4/src/bo4e/com/betrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/com.py` & `bo4e-0.5.4/src/bo4e/com/com.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/dienstleistung.py` & `bo4e-0.5.4/src/bo4e/com/dienstleistung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/energieherkunft.py` & `bo4e-0.5.4/src/bo4e/com/energieherkunft.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/energiemix.py` & `bo4e-0.5.4/src/bo4e/com/energiemix.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/externereferenz.py` & `bo4e-0.5.4/src/bo4e/com/externereferenz.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/fremdkostenblock.py` & `bo4e-0.5.4/src/bo4e/com/fremdkostenblock.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/fremdkostenposition.py` & `bo4e-0.5.4/src/bo4e/com/fremdkostenposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/geokoordinaten.py` & `bo4e-0.5.4/src/bo4e/com/geokoordinaten.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/geraet.py` & `bo4e-0.5.4/src/bo4e/com/geraet.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/geraeteeigenschaften.py` & `bo4e-0.5.4/src/bo4e/com/geraeteeigenschaften.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/hardware.py` & `bo4e-0.5.4/src/bo4e/com/hardware.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/katasteradresse.py` & `bo4e-0.5.4/src/bo4e/com/katasteradresse.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/kostenblock.py` & `bo4e-0.5.4/src/bo4e/com/kostenblock.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/kostenposition.py` & `bo4e-0.5.4/src/bo4e/com/kostenposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/kriteriumwert.py` & `bo4e-0.5.4/src/bo4e/com/kriteriumwert.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/marktgebietinfo.py` & `bo4e-0.5.4/src/bo4e/com/marktgebietinfo.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/menge.py` & `bo4e-0.5.4/src/bo4e/com/menge.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/messlokationszuordnung.py` & `bo4e-0.5.4/src/bo4e/com/messlokationszuordnung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/positionsaufabschlag.py` & `bo4e-0.5.4/src/bo4e/com/positionsaufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/preis.py` & `bo4e-0.5.4/src/bo4e/com/preis.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/preisgarantie.py` & `bo4e-0.5.4/src/bo4e/com/preisgarantie.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/preisposition.py` & `bo4e-0.5.4/src/bo4e/com/preisposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/preisstaffel.py` & `bo4e-0.5.4/src/bo4e/com/preisstaffel.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/rechnungsposition.py` & `bo4e-0.5.4/src/bo4e/com/rechnungsposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/regionalegueltigkeit.py` & `bo4e-0.5.4/src/bo4e/com/regionalegueltigkeit.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/regionalepreisgarantie.py` & `bo4e-0.5.4/src/bo4e/com/regionalepreisgarantie.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/regionalepreisstaffel.py` & `bo4e-0.5.4/src/bo4e/com/regionalepreisstaffel.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/regionaleraufabschlag.py` & `bo4e-0.5.4/src/bo4e/com/regionaleraufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/regionaletarifpreisposition.py` & `bo4e-0.5.4/src/bo4e/com/regionaletarifpreisposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/regionskriterium.py` & `bo4e-0.5.4/src/bo4e/com/regionskriterium.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/rufnummer.py` & `bo4e-0.5.4/src/bo4e/com/rufnummer.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/sigmoidparameter.py` & `bo4e-0.5.4/src/bo4e/com/sigmoidparameter.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/standorteigenschaftengas.py` & `bo4e-0.5.4/src/bo4e/com/standorteigenschaftengas.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/standorteigenschaftenstrom.py` & `bo4e-0.5.4/src/bo4e/com/standorteigenschaftenstrom.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/steuerbetrag.py` & `bo4e-0.5.4/src/bo4e/com/steuerbetrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/tagesvektor.py` & `bo4e-0.5.4/src/bo4e/com/tagesvektor.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/tarifberechnungsparameter.py` & `bo4e-0.5.4/src/bo4e/com/tarifberechnungsparameter.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/tarifeinschraenkung.py` & `bo4e-0.5.4/src/bo4e/com/tarifeinschraenkung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/tarifpreis.py` & `bo4e-0.5.4/src/bo4e/com/tarifpreis.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/tarifpreisposition.py` & `bo4e-0.5.4/src/bo4e/com/tarifpreisposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/tarifpreispositionproort.py` & `bo4e-0.5.4/src/bo4e/com/tarifpreispositionproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/tarifpreisstaffelproort.py` & `bo4e-0.5.4/src/bo4e/com/tarifpreisstaffelproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/unterschrift.py` & `bo4e-0.5.4/src/bo4e/com/unterschrift.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/verbrauch.py` & `bo4e-0.5.4/src/bo4e/com/verbrauch.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/vertragskonditionen.py` & `bo4e-0.5.4/src/bo4e/com/vertragskonditionen.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/vertragsteil.py` & `bo4e-0.5.4/src/bo4e/com/vertragsteil.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/zaehlwerk.py` & `bo4e-0.5.4/src/bo4e/com/zaehlwerk.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/zeitintervall.py` & `bo4e-0.5.4/src/bo4e/com/zeitintervall.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/zeitraum.py` & `bo4e-0.5.4/src/bo4e/com/zeitraum.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/zeitreihenwert.py` & `bo4e-0.5.4/src/bo4e/com/zeitreihenwert.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/zeitreihenwertkompakt.py` & `bo4e-0.5.4/src/bo4e/com/zeitreihenwertkompakt.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/com/zustaendigkeit.py` & `bo4e-0.5.4/src/bo4e/com/zustaendigkeit.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/angebotsstatus.py` & `bo4e-0.5.4/src/bo4e/enum/angebotsstatus.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/artikelid.py` & `bo4e-0.5.4/src/bo4e/enum/artikelid.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/aufabschlagsziel.py` & `bo4e-0.5.4/src/bo4e/enum/aufabschlagsziel.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/ausschreibungsportal.py` & `bo4e-0.5.4/src/bo4e/enum/ausschreibungsportal.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/bdewartikelnummer.py` & `bo4e-0.5.4/src/bo4e/enum/bdewartikelnummer.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/bemessungsgroesse.py` & `bo4e-0.5.4/src/bo4e/enum/bemessungsgroesse.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/bilanzierungsmethode.py` & `bo4e-0.5.4/src/bo4e/enum/bilanzierungsmethode.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/botyp.py` & `bo4e-0.5.4/src/bo4e/enum/botyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/dienstleistungstyp.py` & `bo4e-0.5.4/src/bo4e/enum/dienstleistungstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/erzeugungsart.py` & `bo4e-0.5.4/src/bo4e/enum/erzeugungsart.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/gebiettyp.py` & `bo4e-0.5.4/src/bo4e/enum/gebiettyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/geraetemerkmal.py` & `bo4e-0.5.4/src/bo4e/enum/geraetemerkmal.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/geraetetyp.py` & `bo4e-0.5.4/src/bo4e/enum/geraetetyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/gueltigkeitstyp.py` & `bo4e-0.5.4/src/bo4e/enum/gueltigkeitstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/kalkulationsmethode.py` & `bo4e-0.5.4/src/bo4e/enum/kalkulationsmethode.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/kostenklasse.py` & `bo4e-0.5.4/src/bo4e/enum/kostenklasse.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/kundengruppe.py` & `bo4e-0.5.4/src/bo4e/enum/kundengruppe.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/kundengruppeka.py` & `bo4e-0.5.4/src/bo4e/enum/kundengruppeka.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/kundentyp.py` & `bo4e-0.5.4/src/bo4e/enum/kundentyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/leistungstyp.py` & `bo4e-0.5.4/src/bo4e/enum/leistungstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/marktrolle.py` & `bo4e-0.5.4/src/bo4e/enum/marktrolle.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/mengeneinheit.py` & `bo4e-0.5.4/src/bo4e/enum/mengeneinheit.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/messgroesse.py` & `bo4e-0.5.4/src/bo4e/enum/messgroesse.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/messpreistyp.py` & `bo4e-0.5.4/src/bo4e/enum/messpreistyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/messwertstatus.py` & `bo4e-0.5.4/src/bo4e/enum/messwertstatus.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/messwertstatuszusatz.py` & `bo4e-0.5.4/src/bo4e/enum/messwertstatuszusatz.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/netzebene.py` & `bo4e-0.5.4/src/bo4e/enum/netzebene.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/nnrechnungstyp.py` & `bo4e-0.5.4/src/bo4e/enum/nnrechnungstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/oekolabel.py` & `bo4e-0.5.4/src/bo4e/enum/oekolabel.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/oekozertifikat.py` & `bo4e-0.5.4/src/bo4e/enum/oekozertifikat.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/preisgarantietyp.py` & `bo4e-0.5.4/src/bo4e/enum/preisgarantietyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/preistyp.py` & `bo4e-0.5.4/src/bo4e/enum/preistyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/rechnungslegung.py` & `bo4e-0.5.4/src/bo4e/enum/rechnungslegung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/rechnungsstatus.py` & `bo4e-0.5.4/src/bo4e/enum/rechnungsstatus.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/rechnungstyp.py` & `bo4e-0.5.4/src/bo4e/enum/rechnungstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/regionskriteriumtyp.py` & `bo4e-0.5.4/src/bo4e/enum/regionskriteriumtyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/rufnummernart.py` & `bo4e-0.5.4/src/bo4e/enum/rufnummernart.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/steuerkennzeichen.py` & `bo4e-0.5.4/src/bo4e/enum/steuerkennzeichen.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/tarifkalkulationsmethode.py` & `bo4e-0.5.4/src/bo4e/enum/tarifkalkulationsmethode.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/tarifmerkmal.py` & `bo4e-0.5.4/src/bo4e/enum/tarifmerkmal.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/themengebiet.py` & `bo4e-0.5.4/src/bo4e/enum/themengebiet.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/vertragsart.py` & `bo4e-0.5.4/src/bo4e/enum/vertragsart.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/vertragsstatus.py` & `bo4e-0.5.4/src/bo4e/enum/vertragsstatus.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/voraussetzungen.py` & `bo4e-0.5.4/src/bo4e/enum/voraussetzungen.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/waehrungscode.py` & `bo4e-0.5.4/src/bo4e/enum/waehrungscode.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/zaehlertyp.py` & `bo4e-0.5.4/src/bo4e/enum/zaehlertyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/enum/zeiteinheit.py` & `bo4e-0.5.4/src/bo4e/enum/zeiteinheit.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/utils/__init__.py` & `bo4e-0.5.4/src/bo4e/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/src/bo4e/validators.py` & `bo4e-0.5.4/src/bo4e/validators.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,23 +41,23 @@
     if custom_boolean_converter is not None:
         supplied = custom_boolean_converter
     else:
 
         def supplied(value: Any) -> bool:
             return value is not None and (not isinstance(value, str) or value != "")
 
-    def validator(self: ModelT) -> ModelT:
-        bools = tuple(int(supplied(getattr(self, field))) for field in fields)
+    def validator(cls: type[ModelT], data: dict[str, Any]) -> dict[str, Any]:
+        bools = tuple(int(supplied(data.get(field, None))) for field in fields)
         if bools in valid_combinations:
-            return self
+            return data
         if custom_error_message:
             raise ValueError(custom_error_message)
-        raise ValueError(f"Invalid combination of fields {fields} for {self!r}: {bools}")
+        raise ValueError(f"Invalid combination of fields {fields} for {cls!r}: {bools}")
 
-    return model_validator(mode="after")(validator)
+    return model_validator(mode="before")(validator)
 
 
 # pylint:disable=unused-argument
 def einheit_only_for_abschlagstyp_absolut(  # type: ignore[no-untyped-def]
     cls, value: Waehrungseinheit, validation_info: ValidationInfo
 ) -> Waehrungseinheit:
     """
```

### Comparing `bo4e-0.5.3/src/bo4e.egg-info/PKG-INFO` & `bo4e-0.5.4/src/bo4e.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bo4e
-Version: 0.5.3
+Version: 0.5.4
 Summary: Python Library that implements the BO4E Standard.
 Home-page: https://github.com/Hochfrequenz/BO4E-python
 Author: Kevin Krechan
 Author-email: kevin.krechan@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://bo4e-python.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/Hochfrequenz/BO4E-python
```

### Comparing `bo4e-0.5.3/src/bo4e.egg-info/SOURCES.txt` & `bo4e-0.5.4/src/bo4e.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/serialization_helper.py` & `bo4e-0.5.4/tests/serialization_helper.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_adresse.py` & `bo4e-0.5.4/tests/test_adresse.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_angebot.py` & `bo4e-0.5.4/tests/test_angebot.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_angebotsposition.py` & `bo4e-0.5.4/tests/test_angebotsposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_angebotsteil.py` & `bo4e-0.5.4/tests/test_angebotsteil.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_angebotsvariante.py` & `bo4e-0.5.4/tests/test_angebotsvariante.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_ansprechpartner.py` & `bo4e-0.5.4/tests/test_ansprechpartner.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_aufabschlag.py` & `bo4e-0.5.4/tests/test_aufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_aufabschlagproort.py` & `bo4e-0.5.4/tests/test_aufabschlagproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_aufabschlagregional.py` & `bo4e-0.5.4/tests/test_aufabschlagregional.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_aufabschlagstaffelproort.py` & `bo4e-0.5.4/tests/test_aufabschlagstaffelproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_ausschreibung.py` & `bo4e-0.5.4/tests/test_ausschreibung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_ausschreibungsdetail.py` & `bo4e-0.5.4/tests/test_ausschreibungsdetail.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_ausschreibungslos.py` & `bo4e-0.5.4/tests/test_ausschreibungslos.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_betrag.py` & `bo4e-0.5.4/tests/test_betrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_buendelvertrag.py` & `bo4e-0.5.4/tests/test_buendelvertrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_bypassing_validation.py` & `bo4e-0.5.4/tests/test_bypassing_validation.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_energieherkunft.py` & `bo4e-0.5.4/tests/test_energieherkunft.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_energiemenge.py` & `bo4e-0.5.4/tests/test_energiemenge.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_energiemix.py` & `bo4e-0.5.4/tests/test_energiemix.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_enums.py` & `bo4e-0.5.4/tests/test_enums.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_externe_referenz.py` & `bo4e-0.5.4/tests/test_externe_referenz.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_fremdkosten.py` & `bo4e-0.5.4/tests/test_fremdkosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_fremdkostenblock.py` & `bo4e-0.5.4/tests/test_fremdkostenblock.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_fremdkostenposition.py` & `bo4e-0.5.4/tests/test_fremdkostenposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_geokoordinaten.py` & `bo4e-0.5.4/tests/test_geokoordinaten.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_geraet.py` & `bo4e-0.5.4/tests/test_geraet.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_geraeteeigenschaften.py` & `bo4e-0.5.4/tests/test_geraeteeigenschaften.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_geschaeftsobjekt.py` & `bo4e-0.5.4/tests/test_geschaeftsobjekt.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_geschaeftspartner.py` & `bo4e-0.5.4/tests/test_geschaeftspartner.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_kosten.py` & `bo4e-0.5.4/tests/test_kosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_kostenblock.py` & `bo4e-0.5.4/tests/test_kostenblock.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_kostenposition.py` & `bo4e-0.5.4/tests/test_kostenposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_kriteriumswert.py` & `bo4e-0.5.4/tests/test_kriteriumswert.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_lastgang.py` & `bo4e-0.5.4/tests/test_lastgang.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_lastgangkompakt.py` & `bo4e-0.5.4/tests/test_lastgangkompakt.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_marktlokation.py` & `bo4e-0.5.4/tests/test_marktlokation.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_marktteilnehmer.py` & `bo4e-0.5.4/tests/test_marktteilnehmer.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_menge.py` & `bo4e-0.5.4/tests/test_menge.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_messlokation.py` & `bo4e-0.5.4/tests/test_messlokation.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_messlokationszuordnung.py` & `bo4e-0.5.4/tests/test_messlokationszuordnung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_netznutzungsrechnung.py` & `bo4e-0.5.4/tests/test_netznutzungsrechnung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_positionsaufabschlag.py` & `bo4e-0.5.4/tests/test_positionsaufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_preis.py` & `bo4e-0.5.4/tests/test_preis.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_preisblatt.py` & `bo4e-0.5.4/tests/test_preisblatt.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_preisblatt_dienstleistung.py` & `bo4e-0.5.4/tests/test_preisblatt_dienstleistung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_preisblatt_hardware.py` & `bo4e-0.5.4/tests/test_preisblatt_hardware.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_preisblatt_konzessionsabgabe.py` & `bo4e-0.5.4/tests/test_preisblatt_konzessionsabgabe.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_preisblatt_messung.py` & `bo4e-0.5.4/tests/test_preisblatt_messung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_preisblattnetznutzung.py` & `bo4e-0.5.4/tests/test_preisblattnetznutzung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_preisgarantie.py` & `bo4e-0.5.4/tests/test_preisgarantie.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_preisposition.py` & `bo4e-0.5.4/tests/test_preisposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_preisstaffel.py` & `bo4e-0.5.4/tests/test_preisstaffel.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_rechnung.py` & `bo4e-0.5.4/tests/test_rechnung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_rechnungsposition.py` & `bo4e-0.5.4/tests/test_rechnungsposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_region.py` & `bo4e-0.5.4/tests/test_region.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_regionalegueltigkeit.py` & `bo4e-0.5.4/tests/test_regionalegueltigkeit.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_regionalepreisgarantie.py` & `bo4e-0.5.4/tests/test_regionalepreisgarantie.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_regionalepreisstaffel.py` & `bo4e-0.5.4/tests/test_regionalepreisstaffel.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_regionaleraufabschlag.py` & `bo4e-0.5.4/tests/test_regionaleraufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_regionaletarifpreisposition.py` & `bo4e-0.5.4/tests/test_regionaletarifpreisposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_regionaltarif.py` & `bo4e-0.5.4/tests/test_regionaltarif.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_regionskriterium.py` & `bo4e-0.5.4/tests/test_regionskriterium.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_sigmoidparameter.py` & `bo4e-0.5.4/tests/test_sigmoidparameter.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_standorteigenschaften.py` & `bo4e-0.5.4/tests/test_standorteigenschaften.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_standorteigenschaftengas.py` & `bo4e-0.5.4/tests/test_standorteigenschaftengas.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_standorteigenschaftenstrom.py` & `bo4e-0.5.4/tests/test_standorteigenschaftenstrom.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_steuerbetrag.py` & `bo4e-0.5.4/tests/test_steuerbetrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_tagesvektor.py` & `bo4e-0.5.4/tests/test_tagesvektor.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_tarif.py` & `bo4e-0.5.4/tests/test_tarif.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_tarifberechnungsparameter.py` & `bo4e-0.5.4/tests/test_tarifberechnungsparameter.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_tarifeinschraenkung.py` & `bo4e-0.5.4/tests/test_tarifeinschraenkung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_tarifinfo.py` & `bo4e-0.5.4/tests/test_tarifinfo.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_tarifkosten.py` & `bo4e-0.5.4/tests/test_tarifkosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_tarifpreis.py` & `bo4e-0.5.4/tests/test_tarifpreis.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_tarifpreisblatt.py` & `bo4e-0.5.4/tests/test_tarifpreisblatt.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_tarifpreisposition.py` & `bo4e-0.5.4/tests/test_tarifpreisposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_tarifpreispositionproort.py` & `bo4e-0.5.4/tests/test_tarifpreispositionproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_tarifpreisstaffelproort.py` & `bo4e-0.5.4/tests/test_tarifpreisstaffelproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_unterschrift.py` & `bo4e-0.5.4/tests/test_unterschrift.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_verbrauch.py` & `bo4e-0.5.4/tests/test_verbrauch.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_vertrag.py` & `bo4e-0.5.4/tests/test_vertrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_vertragskonditionen.py` & `bo4e-0.5.4/tests/test_vertragskonditionen.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_vertragsteil.py` & `bo4e-0.5.4/tests/test_vertragsteil.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_zaehler.py` & `bo4e-0.5.4/tests/test_zaehler.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_zeitintervall.py` & `bo4e-0.5.4/tests/test_zeitintervall.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_zeitraum.py` & `bo4e-0.5.4/tests/test_zeitraum.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_zeitreihe.py` & `bo4e-0.5.4/tests/test_zeitreihe.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_zeitreihenwert.py` & `bo4e-0.5.4/tests/test_zeitreihenwert.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/test_zeitreihenwertkompakt.py` & `bo4e-0.5.4/tests/test_zeitreihenwertkompakt.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tests/utils.py` & `bo4e-0.5.4/tests/utils.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.3/tox.ini` & `bo4e-0.5.4/tox.ini`

 * *Files identical despite different names*

