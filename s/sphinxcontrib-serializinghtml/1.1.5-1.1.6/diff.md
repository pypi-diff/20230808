# Comparing `tmp/sphinxcontrib-serializinghtml-1.1.5.tar.gz` & `tmp/sphinxcontrib_serializinghtml-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib-serializinghtml-1.1.5.tar", last modified: Sat May 22 16:07:19 2021, max compression
+gzip compressed data, was "sphinxcontrib_serializinghtml-1.1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinxcontrib-serializinghtml-1.1.5.tar` & `sphinxcontrib_serializinghtml-1.1.6.tar`

### file list

```diff
@@ -1,250 +1,122 @@
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.767718 sphinxcontrib-serializinghtml-1.1.5/
--rw-r--r--   0 tkomiya    (502) staff       (20)      613 2021-05-22 16:05:46.000000 sphinxcontrib-serializinghtml-1.1.5/CHANGES
--rw-r--r--   0 tkomiya    (502) staff       (20)     1453 2020-01-12 15:40:03.000000 sphinxcontrib-serializinghtml-1.1.5/LICENSE
--rw-r--r--   0 tkomiya    (502) staff       (20)      153 2020-01-12 15:40:03.000000 sphinxcontrib-serializinghtml-1.1.5/MANIFEST.in
--rw-r--r--   0 tkomiya    (502) staff       (20)     1372 2021-05-22 16:07:19.767856 sphinxcontrib-serializinghtml-1.1.5/PKG-INFO
--rw-r--r--   0 tkomiya    (502) staff       (20)      923 2020-01-12 15:40:03.000000 sphinxcontrib-serializinghtml-1.1.5/README.rst
--rw-r--r--   0 tkomiya    (502) staff       (20)      530 2021-05-22 16:07:19.768390 sphinxcontrib-serializinghtml-1.1.5/setup.cfg
--rw-r--r--   0 tkomiya    (502) staff       (20)     2119 2020-02-29 04:02:32.000000 sphinxcontrib-serializinghtml-1.1.5/setup.py
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.730647 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/
--rw-r--r--   0 tkomiya    (502) staff       (20)      350 2020-01-12 15:40:03.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/__init__.py
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.731386 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/
--rw-r--r--   0 tkomiya    (502) staff       (20)     6064 2021-05-16 11:15:14.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/__init__.py
--rw-r--r--   0 tkomiya    (502) staff       (20)     1095 2020-01-12 15:40:03.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/jsonimpl.py
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.731637 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.731912 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/.tx/
--rw-r--r--   0 tkomiya    (502) staff       (20)      245 2020-01-12 15:40:03.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/.tx/config
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.716759 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ar/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.732410 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ar/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      882 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ar/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1346 2021-05-22 16:06:10.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ar/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.716965 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/bg/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.732920 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/bg/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      513 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/bg/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1001 2021-05-22 16:06:18.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/bg/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.717193 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/bn/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.733447 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/bn/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      511 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/bn/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)      999 2021-05-22 16:06:14.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/bn/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.717404 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ca/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.733975 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ca/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      511 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ca/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)      999 2021-05-22 16:06:15.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ca/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.717609 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/cak/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.734470 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/cak/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      473 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/cak/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1003 2021-05-22 16:06:10.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/cak/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.717817 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/cs/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.734966 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/cs/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      589 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/cs/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1077 2021-05-22 16:06:10.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/cs/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.718076 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/cy/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.735476 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/cy/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      554 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/cy/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1042 2021-05-22 16:06:10.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/cy/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.718321 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/da/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.736007 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/da/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      751 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/da/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1209 2021-05-22 16:06:11.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/da/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.718547 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/de/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.736597 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/de/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      510 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/de/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)      998 2021-05-22 16:06:14.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/de/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.718759 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/el/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.737110 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/el/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      871 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/el/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1342 2021-05-22 16:06:16.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/el/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.718975 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/eo/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.737653 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/eo/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      513 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/eo/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1001 2021-05-22 16:06:14.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/eo/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.719188 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/es/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.738152 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/es/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      797 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/es/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1336 2021-05-22 16:06:11.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/es/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.719394 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/et/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.738639 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/et/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      663 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/et/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1188 2021-05-22 16:06:15.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/et/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.719612 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/eu/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.739146 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/eu/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      510 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/eu/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)      998 2021-05-22 16:06:14.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/eu/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.719822 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/fa/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.739634 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/fa/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      914 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/fa/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1375 2021-05-22 16:06:17.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/fa/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.720030 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/fi/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.740150 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/fi/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      511 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/fi/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)      999 2021-05-22 16:06:14.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/fi/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.720234 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/fr/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.740651 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/fr/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      794 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/fr/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1298 2021-05-22 16:06:14.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/fr/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.720436 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/he/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.741140 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/he/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      604 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/he/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1092 2021-05-22 16:06:11.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/he/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.720649 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/hi/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.741616 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/hi/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      921 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/hi/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1379 2021-05-22 16:06:10.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/hi/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.720869 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/hi_IN/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.742169 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/hi_IN/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      523 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/hi_IN/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1011 2021-05-22 16:06:10.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/hi_IN/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.721094 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/hr/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.742706 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/hr/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      584 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/hr/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1072 2021-05-22 16:06:15.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/hr/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.721298 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/hu/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.743209 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/hu/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      797 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/hu/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1240 2021-05-22 16:06:10.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/hu/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.721496 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/id/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.743750 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/id/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      750 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/id/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1190 2021-05-22 16:06:10.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/id/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.721712 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/it/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.744240 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/it/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      511 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/it/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)      999 2021-05-22 16:06:17.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/it/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.721914 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ja/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.744723 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ja/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      804 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ja/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1274 2021-05-22 16:06:15.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ja/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.722110 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ko/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.745227 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ko/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      774 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ko/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1220 2021-05-22 16:06:14.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ko/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.722317 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/lt/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.745720 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/lt/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      645 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/lt/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1133 2021-05-22 16:06:11.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/lt/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.722514 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/lv/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.746221 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/lv/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      546 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/lv/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1034 2021-05-22 16:06:11.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/lv/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.722751 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/mk/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.746693 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/mk/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      544 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/mk/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1032 2021-05-22 16:06:10.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/mk/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.722962 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/nb_NO/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.747189 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/nb_NO/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      536 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/nb_NO/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1024 2021-05-22 16:06:15.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/nb_NO/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.723166 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ne/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.747667 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ne/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      510 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ne/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)      998 2021-05-22 16:06:17.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ne/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.723376 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/nl/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.748158 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/nl/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      509 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/nl/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)      997 2021-05-22 16:06:13.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/nl/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.723585 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/pl/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.748678 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/pl/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      760 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/pl/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1260 2021-05-22 16:06:15.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/pl/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.723797 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/pt/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.749178 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/pt/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      514 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/pt/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1002 2021-05-22 16:06:15.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/pt/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.724002 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/pt_BR/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.749664 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/pt_BR/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      802 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/pt_BR/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1270 2021-05-22 16:06:17.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/pt_BR/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.724204 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/pt_PT/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.750181 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/pt_PT/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      531 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/pt_PT/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1019 2021-05-22 16:06:17.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/pt_PT/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.724420 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ro/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.750662 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ro/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      553 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ro/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1041 2021-05-22 16:06:17.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ro/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.724622 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ru/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.751140 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ru/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      649 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ru/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1137 2021-05-22 16:06:14.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ru/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.724862 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/si/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.751635 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/si/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      511 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/si/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)      999 2021-05-22 16:06:10.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/si/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.725135 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sk/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.752144 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sk/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      833 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sk/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1284 2021-05-22 16:06:18.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sk/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.725360 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sl/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.752632 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sl/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      565 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sl/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1053 2021-05-22 16:06:11.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sl/LC_MESSAGES/sphinxcontrib.serializinghtml.po
--rw-r--r--   0 tkomiya    (502) staff       (20)      940 2020-01-12 15:40:03.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sphinxcontrib.serializinghtml.pot
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.725583 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sq/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.753169 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sq/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      776 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sq/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1241 2021-05-22 16:06:18.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sq/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.725797 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sr/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.754916 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sr/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      585 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sr/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1073 2021-05-22 16:06:15.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sr/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.726014 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sr@latin/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.755403 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sr@latin/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      605 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sr@latin/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1093 2021-05-22 16:06:14.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sr@latin/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.726235 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sr_RS/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.755895 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sr_RS/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      600 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sr_RS/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1088 2021-05-22 16:06:17.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sr_RS/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.726446 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sv/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.761122 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sv/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      511 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sv/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)      999 2021-05-22 16:06:11.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sv/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.726657 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ta/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.761744 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ta/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      509 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ta/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)      997 2021-05-22 16:06:16.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ta/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.726886 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/te/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.762215 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/te/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      510 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/te/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)      998 2021-05-22 16:06:18.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/te/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.727106 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/tr/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.762685 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/tr/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      762 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/tr/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1195 2021-05-22 16:06:11.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/tr/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.727318 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/uk_UA/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.763153 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/uk_UA/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      751 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/uk_UA/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1239 2021-05-22 16:06:15.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/uk_UA/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.727526 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ur/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.763616 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ur/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      508 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ur/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)      996 2021-05-22 16:06:15.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ur/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.727741 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/vi/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.764069 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/vi/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      507 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/vi/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)      995 2021-05-22 16:06:11.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/vi/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.727960 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/zh_CN/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.764532 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/zh_CN/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      784 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/zh_CN/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1243 2021-05-22 16:06:14.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/zh_CN/LC_MESSAGES/sphinxcontrib.serializinghtml.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.728170 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/zh_TW/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.765012 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/zh_TW/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      519 2021-05-22 16:06:29.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/zh_TW/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1007 2021-05-22 16:06:17.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/zh_TW/LC_MESSAGES/sphinxcontrib.serializinghtml.po
--rw-r--r--   0 tkomiya    (502) staff       (20)      287 2020-02-29 04:18:19.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/version.py
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.766681 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib_serializinghtml.egg-info/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1372 2021-05-22 16:07:19.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib_serializinghtml.egg-info/PKG-INFO
--rw-r--r--   0 tkomiya    (502) staff       (20)    10177 2021-05-22 16:07:19.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib_serializinghtml.egg-info/SOURCES.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)        1 2021-05-22 16:07:19.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib_serializinghtml.egg-info/dependency_links.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)       14 2021-05-22 16:07:19.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib_serializinghtml.egg-info/namespace_packages.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)        1 2020-02-29 04:16:19.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib_serializinghtml.egg-info/not-zip-safe
--rw-r--r--   0 tkomiya    (502) staff       (20)       50 2021-05-22 16:07:19.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib_serializinghtml.egg-info/requires.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)       14 2021-05-22 16:07:19.000000 sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib_serializinghtml.egg-info/top_level.txt
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.767129 sphinxcontrib-serializinghtml-1.1.5/tests/
--rw-r--r--   0 tkomiya    (502) staff       (20)      402 2020-01-12 15:40:03.000000 sphinxcontrib-serializinghtml-1.1.5/tests/conftest.py
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.728636 sphinxcontrib-serializinghtml-1.1.5/tests/roots/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2021-05-22 16:07:19.767521 sphinxcontrib-serializinghtml-1.1.5/tests/roots/test-basic/
--rw-r--r--   0 tkomiya    (502) staff       (20)        0 2020-01-12 15:40:03.000000 sphinxcontrib-serializinghtml-1.1.5/tests/roots/test-basic/conf.py
--rw-r--r--   0 tkomiya    (502) staff       (20)       22 2020-01-12 15:40:03.000000 sphinxcontrib-serializinghtml-1.1.5/tests/roots/test-basic/index.rst
--rw-r--r--   0 tkomiya    (502) staff       (20)      458 2020-01-12 15:40:03.000000 sphinxcontrib-serializinghtml-1.1.5/tests/test_serializinghtml.py
--rw-r--r--   0 tkomiya    (502) staff       (20)      606 2021-05-16 11:14:58.000000 sphinxcontrib-serializinghtml-1.1.5/tox.ini
+-rw-r--r--   0        0        0      765 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/CHANGES
+-rw-r--r--   0        0        0     1453 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/LICENSE
+-rw-r--r--   0        0        0      480 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/README.rst
+-rw-r--r--   0        0        0     2083 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0     5800 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/__init__.py
+-rw-r--r--   0        0        0      842 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/jsonimpl.py
+-rw-r--r--   0        0        0      245 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/.tx/config
+-rw-r--r--   0        0        0      882 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/ar/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1346 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/ar/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      513 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/bg/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1001 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/bg/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      511 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/bn/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0      999 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/bn/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      511 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/ca/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0      999 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/ca/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      473 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/cak/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1003 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/cak/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      589 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/cs/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1077 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/cs/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      554 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/cy/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1042 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/cy/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      751 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/da/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1209 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/da/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      510 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/de/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0      998 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/de/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      871 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/el/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1342 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/el/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      513 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/eo/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1001 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/eo/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      797 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/es/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1336 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/es/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      663 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/et/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1188 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/et/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      510 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/eu/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0      998 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/eu/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      914 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/fa/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1375 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/fa/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      511 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/fi/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0      999 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/fi/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      794 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/fr/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1298 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/fr/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      604 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/he/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1092 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/he/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      921 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/hi/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1379 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/hi/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      523 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/hi_IN/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1011 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/hi_IN/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      584 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/hr/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1072 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/hr/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      797 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/hu/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1240 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/hu/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      750 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/id/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1190 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/id/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      511 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/it/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0      999 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/it/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      804 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/ja/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1274 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/ja/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      774 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/ko/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1220 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/ko/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      645 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/lt/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1133 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/lt/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      546 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/lv/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1034 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/lv/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      544 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/mk/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1032 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/mk/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      536 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/nb_NO/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1024 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/nb_NO/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      510 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/ne/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0      998 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/ne/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      509 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/nl/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0      997 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/nl/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      760 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/pl/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1260 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/pl/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      514 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/pt/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1002 2023-08-08 18:58:57.140365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/pt/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      802 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/pt_BR/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1270 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/pt_BR/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      531 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/pt_PT/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1019 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/pt_PT/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      553 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/ro/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1041 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/ro/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      649 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/ru/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1137 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/ru/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      511 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/si/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0      999 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/si/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      833 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/sk/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1284 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/sk/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      565 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/sl/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1053 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/sl/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      940 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/sphinxcontrib.serializinghtml.pot
+-rw-r--r--   0        0        0      776 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/sq/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1241 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/sq/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      585 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/sr/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1073 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/sr/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      605 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/sr@latin/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1093 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/sr@latin/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      600 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/sr_RS/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1088 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/sr_RS/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      511 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/sv/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0      999 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/sv/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      509 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/ta/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0      997 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/ta/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      510 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/te/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0      998 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/te/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      762 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/tr/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1195 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/tr/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      751 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/uk_UA/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1239 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/uk_UA/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      508 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/ur/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0      996 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/ur/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      507 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/vi/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0      995 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/vi/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      784 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/zh_CN/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1243 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/zh_CN/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      519 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/zh_TW/LC_MESSAGES/sphinxcontrib.serializinghtml.mo
+-rw-r--r--   0        0        0     1007 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/zh_TW/LC_MESSAGES/sphinxcontrib.serializinghtml.po
+-rw-r--r--   0        0        0      187 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/tests/roots/test-basic/conf.py
+-rw-r--r--   0        0        0       22 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/tests/roots/test-basic/index.rst
+-rw-r--r--   0        0        0      287 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/tests/test_serializinghtml.py
+-rw-r--r--   0        0        0      572 2023-08-08 18:58:57.144365 sphinxcontrib_serializinghtml-1.1.6/tox.ini
+-rw-r--r--   0        0        0     2311 1970-01-01 00:00:00.000000 sphinxcontrib_serializinghtml-1.1.6/PKG-INFO
```

