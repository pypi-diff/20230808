# Comparing `tmp/django-silly-stripe-1.0.3.tar.gz` & `tmp/django-silly-stripe-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-silly-stripe-1.0.3.tar", last modified: Thu Aug  3 16:13:07 2023, max compression
+gzip compressed data, was "django-silly-stripe-1.0.4.tar", last modified: Tue Aug  8 15:02:48 2023, max compression
```

## Comparing `django-silly-stripe-1.0.3.tar` & `django-silly-stripe-1.0.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-08-03 16:13:07.174409 django-silly-stripe-1.0.3/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1072 2023-03-30 21:48:27.000000 django-silly-stripe-1.0.3/LICENSE.md
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      869 2023-08-03 16:13:07.174409 django-silly-stripe-1.0.3/PKG-INFO
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      246 2023-08-01 21:29:17.000000 django-silly-stripe-1.0.3/README.md
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-08-03 16:13:07.166410 django-silly-stripe-1.0.3/django_silly_stripe/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       52 2023-08-01 15:29:31.000000 django-silly-stripe-1.0.3/django_silly_stripe/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1973 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.3/django_silly_stripe/admin.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1495 2023-08-03 15:17:42.000000 django-silly-stripe-1.0.3/django_silly_stripe/conf.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1446 2023-08-03 15:22:25.000000 django-silly-stripe-1.0.3/django_silly_stripe/helpers.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-08-03 16:13:07.174409 django-silly-stripe-1.0.3/django_silly_stripe/migrations/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      931 2023-07-16 19:12:41.000000 django-silly-stripe-1.0.3/django_silly_stripe/migrations/0001_initial.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      620 2023-07-17 19:35:25.000000 django-silly-stripe-1.0.3/django_silly_stripe/migrations/0002_alter_customer_user.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      552 2023-07-24 13:54:55.000000 django-silly-stripe-1.0.3/django_silly_stripe/migrations/0003_remove_customer_stripe_id_alter_customer_id.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      458 2023-07-24 13:54:55.000000 django-silly-stripe-1.0.3/django_silly_stripe/migrations/0004_customer_email.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      414 2023-07-24 13:54:55.000000 django-silly-stripe-1.0.3/django_silly_stripe/migrations/0005_customer_name.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1889 2023-07-24 13:54:55.000000 django-silly-stripe-1.0.3/django_silly_stripe/migrations/0006_product_price.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      398 2023-07-24 13:54:55.000000 django-silly-stripe-1.0.3/django_silly_stripe/migrations/0007_price_metadata.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      868 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.3/django_silly_stripe/migrations/0008_subscription.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      814 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.3/django_silly_stripe/migrations/0009_subscription_end_time_subscription_start_time_and_more.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      603 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.3/django_silly_stripe/migrations/0010_alter_subscription_end_time_and_more.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      435 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.3/django_silly_stripe/migrations/0011_subscription_cancel_at_period_end.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-07-12 12:59:48.000000 django-silly-stripe-1.0.3/django_silly_stripe/migrations/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     3428 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.3/django_silly_stripe/models.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      718 2023-08-01 16:22:24.000000 django-silly-stripe-1.0.3/django_silly_stripe/serializers.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-08-03 16:13:07.174409 django-silly-stripe-1.0.3/django_silly_stripe/templates/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-07-31 14:29:24.000000 django-silly-stripe-1.0.3/django_silly_stripe/templates/__init__.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-08-03 16:13:07.174409 django-silly-stripe-1.0.3/django_silly_stripe/templates/admin/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-07-31 14:29:24.000000 django-silly-stripe-1.0.3/django_silly_stripe/templates/admin/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     6732 2023-07-25 12:20:33.000000 django-silly-stripe-1.0.3/django_silly_stripe/templates/admin/base.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     2203 2023-07-27 16:54:42.000000 django-silly-stripe-1.0.3/django_silly_stripe/urls.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     4149 2023-08-03 15:44:26.000000 django-silly-stripe-1.0.3/django_silly_stripe/views.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     5982 2023-08-03 15:27:58.000000 django-silly-stripe-1.0.3/django_silly_stripe/views_api.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     5268 2023-08-01 18:07:11.000000 django-silly-stripe-1.0.3/django_silly_stripe/views_classic.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-08-03 16:13:07.170410 django-silly-stripe-1.0.3/django_silly_stripe.egg-info/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      869 2023-08-03 16:13:07.000000 django-silly-stripe-1.0.3/django_silly_stripe.egg-info/PKG-INFO
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1390 2023-08-03 16:13:07.000000 django-silly-stripe-1.0.3/django_silly_stripe.egg-info/SOURCES.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        1 2023-08-03 16:13:07.000000 django-silly-stripe-1.0.3/django_silly_stripe.egg-info/dependency_links.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       20 2023-08-03 16:13:07.000000 django-silly-stripe-1.0.3/django_silly_stripe.egg-info/top_level.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2023-08-03 16:13:07.174409 django-silly-stripe-1.0.3/setup.cfg
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)     1744 2023-08-03 16:12:47.000000 django-silly-stripe-1.0.3/setup.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-08-08 15:02:48.052426 django-silly-stripe-1.0.4/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1072 2023-03-30 21:48:27.000000 django-silly-stripe-1.0.4/LICENSE.md
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      869 2023-08-08 15:02:48.052426 django-silly-stripe-1.0.4/PKG-INFO
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      246 2023-08-01 21:29:17.000000 django-silly-stripe-1.0.4/README.md
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-08-08 15:02:48.048426 django-silly-stripe-1.0.4/django_silly_stripe/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       52 2023-08-08 15:00:56.000000 django-silly-stripe-1.0.4/django_silly_stripe/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1973 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.4/django_silly_stripe/admin.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1495 2023-08-08 15:00:56.000000 django-silly-stripe-1.0.4/django_silly_stripe/conf.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1380 2023-08-08 15:00:56.000000 django-silly-stripe-1.0.4/django_silly_stripe/helpers.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-08-08 15:02:48.052426 django-silly-stripe-1.0.4/django_silly_stripe/migrations/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      931 2023-07-16 19:12:41.000000 django-silly-stripe-1.0.4/django_silly_stripe/migrations/0001_initial.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      620 2023-07-17 19:35:25.000000 django-silly-stripe-1.0.4/django_silly_stripe/migrations/0002_alter_customer_user.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      552 2023-07-24 13:54:55.000000 django-silly-stripe-1.0.4/django_silly_stripe/migrations/0003_remove_customer_stripe_id_alter_customer_id.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      458 2023-07-24 13:54:55.000000 django-silly-stripe-1.0.4/django_silly_stripe/migrations/0004_customer_email.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      414 2023-07-24 13:54:55.000000 django-silly-stripe-1.0.4/django_silly_stripe/migrations/0005_customer_name.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1889 2023-07-24 13:54:55.000000 django-silly-stripe-1.0.4/django_silly_stripe/migrations/0006_product_price.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      398 2023-07-24 13:54:55.000000 django-silly-stripe-1.0.4/django_silly_stripe/migrations/0007_price_metadata.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      868 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.4/django_silly_stripe/migrations/0008_subscription.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      814 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.4/django_silly_stripe/migrations/0009_subscription_end_time_subscription_start_time_and_more.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      603 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.4/django_silly_stripe/migrations/0010_alter_subscription_end_time_and_more.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      435 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.4/django_silly_stripe/migrations/0011_subscription_cancel_at_period_end.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-07-12 12:59:48.000000 django-silly-stripe-1.0.4/django_silly_stripe/migrations/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     3428 2023-07-26 18:49:17.000000 django-silly-stripe-1.0.4/django_silly_stripe/models.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      718 2023-08-01 16:22:24.000000 django-silly-stripe-1.0.4/django_silly_stripe/serializers.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-08-08 15:02:48.052426 django-silly-stripe-1.0.4/django_silly_stripe/templates/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-07-31 14:29:24.000000 django-silly-stripe-1.0.4/django_silly_stripe/templates/__init__.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-08-08 15:02:48.052426 django-silly-stripe-1.0.4/django_silly_stripe/templates/admin/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-07-31 14:29:24.000000 django-silly-stripe-1.0.4/django_silly_stripe/templates/admin/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     6732 2023-07-25 12:20:33.000000 django-silly-stripe-1.0.4/django_silly_stripe/templates/admin/base.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     2203 2023-07-27 16:54:42.000000 django-silly-stripe-1.0.4/django_silly_stripe/urls.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     4149 2023-08-08 15:00:56.000000 django-silly-stripe-1.0.4/django_silly_stripe/views.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     5982 2023-08-03 15:27:58.000000 django-silly-stripe-1.0.4/django_silly_stripe/views_api.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     5268 2023-08-01 18:07:11.000000 django-silly-stripe-1.0.4/django_silly_stripe/views_classic.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-08-08 15:02:48.048426 django-silly-stripe-1.0.4/django_silly_stripe.egg-info/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      869 2023-08-08 15:02:48.000000 django-silly-stripe-1.0.4/django_silly_stripe.egg-info/PKG-INFO
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1390 2023-08-08 15:02:48.000000 django-silly-stripe-1.0.4/django_silly_stripe.egg-info/SOURCES.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        1 2023-08-08 15:02:48.000000 django-silly-stripe-1.0.4/django_silly_stripe.egg-info/dependency_links.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       20 2023-08-08 15:02:48.000000 django-silly-stripe-1.0.4/django_silly_stripe.egg-info/top_level.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2023-08-08 15:02:48.052426 django-silly-stripe-1.0.4/setup.cfg
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)     1744 2023-08-08 15:00:56.000000 django-silly-stripe-1.0.4/setup.py
```

### Comparing `django-silly-stripe-1.0.3/LICENSE.md` & `django-silly-stripe-1.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.3/PKG-INFO` & `django-silly-stripe-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-silly-stripe
-Version: 1.0.3
+Version: 1.0.4
 Summary: Wrapper package for python stripe with Django and/or DRF
 Home-page: https://github.com/byoso/django-silly-stripe
 Author: Vincent Fabre
 Author-email: peigne.plume@gmail.com
 License: MIT
 Keywords: django stripe
 Platform: UNKNOWN
