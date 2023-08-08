# Comparing `tmp/sphinxcontrib-htmlhelp-2.0.1.tar.gz` & `tmp/sphinxcontrib_htmlhelp-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib-htmlhelp-2.0.1.tar", last modified: Tue Jan 31 17:28:48 2023, max compression
+gzip compressed data, was "sphinxcontrib_htmlhelp-2.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinxcontrib-htmlhelp-2.0.1.tar` & `sphinxcontrib_htmlhelp-2.0.2.tar`

### file list

```diff
@@ -1,258 +1,131 @@
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.709356 sphinxcontrib-htmlhelp-2.0.1/
--rw-rw-rw-   0        0        0      640 2023-01-31 17:28:20.000000 sphinxcontrib-htmlhelp-2.0.1/CHANGES
--rw-rw-rw-   0        0        0     1439 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/LICENSE
--rw-rw-rw-   0        0        0      199 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2559 2023-01-31 17:28:48.708350 sphinxcontrib-htmlhelp-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      855 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/README.rst
--rw-rw-rw-   0        0        0     1907 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-31 17:28:48.709356 sphinxcontrib-htmlhelp-2.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.483569 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.561066 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/
--rw-rw-rw-   0        0        0    12044 2023-01-31 17:28:20.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.562066 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.563066 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/.tx/
--rw-rw-rw-   0        0        0      224 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/.tx/config
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.486450 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ar/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.565066 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ar/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1025 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ar/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1576 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ar/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.488449 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/bg/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.567066 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/bg/LC_MESSAGES/
--rw-rw-rw-   0        0        0      506 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/bg/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1181 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/bg/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.490500 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/bn/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.570122 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/bn/LC_MESSAGES/
--rw-rw-rw-   0        0        0      504 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/bn/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1179 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/bn/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.491494 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ca/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.571066 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ca/LC_MESSAGES/
--rw-rw-rw-   0        0        0      504 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ca/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1179 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ca/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.492451 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/cak/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.574065 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/cak/LC_MESSAGES/
--rw-rw-rw-   0        0        0      466 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/cak/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1183 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/cak/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.493449 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/cs/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.576066 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/cs/LC_MESSAGES/
--rw-rw-rw-   0        0        0      582 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/cs/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1257 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/cs/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.495449 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/cy/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.577066 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/cy/LC_MESSAGES/
--rw-rw-rw-   0        0        0      547 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/cy/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1222 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/cy/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.496449 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/da/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.580065 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/da/LC_MESSAGES/
--rw-rw-rw-   0        0        0      894 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/da/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1439 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/da/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.497450 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/de/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.581066 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/de/LC_MESSAGES/
--rw-rw-rw-   0        0        0      503 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/de/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1178 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/de/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.499451 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/el/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.583064 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/el/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1050 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/el/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1614 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/el/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.500450 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/eo/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.585065 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/eo/LC_MESSAGES/
--rw-rw-rw-   0        0        0      506 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/eo/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1181 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/eo/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.501450 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/es/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.587065 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/es/LC_MESSAGES/
--rw-rw-rw-   0        0        0      962 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/es/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1591 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/es/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.502450 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/et/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.590081 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/et/LC_MESSAGES/
--rw-rw-rw-   0        0        0      866 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/et/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1448 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/et/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.503450 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/eu/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.592065 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/eu/LC_MESSAGES/
--rw-rw-rw-   0        0        0      503 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/eu/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1178 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/eu/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.504449 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/fa/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.594065 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/fa/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1036 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/fa/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1581 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/fa/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.506449 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/fi/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.596064 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/fi/LC_MESSAGES/
--rw-rw-rw-   0        0        0      504 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/fi/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1179 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/fi/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.507449 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/fr/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.599086 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0        0        0      994 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/fr/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1633 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/fr/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.508449 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/he/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.601065 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/he/LC_MESSAGES/
--rw-rw-rw-   0        0        0      597 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/he/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1272 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/he/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.509449 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/hi/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.603065 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/hi/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1313 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/hi/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1864 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/hi/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.509449 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/hi_IN/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.605066 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/hi_IN/LC_MESSAGES/
--rw-rw-rw-   0        0        0      516 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/hi_IN/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1191 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/hi_IN/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.511051 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/hr/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.606225 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/hr/LC_MESSAGES/
--rw-rw-rw-   0        0        0      577 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/hr/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1252 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/hr/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.512064 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/hu/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.609351 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/hu/LC_MESSAGES/
--rw-rw-rw-   0        0        0      943 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/hu/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1473 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/hu/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.513064 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/id/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.611349 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/id/LC_MESSAGES/
--rw-rw-rw-   0        0        0      929 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/id/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1510 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/id/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.514064 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/it/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.613350 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/it/LC_MESSAGES/
--rw-rw-rw-   0        0        0      504 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/it/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1179 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/it/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.516064 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ja/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.616351 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ja/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1004 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ja/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1561 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ja/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.517064 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ko/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.618351 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ko/LC_MESSAGES/
--rw-rw-rw-   0        0        0      942 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ko/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1475 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ko/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.518065 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/lt/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.620351 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/lt/LC_MESSAGES/
--rw-rw-rw-   0        0        0      638 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/lt/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1313 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/lt/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.519065 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/lv/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.622352 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/lv/LC_MESSAGES/
--rw-rw-rw-   0        0        0      539 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/lv/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1214 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/lv/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.520064 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/mk/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.624349 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/mk/LC_MESSAGES/
--rw-rw-rw-   0        0        0      537 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/mk/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1212 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/mk/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.522064 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/nb_NO/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.626349 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/nb_NO/LC_MESSAGES/
--rw-rw-rw-   0        0        0      529 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/nb_NO/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1204 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/nb_NO/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.523064 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ne/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.628350 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ne/LC_MESSAGES/
--rw-rw-rw-   0        0        0      503 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ne/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1178 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ne/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.524065 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/nl/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.630350 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0      502 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/nl/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1177 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/nl/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.525064 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/pl/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.632349 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/pl/LC_MESSAGES/
--rw-rw-rw-   0        0        0      649 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/pl/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1324 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/pl/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.526064 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/pt/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.635351 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/pt/LC_MESSAGES/
--rw-rw-rw-   0        0        0      507 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/pt/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1182 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/pt/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.528065 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/pt_BR/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.636350 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/pt_BR/LC_MESSAGES/
--rw-rw-rw-   0        0        0      973 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/pt_BR/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1534 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/pt_BR/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.530065 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/pt_PT/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.638351 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/pt_PT/LC_MESSAGES/
--rw-rw-rw-   0        0        0      524 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/pt_PT/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1199 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/pt_PT/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.531064 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ro/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.640352 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ro/LC_MESSAGES/
--rw-rw-rw-   0        0        0      546 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ro/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1221 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ro/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.532064 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ru/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.642350 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ru/LC_MESSAGES/
--rw-rw-rw-   0        0        0      642 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ru/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1317 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ru/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.533064 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/si/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.644351 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/si/LC_MESSAGES/
--rw-rw-rw-   0        0        0      504 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/si/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1179 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/si/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.534064 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sk/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.646351 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sk/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1009 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sk/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1547 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sk/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.536064 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sl/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.648350 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sl/LC_MESSAGES/
--rw-rw-rw-   0        0        0      558 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sl/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1233 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sl/LC_MESSAGES/sphinxcontrib.htmlhelp.po
--rw-rw-rw-   0        0        0     1120 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sphinxcontrib.htmlhelp.pot
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.537064 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sq/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.650351 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sq/LC_MESSAGES/
--rw-rw-rw-   0        0        0      953 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sq/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1508 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sq/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.538064 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sr/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.654349 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sr/LC_MESSAGES/
--rw-rw-rw-   0        0        0      578 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sr/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1253 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sr/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.538064 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sr@latin/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.652349 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sr@latin/LC_MESSAGES/
--rw-rw-rw-   0        0        0      598 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sr@latin/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1273 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sr@latin/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.540064 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sr_RS/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.656350 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sr_RS/LC_MESSAGES/
--rw-rw-rw-   0        0        0      593 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sr_RS/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1268 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sr_RS/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.540064 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sv/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.658349 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sv/LC_MESSAGES/
--rw-rw-rw-   0        0        0      504 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sv/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1179 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sv/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.542065 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ta/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.661350 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ta/LC_MESSAGES/
--rw-rw-rw-   0        0        0      502 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ta/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1177 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ta/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.542065 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/te/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.663350 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/te/LC_MESSAGES/
--rw-rw-rw-   0        0        0      503 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/te/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1178 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/te/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.543064 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/tr/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.665349 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/tr/LC_MESSAGES/
--rw-rw-rw-   0        0        0      939 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/tr/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1465 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/tr/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.545064 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/uk_UA/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.667350 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/uk_UA/LC_MESSAGES/
--rw-rw-rw-   0        0        0      744 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/uk_UA/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1419 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/uk_UA/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.546064 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ur/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.669350 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ur/LC_MESSAGES/
--rw-rw-rw-   0        0        0      501 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ur/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1176 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ur/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.547063 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/vi/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.670351 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/vi/LC_MESSAGES/
--rw-rw-rw-   0        0        0      500 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/vi/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1175 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/vi/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.548064 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/zh_CN/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.673350 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/zh_CN/LC_MESSAGES/
--rw-rw-rw-   0        0        0      917 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/zh_CN/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1498 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/zh_CN/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.549064 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/zh_TW/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.674350 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/zh_TW/LC_MESSAGES/
--rw-rw-rw-   0        0        0      512 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/zh_TW/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
--rw-rw-rw-   0        0        0     1187 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/zh_TW/LC_MESSAGES/sphinxcontrib.htmlhelp.po
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.677352 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/templates/
--rw-rw-rw-   0        0        0      729 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/templates/project.hhc
--rw-rw-rw-   0        0        0     1627 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/templates/project.hhp
--rw-rw-rw-   0        0        0      165 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/templates/project.stp
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.696351 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib_htmlhelp.egg-info/
--rw-rw-rw-   0        0        0     2559 2023-01-31 17:28:48.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib_htmlhelp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8710 2023-01-31 17:28:48.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib_htmlhelp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-31 17:28:48.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib_htmlhelp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-01-31 17:28:48.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib_htmlhelp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-01-31 17:28:48.000000 sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib_htmlhelp.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.698349 sphinxcontrib-htmlhelp-2.0.1/tests/
--rw-rw-rw-   0        0        0      402 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.552066 sphinxcontrib-htmlhelp-2.0.1/tests/roots/
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.700350 sphinxcontrib-htmlhelp-2.0.1/tests/roots/test-basic/
--rw-rw-rw-   0        0        0        0 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/tests/roots/test-basic/conf.py
--rw-rw-rw-   0        0        0       22 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/tests/roots/test-basic/index.rst
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.702350 sphinxcontrib-htmlhelp-2.0.1/tests/roots/test-chm/
--rw-rw-rw-   0        0        0       17 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/tests/roots/test-chm/conf.py
--rw-rw-rw-   0        0        0      376 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/tests/roots/test-chm/index.rst
-drwxrwxrwx   0        0        0        0 2023-01-31 17:28:48.707349 sphinxcontrib-htmlhelp-2.0.1/tests/roots/test-hhc/
--rw-rw-rw-   0        0        0        8 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/tests/roots/test-hhc/bar.rst
--rw-rw-rw-   0        0        0        8 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/tests/roots/test-hhc/baz.rst
--rw-rw-rw-   0        0        0       44 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/tests/roots/test-hhc/conf.py
--rw-rw-rw-   0        0        0       30 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/tests/roots/test-hhc/foo.rst
--rw-rw-rw-   0        0        0      150 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/tests/roots/test-hhc/index.rst
--rw-rw-rw-   0        0        0     4460 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/tests/test_htmlhelp.py
--rw-rw-rw-   0        0        0      752 2023-01-31 17:28:14.000000 sphinxcontrib-htmlhelp-2.0.1/tox.ini
+-rw-r--r--   0        0        0      773 2023-08-08 18:58:50.124389 sphinxcontrib_htmlhelp-2.0.2/CHANGES
+-rw-r--r--   0        0        0     1439 2023-08-08 18:58:50.124389 sphinxcontrib_htmlhelp-2.0.2/LICENSE
+-rw-r--r--   0        0        0      419 2023-08-08 18:58:50.124389 sphinxcontrib_htmlhelp-2.0.2/README.rst
+-rw-r--r--   0        0        0     2000 2023-08-08 18:58:50.124389 sphinxcontrib_htmlhelp-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0    11675 2023-08-08 18:58:50.124389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/__init__.py
+-rw-r--r--   0        0        0      224 2023-08-08 18:58:50.124389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/.tx/config
+-rw-r--r--   0        0        0     1025 2023-08-08 18:58:50.124389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/ar/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1576 2023-08-08 18:58:50.124389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/ar/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      506 2023-08-08 18:58:50.124389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/bg/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1181 2023-08-08 18:58:50.124389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/bg/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      504 2023-08-08 18:58:50.124389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/bn/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1179 2023-08-08 18:58:50.124389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/bn/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      504 2023-08-08 18:58:50.124389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/ca/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1179 2023-08-08 18:58:50.124389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/ca/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      466 2023-08-08 18:58:50.124389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/cak/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1183 2023-08-08 18:58:50.124389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/cak/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      582 2023-08-08 18:58:50.124389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/cs/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1257 2023-08-08 18:58:50.124389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/cs/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      547 2023-08-08 18:58:50.124389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/cy/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1222 2023-08-08 18:58:50.124389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/cy/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      894 2023-08-08 18:58:50.124389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/da/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1439 2023-08-08 18:58:50.124389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/da/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      503 2023-08-08 18:58:50.124389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/de/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1178 2023-08-08 18:58:50.124389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/de/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0     1050 2023-08-08 18:58:50.124389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/el/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1614 2023-08-08 18:58:50.124389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/el/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      506 2023-08-08 18:58:50.124389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/eo/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1181 2023-08-08 18:58:50.124389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/eo/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      962 2023-08-08 18:58:50.124389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/es/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1591 2023-08-08 18:58:50.124389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/es/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      866 2023-08-08 18:58:50.124389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/et/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1448 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/et/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      503 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/eu/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1178 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/eu/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0     1036 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/fa/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1581 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/fa/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      504 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/fi/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1179 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/fi/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      994 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/fr/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1633 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/fr/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      597 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/he/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1272 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/he/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0     1313 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/hi/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1864 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/hi/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      516 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/hi_IN/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1191 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/hi_IN/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      577 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/hr/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1252 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/hr/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      943 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/hu/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1473 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/hu/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      929 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/id/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1510 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/id/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      504 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/it/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1179 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/it/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0     1004 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/ja/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1561 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/ja/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      942 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/ko/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1475 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/ko/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      638 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/lt/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1313 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/lt/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      539 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/lv/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1214 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/lv/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      537 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/mk/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1212 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/mk/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      529 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/nb_NO/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1204 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/nb_NO/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      503 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/ne/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1178 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/ne/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      502 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/nl/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1177 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/nl/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      649 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/pl/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1324 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/pl/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      507 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/pt/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1182 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/pt/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      973 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/pt_BR/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1534 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/pt_BR/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      524 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/pt_PT/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1199 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/pt_PT/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      546 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/ro/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1221 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/ro/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      642 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/ru/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1317 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/ru/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      504 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/si/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1179 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/si/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0     1009 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/sk/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1547 2023-08-08 18:58:50.128389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/sk/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      558 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/sl/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1233 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/sl/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0     1120 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/sphinxcontrib.htmlhelp.pot
+-rw-r--r--   0        0        0      953 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/sq/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1508 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/sq/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      578 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/sr/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1253 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/sr/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      598 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/sr@latin/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1273 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/sr@latin/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      593 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/sr_RS/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1268 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/sr_RS/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      504 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/sv/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1179 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/sv/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      502 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/ta/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1177 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/ta/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      503 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/te/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1178 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/te/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      939 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/tr/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1465 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/tr/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      744 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/uk_UA/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1419 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/uk_UA/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      501 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/ur/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1176 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/ur/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      500 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/vi/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1175 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/vi/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      917 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/zh_CN/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1498 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/zh_CN/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      512 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/zh_TW/LC_MESSAGES/sphinxcontrib.htmlhelp.mo
+-rw-r--r--   0        0        0     1187 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/zh_TW/LC_MESSAGES/sphinxcontrib.htmlhelp.po
+-rw-r--r--   0        0        0      729 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/templates/project.hhc
+-rw-r--r--   0        0        0     1627 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/templates/project.hhp
+-rw-r--r--   0        0        0      165 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/templates/project.stp
+-rw-r--r--   0        0        0      187 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/tests/roots/test-basic/conf.py
+-rw-r--r--   0        0        0       22 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/tests/roots/test-basic/index.rst
+-rw-r--r--   0        0        0       17 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/tests/roots/test-chm/conf.py
+-rw-r--r--   0        0        0      376 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/tests/roots/test-chm/index.rst
+-rw-r--r--   0        0        0        8 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/tests/roots/test-hhc/bar.rst
+-rw-r--r--   0        0        0        8 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/tests/roots/test-hhc/baz.rst
+-rw-r--r--   0        0        0       44 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/tests/roots/test-hhc/conf.py
+-rw-r--r--   0        0        0       30 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/tests/roots/test-hhc/foo.rst
+-rw-r--r--   0        0        0      150 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/tests/roots/test-hhc/index.rst
+-rw-r--r--   0        0        0     4271 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/tests/test_htmlhelp.py
+-rw-r--r--   0        0        0      778 2023-08-08 18:58:50.132389 sphinxcontrib_htmlhelp-2.0.2/tox.ini
+-rw-r--r--   0        0        0     2238 1970-01-01 00:00:00.000000 sphinxcontrib_htmlhelp-2.0.2/PKG-INFO
```

