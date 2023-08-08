# Comparing `tmp/tickit-devices-0.2.0.tar.gz` & `tmp/tickit-devices-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tickit-devices-0.2.0.tar", last modified: Tue Jul 25 08:43:03 2023, max compression
+gzip compressed data, was "tickit-devices-0.3.0.tar", last modified: Tue Aug  8 15:15:13 2023, max compression
```

## Comparing `tickit-devices-0.2.0.tar` & `tickit-devices-0.3.0.tar`

### file list

```diff
@@ -1,181 +1,181 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.389947 tickit-devices-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.361947 tickit-devices-0.2.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.361947 tickit-devices-0.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.353947 tickit-devices-0.2.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.361947 tickit-devices-0.2.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.361947 tickit-devices-0.2.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.361947 tickit-devices-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.gitremotes
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.365947 tickit-devices-0.2.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16446 2023-07-25 08:43:03.389947 tickit-devices-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.365947 tickit-devices-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.365947 tickit-devices-0.2.0/docs/developer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.365947 tickit-devices-0.2.0/docs/developer/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.365947 tickit-devices-0.2.0/docs/developer/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/developer/explanations/decisions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.365947 tickit-devices-0.2.0/docs/developer/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/developer/how-to/build-docs.rst
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/developer/how-to/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/developer/how-to/lint.rst
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/developer/how-to/make-release.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/developer/how-to/pin-requirements.rst
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/developer/how-to/run-tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/developer/how-to/static-analysis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/developer/how-to/test-container.rst
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/developer/how-to/update-tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/developer/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.365947 tickit-devices-0.2.0/docs/developer/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/developer/reference/standards.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.369947 tickit-devices-0.2.0/docs/developer/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/developer/tutorials/dev-install.rst
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.369947 tickit-devices-0.2.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.369947 tickit-devices-0.2.0/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.369947 tickit-devices-0.2.0/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/user/explanations/docs-structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.369947 tickit-devices-0.2.0/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/user/how-to/run-container.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.369947 tickit-devices-0.2.0/docs/user/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.369947 tickit-devices-0.2.0/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/user/tutorials/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.357947 tickit-devices-0.2.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.369947 tickit-devices-0.2.0/examples/configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.369947 tickit-devices-0.2.0/examples/configs/cryostream/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/examples/configs/cryostream/cryo-tcp.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.369947 tickit-devices-0.2.0/examples/configs/eiger/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/examples/configs/eiger/eiger.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.369947 tickit-devices-0.2.0/examples/configs/femto/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/examples/configs/femto/current-monitor.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/examples/configs/multi-ioc.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.369947 tickit-devices-0.2.0/examples/configs/pneumatic/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/examples/configs/pneumatic/attns.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.369947 tickit-devices-0.2.0/examples/configs/synchrotron/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/examples/configs/synchrotron/synchrotron.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/examples/configs/synchrotron/synchrotron_current.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/examples/configs/synchrotron/synchrotron_machine.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/examples/configs/synchrotron/synchrotron_topup.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.369947 tickit-devices-0.2.0/s03_configs/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/s03_configs/synchrotron.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 08:43:03.389947 tickit-devices-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.357947 tickit-devices-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.373947 tickit-devices-0.2.0/src/tickit_devices/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-25 08:43:03.000000 tickit-devices-0.2.0/src/tickit_devices/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.373947 tickit-devices-0.2.0/src/tickit_devices/cryostream/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/cryostream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12363 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/cryostream/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/cryostream/cryostream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/cryostream/states.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/cryostream/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.377947 tickit-devices-0.2.0/src/tickit_devices/eiger/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.377947 tickit-devices-0.2.0/src/tickit_devices/eiger/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/data/dummy_image.py
--rw-r--r--   0 runner    (1001) docker     (123)   514994 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/data/frame_sample
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/data/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/eiger.py
--rw-r--r--   0 runner    (1001) docker     (123)    15464 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/eiger_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/eiger_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/eiger_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/eiger_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.377947 tickit-devices-0.2.0/src/tickit_devices/eiger/filewriter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/filewriter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/filewriter/filewriter_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/filewriter/filewriter_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.377947 tickit-devices-0.2.0/src/tickit_devices/eiger/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/monitor/monitor_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/monitor/monitor_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.381947 tickit-devices-0.2.0/src/tickit_devices/eiger/stream/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/stream/eiger_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/stream/stream_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/stream/stream_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.381947 tickit-devices-0.2.0/src/tickit_devices/femto/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/femto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/femto/current.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/femto/femto.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/femto/record.db
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.381947 tickit-devices-0.2.0/src/tickit_devices/pneumatic/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/pneumatic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.381947 tickit-devices-0.2.0/src/tickit_devices/pneumatic/db_files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/pneumatic/db_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/pneumatic/db_files/filter1.db
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/pneumatic/pneumatic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.381947 tickit-devices-0.2.0/src/tickit_devices/synchrotron/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/synchrotron/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.381947 tickit-devices-0.2.0/src/tickit_devices/synchrotron/db_files/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/synchrotron/db_files/DCCT.db
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/synchrotron/db_files/FILL.db
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/synchrotron/db_files/MSTAT.db
--rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/synchrotron/synchrotron_current.py
--rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/synchrotron/synchrotron_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/synchrotron/synchrotron_topup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.373947 tickit-devices-0.2.0/src/tickit_devices.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16446 2023-07-25 08:43:03.000000 tickit-devices-0.2.0/src/tickit_devices.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-07-25 08:43:03.000000 tickit-devices-0.2.0/src/tickit_devices.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 08:43:03.000000 tickit-devices-0.2.0/src/tickit_devices.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-25 08:43:03.000000 tickit-devices-0.2.0/src/tickit_devices.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-25 08:43:03.000000 tickit-devices-0.2.0/src/tickit_devices.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-25 08:43:03.000000 tickit-devices-0.2.0/src/tickit_devices.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.385947 tickit-devices-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.385947 tickit-devices-0.2.0/tests/cryostream/
--rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/cryostream/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/cryostream/test_cryostream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.385947 tickit-devices-0.2.0/tests/eiger/
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/eiger/test_eiger.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/eiger/test_eiger_filewriter_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/eiger/test_eiger_filewriter_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/eiger/test_eiger_monitor_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/eiger/test_eiger_monitor_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/eiger/test_eiger_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/eiger/test_eiger_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/eiger/test_eiger_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/eiger/test_eiger_stream_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/eiger/test_eiger_stream_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/eiger/test_eiger_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.385947 tickit-devices-0.2.0/tests/femto/
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/femto/test_femto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.385947 tickit-devices-0.2.0/tests/multi/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/multi/test_multi_device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.385947 tickit-devices-0.2.0/tests/pneumatic/
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/pneumatic/test_pneumatic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.389947 tickit-devices-0.2.0/tests/synchrotron/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/synchrotron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/synchrotron/test_synchrotron.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/synchrotron/test_synchrotron_current.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/synchrotron/test_synchrotron_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/synchrotron/test_synchrotron_topup.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.326454 tickit-devices-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.314454 tickit-devices-0.3.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.314454 tickit-devices-0.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.310454 tickit-devices-0.3.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.314454 tickit-devices-0.3.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.314454 tickit-devices-0.3.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.314454 tickit-devices-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/.gitremotes
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.314454 tickit-devices-0.3.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16446 2023-08-08 15:15:13.326454 tickit-devices-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.314454 tickit-devices-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.314454 tickit-devices-0.3.0/docs/developer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.314454 tickit-devices-0.3.0/docs/developer/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.314454 tickit-devices-0.3.0/docs/developer/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/docs/developer/explanations/decisions.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.314454 tickit-devices-0.3.0/docs/developer/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/docs/developer/how-to/build-docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/docs/developer/how-to/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/docs/developer/how-to/lint.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/docs/developer/how-to/make-release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/docs/developer/how-to/pin-requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/docs/developer/how-to/run-tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/docs/developer/how-to/static-analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/docs/developer/how-to/test-container.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/docs/developer/how-to/update-tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/docs/developer/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.314454 tickit-devices-0.3.0/docs/developer/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/docs/developer/reference/standards.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.314454 tickit-devices-0.3.0/docs/developer/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/docs/developer/tutorials/dev-install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/docs/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.318454 tickit-devices-0.3.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.318454 tickit-devices-0.3.0/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.318454 tickit-devices-0.3.0/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/docs/user/explanations/docs-structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.318454 tickit-devices-0.3.0/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/docs/user/how-to/run-container.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.318454 tickit-devices-0.3.0/docs/user/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.318454 tickit-devices-0.3.0/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/docs/user/tutorials/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.310454 tickit-devices-0.3.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.318454 tickit-devices-0.3.0/examples/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.318454 tickit-devices-0.3.0/examples/configs/cryostream/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/examples/configs/cryostream/cryo-tcp.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.318454 tickit-devices-0.3.0/examples/configs/eiger/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/examples/configs/eiger/eiger.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.318454 tickit-devices-0.3.0/examples/configs/femto/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/examples/configs/femto/current-monitor.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/examples/configs/multi-ioc.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.318454 tickit-devices-0.3.0/examples/configs/pneumatic/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/examples/configs/pneumatic/attns.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.318454 tickit-devices-0.3.0/examples/configs/synchrotron/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/examples/configs/synchrotron/synchrotron.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/examples/configs/synchrotron/synchrotron_current.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/examples/configs/synchrotron/synchrotron_machine.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/examples/configs/synchrotron/synchrotron_topup.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.318454 tickit-devices-0.3.0/s03_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/s03_configs/synchrotron.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 15:15:13.326454 tickit-devices-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.310454 tickit-devices-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.318454 tickit-devices-0.3.0/src/tickit_devices/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-08 15:15:13.000000 tickit-devices-0.3.0/src/tickit_devices/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.318454 tickit-devices-0.3.0/src/tickit_devices/cryostream/
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/cryostream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12363 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/cryostream/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/cryostream/cryostream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/cryostream/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/cryostream/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.318454 tickit-devices-0.3.0/src/tickit_devices/eiger/
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/eiger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.322454 tickit-devices-0.3.0/src/tickit_devices/eiger/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/eiger/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/eiger/data/dummy_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)   514994 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/eiger/data/frame_sample
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/eiger/data/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/eiger/eiger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15601 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/eiger/eiger_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/eiger/eiger_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/eiger/eiger_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/eiger/eiger_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.322454 tickit-devices-0.3.0/src/tickit_devices/eiger/filewriter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/eiger/filewriter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/eiger/filewriter/filewriter_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/eiger/filewriter/filewriter_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.322454 tickit-devices-0.3.0/src/tickit_devices/eiger/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/eiger/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/eiger/monitor/monitor_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/eiger/monitor/monitor_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.322454 tickit-devices-0.3.0/src/tickit_devices/eiger/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/eiger/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/eiger/stream/eiger_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/eiger/stream/stream_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/eiger/stream/stream_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.322454 tickit-devices-0.3.0/src/tickit_devices/femto/
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/femto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/femto/current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/femto/femto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/femto/record.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.322454 tickit-devices-0.3.0/src/tickit_devices/pneumatic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/pneumatic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.322454 tickit-devices-0.3.0/src/tickit_devices/pneumatic/db_files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/pneumatic/db_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/pneumatic/db_files/filter1.db
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/pneumatic/pneumatic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.322454 tickit-devices-0.3.0/src/tickit_devices/synchrotron/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/synchrotron/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.322454 tickit-devices-0.3.0/src/tickit_devices/synchrotron/db_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/synchrotron/db_files/DCCT.db
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/synchrotron/db_files/FILL.db
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/synchrotron/db_files/MSTAT.db
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/synchrotron/synchrotron_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/synchrotron/synchrotron_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8247 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/src/tickit_devices/synchrotron/synchrotron_topup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.318454 tickit-devices-0.3.0/src/tickit_devices.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16446 2023-08-08 15:15:13.000000 tickit-devices-0.3.0/src/tickit_devices.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-08-08 15:15:13.000000 tickit-devices-0.3.0/src/tickit_devices.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 15:15:13.000000 tickit-devices-0.3.0/src/tickit_devices.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-08 15:15:13.000000 tickit-devices-0.3.0/src/tickit_devices.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-08 15:15:13.000000 tickit-devices-0.3.0/src/tickit_devices.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-08 15:15:13.000000 tickit-devices-0.3.0/src/tickit_devices.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.322454 tickit-devices-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.322454 tickit-devices-0.3.0/tests/cryostream/
+-rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/tests/cryostream/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/tests/cryostream/test_cryostream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.326454 tickit-devices-0.3.0/tests/eiger/
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/tests/eiger/test_eiger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/tests/eiger/test_eiger_filewriter_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/tests/eiger/test_eiger_filewriter_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/tests/eiger/test_eiger_monitor_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/tests/eiger/test_eiger_monitor_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/tests/eiger/test_eiger_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/tests/eiger/test_eiger_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/tests/eiger/test_eiger_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/tests/eiger/test_eiger_stream_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/tests/eiger/test_eiger_stream_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/tests/eiger/test_eiger_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.326454 tickit-devices-0.3.0/tests/femto/
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/tests/femto/test_femto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.326454 tickit-devices-0.3.0/tests/multi/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/tests/multi/test_multi_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.326454 tickit-devices-0.3.0/tests/pneumatic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/tests/pneumatic/test_pneumatic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:13.326454 tickit-devices-0.3.0/tests/synchrotron/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/tests/synchrotron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/tests/synchrotron/test_synchrotron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/tests/synchrotron/test_synchrotron_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/tests/synchrotron/test_synchrotron_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/tests/synchrotron/test_synchrotron_topup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-08 15:15:05.000000 tickit-devices-0.3.0/tests/test_cli.py
```

### Comparing `tickit-devices-0.2.0/.devcontainer/devcontainer.json` & `tickit-devices-0.3.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/.github/CONTRIBUTING.rst` & `tickit-devices-0.3.0/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/.github/actions/install_requirements/action.yml` & `tickit-devices-0.3.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/.github/dependabot.yml` & `tickit-devices-0.3.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/.github/pages/make_switcher.py` & `tickit-devices-0.3.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/.github/workflows/code.yml` & `tickit-devices-0.3.0/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/.github/workflows/docs.yml` & `tickit-devices-0.3.0/.github/workflows/docs.yml`

 * *Files 9% similar despite different names*

```diff
@@ -42,12 +42,12 @@
       - name: Write switcher.json
         run: python .github/pages/make_switcher.py --add $DOCS_VERSION ${{ github.repository }} .github/pages/switcher.json
 
       - name: Publish Docs to gh-pages
         if: github.event_name == 'push' && github.actor != 'dependabot[bot]'
         # We pin to the SHA, not the tag, for security reasons.
         # https://docs.github.com/en/actions/learn-github-actions/security-hardening-for-github-actions#using-third-party-actions
