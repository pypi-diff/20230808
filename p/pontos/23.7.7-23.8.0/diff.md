# Comparing `tmp/pontos-23.7.7.tar.gz` & `tmp/pontos-23.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pontos-23.7.7.tar", max compression
+gzip compressed data, was "pontos-23.8.0.tar", max compression
```

## Comparing `pontos-23.7.7.tar` & `pontos-23.8.0.tar`

### file list

```diff
@@ -1,257 +1,260 @@
--rw-r--r--   0        0        0    35149 2023-07-19 14:09:56.552589 pontos-23.7.7/LICENSE
--rw-r--r--   0        0        0     3836 2023-07-19 14:09:56.552589 pontos-23.7.7/README.md
--rw-r--r--   0        0        0    92794 2023-07-19 14:09:56.556589 pontos-23.7.7/poetry.lock
--rw-r--r--   0        0        0       32 2023-07-19 14:09:56.556589 pontos-23.7.7/poetry.toml
--rw-r--r--   0        0        0      791 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/__init__.py
--rw-r--r--   0        0        0     1007 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/changelog/__init__.py
--rw-r--r--   0        0        0    12175 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/changelog/conventional_commits.py
--rw-r--r--   0        0        0      965 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/changelog/errors.py
--rw-r--r--   0        0        0     4396 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/changelog/main.py
--rw-r--r--   0        0        0      806 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/errors.py
--rw-r--r--   0        0        0      882 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/git/__init__.py
--rw-r--r--   0        0        0    18039 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/git/git.py
--rw-r--r--   0        0        0     2538 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/git/status.py
--rw-r--r--   0        0        0      760 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/github/__init__.py
--rw-r--r--   0        0        0     1166 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/github/actions/__init__.py
--rw-r--r--   0        0        0     2239 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/github/actions/argparser.py
--rw-r--r--   0        0        0     1472 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/github/actions/cmds.py
--rw-r--r--   0        0        0     7342 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/github/actions/core.py
--rw-r--r--   0        0        0     2426 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/github/actions/env.py
--rw-r--r--   0        0        0      861 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/github/actions/errors.py
--rw-r--r--   0        0        0     4186 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/github/actions/event.py
--rw-r--r--   0        0        0     1100 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/github/actions/main.py
--rw-r--r--   0        0        0     2047 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/github/api/__init__.py
--rw-r--r--   0        0        0     5531 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/github/api/api.py
--rw-r--r--   0        0        0     6210 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/github/api/artifacts.py
--rw-r--r--   0        0        0    34561 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/github/api/branch.py
--rw-r--r--   0        0        0     9395 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/github/api/client.py
--rw-r--r--   0        0        0     1844 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/github/api/contents.py
--rw-r--r--   0        0        0      845 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/github/api/errors.py
--rw-r--r--   0        0        0     1320 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/github/api/helper.py
--rw-r--r--   0        0        0     2813 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/github/api/labels.py
--rw-r--r--   0        0        0    10311 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/github/api/organizations.py
--rw-r--r--   0        0        0    13090 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/github/api/pull_requests.py
--rw-r--r--   0        0        0    12280 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/github/api/release.py
--rw-r--r--   0        0        0    21512 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/github/api/repositories.py
--rw-r--r--   0        0        0     3276 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/github/api/search.py
--rw-r--r--   0        0        0     6004 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/github/api/tags.py
--rw-r--r--   0        0        0    15235 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/github/api/teams.py
--rw-r--r--   0        0        0     9182 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/github/api/workflows.py
--rw-r--r--   0        0        0    11128 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/github/argparser.py
--rw-r--r--   0        0        0     8863 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/github/cmds.py
--rw-r--r--   0        0        0     1347 2023-07-19 14:09:56.556589 pontos-23.7.7/pontos/github/main.py
--rw-r--r--   0        0        0     1134 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/github/models/__init__.py
--rw-r--r--   0        0        0     2336 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/github/models/artifact.py
--rw-r--r--   0        0        0     7532 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/github/models/base.py
--rw-r--r--   0        0        0     6915 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/github/models/branch.py
--rw-r--r--   0        0        0    16573 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/github/models/organization.py
--rw-r--r--   0        0        0    14248 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/github/models/pull_request.py
--rw-r--r--   0        0        0     4607 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/github/models/release.py
--rw-r--r--   0        0        0     4299 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/github/models/search.py
--rw-r--r--   0        0        0     4606 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/github/models/tag.py
--rw-r--r--   0        0        0    11477 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/github/models/workflow.py
--rw-r--r--   0        0        0      790 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/github/pr_template.md
--rw-r--r--   0        0        0     3443 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/github/script/__init__.py
--rw-r--r--   0        0        0      835 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/github/script/errors.py
--rw-r--r--   0        0        0     5403 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/github/script/load.py
--rw-r--r--   0        0        0     1495 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/github/script/parser.py
--rw-r--r--   0        0        0        0 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/github/scripts/__init__.py
--rw-r--r--   0        0        0     1872 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/github/scripts/artifacts-download.py
--rw-r--r--   0        0        0     1862 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/github/scripts/artifacts.py
--rw-r--r--   0        0        0     1605 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/github/scripts/branchprotection.py
--rw-r--r--   0        0        0     5606 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/github/scripts/create-repository.py
--rw-r--r--   0        0        0     2212 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/github/scripts/enforce-admins.py
--rw-r--r--   0        0        0     1834 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/github/scripts/lock-branch.py
--rw-r--r--   0        0        0     2577 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/github/scripts/members.py
--rw-r--r--   0        0        0     2179 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/github/scripts/release-assets-download.py
--rw-r--r--   0        0        0     2294 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/github/scripts/repositories.py
--rw-r--r--   0        0        0     6717 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/github/scripts/search-repositories.py
--rw-r--r--   0        0        0     3689 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/github/scripts/team-repositories.py
--rw-r--r--   0        0        0     1654 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/github/scripts/teams.py
--rw-r--r--   0        0        0     2789 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/github/scripts/workflow-runs.py
--rw-r--r--   0        0        0    14844 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/helper.py
--rw-r--r--   0        0        0     6235 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/models/__init__.py
--rw-r--r--   0        0        0      864 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/nvd/__init__.py
--rw-r--r--   0        0        0     4732 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/nvd/api.py
--rw-r--r--   0        0        0     2177 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/nvd/cpe/__init__.py
--rw-r--r--   0        0        0     7339 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/nvd/cpe/api.py
--rw-r--r--   0        0        0     2651 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/nvd/cve/__init__.py
--rw-r--r--   0        0        0    11470 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/nvd/cve/api.py
--rw-r--r--   0        0        0      716 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/nvd/models/__init__.py
--rw-r--r--   0        0        0     2973 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/nvd/models/cpe.py
--rw-r--r--   0        0        0     7250 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/nvd/models/cve.py
--rw-r--r--   0        0        0     3254 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/nvd/models/cvss_v2.py
--rw-r--r--   0        0        0     4471 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/nvd/models/cvss_v3.py
--rw-r--r--   0        0        0     3561 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/pontos.py
--rw-r--r--   0        0        0        0 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/py.typed
--rw-r--r--   0        0        0     1176 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/release/__init__.py
--rw-r--r--   0        0        0     2472 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/release/helper.py
--rw-r--r--   0        0        0     2127 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/release/main.py
--rw-r--r--   0        0        0     8407 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/release/parser.py
--rw-r--r--   0        0        0    14739 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/release/release.py
--rw-r--r--   0        0        0    12868 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/release/sign.py
--rw-r--r--   0        0        0      886 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/terminal/__init__.py
--rw-r--r--   0        0        0     1770 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/terminal/null.py
--rw-r--r--   0        0        0     5050 2023-07-19 14:09:56.560590 pontos-23.7.7/pontos/terminal/rich.py
--rw-r--r--   0        0        0     9416 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/terminal/terminal.py
--rw-r--r--   0        0        0     7231 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/testing/__init__.py
--rw-r--r--   0        0        0      971 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/typing/__init__.py
--rw-r--r--   0        0        0      773 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/__init__.py
--rw-r--r--   0        0        0      838 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/__main__.py
--rw-r--r--   0        0        0      102 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash
--rw-r--r--   0        0        0       97 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.c
--rw-r--r--   0        0        0       90 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake
--rw-r--r--   0        0        0       93 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.go
--rw-r--r--   0        0        0       97 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.h
--rw-r--r--   0        0        0       97 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.js
--rw-r--r--   0        0        0      224 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl
--rw-r--r--   0        0        0       90 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.po
--rw-r--r--   0        0        0       90 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.py
--rw-r--r--   0        0        0      100 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh
--rw-r--r--   0        0        0       85 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt
--rw-r--r--   0        0        0      117 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml
--rw-r--r--   0        0        0      117 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl
--rw-r--r--   0        0        0       92 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/GPL-2.0-only/template.c
--rw-r--r--   0        0        0       92 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/GPL-2.0-only/template.h
--rw-r--r--   0        0        0      219 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/GPL-2.0-only/template.nasl
--rw-r--r--   0        0        0      101 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/GPL-2.0-or-later/template.bash
--rw-r--r--   0        0        0       96 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/GPL-2.0-or-later/template.c
--rw-r--r--   0        0        0       89 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake
--rw-r--r--   0        0        0       96 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/GPL-2.0-or-later/template.h
--rw-r--r--   0        0        0       96 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/GPL-2.0-or-later/template.js
--rw-r--r--   0        0        0      223 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/GPL-2.0-or-later/template.nasl
--rw-r--r--   0        0        0       89 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/GPL-2.0-or-later/template.po
--rw-r--r--   0        0        0       89 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/GPL-2.0-or-later/template.py
--rw-r--r--   0        0        0       99 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/GPL-2.0-or-later/template.sh
--rw-r--r--   0        0        0       84 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/GPL-2.0-or-later/template.txt
--rw-r--r--   0        0        0      116 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/GPL-2.0-or-later/template.xml
--rw-r--r--   0        0        0      116 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/GPL-2.0-or-later/template.xsl
--rw-r--r--   0        0        0      101 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/GPL-3.0-or-later/template.bash
--rw-r--r--   0        0        0       96 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/GPL-3.0-or-later/template.c
--rw-r--r--   0        0        0       89 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/GPL-3.0-or-later/template.cmake
--rw-r--r--   0        0        0       92 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/GPL-3.0-or-later/template.go
--rw-r--r--   0        0        0       96 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/GPL-3.0-or-later/template.h
--rw-r--r--   0        0        0       96 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/GPL-3.0-or-later/template.js
--rw-r--r--   0        0        0      223 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/GPL-3.0-or-later/template.nasl
--rw-r--r--   0        0        0       89 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/GPL-3.0-or-later/template.po
--rw-r--r--   0        0        0       89 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/GPL-3.0-or-later/template.py
--rw-r--r--   0        0        0       99 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/GPL-3.0-or-later/template.sh
--rw-r--r--   0        0        0       84 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/GPL-3.0-or-later/template.txt
--rw-r--r--   0        0        0      116 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/GPL-3.0-or-later/template.xml
--rw-r--r--   0        0        0      116 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/templates/GPL-3.0-or-later/template.xsl
--rw-r--r--   0        0        0    12149 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/updateheader/updateheader.py
--rw-r--r--   0        0        0     1079 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/version/__init__.py
--rw-r--r--   0        0        0      816 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/version/__main__.py
--rw-r--r--   0        0        0      103 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/version/__version__.py
--rw-r--r--   0        0        0     8837 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/version/_calculator.py
--rw-r--r--   0        0        0     1596 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/version/commands/__init__.py
--rw-r--r--   0        0        0     2871 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/version/commands/_cargo.py
--rw-r--r--   0        0        0     7901 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/version/commands/_cmake.py
--rw-r--r--   0        0        0     2553 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/version/commands/_command.py
--rw-r--r--   0        0        0     3816 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/version/commands/_go.py
--rw-r--r--   0        0        0     6577 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/version/commands/_java.py
--rw-r--r--   0        0        0     6512 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/version/commands/_javascript.py
--rw-r--r--   0        0        0     8479 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/version/commands/_python.py
--rw-r--r--   0        0        0      961 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/version/errors.py
--rw-r--r--   0        0        0     2812 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/version/helper.py
--rw-r--r--   0        0        0     3655 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/version/main.py
--rw-r--r--   0        0        0     4163 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/version/parser.py
--rw-r--r--   0        0        0     3750 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/version/project.py
--rw-r--r--   0        0        0     2163 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/version/schemes/__init__.py
--rw-r--r--   0        0        0    13835 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/version/schemes/_pep440.py
--rw-r--r--   0        0        0     2159 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/version/schemes/_scheme.py
--rw-r--r--   0        0        0    16450 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/version/schemes/_semantic.py
--rw-r--r--   0        0        0     5604 2023-07-19 14:09:56.564590 pontos-23.7.7/pontos/version/version.py
--rw-r--r--   0        0        0     3043 2023-07-19 14:09:56.564590 pontos-23.7.7/pyproject.toml
--rw-r--r--   0        0        0     1518 2023-07-19 14:09:56.564590 pontos-23.7.7/tests/__init__.py
--rw-r--r--   0        0        0     1031 2023-07-19 14:09:56.564590 pontos-23.7.7/tests/changelog/__init__.py
--rw-r--r--   0        0        0      375 2023-07-19 14:09:56.564590 pontos-23.7.7/tests/changelog/changelog.toml
--rw-r--r--   0        0        0    19105 2023-07-19 14:09:56.564590 pontos-23.7.7/tests/changelog/test_conventional_commits.py
--rw-r--r--   0        0        0     1925 2023-07-19 14:09:56.564590 pontos-23.7.7/tests/changelog/test_parser.py
--rw-r--r--   0        0        0       69 2023-07-19 14:09:56.568590 pontos-23.7.7/tests/fake_pyproject.toml
--rw-r--r--   0        0        0      716 2023-07-19 14:09:56.568590 pontos-23.7.7/tests/git/__init__.py
--rw-r--r--   0        0        0    32267 2023-07-19 14:09:56.568590 pontos-23.7.7/tests/git/test_git.py
--rw-r--r--   0        0        0     4215 2023-07-19 14:09:56.568590 pontos-23.7.7/tests/git/test_status.py
--rw-r--r--   0        0        0      716 2023-07-19 14:09:56.568590 pontos-23.7.7/tests/github/__init__.py
--rw-r--r--   0        0        0      716 2023-07-19 14:09:56.568590 pontos-23.7.7/tests/github/actions/__init__.py
--rw-r--r--   0        0        0    29628 2023-07-19 14:09:56.568590 pontos-23.7.7/tests/github/actions/test-pull-request-event.json
--rw-r--r--   0        0        0     5469 2023-07-19 14:09:56.568590 pontos-23.7.7/tests/github/actions/test_core.py
--rw-r--r--   0        0        0     3534 2023-07-19 14:09:56.568590 pontos-23.7.7/tests/github/actions/test_env.py
--rw-r--r--   0        0        0     2086 2023-07-19 14:09:56.568590 pontos-23.7.7/tests/github/actions/test_event.py
--rw-r--r--   0        0        0     1232 2023-07-19 14:09:56.568590 pontos-23.7.7/tests/github/api/__init__.py
--rw-r--r--   0        0        0    20021 2023-07-19 14:09:56.568590 pontos-23.7.7/tests/github/api/pr-files.json
--rw-r--r--   0        0        0     5624 2023-07-19 14:09:56.568590 pontos-23.7.7/tests/github/api/release-response.json
--rw-r--r--   0        0        0    12076 2023-07-19 14:09:56.568590 pontos-23.7.7/tests/github/api/test_artifacts.py
--rw-r--r--   0        0        0    20096 2023-07-19 14:09:56.568590 pontos-23.7.7/tests/github/api/test_branch.py
--rw-r--r--   0        0        0     9619 2023-07-19 14:09:56.568590 pontos-23.7.7/tests/github/api/test_client.py
--rw-r--r--   0        0        0     2087 2023-07-19 14:09:56.568590 pontos-23.7.7/tests/github/api/test_contents.py
--rw-r--r--   0        0        0     2801 2023-07-19 14:09:56.568590 pontos-23.7.7/tests/github/api/test_labels.py
--rw-r--r--   0        0        0    71096 2023-07-19 14:09:56.568590 pontos-23.7.7/tests/github/api/test_organizations.py
--rw-r--r--   0        0        0    58547 2023-07-19 14:09:56.568590 pontos-23.7.7/tests/github/api/test_pull_requests.py
--rw-r--r--   0        0        0    17842 2023-07-19 14:09:56.568590 pontos-23.7.7/tests/github/api/test_release.py
--rw-r--r--   0        0        0    37847 2023-07-19 14:09:56.568590 pontos-23.7.7/tests/github/api/test_repositories.py
--rw-r--r--   0        0        0    24490 2023-07-19 14:09:56.568590 pontos-23.7.7/tests/github/api/test_search.py
--rw-r--r--   0        0        0     9490 2023-07-19 14:09:56.568590 pontos-23.7.7/tests/github/api/test_tags.py
--rw-r--r--   0        0        0    39045 2023-07-19 14:09:56.568590 pontos-23.7.7/tests/github/api/test_teams.py
--rw-r--r--   0        0        0   129346 2023-07-19 14:09:56.568590 pontos-23.7.7/tests/github/api/test_workflows.py
--rw-r--r--   0        0        0      716 2023-07-19 14:09:56.568590 pontos-23.7.7/tests/github/models/__init__.py
--rw-r--r--   0        0        0     3210 2023-07-19 14:09:56.568590 pontos-23.7.7/tests/github/models/test_artifact.py
--rw-r--r--   0        0        0     9831 2023-07-19 14:09:56.568590 pontos-23.7.7/tests/github/models/test_base.py
--rw-r--r--   0        0        0    31873 2023-07-19 14:09:56.568590 pontos-23.7.7/tests/github/models/test_branch.py
--rw-r--r--   0        0        0    19893 2023-07-19 14:09:56.568590 pontos-23.7.7/tests/github/models/test_organization.py
--rw-r--r--   0        0        0    80894 2023-07-19 14:09:56.568590 pontos-23.7.7/tests/github/models/test_pull_request.py
--rw-r--r--   0        0        0    12062 2023-07-19 14:09:56.568590 pontos-23.7.7/tests/github/models/test_release.py
--rw-r--r--   0        0        0     2216 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/github/models/test_search.py
--rw-r--r--   0        0        0     3419 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/github/models/test_tag.py
--rw-r--r--   0        0        0    41463 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/github/models/test_workflow.py
--rw-r--r--   0        0        0      716 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/github/script/__init__.py
--rw-r--r--   0        0        0     3863 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/github/script/test_load.py
--rw-r--r--   0        0        0     2052 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/github/script/test_parser.py
--rw-r--r--   0        0        0     6371 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/github/test_argparser.py
--rw-r--r--   0        0        0     9562 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/github/test_cmds.py
--rw-r--r--   0        0        0      716 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/models/__init__.py
--rw-r--r--   0        0        0     6424 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/models/test_models.py
--rw-r--r--   0        0        0     2505 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/nvd/__init__.py
--rw-r--r--   0        0        0      716 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/nvd/cpe/__init__.py
--rw-r--r--   0        0        0    11290 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/nvd/cpe/test_api.py
--rw-r--r--   0        0        0      716 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/nvd/cve/__init__.py
--rw-r--r--   0        0        0    26602 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/nvd/cve/test_api.py
--rw-r--r--   0        0        0      716 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/nvd/models/__init__.py
--rw-r--r--   0        0        0     3725 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/nvd/models/test_cpe.py
--rw-r--r--   0        0        0    25930 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/nvd/models/test_cve.py
--rw-r--r--   0        0        0     3994 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/nvd/test_api.py
--rw-r--r--   0        0        0      721 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/release/__init__.py
--rw-r--r--   0        0        0     3265 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/release/test_helper.py
--rw-r--r--   0        0        0     9243 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/release/test_parser.py
--rw-r--r--   0        0        0    83503 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/release/test_release.py
--rw-r--r--   0        0        0    25286 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/release/test_sign.py
--rw-r--r--   0        0        0      345 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/release/v1.2.3.md
--rw-r--r--   0        0        0      745 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/terminal/__init__.py
--rw-r--r--   0        0        0     6653 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/terminal/test_terminal.py
--rw-r--r--   0        0        0    20488 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/test_helper.py
--rw-r--r--   0        0        0     1685 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/test_pontos.py
--rw-r--r--   0        0        0      716 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/testing/__init__.py
--rw-r--r--   0        0        0     8007 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/testing/test_testing.py
--rw-r--r--   0        0        0      716 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/typing/__init__.py
--rw-r--r--   0        0        0     1120 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/typing/test_typing.py
--rw-r--r--   0        0        0      721 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/updateheader/__init__.py
--rw-r--r--   0        0        0    15848 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/updateheader/test_header.py
--rw-r--r--   0        0        0     1031 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/version/__init__.py
--rw-r--r--   0        0        0      727 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/version/commands/__init__.py
--rw-r--r--   0        0        0     3847 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/version/commands/test_cargo.py
--rw-r--r--   0        0        0    11322 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/version/commands/test_cmake.py
--rw-r--r--   0        0        0    10400 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/version/commands/test_go.py
--rw-r--r--   0        0        0    11635 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/version/commands/test_java.py
--rw-r--r--   0        0        0    17081 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/version/commands/test_javascript.py
--rw-r--r--   0        0        0    16677 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/version/commands/test_python.py
--rw-r--r--   0        0        0      727 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/version/schemes/__init__.py
--rw-r--r--   0        0        0    26655 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/version/schemes/test_pep440.py
--rw-r--r--   0        0        0    28629 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/version/schemes/test_semantic.py
--rw-r--r--   0        0        0      919 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/version/test_commands.py
--rw-r--r--   0        0        0     1096 2023-07-19 14:09:56.572590 pontos-23.7.7/tests/version/test_errors.py
--rw-r--r--   0        0        0     7621 2023-07-19 14:09:56.576590 pontos-23.7.7/tests/version/test_helper.py
--rw-r--r--   0        0        0    10908 2023-07-19 14:09:56.576590 pontos-23.7.7/tests/version/test_main.py
--rw-r--r--   0        0        0     1131 2023-07-19 14:09:56.576590 pontos-23.7.7/tests/version/test_parser.py
--rw-r--r--   0        0        0     6187 2023-07-19 14:09:56.576590 pontos-23.7.7/tests/version/test_project.py
--rw-r--r--   0        0        0     1791 2023-07-19 14:09:56.576590 pontos-23.7.7/tests/version/test_version.py
--rw-r--r--   0        0        0     5157 1970-01-01 00:00:00.000000 pontos-23.7.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-08 11:21:59.817229 pontos-23.8.0/LICENSE
+-rw-r--r--   0        0        0     3836 2023-08-08 11:21:59.817229 pontos-23.8.0/README.md
+-rw-r--r--   0        0        0    98947 2023-08-08 11:21:59.817229 pontos-23.8.0/poetry.lock
+-rw-r--r--   0        0        0      791 2023-08-08 11:21:59.817229 pontos-23.8.0/pontos/__init__.py
+-rw-r--r--   0        0        0     1007 2023-08-08 11:21:59.817229 pontos-23.8.0/pontos/changelog/__init__.py
+-rw-r--r--   0        0        0    12175 2023-08-08 11:21:59.817229 pontos-23.8.0/pontos/changelog/conventional_commits.py
+-rw-r--r--   0        0        0      965 2023-08-08 11:21:59.817229 pontos-23.8.0/pontos/changelog/errors.py
+-rw-r--r--   0        0        0     4434 2023-08-08 11:21:59.817229 pontos-23.8.0/pontos/changelog/main.py
+-rw-r--r--   0        0        0      806 2023-08-08 11:21:59.817229 pontos-23.8.0/pontos/errors.py
+-rw-r--r--   0        0        0      882 2023-08-08 11:21:59.817229 pontos-23.8.0/pontos/git/__init__.py
+-rw-r--r--   0        0        0    18430 2023-08-08 11:21:59.817229 pontos-23.8.0/pontos/git/git.py
+-rw-r--r--   0        0        0     2538 2023-08-08 11:21:59.817229 pontos-23.8.0/pontos/git/status.py
+-rw-r--r--   0        0        0      760 2023-08-08 11:21:59.817229 pontos-23.8.0/pontos/github/__init__.py
+-rw-r--r--   0        0        0     1166 2023-08-08 11:21:59.817229 pontos-23.8.0/pontos/github/actions/__init__.py
+-rw-r--r--   0        0        0     2239 2023-08-08 11:21:59.817229 pontos-23.8.0/pontos/github/actions/argparser.py
+-rw-r--r--   0        0        0     1472 2023-08-08 11:21:59.817229 pontos-23.8.0/pontos/github/actions/cmds.py
+-rw-r--r--   0        0        0     7390 2023-08-08 11:21:59.817229 pontos-23.8.0/pontos/github/actions/core.py
+-rw-r--r--   0        0        0     2426 2023-08-08 11:21:59.817229 pontos-23.8.0/pontos/github/actions/env.py
+-rw-r--r--   0        0        0      861 2023-08-08 11:21:59.817229 pontos-23.8.0/pontos/github/actions/errors.py
+-rw-r--r--   0        0        0     4186 2023-08-08 11:21:59.817229 pontos-23.8.0/pontos/github/actions/event.py
+-rw-r--r--   0        0        0     1100 2023-08-08 11:21:59.817229 pontos-23.8.0/pontos/github/actions/main.py
+-rw-r--r--   0        0        0     2047 2023-08-08 11:21:59.817229 pontos-23.8.0/pontos/github/api/__init__.py
+-rw-r--r--   0        0        0     5531 2023-08-08 11:21:59.817229 pontos-23.8.0/pontos/github/api/api.py
+-rw-r--r--   0        0        0     6210 2023-08-08 11:21:59.817229 pontos-23.8.0/pontos/github/api/artifacts.py
+-rw-r--r--   0        0        0    34561 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/api/branch.py
+-rw-r--r--   0        0        0     9395 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/api/client.py
+-rw-r--r--   0        0        0     1844 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/api/contents.py
+-rw-r--r--   0        0        0      845 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/api/errors.py
+-rw-r--r--   0        0        0     1320 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/api/helper.py
+-rw-r--r--   0        0        0     2813 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/api/labels.py
+-rw-r--r--   0        0        0    10311 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/api/organizations.py
+-rw-r--r--   0        0        0    13090 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/api/pull_requests.py
+-rw-r--r--   0        0        0    12280 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/api/release.py
+-rw-r--r--   0        0        0    21563 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/api/repositories.py
+-rw-r--r--   0        0        0     3276 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/api/search.py
+-rw-r--r--   0        0        0     6004 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/api/tags.py
+-rw-r--r--   0        0        0    15235 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/api/teams.py
+-rw-r--r--   0        0        0     9182 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/api/workflows.py
+-rw-r--r--   0        0        0    11128 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/argparser.py
+-rw-r--r--   0        0        0     8863 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/cmds.py
+-rw-r--r--   0        0        0     1347 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/main.py
+-rw-r--r--   0        0        0     1134 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/models/__init__.py
+-rw-r--r--   0        0        0     2336 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/models/artifact.py
+-rw-r--r--   0        0        0     7532 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/models/base.py
+-rw-r--r--   0        0        0     6915 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/models/branch.py
+-rw-r--r--   0        0        0    16573 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/models/organization.py
+-rw-r--r--   0        0        0    14248 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/models/pull_request.py
+-rw-r--r--   0        0        0     4607 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/models/release.py
+-rw-r--r--   0        0        0     4299 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/models/search.py
+-rw-r--r--   0        0        0     4606 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/models/tag.py
+-rw-r--r--   0        0        0    11477 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/models/workflow.py
+-rw-r--r--   0        0        0      790 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/pr_template.md
+-rw-r--r--   0        0        0     3443 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/script/__init__.py
+-rw-r--r--   0        0        0      835 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/script/errors.py
+-rw-r--r--   0        0        0     5403 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/script/load.py
+-rw-r--r--   0        0        0     1495 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/script/parser.py
+-rw-r--r--   0        0        0        0 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/scripts/__init__.py
+-rw-r--r--   0        0        0     1886 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/scripts/artifacts-download.py
+-rw-r--r--   0        0        0     1514 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/scripts/artifacts-sum.py
+-rw-r--r--   0        0        0     1862 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/scripts/artifacts.py
+-rw-r--r--   0        0        0     1643 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/scripts/branchprotection.py
+-rw-r--r--   0        0        0     5765 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/scripts/create-repository.py
+-rw-r--r--   0        0        0     2212 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/scripts/enforce-admins.py
+-rw-r--r--   0        0        0     1834 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/scripts/lock-branch.py
+-rw-r--r--   0        0        0     2577 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/scripts/members.py
+-rw-r--r--   0        0        0     2193 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/scripts/release-assets-download.py
+-rw-r--r--   0        0        0     2294 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/scripts/repositories.py
+-rw-r--r--   0        0        0     6766 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/scripts/search-repositories.py
+-rw-r--r--   0        0        0     3672 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/scripts/team-repositories.py
+-rw-r--r--   0        0        0     1654 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/scripts/teams.py
+-rw-r--r--   0        0        0     2810 2023-08-08 11:21:59.821229 pontos-23.8.0/pontos/github/scripts/workflow-runs.py
+-rw-r--r--   0        0        0    14844 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/helper.py
+-rw-r--r--   0        0        0     6132 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/models/__init__.py
+-rw-r--r--   0        0        0      864 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/nvd/__init__.py
+-rw-r--r--   0        0        0     4732 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/nvd/api.py
+-rw-r--r--   0        0        0     2177 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/nvd/cpe/__init__.py
+-rw-r--r--   0        0        0     7339 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/nvd/cpe/api.py
+-rw-r--r--   0        0        0     2651 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/nvd/cve/__init__.py
+-rw-r--r--   0        0        0    11470 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/nvd/cve/api.py
+-rw-r--r--   0        0        0      716 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/nvd/models/__init__.py
+-rw-r--r--   0        0        0     2973 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/nvd/models/cpe.py
+-rw-r--r--   0        0        0     7250 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/nvd/models/cve.py
+-rw-r--r--   0        0        0     3254 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/nvd/models/cvss_v2.py
+-rw-r--r--   0        0        0     4471 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/nvd/models/cvss_v3.py
+-rw-r--r--   0        0        0     3561 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/pontos.py
+-rw-r--r--   0        0        0        0 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/py.typed
+-rw-r--r--   0        0        0     1199 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/release/__init__.py
+-rw-r--r--   0        0        0     1775 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/release/command.py
+-rw-r--r--   0        0        0    13646 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/release/create.py
+-rw-r--r--   0        0        0     4516 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/release/helper.py
+-rw-r--r--   0        0        0     2326 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/release/main.py
+-rw-r--r--   0        0        0    10391 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/release/parser.py
+-rw-r--r--   0        0        0     6564 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/release/show.py
+-rw-r--r--   0        0        0    13061 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/release/sign.py
+-rw-r--r--   0        0        0      886 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/terminal/__init__.py
+-rw-r--r--   0        0        0     1770 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/terminal/null.py
+-rw-r--r--   0        0        0     5331 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/terminal/rich.py
+-rw-r--r--   0        0        0     9416 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/terminal/terminal.py
+-rw-r--r--   0        0        0     7231 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/testing/__init__.py
+-rw-r--r--   0        0        0      971 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/typing/__init__.py
+-rw-r--r--   0        0        0      773 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/__init__.py
+-rw-r--r--   0        0        0      838 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/__main__.py
+-rw-r--r--   0        0        0      102 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash
+-rw-r--r--   0        0        0       97 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.c
+-rw-r--r--   0        0        0       90 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake
+-rw-r--r--   0        0        0       93 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.go
+-rw-r--r--   0        0        0       97 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.h
+-rw-r--r--   0        0        0       97 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.js
+-rw-r--r--   0        0        0      224 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl
+-rw-r--r--   0        0        0       90 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.po
+-rw-r--r--   0        0        0       90 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.py
+-rw-r--r--   0        0        0      100 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh
+-rw-r--r--   0        0        0       85 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt
+-rw-r--r--   0        0        0      117 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml
+-rw-r--r--   0        0        0      117 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl
+-rw-r--r--   0        0        0       92 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/GPL-2.0-only/template.c
+-rw-r--r--   0        0        0       92 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/GPL-2.0-only/template.h
+-rw-r--r--   0        0        0      219 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/GPL-2.0-only/template.nasl
+-rw-r--r--   0        0        0      101 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/GPL-2.0-or-later/template.bash
+-rw-r--r--   0        0        0       96 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/GPL-2.0-or-later/template.c
+-rw-r--r--   0        0        0       89 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake
+-rw-r--r--   0        0        0       96 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/GPL-2.0-or-later/template.h
+-rw-r--r--   0        0        0       96 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/GPL-2.0-or-later/template.js
+-rw-r--r--   0        0        0      223 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/GPL-2.0-or-later/template.nasl
+-rw-r--r--   0        0        0       89 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/GPL-2.0-or-later/template.po
+-rw-r--r--   0        0        0       89 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/GPL-2.0-or-later/template.py
+-rw-r--r--   0        0        0       99 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/GPL-2.0-or-later/template.sh
+-rw-r--r--   0        0        0       84 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/GPL-2.0-or-later/template.txt
+-rw-r--r--   0        0        0      116 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/GPL-2.0-or-later/template.xml
+-rw-r--r--   0        0        0      116 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/GPL-2.0-or-later/template.xsl
+-rw-r--r--   0        0        0      101 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/GPL-3.0-or-later/template.bash
+-rw-r--r--   0        0        0       96 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/GPL-3.0-or-later/template.c
+-rw-r--r--   0        0        0       89 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/GPL-3.0-or-later/template.cmake
+-rw-r--r--   0        0        0       92 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/GPL-3.0-or-later/template.go
+-rw-r--r--   0        0        0       96 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/GPL-3.0-or-later/template.h
+-rw-r--r--   0        0        0       96 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/GPL-3.0-or-later/template.js
+-rw-r--r--   0        0        0      223 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/GPL-3.0-or-later/template.nasl
+-rw-r--r--   0        0        0       89 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/GPL-3.0-or-later/template.po
+-rw-r--r--   0        0        0       89 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/GPL-3.0-or-later/template.py
+-rw-r--r--   0        0        0       99 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/GPL-3.0-or-later/template.sh
+-rw-r--r--   0        0        0       84 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/GPL-3.0-or-later/template.txt
+-rw-r--r--   0        0        0      116 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/GPL-3.0-or-later/template.xml
+-rw-r--r--   0        0        0      116 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/templates/GPL-3.0-or-later/template.xsl
+-rw-r--r--   0        0        0    12149 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/updateheader/updateheader.py
+-rw-r--r--   0        0        0     1079 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/version/__init__.py
+-rw-r--r--   0        0        0      816 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/version/__main__.py
+-rw-r--r--   0        0        0      103 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/version/__version__.py
+-rw-r--r--   0        0        0     8837 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/version/_calculator.py
+-rw-r--r--   0        0        0     1624 2023-08-08 11:21:59.825230 pontos-23.8.0/pontos/version/commands/__init__.py
+-rw-r--r--   0        0        0     2940 2023-08-08 11:21:59.829229 pontos-23.8.0/pontos/version/commands/_cargo.py
+-rw-r--r--   0        0        0     7908 2023-08-08 11:21:59.829229 pontos-23.8.0/pontos/version/commands/_cmake.py
+-rw-r--r--   0        0        0     2553 2023-08-08 11:21:59.829229 pontos-23.8.0/pontos/version/commands/_command.py
+-rw-r--r--   0        0        0     3816 2023-08-08 11:21:59.829229 pontos-23.8.0/pontos/version/commands/_go.py
+-rw-r--r--   0        0        0     6774 2023-08-08 11:21:59.829229 pontos-23.8.0/pontos/version/commands/_java.py
+-rw-r--r--   0        0        0     6512 2023-08-08 11:21:59.829229 pontos-23.8.0/pontos/version/commands/_javascript.py
+-rw-r--r--   0        0        0     8688 2023-08-08 11:21:59.829229 pontos-23.8.0/pontos/version/commands/_python.py
+-rw-r--r--   0        0        0      961 2023-08-08 11:21:59.829229 pontos-23.8.0/pontos/version/errors.py
+-rw-r--r--   0        0        0     2812 2023-08-08 11:21:59.829229 pontos-23.8.0/pontos/version/helper.py
+-rw-r--r--   0        0        0     3655 2023-08-08 11:21:59.829229 pontos-23.8.0/pontos/version/main.py
+-rw-r--r--   0        0        0     4163 2023-08-08 11:21:59.829229 pontos-23.8.0/pontos/version/parser.py
+-rw-r--r--   0        0        0     3750 2023-08-08 11:21:59.829229 pontos-23.8.0/pontos/version/project.py
+-rw-r--r--   0        0        0     2204 2023-08-08 11:21:59.829229 pontos-23.8.0/pontos/version/schemes/__init__.py
+-rw-r--r--   0        0        0    14082 2023-08-08 11:21:59.829229 pontos-23.8.0/pontos/version/schemes/_pep440.py
+-rw-r--r--   0        0        0     2159 2023-08-08 11:21:59.829229 pontos-23.8.0/pontos/version/schemes/_scheme.py
+-rw-r--r--   0        0        0    16992 2023-08-08 11:21:59.829229 pontos-23.8.0/pontos/version/schemes/_semantic.py
+-rw-r--r--   0        0        0     5604 2023-08-08 11:21:59.829229 pontos-23.8.0/pontos/version/version.py
+-rw-r--r--   0        0        0     3088 2023-08-08 11:21:59.829229 pontos-23.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1518 2023-08-08 11:21:59.829229 pontos-23.8.0/tests/__init__.py
+-rw-r--r--   0        0        0     1031 2023-08-08 11:21:59.829229 pontos-23.8.0/tests/changelog/__init__.py
+-rw-r--r--   0        0        0      375 2023-08-08 11:21:59.829229 pontos-23.8.0/tests/changelog/changelog.toml
+-rw-r--r--   0        0        0    19105 2023-08-08 11:21:59.829229 pontos-23.8.0/tests/changelog/test_conventional_commits.py
+-rw-r--r--   0        0        0     1925 2023-08-08 11:21:59.829229 pontos-23.8.0/tests/changelog/test_parser.py
+-rw-r--r--   0        0        0       69 2023-08-08 11:21:59.829229 pontos-23.8.0/tests/fake_pyproject.toml
+-rw-r--r--   0        0        0      716 2023-08-08 11:21:59.829229 pontos-23.8.0/tests/git/__init__.py
+-rw-r--r--   0        0        0    32808 2023-08-08 11:21:59.829229 pontos-23.8.0/tests/git/test_git.py
+-rw-r--r--   0        0        0     4215 2023-08-08 11:21:59.829229 pontos-23.8.0/tests/git/test_status.py
+-rw-r--r--   0        0        0      716 2023-08-08 11:21:59.829229 pontos-23.8.0/tests/github/__init__.py
+-rw-r--r--   0        0        0      716 2023-08-08 11:21:59.829229 pontos-23.8.0/tests/github/actions/__init__.py
+-rw-r--r--   0        0        0    29628 2023-08-08 11:21:59.829229 pontos-23.8.0/tests/github/actions/test-pull-request-event.json
+-rw-r--r--   0        0        0     5469 2023-08-08 11:21:59.829229 pontos-23.8.0/tests/github/actions/test_core.py
+-rw-r--r--   0        0        0     3534 2023-08-08 11:21:59.829229 pontos-23.8.0/tests/github/actions/test_env.py
+-rw-r--r--   0        0        0     2086 2023-08-08 11:21:59.829229 pontos-23.8.0/tests/github/actions/test_event.py
+-rw-r--r--   0        0        0     1232 2023-08-08 11:21:59.829229 pontos-23.8.0/tests/github/api/__init__.py
+-rw-r--r--   0        0        0    20021 2023-08-08 11:21:59.829229 pontos-23.8.0/tests/github/api/pr-files.json
+-rw-r--r--   0        0        0     5624 2023-08-08 11:21:59.829229 pontos-23.8.0/tests/github/api/release-response.json
+-rw-r--r--   0        0        0    12076 2023-08-08 11:21:59.829229 pontos-23.8.0/tests/github/api/test_artifacts.py
+-rw-r--r--   0        0        0    20096 2023-08-08 11:21:59.829229 pontos-23.8.0/tests/github/api/test_branch.py
+-rw-r--r--   0        0        0     9619 2023-08-08 11:21:59.829229 pontos-23.8.0/tests/github/api/test_client.py
+-rw-r--r--   0        0        0     2087 2023-08-08 11:21:59.829229 pontos-23.8.0/tests/github/api/test_contents.py
+-rw-r--r--   0        0        0     2801 2023-08-08 11:21:59.829229 pontos-23.8.0/tests/github/api/test_labels.py
+-rw-r--r--   0        0        0    71096 2023-08-08 11:21:59.829229 pontos-23.8.0/tests/github/api/test_organizations.py
+-rw-r--r--   0        0        0    58547 2023-08-08 11:21:59.829229 pontos-23.8.0/tests/github/api/test_pull_requests.py
+-rw-r--r--   0        0        0    17842 2023-08-08 11:21:59.829229 pontos-23.8.0/tests/github/api/test_release.py
+-rw-r--r--   0        0        0    37847 2023-08-08 11:21:59.829229 pontos-23.8.0/tests/github/api/test_repositories.py
+-rw-r--r--   0        0        0    24490 2023-08-08 11:21:59.829229 pontos-23.8.0/tests/github/api/test_search.py
+-rw-r--r--   0        0        0     9490 2023-08-08 11:21:59.829229 pontos-23.8.0/tests/github/api/test_tags.py
+-rw-r--r--   0        0        0    39045 2023-08-08 11:21:59.829229 pontos-23.8.0/tests/github/api/test_teams.py
+-rw-r--r--   0        0        0   129346 2023-08-08 11:21:59.829229 pontos-23.8.0/tests/github/api/test_workflows.py
+-rw-r--r--   0        0        0      716 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/github/models/__init__.py
+-rw-r--r--   0        0        0     3210 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/github/models/test_artifact.py
+-rw-r--r--   0        0        0     9831 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/github/models/test_base.py
+-rw-r--r--   0        0        0    31873 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/github/models/test_branch.py
+-rw-r--r--   0        0        0    19893 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/github/models/test_organization.py
+-rw-r--r--   0        0        0    80894 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/github/models/test_pull_request.py
+-rw-r--r--   0        0        0    12062 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/github/models/test_release.py
+-rw-r--r--   0        0        0     2216 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/github/models/test_search.py
+-rw-r--r--   0        0        0     3419 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/github/models/test_tag.py
+-rw-r--r--   0        0        0    41463 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/github/models/test_workflow.py
+-rw-r--r--   0        0        0      716 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/github/script/__init__.py
+-rw-r--r--   0        0        0     3863 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/github/script/test_load.py
+-rw-r--r--   0        0        0     2052 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/github/script/test_parser.py
+-rw-r--r--   0        0        0     6371 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/github/test_argparser.py
+-rw-r--r--   0        0        0     9562 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/github/test_cmds.py
+-rw-r--r--   0        0        0      716 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/models/__init__.py
+-rw-r--r--   0        0        0     6424 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/models/test_models.py
+-rw-r--r--   0        0        0     2505 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/nvd/__init__.py
+-rw-r--r--   0        0        0      716 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/nvd/cpe/__init__.py
+-rw-r--r--   0        0        0    11290 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/nvd/cpe/test_api.py
+-rw-r--r--   0        0        0      716 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/nvd/cve/__init__.py
+-rw-r--r--   0        0        0    26602 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/nvd/cve/test_api.py
+-rw-r--r--   0        0        0      716 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/nvd/models/__init__.py
+-rw-r--r--   0        0        0     3725 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/nvd/models/test_cpe.py
+-rw-r--r--   0        0        0    25930 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/nvd/models/test_cve.py
+-rw-r--r--   0        0        0     3994 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/nvd/test_api.py
+-rw-r--r--   0        0        0      721 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/release/__init__.py
+-rw-r--r--   0        0        0    85665 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/release/test_create.py
+-rw-r--r--   0        0        0    10884 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/release/test_helper.py
+-rw-r--r--   0        0        0    13303 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/release/test_parser.py
+-rw-r--r--   0        0        0    11964 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/release/test_show.py
+-rw-r--r--   0        0        0    25810 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/release/test_sign.py
+-rw-r--r--   0        0        0      345 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/release/v1.2.3.md
+-rw-r--r--   0        0        0      745 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/terminal/__init__.py
+-rw-r--r--   0        0        0     6653 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/terminal/test_terminal.py
+-rw-r--r--   0        0        0      716 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/test-typing/__init__.py
+-rw-r--r--   0        0        0     1120 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/test-typing/test_typing.py
+-rw-r--r--   0        0        0    20488 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/test_helper.py
+-rw-r--r--   0        0        0     1685 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/test_pontos.py
+-rw-r--r--   0        0        0      716 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/testing/__init__.py
+-rw-r--r--   0        0        0     8007 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/testing/test_testing.py
+-rw-r--r--   0        0        0      721 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/updateheader/__init__.py
+-rw-r--r--   0        0        0    15848 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/updateheader/test_header.py
+-rw-r--r--   0        0        0     1031 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/version/__init__.py
+-rw-r--r--   0        0        0      727 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/version/commands/__init__.py
+-rw-r--r--   0        0        0     3847 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/version/commands/test_cargo.py
+-rw-r--r--   0        0        0    11322 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/version/commands/test_cmake.py
+-rw-r--r--   0        0        0    10400 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/version/commands/test_go.py
+-rw-r--r--   0        0        0    12511 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/version/commands/test_java.py
+-rw-r--r--   0        0        0    17081 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/version/commands/test_javascript.py
+-rw-r--r--   0        0        0    16677 2023-08-08 11:21:59.833230 pontos-23.8.0/tests/version/commands/test_python.py
+-rw-r--r--   0        0        0      727 2023-08-08 11:21:59.837230 pontos-23.8.0/tests/version/schemes/__init__.py
+-rw-r--r--   0        0        0    26655 2023-08-08 11:21:59.837230 pontos-23.8.0/tests/version/schemes/test_pep440.py
+-rw-r--r--   0        0        0    28629 2023-08-08 11:21:59.837230 pontos-23.8.0/tests/version/schemes/test_semantic.py
+-rw-r--r--   0        0        0      919 2023-08-08 11:21:59.837230 pontos-23.8.0/tests/version/test_commands.py
+-rw-r--r--   0        0        0     1096 2023-08-08 11:21:59.837230 pontos-23.8.0/tests/version/test_errors.py
+-rw-r--r--   0        0        0     7621 2023-08-08 11:21:59.837230 pontos-23.8.0/tests/version/test_helper.py
+-rw-r--r--   0        0        0    10908 2023-08-08 11:21:59.837230 pontos-23.8.0/tests/version/test_main.py
+-rw-r--r--   0        0        0     1131 2023-08-08 11:21:59.837230 pontos-23.8.0/tests/version/test_parser.py
+-rw-r--r--   0        0        0     6187 2023-08-08 11:21:59.837230 pontos-23.8.0/tests/version/test_project.py
+-rw-r--r--   0        0        0     1791 2023-08-08 11:21:59.837230 pontos-23.8.0/tests/version/test_version.py
+-rw-r--r--   0        0        0     5081 1970-01-01 00:00:00.000000 pontos-23.8.0/PKG-INFO
```

### Comparing `pontos-23.7.7/LICENSE` & `pontos-23.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/README.md` & `pontos-23.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/poetry.lock` & `pontos-23.8.0/poetry.lock`

 * *Files 3% similar despite different names*

```diff
@@ -9,58 +9,58 @@
 files = [
     {file = "alabaster-0.7.13-py3-none-any.whl", hash = "sha256:1ee19aca801bbabb5ba3f5f258e4422dfa86f82f3e9cefb0859b283cdd7f62a3"},
     {file = "alabaster-0.7.13.tar.gz", hash = "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"},
 ]
 
 [[package]]
 name = "anyio"
