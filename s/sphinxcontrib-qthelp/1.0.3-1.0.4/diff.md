# Comparing `tmp/sphinxcontrib-qthelp-1.0.3.tar.gz` & `tmp/sphinxcontrib_qthelp-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sphinxcontrib-qthelp-1.0.3.tar", last modified: Sat Feb 29 04:19:04 2020, max compression
+gzip compressed data, was "sphinxcontrib_qthelp-1.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinxcontrib-qthelp-1.0.3.tar` & `sphinxcontrib_qthelp-1.0.4.tar`

### file list

```diff
@@ -1,236 +1,118 @@
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.475090 sphinxcontrib-qthelp-1.0.3/
--rw-r--r--   0 tkomiya    (502) staff       (20)      417 2020-02-29 04:18:51.000000 sphinxcontrib-qthelp-1.0.3/CHANGES
--rw-r--r--   0 tkomiya    (502) staff       (20)     1435 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/LICENSE
--rw-r--r--   0 tkomiya    (502) staff       (20)      195 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/MANIFEST.in
--rw-r--r--   0 tkomiya    (502) staff       (20)     1276 2020-02-29 04:19:04.475273 sphinxcontrib-qthelp-1.0.3/PKG-INFO
--rw-r--r--   0 tkomiya    (502) staff       (20)      843 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/README.rst
--rw-r--r--   0 tkomiya    (502) staff       (20)      470 2020-02-29 04:19:04.475911 sphinxcontrib-qthelp-1.0.3/setup.cfg
--rw-r--r--   0 tkomiya    (502) staff       (20)     2057 2020-02-29 04:01:18.000000 sphinxcontrib-qthelp-1.0.3/setup.py
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.424476 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/
--rw-r--r--   0 tkomiya    (502) staff       (20)      350 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/__init__.py
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.424959 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/
--rw-r--r--   0 tkomiya    (502) staff       (20)    10712 2020-01-12 15:58:51.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/__init__.py
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.425204 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.425843 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/.tx/
--rw-r--r--   0 tkomiya    (502) staff       (20)      218 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/.tx/config
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.411422 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ar/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.426812 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ar/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1194 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ar/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1273 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ar/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.411635 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/bn/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.427759 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/bn/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1112 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/bn/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1191 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/bn/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.411841 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ca/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.428681 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ca/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1112 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ca/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1191 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ca/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.412041 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/cs/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.429527 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/cs/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1190 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/cs/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1269 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/cs/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.412240 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/cy/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.430400 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/cy/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1155 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/cy/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1234 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/cy/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.412438 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/da/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.431239 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/da/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1111 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/da/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1190 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/da/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.412641 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/de/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.432075 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/de/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1111 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/de/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1190 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/de/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.412854 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/el/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.432953 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/el/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1110 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/el/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1189 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/el/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.413067 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/eo/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.433831 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/eo/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1114 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/eo/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1193 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/eo/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.413274 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/es/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.434864 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/es/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1128 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/es/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1328 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/es/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.413481 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/et/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.435773 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/et/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1134 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/et/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1371 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/et/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.413688 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/eu/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.436557 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/eu/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1111 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/eu/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1190 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/eu/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.413893 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/fa/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.437460 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/fa/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1111 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/fa/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1190 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/fa/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.414105 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/fi/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.438224 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/fi/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1112 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/fi/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1191 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/fi/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.414313 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/fr/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.439123 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/fr/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1140 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/fr/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1350 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/fr/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.414523 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/he/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.440045 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/he/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1205 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/he/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1284 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/he/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.414725 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/hi/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.440952 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/hi/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1110 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/hi/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1189 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/hi/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.414931 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/hi_IN/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.441833 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/hi_IN/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1124 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/hi_IN/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1203 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/hi_IN/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.415140 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/hr/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.442847 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/hr/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1185 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/hr/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1264 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/hr/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.415357 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/hu/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.443735 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/hu/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1114 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/hu/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1193 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/hu/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.415579 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/id/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.444653 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/id/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1117 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/id/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1579 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/id/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.415795 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/it/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.445550 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/it/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1112 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/it/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1191 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/it/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.416013 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ja/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.446483 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ja/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1106 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ja/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1185 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ja/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.416232 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ko/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.447347 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ko/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1115 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ko/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1311 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ko/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.416441 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/lt/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.448226 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/lt/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1246 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/lt/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1325 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/lt/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.416651 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/lv/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.449202 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/lv/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1147 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/lv/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1226 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/lv/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.416865 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/mk/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.450174 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/mk/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1145 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/mk/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1224 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/mk/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.417079 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/nb_NO/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.451069 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/nb_NO/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1137 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/nb_NO/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1216 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/nb_NO/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.417296 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ne/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.451941 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ne/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1111 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ne/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1190 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ne/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.417509 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/nl/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.452803 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/nl/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1110 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/nl/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1189 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/nl/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.417719 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/pl/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.453651 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/pl/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1249 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/pl/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1430 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/pl/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.417949 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/pt/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.454553 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/pt/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1115 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/pt/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1194 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/pt/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.418161 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/pt_BR/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.455359 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/pt_BR/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1129 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/pt_BR/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1208 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/pt_BR/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.418377 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/pt_PT/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.456158 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/pt_PT/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1132 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/pt_PT/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1211 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/pt_PT/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.418595 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ro/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.457125 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ro/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1154 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ro/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1233 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ro/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.418804 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ru/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.457921 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ru/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1250 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ru/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1329 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ru/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.419008 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/si/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.458686 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/si/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1112 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/si/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1191 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/si/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.419219 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/sk/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.459506 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/sk/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1186 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/sk/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1265 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/sk/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.419433 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/sl/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.460380 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/sl/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1166 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/sl/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1245 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/sl/LC_MESSAGES/sphinxcontrib.qthelp.po
--rw-r--r--   0 tkomiya    (502) staff       (20)     1135 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/sphinxcontrib.qthelp.pot
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.419641 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/sr/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.461198 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/sr/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1186 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/sr/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1265 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/sr/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.419854 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/sr@latin/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.462101 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/sr@latin/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1208 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/sr@latin/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1287 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/sr@latin/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.420064 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/sv/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.463178 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/sv/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1112 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/sv/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1191 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/sv/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.420277 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ta/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.464042 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ta/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1110 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ta/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1189 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ta/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.420484 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/tr/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.464903 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/tr/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1111 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/tr/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1190 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/tr/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.420699 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/uk_UA/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.465758 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/uk_UA/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1352 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/uk_UA/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1431 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/uk_UA/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.420906 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/vi/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.466539 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/vi/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1108 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/vi/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1187 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/vi/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.421112 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/zh_CN/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.467417 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/zh_CN/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1158 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/zh_CN/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1637 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/zh_CN/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.421324 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/zh_TW/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.468271 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/zh_TW/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1120 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/zh_TW/LC_MESSAGES/sphinxcontrib.qthelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1199 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/zh_TW/LC_MESSAGES/sphinxcontrib.qthelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.469029 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/templates/
--rw-r--r--   0 tkomiya    (502) staff       (20)      567 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/templates/project.qhcp
--rw-r--r--   0 tkomiya    (502) staff       (20)      863 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/templates/project.qhp
--rw-r--r--   0 tkomiya    (502) staff       (20)      269 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/version.py
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.470867 sphinxcontrib-qthelp-1.0.3/sphinxcontrib_qthelp.egg-info/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1276 2020-02-29 04:19:04.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib_qthelp.egg-info/PKG-INFO
--rw-r--r--   0 tkomiya    (502) staff       (20)     7606 2020-02-29 04:19:04.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib_qthelp.egg-info/SOURCES.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)        1 2020-02-29 04:19:04.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib_qthelp.egg-info/dependency_links.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)       14 2020-02-29 04:19:04.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib_qthelp.egg-info/namespace_packages.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)        1 2020-02-29 04:19:04.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib_qthelp.egg-info/not-zip-safe
--rw-r--r--   0 tkomiya    (502) staff       (20)       50 2020-02-29 04:19:04.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib_qthelp.egg-info/requires.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)       14 2020-02-29 04:19:04.000000 sphinxcontrib-qthelp-1.0.3/sphinxcontrib_qthelp.egg-info/top_level.txt
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.471369 sphinxcontrib-qthelp-1.0.3/tests/
--rw-r--r--   0 tkomiya    (502) staff       (20)      402 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/tests/conftest.py
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.422028 sphinxcontrib-qthelp-1.0.3/tests/roots/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.471810 sphinxcontrib-qthelp-1.0.3/tests/roots/test-basic/
--rw-r--r--   0 tkomiya    (502) staff       (20)        0 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/tests/roots/test-basic/conf.py
--rw-r--r--   0 tkomiya    (502) staff       (20)       22 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/tests/roots/test-basic/index.rst
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:19:04.474609 sphinxcontrib-qthelp-1.0.3/tests/roots/test-need-escaped/
--rw-r--r--   0 tkomiya    (502) staff       (20)        8 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/tests/roots/test-need-escaped/bar.rst
--rw-r--r--   0 tkomiya    (502) staff       (20)        8 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/tests/roots/test-need-escaped/baz.rst
--rw-r--r--   0 tkomiya    (502) staff       (20)       62 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/tests/roots/test-need-escaped/conf.py
--rw-r--r--   0 tkomiya    (502) staff       (20)       82 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/tests/roots/test-need-escaped/foo.rst
--rw-r--r--   0 tkomiya    (502) staff       (20)      749 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/tests/roots/test-need-escaped/index.rst
--rw-r--r--   0 tkomiya    (502) staff       (20)       10 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/tests/roots/test-need-escaped/quux.rst
--rw-r--r--   0 tkomiya    (502) staff       (20)       29 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/tests/roots/test-need-escaped/qux.rst
--rw-r--r--   0 tkomiya    (502) staff       (20)     5635 2020-01-12 15:33:12.000000 sphinxcontrib-qthelp-1.0.3/tests/test_qthelp.py
--rw-r--r--   0 tkomiya    (502) staff       (20)      474 2020-01-12 15:58:51.000000 sphinxcontrib-qthelp-1.0.3/tox.ini
+-rw-r--r--   0        0        0      569 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/CHANGES
+-rw-r--r--   0        0        0     1435 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/LICENSE
+-rw-r--r--   0        0        0      409 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/README.rst
+-rw-r--r--   0        0        0     1975 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0    10672 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/__init__.py
+-rw-r--r--   0        0        0      218 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/.tx/config
+-rw-r--r--   0        0        0     1194 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/ar/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1273 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/ar/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1112 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/bn/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1191 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/bn/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1112 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/ca/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1191 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/ca/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1190 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/cs/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1269 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/cs/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1155 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/cy/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1234 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/cy/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1111 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/da/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1190 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/da/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1111 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/de/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1190 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/de/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1110 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/el/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1189 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/el/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1114 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/eo/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1193 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/eo/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1128 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/es/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1328 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/es/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1134 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/et/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1371 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/et/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1111 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/eu/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1190 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/eu/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1111 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/fa/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1190 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/fa/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1112 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/fi/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1191 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/fi/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1140 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/fr/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1350 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/fr/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1205 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/he/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1284 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/he/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1110 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/hi/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1189 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/hi/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1124 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/hi_IN/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1203 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/hi_IN/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1185 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/hr/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1264 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/hr/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1114 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/hu/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1193 2023-08-08 18:58:53.729801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/hu/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1117 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/id/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1579 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/id/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1112 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/it/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1191 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/it/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1106 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/ja/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1185 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/ja/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1115 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/ko/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1311 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/ko/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1246 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/lt/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1325 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/lt/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1147 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/lv/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1226 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/lv/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1145 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/mk/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1224 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/mk/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1137 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/nb_NO/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1216 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/nb_NO/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1111 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/ne/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1190 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/ne/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1110 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/nl/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1189 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/nl/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1249 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/pl/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1430 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/pl/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1115 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/pt/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1194 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/pt/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1129 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/pt_BR/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1208 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/pt_BR/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1132 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/pt_PT/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1211 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/pt_PT/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1154 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/ro/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1233 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/ro/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1250 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/ru/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1329 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/ru/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1112 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/si/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1191 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/si/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1186 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/sk/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1265 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/sk/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1166 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/sl/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1245 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/sl/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1135 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/sphinxcontrib.qthelp.pot
+-rw-r--r--   0        0        0     1186 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/sr/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1265 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/sr/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1208 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/sr@latin/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1287 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/sr@latin/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1112 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/sv/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1191 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/sv/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1110 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/ta/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1189 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/ta/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1111 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/tr/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1190 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/tr/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1352 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/uk_UA/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1431 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/uk_UA/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1108 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/vi/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1187 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/vi/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1158 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/zh_CN/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1637 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/zh_CN/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0     1120 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/zh_TW/LC_MESSAGES/sphinxcontrib.qthelp.mo
+-rw-r--r--   0        0        0     1199 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/zh_TW/LC_MESSAGES/sphinxcontrib.qthelp.po
+-rw-r--r--   0        0        0      567 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/templates/project.qhcp
+-rw-r--r--   0        0        0      863 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/templates/project.qhp
+-rw-r--r--   0        0        0      187 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/tests/roots/test-basic/conf.py
+-rw-r--r--   0        0        0       22 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/tests/roots/test-basic/index.rst
+-rw-r--r--   0        0        0        8 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/tests/roots/test-need-escaped/bar.rst
+-rw-r--r--   0        0        0        8 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/tests/roots/test-need-escaped/baz.rst
+-rw-r--r--   0        0        0       62 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/tests/roots/test-need-escaped/conf.py
+-rw-r--r--   0        0        0       82 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/tests/roots/test-need-escaped/foo.rst
+-rw-r--r--   0        0        0      749 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/tests/roots/test-need-escaped/index.rst
+-rw-r--r--   0        0        0       10 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/tests/roots/test-need-escaped/quux.rst
+-rw-r--r--   0        0        0       29 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/tests/roots/test-need-escaped/qux.rst
+-rw-r--r--   0        0        0     5532 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/tests/test_qthelp.py
+-rw-r--r--   0        0        0      554 2023-08-08 18:58:53.733801 sphinxcontrib_qthelp-1.0.4/tox.ini
+-rw-r--r--   0        0        0     2179 1970-01-01 00:00:00.000000 sphinxcontrib_qthelp-1.0.4/PKG-INFO
```

