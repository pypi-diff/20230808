# Comparing `tmp/sphinxcontrib-applehelp-1.0.4.tar.gz` & `tmp/sphinxcontrib_applehelp-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib-applehelp-1.0.4.tar", last modified: Mon Jan 23 09:40:54 2023, max compression
+gzip compressed data, was "sphinxcontrib_applehelp-1.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinxcontrib-applehelp-1.0.4.tar` & `sphinxcontrib_applehelp-1.0.5.tar`

### file list

```diff
@@ -1,231 +1,114 @@
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.456769 sphinxcontrib-applehelp-1.0.4/
--rw-rw-rw-   0        0        0      516 2023-01-23 09:19:44.000000 sphinxcontrib-applehelp-1.0.4/CHANGES
--rw-rw-rw-   0        0        0     1441 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      201 2023-01-23 09:32:13.000000 sphinxcontrib-applehelp-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2571 2023-01-23 09:40:54.454765 sphinxcontrib-applehelp-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      862 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/README.rst
--rw-rw-rw-   0        0        0     1897 2023-01-23 09:37:42.000000 sphinxcontrib-applehelp-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-23 09:40:54.456769 sphinxcontrib-applehelp-1.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.253540 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.301539 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/
--rw-rw-rw-   0        0        0    10985 2023-01-23 09:40:19.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.302541 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.303538 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/.tx/
--rw-rw-rw-   0        0        0      227 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/.tx/config
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.255538 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ar/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.304539 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ar/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1881 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ar/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2338 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ar/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.256539 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/bn/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.306540 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/bn/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1799 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/bn/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2256 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/bn/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.256539 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ca/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.308539 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ca/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1799 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ca/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2256 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ca/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.257538 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/cak/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.310540 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/cak/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1761 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/cak/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2260 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/cak/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.258539 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/cs/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.312540 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/cs/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1877 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/cs/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2334 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/cs/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.259539 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/cy/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.314539 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/cy/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1842 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/cy/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2299 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/cy/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.262552 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/da/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.316540 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/da/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1798 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/da/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2255 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/da/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.263539 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/de/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.318540 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/de/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1798 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/de/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2255 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/de/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.263539 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/el/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.320540 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/el/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1797 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/el/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2254 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/el/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.264539 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/eo/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.322540 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/eo/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1801 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/eo/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2258 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/eo/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.265539 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/es/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.324540 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/es/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1825 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/es/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2445 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/es/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.265539 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/et/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.326540 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/et/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1827 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/et/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2450 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/et/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.266538 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/eu/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.328540 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/eu/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1798 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/eu/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2255 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/eu/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.267546 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/fa/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.330540 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/fa/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1798 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/fa/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2255 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/fa/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.268539 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/fi/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.332539 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/fi/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1799 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/fi/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2256 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/fi/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.269539 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/fr/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.333539 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/fr/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1910 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/fr/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2879 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/fr/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.270538 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/he/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.335539 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/he/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1892 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/he/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2349 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/he/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.270538 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/hi/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.351769 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/hi/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1797 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/hi/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2254 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/hi/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.271539 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/hi_IN/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.353765 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/hi_IN/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1811 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/hi_IN/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2268 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/hi_IN/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.271539 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/hr/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.355764 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/hr/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1872 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/hr/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2329 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/hr/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.272538 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/hu/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.357765 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/hu/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1801 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/hu/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2258 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/hu/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.273538 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/id/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.360765 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/id/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1856 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/id/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2850 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/id/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.274538 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/it/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.364779 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/it/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1799 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/it/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2256 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/it/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.274538 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ja/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.366764 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ja/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1793 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ja/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2250 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ja/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.275539 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ko/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.368765 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ko/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1992 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ko/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     3071 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ko/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.276538 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/lt/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.370764 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/lt/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1933 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/lt/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2390 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/lt/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.276538 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/lv/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.372766 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/lv/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1834 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/lv/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2291 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/lv/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.277538 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/mk/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.374765 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/mk/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1832 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/mk/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2289 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/mk/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.278539 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/nb_NO/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.376765 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/nb_NO/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1824 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/nb_NO/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2281 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/nb_NO/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.278539 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ne/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.378764 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ne/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1798 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ne/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2255 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ne/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.279538 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/nl/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.380766 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/nl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1797 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/nl/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2254 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/nl/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.280538 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/pl/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.382765 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/pl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1966 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/pl/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2579 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/pl/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.280538 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/pt/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.384764 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/pt/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1802 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/pt/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2259 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/pt/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.281538 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/pt_BR/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.386765 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/pt_BR/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1816 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/pt_BR/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2273 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/pt_BR/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.282540 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/pt_PT/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.388764 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/pt_PT/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1819 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/pt_PT/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2276 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/pt_PT/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.283538 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ro/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.390766 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ro/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1841 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ro/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2298 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ro/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.283538 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ru/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.392764 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ru/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1937 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ru/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2394 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ru/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.284538 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/si/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.394765 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/si/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1799 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/si/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2256 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/si/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.284538 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/sk/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.396764 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/sk/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1873 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/sk/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2330 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/sk/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.285539 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/sl/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.398763 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/sl/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1853 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/sl/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2310 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/sl/LC_MESSAGES/sphinxcontrib.applehelp.po
--rw-rw-rw-   0        0        0     2200 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/sphinxcontrib.applehelp.pot
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.287540 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/sr/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.402764 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/sr/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1873 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/sr/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2330 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/sr/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.286539 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/sr@latin/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.400765 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/sr@latin/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1895 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/sr@latin/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2352 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/sr@latin/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.288539 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/sv/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.404765 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/sv/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1799 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/sv/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2256 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/sv/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.289539 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ta/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.406764 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ta/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1797 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ta/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2254 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ta/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.289539 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/tr/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.408764 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/tr/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1798 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/tr/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2255 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/tr/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.290539 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/uk_UA/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.410764 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/uk_UA/LC_MESSAGES/
--rw-rw-rw-   0        0        0     2039 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/uk_UA/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2496 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/uk_UA/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.291538 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ur/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.418764 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ur/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1796 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ur/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2253 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ur/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.291538 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/vi/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.421764 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/vi/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1795 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/vi/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2252 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/vi/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.292538 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/zh_CN/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.423764 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/zh_CN/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1817 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/zh_CN/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2824 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/zh_CN/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.292538 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/zh_TW/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.426765 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/zh_TW/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1807 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/zh_TW/LC_MESSAGES/sphinxcontrib.applehelp.mo
--rw-rw-rw-   0        0        0     2264 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/zh_TW/LC_MESSAGES/sphinxcontrib.applehelp.po
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.427768 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/templates/
--rw-rw-rw-   0        0        0      403 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/templates/_access.html_t
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.446776 sphinxcontrib-applehelp-1.0.4/sphinxcontrib_applehelp.egg-info/
--rw-rw-rw-   0        0        0     2571 2023-01-23 09:40:54.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib_applehelp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8045 2023-01-23 09:40:54.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib_applehelp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-23 09:40:54.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib_applehelp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-01-23 09:40:54.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib_applehelp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-01-23 09:40:54.000000 sphinxcontrib-applehelp-1.0.4/sphinxcontrib_applehelp.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.449769 sphinxcontrib-applehelp-1.0.4/tests/
--rw-rw-rw-   0        0        0      402 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.294538 sphinxcontrib-applehelp-1.0.4/tests/roots/
-drwxrwxrwx   0        0        0        0 2023-01-23 09:40:54.453768 sphinxcontrib-applehelp-1.0.4/tests/roots/test-basic/
--rw-rw-rw-   0        0        0        0 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/tests/roots/test-basic/conf.py
--rw-rw-rw-   0        0        0       22 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/tests/roots/test-basic/index.rst
--rw-rw-rw-   0        0        0     1558 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/tests/test_applehelp.py
--rw-rw-rw-   0        0        0      750 2023-01-08 00:07:17.000000 sphinxcontrib-applehelp-1.0.4/tox.ini
+-rw-r--r--   0        0        0      649 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/CHANGES
+-rw-r--r--   0        0        0     1441 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/LICENSE
+-rw-r--r--   0        0        0      425 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/README.rst
+-rw-r--r--   0        0        0     2022 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0    10691 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/__init__.py
+-rw-r--r--   0        0        0      227 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/.tx/config
+-rw-r--r--   0        0        0     1881 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ar/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2338 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ar/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1799 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/bn/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2256 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/bn/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1799 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ca/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2256 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ca/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1761 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/cak/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2260 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/cak/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1877 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/cs/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2334 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/cs/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1842 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/cy/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2299 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/cy/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1798 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/da/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2255 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/da/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1798 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/de/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2255 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/de/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1797 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/el/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2254 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/el/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1801 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/eo/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2258 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/eo/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1825 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/es/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2445 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/es/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1827 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/et/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2450 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/et/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1798 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/eu/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2255 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/eu/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1798 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/fa/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2255 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/fa/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1799 2023-08-08 18:58:33.724122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/fi/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2256 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/fi/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1910 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/fr/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2879 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/fr/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1892 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/he/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2349 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/he/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1797 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/hi/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2254 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/hi/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1811 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/hi_IN/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2268 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/hi_IN/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1872 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/hr/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2329 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/hr/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1801 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/hu/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2258 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/hu/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1856 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/id/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2850 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/id/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1799 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/it/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2256 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/it/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1793 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ja/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2250 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ja/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1992 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ko/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     3071 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ko/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1933 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/lt/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2390 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/lt/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1834 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/lv/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2291 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/lv/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1832 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/mk/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2289 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/mk/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1824 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/nb_NO/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2281 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/nb_NO/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1798 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ne/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2255 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ne/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1797 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/nl/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2254 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/nl/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1966 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/pl/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2579 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/pl/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1802 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/pt/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2259 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/pt/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1816 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/pt_BR/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2273 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/pt_BR/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1819 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/pt_PT/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2276 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/pt_PT/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1841 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ro/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2298 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ro/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1937 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ru/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2394 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ru/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1799 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/si/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2256 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/si/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1873 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/sk/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2330 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/sk/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1853 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/sl/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2310 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/sl/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     2200 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/sphinxcontrib.applehelp.pot
+-rw-r--r--   0        0        0     1873 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/sr/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2330 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/sr/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1895 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/sr@latin/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2352 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/sr@latin/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1799 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/sv/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2256 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/sv/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1797 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ta/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2254 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ta/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1798 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/tr/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2255 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/tr/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     2039 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/uk_UA/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2496 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/uk_UA/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1796 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ur/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2253 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ur/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1795 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/vi/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2252 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/vi/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1817 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/zh_CN/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2824 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/zh_CN/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0     1807 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/zh_TW/LC_MESSAGES/sphinxcontrib.applehelp.mo
+-rw-r--r--   0        0        0     2264 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/zh_TW/LC_MESSAGES/sphinxcontrib.applehelp.po
+-rw-r--r--   0        0        0      403 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/templates/_access.html_t
+-rw-r--r--   0        0        0      187 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/tests/roots/test-basic/conf.py
+-rw-r--r--   0        0        0       22 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/tests/roots/test-basic/index.rst
+-rw-r--r--   0        0        0     1415 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/tests/test_applehelp.py
+-rw-r--r--   0        0        0      776 2023-08-08 18:58:33.728122 sphinxcontrib_applehelp-1.0.5/tox.ini
+-rw-r--r--   0        0        0     2207 1970-01-01 00:00:00.000000 sphinxcontrib_applehelp-1.0.5/PKG-INFO
```

