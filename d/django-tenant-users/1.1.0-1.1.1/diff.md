# Comparing `tmp/django-tenant-users-1.1.0.tar.gz` & `tmp/django-tenant-users-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-tenant-users-1.1.0.tar", max compression
+gzip compressed data, was "django-tenant-users-1.1.1.tar", max compression
```

## Comparing `django-tenant-users-1.1.0.tar` & `django-tenant-users-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1064 2021-12-15 06:14:26.393392 django-tenant-users-1.1.0/LICENSE
--rw-r--r--   0        0        0    17372 2022-10-01 22:48:09.476925 django-tenant-users-1.1.0/README.rst
--rw-r--r--   0        0        0     2106 2022-10-01 19:19:17.470353 django-tenant-users-1.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2021-12-15 06:14:26.399164 django-tenant-users-1.1.0/tenant_users/__init__.py
--rw-r--r--   0        0        0        0 2021-12-15 06:14:26.399250 django-tenant-users-1.1.0/tenant_users/permissions/__init__.py
--rw-r--r--   0        0        0      839 2022-02-10 05:39:20.130746 django-tenant-users-1.1.0/tenant_users/permissions/backend.py
--rw-r--r--   0        0        0      861 2021-12-15 06:14:26.399412 django-tenant-users-1.1.0/tenant_users/permissions/functional.py
--rw-r--r--   0        0        0     3005 2022-10-01 18:55:54.418657 django-tenant-users-1.1.0/tenant_users/permissions/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2021-12-15 06:14:26.399563 django-tenant-users-1.1.0/tenant_users/permissions/migrations/__init__.py
--rw-r--r--   0        0        0     4091 2022-02-10 05:39:20.131535 django-tenant-users-1.1.0/tenant_users/permissions/models.py
--rw-r--r--   0        0        0       63 2022-02-10 05:39:20.131774 django-tenant-users-1.1.0/tenant_users/tenants/__init__.py
--rw-r--r--   0        0        0      246 2022-02-10 05:39:20.132041 django-tenant-users-1.1.0/tenant_users/tenants/apps.py
--rw-r--r--   0        0        0        0 2021-12-15 06:14:26.399927 django-tenant-users-1.1.0/tenant_users/tenants/migrations/__init__.py
--rw-r--r--   0        0        0    13491 2022-10-01 18:55:54.420524 django-tenant-users-1.1.0/tenant_users/tenants/models.py
--rw-r--r--   0        0        0     2478 2022-02-10 05:39:20.132749 django-tenant-users-1.1.0/tenant_users/tenants/tasks.py
--rw-r--r--   0        0        0     1532 2022-02-10 05:39:20.133130 django-tenant-users-1.1.0/tenant_users/tenants/utils.py
--rw-r--r--   0        0        0    18615 1970-01-01 00:00:00.000000 django-tenant-users-1.1.0/setup.py
--rw-r--r--   0        0        0    18919 1970-01-01 00:00:00.000000 django-tenant-users-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2021-12-17 15:19:01.356625 django-tenant-users-1.1.1/LICENSE
+-rw-r--r--   0        0        0    17372 2022-11-26 14:54:47.441467 django-tenant-users-1.1.1/README.rst
+-rw-r--r--   0        0        0     2138 2022-11-26 14:55:46.872558 django-tenant-users-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-12-17 15:19:01.362917 django-tenant-users-1.1.1/tenant_users/__init__.py
+-rw-r--r--   0        0        0        0 2021-12-17 15:19:01.363033 django-tenant-users-1.1.1/tenant_users/permissions/__init__.py
+-rw-r--r--   0        0        0      839 2022-11-26 14:54:39.061792 django-tenant-users-1.1.1/tenant_users/permissions/backend.py
+-rw-r--r--   0        0        0      861 2021-12-17 15:19:01.363262 django-tenant-users-1.1.1/tenant_users/permissions/functional.py
+-rw-r--r--   0        0        0     3005 2022-11-26 14:54:39.061627 django-tenant-users-1.1.1/tenant_users/permissions/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2021-12-17 15:19:01.363478 django-tenant-users-1.1.1/tenant_users/permissions/migrations/__init__.py
+-rw-r--r--   0        0        0     4091 2022-11-26 14:54:39.061397 django-tenant-users-1.1.1/tenant_users/permissions/models.py
+-rw-r--r--   0        0        0      111 2022-11-26 14:54:47.457049 django-tenant-users-1.1.1/tenant_users/tenants/__init__.py
+-rw-r--r--   0        0        0      246 2022-01-22 21:05:12.080302 django-tenant-users-1.1.1/tenant_users/tenants/apps.py
+-rw-r--r--   0        0        0        0 2021-12-17 15:19:01.364097 django-tenant-users-1.1.1/tenant_users/tenants/migrations/__init__.py
+-rw-r--r--   0        0        0    13491 2022-09-11 16:18:33.579999 django-tenant-users-1.1.1/tenant_users/tenants/models.py
+-rw-r--r--   0        0        0     2478 2021-12-17 15:19:01.364390 django-tenant-users-1.1.1/tenant_users/tenants/tasks.py
+-rw-r--r--   0        0        0     1532 2021-12-17 15:19:01.364503 django-tenant-users-1.1.1/tenant_users/tenants/utils.py
+-rw-r--r--   0        0        0    18615 1970-01-01 00:00:00.000000 django-tenant-users-1.1.1/setup.py
+-rw-r--r--   0        0        0    18958 1970-01-01 00:00:00.000000 django-tenant-users-1.1.1/PKG-INFO
```

### Comparing `django-tenant-users-1.1.0/LICENSE` & `django-tenant-users-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-tenant-users-1.1.0/README.rst` & `django-tenant-users-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-tenant-users-1.1.0/pyproject.toml` & `django-tenant-users-1.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 skip-string-normalization = true
 include = '\.pyi?$'
 
 
 [tool.poetry]
 name = "django-tenant-users"
 description = "A Django app to extend django-tenants to incorporate global multi-tenant users"