-        uses: peaceiris/actions-gh-pages@bd8c6b06eba6b3d25d72b7a1767993c0aeee42e7 # v3.9.2
+        uses: peaceiris/actions-gh-pages@373f7f263a76c20808c831209c920827a82a2847 # v3.9.3
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
           publish_dir: .github/pages
           keep_files: true
```

### Comparing `tickit-devices-0.2.0/.github/workflows/docs_clean.yml` & `tickit-devices-0.3.0/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/.github/workflows/linkcheck.yml` & `tickit-devices-0.3.0/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/.gitignore` & `tickit-devices-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/.vscode/launch.json` & `tickit-devices-0.3.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/.vscode/settings.json` & `tickit-devices-0.3.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/Dockerfile` & `tickit-devices-0.3.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/LICENSE` & `tickit-devices-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/PKG-INFO` & `tickit-devices-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tickit-devices
-Version: 0.2.0
+Version: 0.3.0
 Summary: Devices for tickit, an event-based device simulation framework
 Author-email: Abigail Emery <abigail.emery@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `tickit-devices-0.2.0/README.rst` & `tickit-devices-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/docs/conf.py` & `tickit-devices-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst` & `tickit-devices-0.3.0/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/docs/developer/explanations/decisions.rst` & `tickit-devices-0.3.0/docs/developer/explanations/decisions.rst`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/docs/developer/how-to/build-docs.rst` & `tickit-devices-0.3.0/docs/developer/how-to/build-docs.rst`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/docs/developer/how-to/lint.rst` & `tickit-devices-0.3.0/docs/developer/how-to/lint.rst`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/docs/developer/how-to/make-release.rst` & `tickit-devices-0.3.0/docs/developer/how-to/make-release.rst`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/docs/developer/how-to/pin-requirements.rst` & `tickit-devices-0.3.0/docs/developer/how-to/pin-requirements.rst`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/docs/developer/how-to/test-container.rst` & `tickit-devices-0.3.0/docs/developer/how-to/test-container.rst`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/docs/developer/how-to/update-tools.rst` & `tickit-devices-0.3.0/docs/developer/how-to/update-tools.rst`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/docs/developer/index.rst` & `tickit-devices-0.3.0/docs/developer/index.rst`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/docs/developer/reference/standards.rst` & `tickit-devices-0.3.0/docs/developer/reference/standards.rst`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/docs/developer/tutorials/dev-install.rst` & `tickit-devices-0.3.0/docs/developer/tutorials/dev-install.rst`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/docs/images/dls-favicon.ico` & `tickit-devices-0.3.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/docs/images/dls-logo.svg` & `tickit-devices-0.3.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/docs/index.rst` & `tickit-devices-0.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/docs/user/explanations/docs-structure.rst` & `tickit-devices-0.3.0/docs/user/explanations/docs-structure.rst`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/docs/user/index.rst` & `tickit-devices-0.3.0/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/docs/user/tutorials/installation.rst` & `tickit-devices-0.3.0/docs/user/tutorials/installation.rst`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/examples/configs/multi-ioc.yaml` & `tickit-devices-0.3.0/examples/configs/multi-ioc.yaml`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/pyproject.toml` & `tickit-devices-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 description = "Devices for tickit, an event-based device simulation framework"
 dependencies = [
-    "tickit>=0.3",
+    "tickit>=0.4.1",
     "typing_extensions",
     "softioc",
     "pydantic>1",
     "apischema"
 ]
 dynamic = ["version"]
 license.file = "LICENSE"