-version = "3.7.0"
+version = "3.7.1"
 description = "High level compatibility layer for multiple asynchronous event loop implementations"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "anyio-3.7.0-py3-none-any.whl", hash = "sha256:eddca883c4175f14df8aedce21054bfca3adb70ffe76a9f607aef9d7fa2ea7f0"},
-    {file = "anyio-3.7.0.tar.gz", hash = "sha256:275d9973793619a5374e1c89a4f4ad3f4b0a5510a2b5b939444bee8f4c4d37ce"},
+    {file = "anyio-3.7.1-py3-none-any.whl", hash = "sha256:91dee416e570e92c64041bd18b900d1d6fa78dff7048769ce5ac5ddad004fbb5"},
+    {file = "anyio-3.7.1.tar.gz", hash = "sha256:44a3c9aba0f5defa43261a8b3efb97891f2bd7d804e0e1f56419befa1adfc780"},
 ]
 
 [package.dependencies]
 exceptiongroup = {version = "*", markers = "python_version < \"3.11\""}
 idna = ">=2.8"
 sniffio = ">=1.1"
 
 [package.extras]
-doc = ["Sphinx (>=6.1.0)", "packaging", "sphinx-autodoc-typehints (>=1.2.0)", "sphinx-rtd-theme", "sphinxcontrib-jquery"]
+doc = ["Sphinx", "packaging", "sphinx-autodoc-typehints (>=1.2.0)", "sphinx-rtd-theme (>=1.2.2)", "sphinxcontrib-jquery"]
 test = ["anyio[trio]", "coverage[toml] (>=4.5)", "hypothesis (>=4.0)", "mock (>=4)", "psutil (>=5.9)", "pytest (>=7.0)", "pytest-mock (>=3.6.1)", "trustme", "uvloop (>=0.17)"]
 trio = ["trio (<0.22)"]
 
 [[package]]
 name = "autohooks"
-version = "23.4.0"
+version = "23.7.0"
 description = "Library for managing git hooks"
 optional = false
-python-versions = ">=3.7.2,<4.0.0"
+python-versions = ">=3.8,<4.0"
 files = [
-    {file = "autohooks-23.4.0-py3-none-any.whl", hash = "sha256:2c3b8506890565ad8c9b690db9b70a9b65068ff9f1c2a2d601d2914ad576cfff"},
-    {file = "autohooks-23.4.0.tar.gz", hash = "sha256:6880ad263f0aaab607bbfc1d42afc407de6234320fcff10d75d4e89f4e711ccd"},
+    {file = "autohooks-23.7.0-py3-none-any.whl", hash = "sha256:1fa417891efc3681bdf109cb2e99688948d1f3587d91dab17f1ed9b4428590a4"},
+    {file = "autohooks-23.7.0.tar.gz", hash = "sha256:cf486581fc111122fc3ea394b60a26bc4da0844cf916b6e4fadf90ff97633fe5"},
 ]
 
 [package.dependencies]
 pontos = ">=22.8.0"
 rich = ">=12.5.1"
 tomlkit = ">=0.5.11"
 
 [[package]]
 name = "autohooks-plugin-black"
-version = "23.4.0"
+version = "23.7.0"
 description = "An autohooks plugin for python code formatting via black"
 optional = false
-python-versions = ">=3.7.2,<4.0.0"
+python-versions = ">=3.8,<4.0"
 files = [
-    {file = "autohooks_plugin_black-23.4.0-py3-none-any.whl", hash = "sha256:1a65814ab573a40799cf52af7aa026e73ef60d784cf14a8eba33aaf245811899"},
-    {file = "autohooks_plugin_black-23.4.0.tar.gz", hash = "sha256:31b0497f8987def02d5387b9eb03c46837621097c9814d19ff6b9da960867a06"},
+    {file = "autohooks_plugin_black-23.7.0-py3-none-any.whl", hash = "sha256:7ce7c25de7da08adf6293b5afa412f4331fc024ff4d872b9daa3247d280eda03"},
+    {file = "autohooks_plugin_black-23.7.0.tar.gz", hash = "sha256:ae2dbda4f8598f8265ef74bcbcf7f14b07d97575368ec8ae03e0fbda32d783dd"},
 ]
 
 [package.dependencies]
 autohooks = ">=21.6.0"
 black = ">=20.8"
 
 [[package]]
@@ -75,14 +75,29 @@
 ]
 
 [package.dependencies]
 autohooks = ">=21.6.0"
 isort = ">=5.8.0,<6.0.0"
 
 [[package]]
+name = "autohooks-plugin-mypy"
+version = "23.3.0"
+description = "An autohooks plugin for python code static typing check with mypy"
+optional = false
+python-versions = ">=3.7.2,<4.0.0"
+files = [
+    {file = "autohooks_plugin_mypy-23.3.0-py3-none-any.whl", hash = "sha256:3cd38cf53c2307ff396beb448d098f6631c3af74ab289bb45fc4f0f53f72a18b"},
+    {file = "autohooks_plugin_mypy-23.3.0.tar.gz", hash = "sha256:eb768b1114c1cb54c8cbfe7f520641b70001d3c90ea9337067ce42567ec44f88"},
+]
+
+[package.dependencies]
+autohooks = ">=21.7.0"
+mypy = ">=0.910"
+
+[[package]]
 name = "autohooks-plugin-ruff"
 version = "23.6.1"
 description = "An autohooks plugin for python code formatting via ruff"
 optional = false
 python-versions = ">=3.7.2,<4.0.0"
 files = [
     {file = "autohooks_plugin_ruff-23.6.1-py3-none-any.whl", hash = "sha256:8afad5fe0d70eadc805e0c2b7b35e50e3e2d21ec45549a1fba721792cff6e28c"},
@@ -120,44 +135,41 @@
 
 [package.extras]
 html5lib = ["html5lib"]
 lxml = ["lxml"]
 
 [[package]]
 name = "black"
-version = "23.3.0"
+version = "23.7.0"
 description = "The uncompromising code formatter."
 optional = false
-python-versions = ">=3.7"
+python-versions = ">=3.8"
 files = [
-    {file = "black-23.3.0-cp310-cp310-macosx_10_16_arm64.whl", hash = "sha256:0945e13506be58bf7db93ee5853243eb368ace1c08a24c65ce108986eac65915"},
-    {file = "black-23.3.0-cp310-cp310-macosx_10_16_universal2.whl", hash = "sha256:67de8d0c209eb5b330cce2469503de11bca4085880d62f1628bd9972cc3366b9"},
-    {file = "black-23.3.0-cp310-cp310-macosx_10_16_x86_64.whl", hash = "sha256:7c3eb7cea23904399866c55826b31c1f55bbcd3890ce22ff70466b907b6775c2"},
-    {file = "black-23.3.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:32daa9783106c28815d05b724238e30718f34155653d4d6e125dc7daec8e260c"},
-    {file = "black-23.3.0-cp310-cp310-win_amd64.whl", hash = "sha256:35d1381d7a22cc5b2be2f72c7dfdae4072a3336060635718cc7e1ede24221d6c"},
-    {file = "black-23.3.0-cp311-cp311-macosx_10_16_arm64.whl", hash = "sha256:a8a968125d0a6a404842fa1bf0b349a568634f856aa08ffaff40ae0dfa52e7c6"},
-    {file = "black-23.3.0-cp311-cp311-macosx_10_16_universal2.whl", hash = "sha256:c7ab5790333c448903c4b721b59c0d80b11fe5e9803d8703e84dcb8da56fec1b"},
-    {file = "black-23.3.0-cp311-cp311-macosx_10_16_x86_64.whl", hash = "sha256:a6f6886c9869d4daae2d1715ce34a19bbc4b95006d20ed785ca00fa03cba312d"},
-    {file = "black-23.3.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6f3c333ea1dd6771b2d3777482429864f8e258899f6ff05826c3a4fcc5ce3f70"},
-    {file = "black-23.3.0-cp311-cp311-win_amd64.whl", hash = "sha256:11c410f71b876f961d1de77b9699ad19f939094c3a677323f43d7a29855fe326"},
-    {file = "black-23.3.0-cp37-cp37m-macosx_10_16_x86_64.whl", hash = "sha256:1d06691f1eb8de91cd1b322f21e3bfc9efe0c7ca1f0e1eb1db44ea367dff656b"},
-    {file = "black-23.3.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:50cb33cac881766a5cd9913e10ff75b1e8eb71babf4c7104f2e9c52da1fb7de2"},
-    {file = "black-23.3.0-cp37-cp37m-win_amd64.whl", hash = "sha256:e114420bf26b90d4b9daa597351337762b63039752bdf72bf361364c1aa05925"},
-    {file = "black-23.3.0-cp38-cp38-macosx_10_16_arm64.whl", hash = "sha256:48f9d345675bb7fbc3dd85821b12487e1b9a75242028adad0333ce36ed2a6d27"},
-    {file = "black-23.3.0-cp38-cp38-macosx_10_16_universal2.whl", hash = "sha256:714290490c18fb0126baa0fca0a54ee795f7502b44177e1ce7624ba1c00f2331"},
-    {file = "black-23.3.0-cp38-cp38-macosx_10_16_x86_64.whl", hash = "sha256:064101748afa12ad2291c2b91c960be28b817c0c7eaa35bec09cc63aa56493c5"},
-    {file = "black-23.3.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:562bd3a70495facf56814293149e51aa1be9931567474993c7942ff7d3533961"},
-    {file = "black-23.3.0-cp38-cp38-win_amd64.whl", hash = "sha256:e198cf27888ad6f4ff331ca1c48ffc038848ea9f031a3b40ba36aced7e22f2c8"},
-    {file = "black-23.3.0-cp39-cp39-macosx_10_16_arm64.whl", hash = "sha256:3238f2aacf827d18d26db07524e44741233ae09a584273aa059066d644ca7b30"},
-    {file = "black-23.3.0-cp39-cp39-macosx_10_16_universal2.whl", hash = "sha256:f0bd2f4a58d6666500542b26354978218a9babcdc972722f4bf90779524515f3"},
-    {file = "black-23.3.0-cp39-cp39-macosx_10_16_x86_64.whl", hash = "sha256:92c543f6854c28a3c7f39f4d9b7694f9a6eb9d3c5e2ece488c327b6e7ea9b266"},
-    {file = "black-23.3.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:3a150542a204124ed00683f0db1f5cf1c2aaaa9cc3495b7a3b5976fb136090ab"},
-    {file = "black-23.3.0-cp39-cp39-win_amd64.whl", hash = "sha256:6b39abdfb402002b8a7d030ccc85cf5afff64ee90fa4c5aebc531e3ad0175ddb"},
-    {file = "black-23.3.0-py3-none-any.whl", hash = "sha256:ec751418022185b0c1bb7d7736e6933d40bbb14c14a0abcf9123d1b159f98dd4"},
-    {file = "black-23.3.0.tar.gz", hash = "sha256:1c7b8d606e728a41ea1ccbd7264677e494e87cf630e399262ced92d4a8dac940"},
+    {file = "black-23.7.0-cp310-cp310-macosx_10_16_arm64.whl", hash = "sha256:5c4bc552ab52f6c1c506ccae05681fab58c3f72d59ae6e6639e8885e94fe2587"},
+    {file = "black-23.7.0-cp310-cp310-macosx_10_16_universal2.whl", hash = "sha256:552513d5cd5694590d7ef6f46e1767a4df9af168d449ff767b13b084c020e63f"},
+    {file = "black-23.7.0-cp310-cp310-macosx_10_16_x86_64.whl", hash = "sha256:86cee259349b4448adb4ef9b204bb4467aae74a386bce85d56ba4f5dc0da27be"},
+    {file = "black-23.7.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:501387a9edcb75d7ae8a4412bb8749900386eaef258f1aefab18adddea1936bc"},
+    {file = "black-23.7.0-cp310-cp310-win_amd64.whl", hash = "sha256:fb074d8b213749fa1d077d630db0d5f8cc3b2ae63587ad4116e8a436e9bbe995"},
+    {file = "black-23.7.0-cp311-cp311-macosx_10_16_arm64.whl", hash = "sha256:b5b0ee6d96b345a8b420100b7d71ebfdd19fab5e8301aff48ec270042cd40ac2"},
+    {file = "black-23.7.0-cp311-cp311-macosx_10_16_universal2.whl", hash = "sha256:893695a76b140881531062d48476ebe4a48f5d1e9388177e175d76234ca247cd"},
+    {file = "black-23.7.0-cp311-cp311-macosx_10_16_x86_64.whl", hash = "sha256:c333286dc3ddca6fdff74670b911cccedacb4ef0a60b34e491b8a67c833b343a"},
+    {file = "black-23.7.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:831d8f54c3a8c8cf55f64d0422ee875eecac26f5f649fb6c1df65316b67c8926"},
+    {file = "black-23.7.0-cp311-cp311-win_amd64.whl", hash = "sha256:7f3bf2dec7d541b4619b8ce526bda74a6b0bffc480a163fed32eb8b3c9aed8ad"},
+    {file = "black-23.7.0-cp38-cp38-macosx_10_16_arm64.whl", hash = "sha256:f9062af71c59c004cd519e2fb8f5d25d39e46d3af011b41ab43b9c74e27e236f"},
+    {file = "black-23.7.0-cp38-cp38-macosx_10_16_universal2.whl", hash = "sha256:01ede61aac8c154b55f35301fac3e730baf0c9cf8120f65a9cd61a81cfb4a0c3"},
+    {file = "black-23.7.0-cp38-cp38-macosx_10_16_x86_64.whl", hash = "sha256:327a8c2550ddc573b51e2c352adb88143464bb9d92c10416feb86b0f5aee5ff6"},
+    {file = "black-23.7.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6d1c6022b86f83b632d06f2b02774134def5d4d4f1dac8bef16d90cda18ba28a"},
+    {file = "black-23.7.0-cp38-cp38-win_amd64.whl", hash = "sha256:27eb7a0c71604d5de083757fbdb245b1a4fae60e9596514c6ec497eb63f95320"},
+    {file = "black-23.7.0-cp39-cp39-macosx_10_16_arm64.whl", hash = "sha256:8417dbd2f57b5701492cd46edcecc4f9208dc75529bcf76c514864e48da867d9"},
+    {file = "black-23.7.0-cp39-cp39-macosx_10_16_universal2.whl", hash = "sha256:47e56d83aad53ca140da0af87678fb38e44fd6bc0af71eebab2d1f59b1acf1d3"},
+    {file = "black-23.7.0-cp39-cp39-macosx_10_16_x86_64.whl", hash = "sha256:25cc308838fe71f7065df53aedd20327969d05671bac95b38fdf37ebe70ac087"},
+    {file = "black-23.7.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:642496b675095d423f9b8448243336f8ec71c9d4d57ec17bf795b67f08132a91"},
+    {file = "black-23.7.0-cp39-cp39-win_amd64.whl", hash = "sha256:ad0014efc7acf0bd745792bd0d8857413652979200ab924fbf239062adc12491"},
+    {file = "black-23.7.0-py3-none-any.whl", hash = "sha256:9fd59d418c60c0348505f2ddf9609c1e1de8e7493eab96198fc89d9f865e7a96"},
+    {file = "black-23.7.0.tar.gz", hash = "sha256:022a582720b0d9480ed82576c920a8c1dde97cc38ff11d8d8859b3bd6ca9eedb"},
 ]
 
 [package.dependencies]
 click = ">=8.0.0"
 mypy-extensions = ">=0.4.3"
 packaging = ">=22.0"
 pathspec = ">=0.9.0"
@@ -169,116 +181,116 @@
 colorama = ["colorama (>=0.4.3)"]
 d = ["aiohttp (>=3.7.4)"]
 jupyter = ["ipython (>=7.8.0)", "tokenize-rt (>=3.2.0)"]
 uvloop = ["uvloop (>=0.15.2)"]
 
 [[package]]
 name = "certifi"
-version = "2023.5.7"
+version = "2023.7.22"
 description = "Python package for providing Mozilla's CA Bundle."
 optional = false
 python-versions = ">=3.6"
 files = [
-    {file = "certifi-2023.5.7-py3-none-any.whl", hash = "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"},
-    {file = "certifi-2023.5.7.tar.gz", hash = "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7"},
+    {file = "certifi-2023.7.22-py3-none-any.whl", hash = "sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9"},
+    {file = "certifi-2023.7.22.tar.gz", hash = "sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082"},
 ]
 
 [[package]]
 name = "charset-normalizer"
-version = "3.1.0"
+version = "3.2.0"
 description = "The Real First Universal Charset Detector. Open, modern and actively maintained alternative to Chardet."
 optional = false
 python-versions = ">=3.7.0"
 files = [
-    {file = "charset-normalizer-3.1.0.tar.gz", hash = "sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5"},
-    {file = "charset_normalizer-3.1.0-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b"},
-    {file = "charset_normalizer-3.1.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60"},
-    {file = "charset_normalizer-3.1.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1"},
-    {file = "charset_normalizer-3.1.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0"},
-    {file = "charset_normalizer-3.1.0-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f"},
-    {file = "charset_normalizer-3.1.0-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0"},
-    {file = "charset_normalizer-3.1.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795"},
-    {file = "charset_normalizer-3.1.0-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c"},
-    {file = "charset_normalizer-3.1.0-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203"},
-    {file = "charset_normalizer-3.1.0-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1"},
-    {file = "charset_normalizer-3.1.0-cp310-cp310-musllinux_1_1_ppc64le.whl", hash = "sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137"},
-    {file = "charset_normalizer-3.1.0-cp310-cp310-musllinux_1_1_s390x.whl", hash = "sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce"},
-    {file = "charset_normalizer-3.1.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a"},
-    {file = "charset_normalizer-3.1.0-cp310-cp310-win32.whl", hash = "sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448"},
-    {file = "charset_normalizer-3.1.0-cp310-cp310-win_amd64.whl", hash = "sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8"},
-    {file = "charset_normalizer-3.1.0-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19"},
-    {file = "charset_normalizer-3.1.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017"},
-    {file = "charset_normalizer-3.1.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df"},
-    {file = "charset_normalizer-3.1.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a"},
-    {file = "charset_normalizer-3.1.0-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41"},
-    {file = "charset_normalizer-3.1.0-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1"},
-    {file = "charset_normalizer-3.1.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62"},
-    {file = "charset_normalizer-3.1.0-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6"},
-    {file = "charset_normalizer-3.1.0-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5"},
-    {file = "charset_normalizer-3.1.0-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be"},
-    {file = "charset_normalizer-3.1.0-cp311-cp311-musllinux_1_1_ppc64le.whl", hash = "sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb"},
-    {file = "charset_normalizer-3.1.0-cp311-cp311-musllinux_1_1_s390x.whl", hash = "sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac"},
-    {file = "charset_normalizer-3.1.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324"},
-    {file = "charset_normalizer-3.1.0-cp311-cp311-win32.whl", hash = "sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909"},
-    {file = "charset_normalizer-3.1.0-cp311-cp311-win_amd64.whl", hash = "sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755"},
-    {file = "charset_normalizer-3.1.0-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373"},
-    {file = "charset_normalizer-3.1.0-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"},
-    {file = "charset_normalizer-3.1.0-cp37-cp37m-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9"},
-    {file = "charset_normalizer-3.1.0-cp37-cp37m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f"},
-    {file = "charset_normalizer-3.1.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28"},
-    {file = "charset_normalizer-3.1.0-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d"},
-    {file = "charset_normalizer-3.1.0-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d"},
-    {file = "charset_normalizer-3.1.0-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d"},
-    {file = "charset_normalizer-3.1.0-cp37-cp37m-musllinux_1_1_ppc64le.whl", hash = "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6"},
-    {file = "charset_normalizer-3.1.0-cp37-cp37m-musllinux_1_1_s390x.whl", hash = "sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84"},
-    {file = "charset_normalizer-3.1.0-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c"},
-    {file = "charset_normalizer-3.1.0-cp37-cp37m-win32.whl", hash = "sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974"},
-    {file = "charset_normalizer-3.1.0-cp37-cp37m-win_amd64.whl", hash = "sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23"},
-    {file = "charset_normalizer-3.1.0-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531"},
-    {file = "charset_normalizer-3.1.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c"},
-    {file = "charset_normalizer-3.1.0-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14"},
-    {file = "charset_normalizer-3.1.0-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb"},
-    {file = "charset_normalizer-3.1.0-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1"},
-    {file = "charset_normalizer-3.1.0-cp38-cp38-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b"},
-    {file = "charset_normalizer-3.1.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0"},
-    {file = "charset_normalizer-3.1.0-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649"},
-    {file = "charset_normalizer-3.1.0-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326"},
-    {file = "charset_normalizer-3.1.0-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11"},
-    {file = "charset_normalizer-3.1.0-cp38-cp38-musllinux_1_1_ppc64le.whl", hash = "sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b"},
-    {file = "charset_normalizer-3.1.0-cp38-cp38-musllinux_1_1_s390x.whl", hash = "sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd"},
-    {file = "charset_normalizer-3.1.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8"},
-    {file = "charset_normalizer-3.1.0-cp38-cp38-win32.whl", hash = "sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0"},
-    {file = "charset_normalizer-3.1.0-cp38-cp38-win_amd64.whl", hash = "sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59"},
-    {file = "charset_normalizer-3.1.0-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e"},
-    {file = "charset_normalizer-3.1.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31"},
-    {file = "charset_normalizer-3.1.0-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f"},
-    {file = "charset_normalizer-3.1.0-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e"},
-    {file = "charset_normalizer-3.1.0-cp39-cp39-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f"},
-    {file = "charset_normalizer-3.1.0-cp39-cp39-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854"},
-    {file = "charset_normalizer-3.1.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706"},
-    {file = "charset_normalizer-3.1.0-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e"},
-    {file = "charset_normalizer-3.1.0-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0"},
-    {file = "charset_normalizer-3.1.0-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230"},
-    {file = "charset_normalizer-3.1.0-cp39-cp39-musllinux_1_1_ppc64le.whl", hash = "sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7"},
-    {file = "charset_normalizer-3.1.0-cp39-cp39-musllinux_1_1_s390x.whl", hash = "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e"},
-    {file = "charset_normalizer-3.1.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f"},
-    {file = "charset_normalizer-3.1.0-cp39-cp39-win32.whl", hash = "sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1"},
-    {file = "charset_normalizer-3.1.0-cp39-cp39-win_amd64.whl", hash = "sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b"},
-    {file = "charset_normalizer-3.1.0-py3-none-any.whl", hash = "sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d"},
+    {file = "charset-normalizer-3.2.0.tar.gz", hash = "sha256:3bb3d25a8e6c0aedd251753a79ae98a093c7e7b471faa3aa9a93a81431987ace"},
+    {file = "charset_normalizer-3.2.0-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:0b87549028f680ca955556e3bd57013ab47474c3124dc069faa0b6545b6c9710"},
+    {file = "charset_normalizer-3.2.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:7c70087bfee18a42b4040bb9ec1ca15a08242cf5867c58726530bdf3945672ed"},
+    {file = "charset_normalizer-3.2.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:a103b3a7069b62f5d4890ae1b8f0597618f628b286b03d4bc9195230b154bfa9"},
+    {file = "charset_normalizer-3.2.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:94aea8eff76ee6d1cdacb07dd2123a68283cb5569e0250feab1240058f53b623"},
+    {file = "charset_normalizer-3.2.0-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:db901e2ac34c931d73054d9797383d0f8009991e723dab15109740a63e7f902a"},
+    {file = "charset_normalizer-3.2.0-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:b0dac0ff919ba34d4df1b6131f59ce95b08b9065233446be7e459f95554c0dc8"},
+    {file = "charset_normalizer-3.2.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:193cbc708ea3aca45e7221ae58f0fd63f933753a9bfb498a3b474878f12caaad"},
+    {file = "charset_normalizer-3.2.0-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:09393e1b2a9461950b1c9a45d5fd251dc7c6f228acab64da1c9c0165d9c7765c"},
+    {file = "charset_normalizer-3.2.0-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:baacc6aee0b2ef6f3d308e197b5d7a81c0e70b06beae1f1fcacffdbd124fe0e3"},
+    {file = "charset_normalizer-3.2.0-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:bf420121d4c8dce6b889f0e8e4ec0ca34b7f40186203f06a946fa0276ba54029"},
+    {file = "charset_normalizer-3.2.0-cp310-cp310-musllinux_1_1_ppc64le.whl", hash = "sha256:c04a46716adde8d927adb9457bbe39cf473e1e2c2f5d0a16ceb837e5d841ad4f"},
+    {file = "charset_normalizer-3.2.0-cp310-cp310-musllinux_1_1_s390x.whl", hash = "sha256:aaf63899c94de41fe3cf934601b0f7ccb6b428c6e4eeb80da72c58eab077b19a"},
+    {file = "charset_normalizer-3.2.0-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:d62e51710986674142526ab9f78663ca2b0726066ae26b78b22e0f5e571238dd"},
+    {file = "charset_normalizer-3.2.0-cp310-cp310-win32.whl", hash = "sha256:04e57ab9fbf9607b77f7d057974694b4f6b142da9ed4a199859d9d4d5c63fe96"},
+    {file = "charset_normalizer-3.2.0-cp310-cp310-win_amd64.whl", hash = "sha256:48021783bdf96e3d6de03a6e39a1171ed5bd7e8bb93fc84cc649d11490f87cea"},
+    {file = "charset_normalizer-3.2.0-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:4957669ef390f0e6719db3613ab3a7631e68424604a7b448f079bee145da6e09"},
+    {file = "charset_normalizer-3.2.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:46fb8c61d794b78ec7134a715a3e564aafc8f6b5e338417cb19fe9f57a5a9bf2"},
+    {file = "charset_normalizer-3.2.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:f779d3ad205f108d14e99bb3859aa7dd8e9c68874617c72354d7ecaec2a054ac"},
+    {file = "charset_normalizer-3.2.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:f25c229a6ba38a35ae6e25ca1264621cc25d4d38dca2942a7fce0b67a4efe918"},
+    {file = "charset_normalizer-3.2.0-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:2efb1bd13885392adfda4614c33d3b68dee4921fd0ac1d3988f8cbb7d589e72a"},
+    {file = "charset_normalizer-3.2.0-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:1f30b48dd7fa1474554b0b0f3fdfdd4c13b5c737a3c6284d3cdc424ec0ffff3a"},
+    {file = "charset_normalizer-3.2.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:246de67b99b6851627d945db38147d1b209a899311b1305dd84916f2b88526c6"},
+    {file = "charset_normalizer-3.2.0-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:9bd9b3b31adcb054116447ea22caa61a285d92e94d710aa5ec97992ff5eb7cf3"},
+    {file = "charset_normalizer-3.2.0-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:8c2f5e83493748286002f9369f3e6607c565a6a90425a3a1fef5ae32a36d749d"},
+    {file = "charset_normalizer-3.2.0-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:3170c9399da12c9dc66366e9d14da8bf7147e1e9d9ea566067bbce7bb74bd9c2"},
+    {file = "charset_normalizer-3.2.0-cp311-cp311-musllinux_1_1_ppc64le.whl", hash = "sha256:7a4826ad2bd6b07ca615c74ab91f32f6c96d08f6fcc3902ceeedaec8cdc3bcd6"},
+    {file = "charset_normalizer-3.2.0-cp311-cp311-musllinux_1_1_s390x.whl", hash = "sha256:3b1613dd5aee995ec6d4c69f00378bbd07614702a315a2cf6c1d21461fe17c23"},
+    {file = "charset_normalizer-3.2.0-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:9e608aafdb55eb9f255034709e20d5a83b6d60c054df0802fa9c9883d0a937aa"},
+    {file = "charset_normalizer-3.2.0-cp311-cp311-win32.whl", hash = "sha256:f2a1d0fd4242bd8643ce6f98927cf9c04540af6efa92323e9d3124f57727bfc1"},
+    {file = "charset_normalizer-3.2.0-cp311-cp311-win_amd64.whl", hash = "sha256:681eb3d7e02e3c3655d1b16059fbfb605ac464c834a0c629048a30fad2b27489"},
+    {file = "charset_normalizer-3.2.0-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:c57921cda3a80d0f2b8aec7e25c8aa14479ea92b5b51b6876d975d925a2ea346"},
+    {file = "charset_normalizer-3.2.0-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:41b25eaa7d15909cf3ac4c96088c1f266a9a93ec44f87f1d13d4a0e86c81b982"},
+    {file = "charset_normalizer-3.2.0-cp37-cp37m-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:f058f6963fd82eb143c692cecdc89e075fa0828db2e5b291070485390b2f1c9c"},
+    {file = "charset_normalizer-3.2.0-cp37-cp37m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:a7647ebdfb9682b7bb97e2a5e7cb6ae735b1c25008a70b906aecca294ee96cf4"},
+    {file = "charset_normalizer-3.2.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:eef9df1eefada2c09a5e7a40991b9fc6ac6ef20b1372abd48d2794a316dc0449"},
+    {file = "charset_normalizer-3.2.0-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:e03b8895a6990c9ab2cdcd0f2fe44088ca1c65ae592b8f795c3294af00a461c3"},
+    {file = "charset_normalizer-3.2.0-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:ee4006268ed33370957f55bf2e6f4d263eaf4dc3cfc473d1d90baff6ed36ce4a"},
+    {file = "charset_normalizer-3.2.0-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:c4983bf937209c57240cff65906b18bb35e64ae872da6a0db937d7b4af845dd7"},
+    {file = "charset_normalizer-3.2.0-cp37-cp37m-musllinux_1_1_ppc64le.whl", hash = "sha256:3bb7fda7260735efe66d5107fb7e6af6a7c04c7fce9b2514e04b7a74b06bf5dd"},
+    {file = "charset_normalizer-3.2.0-cp37-cp37m-musllinux_1_1_s390x.whl", hash = "sha256:72814c01533f51d68702802d74f77ea026b5ec52793c791e2da806a3844a46c3"},
+    {file = "charset_normalizer-3.2.0-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:70c610f6cbe4b9fce272c407dd9d07e33e6bf7b4aa1b7ffb6f6ded8e634e3592"},
+    {file = "charset_normalizer-3.2.0-cp37-cp37m-win32.whl", hash = "sha256:a401b4598e5d3f4a9a811f3daf42ee2291790c7f9d74b18d75d6e21dda98a1a1"},
+    {file = "charset_normalizer-3.2.0-cp37-cp37m-win_amd64.whl", hash = "sha256:c0b21078a4b56965e2b12f247467b234734491897e99c1d51cee628da9786959"},
+    {file = "charset_normalizer-3.2.0-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:95eb302ff792e12aba9a8b8f8474ab229a83c103d74a750ec0bd1c1eea32e669"},
+    {file = "charset_normalizer-3.2.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:1a100c6d595a7f316f1b6f01d20815d916e75ff98c27a01ae817439ea7726329"},
+    {file = "charset_normalizer-3.2.0-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:6339d047dab2780cc6220f46306628e04d9750f02f983ddb37439ca47ced7149"},
+    {file = "charset_normalizer-3.2.0-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:e4b749b9cc6ee664a3300bb3a273c1ca8068c46be705b6c31cf5d276f8628a94"},
+    {file = "charset_normalizer-3.2.0-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:a38856a971c602f98472050165cea2cdc97709240373041b69030be15047691f"},
+    {file = "charset_normalizer-3.2.0-cp38-cp38-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:f87f746ee241d30d6ed93969de31e5ffd09a2961a051e60ae6bddde9ec3583aa"},
+    {file = "charset_normalizer-3.2.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:89f1b185a01fe560bc8ae5f619e924407efca2191b56ce749ec84982fc59a32a"},
+    {file = "charset_normalizer-3.2.0-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:e1c8a2f4c69e08e89632defbfabec2feb8a8d99edc9f89ce33c4b9e36ab63037"},
+    {file = "charset_normalizer-3.2.0-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:2f4ac36d8e2b4cc1aa71df3dd84ff8efbe3bfb97ac41242fbcfc053c67434f46"},
+    {file = "charset_normalizer-3.2.0-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:a386ebe437176aab38c041de1260cd3ea459c6ce5263594399880bbc398225b2"},
+    {file = "charset_normalizer-3.2.0-cp38-cp38-musllinux_1_1_ppc64le.whl", hash = "sha256:ccd16eb18a849fd8dcb23e23380e2f0a354e8daa0c984b8a732d9cfaba3a776d"},
+    {file = "charset_normalizer-3.2.0-cp38-cp38-musllinux_1_1_s390x.whl", hash = "sha256:e6a5bf2cba5ae1bb80b154ed68a3cfa2fa00fde979a7f50d6598d3e17d9ac20c"},
+    {file = "charset_normalizer-3.2.0-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:45de3f87179c1823e6d9e32156fb14c1927fcc9aba21433f088fdfb555b77c10"},
+    {file = "charset_normalizer-3.2.0-cp38-cp38-win32.whl", hash = "sha256:1000fba1057b92a65daec275aec30586c3de2401ccdcd41f8a5c1e2c87078706"},
+    {file = "charset_normalizer-3.2.0-cp38-cp38-win_amd64.whl", hash = "sha256:8b2c760cfc7042b27ebdb4a43a4453bd829a5742503599144d54a032c5dc7e9e"},
+    {file = "charset_normalizer-3.2.0-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:855eafa5d5a2034b4621c74925d89c5efef61418570e5ef9b37717d9c796419c"},
+    {file = "charset_normalizer-3.2.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:203f0c8871d5a7987be20c72442488a0b8cfd0f43b7973771640fc593f56321f"},
+    {file = "charset_normalizer-3.2.0-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:e857a2232ba53ae940d3456f7533ce6ca98b81917d47adc3c7fd55dad8fab858"},
+    {file = "charset_normalizer-3.2.0-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5e86d77b090dbddbe78867a0275cb4df08ea195e660f1f7f13435a4649e954e5"},
+    {file = "charset_normalizer-3.2.0-cp39-cp39-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:c4fb39a81950ec280984b3a44f5bd12819953dc5fa3a7e6fa7a80db5ee853952"},
+    {file = "charset_normalizer-3.2.0-cp39-cp39-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:2dee8e57f052ef5353cf608e0b4c871aee320dd1b87d351c28764fc0ca55f9f4"},
+    {file = "charset_normalizer-3.2.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8700f06d0ce6f128de3ccdbc1acaea1ee264d2caa9ca05daaf492fde7c2a7200"},
+    {file = "charset_normalizer-3.2.0-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:1920d4ff15ce893210c1f0c0e9d19bfbecb7983c76b33f046c13a8ffbd570252"},
+    {file = "charset_normalizer-3.2.0-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:c1c76a1743432b4b60ab3358c937a3fe1341c828ae6194108a94c69028247f22"},
+    {file = "charset_normalizer-3.2.0-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:f7560358a6811e52e9c4d142d497f1a6e10103d3a6881f18d04dbce3729c0e2c"},
+    {file = "charset_normalizer-3.2.0-cp39-cp39-musllinux_1_1_ppc64le.whl", hash = "sha256:c8063cf17b19661471ecbdb3df1c84f24ad2e389e326ccaf89e3fb2484d8dd7e"},
+    {file = "charset_normalizer-3.2.0-cp39-cp39-musllinux_1_1_s390x.whl", hash = "sha256:cd6dbe0238f7743d0efe563ab46294f54f9bc8f4b9bcf57c3c666cc5bc9d1299"},
+    {file = "charset_normalizer-3.2.0-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:1249cbbf3d3b04902ff081ffbb33ce3377fa6e4c7356f759f3cd076cc138d020"},
+    {file = "charset_normalizer-3.2.0-cp39-cp39-win32.whl", hash = "sha256:6c409c0deba34f147f77efaa67b8e4bb83d2f11c8806405f76397ae5b8c0d1c9"},
+    {file = "charset_normalizer-3.2.0-cp39-cp39-win_amd64.whl", hash = "sha256:7095f6fbfaa55defb6b733cfeb14efaae7a29f0b59d8cf213be4e7ca0b857b80"},
+    {file = "charset_normalizer-3.2.0-py3-none-any.whl", hash = "sha256:8e098148dd37b4ce3baca71fb394c81dc5d9c7728c95df695d2dca218edf40e6"},
 ]
 
 [[package]]
 name = "click"
-version = "8.1.3"
+version = "8.1.6"
 description = "Composable command line interface toolkit"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "click-8.1.3-py3-none-any.whl", hash = "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"},
