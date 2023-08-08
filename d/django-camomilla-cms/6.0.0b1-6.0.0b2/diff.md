# Comparing `tmp/django-camomilla-cms-6.0.0b1.tar.gz` & `tmp/django-camomilla-cms-6.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-camomilla-cms-6.0.0b1.tar", last modified: Mon Jul 31 09:05:06 2023, max compression
+gzip compressed data, was "django-camomilla-cms-6.0.0b2.tar", last modified: Tue Aug  8 12:48:40 2023, max compression
```

## Comparing `django-camomilla-cms-6.0.0b1.tar` & `django-camomilla-cms-6.0.0b2.tar`

### file list

```diff
@@ -1,136 +1,148 @@
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.926345 django-camomilla-cms-6.0.0b1/
--rw-r--r--   0 bnznamco   (502) staff       (20)     1063 2023-03-28 16:06:29.000000 django-camomilla-cms-6.0.0b1/LICENSE
--rw-r--r--   0 bnznamco   (502) staff       (20)      224 2023-03-28 16:06:29.000000 django-camomilla-cms-6.0.0b1/MANIFEST.in
--rw-r--r--   0 bnznamco   (502) staff       (20)     1795 2023-07-31 09:05:06.926421 django-camomilla-cms-6.0.0b1/PKG-INFO
--rwxr-xr-x   0 bnznamco   (502) staff       (20)     1259 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/README.md
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.912175 django-camomilla-cms-6.0.0b1/camomilla/
--rwxr-xr-x   0 bnznamco   (502) staff       (20)      110 2023-07-31 09:03:58.000000 django-camomilla-cms-6.0.0b1/camomilla/__init__.py
--rwxr-xr-x   0 bnznamco   (502) staff       (20)     2557 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/admin.py
--rwxr-xr-x   0 bnznamco   (502) staff       (20)      497 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/apps.py
--rw-r--r--   0 bnznamco   (502) staff       (20)      855 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b1/camomilla/authentication.py
--rw-r--r--   0 bnznamco   (502) staff       (20)      165 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/context_processors.py
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.912317 django-camomilla-cms-6.0.0b1/camomilla/contrib/
--rw-r--r--   0 bnznamco   (502) staff       (20)        0 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/contrib/__init__.py
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.912546 django-camomilla-cms-6.0.0b1/camomilla/contrib/modeltranslation/
--rw-r--r--   0 bnznamco   (502) staff       (20)        0 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/contrib/modeltranslation/__init__.py
--rw-r--r--   0 bnznamco   (502) staff       (20)     4883 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/contrib/modeltranslation/hvad_migration.py
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.912836 django-camomilla-cms-6.0.0b1/camomilla/contrib/rest_framework/
--rw-r--r--   0 bnznamco   (502) staff       (20)        0 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/contrib/rest_framework/__init__.py
--rw-r--r--   0 bnznamco   (502) staff       (20)     2621 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/contrib/rest_framework/serializer.py
--rw-r--r--   0 bnznamco   (502) staff       (20)     1220 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b1/camomilla/defaults.py
--rw-r--r--   0 bnznamco   (502) staff       (20)      502 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/dynamic_pages_urls.py
--rw-r--r--   0 bnznamco   (502) staff       (20)      111 2023-03-28 16:06:29.000000 django-camomilla-cms-6.0.0b1/camomilla/exceptions.py
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.913092 django-camomilla-cms-6.0.0b1/camomilla/fields/
--rw-r--r--   0 bnznamco   (502) staff       (20)      400 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/fields/__init__.py
--rw-r--r--   0 bnznamco   (502) staff       (20)     1867 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/fields/json.py
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.913216 django-camomilla-cms-6.0.0b1/camomilla/management/
--rw-r--r--   0 bnznamco   (502) staff       (20)        0 2023-03-28 16:06:29.000000 django-camomilla-cms-6.0.0b1/camomilla/management/__init__.py
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.913470 django-camomilla-cms-6.0.0b1/camomilla/management/commands/
--rw-r--r--   0 bnznamco   (502) staff       (20)        0 2023-03-28 16:06:29.000000 django-camomilla-cms-6.0.0b1/camomilla/management/commands/__init__.py
--rw-r--r--   0 bnznamco   (502) staff       (20)      497 2023-07-18 12:13:50.000000 django-camomilla-cms-6.0.0b1/camomilla/management/commands/regenerate_thumbnails.py
--rw-r--r--   0 bnznamco   (502) staff       (20)     2222 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/model_api.py
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.914375 django-camomilla-cms-6.0.0b1/camomilla/models/
--rw-r--r--   0 bnznamco   (502) staff       (20)      151 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/models/__init__.py
--rw-r--r--   0 bnznamco   (502) staff       (20)     1194 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/models/article.py
--rw-r--r--   0 bnznamco   (502) staff       (20)      956 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/models/content.py
--rw-r--r--   0 bnznamco   (502) staff       (20)     6844 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/models/media.py
--rw-r--r--   0 bnznamco   (502) staff       (20)     2901 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/models/menu.py
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.914525 django-camomilla-cms-6.0.0b1/camomilla/models/mixins/
--rw-r--r--   0 bnznamco   (502) staff       (20)     1225 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/models/mixins/__init__.py
--rw-r--r--   0 bnznamco   (502) staff       (20)    11975 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/models/page.py
--rw-r--r--   0 bnznamco   (502) staff       (20)     1976 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b1/camomilla/parsers.py
--rwxr-xr-x   0 bnznamco   (502) staff       (20)     1813 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b1/camomilla/permissions.py
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.915799 django-camomilla-cms-6.0.0b1/camomilla/serializers/
--rw-r--r--   0 bnznamco   (502) staff       (20)      176 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/serializers/__init__.py
--rw-r--r--   0 bnznamco   (502) staff       (20)      401 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/serializers/article.py
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.915926 django-camomilla-cms-6.0.0b1/camomilla/serializers/base/
--rw-r--r--   0 bnznamco   (502) staff       (20)      488 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/serializers/base/__init__.py
--rw-r--r--   0 bnznamco   (502) staff       (20)      557 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/serializers/content_type.py
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.916461 django-camomilla-cms-6.0.0b1/camomilla/serializers/fields/
--rw-r--r--   0 bnznamco   (502) staff       (20)      528 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/serializers/fields/__init__.py
--rw-r--r--   0 bnznamco   (502) staff       (20)      648 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b1/camomilla/serializers/fields/file.py
--rw-r--r--   0 bnznamco   (502) staff       (20)     3474 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/serializers/fields/json.py
--rw-r--r--   0 bnznamco   (502) staff       (20)     4402 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b1/camomilla/serializers/fields/related.py
--rw-r--r--   0 bnznamco   (502) staff       (20)     1940 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/serializers/media.py
--rw-r--r--   0 bnznamco   (502) staff       (20)      552 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/serializers/menu.py
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.916614 django-camomilla-cms-6.0.0b1/camomilla/serializers/mixins/
--rw-r--r--   0 bnznamco   (502) staff       (20)     5555 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/serializers/mixins/__init__.py
--rw-r--r--   0 bnznamco   (502) staff       (20)      405 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/serializers/page.py
--rw-r--r--   0 bnznamco   (502) staff       (20)     3707 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/serializers/user.py
--rw-r--r--   0 bnznamco   (502) staff       (20)      875 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/serializers/utils.py
--rw-r--r--   0 bnznamco   (502) staff       (20)     1765 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/serializers/validators.py
--rw-r--r--   0 bnznamco   (502) staff       (20)     2565 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/settings.py
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.917052 django-camomilla-cms-6.0.0b1/camomilla/storages/
--rw-r--r--   0 bnznamco   (502) staff       (20)      131 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/storages/__init__.py
--rw-r--r--   0 bnznamco   (502) staff       (20)     1997 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/storages/optimize.py
--rw-r--r--   0 bnznamco   (502) staff       (20)      343 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/storages/overwrite.py
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.917544 django-camomilla-cms-6.0.0b1/camomilla/structured/
--rw-r--r--   0 bnznamco   (502) staff       (20)     3957 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/structured/__init__.py
--rw-r--r--   0 bnznamco   (502) staff       (20)     8475 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/structured/fields.py
--rw-r--r--   0 bnznamco   (502) staff       (20)     4759 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/structured/models.py
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.906836 django-camomilla-cms-6.0.0b1/camomilla/templates/
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.917708 django-camomilla-cms-6.0.0b1/camomilla/templates/defaults/
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.917890 django-camomilla-cms-6.0.0b1/camomilla/templates/defaults/articles/
--rw-r--r--   0 bnznamco   (502) staff       (20)      239 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/templates/defaults/articles/default.html
--rw-r--r--   0 bnznamco   (502) staff       (20)     6638 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/templates/defaults/base.html
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.918058 django-camomilla-cms-6.0.0b1/camomilla/templates/defaults/pages/
--rw-r--r--   0 bnznamco   (502) staff       (20)      144 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/templates/defaults/pages/default.html
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.918518 django-camomilla-cms-6.0.0b1/camomilla/templates/defaults/parts/
--rw-r--r--   0 bnznamco   (502) staff       (20)     2970 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/templates/defaults/parts/langswitch.html
--rw-r--r--   0 bnznamco   (502) staff       (20)      338 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/templates/defaults/parts/menu.html
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.918832 django-camomilla-cms-6.0.0b1/camomilla/templates/defaults/widgets/
--rw-r--r--   0 bnznamco   (502) staff       (20)     3727 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/templates/defaults/widgets/media_select_multiple.html
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.919334 django-camomilla-cms-6.0.0b1/camomilla/templatetags/
--rw-r--r--   0 bnznamco   (502) staff       (20)        0 2023-03-28 16:06:29.000000 django-camomilla-cms-6.0.0b1/camomilla/templatetags/__init__.py
--rw-r--r--   0 bnznamco   (502) staff       (20)      563 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/templatetags/camomilla_filters.py
--rw-r--r--   0 bnznamco   (502) staff       (20)      862 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/templatetags/menus.py
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.919474 django-camomilla-cms-6.0.0b1/camomilla/theme/
--rwxr-xr-x   0 bnznamco   (502) staff       (20)       29 2023-07-31 09:03:58.000000 django-camomilla-cms-6.0.0b1/camomilla/theme/__init__.py
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.907704 django-camomilla-cms-6.0.0b1/camomilla/theme/static/
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.907873 django-camomilla-cms-6.0.0b1/camomilla/theme/static/admin/
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.919632 django-camomilla-cms-6.0.0b1/camomilla/theme/static/admin/css/
--rwxr-xr-x   0 bnznamco   (502) staff       (20)    16681 2023-07-20 08:16:23.000000 django-camomilla-cms-6.0.0b1/camomilla/theme/static/admin/css/responsive.css
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.920109 django-camomilla-cms-6.0.0b1/camomilla/theme/static/admin/img/
--rw-r--r--   0 bnznamco   (502) staff       (20)    18821 2023-03-28 16:06:29.000000 django-camomilla-cms-6.0.0b1/camomilla/theme/static/admin/img/logo.png
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.908058 django-camomilla-cms-6.0.0b1/camomilla/theme/templates/
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.920855 django-camomilla-cms-6.0.0b1/camomilla/theme/templates/admin/
--rwxr-xr-x   0 bnznamco   (502) staff       (20)      585 2023-07-20 08:16:25.000000 django-camomilla-cms-6.0.0b1/camomilla/theme/templates/admin/base_site.html
--rw-r--r--   0 bnznamco   (502) staff       (20)     1261 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/translation.py
--rwxr-xr-x   0 bnznamco   (502) staff       (20)     1716 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/urls.py
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.921934 django-camomilla-cms-6.0.0b1/camomilla/utils/
--rw-r--r--   0 bnznamco   (502) staff       (20)       74 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/utils/__init__.py
--rw-r--r--   0 bnznamco   (502) staff       (20)      520 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/utils/getters.py
--rw-r--r--   0 bnznamco   (502) staff       (20)      255 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/utils/normalization.py
--rw-r--r--   0 bnznamco   (502) staff       (20)     3324 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/utils/seo.py
--rw-r--r--   0 bnznamco   (502) staff       (20)     2273 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/utils/translation.py
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.923313 django-camomilla-cms-6.0.0b1/camomilla/views/
--rw-r--r--   0 bnznamco   (502) staff       (20)      177 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/views/__init__.py
--rw-r--r--   0 bnznamco   (502) staff       (20)      572 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/views/articles.py
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.923473 django-camomilla-cms-6.0.0b1/camomilla/views/base/
--rw-r--r--   0 bnznamco   (502) staff       (20)      222 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b1/camomilla/views/base/__init__.py
--rw-r--r--   0 bnznamco   (502) staff       (20)     1206 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/views/contents.py
--rw-r--r--   0 bnznamco   (502) staff       (20)      441 2023-03-28 16:06:29.000000 django-camomilla-cms-6.0.0b1/camomilla/views/languages.py
--rw-r--r--   0 bnznamco   (502) staff       (20)     3002 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/views/medias.py
--rw-r--r--   0 bnznamco   (502) staff       (20)     1686 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/views/menus.py
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.923892 django-camomilla-cms-6.0.0b1/camomilla/views/mixins/
--rw-r--r--   0 bnznamco   (502) staff       (20)     2438 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/views/mixins/__init__.py
--rw-r--r--   0 bnznamco   (502) staff       (20)     4779 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/views/mixins/ordering.py
--rw-r--r--   0 bnznamco   (502) staff       (20)     5956 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b1/camomilla/views/mixins/pagination.py
--rw-r--r--   0 bnznamco   (502) staff       (20)      486 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/views/pages.py
--rw-r--r--   0 bnznamco   (502) staff       (20)      480 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/views/tags.py
--rw-r--r--   0 bnznamco   (502) staff       (20)     3132 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/camomilla/views/users.py
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.924633 django-camomilla-cms-6.0.0b1/django_camomilla_cms.egg-info/
--rw-r--r--   0 bnznamco   (502) staff       (20)     1795 2023-07-31 09:05:06.000000 django-camomilla-cms-6.0.0b1/django_camomilla_cms.egg-info/PKG-INFO
--rw-r--r--   0 bnznamco   (502) staff       (20)     3135 2023-07-31 09:05:06.000000 django-camomilla-cms-6.0.0b1/django_camomilla_cms.egg-info/SOURCES.txt
--rw-r--r--   0 bnznamco   (502) staff       (20)        1 2023-07-31 09:05:06.000000 django-camomilla-cms-6.0.0b1/django_camomilla_cms.egg-info/dependency_links.txt
--rw-r--r--   0 bnznamco   (502) staff       (20)      219 2023-07-31 09:05:06.000000 django-camomilla-cms-6.0.0b1/django_camomilla_cms.egg-info/requires.txt
--rw-r--r--   0 bnznamco   (502) staff       (20)       16 2023-07-31 09:05:06.000000 django-camomilla-cms-6.0.0b1/django_camomilla_cms.egg-info/top_level.txt
--rw-r--r--   0 bnznamco   (502) staff       (20)     1018 2023-07-31 09:05:06.926745 django-camomilla-cms-6.0.0b1/setup.cfg
--rw-r--r--   0 bnznamco   (502) staff       (20)       87 2023-07-31 09:03:58.000000 django-camomilla-cms-6.0.0b1/setup.py
-drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-07-31 09:05:06.926200 django-camomilla-cms-6.0.0b1/tests/
--rw-r--r--   0 bnznamco   (502) staff       (20)        0 2023-03-28 16:06:29.000000 django-camomilla-cms-6.0.0b1/tests/__init__.py
--rw-r--r--   0 bnznamco   (502) staff       (20)     2347 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b1/tests/test_api.py
--rw-r--r--   0 bnznamco   (502) staff       (20)     1848 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b1/tests/test_camomilla_filters.py
--rw-r--r--   0 bnznamco   (502) staff       (20)      684 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b1/tests/test_models.py
--rw-r--r--   0 bnznamco   (502) staff       (20)     3613 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b1/tests/test_utils.py
--rw-r--r--   0 bnznamco   (502) staff       (20)      562 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b1/tests/urls.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.138134 django-camomilla-cms-6.0.0b2/
+-rw-r--r--   0 bnznamco   (502) staff       (20)     1063 2023-03-28 16:06:29.000000 django-camomilla-cms-6.0.0b2/LICENSE
+-rw-r--r--   0 bnznamco   (502) staff       (20)      224 2023-03-28 16:06:29.000000 django-camomilla-cms-6.0.0b2/MANIFEST.in
+-rw-r--r--   0 bnznamco   (502) staff       (20)     1985 2023-08-08 12:48:40.138219 django-camomilla-cms-6.0.0b2/PKG-INFO
+-rwxr-xr-x   0 bnznamco   (502) staff       (20)     1449 2023-08-02 15:02:55.000000 django-camomilla-cms-6.0.0b2/README.md
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.124419 django-camomilla-cms-6.0.0b2/camomilla/
+-rwxr-xr-x   0 bnznamco   (502) staff       (20)      110 2023-08-08 12:48:35.000000 django-camomilla-cms-6.0.0b2/camomilla/__init__.py
+-rwxr-xr-x   0 bnznamco   (502) staff       (20)     2404 2023-08-04 11:55:05.000000 django-camomilla-cms-6.0.0b2/camomilla/admin.py
+-rwxr-xr-x   0 bnznamco   (502) staff       (20)      497 2023-08-04 09:04:01.000000 django-camomilla-cms-6.0.0b2/camomilla/apps.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      855 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b2/camomilla/authentication.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      165 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/context_processors.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.124551 django-camomilla-cms-6.0.0b2/camomilla/contrib/
+-rw-r--r--   0 bnznamco   (502) staff       (20)        0 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/contrib/__init__.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.124831 django-camomilla-cms-6.0.0b2/camomilla/contrib/modeltranslation/
+-rw-r--r--   0 bnznamco   (502) staff       (20)        0 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/contrib/modeltranslation/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     4883 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/contrib/modeltranslation/hvad_migration.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.125095 django-camomilla-cms-6.0.0b2/camomilla/contrib/rest_framework/
+-rw-r--r--   0 bnznamco   (502) staff       (20)        0 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/contrib/rest_framework/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     2834 2023-08-08 12:44:20.000000 django-camomilla-cms-6.0.0b2/camomilla/contrib/rest_framework/serializer.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     1220 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b2/camomilla/defaults.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      605 2023-08-04 11:55:18.000000 django-camomilla-cms-6.0.0b2/camomilla/dynamic_pages_urls.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      111 2023-03-28 16:06:29.000000 django-camomilla-cms-6.0.0b2/camomilla/exceptions.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.125343 django-camomilla-cms-6.0.0b2/camomilla/fields/
+-rw-r--r--   0 bnznamco   (502) staff       (20)      400 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/fields/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     1867 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/fields/json.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.125471 django-camomilla-cms-6.0.0b2/camomilla/management/
+-rw-r--r--   0 bnznamco   (502) staff       (20)        0 2023-03-28 16:06:29.000000 django-camomilla-cms-6.0.0b2/camomilla/management/__init__.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.125719 django-camomilla-cms-6.0.0b2/camomilla/management/commands/
+-rw-r--r--   0 bnznamco   (502) staff       (20)        0 2023-03-28 16:06:29.000000 django-camomilla-cms-6.0.0b2/camomilla/management/commands/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      497 2023-07-18 12:13:50.000000 django-camomilla-cms-6.0.0b2/camomilla/management/commands/regenerate_thumbnails.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     2222 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/model_api.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.126586 django-camomilla-cms-6.0.0b2/camomilla/models/
+-rw-r--r--   0 bnznamco   (502) staff       (20)      151 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/models/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     1194 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/models/article.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      956 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/models/content.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     6909 2023-08-04 15:45:32.000000 django-camomilla-cms-6.0.0b2/camomilla/models/media.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     2901 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/models/menu.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.126747 django-camomilla-cms-6.0.0b2/camomilla/models/mixins/
+-rw-r--r--   0 bnznamco   (502) staff       (20)     1249 2023-08-04 09:56:23.000000 django-camomilla-cms-6.0.0b2/camomilla/models/mixins/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)    12438 2023-08-07 15:27:11.000000 django-camomilla-cms-6.0.0b2/camomilla/models/page.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.127014 django-camomilla-cms-6.0.0b2/camomilla/openapi/
+-rw-r--r--   0 bnznamco   (502) staff       (20)        0 2023-08-07 07:04:38.000000 django-camomilla-cms-6.0.0b2/camomilla/openapi/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     1087 2023-08-07 15:23:40.000000 django-camomilla-cms-6.0.0b2/camomilla/openapi/schema.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     1976 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b2/camomilla/parsers.py
+-rwxr-xr-x   0 bnznamco   (502) staff       (20)     1813 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b2/camomilla/permissions.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.128263 django-camomilla-cms-6.0.0b2/camomilla/serializers/
+-rw-r--r--   0 bnznamco   (502) staff       (20)      176 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/serializers/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      401 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/serializers/article.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.128418 django-camomilla-cms-6.0.0b2/camomilla/serializers/base/
+-rw-r--r--   0 bnznamco   (502) staff       (20)      488 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/serializers/base/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      557 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/serializers/content_type.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.129004 django-camomilla-cms-6.0.0b2/camomilla/serializers/fields/
+-rw-r--r--   0 bnznamco   (502) staff       (20)      528 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/serializers/fields/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      648 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b2/camomilla/serializers/fields/file.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     3474 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/serializers/fields/json.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     4402 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b2/camomilla/serializers/fields/related.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     1940 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/serializers/media.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      552 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/serializers/menu.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.129139 django-camomilla-cms-6.0.0b2/camomilla/serializers/mixins/
+-rw-r--r--   0 bnznamco   (502) staff       (20)     5503 2023-08-07 15:01:44.000000 django-camomilla-cms-6.0.0b2/camomilla/serializers/mixins/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      405 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/serializers/page.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     3707 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/serializers/user.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      875 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/serializers/utils.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     1775 2023-08-07 15:00:01.000000 django-camomilla-cms-6.0.0b2/camomilla/serializers/validators.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     2699 2023-08-01 14:38:15.000000 django-camomilla-cms-6.0.0b2/camomilla/settings.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.129558 django-camomilla-cms-6.0.0b2/camomilla/storages/
+-rw-r--r--   0 bnznamco   (502) staff       (20)      131 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/storages/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     1997 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/storages/optimize.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      343 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/storages/overwrite.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.130101 django-camomilla-cms-6.0.0b2/camomilla/structured/
+-rw-r--r--   0 bnznamco   (502) staff       (20)     3957 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/structured/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     8475 2023-08-08 12:45:57.000000 django-camomilla-cms-6.0.0b2/camomilla/structured/fields.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     4759 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/structured/models.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.120072 django-camomilla-cms-6.0.0b2/camomilla/templates/
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.119947 django-camomilla-cms-6.0.0b2/camomilla/templates/admin/
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.119995 django-camomilla-cms-6.0.0b2/camomilla/templates/admin/camomilla/
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.130257 django-camomilla-cms-6.0.0b2/camomilla/templates/admin/camomilla/page/
+-rw-r--r--   0 bnznamco   (502) staff       (20)      251 2023-08-04 11:54:25.000000 django-camomilla-cms-6.0.0b2/camomilla/templates/admin/camomilla/page/change_form.html
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.130411 django-camomilla-cms-6.0.0b2/camomilla/templates/defaults/
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.130552 django-camomilla-cms-6.0.0b2/camomilla/templates/defaults/articles/
+-rw-r--r--   0 bnznamco   (502) staff       (20)      239 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/templates/defaults/articles/default.html
+-rw-r--r--   0 bnznamco   (502) staff       (20)     6638 2023-08-04 14:41:01.000000 django-camomilla-cms-6.0.0b2/camomilla/templates/defaults/base.html
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.130690 django-camomilla-cms-6.0.0b2/camomilla/templates/defaults/pages/
+-rw-r--r--   0 bnznamco   (502) staff       (20)      144 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/templates/defaults/pages/default.html
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.131145 django-camomilla-cms-6.0.0b2/camomilla/templates/defaults/parts/
+-rw-r--r--   0 bnznamco   (502) staff       (20)     2970 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/templates/defaults/parts/langswitch.html
+-rw-r--r--   0 bnznamco   (502) staff       (20)      338 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/templates/defaults/parts/menu.html
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.131367 django-camomilla-cms-6.0.0b2/camomilla/templates/defaults/widgets/
+-rw-r--r--   0 bnznamco   (502) staff       (20)     3727 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/templates/defaults/widgets/media_select_multiple.html
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.131981 django-camomilla-cms-6.0.0b2/camomilla/templatetags/
+-rw-r--r--   0 bnznamco   (502) staff       (20)        0 2023-08-04 07:33:48.000000 django-camomilla-cms-6.0.0b2/camomilla/templatetags/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      563 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/templatetags/camomilla_filters.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      862 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/templatetags/menus.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.132301 django-camomilla-cms-6.0.0b2/camomilla/theme/
+-rwxr-xr-x   0 bnznamco   (502) staff       (20)       29 2023-08-08 12:48:35.000000 django-camomilla-cms-6.0.0b2/camomilla/theme/__init__.py
+-rwxr-xr-x   0 bnznamco   (502) staff       (20)      991 2023-08-02 14:52:35.000000 django-camomilla-cms-6.0.0b2/camomilla/theme/apps.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.120754 django-camomilla-cms-6.0.0b2/camomilla/theme/static/
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.120880 django-camomilla-cms-6.0.0b2/camomilla/theme/static/admin/
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.132441 django-camomilla-cms-6.0.0b2/camomilla/theme/static/admin/css/
+-rwxr-xr-x   0 bnznamco   (502) staff       (20)      157 2023-08-04 08:12:18.000000 django-camomilla-cms-6.0.0b2/camomilla/theme/static/admin/css/responsive.css
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.132742 django-camomilla-cms-6.0.0b2/camomilla/theme/static/admin/img/
+-rw-rw-r--   0 bnznamco   (502) staff       (20)    15406 2023-08-04 14:36:07.000000 django-camomilla-cms-6.0.0b2/camomilla/theme/static/admin/img/favicon.ico
+-rw-r--r--   0 bnznamco   (502) staff       (20)     3238 2023-08-02 14:15:30.000000 django-camomilla-cms-6.0.0b2/camomilla/theme/static/admin/img/logo.svg
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.121077 django-camomilla-cms-6.0.0b2/camomilla/theme/templates/
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.132882 django-camomilla-cms-6.0.0b2/camomilla/theme/templates/admin/
+-rwxr-xr-x   0 bnznamco   (502) staff       (20)      254 2023-08-04 14:39:20.000000 django-camomilla-cms-6.0.0b2/camomilla/theme/templates/admin/base.html
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.133034 django-camomilla-cms-6.0.0b2/camomilla/theme/templates/rosetta/
+-rwxr-xr-x   0 bnznamco   (502) staff       (20)    16731 2023-08-04 08:10:01.000000 django-camomilla-cms-6.0.0b2/camomilla/theme/templates/rosetta/base.html
+-rw-r--r--   0 bnznamco   (502) staff       (20)     1261 2023-08-02 14:47:16.000000 django-camomilla-cms-6.0.0b2/camomilla/translation.py
+-rwxr-xr-x   0 bnznamco   (502) staff       (20)     2026 2023-08-07 07:06:35.000000 django-camomilla-cms-6.0.0b2/camomilla/urls.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.134407 django-camomilla-cms-6.0.0b2/camomilla/utils/
+-rw-r--r--   0 bnznamco   (502) staff       (20)       99 2023-08-02 16:08:37.000000 django-camomilla-cms-6.0.0b2/camomilla/utils/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      520 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/utils/getters.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      255 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/utils/normalization.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     3324 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/utils/seo.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      598 2023-08-04 09:22:09.000000 django-camomilla-cms-6.0.0b2/camomilla/utils/templates.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     2426 2023-08-07 08:58:27.000000 django-camomilla-cms-6.0.0b2/camomilla/utils/translation.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.135928 django-camomilla-cms-6.0.0b2/camomilla/views/
+-rw-r--r--   0 bnznamco   (502) staff       (20)      177 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/views/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      572 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/views/articles.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.136083 django-camomilla-cms-6.0.0b2/camomilla/views/base/
+-rw-r--r--   0 bnznamco   (502) staff       (20)      222 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b2/camomilla/views/base/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     1206 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/views/contents.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      441 2023-03-28 16:06:29.000000 django-camomilla-cms-6.0.0b2/camomilla/views/languages.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     3002 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/views/medias.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     1686 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/views/menus.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.136554 django-camomilla-cms-6.0.0b2/camomilla/views/mixins/
+-rw-r--r--   0 bnznamco   (502) staff       (20)     2438 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/views/mixins/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     4779 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/views/mixins/ordering.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     5956 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b2/camomilla/views/mixins/pagination.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      486 2023-08-07 15:28:21.000000 django-camomilla-cms-6.0.0b2/camomilla/views/pages.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      480 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/views/tags.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     3132 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/camomilla/views/users.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.137243 django-camomilla-cms-6.0.0b2/django_camomilla_cms.egg-info/
+-rw-r--r--   0 bnznamco   (502) staff       (20)     1985 2023-08-08 12:48:40.000000 django-camomilla-cms-6.0.0b2/django_camomilla_cms.egg-info/PKG-INFO
+-rw-r--r--   0 bnznamco   (502) staff       (20)     3388 2023-08-08 12:48:40.000000 django-camomilla-cms-6.0.0b2/django_camomilla_cms.egg-info/SOURCES.txt
+-rw-r--r--   0 bnznamco   (502) staff       (20)        1 2023-08-08 12:48:40.000000 django-camomilla-cms-6.0.0b2/django_camomilla_cms.egg-info/dependency_links.txt
+-rw-r--r--   0 bnznamco   (502) staff       (20)      235 2023-08-08 12:48:40.000000 django-camomilla-cms-6.0.0b2/django_camomilla_cms.egg-info/requires.txt
+-rw-r--r--   0 bnznamco   (502) staff       (20)       16 2023-08-08 12:48:40.000000 django-camomilla-cms-6.0.0b2/django_camomilla_cms.egg-info/top_level.txt
+-rw-r--r--   0 bnznamco   (502) staff       (20)     1034 2023-08-08 12:48:40.138571 django-camomilla-cms-6.0.0b2/setup.cfg
+-rw-r--r--   0 bnznamco   (502) staff       (20)       87 2023-08-08 12:48:35.000000 django-camomilla-cms-6.0.0b2/setup.py
+drwxr-xr-x   0 bnznamco   (502) staff       (20)        0 2023-08-08 12:48:40.138020 django-camomilla-cms-6.0.0b2/tests/
+-rw-r--r--   0 bnznamco   (502) staff       (20)        0 2023-03-28 16:06:29.000000 django-camomilla-cms-6.0.0b2/tests/__init__.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     2347 2023-07-31 08:40:08.000000 django-camomilla-cms-6.0.0b2/tests/test_api.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     1848 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b2/tests/test_camomilla_filters.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      684 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b2/tests/test_models.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)     3613 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b2/tests/test_utils.py
+-rw-r--r--   0 bnznamco   (502) staff       (20)      562 2023-06-21 09:17:27.000000 django-camomilla-cms-6.0.0b2/tests/urls.py
```

### Comparing `django-camomilla-cms-6.0.0b1/LICENSE` & `django-camomilla-cms-6.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/PKG-INFO` & `django-camomilla-cms-6.0.0b2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-camomilla-cms
-Version: 6.0.0b1
+Version: 6.0.0b2
 Summary: Django powered cms
 Home-page: https://github.com/lotrekagency/camomilla
 Author: Lotrèk
 Author-email: dimmitutto@lotrek.it
 License: MIT
 Keywords: cms,django,api cms
 Classifier: Environment :: Web Environment
