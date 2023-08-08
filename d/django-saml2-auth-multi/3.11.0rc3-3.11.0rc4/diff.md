# Comparing `tmp/django_saml2_auth_multi-3.11.0rc3.tar.gz` & `tmp/django_saml2_auth_multi-3.11.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_saml2_auth_multi-3.11.0rc3.tar", max compression
+gzip compressed data, was "django_saml2_auth_multi-3.11.0rc4.tar", max compression
```

## Comparing `django_saml2_auth_multi-3.11.0rc3.tar` & `django_saml2_auth_multi-3.11.0rc4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      552 2023-08-02 12:45:30.206550 django_saml2_auth_multi-3.11.0rc3/LICENSE
--rw-r--r--   0        0        0    43886 2023-08-07 14:00:38.376509 django_saml2_auth_multi-3.11.0rc3/README.md
--rw-r--r--   0        0        0       88 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc3/django_saml2_auth_multi/__init__.py
--rw-r--r--   0        0        0     1690 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc3/django_saml2_auth_multi/config.py
--rw-r--r--   0        0        0      940 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc3/django_saml2_auth_multi/errors.py
--rw-r--r--   0        0        0      585 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc3/django_saml2_auth_multi/exceptions.py
--rw-r--r--   0        0        0    17296 2023-08-07 14:25:35.159830 django_saml2_auth_multi-3.11.0rc3/django_saml2_auth_multi/saml.py
--rw-r--r--   0        0        0      327 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc3/django_saml2_auth_multi/templates/django_saml2_auth_multi/denied.html
--rw-r--r--   0        0        0      493 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc3/django_saml2_auth_multi/templates/django_saml2_auth_multi/error.html
--rw-r--r--   0        0        0      308 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc3/django_saml2_auth_multi/templates/django_saml2_auth_multi/signout.html
--rw-r--r--   0        0        0       43 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc3/django_saml2_auth_multi/tests/__init__.py
--rw-r--r--   0        0        0      416 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc3/django_saml2_auth_multi/tests/conftest.py
--rw-r--r--   0        0        0     1567 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc3/django_saml2_auth_multi/tests/metadata.xml
--rw-r--r--   0        0        0     3528 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc3/django_saml2_auth_multi/tests/settings.py
--rw-r--r--   0        0        0    19588 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc3/django_saml2_auth_multi/tests/test_saml.py
--rw-r--r--   0        0        0    23304 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc3/django_saml2_auth_multi/tests/test_user.py
--rw-r--r--   0        0        0     4953 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc3/django_saml2_auth_multi/tests/test_utils.py
--rw-r--r--   0        0        0      244 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc3/django_saml2_auth_multi/tests/utils.py
--rw-r--r--   0        0        0      357 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc3/django_saml2_auth_multi/urls.py
--rw-r--r--   0        0        0    16854 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc3/django_saml2_auth_multi/user.py
--rw-r--r--   0        0        0     7792 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc3/django_saml2_auth_multi/utils.py
--rw-r--r--   0        0        0    11843 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc3/django_saml2_auth_multi/views.py
--rw-r--r--   0        0        0     1505 2023-08-07 14:26:16.496497 django_saml2_auth_multi-3.11.0rc3/pyproject.toml
--rw-r--r--   0        0        0    45391 1970-01-01 00:00:00.000000 django_saml2_auth_multi-3.11.0rc3/PKG-INFO
+-rw-r--r--   0        0        0      552 2023-08-02 12:45:30.206550 django_saml2_auth_multi-3.11.0rc4/LICENSE
+-rw-r--r--   0        0        0    43886 2023-08-07 14:00:38.376509 django_saml2_auth_multi-3.11.0rc4/README.md
+-rw-r--r--   0        0        0       88 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc4/django_saml2_auth_multi/__init__.py
+-rw-r--r--   0        0        0     1690 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc4/django_saml2_auth_multi/config.py
+-rw-r--r--   0        0        0      940 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc4/django_saml2_auth_multi/errors.py
+-rw-r--r--   0        0        0      585 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc4/django_saml2_auth_multi/exceptions.py
+-rw-r--r--   0        0        0    17296 2023-08-07 14:25:35.159830 django_saml2_auth_multi-3.11.0rc4/django_saml2_auth_multi/saml.py
+-rw-r--r--   0        0        0      327 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc4/django_saml2_auth_multi/templates/django_saml2_auth_multi/denied.html
+-rw-r--r--   0        0        0      493 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc4/django_saml2_auth_multi/templates/django_saml2_auth_multi/error.html
+-rw-r--r--   0        0        0      308 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc4/django_saml2_auth_multi/templates/django_saml2_auth_multi/signout.html
+-rw-r--r--   0        0        0       43 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc4/django_saml2_auth_multi/tests/__init__.py
+-rw-r--r--   0        0        0      416 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc4/django_saml2_auth_multi/tests/conftest.py
+-rw-r--r--   0        0        0     1567 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc4/django_saml2_auth_multi/tests/metadata.xml
+-rw-r--r--   0        0        0     3528 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc4/django_saml2_auth_multi/tests/settings.py
+-rw-r--r--   0        0        0    19588 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc4/django_saml2_auth_multi/tests/test_saml.py
+-rw-r--r--   0        0        0    23304 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc4/django_saml2_auth_multi/tests/test_user.py
+-rw-r--r--   0        0        0     4953 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc4/django_saml2_auth_multi/tests/test_utils.py
+-rw-r--r--   0        0        0      244 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc4/django_saml2_auth_multi/tests/utils.py
+-rw-r--r--   0        0        0      357 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc4/django_saml2_auth_multi/urls.py
+-rw-r--r--   0        0        0    16854 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc4/django_saml2_auth_multi/user.py
+-rw-r--r--   0        0        0     7792 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc4/django_saml2_auth_multi/utils.py
+-rw-r--r--   0        0        0    11843 2023-08-07 13:55:59.743178 django_saml2_auth_multi-3.11.0rc4/django_saml2_auth_multi/views.py
+-rw-r--r--   0        0        0     1505 2023-08-08 13:10:49.689875 django_saml2_auth_multi-3.11.0rc4/pyproject.toml
+-rw-r--r--   0        0        0    45391 1970-01-01 00:00:00.000000 django_saml2_auth_multi-3.11.0rc4/PKG-INFO
```

### Comparing `django_saml2_auth_multi-3.11.0rc3/LICENSE` & `django_saml2_auth_multi-3.11.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_saml2_auth_multi-3.11.0rc3/README.md` & `django_saml2_auth_multi-3.11.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `django_saml2_auth_multi-3.11.0rc3/django_saml2_auth_multi/config.py` & `django_saml2_auth_multi-3.11.0rc4/django_saml2_auth_multi/config.py`

 * *Files identical despite different names*

