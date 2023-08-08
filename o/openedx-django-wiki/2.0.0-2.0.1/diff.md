# Comparing `tmp/openedx-django-wiki-2.0.0.tar.gz` & `tmp/openedx-django-wiki-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openedx-django-wiki-2.0.0.tar", last modified: Tue Jan 31 17:17:51 2023, max compression
+gzip compressed data, was "openedx-django-wiki-2.0.1.tar", last modified: Tue Aug  8 10:56:45 2023, max compression
```

## Comparing `openedx-django-wiki-2.0.0.tar` & `openedx-django-wiki-2.0.1.tar`

### file list

```diff
@@ -1,352 +1,352 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.957308 openedx-django-wiki-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)      295 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8873 2023-01-31 17:17:51.957308 openedx-django-wiki-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6765 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.917308 openedx-django-wiki-2.0.0/django_notify/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/django_notify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/django_notify/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)     1450 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/django_notify/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.917308 openedx-django-wiki-2.0.0/django_notify/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     3682 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/django_notify/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/django_notify/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5466 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/django_notify/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/django_notify/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)      384 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/django_notify/tests.py
--rw-r--r--   0 runner    (1001) docker     (122)      741 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/django_notify/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/django_notify/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.921308 openedx-django-wiki-2.0.0/openedx_django_wiki.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8873 2023-01-31 17:17:51.000000 openedx-django-wiki-2.0.0/openedx_django_wiki.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    11736 2023-01-31 17:17:51.000000 openedx-django-wiki-2.0.0/openedx_django_wiki.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-31 17:17:51.000000 openedx-django-wiki-2.0.0/openedx_django_wiki.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-31 17:17:51.000000 openedx-django-wiki-2.0.0/openedx_django_wiki.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       77 2023-01-31 17:17:51.000000 openedx-django-wiki-2.0.0/openedx_django_wiki.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-01-31 17:17:51.000000 openedx-django-wiki-2.0.0/openedx_django_wiki.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.921308 openedx-django-wiki-2.0.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      230 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-31 17:17:51.957308 openedx-django-wiki-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2895 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.921308 openedx-django-wiki-2.0.0/wiki/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2565 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)      520 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.921308 openedx-django-wiki-2.0.0/wiki/conf/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6505 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/conf/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.921308 openedx-django-wiki-2.0.0/wiki/core/
--rw-r--r--   0 runner    (1001) docker     (122)     1037 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      692 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/core/compat.py
--rw-r--r--   0 runner    (1001) docker     (122)      278 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/core/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)      157 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      352 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/core/extensions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/core/http.py
--rw-r--r--   0 runner    (1001) docker     (122)      709 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/core/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.925308 openedx-django-wiki-2.0.0/wiki/core/plugins/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/core/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1708 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/core/plugins/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/core/plugins/loader.py
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/core/plugins/registry.py
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/core/processors.py
--rw-r--r--   0 runner    (1001) docker     (122)     5959 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.925308 openedx-django-wiki-2.0.0/wiki/editors/
--rw-r--r--   0 runner    (1001) docker     (122)      371 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/editors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      599 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/editors/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2574 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/editors/markitup.py
--rw-r--r--   0 runner    (1001) docker     (122)    16747 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.925308 openedx-django-wiki-2.0.0/wiki/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.925308 openedx-django-wiki-2.0.0/wiki/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15856 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/management/commands/wikiviz.py
--rw-r--r--   0 runner    (1001) docker     (122)     4907 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/managers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.925308 openedx-django-wiki-2.0.0/wiki/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)    16759 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      296 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/migrations/0002_remove_article_subscription.py
--rw-r--r--   0 runner    (1001) docker     (122)      887 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/migrations/0003_ip_address_conv.py
--rw-r--r--   0 runner    (1001) docker     (122)      375 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/migrations/0004_increase_slug_size.py
--rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/migrations/0005_remove_attachments_and_images.py
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/migrations/0006_auto_20200110_1003.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.925308 openedx-django-wiki-2.0.0/wiki/models/
--rw-r--r--   0 runner    (1001) docker     (122)     3982 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14323 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/models/article.py
--rw-r--r--   0 runner    (1001) docker     (122)    10001 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/models/pluginbase.py
--rw-r--r--   0 runner    (1001) docker     (122)    11633 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/models/urlpath.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.925308 openedx-django-wiki-2.0.0/wiki/plugins/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.929308 openedx-django-wiki-2.0.0/wiki/plugins/attachments/
--rw-r--r--   0 runner    (1001) docker     (122)       51 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/attachments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      588 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/attachments/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)      996 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/attachments/forms.py
--rw-r--r--   0 runner    (1001) docker     (122)     1859 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/attachments/markdown_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.929308 openedx-django-wiki-2.0.0/wiki/plugins/attachments/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     3703 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/attachments/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/attachments/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5718 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/attachments/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     1614 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/attachments/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.905308 openedx-django-wiki-2.0.0/wiki/plugins/attachments/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.905308 openedx-django-wiki-2.0.0/wiki/plugins/attachments/templates/wiki/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.905308 openedx-django-wiki-2.0.0/wiki/plugins/attachments/templates/wiki/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.929308 openedx-django-wiki-2.0.0/wiki/plugins/attachments/templates/wiki/plugins/attachments/
--rw-r--r--   0 runner    (1001) docker     (122)     2078 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/attachments/templates/wiki/plugins/attachments/delete.html
--rw-r--r--   0 runner    (1001) docker     (122)     2112 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/attachments/templates/wiki/plugins/attachments/history.html
--rw-r--r--   0 runner    (1001) docker     (122)     5464 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/attachments/templates/wiki/plugins/attachments/index.html
--rw-r--r--   0 runner    (1001) docker     (122)     1953 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/attachments/templates/wiki/plugins/attachments/replace.html
--rw-r--r--   0 runner    (1001) docker     (122)     2573 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/attachments/templates/wiki/plugins/attachments/search.html
--rw-r--r--   0 runner    (1001) docker     (122)    13728 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/attachments/views.py
--rw-r--r--   0 runner    (1001) docker     (122)     2331 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/attachments/wiki_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.929308 openedx-django-wiki-2.0.0/wiki/plugins/help/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/help/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/help/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.905308 openedx-django-wiki-2.0.0/wiki/plugins/help/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.905308 openedx-django-wiki-2.0.0/wiki/plugins/help/templates/wiki/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.905308 openedx-django-wiki-2.0.0/wiki/plugins/help/templates/wiki/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.929308 openedx-django-wiki-2.0.0/wiki/plugins/help/templates/wiki/plugins/help/
--rw-r--r--   0 runner    (1001) docker     (122)      801 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/help/templates/wiki/plugins/help/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (122)      384 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/help/tests.py
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/help/views.py
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/help/wiki_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.929308 openedx-django-wiki-2.0.0/wiki/plugins/images/
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      943 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)     2196 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/forms.py
--rw-r--r--   0 runner    (1001) docker     (122)     2523 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/markdown_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.929308 openedx-django-wiki-2.0.0/wiki/plugins/images/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     1673 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3509 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/models.py
--rw-r--r--   0 runner    (1001) docker     (122)      633 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.905308 openedx-django-wiki-2.0.0/wiki/plugins/images/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.905308 openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.905308 openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.929308 openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/colorbox/
--rw-r--r--   0 runner    (1001) docker     (122)     9715 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/colorbox/jquery.colorbox-min.js
--rw-r--r--   0 runner    (1001) docker     (122)    25626 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/colorbox/jquery.colorbox.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.933308 openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/content/
--rw-r--r--   0 runner    (1001) docker     (122)      394 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/content/ajax.html
--rw-r--r--   0 runner    (1001) docker     (122)      732 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/content/flash.html
--rw-r--r--   0 runner    (1001) docker     (122)     8917 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/content/homer.jpg
--rw-r--r--   0 runner    (1001) docker     (122)    55125 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/content/marylou.jpg
--rw-r--r--   0 runner    (1001) docker     (122)    74827 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/content/ohoopee1.jpg
--rw-r--r--   0 runner    (1001) docker     (122)   117411 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/content/ohoopee2.jpg
--rw-r--r--   0 runner    (1001) docker     (122)    71514 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/content/ohoopee3.jpg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.933308 openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/example1/
--rw-r--r--   0 runner    (1001) docker     (122)     4939 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/example1/colorbox.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.933308 openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/example1/images/
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/example1/images/border.png
--rw-r--r--   0 runner    (1001) docker     (122)     2893 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/example1/images/controls.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.933308 openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/borderBottomCenter.png
--rw-r--r--   0 runner    (1001) docker     (122)      215 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/borderBottomLeft.png
--rw-r--r--   0 runner    (1001) docker     (122)      217 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/borderBottomRight.png
--rw-r--r--   0 runner    (1001) docker     (122)      108 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/borderMiddleLeft.png
--rw-r--r--   0 runner    (1001) docker     (122)      108 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/borderMiddleRight.png
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/borderTopCenter.png
--rw-r--r--   0 runner    (1001) docker     (122)      216 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/borderTopLeft.png
--rw-r--r--   0 runner    (1001) docker     (122)      214 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/borderTopRight.png
--rw-r--r--   0 runner    (1001) docker     (122)     9427 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/example1/images/loading.gif
--rw-r--r--   0 runner    (1001) docker     (122)      157 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/example1/images/loading_background.png
--rw-r--r--   0 runner    (1001) docker     (122)      182 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/example1/images/overlay.png
--rw-r--r--   0 runner    (1001) docker     (122)     5140 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/example1/index.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.933308 openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/js/
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/js/images.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.905308 openedx-django-wiki-2.0.0/wiki/plugins/images/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.905308 openedx-django-wiki-2.0.0/wiki/plugins/images/templates/wiki/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.905308 openedx-django-wiki-2.0.0/wiki/plugins/images/templates/wiki/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.937308 openedx-django-wiki-2.0.0/wiki/plugins/images/templates/wiki/plugins/images/
--rw-r--r--   0 runner    (1001) docker     (122)     4015 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/templates/wiki/plugins/images/index.html
--rw-r--r--   0 runner    (1001) docker     (122)     1009 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/templates/wiki/plugins/images/purge.html
--rw-r--r--   0 runner    (1001) docker     (122)      794 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/templates/wiki/plugins/images/render.html
--rw-r--r--   0 runner    (1001) docker     (122)      992 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/templates/wiki/plugins/images/revision_add.html
--rw-r--r--   0 runner    (1001) docker     (122)     4231 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/templates/wiki/plugins/images/sidebar.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.937308 openedx-django-wiki-2.0.0/wiki/plugins/images/templatetags/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      494 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/templatetags/wiki_images_tags.py
--rw-r--r--   0 runner    (1001) docker     (122)     6873 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/views.py
--rw-r--r--   0 runner    (1001) docker     (122)     2208 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/images/wiki_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.937308 openedx-django-wiki-2.0.0/wiki/plugins/links/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/links/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.937308 openedx-django-wiki-2.0.0/wiki/plugins/links/mdx/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/links/mdx/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5113 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/links/mdx/djangowikilinks.py
--rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/links/mdx/urlize.py
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/links/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.905308 openedx-django-wiki-2.0.0/wiki/plugins/links/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.905308 openedx-django-wiki-2.0.0/wiki/plugins/links/templates/wiki/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.905308 openedx-django-wiki-2.0.0/wiki/plugins/links/templates/wiki/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.937308 openedx-django-wiki-2.0.0/wiki/plugins/links/templates/wiki/plugins/links/
--rw-r--r--   0 runner    (1001) docker     (122)     1212 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/links/templates/wiki/plugins/links/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (122)      383 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/links/tests.py
--rw-r--r--   0 runner    (1001) docker     (122)     1097 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/links/views.py
--rw-r--r--   0 runner    (1001) docker     (122)     1179 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/links/wiki_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.937308 openedx-django-wiki-2.0.0/wiki/plugins/notifications/
--rw-r--r--   0 runner    (1001) docker     (122)      107 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2968 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/notifications/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.937308 openedx-django-wiki-2.0.0/wiki/plugins/notifications/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)      862 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/notifications/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/notifications/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3166 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/notifications/models.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/notifications/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.905308 openedx-django-wiki-2.0.0/wiki/plugins/notifications/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.905308 openedx-django-wiki-2.0.0/wiki/plugins/notifications/static/wiki/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.905308 openedx-django-wiki-2.0.0/wiki/plugins/notifications/static/wiki/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.905308 openedx-django-wiki-2.0.0/wiki/plugins/notifications/static/wiki/plugins/notifications/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.937308 openedx-django-wiki-2.0.0/wiki/plugins/notifications/static/wiki/plugins/notifications/js/
--rw-r--r--   0 runner    (1001) docker     (122)     1458 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/notifications/static/wiki/plugins/notifications/js/ui.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.905308 openedx-django-wiki-2.0.0/wiki/plugins/notifications/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.905308 openedx-django-wiki-2.0.0/wiki/plugins/notifications/templates/wiki/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.909308 openedx-django-wiki-2.0.0/wiki/plugins/notifications/templates/wiki/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.937308 openedx-django-wiki-2.0.0/wiki/plugins/notifications/templates/wiki/plugins/notifications/
--rw-r--r--   0 runner    (1001) docker     (122)      905 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/notifications/templates/wiki/plugins/notifications/menubaritem.html
--rw-r--r--   0 runner    (1001) docker     (122)      383 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/notifications/tests.py
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/notifications/views.py
--rw-r--r--   0 runner    (1001) docker     (122)      269 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/plugins/notifications/wiki_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.909308 openedx-django-wiki-2.0.0/wiki/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.909308 openedx-django-wiki-2.0.0/wiki/static/wiki/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.909308 openedx-django-wiki-2.0.0/wiki/static/wiki/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.941308 openedx-django-wiki-2.0.0/wiki/static/wiki/bootstrap/css/
--rw-r--r--   0 runner    (1001) docker     (122)    20470 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/bootstrap/css/bootstrap-responsive.css
--rw-r--r--   0 runner    (1001) docker     (122)    15545 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/bootstrap/css/bootstrap-responsive.min.css
--rw-r--r--   0 runner    (1001) docker     (122)   115072 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/bootstrap/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (122)    95583 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.941308 openedx-django-wiki-2.0.0/wiki/static/wiki/bootstrap/img/
--rw-r--r--   0 runner    (1001) docker     (122)     8777 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/bootstrap/img/glyphicons-halflings-white.png
--rw-r--r--   0 runner    (1001) docker     (122)    12799 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/bootstrap/img/glyphicons-halflings.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.941308 openedx-django-wiki-2.0.0/wiki/static/wiki/bootstrap/js/
--rw-r--r--   0 runner    (1001) docker     (122)    56216 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/bootstrap/js/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (122)    25526 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/bootstrap/js/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.941308 openedx-django-wiki-2.0.0/wiki/static/wiki/img/
--rw-r--r--   0 runner    (1001) docker     (122)     3902 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/img/github_icon.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.941308 openedx-django-wiki-2.0.0/wiki/static/wiki/js/
--rw-r--r--   0 runner    (1001) docker     (122)      313 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/js/core.js
--rw-r--r--   0 runner    (1001) docker     (122)     1053 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/js/diff.js
--rw-r--r--   0 runner    (1001) docker     (122)     2483 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/js/diffview.js
--rw-r--r--   0 runner    (1001) docker     (122)      859 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/js/editor.js
--rw-r--r--   0 runner    (1001) docker     (122)    92556 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/js/jquery.min.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.941308 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/
--rw-r--r--   0 runner    (1001) docker     (122)      127 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/admin.init.js
--rw-r--r--   0 runner    (1001) docker     (122)       77 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/frontend.init.js
--rw-r--r--   0 runner    (1001) docker     (122)    18300 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/jquery.markitup.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.909308 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.941308 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/admin/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.945308 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/admin/images/
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/admin/images/bold.png
--rw-r--r--   0 runner    (1001) docker     (122)      859 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/admin/images/code.png
--rw-r--r--   0 runner    (1001) docker     (122)      276 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/admin/images/h1.png
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/admin/images/h2.png
--rw-r--r--   0 runner    (1001) docker     (122)      306 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/admin/images/h3.png
--rw-r--r--   0 runner    (1001) docker     (122)      293 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/admin/images/h4.png
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/admin/images/h5.png
--rw-r--r--   0 runner    (1001) docker     (122)      310 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/admin/images/h6.png
--rw-r--r--   0 runner    (1001) docker     (122)      223 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/admin/images/italic.png
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/admin/images/link.png
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/admin/images/list-bullet.png
--rw-r--r--   0 runner    (1001) docker     (122)      357 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/admin/images/list-numeric.png
--rw-r--r--   0 runner    (1001) docker     (122)      606 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/admin/images/picture.png
--rw-r--r--   0 runner    (1001) docker     (122)      537 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/admin/images/preview.png
--rw-r--r--   0 runner    (1001) docker     (122)      743 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/admin/images/quotes.png
--rw-r--r--   0 runner    (1001) docker     (122)      319 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/admin/readme.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2408 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/admin/set.js
--rw-r--r--   0 runner    (1001) docker     (122)     1720 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/admin/style.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.945308 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/default/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.945308 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/default/images/
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/default/images/bold.png
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/default/images/clean.png
--rw-r--r--   0 runner    (1001) docker     (122)      516 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/default/images/image.png
--rw-r--r--   0 runner    (1001) docker     (122)      223 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/default/images/italic.png
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/default/images/link.png
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/default/images/list-bullet.png
--rw-r--r--   0 runner    (1001) docker     (122)      357 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/default/images/list-numeric.png
--rw-r--r--   0 runner    (1001) docker     (122)      606 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/default/images/picture.png
--rw-r--r--   0 runner    (1001) docker     (122)      537 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/default/images/preview.png
--rw-r--r--   0 runner    (1001) docker     (122)      269 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/default/images/stroke.png
--rw-r--r--   0 runner    (1001) docker     (122)     1873 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/default/set.js
--rw-r--r--   0 runner    (1001) docker     (122)      886 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/default/style.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.949308 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/frontend/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.949308 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/frontend/images/
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/frontend/images/bold.png
--rw-r--r--   0 runner    (1001) docker     (122)      859 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/frontend/images/code.png
--rw-r--r--   0 runner    (1001) docker     (122)      276 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/frontend/images/h1.png
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/frontend/images/h2.png
--rw-r--r--   0 runner    (1001) docker     (122)      306 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/frontend/images/h3.png
--rw-r--r--   0 runner    (1001) docker     (122)      293 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/frontend/images/h4.png
--rw-r--r--   0 runner    (1001) docker     (122)      304 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/frontend/images/h5.png
--rw-r--r--   0 runner    (1001) docker     (122)      310 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/frontend/images/h6.png
--rw-r--r--   0 runner    (1001) docker     (122)      223 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/frontend/images/italic.png
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/frontend/images/link.png
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/frontend/images/list-bullet.png
--rw-r--r--   0 runner    (1001) docker     (122)      357 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/frontend/images/list-numeric.png
--rw-r--r--   0 runner    (1001) docker     (122)      606 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/frontend/images/picture.png
--rw-r--r--   0 runner    (1001) docker     (122)      537 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/frontend/images/preview.png
--rw-r--r--   0 runner    (1001) docker     (122)      743 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/frontend/images/quotes.png
--rw-r--r--   0 runner    (1001) docker     (122)      319 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/frontend/readme.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2038 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/frontend/set.js
--rw-r--r--   0 runner    (1001) docker     (122)     1647 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/frontend/style.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.909308 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.949308 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/markitup/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.953308 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/markitup/images/
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/markitup/images/bg-container.png
--rw-r--r--   0 runner    (1001) docker     (122)     1642 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-bbcode.png
--rw-r--r--   0 runner    (1001) docker     (122)     1682 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-dotclear.png
--rw-r--r--   0 runner    (1001) docker     (122)     1534 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-html.png
--rw-r--r--   0 runner    (1001) docker     (122)     1529 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-json.png
--rw-r--r--   0 runner    (1001) docker     (122)     1783 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-markdown.png
--rw-r--r--   0 runner    (1001) docker     (122)     1659 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-textile.png
--rw-r--r--   0 runner    (1001) docker     (122)     1488 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-wiki.png
--rw-r--r--   0 runner    (1001) docker     (122)     1495 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-xml.png
--rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/markitup/images/bg-editor.png
--rw-r--r--   0 runner    (1001) docker     (122)      258 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/markitup/images/handle.png
--rw-r--r--   0 runner    (1001) docker     (122)      254 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/markitup/images/menu.png
--rw-r--r--   0 runner    (1001) docker     (122)      240 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/markitup/images/submenu.png
--rw-r--r--   0 runner    (1001) docker     (122)     3337 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/markitup/style.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.953308 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/simple/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.953308 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/simple/images/
--rw-r--r--   0 runner    (1001) docker     (122)      258 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/simple/images/handle.png
--rw-r--r--   0 runner    (1001) docker     (122)      241 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/simple/images/menu.png
--rw-r--r--   0 runner    (1001) docker     (122)      240 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/simple/images/submenu.png
--rw-r--r--   0 runner    (1001) docker     (122)      150 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/simple/readme.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2477 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/simple/style.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.953308 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/templates/preview.css
--rw-r--r--   0 runner    (1001) docker     (122)      406 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/templates/preview.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.909308 openedx-django-wiki-2.0.0/wiki/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.953308 openedx-django-wiki-2.0.0/wiki/templates/wiki/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.957308 openedx-django-wiki-2.0.0/wiki/templates/wiki/accounts/
--rw-r--r--   0 runner    (1001) docker     (122)      675 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/templates/wiki/accounts/login.html
--rw-r--r--   0 runner    (1001) docker     (122)      481 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/templates/wiki/accounts/signup.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.957308 openedx-django-wiki-2.0.0/wiki/templates/wiki/article/
--rw-r--r--   0 runner    (1001) docker     (122)     1300 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/templates/wiki/article/create_root.html
--rw-r--r--   0 runner    (1001) docker     (122)     1258 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/templates/wiki/article.html
--rw-r--r--   0 runner    (1001) docker     (122)     6548 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/templates/wiki/base.html
--rw-r--r--   0 runner    (1001) docker     (122)     2106 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/templates/wiki/create.html
--rw-r--r--   0 runner    (1001) docker     (122)     2232 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/templates/wiki/delete.html
--rw-r--r--   0 runner    (1001) docker     (122)     1572 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/templates/wiki/deleted.html
--rw-r--r--   0 runner    (1001) docker     (122)     2688 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/templates/wiki/dir.html
--rw-r--r--   0 runner    (1001) docker     (122)     2652 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/templates/wiki/edit.html
--rw-r--r--   0 runner    (1001) docker     (122)      618 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/templates/wiki/error.html
--rw-r--r--   0 runner    (1001) docker     (122)     8805 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/templates/wiki/history.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.957308 openedx-django-wiki-2.0.0/wiki/templates/wiki/includes/
--rw-r--r--   0 runner    (1001) docker     (122)      390 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/templates/wiki/includes/anonymous_blocked.html
--rw-r--r--   0 runner    (1001) docker     (122)     1661 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/templates/wiki/includes/article_menu.html
--rw-r--r--   0 runner    (1001) docker     (122)     2449 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/templates/wiki/includes/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (122)      241 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/templates/wiki/includes/editor.html
--rw-r--r--   0 runner    (1001) docker     (122)      992 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/templates/wiki/includes/editor_sidebar.html
--rw-r--r--   0 runner    (1001) docker     (122)      492 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/templates/wiki/includes/editormedia.html
--rw-r--r--   0 runner    (1001) docker     (122)     1241 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/templates/wiki/includes/form.html
--rw-r--r--   0 runner    (1001) docker     (122)      335 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/templates/wiki/includes/pagination.html
--rw-r--r--   0 runner    (1001) docker     (122)      806 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/templates/wiki/includes/render.html
--rw-r--r--   0 runner    (1001) docker     (122)     1052 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/templates/wiki/includes/revision_info.html
--rw-r--r--   0 runner    (1001) docker     (122)      321 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/templates/wiki/permission_denied.html
--rw-r--r--   0 runner    (1001) docker     (122)      970 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/templates/wiki/preview_inline.html
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/templates/wiki/settings.html
--rw-r--r--   0 runner    (1001) docker     (122)      426 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/templates/wiki/source.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.957308 openedx-django-wiki-2.0.0/wiki/templatetags/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2472 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/templatetags/wiki_tags.py
--rw-r--r--   0 runner    (1001) docker     (122)     7490 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/tests.py
--rw-r--r--   0 runner    (1001) docker     (122)     4139 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:51.957308 openedx-django-wiki-2.0.0/wiki/views/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2446 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/views/accounts.py
--rw-r--r--   0 runner    (1001) docker     (122)    27881 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/views/article.py
--rw-r--r--   0 runner    (1001) docker     (122)     1391 2023-01-31 17:17:48.000000 openedx-django-wiki-2.0.0/wiki/views/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.449633 openedx-django-wiki-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      295 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8873 2023-08-08 10:56:45.449633 openedx-django-wiki-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6765 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.405633 openedx-django-wiki-2.0.1/django_notify/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/django_notify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/django_notify/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1450 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/django_notify/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.405633 openedx-django-wiki-2.0.1/django_notify/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     3682 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/django_notify/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/django_notify/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5466 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/django_notify/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/django_notify/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)      384 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/django_notify/tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)      741 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/django_notify/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/django_notify/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.405633 openedx-django-wiki-2.0.1/openedx_django_wiki.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8873 2023-08-08 10:56:44.000000 openedx-django-wiki-2.0.1/openedx_django_wiki.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    11736 2023-08-08 10:56:45.000000 openedx-django-wiki-2.0.1/openedx_django_wiki.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-08 10:56:44.000000 openedx-django-wiki-2.0.1/openedx_django_wiki.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-08 10:56:44.000000 openedx-django-wiki-2.0.1/openedx_django_wiki.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2023-08-08 10:56:44.000000 openedx-django-wiki-2.0.1/openedx_django_wiki.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-08-08 10:56:44.000000 openedx-django-wiki-2.0.1/openedx_django_wiki.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.405633 openedx-django-wiki-2.0.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      230 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-08 10:56:45.449633 openedx-django-wiki-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2895 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.405633 openedx-django-wiki-2.0.1/wiki/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2565 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      520 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.409633 openedx-django-wiki-2.0.1/wiki/conf/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6505 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/conf/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.409633 openedx-django-wiki-2.0.1/wiki/core/
+-rw-r--r--   0 runner    (1001) docker     (122)     1037 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      692 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/core/compat.py
+-rw-r--r--   0 runner    (1001) docker     (122)      278 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/core/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      352 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/core/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1211 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/core/http.py
+-rw-r--r--   0 runner    (1001) docker     (122)      709 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/core/permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.409633 openedx-django-wiki-2.0.1/wiki/core/plugins/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/core/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1708 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/core/plugins/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/core/plugins/loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/core/plugins/registry.py
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/core/processors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5959 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.409633 openedx-django-wiki-2.0.1/wiki/editors/
+-rw-r--r--   0 runner    (1001) docker     (122)      371 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/editors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      599 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/editors/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2574 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/editors/markitup.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16747 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.409633 openedx-django-wiki-2.0.1/wiki/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.413632 openedx-django-wiki-2.0.1/wiki/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15856 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/management/commands/wikiviz.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4907 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/managers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.413632 openedx-django-wiki-2.0.1/wiki/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)    16759 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      296 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/migrations/0002_remove_article_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (122)      887 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/migrations/0003_ip_address_conv.py
+-rw-r--r--   0 runner    (1001) docker     (122)      375 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/migrations/0004_increase_slug_size.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/migrations/0005_remove_attachments_and_images.py
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/migrations/0006_auto_20200110_1003.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.413632 openedx-django-wiki-2.0.1/wiki/models/
+-rw-r--r--   0 runner    (1001) docker     (122)     3982 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14323 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/models/article.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10001 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/models/pluginbase.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11633 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/models/urlpath.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.413632 openedx-django-wiki-2.0.1/wiki/plugins/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.413632 openedx-django-wiki-2.0.1/wiki/plugins/attachments/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/attachments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      588 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/attachments/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      996 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/attachments/forms.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1859 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/attachments/markdown_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.417633 openedx-django-wiki-2.0.1/wiki/plugins/attachments/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     3703 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/attachments/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/attachments/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5718 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/attachments/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1614 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/attachments/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.397632 openedx-django-wiki-2.0.1/wiki/plugins/attachments/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.397632 openedx-django-wiki-2.0.1/wiki/plugins/attachments/templates/wiki/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.397632 openedx-django-wiki-2.0.1/wiki/plugins/attachments/templates/wiki/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.417633 openedx-django-wiki-2.0.1/wiki/plugins/attachments/templates/wiki/plugins/attachments/
+-rw-r--r--   0 runner    (1001) docker     (122)     2078 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/attachments/templates/wiki/plugins/attachments/delete.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2112 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/attachments/templates/wiki/plugins/attachments/history.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5464 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/attachments/templates/wiki/plugins/attachments/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1953 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/attachments/templates/wiki/plugins/attachments/replace.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2573 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/attachments/templates/wiki/plugins/attachments/search.html
+-rw-r--r--   0 runner    (1001) docker     (122)    13728 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/attachments/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2331 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/attachments/wiki_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.417633 openedx-django-wiki-2.0.1/wiki/plugins/help/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/help/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/help/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.397632 openedx-django-wiki-2.0.1/wiki/plugins/help/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.397632 openedx-django-wiki-2.0.1/wiki/plugins/help/templates/wiki/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.397632 openedx-django-wiki-2.0.1/wiki/plugins/help/templates/wiki/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.417633 openedx-django-wiki-2.0.1/wiki/plugins/help/templates/wiki/plugins/help/
+-rw-r--r--   0 runner    (1001) docker     (122)      801 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/help/templates/wiki/plugins/help/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (122)      384 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/help/tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/help/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/help/wiki_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.417633 openedx-django-wiki-2.0.1/wiki/plugins/images/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      943 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2196 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/forms.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2523 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/markdown_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.417633 openedx-django-wiki-2.0.1/wiki/plugins/images/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3509 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      633 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.397632 openedx-django-wiki-2.0.1/wiki/plugins/images/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.397632 openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.397632 openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.417633 openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/colorbox/
+-rw-r--r--   0 runner    (1001) docker     (122)     9715 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/colorbox/jquery.colorbox-min.js
+-rw-r--r--   0 runner    (1001) docker     (122)    25626 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/colorbox/jquery.colorbox.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.421633 openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/content/
+-rw-r--r--   0 runner    (1001) docker     (122)      394 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/content/ajax.html
+-rw-r--r--   0 runner    (1001) docker     (122)      732 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/content/flash.html
+-rw-r--r--   0 runner    (1001) docker     (122)     8917 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/content/homer.jpg
+-rw-r--r--   0 runner    (1001) docker     (122)    55125 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/content/marylou.jpg
+-rw-r--r--   0 runner    (1001) docker     (122)    74827 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/content/ohoopee1.jpg
+-rw-r--r--   0 runner    (1001) docker     (122)   117411 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/content/ohoopee2.jpg
+-rw-r--r--   0 runner    (1001) docker     (122)    71514 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/content/ohoopee3.jpg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.421633 openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/example1/
+-rw-r--r--   0 runner    (1001) docker     (122)     4939 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/example1/colorbox.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.421633 openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/example1/images/
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/example1/images/border.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2893 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/example1/images/controls.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.421633 openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/borderBottomCenter.png
+-rw-r--r--   0 runner    (1001) docker     (122)      215 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/borderBottomLeft.png
+-rw-r--r--   0 runner    (1001) docker     (122)      217 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/borderBottomRight.png
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/borderMiddleLeft.png
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/borderMiddleRight.png
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/borderTopCenter.png
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/borderTopLeft.png
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/example1/images/ie6/borderTopRight.png
+-rw-r--r--   0 runner    (1001) docker     (122)     9427 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/example1/images/loading.gif
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/example1/images/loading_background.png
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/example1/images/overlay.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5140 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/example1/index.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.421633 openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/js/
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/js/images.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.397632 openedx-django-wiki-2.0.1/wiki/plugins/images/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.397632 openedx-django-wiki-2.0.1/wiki/plugins/images/templates/wiki/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.397632 openedx-django-wiki-2.0.1/wiki/plugins/images/templates/wiki/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.425633 openedx-django-wiki-2.0.1/wiki/plugins/images/templates/wiki/plugins/images/
+-rw-r--r--   0 runner    (1001) docker     (122)     4015 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/templates/wiki/plugins/images/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1009 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/templates/wiki/plugins/images/purge.html
+-rw-r--r--   0 runner    (1001) docker     (122)      794 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/templates/wiki/plugins/images/render.html
+-rw-r--r--   0 runner    (1001) docker     (122)      992 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/templates/wiki/plugins/images/revision_add.html
+-rw-r--r--   0 runner    (1001) docker     (122)     4231 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/templates/wiki/plugins/images/sidebar.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.425633 openedx-django-wiki-2.0.1/wiki/plugins/images/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      494 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/templatetags/wiki_images_tags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6873 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2208 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/images/wiki_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.425633 openedx-django-wiki-2.0.1/wiki/plugins/links/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/links/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.425633 openedx-django-wiki-2.0.1/wiki/plugins/links/mdx/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/links/mdx/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5113 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/links/mdx/djangowikilinks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/links/mdx/urlize.py
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/links/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.401633 openedx-django-wiki-2.0.1/wiki/plugins/links/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.401633 openedx-django-wiki-2.0.1/wiki/plugins/links/templates/wiki/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.401633 openedx-django-wiki-2.0.1/wiki/plugins/links/templates/wiki/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.425633 openedx-django-wiki-2.0.1/wiki/plugins/links/templates/wiki/plugins/links/
+-rw-r--r--   0 runner    (1001) docker     (122)     1212 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/links/templates/wiki/plugins/links/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (122)      383 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/links/tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1097 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/links/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1179 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/links/wiki_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.425633 openedx-django-wiki-2.0.1/wiki/plugins/notifications/
+-rw-r--r--   0 runner    (1001) docker     (122)       54 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2968 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/notifications/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.425633 openedx-django-wiki-2.0.1/wiki/plugins/notifications/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)      862 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/notifications/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/notifications/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3166 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/notifications/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/notifications/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.401633 openedx-django-wiki-2.0.1/wiki/plugins/notifications/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.401633 openedx-django-wiki-2.0.1/wiki/plugins/notifications/static/wiki/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.401633 openedx-django-wiki-2.0.1/wiki/plugins/notifications/static/wiki/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.401633 openedx-django-wiki-2.0.1/wiki/plugins/notifications/static/wiki/plugins/notifications/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.425633 openedx-django-wiki-2.0.1/wiki/plugins/notifications/static/wiki/plugins/notifications/js/
+-rw-r--r--   0 runner    (1001) docker     (122)     1458 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/notifications/static/wiki/plugins/notifications/js/ui.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.401633 openedx-django-wiki-2.0.1/wiki/plugins/notifications/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.401633 openedx-django-wiki-2.0.1/wiki/plugins/notifications/templates/wiki/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.401633 openedx-django-wiki-2.0.1/wiki/plugins/notifications/templates/wiki/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.425633 openedx-django-wiki-2.0.1/wiki/plugins/notifications/templates/wiki/plugins/notifications/
+-rw-r--r--   0 runner    (1001) docker     (122)      905 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/notifications/templates/wiki/plugins/notifications/menubaritem.html
+-rw-r--r--   0 runner    (1001) docker     (122)      383 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/notifications/tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/notifications/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)      269 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/plugins/notifications/wiki_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.401633 openedx-django-wiki-2.0.1/wiki/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.401633 openedx-django-wiki-2.0.1/wiki/static/wiki/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.401633 openedx-django-wiki-2.0.1/wiki/static/wiki/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.429633 openedx-django-wiki-2.0.1/wiki/static/wiki/bootstrap/css/
+-rw-r--r--   0 runner    (1001) docker     (122)    20470 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/bootstrap/css/bootstrap-responsive.css
+-rw-r--r--   0 runner    (1001) docker     (122)    15545 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/bootstrap/css/bootstrap-responsive.min.css
+-rw-r--r--   0 runner    (1001) docker     (122)   115072 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/bootstrap/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (122)    95583 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.429633 openedx-django-wiki-2.0.1/wiki/static/wiki/bootstrap/img/
+-rw-r--r--   0 runner    (1001) docker     (122)     8777 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/bootstrap/img/glyphicons-halflings-white.png
+-rw-r--r--   0 runner    (1001) docker     (122)    12799 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/bootstrap/img/glyphicons-halflings.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.429633 openedx-django-wiki-2.0.1/wiki/static/wiki/bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (122)    56216 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/bootstrap/js/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (122)    25526 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/bootstrap/js/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.429633 openedx-django-wiki-2.0.1/wiki/static/wiki/img/
+-rw-r--r--   0 runner    (1001) docker     (122)     3902 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/img/github_icon.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.429633 openedx-django-wiki-2.0.1/wiki/static/wiki/js/
+-rw-r--r--   0 runner    (1001) docker     (122)      313 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/js/core.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1053 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/js/diff.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2483 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/js/diffview.js
+-rw-r--r--   0 runner    (1001) docker     (122)      859 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/js/editor.js
+-rw-r--r--   0 runner    (1001) docker     (122)    92556 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/js/jquery.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.429633 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/
+-rw-r--r--   0 runner    (1001) docker     (122)      127 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/admin.init.js
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/frontend.init.js
+-rw-r--r--   0 runner    (1001) docker     (122)    18300 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/jquery.markitup.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.401633 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.429633 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/admin/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.433633 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/admin/images/
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/admin/images/bold.png
+-rw-r--r--   0 runner    (1001) docker     (122)      859 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/admin/images/code.png
+-rw-r--r--   0 runner    (1001) docker     (122)      276 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/admin/images/h1.png
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/admin/images/h2.png
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/admin/images/h3.png
+-rw-r--r--   0 runner    (1001) docker     (122)      293 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/admin/images/h4.png
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/admin/images/h5.png
+-rw-r--r--   0 runner    (1001) docker     (122)      310 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/admin/images/h6.png
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/admin/images/italic.png
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/admin/images/link.png
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/admin/images/list-bullet.png
+-rw-r--r--   0 runner    (1001) docker     (122)      357 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/admin/images/list-numeric.png
+-rw-r--r--   0 runner    (1001) docker     (122)      606 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/admin/images/picture.png
+-rw-r--r--   0 runner    (1001) docker     (122)      537 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/admin/images/preview.png
+-rw-r--r--   0 runner    (1001) docker     (122)      743 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/admin/images/quotes.png
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/admin/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2408 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/admin/set.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1720 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/admin/style.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.433633 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/default/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.433633 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/default/images/
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/default/images/bold.png
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/default/images/clean.png
+-rw-r--r--   0 runner    (1001) docker     (122)      516 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/default/images/image.png
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/default/images/italic.png
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/default/images/link.png
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/default/images/list-bullet.png
+-rw-r--r--   0 runner    (1001) docker     (122)      357 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/default/images/list-numeric.png
+-rw-r--r--   0 runner    (1001) docker     (122)      606 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/default/images/picture.png
+-rw-r--r--   0 runner    (1001) docker     (122)      537 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/default/images/preview.png
+-rw-r--r--   0 runner    (1001) docker     (122)      269 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/default/images/stroke.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1873 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/default/set.js
+-rw-r--r--   0 runner    (1001) docker     (122)      886 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/default/style.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.433633 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.437633 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/frontend/images/
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/frontend/images/bold.png
+-rw-r--r--   0 runner    (1001) docker     (122)      859 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/frontend/images/code.png
+-rw-r--r--   0 runner    (1001) docker     (122)      276 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/frontend/images/h1.png
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/frontend/images/h2.png
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/frontend/images/h3.png
+-rw-r--r--   0 runner    (1001) docker     (122)      293 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/frontend/images/h4.png
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/frontend/images/h5.png
+-rw-r--r--   0 runner    (1001) docker     (122)      310 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/frontend/images/h6.png
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/frontend/images/italic.png
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/frontend/images/link.png
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/frontend/images/list-bullet.png
+-rw-r--r--   0 runner    (1001) docker     (122)      357 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/frontend/images/list-numeric.png
+-rw-r--r--   0 runner    (1001) docker     (122)      606 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/frontend/images/picture.png
+-rw-r--r--   0 runner    (1001) docker     (122)      537 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/frontend/images/preview.png
+-rw-r--r--   0 runner    (1001) docker     (122)      743 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/frontend/images/quotes.png
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/frontend/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2038 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/frontend/set.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1647 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/frontend/style.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.401633 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.441633 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/markitup/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.441633 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/markitup/images/
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/markitup/images/bg-container.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1642 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-bbcode.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1682 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-dotclear.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1534 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-html.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1529 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-json.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1783 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-markdown.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1659 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-textile.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1488 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-wiki.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1495 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-xml.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/markitup/images/bg-editor.png
+-rw-r--r--   0 runner    (1001) docker     (122)      258 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/markitup/images/handle.png
+-rw-r--r--   0 runner    (1001) docker     (122)      254 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/markitup/images/menu.png
+-rw-r--r--   0 runner    (1001) docker     (122)      240 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/markitup/images/submenu.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3337 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/markitup/style.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.441633 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/simple/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.441633 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/simple/images/
+-rw-r--r--   0 runner    (1001) docker     (122)      258 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/simple/images/handle.png
+-rw-r--r--   0 runner    (1001) docker     (122)      241 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/simple/images/menu.png
+-rw-r--r--   0 runner    (1001) docker     (122)      240 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/simple/images/submenu.png
+-rw-r--r--   0 runner    (1001) docker     (122)      150 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/simple/readme.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2477 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/simple/style.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.441633 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/templates/preview.css
+-rw-r--r--   0 runner    (1001) docker     (122)      406 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/templates/preview.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.401633 openedx-django-wiki-2.0.1/wiki/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.445633 openedx-django-wiki-2.0.1/wiki/templates/wiki/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.445633 openedx-django-wiki-2.0.1/wiki/templates/wiki/accounts/
+-rw-r--r--   0 runner    (1001) docker     (122)      675 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/templates/wiki/accounts/login.html
+-rw-r--r--   0 runner    (1001) docker     (122)      481 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/templates/wiki/accounts/signup.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.445633 openedx-django-wiki-2.0.1/wiki/templates/wiki/article/
+-rw-r--r--   0 runner    (1001) docker     (122)     1300 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/templates/wiki/article/create_root.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1258 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/templates/wiki/article.html
+-rw-r--r--   0 runner    (1001) docker     (122)     6548 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/templates/wiki/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2106 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/templates/wiki/create.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2232 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/templates/wiki/delete.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1572 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/templates/wiki/deleted.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2688 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/templates/wiki/dir.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2652 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/templates/wiki/edit.html
+-rw-r--r--   0 runner    (1001) docker     (122)      618 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/templates/wiki/error.html
+-rw-r--r--   0 runner    (1001) docker     (122)     8805 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/templates/wiki/history.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.445633 openedx-django-wiki-2.0.1/wiki/templates/wiki/includes/
+-rw-r--r--   0 runner    (1001) docker     (122)      390 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/templates/wiki/includes/anonymous_blocked.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1661 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/templates/wiki/includes/article_menu.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2449 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/templates/wiki/includes/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (122)      241 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/templates/wiki/includes/editor.html
+-rw-r--r--   0 runner    (1001) docker     (122)      992 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/templates/wiki/includes/editor_sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/templates/wiki/includes/editormedia.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1241 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/templates/wiki/includes/form.html
+-rw-r--r--   0 runner    (1001) docker     (122)      335 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/templates/wiki/includes/pagination.html
+-rw-r--r--   0 runner    (1001) docker     (122)      806 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/templates/wiki/includes/render.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1052 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/templates/wiki/includes/revision_info.html
+-rw-r--r--   0 runner    (1001) docker     (122)      321 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/templates/wiki/permission_denied.html
+-rw-r--r--   0 runner    (1001) docker     (122)      970 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/templates/wiki/preview_inline.html
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/templates/wiki/settings.html
+-rw-r--r--   0 runner    (1001) docker     (122)      426 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/templates/wiki/source.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.445633 openedx-django-wiki-2.0.1/wiki/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2472 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/templatetags/wiki_tags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7490 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4139 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:45.449633 openedx-django-wiki-2.0.1/wiki/views/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2446 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/views/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27881 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/views/article.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1391 2023-08-08 10:56:38.000000 openedx-django-wiki-2.0.1/wiki/views/mixins.py
```

### Comparing `openedx-django-wiki-2.0.0/PKG-INFO` & `openedx-django-wiki-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-django-wiki
-Version: 2.0.0
+Version: 2.0.1
 Summary: A wiki system written for the Django framework.
 Home-page: UNKNOWN
 Author: Benjamin Bach
 Author-email: benjamin@overtag.dk
 License: GPLv3
 Description: django-wiki
         ===========
