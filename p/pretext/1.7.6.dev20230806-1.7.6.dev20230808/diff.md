# Comparing `tmp/pretext-1.7.6.dev20230806.tar.gz` & `tmp/pretext-1.7.6.dev20230808.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretext-1.7.6.dev20230806.tar", max compression
+gzip compressed data, was "pretext-1.7.6.dev20230808.tar", max compression
```

## Comparing `pretext-1.7.6.dev20230806.tar` & `pretext-1.7.6.dev20230808.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    35148 2023-08-06 06:12:44.243923 pretext-1.7.6.dev20230806/LICENSE
--rw-r--r--   0        0        0     9757 2023-08-06 06:12:44.243923 pretext-1.7.6.dev20230806/README.md
--rw-r--r--   0        0        0     1500 2023-08-06 06:13:25.502509 pretext-1.7.6.dev20230806/pretext/__init__.py
--rw-r--r--   0        0        0       61 2023-08-06 06:12:44.243923 pretext-1.7.6.dev20230806/pretext/__main__.py
--rw-r--r--   0        0        0    11608 2023-08-06 06:12:44.243923 pretext-1.7.6.dev20230806/pretext/build.py
--rw-r--r--   0        0        0    27783 2023-08-06 06:12:44.243923 pretext-1.7.6.dev20230806/pretext/cli.py
--rw-r--r--   0        0        0     6149 2023-08-06 06:12:44.243923 pretext-1.7.6.dev20230806/pretext/codechat.py
--rw-r--r--   0        0        0     5943 2023-08-06 06:12:44.243923 pretext-1.7.6.dev20230806/pretext/config/xml_overlay.py
--rw-r--r--   0        0        0      675 2023-08-06 06:12:44.243923 pretext-1.7.6.dev20230806/pretext/constants.py
--rw-r--r--   0        0        0      350 2023-08-06 06:12:44.243923 pretext-1.7.6.dev20230806/pretext/core/__init__.py
--rw-r--r--   0        0        0   172548 2023-08-06 06:13:30.750839 pretext-1.7.6.dev20230806/pretext/core/pretext.py
--rw-r--r--   0        0        0     1484 2023-08-06 06:12:44.243923 pretext-1.7.6.dev20230806/pretext/core/resources.py
--rw-r--r--   0        0        0  1045313 2023-08-06 06:13:30.750839 pretext-1.7.6.dev20230806/pretext/core/resources.zip
--rw-r--r--   0        0        0    16811 2023-08-06 06:12:44.243923 pretext-1.7.6.dev20230806/pretext/generate.py
--rw-r--r--   0        0        0    29656 2023-08-06 06:12:44.243923 pretext-1.7.6.dev20230806/pretext/project/__init__.py
--rw-r--r--   0        0        0    30392 2023-08-06 06:12:44.243923 pretext-1.7.6.dev20230806/pretext/project/refactor.py
--rw-r--r--   0        0        0     2620 2023-08-06 06:12:44.243923 pretext-1.7.6.dev20230806/pretext/project/xml.py
--rw-r--r--   0        0        0      739 2023-08-06 06:12:44.243923 pretext-1.7.6.dev20230806/pretext/templates/__init__.py
--rw-r--r--   0        0        0     2480 2023-08-06 06:13:30.822843 pretext-1.7.6.dev20230806/pretext/templates/resources/.devcontainer.json
--rw-r--r--   0        0        0     1676 2023-08-06 06:13:30.822843 pretext-1.7.6.dev20230806/pretext/templates/resources/.gitignore
--rw-r--r--   0        0        0        0 2023-08-06 06:13:30.822843 pretext-1.7.6.dev20230806/pretext/templates/resources/__init__.py
--rw-r--r--   0        0        0   158949 2023-08-06 06:13:30.822843 pretext-1.7.6.dev20230806/pretext/templates/resources/article.zip
--rw-r--r--   0        0        0     6455 2023-08-06 06:13:30.794841 pretext-1.7.6.dev20230806/pretext/templates/resources/book.zip
--rw-r--r--   0        0        0   172278 2023-08-06 06:13:30.810842 pretext-1.7.6.dev20230806/pretext/templates/resources/demo.zip
--rw-r--r--   0        0        0     3496 2023-08-06 06:13:30.798842 pretext-1.7.6.dev20230806/pretext/templates/resources/hello.zip
--rw-r--r--   0        0        0     1710 2023-08-06 06:13:30.822843 pretext-1.7.6.dev20230806/pretext/templates/resources/project.ptx
--rw-r--r--   0        0        0      242 2023-08-06 06:13:30.822843 pretext-1.7.6.dev20230806/pretext/templates/resources/publication.ptx
--rw-r--r--   0        0        0     7231 2023-08-06 06:13:30.794841 pretext-1.7.6.dev20230806/pretext/templates/resources/slideshow.zip
--rw-r--r--   0        0        0      109 2023-08-06 06:12:44.243923 pretext-1.7.6.dev20230806/pretext/types.py
--rw-r--r--   0        0        0    25415 2023-08-06 06:12:44.243923 pretext-1.7.6.dev20230806/pretext/utils.py
--rw-r--r--   0        0        0     3353 2023-08-06 06:13:25.502509 pretext-1.7.6.dev20230806/pyproject.toml
--rw-r--r--   0        0        0    10891 1970-01-01 00:00:00.000000 pretext-1.7.6.dev20230806/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-08-08 06:13:15.580701 pretext-1.7.6.dev20230808/LICENSE
+-rw-r--r--   0        0        0     9757 2023-08-08 06:13:15.584701 pretext-1.7.6.dev20230808/README.md
+-rw-r--r--   0        0        0     1500 2023-08-08 06:13:54.084736 pretext-1.7.6.dev20230808/pretext/__init__.py
+-rw-r--r--   0        0        0       61 2023-08-08 06:13:15.584701 pretext-1.7.6.dev20230808/pretext/__main__.py
+-rw-r--r--   0        0        0    11608 2023-08-08 06:13:15.584701 pretext-1.7.6.dev20230808/pretext/build.py
+-rw-r--r--   0        0        0    27783 2023-08-08 06:13:15.584701 pretext-1.7.6.dev20230808/pretext/cli.py
+-rw-r--r--   0        0        0     6149 2023-08-08 06:13:15.584701 pretext-1.7.6.dev20230808/pretext/codechat.py
+-rw-r--r--   0        0        0     5943 2023-08-08 06:13:15.584701 pretext-1.7.6.dev20230808/pretext/config/xml_overlay.py
+-rw-r--r--   0        0        0      675 2023-08-08 06:13:15.584701 pretext-1.7.6.dev20230808/pretext/constants.py
+-rw-r--r--   0        0        0      350 2023-08-08 06:13:15.584701 pretext-1.7.6.dev20230808/pretext/core/__init__.py
+-rw-r--r--   0        0        0   172548 2023-08-08 06:13:59.552741 pretext-1.7.6.dev20230808/pretext/core/pretext.py
+-rw-r--r--   0        0        0     1484 2023-08-08 06:13:15.584701 pretext-1.7.6.dev20230808/pretext/core/resources.py
+-rw-r--r--   0        0        0  1045746 2023-08-08 06:13:59.552741 pretext-1.7.6.dev20230808/pretext/core/resources.zip
+-rw-r--r--   0        0        0    16811 2023-08-08 06:13:15.584701 pretext-1.7.6.dev20230808/pretext/generate.py
+-rw-r--r--   0        0        0    29656 2023-08-08 06:13:15.584701 pretext-1.7.6.dev20230808/pretext/project/__init__.py
+-rw-r--r--   0        0        0    30392 2023-08-08 06:13:15.584701 pretext-1.7.6.dev20230808/pretext/project/refactor.py
+-rw-r--r--   0        0        0     2620 2023-08-08 06:13:15.584701 pretext-1.7.6.dev20230808/pretext/project/xml.py
+-rw-r--r--   0        0        0      739 2023-08-08 06:13:15.584701 pretext-1.7.6.dev20230808/pretext/templates/__init__.py
+-rw-r--r--   0        0        0     2480 2023-08-08 06:13:59.636741 pretext-1.7.6.dev20230808/pretext/templates/resources/.devcontainer.json
+-rw-r--r--   0        0        0     1676 2023-08-08 06:13:59.636741 pretext-1.7.6.dev20230808/pretext/templates/resources/.gitignore
+-rw-r--r--   0        0        0        0 2023-08-08 06:13:59.636741 pretext-1.7.6.dev20230808/pretext/templates/resources/__init__.py
+-rw-r--r--   0        0        0   158949 2023-08-08 06:13:59.636741 pretext-1.7.6.dev20230808/pretext/templates/resources/article.zip
+-rw-r--r--   0        0        0     6455 2023-08-08 06:13:59.600741 pretext-1.7.6.dev20230808/pretext/templates/resources/book.zip
+-rw-r--r--   0        0        0   172278 2023-08-08 06:13:59.624741 pretext-1.7.6.dev20230808/pretext/templates/resources/demo.zip
+-rw-r--r--   0        0        0     3496 2023-08-08 06:13:59.608741 pretext-1.7.6.dev20230808/pretext/templates/resources/hello.zip
+-rw-r--r--   0        0        0     1710 2023-08-08 06:13:59.636741 pretext-1.7.6.dev20230808/pretext/templates/resources/project.ptx
+-rw-r--r--   0        0        0      242 2023-08-08 06:13:59.636741 pretext-1.7.6.dev20230808/pretext/templates/resources/publication.ptx
+-rw-r--r--   0        0        0     7231 2023-08-08 06:13:59.604741 pretext-1.7.6.dev20230808/pretext/templates/resources/slideshow.zip
+-rw-r--r--   0        0        0      109 2023-08-08 06:13:15.584701 pretext-1.7.6.dev20230808/pretext/types.py
+-rw-r--r--   0        0        0    25415 2023-08-08 06:13:15.584701 pretext-1.7.6.dev20230808/pretext/utils.py
+-rw-r--r--   0        0        0     3353 2023-08-08 06:13:54.084736 pretext-1.7.6.dev20230808/pyproject.toml
+-rw-r--r--   0        0        0    10891 1970-01-01 00:00:00.000000 pretext-1.7.6.dev20230808/PKG-INFO
```

### Comparing `pretext-1.7.6.dev20230806/LICENSE` & `pretext-1.7.6.dev20230808/LICENSE`

 * *Files identical despite different names*

### Comparing `pretext-1.7.6.dev20230806/README.md` & `pretext-1.7.6.dev20230808/README.md`

 * *Files identical despite different names*

### Comparing `pretext-1.7.6.dev20230806/pretext/__init__.py` & `pretext-1.7.6.dev20230808/pretext/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from pathlib import Path
 from single_version import get_version
 
 log = logging.getLogger("ptxlogger")
 
 VERSION = get_version("pretext", Path(__file__).parent.parent)
 