### Comparing `sphinxcontrib-qthelp-1.0.3/LICENSE` & `sphinxcontrib_qthelp-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/__init__.py` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,35 @@
-"""
-    sphinxcontrib.qthelp
-    ~~~~~~~~~~~~~~~~~~~~
-
-    Build input files for the Qt collection generator.
-
-    :copyright: Copyright 2007-2019 by the Sphinx team, see README.
-    :license: BSD, see LICENSE for details.
-"""
+"""Build input files for the Qt collection generator."""
+
+from __future__ import annotations
 
 import html
 import os
 import posixpath
 import re
+from collections.abc import Iterable
 from os import path
-from typing import Any, Dict, Iterable, List, Tuple, cast
+from pathlib import Path
+from typing import Any, cast
 
 from docutils import nodes
 from docutils.nodes import Node
 from sphinx import addnodes
 from sphinx.application import Sphinx
 from sphinx.builders.html import StandaloneHTMLBuilder
 from sphinx.environment.adapters.indexentries import IndexEntries
 from sphinx.locale import get_translation
 from sphinx.util import logging
 from sphinx.util.nodes import NodeMatcher
 from sphinx.util.osutil import canon_path, make_filename
 from sphinx.util.template import SphinxRenderer
 
-from sphinxcontrib.qthelp.version import __version__
 
