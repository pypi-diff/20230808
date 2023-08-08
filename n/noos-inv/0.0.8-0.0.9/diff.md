# Comparing `tmp/noos-inv-0.0.8.tar.gz` & `tmp/noos-inv-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noos-inv-0.0.8.tar", last modified: Thu Oct  7 15:03:46 2021, max compression
+gzip compressed data, was "noos-inv-0.0.9.tar", last modified: Thu Sep  1 10:01:11 2022, max compression
```

## Comparing `noos-inv-0.0.8.tar` & `noos-inv-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1077 2021-10-07 15:03:23.197745 noos-inv-0.0.8/LICENSE
--rw-r--r--   0        0        0     3580 2021-10-07 15:03:23.197745 noos-inv-0.0.8/README.md
--rw-r--r--   0        0        0     1317 2021-10-07 15:03:23.197745 noos-inv-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      536 2021-10-07 15:03:23.197745 noos-inv-0.0.8/src/noos_inv/__init__.py
--rw-r--r--   0        0        0     2437 2021-10-07 15:03:23.197745 noos-inv-0.0.8/src/noos_inv/docker.py
--rw-r--r--   0        0        0      545 2021-10-07 15:03:23.197745 noos-inv-0.0.8/src/noos_inv/git.py
--rw-r--r--   0        0        0     2354 2021-10-07 15:03:23.197745 noos-inv-0.0.8/src/noos_inv/helm.py
--rw-r--r--   0        0        0      456 2021-10-07 15:03:23.197745 noos-inv-0.0.8/src/noos_inv/local.py
--rw-r--r--   0        0        0     3579 2021-10-07 15:03:23.197745 noos-inv-0.0.8/src/noos_inv/python.py
--rw-r--r--   0        0        0     1274 2021-10-07 15:03:23.197745 noos-inv-0.0.8/src/noos_inv/terraform.py
--rw-r--r--   0        0        0      256 2021-10-07 15:03:23.197745 noos-inv-0.0.8/src/noos_inv/utils.py
--rw-r--r--   0        0        0     4496 2021-10-07 15:03:47.015198 noos-inv-0.0.8/setup.py
--rw-r--r--   0        0        0     4217 2021-10-07 15:03:47.015805 noos-inv-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1077 2022-09-01 10:00:55.296398 noos-inv-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3580 2022-09-01 10:00:55.296398 noos-inv-0.0.9/README.md
+-rw-r--r--   0        0        0     1819 2022-09-01 10:00:55.296398 noos-inv-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      536 2022-09-01 10:00:55.296398 noos-inv-0.0.9/src/noos_inv/__init__.py
+-rw-r--r--   0        0        0     2381 2022-09-01 10:00:55.296398 noos-inv-0.0.9/src/noos_inv/docker.py
+-rw-r--r--   0        0        0      545 2022-09-01 10:00:55.296398 noos-inv-0.0.9/src/noos_inv/git.py
+-rw-r--r--   0        0        0     3440 2022-09-01 10:00:55.296398 noos-inv-0.0.9/src/noos_inv/helm.py
+-rw-r--r--   0        0        0      456 2022-09-01 10:00:55.296398 noos-inv-0.0.9/src/noos_inv/local.py
+-rw-r--r--   0        0        0     3579 2022-09-01 10:00:55.296398 noos-inv-0.0.9/src/noos_inv/python.py
+-rw-r--r--   0        0        0     1274 2022-09-01 10:00:55.296398 noos-inv-0.0.9/src/noos_inv/terraform.py
+-rw-r--r--   0        0        0      318 2022-09-01 10:00:55.296398 noos-inv-0.0.9/src/noos_inv/utils.py
+-rw-r--r--   0        0        0     4496 2022-09-01 10:01:11.891157 noos-inv-0.0.9/setup.py
+-rw-r--r--   0        0        0     4217 2022-09-01 10:01:11.891602 noos-inv-0.0.9/PKG-INFO
```

### Comparing `noos-inv-0.0.8/LICENSE` & `noos-inv-0.0.9/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020 Noos Energy Limited.
+Copyright (c) 2022 Noos Energy Limited.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `noos-inv-0.0.8/README.md` & `noos-inv-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `noos-inv-0.0.8/pyproject.toml` & `noos-inv-0.0.9/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry>=1.0.0"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 # Description
 name = "noos-inv"