### Comparing `django_saml2_auth_multi-3.11.0rc3/django_saml2_auth_multi/errors.py` & `django_saml2_auth_multi-3.11.0rc4/django_saml2_auth_multi/errors.py`

 * *Files identical despite different names*

### Comparing `django_saml2_auth_multi-3.11.0rc3/django_saml2_auth_multi/exceptions.py` & `django_saml2_auth_multi-3.11.0rc4/django_saml2_auth_multi/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_saml2_auth_multi-3.11.0rc3/django_saml2_auth_multi/saml.py` & `django_saml2_auth_multi-3.11.0rc4/django_saml2_auth_multi/saml.py`

 * *Files identical despite different names*

### Comparing `django_saml2_auth_multi-3.11.0rc3/django_saml2_auth_multi/tests/metadata.xml` & `django_saml2_auth_multi-3.11.0rc4/django_saml2_auth_multi/tests/metadata.xml`

 * *Files identical despite different names*

### Comparing `django_saml2_auth_multi-3.11.0rc3/django_saml2_auth_multi/tests/settings.py` & `django_saml2_auth_multi-3.11.0rc4/django_saml2_auth_multi/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_saml2_auth_multi-3.11.0rc3/django_saml2_auth_multi/tests/test_saml.py` & `django_saml2_auth_multi-3.11.0rc4/django_saml2_auth_multi/tests/test_saml.py`

 * *Files identical despite different names*

### Comparing `django_saml2_auth_multi-3.11.0rc3/django_saml2_auth_multi/tests/test_user.py` & `django_saml2_auth_multi-3.11.0rc4/django_saml2_auth_multi/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `django_saml2_auth_multi-3.11.0rc3/django_saml2_auth_multi/tests/test_utils.py` & `django_saml2_auth_multi-3.11.0rc4/django_saml2_auth_multi/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django_saml2_auth_multi-3.11.0rc3/django_saml2_auth_multi/user.py` & `django_saml2_auth_multi-3.11.0rc4/django_saml2_auth_multi/user.py`

 * *Files identical despite different names*

### Comparing `django_saml2_auth_multi-3.11.0rc3/django_saml2_auth_multi/utils.py` & `django_saml2_auth_multi-3.11.0rc4/django_saml2_auth_multi/utils.py`

 * *Files identical despite different names*

### Comparing `django_saml2_auth_multi-3.11.0rc3/django_saml2_auth_multi/views.py` & `django_saml2_auth_multi-3.11.0rc4/django_saml2_auth_multi/views.py`

 * *Files identical despite different names*

### Comparing `django_saml2_auth_multi-3.11.0rc3/pyproject.toml` & `django_saml2_auth_multi-3.11.0rc4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django_saml2_auth_multi"
-version = "3.11.0-rc3"
+version = "3.11.0-rc4"
 description = "Django SAML2 Authentication For Multi IdP Setups Made Easy."
 license = "Apache 2.0"
 keywords = ["django", "saml", "saml2sso", "authentication", "okta", "standard"]
 classifiers = ["Development Status :: 5 - Production/Stable", "Intended Audience :: Developers", "Topic :: Software Development :: Libraries :: Python Modules", "License :: OSI Approved :: Apache Software License", "Framework :: Django :: 2.2", "Framework :: Django :: 3.2", "Framework :: Django :: 4.0", "Framework :: Django :: 4.1", "Programming Language :: Python :: 3", "Programming Language :: Python :: 3.7", "Programming Language :: Python :: 3.8", "Programming Language :: Python :: 3.9", "Programming Language :: Python :: 3.10", "Programming Language :: Python :: 3.11"]
 homepage = "https://github.com/mfnd/django-saml2-auth-multi"
 authors = ["Fang Li <surivlee+djsaml2auth@gmail.com>", "Mostafa Moradian <mostafa@grafana.com>", "Mustafa Efendioglu <mfnd@protonmail.com>"]
 readme = "README.md"
```

### Comparing `django_saml2_auth_multi-3.11.0rc3/PKG-INFO` & `django_saml2_auth_multi-3.11.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-saml2-auth-multi
-Version: 3.11.0rc3
+Version: 3.11.0rc4
 Summary: Django SAML2 Authentication For Multi IdP Setups Made Easy.
 Home-page: https://github.com/mfnd/django-saml2-auth-multi
 License: Apache 2.0
 Keywords: django,saml,saml2sso,authentication,okta,standard
 Author: Fang Li
 Author-email: surivlee+djsaml2auth@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
```