+__version__ = '1.0.4'
+__version_info__ = (1, 0, 4)
 
 logger = logging.getLogger(__name__)
 package_dir = path.abspath(path.dirname(__file__))
 
 __ = get_translation(__name__, 'console')
 
 
@@ -78,35 +75,39 @@
     def init(self) -> None:
         super().init()
         # the output files for HTML help must be .html only
         self.out_suffix = '.html'
         self.link_suffix = '.html'
         # self.config.html_style = 'traditional.css'
 
-    def get_theme_config(self) -> Tuple[str, Dict]:
+    def get_theme_config(self) -> tuple[str, dict]:
         return self.config.qthelp_theme, self.config.qthelp_theme_options
 
     def handle_finish(self) -> None:
+        self.epilog = self.epilog % {
+            'outdir': '%(outdir)s',
+            'project': self.config.qthelp_basename,
+        }
         self.build_qhp(self.outdir, self.config.qthelp_basename)
 
-    def build_qhp(self, outdir: str, outname: str) -> None:
+    def build_qhp(self, outdir: Path, outname: str) -> None:
         logger.info(__('writing project file...'))
 
         # sections
         tocdoc = self.env.get_and_resolve_doctree(self.config.master_doc, self,
                                                   prune_toctrees=False)
 
         sections = []
         matcher = NodeMatcher(addnodes.compact_paragraph, toctree=True)
         for node in tocdoc.traverse(matcher):  # type: addnodes.compact_paragraph
             sections.extend(self.write_toc(node))
 
         for indexname, indexcls, content, collapse in self.domain_indices:
             item = section_template % {'title': indexcls.localname,
-                                       'ref': '%s.html' % indexname}
+                                       'ref': indexname + self.out_suffix}
             sections.append(' ' * 4 * 4 + item)
         sections = '\n'.join(sections)  # type: ignore
 
         # keywords
         keywords = []
         index = IndexEntries(self.env).create_index(self, group_entries=False)
         for (key, group) in index:
