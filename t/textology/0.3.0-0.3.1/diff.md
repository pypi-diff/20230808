# Comparing `tmp/textology-0.3.0.tar.gz` & `tmp/textology-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textology-0.3.0.tar", last modified: Sun Aug  6 20:25:34 2023, max compression
+gzip compressed data, was "textology-0.3.1.tar", last modified: Mon Aug  7 22:26:32 2023, max compression
```

## Comparing `textology-0.3.0.tar` & `textology-0.3.1.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-08-06 20:25:34.525037 textology-0.3.0/
--rw-r--r--   0 dfritz     (502) staff       (20)     1068 2023-07-01 18:44:36.000000 textology-0.3.0/LICENSE
--rw-r--r--   0 dfritz     (502) staff       (20)       97 2023-07-08 19:46:35.000000 textology-0.3.0/MANIFEST.in
--rw-r--r--   0 dfritz     (502) staff       (20)    15590 2023-08-06 20:25:34.525231 textology-0.3.0/PKG-INFO
--rw-r--r--   0 dfritz     (502) staff       (20)    14228 2023-08-06 20:14:59.000000 textology-0.3.0/README.md
--rw-r--r--   0 dfritz     (502) staff       (20)       34 2023-07-30 17:52:28.000000 textology-0.3.0/requirements-dev.txt
--rw-r--r--   0 dfritz     (502) staff       (20)      182 2023-08-06 20:14:59.000000 textology-0.3.0/requirements-full-dev.txt
--rw-r--r--   0 dfritz     (502) staff       (20)       16 2023-07-30 17:52:28.000000 textology-0.3.0/requirements.txt
--rw-r--r--   0 dfritz     (502) staff       (20)     1667 2023-08-06 20:25:34.526508 textology-0.3.0/setup.cfg
--rw-r--r--   0 dfritz     (502) staff       (20)     3225 2023-07-08 19:46:35.000000 textology-0.3.0/setup.py
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-08-06 20:25:34.492687 textology-0.3.0/textology/
--rw-r--r--   0 dfritz     (502) staff       (20)       69 2023-08-06 20:22:10.000000 textology-0.3.0/textology/__init__.py
--rw-r--r--   0 dfritz     (502) staff       (20)    17290 2023-08-06 20:14:59.000000 textology-0.3.0/textology/apps.py
--rw-r--r--   0 dfritz     (502) staff       (20)     6551 2023-08-06 20:14:59.000000 textology-0.3.0/textology/dash_compat.py
--rw-r--r--   0 dfritz     (502) staff       (20)     2772 2023-07-04 21:19:10.000000 textology-0.3.0/textology/history.py
--rw-r--r--   0 dfritz     (502) staff       (20)      492 2023-07-04 21:19:10.000000 textology-0.3.0/textology/logging.py
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-08-06 20:25:34.501345 textology-0.3.0/textology/observers/
--rw-r--r--   0 dfritz     (502) staff       (20)      885 2023-07-24 01:09:35.000000 textology-0.3.0/textology/observers/__init__.py
--rw-r--r--   0 dfritz     (502) staff       (20)     6230 2023-07-24 01:09:35.000000 textology-0.3.0/textology/observers/_dependencies.py
--rw-r--r--   0 dfritz     (502) staff       (20)      458 2023-07-22 18:13:02.000000 textology-0.3.0/textology/observers/_exceptions.py
--rw-r--r--   0 dfritz     (502) staff       (20)    31303 2023-08-06 20:14:59.000000 textology-0.3.0/textology/observers/_managers.py
--rw-r--r--   0 dfritz     (502) staff       (20)     6499 2023-08-06 20:14:59.000000 textology-0.3.0/textology/pages.py
--rw-r--r--   0 dfritz     (502) staff       (20)    16541 2023-07-16 17:16:06.000000 textology-0.3.0/textology/pytest_utils.py
--rw-r--r--   0 dfritz     (502) staff       (20)    17773 2023-07-16 17:16:06.000000 textology-0.3.0/textology/router.py
--rw-r--r--   0 dfritz     (502) staff       (20)    45559 2023-07-24 01:09:35.000000 textology-0.3.0/textology/test-template.html
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-08-06 20:25:34.509510 textology-0.3.0/textology/widgets/
--rw-r--r--   0 dfritz     (502) staff       (20)     2653 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/__init__.py
--rw-r--r--   0 dfritz     (502) staff       (20)     2176 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_button.py
--rw-r--r--   0 dfritz     (502) staff       (20)    13679 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_extensions.py
--rw-r--r--   0 dfritz     (502) staff       (20)    12301 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_horizontal_menus.py
--rw-r--r--   0 dfritz     (502) staff       (20)     2625 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_list_item.py
--rw-r--r--   0 dfritz     (502) staff       (20)     2407 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_list_item_header.py
--rw-r--r--   0 dfritz     (502) staff       (20)     2611 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_list_item_meta.py
--rw-r--r--   0 dfritz     (502) staff       (20)     5350 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_list_view.py
--rw-r--r--   0 dfritz     (502) staff       (20)     8995 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_location.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1955 2023-07-04 21:18:52.000000 textology-0.3.0/textology/widgets/_modal_dialog.py
--rw-r--r--   0 dfritz     (502) staff       (20)     2263 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_store.py
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-08-06 20:25:34.524591 textology-0.3.0/textology/widgets/_textual/
--rw-r--r--   0 dfritz     (502) staff       (20)      104 2023-07-30 17:52:28.000000 textology-0.3.0/textology/widgets/_textual/__init__.py
--rw-r--r--   0 dfritz     (502) staff       (20)      294 2023-07-30 17:52:28.000000 textology-0.3.0/textology/widgets/_textual/_checkbox.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1651 2023-07-30 17:52:28.000000 textology-0.3.0/textology/widgets/_textual/_containers.py
--rw-r--r--   0 dfritz     (502) staff       (20)     2064 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_content_switcher.py
--rw-r--r--   0 dfritz     (502) staff       (20)     3190 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_data_table.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1770 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_directory_tree.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1095 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_footer.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1561 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_header.py
--rw-r--r--   0 dfritz     (502) staff       (20)      291 2023-07-30 17:52:28.000000 textology-0.3.0/textology/widgets/_textual/_label.py
--rw-r--r--   0 dfritz     (502) staff       (20)      263 2023-07-30 17:52:28.000000 textology-0.3.0/textology/widgets/_textual/_loading_indicator.py
--rw-r--r--   0 dfritz     (502) staff       (20)     3623 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_markdown.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1723 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_option_list.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1540 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_pretty.py
--rw-r--r--   0 dfritz     (502) staff       (20)     2085 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_progress_bar.py
--rw-r--r--   0 dfritz     (502) staff       (20)      308 2023-07-30 17:52:28.000000 textology-0.3.0/textology/widgets/_textual/_radio_button.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1677 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_radio_set.py
--rw-r--r--   0 dfritz     (502) staff       (20)     2137 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_select.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1952 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_selection_list.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1926 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_sparkline.py
--rw-r--r--   0 dfritz     (502) staff       (20)      354 2023-07-30 17:52:28.000000 textology-0.3.0/textology/widgets/_textual/_static.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1742 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_switch.py
--rw-r--r--   0 dfritz     (502) staff       (20)     3437 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_tabbed_content.py
--rw-r--r--   0 dfritz     (502) staff       (20)     2971 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_tabs.py
--rw-r--r--   0 dfritz     (502) staff       (20)     2633 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_text_input.py
--rw-r--r--   0 dfritz     (502) staff       (20)     2244 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_text_log.py
--rw-r--r--   0 dfritz     (502) staff       (20)      234 2023-07-30 17:52:28.000000 textology-0.3.0/textology/widgets/_textual/_tooltip.py
--rw-r--r--   0 dfritz     (502) staff       (20)     1873 2023-08-06 20:14:59.000000 textology-0.3.0/textology/widgets/_textual/_tree.py
-drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-08-06 20:25:34.497838 textology-0.3.0/textology.egg-info/
--rw-r--r--   0 dfritz     (502) staff       (20)    15590 2023-08-06 20:25:34.000000 textology-0.3.0/textology.egg-info/PKG-INFO
--rw-r--r--   0 dfritz     (502) staff       (20)     2088 2023-08-06 20:25:34.000000 textology-0.3.0/textology.egg-info/SOURCES.txt
--rw-r--r--   0 dfritz     (502) staff       (20)        1 2023-08-06 20:25:34.000000 textology-0.3.0/textology.egg-info/dependency_links.txt
--rw-r--r--   0 dfritz     (502) staff       (20)      317 2023-08-06 20:25:34.000000 textology-0.3.0/textology.egg-info/requires.txt
--rw-r--r--   0 dfritz     (502) staff       (20)       10 2023-08-06 20:25:34.000000 textology-0.3.0/textology.egg-info/top_level.txt
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-08-07 22:26:32.655206 textology-0.3.1/
+-rw-r--r--   0 dfritz     (502) staff       (20)     1068 2023-07-01 18:44:36.000000 textology-0.3.1/LICENSE
+-rw-r--r--   0 dfritz     (502) staff       (20)       97 2023-07-08 19:46:35.000000 textology-0.3.1/MANIFEST.in
+-rw-r--r--   0 dfritz     (502) staff       (20)    15590 2023-08-07 22:26:32.655511 textology-0.3.1/PKG-INFO
+-rw-r--r--   0 dfritz     (502) staff       (20)    14228 2023-08-06 20:14:59.000000 textology-0.3.1/README.md
+-rw-r--r--   0 dfritz     (502) staff       (20)       34 2023-07-30 17:52:28.000000 textology-0.3.1/requirements-dev.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)      182 2023-08-06 20:14:59.000000 textology-0.3.1/requirements-full-dev.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)       16 2023-08-06 20:51:25.000000 textology-0.3.1/requirements.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)     1667 2023-08-07 22:26:32.657539 textology-0.3.1/setup.cfg
+-rw-r--r--   0 dfritz     (502) staff       (20)     3225 2023-07-08 19:46:35.000000 textology-0.3.1/setup.py
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-08-07 22:26:32.622188 textology-0.3.1/textology/
+-rw-r--r--   0 dfritz     (502) staff       (20)       69 2023-08-07 22:25:07.000000 textology-0.3.1/textology/__init__.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    17290 2023-08-06 20:14:59.000000 textology-0.3.1/textology/apps.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     6551 2023-08-06 20:14:59.000000 textology-0.3.1/textology/dash_compat.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2772 2023-07-04 21:19:10.000000 textology-0.3.1/textology/history.py
+-rw-r--r--   0 dfritz     (502) staff       (20)      492 2023-07-04 21:19:10.000000 textology-0.3.1/textology/logging.py
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-08-07 22:26:32.629516 textology-0.3.1/textology/observers/
+-rw-r--r--   0 dfritz     (502) staff       (20)      885 2023-07-24 01:09:35.000000 textology-0.3.1/textology/observers/__init__.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     6230 2023-07-24 01:09:35.000000 textology-0.3.1/textology/observers/_dependencies.py
+-rw-r--r--   0 dfritz     (502) staff       (20)      458 2023-07-22 18:13:02.000000 textology-0.3.1/textology/observers/_exceptions.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    31303 2023-08-06 20:14:59.000000 textology-0.3.1/textology/observers/_managers.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     6499 2023-08-06 20:14:59.000000 textology-0.3.1/textology/pages.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    16541 2023-07-16 17:16:06.000000 textology-0.3.1/textology/pytest_utils.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    17773 2023-07-16 17:16:06.000000 textology-0.3.1/textology/router.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    45559 2023-07-24 01:09:35.000000 textology-0.3.1/textology/test-template.html
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-08-07 22:26:32.637669 textology-0.3.1/textology/widgets/
+-rw-r--r--   0 dfritz     (502) staff       (20)     2684 2023-08-06 20:45:46.000000 textology-0.3.1/textology/widgets/__init__.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2176 2023-08-06 20:14:59.000000 textology-0.3.1/textology/widgets/_button.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    13679 2023-08-06 20:14:59.000000 textology-0.3.1/textology/widgets/_extensions.py
+-rw-r--r--   0 dfritz     (502) staff       (20)    12301 2023-08-06 20:14:59.000000 textology-0.3.1/textology/widgets/_horizontal_menus.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2625 2023-08-06 20:14:59.000000 textology-0.3.1/textology/widgets/_list_item.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2407 2023-08-06 20:14:59.000000 textology-0.3.1/textology/widgets/_list_item_header.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2611 2023-08-06 20:14:59.000000 textology-0.3.1/textology/widgets/_list_item_meta.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     5350 2023-08-06 20:14:59.000000 textology-0.3.1/textology/widgets/_list_view.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     8995 2023-08-06 20:14:59.000000 textology-0.3.1/textology/widgets/_location.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1955 2023-07-04 21:18:52.000000 textology-0.3.1/textology/widgets/_modal_dialog.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2263 2023-08-06 20:14:59.000000 textology-0.3.1/textology/widgets/_store.py
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-08-07 22:26:32.654532 textology-0.3.1/textology/widgets/_textual/
+-rw-r--r--   0 dfritz     (502) staff       (20)      104 2023-07-30 17:52:28.000000 textology-0.3.1/textology/widgets/_textual/__init__.py
+-rw-r--r--   0 dfritz     (502) staff       (20)      294 2023-07-30 17:52:28.000000 textology-0.3.1/textology/widgets/_textual/_checkbox.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1651 2023-07-30 17:52:28.000000 textology-0.3.1/textology/widgets/_textual/_containers.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2064 2023-08-06 20:14:59.000000 textology-0.3.1/textology/widgets/_textual/_content_switcher.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     3190 2023-08-06 20:14:59.000000 textology-0.3.1/textology/widgets/_textual/_data_table.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1770 2023-08-06 20:14:59.000000 textology-0.3.1/textology/widgets/_textual/_directory_tree.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1095 2023-08-06 20:14:59.000000 textology-0.3.1/textology/widgets/_textual/_footer.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1561 2023-08-06 20:14:59.000000 textology-0.3.1/textology/widgets/_textual/_header.py
+-rw-r--r--   0 dfritz     (502) staff       (20)      291 2023-07-30 17:52:28.000000 textology-0.3.1/textology/widgets/_textual/_label.py
+-rw-r--r--   0 dfritz     (502) staff       (20)      263 2023-07-30 17:52:28.000000 textology-0.3.1/textology/widgets/_textual/_loading_indicator.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1879 2023-08-06 20:46:25.000000 textology-0.3.1/textology/widgets/_textual/_log.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     3623 2023-08-06 20:14:59.000000 textology-0.3.1/textology/widgets/_textual/_markdown.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1723 2023-08-06 20:14:59.000000 textology-0.3.1/textology/widgets/_textual/_option_list.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1540 2023-08-06 20:14:59.000000 textology-0.3.1/textology/widgets/_textual/_pretty.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2085 2023-08-06 20:14:59.000000 textology-0.3.1/textology/widgets/_textual/_progress_bar.py
+-rw-r--r--   0 dfritz     (502) staff       (20)      308 2023-07-30 17:52:28.000000 textology-0.3.1/textology/widgets/_textual/_radio_button.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1677 2023-08-06 20:14:59.000000 textology-0.3.1/textology/widgets/_textual/_radio_set.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2244 2023-08-06 20:51:25.000000 textology-0.3.1/textology/widgets/_textual/_rich_log.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2137 2023-08-06 20:14:59.000000 textology-0.3.1/textology/widgets/_textual/_select.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1952 2023-08-06 20:14:59.000000 textology-0.3.1/textology/widgets/_textual/_selection_list.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1926 2023-08-06 20:14:59.000000 textology-0.3.1/textology/widgets/_textual/_sparkline.py
+-rw-r--r--   0 dfritz     (502) staff       (20)      354 2023-07-30 17:52:28.000000 textology-0.3.1/textology/widgets/_textual/_static.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1742 2023-08-06 20:14:59.000000 textology-0.3.1/textology/widgets/_textual/_switch.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     3437 2023-08-06 20:14:59.000000 textology-0.3.1/textology/widgets/_textual/_tabbed_content.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2971 2023-08-06 20:14:59.000000 textology-0.3.1/textology/widgets/_textual/_tabs.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     2633 2023-08-06 20:14:59.000000 textology-0.3.1/textology/widgets/_textual/_text_input.py
+-rw-r--r--   0 dfritz     (502) staff       (20)      234 2023-07-30 17:52:28.000000 textology-0.3.1/textology/widgets/_textual/_tooltip.py
+-rw-r--r--   0 dfritz     (502) staff       (20)     1873 2023-08-06 20:14:59.000000 textology-0.3.1/textology/widgets/_textual/_tree.py
+drwxr-xr-x   0 dfritz     (502) staff       (20)        0 2023-08-07 22:26:32.626867 textology-0.3.1/textology.egg-info/
+-rw-r--r--   0 dfritz     (502) staff       (20)    15590 2023-08-07 22:26:32.000000 textology-0.3.1/textology.egg-info/PKG-INFO
+-rw-r--r--   0 dfritz     (502) staff       (20)     2123 2023-08-07 22:26:32.000000 textology-0.3.1/textology.egg-info/SOURCES.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)        1 2023-08-07 22:26:32.000000 textology-0.3.1/textology.egg-info/dependency_links.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)      317 2023-08-07 22:26:32.000000 textology-0.3.1/textology.egg-info/requires.txt
+-rw-r--r--   0 dfritz     (502) staff       (20)       10 2023-08-07 22:26:32.000000 textology-0.3.1/textology.egg-info/top_level.txt
```

### Comparing `textology-0.3.0/LICENSE` & `textology-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/PKG-INFO` & `textology-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textology
-Version: 0.3.0
+Version: 0.3.1
 Summary: Textual extensions for creating Terminal User Interfaces
 Home-page: https://github.com/dfrtz/textology
 Author: David Fritz
 License: MIT
 Project-URL: Issue Tracker, https://github.com/dfrtz/textology/issues
 Project-URL: Source Code, https://github.com/dfrtz/textology
 Platform: MacOS