### Comparing `sphinxcontrib-serializinghtml-1.1.5/CHANGES` & `sphinxcontrib_serializinghtml-1.1.6/CHANGES`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Release 1.1.6 (2023-08-07)
+==========================
+
+* Drop support for Python 3.5, 3.6, 3.7, and 3.8
+* Raise minimum required Sphinx version to 5.0
+
 Release 1.1.5 (2021-05-23)
 ==========================
 
 * Remove deprecation warnings for Sphinx-3.x
 
 Release 1.1.4 (2020-02-29)
 ==========================
```

### Comparing `sphinxcontrib-serializinghtml-1.1.5/LICENSE` & `sphinxcontrib_serializinghtml-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/PKG-INFO` & `sphinxcontrib_serializinghtml-1.1.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,64 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-serializinghtml
-Version: 1.1.5
-Summary: sphinxcontrib-serializinghtml is a sphinx extension which outputs "serialized" HTML files (json and pickle).
-Home-page: http://sphinx-doc.org/
-Author: Georg Brandl
-Author-email: georg@python.org
-License: BSD
-Download-URL: https://pypi.org/project/sphinxcontrib-serializinghtml/
-Description: 
-        sphinxcontrib-serializinghtml is a sphinx extension which outputs
-        "serialized" HTML files (json and pickle).
-        
-Platform: any
+Version: 1.1.6
+Summary: sphinxcontrib-serializinghtml is a sphinx extension which outputs "serialized" HTML files (json and pickle)
+Author-email: Georg Brandl <georg@python.org>
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
-Requires-Python: >=3.5
-Provides-Extra: test
+Requires-Dist: Sphinx>=5
+Requires-Dist: flake8 ; extra == "lint"
+Requires-Dist: mypy ; extra == "lint"
+Requires-Dist: docutils-stubs ; extra == "lint"
+Requires-Dist: pytest ; extra == "test"
+Project-URL: Changelog, https://www.sphinx-doc.org/en/master/changes.html
+Project-URL: Code, https://github.com/sphinx-doc/sphinxcontrib-serializinghtml
+Project-URL: Download, https://pypi.org/project/sphinxcontrib-serializinghtml/
+Project-URL: Homepage, https://www.sphinx-doc.org/
+Project-URL: Issue tracker, https://github.com/sphinx-doc/sphinx/issues
 Provides-Extra: lint
