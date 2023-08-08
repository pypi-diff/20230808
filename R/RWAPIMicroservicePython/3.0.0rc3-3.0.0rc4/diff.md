# Comparing `tmp/RWAPIMicroservicePython-3.0.0rc3.tar.gz` & `tmp/RWAPIMicroservicePython-3.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RWAPIMicroservicePython-3.0.0rc3.tar", last modified: Fri Aug  4 16:43:17 2023, max compression
+gzip compressed data, was "RWAPIMicroservicePython-3.0.0rc4.tar", last modified: Fri Aug  4 17:04:43 2023, max compression
```

## Comparing `RWAPIMicroservicePython-3.0.0rc3.tar` & `RWAPIMicroservicePython-3.0.0rc4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-08-04 16:43:17.362320 RWAPIMicroservicePython-3.0.0rc3/
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     1100 2023-01-19 05:43:02.000000 RWAPIMicroservicePython-3.0.0rc3/LICENSE
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      365 2023-08-04 16:43:17.358986 RWAPIMicroservicePython-3.0.0rc3/PKG-INFO
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     5996 2023-08-04 09:48:11.000000 RWAPIMicroservicePython-3.0.0rc3/README.md
-drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-08-04 16:43:17.358986 RWAPIMicroservicePython-3.0.0rc3/RWAPIMicroservicePython/
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      294 2023-08-03 09:29:42.000000 RWAPIMicroservicePython-3.0.0rc3/RWAPIMicroservicePython/__init__.py
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     3111 2023-08-01 12:50:17.000000 RWAPIMicroservicePython-3.0.0rc3/RWAPIMicroservicePython/cloudwatch.py
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      409 2023-07-31 16:10:42.000000 RWAPIMicroservicePython-3.0.0rc3/RWAPIMicroservicePython/errors.py
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     7114 2023-08-04 16:40:38.000000 RWAPIMicroservicePython-3.0.0rc3/RWAPIMicroservicePython/main.py
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     2079 2023-08-03 13:19:32.000000 RWAPIMicroservicePython-3.0.0rc3/RWAPIMicroservicePython/test_utils.py
-drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-08-04 16:43:17.358986 RWAPIMicroservicePython-3.0.0rc3/RWAPIMicroservicePython.egg-info/
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      365 2023-08-04 16:43:17.000000 RWAPIMicroservicePython-3.0.0rc3/RWAPIMicroservicePython.egg-info/PKG-INFO
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      484 2023-08-04 16:43:17.000000 RWAPIMicroservicePython-3.0.0rc3/RWAPIMicroservicePython.egg-info/SOURCES.txt
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)        1 2023-08-04 16:43:17.000000 RWAPIMicroservicePython-3.0.0rc3/RWAPIMicroservicePython.egg-info/dependency_links.txt
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)        1 2023-08-02 08:02:51.000000 RWAPIMicroservicePython-3.0.0rc3/RWAPIMicroservicePython.egg-info/not-zip-safe
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      171 2023-08-04 16:43:17.000000 RWAPIMicroservicePython-3.0.0rc3/RWAPIMicroservicePython.egg-info/requires.txt
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)       24 2023-08-04 16:43:17.000000 RWAPIMicroservicePython-3.0.0rc3/RWAPIMicroservicePython.egg-info/top_level.txt
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)       38 2023-08-04 16:43:17.362320 RWAPIMicroservicePython-3.0.0rc3/setup.cfg
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      886 2023-08-04 16:42:42.000000 RWAPIMicroservicePython-3.0.0rc3/setup.py
+drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-08-04 17:04:43.051398 RWAPIMicroservicePython-3.0.0rc4/
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     1100 2023-01-19 05:43:02.000000 RWAPIMicroservicePython-3.0.0rc4/LICENSE
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      365 2023-08-04 17:04:43.051398 RWAPIMicroservicePython-3.0.0rc4/PKG-INFO
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     5996 2023-08-04 09:48:11.000000 RWAPIMicroservicePython-3.0.0rc4/README.md
+drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-08-04 17:04:43.051398 RWAPIMicroservicePython-3.0.0rc4/RWAPIMicroservicePython/
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      294 2023-08-03 09:29:42.000000 RWAPIMicroservicePython-3.0.0rc4/RWAPIMicroservicePython/__init__.py
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     3111 2023-08-01 12:50:17.000000 RWAPIMicroservicePython-3.0.0rc4/RWAPIMicroservicePython/cloudwatch.py
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      409 2023-07-31 16:10:42.000000 RWAPIMicroservicePython-3.0.0rc4/RWAPIMicroservicePython/errors.py
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     7114 2023-08-04 17:02:17.000000 RWAPIMicroservicePython-3.0.0rc4/RWAPIMicroservicePython/main.py
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     2079 2023-08-03 13:19:32.000000 RWAPIMicroservicePython-3.0.0rc4/RWAPIMicroservicePython/test_utils.py
+drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-08-04 17:04:43.051398 RWAPIMicroservicePython-3.0.0rc4/RWAPIMicroservicePython.egg-info/
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      365 2023-08-04 17:04:43.000000 RWAPIMicroservicePython-3.0.0rc4/RWAPIMicroservicePython.egg-info/PKG-INFO
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      484 2023-08-04 17:04:43.000000 RWAPIMicroservicePython-3.0.0rc4/RWAPIMicroservicePython.egg-info/SOURCES.txt
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)        1 2023-08-04 17:04:43.000000 RWAPIMicroservicePython-3.0.0rc4/RWAPIMicroservicePython.egg-info/dependency_links.txt
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)        1 2023-08-02 08:02:51.000000 RWAPIMicroservicePython-3.0.0rc4/RWAPIMicroservicePython.egg-info/not-zip-safe
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      171 2023-08-04 17:04:43.000000 RWAPIMicroservicePython-3.0.0rc4/RWAPIMicroservicePython.egg-info/requires.txt
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)       24 2023-08-04 17:04:43.000000 RWAPIMicroservicePython-3.0.0rc4/RWAPIMicroservicePython.egg-info/top_level.txt
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)       38 2023-08-04 17:04:43.051398 RWAPIMicroservicePython-3.0.0rc4/setup.cfg
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      886 2023-08-04 17:04:26.000000 RWAPIMicroservicePython-3.0.0rc4/setup.py
```

### Comparing `RWAPIMicroservicePython-3.0.0rc3/LICENSE` & `RWAPIMicroservicePython-3.0.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `RWAPIMicroservicePython-3.0.0rc3/README.md` & `RWAPIMicroservicePython-3.0.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `RWAPIMicroservicePython-3.0.0rc3/RWAPIMicroservicePython/cloudwatch.py` & `RWAPIMicroservicePython-3.0.0rc4/RWAPIMicroservicePython/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `RWAPIMicroservicePython-3.0.0rc3/RWAPIMicroservicePython/main.py` & `RWAPIMicroservicePython-3.0.0rc4/RWAPIMicroservicePython/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
         if body:
             logged_user_response = requests.post(
                 GATEWAY_URL + '/v1/request/validate',
                 headers={
                     'content-type': 'application/json',
                     'authorization': f"Bearer {MICROSERVICE_TOKEN}"
                 },
-                data=body
+                json=body
             )
 
             if logged_user_response.status_code >= 400:
                 raise ValidationError(message=logged_user_response.text, code=logged_user_response.status_code)
 
             json_response = logged_user_response.json()
```

### Comparing `RWAPIMicroservicePython-3.0.0rc3/RWAPIMicroservicePython/test_utils.py` & `RWAPIMicroservicePython-3.0.0rc4/RWAPIMicroservicePython/test_utils.py`

 * *Files identical despite different names*

### Comparing `RWAPIMicroservicePython-3.0.0rc3/setup.py` & `RWAPIMicroservicePython-3.0.0rc4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='RWAPIMicroservicePython',
-      version='3.0.0-rc.3',
+      version='3.0.0-rc.4',
       long_description='Python integration library for the RW API microservices',
       description='Python integration library for the RW API microservices',
       long_description_content_type='text',
       author='Vizzuality',
       author_email='info@vizzuality.com',
       url='https://vizzuality.com',
       license='MIT',
```

