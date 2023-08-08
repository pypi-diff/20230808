# Comparing `tmp/sphinxcontrib-websupport-1.2.4.tar.gz` & `tmp/sphinxcontrib_websupport-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sphinxcontrib-websupport-1.2.4.tar", last modified: Sun Aug  9 15:34:57 2020, max compression
+gzip compressed data, was "sphinxcontrib_websupport-1.2.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinxcontrib-websupport-1.2.4.tar` & `sphinxcontrib_websupport-1.2.5.tar`

### file list

```diff
@@ -1,122 +1,91 @@
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-08-09 15:34:57.841057 sphinxcontrib-websupport-1.2.4/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1259 2020-08-09 15:06:29.000000 sphinxcontrib-websupport-1.2.4/CHANGES
--rw-r--r--   0 tkomiya    (502) staff       (20)     1443 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/LICENSE
--rw-r--r--   0 tkomiya    (502) staff       (20)      196 2020-03-21 08:18:20.000000 sphinxcontrib-websupport-1.2.4/MANIFEST.in
--rw-r--r--   0 tkomiya    (502) staff       (20)     1333 2020-08-09 15:34:57.841329 sphinxcontrib-websupport-1.2.4/PKG-INFO
--rw-r--r--   0 tkomiya    (502) staff       (20)      840 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/README.rst
--rw-r--r--   0 tkomiya    (502) staff       (20)      414 2020-08-09 15:34:57.846827 sphinxcontrib-websupport-1.2.4/setup.cfg
--rw-r--r--   0 tkomiya    (502) staff       (20)     2435 2020-08-09 15:06:29.000000 sphinxcontrib-websupport-1.2.4/setup.py
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-08-09 15:34:57.805206 sphinxcontrib-websupport-1.2.4/sphinxcontrib/
--rw-r--r--   0 tkomiya    (502) staff       (20)       80 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/sphinxcontrib/__init__.py
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-08-09 15:34:57.807259 sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/
--rw-r--r--   0 tkomiya    (502) staff       (20)      563 2020-02-07 12:32:26.000000 sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/__init__.py
--rw-r--r--   0 tkomiya    (502) staff       (20)     8282 2020-08-09 15:06:29.000000 sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/builder.py
--rw-r--r--   0 tkomiya    (502) staff       (20)    19732 2020-06-27 13:21:48.000000 sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/core.py
--rw-r--r--   0 tkomiya    (502) staff       (20)      479 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/errors.py
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-08-09 15:34:57.811793 sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/files/
--rw-r--r--   0 tkomiya    (502) staff       (20)      673 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/files/ajax-loader.gif
--rw-r--r--   0 tkomiya    (502) staff       (20)      756 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/files/comment-bright.png
--rw-r--r--   0 tkomiya    (502) staff       (20)      829 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/files/comment-close.png
--rw-r--r--   0 tkomiya    (502) staff       (20)      641 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/files/comment.png
--rw-r--r--   0 tkomiya    (502) staff       (20)      222 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/files/down-pressed.png
--rw-r--r--   0 tkomiya    (502) staff       (20)      202 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/files/down.png
--rw-r--r--   0 tkomiya    (502) staff       (20)      214 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/files/up-pressed.png
--rw-r--r--   0 tkomiya    (502) staff       (20)      203 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/files/up.png
--rw-r--r--   0 tkomiya    (502) staff       (20)    25355 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/files/websupport.js
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-08-09 15:34:57.812960 sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/search/
--rw-r--r--   0 tkomiya    (502) staff       (20)     4794 2020-01-12 16:37:27.000000 sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/search/__init__.py
--rw-r--r--   0 tkomiya    (502) staff       (20)      696 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/search/nullsearch.py
--rw-r--r--   0 tkomiya    (502) staff       (20)     2032 2020-01-12 16:37:27.000000 sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/search/whooshsearch.py
--rw-r--r--   0 tkomiya    (502) staff       (20)     2734 2020-01-12 16:37:27.000000 sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/search/xapiansearch.py
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-08-09 15:34:57.814152 sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/storage/
--rw-r--r--   0 tkomiya    (502) staff       (20)     4356 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/storage/__init__.py
--rw-r--r--   0 tkomiya    (502) staff       (20)     2585 2020-04-29 07:55:19.000000 sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/storage/differ.py
--rw-r--r--   0 tkomiya    (502) staff       (20)     7643 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/storage/sqlalchemy_db.py
--rw-r--r--   0 tkomiya    (502) staff       (20)     6161 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/storage/sqlalchemystorage.py
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-08-09 15:34:57.814426 sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/templates/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1186 2020-02-07 12:32:26.000000 sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/templates/searchresults.html
--rw-r--r--   0 tkomiya    (502) staff       (20)      474 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/utils.py
--rw-r--r--   0 tkomiya    (502) staff       (20)      301 2020-08-09 15:06:45.000000 sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/version.py
--rw-r--r--   0 tkomiya    (502) staff       (20)     1668 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/writer.py
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-08-09 15:34:57.816860 sphinxcontrib-websupport-1.2.4/sphinxcontrib_websupport.egg-info/
--rw-r--r--   0 tkomiya    (502) staff       (20)     1333 2020-08-09 15:34:57.000000 sphinxcontrib-websupport-1.2.4/sphinxcontrib_websupport.egg-info/PKG-INFO
--rw-r--r--   0 tkomiya    (502) staff       (20)     3145 2020-08-09 15:34:57.000000 sphinxcontrib-websupport-1.2.4/sphinxcontrib_websupport.egg-info/SOURCES.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)        1 2020-08-09 15:34:57.000000 sphinxcontrib-websupport-1.2.4/sphinxcontrib_websupport.egg-info/dependency_links.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)       83 2020-08-09 15:34:57.000000 sphinxcontrib-websupport-1.2.4/sphinxcontrib_websupport.egg-info/entry_points.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)       14 2020-08-09 15:34:57.000000 sphinxcontrib-websupport-1.2.4/sphinxcontrib_websupport.egg-info/namespace_packages.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)        1 2020-01-12 16:45:25.000000 sphinxcontrib-websupport-1.2.4/sphinxcontrib_websupport.egg-info/not-zip-safe
--rw-r--r--   0 tkomiya    (502) staff       (20)       85 2020-08-09 15:34:57.000000 sphinxcontrib-websupport-1.2.4/sphinxcontrib_websupport.egg-info/requires.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)       14 2020-08-09 15:34:57.000000 sphinxcontrib-websupport-1.2.4/sphinxcontrib_websupport.egg-info/top_level.txt
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-08-09 15:34:57.817669 sphinxcontrib-websupport-1.2.4/tests/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-08-09 15:34:57.831979 sphinxcontrib-websupport-1.2.4/tests/root/
--rw-r--r--   0 tkomiya    (502) staff       (20)     2111 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/Makefile
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-08-09 15:34:57.832486 sphinxcontrib-websupport-1.2.4/tests/root/_static/
--rw-r--r--   0 tkomiya    (502) staff       (20)       56 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/_static/README
--rw-r--r--   0 tkomiya    (502) staff       (20)       58 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/_static/excluded.css
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-08-09 15:34:57.833017 sphinxcontrib-websupport-1.2.4/tests/root/_static/subdir/
--rw-r--r--   0 tkomiya    (502) staff       (20)       16 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/_static/subdir/foo.css
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-08-09 15:34:57.833786 sphinxcontrib-websupport-1.2.4/tests/root/_templates/
--rw-r--r--   0 tkomiya    (502) staff       (20)       67 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/_templates/contentssb.html
--rw-r--r--   0 tkomiya    (502) staff       (20)       99 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/_templates/customsb.html
--rw-r--r--   0 tkomiya    (502) staff       (20)      428 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/_templates/layout.html
--rw-r--r--   0 tkomiya    (502) staff       (20)      160 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/autodoc_fodder.py
--rw-r--r--   0 tkomiya    (502) staff       (20)      479 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/autodoc_missing_imports.py
--rw-r--r--   0 tkomiya    (502) staff       (20)      264 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/bom.po
--rw-r--r--   0 tkomiya    (502) staff       (20)       74 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/bom.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)     3041 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/conf.py
--rw-r--r--   0 tkomiya    (502) staff       (20)     1157 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/contents.txt
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-08-09 15:34:57.834127 sphinxcontrib-websupport-1.2.4/tests/root/en.lproj/
--rw-r--r--   0 tkomiya    (502) staff       (20)      115 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/en.lproj/localized.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)       95 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/ext.py
--rw-r--r--   0 tkomiya    (502) staff       (20)       87 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/extapi.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)      365 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/extensions.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)      770 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/footnote.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)      640 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/images.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)    66247 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/img.foo.png
--rw-r--r--   0 tkomiya    (502) staff       (20)    24976 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/img.gif
--rw-r--r--   0 tkomiya    (502) staff       (20)   141783 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/img.pdf
--rw-r--r--   0 tkomiya    (502) staff       (20)    66247 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/img.png
--rw-r--r--   0 tkomiya    (502) staff       (20)     2076 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/includes.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)      636 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/lists.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)      200 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/literal.inc
--rw-r--r--   0 tkomiya    (502) staff       (20)      232 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/literal_orig.inc
--rw-r--r--   0 tkomiya    (502) staff       (20)     6431 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/markup.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)      373 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/math.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)     1782 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/metadata.add
--rw-r--r--   0 tkomiya    (502) staff       (20)     3718 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/objects.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)      320 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/parsermod.py
--rw-r--r--   0 tkomiya    (502) staff       (20)       45 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/quotes.inc
--rw-r--r--   0 tkomiya    (502) staff       (20)      120 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/rimg.png
--rw-r--r--   0 tkomiya    (502) staff       (20)       34 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/robots.txt
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-08-09 15:34:57.834837 sphinxcontrib-websupport-1.2.4/tests/root/special/
--rw-r--r--   0 tkomiya    (502) staff       (20)       40 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/special/api.h
--rw-r--r--   0 tkomiya    (502) staff       (20)       32 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/special/code.py
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-08-09 15:34:57.836768 sphinxcontrib-websupport-1.2.4/tests/root/subdir/
--rw-r--r--   0 tkomiya    (502) staff       (20)       96 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/subdir/excluded.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)      106 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/subdir/images.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)    66247 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/subdir/img.png
--rw-r--r--   0 tkomiya    (502) staff       (20)      144 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/subdir/include.inc
--rw-r--r--   0 tkomiya    (502) staff       (20)      328 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/subdir/includes.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)    66247 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/subdir/simg.png
--rw-r--r--   0 tkomiya    (502) staff       (20)      180 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/subdir.po
--rw-r--r--   0 tkomiya    (502) staff       (20)   141783 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/svgimg.pdf
--rw-r--r--   0 tkomiya    (502) staff       (20)     7420 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/svgimg.svg
--rw-r--r--   0 tkomiya    (502) staff       (20)       78 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/tabs.inc
--rw-r--r--   0 tkomiya    (502) staff       (20)       48 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/templated.css_t
--rw-r--r--   0 tkomiya    (502) staff       (20)       77 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/test.inc
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-08-09 15:34:57.837399 sphinxcontrib-websupport-1.2.4/tests/root/testtheme/
--rw-r--r--   0 tkomiya    (502) staff       (20)      139 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/testtheme/layout.html
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-08-09 15:34:57.838113 sphinxcontrib-websupport-1.2.4/tests/root/testtheme/static/
--rw-r--r--   0 tkomiya    (502) staff       (20)      120 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/testtheme/static/staticimg.png
--rw-r--r--   0 tkomiya    (502) staff       (20)       82 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/testtheme/static/statictmpl.html_t
--rw-r--r--   0 tkomiya    (502) staff       (20)      104 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/testtheme/theme.conf
--rw-r--r--   0 tkomiya    (502) staff       (20)      107 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/wrongenc.inc
--rw-r--r--   0 tkomiya    (502) staff       (20)     1039 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/root/ziptheme.zip
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-08-09 15:34:57.802441 sphinxcontrib-websupport-1.2.4/tests/roots/
-drwxr-xr-x   0 tkomiya    (502) staff       (20)        0 2020-08-09 15:34:57.840508 sphinxcontrib-websupport-1.2.4/tests/roots/test-searchadapters/
--rw-r--r--   0 tkomiya    (502) staff       (20)       70 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/roots/test-searchadapters/conf.py
--rw-r--r--   0 tkomiya    (502) staff       (20)     6614 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/roots/test-searchadapters/markup.txt
--rw-r--r--   0 tkomiya    (502) staff       (20)     2331 2020-01-12 15:30:32.000000 sphinxcontrib-websupport-1.2.4/tests/test_searchadapters.py
--rw-r--r--   0 tkomiya    (502) staff       (20)     9659 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/test_websupport.py
--rw-r--r--   0 tkomiya    (502) staff       (20)      898 2020-01-12 15:12:28.000000 sphinxcontrib-websupport-1.2.4/tests/util.py
--rw-r--r--   0 tkomiya    (502) staff       (20)      508 2020-01-12 17:07:55.000000 sphinxcontrib-websupport-1.2.4/tox.ini
+-rw-r--r--   0        0        0     1411 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/CHANGES
+-rw-r--r--   0        0        0     1443 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/LICENSE
+-rw-r--r--   0        0        0      402 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/README.rst
+-rw-r--r--   0        0        0     2410 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/pyproject.toml
+-rw-r--r--   0        0        0      319 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/__init__.py
+-rw-r--r--   0        0        0     7886 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/builder.py
+-rw-r--r--   0        0        0    19474 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/core.py
+-rw-r--r--   0        0        0      262 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/errors.py
+-rw-r--r--   0        0        0      673 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/files/ajax-loader.gif
+-rw-r--r--   0        0        0      756 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/files/comment-bright.png
+-rw-r--r--   0        0        0      829 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/files/comment-close.png
+-rw-r--r--   0        0        0      641 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/files/comment.png
+-rw-r--r--   0        0        0      222 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/files/down-pressed.png
+-rw-r--r--   0        0        0      202 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/files/down.png
+-rw-r--r--   0        0        0      214 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/files/up-pressed.png
+-rw-r--r--   0        0        0      203 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/files/up.png
+-rw-r--r--   0        0        0    25355 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/files/websupport.js
+-rw-r--r--   0        0        0     4577 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/search/__init__.py
+-rw-r--r--   0        0        0      457 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/search/nullsearch.py
+-rw-r--r--   0        0        0     1789 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/search/whooshsearch.py
+-rw-r--r--   0        0        0     2491 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/search/xapiansearch.py
+-rw-r--r--   0        0        0     4137 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/storage/__init__.py
+-rw-r--r--   0        0        0     2353 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/storage/differ.py
+-rw-r--r--   0        0        0     7346 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/storage/sqlalchemy_db.py
+-rw-r--r--   0        0        0     5906 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/storage/sqlalchemystorage.py
+-rw-r--r--   0        0        0     1021 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/templates/searchresults.html
+-rw-r--r--   0        0        0      288 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/utils.py
+-rw-r--r--   0        0        0     1461 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/writer.py
+-rw-r--r--   0        0        0      187 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/tests/conftest.py
+-rw-r--r--   0        0        0     2111 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/Makefile
+-rw-r--r--   0        0        0       56 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/_static/README
+-rw-r--r--   0        0        0       58 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/_static/excluded.css
+-rw-r--r--   0        0        0       16 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/_static/subdir/foo.css
+-rw-r--r--   0        0        0       67 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/_templates/contentssb.html
+-rw-r--r--   0        0        0       99 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/_templates/customsb.html
+-rw-r--r--   0        0        0      428 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/_templates/layout.html
+-rw-r--r--   0        0        0      160 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/autodoc_fodder.py
+-rw-r--r--   0        0        0      479 2023-08-08 18:58:56.745300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/autodoc_missing_imports.py
+-rw-r--r--   0        0        0      264 2023-08-08 18:58:56.749300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/bom.po
+-rw-r--r--   0        0        0       74 2023-08-08 18:58:56.749300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/bom.txt
+-rw-r--r--   0        0        0     3016 2023-08-08 18:58:56.749300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/conf.py
+-rw-r--r--   0        0        0     1157 2023-08-08 18:58:56.749300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/contents.txt
+-rw-r--r--   0        0        0      115 2023-08-08 18:58:56.749300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/en.lproj/localized.txt
+-rw-r--r--   0        0        0       95 2023-08-08 18:58:56.749300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/ext.py
+-rw-r--r--   0        0        0       87 2023-08-08 18:58:56.749300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/extapi.txt
+-rw-r--r--   0        0        0      365 2023-08-08 18:58:56.749300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/extensions.txt
+-rw-r--r--   0        0        0      770 2023-08-08 18:58:56.749300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/footnote.txt
+-rw-r--r--   0        0        0      640 2023-08-08 18:58:56.749300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/images.txt
+-rw-r--r--   0        0        0    66247 2023-08-08 18:58:56.749300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/img.foo.png
+-rw-r--r--   0        0        0    24976 2023-08-08 18:58:56.749300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/img.gif
+-rw-r--r--   0        0        0   141783 2023-08-08 18:58:56.749300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/img.pdf
+-rw-r--r--   0        0        0    66247 2023-08-08 18:58:56.749300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/img.png
+-rw-r--r--   0        0        0     2076 2023-08-08 18:58:56.749300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/includes.txt
+-rw-r--r--   0        0        0      636 2023-08-08 18:58:56.749300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/lists.txt
+-rw-r--r--   0        0        0      200 2023-08-08 18:58:56.749300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/literal.inc
+-rw-r--r--   0        0        0      232 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/literal_orig.inc
+-rw-r--r--   0        0        0     6431 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/markup.txt
+-rw-r--r--   0        0        0      373 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/math.txt
+-rw-r--r--   0        0        0     1782 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/metadata.add
+-rw-r--r--   0        0        0     3718 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/objects.txt
+-rw-r--r--   0        0        0      320 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/parsermod.py
+-rw-r--r--   0        0        0       45 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/quotes.inc
+-rw-r--r--   0        0        0      120 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/rimg.png
+-rw-r--r--   0        0        0       34 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/robots.txt
+-rw-r--r--   0        0        0       40 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/special/api.h
+-rw-r--r--   0        0        0       32 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/special/code.py
+-rw-r--r--   0        0        0      180 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/subdir.po
+-rw-r--r--   0        0        0       96 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/subdir/excluded.txt
+-rw-r--r--   0        0        0      106 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/subdir/images.txt
+-rw-r--r--   0        0        0    66247 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/subdir/img.png
+-rw-r--r--   0        0        0      144 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/subdir/include.inc
+-rw-r--r--   0        0        0      328 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/subdir/includes.txt
+-rw-r--r--   0        0        0    66247 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/subdir/simg.png
+-rw-r--r--   0        0        0   141783 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/svgimg.pdf
+-rw-r--r--   0        0        0     7420 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/svgimg.svg
+-rw-r--r--   0        0        0       78 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/tabs.inc
+-rw-r--r--   0        0        0       48 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/templated.css_t
+-rw-r--r--   0        0        0       77 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/test.inc
+-rw-r--r--   0        0        0      139 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/testtheme/layout.html
+-rw-r--r--   0        0        0      120 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/testtheme/static/staticimg.png
+-rw-r--r--   0        0        0       82 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/testtheme/static/statictmpl.html_t
+-rw-r--r--   0        0        0      104 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/testtheme/theme.conf
+-rw-r--r--   0        0        0      107 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/wrongenc.inc
+-rw-r--r--   0        0        0     1039 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/ziptheme.zip
+-rw-r--r--   0        0        0       45 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tests/roots/test-searchadapters/conf.py
+-rw-r--r--   0        0        0     6614 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tests/roots/test-searchadapters/markup.txt
+-rw-r--r--   0        0        0     2139 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tests/test_searchadapters.py
+-rw-r--r--   0        0        0     9234 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tests/test_websupport.py
+-rw-r--r--   0        0        0      393 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tests/util.py
+-rw-r--r--   0        0        0      642 2023-08-08 18:58:56.753300 sphinxcontrib_websupport-1.2.5/tox.ini
+-rw-r--r--   0        0        0     2458 1970-01-01 00:00:00.000000 sphinxcontrib_websupport-1.2.5/PKG-INFO
```

