# Comparing `tmp/cobib-4.1.0.tar.gz` & `tmp/cobib-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cobib-4.1.0.tar", last modified: Sun Jun 11 11:20:21 2023, max compression
+gzip compressed data, was "cobib-4.2.0.tar", last modified: Tue Aug  8 18:43:43 2023, max compression
```

## Comparing `cobib-4.1.0.tar` & `cobib-4.2.0.tar`

### file list

```diff
@@ -1,180 +1,94 @@
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.174786 cobib-4.1.0/
--rw-r--r--   0 max       (1000) max       (1000)      217 2021-09-20 21:31:31.000000 cobib-4.1.0/.coveragerc
--rw-r--r--   0 max       (1000) max       (1000)      268 2023-04-15 10:28:42.000000 cobib-4.1.0/.gitignore
--rw-r--r--   0 max       (1000) max       (1000)     2718 2023-05-27 21:00:12.000000 cobib-4.1.0/.gitlab-ci.yml
--rw-r--r--   0 max       (1000) max       (1000)       75 2023-05-27 21:00:12.000000 cobib-4.1.0/.pydocstylerc
--rw-r--r--   0 max       (1000) max       (1000)      924 2023-06-07 20:33:04.000000 cobib-4.1.0/.pylintdict
--rw-r--r--   0 max       (1000) max       (1000)    11236 2023-04-15 10:28:42.000000 cobib-4.1.0/.pylintrc
--rw-r--r--   0 max       (1000) max       (1000)    31219 2023-06-11 11:18:49.000000 cobib-4.1.0/CHANGELOG.md
--rw-r--r--   0 max       (1000) max       (1000)     2247 2023-05-27 21:00:12.000000 cobib-4.1.0/CONTRIBUTING.md
--rw-r--r--   0 max       (1000) max       (1000)     1076 2023-05-27 21:00:12.000000 cobib-4.1.0/LICENSE.txt
--rw-r--r--   0 max       (1000) max       (1000)      100 2023-05-27 21:00:12.000000 cobib-4.1.0/MANIFEST.in
--rw-r--r--   0 max       (1000) max       (1000)      105 2023-05-27 21:00:12.000000 cobib-4.1.0/Makefile
--rw-r--r--   0 max       (1000) max       (1000)    40072 2023-06-11 11:20:21.174786 cobib-4.1.0/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)     7843 2023-05-27 21:00:12.000000 cobib-4.1.0/README.md
--rw-r--r--   0 max       (1000) max       (1000)    27762 2023-06-11 11:18:21.000000 cobib-4.1.0/cobib.1
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.131452 cobib-4.1.0/html/
--rw-r--r--   0 max       (1000) max       (1000)    34915 2023-05-07 10:49:25.000000 cobib-4.1.0/html/cobib_book.svg
--rw-r--r--   0 max       (1000) max       (1000)    61955 2023-05-07 10:49:25.000000 cobib-4.1.0/html/cobib_logo.svg
--rw-r--r--   0 max       (1000) max       (1000)      554 2023-05-27 21:00:12.000000 cobib-4.1.0/html/index.html.jinja2
--rw-r--r--   0 max       (1000) max       (1000)      398 2023-05-20 15:19:20.000000 cobib-4.1.0/html/module.html.jinja2
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.134786 cobib-4.1.0/logo/
--rw-r--r--   0 max       (1000) max       (1000)    44669 2021-09-20 21:31:31.000000 cobib-4.1.0/logo/cobib_book-squared.png
--rw-r--r--   0 max       (1000) max       (1000)    40896 2021-09-20 21:31:31.000000 cobib-4.1.0/logo/cobib_book.png
--rw-r--r--   0 max       (1000) max       (1000)    34915 2021-09-20 21:31:31.000000 cobib-4.1.0/logo/cobib_book.svg
--rw-r--r--   0 max       (1000) max       (1000)    74851 2021-09-20 21:31:31.000000 cobib-4.1.0/logo/cobib_byline.png
--rw-r--r--   0 max       (1000) max       (1000)    27555 2021-09-20 21:31:31.000000 cobib-4.1.0/logo/cobib_byline.svg
--rw-r--r--   0 max       (1000) max       (1000)   126027 2021-09-20 21:31:31.000000 cobib-4.1.0/logo/cobib_logo.png
--rw-r--r--   0 max       (1000) max       (1000)    61955 2021-09-20 21:31:31.000000 cobib-4.1.0/logo/cobib_logo.svg
--rw-r--r--   0 max       (1000) max       (1000)      507 2023-05-27 21:00:12.000000 cobib-4.1.0/mypy.ini
--rw-r--r--   0 max       (1000) max       (1000)      356 2023-05-27 21:00:12.000000 cobib-4.1.0/pyproject.toml
--rw-r--r--   0 max       (1000) max       (1000)       27 2021-09-20 21:31:31.000000 cobib-4.1.0/pytest.ini
--rw-r--r--   0 max       (1000) max       (1000)      120 2023-06-06 19:52:56.000000 cobib-4.1.0/requirements.txt
--rw-r--r--   0 max       (1000) max       (1000)     1221 2023-06-11 11:20:21.174786 cobib-4.1.0/setup.cfg
--rw-r--r--   0 max       (1000) max       (1000)      296 2021-09-20 21:31:31.000000 cobib-4.1.0/setup.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.118119 cobib-4.1.0/src/
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.138119 cobib-4.1.0/src/cobib/
--rw-r--r--   0 max       (1000) max       (1000)      474 2023-06-11 11:18:13.000000 cobib-4.1.0/src/cobib/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      648 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/__main__.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.141453 cobib-4.1.0/src/cobib/commands/
--rw-r--r--   0 max       (1000) max       (1000)      903 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/commands/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)    22162 2023-06-11 11:12:00.000000 cobib-4.1.0/src/cobib/commands/add.py
--rw-r--r--   0 max       (1000) max       (1000)     7858 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/commands/base_command.py
--rw-r--r--   0 max       (1000) max       (1000)     7187 2023-06-05 20:50:22.000000 cobib-4.1.0/src/cobib/commands/delete.py
--rw-r--r--   0 max       (1000) max       (1000)     8026 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/commands/edit.py
--rw-r--r--   0 max       (1000) max       (1000)     7759 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/commands/export.py
--rw-r--r--   0 max       (1000) max       (1000)     7284 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/commands/import_.py
--rw-r--r--   0 max       (1000) max       (1000)     4805 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/commands/init.py
--rw-r--r--   0 max       (1000) max       (1000)    13208 2023-06-06 19:25:20.000000 cobib-4.1.0/src/cobib/commands/list_.py
--rw-r--r--   0 max       (1000) max       (1000)    18390 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/commands/modify.py
--rw-r--r--   0 max       (1000) max       (1000)     9080 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/commands/open.py
--rw-r--r--   0 max       (1000) max       (1000)     4791 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/commands/redo.py
--rw-r--r--   0 max       (1000) max       (1000)    10393 2023-06-05 20:50:22.000000 cobib-4.1.0/src/cobib/commands/search.py
--rw-r--r--   0 max       (1000) max       (1000)     2388 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/commands/show.py
--rw-r--r--   0 max       (1000) max       (1000)     5488 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/commands/undo.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.141453 cobib-4.1.0/src/cobib/config/
--rw-r--r--   0 max       (1000) max       (1000)     1210 2022-01-13 20:47:42.000000 cobib-4.1.0/src/cobib/config/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)    27574 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/config/config.py
--rw-r--r--   0 max       (1000) max       (1000)    29728 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/config/event.py
--rw-r--r--   0 max       (1000) max       (1000)     9145 2023-06-06 19:19:55.000000 cobib-4.1.0/src/cobib/config/example.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.141453 cobib-4.1.0/src/cobib/database/
--rw-r--r--   0 max       (1000) max       (1000)      283 2021-09-20 21:31:31.000000 cobib-4.1.0/src/cobib/database/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)    10104 2023-06-10 21:09:16.000000 cobib-4.1.0/src/cobib/database/database.py
--rw-r--r--   0 max       (1000) max       (1000)    17670 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/database/entry.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.144786 cobib-4.1.0/src/cobib/importers/
--rw-r--r--   0 max       (1000) max       (1000)      275 2021-12-01 20:44:34.000000 cobib-4.1.0/src/cobib/importers/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     3086 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/importers/base_importer.py
--rw-r--r--   0 max       (1000) max       (1000)    12878 2023-06-11 11:12:00.000000 cobib-4.1.0/src/cobib/importers/zotero.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.144786 cobib-4.1.0/src/cobib/parsers/
--rw-r--r--   0 max       (1000) max       (1000)      520 2021-09-25 22:36:09.000000 cobib-4.1.0/src/cobib/parsers/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     5019 2023-06-06 20:01:42.000000 cobib-4.1.0/src/cobib/parsers/arxiv.py
--rw-r--r--   0 max       (1000) max       (1000)     2053 2021-09-20 21:31:31.000000 cobib-4.1.0/src/cobib/parsers/base_parser.py
--rw-r--r--   0 max       (1000) max       (1000)     2994 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/parsers/bibtex.py
--rw-r--r--   0 max       (1000) max       (1000)     3267 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/parsers/doi.py
--rw-r--r--   0 max       (1000) max       (1000)     4559 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/parsers/isbn.py
--rw-r--r--   0 max       (1000) max       (1000)     3522 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/parsers/url.py
--rw-r--r--   0 max       (1000) max       (1000)     2996 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/parsers/yaml.py
--rw-r--r--   0 max       (1000) max       (1000)        0 2021-09-20 21:31:31.000000 cobib-4.1.0/src/cobib/py.typed
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.148119 cobib-4.1.0/src/cobib/ui/
--rw-r--r--   0 max       (1000) max       (1000)      611 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/ui/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     3391 2023-06-06 19:41:19.000000 cobib-4.1.0/src/cobib/ui/cli.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.151453 cobib-4.1.0/src/cobib/ui/components/
--rw-r--r--   0 max       (1000) max       (1000)     1163 2023-06-05 20:50:22.000000 cobib-4.1.0/src/cobib/ui/components/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     1448 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/ui/components/argument_parser.py
--rw-r--r--   0 max       (1000) max       (1000)      705 2023-06-05 20:50:22.000000 cobib-4.1.0/src/cobib/ui/components/entry_view.py
--rw-r--r--   0 max       (1000) max       (1000)     2946 2023-06-05 20:50:22.000000 cobib-4.1.0/src/cobib/ui/components/help_screen.py
--rw-r--r--   0 max       (1000) max       (1000)     2865 2023-06-05 20:50:22.000000 cobib-4.1.0/src/cobib/ui/components/input_screen.py
--rw-r--r--   0 max       (1000) max       (1000)     2935 2023-06-05 20:50:22.000000 cobib-4.1.0/src/cobib/ui/components/list_view.py
--rw-r--r--   0 max       (1000) max       (1000)     2120 2023-06-05 21:09:33.000000 cobib-4.1.0/src/cobib/ui/components/main_content.py
--rw-r--r--   0 max       (1000) max       (1000)      565 2023-06-05 20:50:22.000000 cobib-4.1.0/src/cobib/ui/components/motion_key.py
--rw-r--r--   0 max       (1000) max       (1000)     2035 2023-06-07 18:57:00.000000 cobib-4.1.0/src/cobib/ui/components/popup.py
--rw-r--r--   0 max       (1000) max       (1000)     1405 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/ui/components/popup_logging_handler.py
--rw-r--r--   0 max       (1000) max       (1000)      668 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/ui/components/popup_panel.py
--rw-r--r--   0 max       (1000) max       (1000)     2054 2023-06-11 11:12:00.000000 cobib-4.1.0/src/cobib/ui/components/progress.py
--rw-r--r--   0 max       (1000) max       (1000)     3313 2023-06-05 20:50:22.000000 cobib-4.1.0/src/cobib/ui/components/prompt.py
--rw-r--r--   0 max       (1000) max       (1000)     2890 2023-06-05 20:50:22.000000 cobib-4.1.0/src/cobib/ui/components/search_view.py
--rw-r--r--   0 max       (1000) max       (1000)     1415 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/ui/components/selection_filter.py
--rw-r--r--   0 max       (1000) max       (1000)     1733 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/ui/shell_helper.py
--rw-r--r--   0 max       (1000) max       (1000)    18572 2023-06-11 11:12:00.000000 cobib-4.1.0/src/cobib/ui/tui.py
--rw-r--r--   0 max       (1000) max       (1000)     4273 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/ui/ui.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.151453 cobib-4.1.0/src/cobib/utils/
--rw-r--r--   0 max       (1000) max       (1000)      242 2021-09-20 21:31:31.000000 cobib-4.1.0/src/cobib/utils/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     6731 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/utils/diff_renderer.py
--rw-r--r--   0 max       (1000) max       (1000)     8237 2023-06-11 11:12:00.000000 cobib-4.1.0/src/cobib/utils/file_downloader.py
--rw-r--r--   0 max       (1000) max       (1000)     4533 2021-09-20 21:32:23.000000 cobib-4.1.0/src/cobib/utils/journal_abbreviations.py
--rw-r--r--   0 max       (1000) max       (1000)     4505 2023-06-06 19:45:15.000000 cobib-4.1.0/src/cobib/utils/logging.py
--rw-r--r--   0 max       (1000) max       (1000)     1837 2021-09-20 21:31:31.000000 cobib-4.1.0/src/cobib/utils/rel_path.py
--rw-r--r--   0 max       (1000) max       (1000)     8644 2023-05-27 21:00:12.000000 cobib-4.1.0/src/cobib/utils/shell_helper.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.138119 cobib-4.1.0/src/cobib.egg-info/
--rw-r--r--   0 max       (1000) max       (1000)    40072 2023-06-11 11:20:21.000000 cobib-4.1.0/src/cobib.egg-info/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)     4344 2023-06-11 11:20:21.000000 cobib-4.1.0/src/cobib.egg-info/SOURCES.txt
--rw-r--r--   0 max       (1000) max       (1000)        1 2023-06-11 11:20:21.000000 cobib-4.1.0/src/cobib.egg-info/dependency_links.txt
--rw-r--r--   0 max       (1000) max       (1000)       47 2023-06-11 11:20:21.000000 cobib-4.1.0/src/cobib.egg-info/entry_points.txt
--rw-r--r--   0 max       (1000) max       (1000)      120 2023-06-11 11:20:21.000000 cobib-4.1.0/src/cobib.egg-info/requires.txt
--rw-r--r--   0 max       (1000) max       (1000)        6 2023-06-11 11:20:21.000000 cobib-4.1.0/src/cobib.egg-info/top_level.txt
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.158119 cobib-4.1.0/tests/
--rw-r--r--   0 max       (1000) max       (1000)     1508 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      872 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/cmdline_test.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.164786 cobib-4.1.0/tests/commands/
--rw-r--r--   0 max       (1000) max       (1000)       68 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/commands/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     5878 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/commands/command_test.py
--rw-r--r--   0 max       (1000) max       (1000)      248 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/commands/example_duplicate_entry.bib
--rw-r--r--   0 max       (1000) max       (1000)      261 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/commands/example_duplicate_entry.yaml
--rw-r--r--   0 max       (1000) max       (1000)      134 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/commands/example_multi_file_entry.bib
--rw-r--r--   0 max       (1000) max       (1000)      155 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/commands/example_multi_file_entry.yaml
--rw-r--r--   0 max       (1000) max       (1000)    24454 2023-06-06 20:01:35.000000 cobib-4.1.0/tests/commands/test_add.py
--rw-r--r--   0 max       (1000) max       (1000)     8961 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/commands/test_delete.py
--rw-r--r--   0 max       (1000) max       (1000)     7992 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/commands/test_edit.py
--rw-r--r--   0 max       (1000) max       (1000)     8218 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/commands/test_export.py
--rw-r--r--   0 max       (1000) max       (1000)     3077 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/commands/test_git_commit_event.py
--rw-r--r--   0 max       (1000) max       (1000)     2167 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/commands/test_import.py
--rw-r--r--   0 max       (1000) max       (1000)     6102 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/commands/test_init.py
--rw-r--r--   0 max       (1000) max       (1000)    10180 2023-06-06 19:28:09.000000 cobib-4.1.0/tests/commands/test_list.py
--rw-r--r--   0 max       (1000) max       (1000)     9207 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/commands/test_modify.py
--rw-r--r--   0 max       (1000) max       (1000)    14520 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/commands/test_open.py
--rw-r--r--   0 max       (1000) max       (1000)     8550 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/commands/test_redo.py
--rw-r--r--   0 max       (1000) max       (1000)     8095 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/commands/test_search.py
--rw-r--r--   0 max       (1000) max       (1000)     4232 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/commands/test_show.py
--rw-r--r--   0 max       (1000) max       (1000)     7831 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/commands/test_undo.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.168119 cobib-4.1.0/tests/config/
--rw-r--r--   0 max       (1000) max       (1000)       28 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/config/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      147 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/config/broken_config.py
--rw-r--r--   0 max       (1000) max       (1000)     3312 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/config/test_config.py
--rw-r--r--   0 max       (1000) max       (1000)     2401 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/config/test_event.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.168119 cobib-4.1.0/tests/database/
--rw-r--r--   0 max       (1000) max       (1000)       30 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/database/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)       59 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/database/example_entry_umlaut.bib
--rw-r--r--   0 max       (1000) max       (1000)     8158 2023-06-10 20:57:45.000000 cobib-4.1.0/tests/database/test_database.py
--rw-r--r--   0 max       (1000) max       (1000)    14623 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/database/test_entry.py
--rw-r--r--   0 max       (1000) max       (1000)      444 2023-06-06 19:45:30.000000 cobib-4.1.0/tests/debug.py
--rw-r--r--   0 max       (1000) max       (1000)      651 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/example_entry.bib
--rw-r--r--   0 max       (1000) max       (1000)      621 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/example_entry.yaml
--rw-r--r--   0 max       (1000) max       (1000)      723 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/example_literature.bib
--rw-r--r--   0 max       (1000) max       (1000)      636 2023-06-10 21:12:23.000000 cobib-4.1.0/tests/example_literature.yaml
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.168119 cobib-4.1.0/tests/importers/
--rw-r--r--   0 max       (1000) max       (1000)       71 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/importers/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      274 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/importers/importer_test.py
--rw-r--r--   0 max       (1000) max       (1000)     4801 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/importers/test_zotero.py
--rw-r--r--   0 max       (1000) max       (1000)     2609 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/importers/zotero_database.yaml
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.171453 cobib-4.1.0/tests/parsers/
--rw-r--r--   0 max       (1000) max       (1000)       65 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/parsers/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     1395 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/parsers/parser_test.py
--rw-r--r--   0 max       (1000) max       (1000)     5763 2023-06-06 19:54:06.000000 cobib-4.1.0/tests/parsers/test_arxiv.py
--rw-r--r--   0 max       (1000) max       (1000)     3224 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/parsers/test_bibtex.py
--rw-r--r--   0 max       (1000) max       (1000)     5017 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/parsers/test_doi.py
--rw-r--r--   0 max       (1000) max       (1000)     5562 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/parsers/test_isbn.py
--rw-r--r--   0 max       (1000) max       (1000)     4374 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/parsers/test_url.py
--rw-r--r--   0 max       (1000) max       (1000)     3251 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/parsers/test_yaml.py
--rw-r--r--   0 max       (1000) max       (1000)     4353 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/test_main.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-11 11:20:21.174786 cobib-4.1.0/tests/utils/
--rw-r--r--   0 max       (1000) max       (1000)       29 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/utils/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      172 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/utils/fixed_database.yaml
--rw-r--r--   0 max       (1000) max       (1000)      163 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/utils/linting_database.yaml
--rw-r--r--   0 max       (1000) max       (1000)     8992 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/utils/test_file_downloader.py
--rw-r--r--   0 max       (1000) max       (1000)     3216 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/utils/test_journal_abbreviations.py
--rw-r--r--   0 max       (1000) max       (1000)     2990 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/utils/test_logging.py
--rw-r--r--   0 max       (1000) max       (1000)      964 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/utils/test_rel_path.py
--rw-r--r--   0 max       (1000) max       (1000)    13535 2023-05-27 21:00:12.000000 cobib-4.1.0/tests/utils/test_shell_helper.py
--rw-r--r--   0 max       (1000) max       (1000)     1909 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/utils/unified_database.yaml
--rw-r--r--   0 max       (1000) max       (1000)     1907 2023-05-07 10:49:48.000000 cobib-4.1.0/tests/utils/unifying_database.yaml
--rw-r--r--   0 max       (1000) max       (1000)     1287 2023-05-27 21:00:12.000000 cobib-4.1.0/tox.ini
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-08-08 18:43:43.093316 cobib-4.2.0/
+-rw-r--r--   0 max       (1000) max       (1000)    33108 2023-08-07 21:59:56.000000 cobib-4.2.0/CHANGELOG.md
+-rw-r--r--   0 max       (1000) max       (1000)     1076 2023-06-12 19:22:05.000000 cobib-4.2.0/LICENSE.txt
+-rw-r--r--   0 max       (1000) max       (1000)      100 2023-06-12 19:22:05.000000 cobib-4.2.0/MANIFEST.in
+-rw-r--r--   0 max       (1000) max       (1000)    41961 2023-08-08 18:43:43.096649 cobib-4.2.0/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)     7843 2023-06-12 19:22:05.000000 cobib-4.2.0/README.md
+-rw-r--r--   0 max       (1000) max       (1000)    30376 2023-08-07 21:59:19.000000 cobib-4.2.0/cobib.1
+-rw-r--r--   0 max       (1000) max       (1000)      356 2023-06-12 19:22:05.000000 cobib-4.2.0/pyproject.toml
+-rw-r--r--   0 max       (1000) max       (1000)      135 2023-07-31 20:26:36.000000 cobib-4.2.0/requirements.txt
+-rw-r--r--   0 max       (1000) max       (1000)     1221 2023-08-08 18:43:43.096649 cobib-4.2.0/setup.cfg
+-rw-r--r--   0 max       (1000) max       (1000)      296 2023-06-12 19:22:05.000000 cobib-4.2.0/setup.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-08-08 18:43:43.063316 cobib-4.2.0/src/
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-08-08 18:43:43.066649 cobib-4.2.0/src/cobib/
+-rw-r--r--   0 max       (1000) max       (1000)      474 2023-08-07 21:58:54.000000 cobib-4.2.0/src/cobib/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      648 2023-06-12 19:22:05.000000 cobib-4.2.0/src/cobib/__main__.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-08-08 18:43:43.076649 cobib-4.2.0/src/cobib/commands/
+-rw-r--r--   0 max       (1000) max       (1000)      903 2023-06-12 19:22:05.000000 cobib-4.2.0/src/cobib/commands/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)    22211 2023-07-31 19:52:43.000000 cobib-4.2.0/src/cobib/commands/add.py
+-rw-r--r--   0 max       (1000) max       (1000)     7888 2023-06-20 19:36:56.000000 cobib-4.2.0/src/cobib/commands/base_command.py
+-rw-r--r--   0 max       (1000) max       (1000)     7239 2023-06-20 19:36:56.000000 cobib-4.2.0/src/cobib/commands/delete.py
+-rw-r--r--   0 max       (1000) max       (1000)     8056 2023-06-20 19:36:56.000000 cobib-4.2.0/src/cobib/commands/edit.py
+-rw-r--r--   0 max       (1000) max       (1000)     7789 2023-06-20 19:36:56.000000 cobib-4.2.0/src/cobib/commands/export.py
+-rw-r--r--   0 max       (1000) max       (1000)     7314 2023-06-20 19:36:56.000000 cobib-4.2.0/src/cobib/commands/import_.py
+-rw-r--r--   0 max       (1000) max       (1000)     4835 2023-06-20 19:36:56.000000 cobib-4.2.0/src/cobib/commands/init.py
+-rw-r--r--   0 max       (1000) max       (1000)    13302 2023-08-06 20:32:54.000000 cobib-4.2.0/src/cobib/commands/list_.py
+-rw-r--r--   0 max       (1000) max       (1000)    18950 2023-08-01 19:25:04.000000 cobib-4.2.0/src/cobib/commands/modify.py
+-rw-r--r--   0 max       (1000) max       (1000)    10566 2023-07-31 19:15:00.000000 cobib-4.2.0/src/cobib/commands/open.py
+-rw-r--r--   0 max       (1000) max       (1000)     4821 2023-06-20 19:36:56.000000 cobib-4.2.0/src/cobib/commands/redo.py
+-rw-r--r--   0 max       (1000) max       (1000)    10811 2023-08-06 20:46:40.000000 cobib-4.2.0/src/cobib/commands/search.py
+-rw-r--r--   0 max       (1000) max       (1000)     2418 2023-08-06 17:42:26.000000 cobib-4.2.0/src/cobib/commands/show.py
+-rw-r--r--   0 max       (1000) max       (1000)     5518 2023-06-20 19:36:56.000000 cobib-4.2.0/src/cobib/commands/undo.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-08-08 18:43:43.076649 cobib-4.2.0/src/cobib/config/
+-rw-r--r--   0 max       (1000) max       (1000)     1253 2023-08-06 20:32:54.000000 cobib-4.2.0/src/cobib/config/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)    35304 2023-08-07 21:10:12.000000 cobib-4.2.0/src/cobib/config/config.py
+-rw-r--r--   0 max       (1000) max       (1000)    29758 2023-06-20 19:36:56.000000 cobib-4.2.0/src/cobib/config/event.py
+-rw-r--r--   0 max       (1000) max       (1000)    11046 2023-08-06 20:32:54.000000 cobib-4.2.0/src/cobib/config/example.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-08-08 18:43:43.079982 cobib-4.2.0/src/cobib/database/
+-rw-r--r--   0 max       (1000) max       (1000)      283 2023-06-12 19:22:05.000000 cobib-4.2.0/src/cobib/database/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)    11018 2023-08-07 21:26:46.000000 cobib-4.2.0/src/cobib/database/database.py
+-rw-r--r--   0 max       (1000) max       (1000)    18672 2023-08-06 20:48:54.000000 cobib-4.2.0/src/cobib/database/entry.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-08-08 18:43:43.079982 cobib-4.2.0/src/cobib/importers/
+-rw-r--r--   0 max       (1000) max       (1000)      275 2023-06-12 19:22:05.000000 cobib-4.2.0/src/cobib/importers/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     3116 2023-06-20 19:36:56.000000 cobib-4.2.0/src/cobib/importers/base_importer.py
+-rw-r--r--   0 max       (1000) max       (1000)    12908 2023-06-20 19:36:56.000000 cobib-4.2.0/src/cobib/importers/zotero.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-08-08 18:43:43.083316 cobib-4.2.0/src/cobib/parsers/
+-rw-r--r--   0 max       (1000) max       (1000)      520 2023-06-12 19:22:05.000000 cobib-4.2.0/src/cobib/parsers/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     5098 2023-08-07 22:17:27.000000 cobib-4.2.0/src/cobib/parsers/arxiv.py
+-rw-r--r--   0 max       (1000) max       (1000)     2053 2023-06-12 19:22:05.000000 cobib-4.2.0/src/cobib/parsers/base_parser.py
+-rw-r--r--   0 max       (1000) max       (1000)     3077 2023-08-06 17:41:53.000000 cobib-4.2.0/src/cobib/parsers/bibtex.py
+-rw-r--r--   0 max       (1000) max       (1000)     3725 2023-08-07 21:47:52.000000 cobib-4.2.0/src/cobib/parsers/doi.py
+-rw-r--r--   0 max       (1000) max       (1000)     4638 2023-07-31 19:36:29.000000 cobib-4.2.0/src/cobib/parsers/isbn.py
+-rw-r--r--   0 max       (1000) max       (1000)     3552 2023-06-20 19:36:56.000000 cobib-4.2.0/src/cobib/parsers/url.py
+-rw-r--r--   0 max       (1000) max       (1000)     3466 2023-08-07 21:30:51.000000 cobib-4.2.0/src/cobib/parsers/yaml.py
+-rw-r--r--   0 max       (1000) max       (1000)        0 2023-06-12 19:22:05.000000 cobib-4.2.0/src/cobib/py.typed
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-08-08 18:43:43.086649 cobib-4.2.0/src/cobib/ui/
+-rw-r--r--   0 max       (1000) max       (1000)      611 2023-06-12 19:22:05.000000 cobib-4.2.0/src/cobib/ui/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     3447 2023-08-06 20:32:54.000000 cobib-4.2.0/src/cobib/ui/cli.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-08-08 18:43:43.093316 cobib-4.2.0/src/cobib/ui/components/
+-rw-r--r--   0 max       (1000) max       (1000)     1238 2023-08-01 21:06:11.000000 cobib-4.2.0/src/cobib/ui/components/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     1448 2023-06-12 19:22:05.000000 cobib-4.2.0/src/cobib/ui/components/argument_parser.py
+-rw-r--r--   0 max       (1000) max       (1000)      705 2023-06-12 19:22:05.000000 cobib-4.2.0/src/cobib/ui/components/entry_view.py
+-rw-r--r--   0 max       (1000) max       (1000)     3123 2023-08-01 21:33:37.000000 cobib-4.2.0/src/cobib/ui/components/help_screen.py
+-rw-r--r--   0 max       (1000) max       (1000)     2865 2023-06-12 19:22:05.000000 cobib-4.2.0/src/cobib/ui/components/input_screen.py
+-rw-r--r--   0 max       (1000) max       (1000)     3557 2023-06-12 19:22:05.000000 cobib-4.2.0/src/cobib/ui/components/list_view.py
+-rw-r--r--   0 max       (1000) max       (1000)     2029 2023-06-12 19:22:05.000000 cobib-4.2.0/src/cobib/ui/components/main_content.py
+-rw-r--r--   0 max       (1000) max       (1000)      565 2023-06-12 19:22:05.000000 cobib-4.2.0/src/cobib/ui/components/motion_key.py
+-rw-r--r--   0 max       (1000) max       (1000)     2035 2023-06-12 19:22:05.000000 cobib-4.2.0/src/cobib/ui/components/popup.py
+-rw-r--r--   0 max       (1000) max       (1000)     1405 2023-06-12 19:22:05.000000 cobib-4.2.0/src/cobib/ui/components/popup_logging_handler.py
+-rw-r--r--   0 max       (1000) max       (1000)      668 2023-06-12 19:22:05.000000 cobib-4.2.0/src/cobib/ui/components/popup_panel.py
+-rw-r--r--   0 max       (1000) max       (1000)     2570 2023-08-01 21:11:06.000000 cobib-4.2.0/src/cobib/ui/components/preset_filter_screen.py
+-rw-r--r--   0 max       (1000) max       (1000)     2054 2023-06-12 19:22:05.000000 cobib-4.2.0/src/cobib/ui/components/progress.py
+-rw-r--r--   0 max       (1000) max       (1000)     3313 2023-06-12 19:22:05.000000 cobib-4.2.0/src/cobib/ui/components/prompt.py
+-rw-r--r--   0 max       (1000) max       (1000)     2936 2023-06-12 19:22:05.000000 cobib-4.2.0/src/cobib/ui/components/search_view.py
+-rw-r--r--   0 max       (1000) max       (1000)     1415 2023-06-12 19:22:05.000000 cobib-4.2.0/src/cobib/ui/components/selection_filter.py
+-rw-r--r--   0 max       (1000) max       (1000)     1763 2023-06-20 19:36:56.000000 cobib-4.2.0/src/cobib/ui/shell_helper.py
+-rw-r--r--   0 max       (1000) max       (1000)    20064 2023-08-06 20:32:54.000000 cobib-4.2.0/src/cobib/ui/tui.py
+-rw-r--r--   0 max       (1000) max       (1000)     4303 2023-06-20 19:36:56.000000 cobib-4.2.0/src/cobib/ui/ui.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-08-08 18:43:43.093316 cobib-4.2.0/src/cobib/utils/
+-rw-r--r--   0 max       (1000) max       (1000)      242 2023-06-12 19:22:05.000000 cobib-4.2.0/src/cobib/utils/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     6731 2023-06-12 19:22:05.000000 cobib-4.2.0/src/cobib/utils/diff_renderer.py
+-rw-r--r--   0 max       (1000) max       (1000)     8267 2023-06-20 19:36:56.000000 cobib-4.2.0/src/cobib/utils/file_downloader.py
+-rw-r--r--   0 max       (1000) max       (1000)     4563 2023-06-20 19:36:56.000000 cobib-4.2.0/src/cobib/utils/journal_abbreviations.py
+-rw-r--r--   0 max       (1000) max       (1000)     4715 2023-07-31 19:52:40.000000 cobib-4.2.0/src/cobib/utils/logging.py
+-rw-r--r--   0 max       (1000) max       (1000)     1837 2023-06-12 19:22:05.000000 cobib-4.2.0/src/cobib/utils/rel_path.py
+-rw-r--r--   0 max       (1000) max       (1000)     8674 2023-06-20 19:36:56.000000 cobib-4.2.0/src/cobib/utils/shell_helper.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-08-08 18:43:43.069982 cobib-4.2.0/src/cobib.egg-info/
+-rw-r--r--   0 max       (1000) max       (1000)    41961 2023-08-08 18:43:43.000000 cobib-4.2.0/src/cobib.egg-info/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)     2304 2023-08-08 18:43:43.000000 cobib-4.2.0/src/cobib.egg-info/SOURCES.txt
+-rw-r--r--   0 max       (1000) max       (1000)        1 2023-08-08 18:43:43.000000 cobib-4.2.0/src/cobib.egg-info/dependency_links.txt
+-rw-r--r--   0 max       (1000) max       (1000)       47 2023-08-08 18:43:43.000000 cobib-4.2.0/src/cobib.egg-info/entry_points.txt
+-rw-r--r--   0 max       (1000) max       (1000)      135 2023-08-08 18:43:43.000000 cobib-4.2.0/src/cobib.egg-info/requires.txt
+-rw-r--r--   0 max       (1000) max       (1000)        6 2023-08-08 18:43:43.000000 cobib-4.2.0/src/cobib.egg-info/top_level.txt
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-08-08 18:43:43.093316 cobib-4.2.0/tests/
+-rw-r--r--   0 max       (1000) max       (1000)     4353 2023-06-12 19:22:05.000000 cobib-4.2.0/tests/test_main.py
```

### Comparing `cobib-4.1.0/CHANGELOG.md` & `cobib-4.2.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,50 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
 