```

### Comparing `tickit-devices-0.2.0/src/tickit_devices/cryostream/base.py` & `tickit-devices-0.3.0/src/tickit_devices/cryostream/base.py`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/src/tickit_devices/cryostream/cryostream.py` & `tickit-devices-0.3.0/src/tickit_devices/cryostream/cryostream.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import asyncio
 import struct
 from typing import AsyncIterable, TypedDict
 
-from tickit.adapters.composed import ComposedAdapter
-from tickit.adapters.interpreters.command import CommandInterpreter, RegexCommand
-from tickit.adapters.servers.tcp import TcpServer
+from tickit.adapters.specifications import RegexCommand
+from tickit.adapters.tcp import CommandAdapter
 from tickit.core.device import Device, DeviceUpdate
 from tickit.core.typedefs import SimTime
-from tickit.utils.byte_format import ByteFormat
 
 from tickit_devices.cryostream.base import CryostreamBase
 from tickit_devices.cryostream.states import PhaseIds
 
 _EXTENDED_STATUS = ">BBHHHBBHHHHHBBBBBBHHBBBBBBBBHH"
 
 
 class CryostreamDevice(Device, CryostreamBase):
     """A Cryostream device, used for cooling of samples using cold gas."""
 
     #: An empty typed mapping of device inputs
-    Inputs: TypedDict = TypedDict("Inputs", {})
+    class Inputs(TypedDict):
+        ...
+
     #: A typed mapping containing the 'temperature' output value
-    Outputs: TypedDict = TypedDict("Outputs", {"temperature": float})
+    class Outputs(TypedDict):
+        temperature: float
 
     def __init__(self) -> None:
         """A Cryostream constructor sets up initial internal values."""
         super().__init__()
         self.phase_id: int = PhaseIds.HOLD.value
         self.callback_period: SimTime = SimTime(int(1e9))
 
@@ -50,39 +51,22 @@
             return DeviceUpdate(
                 self.Outputs(temperature=self.gas_temp),
                 SimTime(time + int(self.plat_duration * 1e10)),
             )
         return DeviceUpdate(self.Outputs(temperature=self.gas_temp), None)
 
 
-class CryostreamAdapter(ComposedAdapter[bytes]):
+class CryostreamAdapter(CommandAdapter):
     """A Cryostream TCP adapter which sends regular status packets and can set modes."""
 
     device: CryostreamDevice
 
-    def __init__(
-        self,
-        host: str = "localhost",
-        port: int = 25565,
-    ) -> None:
-        """A CryostreamAdapter constructor which instantiates a TcpServer with host and
-        port.
-
-        Args:
-            device (Device): The device which this adapter is attached to
-            raise_interrupt (Callable): A callback to request that the device is
-                updated immediately.
-            host (Optional[str]): The host address of the TcpServer. Defaults to
-                "localhost".
-            port (Optional[int]): The bound port of the TcpServer. Defaults to 25565.
-        """
-        super().__init__(
-            TcpServer(format=ByteFormat(b"%b"), host=host, port=port),
-            CommandInterpreter(),
-        )
+    def __init__(self, device: CryostreamDevice) -> None:
+        super().__init__()
+        self.device = device
 
     async def on_connect(self) -> AsyncIterable[bytes]:
         """A method which continiously yields status packets.
 
         Returns:
             AsyncIterable[bytes]: An asyncronous iterable of packed Cryostream status
                 packets.
```

