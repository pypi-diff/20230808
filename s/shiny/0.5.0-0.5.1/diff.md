# Comparing `tmp/shiny-0.5.0.tar.gz` & `tmp/shiny-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shiny-0.5.0.tar", last modified: Tue Aug  1 19:31:43 2023, max compression
+gzip compressed data, was "shiny-0.5.1.tar", last modified: Tue Aug  8 21:08:06 2023, max compression
```

## Comparing `shiny-0.5.0.tar` & `shiny-0.5.1.tar`

### file list

```diff
@@ -1,637 +1,637 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.323697 shiny-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-01 19:29:59.000000 shiny-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-08-01 19:29:59.000000 shiny-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-08-01 19:31:43.323697 shiny-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-08-01 19:29:59.000000 shiny-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.227696 shiny-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-08-01 19:29:59.000000 shiny-0.5.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-08-01 19:31:43.327697 shiny-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 19:29:59.000000 shiny-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.231696 shiny-0.5.0/shiny/
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14463 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/_autoreload.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/_datastructures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/_docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/_fileupload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/_hostenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/_launchbrowser.py
--rw-r--r--   0 runner    (1001) docker     (123)    14776 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/_shinyenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/_static.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/_typing_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13768 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.215696 shiny-0.5.0/shiny/api-examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.231696 shiny-0.5.0/shiny/api-examples/Calc/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/Calc/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.231696 shiny-0.5.0/shiny/api-examples/Effect/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/Effect/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.231696 shiny-0.5.0/shiny/api-examples/Module/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/Module/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.231696 shiny-0.5.0/shiny/api-examples/Progress/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/Progress/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.235696 shiny-0.5.0/shiny/api-examples/SafeException/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/SafeException/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.235696 shiny-0.5.0/shiny/api-examples/SilentCancelOutputException/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/SilentCancelOutputException/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.235696 shiny-0.5.0/shiny/api-examples/SilentException/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/SilentException/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.235696 shiny-0.5.0/shiny/api-examples/Value/
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/Value/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.235696 shiny-0.5.0/shiny/api-examples/close/
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/close/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.235696 shiny-0.5.0/shiny/api-examples/data_frame/
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/data_frame/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.235696 shiny-0.5.0/shiny/api-examples/download/
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/download/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/download/mtcars.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.235696 shiny-0.5.0/shiny/api-examples/download_button/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/download_button/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/download_button/mtcars.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.235696 shiny-0.5.0/shiny/api-examples/download_link/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/download_link/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/download_link/mtcars.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.235696 shiny-0.5.0/shiny/api-examples/dynamic_route/
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/dynamic_route/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.235696 shiny-0.5.0/shiny/api-examples/event/
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/event/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.235696 shiny-0.5.0/shiny/api-examples/file_reader/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/file_reader/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/file_reader/mtcars.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.235696 shiny-0.5.0/shiny/api-examples/include_css/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/include_css/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.235696 shiny-0.5.0/shiny/api-examples/include_css/css/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/include_css/css/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.235696 shiny-0.5.0/shiny/api-examples/include_javascript/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/include_javascript/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.239696 shiny-0.5.0/shiny/api-examples/include_javascript/js/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/include_javascript/js/app.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.239696 shiny-0.5.0/shiny/api-examples/input_action_button/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/input_action_button/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.239696 shiny-0.5.0/shiny/api-examples/input_action_link/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/input_action_link/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.239696 shiny-0.5.0/shiny/api-examples/input_checkbox/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/input_checkbox/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.239696 shiny-0.5.0/shiny/api-examples/input_checkbox_group/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/input_checkbox_group/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.239696 shiny-0.5.0/shiny/api-examples/input_date/
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/input_date/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.239696 shiny-0.5.0/shiny/api-examples/input_date_range/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/input_date_range/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.239696 shiny-0.5.0/shiny/api-examples/input_file/
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/input_file/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.239696 shiny-0.5.0/shiny/api-examples/input_numeric/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/input_numeric/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.239696 shiny-0.5.0/shiny/api-examples/input_password/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/input_password/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.239696 shiny-0.5.0/shiny/api-examples/input_radio_buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/input_radio_buttons/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.239696 shiny-0.5.0/shiny/api-examples/input_select/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/input_select/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.239696 shiny-0.5.0/shiny/api-examples/input_selectize/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/input_selectize/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.239696 shiny-0.5.0/shiny/api-examples/input_slider/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/input_slider/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.239696 shiny-0.5.0/shiny/api-examples/input_switch/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/input_switch/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.239696 shiny-0.5.0/shiny/api-examples/input_text/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/input_text/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.239696 shiny-0.5.0/shiny/api-examples/input_text_area/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/input_text_area/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.239696 shiny-0.5.0/shiny/api-examples/insert_ui/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/insert_ui/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.239696 shiny-0.5.0/shiny/api-examples/invalidate_later/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/invalidate_later/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.239696 shiny-0.5.0/shiny/api-examples/isolate/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/isolate/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.239696 shiny-0.5.0/shiny/api-examples/layout_sidebar/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/layout_sidebar/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.243696 shiny-0.5.0/shiny/api-examples/markdown/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/markdown/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.243696 shiny-0.5.0/shiny/api-examples/modal/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/modal/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.243696 shiny-0.5.0/shiny/api-examples/nav/
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/nav/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.243696 shiny-0.5.0/shiny/api-examples/navset_hidden/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/navset_hidden/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.243696 shiny-0.5.0/shiny/api-examples/notification_show/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/notification_show/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.243696 shiny-0.5.0/shiny/api-examples/on_ended/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/on_ended/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.243696 shiny-0.5.0/shiny/api-examples/on_flush/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/on_flush/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.243696 shiny-0.5.0/shiny/api-examples/on_flushed/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/on_flushed/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.243696 shiny-0.5.0/shiny/api-examples/output_image/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/output_image/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     9472 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/output_image/posit-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.243696 shiny-0.5.0/shiny/api-examples/output_plot/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/output_plot/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.243696 shiny-0.5.0/shiny/api-examples/output_table/
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/output_table/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/output_table/mtcars.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.243696 shiny-0.5.0/shiny/api-examples/output_text/
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/output_text/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.243696 shiny-0.5.0/shiny/api-examples/output_ui/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/output_ui/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.243696 shiny-0.5.0/shiny/api-examples/page_fixed/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/page_fixed/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.243696 shiny-0.5.0/shiny/api-examples/page_fluid/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/page_fluid/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.243696 shiny-0.5.0/shiny/api-examples/panel_absolute/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/panel_absolute/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.243696 shiny-0.5.0/shiny/api-examples/panel_conditional/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/panel_conditional/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.243696 shiny-0.5.0/shiny/api-examples/panel_title/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/panel_title/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.243696 shiny-0.5.0/shiny/api-examples/poll/
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/poll/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.247696 shiny-0.5.0/shiny/api-examples/remove_ui/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/remove_ui/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.247696 shiny-0.5.0/shiny/api-examples/render_image/
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/render_image/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.247696 shiny-0.5.0/shiny/api-examples/req/
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/req/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.247696 shiny-0.5.0/shiny/api-examples/row/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/row/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.247696 shiny-0.5.0/shiny/api-examples/send_custom_message/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/send_custom_message/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.247696 shiny-0.5.0/shiny/api-examples/template/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/template/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.247696 shiny-0.5.0/shiny/api-examples/todo_list/
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/todo_list/app.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/todo_list/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.247696 shiny-0.5.0/shiny/api-examples/update_action_button/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/update_action_button/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.247696 shiny-0.5.0/shiny/api-examples/update_checkbox/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/update_checkbox/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.247696 shiny-0.5.0/shiny/api-examples/update_checkbox_group/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/update_checkbox_group/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.247696 shiny-0.5.0/shiny/api-examples/update_date/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/update_date/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.247696 shiny-0.5.0/shiny/api-examples/update_date_range/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/update_date_range/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.247696 shiny-0.5.0/shiny/api-examples/update_navs/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/update_navs/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.247696 shiny-0.5.0/shiny/api-examples/update_numeric/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/update_numeric/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.247696 shiny-0.5.0/shiny/api-examples/update_radio_buttons/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/update_radio_buttons/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.247696 shiny-0.5.0/shiny/api-examples/update_select/
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/update_select/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.247696 shiny-0.5.0/shiny/api-examples/update_selectize/
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/update_selectize/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.247696 shiny-0.5.0/shiny/api-examples/update_slider/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/update_slider/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.247696 shiny-0.5.0/shiny/api-examples/update_text/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/update_text/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.251696 shiny-0.5.0/shiny/api-examples/www_dir/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/www_dir/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.215696 shiny-0.5.0/shiny/api-examples/www_dir/www/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.251696 shiny-0.5.0/shiny/api-examples/www_dir/www/css/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/www_dir/www/css/more-styles.css
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/www_dir/www/css/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.251696 shiny-0.5.0/shiny/api-examples/www_dir/www/js/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/api-examples/www_dir/www/js/changetext.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.251696 shiny-0.5.0/shiny/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.219696 shiny-0.5.0/shiny/experimental/api-examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.251696 shiny-0.5.0/shiny/experimental/api-examples/accordion/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/api-examples/accordion/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.251696 shiny-0.5.0/shiny/experimental/api-examples/accordion_panel/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/api-examples/accordion_panel/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.251696 shiny-0.5.0/shiny/experimental/api-examples/accordion_panel_close/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/api-examples/accordion_panel_close/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.251696 shiny-0.5.0/shiny/experimental/api-examples/accordion_panel_insert/
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/api-examples/accordion_panel_insert/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.251696 shiny-0.5.0/shiny/experimental/api-examples/accordion_panel_open/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/api-examples/accordion_panel_open/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.251696 shiny-0.5.0/shiny/experimental/api-examples/accordion_panel_remove/
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/api-examples/accordion_panel_remove/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.251696 shiny-0.5.0/shiny/experimental/api-examples/accordion_panel_set/
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/api-examples/accordion_panel_set/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.251696 shiny-0.5.0/shiny/experimental/api-examples/accordion_panel_update/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/api-examples/accordion_panel_update/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.251696 shiny-0.5.0/shiny/experimental/api-examples/as_fill_carrier/
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/api-examples/as_fill_carrier/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.251696 shiny-0.5.0/shiny/experimental/api-examples/as_fill_item/
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/api-examples/as_fill_item/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.251696 shiny-0.5.0/shiny/experimental/api-examples/as_fillable_container/
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/api-examples/as_fillable_container/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.251696 shiny-0.5.0/shiny/experimental/api-examples/card/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/api-examples/card/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.251696 shiny-0.5.0/shiny/experimental/api-examples/card_body/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/api-examples/card_body/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.255696 shiny-0.5.0/shiny/experimental/api-examples/card_footer/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/api-examples/card_footer/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.255696 shiny-0.5.0/shiny/experimental/api-examples/card_header/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/api-examples/card_header/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.255696 shiny-0.5.0/shiny/experimental/api-examples/card_image/
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/api-examples/card_image/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.255696 shiny-0.5.0/shiny/experimental/api-examples/card_title/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/api-examples/card_title/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.255696 shiny-0.5.0/shiny/experimental/api-examples/input_text_area/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/api-examples/input_text_area/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.255696 shiny-0.5.0/shiny/experimental/api-examples/layout_column_wrap/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/api-examples/layout_column_wrap/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.255696 shiny-0.5.0/shiny/experimental/api-examples/layout_sidebar/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/api-examples/layout_sidebar/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.255696 shiny-0.5.0/shiny/experimental/api-examples/page_sidebar/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/api-examples/page_sidebar/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.255696 shiny-0.5.0/shiny/experimental/api-examples/showcase_left_center/
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/api-examples/showcase_left_center/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.255696 shiny-0.5.0/shiny/experimental/api-examples/showcase_top_right/
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/api-examples/showcase_top_right/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.255696 shiny-0.5.0/shiny/experimental/api-examples/sidebar/
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/api-examples/sidebar/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.255696 shiny-0.5.0/shiny/experimental/api-examples/sidebar_toggle/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/api-examples/sidebar_toggle/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.255696 shiny-0.5.0/shiny/experimental/api-examples/tooltip/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/api-examples/tooltip/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.255696 shiny-0.5.0/shiny/experimental/api-examples/tooltip_toggle/
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/api-examples/tooltip_toggle/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.255696 shiny-0.5.0/shiny/experimental/api-examples/update_tooltip/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/api-examples/update_tooltip/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.255696 shiny-0.5.0/shiny/experimental/api-examples/value_box/
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/api-examples/value_box/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.219696 shiny-0.5.0/shiny/experimental/e2e/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.255696 shiny-0.5.0/shiny/experimental/e2e/navbar/
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/e2e/navbar/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.255696 shiny-0.5.0/shiny/experimental/e2e/sidebar/
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/e2e/sidebar/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/e2e/sidebar/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.259696 shiny-0.5.0/shiny/experimental/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22227 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/ui/_accordion.py
--rw-r--r--   0 runner    (1001) docker     (123)    23852 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/ui/_card.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/ui/_color.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/ui/_css_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19432 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/ui/_fill.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/ui/_htmldeps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/ui/_input_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/ui/_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    19709 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/ui/_navs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/ui/_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/ui/_page.py
--rw-r--r--   0 runner    (1001) docker     (123)    21490 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/ui/_sidebar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/ui/_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/ui/_tooltip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/ui/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8554 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/ui/_valuebox.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/ui/_web_component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.259696 shiny-0.5.0/shiny/experimental/www/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.259696 shiny-0.5.0/shiny/experimental/www/bslib/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/www/bslib/_version.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.219696 shiny-0.5.0/shiny/experimental/www/bslib/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.259696 shiny-0.5.0/shiny/experimental/www/bslib/components/accordion/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/www/bslib/components/accordion/accordion.css
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/www/bslib/components/accordion/accordion.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    13751 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/www/bslib/components/accordion/accordion.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.259696 shiny-0.5.0/shiny/experimental/www/bslib/components/card/
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/www/bslib/components/card/card.css
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/www/bslib/components/card/card.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    26497 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/www/bslib/components/card/card.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.259696 shiny-0.5.0/shiny/experimental/www/bslib/components/grid/
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/www/bslib/components/grid/grid.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.263696 shiny-0.5.0/shiny/experimental/www/bslib/components/nav_spacer/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/www/bslib/components/nav_spacer/nav_spacer.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.263696 shiny-0.5.0/shiny/experimental/www/bslib/components/page_fillable/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/www/bslib/components/page_fillable/page_fillable.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.263696 shiny-0.5.0/shiny/experimental/www/bslib/components/page_navbar/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/www/bslib/components/page_navbar/page_navbar.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.263696 shiny-0.5.0/shiny/experimental/www/bslib/components/page_sidebar/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/www/bslib/components/page_sidebar/page_sidebar.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.263696 shiny-0.5.0/shiny/experimental/www/bslib/components/sidebar/
--rw-r--r--   0 runner    (1001) docker     (123)     9516 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/www/bslib/components/sidebar/sidebar.css
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/www/bslib/components/sidebar/sidebar.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    27772 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/www/bslib/components/sidebar/sidebar.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.263696 shiny-0.5.0/shiny/experimental/www/bslib/components/value_box/
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/www/bslib/components/value_box/value_box.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.263696 shiny-0.5.0/shiny/experimental/www/bslib/components/webComponents/
--rw-r--r--   0 runner    (1001) docker     (123)    23059 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/www/bslib/components/webComponents/webComponents.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   206798 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/www/bslib/components/webComponents/webComponents.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.263696 shiny-0.5.0/shiny/experimental/www/htmltools/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/www/htmltools/_version.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.263696 shiny-0.5.0/shiny/experimental/www/htmltools/fill/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/www/htmltools/fill/fill.css
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/www/textarea-autoresize.css
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/experimental/www/textarea-autoresize.js
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/html_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/http_staticfiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/input_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/module.py
--rw-r--r--   0 runner    (1001) docker     (123)    15552 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/plotutils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.263696 shiny-0.5.0/shiny/reactive/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/reactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/reactive/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    13119 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/reactive/_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)    30454 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/reactive/_reactives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.267696 shiny-0.5.0/shiny/render/
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/render/_coordmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    11320 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/render/_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/render/_dataframe_unsafe.py
--rw-r--r--   0 runner    (1001) docker     (123)    25232 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/render/_render.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/render/_try_render_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.267696 shiny-0.5.0/shiny/session/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39788 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/session/_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/session/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.271696 shiny-0.5.0/shiny/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14213 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/ui/_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/ui/_download_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/ui/_html_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/ui/_include_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/ui/_input_action_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/ui/_input_check_radio.py
--rw-r--r--   0 runner    (1001) docker     (123)    10103 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/ui/_input_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/ui/_input_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/ui/_input_numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/ui/_input_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/ui/_input_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/ui/_input_slider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/ui/_input_text.py
--rw-r--r--   0 runner    (1001) docker     (123)    26265 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/ui/_input_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/ui/_insert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/ui/_markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/ui/_modal.py
--rw-r--r--   0 runner    (1001) docker     (123)    27357 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/ui/_navs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/ui/_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/ui/_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/ui/_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/ui/_plot_output_opts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/ui/_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/ui/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.271696 shiny-0.5.0/shiny/ui/_x/
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/ui/_x/_css_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/ui/_x/_fill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/ui/_x/_htmldeps.py
--rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/ui/_x/_sidebar.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/ui/_x/_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/ui/_x/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.271696 shiny-0.5.0/shiny/ui/dataframe/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/ui/dataframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/ui/dataframe/_dataframe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.223696 shiny-0.5.0/shiny/www/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.279696 shiny-0.5.0/shiny/www/shared/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/_version.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.223696 shiny-0.5.0/shiny/www/shared/_x/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.223696 shiny-0.5.0/shiny/www/shared/_x/bslib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.223696 shiny-0.5.0/shiny/www/shared/_x/bslib/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.279696 shiny-0.5.0/shiny/www/shared/_x/bslib/components/nav_spacer/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/_x/bslib/components/nav_spacer/nav_spacer.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.279696 shiny-0.5.0/shiny/www/shared/_x/bslib/components/page_sidebar/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/_x/bslib/components/page_sidebar/page_sidebar.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.283697 shiny-0.5.0/shiny/www/shared/_x/bslib/components/sidebar/
--rw-r--r--   0 runner    (1001) docker     (123)     9516 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/_x/bslib/components/sidebar/sidebar.css
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/_x/bslib/components/sidebar/sidebar.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    27772 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/_x/bslib/components/sidebar/sidebar.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.223696 shiny-0.5.0/shiny/www/shared/_x/htmltools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.283697 shiny-0.5.0/shiny/www/shared/_x/htmltools/fill/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/_x/htmltools/fill/fill.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.283697 shiny-0.5.0/shiny/www/shared/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/bootstrap/_version.json
--rw-r--r--   0 runner    (1001) docker     (123)    80496 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/bootstrap/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   333304 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/bootstrap/bootstrap.bundle.min.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   242914 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/bootstrap/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/bootstrap/font.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.287696 shiny-0.5.0/shiny/www/shared/bootstrap/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    56036 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/bootstrap/fonts/HI_diYsKILxRpg3hIP6sJ7fM7PqPMcMnZFqUwX28DBKXhM0.woff
--rw-r--r--   0 runner    (1001) docker     (123)    56044 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/bootstrap/fonts/HI_diYsKILxRpg3hIP6sJ7fM7PqPMcMnZFqUwX28DMyQhM0.woff
--rw-r--r--   0 runner    (1001) docker     (123)    47776 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/bootstrap/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTbI1rSg.woff
--rw-r--r--   0 runner    (1001) docker     (123)    47984 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/bootstrap/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTsoprSg.woff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.287696 shiny-0.5.0/shiny/www/shared/bootstrap/fonts/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (123)   108738 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    72136 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/bootstrap/fonts/memQYaGs126MiZpBA-UFUIcVXSCEkx2cmqvXlWq8tWZ0Pw86hd0Rk0ZjaVQ.woff
--rw-r--r--   0 runner    (1001) docker     (123)    74700 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/bootstrap/fonts/memQYaGs126MiZpBA-UFUIcVXSCEkx2cmqvXlWq8tWZ0Pw86hd0Rk5hkaVQ.woff
--rw-r--r--   0 runner    (1001) docker     (123)    74564 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/bootstrap/fonts/memQYaGs126MiZpBA-UFUIcVXSCEkx2cmqvXlWq8tWZ0Pw86hd0Rk8ZkaVQ.woff
--rw-r--r--   0 runner    (1001) docker     (123)    74940 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/bootstrap/fonts/memQYaGs126MiZpBA-UFUIcVXSCEkx2cmqvXlWq8tWZ0Pw86hd0Rk_RkaVQ.woff
--rw-r--r--   0 runner    (1001) docker     (123)    74644 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/bootstrap/fonts/memQYaGs126MiZpBA-UFUIcVXSCEkx2cmqvXlWq8tWZ0Pw86hd0RkxhjaVQ.woff
--rw-r--r--   0 runner    (1001) docker     (123)    71660 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/bootstrap/fonts/memQYaGs126MiZpBA-UFUIcVXSCEkx2cmqvXlWq8tWZ0Pw86hd0RkyFjaVQ.woff
--rw-r--r--   0 runner    (1001) docker     (123)    68664 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/bootstrap/fonts/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsg-1y4k.woff
--rw-r--r--   0 runner    (1001) docker     (123)    70652 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/bootstrap/fonts/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsgH1y4k.woff
--rw-r--r--   0 runner    (1001) docker     (123)    69392 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/bootstrap/fonts/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgshZ1y4k.woff
--rw-r--r--   0 runner    (1001) docker     (123)    70524 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/bootstrap/fonts/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsiH0C4k.woff
--rw-r--r--   0 runner    (1001) docker     (123)    70792 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/bootstrap/fonts/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0C4k.woff
--rw-r--r--   0 runner    (1001) docker     (123)    71144 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/bootstrap/fonts/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjr0C4k.woff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.291696 shiny-0.5.0/shiny/www/shared/dataframe/
--rw-r--r--   0 runner    (1001) docker     (123)   104970 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/dataframe/dataframe.js
--rw-r--r--   0 runner    (1001) docker     (123)   537572 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/dataframe/dataframe.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.223696 shiny-0.5.0/shiny/www/shared/datepicker/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.291696 shiny-0.5.0/shiny/www/shared/datepicker/css/
--rw-r--r--   0 runner    (1001) docker     (123)    22729 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/css/bootstrap-datepicker3.css
--rw-r--r--   0 runner    (1001) docker     (123)    21013 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/css/bootstrap-datepicker3.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.291696 shiny-0.5.0/shiny/www/shared/datepicker/js/
--rw-r--r--   0 runner    (1001) docker     (123)    57916 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/bootstrap-datepicker.js
--rw-r--r--   0 runner    (1001) docker     (123)   106348 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/bootstrap-datepicker.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.307697 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker-en-CA.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ar-tn.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ar.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.az.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bg.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bm.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bn.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.br.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bs.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ca.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.cs.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.cy.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.da.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.de.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.el.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-AU.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-CA.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-GB.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-IE.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-NZ.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-ZA.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.eo.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.es.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.et.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.eu.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fa.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fi.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fo.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fr-CH.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fr.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.gl.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.he.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hi.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hr.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hu.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hy.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.id.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.is.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.it-CH.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.it.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ja.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ka.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kh.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kk.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.km.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ko.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kr.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.lt.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.lv.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.me.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.mk.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.mn.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ms.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.nl-BE.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.nl.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.no.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.oc.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.pl.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.pt-BR.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.pt.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ro.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.rs-latin.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.rs.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ru.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.si.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sk.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sl.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sq.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sr-latin.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sr.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sv.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sw.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ta.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.tg.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.th.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.tk.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.tr.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uk.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uz-cyrl.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uz-latn.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.vi.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.zh-CN.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.zh-TW.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.311697 shiny-0.5.0/shiny/www/shared/datepicker/scss/
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/scss/build3.scss
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/datepicker/scss/datepicker3.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.311697 shiny-0.5.0/shiny/www/shared/highlight/
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/highlight/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22392 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/highlight/classref.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/highlight/highlight.pack.js
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/highlight/rstudio.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.223696 shiny-0.5.0/shiny/www/shared/ionrangeslider/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.311697 shiny-0.5.0/shiny/www/shared/ionrangeslider/css/
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/ionrangeslider/css/ion.rangeSlider.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.311697 shiny-0.5.0/shiny/www/shared/ionrangeslider/js/
--rw-r--r--   0 runner    (1001) docker     (123)    84989 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/ionrangeslider/js/ion.rangeSlider.js
--rw-r--r--   0 runner    (1001) docker     (123)    41631 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/ionrangeslider/js/ion.rangeSlider.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.311697 shiny-0.5.0/shiny/www/shared/ionrangeslider/scss/
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/ionrangeslider/scss/_base.scss
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/ionrangeslider/scss/_mixins.scss
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/ionrangeslider/scss/shiny.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.311697 shiny-0.5.0/shiny/www/shared/jquery/
--rw-r--r--   0 runner    (1001) docker     (123)   288580 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/jquery/jquery-3.6.0.js
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/jquery/jquery-3.6.0.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   137972 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/jquery/jquery-3.6.0.min.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.315697 shiny-0.5.0/shiny/www/shared/jqueryui/
--rw-r--r--   0 runner    (1001) docker     (123)    14243 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/jqueryui/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/jqueryui/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.315697 shiny-0.5.0/shiny/www/shared/jqueryui/images/
--rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/jqueryui/images/ui-icons_444444_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/jqueryui/images/ui-icons_555555_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/jqueryui/images/ui-icons_777620_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/jqueryui/images/ui-icons_777777_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/jqueryui/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/jqueryui/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)    32532 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/jqueryui/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    37452 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/jqueryui/jquery-ui.css
--rw-r--r--   0 runner    (1001) docker     (123)   529159 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/jqueryui/jquery-ui.js
--rw-r--r--   0 runner    (1001) docker     (123)    32130 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/jqueryui/jquery-ui.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   255084 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/jqueryui/jquery-ui.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    18718 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/jqueryui/jquery-ui.structure.css
--rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/jqueryui/jquery-ui.structure.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/jqueryui/jquery-ui.theme.css
--rw-r--r--   0 runner    (1001) docker     (123)    13891 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/jqueryui/jquery-ui.theme.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.319697 shiny-0.5.0/shiny/www/shared/requirejs/
--rw-r--r--   0 runner    (1001) docker     (123)    19715 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/requirejs/require.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.223696 shiny-0.5.0/shiny/www/shared/selectize/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.223696 shiny-0.5.0/shiny/www/shared/selectize/accessibility/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.319697 shiny-0.5.0/shiny/www/shared/selectize/accessibility/js/
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/selectize/accessibility/js/selectize-plugin-a11y.js
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/selectize/accessibility/js/selectize-plugin-a11y.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.319697 shiny-0.5.0/shiny/www/shared/selectize/css/
--rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/selectize/css/selectize.bootstrap3.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.319697 shiny-0.5.0/shiny/www/shared/selectize/js/
--rw-r--r--   0 runner    (1001) docker     (123)    45139 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/selectize/js/selectize.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.319697 shiny-0.5.0/shiny/www/shared/selectize/scss/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.319697 shiny-0.5.0/shiny/www/shared/selectize/scss/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/selectize/scss/plugins/drag_drop.scss
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/selectize/scss/plugins/dropdown_header.scss
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/selectize/scss/plugins/optgroup_columns.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/selectize/scss/plugins/remove_button.scss
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/selectize/scss/selectize.bootstrap3.scss
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/selectize/scss/selectize.bootstrap4.scss
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/selectize/scss/selectize.bootstrap5.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/selectize/scss/selectize.default.scss
--rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/selectize/scss/selectize.scss
--rw-r--r--   0 runner    (1001) docker     (123)    23760 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/shiny-autoreload.js
--rw-r--r--   0 runner    (1001) docker     (123)   125989 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/shiny-autoreload.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/shiny-showcase.css
--rw-r--r--   0 runner    (1001) docker     (123)    24731 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/shiny-showcase.js
--rw-r--r--   0 runner    (1001) docker     (123)   126645 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/shiny-showcase.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/shiny-testmode.js
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/shiny-testmode.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   758008 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/shiny.js
--rw-r--r--   0 runner    (1001) docker     (123)  1315406 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/shiny.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/shiny.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   306558 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/shiny.min.js
--rw-r--r--   0 runner    (1001) docker     (123)  1349906 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/shiny.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.319697 shiny-0.5.0/shiny/www/shared/shiny_scss/
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/shiny_scss/bootstrap.scss
--rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/shiny_scss/shiny.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.319697 shiny-0.5.0/shiny/www/shared/showdown/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.319697 shiny-0.5.0/shiny/www/shared/showdown/compressed/
--rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/showdown/compressed/showdown.js
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/showdown/license.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.319697 shiny-0.5.0/shiny/www/shared/showdown/src/
--rw-r--r--   0 runner    (1001) docker     (123)    37933 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/showdown/src/showdown.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.319697 shiny-0.5.0/shiny/www/shared/strftime/
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-08-01 19:29:59.000000 shiny-0.5.0/shiny/www/shared/strftime/strftime-min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.231696 shiny-0.5.0/shiny.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-08-01 19:31:43.000000 shiny-0.5.0/shiny.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21294 2023-08-01 19:31:43.000000 shiny-0.5.0/shiny.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 19:31:43.000000 shiny-0.5.0/shiny.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-01 19:31:43.000000 shiny-0.5.0/shiny.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 19:31:43.000000 shiny-0.5.0/shiny.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-01 19:31:43.000000 shiny-0.5.0/shiny.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 19:31:43.000000 shiny-0.5.0/shiny.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:31:43.323697 shiny-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 19:29:59.000000 shiny-0.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-08-01 19:29:59.000000 shiny-0.5.0/tests/asyncio_prevent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-08-01 19:29:59.000000 shiny-0.5.0/tests/mocktime.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-01 19:29:59.000000 shiny-0.5.0/tests/test_datastructures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-08-01 19:29:59.000000 shiny-0.5.0/tests/test_e2e_regex_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-08-01 19:29:59.000000 shiny-0.5.0/tests/test_markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-08-01 19:29:59.000000 shiny-0.5.0/tests/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-08-01 19:29:59.000000 shiny-0.5.0/tests/test_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-08-01 19:29:59.000000 shiny-0.5.0/tests/test_navs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-08-01 19:29:59.000000 shiny-0.5.0/tests/test_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)    31032 2023-08-01 19:29:59.000000 shiny-0.5.0/tests/test_reactives.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-08-01 19:29:59.000000 shiny-0.5.0/tests/test_shinysession.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-08-01 19:29:59.000000 shiny-0.5.0/tests/test_static.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-08-01 19:29:59.000000 shiny-0.5.0/tests/test_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-08-01 19:29:59.000000 shiny-0.5.0/tests/test_ui_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-08-01 19:29:59.000000 shiny-0.5.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-08-01 19:29:59.000000 shiny-0.5.0/tests/test_utils_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-01 19:29:59.000000 shiny-0.5.0/tests/test_x_sidebar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.846321 shiny-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-08 21:06:46.000000 shiny-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-08-08 21:06:46.000000 shiny-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-08-08 21:08:06.846321 shiny-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-08-08 21:06:46.000000 shiny-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.790321 shiny-0.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-08-08 21:06:46.000000 shiny-0.5.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-08-08 21:08:06.846321 shiny-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 21:06:46.000000 shiny-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.794321 shiny-0.5.1/shiny/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14463 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/_autoreload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/_datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/_fileupload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/_hostenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/_launchbrowser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14776 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/_shinyenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/_static.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/_typing_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13768 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.786321 shiny-0.5.1/shiny/api-examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.794321 shiny-0.5.1/shiny/api-examples/Calc/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/Calc/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.794321 shiny-0.5.1/shiny/api-examples/Effect/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/Effect/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.794321 shiny-0.5.1/shiny/api-examples/Module/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/Module/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.794321 shiny-0.5.1/shiny/api-examples/Progress/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/Progress/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.794321 shiny-0.5.1/shiny/api-examples/SafeException/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/SafeException/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.794321 shiny-0.5.1/shiny/api-examples/SilentCancelOutputException/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/SilentCancelOutputException/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.794321 shiny-0.5.1/shiny/api-examples/SilentException/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/SilentException/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.794321 shiny-0.5.1/shiny/api-examples/Value/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/Value/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.794321 shiny-0.5.1/shiny/api-examples/close/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/close/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.794321 shiny-0.5.1/shiny/api-examples/data_frame/
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/data_frame/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/download/
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/download/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/download/mtcars.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/download_button/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/download_button/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/download_button/mtcars.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/download_link/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/download_link/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/download_link/mtcars.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/dynamic_route/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/dynamic_route/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/event/
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/event/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/file_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/file_reader/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/file_reader/mtcars.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/include_css/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/include_css/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/include_css/css/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/include_css/css/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/include_javascript/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/include_javascript/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/include_javascript/js/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/include_javascript/js/app.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/input_action_button/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/input_action_button/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/input_action_link/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/input_action_link/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/input_checkbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/input_checkbox/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/input_checkbox_group/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/input_checkbox_group/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/input_date/
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/input_date/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/input_date_range/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/input_date_range/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/input_file/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/input_file/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/input_numeric/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/input_numeric/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/input_password/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/input_password/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/input_radio_buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/input_radio_buttons/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/input_select/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/input_select/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/input_selectize/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/input_selectize/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/input_slider/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/input_slider/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/input_switch/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/input_switch/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/input_text/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/input_text/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/input_text_area/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/input_text_area/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/insert_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/insert_ui/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/invalidate_later/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/invalidate_later/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/isolate/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/isolate/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/layout_sidebar/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/layout_sidebar/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/markdown/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/modal/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/modal/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/nav/
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/nav/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/navset_hidden/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/navset_hidden/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/notification_show/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/notification_show/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/on_ended/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/on_ended/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/on_flush/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/on_flush/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/on_flushed/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/on_flushed/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/output_image/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/output_image/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9472 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/output_image/posit-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/output_plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/output_plot/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.798321 shiny-0.5.1/shiny/api-examples/output_table/
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/output_table/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/output_table/mtcars.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.802321 shiny-0.5.1/shiny/api-examples/output_text/
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/output_text/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.802321 shiny-0.5.1/shiny/api-examples/output_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/output_ui/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.802321 shiny-0.5.1/shiny/api-examples/page_fixed/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/page_fixed/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.802321 shiny-0.5.1/shiny/api-examples/page_fluid/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/page_fluid/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.802321 shiny-0.5.1/shiny/api-examples/panel_absolute/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/panel_absolute/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.802321 shiny-0.5.1/shiny/api-examples/panel_conditional/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/panel_conditional/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.802321 shiny-0.5.1/shiny/api-examples/panel_title/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/panel_title/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.802321 shiny-0.5.1/shiny/api-examples/poll/
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/poll/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.802321 shiny-0.5.1/shiny/api-examples/remove_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/remove_ui/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.802321 shiny-0.5.1/shiny/api-examples/render_image/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/render_image/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.802321 shiny-0.5.1/shiny/api-examples/req/
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/req/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.802321 shiny-0.5.1/shiny/api-examples/row/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/row/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.802321 shiny-0.5.1/shiny/api-examples/send_custom_message/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/send_custom_message/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.802321 shiny-0.5.1/shiny/api-examples/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/template/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.802321 shiny-0.5.1/shiny/api-examples/todo_list/
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/todo_list/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/todo_list/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.802321 shiny-0.5.1/shiny/api-examples/update_action_button/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/update_action_button/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.802321 shiny-0.5.1/shiny/api-examples/update_checkbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/update_checkbox/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.802321 shiny-0.5.1/shiny/api-examples/update_checkbox_group/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/update_checkbox_group/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.802321 shiny-0.5.1/shiny/api-examples/update_date/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/update_date/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.802321 shiny-0.5.1/shiny/api-examples/update_date_range/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/update_date_range/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.802321 shiny-0.5.1/shiny/api-examples/update_navs/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/update_navs/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.802321 shiny-0.5.1/shiny/api-examples/update_numeric/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/update_numeric/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.802321 shiny-0.5.1/shiny/api-examples/update_radio_buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/update_radio_buttons/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.802321 shiny-0.5.1/shiny/api-examples/update_select/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/update_select/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.802321 shiny-0.5.1/shiny/api-examples/update_selectize/
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/update_selectize/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.802321 shiny-0.5.1/shiny/api-examples/update_slider/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/update_slider/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.802321 shiny-0.5.1/shiny/api-examples/update_text/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/update_text/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.802321 shiny-0.5.1/shiny/api-examples/www_dir/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/www_dir/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.786321 shiny-0.5.1/shiny/api-examples/www_dir/www/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.802321 shiny-0.5.1/shiny/api-examples/www_dir/www/css/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/www_dir/www/css/more-styles.css
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/www_dir/www/css/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.802321 shiny-0.5.1/shiny/api-examples/www_dir/www/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/api-examples/www_dir/www/js/changetext.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.802321 shiny-0.5.1/shiny/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.786321 shiny-0.5.1/shiny/experimental/api-examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.802321 shiny-0.5.1/shiny/experimental/api-examples/accordion/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/api-examples/accordion/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.802321 shiny-0.5.1/shiny/experimental/api-examples/accordion_panel/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/api-examples/accordion_panel/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.802321 shiny-0.5.1/shiny/experimental/api-examples/accordion_panel_close/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/api-examples/accordion_panel_close/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.806321 shiny-0.5.1/shiny/experimental/api-examples/accordion_panel_insert/
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/api-examples/accordion_panel_insert/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.806321 shiny-0.5.1/shiny/experimental/api-examples/accordion_panel_open/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/api-examples/accordion_panel_open/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.806321 shiny-0.5.1/shiny/experimental/api-examples/accordion_panel_remove/
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/api-examples/accordion_panel_remove/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.806321 shiny-0.5.1/shiny/experimental/api-examples/accordion_panel_set/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/api-examples/accordion_panel_set/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.806321 shiny-0.5.1/shiny/experimental/api-examples/accordion_panel_update/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/api-examples/accordion_panel_update/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.806321 shiny-0.5.1/shiny/experimental/api-examples/as_fill_carrier/
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/api-examples/as_fill_carrier/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.806321 shiny-0.5.1/shiny/experimental/api-examples/as_fill_item/
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/api-examples/as_fill_item/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.806321 shiny-0.5.1/shiny/experimental/api-examples/as_fillable_container/
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/api-examples/as_fillable_container/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.806321 shiny-0.5.1/shiny/experimental/api-examples/card/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/api-examples/card/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.806321 shiny-0.5.1/shiny/experimental/api-examples/card_body/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/api-examples/card_body/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.806321 shiny-0.5.1/shiny/experimental/api-examples/card_footer/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/api-examples/card_footer/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.806321 shiny-0.5.1/shiny/experimental/api-examples/card_header/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/api-examples/card_header/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.806321 shiny-0.5.1/shiny/experimental/api-examples/card_image/
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/api-examples/card_image/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.806321 shiny-0.5.1/shiny/experimental/api-examples/card_title/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/api-examples/card_title/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.806321 shiny-0.5.1/shiny/experimental/api-examples/input_text_area/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/api-examples/input_text_area/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.806321 shiny-0.5.1/shiny/experimental/api-examples/layout_column_wrap/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/api-examples/layout_column_wrap/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.806321 shiny-0.5.1/shiny/experimental/api-examples/layout_sidebar/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/api-examples/layout_sidebar/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.806321 shiny-0.5.1/shiny/experimental/api-examples/page_sidebar/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/api-examples/page_sidebar/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.806321 shiny-0.5.1/shiny/experimental/api-examples/showcase_left_center/
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/api-examples/showcase_left_center/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.806321 shiny-0.5.1/shiny/experimental/api-examples/showcase_top_right/
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/api-examples/showcase_top_right/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.806321 shiny-0.5.1/shiny/experimental/api-examples/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/api-examples/sidebar/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.806321 shiny-0.5.1/shiny/experimental/api-examples/sidebar_toggle/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/api-examples/sidebar_toggle/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.806321 shiny-0.5.1/shiny/experimental/api-examples/tooltip/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/api-examples/tooltip/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.806321 shiny-0.5.1/shiny/experimental/api-examples/tooltip_toggle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/api-examples/tooltip_toggle/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.806321 shiny-0.5.1/shiny/experimental/api-examples/update_tooltip/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/api-examples/update_tooltip/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.806321 shiny-0.5.1/shiny/experimental/api-examples/value_box/
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/api-examples/value_box/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.786321 shiny-0.5.1/shiny/experimental/e2e/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.806321 shiny-0.5.1/shiny/experimental/e2e/navbar/
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/e2e/navbar/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.806321 shiny-0.5.1/shiny/experimental/e2e/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/e2e/sidebar/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/e2e/sidebar/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.810321 shiny-0.5.1/shiny/experimental/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22227 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/ui/_accordion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23852 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/ui/_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/ui/_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/ui/_css_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19432 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/ui/_fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/ui/_htmldeps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/ui/_input_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/ui/_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19709 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/ui/_navs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/ui/_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9330 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/ui/_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21490 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/ui/_sidebar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/ui/_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/ui/_tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/ui/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8554 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/ui/_valuebox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/ui/_web_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.810321 shiny-0.5.1/shiny/experimental/www/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.810321 shiny-0.5.1/shiny/experimental/www/bslib/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/www/bslib/_version.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.790321 shiny-0.5.1/shiny/experimental/www/bslib/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.810321 shiny-0.5.1/shiny/experimental/www/bslib/components/accordion/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/www/bslib/components/accordion/accordion.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/www/bslib/components/accordion/accordion.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13751 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/www/bslib/components/accordion/accordion.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.810321 shiny-0.5.1/shiny/experimental/www/bslib/components/card/
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/www/bslib/components/card/card.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/www/bslib/components/card/card.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    26497 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/www/bslib/components/card/card.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.810321 shiny-0.5.1/shiny/experimental/www/bslib/components/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/www/bslib/components/grid/grid.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.810321 shiny-0.5.1/shiny/experimental/www/bslib/components/nav_spacer/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/www/bslib/components/nav_spacer/nav_spacer.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.810321 shiny-0.5.1/shiny/experimental/www/bslib/components/page_fillable/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/www/bslib/components/page_fillable/page_fillable.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.810321 shiny-0.5.1/shiny/experimental/www/bslib/components/page_navbar/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/www/bslib/components/page_navbar/page_navbar.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.810321 shiny-0.5.1/shiny/experimental/www/bslib/components/page_sidebar/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/www/bslib/components/page_sidebar/page_sidebar.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.810321 shiny-0.5.1/shiny/experimental/www/bslib/components/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (123)     9516 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/www/bslib/components/sidebar/sidebar.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/www/bslib/components/sidebar/sidebar.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27772 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/www/bslib/components/sidebar/sidebar.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.810321 shiny-0.5.1/shiny/experimental/www/bslib/components/value_box/
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/www/bslib/components/value_box/value_box.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.810321 shiny-0.5.1/shiny/experimental/www/bslib/components/webComponents/
+-rw-r--r--   0 runner    (1001) docker     (123)    23059 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/www/bslib/components/webComponents/webComponents.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   206798 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/www/bslib/components/webComponents/webComponents.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.814321 shiny-0.5.1/shiny/experimental/www/htmltools/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/www/htmltools/_version.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.814321 shiny-0.5.1/shiny/experimental/www/htmltools/fill/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/www/htmltools/fill/fill.css
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/www/textarea-autoresize.css
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/experimental/www/textarea-autoresize.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/html_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/http_staticfiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/input_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15552 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/plotutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.814321 shiny-0.5.1/shiny/reactive/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/reactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/reactive/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13119 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/reactive/_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30454 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/reactive/_reactives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.814321 shiny-0.5.1/shiny/render/
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/render/_coordmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11320 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/render/_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/render/_dataframe_unsafe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25232 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/render/_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/render/_try_render_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.814321 shiny-0.5.1/shiny/session/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39788 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/session/_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/session/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.818321 shiny-0.5.1/shiny/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14213 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/ui/_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/ui/_download_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/ui/_html_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/ui/_include_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/ui/_input_action_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/ui/_input_check_radio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10103 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/ui/_input_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/ui/_input_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/ui/_input_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/ui/_input_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/ui/_input_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/ui/_input_slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/ui/_input_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26265 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/ui/_input_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/ui/_insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/ui/_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/ui/_modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27357 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/ui/_navs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/ui/_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/ui/_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/ui/_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/ui/_plot_output_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/ui/_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/ui/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.818321 shiny-0.5.1/shiny/ui/_x/
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/ui/_x/_css_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/ui/_x/_fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/ui/_x/_htmldeps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/ui/_x/_sidebar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/ui/_x/_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/ui/_x/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.818321 shiny-0.5.1/shiny/ui/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/ui/dataframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/ui/dataframe/_dataframe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.790321 shiny-0.5.1/shiny/www/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.822321 shiny-0.5.1/shiny/www/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/_version.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.790321 shiny-0.5.1/shiny/www/shared/_x/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.790321 shiny-0.5.1/shiny/www/shared/_x/bslib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.790321 shiny-0.5.1/shiny/www/shared/_x/bslib/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.822321 shiny-0.5.1/shiny/www/shared/_x/bslib/components/nav_spacer/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/_x/bslib/components/nav_spacer/nav_spacer.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.822321 shiny-0.5.1/shiny/www/shared/_x/bslib/components/page_sidebar/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/_x/bslib/components/page_sidebar/page_sidebar.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.822321 shiny-0.5.1/shiny/www/shared/_x/bslib/components/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (123)     9516 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/_x/bslib/components/sidebar/sidebar.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/_x/bslib/components/sidebar/sidebar.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27772 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/_x/bslib/components/sidebar/sidebar.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.790321 shiny-0.5.1/shiny/www/shared/_x/htmltools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.822321 shiny-0.5.1/shiny/www/shared/_x/htmltools/fill/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/_x/htmltools/fill/fill.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.822321 shiny-0.5.1/shiny/www/shared/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/bootstrap/_version.json
+-rw-r--r--   0 runner    (1001) docker     (123)    80496 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/bootstrap/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   333304 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/bootstrap/bootstrap.bundle.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   242914 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/bootstrap/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/bootstrap/font.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.826321 shiny-0.5.1/shiny/www/shared/bootstrap/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    56036 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/bootstrap/fonts/HI_diYsKILxRpg3hIP6sJ7fM7PqPMcMnZFqUwX28DBKXhM0.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    56044 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/bootstrap/fonts/HI_diYsKILxRpg3hIP6sJ7fM7PqPMcMnZFqUwX28DMyQhM0.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    47776 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/bootstrap/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTbI1rSg.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    47984 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/bootstrap/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTsoprSg.woff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.826321 shiny-0.5.1/shiny/www/shared/bootstrap/fonts/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   108738 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    72136 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/bootstrap/fonts/memQYaGs126MiZpBA-UFUIcVXSCEkx2cmqvXlWq8tWZ0Pw86hd0Rk0ZjaVQ.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    74700 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/bootstrap/fonts/memQYaGs126MiZpBA-UFUIcVXSCEkx2cmqvXlWq8tWZ0Pw86hd0Rk5hkaVQ.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    74564 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/bootstrap/fonts/memQYaGs126MiZpBA-UFUIcVXSCEkx2cmqvXlWq8tWZ0Pw86hd0Rk8ZkaVQ.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    74940 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/bootstrap/fonts/memQYaGs126MiZpBA-UFUIcVXSCEkx2cmqvXlWq8tWZ0Pw86hd0Rk_RkaVQ.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    74644 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/bootstrap/fonts/memQYaGs126MiZpBA-UFUIcVXSCEkx2cmqvXlWq8tWZ0Pw86hd0RkxhjaVQ.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    71660 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/bootstrap/fonts/memQYaGs126MiZpBA-UFUIcVXSCEkx2cmqvXlWq8tWZ0Pw86hd0RkyFjaVQ.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    68664 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/bootstrap/fonts/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsg-1y4k.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    70652 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/bootstrap/fonts/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsgH1y4k.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    69392 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/bootstrap/fonts/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgshZ1y4k.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    70524 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/bootstrap/fonts/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsiH0C4k.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    70792 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/bootstrap/fonts/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0C4k.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    71144 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/bootstrap/fonts/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjr0C4k.woff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.826321 shiny-0.5.1/shiny/www/shared/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (123)   104970 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/dataframe/dataframe.js
+-rw-r--r--   0 runner    (1001) docker     (123)   537572 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/dataframe/dataframe.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.790321 shiny-0.5.1/shiny/www/shared/datepicker/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.830321 shiny-0.5.1/shiny/www/shared/datepicker/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    22729 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/css/bootstrap-datepicker3.css
+-rw-r--r--   0 runner    (1001) docker     (123)    21013 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/css/bootstrap-datepicker3.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.830321 shiny-0.5.1/shiny/www/shared/datepicker/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    57916 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/bootstrap-datepicker.js
+-rw-r--r--   0 runner    (1001) docker     (123)   106348 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/bootstrap-datepicker.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.838321 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker-en-CA.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ar-tn.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ar.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.az.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bg.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bm.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bn.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.br.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bs.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ca.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.cs.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.cy.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.da.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.de.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.el.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-AU.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-CA.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-GB.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-IE.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-NZ.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-ZA.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.eo.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.es.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.et.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.eu.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fa.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fi.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fo.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fr-CH.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fr.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.gl.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.he.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hi.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hr.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hu.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hy.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.id.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.is.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.it-CH.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.it.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ja.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ka.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kh.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kk.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.km.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ko.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kr.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.lt.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.lv.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.me.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.mk.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.mn.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ms.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.nl-BE.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.nl.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.no.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.oc.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.pl.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.pt-BR.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.pt.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ro.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.rs-latin.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.rs.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ru.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.si.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sk.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sl.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sq.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sr-latin.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sr.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sv.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sw.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ta.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.tg.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.th.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.tk.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.tr.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uk.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uz-cyrl.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uz-latn.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.vi.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.zh-CN.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.zh-TW.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.838321 shiny-0.5.1/shiny/www/shared/datepicker/scss/
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/scss/build3.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/datepicker/scss/datepicker3.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.838321 shiny-0.5.1/shiny/www/shared/highlight/
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/highlight/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22392 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/highlight/classref.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/highlight/highlight.pack.js
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/highlight/rstudio.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.790321 shiny-0.5.1/shiny/www/shared/ionrangeslider/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.838321 shiny-0.5.1/shiny/www/shared/ionrangeslider/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/ionrangeslider/css/ion.rangeSlider.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.838321 shiny-0.5.1/shiny/www/shared/ionrangeslider/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    84989 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/ionrangeslider/js/ion.rangeSlider.js
+-rw-r--r--   0 runner    (1001) docker     (123)    41631 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/ionrangeslider/js/ion.rangeSlider.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.838321 shiny-0.5.1/shiny/www/shared/ionrangeslider/scss/
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/ionrangeslider/scss/_base.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/ionrangeslider/scss/_mixins.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/ionrangeslider/scss/shiny.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.838321 shiny-0.5.1/shiny/www/shared/jquery/
+-rw-r--r--   0 runner    (1001) docker     (123)   288580 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/jquery/jquery-3.6.0.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/jquery/jquery-3.6.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   137972 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/jquery/jquery-3.6.0.min.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.842321 shiny-0.5.1/shiny/www/shared/jqueryui/
+-rw-r--r--   0 runner    (1001) docker     (123)    14243 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/jqueryui/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/jqueryui/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.842321 shiny-0.5.1/shiny/www/shared/jqueryui/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/jqueryui/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/jqueryui/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/jqueryui/images/ui-icons_777620_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7163 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/jqueryui/images/ui-icons_777777_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/jqueryui/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/jqueryui/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32532 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/jqueryui/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    37452 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/jqueryui/jquery-ui.css
+-rw-r--r--   0 runner    (1001) docker     (123)   529159 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/jqueryui/jquery-ui.js
+-rw-r--r--   0 runner    (1001) docker     (123)    32130 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/jqueryui/jquery-ui.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   255084 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/jqueryui/jquery-ui.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18718 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/jqueryui/jquery-ui.structure.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/jqueryui/jquery-ui.structure.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/jqueryui/jquery-ui.theme.css
+-rw-r--r--   0 runner    (1001) docker     (123)    13891 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/jqueryui/jquery-ui.theme.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.842321 shiny-0.5.1/shiny/www/shared/requirejs/
+-rw-r--r--   0 runner    (1001) docker     (123)    19715 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/requirejs/require.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.790321 shiny-0.5.1/shiny/www/shared/selectize/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.790321 shiny-0.5.1/shiny/www/shared/selectize/accessibility/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.842321 shiny-0.5.1/shiny/www/shared/selectize/accessibility/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/selectize/accessibility/js/selectize-plugin-a11y.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/selectize/accessibility/js/selectize-plugin-a11y.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.842321 shiny-0.5.1/shiny/www/shared/selectize/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/selectize/css/selectize.bootstrap3.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.842321 shiny-0.5.1/shiny/www/shared/selectize/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    45139 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/selectize/js/selectize.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.842321 shiny-0.5.1/shiny/www/shared/selectize/scss/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.842321 shiny-0.5.1/shiny/www/shared/selectize/scss/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/selectize/scss/plugins/drag_drop.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/selectize/scss/plugins/dropdown_header.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/selectize/scss/plugins/optgroup_columns.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/selectize/scss/plugins/remove_button.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/selectize/scss/selectize.bootstrap3.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/selectize/scss/selectize.bootstrap4.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/selectize/scss/selectize.bootstrap5.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/selectize/scss/selectize.default.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/selectize/scss/selectize.scss
+-rw-r--r--   0 runner    (1001) docker     (123)    23760 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/shiny-autoreload.js
+-rw-r--r--   0 runner    (1001) docker     (123)   125989 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/shiny-autoreload.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/shiny-showcase.css
+-rw-r--r--   0 runner    (1001) docker     (123)    24731 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/shiny-showcase.js
+-rw-r--r--   0 runner    (1001) docker     (123)   126645 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/shiny-showcase.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/shiny-testmode.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/shiny-testmode.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   758008 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/shiny.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1315406 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/shiny.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/shiny.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   306558 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/shiny.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1349906 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/shiny.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.842321 shiny-0.5.1/shiny/www/shared/shiny_scss/
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/shiny_scss/bootstrap.scss
+-rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/shiny_scss/shiny.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.842321 shiny-0.5.1/shiny/www/shared/showdown/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.842321 shiny-0.5.1/shiny/www/shared/showdown/compressed/
+-rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/showdown/compressed/showdown.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/showdown/license.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.842321 shiny-0.5.1/shiny/www/shared/showdown/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    37933 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/showdown/src/showdown.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.842321 shiny-0.5.1/shiny/www/shared/strftime/
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-08-08 21:06:46.000000 shiny-0.5.1/shiny/www/shared/strftime/strftime-min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.794321 shiny-0.5.1/shiny.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-08-08 21:08:06.000000 shiny-0.5.1/shiny.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21294 2023-08-08 21:08:06.000000 shiny-0.5.1/shiny.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 21:08:06.000000 shiny-0.5.1/shiny.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-08 21:08:06.000000 shiny-0.5.1/shiny.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 21:08:06.000000 shiny-0.5.1/shiny.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-08 21:08:06.000000 shiny-0.5.1/shiny.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-08 21:08:06.000000 shiny-0.5.1/shiny.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 21:08:06.846321 shiny-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-08 21:06:46.000000 shiny-0.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-08-08 21:06:46.000000 shiny-0.5.1/tests/asyncio_prevent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-08-08 21:06:46.000000 shiny-0.5.1/tests/mocktime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-08 21:06:46.000000 shiny-0.5.1/tests/test_datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-08-08 21:06:46.000000 shiny-0.5.1/tests/test_e2e_regex_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-08-08 21:06:46.000000 shiny-0.5.1/tests/test_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-08-08 21:06:46.000000 shiny-0.5.1/tests/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-08-08 21:06:46.000000 shiny-0.5.1/tests/test_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-08-08 21:06:46.000000 shiny-0.5.1/tests/test_navs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-08-08 21:06:46.000000 shiny-0.5.1/tests/test_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31032 2023-08-08 21:06:46.000000 shiny-0.5.1/tests/test_reactives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-08-08 21:06:46.000000 shiny-0.5.1/tests/test_shinysession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-08-08 21:06:46.000000 shiny-0.5.1/tests/test_static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-08-08 21:06:46.000000 shiny-0.5.1/tests/test_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-08-08 21:06:46.000000 shiny-0.5.1/tests/test_ui_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-08-08 21:06:46.000000 shiny-0.5.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-08-08 21:06:46.000000 shiny-0.5.1/tests/test_utils_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-08 21:06:46.000000 shiny-0.5.1/tests/test_x_sidebar.py
```

### Comparing `shiny-0.5.0/LICENSE` & `shiny-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/PKG-INFO` & `shiny-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shiny
-Version: 0.5.0
+Version: 0.5.1
 Summary: A web development framework for Python.
 Home-page: https://github.com/rstudio/py-shiny
 Author: Winston Chang
 Author-email: winston@rstudio.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/rstudio/py-shiny/issues
 Project-URL: Documentation, https://shiny.posit.co/py/