### Comparing `sphinxcontrib-applehelp-1.0.4/LICENSE` & `sphinxcontrib_applehelp-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/PKG-INFO` & `sphinxcontrib_applehelp-1.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,76 +1,63 @@
-Metadata-Version: 2.1
-Name: sphinxcontrib-applehelp
-Version: 1.0.4
-Summary: sphinxcontrib-applehelp is a Sphinx extension which outputs Apple help books
-Author-email: Georg Brandl <georg@python.org>
-License: BSD-2-Clause
-Project-URL: Changelog, https://www.sphinx-doc.org/en/master/changes.html
-Project-URL: Code, https://github.com/sphinx-doc/sphinxcontrib-applehelp
-Project-URL: Download, https://pypi.org/project/sphinxcontrib-applehelp/
-Project-URL: Homepage, https://www.sphinx-doc.org/
-Project-URL: Issue tracker, https://github.com/sphinx-doc/sphinx/issues
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Framework :: Sphinx
-Classifier: Framework :: Sphinx :: Extension
-Classifier: Topic :: Documentation
-Classifier: Topic :: Documentation :: Sphinx
-Classifier: Topic :: Text Processing
-Classifier: Topic :: Utilities
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-Provides-Extra: test
-Provides-Extra: lint
-License-File: LICENSE
-
-=======================
-sphinxcontrib-applehelp
-=======================
-
-sphinxcontrib-applehelp is a sphinx extension which outputs Apple help books.
-
-For more details, please visit http://www.sphinx-doc.org/.
-
-Installing
-==========
-
-Install from PyPI::
-
-   pip install -U sphinxcontrib-applehelp
-
-Release signatures
-==================
-
-Releases are signed with following keys:
-
-* `498D6B9E <https://pgp.mit.edu/pks/lookup?op=vindex&search=0x102C2C17498D6B9E>`_
-* `5EBA0E07 <https://pgp.mit.edu/pks/lookup?op=vindex&search=0x1425F8CE5EBA0E07>`_
-
-Testing
-=======
-
-To run the tests with the interpreter available as ``python``, use::
-
-    tox
-
-Continuous testing runs on travis: https://travis-ci.org/sphinx-doc/sphinxcontrib-applehelp
-
-Contributing
-============
-
-See `CONTRIBUTING.rst`__
-
-.. __: https://github.com/sphinx-doc/sphinx/blob/master/CONTRIBUTING.rst
+Metadata-Version: 2.1
+Name: sphinxcontrib-applehelp
+Version: 1.0.5
+Summary: sphinxcontrib-applehelp is a Sphinx extension which outputs Apple help books
+Author-email: Georg Brandl <georg@python.org>
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
+Classifier: Framework :: Sphinx
+Classifier: Framework :: Sphinx :: Extension
+Classifier: Topic :: Documentation
+Classifier: Topic :: Documentation :: Sphinx
+Classifier: Topic :: Text Processing
+Classifier: Topic :: Utilities
+Requires-Dist: Sphinx>=5
+Requires-Dist: flake8 ; extra == "lint"
+Requires-Dist: mypy ; extra == "lint"
+Requires-Dist: docutils-stubs ; extra == "lint"
+Requires-Dist: pytest ; extra == "test"
+Project-URL: Changelog, https://www.sphinx-doc.org/en/master/changes.html
+Project-URL: Code, https://github.com/sphinx-doc/sphinxcontrib-applehelp
+Project-URL: Download, https://pypi.org/project/sphinxcontrib-applehelp/
+Project-URL: Homepage, https://www.sphinx-doc.org/
+Project-URL: Issue tracker, https://github.com/sphinx-doc/sphinx/issues
+Provides-Extra: lint
+Provides-Extra: test
+
+=======================
+sphinxcontrib-applehelp
+=======================
+
+sphinxcontrib-applehelp is a sphinx extension which outputs Apple help books.
+
+For more details, please visit http://www.sphinx-doc.org/.
+
+Installing
+==========
+
+Install from PyPI::
+
+   pip install -U sphinxcontrib-applehelp
+
+Contributing
+============
+
+See `CONTRIBUTING.rst`__
+
+.. __: https://github.com/sphinx-doc/sphinx/blob/master/CONTRIBUTING.rst
+
```

### Comparing `sphinxcontrib-applehelp-1.0.4/pyproject.toml` & `sphinxcontrib_applehelp-1.0.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 [build-system]
-requires = ["setuptools>=64"]
-build-backend = "setuptools.build_meta"
+requires = ["flit_core>=3.7"]
+build-backend = "flit_core.buildapi"
 
 # project metadata
 [project]
 name = "sphinxcontrib-applehelp"
 description = "sphinxcontrib-applehelp is a Sphinx extension which outputs Apple help books"
 readme = "README.rst"
 urls.Changelog = "https://www.sphinx-doc.org/en/master/changes.html"
 urls.Code = "https://github.com/sphinx-doc/sphinxcontrib-applehelp"
 urls.Download = "https://pypi.org/project/sphinxcontrib-applehelp/"
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
 ]
 lint = [
@@ -52,12 +54,24 @@
     "docutils-stubs",
 ]
 
 [[project.authors]]
 name = "Georg Brandl"
 email = "georg@python.org"
 