-version = "0.0.8"
+version = "0.0.9"
 description = "Shared workflows across CI/CD pipelines"
 # Credentials
 license = "MIT"
 authors = ["Noos Energy <contact@noos.energy>"]
 homepage = "https://github.com/noosenergy/noos-invoke"
 # Package data
 readme = "README.md"
@@ -45,18 +45,41 @@
 pytest = "*"
 pytest-cov = "*"
 pytest-mock = "*"
 # Debugging
 ipdb = "*"
 ipython = "*"
 
+[tool.black]
+line-length = 99
+target_version = ['py38']
+
 [tool.isort]
 line_length = 99
+profile = "black"
 multi_line_output = 3
 lines_after_imports = 2
 default_section = "THIRDPARTY"
 known_first_party = "noos_inv"
 sections = "STDLIB,THIRDPARTY,FIRSTPARTY,LOCALFOLDER"
 
-[tool.black]
-line-length = 99
-target_version = ['py38']
+[tool.mypy]
+install_types = true
+non_interactive = true
+incremental = true
+warn_unused_configs = false
+warn_unused_ignores = true
+check_untyped_defs = true
+warn_redundant_casts = true
+ignore_missing_imports = true
+
+[tool.pytest.ini_options]
+python_files = "test_*.py"
+python_classes = "Test"
+python_functions = "test_*"
+filterwarnings = "error::RuntimeWarning"
+pythonpath = ["src"]
+junit_family = "xunit2"
+addopts = "--junitxml=pytest.xml"
+
+[tool.coverage.run]
+source = "noos_inv/*"
```

### Comparing `noos-inv-0.0.8/src/noos_inv/__init__.py` & `noos-inv-0.0.9/src/noos_inv/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # http://docs.pyinvoke.org/en/stable/concepts/library.html
 
 from invoke import Collection, Config, Program
 
 from . import docker, git, helm, local, python, terraform
 
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 
 class BaseConfig(Config):
     prefix = "noosinv"
 
 
 ns = Collection()
```

### Comparing `noos-inv-0.0.8/src/noos_inv/docker.py` & `noos-inv-0.0.9/src/noos_inv/docker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,39 @@
-import enum
 import os
 from typing import Optional
 
 from invoke import Collection, Context, task
 
 from . import utils
 
 
 CONFIG = {
     "docker": {
         # Sensitive
         "repo": None,
+        "user": "AWS",
         "token": None,
         "arg": None,
         # Non-sensitive
-        "user": "AWS",
-        "name": "webserver",
         "file": "Dockerfile",
         "context": ".",
+        "name": "webserver",
         "tag": "test",
     }
 }
 
 
-class UserType(str, enum.Enum):
-    AWS = "AWS"
-
-
 # Docker deployment workflow:
 
 
 @task
 def login(ctx, repo=None, user=None, token=None):
     """Login to Docker remote registry (AWS ECR or Dockerhub)."""
     user = user or ctx.docker.user
-    if user == UserType.AWS:
+    if user == utils.UserType.AWS:
         _aws_login(ctx, repo)
     else:
         _dockerhub_login(ctx, user, token)
 
 
 def _aws_login(ctx: Context, repo: Optional[str]) -> None:
     repo = repo or ctx.docker.repo
```

### Comparing `noos-inv-0.0.8/src/noos_inv/git.py` & `noos-inv-0.0.9/src/noos_inv/git.py`

 * *Files identical despite different names*

### Comparing `noos-inv-0.0.8/src/noos_inv/helm.py` & `noos-inv-0.0.9/src/noos_inv/helm.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,57 @@
-from invoke import Collection, task
+from typing import Optional
+
+from invoke import Collection, Context, task
 
 from . import utils
 
 
 CONFIG = {
     "helm": {
+        # Sensitive
         "repo": "local-repo",
         "url": None,
-        "user": None,
+        "user": "AWS",
         "token": None,
+        # Non-sensitive
         "plugins": ["https://github.com/chartmuseum/helm-push.git"],
         "chart": "./helm/chart",
         "values": "./local/helm-values.yaml",
+        "name": "webserver",
+        "tag": "0.1.0",
     }
 }
 
 
 # Helm deployment workflow:
 
 
 @task
 def login(ctx, repo=None, url=None, user=None, token=None):