```

### Comparing `openedx-django-wiki-2.0.0/README.md` & `openedx-django-wiki-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/django_notify/decorators.py` & `openedx-django-wiki-2.0.1/django_notify/decorators.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/django_notify/migrations/0001_initial.py` & `openedx-django-wiki-2.0.1/django_notify/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/django_notify/models.py` & `openedx-django-wiki-2.0.1/django_notify/models.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/django_notify/settings.py` & `openedx-django-wiki-2.0.1/django_notify/settings.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/django_notify/urls.py` & `openedx-django-wiki-2.0.1/django_notify/urls.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/django_notify/views.py` & `openedx-django-wiki-2.0.1/django_notify/views.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/openedx_django_wiki.egg-info/PKG-INFO` & `openedx-django-wiki-2.0.1/openedx_django_wiki.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-django-wiki
-Version: 2.0.0
+Version: 2.0.1
 Summary: A wiki system written for the Django framework.
 Home-page: UNKNOWN
 Author: Benjamin Bach
 Author-email: benjamin@overtag.dk
 License: GPLv3
 Description: django-wiki
         ===========
```

### Comparing `openedx-django-wiki-2.0.0/openedx_django_wiki.egg-info/SOURCES.txt` & `openedx-django-wiki-2.0.1/openedx_django_wiki.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/setup.py` & `openedx-django-wiki-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 package_data = {
     package_name: template_patterns
     for package_name in packages
 }
 
 setup(
     name="openedx-django-wiki",
-    version="2.0.0",
+    version="2.0.1",
     author="Benjamin Bach",
     author_email="benjamin@overtag.dk",
     long_description_content_type='text/markdown',
     description="A wiki system written for the Django framework.",
     license="GPLv3",
     keywords="django wiki markdown",
     packages=find_packages(exclude=["testproject", "testproject.*"]),
```

### Comparing `openedx-django-wiki-2.0.0/wiki/admin.py` & `openedx-django-wiki-2.0.1/wiki/admin.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/apps.py` & `openedx-django-wiki-2.0.1/wiki/apps.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/conf/settings.py` & `openedx-django-wiki-2.0.1/wiki/conf/settings.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/core/__init__.py` & `openedx-django-wiki-2.0.1/wiki/core/__init__.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/core/compat.py` & `openedx-django-wiki-2.0.1/wiki/core/compat.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/core/http.py` & `openedx-django-wiki-2.0.1/wiki/core/http.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/core/permissions.py` & `openedx-django-wiki-2.0.1/wiki/core/permissions.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/core/plugins/base.py` & `openedx-django-wiki-2.0.1/wiki/core/plugins/base.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/core/plugins/loader.py` & `openedx-django-wiki-2.0.1/wiki/core/plugins/loader.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/core/plugins/registry.py` & `openedx-django-wiki-2.0.1/wiki/core/plugins/registry.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/core/processors.py` & `openedx-django-wiki-2.0.1/wiki/core/processors.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/decorators.py` & `openedx-django-wiki-2.0.1/wiki/decorators.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/editors/base.py` & `openedx-django-wiki-2.0.1/wiki/editors/base.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/editors/markitup.py` & `openedx-django-wiki-2.0.1/wiki/editors/markitup.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/forms.py` & `openedx-django-wiki-2.0.1/wiki/forms.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/management/commands/wikiviz.py` & `openedx-django-wiki-2.0.1/wiki/management/commands/wikiviz.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/managers.py` & `openedx-django-wiki-2.0.1/wiki/managers.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/middleware.py` & `openedx-django-wiki-2.0.1/wiki/middleware.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/migrations/0001_initial.py` & `openedx-django-wiki-2.0.1/wiki/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/migrations/0003_ip_address_conv.py` & `openedx-django-wiki-2.0.1/wiki/migrations/0003_ip_address_conv.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/migrations/0005_remove_attachments_and_images.py` & `openedx-django-wiki-2.0.1/wiki/migrations/0005_remove_attachments_and_images.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/migrations/0006_auto_20200110_1003.py` & `openedx-django-wiki-2.0.1/wiki/migrations/0006_auto_20200110_1003.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/models/__init__.py` & `openedx-django-wiki-2.0.1/wiki/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/models/article.py` & `openedx-django-wiki-2.0.1/wiki/models/article.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/models/pluginbase.py` & `openedx-django-wiki-2.0.1/wiki/models/pluginbase.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/models/urlpath.py` & `openedx-django-wiki-2.0.1/wiki/models/urlpath.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/attachments/admin.py` & `openedx-django-wiki-2.0.1/wiki/plugins/attachments/admin.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/attachments/forms.py` & `openedx-django-wiki-2.0.1/wiki/plugins/attachments/forms.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/attachments/markdown_extensions.py` & `openedx-django-wiki-2.0.1/wiki/plugins/attachments/markdown_extensions.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/attachments/migrations/0001_initial.py` & `openedx-django-wiki-2.0.1/wiki/plugins/attachments/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/attachments/models.py` & `openedx-django-wiki-2.0.1/wiki/plugins/attachments/models.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/attachments/settings.py` & `openedx-django-wiki-2.0.1/wiki/plugins/attachments/settings.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/attachments/templates/wiki/plugins/attachments/delete.html` & `openedx-django-wiki-2.0.1/wiki/plugins/attachments/templates/wiki/plugins/attachments/delete.html`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/attachments/templates/wiki/plugins/attachments/history.html` & `openedx-django-wiki-2.0.1/wiki/plugins/attachments/templates/wiki/plugins/attachments/history.html`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/attachments/templates/wiki/plugins/attachments/index.html` & `openedx-django-wiki-2.0.1/wiki/plugins/attachments/templates/wiki/plugins/attachments/index.html`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/attachments/templates/wiki/plugins/attachments/replace.html` & `openedx-django-wiki-2.0.1/wiki/plugins/attachments/templates/wiki/plugins/attachments/replace.html`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/attachments/templates/wiki/plugins/attachments/search.html` & `openedx-django-wiki-2.0.1/wiki/plugins/attachments/templates/wiki/plugins/attachments/search.html`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/attachments/views.py` & `openedx-django-wiki-2.0.1/wiki/plugins/attachments/views.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/attachments/wiki_plugin.py` & `openedx-django-wiki-2.0.1/wiki/plugins/attachments/wiki_plugin.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/help/templates/wiki/plugins/help/sidebar.html` & `openedx-django-wiki-2.0.1/wiki/plugins/help/templates/wiki/plugins/help/sidebar.html`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/help/wiki_plugin.py` & `openedx-django-wiki-2.0.1/wiki/plugins/help/wiki_plugin.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/images/admin.py` & `openedx-django-wiki-2.0.1/wiki/plugins/images/admin.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/images/forms.py` & `openedx-django-wiki-2.0.1/wiki/plugins/images/forms.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/images/markdown_extensions.py` & `openedx-django-wiki-2.0.1/wiki/plugins/images/markdown_extensions.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/images/migrations/0001_initial.py` & `openedx-django-wiki-2.0.1/wiki/plugins/images/migrations/0001_initial.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             },
             bases=('wiki.revisionplugin',),
         ),
         migrations.CreateModel(
             name='ImageRevision',
             fields=[
                 ('revisionpluginrevision_ptr', models.OneToOneField(parent_link=True, auto_created=True, primary_key=True, serialize=False, to='wiki.RevisionPluginRevision', on_delete=models.CASCADE)),
-                ('image', models.ImageField(upload_to=wiki.plugins.images.models.upload_path, width_field=b'width', height_field=b'height', max_length=2000, blank=True, null=True)),
+                ('image', models.ImageField(upload_to=wiki.plugins.images.models.upload_path, width_field='width', height_field='height', max_length=2000, blank=True, null=True)),
                 ('width', models.SmallIntegerField(null=True, blank=True)),
                 ('height', models.SmallIntegerField(null=True, blank=True)),
             ],
             options={
                 'ordering': ('-created',),
                 'verbose_name': 'image revision',
                 'verbose_name_plural': 'image revisions',
```

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/images/models.py` & `openedx-django-wiki-2.0.1/wiki/plugins/images/models.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/images/settings.py` & `openedx-django-wiki-2.0.1/wiki/plugins/images/settings.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/colorbox/jquery.colorbox-min.js` & `openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/colorbox/jquery.colorbox-min.js`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/colorbox/jquery.colorbox.js` & `openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/colorbox/jquery.colorbox.js`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/content/flash.html` & `openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/content/flash.html`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/content/homer.jpg` & `openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/content/homer.jpg`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/content/marylou.jpg` & `openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/content/marylou.jpg`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/content/ohoopee1.jpg` & `openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/content/ohoopee1.jpg`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/content/ohoopee2.jpg` & `openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/content/ohoopee2.jpg`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/content/ohoopee3.jpg` & `openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/content/ohoopee3.jpg`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/example1/colorbox.css` & `openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/example1/colorbox.css`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/example1/images/controls.png` & `openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/example1/images/controls.png`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/example1/images/loading.gif` & `openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/example1/images/loading.gif`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/images/static/wiki/colorbox/example1/index.html` & `openedx-django-wiki-2.0.1/wiki/plugins/images/static/wiki/colorbox/example1/index.html`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/images/templates/wiki/plugins/images/index.html` & `openedx-django-wiki-2.0.1/wiki/plugins/images/templates/wiki/plugins/images/index.html`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/images/templates/wiki/plugins/images/purge.html` & `openedx-django-wiki-2.0.1/wiki/plugins/images/templates/wiki/plugins/images/purge.html`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/images/templates/wiki/plugins/images/render.html` & `openedx-django-wiki-2.0.1/wiki/plugins/images/templates/wiki/plugins/images/render.html`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/images/templates/wiki/plugins/images/revision_add.html` & `openedx-django-wiki-2.0.1/wiki/plugins/images/templates/wiki/plugins/images/revision_add.html`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/images/templates/wiki/plugins/images/sidebar.html` & `openedx-django-wiki-2.0.1/wiki/plugins/images/templates/wiki/plugins/images/sidebar.html`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/images/views.py` & `openedx-django-wiki-2.0.1/wiki/plugins/images/views.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/images/wiki_plugin.py` & `openedx-django-wiki-2.0.1/wiki/plugins/images/wiki_plugin.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/links/mdx/djangowikilinks.py` & `openedx-django-wiki-2.0.1/wiki/plugins/links/mdx/djangowikilinks.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/links/mdx/urlize.py` & `openedx-django-wiki-2.0.1/wiki/plugins/links/mdx/urlize.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/links/templates/wiki/plugins/links/sidebar.html` & `openedx-django-wiki-2.0.1/wiki/plugins/links/templates/wiki/plugins/links/sidebar.html`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/links/views.py` & `openedx-django-wiki-2.0.1/wiki/plugins/links/views.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/links/wiki_plugin.py` & `openedx-django-wiki-2.0.1/wiki/plugins/links/wiki_plugin.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/notifications/forms.py` & `openedx-django-wiki-2.0.1/wiki/plugins/notifications/forms.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/notifications/migrations/0001_initial.py` & `openedx-django-wiki-2.0.1/wiki/plugins/notifications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/notifications/models.py` & `openedx-django-wiki-2.0.1/wiki/plugins/notifications/models.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/notifications/static/wiki/plugins/notifications/js/ui.js` & `openedx-django-wiki-2.0.1/wiki/plugins/notifications/static/wiki/plugins/notifications/js/ui.js`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/plugins/notifications/templates/wiki/plugins/notifications/menubaritem.html` & `openedx-django-wiki-2.0.1/wiki/plugins/notifications/templates/wiki/plugins/notifications/menubaritem.html`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/bootstrap/css/bootstrap-responsive.css` & `openedx-django-wiki-2.0.1/wiki/static/wiki/bootstrap/css/bootstrap-responsive.css`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/bootstrap/css/bootstrap-responsive.min.css` & `openedx-django-wiki-2.0.1/wiki/static/wiki/bootstrap/css/bootstrap-responsive.min.css`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/bootstrap/css/bootstrap.css` & `openedx-django-wiki-2.0.1/wiki/static/wiki/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/bootstrap/css/bootstrap.min.css` & `openedx-django-wiki-2.0.1/wiki/static/wiki/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/bootstrap/img/glyphicons-halflings-white.png` & `openedx-django-wiki-2.0.1/wiki/static/wiki/bootstrap/img/glyphicons-halflings-white.png`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/bootstrap/img/glyphicons-halflings.png` & `openedx-django-wiki-2.0.1/wiki/static/wiki/bootstrap/img/glyphicons-halflings.png`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/bootstrap/js/bootstrap.js` & `openedx-django-wiki-2.0.1/wiki/static/wiki/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/bootstrap/js/bootstrap.min.js` & `openedx-django-wiki-2.0.1/wiki/static/wiki/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/img/github_icon.png` & `openedx-django-wiki-2.0.1/wiki/static/wiki/img/github_icon.png`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/js/diff.js` & `openedx-django-wiki-2.0.1/wiki/static/wiki/js/diff.js`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/js/diffview.js` & `openedx-django-wiki-2.0.1/wiki/static/wiki/js/diffview.js`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/js/editor.js` & `openedx-django-wiki-2.0.1/wiki/static/wiki/js/editor.js`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/js/jquery.min.js` & `openedx-django-wiki-2.0.1/wiki/static/wiki/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/jquery.markitup.js` & `openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/jquery.markitup.js`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/admin/images/code.png` & `openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/admin/images/code.png`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/admin/images/picture.png` & `openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/admin/images/picture.png`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/admin/images/preview.png` & `openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/admin/images/preview.png`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/admin/images/quotes.png` & `openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/admin/images/quotes.png`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/admin/set.js` & `openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/admin/set.js`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/admin/style.css` & `openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/admin/style.css`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/default/images/clean.png` & `openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/default/images/clean.png`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/default/images/image.png` & `openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/default/images/image.png`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/default/images/picture.png` & `openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/default/images/picture.png`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/default/images/preview.png` & `openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/default/images/preview.png`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/default/set.js` & `openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/default/set.js`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/default/style.css` & `openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/default/style.css`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/frontend/images/code.png` & `openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/frontend/images/code.png`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/frontend/images/picture.png` & `openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/frontend/images/picture.png`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/frontend/images/preview.png` & `openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/frontend/images/preview.png`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/frontend/images/quotes.png` & `openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/frontend/images/quotes.png`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/frontend/set.js` & `openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/frontend/set.js`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/sets/frontend/style.css` & `openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/sets/frontend/style.css`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-bbcode.png` & `openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-bbcode.png`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-dotclear.png` & `openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-dotclear.png`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-html.png` & `openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-html.png`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-json.png` & `openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-json.png`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-markdown.png` & `openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-markdown.png`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-textile.png` & `openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-textile.png`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-wiki.png` & `openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-wiki.png`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-xml.png` & `openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/markitup/images/bg-editor-xml.png`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/markitup/images/bg-editor.png` & `openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/markitup/images/bg-editor.png`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/markitup/style.css` & `openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/markitup/style.css`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/static/wiki/markitup/skins/simple/style.css` & `openedx-django-wiki-2.0.1/wiki/static/wiki/markitup/skins/simple/style.css`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/templates/wiki/accounts/login.html` & `openedx-django-wiki-2.0.1/wiki/templates/wiki/accounts/login.html`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/templates/wiki/article/create_root.html` & `openedx-django-wiki-2.0.1/wiki/templates/wiki/article/create_root.html`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/templates/wiki/article.html` & `openedx-django-wiki-2.0.1/wiki/templates/wiki/article.html`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/templates/wiki/base.html` & `openedx-django-wiki-2.0.1/wiki/templates/wiki/base.html`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/templates/wiki/create.html` & `openedx-django-wiki-2.0.1/wiki/templates/wiki/create.html`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/templates/wiki/delete.html` & `openedx-django-wiki-2.0.1/wiki/templates/wiki/delete.html`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/templates/wiki/deleted.html` & `openedx-django-wiki-2.0.1/wiki/templates/wiki/deleted.html`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/templates/wiki/dir.html` & `openedx-django-wiki-2.0.1/wiki/templates/wiki/dir.html`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/templates/wiki/edit.html` & `openedx-django-wiki-2.0.1/wiki/templates/wiki/edit.html`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/templates/wiki/error.html` & `openedx-django-wiki-2.0.1/wiki/templates/wiki/error.html`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/templates/wiki/history.html` & `openedx-django-wiki-2.0.1/wiki/templates/wiki/history.html`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/templates/wiki/includes/article_menu.html` & `openedx-django-wiki-2.0.1/wiki/templates/wiki/includes/article_menu.html`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/templates/wiki/includes/breadcrumbs.html` & `openedx-django-wiki-2.0.1/wiki/templates/wiki/includes/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/templates/wiki/includes/editor_sidebar.html` & `openedx-django-wiki-2.0.1/wiki/templates/wiki/includes/editor_sidebar.html`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/templates/wiki/includes/form.html` & `openedx-django-wiki-2.0.1/wiki/templates/wiki/includes/form.html`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/templates/wiki/includes/render.html` & `openedx-django-wiki-2.0.1/wiki/templates/wiki/includes/render.html`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/templates/wiki/includes/revision_info.html` & `openedx-django-wiki-2.0.1/wiki/templates/wiki/includes/revision_info.html`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/templates/wiki/preview_inline.html` & `openedx-django-wiki-2.0.1/wiki/templates/wiki/preview_inline.html`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/templates/wiki/settings.html` & `openedx-django-wiki-2.0.1/wiki/templates/wiki/settings.html`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/templatetags/wiki_tags.py` & `openedx-django-wiki-2.0.1/wiki/templatetags/wiki_tags.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/tests.py` & `openedx-django-wiki-2.0.1/wiki/tests.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/urls.py` & `openedx-django-wiki-2.0.1/wiki/urls.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/views/accounts.py` & `openedx-django-wiki-2.0.1/wiki/views/accounts.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/views/article.py` & `openedx-django-wiki-2.0.1/wiki/views/article.py`

 * *Files identical despite different names*

### Comparing `openedx-django-wiki-2.0.0/wiki/views/mixins.py` & `openedx-django-wiki-2.0.1/wiki/views/mixins.py`

 * *Files identical despite different names*