### Comparing `tickit-devices-0.2.0/src/tickit_devices/cryostream/states.py` & `tickit-devices-0.3.0/src/tickit_devices/cryostream/states.py`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/src/tickit_devices/cryostream/status.py` & `tickit-devices-0.3.0/src/tickit_devices/cryostream/status.py`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/src/tickit_devices/eiger/data/dummy_image.py` & `tickit-devices-0.3.0/src/tickit_devices/eiger/data/dummy_image.py`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/src/tickit_devices/eiger/data/frame_sample` & `tickit-devices-0.3.0/src/tickit_devices/eiger/data/frame_sample`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/src/tickit_devices/eiger/data/schema.py` & `tickit-devices-0.3.0/src/tickit_devices/eiger/data/schema.py`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/src/tickit_devices/eiger/eiger.py` & `tickit-devices-0.3.0/src/tickit_devices/eiger/eiger.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,18 +37,19 @@
     settings: EigerSettings
     status: EigerStatus
     stream: EigerStream
 
     _num_frames_left: int
     _data_queue: Queue
 
-    #: An empty typed mapping of input values
-    Inputs: TypedDict = TypedDict("Inputs", {"trigger": bool}, total=False)
-    #: A typed mapping containing the 'value' output value
-    Outputs: TypedDict = TypedDict("Outputs", {})
+    class Inputs(TypedDict, total=False):
+        trigger: bool
+
+    class Outputs(TypedDict):
+        ...
 
     def __init__(
         self,
         settings: Optional[EigerSettings] = None,
         status: Optional[EigerStatus] = None,
         stream: Optional[EigerStream] = None,
     ) -> None:
```

### Comparing `tickit-devices-0.2.0/src/tickit_devices/eiger/eiger_adapters.py` & `tickit-devices-0.3.0/src/tickit_devices/eiger/eiger_adapters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 
 from aiohttp import web
 from apischema import serialize
-from tickit.adapters.httpadapter import HttpAdapter
-from tickit.adapters.interpreters.endpoints.http_endpoint import HttpEndpoint
-from tickit.adapters.zeromq.push_adapter import ZeroMqPushAdapter
+from tickit.adapters.http import HttpAdapter
+from tickit.adapters.specifications import HttpEndpoint
+from tickit.adapters.zmq import ZeroMqPushAdapter
 
 from tickit_devices.eiger.eiger import EigerDevice
 from tickit_devices.eiger.eiger_schema import SequenceComplete, Value, construct_value
 from tickit_devices.eiger.eiger_status import State
 
 API_VERSION = "1.8.0"
 DETECTOR_API = f"detector/api/{API_VERSION}"
@@ -20,14 +20,17 @@
 
 
 class EigerRESTAdapter(HttpAdapter):
     """An Eiger adapter which parses the commands sent to the HTTP server."""
 
     device: EigerDevice
 
+    def __init__(self, device: EigerDevice) -> None:
+        self.device = device
+
     @HttpEndpoint.get(f"/{DETECTOR_API}" + "/config/{parameter_name}")
     async def get_config(self, request: web.Request) -> web.Response:
         """A HTTP Endpoint for requesting configuration variables from the Eiger.
 
         Args:
             request (web.Request): The request object that takes the given parameter.
 
@@ -185,15 +188,15 @@
         Returns:
             web.Response: The response object returned given the result of the HTTP
                 request.
         """
         LOGGER.debug("Triggering Eiger")
         await self.device.trigger()
 