-    {file = "click-8.1.3.tar.gz", hash = "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e"},
+    {file = "click-8.1.6-py3-none-any.whl", hash = "sha256:fa244bb30b3b5ee2cae3da8f55c9e5e0c0e86093306301fb418eb9dc40fbded5"},
+    {file = "click-8.1.6.tar.gz", hash = "sha256:48ee849951919527a045bfe3bf7baa8a959c423134e1a5b98c05c20ba75a1cbd"},
 ]
 
 [package.dependencies]
 colorama = {version = "*", markers = "platform_system == \"Windows\""}
 
 [[package]]
 name = "colorama"
@@ -400,21 +412,21 @@
 ]
 
 [package.extras]
 test = ["pytest (>=6)"]
 
 [[package]]
 name = "furo"
-version = "2023.5.20"
+version = "2023.7.26"
 description = "A clean customisable Sphinx documentation theme."
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "furo-2023.5.20-py3-none-any.whl", hash = "sha256:594a8436ddfe0c071f3a9e9a209c314a219d8341f3f1af33fdf7c69544fab9e6"},
-    {file = "furo-2023.5.20.tar.gz", hash = "sha256:40e09fa17c6f4b22419d122e933089226dcdb59747b5b6c79363089827dea16f"},
+    {file = "furo-2023.7.26-py3-none-any.whl", hash = "sha256:1c7936929ec57c5ddecc7c85f07fa8b2ce536b5c89137764cca508be90e11efd"},
+    {file = "furo-2023.7.26.tar.gz", hash = "sha256:257f63bab97aa85213a1fa24303837a3c3f30be92901ec732fea74290800f59e"},
 ]
 
 [package.dependencies]
 beautifulsoup4 = "*"
 pygments = ">=2.7"
 sphinx = ">=6.0,<8.0"
 sphinx-basic-ng = "*"
@@ -454,21 +466,21 @@
 files = [
     {file = "hpack-4.0.0-py3-none-any.whl", hash = "sha256:84a076fad3dc9a9f8063ccb8041ef100867b1878b25ef0ee63847a5d53818a6c"},
     {file = "hpack-4.0.0.tar.gz", hash = "sha256:fc41de0c63e687ebffde81187a948221294896f6bdc0ae2312708df339430095"},
 ]
 
 [[package]]
 name = "httpcore"
-version = "0.17.2"
+version = "0.17.3"
 description = "A minimal low-level HTTP client."
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "httpcore-0.17.2-py3-none-any.whl", hash = "sha256:5581b9c12379c4288fe70f43c710d16060c10080617001e6b22a3b6dbcbefd36"},
-    {file = "httpcore-0.17.2.tar.gz", hash = "sha256:125f8375ab60036db632f34f4b627a9ad085048eef7cb7d2616fea0f739f98af"},
+    {file = "httpcore-0.17.3-py3-none-any.whl", hash = "sha256:c2789b767ddddfa2a5782e3199b2b7f6894540b17b16ec26b2c4d8e103510b87"},
+    {file = "httpcore-0.17.3.tar.gz", hash = "sha256:a6f30213335e34c1ade7be6ec7c47f19f50c56db36abef1a9dfa3815b1cb3888"},
 ]
 
 [package.dependencies]
 anyio = ">=3.0,<5.0"
 certifi = "*"
 h11 = ">=0.13,<0.15"
 sniffio = "==1.*"
@@ -532,30 +544,30 @@
 files = [
     {file = "imagesize-1.4.1-py2.py3-none-any.whl", hash = "sha256:0d8d18d08f840c19d0ee7ca1fd82490fdc3729b7ac93f49870406ddde8ef8d8b"},
     {file = "imagesize-1.4.1.tar.gz", hash = "sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a"},
 ]
 
 [[package]]
 name = "importlib-metadata"
-version = "6.7.0"
+version = "6.8.0"
 description = "Read metadata from Python packages"
 optional = false
-python-versions = ">=3.7"
+python-versions = ">=3.8"
 files = [
-    {file = "importlib_metadata-6.7.0-py3-none-any.whl", hash = "sha256:cb52082e659e97afc5dac71e79de97d8681de3aa07ff18578330904a9d18e5b5"},
-    {file = "importlib_metadata-6.7.0.tar.gz", hash = "sha256:1aaf550d4f73e5d6783e7acb77aec43d49da8017410afae93822cc9cca98c4d4"},
+    {file = "importlib_metadata-6.8.0-py3-none-any.whl", hash = "sha256:3ebb78df84a805d7698245025b975d9d67053cd94c79245ba4b3eb694abe68bb"},
+    {file = "importlib_metadata-6.8.0.tar.gz", hash = "sha256:dbace7892d8c0c4ac1ad096662232f831d4e64f4c4545bd53016a3e9d4654743"},
 ]
 
 [package.dependencies]
 zipp = ">=0.5"
 
 [package.extras]
 docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
 perf = ["ipython"]
-testing = ["flufl.flake8", "importlib-resources (>=1.3)", "packaging", "pyfakefs", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-mypy (>=0.9.1)", "pytest-perf (>=0.9.2)", "pytest-ruff"]
+testing = ["flufl.flake8", "importlib-resources (>=1.3)", "packaging", "pyfakefs", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=2.2)", "pytest-mypy (>=0.9.1)", "pytest-perf (>=0.9.2)", "pytest-ruff"]
 
 [[package]]
 name = "isort"
 version = "5.12.0"
 description = "A Python utility / library to sort Python imports."
 optional = false
 python-versions = ">=3.8.0"
@@ -608,26 +620,30 @@
 description = "Powerful and Pythonic XML processing library combining libxml2/libxslt with the ElementTree API."
 optional = false
 python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, != 3.4.*"
 files = [
     {file = "lxml-4.9.3-cp27-cp27m-macosx_11_0_x86_64.whl", hash = "sha256:b0a545b46b526d418eb91754565ba5b63b1c0b12f9bd2f808c852d9b4b2f9b5c"},
     {file = "lxml-4.9.3-cp27-cp27m-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:075b731ddd9e7f68ad24c635374211376aa05a281673ede86cbe1d1b3455279d"},
     {file = "lxml-4.9.3-cp27-cp27m-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:1e224d5755dba2f4a9498e150c43792392ac9b5380aa1b845f98a1618c94eeef"},
+    {file = "lxml-4.9.3-cp27-cp27m-win32.whl", hash = "sha256:2c74524e179f2ad6d2a4f7caf70e2d96639c0954c943ad601a9e146c76408ed7"},
+    {file = "lxml-4.9.3-cp27-cp27m-win_amd64.whl", hash = "sha256:4f1026bc732b6a7f96369f7bfe1a4f2290fb34dce00d8644bc3036fb351a4ca1"},
     {file = "lxml-4.9.3-cp27-cp27mu-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:c0781a98ff5e6586926293e59480b64ddd46282953203c76ae15dbbbf302e8bb"},
     {file = "lxml-4.9.3-cp27-cp27mu-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:cef2502e7e8a96fe5ad686d60b49e1ab03e438bd9123987994528febd569868e"},
     {file = "lxml-4.9.3-cp310-cp310-macosx_11_0_x86_64.whl", hash = "sha256:b86164d2cff4d3aaa1f04a14685cbc072efd0b4f99ca5708b2ad1b9b5988a991"},
     {file = "lxml-4.9.3-cp310-cp310-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_24_i686.whl", hash = "sha256:42871176e7896d5d45138f6d28751053c711ed4d48d8e30b498da155af39aebd"},
+    {file = "lxml-4.9.3-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:ae8b9c6deb1e634ba4f1930eb67ef6e6bf6a44b6eb5ad605642b2d6d5ed9ce3c"},
     {file = "lxml-4.9.3-cp310-cp310-manylinux_2_28_aarch64.whl", hash = "sha256:411007c0d88188d9f621b11d252cce90c4a2d1a49db6c068e3c16422f306eab8"},
     {file = "lxml-4.9.3-cp310-cp310-manylinux_2_28_x86_64.whl", hash = "sha256:cd47b4a0d41d2afa3e58e5bf1f62069255aa2fd6ff5ee41604418ca925911d76"},
     {file = "lxml-4.9.3-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:0e2cb47860da1f7e9a5256254b74ae331687b9672dfa780eed355c4c9c3dbd23"},
     {file = "lxml-4.9.3-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:1247694b26342a7bf47c02e513d32225ededd18045264d40758abeb3c838a51f"},
     {file = "lxml-4.9.3-cp310-cp310-win32.whl", hash = "sha256:cdb650fc86227eba20de1a29d4b2c1bfe139dc75a0669270033cb2ea3d391b85"},
     {file = "lxml-4.9.3-cp310-cp310-win_amd64.whl", hash = "sha256:97047f0d25cd4bcae81f9ec9dc290ca3e15927c192df17331b53bebe0e3ff96d"},
     {file = "lxml-4.9.3-cp311-cp311-macosx_11_0_universal2.whl", hash = "sha256:1f447ea5429b54f9582d4b955f5f1985f278ce5cf169f72eea8afd9502973dd5"},
     {file = "lxml-4.9.3-cp311-cp311-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_24_i686.whl", hash = "sha256:57d6ba0ca2b0c462f339640d22882acc711de224d769edf29962b09f77129cbf"},
+    {file = "lxml-4.9.3-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:9767e79108424fb6c3edf8f81e6730666a50feb01a328f4a016464a5893f835a"},
     {file = "lxml-4.9.3-cp311-cp311-manylinux_2_28_aarch64.whl", hash = "sha256:71c52db65e4b56b8ddc5bb89fb2e66c558ed9d1a74a45ceb7dcb20c191c3df2f"},
     {file = "lxml-4.9.3-cp311-cp311-manylinux_2_28_x86_64.whl", hash = "sha256:d73d8ecf8ecf10a3bd007f2192725a34bd62898e8da27eb9d32a58084f93962b"},
     {file = "lxml-4.9.3-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:0a3d3487f07c1d7f150894c238299934a2a074ef590b583103a45002035be120"},
     {file = "lxml-4.9.3-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:9e28c51fa0ce5674be9f560c6761c1b441631901993f76700b1b30ca6c8378d6"},
     {file = "lxml-4.9.3-cp311-cp311-win32.whl", hash = "sha256:0bfd0767c5c1de2551a120673b72e5d4b628737cb05414f03c3277bf9bed3305"},
     {file = "lxml-4.9.3-cp311-cp311-win_amd64.whl", hash = "sha256:25f32acefac14ef7bd53e4218fe93b804ef6f6b92ffdb4322bb6d49d94cad2bc"},
     {file = "lxml-4.9.3-cp312-cp312-macosx_11_0_universal2.whl", hash = "sha256:d3ff32724f98fbbbfa9f49d82852b159e9784d6094983d9a8b7f2ddaebb063d4"},
@@ -639,58 +655,65 @@
     {file = "lxml-4.9.3-cp35-cp35m-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:56dc1f1ebccc656d1b3ed288f11e27172a01503fc016bcabdcbc0978b19352b7"},
     {file = "lxml-4.9.3-cp35-cp35m-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:578695735c5a3f51569810dfebd05dd6f888147a34f0f98d4bb27e92b76e05c2"},
     {file = "lxml-4.9.3-cp35-cp35m-win32.whl", hash = "sha256:704f61ba8c1283c71b16135caf697557f5ecf3e74d9e453233e4771d68a1f42d"},
     {file = "lxml-4.9.3-cp35-cp35m-win_amd64.whl", hash = "sha256:c41bfca0bd3532d53d16fd34d20806d5c2b1ace22a2f2e4c0008570bf2c58833"},
     {file = "lxml-4.9.3-cp36-cp36m-macosx_11_0_x86_64.whl", hash = "sha256:64f479d719dc9f4c813ad9bb6b28f8390360660b73b2e4beb4cb0ae7104f1c12"},
     {file = "lxml-4.9.3-cp36-cp36m-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_24_i686.whl", hash = "sha256:dd708cf4ee4408cf46a48b108fb9427bfa00b9b85812a9262b5c668af2533ea5"},
     {file = "lxml-4.9.3-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5c31c7462abdf8f2ac0577d9f05279727e698f97ecbb02f17939ea99ae8daa98"},
+    {file = "lxml-4.9.3-cp36-cp36m-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:e3cd95e10c2610c360154afdc2f1480aea394f4a4f1ea0a5eacce49640c9b190"},
     {file = "lxml-4.9.3-cp36-cp36m-manylinux_2_28_x86_64.whl", hash = "sha256:4930be26af26ac545c3dffb662521d4e6268352866956672231887d18f0eaab2"},
     {file = "lxml-4.9.3-cp36-cp36m-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:4aec80cde9197340bc353d2768e2a75f5f60bacda2bab72ab1dc499589b3878c"},
     {file = "lxml-4.9.3-cp36-cp36m-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:14e019fd83b831b2e61baed40cab76222139926b1fb5ed0e79225bc0cae14584"},
     {file = "lxml-4.9.3-cp36-cp36m-musllinux_1_1_aarch64.whl", hash = "sha256:0c0850c8b02c298d3c7006b23e98249515ac57430e16a166873fc47a5d549287"},
     {file = "lxml-4.9.3-cp36-cp36m-musllinux_1_1_x86_64.whl", hash = "sha256:aca086dc5f9ef98c512bac8efea4483eb84abbf926eaeedf7b91479feb092458"},
     {file = "lxml-4.9.3-cp36-cp36m-win32.whl", hash = "sha256:50baa9c1c47efcaef189f31e3d00d697c6d4afda5c3cde0302d063492ff9b477"},
     {file = "lxml-4.9.3-cp36-cp36m-win_amd64.whl", hash = "sha256:bef4e656f7d98aaa3486d2627e7d2df1157d7e88e7efd43a65aa5dd4714916cf"},
     {file = "lxml-4.9.3-cp37-cp37m-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_24_i686.whl", hash = "sha256:46f409a2d60f634fe550f7133ed30ad5321ae2e6630f13657fb9479506b00601"},
     {file = "lxml-4.9.3-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.manylinux_2_24_aarch64.whl", hash = "sha256:4c28a9144688aef80d6ea666c809b4b0e50010a2aca784c97f5e6bf143d9f129"},
+    {file = "lxml-4.9.3-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:141f1d1a9b663c679dc524af3ea1773e618907e96075262726c7612c02b149a4"},
     {file = "lxml-4.9.3-cp37-cp37m-manylinux_2_28_x86_64.whl", hash = "sha256:53ace1c1fd5a74ef662f844a0413446c0629d151055340e9893da958a374f70d"},
     {file = "lxml-4.9.3-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:17a753023436a18e27dd7769e798ce302963c236bc4114ceee5b25c18c52c693"},
     {file = "lxml-4.9.3-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:7d298a1bd60c067ea75d9f684f5f3992c9d6766fadbc0bcedd39750bf344c2f4"},
     {file = "lxml-4.9.3-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:081d32421db5df44c41b7f08a334a090a545c54ba977e47fd7cc2deece78809a"},
     {file = "lxml-4.9.3-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:23eed6d7b1a3336ad92d8e39d4bfe09073c31bfe502f20ca5116b2a334f8ec02"},
     {file = "lxml-4.9.3-cp37-cp37m-win32.whl", hash = "sha256:1509dd12b773c02acd154582088820893109f6ca27ef7291b003d0e81666109f"},
     {file = "lxml-4.9.3-cp37-cp37m-win_amd64.whl", hash = "sha256:120fa9349a24c7043854c53cae8cec227e1f79195a7493e09e0c12e29f918e52"},
     {file = "lxml-4.9.3-cp38-cp38-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_24_i686.whl", hash = "sha256:4d2d1edbca80b510443f51afd8496be95529db04a509bc8faee49c7b0fb6d2cc"},
     {file = "lxml-4.9.3-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.manylinux_2_24_aarch64.whl", hash = "sha256:8d7e43bd40f65f7d97ad8ef5c9b1778943d02f04febef12def25f7583d19baac"},
+    {file = "lxml-4.9.3-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:71d66ee82e7417828af6ecd7db817913cb0cf9d4e61aa0ac1fde0583d84358db"},
     {file = "lxml-4.9.3-cp38-cp38-manylinux_2_28_x86_64.whl", hash = "sha256:6fc3c450eaa0b56f815c7b62f2b7fba7266c4779adcf1cece9e6deb1de7305ce"},
     {file = "lxml-4.9.3-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:65299ea57d82fb91c7f019300d24050c4ddeb7c5a190e076b5f48a2b43d19c42"},
     {file = "lxml-4.9.3-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:eadfbbbfb41b44034a4c757fd5d70baccd43296fb894dba0295606a7cf3124aa"},
     {file = "lxml-4.9.3-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:3e9bdd30efde2b9ccfa9cb5768ba04fe71b018a25ea093379c857c9dad262c40"},
     {file = "lxml-4.9.3-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:fcdd00edfd0a3001e0181eab3e63bd5c74ad3e67152c84f93f13769a40e073a7"},
     {file = "lxml-4.9.3-cp38-cp38-win32.whl", hash = "sha256:57aba1bbdf450b726d58b2aea5fe47c7875f5afb2c4a23784ed78f19a0462574"},
     {file = "lxml-4.9.3-cp38-cp38-win_amd64.whl", hash = "sha256:92af161ecbdb2883c4593d5ed4815ea71b31fafd7fd05789b23100d081ecac96"},
     {file = "lxml-4.9.3-cp39-cp39-macosx_11_0_x86_64.whl", hash = "sha256:9bb6ad405121241e99a86efff22d3ef469024ce22875a7ae045896ad23ba2340"},
     {file = "lxml-4.9.3-cp39-cp39-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_24_i686.whl", hash = "sha256:8ed74706b26ad100433da4b9d807eae371efaa266ffc3e9191ea436087a9d6a7"},
+    {file = "lxml-4.9.3-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:fbf521479bcac1e25a663df882c46a641a9bff6b56dc8b0fafaebd2f66fb231b"},
     {file = "lxml-4.9.3-cp39-cp39-manylinux_2_28_aarch64.whl", hash = "sha256:303bf1edce6ced16bf67a18a1cf8339d0db79577eec5d9a6d4a80f0fb10aa2da"},
     {file = "lxml-4.9.3-cp39-cp39-manylinux_2_28_x86_64.whl", hash = "sha256:5515edd2a6d1a5a70bfcdee23b42ec33425e405c5b351478ab7dc9347228f96e"},
     {file = "lxml-4.9.3-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:690dafd0b187ed38583a648076865d8c229661ed20e48f2335d68e2cf7dc829d"},
     {file = "lxml-4.9.3-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:b6420a005548ad52154c8ceab4a1290ff78d757f9e5cbc68f8c77089acd3c432"},
     {file = "lxml-4.9.3-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:bb3bb49c7a6ad9d981d734ef7c7193bc349ac338776a0360cc671eaee89bcf69"},
     {file = "lxml-4.9.3-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:d27be7405547d1f958b60837dc4c1007da90b8b23f54ba1f8b728c78fdb19d50"},
     {file = "lxml-4.9.3-cp39-cp39-win32.whl", hash = "sha256:8df133a2ea5e74eef5e8fc6f19b9e085f758768a16e9877a60aec455ed2609b2"},
     {file = "lxml-4.9.3-cp39-cp39-win_amd64.whl", hash = "sha256:4dd9a263e845a72eacb60d12401e37c616438ea2e5442885f65082c276dfb2b2"},
     {file = "lxml-4.9.3-pp310-pypy310_pp73-manylinux_2_28_x86_64.whl", hash = "sha256:6689a3d7fd13dc687e9102a27e98ef33730ac4fe37795d5036d18b4d527abd35"},
     {file = "lxml-4.9.3-pp37-pypy37_pp73-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_24_i686.whl", hash = "sha256:f6bdac493b949141b733c5345b6ba8f87a226029cbabc7e9e121a413e49441e0"},
+    {file = "lxml-4.9.3-pp37-pypy37_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:05186a0f1346ae12553d66df1cfce6f251589fea3ad3da4f3ef4e34b2d58c6a3"},
     {file = "lxml-4.9.3-pp37-pypy37_pp73-manylinux_2_28_x86_64.whl", hash = "sha256:c2006f5c8d28dee289f7020f721354362fa304acbaaf9745751ac4006650254b"},
     {file = "lxml-4.9.3-pp38-pypy38_pp73-macosx_11_0_x86_64.whl", hash = "sha256:5c245b783db29c4e4fbbbfc9c5a78be496c9fea25517f90606aa1f6b2b3d5f7b"},
     {file = "lxml-4.9.3-pp38-pypy38_pp73-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_24_i686.whl", hash = "sha256:4fb960a632a49f2f089d522f70496640fdf1218f1243889da3822e0a9f5f3ba7"},
+    {file = "lxml-4.9.3-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:50670615eaf97227d5dc60de2dc99fb134a7130d310d783314e7724bf163f75d"},
     {file = "lxml-4.9.3-pp38-pypy38_pp73-manylinux_2_28_x86_64.whl", hash = "sha256:9719fe17307a9e814580af1f5c6e05ca593b12fb7e44fe62450a5384dbf61b4b"},
     {file = "lxml-4.9.3-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:3331bece23c9ee066e0fb3f96c61322b9e0f54d775fccefff4c38ca488de283a"},
     {file = "lxml-4.9.3-pp39-pypy39_pp73-macosx_11_0_x86_64.whl", hash = "sha256:ed667f49b11360951e201453fc3967344d0d0263aa415e1619e85ae7fd17b4e0"},
     {file = "lxml-4.9.3-pp39-pypy39_pp73-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_24_i686.whl", hash = "sha256:8b77946fd508cbf0fccd8e400a7f71d4ac0e1595812e66025bac475a8e811694"},
+    {file = "lxml-4.9.3-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux_2_24_x86_64.whl", hash = "sha256:e4da8ca0c0c0aea88fd46be8e44bd49716772358d648cce45fe387f7b92374a7"},
     {file = "lxml-4.9.3-pp39-pypy39_pp73-manylinux_2_28_x86_64.whl", hash = "sha256:fe4bda6bd4340caa6e5cf95e73f8fea5c4bfc55763dd42f1b50a94c1b4a2fbd4"},
     {file = "lxml-4.9.3-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:f3df3db1d336b9356dd3112eae5f5c2b8b377f3bc826848567f10bfddfee77e9"},
     {file = "lxml-4.9.3.tar.gz", hash = "sha256:48628bd53a426c9eb9bc066a923acaa0878d1e86129fd5359aee99285f4eed9c"},
 ]
 
 [package.extras]
 cssselect = ["cssselect (>=0.7)"]
@@ -808,14 +831,60 @@
 python-versions = ">=3.7"
 files = [
     {file = "mdurl-0.1.2-py3-none-any.whl", hash = "sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8"},
     {file = "mdurl-0.1.2.tar.gz", hash = "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"},
 ]
 
 [[package]]
+name = "mypy"
+version = "1.4.1"
+description = "Optional static typing for Python"
+optional = false
+python-versions = ">=3.7"
+files = [
+    {file = "mypy-1.4.1-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:566e72b0cd6598503e48ea610e0052d1b8168e60a46e0bfd34b3acf2d57f96a8"},
+    {file = "mypy-1.4.1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:ca637024ca67ab24a7fd6f65d280572c3794665eaf5edcc7e90a866544076878"},
+    {file = "mypy-1.4.1-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:0dde1d180cd84f0624c5dcaaa89c89775550a675aff96b5848de78fb11adabcd"},
+    {file = "mypy-1.4.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:8c4d8e89aa7de683e2056a581ce63c46a0c41e31bd2b6d34144e2c80f5ea53dc"},
+    {file = "mypy-1.4.1-cp310-cp310-win_amd64.whl", hash = "sha256:bfdca17c36ae01a21274a3c387a63aa1aafe72bff976522886869ef131b937f1"},
+    {file = "mypy-1.4.1-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:7549fbf655e5825d787bbc9ecf6028731973f78088fbca3a1f4145c39ef09462"},
+    {file = "mypy-1.4.1-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:98324ec3ecf12296e6422939e54763faedbfcc502ea4a4c38502082711867258"},
+    {file = "mypy-1.4.1-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:141dedfdbfe8a04142881ff30ce6e6653c9685b354876b12e4fe6c78598b45e2"},
+    {file = "mypy-1.4.1-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:8207b7105829eca6f3d774f64a904190bb2231de91b8b186d21ffd98005f14a7"},
+    {file = "mypy-1.4.1-cp311-cp311-win_amd64.whl", hash = "sha256:16f0db5b641ba159eff72cff08edc3875f2b62b2fa2bc24f68c1e7a4e8232d01"},
+    {file = "mypy-1.4.1-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:470c969bb3f9a9efcedbadcd19a74ffb34a25f8e6b0e02dae7c0e71f8372f97b"},
+    {file = "mypy-1.4.1-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e5952d2d18b79f7dc25e62e014fe5a23eb1a3d2bc66318df8988a01b1a037c5b"},
+    {file = "mypy-1.4.1-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:190b6bab0302cec4e9e6767d3eb66085aef2a1cc98fe04936d8a42ed2ba77bb7"},
+    {file = "mypy-1.4.1-cp37-cp37m-win_amd64.whl", hash = "sha256:9d40652cc4fe33871ad3338581dca3297ff5f2213d0df345bcfbde5162abf0c9"},
+    {file = "mypy-1.4.1-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:01fd2e9f85622d981fd9063bfaef1aed6e336eaacca00892cd2d82801ab7c042"},
+    {file = "mypy-1.4.1-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:2460a58faeea905aeb1b9b36f5065f2dc9a9c6e4c992a6499a2360c6c74ceca3"},
+    {file = "mypy-1.4.1-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a2746d69a8196698146a3dbe29104f9eb6a2a4d8a27878d92169a6c0b74435b6"},
+    {file = "mypy-1.4.1-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:ae704dcfaa180ff7c4cfbad23e74321a2b774f92ca77fd94ce1049175a21c97f"},
+    {file = "mypy-1.4.1-cp38-cp38-win_amd64.whl", hash = "sha256:43d24f6437925ce50139a310a64b2ab048cb2d3694c84c71c3f2a1626d8101dc"},
+    {file = "mypy-1.4.1-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:c482e1246726616088532b5e964e39765b6d1520791348e6c9dc3af25b233828"},
+    {file = "mypy-1.4.1-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:43b592511672017f5b1a483527fd2684347fdffc041c9ef53428c8dc530f79a3"},
+    {file = "mypy-1.4.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:34a9239d5b3502c17f07fd7c0b2ae6b7dd7d7f6af35fbb5072c6208e76295816"},
+    {file = "mypy-1.4.1-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:5703097c4936bbb9e9bce41478c8d08edd2865e177dc4c52be759f81ee4dd26c"},
+    {file = "mypy-1.4.1-cp39-cp39-win_amd64.whl", hash = "sha256:e02d700ec8d9b1859790c0475df4e4092c7bf3272a4fd2c9f33d87fac4427b8f"},
+    {file = "mypy-1.4.1-py3-none-any.whl", hash = "sha256:45d32cec14e7b97af848bddd97d85ea4f0db4d5a149ed9676caa4eb2f7402bb4"},
+    {file = "mypy-1.4.1.tar.gz", hash = "sha256:9bbcd9ab8ea1f2e1c8031c21445b511442cc45c89951e49bbf852cbb70755b1b"},
+]
+
+[package.dependencies]
+mypy-extensions = ">=1.0.0"
+tomli = {version = ">=1.1.0", markers = "python_version < \"3.11\""}
+typing-extensions = ">=4.1.0"
+
+[package.extras]
+dmypy = ["psutil (>=4.0)"]
+install-types = ["pip"]
+python2 = ["typed-ast (>=1.4.0,<2)"]
+reports = ["lxml"]
+
+[[package]]
 name = "mypy-extensions"
 version = "1.0.0"
 description = "Type system extensions for programs checked with the mypy type checker."
 optional = false
 python-versions = ">=3.5"
 files = [
     {file = "mypy_extensions-1.0.0-py3-none-any.whl", hash = "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d"},
@@ -868,21 +937,21 @@
 files = [
     {file = "pathspec-0.11.1-py3-none-any.whl", hash = "sha256:d8af70af76652554bd134c22b3e8a1cc46ed7d91edcdd721ef1a0c51a84a5293"},
     {file = "pathspec-0.11.1.tar.gz", hash = "sha256:2798de800fa92780e33acca925945e9a19a133b715067cf165b8866c15a31687"},
 ]
 
 [[package]]
 name = "platformdirs"
-version = "3.8.0"
+version = "3.9.1"
 description = "A small Python package for determining appropriate platform-specific dirs, e.g. a \"user data dir\"."
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "platformdirs-3.8.0-py3-none-any.whl", hash = "sha256:ca9ed98ce73076ba72e092b23d3c93ea6c4e186b3f1c3dad6edd98ff6ffcca2e"},
-    {file = "platformdirs-3.8.0.tar.gz", hash = "sha256:b0cabcb11063d21a0b261d557acb0a9d2126350e63b70cdf7db6347baea456dc"},
+    {file = "platformdirs-3.9.1-py3-none-any.whl", hash = "sha256:ad8291ae0ae5072f66c16945166cb11c63394c7a3ad1b1bc9828ca3162da8c2f"},
+    {file = "platformdirs-3.9.1.tar.gz", hash = "sha256:1b42b450ad933e981d56e59f1b97495428c9bd60698baab9f3eb3d00d5822421"},
 ]
 
 [package.extras]
 docs = ["furo (>=2023.5.20)", "proselint (>=0.13)", "sphinx (>=7.0.1)", "sphinx-autodoc-typehints (>=1.23,!=1.23.4)"]
 test = ["appdirs (==1.4.4)", "covdefaults (>=2.3)", "pytest (>=7.3.1)", "pytest-cov (>=4.1)", "pytest-mock (>=3.10)"]
 
 [[package]]