@@ -134,15 +135,15 @@
                                master_doc=self.config.master_doc,
                                sections=sections, keywords=keywords,
                                files=self.get_project_files(outdir))
             f.write(body)
 
         homepage = 'qthelp://' + posixpath.join(
             nspace, 'doc', self.get_target_uri(self.config.master_doc))
-        startpage = 'qthelp://' + posixpath.join(nspace, 'doc', 'index.html')
+        startpage = 'qthelp://' + posixpath.join(nspace, 'doc', 'index%s' % self.link_suffix)
 
         logger.info(__('writing collection project file...'))
         with open(path.join(outdir, outname + '.qhcp'), 'w', encoding='utf-8') as f:
             body = render_file('project.qhcp', outname=outname,
                                title=self.config.html_short_title,
                                homepage=homepage, startpage=startpage)
             f.write(body)
@@ -156,16 +157,16 @@
             return False
         if not isinstance(node[0][0], nodes.reference):
             return False
         if not isinstance(node[1], nodes.bullet_list):
             return False
         return True
 
-    def write_toc(self, node: Node, indentlevel: int = 4) -> List[str]:
-        parts = []  # type: List[str]
+    def write_toc(self, node: Node, indentlevel: int = 4) -> list[str]:
+        parts: list[str] = []
         if isinstance(node, nodes.list_item) and self.isdocnode(node):
             compact_paragraph = cast(addnodes.compact_paragraph, node[0])
             reference = cast(nodes.reference, compact_paragraph[0])
             link = reference['refuri']
             title = html.escape(reference.astext()).replace('"', '&quot;')
             item = '<section title="%(title)s" ref="%(ref)s">' % \
                 {'title': title, 'ref': link}