-        await self.raise_interrupt()
+        await self.interrupt()
         await self.device.finished_aquisition.wait()
 
         return web.json_response(serialize(SequenceComplete(4)))
 
     @HttpEndpoint.put(f"/{DETECTOR_API}" + "/command/cancel", interrupt=True)
     async def cancel_eiger(self, request: web.Request) -> web.Response:
         """A HTTP Endpoint for the 'cancel' command of the Eiger.
@@ -417,11 +420,15 @@
 
 
 class EigerZMQAdapter(ZeroMqPushAdapter):
     """An Eiger adapter which parses the data to send along a ZeroMQStream."""
 
     device: EigerDevice
 
+    def __init__(self, device: EigerDevice) -> None:
+        super().__init__()
+        self.device = device
+
     def after_update(self) -> None:
         """Updates IOC values immediately following a device update."""
         buffered_data = self.device.stream.consume_data()
-        self.send_message_sequence_soon([list(buffered_data)])
+        self.add_message_to_stream([list(buffered_data)])
```

### Comparing `tickit-devices-0.2.0/src/tickit_devices/eiger/eiger_schema.py` & `tickit-devices-0.3.0/src/tickit_devices/eiger/eiger_schema.py`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/src/tickit_devices/eiger/eiger_settings.py` & `tickit-devices-0.3.0/src/tickit_devices/eiger/eiger_settings.py`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/src/tickit_devices/eiger/eiger_status.py` & `tickit-devices-0.3.0/src/tickit_devices/eiger/eiger_status.py`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/src/tickit_devices/eiger/filewriter/filewriter_config.py` & `tickit-devices-0.3.0/src/tickit_devices/eiger/filewriter/filewriter_config.py`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/src/tickit_devices/eiger/filewriter/filewriter_status.py` & `tickit-devices-0.3.0/src/tickit_devices/eiger/filewriter/filewriter_status.py`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/src/tickit_devices/eiger/monitor/monitor_config.py` & `tickit-devices-0.3.0/src/tickit_devices/eiger/monitor/monitor_config.py`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/src/tickit_devices/eiger/monitor/monitor_status.py` & `tickit-devices-0.3.0/src/tickit_devices/eiger/monitor/monitor_status.py`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/src/tickit_devices/eiger/stream/eiger_stream.py` & `tickit-devices-0.3.0/src/tickit_devices/eiger/stream/eiger_stream.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,18 +30,19 @@
 
     status: StreamStatus
     config: StreamConfig
     callback_period: SimTime
 
     _message_buffer: Queue[_Message]
 
-    #: An empty typed mapping of input values
-    Inputs: TypedDict = TypedDict("Inputs", {})
-    #: A typed mapping containing the 'value' output value
-    Outputs: TypedDict = TypedDict("Outputs", {})
+    class Inputs(TypedDict):
+        ...
+
+    class Outputs(TypedDict):
+        ...
 
     def __init__(self, callback_period: int = int(1e9)) -> None:
         """An Eiger Stream constructor."""
         self.status = StreamStatus()
         self.config = StreamConfig()
         self.callback_period = SimTime(callback_period)
```

### Comparing `tickit-devices-0.2.0/src/tickit_devices/eiger/stream/stream_config.py` & `tickit-devices-0.3.0/src/tickit_devices/eiger/stream/stream_config.py`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/src/tickit_devices/eiger/stream/stream_status.py` & `tickit-devices-0.3.0/src/tickit_devices/eiger/stream/stream_status.py`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/src/tickit_devices/femto/__init__.py` & `tickit-devices-0.3.0/src/tickit_devices/femto/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import pydantic.v1.dataclasses
+from tickit.adapters.io import EpicsIo
+from tickit.core.adapter import AdapterContainer
 from tickit.core.components.component import Component, ComponentConfig
 from tickit.core.components.device_simulation import DeviceSimulation
 
 from .current import CurrentDevice
 from .femto import FemtoAdapter, FemtoDevice
 
 
@@ -12,20 +14,30 @@
 
     initial_gain: float = 2.5
     initial_current: float = 0.0
     db_file: str = "src/tickit_devices/femto/record.db"
     ioc_name: str = "FEMTO"
 
     def __call__(self) -> Component:  # noqa: D102
+        device = FemtoDevice(
+            initial_gain=self.initial_gain, initial_current=self.initial_current
+        )
+        adapters = [
+            AdapterContainer(
+                FemtoAdapter(device),
+                EpicsIo(
+                    self.ioc_name,
+                    self.db_file,
+                ),
+            )
+        ]
         return DeviceSimulation(
             name=self.name,
-            device=FemtoDevice(
-                initial_gain=self.initial_gain, initial_current=self.initial_current
-            ),
-            adapters=[FemtoAdapter(db_file=self.db_file, ioc_name=self.ioc_name)],
+            device=device,
+            adapters=adapters,
         )
 
 
 @pydantic.v1.dataclasses.dataclass
 class Current(ComponentConfig):
     """Simulated current source."""
```

### Comparing `tickit-devices-0.2.0/src/tickit_devices/femto/current.py` & `tickit-devices-0.3.0/src/tickit_devices/femto/current.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,16 +4,20 @@
 from tickit.core.device import Device, DeviceUpdate
 from tickit.core.typedefs import SimTime
 
 
 class CurrentDevice(Device):
     """The current configured device."""
 
+    class Inputs(TypedDict):
+        ...
+
     #: A typed mapping containing the current output value
-    Outputs: TypedDict = TypedDict("Outputs", {"output": float})
+    class Outputs(TypedDict):
+        output: float
 
     def __init__(self, callback_period: int) -> None:
         """Initialise the current device.
 
         Args:
             callback_period (Optional[int]): The duration in which the device should \
                 next be updated. Defaults to int(1e9).
```

### Comparing `tickit-devices-0.2.0/src/tickit_devices/femto/femto.py` & `tickit-devices-0.3.0/src/tickit_devices/femto/femto.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 from typing import TypedDict
 
 from softioc import builder
-from tickit.adapters.epicsadapter import EpicsAdapter
+from tickit.adapters.epics import EpicsAdapter
 from tickit.core.device import Device, DeviceUpdate
 from tickit.core.typedefs import SimTime
 
 
 class FemtoDevice(Device):
     """Electronic signal amplifier."""
 
-    #: An empty typed mapping of device inputs
-    Inputs: TypedDict = TypedDict("Inputs", {"input": float})
-    #: A typed mapping containing the current output value
-    Outputs: TypedDict = TypedDict("Outputs", {"current": float})
+    class Inputs(TypedDict):
+        input: float
+
+    class Outputs(TypedDict):
+        current: float
 
     def __init__(
         self,
         initial_gain: float,
         initial_current: float,
     ) -> None:
         """Initialise the Femto device class.
 
         Args:
             initial_gain (Optional[float]): The initial amplified difference between \
                 the input and output signals. Defaults to 2.5.
             initial_current (Optional[float]): The input signal current. \
                 Defaults to 0.0.
         """
-        self.gain: float = initial_gain
-        self._current: float = initial_current
+        self.gain = initial_gain
+        self._current = initial_current
+        self._output_current = initial_current * initial_gain
 
     def set_gain(self, gain: float) -> None:
         """Sets a new amplified difference between the input and output signals.
 
         Args:
             gain (float): The amplified difference between the input and output signals.
         """
@@ -84,22 +86,26 @@
 
 
 class FemtoAdapter(EpicsAdapter):
     """The adapter for the Femto device."""
 
     device: FemtoDevice
 
+    def __init__(self, device: FemtoDevice) -> None:
+        super().__init__()
+        self.device = device
+
     async def callback(self, value) -> None:
         """Device callback function.
 
         Args:
             value (float): The value to set the gain to.
         """
         self.device.set_gain(value)
-        await self.raise_interrupt()
+        await self.interrupt()
 
     def on_db_load(self) -> None:
         """Customises records that have been loaded in to suit the simulation."""
         builder.aOut(
             "GAIN", initial_value=self.device.get_gain(), on_update=self.callback
         )
         self.link_input_on_interrupt(builder.aIn("GAIN_RBV"), self.device.get_gain)
```

### Comparing `tickit-devices-0.2.0/src/tickit_devices/pneumatic/pneumatic.py` & `tickit-devices-0.3.0/src/tickit_devices/pneumatic/pneumatic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from typing import TypedDict
 
 from softioc import builder
-from tickit.adapters.epicsadapter import EpicsAdapter
+from tickit.adapters.epics import EpicsAdapter
 from tickit.core.device import Device, DeviceUpdate
 from tickit.core.typedefs import SimTime
 
 
 class PneumaticDevice(Device):
     """Pneumatic Device with movement controls."""
 
+    class Inputs(TypedDict):
+        ...
+
     #: A typed mapping containing the current output value
-    Outputs: TypedDict = TypedDict("Outputs", {"output": float})
+    class Outputs(TypedDict):
+        output: float
 
     def __init__(
         self,
         initial_speed: float,
         initial_state: bool,
     ) -> None:
         """Initialise a Pneumatic object."""
@@ -74,22 +78,26 @@
     """An adapter for the Pneumatic class.
 
     Connects the device to an external messaging protocol.
     """
 
     device: PneumaticDevice
 
