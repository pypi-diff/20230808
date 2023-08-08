# Comparing `tmp/celery_sqlalchemy_kit-0.1.2.tar.gz` & `tmp/celery_sqlalchemy_kit-0.1.3.tar.gz`

## Comparing `celery_sqlalchemy_kit-0.1.2.tar` & `celery_sqlalchemy_kit-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.2/docker-compose.yml
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.2/celery_sqlalchemy_kit/__init__.py
--rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.2/celery_sqlalchemy_kit/base_task.py
--rw-r--r--   0        0        0     9938 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.2/celery_sqlalchemy_kit/scheduler.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.2/celery_sqlalchemy_kit/db/__init__.py
--rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.2/celery_sqlalchemy_kit/db/crud.py
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.2/celery_sqlalchemy_kit/db/model.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.2/celery_sqlalchemy_kit/db/session.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.2/example/.env.example
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.2/example/celery_app.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.2/example/custom_tasks.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.2/tests/celery_test_instance.py
--rw-r--r--   0        0        0     5066 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.2/tests/test_celery_scheduler.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.2/tests/build/dockerfile
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.2/tests/build/requirements.dev.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.2/tests/scripts/__init__.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.2/tests/scripts/prestart.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.2/tests/scripts/setup_routines_table.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.2/tests/scripts/start_celery.sh
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.2/tests/scripts/start_celery_beat.sh
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.2/tests/scripts/start_tests.sh
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.2/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.2/LICENSE
--rw-r--r--   0        0        0     7946 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.2/README.md
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     8923 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.3/docker-compose.yml
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.3/celery_sqlalchemy_kit/__init__.py
+-rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.3/celery_sqlalchemy_kit/base_task.py
+-rw-r--r--   0        0        0     9938 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.3/celery_sqlalchemy_kit/scheduler.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.3/celery_sqlalchemy_kit/db/__init__.py
+-rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.3/celery_sqlalchemy_kit/db/crud.py
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.3/celery_sqlalchemy_kit/db/model.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.3/celery_sqlalchemy_kit/db/session.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.3/example/.env.example
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.3/example/celery_app.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.3/example/custom_tasks.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.3/tests/celery_test_instance.py
+-rw-r--r--   0        0        0     5066 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.3/tests/test_celery_scheduler.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.3/tests/build/dockerfile
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.3/tests/build/requirements.dev.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.3/tests/scripts/__init__.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.3/tests/scripts/prestart.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.3/tests/scripts/setup_routines_table.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.3/tests/scripts/start_celery.sh
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.3/tests/scripts/start_celery_beat.sh
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.3/tests/scripts/start_tests.sh
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.3/LICENSE
+-rw-r--r--   0        0        0     7946 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.3/README.md
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     8923 2020-02-02 00:00:00.000000 celery_sqlalchemy_kit-0.1.3/PKG-INFO
```

### Comparing `celery_sqlalchemy_kit-0.1.2/docker-compose.yml` & `celery_sqlalchemy_kit-0.1.3/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `celery_sqlalchemy_kit-0.1.2/celery_sqlalchemy_kit/base_task.py` & `celery_sqlalchemy_kit-0.1.3/celery_sqlalchemy_kit/base_task.py`

 * *Files identical despite different names*