```

### Comparing `textology-0.3.0/README.md` & `textology-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/setup.cfg` & `textology-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/setup.py` & `textology-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/apps.py` & `textology-0.3.1/textology/apps.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/dash_compat.py` & `textology-0.3.1/textology/dash_compat.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/history.py` & `textology-0.3.1/textology/history.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/observers/__init__.py` & `textology-0.3.1/textology/observers/__init__.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/observers/_dependencies.py` & `textology-0.3.1/textology/observers/_dependencies.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/observers/_managers.py` & `textology-0.3.1/textology/observers/_managers.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/pages.py` & `textology-0.3.1/textology/pages.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/pytest_utils.py` & `textology-0.3.1/textology/pytest_utils.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/router.py` & `textology-0.3.1/textology/router.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/test-template.html` & `textology-0.3.1/textology/test-template.html`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/widgets/__init__.py` & `textology-0.3.1/textology/widgets/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,27 +33,28 @@
 from ._textual._content_switcher import ContentSwitcher
 from ._textual._data_table import DataTable
 from ._textual._directory_tree import DirectoryTree
 from ._textual._footer import Footer
 from ._textual._header import Header
 from ._textual._label import Label
 from ._textual._loading_indicator import LoadingIndicator
+from ._textual._log import Log
 from ._textual._markdown import Markdown
 from ._textual._markdown import MarkdownViewer
 from ._textual._option_list import OptionList
 from ._textual._pretty import Pretty
 from ._textual._progress_bar import ProgressBar
 from ._textual._radio_button import RadioButton
 from ._textual._radio_set import RadioSet
+from ._textual._rich_log import RichLog
 from ._textual._select import Select
 from ._textual._selection_list import SelectionList
 from ._textual._sparkline import Sparkline
 from ._textual._static import Static
 from ._textual._switch import Switch
 from ._textual._tabbed_content import TabbedContent
 from ._textual._tabbed_content import TabPane
 from ._textual._tabs import Tab
 from ._textual._tabs import Tabs
 from ._textual._text_input import TextInput
-from ._textual._text_log import TextLog
 from ._textual._tooltip import Tooltip
 from ._textual._tree import Tree
```