@@ -212,16 +213,16 @@
         if id:
             item = ' ' * 12 + '<keyword name="%s" id="%s" ref="%s"/>' % (nameattr, id, refattr)
         else:
             item = ' ' * 12 + '<keyword name="%s" ref="%s"/>' % (nameattr, refattr)
         item.encode('ascii', 'xmlcharrefreplace')
         return item
 
-    def build_keywords(self, title: str, refs: List[Any], subitems: Any) -> List[str]:
-        keywords = []  # type: List[str]
+    def build_keywords(self, title: str, refs: list[Any], subitems: Any) -> list[str]:
+        keywords: list[str] = []
 
         # if len(refs) == 0: # XXX
         #     write_param('See Also', title)
         if len(refs) == 1:
             keywords.append(self.keyword_item(title, refs[0]))
         elif len(refs) > 1:
             for i, ref in enumerate(refs):  # XXX
@@ -234,32 +235,29 @@
 
         if subitems:
             for subitem in subitems:
                 keywords.extend(self.build_keywords(subitem[0], subitem[1], []))
 
         return keywords
 
-    def get_project_files(self, outdir: str) -> List[str]:
-        if not outdir.endswith(os.sep):
-            outdir += os.sep
-        olen = len(outdir)
+    def get_project_files(self, outdir: Path) -> list[str]:
         project_files = []
         staticdir = path.join(outdir, '_static')
         imagesdir = path.join(outdir, self.imagedir)
         for root, dirs, files in os.walk(outdir):
             resourcedir = root.startswith((staticdir, imagesdir))
             for fn in sorted(files):
                 if (resourcedir and not fn.endswith('.js')) or fn.endswith('.html'):
-                    filename = path.join(root, fn)[olen:]
+                    filename = path.relpath(path.join(root, fn), outdir)
                     project_files.append(canon_path(filename))
 
         return project_files
 
 