+Provides-Extra: test
+
+=============================
+sphinxcontrib-serializinghtml
+=============================
+
+sphinxcontrib-serializinghtml is a sphinx extension which outputs
+"serialized" HTML files (json and pickle).
+
+For more details, please visit http://www.sphinx-doc.org/.
+
+Installing
+==========
+
+Install from PyPI::
+
+   pip install -U sphinxcontrib-serializinghtml
+
+Contributing
+============
+
+See `CONTRIBUTING.rst`__
+
+.. __: https://github.com/sphinx-doc/sphinx/blob/master/CONTRIBUTING.rst
+
```

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/__init__.py` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,24 @@
-"""
-    sphinxcontrib.serializinghtml
-    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-    :copyright: Copyright 2007-2019 by the Sphinx team, see README.
-    :license: BSD, see LICENSE for details.
-"""
+from __future__ import annotations
 
+import os
 import pickle
 import types
 from os import path
-from typing import Any, Dict
+from typing import Any
 
 from sphinx.application import ENV_PICKLE_FILENAME, Sphinx
 from sphinx.builders.html import BuildInfo, StandaloneHTMLBuilder
 from sphinx.locale import get_translation
 from sphinx.util.osutil import SEP, copyfile, ensuredir, os_path
 
 from sphinxcontrib.serializinghtml import jsonimpl
