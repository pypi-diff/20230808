# Comparing `tmp/sphinxcontrib-devhelp-1.0.2.tar.gz` & `tmp/sphinxcontrib_devhelp-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sphinxcontrib-devhelp-1.0.2.tar", last modified: Sat Feb 29 04:14:35 2020, max compression
+gzip compressed data, was "sphinxcontrib_devhelp-1.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinxcontrib-devhelp-1.0.2.tar` & `sphinxcontrib_devhelp-1.0.3.tar`

### file list

```diff
@@ -1,225 +1,109 @@
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.472862 sphinxcontrib-devhelp-1.0.2/
--rw-r--r--   0 tkomiya    (502) staff       (20)      300 2020-02-29 04:14:22.000000 sphinxcontrib-devhelp-1.0.2/CHANGES
--rw-r--r--   0 tkomiya    (502) staff       (20)     1437 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/LICENSE
--rw-r--r--   0 tkomiya    (502) staff       (20)      145 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/MANIFEST.in
--rw-r--r--   0 tkomiya    (502) staff       (20)     1282 2020-02-29 04:14:35.473001 sphinxcontrib-devhelp-1.0.2/PKG-INFO
--rw-r--r--   0 tkomiya    (502) staff       (20)      901 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/README.rst
--rw-r--r--   0 tkomiya    (502) staff       (20)      474 2020-02-29 04:14:35.473535 sphinxcontrib-devhelp-1.0.2/setup.cfg
--rw-r--r--   0 tkomiya    (502) staff       (20)     2062 2020-02-29 04:02:39.000000 sphinxcontrib-devhelp-1.0.2/setup.py
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.425627 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/
--rw-r--r--   0 tkomiya    (502) staff       (20)      350 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/__init__.py
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.426147 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/
--rw-r--r--   0 tkomiya    (502) staff       (20)     5146 2020-01-12 15:58:33.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/__init__.py
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.426396 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.427034 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/.tx/
--rw-r--r--   0 tkomiya    (502) staff       (20)      221 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/.tx/config
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.412297 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ar/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.428081 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ar/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      959 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ar/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1106 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ar/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.412541 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/bn/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.428895 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/bn/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      877 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/bn/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1024 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/bn/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.412835 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ca/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.429803 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ca/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      877 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ca/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1024 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ca/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.413092 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/cs/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.431037 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/cs/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      955 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/cs/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1102 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/cs/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.413374 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/cy/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.432134 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/cy/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      920 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/cy/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1067 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/cy/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.413672 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/da/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.433034 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/da/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      876 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/da/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1023 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/da/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.413928 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/de/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.433874 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/de/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      876 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/de/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1023 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/de/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.414147 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/el/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.434676 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/el/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      875 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/el/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1022 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/el/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.414373 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/eo/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.435574 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/eo/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      879 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/eo/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1026 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/eo/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.414590 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/es/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.436397 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/es/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      877 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/es/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1024 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/es/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.414802 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/et/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.437280 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/et/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      885 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/et/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1293 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/et/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.415017 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/eu/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.438157 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/eu/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      876 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/eu/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1023 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/eu/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.415227 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/fa/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.439057 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/fa/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      876 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/fa/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1023 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/fa/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.415439 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/fi/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.439942 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/fi/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      877 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/fi/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1024 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/fi/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.415651 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/fr/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.440818 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/fr/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      901 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/fr/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1310 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/fr/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.415865 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/he/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.441677 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/he/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      970 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/he/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1117 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/he/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.416077 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/hi/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.442540 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/hi/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      875 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/hi/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1022 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/hi/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.416295 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/hi_IN/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.443428 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/hi_IN/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      889 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/hi_IN/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1036 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/hi_IN/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.416506 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/hr/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.444306 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/hr/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      950 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/hr/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1097 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/hr/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.416728 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/hu/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.445487 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/hu/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      879 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/hu/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1026 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/hu/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.416947 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/id/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.446279 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/id/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      877 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/id/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1296 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/id/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.417169 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/it/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.447179 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/it/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      877 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/it/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1024 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/it/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.417396 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ja/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.448063 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ja/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      871 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ja/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1018 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ja/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.417621 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ko/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.449024 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ko/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      869 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ko/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1016 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ko/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.417831 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/lt/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.449886 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/lt/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1011 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/lt/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1158 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/lt/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.418047 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/lv/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.450762 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/lv/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      912 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/lv/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1059 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/lv/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.418267 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/mk/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.451542 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/mk/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      910 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/mk/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1057 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/mk/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.418484 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/nb_NO/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.452372 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/nb_NO/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      902 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/nb_NO/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1049 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/nb_NO/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.418698 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ne/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.453252 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ne/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      876 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ne/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1023 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ne/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.418918 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/nl/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.454172 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/nl/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      875 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/nl/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1022 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/nl/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.419129 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/pl/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.455046 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/pl/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1012 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/pl/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1398 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/pl/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.419346 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/pt/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.455894 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/pt/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      880 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/pt/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1027 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/pt/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.419571 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/pt_BR/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.456751 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/pt_BR/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      894 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/pt_BR/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1041 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/pt_BR/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.419803 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/pt_PT/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.457593 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/pt_PT/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      897 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/pt_PT/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1044 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/pt_PT/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.420035 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ro/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.458422 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ro/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      919 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ro/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1066 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ro/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.420254 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ru/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.459544 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ru/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1015 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ru/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1162 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ru/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.420485 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/si/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.460404 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/si/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      877 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/si/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1024 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/si/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.420707 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/sk/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.461362 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/sk/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      951 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/sk/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1098 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/sk/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.420928 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/sl/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.462189 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/sl/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      931 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/sl/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1078 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/sl/LC_MESSAGES/sphinxcontrib.devhelp.po
--rw-r--r--   0 tkomiya    (502) staff       (20)      965 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/sphinxcontrib.devhelp.pot
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.421148 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/sr/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.463098 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/sr/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      951 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/sr/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1098 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/sr/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.421378 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/sr@latin/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.463930 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/sr@latin/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      973 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/sr@latin/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1120 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/sr@latin/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.421595 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/sv/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.464842 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/sv/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      877 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/sv/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1024 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/sv/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.421809 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ta/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.465819 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ta/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      875 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ta/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1022 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ta/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.422030 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/tr/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.466538 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/tr/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      876 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/tr/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1023 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/tr/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.422243 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/uk_UA/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.467284 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/uk_UA/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1117 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/uk_UA/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1264 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/uk_UA/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.422465 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/vi/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.468067 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/vi/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      873 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/vi/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1020 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/vi/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.422693 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/zh_CN/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.468897 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/zh_CN/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      930 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/zh_CN/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1368 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/zh_CN/LC_MESSAGES/sphinxcontrib.devhelp.po
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.422916 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/zh_TW/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.469649 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/zh_TW/LC_MESSAGES/
--rw-r--r--   0 tkomiya    (502) staff       (20)      885 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/zh_TW/LC_MESSAGES/sphinxcontrib.devhelp.mo
--rw-r--r--   0 tkomiya    (502) staff       (20)     1032 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/zh_TW/LC_MESSAGES/sphinxcontrib.devhelp.po
--rw-r--r--   0 tkomiya    (502) staff       (20)      271 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/version.py
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.471563 sphinxcontrib-devhelp-1.0.2/sphinxcontrib_devhelp.egg-info/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1282 2020-02-29 04:14:35.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib_devhelp.egg-info/PKG-INFO
--rw-r--r--   0 tkomiya    (502) staff       (20)     7455 2020-02-29 04:14:35.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib_devhelp.egg-info/SOURCES.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)        1 2020-02-29 04:14:35.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib_devhelp.egg-info/dependency_links.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)       14 2020-02-29 04:14:35.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib_devhelp.egg-info/namespace_packages.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)        1 2020-02-29 04:14:35.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib_devhelp.egg-info/not-zip-safe
--rw-r--r--   0 tkomiya    (502) staff       (20)       50 2020-02-29 04:14:35.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib_devhelp.egg-info/requires.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)       14 2020-02-29 04:14:35.000000 sphinxcontrib-devhelp-1.0.2/sphinxcontrib_devhelp.egg-info/top_level.txt
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.472050 sphinxcontrib-devhelp-1.0.2/tests/
--rw-r--r--   0 tkomiya    (502) staff       (20)      402 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/tests/conftest.py
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.423379 sphinxcontrib-devhelp-1.0.2/tests/roots/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-02-29 04:14:35.472506 sphinxcontrib-devhelp-1.0.2/tests/roots/test-basic/
--rw-r--r--   0 tkomiya    (502) staff       (20)        0 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/tests/roots/test-basic/conf.py
--rw-r--r--   0 tkomiya    (502) staff       (20)       22 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/tests/roots/test-basic/index.rst
--rw-r--r--   0 tkomiya    (502) staff       (20)      321 2020-01-12 15:31:11.000000 sphinxcontrib-devhelp-1.0.2/tests/test_devhelp.py
--rw-r--r--   0 tkomiya    (502) staff       (20)      474 2020-01-12 15:58:33.000000 sphinxcontrib-devhelp-1.0.2/tox.ini
+-rw-r--r--   0        0        0      451 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/CHANGES
+-rw-r--r--   0        0        0     1437 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/LICENSE
+-rw-r--r--   0        0        0      466 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/README.rst
+-rw-r--r--   0        0        0     1981 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4906 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/__init__.py
+-rw-r--r--   0        0        0      221 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/.tx/config
+-rw-r--r--   0        0        0      959 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/ar/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1106 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/ar/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      877 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/bn/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1024 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/bn/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      877 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/ca/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1024 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/ca/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      955 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/cs/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1102 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/cs/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      920 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/cy/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1067 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/cy/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      876 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/da/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1023 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/da/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      876 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/de/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1023 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/de/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      875 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/el/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1022 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/el/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      879 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/eo/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1026 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/eo/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      877 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/es/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1024 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/es/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      885 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/et/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1293 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/et/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      876 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/eu/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1023 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/eu/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      876 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/fa/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1023 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/fa/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      877 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/fi/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1024 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/fi/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      901 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/fr/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1310 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/fr/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      970 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/he/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1117 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/he/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      875 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/hi/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1022 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/hi/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      889 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/hi_IN/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1036 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/hi_IN/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      950 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/hr/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1097 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/hr/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      879 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/hu/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1026 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/hu/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      877 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/id/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1296 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/id/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      877 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/it/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1024 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/it/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      871 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/ja/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1018 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/ja/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      869 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/ko/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1016 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/ko/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0     1011 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/lt/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1158 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/lt/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      912 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/lv/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1059 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/lv/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      910 2023-08-08 18:58:45.224013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/mk/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1057 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/mk/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      902 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/nb_NO/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1049 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/nb_NO/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      876 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/ne/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1023 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/ne/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      875 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/nl/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1022 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/nl/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0     1012 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/pl/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1398 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/pl/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      880 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/pt/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1027 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/pt/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      894 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/pt_BR/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1041 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/pt_BR/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      897 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/pt_PT/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1044 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/pt_PT/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      919 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/ro/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1066 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/ro/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0     1015 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/ru/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1162 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/ru/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      877 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/si/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1024 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/si/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      951 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/sk/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1098 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/sk/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      931 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/sl/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1078 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/sl/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      965 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/sphinxcontrib.devhelp.pot
+-rw-r--r--   0        0        0      951 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/sr/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1098 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/sr/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      973 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/sr@latin/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1120 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/sr@latin/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      877 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/sv/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1024 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/sv/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      875 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/ta/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1022 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/ta/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      876 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/tr/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1023 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/tr/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0     1117 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/uk_UA/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1264 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/uk_UA/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      873 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/vi/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1020 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/vi/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      930 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/zh_CN/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1368 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/zh_CN/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      885 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/zh_TW/LC_MESSAGES/sphinxcontrib.devhelp.mo
+-rw-r--r--   0        0        0     1032 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/zh_TW/LC_MESSAGES/sphinxcontrib.devhelp.po
+-rw-r--r--   0        0        0      187 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/tests/roots/test-basic/conf.py
+-rw-r--r--   0        0        0       22 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/tests/roots/test-basic/index.rst
+-rw-r--r--   0        0        0      166 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/tests/test_devhelp.py
+-rw-r--r--   0        0        0      554 2023-08-08 18:58:45.228013 sphinxcontrib_devhelp-1.0.3/tox.ini
+-rw-r--r--   0        0        0     2241 1970-01-01 00:00:00.000000 sphinxcontrib_devhelp-1.0.3/PKG-INFO
```

