# Comparing `tmp/django-mp-seo-9.0.2.tar.gz` & `tmp/django-mp-seo-9.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-mp-seo-9.0.2.tar", last modified: Wed Jun 21 13:23:45 2023, max compression
+gzip compressed data, was "dist/django-mp-seo-9.0.3.tar", last modified: Tue Aug  8 15:36:30 2023, max compression
```

## Comparing `django-mp-seo-9.0.2.tar` & `django-mp-seo-9.0.3.tar`

### file list

```diff
@@ -1,60 +1,57 @@
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-06-21 13:23:45.000000 django-mp-seo-9.0.2/
--rw-rw-r--   0 dev       (1000) dev       (1000)      746 2021-12-18 19:09:41.000000 django-mp-seo-9.0.2/LICENSE
--rw-rw-r--   0 dev       (1000) dev       (1000)      135 2021-12-18 19:09:41.000000 django-mp-seo-9.0.2/MANIFEST.in
--rw-rw-r--   0 dev       (1000) dev       (1000)      322 2023-06-21 13:23:45.000000 django-mp-seo-9.0.2/PKG-INFO
--rw-rw-r--   0 dev       (1000) dev       (1000)     2550 2021-12-18 19:09:41.000000 django-mp-seo-9.0.2/README.md
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-06-21 13:23:45.000000 django-mp-seo-9.0.2/django_mp_seo.egg-info/
--rw-rw-r--   0 dev       (1000) dev       (1000)      322 2023-06-21 13:23:45.000000 django-mp-seo-9.0.2/django_mp_seo.egg-info/PKG-INFO
--rw-rw-r--   0 dev       (1000) dev       (1000)     1218 2023-06-21 13:23:45.000000 django-mp-seo-9.0.2/django_mp_seo.egg-info/SOURCES.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)        1 2023-06-21 13:23:45.000000 django-mp-seo-9.0.2/django_mp_seo.egg-info/dependency_links.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)       26 2023-06-21 13:23:45.000000 django-mp-seo-9.0.2/django_mp_seo.egg-info/requires.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)        4 2023-06-21 13:23:45.000000 django-mp-seo-9.0.2/django_mp_seo.egg-info/top_level.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)       27 2021-12-18 19:09:41.000000 django-mp-seo-9.0.2/requirements.txt
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-06-21 13:23:45.000000 django-mp-seo-9.0.2/seo/
--rw-rw-r--   0 dev       (1000) dev       (1000)      493 2022-09-07 17:20:05.000000 django-mp-seo-9.0.2/seo/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1862 2021-12-18 19:10:44.000000 django-mp-seo-9.0.2/seo/admin.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1138 2021-12-18 19:10:44.000000 django-mp-seo-9.0.2/seo/lib.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-06-21 13:23:45.000000 django-mp-seo-9.0.2/seo/locale/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-06-21 13:23:45.000000 django-mp-seo-9.0.2/seo/locale/ru/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-06-21 13:23:45.000000 django-mp-seo-9.0.2/seo/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 dev       (1000) dev       (1000)     2342 2021-12-18 19:10:44.000000 django-mp-seo-9.0.2/seo/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 dev       (1000) dev       (1000)     3781 2021-12-18 19:10:44.000000 django-mp-seo-9.0.2/seo/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-06-21 13:23:45.000000 django-mp-seo-9.0.2/seo/locale/uk/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-06-21 13:23:45.000000 django-mp-seo-9.0.2/seo/locale/uk/LC_MESSAGES/
--rw-rw-r--   0 dev       (1000) dev       (1000)     2281 2021-12-18 19:10:44.000000 django-mp-seo-9.0.2/seo/locale/uk/LC_MESSAGES/django.mo
--rw-rw-r--   0 dev       (1000) dev       (1000)     3717 2021-12-18 19:10:44.000000 django-mp-seo-9.0.2/seo/locale/uk/LC_MESSAGES/django.po
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-06-21 13:23:45.000000 django-mp-seo-9.0.2/seo/management/
--rw-rw-r--   0 dev       (1000) dev       (1000)        0 2021-12-18 19:10:44.000000 django-mp-seo-9.0.2/seo/management/__init__.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-06-21 13:23:45.000000 django-mp-seo-9.0.2/seo/management/commands/
--rw-rw-r--   0 dev       (1000) dev       (1000)        0 2021-12-18 19:10:44.000000 django-mp-seo-9.0.2/seo/management/commands/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1124 2021-12-18 19:10:44.000000 django-mp-seo-9.0.2/seo/management/commands/sync_page_meta.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      357 2023-06-21 13:23:29.000000 django-mp-seo-9.0.2/seo/middleware.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-06-21 13:23:45.000000 django-mp-seo-9.0.2/seo/migrations/
--rw-rw-r--   0 dev       (1000) dev       (1000)     1457 2021-12-18 19:10:44.000000 django-mp-seo-9.0.2/seo/migrations/0001_initial.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      801 2021-12-18 19:10:44.000000 django-mp-seo-9.0.2/seo/migrations/0002_auto_20190427_0832.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      874 2021-12-18 19:10:44.000000 django-mp-seo-9.0.2/seo/migrations/0003_auto_20190427_0906.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      425 2021-12-18 19:10:44.000000 django-mp-seo-9.0.2/seo/migrations/0004_auto_20190427_0953.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      459 2021-12-18 19:10:44.000000 django-mp-seo-9.0.2/seo/migrations/0005_auto_20190427_1001.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      422 2021-12-18 19:10:44.000000 django-mp-seo-9.0.2/seo/migrations/0006_pagemeta_og_image.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      976 2021-12-18 19:10:44.000000 django-mp-seo-9.0.2/seo/migrations/0007_search_query.py
--rw-rw-r--   0 dev       (1000) dev       (1000)        0 2021-12-18 19:10:44.000000 django-mp-seo-9.0.2/seo/migrations/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     4715 2022-09-07 17:20:05.000000 django-mp-seo-9.0.2/seo/models.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1158 2021-12-18 19:10:44.000000 django-mp-seo-9.0.2/seo/sitemaps.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-06-21 13:23:45.000000 django-mp-seo-9.0.2/seo/templates/
--rw-rw-r--   0 dev       (1000) dev       (1000)      238 2021-12-18 19:10:44.000000 django-mp-seo-9.0.2/seo/templates/403.html
--rw-rw-r--   0 dev       (1000) dev       (1000)      232 2021-12-18 19:10:44.000000 django-mp-seo-9.0.2/seo/templates/404.html
--rw-rw-r--   0 dev       (1000) dev       (1000)      289 2021-12-18 19:10:44.000000 django-mp-seo-9.0.2/seo/templates/500.html
--rw-rw-r--   0 dev       (1000) dev       (1000)     1134 2021-12-18 19:10:44.000000 django-mp-seo-9.0.2/seo/templates/error.html
--rw-rw-r--   0 dev       (1000) dev       (1000)      270 2021-12-18 19:10:44.000000 django-mp-seo-9.0.2/seo/templates/language_meta_tags.html
--rw-rw-r--   0 dev       (1000) dev       (1000)      678 2021-12-18 19:10:44.000000 django-mp-seo-9.0.2/seo/templates/sitemap.html
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-06-21 13:23:45.000000 django-mp-seo-9.0.2/seo/templates/sitemetrics/
--rw-rw-r--   0 dev       (1000) dev       (1000)      329 2021-12-18 19:10:44.000000 django-mp-seo-9.0.2/seo/templates/sitemetrics/google.html
--rw-rw-r--   0 dev       (1000) dev       (1000)       43 2021-12-18 19:10:44.000000 django-mp-seo-9.0.2/seo/templates/sitemetrics_tag.html
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-06-21 13:23:45.000000 django-mp-seo-9.0.2/seo/templatetags/
--rw-rw-r--   0 dev       (1000) dev       (1000)        0 2021-12-18 19:10:44.000000 django-mp-seo-9.0.2/seo/templatetags/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1000 2021-12-18 19:10:44.000000 django-mp-seo-9.0.2/seo/templatetags/seo.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      191 2021-12-18 19:10:44.000000 django-mp-seo-9.0.2/seo/translation.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      267 2021-12-18 19:10:44.000000 django-mp-seo-9.0.2/seo/urls.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      830 2021-12-18 19:10:44.000000 django-mp-seo-9.0.2/seo/views.py
--rw-rw-r--   0 dev       (1000) dev       (1000)       79 2023-06-21 13:23:45.000000 django-mp-seo-9.0.2/setup.cfg
--rw-rw-r--   0 dev       (1000) dev       (1000)      531 2023-06-21 13:23:29.000000 django-mp-seo-9.0.2/setup.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-08-08 15:36:30.000000 django-mp-seo-9.0.3/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      746 2021-12-18 19:09:41.000000 django-mp-seo-9.0.3/LICENSE
+-rw-rw-r--   0 dev       (1000) dev       (1000)      135 2021-12-18 19:09:41.000000 django-mp-seo-9.0.3/MANIFEST.in
+-rw-rw-r--   0 dev       (1000) dev       (1000)      322 2023-08-08 15:36:30.000000 django-mp-seo-9.0.3/PKG-INFO
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2523 2023-08-08 15:34:29.000000 django-mp-seo-9.0.3/README.md
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-08-08 15:36:30.000000 django-mp-seo-9.0.3/django_mp_seo.egg-info/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      322 2023-08-08 15:36:30.000000 django-mp-seo-9.0.3/django_mp_seo.egg-info/PKG-INFO
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1130 2023-08-08 15:36:30.000000 django-mp-seo-9.0.3/django_mp_seo.egg-info/SOURCES.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)        1 2023-08-08 15:36:30.000000 django-mp-seo-9.0.3/django_mp_seo.egg-info/dependency_links.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)        4 2023-08-08 15:36:30.000000 django-mp-seo-9.0.3/django_mp_seo.egg-info/top_level.txt
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-08-08 15:36:30.000000 django-mp-seo-9.0.3/seo/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      329 2023-08-08 15:34:29.000000 django-mp-seo-9.0.3/seo/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1862 2021-12-18 19:10:44.000000 django-mp-seo-9.0.3/seo/admin.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1138 2021-12-18 19:10:44.000000 django-mp-seo-9.0.3/seo/lib.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-08-08 15:36:30.000000 django-mp-seo-9.0.3/seo/locale/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-08-08 15:36:30.000000 django-mp-seo-9.0.3/seo/locale/ru/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-08-08 15:36:30.000000 django-mp-seo-9.0.3/seo/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2342 2021-12-18 19:10:44.000000 django-mp-seo-9.0.3/seo/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3781 2021-12-18 19:10:44.000000 django-mp-seo-9.0.3/seo/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-08-08 15:36:30.000000 django-mp-seo-9.0.3/seo/locale/uk/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-08-08 15:36:30.000000 django-mp-seo-9.0.3/seo/locale/uk/LC_MESSAGES/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2281 2021-12-18 19:10:44.000000 django-mp-seo-9.0.3/seo/locale/uk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3717 2021-12-18 19:10:44.000000 django-mp-seo-9.0.3/seo/locale/uk/LC_MESSAGES/django.po
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-08-08 15:36:30.000000 django-mp-seo-9.0.3/seo/management/
+-rw-rw-r--   0 dev       (1000) dev       (1000)        0 2021-12-18 19:10:44.000000 django-mp-seo-9.0.3/seo/management/__init__.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-08-08 15:36:30.000000 django-mp-seo-9.0.3/seo/management/commands/
+-rw-rw-r--   0 dev       (1000) dev       (1000)        0 2021-12-18 19:10:44.000000 django-mp-seo-9.0.3/seo/management/commands/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1124 2021-12-18 19:10:44.000000 django-mp-seo-9.0.3/seo/management/commands/sync_page_meta.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      357 2023-06-21 13:23:29.000000 django-mp-seo-9.0.3/seo/middleware.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-08-08 15:36:30.000000 django-mp-seo-9.0.3/seo/migrations/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1457 2021-12-18 19:10:44.000000 django-mp-seo-9.0.3/seo/migrations/0001_initial.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      801 2021-12-18 19:10:44.000000 django-mp-seo-9.0.3/seo/migrations/0002_auto_20190427_0832.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      874 2021-12-18 19:10:44.000000 django-mp-seo-9.0.3/seo/migrations/0003_auto_20190427_0906.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      425 2021-12-18 19:10:44.000000 django-mp-seo-9.0.3/seo/migrations/0004_auto_20190427_0953.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      459 2021-12-18 19:10:44.000000 django-mp-seo-9.0.3/seo/migrations/0005_auto_20190427_1001.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      422 2021-12-18 19:10:44.000000 django-mp-seo-9.0.3/seo/migrations/0006_pagemeta_og_image.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      976 2021-12-18 19:10:44.000000 django-mp-seo-9.0.3/seo/migrations/0007_search_query.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)        0 2021-12-18 19:10:44.000000 django-mp-seo-9.0.3/seo/migrations/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     4715 2022-09-07 17:20:05.000000 django-mp-seo-9.0.3/seo/models.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1158 2021-12-18 19:10:44.000000 django-mp-seo-9.0.3/seo/sitemaps.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-08-08 15:36:30.000000 django-mp-seo-9.0.3/seo/templates/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      238 2021-12-18 19:10:44.000000 django-mp-seo-9.0.3/seo/templates/403.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)      232 2021-12-18 19:10:44.000000 django-mp-seo-9.0.3/seo/templates/404.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)      289 2021-12-18 19:10:44.000000 django-mp-seo-9.0.3/seo/templates/500.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1134 2021-12-18 19:10:44.000000 django-mp-seo-9.0.3/seo/templates/error.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)      270 2021-12-18 19:10:44.000000 django-mp-seo-9.0.3/seo/templates/language_meta_tags.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)      678 2021-12-18 19:10:44.000000 django-mp-seo-9.0.3/seo/templates/sitemap.html
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-08-08 15:36:30.000000 django-mp-seo-9.0.3/seo/templates/sitemetrics/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      329 2021-12-18 19:10:44.000000 django-mp-seo-9.0.3/seo/templates/sitemetrics/google.html
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-08-08 15:36:30.000000 django-mp-seo-9.0.3/seo/templatetags/
+-rw-rw-r--   0 dev       (1000) dev       (1000)        0 2021-12-18 19:10:44.000000 django-mp-seo-9.0.3/seo/templatetags/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      885 2023-08-08 15:34:29.000000 django-mp-seo-9.0.3/seo/templatetags/seo.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      191 2021-12-18 19:10:44.000000 django-mp-seo-9.0.3/seo/translation.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      267 2021-12-18 19:10:44.000000 django-mp-seo-9.0.3/seo/urls.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      830 2021-12-18 19:10:44.000000 django-mp-seo-9.0.3/seo/views.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)       79 2023-08-08 15:36:30.000000 django-mp-seo-9.0.3/setup.cfg
+-rw-rw-r--   0 dev       (1000) dev       (1000)      426 2023-08-08 15:35:05.000000 django-mp-seo-9.0.3/setup.py
```

### Comparing `django-mp-seo-9.0.2/LICENSE` & `django-mp-seo-9.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-mp-seo-9.0.2/README.md` & `django-mp-seo-9.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -111,17 +111,15 @@
         {% endblock %}
 
     </body>
  
     {% block js %}
      
         ...