### Comparing `sphinxcontrib-websupport-1.2.4/CHANGES` & `sphinxcontrib_websupport-1.2.5/CHANGES`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Release 1.2.5 (2023-08-07)
+==========================
+
+* Drop support for Python 3.5, 3.6, 3.7, and 3.8
+* Raise minimum required Sphinx version to 5.0
+
 Release 1.2.4 (2020-08-09)
 ==========================
 
 * Import PickleHTMLBuilder from sphinxcontrib-serializinghtml package
 
 Release 1.2.3 (2020-06-27)
 ==========================
```

### Comparing `sphinxcontrib-websupport-1.2.4/LICENSE` & `sphinxcontrib_websupport-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-websupport-1.2.4/setup.py` & `sphinxcontrib_websupport-1.2.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,82 +1,90 @@
-# -*- coding: utf-8 -*-
-import os
-from setuptools import setup, find_packages
-
-long_desc = '''
-sphinxcontrib-websupport provides a Python API to easily integrate Sphinx
-documentation into your Web application.
-'''
-
-extras_require = {
-    # Environment Marker works for wheel 0.24 or later
-    'test': [
-        'pytest',
-        'sqlalchemy',
-        'whoosh',
-        'Sphinx',
-    ],
-    'lint': [
-        'flake8',
-    ],
-}
-
-
-def get_version():
-    """Get version number of the package from version.py without importing core module."""
-    package_dir = os.path.abspath(os.path.dirname(__file__))
-    version_file = os.path.join(package_dir, 'sphinxcontrib/websupport/version.py')
-
-    namespace = {}
-    with open(version_file, 'rt') as f:
-        exec(f.read(), namespace)
-
-    return namespace['__version__']
-
-
-setup(
-    name='sphinxcontrib-websupport',
-    version=get_version(),
-    url='http://sphinx-doc.org/',
-    download_url='https://pypi.org/project/sphinxcontrib-websupport/',
-    license='BSD',
-    author='Georg Brandl',
-    author_email='georg@python.org',
-    description='Sphinx API for Web Apps',
-    long_description=long_desc,
-    zip_safe=False,
-    classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Environment :: Console',
-        'Environment :: Web Environment',
-        'Intended Audience :: Developers',
-        'Intended Audience :: Education',
-        'License :: OSI Approved :: BSD License',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Framework :: Sphinx',
-        'Framework :: Sphinx :: Extension',
-        'Topic :: Documentation',
-        'Topic :: Documentation :: Sphinx',
-        'Topic :: Text Processing',
-        'Topic :: Utilities',
-    ],
-    platforms='any',
-    python_requires=">=3.5",
-    packages=find_packages(exclude=['tests']),
-    include_package_data=True,
-    install_requires=[
-        'sphinxcontrib-serializinghtml',
-    ],
-    extras_require=extras_require,
-    entry_points={
-        'sphinx.builders': [
-            'websupport = sphinxcontrib.websupport.builder:WebSupportBuilder',
-        ],
-    },
-    namespace_packages=['sphinxcontrib'],
-)
+[build-system]
+requires = ["flit_core>=3.7"]
+build-backend = "flit_core.buildapi"
+
+# project metadata
+[project]
+name = "sphinxcontrib-websupport"
+description = """sphinxcontrib-websupport provides a Python API to easily \
+integrate Sphinx documentation into your Web application"""
+readme = "README.rst"
+urls.Changelog = "https://www.sphinx-doc.org/en/master/changes.html"
+urls.Code = "https://github.com/sphinx-doc/sphinxcontrib-websupport"
+urls.Download = "https://pypi.org/project/sphinxcontrib-websupport/"
+urls.Homepage = "https://www.sphinx-doc.org/"
+urls."Issue tracker" = "https://github.com/sphinx-doc/sphinx/issues"
+license.text = "BSD-2-Clause"
+requires-python = ">=3.9"
+
+# Classifiers list: https://pypi.org/classifiers/
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Environment :: Console",
+    "Environment :: Web Environment",
+    "Intended Audience :: Developers",
+    "Intended Audience :: Education",
+    "License :: OSI Approved :: BSD License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3.13",
+    "Framework :: Sphinx",
+    "Framework :: Sphinx :: Extension",
+    "Topic :: Documentation",
+    "Topic :: Documentation :: Sphinx",
+    "Topic :: Text Processing",
+    "Topic :: Utilities",
+]
+dependencies = [
+    "jinja2",
+    "Sphinx>=5",
+    "sphinxcontrib-serializinghtml",
+]
+dynamic = ["version"]
+
+[project.optional-dependencies]
+test = [
+    "pytest",
+    "sqlalchemy",
+    "whoosh",
+    # greenlet is required by sqlalchemy; 3.12 only supported in 3.0.0a1+
+    "greenlet>=3.0.0a1; python_version >= '3.12'",
+]
+lint = [
+    "flake8",
+    "mypy",
+    "docutils-stubs",
+]
+
+[[project.authors]]
+name = "Georg Brandl"
+email = "georg@python.org"
+
+[project.entry-points]
+"sphinx.builders".websupport = "sphinxcontrib.websupport.builder:WebSupportBuilder"
+
+
+[tool.flit.module]
+name = "sphinxcontrib.websupport"
+
+[tool.flit.sdist]
+include = [
+    "CHANGES",
+    "LICENSE",
+    # Tests
+    "tests/",
+    "tox.ini",
+]
+
+[tool.mypy]
+ignore_missing_imports = true
+
+[tool.pytest.ini_options]
+markers = [
+    "support",
+]
```

### Comparing `sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/builder.py` & `sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/builder.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,32 @@
-# -*- coding: utf-8 -*-
-"""
-    sphinx.builders.websupport
-    ~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-    Builder for the web support package.
-
-    :copyright: Copyright 2007-2016 by the Sphinx team, see AUTHORS.
-    :license: BSD, see LICENSE for details.
-"""
+"""Builder for the web support extension."""
+
+from __future__ import annotations
 
 from os import path
 import posixpath
 import shutil
