# Comparing `tmp/django_welkin-0.0.1b1.tar.gz` & `tmp/django_welkin-0.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_welkin-0.0.1b1.tar", max compression
+gzip compressed data, was "django_welkin-0.0.2a0.tar", max compression
```

## Comparing `django_welkin-0.0.1b1.tar` & `django_welkin-0.0.2a0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0    35149 2022-10-13 23:04:16.167505 django_welkin-0.0.1b1/LICENSE
--rw-r--r--   0        0        0      687 2022-10-13 23:04:16.167505 django_welkin-0.0.1b1/README.md
--rw-r--r--   0        0        0        0 2022-10-13 23:04:16.167505 django_welkin-0.0.1b1/django_welkin/__init__.py
--rw-r--r--   0        0        0     1181 2022-10-13 23:04:16.167505 django_welkin-0.0.1b1/django_welkin/admin.py
--rw-r--r--   0        0        0      135 2022-10-13 23:04:16.167505 django_welkin-0.0.1b1/django_welkin/apps.py
--rw-r--r--   0        0        0      528 2022-10-13 23:04:16.167505 django_welkin-0.0.1b1/django_welkin/forms.py
--rw-r--r--   0        0        0        0 2022-10-13 23:04:16.167505 django_welkin-0.0.1b1/django_welkin/management/__init__.py
--rw-r--r--   0        0        0        0 2022-10-13 23:04:16.167505 django_welkin-0.0.1b1/django_welkin/management/commands/__init__.py
--rw-r--r--   0        0        0     1082 2022-10-13 23:04:16.167505 django_welkin-0.0.1b1/django_welkin/management/commands/welkin_load_configuration.py
--rw-r--r--   0        0        0     5971 2022-10-13 23:04:16.167505 django_welkin-0.0.1b1/django_welkin/management/commands/welkin_sync_models.py
--rw-r--r--   0        0        0     8745 2022-10-13 23:04:16.167505 django_welkin-0.0.1b1/django_welkin/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-10-13 23:04:16.167505 django_welkin-0.0.1b1/django_welkin/migrations/__init__.py
--rw-r--r--   0        0        0      366 2022-10-13 23:04:16.167505 django_welkin-0.0.1b1/django_welkin/models/__init__.py
--rw-r--r--   0        0        0      694 2022-10-13 23:04:16.167505 django_welkin-0.0.1b1/django_welkin/models/base.py
--rw-r--r--   0        0        0     1627 2022-10-13 23:04:16.167505 django_welkin-0.0.1b1/django_welkin/models/calendar.py
--rw-r--r--   0        0        0     1918 2022-10-13 23:04:16.167505 django_welkin-0.0.1b1/django_welkin/models/cdt.py
--rw-r--r--   0        0        0     1330 2022-10-13 23:04:16.167505 django_welkin-0.0.1b1/django_welkin/models/chat.py
--rw-r--r--   0        0        0     1152 2022-10-13 23:04:16.167505 django_welkin-0.0.1b1/django_welkin/models/configuration.py
--rw-r--r--   0        0        0     1679 2022-10-13 23:04:16.167505 django_welkin-0.0.1b1/django_welkin/models/patient.py
--rw-r--r--   0        0        0      634 2022-10-13 23:04:16.167505 django_welkin-0.0.1b1/django_welkin/models/user.py
--rw-r--r--   0        0        0      570 2022-10-13 23:04:16.167505 django_welkin-0.0.1b1/django_welkin/models/webhook.py
--rw-r--r--   0        0        0      166 2022-10-13 23:04:16.167505 django_welkin-0.0.1b1/django_welkin/urls.py
--rw-r--r--   0        0        0     2196 2022-10-13 23:04:16.167505 django_welkin-0.0.1b1/django_welkin/views.py
--rw-r--r--   0        0        0     1346 2022-10-13 23:04:16.171505 django_welkin-0.0.1b1/pyproject.toml
--rw-r--r--   0        0        0     1556 1970-01-01 00:00:00.000000 django_welkin-0.0.1b1/setup.py
--rw-r--r--   0        0        0     1959 1970-01-01 00:00:00.000000 django_welkin-0.0.1b1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-08 20:34:49.851515 django_welkin-0.0.2a0/LICENSE
+-rw-r--r--   0        0        0      986 2023-08-08 20:34:49.851515 django_welkin-0.0.2a0/README.md
+-rw-r--r--   0        0        0        0 2023-08-08 20:34:49.851515 django_welkin-0.0.2a0/django_welkin/__init__.py
+-rw-r--r--   0        0        0     1181 2023-08-08 20:34:49.851515 django_welkin-0.0.2a0/django_welkin/admin.py
+-rw-r--r--   0        0        0      291 2023-08-08 20:34:49.851515 django_welkin-0.0.2a0/django_welkin/apps.py
+-rw-r--r--   0        0        0      528 2023-08-08 20:34:49.855515 django_welkin-0.0.2a0/django_welkin/forms.py
+-rw-r--r--   0        0        0        0 2023-08-08 20:34:49.855515 django_welkin-0.0.2a0/django_welkin/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 20:34:49.855515 django_welkin-0.0.2a0/django_welkin/management/commands/__init__.py
+-rw-r--r--   0        0        0     1082 2023-08-08 20:34:49.855515 django_welkin-0.0.2a0/django_welkin/management/commands/welkin_load_configuration.py
+-rw-r--r--   0        0        0     6121 2023-08-08 20:34:49.855515 django_welkin-0.0.2a0/django_welkin/management/commands/welkin_sync_models.py
+-rw-r--r--   0        0        0     8745 2023-08-08 20:34:49.855515 django_welkin-0.0.2a0/django_welkin/migrations/0001_initial.py
+-rw-r--r--   0        0        0      723 2023-08-08 20:34:49.855515 django_welkin-0.0.2a0/django_welkin/migrations/0002_alter_configuration_id_alter_webhookmessage_id.py
+-rw-r--r--   0        0        0      891 2023-08-08 20:34:49.855515 django_welkin-0.0.2a0/django_welkin/migrations/0003_user_email_alter_configuration_id_and_more.py
+-rw-r--r--   0        0        0        0 2023-08-08 20:34:49.855515 django_welkin-0.0.2a0/django_welkin/migrations/__init__.py
+-rw-r--r--   0        0        0      366 2023-08-08 20:34:49.855515 django_welkin-0.0.2a0/django_welkin/models/__init__.py
+-rw-r--r--   0        0        0      694 2023-08-08 20:34:49.855515 django_welkin-0.0.2a0/django_welkin/models/base.py
+-rw-r--r--   0        0        0     1627 2023-08-08 20:34:49.855515 django_welkin-0.0.2a0/django_welkin/models/calendar.py
+-rw-r--r--   0        0        0     1918 2023-08-08 20:34:49.855515 django_welkin-0.0.2a0/django_welkin/models/cdt.py
+-rw-r--r--   0        0        0     1330 2023-08-08 20:34:49.855515 django_welkin-0.0.2a0/django_welkin/models/chat.py
+-rw-r--r--   0        0        0     1152 2023-08-08 20:34:49.855515 django_welkin-0.0.2a0/django_welkin/models/configuration.py
+-rw-r--r--   0        0        0     1679 2023-08-08 20:34:49.855515 django_welkin-0.0.2a0/django_welkin/models/patient.py
+-rw-r--r--   0        0        0      754 2023-08-08 20:34:49.855515 django_welkin-0.0.2a0/django_welkin/models/user.py
+-rw-r--r--   0        0        0      570 2023-08-08 20:34:49.855515 django_welkin-0.0.2a0/django_welkin/models/webhook.py
+-rw-r--r--   0        0        0      166 2023-08-08 20:34:49.855515 django_welkin-0.0.2a0/django_welkin/urls.py
+-rw-r--r--   0        0        0     2196 2023-08-08 20:34:49.855515 django_welkin-0.0.2a0/django_welkin/views.py
+-rw-r--r--   0        0        0     1617 2023-08-08 20:34:49.855515 django_welkin-0.0.2a0/pyproject.toml
+-rw-r--r--   0        0        0     2258 1970-01-01 00:00:00.000000 django_welkin-0.0.2a0/PKG-INFO
```

### Comparing `django_welkin-0.0.1b1/LICENSE` & `django_welkin-0.0.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_welkin-0.0.1b1/django_welkin/admin.py` & `django_welkin-0.0.2a0/django_welkin/admin.py`

 * *Files identical despite different names*

### Comparing `django_welkin-0.0.1b1/django_welkin/forms.py` & `django_welkin-0.0.2a0/django_welkin/forms.py`

 * *Files identical despite different names*

### Comparing `django_welkin-0.0.1b1/django_welkin/management/commands/welkin_load_configuration.py` & `django_welkin-0.0.2a0/django_welkin/management/commands/welkin_load_configuration.py`

 * *Files identical despite different names*

### Comparing `django_welkin-0.0.1b1/django_welkin/management/commands/welkin_sync_models.py` & `django_welkin-0.0.2a0/django_welkin/management/commands/welkin_sync_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from datetime import datetime, timedelta, timezone
 
 from django.core.exceptions import ObjectDoesNotExist
 from django.core.management.base import BaseCommand