- 
-        {% sitemetrics %}
- 
+  
     {% endblock %}
  
 </html>
 ```
 
 Run migrations:
```

### Comparing `django-mp-seo-9.0.2/django_mp_seo.egg-info/SOURCES.txt` & `django-mp-seo-9.0.3/django_mp_seo.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
-requirements.txt
 setup.cfg
 setup.py
 django_mp_seo.egg-info/PKG-INFO
 django_mp_seo.egg-info/SOURCES.txt
 django_mp_seo.egg-info/dependency_links.txt
-django_mp_seo.egg-info/requires.txt
 django_mp_seo.egg-info/top_level.txt
 seo/__init__.py
 seo/admin.py
 seo/lib.py
 seo/middleware.py
 seo/models.py
 seo/sitemaps.py
@@ -35,11 +33,10 @@
 seo/migrations/__init__.py
 seo/templates/403.html
 seo/templates/404.html
 seo/templates/500.html
 seo/templates/error.html
 seo/templates/language_meta_tags.html
 seo/templates/sitemap.html
-seo/templates/sitemetrics_tag.html
 seo/templates/sitemetrics/google.html
 seo/templatetags/__init__.py
 seo/templatetags/seo.py
```

### Comparing `django-mp-seo-9.0.2/seo/admin.py` & `django-mp-seo-9.0.3/seo/admin.py`

 * *Files identical despite different names*

### Comparing `django-mp-seo-9.0.2/seo/lib.py` & `django-mp-seo-9.0.3/seo/lib.py`

 * *Files identical despite different names*

### Comparing `django-mp-seo-9.0.2/seo/locale/ru/LC_MESSAGES/django.mo` & `django-mp-seo-9.0.3/seo/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-mp-seo-9.0.2/seo/locale/ru/LC_MESSAGES/django.po` & `django-mp-seo-9.0.3/seo/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-mp-seo-9.0.2/seo/locale/uk/LC_MESSAGES/django.mo` & `django-mp-seo-9.0.3/seo/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-mp-seo-9.0.2/seo/locale/uk/LC_MESSAGES/django.po` & `django-mp-seo-9.0.3/seo/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-mp-seo-9.0.2/seo/management/commands/sync_page_meta.py` & `django-mp-seo-9.0.3/seo/management/commands/sync_page_meta.py`

 * *Files identical despite different names*

### Comparing `django-mp-seo-9.0.2/seo/migrations/0001_initial.py` & `django-mp-seo-9.0.3/seo/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-mp-seo-9.0.2/seo/migrations/0002_auto_20190427_0832.py` & `django-mp-seo-9.0.3/seo/migrations/0002_auto_20190427_0832.py`

 * *Files identical despite different names*

### Comparing `django-mp-seo-9.0.2/seo/migrations/0003_auto_20190427_0906.py` & `django-mp-seo-9.0.3/seo/migrations/0003_auto_20190427_0906.py`

 * *Files identical despite different names*

### Comparing `django-mp-seo-9.0.2/seo/migrations/0007_search_query.py` & `django-mp-seo-9.0.3/seo/migrations/0007_search_query.py`

 * *Files identical despite different names*

### Comparing `django-mp-seo-9.0.2/seo/models.py` & `django-mp-seo-9.0.3/seo/models.py`

 * *Files identical despite different names*

### Comparing `django-mp-seo-9.0.2/seo/sitemaps.py` & `django-mp-seo-9.0.3/seo/sitemaps.py`

 * *Files identical despite different names*

### Comparing `django-mp-seo-9.0.2/seo/templates/error.html` & `django-mp-seo-9.0.3/seo/templates/error.html`

 * *Files identical despite different names*

### Comparing `django-mp-seo-9.0.2/seo/templates/sitemap.html` & `django-mp-seo-9.0.3/seo/templates/sitemap.html`

 * *Files identical despite different names*

### Comparing `django-mp-seo-9.0.2/seo/templatetags/seo.py` & `django-mp-seo-9.0.3/seo/templatetags/seo.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,12 +29,7 @@
 @register.simple_tag(takes_context=True)
 def get_favicon_tag(context, path=None):
 
     if path is None:
         path = context['STATIC_URL'] + 'img/favicon.ico'
 
     return mark_safe('<link rel="shortcut icon" href="{}">'.format(path))
-
-
-@register.inclusion_tag('sitemetrics_tag.html', takes_context=True)
-def sitemetrics(context):
-    return context
```

### Comparing `django-mp-seo-9.0.2/seo/views.py` & `django-mp-seo-9.0.3/seo/views.py`

 * *Files identical despite different names*