+from typing import TYPE_CHECKING, Any
 
 from docutils.io import StringOutput
 
-from sphinx import version_info as sphinx_version
 from sphinx.jinja2glue import BuiltinTemplateLoader
 from sphinx.util.osutil import os_path, relative_uri, ensuredir, copyfile
 from sphinxcontrib.serializinghtml import PickleHTMLBuilder
 
-from . import package_dir
-from .writer import WebSupportTranslator
-from .utils import is_commentable
+from sphinxcontrib.websupport import package_dir
+from sphinxcontrib.websupport.writer import WebSupportTranslator
+from sphinxcontrib.websupport.utils import is_commentable
+
 
+if TYPE_CHECKING:
+    from collections.abc import Iterable
 
-if False:
-    # For type annotation
-    from typing import Any, Dict, Iterable, Tuple  # NOQA
-    from docutils import nodes  # NOQA
-    from sphinx.application import Sphinx  # NOQA
+    from docutils import nodes
+    from sphinx.application import Sphinx
 
 RESOURCES = [
     'ajax-loader.gif',
     'comment-bright.png',
     'comment-close.png',
     'comment.png',
     'down-pressed.png',
@@ -48,47 +41,46 @@
     """
     Builds documents for the web support package.
     """
     name = 'websupport'
     default_translator_class = WebSupportTranslator
     versioning_compare = True  # for commentable node's uuid stability.
 
-    def init(self):
-        # type: () -> None
+    def init(self) -> None:
         PickleHTMLBuilder.init(self)
         # templates are needed for this builder, but the serializing
         # builder does not initialize them
         self.init_templates()
         if not isinstance(self.templates, BuiltinTemplateLoader):
             raise RuntimeError('websupport builder must be used with '
                                'the builtin templates')
         # add our custom JS
         self.script_files.append('_static/websupport.js')
 
     @property
     def versioning_method(self):
-        if sphinx_version < (2, 0):
-            return 'commentable'
-        else:
-            return is_commentable
+        return is_commentable
 
-    def set_webinfo(self, staticdir, virtual_staticdir, search, storage):
-        # type: (str, str, Any, str) -> None
+    def set_webinfo(
+        self,
+        staticdir: str,
+        virtual_staticdir: str,
+        search: Any,
+        storage: str,
+    ) -> None:
         self.staticdir = staticdir
         self.virtual_staticdir = virtual_staticdir
         self.search = search
         self.storage = storage
 
-    def prepare_writing(self, docnames):
-        # type: (Iterable[str]) -> None
+    def prepare_writing(self, docnames: Iterable[str]) -> None:
         PickleHTMLBuilder.prepare_writing(self, docnames)
         self.globalcontext['no_search_suffix'] = True
 
-    def write_doc(self, docname, doctree):
-        # type: (str, nodes.Node) -> None
+    def write_doc(self, docname: str, doctree: nodes.document) -> None:
         destination = StringOutput(encoding='utf-8')
         doctree.settings = self.docsettings
 
         self.secnumbers = self.env.toc_secnumbers.get(docname, {})
         self.fignumbers = self.env.toc_fignumbers.get(docname, {})
         self.imgpath = '/' + posixpath.join(self.virtual_staticdir, self.imagedir)
         self.dlpath = '/' + posixpath.join(self.virtual_staticdir, '_downloads')
@@ -97,38 +89,40 @@
         self.docwriter.assemble_parts()
         body = self.docwriter.parts['fragment']
         metatags = self.docwriter.clean_meta
 
         ctx = self.get_doc_context(docname, body, metatags)
         self.handle_page(docname, ctx, event_arg=doctree)
 
-    def write_doc_serialized(self, docname, doctree):
-        # type: (str, nodes.Node) -> None
+    def write_doc_serialized(self, docname: str, doctree: nodes.Node) -> None:
         self.imgpath = '/' + posixpath.join(self.virtual_staticdir, self.imagedir)
         self.post_process_images(doctree)
         title = self.env.longtitles.get(docname)
         title = title and self.render_partial(title)['title'] or ''
         self.index_page(docname, doctree, title)
 
-    def load_indexer(self, docnames):
-        # type: (Iterable[str]) -> None
+    def load_indexer(self, docnames: Iterable[str]) -> None:
         self.indexer = self.search  # type: ignore
         self.indexer.init_indexing(changed=docnames)  # type: ignore
 
-    def _render_page(self, pagename, addctx, templatename, event_arg=None):
-        # type: (str, Dict, str, str) -> Tuple[Dict, Dict]
+    def _render_page(
+        self,
+        pagename: str,
+        addctx: dict,
+        templatename: str,
+        event_arg: Any = None,
+    ) -> tuple[dict, dict]:
         # This is mostly copied from StandaloneHTMLBuilder. However, instead
         # of rendering the template and saving the html, create a context
         # dict and pickle it.
         ctx = self.globalcontext.copy()
         ctx['pagename'] = pagename
 
-        def pathto(otheruri, resource=False,
-                   baseuri=self.get_target_uri(pagename)):
-            # type: (str, bool, str) -> str
+        def pathto(otheruri: str, resource: bool = False,
+                   baseuri: str = self.get_target_uri(pagename)) -> str:
             if resource and '://' in otheruri:
                 return otheruri
             elif not resource:
                 otheruri = self.get_target_uri(otheruri)
                 return relative_uri(baseuri, otheruri) or '#'
             else:
                 return '/' + posixpath.join(self.virtual_staticdir, otheruri)
@@ -156,17 +150,16 @@
         template_module = template.make_module(ctx)
         for item in ['sidebar', 'relbar', 'script', 'css']:
             if hasattr(template_module, item):
                 doc_ctx[item] = getattr(template_module, item)()
 
         return ctx, doc_ctx
 
-    def handle_page(self, pagename, addctx, templatename='page.html',
-                    outfilename=None, event_arg=None):
-        # type: (str, Dict, str, str, str) -> None
+    def handle_page(self, pagename: str, addctx: dict, templatename: str = 'page.html',
+                    outfilename: str | None = None, event_arg: Any = None) -> None:
         ctx, doc_ctx = self._render_page(pagename, addctx,
                                          templatename, event_arg)
 
         if not outfilename:
             outfilename = path.join(self.outdir, 'pickles',
                                     os_path(pagename) + self.out_suffix)
         ensuredir(path.dirname(outfilename))
@@ -176,16 +169,15 @@
         # "show source" link
         if ctx.get('sourcename'):
             source_name = path.join(self.staticdir,
                                     '_sources', os_path(ctx['sourcename']))
             ensuredir(path.dirname(source_name))
             copyfile(self.env.doc2path(pagename), source_name)
 
-    def handle_finish(self):
-        # type: () -> None
+    def handle_finish(self) -> None:
         # get global values for css and script files
         _, doc_ctx = self._render_page('tmp', {}, 'page.html')
         self.globalcontext['css'] = doc_ctx['css']
         self.globalcontext['script'] = doc_ctx['script']
 
         PickleHTMLBuilder.handle_finish(self)
 
@@ -196,32 +188,28 @@
             dst = path.join(self.staticdir, directory)
             if path.isdir(src):
                 if path.isdir(dst):
                     shutil.rmtree(dst)
                 shutil.move(src, dst)
         self.copy_resources()
 
-    def copy_resources(self):
-        # type: () -> None
+    def copy_resources(self) -> None:
         # copy resource files to static dir
         dst = path.join(self.staticdir, '_static')
 
         if path.isdir(dst):
             for resource in RESOURCES:
                 src = path.join(package_dir, 'files', resource)
                 shutil.copy(src, dst)
 
-    def dump_search_index(self):
-        # type: () -> None
+    def dump_search_index(self) -> None:
         self.indexer.finish_indexing()  # type: ignore
 
 
-def setup(app):
-    # type: (Sphinx) -> Dict[str, Any]
-    if sphinx_version >= (2, 0):
-        app.add_builder(WebSupportBuilder)
+def setup(app: Sphinx) -> dict[str, Any]:
+    app.add_builder(WebSupportBuilder)
 
     return {
         'version': 'builtin',
         'parallel_read_safe': True,
         'parallel_write_safe': True,
     }
```

### Comparing `sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/core.py` & `sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,10 @@
-# -*- coding: utf-8 -*-
-"""
-    sphinxcontrib.websupport.core
-    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-    Base Module for web support functions.
-
-    :copyright: Copyright 2007-2016 by the Sphinx team, see AUTHORS.
-    :license: BSD, see LICENSE for details.
-"""
+"""Base Module for web support functions."""
+
+from __future__ import annotations
 
 import html
 import sys
 import pickle
 import posixpath
 from os import path
 
@@ -27,18 +20,14 @@
 from sphinxcontrib.websupport.storage import StorageBackend
 
 try:
     from sphinxcontrib.serializinghtml.jsonimpl import dumps as dump_json
 except ImportError:
     from sphinx.util.jsonimpl import dumps as dump_json
 
-if False:
-    # For type annotation
-    from typing import Dict  # NOQA
-
 
 class WebSupport(object):
     """The main API class for the web support package. All interactions
     with the web support package should occur through this class.
     """
     def __init__(self,
                  srcdir=None,      # only required for building
@@ -398,15 +387,15 @@
         self.storage.accept_comment(comment_id)
 
     def _make_base_comment_options(self):
         """Helper method to create the part of the COMMENT_OPTIONS javascript
         that remains the same throughout the lifetime of the
         :class:`~sphinxcontrib.websupport.WebSupport` object.
         """
-        self.base_comment_opts = {}  # type: Dict[str, str]
+        self.base_comment_opts: dict[str, str] = {}
 
         if self.docroot != '':
             comment_urls = [
                 ('addCommentURL', '_add_comment'),
                 ('getCommentsURL', '_get_comments'),
                 ('processVoteURL', '_process_vote'),
                 ('acceptCommentURL', '_accept_comment'),
```

### Comparing `sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/files/ajax-loader.gif` & `sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/files/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/files/comment-bright.png` & `sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/files/comment-bright.png`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/files/comment-close.png` & `sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/files/comment-close.png`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/files/comment.png` & `sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/files/comment.png`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/files/websupport.js` & `sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/files/websupport.js`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/search/__init__.py` & `sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/search/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,8 @@
-# -*- coding: utf-8 -*-
-"""
-    sphinxcontrib.websupport.search
-    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-    Server side search support for the web support package.
-
-    :copyright: Copyright 2007-2016 by the Sphinx team, see AUTHORS.
-    :license: BSD, see LICENSE for details.
-"""
+"""Server side search support for the web support package."""
 
 import re
 
 
 class BaseSearch(object):
     def __init__(self, path):
         pass
```

### Comparing `sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/search/whooshsearch.py` & `sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/search/whooshsearch.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,8 @@
-# -*- coding: utf-8 -*-
-"""
-    sphinxcontrib.websupport.search.whooshsearch
-    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-    Whoosh search adapter.
-
-    :copyright: Copyright 2007-2016 by the Sphinx team, see AUTHORS.
-    :license: BSD, see LICENSE for details.
-"""
+"""Whoosh search adapter."""
 
 from whoosh import index
 from whoosh.fields import Schema, ID, TEXT
 from whoosh.qparser import QueryParser
 from whoosh.analysis import StemmingAnalyzer
 
 from sphinx.util.osutil import ensuredir
```

### Comparing `sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/search/xapiansearch.py` & `sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/search/xapiansearch.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,8 @@
-# -*- coding: utf-8 -*-
-"""
-    sphinxcontrib.websupport.search.xapiansearch
-    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-    Xapian search adapter.
-
-    :copyright: Copyright 2007-2016 by the Sphinx team, see AUTHORS.
-    :license: BSD, see LICENSE for details.
-"""
+"""Xapian search adapter."""
 
 import xapian
 
 from sphinx.util.osutil import ensuredir
 from sphinxcontrib.websupport.search import BaseSearch
```

### Comparing `sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/storage/__init__.py` & `sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/storage/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,8 @@
-# -*- coding: utf-8 -*-
-"""
-    sphinxcontrib.websupport.storage
-    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-    Storage for the websupport package.
-
-    :copyright: Copyright 2007-2016 by the Sphinx team, see AUTHORS.
-    :license: BSD, see LICENSE for details.
-"""
+"""Storage for the websupport package."""
 
 
 class StorageBackend(object):
     def pre_build(self):
         """Called immediately before the build process begins. Use this
         to prepare the StorageBackend for the addition of nodes.
         """
```

### Comparing `sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/storage/differ.py` & `sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/storage/differ.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,8 @@
-# -*- coding: utf-8 -*-
-"""
-    sphinxcontrib.websupport.storage.differ
-    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-    A differ for creating an HTML representations of proposal diffs
-
-    :copyright: Copyright 2007-2016 by the Sphinx team, see AUTHORS.
-    :license: BSD, see LICENSE for details.
-"""
+"""A differ for creating an HTML representations of proposal diffs."""
 
 import html
 import re
 from difflib import Differ
 
 
 class CombinedHtmlDiff(object):
```

### Comparing `sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/storage/sqlalchemy_db.py` & `sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/storage/sqlalchemy_db.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,21 @@
-# -*- coding: utf-8 -*-
 """
-    sphinxcontrib.websupport.storage.sqlalchemy_db
-    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-    SQLAlchemy table and mapper definitions used by the
-    :class:`sphinxcontrib.websupport.storage.sqlalchemystorage.SQLAlchemyStorage`.
-
-    :copyright: Copyright 2007-2016 by the Sphinx team, see AUTHORS.
-    :license: BSD, see LICENSE for details.
+SQLAlchemy table and mapper definitions used by the
+:py:class:`sphinxcontrib.websupport.storage.sqlalchemystorage.SQLAlchemyStorage`.
 """
 
+from __future__ import annotations
+
 from datetime import datetime
 
 from sqlalchemy import Column, Integer, Text, String, Boolean, \
     ForeignKey, DateTime
 from sqlalchemy.orm import relation, sessionmaker, aliased
 from sqlalchemy.ext.declarative import declarative_base
 
-if False:
-    # For type annotation
-    from typing import List  # NOQA
-
 Base = declarative_base()
 Session = sessionmaker()
 
 db_prefix = 'sphinx_'
 
 
 class Node(Base):  # type: ignore
@@ -74,15 +65,15 @@
     def _nest_comments(self, results, username):
         """Given the flat list of results, convert the list into a
         tree.
 
         :param results: the flat list of comments
         :param username: the name of the user requesting the comments.
         """
-        comments = []  # type: List
+        comments = []
         list_stack = [comments]
         for r in results:
             if username:
                 comment, vote = r
             else:
                 comment, vote = (r, 0)
```

### Comparing `sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/storage/sqlalchemystorage.py` & `sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/storage/sqlalchemystorage.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,8 @@
-# -*- coding: utf-8 -*-
-"""
-    sphinxcontrib.websupport.storage.sqlalchemystorage
-    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-    An SQLAlchemy storage backend.
-
-    :copyright: Copyright 2007-2016 by the Sphinx team, see AUTHORS.
-    :license: BSD, see LICENSE for details.
-"""
+"""An SQLAlchemy storage backend."""
 
 from datetime import datetime
 
 import sqlalchemy
 from sqlalchemy.orm import aliased
 from sqlalchemy.sql import func
```

### Comparing `sphinxcontrib-websupport-1.2.4/sphinxcontrib/websupport/writer.py` & `sphinxcontrib_websupport-1.2.5/sphinxcontrib/websupport/writer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,12 @@
-# -*- coding: utf-8 -*-
-"""
-    sphinxcontrib.websupport.writer
-    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-    sphinxcontrib.websupport writer that adds comment-related annotations.
-
-    :copyright: Copyright 2007-2016 by the Sphinx team, see AUTHORS.
-    :license: BSD, see LICENSE for details.
-"""
+"""websupport writer that adds comment-related annotations."""
 
 from sphinx.writers.html import HTMLTranslator
 
-from .utils import is_commentable
+from sphinxcontrib.websupport.utils import is_commentable
 
 
 class WebSupportTranslator(HTMLTranslator):
     """
     Our custom HTML translator.
     """
```

### Comparing `sphinxcontrib-websupport-1.2.4/tests/root/Makefile` & `sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/Makefile`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-websupport-1.2.4/tests/root/conf.py` & `sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 import sys, os
 
 sys.path.append(os.path.abspath('.'))
 
 extensions = ['sphinx.ext.autodoc', 'sphinx.ext.jsmath', 'sphinx.ext.todo',
               'sphinx.ext.coverage', 'sphinx.ext.extlinks', 'ext']
```

### Comparing `sphinxcontrib-websupport-1.2.4/tests/root/contents.txt` & `sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/contents.txt`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-websupport-1.2.4/tests/root/footnote.txt` & `sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/footnote.txt`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-websupport-1.2.4/tests/root/images.txt` & `sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/images.txt`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-websupport-1.2.4/tests/root/img.foo.png` & `sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/img.foo.png`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-websupport-1.2.4/tests/root/img.gif` & `sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/img.gif`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-websupport-1.2.4/tests/root/img.pdf` & `sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/img.pdf`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-websupport-1.2.4/tests/root/img.png` & `sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/img.png`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-websupport-1.2.4/tests/root/includes.txt` & `sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/includes.txt`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-websupport-1.2.4/tests/root/lists.txt` & `sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/lists.txt`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-websupport-1.2.4/tests/root/markup.txt` & `sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/markup.txt`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-websupport-1.2.4/tests/root/metadata.add` & `sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/metadata.add`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-websupport-1.2.4/tests/root/objects.txt` & `sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/objects.txt`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-websupport-1.2.4/tests/root/subdir/img.png` & `sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/subdir/img.png`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-websupport-1.2.4/tests/root/subdir/simg.png` & `sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/subdir/simg.png`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-websupport-1.2.4/tests/root/svgimg.pdf` & `sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/svgimg.pdf`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-websupport-1.2.4/tests/root/svgimg.svg` & `sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/svgimg.svg`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-websupport-1.2.4/tests/root/ziptheme.zip` & `sphinxcontrib_websupport-1.2.5/tests/roots/test-root/root/ziptheme.zip`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-websupport-1.2.4/tests/roots/test-searchadapters/markup.txt` & `sphinxcontrib_websupport-1.2.5/tests/roots/test-searchadapters/markup.txt`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-websupport-1.2.4/tests/test_searchadapters.py` & `sphinxcontrib_websupport-1.2.5/tests/test_searchadapters.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,33 @@
-# -*- coding: utf-8 -*-
-"""
-    test_searchadapters
-    ~~~~~~~~~~~~~~~~~~~
-
-    Test the Web Support Package search adapters.
-
-    :copyright: Copyright 2007-2018 by the Sphinx team, see AUTHORS.
-    :license: BSD, see LICENSE for details.
-"""
+"""Test the Web Support Package search adapters."""
+
+import shutil
+from io import StringIO
 
-from six import StringIO
 import pytest
 
 from sphinxcontrib.websupport import WebSupport
 
-from test_websupport import sqlalchemy_missing
-from util import rootdir, tempdir, skip_unless_importable
+from test_websupport import skip_if_sqlalchemy_missing
+from util import skip_unless_importable
 
 
-def teardown_module():
-    (tempdir / 'websupport').rmtree(True)
+def teardown_module(tmp_path):
+    shutil.rmtree(tmp_path / 'websupport', ignore_errors=True)
 
 
-def search_adapter_helper(adapter):
-    settings = {'srcdir': rootdir / 'roots' / 'test-searchadapters',
-                'builddir': tempdir / 'websupport',
-                'status': StringIO(),
-                'warning': StringIO(),
-                'search': adapter}
-    support = WebSupport(**settings)
+@pytest.fixture
+def search_adapter_helper(rootdir, tmp_path, adapter):
+    support = WebSupport(
+        srcdir=rootdir / 'test-searchadapters',
+        builddir=tmp_path / 'websupport',
+        status=StringIO(),
+        warning=StringIO(),
+        search=adapter
+    )
     support.build()
 
     s = support.search
 
     # Test the adapters query method. A search for "Epigraph" should return
     # one result.
     results = s.query(u'Epigraph')
@@ -55,16 +50,16 @@
         '%s search adapter returned %s search result(s), should have been 1'\
         % (adapter, len(results))
     # Make sure it works through the WebSupport API
     support.get_search_results(u'SomeLongRandomWord')
 
 
 @skip_unless_importable('xapian', 'needs xapian bindings installed')
-@pytest.mark.skipif(sqlalchemy_missing, reason='needs sqlalchemy')
-def test_xapian():
-    search_adapter_helper('xapian')
+@skip_if_sqlalchemy_missing
+def test_xapian(rootdir, tmp_path):
+    search_adapter_helper(rootdir, tmp_path, 'xapian')
 
 
 @skip_unless_importable('whoosh', 'needs whoosh package installed')
-@pytest.mark.skipif(sqlalchemy_missing, reason='needs sqlalchemy')
-def test_whoosh():
-    search_adapter_helper('whoosh')
+@skip_if_sqlalchemy_missing
+def test_whoosh(rootdir, tmp_path, adapter):
+    search_adapter_helper(rootdir, tmp_path, 'whoosh')
```

### Comparing `sphinxcontrib-websupport-1.2.4/tests/test_websupport.py` & `sphinxcontrib_websupport-1.2.5/tests/test_websupport.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,8 @@
-# -*- coding: utf-8 -*-
-"""
-    test_websupport
-    ~~~~~~~~~~~~~~~
-
-    Test the Web Support Package
-
-    :copyright: Copyright 2007-2018 by the Sphinx team, see AUTHORS.
-    :license: BSD, see LICENSE for details.
-"""
+"""Test the Web Support Package"""
 
 from sphinxcontrib.websupport import WebSupport
 from sphinxcontrib.websupport.errors import DocumentNotFoundError, \
     CommentNotAllowedError, UserNotAuthorizedError
 from sphinxcontrib.websupport.storage import StorageBackend
 from sphinxcontrib.websupport.storage.differ import CombinedHtmlDiff
 try:
@@ -19,25 +10,29 @@
         Comment, CommentVote
     from sphinxcontrib.websupport.storage.sqlalchemy_db import Node
     sqlalchemy_missing = False
 except ImportError:
     sqlalchemy_missing = True
 
 import pytest
-from util import rootdir, tempdir
+
+skip_if_sqlalchemy_missing = pytest.mark.skipif(
+    sqlalchemy_missing,
+    reason='needs sqlalchemy',
+)
 
 
 @pytest.fixture
-def support(request):
+def support(rootdir, tmp_path, request):
     settings = {
-        'srcdir': rootdir / 'root',
+        'srcdir': rootdir / 'test-root',
         # to use same directory for 'builddir' in each 'support' fixture, using
         # 'tempdir' (static) value instead of 'tempdir' fixture value.
         # each test expect result of db value at previous test case.
-        'builddir': tempdir / 'websupport'
+        'builddir': tmp_path / 'websupport'
     }
     marker = request.node.get_closest_marker('support')
     if marker:
         settings.update(marker.kwargs)
 
     support = WebSupport(**settings)
     yield support
@@ -46,39 +41,39 @@
 with_support = pytest.mark.support
 
 
 class NullStorage(StorageBackend):
     pass
 
 
-@with_support(storage=NullStorage())
+@with_support(storage=NullStorage(), srcdir=None)
 def test_no_srcdir(support):
     # make sure the correct exception is raised if srcdir is not given.
     with pytest.raises(RuntimeError):
         support.build()
 
 
-@pytest.mark.skipif(sqlalchemy_missing, reason='needs sqlalchemy')
+@skip_if_sqlalchemy_missing
 @with_support()
 def test_build(support):
     support.build()
 
 
-@pytest.mark.skipif(sqlalchemy_missing, reason='needs sqlalchemy')
+@skip_if_sqlalchemy_missing
 @with_support()
 def test_get_document(support):
     with pytest.raises(DocumentNotFoundError):
         support.get_document('nonexisting')
 
     contents = support.get_document('contents')
     assert contents['title'] and contents['body'] \
         and contents['sidebar'] and contents['relbar']
 
 
-@pytest.mark.skipif(sqlalchemy_missing, reason='needs sqlalchemy')
+@skip_if_sqlalchemy_missing
 @with_support()
 def test_comments(support):
     session = Session()
     nodes = session.query(Node).all()
     first_node = nodes[0]
     second_node = nodes[1]
 
@@ -119,15 +114,15 @@
     children = comments[0]['children']
     assert len(comments) == 1
     assert comments[0]['text'] == '<p>First test comment</p>\n'
     assert len(children) == 1
     assert children[0]['text'] == '<p>Child test comment</p>\n'
 
 
-@pytest.mark.skipif(sqlalchemy_missing, reason='needs sqlalchemy')
+@skip_if_sqlalchemy_missing
 @with_support()
 def test_user_delete_comments(support):
     def get_comment():
         session = Session()
         node = session.query(Node).first()
         session.close()
         return support.get_data(node.id)['comments'][0]
@@ -148,15 +143,15 @@
 
 
 def moderation_callback(comment):
     global called
     called = True
 
 
-@pytest.mark.skipif(sqlalchemy_missing, reason='needs sqlalchemy')
+@skip_if_sqlalchemy_missing
 @with_support(moderation_callback=moderation_callback)
 def test_moderation(support):
     session = Session()
     nodes = session.query(Node).all()
     node = nodes[7]
     session.close()
     accepted = support.add_comment('Accepted Comment', node_id=node.id,
@@ -174,15 +169,15 @@
     support.delete_comment(deleted['id'], moderator=True)
     comments = support.get_data(node.id)['comments']
     assert len(comments) == 1
     comments = support.get_data(node.id, moderator=True)['comments']
     assert len(comments) == 1
 
 
-@pytest.mark.skipif(sqlalchemy_missing, reason='needs sqlalchemy')
+@skip_if_sqlalchemy_missing
 @with_support()
 def test_moderator_delete_comments(support):
     def get_comment():
         session = Session()
         node = session.query(Node).first()
         session.close()
         return support.get_data(node.id, moderator=True)['comments'][1]
@@ -190,15 +185,15 @@
     comment = get_comment()
     support.delete_comment(comment['id'], username='user_two',
                            moderator=True)
     with pytest.raises(IndexError):
         get_comment()
 
 
-@pytest.mark.skipif(sqlalchemy_missing, reason='needs sqlalchemy')
+@skip_if_sqlalchemy_missing
 @with_support()
 def test_update_username(support):
     support.update_username('user_two', 'new_user_two')
     session = Session()
     comments = session.query(Comment).\
         filter(Comment.username == 'user_two').all()
     assert len(comments) == 0
@@ -209,15 +204,15 @@
         filter(Comment.username == 'new_user_two').all()
     assert len(comments) == 1
     votes = session.query(CommentVote).\
         filter(CommentVote.username == 'new_user_two').all()
     assert len(votes) == 0
 
 
-@pytest.mark.skipif(sqlalchemy_missing, reason='needs sqlalchemy')
+@skip_if_sqlalchemy_missing
 @with_support()
 def test_proposals(support):
     session = Session()
     node = session.query(Node).first()
 
     data = support.get_data(node.id)
 
@@ -225,15 +220,15 @@
     proposal = source[:5] + source[10:15] + 'asdf' + source[15:]
 
     support.add_comment('Proposal comment',
                         node_id=node.id,
                         proposal=proposal)
 
 
-@pytest.mark.skipif(sqlalchemy_missing, reason='needs sqlalchemy')
+@skip_if_sqlalchemy_missing
 @with_support()
 def test_voting(support):
     session = Session()
     nodes = session.query(Node).all()
     node = nodes[0]
 
     comment = support.get_data(node.id)['comments'][0]
```