+from django.conf import settings
 from django.db import IntegrityError
 from django.utils.dateparse import parse_datetime
 from welkin.exceptions import WelkinHTTPError
 from welkin.models.formation import FormationDataType
 
+
 from ...models import CDT, CalendarEvent, CDTRecord, Patient, User
 from ...models.base import _Welkin
 
+# TODO: send out a warning to indicate this will removed soon
+SYNC_ROLES = settings.WELKIN_SYNC_ROLES or ["health-coach", "physician"]
 
 # pylint: disable=no-member
 class Command(BaseCommand):
     help = "Refresh Welkin data in the DB"  # noqa: A003
 
     def handle(self, *args, **options):
         client = _Welkin()
@@ -39,15 +43,15 @@
     def sync_users(self, client):
         self.stdout.write("Refreshing users")
         for user in client.Users().get(paginate=True):
             for role in user.roles:
                 if role["instanceName"] != client.instance:
                     continue
 
-                if role["permissionName"] in ["health-coach", "physician"]:
+                if role["permissionName"] in SYNC_ROLES:
                     User.objects.update_or_create(
                         id=user.id,
                         defaults={
                             "first_name": user.firstName,
                             "last_name": user.lastName,
                         },
                     )
```

### Comparing `django_welkin-0.0.1b1/django_welkin/migrations/0001_initial.py` & `django_welkin-0.0.2a0/django_welkin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_welkin-0.0.1b1/django_welkin/models/base.py` & `django_welkin-0.0.2a0/django_welkin/models/base.py`

 * *Files identical despite different names*

### Comparing `django_welkin-0.0.1b1/django_welkin/models/calendar.py` & `django_welkin-0.0.2a0/django_welkin/models/calendar.py`

 * *Files identical despite different names*

### Comparing `django_welkin-0.0.1b1/django_welkin/models/cdt.py` & `django_welkin-0.0.2a0/django_welkin/models/cdt.py`

 * *Files identical despite different names*

### Comparing `django_welkin-0.0.1b1/django_welkin/models/chat.py` & `django_welkin-0.0.2a0/django_welkin/models/chat.py`

 * *Files identical despite different names*

### Comparing `django_welkin-0.0.1b1/django_welkin/models/configuration.py` & `django_welkin-0.0.2a0/django_welkin/models/configuration.py`

 * *Files identical despite different names*

### Comparing `django_welkin-0.0.1b1/django_welkin/models/patient.py` & `django_welkin-0.0.2a0/django_welkin/models/patient.py`

 * *Files identical despite different names*

### Comparing `django_welkin-0.0.1b1/django_welkin/models/user.py` & `django_welkin-0.0.2a0/django_welkin/models/user.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 
 from .base import WelkinModel, _Welkin
 
 
 class User(WelkinModel):
     first_name = models.CharField(_("first name"), max_length=255)
     last_name = models.CharField(_("last name"), max_length=255)