-def setup(app: Sphinx) -> Dict[str, Any]:
+def setup(app: Sphinx) -> dict[str, Any]:
     app.setup_extension('sphinx.builders.html')
     app.add_builder(QtHelpBuilder)
     app.add_message_catalog(__name__, path.join(package_dir, 'locales'))
 
     app.add_config_value('qthelp_basename', lambda self: make_filename(self.project), 'html')
     app.add_config_value('qthelp_namespace', None, 'html', [str])
     app.add_config_value('qthelp_theme', 'nonav', 'html')
```

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ar/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/ar/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ar/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/ar/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/bn/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/bn/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/bn/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/bn/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ca/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/ca/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ca/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/ca/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/cs/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/cs/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/cs/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/cs/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/cy/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/cy/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/cy/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/cy/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/da/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/da/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/da/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/da/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/de/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/de/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/de/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/de/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/el/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/el/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/el/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/el/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/eo/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/eo/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/eo/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/eo/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/es/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/es/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/es/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/es/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/et/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/et/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/et/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/et/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/eu/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/eu/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/eu/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/eu/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/fa/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/fa/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/fa/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/fa/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/fi/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/fi/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/fi/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/fi/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/fr/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/fr/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/fr/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/fr/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/he/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/he/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/he/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/he/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/hi/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/hi/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/hi/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/hi/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/hi_IN/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/hi_IN/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/hi_IN/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/hi_IN/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/hr/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/hr/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/hr/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/hr/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/hu/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/hu/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/hu/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/hu/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/id/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/id/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/id/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/id/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/it/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/it/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/it/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/it/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ja/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/ja/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ja/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/ja/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ko/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/ko/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ko/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/ko/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/lt/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/lt/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/lt/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/lt/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/lv/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/lv/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/lv/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/lv/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/mk/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/mk/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/mk/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/mk/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/nb_NO/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/nb_NO/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/nb_NO/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/nb_NO/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ne/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/ne/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ne/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/ne/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/nl/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/nl/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/nl/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/nl/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/pl/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/pl/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/pl/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/pl/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/pt/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/pt/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/pt/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/pt/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/pt_BR/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/pt_BR/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/pt_BR/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/pt_BR/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/pt_PT/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/pt_PT/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/pt_PT/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/pt_PT/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ro/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/ro/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ro/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/ro/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ru/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/ru/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ru/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/ru/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/si/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/si/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/si/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/si/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/sk/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/sk/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/sk/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/sk/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/sl/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/sl/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/sl/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/sl/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/sphinxcontrib.qthelp.pot` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/sphinxcontrib.qthelp.pot`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/sr/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/sr/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/sr/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/sr/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/sr@latin/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/sr@latin/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/sr@latin/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/sr@latin/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/sv/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/sv/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/sv/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/sv/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ta/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/ta/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/ta/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/ta/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/tr/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/tr/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/tr/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/tr/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/uk_UA/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/uk_UA/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/uk_UA/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/uk_UA/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/vi/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/vi/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/vi/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/vi/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/zh_CN/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/zh_CN/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/zh_CN/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/zh_CN/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/zh_TW/LC_MESSAGES/sphinxcontrib.qthelp.mo` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/zh_TW/LC_MESSAGES/sphinxcontrib.qthelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/locales/zh_TW/LC_MESSAGES/sphinxcontrib.qthelp.po` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/locales/zh_TW/LC_MESSAGES/sphinxcontrib.qthelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/templates/project.qhcp` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/templates/project.qhcp`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/sphinxcontrib/qthelp/templates/project.qhp` & `sphinxcontrib_qthelp-1.0.4/sphinxcontrib/qthelp/templates/project.qhp`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/tests/roots/test-need-escaped/index.rst` & `sphinxcontrib_qthelp-1.0.4/tests/roots/test-need-escaped/index.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-qthelp-1.0.3/tests/test_qthelp.py` & `sphinxcontrib_qthelp-1.0.4/tests/test_qthelp.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,28 @@
-"""
-    test_qthelp
-    ~~~~~~~~~~~
-
-    Test for qthelp extension.
-
-    :copyright: Copyright 2007-2019 by the Sphinx team, see AUTHORS.
-    :license: BSD, see LICENSE for details.
-"""
+"""Test for qthelp extension."""
 
 import pytest
 
 from sphinx.testing.util import etree_parse
 
 
 @pytest.mark.sphinx('qthelp', testroot='basic')
 def test_qthelp_basic(app, status, warning):
     app.builder.build_all()
 
