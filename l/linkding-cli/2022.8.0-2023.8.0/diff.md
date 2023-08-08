# Comparing `tmp/linkding_cli-2022.8.0.tar.gz` & `tmp/linkding_cli-2023.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkding_cli-2022.8.0.tar", max compression
+gzip compressed data, was "linkding_cli-2023.8.0.tar", max compression
```

## Comparing `linkding_cli-2022.8.0.tar` & `linkding_cli-2023.8.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0     1067 2022-08-04 23:47:33.070871 linkding_cli-2022.8.0/LICENSE
--rw-r--r--   0        0        0    11929 2022-08-04 23:47:33.070871 linkding_cli-2022.8.0/README.md
--rw-r--r--   0        0        0       39 2022-08-04 23:47:33.070871 linkding_cli-2022.8.0/linkding_cli/__init__.py
--rw-r--r--   0        0        0     1425 2022-08-04 23:47:33.070871 linkding_cli-2022.8.0/linkding_cli/cli.py
--rw-r--r--   0        0        0       23 2022-08-04 23:47:33.070871 linkding_cli-2022.8.0/linkding_cli/commands/__init__.py
--rw-r--r--   0        0        0     6643 2022-08-04 23:47:33.070871 linkding_cli-2022.8.0/linkding_cli/commands/bookmark.py
--rw-r--r--   0        0        0     1632 2022-08-04 23:47:33.070871 linkding_cli-2022.8.0/linkding_cli/commands/tag.py
--rw-r--r--   0        0        0     2274 2022-08-04 23:47:33.070871 linkding_cli-2022.8.0/linkding_cli/config.py
--rw-r--r--   0        0        0      282 2022-08-04 23:47:33.070871 linkding_cli-2022.8.0/linkding_cli/const.py
--rw-r--r--   0        0        0      912 2022-08-04 23:47:33.070871 linkding_cli-2022.8.0/linkding_cli/core.py
--rw-r--r--   0        0        0      224 2022-08-04 23:47:33.070871 linkding_cli-2022.8.0/linkding_cli/errors.py
--rw-r--r--   0        0        0       22 2022-08-04 23:47:33.070871 linkding_cli-2022.8.0/linkding_cli/helpers/__init__.py
--rw-r--r--   0        0        0     1710 2022-08-04 23:47:33.070871 linkding_cli-2022.8.0/linkding_cli/helpers/logging.py
--rw-r--r--   0        0        0        0 2022-08-04 23:47:33.070871 linkding_cli-2022.8.0/linkding_cli/py.typed
--rw-r--r--   0        0        0      364 2022-08-04 23:47:33.070871 linkding_cli-2022.8.0/linkding_cli/util/__init__.py
--rw-r--r--   0        0        0     3051 2022-08-04 23:47:33.070871 linkding_cli-2022.8.0/pyproject.toml
--rw-r--r--   0        0        0    13318 2022-08-04 23:47:46.763260 linkding_cli-2022.8.0/setup.py
--rw-r--r--   0        0        0    12859 2022-08-04 23:47:46.764196 linkding_cli-2022.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-08-08 16:55:23.960150 linkding_cli-2023.8.0/LICENSE
+-rw-r--r--   0        0        0    12557 2023-08-08 16:55:23.960150 linkding_cli-2023.8.0/README.md
+-rw-r--r--   0        0        0       39 2023-08-08 16:55:23.960150 linkding_cli-2023.8.0/linkding_cli/__init__.py
+-rw-r--r--   0        0        0     1724 2023-08-08 16:55:23.960150 linkding_cli-2023.8.0/linkding_cli/cli.py
+-rw-r--r--   0        0        0       23 2023-08-08 16:55:23.960150 linkding_cli-2023.8.0/linkding_cli/commands/__init__.py
+-rw-r--r--   0        0        0     8782 2023-08-08 16:55:23.960150 linkding_cli-2023.8.0/linkding_cli/commands/bookmark.py
+-rw-r--r--   0        0        0     2008 2023-08-08 16:55:23.960150 linkding_cli-2023.8.0/linkding_cli/commands/tag.py
+-rw-r--r--   0        0        0     2662 2023-08-08 16:55:23.960150 linkding_cli-2023.8.0/linkding_cli/config.py
+-rw-r--r--   0        0        0      328 2023-08-08 16:55:23.960150 linkding_cli-2023.8.0/linkding_cli/const.py
+-rw-r--r--   0        0        0      977 2023-08-08 16:55:23.960150 linkding_cli-2023.8.0/linkding_cli/core.py
+-rw-r--r--   0        0        0      224 2023-08-08 16:55:23.960150 linkding_cli-2023.8.0/linkding_cli/errors.py
+-rw-r--r--   0        0        0       22 2023-08-08 16:55:23.960150 linkding_cli-2023.8.0/linkding_cli/helpers/__init__.py
+-rw-r--r--   0        0        0     2447 2023-08-08 16:55:23.960150 linkding_cli-2023.8.0/linkding_cli/helpers/logging.py
+-rw-r--r--   0        0        0        0 2023-08-08 16:55:23.960150 linkding_cli-2023.8.0/linkding_cli/py.typed
+-rw-r--r--   0        0        0      485 2023-08-08 16:55:23.960150 linkding_cli-2023.8.0/linkding_cli/util/__init__.py
+-rw-r--r--   0        0        0     3736 2023-08-08 16:55:23.964151 linkding_cli-2023.8.0/pyproject.toml
+-rw-r--r--   0        0        0    13630 1970-01-01 00:00:00.000000 linkding_cli-2023.8.0/PKG-INFO
```

### Comparing `linkding_cli-2022.8.0/LICENSE` & `linkding_cli-2023.8.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Aaron Bach
+Copyright (c) 2021-2022 Aaron Bach
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `linkding_cli-2022.8.0/README.md` & `linkding_cli-2023.8.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,56 @@
 # 🔖 linkding-cli: A CLI to interact with a linkding instance
 
-[![CI](https://github.com/bachya/linkding-cli/workflows/CI/badge.svg)](https://github.com/bachya/linkding-cli/actions)
-[![PyPi](https://img.shields.io/pypi/v/linkding-cli.svg)](https://pypi.python.org/pypi/linkding-cli)
-[![Version](https://img.shields.io/pypi/pyversions/linkding-cli.svg)](https://pypi.python.org/pypi/linkding-cli)
-[![License](https://img.shields.io/pypi/l/linkding-cli.svg)](https://github.com/bachya/linkding-cli/blob/master/LICENSE)
-[![Code Coverage](https://codecov.io/gh/bachya/linkding-cli/branch/master/graph/badge.svg)](https://codecov.io/gh/bachya/linkding-cli)
-[![Maintainability](https://api.codeclimate.com/v1/badges/f01be3cd230902508636/maintainability)](https://codeclimate.com/github/bachya/linkding-cli/maintainability)
-[![Say Thanks](https://img.shields.io/badge/SayThanks-!-1EAEDB.svg)](https://saythanks.io/to/bachya)
+[![CI][ci-badge]][ci]
+[![PyPI][pypi-badge]][pypi]
+[![Version][version-badge]][version]
+[![License][license-badge]][license]
+[![Code Coverage][codecov-badge]][codecov]
+[![Maintainability][maintainability-badge]][maintainability]
 
-`linkding-cli` is a CLI to interact with a
-[linkding](https://github.com/sissbruecker/linkding) instance.
+`linkding-cli` is a CLI to interact with a [linkding][linkding] instance.
 
 - [Installation](#installation)
 - [Python Versions](#python-versions)
 - [Usage](#usage)
-  * [Main Help](#main-help)
-  * [Configuration](#configuration)
-    + [Example: CLI Options](#example--cli-options)
-    + [Example: Environment Variables](#example--environment-variables)
-    + [Example: Configuration File](#example--configuration-file)
-    + [Merging Configuration Options](#merging-configuration-options)
-  * [Bookmarks](#bookmarks)
-    + [The `bookmarks all` command](#the-bookmarks-all-command)
-    + [The `bookmarks archive` command](#the-bookmarks-archive-command)
-    + [The `bookmarks create` command](#the-bookmarks-create-command)
-    + [The `bookmarks delete` command](#the-bookmarks-delete-command)
-    + [The `bookmarks get` command](#the-bookmarks-get-command)
-    + [The `bookmarks unarchive` command](#the-bookmarks-unarchive-command)
-    + [The `bookmarks update` command](#the-bookmarks-update-command)
-  * [Tags](#tags)
-    + [The `tags all` command](#the-tags-all-command)
-    + [The `tags create` command](#the-tags-create-command)
-    + [The `tags get` command](#the-tags-get-command)
-  * [Misc.](#misc)
-    + [Parsing and Pretty Printing Data](#parsing-and-pretty-printing-data)
+  - [Main Help](#main-help)
+  - [Configuration](#configuration)
+    - [Example: CLI Options](#example--cli-options)
+    - [Example: Environment Variables](#example--environment-variables)
+    - [Example: Configuration File](#example--configuration-file)
+    - [Merging Configuration Options](#merging-configuration-options)
+  - [Bookmarks](#bookmarks)
+    - [The `bookmarks all` command](#the-bookmarks-all-command)
+    - [The `bookmarks archive` command](#the-bookmarks-archive-command)
+    - [The `bookmarks create` command](#the-bookmarks-create-command)
+    - [The `bookmarks delete` command](#the-bookmarks-delete-command)
+    - [The `bookmarks get` command](#the-bookmarks-get-command)
+    - [The `bookmarks unarchive` command](#the-bookmarks-unarchive-command)
+    - [The `bookmarks update` command](#the-bookmarks-update-command)
+  - [Tags](#tags)
+    - [The `tags all` command](#the-tags-all-command)
+    - [The `tags create` command](#the-tags-create-command)
+    - [The `tags get` command](#the-tags-get-command)
+  - [Misc.](#misc)
+    - [Parsing and Pretty Printing Data](#parsing-and-pretty-printing-data)
 - [Contributing](#contributing)
 
 # Installation
 
-```python
+```bash
 pip install linkding-cli
 ```
 
 # Python Versions
 
 `linkding-cli` is currently supported on:
 