### Comparing `sphinxcontrib-htmlhelp-2.0.1/CHANGES` & `sphinxcontrib_htmlhelp-2.0.2/CHANGES`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Release 2.0.2 (2023-08-07)
+==========================
+
+* Drop support for Python 3.8
+* Raise minimum required Sphinx version to 5.0
+
 Release 2.0.1 (2023-01-31)
 ==========================
 
 * Drop support for Python 3.7 and lower
 * Fix deprecation warnings from Sphinx 6.1
 
 Release 2.0.0 (2021-05-23)
```

### Comparing `sphinxcontrib-htmlhelp-2.0.1/LICENSE` & `sphinxcontrib_htmlhelp-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/pyproject.toml` & `sphinxcontrib_htmlhelp-2.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 [build-system]
-requires = ["setuptools>=64"]
-build-backend = "setuptools.build_meta"
+requires = ["flit_core>=3.7"]
+build-backend = "flit_core.buildapi"
 
 # project metadata
 [project]
 name = "sphinxcontrib-htmlhelp"
 description = "sphinxcontrib-htmlhelp is a sphinx extension which renders HTML help files"
 readme = "README.rst"
 urls.Changelog = "https://www.sphinx-doc.org/en/master/changes.html"
 urls.Code = "https://github.com/sphinx-doc/sphinxcontrib-htmlhelp"
 urls.Download = "https://pypi.org/project/sphinxcontrib-htmlhelp/"
 urls.Homepage = "https://www.sphinx-doc.org/"
 urls."Issue tracker" = "https://github.com/sphinx-doc/sphinx/issues"
 license.text = "BSD-2-Clause"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 
 # Classifiers list: https://pypi.org/classifiers/
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3.13",
     "Framework :: Sphinx",
     "Framework :: Sphinx :: Extension",
     "Topic :: Documentation",
     "Topic :: Documentation :: Sphinx",
     "Topic :: Text Processing",
     "Topic :: Utilities",
 ]