+    def __init__(self, device: PneumaticDevice) -> None:
+        super().__init__()
+        self.device = device
+
     async def callback(self, value) -> None:
         """Set the state of the device and await a response.
 
         Args:
             value (bool): The value to set the state to.
         """
         self.device.set_state()
-        await self.raise_interrupt()
+        await self.interrupt()
 
     def on_db_load(self):
         """Adds a record of the current state to the mapping of interrupting records."""
         builder.boolOut("FILTER", initial_value=False, on_update=self.callback)
         self.link_input_on_interrupt(
             builder.boolIn("FILTER_RBV"), self.device.get_state
         )
```

### Comparing `tickit-devices-0.2.0/src/tickit_devices/synchrotron/db_files/MSTAT.db` & `tickit-devices-0.3.0/src/tickit_devices/synchrotron/db_files/MSTAT.db`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/src/tickit_devices/synchrotron/synchrotron_current.py` & `tickit-devices-0.3.0/src/tickit_devices/synchrotron/synchrotron_current.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import pathlib
 from typing import Optional, TypedDict
 
 import pydantic.v1.dataclasses
 from softioc import builder
-from tickit.adapters.composed import ComposedAdapter
-from tickit.adapters.epicsadapter import EpicsAdapter
-from tickit.adapters.interpreters.command import CommandInterpreter, RegexCommand
-from tickit.adapters.servers.tcp import TcpServer
-from tickit.core.adapter import Server
+from tickit.adapters.epics import EpicsAdapter
+from tickit.adapters.io import EpicsIo, TcpIo
+from tickit.adapters.specifications import RegexCommand
+from tickit.adapters.tcp import CommandAdapter
+from tickit.core.adapter import AdapterContainer
 from tickit.core.components.component import Component, ComponentConfig
 from tickit.core.components.device_simulation import DeviceSimulation
 from tickit.core.device import Device, DeviceUpdate
 from tickit.core.typedefs import SimTime
 from tickit.utils.byte_format import ByteFormat
 
 
@@ -21,17 +21,20 @@
     This SynchrotronCurrentDevice simulates only a single signal that can be read,
     the beam current.The real world pv for this current is SR-DI-DCCT-01:SIGNAL.
 
     The signal is read via and epics adapter, and set using a tcp adapter.
     """
 
     #: An empty typed mapping of device inputs
-    Inputs: TypedDict = TypedDict("Inputs", {})
+    class Inputs(TypedDict):
+        ...
+
     #: A typed mapping containing the current output value
-    Outputs: TypedDict = TypedDict("Outputs", {"current": float})
+    class Outputs(TypedDict):
+        current: float
 
     def __init__(
         self,
         initial_current: Optional[float],
         callback_period: int = int(1e9),
         countdown: float = 600.0,
         fill_time: float = 15.0,
@@ -104,33 +107,23 @@
         )
 
     def get_current(self) -> float:
         """Beam current getter for the epics adapter."""
         return self.beam_current
 
 
-class SynchrotronCurrentTCPAdapter(ComposedAdapter):
+class SynchrotronCurrentTCPAdapter(CommandAdapter):
     """A TCP adapter to set a SynchrotronCurrentDevice PV values."""
 
     device: SynchrotronCurrentDevice
+    _byte_format: ByteFormat = ByteFormat(b"%b\r\n")
 
-    def __init__(
-        self,
-        server: Server,
-    ) -> None:
-        """Instantiates current adapter TcpServer with configured host and port.
-
-        Args:
-            server (Server): The immutable data container used to configure a
-                server.
-        """
-        super().__init__(
-            server,
-            CommandInterpreter(),
-        )
+    def __init__(self, device: SynchrotronCurrentDevice) -> None:
+        super().__init__()
+        self.device = device
 
     @RegexCommand(r"C=(\d+\.?\d*)", interrupt=True, format="utf-8")
     async def set_beam_current(self, value: float) -> None:
         """Regex string command that sets the value of beam_current.
 
         Args:
             value (int): The new value of beam_current.
@@ -148,38 +141,53 @@
 
 
 class SynchrotronCurrentEpicsAdapter(EpicsAdapter):
     """Epics adapter for reading device current as a PV through channel access."""
 
     device: SynchrotronCurrentDevice
 
+    def __init__(self, device: SynchrotronCurrentDevice) -> None:
+        super().__init__()
+        self.device = device
+
     def on_db_load(self) -> None:
         """Link loaded in record with getter for device."""
         self.link_input_on_interrupt(builder.aIn("SIGNAL"), self.device.get_current)
 
 
 @pydantic.v1.dataclasses.dataclass
 class SynchrotronCurrent(ComponentConfig):
     """Synchrotron current component."""
 
     initial_current: Optional[float]
     callback_period: int = int(1e9)
     host: str = "localhost"
     port: int = 25565
-    format: ByteFormat = ByteFormat(b"%b\r\n")
     db_file: str = str(pathlib.Path(__file__).parent.absolute() / "db_files/DCCT.db")
     ioc_name: str = "SR-DI-DCCT-01"
 
     def __call__(self) -> Component:  # noqa: D102
-        return DeviceSimulation(
-            name=self.name,
-            device=SynchrotronCurrentDevice(
-                self.initial_current,
-                callback_period=self.callback_period,
+        device = SynchrotronCurrentDevice(
+            self.initial_current,
+            callback_period=self.callback_period,
+        )
+        adapters = [
+            AdapterContainer(
+                SynchrotronCurrentTCPAdapter(device),
+                TcpIo(
+                    self.host,
+                    self.port,
+                ),
             ),
-            adapters=[
-                SynchrotronCurrentTCPAdapter(
-                    TcpServer(self.host, self.port, self.format)
+            AdapterContainer(
+                SynchrotronCurrentEpicsAdapter(device),
+                EpicsIo(
+                    self.ioc_name,
+                    self.db_file,
                 ),
-                SynchrotronCurrentEpicsAdapter(self.ioc_name, self.db_file),
-            ],
+            ),
+        ]
+        return DeviceSimulation(
+            name=self.name,
+            device=device,
+            adapters=adapters,
         )
```

### Comparing `tickit-devices-0.2.0/src/tickit_devices/synchrotron/synchrotron_machine.py` & `tickit-devices-0.3.0/src/tickit_devices/synchrotron/synchrotron_machine.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 import pathlib
 from typing import TypedDict
 
 import pydantic.v1.dataclasses
 from softioc import builder
-from tickit.adapters.composed import ComposedAdapter
-from tickit.adapters.epicsadapter import EpicsAdapter
-from tickit.adapters.interpreters.command import CommandInterpreter, RegexCommand
-from tickit.adapters.servers.tcp import TcpServer
-from tickit.core.adapter import Server
+from tickit.adapters.epics import EpicsAdapter
+from tickit.adapters.io import EpicsIo, TcpIo
+from tickit.adapters.specifications import RegexCommand
+from tickit.adapters.tcp import CommandAdapter
+from tickit.core.adapter import AdapterContainer
 from tickit.core.components.component import Component, ComponentConfig
 from tickit.core.components.device_simulation import DeviceSimulation
 from tickit.core.device import Device, DeviceUpdate
 from tickit.core.typedefs import SimTime
 from tickit.utils.byte_format import ByteFormat
 
 
 class SynchrotronMachineStatusDevice(Device):
     """Device to simulate the machine status records from the synchrotron.
 
     The signal is read via an epics adapter, and set using a tcp adapter.
     """
 