-[tool.setuptools.dynamic]
-version.attr = "sphinxcontrib.applehelp.__version__"
+[tool.flit.module]
+name = "sphinxcontrib.applehelp"
+
+[tool.flit.sdist]
+include = [
+    "CHANGES",
+    "LICENSE",
+    # Tests
+    "tests/",
+    "tox.ini",
+]
+exclude = [
+    "doc/_build",
+]
 
 [tool.mypy]
 ignore_missing_imports = true
```

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/__init__.py` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,16 @@
-"""
-    sphinxcontrib.applehelp
-    ~~~~~~~~~~~~~~~~~~~~~~~
-
-    Build Apple help books.
-
-    :copyright: Copyright 2007-2019 by the Sphinx team, see README.
-    :license: BSD, see LICENSE for details.
-"""
+"""Build Apple help books."""
 
 import plistlib
 import shlex
 import subprocess
 from os import environ
 from os import path
 from subprocess import CalledProcessError, PIPE, STDOUT
-from typing import Any, Dict
+from typing import Any
 
 import sphinx
 from sphinx.application import Sphinx
 from sphinx.builders.html import StandaloneHTMLBuilder
 from sphinx.errors import SphinxError
 from sphinx.locale import get_translation
 from sphinx.util import logging
@@ -29,16 +21,16 @@
 if sphinx.version_info[:2] >= (6, 1):
     from sphinx.util.display import SkipProgressMessage, progress_message
 else:
     from sphinx.util import (  # type: ignore[attr-defined,no-redef]
         SkipProgressMessage, progress_message
     )
 
