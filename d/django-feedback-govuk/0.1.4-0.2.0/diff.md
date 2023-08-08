# Comparing `tmp/django_feedback_govuk-0.1.4.tar.gz` & `tmp/django_feedback_govuk-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_feedback_govuk-0.1.4.tar", max compression
+gzip compressed data, was "django_feedback_govuk-0.2.0.tar", max compression
```

## Comparing `django_feedback_govuk-0.1.4.tar` & `django_feedback_govuk-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,36 @@
--rw-r--r--   0        0        0     1091 2023-03-14 14:16:27.435397 django_feedback_govuk-0.1.4/LICENSE
--rw-r--r--   0        0        0     3779 2023-07-25 15:16:30.134524 django_feedback_govuk-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-03-14 14:16:27.435813 django_feedback_govuk-0.1.4/django_feedback_govuk/__init__.py
--rw-r--r--   0        0        0       95 2023-03-14 14:16:27.435920 django_feedback_govuk-0.1.4/django_feedback_govuk/admin.py
--rw-r--r--   0        0        0     1701 2023-05-12 10:41:14.673909 django_feedback_govuk-0.1.4/django_feedback_govuk/forms.py
--rw-r--r--   0        0        0     1840 2023-03-14 15:01:24.022779 django_feedback_govuk-0.1.4/django_feedback_govuk/migrations/0001_initial.py
--rw-r--r--   0        0        0      599 2023-05-12 10:17:33.056308 django_feedback_govuk-0.1.4/django_feedback_govuk/migrations/0002_alter_feedback_submitter.py
--rw-r--r--   0        0        0        0 2023-03-14 14:16:27.436236 django_feedback_govuk-0.1.4/django_feedback_govuk/migrations/__init__.py
--rw-r--r--   0        0        0      931 2023-05-12 10:17:33.056402 django_feedback_govuk-0.1.4/django_feedback_govuk/models.py
--rw-r--r--   0        0        0      789 2023-04-19 09:27:29.084478 django_feedback_govuk-0.1.4/django_feedback_govuk/notify.py
--rw-r--r--   0        0        0     2061 2023-03-30 14:40:03.820144 django_feedback_govuk-0.1.4/django_feedback_govuk/settings.py
--rw-r--r--   0        0        0     3357 2023-03-14 16:21:30.430574 django_feedback_govuk-0.1.4/django_feedback_govuk/static/django_feedback_govuk/star-rating.css
--rw-r--r--   0        0        0     2339 2023-03-27 15:26:37.000943 django_feedback_govuk-0.1.4/django_feedback_govuk/templates/django_feedback_govuk/includes/pagination.html
--rw-r--r--   0        0        0      180 2023-03-30 14:37:22.279652 django_feedback_govuk-0.1.4/django_feedback_govuk/templates/django_feedback_govuk/partials/confirm.html
--rw-r--r--   0        0        0     1399 2023-03-27 15:26:37.002076 django_feedback_govuk-0.1.4/django_feedback_govuk/templates/django_feedback_govuk/partials/listing.html
--rw-r--r--   0        0        0      351 2023-05-12 10:41:38.860286 django_feedback_govuk-0.1.4/django_feedback_govuk/templates/django_feedback_govuk/partials/submit.html
--rw-r--r--   0        0        0       49 2023-03-14 16:54:07.004331 django_feedback_govuk-0.1.4/django_feedback_govuk/templates/django_feedback_govuk/templates/confirm.html
--rw-r--r--   0        0        0       49 2023-03-14 16:54:07.001438 django_feedback_govuk-0.1.4/django_feedback_govuk/templates/django_feedback_govuk/templates/listing.html
--rw-r--r--   0        0        0       48 2023-03-14 16:54:07.003157 django_feedback_govuk-0.1.4/django_feedback_govuk/templates/django_feedback_govuk/templates/submit.html
--rw-r--r--   0        0        0     1898 2023-03-14 16:54:07.005607 django_feedback_govuk-0.1.4/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/radios.html
--rw-r--r--   0        0        0     1737 2023-03-27 15:26:37.001191 django_feedback_govuk-0.1.4/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/star_rating.html
--rw-r--r--   0        0        0        0 2023-03-14 16:54:07.001284 django_feedback_govuk-0.1.4/django_feedback_govuk/templatetags/__init__.py
--rw-r--r--   0        0        0     1605 2023-03-30 14:38:34.189260 django_feedback_govuk-0.1.4/django_feedback_govuk/templatetags/feedback_tags.py
--rw-r--r--   0        0        0        0 2023-04-19 10:40:19.911848 django_feedback_govuk-0.1.4/django_feedback_govuk/tests/__init__.py
--rw-r--r--   0        0        0      406 2023-04-19 11:01:06.172436 django_feedback_govuk-0.1.4/django_feedback_govuk/tests/factories.py
--rw-r--r--   0        0        0     1870 2023-04-19 11:05:11.695891 django_feedback_govuk-0.1.4/django_feedback_govuk/tests/settings.py
--rw-r--r--   0        0        0      558 2023-04-19 11:08:49.348404 django_feedback_govuk-0.1.4/django_feedback_govuk/tests/test_views.py
--rw-r--r--   0        0        0      153 2023-04-19 10:48:59.640805 django_feedback_govuk-0.1.4/django_feedback_govuk/tests/urls.py
--rw-r--r--   0        0        0      471 2023-03-27 15:26:37.002513 django_feedback_govuk-0.1.4/django_feedback_govuk/urls.py
--rw-r--r--   0        0        0     1839 2023-07-25 15:06:50.646118 django_feedback_govuk-0.1.4/django_feedback_govuk/views.py
--rw-r--r--   0        0        0     1877 2023-07-25 15:16:30.134442 django_feedback_govuk-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4976 1970-01-01 00:00:00.000000 django_feedback_govuk-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-03-14 14:16:27.435397 django_feedback_govuk-0.2.0/LICENSE
+-rw-r--r--   0        0        0     6594 2023-08-07 15:12:27.827938 django_feedback_govuk-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-03-14 14:16:27.435813 django_feedback_govuk-0.2.0/django_feedback_govuk/__init__.py
+-rw-r--r--   0        0        0       95 2023-03-14 14:16:27.435920 django_feedback_govuk-0.2.0/django_feedback_govuk/admin.py
+-rw-r--r--   0        0        0     2205 2023-08-07 14:30:01.127714 django_feedback_govuk-0.2.0/django_feedback_govuk/forms.py
+-rw-r--r--   0        0        0     1840 2023-03-14 15:01:24.022779 django_feedback_govuk-0.2.0/django_feedback_govuk/migrations/0001_initial.py
+-rw-r--r--   0        0        0      599 2023-05-12 10:17:33.056308 django_feedback_govuk-0.2.0/django_feedback_govuk/migrations/0002_alter_feedback_submitter.py
+-rw-r--r--   0        0        0     4023 2023-08-04 13:30:00.647927 django_feedback_govuk-0.2.0/django_feedback_govuk/migrations/0003_restructure_feedback.py
+-rw-r--r--   0        0        0      466 2023-08-04 14:11:11.967549 django_feedback_govuk-0.2.0/django_feedback_govuk/migrations/0004_alter_basefeedback_id.py
+-rw-r--r--   0        0        0        0 2023-03-14 14:16:27.436236 django_feedback_govuk-0.2.0/django_feedback_govuk/migrations/__init__.py
+-rw-r--r--   0        0        0      967 2023-08-04 15:03:25.339404 django_feedback_govuk-0.2.0/django_feedback_govuk/models.py
+-rw-r--r--   0        0        0      789 2023-04-19 09:27:29.084478 django_feedback_govuk-0.2.0/django_feedback_govuk/notify.py
+-rw-r--r--   0        0        0     2409 2023-08-07 15:22:40.806617 django_feedback_govuk-0.2.0/django_feedback_govuk/settings.py
+-rw-r--r--   0        0        0     3357 2023-03-14 16:21:30.430574 django_feedback_govuk-0.2.0/django_feedback_govuk/static/django_feedback_govuk/star-rating.css
+-rw-r--r--   0        0        0     2339 2023-03-27 15:26:37.000943 django_feedback_govuk-0.2.0/django_feedback_govuk/templates/django_feedback_govuk/includes/pagination.html
+-rw-r--r--   0        0        0      180 2023-03-30 14:37:22.279652 django_feedback_govuk-0.2.0/django_feedback_govuk/templates/django_feedback_govuk/partials/confirm.html
+-rw-r--r--   0        0        0     1262 2023-08-07 14:54:31.051907 django_feedback_govuk-0.2.0/django_feedback_govuk/templates/django_feedback_govuk/partials/listing.html
+-rw-r--r--   0        0        0      394 2023-08-07 09:56:45.202028 django_feedback_govuk-0.2.0/django_feedback_govuk/templates/django_feedback_govuk/partials/submit.html
+-rw-r--r--   0        0        0      656 2023-08-08 13:19:15.633440 django_feedback_govuk-0.2.0/django_feedback_govuk/templates/django_feedback_govuk/partials/submitted.html
+-rw-r--r--   0        0        0       49 2023-03-14 16:54:07.004331 django_feedback_govuk-0.2.0/django_feedback_govuk/templates/django_feedback_govuk/templates/confirm.html
+-rw-r--r--   0        0        0      170 2023-08-07 14:19:10.227646 django_feedback_govuk-0.2.0/django_feedback_govuk/templates/django_feedback_govuk/templates/listing.html
+-rw-r--r--   0        0        0       63 2023-08-07 09:56:47.682637 django_feedback_govuk-0.2.0/django_feedback_govuk/templates/django_feedback_govuk/templates/submit.html
+-rw-r--r--   0        0        0       50 2023-08-07 14:57:13.037656 django_feedback_govuk-0.2.0/django_feedback_govuk/templates/django_feedback_govuk/templates/submitted.html
+-rw-r--r--   0        0        0     1898 2023-03-14 16:54:07.005607 django_feedback_govuk-0.2.0/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/radios.html
+-rw-r--r--   0        0        0     1737 2023-03-27 15:26:37.001191 django_feedback_govuk-0.2.0/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/star_rating.html
+-rw-r--r--   0        0        0        0 2023-03-14 16:54:07.001284 django_feedback_govuk-0.2.0/django_feedback_govuk/templatetags/__init__.py
+-rw-r--r--   0        0        0     2338 2023-08-07 14:57:34.655579 django_feedback_govuk-0.2.0/django_feedback_govuk/templatetags/feedback_tags.py
+-rw-r--r--   0        0        0        0 2023-04-19 10:40:19.911848 django_feedback_govuk-0.2.0/django_feedback_govuk/tests/__init__.py
+-rw-r--r--   0        0        0      406 2023-04-19 11:01:06.172436 django_feedback_govuk-0.2.0/django_feedback_govuk/tests/factories.py
+-rw-r--r--   0        0        0     1923 2023-08-07 15:42:14.291502 django_feedback_govuk-0.2.0/django_feedback_govuk/tests/settings.py
+-rw-r--r--   0        0        0     1964 2023-08-08 12:54:38.518706 django_feedback_govuk-0.2.0/django_feedback_govuk/tests/test_views.py
+-rw-r--r--   0        0        0      153 2023-04-19 10:48:59.640805 django_feedback_govuk-0.2.0/django_feedback_govuk/tests/urls.py
+-rw-r--r--   0        0        0      725 2023-08-07 14:18:02.761750 django_feedback_govuk-0.2.0/django_feedback_govuk/urls.py
+-rw-r--r--   0        0        0     5451 2023-08-08 13:16:19.944646 django_feedback_govuk-0.2.0/django_feedback_govuk/views.py
+-rw-r--r--   0        0        0     1889 2023-08-08 13:07:33.949621 django_feedback_govuk-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7791 1970-01-01 00:00:00.000000 django_feedback_govuk-0.2.0/PKG-INFO
```

### Comparing `django_feedback_govuk-0.1.4/LICENSE` & `django_feedback_govuk-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.4/django_feedback_govuk/forms.py` & `django_feedback_govuk-0.2.0/django_feedback_govuk/forms.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,67 @@
 from crispy_forms_gds.helper import FormHelper
 from crispy_forms_gds.layout import HTML, Field, Fieldset, Hidden, Layout, Size, Submit
