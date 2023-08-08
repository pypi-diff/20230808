# Comparing `tmp/django-post_office-3.7.0.tar.gz` & `tmp/django-post_office-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-post_office-3.7.0.tar", last modified: Tue May 30 04:47:13 2023, max compression
+gzip compressed data, was "django-post_office-3.7.1.tar", last modified: Tue Aug  8 12:56:49 2023, max compression
```

## Comparing `django-post_office-3.7.0.tar` & `django-post_office-3.7.1.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.958333 django-post_office-3.7.0/
--rw-r--r--   0 selwin     (501) staff       (20)      342 2021-12-21 05:02:58.000000 django-post_office-3.7.0/AUTHORS.rst
--rw-r--r--   0 selwin     (501) staff       (20)     1053 2017-12-06 05:45:13.000000 django-post_office-3.7.0/LICENSE.txt
--rw-r--r--   0 selwin     (501) staff       (20)      257 2022-10-27 07:39:26.000000 django-post_office-3.7.0/MANIFEST.in
--rw-r--r--   0 selwin     (501) staff       (20)    26166 2023-05-30 04:47:13.958213 django-post_office-3.7.0/PKG-INFO
--rw-r--r--   0 selwin     (501) staff       (20)    24967 2023-05-30 04:31:13.000000 django-post_office-3.7.0/README.md
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.947616 django-post_office-3.7.0/django_post_office.egg-info/
--rw-r--r--   0 selwin     (501) staff       (20)    26166 2023-05-30 04:47:13.000000 django-post_office-3.7.0/django_post_office.egg-info/PKG-INFO
--rw-r--r--   0 selwin     (501) staff       (20)     2714 2023-05-30 04:47:13.000000 django-post_office-3.7.0/django_post_office.egg-info/SOURCES.txt
--rw-r--r--   0 selwin     (501) staff       (20)        1 2023-05-30 04:47:13.000000 django-post_office-3.7.0/django_post_office.egg-info/dependency_links.txt
--rw-r--r--   0 selwin     (501) staff       (20)        1 2017-12-06 05:55:06.000000 django-post_office-3.7.0/django_post_office.egg-info/not-zip-safe
--rw-r--r--   0 selwin     (501) staff       (20)       68 2023-05-30 04:47:13.000000 django-post_office-3.7.0/django_post_office.egg-info/requires.txt
--rw-r--r--   0 selwin     (501) staff       (20)       12 2023-05-30 04:47:13.000000 django-post_office-3.7.0/django_post_office.egg-info/top_level.txt
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.951729 django-post_office-3.7.0/post_office/
--rw-r--r--   0 selwin     (501) staff       (20)      323 2021-12-21 05:02:58.000000 django-post_office-3.7.0/post_office/__init__.py
--rw-r--r--   0 selwin     (501) staff       (20)    12134 2022-11-19 11:28:46.000000 django-post_office-3.7.0/post_office/admin.py
--rw-r--r--   0 selwin     (501) staff       (20)      508 2022-10-07 02:18:01.000000 django-post_office-3.7.0/post_office/apps.py
--rw-r--r--   0 selwin     (501) staff       (20)     2687 2023-05-30 04:31:13.000000 django-post_office-3.7.0/post_office/backends.py
--rw-r--r--   0 selwin     (501) staff       (20)      646 2017-12-06 05:45:13.000000 django-post_office-3.7.0/post_office/cache.py
--rw-r--r--   0 selwin     (501) staff       (20)     1137 2020-02-28 08:42:53.000000 django-post_office-3.7.0/post_office/connections.py
--rw-r--r--   0 selwin     (501) staff       (20)     1848 2020-08-22 01:45:58.000000 django-post_office-3.7.0/post_office/fields.py
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.945377 django-post_office-3.7.0/post_office/locale/
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.945055 django-post_office-3.7.0/post_office/locale/de/
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.952106 django-post_office-3.7.0/post_office/locale/de/LC_MESSAGES/
--rw-r--r--   0 selwin     (501) staff       (20)     2724 2020-02-28 08:42:53.000000 django-post_office-3.7.0/post_office/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 selwin     (501) staff       (20)     3710 2020-02-28 08:42:53.000000 django-post_office-3.7.0/post_office/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.945144 django-post_office-3.7.0/post_office/locale/es/
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.952338 django-post_office-3.7.0/post_office/locale/es/LC_MESSAGES/
--rw-r--r--   0 selwin     (501) staff       (20)     1774 2021-12-21 05:02:58.000000 django-post_office-3.7.0/post_office/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 selwin     (501) staff       (20)     2420 2021-12-21 05:02:58.000000 django-post_office-3.7.0/post_office/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.945236 django-post_office-3.7.0/post_office/locale/it/
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.952574 django-post_office-3.7.0/post_office/locale/it/LC_MESSAGES/
--rw-r--r--   0 selwin     (501) staff       (20)     1573 2020-10-31 09:08:42.000000 django-post_office-3.7.0/post_office/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 selwin     (501) staff       (20)     2382 2020-10-31 09:08:42.000000 django-post_office-3.7.0/post_office/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.945325 django-post_office-3.7.0/post_office/locale/pl/
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.952811 django-post_office-3.7.0/post_office/locale/pl/LC_MESSAGES/
--rw-r--r--   0 selwin     (501) staff       (20)     2698 2017-12-06 05:45:13.000000 django-post_office-3.7.0/post_office/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 selwin     (501) staff       (20)     4300 2017-12-06 05:45:13.000000 django-post_office-3.7.0/post_office/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.945411 django-post_office-3.7.0/post_office/locale/ru_RU/
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.953081 django-post_office-3.7.0/post_office/locale/ru_RU/LC_MESSAGES/
--rw-r--r--   0 selwin     (501) staff       (20)     3274 2018-07-24 09:47:33.000000 django-post_office-3.7.0/post_office/locale/ru_RU/LC_MESSAGES/django.mo
--rw-r--r--   0 selwin     (501) staff       (20)     4901 2018-07-24 09:47:33.000000 django-post_office-3.7.0/post_office/locale/ru_RU/LC_MESSAGES/django.po
--rw-r--r--   0 selwin     (501) staff       (20)     4844 2020-12-04 00:14:03.000000 django-post_office-3.7.0/post_office/lockfile.py
--rw-r--r--   0 selwin     (501) staff       (20)     1072 2020-02-28 08:42:53.000000 django-post_office-3.7.0/post_office/logutils.py
--rw-r--r--   0 selwin     (501) staff       (20)    12590 2022-10-07 02:18:01.000000 django-post_office-3.7.0/post_office/mail.py
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.953274 django-post_office-3.7.0/post_office/management/
--rw-r--r--   0 selwin     (501) staff       (20)        0 2017-12-06 05:45:13.000000 django-post_office-3.7.0/post_office/management/__init__.py
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.953583 django-post_office-3.7.0/post_office/management/commands/
--rw-r--r--   0 selwin     (501) staff       (20)        0 2017-12-06 05:45:13.000000 django-post_office-3.7.0/post_office/management/commands/__init__.py
--rw-r--r--   0 selwin     (501) staff       (20)     1191 2021-12-21 05:02:58.000000 django-post_office-3.7.0/post_office/management/commands/cleanup_mail.py
--rw-r--r--   0 selwin     (501) staff       (20)      855 2020-12-04 00:14:03.000000 django-post_office-3.7.0/post_office/management/commands/send_queued_mail.py
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.955220 django-post_office-3.7.0/post_office/migrations/
--rw-r--r--   0 selwin     (501) staff       (20)     4526 2023-05-30 04:31:13.000000 django-post_office-3.7.0/post_office/migrations/0001_initial.py
--rw-r--r--   0 selwin     (501) staff       (20)     5252 2020-02-28 08:42:53.000000 django-post_office-3.7.0/post_office/migrations/0002_add_i18n_and_backend_alias.py
--rw-r--r--   0 selwin     (501) staff       (20)     2512 2020-02-28 08:42:53.000000 django-post_office-3.7.0/post_office/migrations/0003_longer_subject.py
--rw-r--r--   0 selwin     (501) staff       (20)     4917 2023-05-30 04:31:13.000000 django-post_office-3.7.0/post_office/migrations/0004_auto_20160607_0901.py
--rw-r--r--   0 selwin     (501) staff       (20)      391 2020-02-28 08:42:53.000000 django-post_office-3.7.0/post_office/migrations/0005_auto_20170515_0013.py
--rw-r--r--   0 selwin     (501) staff       (20)      370 2020-02-28 08:42:53.000000 django-post_office-3.7.0/post_office/migrations/0006_attachment_mimetype.py
--rw-r--r--   0 selwin     (501) staff       (20)      433 2020-02-28 08:42:53.000000 django-post_office-3.7.0/post_office/migrations/0007_auto_20170731_1342.py
--rw-r--r--   0 selwin     (501) staff       (20)      426 2023-05-30 04:31:13.000000 django-post_office-3.7.0/post_office/migrations/0008_attachment_headers.py
--rw-r--r--   0 selwin     (501) staff       (20)      912 2020-08-22 01:45:58.000000 django-post_office-3.7.0/post_office/migrations/0009_requeued_mode.py
--rw-r--r--   0 selwin     (501) staff       (20)     1481 2020-10-31 09:08:42.000000 django-post_office-3.7.0/post_office/migrations/0010_message_id.py
--rw-r--r--   0 selwin     (501) staff       (20)      957 2020-11-05 07:48:55.000000 django-post_office-3.7.0/post_office/migrations/0011_models_help_text.py
--rw-r--r--   0 selwin     (501) staff       (20)        0 2017-12-06 05:45:13.000000 django-post_office-3.7.0/post_office/migrations/__init__.py
--rw-r--r--   0 selwin     (501) staff       (20)    13246 2023-05-30 04:31:13.000000 django-post_office-3.7.0/post_office/models.py
--rw-r--r--   0 selwin     (501) staff       (20)     5371 2022-10-07 02:18:01.000000 django-post_office-3.7.0/post_office/sanitizer.py
--rw-r--r--   0 selwin     (501) staff       (20)     3388 2023-05-30 04:31:13.000000 django-post_office-3.7.0/post_office/settings.py
--rw-r--r--   0 selwin     (501) staff       (20)      558 2021-12-21 05:02:58.000000 django-post_office-3.7.0/post_office/signals.py
--rw-r--r--   0 selwin     (501) staff       (20)     1534 2020-12-04 00:14:03.000000 django-post_office-3.7.0/post_office/tasks.py
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.955294 django-post_office-3.7.0/post_office/template/
--rw-r--r--   0 selwin     (501) staff       (20)      712 2022-10-07 02:18:01.000000 django-post_office-3.7.0/post_office/template/__init__.py
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.955599 django-post_office-3.7.0/post_office/template/backends/
--rw-r--r--   0 selwin     (501) staff       (20)        0 2020-02-28 08:42:53.000000 django-post_office-3.7.0/post_office/template/backends/__init__.py
--rw-r--r--   0 selwin     (501) staff       (20)     2177 2020-02-28 08:42:53.000000 django-post_office-3.7.0/post_office/template/backends/post_office.py
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.945783 django-post_office-3.7.0/post_office/templates/
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.945822 django-post_office-3.7.0/post_office/templates/admin/
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.945913 django-post_office-3.7.0/post_office/templates/admin/post_office/
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.955720 django-post_office-3.7.0/post_office/templates/admin/post_office/email/
--rw-r--r--   0 selwin     (501) staff       (20)      259 2022-07-04 08:15:16.000000 django-post_office-3.7.0/post_office/templates/admin/post_office/email/change_form.html
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.955838 django-post_office-3.7.0/post_office/templates/admin/post_office/emailtemplate/
--rw-r--r--   0 selwin     (501) staff       (20)     1676 2022-10-27 07:39:26.000000 django-post_office-3.7.0/post_office/templates/admin/post_office/emailtemplate/change_form.html
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.956237 django-post_office-3.7.0/post_office/templatetags/
--rw-r--r--   0 selwin     (501) staff       (20)        0 2020-02-28 08:42:53.000000 django-post_office-3.7.0/post_office/templatetags/__init__.py
--rw-r--r--   0 selwin     (501) staff       (20)     1359 2020-08-22 01:45:58.000000 django-post_office-3.7.0/post_office/templatetags/post_office.py
--rw-r--r--   0 selwin     (501) staff       (20)     3280 2021-12-21 05:02:58.000000 django-post_office-3.7.0/post_office/test_settings.py
--rw-r--r--   0 selwin     (501) staff       (20)      126 2021-12-21 05:02:58.000000 django-post_office-3.7.0/post_office/test_urls.py
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.957996 django-post_office-3.7.0/post_office/tests/
--rw-r--r--   0 selwin     (501) staff       (20)      287 2017-12-06 05:45:13.000000 django-post_office-3.7.0/post_office/tests/__init__.py
--rw-r--r--   0 selwin     (501) staff       (20)     7406 2022-10-27 07:39:26.000000 django-post_office-3.7.0/post_office/tests/test_backends.py
--rw-r--r--   0 selwin     (501) staff       (20)     1437 2017-12-06 05:45:13.000000 django-post_office-3.7.0/post_office/tests/test_cache.py
--rw-r--r--   0 selwin     (501) staff       (20)     6059 2018-07-24 09:47:33.000000 django-post_office-3.7.0/post_office/tests/test_commands.py
--rw-r--r--   0 selwin     (501) staff       (20)      459 2017-12-06 05:45:13.000000 django-post_office-3.7.0/post_office/tests/test_connections.py
--rw-r--r--   0 selwin     (501) staff       (20)     2659 2020-08-22 01:45:58.000000 django-post_office-3.7.0/post_office/tests/test_forms.py
--rw-r--r--   0 selwin     (501) staff       (20)     8316 2023-05-30 04:31:13.000000 django-post_office-3.7.0/post_office/tests/test_html_email.py
--rw-r--r--   0 selwin     (501) staff       (20)     1943 2017-12-06 05:45:13.000000 django-post_office-3.7.0/post_office/tests/test_lockfile.py
--rw-r--r--   0 selwin     (501) staff       (20)    21498 2023-05-30 04:31:13.000000 django-post_office-3.7.0/post_office/tests/test_mail.py
--rw-r--r--   0 selwin     (501) staff       (20)    15050 2020-02-28 08:42:53.000000 django-post_office-3.7.0/post_office/tests/test_models.py
--rw-r--r--   0 selwin     (501) staff       (20)     8552 2020-02-28 08:42:53.000000 django-post_office-3.7.0/post_office/tests/test_utils.py
--rw-r--r--   0 selwin     (501) staff       (20)     1129 2020-02-28 08:42:53.000000 django-post_office-3.7.0/post_office/tests/test_views.py
--rw-r--r--   0 selwin     (501) staff       (20)     5572 2021-12-21 05:02:58.000000 django-post_office-3.7.0/post_office/utils.py
--rw-r--r--   0 selwin     (501) staff       (20)     1365 2020-10-31 09:08:42.000000 django-post_office-3.7.0/post_office/validators.py
--rw-r--r--   0 selwin     (501) staff       (20)        7 2023-05-30 04:42:50.000000 django-post_office-3.7.0/post_office/version.txt
--rw-r--r--   0 selwin     (501) staff       (20)       26 2017-12-06 05:45:13.000000 django-post_office-3.7.0/post_office/views.py
--rw-r--r--   0 selwin     (501) staff       (20)       38 2023-05-30 04:47:13.958363 django-post_office-3.7.0/setup.cfg
--rw-r--r--   0 selwin     (501) staff       (20)     2435 2023-05-30 04:46:49.000000 django-post_office-3.7.0/setup.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-08-08 12:56:49.410705 django-post_office-3.7.1/
+-rw-r--r--   0 selwin     (501) staff       (20)      342 2021-12-21 05:02:58.000000 django-post_office-3.7.1/AUTHORS.rst
+-rw-r--r--   0 selwin     (501) staff       (20)     1053 2017-12-06 05:45:13.000000 django-post_office-3.7.1/LICENSE.txt
+-rw-r--r--   0 selwin     (501) staff       (20)      257 2022-10-27 07:39:26.000000 django-post_office-3.7.1/MANIFEST.in
+-rw-r--r--   0 selwin     (501) staff       (20)    26166 2023-08-08 12:56:49.410553 django-post_office-3.7.1/PKG-INFO
+-rw-r--r--   0 selwin     (501) staff       (20)    24967 2023-05-30 04:31:13.000000 django-post_office-3.7.1/README.md
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-08-08 12:56:49.399675 django-post_office-3.7.1/django_post_office.egg-info/
+-rw-r--r--   0 selwin     (501) staff       (20)    26166 2023-08-08 12:56:49.000000 django-post_office-3.7.1/django_post_office.egg-info/PKG-INFO
+-rw-r--r--   0 selwin     (501) staff       (20)     2714 2023-08-08 12:56:49.000000 django-post_office-3.7.1/django_post_office.egg-info/SOURCES.txt
+-rw-r--r--   0 selwin     (501) staff       (20)        1 2023-08-08 12:56:49.000000 django-post_office-3.7.1/django_post_office.egg-info/dependency_links.txt
+-rw-r--r--   0 selwin     (501) staff       (20)        1 2017-12-06 05:55:06.000000 django-post_office-3.7.1/django_post_office.egg-info/not-zip-safe
+-rw-r--r--   0 selwin     (501) staff       (20)       68 2023-08-08 12:56:49.000000 django-post_office-3.7.1/django_post_office.egg-info/requires.txt
+-rw-r--r--   0 selwin     (501) staff       (20)       12 2023-08-08 12:56:49.000000 django-post_office-3.7.1/django_post_office.egg-info/top_level.txt
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-08-08 12:56:49.403756 django-post_office-3.7.1/post_office/
+-rw-r--r--   0 selwin     (501) staff       (20)      323 2021-12-21 05:02:58.000000 django-post_office-3.7.1/post_office/__init__.py
+-rw-r--r--   0 selwin     (501) staff       (20)    12098 2023-08-08 08:40:37.000000 django-post_office-3.7.1/post_office/admin.py
+-rw-r--r--   0 selwin     (501) staff       (20)      508 2022-10-07 02:18:01.000000 django-post_office-3.7.1/post_office/apps.py
+-rw-r--r--   0 selwin     (501) staff       (20)     2687 2023-05-30 04:31:13.000000 django-post_office-3.7.1/post_office/backends.py
+-rw-r--r--   0 selwin     (501) staff       (20)      646 2017-12-06 05:45:13.000000 django-post_office-3.7.1/post_office/cache.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1137 2020-02-28 08:42:53.000000 django-post_office-3.7.1/post_office/connections.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1848 2020-08-22 01:45:58.000000 django-post_office-3.7.1/post_office/fields.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-08-08 12:56:49.397488 django-post_office-3.7.1/post_office/locale/
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-08-08 12:56:49.397182 django-post_office-3.7.1/post_office/locale/de/
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-08-08 12:56:49.403998 django-post_office-3.7.1/post_office/locale/de/LC_MESSAGES/
+-rw-r--r--   0 selwin     (501) staff       (20)     2724 2020-02-28 08:42:53.000000 django-post_office-3.7.1/post_office/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 selwin     (501) staff       (20)     3710 2020-02-28 08:42:53.000000 django-post_office-3.7.1/post_office/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-08-08 12:56:49.397271 django-post_office-3.7.1/post_office/locale/es/
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-08-08 12:56:49.404239 django-post_office-3.7.1/post_office/locale/es/LC_MESSAGES/
+-rw-r--r--   0 selwin     (501) staff       (20)     1774 2021-12-21 05:02:58.000000 django-post_office-3.7.1/post_office/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 selwin     (501) staff       (20)     2420 2021-12-21 05:02:58.000000 django-post_office-3.7.1/post_office/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-08-08 12:56:49.397354 django-post_office-3.7.1/post_office/locale/it/
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-08-08 12:56:49.404483 django-post_office-3.7.1/post_office/locale/it/LC_MESSAGES/
+-rw-r--r--   0 selwin     (501) staff       (20)     1573 2020-10-31 09:08:42.000000 django-post_office-3.7.1/post_office/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 selwin     (501) staff       (20)     2382 2020-10-31 09:08:42.000000 django-post_office-3.7.1/post_office/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-08-08 12:56:49.397438 django-post_office-3.7.1/post_office/locale/pl/
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-08-08 12:56:49.404721 django-post_office-3.7.1/post_office/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 selwin     (501) staff       (20)     2698 2017-12-06 05:45:13.000000 django-post_office-3.7.1/post_office/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 selwin     (501) staff       (20)     4300 2017-12-06 05:45:13.000000 django-post_office-3.7.1/post_office/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-08-08 12:56:49.397521 django-post_office-3.7.1/post_office/locale/ru_RU/
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-08-08 12:56:49.404966 django-post_office-3.7.1/post_office/locale/ru_RU/LC_MESSAGES/
+-rw-r--r--   0 selwin     (501) staff       (20)     3274 2018-07-24 09:47:33.000000 django-post_office-3.7.1/post_office/locale/ru_RU/LC_MESSAGES/django.mo
+-rw-r--r--   0 selwin     (501) staff       (20)     4901 2018-07-24 09:47:33.000000 django-post_office-3.7.1/post_office/locale/ru_RU/LC_MESSAGES/django.po
+-rw-r--r--   0 selwin     (501) staff       (20)     4844 2020-12-04 00:14:03.000000 django-post_office-3.7.1/post_office/lockfile.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1072 2020-02-28 08:42:53.000000 django-post_office-3.7.1/post_office/logutils.py
+-rw-r--r--   0 selwin     (501) staff       (20)    12555 2023-08-08 01:51:12.000000 django-post_office-3.7.1/post_office/mail.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-08-08 12:56:49.405081 django-post_office-3.7.1/post_office/management/
+-rw-r--r--   0 selwin     (501) staff       (20)        0 2017-12-06 05:45:13.000000 django-post_office-3.7.1/post_office/management/__init__.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-08-08 12:56:49.405369 django-post_office-3.7.1/post_office/management/commands/
+-rw-r--r--   0 selwin     (501) staff       (20)        0 2017-12-06 05:45:13.000000 django-post_office-3.7.1/post_office/management/commands/__init__.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1191 2021-12-21 05:02:58.000000 django-post_office-3.7.1/post_office/management/commands/cleanup_mail.py
+-rw-r--r--   0 selwin     (501) staff       (20)      855 2020-12-04 00:14:03.000000 django-post_office-3.7.1/post_office/management/commands/send_queued_mail.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-08-08 12:56:49.407173 django-post_office-3.7.1/post_office/migrations/
+-rw-r--r--   0 selwin     (501) staff       (20)     4526 2023-05-30 04:31:13.000000 django-post_office-3.7.1/post_office/migrations/0001_initial.py
+-rw-r--r--   0 selwin     (501) staff       (20)     5252 2020-02-28 08:42:53.000000 django-post_office-3.7.1/post_office/migrations/0002_add_i18n_and_backend_alias.py
+-rw-r--r--   0 selwin     (501) staff       (20)     2512 2020-02-28 08:42:53.000000 django-post_office-3.7.1/post_office/migrations/0003_longer_subject.py
+-rw-r--r--   0 selwin     (501) staff       (20)     4917 2023-05-30 04:31:13.000000 django-post_office-3.7.1/post_office/migrations/0004_auto_20160607_0901.py
+-rw-r--r--   0 selwin     (501) staff       (20)      391 2020-02-28 08:42:53.000000 django-post_office-3.7.1/post_office/migrations/0005_auto_20170515_0013.py
+-rw-r--r--   0 selwin     (501) staff       (20)      370 2020-02-28 08:42:53.000000 django-post_office-3.7.1/post_office/migrations/0006_attachment_mimetype.py
+-rw-r--r--   0 selwin     (501) staff       (20)      433 2020-02-28 08:42:53.000000 django-post_office-3.7.1/post_office/migrations/0007_auto_20170731_1342.py
+-rw-r--r--   0 selwin     (501) staff       (20)      426 2023-05-30 04:31:13.000000 django-post_office-3.7.1/post_office/migrations/0008_attachment_headers.py
+-rw-r--r--   0 selwin     (501) staff       (20)      912 2020-08-22 01:45:58.000000 django-post_office-3.7.1/post_office/migrations/0009_requeued_mode.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1481 2020-10-31 09:08:42.000000 django-post_office-3.7.1/post_office/migrations/0010_message_id.py
+-rw-r--r--   0 selwin     (501) staff       (20)      957 2020-11-05 07:48:55.000000 django-post_office-3.7.1/post_office/migrations/0011_models_help_text.py
+-rw-r--r--   0 selwin     (501) staff       (20)        0 2017-12-06 05:45:13.000000 django-post_office-3.7.1/post_office/migrations/__init__.py
+-rw-r--r--   0 selwin     (501) staff       (20)    13246 2023-05-30 04:31:13.000000 django-post_office-3.7.1/post_office/models.py
+-rw-r--r--   0 selwin     (501) staff       (20)     5371 2022-10-07 02:18:01.000000 django-post_office-3.7.1/post_office/sanitizer.py
+-rw-r--r--   0 selwin     (501) staff       (20)     3388 2023-05-30 04:31:13.000000 django-post_office-3.7.1/post_office/settings.py
+-rw-r--r--   0 selwin     (501) staff       (20)      558 2021-12-21 05:02:58.000000 django-post_office-3.7.1/post_office/signals.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1534 2020-12-04 00:14:03.000000 django-post_office-3.7.1/post_office/tasks.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-08-08 12:56:49.407257 django-post_office-3.7.1/post_office/template/
+-rw-r--r--   0 selwin     (501) staff       (20)      712 2022-10-07 02:18:01.000000 django-post_office-3.7.1/post_office/template/__init__.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-08-08 12:56:49.407570 django-post_office-3.7.1/post_office/template/backends/
+-rw-r--r--   0 selwin     (501) staff       (20)        0 2020-02-28 08:42:53.000000 django-post_office-3.7.1/post_office/template/backends/__init__.py
+-rw-r--r--   0 selwin     (501) staff       (20)     2177 2020-02-28 08:42:53.000000 django-post_office-3.7.1/post_office/template/backends/post_office.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-08-08 12:56:49.397870 django-post_office-3.7.1/post_office/templates/
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-08-08 12:56:49.397909 django-post_office-3.7.1/post_office/templates/admin/
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-08-08 12:56:49.398005 django-post_office-3.7.1/post_office/templates/admin/post_office/
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-08-08 12:56:49.407705 django-post_office-3.7.1/post_office/templates/admin/post_office/email/
+-rw-r--r--   0 selwin     (501) staff       (20)      259 2022-07-04 08:15:16.000000 django-post_office-3.7.1/post_office/templates/admin/post_office/email/change_form.html
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-08-08 12:56:49.407840 django-post_office-3.7.1/post_office/templates/admin/post_office/emailtemplate/
+-rw-r--r--   0 selwin     (501) staff       (20)     1676 2022-10-27 07:39:26.000000 django-post_office-3.7.1/post_office/templates/admin/post_office/emailtemplate/change_form.html
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-08-08 12:56:49.408144 django-post_office-3.7.1/post_office/templatetags/
+-rw-r--r--   0 selwin     (501) staff       (20)        0 2020-02-28 08:42:53.000000 django-post_office-3.7.1/post_office/templatetags/__init__.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1359 2020-08-22 01:45:58.000000 django-post_office-3.7.1/post_office/templatetags/post_office.py
+-rw-r--r--   0 selwin     (501) staff       (20)     3280 2021-12-21 05:02:58.000000 django-post_office-3.7.1/post_office/test_settings.py
+-rw-r--r--   0 selwin     (501) staff       (20)      126 2021-12-21 05:02:58.000000 django-post_office-3.7.1/post_office/test_urls.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-08-08 12:56:49.410313 django-post_office-3.7.1/post_office/tests/
+-rw-r--r--   0 selwin     (501) staff       (20)      287 2017-12-06 05:45:13.000000 django-post_office-3.7.1/post_office/tests/__init__.py
+-rw-r--r--   0 selwin     (501) staff       (20)     7406 2022-10-27 07:39:26.000000 django-post_office-3.7.1/post_office/tests/test_backends.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1437 2017-12-06 05:45:13.000000 django-post_office-3.7.1/post_office/tests/test_cache.py
+-rw-r--r--   0 selwin     (501) staff       (20)     6059 2018-07-24 09:47:33.000000 django-post_office-3.7.1/post_office/tests/test_commands.py
+-rw-r--r--   0 selwin     (501) staff       (20)      459 2017-12-06 05:45:13.000000 django-post_office-3.7.1/post_office/tests/test_connections.py
+-rw-r--r--   0 selwin     (501) staff       (20)     2659 2020-08-22 01:45:58.000000 django-post_office-3.7.1/post_office/tests/test_forms.py
+-rw-r--r--   0 selwin     (501) staff       (20)     8316 2023-05-30 04:31:13.000000 django-post_office-3.7.1/post_office/tests/test_html_email.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1943 2017-12-06 05:45:13.000000 django-post_office-3.7.1/post_office/tests/test_lockfile.py
+-rw-r--r--   0 selwin     (501) staff       (20)    21498 2023-05-30 04:31:13.000000 django-post_office-3.7.1/post_office/tests/test_mail.py
+-rw-r--r--   0 selwin     (501) staff       (20)    15050 2020-02-28 08:42:53.000000 django-post_office-3.7.1/post_office/tests/test_models.py
+-rw-r--r--   0 selwin     (501) staff       (20)     8552 2020-02-28 08:42:53.000000 django-post_office-3.7.1/post_office/tests/test_utils.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1129 2020-02-28 08:42:53.000000 django-post_office-3.7.1/post_office/tests/test_views.py
+-rw-r--r--   0 selwin     (501) staff       (20)     5727 2023-08-08 08:40:37.000000 django-post_office-3.7.1/post_office/utils.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1365 2020-10-31 09:08:42.000000 django-post_office-3.7.1/post_office/validators.py
+-rw-r--r--   0 selwin     (501) staff       (20)        7 2023-08-08 08:41:14.000000 django-post_office-3.7.1/post_office/version.txt
+-rw-r--r--   0 selwin     (501) staff       (20)       26 2017-12-06 05:45:13.000000 django-post_office-3.7.1/post_office/views.py
+-rw-r--r--   0 selwin     (501) staff       (20)       38 2023-08-08 12:56:49.410741 django-post_office-3.7.1/setup.cfg
+-rw-r--r--   0 selwin     (501) staff       (20)     2435 2023-05-30 04:46:49.000000 django-post_office-3.7.1/setup.py
```

### Comparing `django-post_office-3.7.0/LICENSE.txt` & `django-post_office-3.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/PKG-INFO` & `django-post_office-3.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-post_office
-Version: 3.7.0
+Version: 3.7.1
 Summary: A Django app to monitor and send mail asynchronously, complete with template support.
 Home-page: https://github.com/ui/django-post_office
 Author: Selwin Ong
 Author-email: selwin.ong@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `django-post_office-3.7.0/README.md` & `django-post_office-3.7.1/README.md`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/django_post_office.egg-info/PKG-INFO` & `django-post_office-3.7.1/django_post_office.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-post-office