-__version__ = '1.0.4'
-__version_info__ = (1, 0, 4)
+__version__ = '1.0.5'
+__version_info__ = (1, 0, 5)
 
 package_dir = path.abspath(path.dirname(__file__))
 template_dir = path.join(package_dir, 'templates')
 
 __ = get_translation(__name__, 'console')
 logger = logging.getLogger(__name__)
 
@@ -82,20 +74,20 @@
         self.out_suffix = '.html'
         self.link_suffix = '.html'
 
         if self.config.applehelp_bundle_id is None:
             raise SphinxError(__('You must set applehelp_bundle_id before '
                                  'building Apple Help output'))
 
-        self.bundle_path = path.join(self.outdir,  # type: ignore
-                                     self.config.applehelp_bundle_name + '.help')
-        self.outdir = path.join(self.bundle_path,
-                                'Contents',
-                                'Resources',
-                                self.config.applehelp_locale + '.lproj')
+        self.bundle_path = self.outdir / (self.config.applehelp_bundle_name + '.help')
+        self.outdir = self.bundle_path.joinpath(
+            'Contents',
+            'Resources',
+            self.config.applehelp_locale + '.lproj',
+        )
 
     def handle_finish(self) -> None:
         super().handle_finish()
 
         self.finish_tasks.add_task(self.copy_localized_files)
         self.finish_tasks.add_task(self.build_helpbook)
 
