# Comparing `tmp/xdcget-0.2.3.tar.gz` & `tmp/xdcget-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdcget-0.2.3.tar", last modified: Mon Jul 17 08:18:30 2023, max compression
+gzip compressed data, was "xdcget-0.3.0.tar", last modified: Tue Aug  8 16:35:56 2023, max compression
```

## Comparing `xdcget-0.2.3.tar` & `xdcget-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,32 @@
-drwxrwxr-x   0 hpk       (1000) hpk       (1000)        0 2023-07-17 08:18:30.439728 xdcget-0.2.3/
--rw-rw-r--   0 hpk       (1000) hpk       (1000)     3352 2023-07-17 08:18:30.439728 xdcget-0.2.3/PKG-INFO
--rw-rw-r--   0 hpk       (1000) hpk       (1000)     2800 2023-07-17 08:17:51.000000 xdcget-0.2.3/README.md
--rw-rw-r--   0 hpk       (1000) hpk       (1000)     1310 2023-07-17 08:18:18.000000 xdcget-0.2.3/pyproject.toml
--rw-rw-r--   0 hpk       (1000) hpk       (1000)       38 2023-07-17 08:18:30.439728 xdcget-0.2.3/setup.cfg
-drwxrwxr-x   0 hpk       (1000) hpk       (1000)        0 2023-07-17 08:18:30.439728 xdcget-0.2.3/src/
-drwxrwxr-x   0 hpk       (1000) hpk       (1000)        0 2023-07-17 08:18:30.439728 xdcget-0.2.3/src/xdcget/
--rw-rw-r--   0 hpk       (1000) hpk       (1000)        2 2023-07-05 12:29:52.000000 xdcget-0.2.3/src/xdcget/__init__.py
--rw-rw-r--   0 hpk       (1000) hpk       (1000)     6643 2023-07-13 14:35:59.000000 xdcget-0.2.3/src/xdcget/config.py
--rw-rw-r--   0 hpk       (1000) hpk       (1000)     2311 2023-07-13 14:35:59.000000 xdcget-0.2.3/src/xdcget/main.py
--rw-rw-r--   0 hpk       (1000) hpk       (1000)    11185 2023-07-14 13:04:30.000000 xdcget-0.2.3/src/xdcget/storage.py
-drwxrwxr-x   0 hpk       (1000) hpk       (1000)        0 2023-07-17 08:18:30.439728 xdcget-0.2.3/src/xdcget.egg-info/
--rw-rw-r--   0 hpk       (1000) hpk       (1000)     3352 2023-07-17 08:18:30.000000 xdcget-0.2.3/src/xdcget.egg-info/PKG-INFO
--rw-rw-r--   0 hpk       (1000) hpk       (1000)      377 2023-07-17 08:18:30.000000 xdcget-0.2.3/src/xdcget.egg-info/SOURCES.txt
--rw-rw-r--   0 hpk       (1000) hpk       (1000)        1 2023-07-17 08:18:30.000000 xdcget-0.2.3/src/xdcget.egg-info/dependency_links.txt
--rw-rw-r--   0 hpk       (1000) hpk       (1000)       44 2023-07-17 08:18:30.000000 xdcget-0.2.3/src/xdcget.egg-info/entry_points.txt
--rw-rw-r--   0 hpk       (1000) hpk       (1000)       43 2023-07-17 08:18:30.000000 xdcget-0.2.3/src/xdcget.egg-info/requires.txt
--rw-rw-r--   0 hpk       (1000) hpk       (1000)        7 2023-07-17 08:18:30.000000 xdcget-0.2.3/src/xdcget.egg-info/top_level.txt
-drwxrwxr-x   0 hpk       (1000) hpk       (1000)        0 2023-07-17 08:18:30.439728 xdcget-0.2.3/tests/
--rw-rw-r--   0 hpk       (1000) hpk       (1000)     2438 2023-07-16 11:24:32.000000 xdcget-0.2.3/tests/test_config.py
--rw-rw-r--   0 hpk       (1000) hpk       (1000)     1521 2023-07-16 11:24:32.000000 xdcget-0.2.3/tests/test_main.py
--rw-rw-r--   0 hpk       (1000) hpk       (1000)     2695 2023-07-16 11:24:32.000000 xdcget-0.2.3/tests/test_storage.py
+drwxrwxr-x   0 hpk       (1000) hpk       (1000)        0 2023-08-08 16:35:56.447983 xdcget-0.3.0/
+drwxrwxr-x   0 hpk       (1000) hpk       (1000)        0 2023-08-08 16:35:56.443983 xdcget-0.3.0/.forgejo/
+drwxrwxr-x   0 hpk       (1000) hpk       (1000)        0 2023-08-08 16:35:56.447983 xdcget-0.3.0/.forgejo/workflows/
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)      468 2023-08-05 15:54:53.000000 xdcget-0.3.0/.forgejo/workflows/test.yml
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)     2035 2023-07-20 13:08:37.000000 xdcget-0.3.0/.gitignore
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)    16727 2023-07-17 09:17:17.000000 xdcget-0.3.0/LICENSE
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)     3623 2023-08-08 16:35:56.447983 xdcget-0.3.0/PKG-INFO
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)     3071 2023-07-24 14:16:36.000000 xdcget-0.3.0/README.md
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)     1695 2023-08-05 15:54:53.000000 xdcget-0.3.0/pyproject.toml
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)       38 2023-08-08 16:35:56.447983 xdcget-0.3.0/setup.cfg
+drwxrwxr-x   0 hpk       (1000) hpk       (1000)        0 2023-08-08 16:35:56.443983 xdcget-0.3.0/src/
+drwxrwxr-x   0 hpk       (1000) hpk       (1000)        0 2023-08-08 16:35:56.447983 xdcget-0.3.0/src/xdcget/
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)      129 2023-07-20 13:08:37.000000 xdcget-0.3.0/src/xdcget/__init__.py
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)      160 2023-08-08 16:35:56.000000 xdcget-0.3.0/src/xdcget/_version.py
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)     6717 2023-08-05 17:43:48.000000 xdcget-0.3.0/src/xdcget/config.py
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)      704 2023-07-28 07:22:16.000000 xdcget-0.3.0/src/xdcget/errors.py
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)     3051 2023-07-28 07:22:16.000000 xdcget-0.3.0/src/xdcget/main.py
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)    11740 2023-07-28 07:22:16.000000 xdcget-0.3.0/src/xdcget/storage.py
+drwxrwxr-x   0 hpk       (1000) hpk       (1000)        0 2023-08-08 16:35:56.447983 xdcget-0.3.0/src/xdcget.egg-info/
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)     3623 2023-08-08 16:35:56.000000 xdcget-0.3.0/src/xdcget.egg-info/PKG-INFO
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)      509 2023-08-08 16:35:56.000000 xdcget-0.3.0/src/xdcget.egg-info/SOURCES.txt
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)        1 2023-08-08 16:35:56.000000 xdcget-0.3.0/src/xdcget.egg-info/dependency_links.txt
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)       44 2023-08-08 16:35:56.000000 xdcget-0.3.0/src/xdcget.egg-info/entry_points.txt
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)       24 2023-08-08 16:35:56.000000 xdcget-0.3.0/src/xdcget.egg-info/requires.txt
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)        7 2023-08-08 16:35:56.000000 xdcget-0.3.0/src/xdcget.egg-info/top_level.txt
+drwxrwxr-x   0 hpk       (1000) hpk       (1000)        0 2023-08-08 16:35:56.447983 xdcget-0.3.0/tests/
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)     5284 2023-08-05 17:43:48.000000 xdcget-0.3.0/tests/conftest.py
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)     3460 2023-07-19 14:22:44.000000 xdcget-0.3.0/tests/test_config.py
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)     3016 2023-08-05 17:43:48.000000 xdcget-0.3.0/tests/test_main.py
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)     2877 2023-08-05 15:54:53.000000 xdcget-0.3.0/tests/test_storage.py
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)     8522 2023-07-27 09:04:06.000000 xdcget-0.3.0/xdcget.ini
+-rw-rw-r--   0 hpk       (1000) hpk       (1000)    12816 2023-08-05 17:43:48.000000 xdcget-0.3.0/xdcget.lock
```

### Comparing `xdcget-0.2.3/PKG-INFO` & `xdcget-0.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,93 +1,110 @@
 Metadata-Version: 2.1
 Name: xdcget
