# Comparing `tmp/PDKMaster-0.9.4.tar.gz` & `tmp/PDKMaster-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PDKMaster-0.9.4.tar", last modified: Wed Jul 26 12:05:03 2023, max compression
+gzip compressed data, was "PDKMaster-0.9.5.tar", last modified: Tue Aug  8 13:57:39 2023, max compression
```

## Comparing `PDKMaster-0.9.4.tar` & `PDKMaster-0.9.5.tar`

### file list

```diff
@@ -1,177 +1,177 @@
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.104557 PDKMaster-0.9.4/
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.072557 PDKMaster-0.9.4/.ci/
--rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)     1069 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/.ci/check-dco.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      155 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/.gitignore
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2183 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/.gitlab-ci.yml
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6586 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/Contributing.md
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      566 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/LICENSE.md
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.072557 PDKMaster-0.9.4/LICENSES/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    34523 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/LICENSES/agpl-3.0.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    11358 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/LICENSES/apache-2.0.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13419 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/LICENSES/cern_ohl_s_v2.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18009 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/LICENSES/gpl-2.0.txt
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.076557 PDKMaster-0.9.4/PDKMaster.egg-info/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9871 2023-07-26 12:05:02.000000 PDKMaster-0.9.4/PDKMaster.egg-info/PKG-INFO
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3966 2023-07-26 12:05:03.000000 PDKMaster-0.9.4/PDKMaster.egg-info/SOURCES.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        1 2023-07-26 12:05:02.000000 PDKMaster-0.9.4/PDKMaster.egg-info/dependency_links.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       61 2023-07-26 12:05:02.000000 PDKMaster-0.9.4/PDKMaster.egg-info/requires.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       15 2023-07-26 12:05:02.000000 PDKMaster-0.9.4/PDKMaster.egg-info/top_level.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9871 2023-07-26 12:05:03.104557 PDKMaster-0.9.4/PKG-INFO
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9403 2023-07-26 12:03:03.000000 PDKMaster-0.9.4/README.md
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.076557 PDKMaster-0.9.4/ReleaseNotes/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      442 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/ReleaseNotes/v0.1.md
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1234 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/ReleaseNotes/v0.2.0.md
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1471 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/ReleaseNotes/v0.3.0.md
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2547 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/ReleaseNotes/v0.9.0.md
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.076557 PDKMaster-0.9.4/assura_yaml/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        0 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/assura_yaml/.keepme
--rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)      595 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/checkskill.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       14 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/ci-requirements.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       61 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/dev-requirements.txt
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.076557 PDKMaster-0.9.4/display_yaml/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        0 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/display_yaml/.keepme
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.064557 PDKMaster-0.9.4/docs/
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.080557 PDKMaster-0.9.4/docs/src/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6063 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/docs/src/conf.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      456 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/docs/src/index.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      141 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/docs/src/pdkmaster._util.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      560 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/docs/src/pdkmaster.design.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      443 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/docs/src/pdkmaster.dispatch.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      312 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/docs/src/pdkmaster.io.coriolis.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      462 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/docs/src/pdkmaster.io.klayout.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      934 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/docs/src/pdkmaster.io.parsing.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      318 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/docs/src/pdkmaster.io.pdkmaster.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      262 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/docs/src/pdkmaster.io.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      449 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/docs/src/pdkmaster.io.spice.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      290 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/docs/src/pdkmaster.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1556 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/docs/src/pdkmaster.technology.rst
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3746 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/dodo.py
--rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)     4469 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/extract_rules.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    26261 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/files.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.080557 PDKMaster-0.9.4/pdkmaster/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      709 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18133 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/_util.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.080557 PDKMaster-0.9.4/pdkmaster/design/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      237 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/design/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6045 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/design/cell.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    10199 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/design/circuit.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     8637 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/design/factory.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.084557 PDKMaster-0.9.4/pdkmaster/design/layout/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      664 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/design/layout/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    28707 2023-07-26 08:56:45.000000 PDKMaster-0.9.4/pdkmaster/design/layout/_circuitlayouter.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    48052 2023-07-26 08:56:45.000000 PDKMaster-0.9.4/pdkmaster/design/layout/_primitivelayouter.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3335 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/design/layout/factory_.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    22622 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/design/layout/layout_.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2887 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/design/library.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2600 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/design/routinggauge.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.084557 PDKMaster-0.9.4/pdkmaster/dispatch/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1375 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/dispatch/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1378 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/dispatch/edge.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1956 2023-07-24 14:24:09.000000 PDKMaster-0.9.4/pdkmaster/dispatch/mask.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     8101 2023-07-26 08:56:38.000000 PDKMaster-0.9.4/pdkmaster/dispatch/primitive.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2803 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/dispatch/rule.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3801 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/dispatch/shape.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.084557 PDKMaster-0.9.4/pdkmaster/io/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/io/__init__.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.084557 PDKMaster-0.9.4/pdkmaster/io/coriolis/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      120 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/io/coriolis/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    58632 2023-07-26 08:24:56.000000 PDKMaster-0.9.4/pdkmaster/io/coriolis/export.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.084557 PDKMaster-0.9.4/pdkmaster/io/klayout/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      142 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/io/klayout/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    37919 2023-07-26 08:57:55.000000 PDKMaster-0.9.4/pdkmaster/io/klayout/export.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    23519 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/io/klayout/merge_.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.084557 PDKMaster-0.9.4/pdkmaster/io/lefdef/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      261 2023-07-25 08:57:03.000000 PDKMaster-0.9.4/pdkmaster/io/lefdef/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9948 2023-07-26 08:24:48.000000 PDKMaster-0.9.4/pdkmaster/io/lefdef/export.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.088557 PDKMaster-0.9.4/pdkmaster/io/notebook/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      121 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/io/notebook/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1253 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/io/notebook/plotter.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.088557 PDKMaster-0.9.4/pdkmaster/io/parsing/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      214 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/io/parsing/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18847 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/io/parsing/assura.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      422 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/io/parsing/display.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      822 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/io/parsing/layermap.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    17548 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/io/parsing/skill_grammar.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    24374 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/io/parsing/tf.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.088557 PDKMaster-0.9.4/pdkmaster/io/pdkmaster/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      120 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/io/pdkmaster/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18067 2023-07-26 08:56:38.000000 PDKMaster-0.9.4/pdkmaster/io/pdkmaster/export.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.088557 PDKMaster-0.9.4/pdkmaster/io/spice/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      165 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/io/spice/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    15809 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/io/spice/pyspice.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     5904 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/io/spice/spice_.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      181 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/io/spice/typing.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.092557 PDKMaster-0.9.4/pdkmaster/technology/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      276 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/technology/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4032 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/technology/edge.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    77846 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/technology/geometry.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18203 2023-07-26 09:02:44.000000 PDKMaster-0.9.4/pdkmaster/technology/mask.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      627 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/technology/net.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.092557 PDKMaster-0.9.4/pdkmaster/technology/primitive/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      466 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/technology/primitive/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    10122 2023-07-26 08:56:45.000000 PDKMaster-0.9.4/pdkmaster/technology/primitive/_core.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2421 2023-07-26 08:56:45.000000 PDKMaster-0.9.4/pdkmaster/technology/primitive/_derived.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1176 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/technology/primitive/_param.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    24164 2023-07-26 08:57:55.000000 PDKMaster-0.9.4/pdkmaster/technology/primitive/conductors.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    44879 2023-07-26 12:04:52.000000 PDKMaster-0.9.4/pdkmaster/technology/primitive/devices.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4914 2023-07-26 12:04:52.000000 PDKMaster-0.9.4/pdkmaster/technology/primitive/layers.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6752 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/technology/primitive/rules.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9109 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/technology/property_.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2138 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/pdkmaster/technology/rule.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    25167 2023-07-26 12:04:52.000000 PDKMaster-0.9.4/pdkmaster/technology/technology_.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2246 2023-07-26 12:04:52.000000 PDKMaster-0.9.4/pdkmaster/technology/wafer_.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3344 2023-07-26 08:24:56.000000 PDKMaster-0.9.4/pdkmaster/typing.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       38 2023-07-26 12:05:03.104557 PDKMaster-0.9.4/setup.cfg
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1410 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/setup.py
--rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)      863 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/skill.py
--rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)     1278 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/skill2yaml.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.096557 PDKMaster-0.9.4/test/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/__init__.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.096557 PDKMaster-0.9.4/test/unit/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     7946 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/_util.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.096557 PDKMaster-0.9.4/test/unit/design/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/design/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3025 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/design/cell.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2470 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/design/circuit.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3664 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/design/factory.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    37661 2023-07-26 08:56:45.000000 PDKMaster-0.9.4/test/unit/design/layout.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4584 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/design/library.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.100557 PDKMaster-0.9.4/test/unit/dispatch/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/dispatch/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1343 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/dispatch/edge.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1397 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/dispatch/mask.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1752 2023-07-26 08:56:38.000000 PDKMaster-0.9.4/test/unit/dispatch/primitive.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1531 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/dispatch/rule.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3403 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/dispatch/shape.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13201 2023-07-26 08:56:45.000000 PDKMaster-0.9.4/test/unit/dummy.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.100557 PDKMaster-0.9.4/test/unit/io/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/io/__init__.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.100557 PDKMaster-0.9.4/test/unit/io/klayout/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/io/klayout/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13480 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/io/klayout/export.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    20839 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/io/klayout/merge.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.100557 PDKMaster-0.9.4/test/unit/io/lefdef/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-25 08:57:03.000000 PDKMaster-0.9.4/test/unit/io/lefdef/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1573 2023-07-25 08:57:03.000000 PDKMaster-0.9.4/test/unit/io/lefdef/export.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.100557 PDKMaster-0.9.4/test/unit/io/pdkmaster/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/io/pdkmaster/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1862 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/io/pdkmaster/export.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.100557 PDKMaster-0.9.4/test/unit/io/spice/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/io/spice/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     7947 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/io/spice/pyspice.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1317 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/io/spice/spice_.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.104557 PDKMaster-0.9.4/test/unit/technology/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/technology/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1313 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/technology/edge.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    56025 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/technology/geometry.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6370 2023-07-26 09:02:44.000000 PDKMaster-0.9.4/test/unit/technology/mask.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    53365 2023-07-26 09:02:44.000000 PDKMaster-0.9.4/test/unit/technology/primitive.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2775 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/technology/property.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2072 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test/unit/technology/rule.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    17585 2023-07-26 12:04:52.000000 PDKMaster-0.9.4/test/unit/technology/technology.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1052 2023-07-26 12:04:52.000000 PDKMaster-0.9.4/test/unit/technology/wafer.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1438 2023-07-26 09:02:44.000000 PDKMaster-0.9.4/test/unit/typing.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      673 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/test.tf
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 12:05:03.104557 PDKMaster-0.9.4/tf_yaml/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        0 2023-07-14 12:02:40.000000 PDKMaster-0.9.4/tf_yaml/.keepme
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.657629 PDKMaster-0.9.5/
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.625629 PDKMaster-0.9.5/.ci/
+-rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)     1069 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/.ci/check-dco.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      155 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/.gitignore
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2183 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/.gitlab-ci.yml
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6586 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/Contributing.md
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      566 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/LICENSE.md
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.625629 PDKMaster-0.9.5/LICENSES/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    34523 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/LICENSES/agpl-3.0.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    11358 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/LICENSES/apache-2.0.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13419 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/LICENSES/cern_ohl_s_v2.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18009 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/LICENSES/gpl-2.0.txt
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.629629 PDKMaster-0.9.5/PDKMaster.egg-info/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    10060 2023-08-08 13:57:39.000000 PDKMaster-0.9.5/PDKMaster.egg-info/PKG-INFO
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3966 2023-08-08 13:57:39.000000 PDKMaster-0.9.5/PDKMaster.egg-info/SOURCES.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        1 2023-08-08 13:57:39.000000 PDKMaster-0.9.5/PDKMaster.egg-info/dependency_links.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       61 2023-08-08 13:57:39.000000 PDKMaster-0.9.5/PDKMaster.egg-info/requires.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       15 2023-08-08 13:57:39.000000 PDKMaster-0.9.5/PDKMaster.egg-info/top_level.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    10060 2023-08-08 13:57:39.657629 PDKMaster-0.9.5/PKG-INFO
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9592 2023-08-08 13:50:43.000000 PDKMaster-0.9.5/README.md
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.629629 PDKMaster-0.9.5/ReleaseNotes/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      442 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/ReleaseNotes/v0.1.md
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1234 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/ReleaseNotes/v0.2.0.md
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1471 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/ReleaseNotes/v0.3.0.md
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2547 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/ReleaseNotes/v0.9.0.md
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.629629 PDKMaster-0.9.5/assura_yaml/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        0 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/assura_yaml/.keepme
+-rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)      595 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/checkskill.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       14 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/ci-requirements.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       61 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/dev-requirements.txt
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.629629 PDKMaster-0.9.5/display_yaml/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        0 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/display_yaml/.keepme
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.617629 PDKMaster-0.9.5/docs/
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.633629 PDKMaster-0.9.5/docs/src/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6063 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/docs/src/conf.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      456 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/docs/src/index.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      141 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/docs/src/pdkmaster._util.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      560 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/docs/src/pdkmaster.design.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      443 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/docs/src/pdkmaster.dispatch.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      312 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/docs/src/pdkmaster.io.coriolis.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      462 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/docs/src/pdkmaster.io.klayout.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      934 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/docs/src/pdkmaster.io.parsing.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      318 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/docs/src/pdkmaster.io.pdkmaster.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      262 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/docs/src/pdkmaster.io.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      449 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/docs/src/pdkmaster.io.spice.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      290 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/docs/src/pdkmaster.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1556 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/docs/src/pdkmaster.technology.rst
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3746 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/dodo.py
+-rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)     4469 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/extract_rules.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    26261 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/files.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.633629 PDKMaster-0.9.5/pdkmaster/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      709 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18133 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/_util.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.633629 PDKMaster-0.9.5/pdkmaster/design/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      237 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/design/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6045 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/design/cell.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    10199 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/design/circuit.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     8637 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/design/factory.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.637629 PDKMaster-0.9.5/pdkmaster/design/layout/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      664 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/design/layout/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    28707 2023-07-26 08:56:45.000000 PDKMaster-0.9.5/pdkmaster/design/layout/_circuitlayouter.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    48505 2023-08-08 13:50:43.000000 PDKMaster-0.9.5/pdkmaster/design/layout/_primitivelayouter.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3335 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/design/layout/factory_.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    22622 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/design/layout/layout_.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2887 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/design/library.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2600 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/design/routinggauge.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.637629 PDKMaster-0.9.5/pdkmaster/dispatch/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1375 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/dispatch/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1378 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/dispatch/edge.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1956 2023-07-24 14:24:09.000000 PDKMaster-0.9.5/pdkmaster/dispatch/mask.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     8101 2023-07-26 08:56:38.000000 PDKMaster-0.9.5/pdkmaster/dispatch/primitive.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2803 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/dispatch/rule.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3801 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/dispatch/shape.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.637629 PDKMaster-0.9.5/pdkmaster/io/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/io/__init__.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.637629 PDKMaster-0.9.5/pdkmaster/io/coriolis/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      120 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/io/coriolis/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    58632 2023-07-26 08:24:56.000000 PDKMaster-0.9.5/pdkmaster/io/coriolis/export.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.641629 PDKMaster-0.9.5/pdkmaster/io/klayout/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      142 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/io/klayout/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    37919 2023-07-26 08:57:55.000000 PDKMaster-0.9.5/pdkmaster/io/klayout/export.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    23519 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/io/klayout/merge_.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.641629 PDKMaster-0.9.5/pdkmaster/io/lefdef/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      261 2023-07-25 08:57:03.000000 PDKMaster-0.9.5/pdkmaster/io/lefdef/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9948 2023-07-26 08:24:48.000000 PDKMaster-0.9.5/pdkmaster/io/lefdef/export.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.641629 PDKMaster-0.9.5/pdkmaster/io/notebook/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      121 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/io/notebook/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1253 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/io/notebook/plotter.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.641629 PDKMaster-0.9.5/pdkmaster/io/parsing/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      214 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/io/parsing/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18847 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/io/parsing/assura.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      422 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/io/parsing/display.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      822 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/io/parsing/layermap.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    17548 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/io/parsing/skill_grammar.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    24374 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/io/parsing/tf.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.641629 PDKMaster-0.9.5/pdkmaster/io/pdkmaster/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      120 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/io/pdkmaster/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18067 2023-07-26 08:56:38.000000 PDKMaster-0.9.5/pdkmaster/io/pdkmaster/export.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.645629 PDKMaster-0.9.5/pdkmaster/io/spice/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      165 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/io/spice/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    15809 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/io/spice/pyspice.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     5904 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/io/spice/spice_.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      181 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/io/spice/typing.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.645629 PDKMaster-0.9.5/pdkmaster/technology/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      276 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/technology/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4032 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/technology/edge.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    77846 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/technology/geometry.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18203 2023-07-26 09:02:44.000000 PDKMaster-0.9.5/pdkmaster/technology/mask.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      627 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/technology/net.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.649629 PDKMaster-0.9.5/pdkmaster/technology/primitive/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      466 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/technology/primitive/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    10122 2023-07-26 08:56:45.000000 PDKMaster-0.9.5/pdkmaster/technology/primitive/_core.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2421 2023-07-26 08:56:45.000000 PDKMaster-0.9.5/pdkmaster/technology/primitive/_derived.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1176 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/technology/primitive/_param.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    24164 2023-07-26 08:57:55.000000 PDKMaster-0.9.5/pdkmaster/technology/primitive/conductors.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    44812 2023-08-08 13:50:33.000000 PDKMaster-0.9.5/pdkmaster/technology/primitive/devices.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4914 2023-07-26 12:04:52.000000 PDKMaster-0.9.5/pdkmaster/technology/primitive/layers.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6752 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/technology/primitive/rules.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     9109 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/technology/property_.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2138 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/pdkmaster/technology/rule.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    25167 2023-07-26 12:04:52.000000 PDKMaster-0.9.5/pdkmaster/technology/technology_.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2246 2023-07-26 12:04:52.000000 PDKMaster-0.9.5/pdkmaster/technology/wafer_.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3344 2023-07-26 08:24:56.000000 PDKMaster-0.9.5/pdkmaster/typing.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       38 2023-08-08 13:57:39.657629 PDKMaster-0.9.5/setup.cfg
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1410 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/setup.py
+-rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)      863 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/skill.py
+-rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)     1278 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/skill2yaml.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.649629 PDKMaster-0.9.5/test/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/__init__.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.649629 PDKMaster-0.9.5/test/unit/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     7946 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/_util.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.649629 PDKMaster-0.9.5/test/unit/design/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/design/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3025 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/design/cell.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2470 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/design/circuit.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3664 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/design/factory.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    37661 2023-07-26 08:56:45.000000 PDKMaster-0.9.5/test/unit/design/layout.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4584 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/design/library.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.653629 PDKMaster-0.9.5/test/unit/dispatch/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/dispatch/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1343 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/dispatch/edge.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1397 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/dispatch/mask.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1752 2023-07-26 08:56:38.000000 PDKMaster-0.9.5/test/unit/dispatch/primitive.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1531 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/dispatch/rule.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3403 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/dispatch/shape.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13201 2023-07-26 08:56:45.000000 PDKMaster-0.9.5/test/unit/dummy.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.653629 PDKMaster-0.9.5/test/unit/io/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/io/__init__.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.653629 PDKMaster-0.9.5/test/unit/io/klayout/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/io/klayout/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13480 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/io/klayout/export.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    20839 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/io/klayout/merge.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.653629 PDKMaster-0.9.5/test/unit/io/lefdef/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-25 08:57:03.000000 PDKMaster-0.9.5/test/unit/io/lefdef/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1573 2023-07-25 08:57:03.000000 PDKMaster-0.9.5/test/unit/io/lefdef/export.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.653629 PDKMaster-0.9.5/test/unit/io/pdkmaster/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/io/pdkmaster/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1862 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/io/pdkmaster/export.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.653629 PDKMaster-0.9.5/test/unit/io/spice/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/io/spice/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     7947 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/io/spice/pyspice.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1317 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/io/spice/spice_.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.657629 PDKMaster-0.9.5/test/unit/technology/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       98 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/technology/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1313 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/technology/edge.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    56025 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/technology/geometry.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     6370 2023-07-26 09:02:44.000000 PDKMaster-0.9.5/test/unit/technology/mask.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    53229 2023-08-08 13:50:33.000000 PDKMaster-0.9.5/test/unit/technology/primitive.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2775 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/technology/property.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2072 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test/unit/technology/rule.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    17588 2023-08-08 13:50:33.000000 PDKMaster-0.9.5/test/unit/technology/technology.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1052 2023-07-26 12:04:52.000000 PDKMaster-0.9.5/test/unit/technology/wafer.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1438 2023-07-26 09:02:44.000000 PDKMaster-0.9.5/test/unit/typing.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      673 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/test.tf
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-08-08 13:57:39.657629 PDKMaster-0.9.5/tf_yaml/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        0 2023-07-14 12:02:40.000000 PDKMaster-0.9.5/tf_yaml/.keepme
```

### Comparing `PDKMaster-0.9.4/.ci/check-dco.py` & `PDKMaster-0.9.5/.ci/check-dco.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/.gitlab-ci.yml` & `PDKMaster-0.9.5/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/Contributing.md` & `PDKMaster-0.9.5/Contributing.md`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/LICENSE.md` & `PDKMaster-0.9.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/LICENSES/agpl-3.0.txt` & `PDKMaster-0.9.5/LICENSES/agpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/LICENSES/apache-2.0.txt` & `PDKMaster-0.9.5/LICENSES/apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/LICENSES/cern_ohl_s_v2.txt` & `PDKMaster-0.9.5/LICENSES/cern_ohl_s_v2.txt`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/LICENSES/gpl-2.0.txt` & `PDKMaster-0.9.5/LICENSES/gpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/PDKMaster.egg-info/PKG-INFO` & `PDKMaster-0.9.5/PDKMaster.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PDKMaster
-Version: 0.9.4
+Version: 0.9.5
 Summary: ASIC PDK Manager and Design Framework
 Author: Staf Verhaegen
 Author-email: staf@fibraservi.eu
 License: AGPL-3.0-or-later OR GPL-2.0-or-later OR CERN-OHL-S-2.0+ OR Apache-2.0
 Project-URL: Source Code, https://gitlab.com/Chips4Makers/PDKMaster
 Project-URL: Bug Tracker, https://gitlab.com/Chips4Makers/PDKMaster/issues
 Requires-Python: >=3.6