@@ -229,15 +221,15 @@
                 subprocess.run(args, stdout=PIPE, stderr=STDOUT, check=True)
             except OSError:
                 raise AppleHelpCodeSigningFailed(__('Command not found: %s') % args[0])
             except CalledProcessError as exc:
                 raise AppleHelpCodeSigningFailed(exc.stdout)
 
 
-def setup(app: Sphinx) -> Dict[str, Any]:
+def setup(app: Sphinx) -> dict[str, Any]:
     app.setup_extension('sphinx.builders.html')
     app.add_builder(AppleHelpBuilder)
     app.add_message_catalog(__name__, path.join(package_dir, 'locales'))
 
     app.add_config_value('applehelp_bundle_name',
                          lambda self: make_filename(self.project), 'applehelp')
     app.add_config_value('applehelp_bundle_id', None, 'applehelp', [str])
```

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ar/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ar/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ar/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ar/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/bn/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/bn/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/bn/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/bn/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ca/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ca/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ca/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ca/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/cak/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/cak/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/cak/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/cak/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/cs/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/cs/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/cs/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/cs/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/cy/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/cy/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/cy/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/cy/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/da/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/da/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/da/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/da/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/de/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/de/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/de/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/de/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/el/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/el/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/el/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/el/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/eo/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/eo/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/eo/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/eo/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/es/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/es/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/es/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/es/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/et/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/et/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/et/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/et/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/eu/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/eu/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/eu/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/eu/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/fa/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/fa/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/fa/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/fa/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/fi/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/fi/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/fi/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/fi/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/fr/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/fr/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/fr/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/fr/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/he/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/he/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/he/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/he/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/hi/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/hi/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/hi/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/hi/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/hi_IN/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/hi_IN/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/hi_IN/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/hi_IN/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/hr/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/hr/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/hr/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/hr/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/hu/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/hu/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/hu/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/hu/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/id/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/id/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/id/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/id/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/it/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/it/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/it/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/it/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ja/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ja/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ja/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ja/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ko/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ko/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ko/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ko/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/lt/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/lt/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/lt/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/lt/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/lv/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/lv/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/lv/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/lv/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/mk/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/mk/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/mk/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/mk/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/nb_NO/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/nb_NO/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/nb_NO/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/nb_NO/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ne/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ne/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ne/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ne/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/nl/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/nl/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/nl/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/nl/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/pl/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/pl/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/pl/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/pl/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/pt/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/pt/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/pt/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/pt/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/pt_BR/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/pt_BR/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/pt_BR/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/pt_BR/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/pt_PT/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/pt_PT/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/pt_PT/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/pt_PT/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ro/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ro/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ro/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ro/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ru/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ru/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ru/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ru/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/si/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/si/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/si/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/si/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/sk/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/sk/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/sk/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/sk/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/sl/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/sl/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/sl/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/sl/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/sphinxcontrib.applehelp.pot` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/sphinxcontrib.applehelp.pot`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/sr/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/sr/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/sr/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/sr/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/sr@latin/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/sr@latin/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/sr@latin/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/sr@latin/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/sv/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/sv/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/sv/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/sv/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ta/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ta/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ta/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ta/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/tr/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/tr/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/tr/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/tr/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/uk_UA/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/uk_UA/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/uk_UA/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/uk_UA/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ur/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ur/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/ur/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/ur/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/vi/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/vi/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/vi/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/vi/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/zh_CN/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/zh_CN/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/zh_CN/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/zh_CN/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/zh_TW/LC_MESSAGES/sphinxcontrib.applehelp.mo` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/zh_TW/LC_MESSAGES/sphinxcontrib.applehelp.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/sphinxcontrib/applehelp/locales/zh_TW/LC_MESSAGES/sphinxcontrib.applehelp.po` & `sphinxcontrib_applehelp-1.0.5/sphinxcontrib/applehelp/locales/zh_TW/LC_MESSAGES/sphinxcontrib.applehelp.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-applehelp-1.0.4/tests/test_applehelp.py` & `sphinxcontrib_applehelp-1.0.5/tests/test_applehelp.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,43 @@
-"""
-    test_applehelp
-    ~~~~~~~~~~~~~~
-
-    Test for applehelp extension.
-
-    :copyright: Copyright 2007-2019 by the Sphinx team, see AUTHORS.
-    :license: BSD, see LICENSE for details.
-"""
+"""Test for applehelp extension."""
 