```

### Comparing `shiny-0.5.0/README.md` & `shiny-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/docs/Makefile` & `shiny-0.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/setup.cfg` & `shiny-0.5.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 shiny = py.typed
 
 [options.entry_points]
 console_scripts = 
 	shiny = shiny._main:main
 
 [flake8]
-ignore = E302, E501, F403, F405, W503
+ignore = E302, E501, F403, F405, W503, E203
 extend_exclude = docs, .venv, venv, typings, e2e, build
 
 [isort]
 profile = black
 skip = 
 	__init__.py
 	typings/
```

### Comparing `shiny-0.5.0/shiny/__init__.py` & `shiny-0.5.1/shiny/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """A package for building reactive web applications."""
 
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 from ._shinyenv import is_pyodide as _is_pyodide
 
 # User-facing subpackages that should be available on `from shiny import *`
 from . import reactive
 from . import render
 from .session import (
```

### Comparing `shiny-0.5.0/shiny/_app.py` & `shiny-0.5.1/shiny/_app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/_autoreload.py` & `shiny-0.5.1/shiny/_autoreload.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/_connection.py` & `shiny-0.5.1/shiny/_connection.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/_datastructures.py` & `shiny-0.5.1/shiny/_datastructures.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/_deprecated.py` & `shiny-0.5.1/shiny/_deprecated.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/_docstring.py` & `shiny-0.5.1/shiny/_docstring.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/_error.py` & `shiny-0.5.1/shiny/_error.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/_fileupload.py` & `shiny-0.5.1/shiny/_fileupload.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/_hostenv.py` & `shiny-0.5.1/shiny/_hostenv.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/_launchbrowser.py` & `shiny-0.5.1/shiny/_launchbrowser.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/_main.py` & `shiny-0.5.1/shiny/_main.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/_namespaces.py` & `shiny-0.5.1/shiny/_namespaces.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/_static.py` & `shiny-0.5.1/shiny/_static.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/_typing_extensions.py` & `shiny-0.5.1/shiny/_typing_extensions.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/_utils.py` & `shiny-0.5.1/shiny/_utils.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/_validation.py` & `shiny-0.5.1/shiny/_validation.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/Calc/app.py` & `shiny-0.5.1/shiny/api-examples/Calc/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/Module/app.py` & `shiny-0.5.1/shiny/api-examples/Module/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/Progress/app.py` & `shiny-0.5.1/shiny/api-examples/Progress/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/SilentCancelOutputException/app.py` & `shiny-0.5.1/shiny/api-examples/SilentCancelOutputException/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/SilentException/app.py` & `shiny-0.5.1/shiny/api-examples/SilentException/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/Value/app.py` & `shiny-0.5.1/shiny/api-examples/Value/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/close/app.py` & `shiny-0.5.1/shiny/api-examples/close/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/data_frame/app.py` & `shiny-0.5.1/shiny/api-examples/data_frame/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/download/app.py` & `shiny-0.5.1/shiny/api-examples/download/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/download/mtcars.csv` & `shiny-0.5.1/shiny/api-examples/download/mtcars.csv`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/download_button/app.py` & `shiny-0.5.1/shiny/api-examples/download_button/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/download_button/mtcars.csv` & `shiny-0.5.1/shiny/api-examples/download_button/mtcars.csv`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/download_link/app.py` & `shiny-0.5.1/shiny/api-examples/download_link/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/download_link/mtcars.csv` & `shiny-0.5.1/shiny/api-examples/download_link/mtcars.csv`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/dynamic_route/app.py` & `shiny-0.5.1/shiny/api-examples/dynamic_route/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/event/app.py` & `shiny-0.5.1/shiny/api-examples/event/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/file_reader/mtcars.csv` & `shiny-0.5.1/shiny/api-examples/file_reader/mtcars.csv`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/input_action_button/app.py` & `shiny-0.5.1/shiny/api-examples/input_action_button/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/input_action_link/app.py` & `shiny-0.5.1/shiny/api-examples/input_action_link/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/input_checkbox_group/app.py` & `shiny-0.5.1/shiny/api-examples/input_checkbox_group/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/input_date/app.py` & `shiny-0.5.1/shiny/api-examples/input_date/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/input_date_range/app.py` & `shiny-0.5.1/shiny/api-examples/input_date_range/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/input_file/app.py` & `shiny-0.5.1/shiny/api-examples/input_file/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/input_select/app.py` & `shiny-0.5.1/shiny/api-examples/input_select/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/input_selectize/app.py` & `shiny-0.5.1/shiny/api-examples/input_selectize/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/input_slider/app.py` & `shiny-0.5.1/shiny/api-examples/input_slider/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/isolate/app.py` & `shiny-0.5.1/shiny/api-examples/isolate/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/layout_sidebar/app.py` & `shiny-0.5.1/shiny/api-examples/layout_sidebar/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/modal/app.py` & `shiny-0.5.1/shiny/api-examples/modal/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/nav/app.py` & `shiny-0.5.1/shiny/api-examples/nav/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/navset_hidden/app.py` & `shiny-0.5.1/shiny/api-examples/navset_hidden/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/notification_show/app.py` & `shiny-0.5.1/shiny/api-examples/notification_show/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/on_flush/app.py` & `shiny-0.5.1/shiny/api-examples/on_flush/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/on_flushed/app.py` & `shiny-0.5.1/shiny/api-examples/on_flushed/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/output_image/posit-logo.png` & `shiny-0.5.1/shiny/api-examples/output_image/posit-logo.png`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/output_plot/app.py` & `shiny-0.5.1/shiny/api-examples/output_plot/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/output_table/app.py` & `shiny-0.5.1/shiny/api-examples/output_table/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/output_table/mtcars.csv` & `shiny-0.5.1/shiny/api-examples/output_table/mtcars.csv`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/output_text/app.py` & `shiny-0.5.1/shiny/api-examples/output_text/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/page_fixed/app.py` & `shiny-0.5.1/shiny/api-examples/page_fixed/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/page_fluid/app.py` & `shiny-0.5.1/shiny/api-examples/page_fluid/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/panel_conditional/app.py` & `shiny-0.5.1/shiny/api-examples/panel_conditional/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/poll/app.py` & `shiny-0.5.1/shiny/api-examples/poll/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/render_image/app.py` & `shiny-0.5.1/shiny/api-examples/render_image/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/req/app.py` & `shiny-0.5.1/shiny/api-examples/req/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/row/app.py` & `shiny-0.5.1/shiny/api-examples/row/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/send_custom_message/app.py` & `shiny-0.5.1/shiny/api-examples/send_custom_message/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/todo_list/app.py` & `shiny-0.5.1/shiny/api-examples/todo_list/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/update_action_button/app.py` & `shiny-0.5.1/shiny/api-examples/update_action_button/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/update_checkbox_group/app.py` & `shiny-0.5.1/shiny/api-examples/update_checkbox_group/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/update_date/app.py` & `shiny-0.5.1/shiny/api-examples/update_date/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/update_date_range/app.py` & `shiny-0.5.1/shiny/api-examples/update_date_range/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/update_navs/app.py` & `shiny-0.5.1/shiny/api-examples/update_navs/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/update_numeric/app.py` & `shiny-0.5.1/shiny/api-examples/update_numeric/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/update_radio_buttons/app.py` & `shiny-0.5.1/shiny/api-examples/update_radio_buttons/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/update_select/app.py` & `shiny-0.5.1/shiny/api-examples/update_select/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/update_slider/app.py` & `shiny-0.5.1/shiny/api-examples/update_slider/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/update_text/app.py` & `shiny-0.5.1/shiny/api-examples/update_text/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/api-examples/www_dir/app.py` & `shiny-0.5.1/shiny/api-examples/www_dir/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/api-examples/accordion/app.py` & `shiny-0.5.1/shiny/experimental/api-examples/accordion/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/api-examples/accordion_panel/app.py` & `shiny-0.5.1/shiny/experimental/api-examples/accordion_panel/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/api-examples/accordion_panel_close/app.py` & `shiny-0.5.1/shiny/experimental/api-examples/accordion_panel_close/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/api-examples/accordion_panel_insert/app.py` & `shiny-0.5.1/shiny/experimental/api-examples/accordion_panel_insert/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/api-examples/accordion_panel_open/app.py` & `shiny-0.5.1/shiny/experimental/api-examples/accordion_panel_open/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/api-examples/accordion_panel_remove/app.py` & `shiny-0.5.1/shiny/experimental/api-examples/accordion_panel_remove/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/api-examples/accordion_panel_set/app.py` & `shiny-0.5.1/shiny/experimental/api-examples/accordion_panel_set/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/api-examples/accordion_panel_update/app.py` & `shiny-0.5.1/shiny/experimental/api-examples/accordion_panel_update/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/api-examples/as_fill_carrier/app.py` & `shiny-0.5.1/shiny/experimental/api-examples/as_fill_carrier/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/api-examples/as_fill_item/app.py` & `shiny-0.5.1/shiny/experimental/api-examples/as_fill_item/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/api-examples/as_fillable_container/app.py` & `shiny-0.5.1/shiny/experimental/api-examples/as_fillable_container/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/api-examples/card/app.py` & `shiny-0.5.1/shiny/experimental/api-examples/card/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/api-examples/card_body/app.py` & `shiny-0.5.1/shiny/experimental/api-examples/card_body/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/api-examples/card_image/app.py` & `shiny-0.5.1/shiny/experimental/api-examples/card_image/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/api-examples/showcase_left_center/app.py` & `shiny-0.5.1/shiny/experimental/api-examples/showcase_left_center/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/api-examples/showcase_top_right/app.py` & `shiny-0.5.1/shiny/experimental/api-examples/showcase_top_right/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/api-examples/sidebar/app.py` & `shiny-0.5.1/shiny/experimental/api-examples/sidebar/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/api-examples/sidebar_toggle/app.py` & `shiny-0.5.1/shiny/experimental/api-examples/sidebar_toggle/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/api-examples/tooltip/app.py` & `shiny-0.5.1/shiny/experimental/api-examples/tooltip/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/api-examples/tooltip_toggle/app.py` & `shiny-0.5.1/shiny/experimental/api-examples/tooltip_toggle/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/api-examples/update_tooltip/app.py` & `shiny-0.5.1/shiny/experimental/api-examples/update_tooltip/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/api-examples/value_box/app.py` & `shiny-0.5.1/shiny/experimental/api-examples/value_box/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/e2e/navbar/app.py` & `shiny-0.5.1/shiny/experimental/e2e/navbar/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/e2e/sidebar/app.py` & `shiny-0.5.1/shiny/experimental/e2e/sidebar/app.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/e2e/sidebar/data.py` & `shiny-0.5.1/shiny/experimental/e2e/sidebar/data.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/ui/__init__.py` & `shiny-0.5.1/shiny/experimental/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/ui/_accordion.py` & `shiny-0.5.1/shiny/experimental/ui/_accordion.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/ui/_card.py` & `shiny-0.5.1/shiny/experimental/ui/_card.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/ui/_css_unit.py` & `shiny-0.5.1/shiny/experimental/ui/_css_unit.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/ui/_fill.py` & `shiny-0.5.1/shiny/experimental/ui/_fill.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/ui/_htmldeps.py` & `shiny-0.5.1/shiny/experimental/ui/_htmldeps.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/ui/_input_text.py` & `shiny-0.5.1/shiny/experimental/ui/_input_text.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/ui/_layout.py` & `shiny-0.5.1/shiny/experimental/ui/_layout.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/ui/_navs.py` & `shiny-0.5.1/shiny/experimental/ui/_navs.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/ui/_output.py` & `shiny-0.5.1/shiny/experimental/ui/_output.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/ui/_page.py` & `shiny-0.5.1/shiny/experimental/ui/_page.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     MetadataNode,
     Tag,
     TagAttrs,
     TagAttrValue,
     TagChild,
     TagList,
     css,
+    head_content,
     tags,
 )
 
 from ...types import MISSING, MISSING_TYPE, NavSetArg
 from ...ui._page import page_bootstrap
 from ...ui._utils import get_window_title
 from ._css_unit import CssUnit, as_css_padding, as_css_unit