### Comparing `sphinxcontrib-devhelp-1.0.2/LICENSE` & `sphinxcontrib_devhelp-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/__init__.py` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,39 @@
-"""
-    sphinxcontrib.devhelp
-    ~~~~~~~~~~~~~~~~~~~~~
-
-    Build HTML documentation and Devhelp_ support files.
-
-    .. _Devhelp: https://wiki.gnome.org/Apps/Devhelp
+"""Build HTML documentation and Devhelp_ support files.
 
-    :copyright: Copyright 2007-2019 by the Sphinx team, see README.
-    :license: BSD, see LICENSE for details.
+.. _Devhelp: https://wiki.gnome.org/Apps/Devhelp
 """
 
+from __future__ import annotations
+
 import gzip
 import re
 from os import path
-from typing import Any, Dict
+from typing import TYPE_CHECKING, Any
 
 from docutils import nodes
 from sphinx import addnodes
 from sphinx.application import Sphinx
 from sphinx.builders.html import StandaloneHTMLBuilder
 from sphinx.environment.adapters.indexentries import IndexEntries
 from sphinx.locale import get_translation
 from sphinx.util import logging
 from sphinx.util.nodes import NodeMatcher
 from sphinx.util.osutil import make_filename
 
-from sphinxcontrib.devhelp.version import __version__
-
 try:
     import xml.etree.ElementTree as etree
 except ImportError:
     import lxml.etree as etree  # type: ignore
 
+if TYPE_CHECKING:
+    from pathlib import Path
 
-if False:
-    # For type annotation
-    from typing import List  # NOQA
-
+__version__ = '1.0.3'
+__version_info__ = (1, 0, 3)
 
 logger = logging.getLogger(__name__)
 __ = get_translation(__name__, 'console')
 
 package_dir = path.abspath(path.dirname(__file__))
 
 
@@ -59,26 +52,23 @@
     supported_image_types = ['image/png', 'image/gif', 'image/jpeg']
 
     # don't add links
     add_permalinks = False
     # don't add sidebar etc.
     embedded = True
 
-    def init(self):
-        # type: () -> None
+    def init(self) -> None:
         super().init()
         self.out_suffix = '.html'
         self.link_suffix = '.html'
 
-    def handle_finish(self):
-        # type: () -> None
+    def handle_finish(self) -> None:
         self.build_devhelp(self.outdir, self.config.devhelp_basename)
 
-    def build_devhelp(self, outdir, outname):
-        # type: (str, str) -> None
+    def build_devhelp(self, outdir: Path, outname: str) -> None:
         logger.info(__('dumping devhelp index...'))
 
         # Basic info
         root = etree.Element('book',
                              title=self.config.html_title,
                              name=self.config.project,
                              link="index.html",
@@ -87,16 +77,15 @@
 
         # TOC
         chapters = etree.SubElement(root, 'chapters')
 
         tocdoc = self.env.get_and_resolve_doctree(
             self.config.master_doc, self, prune_toctrees=False)
 
-        def write_toc(node, parent):
-            # type: (nodes.Node, etree.Element) -> None
+        def write_toc(node: nodes.Node, parent: etree.Element) -> None:
             if isinstance(node, addnodes.compact_paragraph) or \
                isinstance(node, nodes.bullet_list):
                 for subnode in node:
                     write_toc(subnode, parent)
             elif isinstance(node, nodes.list_item):
                 item = etree.SubElement(parent, 'sub')
                 for subnode in node:
@@ -109,16 +98,15 @@
         for node in tocdoc.traverse(matcher):  # type: addnodes.compact_paragraph
             write_toc(node, chapters)
 
         # Index
         functions = etree.SubElement(root, 'functions')
         index = IndexEntries(self.env).create_index(self)
 
-        def write_index(title, refs, subitems):
-            # type: (str, List[Any], Any) -> None
+        def write_index(title: str, refs: list[Any], subitems: Any) -> None:
             if len(refs) == 0:
                 pass
             elif len(refs) == 1:
                 etree.SubElement(functions, 'function',
                                  name=title, link=refs[0][1])
             else:
                 for i, ref in enumerate(refs):
@@ -135,18 +123,18 @@
         for (key, group) in index:
             for title, (refs, subitems, key) in group:
                 write_index(title, refs, subitems)
 
         # Dump the XML file
         xmlfile = path.join(outdir, outname + '.devhelp.gz')
         with gzip.open(xmlfile, 'w') as f:
-            tree.write(f, 'utf-8')
+            tree.write(f, 'utf-8')  # type: ignore
 
 
-def setup(app: Sphinx) -> Dict[str, Any]:
+def setup(app: Sphinx) -> dict[str, Any]:
     app.setup_extension('sphinx.builders.html')
     app.add_builder(DevhelpBuilder)
     app.add_message_catalog(__name__, path.join(package_dir, 'locales'))
 
     app.add_config_value('devhelp_basename',
                          lambda self: make_filename(self.project),
                          'devhelp')
```

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ar/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/ar/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ar/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/ar/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/bn/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/bn/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/bn/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/bn/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ca/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/ca/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ca/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/ca/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/cs/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/cs/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/cs/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/cs/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/cy/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/cy/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/cy/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/cy/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/da/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/da/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/da/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/da/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/de/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/de/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/de/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/de/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/el/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/el/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/el/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/el/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/eo/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/eo/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/eo/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/eo/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/es/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/es/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/es/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/es/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/et/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/et/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/et/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/et/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/eu/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/eu/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/eu/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/eu/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/fa/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/fa/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/fa/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/fa/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/fi/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/fi/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/fi/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/fi/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/fr/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/fr/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/fr/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/fr/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/he/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/he/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/he/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/he/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/hi/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/hi/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/hi/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/hi/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/hi_IN/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/hi_IN/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/hi_IN/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/hi_IN/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/hr/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/hr/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/hr/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/hr/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/hu/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/hu/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/hu/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/hu/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/id/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/id/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/id/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/id/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/it/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/it/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/it/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/it/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ja/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/ja/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ja/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/ja/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ko/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/ko/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ko/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/ko/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/lt/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/lt/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/lt/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/lt/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/lv/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/lv/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/lv/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/lv/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/mk/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/mk/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/mk/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/mk/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/nb_NO/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/nb_NO/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/nb_NO/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/nb_NO/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ne/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/ne/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ne/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/ne/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/nl/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/nl/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/nl/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/nl/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/pl/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/pl/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/pl/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/pl/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/pt/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/pt/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/pt/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/pt/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/pt_BR/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/pt_BR/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/pt_BR/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/pt_BR/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/pt_PT/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/pt_PT/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/pt_PT/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/pt_PT/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ro/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/ro/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ro/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/ro/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ru/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/ru/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ru/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/ru/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/si/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/si/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/si/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/si/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/sk/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/sk/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/sk/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/sk/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/sl/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/sl/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/sl/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/sl/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/sphinxcontrib.devhelp.pot` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/sphinxcontrib.devhelp.pot`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/sr/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/sr/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/sr/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/sr/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/sr@latin/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/sr@latin/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/sr@latin/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/sr@latin/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/sv/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/sv/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/sv/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/sv/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ta/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/ta/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/ta/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/ta/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/tr/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/tr/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/tr/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/tr/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/uk_UA/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/uk_UA/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/uk_UA/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/uk_UA/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/vi/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/vi/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/vi/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/vi/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/zh_CN/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/zh_CN/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/zh_CN/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/zh_CN/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/zh_TW/LC_MESSAGES/sphinxcontrib.devhelp.mo` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/zh_TW/LC_MESSAGES/sphinxcontrib.devhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-devhelp-1.0.2/sphinxcontrib/devhelp/locales/zh_TW/LC_MESSAGES/sphinxcontrib.devhelp.po` & `sphinxcontrib_devhelp-1.0.3/sphinxcontrib/devhelp/locales/zh_TW/LC_MESSAGES/sphinxcontrib.devhelp.po`

 * *Files identical despite different names*

