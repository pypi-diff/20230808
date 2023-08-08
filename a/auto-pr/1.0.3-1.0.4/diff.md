# Comparing `tmp/auto_pr-1.0.3.tar.gz` & `tmp/auto_pr-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_pr-1.0.3.tar", max compression
+gzip compressed data, was "auto_pr-1.0.4.tar", max compression
```

## Comparing `auto_pr-1.0.3.tar` & `auto_pr-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-07-24 12:21:10.647512 auto_pr-1.0.3/LICENSE
--rw-r--r--   0        0        0     4455 2023-07-24 12:21:10.647512 auto_pr-1.0.3/README.md
--rw-r--r--   0        0        0     9033 2023-07-24 12:21:10.647512 auto_pr-1.0.3/autopr/__init__.py
--rw-r--r--   0        0        0       63 2023-07-24 12:21:10.647512 auto_pr-1.0.3/autopr/__main__.py
--rw-r--r--   0        0        0     1571 2023-07-24 12:21:10.647512 auto_pr-1.0.3/autopr/config.py
--rw-r--r--   0        0        0     2139 2023-07-24 12:21:10.647512 auto_pr-1.0.3/autopr/database.py
--rw-r--r--   0        0        0     5176 2023-07-24 12:21:10.647512 auto_pr-1.0.3/autopr/github.py
--rw-r--r--   0        0        0     9068 2023-07-24 12:21:10.647512 auto_pr-1.0.3/autopr/repo.py
--rw-r--r--   0        0        0      451 2023-07-24 12:21:10.647512 auto_pr-1.0.3/autopr/util.py
--rw-r--r--   0        0        0     3368 2023-07-24 12:21:10.647512 auto_pr-1.0.3/autopr/workdir.py
--rw-r--r--   0        0        0      792 2023-07-24 12:21:10.647512 auto_pr-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     5439 1970-01-01 00:00:00.000000 auto_pr-1.0.3/setup.py
--rw-r--r--   0        0        0     5321 1970-01-01 00:00:00.000000 auto_pr-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-08 15:02:23.610369 auto_pr-1.0.4/LICENSE
+-rw-r--r--   0        0        0     4401 2023-08-08 15:02:23.610369 auto_pr-1.0.4/README.md
+-rw-r--r--   0        0        0     9524 2023-08-08 15:02:23.614369 auto_pr-1.0.4/autopr/__init__.py
+-rw-r--r--   0        0        0       63 2023-08-08 15:02:23.614369 auto_pr-1.0.4/autopr/__main__.py
+-rw-r--r--   0        0        0     1571 2023-08-08 15:02:23.614369 auto_pr-1.0.4/autopr/config.py
+-rw-r--r--   0        0        0     2683 2023-08-08 15:02:23.614369 auto_pr-1.0.4/autopr/database.py
+-rw-r--r--   0        0        0     5176 2023-08-08 15:02:23.614369 auto_pr-1.0.4/autopr/github.py
+-rw-r--r--   0        0        0     9068 2023-08-08 15:02:23.614369 auto_pr-1.0.4/autopr/repo.py
+-rw-r--r--   0        0        0      451 2023-08-08 15:02:23.614369 auto_pr-1.0.4/autopr/util.py
+-rw-r--r--   0        0        0     3368 2023-08-08 15:02:23.614369 auto_pr-1.0.4/autopr/workdir.py
+-rw-r--r--   0        0        0      792 2023-08-08 15:02:23.614369 auto_pr-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5394 1970-01-01 00:00:00.000000 auto_pr-1.0.4/setup.py
+-rw-r--r--   0        0        0     5267 1970-01-01 00:00:00.000000 auto_pr-1.0.4/PKG-INFO
```

### Comparing `auto_pr-1.0.3/LICENSE` & `auto_pr-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_pr-1.0.3/README.md` & `auto_pr-1.0.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 <img width="128" src="https://github.com/getyourguide/auto-pr/raw/master/img/logo.svg" alt="auto-pr logo" />
 
 ![CI](https://github.com/getyourguide/auto-pr/workflows/CI/badge.svg)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/7db0700cf0b74ac6976e520fbdb92a7f)](https://www.codacy.com/gh/getyourguide/auto-pr/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=getyourguide/auto-pr&amp;utm_campaign=Badge_Grade)
-[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/7db0700cf0b74ac6976e520fbdb92a7f)](https://www.codacy.com/gh/getyourguide/auto-pr/dashboard?utm_source=github.com&utm_medium=referral&utm_content=getyourguide/auto-pr&utm_campaign=Badge_Coverage)
+[![Publish](https://github.com/getyourguide/auto-pr/actions/workflows/publish.yml/badge.svg)](https://github.com/getyourguide/auto-pr/actions/workflows/publish.yml)
 [![PyPI version](https://badge.fury.io/py/auto-pr.svg)](https://badge.fury.io/py/auto-pr)
 ![PyPI downloads](https://img.shields.io/pypi/dm/auto-pr)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # auto-pr
 
 A command line tool to perform bulk updates across multiple GitHub repositories.
@@ -105,14 +104,24 @@
 auto-pr run
 ```
 
 This will perform the changes to a branch on the locally cloned repository and push the branch upstream with the information you provided within `config.yaml`.
 
 See `--help` for more information about other commands and their  usage.
 
+### Reset
+You can reset the list of repos in `db.json` using `auto-pr reset all`, or `auto-pr reset from FILE`
+
+When using `auto-pr reset from FILE`, the list of repos should be provided as a newline separated list of repos like `<owner>/<name>`, e.g:
+
+```text
+getyourguide/test
+getyourguide/auto-pr
+```
+
 ## Security
 
 For sensitive security matters please contact [security@getyourguide.com](mailto:security@getyourguide.com).
 
 ## Legal
 
 Copyright 2021 GetYourGuide GmbH.
```

### Comparing `auto_pr-1.0.3/autopr/__init__.py` & `auto_pr-1.0.4/autopr/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import time
 from pathlib import Path
-from typing import List, Optional
+from typing import Iterator, List, Optional, TextIO
 
 import click
 from single_source import get_version
 
 from autopr import config, database, github, repo, workdir
 from autopr.util import CliException, error, is_debug, set_debug
 
@@ -210,23 +210,40 @@
             change_pushed = repo.push_changes(repository, db, cfg, gh, WORKDIR)
         except CliException as e:
             error(f"Error: {e}")
 
     click.secho(f"Done!", bold=True)
 
 
-@cli.command()
+@cli.group()
 def reset():
+    """Commands for resetting repos to allow for reruns"""
+    pass
+
+
+@reset.command(name="all")
+def reset_all():
     """Mark all mapped repositories as not done"""
     db = workdir.read_database(WORKDIR)
-    db.reset()
+    db.reset_all()
     workdir.write_database(WORKDIR, db)
     click.secho("Repositories marked as not done")
 
 
+@reset.command(
+    name="from", help="reset using a file listing of repos written as <owner>/<name>"
+)
+@click.argument("file", type=click.File("r"))
+def reset_from(file: TextIO):
+    repos: Iterator[str] = map(lambda l: l.strip(), file.readlines())
+    db = workdir.read_database(WORKDIR)
+    db.reset_from(repos)
+    workdir.write_database(WORKDIR, db)
+
+
 def _print_repository_list(
     title: str, repositories: List[database.Repository], total: int
 ):
     click.secho(f"{title} [{len(repositories)}/{total}]:", bold=True)
     for repository in repositories:
         link_str = ""
         if repository.existing_pr is not None:
```

### Comparing `auto_pr-1.0.3/autopr/config.py` & `auto_pr-1.0.4/autopr/config.py`

 * *Files identical despite different names*

### Comparing `auto_pr-1.0.3/autopr/database.py` & `auto_pr-1.0.4/autopr/database.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass, field
-from typing import List, Optional
+from typing import Dict, Iterator, List, Optional
 
 import marshmallow_dataclass
 
 
 @dataclass
 class Repository:
     owner: str
@@ -62,13 +62,26 @@
         new_repos = set(
             (repository.owner, repository.name) for repository in from_db.repositories
         )
         for repository in self.repositories:
             if (repository.owner, repository.name) not in new_repos:
                 repository.removed = True
 
-    def reset(self) -> None:
+    def reset_from(self, selected_repos: Iterator[str]):
+        resets: Dict[str, bool] = {name: False for name in selected_repos}
+        for repository in self.repositories:
+            repo_id = f"{repository.owner}/{repository.name}"
+            if repo_id in resets:
+                print(f"{repo_id} was reset")
+                resets[repo_id] = True
+                repository.done = False
+
+        for name, done in resets.items():
+            if not done:
+                print(f"{name} was not in the database")
+
+    def reset_all(self) -> None:
         for repository in self.repositories:
             repository.done = False
 
 
 DATABASE_SCHEMA = marshmallow_dataclass.class_schema(Database)()
```

### Comparing `auto_pr-1.0.3/autopr/github.py` & `auto_pr-1.0.4/autopr/github.py`

 * *Files identical despite different names*

### Comparing `auto_pr-1.0.3/autopr/repo.py` & `auto_pr-1.0.4/autopr/repo.py`

 * *Files identical despite different names*

### Comparing `auto_pr-1.0.3/autopr/workdir.py` & `auto_pr-1.0.4/autopr/workdir.py`

 * *Files identical despite different names*

### Comparing `auto_pr-1.0.3/pyproject.toml` & `auto_pr-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "auto-pr"
-version = "1.0.3"
+version = "1.0.4"
 description = "Perform bulk updates across repositories"
 license = "Apache-2.0"
 
 authors = ["GetYourGuide GmbH"]
 
 readme = "README.md"
 repository = "https://github.com/getyourguide/auto-pr"
```

### Comparing `auto_pr-1.0.3/setup.py` & `auto_pr-1.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,17 +16,17 @@
  'single-source==0.2.0']
 
 entry_points = \
 {'console_scripts': ['auto-pr = autopr:main']}
 
 setup_kwargs = {
     'name': 'auto-pr',
-    'version': '1.0.3',
+    'version': '1.0.4',
     'description': 'Perform bulk updates across repositories',
-    'long_description': '<img width="128" src="https://github.com/getyourguide/auto-pr/raw/master/img/logo.svg" alt="auto-pr logo" />\n\n![CI](https://github.com/getyourguide/auto-pr/workflows/CI/badge.svg)\n[![Codacy Badge](https://app.codacy.com/project/badge/Grade/7db0700cf0b74ac6976e520fbdb92a7f)](https://www.codacy.com/gh/getyourguide/auto-pr/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=getyourguide/auto-pr&amp;utm_campaign=Badge_Grade)\n[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/7db0700cf0b74ac6976e520fbdb92a7f)](https://www.codacy.com/gh/getyourguide/auto-pr/dashboard?utm_source=github.com&utm_medium=referral&utm_content=getyourguide/auto-pr&utm_campaign=Badge_Coverage)\n[![PyPI version](https://badge.fury.io/py/auto-pr.svg)](https://badge.fury.io/py/auto-pr)\n![PyPI downloads](https://img.shields.io/pypi/dm/auto-pr)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n# auto-pr\n\nA command line tool to perform bulk updates across multiple GitHub repositories.\n\n## How to install\n\nWith [pipx](https://pipxproject.github.io/pipx/) (recommended):\n\n```bash\npipx install auto-pr\n```\nWith pip:\n\n```bash\npip install auto-pr\n```\n\n## Usage\n\n[![Usage](https://github.com/getyourguide/auto-pr/raw/master/img/workflow.svg)](https://github.com/getyourguide/auto-pr/raw/master/img/workflow.svg)\n\n### Init\n\nFirst initialise the project directory by running the `init` command within an empty directory.\n\n```bash\nauto-pr init --api-key=<github_token> --ssh-key-file=<path-to-ssh-key>\n```\n\nWhere `<github_token>` is a GitHub [personal access token](https://github.com/settings/tokens) which has `repo` and `user:user:email` scope.\n\nNext modify the generated `config.yaml` file with your desired configurations.\n\n```yaml\ncredentials:\n  api_key: <github_token>\n  ssh_key_file: /path/to/ssh/key/to/push/.ssh/id_rsa\npr:\n  body: >\n    Body of the PR that will be generated\n\n    Can be multi-line :)\n  branch: auto-pr # The branch name to use when making changes\n  message: Replace default pipelines with modules # Commit message\n  title: \'My awesome change\' # Title of the PR\nrepositories: # Rules that define what repos to update\n  - mode: add\n    match_owner: <org/user>\nupdate_command:\n  - touch\n  - my-file\n```\n\n### Repositories\n\nYou can define the list of repositories to pull and build into the database to update using a list of rules.\n\n-   `mode` - either `add` or `remove` - used to either match or negate\n-   `public` (optional) - pull only public or private, leave out for both\n-   `archived` (optional) -  archived or non-archived, leave out for both\n-   `match_owner` (optional) - the owner or user to pull\n-   `match_name` (optional) - a list of regular expressions to match against to pull\n\nThe flags of the filter rules are optional not specifying will run the command on all repositories that the token has access too.\n\n### Update Command\n\nThis is the list containing the command to be executed along with the arguments passed to it. It will be executed from\nthe root of each repository that is processed.\n\nIf an error occurs during the execution it will be displayed in the output but will not halt the execution.\n\nSee [example commands](docs/examples.md#commands)\n\n### Pull\n\nAfter you have configured the project you can now pull the repositories down that match your rules.\n\n```bash\nauto-pr pull\n```\n\nThis will generate a `db.json` file within your workdir containing a list of mapped repositories and their state.\n\nThis command can be run multiple times, if there are new matching repositories found they will be merged into the existing database.\n\n### Test\n\nOnce the `pull` command has finished setting up the work directory you can now run test to check what the changes that will be made by the script will yield.\n\n### Run\n\nWhen you\'re confident with the changes output from the `test` command you can finally execute `run`.\n\n```bash\nauto-pr run\n```\n\nThis will perform the changes to a branch on the locally cloned repository and push the branch upstream with the information you provided within `config.yaml`.\n\nSee `--help` for more information about other commands and their  usage.\n\n## Security\n\nFor sensitive security matters please contact [security@getyourguide.com](mailto:security@getyourguide.com).\n\n## Legal\n\nCopyright 2021 GetYourGuide GmbH.\n\nauto-pr is licensed under the Apache License, Version 2.0. See [LICENSE](LICENSE) for the full text.\n',
+    'long_description': '<img width="128" src="https://github.com/getyourguide/auto-pr/raw/master/img/logo.svg" alt="auto-pr logo" />\n\n![CI](https://github.com/getyourguide/auto-pr/workflows/CI/badge.svg)\n[![Publish](https://github.com/getyourguide/auto-pr/actions/workflows/publish.yml/badge.svg)](https://github.com/getyourguide/auto-pr/actions/workflows/publish.yml)\n[![PyPI version](https://badge.fury.io/py/auto-pr.svg)](https://badge.fury.io/py/auto-pr)\n![PyPI downloads](https://img.shields.io/pypi/dm/auto-pr)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n# auto-pr\n\nA command line tool to perform bulk updates across multiple GitHub repositories.\n\n## How to install\n\nWith [pipx](https://pipxproject.github.io/pipx/) (recommended):\n\n```bash\npipx install auto-pr\n```\nWith pip:\n\n```bash\npip install auto-pr\n```\n\n## Usage\n\n[![Usage](https://github.com/getyourguide/auto-pr/raw/master/img/workflow.svg)](https://github.com/getyourguide/auto-pr/raw/master/img/workflow.svg)\n\n### Init\n\nFirst initialise the project directory by running the `init` command within an empty directory.\n\n```bash\nauto-pr init --api-key=<github_token> --ssh-key-file=<path-to-ssh-key>\n```\n\nWhere `<github_token>` is a GitHub [personal access token](https://github.com/settings/tokens) which has `repo` and `user:user:email` scope.\n\nNext modify the generated `config.yaml` file with your desired configurations.\n\n```yaml\ncredentials:\n  api_key: <github_token>\n  ssh_key_file: /path/to/ssh/key/to/push/.ssh/id_rsa\npr:\n  body: >\n    Body of the PR that will be generated\n\n    Can be multi-line :)\n  branch: auto-pr # The branch name to use when making changes\n  message: Replace default pipelines with modules # Commit message\n  title: \'My awesome change\' # Title of the PR\nrepositories: # Rules that define what repos to update\n  - mode: add\n    match_owner: <org/user>\nupdate_command:\n  - touch\n  - my-file\n```\n\n### Repositories\n\nYou can define the list of repositories to pull and build into the database to update using a list of rules.\n\n-   `mode` - either `add` or `remove` - used to either match or negate\n-   `public` (optional) - pull only public or private, leave out for both\n-   `archived` (optional) -  archived or non-archived, leave out for both\n-   `match_owner` (optional) - the owner or user to pull\n-   `match_name` (optional) - a list of regular expressions to match against to pull\n\nThe flags of the filter rules are optional not specifying will run the command on all repositories that the token has access too.\n\n### Update Command\n\nThis is the list containing the command to be executed along with the arguments passed to it. It will be executed from\nthe root of each repository that is processed.\n\nIf an error occurs during the execution it will be displayed in the output but will not halt the execution.\n\nSee [example commands](docs/examples.md#commands)\n\n### Pull\n\nAfter you have configured the project you can now pull the repositories down that match your rules.\n\n```bash\nauto-pr pull\n```\n\nThis will generate a `db.json` file within your workdir containing a list of mapped repositories and their state.\n\nThis command can be run multiple times, if there are new matching repositories found they will be merged into the existing database.\n\n### Test\n\nOnce the `pull` command has finished setting up the work directory you can now run test to check what the changes that will be made by the script will yield.\n\n### Run\n\nWhen you\'re confident with the changes output from the `test` command you can finally execute `run`.\n\n```bash\nauto-pr run\n```\n\nThis will perform the changes to a branch on the locally cloned repository and push the branch upstream with the information you provided within `config.yaml`.\n\nSee `--help` for more information about other commands and their  usage.\n\n### Reset\nYou can reset the list of repos in `db.json` using `auto-pr reset all`, or `auto-pr reset from FILE`\n\nWhen using `auto-pr reset from FILE`, the list of repos should be provided as a newline separated list of repos like `<owner>/<name>`, e.g:\n\n```text\ngetyourguide/test\ngetyourguide/auto-pr\n```\n\n## Security\n\nFor sensitive security matters please contact [security@getyourguide.com](mailto:security@getyourguide.com).\n\n## Legal\n\nCopyright 2021 GetYourGuide GmbH.\n\nauto-pr is licensed under the Apache License, Version 2.0. See [LICENSE](LICENSE) for the full text.\n',
     'author': 'GetYourGuide GmbH',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/getyourguide/auto-pr',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `auto_pr-1.0.3/PKG-INFO` & `auto_pr-1.0.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-pr
-Version: 1.0.3
+Version: 1.0.4
 Summary: Perform bulk updates across repositories
 Home-page: https://github.com/getyourguide/auto-pr
 License: Apache-2.0
 Author: GetYourGuide GmbH
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -20,16 +20,15 @@
 Requires-Dist: single-source (==0.2.0)
 Project-URL: Repository, https://github.com/getyourguide/auto-pr
 Description-Content-Type: text/markdown
 
 <img width="128" src="https://github.com/getyourguide/auto-pr/raw/master/img/logo.svg" alt="auto-pr logo" />
 
 ![CI](https://github.com/getyourguide/auto-pr/workflows/CI/badge.svg)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/7db0700cf0b74ac6976e520fbdb92a7f)](https://www.codacy.com/gh/getyourguide/auto-pr/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=getyourguide/auto-pr&amp;utm_campaign=Badge_Grade)
-[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/7db0700cf0b74ac6976e520fbdb92a7f)](https://www.codacy.com/gh/getyourguide/auto-pr/dashboard?utm_source=github.com&utm_medium=referral&utm_content=getyourguide/auto-pr&utm_campaign=Badge_Coverage)
+[![Publish](https://github.com/getyourguide/auto-pr/actions/workflows/publish.yml/badge.svg)](https://github.com/getyourguide/auto-pr/actions/workflows/publish.yml)
 [![PyPI version](https://badge.fury.io/py/auto-pr.svg)](https://badge.fury.io/py/auto-pr)
 ![PyPI downloads](https://img.shields.io/pypi/dm/auto-pr)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # auto-pr
 
 A command line tool to perform bulk updates across multiple GitHub repositories.
@@ -128,14 +127,24 @@
 auto-pr run
 ```
 
 This will perform the changes to a branch on the locally cloned repository and push the branch upstream with the information you provided within `config.yaml`.
 
 See `--help` for more information about other commands and their  usage.
 
+### Reset
+You can reset the list of repos in `db.json` using `auto-pr reset all`, or `auto-pr reset from FILE`
+
+When using `auto-pr reset from FILE`, the list of repos should be provided as a newline separated list of repos like `<owner>/<name>`, e.g:
+
+```text
+getyourguide/test
+getyourguide/auto-pr
+```
+
 ## Security
 
 For sensitive security matters please contact [security@getyourguide.com](mailto:security@getyourguide.com).
 
 ## Legal
 
 Copyright 2021 GetYourGuide GmbH.
```