-Version: 0.2.3
+Version: 0.3.0
 Summary: experimental tool for collecting latest releases of webxdc apps
 License: MPL-2.0
 Project-URL: homepage, https://codeberg.org/webxdc/xdcget
 Project-URL: issues, https://codeberg.org/webxdc/xdcget/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: POSIX
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: test
+License-File: LICENSE
 
 
 # xdcget: a command line tool to collect webxdc apps from git repositories 
 
-The "xdcget" command line tool collects [WebXDC](https://webxdc.org) apps
-via the release API of Codeberg and Github.
 The main purpose for this tool is to maintain a cache of released webxdc apps
 and to export release files so they can be imported from the 
-[WebXDC Store](https://github.com/webxdc/store)
-which in turn can be used by Delta Chat users to discover webxdc apps for sharing in chats. 
+[xdcstore bot](https://github.com/webxdc/store)
+which in turn can be contacted by Delta Chat users 
+in order to be able to search and share webxdc apps in chats. 
 
 ## Getting started  
 
 1. Install `xdcget` command line tool from a local checkout:
 
         pip install -e . 
 
 2. Initialize config files: 
 
         xdcget init 
 
-3. Edit `xdcget.ini` to contain your Codeberg and Github API access token (see below)
-   and also adjust config options as needed.  
+3. Edit `xdcget.ini` and make sure that you set environment variables 
+   containing your credentials for Codeberg/Github API usage. 
+   See below for how to get API credentials. 
 
-4. Edit `sources.ini` to modify the list of source repositories. 
-
-5. Run the `update` command to cache all releases for 
-   repositories listed in `sources.ini`:
+4. Run the `update` command to retrieve newest webxdc app releases 
+   for repositories listed in `xdcget.ini` and export them to the `export` directory: 
 
         xdcget update 
 
-6. Run the `export` command to create files for `xdcstore import <PATH>`
-
-        xdcget export 
 
 ## Getting a Codeberg API access token 
 
 Login with Codeberg and open https://codeberg.org/user/settings/applications 
 to generate a new token.  This token does not need any special "scopes"
-it's only used for querying releases of public repositories.  
+it's only used for querying releases of public repositories.
 You can copy the resulting API token into your clipboard
-and then insert it into the config file: 
-
-    # the line you need to put into `xdcget.ini` 
-    CODEBERG_USER = <your-codeberg-user-name> 
-    CODEBERG_TOKEN = <paste-your-codeberg-access-token-here> 
+and then set it into the environment variables you declared in the config file:
 
+    # bash example
+    export XDCGET_CODEBERG_USER=<your-codeberg-user-name>
+    export XDCGET_CODEBERG_TOKEN=<paste-your-codeberg-access-token-here>
 
 ## Getting a Github API access token 
 
 Login with github and open https://github.com/settings/tokens
 to generate a new token.  This token does not need any access
 to your private repos -- it's only used for querying releases 
 of public repositories.  You may give it 90 days or other expiration
 times as you feel fine with. 
 You can copy the resulting API token into your clipboard
-and then insert it into the config file: 
+and then set it into the environment variables you declared in the config file:
+
+    # bash example
+    export XDCGET_GITHUB_USER=<your-github-user-name>
+    export XDCGET_GITHUB_TOKEN=<paste-your-github-access-token-here>
+
+## Contributing
+
+Install tox:
 
-    # the line you need to put into `xdcget.ini` 
-    GITHUB_USER = <your-github-user-name> 
-    GITHUB_TOKEN = <paste-your-github-access-token-here> 
+```
+pip install tox
+```
 
+We use [black](https://github.com/psf/black) to format the code and [ruff](https://beta.ruff.rs/docs) as linter. After modifying the code, run:
 
-## Building and publishing xdcget releases (maintainer notes)
+```
+tox -e lint
+```
 
-This project uses a single `pyproject.toml` to define all python build/test metadata.
-See [Packaging Python Projects](https://packaging.python.org/en/latest/tutorials/packaging-projects/?highlight=pyproject.toml) for more details. 
+Run automated tests with:
 
-Quick notes on requirements for releasing: 
+```
+tox
+```
 
-- `pip install build twine` for building and uploading distribution files 
+**IMPORTANT:** Pull Requests with new features / bug fixes should come with automated tests.
+
+### Building and publishing xdcget releases
+
+Quick notes on requirements for testing and releasing: 
+
+- `pip install tox build twine` to install development dependencies
+
+- `tox` to run tests
 
 - `python -m build` to build the distribution files
 
 - [create API-tokens on PyPI](https://pypi.org/manage/account/)
   to be able to upload to PyPI repositories. 
 
-- `twine upload dist/*` to upload all built distribution files 
+- Use git to tag a release before uploading (e.g. "git tag" and "git push --tags") 
+  The version of xdcget (also obtained via `xdcget --version`) is dynamically 
+  computed using [setuptools-scm](https://pypi.org/project/setuptools-scm/)
 
+- `twine upload dist/*` to upload all built distribution files
```

### Comparing `xdcget-0.2.3/README.md` & `xdcget-0.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,78 +1,95 @@
 
 # xdcget: a command line tool to collect webxdc apps from git repositories 
 
-The "xdcget" command line tool collects [WebXDC](https://webxdc.org) apps
-via the release API of Codeberg and Github.
 The main purpose for this tool is to maintain a cache of released webxdc apps
 and to export release files so they can be imported from the 
-[WebXDC Store](https://github.com/webxdc/store)
-which in turn can be used by Delta Chat users to discover webxdc apps for sharing in chats. 
+[xdcstore bot](https://github.com/webxdc/store)
+which in turn can be contacted by Delta Chat users 
+in order to be able to search and share webxdc apps in chats. 
 
 ## Getting started  
 
 1. Install `xdcget` command line tool from a local checkout:
 
         pip install -e . 
 
 2. Initialize config files: 
 
         xdcget init 
 
-3. Edit `xdcget.ini` to contain your Codeberg and Github API access token (see below)
-   and also adjust config options as needed.  
+3. Edit `xdcget.ini` and make sure that you set environment variables 
+   containing your credentials for Codeberg/Github API usage. 
+   See below for how to get API credentials. 
 
-4. Edit `sources.ini` to modify the list of source repositories. 
-
-5. Run the `update` command to cache all releases for 
-   repositories listed in `sources.ini`:
+4. Run the `update` command to retrieve newest webxdc app releases 
+   for repositories listed in `xdcget.ini` and export them to the `export` directory: 
 
         xdcget update 
 
-6. Run the `export` command to create files for `xdcstore import <PATH>`
-
-        xdcget export 
 
 ## Getting a Codeberg API access token 
 
 Login with Codeberg and open https://codeberg.org/user/settings/applications 
 to generate a new token.  This token does not need any special "scopes"
-it's only used for querying releases of public repositories.  
+it's only used for querying releases of public repositories.
 You can copy the resulting API token into your clipboard
-and then insert it into the config file: 
-
-    # the line you need to put into `xdcget.ini` 
-    CODEBERG_USER = <your-codeberg-user-name> 
-    CODEBERG_TOKEN = <paste-your-codeberg-access-token-here> 
+and then set it into the environment variables you declared in the config file:
 
+    # bash example
+    export XDCGET_CODEBERG_USER=<your-codeberg-user-name>
+    export XDCGET_CODEBERG_TOKEN=<paste-your-codeberg-access-token-here>
 
 ## Getting a Github API access token 
 
 Login with github and open https://github.com/settings/tokens
 to generate a new token.  This token does not need any access
 to your private repos -- it's only used for querying releases 
 of public repositories.  You may give it 90 days or other expiration
 times as you feel fine with. 
 You can copy the resulting API token into your clipboard
-and then insert it into the config file: 
+and then set it into the environment variables you declared in the config file:
+
+    # bash example
+    export XDCGET_GITHUB_USER=<your-github-user-name>
+    export XDCGET_GITHUB_TOKEN=<paste-your-github-access-token-here>
+
+## Contributing
+
+Install tox:
 
-    # the line you need to put into `xdcget.ini` 
-    GITHUB_USER = <your-github-user-name> 
-    GITHUB_TOKEN = <paste-your-github-access-token-here> 
+```
+pip install tox
+```
 
+We use [black](https://github.com/psf/black) to format the code and [ruff](https://beta.ruff.rs/docs) as linter. After modifying the code, run:
 
-## Building and publishing xdcget releases (maintainer notes)
+```
+tox -e lint
+```
 
-This project uses a single `pyproject.toml` to define all python build/test metadata.
-See [Packaging Python Projects](https://packaging.python.org/en/latest/tutorials/packaging-projects/?highlight=pyproject.toml) for more details. 
+Run automated tests with:
 
-Quick notes on requirements for releasing: 
+```
+tox
+```
 
-- `pip install build twine` for building and uploading distribution files 
+**IMPORTANT:** Pull Requests with new features / bug fixes should come with automated tests.
+
+### Building and publishing xdcget releases
+
+Quick notes on requirements for testing and releasing: 
+
+- `pip install tox build twine` to install development dependencies
+
+- `tox` to run tests
 
 - `python -m build` to build the distribution files
 
 - [create API-tokens on PyPI](https://pypi.org/manage/account/)
   to be able to upload to PyPI repositories. 
 
-- `twine upload dist/*` to upload all built distribution files 
+- Use git to tag a release before uploading (e.g. "git tag" and "git push --tags") 
+  The version of xdcget (also obtained via `xdcget --version`) is dynamically 
+  computed using [setuptools-scm](https://pypi.org/project/setuptools-scm/)
 
+- `twine upload dist/*` to upload all built distribution files
```

### Comparing `xdcget-0.2.3/pyproject.toml` & `xdcget-0.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+[build-system]
+requires = ["setuptools>=45", "setuptools_scm[toml]>=6.2"]
+build-backend = "setuptools.build_meta"
+
 [project]
 name = "xdcget"
-version = "0.2.3"
+dynamic = ["version"]
 description = "experimental tool for collecting latest releases of webxdc apps"
 license = {text = "MPL-2.0"}
-requires-python = ">=3.10"
+requires-python = ">=3.9"
 readme = "README.md"
 
 scripts = {xdcget = "xdcget.main:main"}
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
@@ -18,55 +22,66 @@
 
 dependencies = [
     "requests",
     "termcolor",
     "toml",
 ]
 
-[project.optional-dependencies]
-test = ["pytest", "tox"]
-
 [project.urls]
 homepage = "https://codeberg.org/webxdc/xdcget"
 issues = "https://codeberg.org/webxdc/xdcget/issues"
 
+[tool.setuptools_scm]
+write_to = "src/xdcget/_version.py"
+
+[tool.pytest.ini_options]
+addopts = "-v -ra --strict-markers"
+norecursedirs = ".tox"
+xfail_strict = true
+timeout = 150
+timeout_func_only = true
+
 [tool.tox]
 legacy_tox_ini = """
 [tox]
+isolated_build = true
 envlist =
     py3
     lint
 
 [testenv]
 commands =
     pytest {posargs: tests}
 passenv =
-    GITHUB_USER
-    GITHUB_TOKEN
-    CODEBERG_USER
-    CODEBERG_TOKEN
+    XDCGET_GITHUB_USER
+    XDCGET_GITHUB_TOKEN
+    XDCGET_CODEBERG_USER
+    XDCGET_CODEBERG_TOKEN
 deps =
     pytest
     pytest-timeout
     pdbpp
+    requests-mock
 
 
 [testenv:lint]
 skipsdist = True
 skip_install = True
 deps =
     ruff
     black
 commands =
     black --quiet --check --diff src/xdcget tests/
     ruff src/xdcget tests/
-
-
-[pytest]
-addopts = -v -ra --strict-markers
-norecursedirs = .tox
-xfail_strict=true
-timeout = 150
-timeout_func_only = True
-markers =
-    ignored: ignore this test in default test runs, use --ignored to run.
 """
+
+[tool.ruff]
+select = [
+    "E", "W", # pycodestyle
+    "F", # Pyflakes
+    "PTH", # flake8-use-pathlib
+    "I", # isort
+    "RUF", # Ruff-specific rules
+    "UP", # pyupgrade
+    "YTT", # flake8-2020
+    "D400", "D401", "D402", "D403", "D404", # pydocstyle
+]
```

### Comparing `xdcget-0.2.3/src/xdcget/config.py` & `xdcget-0.3.0/src/xdcget/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,146 +1,135 @@
+import configparser
 import os
-import time
 import re
-from pathlib import Path
+import time
+from contextlib import contextmanager
 from dataclasses import dataclass
+from pathlib import Path
 from typing import Optional
 
-import configparser
-from contextlib import contextmanager
+from .errors import EmptyOrUnsetEnvVar, MissingOrEmptyField
 
 
 @contextmanager
 def line_writer(fn):
     with fn.open("w") as f:
 
         def writer(*args):
             print(*args, file=f)
 
         yield writer
 
 
 def write_initial_config(xdcget_ini, out):
     assert not xdcget_ini.exists(), xdcget_ini
-
-    export_dir = Path("export_dir")
-    cache_dir = Path("cache_dir")
-    sources_ini_path = Path("sources.ini")
-    if not sources_ini_path.exists():
-        with line_writer(sources_ini_path) as w:
-            w("#[<projectname>]")
-            w("#app_id = ")
-            w("#source_code_url = ")
-        out.green(f"created -- please inspect: {sources_ini_path}")
-    else:
-        out.green(f"using existing sources: {sources_ini_path}")
-
-    def getenv_or_empty(key):
-        return os.environ.get(key, "")
-
     write_xdcget_ini(
-        xdcget_ini,
-        export_dir=export_dir,
-        cache_dir=cache_dir,
-        sources_ini_path=sources_ini_path,
-        codeberg_user=getenv_or_empty("CODEBERG_USER"),
-        codeberg_token=getenv_or_empty("CODEBERG_TOKEN"),
-        github_user=getenv_or_empty("GITHUB_USER"),
-        github_token=getenv_or_empty("GITHUB_TOKEN"),
+        xdcget_ini, export_dir=Path("export_dir"), cache_dir=Path("cache_dir")
     )
     out.green(f"created -- please inspect: {xdcget_ini}")
 
 
 def write_xdcget_ini(
     path,
     export_dir,
     cache_dir,
-    sources_ini_path,
-    codeberg_user,
-    codeberg_token,
-    github_user,
-    github_token,
+    codeberg_user_env_var="XDCGET_CODEBERG_USER",
+    codeberg_token_env_var="XDCGET_CODEBERG_TOKEN",
+    github_user_env_var="XDCGET_GITHUB_USER",
+    github_token_env_var="XDCGET_GITHUB_TOKEN",
+    sources="""\
+#[app:<projectname>]
+#source_code_url =
+##description =
+""",
 ):
     def get_rel_or_abs(path, rootpath):
         path = path.absolute()
         rootpath = rootpath.absolute()
         if path.is_relative_to(rootpath.parent):
             return Path(path.relative_to(rootpath.parent))
         return path
 
     with line_writer(path) as w:
         cache_dir = get_rel_or_abs(cache_dir, path)
         export_dir = get_rel_or_abs(export_dir, path)
-        sources_ini_path = get_rel_or_abs(sources_ini_path, path)
 
         w("[xdcget]")
         w("# all paths can be relative to the directory of the xdcget.ini file")
         w(f"export_dir = {export_dir}")
         w(f"cache_dir = {cache_dir}")
-        w(f"sources = {sources_ini_path}")
         w()
-        w("[api-codeberg]")
+        w("[api:codeberg]")
         w("root_url = https://codeberg.org")
         w("api_url = https://codeberg.org/api/v1/")
-        w(f"user = {codeberg_user}")
-        w(f"token = {codeberg_token}")
+        w(f"user_env_var = {codeberg_user_env_var}")
+        w(f"token_env_var = {codeberg_token_env_var}")
         w()
-        w("[api-github]")
+        w("[api:github]")
         w("root_url = https://github.com")
         w("api_url = https://api.github.com/")
-        w(f"user = {github_user}")
-        w(f"token = {github_token}")
+        w(f"user_env_var = {github_user_env_var}")
+        w(f"token_env_var = {github_token_env_var}")
+        w()
+        w(sources)
 
 
 def read_config(xdcget_ini_path):
     with xdcget_ini_path.open("r") as f:
         parser = configparser.ConfigParser()
         parser.read_file(f)
         api_defs = []
+        app_defs = []
         cfg = None
         basedir = xdcget_ini_path.parent
         for key in sorted(parser.sections()):
             api_def = parser[key]
-            if not key.startswith("api-"):
+            if key.startswith("api:"):
+                if not api_def.get("user_env_var"):
+                    raise MissingOrEmptyField(section=key, field="user_env_var")
+                if not api_def.get("token_env_var"):
+                    raise MissingOrEmptyField(section=key, field="token_env_var")
+                user = os.environ.get(api_def["user_env_var"])
+                if not user:
+                    raise EmptyOrUnsetEnvVar(section=key, var=api_def["user_env_var"])
+                token = os.environ.get(api_def["token_env_var"])
+                if not token:
+                    raise EmptyOrUnsetEnvVar(section=key, var=api_def["token_env_var"])
+                api_defs.append(
+                    HostedApiDef(
+                        api_def["root_url"], api_def["api_url"], user=user, token=token
+                    )
+                )
+            elif key.startswith("app:"):
+                app_id = key[len("app:") :]
+                validate_app_id(app_id)
+                app_defs.append(SourceDef(app_id=app_id, **parser[key]))
+            else:
                 assert key == "xdcget"
                 cfg = parser[key]
-                continue
-            api_defs.append(HostedApiDef(**api_def))
-        sources_path = basedir.joinpath(cfg["sources"])
-        source_defs = parse_sources_ini(sources_path)
 
     return Config(
         xdcget_ini_path=xdcget_ini_path,
         export_dir=basedir.joinpath(cfg["export_dir"]),
         cache_dir=basedir.joinpath(cfg["cache_dir"]),
         api_defs=api_defs,
-        source_defs=source_defs,
+        source_defs=app_defs,
     )
 
 
-class InvalidAppId(Exception):
-    """Invalid app-id for a app"""
+def validate_app_id(app_id):
+    if app_id.lower() != app_id:
+        raise InvalidAppId(f"{app_id!r} is not lowercase")
+    rex = re.compile(r"^[a-z][a-z0-9\-]*$")
+    if not rex.match(app_id) or app_id.strip("-") != app_id:
+        raise InvalidAppId(f"{app_id!r} contains invalid characters")
 
 
-def parse_sources_ini(path):
-    assert path.exists(), path
-    parser = configparser.ConfigParser()
-    parser.read(path)
-    rex = re.compile(r"^[a-z][a-z0-9\-]*$")
-    res = []
-    for app_id in sorted(parser.sections()):
-        if app_id.lower() != app_id:
-            raise InvalidAppId(f"{app_id!r} is not lowercase")
-
-        if not rex.match(app_id) or app_id.endswith("-"):
-            raise InvalidAppId(f"{app_id!r} contains invalid characters")
-
-        source_def = parser[app_id]
-        res.append(SourceDef(app_id=app_id, **source_def))
-    return res
+class InvalidAppId(Exception):
+    """Invalid app-id for a app."""
 
 
 @dataclass
 class HostedApiDef:
     root_url: str
     api_url: str
     user: str
@@ -152,14 +141,15 @@
 
     def serves(self, api_def):
         return api_def.source_code_url.startswith(self.root_url)
 
     def get_current_rate_limit(self, requests):
         if self.root_url == "https://github.com":
             r = requests.get("https://api.github.com/rate_limit", auth=self.auth)
+            r.raise_for_status()
             cr = r.json()["resources"]["core"]
             return "gh api rate limits: {} out of {}, reset in {} secs".format(
                 cr["used"], cr["limit"], cr["reset"] - time.time()
             )
 
 
 @dataclass
@@ -206,15 +196,15 @@
         self.export_dir = basedir.joinpath(export_dir).absolute()
         self.cache_dir = basedir.joinpath(cache_dir).absolute()
         self.api_defs = api_defs
         self.source_defs = source_defs
 
     @property
     def app_index_path(self):
-        return self.xdcget_ini_path.parent.joinpath("sources.lock").absolute()
+        return self.xdcget_ini_path.parent.joinpath("xdcget.lock").absolute()
 
     def iter_xdc_sources(self):
         for source_def in self.source_defs:
             for api_def in self.api_defs:
                 if api_def.serves(source_def):
                     yield XDCSource(self.export_dir, source_def, api_def)
                     break
```

### Comparing `xdcget-0.2.3/src/xdcget/storage.py` & `xdcget-0.3.0/src/xdcget/storage.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-"""
-release caching and exporting of release files
-"""
-import os
+"""Release caching and exporting of release files."""
 import copy
 import shutil
-import toml
 from contextlib import contextmanager
 from dataclasses import dataclass
-from zipfile import ZipFile, ZIP_DEFLATED
+from zipfile import ZIP_DEFLATED, ZipFile
 
 import requests
+import toml
 
 
 def do_request(url, auth=None, exc=True):
     r = requests.get(url, auth=auth)
     if exc and not r.ok:
         r.raise_for_status()
     return r
@@ -52,219 +49,231 @@
 
     def download(self):
         r = do_request(self.url)
         r.raise_for_status()
         return r
 
 
-def perform_update(config, out):
-    for api_def in config.api_defs:
-        s = api_def.get_current_rate_limit(requests)
-        if s:
-            out(s)
+def perform_update(config, app_filter, out, offline):
+    """Update webxdcs.
+
+    Args:
+        config: configuration read from xdcget.ini
+        app_filter: if not None, only update the sources
+            whose app-id contains this string.
+        out: output printer
+        offline: if True, don't perform any network requests
+    """
+    if not offline:
+        for api_def in config.api_defs:
+            s = api_def.get_current_rate_limit(requests)
+            if s:
+                out(s)
 
-    retrieved = changed = num_all_problems = 0
+    retrieved = changed = checked = num_all_problems = 0
     config.cache_dir.mkdir(exist_ok=True, parents=True)
 
     with app_index_writer(config=config) as app_index:
         for xdc_source in config.iter_xdc_sources():
-            try:
-                remote_release = get_latest_remote_release(xdc_source)
-            except NoReleases as e:
-                out.red(f"NO RELEASES: {e.url}\n")
-                num_all_problems += 1
+            if app_filter and app_filter not in xdc_source.source_def.app_id:
                 continue
 
-            old_index_release = app_index.get_release(xdc_source.app_id)
-            index_release = app_index.set_release_from_remote(
-                xdc_source.app_id, remote_release
-            )
-            if old_index_release != index_release:
-                changed += 1
+            checked += 1
+            if offline:
+                index_release = app_index.get_release(xdc_source.app_id)
+                remote_release = index_release
+            else:
+                try:
+                    remote_release = get_latest_remote_release(xdc_source)
+                except NoReleases as e:
+                    out.red(f"NO RELEASES: {e.url}\n")
+                    num_all_problems += 1
+                    continue
+
+                old = app_index.get_release(xdc_source.app_id)
+                index_release = app_index.create_release_from_remote(
+                    xdc_source.app_id, remote_release
+                )
+                if getattr(old, "tag_name", None) != index_release.tag_name:
+                    changed += 1
 
             cache_path = config.cache_dir.joinpath(index_release.cache_relname)
             rel = index_release
             if True:
                 s = f"got release: [{rel.app_id}] "
                 s += " ".join([remote_release.name, rel.tag_name, rel.date])
                 out(s)
                 out(f"        url: {rel.url}")
             if cache_path.exists():
                 out(f"     cached: {cache_path}")
-            else:
+            elif not offline:
                 r = remote_release.download()
                 cache_path.write_bytes(r.content)
                 retrieved += 1
                 out(f"     stored: {cache_path}", green=True)
+            else:
+                out.red("skipping download action because of offline run")
+                out("")
+                continue
+
             for problem in check_xdc_consistency(cache_path, xdc_source):
                 out.red(problem)
                 num_all_problems += 1
+
+            manifest, _ = get_manifest_toml_and_icon(cache_path)
+            index_release.name = manifest["name"]
+            app_index.set_release(index_release)
             out("")
 
-        out.green(
-            f"{app_index.get_num_apps()} apps checked from {config.app_index_path}"
-        )
+        out.green(f"{checked} apps checked from {config.app_index_path}")
         out.green(f"{changed} apps had newer versions")
         out.green(f"{retrieved} '.xdc' release files retrieved")
         if num_all_problems > 0:
             out.red(f"{num_all_problems} problems found")
         else:
             out.green("all good, no problems detected in .xdc files")
 
 
 def check_xdc_consistency(xdc_path, xdc_source):
+    """Check .xdc file. Yields found problems if any.
+
+    Args:
+        xdc_path: path to the .xdc file.
+        xdc_source: corresponding part of the xdcget.ini source configuration file.
+    """
     MAX_SUMMARY_CHARS = 30
     MIN_DETAILS_CHARS = 40
 
+    manifest, icon_found = get_manifest_toml_and_icon(xdc_path)
+    manifest_sc = manifest.get("source_code_url")
+    if manifest_sc:
+        sc = xdc_source.source_def.source_code_url
+        if sc != manifest_sc:
+            yield f"warn: manifest {manifest_sc} != {sc}"
+    description = xdc_source.description
+    if not description:
+        yield "error: 'description' field not in xdcget.ini"
+    else:
+        lines = description.strip().split("\n")
+        if len(lines[0]) > MAX_SUMMARY_CHARS:
+            extra = len(lines[0]) - MAX_SUMMARY_CHARS
+            yield f"error: description summary {extra} chars too much"
+        if lines[0][-1:] == ".":
+            yield "error: description summary ends with '.'"
+        if len(lines) < 2:
+            yield "error: description misses detail lines"
+        else:
+            joint = " ".join(lines[1:])
+            if len(joint) < MIN_DETAILS_CHARS:
+                yield "error: description details have less than 40 chars"
+
+    if "app_id" in manifest:
+        yield f"error: manifest has app_id {manifest['app_id']}, ignoring"
+    if "version" in manifest:
+        yield "error: manifest has 'version', ignoring"
+    if not icon_found:
+        yield "error: no 'icon.png' or 'icon.jpg' in .xdc file"
+
+
+def get_manifest_toml_and_icon(xdc_path):
+    """Extract manifest.toml from .xdc and check if it contains an icon."""
     zf = ZipFile(xdc_path)
-    icon_found = False
+    icon_found = manifest = None
     for fname in zf.namelist():
         if fname.lower().endswith("manifest.toml"):
             content = zf.read(fname)
             manifest = toml.loads(content.decode("utf-8"))
-            manifest_sc = manifest.get("source_code_url")
-            if manifest_sc:
-                sc = xdc_source.source_def.source_code_url
-                if sc != manifest_sc:
-                    yield f"warn: manifest {manifest_sc} != {sc}"
-            description = xdc_source.description
-            if not description:
-                yield "error: 'description' field not in sources.ini"
-            else:
-                lines = description.strip().split("\n")
-                if len(lines[0]) > MAX_SUMMARY_CHARS:
-                    extra = len(lines[0]) - MAX_SUMMARY_CHARS
-                    yield f"error: description summary {extra} chars too much"
-                if lines[0][-1:] == ".":
-                    yield "error: description summary ends with '.'"
-                if len(lines) < 2:
-                    yield "error: description misses detail lines"
-                else:
-                    joint = " ".join(lines[1:])
-                    if len(joint) < MIN_DETAILS_CHARS:
-                        yield "error: description details have less than 40 chars"
-
-            if "app_id" in manifest:
-                yield f"error: manifest has app_id {manifest['app_id']}, ignoring"
-            if "version" in manifest:
-                yield "error: manifest has 'version', ignoring"
         elif fname.lower() in ("icon.png", "icon.jpg"):
             icon_found = True
 
-    if not icon_found:
-        yield "error: no 'icon.png' or 'icon.jpg' in .xdc file"
-
-
-def perform_status(config, out):
-    app_index = get_app_index(config)
-
-    num_releases = num_cached = 0
-    for index_release in app_index.iter_releases():
-        ver = index_release.version
-        tag = index_release.tag_name
-        date = index_release.date
-        out(f"[{index_release.app_id}] version={ver} tag={tag} date={date}")
-        out(f"url={index_release.url}")
-        cache_path = config.cache_dir.joinpath(index_release.cache_relname)
-        if cache_path.exists():
-            num_cached += 1
-            out(f"cached at: {cache_path}")
-        else:
-            out(f"not cached: {cache_path}", red=True)
-        out("")
-        num_releases += 1
-
-    if num_releases == 0:
-        out.red("app_index is empty: initial 'update' is needed")
-        raise SystemExit(1)
-
-    out.green(f"{num_releases} apps found in index at {config.app_index_path}")
-    out.green(f"{num_cached} apps are cached in {config.cache_dir}")
+    return manifest, icon_found
 
 
 class IndexRelease:
     def __init__(
         self,
         app_id,
-        version,
         tag_name,
         url,
         date,
         description,
         source_code_url="",
+        name="",
     ):
         self.app_id = app_id
-        self.version = version
         self.tag_name = tag_name
         self.url = url
         self.date = date
         self.cache_relname = f"{app_id}-{tag_name}.xdc"
         self.description = description
         self.source_code_url = source_code_url
+        self.name = name
 
     def __eq__(self, other):
         return self.__dict__ == getattr(other, "__dict__", None)
 
     def toml_data(self):
-        return self.__dict__.copy()
+        return dict(
+            app_id=self.app_id,
+            name=self.name,
+            tag_name=self.tag_name,
+            url=self.url,
+            date=self.date,
+            cache_relname=f"{self.app_id}-{self.tag_name}.xdc",
+            description=self.description,
+            source_code_url=self.source_code_url,
+        )
 
 
 class AppIndex:
+    """Application index."""
+
     def __init__(self, data, config):
-        self._data = data
-        self.config = config
+        self._data = data  # Contents of the xdcget.lock file
+        self.config = config  # Contents of the xdcget.ini file
 
     def get_num_apps(self):
+        """Return number of applications in the index."""
         return len(self._data)
 
-    def _set_release(self, index_release: IndexRelease):
+    def set_release(self, index_release: IndexRelease):
         assert "." not in index_release.app_id
+        assert index_release.name, "name attribute can not be empty"
         self._data[index_release.app_id] = index_release.toml_data()
 
-    def set_release_from_remote(self, app_id, remote_release):
-        cur = self.get_release(app_id)
+    def create_release_from_remote(self, app_id, remote_release):
         rel = remote_release
-        version = 1
-        if cur is not None:
-            # if a different release is available, increment version
-            if cur.url == rel.url and cur.tag_name == rel.tag_name:
-                version = cur.version
-            else:
-                version = cur.version + 1
-
         source = self.config.get_xdc_source(app_id)
-        index_release = IndexRelease(
+        return IndexRelease(
             app_id=app_id,
-            version=version,
             tag_name=rel.tag_name,
             url=rel.url,
             date=remote_release.date,
             description=source.description,
             source_code_url=source.source_def.source_code_url,
         )
-        self._set_release(index_release)
-        return index_release
 
     def get_release(self, app_id):
         release = self._data.get(app_id)
         if release is not None:
             assert app_id == release["app_id"]
             if "cache_relname" in release:
                 del release["cache_relname"]
             return IndexRelease(**release)
 
-    def get_next_release_version(self, app_id):
-        rel = self.get_release(app_id)
-        return (rel.version + 1) if rel else 1
-
     def iter_releases(self):
         return (self.get_release(app_id) for app_id in self._data)
 
 
 def get_app_index(config):
+    """Read the application index.
+
+    Args:
+        config: contents of the xdcget.ini configuration file.
+    """
     if config.app_index_path.exists():
         with config.app_index_path.open("r") as f:
             lock_data = toml.load(f)
     else:
         lock_data = {}
     return AppIndex(lock_data, config)
 
@@ -274,61 +283,67 @@
     path = config.app_index_path
     if path.exists():
         with path.open("r") as f:
             lock_data = toml.load(f)
     else:
         lock_data = {}
     new_data = copy.deepcopy(lock_data)
+
+    # prune apps from the index not defined in our app sources list
+    for app_id in set(new_data) - set(x.app_id for x in config.source_defs):
+        del new_data[app_id]
+
     app_index = AppIndex(new_data, config=config)
 
     yield app_index
 
     if new_data != lock_data:
         tmp = path.parent.joinpath(path.name + ".tmp")
         with tmp.open("w") as f:
             toml.dump(new_data, f)
-        os.rename(tmp, path)
+        tmp.rename(path)
 
 
-def perform_export(config, out):
-    config.export_dir.mkdir(exist_ok=True, parents=True)
+def perform_export(config, out, offline):
+    if config.export_dir.exists():
+        shutil.rmtree(config.export_dir)
+
+    config.export_dir.mkdir()
     app_index = get_app_index(config)
     num = 0
     for index_release in app_index.iter_releases():
-        path = export_to_xdcstore(config, index_release)
-        out(f"exported: {path}")
-        out(f"          app_id={index_release.app_id} version={index_release.version}")
+        export_to_xdcstore(config, index_release)
         num += 1
 
     if num == 0:
-        out.red("No apps to export, did you run 'update' first?")
+        out.red("No apps to export, probably a configuration error?")
         raise SystemExit(1)
+
     dest = config.export_dir.joinpath(config.app_index_path.name)
     shutil.copy(config.app_index_path, dest)
-    out.green(f"Exported store metadata for {num} apps to {dest})")
+    out.green(f"Exported store metadata for {num} apps to {dest}")
+    out.green(f"Exported {num} webxdc release files to {dest.parent}")
 
 
 def export_to_xdcstore(config, index_release):
-    # XXX needs more tests -- better at unit test level, avoiding network-IO
     cache_path = config.cache_dir.joinpath(index_release.cache_relname)
-    xdc_source = config.get_xdc_source(index_release.app_id)
-    assert xdc_source is not None, index_release.app_id
-    zf = ZipFile(cache_path)
     new_zf_path = config.export_dir.joinpath(index_release.cache_relname)
+    # note that the original asset might use a different compression
+    # method but we will write it out with standard ZIP_DEFLATED
+    # because that's the only method that Delta Chat core supports as of 1.117.0
+    zf = ZipFile(cache_path)
     new_zf = ZipFile(new_zf_path.open("wb"), compression=ZIP_DEFLATED, mode="w")
     for fname in zf.namelist():
         content = zf.read(fname)
         if fname == "manifest.toml":
             manifest = toml.loads(content.decode("utf-8"))
-            manifest["app_id"] = index_release.app_id
-            manifest["version"] = index_release.version
-            manifest["date"] = index_release.date
-            manifest["description"] = xdc_source.description
-            # override possibly wrong source_code_urls
-            # we know exactly where we are getting the source from
-            # so let's just use it.
+            # we know exactly where we were getting the source asset from
+            # so it's a better source than what was manually specified
             manifest["source_code_url"] = index_release.source_code_url
-
+            # put the "tag_name" into the produced manifest so that
+            # together with the source_code_url we have a somewhat precise
+            # reference for any ".xdc" file the store hands out
+            manifest["tag_name"] = index_release.tag_name
             content = toml.dumps(manifest).encode("utf-8")
         new_zf.writestr(fname, data=content)
     new_zf.close()
     return new_zf_path
```

### Comparing `xdcget-0.2.3/src/xdcget.egg-info/PKG-INFO` & `xdcget-0.3.0/src/xdcget.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,93 +1,110 @@
 Metadata-Version: 2.1
 Name: xdcget
-Version: 0.2.3
+Version: 0.3.0
 Summary: experimental tool for collecting latest releases of webxdc apps
 License: MPL-2.0
 Project-URL: homepage, https://codeberg.org/webxdc/xdcget
 Project-URL: issues, https://codeberg.org/webxdc/xdcget/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: POSIX
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: test
+License-File: LICENSE
 
 
 # xdcget: a command line tool to collect webxdc apps from git repositories 
 
-The "xdcget" command line tool collects [WebXDC](https://webxdc.org) apps
-via the release API of Codeberg and Github.
 The main purpose for this tool is to maintain a cache of released webxdc apps
 and to export release files so they can be imported from the 
-[WebXDC Store](https://github.com/webxdc/store)
-which in turn can be used by Delta Chat users to discover webxdc apps for sharing in chats. 
+[xdcstore bot](https://github.com/webxdc/store)
+which in turn can be contacted by Delta Chat users 
+in order to be able to search and share webxdc apps in chats. 
 
 ## Getting started  
 
 1. Install `xdcget` command line tool from a local checkout:
 
         pip install -e . 
 
 2. Initialize config files: 
 
         xdcget init 
 
-3. Edit `xdcget.ini` to contain your Codeberg and Github API access token (see below)
-   and also adjust config options as needed.  
+3. Edit `xdcget.ini` and make sure that you set environment variables 
+   containing your credentials for Codeberg/Github API usage. 
+   See below for how to get API credentials. 
 
-4. Edit `sources.ini` to modify the list of source repositories. 
-
-5. Run the `update` command to cache all releases for 
-   repositories listed in `sources.ini`:
+4. Run the `update` command to retrieve newest webxdc app releases 
+   for repositories listed in `xdcget.ini` and export them to the `export` directory: 
 
         xdcget update 
 
-6. Run the `export` command to create files for `xdcstore import <PATH>`
-
-        xdcget export 
 
 ## Getting a Codeberg API access token 
 
 Login with Codeberg and open https://codeberg.org/user/settings/applications 
 to generate a new token.  This token does not need any special "scopes"
-it's only used for querying releases of public repositories.  
+it's only used for querying releases of public repositories.
 You can copy the resulting API token into your clipboard
-and then insert it into the config file: 
-
-    # the line you need to put into `xdcget.ini` 
-    CODEBERG_USER = <your-codeberg-user-name> 
-    CODEBERG_TOKEN = <paste-your-codeberg-access-token-here> 
+and then set it into the environment variables you declared in the config file:
 
+    # bash example
+    export XDCGET_CODEBERG_USER=<your-codeberg-user-name>
+    export XDCGET_CODEBERG_TOKEN=<paste-your-codeberg-access-token-here>
 
 ## Getting a Github API access token 
 
 Login with github and open https://github.com/settings/tokens
 to generate a new token.  This token does not need any access
 to your private repos -- it's only used for querying releases 
 of public repositories.  You may give it 90 days or other expiration
 times as you feel fine with. 
 You can copy the resulting API token into your clipboard
-and then insert it into the config file: 
+and then set it into the environment variables you declared in the config file:
+
+    # bash example
+    export XDCGET_GITHUB_USER=<your-github-user-name>
+    export XDCGET_GITHUB_TOKEN=<paste-your-github-access-token-here>
+
+## Contributing
+
+Install tox:
 
-    # the line you need to put into `xdcget.ini` 
-    GITHUB_USER = <your-github-user-name> 
-    GITHUB_TOKEN = <paste-your-github-access-token-here> 
+```
+pip install tox
+```
 
+We use [black](https://github.com/psf/black) to format the code and [ruff](https://beta.ruff.rs/docs) as linter. After modifying the code, run:
 
-## Building and publishing xdcget releases (maintainer notes)
+```
+tox -e lint
+```
 
-This project uses a single `pyproject.toml` to define all python build/test metadata.
-See [Packaging Python Projects](https://packaging.python.org/en/latest/tutorials/packaging-projects/?highlight=pyproject.toml) for more details. 
+Run automated tests with:
 
-Quick notes on requirements for releasing: 
+```
+tox
+```
 
-- `pip install build twine` for building and uploading distribution files 
+**IMPORTANT:** Pull Requests with new features / bug fixes should come with automated tests.
+
+### Building and publishing xdcget releases
+
+Quick notes on requirements for testing and releasing: 
+
+- `pip install tox build twine` to install development dependencies
+
+- `tox` to run tests
 
 - `python -m build` to build the distribution files
 
 - [create API-tokens on PyPI](https://pypi.org/manage/account/)
   to be able to upload to PyPI repositories. 
 
-- `twine upload dist/*` to upload all built distribution files 
+- Use git to tag a release before uploading (e.g. "git tag" and "git push --tags") 
+  The version of xdcget (also obtained via `xdcget --version`) is dynamically 
+  computed using [setuptools-scm](https://pypi.org/project/setuptools-scm/)
 
+- `twine upload dist/*` to upload all built distribution files
```

### Comparing `xdcget-0.2.3/tests/test_storage.py` & `xdcget-0.3.0/tests/test_storage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,77 +1,76 @@
 import pytest
-
-from xdcget.config import XDCSource, SourceDef
-from xdcget.storage import (
-    get_latest_remote_release,
-    app_index_writer,
-    RemoteRelease,
-)
+from xdcget.config import SourceDef, XDCSource
+from xdcget.storage import RemoteRelease, app_index_writer, get_latest_remote_release
 
 
 class TestAppIndex:
     @pytest.fixture
     def pseudo_Config(self):
         class Config:
-            def __init__(self, path):
+            def __init__(self, path, app_ids=[]):
                 self.app_index_path = path
+                self.app_ids = app_ids
+                self.source_defs = []
 
             def get_xdc_source(self, app_id):
                 return XDCSource("", SourceDef("hello", "", ""), None)
 
         return Config
 
     def test_write_one(self, tmp_path, pseudo_Config):
         path = tmp_path.joinpath("test.lock")
         remote_release = RemoteRelease("hello", "0.1.0", "https://a.org", "DATE")
 
         config = pseudo_Config(path)
         with app_index_writer(config) as app_index:
-            app_index.set_release_from_remote("webxdc-hello", remote_release)
+            ir = app_index.create_release_from_remote("webxdc-hello", remote_release)
+            ir.name = "hello"
+            app_index.set_release(ir)
 
         assert app_index.get_release(app_id="xzy") is None
         assert app_index.get_num_apps() == 1
         release = app_index.get_release(app_id="webxdc-hello")
         assert release.url == remote_release.url
         assert release.tag_name == remote_release.tag_name
-        assert release.version == 1
+        assert release.name == "hello"
         assert release.cache_relname == "webxdc-hello-0.1.0.xdc"
-
         assert release == app_index.get_release(app_id="webxdc-hello")
 
-        app_index._set_release(release)
+        app_index.set_release(release)
         release2 = app_index.get_release("webxdc-hello")
         assert release2.cache_relname == release.cache_relname
-        assert release2.version == release.version
+        assert release2.tag_name == release.tag_name
 
     def test_write_three(self, tmp_path, pseudo_Config):
         path = tmp_path.joinpath("test.lock")
         config = pseudo_Config(path)
         with app_index_writer(config) as app_index:
             for num in range(4):
                 rel = RemoteRelease("hello", f"0.{num}.0", "https://a.org", "DATE")
-                app_index.set_release_from_remote("webxdc-hello", rel)
+                ir = app_index.create_release_from_remote("webxdc-hello", rel)
+                ir.name = "hello"
+                app_index.set_release(ir)
 
         index_rel = app_index.get_release("webxdc-hello")
-        assert index_rel.version == 4
         assert index_rel.tag_name == "0.3.0"
         assert index_rel.url == "https://a.org"
 
         rel = RemoteRelease("hello", index_rel.tag_name, index_rel.url, "DATE")
-        index_release = app_index.set_release_from_remote(index_rel.app_id, rel)
-        assert index_release.version == 4
+        index_release = app_index.create_release_from_remote(index_rel.app_id, rel)
+        assert index_release.tag_name == index_rel.tag_name
 
 
 def test_get_latest_remote_release(config_example1):
     xdc1, xdc2 = config_example1.iter_xdc_sources()
 
     rel = get_latest_remote_release(xdc1)
     assert rel.name == "checklist.xdc"
-    assert rel.tag_name.startswith("0.")
+    assert rel.tag_name
     assert rel.url
     assert rel.date
 
     rel = get_latest_remote_release(xdc2)
     assert rel.name == "poll.xdc"
-    assert rel.tag_name.startswith("v1.")
+    assert rel.tag_name
     assert rel.url
     assert rel.date
```