@@ -933,59 +1002,59 @@
 doc = ["sphinx (>=4.5.0)", "tabulate (>=0.8.9)"]
 gendocs = ["pytoolconfig[doc]", "sphinx (>=4.5.0)", "sphinx-autodoc-typehints (>=1.18.1)", "sphinx-rtd-theme (>=1.0.0)"]
 global = ["platformdirs (>=1.4.4)"]
 validation = ["pydantic (>=1.7.4)"]
 
 [[package]]
 name = "pyyaml"
-version = "6.0"
+version = "6.0.1"
 description = "YAML parser and emitter for Python"
 optional = false
 python-versions = ">=3.6"
 files = [
-    {file = "PyYAML-6.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:d4db7c7aef085872ef65a8fd7d6d09a14ae91f691dec3e87ee5ee0539d516f53"},
-    {file = "PyYAML-6.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:9df7ed3b3d2e0ecfe09e14741b857df43adb5a3ddadc919a2d94fbdf78fea53c"},
-    {file = "PyYAML-6.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:77f396e6ef4c73fdc33a9157446466f1cff553d979bd00ecb64385760c6babdc"},
-    {file = "PyYAML-6.0-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:a80a78046a72361de73f8f395f1f1e49f956c6be882eed58505a15f3e430962b"},
-    {file = "PyYAML-6.0-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"},
-    {file = "PyYAML-6.0-cp310-cp310-win32.whl", hash = "sha256:2cd5df3de48857ed0544b34e2d40e9fac445930039f3cfe4bcc592a1f836d513"},
-    {file = "PyYAML-6.0-cp310-cp310-win_amd64.whl", hash = "sha256:daf496c58a8c52083df09b80c860005194014c3698698d1a57cbcfa182142a3a"},
-    {file = "PyYAML-6.0-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:d4b0ba9512519522b118090257be113b9468d804b19d63c71dbcf4a48fa32358"},
-    {file = "PyYAML-6.0-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:81957921f441d50af23654aa6c5e5eaf9b06aba7f0a19c18a538dc7ef291c5a1"},
-    {file = "PyYAML-6.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:afa17f5bc4d1b10afd4466fd3a44dc0e245382deca5b3c353d8b757f9e3ecb8d"},
-    {file = "PyYAML-6.0-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:dbad0e9d368bb989f4515da330b88a057617d16b6a8245084f1b05400f24609f"},
-    {file = "PyYAML-6.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:432557aa2c09802be39460360ddffd48156e30721f5e8d917f01d31694216782"},
-    {file = "PyYAML-6.0-cp311-cp311-win32.whl", hash = "sha256:bfaef573a63ba8923503d27530362590ff4f576c626d86a9fed95822a8255fd7"},
-    {file = "PyYAML-6.0-cp311-cp311-win_amd64.whl", hash = "sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf"},
-    {file = "PyYAML-6.0-cp36-cp36m-macosx_10_9_x86_64.whl", hash = "sha256:897b80890765f037df3403d22bab41627ca8811ae55e9a722fd0392850ec4d86"},
-    {file = "PyYAML-6.0-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:50602afada6d6cbfad699b0c7bb50d5ccffa7e46a3d738092afddc1f9758427f"},
-    {file = "PyYAML-6.0-cp36-cp36m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:48c346915c114f5fdb3ead70312bd042a953a8ce5c7106d5bfb1a5254e47da92"},
-    {file = "PyYAML-6.0-cp36-cp36m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:98c4d36e99714e55cfbaaee6dd5badbc9a1ec339ebfc3b1f52e293aee6bb71a4"},
-    {file = "PyYAML-6.0-cp36-cp36m-win32.whl", hash = "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293"},
-    {file = "PyYAML-6.0-cp36-cp36m-win_amd64.whl", hash = "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57"},
-    {file = "PyYAML-6.0-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:819b3830a1543db06c4d4b865e70ded25be52a2e0631ccd2f6a47a2822f2fd7c"},
-    {file = "PyYAML-6.0-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:473f9edb243cb1935ab5a084eb238d842fb8f404ed2193a915d1784b5a6b5fc0"},
-    {file = "PyYAML-6.0-cp37-cp37m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:0ce82d761c532fe4ec3f87fc45688bdd3a4c1dc5e0b4a19814b9009a29baefd4"},
-    {file = "PyYAML-6.0-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:231710d57adfd809ef5d34183b8ed1eeae3f76459c18fb4a0b373ad56bedcdd9"},
-    {file = "PyYAML-6.0-cp37-cp37m-win32.whl", hash = "sha256:c5687b8d43cf58545ade1fe3e055f70eac7a5a1a0bf42824308d868289a95737"},
-    {file = "PyYAML-6.0-cp37-cp37m-win_amd64.whl", hash = "sha256:d15a181d1ecd0d4270dc32edb46f7cb7733c7c508857278d3d378d14d606db2d"},
-    {file = "PyYAML-6.0-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:0b4624f379dab24d3725ffde76559cff63d9ec94e1736b556dacdfebe5ab6d4b"},
-    {file = "PyYAML-6.0-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:213c60cd50106436cc818accf5baa1aba61c0189ff610f64f4a3e8c6726218ba"},
-    {file = "PyYAML-6.0-cp38-cp38-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:9fa600030013c4de8165339db93d182b9431076eb98eb40ee068700c9c813e34"},
-    {file = "PyYAML-6.0-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:277a0ef2981ca40581a47093e9e2d13b3f1fbbeffae064c1d21bfceba2030287"},
-    {file = "PyYAML-6.0-cp38-cp38-win32.whl", hash = "sha256:d4eccecf9adf6fbcc6861a38015c2a64f38b9d94838ac1810a9023a0609e1b78"},
-    {file = "PyYAML-6.0-cp38-cp38-win_amd64.whl", hash = "sha256:1e4747bc279b4f613a09eb64bba2ba602d8a6664c6ce6396a4d0cd413a50ce07"},
-    {file = "PyYAML-6.0-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b"},
-    {file = "PyYAML-6.0-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174"},
-    {file = "PyYAML-6.0-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d67d839ede4ed1b28a4e8909735fc992a923cdb84e618544973d7dfc71540803"},
-    {file = "PyYAML-6.0-cp39-cp39-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:cba8c411ef271aa037d7357a2bc8f9ee8b58b9965831d9e51baf703280dc73d3"},
-    {file = "PyYAML-6.0-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_12_x86_64.manylinux2010_x86_64.whl", hash = "sha256:40527857252b61eacd1d9af500c3337ba8deb8fc298940291486c465c8b46ec0"},
-    {file = "PyYAML-6.0-cp39-cp39-win32.whl", hash = "sha256:b5b9eccad747aabaaffbc6064800670f0c297e52c12754eb1d976c57e4f74dcb"},
-    {file = "PyYAML-6.0-cp39-cp39-win_amd64.whl", hash = "sha256:b3d267842bf12586ba6c734f89d1f5b871df0273157918b0ccefa29deb05c21c"},
-    {file = "PyYAML-6.0.tar.gz", hash = "sha256:68fb519c14306fec9720a2a5b45bc9f0c8d1b9c72adf45c37baedfcd949c35a2"},
+    {file = "PyYAML-6.0.1-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:d858aa552c999bc8a8d57426ed01e40bef403cd8ccdd0fc5f6f04a00414cac2a"},
+    {file = "PyYAML-6.0.1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:fd66fc5d0da6d9815ba2cebeb4205f95818ff4b79c3ebe268e75d961704af52f"},
+    {file = "PyYAML-6.0.1-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:69b023b2b4daa7548bcfbd4aa3da05b3a74b772db9e23b982788168117739938"},
+    {file = "PyYAML-6.0.1-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:81e0b275a9ecc9c0c0c07b4b90ba548307583c125f54d5b6946cfee6360c733d"},
+    {file = "PyYAML-6.0.1-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ba336e390cd8e4d1739f42dfe9bb83a3cc2e80f567d8805e11b46f4a943f5515"},
+    {file = "PyYAML-6.0.1-cp310-cp310-win32.whl", hash = "sha256:bd4af7373a854424dabd882decdc5579653d7868b8fb26dc7d0e99f823aa5924"},
+    {file = "PyYAML-6.0.1-cp310-cp310-win_amd64.whl", hash = "sha256:fd1592b3fdf65fff2ad0004b5e363300ef59ced41c2e6b3a99d4089fa8c5435d"},
+    {file = "PyYAML-6.0.1-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:6965a7bc3cf88e5a1c3bd2e0b5c22f8d677dc88a455344035f03399034eb3007"},
+    {file = "PyYAML-6.0.1-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:f003ed9ad21d6a4713f0a9b5a7a0a79e08dd0f221aff4525a2be4c346ee60aab"},
+    {file = "PyYAML-6.0.1-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:42f8152b8dbc4fe7d96729ec2b99c7097d656dc1213a3229ca5383f973a5ed6d"},
+    {file = "PyYAML-6.0.1-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:062582fca9fabdd2c8b54a3ef1c978d786e0f6b3a1510e0ac93ef59e0ddae2bc"},
+    {file = "PyYAML-6.0.1-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d2b04aac4d386b172d5b9692e2d2da8de7bfb6c387fa4f801fbf6fb2e6ba4673"},
+    {file = "PyYAML-6.0.1-cp311-cp311-win32.whl", hash = "sha256:1635fd110e8d85d55237ab316b5b011de701ea0f29d07611174a1b42f1444741"},
+    {file = "PyYAML-6.0.1-cp311-cp311-win_amd64.whl", hash = "sha256:bf07ee2fef7014951eeb99f56f39c9bb4af143d8aa3c21b1677805985307da34"},
+    {file = "PyYAML-6.0.1-cp36-cp36m-macosx_10_9_x86_64.whl", hash = "sha256:50550eb667afee136e9a77d6dc71ae76a44df8b3e51e41b77f6de2932bfe0f47"},
+    {file = "PyYAML-6.0.1-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:1fe35611261b29bd1de0070f0b2f47cb6ff71fa6595c077e42bd0c419fa27b98"},
+    {file = "PyYAML-6.0.1-cp36-cp36m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:704219a11b772aea0d8ecd7058d0082713c3562b4e271b849ad7dc4a5c90c13c"},
+    {file = "PyYAML-6.0.1-cp36-cp36m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:afd7e57eddb1a54f0f1a974bc4391af8bcce0b444685d936840f125cf046d5bd"},
+    {file = "PyYAML-6.0.1-cp36-cp36m-win32.whl", hash = "sha256:fca0e3a251908a499833aa292323f32437106001d436eca0e6e7833256674585"},
+    {file = "PyYAML-6.0.1-cp36-cp36m-win_amd64.whl", hash = "sha256:f22ac1c3cac4dbc50079e965eba2c1058622631e526bd9afd45fedd49ba781fa"},
+    {file = "PyYAML-6.0.1-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:b1275ad35a5d18c62a7220633c913e1b42d44b46ee12554e5fd39c70a243d6a3"},
+    {file = "PyYAML-6.0.1-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:18aeb1bf9a78867dc38b259769503436b7c72f7a1f1f4c93ff9a17de54319b27"},
+    {file = "PyYAML-6.0.1-cp37-cp37m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:596106435fa6ad000c2991a98fa58eeb8656ef2325d7e158344fb33864ed87e3"},
+    {file = "PyYAML-6.0.1-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:baa90d3f661d43131ca170712d903e6295d1f7a0f595074f151c0aed377c9b9c"},
+    {file = "PyYAML-6.0.1-cp37-cp37m-win32.whl", hash = "sha256:9046c58c4395dff28dd494285c82ba00b546adfc7ef001486fbf0324bc174fba"},
+    {file = "PyYAML-6.0.1-cp37-cp37m-win_amd64.whl", hash = "sha256:4fb147e7a67ef577a588a0e2c17b6db51dda102c71de36f8549b6816a96e1867"},
+    {file = "PyYAML-6.0.1-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:1d4c7e777c441b20e32f52bd377e0c409713e8bb1386e1099c2415f26e479595"},
+    {file = "PyYAML-6.0.1-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a0cd17c15d3bb3fa06978b4e8958dcdc6e0174ccea823003a106c7d4d7899ac5"},
+    {file = "PyYAML-6.0.1-cp38-cp38-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:28c119d996beec18c05208a8bd78cbe4007878c6dd15091efb73a30e90539696"},
+    {file = "PyYAML-6.0.1-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:7e07cbde391ba96ab58e532ff4803f79c4129397514e1413a7dc761ccd755735"},
+    {file = "PyYAML-6.0.1-cp38-cp38-win32.whl", hash = "sha256:184c5108a2aca3c5b3d3bf9395d50893a7ab82a38004c8f61c258d4428e80206"},
+    {file = "PyYAML-6.0.1-cp38-cp38-win_amd64.whl", hash = "sha256:1e2722cc9fbb45d9b87631ac70924c11d3a401b2d7f410cc0e3bbf249f2dca62"},
+    {file = "PyYAML-6.0.1-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:9eb6caa9a297fc2c2fb8862bc5370d0303ddba53ba97e71f08023b6cd73d16a8"},
+    {file = "PyYAML-6.0.1-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:c8098ddcc2a85b61647b2590f825f3db38891662cfc2fc776415143f599bb859"},
+    {file = "PyYAML-6.0.1-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5773183b6446b2c99bb77e77595dd486303b4faab2b086e7b17bc6bef28865f6"},
+    {file = "PyYAML-6.0.1-cp39-cp39-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:b786eecbdf8499b9ca1d697215862083bd6d2a99965554781d0d8d1ad31e13a0"},
+    {file = "PyYAML-6.0.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:bc1bf2925a1ecd43da378f4db9e4f799775d6367bdb94671027b73b393a7c42c"},
+    {file = "PyYAML-6.0.1-cp39-cp39-win32.whl", hash = "sha256:faca3bdcf85b2fc05d06ff3fbc1f83e1391b3e724afa3feba7d13eeab355484c"},
+    {file = "PyYAML-6.0.1-cp39-cp39-win_amd64.whl", hash = "sha256:510c9deebc5c0225e8c96813043e62b680ba2f9c50a08d3724c7f28a747d1486"},
+    {file = "PyYAML-6.0.1.tar.gz", hash = "sha256:bfdf460b1736c775f2ba9f6a92bca30bc2095067b8a9d77876d1fad6cc3b4a43"},
 ]
 
 [[package]]
 name = "requests"
 version = "2.31.0"
 description = "Python HTTP for Humans."
 optional = false
@@ -1003,21 +1072,21 @@
 
 [package.extras]
 socks = ["PySocks (>=1.5.6,!=1.5.7)"]
 use-chardet-on-py3 = ["chardet (>=3.0.2,<6)"]
 
 [[package]]
 name = "rich"
-version = "13.4.2"
+version = "13.5.2"
 description = "Render rich text, tables, progress bars, syntax highlighting, markdown and more to the terminal"
 optional = false
 python-versions = ">=3.7.0"
 files = [
-    {file = "rich-13.4.2-py3-none-any.whl", hash = "sha256:8f87bc7ee54675732fa66a05ebfe489e27264caeeff3728c945d25971b6485ec"},
-    {file = "rich-13.4.2.tar.gz", hash = "sha256:d653d6bccede5844304c605d5aac802c7cf9621efd700b46c7ec2b51ea914898"},
+    {file = "rich-13.5.2-py3-none-any.whl", hash = "sha256:146a90b3b6b47cac4a73c12866a499e9817426423f57c5a66949c086191a8808"},
+    {file = "rich-13.5.2.tar.gz", hash = "sha256:fb9d6c0a0f643c99eed3875b5377a184132ba9be4d61516a55273d3554d75a39"},
 ]
 
 [package.dependencies]
 markdown-it-py = ">=2.2.0"
 pygments = ">=2.13.0,<3.0.0"
 
 [package.extras]
@@ -1040,36 +1109,36 @@
 [package.extras]
 dev = ["build (>=0.7.0)", "pre-commit (>=2.20.0)", "pytest (>=7.0.1)", "pytest-timeout (>=2.1.0)"]
 doc = ["pytoolconfig[doc]", "sphinx (>=4.5.0)", "sphinx-autodoc-typehints (>=1.18.1)", "sphinx-rtd-theme (>=1.0.0)"]
 release = ["pip-tools (>=6.12.1)", "toml (>=0.10.2)", "twine (>=4.0.2)"]
 
 [[package]]
 name = "ruff"
-version = "0.0.275"
+version = "0.0.280"
 description = "An extremely fast Python linter, written in Rust."
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "ruff-0.0.275-py3-none-macosx_10_7_x86_64.whl", hash = "sha256:5e6554a072e7ce81eb6f0bec1cebd3dcb0e358652c0f4900d7d630d61691e914"},
-    {file = "ruff-0.0.275-py3-none-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:1cc599022fe5ffb143a965b8d659eb64161ab8ab4433d208777eab018a1aab67"},
-    {file = "ruff-0.0.275-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:5206fc1cd8c1c1deadd2e6360c0dbcd690f1c845da588ca9d32e4a764a402c60"},
-    {file = "ruff-0.0.275-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:0c4e6468da26f77b90cae35319d310999f471a8c352998e9b39937a23750149e"},
-    {file = "ruff-0.0.275-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:0dbdea02942131dbc15dd45f431d152224f15e1dd1859fcd0c0487b658f60f1a"},
-    {file = "ruff-0.0.275-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:22efd9f41af27ef8fb9779462c46c35c89134d33e326c889971e10b2eaf50c63"},
-    {file = "ruff-0.0.275-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:2c09662112cfa22d7467a19252a546291fd0eae4f423e52b75a7a2000a1894db"},
-    {file = "ruff-0.0.275-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:80043726662144876a381efaab88841c88e8df8baa69559f96b22d4fa216bef1"},
-    {file = "ruff-0.0.275-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5859ee543b01b7eb67835dfd505faa8bb7cc1550f0295c92c1401b45b42be399"},
-    {file = "ruff-0.0.275-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:c8ace4d40a57b5ea3c16555f25a6b16bc5d8b2779ae1912ce2633543d4e9b1da"},
-    {file = "ruff-0.0.275-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:8347fc16aa185aae275906c4ac5b770e00c896b6a0acd5ba521f158801911998"},
-    {file = "ruff-0.0.275-py3-none-musllinux_1_2_i686.whl", hash = "sha256:ec43658c64bfda44fd84bbea9da8c7a3b34f65448192d1c4dd63e9f4e7abfdd4"},
-    {file = "ruff-0.0.275-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:508b13f7ca37274cceaba4fb3ea5da6ca192356323d92acf39462337c33ad14e"},
-    {file = "ruff-0.0.275-py3-none-win32.whl", hash = "sha256:6afb1c4422f24f361e877937e2a44b3f8176774a476f5e33845ebfe887dd5ec2"},
-    {file = "ruff-0.0.275-py3-none-win_amd64.whl", hash = "sha256:d9b264d78621bf7b698b6755d4913ab52c19bd28bee1a16001f954d64c1a1220"},
-    {file = "ruff-0.0.275-py3-none-win_arm64.whl", hash = "sha256:a19ce3bea71023eee5f0f089dde4a4272d088d5ac0b675867e074983238ccc65"},
-    {file = "ruff-0.0.275.tar.gz", hash = "sha256:a63a0b645da699ae5c758fce19188e901b3033ec54d862d93fcd042addf7f38d"},
+    {file = "ruff-0.0.280-py3-none-macosx_10_7_x86_64.whl", hash = "sha256:48ed5aca381050a4e2f6d232db912d2e4e98e61648b513c350990c351125aaec"},
+    {file = "ruff-0.0.280-py3-none-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:ef6ee3e429fd29d6a5ceed295809e376e6ece5b0f13c7e703efaf3d3bcb30b96"},
+    {file = "ruff-0.0.280-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d878370f7e9463ac40c253724229314ff6ebe4508cdb96cb536e1af4d5a9cd4f"},
+    {file = "ruff-0.0.280-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:83e8f372fa5627eeda5b83b5a9632d2f9c88fc6d78cead7e2a1f6fb05728d137"},
+    {file = "ruff-0.0.280-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:7008fc6ca1df18b21fa98bdcfc711dad5f94d0fc3c11791f65e460c48ef27c82"},
+    {file = "ruff-0.0.280-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:fe7118c1eae3fda17ceb409629c7f3b5a22dffa7caf1f6796776936dca1fe653"},
+    {file = "ruff-0.0.280-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:37359cd67d2af8e09110a546507c302cbea11c66a52d2a9b6d841d465f9962d4"},
+    {file = "ruff-0.0.280-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:bd58af46b0221efb95966f1f0f7576df711cb53e50d2fdb0e83c2f33360116a4"},
+    {file = "ruff-0.0.280-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2e7c15828d09f90e97bea8feefcd2907e8c8ce3a1f959c99f9b4b3469679f33c"},
+    {file = "ruff-0.0.280-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:2dae8f2d9c44c5c49af01733c2f7956f808db682a4193180dedb29dd718d7bbe"},
+    {file = "ruff-0.0.280-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:5f972567163a20fb8c2d6afc60c2ea5ef8b68d69505760a8bd0377de8984b4f6"},
+    {file = "ruff-0.0.280-py3-none-musllinux_1_2_i686.whl", hash = "sha256:8ffa7347ad11643f29de100977c055e47c988cd6d9f5f5ff83027600b11b9189"},
+    {file = "ruff-0.0.280-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:7a37dab70114671d273f203268f6c3366c035fe0c8056614069e90a65e614bfc"},
+    {file = "ruff-0.0.280-py3-none-win32.whl", hash = "sha256:7784e3606352fcfb193f3cd22b2e2117c444cb879ef6609ec69deabd662b0763"},
+    {file = "ruff-0.0.280-py3-none-win_amd64.whl", hash = "sha256:4a7d52457b5dfcd3ab24b0b38eefaead8e2dca62b4fbf10de4cd0938cf20ce30"},
+    {file = "ruff-0.0.280-py3-none-win_arm64.whl", hash = "sha256:b7de5b8689575918e130e4384ed9f539ce91d067c0a332aedef6ca7188adac2d"},
+    {file = "ruff-0.0.280.tar.gz", hash = "sha256:581c43e4ac5e5a7117ad7da2120d960a4a99e68ec4021ec3cd47fe1cf78f8380"},
 ]
 
 [[package]]
 name = "semver"
 version = "3.0.1"
 description = "Python helper for Semantic Versioning (https://semver.org)"
 optional = false
@@ -1121,21 +1190,21 @@
 files = [
     {file = "soupsieve-2.4.1-py3-none-any.whl", hash = "sha256:1c1bfee6819544a3447586c889157365a27e10d88cde3ad3da0cf0ddf646feb8"},
     {file = "soupsieve-2.4.1.tar.gz", hash = "sha256:89d12b2d5dfcd2c9e8c22326da9d9aa9cb3dfab0a83a024f05704076ee8d35ea"},
 ]
 
 [[package]]
 name = "sphinx"
-version = "7.0.1"
+version = "7.1.2"
 description = "Python documentation generator"
 optional = false
 python-versions = ">=3.8"
 files = [
-    {file = "Sphinx-7.0.1.tar.gz", hash = "sha256:61e025f788c5977d9412587e733733a289e2b9fdc2fef8868ddfbfc4ccfe881d"},
-    {file = "sphinx-7.0.1-py3-none-any.whl", hash = "sha256:60c5e04756c1709a98845ed27a2eed7a556af3993afb66e77fec48189f742616"},
+    {file = "sphinx-7.1.2-py3-none-any.whl", hash = "sha256:d170a81825b2fcacb6dfd5a0d7f578a053e45d3f2b153fecc948c37344eb4cbe"},
+    {file = "sphinx-7.1.2.tar.gz", hash = "sha256:780f4d32f1d7d1126576e0e5ecc19dc32ab76cd24e950228dcf7b1f6d3d9e22f"},
 ]
 
 [package.dependencies]
 alabaster = ">=0.7,<0.8"
 babel = ">=2.9"
 colorama = {version = ">=0.4.5", markers = "sys_platform == \"win32\""}
 docutils = ">=0.18.1,<0.21"
@@ -1175,21 +1244,21 @@
 sphinx = "*"
 
 [package.extras]
 test = ["pytest", "pytest-cov"]
 
 [[package]]
 name = "sphinx-basic-ng"
-version = "1.0.0b1"
+version = "1.0.0b2"
 description = "A modern skeleton for Sphinx themes."
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "sphinx_basic_ng-1.0.0b1-py3-none-any.whl", hash = "sha256:ade597a3029c7865b24ad0eda88318766bcc2f9f4cef60df7e28126fde94db2a"},
-    {file = "sphinx_basic_ng-1.0.0b1.tar.gz", hash = "sha256:89374bd3ccd9452a301786781e28c8718e99960f2d4f411845ea75fc7bb5a9b0"},
+    {file = "sphinx_basic_ng-1.0.0b2-py3-none-any.whl", hash = "sha256:eb09aedbabfb650607e9b4b68c9d240b90b1e1be221d6ad71d61c52e29f7932b"},
+    {file = "sphinx_basic_ng-1.0.0b2.tar.gz", hash = "sha256:9ec55a47c90c8c002b5960c57492ec3021f5193cb26cebc2dc4ea226848651c9"},
 ]
 
 [package.dependencies]
 sphinx = ">=4.0"
 
 [package.extras]
 docs = ["furo", "ipython", "myst-parser", "sphinx-copybutton", "sphinx-inline-tabs"]
@@ -1292,21 +1361,21 @@
 files = [
     {file = "tomli-2.0.1-py3-none-any.whl", hash = "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc"},
     {file = "tomli-2.0.1.tar.gz", hash = "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"},
 ]
 
 [[package]]
 name = "tomlkit"
-version = "0.11.8"
+version = "0.12.1"
 description = "Style preserving TOML library"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "tomlkit-0.11.8-py3-none-any.whl", hash = "sha256:8c726c4c202bdb148667835f68d68780b9a003a9ec34167b6c673b38eff2a171"},
-    {file = "tomlkit-0.11.8.tar.gz", hash = "sha256:9330fc7faa1db67b541b28e62018c17d20be733177d290a13b24c62d1614e0c3"},
+    {file = "tomlkit-0.12.1-py3-none-any.whl", hash = "sha256:712cbd236609acc6a3e2e97253dfc52d4c2082982a88f61b640ecf0817eab899"},
+    {file = "tomlkit-0.12.1.tar.gz", hash = "sha256:38e1ff8edb991273ec9f6181244a6a391ac30e9f5098e7535640ea6be97a7c86"},
 ]
 
 [[package]]
 name = "tornado"
 version = "6.3.2"
 description = "Tornado is a Python web framework and asynchronous networking library, originally developed at FriendFeed."
 optional = false
@@ -1334,41 +1403,41 @@
 files = [
     {file = "typing_extensions-4.7.1-py3-none-any.whl", hash = "sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36"},
     {file = "typing_extensions-4.7.1.tar.gz", hash = "sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2"},
 ]
 
 [[package]]
 name = "urllib3"
-version = "2.0.3"
+version = "2.0.4"
 description = "HTTP library with thread-safe connection pooling, file post, and more."
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "urllib3-2.0.3-py3-none-any.whl", hash = "sha256:48e7fafa40319d358848e1bc6809b208340fafe2096f1725d05d67443d0483d1"},
-    {file = "urllib3-2.0.3.tar.gz", hash = "sha256:bee28b5e56addb8226c96f7f13ac28cb4c301dd5ea8a6ca179c0b9835e032825"},
+    {file = "urllib3-2.0.4-py3-none-any.whl", hash = "sha256:de7df1803967d2c2a98e4b11bb7d6bd9210474c46e8a0401514e3a42a75ebde4"},
+    {file = "urllib3-2.0.4.tar.gz", hash = "sha256:8d22f86aae8ef5e410d4f539fde9ce6b2113a001bb4d189e0aed70642d602b11"},
 ]
 
 [package.extras]
 brotli = ["brotli (>=1.0.9)", "brotlicffi (>=0.8.0)"]
 secure = ["certifi", "cryptography (>=1.9)", "idna (>=2.0.0)", "pyopenssl (>=17.1.0)", "urllib3-secure-extra"]
 socks = ["pysocks (>=1.5.6,!=1.5.7,<2.0)"]
 zstd = ["zstandard (>=0.18.0)"]
 
 [[package]]
 name = "zipp"
-version = "3.15.0"
+version = "3.16.2"
 description = "Backport of pathlib-compatible object wrapper for zip files"
 optional = false
-python-versions = ">=3.7"
+python-versions = ">=3.8"
 files = [
-    {file = "zipp-3.15.0-py3-none-any.whl", hash = "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"},
-    {file = "zipp-3.15.0.tar.gz", hash = "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b"},
+    {file = "zipp-3.16.2-py3-none-any.whl", hash = "sha256:679e51dd4403591b2d6838a48de3d283f3d188412a9782faadf845f298736ba0"},
+    {file = "zipp-3.16.2.tar.gz", hash = "sha256:ebc15946aa78bd63458992fc81ec3b6f7b1e92d51c35e6de1c3804e73b799147"},
 ]
 
 [package.extras]
-docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
-testing = ["big-O", "flake8 (<5)", "jaraco.functools", "jaraco.itertools", "more-itertools", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)"]
+docs = ["furo", "jaraco.packaging (>=9.3)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
+testing = ["big-O", "jaraco.functools", "jaraco.itertools", "more-itertools", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=2.2)", "pytest-ignore-flaky", "pytest-mypy (>=0.9.1)", "pytest-ruff"]
 
 [metadata]
 lock-version = "2.0"
-python-versions = ">=3.9"
-content-hash = "101f72bf9997ae59442504beba598f808109ecb772fbd43a1fe2465bd5d6278e"
+python-versions = "^3.9"
+content-hash = "5747d995f1e8f40f2f881d59bf338fdd379a94bd44e036cfdde655cec61beadb"
```

### Comparing `pontos-23.7.7/pontos/__init__.py` & `pontos-23.8.0/pontos/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/changelog/__init__.py` & `pontos-23.8.0/pontos/changelog/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/changelog/conventional_commits.py` & `pontos-23.8.0/pontos/changelog/conventional_commits.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/changelog/errors.py` & `pontos-23.8.0/pontos/changelog/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/changelog/main.py` & `pontos-23.8.0/pontos/changelog/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,31 +12,31 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import sys
-from argparse import ArgumentParser
+from argparse import ArgumentParser, Namespace
 from pathlib import Path
-from typing import Iterable, NoReturn
+from typing import NoReturn, Optional, Sequence
 
 from pontos.changelog.conventional_commits import ChangelogBuilder
 from pontos.errors import PontosError
 from pontos.terminal.null import NullTerminal
 from pontos.terminal.rich import RichTerminal
 from pontos.version.helper import get_last_release_version
 from pontos.version.schemes import (
     VERSIONING_SCHEMES,
     VersioningScheme,
     versioning_scheme_argument_type,
 )
 
 
-def parse_args(args: Iterable[str] = None) -> ArgumentParser:
+def parse_args(args: Optional[Sequence[str]] = None) -> Namespace:
     parser = ArgumentParser(
         description="Conventional commits utility.",
         prog="pontos-changelog",
     )
 
     parser.add_argument(
         "--config",
@@ -106,18 +106,18 @@
     next_version = getattr(parsed_args, "next_version", None)
     if next_version:
         parsed_args.next_version = scheme.parse_version(next_version)
 
     return parsed_args
 
 
-def main(args: Iterable[str] = None) -> NoReturn:
+def main(args: Optional[Sequence[str]] = None) -> NoReturn:
     parsed_args = parse_args(args)
 
-    term = NullTerminal if parsed_args.quiet else RichTerminal()
+    term = NullTerminal() if parsed_args.quiet else RichTerminal()
 
     if parsed_args.current_version:
         last_version = parsed_args.current_version
     else:
         last_version = get_last_release_version(
             parsed_args.versioning_scheme.parse_version,
             git_tag_prefix=parsed_args.git_tag_prefix,
```

### Comparing `pontos-23.7.7/pontos/errors.py` & `pontos-23.8.0/pontos/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/git/__init__.py` & `pontos-23.8.0/pontos/git/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/git/git.py` & `pontos-23.8.0/pontos/git/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import subprocess
 from enum import Enum
 from os import PathLike, fspath
 from pathlib import Path
-from typing import Iterable, Iterator, List, Optional, Union
+from typing import Collection, Iterable, Iterator, List, Optional, Union
 
 from pontos.errors import PontosError
 from pontos.git.status import StatusEntry, parse_git_status
 
 DEFAULT_TAG_SORT_SUFFIX = [
     "-alpha",
     "a",
@@ -378,82 +378,94 @@
             args = ["tag", "-l"]
 
         if tag_name:
             args.append(tag_name)
 
         return self.exec(*args).splitlines()
 
-    def add(self, files: Union[PathLike, List[PathLike]]) -> None:
+    def add(
+        self,
+        files: Union[str, PathLike[str], list[Union[PathLike[str], str]]],
+    ) -> None:
         """
         Add files to the git staging area
 
         Args:
             files: A single file or a list of files to add to the staging area
         """
-        if isinstance(files, (PathLike, str, bytes)):
+        if isinstance(files, (PathLike, str)):
             files = [files]
 
         args = ["add"]
         args.extend([fspath(file) for file in files])
 
         self.exec(*args)
 
     def commit(
         self,
         message: str,
         *,
         verify: Optional[bool] = None,
+        gpg_sign: Optional[bool] = None,
         gpg_signing_key: Optional[str] = None,
     ) -> None:
         """
         Create a new commit
 
         Args:
             message: Message of the commit
             verify: Set to False to skip git hooks
+            gpg_sign: Set to False to skip signing the commit via GPG
             gpg_signing_key: GPG Key ID to use to sign the commit
         """
         args = ["commit"]
         if verify is False:
             args.append("--no-verify")
         if gpg_signing_key:
             args.append(f"-S{gpg_signing_key}")
+        if gpg_sign is False:
+            args.append("--no-gpg-sign")
 
         args.extend(["-m", message])
 
         self.exec(*args)
 
     def tag(
         self,
         tag: str,
         *,
         gpg_key_id: Optional[str] = None,
         message: Optional[str] = None,
         force: Optional[bool] = False,
+        sign: Optional[bool] = None,
     ) -> None:
         """
         Create a Tag
 
         Args:
             tag: Tag name to create.
             gpg_key_id: GPG Key to sign the tag.
             message: Use message to annotate the given tag.
             force: True to replace an existing tag.
+            sign: Set to False to deactivate signing of the tag.
         """
         args = ["tag"]
 
         if gpg_key_id:
             args.extend(["-u", gpg_key_id])
 
         if message:
             args.extend(["-m", message])
 
         if force:
             args.append("--force")
 
+        if sign is False:
+            args.append("--no-sign")
+
         args.append(tag)
 
         self.exec(*args)
 
     def fetch(
         self,
         remote: Optional[str] = None,
@@ -553,15 +565,15 @@
 
     def show(
         self,
         *show_args: str,
         format: Optional[str] = None,
         oneline: Optional[bool] = None,
         patch: Optional[bool] = None,
-        objects: Union[str, Iterable[str], None] = None,
+        objects: Union[str, Collection[str], None] = None,
     ) -> Union[str, list[str]]:
         """
         Show various types of git objects
 
         Args:
             format: Pretty format the output.
             oneline: Print the abbreviated commit id and commit message in one
@@ -645,21 +657,21 @@
         args.extend(commit)
         return self.exec(*args).splitlines()
 
     def move(self, old: PathLike, new: PathLike) -> None:
         """
         Move a file from old to new
         """
-        return self.exec("mv", fspath(old), fspath(new))
+        self.exec("mv", fspath(old), fspath(new))
 
     def remove(self, to_remove: PathLike) -> None:
         """
         Remove a file from git
         """
-        return self.exec("rm", fspath(to_remove))
+        self.exec("rm", fspath(to_remove))
 
     def status(
         self,
         files: Optional[Iterable[PathLike]] = None,
     ) -> Iterator[StatusEntry]:
         """Get information about the current git status.
```

### Comparing `pontos-23.7.7/pontos/git/status.py` & `pontos-23.8.0/pontos/git/status.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/__init__.py` & `pontos-23.8.0/pontos/github/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/actions/__init__.py` & `pontos-23.8.0/pontos/github/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/actions/argparser.py` & `pontos-23.8.0/pontos/github/actions/argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/actions/cmds.py` & `pontos-23.8.0/pontos/github/actions/cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/actions/core.py` & `pontos-23.8.0/pontos/github/actions/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import os
 from contextlib import contextmanager
 from io import TextIOWrapper
 from pathlib import Path
 from typing import Generator, Optional
 
 from pontos.github.actions.errors import GitHubActionsError
+from pontos.typing import SupportsStr
 
 
 def _to_options(
     name: Optional[str] = None,
     line: Optional[str] = None,
     end_line: Optional[str] = None,
     column: Optional[str] = None,
@@ -200,15 +201,15 @@
         print(f"::debug::{message}")
 
 
 class ActionOutput:
     def __init__(self, file: TextIOWrapper) -> None:
         self._file = file
 
-    def write(self, name: str, value: str):
+    def write(self, name: str, value: SupportsStr):
         """
         Set action output
 
         An action output can be consumed by another job
 
         Args:
             name: Name of the output variable
@@ -240,15 +241,15 @@
                 "action output."
             )
 
         with Path(output_filename).open("a", encoding="utf8") as f:
             yield ActionOutput(f)
 
     @staticmethod
-    def output(name: str, value: str):
+    def output(name: str, value: SupportsStr):
         """
         Set action output
 
         An action output can be consumed by another job
 
         Args:
             name: Name of the output variable
@@ -261,18 +262,18 @@
                 "action output."
             )
 
         with Path(output_filename).open("a", encoding="utf8") as f:
             f.write(f"{name}={value}\n")
 
     @staticmethod
-    def input(name: str, default: Optional[str] = None) -> str:
+    def input(name: str, default: Optional[str] = None) -> Optional[str]:
         """
         Get the value of an action input
 
         Args:
             name: Name of the input variable
             default: Use as default if the is no value for the variable
         """
         return os.environ.get(
-            f"INPUT_{name.replace(' ', '_').upper()}", default  # type: ignore
+            f"INPUT_{name.replace(' ', '_').upper()}", default
         )
```

### Comparing `pontos-23.7.7/pontos/github/actions/env.py` & `pontos-23.8.0/pontos/github/actions/env.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/actions/errors.py` & `pontos-23.8.0/pontos/github/actions/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/actions/event.py` & `pontos-23.8.0/pontos/github/actions/event.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/actions/main.py` & `pontos-23.8.0/pontos/github/actions/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/api/__init__.py` & `pontos-23.8.0/pontos/github/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/api/api.py` & `pontos-23.8.0/pontos/github/api/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/api/artifacts.py` & `pontos-23.8.0/pontos/github/api/artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/api/branch.py` & `pontos-23.8.0/pontos/github/api/branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/api/client.py` & `pontos-23.8.0/pontos/github/api/client.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/api/contents.py` & `pontos-23.8.0/pontos/github/api/contents.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/api/errors.py` & `pontos-23.8.0/pontos/github/api/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/api/helper.py` & `pontos-23.8.0/pontos/github/api/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/api/labels.py` & `pontos-23.8.0/pontos/github/api/labels.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/api/organizations.py` & `pontos-23.8.0/pontos/github/api/organizations.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/api/pull_requests.py` & `pontos-23.8.0/pontos/github/api/pull_requests.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/api/release.py` & `pontos-23.8.0/pontos/github/api/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/api/repositories.py` & `pontos-23.8.0/pontos/github/api/repositories.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     MergeCommitMessage,
     MergeCommitTitle,
     Repository,
     SquashMergeCommitMessage,
     SquashMergeCommitTitle,
 )
 from pontos.helper import enum_or_value
+from pontos.typing import SupportsStr
 
 
 class GitHubAsyncRESTRepositories(GitHubAsyncREST):
     async def get(self, repo: str) -> Repository:
         """
         Get a repository
 
@@ -94,15 +95,15 @@
         homepage: Optional[str] = None,
         private: Optional[bool] = False,
         has_issues: Optional[bool] = True,
         has_projects: Optional[bool] = True,
         has_wiki: Optional[bool] = True,
         has_downloads: Optional[bool] = True,
         is_template: Optional[bool] = False,
-        team_id: Optional[str] = None,
+        team_id: Optional[SupportsStr] = None,
         auto_init: Optional[bool] = False,
         gitignore_template: Optional[Union[GitIgnoreTemplate, str]] = None,
         license_template: Optional[Union[LicenseType, str]] = None,
         allow_squash_merge: Optional[bool] = True,
         allow_merge_commit: Optional[bool] = True,
         allow_rebase_merge: Optional[bool] = True,
         allow_auto_merge: Optional[bool] = False,
@@ -237,15 +238,15 @@
         if has_projects is not None:
             data["has_projects"] = has_projects
         if has_wiki is not None:
             data["has_wiki"] = has_wiki
         if is_template is not None:
             data["is_template"] = is_template
         if team_id:
-            data["team_id"] = team_id
+            data["team_id"] = str(team_id)
         if has_downloads is not None:
             data["has_downloads"] = has_downloads
         if auto_init is not None:
             data["auto_init"] = auto_init
         if gitignore_template:
             data["gitignore_template"] = (
                 gitignore_template.value
```

### Comparing `pontos-23.7.7/pontos/github/api/search.py` & `pontos-23.8.0/pontos/github/api/search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/api/tags.py` & `pontos-23.8.0/pontos/github/api/tags.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/api/teams.py` & `pontos-23.8.0/pontos/github/api/teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/api/workflows.py` & `pontos-23.8.0/pontos/github/api/workflows.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/argparser.py` & `pontos-23.8.0/pontos/github/argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/cmds.py` & `pontos-23.8.0/pontos/github/cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/main.py` & `pontos-23.8.0/pontos/github/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/models/__init__.py` & `pontos-23.8.0/pontos/github/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/models/artifact.py` & `pontos-23.8.0/pontos/github/models/artifact.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/models/base.py` & `pontos-23.8.0/pontos/github/models/base.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/models/branch.py` & `pontos-23.8.0/pontos/github/models/branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/models/organization.py` & `pontos-23.8.0/pontos/github/models/organization.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/models/pull_request.py` & `pontos-23.8.0/pontos/github/models/pull_request.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/models/release.py` & `pontos-23.8.0/pontos/github/models/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/models/search.py` & `pontos-23.8.0/pontos/github/models/search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/models/tag.py` & `pontos-23.8.0/pontos/github/models/tag.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/models/workflow.py` & `pontos-23.8.0/pontos/github/models/workflow.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/pr_template.md` & `pontos-23.8.0/pontos/github/pr_template.md`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/script/__init__.py` & `pontos-23.8.0/pontos/github/script/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/script/errors.py` & `pontos-23.8.0/pontos/github/script/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/script/load.py` & `pontos-23.8.0/pontos/github/script/load.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/script/parser.py` & `pontos-23.8.0/pontos/github/script/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/scripts/artifacts-download.py` & `pontos-23.8.0/pontos/github/scripts/artifacts-download.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,7 +47,9 @@
             args.repository, args.artifact
         ) as download:
             async for content, progress in download:
                 rich_progress.advance(task_id, progress or 1)
                 f.write(content)
 
             rich_progress.update(task_id, total=1, completed=1)
+
+    return 0
```

### Comparing `pontos-23.7.7/pontos/github/scripts/artifacts.py` & `pontos-23.8.0/pontos/github/scripts/artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/scripts/branchprotection.py` & `pontos-23.8.0/pontos/github/scripts/branchprotection.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,16 +30,18 @@
     # draft script for updating the branch protections
     branch_protection = await api.branches.protection_rules(
         args.repo, args.branch
     )
     # switch required signatures enabled/disabled
     kwargs = update_from_applied_settings(
         branch_protection,
-        # pylint: disable=line-too-long
-        required_signatures=not branch_protection.required_signatures.enabled,
+        required_signatures=not (
+            branch_protection.required_signatures
+            and branch_protection.required_signatures.enabled
+        ),
     )
     await api.branches.update_protection_rules(
         args.repo,
         args.branch,
         **kwargs,
     )
     return 0
```

### Comparing `pontos-23.7.7/pontos/github/scripts/create-repository.py` & `pontos-23.8.0/pontos/github/scripts/create-repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from argparse import ArgumentParser, Namespace
 from typing import Union
 
 from pontos.git import Git, MergeStrategy
 from pontos.github.api import GitHubAsyncRESTApi
 from pontos.github.api.repositories import GitIgnoreTemplate, LicenseType
 from pontos.github.models.base import Permission
+from pontos.github.script.errors import GitHubScriptError
 from pontos.testing import temp_directory
 
 TEMPLATES = {
     "python": "https://github.com/greenbone/python-project-template.git",
     "go": "https://github.com/greenbone/go-project-template.git",
 }
 
@@ -132,14 +133,17 @@
             auto_init=True,
             gitignore_template=GITIGNORE.get(args.template),
             team_id=team_id,
         )
 
         repo_url = repo.ssh_url
 
+        if not repo_url:
+            raise GitHubScriptError("No ssh repository URL")
+
         git.add_remote("upstream", repo_url)
         git.fetch("upstream")
 
         if args.template:
             git.rebase("upstream/main", strategy=MergeStrategy.ORT_OURS)
         else:
             git.checkout("main", start_point="upstream/main")
@@ -166,7 +170,9 @@
             required_approving_review_count=1,
             required_conversation_resolution=True,
             dismiss_stale_reviews=True,
             allow_force_pushes=False,
             allow_deletions=False,
             restrictions_users=[],
         )
+
+    return 0
```

### Comparing `pontos-23.7.7/pontos/github/scripts/enforce-admins.py` & `pontos-23.8.0/pontos/github/scripts/enforce-admins.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/scripts/lock-branch.py` & `pontos-23.8.0/pontos/github/scripts/lock-branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/scripts/members.py` & `pontos-23.8.0/pontos/github/scripts/members.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/scripts/release-assets-download.py` & `pontos-23.8.0/pontos/github/scripts/release-assets-download.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,7 +57,9 @@
         )
         async with download_api(args.repository, args.tag) as download:
             async for content, progress in download:
                 rich_progress.advance(task_id, progress or 1)
                 f.write(content)
 
             rich_progress.update(task_id, total=1, completed=1)
+
+    return 0
```

### Comparing `pontos-23.7.7/pontos/github/scripts/repositories.py` & `pontos-23.8.0/pontos/github/scripts/repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/scripts/search-repositories.py` & `pontos-23.8.0/pontos/github/scripts/search-repositories.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,28 +19,29 @@
 This script search for repositories and prints out all found repositories
 """
 
 import csv
 import sys
 from abc import ABC, abstractmethod
 from argparse import ArgumentParser, ArgumentTypeError, Namespace
-from typing import Dict, Iterable, Union
+from typing import Collection, Optional, Union
 
 from rich.console import Console
 from rich.table import Table
 
 from pontos.github.api import GitHubAsyncRESTApi
 from pontos.github.models.search import (
     InDescriptionQualifier,
     InNameQualifier,
     InReadmeQualifier,
     InTopicsQualifier,
     IsPrivateQualifier,
     IsPublicQualifier,
     OrganizationQualifier,
+    Qualifier,
     RepositorySort,
     SortOrder,
     UserQualifier,
 )
 
 
 def lower(value: str) -> str:
@@ -133,47 +134,47 @@
         type=sort_type,
         help="Sort order. Choices: "
         f"{', '.join([o.name for o in RepositorySort])}.",
     )
 
 
 class Format(ABC):
-    def __init__(self, columns: Iterable[str]) -> None:
+    def __init__(self, columns: Collection[str]) -> None:
         self.columns = columns
 
     @abstractmethod
-    def add_row(self, **kwargs: Dict[str, str]) -> None:
+    def add_row(self, **kwargs: Optional[str]) -> None:
         pass
 
     def finish(self) -> None:
         pass
 
 
 class CSVFormat(Format):
-    def __init__(self, columns: Iterable[str]) -> None:
+    def __init__(self, columns: Collection[str]) -> None:
         super().__init__(columns)
         self.csv_writer = csv.DictWriter(sys.stdout, fieldnames=self.columns)
 
-    def add_row(self, **kwargs: Dict[str, str]) -> None:
+    def add_row(self, **kwargs: Optional[str]) -> None:
         row = {}
         for column in self.columns:
             row[column] = kwargs[column]
 
         self.csv_writer.writerow(row)
 
 
 class ConsoleFormat(Format):
-    def __init__(self, columns: Iterable[str]) -> None:
+    def __init__(self, columns: Collection[str]) -> None:
         super().__init__(columns)
         self.table = Table()
 
         for column in self.columns:
             self.table.add_column(column)
 
-    def add_row(self, **kwargs: Dict[str, str]) -> None:
+    def add_row(self, **kwargs: Optional[str]) -> None:
         row = []
         for column in self.columns:
             value = kwargs[column]
             if column == "url":
                 value = f"[link={value}]{value}[/link]"
 
             row.append(value)
@@ -184,19 +185,19 @@
         console = Console()
         console.print(self.table)
         console.print(f"{self.table.row_count} repositories.", highlight=False)
 
 
 async def github_script(api: GitHubAsyncRESTApi, args: Namespace) -> int:
     if args.format == "console":
-        output = ConsoleFormat(args.columns)
+        output: Format = ConsoleFormat(args.columns)
     else:
         output = CSVFormat(args.columns)
 
-    qualifiers = []
+    qualifiers: list[Qualifier] = []
 
     if args.public:
         qualifiers.append(IsPublicQualifier())
 
     if args.private:
         qualifiers.append(IsPrivateQualifier())
```

### Comparing `pontos-23.7.7/pontos/github/scripts/team-repositories.py` & `pontos-23.8.0/pontos/github/scripts/team-repositories.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 """
 This script adds team(s) to a list of repositories of an organization
 """
 
 import asyncio
 from argparse import ArgumentParser, FileType, Namespace
 from io import TextIOWrapper
-from typing import List, Set, Union
+from typing import Set, Union
 
 from httpx import HTTPStatusError
 
 from pontos.github.api import GitHubAsyncRESTApi
 from pontos.github.models.base import Permission
 
 
@@ -74,15 +74,15 @@
 
 
 async def github_script(api: GitHubAsyncRESTApi, args: Namespace) -> int:
     if args.file:
         file: TextIOWrapper = args.file
         repositories = [line.strip() for line in file.readlines()]
     else:
-        repositories: List[str] = args.repositories
+        repositories = args.repositories
 
     tasks = []
     for team in args.teams:
         for repo in repositories:
             tasks.append(
                 asyncio.create_task(
                     api.teams.add_permission(
```

### Comparing `pontos-23.7.7/pontos/github/scripts/teams.py` & `pontos-23.8.0/pontos/github/scripts/teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/github/scripts/workflow-runs.py` & `pontos-23.8.0/pontos/github/scripts/workflow-runs.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             run.name,
             str(run.id),
             f"[link={run.html_url}]{run.html_url}[/link]",
             run.head_branch,
             run.event.value,
             run.conclusion,
             str(run.updated_at),
-            run.actor.login,
+            run.actor.login if run.actor else "",
         )
         count += 1
 
     console = Console()
     console.print(table)
 
     print(f"{count} workflow runs.")
```

### Comparing `pontos-23.7.7/pontos/helper.py` & `pontos-23.8.0/pontos/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/models/__init__.py` & `pontos-23.8.0/pontos/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,25 +14,20 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from dataclasses import dataclass
 from datetime import date, datetime
 from inspect import isclass
-from typing import Any, Dict, Type, Union, get_type_hints
+from typing import Any, Dict, Type, Union, get_args, get_origin, get_type_hints
 
 from dateutil import parser as dateparser
 
 from pontos.errors import PontosError
 
-try:
-    from typing import get_args, get_origin
-except ImportError:
-    from typing_extensions import get_args, get_origin
-
 __all__ = (
     "Model",
     "ModelError",
     "dotted_attributes",
 )
```

### Comparing `pontos-23.7.7/pontos/nvd/__init__.py` & `pontos-23.8.0/pontos/nvd/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/nvd/api.py` & `pontos-23.8.0/pontos/nvd/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/nvd/cpe/__init__.py` & `pontos-23.8.0/pontos/nvd/cpe/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/nvd/cpe/api.py` & `pontos-23.8.0/pontos/nvd/cpe/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/nvd/cve/__init__.py` & `pontos-23.8.0/pontos/nvd/cve/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/nvd/cve/api.py` & `pontos-23.8.0/pontos/nvd/cve/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/nvd/models/__init__.py` & `pontos-23.8.0/pontos/nvd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/nvd/models/cpe.py` & `pontos-23.8.0/pontos/nvd/models/cpe.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/nvd/models/cve.py` & `pontos-23.8.0/pontos/nvd/models/cve.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/nvd/models/cvss_v2.py` & `pontos-23.8.0/pontos/nvd/models/cvss_v2.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/nvd/models/cvss_v3.py` & `pontos-23.8.0/pontos/nvd/models/cvss_v3.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/pontos.py` & `pontos-23.8.0/pontos/pontos.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/release/__init__.py` & `pontos-23.8.0/pontos/release/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from .create import CreateReleaseCommand, CreateReleaseReturnValue
 from .helper import ReleaseType, find_signing_key, get_git_repository_name
 from .main import main
-from .release import ReleaseCommand, ReleaseReturnValue
 from .sign import SignatureError, SignCommand, SignReturnValue
 
 __all__ = (
     "ReleaseType",
     "get_git_repository_name",
     "find_signing_key",
-    "ReleaseCommand",
-    "ReleaseReturnValue",
+    "CreateReleaseCommand",
+    "CreateReleaseReturnValue",
     "SignCommand",
     "SignatureError",
     "SignReturnValue",
     "main",
 )
```

### Comparing `pontos-23.7.7/pontos/release/main.py` & `pontos-23.8.0/pontos/release/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,56 +14,60 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 
+import logging
 import subprocess
 import sys
 from typing import NoReturn
 
 from pontos.git import GitError
 from pontos.release.parser import parse_args
 from pontos.terminal.null import NullTerminal
 from pontos.terminal.rich import RichTerminal
 
 
 def main(
     args=None,
 ) -> NoReturn:
     username, token, parsed_args = parse_args(args)
+    logging.basicConfig(format="%(levelname)s - %(name)s - %(message)s")
+
     if parsed_args.quiet:
         term = NullTerminal()
+        error_terminal = NullTerminal()
+        logging.disable()
     else:
-        term = RichTerminal()
-
-    term.bold_info(f"pontos-release => {parsed_args.func.__name__}")
+        term = RichTerminal()  # type: ignore[assignment]
+        error_terminal = RichTerminal(file=sys.stderr)  # type: ignore[assignment] # noqa: E501
 
-    with term.indent():
-        try:
-            retval = parsed_args.func(
-                term,
-                parsed_args,
-                username=username,
-                token=token,
-            )
-            sys.exit(int(retval))
-        except KeyboardInterrupt:
-            sys.exit(1)
-        except GitError as e:
-            term.error(f'Could not run git command "{e.cmd}".')
-            error = e.stderr if e.stderr else e.stdout
-            term.print(f"Output was: {error}")
-            sys.exit(1)
-        except subprocess.CalledProcessError as e:
-            if "--passphrase" not in e.cmd:
-                term.error(f'Could not run command "{e.cmd}".')
-            else:
-                term.error("Headless signing failed.")
+    try:
+        retval = parsed_args.func(
+            parsed_args,
+            terminal=term,
+            error_terminal=error_terminal,
+            username=username,
+            token=token,
+        )
+        sys.exit(int(retval))
+    except KeyboardInterrupt:
+        sys.exit(1)
+    except GitError as e:
+        error_terminal.error(f'Could not run git command "{e.cmd}".')
+        error = e.stderr if e.stderr else e.stdout
+        error_terminal.print(f"Output was: {error}")
+        sys.exit(1)
+    except subprocess.CalledProcessError as e:
+        if "--passphrase" not in e.cmd:
+            error_terminal.error(f'Could not run command "{e.cmd}".')
+        else:
+            error_terminal.error("Headless signing failed.")
 
-            term.print(f"Error was: {e.stderr}")
-            sys.exit(1)
+        error_terminal.print(f"Error was: {e.stderr}")
+        sys.exit(1)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pontos-23.7.7/pontos/release/parser.py` & `pontos-23.8.0/pontos/release/parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,30 +21,32 @@
     ArgumentParser,
     ArgumentTypeError,
     BooleanOptionalAction,
     Namespace,
 )
 from enum import Enum
 from pathlib import Path
-from typing import Callable, Tuple, Type
+from typing import Callable, Optional, Tuple, Type
 
 from pontos.release.helper import ReleaseType
+from pontos.release.show import OutputFormat, show
 from pontos.version.schemes import (
     VERSIONING_SCHEMES,
+    PEP440VersioningScheme,
     VersioningScheme,
     versioning_scheme_argument_type,
 )
 
-from .release import release
+from .create import create_release
 from .sign import sign
 
 DEFAULT_SIGNING_KEY = "0ED1E580"
 
 
-def to_choices(enum: Type[Enum]) -> list[str]:
+def to_choices(enum: Type[Enum]) -> str:
     return ", ".join([t.value for t in enum])
 
 
 def enum_type(enum: Type[Enum]) -> Callable[[str], Enum]:
     def convert(value: str) -> Enum:
         try:
             return enum(value)
@@ -60,15 +62,15 @@
     argparse._StoreAction
 ):  # pylint: disable=protected-access
     def __call__(self, parser, namespace, values, option_string=None):
         setattr(namespace, "release_type", ReleaseType.VERSION)
         setattr(namespace, self.dest, values)
 
 
-def parse_args(args) -> Tuple[str, str, Namespace]:
+def parse_args(args) -> Tuple[Optional[str], Optional[str], Namespace]:
     """
     Return user, token, parsed arguments
     """
     parser = ArgumentParser(
         description="Release handling utility.",
         prog="pontos-release",
     )
@@ -84,100 +86,104 @@
         title="subcommands",
         description="valid subcommands",
         help="additional help",
         dest="command",
         required=True,
     )
 
-    release_parser = subparsers.add_parser("release")
-    release_parser.set_defaults(func=release)
-    release_parser.add_argument(
+    create_parser = subparsers.add_parser(
+        "create", help="Create a new release", aliases=["release"]
+    )
+    create_parser.set_defaults(func=create_release)
+    create_parser.add_argument(
         "--versioning-scheme",
         help="Versioning scheme to use for parsing and handling version "
         f"information. Choices are {', '.join(VERSIONING_SCHEMES.keys())}. "
         "Default: %(default)s",
         default="pep440",
         type=versioning_scheme_argument_type,
     )
-    release_parser.add_argument(
+    create_parser.add_argument(
         "--release-type",
         help="Select the release type for calculating the release version. "
         f"Possible choices are: {to_choices(ReleaseType)}.",
         type=enum_type(ReleaseType),
     )
-    release_parser.add_argument(
+    create_parser.add_argument(
         "--release-version",
         help=(
             "Will release changelog as version. "
             "Default: lookup version in project definition."
         ),
         action=ReleaseVersionAction,
     )
-    release_parser.add_argument(
+    create_parser.add_argument(
         "--release-series",
         help="Create a release for a release series. Setting a release series "
         "is required if the latest tag version is newer then the to be "
         'released version. Examples: "1.2", "2", "22.4"',
     )
 
-    release_parser.add_argument(
+    create_parser.add_argument(
         "--next-version",
         help=(
             "Sets the next version in project definition "
             "after the release. Default: set to next dev version"
         ),
     )
 
-    release_parser.add_argument(
+    create_parser.add_argument(
         "--git-remote-name",
         help="The git remote name to push the commits and tag to",
     )
-    release_parser.add_argument(
+    create_parser.add_argument(
         "--git-tag-prefix",
         default="v",
         const="",
         nargs="?",
         help="Prefix for git tag versions. Default: %(default)s",
     )
-    release_parser.add_argument(
+    create_parser.add_argument(
         "--git-signing-key",
         help="The key to sign the commits and tag for a release",
         default=os.environ.get("GPG_SIGNING_KEY"),
     )
-    release_parser.add_argument(
+    create_parser.add_argument(
         "--project",
         help="The github project",
     )
-    release_parser.add_argument(
+    create_parser.add_argument(
         "--space",
         default="greenbone",
         help="User/Team name in github",
     )
-    release_parser.add_argument(
+    create_parser.add_argument(
         "--local",
         action="store_true",
         help="Only create release changes locally and do not upload them to a "
         "remote repository. Also do not create a GitHub release.",
     )
-    release_parser.add_argument(
+    create_parser.add_argument(
         "--conventional-commits-config",
         dest="cc_config",
         type=Path,
         help="Conventional commits config file (toml), including conventions."
         " If not set defaults are used.",
     )
-    release_parser.add_argument(
+    create_parser.add_argument(
         "--update-project",
         help="Update version in project files like pyproject.toml. By default "
         "project files are updated.",
         action=BooleanOptionalAction,
         default=True,
     )
 
-    sign_parser = subparsers.add_parser("sign")
+    sign_parser = subparsers.add_parser(
+        "sign", help="Create signatures for an existing release"
+    )
     sign_parser.set_defaults(func=sign)
     sign_parser.add_argument(
         "--signing-key",
         default=DEFAULT_SIGNING_KEY,
         help="The key to sign zip, tarballs of a release. Default %(default)s.",
     )
     sign_parser.add_argument(
@@ -221,19 +227,70 @@
             "Use gpg in a headless mode e.g. for "
             "the CI and use this passphrase for signing."
         ),
     )
     sign_parser.add_argument(
         "--dry-run", action="store_true", help="Do not upload signed files."
     )
+
+    show_parser = subparsers.add_parser(
+        "show",
+        help="Show release information about the current release version and "
+        "determine the next release version",
+    )
+    show_parser.set_defaults(func=show)
+    show_parser.add_argument(
+        "--versioning-scheme",
+        help="Versioning scheme to use for parsing and handling version "
+        f"information. Choices are {', '.join(VERSIONING_SCHEMES.keys())}. "
+        "Default: %(default)s",
+        default="pep440",
+        type=versioning_scheme_argument_type,
+    )
+    show_parser.add_argument(
+        "--release-type",
+        help="Select the release type for calculating the release version. "
+        f"Possible choices are: {to_choices(ReleaseType)}.",
+        type=enum_type(ReleaseType),
+    )
+    show_parser.add_argument(
+        "--release-version",
+        help=(
+            "Will release changelog as version. "
+            "Default: lookup version in project definition."
+        ),
+        action=ReleaseVersionAction,
+    )
+    show_parser.add_argument(
+        "--release-series",
+        help="Create a release for a release series. Setting a release series "
+        "is required if the latest tag version is newer then the to be "
+        'released version. Examples: "1.2", "2", "22.4"',
+    )
+    show_parser.add_argument(
+        "--git-tag-prefix",
+        default="v",
+        const="",
+        nargs="?",
+        help="Prefix for git tag versions. Default: %(default)s",
+    )
+    show_parser.add_argument(
+        "--output-format",
+        help="Print in the desired output format. "
+        f"Possible choices are: {to_choices(OutputFormat)}.",
+        type=enum_type(OutputFormat),
+    )
+
     parsed_args = parser.parse_args(args)
 
-    scheme: VersioningScheme = getattr(parsed_args, "versioning_scheme", None)
+    scheme: type[VersioningScheme] = getattr(
+        parsed_args, "versioning_scheme", PEP440VersioningScheme
+    )
 
-    if parsed_args.func in (release,):
+    if parsed_args.func in (create_release, show):
         # check for release-type
         if not getattr(parsed_args, "release_type", None):
             parser.error("--release-type is required.")
 
         if (
             getattr(parsed_args, "release_version", None)
             and parsed_args.release_type != ReleaseType.VERSION
```

### Comparing `pontos-23.7.7/pontos/release/release.py` & `pontos-23.8.0/pontos/release/create.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,35 +12,40 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 
-import asyncio
 from argparse import Namespace
 from dataclasses import dataclass
 from enum import IntEnum, auto
 from pathlib import Path
-from typing import Optional
+from typing import Optional, SupportsInt
 
 import httpx
 
 from pontos.changelog.conventional_commits import ChangelogBuilder
 from pontos.errors import PontosError
 from pontos.git import Git
 from pontos.github.actions.core import ActionIO
 from pontos.github.api import GitHubAsyncRESTApi
+from pontos.release.command import AsyncCommand
 from pontos.terminal import Terminal
-from pontos.version import Version, VersionCalculator, VersionError
+from pontos.version import Version, VersionError
 from pontos.version.helper import get_last_release_version
 from pontos.version.project import Project
 from pontos.version.schemes import VersioningScheme
 
-from .helper import ReleaseType, find_signing_key, get_git_repository_name
+from .helper import (
+    ReleaseType,
+    find_signing_key,
+    get_git_repository_name,
+    get_next_release_version,
+)
 
 
 @dataclass
 class ReleaseInformation:
     last_release_version: Optional[Version]
     release_version: Version
     git_release_tag: str
@@ -52,15 +57,15 @@
                 "last-release-version", self.last_release_version or ""
             )
             output.write("release-version", self.release_version)
             output.write("git-release-tag", self.git_release_tag)
             output.write("next-version", self.next_version)
 
 
-class ReleaseReturnValue(IntEnum):
+class CreateReleaseReturnValue(IntEnum):
     """
     Possible return values of ReleaseCommand
     """
 
     SUCCESS = 0
     PROJECT_SETTINGS_NOT_FOUND = auto()
     TOKEN_MISSING = auto()
@@ -68,73 +73,35 @@
     NO_RELEASE_VERSION = auto()
     ALREADY_TAKEN = auto()
     CREATE_RELEASE_ERROR = auto()
     UPDATE_VERSION_ERROR = auto()
     UPDATE_VERSION_AFTER_RELEASE_ERROR = auto()
 
 
-class ReleaseCommand:
+class CreateReleaseCommand(AsyncCommand):
     """
     A CLI command for creating a release
 
     Args:
         terminal: A Terminal for output
     """
 
-    def __init__(self, terminal: Terminal) -> None:
+    def __init__(self, *, terminal: Terminal, error_terminal: Terminal) -> None:
+        super().__init__(terminal=terminal, error_terminal=error_terminal)
         self.git = Git()
-        self.terminal = terminal
-
-    def _get_next_release_version(
-        self,
-        *,
-        last_release_version: Version,
-        calculator: VersionCalculator,
-        release_type: ReleaseType,
-        release_version: Optional[Version],
-    ) -> Version:
-        if release_type == ReleaseType.CALENDAR:
-            return calculator.next_calendar_version(last_release_version)
-
-        if release_type == ReleaseType.PATCH:
-            return calculator.next_patch_version(last_release_version)
-
-        if release_type == ReleaseType.MINOR:
-            return calculator.next_minor_version(last_release_version)
-
-        if release_type == ReleaseType.MAJOR:
-            return calculator.next_major_version(last_release_version)
-
-        if release_type == ReleaseType.ALPHA:
-            return calculator.next_alpha_version(last_release_version)
-
-        if release_type == ReleaseType.BETA:
-            return calculator.next_beta_version(last_release_version)
-
-        if release_type == ReleaseType.RELEASE_CANDIDATE:
-            return calculator.next_release_candidate_version(
-                last_release_version
-            )
-
-        if not release_version:
-            raise VersionError(
-                "No release version provided. Either use a different release "
-                "strategy or provide a release version."
-            )
-        return release_version
 
     def _has_tag(self, git_version: str) -> bool:
         git_tags = self.git.list_tags()
         return git_version in git_tags
 
     def _create_changelog(
         self,
         release_version: Version,
         last_release_version: Optional[Version],
-        cc_config: Path,
+        cc_config: Optional[Path],
     ) -> str:
         changelog_builder = ChangelogBuilder(
             space=self.space,
             project=self.project,
             config=cc_config,
             git_tag_prefix=self.git_tag_prefix,
         )
@@ -158,32 +125,32 @@
             repo,
             git_version,
             name=f"{self.project} {release_version}",
             body=release_text,
             prerelease=release_version.is_pre_release,
         )
 
-    async def run(
+    async def async_run(  # type: ignore[override]
         self,
         *,
         token: str,
         space: str,
-        project: Optional[str],
+        project_name: Optional[str],
         versioning_scheme: VersioningScheme,
         release_type: ReleaseType,
         release_version: Optional[Version],
-        next_version: Optional[str],
+        next_version: Optional[Version],
         git_signing_key: str,
         git_remote_name: Optional[str],
         git_tag_prefix: Optional[str],
         cc_config: Optional[Path],
         local: Optional[bool] = False,
         release_series: Optional[str] = None,
         update_project: bool = True,
-    ) -> ReleaseReturnValue:
+    ) -> CreateReleaseReturnValue:
         """
         Create a release
 
         Args:
             token: A token for creating a release on GitHub
             space: GitHub username or organization. Required for generating
                 links in the changelog.
@@ -214,15 +181,17 @@
         git_signing_key = (
             git_signing_key
             if git_signing_key is not None
             else find_signing_key(self.terminal)
         )
         self.git_tag_prefix = git_tag_prefix or ""
         self.project = (
-            project if project is not None else get_git_repository_name()
+            project_name
+            if project_name is not None
+            else get_git_repository_name()
         )
         self.space = space
 
         self.terminal.info(f"Using versioning scheme {versioning_scheme.name}")
 
         try:
             last_release_version = get_last_release_version(
@@ -230,73 +199,69 @@
                 git_tag_prefix=self.git_tag_prefix,
                 tag_name=f"{self.git_tag_prefix}{release_series}.*"
                 if release_series
                 else None,
             )
         except PontosError as e:
             last_release_version = None
-            self.terminal.warning(
-                f"Could not determine last release version. {e}"
-            )
+            self.print_warning(f"Could not determine last release version. {e}")
 
         if not last_release_version:
             if not release_version:
-                self.terminal.error("Unable to determine last release version.")
-                return ReleaseReturnValue.NO_LAST_RELEASE_VERSION
+                self.print_error("Unable to determine last release version.")
+                return CreateReleaseReturnValue.NO_LAST_RELEASE_VERSION
             else:
                 self.terminal.info(
                     f"Creating the initial release {release_version}"
                 )
 
         else:
             self.terminal.info(f"Last release was {last_release_version}")
 
         calculator = versioning_scheme.calculator()
 
         try:
-            release_version = self._get_next_release_version(
+            release_version = get_next_release_version(
                 last_release_version=last_release_version,
                 calculator=calculator,
                 release_type=release_type,
                 release_version=release_version,
             )
         except VersionError as e:
-            self.terminal.error(f"Unable to determine release version. {e}")
-            return ReleaseReturnValue.NO_RELEASE_VERSION
+            self.print_error(f"Unable to determine release version. {e}")
+            return CreateReleaseReturnValue.NO_RELEASE_VERSION
 
         self.terminal.info(f"Preparing the release {release_version}")
 
         git_version = f"{self.git_tag_prefix}{release_version}"
 
         if self._has_tag(git_version):
-            self.terminal.error(f"Git tag {git_version} already exists.")
-            return ReleaseReturnValue.ALREADY_TAKEN
+            self.print_error(f"Git tag {git_version} already exists.")
+            return CreateReleaseReturnValue.ALREADY_TAKEN
 
         if update_project:
             try:
                 project = Project(versioning_scheme)
             except PontosError as e:
-                self.terminal.error(
-                    f"Unable to determine project settings. {e}"
-                )
-                return ReleaseReturnValue.PROJECT_SETTINGS_NOT_FOUND
+                self.print_error(f"Unable to determine project settings. {e}")
+                return CreateReleaseReturnValue.PROJECT_SETTINGS_NOT_FOUND
 
             try:
                 updated = project.update_version(release_version)
 
                 self.terminal.ok(f"Updated version to {release_version}")
 
                 for path in updated.changed_files:
                     self.terminal.info(f"Adding changes of {path}")
                     self.git.add(path)
             except VersionError as e:
                 self.terminal.error(
                     f"Unable to update version to {release_version}. {e}"
                 )
-                return ReleaseReturnValue.UPDATE_VERSION_ERROR
+                return CreateReleaseReturnValue.UPDATE_VERSION_ERROR
 
         if last_release_version:
             self.terminal.info(
                 f"Creating changelog for {release_version} since "
                 f"{last_release_version}"
             )
         else:
@@ -331,31 +296,33 @@
             try:
                 self.terminal.info(f"Creating release for {release_version}")
 
                 await self._create_release(release_version, token, release_text)
 
                 self.terminal.ok(f"Created release {release_version}")
             except httpx.HTTPStatusError as e:
-                self.terminal.error(str(e))
-                return ReleaseReturnValue.CREATE_RELEASE_ERROR
+                self.print_error(str(e))
+                return CreateReleaseReturnValue.CREATE_RELEASE_ERROR
 
         if not next_version:
             next_version = calculator.next_dev_version(release_version)
 
         if update_project:
             try:
                 updated = project.update_version(next_version)
                 self.terminal.ok(
                     f"Updated version after release to {next_version}"
                 )
             except VersionError as e:
-                self.terminal.error(
+                self.print_error(
                     f"Error while updating version after release. {e}"
                 )
-                return ReleaseReturnValue.UPDATE_VERSION_AFTER_RELEASE_ERROR
+                return (
+                    CreateReleaseReturnValue.UPDATE_VERSION_AFTER_RELEASE_ERROR
+                )
 
             for f in updated.changed_files:
                 self.terminal.info(f"Adding changes of {f}")
                 self.git.add(f)
 
         # check if files have been modified and create a commit
         status = list(self.git.status())
@@ -379,43 +346,43 @@
             release_version=release_version,
             git_release_tag=git_version,
             next_version=next_version,
         )
         if ActionIO.has_output():
             self.release_information.write_github_output()
 
-        return ReleaseReturnValue.SUCCESS
+        return CreateReleaseReturnValue.SUCCESS
 
 
-def release(
-    terminal: Terminal,
+def create_release(
     args: Namespace,
     *,
     token: str,
+    terminal: Terminal,
+    error_terminal: Terminal,
     **_kwargs,
-) -> IntEnum:
+) -> SupportsInt:
     if not token:
-        terminal.error(
+        error_terminal.error(
             "Token is missing. The GitHub token is required to create a "
             "release."
         )
-        return ReleaseReturnValue.TOKEN_MISSING
+        return CreateReleaseReturnValue.TOKEN_MISSING
 
-    cmd = ReleaseCommand(terminal)
-    return asyncio.run(
-        cmd.run(
-            token=token,
-            space=args.space,
-            project=args.project,
-            versioning_scheme=args.versioning_scheme,
-            release_type=args.release_type,
-            release_version=args.release_version,
-            next_version=args.next_version,
-            git_remote_name=args.git_remote_name,
-            git_signing_key=args.git_signing_key,
-            git_tag_prefix=args.git_tag_prefix,
-            cc_config=args.cc_config,
-            local=args.local,
-            release_series=args.release_series,
-            update_project=args.update_project,
-        )
+    return CreateReleaseCommand(
+        terminal=terminal, error_terminal=error_terminal
+    ).run(
+        token=token,
+        space=args.space,
+        project_name=args.project,
+        versioning_scheme=args.versioning_scheme,
+        release_type=args.release_type,
+        release_version=args.release_version,
+        next_version=args.next_version,
+        git_remote_name=args.git_remote_name,
+        git_signing_key=args.git_signing_key,
+        git_tag_prefix=args.git_tag_prefix,
+        cc_config=args.cc_config,
+        local=args.local,
+        release_series=args.release_series,
+        update_project=args.update_project,
     )
```

### Comparing `pontos-23.7.7/pontos/release/sign.py` & `pontos-23.8.0/pontos/release/sign.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,27 +18,28 @@
 
 import asyncio
 import hashlib
 import subprocess
 from argparse import Namespace
 from asyncio.subprocess import Process
 from enum import IntEnum
+from os import PathLike
 from pathlib import Path
-from typing import AsyncContextManager, Iterable, Optional
+from typing import AsyncContextManager, Optional, SupportsInt, Union
 
 import httpx
 from rich.progress import Progress as RichProgress
 from rich.progress import TextColumn
 
 from pontos.errors import PontosError
 from pontos.git.git import GitError
 from pontos.github.api import GitHubAsyncRESTApi
 from pontos.helper import AsyncDownloadProgressIterable
+from pontos.release.command import AsyncCommand
 from pontos.terminal import Terminal
-from pontos.terminal.rich import RichTerminal
 from pontos.version import Version
 from pontos.version.helper import get_last_release_version
 from pontos.version.schemes import VersioningScheme
 
 from .helper import get_git_repository_name
 
 
@@ -58,33 +59,30 @@
 
 class SignatureError(PontosError):
     """
     Error while creating a signature
     """
 
 
-async def cmd_runner(*args: Iterable[str]) -> Process:
+async def cmd_runner(*args: Union[str, PathLike[str]]) -> Process:
     return await asyncio.create_subprocess_exec(
         *args,
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
     )
 
 
-class SignCommand:
+class SignCommand(AsyncCommand):
     """
     A CLI command for signing a release
 
     Args:
         terminal: A Terminal for output
     """
 
-    def __init__(self, terminal: RichTerminal) -> None:
-        self.terminal = terminal
-
     async def _async_download_progress(
         self,
         rich_progress: RichProgress,
         progress: AsyncDownloadProgressIterable[bytes],
         destination: Path,
     ) -> None:
         with destination.open("wb") as f:
@@ -182,15 +180,15 @@
         _, stderr = await process.communicate()
         if process.returncode:
             raise SignatureError(
                 f"Could not create signature for {file_path}. "
                 f"{stderr.decode(errors='replace')}"
             )
 
-    async def run(
+    async def async_run(  # type: ignore[override]
         self,
         *,
         token: str,
         space: str,
         versioning_scheme: VersioningScheme,
         signing_key: str,
         passphrase: str,
@@ -220,28 +218,28 @@
             passphrase: Passphrase for the signing key
             release_series: Optional release series to use.
                 For example: "1.2", "2", "23".
         """
         if not token and not dry_run:
             # dry run doesn't upload assets. therefore a token MAY NOT be
             # required # for public repositories.
-            self.terminal.error(
+            self.print_error(
                 "Token is missing. The GitHub token is required to upload "
                 "signature files."
             )
             return SignReturnValue.TOKEN_MISSING
 
         self.terminal.info(f"Using versioning scheme {versioning_scheme.name}")
 
         try:
             project = (
                 project if project is not None else get_git_repository_name()
             )
         except GitError as e:
-            self.terminal.error(f"Could not determine project. {e}")
+            self.print_error(f"Could not determine project. {e}")
             return SignReturnValue.NO_PROJECT
 
         try:
             release_version = (
                 release_version
                 if release_version is not None
                 else get_last_release_version(
@@ -249,36 +247,39 @@
                     git_tag_prefix=git_tag_prefix,
                     tag_name=f"{git_tag_prefix}{release_series}.*"
                     if release_series
                     else None,
                 )
             )
         except PontosError as e:
-            self.terminal.error(f"Could not determine release version. {e}")
+            self.print_error(f"Could not determine release version. {e}")
             return SignReturnValue.NO_RELEASE_VERSION
 
         if not release_version:
             return SignReturnValue.NO_RELEASE_VERSION
 
         git_version: str = f"{git_tag_prefix}{release_version}"
         repo = f"{space}/{project}"
 
         async with GitHubAsyncRESTApi(token=token) as github:
             if not await github.releases.exists(repo, git_version):
-                self.terminal.error(
+                self.print_error(
                     f"Release version {git_version} does not exist."
                 )
                 return SignReturnValue.NO_RELEASE
 
             tasks = []
 
             zip_destination = Path(f"{project}-{release_version}.zip")
             tarball_destination = Path(f"{project}-{release_version}.tar.gz")
 
-            with self.terminal.progress(
+            # terminal can be a NullTerminal here too that doesn't have a
+            # progress. this needs to be fixed and the type ignore removed
+            # afterwards
+            with self.terminal.progress(  # type: ignore[attr-defined]
                 additional_columns=[
                     TextColumn("[progress.description]{task.fields[sha256]}"),
                 ]
             ) as rich_progress:
                 tasks.append(
                     asyncio.create_task(
                         self.download_zip(
@@ -331,15 +332,15 @@
             has_error = False
             for task in done:
                 try:
                     await task
                 except (asyncio.CancelledError, asyncio.InvalidStateError):
                     pass
                 except SignatureError as e:
-                    self.terminal.error(e)
+                    self.print_error(e)
                     has_error = True
 
             for task in pending:
                 # we had an error
                 try:
                     task.cancel()
                     await task
@@ -363,34 +364,33 @@
             try:
                 # pylint: disable=line-too-long
                 async for uploaded_file in github.releases.upload_release_assets(  # noqa: E501
                     repo, git_version, upload_files
                 ):
                     self.terminal.ok(f"Uploaded: {uploaded_file}")
             except httpx.HTTPStatusError as e:
-                self.terminal.error(f"Failed uploading asset {e}.")
+                self.print_error(f"Failed uploading asset {e}.")
                 return SignReturnValue.UPLOAD_ASSET_ERROR
 
         return SignReturnValue.SUCCESS
 
 
 def sign(
-    terminal: Terminal,
     args: Namespace,
     *,
+    terminal: Terminal,
+    error_terminal: Terminal,
     token: str,
     **_kwargs,
-) -> IntEnum:
-    return asyncio.run(
-        SignCommand(terminal).run(
-            token=token,
-            dry_run=args.dry_run,
-            project=args.project,
-            space=args.space,
-            versioning_scheme=args.versioning_scheme,
-            git_tag_prefix=args.git_tag_prefix,
-            release_version=args.release_version,
-            signing_key=args.signing_key,
-            passphrase=args.passphrase,
-            release_series=args.release_series,
-        )
+) -> SupportsInt:
+    return SignCommand(terminal=terminal, error_terminal=error_terminal).run(
+        token=token,
+        dry_run=args.dry_run,
+        project=args.project,
+        space=args.space,
+        versioning_scheme=args.versioning_scheme,
+        git_tag_prefix=args.git_tag_prefix,
+        release_version=args.release_version,
+        signing_key=args.signing_key,
+        passphrase=args.passphrase,
+        release_series=args.release_series,
     )
```

### Comparing `pontos-23.7.7/pontos/terminal/__init__.py` & `pontos-23.8.0/pontos/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/terminal/null.py` & `pontos-23.8.0/pontos/terminal/null.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/terminal/rich.py` & `pontos-23.8.0/pontos/terminal/rich.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-from typing import Any, Callable, Iterable, Optional
+from typing import IO, Any, Callable, Iterable, Optional
 
 from rich.console import Console, RenderableType
 from rich.padding import Padding
 from rich.progress import (
     BarColumn,
     Progress,
     ProgressColumn,
@@ -64,17 +64,27 @@
 
 
 class RichTerminal(Terminal):
     """
     A Terminal based on `rich <https://github.com/Textualize/rich/>`_.
     """
 
-    def __init__(self) -> None:
+    def __init__(
+        self,
+        file: Optional[IO[str]] = None,
+    ) -> None:
+        """
+        Create a new RichTerminal
+
+        Args:
+            file: A file object where the output should write to.
+                Default is stdout.
+        """
         super().__init__()
-        self._console = Console()
+        self._console = Console(file=file)
 
     def _indent_message(self):
         return " " * self._indent
 
     def _print_status(
         self,
         *messages: Any,
@@ -146,14 +156,14 @@
         with self.progress() as rich_progress:
             task_description = f"Downloading [blue]{progress.url}"
             if progress.length:
                 task_id = rich_progress.add_task(
                     task_description, total=progress.length
                 )
                 for percent in progress:
-                    rich_progress.advance(task_id, percent)
+                    rich_progress.advance(task_id, percent)  # type: ignore[arg-type] # noqa: E501
             else:
                 task_id = rich_progress.add_task(task_description, total=None)
                 for _ in progress:
                     rich_progress.advance(task_id)
 
             rich_progress.update(task_id, total=1, completed=1)
```

### Comparing `pontos-23.7.7/pontos/terminal/terminal.py` & `pontos-23.8.0/pontos/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/testing/__init__.py` & `pontos-23.8.0/pontos/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/typing/__init__.py` & `pontos-23.8.0/pontos/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/updateheader/__init__.py` & `pontos-23.8.0/pontos/updateheader/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/updateheader/__main__.py` & `pontos-23.8.0/pontos/updateheader/__main__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/updateheader/updateheader.py` & `pontos-23.8.0/pontos/updateheader/updateheader.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/version/__init__.py` & `pontos-23.8.0/pontos/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/version/__main__.py` & `pontos-23.8.0/pontos/version/__main__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/version/_calculator.py` & `pontos-23.8.0/pontos/version/_calculator.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/version/commands/__init__.py` & `pontos-23.8.0/pontos/version/commands/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     "JavaScriptVersionCommand",
     "JavaVersionCommand",
     "PythonVersionCommand",
     "CargoVersionCommand",
     "get_commands",
 )
 
-__COMMANDS: Tuple[Type[VersionCommand]] = (
+__COMMANDS: Tuple[Type[VersionCommand]] = (  # type: ignore[assignment]
     CMakeVersionCommand,
     GoVersionCommand,
     JavaVersionCommand,
     JavaScriptVersionCommand,
     PythonVersionCommand,
     CargoVersionCommand,
 )
```

### Comparing `pontos-23.7.7/pontos/version/commands/_cargo.py` & `pontos-23.8.0/pontos/version/commands/_cargo.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,27 +49,27 @@
             # just ignore current version and override it
             previous_version = None
 
         changed_files = []
         for project_path, project in self.__as_project_document(
             self.project_file_path
         ):
-            project["package"]["version"] = str(new_version)
+            project["package"]["version"] = str(new_version)  # type: ignore[index] # noqa: E501
             project_path.write_text(tomlkit.dumps(project))
             changed_files.append(project_path)
         return VersionUpdate(
             previous=previous_version,
             new=new_version,
             changed_files=changed_files,
         )
 
     def get_current_version(self) -> Version:
         (_, document) = next(self.__as_project_document(self.project_file_path))
         current_version = self.versioning_scheme.parse_version(
-            document["package"]["version"]
+            document["package"]["version"]  # type: ignore[index, arg-type]
         )
         return self.versioning_scheme.from_version(current_version)
 
     def verify_version(
         self, version: Union[Literal["current"], Version, None]
     ) -> None:
         current_version = self.get_current_version()
```

### Comparing `pontos-23.7.7/pontos/version/commands/_cmake.py` & `pontos-23.8.0/pontos/version/commands/_cmake.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,16 +117,18 @@
             )
             develop = True
         else:
             develop = False
 
         to_update = self._cmake_content_lines[self._version_line_number]
         updated = to_update.replace(self._current_version, str(new_version))
+
         self._cmake_content_lines[self._version_line_number] = updated
-        self._current_version = new_version
+        self._current_version = str(new_version)
+
         if self._project_dev_version_line_number:
             self._cmake_content_lines[
                 self._project_dev_version_line_number
             ] = self._cmake_content_lines[
                 self._project_dev_version_line_number
             ].replace(
                 str(int(not develop)), str(int(develop))
```

### Comparing `pontos-23.7.7/pontos/version/commands/_command.py` & `pontos-23.8.0/pontos/version/commands/_command.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/version/commands/_go.py` & `pontos-23.8.0/pontos/version/commands/_go.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/version/commands/_java.py` & `pontos-23.8.0/pontos/version/commands/_java.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+import logging
 import re
 from pathlib import Path
 from typing import Literal, Optional, Union
 
 from lxml import etree
 
 from ..errors import VersionError
@@ -33,25 +34,28 @@
 __version__ = "{}"\n"""
 
 
 def find_file(
     filename: Path, search_path: str, search_glob: str
 ) -> Optional[Path]:
     """Find a file somewhere within an directory tree
-    Arguments:
-        filename (Path)     The file to look up
-        search_path (str)   The path to look for the file
-        search_glob (str)   The glob search pattern
+
+    Arg:
+        filename: The file to look up
+        search_path: The path to look for the file
+        search_glob: The glob search pattern
 
     Returns:
-    The file as Path object, if existing"""
+        The file as Path object, if existing
+    """
     search_path = Path(search_path).resolve()
     for file_path in search_path.glob(search_glob):
         if file_path.is_file() and file_path.name == filename.name:
             return file_path
+    logging.warning("File %s not found in %s.", filename.name, search_path)
     return None
 
 
 def replace_string_in_file(
     file_path: Path, pattern: str, replacement: str
 ) -> None:
     # Read the content of the file
@@ -62,14 +66,19 @@
 
     # Replace the matched group (Group 1) with the replacement
     if match:
         # Write the updated content back to the file
         file_path.write_text(
             content.replace(match.group(1), replacement), encoding="utf-8"
         )
+    logging.warning(
+        "Couldn't match the pattern %s in the content of %s.",
+        pattern,
+        file_path,
+    )
 
 
 # This class is used for Java Version command(s)
 class JavaVersionCommand(VersionCommand):
     project_file_name = "pom.xml"
     _properties_file_path = Path("src/main/resources/application.properties")
     _pom_xml: Optional[etree.Element] = None
```

### Comparing `pontos-23.7.7/pontos/version/commands/_javascript.py` & `pontos-23.8.0/pontos/version/commands/_javascript.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/version/commands/_python.py` & `pontos-23.8.0/pontos/version/commands/_python.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,20 +43,20 @@
         """
         Return the version information from the [tool.poetry] section of the
         pyproject.toml file. The version may be in non standardized form.
         """
 
         if (
             "tool" in self.pyproject_toml
-            and "poetry" in self.pyproject_toml["tool"]  # type: ignore
-            and "version" in self.pyproject_toml["tool"]["poetry"]  # type: ignore # pylint: disable=line-too-long # noqa: E501
+            and "poetry" in self.pyproject_toml["tool"]  # type: ignore[operator] # noqa: E501
+            and "version" in self.pyproject_toml["tool"]["poetry"]  # type: ignore[operator,index] # noqa: E501
         ):
             return PEP440VersioningScheme.parse_version(
-                self.pyproject_toml["tool"]["poetry"]["version"]
-            )  # type: ignore
+                str(self.pyproject_toml["tool"]["poetry"]["version"])  # type: ignore[index] # noqa: E501
+            )
 
         raise VersionError(
             "Version information not found in "
             f"{self.project_file_path} file."
         )
 
     def _update_version_file(self, new_version: Version) -> None:
@@ -143,16 +143,21 @@
             version_module_name
         ]
         module_name = ".".join(module_parts)
         try:
             spec = importlib.util.spec_from_file_location(
                 module_name, self.version_file_path
             )
+            if not spec:
+                raise VersionError(
+                    f"Could not load version from '{module_name}'. "
+                )
+
             version_module = importlib.util.module_from_spec(spec)
-            spec.loader.exec_module(version_module)
+            spec.loader.exec_module(version_module)  # type: ignore[union-attr]
             return PEP440VersioningScheme.parse_version(
                 version_module.__version__
             )
         except FileNotFoundError:
             raise VersionError(
                 f"Could not load version from '{module_name}'. "
                 f"{self.version_file_path} not found."
```

### Comparing `pontos-23.7.7/pontos/version/errors.py` & `pontos-23.8.0/pontos/version/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/version/helper.py` & `pontos-23.8.0/pontos/version/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/version/main.py` & `pontos-23.8.0/pontos/version/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/version/parser.py` & `pontos-23.8.0/pontos/version/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/version/project.py` & `pontos-23.8.0/pontos/version/project.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/version/schemes/__init__.py` & `pontos-23.8.0/pontos/version/schemes/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,21 +26,21 @@
     "versioning_scheme_argument_type",
     "VersioningScheme",
     "PEP440VersioningScheme",
     "SemanticVersioningScheme",
 )
 
 #: Dictionary with available versioning schemes
-VERSIONING_SCHEMES = {
+VERSIONING_SCHEMES: dict[str, type[VersioningScheme]] = {
     "pep440": PEP440VersioningScheme,
     "semver": SemanticVersioningScheme,
 }
 
 
-def versioning_scheme_argument_type(value: str) -> VersioningScheme:
+def versioning_scheme_argument_type(value: str) -> type[VersioningScheme]:
     """
     Verifies if the passed value is a valid versioning scheme and returns
     the corresponding versioning scheme.
 
     Intended to be used as in `ArgumentParser.add_argument` as the type.
 
     Raises:
```

### Comparing `pontos-23.7.7/pontos/version/schemes/_pep440.py` & `pontos-23.8.0/pontos/version/schemes/_pep440.py`

 * *Files 11% similar despite different names*

```diff
@@ -107,25 +107,25 @@
     def is_dev_release(self) -> bool:
         """Whether this version is a development release."""
         return self._version.is_devrelease
 
     @property
     def is_alpha_release(self) -> bool:
         """Whether this version is a alpha release."""
-        return self.is_pre_release and self.pre and self.pre[0] == "alpha"
+        return bool(self.is_pre_release and self.pre and self.pre[0] == "alpha")
 
     @property
     def is_beta_release(self) -> bool:
         """Whether this version is a beta release."""
-        return self.is_pre_release and self.pre and self.pre[0] == "beta"
+        return bool(self.is_pre_release and self.pre and self.pre[0] == "beta")
 
     @property
     def is_release_candidate(self) -> bool:
         """Whether this version is a release candidate."""
-        return self.is_pre_release and self.pre and self.pre[0] == "rc"
+        return bool(self.is_pre_release and self.pre and self.pre[0] == "rc")
 
     @classmethod
     def from_string(cls, version: str) -> "PEP440Version":
         """
         Create a version from a version string
 
         Args:
@@ -178,15 +178,15 @@
                     f"{version.minor}."
                     f"{version.patch}"
                     f"-{version.pre[0]}{version.pre[1]}"
                     f".dev{version.dev}"
                 )
         elif version.is_pre_release:
             new_version = cls.from_string(
-                f"{version.major}."
+                f"{version.major}."  # type: ignore[index]
                 f"{version.minor}."
                 f"{version.patch}"
                 f"-{version.pre[0]}{version.pre[1]}"
                 f"{version_local}"
             )
         else:
             new_version = cls.from_string(str(version))
@@ -244,33 +244,33 @@
         Examples:
             "1.2.3" will return "1.2.4.dev1"
             "1.2.3.dev1" will return "1.2.3.dev2"
         """
         if current_version.is_dev_release:
             if current_version.pre:
                 return cls.version_from_string(
-                    f"{current_version.major}."
+                    f"{current_version.major}."  # type: ignore[operator]
                     f"{current_version.minor}."
                     f"{current_version.patch}"
                     f"-{current_version.pre[0]}{current_version.pre[1]}"
                     f".dev{current_version.dev + 1}"
                 )
             return cls.version_from_string(
-                f"{current_version.major}."
+                f"{current_version.major}."  # type: ignore[operator]
                 f"{current_version.minor}."
                 f"{current_version.patch}"
                 f".dev{current_version.dev + 1}"
             )
 
         if current_version.is_pre_release:
             return cls.version_from_string(
-                f"{current_version.major}."
+                f"{current_version.major}."  # type: ignore[index]
                 f"{current_version.minor}."
                 f"{current_version.patch}"
-                f"{current_version.pre[0]}{current_version.pre[1] + 1}.dev1"
+                f"{current_version.pre[0]}{current_version.pre[1] + 1}.dev1"  # type: ignore[index] # noqa: E501
             )
 
         return cls.version_from_string(
             f"{current_version.major}."
             f"{current_version.minor}."
             f"{current_version.patch + 1}.dev1"
         )
@@ -304,15 +304,15 @@
                 f"{current_version.patch}a1"
             )
 
         if current_version.is_alpha_release:
             return cls.version_from_string(
                 f"{current_version.major}."
                 f"{current_version.minor}."
-                f"{current_version.patch}a{current_version.pre[1] + 1}"
+                f"{current_version.patch}a{current_version.pre[1] + 1}"  # type: ignore[index] # noqa: E501
             )
 
         return cls.version_from_string(
             f"{current_version.major}."
             f"{current_version.minor}."
             f"{current_version.patch + 1}a1"
         )
@@ -348,15 +348,15 @@
             )
 
         if current_version.is_beta_release:
             return cls.version_from_string(
                 f"{current_version.major}."
                 f"{current_version.minor}."
                 f"{current_version.patch}"
-                f"b{current_version.pre[1] + 1}"
+                f"b{current_version.pre[1] + 1}"  # type: ignore[index]
             )
         return cls.version_from_string(
             f"{current_version.major}."
             f"{current_version.minor}."
             f"{current_version.patch + 1}b1"
         )
 
@@ -392,15 +392,15 @@
                 f"{current_version.patch}rc1"
             )
 
         if current_version.is_release_candidate:
             return cls.version_from_string(
                 f"{current_version.major}."
                 f"{current_version.minor}."
-                f"{current_version.patch}rc{current_version.pre[1] + 1}"
+                f"{current_version.patch}rc{current_version.pre[1] + 1}"  # type: ignore[index] # noqa: E501
             )
 
         return cls.version_from_string(
             f"{current_version.major}."
             f"{current_version.minor}."
             f"{current_version.patch + 1}rc1"
         )
```

### Comparing `pontos-23.7.7/pontos/version/schemes/_scheme.py` & `pontos-23.8.0/pontos/version/schemes/_scheme.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pontos/version/schemes/_semantic.py` & `pontos-23.8.0/pontos/version/schemes/_semantic.py`

 * *Files 10% similar despite different names*

```diff
@@ -116,25 +116,25 @@
     def is_dev_release(self) -> bool:
         """Whether this version is a development release."""
         return self._dev is not None
 
     @property
     def is_alpha_release(self) -> bool:
         """Whether this version is a alpha release."""
-        return self.is_pre_release and self.pre[0] == "alpha"
+        return self.is_pre_release and self.pre[0] == "alpha"  # type: ignore[index] # noqa: E501
 
     @property
     def is_beta_release(self) -> bool:
         """Whether this version is a beta release."""
-        return self.is_pre_release and self.pre[0] == "beta"
+        return self.is_pre_release and self.pre[0] == "beta"  # type: ignore[index] # noqa: E501
 
     @property
     def is_release_candidate(self) -> bool:
         """Whether this version is a release candidate."""
-        return self.is_pre_release and self.pre[0] == "rc"
+        return self.is_pre_release and self.pre[0] == "rc"  # type: ignore[index] # noqa: E501
 
     @property
     def major(self) -> int:
         """The first item of :attr:`release` or ``0`` if unavailable."""
         return self._version_info.major
 
     @property
@@ -181,42 +181,42 @@
 
     def __gt__(self, other: Any) -> bool:
         if not isinstance(other, Version):
             raise ValueError(f"Can't compare {type(self)} with {type(other)}")
         if not isinstance(other, type(self)):
             other = self.from_version(other)
 
-        if self._version_info.to_tuple()[:3] > other._version_info[:3]:
+        if self._version_info.to_tuple()[:3] > other._version_info[:3]:  # type: ignore[operator] # noqa: E501
             return True
-        if self._version_info.to_tuple()[:3] < other._version_info[:3]:
+        if self._version_info.to_tuple()[:3] < other._version_info[:3]:  # type: ignore[operator] # noqa: E501
             return False
 
         # major, minor and patch are equal
         if self.is_dev_release:
             if not other.is_pre_release and not other.is_dev_release:
                 return False
             if not self.is_pre_release and other.is_pre_release:
                 return False
             if not self.is_pre_release:
-                return self.dev > other.dev
+                return self.dev > other.dev  # type: ignore[operator]
 
             if self.is_pre_release:
                 if other.is_dev_release and self.pre == other.pre:
-                    return self.dev > other.dev
-                return self.pre > other.pre
+                    return self.dev > other.dev  # type: ignore[operator]
+                return self.pre > other.pre  # type: ignore[operator]
 
         # not a dev release
         if self.is_pre_release:
             if not other.is_pre_release and not other.is_dev_release:
                 return False
 
             if other.is_pre_release:
                 if other.is_dev_release:
-                    return self.pre >= other.pre
-                return self.pre > other.pre
+                    return self.pre >= other.pre  # type: ignore[operator]
+                return self.pre > other.pre  # type: ignore[operator]
 
             # other is a dev release
             return True
 
         if other.is_dev_release or other.is_pre_release:
             return True
 
@@ -285,28 +285,28 @@
                     f"-dev{version.dev}"
                 )
         elif version.is_alpha_release:
             new_version = cls.from_string(
                 f"{version.major}."
                 f"{version.minor}."
                 f"{version.patch}"
-                f"-alpha{version.pre[1]}"
+                f"-alpha{version.pre[1]}"  # type: ignore[index]
                 f"{version_local}"
             )
         elif version.is_beta_release:
             new_version = cls.from_string(
                 f"{version.major}."
                 f"{version.minor}."
                 f"{version.patch}"
-                f"-beta{version.pre[1]}"
+                f"-beta{version.pre[1]}"  # type: ignore[index]
                 f"{version_local}"
             )
         elif version.is_pre_release:
             new_version = cls.from_string(
-                f"{version.major}."
+                f"{version.major}."  # type: ignore[index]
                 f"{version.minor}."
                 f"{version.patch}"
                 f"-{version.pre[0]}{version.pre[1]}"
                 f"{version_local}"
             )
         else:
             new_version = cls.from_string(str(version))
@@ -323,33 +323,33 @@
     def next_dev_version(cls, current_version: Version) -> Version:
         """
         Get the next development version from a valid version
         """
         if current_version.is_dev_release:
             if current_version.pre:
                 return cls.version_from_string(
-                    f"{current_version.major}."
+                    f"{current_version.major}."  # type: ignore[operator]
                     f"{current_version.minor}."
                     f"{current_version.patch}"
                     f"-{current_version.pre[0]}{current_version.pre[1]}"
                     f"-dev{current_version.dev + 1}"
                 )
             return cls.version_from_string(
-                f"{current_version.major}."
+                f"{current_version.major}."  # type: ignore[operator]
                 f"{current_version.minor}."
                 f"{current_version.patch}"
                 f"-dev{current_version.dev + 1}"
             )
 
         if current_version.is_pre_release:
             return cls.version_from_string(
                 f"{current_version.major}."
                 f"{current_version.minor}."
                 f"{current_version.patch}-"
-                f"{current_version.pre[0]}{current_version.pre[1] + 1}-dev1"
+                f"{current_version.pre[0]}{current_version.pre[1] + 1}-dev1"  # type: ignore[index] # noqa: E501
             )
 
         return cls.version_from_string(
             f"{current_version.major}."
             f"{current_version.minor}."
             f"{current_version.patch + 1}"
             "-dev1"
@@ -380,15 +380,15 @@
                 f"{current_version.patch}-alpha1"
             )
         if current_version.is_alpha_release:
             return cls.version_from_string(
                 f"{current_version.major}."
                 f"{current_version.minor}."
                 f"{current_version.patch}"
-                f"-alpha{current_version.pre[1] + 1}"
+                f"-alpha{current_version.pre[1] + 1}"  # type: ignore[index]
             )
         return cls.version_from_string(
             f"{current_version.major}."
             f"{current_version.minor}."
             f"{current_version.patch + 1}"
             "-alpha1"
         )
@@ -420,15 +420,15 @@
                 "-beta1"
             )
         if current_version.is_beta_release:
             return cls.version_from_string(
                 f"{current_version.major}."
                 f"{current_version.minor}."
                 f"{current_version.patch}"
-                f"-beta{current_version.pre[1] + 1}"
+                f"-beta{current_version.pre[1] + 1}"  # type: ignore[index]
             )
         return cls.version_from_string(
             f"{current_version.major}."
             f"{current_version.minor}."
             f"{current_version.patch + 1}"
             "-beta1"
         )
@@ -460,15 +460,15 @@
                 f"{current_version.patch}-rc1"
             )
         if current_version.is_release_candidate:
             return cls.version_from_string(
                 f"{current_version.major}."
                 f"{current_version.minor}."
                 f"{current_version.patch}"
-                f"-rc{current_version.pre[1] + 1}"
+                f"-rc{current_version.pre[1] + 1}"  # type: ignore[index]
             )
         return cls.version_from_string(
             f"{current_version.major}."
             f"{current_version.minor}."
             f"{current_version.patch + 1}"
             "-rc1"
         )
```

### Comparing `pontos-23.7.7/pontos/version/version.py` & `pontos-23.8.0/pontos/version/version.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/pyproject.toml` & `pontos-23.8.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pontos"
-version = "23.7.7"
+version = "23.8.0"
 description = "Common utilities and tools maintained by Greenbone Networks"
 authors = ["Greenbone AG <info@greenbone.net>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/greenbone/pontos/"
 repository = "https://github.com/greenbone/pontos/"
 documentation = "https://greenbone.github.io/pontos/"
@@ -22,75 +22,83 @@
   "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 packages = [
   { include = "pontos"},
   { include = "tests", format = "sdist" },
   { include = "poetry.lock", format = "sdist" },
-  { include = "poetry.toml", format = "sdist" },
 ]
 include = [
   "pontos/updateheader/templates/",
   "pontos/github/pr_template.md"
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.9"
+python = "^3.9"
 colorful = ">=0.5.4"
 tomlkit = ">=0.5.11"
 packaging = ">=20.3"
-httpx = {extras = ["http2"], version = ">=0.23,<0.25"}
+httpx = {extras = ["http2"], version = ">=0.23"}
 rich = ">=12.4.4"
-typing-extensions = { version = "^4.4.0", python = "<3.8" }
 python-dateutil = ">=2.8.2"
 semver = ">=2.13"
 lxml = ">=4.9.0"
 
-[tool.poetry.dev-dependencies]
-autohooks = { version = ">=22.7.0", python = "^3.9" }
-autohooks-plugin-black = { version = ">=22.7.0", python = "^3.9" }
-autohooks-plugin-isort = { version = ">=22.3.0", python = "^3.9" }
-autohooks-plugin-ruff = { version = ">=23.6.1", python = "^3.9" }
+[tool.poetry.group.dev.dependencies]
+autohooks = ">=22.7.0"
+autohooks-plugin-black = ">=22.7.0"
+autohooks-plugin-isort = ">=22.3.0"
+autohooks-plugin-ruff = ">=23.6.1"
+autohooks-plugin-mypy = ">=23.3.0"
 rope = ">=1.9.0"
 coverage = ">=7.2"
 myst-parser = ">=0.19.1"
 Sphinx = ">=7.0.1"
 furo = ">=2023.5.20"
 sphinx-autobuild = ">=2021.3.14"
 
 [tool.black]
 line-length = 80
 target-version = ['py39', 'py310', 'py311']
 exclude = '''
 /(
     \.git
-  | \.hg
   | \.venv
-  | \.circleci
   | \.github
   | \.vscode
   | _build
   | build
   | dist
   | docs
 )/
 '''
 
 [tool.autohooks]
-pre-commit = ['autohooks.plugins.black', 'autohooks.plugins.isort', 'autohooks.plugins.ruff']
+pre-commit = ['autohooks.plugins.black', 'autohooks.plugins.isort', 'autohooks.plugins.ruff', 'autohooks.plugins.mypy']
 mode = "poetry"
 
 [tool.isort]
 profile = "black"
 line_length = 80
 
 [tool.ruff]
 line-length = 80
 target-version = "py39"
 
+[tool.mypy]
+files = "pontos"
+ignore_missing_imports = true
+explicit_package_bases = true
+allow_redefinition = true
+exclude = 'pontos/updateheader/templates/.*/*\.py'
+
+[[tool.mypy.overrides]]
+module = "dateutil"
+ignore_missing_imports = true
+
 [tool.pontos.version]
 version-module-file = "pontos/version/__version__.py"
 
 [tool.poetry.scripts]
 pontos = 'pontos:main'
 pontos-version = 'pontos.version:main'
 pontos-release = 'pontos.release:main'
```

### Comparing `pontos-23.7.7/tests/__init__.py` & `pontos-23.8.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/changelog/__init__.py` & `pontos-23.8.0/tests/changelog/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/changelog/test_conventional_commits.py` & `pontos-23.8.0/tests/changelog/test_conventional_commits.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/changelog/test_parser.py` & `pontos-23.8.0/tests/changelog/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/git/__init__.py` & `pontos-23.8.0/tests/git/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/git/test_git.py` & `pontos-23.8.0/tests/git/test_git.py`

 * *Files 1% similar despite different names*

```diff
@@ -391,14 +391,23 @@
         git.commit("Add foo", verify=False)
 
         exec_git_mock.assert_called_once_with(
             "commit", "--no-verify", "-m", "Add foo", cwd=None
         )
 
     @patch("pontos.git.git.exec_git")
+    def test_commit_without_gpg_sign(self, exec_git_mock):
+        git = Git()
+        git.commit("Add foo", gpg_sign=False)
+
+        exec_git_mock.assert_called_once_with(
+            "commit", "--no-gpg-sign", "-m", "Add foo", cwd=None
+        )
+
+    @patch("pontos.git.git.exec_git")
     def test_tag(self, exec_git_mock):
         git = Git()
         git.tag(tag="test")
 
         exec_git_mock.assert_called_once_with("tag", "test", cwd=None)
 
     @patch("pontos.git.git.exec_git")
@@ -425,14 +434,23 @@
         git.tag("test", force=True)
 
         exec_git_mock.assert_called_once_with(
             "tag", "--force", "test", cwd=None
         )
 
     @patch("pontos.git.git.exec_git")
+    def test_tag_without_sign(self, exec_git_mock):
+        git = Git()
+        git.tag("test", sign=False)
+
+        exec_git_mock.assert_called_once_with(
+            "tag", "--no-sign", "test", cwd=None
+        )
+
+    @patch("pontos.git.git.exec_git")
     def test_fetch(self, exec_git_mock):
         git = Git()
         git.fetch()
 
         exec_git_mock.assert_called_once_with("fetch", cwd=None)
 
     @patch("pontos.git.git.exec_git")
```

### Comparing `pontos-23.7.7/tests/git/test_status.py` & `pontos-23.8.0/tests/git/test_status.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/__init__.py` & `pontos-23.8.0/tests/github/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/actions/__init__.py` & `pontos-23.8.0/tests/github/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/actions/test-pull-request-event.json` & `pontos-23.8.0/tests/github/actions/test-pull-request-event.json`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/actions/test_core.py` & `pontos-23.8.0/tests/github/actions/test_core.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/actions/test_env.py` & `pontos-23.8.0/tests/github/actions/test_env.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/actions/test_event.py` & `pontos-23.8.0/tests/github/actions/test_event.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/api/__init__.py` & `pontos-23.8.0/tests/github/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/api/pr-files.json` & `pontos-23.8.0/tests/github/api/pr-files.json`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/api/release-response.json` & `pontos-23.8.0/tests/github/api/release-response.json`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/api/test_artifacts.py` & `pontos-23.8.0/tests/github/api/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/api/test_branch.py` & `pontos-23.8.0/tests/github/api/test_branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/api/test_client.py` & `pontos-23.8.0/tests/github/api/test_client.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/api/test_contents.py` & `pontos-23.8.0/tests/github/api/test_contents.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/api/test_labels.py` & `pontos-23.8.0/tests/github/api/test_labels.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/api/test_organizations.py` & `pontos-23.8.0/tests/github/api/test_organizations.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/api/test_pull_requests.py` & `pontos-23.8.0/tests/github/api/test_pull_requests.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/api/test_release.py` & `pontos-23.8.0/tests/github/api/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/api/test_repositories.py` & `pontos-23.8.0/tests/github/api/test_repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/api/test_search.py` & `pontos-23.8.0/tests/github/api/test_search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/api/test_tags.py` & `pontos-23.8.0/tests/github/api/test_tags.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/api/test_teams.py` & `pontos-23.8.0/tests/github/api/test_teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/api/test_workflows.py` & `pontos-23.8.0/tests/github/api/test_workflows.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/models/__init__.py` & `pontos-23.8.0/tests/github/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/models/test_artifact.py` & `pontos-23.8.0/tests/github/models/test_artifact.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/models/test_base.py` & `pontos-23.8.0/tests/github/models/test_base.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/models/test_branch.py` & `pontos-23.8.0/tests/github/models/test_branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/models/test_organization.py` & `pontos-23.8.0/tests/github/models/test_organization.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/models/test_pull_request.py` & `pontos-23.8.0/tests/github/models/test_pull_request.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/models/test_release.py` & `pontos-23.8.0/tests/github/models/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/models/test_search.py` & `pontos-23.8.0/tests/github/models/test_search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/models/test_tag.py` & `pontos-23.8.0/tests/github/models/test_tag.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/models/test_workflow.py` & `pontos-23.8.0/tests/github/models/test_workflow.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/script/__init__.py` & `pontos-23.8.0/tests/github/script/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/script/test_load.py` & `pontos-23.8.0/tests/github/script/test_load.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/script/test_parser.py` & `pontos-23.8.0/tests/github/script/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/test_argparser.py` & `pontos-23.8.0/tests/github/test_argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/github/test_cmds.py` & `pontos-23.8.0/tests/github/test_cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/models/__init__.py` & `pontos-23.8.0/tests/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/models/test_models.py` & `pontos-23.8.0/tests/models/test_models.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/nvd/__init__.py` & `pontos-23.8.0/tests/nvd/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/nvd/cpe/__init__.py` & `pontos-23.8.0/tests/nvd/cpe/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/nvd/cpe/test_api.py` & `pontos-23.8.0/tests/nvd/cpe/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/nvd/cve/__init__.py` & `pontos-23.8.0/tests/nvd/cve/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/nvd/cve/test_api.py` & `pontos-23.8.0/tests/nvd/cve/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/nvd/models/__init__.py` & `pontos-23.8.0/tests/nvd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/nvd/models/test_cpe.py` & `pontos-23.8.0/tests/nvd/models/test_cpe.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/nvd/models/test_cve.py` & `pontos-23.8.0/tests/nvd/models/test_cve.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/nvd/test_api.py` & `pontos-23.8.0/tests/nvd/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/release/__init__.py` & `pontos-23.8.0/tests/release/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/release/test_parser.py` & `pontos-23.8.0/tests/release/test_parser.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,19 +17,20 @@
 
 import unittest
 from contextlib import redirect_stderr
 from io import StringIO
 from pathlib import Path
 from unittest.mock import patch
 
+from pontos.release.create import create_release
 from pontos.release.helper import ReleaseType
 from pontos.release.parser import DEFAULT_SIGNING_KEY, parse_args
-from pontos.release.release import release
+from pontos.release.show import OutputFormat, show
 from pontos.release.sign import sign
-from pontos.version.schemes._pep440 import PEP440Version
+from pontos.version.schemes._pep440 import PEP440Version, PEP440VersioningScheme
 
 
 class ParseArgsTestCase(unittest.TestCase):
     def test_quiet(self):
         _, _, args = parse_args(["-q", "sign"])
         self.assertTrue(args.quiet)
 
@@ -47,15 +48,15 @@
         self.assertEqual(token, "foo")
 
 
 class ReleaseParseArgsTestCase(unittest.TestCase):
     def test_release_func(self):
         _, _, args = parse_args(["release", "--release-type", "patch"])
 
-        self.assertEqual(args.func, release)
+        self.assertEqual(args.func, create_release)
 
     def test_default(self):
         _, _, args = parse_args(["release", "--release-type", "patch"])
 
         self.assertEqual(args.git_tag_prefix, "v")
         self.assertEqual(args.space, "greenbone")
         self.assertFalse(args.local)
@@ -286,7 +287,134 @@
 
         self.assertEqual(args.passphrase, "123")
 
     def test_release_series(self):
         _, _, args = parse_args(["sign", "--release-series", "22.4"])
 
         self.assertEqual(args.release_series, "22.4")
+
+
+class ShowParseArgsTestCase(unittest.TestCase):
+    def test_show_func(self):
+        _, _, args = parse_args(["show", "--release-type", "patch"])
+
+        self.assertEqual(args.func, show)
+
+    def test_defaults(self):
+        _, _, args = parse_args(["show", "--release-type", "patch"])
+
+        self.assertEqual(args.git_tag_prefix, "v")
+        self.assertEqual(args.versioning_scheme, PEP440VersioningScheme)
+
+    def test_release_series(self):
+        _, _, args = parse_args(
+            ["show", "--release-type", "patch", "--release-series", "1.2"]
+        )
+
+        self.assertEqual(args.release_series, "1.2")
+
+    def test_release_type(self):
+        _, _, args = parse_args(["show", "--release-type", "patch"])
+
+        self.assertEqual(args.release_type, ReleaseType.PATCH)
+
+        _, _, args = parse_args(["show", "--release-type", "calendar"])
+
+        self.assertEqual(args.release_type, ReleaseType.CALENDAR)
+
+        _, _, args = parse_args(["show", "--release-type", "minor"])
+
+        self.assertEqual(args.release_type, ReleaseType.MINOR)
+
+        _, _, args = parse_args(["show", "--release-type", "major"])
+
+        self.assertEqual(args.release_type, ReleaseType.MAJOR)
+
+        _, _, args = parse_args(["show", "--release-type", "alpha"])
+
+        self.assertEqual(args.release_type, ReleaseType.ALPHA)
+
+        _, _, args = parse_args(["show", "--release-type", "beta"])
+
+        self.assertEqual(args.release_type, ReleaseType.BETA)
+
+        _, _, args = parse_args(["show", "--release-type", "release-candidate"])
+
+        self.assertEqual(args.release_type, ReleaseType.RELEASE_CANDIDATE)
+
+        with self.assertRaises(SystemExit), redirect_stderr(StringIO()):
+            parse_args(["show", "--release-type", "foo"])
+
+    def test_git_tag_prefix(self):
+        _, _, args = parse_args(
+            ["show", "--git-tag-prefix", "a", "--release-type", "patch"]
+        )
+
+        self.assertEqual(args.git_tag_prefix, "a")
+
+        _, _, args = parse_args(
+            ["show", "--git-tag-prefix", "", "--release-type", "patch"]
+        )
+
+        self.assertEqual(args.git_tag_prefix, "")
+
+        _, _, args = parse_args(
+            ["show", "--git-tag-prefix", "--release-type", "patch"]
+        )
+
+        self.assertEqual(args.git_tag_prefix, "")
+
+    def test_release_version(self):
+        _, _, args = parse_args(["show", "--release-version", "1.2.3"])
+
+        self.assertEqual(args.release_version, PEP440Version("1.2.3"))
+        self.assertEqual(args.release_type, ReleaseType.VERSION)
+
+        with self.assertRaises(SystemExit), redirect_stderr(StringIO()):
+            parse_args(
+                [
+                    "show",
+                    "--release-version",
+                    "1.2.3",
+                    "--release-type",
+                    "patch",
+                ]
+            )
+
+        with self.assertRaises(SystemExit), redirect_stderr(StringIO()):
+            parse_args(
+                [
+                    "show",
+                    "--release-version",
+                    "1.2.3",
+                    "--release-type",
+                    "calendar",
+                ]
+            )
+
+    def test_output_format(self):
+        _, _, args = parse_args(
+            ["show", "--release-type", "patch", "--output-format", "env"]
+        )
+
+        self.assertEqual(args.output_format, OutputFormat.ENV)
+
+        _, _, args = parse_args(
+            ["show", "--release-type", "patch", "--output-format", "json"]
+        )
+
+        self.assertEqual(args.output_format, OutputFormat.JSON)
+
+        _, _, args = parse_args(
+            [
+                "show",
+                "--release-type",
+                "patch",
+                "--output-format",
+                "github-action",
+            ]
+        )
+
+        with patch.dict(
+            "os.environ", {"GITHUB_OUTPUT": "/tmp/output"}, clear=True
+        ):
+            self.assertEqual(args.output_format, OutputFormat.GITHUB_ACTION)
```

### Comparing `pontos-23.7.7/tests/release/test_release.py` & `pontos-23.8.0/tests/release/test_create.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,20 +26,20 @@
 from unittest.mock import AsyncMock, MagicMock, call, patch
 
 from httpx import HTTPStatusError, Request, Response
 
 from pontos.git.git import ConfigScope, Git
 from pontos.git.status import StatusEntry
 from pontos.github.actions.errors import GitHubActionsError
-from pontos.release.main import parse_args
-from pontos.release.release import (
+from pontos.release.create import (
+    CreateReleaseReturnValue,
     ReleaseInformation,
-    ReleaseReturnValue,
-    release,
+    create_release,
 )
+from pontos.release.main import parse_args
 from pontos.terminal.terminal import Terminal
 from pontos.testing import temp_directory, temp_git_repository
 from pontos.version import VersionError, VersionUpdate
 from pontos.version.commands import GoVersionCommand
 from pontos.version.schemes._pep440 import PEP440Version, PEP440VersioningScheme
 
 
@@ -147,25 +147,26 @@
     "os.environ",
     {
         "GITHUB_TOKEN": "foo",
         "GITHUB_USER": "user",
         "GPG_SIGNING_KEY": "1234",
     },
 )
-class ReleaseTestCase(unittest.TestCase):
-    @patch("pontos.release.release.Git", autospec=True)
-    @patch("pontos.release.release.get_last_release_version", autospec=True)
+class CreateReleaseTestCase(unittest.TestCase):
+    @patch("pontos.release.create.Git", autospec=True)
+    @patch("pontos.release.create.get_last_release_version", autospec=True)
     @patch(
-        "pontos.release.release.ReleaseCommand._create_release", autospec=True
+        "pontos.release.create.CreateReleaseCommand._create_release",
+        autospec=True,
     )
     @patch(
-        "pontos.release.release.ReleaseCommand._create_changelog",
+        "pontos.release.create.CreateReleaseCommand._create_changelog",
         autospec=True,
     )
-    @patch("pontos.release.release.Project._gather_commands", autospec=True)
+    @patch("pontos.release.create.Project._gather_commands", autospec=True)
     def test_release_version(
         self,
         gather_commands_mock: MagicMock,
         create_changelog_mock: MagicMock,
         create_release_mock: AsyncMock,
         get_last_release_version_mock: MagicMock,
         git_mock: MagicMock,
@@ -203,16 +204,17 @@
                 "0.0.2",
                 "--next-version",
                 "1.0.0.dev1",
             ]
         )
 
         with temp_git_repository():
-            released = release(
+            released = create_release(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
         git_instance_mock.push.assert_has_calls(
             [
                 call(follow_tags=True, remote=None),
@@ -250,26 +252,27 @@
                 ),
             ]
         )
         git_instance_mock.tag.assert_called_once_with(
             "v0.0.2", gpg_key_id="1234", message="Automatic release to 0.0.2"
         )
 
-        self.assertEqual(released, ReleaseReturnValue.SUCCESS)
+        self.assertEqual(released, CreateReleaseReturnValue.SUCCESS)
 
-    @patch("pontos.release.release.Git", autospec=True)
-    @patch("pontos.release.release.get_last_release_version", autospec=True)
+    @patch("pontos.release.create.Git", autospec=True)
+    @patch("pontos.release.create.get_last_release_version", autospec=True)
     @patch(
-        "pontos.release.release.ReleaseCommand._create_release", autospec=True
+        "pontos.release.create.CreateReleaseCommand._create_release",
+        autospec=True,
     )
     @patch(
-        "pontos.release.release.ReleaseCommand._create_changelog",
+        "pontos.release.create.CreateReleaseCommand._create_changelog",
         autospec=True,
     )
-    @patch("pontos.release.release.Project._gather_commands", autospec=True)
+    @patch("pontos.release.create.Project._gather_commands", autospec=True)
     def test_initial_release_version(
         self,
         gather_commands_mock: MagicMock,
         create_changelog_mock: MagicMock,
         create_release_mock: AsyncMock,
         get_last_release_version_mock: MagicMock,
         git_mock: MagicMock,
@@ -305,16 +308,17 @@
                 "foo",
                 "--release-version",
                 "1.0.0",
             ]
         )
 
         with temp_git_repository():
-            released = release(
+            released = create_release(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
         git_instance_mock.push.assert_has_calls(
             [
                 call(follow_tags=True, remote=None),
@@ -352,26 +356,27 @@
                 ),
             ]
         )
         git_instance_mock.tag.assert_called_once_with(
             "v1.0.0", gpg_key_id="1234", message="Automatic release to 1.0.0"
         )
 
-        self.assertEqual(released, ReleaseReturnValue.SUCCESS)
+        self.assertEqual(released, CreateReleaseReturnValue.SUCCESS)
 
-    @patch("pontos.release.release.Git", autospec=True)
-    @patch("pontos.release.release.get_last_release_version", autospec=True)
+    @patch("pontos.release.create.Git", autospec=True)
+    @patch("pontos.release.create.get_last_release_version", autospec=True)
     @patch(
-        "pontos.release.release.ReleaseCommand._create_release", autospec=True
+        "pontos.release.create.CreateReleaseCommand._create_release",
+        autospec=True,
     )
     @patch(
-        "pontos.release.release.ReleaseCommand._create_changelog",
+        "pontos.release.create.CreateReleaseCommand._create_changelog",
         autospec=True,
     )
-    @patch("pontos.release.release.Project._gather_commands", autospec=True)
+    @patch("pontos.release.create.Project._gather_commands", autospec=True)
     def test_release_patch(
         self,
         gather_commands_mock: MagicMock,
         create_changelog_mock: MagicMock,
         create_release_mock: AsyncMock,
         get_last_release_version_mock: MagicMock,
         git_mock: MagicMock,
@@ -409,16 +414,17 @@
                 "patch",
                 "--next-version",
                 "1.0.0.dev1",
             ]
         )
 
         with temp_git_repository():
-            released = release(
+            released = create_release(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
         git_instance_mock.push.assert_has_calls(
             [
                 call(follow_tags=True, remote=None),
@@ -455,26 +461,27 @@
                 ),
             ]
         )
         git_instance_mock.tag.assert_called_once_with(
             "v0.0.2", gpg_key_id="1234", message="Automatic release to 0.0.2"
         )
 
-        self.assertEqual(released, ReleaseReturnValue.SUCCESS)
+        self.assertEqual(released, CreateReleaseReturnValue.SUCCESS)
 
-    @patch("pontos.release.release.Git", autospec=True)
-    @patch("pontos.release.release.get_last_release_version", autospec=True)
+    @patch("pontos.release.create.Git", autospec=True)
+    @patch("pontos.release.create.get_last_release_version", autospec=True)
     @patch(
-        "pontos.release.release.ReleaseCommand._create_release", autospec=True
+        "pontos.release.create.CreateReleaseCommand._create_release",
+        autospec=True,
     )
     @patch(
-        "pontos.release.release.ReleaseCommand._create_changelog",
+        "pontos.release.create.CreateReleaseCommand._create_changelog",
         autospec=True,
     )
-    @patch("pontos.release.release.Project._gather_commands", autospec=True)
+    @patch("pontos.release.create.Project._gather_commands", autospec=True)
     def test_release_calendar(
         self,
         gather_commands_mock: MagicMock,
         create_changelog_mock: MagicMock,
         create_release_mock: AsyncMock,
         get_last_release_version_mock: MagicMock,
         git_mock: MagicMock,
@@ -511,16 +518,17 @@
                 "foo",
                 "--release-type",
                 "calendar",
             ]
         )
 
         with temp_git_repository():
-            released = release(
+            released = create_release(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
         git_instance_mock.push.assert_has_calls(
             [
                 call(follow_tags=True, remote=None),
@@ -560,26 +568,27 @@
         )
         git_instance_mock.tag.assert_called_once_with(
             f"v{release_version}",
             gpg_key_id="1234",
             message=f"Automatic release to {release_version}",
         )
 
-        self.assertEqual(released, ReleaseReturnValue.SUCCESS)
+        self.assertEqual(released, CreateReleaseReturnValue.SUCCESS)
 
-    @patch("pontos.release.release.Git", autospec=True)
-    @patch("pontos.release.release.get_last_release_version", autospec=True)
+    @patch("pontos.release.create.Git", autospec=True)
+    @patch("pontos.release.create.get_last_release_version", autospec=True)
     @patch(
-        "pontos.release.release.ReleaseCommand._create_release", autospec=True
+        "pontos.release.create.CreateReleaseCommand._create_release",
+        autospec=True,
     )
     @patch(
-        "pontos.release.release.ReleaseCommand._create_changelog",
+        "pontos.release.create.CreateReleaseCommand._create_changelog",
         autospec=True,
     )
-    @patch("pontos.release.release.Project._gather_commands", autospec=True)
+    @patch("pontos.release.create.Project._gather_commands", autospec=True)
     def test_release_minor(
         self,
         gather_commands_mock: MagicMock,
         create_changelog_mock: MagicMock,
         create_release_mock: AsyncMock,
         get_last_release_version_mock: MagicMock,
         git_mock: MagicMock,
@@ -617,16 +626,17 @@
                 "minor",
                 "--next-version",
                 "0.1.1.dev1",
             ]
         )
 
         with temp_git_repository():
-            released = release(
+            released = create_release(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
         git_instance_mock.push.assert_has_calls(
             [
                 call(follow_tags=True, remote=None),
@@ -663,26 +673,27 @@
                 ),
             ]
         )
         git_instance_mock.tag.assert_called_once_with(
             "v0.1.0", gpg_key_id="1234", message="Automatic release to 0.1.0"
         )
 
-        self.assertEqual(released, ReleaseReturnValue.SUCCESS)
+        self.assertEqual(released, CreateReleaseReturnValue.SUCCESS)
 
-    @patch("pontos.release.release.Git", autospec=True)
-    @patch("pontos.release.release.get_last_release_version", autospec=True)
+    @patch("pontos.release.create.Git", autospec=True)
+    @patch("pontos.release.create.get_last_release_version", autospec=True)
     @patch(
-        "pontos.release.release.ReleaseCommand._create_release", autospec=True
+        "pontos.release.create.CreateReleaseCommand._create_release",
+        autospec=True,
     )
     @patch(
-        "pontos.release.release.ReleaseCommand._create_changelog",
+        "pontos.release.create.CreateReleaseCommand._create_changelog",
         autospec=True,
     )
-    @patch("pontos.release.release.Project._gather_commands", autospec=True)
+    @patch("pontos.release.create.Project._gather_commands", autospec=True)
     def test_release_major(
         self,
         gather_commands_mock: MagicMock,
         create_changelog_mock: MagicMock,
         create_release_mock: AsyncMock,
         get_last_release_version_mock: MagicMock,
         git_mock: MagicMock,
@@ -720,16 +731,17 @@
                 "major",
                 "--next-version",
                 "1.0.1.dev1",
             ]
         )
 
         with temp_git_repository():
-            released = release(
+            released = create_release(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
         git_instance_mock.push.assert_has_calls(
             [
                 call(follow_tags=True, remote=None),
@@ -766,26 +778,27 @@
                 ),
             ]
         )
         git_instance_mock.tag.assert_called_once_with(
             "v1.0.0", gpg_key_id="1234", message="Automatic release to 1.0.0"
         )
 
-        self.assertEqual(released, ReleaseReturnValue.SUCCESS)
+        self.assertEqual(released, CreateReleaseReturnValue.SUCCESS)
 
-    @patch("pontos.release.release.Git", autospec=True)
-    @patch("pontos.release.release.get_last_release_version", autospec=True)
+    @patch("pontos.release.create.Git", autospec=True)
+    @patch("pontos.release.create.get_last_release_version", autospec=True)
     @patch(
-        "pontos.release.release.ReleaseCommand._create_release", autospec=True
+        "pontos.release.create.CreateReleaseCommand._create_release",
+        autospec=True,
     )
     @patch(
-        "pontos.release.release.ReleaseCommand._create_changelog",
+        "pontos.release.create.CreateReleaseCommand._create_changelog",
         autospec=True,
     )
-    @patch("pontos.release.release.Project._gather_commands", autospec=True)
+    @patch("pontos.release.create.Project._gather_commands", autospec=True)
     def test_release_alpha(
         self,
         gather_commands_mock: MagicMock,
         create_changelog_mock: MagicMock,
         create_release_mock: AsyncMock,
         get_last_release_version_mock: MagicMock,
         git_mock: MagicMock,
@@ -821,16 +834,17 @@
                 "foo",
                 "--release-type",
                 "alpha",
             ]
         )
 
         with temp_git_repository():
-            released = release(
+            released = create_release(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
         git_instance_mock.push.assert_has_calls(
             [
                 call(follow_tags=True, remote=None),
@@ -869,26 +883,27 @@
         )
         git_instance_mock.tag.assert_called_once_with(
             "v0.0.2a1",
             gpg_key_id="1234",
             message="Automatic release to 0.0.2a1",
         )
 
-        self.assertEqual(released, ReleaseReturnValue.SUCCESS)
+        self.assertEqual(released, CreateReleaseReturnValue.SUCCESS)
 
-    @patch("pontos.release.release.Git", autospec=True)
-    @patch("pontos.release.release.get_last_release_version", autospec=True)
+    @patch("pontos.release.create.Git", autospec=True)
+    @patch("pontos.release.create.get_last_release_version", autospec=True)
     @patch(
-        "pontos.release.release.ReleaseCommand._create_release", autospec=True
+        "pontos.release.create.CreateReleaseCommand._create_release",
+        autospec=True,
     )
     @patch(
-        "pontos.release.release.ReleaseCommand._create_changelog",
+        "pontos.release.create.CreateReleaseCommand._create_changelog",
         autospec=True,
     )
-    @patch("pontos.release.release.Project._gather_commands", autospec=True)
+    @patch("pontos.release.create.Project._gather_commands", autospec=True)
     def test_release_beta(
         self,
         gather_commands_mock: MagicMock,
         create_changelog_mock: MagicMock,
         create_release_mock: AsyncMock,
         get_last_release_version_mock: MagicMock,
         git_mock: MagicMock,
@@ -924,16 +939,17 @@
                 "foo",
                 "--release-type",
                 "beta",
             ]
         )
 
         with temp_git_repository():
-            released = release(
+            released = create_release(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
         git_instance_mock.push.assert_has_calls(
             [
                 call(follow_tags=True, remote=None),
@@ -972,26 +988,27 @@
         )
         git_instance_mock.tag.assert_called_once_with(
             "v0.0.2b1",
             gpg_key_id="1234",
             message="Automatic release to 0.0.2b1",
         )
 
-        self.assertEqual(released, ReleaseReturnValue.SUCCESS)
+        self.assertEqual(released, CreateReleaseReturnValue.SUCCESS)
 
-    @patch("pontos.release.release.Git", autospec=True)
-    @patch("pontos.release.release.get_last_release_version", autospec=True)
+    @patch("pontos.release.create.Git", autospec=True)
+    @patch("pontos.release.create.get_last_release_version", autospec=True)
     @patch(
-        "pontos.release.release.ReleaseCommand._create_release", autospec=True
+        "pontos.release.create.CreateReleaseCommand._create_release",
+        autospec=True,
     )
     @patch(
-        "pontos.release.release.ReleaseCommand._create_changelog",
+        "pontos.release.create.CreateReleaseCommand._create_changelog",
         autospec=True,
     )
-    @patch("pontos.release.release.Project._gather_commands", autospec=True)
+    @patch("pontos.release.create.Project._gather_commands", autospec=True)
     def test_release_release_candidate(
         self,
         gather_commands_mock: MagicMock,
         create_changelog_mock: MagicMock,
         create_release_mock: AsyncMock,
         get_last_release_version_mock: MagicMock,
         git_mock: MagicMock,
@@ -1027,16 +1044,17 @@
                 "foo",
                 "--release-type",
                 "release-candidate",
             ]
         )
 
         with temp_git_repository():
-            released = release(
+            released = create_release(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
         git_instance_mock.push.assert_has_calls(
             [
                 call(follow_tags=True, remote=None),
@@ -1075,38 +1093,39 @@
         )
         git_instance_mock.tag.assert_called_once_with(
             "v0.0.2rc1",
             gpg_key_id="1234",
             message="Automatic release to 0.0.2rc1",
         )
 
-        self.assertEqual(released, ReleaseReturnValue.SUCCESS)
+        self.assertEqual(released, CreateReleaseReturnValue.SUCCESS)
 
     def test_no_token(
         self,
     ):
         _, _, args = parse_args(
             [
                 "release",
                 "--project",
                 "foo",
                 "--release-version",
                 "0.0.1",
             ]
         )
 
-        released = release(
+        released = create_release(
             terminal=mock_terminal(),
+            error_terminal=mock_terminal(),
             args=args,
             token=None,
         )
 
-        self.assertEqual(released, ReleaseReturnValue.TOKEN_MISSING)
+        self.assertEqual(released, CreateReleaseReturnValue.TOKEN_MISSING)
 
-    @patch("pontos.release.release.get_last_release_version", autospec=True)
+    @patch("pontos.release.create.get_last_release_version", autospec=True)
     def test_no_project_settings(
         self,
         get_last_release_version_mock: MagicMock,
     ):
         current_version = PEP440Version("0.0.1")
         get_last_release_version_mock.return_value = current_version
 
@@ -1116,34 +1135,36 @@
                 "--project",
                 "foo",
                 "--release-version",
                 "0.0.1",
             ]
         )
         with temp_git_repository():
-            released = release(
+            released = create_release(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
         self.assertEqual(
-            released, ReleaseReturnValue.PROJECT_SETTINGS_NOT_FOUND
+            released, CreateReleaseReturnValue.PROJECT_SETTINGS_NOT_FOUND
         )
 
-    @patch("pontos.release.release.Git", autospec=True)
-    @patch("pontos.release.release.get_last_release_version", autospec=True)
+    @patch("pontos.release.create.Git", autospec=True)
+    @patch("pontos.release.create.get_last_release_version", autospec=True)
     @patch(
-        "pontos.release.release.ReleaseCommand._create_release", autospec=True
+        "pontos.release.create.CreateReleaseCommand._create_release",
+        autospec=True,
     )
     @patch(
-        "pontos.release.release.ReleaseCommand._create_changelog",
+        "pontos.release.create.CreateReleaseCommand._create_changelog",
         autospec=True,
     )
-    @patch("pontos.release.release.Project", autospec=True)
+    @patch("pontos.release.create.Project", autospec=True)
     def test_no_update_project(
         self,
         project_mock: MagicMock,
         create_changelog_mock: MagicMock,
         create_release_mock: AsyncMock,
         get_last_release_version_mock: MagicMock,
         git_mock: MagicMock,
@@ -1165,16 +1186,17 @@
                 "--next-version",
                 "1.0.0.dev1",
                 "--no-update-project",
             ]
         )
 
         with temp_git_repository():
-            released = release(
+            released = create_release(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
         git_instance_mock.push.assert_has_calls(
             [
                 call(follow_tags=True, remote=None),
@@ -1189,38 +1211,41 @@
 
         git_instance_mock.add.assert_not_called()
         git_instance_mock.commit.assert_not_called()
         git_instance_mock.tag.assert_called_once_with(
             "v0.0.2", gpg_key_id="1234", message="Automatic release to 0.0.2"
         )
 
-        self.assertEqual(released, ReleaseReturnValue.SUCCESS)
+        self.assertEqual(released, CreateReleaseReturnValue.SUCCESS)
 
         project_mock.assert_not_called()
 
     def test_last_release_version_error(self):
         _, token, args = parse_args(
             [
                 "release",
                 "--project",
                 "foo",
                 "--release-type",
                 "major",
             ]
         )
         with temp_git_repository():
-            released = release(
+            released = create_release(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
-        self.assertEqual(released, ReleaseReturnValue.NO_LAST_RELEASE_VERSION)
+        self.assertEqual(
+            released, CreateReleaseReturnValue.NO_LAST_RELEASE_VERSION
+        )
 
-    @patch("pontos.release.release.get_last_release_version", autospec=True)
+    @patch("pontos.release.create.get_last_release_version", autospec=True)
     def test_no_last_release_version(
         self,
         get_last_release_version_mock: MagicMock,
     ):
         get_last_release_version_mock.return_value = None
         _, token, args = parse_args(
             [
@@ -1228,25 +1253,28 @@
                 "--project",
                 "foo",
                 "--release-type",
                 "minor",
             ]
         )
         with temp_git_repository():
-            released = release(
+            released = create_release(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
-        self.assertEqual(released, ReleaseReturnValue.NO_LAST_RELEASE_VERSION)
+        self.assertEqual(
+            released, CreateReleaseReturnValue.NO_LAST_RELEASE_VERSION
+        )
 
-    @patch("pontos.release.release.get_last_release_version", autospec=True)
+    @patch("pontos.release.create.get_last_release_version", autospec=True)
     @patch(
-        "pontos.release.release.ReleaseCommand._get_next_release_version",
+        "pontos.release.create.get_next_release_version",
         autospec=True,
     )
     def test_no_release_error(
         self,
         get_next_release_version_mock: MagicMock,
         get_last_release_version_mock: MagicMock,
     ):
@@ -1263,23 +1291,24 @@
                 "123",
                 "--release-type",
                 "patch",
             ]
         )
 
         with temp_git_repository():
-            released = release(
+            released = create_release(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
-        self.assertEqual(released, ReleaseReturnValue.NO_RELEASE_VERSION)
+        self.assertEqual(released, CreateReleaseReturnValue.NO_RELEASE_VERSION)
 
-    @patch("pontos.release.release.Git", autospec=True)
+    @patch("pontos.release.create.Git", autospec=True)
     @patch("pontos.version.helper.Git", autospec=True)
     def test_has_tag(
         self,
         git_mock1: MagicMock,
         git_mock2: MagicMock,
     ):
         tags = ["v1.0.0", "v1.0.1"]
@@ -1293,31 +1322,33 @@
                 "1.0.1",
                 "--project",
                 "bla",
             ]
         )
 
         with temp_git_repository():
-            released = release(
+            released = create_release(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 token=token,
                 args=args,
             )
 
-            self.assertEqual(released, ReleaseReturnValue.ALREADY_TAKEN)
+            self.assertEqual(released, CreateReleaseReturnValue.ALREADY_TAKEN)
 
         git_mock1.return_value.list_tags.assert_called_once()
         git_mock2.return_value.list_tags.assert_called_once()
 
-    @patch("pontos.release.release.Git", autospec=True)
-    @patch("pontos.release.release.get_last_release_version", autospec=True)
+    @patch("pontos.release.create.Git", autospec=True)
+    @patch("pontos.release.create.get_last_release_version", autospec=True)
     @patch(
-        "pontos.release.release.ReleaseCommand._create_release", autospec=True
+        "pontos.release.create.CreateReleaseCommand._create_release",
+        autospec=True,
     )
-    @patch("pontos.release.release.Project._gather_commands", autospec=True)
+    @patch("pontos.release.create.Project._gather_commands", autospec=True)
     def test_update_version_error(
         self,
         gather_commands_mock: MagicMock,
         create_release_mock: AsyncMock,
         get_last_release_version_mock: MagicMock,
         git_mock: MagicMock,
     ):
@@ -1336,16 +1367,17 @@
                 "0.0.1",
                 "--next-version",
                 "0.0.2.dev1",
             ]
         )
 
         with temp_git_repository():
-            released = release(
+            released = create_release(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
         git_mock.return_value.push.assert_not_called()
 
         command_mock.update_version.assert_called_once_with(
@@ -1354,25 +1386,29 @@
 
         create_release_mock.assert_not_awaited()
 
         git_mock.return_value.add.assert_not_called()
         git_mock.return_value.commit.assert_not_called()
         git_mock.return_value.tag.assert_not_called()
 
-        self.assertEqual(released, ReleaseReturnValue.UPDATE_VERSION_ERROR)
+        self.assertEqual(
+            released, CreateReleaseReturnValue.UPDATE_VERSION_ERROR
+        )
 
-    @patch("pontos.release.release.Git", autospec=True)
-    @patch("pontos.release.release.get_last_release_version", autospec=True)
+    @patch("pontos.release.create.Git", autospec=True)
+    @patch("pontos.release.create.get_last_release_version", autospec=True)
     @patch(
-        "pontos.release.release.ReleaseCommand._create_release", autospec=True
+        "pontos.release.create.CreateReleaseCommand._create_release",
+        autospec=True,
     )
     @patch(
-        "pontos.release.release.ReleaseCommand._create_changelog", autospec=True
+        "pontos.release.create.CreateReleaseCommand._create_changelog",
+        autospec=True,
     )
-    @patch("pontos.release.release.Project._gather_commands", autospec=True)
+    @patch("pontos.release.create.Project._gather_commands", autospec=True)
     def test_github_create_release_failure(
         self,
         gather_commands_mock: MagicMock,
         create_changelog_mock: MagicMock,
         create_release_mock: AsyncMock,
         get_last_release_version_mock: MagicMock,
         git_mock: MagicMock,
@@ -1415,21 +1451,24 @@
                 "0.0.1",
                 "--next-version",
                 "0.0.2.dev1",
             ]
         )
 
         with temp_git_repository():
-            released = release(
+            released = create_release(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
-        self.assertEqual(released, ReleaseReturnValue.CREATE_RELEASE_ERROR)
+        self.assertEqual(
+            released, CreateReleaseReturnValue.CREATE_RELEASE_ERROR
+        )
 
         git_instance_mock.push.assert_called_once_with(
             follow_tags=True, remote=None
         )
         git_instance_mock.add.assert_called_once_with("MyProject.conf")
         git_instance_mock.commit.assert_called_once_with(
             "Automatic release to 0.0.1", verify=False, gpg_signing_key="1234"
@@ -1439,23 +1478,25 @@
         )
 
         self.assertEqual(
             create_release_mock.await_args.args[1:],
             (release_version, "foo", "A Changelog"),
         )
 
-    @patch("pontos.release.release.Git", autospec=True)
-    @patch("pontos.release.release.get_last_release_version", autospec=True)
+    @patch("pontos.release.create.Git", autospec=True)
+    @patch("pontos.release.create.get_last_release_version", autospec=True)
     @patch(
-        "pontos.release.release.ReleaseCommand._create_release", autospec=True
+        "pontos.release.create.CreateReleaseCommand._create_release",
+        autospec=True,
     )
     @patch(
-        "pontos.release.release.ReleaseCommand._create_changelog", autospec=True
+        "pontos.release.create.CreateReleaseCommand._create_changelog",
+        autospec=True,
     )
-    @patch("pontos.release.release.Project._gather_commands", autospec=True)
+    @patch("pontos.release.create.Project._gather_commands", autospec=True)
     def test_update_version_after_release_error(
         self,
         gather_commands_mock: MagicMock,
         create_changelog_mock: MagicMock,
         create_release_mock: AsyncMock,
         get_last_release_version_mock: MagicMock,
         git_mock: MagicMock,
@@ -1489,16 +1530,17 @@
                 "0.0.1",
                 "--next-version",
                 "0.0.2.dev1",
             ]
         )
 
         with temp_git_repository():
-            released = release(
+            released = create_release(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
         git_instance_mock.push.assert_called_once_with(
             follow_tags=True, remote=None
         )
@@ -1520,26 +1562,29 @@
             "Automatic release to 0.0.1", verify=False, gpg_signing_key="1234"
         )
         git_instance_mock.tag.assert_called_once_with(
             "v0.0.1", gpg_key_id="1234", message="Automatic release to 0.0.1"
         )
 
         self.assertEqual(
-            released, ReleaseReturnValue.UPDATE_VERSION_AFTER_RELEASE_ERROR
+            released,
+            CreateReleaseReturnValue.UPDATE_VERSION_AFTER_RELEASE_ERROR,
         )
 
-    @patch("pontos.release.release.Git", autospec=True)
-    @patch("pontos.release.release.get_last_release_version", autospec=True)
+    @patch("pontos.release.create.Git", autospec=True)
+    @patch("pontos.release.create.get_last_release_version", autospec=True)
     @patch(
-        "pontos.release.release.ReleaseCommand._create_release", autospec=True
+        "pontos.release.create.CreateReleaseCommand._create_release",
+        autospec=True,
     )
     @patch(
-        "pontos.release.release.ReleaseCommand._create_changelog", autospec=True
+        "pontos.release.create.CreateReleaseCommand._create_changelog",
+        autospec=True,
     )
-    @patch("pontos.release.release.Project._gather_commands", autospec=True)
+    @patch("pontos.release.create.Project._gather_commands", autospec=True)
     def test_release_to_specific_git_remote(
         self,
         gather_commands_mock: MagicMock,
         create_changelog_mock: MagicMock,
         create_release_mock: AsyncMock,
         get_last_release_version_mock: MagicMock,
         git_mock,
@@ -1581,16 +1626,17 @@
                 "upstream",
                 "--git-signing-key",
                 "1234",
             ]
         )
 
         with temp_git_repository():
-            released = release(
+            released = create_release(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
         git_instance_mock.push.assert_has_calls(
             [
                 call(follow_tags=True, remote="upstream"),
@@ -1617,25 +1663,27 @@
             verify=False,
             gpg_signing_key="1234",
         )
         git_instance_mock.tag.assert_called_once_with(
             "v0.0.1", gpg_key_id="1234", message="Automatic release to 0.0.1"
         )
 
-        self.assertEqual(released, ReleaseReturnValue.SUCCESS)
+        self.assertEqual(released, CreateReleaseReturnValue.SUCCESS)
 
-    @patch("pontos.release.release.Git", autospec=True)
-    @patch("pontos.release.release.get_last_release_version", autospec=True)
+    @patch("pontos.release.create.Git", autospec=True)
+    @patch("pontos.release.create.get_last_release_version", autospec=True)
     @patch(
-        "pontos.release.release.ReleaseCommand._create_release", autospec=True
+        "pontos.release.create.CreateReleaseCommand._create_release",
+        autospec=True,
     )
     @patch(
-        "pontos.release.release.ReleaseCommand._create_changelog", autospec=True
+        "pontos.release.create.CreateReleaseCommand._create_changelog",
+        autospec=True,
     )
-    @patch("pontos.release.release.Project._gather_commands", autospec=True)
+    @patch("pontos.release.create.Project._gather_commands", autospec=True)
     def test_release_without_git_prefix(
         self,
         gather_commands_mock: MagicMock,
         create_changelog_mock: MagicMock,
         create_release_mock: AsyncMock,
         get_last_release_version_mock: MagicMock,
         git_mock,
@@ -1675,16 +1723,17 @@
                 "0.0.2.dev1",
                 "--git-tag-prefix",
                 "",
             ]
         )
 
         with temp_git_repository():
-            released = release(
+            released = create_release(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
         git_instance_mock.push.assert_has_calls(
             [
                 call(follow_tags=True, remote=None),
@@ -1711,23 +1760,24 @@
             verify=False,
             gpg_signing_key="1234",
         )
         git_instance_mock.tag.assert_called_once_with(
             "0.0.1", gpg_key_id="1234", message="Automatic release to 0.0.1"
         )
 
-        self.assertEqual(released, ReleaseReturnValue.SUCCESS)
+        self.assertEqual(released, CreateReleaseReturnValue.SUCCESS)
 
-    @patch("pontos.release.release.Git", autospec=True)
-    @patch("pontos.release.release.get_last_release_version", autospec=True)
-    @patch("pontos.release.release.GitHubAsyncRESTApi", autospec=True)
+    @patch("pontos.release.create.Git", autospec=True)
+    @patch("pontos.release.create.get_last_release_version", autospec=True)
+    @patch("pontos.release.create.GitHubAsyncRESTApi", autospec=True)
     @patch(
-        "pontos.release.release.ReleaseCommand._create_changelog", autospec=True
+        "pontos.release.create.CreateReleaseCommand._create_changelog",
+        autospec=True,
     )
-    @patch("pontos.release.release.Project._gather_commands", autospec=True)
+    @patch("pontos.release.create.Project._gather_commands", autospec=True)
     def test_release_github_api(
         self,
         gather_commands_mock: MagicMock,
         create_changelog_mock: MagicMock,
         github_api_mock: AsyncMock,
         get_last_release_version_mock: MagicMock,
         git_mock,
@@ -1771,16 +1821,17 @@
                 "0.0.2.dev1",
                 "--git-remote-name",
                 "upstream",
             ]
         )
 
         with temp_git_repository():
-            released = release(
+            released = create_release(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
         git_instance_mock.push.assert_has_calls(
             [
                 call(follow_tags=True, remote="upstream"),
@@ -1810,23 +1861,24 @@
             verify=False,
             gpg_signing_key="1234",
         )
         git_instance_mock.tag.assert_called_once_with(
             "v0.0.1", gpg_key_id="1234", message="Automatic release to 0.0.1"
         )
 
-        self.assertEqual(released, ReleaseReturnValue.SUCCESS)
+        self.assertEqual(released, CreateReleaseReturnValue.SUCCESS)
 
-    @patch("pontos.release.release.Git", autospec=True)
-    @patch("pontos.release.release.get_last_release_version", autospec=True)
-    @patch("pontos.release.release.GitHubAsyncRESTApi", autospec=True)
+    @patch("pontos.release.create.Git", autospec=True)
+    @patch("pontos.release.create.get_last_release_version", autospec=True)
+    @patch("pontos.release.create.GitHubAsyncRESTApi", autospec=True)
     @patch(
-        "pontos.release.release.ReleaseCommand._create_changelog", autospec=True
+        "pontos.release.create.CreateReleaseCommand._create_changelog",
+        autospec=True,
     )
-    @patch("pontos.release.release.Project._gather_commands", autospec=True)
+    @patch("pontos.release.create.Project._gather_commands", autospec=True)
     def test_release_github_api_pre_release(
         self,
         gather_commands_mock: MagicMock,
         create_changelog_mock: MagicMock,
         github_api_mock: AsyncMock,
         get_last_release_version_mock: MagicMock,
         git_mock,
@@ -1870,16 +1922,17 @@
                 "0.0.1a1+dev1",
                 "--git-remote-name",
                 "upstream",
             ]
         )
 
         with temp_git_repository():
-            released = release(
+            released = create_release(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
         git_instance_mock.push.assert_has_calls(
             [
                 call(follow_tags=True, remote="upstream"),
@@ -1911,22 +1964,23 @@
         )
         git_instance_mock.tag.assert_called_once_with(
             "v0.0.1a1",
             gpg_key_id="1234",
             message="Automatic release to 0.0.1a1",
         )
 
-        self.assertEqual(released, ReleaseReturnValue.SUCCESS)
+        self.assertEqual(released, CreateReleaseReturnValue.SUCCESS)
 
-    @patch("pontos.release.release.Git", autospec=True)
+    @patch("pontos.release.create.Git", autospec=True)
     @patch(
-        "pontos.release.release.ReleaseCommand._create_release", autospec=True
+        "pontos.release.create.CreateReleaseCommand._create_release",
+        autospec=True,
     )
     @patch(
-        "pontos.release.release.ReleaseCommand._create_changelog",
+        "pontos.release.create.CreateReleaseCommand._create_changelog",
         autospec=True,
     )
     def test_release_with_go_project(
         self,
         create_changelog_mock: MagicMock,
         create_release_mock: AsyncMock,
         git_mock,
@@ -1939,21 +1993,22 @@
         git_instance_mock.status.return_value = [
             StatusEntry(f"M  {GoVersionCommand.version_file_path}")
         ]
 
         _, token, args = parse_args(["release", "--release-type", "patch"])
 
         with setup_go_project(current_version="0.0.1", tags=["0.0.1"]):
-            released = release(
+            released = create_release(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
-        self.assertEqual(released, ReleaseReturnValue.SUCCESS)
+        self.assertEqual(released, CreateReleaseReturnValue.SUCCESS)
 
         git_instance_mock.push.assert_called_with(follow_tags=True, remote=None)
         git_instance_mock.add.assert_called_with(
             GoVersionCommand.version_file_path
         )
         git_instance_mock.commit.assert_called_with(
             "Automatic adjustments after release\n\n"
@@ -1966,23 +2021,24 @@
         )
 
         self.assertEqual(
             create_release_mock.await_args.args[1:],
             (release_version, "foo", "A Changelog"),
         )
 
-        self.assertEqual(released, ReleaseReturnValue.SUCCESS)
+        self.assertEqual(released, CreateReleaseReturnValue.SUCCESS)
 
-    @patch("pontos.release.release.Git", autospec=True)
-    @patch("pontos.release.release.get_last_release_version", autospec=True)
+    @patch("pontos.release.create.Git", autospec=True)
+    @patch("pontos.release.create.get_last_release_version", autospec=True)
     @patch("pontos.changelog.conventional_commits.Git", autospec=True)
     @patch(
-        "pontos.release.release.ReleaseCommand._create_release", autospec=True
+        "pontos.release.create.CreateReleaseCommand._create_release",
+        autospec=True,
     )
-    @patch("pontos.release.release.Project._gather_commands", autospec=True)
+    @patch("pontos.release.create.Project._gather_commands", autospec=True)
     def test_release_with_changelog(
         self,
         gather_commands_mock: MagicMock,
         create_release_mock: AsyncMock,
         cc_git_mock: MagicMock,
         get_last_release_version_mock: MagicMock,
         git_mock: MagicMock,
@@ -2046,16 +2102,17 @@
                 "0.0.2",
                 "--next-version",
                 "1.0.0.dev1",
             ]
         )
 
         with temp_git_repository():
-            released = release(
+            released = create_release(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
         git_instance_mock.list_tags.assert_called_once_with()
 
         cc_git_mock.return_value.log.assert_called_once_with(
@@ -2099,25 +2156,27 @@
                     "* Update to version 1.0.0.dev1\n",
                     verify=False,
                     gpg_signing_key="1234",
                 ),
             ]
         )
 
-        self.assertEqual(released, ReleaseReturnValue.SUCCESS)
+        self.assertEqual(released, CreateReleaseReturnValue.SUCCESS)
 
-    @patch("pontos.release.release.Git", autospec=True)
-    @patch("pontos.release.release.get_last_release_version", autospec=True)
+    @patch("pontos.release.create.Git", autospec=True)
+    @patch("pontos.release.create.get_last_release_version", autospec=True)
     @patch(
-        "pontos.release.release.ReleaseCommand._create_release", autospec=True
+        "pontos.release.create.CreateReleaseCommand._create_release",
+        autospec=True,
     )
     @patch(
-        "pontos.release.release.ReleaseCommand._create_changelog", autospec=True
+        "pontos.release.create.CreateReleaseCommand._create_changelog",
+        autospec=True,
     )
-    @patch("pontos.release.release.Project._gather_commands", autospec=True)
+    @patch("pontos.release.create.Project._gather_commands", autospec=True)
     def test_release_local(
         self,
         gather_commands_mock: MagicMock,
         create_changelog_mock: MagicMock,
         create_release_mock: AsyncMock,
         get_last_release_version_mock: MagicMock,
         git_mock,
@@ -2156,16 +2215,17 @@
                 "--next-version",
                 "0.0.2.dev1",
                 "--local",
             ]
         )
 
         with temp_git_repository():
-            released = release(
+            released = create_release(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
         git_instance_mock.push.assert_not_called()
 
         create_release_mock.assert_not_awaited()
@@ -2184,15 +2244,15 @@
             verify=False,
             gpg_signing_key="1234",
         )
         git_instance_mock.tag.assert_called_once_with(
             "v0.0.1", gpg_key_id="1234", message="Automatic release to 0.0.1"
         )
 
-        self.assertEqual(released, ReleaseReturnValue.SUCCESS)
+        self.assertEqual(released, CreateReleaseReturnValue.SUCCESS)
 
 
 @dataclass
 class Release:
     release_type: str
     expected_release_version: str
     tags: list[str] = field(default_factory=list)
@@ -2202,17 +2262,17 @@
 
 
 @patch.dict(
     "os.environ",
     {"GITHUB_TOKEN": "foo", "GITHUB_USER": "user", "GPG_SIGNING_KEY": ""},
 )
 class ReleaseGoProjectTestCase(unittest.TestCase):
-    @patch("pontos.release.release.Git.push", autospec=True)
+    @patch("pontos.release.create.Git.push", autospec=True)
     @patch(
-        "pontos.release.release.GitHubAsyncRESTApi",
+        "pontos.release.create.GitHubAsyncRESTApi",
         autospec=True,
     )
     def test_release(
         self, github_api_mock: AsyncMock, _git_push_mock: MagicMock
     ):
         create_api_mock = AsyncMock()
         github_api_mock.return_value.releases.create = create_api_mock
@@ -2283,39 +2343,40 @@
         for r in releases:
             with setup_go_project(
                 current_version=r.current_version, tags=r.tags
             ):
                 _, token, args = parse_args(
                     ["release", "--release-type", r.release_type]
                 )
-                released = release(
+                released = create_release(
                     terminal=mock_terminal(),
+                    error_terminal=mock_terminal(),
                     args=args,
                     token=token,
                 )
 
             self.assertEqual(
                 released,
-                ReleaseReturnValue.SUCCESS,
+                CreateReleaseReturnValue.SUCCESS,
                 f"v{r.expected_release_version}",
             )
             self.assertEqual(
                 create_api_mock.call_args.args[1],
                 f"v{r.expected_release_version}",
             )
 
             create_api_mock.reset_mock()
 
     @patch(
-        "pontos.release.release.ReleaseCommand._create_changelog",
+        "pontos.release.create.CreateReleaseCommand._create_changelog",
         autospec=True,
     )
-    @patch("pontos.release.release.Git.push", autospec=True)
+    @patch("pontos.release.create.Git.push", autospec=True)
     @patch(
-        "pontos.release.release.GitHubAsyncRESTApi",
+        "pontos.release.create.GitHubAsyncRESTApi",
         autospec=True,
     )
     def test_release_series(
         self,
         github_api_mock: AsyncMock,
         _git_push_mock: MagicMock,
         create_changelog_mock: MagicMock,
@@ -2451,21 +2512,22 @@
                 current_version=r.current_version, tags=r.tags
             ):
                 input_args = ["release", "--release-type", r.release_type]
                 if r.release_series:
                     input_args.extend(["--release-series", r.release_series])
 
                 _, token, args = parse_args(input_args)
-                released = release(
+                released = create_release(
                     terminal=mock_terminal(),
+                    error_terminal=mock_terminal(),
                     args=args,
                     token=token,
                 )
 
-            self.assertEqual(released, ReleaseReturnValue.SUCCESS)
+            self.assertEqual(released, CreateReleaseReturnValue.SUCCESS)
             self.assertEqual(
                 create_api_mock.call_args.args[1],
                 f"v{r.expected_release_version}",
                 f"Unexpected current release version {r}",
             )
 
             self.assertEqual(
```

### Comparing `pontos-23.7.7/tests/release/test_sign.py` & `pontos-23.8.0/tests/release/test_sign.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,15 @@
                 "--release-version",
                 "0.0.1",
             ]
         )
 
         result = sign(
             terminal=mock_terminal(),
+            error_terminal=mock_terminal(),
             args=args,
             token=token,
         )
 
         self.assertEqual(result, SignReturnValue.TOKEN_MISSING)
 
     def test_no_project(self):
@@ -61,14 +62,15 @@
                 [
                     "sign",
                 ]
             )
 
             result = sign(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
             self.assertEqual(result, SignReturnValue.NO_PROJECT)
 
     def test_no_release_error(self):
@@ -79,14 +81,15 @@
                     "--project",
                     "foo",
                 ]
             )
 
             result = sign(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
             self.assertEqual(result, SignReturnValue.NO_RELEASE_VERSION)
 
     @patch("pontos.release.sign.get_last_release_version", autospec=True)
@@ -100,14 +103,15 @@
                     "--project",
                     "foo",
                 ]
             )
 
             result = sign(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
             self.assertEqual(result, SignReturnValue.NO_RELEASE_VERSION)
 
     @patch("pontos.release.sign.GitHubAsyncRESTApi.releases", autospec=True)
@@ -123,14 +127,15 @@
                     "--release-version",
                     "1.2.3",
                 ]
             )
 
             result = sign(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
             self.assertEqual(result, SignReturnValue.NO_RELEASE)
 
     @patch("pontos.release.sign.cmd_runner", autospec=True)
@@ -178,14 +183,15 @@
                     "--release-version",
                     "1.2.3",
                 ]
             )
 
             result = sign(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
             self.assertEqual(result, SignReturnValue.SUCCESS)
 
             cmd_runner_mock.assert_has_calls(
@@ -286,14 +292,15 @@
                     "--project",
                     "foo",
                 ]
             )
 
             result = sign(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
             self.assertEqual(result, SignReturnValue.SUCCESS)
 
             cmd_runner_mock.assert_has_calls(
@@ -392,14 +399,15 @@
         with temp_directory(change_into=True):
             _, token, args = parse_args(
                 ["sign", "--project", "foo", "--release-series", "2"]
             )
 
             result = sign(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
             self.assertEqual(result, SignReturnValue.SUCCESS)
 
             cmd_runner_mock.assert_has_calls(
@@ -500,14 +508,15 @@
                     "1.2.3",
                     "--dry-run",
                 ]
             )
 
             result = sign(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
             self.assertEqual(result, SignReturnValue.SUCCESS)
 
             cmd_runner_mock.assert_has_calls(
@@ -598,14 +607,15 @@
                     "--release-version",
                     "1.2.3",
                 ]
             )
 
             result = sign(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
             self.assertEqual(
                 result, SignReturnValue.SIGNATURE_GENERATION_FAILED
             )
@@ -678,14 +688,15 @@
                     "--release-version",
                     "1.2.3",
                 ]
             )
 
             result = sign(
                 terminal=mock_terminal(),
+                error_terminal=mock_terminal(),
                 args=args,
                 token=token,
             )
 
             self.assertEqual(result, SignReturnValue.UPLOAD_ASSET_ERROR)
 
             cmd_runner_mock.assert_has_calls(
```

### Comparing `pontos-23.7.7/tests/terminal/__init__.py` & `pontos-23.8.0/tests/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/terminal/test_terminal.py` & `pontos-23.8.0/tests/terminal/test_terminal.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/test_helper.py` & `pontos-23.8.0/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/test_pontos.py` & `pontos-23.8.0/tests/test_pontos.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/testing/__init__.py` & `pontos-23.8.0/tests/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/testing/test_testing.py` & `pontos-23.8.0/tests/testing/test_testing.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/typing/__init__.py` & `pontos-23.8.0/tests/test-typing/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/typing/test_typing.py` & `pontos-23.8.0/tests/test-typing/test_typing.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/updateheader/__init__.py` & `pontos-23.8.0/tests/updateheader/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/updateheader/test_header.py` & `pontos-23.8.0/tests/updateheader/test_header.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/version/__init__.py` & `pontos-23.8.0/tests/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/version/commands/__init__.py` & `pontos-23.8.0/tests/version/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/version/commands/test_cargo.py` & `pontos-23.8.0/tests/version/commands/test_cargo.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/version/commands/test_cmake.py` & `pontos-23.8.0/tests/version/commands/test_cmake.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/version/commands/test_go.py` & `pontos-23.8.0/tests/version/commands/test_go.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/version/commands/test_java.py` & `pontos-23.8.0/tests/version/commands/test_java.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,16 +55,25 @@
             Path(
                 temp_dir / "foo/bat/config/swagger/SwaggerConfig.java",
                 parents=True,
             )
             filename = Path("NonExistentFile.java")
             search_path = temp_dir
             search_glob = "**/config/swagger/*"
-
-            result = find_file(filename, search_path, search_glob)
+            with self.assertLogs("root", level="WARNING") as cm:
+                result = find_file(filename, search_path, search_glob)
+                self.assertEqual(
+                    cm.output,
+                    [
+                        (
+                            f"WARNING:root:File {filename.name} not "
+                            f"found in {search_path.resolve()}."
+                        )
+                    ],
+                )
 
             self.assertIsNone(result)
 
 
 class TestReplaceString(unittest.TestCase):
     def test_replace_string_in_file(self):
         # Define the test parameters
@@ -163,14 +172,16 @@
             VersionError, "Premature end of data in tag foo"
         ):
             cmd = JavaVersionCommand(PEP440VersioningScheme)
             cmd.get_current_version()
 
 
 class UpdateJavaVersionCommandTestCase(unittest.TestCase):
+    swagger_file = "SwaggerConfig.java"
+
     def test_update_version_file(self):
         content = """<?xml version="1.0" encoding="UTF-8"?>
         <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 https://maven.apache.org/xsd/maven-4.0.0.xsd">
         <modelVersion>4.0.0</modelVersion><groupId>net.greenbone.umbrella</groupId>
         <artifactId>msspadminservice</artifactId><version>2023.5.3</version></project>"""
 
         with temp_file(content, name="pom.xml", change_into=True) as temp:
@@ -197,17 +208,28 @@
     def test_update_version_develop(self):
         content = """<?xml version="1.0" encoding="UTF-8"?>
         <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 https://maven.apache.org/xsd/maven-4.0.0.xsd">
         <modelVersion>4.0.0</modelVersion><groupId>net.greenbone.umbrella</groupId>
         <artifactId>msspadminservice</artifactId><version>2023.5.3</version></project>"""
 
         with temp_file(content, name="pom.xml", change_into=True) as temp:
+            swagger_search_path = Path("src").resolve()
             cmd = JavaVersionCommand(PEP440VersioningScheme)
             new_version = PEP440VersioningScheme.parse_version("2023.6.0.dev1")
-            updated = cmd.update_version(new_version)
+            with self.assertLogs("root", level="WARNING") as cm:
+                updated = cmd.update_version(new_version)
+                self.assertEqual(
+                    cm.output,
+                    [
+                        (
+                            f"WARNING:root:File {self.swagger_file} not "
+                            f"found in {swagger_search_path.resolve()}."
+                        )
+                    ],
+                )
 
             self.assertEqual(
                 updated.previous,
                 PEP440VersioningScheme.parse_version("2023.5.3"),
             )
             self.assertEqual(
                 updated.new,
```

### Comparing `pontos-23.7.7/tests/version/commands/test_javascript.py` & `pontos-23.8.0/tests/version/commands/test_javascript.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/version/commands/test_python.py` & `pontos-23.8.0/tests/version/commands/test_python.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/version/schemes/__init__.py` & `pontos-23.8.0/tests/version/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/version/schemes/test_pep440.py` & `pontos-23.8.0/tests/version/schemes/test_pep440.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/version/schemes/test_semantic.py` & `pontos-23.8.0/tests/version/schemes/test_semantic.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/version/test_commands.py` & `pontos-23.8.0/tests/version/test_commands.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/version/test_errors.py` & `pontos-23.8.0/tests/version/test_errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/version/test_helper.py` & `pontos-23.8.0/tests/version/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/version/test_main.py` & `pontos-23.8.0/tests/version/test_main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/version/test_parser.py` & `pontos-23.8.0/tests/version/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/version/test_project.py` & `pontos-23.8.0/tests/version/test_project.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/tests/version/test_version.py` & `pontos-23.8.0/tests/version/test_version.py`

 * *Files identical despite different names*

### Comparing `pontos-23.7.7/PKG-INFO` & `pontos-23.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: pontos
-Version: 23.7.7
+Version: 23.8.0
 Summary: Common utilities and tools maintained by Greenbone Networks
 Home-page: https://github.com/greenbone/pontos/
 License: GPL-3.0-or-later
 Author: Greenbone AG
 Author-email: info@greenbone.net
-Requires-Python: >=3.9
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: colorful (>=0.5.4)
-Requires-Dist: httpx[http2] (>=0.23,<0.25)
+Requires-Dist: httpx[http2] (>=0.23)
 Requires-Dist: lxml (>=4.9.0)
 Requires-Dist: packaging (>=20.3)
 Requires-Dist: python-dateutil (>=2.8.2)
 Requires-Dist: rich (>=12.4.4)
 Requires-Dist: semver (>=2.13)
 Requires-Dist: tomlkit (>=0.5.11)
-Requires-Dist: typing-extensions (>=4.4.0,<5.0.0) ; python_version < "3.8"
 Project-URL: Documentation, https://greenbone.github.io/pontos/
 Project-URL: Repository, https://github.com/greenbone/pontos/
 Description-Content-Type: text/markdown
 
 ![Greenbone Logo](https://www.greenbone.net/wp-content/uploads/gb_new-logo_horizontal_rgb_small.png)
 
 # Pontos - Greenbone Python Utilities and Tools <!-- omit in toc -->
```