-* Python 3.8
-* Python 3.9
-* Python 3.10
+- Python 3.9
+- Python 3.10
+- Python 3.11
 
 # Usage
 
 ## Main Help
 
 ```
 $ linkding --help
@@ -69,23 +67,23 @@
   --show-completion     Show completion for the current shell, to copy it or
                         customize the installation.
   --help                Show this message and exit.
 
 Commands:
   bookmarks  Work with bookmarks.
   tags       Work with tags.
-  ```
+```
 
 ## Configuration
 
 Configuration can be provided via a variety of sources:
 
-* CLI Options
-* Environment Variables
-* Configuration File
+- CLI Options
+- Environment Variables
+- Configuration File
 
 ### Example: CLI Options
 
 ```
 $ linkding -u http://127.0.0.1:8000 -t abcde12345 ...
 ```
 
@@ -148,30 +146,30 @@
   all        Get all bookmarks.
   archive    Archive a bookmark by its linkding ID.
   create     Create a bookmark.
   delete     Delete a bookmark by its linkding ID.
   get        Get a bookmark by its linkding ID.
   unarchive  Unarchive a bookmark by its linkding ID.
   update     Update a bookmark by its linkding ID.
-  ```
+```
 
 ### The `bookmarks all` command
 
 ```
 Usage: linkding bookmarks all [OPTIONS]
 
   Get all bookmarks.
 
 Options:
   -a, --archived        Return archived bookmarks.
   -l, --limit INTEGER   The number of bookmarks to return.
   -o, --offset INTEGER  The index from which to return results.
   -q, --query TEXT      Return bookmarks containing a query string.
   --help                Show this message and exit.