```

### Comparing `django-silly-stripe-1.0.3/django_silly_stripe/admin.py` & `django-silly-stripe-1.0.4/django_silly_stripe/admin.py`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.3/django_silly_stripe/conf.py` & `django-silly-stripe-1.0.4/django_silly_stripe/conf.py`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.3/django_silly_stripe/helpers.py` & `django-silly-stripe-1.0.4/django_silly_stripe/helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,21 +4,18 @@
 from django.db.models import Q
 from django.db.models import QuerySet
 
 
 from .conf import SILLY_STRIPE as dss_conf
 
 
-def dev_log(message, *args, **kwargs):
+def dev_log(*args, **kwargs):
     """Prints a message if PRINT_DEV_LOGS is True."""
-    text = message
-    for arg in args:
-        text += str(arg)
     if dss_conf["PRINT_DEV_LOGS"]:
-        print(text)
+        print(args, kwargs)
 
 
 def user_creates_new_customer(user):
     """If a user does not have a customer, creates one.
     Returns the user."""
     if hasattr(user, 'customer'):
         return user
```

### Comparing `django-silly-stripe-1.0.3/django_silly_stripe/migrations/0001_initial.py` & `django-silly-stripe-1.0.4/django_silly_stripe/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.3/django_silly_stripe/migrations/0002_alter_customer_user.py` & `django-silly-stripe-1.0.4/django_silly_stripe/migrations/0002_alter_customer_user.py`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.3/django_silly_stripe/migrations/0003_remove_customer_stripe_id_alter_customer_id.py` & `django-silly-stripe-1.0.4/django_silly_stripe/migrations/0003_remove_customer_stripe_id_alter_customer_id.py`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.3/django_silly_stripe/migrations/0006_product_price.py` & `django-silly-stripe-1.0.4/django_silly_stripe/migrations/0006_product_price.py`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.3/django_silly_stripe/migrations/0008_subscription.py` & `django-silly-stripe-1.0.4/django_silly_stripe/migrations/0008_subscription.py`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.3/django_silly_stripe/migrations/0009_subscription_end_time_subscription_start_time_and_more.py` & `django-silly-stripe-1.0.4/django_silly_stripe/migrations/0009_subscription_end_time_subscription_start_time_and_more.py`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.3/django_silly_stripe/migrations/0010_alter_subscription_end_time_and_more.py` & `django-silly-stripe-1.0.4/django_silly_stripe/migrations/0010_alter_subscription_end_time_and_more.py`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.3/django_silly_stripe/models.py` & `django-silly-stripe-1.0.4/django_silly_stripe/models.py`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.3/django_silly_stripe/serializers.py` & `django-silly-stripe-1.0.4/django_silly_stripe/serializers.py`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.3/django_silly_stripe/templates/admin/base.html` & `django-silly-stripe-1.0.4/django_silly_stripe/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.3/django_silly_stripe/urls.py` & `django-silly-stripe-1.0.4/django_silly_stripe/urls.py`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.3/django_silly_stripe/views.py` & `django-silly-stripe-1.0.4/django_silly_stripe/views.py`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.3/django_silly_stripe/views_api.py` & `django-silly-stripe-1.0.4/django_silly_stripe/views_api.py`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.3/django_silly_stripe/views_classic.py` & `django-silly-stripe-1.0.4/django_silly_stripe/views_classic.py`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.3/django_silly_stripe.egg-info/PKG-INFO` & `django-silly-stripe-1.0.4/django_silly_stripe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-silly-stripe
-Version: 1.0.3
+Version: 1.0.4
 Summary: Wrapper package for python stripe with Django and/or DRF
 Home-page: https://github.com/byoso/django-silly-stripe
 Author: Vincent Fabre
 Author-email: peigne.plume@gmail.com
 License: MIT
 Keywords: django stripe
 Platform: UNKNOWN
```

### Comparing `django-silly-stripe-1.0.3/django_silly_stripe.egg-info/SOURCES.txt` & `django-silly-stripe-1.0.4/django_silly_stripe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-silly-stripe-1.0.3/setup.py` & `django-silly-stripe-1.0.4/setup.py`

 * *Files identical despite different names*

