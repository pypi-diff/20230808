# Comparing `tmp/aiogramarch-1.1.1.tar.gz` & `tmp/aiogramarch-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogramarch-1.1.1.tar", max compression
+gzip compressed data, was "aiogramarch-1.1.2.tar", max compression
```

## Comparing `aiogramarch-1.1.1.tar` & `aiogramarch-1.1.2.tar`

### file list

```diff
@@ -1,31 +1,40 @@
--rw-r--r--   0        0        0      115 2023-08-07 05:37:42.215703 aiogramarch-1.1.1/aiogramarch/__init__.py
--rw-r--r--   0        0        0        0 2023-08-05 22:13:31.659111 aiogramarch-1.1.1/aiogramarch/arch/__init__.py
--rw-r--r--   0        0        0      227 2023-08-08 08:01:12.391123 aiogramarch-1.1.1/aiogramarch/arch/bot.py
--rw-r--r--   0        0        0      348 2023-08-07 10:31:28.484918 aiogramarch-1.1.1/aiogramarch/arch/database.py
--rw-r--r--   0        0        0      429 2023-08-08 06:55:56.208818 aiogramarch-1.1.1/aiogramarch/arch/settings.py
--rw-r--r--   0        0        0     1076 2023-08-08 08:03:41.900952 aiogramarch-1.1.1/aiogramarch/arch/startapp.py
--rw-r--r--   0        0        0        0 2023-08-07 14:49:53.686426 aiogramarch-1.1.1/aiogramarch/cli/__init__.py
--rw-r--r--   0        0        0     1900 2023-08-07 20:28:25.582852 aiogramarch-1.1.1/aiogramarch/cli/app.py
--rw-r--r--   0        0        0      146 2023-02-11 08:53:23.735388 aiogramarch-1.1.1/aiogramarch/cli/context.py
--rw-r--r--   0        0        0     1692 2023-08-07 19:59:26.089012 aiogramarch-1.1.1/aiogramarch/cli/template_generator.py
--rw-r--r--   0        0        0        0 2023-02-10 13:55:25.163909 aiogramarch-1.1.1/aiogramarch/cli/templates/__init__.py
--rw-r--r--   0        0        0        0 2023-02-10 13:56:06.325380 aiogramarch-1.1.1/aiogramarch/cli/templates/app/__init__.py
--rw-r--r--   0        0        0       53 2023-02-11 09:02:53.545791 aiogramarch-1.1.1/aiogramarch/cli/templates/app/cookiecutter.json
--rw-r--r--   0        0        0        0 2023-02-10 13:56:38.157436 aiogramarch-1.1.1/aiogramarch/cli/templates/app/{{ cookiecutter.app_name }}/__init__.py
--rw-r--r--   0        0        0      129 2023-03-04 17:18:05.655741 aiogramarch-1.1.1/aiogramarch/cli/templates/app/{{ cookiecutter.app_name }}/callback_factory.py
--rw-r--r--   0        0        0      282 2023-03-04 17:16:16.525039 aiogramarch-1.1.1/aiogramarch/cli/templates/app/{{ cookiecutter.app_name }}/handlers.py
--rw-r--r--   0        0        0      176 2023-03-05 14:28:59.447671 aiogramarch-1.1.1/aiogramarch/cli/templates/app/{{ cookiecutter.app_name }}/models.py
--rw-r--r--   0        0        0       25 2023-03-04 17:17:27.233059 aiogramarch-1.1.1/aiogramarch/cli/templates/app/{{ cookiecutter.app_name }}/services.py
--rw-r--r--   0        0        0      105 2023-03-04 17:19:10.183520 aiogramarch-1.1.1/aiogramarch/cli/templates/app/{{ cookiecutter.app_name }}/states.py
--rw-r--r--   0        0        0        0 2023-02-10 13:56:49.743140 aiogramarch-1.1.1/aiogramarch/cli/templates/project/__init__.py
--rw-r--r--   0        0        0       61 2023-02-11 08:05:26.713003 aiogramarch-1.1.1/aiogramarch/cli/templates/project/cookiecutter.json
--rw-r--r--   0        0        0       43 2023-08-07 15:25:49.081310 aiogramarch-1.1.1/aiogramarch/cli/templates/project/{{ cookiecutter.project_name }}/env.env
--rw-r--r--   0        0        0       69 2023-08-07 15:25:49.090311 aiogramarch-1.1.1/aiogramarch/cli/templates/project/{{ cookiecutter.project_name }}/main.py
--rw-r--r--   0        0        0      111 2023-08-07 16:41:13.805407 aiogramarch-1.1.1/aiogramarch/cli/templates/project/{{ cookiecutter.project_name }}/requirements.txt
--rw-r--r--   0        0        0     2166 2023-08-07 17:52:05.206228 aiogramarch-1.1.1/aiogramarch/cli/templates/project/{{ cookiecutter.project_name }}/src/__init__.py
--rw-r--r--   0        0        0     1119 2023-08-08 06:54:42.284247 aiogramarch-1.1.1/aiogramarch/config.py
--rw-r--r--   0        0        0     1126 2023-02-10 12:44:45.759881 aiogramarch-1.1.1/LICENSE.md
--rw-r--r--   0        0        0      553 2023-08-08 08:19:54.011327 aiogramarch-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      371 2023-07-31 10:11:05.219982 aiogramarch-1.1.1/README.md
--rw-r--r--   0        0        0     1528 1970-01-01 00:00:00.000000 aiogramarch-1.1.1/setup.py
--rw-r--r--   0        0        0     1078 1970-01-01 00:00:00.000000 aiogramarch-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      115 2023-08-07 05:37:42.215703 aiogramarch-1.1.2/aiogramarch/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 22:13:31.659111 aiogramarch-1.1.2/aiogramarch/arch/__init__.py
+-rw-r--r--   0        0        0      157 2023-08-07 05:35:28.876890 aiogramarch-1.1.2/aiogramarch/arch/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      748 2023-08-07 05:35:30.855903 aiogramarch-1.1.2/aiogramarch/arch/__pycache__/database.cpython-310.pyc
+-rw-r--r--   0        0        0      718 2023-08-07 05:36:51.010457 aiogramarch-1.1.2/aiogramarch/arch/__pycache__/settings.cpython-310.pyc
+-rw-r--r--   0        0        0     1187 2023-08-07 06:33:59.219744 aiogramarch-1.1.2/aiogramarch/arch/__pycache__/startapp.cpython-310.pyc
+-rw-r--r--   0        0        0      227 2023-08-08 08:01:12.391123 aiogramarch-1.1.2/aiogramarch/arch/bot.py
+-rw-r--r--   0        0        0      348 2023-08-07 10:31:28.484918 aiogramarch-1.1.2/aiogramarch/arch/database.py
+-rw-r--r--   0        0        0      390 2023-08-08 08:22:00.093543 aiogramarch-1.1.2/aiogramarch/arch/settings.py
+-rw-r--r--   0        0        0     1076 2023-08-08 08:03:41.900952 aiogramarch-1.1.2/aiogramarch/arch/startapp.py
+-rw-r--r--   0        0        0        0 2023-08-07 14:49:53.686426 aiogramarch-1.1.2/aiogramarch/cli/__init__.py
+-rw-r--r--   0        0        0      156 2023-08-07 14:50:16.402156 aiogramarch-1.1.2/aiogramarch/cli/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2041 2023-08-07 20:53:48.068830 aiogramarch-1.1.2/aiogramarch/cli/__pycache__/app.cpython-310.pyc
+-rw-r--r--   0        0        0      530 2023-08-07 14:52:37.611292 aiogramarch-1.1.2/aiogramarch/cli/__pycache__/context.cpython-310.pyc
+-rw-r--r--   0        0        0     1850 2023-08-07 20:15:40.995105 aiogramarch-1.1.2/aiogramarch/cli/__pycache__/template_generator.cpython-310.pyc
+-rw-r--r--   0        0        0     1900 2023-08-07 20:28:25.582852 aiogramarch-1.1.2/aiogramarch/cli/app.py
+-rw-r--r--   0        0        0      146 2023-02-11 08:53:23.735388 aiogramarch-1.1.2/aiogramarch/cli/context.py
+-rw-r--r--   0        0        0     1692 2023-08-07 19:59:26.089012 aiogramarch-1.1.2/aiogramarch/cli/template_generator.py
+-rw-r--r--   0        0        0        0 2023-02-10 13:55:25.163909 aiogramarch-1.1.2/aiogramarch/cli/templates/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-10 13:56:06.325380 aiogramarch-1.1.2/aiogramarch/cli/templates/app/__init__.py
+-rw-r--r--   0        0        0       53 2023-02-11 09:02:53.545791 aiogramarch-1.1.2/aiogramarch/cli/templates/app/cookiecutter.json
+-rw-r--r--   0        0        0        0 2023-02-10 13:56:38.157436 aiogramarch-1.1.2/aiogramarch/cli/templates/app/{{ cookiecutter.app_name }}/__init__.py
+-rw-r--r--   0        0        0      129 2023-03-04 17:18:05.655741 aiogramarch-1.1.2/aiogramarch/cli/templates/app/{{ cookiecutter.app_name }}/callback_factory.py
+-rw-r--r--   0        0        0      282 2023-03-04 17:16:16.525039 aiogramarch-1.1.2/aiogramarch/cli/templates/app/{{ cookiecutter.app_name }}/handlers.py
+-rw-r--r--   0        0        0      176 2023-03-05 14:28:59.447671 aiogramarch-1.1.2/aiogramarch/cli/templates/app/{{ cookiecutter.app_name }}/models.py
+-rw-r--r--   0        0        0       25 2023-03-04 17:17:27.233059 aiogramarch-1.1.2/aiogramarch/cli/templates/app/{{ cookiecutter.app_name }}/services.py
+-rw-r--r--   0        0        0      105 2023-03-04 17:19:10.183520 aiogramarch-1.1.2/aiogramarch/cli/templates/app/{{ cookiecutter.app_name }}/states.py
+-rw-r--r--   0        0        0        0 2023-02-10 13:56:49.743140 aiogramarch-1.1.2/aiogramarch/cli/templates/project/__init__.py
+-rw-r--r--   0        0        0       61 2023-02-11 08:05:26.713003 aiogramarch-1.1.2/aiogramarch/cli/templates/project/cookiecutter.json
+-rw-r--r--   0        0        0       43 2023-08-07 15:25:49.081310 aiogramarch-1.1.2/aiogramarch/cli/templates/project/{{ cookiecutter.project_name }}/env.env
+-rw-r--r--   0        0        0       69 2023-08-07 15:25:49.090311 aiogramarch-1.1.2/aiogramarch/cli/templates/project/{{ cookiecutter.project_name }}/main.py
+-rw-r--r--   0        0        0      111 2023-08-07 16:41:13.805407 aiogramarch-1.1.2/aiogramarch/cli/templates/project/{{ cookiecutter.project_name }}/requirements.txt
+-rw-r--r--   0        0        0     2166 2023-08-07 17:52:05.206228 aiogramarch-1.1.2/aiogramarch/cli/templates/project/{{ cookiecutter.project_name }}/src/__init__.py
+-rw-r--r--   0        0        0     1423 2023-08-07 15:25:49.096319 aiogramarch-1.1.2/aiogramarch/cli/templates/project/{{ cookiecutter.project_name }}/src/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1119 2023-08-08 06:54:42.284247 aiogramarch-1.1.2/aiogramarch/config.py
+-rw-r--r--   0        0        0     1126 2023-02-10 12:44:45.759881 aiogramarch-1.1.2/LICENSE.md
+-rw-r--r--   0        0        0      553 2023-08-08 08:22:40.282947 aiogramarch-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      371 2023-07-31 10:11:05.219982 aiogramarch-1.1.2/README.md
+-rw-r--r--   0        0        0     1528 1970-01-01 00:00:00.000000 aiogramarch-1.1.2/setup.py
+-rw-r--r--   0        0        0     1078 1970-01-01 00:00:00.000000 aiogramarch-1.1.2/PKG-INFO
```

### Comparing `aiogramarch-1.1.1/aiogramarch/arch/startapp.py` & `aiogramarch-1.1.2/aiogramarch/arch/startapp.py`

 * *Files identical despite different names*

### Comparing `aiogramarch-1.1.1/aiogramarch/cli/app.py` & `aiogramarch-1.1.2/aiogramarch/cli/app.py`

 * *Files identical despite different names*

### Comparing `aiogramarch-1.1.1/aiogramarch/cli/template_generator.py` & `aiogramarch-1.1.2/aiogramarch/cli/template_generator.py`

 * *Files identical despite different names*

### Comparing `aiogramarch-1.1.1/aiogramarch/cli/templates/project/{{ cookiecutter.project_name }}/src/__init__.py` & `aiogramarch-1.1.2/aiogramarch/cli/templates/project/{{ cookiecutter.project_name }}/src/__init__.py`

 * *Files identical despite different names*

### Comparing `aiogramarch-1.1.1/aiogramarch/config.py` & `aiogramarch-1.1.2/aiogramarch/config.py`

 * *Files identical despite different names*

### Comparing `aiogramarch-1.1.1/LICENSE.md` & `aiogramarch-1.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aiogramarch-1.1.1/pyproject.toml` & `aiogramarch-1.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiogramarch"
-version = "1.1.1"
+version = "1.1.2"
 description = "Managing aiogram projects"
 authors = ["BulatXam <Khamdbulat@yandex.ru>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7"
```

### Comparing `aiogramarch-1.1.1/setup.py` & `aiogramarch-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
  'pydantic==1.10.12']
 
 entry_points = \
 {'console_scripts': ['aiogramarch = aiogramarch.template.app:cli']}
 
 setup_kwargs = {
     'name': 'aiogramarch',
-    'version': '1.1.1',
+    'version': '1.1.2',
     'description': 'Managing aiogram projects',
     'long_description': '# <p align="center"> Aiogramarch </p>\nProject manager and generator for Aiogram\n\n\n\n___\n\n## Installation\n\n``` python\npip install aiogram-manager\n```\n___\n\n## How to use\n\n``` bash\naiogram startproject [projectname]\n```\n\n``` bash\ncd codingbot\n```\n\n``` bash\naiogram startapp [appname]\n```\n\n___\n\n## Utils options\n\n``` bash\naiogram --help\n```\n',
     'author': 'BulatXam',
     'author_email': 'Khamdbulat@yandex.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `aiogramarch-1.1.1/PKG-INFO` & `aiogramarch-1.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogramarch
-Version: 1.1.1
+Version: 1.1.2
 Summary: Managing aiogram projects
 License: MIT
 Author: BulatXam
 Author-email: Khamdbulat@yandex.ru
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