-from sphinxcontrib.serializinghtml.version import __version__
 
-if False:
-    # For type annotation
-    from typing import Any, Dict, Tuple  # NOQA
+__version__ = '1.1.6'
+__version_info__ = (1, 1, 6)
 
 package_dir = path.abspath(path.dirname(__file__))
 
 __ = get_translation(__name__, 'console')
 
 
 #: the filename for the "last build" file (for serializing builders)
@@ -35,59 +28,56 @@
 class SerializingHTMLBuilder(StandaloneHTMLBuilder):
     """
     An abstract builder that serializes the generated HTML.
     """
     #: the serializing implementation to use.  Set this to a module that
     #: implements a `dump`, `load`, `dumps` and `loads` functions
     #: (pickle, simplejson etc.)
-    implementation = None  # type: Any
+    implementation: Any = None
     implementation_dumps_unicode = False
     #: additional arguments for dump()
-    additional_dump_args = ()  # type: Tuple
+    additional_dump_args: tuple = ()
 
     #: the filename for the global context file
-    globalcontext_filename = None  # type: str
+    globalcontext_filename: str = ''
 
     supported_image_types = ['image/svg+xml', 'image/png',
                              'image/gif', 'image/jpeg']
 
-    def init(self):
-        # type: () -> None
+    def init(self) -> None:
         self.build_info = BuildInfo(self.config, self.tags)
         self.imagedir = '_images'