-    """Login to Helm remote registry (Chart Museum)."""
+    """Login to Helm remote registry (AWS ECR or Chart Museum)."""
     repo = repo or ctx.helm.repo
-    url = url or ctx.helm.url
     user = user or ctx.helm.user
+    if user == utils.UserType.AWS:
+        _aws_login(ctx, repo)
+    else:
+        _cm_login(ctx, user, repo, url, token)
+
+
+def _aws_login(ctx: Context, repo: str) -> None:
+    cmd = "aws ecr get-login-password | "
+    cmd += f"helm registry login --username AWS --password-stdin {repo}"
+    ctx.run(cmd)
+
+
+def _cm_login(
+    ctx: Context, user: str, repo: str, url: Optional[str], token: Optional[str]
+) -> None:
+    url = url or ctx.helm.url
     token = token or ctx.helm.token
     assert url is not None, "Missing remote Helm registry url."
-    assert user is not None, "Missing remote Helm registry user."
     assert token is not None, "Missing remote Helm registry token."
     ctx.run(f"helm repo add {repo} {url} --username {user} --password {token}")
 
 
 @task(iterable=["plugins"])
 def install(ctx, plugins=None):
     """Provision local Helm client (Chart Museum Plugin)."""
@@ -67,19 +87,35 @@
     cmd += f"--create-namespace --namespace {namespace} --kube-context {context}"
     if dry_run:
         cmd += " --dry-run --debug"
     ctx.run(cmd)
 
 
 @task
-def push(ctx, chart=None, repo=None):
-    """Push Helm chart to a remote registry."""
-    chart = chart or ctx.helm.chart
+def push(ctx, chart=None, repo=None, name=None, tag=None):
+    """Push Helm chart to a remote registry (AWS ECR or Chart Museum)."""
     repo = repo or ctx.helm.repo
+    chart = chart or ctx.helm.chart
     utils.check_path(chart)
+    if ctx.helm.user == utils.UserType.AWS:
+        _aws_push(ctx, chart, repo, name, tag)
+    else:
+        _cm_push(ctx, chart, repo)
+
+
+def _aws_push(
+    ctx: Context, chart: str, repo: Optional[str], name: Optional[str], tag: Optional[str]
+) -> None:
+    names = (name or ctx.helm.name).split("/")
+    tag = tag or ctx.helm.tag
+    ctx.run(f"helm package {chart} --dependency-update")
+    ctx.run(f"helm push {names[-1]}-{tag}.tgz oci://{repo}/{'/'.join(names[:-1])}")
+
+
+def _cm_push(ctx: Context, chart: str, repo: Optional[str]) -> None:
     ctx.run(f"helm dependency update {chart}")
     ctx.run(f"helm cm-push {chart} {repo}")
 
 
 ns = Collection("helm")
 ns.configure(CONFIG)
 ns.add_task(login)