-    #: An empty typed mapping of device inputs
-    Inputs: TypedDict = TypedDict("Inputs", {})
-    #: A typed mapping containing the current output value
-    Outputs: TypedDict = TypedDict(
-        "Outputs",
-        {
-            "mode": int,
-            "user_countdown": float,
-            "beam_energy": float,
-        },
-    )
+    class Inputs(TypedDict):
+        ...
+
+    class Outputs(TypedDict):
+        mode: int
+        user_countdown: float
+        beam_energy: float
 
     def __init__(
         self,
         initial_mode: int,
         initial_countdown: float,
         initial_energy: float,
     ) -> None:
@@ -84,33 +80,23 @@
         return self.user_countdown
 
     def get_beam_energy(self) -> float:
         """Return value of beam energy, required for epics adapter."""
         return self.beam_energy
 
 
-class SynchrotronMachineStatusTCPAdapter(ComposedAdapter):
+class SynchrotronMachineStatusTCPAdapter(CommandAdapter):
     """A TCP adapter to set a SynchrotronMachineStatusDevice PV values."""
 
     device: SynchrotronMachineStatusDevice
+    _byte_format: ByteFormat = ByteFormat(b"%b\r\n")
 
-    def __init__(
-        self,
-        server: Server,
-    ) -> None:
-        """Synchrotron adapter, instantiates TcpServer with configured host and port.
-
-        Args:
-            server (Server): The immutable data container used to configure a
-                server.
-        """
-        super().__init__(
-            server,
-            CommandInterpreter(),
-        )
+    def __init__(self, device: SynchrotronMachineStatusDevice) -> None:
+        super().__init__()
+        self.device = device
 
     @RegexCommand(r"mode=([0-7])", interrupt=True, format="utf-8")
     async def set_synchrotron_mode(self, value: int) -> None:
         """Regex string command to set the value of synchrotron_mode.
 
         Args:
             value (int): The new value of synchrotron mode in digits 0-7.
@@ -166,14 +152,18 @@
 
 
 class SynchrotronMachineStatusEpicsAdapter(EpicsAdapter):
     """Epics adapter for reading device values as a PV through channel access."""
 
     device: SynchrotronMachineStatusDevice
 
+    def __init__(self, device: SynchrotronMachineStatusDevice) -> None:
+        super().__init__()
+        self.device = device
+
     def on_db_load(self) -> None:
         """Link epics records with getters for device.
 
         The MODE record is loaded via db, the other two are created here.
         """
         self.link_input_on_interrupt(builder.mbbIn("MODE"), self.device.get_mode)
         self.link_input_on_interrupt(
@@ -190,26 +180,37 @@
     """Synchrotron Machine status component."""
 
     initial_mode: int = 4
     initial_countdown: float = 100000
     initial_energy: float = 3.0
     host: str = "localhost"
     port: int = 25565
-    format: ByteFormat = ByteFormat(b"%b\r\n")
     db_file: str = str(pathlib.Path(__file__).parent.absolute() / "db_files/MSTAT.db")
     ioc_name: str = "CS-CS-MSTAT-01"
 
     def __call__(self) -> Component:  # noqa: D102
-        return DeviceSimulation(
-            name=self.name,
-            device=SynchrotronMachineStatusDevice(
-                self.initial_mode,
-                self.initial_countdown,
-                self.initial_energy,
+        device = SynchrotronMachineStatusDevice(
+            self.initial_mode,
+            self.initial_countdown,
+            self.initial_energy,
+        )
+        adapters = [
+            AdapterContainer(
+                SynchrotronMachineStatusTCPAdapter(device),
+                TcpIo(
+                    self.host,
+                    self.port,
+                ),
             ),
-            adapters=[
-                SynchrotronMachineStatusTCPAdapter(
-                    TcpServer(self.host, self.port, self.format)
+            AdapterContainer(
+                SynchrotronMachineStatusEpicsAdapter(device),
+                EpicsIo(
+                    self.ioc_name,
+                    self.db_file,
                 ),
-                SynchrotronMachineStatusEpicsAdapter(self.ioc_name, self.db_file),
-            ],
+            ),
+        ]
+        return DeviceSimulation(
+            name=self.name,
+            device=device,
+            adapters=adapters,
         )
```

### Comparing `tickit-devices-0.2.0/src/tickit_devices/synchrotron/synchrotron_topup.py` & `tickit-devices-0.3.0/src/tickit_devices/synchrotron/synchrotron_topup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 import pathlib
 from typing import TypedDict
 
 import pydantic.v1.dataclasses
 from softioc import builder
-from tickit.adapters.composed import ComposedAdapter
-from tickit.adapters.epicsadapter import EpicsAdapter
-from tickit.adapters.interpreters.command import CommandInterpreter, RegexCommand
-from tickit.adapters.servers.tcp import TcpServer
-from tickit.core.adapter import Server
+from tickit.adapters.epics import EpicsAdapter
+from tickit.adapters.io import EpicsIo, TcpIo
+from tickit.adapters.specifications import RegexCommand
+from tickit.adapters.tcp import CommandAdapter
+from tickit.core.adapter import AdapterContainer
 from tickit.core.components.component import Component, ComponentConfig
 from tickit.core.components.device_simulation import DeviceSimulation
 from tickit.core.device import Device, DeviceUpdate
 from tickit.core.typedefs import SimTime
 from tickit.utils.byte_format import ByteFormat
 
 
 class SynchrotronTopUpDevice(Device):
     """Device to simulate the top up records from the synchrotron.
 
     The signal is read via an epics adapter, and set using a tcp adapter.
     """
 
-    #: An empty typed mapping of device inputs
-    Inputs: TypedDict = TypedDict("Inputs", {"current": float})
-    #: A typed mapping containing the current output value
-    Outputs: TypedDict = TypedDict(
-        "Outputs",
-        {
-            "countdown": float,
-            "end_countdown": float,
-        },
-    )
+    class Inputs(TypedDict):
+        current: float
+
+    class Outputs(TypedDict):
+        countdown: float
+        end_countdown: float
 
     def __init__(
         self,
         initial_countdown: float = 600.0,
         initial_end_countdown: float = 620.0,
         callback_period: int = int(1e9),
         last_current: float = 300.0,
@@ -129,33 +125,23 @@
         return self.countdown
 
     def get_end_countdown(self) -> float:
         """Return value of end_countdown, required for epics adapter."""
         return self.end_countdown
 
 
-class SynchrotronTopUpTCPAdapter(ComposedAdapter):
+class SynchrotronTopUpTCPAdapter(CommandAdapter):
     """A TCP adapter to set a SynchrotronTopUpDevice PV values."""
 
     device: SynchrotronTopUpDevice
+    _byte_format: ByteFormat = ByteFormat(b"%b\r\n")
 
-    def __init__(
-        self,
-        server: Server,
-    ) -> None:
-        """Synchrotron adapter, instantiates TcpServer with configured host and port.
-
-        Args:
-            server (Server): The immutable data container used to configure a
-                server.
-        """
-        super().__init__(
-            server,
-            CommandInterpreter(),
-        )
+    def __init__(self, device: SynchrotronTopUpDevice) -> None:
+        super().__init__()
+        self.device = device
 
     @RegexCommand(r"CD=(\d+\.?\d*)", interrupt=True, format="utf-8")
     async def set_countdown(self, value: float) -> None:
         """Regex string command to set the value of countdown.
 
         Args:
             value (int): The new value of countdown.