-from django.forms import HiddenInput, ModelForm, RadioSelect
+from django.forms import ModelForm, RadioSelect
 
-from .models import Feedback, SatisfactionOptions
-from .settings import dfg_settings
+from django_feedback_govuk.models import BaseFeedback, Feedback, SatisfactionOptions
+from django_feedback_govuk.settings import dfg_settings
 
 
-class FeedbackForm(ModelForm):
+SUBMIT_BUTTON = Submit("submit", "Send feedback")
+
+
+class BaseFeedbackForm(ModelForm):
     class Meta:
-        model = Feedback
-        fields = ["satisfaction", "comment", "submitter"]
+        model = BaseFeedback
+        fields = ["submitter"]
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         submitter = self.initial["submitter"]
         submitter_id = str(submitter.id) if submitter.id else ""
 
         self.fields["submitter"].required = False
+
+        self.helper = FormHelper()
+        self.helper.layout = Layout(
+            Hidden("submitter", submitter_id),
+            SUBMIT_BUTTON,
+        )
+
+
+class FeedbackForm(BaseFeedbackForm):
+    class Meta:
+        model = Feedback
+        fields = ["satisfaction", "comment", "submitter"]
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
         self.fields["satisfaction"].label = ""
         self.fields["satisfaction"].required = True
         self.fields["satisfaction"].widget = RadioSelect()
         self.fields["satisfaction"].choices = SatisfactionOptions.choices
         self.fields["comment"].label = ""
 