+from pathlib import Path
 import plistlib
 
 import pytest
 
-from sphinx.testing.path import path
-
 
 def check_structure(outdir):
     contentsdir = outdir / 'Contents'
-    assert contentsdir.isdir()
-    assert (contentsdir / 'Info.plist').isfile()
+    assert contentsdir.is_dir()
+    assert (contentsdir / 'Info.plist').is_file()
 
-    with open(contentsdir / 'Info.plist', 'rb') as f:
+    with contentsdir.joinpath('Info.plist').open('rb') as f:
         plist = plistlib.load(f)
     assert plist
     assert len(plist)
     assert plist.get('CFBundleIdentifier', None) == 'org.sphinx-doc.Sphinx.help'
 
-    assert (contentsdir / 'Resources').isdir()
-    assert (contentsdir / 'Resources' / 'en.lproj').isdir()
+    assert (contentsdir / 'Resources').is_dir()
+    assert (contentsdir / 'Resources' / 'en.lproj').is_dir()
 
 
 def check_localization(outdir):
     lprojdir = outdir / 'Contents' / 'Resources' / 'en.lproj'
-    assert (lprojdir / 'localized.txt').isfile()
+    assert (lprojdir / 'localized.txt').is_file()
 
 
 @pytest.mark.sphinx(
     'applehelp', testroot='basic', srcdir='applehelp_output',
     confoverrides={'applehelp_bundle_id': 'org.sphinx-doc.Sphinx.help',
                    'applehelp_disable_external_tools': True})
 def test_applehelp_output(app, status, warning):
-    (app.srcdir / 'en.lproj').makedirs()
-    (app.srcdir / 'en.lproj' / 'localized.txt').write_text('')
+    (app.srcdir / 'en.lproj').mkdir(parents=True, exist_ok=True)
+    (app.srcdir / 'en.lproj' / 'localized.txt').touch()
     app.builder.build_all()
 
     # Have to use bundle_path, not outdir, because we alter the latter
     # to point to the lproj directory so that the HTML arrives in the
     # correct location.
-    bundle_path = path(app.builder.bundle_path)
+    bundle_path = Path(app.builder.bundle_path)
     check_structure(bundle_path)
     check_localization(bundle_path)
```

### Comparing `sphinxcontrib-applehelp-1.0.4/tox.ini` & `sphinxcontrib_applehelp-1.0.5/tox.ini`

 * *Files 11% similar despite different names*

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
 extras=
     lint
 commands=
-    mypy sphinxcontrib/
+    mypy sphinxcontrib/ --explicit-package-bases
```