-dependencies = []
+dependencies = [
+    "Sphinx>=5",
+]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "html5lib",
 ]
@@ -53,12 +55,21 @@
     "docutils-stubs",
 ]
 
 [[project.authors]]
 name = "Georg Brandl"
 email = "georg@python.org"
 
-[tool.setuptools.dynamic]
-version.attr = "sphinxcontrib.htmlhelp.__version__"
+[tool.flit.module]
+name = "sphinxcontrib.htmlhelp"
+
+[tool.flit.sdist]
+include = [
+    "CHANGES",
+    "LICENSE",
+    # Tests
+    "tests/",
+    "tox.ini",
+]
 
 [tool.mypy]
 ignore_missing_imports = true
```

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/__init__.py` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,16 @@
-"""
-    sphinxcontrib.htmlhelp
-    ~~~~~~~~~~~~~~~~~~~~~~
-
-    Build HTML help support files.
-
-    :copyright: Copyright 2007-2019 by the Sphinx team, see README.
-    :license: BSD, see LICENSE for details.
-"""
+"""Build HTML help support files."""
+
+from __future__ import annotations
 
 import html
 import os
 from os import path
-from typing import Any, Dict, List, Set, Tuple, Type
+from pathlib import Path
+from typing import Any
 
 from docutils import nodes
 from docutils.nodes import Element, Node, document
 
 import sphinx
 from sphinx import addnodes
 from sphinx.application import Sphinx
