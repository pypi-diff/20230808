# Comparing `tmp/sigmaepsilon.core-0.0.1.tar.gz` & `tmp/sigmaepsilon.core-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigmaepsilon.core-0.0.1.tar", last modified: Sun Jul  2 17:51:05 2023, max compression
+gzip compressed data, was "sigmaepsilon.core-1.0.0.tar", last modified: Tue Aug  8 15:41:26 2023, max compression
```

## Comparing `sigmaepsilon.core-0.0.1.tar` & `sigmaepsilon.core-1.0.0.tar`

### file list

```diff
@@ -1,191 +1,73 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:05.683476 sigmaepsilon.core-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:04.245901 sigmaepsilon.core-0.0.1/.circleci/
--rw-rw-rw-   0        0        0     6032 2023-07-01 21:32:16.000000 sigmaepsilon.core-0.0.1/.circleci/config.yml
--rw-rw-rw-   0        0        0     3246 2023-07-01 10:28:29.000000 sigmaepsilon.core-0.0.1/.gitignore
--rw-rw-rw-   0        0        0      954 2023-06-27 21:10:36.000000 sigmaepsilon.core-0.0.1/.readthedocs.yaml
--rw-rw-rw-   0        0        0     1090 2023-06-27 20:52:03.000000 sigmaepsilon.core-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      225 2023-07-01 12:37:53.000000 sigmaepsilon.core-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4742 2023-07-02 17:51:05.682482 sigmaepsilon.core-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2463 2023-07-02 12:29:34.000000 sigmaepsilon.core-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:04.252900 sigmaepsilon.core-0.0.1/docs/
--rw-rw-rw-   0        0        0      658 2022-09-19 20:50:54.000000 sigmaepsilon.core-0.0.1/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:04.165695 sigmaepsilon.core-0.0.1/docs/build/
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:04.285668 sigmaepsilon.core-0.0.1/docs/build/doctrees/
--rw-rw-rw-   0        0        0    13934 2023-07-02 13:00:43.000000 sigmaepsilon.core-0.0.1/docs/build/doctrees/README_link.doctree
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:04.322366 sigmaepsilon.core-0.0.1/docs/build/doctrees/api/
--rw-rw-rw-   0        0        0     6698 2023-07-02 17:24:46.000000 sigmaepsilon.core-0.0.1/docs/build/doctrees/api/api_acp.doctree
--rw-rw-rw-   0        0        0    26094 2023-07-02 17:29:02.000000 sigmaepsilon.core-0.0.1/docs/build/doctrees/api/api_cp.doctree
--rw-rw-rw-   0        0        0    25603 2023-07-02 13:00:43.000000 sigmaepsilon.core-0.0.1/docs/build/doctrees/api/api_formatting.doctree
--rw-rw-rw-   0        0        0     6318 2023-07-02 13:00:43.000000 sigmaepsilon.core-0.0.1/docs/build/doctrees/api/api_infix.doctree
--rw-rw-rw-   0        0        0    32934 2023-07-02 16:47:02.000000 sigmaepsilon.core-0.0.1/docs/build/doctrees/api/api_meta.doctree
--rw-rw-rw-   0        0        0    38019 2023-07-02 17:17:45.000000 sigmaepsilon.core-0.0.1/docs/build/doctrees/api/api_wrapping.doctree
--rw-rw-rw-   0        0        0     2805 2023-07-02 17:27:52.000000 sigmaepsilon.core-0.0.1/docs/build/doctrees/api.doctree
--rw-rw-rw-   0        0        0  3811222 2023-07-02 17:29:02.000000 sigmaepsilon.core-0.0.1/docs/build/doctrees/environment.pickle
--rw-rw-rw-   0        0        0  3702322 2023-07-02 13:00:43.000000 sigmaepsilon.core-0.0.1/docs/build/doctrees/index.doctree
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:04.165695 sigmaepsilon.core-0.0.1/docs/build/doctrees/nbsphinx/
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:04.327366 sigmaepsilon.core-0.0.1/docs/build/doctrees/nbsphinx/notebooks/
--rw-rw-rw-   0        0        0      264 2023-07-01 22:25:02.000000 sigmaepsilon.core-0.0.1/docs/build/doctrees/nbsphinx/notebooks/notebook1.ipynb
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:04.334365 sigmaepsilon.core-0.0.1/docs/build/doctrees/notebooks/
--rw-rw-rw-   0        0        0     4333 2023-07-01 22:25:03.000000 sigmaepsilon.core-0.0.1/docs/build/doctrees/notebooks/notebook1.doctree
--rw-rw-rw-   0        0        0     2725 2023-07-01 22:25:03.000000 sigmaepsilon.core-0.0.1/docs/build/doctrees/user_guide.doctree
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:04.609847 sigmaepsilon.core-0.0.1/docs/build/html/
--rw-rw-rw-   0        0        0      234 2023-07-02 17:29:02.000000 sigmaepsilon.core-0.0.1/docs/build/html/.buildinfo
--rw-rw-rw-   0        0        0    17534 2023-07-02 13:00:43.000000 sigmaepsilon.core-0.0.1/docs/build/html/README_link.html
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:04.648775 sigmaepsilon.core-0.0.1/docs/build/html/_modules/
--rw-rw-rw-   0        0        0    11570 2023-07-02 17:29:02.000000 sigmaepsilon.core-0.0.1/docs/build/html/_modules/index.html
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:04.166693 sigmaepsilon.core-0.0.1/docs/build/html/_modules/sigmaepsilon/
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:04.969035 sigmaepsilon.core-0.0.1/docs/build/html/_modules/sigmaepsilon/core/
--rw-rw-rw-   0        0        0    21109 2023-07-02 13:00:44.000000 sigmaepsilon.core-0.0.1/docs/build/html/_modules/sigmaepsilon/core/abstract.html
--rw-rw-rw-   0        0        0    29797 2023-07-02 17:24:46.000000 sigmaepsilon.core-0.0.1/docs/build/html/_modules/sigmaepsilon/core/acp.html
--rw-rw-rw-   0        0        0    16338 2023-07-01 22:25:03.000000 sigmaepsilon.core-0.0.1/docs/build/html/_modules/sigmaepsilon/core/attr.html
--rw-rw-rw-   0        0        0    28051 2023-07-02 17:29:02.000000 sigmaepsilon.core-0.0.1/docs/build/html/_modules/sigmaepsilon/core/cp.html
--rw-rw-rw-   0        0        0    21935 2023-07-02 11:08:39.000000 sigmaepsilon.core-0.0.1/docs/build/html/_modules/sigmaepsilon/core/formatting.html
--rw-rw-rw-   0        0        0    17555 2023-07-01 22:25:03.000000 sigmaepsilon.core-0.0.1/docs/build/html/_modules/sigmaepsilon/core/infix.html
--rw-rw-rw-   0        0        0    30667 2023-07-02 16:47:02.000000 sigmaepsilon.core-0.0.1/docs/build/html/_modules/sigmaepsilon/core/meta.html
--rw-rw-rw-   0        0        0    15553 2023-07-01 22:25:03.000000 sigmaepsilon.core-0.0.1/docs/build/html/_modules/sigmaepsilon/core/typing.html
--rw-rw-rw-   0        0        0    37117 2023-07-02 17:17:45.000000 sigmaepsilon.core-0.0.1/docs/build/html/_modules/sigmaepsilon/core/wrapping.html
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:04.986019 sigmaepsilon.core-0.0.1/docs/build/html/_sources/
--rw-rw-rw-   0        0        0       35 2023-07-01 22:27:28.000000 sigmaepsilon.core-0.0.1/docs/build/html/_sources/README_link.md.txt
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:05.018020 sigmaepsilon.core-0.0.1/docs/build/html/_sources/api/
--rw-rw-rw-   0        0        0      159 2023-07-02 17:24:42.000000 sigmaepsilon.core-0.0.1/docs/build/html/_sources/api/api_acp.rst.txt
--rw-rw-rw-   0        0        0      107 2023-07-02 17:27:37.000000 sigmaepsilon.core-0.0.1/docs/build/html/_sources/api/api_cp.rst.txt
--rw-rw-rw-   0        0        0       97 2023-07-02 11:06:16.000000 sigmaepsilon.core-0.0.1/docs/build/html/_sources/api/api_formatting.rst.txt
--rw-rw-rw-   0        0        0      107 2023-07-02 11:05:33.000000 sigmaepsilon.core-0.0.1/docs/build/html/_sources/api/api_infix.rst.txt
--rw-rw-rw-   0        0        0      270 2023-07-02 10:59:02.000000 sigmaepsilon.core-0.0.1/docs/build/html/_sources/api/api_meta.rst.txt
--rw-rw-rw-   0        0        0       89 2023-07-02 10:59:51.000000 sigmaepsilon.core-0.0.1/docs/build/html/_sources/api/api_wrapping.rst.txt
--rw-rw-rw-   0        0        0      172 2023-07-02 17:27:29.000000 sigmaepsilon.core-0.0.1/docs/build/html/_sources/api.rst.txt
--rw-rw-rw-   0        0        0      230 2023-07-02 12:18:50.000000 sigmaepsilon.core-0.0.1/docs/build/html/_sources/index.rst.txt
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:05.023059 sigmaepsilon.core-0.0.1/docs/build/html/_sources/notebooks/
--rw-rw-rw-   0        0        0      267 2023-07-01 22:24:54.000000 sigmaepsilon.core-0.0.1/docs/build/html/_sources/notebooks/notebook1.ipynb.txt
--rw-rw-rw-   0        0        0       85 2023-07-01 22:13:56.000000 sigmaepsilon.core-0.0.1/docs/build/html/_sources/user_guide.rst.txt
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:05.040020 sigmaepsilon.core-0.0.1/docs/build/html/_sphinx_design_static/
--rw-rw-rw-   0        0        0    48418 2023-07-01 22:19:59.000000 sigmaepsilon.core-0.0.1/docs/build/html/_sphinx_design_static/design-style.1e8bd061cd6da7fc9cf755528e8ffc24.min.css
--rw-rw-rw-   0        0        0      797 2023-07-01 22:19:59.000000 sigmaepsilon.core-0.0.1/docs/build/html/_sphinx_design_static/design-tabs.js
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:05.245633 sigmaepsilon.core-0.0.1/docs/build/html/_static/
--rw-rw-rw-   0        0        0    15715 2023-07-02 17:29:02.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/basic.css
--rw-rw-rw-   0        0        0      313 2023-07-01 22:19:31.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/check-solid.svg
--rw-rw-rw-   0        0        0     9031 2023-07-01 22:19:31.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/clipboard.min.js
--rw-rw-rw-   0        0        0      411 2023-07-01 22:19:31.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/copy-button.svg
--rw-rw-rw-   0        0        0     2060 2023-07-01 22:19:31.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/copybutton.css
--rw-rw-rw-   0        0        0     8714 2023-07-02 17:29:02.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/copybutton.js
--rw-rw-rw-   0        0        0     2698 2023-07-01 22:19:31.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/copybutton_funcs.js
--rw-rw-rw-   0        0        0    48418 2023-07-01 22:19:59.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/design-style.1e8bd061cd6da7fc9cf755528e8ffc24.min.css
--rw-rw-rw-   0        0        0      797 2023-07-01 22:19:59.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/design-tabs.js
--rw-rw-rw-   0        0        0     4472 2023-07-01 22:19:28.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/doctools.js
--rw-rw-rw-   0        0        0      433 2023-07-02 17:29:02.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/documentation_options.js
--rw-rw-rw-   0        0        0      286 2023-07-01 22:19:28.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/file.png
--rw-rw-rw-   0        0        0     4957 2023-07-02 17:29:02.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/language_data.js
--rw-rw-rw-   0        0        0       90 2023-07-01 22:19:28.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/minus.png
--rw-rw-rw-   0        0        0     4467 2023-07-01 22:19:33.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/nbsphinx-broken-thumbnail.svg
--rw-rw-rw-   0        0        0     7120 2023-07-02 11:09:08.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/nbsphinx-code-cells.css
--rw-rw-rw-   0        0        0      584 2023-07-01 22:19:33.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/nbsphinx-gallery.css
--rw-rw-rw-   0        0        0     2871 2023-07-01 22:19:33.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/nbsphinx-no-thumbnail.svg
--rw-rw-rw-   0        0        0       90 2023-07-01 22:19:28.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/plus.png
--rw-rw-rw-   0        0        0    12908 2023-07-02 17:36:42.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/pygments.css
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:05.303124 sigmaepsilon.core-0.0.1/docs/build/html/_static/scripts/
--rw-rw-rw-   0        0        0    80813 2023-07-01 22:19:31.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/scripts/bootstrap.js
--rw-rw-rw-   0        0        0      237 2023-07-01 22:19:31.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/scripts/bootstrap.js.LICENSE.txt
--rw-rw-rw-   0        0        0   335757 2023-07-01 22:19:31.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/scripts/bootstrap.js.map
--rw-rw-rw-   0        0        0     4456 2023-07-01 22:19:31.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/scripts/pydata-sphinx-theme.js
--rw-rw-rw-   0        0        0    19648 2023-07-01 22:19:31.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/scripts/pydata-sphinx-theme.js.map
--rw-rw-rw-   0        0        0    18215 2023-07-01 22:19:28.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/searchtools.js
--rw-rw-rw-   0        0        0     4712 2023-07-01 22:19:28.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/sphinx_highlight.js
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:05.321122 sigmaepsilon.core-0.0.1/docs/build/html/_static/styles/
--rw-rw-rw-   0        0        0   176654 2023-07-01 22:19:31.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/styles/bootstrap.css
--rw-rw-rw-   0        0        0    63341 2023-07-01 22:19:31.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/styles/pydata-sphinx-theme.css
--rw-rw-rw-   0        0        0      106 2023-07-01 22:19:31.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/styles/theme.css
--rw-rw-rw-   0        0        0     2589 2023-07-01 22:19:31.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/tabs.css
--rw-rw-rw-   0        0        0      782 2023-07-01 22:19:31.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/tabs.js
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:04.182694 sigmaepsilon.core-0.0.1/docs/build/html/_static/vendor/
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:04.183693 sigmaepsilon.core-0.0.1/docs/build/html/_static/vendor/fontawesome/
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:05.328141 sigmaepsilon.core-0.0.1/docs/build/html/_static/vendor/fontawesome/6.1.2/
--rw-rw-rw-   0        0        0     7427 2023-07-01 22:19:31.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:05.334209 sigmaepsilon.core-0.0.1/docs/build/html/_static/vendor/fontawesome/6.1.2/css/
--rw-rw-rw-   0        0        0   101691 2023-07-01 22:19:31.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:05.381506 sigmaepsilon.core-0.0.1/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/
--rw-rw-rw-   0        0        0   181264 2023-07-01 22:19:31.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
--rw-rw-rw-   0        0        0   105112 2023-07-01 22:19:31.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
--rw-rw-rw-   0        0        0    60236 2023-07-01 22:19:31.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
--rw-rw-rw-   0        0        0    24028 2023-07-01 22:19:31.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
--rw-rw-rw-   0        0        0   389948 2023-07-01 22:19:31.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
--rw-rw-rw-   0        0        0   154840 2023-07-01 22:19:31.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
--rw-rw-rw-   0        0        0    10084 2023-07-01 22:19:31.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
--rw-rw-rw-   0        0        0     4776 2023-07-01 22:19:31.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
--rw-rw-rw-   0        0        0     1863 2023-07-01 22:19:31.000000 sigmaepsilon.core-0.0.1/docs/build/html/_static/webpack-macros.html
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:05.585801 sigmaepsilon.core-0.0.1/docs/build/html/api/
--rw-rw-rw-   0        0        0    14622 2023-07-02 17:24:46.000000 sigmaepsilon.core-0.0.1/docs/build/html/api/api_acp.html
--rw-rw-rw-   0        0        0    25930 2023-07-02 17:29:02.000000 sigmaepsilon.core-0.0.1/docs/build/html/api/api_cp.html
--rw-rw-rw-   0        0        0    24478 2023-07-02 13:00:44.000000 sigmaepsilon.core-0.0.1/docs/build/html/api/api_formatting.html
--rw-rw-rw-   0        0        0    16702 2023-07-02 13:00:44.000000 sigmaepsilon.core-0.0.1/docs/build/html/api/api_infix.html
--rw-rw-rw-   0        0        0    34128 2023-07-02 16:47:02.000000 sigmaepsilon.core-0.0.1/docs/build/html/api/api_meta.html
--rw-rw-rw-   0        0        0    35088 2023-07-02 17:17:45.000000 sigmaepsilon.core-0.0.1/docs/build/html/api/api_wrapping.html
--rw-rw-rw-   0        0        0    18736 2023-07-02 17:29:02.000000 sigmaepsilon.core-0.0.1/docs/build/html/api.html
--rw-rw-rw-   0        0        0    17157 2023-07-02 17:29:02.000000 sigmaepsilon.core-0.0.1/docs/build/html/genindex.html
--rw-rw-rw-   0        0        0    19039 2023-07-02 17:29:02.000000 sigmaepsilon.core-0.0.1/docs/build/html/index.html
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:05.623804 sigmaepsilon.core-0.0.1/docs/build/html/notebooks/
--rw-rw-rw-   0        0        0    14548 2023-07-01 22:25:03.000000 sigmaepsilon.core-0.0.1/docs/build/html/notebooks/notebook1.html
--rw-rw-rw-   0        0        0      264 2023-07-01 22:25:02.000000 sigmaepsilon.core-0.0.1/docs/build/html/notebooks/notebook1.ipynb
--rw-rw-rw-   0        0        0      660 2023-07-02 17:29:02.000000 sigmaepsilon.core-0.0.1/docs/build/html/objects.inv
--rw-rw-rw-   0        0        0    12323 2023-07-02 17:29:02.000000 sigmaepsilon.core-0.0.1/docs/build/html/py-modindex.html
--rw-rw-rw-   0        0        0    11425 2023-07-02 17:29:02.000000 sigmaepsilon.core-0.0.1/docs/build/html/search.html
--rw-rw-rw-   0        0        0    10592 2023-07-02 17:29:02.000000 sigmaepsilon.core-0.0.1/docs/build/html/searchindex.js
--rw-rw-rw-   0        0        0    13744 2023-07-01 22:25:03.000000 sigmaepsilon.core-0.0.1/docs/build/html/user_guide.html
--rwxrwxrwx   0        0        0      804 2022-09-19 20:50:54.000000 sigmaepsilon.core-0.0.1/docs/make.bat
--rw-rw-rw-   0        0        0      114 2023-07-02 12:20:40.000000 sigmaepsilon.core-0.0.1/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:05.626805 sigmaepsilon.core-0.0.1/docs/source/
--rw-rw-rw-   0        0        0       35 2023-07-01 22:27:28.000000 sigmaepsilon.core-0.0.1/docs/source/README_link.md
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:05.631805 sigmaepsilon.core-0.0.1/docs/source/api/
--rw-rw-rw-   0        0        0      107 2023-07-02 17:27:37.000000 sigmaepsilon.core-0.0.1/docs/source/api/api_cp.rst
--rw-rw-rw-   0        0        0       97 2023-07-02 11:06:16.000000 sigmaepsilon.core-0.0.1/docs/source/api/api_formatting.rst
--rw-rw-rw-   0        0        0      107 2023-07-02 11:05:33.000000 sigmaepsilon.core-0.0.1/docs/source/api/api_infix.rst
--rw-rw-rw-   0        0        0      270 2023-07-02 10:59:02.000000 sigmaepsilon.core-0.0.1/docs/source/api/api_meta.rst
--rw-rw-rw-   0        0        0       89 2023-07-02 10:59:51.000000 sigmaepsilon.core-0.0.1/docs/source/api/api_wrapping.rst
--rw-rw-rw-   0        0        0      172 2023-07-02 17:27:29.000000 sigmaepsilon.core-0.0.1/docs/source/api.rst
--rw-rw-rw-   0        0        0     4184 2023-07-02 12:23:11.000000 sigmaepsilon.core-0.0.1/docs/source/conf.py
--rw-rw-rw-   0        0        0      230 2023-07-02 12:18:50.000000 sigmaepsilon.core-0.0.1/docs/source/index.rst
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:05.632818 sigmaepsilon.core-0.0.1/docs/source/notebooks/
--rw-rw-rw-   0        0        0      267 2023-07-01 22:24:54.000000 sigmaepsilon.core-0.0.1/docs/source/notebooks/notebook1.ipynb
--rw-rw-rw-   0        0        0     1618 2023-07-01 22:18:37.000000 sigmaepsilon.core-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       34 2023-07-01 20:14:51.000000 sigmaepsilon.core-0.0.1/requirements-dev.txt
--rw-rw-rw-   0        0        0       18 2023-07-01 20:14:00.000000 sigmaepsilon.core-0.0.1/requirements-test.txt
--rw-rw-rw-   0        0        0       12 2023-07-01 20:12:15.000000 sigmaepsilon.core-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-02 17:51:05.683476 sigmaepsilon.core-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:04.185694 sigmaepsilon.core-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:04.186695 sigmaepsilon.core-0.0.1/src/sigmaepsilon/
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:05.676474 sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/
--rw-rw-rw-   0        0        0     2588 2023-07-01 22:02:56.000000 sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/__init__.py
--rw-rw-rw-   0        0        0     4816 2023-07-02 13:00:06.000000 sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/abstract.py
--rw-rw-rw-   0        0        0     5124 2023-07-02 17:27:48.000000 sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/acp.py
--rw-rw-rw-   0        0        0     2842 2023-07-01 08:57:26.000000 sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/alphabet.py
--rw-rw-rw-   0        0        0     1021 2022-12-01 08:15:53.000000 sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/attr.py
--rw-rw-rw-   0        0        0    35644 2023-06-29 18:56:17.000000 sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/colors.py
--rw-rw-rw-   0        0        0     6217 2023-07-02 17:28:58.000000 sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/cp.py
--rw-rw-rw-   0        0        0      794 2023-06-30 22:49:33.000000 sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/decorate.py
--rw-rw-rw-   0        0        0     5080 2023-06-30 22:18:08.000000 sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/downloads.py
--rw-rw-rw-   0        0        0     2722 2023-06-29 18:43:55.000000 sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/formatting.py
--rw-rw-rw-   0        0        0     1068 2023-06-30 23:18:48.000000 sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/infix.py
--rw-rw-rw-   0        0        0      465 2023-07-02 17:34:55.000000 sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/io.py
--rw-rw-rw-   0        0        0     2417 2023-06-29 18:54:49.000000 sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/kwargtools.py
--rw-rw-rw-   0        0        0     5003 2023-07-02 16:46:41.000000 sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/meta.py
--rw-rw-rw-   0        0        0     1125 2023-06-29 19:07:13.000000 sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/osutils.py
--rw-rw-rw-   0        0        0     6757 2023-06-30 23:16:37.000000 sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/signature.py
--rw-rw-rw-   0        0        0      654 2023-07-02 17:31:48.000000 sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/testing.py
--rw-rw-rw-   0        0        0      410 2023-06-29 18:30:18.000000 sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/thirdparty.py
--rw-rw-rw-   0        0        0      924 2023-06-29 21:58:42.000000 sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/typing.py
--rw-rw-rw-   0        0        0      505 2023-07-02 17:33:21.000000 sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/warning.py
--rw-rw-rw-   0        0        0     8039 2023-07-02 17:17:41.000000 sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/wrapping.py
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:05.656963 sigmaepsilon.core-0.0.1/src/sigmaepsilon.core.egg-info/
--rw-rw-rw-   0        0        0     4742 2023-07-02 17:51:04.000000 sigmaepsilon.core-0.0.1/src/sigmaepsilon.core.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6050 2023-07-02 17:51:04.000000 sigmaepsilon.core-0.0.1/src/sigmaepsilon.core.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 17:51:04.000000 sigmaepsilon.core-0.0.1/src/sigmaepsilon.core.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      186 2023-07-02 17:51:04.000000 sigmaepsilon.core-0.0.1/src/sigmaepsilon.core.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-02 17:51:04.000000 sigmaepsilon.core-0.0.1/src/sigmaepsilon.core.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-02 17:51:05.682482 sigmaepsilon.core-0.0.1/tests/
--rw-rw-rw-   0        0        0        0 2023-07-01 08:52:55.000000 sigmaepsilon.core-0.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0      619 2023-06-27 21:02:43.000000 sigmaepsilon.core-0.0.1/tests/test_attr.py
--rw-rw-rw-   0        0        0      392 2023-06-30 23:13:05.000000 sigmaepsilon.core-0.0.1/tests/test_infix.py
--rw-rw-rw-   0        0        0     3617 2023-06-27 21:20:04.000000 sigmaepsilon.core-0.0.1/tests/test_meta.py
--rw-rw-rw-   0        0        0      388 2023-06-27 21:02:56.000000 sigmaepsilon.core-0.0.1/tests/test_property.py
--rw-rw-rw-   0        0        0     3132 2023-06-30 22:54:25.000000 sigmaepsilon.core-0.0.1/tests/test_tools.py
--rw-rw-rw-   0        0        0     1649 2023-06-27 21:03:06.000000 sigmaepsilon.core-0.0.1/tests/test_wrap.py
--rw-rw-rw-   0        0        0      261 2023-07-01 20:38:53.000000 sigmaepsilon.core-0.0.1/tox.ini
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:41:26.597715 sigmaepsilon.core-1.0.0/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:41:26.589716 sigmaepsilon.core-1.0.0/.circleci/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5983 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/.circleci/config.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3085 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      920 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/.readthedocs.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1069 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      213 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4717 2023-08-08 15:41:26.597715 sigmaepsilon.core-1.0.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2483 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:41:26.589716 sigmaepsilon.core-1.0.0/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      638 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/docs/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      769 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/docs/make.bat
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/docs/requirements.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:41:26.589716 sigmaepsilon.core-1.0.0/docs/source/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       33 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/docs/source/README_link.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:41:26.589716 sigmaepsilon.core-1.0.0/docs/source/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      102 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/docs/source/api/api_cp.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       92 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/docs/source/api/api_formatting.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      102 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/docs/source/api/api_infix.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      254 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/docs/source/api/api_meta.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       84 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/docs/source/api/api_wrapping.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      162 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/docs/source/api.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4059 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/docs/source/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      214 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/docs/source/index.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:41:26.589716 sigmaepsilon.core-1.0.0/docs/source/notebooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      267 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/docs/source/notebooks/notebook1.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1570 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       31 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/requirements-dev.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       23 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/requirements-test.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       11 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-08 15:41:26.597715 sigmaepsilon.core-1.0.0/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:41:26.585716 sigmaepsilon.core-1.0.0/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:41:26.585716 sigmaepsilon.core-1.0.0/src/sigmaepsilon/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:41:26.593716 sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2510 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4665 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/abstract.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4982 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/acp.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2754 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/alphabet.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      983 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/attr.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    34515 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/colors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6045 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/cp.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      758 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/decorate.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4905 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/downloads.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      104 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2622 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/formatting.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1030 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/infix.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      447 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/io.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2328 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/kwargtools.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4864 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/meta.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      468 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/misc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1085 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/osutils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6562 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/signature.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      630 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/testing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      394 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/thirdparty.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      883 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/typing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      485 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/warning.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7791 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/wrapping.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:41:26.593716 sigmaepsilon.core-1.0.0/src/sigmaepsilon.core.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4717 2023-08-08 15:41:26.000000 sigmaepsilon.core-1.0.0/src/sigmaepsilon.core.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1627 2023-08-08 15:41:26.000000 sigmaepsilon.core-1.0.0/src/sigmaepsilon.core.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-08 15:41:26.000000 sigmaepsilon.core-1.0.0/src/sigmaepsilon.core.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      192 2023-08-08 15:41:26.000000 sigmaepsilon.core-1.0.0/src/sigmaepsilon.core.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-08-08 15:41:26.000000 sigmaepsilon.core-1.0.0/src/sigmaepsilon.core.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:41:26.597715 sigmaepsilon.core-1.0.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      596 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/tests/test_attr.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      375 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/tests/test_infix.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3473 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/tests/test_meta.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1054 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/tests/test_misc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      367 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/tests/test_property.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3038 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/tests/test_tools.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1578 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/tests/test_wrap.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      250 2023-08-08 15:41:10.000000 sigmaepsilon.core-1.0.0/tox.ini
```

### Comparing `sigmaepsilon.core-0.0.1/.readthedocs.yaml` & `sigmaepsilon.core-1.0.0/.readthedocs.yaml`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-# .readthedocs.yaml
-# Read the Docs configuration file
-# See https://docs.readthedocs.io/en/stable/config-file/v2.html for details
-
-# Required
-version: 2
-
-# Set the version of Python and other tools you might need
-build:
-  os: ubuntu-20.04
-  tools:
-    python: "3.10"
-    # You can also specify other tool versions:
-    # nodejs: "16"
-    # rust: "1.55"
-    # golang: "1.17"
-
-# Build documentation in the docs/ directory with Sphinx
-sphinx:
-   configuration: docs/source/conf.py
-
-# If using Sphinx, optionally build your docs in additional formats such as PDF
-# formats:
-#    - pdf
-
-python:
-  # Install our python package before building the docs
-  install:
-    - requirements: docs/requirements.txt
-    - requirements: requirements.txt
-    - method: pip
-      path: .
-
-submodules:                                                                                                                          
+# .readthedocs.yaml
+# Read the Docs configuration file
+# See https://docs.readthedocs.io/en/stable/config-file/v2.html for details
+
+# Required
+version: 2
+
+# Set the version of Python and other tools you might need
+build:
+  os: ubuntu-20.04
+  tools:
+    python: "3.10"
+    # You can also specify other tool versions:
+    # nodejs: "16"
+    # rust: "1.55"
+    # golang: "1.17"
+
+# Build documentation in the docs/ directory with Sphinx
+sphinx:
+   configuration: docs/source/conf.py
+
+# If using Sphinx, optionally build your docs in additional formats such as PDF
+# formats:
+#    - pdf
+
+python:
+  # Install our python package before building the docs
+  install:
+    - requirements: docs/requirements.txt
+    - requirements: requirements.txt
+    - method: pip
+      path: .
+
+submodules:                                                                                                                          
     include: all
```

