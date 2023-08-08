# Comparing `tmp/anonfile-0.2.7.tar.gz` & `tmp/anonfile-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/anonfile-0.2.7.tar", last modified: Sun Sep 12 19:49:09 2021, max compression
+gzip compressed data, was "anonfile-1.0.0.tar", last modified: Tue Aug  8 13:13:47 2023, max compression
```

## Comparing `anonfile-0.2.7.tar` & `anonfile-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-12 19:49:09.000000 anonfile-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (121)     6528 2021-09-12 19:49:09.000000 anonfile-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4419 2021-09-12 19:48:54.000000 anonfile-0.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-12 19:49:09.000000 anonfile-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2592 2021-09-12 19:48:54.000000 anonfile-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-12 19:49:09.000000 anonfile-0.2.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-12 19:49:09.000000 anonfile-0.2.7/src/anonfile/
--rw-r--r--   0 runner    (1001) docker     (121)     6557 2021-09-12 19:48:54.000000 anonfile-0.2.7/src/anonfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13104 2021-09-12 19:48:54.000000 anonfile-0.2.7/src/anonfile/anonfile.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-12 19:49:09.000000 anonfile-0.2.7/src/anonfile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6528 2021-09-12 19:49:09.000000 anonfile-0.2.7/src/anonfile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      286 2021-09-12 19:49:09.000000 anonfile-0.2.7/src/anonfile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-12 19:49:09.000000 anonfile-0.2.7/src/anonfile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2021-09-12 19:49:09.000000 anonfile-0.2.7/src/anonfile.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-09-12 19:49:09.000000 anonfile-0.2.7/src/anonfile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-09-12 19:49:09.000000 anonfile-0.2.7/src/anonfile.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:13:47.878616 anonfile-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-08-08 13:13:31.000000 anonfile-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-08 13:13:31.000000 anonfile-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-08-08 13:13:47.878616 anonfile-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-08-08 13:13:31.000000 anonfile-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:13:47.878616 anonfile-1.0.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-08 13:13:31.000000 anonfile-1.0.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-08 13:13:31.000000 anonfile-1.0.0/requirements/release.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 13:13:47.878616 anonfile-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-08-08 13:13:31.000000 anonfile-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:13:47.878616 anonfile-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:13:47.878616 anonfile-1.0.0/src/anonfile/
+-rw-r--r--   0 runner    (1001) docker     (123)     6793 2023-08-08 13:13:31.000000 anonfile-1.0.0/src/anonfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-08-08 13:13:31.000000 anonfile-1.0.0/src/anonfile/anonfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:13:47.878616 anonfile-1.0.0/src/anonfile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-08-08 13:13:47.000000 anonfile-1.0.0/src/anonfile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-08 13:13:47.000000 anonfile-1.0.0/src/anonfile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 13:13:47.000000 anonfile-1.0.0/src/anonfile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-08 13:13:47.000000 anonfile-1.0.0/src/anonfile.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-08 13:13:47.000000 anonfile-1.0.0/src/anonfile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-08 13:13:47.000000 anonfile-1.0.0/src/anonfile.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `anonfile-0.2.7/PKG-INFO` & `anonfile-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anonfile
-Version: 0.2.7
+Version: 1.0.0
 Summary: An unofficial library that wraps the anonfile.com REST API.
 Home-page: https://github.com/nstrydom2/anonfile-api
 Author: Nicholas Strydom
 Author-email: nstrydom@gmail.com
 License: UNKNOWN
 Project-URL: Source Code, https://github.com/nstrydom2/anonfile-api
 Project-URL: Bug Reports, https://github.com/nstrydom2/anonfile-api/issues
@@ -21,44 +21,49 @@
         [![CI](https://github.com/nstrydom2/anonfile-api/actions/workflows/python-package.yml/badge.svg?branch=master)](https://github.com/nstrydom2/anonfile-api/actions/workflows/python-package.yml)
         [![PyPI download total](https://img.shields.io/pypi/dm/anonfile)](https://pypi.python.org/pypi/anonfile/)
         [![PyPI pyversions](https://img.shields.io/pypi/pyversions/anonfile)](https://pypi.python.org/pypi/anonfile/)
         [![PyPI license](https://img.shields.io/pypi/l/anonfile)](https://pypi.python.org/pypi/anonfile/)
         
         
         This unofficial Python API was created to make uploading and downloading files
-        from <anonfiles.com> simple and effective for programming in Python. The goal of
+        from https://anonfiles.com simple and effective for programming in Python. The goal of
         the project is to create an intuitive library for anonymous file sharing.
         
         ## Getting Started
         
         These instructions will get you a copy of the project up and running on your local
         machine for development and testing purposes. See deployment for notes on how to
         deploy the project on a live system.
         
         ### Prerequisites
         
-        Python 3.7+ is required to run this application, other than that there are no
+        Python 3.8+ is required to run this application, other than that there are no
         prerequisites for the project, as the dependencies are included in the repository.
         
         ### Installing
         
         To install the library is as simple as running
         
         ```bash
         pip install anonfile
         ```
         
-        from the command line. To install this library in debug mode, use
+        from the command line. To install this library in debug mode with dev dependencies, use
         
         ```bash
-        pip install -e .
+        pip install -e .[dev]
         ```
         
         instead. It is recommended to create an virtual environment prior
-        to installing this library.
+        to installing this library. If you only intend to use this library from the CLI,
+        use [pipx](https://pypa.github.io/pipx/) for the installation instead:
+        
+        ```bash
+        pipx install anonfile
+        ```
         
         ### Dev Notes
         
         Run unit tests locally:
         
         ```bash
         pytest --verbose -s [--token "REDACTED"]