### Comparing `textology-0.3.0/textology/widgets/_button.py` & `textology-0.3.1/textology/widgets/_button.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/widgets/_extensions.py` & `textology-0.3.1/textology/widgets/_extensions.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/widgets/_horizontal_menus.py` & `textology-0.3.1/textology/widgets/_horizontal_menus.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/widgets/_list_item.py` & `textology-0.3.1/textology/widgets/_list_item.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/widgets/_list_item_header.py` & `textology-0.3.1/textology/widgets/_list_item_header.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/widgets/_list_item_meta.py` & `textology-0.3.1/textology/widgets/_list_item_meta.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/widgets/_list_view.py` & `textology-0.3.1/textology/widgets/_list_view.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/widgets/_location.py` & `textology-0.3.1/textology/widgets/_location.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/widgets/_modal_dialog.py` & `textology-0.3.1/textology/widgets/_modal_dialog.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/widgets/_store.py` & `textology-0.3.1/textology/widgets/_store.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/widgets/_textual/_containers.py` & `textology-0.3.1/textology/widgets/_textual/_containers.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/widgets/_textual/_content_switcher.py` & `textology-0.3.1/textology/widgets/_textual/_content_switcher.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/widgets/_textual/_data_table.py` & `textology-0.3.1/textology/widgets/_textual/_data_table.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/widgets/_textual/_directory_tree.py` & `textology-0.3.1/textology/widgets/_textual/_directory_tree.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/widgets/_textual/_footer.py` & `textology-0.3.1/textology/widgets/_textual/_footer.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/widgets/_textual/_header.py` & `textology-0.3.1/textology/widgets/_textual/_header.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/widgets/_textual/_markdown.py` & `textology-0.3.1/textology/widgets/_textual/_markdown.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/widgets/_textual/_option_list.py` & `textology-0.3.1/textology/widgets/_textual/_option_list.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/widgets/_textual/_pretty.py` & `textology-0.3.1/textology/widgets/_textual/_pretty.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/widgets/_textual/_progress_bar.py` & `textology-0.3.1/textology/widgets/_textual/_progress_bar.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/widgets/_textual/_radio_set.py` & `textology-0.3.1/textology/widgets/_textual/_radio_set.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/widgets/_textual/_select.py` & `textology-0.3.1/textology/widgets/_textual/_select.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/widgets/_textual/_selection_list.py` & `textology-0.3.1/textology/widgets/_textual/_selection_list.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/widgets/_textual/_sparkline.py` & `textology-0.3.1/textology/widgets/_textual/_sparkline.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/widgets/_textual/_switch.py` & `textology-0.3.1/textology/widgets/_textual/_switch.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/widgets/_textual/_tabbed_content.py` & `textology-0.3.1/textology/widgets/_textual/_tabbed_content.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/widgets/_textual/_tabs.py` & `textology-0.3.1/textology/widgets/_textual/_tabs.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/widgets/_textual/_text_input.py` & `textology-0.3.1/textology/widgets/_textual/_text_input.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology/widgets/_textual/_text_log.py` & `textology-0.3.1/textology/widgets/_textual/_rich_log.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""Extended Textual TextLog widget."""
+"""Extended Textual RichLog widget."""
 
 from typing import Any
 from typing import Callable
 
 from textual import events
 from textual import widgets
 
 from .._extensions import WidgetExtension
 
 