### Comparing `sigmaepsilon.core-0.0.1/PKG-INFO` & `sigmaepsilon.core-1.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-Metadata-Version: 2.1
-Name: sigmaepsilon.core
-Version: 0.0.1
-Summary: Common developer utilities for Python projects.
-Author-email: SigmaEpsilon <bencebalogh@sigmaepsilon.com>
-Maintainer-email: SigmaEpsilon <bencebalogh@sigmaepsilon.com>
-License: MIT License
-        
-        Copyright (c) 2023 SigmaEpsilon
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/sigma-epsilon/sigmaepsilon.core
-Keywords: engineering,mechanics,science,numerical analysis,finite element method,solid mechanics,optimization
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Operating System :: OS Independent
-Requires-Python: <3.11,>=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: dev
-Provides-Extra: docs
-License-File: LICENSE
-
-# **sigmaepsilon.core** - Common developer utilities for Python projects
-
-[![CircleCI](https://circleci.com/gh/dewloosh/sigmaepsilon.core.svg?style=shield)](https://circleci.com/gh/sigma-epsilon/sigmaepsilon.core)
-[![Documentation Status](https://readthedocs.org/projects/sigmaepsiloncore/badge/?version=latest)](https://sigmaepsiloncore.readthedocs.io/en/latest/?badge=latest)
-[![Python 3.7-3.10](https://img.shields.io/badge/python-3.7%E2%80%923.10-blue)](https://www.python.org)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![PyPI](https://badge.fury.io/py/sigmaepsilon.math.svg)](https://pypi.org/project/sigmaepsilon.math)
-
-The package contains some usefull stuff for general Python development activites that turned out to be highly reusable during developing projects in the SigmaEpsilon namespace.
-
-Some of the most notable contents:
-
-* Metaprogramming
-  * A collection of meta and abstract base classes.
-  * A `classproperty` decorator.
-  * A solution to enforce abstract class properties on a class.
-  
-* Wrapping
-  * An extendible `Wrapper` class and a few factory functions to help you safely wrap objects.
-
-## **Documentation**
-
-The [documentation](https://sigmaepsiloncore.readthedocs.io/en/latest/) is hosted on ReadTheDocs.
-
-## **Installation**
-
-`sigmaepsilon.core` can be installed (either in a virtual enviroment or globally) from PyPI using `pip` on Python >= 3.7:
-
-```console
->>> pip install sigmaepsilon.core
-```
-
-or chechkout with the following command using GitHub CLI
-
-```console
-gh repo clone sigma-epsilon/sigmaepsilon.core
-```
-
-and install from source by typing
-
-```console
->>> pip install .
-```
-
-If you want to run the tests, you can install the necessary optional dependencies like this
-
-```console
->>> pip install ".[test]"
-```
-
-### For developers
-
-For development purposes, it is suggested to install the package in editable mode, with the optional dependencies for both testing, development and documentation
-
-```console
->>> pip install -e ".[test, dev, docs]"
-```
-
-## Testing
-
-To run the tests, run the following command in the root of the project:
-
-```console
->>> pytest
-```
-
-## **License**
-
-This package is licensed under the MIT license. See the attached LICENSE file for the details.
+Metadata-Version: 2.1
+Name: sigmaepsilon.core
+Version: 1.0.0
+Summary: Common developer utilities for Python projects.
+Author-email: SigmaEpsilon <bencebalogh@sigmaepsilon.com>
+Maintainer-email: SigmaEpsilon <bencebalogh@sigmaepsilon.com>
+License: MIT License
+        
+        Copyright (c) 2023 SigmaEpsilon
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/sigma-epsilon/sigmaepsilon.core
+Keywords: engineering,mechanics,science,numerical analysis,finite element method,solid mechanics,optimization
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Operating System :: OS Independent
+Requires-Python: <3.11,>=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: dev
+Provides-Extra: docs
+License-File: LICENSE
+
+# **sigmaepsilon.core** - Common developer utilities for Python projects
+
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/sigma-epsilon/sigmaepsilon.core/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/sigma-epsilon/sigmaepsilon.core/tree/main)
+[![Documentation Status](https://readthedocs.org/projects/sigmaepsiloncore/badge/?version=latest)](https://sigmaepsiloncore.readthedocs.io/en/latest/?badge=latest)
+[![Python 3.7-3.10](https://img.shields.io/badge/python-3.7%E2%80%923.10-blue)](https://www.python.org)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![PyPI](https://badge.fury.io/py/sigmaepsilon.core.svg)](https://pypi.org/project/sigmaepsilon.core)
+
+The package contains some usefull stuff for general Python development activites that turned out to be highly reusable during developing projects in the SigmaEpsilon namespace.
+
+Some of the most notable contents:
+
+* Metaprogramming
+  * A collection of meta and abstract base classes.
+  * A `classproperty` decorator.
+  * A solution to enforce abstract class properties on a class.
+  
+* Wrapping
+  * An extendible `Wrapper` class and a few factory functions to help you safely wrap objects.
+
+## **Documentation**
+
+The [documentation](https://sigmaepsiloncore.readthedocs.io/en/latest/) is hosted on ReadTheDocs.
+
+## **Installation**
+
+`sigmaepsilon.core` can be installed (either in a virtual enviroment or globally) from PyPI using `pip` on Python >= 3.7:
+
+```console
+>>> pip install sigmaepsilon.core
+```
+
+or chechkout with the following command using GitHub CLI
+
+```console
+gh repo clone sigma-epsilon/sigmaepsilon.core
+```
+
+and install from source by typing
+
+```console
+>>> pip install .
+```
+
+If you want to run the tests, you can install the package along with the necessary optional dependencies like this
+
+```console
+>>> pip install ".[test]"
+```
+
+### For developers
+
+For development purposes, it is suggested to install the package in editable mode, with the optional dependencies for both testing, development and documentation
+
+```console
+>>> pip install -e ".[test, dev, docs]"
+```
+
+## Testing
+
+To run the tests, run the following command in the root of the project:
+
+```console
+>>> pytest
+```
+
+## **License**
+
+This package is licensed under the MIT license. See the attached LICENSE file for the details.
```

### Comparing `sigmaepsilon.core-0.0.1/README.md` & `sigmaepsilon.core-1.0.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-# **sigmaepsilon.core** - Common developer utilities for Python projects
-
-[![CircleCI](https://circleci.com/gh/dewloosh/sigmaepsilon.core.svg?style=shield)](https://circleci.com/gh/sigma-epsilon/sigmaepsilon.core)
-[![Documentation Status](https://readthedocs.org/projects/sigmaepsiloncore/badge/?version=latest)](https://sigmaepsiloncore.readthedocs.io/en/latest/?badge=latest)
-[![Python 3.7-3.10](https://img.shields.io/badge/python-3.7%E2%80%923.10-blue)](https://www.python.org)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![PyPI](https://badge.fury.io/py/sigmaepsilon.math.svg)](https://pypi.org/project/sigmaepsilon.math)
-
-The package contains some usefull stuff for general Python development activites that turned out to be highly reusable during developing projects in the SigmaEpsilon namespace.
-
-Some of the most notable contents:
-
-* Metaprogramming
-  * A collection of meta and abstract base classes.
-  * A `classproperty` decorator.
-  * A solution to enforce abstract class properties on a class.
-  
-* Wrapping
-  * An extendible `Wrapper` class and a few factory functions to help you safely wrap objects.
-
-## **Documentation**
-
-The [documentation](https://sigmaepsiloncore.readthedocs.io/en/latest/) is hosted on ReadTheDocs.
-
-## **Installation**
-
-`sigmaepsilon.core` can be installed (either in a virtual enviroment or globally) from PyPI using `pip` on Python >= 3.7:
-
-```console
->>> pip install sigmaepsilon.core
-```
-
-or chechkout with the following command using GitHub CLI
-
-```console
-gh repo clone sigma-epsilon/sigmaepsilon.core
-```
-
-and install from source by typing
-
-```console
->>> pip install .
-```
-
-If you want to run the tests, you can install the necessary optional dependencies like this
-
-```console
->>> pip install ".[test]"
-```
-
-### For developers
-
-For development purposes, it is suggested to install the package in editable mode, with the optional dependencies for both testing, development and documentation
-
-```console
->>> pip install -e ".[test, dev, docs]"
-```
-
-## Testing
-
-To run the tests, run the following command in the root of the project:
-
-```console
->>> pytest
-```
-
-## **License**
-
-This package is licensed under the MIT license. See the attached LICENSE file for the details.
+# **sigmaepsilon.core** - Common developer utilities for Python projects
+
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/sigma-epsilon/sigmaepsilon.core/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/sigma-epsilon/sigmaepsilon.core/tree/main)
+[![Documentation Status](https://readthedocs.org/projects/sigmaepsiloncore/badge/?version=latest)](https://sigmaepsiloncore.readthedocs.io/en/latest/?badge=latest)
+[![Python 3.7-3.10](https://img.shields.io/badge/python-3.7%E2%80%923.10-blue)](https://www.python.org)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![PyPI](https://badge.fury.io/py/sigmaepsilon.core.svg)](https://pypi.org/project/sigmaepsilon.core)
+
+The package contains some usefull stuff for general Python development activites that turned out to be highly reusable during developing projects in the SigmaEpsilon namespace.
+
+Some of the most notable contents:
+
+* Metaprogramming
+  * A collection of meta and abstract base classes.
+  * A `classproperty` decorator.
+  * A solution to enforce abstract class properties on a class.
+  
+* Wrapping
+  * An extendible `Wrapper` class and a few factory functions to help you safely wrap objects.
+
+## **Documentation**
+
+The [documentation](https://sigmaepsiloncore.readthedocs.io/en/latest/) is hosted on ReadTheDocs.
+
+## **Installation**
+
+`sigmaepsilon.core` can be installed (either in a virtual enviroment or globally) from PyPI using `pip` on Python >= 3.7:
+
+```console
+>>> pip install sigmaepsilon.core
+```
+
+or chechkout with the following command using GitHub CLI
+
+```console
+gh repo clone sigma-epsilon/sigmaepsilon.core
+```
+
+and install from source by typing
+
+```console
+>>> pip install .
+```
+
+If you want to run the tests, you can install the package along with the necessary optional dependencies like this
+
+```console
+>>> pip install ".[test]"
+```
+
+### For developers
+
+For development purposes, it is suggested to install the package in editable mode, with the optional dependencies for both testing, development and documentation
+
+```console
+>>> pip install -e ".[test, dev, docs]"
+```
+
+## Testing
+
+To run the tests, run the following command in the root of the project:
+
+```console
+>>> pytest
+```
+
+## **License**
+
+This package is licensed under the MIT license. See the attached LICENSE file for the details.
```

### Comparing `sigmaepsilon.core-0.0.1/docs/Makefile` & `sigmaepsilon.core-1.0.0/docs/Makefile`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Minimal makefile for Sphinx documentation
-#
-
-# You can set these variables from the command line, and also
-# from the environment for the first two.
-SPHINXOPTS    ?=
-SPHINXBUILD   ?= sphinx-build
-SOURCEDIR     = source
-BUILDDIR      = build
-
-# Put it first so that "make" without argument is like "make help".
-help:
-	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
-
-.PHONY: help Makefile
-
-# Catch-all target: route all unknown targets to Sphinx using the new
-# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
-%: Makefile
-	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+# Minimal makefile for Sphinx documentation
+#
+
+# You can set these variables from the command line, and also
+# from the environment for the first two.
+SPHINXOPTS    ?=
+SPHINXBUILD   ?= sphinx-build
+SOURCEDIR     = source
+BUILDDIR      = build
+
+# Put it first so that "make" without argument is like "make help".
+help:
+	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+
+.PHONY: help Makefile
+
+# Catch-all target: route all unknown targets to Sphinx using the new
+# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
+%: Makefile
+	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `sigmaepsilon.core-0.0.1/docs/source/conf.py` & `sigmaepsilon.core-1.0.0/docs/source/conf.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,125 +1,125 @@
-# Configuration file for the Sphinx documentation builder.
-#
-# For the full list of built-in configuration values, see the documentation:
-# https://www.sphinx-doc.org/en/master/usage/configuration.html
-
-# For ideas:
-
-# https://github.com/pradyunsg/furo/blob/main/docs/conf.py
-# https://github.com/sphinx-gallery/sphinx-gallery/blob/master/doc/conf.py
-
-# --------------------------------------------------------------------------
-
-import sys
-import os
-from datetime import date
-
-import sigmaepsilon.core as library
-
-from sphinx.config import Config
-
-# If extensions (or modules to document with autodoc) are in another directory,
-# add these directories to sys.path here. If the directory is relative to the
-# documentation root, use os.path.abspath to make it absolute, like shown here.
-sys.path.insert(0, os.path.abspath("."))
-sys.path.insert(0, os.path.abspath("../../src"))
-
-# -- Project information -----------------------------------------------------
-# https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
-
-project = library.__pkg_name__
-copyright = "2014-%s, Bence Balogh" % date.today().year
-author = "Bence Balogh"
-
-
-def setup(app: Config):
-    app.add_config_value("project_name", project, "html")
-
-
-# The short X.Y version.
-version = library.__version__
-# The full version, including alpha/beta/rc tags.
-release = "v" + library.__version__
-
-# -- General configuration ---------------------------------------------------
-# https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
-
-extensions = [
-    # allows to work with markdown files
-    "myst_parser",  # pip install myst-parser for this
-    # to plot summary about durations of file generations
-    "sphinx.ext.duration",
-    # to test code snippets in docstrings
-    "sphinx.ext.doctest",
-    # for automatic exploration of the source files
-    "sphinx.ext.autodoc",
-    # to enable cross referencing other documents on the internet
-    "sphinx.ext.intersphinx",
-    # Napoleon is a extension that enables Sphinx to parse both NumPy and Google style docstrings
-    "sphinx.ext.napoleon",
-    #'sphinx_gallery.gen_gallery',
-    #'sphinx_gallery.load_style',  # load CSS for gallery (needs SG >= 0.6)
-    #"nbsphinx",  # to handle jupyter notebooks
-    #"nbsphinx_link",  # for including notebook files from outside the sphinx source root
-    "sphinx_copybutton",  # for "copy to clipboard" buttons
-    "sphinx.ext.mathjax",  # for math equations
-    #"sphinxcontrib.bibtex",  # for bibliographic references
-    #"sphinxcontrib.rsvgconverter",  # for SVG->PDF conversion in LaTeX output
-    "sphinx.ext.viewcode",
-    "sphinx.ext.autosummary",
-    "sphinx.ext.doctest",
-    "sphinx.ext.todo",
-    "sphinx.ext.coverage",
-    "sphinx.ext.extlinks",
-    "sphinx.ext.mathjax",
-    "sphinx_design",
-    "sphinx_inline_tabs",
-]
-
-autosummary_generate = True
-
-templates_path = ["_templates"]
-
-exclude_patterns = ["_build"]
-
-source_suffix = {
-    ".rst": "restructuredtext",
-    ".txt": "markdown",
-    ".md": "markdown",
-}
-
-# The master toctree document.
-master_doc = "index"
-
-language = "EN"
-
-# See warnings about bad links
-nitpicky = True
-nitpick_ignore = [
-    ("", "Pygments lexer name 'ipython' is not known"),
-    ("", "Pygments lexer name 'ipython3' is not known"),
-]
-
-# The name of the Pygments (syntax highlighting) style to use.
-pygments_style = "sphinx"
-pygments_dark_style = "github-dark"
-highlight_language = "python3"
-
-intersphinx_mapping = {
-    "python": (r"https://docs.python.org/{.major}".format(sys.version_info), None),
-    "numpy": (r"https://numpy.org/doc/stable/", None),
-    "sphinx": (r"https://www.sphinx-doc.org/en/master", None),
-}
-
-# -- MathJax Configuration -------------------------------------------------
-
-mathjax3_config = {
-    "tex": {"tags": "ams", "useLabelIds": True},
-}
-
-# -- Options for HTML output -------------------------------------------------
-# https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
-
-html_theme = "pydata_sphinx_theme"
-
-html_static_path = ["_static"]
+# Configuration file for the Sphinx documentation builder.
+#
+# For the full list of built-in configuration values, see the documentation:
+# https://www.sphinx-doc.org/en/master/usage/configuration.html
+
+# For ideas:
+
+# https://github.com/pradyunsg/furo/blob/main/docs/conf.py
+# https://github.com/sphinx-gallery/sphinx-gallery/blob/master/doc/conf.py
+
+# --------------------------------------------------------------------------
+
+import sys
+import os
+from datetime import date
+
+import sigmaepsilon.core as library
+
+from sphinx.config import Config
+
+# If extensions (or modules to document with autodoc) are in another directory,
+# add these directories to sys.path here. If the directory is relative to the
+# documentation root, use os.path.abspath to make it absolute, like shown here.
+sys.path.insert(0, os.path.abspath("."))
+sys.path.insert(0, os.path.abspath("../../src"))
+
+# -- Project information -----------------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
+
+project = library.__pkg_name__
+copyright = "2014-%s, Bence Balogh" % date.today().year
+author = "Bence Balogh"
+
+
+def setup(app: Config):
+    app.add_config_value("project_name", project, "html")
+
+
+# The short X.Y version.
+version = library.__version__
+# The full version, including alpha/beta/rc tags.
+release = "v" + library.__version__
+
+# -- General configuration ---------------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
+
+extensions = [
+    # allows to work with markdown files
+    "myst_parser",  # pip install myst-parser for this
+    # to plot summary about durations of file generations
+    "sphinx.ext.duration",
+    # to test code snippets in docstrings
+    "sphinx.ext.doctest",
+    # for automatic exploration of the source files
+    "sphinx.ext.autodoc",
+    # to enable cross referencing other documents on the internet
+    "sphinx.ext.intersphinx",
+    # Napoleon is a extension that enables Sphinx to parse both NumPy and Google style docstrings
+    "sphinx.ext.napoleon",
+    #'sphinx_gallery.gen_gallery',
+    #'sphinx_gallery.load_style',  # load CSS for gallery (needs SG >= 0.6)
+    #"nbsphinx",  # to handle jupyter notebooks
+    #"nbsphinx_link",  # for including notebook files from outside the sphinx source root
+    "sphinx_copybutton",  # for "copy to clipboard" buttons
+    "sphinx.ext.mathjax",  # for math equations
+    #"sphinxcontrib.bibtex",  # for bibliographic references
+    #"sphinxcontrib.rsvgconverter",  # for SVG->PDF conversion in LaTeX output
+    "sphinx.ext.viewcode",
+    "sphinx.ext.autosummary",
+    "sphinx.ext.doctest",
+    "sphinx.ext.todo",
+    "sphinx.ext.coverage",
+    "sphinx.ext.extlinks",
+    "sphinx.ext.mathjax",
+    "sphinx_design",
+    "sphinx_inline_tabs",
+]
+
+autosummary_generate = True
+
+templates_path = ["_templates"]
+
+exclude_patterns = ["_build"]
+
+source_suffix = {
+    ".rst": "restructuredtext",
+    ".txt": "markdown",
+    ".md": "markdown",
+}
+
+# The master toctree document.
+master_doc = "index"
+
+language = "EN"
+
+# See warnings about bad links
+nitpicky = True
+nitpick_ignore = [
+    ("", "Pygments lexer name 'ipython' is not known"),
+    ("", "Pygments lexer name 'ipython3' is not known"),
+]
+
+# The name of the Pygments (syntax highlighting) style to use.
+pygments_style = "sphinx"
+pygments_dark_style = "github-dark"
+highlight_language = "python3"
+
+intersphinx_mapping = {
+    "python": (r"https://docs.python.org/{.major}".format(sys.version_info), None),
+    "numpy": (r"https://numpy.org/doc/stable/", None),
+    "sphinx": (r"https://www.sphinx-doc.org/en/master", None),
+}
+
+# -- MathJax Configuration -------------------------------------------------
+
+mathjax3_config = {
+    "tex": {"tags": "ams", "useLabelIds": True},
+}
+
+# -- Options for HTML output -------------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
+
+html_theme = "pydata_sphinx_theme"
+
+html_static_path = ["_static"]
```

### Comparing `sigmaepsilon.core-0.0.1/pyproject.toml` & `sigmaepsilon.core-1.0.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-[build-system]
-requires = [
-    "setuptools>=65.5.1",
-    "setuptools-scm",
-    "wheel>=0.38.0"
-]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "sigmaepsilon.core"
-version = "0.0.1"
-description = "Common developer utilities for Python projects."
-classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3 :: Only",
-        "Operating System :: OS Independent",
-]
-readme = {file = "README.md", content-type = "text/markdown"}
-authors = [
-    { name = "SigmaEpsilon", email = "bencebalogh@sigmaepsilon.com" }
-]
-maintainers = [
-    { name = "SigmaEpsilon", email = "bencebalogh@sigmaepsilon.com" }
-]
-license = { file = "LICENSE" }
-keywords = [
-    "engineering", "mechanics", "science", "numerical analysis", 
-    "finite element method", "solid mechanics", "optimization"
-]
-requires-python = ">=3.7, <3.11"
-dynamic = ["dependencies", "optional-dependencies"]
-
-[tool.setuptools.packages.find]
-where = ["src"]
-
-[tool.setuptools.dynamic]
-dependencies = { file = ["requirements.txt"] }
-optional-dependencies.test = { file = ["requirements-test.txt"] }
-optional-dependencies.dev = { file = ["requirements-dev.txt"] }
-optional-dependencies.docs = { file = ["docs/requirements.txt"] }
-
-[project.urls]
-Homepage = "https://github.com/sigma-epsilon/sigmaepsilon.core"
+[build-system]
+requires = [
+    "setuptools>=65.5.1",
+    "setuptools-scm",
+    "wheel>=0.38.0"
+]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "sigmaepsilon.core"
+version = "1.0.0"
+description = "Common developer utilities for Python projects."
+classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3 :: Only",
+        "Operating System :: OS Independent",
+]
+readme = {file = "README.md", content-type = "text/markdown"}
+authors = [
+    { name = "SigmaEpsilon", email = "bencebalogh@sigmaepsilon.com" }
+]
+maintainers = [
+    { name = "SigmaEpsilon", email = "bencebalogh@sigmaepsilon.com" }
+]
+license = { file = "LICENSE" }
+keywords = [
+    "engineering", "mechanics", "science", "numerical analysis", 
+    "finite element method", "solid mechanics", "optimization"
+]
+requires-python = ">=3.7, <3.11"
+dynamic = ["dependencies", "optional-dependencies"]
+
+[tool.setuptools.packages.find]
+where = ["src"]
+
+[tool.setuptools.dynamic]
+dependencies = { file = ["requirements.txt"] }
+optional-dependencies.test = { file = ["requirements-test.txt"] }
+optional-dependencies.dev = { file = ["requirements-dev.txt"] }
+optional-dependencies.docs = { file = ["docs/requirements.txt"] }
+
+[project.urls]
+Homepage = "https://github.com/sigma-epsilon/sigmaepsilon.core"
```

### Comparing `sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/abstract.py` & `sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/abstract.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,151 +1,151 @@
-# -*- coding: utf-8 -*-
-from .meta import *
-
-
-__all__ = ["ABC_Strong", "ABC_Weak", "ABC_Safe"]
-
-
-class ABC_Weak(metaclass=ABCMeta_Weak):
-    """
-    Helper class that provides a standard way to create an ABC using
-    inheritance. It follows weak abstraction in the meaning, that
-    it is enough to implement the abstarcts in the instance, they impose no
-    restriction on the inherited class itself. Therefore, error only occurs at
-    runtime.
-    
-    Notes
-    -----
-    This class provides nothing over the default behaviour offered by Python's
-    standard library, but it is equipped with some useful machinery for
-    subclasses that do. All other metaclasses of this module are subclasses of this
-    class.
-    
-    See also
-    --------
-    :class:`~sigmaepsilon.core.meta.ABCMeta_Weak`
-
-    Examples
-    --------
-    Create an abstract class with an abstract instance method.
-
-    >>> class ABC_Parent_Weak(ABC_Weak):
-    >>>     @abstractmethod
-    >>>     def abc_method_parent(self):
-    >>>         pass
-
-    Now if we subclass our parent class without implementing `abc_method_parent`,
-    nothing happens at runtime (when the class is created).
-
-    >>> class ABC_Child_Weak(ABC_Parent_Weak):
-    >>>     @abstractmethod
-    >>>     def abc_method_child(self):
-    >>>         pass
-
-    If we create an instance with implementing the abstract classes prescribed,
-    it works fine.
-
-    >>> class MyClass(ABC_Parent_Weak):
-    >>>     def abc_method_child(self):
-    >>>         pass
-    ...
-    >>>     def abc_method_parent(self):
-    >>>         pass
-    ...
-    >>> foo = MyClass()
-
-    If miss any of the required implementations, we can see a `TypeError`:
-
-    >>> class MyClass(ABC_Parent_Weak):
-    >>>     def abc_method_child(self):
-    >>>         pass
-    ...
-    >>> foo = MyClass()
-    Traceback (most recent call last):
-        ...
-    TypeError: Can't instantiate abstract class MyClass with abstract methods abc_method_parent
-    """
-    __slots__ = ()
-
-
-class ABC_Strong(metaclass=ABCMeta_Strong):
-    """
-    Helper class that provides a standard way to create an ABC using
-    inheritance. It follows strong abstraction in the meaning, that
-    an abstract function of any of the base classes must be implemented or
-    delayed with the use of another @abstractmethod decorator.
-    Contrary to the weak metaclass, error occurs when the class is created.
-    
-    See also
-    --------
-    :class:`~sigmaepsilon.core.meta.ABCMeta_Strong`
-
-    Examples
-    --------
-    Create an abstract class with abstract instance methods.
-
-    >>> class MyParentAbstractClass(ABC_Strong):
-    >>>     @abstractmethod
-    >>>     def my_abstract_method_A(self):
-    >>>         pass
-    ...
-    >>>     @abstractmethod
-    >>>     def my_abstract_method_B(self):
-    >>>         pass
-
-    Now if we subclass our parent class, we can either provide an implementation
-    of our abstract methods, or delay the implementation by using the `abstractmethod`
-    decorator again.
-
-    >>> class MyChildAbstractClass(MyParentAbstractClass):
-    >>>     @abstractmethod
-    >>>     def my_abstract_method_A(self):
-    >>>         # this is delayed
-    >>>         pass
-    ...
-    >>>     def my_abstract_method_B(self):
-    >>>         pass
-
-    In every other case, we will se an error when the class is created.
-
-    >>> class MyChildAbstractClass(MyParentAbstractClass):
-    >>>     @abstractmethod
-    >>>     def my_abstract_method_A(self):
-    >>>         pass
-    Traceback (most recent call last):
-        ...
-    TypeError: Can't create abstract class MyChildAbstractClas! MyChildAbstractClas must implement abstract method my_abstract_method_B of class MyParentAbstractClass.
-    """
-    __slots__ = ()
-
-
-class ABC_Safe(metaclass=ABCMeta_Safe):
-    """
-    Helper class that provides a standard way to create an ABC using
-    inheritance. Throws a `TypeError`
-    if a method tries to shadow a method in any of the base
-    classes.
-    
-    See also
-    --------
-    :class:`~sigmaepsilon.core.meta.ABCMeta_Safe`
-
-    Examples
-    --------
-    Create an abstract class with an instance method.
-
-    >>> class ABC_Parent_Safe(ABC_Safe):
-    >>>     def funcParentSafe(self):
-    >>>         pass
-
-    Now, if we try to overload any implementation in the parent class, we
-    got a `TypeError` when the class is created.
-
-    >>> class ABC_Child_Safe(ABC_Parent_Safe):
-    >>>     def funcParentSafe(self):
-    >>>         pass
-    Traceback (most recent call last):
-        ...
-    TypeError: Can't create abstract class ABC_Child_Safe! Method funcParentSafe is already implemented in class ABC_Parent_Safe.
-    """
-    __slots__ = ()
-
+# -*- coding: utf-8 -*-
+from .meta import *
+
+
+__all__ = ["ABC_Strong", "ABC_Weak", "ABC_Safe"]
+
+
+class ABC_Weak(metaclass=ABCMeta_Weak):
+    """
+    Helper class that provides a standard way to create an ABC using
+    inheritance. It follows weak abstraction in the meaning, that
+    it is enough to implement the abstarcts in the instance, they impose no
+    restriction on the inherited class itself. Therefore, error only occurs at
+    runtime.
+    
+    Notes
+    -----
+    This class provides nothing over the default behaviour offered by Python's
+    standard library, but it is equipped with some useful machinery for
+    subclasses that do. All other metaclasses of this module are subclasses of this
+    class.
+    
+    See also
+    --------
+    :class:`~sigmaepsilon.core.meta.ABCMeta_Weak`
+
+    Examples
+    --------
+    Create an abstract class with an abstract instance method.
+
+    >>> class ABC_Parent_Weak(ABC_Weak):
+    >>>     @abstractmethod
+    >>>     def abc_method_parent(self):
+    >>>         pass
+
+    Now if we subclass our parent class without implementing `abc_method_parent`,
+    nothing happens at runtime (when the class is created).
+
+    >>> class ABC_Child_Weak(ABC_Parent_Weak):
+    >>>     @abstractmethod
+    >>>     def abc_method_child(self):
+    >>>         pass
+
+    If we create an instance with implementing the abstract classes prescribed,
+    it works fine.
+
+    >>> class MyClass(ABC_Parent_Weak):
+    >>>     def abc_method_child(self):
+    >>>         pass
+    ...
+    >>>     def abc_method_parent(self):
+    >>>         pass
+    ...
+    >>> foo = MyClass()
+
+    If miss any of the required implementations, we can see a `TypeError`:
+
+    >>> class MyClass(ABC_Parent_Weak):
+    >>>     def abc_method_child(self):
+    >>>         pass
+    ...
+    >>> foo = MyClass()
+    Traceback (most recent call last):
+        ...
+    TypeError: Can't instantiate abstract class MyClass with abstract methods abc_method_parent
+    """
+    __slots__ = ()
+
+
+class ABC_Strong(metaclass=ABCMeta_Strong):
+    """
+    Helper class that provides a standard way to create an ABC using
+    inheritance. It follows strong abstraction in the meaning, that
+    an abstract function of any of the base classes must be implemented or
+    delayed with the use of another @abstractmethod decorator.
+    Contrary to the weak metaclass, error occurs when the class is created.
+    
+    See also
+    --------
+    :class:`~sigmaepsilon.core.meta.ABCMeta_Strong`
+
+    Examples
+    --------
+    Create an abstract class with abstract instance methods.
+
+    >>> class MyParentAbstractClass(ABC_Strong):
+    >>>     @abstractmethod
+    >>>     def my_abstract_method_A(self):
+    >>>         pass
+    ...
+    >>>     @abstractmethod
+    >>>     def my_abstract_method_B(self):
+    >>>         pass
+
+    Now if we subclass our parent class, we can either provide an implementation
+    of our abstract methods, or delay the implementation by using the `abstractmethod`
+    decorator again.
+
+    >>> class MyChildAbstractClass(MyParentAbstractClass):
+    >>>     @abstractmethod
+    >>>     def my_abstract_method_A(self):
+    >>>         # this is delayed
+    >>>         pass
+    ...
+    >>>     def my_abstract_method_B(self):
+    >>>         pass
+
+    In every other case, we will se an error when the class is created.
+
+    >>> class MyChildAbstractClass(MyParentAbstractClass):
+    >>>     @abstractmethod
+    >>>     def my_abstract_method_A(self):
+    >>>         pass
+    Traceback (most recent call last):
+        ...
+    TypeError: Can't create abstract class MyChildAbstractClas! MyChildAbstractClas must implement abstract method my_abstract_method_B of class MyParentAbstractClass.
+    """
+    __slots__ = ()
+
+
+class ABC_Safe(metaclass=ABCMeta_Safe):
+    """
+    Helper class that provides a standard way to create an ABC using
+    inheritance. Throws a `TypeError`
+    if a method tries to shadow a method in any of the base
+    classes.
+    
+    See also
+    --------
+    :class:`~sigmaepsilon.core.meta.ABCMeta_Safe`
+
+    Examples
+    --------
+    Create an abstract class with an instance method.
+
+    >>> class ABC_Parent_Safe(ABC_Safe):
+    >>>     def funcParentSafe(self):
+    >>>         pass
+
+    Now, if we try to overload any implementation in the parent class, we
+    got a `TypeError` when the class is created.
+
+    >>> class ABC_Child_Safe(ABC_Parent_Safe):
+    >>>     def funcParentSafe(self):
+    >>>         pass
+    Traceback (most recent call last):
+        ...
+    TypeError: Can't create abstract class ABC_Child_Safe! Method funcParentSafe is already implemented in class ABC_Parent_Safe.
+    """
+    __slots__ = ()
+
```

### Comparing `sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/acp.py` & `sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/acp.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,143 +1,143 @@
-# -*- coding: utf-8 -*-
-"""
-Multiple solutions on how to enforce an abstract class property
-on an object. Generic types like 'List[int]' are not allowed, 
-because the don't work well with the isinstance()-like methods.
-"""
-from typing import Callable
-
-__all__ = ['abstract_class_property', 'setproperty']
-
-
-def abstract_class_property(**kwargs) -> Callable:
-    return abstract_class_property_B(**kwargs)
-
-
-def setproperty(**kwargs):
-    def decorator(cls):
-        for key, value in kwargs.items():
-            setattr(cls, key, value)
-        return cls
-    return decorator
-
-
-"""
-Implementation A: class annotations solution using an object descriptor 
-and a wrapper class with classic pythonic manipulations.
-"""
-
-
-def abstract_class_property_A(**kwargs) -> Callable:
-    """
-    Decorator function to decorate objects with abstract
-    class properties. Leaves behind another decorator 
-    that takes a class as its input.
-    """
-
-    def abstractor(WrappedClass):
-
-        class PropertyWrapper(WrappedClass):
-            """
-            A Wrapper class to decorate objects with abstract class properties.
-            The class has a default dummy annotation, just so that we can append 
-            the items of the input dictionary d to the class definition.
-            The dummy property is deleted at the end.
-            """
-            _dummy_: None
-
-            def __init__(self, *args, **kwargs):
-                WrappedClass.__init__(self)
-                d_ = dict()
-                d_props = PropertyWrapper.__dict__.get('__annotations__', {})
-                for key, value in d_props.items():
-                    d_[key] = value
-                d_self = self.__class__.__dict__.get('__annotations__', {})
-                for key, value in d_self.items():
-                    d_[key] = value
-                for key in d_.keys():
-                    if not hasattr(self, key):
-                        raise AttributeError(f'required attribute {key} not present '
-                                             f'in {self.__class__}')
-                return
-
-        res = PropertyWrapper
-        d_ = res.__dict__['__annotations__']
-        for key, value in kwargs.items():
-            d_[key] = value
-        for key, value in WrappedClass.__dict__.get('__annotations__', {}).items():
-            d_[key] = value
-        del d_['_dummy_']
-        return res
-
-    return abstractor
-
-
-"""
-Implementation B: class annotations solution using an object descriptor and a 
-wrapper class using the __mro__ property of the class.
-This implementation also checks the validity of the declaration.
-"""
-
-
-def abstract_class_property_B(**kwargs) -> Callable:
-    """
-    Decorator function to decorate objects with abstract
-    class properties. Leaves behind another decorator
-    that takes a class as its input.
-    """
-
-    def abstractor(WrappedClass):
-
-        class PropertyWrapper(WrappedClass):
-            """
-            A Wrapper class to decorate objects with abstract class properties.
-            The class has a default dummy annotation, just so that we can append 
-            the items of the input dictionary d to the class definition.
-            The dummy property is deleted at the end.
-            """
-            _dummy_: None
-
-            def __init__(self, *args, **kwargs):
-                WrappedClass.__init__(self)
-                self.__check_absclsprops__()
-                return
-
-            @classmethod
-            def __absclsprops__(cls):
-                """
-                Collects the abstracts class properties and their
-                expected types based on the MRO of the class.
-                """
-                t = cls.__mro__
-                l = [ti.__dict__.get('__annotations__', {}) for ti in t]
-                res = dict()
-                for d in l:
-                    for key, value in d.items():
-                        res[key] = value
-                return res
-
-            def __check_absclsprops__(self):
-                """
-                Checks if the instance has attributes according to
-                the anstract annotations. Returns True if every attribute is
-                a type-correct declaration.
-                """
-                props = self.__class__.__absclsprops__()
-                for key, value in props.items():
-                    if not hasattr(self, key):
-                        raise AttributeError(f'required attribute {key} not present '
-                                             f'in {self.__class__}')
-                    else:
-                        if not isinstance(getattr(self, key), value):
-                            raise TypeError(
-                                'TypeError. key : {}, value = {}'.format(key, value))
-                return True
-
-        res = PropertyWrapper
-        d_ = res.__dict__['__annotations__']
-        for key, value in kwargs.items():
-            d_[key] = value
-        del d_['_dummy_']
-        return res
-
+# -*- coding: utf-8 -*-
+"""
+Multiple solutions on how to enforce an abstract class property
+on an object. Generic types like 'List[int]' are not allowed, 
+because the don't work well with the isinstance()-like methods.
+"""
+from typing import Callable
+
+__all__ = ['abstract_class_property', 'setproperty']
+
+
+def abstract_class_property(**kwargs) -> Callable:
+    return abstract_class_property_B(**kwargs)
+
+
+def setproperty(**kwargs):
+    def decorator(cls):
+        for key, value in kwargs.items():
+            setattr(cls, key, value)
+        return cls
+    return decorator
+
+
+"""
+Implementation A: class annotations solution using an object descriptor 
+and a wrapper class with classic pythonic manipulations.
+"""
+
+
+def abstract_class_property_A(**kwargs) -> Callable:
+    """
+    Decorator function to decorate objects with abstract
+    class properties. Leaves behind another decorator 
+    that takes a class as its input.
+    """
+
+    def abstractor(WrappedClass):
+
+        class PropertyWrapper(WrappedClass):
+            """
+            A Wrapper class to decorate objects with abstract class properties.
+            The class has a default dummy annotation, just so that we can append 
+            the items of the input dictionary d to the class definition.
+            The dummy property is deleted at the end.
+            """
+            _dummy_: None
+
+            def __init__(self, *args, **kwargs):
+                WrappedClass.__init__(self)
+                d_ = dict()
+                d_props = PropertyWrapper.__dict__.get('__annotations__', {})
+                for key, value in d_props.items():
+                    d_[key] = value
+                d_self = self.__class__.__dict__.get('__annotations__', {})
+                for key, value in d_self.items():
+                    d_[key] = value
+                for key in d_.keys():
+                    if not hasattr(self, key):
+                        raise AttributeError(f'required attribute {key} not present '
+                                             f'in {self.__class__}')
+                return
+
+        res = PropertyWrapper
+        d_ = res.__dict__['__annotations__']
+        for key, value in kwargs.items():
+            d_[key] = value
+        for key, value in WrappedClass.__dict__.get('__annotations__', {}).items():
+            d_[key] = value
+        del d_['_dummy_']
+        return res
+
+    return abstractor
+
+
+"""
+Implementation B: class annotations solution using an object descriptor and a 
+wrapper class using the __mro__ property of the class.
+This implementation also checks the validity of the declaration.
+"""
+
+
+def abstract_class_property_B(**kwargs) -> Callable:
+    """
+    Decorator function to decorate objects with abstract
+    class properties. Leaves behind another decorator
+    that takes a class as its input.
+    """
+
+    def abstractor(WrappedClass):
+
+        class PropertyWrapper(WrappedClass):
+            """
+            A Wrapper class to decorate objects with abstract class properties.
+            The class has a default dummy annotation, just so that we can append 
+            the items of the input dictionary d to the class definition.
+            The dummy property is deleted at the end.
+            """
+            _dummy_: None
+
+            def __init__(self, *args, **kwargs):
+                WrappedClass.__init__(self)
+                self.__check_absclsprops__()
+                return
+
+            @classmethod
+            def __absclsprops__(cls):
+                """
+                Collects the abstracts class properties and their
+                expected types based on the MRO of the class.
+                """
+                t = cls.__mro__
+                l = [ti.__dict__.get('__annotations__', {}) for ti in t]
+                res = dict()
+                for d in l:
+                    for key, value in d.items():
+                        res[key] = value
+                return res
+
+            def __check_absclsprops__(self):
+                """
+                Checks if the instance has attributes according to
+                the anstract annotations. Returns True if every attribute is
+                a type-correct declaration.
+                """
+                props = self.__class__.__absclsprops__()
+                for key, value in props.items():
+                    if not hasattr(self, key):
+                        raise AttributeError(f'required attribute {key} not present '
+                                             f'in {self.__class__}')
+                    else:
+                        if not isinstance(getattr(self, key), value):
+                            raise TypeError(
+                                'TypeError. key : {}, value = {}'.format(key, value))
+                return True
+
+        res = PropertyWrapper
+        d_ = res.__dict__['__annotations__']
+        for key, value in kwargs.items():
+            d_[key] = value
+        del d_['_dummy_']
+        return res
+
     return abstractor
```

### Comparing `sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/alphabet.py` & `sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/alphabet.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-# -*- coding: utf-8 -*-
-from typing import Union
-
-try:
-    from collections.abc import Iterable
-except ImportError:
-    from collections import Iterable
-
-__all__ = ["alphapet", "ordrange", "latinrange", "greekrange", "urange", "arabicrange"]
-
-
-def alphabet(abctype: str = "latin", start: Union[str, int] = None) -> Iterable:
-    """
-    Generator function that yields characters from different alphabets based on
-    the specified `abctype` and `start` parameters.
-
-    Parameters
-    ----------
-    abctype: str, Optional
-        The tipe of the alphabet. Accepted values are 'ord' or 'o' for ASCII ordinal values,
-        'latin' or 'l' for Latin, 'u' for Unicode and 'greek' or 'g' for Greek letters.
-        Default is 'latin'.
-    start: Union[str, int], Optional
-        The code of the character to start with. Default is `None`, in which case
-        a character is automatically selected as the first letter of the alphabet.
-
-    Yields
-    ------
-    string
-        A character from the specified alphabet.
-
-    Examples
-    --------
-    To generate 5 greek characters:
-    >>> from sigmaepsilon.core.alphabet import alphabet
-    >>> f = alphabet('greek')
-    >>> characters = list(map(alphabet('greek'), range(5)))
-    """
-    if abctype in ("ord", "o"):
-        start = 0 if start is None else start
-    elif abctype in ("latin", "l"):
-        start = ord("a") if start is None else start
-    elif abctype == "u":
-        start = ord("\u0000") if start is None else start
-    elif abctype in ("greek", "g"):
-        start = ord("\u03b1") if start is None else start
-    else:
-        raise ValueError("Invalid alphabet.")
-    start = ord(start) if isinstance(start, str) else start
-    while True:
-        yield chr(start)
-        start += 1
-
-
-def ordrange(N: int = 1, **kwargs) -> Iterable:
-    start = kwargs.pop("start", 0)
-    if isinstance(start, str):
-        start = ord(start)
-    stop = kwargs.pop("stop", None)
-    if stop is None or stop == start:
-        stop = start + N
-    return [chr(c) for c in range(start, stop)]
-
-
-def latinrange(N: int = 1, **kwargs) -> Iterable:
-    start = kwargs.pop("start", 97)
-    stop = kwargs.pop("stop", None)
-    return ordrange(N, start=start, stop=stop)
-
-
-def urange(N: int = 1, **kwargs) -> Iterable:
-    start = kwargs.pop("start", "\u0000")
-    stop = kwargs.pop("stop", None)
-    if stop is None:
-        stop = start
-    return ordrange(N, start=ord(start), stop=ord(stop))
-
-
-def greekrange(N: int = 1) -> Iterable:
-    return urange(N, start="\u03b1")
-
-
-def arabicrange(N: int = 1, **kwargs) -> Iterable:
-    start = kwargs.pop("start", 0)
-    stop = kwargs.pop("stop", None)
-    if stop is None or stop == start:
-        stop = start + N
-    return [str(c) for c in range(start, stop)]
+# -*- coding: utf-8 -*-
+from typing import Union
+
+try:
+    from collections.abc import Iterable
+except ImportError:
+    from collections import Iterable
+
+__all__ = ["alphapet", "ordrange", "latinrange", "greekrange", "urange", "arabicrange"]
+
+
+def alphabet(abctype: str = "latin", start: Union[str, int] = None) -> Iterable:
+    """
+    Generator function that yields characters from different alphabets based on
+    the specified `abctype` and `start` parameters.
+
+    Parameters
+    ----------
+    abctype: str, Optional
+        The tipe of the alphabet. Accepted values are 'ord' or 'o' for ASCII ordinal values,
+        'latin' or 'l' for Latin, 'u' for Unicode and 'greek' or 'g' for Greek letters.
+        Default is 'latin'.
+    start: Union[str, int], Optional
+        The code of the character to start with. Default is `None`, in which case
+        a character is automatically selected as the first letter of the alphabet.
+
+    Yields
+    ------
+    string
+        A character from the specified alphabet.
+
+    Examples
+    --------
+    To generate 5 greek characters:
+    >>> from sigmaepsilon.core.alphabet import alphabet
+    >>> f = alphabet('greek')
+    >>> characters = list(map(alphabet('greek'), range(5)))
+    """
+    if abctype in ("ord", "o"):
+        start = 0 if start is None else start
+    elif abctype in ("latin", "l"):
+        start = ord("a") if start is None else start
+    elif abctype == "u":
+        start = ord("\u0000") if start is None else start
+    elif abctype in ("greek", "g"):
+        start = ord("\u03b1") if start is None else start
+    else:
+        raise ValueError("Invalid alphabet.")
+    start = ord(start) if isinstance(start, str) else start
+    while True:
+        yield chr(start)
+        start += 1
+
+
+def ordrange(N: int = 1, **kwargs) -> Iterable:
+    start = kwargs.pop("start", 0)
+    if isinstance(start, str):
+        start = ord(start)
+    stop = kwargs.pop("stop", None)
+    if stop is None or stop == start:
+        stop = start + N
+    return [chr(c) for c in range(start, stop)]
+
+
+def latinrange(N: int = 1, **kwargs) -> Iterable:
+    start = kwargs.pop("start", 97)
+    stop = kwargs.pop("stop", None)
+    return ordrange(N, start=start, stop=stop)
+
+
+def urange(N: int = 1, **kwargs) -> Iterable:
+    start = kwargs.pop("start", "\u0000")
+    stop = kwargs.pop("stop", None)
+    if stop is None:
+        stop = start
+    return ordrange(N, start=ord(start), stop=ord(stop))
+
+
+def greekrange(N: int = 1) -> Iterable:
+    return urange(N, start="\u03b1")
+
+
+def arabicrange(N: int = 1, **kwargs) -> Iterable:
+    start = kwargs.pop("start", 0)
+    stop = kwargs.pop("stop", None)
+    if stop is None or stop == start:
+        stop = start + N
+    return [str(c) for c in range(start, stop)]
```

### Comparing `sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/attr.py` & `sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/attr.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-# -*- coding: utf-8 -*-
-from types import FunctionType
-from abc import abstractmethod
-
-
-def attributor(*attrs: str) -> FunctionType:
-    """
-    It renders a decorator a default behaviour. If a decorator
-    is called with a None argument, it returns the attribute, otherwise it 
-    returns the decorated function.
-    """
-    abstract = '__isabstractmethod__' in attrs
-    if abstract:
-        attributes = [x for x in attrs if x != '__isabstractmethod__']
-    else:
-        attributes = attrs
-
-    def decorator(fnc):
-        if fnc is None:
-            return attrs
-        else:
-            for attr in attributes:
-                setattr(fnc, attr, True)
-        if abstract:
-            return abstractmethod(fnc)
-        return fnc
-    return decorator
-
-
-if __name__ == '__main__':
-
-    axiom = attributor('__isaxiom__')
-    abstractaxiom = attributor('__isaxiom__', '__isabstractmethod__')
-
-    @axiom
-    def foo(a, b):
-        return 'an axiom'
-
+# -*- coding: utf-8 -*-
+from types import FunctionType
+from abc import abstractmethod
+
+
+def attributor(*attrs: str) -> FunctionType:
+    """
+    It renders a decorator a default behaviour. If a decorator
+    is called with a None argument, it returns the attribute, otherwise it 
+    returns the decorated function.
+    """
+    abstract = '__isabstractmethod__' in attrs
+    if abstract:
+        attributes = [x for x in attrs if x != '__isabstractmethod__']
+    else:
+        attributes = attrs
+
+    def decorator(fnc):
+        if fnc is None:
+            return attrs
+        else:
+            for attr in attributes:
+                setattr(fnc, attr, True)
+        if abstract:
+            return abstractmethod(fnc)
+        return fnc
+    return decorator
+
+
+if __name__ == '__main__':
+
+    axiom = attributor('__isaxiom__')
+    abstractaxiom = attributor('__isaxiom__', '__isabstractmethod__')
+
+    @axiom
+    def foo(a, b):
+        return 'an axiom'
+
     print(foo.__isaxiom__)
```

### Comparing `sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/cp.py` & `sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/cp.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,172 +1,172 @@
-"""
-Class property borrowed from the astropy package.
-"""
-import functools
-import threading
-
-_NotFound = object()
-
-__all__ = ["classproperty"]
-
-# TODO: This can still be made to work for setters by implementing an
-# accompanying metaclass that supports it; we just don't need that right
-# this moment
-class classproperty(property):
-    """
-    Similar to `property`, but allows class-level properties.  That is,
-    a property whose getter is like a `classmethod`.
-    The wrapped method may explicitly use the `classmethod` decorator (which
-    must become before this decorator), or the `classmethod` may be omitted
-    (it is implicit through use of this decorator).
-    
-    .. note::
-        classproperty only works for *read-only* properties.  It does not
-        currently allow writeable/deletable properties, due to subtleties of how
-        Python descriptors work.  In order to implement such properties on a class,
-        a metaclass for that class must be implemented.
-        
-    Parameters
-    ----------
-    fget: callable
-        The function that computes the value of this property (in particular,
-        the function when this is used as a decorator) a la `property`.
-    doc: str, optional
-        The docstring for the property--by default inherited from the getter
-        function.
-    lazy: bool, optional
-        If True, caches the value returned by the first call to the getter
-        function, so that it is only called once (used for lazy evaluation
-        of an attribute).  This is analogous to `lazyproperty`.  The ``lazy``
-        argument can also be used when `classproperty` is used as a decorator
-        (see the third example below).  When used in the decorator syntax this
-        *must* be passed in as a keyword argument.
-        
-    Examples
-    --------
-    ::
-        >>> class Foo:
-        ...     _bar_internal = 1
-        ...     @classproperty
-        ...     def bar(cls):
-        ...         return cls._bar_internal + 1
-        ...
-        >>> Foo.bar
-        2
-        >>> foo_instance = Foo()
-        >>> foo_instance.bar
-        2
-        >>> foo_instance._bar_internal = 2
-        >>> foo_instance.bar  # Ignores instance attributes
-        2
-    As previously noted, a `classproperty` is limited to implementing
-    read-only attributes::
-        >>> class Foo:
-        ...     _bar_internal = 1
-        ...     @classproperty
-        ...     def bar(cls):
-        ...         return cls._bar_internal
-        ...     @bar.setter
-        ...     def bar(cls, value):
-        ...         cls._bar_internal = value
-        ...
-        Traceback (most recent call last):
-        ...
-        NotImplementedError: classproperty can only be read-only; use a
-        metaclass to implement modifiable class-level properties
-    When the ``lazy`` option is used, the getter is only called once::
-        >>> class Foo:
-        ...     @classproperty(lazy=True)
-        ...     def bar(cls):
-        ...         print("Performing complicated calculation")
-        ...         return 1
-        ...
-        >>> Foo.bar
-        Performing complicated calculation
-        1
-        >>> Foo.bar
-        1
-    If a subclass inherits a lazy `classproperty` the property is still
-    re-evaluated for the subclass::
-        >>> class FooSub(Foo):
-        ...     pass
-        ...
-        >>> FooSub.bar
-        Performing complicated calculation
-        1
-        >>> FooSub.bar
-        1
-    """
-
-    def __new__(cls, fget=None, doc=None, lazy=False):
-        if fget is None:
-            # Being used as a decorator--return a wrapper that implements
-            # decorator syntax
-            def wrapper(func):
-                return cls(func, lazy=lazy)
-
-            return wrapper
-
-        return super().__new__(cls)
-
-    def __init__(self, fget, doc=None, lazy=False):
-        self._lazy = lazy
-        if lazy:
-            self._lock = threading.RLock()  # Protects _cache
-            self._cache = {}
-        fget = self._wrap_fget(fget)
-
-        super().__init__(fget=fget, doc=doc)
-
-        # There is a buglet in Python where self.__doc__ doesn't
-        # get set properly on instances of property subclasses if
-        # the doc argument was used rather than taking the docstring
-        # from fget
-        # Related Python issue: https://bugs.python.org/issue24766
-        if doc is not None:
-            self.__doc__ = doc
-
-    def __get__(self, obj, objtype):
-        if self._lazy:
-            val = self._cache.get(objtype, _NotFound)
-            if val is _NotFound:
-                with self._lock:
-                    # Check if another thread initialised before we locked.
-                    val = self._cache.get(objtype, _NotFound)
-                    if val is _NotFound:
-                        val = self.fget.__wrapped__(objtype)
-                        self._cache[objtype] = val
-        else:
-            # The base property.__get__ will just return self here;
-            # instead we pass objtype through to the original wrapped
-            # function (which takes the class as its sole argument)
-            val = self.fget.__wrapped__(objtype)
-        return val
-
-    def getter(self, fget):
-        return super().getter(self._wrap_fget(fget))
-
-    def setter(self, fset):
-        raise NotImplementedError(
-            "classproperty can only be read-only; use a metaclass to "
-            "implement modifiable class-level properties"
-        )
-
-    def deleter(self, fdel):
-        raise NotImplementedError(
-            "classproperty can only be read-only; use a metaclass to "
-            "implement modifiable class-level properties"
-        )
-
-    @staticmethod
-    def _wrap_fget(orig_fget):
-        if isinstance(orig_fget, classmethod):
-            orig_fget = orig_fget.__func__
-
-        # Using stock functools.wraps instead of the fancier version
-        # found later in this module, which is overkill for this purpose
-
-        @functools.wraps(orig_fget)
-        def fget(obj):
-            return orig_fget(obj.__class__)
-
-        return fget
+"""
+Class property borrowed from the astropy package.
+"""
+import functools
+import threading
+
+_NotFound = object()
+
+__all__ = ["classproperty"]
+
+# TODO: This can still be made to work for setters by implementing an
+# accompanying metaclass that supports it; we just don't need that right
+# this moment
+class classproperty(property):
+    """
+    Similar to `property`, but allows class-level properties.  That is,
+    a property whose getter is like a `classmethod`.
+    The wrapped method may explicitly use the `classmethod` decorator (which
+    must become before this decorator), or the `classmethod` may be omitted
+    (it is implicit through use of this decorator).
+    
+    .. note::
+        classproperty only works for *read-only* properties.  It does not
+        currently allow writeable/deletable properties, due to subtleties of how
+        Python descriptors work.  In order to implement such properties on a class,
+        a metaclass for that class must be implemented.
+        
+    Parameters
+    ----------
+    fget: callable
+        The function that computes the value of this property (in particular,
+        the function when this is used as a decorator) a la `property`.
+    doc: str, optional
+        The docstring for the property--by default inherited from the getter
+        function.
+    lazy: bool, optional
+        If True, caches the value returned by the first call to the getter
+        function, so that it is only called once (used for lazy evaluation
+        of an attribute).  This is analogous to `lazyproperty`.  The ``lazy``
+        argument can also be used when `classproperty` is used as a decorator
+        (see the third example below).  When used in the decorator syntax this
+        *must* be passed in as a keyword argument.
+        
+    Examples
+    --------
+    ::
+        >>> class Foo:
+        ...     _bar_internal = 1
+        ...     @classproperty
+        ...     def bar(cls):
+        ...         return cls._bar_internal + 1
+        ...
+        >>> Foo.bar
+        2
+        >>> foo_instance = Foo()
+        >>> foo_instance.bar
+        2
+        >>> foo_instance._bar_internal = 2
+        >>> foo_instance.bar  # Ignores instance attributes
+        2
+    As previously noted, a `classproperty` is limited to implementing
+    read-only attributes::
+        >>> class Foo:
+        ...     _bar_internal = 1
+        ...     @classproperty
+        ...     def bar(cls):
+        ...         return cls._bar_internal
+        ...     @bar.setter
+        ...     def bar(cls, value):
+        ...         cls._bar_internal = value
+        ...
+        Traceback (most recent call last):
+        ...
+        NotImplementedError: classproperty can only be read-only; use a
+        metaclass to implement modifiable class-level properties
+    When the ``lazy`` option is used, the getter is only called once::
+        >>> class Foo:
+        ...     @classproperty(lazy=True)
+        ...     def bar(cls):
+        ...         print("Performing complicated calculation")
+        ...         return 1
+        ...
+        >>> Foo.bar
+        Performing complicated calculation
+        1
+        >>> Foo.bar
+        1
+    If a subclass inherits a lazy `classproperty` the property is still
+    re-evaluated for the subclass::
+        >>> class FooSub(Foo):
+        ...     pass
+        ...
+        >>> FooSub.bar
+        Performing complicated calculation
+        1
+        >>> FooSub.bar
+        1
+    """
+
+    def __new__(cls, fget=None, doc=None, lazy=False):
+        if fget is None:
+            # Being used as a decorator--return a wrapper that implements
+            # decorator syntax
+            def wrapper(func):
+                return cls(func, lazy=lazy)
+
+            return wrapper
+
+        return super().__new__(cls)
+
+    def __init__(self, fget, doc=None, lazy=False):
+        self._lazy = lazy
+        if lazy:
+            self._lock = threading.RLock()  # Protects _cache
+            self._cache = {}
+        fget = self._wrap_fget(fget)
+
+        super().__init__(fget=fget, doc=doc)
+
+        # There is a buglet in Python where self.__doc__ doesn't
+        # get set properly on instances of property subclasses if
+        # the doc argument was used rather than taking the docstring
+        # from fget
+        # Related Python issue: https://bugs.python.org/issue24766
+        if doc is not None:
+            self.__doc__ = doc
+
+    def __get__(self, obj, objtype):
+        if self._lazy:
+            val = self._cache.get(objtype, _NotFound)
+            if val is _NotFound:
+                with self._lock:
+                    # Check if another thread initialised before we locked.
+                    val = self._cache.get(objtype, _NotFound)
+                    if val is _NotFound:
+                        val = self.fget.__wrapped__(objtype)
+                        self._cache[objtype] = val
+        else:
+            # The base property.__get__ will just return self here;
+            # instead we pass objtype through to the original wrapped
+            # function (which takes the class as its sole argument)
+            val = self.fget.__wrapped__(objtype)
+        return val
+
+    def getter(self, fget):
+        return super().getter(self._wrap_fget(fget))
+
+    def setter(self, fset):
+        raise NotImplementedError(
+            "classproperty can only be read-only; use a metaclass to "
+            "implement modifiable class-level properties"
+        )
+
+    def deleter(self, fdel):
+        raise NotImplementedError(
+            "classproperty can only be read-only; use a metaclass to "
+            "implement modifiable class-level properties"
+        )
+
+    @staticmethod
+    def _wrap_fget(orig_fget):
+        if isinstance(orig_fget, classmethod):
+            orig_fget = orig_fget.__func__
+
+        # Using stock functools.wraps instead of the fancier version
+        # found later in this module, which is overkill for this purpose
+
+        @functools.wraps(orig_fget)
+        def fget(obj):
+            return orig_fget(obj.__class__)
+
+        return fget
```

### Comparing `sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/downloads.py` & `sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/downloads.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,175 +1,175 @@
-"""
-Downloadable datasets collected from various sources.
-
-Once downloaded, these datasets are stored locally allowing for the
-rapid reuse of these datasets.
-
-Examples
---------
->>> from sigmaepsilon.core.downloads import download_stand
->>> download_stand()
-...
-"""
-
-from functools import partial
-import os
-import shutil
-from urllib.request import urlretrieve
-import zipfile
-from typing import Optional
-from types import ModuleType
-
-from .thirdparty import import_package
-from . import EXAMPLES_PATH, SIGMAEPSILON_DATA_PATH as DATA_PATH
-
-pyvista: Optional[ModuleType] = import_package("pyvista")
-
-
-__all__ = ["download_file", "delete_downloads"]
-
-
-def _check_examples_path():
-    """Check if the examples path exists."""
-    if not EXAMPLES_PATH:
-        raise FileNotFoundError(
-            "EXAMPLES_PATH does not exist. Try setting the "
-            "environment variable `SIGMAEPSILON_USERDATA_PATH` "
-            "to a writable path and restarting Python"
-        )
-
-
-def _decompress(filename):
-    _check_examples_path()
-    zip_ref = zipfile.ZipFile(filename, "r")
-    zip_ref.extractall(EXAMPLES_PATH)
-    return zip_ref.close()
-
-
-def _get_vtk_file_url(filename):
-    return f"https://github.com/sigma-epsilon/sigmaepsilon.data/raw/main/{filename}"
-
-
-def _http_request(url):
-    return urlretrieve(url)
-
-
-def _repo_file_request(repo_path, filename):
-    return os.path.join(repo_path, "Data", filename), None
-
-
-def _retrieve_file(retriever, filename):
-    """
-    Retrieve file and cache it in sigmaepsilon.core.EXAMPLES_PATH.
-
-    Parameters
-    ----------
-    retriever: str or callable
-        If str, it is treated as a url.
-        If callable, the function must take no arguments and must
-        return a tuple like (file_path, resp), where file_path is
-        the path to the file to use.
-    filename: str
-        The name of the file.
-
-    Notes
-    -----
-    You must have `PyVista` installed to handle zip files.
-    """
-    _check_examples_path()
-    # First check if file has already been downloaded
-    local_path = os.path.join(EXAMPLES_PATH, os.path.basename(filename))
-    local_path_no_zip = local_path.replace(".zip", "")
-    if os.path.isfile(local_path_no_zip) or os.path.isdir(local_path_no_zip):
-        return local_path_no_zip, None
-    if isinstance(retriever, str):
-        retriever = partial(_http_request, retriever)
-    saved_file, resp = retriever()
-    # new_name = saved_file.replace(os.path.basename(saved_file), os.path.basename(filename))
-    # Make sure folder exists!
-    if not os.path.isdir(os.path.dirname((local_path))):
-        os.makedirs(os.path.dirname((local_path)))
-    if DATA_PATH is None:
-        shutil.move(saved_file, local_path)
-    else:
-        if os.path.isdir(saved_file):
-            shutil.copytree(saved_file, local_path)
-        else:
-            shutil.copy(saved_file, local_path)
-    if pyvista:
-        if pyvista.get_ext(local_path) in [".zip"]:
-            _decompress(local_path)
-            local_path = local_path[:-4]
-    return local_path, resp
-
-
-def _download_file(filename):
-    if DATA_PATH is None:
-        url = _get_vtk_file_url(filename)
-        retriever = partial(_http_request, url)
-    else:
-        if not os.path.isdir(DATA_PATH):
-            raise FileNotFoundError(
-                f"Data repository path does not exist at:\n\n{DATA_PATH}"
-            )
-        if not os.path.isdir(os.path.join(DATA_PATH, "Data")):
-            raise FileNotFoundError(
-                f'Data repository does not have "Data" folder at:\n\n{DATA_PATH}'
-            )
-        retriever = partial(_repo_file_request, DATA_PATH, filename)
-    return _retrieve_file(retriever, filename)
-
-
-def _download_and_read(filename):
-    saved_file, _ = _download_file(filename)
-    return saved_file
-
-
-def download_file(filename: str) -> str:
-    """
-    Downloads a data file and returns the path of it on
-    your local filesystem.
-
-    Parameters
-    ----------
-    filename: str
-        The name of the file to download with extension included.
-
-    Returns
-    -------
-    str
-        A path to a file on your filesystem.
-
-    See also
-    --------
-    :func:`~sigmaepsilon.core.downloads.delete_downloads`
-
-    Example
-    --------
-    >>> from sigmaepsilon.core.downloads import download_file
-    >>> download_file("stand.vtk")
-    """
-    return _download_and_read(filename)
-
-
-def delete_downloads() -> bool:
-    """
-    Delete all downloaded examples to free space or update the files.
-    Returns `True` if the operation was succesful, or `False` if it wasn't.
-
-    See also
-    --------
-    :func:`~sigmaepsilon.core.downloads.download_file`
-
-    Examples
-    --------
-    Delete all local downloads.
-
-    >>> from sigmaepsilon.core import delete_downloads
-    >>> delete_downloads()  # doctest:+SKIP
-    True
-    """
-    _check_examples_path()
-    shutil.rmtree(EXAMPLES_PATH)
-    os.makedirs(EXAMPLES_PATH)
-    return True
-
+"""
+Downloadable datasets collected from various sources.
+
+Once downloaded, these datasets are stored locally allowing for the
+rapid reuse of these datasets.
+
+Examples
+--------
+>>> from sigmaepsilon.core.downloads import download_stand
+>>> download_stand()
+...
+"""
+
+from functools import partial
+import os
+import shutil
+from urllib.request import urlretrieve
+import zipfile
+from typing import Optional
+from types import ModuleType
+
+from .thirdparty import import_package
+from . import EXAMPLES_PATH, SIGMAEPSILON_DATA_PATH as DATA_PATH
+
+pyvista: Optional[ModuleType] = import_package("pyvista")
+
+
+__all__ = ["download_file", "delete_downloads"]
+
+
+def _check_examples_path():
+    """Check if the examples path exists."""
+    if not EXAMPLES_PATH:
+        raise FileNotFoundError(
+            "EXAMPLES_PATH does not exist. Try setting the "
+            "environment variable `SIGMAEPSILON_USERDATA_PATH` "
+            "to a writable path and restarting Python"
+        )
+
+
+def _decompress(filename):
+    _check_examples_path()
+    zip_ref = zipfile.ZipFile(filename, "r")
+    zip_ref.extractall(EXAMPLES_PATH)
+    return zip_ref.close()
+
+
+def _get_vtk_file_url(filename):
+    return f"https://github.com/sigma-epsilon/sigmaepsilon.data/raw/main/{filename}"
+
+
+def _http_request(url):
+    return urlretrieve(url)
+
+
+def _repo_file_request(repo_path, filename):
+    return os.path.join(repo_path, "Data", filename), None
+
+
+def _retrieve_file(retriever, filename):
+    """
+    Retrieve file and cache it in sigmaepsilon.core.EXAMPLES_PATH.
+
+    Parameters
+    ----------
+    retriever: str or callable
+        If str, it is treated as a url.
+        If callable, the function must take no arguments and must
+        return a tuple like (file_path, resp), where file_path is
+        the path to the file to use.
+    filename: str
+        The name of the file.
+
+    Notes
+    -----
+    You must have `PyVista` installed to handle zip files.
+    """
+    _check_examples_path()
+    # First check if file has already been downloaded
+    local_path = os.path.join(EXAMPLES_PATH, os.path.basename(filename))
+    local_path_no_zip = local_path.replace(".zip", "")
+    if os.path.isfile(local_path_no_zip) or os.path.isdir(local_path_no_zip):
+        return local_path_no_zip, None
+    if isinstance(retriever, str):
+        retriever = partial(_http_request, retriever)
+    saved_file, resp = retriever()
+    # new_name = saved_file.replace(os.path.basename(saved_file), os.path.basename(filename))
+    # Make sure folder exists!
+    if not os.path.isdir(os.path.dirname((local_path))):
+        os.makedirs(os.path.dirname((local_path)))
+    if DATA_PATH is None:
+        shutil.move(saved_file, local_path)
+    else:
+        if os.path.isdir(saved_file):
+            shutil.copytree(saved_file, local_path)
+        else:
+            shutil.copy(saved_file, local_path)
+    if pyvista:
+        if pyvista.get_ext(local_path) in [".zip"]:
+            _decompress(local_path)
+            local_path = local_path[:-4]
+    return local_path, resp
+
+
+def _download_file(filename):
+    if DATA_PATH is None:
+        url = _get_vtk_file_url(filename)
+        retriever = partial(_http_request, url)
+    else:
+        if not os.path.isdir(DATA_PATH):
+            raise FileNotFoundError(
+                f"Data repository path does not exist at:\n\n{DATA_PATH}"
+            )
+        if not os.path.isdir(os.path.join(DATA_PATH, "Data")):
+            raise FileNotFoundError(
+                f'Data repository does not have "Data" folder at:\n\n{DATA_PATH}'
+            )
+        retriever = partial(_repo_file_request, DATA_PATH, filename)
+    return _retrieve_file(retriever, filename)
+
+
+def _download_and_read(filename):
+    saved_file, _ = _download_file(filename)
+    return saved_file
+
+
+def download_file(filename: str) -> str:
+    """
+    Downloads a data file and returns the path of it on
+    your local filesystem.
+
+    Parameters
+    ----------
+    filename: str
+        The name of the file to download with extension included.
+
+    Returns
+    -------
+    str
+        A path to a file on your filesystem.
+
+    See also
+    --------
+    :func:`~sigmaepsilon.core.downloads.delete_downloads`
+
+    Example
+    --------
+    >>> from sigmaepsilon.core.downloads import download_file
+    >>> download_file("stand.vtk")
+    """
+    return _download_and_read(filename)
+
+
+def delete_downloads() -> bool:
+    """
+    Delete all downloaded examples to free space or update the files.
+    Returns `True` if the operation was succesful, or `False` if it wasn't.
+
+    See also
+    --------
+    :func:`~sigmaepsilon.core.downloads.download_file`
+
+    Examples
+    --------
+    Delete all local downloads.
+
+    >>> from sigmaepsilon.core import delete_downloads
+    >>> delete_downloads()  # doctest:+SKIP
+    True
+    """
+    _check_examples_path()
+    shutil.rmtree(EXAMPLES_PATH)
+    os.makedirs(EXAMPLES_PATH)
+    return True
+
```

### Comparing `sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/formatting.py` & `sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/formatting.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-# -*- coding: utf-8 -*-
-from typing import Optional, Union, Iterable
-from types import ModuleType
-from .typing import issequence
-from .thirdparty import import_package
-
-__all__ = ["float_to_str_sig", "floatformatter"]
-
-
-def floatformatter(*, sig: Optional[int] = 6) -> str:
-    """
-    Returns a formatter, which essantially a string temapate
-    ready to be formatted.
-
-    Parameters
-    ----------
-    sig: int, Optional
-        Number of significant digits. Default is 6.
-
-    Returns
-    -------
-    string
-        The string to be formatted.
-        
-    See also
-    --------
-    :func:`~sigmaepsilon.core.formatting.float_to_str_sig`
-        
-    Example
-    --------
-    Print the value of pi as a string with 4 significant digits:
-
-    >>> from sigmaepsilon.core.formatting import floatformatter
-    >>> import math
-    >>> formatter = floatformatter(sig=4)
-    >>> formatter.format(math.pi)
-    '3.142'
-    """
-    return "{" + "0:.{}g".format(sig) + "}"
-
-
-def float_to_str_sig(
-    value: Union[float, Iterable[float]],
-    *,
-    sig: Optional[int] = 6,
-    atol: Optional[float] = 1e-7
-) -> Union[str, Iterable[str]]:
-    """
-    Returns a string representation of a floating point number, with
-    given significant digits.
-
-    Parameters
-    ----------
-    value: Union[float, Iterable[float]]
-        A single value, or an iterable.
-
-    sig: int, Optional
-        Number of significant digits. Default is 6.
-
-    atol: float, Optional
-        Floating point tolerance. Values smaller than this
-        in the absolute sense are treated as zero. Default is 1e-7.
-
-    Returns
-    -------
-    Union[str, Iterable[str]]
-        String representation of the provided input.
-        
-    See also
-    --------
-    :func:`~sigmaepsilon.core.formatting.floatformatter`
-
-    Example
-    --------
-    Print the value of pi as a string with 4 significant digits:
-
-    >>> from sigmaepsilon.core.formatting import float_to_str_sig
-    >>> import math
-    >>> float_to_str_sig(math.pi, sig=4)
-    '3.142'
-    """
-    if not issequence(value):
-        if atol is not None:
-            if abs(value) < atol:
-                value = 0.0
-        return floatformatter(sig=sig).format(value)
-    else:
-        np: Optional[ModuleType] = import_package("numpy")
-        if not np:
-            raise ImportError("You need numpy for this.")
-        value = np.array(value)
-        if atol is not None:
-            inds = np.where(np.abs(value) < atol)[0]
-            value[inds] = 0.0
-        formatter = floatformatter(sig=sig)
-
-        def f(v):
-            return formatter.format(v)
-
-        return list(map(f, value))
+# -*- coding: utf-8 -*-
+from typing import Optional, Union, Iterable
+from types import ModuleType
+from .typing import issequence
+from .thirdparty import import_package
+
+__all__ = ["float_to_str_sig", "floatformatter"]
+
+
+def floatformatter(*, sig: Optional[int] = 6) -> str:
+    """
+    Returns a formatter, which essantially a string temapate
+    ready to be formatted.
+
+    Parameters
+    ----------
+    sig: int, Optional
+        Number of significant digits. Default is 6.
+
+    Returns
+    -------
+    string
+        The string to be formatted.
+        
+    See also
+    --------
+    :func:`~sigmaepsilon.core.formatting.float_to_str_sig`
+        
+    Example
+    --------
+    Print the value of pi as a string with 4 significant digits:
+
+    >>> from sigmaepsilon.core.formatting import floatformatter
+    >>> import math
+    >>> formatter = floatformatter(sig=4)
+    >>> formatter.format(math.pi)
+    '3.142'
+    """
+    return "{" + "0:.{}g".format(sig) + "}"
+
+
+def float_to_str_sig(
+    value: Union[float, Iterable[float]],
+    *,
+    sig: Optional[int] = 6,
+    atol: Optional[float] = 1e-7
+) -> Union[str, Iterable[str]]:
+    """
+    Returns a string representation of a floating point number, with
+    given significant digits.
+
+    Parameters
+    ----------
+    value: Union[float, Iterable[float]]
+        A single value, or an iterable.
+
+    sig: int, Optional
+        Number of significant digits. Default is 6.
+
+    atol: float, Optional
+        Floating point tolerance. Values smaller than this
+        in the absolute sense are treated as zero. Default is 1e-7.
+
+    Returns
+    -------
+    Union[str, Iterable[str]]
+        String representation of the provided input.
+        
+    See also
+    --------
+    :func:`~sigmaepsilon.core.formatting.floatformatter`
+
+    Example
+    --------
+    Print the value of pi as a string with 4 significant digits:
+
+    >>> from sigmaepsilon.core.formatting import float_to_str_sig
+    >>> import math
+    >>> float_to_str_sig(math.pi, sig=4)
+    '3.142'
+    """
+    if not issequence(value):
+        if atol is not None:
+            if abs(value) < atol:
+                value = 0.0
+        return floatformatter(sig=sig).format(value)
+    else:
+        np: Optional[ModuleType] = import_package("numpy")
+        if not np:
+            raise ImportError("You need numpy for this.")
+        value = np.array(value)
+        if atol is not None:
+            inds = np.where(np.abs(value) < atol)[0]
+            value[inds] = 0.0
+        formatter = floatformatter(sig=sig)
+
+        def f(v):
+            return formatter.format(v)
+
+        return list(map(f, value))
```

### Comparing `sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/infix.py` & `sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/infix.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-# -*- coding: utf-8 -*-
-from typing import Callable, Any
-
-__all__ = ["InfixOperator"]
-
-
-class InfixOperator:
-    """
-    Implements a custom Infix operator using  the 
-    operators '<<', '>>' and '|'.
-
-    Examples
-    --------
-    >>> x = InfixOperator(lambda x, y: x * y)
-    >>> print(2 | x | 4)
-    8
-
-    >>> x = InfixOperator(lambda x, y: x + y)
-    >>> print(2 << x >> 4)
-    6
-    """
-
-    def __init__(self, function: Callable):
-        self._function = function
-
-    def __ror__(self, other: Any) -> "InfixOperator":
-        return InfixOperator(lambda x, self=self, other=other: self._function(other, x))
-
-    def __or__(self, other: Any) -> Any:
-        return self._function(other)
-
-    def __rlshift__(self, other: Any) -> "InfixOperator":
-        return InfixOperator(lambda x, self=self, other=other: self._function(other, x))
-
-    def __rshift__(self, other: Any) -> Any:
-        return self._function(other)
-
-    def __call__(self, value1: Any, value2: Any) -> Any:
+# -*- coding: utf-8 -*-
+from typing import Callable, Any
+
+__all__ = ["InfixOperator"]
+
+
+class InfixOperator:
+    """
+    Implements a custom Infix operator using  the 
+    operators '<<', '>>' and '|'.
+
+    Examples
+    --------
+    >>> x = InfixOperator(lambda x, y: x * y)
+    >>> print(2 | x | 4)
+    8
+
+    >>> x = InfixOperator(lambda x, y: x + y)
+    >>> print(2 << x >> 4)
+    6
+    """
+
+    def __init__(self, function: Callable):
+        self._function = function
+
+    def __ror__(self, other: Any) -> "InfixOperator":
+        return InfixOperator(lambda x, self=self, other=other: self._function(other, x))
+
+    def __or__(self, other: Any) -> Any:
+        return self._function(other)
+
+    def __rlshift__(self, other: Any) -> "InfixOperator":
+        return InfixOperator(lambda x, self=self, other=other: self._function(other, x))
+
+    def __rshift__(self, other: Any) -> Any:
+        return self._function(other)
+
+    def __call__(self, value1: Any, value2: Any) -> Any:
         return self._function(value1, value2)
```

### Comparing `sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/kwargtools.py` & `sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/kwargtools.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-# -*- coding: utf-8 -*-
-from typing import Callable
-
-try:
-    from collections.abc import Iterable
-except ImportError:
-    from collections import Iterable
-
-
-__all__ = [
-    "isinkwargs",
-    "allinkwargs",
-    "anyinkwargs",
-    "getfromkwargs",
-    "popfromkwargs",
-    "getallfromkwargs",
-    "getasany",
-    "countkwargs"
-]
-
-
-def isinkwargs(keys, **kwargs):
-    if isinstance(keys, Iterable) and not isinstance(keys, str):
-        return [key in kwargs for key in keys]
-    else:
-        return keys in kwargs
-
-
-def allinkwargs(keys, **kwargs):
-    if isinstance(keys, Iterable) and not isinstance(keys, str):
-        return all([key in kwargs for key in keys])
-    else:
-        return keys in kwargs
-
-
-def anyinkwargs(keys, **kwargs):
-    if isinstance(keys, Iterable) and not isinstance(keys, str):
-        return any([key in kwargs for key in keys])
-    else:
-        return keys in kwargs
-
-
-def getfromkwargs(keys, default=None, astype=None, **kwargs):
-    res = [kwargs.get(k, default) for k in keys]
-    if astype is None:
-        return res
-    else:
-        return [astype(p) for p in res]
-
-
-def popfromkwargs(keys, d: dict = None, *args, default=None, astype=None, **kwargs):
-    res = [d.pop(k, default) for k in keys]
-    if astype is None:
-        return res
-    else:
-        return [astype(p) for p in res]
-
-
-def getallfromkwargs(keys, default=None, **kwargs):
-    params = getfromkwargs(keys, default=default, **kwargs)
-    if None not in params:
-        return params
-    else:
-        missing = list(filter(lambda p: p == default, params))
-        if len(missing) == 1:
-            key = keys[missing[0]]
-            raise RuntimeError(
-                "Parameter {} is missing from the definition!".format(key)
-            )
-        else:
-            missing_keys = [keys[i] for i in missing]
-            raise RuntimeError(
-                "Parameters {} is missing from the definition!".format(missing_keys)
-            )
-
-
-def getasany(keys, default=None, **kwargs):
-    try:
-        condition = [key in kwargs for key in keys]
-        if not any(condition) == True:
-            return default
-        return kwargs[keys[condition.index(True)]]
-    except Exception:
-        return None
-
-
-def countkwargs(fnc: Callable, **kwargs):
-    assert callable(fnc)
-    return sum(list(map(fnc, kwargs.keys())))
+# -*- coding: utf-8 -*-
+from typing import Callable
+
+try:
+    from collections.abc import Iterable
+except ImportError:
+    from collections import Iterable
+
+
+__all__ = [
+    "isinkwargs",
+    "allinkwargs",
+    "anyinkwargs",
+    "getfromkwargs",
+    "popfromkwargs",
+    "getallfromkwargs",
+    "getasany",
+    "countkwargs"
+]
+
+
+def isinkwargs(keys, **kwargs):
+    if isinstance(keys, Iterable) and not isinstance(keys, str):
+        return [key in kwargs for key in keys]
+    else:
+        return keys in kwargs
+
+
+def allinkwargs(keys, **kwargs):
+    if isinstance(keys, Iterable) and not isinstance(keys, str):
+        return all([key in kwargs for key in keys])
+    else:
+        return keys in kwargs
+
+
+def anyinkwargs(keys, **kwargs):
+    if isinstance(keys, Iterable) and not isinstance(keys, str):
+        return any([key in kwargs for key in keys])
+    else:
+        return keys in kwargs
+
+
+def getfromkwargs(keys, default=None, astype=None, **kwargs):
+    res = [kwargs.get(k, default) for k in keys]
+    if astype is None:
+        return res
+    else:
+        return [astype(p) for p in res]
+
+
+def popfromkwargs(keys, d: dict = None, *args, default=None, astype=None, **kwargs):
+    res = [d.pop(k, default) for k in keys]
+    if astype is None:
+        return res
+    else:
+        return [astype(p) for p in res]
+
+
+def getallfromkwargs(keys, default=None, **kwargs):
+    params = getfromkwargs(keys, default=default, **kwargs)
+    if None not in params:
+        return params
+    else:
+        missing = list(filter(lambda p: p == default, params))
+        if len(missing) == 1:
+            key = keys[missing[0]]
+            raise RuntimeError(
+                "Parameter {} is missing from the definition!".format(key)
+            )
+        else:
+            missing_keys = [keys[i] for i in missing]
+            raise RuntimeError(
+                "Parameters {} is missing from the definition!".format(missing_keys)
+            )
+
+
+def getasany(keys, default=None, **kwargs):
+    try:
+        condition = [key in kwargs for key in keys]
+        if not any(condition) == True:
+            return default
+        return kwargs[keys[condition.index(True)]]
+    except Exception:
+        return None
+
+
+def countkwargs(fnc: Callable, **kwargs):
+    assert callable(fnc)
+    return sum(list(map(fnc, kwargs.keys())))
```

### Comparing `sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/meta.py` & `sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/meta.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-# -*- coding: utf-8 -*-
-from abc import ABCMeta
-
-
-__all__ = ["ABCMeta_Weak", "ABCMeta_Strong", "ABCMeta_Safe"]
-
-
-def _is_callable(n, v):
-    return callable(v) and ("__" not in n)
-
-
-class ABCMeta_Weak(ABCMeta):
-    """
-    Standard python metaclass. It follows weak abstraction in the meaning, that
-    it is enough to implement the abstarcts in the instance, they impose no
-    restriction on the inherited class itself. Therefore, error only occurs at
-    runtime.
-
-    Notes
-    -----
-    This class provides nothing over the default behaviour offered by Python's
-    standard library, but it is equipped with some useful machinery for
-    subclasses that do. All other metaclasses of this module are subclasses of this
-    class.
-
-    See also
-    --------
-    :class:`~sigmaepsilon.core.abstract.ABC_Weak`
-    """
-
-    @staticmethod
-    def _get_cls_methods(namespace: dict, nomagic: bool = False) -> set:
-        """
-        Returns the callable items in the namespace of the class.
-        If `nomagic=False`, magic functions with trailing double
-        underscores are not returned.
-        """
-        if not nomagic:
-            return {name for name, value in namespace.items() if callable(value)}
-        else:
-            return {
-                name for name, value in namespace.items() if _is_callable(name, value)
-            }
-
-    @staticmethod
-    def _get_cls_abstracts(namespace: dict) -> set:
-        """
-        Returns the abstract methods of the namespace.
-        """
-        return getattr(namespace, "__abstractmethods__", set())
-
-    @staticmethod
-    def _get_base_methods(bases: list) -> dict:
-        """
-        Returns the callables in an iterable of base classes.
-        """
-        base_methods = {}
-        for base in bases:
-            base_methods[base.__name__] = {}
-            for k, v in base.__dict__.items():
-                if _is_callable(k, v):
-                    base_methods[base.__name__][k] = v
-        return base_methods
-
-    @staticmethod
-    def _get_base_abstracts(bases):
-        """
-        Returns the abstract callables in an iterable of base classes.
-        """
-        base_abc_methods = {}
-        for base in bases:
-            base_abc_methods[base.__name__] = getattr(
-                base, "__abstractmethods__", set()
-            )
-        return base_abc_methods
-
-
-class ABCMeta_Strong(ABCMeta_Weak):
-    """
-    Strong Python metaclass. It follows strong abstraction in the meaning, that
-    an abstract function of any of the base classes must be implemented or
-    delayed with the use of another @abstractmethod decorator.
-    Contrary to the weak metaclass, error occurs when the class is created.
-
-    See also
-    --------
-    :class:`~sigmaepsilon.core.abstract.ABC_Strong`
-    """
-
-    def __init__(self, name, bases, namespace, *args, **kwargs):
-        super().__init__(name, bases, namespace, *args, **kwargs)
-
-    def __new__(metaclass, name, bases, namespace, *args, **kwargs):
-        cls = super().__new__(metaclass, name, bases, namespace, *args, **kwargs)
-        cls_methods = metaclass._get_cls_methods(namespace)
-        for base in bases:
-            base_abstracts = set()
-            for method_name in getattr(base, "__abstractmethods__", set()):
-                value = getattr(cls, method_name, None)
-                if getattr(value, "__isabstractmethod__", False):
-                    base_abstracts.add(method_name)
-            for abstract in base_abstracts:
-                if abstract not in cls_methods:
-                    err_str = (
-                        f"Can't create abstract class {name}!"
-                        f" {name} must implement abstract method {abstract} of"
-                        f" class {base.__name__}."
-                    )
-                    raise TypeError(err_str)
-        return cls
-
-
-class ABCMeta_Safe(ABCMeta_Weak):
-    """
-    Python metaclass for safe inheritance. Throws a `TypeError`
-    if a method tries to shadow a method in any of the base
-    classes.
-    
-    See also
-    --------
-    :class:`~sigmaepsilon.core.abstract.ABC_Safe`
-    """
-
-    def __init__(self, name, bases, namespace, *args, **kwargs):
-        super().__init__(name, bases, namespace, *args, **kwargs)
-
-    def __new__(metaclass, name, bases, namespace, *args, **kwargs):
-        cls = super().__new__(metaclass, name, bases, namespace, *args, **kwargs)
-        cls_methods = metaclass._get_cls_methods(namespace, nomagic=True)
-        for base in bases:
-            for method in cls_methods:
-                if hasattr(base, method):
-                    err_str = (
-                        f"Can't create abstract class {name}!"
-                        f" Method {method} is already implemented in class"
-                        f" {base.__name__}."
-                    )
-                    raise TypeError(err_str)
-        return cls
+# -*- coding: utf-8 -*-
+from abc import ABCMeta
+
+
+__all__ = ["ABCMeta_Weak", "ABCMeta_Strong", "ABCMeta_Safe"]
+
+
+def _is_callable(n, v):
+    return callable(v) and ("__" not in n)
+
+
+class ABCMeta_Weak(ABCMeta):
+    """
+    Standard python metaclass. It follows weak abstraction in the meaning, that
+    it is enough to implement the abstarcts in the instance, they impose no
+    restriction on the inherited class itself. Therefore, error only occurs at
+    runtime.
+
+    Notes
+    -----
+    This class provides nothing over the default behaviour offered by Python's
+    standard library, but it is equipped with some useful machinery for
+    subclasses that do. All other metaclasses of this module are subclasses of this
+    class.
+
+    See also
+    --------
+    :class:`~sigmaepsilon.core.abstract.ABC_Weak`
+    """
+
+    @staticmethod
+    def _get_cls_methods(namespace: dict, nomagic: bool = False) -> set:
+        """
+        Returns the callable items in the namespace of the class.
+        If `nomagic=False`, magic functions with trailing double
+        underscores are not returned.
+        """
+        if not nomagic:
+            return {name for name, value in namespace.items() if callable(value)}
+        else:
+            return {
+                name for name, value in namespace.items() if _is_callable(name, value)
+            }
+
+    @staticmethod
+    def _get_cls_abstracts(namespace: dict) -> set:
+        """
+        Returns the abstract methods of the namespace.
+        """
+        return getattr(namespace, "__abstractmethods__", set())
+
+    @staticmethod
+    def _get_base_methods(bases: list) -> dict:
+        """
+        Returns the callables in an iterable of base classes.
+        """
+        base_methods = {}
+        for base in bases:
+            base_methods[base.__name__] = {}
+            for k, v in base.__dict__.items():
+                if _is_callable(k, v):
+                    base_methods[base.__name__][k] = v
+        return base_methods
+
+    @staticmethod
+    def _get_base_abstracts(bases):
+        """
+        Returns the abstract callables in an iterable of base classes.
+        """
+        base_abc_methods = {}
+        for base in bases:
+            base_abc_methods[base.__name__] = getattr(
+                base, "__abstractmethods__", set()
+            )
+        return base_abc_methods
+
+
+class ABCMeta_Strong(ABCMeta_Weak):
+    """
+    Strong Python metaclass. It follows strong abstraction in the meaning, that
+    an abstract function of any of the base classes must be implemented or
+    delayed with the use of another @abstractmethod decorator.
+    Contrary to the weak metaclass, error occurs when the class is created.
+
+    See also
+    --------
+    :class:`~sigmaepsilon.core.abstract.ABC_Strong`
+    """
+
+    def __init__(self, name, bases, namespace, *args, **kwargs):
+        super().__init__(name, bases, namespace, *args, **kwargs)
+
+    def __new__(metaclass, name, bases, namespace, *args, **kwargs):
+        cls = super().__new__(metaclass, name, bases, namespace, *args, **kwargs)
+        cls_methods = metaclass._get_cls_methods(namespace)
+        for base in bases:
+            base_abstracts = set()
+            for method_name in getattr(base, "__abstractmethods__", set()):
+                value = getattr(cls, method_name, None)
+                if getattr(value, "__isabstractmethod__", False):
+                    base_abstracts.add(method_name)
+            for abstract in base_abstracts:
+                if abstract not in cls_methods:
+                    err_str = (
+                        f"Can't create abstract class {name}!"
+                        f" {name} must implement abstract method {abstract} of"
+                        f" class {base.__name__}."
+                    )
+                    raise TypeError(err_str)
+        return cls
+
+
+class ABCMeta_Safe(ABCMeta_Weak):
+    """
+    Python metaclass for safe inheritance. Throws a `TypeError`
+    if a method tries to shadow a method in any of the base
+    classes.
+    
+    See also
+    --------
+    :class:`~sigmaepsilon.core.abstract.ABC_Safe`
+    """
+
+    def __init__(self, name, bases, namespace, *args, **kwargs):
+        super().__init__(name, bases, namespace, *args, **kwargs)
+
+    def __new__(metaclass, name, bases, namespace, *args, **kwargs):
+        cls = super().__new__(metaclass, name, bases, namespace, *args, **kwargs)
+        cls_methods = metaclass._get_cls_methods(namespace, nomagic=True)
+        for base in bases:
+            for method in cls_methods:
+                if hasattr(base, method):
+                    err_str = (
+                        f"Can't create abstract class {name}!"
+                        f" Method {method} is already implemented in class"
+                        f" {base.__name__}."
+                    )
+                    raise TypeError(err_str)
+        return cls
```

### Comparing `sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/osutils.py` & `sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/osutils.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-import os
-import inspect
-from typing import Callable
-
-__all__ = ["find_source_folder", "get_definition_file_path"]
-
-
-def find_source_folder(current_file: str = None, maxlevel: int = 10) -> str:
-    """
-    Returns the source folder.
-    """
-    if current_file is None:
-        current_file = __file__
-
-    parent_is_src = False
-    for _ in range(maxlevel):
-        parent_is_src = os.path.dirname(current_file).endswith("src")
-        if parent_is_src:
-            break
-        else:
-            current_file = os.path.dirname(current_file)
-
-    if parent_is_src:
-        return os.path.dirname(current_file)
-    else:
-        raise RuntimeError
-
-
-def get_definition_file_path(obj: Callable) -> str:
-    """
-    Returns the path of the file a class or a function is implemented in.
-    """
-    if inspect.isfunction(obj) or inspect.ismethod(obj):
-        file_path = inspect.getfile(obj)
-    elif inspect.isclass(obj):
-        file_path = inspect.getfile(obj.__class__)
-    else:
-        raise ValueError("Input must be a function or class.")
-
-    return os.path.abspath(file_path)
+import os
+import inspect
+from typing import Callable
+
+__all__ = ["find_source_folder", "get_definition_file_path"]
+
+
+def find_source_folder(current_file: str = None, maxlevel: int = 10) -> str:
+    """
+    Returns the source folder.
+    """
+    if current_file is None:
+        current_file = __file__
+
+    parent_is_src = False
+    for _ in range(maxlevel):
+        parent_is_src = os.path.dirname(current_file).endswith("src")
+        if parent_is_src:
+            break
+        else:
+            current_file = os.path.dirname(current_file)
+
+    if parent_is_src:
+        return os.path.dirname(current_file)
+    else:
+        raise RuntimeError
+
+
+def get_definition_file_path(obj: Callable) -> str:
+    """
+    Returns the path of the file a class or a function is implemented in.
+    """
+    if inspect.isfunction(obj) or inspect.ismethod(obj):
+        file_path = inspect.getfile(obj)
+    elif inspect.isclass(obj):
+        file_path = inspect.getfile(obj.__class__)
+    else:
+        raise ValueError("Input must be a function or class.")
+
+    return os.path.abspath(file_path)
```

### Comparing `sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/signature.py` & `sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/signature.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,195 +1,195 @@
-# -*- coding: utf-8 -*-
-from inspect import signature, Parameter
-from typing import Any
-from typing import Generic as _GenericAlias
-
-
-__all__ = ["Signature"]
-
-
-class Signature(dict):
-    """
-    A class to differentiate between function declarations using their
-    type signatures. It helps to decide if an implementation satisfies
-    some requirements imposed on a class.
-    """
-
-    __abckey__ = "isabstractoperation"
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(**kwargs)
-        setattr(self, "isabstract", "abstract" in args)
-
-    @classmethod
-    def from_function(cls, funcobj, *attrs, **kwargs):
-        if getattr(funcobj, cls.__abckey__, False):
-            sig = Signature("abstract", **kwargs)
-        else:
-            sig = Signature(**kwargs)
-
-        sig["name"] = funcobj.__name__
-        if len(attrs) > 0:
-            sig["attrs"] = frozenset(attrs)
-        else:
-            sig["attrs"] = frozenset()
-
-        params = signature(funcobj).parameters
-        if "args" in params or "kwargs" in params:
-            raise TypeError("Operation can only have a finite number of arguments!")
-        if "self" in params or "cls" in params:
-            sig["arity"] = len(params) - 1
-        else:
-            sig["arity"] = len(params)
-
-        if sig["arity"] == 0:
-            sig["dtype"] = [Any]
-        else:
-            sig["dtype"] = []
-            for pname, param in params.items():
-                if pname not in ["self", "cls"]:
-                    if param.annotation is not Parameter.empty:
-                        sig["dtype"].append(param.annotation)
-                    else:
-                        sig["dtype"].append(Any)
-
-        annotations = funcobj.__annotations__
-        if "return" in annotations:
-            sig["rtype"] = annotations["return"]
-        else:
-            sig["rtype"] = Any
-
-        return sig
-
-    @classmethod
-    def from_property(cls, funcobj, **kwargs):
-        if funcobj.isabstractattribute:
-            sig = Signature("abstract", **kwargs)
-        else:
-            sig = Signature(**kwargs)
-
-        sig["name"] = funcobj.__name__
-
-        annotations = funcobj.__annotations__
-        if "return" in annotations:
-            sig["rtype"] = annotations["return"]
-        else:
-            sig["rtype"] = Any
-
-        return sig
-
-    def compatible_function(self, other: "Signature") -> bool:
-        """
-        Returns True if two instances are compatible in terms of
-        domain type and result type.
-        """
-        if not isinstance(other, Signature):
-            return False
-
-        # check domain types
-        for type1, type2 in zip(self["dtype"], other["dtype"]):
-            if type1 == Any:
-                continue
-            elif isinstance(type1, _GenericAlias):
-                if not isinstance(type2, _GenericAlias):
-                    typeargs = type1.__dict__["__args__"]
-                    if type2 not in typeargs:
-                        return False
-                else:
-                    if type1 != type2:
-                        return False
-            else:
-                if type1 != type2:
-                    return False
-
-        # check result type
-        if isinstance(self["rtype"], _GenericAlias):
-            if not isinstance(other["rtype"], _GenericAlias):
-                typeargs = self["rtype"].__dict__["__args__"]
-                if not other["rtype"] in typeargs:
-                    return False
-            else:
-                if self["rtype"] != other["rtype"]:
-                    return False
-        elif self["rtype"] != Any:
-            if self["rtype"] != other["rtype"]:
-                return False
-
-        return True
-
-    def accepts_property(self, other: "Signature") -> bool:
-        """
-        Returns True if other (implemented operation's signature) is
-        compatible to self (abstract operation's signature).
-        Every value to every key of self must be present in other.
-        For example, here is where axioms are forced to match
-        between two signatures.
-        """
-        if any([not self.isabstract, other.isabstract]):
-            return False
-        if not self.compatible_op(other):
-            return False
-        if not self["name"] == other["name"]:
-            return False
-
-        for key, value in self.items():
-            if key not in ["rtype", "dtype"]:
-                if key in other:
-                    if isinstance(value, frozenset) and isinstance(
-                        other[key], frozenset
-                    ):
-                        if not value.issubset(other[key]):
-                            return False
-                    else:
-                        if not value == other[key]:
-                            return False
-                else:
-                    return False
-        return True
-
-    def update_function(self, other: "Signature"):
-        """
-        Updates self with the content of other. Both must be abstracts.
-        """
-        assert isinstance(other, Signature)
-        assert self.isabstract and other.isabstract
-        assert self.compatible_op(other)
-        for key, value in other.items():
-            if key not in ["rtype", "dtype"]:
-                if isinstance(value, frozenset):
-                    if key in self and isinstance(self[key], frozenset):
-                        s = set(self[key])
-                        s.update(set(value))
-                        self[key] = frozenset(s)
-                    else:
-                        self[key] = value
-                else:
-                    self[key] = value
-        return
-
-    def accepts_property(self, value: Any = None) -> bool:
-        """
-        Returns True if other (implemented attribute's signature) is
-        compatible to self (abstract attribute's signature).
-        Name and result type must match.
-        """
-        if not self.isabstract:
-            return False
-        if value is None:
-            return False
-
-        # check result type
-        if isinstance(self["rtype"], _GenericAlias):
-            if not isinstance(type(value), _GenericAlias):
-                typeargs = self["rtype"].__dict__["__args__"]
-                if not type(value) in typeargs:
-                    return False
-            else:
-                if self["rtype"] != type(value):
-                    return False
-        elif self["rtype"] != Any:
-            if self["rtype"] != type(value):
-                return False
-        return True
-
-    def accepts_parameters(self, *args):
-        raise NotImplementedError
+# -*- coding: utf-8 -*-
+from inspect import signature, Parameter
+from typing import Any
+from typing import Generic as _GenericAlias
+
+
+__all__ = ["Signature"]
+
+
+class Signature(dict):
+    """
+    A class to differentiate between function declarations using their
+    type signatures. It helps to decide if an implementation satisfies
+    some requirements imposed on a class.
+    """
+
+    __abckey__ = "isabstractoperation"
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(**kwargs)
+        setattr(self, "isabstract", "abstract" in args)
+
+    @classmethod
+    def from_function(cls, funcobj, *attrs, **kwargs):
+        if getattr(funcobj, cls.__abckey__, False):
+            sig = Signature("abstract", **kwargs)
+        else:
+            sig = Signature(**kwargs)
+
+        sig["name"] = funcobj.__name__
+        if len(attrs) > 0:
+            sig["attrs"] = frozenset(attrs)
+        else:
+            sig["attrs"] = frozenset()
+
+        params = signature(funcobj).parameters
+        if "args" in params or "kwargs" in params:
+            raise TypeError("Operation can only have a finite number of arguments!")
+        if "self" in params or "cls" in params:
+            sig["arity"] = len(params) - 1
+        else:
+            sig["arity"] = len(params)
+
+        if sig["arity"] == 0:
+            sig["dtype"] = [Any]
+        else:
+            sig["dtype"] = []
+            for pname, param in params.items():
+                if pname not in ["self", "cls"]:
+                    if param.annotation is not Parameter.empty:
+                        sig["dtype"].append(param.annotation)
+                    else:
+                        sig["dtype"].append(Any)
+
+        annotations = funcobj.__annotations__
+        if "return" in annotations:
+            sig["rtype"] = annotations["return"]
+        else:
+            sig["rtype"] = Any
+
+        return sig
+
+    @classmethod
+    def from_property(cls, funcobj, **kwargs):
+        if funcobj.isabstractattribute:
+            sig = Signature("abstract", **kwargs)
+        else:
+            sig = Signature(**kwargs)
+
+        sig["name"] = funcobj.__name__
+
+        annotations = funcobj.__annotations__
+        if "return" in annotations:
+            sig["rtype"] = annotations["return"]
+        else:
+            sig["rtype"] = Any
+
+        return sig
+
+    def compatible_function(self, other: "Signature") -> bool:
+        """
+        Returns True if two instances are compatible in terms of
+        domain type and result type.
+        """
+        if not isinstance(other, Signature):
+            return False
+
+        # check domain types
+        for type1, type2 in zip(self["dtype"], other["dtype"]):
+            if type1 == Any:
+                continue
+            elif isinstance(type1, _GenericAlias):
+                if not isinstance(type2, _GenericAlias):
+                    typeargs = type1.__dict__["__args__"]
+                    if type2 not in typeargs:
+                        return False
+                else:
+                    if type1 != type2:
+                        return False
+            else:
+                if type1 != type2:
+                    return False
+
+        # check result type
+        if isinstance(self["rtype"], _GenericAlias):
+            if not isinstance(other["rtype"], _GenericAlias):
+                typeargs = self["rtype"].__dict__["__args__"]
+                if not other["rtype"] in typeargs:
+                    return False
+            else:
+                if self["rtype"] != other["rtype"]:
+                    return False
+        elif self["rtype"] != Any:
+            if self["rtype"] != other["rtype"]:
+                return False
+
+        return True
+
+    def accepts_property(self, other: "Signature") -> bool:
+        """
+        Returns True if other (implemented operation's signature) is
+        compatible to self (abstract operation's signature).
+        Every value to every key of self must be present in other.
+        For example, here is where axioms are forced to match
+        between two signatures.
+        """
+        if any([not self.isabstract, other.isabstract]):
+            return False
+        if not self.compatible_op(other):
+            return False
+        if not self["name"] == other["name"]:
+            return False
+
+        for key, value in self.items():
+            if key not in ["rtype", "dtype"]:
+                if key in other:
+                    if isinstance(value, frozenset) and isinstance(
+                        other[key], frozenset
+                    ):
+                        if not value.issubset(other[key]):
+                            return False
+                    else:
+                        if not value == other[key]:
+                            return False
+                else:
+                    return False
+        return True
+
+    def update_function(self, other: "Signature"):
+        """
+        Updates self with the content of other. Both must be abstracts.
+        """
+        assert isinstance(other, Signature)
+        assert self.isabstract and other.isabstract
+        assert self.compatible_op(other)
+        for key, value in other.items():
+            if key not in ["rtype", "dtype"]:
+                if isinstance(value, frozenset):
+                    if key in self and isinstance(self[key], frozenset):
+                        s = set(self[key])
+                        s.update(set(value))
+                        self[key] = frozenset(s)
+                    else:
+                        self[key] = value
+                else:
+                    self[key] = value
+        return
+
+    def accepts_property(self, value: Any = None) -> bool:
+        """
+        Returns True if other (implemented attribute's signature) is
+        compatible to self (abstract attribute's signature).
+        Name and result type must match.
+        """
+        if not self.isabstract:
+            return False
+        if value is None:
+            return False
+
+        # check result type
+        if isinstance(self["rtype"], _GenericAlias):
+            if not isinstance(type(value), _GenericAlias):
+                typeargs = self["rtype"].__dict__["__args__"]
+                if not type(value) in typeargs:
+                    return False
+            else:
+                if self["rtype"] != type(value):
+                    return False
+        elif self["rtype"] != Any:
+            if self["rtype"] != type(value):
+                return False
+        return True
+
+    def accepts_parameters(self, *args):
+        raise NotImplementedError
```

### Comparing `sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/testing.py` & `sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/testing.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-"""
-This module contains reusable stuff for unittesting.
-"""
-import unittest
-from typing import Callable
-
-
-__all__ = ["SigmaEpsilonTestCase"]
-
-
-class SigmaEpsilonTestCase(unittest.TestCase):
-    """
-    A base class for test cases in SigmaEpsilon projects.
-    """
-    def assertFailsProperly(self, exc:Exception, fnc:Callable, *args, **kwargs):
-        """
-        Checks if a certain call fails the way it is expected to.
-        """
-        failed_properly = False
-        try:
-            fnc(*args, **kwargs)
-        except exc:
-            failed_properly = True
-        finally:
+"""
+This module contains reusable stuff for unittesting.
+"""
+import unittest
+from typing import Callable
+
+
+__all__ = ["SigmaEpsilonTestCase"]
+
+
+class SigmaEpsilonTestCase(unittest.TestCase):
+    """
+    A base class for test cases in SigmaEpsilon projects.
+    """
+    def assertFailsProperly(self, exc:Exception, fnc:Callable, *args, **kwargs):
+        """
+        Checks if a certain call fails the way it is expected to.
+        """
+        failed_properly = False
+        try:
+            fnc(*args, **kwargs)
+        except exc:
+            failed_properly = True
+        finally:
             self.assertTrue(failed_properly)
```

### Comparing `sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/typing.py` & `sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/typing.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# -*- coding: utf-8 -*-
-from typing import Hashable
-import six
-
-try:
-    from collections.abc import Iterable
-except ImportError:
-    from collections import Iterable
-
-
-__all__ = ["issequence", "ishashable"]
-
-
-def issequence(arg) -> bool:
-    """
-    Returns `True` if `arg` is any kind of iterable, but not a string,
-    returns `False` otherwise.
-    
-    Examples
-    --------
-    The formatter to use to print a floating point number with 4 digits:
-    
-    >>> from sigmaepsilon.core.typing import issequence
-    >>> issequence([1, 2])
-    True
-    
-    To print the actual value as a string:
-    
-    >>> issequence('lorem ipsum')
-    False    
-    """
-    return (
-        isinstance(arg, Iterable)
-        and not isinstance(arg, six.string_types)
-    )
-    
-
-def ishashable(obj):
-    """
-    Returns `True` if `obj` is hashable.
-    """
+# -*- coding: utf-8 -*-
+from typing import Hashable
+import six
+
+try:
+    from collections.abc import Iterable
+except ImportError:
+    from collections import Iterable
+
+
+__all__ = ["issequence", "ishashable"]
+
+
+def issequence(arg) -> bool:
+    """
+    Returns `True` if `arg` is any kind of iterable, but not a string,
+    returns `False` otherwise.
+    
+    Examples
+    --------
+    The formatter to use to print a floating point number with 4 digits:
+    
+    >>> from sigmaepsilon.core.typing import issequence
+    >>> issequence([1, 2])
+    True
+    
+    To print the actual value as a string:
+    
+    >>> issequence('lorem ipsum')
+    False    
+    """
+    return (
+        isinstance(arg, Iterable)
+        and not isinstance(arg, six.string_types)
+    )
+    
+
+def ishashable(obj):
+    """
+    Returns `True` if `obj` is hashable.
+    """
     return isinstance(obj, Hashable)
```

### Comparing `sigmaepsilon.core-0.0.1/src/sigmaepsilon/core/wrapping.py` & `sigmaepsilon.core-1.0.0/src/sigmaepsilon/core/wrapping.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,248 +1,248 @@
-# -*- coding: utf-8 -*-
-from typing import Any
-
-__all__ = ["Wrapper", "wrapper", "customwrapper", "wrap"]
-
-NoneType = type(None)
-
-
-class Wrapper:
-    """
-    Wrapper base class that makes it easy (and safe) to extend other objects.
-    Based on the provided arguments at initialization, the wrapper either
-    
-    (a) wraps an existing object at object creation provided as a keyword
-        argument with `Wrapper.wrapkey`
-    (b) wraps an existing object at object creation if it is a positional
-        argument and an instance of `Wrapper.wraptype`
-    (b) wraps the object Wrapper.wraptype(*args, **kwargs) if
-        `Wrapper.wraptype` is not `None`
-        
-    The attributes and methods of the wrapped instance are all accessible
-    through the wrapper.
-    
-    Using a wrapper is a good idea if you want to easily extend the functionality
-    provided by a class of an external library without having to worry about shadowing
-    an important method and thus risking to break the behaviour of the wrapped object.
-        
-    Examples
-    --------
-    >>> import numpy as np
-    >>>
-    >>> arr = np.eye(3)
-    >>> wrapper = Wrapper(wrap=arr)
-    
-    Now the wrapped NumPy array is accessible as `wrapper.wrapped`.
-    
-    A wrapper class can be used to extend the behaviour:
-    
-    >>> MyWrapper(Wrapper):
-    >>>     wraptype = np.ndarray
-    >>>     
-    >>>     def invert() -> None:
-    >>>         self.wrapped = np.linalg.inv(self.wrapped)
-    
-    With this solution, you don't have to worry about shadowing an existing
-    implementation of NumPy arrays. Not that NumPy arrays might not have a method
-    called `invert` at the time of implementing the class `MyWrapper`, but it might
-    change in the future. You can even check that internally and get notified: 
-    
-    >>> import warnings
-    >>>
-    >>> MyWrapper(Wrapper):
-    >>>     wraptype = np.ndarray
-    >>>     
-    >>>     def invert() -> None:
-    >>>         if hasattr(self.wrapped, "invert"):
-    >>>             warnings.warn("'invert' already exists in the object")
-    >>>         self.wrapped = np.linalg.inv(self.wrapped)
-    
-    Then, to wrap a NumPy array, you can do this (since the `wraptype` attribute is set,
-    the MyWrapper class is going to catch the object to wrap as a positional argument):
-    
-    >>> wrapper = MyWrapper(arr)
-    """
-    wrapkey: str = "wrap"
-    wraptype: Any = NoneType
-
-    def __init__(self, *args, **kwargs):
-        super().__init__()
-        self._wrapped = None
-        self.wrap(kwargs.get(self.wrapkey, None))
-
-        if self._wrapped is None and self.wraptype is not NoneType:
-            for arg in args:
-                if isinstance(arg, self.wraptype):
-                    self._wrapped = arg
-                    break
-
-            if self._wrapped is None:
-                try:
-                    if self.wraptype is not NoneType:
-                        self._wrapped = self.wraptype(*args, **kwargs)
-                except Exception:
-                    raise ValueError(
-                        "Wrapped class '{}' cannot be "
-                        + "initiated with these "
-                        + "arguments".format(self.wraptype.__name__)
-                    )
-        else:
-            if self.wraptype is not NoneType:
-                assert isinstance(
-                    self._wrapped, self.wraptype
-                ), "Wrong type, unable to wrap object : {}".format(self._wrapped)
-
-    @property
-    def wrapped(self):
-        """Retruns the wrapped object."""
-        return self._wrapped
-
-    def wrap(self, obj: Any=None) -> Any:
-        """Wraps the provided object and returns the wrapper instance."""
-        if self.wraptype is not NoneType:
-            if isinstance(obj, self.wraptype):
-                self._wrapped = obj
-        else:
-            self._wrapped = obj
-        return self
-
-    def wraps(self):
-        """Returns `True` if the instance wraps something or `False` if it doesn't."""
-        return self._wrapped is not None
-
-    def wrapped_obj(self):
-        return self._wrapped
-
-    def __hasattr__(self, attr):
-        return any([attr in self.__dict__, attr in self._wrapped.__dict__])
-
-    def __getattr__(self, attr):
-        if attr in self.__dict__:
-            return getattr(self, attr)
-        try:
-            return getattr(self._wrapped, attr)
-        except Exception:
-            raise AttributeError(
-                "'{}' object has no attribute \
-                called {}".format(
-                    self.__class__.__name__, attr
-                )
-            )
-
-    def __getitem__(self, index):
-        try:
-            return super().__getitem__(index)
-        except Exception:
-            try:
-                return self._wrapped.__getitem__(index)
-            except Exception:
-                raise TypeError(
-                    "'{}' object is not "
-                    "subscriptable".format(self.__class__.__name__)
-                )
-
-    def __setitem__(self, index, value):
-        try:
-            return super().__setitem__(index, value)
-        except Exception:
-            try:
-                return self._wrapped.__setitem__(index, value)
-            except Exception:
-                raise TypeError(
-                    "'{}' object does not support "
-                    "item assignment".format(self.__class__.__name__)
-                )
-
-
-def customwrapper(*, wrapkey:str="wrap", wraptype: Any=NoneType) -> Wrapper:
-    """
-    A factory function that returns a class decorator turning a class type 
-    into a wrapper type, that either
-    
-    (a) wraps an existing object at object creation provided as a keyword
-        argument with wrapkey
-    (b) wraps an existing object at object creation if it is a positional
-        argument and an instance of wraptype
-    (b) wraps the object wraptype(*args, **kwargs)
-    
-    See also
-    --------
-    :class:`~sigmaepsilon.core.wrapping.Wrapper`
-    
-    Examples
-    --------
-    Take this example from the :class:`~sigmaepsilon.core.wrapping.Wrapper` class:
-    
-    >>> MyWrapper(Wrapper):
-    >>>     wraptype = np.ndarray
-    >>>
-    >>>     def invert() -> None:
-    >>>         self.wrapped = np.linalg.inv(self.wrapped)
-    
-    An equivalent implementation of this is the following:
-    
-    >>> @customwrapper(wraptype=np.ndarray)
-    >>> MyWrapper:
-    >>>     def invert() -> None:
-    >>>         self.wrapped = np.linalg.inv(self.wrapped)
-    
-    Notice how the class `MyWrapper` is not inherited from the `Wrapper` class.
-    """
-
-    class BaseWrapperType(Wrapper):
-        ...
-
-    BaseWrapperType.wrapkey = wrapkey
-    BaseWrapperType.wraptype = wraptype
-
-    def wrapper(BaseType):
-        class WrapperType(BaseWrapperType, BaseType):
-            basetype = BaseType
-
-        return WrapperType
-
-    return wrapper
-
-
-def wrapper(BaseType: Any) -> Wrapper:
-    """
-    Simple class decorator that turns a type into a wrapper with default
-    behaviour.
-    
-    Notes
-    -----
-    This is the same as using the :func:`~sigmaepsilon.core.wrapping.customwrapper`
-    with the default values.
-    
-    See also
-    --------
-    :class:`~sigmaepsilon.core.wrapping.Wrapper`
-    :func:`~sigmaepsilon.core.wrapping.customwrapper`
-    
-    Example
-    -------
-    >>> @wrapper
-    >>> MyWrapper:
-    >>>     def invert() -> None:
-    >>>         self.wrapped = np.linalg.inv(self.wrapped)
-    """
-    class WrapperType(Wrapper, BaseType):
-        basetype = BaseType
-
-    return WrapperType
-
-
-def wrap(obj: object) -> Wrapper:
-    """
-    Wraps an object and returns the wrapper.
-    
-    See also
-    --------
-    :class:`~sigmaepsilon.core.wrapping.Wrapper`
-    
-    Example
-    -------
-    >>> import numpy as np
-    >>> wrapper = wrap(np.eye(3))
-    """
-    return Wrapper(wrap=obj)
+# -*- coding: utf-8 -*-
+from typing import Any
+
+__all__ = ["Wrapper", "wrapper", "customwrapper", "wrap"]
+
+NoneType = type(None)
+
+
+class Wrapper:
+    """
+    Wrapper base class that makes it easy (and safe) to extend other objects.
+    Based on the provided arguments at initialization, the wrapper either
+    
+    (a) wraps an existing object at object creation provided as a keyword
+        argument with `Wrapper.wrapkey`
+    (b) wraps an existing object at object creation if it is a positional
+        argument and an instance of `Wrapper.wraptype`
+    (b) wraps the object Wrapper.wraptype(*args, **kwargs) if
+        `Wrapper.wraptype` is not `None`
+        
+    The attributes and methods of the wrapped instance are all accessible
+    through the wrapper.
+    
+    Using a wrapper is a good idea if you want to easily extend the functionality
+    provided by a class of an external library without having to worry about shadowing
+    an important method and thus risking to break the behaviour of the wrapped object.
+        
+    Examples
+    --------
+    >>> import numpy as np
+    >>>
+    >>> arr = np.eye(3)
+    >>> wrapper = Wrapper(wrap=arr)
+    
+    Now the wrapped NumPy array is accessible as `wrapper.wrapped`.
+    
+    A wrapper class can be used to extend the behaviour:
+    
+    >>> MyWrapper(Wrapper):
+    >>>     wraptype = np.ndarray
+    >>>     
+    >>>     def invert() -> None:
+    >>>         self.wrapped = np.linalg.inv(self.wrapped)
+    
+    With this solution, you don't have to worry about shadowing an existing
+    implementation of NumPy arrays. Not that NumPy arrays might not have a method
+    called `invert` at the time of implementing the class `MyWrapper`, but it might
+    change in the future. You can even check that internally and get notified: 
+    
+    >>> import warnings
+    >>>
+    >>> MyWrapper(Wrapper):
+    >>>     wraptype = np.ndarray
+    >>>     
+    >>>     def invert() -> None:
+    >>>         if hasattr(self.wrapped, "invert"):
+    >>>             warnings.warn("'invert' already exists in the object")
+    >>>         self.wrapped = np.linalg.inv(self.wrapped)
+    
+    Then, to wrap a NumPy array, you can do this (since the `wraptype` attribute is set,
+    the MyWrapper class is going to catch the object to wrap as a positional argument):
+    
+    >>> wrapper = MyWrapper(arr)
+    """
+    wrapkey: str = "wrap"
+    wraptype: Any = NoneType
+
+    def __init__(self, *args, **kwargs):
+        super().__init__()
+        self._wrapped = None
+        self.wrap(kwargs.get(self.wrapkey, None))
+
+        if self._wrapped is None and self.wraptype is not NoneType:
+            for arg in args:
+                if isinstance(arg, self.wraptype):
+                    self._wrapped = arg
+                    break
+
+            if self._wrapped is None:
+                try:
+                    if self.wraptype is not NoneType:
+                        self._wrapped = self.wraptype(*args, **kwargs)
+                except Exception:
+                    raise ValueError(
+                        "Wrapped class '{}' cannot be "
+                        + "initiated with these "
+                        + "arguments".format(self.wraptype.__name__)
+                    )
+        else:
+            if self.wraptype is not NoneType:
+                assert isinstance(
+                    self._wrapped, self.wraptype
+                ), "Wrong type, unable to wrap object : {}".format(self._wrapped)
+
+    @property
+    def wrapped(self):
+        """Retruns the wrapped object."""
+        return self._wrapped
+
+    def wrap(self, obj: Any=None) -> Any:
+        """Wraps the provided object and returns the wrapper instance."""
+        if self.wraptype is not NoneType:
+            if isinstance(obj, self.wraptype):
+                self._wrapped = obj
+        else:
+            self._wrapped = obj
+        return self
+
+    def wraps(self):
+        """Returns `True` if the instance wraps something or `False` if it doesn't."""
+        return self._wrapped is not None
+
+    def wrapped_obj(self):
+        return self._wrapped
+
+    def __hasattr__(self, attr):
+        return any([attr in self.__dict__, attr in self._wrapped.__dict__])
+
+    def __getattr__(self, attr):
+        if attr in self.__dict__:
+            return getattr(self, attr)
+        try:
+            return getattr(self._wrapped, attr)
+        except Exception:
+            raise AttributeError(
+                "'{}' object has no attribute \
+                called {}".format(
+                    self.__class__.__name__, attr
+                )
+            )
+
+    def __getitem__(self, index):
+        try:
+            return super().__getitem__(index)
+        except Exception:
+            try:
+                return self._wrapped.__getitem__(index)
+            except Exception:
+                raise TypeError(
+                    "'{}' object is not "
+                    "subscriptable".format(self.__class__.__name__)
+                )
+
+    def __setitem__(self, index, value):
+        try:
+            return super().__setitem__(index, value)
+        except Exception:
+            try:
+                return self._wrapped.__setitem__(index, value)
+            except Exception:
+                raise TypeError(
+                    "'{}' object does not support "
+                    "item assignment".format(self.__class__.__name__)
+                )
+
+
+def customwrapper(*, wrapkey:str="wrap", wraptype: Any=NoneType) -> Wrapper:
+    """
+    A factory function that returns a class decorator turning a class type 
+    into a wrapper type, that either
+    
+    (a) wraps an existing object at object creation provided as a keyword
+        argument with wrapkey
+    (b) wraps an existing object at object creation if it is a positional
+        argument and an instance of wraptype
+    (b) wraps the object wraptype(*args, **kwargs)
+    
+    See also
+    --------
+    :class:`~sigmaepsilon.core.wrapping.Wrapper`
+    
+    Examples
+    --------
+    Take this example from the :class:`~sigmaepsilon.core.wrapping.Wrapper` class:
+    
+    >>> MyWrapper(Wrapper):
+    >>>     wraptype = np.ndarray
+    >>>
+    >>>     def invert() -> None:
+    >>>         self.wrapped = np.linalg.inv(self.wrapped)
+    
+    An equivalent implementation of this is the following:
+    
+    >>> @customwrapper(wraptype=np.ndarray)
+    >>> MyWrapper:
+    >>>     def invert() -> None:
+    >>>         self.wrapped = np.linalg.inv(self.wrapped)
+    
+    Notice how the class `MyWrapper` is not inherited from the `Wrapper` class.
+    """
+
+    class BaseWrapperType(Wrapper):
+        ...
+
+    BaseWrapperType.wrapkey = wrapkey
+    BaseWrapperType.wraptype = wraptype
+
+    def wrapper(BaseType):
+        class WrapperType(BaseWrapperType, BaseType):
+            basetype = BaseType
+
+        return WrapperType
+
+    return wrapper
+
+
+def wrapper(BaseType: Any) -> Wrapper:
+    """
+    Simple class decorator that turns a type into a wrapper with default
+    behaviour.
+    
+    Notes
+    -----
+    This is the same as using the :func:`~sigmaepsilon.core.wrapping.customwrapper`
+    with the default values.
+    
+    See also
+    --------
+    :class:`~sigmaepsilon.core.wrapping.Wrapper`
+    :func:`~sigmaepsilon.core.wrapping.customwrapper`
+    
+    Example
+    -------
+    >>> @wrapper
+    >>> MyWrapper:
+    >>>     def invert() -> None:
+    >>>         self.wrapped = np.linalg.inv(self.wrapped)
+    """
+    class WrapperType(Wrapper, BaseType):
+        basetype = BaseType
+
+    return WrapperType
+
+
+def wrap(obj: object) -> Wrapper:
+    """
+    Wraps an object and returns the wrapper.
+    
+    See also
+    --------
+    :class:`~sigmaepsilon.core.wrapping.Wrapper`
+    
+    Example
+    -------
+    >>> import numpy as np
+    >>> wrapper = wrap(np.eye(3))
+    """
+    return Wrapper(wrap=obj)
```

### Comparing `sigmaepsilon.core-0.0.1/src/sigmaepsilon.core.egg-info/PKG-INFO` & `sigmaepsilon.core-1.0.0/src/sigmaepsilon.core.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-Metadata-Version: 2.1
-Name: sigmaepsilon.core
-Version: 0.0.1
-Summary: Common developer utilities for Python projects.
-Author-email: SigmaEpsilon <bencebalogh@sigmaepsilon.com>
-Maintainer-email: SigmaEpsilon <bencebalogh@sigmaepsilon.com>
-License: MIT License
-        
-        Copyright (c) 2023 SigmaEpsilon
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/sigma-epsilon/sigmaepsilon.core
-Keywords: engineering,mechanics,science,numerical analysis,finite element method,solid mechanics,optimization
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Operating System :: OS Independent
-Requires-Python: <3.11,>=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: dev
-Provides-Extra: docs
-License-File: LICENSE
-
-# **sigmaepsilon.core** - Common developer utilities for Python projects
-
-[![CircleCI](https://circleci.com/gh/dewloosh/sigmaepsilon.core.svg?style=shield)](https://circleci.com/gh/sigma-epsilon/sigmaepsilon.core)
-[![Documentation Status](https://readthedocs.org/projects/sigmaepsiloncore/badge/?version=latest)](https://sigmaepsiloncore.readthedocs.io/en/latest/?badge=latest)
-[![Python 3.7-3.10](https://img.shields.io/badge/python-3.7%E2%80%923.10-blue)](https://www.python.org)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![PyPI](https://badge.fury.io/py/sigmaepsilon.math.svg)](https://pypi.org/project/sigmaepsilon.math)
-
-The package contains some usefull stuff for general Python development activites that turned out to be highly reusable during developing projects in the SigmaEpsilon namespace.
-
-Some of the most notable contents:
-
-* Metaprogramming
-  * A collection of meta and abstract base classes.
-  * A `classproperty` decorator.
-  * A solution to enforce abstract class properties on a class.
-  
-* Wrapping
-  * An extendible `Wrapper` class and a few factory functions to help you safely wrap objects.
-
-## **Documentation**
-
-The [documentation](https://sigmaepsiloncore.readthedocs.io/en/latest/) is hosted on ReadTheDocs.
-
-## **Installation**
-
-`sigmaepsilon.core` can be installed (either in a virtual enviroment or globally) from PyPI using `pip` on Python >= 3.7:
-
-```console
->>> pip install sigmaepsilon.core
-```
-
-or chechkout with the following command using GitHub CLI
-
-```console
-gh repo clone sigma-epsilon/sigmaepsilon.core
-```
-
-and install from source by typing
-
-```console
->>> pip install .
-```
-
-If you want to run the tests, you can install the necessary optional dependencies like this
-
-```console
->>> pip install ".[test]"
-```
-
-### For developers
-
-For development purposes, it is suggested to install the package in editable mode, with the optional dependencies for both testing, development and documentation
-
-```console
->>> pip install -e ".[test, dev, docs]"
-```
-
-## Testing
-
-To run the tests, run the following command in the root of the project:
-
-```console
->>> pytest
-```
-
-## **License**
-
-This package is licensed under the MIT license. See the attached LICENSE file for the details.
+Metadata-Version: 2.1
+Name: sigmaepsilon.core
+Version: 1.0.0
+Summary: Common developer utilities for Python projects.
+Author-email: SigmaEpsilon <bencebalogh@sigmaepsilon.com>
+Maintainer-email: SigmaEpsilon <bencebalogh@sigmaepsilon.com>
+License: MIT License
+        
+        Copyright (c) 2023 SigmaEpsilon
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/sigma-epsilon/sigmaepsilon.core
+Keywords: engineering,mechanics,science,numerical analysis,finite element method,solid mechanics,optimization
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Operating System :: OS Independent
+Requires-Python: <3.11,>=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: dev
+Provides-Extra: docs
+License-File: LICENSE
+
+# **sigmaepsilon.core** - Common developer utilities for Python projects
+
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/sigma-epsilon/sigmaepsilon.core/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/sigma-epsilon/sigmaepsilon.core/tree/main)
+[![Documentation Status](https://readthedocs.org/projects/sigmaepsiloncore/badge/?version=latest)](https://sigmaepsiloncore.readthedocs.io/en/latest/?badge=latest)
+[![Python 3.7-3.10](https://img.shields.io/badge/python-3.7%E2%80%923.10-blue)](https://www.python.org)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![PyPI](https://badge.fury.io/py/sigmaepsilon.core.svg)](https://pypi.org/project/sigmaepsilon.core)
+
+The package contains some usefull stuff for general Python development activites that turned out to be highly reusable during developing projects in the SigmaEpsilon namespace.
+
+Some of the most notable contents:
+
+* Metaprogramming
+  * A collection of meta and abstract base classes.
+  * A `classproperty` decorator.
+  * A solution to enforce abstract class properties on a class.
+  
+* Wrapping
+  * An extendible `Wrapper` class and a few factory functions to help you safely wrap objects.
+
+## **Documentation**
+
+The [documentation](https://sigmaepsiloncore.readthedocs.io/en/latest/) is hosted on ReadTheDocs.
+
+## **Installation**
+
+`sigmaepsilon.core` can be installed (either in a virtual enviroment or globally) from PyPI using `pip` on Python >= 3.7:
+
+```console
+>>> pip install sigmaepsilon.core
+```
+
+or chechkout with the following command using GitHub CLI
+
+```console
+gh repo clone sigma-epsilon/sigmaepsilon.core
+```
+
+and install from source by typing
+
+```console
+>>> pip install .
+```
+
+If you want to run the tests, you can install the package along with the necessary optional dependencies like this
+
+```console
+>>> pip install ".[test]"
+```
+
+### For developers
+
+For development purposes, it is suggested to install the package in editable mode, with the optional dependencies for both testing, development and documentation
+
+```console
+>>> pip install -e ".[test, dev, docs]"
+```
+
+## Testing
+
+To run the tests, run the following command in the root of the project:
+
+```console
+>>> pytest
+```
+
+## **License**
+
+This package is licensed under the MIT license. See the attached LICENSE file for the details.
```

### Comparing `sigmaepsilon.core-0.0.1/tests/test_attr.py` & `sigmaepsilon.core-1.0.0/tests/test_attr.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# -*- coding: utf-8 -*-
-import unittest
-
-from sigmaepsilon.core import attributor
-
-
-class TestAttributor(unittest.TestCase):
-
-    def test_attributor(self):
-        axiom = attributor('__isaxiom__')
-        abstractaxiom = attributor('__isaxiom__', '__isabstractmethod__')
-
-        @axiom
-        def foo(a, b): return 'an axiom'
-        self.assertTrue(foo.__isaxiom__)
-        
-        @abstractaxiom
-        def foo(a, b): return 'an abstract axiom'
-        self.assertTrue(foo.__isaxiom__)
-        self.assertTrue(foo.__isabstractmethod__)
-
-if __name__ == "__main__":
-    
+# -*- coding: utf-8 -*-
+import unittest
+
+from sigmaepsilon.core import attributor
+
+
+class TestAttributor(unittest.TestCase):
+
+    def test_attributor(self):
+        axiom = attributor('__isaxiom__')
+        abstractaxiom = attributor('__isaxiom__', '__isabstractmethod__')
+
+        @axiom
+        def foo(a, b): return 'an axiom'
+        self.assertTrue(foo.__isaxiom__)
+        
+        @abstractaxiom
+        def foo(a, b): return 'an abstract axiom'
+        self.assertTrue(foo.__isaxiom__)
+        self.assertTrue(foo.__isabstractmethod__)
+
+if __name__ == "__main__":
+    
     unittest.main()
```

### Comparing `sigmaepsilon.core-0.0.1/tests/test_tools.py` & `sigmaepsilon.core-1.0.0/tests/test_tools.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-# -*- coding: utf-8 -*-
-import unittest
-
-import math
-
-from sigmaepsilon.core.typing import issequence
-from sigmaepsilon.core.formatting import float_to_str_sig
-from sigmaepsilon.core.decorate import suppress, timeit
-from sigmaepsilon.core.alphabet import alphabet, ordrange, latinrange, \
-    urange, greekrange, arabicrange
-from sigmaepsilon.core.kwargtools import isinkwargs, allinkwargs, anyinkwargs, \
-    getfromkwargs, popfromkwargs, getallfromkwargs, getasany, countkwargs
-
-
-class TestTools(unittest.TestCase):
-
-    def test_tools(self):
-        assert float_to_str_sig(math.pi, sig=4) == '3.142'
-        seq = [math.pi, math.pi]
-        assert issequence(seq)
-        assert not issequence(seq[0])
-        assert float_to_str_sig(seq, sig=4) == ['3.142', '3.142']
-        assert issequence([1, 2, 3])
-        assert not issequence('123')
-
-    def test_kwargtools(self):
-        kwargs = dict(a = 1, c = 2)
-        assert isinkwargs('a', **kwargs)
-        assert all(isinkwargs(['a', 'c'], **kwargs))
-        assert not isinkwargs('b', **kwargs)
-        assert not any(isinkwargs(['b', 'd'], **kwargs))
-        assert any(isinkwargs(['a', 'b'], **kwargs))
-        assert any(isinkwargs(['c', 'd'], **kwargs))
-        assert allinkwargs(['a', 'c'], **kwargs)
-        assert allinkwargs('a', **kwargs)
-        assert anyinkwargs(['d', 'c'], **kwargs)
-        assert anyinkwargs('c', **kwargs)
-        assert getfromkwargs(['a'], None, int, **kwargs) == [1]
-        assert getfromkwargs(['b'], None, None, **kwargs) == [None]
-        assert getallfromkwargs(['a', 'c'], None, **kwargs) == [1, 2]
-        assert getasany(['a', 'b'], None, **kwargs) == 1
-        
-        d = {'E1': 1, 'E2': 2, 'G12': 12, 'NU23': 0}
-        nE = countkwargs(lambda s: s[0] == 'E', **d)
-        nG = countkwargs(lambda s: s[0] == 'G', **d)
-        nNU = countkwargs(lambda s: s[0:2] == 'NU', **d)
-        assert nE == 2
-        assert nG == 1
-        assert nNU == 1
-        popfromkwargs(['E1'], d)
-        assert isinstance(popfromkwargs(['E2'], d, astype=float)[0], float)
-        assert 'E1' not in d
-        
-    def test_alphabet(self):
-        for abctype in ['ord', 'latin', 'u', 'greek']:
-            g = alphabet(abctype)
-            [next(g) for i in range(5)]
-        
-        ordrange(5)
-        latinrange(5)
-        urange(5)
-        greekrange(5)
-        arabicrange(5)
-                
-        lrange = latinrange(5, start='i')
-        grange = greekrange(5)
-        orange = ordrange(5)
-        arange = arabicrange(5, start=1)
-
-        abc = alphabet('latin', start='i')
-        next(abc)
-
-        abc = alphabet(start='u')
-        next(abc)
-            
-        abc = alphabet('u', start='\x03')
-        next(abc)
-        
-        abc = alphabet('u', start='\x03')
-        pokerstr = [next(abc) for _ in range(4)]
-        
-        
-    def test_misc(self):
-        
-        @timeit
-        def foo(): return None
-        
-        @suppress
-        def foo(): return None
-            
-
-
-if __name__ == "__main__":
-    unittest.main()
+# -*- coding: utf-8 -*-
+import unittest
+
+import math
+
+from sigmaepsilon.core.typing import issequence
+from sigmaepsilon.core.formatting import float_to_str_sig
+from sigmaepsilon.core.decorate import suppress, timeit
+from sigmaepsilon.core.alphabet import alphabet, ordrange, latinrange, \
+    urange, greekrange, arabicrange
+from sigmaepsilon.core.kwargtools import isinkwargs, allinkwargs, anyinkwargs, \
+    getfromkwargs, popfromkwargs, getallfromkwargs, getasany, countkwargs
+
+
+class TestTools(unittest.TestCase):
+
+    def test_tools(self):
+        assert float_to_str_sig(math.pi, sig=4) == '3.142'
+        seq = [math.pi, math.pi]
+        assert issequence(seq)
+        assert not issequence(seq[0])
+        assert float_to_str_sig(seq, sig=4) == ['3.142', '3.142']
+        assert issequence([1, 2, 3])
+        assert not issequence('123')
+
+    def test_kwargtools(self):
+        kwargs = dict(a = 1, c = 2)
+        assert isinkwargs('a', **kwargs)
+        assert all(isinkwargs(['a', 'c'], **kwargs))
+        assert not isinkwargs('b', **kwargs)
+        assert not any(isinkwargs(['b', 'd'], **kwargs))
+        assert any(isinkwargs(['a', 'b'], **kwargs))
+        assert any(isinkwargs(['c', 'd'], **kwargs))
+        assert allinkwargs(['a', 'c'], **kwargs)
+        assert allinkwargs('a', **kwargs)
+        assert anyinkwargs(['d', 'c'], **kwargs)
+        assert anyinkwargs('c', **kwargs)
+        assert getfromkwargs(['a'], None, int, **kwargs) == [1]
+        assert getfromkwargs(['b'], None, None, **kwargs) == [None]
+        assert getallfromkwargs(['a', 'c'], None, **kwargs) == [1, 2]
+        assert getasany(['a', 'b'], None, **kwargs) == 1
+        
+        d = {'E1': 1, 'E2': 2, 'G12': 12, 'NU23': 0}
+        nE = countkwargs(lambda s: s[0] == 'E', **d)
+        nG = countkwargs(lambda s: s[0] == 'G', **d)
+        nNU = countkwargs(lambda s: s[0:2] == 'NU', **d)
+        assert nE == 2
+        assert nG == 1
+        assert nNU == 1
+        popfromkwargs(['E1'], d)
+        assert isinstance(popfromkwargs(['E2'], d, astype=float)[0], float)
+        assert 'E1' not in d
+        
+    def test_alphabet(self):
+        for abctype in ['ord', 'latin', 'u', 'greek']:
+            g = alphabet(abctype)
+            [next(g) for i in range(5)]
+        
+        ordrange(5)
+        latinrange(5)
+        urange(5)
+        greekrange(5)
+        arabicrange(5)
+                
+        lrange = latinrange(5, start='i')
+        grange = greekrange(5)
+        orange = ordrange(5)
+        arange = arabicrange(5, start=1)
+
+        abc = alphabet('latin', start='i')
+        next(abc)
+
+        abc = alphabet(start='u')
+        next(abc)
+            
+        abc = alphabet('u', start='\x03')
+        next(abc)
+        
+        abc = alphabet('u', start='\x03')
+        pokerstr = [next(abc) for _ in range(4)]
+        
+        
+    def test_misc(self):
+        
+        @timeit
+        def foo(): return None
+        
+        @suppress
+        def foo(): return None
+            
+
+
+if __name__ == "__main__":
+    unittest.main()
```