@@ -40,21 +40,20 @@
     from camomilla.defaults import *
 
 Remember to add all the required applications in your project
 
 ```python
 INSTALLED_APPS = [
     ...
-    'camomilla',
-    'camomilla.theme',
-    'djsuperadmin',
-    'modeltranslation',
-    'djlotrek',
-    'rest_framework',
-    'rest_framework.authtoken',
+    'camomilla', # always needed
+    'camomilla.theme', # needed to customize admin interface
+    'djsuperadmin', # needed if you whant to use djsuperadmin for contents
+    'modeltranslation', # needed if your website is multilanguage (can be added later)
+    'rest_framework',  # always needed
+    'rest_framework.authtoken',  # always needed
     ...
 ]
 ```
 
 ## Run the server
 
     $ python manage.py runserver
```

### Comparing `django-camomilla-cms-6.0.0b1/README.md` & `django-camomilla-cms-6.0.0b2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -22,21 +22,20 @@
     from camomilla.defaults import *
 
 Remember to add all the required applications in your project
 
 ```python
 INSTALLED_APPS = [
     ...
-    'camomilla',
-    'camomilla.theme',
-    'djsuperadmin',
-    'modeltranslation',
-    'djlotrek',
-    'rest_framework',
-    'rest_framework.authtoken',
+    'camomilla', # always needed
+    'camomilla.theme', # needed to customize admin interface
+    'djsuperadmin', # needed if you whant to use djsuperadmin for contents
+    'modeltranslation', # needed if your website is multilanguage (can be added later)
+    'rest_framework',  # always needed
+    'rest_framework.authtoken',  # always needed
     ...
 ]
 ```
 
 ## Run the server
 
     $ python manage.py runserver