### Comparing `celery_sqlalchemy_kit-0.1.2/celery_sqlalchemy_kit/scheduler.py` & `celery_sqlalchemy_kit-0.1.3/celery_sqlalchemy_kit/scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,15 @@
         """
         logger.debug("get schedule")
         schedule_entries = {}
         try:
             self._db_routines = crud.get_multiple(db=self._session, active=True)
             schedule_entries = self.db_routines_to_schedule_entries(db_routines=self._db_routines)
         except SQLAlchemyError as e:
-            if self.db_tries > 0:
+            if self.db_tries > 1:
                 raise e
             self._task_db.renew()
             self._session = self._task_db.session
             self.db_tries = 1
             return self.get_schedule()
         except Exception as e:
             logger.error(e, exc_info=True)
```

### Comparing `celery_sqlalchemy_kit-0.1.2/celery_sqlalchemy_kit/db/crud.py` & `celery_sqlalchemy_kit-0.1.3/celery_sqlalchemy_kit/db/crud.py`

 * *Files identical despite different names*

### Comparing `celery_sqlalchemy_kit-0.1.2/celery_sqlalchemy_kit/db/model.py` & `celery_sqlalchemy_kit-0.1.3/celery_sqlalchemy_kit/db/model.py`

 * *Files identical despite different names*

### Comparing `celery_sqlalchemy_kit-0.1.2/example/celery_app.py` & `celery_sqlalchemy_kit-0.1.3/example/celery_app.py`

 * *Files identical despite different names*

### Comparing `celery_sqlalchemy_kit-0.1.2/example/custom_tasks.py` & `celery_sqlalchemy_kit-0.1.3/example/custom_tasks.py`

 * *Files identical despite different names*

### Comparing `celery_sqlalchemy_kit-0.1.2/tests/celery_test_instance.py` & `celery_sqlalchemy_kit-0.1.3/tests/celery_test_instance.py`

 * *Files identical despite different names*

### Comparing `celery_sqlalchemy_kit-0.1.2/tests/test_celery_scheduler.py` & `celery_sqlalchemy_kit-0.1.3/tests/test_celery_scheduler.py`

 * *Files identical despite different names*

### Comparing `celery_sqlalchemy_kit-0.1.2/tests/build/dockerfile` & `celery_sqlalchemy_kit-0.1.3/tests/build/dockerfile`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 FROM python:3.10-slim
 
 ENV PYTHONDONTWRITEBYTECODE 1
 ENV PYTHONBUFFERED 1
 # install system dependencies
 RUN apt-get update \
-  && apt-get -y install netcat gcc libpq-dev build-essential curl \
+  && apt-get -y install netcat-openbsd gcc libpq-dev build-essential curl \
   && apt-get clean
 
 # install python dependencies
 RUN mkdir -p /celery_sqlalchemy_kit
 WORKDIR /
 COPY /tests/build/requirements.dev.txt /
 RUN pip install --upgrade pip
```

### Comparing `celery_sqlalchemy_kit-0.1.2/tests/scripts/prestart.py` & `celery_sqlalchemy_kit-0.1.3/tests/scripts/prestart.py`

 * *Files identical despite different names*

### Comparing `celery_sqlalchemy_kit-0.1.2/tests/scripts/setup_routines_table.py` & `celery_sqlalchemy_kit-0.1.3/tests/scripts/setup_routines_table.py`

 * *Files identical despite different names*

### Comparing `celery_sqlalchemy_kit-0.1.2/LICENSE` & `celery_sqlalchemy_kit-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `celery_sqlalchemy_kit-0.1.2/README.md` & `celery_sqlalchemy_kit-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `celery_sqlalchemy_kit-0.1.2/pyproject.toml` & `celery_sqlalchemy_kit-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "celery-sqlalchemy-kit"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Amelie Luecke", email="amelie.luecke@cap-on.de" }, { name="Philipp Ratz", email="philipp.ratz@cap-on.de" }
 ]
 description = "Schedule tasks in an SQL Database and define Async Celery Tasks."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `celery_sqlalchemy_kit-0.1.2/PKG-INFO` & `celery_sqlalchemy_kit-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celery-sqlalchemy-kit
-Version: 0.1.2
+Version: 0.1.3
 Summary: Schedule tasks in an SQL Database and define Async Celery Tasks.
 Project-URL: Homepage, https://github.com/cap-on/celery-sqlalchemy-kit
 Project-URL: Bug Tracker, https://github.com/cap-on/celery-sqlalchemy-kit/issues
 Author-email: Amelie Luecke <amelie.luecke@cap-on.de>, Philipp Ratz <philipp.ratz@cap-on.de>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