@@ -24,23 +19,22 @@
 from sphinx.environment.adapters.indexentries import IndexEntries
 from sphinx.locale import get_translation
 from sphinx.util import logging
 from sphinx.util.fileutil import copy_asset_file
 from sphinx.util.nodes import NodeMatcher
 from sphinx.util.osutil import make_filename_from_project, relpath
 from sphinx.util.template import SphinxRenderer
-from sphinx.writers.html import HTMLTranslator
 
 if sphinx.version_info[:2] >= (6, 1):
     from sphinx.util.display import progress_message
 else:
     from sphinx.util import progress_message  # type: ignore[attr-defined,no-redef]
 
-__version__ = '2.0.1'
-__version_info__ = (2, 0, 1)
+__version__ = '2.0.2'
+__version_info__ = (2, 0, 2)
 
 logger = logging.getLogger(__name__)
 __ = get_translation(__name__, 'console')
 
 package_dir = path.abspath(path.dirname(__file__))
 template_dir = path.join(package_dir, 'templates')
 
@@ -94,15 +88,15 @@
     s = s.replace('&#x27;', '&#39;')    # re-escape as decimal
     return s
 
 
 class ToCTreeVisitor(nodes.NodeVisitor):
     def __init__(self, document: document) -> None:
         super().__init__(document)