@@ -274,15 +275,15 @@
     style = css(
         padding=as_css_padding(padding),
         gap=as_css_unit(gap),
         __bslib_page_fill_mobile_height="100%" if fillable_mobile else "auto",
     )
 
     return page_bootstrap(
-        tags.head(tags.style("html { height: 100%; }")),
+        head_content(tags.style("html { height: 100%; }")),
         as_fillable_container(
             tags.body(
                 {"class": "bslib-page-fill bslib-gap-spacing", "style": style},
                 attrs,
                 *children,
             )
         ),
```

### Comparing `shiny-0.5.0/shiny/experimental/ui/_sidebar.py` & `shiny-0.5.1/shiny/experimental/ui/_sidebar.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/ui/_tag.py` & `shiny-0.5.1/shiny/experimental/ui/_tag.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/ui/_tooltip.py` & `shiny-0.5.1/shiny/experimental/ui/_tooltip.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/ui/_utils.py` & `shiny-0.5.1/shiny/experimental/ui/_utils.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/ui/_valuebox.py` & `shiny-0.5.1/shiny/experimental/ui/_valuebox.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/www/bslib/components/accordion/accordion.min.js` & `shiny-0.5.1/shiny/experimental/www/bslib/components/accordion/accordion.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/www/bslib/components/accordion/accordion.min.js.map` & `shiny-0.5.1/shiny/experimental/www/bslib/components/accordion/accordion.min.js.map`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/www/bslib/components/card/card.css` & `shiny-0.5.1/shiny/experimental/www/bslib/components/card/card.css`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/www/bslib/components/card/card.min.js` & `shiny-0.5.1/shiny/experimental/www/bslib/components/card/card.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/www/bslib/components/card/card.min.js.map` & `shiny-0.5.1/shiny/experimental/www/bslib/components/card/card.min.js.map`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/www/bslib/components/grid/grid.css` & `shiny-0.5.1/shiny/experimental/www/bslib/components/grid/grid.css`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/www/bslib/components/nav_spacer/nav_spacer.css` & `shiny-0.5.1/shiny/experimental/www/bslib/components/nav_spacer/nav_spacer.css`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/www/bslib/components/page_navbar/page_navbar.css` & `shiny-0.5.1/shiny/experimental/www/bslib/components/page_navbar/page_navbar.css`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/www/bslib/components/sidebar/sidebar.css` & `shiny-0.5.1/shiny/experimental/www/bslib/components/sidebar/sidebar.css`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/www/bslib/components/sidebar/sidebar.min.js` & `shiny-0.5.1/shiny/experimental/www/bslib/components/sidebar/sidebar.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/www/bslib/components/sidebar/sidebar.min.js.map` & `shiny-0.5.1/shiny/experimental/www/bslib/components/sidebar/sidebar.min.js.map`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/www/bslib/components/value_box/value_box.css` & `shiny-0.5.1/shiny/experimental/www/bslib/components/value_box/value_box.css`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/www/bslib/components/webComponents/webComponents.min.js` & `shiny-0.5.1/shiny/experimental/www/bslib/components/webComponents/webComponents.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/experimental/www/bslib/components/webComponents/webComponents.min.js.map` & `shiny-0.5.1/shiny/experimental/www/bslib/components/webComponents/webComponents.min.js.map`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/html_dependencies.py` & `shiny-0.5.1/shiny/html_dependencies.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/http_staticfiles.py` & `shiny-0.5.1/shiny/http_staticfiles.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/input_handler.py` & `shiny-0.5.1/shiny/input_handler.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/module.py` & `shiny-0.5.1/shiny/module.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/plotutils.py` & `shiny-0.5.1/shiny/plotutils.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/reactive/__init__.py` & `shiny-0.5.1/shiny/reactive/__init__.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/reactive/_core.py` & `shiny-0.5.1/shiny/reactive/_core.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/reactive/_poll.py` & `shiny-0.5.1/shiny/reactive/_poll.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/reactive/_reactives.py` & `shiny-0.5.1/shiny/reactive/_reactives.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/render/__init__.py` & `shiny-0.5.1/shiny/render/__init__.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/render/_coordmap.py` & `shiny-0.5.1/shiny/render/_coordmap.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/render/_dataframe.py` & `shiny-0.5.1/shiny/render/_dataframe.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/render/_dataframe_unsafe.py` & `shiny-0.5.1/shiny/render/_dataframe_unsafe.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/render/_render.py` & `shiny-0.5.1/shiny/render/_render.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/render/_try_render_plot.py` & `shiny-0.5.1/shiny/render/_try_render_plot.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/session/_session.py` & `shiny-0.5.1/shiny/session/_session.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/session/_utils.py` & `shiny-0.5.1/shiny/session/_utils.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/types.py` & `shiny-0.5.1/shiny/types.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/ui/__init__.py` & `shiny-0.5.1/shiny/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/ui/_bootstrap.py` & `shiny-0.5.1/shiny/ui/_bootstrap.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/ui/_download_button.py` & `shiny-0.5.1/shiny/ui/_download_button.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/ui/_html_dependencies.py` & `shiny-0.5.1/shiny/ui/_html_dependencies.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/ui/_include_helpers.py` & `shiny-0.5.1/shiny/ui/_include_helpers.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/ui/_input_action_button.py` & `shiny-0.5.1/shiny/ui/_input_action_button.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/ui/_input_check_radio.py` & `shiny-0.5.1/shiny/ui/_input_check_radio.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/ui/_input_date.py` & `shiny-0.5.1/shiny/ui/_input_date.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/ui/_input_file.py` & `shiny-0.5.1/shiny/ui/_input_file.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/ui/_input_numeric.py` & `shiny-0.5.1/shiny/ui/_input_numeric.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/ui/_input_password.py` & `shiny-0.5.1/shiny/ui/_input_password.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/ui/_input_select.py` & `shiny-0.5.1/shiny/ui/_input_select.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/ui/_input_slider.py` & `shiny-0.5.1/shiny/ui/_input_slider.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/ui/_input_text.py` & `shiny-0.5.1/shiny/ui/_input_text.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/ui/_input_update.py` & `shiny-0.5.1/shiny/ui/_input_update.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/ui/_insert.py` & `shiny-0.5.1/shiny/ui/_insert.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/ui/_markdown.py` & `shiny-0.5.1/shiny/ui/_markdown.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/ui/_modal.py` & `shiny-0.5.1/shiny/ui/_modal.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/ui/_navs.py` & `shiny-0.5.1/shiny/ui/_navs.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/ui/_notification.py` & `shiny-0.5.1/shiny/ui/_notification.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/ui/_output.py` & `shiny-0.5.1/shiny/ui/_output.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/ui/_page.py` & `shiny-0.5.1/shiny/ui/_page.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/ui/_plot_output_opts.py` & `shiny-0.5.1/shiny/ui/_plot_output_opts.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/ui/_progress.py` & `shiny-0.5.1/shiny/ui/_progress.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/ui/_utils.py` & `shiny-0.5.1/shiny/ui/_utils.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/ui/_x/_css_unit.py` & `shiny-0.5.1/shiny/ui/_x/_css_unit.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/ui/_x/_fill.py` & `shiny-0.5.1/shiny/ui/_x/_fill.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/ui/_x/_htmldeps.py` & `shiny-0.5.1/shiny/ui/_x/_htmldeps.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         "bslib-sidebar",
         bslib_version,
         source={
             "package": "shiny",
             "subdir": _x_sidebar_path,
         },
         script={"src": "sidebar.min.js"},
+        stylesheet={"href": "sidebar.css"},
         all_files=True,
     )
 
 
 def nav_spacer_dependency() -> HTMLDependency:
     return HTMLDependency(
         "bslib-nav-spacer",
```

### Comparing `shiny-0.5.0/shiny/ui/_x/_sidebar.py` & `shiny-0.5.1/shiny/ui/_x/_sidebar.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/ui/_x/_tag.py` & `shiny-0.5.1/shiny/ui/_x/_tag.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/ui/_x/_utils.py` & `shiny-0.5.1/shiny/ui/_x/_utils.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/ui/dataframe/_dataframe.py` & `shiny-0.5.1/shiny/ui/dataframe/_dataframe.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/_x/bslib/components/nav_spacer/nav_spacer.css` & `shiny-0.5.1/shiny/www/shared/_x/bslib/components/nav_spacer/nav_spacer.css`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/_x/bslib/components/sidebar/sidebar.css` & `shiny-0.5.1/shiny/www/shared/_x/bslib/components/sidebar/sidebar.css`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/_x/bslib/components/sidebar/sidebar.min.js` & `shiny-0.5.1/shiny/www/shared/_x/bslib/components/sidebar/sidebar.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/_x/bslib/components/sidebar/sidebar.min.js.map` & `shiny-0.5.1/shiny/www/shared/_x/bslib/components/sidebar/sidebar.min.js.map`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/bootstrap/bootstrap.bundle.min.js` & `shiny-0.5.1/shiny/www/shared/bootstrap/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/bootstrap/bootstrap.bundle.min.js.map` & `shiny-0.5.1/shiny/www/shared/bootstrap/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/bootstrap/bootstrap.min.css` & `shiny-0.5.1/shiny/www/shared/bootstrap/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/bootstrap/font.css` & `shiny-0.5.1/shiny/www/shared/bootstrap/font.css`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/bootstrap/fonts/HI_diYsKILxRpg3hIP6sJ7fM7PqPMcMnZFqUwX28DBKXhM0.woff` & `shiny-0.5.1/shiny/www/shared/bootstrap/fonts/HI_diYsKILxRpg3hIP6sJ7fM7PqPMcMnZFqUwX28DBKXhM0.woff`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/bootstrap/fonts/HI_diYsKILxRpg3hIP6sJ7fM7PqPMcMnZFqUwX28DMyQhM0.woff` & `shiny-0.5.1/shiny/www/shared/bootstrap/fonts/HI_diYsKILxRpg3hIP6sJ7fM7PqPMcMnZFqUwX28DMyQhM0.woff`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/bootstrap/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTbI1rSg.woff` & `shiny-0.5.1/shiny/www/shared/bootstrap/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTbI1rSg.woff`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/bootstrap/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTsoprSg.woff` & `shiny-0.5.1/shiny/www/shared/bootstrap/fonts/HI_jiYsKILxRpg3hIP6sJ7fM7PqlOPHYvDP_W9O7GQTTsoprSg.woff`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.eot` & `shiny-0.5.1/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.svg` & `shiny-0.5.1/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.ttf` & `shiny-0.5.1/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.woff` & `shiny-0.5.1/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.woff2` & `shiny-0.5.1/shiny/www/shared/bootstrap/fonts/bootstrap/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/bootstrap/fonts/memQYaGs126MiZpBA-UFUIcVXSCEkx2cmqvXlWq8tWZ0Pw86hd0Rk0ZjaVQ.woff` & `shiny-0.5.1/shiny/www/shared/bootstrap/fonts/memQYaGs126MiZpBA-UFUIcVXSCEkx2cmqvXlWq8tWZ0Pw86hd0Rk0ZjaVQ.woff`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/bootstrap/fonts/memQYaGs126MiZpBA-UFUIcVXSCEkx2cmqvXlWq8tWZ0Pw86hd0Rk5hkaVQ.woff` & `shiny-0.5.1/shiny/www/shared/bootstrap/fonts/memQYaGs126MiZpBA-UFUIcVXSCEkx2cmqvXlWq8tWZ0Pw86hd0Rk5hkaVQ.woff`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/bootstrap/fonts/memQYaGs126MiZpBA-UFUIcVXSCEkx2cmqvXlWq8tWZ0Pw86hd0Rk8ZkaVQ.woff` & `shiny-0.5.1/shiny/www/shared/bootstrap/fonts/memQYaGs126MiZpBA-UFUIcVXSCEkx2cmqvXlWq8tWZ0Pw86hd0Rk8ZkaVQ.woff`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/bootstrap/fonts/memQYaGs126MiZpBA-UFUIcVXSCEkx2cmqvXlWq8tWZ0Pw86hd0Rk_RkaVQ.woff` & `shiny-0.5.1/shiny/www/shared/bootstrap/fonts/memQYaGs126MiZpBA-UFUIcVXSCEkx2cmqvXlWq8tWZ0Pw86hd0Rk_RkaVQ.woff`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/bootstrap/fonts/memQYaGs126MiZpBA-UFUIcVXSCEkx2cmqvXlWq8tWZ0Pw86hd0RkxhjaVQ.woff` & `shiny-0.5.1/shiny/www/shared/bootstrap/fonts/memQYaGs126MiZpBA-UFUIcVXSCEkx2cmqvXlWq8tWZ0Pw86hd0RkxhjaVQ.woff`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/bootstrap/fonts/memQYaGs126MiZpBA-UFUIcVXSCEkx2cmqvXlWq8tWZ0Pw86hd0RkyFjaVQ.woff` & `shiny-0.5.1/shiny/www/shared/bootstrap/fonts/memQYaGs126MiZpBA-UFUIcVXSCEkx2cmqvXlWq8tWZ0Pw86hd0RkyFjaVQ.woff`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/bootstrap/fonts/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsg-1y4k.woff` & `shiny-0.5.1/shiny/www/shared/bootstrap/fonts/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsg-1y4k.woff`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/bootstrap/fonts/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsgH1y4k.woff` & `shiny-0.5.1/shiny/www/shared/bootstrap/fonts/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsgH1y4k.woff`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/bootstrap/fonts/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgshZ1y4k.woff` & `shiny-0.5.1/shiny/www/shared/bootstrap/fonts/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgshZ1y4k.woff`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/bootstrap/fonts/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsiH0C4k.woff` & `shiny-0.5.1/shiny/www/shared/bootstrap/fonts/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsiH0C4k.woff`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/bootstrap/fonts/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0C4k.woff` & `shiny-0.5.1/shiny/www/shared/bootstrap/fonts/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0C4k.woff`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/bootstrap/fonts/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjr0C4k.woff` & `shiny-0.5.1/shiny/www/shared/bootstrap/fonts/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjr0C4k.woff`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/dataframe/dataframe.js` & `shiny-0.5.1/shiny/www/shared/dataframe/dataframe.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/dataframe/dataframe.js.map` & `shiny-0.5.1/shiny/www/shared/dataframe/dataframe.js.map`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/css/bootstrap-datepicker3.css` & `shiny-0.5.1/shiny/www/shared/datepicker/css/bootstrap-datepicker3.css`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/css/bootstrap-datepicker3.min.css` & `shiny-0.5.1/shiny/www/shared/datepicker/css/bootstrap-datepicker3.min.css`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/bootstrap-datepicker.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/bootstrap-datepicker.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/bootstrap-datepicker.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/bootstrap-datepicker.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker-en-CA.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker-en-CA.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ar-tn.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ar-tn.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ar.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ar.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.az.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.az.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bg.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bg.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bm.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bm.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bn.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.bn.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ca.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ca.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.cs.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.cs.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.da.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.da.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.de.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.de.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.el.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.el.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-AU.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-AU.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-CA.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-CA.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-GB.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-GB.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-IE.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-IE.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-NZ.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-NZ.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-ZA.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.en-ZA.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.eo.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.eo.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.es.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.es.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.et.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.et.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.eu.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.eu.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fa.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fa.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fi.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fi.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fr-CH.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fr-CH.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fr.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.fr.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.he.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.he.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hi.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hi.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hu.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hu.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hy.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.hy.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.it.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.it.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ka.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ka.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kh.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kh.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kk.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kk.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.km.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.km.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ko.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ko.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kr.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.kr.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.lt.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.lt.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.lv.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.lv.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.mk.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.mk.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.mn.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.mn.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.nl-BE.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.nl-BE.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.nl.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.nl.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.no.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.no.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.oc.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.oc.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.pl.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.pl.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.rs-latin.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.rs-latin.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.rs.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.rs.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ru.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ru.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.si.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.si.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sq.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sq.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sr.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.sr.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ta.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.ta.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.tg.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.tg.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.th.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.th.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.tk.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.tk.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uk.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uk.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uz-cyrl.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uz-cyrl.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uz-latn.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.uz-latn.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.vi.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.vi.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.zh-CN.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.zh-CN.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.zh-TW.min.js` & `shiny-0.5.1/shiny/www/shared/datepicker/js/locales/bootstrap-datepicker.zh-TW.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/scss/build3.scss` & `shiny-0.5.1/shiny/www/shared/datepicker/scss/build3.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/datepicker/scss/datepicker3.scss` & `shiny-0.5.1/shiny/www/shared/datepicker/scss/datepicker3.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/highlight/LICENSE` & `shiny-0.5.1/shiny/www/shared/highlight/LICENSE`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/highlight/classref.txt` & `shiny-0.5.1/shiny/www/shared/highlight/classref.txt`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/highlight/highlight.pack.js` & `shiny-0.5.1/shiny/www/shared/highlight/highlight.pack.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/highlight/rstudio.css` & `shiny-0.5.1/shiny/www/shared/highlight/rstudio.css`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/ionrangeslider/css/ion.rangeSlider.css` & `shiny-0.5.1/shiny/www/shared/ionrangeslider/css/ion.rangeSlider.css`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/ionrangeslider/js/ion.rangeSlider.js` & `shiny-0.5.1/shiny/www/shared/ionrangeslider/js/ion.rangeSlider.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/ionrangeslider/js/ion.rangeSlider.min.js` & `shiny-0.5.1/shiny/www/shared/ionrangeslider/js/ion.rangeSlider.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/ionrangeslider/scss/_base.scss` & `shiny-0.5.1/shiny/www/shared/ionrangeslider/scss/_base.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/ionrangeslider/scss/shiny.scss` & `shiny-0.5.1/shiny/www/shared/ionrangeslider/scss/shiny.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/jquery/jquery-3.6.0.js` & `shiny-0.5.1/shiny/www/shared/jquery/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/jquery/jquery-3.6.0.min.js` & `shiny-0.5.1/shiny/www/shared/jquery/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/jquery/jquery-3.6.0.min.map` & `shiny-0.5.1/shiny/www/shared/jquery/jquery-3.6.0.min.map`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/jqueryui/AUTHORS.txt` & `shiny-0.5.1/shiny/www/shared/jqueryui/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/jqueryui/LICENSE.txt` & `shiny-0.5.1/shiny/www/shared/jqueryui/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/jqueryui/images/ui-icons_444444_256x240.png` & `shiny-0.5.1/shiny/www/shared/jqueryui/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/jqueryui/images/ui-icons_555555_256x240.png` & `shiny-0.5.1/shiny/www/shared/jqueryui/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/jqueryui/images/ui-icons_777620_256x240.png` & `shiny-0.5.1/shiny/www/shared/jqueryui/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/jqueryui/images/ui-icons_777777_256x240.png` & `shiny-0.5.1/shiny/www/shared/jqueryui/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/jqueryui/images/ui-icons_cc0000_256x240.png` & `shiny-0.5.1/shiny/www/shared/jqueryui/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/jqueryui/images/ui-icons_ffffff_256x240.png` & `shiny-0.5.1/shiny/www/shared/jqueryui/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/jqueryui/index.html` & `shiny-0.5.1/shiny/www/shared/jqueryui/index.html`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/jqueryui/jquery-ui.css` & `shiny-0.5.1/shiny/www/shared/jqueryui/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/jqueryui/jquery-ui.js` & `shiny-0.5.1/shiny/www/shared/jqueryui/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/jqueryui/jquery-ui.min.css` & `shiny-0.5.1/shiny/www/shared/jqueryui/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/jqueryui/jquery-ui.min.js` & `shiny-0.5.1/shiny/www/shared/jqueryui/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/jqueryui/jquery-ui.structure.css` & `shiny-0.5.1/shiny/www/shared/jqueryui/jquery-ui.structure.css`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/jqueryui/jquery-ui.structure.min.css` & `shiny-0.5.1/shiny/www/shared/jqueryui/jquery-ui.structure.min.css`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/jqueryui/jquery-ui.theme.css` & `shiny-0.5.1/shiny/www/shared/jqueryui/jquery-ui.theme.css`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/jqueryui/jquery-ui.theme.min.css` & `shiny-0.5.1/shiny/www/shared/jqueryui/jquery-ui.theme.min.css`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/requirejs/require.min.js` & `shiny-0.5.1/shiny/www/shared/requirejs/require.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/selectize/accessibility/js/selectize-plugin-a11y.js` & `shiny-0.5.1/shiny/www/shared/selectize/accessibility/js/selectize-plugin-a11y.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/selectize/accessibility/js/selectize-plugin-a11y.min.js` & `shiny-0.5.1/shiny/www/shared/selectize/accessibility/js/selectize-plugin-a11y.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/selectize/css/selectize.bootstrap3.css` & `shiny-0.5.1/shiny/www/shared/selectize/css/selectize.bootstrap3.css`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/selectize/js/selectize.min.js` & `shiny-0.5.1/shiny/www/shared/selectize/js/selectize.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/selectize/scss/plugins/dropdown_header.scss` & `shiny-0.5.1/shiny/www/shared/selectize/scss/plugins/dropdown_header.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/selectize/scss/plugins/remove_button.scss` & `shiny-0.5.1/shiny/www/shared/selectize/scss/plugins/remove_button.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/selectize/scss/selectize.bootstrap3.scss` & `shiny-0.5.1/shiny/www/shared/selectize/scss/selectize.bootstrap3.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/selectize/scss/selectize.bootstrap4.scss` & `shiny-0.5.1/shiny/www/shared/selectize/scss/selectize.bootstrap4.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/selectize/scss/selectize.default.scss` & `shiny-0.5.1/shiny/www/shared/selectize/scss/selectize.default.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/selectize/scss/selectize.scss` & `shiny-0.5.1/shiny/www/shared/selectize/scss/selectize.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/shiny-autoreload.js` & `shiny-0.5.1/shiny/www/shared/shiny-autoreload.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/shiny-autoreload.js.map` & `shiny-0.5.1/shiny/www/shared/shiny-autoreload.js.map`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/shiny-showcase.css` & `shiny-0.5.1/shiny/www/shared/shiny-showcase.css`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/shiny-showcase.js` & `shiny-0.5.1/shiny/www/shared/shiny-showcase.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/shiny-showcase.js.map` & `shiny-0.5.1/shiny/www/shared/shiny-showcase.js.map`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/shiny-testmode.js.map` & `shiny-0.5.1/shiny/www/shared/shiny-testmode.js.map`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/shiny.js` & `shiny-0.5.1/shiny/www/shared/shiny.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/shiny.js.map` & `shiny-0.5.1/shiny/www/shared/shiny.js.map`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/shiny.min.css` & `shiny-0.5.1/shiny/www/shared/shiny.min.css`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/shiny.min.js` & `shiny-0.5.1/shiny/www/shared/shiny.min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/shiny.min.js.map` & `shiny-0.5.1/shiny/www/shared/shiny.min.js.map`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/shiny_scss/bootstrap.scss` & `shiny-0.5.1/shiny/www/shared/shiny_scss/bootstrap.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/shiny_scss/shiny.scss` & `shiny-0.5.1/shiny/www/shared/shiny_scss/shiny.scss`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/showdown/compressed/showdown.js` & `shiny-0.5.1/shiny/www/shared/showdown/compressed/showdown.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/showdown/license.txt` & `shiny-0.5.1/shiny/www/shared/showdown/license.txt`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/showdown/src/showdown.js` & `shiny-0.5.1/shiny/www/shared/showdown/src/showdown.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny/www/shared/strftime/strftime-min.js` & `shiny-0.5.1/shiny/www/shared/strftime/strftime-min.js`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny.egg-info/PKG-INFO` & `shiny-0.5.1/shiny.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shiny
-Version: 0.5.0
+Version: 0.5.1
 Summary: A web development framework for Python.
 Home-page: https://github.com/rstudio/py-shiny
 Author: Winston Chang
 Author-email: winston@rstudio.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/rstudio/py-shiny/issues
 Project-URL: Documentation, https://shiny.posit.co/py/
```

### Comparing `shiny-0.5.0/shiny.egg-info/SOURCES.txt` & `shiny-0.5.1/shiny.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/shiny.egg-info/requires.txt` & `shiny-0.5.1/shiny.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/tests/asyncio_prevent.py` & `shiny-0.5.1/tests/asyncio_prevent.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/tests/mocktime.py` & `shiny-0.5.1/tests/mocktime.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/tests/test_e2e_regex_matching.py` & `shiny-0.5.1/tests/test_e2e_regex_matching.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/tests/test_markdown.py` & `shiny-0.5.1/tests/test_markdown.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/tests/test_modules.py` & `shiny-0.5.1/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/tests/test_namespaces.py` & `shiny-0.5.1/tests/test_namespaces.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/tests/test_navs.py` & `shiny-0.5.1/tests/test_navs.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/tests/test_poll.py` & `shiny-0.5.1/tests/test_poll.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/tests/test_reactives.py` & `shiny-0.5.1/tests/test_reactives.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/tests/test_shinysession.py` & `shiny-0.5.1/tests/test_shinysession.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/tests/test_static.py` & `shiny-0.5.1/tests/test_static.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/tests/test_ui.py` & `shiny-0.5.1/tests/test_ui.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/tests/test_ui_dependencies.py` & `shiny-0.5.1/tests/test_ui_dependencies.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/tests/test_utils.py` & `shiny-0.5.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/tests/test_utils_async.py` & `shiny-0.5.1/tests/test_utils_async.py`

 * *Files identical despite different names*

### Comparing `shiny-0.5.0/tests/test_x_sidebar.py` & `shiny-0.5.1/tests/test_x_sidebar.py`

 * *Files identical despite different names*