-  ```
+```
 
 #### Examples:
 
 ```sh
 # Get all bookmarks, but limit the results to 10:
 $ linkding bookmarks all --limit 10
 
@@ -187,15 +185,15 @@
   Archive a bookmark by its linkding ID.
 
 Arguments:
   [BOOKMARK_ID]  The ID of a bookmark to archive.
 
 Options:
   --help  Show this message and exit.
-  ```
+```
 
 #### Examples:
 
 ```sh
 # Archive bookmark 12:
 $ linkding bookmarks archive 12
 ```
@@ -210,22 +208,23 @@
 Arguments:
   URL  The URL to bookmark.  [required]
 
 Options:
   -a, --archived                 Whether the newly-created bookmark should be
                                  immediately archived.
   -d, --description DESCRIPTION  The description to give the bookmark.
+  -n, --notes NOTES              Any Markdown-formatted notes to add to the bookmark.
   --shared                       Whether the newly-created bookmark should be
                                  shareable with other linkding users
   --tags TAG1,TAG2,...           The tags to apply to the bookmark.
   -t, --title TITLE              The title to give the bookmark.
   --unread                       Whether the newly-created bookmark should be
                                  marked as unread.
   --help                         Show this message and exit.
-  ```
+```
 
 #### Examples:
 
 ```sh
 # Create a bookmark:
 $ linkding bookmarks create https://example.com
 
@@ -244,15 +243,15 @@
   Delete a bookmark by its linkding ID.
 
 Arguments:
   [BOOKMARK_ID]  The ID of a bookmark to delete.
 
 Options:
   --help  Show this message and exit.
-  ```
+```
 
 #### Examples:
 
 ```sh
 # Delete the bookmark with an ID of 12:
 $ linkding bookmarks delete 12
 ```
@@ -265,15 +264,15 @@
   Get a bookmark by its linkding ID.
 
 Arguments:
   [BOOKMARK_ID]  The ID of a bookmark to retrieve.
 
 Options:
   --help  Show this message and exit.
-  ```
+```
 
 #### Examples:
 
 ```sh
 # Get bookmark 12:
 $ linkding bookmarks get 12
 ```
@@ -286,15 +285,15 @@
   Unarchive a bookmark by its linkding ID.
 
 Arguments:
   [BOOKMARK_ID]  The ID of a bookmark to unarchive.
 
 Options:
   --help  Show this message and exit.
-  ```
+```
 
 #### Examples:
 
 ```sh
 # Unarchive bookmark 12:
 $ linkding bookmarks unarchive 12
 ```
@@ -308,14 +307,15 @@
 
 Arguments:
   BOOKMARK_ID  The ID of a bookmark to update.  [required]
 
 Options:
   -u, --url URL                  The URL to assign to the bookmark.
   -d, --description DESCRIPTION  The description to give the bookmark.
+  -n, --notes NOTES              Any Markdown-formatted notes to add to the bookmark.
   --shared                       Whether the -created bookmark should be
                                  shareable with other linkding users
   --tags TAG1,TAG2,...           The tags to apply to the bookmark.
   -t, --title TITLE              The title to give the bookmark.
   --unread                       Whether the bookmark should be marked as
                                  unread.
   --help                         Show this message and exit.
@@ -341,28 +341,28 @@
 Options:
   --help  Show this message and exit.
 
 Commands:
   all     Get all tags.
   create  Create a tag.
   get     Get a tag by its linkding ID.