-        self.current_docname = None
-        self.theme = None       # no theme necessary
-        self.templates = None   # no template bridge necessary
+        self.current_docname = ''
+        self.theme = None  # type: ignore[assignment] # no theme necessary
+        self.templates = None  # no template bridge necessary
         self.init_templates()
         self.init_highlighter()
         self.init_css_files()
         self.init_js_files()
         self.use_index = self.get_builder_config('use_index', 'html')
 
-    def get_target_uri(self, docname, typ=None):
-        # type: (str, str) -> str
+    def get_target_uri(self, docname: str, typ: str | None = None) -> str:
         if docname == 'index':
             return ''
         if docname.endswith(SEP + 'index'):
             return docname[:-5]  # up to sep
         return docname + SEP
 
-    def dump_context(self, context, filename):
-        # type: (Dict, str) -> None
+    def dump_context(self, context: dict, filename: str | os.PathLike[str]) -> None:
         if self.implementation_dumps_unicode:
             with open(filename, 'w', encoding='utf-8') as ft:
                 self.implementation.dump(context, ft, *self.additional_dump_args)
         else:
             with open(filename, 'wb') as fb:
                 self.implementation.dump(context, fb, *self.additional_dump_args)
 
-    def handle_page(self, pagename, ctx, templatename='page.html',
-                    outfilename=None, event_arg=None):
-        # type: (str, Dict, str, str, Any) -> None
+    def handle_page(self, pagename: str, ctx: dict, templatename: str = 'page.html',
+                    outfilename: str | None = None, event_arg: Any = None) -> None:
         ctx['current_page_name'] = pagename