-class TextLog(WidgetExtension, widgets.TextLog):
+class RichLog(WidgetExtension, widgets.RichLog):
     """An extended widget for logging text."""
 
     def __init__(
         self,
         *,
         max_lines: int | None = None,
         min_width: int = 78,
@@ -25,15 +25,15 @@
         id: str | None = None,
         classes: str | None = None,
         disabled: bool = False,
         styles: dict[str, Any] | None = None,
         disabled_messages: list[type[events.Message]] | None = None,
         callbacks: dict[str, Callable] | None = None,
     ) -> None:
-        """Initialize a TextLog widget.
+        """Initialize a RichLog widget.
 
         Args:
             max_lines: Maximum number of lines in the log or `None` for no maximum.
             min_width: Minimum width of renderables.
             wrap: Enable word wrapping (default is off).
             highlight: Automatically highlight content.
             markup: Apply Rich console markup.
```

### Comparing `textology-0.3.0/textology/widgets/_textual/_tree.py` & `textology-0.3.1/textology/widgets/_textual/_tree.py`

 * *Files identical despite different names*

### Comparing `textology-0.3.0/textology.egg-info/PKG-INFO` & `textology-0.3.1/textology.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textology
-Version: 0.3.0
+Version: 0.3.1
 Summary: Textual extensions for creating Terminal User Interfaces
 Home-page: https://github.com/dfrtz/textology
 Author: David Fritz
 License: MIT
 Project-URL: Issue Tracker, https://github.com/dfrtz/textology/issues
 Project-URL: Source Code, https://github.com/dfrtz/textology
 Platform: MacOS