-  ```
+```
 
 ### The `tags all` command
 
 ```
 Usage: linkding tags all [OPTIONS]
 
   Get all tags.
 
 Options:
   -l, --limit INTEGER   The number of tags to return.
   -o, --offset INTEGER  The index from which to return results.
   --help                Show this message and exit.
-  ```
+```
 
 #### Examples:
 
 ```sh
 # Get all tags, but limit the results to 10:
 $ linkding tags all --limit 10
 ```
@@ -375,15 +375,15 @@
   Create a tag.
 
 Arguments:
   TAG_NAME  The tag to create.  [required]
 
 Options:
   --help  Show this message and exit.
-  ```
+```
 
 #### Examples:
 
 ```sh
 # Create a tag:
 $ linkding tags create sample-tag
 ```
@@ -396,30 +396,30 @@
   Get a tag by its linkding ID.
 
 Arguments:
   TAG_ID  The ID of a tag to retrieve.  [required]
 
 Options:
   --help  Show this message and exit.
-  ```
+```
 
 #### Examples:
 
 ```sh
 # Get tag 12:
 $ linkding tags get 12
 ```
 
 ## Misc.
 
 ### Parsing and Pretty Printing Data
 
 `linkding-cli` doesn't have built-in utilities for modifying JSON output in any way.
-Instead, it's recommended to use a tool like [`jq`](https://stedolan.github.io/jq/).
-This allows for multiple new outcomes, like pretty-printing:
+Instead, it's recommended to use a tool like [`jq`][jq]. This allows for multiple new
+outcomes, like pretty-printing:
 
 ```
 $ linkding bookmarks all | jq
 {
   "count": 123,
   "next": "http://127.0.0.1:8000/api/bookmarks/?limit=100&offset=100",
   "previous": null,
@@ -447,19 +447,39 @@
 ```
 $ linkding bookmarks all | jq '.results[0].title'
 "Example title"
 ```
 
 # Contributing
 
-1. [Check for open features/bugs](https://github.com/bachya/linkding-cli/issues)
-  or [initiate a discussion on one](https://github.com/bachya/linkding-cli/issues/new).
-2. [Fork the repository](https://github.com/bachya/linkding-cli/fork).
+Thanks to all of [our contributors][contributors] so far!
+
+1. [Check for open features/bugs][issues] or [initiate a discussion on one][new-issue].
+2. [Fork the repository][fork].
 3. (_optional, but highly recommended_) Create a virtual environment: `python3 -m venv .venv`
 4. (_optional, but highly recommended_) Enter the virtual environment: `source ./.venv/bin/activate`
 5. Install the dev environment: `script/setup`
-6. Code your new feature or bug fix.
+6. Code your new feature or bug fix on a new branch.
 7. Write tests that cover your new functionality.
-8. Run tests and ensure 100% code coverage: `nox -rs coverage`
+8. Run tests and ensure 100% code coverage: `poetry run pytest --cov linkding_cli tests`
 9. Update `README.md` with any new documentation.
-10. Add yourself to `AUTHORS.md`.
-11. Submit a pull request!
+10. Submit a pull request!
+
+[ci-badge]: https://github.com/bachya/linkding-cli/workflows/CI/badge.svg
+[ci]: https://github.com/bachya/linkding-cli/actions
+[codecov-badge]: https://codecov.io/gh/bachya/linkding-cli/branch/dev/graph/badge.svg
+[codecov]: https://codecov.io/gh/bachya/linkding-cli
+[contributors]: https://github.com/bachya/linkding-cli/graphs/contributors
+[fork]: https://github.com/bachya/linkding-cli/fork
+[issues]: https://github.com/bachya/linkding-cli/issues
+[jq]: https://stedolan.github.io/jq/
+[license-badge]: https://img.shields.io/pypi/l/linkding-cli.svg
+[license]: https://github.com/bachya/linkding-cli/blob/main/LICENSE
+[linkding]: https://github.com/sissbruecker/linkding
+[maintainability-badge]: https://api.codeclimate.com/v1/badges/f01be3cd230902508636/maintainability
+[maintainability]: https://codeclimate.com/github/bachya/linkding-cli/maintainability
+[new-issue]: https://github.com/bachya/linkding-cli/issues/new
+[new-issue]: https://github.com/bachya/linkding-cli/issues/new
+[pypi-badge]: https://img.shields.io/pypi/v/linkding-cli.svg
+[pypi]: https://pypi.python.org/pypi/linkding-cli
+[version-badge]: https://img.shields.io/pypi/pyversions/linkding-cli.svg
+[version]: https://pypi.python.org/pypi/linkding-cli
```

### Comparing `linkding_cli-2022.8.0/linkding_cli/cli.py` & `linkding_cli-2023.8.0/linkding_cli/cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 """Define the main interface to the CLI."""
+# pylint: disable=unused-argument
+from __future__ import annotations
+
 from pathlib import Path
 
 import typer
 
 from linkding_cli.commands.bookmark import BOOKMARK_APP
 from linkding_cli.commands.tag import TAG_APP
 from linkding_cli.const import ENV_CONFIG, ENV_TOKEN, ENV_URL
@@ -44,14 +47,22 @@
     verbose: bool = typer.Option(
         False,
         "--verbose",
         "-v",
         help="Increase verbosity of standard output.",
     ),
 ) -> None:
-    """Interact with a linkding instance."""
+    """Interact with a linkding instance.
+
+    Args:
+        ctx: A Typer Context object.
+        config: A path to a config file
+        token: A linkding API token.
+        url: A URL to a linkding instance.
+        verbose: Increase verbosity of standard output.
+    """
     ctx.obj = LinkDing(ctx)
 
 
 APP = typer.Typer(callback=main)
 APP.add_typer(BOOKMARK_APP, name="bookmarks", help="Work with bookmarks.")
 APP.add_typer(TAG_APP, name="tags", help="Work with tags.")
```

### Comparing `linkding_cli-2022.8.0/linkding_cli/commands/tag.py` & `linkding_cli-2023.8.0/linkding_cli/commands/tag.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Define the tag command."""
+from __future__ import annotations
+
 import asyncio
 import json
 
 import typer
 
 from linkding_cli.const import CONF_LIMIT, CONF_OFFSET
 from linkding_cli.helpers.logging import log_exception
@@ -10,15 +12,20 @@
 
 
 @log_exception()
 def create(
     ctx: typer.Context,
     tag_name: str = typer.Argument(..., help="The tag to create."),
 ) -> None:
-    """Create a tag."""
+    """Create a tag.
+
+    Args:
+        ctx: A Typer Context object.
+        tag_name: The tag to create.
+    """
     data = asyncio.run(ctx.obj.client.tags.async_create(tag_name))
     typer.echo(json.dumps(data))
 
 
 @log_exception()
 def get_all(
     ctx: typer.Context,
@@ -31,15 +38,21 @@
     offset: int = typer.Option(
         None,
         "--offset",
         "-o",
         help="The index from which to return results.",
     ),
 ) -> None:
-    """Get all tags."""
+    """Get all tags.
+
+    Args:
+        ctx: A Typer Context object.
+        limit: The number of tags to return.
+        offset: The index from which to return results.
+    """
     api_kwargs = generate_api_payload(
         (
             (CONF_LIMIT, limit),
             (CONF_OFFSET, offset),
         )
     )
 
@@ -48,21 +61,26 @@
 
 
 @log_exception()
 def get_by_id(
     ctx: typer.Context,
     tag_id: int = typer.Argument(..., help="The ID of a tag to retrieve."),
 ) -> None:
-    """Get a tag by its linkding ID."""
+    """Get a tag by its linkding ID.
+
+    Args:
+        ctx: A Typer Context object.
+        tag_id: The ID of a tag to retrieve.
+    """
     data = asyncio.run(ctx.obj.client.tags.async_get_single(tag_id))
     typer.echo(json.dumps(data))
 
 
 @log_exception()
-def main(ctx: typer.Context) -> None:
+def main(_: typer.Context) -> None:
     """Interact with tags."""
     pass
 
 
 TAG_APP = typer.Typer(callback=main)
 TAG_APP.command(name="all")(get_all)
 TAG_APP.command(name="create")(create)
```

### Comparing `linkding_cli-2022.8.0/linkding_cli/config.py` & `linkding_cli-2023.8.0/linkding_cli/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 """Define configuration management."""
 from __future__ import annotations
 
 from typing import cast
 
-from ruamel.yaml import YAML
 import typer
+from ruamel.yaml import YAML
 
 from linkding_cli.const import CONF_TOKEN, CONF_URL, CONF_VERBOSE, LOGGER
 from linkding_cli.errors import ConfigError
 
 CONF_CONFIG = "config"
 
 
 class Config:
     """Define the config manager object."""
 
     def __init__(self, ctx: typer.Context) -> None:
-        """Initialize."""
+        """Initialize.
+
+        Args:
+            ctx: A Typer Context object.
+
+        Raises:
+            ConfigError: Raised upon invalid config
+        """
         LOGGER.debug("Command: %s", ctx.invoked_subcommand)
         LOGGER.debug("Arguments: %s", ctx.args)
         LOGGER.debug("Options: %s", ctx.params)
 
         self._config = {}
 
         # If the user provides a config file, attempt to load it:
@@ -44,24 +51,40 @@
         for param in (CONF_TOKEN, CONF_URL):
             if not self._config[param]:
                 raise ConfigError(f"Missing required option: --{param}")
 
         LOGGER.debug("Loaded Config: %s", self)
 
     def __str__(self) -> str:
-        """Define the string representation."""
+        """Define the string representation.
+
+        Returns:
+            A string representation.
+        """
         return f"<Config token={self.token} url={self.url} verbose={self.verbose}>"
 
     @property
     def token(self) -> str:
-        """Return the linkding token."""
+        """Return the linkding API token.
+
+        Returns:
+            The linkding API token.
+        """
         return cast(str, self._config[CONF_TOKEN])
 
     @property
     def url(self) -> str:
-        """Return the linkding URL."""
+        """Return the linkding URL.
+
+        Returns:
+            The linkding API token.
+        """
         return cast(str, self._config[CONF_URL])
 
     @property
     def verbose(self) -> bool:
-        """Return the verbosity level."""
+        """Return the verbosity level.
+
+        Returns:
+            The verbosity level.
+        """
         return cast(bool, self._config[CONF_VERBOSE])
```

### Comparing `linkding_cli-2022.8.0/linkding_cli/core.py` & `linkding_cli-2023.8.0/linkding_cli/core.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 """Define a data object."""
 from __future__ import annotations
 
 import logging
 
-from aiolinkding import Client
 import typer
+from aiolinkding import Client
 
 from linkding_cli.config import Config
 from linkding_cli.const import CONF_VERBOSE
 from linkding_cli.helpers.logging import TyperLoggerHandler
 
 
 class LinkDing:  # pylint: disable=too-few-public-methods
     """Define a master linkding manager object."""
 
     def __init__(self, ctx: typer.Context) -> None:
-        """Initialize."""
+        """Initialize.
+
+        Args:
+            ctx: A Typer Context object.
+        """
         if ctx.params[CONF_VERBOSE]:
             log_level = logging.DEBUG
         else:
             log_level = logging.INFO
 
         typer_handler = TyperLoggerHandler()
         logging.basicConfig(
```

### Comparing `linkding_cli-2022.8.0/linkding_cli/helpers/logging.py` & `linkding_cli-2023.8.0/linkding_cli/helpers/logging.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,86 @@
 """Define logging helpers."""
 from __future__ import annotations
 
-from functools import wraps
 import logging
 import traceback
-from typing import Any, Callable, TypeVar
+from collections.abc import Callable
+from functools import wraps
+from typing import Any, TypeVar, cast
 
 import typer
 
 from linkding_cli.const import LOGGER
 
-T = TypeVar("T")
-
 
 class TyperLoggerHandler(logging.Handler):
     """Define a logging handler that works with Typer."""
 
     def emit(self, record: logging.LogRecord) -> None:
-        """Emit a log record."""
+        """Emit a log record.
+
+        Args:
+            record: The log record.
+        """
         foreground = None
         if record.levelno == logging.CRITICAL:
             foreground = typer.colors.BRIGHT_RED
         elif record.levelno == logging.DEBUG:
             foreground = typer.colors.BRIGHT_BLUE
         elif record.levelno == logging.ERROR:
             foreground = typer.colors.BRIGHT_RED
         elif record.levelno == logging.INFO:
             foreground = typer.colors.BRIGHT_GREEN
         elif record.levelno == logging.WARNING:
             foreground = typer.colors.BRIGHT_YELLOW
         typer.secho(self.format(record), fg=foreground)
 
 
+_T = TypeVar("_T")
+_CallableThatFailsType = Callable[..., _T]
+
+
 def log_exception(
     *, exit_code: int = 1
-) -> Callable[[Callable[..., T]], Callable[..., T]]:
-    """Define a dectorator to handle exceptions via typer output."""
+) -> Callable[[_CallableThatFailsType], _CallableThatFailsType]:
+    """Define a dectorator to handle exceptions via typer output.
 
-    def decorator(func: Callable[..., T]) -> Callable[..., T]:
-        """Decorate."""
+    Args:
+        exit_code: The code to exit with upon exception.
+
+    Returns:
+        The decorated callable.
+    """
+
+    def decorator(func: _CallableThatFailsType) -> _CallableThatFailsType:
+        """Decorate.
+
+        Args:
+            func: The callable to decorate.
+
+        Returns:
+            The decorated callable.
+        """
 
         @wraps(func)
-        def wrapper(*args: Any, **kwargs: dict[str, Any]) -> T:
-            """Wrap."""
+        def wrapper(*args: Any, **kwargs: dict[str, Any]) -> dict[str, Any]:
+            """Wrap.
+
+            Args:
+                args: The callable's arguments.
+                kwargs: The callable's keyword arguments.
+
+            Returns:
+                The original callable's return type.
+
+            Raises:
+                Exit: Raised when the command fails in any way.
+            """
             try:
-                return func(*args, **kwargs)
+                return cast(dict[str, Any], func(*args, **kwargs))
             except Exception as err:  # pylint: disable=broad-except
                 LOGGER.error(err)
                 LOGGER.debug("".join(traceback.format_tb(err.__traceback__)))
                 raise typer.Exit(code=exit_code) from err
 
         return wrapper
```

### Comparing `linkding_cli-2022.8.0/PKG-INFO` & `linkding_cli-2023.8.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,81 +1,81 @@
 Metadata-Version: 2.1
 Name: linkding-cli
-Version: 2022.8.0
+Version: 2023.8.0
 Summary: A CLI to interact with a linkding instance
 Home-page: https://github.com/bachya/linkding-cli
 License: MIT
 Author: Aaron Bach
 Author-email: bachya1208@gmail.com
-Requires-Python: >=3.8.0,<4.0.0
+Requires-Python: >=3.9.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Dist: aiolinkding (>=2022.8.0)
+Requires-Dist: aiolinkding (>=2023.01.0)
 Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
-Requires-Dist: typer[all] (>=0.6.0,<0.7.0)
+Requires-Dist: typer[all] (>=0.6,<0.10)
+Project-URL: Bug Tracker, https://github.com/bachya/linkding_cli/issues
+Project-URL: Changelog, https://github.com/bachya/linkding_cli/releases
 Project-URL: Repository, https://github.com/bachya/linkding-cli
 Description-Content-Type: text/markdown
 
 # 🔖 linkding-cli: A CLI to interact with a linkding instance
 
-[![CI](https://github.com/bachya/linkding-cli/workflows/CI/badge.svg)](https://github.com/bachya/linkding-cli/actions)
-[![PyPi](https://img.shields.io/pypi/v/linkding-cli.svg)](https://pypi.python.org/pypi/linkding-cli)
-[![Version](https://img.shields.io/pypi/pyversions/linkding-cli.svg)](https://pypi.python.org/pypi/linkding-cli)
-[![License](https://img.shields.io/pypi/l/linkding-cli.svg)](https://github.com/bachya/linkding-cli/blob/master/LICENSE)
-[![Code Coverage](https://codecov.io/gh/bachya/linkding-cli/branch/master/graph/badge.svg)](https://codecov.io/gh/bachya/linkding-cli)
-[![Maintainability](https://api.codeclimate.com/v1/badges/f01be3cd230902508636/maintainability)](https://codeclimate.com/github/bachya/linkding-cli/maintainability)
-[![Say Thanks](https://img.shields.io/badge/SayThanks-!-1EAEDB.svg)](https://saythanks.io/to/bachya)
+[![CI][ci-badge]][ci]
+[![PyPI][pypi-badge]][pypi]
+[![Version][version-badge]][version]
+[![License][license-badge]][license]
+[![Code Coverage][codecov-badge]][codecov]
+[![Maintainability][maintainability-badge]][maintainability]
 
-`linkding-cli` is a CLI to interact with a
-[linkding](https://github.com/sissbruecker/linkding) instance.
+`linkding-cli` is a CLI to interact with a [linkding][linkding] instance.
 
 - [Installation](#installation)
 - [Python Versions](#python-versions)
 - [Usage](#usage)
-  * [Main Help](#main-help)
-  * [Configuration](#configuration)
-    + [Example: CLI Options](#example--cli-options)
-    + [Example: Environment Variables](#example--environment-variables)
-    + [Example: Configuration File](#example--configuration-file)
-    + [Merging Configuration Options](#merging-configuration-options)
-  * [Bookmarks](#bookmarks)
-    + [The `bookmarks all` command](#the-bookmarks-all-command)
-    + [The `bookmarks archive` command](#the-bookmarks-archive-command)
-    + [The `bookmarks create` command](#the-bookmarks-create-command)
-    + [The `bookmarks delete` command](#the-bookmarks-delete-command)
-    + [The `bookmarks get` command](#the-bookmarks-get-command)
-    + [The `bookmarks unarchive` command](#the-bookmarks-unarchive-command)
-    + [The `bookmarks update` command](#the-bookmarks-update-command)
-  * [Tags](#tags)
-    + [The `tags all` command](#the-tags-all-command)
-    + [The `tags create` command](#the-tags-create-command)
-    + [The `tags get` command](#the-tags-get-command)
-  * [Misc.](#misc)
-    + [Parsing and Pretty Printing Data](#parsing-and-pretty-printing-data)
+  - [Main Help](#main-help)
+  - [Configuration](#configuration)
+    - [Example: CLI Options](#example--cli-options)
+    - [Example: Environment Variables](#example--environment-variables)
+    - [Example: Configuration File](#example--configuration-file)
+    - [Merging Configuration Options](#merging-configuration-options)
+  - [Bookmarks](#bookmarks)
+    - [The `bookmarks all` command](#the-bookmarks-all-command)
+    - [The `bookmarks archive` command](#the-bookmarks-archive-command)
+    - [The `bookmarks create` command](#the-bookmarks-create-command)
+    - [The `bookmarks delete` command](#the-bookmarks-delete-command)
+    - [The `bookmarks get` command](#the-bookmarks-get-command)
+    - [The `bookmarks unarchive` command](#the-bookmarks-unarchive-command)
+    - [The `bookmarks update` command](#the-bookmarks-update-command)
+  - [Tags](#tags)
+    - [The `tags all` command](#the-tags-all-command)
+    - [The `tags create` command](#the-tags-create-command)
+    - [The `tags get` command](#the-tags-get-command)
+  - [Misc.](#misc)
+    - [Parsing and Pretty Printing Data](#parsing-and-pretty-printing-data)
 - [Contributing](#contributing)
 
 # Installation
 
-```python
+```bash
 pip install linkding-cli
 ```
 
 # Python Versions
 
 `linkding-cli` is currently supported on:
 
-* Python 3.8
-* Python 3.9
-* Python 3.10
+- Python 3.9
+- Python 3.10
+- Python 3.11
 
 # Usage
 
 ## Main Help
 
 ```
 $ linkding --help
@@ -92,23 +92,23 @@
   --show-completion     Show completion for the current shell, to copy it or
                         customize the installation.
   --help                Show this message and exit.
 
 Commands:
   bookmarks  Work with bookmarks.
   tags       Work with tags.
-  ```
+```
 
 ## Configuration
 
 Configuration can be provided via a variety of sources:
 
-* CLI Options
-* Environment Variables
-* Configuration File
+- CLI Options
+- Environment Variables
+- Configuration File
 
 ### Example: CLI Options
 
 ```
 $ linkding -u http://127.0.0.1:8000 -t abcde12345 ...
 ```
 
@@ -171,30 +171,30 @@
   all        Get all bookmarks.
   archive    Archive a bookmark by its linkding ID.
   create     Create a bookmark.
   delete     Delete a bookmark by its linkding ID.
   get        Get a bookmark by its linkding ID.
   unarchive  Unarchive a bookmark by its linkding ID.
   update     Update a bookmark by its linkding ID.
-  ```
+```
 
 ### The `bookmarks all` command
 
 ```
 Usage: linkding bookmarks all [OPTIONS]
 
   Get all bookmarks.
 
 Options:
   -a, --archived        Return archived bookmarks.
   -l, --limit INTEGER   The number of bookmarks to return.
   -o, --offset INTEGER  The index from which to return results.
   -q, --query TEXT      Return bookmarks containing a query string.
   --help                Show this message and exit.
-  ```
+```
 
 #### Examples:
 
 ```sh
 # Get all bookmarks, but limit the results to 10:
 $ linkding bookmarks all --limit 10
 
@@ -210,15 +210,15 @@
   Archive a bookmark by its linkding ID.
 
 Arguments:
   [BOOKMARK_ID]  The ID of a bookmark to archive.
 
 Options:
   --help  Show this message and exit.
-  ```
+```
 
 #### Examples:
 
 ```sh
 # Archive bookmark 12:
 $ linkding bookmarks archive 12
 ```
@@ -233,22 +233,23 @@
 Arguments:
   URL  The URL to bookmark.  [required]
 
 Options:
   -a, --archived                 Whether the newly-created bookmark should be
                                  immediately archived.
   -d, --description DESCRIPTION  The description to give the bookmark.
+  -n, --notes NOTES              Any Markdown-formatted notes to add to the bookmark.
   --shared                       Whether the newly-created bookmark should be
                                  shareable with other linkding users
   --tags TAG1,TAG2,...           The tags to apply to the bookmark.
   -t, --title TITLE              The title to give the bookmark.
   --unread                       Whether the newly-created bookmark should be
                                  marked as unread.
   --help                         Show this message and exit.
-  ```
+```
 
 #### Examples:
 
 ```sh
 # Create a bookmark:
 $ linkding bookmarks create https://example.com
 
@@ -267,15 +268,15 @@
   Delete a bookmark by its linkding ID.
 
 Arguments:
   [BOOKMARK_ID]  The ID of a bookmark to delete.
 
 Options:
   --help  Show this message and exit.
-  ```
+```
 
 #### Examples:
 
 ```sh
 # Delete the bookmark with an ID of 12:
 $ linkding bookmarks delete 12
 ```
@@ -288,15 +289,15 @@
   Get a bookmark by its linkding ID.
 
 Arguments:
   [BOOKMARK_ID]  The ID of a bookmark to retrieve.
 
 Options:
   --help  Show this message and exit.
-  ```
+```
 
 #### Examples:
 
 ```sh
 # Get bookmark 12:
 $ linkding bookmarks get 12
 ```
@@ -309,15 +310,15 @@
   Unarchive a bookmark by its linkding ID.
 
 Arguments:
   [BOOKMARK_ID]  The ID of a bookmark to unarchive.
 
 Options:
   --help  Show this message and exit.
-  ```
+```
 
 #### Examples:
 
 ```sh
 # Unarchive bookmark 12:
 $ linkding bookmarks unarchive 12
 ```
@@ -331,14 +332,15 @@
 
 Arguments:
   BOOKMARK_ID  The ID of a bookmark to update.  [required]
 
 Options:
   -u, --url URL                  The URL to assign to the bookmark.
   -d, --description DESCRIPTION  The description to give the bookmark.
+  -n, --notes NOTES              Any Markdown-formatted notes to add to the bookmark.
   --shared                       Whether the -created bookmark should be
                                  shareable with other linkding users
   --tags TAG1,TAG2,...           The tags to apply to the bookmark.
   -t, --title TITLE              The title to give the bookmark.
   --unread                       Whether the bookmark should be marked as
                                  unread.
   --help                         Show this message and exit.
@@ -364,28 +366,28 @@
 Options:
   --help  Show this message and exit.
 
 Commands:
   all     Get all tags.
   create  Create a tag.
   get     Get a tag by its linkding ID.
-  ```
+```
 
 ### The `tags all` command
 
 ```
 Usage: linkding tags all [OPTIONS]
 
   Get all tags.
 
 Options:
   -l, --limit INTEGER   The number of tags to return.
   -o, --offset INTEGER  The index from which to return results.
   --help                Show this message and exit.
-  ```
+```
 
 #### Examples:
 
 ```sh
 # Get all tags, but limit the results to 10:
 $ linkding tags all --limit 10
 ```
@@ -398,15 +400,15 @@
   Create a tag.
 
 Arguments:
   TAG_NAME  The tag to create.  [required]
 
 Options:
   --help  Show this message and exit.
-  ```
+```
 
 #### Examples:
 
 ```sh
 # Create a tag:
 $ linkding tags create sample-tag
 ```
@@ -419,30 +421,30 @@
   Get a tag by its linkding ID.
 
 Arguments:
   TAG_ID  The ID of a tag to retrieve.  [required]
 
 Options:
   --help  Show this message and exit.
-  ```
+```
 
 #### Examples:
 
 ```sh
 # Get tag 12:
 $ linkding tags get 12
 ```
 
 ## Misc.
 
 ### Parsing and Pretty Printing Data
 
 `linkding-cli` doesn't have built-in utilities for modifying JSON output in any way.
-Instead, it's recommended to use a tool like [`jq`](https://stedolan.github.io/jq/).
-This allows for multiple new outcomes, like pretty-printing:
+Instead, it's recommended to use a tool like [`jq`][jq]. This allows for multiple new
+outcomes, like pretty-printing:
 
 ```
 $ linkding bookmarks all | jq
 {
   "count": 123,
   "next": "http://127.0.0.1:8000/api/bookmarks/?limit=100&offset=100",
   "previous": null,
@@ -470,20 +472,40 @@
 ```
 $ linkding bookmarks all | jq '.results[0].title'
 "Example title"
 ```
 
 # Contributing
 
-1. [Check for open features/bugs](https://github.com/bachya/linkding-cli/issues)
-  or [initiate a discussion on one](https://github.com/bachya/linkding-cli/issues/new).
-2. [Fork the repository](https://github.com/bachya/linkding-cli/fork).
+Thanks to all of [our contributors][contributors] so far!
+
+1. [Check for open features/bugs][issues] or [initiate a discussion on one][new-issue].
+2. [Fork the repository][fork].
 3. (_optional, but highly recommended_) Create a virtual environment: `python3 -m venv .venv`
 4. (_optional, but highly recommended_) Enter the virtual environment: `source ./.venv/bin/activate`
 5. Install the dev environment: `script/setup`
-6. Code your new feature or bug fix.
+6. Code your new feature or bug fix on a new branch.
 7. Write tests that cover your new functionality.
-8. Run tests and ensure 100% code coverage: `nox -rs coverage`
+8. Run tests and ensure 100% code coverage: `poetry run pytest --cov linkding_cli tests`
 9. Update `README.md` with any new documentation.
-10. Add yourself to `AUTHORS.md`.
-11. Submit a pull request!
+10. Submit a pull request!
+
+[ci-badge]: https://github.com/bachya/linkding-cli/workflows/CI/badge.svg
+[ci]: https://github.com/bachya/linkding-cli/actions
+[codecov-badge]: https://codecov.io/gh/bachya/linkding-cli/branch/dev/graph/badge.svg
+[codecov]: https://codecov.io/gh/bachya/linkding-cli
+[contributors]: https://github.com/bachya/linkding-cli/graphs/contributors
+[fork]: https://github.com/bachya/linkding-cli/fork
+[issues]: https://github.com/bachya/linkding-cli/issues
+[jq]: https://stedolan.github.io/jq/
+[license-badge]: https://img.shields.io/pypi/l/linkding-cli.svg
+[license]: https://github.com/bachya/linkding-cli/blob/main/LICENSE
+[linkding]: https://github.com/sissbruecker/linkding
+[maintainability-badge]: https://api.codeclimate.com/v1/badges/f01be3cd230902508636/maintainability
+[maintainability]: https://codeclimate.com/github/bachya/linkding-cli/maintainability
+[new-issue]: https://github.com/bachya/linkding-cli/issues/new
+[new-issue]: https://github.com/bachya/linkding-cli/issues/new
+[pypi-badge]: https://img.shields.io/pypi/v/linkding-cli.svg
+[pypi]: https://pypi.python.org/pypi/linkding-cli
+[version-badge]: https://img.shields.io/pypi/pyversions/linkding-cli.svg
+[version]: https://pypi.python.org/pypi/linkding-cli
```