@@ -191,14 +177,18 @@
 
 
 class SynchrotronTopUpEpicsAdapter(EpicsAdapter):
     """Epics adapter for reading device values as a PV through channel access."""
 
     device: SynchrotronTopUpDevice
 
+    def __init__(self, device: SynchrotronTopUpDevice) -> None:
+        super().__init__()
+        self.device = device
+
     def on_db_load(self) -> None:
         """Link epics records with getters for device."""
         self.link_input_on_interrupt(
             builder.aIn("COUNTDOWN"), self.device.get_countdown
         )
         self.link_input_on_interrupt(
             builder.aIn("ENDCOUNTDN"),
@@ -211,26 +201,37 @@
     """Synchrotron top up status component."""
 
     initial_countdown: float = 600
     initial_end_countdown: float = 620
     callback_period: int = int(1e9)
     host: str = "localhost"
     port: int = 25565
-    format: ByteFormat = ByteFormat(b"%b\r\n")
     db_file: str = str(pathlib.Path(__file__).parent.absolute() / "db_files/FILL.db")
     ioc_name: str = "SR-CS-FILL-01"
 
     def __call__(self) -> Component:  # noqa: D102
-        return DeviceSimulation(
-            name=self.name,
-            device=SynchrotronTopUpDevice(
-                self.initial_countdown,
-                self.initial_end_countdown,
-                callback_period=self.callback_period,
+        device = SynchrotronTopUpDevice(
+            self.initial_countdown,
+            self.initial_end_countdown,
+            callback_period=self.callback_period,
+        )
+        adapters = [
+            AdapterContainer(
+                SynchrotronTopUpTCPAdapter(device),
+                TcpIo(
+                    self.host,
+                    self.port,
+                ),
             ),
-            adapters=[
-                SynchrotronTopUpTCPAdapter(
-                    TcpServer(self.host, self.port, self.format)
+            AdapterContainer(
+                SynchrotronTopUpEpicsAdapter(device),
+                EpicsIo(
+                    self.ioc_name,
+                    self.db_file,
                 ),
-                SynchrotronTopUpEpicsAdapter(self.ioc_name, self.db_file),
-            ],
+            ),
+        ]
+        return DeviceSimulation(
+            name=self.name,
+            device=device,
+            adapters=adapters,
         )
```

### Comparing `tickit-devices-0.2.0/src/tickit_devices.egg-info/PKG-INFO` & `tickit-devices-0.3.0/src/tickit_devices.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tickit-devices
-Version: 0.2.0
+Version: 0.3.0
 Summary: Devices for tickit, an event-based device simulation framework
 Author-email: Abigail Emery <abigail.emery@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `tickit-devices-0.2.0/src/tickit_devices.egg-info/SOURCES.txt` & `tickit-devices-0.3.0/src/tickit_devices.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/tests/conftest.py` & `tickit-devices-0.3.0/tests/conftest.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import sys
 from subprocess import PIPE, STDOUT, Popen
 
 import pytest
 import pytest_asyncio
 from tickit.core.management.event_router import InverseWiring
 from tickit.core.management.schedulers.master import MasterScheduler
-from tickit.core.runner import run_all_forever
 from tickit.core.state_interfaces.state_interface import get_interface
 from tickit.utils.configuration.loading import read_configs
 
 
 # https://docs.pytest.org/en/latest/example/parametrize.html#indirect-parametrization
 @pytest.fixture
 def tickit_process(request):
@@ -37,17 +36,20 @@
 async def tickit_task(request):
     """Task that runs ``tickit all <config_path>``."""
     config_path: str = request.param
     configs = read_configs(config_path)
     inverse_wiring = InverseWiring.from_component_configs(configs)
     scheduler = MasterScheduler(inverse_wiring, *get_interface("internal"))
     t = asyncio.Task(
-        run_all_forever(
-            [c().run_forever(*get_interface("internal")) for c in configs]
-            + [scheduler.run_forever()]
+        asyncio.wait(
+            [
+                asyncio.create_task(c().run_forever(*get_interface("internal")))
+                for c in configs
+            ]
+            + [asyncio.create_task(scheduler.run_forever())]
         )
     )
     # TODO: would like to await all_servers_running() here
     await asyncio.sleep(0.5)
     yield t
     tasks = asyncio.tasks.all_tasks()
     for task in tasks:
```

### Comparing `tickit-devices-0.2.0/tests/cryostream/test_base.py` & `tickit-devices-0.3.0/tests/cryostream/test_base.py`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/tests/cryostream/test_cryostream.py` & `tickit-devices-0.3.0/tests/cryostream/test_cryostream.py`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/tests/eiger/test_eiger.py` & `tickit-devices-0.3.0/tests/eiger/test_eiger.py`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/tests/eiger/test_eiger_settings.py` & `tickit-devices-0.3.0/tests/eiger/test_eiger_settings.py`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/tests/eiger/test_eiger_stream.py` & `tickit-devices-0.3.0/tests/eiger/test_eiger_stream.py`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/tests/eiger/test_eiger_system.py` & `tickit-devices-0.3.0/tests/eiger/test_eiger_system.py`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/tests/femto/test_femto.py` & `tickit-devices-0.3.0/tests/femto/test_femto.py`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/tests/multi/test_multi_device.py` & `tickit-devices-0.3.0/tests/multi/test_multi_device.py`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/tests/pneumatic/test_pneumatic.py` & `tickit-devices-0.3.0/tests/pneumatic/test_pneumatic.py`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/tests/synchrotron/test_synchrotron_current.py` & `tickit-devices-0.3.0/tests/synchrotron/test_synchrotron_current.py`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/tests/synchrotron/test_synchrotron_machine.py` & `tickit-devices-0.3.0/tests/synchrotron/test_synchrotron_machine.py`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.2.0/tests/synchrotron/test_synchrotron_topup.py` & `tickit-devices-0.3.0/tests/synchrotron/test_synchrotron_topup.py`

 * *Files identical despite different names*

