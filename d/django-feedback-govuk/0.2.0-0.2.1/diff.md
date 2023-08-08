# Comparing `tmp/django_feedback_govuk-0.2.0.tar.gz` & `tmp/django_feedback_govuk-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_feedback_govuk-0.2.0.tar", max compression
+gzip compressed data, was "django_feedback_govuk-0.2.1.tar", max compression
```

## Comparing `django_feedback_govuk-0.2.0.tar` & `django_feedback_govuk-0.2.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1091 2023-03-14 14:16:27.435397 django_feedback_govuk-0.2.0/LICENSE
--rw-r--r--   0        0        0     6594 2023-08-07 15:12:27.827938 django_feedback_govuk-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-03-14 14:16:27.435813 django_feedback_govuk-0.2.0/django_feedback_govuk/__init__.py
--rw-r--r--   0        0        0       95 2023-03-14 14:16:27.435920 django_feedback_govuk-0.2.0/django_feedback_govuk/admin.py
--rw-r--r--   0        0        0     2205 2023-08-07 14:30:01.127714 django_feedback_govuk-0.2.0/django_feedback_govuk/forms.py
--rw-r--r--   0        0        0     1840 2023-03-14 15:01:24.022779 django_feedback_govuk-0.2.0/django_feedback_govuk/migrations/0001_initial.py
--rw-r--r--   0        0        0      599 2023-05-12 10:17:33.056308 django_feedback_govuk-0.2.0/django_feedback_govuk/migrations/0002_alter_feedback_submitter.py
--rw-r--r--   0        0        0     4023 2023-08-04 13:30:00.647927 django_feedback_govuk-0.2.0/django_feedback_govuk/migrations/0003_restructure_feedback.py
--rw-r--r--   0        0        0      466 2023-08-04 14:11:11.967549 django_feedback_govuk-0.2.0/django_feedback_govuk/migrations/0004_alter_basefeedback_id.py
--rw-r--r--   0        0        0        0 2023-03-14 14:16:27.436236 django_feedback_govuk-0.2.0/django_feedback_govuk/migrations/__init__.py
--rw-r--r--   0        0        0      967 2023-08-04 15:03:25.339404 django_feedback_govuk-0.2.0/django_feedback_govuk/models.py
--rw-r--r--   0        0        0      789 2023-04-19 09:27:29.084478 django_feedback_govuk-0.2.0/django_feedback_govuk/notify.py
--rw-r--r--   0        0        0     2409 2023-08-07 15:22:40.806617 django_feedback_govuk-0.2.0/django_feedback_govuk/settings.py
--rw-r--r--   0        0        0     3357 2023-03-14 16:21:30.430574 django_feedback_govuk-0.2.0/django_feedback_govuk/static/django_feedback_govuk/star-rating.css
--rw-r--r--   0        0        0     2339 2023-03-27 15:26:37.000943 django_feedback_govuk-0.2.0/django_feedback_govuk/templates/django_feedback_govuk/includes/pagination.html
--rw-r--r--   0        0        0      180 2023-03-30 14:37:22.279652 django_feedback_govuk-0.2.0/django_feedback_govuk/templates/django_feedback_govuk/partials/confirm.html
--rw-r--r--   0        0        0     1262 2023-08-07 14:54:31.051907 django_feedback_govuk-0.2.0/django_feedback_govuk/templates/django_feedback_govuk/partials/listing.html
--rw-r--r--   0        0        0      394 2023-08-07 09:56:45.202028 django_feedback_govuk-0.2.0/django_feedback_govuk/templates/django_feedback_govuk/partials/submit.html
--rw-r--r--   0        0        0      656 2023-08-08 13:19:15.633440 django_feedback_govuk-0.2.0/django_feedback_govuk/templates/django_feedback_govuk/partials/submitted.html
--rw-r--r--   0        0        0       49 2023-03-14 16:54:07.004331 django_feedback_govuk-0.2.0/django_feedback_govuk/templates/django_feedback_govuk/templates/confirm.html
--rw-r--r--   0        0        0      170 2023-08-07 14:19:10.227646 django_feedback_govuk-0.2.0/django_feedback_govuk/templates/django_feedback_govuk/templates/listing.html
--rw-r--r--   0        0        0       63 2023-08-07 09:56:47.682637 django_feedback_govuk-0.2.0/django_feedback_govuk/templates/django_feedback_govuk/templates/submit.html
--rw-r--r--   0        0        0       50 2023-08-07 14:57:13.037656 django_feedback_govuk-0.2.0/django_feedback_govuk/templates/django_feedback_govuk/templates/submitted.html
--rw-r--r--   0        0        0     1898 2023-03-14 16:54:07.005607 django_feedback_govuk-0.2.0/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/radios.html
--rw-r--r--   0        0        0     1737 2023-03-27 15:26:37.001191 django_feedback_govuk-0.2.0/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/star_rating.html
--rw-r--r--   0        0        0        0 2023-03-14 16:54:07.001284 django_feedback_govuk-0.2.0/django_feedback_govuk/templatetags/__init__.py
--rw-r--r--   0        0        0     2338 2023-08-07 14:57:34.655579 django_feedback_govuk-0.2.0/django_feedback_govuk/templatetags/feedback_tags.py
--rw-r--r--   0        0        0        0 2023-04-19 10:40:19.911848 django_feedback_govuk-0.2.0/django_feedback_govuk/tests/__init__.py
--rw-r--r--   0        0        0      406 2023-04-19 11:01:06.172436 django_feedback_govuk-0.2.0/django_feedback_govuk/tests/factories.py
--rw-r--r--   0        0        0     1923 2023-08-07 15:42:14.291502 django_feedback_govuk-0.2.0/django_feedback_govuk/tests/settings.py
--rw-r--r--   0        0        0     1964 2023-08-08 12:54:38.518706 django_feedback_govuk-0.2.0/django_feedback_govuk/tests/test_views.py
--rw-r--r--   0        0        0      153 2023-04-19 10:48:59.640805 django_feedback_govuk-0.2.0/django_feedback_govuk/tests/urls.py
--rw-r--r--   0        0        0      725 2023-08-07 14:18:02.761750 django_feedback_govuk-0.2.0/django_feedback_govuk/urls.py
--rw-r--r--   0        0        0     5451 2023-08-08 13:16:19.944646 django_feedback_govuk-0.2.0/django_feedback_govuk/views.py
--rw-r--r--   0        0        0     1889 2023-08-08 13:07:33.949621 django_feedback_govuk-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     7791 1970-01-01 00:00:00.000000 django_feedback_govuk-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-03-14 14:16:27.435397 django_feedback_govuk-0.2.1/LICENSE
+-rw-r--r--   0        0        0     6594 2023-08-07 15:12:27.827938 django_feedback_govuk-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-03-14 14:16:27.435813 django_feedback_govuk-0.2.1/django_feedback_govuk/__init__.py
+-rw-r--r--   0        0        0       95 2023-03-14 14:16:27.435920 django_feedback_govuk-0.2.1/django_feedback_govuk/admin.py
+-rw-r--r--   0        0        0     2205 2023-08-07 14:30:01.127714 django_feedback_govuk-0.2.1/django_feedback_govuk/forms.py
+-rw-r--r--   0        0        0     1840 2023-03-14 15:01:24.022779 django_feedback_govuk-0.2.1/django_feedback_govuk/migrations/0001_initial.py
+-rw-r--r--   0        0        0      599 2023-05-12 10:17:33.056308 django_feedback_govuk-0.2.1/django_feedback_govuk/migrations/0002_alter_feedback_submitter.py
+-rw-r--r--   0        0        0     4023 2023-08-04 13:30:00.647927 django_feedback_govuk-0.2.1/django_feedback_govuk/migrations/0003_restructure_feedback.py
+-rw-r--r--   0        0        0      466 2023-08-04 14:11:11.967549 django_feedback_govuk-0.2.1/django_feedback_govuk/migrations/0004_alter_basefeedback_id.py
+-rw-r--r--   0        0        0        0 2023-03-14 14:16:27.436236 django_feedback_govuk-0.2.1/django_feedback_govuk/migrations/__init__.py
+-rw-r--r--   0        0        0      967 2023-08-04 15:03:25.339404 django_feedback_govuk-0.2.1/django_feedback_govuk/models.py
+-rw-r--r--   0        0        0      789 2023-04-19 09:27:29.084478 django_feedback_govuk-0.2.1/django_feedback_govuk/notify.py
+-rw-r--r--   0        0        0     2409 2023-08-07 15:22:40.806617 django_feedback_govuk-0.2.1/django_feedback_govuk/settings.py
+-rw-r--r--   0        0        0     3357 2023-03-14 16:21:30.430574 django_feedback_govuk-0.2.1/django_feedback_govuk/static/django_feedback_govuk/star-rating.css
+-rw-r--r--   0        0        0     2339 2023-03-27 15:26:37.000943 django_feedback_govuk-0.2.1/django_feedback_govuk/templates/django_feedback_govuk/includes/pagination.html
+-rw-r--r--   0        0        0      180 2023-03-30 14:37:22.279652 django_feedback_govuk-0.2.1/django_feedback_govuk/templates/django_feedback_govuk/partials/confirm.html
+-rw-r--r--   0        0        0     1262 2023-08-07 14:54:31.051907 django_feedback_govuk-0.2.1/django_feedback_govuk/templates/django_feedback_govuk/partials/listing.html
+-rw-r--r--   0        0        0      394 2023-08-07 09:56:45.202028 django_feedback_govuk-0.2.1/django_feedback_govuk/templates/django_feedback_govuk/partials/submit.html
+-rw-r--r--   0        0        0      656 2023-08-08 13:19:15.633440 django_feedback_govuk-0.2.1/django_feedback_govuk/templates/django_feedback_govuk/partials/submitted.html
+-rw-r--r--   0        0        0       49 2023-03-14 16:54:07.004331 django_feedback_govuk-0.2.1/django_feedback_govuk/templates/django_feedback_govuk/templates/confirm.html
+-rw-r--r--   0        0        0      170 2023-08-07 14:19:10.227646 django_feedback_govuk-0.2.1/django_feedback_govuk/templates/django_feedback_govuk/templates/listing.html
+-rw-r--r--   0        0        0       63 2023-08-07 09:56:47.682637 django_feedback_govuk-0.2.1/django_feedback_govuk/templates/django_feedback_govuk/templates/submit.html
+-rw-r--r--   0        0        0       50 2023-08-07 14:57:13.037656 django_feedback_govuk-0.2.1/django_feedback_govuk/templates/django_feedback_govuk/templates/submitted.html
+-rw-r--r--   0        0        0     1898 2023-03-14 16:54:07.005607 django_feedback_govuk-0.2.1/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/radios.html
+-rw-r--r--   0        0        0     1737 2023-03-27 15:26:37.001191 django_feedback_govuk-0.2.1/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/star_rating.html
+-rw-r--r--   0        0        0        0 2023-03-14 16:54:07.001284 django_feedback_govuk-0.2.1/django_feedback_govuk/templatetags/__init__.py
+-rw-r--r--   0        0        0     2338 2023-08-07 14:57:34.655579 django_feedback_govuk-0.2.1/django_feedback_govuk/templatetags/feedback_tags.py
+-rw-r--r--   0        0        0        0 2023-04-19 10:40:19.911848 django_feedback_govuk-0.2.1/django_feedback_govuk/tests/__init__.py
+-rw-r--r--   0        0        0      406 2023-04-19 11:01:06.172436 django_feedback_govuk-0.2.1/django_feedback_govuk/tests/factories.py
+-rw-r--r--   0        0        0     1923 2023-08-07 15:42:14.291502 django_feedback_govuk-0.2.1/django_feedback_govuk/tests/settings.py
+-rw-r--r--   0        0        0     1964 2023-08-08 12:54:38.518706 django_feedback_govuk-0.2.1/django_feedback_govuk/tests/test_views.py
+-rw-r--r--   0        0        0      153 2023-04-19 10:48:59.640805 django_feedback_govuk-0.2.1/django_feedback_govuk/tests/urls.py
+-rw-r--r--   0        0        0      725 2023-08-07 14:18:02.761750 django_feedback_govuk-0.2.1/django_feedback_govuk/urls.py
+-rw-r--r--   0        0        0     5429 2023-08-08 13:32:11.314955 django_feedback_govuk-0.2.1/django_feedback_govuk/views.py
+-rw-r--r--   0        0        0     1889 2023-08-08 13:38:27.749345 django_feedback_govuk-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     7791 1970-01-01 00:00:00.000000 django_feedback_govuk-0.2.1/PKG-INFO
```

### Comparing `django_feedback_govuk-0.2.0/LICENSE` & `django_feedback_govuk-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.0/README.md` & `django_feedback_govuk-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.0/django_feedback_govuk/forms.py` & `django_feedback_govuk-0.2.1/django_feedback_govuk/forms.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.0/django_feedback_govuk/migrations/0001_initial.py` & `django_feedback_govuk-0.2.1/django_feedback_govuk/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.0/django_feedback_govuk/migrations/0002_alter_feedback_submitter.py` & `django_feedback_govuk-0.2.1/django_feedback_govuk/migrations/0002_alter_feedback_submitter.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.0/django_feedback_govuk/migrations/0003_restructure_feedback.py` & `django_feedback_govuk-0.2.1/django_feedback_govuk/migrations/0003_restructure_feedback.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.0/django_feedback_govuk/models.py` & `django_feedback_govuk-0.2.1/django_feedback_govuk/models.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.0/django_feedback_govuk/notify.py` & `django_feedback_govuk-0.2.1/django_feedback_govuk/notify.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.0/django_feedback_govuk/settings.py` & `django_feedback_govuk-0.2.1/django_feedback_govuk/settings.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.0/django_feedback_govuk/static/django_feedback_govuk/star-rating.css` & `django_feedback_govuk-0.2.1/django_feedback_govuk/static/django_feedback_govuk/star-rating.css`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.0/django_feedback_govuk/templates/django_feedback_govuk/includes/pagination.html` & `django_feedback_govuk-0.2.1/django_feedback_govuk/templates/django_feedback_govuk/includes/pagination.html`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.0/django_feedback_govuk/templates/django_feedback_govuk/partials/listing.html` & `django_feedback_govuk-0.2.1/django_feedback_govuk/templates/django_feedback_govuk/partials/listing.html`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.0/django_feedback_govuk/templates/django_feedback_govuk/partials/submitted.html` & `django_feedback_govuk-0.2.1/django_feedback_govuk/templates/django_feedback_govuk/partials/submitted.html`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.0/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/radios.html` & `django_feedback_govuk-0.2.1/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/radios.html`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.0/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/star_rating.html` & `django_feedback_govuk-0.2.1/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/star_rating.html`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.0/django_feedback_govuk/templatetags/feedback_tags.py` & `django_feedback_govuk-0.2.1/django_feedback_govuk/templatetags/feedback_tags.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.0/django_feedback_govuk/tests/settings.py` & `django_feedback_govuk-0.2.1/django_feedback_govuk/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.0/django_feedback_govuk/tests/test_views.py` & `django_feedback_govuk-0.2.1/django_feedback_govuk/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.0/django_feedback_govuk/urls.py` & `django_feedback_govuk-0.2.1/django_feedback_govuk/urls.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.2.0/django_feedback_govuk/views.py` & `django_feedback_govuk-0.2.1/django_feedback_govuk/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,16 +63,15 @@
 
 def feedback_confirm(request):
     return render(request, "django_feedback_govuk/templates/confirm.html")
 
 
 class UserCanViewFeedback(UserPassesTestMixin):
     def test_func(self):
-        return True
-        # return self.request.user.has_perm("django_feedback_govuk.view_feedback")
+        return self.request.user.has_perm("django_feedback_govuk.view_feedback")
 
 
 class SubmittedFeedback(UserCanViewFeedback, TemplateView):
     template_name = "django_feedback_govuk/templates/submitted.html"
 
     def dispatch(
         self, request: http.HttpRequest, *args: Any, **kwargs: Any
```

### Comparing `django_feedback_govuk-0.2.0/pyproject.toml` & `django_feedback_govuk-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-feedback-govuk"
-version = "0.2.0"
+version = "0.2.1"
 description = "A Django app to gather and send internal Government staff feedback"
 authors = [
     "jafacakes2011 <cameron.lamb@digitial.trade.gov.uk>",
     "marcelkornblum <marcel.kornblum@digitial.trade.gov.uk>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `django_feedback_govuk-0.2.0/PKG-INFO` & `django_feedback_govuk-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-feedback-govuk
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Django app to gather and send internal Government staff feedback
 License: MIT
 Author: jafacakes2011
 Author-email: cameron.lamb@digitial.trade.gov.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