-Version: 3.7.0
+Version: 3.7.1
 Summary: A Django app to monitor and send mail asynchronously, complete with template support.
 Home-page: https://github.com/ui/django-post_office
 Author: Selwin Ong
 Author-email: selwin.ong@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `django-post_office-3.7.0/django_post_office.egg-info/SOURCES.txt` & `django-post_office-3.7.1/django_post_office.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/admin.py` & `django-post_office-3.7.1/post_office/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,14 @@
 requeue.short_description = 'Requeue selected emails'
 
 
 class EmailAdmin(admin.ModelAdmin):
     list_display = ['truncated_message_id', 'to_display', 'shortened_subject', 'status', 'last_updated', 'scheduled_time', 'use_template']
     search_fields = ['to', 'subject']
     readonly_fields = ['message_id', 'render_subject', 'render_plaintext_body',  'render_html_body']
-    date_hierarchy = 'last_updated'
     inlines = [AttachmentInline, LogInline]
     list_filter = ['status', 'template__language', 'template__name']
     formfield_overrides = {
         CommaSeparatedEmailField: {'widget': CommaSeparatedEmailWidget}
     }
     actions = [requeue]
```

### Comparing `django-post_office-3.7.0/post_office/backends.py` & `django-post_office-3.7.1/post_office/backends.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/cache.py` & `django-post_office-3.7.1/post_office/cache.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/connections.py` & `django-post_office-3.7.1/post_office/connections.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/fields.py` & `django-post_office-3.7.1/post_office/fields.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/locale/de/LC_MESSAGES/django.mo` & `django-post_office-3.7.1/post_office/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/locale/de/LC_MESSAGES/django.po` & `django-post_office-3.7.1/post_office/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/locale/es/LC_MESSAGES/django.mo` & `django-post_office-3.7.1/post_office/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/locale/es/LC_MESSAGES/django.po` & `django-post_office-3.7.1/post_office/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/locale/it/LC_MESSAGES/django.mo` & `django-post_office-3.7.1/post_office/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/locale/it/LC_MESSAGES/django.po` & `django-post_office-3.7.1/post_office/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/locale/pl/LC_MESSAGES/django.mo` & `django-post_office-3.7.1/post_office/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/locale/pl/LC_MESSAGES/django.po` & `django-post_office-3.7.1/post_office/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/locale/ru_RU/LC_MESSAGES/django.mo` & `django-post_office-3.7.1/post_office/locale/ru_RU/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/locale/ru_RU/LC_MESSAGES/django.po` & `django-post_office-3.7.1/post_office/locale/ru_RU/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/lockfile.py` & `django-post_office-3.7.1/post_office/lockfile.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/logutils.py` & `django-post_office-3.7.1/post_office/logutils.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/mail.py` & `django-post_office-3.7.1/post_office/mail.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,19 +182,18 @@
     Returns the queryset of emails eligible for sending – fulfilling these conditions:
      - Status is queued or requeued
      - Has scheduled_time before the current time or is None
      - Has expires_at after the current time or is None
     """
     now = timezone.now()
     query = (
-        (Q(status=STATUS.queued) | Q(status=STATUS.requeued)) &
-        (Q(scheduled_time__lte=now) | Q(scheduled_time__isnull=True)) &
-        (Q(expires_at__gt=now) | Q(expires_at__isnull=True))
+        (Q(scheduled_time__lte=now) | Q(scheduled_time=None)) &
+        (Q(expires_at__gt=now) | Q(expires_at=None))
     )
-    return Email.objects.filter(query) \
+    return Email.objects.filter(query, status__in=[STATUS.queued, STATUS.requeued]) \
                 .select_related('template') \
                 .order_by(*get_sending_order()).prefetch_related('attachments')[:get_batch_size()]
 
 
 def send_queued(processes=1, log_level=None):
     """
     Sends out all queued mails that has scheduled_time less than now or None