+        ctx.setdefault('pathto', lambda p: p)
         self.add_sidebars(pagename, ctx)
 
         if not outfilename:
             outfilename = path.join(self.outdir,
                                     os_path(pagename) + self.out_suffix)
 
         # we're not taking the return value here, since no template is
@@ -106,18 +96,17 @@
         # "show source" link
         if ctx.get('sourcename'):
             source_name = path.join(self.outdir, '_sources',
                                     os_path(ctx['sourcename']))
             ensuredir(path.dirname(source_name))
             copyfile(self.env.doc2path(pagename), source_name)
 
-    def handle_finish(self):
-        # type: () -> None
+    def handle_finish(self) -> None:
         # dump the global context
-        outfilename = path.join(self.outdir, self.globalcontext_filename)
+        outfilename = self.outdir / self.globalcontext_filename
         self.dump_context(self.globalcontext, outfilename)
 
         # super here to dump the search index
         super().handle_finish()
 
         # copy the environment file from the doctree dir to the output dir
         # as needed by the web app
@@ -158,15 +147,15 @@
     indexer_format = jsonimpl
     indexer_dumps_unicode = True
     out_suffix = '.fjson'
     globalcontext_filename = 'globalcontext.json'
     searchindex_filename = 'searchindex.json'
 
 