```

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/authentication.py` & `django-camomilla-cms-6.0.0b2/camomilla/authentication.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/contrib/modeltranslation/hvad_migration.py` & `django-camomilla-cms-6.0.0b2/camomilla/contrib/modeltranslation/hvad_migration.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/defaults.py` & `django-camomilla-cms-6.0.0b2/camomilla/defaults.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/fields/json.py` & `django-camomilla-cms-6.0.0b2/camomilla/fields/json.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/model_api.py` & `django-camomilla-cms-6.0.0b2/camomilla/model_api.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/models/article.py` & `django-camomilla-cms-6.0.0b2/camomilla/models/article.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/models/content.py` & `django-camomilla-cms-6.0.0b2/camomilla/models/content.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/models/media.py` & `django-camomilla-cms-6.0.0b2/camomilla/models/media.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 class AbstractMediaFolder(models.Model):
     title = models.CharField(max_length=200)
     slug = models.SlugField(editable=False, max_length=200, blank=True, null=True)
     creation_date = models.DateTimeField(auto_now_add=True)
     last_modified = models.DateTimeField(auto_now=True)
-    path = models.TextField(blank=True, null=True)
+    path = models.TextField(blank=True, null=True, editable=False)
     updir = models.ForeignKey(
         "self",
         on_delete=models.CASCADE,
         related_name="child_folders",
         null=True,
         blank=True,
     )
@@ -50,15 +50,15 @@
         else:
             self.path = "/{0}".format(self.slug)
 
         super().save(*args, **kwargs)
         self.update_childs()
 
     def __str__(self):
-        return "[%s] %s" % (self.__class__.__name__, self.name)
+        return "[%s] %s" % (self.__class__.__name__, self.title)
 
 
 class MediaFolder(AbstractMediaFolder):
     pass
 
 
 class Media(models.Model):
@@ -71,17 +71,17 @@
     thumbnail = models.ImageField(
         upload_to=THUMBNAIL_FOLDER,
         max_length=500,
         null=True,
         blank=True,
     )
     created = models.DateTimeField(auto_now=True)
-    size = models.IntegerField(default=0, blank=True, null=True)
-    mime_type = models.CharField(max_length=128, blank=True, null=True)
-    image_props = JSONField(default=dict, blank=True)
+    size = models.IntegerField(default=0, blank=True, null=True, editable=False)
+    mime_type = models.CharField(max_length=128, blank=True, null=True, editable=False)
+    image_props = JSONField(default=dict, blank=True, editable=False)
     folder = models.ForeignKey(
         MediaFolder,
         null=True,
         blank=True,
         related_name="media_folder",
         on_delete=models.CASCADE,
     )
```

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/models/menu.py` & `django-camomilla-cms-6.0.0b2/camomilla/models/menu.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/models/mixins/__init__.py` & `django-camomilla-cms-6.0.0b2/camomilla/models/mixins/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     )
 
     class Meta:
         abstract = True
 
 
 class MetaMixin(models.Model):