-        self.helper = FormHelper()
-        self.helper.layout = Layout(
-            Hidden("submitter", submitter_id),
+        self.helper.layout.remove(SUBMIT_BUTTON)
+        self.helper.layout.append(
             Fieldset(
                 Field.radios(
                     "satisfaction",
                     template="django_feedback_govuk/widgets/star_rating/star_rating.html",
                 ),
                 legend=dfg_settings.COPY_FIELD_SATISFACTION_LEGEND,
                 legend_size=Size.MEDIUM,
-            ),
+            )
+        )
+        self.helper.layout.append(
             Fieldset(
-                HTML(f"<p class='govuk-hint'>{dfg_settings.COPY_FIELD_COMMENT_HINT}</p>"),
+                HTML(
+                    f"<p class='govuk-hint'>{dfg_settings.COPY_FIELD_COMMENT_HINT}</p>"
+                ),
                 Field("comment"),
                 legend=dfg_settings.COPY_FIELD_COMMENT_LEGEND,
                 legend_size=Size.MEDIUM,
-            ),
-            Submit("submit", "Send feedback"),
+            )
         )
-
+        self.helper.layout.append(SUBMIT_BUTTON)
```

### Comparing `django_feedback_govuk-0.1.4/django_feedback_govuk/migrations/0001_initial.py` & `django_feedback_govuk-0.2.0/django_feedback_govuk/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.4/django_feedback_govuk/migrations/0002_alter_feedback_submitter.py` & `django_feedback_govuk-0.2.0/django_feedback_govuk/migrations/0002_alter_feedback_submitter.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.4/django_feedback_govuk/models.py` & `django_feedback_govuk-0.2.0/django_feedback_govuk/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,16 +11,19 @@
     VERY_DISSATISFIED = "very_dissatisfied", "Very dissatisfied"
     DISSATISFIED = "dissatisfied", "Dissatisfied"
     NEUTRAL = "neutral", "Neither satisfied or dissatisfied"
     SATISFIED = "satisfied", "Satisfied"
     VERY_SATISFIED = "very_satisfied", "Very satisfied"
 
 
