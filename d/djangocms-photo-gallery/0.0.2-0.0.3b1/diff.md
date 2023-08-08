# Comparing `tmp/djangocms_photo_gallery-0.0.2.tar.gz` & `tmp/djangocms_photo_gallery-0.0.3b1.tar.gz`

## Comparing `djangocms_photo_gallery-0.0.2.tar` & `djangocms_photo_gallery-0.0.3b1.tar`

### file list

```diff
@@ -1,36 +1,24 @@
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/.idea/djangocms-photo-gallery.iml
--rw-r--r--   0        0        0     4409 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/.idea/misc.xml
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/.idea/modules.xml
--rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/.idea/workspace.xml
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/README.md
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/__about__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/__init__.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/admin.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/apps.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/cms_apps.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/cms_plugins.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/models.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/tests.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/urls.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/views.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/.idea/.gitignore
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/.idea/djangocms-photo-gallery.iml
--rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/.idea/misc.xml
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/.idea/modules.xml
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/.idea/workspace.xml
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4522 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/migrations/__init__.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/templates/djangocms_photo_gallery/album_list.html
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/templates/djangocms_photo_gallery/include/album.html
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/templates/djangocms_photo_gallery/plugins/album.html
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/README.md
--rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.3b1/src/djangocms_photo_gallery/README.md
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.3b1/src/djangocms_photo_gallery/__about__.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.3b1/src/djangocms_photo_gallery/__init__.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.3b1/src/djangocms_photo_gallery/admin.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.3b1/src/djangocms_photo_gallery/apps.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.3b1/src/djangocms_photo_gallery/cms_apps.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.3b1/src/djangocms_photo_gallery/cms_plugins.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.3b1/src/djangocms_photo_gallery/models.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.3b1/src/djangocms_photo_gallery/tests.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.3b1/src/djangocms_photo_gallery/urls.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.3b1/src/djangocms_photo_gallery/views.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.3b1/src/djangocms_photo_gallery/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.3b1/src/djangocms_photo_gallery/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4522 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.3b1/src/djangocms_photo_gallery/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.3b1/src/djangocms_photo_gallery/migrations/__init__.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.3b1/src/djangocms_photo_gallery/templates/djangocms_photo_gallery/album_list.html
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.3b1/src/djangocms_photo_gallery/templates/djangocms_photo_gallery/include/album.html
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.3b1/src/djangocms_photo_gallery/templates/djangocms_photo_gallery/plugins/album.html
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.3b1/tests/__init__.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.3b1/.gitignore
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.3b1/LICENSE.txt
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.3b1/README.md
+-rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.3b1/pyproject.toml
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 djangocms_photo_gallery-0.0.3b1/PKG-INFO
```

### Comparing `djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/README.md` & `djangocms_photo_gallery-0.0.3b1/src/djangocms_photo_gallery/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 
 In the settings of the project (e. g. `settings.py`), you need to add entries in ` 
 
 ```python
 INSTALLED_APPS: list = [
     # …
     'easy_thumbnails',
+    'django-parler',
+    'djangocms_text_ckeditor',
     'djangocms_photo_gallery',
 ]
 
 THUMBNAIL_ALIASES = {
     '': {
         'gallery': {
                     'size': (300, 200),
```

### Comparing `djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/models.py` & `djangocms_photo_gallery-0.0.3b1/src/djangocms_photo_gallery/models.py`

 * *Files identical despite different names*

### Comparing `djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/locale/de/LC_MESSAGES/django.mo` & `djangocms_photo_gallery-0.0.3b1/src/djangocms_photo_gallery/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/locale/de/LC_MESSAGES/django.po` & `djangocms_photo_gallery-0.0.3b1/src/djangocms_photo_gallery/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/migrations/0001_initial.py` & `djangocms_photo_gallery-0.0.3b1/src/djangocms_photo_gallery/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms_photo_gallery-0.0.2/src/djangocms_photo_gallery/templates/djangocms_photo_gallery/include/album.html` & `djangocms_photo_gallery-0.0.3b1/src/djangocms_photo_gallery/templates/djangocms_photo_gallery/include/album.html`

 * *Files identical despite different names*

### Comparing `djangocms_photo_gallery-0.0.2/LICENSE.txt` & `djangocms_photo_gallery-0.0.3b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djangocms_photo_gallery-0.0.2/README.md` & `djangocms_photo_gallery-0.0.3b1/README.md`

 * *Files identical despite different names*

### Comparing `djangocms_photo_gallery-0.0.2/pyproject.toml` & `djangocms_photo_gallery-0.0.3b1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -22,14 +22,16 @@
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "Django",
   "django-cms",
   "easy-thumbnails",
+  "django-parler",
+  "djangocms_text_ckeditor",
 ]
 
 [project.urls]
 Documentation = "https://github.com/MacLake/djangocms-photo-gallery#readme"
 Issues = "https://github.com/MacLake/djangocms-photo-gallery/issues"
 Source = "https://github.com/MacLake/djangocms-photo-gallery"
```

### Comparing `djangocms_photo_gallery-0.0.2/PKG-INFO` & `djangocms_photo_gallery-0.0.3b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-photo-gallery
-Version: 0.0.2
+Version: 0.0.3b1
 Project-URL: Documentation, https://github.com/MacLake/djangocms-photo-gallery#readme
 Project-URL: Issues, https://github.com/MacLake/djangocms-photo-gallery/issues
 Project-URL: Source, https://github.com/MacLake/djangocms-photo-gallery
 Author-email: Jens-Erik Weber <Jens-Erik.Weber@passiv.de>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -13,14 +13,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9
 Requires-Dist: django
 Requires-Dist: django-cms
+Requires-Dist: django-parler
+Requires-Dist: djangocms-text-ckeditor
 Requires-Dist: easy-thumbnails
 Description-Content-Type: text/markdown
 
 # djangocms-photo-gallery
 
 [![PyPI - Version](https://img.shields.io/pypi/v/djangocms-photo-gallery.svg)](https://pypi.org/project/djangocms-photo-gallery)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/djangocms-photo-gallery.svg)](https://pypi.org/project/djangocms-photo-gallery)
```