-CORE_COMMIT = '0e1d2ae93af3a2b0a7bca038422a34d192445035'
+CORE_COMMIT = '7af51c6808a0f3107cf7f572e895da3c71898f14'
 
 
 def activate() -> None:
     """
     This function was provided by the original `pretext` package
     deployed to PyPI by Alex Willmer. Thanks to their generosity,
     we were allowed to adopt this namespace as of 1.0, so we raise an error here
```

### Comparing `pretext-1.7.6.dev20230806/pretext/build.py` & `pretext-1.7.6.dev20230808/pretext/build.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.6.dev20230806/pretext/cli.py` & `pretext-1.7.6.dev20230808/pretext/cli.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.6.dev20230806/pretext/codechat.py` & `pretext-1.7.6.dev20230808/pretext/codechat.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.6.dev20230806/pretext/config/xml_overlay.py` & `pretext-1.7.6.dev20230808/pretext/config/xml_overlay.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.6.dev20230806/pretext/constants.py` & `pretext-1.7.6.dev20230808/pretext/constants.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.6.dev20230806/pretext/core/pretext.py` & `pretext-1.7.6.dev20230808/pretext/core/pretext.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.6.dev20230806/pretext/core/resources.py` & `pretext-1.7.6.dev20230808/pretext/core/resources.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.6.dev20230806/pretext/core/resources.zip` & `pretext-1.7.6.dev20230808/pretext/core/resources.zip`

 * *Files 18% similar despite different names*

#### zipinfo {}

```diff
@@ -1,144 +1,144 @@
-Zip file size: 1045313 bytes, number of entries: 142
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-06 06:13 css/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-06 06:13 pretext/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-06 06:13 schema/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-06 06:13 script/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-06 06:13 xsl/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-06 06:13 script/mjsre/
--rw-r--r--  2.0 unx      258 b- defN 23-Aug-06 06:13 script/README.md
--rw-r--r--  2.0 unx     2666 b- defN 23-Aug-06 06:13 script/mbx
--rw-r--r--  2.0 unx      116 b- defN 23-Aug-06 06:13 script/mjsre/package.json
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-06 06:13 script/mjsre/update-sre
--rw-r--r--  2.0 unx     9251 b- defN 23-Aug-06 06:13 script/mjsre/mj-sre-page.js
--rw-r--r--  2.0 unx      481 b- defN 23-Aug-06 06:13 script/mjsre/README.md
--rw-r--r--  2.0 unx   134086 b- defN 23-Aug-06 06:13 schema/pretext.xml
--rw-r--r--  2.0 unx   125241 b- defN 23-Aug-06 06:13 schema/pretext.xsd
--rw-r--r--  2.0 unx    18421 b- defN 23-Aug-06 06:13 schema/pretext-schematron.xsl
--rw-r--r--  2.0 unx    25870 b- defN 23-Aug-06 06:13 schema/pretext-validation-plus.xsl
--rw-r--r--  2.0 unx    58129 b- defN 23-Aug-06 06:13 schema/pretext.rnc
--rw-r--r--  2.0 unx      326 b- defN 23-Aug-06 06:13 schema/xml.xsd
--rw-r--r--  2.0 unx   101895 b- defN 23-Aug-06 06:13 schema/pretext.rng
--rw-r--r--  2.0 unx    17587 b- defN 23-Aug-06 06:13 schema/pretext-dev.rnc
--rw-r--r--  2.0 unx     1180 b- defN 23-Aug-06 06:13 schema/README.md
--rw-r--r--  2.0 unx    34210 b- defN 23-Aug-06 06:13 schema/pretext-dev.rng
--rw-r--r--  2.0 unx     3135 b- defN 23-Aug-06 06:13 schema/build.sh
--rw-r--r--  2.0 unx     2566 b- defN 23-Aug-06 06:13 pretext/pretext.cfg
--rw-r--r--  2.0 unx     1955 b- defN 23-Aug-06 06:13 pretext/module-test.py
--rw-r--r--  2.0 unx    30908 b- defN 23-Aug-06 06:13 pretext/pretext
--rw-r--r--  2.0 unx   172548 b- defN 23-Aug-06 06:13 pretext/pretext.py
--rw-r--r--  2.0 unx    36045 b- defN 23-Aug-06 06:13 pretext/braille_format.py
--rw-r--r--  2.0 unx     1367 b- defN 23-Aug-06 06:13 pretext/README.md
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-06 06:13 pretext/__init__.py
--rw-r--r--  2.0 unx     2446 b- defN 23-Aug-06 06:13 css/colors_martiansands.css
--rw-r--r--  2.0 unx     4021 b- defN 23-Aug-06 06:13 css/update_css
--rw-r--r--  2.0 unx    71198 b- defN 23-Aug-06 06:13 css/pretext_add_on.css
--rw-r--r--  2.0 unx    12567 b- defN 23-Aug-06 06:13 css/style_oscarlevin.css
--rw-r--r--  2.0 unx     1276 b- defN 23-Aug-06 06:13 css/colors_maroon_grey.css
--rw-r--r--  2.0 unx    63664 b- defN 23-Aug-06 06:13 css/mathbook-add-on.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Aug-06 06:13 css/colors_green_blue.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Aug-06 06:13 css/colors_ruby_emerald.css
--rw-r--r--  2.0 unx     2441 b- defN 23-Aug-06 06:13 css/kindle.css
--rw-r--r--  2.0 unx    22438 b- defN 23-Aug-06 06:13 css/pretext.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Aug-06 06:13 css/colors_blue_red.css
--rw-r--r--  2.0 unx     2446 b- defN 23-Aug-06 06:13 css/colors_darkmartiansands.css
--rw-r--r--  2.0 unx     1362 b- defN 23-Aug-06 06:13 css/epub.css
--rw-r--r--  2.0 unx     3473 b- defN 23-Aug-06 06:13 css/style_soundwriting.css
--rw-r--r--  2.0 unx      691 b- defN 23-Aug-06 06:13 css/colors_pastel_blue_orange.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Aug-06 06:13 css/colors_ruby_turquoise.css
--rw-r--r--  2.0 unx     2608 b- defN 23-Aug-06 06:13 css/colors_default.css
--rw-r--r--  2.0 unx     2438 b- defN 23-Aug-06 06:13 css/colors_blue_grey.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Aug-06 06:13 css/colors_orange_navy.css
--rw-r--r--  2.0 unx   435680 b- defN 23-Aug-06 06:13 css/mathbook-3.css
--rw-r--r--  2.0 unx     7761 b- defN 23-Aug-06 06:13 css/style_default.css
--rw-r--r--  2.0 unx     1338 b- defN 23-Aug-06 06:13 css/colors_red_blue.css
--rw-r--r--  2.0 unx   146685 b- defN 23-Aug-06 06:13 css/mathbook-content.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Aug-06 06:13 css/colors_ruby_amethyst.css
--rw-r--r--  2.0 unx     1865 b- defN 23-Aug-06 06:13 css/README.md
--rw-r--r--  2.0 unx     2397 b- defN 23-Aug-06 06:13 css/colors_green_plum.css
--rw-r--r--  2.0 unx     4308 b- defN 23-Aug-06 06:13 css/colors_blue_green.css
--rw-r--r--  2.0 unx     1280 b- defN 23-Aug-06 06:13 css/colors_brown_gold.css
--rw-r--r--  2.0 unx    14069 b- defN 23-Aug-06 06:13 css/setcolors.css
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-06 06:13 xsl/latex/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-06 06:13 xsl/localizations/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-06 06:13 xsl/support/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-06 06:13 xsl/utilities/
--rw-r--r--  2.0 unx     2725 b- defN 23-Aug-06 06:13 xsl/extract-asymptote.xsl
--rw-r--r--  2.0 unx    10708 b- defN 23-Aug-06 06:13 xsl/pretext-units.xsl
--rw-r--r--  2.0 unx    17293 b- defN 23-Aug-06 06:13 xsl/pretext-ww-problem-sets.xsl
--rw-r--r--  2.0 unx     4571 b- defN 23-Aug-06 06:13 xsl/pretext-litprog.xsl
--rw-r--r--  2.0 unx     8125 b- defN 23-Aug-06 06:13 xsl/extract-sageplot.xsl
--rw-r--r--  2.0 unx   548615 b- defN 23-Aug-06 06:13 xsl/pretext-common.xsl
--rw-r--r--  2.0 unx     3560 b- defN 23-Aug-06 06:13 xsl/pretext-basic-html.xsl
--rw-r--r--  2.0 unx    21086 b- defN 23-Aug-06 06:13 xsl/pretext-smc.xsl
--rw-r--r--  2.0 unx     2597 b- defN 23-Aug-06 06:13 xsl/extract-trace.xsl
--rw-r--r--  2.0 unx    19072 b- defN 23-Aug-06 06:13 xsl/extract-latex-image.xsl
--rw-r--r--  2.0 unx     2248 b- defN 23-Aug-06 06:13 xsl/extract-mom.xsl
--rw-r--r--  2.0 unx    67275 b- defN 23-Aug-06 06:13 xsl/pretext-epub.xsl
--rw-r--r--  2.0 unx    11766 b- defN 23-Aug-06 06:13 xsl/pretext-sage-doctest.xsl
--rw-r--r--  2.0 unx     6066 b- defN 23-Aug-06 06:13 xsl/pretext-json-manifest.xsl
--rw-r--r--  2.0 unx    22121 b- defN 23-Aug-06 06:13 xsl/pretext-revealjs.xsl
--rw-r--r--  2.0 unx     2740 b- defN 23-Aug-06 06:13 xsl/extract-youtube.xsl
--rw-r--r--  2.0 unx    40230 b- defN 23-Aug-06 06:13 xsl/pretext-jupyter.xsl
--rw-r--r--  2.0 unx   611284 b- defN 23-Aug-06 06:13 xsl/pretext-html.xsl
--rw-r--r--  2.0 unx    39918 b- defN 23-Aug-06 06:13 xsl/pretext-runestone-static.xsl
--rw-r--r--  2.0 unx     9787 b- defN 23-Aug-06 06:13 xsl/entities.ent
--rw-r--r--  2.0 unx     3239 b- defN 23-Aug-06 06:13 xsl/extract-interactive.xsl
--rw-r--r--  2.0 unx   231265 b- defN 23-Aug-06 06:13 xsl/publisher-variables.xsl
--rw-r--r--  2.0 unx     2709 b- defN 23-Aug-06 06:13 xsl/extract-qrcode.xsl
--rw-r--r--  2.0 unx    13037 b- defN 23-Aug-06 06:13 xsl/pretext-text.xsl
--rw-r--r--  2.0 unx    41730 b- defN 23-Aug-06 06:13 xsl/pretext-beamer.xsl
--rw-r--r--  2.0 unx    43020 b- defN 23-Aug-06 06:13 xsl/pretext-text-utilities.xsl
--rw-r--r--  2.0 unx     2601 b- defN 23-Aug-06 06:13 xsl/pretext-merge.xsl
--rw-r--r--  2.0 unx   139486 b- defN 23-Aug-06 06:13 xsl/extract-pg.xsl
--rw-r--r--  2.0 unx   116581 b- defN 23-Aug-06 06:13 xsl/pretext-assembly.xsl
--rw-r--r--  2.0 unx     2846 b- defN 23-Aug-06 06:13 xsl/extract-datafile.xsl
--rw-r--r--  2.0 unx     1768 b- defN 23-Aug-06 06:13 xsl/README.md
--rw-r--r--  2.0 unx    13186 b- defN 23-Aug-06 06:13 xsl/pretext-solution-manual-latex.xsl
--rw-r--r--  2.0 unx     6281 b- defN 23-Aug-06 06:13 xsl/pretext-numbers.xsl
--rw-r--r--  2.0 unx     8535 b- defN 23-Aug-06 06:13 xsl/pretext-view-source.xsl
--rw-r--r--  2.0 unx    12084 b- defN 23-Aug-06 06:13 xsl/xml-to-json.xsl
--rw-r--r--  2.0 unx     8130 b- defN 23-Aug-06 06:13 xsl/extract-identity.xsl
--rw-r--r--  2.0 unx    94587 b- defN 23-Aug-06 06:13 xsl/pretext-braille-preprint.xsl
--rw-r--r--  2.0 unx   111515 b- defN 23-Aug-06 06:13 xsl/pretext-runestone.xsl
--rw-r--r--  2.0 unx   544154 b- defN 23-Aug-06 06:13 xsl/pretext-latex.xsl
--rw-r--r--  2.0 unx      787 b- defN 23-Aug-06 06:13 xsl/utilities/deprecate-index.sed
--rw-r--r--  2.0 unx      513 b- defN 23-Aug-06 06:13 xsl/utilities/deprecate-autoname.sed
--rw-r--r--  2.0 unx     4926 b- defN 23-Aug-06 06:13 xsl/utilities/pretext-enhanced-source.xsl
--rw-r--r--  2.0 unx    30257 b- defN 23-Aug-06 06:13 xsl/utilities/fix-deprecations.xsl
--rw-r--r--  2.0 unx     1810 b- defN 23-Aug-06 06:13 xsl/utilities/README.md
--rw-r--r--  2.0 unx     4299 b- defN 23-Aug-06 06:13 xsl/utilities/author-report.xsl
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-06 06:13 xsl/support/play-button/
--rw-r--r--  2.0 unx     5879 b- defN 23-Aug-06 06:13 xsl/support/package-math.xsl
--rw-r--r--  2.0 unx     5241 b- defN 23-Aug-06 06:13 xsl/support/pretext-pg-macros.xsl
--rw-r--r--  2.0 unx      486 b- defN 23-Aug-06 06:13 xsl/support/runestone-services.xml
--rw-r--r--  2.0 unx    10306 b- defN 23-Aug-06 06:13 xsl/support/extract-math.xsl
--rw-r--r--  2.0 unx     5065 b- defN 23-Aug-06 06:13 xsl/support/extract-latex-image-labels.xsl
--rw-r--r--  2.0 unx      504 b- defN 23-Aug-06 06:13 xsl/support/README.md
--rw-r--r--  2.0 unx     5800 b- defN 23-Aug-06 06:13 xsl/support/tactile-svg.xsl
--rw-r--r--  2.0 unx      722 b- defN 23-Aug-06 06:13 xsl/support/play-button/play-button.svg
--rw-r--r--  2.0 unx     2657 b- defN 23-Aug-06 06:13 xsl/support/play-button/README.md
--rw-r--r--  2.0 unx     6621 b- defN 23-Aug-06 06:13 xsl/support/play-button/play-button.png
--rw-r--r--  2.0 unx    17231 b- defN 23-Aug-06 06:13 xsl/localizations/de-DE.xml
--rw-r--r--  2.0 unx    16312 b- defN 23-Aug-06 06:13 xsl/localizations/pt-BR.xml
--rw-r--r--  2.0 unx     2286 b- defN 23-Aug-06 06:13 xsl/localizations/localizations.xml
--rw-r--r--  2.0 unx    17301 b- defN 23-Aug-06 06:13 xsl/localizations/fi-FI.xml
--rw-r--r--  2.0 unx    16349 b- defN 23-Aug-06 06:13 xsl/localizations/fr-FR.xml
--rw-r--r--  2.0 unx    16534 b- defN 23-Aug-06 06:13 xsl/localizations/es-ES.xml
--rw-r--r--  2.0 unx    16837 b- defN 23-Aug-06 06:13 xsl/localizations/af-ZA.xml
--rw-r--r--  2.0 unx    19185 b- defN 23-Aug-06 06:13 xsl/localizations/nl-NL.xml
--rw-r--r--  2.0 unx    16252 b- defN 23-Aug-06 06:13 xsl/localizations/ca-ES.xml
--rw-r--r--  2.0 unx    17056 b- defN 23-Aug-06 06:13 xsl/localizations/bg-BG.xml
--rw-r--r--  2.0 unx    17081 b- defN 23-Aug-06 06:13 xsl/localizations/pt-PT.xml
--rw-r--r--  2.0 unx    15582 b- defN 23-Aug-06 06:13 xsl/localizations/cs-CZ.xml
--rw-r--r--  2.0 unx    20481 b- defN 23-Aug-06 06:13 xsl/localizations/ku-CKB.xml
--rw-r--r--  2.0 unx    19326 b- defN 23-Aug-06 06:13 xsl/localizations/en-US.xml
--rw-r--r--  2.0 unx     4760 b- defN 23-Aug-06 06:13 xsl/localizations/README.md
--rw-r--r--  2.0 unx    15866 b- defN 23-Aug-06 06:13 xsl/localizations/it-IT.xml
--rw-r--r--  2.0 unx    16085 b- defN 23-Aug-06 06:13 xsl/localizations/hu-HU.xml
--rw-r--r--  2.0 unx    16500 b- defN 23-Aug-06 06:13 xsl/localizations/fr-CA.xml
--rw-r--r--  2.0 unx     5135 b- defN 23-Aug-06 06:13 xsl/latex/pretext-latex-guide.xsl
--rw-r--r--  2.0 unx     2261 b- defN 23-Aug-06 06:13 xsl/latex/pretext-latex-AIM.xsl
--rw-r--r--  2.0 unx    14482 b- defN 23-Aug-06 06:13 xsl/latex/pretext-latex-chaos.xsl
--rw-r--r--  2.0 unx     7526 b- defN 23-Aug-06 06:13 xsl/latex/pretext-latex-CLP.xsl
--rw-r--r--  2.0 unx     3024 b- defN 23-Aug-06 06:13 xsl/latex/pretext-latex-dyslexic-font.xsl
-142 files, 4849033 bytes uncompressed, 1027739 bytes compressed:  78.8%
+Zip file size: 1045746 bytes, number of entries: 142
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-08 06:13 css/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-08 06:13 pretext/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-08 06:13 schema/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-08 06:13 script/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-08 06:13 xsl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-08 06:13 script/mjsre/
+-rw-r--r--  2.0 unx      258 b- defN 23-Aug-08 06:13 script/README.md
+-rw-r--r--  2.0 unx     2666 b- defN 23-Aug-08 06:13 script/mbx
+-rw-r--r--  2.0 unx      116 b- defN 23-Aug-08 06:13 script/mjsre/package.json
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-08 06:13 script/mjsre/update-sre
+-rw-r--r--  2.0 unx     9251 b- defN 23-Aug-08 06:13 script/mjsre/mj-sre-page.js
+-rw-r--r--  2.0 unx      481 b- defN 23-Aug-08 06:13 script/mjsre/README.md
+-rw-r--r--  2.0 unx   134438 b- defN 23-Aug-08 06:13 schema/pretext.xml
+-rw-r--r--  2.0 unx   126785 b- defN 23-Aug-08 06:13 schema/pretext.xsd
+-rw-r--r--  2.0 unx    18421 b- defN 23-Aug-08 06:13 schema/pretext-schematron.xsl
+-rw-r--r--  2.0 unx    25870 b- defN 23-Aug-08 06:13 schema/pretext-validation-plus.xsl
+-rw-r--r--  2.0 unx    58378 b- defN 23-Aug-08 06:13 schema/pretext.rnc
+-rw-r--r--  2.0 unx      326 b- defN 23-Aug-08 06:13 schema/xml.xsd
+-rw-r--r--  2.0 unx   102431 b- defN 23-Aug-08 06:13 schema/pretext.rng
+-rw-r--r--  2.0 unx    17587 b- defN 23-Aug-08 06:13 schema/pretext-dev.rnc
+-rw-r--r--  2.0 unx     1180 b- defN 23-Aug-08 06:13 schema/README.md
+-rw-r--r--  2.0 unx    34210 b- defN 23-Aug-08 06:13 schema/pretext-dev.rng
+-rw-r--r--  2.0 unx     3135 b- defN 23-Aug-08 06:13 schema/build.sh
+-rw-r--r--  2.0 unx     2566 b- defN 23-Aug-08 06:13 pretext/pretext.cfg
+-rw-r--r--  2.0 unx     1955 b- defN 23-Aug-08 06:13 pretext/module-test.py
+-rw-r--r--  2.0 unx    30908 b- defN 23-Aug-08 06:13 pretext/pretext
+-rw-r--r--  2.0 unx   172548 b- defN 23-Aug-08 06:13 pretext/pretext.py
+-rw-r--r--  2.0 unx    36045 b- defN 23-Aug-08 06:13 pretext/braille_format.py
+-rw-r--r--  2.0 unx     1367 b- defN 23-Aug-08 06:13 pretext/README.md
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-08 06:13 pretext/__init__.py
+-rw-r--r--  2.0 unx     2446 b- defN 23-Aug-08 06:13 css/colors_martiansands.css
+-rw-r--r--  2.0 unx     4021 b- defN 23-Aug-08 06:13 css/update_css
+-rw-r--r--  2.0 unx    71198 b- defN 23-Aug-08 06:13 css/pretext_add_on.css
+-rw-r--r--  2.0 unx    12567 b- defN 23-Aug-08 06:13 css/style_oscarlevin.css
+-rw-r--r--  2.0 unx     1276 b- defN 23-Aug-08 06:13 css/colors_maroon_grey.css
+-rw-r--r--  2.0 unx    63664 b- defN 23-Aug-08 06:13 css/mathbook-add-on.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Aug-08 06:13 css/colors_green_blue.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Aug-08 06:13 css/colors_ruby_emerald.css
+-rw-r--r--  2.0 unx     2441 b- defN 23-Aug-08 06:13 css/kindle.css
+-rw-r--r--  2.0 unx    22438 b- defN 23-Aug-08 06:13 css/pretext.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Aug-08 06:13 css/colors_blue_red.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-Aug-08 06:13 css/colors_darkmartiansands.css
+-rw-r--r--  2.0 unx     1362 b- defN 23-Aug-08 06:13 css/epub.css
+-rw-r--r--  2.0 unx     3473 b- defN 23-Aug-08 06:13 css/style_soundwriting.css
+-rw-r--r--  2.0 unx      691 b- defN 23-Aug-08 06:13 css/colors_pastel_blue_orange.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Aug-08 06:13 css/colors_ruby_turquoise.css
+-rw-r--r--  2.0 unx     2608 b- defN 23-Aug-08 06:13 css/colors_default.css
+-rw-r--r--  2.0 unx     2438 b- defN 23-Aug-08 06:13 css/colors_blue_grey.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Aug-08 06:13 css/colors_orange_navy.css
+-rw-r--r--  2.0 unx   435680 b- defN 23-Aug-08 06:13 css/mathbook-3.css
+-rw-r--r--  2.0 unx     7761 b- defN 23-Aug-08 06:13 css/style_default.css
+-rw-r--r--  2.0 unx     1338 b- defN 23-Aug-08 06:13 css/colors_red_blue.css
+-rw-r--r--  2.0 unx   146685 b- defN 23-Aug-08 06:13 css/mathbook-content.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Aug-08 06:13 css/colors_ruby_amethyst.css
+-rw-r--r--  2.0 unx     1865 b- defN 23-Aug-08 06:13 css/README.md
+-rw-r--r--  2.0 unx     2397 b- defN 23-Aug-08 06:13 css/colors_green_plum.css
+-rw-r--r--  2.0 unx     4308 b- defN 23-Aug-08 06:13 css/colors_blue_green.css
+-rw-r--r--  2.0 unx     1280 b- defN 23-Aug-08 06:13 css/colors_brown_gold.css
+-rw-r--r--  2.0 unx    14069 b- defN 23-Aug-08 06:13 css/setcolors.css
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-08 06:13 xsl/latex/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-08 06:13 xsl/localizations/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-08 06:13 xsl/support/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-08 06:13 xsl/utilities/
+-rw-r--r--  2.0 unx     2725 b- defN 23-Aug-08 06:13 xsl/extract-asymptote.xsl
+-rw-r--r--  2.0 unx    10708 b- defN 23-Aug-08 06:13 xsl/pretext-units.xsl
+-rw-r--r--  2.0 unx    17293 b- defN 23-Aug-08 06:13 xsl/pretext-ww-problem-sets.xsl
+-rw-r--r--  2.0 unx     4571 b- defN 23-Aug-08 06:13 xsl/pretext-litprog.xsl
+-rw-r--r--  2.0 unx     8125 b- defN 23-Aug-08 06:13 xsl/extract-sageplot.xsl
+-rw-r--r--  2.0 unx   548615 b- defN 23-Aug-08 06:13 xsl/pretext-common.xsl
+-rw-r--r--  2.0 unx     3560 b- defN 23-Aug-08 06:13 xsl/pretext-basic-html.xsl
+-rw-r--r--  2.0 unx    21086 b- defN 23-Aug-08 06:13 xsl/pretext-smc.xsl
+-rw-r--r--  2.0 unx     2597 b- defN 23-Aug-08 06:13 xsl/extract-trace.xsl
+-rw-r--r--  2.0 unx    19072 b- defN 23-Aug-08 06:13 xsl/extract-latex-image.xsl
+-rw-r--r--  2.0 unx     2248 b- defN 23-Aug-08 06:13 xsl/extract-mom.xsl
+-rw-r--r--  2.0 unx    67275 b- defN 23-Aug-08 06:13 xsl/pretext-epub.xsl
+-rw-r--r--  2.0 unx    11766 b- defN 23-Aug-08 06:13 xsl/pretext-sage-doctest.xsl
+-rw-r--r--  2.0 unx     6066 b- defN 23-Aug-08 06:13 xsl/pretext-json-manifest.xsl
+-rw-r--r--  2.0 unx    22121 b- defN 23-Aug-08 06:13 xsl/pretext-revealjs.xsl
+-rw-r--r--  2.0 unx     2740 b- defN 23-Aug-08 06:13 xsl/extract-youtube.xsl
+-rw-r--r--  2.0 unx    40230 b- defN 23-Aug-08 06:13 xsl/pretext-jupyter.xsl
+-rw-r--r--  2.0 unx   611607 b- defN 23-Aug-08 06:13 xsl/pretext-html.xsl
+-rw-r--r--  2.0 unx    39918 b- defN 23-Aug-08 06:13 xsl/pretext-runestone-static.xsl
+-rw-r--r--  2.0 unx     9787 b- defN 23-Aug-08 06:13 xsl/entities.ent
+-rw-r--r--  2.0 unx     3239 b- defN 23-Aug-08 06:13 xsl/extract-interactive.xsl
+-rw-r--r--  2.0 unx   231265 b- defN 23-Aug-08 06:13 xsl/publisher-variables.xsl
+-rw-r--r--  2.0 unx     2709 b- defN 23-Aug-08 06:13 xsl/extract-qrcode.xsl
+-rw-r--r--  2.0 unx    13037 b- defN 23-Aug-08 06:13 xsl/pretext-text.xsl
+-rw-r--r--  2.0 unx    41730 b- defN 23-Aug-08 06:13 xsl/pretext-beamer.xsl
+-rw-r--r--  2.0 unx    43020 b- defN 23-Aug-08 06:13 xsl/pretext-text-utilities.xsl
+-rw-r--r--  2.0 unx     2601 b- defN 23-Aug-08 06:13 xsl/pretext-merge.xsl
+-rw-r--r--  2.0 unx   139486 b- defN 23-Aug-08 06:13 xsl/extract-pg.xsl
+-rw-r--r--  2.0 unx   116581 b- defN 23-Aug-08 06:13 xsl/pretext-assembly.xsl
+-rw-r--r--  2.0 unx     2846 b- defN 23-Aug-08 06:13 xsl/extract-datafile.xsl
+-rw-r--r--  2.0 unx     1768 b- defN 23-Aug-08 06:13 xsl/README.md
+-rw-r--r--  2.0 unx    13186 b- defN 23-Aug-08 06:13 xsl/pretext-solution-manual-latex.xsl
+-rw-r--r--  2.0 unx     6281 b- defN 23-Aug-08 06:13 xsl/pretext-numbers.xsl
+-rw-r--r--  2.0 unx     8535 b- defN 23-Aug-08 06:13 xsl/pretext-view-source.xsl
+-rw-r--r--  2.0 unx    12084 b- defN 23-Aug-08 06:13 xsl/xml-to-json.xsl
+-rw-r--r--  2.0 unx     8130 b- defN 23-Aug-08 06:13 xsl/extract-identity.xsl
+-rw-r--r--  2.0 unx    94587 b- defN 23-Aug-08 06:13 xsl/pretext-braille-preprint.xsl
+-rw-r--r--  2.0 unx   111515 b- defN 23-Aug-08 06:13 xsl/pretext-runestone.xsl
+-rw-r--r--  2.0 unx   545014 b- defN 23-Aug-08 06:13 xsl/pretext-latex.xsl
+-rw-r--r--  2.0 unx      787 b- defN 23-Aug-08 06:13 xsl/utilities/deprecate-index.sed
+-rw-r--r--  2.0 unx      513 b- defN 23-Aug-08 06:13 xsl/utilities/deprecate-autoname.sed
+-rw-r--r--  2.0 unx     4926 b- defN 23-Aug-08 06:13 xsl/utilities/pretext-enhanced-source.xsl
+-rw-r--r--  2.0 unx    30257 b- defN 23-Aug-08 06:13 xsl/utilities/fix-deprecations.xsl
+-rw-r--r--  2.0 unx     1810 b- defN 23-Aug-08 06:13 xsl/utilities/README.md
+-rw-r--r--  2.0 unx     4299 b- defN 23-Aug-08 06:13 xsl/utilities/author-report.xsl
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-08 06:13 xsl/support/play-button/
+-rw-r--r--  2.0 unx     5879 b- defN 23-Aug-08 06:13 xsl/support/package-math.xsl
+-rw-r--r--  2.0 unx     5241 b- defN 23-Aug-08 06:13 xsl/support/pretext-pg-macros.xsl
+-rw-r--r--  2.0 unx      486 b- defN 23-Aug-08 06:13 xsl/support/runestone-services.xml
+-rw-r--r--  2.0 unx    10306 b- defN 23-Aug-08 06:13 xsl/support/extract-math.xsl
+-rw-r--r--  2.0 unx     5065 b- defN 23-Aug-08 06:13 xsl/support/extract-latex-image-labels.xsl
+-rw-r--r--  2.0 unx      504 b- defN 23-Aug-08 06:13 xsl/support/README.md
+-rw-r--r--  2.0 unx     5800 b- defN 23-Aug-08 06:13 xsl/support/tactile-svg.xsl
+-rw-r--r--  2.0 unx      722 b- defN 23-Aug-08 06:13 xsl/support/play-button/play-button.svg
+-rw-r--r--  2.0 unx     2657 b- defN 23-Aug-08 06:13 xsl/support/play-button/README.md
+-rw-r--r--  2.0 unx     6621 b- defN 23-Aug-08 06:13 xsl/support/play-button/play-button.png
+-rw-r--r--  2.0 unx    17231 b- defN 23-Aug-08 06:13 xsl/localizations/de-DE.xml
+-rw-r--r--  2.0 unx    16312 b- defN 23-Aug-08 06:13 xsl/localizations/pt-BR.xml
+-rw-r--r--  2.0 unx     2286 b- defN 23-Aug-08 06:13 xsl/localizations/localizations.xml
+-rw-r--r--  2.0 unx    17301 b- defN 23-Aug-08 06:13 xsl/localizations/fi-FI.xml
+-rw-r--r--  2.0 unx    16349 b- defN 23-Aug-08 06:13 xsl/localizations/fr-FR.xml
+-rw-r--r--  2.0 unx    16534 b- defN 23-Aug-08 06:13 xsl/localizations/es-ES.xml
+-rw-r--r--  2.0 unx    16837 b- defN 23-Aug-08 06:13 xsl/localizations/af-ZA.xml
+-rw-r--r--  2.0 unx    19185 b- defN 23-Aug-08 06:13 xsl/localizations/nl-NL.xml
+-rw-r--r--  2.0 unx    16252 b- defN 23-Aug-08 06:13 xsl/localizations/ca-ES.xml
+-rw-r--r--  2.0 unx    17056 b- defN 23-Aug-08 06:13 xsl/localizations/bg-BG.xml
+-rw-r--r--  2.0 unx    17081 b- defN 23-Aug-08 06:13 xsl/localizations/pt-PT.xml
+-rw-r--r--  2.0 unx    15582 b- defN 23-Aug-08 06:13 xsl/localizations/cs-CZ.xml
+-rw-r--r--  2.0 unx    20481 b- defN 23-Aug-08 06:13 xsl/localizations/ku-CKB.xml
+-rw-r--r--  2.0 unx    19326 b- defN 23-Aug-08 06:13 xsl/localizations/en-US.xml
+-rw-r--r--  2.0 unx     4760 b- defN 23-Aug-08 06:13 xsl/localizations/README.md
+-rw-r--r--  2.0 unx    15866 b- defN 23-Aug-08 06:13 xsl/localizations/it-IT.xml
+-rw-r--r--  2.0 unx    16085 b- defN 23-Aug-08 06:13 xsl/localizations/hu-HU.xml
+-rw-r--r--  2.0 unx    16500 b- defN 23-Aug-08 06:13 xsl/localizations/fr-CA.xml
+-rw-r--r--  2.0 unx     5135 b- defN 23-Aug-08 06:13 xsl/latex/pretext-latex-guide.xsl
+-rw-r--r--  2.0 unx     2261 b- defN 23-Aug-08 06:13 xsl/latex/pretext-latex-AIM.xsl
+-rw-r--r--  2.0 unx    14482 b- defN 23-Aug-08 06:13 xsl/latex/pretext-latex-chaos.xsl
+-rw-r--r--  2.0 unx     7526 b- defN 23-Aug-08 06:13 xsl/latex/pretext-latex-CLP.xsl
+-rw-r--r--  2.0 unx     3024 b- defN 23-Aug-08 06:13 xsl/latex/pretext-latex-dyslexic-font.xsl
+142 files, 4852897 bytes uncompressed, 1028172 bytes compressed:  78.8%
```

#### schema/pretext.xml

##### schema/pretext.xml

```diff
@@ -1927,45 +1927,53 @@
     <section>
       <title>Figures, Tables, Listings and Named Lists</title>
       <p>
         These are containers that all carry titles (mandatory and optional), captions for two, and numbers.  They need to be filled with other (atomic) items, which we generally call
         <term>planar</term>
         due to their two-dimensional and rigid characteristics.  These have also called
         <term>captioned items</term>
-        in the code, even if not all allow a caption.
+        in the code, even if not all allow a caption.  The option for a lanscape orientation is only relevant for print, and not within a
+        <c>sidebyside</c>
+        .
       </p>
       <!-- 2021-12-29: should add audio and interacive to figure, once ready -->
       <fragment xml:id="table-figure">
         <title>Captioned and titled displays</title>
         <code>Caption =
                 element caption {TextLong}
+            Landscape =
+                attribute landscape {&quot;yes&quot; | &quot;no&quot;}
             Figure =
                 element figure {
                     MetaDataCaption,
+                    Landscape?,
                     (
                         Image |
                         Video |
                         SideBySide |
                         SideBySideGroup |
                         MuseScore
                     )
                 } |
                 element table {
                     MetaDataAltTitle,
+                    Landscape?,
                     Tabular
                 } |
                 element listing {
                     MetaDataCaption,
+                    Landscape?,
                     (
                         Program |
                         Console
                     )
                 } |
                 element list {
                     MetaDataAltTitle,
+                    Landscape?,
                     IntroductionText?,
                     List,
                     ConclusionText?
                 }</code>
       </fragment>
       <p>
         The guts of a table go in a
@@ -2163,14 +2171,15 @@
         <code>Image = ImageRaster | ImageCode
             ImageRaster =
                 element image {
                     UniqueID?,
                     PermanentID?,
                     attribute width {text}?,
                     attribute margins {text}?,
+                    attribute rotate {text}?,
                     attribute archive {text}?,
                     attribute source {text},
                     attribute decorative {&quot;yes&quot; | &quot;no&quot;}?,
                     element description {TextShort}?
                 }
             ImageCode =
                 element image {
```

#### schema/pretext.xsd

##### schema/pretext.xsd

```diff
@@ -1544,14 +1544,24 @@
     </xs:complexType>
   </xs:element>
   <xs:element name="caption">
     <xs:complexType mixed="true">
       <xs:group ref="TextLong"/>
     </xs:complexType>
   </xs:element>
+  <xs:attributeGroup name="Landscape">
+    <xs:attribute name="landscape" use="required">
+      <xs:simpleType>
+        <xs:restriction base="xs:token">
+          <xs:enumeration value="yes"/>
+          <xs:enumeration value="no"/>
+        </xs:restriction>
+      </xs:simpleType>
+    </xs:attribute>
+  </xs:attributeGroup>
   <xs:group name="Figure">
     <xs:choice>
       <xs:element ref="figure"/>
       <xs:element ref="table"/>
       <xs:element ref="listing"/>
       <xs:element ref="list"/>
     </xs:choice>
@@ -1563,50 +1573,82 @@
           <xs:choice>
             <xs:group ref="Image"/>
             <xs:element ref="video"/>
             <xs:group ref="SideBySide"/>
             <xs:group ref="SideBySideGroup"/>
             <xs:element ref="score"/>
           </xs:choice>
+          <xs:attribute name="landscape">
+            <xs:simpleType>
+              <xs:restriction base="xs:token">
+                <xs:enumeration value="yes"/>
+                <xs:enumeration value="no"/>
+              </xs:restriction>
+            </xs:simpleType>
+          </xs:attribute>
         </xs:extension>
       </xs:complexContent>
     </xs:complexType>
   </xs:element>
   <xs:element name="table">
     <xs:complexType>
       <xs:complexContent>
         <xs:extension base="MetaDataAltTitle">
           <xs:sequence>
             <xs:element ref="tabular"/>
           </xs:sequence>
+          <xs:attribute name="landscape">
+            <xs:simpleType>
+              <xs:restriction base="xs:token">
+                <xs:enumeration value="yes"/>
+                <xs:enumeration value="no"/>
+              </xs:restriction>
+            </xs:simpleType>
+          </xs:attribute>
         </xs:extension>
       </xs:complexContent>
     </xs:complexType>
   </xs:element>
   <xs:element name="listing">
     <xs:complexType>
       <xs:complexContent>
         <xs:extension base="MetaDataCaption">
           <xs:choice>
             <xs:element ref="program"/>
             <xs:element ref="console"/>
           </xs:choice>
+          <xs:attribute name="landscape">
+            <xs:simpleType>
+              <xs:restriction base="xs:token">
+                <xs:enumeration value="yes"/>
+                <xs:enumeration value="no"/>
+              </xs:restriction>
+            </xs:simpleType>
+          </xs:attribute>
         </xs:extension>
       </xs:complexContent>
     </xs:complexType>
   </xs:element>
   <xs:element name="list">
     <xs:complexType>
       <xs:complexContent>
         <xs:extension base="MetaDataAltTitle">
           <xs:sequence>
             <xs:group minOccurs="0" ref="IntroductionText"/>
             <xs:group ref="List"/>
             <xs:group minOccurs="0" ref="ConclusionText"/>
           </xs:sequence>
+          <xs:attribute name="landscape">
+            <xs:simpleType>
+              <xs:restriction base="xs:token">
+                <xs:enumeration value="yes"/>
+                <xs:enumeration value="no"/>
+              </xs:restriction>
+            </xs:simpleType>
+          </xs:attribute>
         </xs:extension>
       </xs:complexContent>
     </xs:complexType>
   </xs:element>
   <xs:element name="stack">
     <xs:complexType>
       <xs:choice maxOccurs="unbounded">
@@ -1717,14 +1759,15 @@
               </xs:complexType>
             </xs:element>
           </xs:sequence>
           <xs:attribute ref="xml:id"/>
           <xs:attribute name="permid"/>
           <xs:attribute name="width"/>
           <xs:attribute name="margins"/>
+          <xs:attribute name="rotate"/>
           <xs:attribute name="archive"/>
           <xs:attribute name="source" use="required"/>
           <xs:attribute name="decorative">
             <xs:simpleType>
               <xs:restriction base="xs:token">
                 <xs:enumeration value="yes"/>
                 <xs:enumeration value="no"/>
```

#### schema/pretext.rnc

```diff
@@ -651,38 +651,44 @@
                 element assemblage {
                     MetaDataTitleOptional,
                     (BlockText | SideBySideNoCaption | SideBySideGroupNoCaption)+
                 }
             
             Caption =
                 element caption {TextLong}
+            Landscape =
+                attribute landscape {"yes" | "no"}
             Figure =
                 element figure {
                     MetaDataCaption,
+                    Landscape?,
                     (
                         Image |
                         Video |
                         SideBySide |
                         SideBySideGroup |
                         MuseScore
                     )
                 } |
                 element table {
                     MetaDataAltTitle,
+                    Landscape?,
                     Tabular
                 } |
                 element listing {
                     MetaDataCaption,
+                    Landscape?,
                     (
                         Program |
                         Console
                     )
                 } |
                 element list {
                     MetaDataAltTitle,
+                    Landscape?,
                     IntroductionText?,
                     List,
                     ConclusionText?
                 }
             
             Stack =
                 element stack {
@@ -749,14 +755,15 @@
             Image = ImageRaster | ImageCode
             ImageRaster =
                 element image {
                     UniqueID?,
                     PermanentID?,
                     attribute width {text}?,
                     attribute margins {text}?,
+                    attribute rotate {text}?,
                     attribute archive {text}?,
                     attribute source {text},
                     attribute decorative {"yes" | "no"}?,
                     element description {TextShort}?
                 }
             ImageCode =
                 element image {
```

#### schema/pretext.rng

##### schema/pretext.rng

```diff
@@ -1751,40 +1751,60 @@
     </element>
   </define>
   <define name="Caption">
     <element name="caption">
       <ref name="TextLong"/>
     </element>
   </define>
+  <define name="Landscape">
+    <attribute name="landscape">
+      <choice>
+        <value>yes</value>
+        <value>no</value>
+      </choice>
+    </attribute>
+  </define>
   <define name="Figure">
     <choice>
       <element name="figure">
         <ref name="MetaDataCaption"/>
+        <optional>
+          <ref name="Landscape"/>
+        </optional>
         <choice>
           <ref name="Image"/>
           <ref name="Video"/>
           <ref name="SideBySide"/>
           <ref name="SideBySideGroup"/>
           <ref name="MuseScore"/>
         </choice>
       </element>
       <element name="table">
         <ref name="MetaDataAltTitle"/>
+        <optional>
+          <ref name="Landscape"/>
+        </optional>
         <ref name="Tabular"/>
       </element>
       <element name="listing">
         <ref name="MetaDataCaption"/>
+        <optional>
+          <ref name="Landscape"/>
+        </optional>
         <choice>
           <ref name="Program"/>
           <ref name="Console"/>
         </choice>
       </element>
       <element name="list">
         <ref name="MetaDataAltTitle"/>
         <optional>
+          <ref name="Landscape"/>
+        </optional>
+        <optional>
           <ref name="IntroductionText"/>
         </optional>
         <ref name="List"/>
         <optional>
           <ref name="ConclusionText"/>
         </optional>
       </element>
@@ -1898,14 +1918,17 @@
       <optional>
         <attribute name="width"/>
       </optional>
       <optional>
         <attribute name="margins"/>
       </optional>
       <optional>
+        <attribute name="rotate"/>
+      </optional>
+      <optional>
         <attribute name="archive"/>
       </optional>
       <attribute name="source"/>
       <optional>
         <attribute name="decorative">
           <choice>
             <value>yes</value>
```

#### xsl/pretext-html.xsl

##### xsl/pretext-html.xsl

```diff
@@ -5930,14 +5930,21 @@
             </xsl:when>
             <xsl:when test="not(string(description) = '')">
               <xsl:attribute name="alt">
                 <xsl:apply-templates select="description"/>
               </xsl:attribute>
             </xsl:when>
           </xsl:choose>
+          <xsl:if test="@rotate">
+            <xsl:attribute name="style">
+              <xsl:text>transform: rotate(</xsl:text>
+              <xsl:value-of select="@rotate"/>
+              <xsl:text>deg)</xsl:text>
+            </xsl:attribute>
+          </xsl:if>
         </img>
         <!-- possibly annotate with archive links -->
         <xsl:apply-templates select="." mode="archive">
           <xsl:with-param name="base-pathname">
             <!-- empty when not using managed directories -->
             <xsl:value-of select="$external-directory"/>
             <xsl:call-template name="substring-before-last">
```

#### xsl/pretext-latex.xsl

##### xsl/pretext-latex.xsl

```diff
@@ -1547,14 +1547,18 @@
       </xsl:if>
     </xsl:if>
     <!-- TODO:  \showidx package as part of a draft mode, prints entries in margin -->
     <xsl:if test="$document-root//ol[@cols]|$document-root//ul[@cols]|$document-root//contributors">
       <xsl:text>%% Multiple column, column-major lists</xsl:text>
       <xsl:text>\usepackage{multicol}</xsl:text>
     </xsl:if>
+    <xsl:if test="$document-root//@landscape">
+      <xsl:text>%% The rotating package provides sidewaysfigure and sidewaystables environments</xsl:text>
+      <xsl:text>\usepackage{rotating}</xsl:text>
+    </xsl:if>
     <xsl:if test="$document-root//ol or $document-root//ul or $document-root//task or $document-root//references or $b-has-webwork-var">
       <xsl:text>%% More flexible list management, esp. for references</xsl:text>
       <xsl:text>%% But also for specifying labels (i.e. custom order) on nested lists</xsl:text>
       <xsl:text>\usepackage</xsl:text>
       <!-- next test is simpler than necessary, only needed for 'popup' versions of @form -->
       <xsl:if test="$b-has-webwork-var">
         <xsl:text>[inline]</xsl:text>
@@ -7982,14 +7986,17 @@
   </xsl:template>
   <!-- Figures, Listings -->
   <!-- 0: enviroment name may be prefixed with "sub" -->
   <!-- 1: caption text                               -->
   <!-- 2: standard identifier for cross-references   -->
   <!-- 3: empty, or a hard-coded number from -common -->
   <xsl:template match="figure|listing">
+    <xsl:if test="@landscape and $b-latex-print">
+      <xsl:text>\begin{sidewaysfigure}%</xsl:text>
+    </xsl:if>
     <xsl:text>\begin{</xsl:text>
     <xsl:apply-templates select="." mode="environment-name"/>
     <xsl:text>}{</xsl:text>
     <xsl:apply-templates select="." mode="type-name"/>
     <xsl:text>}{</xsl:text>
     <xsl:apply-templates select="." mode="caption-full"/>
     <xsl:text>}{</xsl:text>
@@ -8010,22 +8017,28 @@
     <!-- multiple, program|console                       -->
     <xsl:apply-templates select="*"/>
     <!-- reserve space for the caption -->
     <xsl:text>\tcblower</xsl:text>
     <xsl:text>\end{</xsl:text>
     <xsl:apply-templates select="." mode="environment-name"/>
     <xsl:text>}%</xsl:text>
+    <xsl:if test="@landscape and $b-latex-print">
+      <xsl:text>\end{sidewaysfigure}%</xsl:text>
+    </xsl:if>
     <xsl:apply-templates select="." mode="pop-footnote-text"/>
   </xsl:template>
   <!-- Tables, (Named) Lists -->
   <!-- 0: enviroment name may be prefixed with "sub"  -->
   <!-- 1: title text, bolded here, not in environment -->
   <!-- 2: standard identifier for cross-references    -->
   <!-- 3: empty, or a hard-coded number from -common  -->
   <xsl:template match="table|list">
+    <xsl:if test="@landscape and $b-latex-print">
+      <xsl:text>\begin{sidewaystable}%</xsl:text>
+    </xsl:if>
     <xsl:text>\begin{</xsl:text>
     <xsl:apply-templates select="." mode="environment-name"/>
     <xsl:text>}{</xsl:text>
     <xsl:apply-templates select="." mode="type-name"/>
     <xsl:text>}{</xsl:text>
     <xsl:text>\textbf{</xsl:text>
     <xsl:apply-templates select="." mode="title-full"/>
@@ -8049,14 +8062,17 @@
     <!-- title goes in lower part when in a sidebyside -->
     <xsl:if test="($fig-placement = 'subnumber') or ($fig-placement = 'panel')">
       <xsl:text>\tcblower</xsl:text>
     </xsl:if>
     <xsl:text>\end{</xsl:text>
     <xsl:apply-templates select="." mode="environment-name"/>
     <xsl:text>}%</xsl:text>
+    <xsl:if test="@landscape and $b-latex-print">
+      <xsl:text>\end{sidewaystable}%</xsl:text>
+    </xsl:if>
     <xsl:apply-templates select="." mode="pop-footnote-text"/>
   </xsl:template>
   <!-- ################## -->
   <!-- SideBySide Layouts -->
   <!-- ################## -->
   <!-- See xsl/pretext-common.xsl for descriptions of the  -->
   <!-- four modal templates which must be implemented here  -->
@@ -8180,16 +8196,21 @@
             <xsl:otherwise>
               <xsl:value-of select="@source"/>
             </xsl:otherwise>
           </xsl:choose>
         </xsl:with-param>
       </xsl:call-template>
     </xsl:variable>
-    <xsl:text>\includegraphics[width=\linewidth]</xsl:text>
-    <xsl:text>{</xsl:text>
+    <xsl:text>\includegraphics[width=\linewidth</xsl:text>
+    <xsl:if test="@rotate">
+      <xsl:text>,angle=</xsl:text>
+      <xsl:value-of select="@rotate"/>
+      <xsl:text>,origin=c</xsl:text>
+    </xsl:if>
+    <xsl:text>]{</xsl:text>
     <xsl:choose>
       <xsl:when test="@pi:generated">
         <xsl:value-of select="$generated-directory"/>
         <xsl:value-of select="@pi:generated"/>
       </xsl:when>
       <xsl:otherwise>
         <!-- empty when not using managed directories -->
```

### Comparing `pretext-1.7.6.dev20230806/pretext/generate.py` & `pretext-1.7.6.dev20230808/pretext/generate.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.6.dev20230806/pretext/project/__init__.py` & `pretext-1.7.6.dev20230808/pretext/project/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.6.dev20230806/pretext/project/refactor.py` & `pretext-1.7.6.dev20230808/pretext/project/refactor.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.6.dev20230806/pretext/project/xml.py` & `pretext-1.7.6.dev20230808/pretext/project/xml.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.6.dev20230806/pretext/templates/__init__.py` & `pretext-1.7.6.dev20230808/pretext/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.6.dev20230806/pretext/templates/resources/.devcontainer.json` & `pretext-1.7.6.dev20230808/pretext/templates/resources/.devcontainer.json`

 * *Files identical despite different names*

### Comparing `pretext-1.7.6.dev20230806/pretext/templates/resources/.gitignore` & `pretext-1.7.6.dev20230808/pretext/templates/resources/.gitignore`

 * *Files identical despite different names*

### Comparing `pretext-1.7.6.dev20230806/pretext/templates/resources/article.zip` & `pretext-1.7.6.dev20230808/pretext/templates/resources/article.zip`

 * *Files 2% similar despite different names*

#### zipinfo {}

```diff
@@ -1,14 +1,14 @@
 Zip file size: 158949 bytes, number of entries: 12
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-06 06:12 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-06 06:12 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-06 06:12 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Aug-06 06:13 .gitignore
--rw-r--r--  2.0 unx     1710 b- defN 23-Aug-06 06:13 project.ptx
--rw-r--r--  2.0 unx     2538 b- defN 23-Aug-06 06:13 codechat_config.yaml
--rw-r--r--  2.0 unx       86 b- defN 23-Aug-06 06:12 README.md
--rw-r--r--  2.0 unx      449 b- defN 23-Aug-06 06:12 source/section-1.ptx
--rw-r--r--  2.0 unx      982 b- defN 23-Aug-06 06:12 source/section-2.ptx
--rw-r--r--  2.0 unx      430 b- defN 23-Aug-06 06:12 source/main.ptx
--rw-r--r--  2.0 unx   154806 b- defN 23-Aug-06 06:12 assets/frog.jpg
--rw-r--r--  2.0 unx      242 b- defN 23-Aug-06 06:12 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-08 06:13 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-08 06:13 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-08 06:13 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Aug-08 06:13 .gitignore
+-rw-r--r--  2.0 unx     1710 b- defN 23-Aug-08 06:13 project.ptx
+-rw-r--r--  2.0 unx     2538 b- defN 23-Aug-08 06:13 codechat_config.yaml
+-rw-r--r--  2.0 unx       86 b- defN 23-Aug-08 06:13 README.md
+-rw-r--r--  2.0 unx      449 b- defN 23-Aug-08 06:13 source/section-1.ptx
+-rw-r--r--  2.0 unx      982 b- defN 23-Aug-08 06:13 source/section-2.ptx
+-rw-r--r--  2.0 unx      430 b- defN 23-Aug-08 06:13 source/main.ptx
+-rw-r--r--  2.0 unx   154806 b- defN 23-Aug-08 06:13 assets/frog.jpg
+-rw-r--r--  2.0 unx      242 b- defN 23-Aug-08 06:13 publication/publication.ptx
 12 files, 162919 bytes uncompressed, 157669 bytes compressed:  3.2%
```

### Comparing `pretext-1.7.6.dev20230806/pretext/templates/resources/book.zip` & `pretext-1.7.6.dev20230808/pretext/templates/resources/book.zip`

 * *Files 11% similar despite different names*

#### zipinfo {}

```diff
@@ -1,10 +1,10 @@
 Zip file size: 6455 bytes, number of entries: 8
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-06 06:12 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-06 06:12 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Aug-06 06:13 .gitignore
--rw-r--r--  2.0 unx     1710 b- defN 23-Aug-06 06:13 project.ptx
--rw-r--r--  2.0 unx     2538 b- defN 23-Aug-06 06:13 codechat_config.yaml
--rw-r--r--  2.0 unx       82 b- defN 23-Aug-06 06:12 README.md
--rw-r--r--  2.0 unx     1767 b- defN 23-Aug-06 06:12 source/main.ptx
--rw-r--r--  2.0 unx     6114 b- defN 23-Aug-06 06:12 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-08 06:13 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-08 06:13 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Aug-08 06:13 .gitignore
+-rw-r--r--  2.0 unx     1710 b- defN 23-Aug-08 06:13 project.ptx
+-rw-r--r--  2.0 unx     2538 b- defN 23-Aug-08 06:13 codechat_config.yaml
+-rw-r--r--  2.0 unx       82 b- defN 23-Aug-08 06:13 README.md
+-rw-r--r--  2.0 unx     1767 b- defN 23-Aug-08 06:13 source/main.ptx
+-rw-r--r--  2.0 unx     6114 b- defN 23-Aug-08 06:13 publication/publication.ptx
 8 files, 13887 bytes uncompressed, 5603 bytes compressed:  59.7%
```

### Comparing `pretext-1.7.6.dev20230806/pretext/templates/resources/demo.zip` & `pretext-1.7.6.dev20230808/pretext/templates/resources/demo.zip`

 * *Files 6% similar despite different names*

#### zipinfo {}

```diff
@@ -1,35 +1,35 @@
 Zip file size: 172278 bytes, number of entries: 33
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-06 06:12 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-06 06:12 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-06 06:12 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Aug-06 06:13 .gitignore
--rw-r--r--  2.0 unx     1710 b- defN 23-Aug-06 06:13 project.ptx
--rw-r--r--  2.0 unx     2538 b- defN 23-Aug-06 06:13 codechat_config.yaml
--rw-r--r--  2.0 unx       82 b- defN 23-Aug-06 06:12 README.md
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-06 06:12 source/images/
--rw-r--r--  2.0 unx      339 b- defN 23-Aug-06 06:12 source/ch-features.ptx
--rw-r--r--  2.0 unx     1697 b- defN 23-Aug-06 06:12 source/sec-first-examples.ptx
--rw-r--r--  2.0 unx      375 b- defN 23-Aug-06 06:12 source/fig-sage2d.ptx
--rw-r--r--  2.0 unx      885 b- defN 23-Aug-06 06:12 source/backmatter.ptx
--rw-r--r--  2.0 unx      867 b- defN 23-Aug-06 06:12 source/sec-features.ptx
--rw-r--r--  2.0 unx     2295 b- defN 23-Aug-06 06:12 source/ch-generate.ptx
--rw-r--r--  2.0 unx      335 b- defN 23-Aug-06 06:12 source/fig-asymptote.ptx
--rw-r--r--  2.0 unx     2080 b- defN 23-Aug-06 06:12 source/frontmatter.ptx
--rw-r--r--  2.0 unx      381 b- defN 23-Aug-06 06:12 source/fig-tikz.ptx
--rw-r--r--  2.0 unx      230 b- defN 23-Aug-06 06:12 source/ch-empty.ptx
--rw-r--r--  2.0 unx      847 b- defN 23-Aug-06 06:12 source/sec-first-intro.ptx
--rw-r--r--  2.0 unx     1515 b- defN 23-Aug-06 06:12 source/ex-first.ptx
--rw-r--r--  2.0 unx      777 b- defN 23-Aug-06 06:12 source/ww.ptx
--rw-r--r--  2.0 unx      411 b- defN 23-Aug-06 06:12 source/fig-sage3d.ptx
--rw-r--r--  2.0 unx     1115 b- defN 23-Aug-06 06:12 source/ch-first with spaces.ptx
--rw-r--r--  2.0 unx     1616 b- defN 23-Aug-06 06:12 source/docinfo.ptx
--rw-r--r--  2.0 unx     2428 b- defN 23-Aug-06 06:12 source/main.ptx
--rw-r--r--  2.0 unx      835 b- defN 23-Aug-06 06:12 source/images/cflag.asy
--rw-r--r--  2.0 unx       93 b- defN 23-Aug-06 06:12 source/images/sageplot3d.sage
--rw-r--r--  2.0 unx      357 b- defN 23-Aug-06 06:12 source/images/tikz.tex
--rw-r--r--  2.0 unx       10 b- defN 23-Aug-06 06:12 source/images/sageplot2d.sage
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-06 06:12 assets/jsxgraph/
--rw-r--r--  2.0 unx   154806 b- defN 23-Aug-06 06:12 assets/frog.jpg
--rw-r--r--  2.0 unx     1737 b- defN 23-Aug-06 06:12 assets/jsxgraph/infinity.js
--rw-r--r--  2.0 unx     6092 b- defN 23-Aug-06 06:12 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-08 06:13 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-08 06:13 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-08 06:13 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Aug-08 06:13 .gitignore
+-rw-r--r--  2.0 unx     1710 b- defN 23-Aug-08 06:13 project.ptx
+-rw-r--r--  2.0 unx     2538 b- defN 23-Aug-08 06:13 codechat_config.yaml
+-rw-r--r--  2.0 unx       82 b- defN 23-Aug-08 06:13 README.md
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-08 06:13 source/images/
+-rw-r--r--  2.0 unx      339 b- defN 23-Aug-08 06:13 source/ch-features.ptx
+-rw-r--r--  2.0 unx     1697 b- defN 23-Aug-08 06:13 source/sec-first-examples.ptx
+-rw-r--r--  2.0 unx      375 b- defN 23-Aug-08 06:13 source/fig-sage2d.ptx
+-rw-r--r--  2.0 unx      885 b- defN 23-Aug-08 06:13 source/backmatter.ptx
+-rw-r--r--  2.0 unx      867 b- defN 23-Aug-08 06:13 source/sec-features.ptx
+-rw-r--r--  2.0 unx     2295 b- defN 23-Aug-08 06:13 source/ch-generate.ptx
+-rw-r--r--  2.0 unx      335 b- defN 23-Aug-08 06:13 source/fig-asymptote.ptx
+-rw-r--r--  2.0 unx     2080 b- defN 23-Aug-08 06:13 source/frontmatter.ptx
+-rw-r--r--  2.0 unx      381 b- defN 23-Aug-08 06:13 source/fig-tikz.ptx
+-rw-r--r--  2.0 unx      230 b- defN 23-Aug-08 06:13 source/ch-empty.ptx
+-rw-r--r--  2.0 unx      847 b- defN 23-Aug-08 06:13 source/sec-first-intro.ptx
+-rw-r--r--  2.0 unx     1515 b- defN 23-Aug-08 06:13 source/ex-first.ptx
+-rw-r--r--  2.0 unx      777 b- defN 23-Aug-08 06:13 source/ww.ptx
+-rw-r--r--  2.0 unx      411 b- defN 23-Aug-08 06:13 source/fig-sage3d.ptx
+-rw-r--r--  2.0 unx     1115 b- defN 23-Aug-08 06:13 source/ch-first with spaces.ptx
+-rw-r--r--  2.0 unx     1616 b- defN 23-Aug-08 06:13 source/docinfo.ptx
+-rw-r--r--  2.0 unx     2428 b- defN 23-Aug-08 06:13 source/main.ptx
+-rw-r--r--  2.0 unx      835 b- defN 23-Aug-08 06:13 source/images/cflag.asy
+-rw-r--r--  2.0 unx       93 b- defN 23-Aug-08 06:13 source/images/sageplot3d.sage
+-rw-r--r--  2.0 unx      357 b- defN 23-Aug-08 06:13 source/images/tikz.tex
+-rw-r--r--  2.0 unx       10 b- defN 23-Aug-08 06:13 source/images/sageplot2d.sage
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-08 06:13 assets/jsxgraph/
+-rw-r--r--  2.0 unx   154806 b- defN 23-Aug-08 06:13 assets/frog.jpg
+-rw-r--r--  2.0 unx     1737 b- defN 23-Aug-08 06:13 assets/jsxgraph/infinity.js
+-rw-r--r--  2.0 unx     6092 b- defN 23-Aug-08 06:13 publication/publication.ptx
 33 files, 188129 bytes uncompressed, 168462 bytes compressed:  10.5%
```

### Comparing `pretext-1.7.6.dev20230806/pretext/templates/resources/hello.zip` & `pretext-1.7.6.dev20230808/pretext/templates/resources/hello.zip`

 * *Files 14% similar despite different names*

#### zipinfo {}

```diff
@@ -1,10 +1,10 @@
 Zip file size: 3496 bytes, number of entries: 8
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-06 06:12 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-06 06:12 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Aug-06 06:13 .gitignore
--rw-r--r--  2.0 unx     1217 b- defN 23-Aug-06 06:12 project.ptx
--rw-r--r--  2.0 unx     2538 b- defN 23-Aug-06 06:13 codechat_config.yaml
--rw-r--r--  2.0 unx       69 b- defN 23-Aug-06 06:12 README.md
--rw-r--r--  2.0 unx      156 b- defN 23-Aug-06 06:12 source/main.ptx
--rw-r--r--  2.0 unx      242 b- defN 23-Aug-06 06:12 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-08 06:13 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-08 06:13 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Aug-08 06:13 .gitignore
+-rw-r--r--  2.0 unx     1217 b- defN 23-Aug-08 06:13 project.ptx
+-rw-r--r--  2.0 unx     2538 b- defN 23-Aug-08 06:13 codechat_config.yaml
+-rw-r--r--  2.0 unx       69 b- defN 23-Aug-08 06:13 README.md
+-rw-r--r--  2.0 unx      156 b- defN 23-Aug-08 06:13 source/main.ptx
+-rw-r--r--  2.0 unx      242 b- defN 23-Aug-08 06:13 publication/publication.ptx
 8 files, 5898 bytes uncompressed, 2644 bytes compressed:  55.2%
```

### Comparing `pretext-1.7.6.dev20230806/pretext/templates/resources/project.ptx` & `pretext-1.7.6.dev20230808/pretext/templates/resources/project.ptx`

 * *Files identical despite different names*

### Comparing `pretext-1.7.6.dev20230806/pretext/templates/resources/slideshow.zip` & `pretext-1.7.6.dev20230808/pretext/templates/resources/slideshow.zip`

 * *Files 9% similar despite different names*

#### zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 7231 bytes, number of entries: 9
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-06 06:12 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-06 06:12 source/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-06 06:12 xsl/
--rw-r--r--  2.0 unx     1676 b- defN 23-Aug-06 06:13 .gitignore
--rw-r--r--  2.0 unx      784 b- defN 23-Aug-06 06:12 project.ptx
--rw-r--r--  2.0 unx     2538 b- defN 23-Aug-06 06:13 codechat_config.yaml
--rw-r--r--  2.0 unx    11200 b- defN 23-Aug-06 06:12 source/main.ptx
--rw-r--r--  2.0 unx     2097 b- defN 23-Aug-06 06:12 publication/publication.ptx
--rw-r--r--  2.0 unx      190 b- defN 23-Aug-06 06:12 xsl/slides.xsl
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-08 06:13 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-08 06:13 source/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-08 06:13 xsl/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Aug-08 06:13 .gitignore
+-rw-r--r--  2.0 unx      784 b- defN 23-Aug-08 06:13 project.ptx
+-rw-r--r--  2.0 unx     2538 b- defN 23-Aug-08 06:13 codechat_config.yaml
+-rw-r--r--  2.0 unx    11200 b- defN 23-Aug-08 06:13 source/main.ptx
+-rw-r--r--  2.0 unx     2097 b- defN 23-Aug-08 06:13 publication/publication.ptx
+-rw-r--r--  2.0 unx      190 b- defN 23-Aug-08 06:13 xsl/slides.xsl
 9 files, 18485 bytes uncompressed, 6285 bytes compressed:  66.0%
```

### Comparing `pretext-1.7.6.dev20230806/pretext/utils.py` & `pretext-1.7.6.dev20230808/pretext/utils.py`

 * *Files identical despite different names*

### Comparing `pretext-1.7.6.dev20230806/pyproject.toml` & `pretext-1.7.6.dev20230808/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # See https://python-poetry.org/docs/dependency-specification/ to get an understanding of
 # how poetry specifies dependencies.
 #
 # Project metadata
 # ----------------
 [tool.poetry]
 name = "pretext"
-version = "1.7.6.dev20230806"
+version = "1.7.6.dev20230808"
 description = "A package to author, build, and deploy PreTeXt projects."
 readme = "README.md"
 homepage = "https://pretextbook.org"
 repository = "https://github.com/PreTeXtBook/pretext-cli"
 authors = ["Oscar Levin <oscar.levin@unco.edu>", "Steven Clontz <steven.clontz@gmail.com>",]
 license = "GPL-3.0-or-later"
 include = [
```

### Comparing `pretext-1.7.6.dev20230806/PKG-INFO` & `pretext-1.7.6.dev20230808/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretext
-Version: 1.7.6.dev20230806
+Version: 1.7.6.dev20230808
 Summary: A package to author, build, and deploy PreTeXt projects.
 Home-page: https://pretextbook.org
 License: GPL-3.0-or-later
 Author: Oscar Levin
 Author-email: oscar.levin@unco.edu
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