@@ -74,23 +79,23 @@
         files is made accessible to any user that [signs into your account](https://anonfiles.com/login).
         
         ```python
         from anonfile import AnonFile
         
         anon = AnonFile()
         
-        # upload a file and enable progressbar terminal feedback
+        # upload a file and enable progressbar terminal feedback (off by default)
         upload = anon.upload('/home/guest/jims_paperwork.doc', progressbar=True)
         print(upload.url.geturl())
         
         # download a file and set the download directory
         from pathlib import Path
         target_dir = Path.home().joinpath('Downloads')
-        filename = anon.download("https://anonfiles.com/9ee1jcu6u9/test_txt", path=target_dir)
-        print(filename)
+        download = anon.download("https://anonfiles.com/9ee1jcu6u9/test_txt", path=target_dir)
+        print(download.file_path)
         ```
         
         And voilà, pain-free anonymous file sharing. If you want more information about
         the `AnonFile` API visit [anonfiles.com](https://anonfiles.com/docs/api).
         
         ## Command Line Interface
         
@@ -116,14 +121,15 @@
         
         ## Authors
         
         | Name             | Mail Address                | GitHub Profile                                |
         |------------------|-----------------------------|-----------------------------------------------|
         | Nicholas Strydom | nstrydom@gmail.com          | [nstrydom2](https://github.com/nstrydom2)     |
         | hentai-chan      | dev.hentai-chan@outlook.com | [hentai-chan](https://github.com/hentai-chan) |
+        | Stefan Greve     | greve.stefan@outlook.jp     | [StefanGreve](https://github.com/stefangreve) |
         
         See also the list of [contributors](https://github.com/nstrydom2/anonfile-api/contributors)
         who participated in this project.
         
         ## License
         
         This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for more details.
@@ -136,19 +142,20 @@
         * My Dad
         * Hat tip to anyone whose code was used
         * Inspiration
         * etc
         
 Keywords: anonfile rest api
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: anonfile Version: 0.2.7 Summary: An unofficial
+Metadata-Version: 2.1 Name: anonfile Version: 1.0.0 Summary: An unofficial
 library that wraps the anonfile.com REST API. Home-page: https://github.com/
 nstrydom2/anonfile-api Author: Nicholas Strydom Author-email:
 nstrydom@gmail.com License: UNKNOWN Project-URL: Source Code, https://
 github.com/nstrydom2/anonfile-api Project-URL: Bug Reports, https://github.com/
 nstrydom2/anonfile-api/issues Project-URL: Changelog, https://github.com/
 nstrydom2/anonfile-api/blob/master/CHANGELOG.md Description:
   [https://raw.githubusercontent.com/nstrydom2/anonfile-api/master/logo.svg]
@@ -11,59 +11,64 @@
 (https://github.com/nstrydom2/anonfile-api/actions/workflows/python-
 package.yml/badge.svg?branch=master)](https://github.com/nstrydom2/anonfile-
 api/actions/workflows/python-package.yml) [![PyPI download total](https://
 img.shields.io/pypi/dm/anonfile)](https://pypi.python.org/pypi/anonfile/) [!
 [PyPI pyversions](https://img.shields.io/pypi/pyversions/anonfile)](https://
 pypi.python.org/pypi/anonfile/) [![PyPI license](https://img.shields.io/pypi/l/
 anonfile)](https://pypi.python.org/pypi/anonfile/) This unofficial Python API
-was created to make uploading and downloading files from
-com> simple and effective for programming in Python. The goal of the project is
-to create an intuitive library for anonymous file sharing. ## Getting Started
+was created to make uploading and downloading files from https://anonfiles.com
+simple and effective for programming in Python. The goal of the project is to
+create an intuitive library for anonymous file sharing. ## Getting Started
 These instructions will get you a copy of the project up and running on your
 local machine for development and testing purposes. See deployment for notes on
-how to deploy the project on a live system. ### Prerequisites Python 3.7+ is
+how to deploy the project on a live system. ### Prerequisites Python 3.8+ is
 required to run this application, other than that there are no prerequisites
 for the project, as the dependencies are included in the repository. ###
 Installing To install the library is as simple as running ```bash pip install
-anonfile ``` from the command line. To install this library in debug mode, use
-```bash pip install -e . ``` instead. It is recommended to create an virtual
-environment prior to installing this library. ### Dev Notes Run unit tests
-locally: ```bash pytest --verbose -s [--token "REDACTED"] ``` Add the `-
-k test_*` option if you want to test only a single function. ## Usage Import
-the module and instantiate the `AnonFile()` constructor. Setting the download
-directory in `path` is optional. Using the API `token` in the constructor is
-optional as well. A valid `token` registers all file uploads online, i.e. a
-list of all uploaded files is made accessible to any user that [signs into your
-account](https://anonfiles.com/login). ```python from anonfile import AnonFile
-anon = AnonFile() # upload a file and enable progressbar terminal feedback
-upload = anon.upload('/home/guest/jims_paperwork.doc', progressbar=True) print
-(upload.url.geturl()) # download a file and set the download directory from
-pathlib import Path target_dir = Path.home().joinpath('Downloads') filename =
-anon.download("https://anonfiles.com/9ee1jcu6u9/test_txt", path=target_dir)
-print(filename) ``` And voilÃ , pain-free anonymous file sharing. If you want
-more information about the `AnonFile` API visit [anonfiles.com](https://
+anonfile ``` from the command line. To install this library in debug mode with
+dev dependencies, use ```bash pip install -e .[dev] ``` instead. It is
+recommended to create an virtual environment prior to installing this library.
+If you only intend to use this library from the CLI, use [pipx](https://
+pypa.github.io/pipx/) for the installation instead: ```bash pipx install
+anonfile ``` ### Dev Notes Run unit tests locally: ```bash pytest --verbose -s
+[--token "REDACTED"] ``` Add the `-k test_*` option if you want to test only a
+single function. ## Usage Import the module and instantiate the `AnonFile()`
+constructor. Setting the download directory in `path` is optional. Using the
+API `token` in the constructor is optional as well. A valid `token` registers
+all file uploads online, i.e. a list of all uploaded files is made accessible
+to any user that [signs into your account](https://anonfiles.com/login).
+```python from anonfile import AnonFile anon = AnonFile() # upload a file and
+enable progressbar terminal feedback (off by default) upload = anon.upload('/
+home/guest/jims_paperwork.doc', progressbar=True) print(upload.url.geturl()) #
+download a file and set the download directory from pathlib import Path
+target_dir = Path.home().joinpath('Downloads') download = anon.download("https:
+//anonfiles.com/9ee1jcu6u9/test_txt", path=target_dir) print
+(download.file_path) ``` And voilÃ , pain-free anonymous file sharing. If you
+want more information about the `AnonFile` API visit [anonfiles.com](https://
 anonfiles.com/docs/api). ## Command Line Interface ```bash # open help page for
 specific commands anonfile [download|upload|preview|log] --help # note: both
 methods expect at least one argument, but can take on more anonfile download --
 url https://anonfiles.com/93k5x1ucu0/test_txt anonfile upload --file ./test.txt
 ``` ## Built With * [Requests](http://docs.python-requests.org/en/master/) -
 Http for Humans * [TQDM](https://github.com/tqdm/tqdm) - Fast & Extensible
 Progress Bars * [anonfiles.com](https://anonfiles.com/docs/api) - AnonFiles.com
 REST API ## Versioning Navigate to [tags on this repository](https://
 github.com/nstrydom2/anonfile-api/tags) to see all available versions. ##
 Authors | Name | Mail Address | GitHub Profile | |------------------|----------
 -------------------|-----------------------------------------------| | Nicholas
 Strydom | nstrydom@gmail.com | [nstrydom2](https://github.com/nstrydom2) | |
 hentai-chan | dev.hentai-chan@outlook.com | [hentai-chan](https://github.com/
-hentai-chan) | See also the list of [contributors](https://github.com/
-nstrydom2/anonfile-api/contributors) who participated in this project. ##
-License This project is licensed under the MIT License - see the [LICENSE]
-(LICENSE) file for more details. ## Acknowledgments * Joseph Marie Jacquard *
-Charles Babbage * Ada Lovelace * My Dad * Hat tip to anyone whose code was used
-* Inspiration * etc Keywords: anonfile rest api Platform: UNKNOWN Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Intended Audience :: Developers Classifier: Natural Language :: English
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content Classifier: Topic
-:: Software Development :: Libraries Classifier: Topic :: Utilities Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
+hentai-chan) | | Stefan Greve | greve.stefan@outlook.jp | [StefanGreve](https:/
+/github.com/stefangreve) | See also the list of [contributors](https://
+github.com/nstrydom2/anonfile-api/contributors) who participated in this
+project. ## License This project is licensed under the MIT License - see the
+[LICENSE](LICENSE) file for more details. ## Acknowledgments * Joseph Marie
+Jacquard * Charles Babbage * Ada Lovelace * My Dad * Hat tip to anyone whose
+code was used * Inspiration * etc Keywords: anonfile rest api Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Intended
+Audience :: Developers Classifier: Natural Language :: English Classifier:
+Topic :: Internet :: WWW/HTTP :: Dynamic Content Classifier: Topic :: Software
+Development :: Libraries Classifier: Topic :: Utilities Classifier: License ::
+OSI Approved :: MIT License Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8 Description-Content-Type: text/markdown
```

### Comparing `anonfile-0.2.7/README.md` & `anonfile-1.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,128 +1,134 @@
-<p align="center">
-  <a href="https://github.com/nstrydom2/anonfile-api" title="Project Logo">
-    <img height="150" style="margin-top:15px" src="https://raw.githubusercontent.com/nstrydom2/anonfile-api/master/logo.svg">
-  </a>
-</p>
-
-# Anonfiles.com Unofficial Python API
-
-[![PyPI version shields.io](https://img.shields.io/pypi/v/anonfile)](https://pypi.python.org/pypi/anonfile/)
-[![CI](https://github.com/nstrydom2/anonfile-api/actions/workflows/python-package.yml/badge.svg?branch=master)](https://github.com/nstrydom2/anonfile-api/actions/workflows/python-package.yml)
-[![PyPI download total](https://img.shields.io/pypi/dm/anonfile)](https://pypi.python.org/pypi/anonfile/)
-[![PyPI pyversions](https://img.shields.io/pypi/pyversions/anonfile)](https://pypi.python.org/pypi/anonfile/)
-[![PyPI license](https://img.shields.io/pypi/l/anonfile)](https://pypi.python.org/pypi/anonfile/)
-
-
-This unofficial Python API was created to make uploading and downloading files
-from <anonfiles.com> simple and effective for programming in Python. The goal of
-the project is to create an intuitive library for anonymous file sharing.
-
-## Getting Started
-
-These instructions will get you a copy of the project up and running on your local
-machine for development and testing purposes. See deployment for notes on how to
-deploy the project on a live system.
-
-### Prerequisites
-
-Python 3.7+ is required to run this application, other than that there are no
-prerequisites for the project, as the dependencies are included in the repository.
-
-### Installing
-
-To install the library is as simple as running
-
-```bash
-pip install anonfile
-```
-
-from the command line. To install this library in debug mode, use
-
-```bash
-pip install -e .
-```
-
-instead. It is recommended to create an virtual environment prior
-to installing this library.
-
-### Dev Notes
-
-Run unit tests locally:
-
-```bash
-pytest --verbose -s [--token "REDACTED"]
-```
-
-Add the `-k test_*` option if you want to test only a single function.
-
-## Usage
-
-Import the module and instantiate the `AnonFile()` constructor. Setting the download
-directory in `path` is optional. Using the API `token` in the constructor is optional
-as well. A valid `token` registers all file uploads online, i.e. a list of all uploaded
-files is made accessible to any user that [signs into your account](https://anonfiles.com/login).
-
-```python
-from anonfile import AnonFile
-
-anon = AnonFile()
-
-# upload a file and enable progressbar terminal feedback
-upload = anon.upload('/home/guest/jims_paperwork.doc', progressbar=True)
-print(upload.url.geturl())
-
-# download a file and set the download directory
-from pathlib import Path
-target_dir = Path.home().joinpath('Downloads')
-filename = anon.download("https://anonfiles.com/9ee1jcu6u9/test_txt", path=target_dir)
-print(filename)
-```
-
-And voilà, pain-free anonymous file sharing. If you want more information about
-the `AnonFile` API visit [anonfiles.com](https://anonfiles.com/docs/api).
-
-## Command Line Interface
-
-```bash
-# open help page for specific commands
-anonfile [download|upload|preview|log] --help
-
-# note: both methods expect at least one argument, but can take on more
-anonfile download --url https://anonfiles.com/93k5x1ucu0/test_txt
-anonfile upload --file ./test.txt
-```
-
-## Built With
-
-* [Requests](http://docs.python-requests.org/en/master/) - Http for Humans
-* [TQDM](https://github.com/tqdm/tqdm) - Fast & Extensible Progress Bars
-* [anonfiles.com](https://anonfiles.com/docs/api) - AnonFiles.com REST API
-
-## Versioning
-
-Navigate to [tags on this repository](https://github.com/nstrydom2/anonfile-api/tags)
-to see all available versions.
-
-## Authors
-
-| Name             | Mail Address                | GitHub Profile                                |
-|------------------|-----------------------------|-----------------------------------------------|
-| Nicholas Strydom | nstrydom@gmail.com          | [nstrydom2](https://github.com/nstrydom2)     |
-| hentai-chan      | dev.hentai-chan@outlook.com | [hentai-chan](https://github.com/hentai-chan) |
-
-See also the list of [contributors](https://github.com/nstrydom2/anonfile-api/contributors)
-who participated in this project.
-
-## License
-
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for more details.
-
-## Acknowledgments
-
-* Joseph Marie Jacquard
-* Charles Babbage
-* Ada Lovelace
-* My Dad
-* Hat tip to anyone whose code was used
-* Inspiration
-* etc
+<p align="center">
+  <a href="https://github.com/nstrydom2/anonfile-api" title="Project Logo">
+    <img height="150" style="margin-top:15px" src="https://raw.githubusercontent.com/nstrydom2/anonfile-api/master/logo.svg">
+  </a>
+</p>
+
+# Anonfiles.com Unofficial Python API
+
+[![PyPI version shields.io](https://img.shields.io/pypi/v/anonfile)](https://pypi.python.org/pypi/anonfile/)
+[![CI](https://github.com/nstrydom2/anonfile-api/actions/workflows/python-package.yml/badge.svg?branch=master)](https://github.com/nstrydom2/anonfile-api/actions/workflows/python-package.yml)
+[![PyPI download total](https://img.shields.io/pypi/dm/anonfile)](https://pypi.python.org/pypi/anonfile/)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/anonfile)](https://pypi.python.org/pypi/anonfile/)
+[![PyPI license](https://img.shields.io/pypi/l/anonfile)](https://pypi.python.org/pypi/anonfile/)
+
+
+This unofficial Python API was created to make uploading and downloading files
+from https://anonfiles.com simple and effective for programming in Python. The goal of
+the project is to create an intuitive library for anonymous file sharing.
+
+## Getting Started
+
+These instructions will get you a copy of the project up and running on your local
+machine for development and testing purposes. See deployment for notes on how to
+deploy the project on a live system.
+
+### Prerequisites
+
+Python 3.8+ is required to run this application, other than that there are no
+prerequisites for the project, as the dependencies are included in the repository.
+
+### Installing
+
+To install the library is as simple as running
+
+```bash
+pip install anonfile
+```
+
+from the command line. To install this library in debug mode with dev dependencies, use
+
+```bash
+pip install -e .[dev]
+```
+
+instead. It is recommended to create an virtual environment prior
+to installing this library. If you only intend to use this library from the CLI,
+use [pipx](https://pypa.github.io/pipx/) for the installation instead:
+
+```bash
+pipx install anonfile
+```
+
+### Dev Notes
+
+Run unit tests locally:
+
+```bash
+pytest --verbose -s [--token "REDACTED"]
+```
+
+Add the `-k test_*` option if you want to test only a single function.
+
+## Usage
+
+Import the module and instantiate the `AnonFile()` constructor. Setting the download
+directory in `path` is optional. Using the API `token` in the constructor is optional
+as well. A valid `token` registers all file uploads online, i.e. a list of all uploaded
+files is made accessible to any user that [signs into your account](https://anonfiles.com/login).
+
+```python
+from anonfile import AnonFile
+
+anon = AnonFile()
+
+# upload a file and enable progressbar terminal feedback (off by default)
+upload = anon.upload('/home/guest/jims_paperwork.doc', progressbar=True)
+print(upload.url.geturl())
+
+# download a file and set the download directory
+from pathlib import Path
+target_dir = Path.home().joinpath('Downloads')
+download = anon.download("https://anonfiles.com/9ee1jcu6u9/test_txt", path=target_dir)
+print(download.file_path)
+```
+
+And voilà, pain-free anonymous file sharing. If you want more information about
+the `AnonFile` API visit [anonfiles.com](https://anonfiles.com/docs/api).
+
+## Command Line Interface
+
+```bash
+# open help page for specific commands
+anonfile [download|upload|preview|log] --help
+
+# note: both methods expect at least one argument, but can take on more
+anonfile download --url https://anonfiles.com/93k5x1ucu0/test_txt
+anonfile upload --file ./test.txt
+```
+
+## Built With
+
+* [Requests](http://docs.python-requests.org/en/master/) - Http for Humans
+* [TQDM](https://github.com/tqdm/tqdm) - Fast & Extensible Progress Bars
+* [anonfiles.com](https://anonfiles.com/docs/api) - AnonFiles.com REST API
+
+## Versioning
+
+Navigate to [tags on this repository](https://github.com/nstrydom2/anonfile-api/tags)
+to see all available versions.
+
+## Authors
+
+| Name             | Mail Address                | GitHub Profile                                |
+|------------------|-----------------------------|-----------------------------------------------|
+| Nicholas Strydom | nstrydom@gmail.com          | [nstrydom2](https://github.com/nstrydom2)     |
+| hentai-chan      | dev.hentai-chan@outlook.com | [hentai-chan](https://github.com/hentai-chan) |
+| Stefan Greve     | greve.stefan@outlook.jp     | [StefanGreve](https://github.com/stefangreve) |
+
+See also the list of [contributors](https://github.com/nstrydom2/anonfile-api/contributors)
+who participated in this project.
+
+## License
+
+This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for more details.
+
+## Acknowledgments
+
+* Joseph Marie Jacquard
+* Charles Babbage
+* Ada Lovelace
+* My Dad
+* Hat tip to anyone whose code was used
+* Inspiration
+* etc
```

#### html2text {}

```diff
@@ -4,52 +4,56 @@
 (https://github.com/nstrydom2/anonfile-api/actions/workflows/python-
 package.yml/badge.svg?branch=master)](https://github.com/nstrydom2/anonfile-
 api/actions/workflows/python-package.yml) [![PyPI download total](https://
 img.shields.io/pypi/dm/anonfile)](https://pypi.python.org/pypi/anonfile/) [!
 [PyPI pyversions](https://img.shields.io/pypi/pyversions/anonfile)](https://
 pypi.python.org/pypi/anonfile/) [![PyPI license](https://img.shields.io/pypi/l/
 anonfile)](https://pypi.python.org/pypi/anonfile/) This unofficial Python API
-was created to make uploading and downloading files from
-com> simple and effective for programming in Python. The goal of the project is
-to create an intuitive library for anonymous file sharing. ## Getting Started
+was created to make uploading and downloading files from https://anonfiles.com
+simple and effective for programming in Python. The goal of the project is to
+create an intuitive library for anonymous file sharing. ## Getting Started
 These instructions will get you a copy of the project up and running on your
 local machine for development and testing purposes. See deployment for notes on
-how to deploy the project on a live system. ### Prerequisites Python 3.7+ is
+how to deploy the project on a live system. ### Prerequisites Python 3.8+ is
 required to run this application, other than that there are no prerequisites
 for the project, as the dependencies are included in the repository. ###
 Installing To install the library is as simple as running ```bash pip install
-anonfile ``` from the command line. To install this library in debug mode, use
-```bash pip install -e . ``` instead. It is recommended to create an virtual
-environment prior to installing this library. ### Dev Notes Run unit tests
-locally: ```bash pytest --verbose -s [--token "REDACTED"] ``` Add the `-
-k test_*` option if you want to test only a single function. ## Usage Import
-the module and instantiate the `AnonFile()` constructor. Setting the download
-directory in `path` is optional. Using the API `token` in the constructor is
-optional as well. A valid `token` registers all file uploads online, i.e. a
-list of all uploaded files is made accessible to any user that [signs into your
-account](https://anonfiles.com/login). ```python from anonfile import AnonFile
-anon = AnonFile() # upload a file and enable progressbar terminal feedback
-upload = anon.upload('/home/guest/jims_paperwork.doc', progressbar=True) print
-(upload.url.geturl()) # download a file and set the download directory from
-pathlib import Path target_dir = Path.home().joinpath('Downloads') filename =
-anon.download("https://anonfiles.com/9ee1jcu6u9/test_txt", path=target_dir)
-print(filename) ``` And voilÃ , pain-free anonymous file sharing. If you want
-more information about the `AnonFile` API visit [anonfiles.com](https://
+anonfile ``` from the command line. To install this library in debug mode with
+dev dependencies, use ```bash pip install -e .[dev] ``` instead. It is
+recommended to create an virtual environment prior to installing this library.
+If you only intend to use this library from the CLI, use [pipx](https://
+pypa.github.io/pipx/) for the installation instead: ```bash pipx install
+anonfile ``` ### Dev Notes Run unit tests locally: ```bash pytest --verbose -s
+[--token "REDACTED"] ``` Add the `-k test_*` option if you want to test only a
+single function. ## Usage Import the module and instantiate the `AnonFile()`
+constructor. Setting the download directory in `path` is optional. Using the
+API `token` in the constructor is optional as well. A valid `token` registers
+all file uploads online, i.e. a list of all uploaded files is made accessible
+to any user that [signs into your account](https://anonfiles.com/login).
+```python from anonfile import AnonFile anon = AnonFile() # upload a file and
+enable progressbar terminal feedback (off by default) upload = anon.upload('/
+home/guest/jims_paperwork.doc', progressbar=True) print(upload.url.geturl()) #
+download a file and set the download directory from pathlib import Path
+target_dir = Path.home().joinpath('Downloads') download = anon.download("https:
+//anonfiles.com/9ee1jcu6u9/test_txt", path=target_dir) print
+(download.file_path) ``` And voilÃ , pain-free anonymous file sharing. If you
+want more information about the `AnonFile` API visit [anonfiles.com](https://
 anonfiles.com/docs/api). ## Command Line Interface ```bash # open help page for
 specific commands anonfile [download|upload|preview|log] --help # note: both
 methods expect at least one argument, but can take on more anonfile download --
 url https://anonfiles.com/93k5x1ucu0/test_txt anonfile upload --file ./test.txt
 ``` ## Built With * [Requests](http://docs.python-requests.org/en/master/) -
 Http for Humans * [TQDM](https://github.com/tqdm/tqdm) - Fast & Extensible
 Progress Bars * [anonfiles.com](https://anonfiles.com/docs/api) - AnonFiles.com
 REST API ## Versioning Navigate to [tags on this repository](https://
 github.com/nstrydom2/anonfile-api/tags) to see all available versions. ##
 Authors | Name | Mail Address | GitHub Profile | |------------------|----------
 -------------------|-----------------------------------------------| | Nicholas
 Strydom | nstrydom@gmail.com | [nstrydom2](https://github.com/nstrydom2) | |
 hentai-chan | dev.hentai-chan@outlook.com | [hentai-chan](https://github.com/
-hentai-chan) | See also the list of [contributors](https://github.com/
-nstrydom2/anonfile-api/contributors) who participated in this project. ##
-License This project is licensed under the MIT License - see the [LICENSE]
-(LICENSE) file for more details. ## Acknowledgments * Joseph Marie Jacquard *
-Charles Babbage * Ada Lovelace * My Dad * Hat tip to anyone whose code was used
-* Inspiration * etc
+hentai-chan) | | Stefan Greve | greve.stefan@outlook.jp | [StefanGreve](https:/
+/github.com/stefangreve) | See also the list of [contributors](https://
+github.com/nstrydom2/anonfile-api/contributors) who participated in this
+project. ## License This project is licensed under the MIT License - see the
+[LICENSE](LICENSE) file for more details. ## Acknowledgments * Joseph Marie
+Jacquard * Charles Babbage * Ada Lovelace * My Dad * Hat tip to anyone whose
+code was used * Inspiration * etc
```

### Comparing `anonfile-0.2.7/setup.py` & `anonfile-1.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,66 +1,68 @@
-import re
-
-from setuptools import find_packages, setup
-
-with open("src/anonfile/anonfile.py", encoding='utf-8') as file_handler:
-    lines = file_handler.read()
-    version = re.search(r'__version__ = "(.*?)"', lines).group(1)
-    package_name = re.search(r'package_name = "(.*?)"', lines).group(1)
-    python_major = int(re.search(r'python_major = "(.*?)"', lines).group(1))
-    python_minor = int(re.search(r'python_minor = "(.*?)"', lines).group(1))
-
-print("reading dependency file")
-
-with open("requirements/release.txt", mode='r', encoding='utf-8') as requirements:
-    packages = requirements.read().splitlines()
-
-with open("requirements/dev.txt", mode='r', encoding='utf-8') as requirements:
-    dev_packages = requirements.read().splitlines()
-
-print("reading readme file")
-
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
-setup(
-    name=package_name,
-    version=version,
-    author="Nicholas Strydom",
-    author_email="nstrydom@gmail.com",
-    description="An unofficial library that wraps the anonfile.com REST API.",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/nstrydom2/anonfile-api",
-    project_urls={
-        'Source Code': "https://github.com/nstrydom2/anonfile-api",
-        'Bug Reports': "https://github.com/nstrydom2/anonfile-api/issues",
-        'Changelog': "https://github.com/nstrydom2/anonfile-api/blob/master/CHANGELOG.md"
-    },    
-    python_requires=">=%d.%d" % (python_major, python_minor),
-    install_requires=packages,
-    extra_requires={
-        'dev': dev_packages[1:],
-        'test': ['pytest']
-    },
-    package_dir={'': 'src'},
-    packages=find_packages(where='src'),
-    entry_points={
-        'console_scripts': ['%s=%s.__init__:main' % (package_name, package_name)]
-    },
-    classifiers=[
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Intended Audience :: Developers",
-        "Natural Language :: English",
-        "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
-        "Topic :: Software Development :: Libraries",
-        "Topic :: Utilities",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    keywords="anonfile rest api"
-)
-
-wheel_name = package_name.replace('-', '_') if '-' in package_name else package_name
-print("\033[92mSetup is complete. Run 'python -m pip install dist/%s-%s-py%d-none-any.whl' to install this wheel.\033[0m" % (wheel_name, version, python_major))
+import re
+
+from setuptools import find_packages, setup
+
+with open("src/anonfile/anonfile.py", encoding='utf-8') as file_handler:
+    lines = file_handler.read()
+    version = re.search(r'__version__ = "(.*?)"', lines).group(1)
+    package_name = re.search(r'package_name = "(.*?)"', lines).group(1)
+    python_major = int(re.search(r'python_major = "(.*?)"', lines).group(1))
+    python_minor = int(re.search(r'python_minor = "(.*?)"', lines).group(1))
+
+print("reading dependency file")
+
+with open("requirements/release.txt", mode='r', encoding='utf-8') as requirements:
+    packages = requirements.read().splitlines()
+
+with open("requirements/dev.txt", mode='r', encoding='utf-8') as requirements:
+    dev_packages = requirements.read().splitlines()
+
+print("reading readme file")
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
+setup(
+    name=package_name,
+    version=version,
+    author="Nicholas Strydom",
+    author_email="nstrydom@gmail.com",
+    description="An unofficial library that wraps the anonfile.com REST API.",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/nstrydom2/anonfile-api",
+    project_urls={
+        'Source Code': "https://github.com/nstrydom2/anonfile-api",
+        'Bug Reports': "https://github.com/nstrydom2/anonfile-api/issues",
+        'Changelog': "https://github.com/nstrydom2/anonfile-api/blob/master/CHANGELOG.md"
+    },
+    python_requires=">=%d.%d" % (python_major, python_minor),
+    install_requires=packages,
+    extra_requires={
+        'dev': dev_packages[1:],
+        'test': ['pytest']
+    },
+    package_dir={'': 'src'},
+    packages=find_packages(where='src'),
+    include_package_data=True,
+    entry_points={
+        'console_scripts': ['%s=%s.__init__:main' % (package_name, package_name)]
+    },
+    classifiers=[
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Intended Audience :: Developers",
+        "Natural Language :: English",
+        "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
+        "Topic :: Software Development :: Libraries",
+        "Topic :: Utilities",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    keywords="anonfile rest api"
+)
+
+wheel_name = package_name.replace('-', '_') if '-' in package_name else package_name
+print("\033[92mSetup is complete. Run 'python -m pip install dist/%s-%s-py%d-none-any.whl' to install this wheel.\033[0m" % (wheel_name, version, python_major))
```

### Comparing `anonfile-0.2.7/src/anonfile/__init__.py` & `anonfile-1.0.0/src/anonfile/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,133 +1,139 @@
-#!/usr/bin/env python3
-
-from __future__ import annotations
-
-import argparse
-import sys
-from collections import namedtuple
-from distutils.util import strtobool
-from pathlib import Path
-from typing import List
-
-from .anonfile import *
-from .anonfile import __version__
-
-
-def __print_dict(dictionary: dict, indent: int = 4) -> None:
-    print("{\n%s\n}" % '\n'.join([f"\033[36m{indent * ' '}{key}\033[0m: \033[32m{value}\033[0m" for key, value in dictionary.items()]))
-
-
-def __from_file(path: Path) -> List[str]:
-    with open(path, mode='r', encoding='utf-8') as file_handler:
-        return [line.rstrip() for line in file_handler.readlines() if line[0] != '#']
-
-
-def format_proxies(proxies: str) -> dict:
-    return {prot: f"{prot}://{ip}" for (prot, ip) in [proxy.split('://') for proxy in proxies.split()]}
-
-
-def main():
-    parser = argparse.ArgumentParser(prog=package_name)
-    parser._positionals.title = 'Commands'
-    parser._optionals.title = 'Arguments'
-
-    parser.add_argument('-v', '--version', action='version', version=f"%(prog)s {__version__}")
-    parser.add_argument('-V', '--verbose', default=True, action='store_true', help="increase output verbosity (default)")
-    parser.add_argument('--no-verbose', dest='verbose', action='store_false', help="run commands silently")
-    parser.add_argument('-l', '--logging', default=True, action='store_true', help="enable URL logging (default)")
-    parser.add_argument('--no-logging', dest='logging', action='store_false', help="disable all logging activities")
-    parser.add_argument('-t', '--token', type=str, default='secret', help="configure an API token (optional)")
-    parser.add_argument('-a', '--user-agent', type=str, default=None, help="configure custom User-Agent (optional)")
-    parser.add_argument('-p', '--proxies', type=str, default=None, help="configure HTTP and/or HTTPS proxies (optional)")
-
-    subparser = parser.add_subparsers(dest='command')
-    upload_parser = subparser.add_parser('upload', help="upload a file to https://anonfiles.com")
-    upload_parser.add_argument('-f', '--file', nargs='+', type=Path, help="one or more files to upload.", required=True)
-
-    preview_parser = subparser.add_parser('preview', help="read meta data from a file on https://anonfiles.com")
-    preview_parser.add_argument('-u', '--url', nargs='+', type=str, help="one or more URLs to preview", required=True)
-
-    download_parser = subparser.add_parser('download', help="download a file from https://anonfiles.com")
-    download_parser.add_argument('-u', '--url', nargs='*', type=str, help="one or more URLs to download")
-    download_parser.add_argument('-f', '--batch-file', type=Path, nargs='?', help="file containing URLs to download, one URL per line")
-    download_parser.add_argument('-p', '--path', type=Path, default=Path.cwd(), help="download directory (CWD by default)")
-    download_parser.add_argument('-c', '--check', default=True, action='store_true', help="check for duplicates (default)")
-    download_parser.add_argument('--no-check', dest='check', action='store_false', help="disable checking for duplicates")
-
-    log_parser = subparser.add_parser('log', help="access the anonfile logger")
-    log_parser.add_argument('--reset', action='store_true', help="reset all log file entries")
-    log_parser.add_argument('--path', action='store_true', help="return the log file path")
-    log_parser.add_argument('--read', action='store_true', help='read the log file')
-
-    try:
-        args = parser.parse_args()
-        anon = AnonFile(args.token, user_agent=args.user_agent, proxies=format_proxies(args.proxies) if args.proxies else None)
-
-        if args.command is None:
-            raise UserWarning("missing a command")
-
-        if args.user_agent is not None:
-            anon.user_agent = args.user_agent
-
-        if args.command == 'upload':
-            for file in args.file:
-                upload = anon.upload(file, progressbar=args.verbose, enable_logging=args.logging)
-                print(f"URL: {upload.url.geturl()}")
-
-        if args.command == 'preview':
-            for url in args.url:
-                preview = anon.preview(url)
-                values = ['online' if preview.status else 'offline', preview.file_path.name, preview.url.geturl(), preview.ddl.geturl(), preview.id, f"{preview.size}B"]
-
-                if args.verbose:
-                    __print_dict(dict(zip(['Status', 'File Path', 'URL', 'DDL', 'ID', 'Size'], values)))
-                else:
-                    print(','.join(values))
-
-        if args.command == 'download':
-            for url in (args.url or __from_file(args.batch_file)):
-                download = lambda url: anon.download(url, args.path, progressbar=args.verbose, enable_logging=args.logging)
-
-                if args.check and anon.preview(url, args.path).file_path.exists():
-                    print(f"\033[33mWarning:\033[0m A file with the same name already exists in {str(args.path)!r}.")
-                    choice = input("Proceed with download? [Y/n] ")
-                    if choice == '' or strtobool(choice):
-                        print(f"File: {download(url).file_path}")
-                else:
-                    print(f"File: {download(url).file_path}")
-
-        if args.command == 'log':
-            if args.reset:
-                open(get_logfile_path(), mode='w', encoding='utf-8').close()
-            if args.path:
-                print(get_logfile_path())
-            if args.read:
-                with open(get_logfile_path(), mode='r', encoding='utf-8') as file_handler:
-                    log = file_handler.readlines()
-
-                    if not log:
-                        msg = "Nothing to read because the log file is empty"
-                        print(f"\033[33m{'[ WARNING ]'.ljust(12, ' ')}\033[0m{msg}")
-                        return
-
-                    parse = lambda line: line.strip('\n').split('::')
-                    Entry = namedtuple('Entry', 'timestamp method url')
-
-                    tabulate = "{:<19} {:<8} {:<30}".format
-
-                    print(f"\033[32m{tabulate('Date', 'Method', 'URL')}\033[0m")
-
-                    for line in log:
-                        entry = Entry(parse(line)[0], parse(line)[1], parse(line)[2])
-                        print(tabulate(entry.timestamp, entry.method, entry.url))
-
-    except UserWarning as bad_human:
-        print(f"error: {bad_human}")
-        parser.print_help(sys.stderr)
-        sys.exit(2)
-    except Exception as error:
-        print(error, file=sys.stderr)
-
-
-if __name__ == '__main__':
-    main()
+#!/usr/bin/env python3
+
+from __future__ import annotations
+
+import json
+import sys
+from argparse import ArgumentParser
+from collections import namedtuple
+from pathlib import Path
+from typing import List
+
+from .anonfile import *
+from .anonfile import __version__, package_name
+
+
+def str2bool(val: str) -> bool:
+    return val.lower() in ('yes', 'y', 'true', 't', '1', 'on', '')
+
+def __from_file(path: Path) -> List[str]:
+    with open(path, mode='r', encoding='utf-8') as file_handler:
+        return [line.rstrip() for line in file_handler.readlines() if line[0] != '#']
+
+def format_proxies(proxies: str) -> dict:
+    return {prot: f"{prot}://{ip}" for (prot, ip) in [proxy.split('://') for proxy in proxies.split()]}
+
+def build_parser(package_name: str, version: str) -> ArgumentParser:
+    parser = ArgumentParser(prog=package_name)
+    parser._positionals.title = 'Commands'
+    parser._optionals.title = 'Arguments'
+
+    parser.add_argument('-v', '--version', action='version', version=f"%(prog)s {version}")
+    parser.add_argument('-V', '--verbose', default=True, action='store_true', help="increase output verbosity (default)")
+    parser.add_argument('--no-verbose', dest='verbose', action='store_false', help="run commands silently")
+    parser.add_argument('-l', '--logging', default=True, action='store_true', help="enable URL logging (default)")
+    parser.add_argument('--no-logging', dest='logging', action='store_false', help="disable all logging activities")
+    parser.add_argument('-t', '--token', type=str, default='secret', help="configure an API token (optional)")
+    parser.add_argument('-a', '--user-agent', type=str, default=None, help="configure custom User-Agent (optional)")
+    parser.add_argument('-p', '--proxies', type=str, default=None, help="configure HTTP and/or HTTPS proxies (optional)")
+
+    subparser = parser.add_subparsers(dest='command')
+    upload_parser = subparser.add_parser('upload', help="upload a file to https://anonfiles.com")
+    upload_parser.add_argument('-f', '--file', nargs='+', type=Path, help="one or more files to upload.", required=True)
+
+    preview_parser = subparser.add_parser('preview', help="read meta data from a file on https://anonfiles.com")
+    preview_parser.add_argument('-u', '--url', nargs='+', type=str, help="one or more URLs to preview", required=True)
+
+    download_parser = subparser.add_parser('download', help="download a file from https://anonfiles.com")
+    download_parser.add_argument('-u', '--url', nargs='*', type=str, help="one or more URLs to download")
+    download_parser.add_argument('-f', '--batch-file', type=Path, nargs='?', help="file containing URLs to download, one URL per line")
+    download_parser.add_argument('-p', '--path', type=Path, default=Path.cwd(), help="download directory (CWD by default)")
+    download_parser.add_argument('-c', '--check', default=True, action='store_true', help="check for duplicates (default)")
+    download_parser.add_argument('--no-check', dest='check', action='store_false', help="disable checking for duplicates")
+
+    log_parser = subparser.add_parser('log', help="access the anonfile logger")
+    log_parser.add_argument('--reset', action='store_true', help="reset all log file entries")
+    log_parser.add_argument('--path', action='store_true', help="return the log file path")
+    log_parser.add_argument('--read', action='store_true', help='read the log file')
+
+    return parser
+
+def main():
+    parser = build_parser(package_name, __version__)
+
+    try:
+        args = parser.parse_args()
+        anon = AnonFile(args.token, user_agent=args.user_agent, proxies=format_proxies(args.proxies) if args.proxies else None)
+
+        if args.command is None:
+            raise UserWarning("missing a command")
+
+        if args.user_agent is not None:
+            anon.user_agent = args.user_agent
+
+        if args.command == 'upload':
+            for file in args.file:
+                upload = anon.upload(file, progressbar=args.verbose, enable_logging=args.logging)
+                print(f"URL: {upload.url.geturl()}")
+
+        if args.command == 'preview':
+            for url in args.url:
+                preview = anon.preview(url)
+                response = {
+                    'Status': 'online' if preview.status else 'offline',
+                    'File Path': preview.file_path.name,
+                    'URL': preview.url.geturl(),
+                    'DDL': preview.ddl.geturl(),
+                    'ID': preview.id,
+                    'Size': preview.size_readable,
+                }
+
+                print(json.dumps(response, indent=4) if args.verbose else ','.join(response.values))
+
+        if args.command == 'download':
+            for url in (args.url or __from_file(args.batch_file)):
+                download = lambda url: anon.download(url, args.path, progressbar=args.verbose, enable_logging=args.logging)
+
+                if args.check and anon.preview(url, args.path).file_path.exists():
+                    print(f"Warning: A file with the same name already exists in {str(args.path)!r}.")
+                    prompt = input("Proceed with download? [Y/n] ")
+                    if str2bool(prompt):
+                        print(f"File: {download(url).file_path}")
+                else:
+                    print(f"File: {download(url).file_path}")
+
+        if args.command == 'log':
+            if args.reset:
+                open(get_logfile_path(), mode='w', encoding='utf-8').close()
+            if args.path:
+                print(get_logfile_path())
+            if args.read:
+                with open(get_logfile_path(), mode='r', encoding='utf-8') as file_handler:
+                    log = file_handler.readlines()
+
+                    if not log:
+                        msg = "Nothing to read because the log file is empty"
+                        print(f"\033[33m{'[ WARNING ]'.ljust(12, ' ')}\033[0m{msg}")
+                        return
+
+                    parse = lambda line: line.strip('\n').split('::')
+                    Entry = namedtuple('Entry', 'timestamp method url')
+
+                    tabulate = "{:<19} {:<8} {:<30}".format
+
+                    print(f"\033[32m{tabulate('Date', 'Method', 'URL')}\033[0m")
+
+                    for line in log:
+                        entry = Entry(parse(line)[0], parse(line)[1], parse(line)[2])
+                        print(tabulate(entry.timestamp, entry.method, entry.url))
+
+    except UserWarning as bad_human:
+        print(f"error: {bad_human}")
+        parser.print_help(sys.stderr)
+        sys.exit(2)
+    except Exception as error:
+        print(error, file=sys.stderr)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `anonfile-0.2.7/src/anonfile.egg-info/PKG-INFO` & `anonfile-1.0.0/src/anonfile.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anonfile
-Version: 0.2.7
+Version: 1.0.0
 Summary: An unofficial library that wraps the anonfile.com REST API.
 Home-page: https://github.com/nstrydom2/anonfile-api
 Author: Nicholas Strydom
 Author-email: nstrydom@gmail.com
 License: UNKNOWN
 Project-URL: Source Code, https://github.com/nstrydom2/anonfile-api
 Project-URL: Bug Reports, https://github.com/nstrydom2/anonfile-api/issues
@@ -21,44 +21,49 @@
         [![CI](https://github.com/nstrydom2/anonfile-api/actions/workflows/python-package.yml/badge.svg?branch=master)](https://github.com/nstrydom2/anonfile-api/actions/workflows/python-package.yml)
         [![PyPI download total](https://img.shields.io/pypi/dm/anonfile)](https://pypi.python.org/pypi/anonfile/)
         [![PyPI pyversions](https://img.shields.io/pypi/pyversions/anonfile)](https://pypi.python.org/pypi/anonfile/)
         [![PyPI license](https://img.shields.io/pypi/l/anonfile)](https://pypi.python.org/pypi/anonfile/)
         
         
         This unofficial Python API was created to make uploading and downloading files
-        from <anonfiles.com> simple and effective for programming in Python. The goal of
+        from https://anonfiles.com simple and effective for programming in Python. The goal of
         the project is to create an intuitive library for anonymous file sharing.
         
         ## Getting Started
         
         These instructions will get you a copy of the project up and running on your local
         machine for development and testing purposes. See deployment for notes on how to
         deploy the project on a live system.
         
         ### Prerequisites
         
-        Python 3.7+ is required to run this application, other than that there are no
+        Python 3.8+ is required to run this application, other than that there are no
         prerequisites for the project, as the dependencies are included in the repository.
         
         ### Installing
         
         To install the library is as simple as running
         
         ```bash
         pip install anonfile
         ```
         
-        from the command line. To install this library in debug mode, use
+        from the command line. To install this library in debug mode with dev dependencies, use
         
         ```bash
-        pip install -e .
+        pip install -e .[dev]
         ```
         
         instead. It is recommended to create an virtual environment prior
-        to installing this library.
+        to installing this library. If you only intend to use this library from the CLI,
+        use [pipx](https://pypa.github.io/pipx/) for the installation instead:
+        
+        ```bash
+        pipx install anonfile
+        ```
         
         ### Dev Notes
         
         Run unit tests locally:
         
         ```bash
         pytest --verbose -s [--token "REDACTED"]
@@ -74,23 +79,23 @@
         files is made accessible to any user that [signs into your account](https://anonfiles.com/login).
         
         ```python
         from anonfile import AnonFile
         
         anon = AnonFile()
         
-        # upload a file and enable progressbar terminal feedback
+        # upload a file and enable progressbar terminal feedback (off by default)
         upload = anon.upload('/home/guest/jims_paperwork.doc', progressbar=True)
         print(upload.url.geturl())
         
         # download a file and set the download directory
         from pathlib import Path
         target_dir = Path.home().joinpath('Downloads')
-        filename = anon.download("https://anonfiles.com/9ee1jcu6u9/test_txt", path=target_dir)
-        print(filename)
+        download = anon.download("https://anonfiles.com/9ee1jcu6u9/test_txt", path=target_dir)
+        print(download.file_path)
         ```
         
         And voilà, pain-free anonymous file sharing. If you want more information about
         the `AnonFile` API visit [anonfiles.com](https://anonfiles.com/docs/api).
         
         ## Command Line Interface
         
@@ -116,14 +121,15 @@
         
         ## Authors
         
         | Name             | Mail Address                | GitHub Profile                                |
         |------------------|-----------------------------|-----------------------------------------------|
         | Nicholas Strydom | nstrydom@gmail.com          | [nstrydom2](https://github.com/nstrydom2)     |
         | hentai-chan      | dev.hentai-chan@outlook.com | [hentai-chan](https://github.com/hentai-chan) |
+        | Stefan Greve     | greve.stefan@outlook.jp     | [StefanGreve](https://github.com/stefangreve) |
         
         See also the list of [contributors](https://github.com/nstrydom2/anonfile-api/contributors)
         who participated in this project.
         
         ## License
         
         This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for more details.
@@ -136,19 +142,20 @@
         * My Dad
         * Hat tip to anyone whose code was used
         * Inspiration
         * etc
         
 Keywords: anonfile rest api
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: anonfile Version: 0.2.7 Summary: An unofficial
+Metadata-Version: 2.1 Name: anonfile Version: 1.0.0 Summary: An unofficial
 library that wraps the anonfile.com REST API. Home-page: https://github.com/
 nstrydom2/anonfile-api Author: Nicholas Strydom Author-email:
 nstrydom@gmail.com License: UNKNOWN Project-URL: Source Code, https://
 github.com/nstrydom2/anonfile-api Project-URL: Bug Reports, https://github.com/
 nstrydom2/anonfile-api/issues Project-URL: Changelog, https://github.com/
 nstrydom2/anonfile-api/blob/master/CHANGELOG.md Description:
   [https://raw.githubusercontent.com/nstrydom2/anonfile-api/master/logo.svg]
@@ -11,59 +11,64 @@
 (https://github.com/nstrydom2/anonfile-api/actions/workflows/python-
 package.yml/badge.svg?branch=master)](https://github.com/nstrydom2/anonfile-
 api/actions/workflows/python-package.yml) [![PyPI download total](https://
 img.shields.io/pypi/dm/anonfile)](https://pypi.python.org/pypi/anonfile/) [!
 [PyPI pyversions](https://img.shields.io/pypi/pyversions/anonfile)](https://
 pypi.python.org/pypi/anonfile/) [![PyPI license](https://img.shields.io/pypi/l/
 anonfile)](https://pypi.python.org/pypi/anonfile/) This unofficial Python API
-was created to make uploading and downloading files from
-com> simple and effective for programming in Python. The goal of the project is
-to create an intuitive library for anonymous file sharing. ## Getting Started
+was created to make uploading and downloading files from https://anonfiles.com
+simple and effective for programming in Python. The goal of the project is to
+create an intuitive library for anonymous file sharing. ## Getting Started
 These instructions will get you a copy of the project up and running on your
 local machine for development and testing purposes. See deployment for notes on
-how to deploy the project on a live system. ### Prerequisites Python 3.7+ is
+how to deploy the project on a live system. ### Prerequisites Python 3.8+ is
 required to run this application, other than that there are no prerequisites
 for the project, as the dependencies are included in the repository. ###
 Installing To install the library is as simple as running ```bash pip install
-anonfile ``` from the command line. To install this library in debug mode, use
-```bash pip install -e . ``` instead. It is recommended to create an virtual
-environment prior to installing this library. ### Dev Notes Run unit tests
-locally: ```bash pytest --verbose -s [--token "REDACTED"] ``` Add the `-
-k test_*` option if you want to test only a single function. ## Usage Import
-the module and instantiate the `AnonFile()` constructor. Setting the download
-directory in `path` is optional. Using the API `token` in the constructor is
-optional as well. A valid `token` registers all file uploads online, i.e. a
-list of all uploaded files is made accessible to any user that [signs into your
-account](https://anonfiles.com/login). ```python from anonfile import AnonFile
-anon = AnonFile() # upload a file and enable progressbar terminal feedback
-upload = anon.upload('/home/guest/jims_paperwork.doc', progressbar=True) print
-(upload.url.geturl()) # download a file and set the download directory from
-pathlib import Path target_dir = Path.home().joinpath('Downloads') filename =
-anon.download("https://anonfiles.com/9ee1jcu6u9/test_txt", path=target_dir)
-print(filename) ``` And voilÃ , pain-free anonymous file sharing. If you want
-more information about the `AnonFile` API visit [anonfiles.com](https://
+anonfile ``` from the command line. To install this library in debug mode with
+dev dependencies, use ```bash pip install -e .[dev] ``` instead. It is
+recommended to create an virtual environment prior to installing this library.
+If you only intend to use this library from the CLI, use [pipx](https://
+pypa.github.io/pipx/) for the installation instead: ```bash pipx install
+anonfile ``` ### Dev Notes Run unit tests locally: ```bash pytest --verbose -s
+[--token "REDACTED"] ``` Add the `-k test_*` option if you want to test only a
+single function. ## Usage Import the module and instantiate the `AnonFile()`
+constructor. Setting the download directory in `path` is optional. Using the
+API `token` in the constructor is optional as well. A valid `token` registers
+all file uploads online, i.e. a list of all uploaded files is made accessible
+to any user that [signs into your account](https://anonfiles.com/login).
+```python from anonfile import AnonFile anon = AnonFile() # upload a file and
+enable progressbar terminal feedback (off by default) upload = anon.upload('/
+home/guest/jims_paperwork.doc', progressbar=True) print(upload.url.geturl()) #
+download a file and set the download directory from pathlib import Path
+target_dir = Path.home().joinpath('Downloads') download = anon.download("https:
+//anonfiles.com/9ee1jcu6u9/test_txt", path=target_dir) print
+(download.file_path) ``` And voilÃ , pain-free anonymous file sharing. If you
+want more information about the `AnonFile` API visit [anonfiles.com](https://
 anonfiles.com/docs/api). ## Command Line Interface ```bash # open help page for
 specific commands anonfile [download|upload|preview|log] --help # note: both
 methods expect at least one argument, but can take on more anonfile download --
 url https://anonfiles.com/93k5x1ucu0/test_txt anonfile upload --file ./test.txt
 ``` ## Built With * [Requests](http://docs.python-requests.org/en/master/) -
 Http for Humans * [TQDM](https://github.com/tqdm/tqdm) - Fast & Extensible
 Progress Bars * [anonfiles.com](https://anonfiles.com/docs/api) - AnonFiles.com
 REST API ## Versioning Navigate to [tags on this repository](https://
 github.com/nstrydom2/anonfile-api/tags) to see all available versions. ##
 Authors | Name | Mail Address | GitHub Profile | |------------------|----------
 -------------------|-----------------------------------------------| | Nicholas
 Strydom | nstrydom@gmail.com | [nstrydom2](https://github.com/nstrydom2) | |
 hentai-chan | dev.hentai-chan@outlook.com | [hentai-chan](https://github.com/
-hentai-chan) | See also the list of [contributors](https://github.com/
-nstrydom2/anonfile-api/contributors) who participated in this project. ##
-License This project is licensed under the MIT License - see the [LICENSE]
-(LICENSE) file for more details. ## Acknowledgments * Joseph Marie Jacquard *
-Charles Babbage * Ada Lovelace * My Dad * Hat tip to anyone whose code was used
-* Inspiration * etc Keywords: anonfile rest api Platform: UNKNOWN Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Intended Audience :: Developers Classifier: Natural Language :: English
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content Classifier: Topic
-:: Software Development :: Libraries Classifier: Topic :: Utilities Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
+hentai-chan) | | Stefan Greve | greve.stefan@outlook.jp | [StefanGreve](https:/
+/github.com/stefangreve) | See also the list of [contributors](https://
+github.com/nstrydom2/anonfile-api/contributors) who participated in this
+project. ## License This project is licensed under the MIT License - see the
+[LICENSE](LICENSE) file for more details. ## Acknowledgments * Joseph Marie
+Jacquard * Charles Babbage * Ada Lovelace * My Dad * Hat tip to anyone whose
+code was used * Inspiration * etc Keywords: anonfile rest api Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Intended
+Audience :: Developers Classifier: Natural Language :: English Classifier:
+Topic :: Internet :: WWW/HTTP :: Dynamic Content Classifier: Topic :: Software
+Development :: Libraries Classifier: Topic :: Utilities Classifier: License ::
+OSI Approved :: MIT License Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8 Description-Content-Type: text/markdown
```