-    qhp = (app.outdir / 'Python.qhp').text()
+    qhp = (app.outdir / 'Python.qhp').read_text()
     assert '<customFilter name="Python ">' in qhp
     assert '<filterAttribute>Python</filterAttribute>' in qhp
     assert '<filterAttribute></filterAttribute>' in qhp
     assert '<section title="Python  documentation" ref="index.html">' in qhp
     assert '<file>genindex.html</file>' in qhp
     assert '<file>index.html</file>' in qhp
     assert '<file>_static/basic.css</file>' in qhp
 
-    qhcp = (app.outdir / 'Python.qhcp').text()
+    qhcp = (app.outdir / 'Python.qhcp').read_text()
     assert '<title>Python  documentation</title>' in qhcp
     assert '<homePage>qthelp://org.sphinx.python/doc/index.html</homePage>' in qhcp
     assert '<startPage>qthelp://org.sphinx.python/doc/index.html</startPage>' in qhcp
     assert '<input>Python.qhp</input>' in qhcp
     assert '<output>Python.qch</output>' in qhcp
     assert '<file>Python.qch</file>' in qhcp
 
@@ -87,48 +79,48 @@
 
 
 @pytest.mark.sphinx('qthelp', testroot='basic')
 def test_qthelp_namespace(app, status, warning):
     # default namespace
     app.builder.build_all()
 
-    qhp = (app.outdir / 'Python.qhp').text()
+    qhp = (app.outdir / 'Python.qhp').read_text()
     assert '<namespace>org.sphinx.python</namespace>' in qhp
 
-    qhcp = (app.outdir / 'Python.qhcp').text()
+    qhcp = (app.outdir / 'Python.qhcp').read_text()
     assert '<homePage>qthelp://org.sphinx.python/doc/index.html</homePage>' in qhcp
     assert '<startPage>qthelp://org.sphinx.python/doc/index.html</startPage>' in qhcp
 
     # give a namespace
     app.config.qthelp_namespace = 'org.sphinx-doc.sphinx'
     app.builder.build_all()
 
-    qhp = (app.outdir / 'Python.qhp').text()
+    qhp = (app.outdir / 'Python.qhp').read_text()
     assert '<namespace>org.sphinx-doc.sphinx</namespace>' in qhp
 
-    qhcp = (app.outdir / 'Python.qhcp').text()
+    qhcp = (app.outdir / 'Python.qhcp').read_text()
     assert '<homePage>qthelp://org.sphinx-doc.sphinx/doc/index.html</homePage>' in qhcp
     assert '<startPage>qthelp://org.sphinx-doc.sphinx/doc/index.html</startPage>' in qhcp
 
 
 @pytest.mark.sphinx('qthelp', testroot='basic')
 def test_qthelp_title(app, status, warning):
     # default title
     app.builder.build_all()
 
-    qhp = (app.outdir / 'Python.qhp').text()
+    qhp = (app.outdir / 'Python.qhp').read_text()
     assert '<section title="Python  documentation" ref="index.html">' in qhp
 
-    qhcp = (app.outdir / 'Python.qhcp').text()
+    qhcp = (app.outdir / 'Python.qhcp').read_text()
     assert '<title>Python  documentation</title>' in qhcp
 
     # give a title
     app.config.html_title = 'Sphinx <b>"full"</b> title'
     app.config.html_short_title = 'Sphinx <b>"short"</b> title'
     app.builder.build_all()
 
-    qhp = (app.outdir / 'Python.qhp').text()
+    qhp = (app.outdir / 'Python.qhp').read_text()
     assert ('<section title="Sphinx &lt;b&gt;&#34;full&#34;&lt;/b&gt; title" ref="index.html">'
             in qhp)
 
-    qhcp = (app.outdir / 'Python.qhcp').text()
+    qhcp = (app.outdir / 'Python.qhcp').read_text()
     assert '<title>Sphinx &lt;b&gt;&#34;short&#34;&lt;/b&gt; title</title>' in qhcp
```