-class Feedback(models.Model):
-    satisfaction = models.CharField(max_length=30, choices=SatisfactionOptions.choices)
-    comment = models.TextField(blank=True)
+class BaseFeedback(models.Model):
     submitter = models.ForeignKey(get_user_model(), on_delete=models.CASCADE, null=True)
     submitted_at = models.DateTimeField(null=True, auto_now_add=True)
 
     class Meta:
         verbose_name = "Feedback Submission"
         verbose_name_plural = "Feedback Submissions"
+
+
+class Feedback(BaseFeedback):
+    satisfaction = models.CharField(max_length=30, choices=SatisfactionOptions.choices)
+    comment = models.TextField(blank=True)
```

### Comparing `django_feedback_govuk-0.1.4/django_feedback_govuk/notify.py` & `django_feedback_govuk-0.2.0/django_feedback_govuk/notify.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.4/django_feedback_govuk/settings.py` & `django_feedback_govuk-0.2.0/django_feedback_govuk/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,49 @@
-from typing import List
+from typing import Dict, List
 
 from django.conf import settings
 
 
+DEFAULT_FEEDBACK_ID = "default"
+
 DEFAULTS = {
     "SERVICE_NAME": "Example service",
     "FEEDBACK_NOTIFICATION_EMAIL_TEMPLATE_ID": "xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
     "FEEDBACK_NOTIFICATION_EMAIL_RECIPIENTS": [
         "email@example.com",
     ],
     "COPY": {
         "SUBMIT_TITLE": "Give feedback on {{ service_name }}",
         "CONFIRM_TITLE": "Feedback submitted",
         "CONFIRM_BODY": "Thank you for submitting your feedback.",
         "FIELD_SATISFACTION_LEGEND": "Overall, how did you feel about the service you received today?",
         "FIELD_COMMENT_LEGEND": "How could we improve this service?",
         "FIELD_COMMENT_HINT": "Do not include any personal or financial information, for example your National Insurance or credit card numbers.",
     },
+    "FEEDBACK_FORMS": {
+        DEFAULT_FEEDBACK_ID: {
+            "model": "django_feedback_govuk.models.Feedback",
+            "form": "django_feedback_govuk.forms.FeedbackForm",
+            "view": "django_feedback_govuk.views.FeedbackView",
+        },
+    },
 }
 
 
 class DjangoFeedbackGovUKSettings:
     SERVICE_NAME: str
     FEEDBACK_NOTIFICATION_EMAIL_TEMPLATE_ID: str
     FEEDBACK_NOTIFICATION_EMAIL_RECIPIENTS: List[str]
     COPY_SUBMIT_TITLE: str
     COPY_CONFIRM_TITLE: str
     COPY_CONFIRM_BODY: str
     COPY_FIELD_SATISFACTION_LEGEND: str
     COPY_FIELD_COMMENT_LEGEND: str
     COPY_FIELD_COMMENT_HINT: str