-        self.body = []  # type: List[str]
+        self.body: list[str] = []
         self.depth = 0
 
     def append(self, text: str) -> None:
         self.body.append(text)
 
     def astext(self) -> str:
         return '\n'.join(self.body)
@@ -169,24 +163,19 @@
         self.link_suffix = '.html'
         super().init()
         # determine the correct locale setting
         locale = chm_locales.get(self.config.language)
         if locale is not None:
             self.lcid, self.encoding = locale
 
-    @property
-    def default_translator_class(self) -> "Type[nodes.NodeVisitor]":  # type: ignore
-        # Use HTML4 writer always
-        return HTMLTranslator
-
-    def prepare_writing(self, docnames: Set[str]) -> None:
+    def prepare_writing(self, docnames: set[str]) -> None:
         super().prepare_writing(docnames)
         self.globalcontext['html5_doctype'] = False
 
-    def update_page_context(self, pagename: str, templatename: str, ctx: Dict, event_arg: str) -> None:  # NOQA
+    def update_page_context(self, pagename: str, templatename: str, ctx: dict, event_arg: str) -> None:  # NOQA
         ctx['encoding'] = self.encoding
 
     def handle_finish(self) -> None:
         self.copy_stopword_list()
         self.build_project_file()
         self.build_toc_file()
         self.build_hhx(self.outdir, self.config.htmlhelp_basename)