-    meta = models.JSONField(default=dict)
+    meta = models.JSONField(default=dict, null=False, blank=True)
 
     def get_meta(self, key, default=None):
         return self.meta.get(key, default)
 
     def update_meta(self, key, value):
         self.meta[key] = value
         super(MetaMixin, self).save(update_fields=["meta"])
```

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/models/page.py` & `django-camomilla-cms-6.0.0b2/camomilla/models/page.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,29 +4,34 @@
 from django.core.exceptions import ObjectDoesNotExist
 from django.db import ProgrammingError, OperationalError, models, transaction
 from django.db.models.signals import post_delete
 from django.dispatch import receiver
 from django.http import Http404
 from django.urls import NoReverseMatch, reverse
 from django.utils import timezone
+from django.utils.functional import lazy
 from django.utils.text import slugify
 from django.utils.translation import gettext_lazy as _
 
 from camomilla.models.mixins import MetaMixin, SeoMixin
 from camomilla.utils import (
     activate_languages,
     get_field_translations,
     get_nofallbacks,
     lang_fallback_query,
     set_nofallbacks,
     url_lang_decompose,
+    get_all_templates_files
 )
 from camomilla.utils.getters import pointed_getter
 from camomilla import settings
 
+def GET_TEMPLATE_CHOICES():
+    return [(t,t)for t in get_all_templates_files()]
+
 
 class UrlNodeManager(models.Manager):
     @property
     def related_names(self):
         self._related_names = getattr(
             self,
             "_related_names",
@@ -114,36 +119,40 @@
         return new_class
 
 
 class AbstractPage(SeoMixin, MetaMixin, models.Model, metaclass=PageBase):
     date_created = models.DateTimeField(auto_now_add=True)
     date_updated_at = models.DateTimeField(auto_now=True)
     url_node = models.OneToOneField(
-        UrlNode, on_delete=models.CASCADE, related_name=URL_NODE_RELATED_NAME, null=True
+        UrlNode, on_delete=models.CASCADE, related_name=URL_NODE_RELATED_NAME, null=True, editable=False
     )
     breadcrumbs_title = models.CharField(max_length=128, null=True, blank=True)
     slug = models.SlugField(max_length=150, allow_unicode=True, null=True, blank=True)
     status = models.CharField(
         max_length=3,
         choices=PAGE_STATUS,
         default="DRF",
     )
-    template = models.CharField(max_length=500, null=True, blank=True)
-    template_data = models.JSONField(default=dict)
-    identifier = models.CharField(max_length=200, null=True, unique=True)
+    template = models.CharField(max_length=500, null=True, blank=True, choices=[])
+    template_data = models.JSONField(default=dict, null=False, blank=True)
+    identifier = models.CharField(max_length=200, null=True, unique=True, default=uuid4)
     pubblication_date = models.DateTimeField(null=True, blank=True)
     indexable = models.BooleanField(default=True)
     ordering = models.PositiveIntegerField(default=0, blank=False, null=False)
     parent_page = models.ForeignKey(
         "self",
         related_name=PAGE_CHILD_RELATED_NAME,
         null=True,
         blank=True,
         on_delete=models.CASCADE,
     )
+    
+    def __init__(self, *args, **kwargs):
+        super(AbstractPage, self).__init__(*args, **kwargs)
+        self._meta.get_field('template').choices = lazy(GET_TEMPLATE_CHOICES,list)()
 
     def __str__(self) -> str:
         return "(%s) %s" % (self.__class__.__name__, self.title or self.permalink)
 
     def get_context(self, request=None):
         context={
             "page": self,
@@ -219,30 +228,30 @@
             force = force or old_permalink != new_permalink
             set_nofallbacks(self.url_node, "permalink", new_permalink)
         if force:
             self.url_node.save()
             self.update_childs()
         return self.url_node
 
-    def generate_permalink(self) -> str:
+    def generate_permalink(self, safe:bool=True) -> str:
         slug = get_nofallbacks(self, "slug")
-        if slug is None:
+        if slug is None and not self.permalink:
             translations = get_field_translations(self, "slug").values()
             fallback_slug = next((t for t in translations if t is not None), None)
             slug = (
                 slugify(self.title or uuid4(), allow_unicode=True)
                 if fallback_slug is None
                 else fallback_slug
             )
             set_nofallbacks(self, "slug", slug)
-        permalink = "/%s" % slugify(slug, allow_unicode=True)
+        permalink = "/%s" % slugify(slug or "", allow_unicode=True)
         if self.parent:
             permalink = f"{self.parent.permalink}{permalink}"
         qs = UrlNode.objects.exclude(pk=getattr(self.url_node or object, "pk", None))
-        if qs.filter(permalink=permalink).exists():
+        if safe and qs.filter(permalink=permalink).exists():
             permalink = "/".join(
                 permalink.split("/")[:-1] + [slugify(uuid4(), allow_unicode=True)]
             )
         return permalink
 
     def update_childs(self) -> None:
         # without pk, no childs there
```

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/parsers.py` & `django-camomilla-cms-6.0.0b2/camomilla/parsers.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/permissions.py` & `django-camomilla-cms-6.0.0b2/camomilla/permissions.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/serializers/content_type.py` & `django-camomilla-cms-6.0.0b2/camomilla/serializers/content_type.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/serializers/fields/__init__.py` & `django-camomilla-cms-6.0.0b2/camomilla/serializers/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/serializers/fields/file.py` & `django-camomilla-cms-6.0.0b2/camomilla/serializers/fields/file.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/serializers/fields/json.py` & `django-camomilla-cms-6.0.0b2/camomilla/serializers/fields/json.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/serializers/fields/related.py` & `django-camomilla-cms-6.0.0b2/camomilla/serializers/fields/related.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/serializers/media.py` & `django-camomilla-cms-6.0.0b2/camomilla/serializers/media.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/serializers/menu.py` & `django-camomilla-cms-6.0.0b2/camomilla/serializers/menu.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/serializers/mixins/__init__.py` & `django-camomilla-cms-6.0.0b2/camomilla/serializers/mixins/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 import django
-from django.conf import settings
+from django.conf import settings as django_settings
 from django.db.models.aggregates import Max
 from django.db.models.functions import Coalesce
 from django.utils import translation
 from modeltranslation.settings import AVAILABLE_LANGUAGES
 from modeltranslation.utils import build_localized_fieldname
 from rest_framework import serializers
 from rest_framework.utils import model_meta
 
 from camomilla.fields import ORDERING_ACCEPTED_FIELDS
 from camomilla.serializers.fields.related import RelatedField
 from camomilla.serializers.utils import build_standard_model_serializer
 from camomilla.serializers.validators import UniquePermalinkValidator
 from camomilla.utils import dict_merge