@@ -14,14 +14,17 @@
 # Description
 
 PDK Master is a tool to manage [PDK](https://en.wikipedia.org/wiki/Process_design_kit)s for ASIC design and a framework for designing circuits and layouts in those technologies.
 It is a Python framework under heavy development and with an unstable API.
 
 # Release history
 
+* v0.9.5: allow use of MOSFET.gate4mosfet attribute before MOSFET is added to Technology.
+  This allows having rules added to the technology that are using the gate of a specific
+  MOSFET.
 * v0.9.4:
   * Support for WaferWire without an implant for diode, MOSFET etc.
   * Roadworks on layer manipulation
   * API improvements, unification and deprecation
 * v0.9.3:
   * First LEF/DEF support: support exporting tech.lef file
   * Bug fixing
```

### Comparing `PDKMaster-0.9.4/PDKMaster.egg-info/SOURCES.txt` & `PDKMaster-0.9.5/PDKMaster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/PKG-INFO` & `PDKMaster-0.9.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PDKMaster
-Version: 0.9.4
+Version: 0.9.5
 Summary: ASIC PDK Manager and Design Framework
 Author: Staf Verhaegen
 Author-email: staf@fibraservi.eu
 License: AGPL-3.0-or-later OR GPL-2.0-or-later OR CERN-OHL-S-2.0+ OR Apache-2.0
 Project-URL: Source Code, https://gitlab.com/Chips4Makers/PDKMaster
 Project-URL: Bug Tracker, https://gitlab.com/Chips4Makers/PDKMaster/issues
 Requires-Python: >=3.6
@@ -14,14 +14,17 @@
 # Description
 
 PDK Master is a tool to manage [PDK](https://en.wikipedia.org/wiki/Process_design_kit)s for ASIC design and a framework for designing circuits and layouts in those technologies.
 It is a Python framework under heavy development and with an unstable API.
 
 # Release history
 
+* v0.9.5: allow use of MOSFET.gate4mosfet attribute before MOSFET is added to Technology.
+  This allows having rules added to the technology that are using the gate of a specific
+  MOSFET.
 * v0.9.4:
   * Support for WaferWire without an implant for diode, MOSFET etc.
   * Roadworks on layer manipulation
   * API improvements, unification and deprecation
 * v0.9.3:
   * First LEF/DEF support: support exporting tech.lef file
   * Bug fixing
```

### Comparing `PDKMaster-0.9.4/README.md` & `PDKMaster-0.9.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # Description
 
 PDK Master is a tool to manage [PDK](https://en.wikipedia.org/wiki/Process_design_kit)s for ASIC design and a framework for designing circuits and layouts in those technologies.
 It is a Python framework under heavy development and with an unstable API.
 
 # Release history
 
+* v0.9.5: allow use of MOSFET.gate4mosfet attribute before MOSFET is added to Technology.
+  This allows having rules added to the technology that are using the gate of a specific
+  MOSFET.
 * v0.9.4:
   * Support for WaferWire without an implant for diode, MOSFET etc.
   * Roadworks on layer manipulation
   * API improvements, unification and deprecation
 * v0.9.3:
   * First LEF/DEF support: support exporting tech.lef file
   * Bug fixing
```

### Comparing `PDKMaster-0.9.4/ReleaseNotes/v0.2.0.md` & `PDKMaster-0.9.5/ReleaseNotes/v0.2.0.md`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/ReleaseNotes/v0.3.0.md` & `PDKMaster-0.9.5/ReleaseNotes/v0.3.0.md`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/ReleaseNotes/v0.9.0.md` & `PDKMaster-0.9.5/ReleaseNotes/v0.9.0.md`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/checkskill.py` & `PDKMaster-0.9.5/checkskill.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/docs/src/conf.py` & `PDKMaster-0.9.5/docs/src/conf.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/docs/src/pdkmaster.design.rst` & `PDKMaster-0.9.5/docs/src/pdkmaster.design.rst`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/docs/src/pdkmaster.io.parsing.rst` & `PDKMaster-0.9.5/docs/src/pdkmaster.io.parsing.rst`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/docs/src/pdkmaster.technology.rst` & `PDKMaster-0.9.5/docs/src/pdkmaster.technology.rst`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/dodo.py` & `PDKMaster-0.9.5/dodo.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/extract_rules.py` & `PDKMaster-0.9.5/extract_rules.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/files.py` & `PDKMaster-0.9.5/files.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/__init__.py` & `PDKMaster-0.9.5/pdkmaster/__init__.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/_util.py` & `PDKMaster-0.9.5/pdkmaster/_util.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/design/cell.py` & `PDKMaster-0.9.5/pdkmaster/design/cell.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/design/circuit.py` & `PDKMaster-0.9.5/pdkmaster/design/circuit.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/design/factory.py` & `PDKMaster-0.9.5/pdkmaster/design/factory.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/design/layout/__init__.py` & `PDKMaster-0.9.5/pdkmaster/design/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/design/layout/_circuitlayouter.py` & `PDKMaster-0.9.5/pdkmaster/design/layout/_circuitlayouter.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/design/layout/_primitivelayouter.py` & `PDKMaster-0.9.5/pdkmaster/design/layout/_primitivelayouter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1003,25 +1003,29 @@
         else:
             top = portnets["top"]
             bottom = portnets["bottom"]
 
         via = prim.via
 
         # Params
-        top_width = mimcapargs["width"]
-        top_height = mimcapargs["height"]
+        top_width: float = mimcapargs["width"]
+        top_height: float = mimcapargs["height"]
         connect_up = mimcapargs["bottom_connect_up"]
 
         # TODO: Allow to specify top of the via layer
         upper_metal = via.top[0]
         assert isinstance(upper_metal, _prm.MetalWire)
         assert upper_metal.pin is not None
         upper_pin: _prm.Marker = upper_metal.pin
 
         # Compute dimensions
+        bottomvia_outerbound: Optional[_geo.ShapeT] = None
+        bottomupper_outerwidth: Optional[float] = None
+        bottomupper_outerheight: Optional[float] = None
+        bottomupper_ringwidth: Optional[float] = None
         if connect_up:
             bottomvia_outerwidth = (
                 top_width + 2*prim.min_bottomvia_top_space + 2*via.width
             )
             bottomvia_outerheight = (
                 top_height + 2*prim.min_bottomvia_top_space + 2*via.width
             )
@@ -1064,14 +1068,19 @@
         via_upmbb = via_lay.bounds(mask=upper_metal.mask)
         layout.add_shape(layer=upper_pin, net=top, shape=via_upmbb)
 
         shape = _geo.Rect.from_size(width=bottom_width, height=bottom_height)
         layout.add_shape(layer=prim.bottom, net=bottom, shape=shape)
 
         if connect_up:
+            assert bottomvia_outerbound is not None
+            assert bottomupper_outerwidth is not None
+            assert bottomupper_outerheight is not None
+            assert bottomupper_ringwidth is not None
+
             shape = _geo.RectRing(
                 outer_bound=bottomvia_outerbound,
                 rect_width=via.width, min_rect_space=via.min_space,
             )
             layout.add_shape(layer=via, net=bottom, shape=shape)
 
             shape = _geo.Ring(
```

### Comparing `PDKMaster-0.9.4/pdkmaster/design/layout/factory_.py` & `PDKMaster-0.9.5/pdkmaster/design/layout/factory_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/design/layout/layout_.py` & `PDKMaster-0.9.5/pdkmaster/design/layout/layout_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/design/library.py` & `PDKMaster-0.9.5/pdkmaster/design/library.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/design/routinggauge.py` & `PDKMaster-0.9.5/pdkmaster/design/routinggauge.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/dispatch/__init__.py` & `PDKMaster-0.9.5/pdkmaster/dispatch/__init__.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/dispatch/edge.py` & `PDKMaster-0.9.5/pdkmaster/dispatch/edge.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/dispatch/mask.py` & `PDKMaster-0.9.5/pdkmaster/dispatch/mask.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/dispatch/primitive.py` & `PDKMaster-0.9.5/pdkmaster/dispatch/primitive.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/dispatch/rule.py` & `PDKMaster-0.9.5/pdkmaster/dispatch/rule.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/dispatch/shape.py` & `PDKMaster-0.9.5/pdkmaster/dispatch/shape.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/io/coriolis/export.py` & `PDKMaster-0.9.5/pdkmaster/io/coriolis/export.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/io/klayout/export.py` & `PDKMaster-0.9.5/pdkmaster/io/klayout/export.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/io/klayout/merge_.py` & `PDKMaster-0.9.5/pdkmaster/io/klayout/merge_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/io/lefdef/export.py` & `PDKMaster-0.9.5/pdkmaster/io/lefdef/export.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/io/notebook/plotter.py` & `PDKMaster-0.9.5/pdkmaster/io/notebook/plotter.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/io/parsing/assura.py` & `PDKMaster-0.9.5/pdkmaster/io/parsing/assura.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/io/parsing/layermap.py` & `PDKMaster-0.9.5/pdkmaster/io/parsing/layermap.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/io/parsing/skill_grammar.py` & `PDKMaster-0.9.5/pdkmaster/io/parsing/skill_grammar.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/io/parsing/tf.py` & `PDKMaster-0.9.5/pdkmaster/io/parsing/tf.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/io/pdkmaster/export.py` & `PDKMaster-0.9.5/pdkmaster/io/pdkmaster/export.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/io/spice/pyspice.py` & `PDKMaster-0.9.5/pdkmaster/io/spice/pyspice.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/io/spice/spice_.py` & `PDKMaster-0.9.5/pdkmaster/io/spice/spice_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/technology/edge.py` & `PDKMaster-0.9.5/pdkmaster/technology/edge.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/technology/geometry.py` & `PDKMaster-0.9.5/pdkmaster/technology/geometry.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/technology/mask.py` & `PDKMaster-0.9.5/pdkmaster/technology/mask.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/technology/net.py` & `PDKMaster-0.9.5/pdkmaster/technology/net.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/technology/primitive/_core.py` & `PDKMaster-0.9.5/pdkmaster/technology/primitive/_core.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/technology/primitive/_derived.py` & `PDKMaster-0.9.5/pdkmaster/technology/primitive/_derived.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/technology/primitive/_param.py` & `PDKMaster-0.9.5/pdkmaster/technology/primitive/_param.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/technology/primitive/conductors.py` & `PDKMaster-0.9.5/pdkmaster/technology/primitive/conductors.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/technology/primitive/devices.py` & `PDKMaster-0.9.5/pdkmaster/technology/primitive/devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -925,14 +925,23 @@
         elif contact is not None:
             raise ValueError(
                 "contact layer provided without min_contactgate_space specification",
             )
         self.min_contactgate_space = min_contactgate_space
         self.contact = contact
 
+        # Derive _gate4mosfet
+        gate_prims = (gate, *implant)
+        if well is not None:
+            gate_prims += (well,)
+        gate4mosfet = gate_prims[0] if len(gate_prims) == 1 else _Intersect(prims=gate_prims)
+        if (well is None) and gate.active.well:
+            gate4mosfet = gate4mosfet.remove(gate.active.well)
+        self._gate4mosfet = gate4mosfet.alias(f"gate:mosfet:{name}")
+
         # MOSFET is symmetric so both diffusion regions can be source or drain
         bulknet = (
             _PrimitiveNet(prim=self, name="bulk") if well is not None
             else _wfr.SubstrateNet(name="bulk")
         )
         self.ports += (
             _PrimitiveNet(prim=self, name="sourcedrain1"),
@@ -951,19 +960,14 @@
         return any(impl.type_ != adjImpl for impl in self.implant)
     @property
     def gate4mosfet(self) -> MaskPrimitiveT:
         """gate_prim attribute is the primitive representing the gate of the MOSFET
         object. Main reason it exists is to use it in rules; for example a minimum spacing
         to the gate of a transistor.
         """
-        if not hasattr(self, "_gate4mosfet"):
-            raise TypeError(
-                "gate4mosfet attribute may not be accessed before the MOSFET is added"
-                " to a technology"
-            )
         return self._gate4mosfet
     # Backwards compatibility
     gate_prim = gate4mosfet
     @property
     def gate_mask(self) -> _msk.MaskT:
         """
         API Notes:
@@ -972,23 +976,15 @@
         return self.gate4mosfet.mask
 
     def _generate_rules(self, *,
         tech: _tch.Technology,
     ) -> Iterable[_rle.RuleT]:
         yield from super()._generate_rules(tech=tech)
 
-        markers = (
-            self.well if self.well is not None else tech.substrate_prim,
-            *self.implant,
-        )
-        derivedgate = cast(
-            _Alias,
-            _Intersect(prims=(self.gate, *markers)).alias(f"gate:mosfet:{self.name}"),
-        )
-        self._gate4mosfet = derivedgate
+        derivedgate = cast(_Alias, self.gate4mosfet)
         derivedgate_edge = _edg.MaskEdge(derivedgate.mask)
         poly_mask = self.gate.poly.mask
         poly_edge = _edg.MaskEdge(poly_mask)
         channel_edge = _edg.Intersect((derivedgate_edge, poly_edge))
         active_mask = self.gate.active.mask
         active_edge = _edg.MaskEdge(active_mask)
         fieldgate_edge = _edg.Intersect((derivedgate_edge, active_edge))
```

### Comparing `PDKMaster-0.9.4/pdkmaster/technology/primitive/layers.py` & `PDKMaster-0.9.5/pdkmaster/technology/primitive/layers.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/technology/primitive/rules.py` & `PDKMaster-0.9.5/pdkmaster/technology/primitive/rules.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/technology/property_.py` & `PDKMaster-0.9.5/pdkmaster/technology/property_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/technology/rule.py` & `PDKMaster-0.9.5/pdkmaster/technology/rule.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/technology/technology_.py` & `PDKMaster-0.9.5/pdkmaster/technology/technology_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/technology/wafer_.py` & `PDKMaster-0.9.5/pdkmaster/technology/wafer_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/pdkmaster/typing.py` & `PDKMaster-0.9.5/pdkmaster/typing.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/setup.py` & `PDKMaster-0.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/skill.py` & `PDKMaster-0.9.5/skill.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/skill2yaml.py` & `PDKMaster-0.9.5/skill2yaml.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/test/unit/_util.py` & `PDKMaster-0.9.5/test/unit/_util.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/test/unit/design/cell.py` & `PDKMaster-0.9.5/test/unit/design/cell.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/test/unit/design/circuit.py` & `PDKMaster-0.9.5/test/unit/design/circuit.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/test/unit/design/factory.py` & `PDKMaster-0.9.5/test/unit/design/factory.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/test/unit/design/layout.py` & `PDKMaster-0.9.5/test/unit/design/layout.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/test/unit/design/library.py` & `PDKMaster-0.9.5/test/unit/design/library.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/test/unit/dispatch/edge.py` & `PDKMaster-0.9.5/test/unit/dispatch/edge.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/test/unit/dispatch/mask.py` & `PDKMaster-0.9.5/test/unit/dispatch/mask.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/test/unit/dispatch/primitive.py` & `PDKMaster-0.9.5/test/unit/dispatch/primitive.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/test/unit/dispatch/rule.py` & `PDKMaster-0.9.5/test/unit/dispatch/rule.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/test/unit/dispatch/shape.py` & `PDKMaster-0.9.5/test/unit/dispatch/shape.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/test/unit/dummy.py` & `PDKMaster-0.9.5/test/unit/dummy.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/test/unit/io/klayout/export.py` & `PDKMaster-0.9.5/test/unit/io/klayout/export.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/test/unit/io/klayout/merge.py` & `PDKMaster-0.9.5/test/unit/io/klayout/merge.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/test/unit/io/lefdef/export.py` & `PDKMaster-0.9.5/test/unit/io/lefdef/export.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/test/unit/io/pdkmaster/export.py` & `PDKMaster-0.9.5/test/unit/io/pdkmaster/export.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/test/unit/io/spice/pyspice.py` & `PDKMaster-0.9.5/test/unit/io/spice/pyspice.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/test/unit/io/spice/spice_.py` & `PDKMaster-0.9.5/test/unit/io/spice/spice_.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/test/unit/technology/edge.py` & `PDKMaster-0.9.5/test/unit/technology/edge.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/test/unit/technology/geometry.py` & `PDKMaster-0.9.5/test/unit/technology/geometry.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/test/unit/technology/mask.py` & `PDKMaster-0.9.5/test/unit/technology/mask.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/test/unit/technology/primitive.py` & `PDKMaster-0.9.5/test/unit/technology/primitive.py`

 * *Files 0% similar despite different names*

```diff
@@ -1161,18 +1161,14 @@
         self.assertNotEqual(prim1, prim2)
         self.assertNotEqual(prim1, prim3)
 
         self.assertTrue(prim1.has_typeimplant)
         self.assertTrue(prim2.has_typeimplant)
         self.assertFalse(prim3.has_typeimplant)
 
-        # Access gate4mosfet before being added to technology
-        with self.assertRaises(TypeError):
-            prim1.gate4mosfet
-
         self.assertAlmostEqual(prim1.computed.min_l, 1.5, places=6)
         self.assertAlmostEqual(prim1.computed.min_sd_width, 0.15, places=6)
         self.assertAlmostEqual(prim1.computed.min_contactgate_space, 0.1, places=6)
         self.assertAlmostEqual(prim3.computed.min_contactgate_space, 0.15, places=6)
         self.assertEqual(prim1.computed.contact, ch)
         self.assertAlmostEqual(prim2.computed.min_l, 1.0, places=6)
         self.assertAlmostEqual(prim2.computed.min_sd_width, 0.15, places=6)
```

### Comparing `PDKMaster-0.9.4/test/unit/technology/property.py` & `PDKMaster-0.9.5/test/unit/technology/property.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/test/unit/technology/rule.py` & `PDKMaster-0.9.5/test/unit/technology/rule.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/test/unit/technology/technology.py` & `PDKMaster-0.9.5/test/unit/technology/technology.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,15 +239,15 @@
         self.assertEqual(
             dummy_tech.substrate,
             dummy_tech.substrate_prim.mask,
         )
 
     def test_mosfet(self):
         nmos = dummy_prims.nmos
-        prim = _prm._derived._Intersect(prims=(nmos.gate, dummy_tech.substrate_prim, *nmos.implant))
+        prim = _prm._derived._Intersect(prims=(nmos.gate, *nmos.implant)).remove(nmos.gate.active.well)
         alias = prim.alias("gate:mosfet:nmos")
         self.assertEqual(nmos.gate4mosfet._prim, prim)
         self.assertEqual(nmos.gate4mosfet, alias)
         self.assertEqual(nmos.gate_mask, nmos.gate4mosfet.mask)
 
     def test_check(self):
         class MyTech(_tch.Technology):
```

### Comparing `PDKMaster-0.9.4/test/unit/technology/wafer.py` & `PDKMaster-0.9.5/test/unit/technology/wafer.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/test/unit/typing.py` & `PDKMaster-0.9.5/test/unit/typing.py`

 * *Files identical despite different names*

### Comparing `PDKMaster-0.9.4/test.tf` & `PDKMaster-0.9.5/test.tf`

 * *Files identical despite different names*