```

### Comparing `textology-0.3.0/textology.egg-info/SOURCES.txt` & `textology-0.3.1/textology.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -41,24 +41,25 @@
 textology/widgets/_textual/_content_switcher.py
 textology/widgets/_textual/_data_table.py
 textology/widgets/_textual/_directory_tree.py
 textology/widgets/_textual/_footer.py
 textology/widgets/_textual/_header.py
 textology/widgets/_textual/_label.py
 textology/widgets/_textual/_loading_indicator.py
+textology/widgets/_textual/_log.py
 textology/widgets/_textual/_markdown.py
 textology/widgets/_textual/_option_list.py
 textology/widgets/_textual/_pretty.py
 textology/widgets/_textual/_progress_bar.py
 textology/widgets/_textual/_radio_button.py
 textology/widgets/_textual/_radio_set.py
+textology/widgets/_textual/_rich_log.py
 textology/widgets/_textual/_select.py
 textology/widgets/_textual/_selection_list.py
 textology/widgets/_textual/_sparkline.py
 textology/widgets/_textual/_static.py
 textology/widgets/_textual/_switch.py
 textology/widgets/_textual/_tabbed_content.py
 textology/widgets/_textual/_tabs.py
 textology/widgets/_textual/_text_input.py
-textology/widgets/_textual/_text_log.py
 textology/widgets/_textual/_tooltip.py
 textology/widgets/_textual/_tree.py
```