-from camomilla.settings import ENABLE_TRANSLATIONS
+from camomilla import settings
 
 if django.VERSION >= (4, 0):
     from django.db.models import JSONField as DjangoJSONField
 else:
     from django.contrib.postgres.fields import JSONField as DjangoJSONField
 
 
 # TODO: decide what to do with LangInfoMixin mixin!
 class LangInfoMixin(metaclass=serializers.SerializerMetaclass):
     lang_info = serializers.SerializerMethodField("get_lang_info", read_only=True)
 
     def get_lang_info(self, obj, *args, **kwargs):
         languages = []
-        for key, language in settings.LANGUAGES:
+        for key, language in django_settings.LANGUAGES:
             languages.append({"id": key, "name": language})
         return {
-            "default": settings.LANGUAGE_CODE,
+            "default": django_settings.LANGUAGE_CODE,
             "active": translation.get_language(),
             "site_languages": languages,
         }
 
     def get_default_field_names(self, *args):
         field_names = super().get_default_field_names(*args)
         self.action = getattr(
@@ -93,27 +93,24 @@
                 if self.is_json_field(attr, value, info):
                     validated_data[attr] = dict_merge(
                         getattr(instance, attr, {}), value
                     )
         return super().update(instance, validated_data)
 
 
-DEFAULT_NESTING_DEPTH = getattr(settings, "CAMOMILLA_DRF_NESTING_DEPTH", 10)
-
-
 class NestMixin:
     def __init__(self, *args, **kwargs):
         self._depth = kwargs.pop("depth", None)
         return super().__init__(*args, **kwargs)
 
     def build_nested_field(self, field_name, relation_info, nested_depth):
         return self.build_relational_field(field_name, relation_info, nested_depth)
 
     def build_relational_field(
-        self, field_name, relation_info, nested_depth=DEFAULT_NESTING_DEPTH + 1
+        self, field_name, relation_info, nested_depth=settings.API_NESTING_DEPTH + 1
     ):
         nested_depth = nested_depth if self._depth is None else self._depth
         field_class, field_kwargs = super().build_relational_field(
             field_name, relation_info
         )
         if (
             field_class is RelatedField and nested_depth > 1
@@ -125,15 +122,15 @@
 
 
 
 class AbstractPageMixin(serializers.ModelSerializer):
     LANG_PERMALINK_FIELDS = [
         build_localized_fieldname("permalink", lang)
         for lang in AVAILABLE_LANGUAGES
-        if ENABLE_TRANSLATIONS
+        if settings.ENABLE_TRANSLATIONS
     ]
 
     @property
     def translation_fields(self):
         return super().translation_fields + ["permalink"]
 
     def get_default_field_names(self, *args):
```

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/serializers/user.py` & `django-camomilla-cms-6.0.0b2/camomilla/serializers/user.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/serializers/utils.py` & `django-camomilla-cms-6.0.0b2/camomilla/serializers/utils.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/serializers/validators.py` & `django-camomilla-cms-6.0.0b2/camomilla/serializers/validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,13 +31,13 @@
         for language in activate_languages():
             f_name = build_localized_fieldname("slug", language)
             slug = value.get(f_name, instance and get_nofallbacks(instance, "slug"))
             fake_instance = serializer.Meta.model()
             set_nofallbacks(fake_instance, "slug", slug)
             if parent_page:
                 set_nofallbacks(fake_instance, parent_page_field, parent_page)
-            permalink = fake_instance.generate_permalink()
+            permalink = fake_instance.generate_permalink(safe=False)
             qs = UrlNode.objects.exclude(**exclude_kwargs)
             if qs.filter(permalink=permalink).exists():
                 errors[f_name] = self.message
         if len(errors.keys()):
             raise ValidationError(errors)
```

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/settings.py` & `django-camomilla-cms-6.0.0b2/camomilla/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,17 @@
 
 ARTICLE_DEFAULT_TEMPLATE = pointed_getter(
     django_settings,
     "CAMOMILLA.RENDER.ARTICLE.DEFAULT_TEMPLATE",
     "defaults/articles/default.html",
 )
 PAGE_DEFAULT_TEMPLATE = pointed_getter(
-    django_settings, "CAMOMILLA.RENDER.PAGE.DEFAULT_TEMPLATE", "defaults/pages/default.html"
+    django_settings,
+    "CAMOMILLA.RENDER.PAGE.DEFAULT_TEMPLATE",
+    "defaults/pages/default.html",
 )
 ARTICLE_INJECT_CONTEXT_FUNC = pointed_getter(
     django_settings, "CAMOMILLA.RENDER.ARTICLE.INJECT_CONTEXT", None
 )
 PAGE_INJECT_CONTEXT_FUNC = pointed_getter(
     django_settings, "CAMOMILLA.RENDER.PAGE.INJECT_CONTEXT", None
 )
@@ -59,22 +61,25 @@
 )
 MEDIA_OPTIMIZE_DPI = pointed_getter(django_settings, "CAMOMILLA.MEDIA.OPTIMIZE.DPI", 30)
 
 ENABLE_MEDIA_OPTIMIZATION = pointed_getter(
     django_settings, "CAMOMILLA.MEDIA.OPTIMIZE.ENABLE", True
 )
 
+API_NESTING_DEPTH = pointed_getter(django_settings, "CAMOMILLA.API.NESTING_DEPTH", 10)
+
 # camomilla settings example
 # CAMOMILLA = {
 #     "PROJECT_TITLE": "",
 #     "ROUTER": {
 #         "BASE_URL": ""
 #     },
 #     "MEDIA": {
 #         "OPTIMIZE": {"MAX_WIDTH": 1980, "MAX_HEIGHT": 1400, "DPI": 30, "ENABLE": True},
 #         "THUMBNAIL": {"FOLDER": "", "WIDTH": 50, "HEIGHT": 50}
 #     },
 #     "RENDER": {
 #         "ARTICLE": {"DEFAULT_TEMPLATE": "", "INJECT_CONTEXT": None },
 #         "PAGE": {"DEFAULT_TEMPLATE": "", "INJECT_CONTEXT": None }
-#     }
+#     },
+#     "API": {"NESTING_DEPTH": 10 }
 # }
```

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/storages/optimize.py` & `django-camomilla-cms-6.0.0b2/camomilla/storages/optimize.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/structured/__init__.py` & `django-camomilla-cms-6.0.0b2/camomilla/structured/__init__.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/structured/fields.py` & `django-camomilla-cms-6.0.0b2/camomilla/structured/fields.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/structured/models.py` & `django-camomilla-cms-6.0.0b2/camomilla/structured/models.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/templates/defaults/base.html` & `django-camomilla-cms-6.0.0b2/camomilla/templates/defaults/base.html`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/templates/defaults/parts/langswitch.html` & `django-camomilla-cms-6.0.0b2/camomilla/templates/defaults/parts/langswitch.html`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/templates/defaults/widgets/media_select_multiple.html` & `django-camomilla-cms-6.0.0b2/camomilla/templates/defaults/widgets/media_select_multiple.html`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/templatetags/camomilla_filters.py` & `django-camomilla-cms-6.0.0b2/camomilla/templatetags/camomilla_filters.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/templatetags/menus.py` & `django-camomilla-cms-6.0.0b2/camomilla/templatetags/menus.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/translation.py` & `django-camomilla-cms-6.0.0b2/camomilla/translation.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/urls.py` & `django-camomilla-cms-6.0.0b2/camomilla/urls.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from django.shortcuts import redirect
 from django.urls import include, path
 from rest_framework import routers
 from importlib.util import find_spec
+from rest_framework.schemas import get_schema_view
 
+from camomilla.openapi.schema import SchemaGenerator
 from camomilla.views import (
     ArticleViewSet,
     CamomillaAuthLogin,
     CamomillaAuthLogout,
     CamomillaObtainAuthToken,
     ContentViewSet,
     LanguageViewSet,
@@ -37,13 +39,19 @@
     path(
         "profiles/me/", lambda _: redirect("../../users/current/"), name="profiles-me"
     ),
     path("token-auth/", CamomillaObtainAuthToken.as_view(), name="api_token"),
     path("auth/login/", CamomillaAuthLogin.as_view(), name="login"),
     path("auth/logout/", CamomillaAuthLogout.as_view(), name="logout"),
     path("languages/", LanguageViewSet.as_view(), name="get_languages"),
+    path('openapi', get_schema_view(
+        title="Camomilla",
+        description="API for all things …",
+        version="1.0.0",
+        generator_class=SchemaGenerator
+    ), name='openapi-schema'),
 ]
 
 if find_spec("djsuperadmin.urls") is not None:
     urlpatterns += [
         path("djsuperadmin/", include("djsuperadmin.urls")),
     ]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/utils/getters.py` & `django-camomilla-cms-6.0.0b2/camomilla/utils/getters.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/utils/seo.py` & `django-camomilla-cms-6.0.0b2/camomilla/utils/seo.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/utils/translation.py` & `django-camomilla-cms-6.0.0b2/camomilla/utils/translation.py`

 * *Files 15% similar despite different names*

```diff
@@ -56,7 +56,12 @@
     query = Q()
     for lang in AVAILABLE_LANGUAGES:
         query |= Q(**{f"{key}_{lang}": value for key, value in kwargs.items()})
     if current_lang:
         query = (query & Q(**{f"{key}_{current_lang}__isnull": True for key in kwargs.keys()}))
         query |= Q(**{f"{key}_{current_lang}": value for key, value in kwargs.items()})
     return query
+
+
+def is_translatable(model:Model) -> bool:
+    from modeltranslation.translator import translator
+    return model in translator.get_registered_models()
```

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/views/articles.py` & `django-camomilla-cms-6.0.0b2/camomilla/views/articles.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/views/contents.py` & `django-camomilla-cms-6.0.0b2/camomilla/views/contents.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/views/medias.py` & `django-camomilla-cms-6.0.0b2/camomilla/views/medias.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/views/menus.py` & `django-camomilla-cms-6.0.0b2/camomilla/views/menus.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/views/mixins/__init__.py` & `django-camomilla-cms-6.0.0b2/camomilla/views/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/views/mixins/ordering.py` & `django-camomilla-cms-6.0.0b2/camomilla/views/mixins/ordering.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/views/mixins/pagination.py` & `django-camomilla-cms-6.0.0b2/camomilla/views/mixins/pagination.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/camomilla/views/users.py` & `django-camomilla-cms-6.0.0b2/camomilla/views/users.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/django_camomilla_cms.egg-info/PKG-INFO` & `django-camomilla-cms-6.0.0b2/django_camomilla_cms.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-camomilla-cms
-Version: 6.0.0b1
+Version: 6.0.0b2
 Summary: Django powered cms
 Home-page: https://github.com/lotrekagency/camomilla
 Author: Lotrèk
 Author-email: dimmitutto@lotrek.it
 License: MIT
 Keywords: cms,django,api cms
 Classifier: Environment :: Web Environment
@@ -40,21 +40,20 @@
     from camomilla.defaults import *
 
 Remember to add all the required applications in your project
 
 ```python
 INSTALLED_APPS = [
     ...
-    'camomilla',
-    'camomilla.theme',
-    'djsuperadmin',
-    'modeltranslation',
-    'djlotrek',
-    'rest_framework',
-    'rest_framework.authtoken',
+    'camomilla', # always needed
+    'camomilla.theme', # needed to customize admin interface
+    'djsuperadmin', # needed if you whant to use djsuperadmin for contents
+    'modeltranslation', # needed if your website is multilanguage (can be added later)
+    'rest_framework',  # always needed
+    'rest_framework.authtoken',  # always needed
     ...
 ]
 ```
 
 ## Run the server
 
     $ python manage.py runserver
```

### Comparing `django-camomilla-cms-6.0.0b1/django_camomilla_cms.egg-info/SOURCES.txt` & `django-camomilla-cms-6.0.0b2/django_camomilla_cms.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 camomilla/models/__init__.py
 camomilla/models/article.py
 camomilla/models/content.py
 camomilla/models/media.py
 camomilla/models/menu.py
 camomilla/models/page.py
 camomilla/models/mixins/__init__.py
+camomilla/openapi/__init__.py
+camomilla/openapi/schema.py
 camomilla/serializers/__init__.py
 camomilla/serializers/article.py
 camomilla/serializers/content_type.py
 camomilla/serializers/media.py
 camomilla/serializers/menu.py
 camomilla/serializers/page.py
 camomilla/serializers/user.py
@@ -51,31 +53,36 @@
 camomilla/serializers/mixins/__init__.py
 camomilla/storages/__init__.py
 camomilla/storages/optimize.py
 camomilla/storages/overwrite.py
 camomilla/structured/__init__.py
 camomilla/structured/fields.py
 camomilla/structured/models.py
+camomilla/templates/admin/camomilla/page/change_form.html
 camomilla/templates/defaults/base.html
 camomilla/templates/defaults/articles/default.html
 camomilla/templates/defaults/pages/default.html
 camomilla/templates/defaults/parts/langswitch.html
 camomilla/templates/defaults/parts/menu.html
 camomilla/templates/defaults/widgets/media_select_multiple.html
 camomilla/templatetags/__init__.py
 camomilla/templatetags/camomilla_filters.py
 camomilla/templatetags/menus.py
 camomilla/theme/__init__.py
+camomilla/theme/apps.py
 camomilla/theme/static/admin/css/responsive.css
-camomilla/theme/static/admin/img/logo.png
-camomilla/theme/templates/admin/base_site.html
+camomilla/theme/static/admin/img/favicon.ico
+camomilla/theme/static/admin/img/logo.svg
+camomilla/theme/templates/admin/base.html
+camomilla/theme/templates/rosetta/base.html
 camomilla/utils/__init__.py
 camomilla/utils/getters.py
 camomilla/utils/normalization.py
 camomilla/utils/seo.py
+camomilla/utils/templates.py
 camomilla/utils/translation.py
 camomilla/views/__init__.py
 camomilla/views/articles.py
 camomilla/views/contents.py
 camomilla/views/languages.py
 camomilla/views/medias.py
 camomilla/views/menus.py
```

### Comparing `django-camomilla-cms-6.0.0b1/setup.cfg` & `django-camomilla-cms-6.0.0b2/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 packages = find:
 include_package_data = True
 python_requires = >= 3.6
 install_requires = 
 	django-modeltranslation>=0.18.7
 	djsuperadmin>=0.9,<1.0.0
 	djangorestframework>=3.10.0,<4.0.0
-	djlotrek>=0.1.6,<1.0.0
-	Pillow>=6.2.0,<7.0.0
+	django-admin-interface>=0.26.0,<1.0.0
+	Pillow>=6.2.0,<10.0.0
 	django-ckeditor>=5.7.1,<7.0.0
 	python-magic>=0.4,<0.5
 	jsonmodels==2.6.0
 	Django>=3.2
 
 [bdist_wheel]
 universal = true
```

### Comparing `django-camomilla-cms-6.0.0b1/tests/test_api.py` & `django-camomilla-cms-6.0.0b2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/tests/test_camomilla_filters.py` & `django-camomilla-cms-6.0.0b2/tests/test_camomilla_filters.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/tests/test_models.py` & `django-camomilla-cms-6.0.0b2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/tests/test_utils.py` & `django-camomilla-cms-6.0.0b2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-camomilla-cms-6.0.0b1/tests/urls.py` & `django-camomilla-cms-6.0.0b2/tests/urls.py`

 * *Files identical despite different names*