-version = "1.1.0"
+version = "1.1.1"
 license = "MIT License"
 
 packages = [
   { include = 'tenant_users' },
 ]
 
 authors = [
@@ -38,14 +38,15 @@
 
 classifiers = [
   "Environment :: Web Environment",
   "Framework :: Django",
   "Framework :: Django :: 2.2",
   "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.0",
+  "Framework :: Django :: 4.1",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
```

### Comparing `django-tenant-users-1.1.0/tenant_users/permissions/backend.py` & `django-tenant-users-1.1.1/tenant_users/permissions/backend.py`

 * *Files identical despite different names*

### Comparing `django-tenant-users-1.1.0/tenant_users/permissions/functional.py` & `django-tenant-users-1.1.1/tenant_users/permissions/functional.py`

 * *Files identical despite different names*

### Comparing `django-tenant-users-1.1.0/tenant_users/permissions/migrations/0001_initial.py` & `django-tenant-users-1.1.1/tenant_users/permissions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-tenant-users-1.1.0/tenant_users/permissions/models.py` & `django-tenant-users-1.1.1/tenant_users/permissions/models.py`

 * *Files identical despite different names*

### Comparing `django-tenant-users-1.1.0/tenant_users/tenants/models.py` & `django-tenant-users-1.1.1/tenant_users/tenants/models.py`

 * *Files identical despite different names*

### Comparing `django-tenant-users-1.1.0/tenant_users/tenants/tasks.py` & `django-tenant-users-1.1.1/tenant_users/tenants/tasks.py`

 * *Files identical despite different names*

### Comparing `django-tenant-users-1.1.0/tenant_users/tenants/utils.py` & `django-tenant-users-1.1.1/tenant_users/tenants/utils.py`

 * *Files identical despite different names*

### Comparing `django-tenant-users-1.1.0/setup.py` & `django-tenant-users-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 {'': ['*']}
 
 install_requires = \
 ['Django>=2.2,<4.2,!=3.0.*,!=3.1.*', 'django-tenants>=3.4.5,<4.0.0']
 
 setup_kwargs = {
     'name': 'django-tenant-users',
-    'version': '1.1.0',
+    'version': '1.1.1',
     'description': 'A Django app to extend django-tenants to incorporate global multi-tenant users',
     'long_description': '===================\ndjango-tenant-users\n===================\n.. image:: https://github.com/Corvia/django-tenant-users/actions/workflows/test.yml/badge.svg\n    :alt: Build Status\n    :target: https://github.com/Corvia/django-tenant-users/actions/workflows/test.yml\n\n.. image:: https://codecov.io/gh/Corvia/django-tenant-users/branch/master/graph/badge.svg?token=PRS5HhOYPl\n    :alt: codecov\n    :target: https://codecov.io/gh/Corvia/django-tenant-users\n\n.. image:: https://img.shields.io/pypi/v/django-tenant-users.svg?maxAge=180\n    :alt: PyPI Package\n    :target: https://pypi.org/project/django-tenant-users/\n\n.. image:: https://img.shields.io/pypi/pyversions/django-tenant-users.svg?maxAge=180\n    :alt: Python Versions\n    :target: https://pypi.org/project/django-tenant-users/\n\n.. image:: https://img.shields.io/pypi/djversions/django-tenant-users.svg?maxAge=180\n    :alt: Django Versions\n    :target: https://pypi.org/project/django-tenant-users/\n\n.. image:: https://img.shields.io/pypi/dm/django-tenant-users.svg?maxAge=180\n    :alt: PyPI Monthly Downloads\n    :target: https://pypi.org/project/django-tenant-users/\n\nTable of Contents\n=================\n\n- `Overview <overview_>`_\n- `Installation <installation_>`_\n- `Test Project <test-project_>`_\n- `Basic Settings <basic-settings_>`_\n- `Modifying the Tenant Model <modifying-the-tenant-model_>`_\n- `Creating the User Model <creating-the-user-model_>`_\n- `Setting up the Authentication Backend <setting-up-the-authentication-backend_>`_\n- `Setting up Cross Domain Cookies <setting-up-cross-domain-cookies_>`_\n- `Migrating and Creating the Public Tenant <migrating-and-creating-the-public-tenant_>`_\n- `Provisioning a Tenant <provisioning-a-tenant_>`_\n- `Creating a User <creating-a-user_>`_\n\nThis application expands the django users and permissions frameworks to work alongside\ndjango-tenant-schemas or django-tenants to allow global users with permissions on a per-tenant basis.\nThis allows a single user to belong to multiple tenants and permissions in each tenant, including allowing permissions in the public tenant. This app also adds support for querying all tenants a user belongs to.\n\n.. _overview:\n\nOverview\n========\n\nTo simplify the use of Django\'s models and ORM layer, we need to isolate each tenant so we don\'t have to filter objects (queries) by tenant. Since we are using PostgreSQL we handle this by using a separate schema for each tenant. We use django-tenant-schemas or django-tenants to handle all of this. Using separate schemas per tenant provides a small layer of security, permissions isolation, and some performance benefits. On the flip side, we\'ve now segregated the database completely on a per-tenant basis, and have no default support for global authentication. For instance, if one user belongs to multiple tenants they should not need to have multiple accounts and should not have to sign in multiple times (i.e. be forced to sign for each tenant). They also should be able to see all the tenants they belong to. By default, this is not possible with django-tenant-schemas or django-tenants so we have created a solution to this problem (described below).\n\n\nThe django middleware (django-tenant-schemas or django-tenants) handles the schema setting automatically on a per-request basis. It does this by looking at the subdomain that the request comes in on and maps that to a \'tenant\'. No subdomain, or the \'www\' subdomain map to a default \'public\' tenant. In order for this mapping to work to a tenant, we have to create the tenant and the tenant\'s schema in the database.\n\nWe leverage the tenant schemas middleware to handle most of this transparently. However, to get global authentication (global user accounts) and per-tenant authorization (permissions) working we rely on some of the nuances of schemas.\n\nA schema is quite similar to a search path on a file system "path1;path2;path3" that gets searched in order. If no model exists in the first schema then the next one is searched. If the model exists but is empty, it does not continue searching (a model was found). By default, the \'public\' schema is always transparently appended to the end of the schema path whenever set_schema is called.\n\nGlobal Authentication Solution\n------------------------------\n\nWith this in mind, it\'s easy to see that we can create a users table at the global level in the public schema but NOT in the tenants schemas and the users table will still be searched and found, regardless of which tenant is selected. However, the problem is that we need to create our permissions on a per tenant basis, not at a global level. In fact, since the public schema also represents the website, the permissions for a user at the global level should only reflect the permissions for the website (i.e. can I post on the blog?). It\'s really an entirely different permission set at the public schema level that we need to support.\n\nThe difficulty comes in at the Django level. Luckily Django supports using a custom user model. However, internally, the way Django uses the model tightly couples aspects of the authentication (user/pass and profile) and authorization (permissions) together, despite each one of those aspects inheriting from a separate mixin (parent tree: see PermissionsMixin and AbstractUserBase classes). As an artifact of the coupling, the authentication/permissions backend, as well as other components, make the assumption that it is one one model in the database. The built in function get_user_model() returns the model that is configured as the user model (whether its the stock django user model or a custom user model). We handle this in a relatively simplistic way. First, we decouple the two components (user profile and user permissions) into UserProfile and UserTenantPermissions. We install the UserProfile only at the SHARED_APPs (public schema) level. We install the Permissions model at ALL levels -- SHARED_APPs and TENANT_APPs (both public schema, and per tenant schema). Then we \'facade\' the two together (see AbstractBaseUserFacade and TenantPermissionsMixinFacade classes) to make each model look and behave like it encapsulates all of the functionality of a single unified user model. The part that makes it a little more tricky (and perhaps more clever) is that the two models that are linked at any point in time for a query is defined by the currently set schema.\n\nLet\'s look at an example. When accessing the website (via a request), the public schema is set (because its the public tenant), then the public Permissions model located in the public schema is what gets looked up by permissions queries, as well as the public user model (which is also located in the public schema). When a request comes in for a tenant, "EvilCorp" the EvilCorp schema is selected automatically via the middleware. However, remember that the schema set is really a search path that also contains the public schema appended to the end (see above). Thus, when a query comes in looking up permissions, it finds a permissions model INSIDE the EvilCorp tenant, and uses those permissions (rather than the model in the public schema), but when it looks up the UserProfile, nothing exists in the EvilCorp tenant schema so it falls back and searches the public schema and finds the UserProfile there. So essentially we end up \'glueing\' these components together at run time for any given query using the schema search path.\n\nNext, we have to create a custom authentication backend to handle the new user/permission model segregation. Luckily this is fairly easy and almost requires no changes since both our models provide facade interfaces to each other! We don\'t have to change any of the logic in the auth backend (in fact the permission caching still even works at a per-tenant level automagially!). The only change we make is slight, and that is the way the default backend uses get_user_model() to look up meta data about the user model. We just override methods using this functionality to change this behavior and force it to use the tenant permissions model for permissions meta work, instead of the user model thats returned from get_user_model().\n\nTenants are stored at the public schema level and are also what defines each tenant. Tenants and users are linked at the public level as well, so we can query a user and see what tenants it belongs to, or query a tenant and see what users are associated. However, the permissions of a user are defined inside the tenant\'s schema itself, so to view that data, we have to switch the schema over (normally this happens automatically, but in the case of wanting to view a users permissions on a public profile page, we would have to force set the schema (connection.set_schema(\'EvilCorp\'), as defined in the Tenant model for that tenant). We also have to remember to set it back. Most use cases will not ever have to touch the schema setting directly.\n\nUser and Tenant \'Deletion\'\n---------------------------\n\nWith this solution, we also implement an alternative to avoid actually deleting users or tenants, so we need a way to make them disappear into the ether (from the users perspective) without conflict (i.e. don\'t allow a deleted tenant to permanently monopolize a tenant URL subdomain, and don\'t allow a users email to never be used again for signup). To handle the user delete, we just set the user is_active/staff/superuser to false and delete all links to any tenants it owns, as well as all instances of permissions it has in any tenant it was associated with. A user can "delete" a tenant manually, or in the case that a deleted user owns a tenant, we "delete" the tenant. When we "delete" a tenant, we disassociate any users with any permissions, and then change the owner of the tenant\'s schema to the public schema\'s owner (the same owner that was configured when create_public_tenant command was run). When we do this, we also rename the tenant\'s URL to be ownerid-timestamp-originalurl. Not only does this encapsulate some of the history of the tenant\'s ownership, but it also frees up the URL namespace. Also, we never have to worry about schemas in the database conflicting because when we generate a tenant\'s schema, we append the timestamp (in seconds since the epoch) to the name. Thus, every schema ends up unique when made, eliminating any schema level conflicts.\n\nTo do a full delete on Users/Tenants the delete methods can be overridden, or force_drop=True can be passed in to delete.\n\n.. _installation:\n\nInstallation\n============\nAssuming you already have django-tenant-schemas or django-tenants installed and configured, the first step is to install ``django-tenant-users``.\n\n.. code-block:: bash\n\n    pip install django-tenant-users\n\n.. _test-project:\n\nTest Project\n============\n\nAll of the following settings/configuration can be seen in `django_test_app <https://github.com/Corvia/django-tenant-users/tree/master/django_test_app>`_.\n\n.. _basic-settings:\n\nBasic Settings\n==============\n\nYou\'ll have to make the following additions to the ``SHARED_APPS`` and ``TENANT_APPS` in your ``settings.py`` file.\n\n.. code-block:: python\n\n    SHARED_APPS=[\n        # ...\n        \'django.contrib.auth\', # Defined in both shared apps and tenant apps\n        \'django.contrib.contenttypes\', # Defined in both shared apps and tenant apps\n        \'tenant_users.permissions\', # Defined in both shared apps and tenant apps\n        \'tenant_users.tenants\', # defined only in shared apps\n        \'companies\', # Custom defined app that contains the TenantModel. Must NOT exist in TENANT_APPS\n        \'users\', # Custom app that contains the new User Model (see below). Must NOT exist in TENANT_APPS\n        # ...\n    ]\n\n    TENANT_APPS=[\n        # ...\n        \'django.contrib.auth\', # Defined in both shared apps and tenant apps\n        \'django.contrib.contenttypes\', # Defined in both shared apps and tenant apps\n        \'tenant_users.permissions\', # Defined in both shared apps and tenant apps\n        # ...\n    ]\n\nYou will have to set the ``TENANT_USERS_DOMAIN`` setting to the domain hosting the tenants. This is utilized in provision_tenant to fill out the domain_url to match incoming requests.\n\n.. code-block:: python\n\n    TENANT_USERS_DOMAIN = "example.com"\n\n.. _modifying-the-tenant-model:\n\nModifying the Tenant Model\n==========================\n\nNext we need to modify the TenantModel, which you should already have configured in settings.py. We need to change the inerhitance chain to inherit from ``TenantBase`` (previously it was ``TenantMixin``). Below is an example TenantModel located in the \'customers\' app that we installed above in the basic configuration section. Note. this \'customers\' should ONLY be installed in the SHARED_APPs list.\n\n.. code-block:: python\n\n    # customers/model.py\n\n    from tenant_users.tenants.models import TenantBase\n\n    class Client(TenantBase):\n        name = models.CharField(max_length=100)\n        description = models.TextField(max_length=200)\n\nThe settings.py file entry should look like:\n\n.. code-block:: python\n\n    settings.py\n\n    TENANT_MODEL = \'customers.Client\'\n\n.. _creating-the-user-model:\n\nCreating the User Model\n=======================\n\nNow we need to do the same thing to the User model. If you are not using a custom user model, then one needs to be built and configured in settings.py. The custom user model needs to inherit from the tenant_users UserProfile model. Additional fields can then be added to your custom user model, if desired. In this example, we will add the TenantUser model to the ``users`` application that we installed above in the basic configuration.\n\n.. code-block:: python\n\n    # users/models.py\n\n    from tenant_users.tenants.models import UserProfile\n\n    class TenantUser(UserProfile):\n        name = models.CharField(\n            _("Name"),\n            max_length = 100,\n            blank = True,\n        )\n\nThe settings.py file entry would look like (see Django documentation for more details):\n\n.. code-block:: python\n\n    settings.py\n\n    AUTH_USER_MODEL = \'users.TenantUser\'\n\n.. _setting-up-the-authentication-backend:\n\nSetting up the Authentication Backend\n=====================================\n\nAt this point we now have all of the user, permissions, and tenant models configured. Because Django does not completely isolate authorization (permissions) from authentication (user/pass) we have to use a minimally modified authentication backend. Switch the authentication backend as follows:\n\n\n.. code-block:: python\n\n    AUTHENTICATION_BACKENDS = (\n        \'tenant_users.permissions.backend.UserBackend\',\n    )\n\n\n\n**Notes**:\nIf you want to use django admin you will have to utilize admin multisite. Warning: if you set this up incorrectly you could expose access to models that users are not permitted to access (due to the schema search path being present, and falling through. See notes in code).\nYou must reset migrations after updating the user model.\n\n\n\n.. _setting-up-cross-domain-cookies:\n\nSetting up cross domain cookies\n===============================\n\nSetting up cross domain cookies will allow a single sign on to access any of the tenants with the same session cookies.\n\n.. code-block:: python\n\n    SESSION_COOKIE_DOMAIN = \'.mydomain.com\'\n\nWarning: read the django documentation to understand the impacts of using ``SESSION_COOKIE_DOMAIN``\n\n.. _migrating-and-creating-the-public-tenant:\n\nMigrating and Creating the Public Tenant\n========================================\n\nDjango tenant schemas requires ``migrate_schemas`` to be called and a public tenant to be created. Here is an example of creating the public tenant along with a default \'system\' tenant owner.\n\n\n.. code-block:: python\n\n    # Create public tenant user.\n    from tenant_users.tenants.utils import create_public_tenant\n    create_public_tenant(domain_url="my.evilcorp.domain", owner_email="admin@evilcorp.com")\n\n.. _provisioning-a-tenant:\n\nProvisioning a Tenant\n======================\n\nHere is an example to provision a tenant with the url "evilcorp.example.com". The Domain Name is taken from the ``TENANT_USERS_DOMAIN`` Variable in the Django settings file.\n\nThe user with the specified email will not be created by the ``provision_tenant`` command and has to exist beforhand. The user will be the owner of the tenant. In this example the Adminuser from the section above is used. To create another user see `Creating a User Section <creating-a-user_>`_\n\n.. code-block:: python\n\n    from tenant_users.tenants.tasks import provision_tenant\n\n    fqdn = provision_tenant(tenant_name="EvilCorp", tenant_slug="evilcorp", user_email="admin@evilcorp.com").\n\n**Note:** Since provisioning a tenant also has to create the entire schema -- depending on the models installed, it can take a while. It is recommended that this does not occur in the request/response cycle. A good asynchronous option is to use a task runner like Celery (along with tenant-schemas-celery) to handle this.\n\n\n.. _creating-a-user:\n\nCreating a User\n===============\n\nAll users apart from the first public tenant user (see `Migrating and Creating the Public Tenant <migrating-and-creating-the-public-tenant_>`_ for creating the first public tenant user) should be created through the object manager.\n\n.. code-block:: python\n\n    user = TenantUser.objects.create_user(email="user@evilcorp.com", password=\'password\', is_active=True)\n\nCurrently all users rely on an email for the username.\n',
     'author': 'Corvia Technologies, LLC',
     'author_email': 'support@corvia.tech',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://www.github.com/Corvia/django-tenant-users',
```

### Comparing `django-tenant-users-1.1.0/PKG-INFO` & `django-tenant-users-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: django-tenant-users
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Django app to extend django-tenants to incorporate global multi-tenant users
 Home-page: https://www.github.com/Corvia/django-tenant-users
 License: MIT
 Keywords: django,django-tenant-users
 Author: Corvia Technologies, LLC
 Author-email: support@corvia.tech
 Requires-Python: >=3.7,<4.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