+    FEEDBACK_FORMS: Dict[str, Dict[str, str]]
 
     def __getattr__(self, attr):
         django_settings = getattr(settings, "DJANGO_FEEDBACK_GOVUK", {})
 
         # Get COPY values
         if attr.startswith("COPY_"):
             copy_key = attr[5:]
```

### Comparing `django_feedback_govuk-0.1.4/django_feedback_govuk/static/django_feedback_govuk/star-rating.css` & `django_feedback_govuk-0.2.0/django_feedback_govuk/static/django_feedback_govuk/star-rating.css`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.4/django_feedback_govuk/templates/django_feedback_govuk/includes/pagination.html` & `django_feedback_govuk-0.2.0/django_feedback_govuk/templates/django_feedback_govuk/includes/pagination.html`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.4/django_feedback_govuk/templates/django_feedback_govuk/partials/listing.html` & `django_feedback_govuk-0.2.0/django_feedback_govuk/templates/django_feedback_govuk/partials/listing.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,28 @@
+{% load feedback_tags %}
 
 <div class="govuk-grid-row">
     <div class="govuk-grid-column-full">
-        <h1 class="govuk-heading-l">Feedback</h1>
+        <h1 class="govuk-heading-l">Submitted feedback ({{ form_id }})</h1>
         <table class="govuk-table">
             <thead class="govuk-table__head">
                 <tr class="govuk-table__row">
-                    <th scope="col" class="govuk-table__header">How did you feel about the service you received today?</th>
-                    <th scope="col" class="govuk-table__header">How could we improve this service?</th>
-                    <th scope="col" class="govuk-table__header">Submitted by</th>
-                    <th scope="col" class="govuk-table__header">Submitted at</th>
+                    {% for field_name in fields %}
+                        <th scope="col" class="govuk-table__header">{{ form|get_feedback_form_label:field_name }}</th>
+                    {% endfor %}
+                    <th scope="col" class="govuk-table__header">Submitted</th>
                 </tr>
             </thead>
             <tbody class="govuk-table__body">
                 {% for object in page_obj.object_list %}
                     <tr class="govuk-table__row">