-def setup(app: Sphinx) -> Dict[str, Any]:
+def setup(app: Sphinx) -> dict[str, Any]:
     app.setup_extension('sphinx.builders.html')
     app.add_builder(JSONHTMLBuilder)
     app.add_builder(PickleHTMLBuilder)
     app.add_message_catalog(__name__, path.join(package_dir, 'locales'))
 
     return {
         'version': __version__,
```

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/jsonimpl.py` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/jsonimpl.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,33 @@
-"""
-    sphinx.util.jsonimpl
-    ~~~~~~~~~~~~~~~~~~~~
-
-    JSON serializer implementation wrapper.
-
-    :copyright: Copyright 2007-2019 by the Sphinx team, see AUTHORS.
-    :license: BSD, see LICENSE for details.
-"""
+"""JSON serializer implementation wrapper."""
+
+from __future__ import annotations
 
 import json
 from collections import UserString
-
-if False:
-    # For type annotation
-    from typing import Any, IO  # NOQA
+from typing import Any, IO
 
 
 class SphinxJSONEncoder(json.JSONEncoder):
     """JSONEncoder subclass that forces translation proxies."""
-    def default(self, obj):
-        # type: (Any) -> str
+    def default(self, obj: Any) -> str:
         if isinstance(obj, UserString):
             return str(obj)
         return super().default(obj)
 
 
-def dump(obj, fp, *args, **kwds):
-    # type: (Any, IO, Any, Any) -> None
+def dump(obj: Any, fp: IO, *args: Any, **kwds: Any) -> None:
     kwds['cls'] = SphinxJSONEncoder
     json.dump(obj, fp, *args, **kwds)
 
 
-def dumps(obj, *args, **kwds):
-    # type: (Any, Any, Any) -> str
+def dumps(obj: Any, *args: Any, **kwds: Any) -> str:
     kwds['cls'] = SphinxJSONEncoder
     return json.dumps(obj, *args, **kwds)
 
 
-def load(*args, **kwds):
-    # type: (Any, Any) -> Any
+def load(*args: Any, **kwds: Any) -> Any:
     return json.load(*args, **kwds)
 
 
-def loads(*args, **kwds):
-    # type: (Any, Any) -> Any
+def loads(*args: Any, **kwds: Any) -> Any:
     return json.loads(*args, **kwds)
```

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ar/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/ar/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ar/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/ar/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/bg/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/bg/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/bg/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/bg/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/bn/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/bn/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ca/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/ca/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/cak/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/cak/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/cs/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/cs/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/cs/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/cs/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/cy/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/cy/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/cy/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/cy/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/da/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/da/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/da/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/da/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/de/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/de/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/el/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/el/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/el/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/el/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/eo/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/eo/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/eo/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/eo/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/es/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/es/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/es/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/es/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/et/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/et/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/et/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/et/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/eu/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/eu/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/fa/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/fa/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/fa/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/fa/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/fi/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/fi/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/fr/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/fr/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/fr/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/fr/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/he/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/he/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/he/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/he/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/hi/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/hi/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/hi/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/hi/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/hi_IN/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/hi_IN/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/hi_IN/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/hi_IN/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/hr/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/hr/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/hr/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/hr/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/hu/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/hu/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/hu/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/hu/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/id/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/id/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/id/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/id/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/it/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/it/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ja/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/ja/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ja/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/ja/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ko/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/ko/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ko/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/ko/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/lt/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/lt/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/lt/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/lt/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/lv/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/lv/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/lv/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/lv/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/mk/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/mk/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/mk/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/mk/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/nb_NO/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/nb_NO/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/nb_NO/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/nb_NO/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ne/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/ne/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/nl/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/nl/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/pl/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/pl/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/pl/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/pl/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/pt/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/pt/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/pt/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/pt/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/pt_BR/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/pt_BR/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/pt_BR/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/pt_BR/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/pt_PT/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/pt_PT/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/pt_PT/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/pt_PT/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ro/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/ro/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ro/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/ro/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ru/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/ru/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ru/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/ru/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/si/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/si/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sk/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/sk/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sk/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/sk/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sl/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/sl/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sl/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/sl/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sphinxcontrib.serializinghtml.pot` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/sphinxcontrib.serializinghtml.pot`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sq/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/sq/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sq/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/sq/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sr/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/sr/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sr/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/sr/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sr@latin/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/sr@latin/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sr@latin/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/sr@latin/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sr_RS/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/sr_RS/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sr_RS/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/sr_RS/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/sv/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/sv/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ta/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/ta/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/te/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/te/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/tr/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/tr/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/tr/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/tr/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/uk_UA/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/uk_UA/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/uk_UA/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/uk_UA/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/ur/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/ur/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/vi/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/vi/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/zh_CN/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/zh_CN/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/zh_CN/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/zh_CN/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/zh_TW/LC_MESSAGES/sphinxcontrib.serializinghtml.mo` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/zh_TW/LC_MESSAGES/sphinxcontrib.serializinghtml.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-serializinghtml-1.1.5/sphinxcontrib/serializinghtml/locales/zh_TW/LC_MESSAGES/sphinxcontrib.serializinghtml.po` & `sphinxcontrib_serializinghtml-1.1.6/sphinxcontrib/serializinghtml/locales/zh_TW/LC_MESSAGES/sphinxcontrib.serializinghtml.po`

 * *Files identical despite different names*