```

### Comparing `noos-inv-0.0.8/src/noos_inv/python.py` & `noos-inv-0.0.9/src/noos_inv/python.py`

 * *Files identical despite different names*

### Comparing `noos-inv-0.0.8/src/noos_inv/terraform.py` & `noos-inv-0.0.9/src/noos_inv/terraform.py`

 * *Files identical despite different names*

### Comparing `noos-inv-0.0.8/setup.py` & `noos-inv-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['invoke']
 
 entry_points = \
 {'console_scripts': ['noosinv = noos_inv:main.run']}
 
 setup_kwargs = {
     'name': 'noos-inv',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Shared workflows across CI/CD pipelines',
     'long_description': '[![CircleCI](https://circleci.com/gh/noosenergy/noos-invoke.svg?style=svg&circle-token=68d1a71e4f53ab1a1f33110e9a8c24bd3300a8ba)](https://circleci.com/gh/noosenergy/noos-invoke)\n\n# Noos Invoke\n\nSoftware development kit for sharing workflows across CI/CD pipelines.\n\nSuch a project aims to enforce parity and reproducability between local development and CI/CD workflows in remote containers (e.g. executable versions, command line calls, environment variables...) - developped with `inv[oke]`(https://github.com/pyinvoke/invoke).\n\n## Installation\n\nInstall the package from the [PyPi repository](https://pypi.org/project/noos-inv/):\n\n    $ pip install noos-inv\n\nTo enable shell completion, execute the following command (e.g. `zsh`),\n\n    $ noosinv --print-completion-script=zsh\n\nAnd copy/paste its `stdout` into your shell config.\n\n```bash\n# NOOSINV completion script\n\n_complete_noosinv() {\n    collection_arg=\'\'\n    if [[ "${words}" =~ "(-c|--collection) [^ ]+" ]]; then\n        collection_arg=$MATCH\n    fi\n    reply=( $(noosinv ${=collection_arg} --complete -- ${words}) )\n}\n\ncompctl -K _complete_noosinv + -f noosinv\n```\n\nFinally, still in your shell config, enable automatic sub shell loading:\n\n```bash\n# ENV variable sub shell loading with command "source .env"\n\nset -a\n```\n\n## Usage as a command line tool\n\nThe `noos-inv` package installs a CLI binary, for managing common CI/CD tasks.\n\nFrom the terminal,\n\n```\n$ noosinv\n\nUsage: noosinv [--core-opts] <subcommand> [--subcommand-opts] ...\n\nSubcommands:\n\n  docker.build       Build Docker image locally.\n  docker.login       Login to Docker remote registry (AWS ECR or Dockerhub).\n  docker.push        Push Docker image to a remote registry.\n  git.config         Setup git credentials with a Github token.\n  helm.install       Provision local Helm client (Chart Museum Plugin).\n  helm.lint          Check compliance of Helm charts / values.\n  helm.login         Login to Helm remote registry (Chart Museum).\n  helm.push          Push Helm chart to a remote registry.\n  helm.test          Test local deployment in Minikube.\n  local.dotenv       Create local dotenv file.\n  python.clean       Clean project from temp files / dirs.\n  python.coverage    Run coverage test report.\n  python.format      Auto-format source code.\n  python.lint        Run python linters.\n  python.package     Build project wheel distribution.\n  python.release     Publish wheel distribution to PyPi.\n  python.test        Run pytest with optional grouped tests.\n  terraform.run      Run a plan in Terraform cloud.\n  terraform.update   Update variable in Terraform cloud.\n```\n\nSource your environnement variables first for a seamless experience.\n(use command `local.dotenv` to create it from the provided template)\n\n    $ source .env\n\n## Development\n\nOn Mac OSX, make sure [poetry](https://python-poetry.org/) has been installed and pre-configured,\n\n    $ brew install poetry\n\nThis project is shipped with a Makefile, which is ready to do basic common tasks.\n\n```\n$ make\n\nhelp                           Display this auto-generated help message\nupdate                         Lock and install build dependencies\nclean                          Clean project from temp files / dirs\nformat                         Run auto-formatting linters\ninstall                        Install build dependencies from lock file\nlint                           Run python linters\ntest                           Run pytest with all tests\npackage                        Build project wheel distribution\nrelease                        Publish wheel distribution to PyPi\n```\n',
     'author': 'Noos Energy',
     'author_email': 'contact@noos.energy',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/noosenergy/noos-invoke',
```

### Comparing `noos-inv-0.0.8/PKG-INFO` & `noos-inv-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noos-inv
-Version: 0.0.8
+Version: 0.0.9
 Summary: Shared workflows across CI/CD pipelines
 Home-page: https://github.com/noosenergy/noos-invoke
 License: MIT
 Author: Noos Energy
 Author-email: contact@noos.energy
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