```

### Comparing `django-post_office-3.7.0/post_office/management/commands/cleanup_mail.py` & `django-post_office-3.7.1/post_office/management/commands/cleanup_mail.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/management/commands/send_queued_mail.py` & `django-post_office-3.7.1/post_office/management/commands/send_queued_mail.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/migrations/0001_initial.py` & `django-post_office-3.7.1/post_office/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/migrations/0002_add_i18n_and_backend_alias.py` & `django-post_office-3.7.1/post_office/migrations/0002_add_i18n_and_backend_alias.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/migrations/0003_longer_subject.py` & `django-post_office-3.7.1/post_office/migrations/0003_longer_subject.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/migrations/0004_auto_20160607_0901.py` & `django-post_office-3.7.1/post_office/migrations/0004_auto_20160607_0901.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/migrations/0009_requeued_mode.py` & `django-post_office-3.7.1/post_office/migrations/0009_requeued_mode.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/migrations/0010_message_id.py` & `django-post_office-3.7.1/post_office/migrations/0010_message_id.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/migrations/0011_models_help_text.py` & `django-post_office-3.7.1/post_office/migrations/0011_models_help_text.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/models.py` & `django-post_office-3.7.1/post_office/models.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/sanitizer.py` & `django-post_office-3.7.1/post_office/sanitizer.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/settings.py` & `django-post_office-3.7.1/post_office/settings.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/signals.py` & `django-post_office-3.7.1/post_office/signals.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/tasks.py` & `django-post_office-3.7.1/post_office/tasks.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/template/__init__.py` & `django-post_office-3.7.1/post_office/template/__init__.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/template/backends/post_office.py` & `django-post_office-3.7.1/post_office/template/backends/post_office.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/templates/admin/post_office/emailtemplate/change_form.html` & `django-post_office-3.7.1/post_office/templates/admin/post_office/emailtemplate/change_form.html`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/templatetags/post_office.py` & `django-post_office-3.7.1/post_office/templatetags/post_office.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/test_settings.py` & `django-post_office-3.7.1/post_office/test_settings.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/tests/test_backends.py` & `django-post_office-3.7.1/post_office/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/tests/test_cache.py` & `django-post_office-3.7.1/post_office/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/tests/test_commands.py` & `django-post_office-3.7.1/post_office/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/tests/test_forms.py` & `django-post_office-3.7.1/post_office/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/tests/test_html_email.py` & `django-post_office-3.7.1/post_office/tests/test_html_email.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/tests/test_lockfile.py` & `django-post_office-3.7.1/post_office/tests/test_lockfile.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/tests/test_mail.py` & `django-post_office-3.7.1/post_office/tests/test_mail.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/tests/test_models.py` & `django-post_office-3.7.1/post_office/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/tests/test_utils.py` & `django-post_office-3.7.1/post_office/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/tests/test_views.py` & `django-post_office-3.7.1/post_office/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/post_office/utils.py` & `django-post_office-3.7.1/post_office/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -142,27 +142,33 @@
 
 def cleanup_expired_mails(cutoff_date, delete_attachments=True, batch_size=1000):
     """
     Delete all emails before the given cutoff date.
     Optionally also delete pending attachments.
     Return the number of deleted emails and attachments.
     """
-    expired_emails_ids = Email.objects.filter(created__lt=cutoff_date).values_list('id', flat=True)
-    email_id_batches = split_emails(expired_emails_ids, batch_size)
     total_deleted_emails = 0
-    
-    for email_ids in email_id_batches:
-        # Delete email and incr total_deleted_emails counter
+
+    while True:
+        email_ids = Email.objects.filter(created__lt=cutoff_date).values_list('id', flat=True)[:batch_size]
+        if not email_ids:
+            break
+
         _, deleted_data = Email.objects.filter(id__in=email_ids).delete()
         if deleted_data:
             total_deleted_emails += deleted_data['post_office.Email']
 
+    attachments_count = 0
     if delete_attachments:
-        attachments = Attachment.objects.filter(emails=None)
-        for attachment in attachments:
-            # Delete the actual file
-            attachment.file.delete()
-        attachments_count, _ = attachments.delete()
-    else:
-        attachments_count = 0
+        while True:
+            attachments = Attachment.objects.filter(emails=None)[:batch_size]
+            if not attachments:
+                break
+            attachment_ids = set()
+            for attachment in attachments:
+                # Delete the actual file
+                attachment.file.delete()
+                attachment_ids.add(attachment.id)
+            deleted_count, _ = Attachment.objects.filter(id__in=attachment_ids).delete()
+            attachments_count += deleted_count
 
     return total_deleted_emails, attachments_count
```

### Comparing `django-post_office-3.7.0/post_office/validators.py` & `django-post_office-3.7.1/post_office/validators.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.7.0/setup.py` & `django-post_office-3.7.1/setup.py`

 * *Files identical despite different names*