@@ -195,15 +184,15 @@
         for node in doctree.traverse(nodes.reference):
             # add ``target=_blank`` attributes to external links
             if node.get('internal') is None and 'refuri' in node:
                 node['target'] = '_blank'
 
         super().write_doc(docname, doctree)
 
-    def render(self, name: str, context: Dict) -> str:
+    def render(self, name: str, context: dict) -> str:
         template = SphinxRenderer(template_dir)
         return template.render(name, context)
 
     @progress_message(__('copying stopword list'))
     def copy_stopword_list(self) -> None:
         """Copy a stopword list (.stp) to outdir.
 
@@ -218,15 +207,15 @@
         filename = path.join(self.outdir, self.config.htmlhelp_basename + '.stp')
         copy_asset_file(template, filename)
 
     @progress_message(__('writing project file'))
     def build_project_file(self) -> None:
         """Create a project file (.hhp) on outdir."""
         # scan project files
-        project_files = []  # type: List[str]
+        project_files: list[str] = []
         for root, dirs, files in os.walk(self.outdir):
             dirs.sort()
             files.sort()
             in_staticdir = root.startswith(path.join(self.outdir, '_static'))
             for fn in sorted(files):
                 if (in_staticdir and not fn.endswith('.js')) or fn.endswith('.html'):
                     fn = relpath(path.join(root, fn), self.outdir)
@@ -263,22 +252,22 @@
                 'suffix': self.out_suffix,
                 'short_title': self.config.html_short_title,
                 'master_doc': self.config.master_doc,
                 'domain_indices': self.domain_indices,
             }
             f.write(self.render('project.hhc', context))
 
-    def build_hhx(self, outdir: str, outname: str) -> None:
+    def build_hhx(self, outdir: Path, outname: str) -> None:
         logger.info(__('writing index file...'))
         index = IndexEntries(self.env).create_index(self)
         filename = path.join(outdir, outname + '.hhk')
         with open(filename, 'w', encoding=self.encoding, errors='xmlcharrefreplace') as f:
             f.write('<UL>\n')
 
-            def write_index(title: str, refs: List[Tuple[str, str]], subitems: List[Tuple[str, List[Tuple[str, str]]]]) -> None:  # NOQA
+            def write_index(title: str, refs: list[tuple[str, str]], subitems: list[tuple[str, list[tuple[str, str]]]]) -> None:  # NOQA
                 def write_param(name: str, value: str) -> None:
                     item = '    <param name="%s" value="%s">\n' % (name, value)
                     f.write(item)
                 title = chm_htmlescape(title, True)
                 f.write('<LI> <OBJECT type="text/sitemap">\n')
                 write_param('Keyword', title)
                 if len(refs) == 0:
@@ -303,15 +292,15 @@
 
 
 def default_htmlhelp_basename(config: Config) -> str:
     """Better default htmlhelp_basename setting."""
     return make_filename_from_project(config.project) + 'doc'
 
 
-def setup(app: Sphinx) -> Dict[str, Any]:
+def setup(app: Sphinx) -> dict[str, Any]:
     app.setup_extension('sphinx.builders.html')
     app.add_builder(HTMLHelpBuilder)
     app.add_message_catalog(__name__, path.join(package_dir, 'locales'))
 
     app.add_config_value('htmlhelp_basename', default_htmlhelp_basename, '')
     app.add_config_value('htmlhelp_file_suffix', None, 'html', [str])
     app.add_config_value('htmlhelp_link_suffix', None, 'html', [str])
```

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ar/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/ar/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ar/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/ar/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/bg/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/bg/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/bn/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/bn/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ca/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/ca/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/cak/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/cak/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/cs/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/cs/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/cs/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/cs/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/cy/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/cy/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/cy/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/cy/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/da/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/da/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/da/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/da/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/de/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/de/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/el/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/el/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/el/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/el/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/eo/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/eo/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/es/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/es/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/es/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/es/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/et/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/et/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/et/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/et/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/eu/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/eu/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/fa/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/fa/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/fa/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/fa/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/fi/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/fi/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/fr/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/fr/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/fr/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/fr/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/he/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/he/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/he/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/he/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/hi/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/hi/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/hi/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/hi/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/hi_IN/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/hi_IN/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/hi_IN/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/hi_IN/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/hr/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/hr/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/hr/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/hr/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/hu/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/hu/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/hu/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/hu/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/id/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/id/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/id/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/id/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/it/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/it/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ja/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/ja/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ja/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/ja/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ko/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/ko/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ko/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/ko/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/lt/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/lt/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/lt/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/lt/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/lv/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/lv/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/lv/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/lv/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/mk/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/mk/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/mk/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/mk/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/nb_NO/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/nb_NO/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/nb_NO/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/nb_NO/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ne/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/ne/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/nl/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/nl/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/pl/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/pl/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/pl/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/pl/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/pt/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/pt/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/pt_BR/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/pt_BR/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/pt_BR/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/pt_BR/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/pt_PT/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/pt_PT/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/pt_PT/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/pt_PT/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ro/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/ro/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ro/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/ro/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ru/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/ru/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ru/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/ru/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/si/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/si/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sk/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/sk/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sk/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/sk/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sl/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/sl/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sl/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/sl/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sphinxcontrib.htmlhelp.pot` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/sphinxcontrib.htmlhelp.pot`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sq/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/sq/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sq/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/sq/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sr/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/sr/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sr/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/sr/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sr@latin/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/sr@latin/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sr@latin/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/sr@latin/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sr_RS/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/sr_RS/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sr_RS/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/sr_RS/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/sv/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/sv/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ta/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/ta/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/te/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/te/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/tr/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/tr/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/tr/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/tr/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/uk_UA/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/uk_UA/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/uk_UA/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/uk_UA/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/ur/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/ur/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/vi/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/vi/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/zh_CN/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/zh_CN/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/zh_CN/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/zh_CN/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/zh_TW/LC_MESSAGES/sphinxcontrib.htmlhelp.mo` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/zh_TW/LC_MESSAGES/sphinxcontrib.htmlhelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/locales/zh_TW/LC_MESSAGES/sphinxcontrib.htmlhelp.po` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/locales/zh_TW/LC_MESSAGES/sphinxcontrib.htmlhelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/templates/project.hhc` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/templates/project.hhc`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/sphinxcontrib/htmlhelp/templates/project.hhp` & `sphinxcontrib_htmlhelp-2.0.2/sphinxcontrib/htmlhelp/templates/project.hhp`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-htmlhelp-2.0.1/tests/test_htmlhelp.py` & `sphinxcontrib_htmlhelp-2.0.2/tests/test_htmlhelp.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,8 @@
-"""
-    test_build_htmlhelp
-    ~~~~~~~~~~~~~~~~~~~
-
-    Test the HTML Help builder and check output against XPath.
-
-    :copyright: Copyright 2007-2019 by the Sphinx team, see AUTHORS.
-    :license: BSD, see LICENSE for details.
-"""
+"""Test the HTML Help builder and check output against XPath."""
 
 import re
 
 import pytest
 from html5lib import HTMLParser
 
 from sphinxcontrib.htmlhelp import chm_htmlescape, default_htmlhelp_basename
@@ -59,18 +51,16 @@
 
 @pytest.mark.sphinx('htmlhelp', testroot='chm')
 def test_chm(app):
     app.build()
 
     # check .hhk file
     outname = app.builder.config.htmlhelp_basename
-    hhk_path = str(app.outdir / outname + '.hhk')
-
-    with open(hhk_path, 'rb') as f:
-        data = f.read()
+    hhk_path = (app.outdir / outname).with_suffix('.hhk')
+    data = hhk_path.read_bytes()
     m = re.search(br'&#[xX][0-9a-fA-F]+;', data)
     assert m is None, 'Hex escaping exists in .hhk file: ' + str(m.group(0))
 
 
 @pytest.mark.sphinx('htmlhelp', testroot='hhc')
 def test_htmlhelp_hhc(app):
     app.build()
```

### Comparing `sphinxcontrib-htmlhelp-2.0.1/tox.ini` & `sphinxcontrib_htmlhelp-2.0.2/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tox]
 minversion = 2.4.0
 envlist =
-    py{38,39,310,311,312},
+    py{39,310,311,312,313},
     flake8,
     mypy
 isolated_build = True
 
 [testenv]
 usedevelop = True
 passenv =
@@ -38,8 +38,8 @@
 
 [testenv:mypy]
 description =
     Run type checks.
 extras =
     lint
 commands=
-    mypy sphinxcontrib/
+    mypy sphinxcontrib/ --explicit-package-bases
```

