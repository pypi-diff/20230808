# Comparing `tmp/capeditor-0.2.9.tar.gz` & `tmp/capeditor-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capeditor-0.2.9.tar", last modified: Sun Jul 16 20:06:59 2023, max compression
+gzip compressed data, was "capeditor-0.3.0.tar", last modified: Tue Aug  8 12:38:15 2023, max compression
```

## Comparing `capeditor-0.2.9.tar` & `capeditor-0.3.0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:06:59.380447 capeditor-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-16 20:06:40.000000 capeditor-0.2.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-07-16 20:06:59.380447 capeditor-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-07-16 20:06:40.000000 capeditor-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:06:59.372446 capeditor-0.2.9/capeditor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    24001 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/blocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:06:59.372446 capeditor-0.2.9/capeditor/forms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/forms/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/forms/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:06:59.368445 capeditor-0.2.9/capeditor/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:06:59.368445 capeditor-0.2.9/capeditor/locale/am/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:06:59.376446 capeditor-0.2.9/capeditor/locale/am/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18830 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/locale/am/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    30674 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/locale/am/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:06:59.368445 capeditor-0.2.9/capeditor/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:06:59.376446 capeditor-0.2.9/capeditor/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    18042 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    30025 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:06:59.368445 capeditor-0.2.9/capeditor/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:06:59.376446 capeditor-0.2.9/capeditor/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    15036 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    26134 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:06:59.368445 capeditor-0.2.9/capeditor/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:06:59.376446 capeditor-0.2.9/capeditor/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    15856 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    27357 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:06:59.368445 capeditor-0.2.9/capeditor/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:06:59.376446 capeditor-0.2.9/capeditor/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    15859 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    27296 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:06:59.368445 capeditor-0.2.9/capeditor/locale/sw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:06:59.376446 capeditor-0.2.9/capeditor/locale/sw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    15240 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/locale/sw/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    26457 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/locale/sw/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:06:59.376446 capeditor-0.2.9/capeditor/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14563 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/renderers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:06:59.368445 capeditor-0.2.9/capeditor/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:06:59.368445 capeditor-0.2.9/capeditor/static/capeditor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:06:59.376446 capeditor-0.2.9/capeditor/static/capeditor/css/
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/static/capeditor/css/cap_detail_page.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:06:59.376446 capeditor-0.2.9/capeditor/static/capeditor/css/widget/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/static/capeditor/css/widget/boundary-widget.css
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/static/capeditor/css/widget/circle-widget.css
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/static/capeditor/css/widget/polygon-widget.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:06:59.376446 capeditor-0.2.9/capeditor/static/capeditor/js/
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/static/capeditor/js/cap_accordion.js
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/static/capeditor/js/conditional_fields.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:06:59.380447 capeditor-0.2.9/capeditor/static/capeditor/js/widget/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/static/capeditor/js/widget/circle-widget-telepath.js
--rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/static/capeditor/js/widget/circle-widget.js
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js
--rw-r--r--   0 runner    (1001) docker     (123)    10704 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/static/capeditor/js/widget/polygon-widget.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:06:59.368445 capeditor-0.2.9/capeditor/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:06:59.380447 capeditor-0.2.9/capeditor/templates/capeditor/
--rw-r--r--   0 runner    (1001) docker     (123)    15623 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/templates/capeditor/cap_alert_page.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:06:59.380447 capeditor-0.2.9/capeditor/templates/capeditor/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/templates/capeditor/icons/cap-alert-full.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/templates/capeditor/icons/cap-alert.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:06:59.380447 capeditor-0.2.9/capeditor/templates/capeditor/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/templates/capeditor/widgets/boundary_polygon_widget.html
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/templates/capeditor/widgets/circle_widget.html
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/templates/capeditor/widgets/polygon_widget.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-16 20:06:40.000000 capeditor-0.2.9/capeditor/wagtail_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 20:06:59.372446 capeditor-0.2.9/capeditor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-07-16 20:06:59.000000 capeditor-0.2.9/capeditor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-16 20:06:59.000000 capeditor-0.2.9/capeditor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 20:06:59.000000 capeditor-0.2.9/capeditor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-16 20:06:59.000000 capeditor-0.2.9/capeditor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-16 20:06:59.000000 capeditor-0.2.9/capeditor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-16 20:06:40.000000 capeditor-0.2.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-16 20:06:59.380447 capeditor-0.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:38:15.398460 capeditor-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-08 12:37:58.000000 capeditor-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-08-08 12:38:15.398460 capeditor-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-08-08 12:37:58.000000 capeditor-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:38:15.394459 capeditor-0.3.0/capeditor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24001 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/blocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:38:15.394459 capeditor-0.3.0/capeditor/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/forms/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/forms/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:38:15.390459 capeditor-0.3.0/capeditor/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:38:15.390459 capeditor-0.3.0/capeditor/locale/am/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:38:15.394459 capeditor-0.3.0/capeditor/locale/am/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18830 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/locale/am/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30674 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/locale/am/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:38:15.390459 capeditor-0.3.0/capeditor/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:38:15.394459 capeditor-0.3.0/capeditor/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    18042 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    30025 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:38:15.390459 capeditor-0.3.0/capeditor/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:38:15.394459 capeditor-0.3.0/capeditor/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    15036 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    26134 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:38:15.390459 capeditor-0.3.0/capeditor/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:38:15.394459 capeditor-0.3.0/capeditor/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    15856 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    27357 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:38:15.390459 capeditor-0.3.0/capeditor/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:38:15.398460 capeditor-0.3.0/capeditor/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    15859 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    27296 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:38:15.390459 capeditor-0.3.0/capeditor/locale/sw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:38:15.398460 capeditor-0.3.0/capeditor/locale/sw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    15240 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/locale/sw/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    26457 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/locale/sw/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:38:15.398460 capeditor-0.3.0/capeditor/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14612 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:38:15.390459 capeditor-0.3.0/capeditor/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:38:15.390459 capeditor-0.3.0/capeditor/static/capeditor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:38:15.398460 capeditor-0.3.0/capeditor/static/capeditor/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/static/capeditor/css/cap_detail_page.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:38:15.398460 capeditor-0.3.0/capeditor/static/capeditor/css/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/static/capeditor/css/widget/boundary-widget.css
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/static/capeditor/css/widget/circle-widget.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/static/capeditor/css/widget/polygon-widget.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:38:15.398460 capeditor-0.3.0/capeditor/static/capeditor/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/static/capeditor/js/cap_accordion.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/static/capeditor/js/conditional_fields.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:38:15.398460 capeditor-0.3.0/capeditor/static/capeditor/js/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8373 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/static/capeditor/js/widget/circle-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/static/capeditor/js/widget/circle-widget.js
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/static/capeditor/js/widget/polygon-widget.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:38:15.390459 capeditor-0.3.0/capeditor/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:38:15.398460 capeditor-0.3.0/capeditor/templates/capeditor/
+-rw-r--r--   0 runner    (1001) docker     (123)    15623 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/templates/capeditor/cap_alert_page.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:38:15.398460 capeditor-0.3.0/capeditor/templates/capeditor/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/templates/capeditor/icons/cap-alert-full.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/templates/capeditor/icons/cap-alert.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:38:15.398460 capeditor-0.3.0/capeditor/templates/capeditor/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/templates/capeditor/widgets/boundary_polygon_widget.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/templates/capeditor/widgets/circle_widget.html
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/templates/capeditor/widgets/polygon_widget.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-08-08 12:37:58.000000 capeditor-0.3.0/capeditor/wagtail_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 12:38:15.394459 capeditor-0.3.0/capeditor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-08-08 12:38:15.000000 capeditor-0.3.0/capeditor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-08-08 12:38:15.000000 capeditor-0.3.0/capeditor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 12:38:15.000000 capeditor-0.3.0/capeditor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-08 12:38:15.000000 capeditor-0.3.0/capeditor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-08 12:38:15.000000 capeditor-0.3.0/capeditor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-08 12:37:58.000000 capeditor-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-08 12:38:15.402460 capeditor-0.3.0/setup.cfg
```

### Comparing `capeditor-0.2.9/PKG-INFO` & `capeditor-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capeditor
-Version: 0.2.9
+Version: 0.3.0
 Summary: Wagtail based CAP Editor
 Home-page: https://github.com/wmo-raf/cap-editor
 Author: Grace Amondi, Erick Otenyo
 Author-email: miswa.grace@gmail.com, otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -51,27 +51,21 @@
             -   [B. Alert Info](#b.-alert-info)
             -   [C. Alert Area](#c.-alert-area)
             -   [D. Alert Resource](#d.-alert-resource)
     -   [Integrations](#integrations)
     
 ## Quick start
 
-#### 1. Clone repository
+#### 1. Install in virualenvironment using pip
 
 ``` sh
-git clone https://github.com/wmo-raf/cap-editor.git
+pip install capeditor
 ```
 
-#### 2. Install in virualenvironment using pip
-
-``` sh
-pip install path_to/capeditor/dist/capeditor-{version}.tar.gz
-```
-
-#### 3. Configure settings
+#### 2. Configure settings
 
 In your `settings.py` or `settings/base.py`, within the installed apps,
 include the `rest_framework, rest_framework_xml` and `capeditor` as
 below:
 
 ``` py
 INSTALLED_APPS = [
@@ -92,31 +86,15 @@
     ),
     'DEFAULT_PARSER_CLASSES': (
         'rest_framework_xml.parsers.XMLParser',
     ),
 }
 ```
 
-#### 4. Include the cap urls
-
-In `urls.py`, include the cap urls as below. This is where the cap api
-for listed (`/cap/caps.xml`) and detailed(`/cap/{cap_id}.xml`) cap view
-will be hosted.
-
-``` py
-from capeditor import urls as cap_urls
-
-urlpatterns = [
-    # ...
-    path('cap', include(cap_urls))
-
-]
-```
-
-#### 5. Run model migrations
+#### 3. Run model migrations
 
 ``` sh
 python manage.py migrate
 ```
 
 ## Usage
 
@@ -242,54 +220,10 @@
 Multiple instances of this section are allowed. It contains the
 **Description (resourceDesc), MIME Type (mimeType), File Size (size),
 URI (uri), Dereferenced URI (derefUri) and Digest (digest)**
 
 ## Integrations
 
 To integrate the alerts to another wagtail page and include in
-templates, for example in the home page follow the instructions below:
+templates, for example in the home page refer to sandbox folder for sample standalone.
 
-Call the alerts in your models.py under the 'get_context' method:
 
-``` py
-from capeditor.models import Alert
-
-class HomePage(Page):
-
-    # ...
-
-
-    def get_context(self, request, *args, **kwargs):
-        context =super().get_context(request, *args, **kwargs)
-       
-        context['alerts'] = Alert.objects.live().public()
-        context['latest_alerts'] = context['alerts'][:3]
-        return context  
-```
-
-Parse the alerts in the home template:
-
-``` django
-
-{% for alert in latest_alerts.all %}
-    
-    <p>{{alert.sent}}</p>
-
-    <!-- info list  -->
-    {% for info in alert.alert_info.all %}
-        {% if alerts %}
-
-            <p>{{info.event}}</p>
-            <p>{{info.get_severity_display}}</p>
-
-            <!-- area list  -->
-            {% for alert_area in info.alert_areas.values%}
-                <p>{{alert_area.areaDesc}}</p>
-                <p>{{ alert_area.area }}</p>
-            {% endfor %}
-
-            <!-- other fields  -->
-
-        {% endif %}
-    {% endfor %}
-{% endfor %}
-```
```

### Comparing `capeditor-0.2.9/README.md` & `capeditor-0.3.0/capeditor.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: capeditor
+Version: 0.3.0
+Summary: Wagtail based CAP Editor
+Home-page: https://github.com/wmo-raf/cap-editor
+Author: Grace Amondi, Erick Otenyo
+Author-email: miswa.grace@gmail.com, otenyo.erick@gmail.com
+License: MIT
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+
 # CAP Editor  <img style="float: right;" height="40" src="images/caplogo.jpeg" markdown="1"> 
 [![Upload Python Package](https://github.com/wmo-raf/cap-editor/actions/workflows/publish.yml/badge.svg)](https://github.com/wmo-raf/cap-editor/actions/workflows/publish.yml)
 
 A Wagtail Commmon Alerting Protocol (CAP) Editor python package
 installable as an app on any wagtail project (version\>=4.1).
 
 The **Common Alerting Protocol (CAP)** provides an open, non-proprietary
@@ -30,27 +51,21 @@
             -   [B. Alert Info](#b.-alert-info)
             -   [C. Alert Area](#c.-alert-area)
             -   [D. Alert Resource](#d.-alert-resource)
     -   [Integrations](#integrations)
     
 ## Quick start
 
-#### 1. Clone repository
+#### 1. Install in virualenvironment using pip
 
 ``` sh
-git clone https://github.com/wmo-raf/cap-editor.git
+pip install capeditor
 ```
 
-#### 2. Install in virualenvironment using pip
-
-``` sh
-pip install path_to/capeditor/dist/capeditor-{version}.tar.gz
-```
-
-#### 3. Configure settings
+#### 2. Configure settings
 
 In your `settings.py` or `settings/base.py`, within the installed apps,
 include the `rest_framework, rest_framework_xml` and `capeditor` as
 below:
 
 ``` py
 INSTALLED_APPS = [
@@ -71,31 +86,15 @@
     ),
     'DEFAULT_PARSER_CLASSES': (
         'rest_framework_xml.parsers.XMLParser',
     ),
 }
 ```
 
-#### 4. Include the cap urls
-
-In `urls.py`, include the cap urls as below. This is where the cap api
-for listed (`/cap/caps.xml`) and detailed(`/cap/{cap_id}.xml`) cap view
-will be hosted.
-
-``` py
-from capeditor import urls as cap_urls
-
-urlpatterns = [
-    # ...
-    path('cap', include(cap_urls))
-
-]
-```
-
-#### 5. Run model migrations
+#### 3. Run model migrations
 
 ``` sh
 python manage.py migrate
 ```
 
 ## Usage
 
@@ -221,54 +220,10 @@
 Multiple instances of this section are allowed. It contains the
 **Description (resourceDesc), MIME Type (mimeType), File Size (size),
 URI (uri), Dereferenced URI (derefUri) and Digest (digest)**
 
 ## Integrations
 
 To integrate the alerts to another wagtail page and include in
-templates, for example in the home page follow the instructions below:
+templates, for example in the home page refer to sandbox folder for sample standalone.
 
-Call the alerts in your models.py under the 'get_context' method:
 
-``` py
-from capeditor.models import Alert
-
-class HomePage(Page):
-
-    # ...
-
-
-    def get_context(self, request, *args, **kwargs):
-        context =super().get_context(request, *args, **kwargs)
-       
-        context['alerts'] = Alert.objects.live().public()
-        context['latest_alerts'] = context['alerts'][:3]
-        return context  
-```
-
-Parse the alerts in the home template:
-
-``` django
-
-{% for alert in latest_alerts.all %}
-    
-    <p>{{alert.sent}}</p>
-
-    <!-- info list  -->
-    {% for info in alert.alert_info.all %}
-        {% if alerts %}
-
-            <p>{{info.event}}</p>
-            <p>{{info.get_severity_display}}</p>
-
-            <!-- area list  -->
-            {% for alert_area in info.alert_areas.values%}
-                <p>{{alert_area.areaDesc}}</p>
-                <p>{{ alert_area.area }}</p>
-            {% endfor %}
-
-            <!-- other fields  -->
-
-        {% endif %}
-    {% endfor %}
-{% endfor %}
-```
```

### Comparing `capeditor-0.2.9/capeditor/blocks.py` & `capeditor-0.3.0/capeditor/blocks.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.9/capeditor/forms/widgets.py` & `capeditor-0.3.0/capeditor/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.9/capeditor/locale/am/LC_MESSAGES/django.mo` & `capeditor-0.3.0/capeditor/locale/am/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.9/capeditor/locale/am/LC_MESSAGES/django.po` & `capeditor-0.3.0/capeditor/locale/am/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.9/capeditor/locale/ar/LC_MESSAGES/django.mo` & `capeditor-0.3.0/capeditor/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.9/capeditor/locale/ar/LC_MESSAGES/django.po` & `capeditor-0.3.0/capeditor/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.9/capeditor/locale/en/LC_MESSAGES/django.mo` & `capeditor-0.3.0/capeditor/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.9/capeditor/locale/en/LC_MESSAGES/django.po` & `capeditor-0.3.0/capeditor/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.9/capeditor/locale/es/LC_MESSAGES/django.mo` & `capeditor-0.3.0/capeditor/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.9/capeditor/locale/es/LC_MESSAGES/django.po` & `capeditor-0.3.0/capeditor/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.9/capeditor/locale/fr/LC_MESSAGES/django.mo` & `capeditor-0.3.0/capeditor/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.9/capeditor/locale/fr/LC_MESSAGES/django.po` & `capeditor-0.3.0/capeditor/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.9/capeditor/locale/sw/LC_MESSAGES/django.mo` & `capeditor-0.3.0/capeditor/locale/sw/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.9/capeditor/locale/sw/LC_MESSAGES/django.po` & `capeditor-0.3.0/capeditor/locale/sw/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.9/capeditor/migrations/0001_initial.py` & `capeditor-0.3.0/capeditor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.9/capeditor/models.py` & `capeditor-0.3.0/capeditor/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,14 +165,16 @@
                         info_field.block.child_blocks[block_type].child_blocks[field_name].name = name
                         info_field.block.child_blocks[block_type].child_blocks[field_name].label = label
 
 
 class AbstractCapAlertPage(Page):
     base_form_class = CapAlertPageForm
 
+    exclude_fields_in_copy = ["identifier"]
+
     STATUS_CHOICES = (
         ("Draft", _("Draft - A preliminary template or draft, not actionable in its current form")),
         ("Actual", _("Actual - Actionable by all targeted recipients")),
         ("Test", _("Test - Technical testing only, all recipients disregard")),
         ("Exercise", _("Exercise - Actionable only by designated exercise participants; "
                        "exercise identifier SHOULD appear in note")),
         ("system", _("System - For messages that support alert network internal functions")),
@@ -193,15 +195,15 @@
         ('Restricted', _("Restricted - For dissemination only to users with a known operational "
                          "requirement as in the restriction field")),
         ('Private', _("Private - For dissemination only to specified addresses"
                       " as in the addresses field in the alert")),
     )
 
     identifier = models.UUIDField(default=uuid.uuid4, editable=False, verbose_name=_("Identifier"),
-                                  help_text=_("Unique ID. Auto generated on creation."), )
+                                  help_text=_("Unique ID. Auto generated on creation."), unique=True)
     sender = models.CharField(max_length=255, verbose_name=_("Sender"), default=get_default_sender,
                               help_text=_("Identifies the originator of an alert. "
                                           "For example the website address of the institution"))
     sent = models.DateTimeField(default=timezone.now, verbose_name=_("Sent"),
                                 help_text=_("Time and date of origination of the alert"))
     status = models.CharField(max_length=50, choices=STATUS_CHOICES, default="Actual", verbose_name=_("Status"),
                               help_text=_("The code denoting the appropriate handling of the alert"))
@@ -315,9 +317,7 @@
                 areas.append(area.get("areaDesc"))
 
         return ", ".join(areas)
 
     @property
     def xml_link(self):
         return None
-    
-
```

### Comparing `capeditor-0.2.9/capeditor/renderers.py` & `capeditor-0.3.0/capeditor/renderers.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.9/capeditor/serializers.py` & `capeditor-0.3.0/capeditor/serializers.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.9/capeditor/static/capeditor/css/cap_detail_page.css` & `capeditor-0.3.0/capeditor/static/capeditor/css/cap_detail_page.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.9/capeditor/static/capeditor/css/widget/circle-widget.css` & `capeditor-0.3.0/capeditor/static/capeditor/css/widget/circle-widget.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.9/capeditor/static/capeditor/css/widget/polygon-widget.css` & `capeditor-0.3.0/capeditor/static/capeditor/css/widget/polygon-widget.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.9/capeditor/static/capeditor/js/cap_accordion.js` & `capeditor-0.3.0/capeditor/static/capeditor/js/cap_accordion.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.9/capeditor/static/capeditor/js/conditional_fields.js` & `capeditor-0.3.0/capeditor/static/capeditor/js/conditional_fields.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.9/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js` & `capeditor-0.3.0/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.9/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js` & `capeditor-0.3.0/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -114,17 +114,15 @@
         style: defaultStyle,
         doubleClickZoom: false,
     });
 
 
     this.map.addControl(
         new maplibregl.NavigationControl({
-            visualizePitch: true,
-            showZoom: true,
-            showCompass: true,
+            showCompass: false,
         }), "bottom-right"
     );
 
     this.map.addControl(new maplibregl.FullscreenControl());
 
     await new Promise((resolve) => this.map.on("load", resolve));
```

### Comparing `capeditor-0.2.9/capeditor/static/capeditor/js/widget/circle-widget-telepath.js` & `capeditor-0.3.0/capeditor/static/capeditor/js/widget/circle-widget-telepath.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.9/capeditor/static/capeditor/js/widget/circle-widget.js` & `capeditor-0.3.0/capeditor/static/capeditor/js/widget/circle-widget.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -135,17 +135,15 @@
         style: defaultStyle,
         doubleClickZoom: false,
     });
 
 
     this.map.addControl(
         new maplibregl.NavigationControl({
-            visualizePitch: true,
-            showZoom: true,
-            showCompass: true,
+            showCompass: false,
         }), "bottom-right"
     );
 
     this.map.addControl(new maplibregl.FullscreenControl());
 
     await new Promise((resolve) => this.map.on("load", resolve));
```

### Comparing `capeditor-0.2.9/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js` & `capeditor-0.3.0/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.9/capeditor/static/capeditor/js/widget/polygon-widget.js` & `capeditor-0.3.0/capeditor/static/capeditor/js/widget/polygon-widget.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -166,17 +166,15 @@
         style: defaultStyle,
         doubleClickZoom: false,
     });
 
 
     this.map.addControl(
         new maplibregl.NavigationControl({
-            visualizePitch: true,
-            showZoom: true,
-            showCompass: true,
+            showCompass: false,
         }), "bottom-right"
     );
 
     this.map.addControl(new maplibregl.FullscreenControl());
 
     await new Promise((resolve) => this.map.on("load", resolve));
```

### Comparing `capeditor-0.2.9/capeditor/templates/capeditor/cap_alert_page.html` & `capeditor-0.3.0/capeditor/templates/capeditor/cap_alert_page.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.9/capeditor/templates/capeditor/icons/cap-alert-full.svg` & `capeditor-0.3.0/capeditor/templates/capeditor/icons/cap-alert-full.svg`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.9/capeditor/templates/capeditor/icons/cap-alert.svg` & `capeditor-0.3.0/capeditor/templates/capeditor/icons/cap-alert.svg`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.9/capeditor/templates/capeditor/widgets/circle_widget.html` & `capeditor-0.3.0/capeditor/templates/capeditor/widgets/circle_widget.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.9/capeditor.egg-info/PKG-INFO` & `capeditor-0.3.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: capeditor
-Version: 0.2.9
-Summary: Wagtail based CAP Editor
-Home-page: https://github.com/wmo-raf/cap-editor
-Author: Grace Amondi, Erick Otenyo
-Author-email: miswa.grace@gmail.com, otenyo.erick@gmail.com
-License: MIT
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
 # CAP Editor  <img style="float: right;" height="40" src="images/caplogo.jpeg" markdown="1"> 
 [![Upload Python Package](https://github.com/wmo-raf/cap-editor/actions/workflows/publish.yml/badge.svg)](https://github.com/wmo-raf/cap-editor/actions/workflows/publish.yml)
 
 A Wagtail Commmon Alerting Protocol (CAP) Editor python package
 installable as an app on any wagtail project (version\>=4.1).
 
 The **Common Alerting Protocol (CAP)** provides an open, non-proprietary
@@ -51,27 +30,21 @@
             -   [B. Alert Info](#b.-alert-info)
             -   [C. Alert Area](#c.-alert-area)
             -   [D. Alert Resource](#d.-alert-resource)
     -   [Integrations](#integrations)
     
 ## Quick start
 
-#### 1. Clone repository
+#### 1. Install in virualenvironment using pip
 
 ``` sh
-git clone https://github.com/wmo-raf/cap-editor.git
+pip install capeditor
 ```
 
-#### 2. Install in virualenvironment using pip
-
-``` sh
-pip install path_to/capeditor/dist/capeditor-{version}.tar.gz
-```
-
-#### 3. Configure settings
+#### 2. Configure settings
 
 In your `settings.py` or `settings/base.py`, within the installed apps,
 include the `rest_framework, rest_framework_xml` and `capeditor` as
 below:
 
 ``` py
 INSTALLED_APPS = [
@@ -92,31 +65,15 @@
     ),
     'DEFAULT_PARSER_CLASSES': (
         'rest_framework_xml.parsers.XMLParser',
     ),
 }
 ```
 
-#### 4. Include the cap urls
-
-In `urls.py`, include the cap urls as below. This is where the cap api
-for listed (`/cap/caps.xml`) and detailed(`/cap/{cap_id}.xml`) cap view
-will be hosted.
-
-``` py
-from capeditor import urls as cap_urls
-
-urlpatterns = [
-    # ...
-    path('cap', include(cap_urls))
-
-]
-```
-
-#### 5. Run model migrations
+#### 3. Run model migrations
 
 ``` sh
 python manage.py migrate
 ```
 
 ## Usage
 
@@ -242,54 +199,10 @@
 Multiple instances of this section are allowed. It contains the
 **Description (resourceDesc), MIME Type (mimeType), File Size (size),
 URI (uri), Dereferenced URI (derefUri) and Digest (digest)**
 
 ## Integrations
 
 To integrate the alerts to another wagtail page and include in
-templates, for example in the home page follow the instructions below:
+templates, for example in the home page refer to sandbox folder for sample standalone.
 
-Call the alerts in your models.py under the 'get_context' method:
 
-``` py
-from capeditor.models import Alert
-
-class HomePage(Page):
-
-    # ...
-
-
-    def get_context(self, request, *args, **kwargs):
-        context =super().get_context(request, *args, **kwargs)
-       
-        context['alerts'] = Alert.objects.live().public()
-        context['latest_alerts'] = context['alerts'][:3]
-        return context  
-```
-
-Parse the alerts in the home template:
-
-``` django
-
-{% for alert in latest_alerts.all %}
-    
-    <p>{{alert.sent}}</p>
-
-    <!-- info list  -->
-    {% for info in alert.alert_info.all %}
-        {% if alerts %}
-
-            <p>{{info.event}}</p>
-            <p>{{info.get_severity_display}}</p>
-
-            <!-- area list  -->
-            {% for alert_area in info.alert_areas.values%}
-                <p>{{alert_area.areaDesc}}</p>
-                <p>{{ alert_area.area }}</p>
-            {% endfor %}
-
-            <!-- other fields  -->
-
-        {% endif %}
-    {% endfor %}
-{% endfor %}
-```
```

### Comparing `capeditor-0.2.9/capeditor.egg-info/SOURCES.txt` & `capeditor-0.3.0/capeditor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `capeditor-0.2.9/setup.cfg` & `capeditor-0.3.0/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = capeditor
-version = 0.2.9
+version = 0.3.0
 description = Wagtail based CAP Editor
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/cap-editor
 author = Grace Amondi, Erick Otenyo
 author_email = miswa.grace@gmail.com, otenyo.erick@gmail.com
 license = MIT
@@ -26,14 +26,14 @@
 python_requires = >=3.9
 install_requires = 
 	wagtail>=4.2.2
 	djangorestframework-xml
 	python-magic
 	shapely>=2.0.1
 	wagtail-icon-chooser>=0.0.4
-	adm-boundary-manager>=0.0.3
+	adm-boundary-manager>=0.0.6
 	wagtail-humanitarian-icons>=2.0.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