-                        <td class="govuk-table__cell">{{ object.get_satisfaction_display }}</td>
-                        <td class="govuk-table__cell">{{ object.comment }}</td>
-                        <td class="govuk-table__cell">{{ object.submitter }}</td>
-                        <td class="govuk-table__cell">{{ object.submitted_at|date:"d/m/Y H:i" }}</td>
+                        {% for field_name in fields %}
+                            <td class="govuk-table__cell">{{ object|get_feedback_value:field_name }}</td>
+                        {% endfor %}
+                        <td class="govuk-table__cell">{{ object.submitted_at }}</td>
                     </tr>
                 {% endfor %}
             </tbody>
         </table>
         {% include "django_feedback_govuk/includes/pagination.html" with page=page_obj %}
     </div>
 </div>
```

#### html2text {}

```diff
@@ -1,10 +1,6 @@
-****** Feedback ******
-How did you feel about the      How could we
-service you received today?     improve this   Submitted by     Submitted at
-                                service?
-{                               {              {                {
-{                               {              {                {
-object.get_satisfaction_display object.comment object.submitter object.submitted_at|date:
-}}                              }}             }}               "d/m/Y H:i" }}
+{% load feedback_tags %}
+****** Submitted feedback ({{ form_id }}) ******
+{{ form|get_feedback_form_label:field_name }} Submitted
+{{ object|get_feedback_value:field_name }}    {{ object.submitted_at }}
 {% include "django_feedback_govuk/includes/pagination.html" with page=page_obj
 %}
```

### Comparing `django_feedback_govuk-0.1.4/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/radios.html` & `django_feedback_govuk-0.2.0/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/radios.html`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.4/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/star_rating.html` & `django_feedback_govuk-0.2.0/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/star_rating.html`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.4/django_feedback_govuk/tests/settings.py` & `django_feedback_govuk-0.2.0/django_feedback_govuk/tests/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 
 MEDIA_ROOT = os.path.join(TESTS_PATH, "media")
 
 STATIC_ROOT = os.path.join(TESTS_PATH, "static")
 
 ROOT_URLCONF = "django_feedback_govuk.tests.urls"
 
+DEFAULT_AUTO_FIELD = "django.db.models.BigAutoField"
 
 # Crispy forms
 CRISPY_ALLOWED_TEMPLATE_PACKS = ["gds"]
 CRISPY_TEMPLATE_PACK = "gds"
 
 # Django Feedback GovUK
 DJANGO_FEEDBACK_GOVUK = {
```

### Comparing `django_feedback_govuk-0.1.4/pyproject.toml` & `django_feedback_govuk-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 [tool.poetry]
 name = "django-feedback-govuk"
-version = "0.1.4"
+version = "0.2.0"
 description = "A Django app to gather and send internal Government staff feedback"
-authors = ["jafacakes2011 <cameron.lamb@digitial.trade.gov.uk>", "marcelkornblum <marcel.kornblum@digitial.trade.gov.uk>"]
+authors = [
+    "jafacakes2011 <cameron.lamb@digitial.trade.gov.uk>",
+    "marcelkornblum <marcel.kornblum@digitial.trade.gov.uk>",
+]
 license = "MIT"
 readme = "README.md"
-packages = [{include = "django_feedback_govuk"}]
+packages = [{ include = "django_feedback_govuk" }]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
-    "Topic :: Software Development :: Libraries :: Python Modules"
+    "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 Django = ">=3.2,<4.3"
 crispy-forms-gds = "^0.2.4"
 notifications-python-client = "^8.0.0"
@@ -46,27 +49,23 @@
 
 [tool.pytest.ini_options]
 minversion = "7.0"
 DJANGO_SETTINGS_MODULE = "tests.settings"
 python_files = ["tests.py", "test_*.py", "*_tests.py"]
 
 [tool.coverage.run]
-omit = [
-    "*/migrations/*",
-    "*/test/*",
-    "selenium_tests/*"
-]
+omit = ["*/migrations/*", "*/test/*", "selenium_tests/*"]
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 skip_gitignore = true
 line_length = 88
 lines_after_imports = 2
 
 [tool.djlint]
-extension="html"
-profile="django"
-format_js=false
-format_css=false
-ignore="T002,H006,H017,H023"
-preserve_blank_lines=true
+extension = "html"
+profile = "django"
+format_js = false
+format_css = false
+ignore = "T002,H006,H017,H023"
+preserve_blank_lines = true
```