+## [4.2.0] - 2023-08-08
+
+Pypi: https://pypi.org/project/cobib/4.2.0/
+
+### Added
+- added the `config.tui.scroll_offset` setting
+- added the `--field` command line option to the `open` command
+- (DEV) added a new `HINT` logging level which has value 35 and thus allows to
+  provide information to the user with a higher priority than `WARNING`
+- added the new `config.tui.preset_filters` (#114)
+  - preset filters can be selected from the TUI via the `p` key binding
+  - the first 9 filters can be selected directly by pressing the respective number
+  - pressing `0` resets any applied filter
+- implemented special tags (#63,!83)
+  - adds new builtin tags which will trigger special highlights of entries: `new`, `high`, `medium`, `low`
+  - adds the new `config.theme` settings section for configuring these settings
+  - you can also add more special tags via `config.theme.tags.user_tags`
+- added the `--skip-files` command line option to the `search` command
+
+### Changed
+- unicode symbols in entry labels will now be replaced with ascii ones (#119,#120)
+  - this is configured via the `config.database.format.default_label` setting, so if you are using a
+    custom value for this, be sure to update your config to make use of this feature
+- some user-visible logging messages around label disambiguation have been added (see also #121)
+- a warning has been added when the YAML parser encounters identical labels (which normally should
+  not occur in the database but if it does, coBib does not really know how to resolve this)
+- DOI redirect links are now followed recursively (up to 3 times), improving PDF
+  download link detection in the process (#97)
+
+### Deprecated
+- the `config.commands.search.highlights` section is deprecated in favor of `config.theme.search`
+
+### Fixed
+- retain scroll position in the TUI's list view
+
+
 ## [4.1.0] - 2023-06-11
 
 Pypi: https://pypi.org/project/cobib/4.1.0/
 
 ### Added
 - added the following settings which specify whether or not to preserve
   associated files during the respective commands being run:
@@ -763,15 +799,16 @@
 
 ## [0.1] - 2019-04-29
 
 ### Added
 - initial version with a basic `sqlite3`-based database
 
 
-[Unreleased]: https://gitlab.com/cobib/cobib/-/compare/v4.1.0...master
+[Unreleased]: https://gitlab.com/cobib/cobib/-/compare/v4.2.0...master
+[4.2.0]: https://gitlab.com/cobib/cobib/-/compare/v4.2.0
 [4.1.0]: https://gitlab.com/cobib/cobib/-/compare/v4.1.0
 [4.0.0]: https://gitlab.com/cobib/cobib/-/compare/v4.0.0
 [3.5.5]: https://gitlab.com/cobib/cobib/-/compare/v3.5.5
 [3.5.4]: https://gitlab.com/cobib/cobib/-/compare/v3.5.4
 [3.5.3]: https://gitlab.com/cobib/cobib/-/compare/v3.5.3
 [3.5.2]: https://gitlab.com/cobib/cobib/-/compare/v3.5.2
 [3.5.1]: https://gitlab.com/cobib/cobib/-/compare/v3.5.1
```

### Comparing `cobib-4.1.0/LICENSE.txt` & `cobib-4.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cobib-4.1.0/PKG-INFO` & `cobib-4.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cobib
-Version: 4.1.0
+Version: 4.2.0
 Summary: Console Bibliography
 Home-page: https://gitlab.com/cobib/cobib
 Author: Max Rossmannek
 Author-email: max.rossmannek@uzh.ch
 License: MIT License
 Project-URL: Bug Tracker, https://gitlab.com/cobib/cobib/-/issues
 Project-URL: Documentation, https://cobib.gitlab.io/cobib/cobib.html
@@ -289,14 +289,50 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
 
+## [4.2.0] - 2023-08-08
+
+Pypi: https://pypi.org/project/cobib/4.2.0/
+
+### Added
+- added the `config.tui.scroll_offset` setting
+- added the `--field` command line option to the `open` command
+- (DEV) added a new `HINT` logging level which has value 35 and thus allows to
+  provide information to the user with a higher priority than `WARNING`
+- added the new `config.tui.preset_filters` (#114)
+  - preset filters can be selected from the TUI via the `p` key binding
+  - the first 9 filters can be selected directly by pressing the respective number
+  - pressing `0` resets any applied filter
+- implemented special tags (#63,!83)
+  - adds new builtin tags which will trigger special highlights of entries: `new`, `high`, `medium`, `low`
+  - adds the new `config.theme` settings section for configuring these settings
+  - you can also add more special tags via `config.theme.tags.user_tags`
+- added the `--skip-files` command line option to the `search` command
+
+### Changed
+- unicode symbols in entry labels will now be replaced with ascii ones (#119,#120)
+  - this is configured via the `config.database.format.default_label` setting, so if you are using a
+    custom value for this, be sure to update your config to make use of this feature
+- some user-visible logging messages around label disambiguation have been added (see also #121)
+- a warning has been added when the YAML parser encounters identical labels (which normally should
+  not occur in the database but if it does, coBib does not really know how to resolve this)
+- DOI redirect links are now followed recursively (up to 3 times), improving PDF
+  download link detection in the process (#97)
+
+### Deprecated
+- the `config.commands.search.highlights` section is deprecated in favor of `config.theme.search`
+
+### Fixed
+- retain scroll position in the TUI's list view
+
+
 ## [4.1.0] - 2023-06-11
 
 Pypi: https://pypi.org/project/cobib/4.1.0/
 
 ### Added
 - added the following settings which specify whether or not to preserve
   associated files during the respective commands being run:
@@ -1049,15 +1085,16 @@
 
 ## [0.1] - 2019-04-29
 
 ### Added
 - initial version with a basic `sqlite3`-based database
 
 
-[Unreleased]: https://gitlab.com/cobib/cobib/-/compare/v4.1.0...master
+[Unreleased]: https://gitlab.com/cobib/cobib/-/compare/v4.2.0...master
+[4.2.0]: https://gitlab.com/cobib/cobib/-/compare/v4.2.0
 [4.1.0]: https://gitlab.com/cobib/cobib/-/compare/v4.1.0
 [4.0.0]: https://gitlab.com/cobib/cobib/-/compare/v4.0.0
 [3.5.5]: https://gitlab.com/cobib/cobib/-/compare/v3.5.5
 [3.5.4]: https://gitlab.com/cobib/cobib/-/compare/v3.5.4
 [3.5.3]: https://gitlab.com/cobib/cobib/-/compare/v3.5.3
 [3.5.2]: https://gitlab.com/cobib/cobib/-/compare/v3.5.2
 [3.5.1]: https://gitlab.com/cobib/cobib/-/compare/v3.5.1
```

### Comparing `cobib-4.1.0/README.md` & `cobib-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cobib-4.1.0/cobib.1` & `cobib-4.2.0/cobib.1`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH COBIB 1 2023-06-11 v4.1.0
+.TH COBIB 1 2023-08-08 v4.2.0
 .SH NAME
 coBib \- Console-based Bibliography Management
 .SH SYNOPSIS
 .B cobib
 [\fB\-\-version\fR]
 [\fB\-h\fR|\fB\-\-help\fR]
 [\fB\-v\fR|\fB\-\-verbose\fR]
@@ -267,14 +267,21 @@
 reapply the last undone changes (see above). See also \fIDATABASE/git\fR in the
 \fBCONFIGURATION\fR section for more information.
 .TP
 .B cobib open \fI<label>\fR
 Opens any associated \fIfile\fR of the entry with the given \fIlabel\fR.
 If multiple files are associated with the entry, the user can choose which
 file(s) to open through an interactive menu.
+.PP
+.in +8n
+.BR \-\-field " " \fI<choice>\fR
+.in +4n
+Specifies the field type to open. This bypasses the interactive prompt if
+multiple actionable fields are found. The choice can be either \fIall\fR or any
+of the values configured in \fIconfig.commands.open.fields\fR.
 .TP
 .B cobib show \fI<label>\fR
 Prints the entry with the given \fIlabel\fR in \fIBibLaTex\fR format to stdout.
 .TP
 .B cobib list \fI<args>\fR
 Lists all entries of the database in a basic table format to stdout which match
 the specified \fBFILTERS\fR (more information is provided in that section).
@@ -329,14 +336,19 @@
 This takes precedence over the \fIconfig.commands.search.ignore_case\fR setting.
 .PP
 .in +8n
 .BR \-I ", " \-\-no\-ignore\-case
 .in +4n
 Makes the search case-insensitive.
 This takes precedence over the \fIconfig.commands.list_.ignore_case\fR setting.
+.PP
+.in +8n
+.BR \-\-skip\-files
+.in +4n
+Skips searching the associated files.
 .TP
 .B cobib export \fI<args>\fR ...
 Exports the database.
 The positional arguments may be used to provide \fBFILTERS\fR which the entries
 must match in order to be included in the export \fIor\fR to provide a list of
 labels of the entries which are to be exported (this requires the \fI-s\fR flag
 to be set).
@@ -484,14 +496,17 @@
 .TP
 .BR v " " select
 Adds the current label to the \fIselection\fR.
 .TP
 .BR / " " search
 Opens a search prompt and views the results in an interactive tree structure.
 .TP
+.BR digit " " preset
+Immediately seledcts the preset filter given by that digit (0 = reset).
+.TP
 .BR a " " add
 Opens a command prompt which allows running the \fBadd\fR command as if outside
 of the TUI.
 .TP
 .BR d " " delete
 Deletes the current (or \fIselected\fR) label(s).
 .TP
@@ -509,14 +524,17 @@
 Opens a command prompt which allows running the \fBmodify\fR command as if
 outside of the TUI. If a \fIselection\fR is present, the \fI-s\fR argument will
 be set automatically.
 .TP
 .BR o " " open
 Opens the current (or \fIselected\fR) label(s).
 .TP
+.BR p " " preset
+Allows selecting a preset filter (see \fIconfig.tui.preset_filters\fR).
+.TP
 .BR r " " redo
 Reapplies the last undone change.
 This requires the git-integration (since v2.6.0) to be enabled!
 .TP
 .BR s " " sort
 Allows sorting the list view.
 .TP
@@ -626,22 +644,14 @@
 Specifies the program used to search in associated files.
 .TP
 .IR config.commands.search.grep_args = []
 Allows the specification of additional arguments for the \fIgrep\fR command.
 .TP
 .IR config.commands.search.ignore_case = False
 This boolean setting indicates whether search defaults to be case-insensitive.
-.TP
-.IR config.commands.search.highlights.label = 'blue'
-Specifies the color used to highlight the entry labels when displaying search
-rsults.
-.TP
-.IR config.commands.search.highlights.label = 'red'
-Specifies the color used to highlight the query matches when displaying search
-rsults.
 .PP
 .BR DATABASE
 .TP
 .IR config.database.file = '~/.local/share/cobib/literature.yaml'
 This setting sets the path to the database file. You can use \fI~\fR to
 represent your \fI$HOME\fR directory.
 .TP
@@ -649,19 +659,22 @@
 This boolean field indicates whether the database file should automatically be
 tracked in a git repository.
 Note, that you must initialize the git-tracking with \fIcobib init --git\fR. If
 you already have an existing database file, it will be preserved. Nonetheless,
 it is a good idea to make a backup before doing so, just in case.
 Also be sure to at least set a \fIname\fR and \fIemail\fR in the git config!
 .TP
-.IR config.database.format.label_default = '{label}'
+.IR config.database.format.label_default = '{unidecode(label)}'
 This field specifies the default label format in an f-string modification style
-as interpreted by the \fImodify\fR command. The default setting leaves the label
-unchanged from the import resource proposal. A simple example which uses the
-first authors surname and year is \fI'{author.split()[1]}{year}'\fR.
+as interpreted by the \fImodify\fR command. The default configuration value
+passes the originally provided label through \fItext-unidecode\fR which replaces
+all Unicode symbols with pure ASCII ones. A more useful example is
+\fI'{unidecode(author.split(' and ')[0].split()[-1])}{year}'\fR which takes the
+surname of the first author, replaces the Unicode characters and then
+immediately appends the publication year.
 .TP
 .IR config.database.format.label_suffix = ('_',\ LabelSuffix.ALPHA)
 This field specifies the default label disambiguator. The option takes a tuple
 of length 2, where the first entry is the string separating the proposed label
 from the disambiguator and the second one is one of the enumerators provided by
 \ficonfig.LabelSuffix\fR.
 .TP
@@ -688,14 +701,72 @@
 .TP
 .IR config.parsers.yaml.use_c_lib_yaml = True
 This boolean setting indicates whether to use the C-based implementation of the
 YAML parser. For this to work, additional packages may need to be installed.
 Read https://yaml.readthedocs.io/en/latest/install.html#optional-requirements
 for more details.
 .PP
+.BR THEME
+.TP
+.IR config.theme.search.label = 'blue'
+Specifies the color used to highlight the entry labels when displaying search
+rsults.
+.TP
+.IR config.theme.search.label = 'red'
+Specifies the color used to highlight the query matches when displaying search
+results.
+.TP
+.IR config.theme.tags.new = (10,\ 'bright_cyan')
+Specifies the weight and color used to highlight the labels of entries which
+have the \fInew\fR tag. coBib does NOT add this tag automatically, but you can
+do this easily with a \fIPostAddCommand\fR hook like so:
+
+    @Event.PostAddCommand.subscribe
+    def add_new_tag(cmd: AddCommand) -> None:
+        for entry in cmd.new_entries.values():
+            if "new" not in entry.tags:
+                entry.tags = entry.tags + ["new"]
+
+.TP
+.IR config.theme.tags.high = (40,\ 'on\ bright_red')
+Specifies the weight and color used to highlight the labels of entries which
+have the \fIhigh\fR priority tag.
+.TP
+.IR config.theme.tags.medium = (30,\ 'bright_red')
+Specifies the weight and color used to highlight the labels of entries which
+have the \fImedium\fR priority tag.
+.TP
+.IR config.theme.tags.low = (20,\ 'bright_yellow')
+Specifies the weight and color used to highlight the labels of entries which
+have the \fIlow\fR priority tag.
+.TP
+.IR config.theme.tags.user_tags = {}
+You can define more tags which should undergo special markup. Note, that the
+tags must be lower case, start with a letter and only contain letters or the
+characters \fI'.'\fR, \fI'-'\fR, \fI'_'\fR.
+.PP
+.BR TUI
+.TP
+.IR config.tui.scroll_offset = 2
+The minimum number of lines to keep above and below the cursor in the TUI's list
+view. This is similar to Vim's \fIscrolloff\fR setting.
+.TP
+.IR config.tui.preset_filters = []
+You can provide a list of preset filters. These can be interactively selected in
+the TUI by pressing \fIp\fR. To specify these, simply provide a string with the
+filter arguments, for example:
+
+    config.tui.preset_filters = [
+        "++tags READING",
+        "++year 2023",
+    ]
+
+The first 9 filters can be quickly accessed in the TUI by simply pressing the
+corresponding number. You can also use \fI0\fR to reset any applied filter.
+.PP
 .BR UTILS
 .TP
 .IR config.utils.file_downloader.default_location = '~/.local/share/cobib'
 This setting sets the default location for any downloaded associated files.
 .TP
 .IR config.utils.file_downloader.url_map = {}
 You can provide rules to map from a journal's landing page URL to its PDF URL.
```

### Comparing `cobib-4.1.0/setup.cfg` & `cobib-4.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `cobib-4.1.0/src/cobib/__main__.py` & `cobib-4.2.0/src/cobib/__main__.py`

 * *Files identical despite different names*

### Comparing `cobib-4.1.0/src/cobib/commands/__init__.py` & `cobib-4.2.0/src/cobib/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `cobib-4.1.0/src/cobib/commands/add.py` & `cobib-4.2.0/src/cobib/commands/add.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,23 +158,24 @@
 from cobib.utils.journal_abbreviations import JournalAbbreviations
 
 from .base_command import ArgumentParser, Command
 from .edit import EditCommand
 from .modify import evaluate_as_f_string
 
 LOGGER = logging.getLogger(__name__)
+"""@private module logger."""
 
 
 class AddCommand(Command):
     """The Add Command.
 
     This command can parse the following arguments:
 
         * `-l`, `--label`: the label to give to the new entry.
-        * `-d`, `--disambiguation`: hard-codes the reply to be used if a disambiguation prompt would
+        * `--disambiguation`: hard-codes the reply to be used if a disambiguation prompt would
           occur.
         * `-f`, `--file`: one or multiple files to associate with this entry. This data will be
           stored in the `cobib.database.Entry.file` property.
         * `-p`, `--path`: the path to store the downloaded associated file in. This can be used to
           overwrite the `cobib.config.config.FileDownloaderConfig.default_location`.
         * `--skip-download`: skips the automatic download of an associated file.
         * `--force-download`: forces the automatic download of an associated file.
@@ -490,15 +491,15 @@
 
         bib.save()
 
         self.git()
 
         for label in self.new_entries:
             msg = f"'{label}' was added to the database."
-            LOGGER.info(msg)
+            LOGGER.log(35, msg)
 
     @staticmethod
     def _wrap_prompt_process_response(
         func: Callable[[PromptBase[PromptType], str], PromptType]
     ) -> Callable[[PromptBase[PromptType], str], PromptType]:
         """A method to wrap a `PromptBase.process_response` method.
 
@@ -508,15 +509,15 @@
         Args:
             func: the `PromptBase.process_response` method to be wrapped.
 
         Returns:
             The wrapped `PromptBase.process_response` method.
         """
 
-        @override
+        @override  # type: ignore[misc]
         @wraps(func)
         def process_response(prompt: PromptBase[PromptType], value: str) -> PromptType:
             return_value: PromptType = func(prompt, value)
 
             if return_value == "help":
                 LOGGER.debug("User requested help.")
                 raise InvalidResponse(
```

### Comparing `cobib-4.1.0/src/cobib/commands/base_command.py` & `cobib-4.2.0/src/cobib/commands/base_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from textual.widget import Widget
 
 from cobib.config import Event, config
 from cobib.ui.components import ArgumentParser as ArgumentParser
 from cobib.utils.rel_path import RelPath
 
 LOGGER = logging.getLogger(__name__)
+"""@private module logger."""
 
 
 class Command(ABC):
     """The Command interface.
 
     This interface should be implemented by all concrete command implementations.
     """
```

### Comparing `cobib-4.1.0/src/cobib/commands/delete.py` & `cobib-4.2.0/src/cobib/commands/delete.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 from cobib.config import Event, config
 from cobib.database import Database
 from cobib.utils.rel_path import RelPath
 
 from .base_command import ArgumentParser, Command
 
 LOGGER = logging.getLogger(__name__)
+"""@private module logger."""
 
 
 class DeleteCommand(Command):
     """The Delete Command.
 
     This command can parse the following arguments:
 
@@ -179,15 +180,15 @@
         Args:
             func: the `PromptBase.process_response` method to be wrapped.
 
         Returns:
             The wrapped `PromptBase.process_response` method.
         """
 
-        @override
+        @override  # type: ignore[misc]
         @wraps(func)
         def process_response(prompt: PromptBase[PromptType], value: str) -> PromptType:
             return_value: PromptType = func(prompt, value)
 
             if isinstance(return_value, bool):
                 return return_value  # type: ignore[return-value]
```

### Comparing `cobib-4.1.0/src/cobib/commands/edit.py` & `cobib-4.2.0/src/cobib/commands/edit.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 from cobib.database import Database, Entry
 from cobib.parsers.yaml import YAMLParser
 from cobib.utils.rel_path import RelPath
 
 from .base_command import ArgumentParser, Command
 
 LOGGER = logging.getLogger(__name__)
+"""@private module logger."""
 
 
 class EditCommand(Command):
     """The Edit Command.
 
     This command can parse the following arguments:
```

### Comparing `cobib-4.1.0/src/cobib/commands/export.py` & `cobib-4.2.0/src/cobib/commands/export.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,15 @@
 from cobib.utils.journal_abbreviations import JournalAbbreviations
 from cobib.utils.rel_path import RelPath
 
 from .base_command import ArgumentParser, Command
 from .list_ import ListCommand
 
 LOGGER = logging.getLogger(__name__)
+"""@private module logger."""
 
 
 class ExportCommand(Command):
     """The Export Command.
 
     This command can parse the following arguments:
```

### Comparing `cobib-4.1.0/src/cobib/commands/import_.py` & `cobib-4.2.0/src/cobib/commands/import_.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 from cobib import importers
 from cobib.config import Event, config
 from cobib.database import Database, Entry
 
 from .base_command import ArgumentParser, Command
 
 LOGGER = logging.getLogger(__name__)
+"""@private module logger."""
 
 
 class ImportCommand(Command):
     """The ImportCommand.
 
     This command can parse the following arguments:
```

### Comparing `cobib-4.1.0/src/cobib/commands/init.py` & `cobib-4.2.0/src/cobib/commands/init.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 
 from cobib.config import Event, config
 from cobib.utils.rel_path import RelPath
 
 from .base_command import ArgumentParser, Command
 
 LOGGER = logging.getLogger(__name__)
+"""@private module logger."""
 
 
 class InitCommand(Command):
     """The Init Command.
 
     This command can parse the following arguments:
```

### Comparing `cobib-4.1.0/src/cobib/commands/list_.py` & `cobib-4.2.0/src/cobib/commands/list_.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,15 @@
 from cobib.config import Event, config
 from cobib.database import Database, Entry
 from cobib.ui.components import ListView
 
 from .base_command import ArgumentParser, Command
 
 LOGGER = logging.getLogger(__name__)
+"""@private module logger."""
 
 
 class ListCommand(Command):
     """The List Command.
 
     This command can parse the following arguments:
 
@@ -338,26 +339,28 @@
     def render_rich(self) -> ConsoleRenderable:
         rich_table = Table()
 
         for col in self.columns:
             rich_table.add_column(col)
 
         for entry in self.entries:
-            stringified: Dict[str, str] = entry.stringify()
+            stringified: Dict[str, str] = entry.stringify(markup=True)
 
             rich_table.add_row(*(stringified.get(col, "") for col in self.columns))
 
         return rich_table
 
     @override
     def render_textual(self) -> ListView:
         textual_table = ListView()
 
         for col in self.columns:
             textual_table.add_column(col, width=None)
 
         for entry in self.entries:
-            stringified: Dict[str, str] = entry.stringify()
+            stringified: Dict[str, str] = entry.stringify(markup=True)
 
-            textual_table.add_row(*(Text(stringified.get(col, "")) for col in self.columns))
+            textual_table.add_row(
+                *(Text.from_markup(stringified.get(col, "")) for col in self.columns)
+            )
 
         return textual_table
```

### Comparing `cobib-4.1.0/src/cobib/commands/modify.py` & `cobib-4.2.0/src/cobib/commands/modify.py`

 * *Files 7% similar despite different names*

```diff
@@ -88,26 +88,28 @@
 
 import ast
 import logging
 from typing import Any, Callable, Dict, List, Optional, Tuple, Type
 
 from rich.console import Console
 from rich.prompt import PromptBase, PromptType
+from text_unidecode import unidecode
 from textual.app import App
 from typing_extensions import override
 
 from cobib.config import Event, config
 from cobib.database import Database, Entry
 from cobib.utils.logging import get_stream_handler
 from cobib.utils.rel_path import RelPath
 
 from .base_command import ArgumentParser, Command
 from .list_ import ListCommand
 
 LOGGER = logging.getLogger(__name__)
+"""@private module logger."""
 
 
 class ModifyCommand(Command):
     """The Modify Command.
 
     This command can parse the following arguments:
 
@@ -379,19 +381,23 @@
 
 def evaluate_ast_node(node: ast.expr, locals_: Optional[Dict[str, Any]] = None) -> str:
     """Evaluates an AST node representing an f-string.
 
     Args:
         node: the AST expression extracted from an f-string.
         locals_: the dictionary of local variables to be used as context for the expression
-            evaluation.
+            evaluation. For convenience, this will include the `unidecode` method provided by
+            [text-unidecode](https://pypi.org/project/text-unidecode).
 
     Returns:
         The evaluated AST node expression.
     """
+    if locals_ is not None and "unidecode" not in locals_:
+        locals_["unidecode"] = unidecode
+
     try:
         # pylint: disable=eval-used
         return eval(  # type: ignore
             compile(ast.Expression(node), filename="<string>", mode="eval"), locals_
         )
     except NameError as err:
         LOGGER.warning("You tried use an undefined variable. Falling back to an empty string.")
@@ -401,25 +407,29 @@
 
 def evaluate_as_f_string(value: str, locals_: Optional[Dict[str, Any]] = None) -> str:
     """Evaluates a string as if it were a literal f-string.
 
     Args:
         value: the string to be evaluated.
         locals_: the dictionary of local variables to be used as context for the expression
-            evaluation.
+            evaluation. For convenience, this will include the `unidecode` method provided by
+            [text-unidecode](https://pypi.org/project/text-unidecode).
 
     Returns:
         The evaluated f-string.
 
     Raises:
         ValueError: if an unexpected AST component type is encountered.
 
     References:
         <https://stackoverflow.com/a/61190684>
     """
+    if locals_ is not None and "unidecode" not in locals_:
+        locals_["unidecode"] = unidecode
+
     result: List[str] = []
     for part in ast.parse(f"f'''{value}'''").body[0].value.values:  # type: ignore
         typ = type(part)
 
         if typ is ast.Constant:
             result.append(part.value)
 
@@ -427,15 +437,15 @@
             value = evaluate_ast_node(part.value, locals_)
 
             if part.conversion >= 0:
                 conversions: Dict[str, Callable[[Any], str]] = {"a": ascii, "r": repr, "s": str}
                 value = conversions[chr(part.conversion)](value)
 
             if part.format_spec:
-                value = format(value, evaluate_ast_node(part.format_spec))
+                value = format(value, evaluate_ast_node(part.format_spec, locals_))
 
             result.append(str(value))
 
         else:
             LOGGER.warning("Unexpected AST node expression type '%s' for an f-string.", typ)
             raise ValueError
```

### Comparing `cobib-4.1.0/src/cobib/commands/open.py` & `cobib-4.2.0/src/cobib/commands/open.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,22 @@
 With the above options, here is what will happen depending on the users choice:
 * `1`, `2`, or `3`: will open the respective file or URL.
 * `file` or `url`: will open the respective group.
 * `all`: will open all matches.
 * `help`: will print the detailed help-menu again.
 * `cancel`: will abort the command.
 
+Since coBib v4.2.0 you can also bypass the above interactive prompt from the command-line using the
+optional `--field` argument. However, this only allows you to specify `all` or an openable field
+name (e.g. `file` or `url`) but *not* any of the numbers (since you would not know the order up
+front). Here is an example which will open all openable fields found in an entry:
+```
+cobib open <label 1> --field all
+```
+
 ### TUI
 
 You can also trigger this command from the `cobib.ui.tui.TUI`.
 By default, it is bound to the `o` key.
 """
 
 from __future__ import annotations
@@ -59,37 +67,45 @@
 from cobib.config import Event, config
 from cobib.database import Database
 from cobib.utils.rel_path import RelPath
 
 from .base_command import ArgumentParser, Command
 
 LOGGER = logging.getLogger(__name__)
+"""@private module logger."""
 
 
 class OpenCommand(Command):
     """The Open Command.
 
     This command can parse the following arguments:
 
         * `labels`: one (or multiple) labels of the entries to be opened.
+        * `--field`: specifies the field to be opened, bypassing the interactive prompt.
     """
 
     name = "open"
 
     @override
     @classmethod
     def init_argparser(cls) -> None:
         parser = ArgumentParser(prog="open", description="Open subcommand parser.")
         parser.add_argument("labels", type=str, nargs="+", help="labels of the entries")
+        parser.add_argument(
+            "--field",
+            type=str,
+            choices=["all"] + config.commands.open.fields,
+            help="which field to open in case multiple are found",
+        )
         cls.argparser = parser
 
     # TODO: can we make the implementation cleaner and avoid the type ignore comment below?
     @override
     async def execute(self) -> None:  # type: ignore[override]
-        # pylint: disable=invalid-overridden-method
+        # pylint: disable=invalid-overridden-method,too-many-branches
         LOGGER.debug("Starting Open command.")
 
         Event.PreOpenCommand.fire(self)
 
         bib = Database()
 
         for label in self.largs.labels:
@@ -118,14 +134,33 @@
                 msg = f"The entry '{label}' has no actionable field associated with it."
                 LOGGER.warning(msg)
                 continue
 
             if count == 1:
                 # we found a single URL to open
                 self._open_url(list(things_to_open.values())[0][0])
+
+            elif self.largs.field is not None:
+                choice = self.largs.field
+                LOGGER.debug("User selected the %s set of urls from the CLI.", choice)
+
+                if choice == "all":
+                    for urls in things_to_open.values():
+                        for url in urls:
+                            self._open_url(url)
+
+                elif choice in things_to_open.keys():
+                    for url in things_to_open[choice]:
+                        self._open_url(url)
+
+                else:
+                    msg = f"The entry '{label}' has no field '{choice}' associated with it."
+                    LOGGER.warning(msg)
+                    continue
+
             else:
                 # we query the user what to do
                 idx = 0
                 url_list: list[ParseResult] = []
                 prompt_text = Text()
                 choices = ["all"] + config.commands.open.fields + ["help", "cancel"]
 
@@ -216,15 +251,15 @@
         Args:
             func: the `PromptBase.process_response` method to be wrapped.
 
         Returns:
             The wrapped `PromptBase.process_response` method.
         """
 
-        @override
+        @override  # type: ignore[misc]
         @wraps(func)
         def process_response(prompt: PromptBase[PromptType], value: str) -> PromptType:
             return_value: PromptType = func(prompt, value)
 
             if return_value == "help":
                 LOGGER.debug("User requested help.")
                 raise InvalidResponse(
```

### Comparing `cobib-4.1.0/src/cobib/commands/redo.py` & `cobib-4.2.0/src/cobib/commands/redo.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 from cobib.config import Event, config
 from cobib.database import Database
 from cobib.utils.rel_path import RelPath
 
 from .base_command import ArgumentParser, Command
 
 LOGGER = logging.getLogger(__name__)
+"""@private module logger."""
 
 
 class RedoCommand(Command):
     """The Redo Command.
 
     This command does not parse any additional arguments.
     """
```

### Comparing `cobib-4.1.0/src/cobib/commands/search.py` & `cobib-4.2.0/src/cobib/commands/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,16 @@
 
 ### Associated files
 
 The search will also be performed on any associated files of your entries.
 You can configure the tool which is used to perform this search via the
 `cobib.config.config.SearchCommandConfig.grep` setting (defaults to `grep`).
 
+If you do not want to search through associated files, you can specify the `--skip-files` argument.
+
 ### TUI
 
 You can also trigger this command from the `cobib.ui.tui.TUI`.
 By default, it is bound to the `/` key.
 
 .. note::
    For more information on the searching mechanisms see also `cobib.database.Entry.search`.
@@ -72,14 +74,15 @@
 from cobib.database import Entry
 from cobib.ui.components import SearchView
 
 from .base_command import ArgumentParser, Command
 from .list_ import ListCommand
 
 LOGGER = logging.getLogger(__name__)
+"""@private module logger."""
 
 
 class SearchCommand(Command):
     """The Search Command.
 
     This command can parse the following arguments:
 
@@ -90,14 +93,15 @@
           overwrites the `cobib.config.config.SearchCommandConfig.ignore_case` setting.
         * `-I`, `--no-ignore-case`: if specified, the search will be case-sensitive. This
           overwrites the `cobib.config.config.SearchCommandConfig.ignore_case` setting.
         * `-c`, `--context`: you can specify the number of lines of "context" which is the number of
           lines before and after the actual match to be included in the output. This is similar to
           the `-C` option of `grep`. You can configure the default value via the
           `cobib.config.config.SearchCommandConfig.context` setting.
+        * `--skip-files`: if specified, associated files will **not** be searched.
         * in addition to the above, you can add `filters` to narrow the search down to a subset of
           your database. For more information refer to `cobib.commands.list_`.
     """
 
     name = "search"
 
     @override
@@ -146,14 +150,20 @@
             "-c",
             "--context",
             type=int,
             default=config.commands.search.context,
             help="number of context lines to provide for each match",
         )
         parser.add_argument(
+            "--skip-files",
+            action="store_true",
+            default=None,
+            help="do NOT search through associated files",
+        )
+        parser.add_argument(
             "filter",
             nargs="*",
             help="You can specify filters as used by the `list` command in order to select a "
             "subset of labels to be modified. To ensure this works as expected you should add the "
             "pseudo-argument '--' before the list of filters. See also `list --help` for more "
             "information.",
         )
@@ -188,15 +198,17 @@
 
         ignore_case = config.commands.search.ignore_case
         if self.largs.ignore_case is not None:
             ignore_case = self.largs.ignore_case
         LOGGER.debug("The search will be performed case %ssensitive", "in" if ignore_case else "")
 
         for entry in self.entries.copy():
-            matches = entry.search(self.largs.query, self.largs.context, ignore_case)
+            matches = entry.search(
+                self.largs.query, self.largs.context, ignore_case, self.largs.skip_files
+            )
             if not matches:
                 self.entries.remove(entry)
                 continue
 
             self.matches.append(matches)
             self.hits += len(matches)
 
@@ -222,27 +234,27 @@
         ignore_case = config.commands.search.ignore_case
         if self.largs.ignore_case is not None:
             ignore_case = self.largs.ignore_case
 
         tree = Tree(".", hide_root=True)
         for entry, matches in zip(self.entries, self.matches):
             subtree = tree.add(
-                Text.assemble(
-                    (entry.label, config.commands.search.highlights.label),
-                    f" - {len(matches)} match" + ("es" if len(matches) > 1 else ""),
+                Text.from_markup(
+                    f"[search.label]{entry.markup_label()}[/search.label] - {len(matches)} match"
+                    + ("es" if len(matches) > 1 else "")
                 )
             )
 
             for idx, match in enumerate(matches):
                 matchtree = subtree.add(str(idx + 1))
                 for line in match:
                     line_text = Text(line)
                     line_text.highlight_words(
                         self.largs.query,
-                        config.commands.search.highlights.query,
+                        config.theme.search.query,
                         case_sensitive=not ignore_case,
                     )
                     matchtree.add(line_text)
 
         return tree
 
     @override
@@ -250,17 +262,17 @@
         ignore_case = config.commands.search.ignore_case
         if self.largs.ignore_case is not None:
             ignore_case = self.largs.ignore_case
 
         tree = SearchView(".")
         for entry, matches in zip(self.entries, self.matches):
             subtree = tree.root.add(
-                Text.assemble(
-                    (entry.label, config.commands.search.highlights.label),
-                    f" - {len(matches)} match" + ("es" if len(matches) > 1 else ""),
+                Text.from_markup(
+                    f"[search.label]{entry.markup_label()}[/search.label] - {len(matches)} match"
+                    + ("es" if len(matches) > 1 else "")
                 ),
                 # TODO: make configurable
                 expand=False,
             )
 
             for idx, match in enumerate(matches):
                 matchtree = subtree.add(
@@ -268,13 +280,13 @@
                     # TODO: make configurable
                     expand=True,
                 )
                 for line in match:
                     line_text = Text(line)
                     line_text.highlight_words(
                         self.largs.query,
-                        config.commands.search.highlights.query,
+                        config.theme.search.query,
                         case_sensitive=not ignore_case,
                     )
                     matchtree.add_leaf(line_text)
 
         return tree
```

### Comparing `cobib-4.1.0/src/cobib/commands/show.py` & `cobib-4.2.0/src/cobib/commands/show.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from cobib.config import Event
 from cobib.database import Database
 from cobib.parsers.bibtex import BibtexParser
 
 from .base_command import ArgumentParser, Command
 
 LOGGER = logging.getLogger(__name__)
+"""@private module logger."""
 
 
 class ShowCommand(Command):
     """The Show Command.
 
     This command can parse the following arguments:
```

### Comparing `cobib-4.1.0/src/cobib/commands/undo.py` & `cobib-4.2.0/src/cobib/commands/undo.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 from cobib.config import Event, config
 from cobib.database import Database
 from cobib.utils.rel_path import RelPath
 
 from .base_command import ArgumentParser, Command
 
 LOGGER = logging.getLogger(__name__)
+"""@private module logger."""
 
 
 class UndoCommand(Command):
     """The Undo Command.
 
     This command can parse the following arguments:
```

### Comparing `cobib-4.1.0/src/cobib/config/__init__.py` & `cobib-4.2.0/src/cobib/config/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,9 +19,10 @@
 from cobib.config import config
 ```
 
 For more information take a look at the example configuration, `cobib.config.example`.
 """
 
 from .config import LabelSuffix as LabelSuffix
+from .config import TagMarkup as TagMarkup
 from .config import config as config
 from .event import Event as Event
```

### Comparing `cobib-4.1.0/src/cobib/config/config.py` & `cobib-4.2.0/src/cobib/config/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,28 +10,32 @@
 from __future__ import annotations
 
 import importlib.util
 import io
 import logging
 import os
 import sys
+import warnings
 from abc import abstractmethod
-from dataclasses import MISSING, dataclass, field
+from dataclasses import MISSING, dataclass, field, fields
 from enum import Enum
 from pathlib import Path
-from typing import TYPE_CHECKING, Callable, Optional, TextIO, Union
+from typing import TYPE_CHECKING, Callable, NamedTuple, Optional, TextIO, Union
 
+from rich.style import Style
+from rich.theme import Theme
 from typing_extensions import override
 
 from cobib.utils.rel_path import RelPath
 
 if TYPE_CHECKING:
     from .event import Event
 
 LOGGER = logging.getLogger(__name__)
+"""@private module logger."""
 
 
 @dataclass
 class _ConfigBase:
     """Base class for configuration section dataclasses."""
 
     @staticmethod
@@ -62,14 +66,174 @@
         for name, field_ in self.__dataclass_fields__.items():
             if field_.default != MISSING:
                 setattr(self, name, field_.default)
             else:
                 setattr(self, name, field_.default_factory())  # type: ignore[misc]
 
 
+class TagMarkup(NamedTuple):
+    """A tuple for representing the weight and style of a tag."""
+
+    weight: int
+    """The weight of the tag. This integer is used to determine the markup priority of the tag.
+    Higher integer values indicate a higher priority."""
+    style: str | Style
+    """The style of the tag. This can be a `rich.Style` or a string which can be interpreted by
+    `rich.Style.parse`."""
+
+
+@dataclass
+class TagsThemeConfig(_ConfigBase):
+    """The markup configuration for special tags.
+
+    The tag names configured via this setting will be marked up via a `rich.Theme`. This allows you
+    to easily customize a visual differentiation of your entries based on simple properties.
+
+    The style and weight of the builtin special tags can be configured directly or you can add fully
+    custom special tags via the `user_tags` field.
+    """
+
+    new: TagMarkup = TagMarkup(10, "bold bright_cyan")
+    """The markup of the `new` tag. By default, coBib does *not* add this automatically, but you can
+    do this easily with a `PostAddCommand` hook like so:
+
+    ```python
+    @Event.PostAddCommand.subscribe
+    def add_new_tag(cmd: AddCommand) -> None:
+        for entry in cmd.new_entries.values():
+            if "new" not in entry.tags:
+                entry.tags = entry.tags + ["new"]
+    ```
+
+    .. note::
+       The `new` tag has a lower weight than all of the builtin priority tags (`high`, `medium`,
+       `low`) allowing these to be used to further classify new entries on a reading list.
+    """
+    high: TagMarkup = TagMarkup(40, "on bright_red")
+    """The markup of the `high` priority tag."""
+    medium: TagMarkup = TagMarkup(30, "bright_red")
+    """The markup of the `medium` priority tag."""
+    low: TagMarkup = TagMarkup(20, "bright_yellow")
+    """The markup of the `low` priority tag."""
+    user_tags: dict[str, TagMarkup] = field(default_factory=dict)
+    """A dictionary to add weight and markup definitions for arbitrary tags. The keys of the
+    dictionary will be compared as is to the tags of an `cobib.database.entry.Entry`.
+
+    .. note::
+       Because the markup names are used in a `rich.Theme`, they must be lower case, start with a
+       letter, and only contain letters or the characters `"."`, `"-"`, `"_"`. See also
+       [here](https://rich.readthedocs.io/en/stable/style.html#style-themes).
+    """
+
+    @property
+    def names(self) -> set[str]:
+        """Returns the set of all special tag names."""
+        return {f.name for f in fields(self)} - {"user_tags"} | set(self.user_tags.keys())
+
+    @property
+    def styles(self) -> dict[str, str | Style]:
+        """Returns the combined dictionary of all special tag styles."""
+        styles: dict[str, str | Style] = {}
+        for field_ in fields(self):
+            tag_markup = getattr(self, field_.name)
+            if isinstance(tag_markup, TagMarkup):
+                styles[f"tag.{field_.name}"] = tag_markup.style
+
+        for name, weighted_style in self.user_tags.items():
+            styles[f"tag.{name}"] = weighted_style.style
+
+        return styles
+
+    @property
+    def weights(self) -> dict[str, int]:
+        """Returns the combined dictionary of all special tag weights."""
+        weights: dict[str, int] = {}
+        for field_ in fields(self):
+            tag_markup = getattr(self, field_.name)
+            if isinstance(tag_markup, TagMarkup):
+                weights[field_.name] = tag_markup.weight
+
+        for name, weighted_style in self.user_tags.items():
+            weights[name] = weighted_style.weight
+
+        return weights
+
+    @override
+    def validate(self) -> None:
+        self._assert(
+            isinstance(self.new, TagMarkup), "config.theme.tags.new should be a TagMarkup tuple."
+        )
+        self._assert(
+            isinstance(self.high, TagMarkup), "config.theme.tags.high should be a TagMarkup tuple."
+        )
+        self._assert(
+            isinstance(self.medium, TagMarkup),
+            "config.theme.tags.medium should be a TagMarkup tuple.",
+        )
+        self._assert(
+            isinstance(self.low, TagMarkup), "config.theme.tags.low should be a TagMarkup tuple."
+        )
+        self._assert(
+            isinstance(self.user_tags, dict),
+            "config.theme.tags.user_tags should be a dict.",
+        )
+        for name, tag_markup in self.user_tags.items():
+            self._assert(
+                isinstance(tag_markup, TagMarkup),
+                f"The '{name}' entry in config.theme.tags.user_tags should be a TagMarkup tuple.",
+            )
+
+
+@dataclass
+class SearchHighlightConfig(_ConfigBase):
+    """The `config.theme.search` section."""
+
+    label: str | Style = "blue"
+    """Specifies the color with which to highlight the labels of search results."""
+    query: str | Style = "red"
+    """Specifies the color with which to highlight the query matches of a search."""
+
+    @property
+    def styles(self) -> dict[str, str | Style]:
+        """Returns the `rich.Theme`-compatible styles dictionary of the configured highlights."""
+        return {
+            "search.label": self.label,
+            "search.query": self.query,
+        }
+
+    @override
+    def validate(self) -> None:
+        LOGGER.debug("Validating the THEME.SEARCH configuration section.")
+        self._assert(isinstance(self.label, str), "config.theme.search.label should be a string.")
+        self._assert(isinstance(self.query, str), "config.theme.search.query should be a string.")
+
+
+@dataclass
+class ThemeConfig(_ConfigBase):
+    """The `config.theme` section."""
+
+    search: SearchHighlightConfig = field(default_factory=lambda: SearchHighlightConfig())
+    """The nested section for theme settings related to the `search` command."""
+    tags: TagsThemeConfig = field(default_factory=lambda: TagsThemeConfig())
+    """The nested section for the markup of special tags."""
+
+    @override
+    def validate(self) -> None:
+        LOGGER.debug("Validating the THEME configuration section.")
+        self.search.validate()
+        self.tags.validate()
+
+    def build(self) -> Theme:
+        """Returns the built `rich.Theme` from the configured styles."""
+        theme: dict[str, str | Style] = {}
+        theme.update(self.search.styles)
+        theme.update(self.tags.styles)
+        return Theme(theme)
+
+
 @dataclass
 class LoggingConfig(_ConfigBase):
     """The `config.logging` section."""
 
     cache: str | Path = "~/.cache/cobib/cache"
     """Specifies the default cache location."""
     logfile: str | Path = "~/.cache/cobib/cobib.log"
@@ -236,36 +400,14 @@
         self._assert(
             isinstance(self.fields, list),
             "config.commands.open.fields should be a list.",
         )
 
 
 @dataclass
-class SearchHighlightConfig(_ConfigBase):
-    """The `config.commands.search.highlights` section."""
-
-    label: str = "blue"
-    """Specifies the color with which to highlight the labels of search results."""
-    query: str = "red"
-    """Specifies the color with which to highlight the query matches of a search."""
-
-    @override
-    def validate(self) -> None:
-        LOGGER.debug("Validating the COMMANDS.SEARCH.HIGHLIGHTS configuration section.")
-        self._assert(
-            isinstance(self.label, str),
-            "config.commands.search.highlights.label should be a string.",
-        )
-        self._assert(
-            isinstance(self.query, str),
-            "config.commands.search.highlights.query should be a string.",
-        )
-
-
-@dataclass
 class SearchCommandConfig(_ConfigBase):
     """The `config.commands.search` section."""
 
     context: int = 1
     """Specifies the default number of context line to provide for each search query match. This is
     similar to the `-C` option of `grep`."""
     grep: str = "grep"
@@ -273,16 +415,27 @@
     default tool (`grep`) will not provide results for attached PDFs but other tools such as
     [ripgrep-all](https://github.com/phiresky/ripgrep-all) will."""
     grep_args: list[str] = field(default_factory=list)
     """Specifies additional arguments for your grep command. Note, that GNU's grep understands
     extended regex patterns even without specifying `-E`."""
     ignore_case: bool = False
     """Specifies whether searches should be performed case-insensitive."""
-    highlights: SearchHighlightConfig = field(default_factory=lambda: SearchHighlightConfig())
-    """The nested section for highlights used when displaying search results."""
+
+    @property
+    def highlights(self) -> SearchHighlightConfig:
+        """**DEPRECATED** Use `config.theme.search` instead!
+
+        The nested section for highlights used when displaying search results.
+        """
+        warnings.warn(
+            "The config.commands.search.highlights setting is DEPRECATED! Please use the new "
+            "config.theme.search setting instead.",
+            FutureWarning,
+        )
+        return config.theme.search
 
     @override
     def validate(self) -> None:
         LOGGER.debug("Validating the COMMANDS.SEARCH configuration section.")
         self._assert(
             isinstance(self.context, int) and self.context >= 0,
             "config.commands.search.context should be a non-negative integer.",
@@ -295,15 +448,14 @@
             isinstance(self.grep_args, list),
             "config.commands.search.grep_args should be a list.",
         )
         self._assert(
             isinstance(self.ignore_case, bool),
             "config.commands.search.ignore_case should be a boolean.",
         )
-        self.highlights.validate()
 
 
 @dataclass
 class CommandConfig(_ConfigBase):
     """The `config.commands` section."""
 
     add: AddCommandConfig = field(default_factory=lambda: AddCommandConfig())
@@ -347,21 +499,22 @@
     NUMERIC = lambda count: str(count)
 
 
 @dataclass
 class DatabaseFormatConfig(_ConfigBase):
     """The `config.database.format` section."""
 
-    label_default: str = "{label}"
+    label_default: str = "{unidecode(label)}"
     """Specifies a default label format which will be used for database entry keys. The format of
     this option follows the f-string like formatting of modifications (see also the documentation
-    of the `cobib.commands.modify.ModifyCommand`). The default configuration value leaves the label
-    unchanged compared to the metadata provided by the source from which the entry gets added. A
-    more useful example is `"{author.split(' and ')[0].split()[-1]}{year}"` which takes the surname
-    of the first author and immediately appends the publication year."""
+    of the `cobib.commands.modify.ModifyCommand`). The default configuration value passes the
+    originally provided label through [text-unidecode](https://pypi.org/project/text-unidecode/)
+    which replaces all Unicode symbols with pure ASCII ones. A more useful example is
+    `"{unidecode(author.split(' and ')[0].split()[-1])}{year}"` which takes the surname of the first
+    author, replaces the Unicode characters and then immediately appends the publication year."""
     label_suffix: tuple[str, LabelSuffix] = field(default_factory=lambda: ("_", LabelSuffix.ALPHA))
     """Specifies the suffix format which is used to disambiguate labels if a conflict would occur.
     This option takes a tuple of length 2, where the first entry is the string separating the
     proposed label from the enumerator and the second one is one of the enumerators provided by the
     `LabelSuffix` object. The available enumerators are:
         - ALPHA: a, b, ...
         - CAPTIAL: A, B, ...
@@ -525,14 +678,53 @@
     def validate(self) -> None:
         LOGGER.debug("Validating the PARSERS configuration section.")
         self.bibtex.validate()
         self.yaml.validate()
 
 
 @dataclass
+class TUIConfig(_ConfigBase):
+    """The `config.tui` section."""
+
+    scroll_offset: int = 2
+    """The minimum number of lines to keep above and below the cursor in the
+    `cobib.ui.tui.components.ListView`. This is similar to Vim's `scrolloff` setting."""
+    preset_filters: list[str] = field(default_factory=list)
+    """Permits providing a list of preset filters. These can be interactively selected in the TUI by
+    pressing `p`. To specify these, simply provide a string with the filter arguments, for example:
+
+    ```python
+    config.tui.preset_filters = [
+        "++tags READING",
+        "++year 2023",
+    ]
+    ```
+
+    The first 9 filters can be quickly accessed in the TUI by simply pressing the corresponding
+    number. You can also use 0 to reset any applied filter."""
+
+    @override
+    def validate(self) -> None:
+        LOGGER.debug("Validating the TUI configuration section.")
+        self._assert(
+            isinstance(self.scroll_offset, int),
+            "config.tui.scroll_offset should be an integer.",
+        )
+        self._assert(
+            isinstance(self.preset_filters, list),
+            "config.tui.preset_filters should be a list.",
+        )
+        for preset in self.preset_filters:
+            self._assert(
+                isinstance(preset, str),
+                "config.tui.preset_filters should be a list of strings.",
+            )
+
+
+@dataclass
 class FileDownloaderConfig(_ConfigBase):
     """The `config.utils.file_downloader` section."""
 
     default_location: str = "~/.local/share/cobib"
     """Specifies the default download location for associated files."""
     url_map: dict[str, str] = field(default_factory=dict)
     """Permits providing rules to map from a journal's landing page URL to its PDF URL. To do so,
@@ -621,14 +813,18 @@
     ```
 
     Note, that the typing is required for the config validation to pass!
     For more information refer to the `cobib.config.Event` documentation.
     """
     parsers: ParserConfig = field(default_factory=lambda: ParserConfig())
     """The nested section for the parsers settings."""
+    theme: ThemeConfig = field(default_factory=lambda: ThemeConfig())
+    """The nested section for the theme settings."""
+    tui: TUIConfig = field(default_factory=lambda: TUIConfig())
+    """The nested section for the TUI settings."""
     utils: UtilsConfig = field(default_factory=lambda: UtilsConfig())
     """The nested section for the utils settings."""
 
     # pylint: disable=invalid-name
     XDG_CONFIG_FILE: str | Path = field(
         default="~/.config/cobib/config.py", init=False, repr=False, compare=False
     )
@@ -637,14 +833,16 @@
     @override
     def validate(self) -> None:
         LOGGER.info("Validating the runtime configuration.")
         self.logging.validate()
         self.commands.validate()
         self.database.validate()
         self.parsers.validate()
+        self.theme.validate()
+        self.tui.validate()
         self.utils.validate()
 
         LOGGER.debug("Validating the EVENTS configuration section.")
         self._assert(isinstance(self.events, dict), "config.events should be a dict.")
         for event in self.events:
             self._assert(
                 event.validate(),
```

### Comparing `cobib-4.1.0/src/cobib/config/event.py` & `cobib-4.2.0/src/cobib/config/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,14 +114,15 @@
         "ForwardRef('commands.SearchCommand')": "cobib.commands.search.SearchCommand",
         "ForwardRef('commands.ShowCommand')": "cobib.commands.show.ShowCommand",
         "ForwardRef('commands.UndoCommand')": "cobib.commands.undo.UndoCommand",
         "ForwardRef('importers.ZoteroImporter')": "cobib.importers.zotero.ZoteroImporter",
     }
 
 LOGGER = logging.getLogger(__name__)
+"""@private module logger."""
 
 
 class Event(Enum):
     # pylint: disable=invalid-name
     """Subscribable events triggered at runtime.
 
     The following sections list all events available in coBib. The heading of each section includes
```

### Comparing `cobib-4.1.0/src/cobib/config/example.py` & `cobib-4.2.0/src/cobib/config/example.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 """
 
 # Generally, you won't need these, but the default configuration relies on them.
 import os
 import sys
 
 # To get started you must import coBib's configuration.
-from cobib.config import LabelSuffix, config
+from cobib.config import LabelSuffix, TagMarkup, config
 
 # Now, you are all set to apply your own settings.
 
 
 # LOGGING
 # You can specify the default cache location.
 config.logging.cache = "~/.cache/cobib/cache"
@@ -77,18 +77,14 @@
 # of strings in the following setting. Note, that GNU's grep understands extended regex patterns
 # even without specifying `-E`.
 config.commands.search.grep_args = []
 
 # You can specify whether searches should be performed case-insensitive.
 config.commands.search.ignore_case = False
 
-# You can configure the search label and query highlights.
-config.commands.search.highlights.label = "blue"
-config.commands.search.highlights.query = "red"
-
 
 # DATABASE
 # These settings affect the database in general.
 
 # You can specify the path to the database YAML file. You can use a `~` to represent your `$HOME`
 # directory.
 config.database.file = "~/.local/share/cobib/literature.yaml"
@@ -102,19 +98,21 @@
 
 # DATABASE.FORMAT
 # You can also specify some aspects about the format of the database.
 
 # You can specify a default label format which will be used for the database entry keys. The format
 # of this option follows the f-string like formatting of modifications (see also the documentation
 # of the [ModifyCommand](https://cobib.gitlab.io/cobib/cobib/commands/modify.html)). The default
-# configuration value leaves the label unchanged compared to the metadata provided by the source
-# from which the entry gets added. A more useful example is
-#     `"{author.split(' and ')[0].split()[-1]}{year}"`
-# which takes the surname of the first author and immediately appends the publication year.
-config.database.format.label_default = "{label}"
+# configuration value passes the originally provided label through
+# [text-unidecode](https://pypi.org/project/text-unidecode/) which replaces all Unicode symbols with
+# pure ASCII ones. A more useful example is
+#     `"{unidecode(author.split(' and ')[0].split()[-1])}{year}"`
+# which takes the surname of the first author, replaces the Unicode characters and then immediately
+# appends the publication year.
+config.database.format.label_default = "{unidecode(label)}"
 
 # You can specify the suffix format which is used to disambiguate labels if a conflict would occur.
 # This option takes a tuple of length 2, where the first entry is the string separating the proposed
 # label from the enumerator and the second one is one of the enumerators provided in the
 # `config.LabelSuffix` object. The available enumerators are:
 #   - ALPHA: a, b, ...
 #   - CAPTIAL: A, B, ...
@@ -144,14 +142,59 @@
 
 # You can specify that the C-based implementation of the YAML parser (called `LibYAML`) shall be
 # used, *significantly* increasing the performance of the parsing. Note, that this requires manual
 # installation of the C-based parser:
 # https://yaml.readthedocs.io/en/latest/install.html#optional-requirements
 config.parsers.yaml.use_c_lib_yaml = True
 
+# THEME
+
+# You can configure the search label and query highlights.
+config.theme.search.label = "blue"
+config.theme.search.query = "red"
+
+# You can also configure the markup used for the following builtin special tags:
+config.theme.tags.new = TagMarkup(10, "bold bright_cyan")
+config.theme.tags.high = TagMarkup(40, "on bright_red")
+config.theme.tags.medium = TagMarkup(30, "bright_red")
+config.theme.tags.low = TagMarkup(20, "bright_yellow")
+# None of these tags are added automatically, but you can do this easily with a `PostAddCommand`
+# hook like so:
+#
+#    @Event.PostAddCommand.subscribe
+#    def add_new_tag(cmd: AddCommand) -> None:
+#        for entry in cmd.new_entries.values():
+#            if "new" not in entry.tags:
+#                entry.tags = entry.tags + ["new"]
+#
+# Note, that the `new` tag has a lower weight than all of the builtin priority tags (`high`,
+# `medium`, `low`) allowing these to be used to further classify new entries on a reading list.
+
+# You can even specify your own tag names which should be treated with special markup.
+# Because the markup names are used in a `rich.Theme`, they must be lower case, start with a letter,
+# and only contain letters or the characters `"."`, `"-"`, `"_"`.
+config.theme.tags.user_tags = {}
+
+# TUI
+
+# You can configure the minimum number of lines to keep above and below the cursor in the TUI's list
+# view. This is similar to Vim's `scrolloff` setting.
+config.tui.scroll_offset = 2
+# You can provide a list of preset filters. These can be interactively selected in the TUI by
+# pressing `p`. To specify these, simply provide a string with the filter arguments, for example:
+#
+#     config.tui.preset_filters = [
+#         "++tags READING",
+#         "++year 2023",
+#     ]
+#
+# The first 9 filters can be quickly accessed in the TUI by simply pressing the corresponding
+# number. You can also use 0 to reset any applied filter.
+config.tui.preset_filters = []
+
 # UTILS
 
 # You can specify the default download location for associated files.
 config.utils.file_downloader.default_location = "~/.local/share/cobib"
 
 # You can provide rules to map from a journal's landing page URL to its PDF URL. To do so, you must
 # insert an entry into the following dictionary, with a regex-pattern matching the journal's landing
```

### Comparing `cobib-4.1.0/src/cobib/database/database.py` & `cobib-4.2.0/src/cobib/database/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from cobib.config import config
 from cobib.utils.rel_path import RelPath
 
 if TYPE_CHECKING:
     import cobib.database
 
 LOGGER = logging.getLogger(__name__)
+"""@private module logger."""
 
 
 # TODO: once Python 3.9 becomes the default, OrderedDict can be properly sub-typed
 class Database(OrderedDict):  # type: ignore
     """coBib's Database class is a runtime interface to the plain-test YAML file.
 
     This class is a *singleton*.
@@ -109,26 +110,45 @@
         Args:
             label: the label which to disambiguate.
             entry: the `Entry` to which this label belongs.
 
         Returns:
             A unique label.
         """
-        if label not in self.keys() or self[label] == entry:
+        if label not in self.keys():
+            LOGGER.info("The label '%s' does not yet exist in the runtime database.", label)
             return label
 
-        LOGGER.warning("Label '%s' already exists in database. Running disambiguation.", label)
+        if self[label] == entry:
+            LOGGER.log(
+                35,
+                "Even though the label '%s' already exists in the runtime database, the entry is "
+                "identical and, thus, no further disambiguation is necessary.",
+                label,
+            )
+            return label
+
+        LOGGER.warning("The label '%s' already exists in database. Running disambiguation.", label)
         separator, enumerator = config.database.format.label_suffix
         offset = 0
         while True:
             offset += 1
             new_label: str = label + separator + enumerator(offset)  # type: ignore[operator]
             if new_label not in self.keys():
                 LOGGER.info("Found new unique label: %s", new_label)
                 return new_label
+            LOGGER.log(
+                35,
+                "The label '%s' also already exists in the database. You are seeing this because "
+                "you are running a disambiguation of the label '%s'. You may want to check whether "
+                "these two entries are related and (if so) edit or merge them manually. For more "
+                "information see also: https://gitlab.com/cobib/cobib/-/issues/121",
+                new_label,
+                label,
+            )
 
     @classmethod
     def read(cls) -> None:
         """Reads the database file.
 
         The YAML database file pointed to by the configuration file is read in and parsed.
         This uses `cobib.parsers.YAMLParser` to parse the data.
```

### Comparing `cobib-4.1.0/src/cobib/database/entry.py` & `cobib-4.2.0/src/cobib/database/entry.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,19 +8,20 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
 from pylatexenc.latexencode import UnicodeToLatexEncoder
 
 from cobib.config import config
 from cobib.utils.rel_path import RelPath
 
-LOGGER = logging.getLogger(__name__)
-
 if TYPE_CHECKING:
     import cobib.parsers
 
+LOGGER = logging.getLogger(__name__)
+"""@private module logger."""
+
 
 class Entry:
     """coBib's bibliographic entry.
 
     coBib's `Database` stores the bibliographic information in entries which are instances of this
     class. This only contains a `label` which is a string used as a key to associate this entry as
     well as a free-form `data` dictionary, which can contain arbitrary key-value pairs.
@@ -94,14 +95,28 @@
 
         Args:
             label: the label of this entry.
         """
         LOGGER.debug("Changing the label '%s' to '%s'.", self.label, label)
         self._label = str(label)
 
+    def markup_label(self) -> str:
+        """Returns the label of this entry with the rich markup based on special tags."""
+        markup_label = self.label
+
+        markup_tags: dict[str, int] = {}
+        for tag in self.tags:
+            if tag in config.theme.tags.names:
+                markup_tags[f"tag.{tag}"] = config.theme.tags.weights[tag]
+
+        for tag, _ in sorted(markup_tags.items(), key=lambda item: item[1], reverse=True):
+            markup_label = f"[{tag}]{markup_label}[/{tag}]"
+
+        return markup_label
+
     @property
     def tags(self) -> List[str]:
         """The tags of this entry."""
         return self.data.get("tags", [])
 
     @tags.setter
     def tags(self, tags: Union[str, List[str]]) -> None:
@@ -223,22 +238,25 @@
                 "month",
                 self.label,
                 month,
                 self.data["month"],
                 extra={"entry": self.label, "field": "month"},
             )
 
-    def stringify(self) -> Dict[str, str]:
+    def stringify(self, *, markup: bool = False) -> Dict[str, str]:
         """Returns an identical entry to self but with all fields converted to strings.
 
+        Args:
+            markup: whether or not to add markup based on the configured special tags.
+
         Returns:
             An `Entry` with purely string fields.
         """
         data = {}
-        data["label"] = self.label
+        data["label"] = self.markup_label() if markup else self.label
         for field, value in self.data.items():
             if isinstance(value, list) and hasattr(config.database.stringify.list_separator, field):
                 data[field] = getattr(config.database.stringify.list_separator, field).join(value)
             else:
                 data[field] = str(value)
         return data
 
@@ -339,15 +357,19 @@
                 else:
                     match_list.append(not key[1])
         if or_:
             return any(m for m in match_list)
         return all(m for m in match_list)
 
     def search(
-        self, query: List[str], context: int = 1, ignore_case: bool = False
+        self,
+        query: List[str],
+        context: int = 1,
+        ignore_case: bool = False,
+        skip_files: bool = False,
     ) -> List[List[str]]:
         """Search entry contents for the query strings.
 
         The entry will *always* be converted to a searchable string using the
         `cobib.parsers.BibtexParser.dump` method. This text will then be search for each item in
         `query` and will interpret these as regex patterns.
         If a `file` is associated with this entry, the search will try its best to recursively query
@@ -355,14 +377,15 @@
         tool, `cobib.config.config.SearchCommandConfig.grep`.
 
         Args:
             query: the list of regex patterns to search for.
             context: the number of context lines to provide for each match. This behaves similarly
                 to the *Context Line Control* available for the UNIX `grep` command (`--context`).
             ignore_case: if True, the search will be case-*in*sensitive.
+            skip_files: if True, associated files will *not* be searched.
 
         Returns:
             A list of lists containing the context for each match associated with this entry.
         """
         LOGGER.debug("Searching entry %s.", self.label)
         matches: List[List[str]] = []
         # pylint: disable=import-outside-toplevel,cyclic-import
@@ -386,14 +409,18 @@
                     matches[-1].append(line)
                     # lower context
                     for string in bibtex[max(idx + 1, 0) : min(idx + context + 1, len(bibtex))]:
                         if re_compiled.search(string):
                             break
                         matches[-1].append(string)
 
+            if skip_files:
+                LOGGER.info("Skipping the search in associated files of %s", self.label)
+                continue
+
             for file_ in self.file:
                 grep_prog = config.commands.search.grep
                 path = RelPath(file_).path
                 if not path.exists():
                     LOGGER.warning(
                         "The associated file %s of entry %s does not exist!", file_, self.label
                     )
```

### Comparing `cobib-4.1.0/src/cobib/importers/base_importer.py` & `cobib-4.2.0/src/cobib/importers/base_importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from abc import ABC, abstractmethod
 from typing import List
 
 from cobib.database import Entry
 from cobib.ui.components import ArgumentParser as ArgumentParser
 
 LOGGER = logging.getLogger(__name__)
+"""@private module logger."""
 
 
 class Importer(ABC):
     """The Importer interface.
 
     This interface should be implemented by all concrete importer implementations.
     """
```

### Comparing `cobib-4.1.0/src/cobib/importers/zotero.py` & `cobib-4.2.0/src/cobib/importers/zotero.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 from cobib.parsers import BibtexParser
 from cobib.utils.file_downloader import FileDownloader
 from cobib.utils.rel_path import RelPath
 
 from .base_importer import ArgumentParser, Importer
 
 LOGGER = logging.getLogger(__name__)
+"""@private module logger."""
 
 
 class ZoteroImporter(Importer):
     """The Zotero Importer.
 
     This importer can parse the following arguments:
```

### Comparing `cobib-4.1.0/src/cobib/parsers/__init__.py` & `cobib-4.2.0/src/cobib/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `cobib-4.1.0/src/cobib/parsers/arxiv.py` & `cobib-4.2.0/src/cobib/parsers/arxiv.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
 from cobib.config import Event
 from cobib.database import Entry
 
 from .base_parser import Parser
 
 LOGGER = logging.getLogger(__name__)
+"""@private module logger."""
 
 ARXIV_URL = "https://export.arxiv.org/api/query?id_list="
 """arXiv exporting URL taken from [here](https://arxiv.org/help/oa)."""
 ARXIV_REGEX = r"(\d{4}.\d{4,5}|[a-z\-]+(\.[A-Z]{2})?\/\d{7})(v\d+)?"
 """A regex pattern used to match valid DOIs."""
 
 
@@ -110,15 +111,16 @@
         if "doi" in entry:
             entry["ENTRYTYPE"] = "article"
         else:
             entry["ENTRYTYPE"] = "unpublished"
         # strip last 'and' from author field
         entry["author"] = entry["author"][:-5]
         bib = OrderedDict()
-        bib[label] = Entry(label, entry)
+        actual_entry = Entry(label, entry)
+        bib[actual_entry.label] = actual_entry
 
         Event.PostArxivParse.fire(bib)
 
         return bib
 
     def dump(self, entry: Entry) -> None:
         """We cannot dump a generic entry as an arXiv ID."""
```

### Comparing `cobib-4.1.0/src/cobib/parsers/base_parser.py` & `cobib-4.2.0/src/cobib/parsers/base_parser.py`

 * *Files identical despite different names*

### Comparing `cobib-4.1.0/src/cobib/parsers/bibtex.py` & `cobib-4.2.0/src/cobib/parsers/bibtex.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 from cobib.config import Event, config
 from cobib.database import Entry
 
 from .base_parser import Parser
 
 LOGGER = logging.getLogger(__name__)
+"""@private module logger."""
 
 
 class BibtexParser(Parser):
     """The BibTex Parser."""
 
     name = "bibtex"
 
@@ -51,15 +52,16 @@
         bib = OrderedDict()
         for entry in database.entries:
             if "month" in entry.keys() and isinstance(
                 entry["month"], bibtexparser.bibtexexpression.BibDataStringExpression
             ):
                 entry["month"] = entry["month"].expr[0].name
             label = entry.pop("ID")
-            bib[label] = Entry(label, entry)
+            actual_entry = Entry(label, entry)
+            bib[actual_entry.label] = actual_entry
 
         Event.PostBibtexParse.fire(bib)
 
         return bib
 
     @override
     def dump(self, entry: Entry) -> str:
```

### Comparing `cobib-4.1.0/src/cobib/parsers/doi.py` & `cobib-4.2.0/src/cobib/parsers/doi.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 from cobib.config import Event
 from cobib.database import Entry
 
 from .base_parser import Parser
 from .bibtex import BibtexParser
 
 LOGGER = logging.getLogger(__name__)
+"""@private module logger."""
 
 DOI_URL = "https://doi.org/"
 """The DOI 'API' URL."""
 DOI_HEADER = {"Accept": "application/x-bibtex"}
 """The DOI 'API' header taken from [here](https://crosscite.org/docs.html)."""
 DOI_REGEX = r'(10\.[0-9a-zA-Z]+\/(?:(?!["&\'\?])\S)+)\b'
 """A regex pattern used to match valid DOIs."""
@@ -65,22 +66,31 @@
             LOGGER.warning(msg)
             return OrderedDict()
         doi = match.group(1)
         LOGGER.info("Gathering BibTex data for DOI: %s.", doi)
         try:
             page = requests.get(DOI_URL + doi, headers=DOI_HEADER, timeout=10)
             # this assumes that the doi.org page redirects to the correct journal's landing page
-            redirected_url = requests.head(DOI_URL + doi, timeout=1).headers["Location"]
+            redirected_url: str = ""
+            header = requests.head(DOI_URL + doi, timeout=1).headers
+            LOGGER.debug("The DOI URL header: '%s'", header)
+            max_iter = 3
+            while "Location" in header and max_iter:
+                max_iter -= 1
+                redirected_url = header["Location"]
+                LOGGER.debug("The found URL redirects to: '%s'", redirected_url)
+                header = requests.head(redirected_url, timeout=1).headers
         except requests.exceptions.RequestException as err:
             LOGGER.error("An Exception occurred while trying to query the DOI: %s.", doi)
             LOGGER.error(err)
             return OrderedDict()
         bib = BibtexParser().parse(page.text)
-        for entry in bib.values():
-            entry.data["_download"] = redirected_url
+        if redirected_url:
+            for entry in bib.values():
+                entry.data["_download"] = redirected_url
 
         Event.PostDOIParse.fire(bib)
 
         return bib
 
     def dump(self, entry: Entry) -> None:
         """We cannot dump a generic entry as a DOI."""
```

### Comparing `cobib-4.1.0/src/cobib/parsers/isbn.py` & `cobib-4.2.0/src/cobib/parsers/isbn.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
 from cobib.config import Event
 from cobib.database import Entry
 
 from .base_parser import Parser
 
 LOGGER = logging.getLogger(__name__)
+"""@private module logger."""
 
 ISBN_URL = "https://openlibrary.org/api/books?bibkeys=ISBN:"
 """ISBN API URL taken from [here](https://openlibrary.org/dev/docs/api/books)."""
 ISBN_REGEX = re.compile(
     r"(97[89]{1}(?:-?\d){10}|\d{9}[0-9X]{1}|[-0-9X]{10,16})", re.I | re.M | re.S
 )
 """A regex pattern used to match valid ISBNs. Adapted from
@@ -105,15 +106,16 @@
                 label = value[0]["name"].split()[-1] + label
                 entry["author"] = " and ".join([a["name"] for a in value])
             elif key == "publishers":
                 entry["publisher"] = " and ".join([a["name"] for a in value])
         # set entry-type do 'book'
         entry["ENTRYTYPE"] = "book"
         bib = OrderedDict()
-        bib[label] = Entry(label, entry)
+        actual_entry = Entry(label, entry)
+        bib[actual_entry.label] = actual_entry
 
         Event.PostISBNParse.fire(bib)
 
         return bib
 
     def dump(self, entry: Entry) -> None:
         """We cannot dump a generic entry as an ISBN."""
```

### Comparing `cobib-4.1.0/src/cobib/parsers/url.py` & `cobib-4.2.0/src/cobib/parsers/url.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
 from .arxiv import ARXIV_REGEX, ArxivParser
 from .base_parser import Parser
 from .doi import DOI_REGEX, DOIParser
 from .isbn import ISBN_REGEX, ISBNParser
 
 LOGGER = logging.getLogger(__name__)
+"""@private module logger."""
 
 
 class URLParser(Parser):
     # pylint: disable=too-many-return-statements
     """The URL Parser."""
 
     name = "url"
```

### Comparing `cobib-4.1.0/src/cobib/parsers/yaml.py` & `cobib-4.2.0/src/cobib/parsers/yaml.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
 from cobib.config import Event, config
 from cobib.database.entry import Entry
 
 from .base_parser import Parser
 
 LOGGER = logging.getLogger(__name__)
+"""@private module logger."""
 
 
 class YAMLParser(Parser):
     """The YAML Parser."""
 
     name = "yaml"
 
@@ -48,31 +49,39 @@
             YAMLParser._yaml.explicit_end = True  # type: ignore[assignment]
             YAMLParser._yaml.default_flow_style = False
 
     @override
     def parse(self, string: Union[str, Path]) -> Dict[str, Entry]:
         string = Event.PreYAMLParse.fire(string) or string
 
-        bib = OrderedDict()
+        bib: Dict[str, Entry] = OrderedDict()
         LOGGER.debug("Loading YAML data from file: %s.", string)
         try:
             stream: IO = io.StringIO(Path(string))  # type: ignore[arg-type,type-arg]
         except TypeError:
             try:
                 stream = open(string, "r", encoding="utf-8")  # pylint: disable=consider-using-with
             except FileNotFoundError as exc:
                 raise exc
         for entry in track(
             self._yaml.load_all(stream),  # type: ignore[union-attr]
             description="Reading database...",
             transient=True,
-            console=Console(file=sys.stderr),  # TODO: do not hard-code this
+            console=Console(file=sys.stderr),
         ):
             for label, data in entry.items():
-                bib[label] = Entry(label, data)
+                actual_entry = Entry(label, data)
+                if actual_entry.label in bib.keys():
+                    LOGGER.warning(
+                        "An entry with label '%s' was already encountered earlier on in the YAML "
+                        "file! Please check the file manually as this cannot be resolved "
+                        "automatically by coBib.",
+                        actual_entry.label,
+                    )
+                bib[actual_entry.label] = actual_entry
         stream.close()
 
         Event.PostYAMLParse.fire(bib)
 
         return bib
 
     @override
```

### Comparing `cobib-4.1.0/src/cobib/ui/__init__.py` & `cobib-4.2.0/src/cobib/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `cobib-4.1.0/src/cobib/ui/cli.py` & `cobib-4.2.0/src/cobib/ui/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from cobib.config import config
 from cobib.database import Database
 from cobib.ui.tui import TUI
 from cobib.ui.ui import UI
 from cobib.utils.logging import print_changelog
 
 LOGGER = logging.getLogger(__name__)
+"""@private module logger."""
 
 
 class CLI(UI):
     """The CLI class.
 
     In addition to the global arguments documented by the base class, the following are supported:
 
@@ -59,15 +60,15 @@
         )
 
     # pylint: disable=invalid-overridden-method
     @override
     async def run(self) -> None:  # type: ignore[override]
         arguments = self.parse_args()
 
-        console = Console()
+        console = Console(theme=config.theme.build())
 
         if not arguments.porcelain:
             # print latest changelog
             changelog = print_changelog(__version__, config.logging.version)
             if changelog is not None:
                 console.print(changelog)
```

### Comparing `cobib-4.1.0/src/cobib/ui/components/__init__.py` & `cobib-4.2.0/src/cobib/ui/components/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,11 +16,12 @@
 from .input_screen import InputScreen as InputScreen
 from .list_view import ListView as ListView
 from .main_content import MainContent as MainContent
 from .motion_key import MotionKey as MotionKey
 from .popup import Popup as Popup
 from .popup_logging_handler import PopupLoggingHandler as PopupLoggingHandler
 from .popup_panel import PopupPanel as PopupPanel
+from .preset_filter_screen import PresetFilterScreen as PresetFilterScreen
 from .progress import Progress as Progress
 from .prompt import Prompt as Prompt
 from .search_view import SearchView as SearchView
 from .selection_filter import SelectionFilter as SelectionFilter
```

### Comparing `cobib-4.1.0/src/cobib/ui/components/argument_parser.py` & `cobib-4.2.0/src/cobib/ui/components/argument_parser.py`

 * *Files identical despite different names*

### Comparing `cobib-4.1.0/src/cobib/ui/components/entry_view.py` & `cobib-4.2.0/src/cobib/ui/components/entry_view.py`

 * *Files identical despite different names*

### Comparing `cobib-4.1.0/src/cobib/ui/components/help_screen.py` & `cobib-4.2.0/src/cobib/ui/components/help_screen.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,21 +45,23 @@
         ("q", "Quit's coBib"),
         ("question_mark", "Toggles the help screen"),
         ("underscore", "Toggles between the horizontal and vertical layout"),
         ("space", "Toggles folding of a search result"),
         ("colon", "Starts the prompt for an arbitrary coBib command"),
         ("v", "Selects the current entry"),
         ("slash", "Searches the database for the provided string"),
+        ("digit", "Immediately selects the preset filter given by that digit (0 = reset)"),
         ("a", "Prompts for a new entry to be added to the database"),
         ("d", "Deletes the current (or selected) entries"),
         ("e", "Edits the current entry"),
         ("f", "Allows filtering the table using `++/--` keywords"),
         ("i", "Imports entries from another source"),
         ("m", "Prompts for a modification (respects selection)"),
         ("o", "Opens the current (or selected) entries"),
+        ("p", "Allows selecting a preset filter (see `config.tui.preset_filters`)"),
         ("r", "Redoes the last undone change. Requires git-tracking!"),
         ("s", "Prompts for the field to sort by (use -r to list in reverse)"),
         ("u", "Undes the last change. Requires git-tracking!"),
         ("x", "Exports the current (or selected) entries"),
         ("j", "Moves one row down"),
         ("k", "Moves one row up"),
         ("h", "Moves to the left"),
```

### Comparing `cobib-4.1.0/src/cobib/ui/components/input_screen.py` & `cobib-4.2.0/src/cobib/ui/components/input_screen.py`

 * *Files identical despite different names*

### Comparing `cobib-4.1.0/src/cobib/ui/components/list_view.py` & `cobib-4.2.0/src/cobib/ui/components/search_view.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,32 @@
-"""coBib's list results viewer widget.
+"""coBib's search results viewer widget.
 
-This widget gets produces by `cobib.commands.list.ListCommand.render_textual`.
-It subclasses textual's built-in `DataTable` widget.
+This widget gets produces by `cobib.commands.search.SearchCommand.render_textual`.
+It subclasses textual's built-in `Tree` widget.
 
 .. warning::
 
    This module makes no API stability guarantees! Refer to `cobib.ui.components` for more details.
 """
 
 from __future__ import annotations
 
-from typing import Any
-
 from rich.text import Text
 from textual.binding import Binding
-from textual.coordinate import Coordinate
-from textual.reactive import reactive
-from textual.widgets import DataTable
+from textual.css.query import NoMatches
+from textual.widgets import Tree
 from typing_extensions import override
 
 from .motion_key import MotionKey
 
 
-class ListView(DataTable[Text]):
-    """coBib's list results viewer widget."""
-
-    id = "cobib-list-view"
+class SearchView(Tree[Text]):
+    """coBib's search results viewer widget."""
 
-    cursor_type = reactive("row")
+    id = "cobib-search-view"
 
     BINDINGS = [
         Binding("j", "motion('down', 'cursor_down')", "Down", show=False),
         Binding("k", "motion('up', 'cursor_up')", "Up", show=False),
         Binding("h", "motion('left', 'cursor_left')", "Left", show=False),
         Binding("l", "motion('right', 'cursor_right')", "Right", show=False),
         Binding("down", "motion('down', 'cursor_down')", "Down", show=False),
@@ -46,27 +41,17 @@
     | space | Toggle the expand/collapsed space of the current item. |
     | j, down | Moves one row down. |
     | k, up | Moves one row up. |
     | h, left | Moves to the left. |
     | l, right | Moves to the right. |
     """
 
-    DEFAULT_CSS = """
-        ListView {
-            height: 1fr;
-        }
-    """
-
     @override
-    def __init__(self, *args: Any, **kwargs: Any) -> None:
-        super().__init__(*args, **kwargs)
-
-        # TODO: revisit this based on the outcome of https://github.com/Textualize/textual/pull/2740
-        self.fixed_columns = 1
-        self.zebra_stripes = True
+    def on_mount(self) -> None:
+        self.show_root = False
 
     def action_motion(self, key: str, action: str) -> None:
         """Action to move the cursor.
 
         Under the hood, this delegates to the respective built-in cursor motion methods.
         However, this method also posts a `cobib.ui.components.motion_key.MotionKey` event.
 
@@ -81,9 +66,16 @@
 
     def get_current_label(self) -> str:
         """Gets the label of the entry currently under the cursor.
 
         Returns:
             The label of the entry currently under the cursor.
         """
-        label = self.get_cell_at(Coordinate(self.cursor_row, 0)).plain
+        previous_node, current_node = self.cursor_node, self.cursor_node
+        if current_node is None:
+            raise NoMatches  # pylint: disable=raise-missing-from
+        while current_node.parent is not None:
+            previous_node, current_node = current_node, current_node.parent
+        if previous_node is None:
+            raise NoMatches  # pylint: disable=raise-missing-from
+        label = str(previous_node.label).split(" - ", maxsplit=1)[0]
         return label
```

### Comparing `cobib-4.1.0/src/cobib/ui/components/main_content.py` & `cobib-4.2.0/src/cobib/ui/components/main_content.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,16 +23,14 @@
 
     DEFAULT_CSS = """
         MainContent {
             width: 2fr;
         }
     """
 
-    # TODO: add a validation hook to the mount method to prevent widgets of "wrong" type?
-
     def get_current_label(self) -> str:
         """Gets the label of the entry currently under the cursor.
 
         Raises:
             NoMatches: when `current` is `None`.
 
         Returns:
```

### Comparing `cobib-4.1.0/src/cobib/ui/components/motion_key.py` & `cobib-4.2.0/src/cobib/ui/components/motion_key.py`

 * *Files identical despite different names*

### Comparing `cobib-4.1.0/src/cobib/ui/components/popup.py` & `cobib-4.2.0/src/cobib/ui/components/popup.py`

 * *Files identical despite different names*

### Comparing `cobib-4.1.0/src/cobib/ui/components/popup_logging_handler.py` & `cobib-4.2.0/src/cobib/ui/components/popup_logging_handler.py`

 * *Files identical despite different names*

### Comparing `cobib-4.1.0/src/cobib/ui/components/popup_panel.py` & `cobib-4.2.0/src/cobib/ui/components/popup_panel.py`

 * *Files identical despite different names*

### Comparing `cobib-4.1.0/src/cobib/ui/components/progress.py` & `cobib-4.2.0/src/cobib/ui/components/progress.py`

 * *Files identical despite different names*

### Comparing `cobib-4.1.0/src/cobib/ui/components/prompt.py` & `cobib-4.2.0/src/cobib/ui/components/prompt.py`

 * *Files identical despite different names*

### Comparing `cobib-4.1.0/src/cobib/ui/components/search_view.py` & `cobib-4.2.0/src/cobib/ui/components/list_view.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-"""coBib's search results viewer widget.
+"""coBib's list results viewer widget.
 
-This widget gets produces by `cobib.commands.search.SearchCommand.render_textual`.
-It subclasses textual's built-in `Tree` widget.
+This widget gets produces by `cobib.commands.list.ListCommand.render_textual`.
+It subclasses textual's built-in `DataTable` widget.
 
 .. warning::
 
    This module makes no API stability guarantees! Refer to `cobib.ui.components` for more details.
 """
 
 from __future__ import annotations
 
 from rich.text import Text
 from textual.binding import Binding
-from textual.css.query import NoMatches
-from textual.reactive import reactive
-from textual.widgets import Tree
+from textual.coordinate import Coordinate
+from textual.geometry import Region, clamp
+from textual.widgets import DataTable
+from typing_extensions import override
 
-from .motion_key import MotionKey
+from cobib.config import config
 
+from .motion_key import MotionKey
 
-class SearchView(Tree[Text]):
-    """coBib's search results viewer widget."""
 
-    id = "cobib-search-view"
+class ListView(DataTable[Text]):
+    """coBib's list results viewer widget."""
 
-    show_root = reactive(False)
+    id = "cobib-list-view"
 
     BINDINGS = [
         Binding("j", "motion('down', 'cursor_down')", "Down", show=False),
         Binding("k", "motion('up', 'cursor_up')", "Up", show=False),
         Binding("h", "motion('left', 'cursor_left')", "Left", show=False),
         Binding("l", "motion('right', 'cursor_right')", "Right", show=False),
         Binding("down", "motion('down', 'cursor_down')", "Down", show=False),
@@ -43,14 +44,42 @@
     | space | Toggle the expand/collapsed space of the current item. |
     | j, down | Moves one row down. |
     | k, up | Moves one row up. |
     | h, left | Moves to the left. |
     | l, right | Moves to the right. |
     """
 
+    DEFAULT_CSS = """
+        ListView {
+            height: 1fr;
+        }
+    """
+
+    @property
+    @override
+    def scrollable_content_region(self) -> Region:
+        # we shrink the scroll-able content region by the scroll offset at the bottom
+        # NOTE: shrinking at the top does not seem to yield the intended result as it merely adds to
+        # the offset at the bottom
+        return super().scrollable_content_region.shrink((0, 0, config.tui.scroll_offset, 0))
+
+    @override
+    def validate_scroll_y(self, value: float) -> float:
+        # we implement the scroll offset at the top by forcing the scroll y value to be at
+        # least an offset away from the cursor row
+        if self.cursor_row - value < config.tui.scroll_offset:
+            value = self.cursor_row - config.tui.scroll_offset
+        return clamp(value, 0, self.row_count)
+
+    @override
+    def on_mount(self) -> None:
+        self.fixed_columns = 1
+        self.zebra_stripes = True
+        self.cursor_type = "row"
+
     def action_motion(self, key: str, action: str) -> None:
         """Action to move the cursor.
 
         Under the hood, this delegates to the respective built-in cursor motion methods.
         However, this method also posts a `cobib.ui.components.motion_key.MotionKey` event.
 
         Args:
@@ -64,16 +93,9 @@
 
     def get_current_label(self) -> str:
         """Gets the label of the entry currently under the cursor.
 
         Returns:
             The label of the entry currently under the cursor.
         """
-        previous_node, current_node = self.cursor_node, self.cursor_node
-        if current_node is None:
-            raise NoMatches  # pylint: disable=raise-missing-from
-        while current_node.parent is not None:
-            previous_node, current_node = current_node, current_node.parent
-        if previous_node is None:
-            raise NoMatches  # pylint: disable=raise-missing-from
-        label = str(previous_node.label).split(" - ", maxsplit=1)[0]
+        label = self.get_cell_at(Coordinate(self.cursor_row, 0)).plain
         return label
```

### Comparing `cobib-4.1.0/src/cobib/ui/components/selection_filter.py` & `cobib-4.2.0/src/cobib/ui/components/selection_filter.py`

 * *Files identical despite different names*

### Comparing `cobib-4.1.0/src/cobib/ui/shell_helper.py` & `cobib-4.2.0/src/cobib/ui/shell_helper.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 from typing_extensions import override
 
 from cobib.ui.ui import UI
 from cobib.utils import shell_helper
 
 LOGGER = logging.getLogger(__name__)
+"""@private module logger."""
 
 
 class ShellHelper(UI):
     """The shell-helper interface class.
 
     In addition to the global arguments documented by the base class, the following are supported:
```

### Comparing `cobib-4.1.0/src/cobib/ui/tui.py` & `cobib-4.2.0/src/cobib/ui/tui.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,24 +27,26 @@
 from textual.keys import Keys
 from textual.logging import TextualHandler
 from textual.widget import AwaitMount, Widget
 from textual.widgets import Footer, Header, Input, Static
 from typing_extensions import override
 
 from cobib import commands
+from cobib.config import config
 from cobib.ui.components import (
     EntryView,
     HelpScreen,
     InputScreen,
     ListView,
     MainContent,
     MotionKey,
     Popup,
     PopupLoggingHandler,
     PopupPanel,
+    PresetFilterScreen,
     Progress,
     Prompt,
     SearchView,
     SelectionFilter,
 )
 from cobib.ui.ui import UI
 from cobib.utils.file_downloader import FileDownloader
@@ -81,69 +83,75 @@
     DEFAULT_CSS = """
         Screen {
             layers: default popup overlay;
             align-vertical: bottom;
         }
     """
 
+    _PRESET_FILTER_BINDINGS = [(f"{i}", f"preset_filter({i})", f"Preset #{i}") for i in range(10)]
     BINDINGS = [
         ("q", "quit", "Quit"),
         ("question_mark", "push_screen('help')", "Help"),
         ("underscore", "toggle_layout", "Layout"),
         ("colon", "prompt(':')", "Prompt"),
         ("v", "select", "Select"),
         ("slash", "prompt('/')", "Search"),
         ("a", "prompt('add ')", "Add"),
         ("d", "delete", "Delete"),
         ("e", "edit", "Edit"),
         ("f", "filter", "Filter"),
         ("i", "prompt('import ')", "Import"),
         ("m", "prompt('modify ', False, True)", "Modify"),
         ("o", "open", "Open"),
+        ("p", "preset_filter()", "Preset"),
         ("r", "prompt('redo', True)", "Redo"),
         ("s", "sort", "Sort"),
         ("u", "prompt('undo', True)", "Undo"),
         ("x", "prompt('export ', False, True)", "Export"),
+        *_PRESET_FILTER_BINDINGS,
     ]
     """
     | Key(s) | Description |
     | :- | :- |
     | q | Quit's coBib. |
     | ? | Toggles the help screen. |
     | _ | Toggles between the horizontal and vertical layout. |
-    | space | Toggles folding of a search result. |
     | : | Starts the prompt for an arbitrary coBib command. |
     | v | Selects the current entry. |
     | / | Searches the database for the provided string. |
+    | digit | Immediately selects the preset filter given by that digit (0 = reset). |
     | a | Prompts for a new entry to be added to the database. |
     | d | Deletes the current (or selected) entries. |
     | e | Edits the current entry. |
     | f | Allows filtering the table using `++/--` keywords. |
     | i | Imports entries from another source. |
     | m | Prompts for a modification (respects selection). |
     | o | Opens the current (or selected) entries. |
+    | p | Allows selecting a preset filter (see `config.tui.preset_filters`). |
     | r | Redoes the last undone change. Requires git-tracking! |
     | s | Prompts for the field to sort by (use -r to list in reverse). |
     | u | Undes the last change. Requires git-tracking! |
     | x | Exports the current (or selected) entries. |
     """
 
     SCREENS = {
         "help": HelpScreen,
         "input": InputScreen,
+        "preset_filter": PresetFilterScreen,
     }
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         """Initializes the TUI.
 
         Args:
             *args: any positional arguments for textual's underlying `App` class.
             **kwargs: any keyword arguments for textual's underlying `App` class.
         """
         super().__init__(*args, **kwargs)
+        self.console.push_theme(config.theme.build())
         self.root_logger.addHandler(TextualHandler())
         self.title = "coBib"
         self.sub_title = "The Console Bibliography Manager"
         self._list_args = ["-r"]
         self._filter: SelectionFilter = SelectionFilter()
         self._filters.append(self._filter)
         self._background_tasks: set[asyncio.Task] = set()  # type: ignore[type-arg]
@@ -354,14 +362,33 @@
             labels = list(self._filter.selection)
             self._filter.selection.clear()
         else:
             labels = [main.get_current_label()]
 
         self._run_command(["open"] + labels)
 
+    async def action_preset_filter(self, idx: int | None = None) -> None:
+        """The preset filter selection action.
+
+        This action selects (or prompts for) a preset filter from `config.tui.preset_filters`.
+
+        Args:
+            idx: the index of which preset filter to select. When this is `None`, the user will be
+                prompted interactively. When `0`, all filters will be reset.
+        """
+        if idx is None:
+            await_mount = self.push_screen("preset_filter", self._process_input)
+            await await_mount
+        else:
+            idx = int(idx)
+            if idx == 0:
+                await self._process_input("list -r")
+            elif idx <= len(config.tui.preset_filters):
+                await self._process_input(f"list {config.tui.preset_filters[idx-1]}")
+
     async def action_filter(self) -> None:
         """The filter action.
 
         This action triggers the `cobib.commands.list.ListCommand` via the `action_prompt` and
         allows the user to provide additional filters.
         """
         await self.action_prompt("list " + " ".join(self._list_args) + " ")
@@ -412,21 +439,26 @@
             show_cmd.render_rich(
                 background_color=entry.background_colors[1].rich_color.name,
             )
         )
 
     async def _update_table(self) -> None:
         """Updates the list of entries displayed in the `MainContent`."""
-        # TODO: retain scroll position
+        main = self.query_one(MainContent)
+        old_table = main.query_one(ListView)
         command = commands.ListCommand(*self._list_args)
         command.execute()
         table = command.render_textual()
-        main = self.query_one(MainContent)
         await main.replace_widget(table)
         table.focus()
+        if old_table is not None:
+            table.cursor_coordinate = old_table.cursor_coordinate
+            table.scroll_x = old_table.scroll_x
+            table.scroll_y = old_table.scroll_y
+            del old_table
         self.refresh(layout=True)
 
     async def _update_tree(self, command: list[str]) -> None:
         """Updates the tree of search results displayed in the `MainContent`."""
         subcmd = commands.SearchCommand(*command)
         subcmd.execute()
         tree = subcmd.render_textual()
```

### Comparing `cobib-4.1.0/src/cobib/ui/ui.py` & `cobib-4.2.0/src/cobib/ui/ui.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from typing import Any
 
 from cobib.config import config
 from cobib.ui.components import ArgumentParser
 from cobib.utils.logging import get_file_handler, get_stream_handler
 
 LOGGER = logging.getLogger(__name__)
+"""@private module logger."""
 
 
 class UI:
     """The UI base class.
 
     The following global arguments can be parsed:
```

### Comparing `cobib-4.1.0/src/cobib/utils/diff_renderer.py` & `cobib-4.2.0/src/cobib/utils/diff_renderer.py`

 * *Files identical despite different names*

### Comparing `cobib-4.1.0/src/cobib/utils/file_downloader.py` & `cobib-4.2.0/src/cobib/utils/file_downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from textual.app import App
 
 from cobib.config import Event, config
 
 from .rel_path import RelPath
 
 LOGGER = logging.getLogger(__name__)
+"""@private module logger."""
 
 
 class FileDownloader:
     """The file downloader singleton.
 
     This utility centralizes the downloading of associated files.
     """
```

### Comparing `cobib-4.1.0/src/cobib/utils/journal_abbreviations.py` & `cobib-4.2.0/src/cobib/utils/journal_abbreviations.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import logging
 from typing import Callable, Dict, Optional
 
 from cobib.config import config
 
 LOGGER = logging.getLogger(__name__)
+"""@private module logger."""
 
 
 class JournalAbbreviations:
     """The Journal abbreviation singleton.
 
     This utility centralizes coBib's methodology of converting between full and abbreviated journal
     names. It implements the singleton pattern to enforce consistency across all modules.
```

### Comparing `cobib-4.1.0/src/cobib/utils/logging.py` & `cobib-4.2.0/src/cobib/utils/logging.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 from rich.markdown import Markdown
 from rich.panel import Panel
 from rich.text import Text
 from typing_extensions import override
 
 from .rel_path import RelPath
 
+# NOTE: we add a custom HINT level which has a higher priority than WARNING and, thus, can be used
+# to provide information to the user that might be useful to see at runtime.
+logging.addLevelName(35, "HINT")
+
 
 class _StderrHandler(logging.StreamHandler):  # type: ignore[type-arg]
     """A logging handler hard-coded to `sys.stderr`.
 
     The reason for explicitly deriving this class, is that Python's `logging.StreamHandler` does not
     respect stream redirection. However, for coBib's TUI this is an important requirement which can
     be achieved by a runtime check of the stream during the `emit` method.
```

### Comparing `cobib-4.1.0/src/cobib/utils/rel_path.py` & `cobib-4.2.0/src/cobib/utils/rel_path.py`

 * *Files identical despite different names*

### Comparing `cobib-4.1.0/src/cobib/utils/shell_helper.py` & `cobib-4.2.0/src/cobib/utils/shell_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from rich.console import Console
 from rich.prompt import PromptBase, PromptType
 from textual.app import App
 
 from .rel_path import RelPath
 
 LOGGER = logging.getLogger(__name__)
+"""@private module logger."""
 
 
 def list_commands(*args: str) -> List[str]:
     """Lists all available subcommands.
 
     Args:
         args: a sequence of additional arguments used for the execution. None are supported yet.
```

### Comparing `cobib-4.1.0/src/cobib.egg-info/PKG-INFO` & `cobib-4.2.0/src/cobib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cobib
-Version: 4.1.0
+Version: 4.2.0
 Summary: Console Bibliography
 Home-page: https://gitlab.com/cobib/cobib
 Author: Max Rossmannek
 Author-email: max.rossmannek@uzh.ch
 License: MIT License
 Project-URL: Bug Tracker, https://gitlab.com/cobib/cobib/-/issues
 Project-URL: Documentation, https://cobib.gitlab.io/cobib/cobib.html
@@ -289,14 +289,50 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
 
+## [4.2.0] - 2023-08-08
+
+Pypi: https://pypi.org/project/cobib/4.2.0/
+
+### Added
+- added the `config.tui.scroll_offset` setting
+- added the `--field` command line option to the `open` command
+- (DEV) added a new `HINT` logging level which has value 35 and thus allows to
+  provide information to the user with a higher priority than `WARNING`
+- added the new `config.tui.preset_filters` (#114)
+  - preset filters can be selected from the TUI via the `p` key binding
+  - the first 9 filters can be selected directly by pressing the respective number
+  - pressing `0` resets any applied filter
+- implemented special tags (#63,!83)
+  - adds new builtin tags which will trigger special highlights of entries: `new`, `high`, `medium`, `low`
+  - adds the new `config.theme` settings section for configuring these settings
+  - you can also add more special tags via `config.theme.tags.user_tags`
+- added the `--skip-files` command line option to the `search` command
+
+### Changed
+- unicode symbols in entry labels will now be replaced with ascii ones (#119,#120)
+  - this is configured via the `config.database.format.default_label` setting, so if you are using a
+    custom value for this, be sure to update your config to make use of this feature
+- some user-visible logging messages around label disambiguation have been added (see also #121)
+- a warning has been added when the YAML parser encounters identical labels (which normally should
+  not occur in the database but if it does, coBib does not really know how to resolve this)
+- DOI redirect links are now followed recursively (up to 3 times), improving PDF
+  download link detection in the process (#97)
+
+### Deprecated
+- the `config.commands.search.highlights` section is deprecated in favor of `config.theme.search`
+
+### Fixed
+- retain scroll position in the TUI's list view
+
+
 ## [4.1.0] - 2023-06-11
 
 Pypi: https://pypi.org/project/cobib/4.1.0/
 
 ### Added
 - added the following settings which specify whether or not to preserve
   associated files during the respective commands being run:
@@ -1049,15 +1085,16 @@
 
 ## [0.1] - 2019-04-29
 
 ### Added
 - initial version with a basic `sqlite3`-based database
 
 
-[Unreleased]: https://gitlab.com/cobib/cobib/-/compare/v4.1.0...master
+[Unreleased]: https://gitlab.com/cobib/cobib/-/compare/v4.2.0...master
+[4.2.0]: https://gitlab.com/cobib/cobib/-/compare/v4.2.0
 [4.1.0]: https://gitlab.com/cobib/cobib/-/compare/v4.1.0
 [4.0.0]: https://gitlab.com/cobib/cobib/-/compare/v4.0.0
 [3.5.5]: https://gitlab.com/cobib/cobib/-/compare/v3.5.5
 [3.5.4]: https://gitlab.com/cobib/cobib/-/compare/v3.5.4
 [3.5.3]: https://gitlab.com/cobib/cobib/-/compare/v3.5.3
 [3.5.2]: https://gitlab.com/cobib/cobib/-/compare/v3.5.2
 [3.5.1]: https://gitlab.com/cobib/cobib/-/compare/v3.5.1
```

### Comparing `cobib-4.1.0/tests/test_main.py` & `cobib-4.2.0/tests/test_main.py`

 * *Files identical despite different names*