+    email = models.CharField(
+        _("email"),
+        max_length=255,
+        blank=True,
+        default="",
+    )
 
     class Meta:
         verbose_name = _("user")
         verbose_name_plural = _("users")
 
     def __str__(self):
         return f"{self.first_name} {self.last_name}"
```

### Comparing `django_welkin-0.0.1b1/django_welkin/models/webhook.py` & `django_welkin-0.0.2a0/django_welkin/models/webhook.py`

 * *Files identical despite different names*

### Comparing `django_welkin-0.0.1b1/django_welkin/views.py` & `django_welkin-0.0.2a0/django_welkin/views.py`

 * *Files identical despite different names*

### Comparing `django_welkin-0.0.1b1/PKG-INFO` & `django_welkin-0.0.2a0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: django-welkin
-Version: 0.0.1b1
+Version: 0.0.2a0
 Summary: A Django app interfacing with the Welkin API.
 Home-page: https://pypi.org/project/django-welkin/
 License: GPL-3.0-or-later
 Author: Sam Morgan
 Author-email: sam@lightmatter.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Dist: django-solo (>=2.0.0,<3.0.0)
-Requires-Dist: welkin (>=0.0.6,<0.0.7)
+Requires-Dist: welkin (>=0.0.6,<0.0.8)
 Project-URL: Documentation, https://django-welkin.readthedocs.io/
 Project-URL: Repository, https://github.com/lightmatter/django-welkin
 Description-Content-Type: text/markdown
 
 # Welkin
 
 Welkin is a Django app to connect to the Welkin Health API.
@@ -57,7 +57,17 @@
 ```
 
 4. Run `python manage.py migrate` to create the welkin models.
 
 5. Start the development server and visit http://localhost:8000/admin/welkin/configuration/
    to and add API secrets to the singleton (you'll need the Admin app enabled).
 
+## Configuration
+
+### Syncing Users
+The sync command will only sync the users who have one of the roles in `settings.WELKIN_SYNC_ROLES`.
+When set this should be a list containing the roles that are allowed to be synced.
+For instance by default this list is:
+```py
+["health-coach", "physician"]
+```
+
```

