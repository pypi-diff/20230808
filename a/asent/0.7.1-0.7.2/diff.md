# Comparing `tmp/asent-0.7.1.tar.gz` & `tmp/asent-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asent-0.7.1.tar", last modified: Wed Mar  8 12:17:12 2023, max compression
+gzip compressed data, was "asent-0.7.2.tar", last modified: Tue Aug  8 09:01:50 2023, max compression
```

## Comparing `asent-0.7.1.tar` & `asent-0.7.2.tar`

### file list

```diff
@@ -1,186 +1,186 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 12:17:12.429670 asent-0.7.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 12:17:12.389670 asent-0.7.1/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 12:17:12.389670 asent-0.7.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      716 2023-03-08 12:17:00.000000 asent-0.7.1/.github/ISSUE_TEMPLATE/01_bugs.md
--rw-r--r--   0 root         (0) root         (0)      418 2023-03-08 12:17:00.000000 asent-0.7.1/.github/ISSUE_TEMPLATE/02_docs.md
--rw-r--r--   0 root         (0) root         (0)      291 2023-03-08 12:17:00.000000 asent-0.7.1/.github/ISSUE_TEMPLATE/03_feature-request.md
--rw-r--r--   0 root         (0) root         (0)      597 2023-03-08 12:17:00.000000 asent-0.7.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 root         (0) root         (0)      776 2023-03-08 12:17:00.000000 asent-0.7.1/.github/dependabot.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 12:17:12.393670 asent-0.7.1/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1013 2023-03-08 12:17:00.000000 asent-0.7.1/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)     1143 2023-03-08 12:17:00.000000 asent-0.7.1/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)     1673 2023-03-08 12:17:00.000000 asent-0.7.1/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)      867 2023-03-08 12:17:00.000000 asent-0.7.1/.github/workflows/stale.yml
--rw-r--r--   0 root         (0) root         (0)     2810 2023-03-08 12:17:00.000000 asent-0.7.1/.github/workflows/tests.yml
--rw-r--r--   0 root         (0) root         (0)      324 2023-03-08 12:17:00.000000 asent-0.7.1/.gitignore
--rw-r--r--   0 root         (0) root         (0)      732 2023-03-08 12:17:00.000000 asent-0.7.1/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)     2006 2023-03-08 12:17:01.000000 asent-0.7.1/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1075 2023-03-08 12:17:00.000000 asent-0.7.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8023 2023-03-08 12:17:12.429670 asent-0.7.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5409 2023-03-08 12:17:00.000000 asent-0.7.1/README.md
--rw-r--r--   0 root         (0) root         (0)      378 2023-03-08 12:17:00.000000 asent-0.7.1/citation.cff
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 12:17:12.393670 asent-0.7.1/dev/
--rw-r--r--   0 root         (0) root         (0)     1064 2023-03-08 12:17:00.000000 asent-0.7.1/dev/add_new_language.py
--rw-r--r--   0 root         (0) root         (0)     1588 2023-03-08 12:17:00.000000 asent-0.7.1/dev/emoji_sentiment_creator.py
--rwxr-xr-x   0 root         (0) root         (0)   118417 2023-03-08 12:17:00.000000 asent-0.7.1/dev/emoji_utf8_lexicon.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 12:17:12.393670 asent-0.7.1/docs/
--rw-r--r--   0 root         (0) root         (0)      633 2023-03-08 12:17:00.000000 asent-0.7.1/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 12:17:12.393670 asent-0.7.1/docs/_static/
--rw-r--r--   0 root         (0) root         (0)    15406 2023-03-08 12:17:00.000000 asent-0.7.1/docs/_static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)    33247 2023-03-08 12:17:00.000000 asent-0.7.1/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)    33481 2023-03-08 12:17:00.000000 asent-0.7.1/docs/_static/icon_dark.png
--rw-r--r--   0 root         (0) root         (0)      518 2023-03-08 12:17:00.000000 asent-0.7.1/docs/asent.component.rst
--rw-r--r--   0 root         (0) root         (0)      343 2023-03-08 12:17:00.000000 asent-0.7.1/docs/asent.getters.rst
--rw-r--r--   0 root         (0) root         (0)      352 2023-03-08 12:17:00.000000 asent-0.7.1/docs/asent.visualize.rst
--rw-r--r--   0 root         (0) root         (0)     4185 2023-03-08 12:17:00.000000 asent-0.7.1/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)    11750 2023-03-08 12:17:00.000000 asent-0.7.1/docs/customizing.rst
--rw-r--r--   0 root         (0) root         (0)     2918 2023-03-08 12:17:00.000000 asent-0.7.1/docs/faq.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 12:17:12.397670 asent-0.7.1/docs/img/
--rw-r--r--   0 root         (0) root         (0)   299111 2023-03-08 12:17:00.000000 asent-0.7.1/docs/img/Screenshot 2021-12-07 at 20.46.02.png
--rw-r--r--   0 root         (0) root         (0)   129366 2023-03-08 12:17:00.000000 asent-0.7.1/docs/img/dep_parse.png
--rw-r--r--   0 root         (0) root         (0)   143218 2023-03-08 12:17:00.000000 asent-0.7.1/docs/img/doc_polarity.png
--rw-r--r--   0 root         (0) root         (0)    11937 2023-03-08 12:17:00.000000 asent-0.7.1/docs/img/icon.png
--rw-r--r--   0 root         (0) root         (0)    29045 2023-03-08 12:17:00.000000 asent-0.7.1/docs/img/logo_black_font.png
--rw-r--r--   0 root         (0) root         (0)    33481 2023-03-08 12:17:00.000000 asent-0.7.1/docs/img/logo_dark.png
--rw-r--r--   0 root         (0) root         (0)    33247 2023-03-08 12:17:00.000000 asent-0.7.1/docs/img/logo_red_font.png
--rw-r--r--   0 root         (0) root         (0)    37494 2023-03-08 12:17:00.000000 asent-0.7.1/docs/img/model_analysis.png
--rw-r--r--   0 root         (0) root         (0)    37494 2023-03-08 12:17:00.000000 asent-0.7.1/docs/img/model_analysis1.png
--rw-r--r--   0 root         (0) root         (0)    11308 2023-03-08 12:17:00.000000 asent-0.7.1/docs/img/model_pred.png
--rw-r--r--   0 root         (0) root         (0)    16270 2023-03-08 12:17:00.000000 asent-0.7.1/docs/img/model_pred_sv.png
--rw-r--r--   0 root         (0) root         (0)     9602 2023-03-08 12:17:00.000000 asent-0.7.1/docs/img/model_pred_sv1.png
--rw-r--r--   0 root         (0) root         (0)    16771 2023-03-08 12:17:00.000000 asent-0.7.1/docs/img/model_pred_sv2.png
--rw-r--r--   0 root         (0) root         (0)   184712 2023-03-08 12:17:00.000000 asent-0.7.1/docs/img/token_polarity.png
--rw-r--r--   0 root         (0) root         (0)     1375 2023-03-08 12:17:00.000000 asent-0.7.1/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      582 2023-03-08 12:17:00.000000 asent-0.7.1/docs/installation.rst
--rw-r--r--   0 root         (0) root         (0)     8116 2023-03-08 12:17:00.000000 asent-0.7.1/docs/introduction.rst
--rw-r--r--   0 root         (0) root         (0)    81205 2023-03-08 12:17:00.000000 asent-0.7.1/docs/languages.rst
--rw-r--r--   0 root         (0) root         (0)     2296 2023-03-08 12:17:00.000000 asent-0.7.1/docs/news.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 12:17:12.397670 asent-0.7.1/docs/tutorials/
--rw-r--r--   0 root         (0) root         (0)    46116 2023-03-08 12:17:00.000000 asent-0.7.1/docs/tutorials/customizing_your_pipeline.ipynb
--rw-r--r--   0 root         (0) root         (0)    18927 2023-03-08 12:17:00.000000 asent-0.7.1/docs/tutorials/introduction.ipynb
--rw-r--r--   0 root         (0) root         (0)      289 2023-03-08 12:17:00.000000 asent-0.7.1/docs/tutorials/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     3045 2023-03-08 12:17:01.000000 asent-0.7.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-08 12:17:12.429670 asent-0.7.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 12:17:12.389670 asent-0.7.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 12:17:12.401670 asent-0.7.1/src/asent/
--rw-r--r--   0 root         (0) root         (0)      262 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/__init__.py
--rw-r--r--   0 root         (0) root         (0)      222 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/about.py
--rw-r--r--   0 root         (0) root         (0)     7060 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/component.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/constants.py
--rw-r--r--   0 root         (0) root         (0)     4606 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/data_classes.py
--rw-r--r--   0 root         (0) root         (0)    21762 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/getters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 12:17:12.401670 asent-0.7.1/src/asent/lang/
--rw-r--r--   0 root         (0) root         (0)      318 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lang/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3030 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lang/autoconstructed.py
--rw-r--r--   0 root         (0) root         (0)     2862 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lang/da.py
--rw-r--r--   0 root         (0) root         (0)      372 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lang/emoji.py
--rw-r--r--   0 root         (0) root         (0)     4048 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lang/en.py
--rw-r--r--   0 root         (0) root         (0)     3574 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lang/no.py
--rw-r--r--   0 root         (0) root         (0)     2940 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lang/sv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 12:17:12.425670 asent-0.7.1/src/asent/lexicons/
--rw-r--r--   0 root         (0) root         (0)    26647 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/af_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)     1005 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/an_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    35208 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/ar_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    23404 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/az_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    29039 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/be_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    54863 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/bg_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    50771 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/bn_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/br_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    22886 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/bs_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    37694 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/ca_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    31326 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/cs_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    17668 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/cy_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    44942 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/da_lexicon_afinn_v1.txt
--rw-r--r--   0 root         (0) root         (0)    38777 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/da_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)   143899 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/da_lexicon_sentida_lemma_v1.csv
--rw-r--r--   0 root         (0) root         (0)    48916 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/de_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    53585 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/el_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)   123881 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/emoji_v1.json
--rwxr-xr-x   0 root         (0) root         (0)   426687 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/en_lexicon_v1.txt
--rw-r--r--   0 root         (0) root         (0)    28399 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/eo_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    51397 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/es_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    24253 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/et_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    23008 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/eu_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    32616 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/fa_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    40596 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/fi_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)     1171 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/fo_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    55988 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/fr_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)     2023 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/fy_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    12141 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/ga_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)     3505 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/gd_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    32556 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/gl_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    41926 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/gu_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    33531 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/he_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    73260 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/hi_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    25223 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/hr_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)     4273 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/ht_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    44684 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/hu_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    30612 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/hy_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)     3624 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/ia_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    32599 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/id_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)     1789 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/io_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    19690 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/is_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    54634 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/it_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    13231 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/ja_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    62779 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/ka_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    15013 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/km_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    52157 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/kn_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    23884 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/ko_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)     1275 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/ku_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)     3653 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/ky_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    21887 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/la_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)     2237 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/lb_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    26858 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/lt_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    23562 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/lv_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    56745 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/mk_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    33123 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/mr_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    32638 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/ms_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)     9570 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/mt_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    47020 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/nl_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    19930 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/nn_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    35292 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/no_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    38561 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/no_lexicon_v1.txt
--rw-r--r--   0 root         (0) root         (0)    43565 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/pl_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    47590 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/pt_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)     1071 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/rm_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    38145 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/ro_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    58383 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/ru_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    29290 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/sk_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    25541 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/sl_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    23026 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/sq_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    36153 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/sr_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    42702 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/sv_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)   302034 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/sv_lexicon_v1.txt
--rw-r--r--   0 root         (0) root         (0)    13897 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/sw_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    53790 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/ta_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    56076 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/te_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    23321 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/th_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)      752 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/tk_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    20509 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/tl_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    28309 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/tr_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    56455 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/uk_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    17160 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/ur_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)      988 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/uz_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)     9585 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/vi_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)      396 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/vo_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)     1839 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/wa_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)     5665 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/yi_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    17307 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/zh_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)    35755 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/lexicons/zhw_lexicon_chen_skiena_2014_v1.txt
--rw-r--r--   0 root         (0) root         (0)     1367 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/utils.py
--rw-r--r--   0 root         (0) root         (0)     7505 2023-03-08 12:17:00.000000 asent-0.7.1/src/asent/visualize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 12:17:12.401670 asent-0.7.1/src/asent.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8023 2023-03-08 12:17:12.000000 asent-0.7.1/src/asent.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6715 2023-03-08 12:17:12.000000 asent-0.7.1/src/asent.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-08 12:17:12.000000 asent-0.7.1/src/asent.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      418 2023-03-08 12:17:12.000000 asent-0.7.1/src/asent.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-03-08 12:17:12.000000 asent-0.7.1/src/asent.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 12:17:12.429670 asent-0.7.1/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-08 12:17:00.000000 asent-0.7.1/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      140 2023-03-08 12:17:00.000000 asent-0.7.1/tests/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      406 2023-03-08 12:17:00.000000 asent-0.7.1/tests/test_all_langs.py
--rw-r--r--   0 root         (0) root         (0)      687 2023-03-08 12:17:00.000000 asent-0.7.1/tests/test_bugs.py
--rw-r--r--   0 root         (0) root         (0)     1819 2023-03-08 12:17:00.000000 asent-0.7.1/tests/test_data_classes.py
--rw-r--r--   0 root         (0) root         (0)     8791 2023-03-08 12:17:00.000000 asent-0.7.1/tests/test_getters.py
--rw-r--r--   0 root         (0) root         (0)      645 2023-03-08 12:17:00.000000 asent-0.7.1/tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)      973 2023-03-08 12:17:00.000000 asent-0.7.1/tests/test_visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:01:50.912130 asent-0.7.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:01:50.876126 asent-0.7.2/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:01:50.876126 asent-0.7.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      716 2023-08-08 09:01:38.000000 asent-0.7.2/.github/ISSUE_TEMPLATE/01_bugs.md
+-rw-r--r--   0 root         (0) root         (0)      418 2023-08-08 09:01:38.000000 asent-0.7.2/.github/ISSUE_TEMPLATE/02_docs.md
+-rw-r--r--   0 root         (0) root         (0)      291 2023-08-08 09:01:38.000000 asent-0.7.2/.github/ISSUE_TEMPLATE/03_feature-request.md
+-rw-r--r--   0 root         (0) root         (0)      597 2023-08-08 09:01:38.000000 asent-0.7.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 root         (0) root         (0)      776 2023-08-08 09:01:38.000000 asent-0.7.2/.github/dependabot.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:01:50.876126 asent-0.7.2/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1013 2023-08-08 09:01:38.000000 asent-0.7.2/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-08-08 09:01:38.000000 asent-0.7.2/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-08-08 09:01:38.000000 asent-0.7.2/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)      867 2023-08-08 09:01:38.000000 asent-0.7.2/.github/workflows/stale.yml
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-08-08 09:01:38.000000 asent-0.7.2/.github/workflows/tests.yml
+-rw-r--r--   0 root         (0) root         (0)      324 2023-08-08 09:01:38.000000 asent-0.7.2/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      728 2023-08-08 09:01:38.000000 asent-0.7.2/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-08-08 09:01:39.000000 asent-0.7.2/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-08-08 09:01:38.000000 asent-0.7.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8023 2023-08-08 09:01:50.912130 asent-0.7.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5409 2023-08-08 09:01:38.000000 asent-0.7.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      378 2023-08-08 09:01:38.000000 asent-0.7.2/citation.cff
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:01:50.880127 asent-0.7.2/dev/
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-08-08 09:01:38.000000 asent-0.7.2/dev/add_new_language.py
+-rw-r--r--   0 root         (0) root         (0)     1588 2023-08-08 09:01:38.000000 asent-0.7.2/dev/emoji_sentiment_creator.py
+-rwxr-xr-x   0 root         (0) root         (0)   118417 2023-08-08 09:01:38.000000 asent-0.7.2/dev/emoji_utf8_lexicon.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:01:50.880127 asent-0.7.2/docs/
+-rw-r--r--   0 root         (0) root         (0)      633 2023-08-08 09:01:38.000000 asent-0.7.2/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:01:50.880127 asent-0.7.2/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)    15406 2023-08-08 09:01:38.000000 asent-0.7.2/docs/_static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)    33247 2023-08-08 09:01:38.000000 asent-0.7.2/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)    33481 2023-08-08 09:01:38.000000 asent-0.7.2/docs/_static/icon_dark.png
+-rw-r--r--   0 root         (0) root         (0)      518 2023-08-08 09:01:38.000000 asent-0.7.2/docs/asent.component.rst
+-rw-r--r--   0 root         (0) root         (0)      343 2023-08-08 09:01:38.000000 asent-0.7.2/docs/asent.getters.rst
+-rw-r--r--   0 root         (0) root         (0)      352 2023-08-08 09:01:38.000000 asent-0.7.2/docs/asent.visualize.rst
+-rw-r--r--   0 root         (0) root         (0)     4185 2023-08-08 09:01:38.000000 asent-0.7.2/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)    11750 2023-08-08 09:01:38.000000 asent-0.7.2/docs/customizing.rst
+-rw-r--r--   0 root         (0) root         (0)     2918 2023-08-08 09:01:38.000000 asent-0.7.2/docs/faq.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:01:50.884127 asent-0.7.2/docs/img/
+-rw-r--r--   0 root         (0) root         (0)   299111 2023-08-08 09:01:38.000000 asent-0.7.2/docs/img/Screenshot 2021-12-07 at 20.46.02.png
+-rw-r--r--   0 root         (0) root         (0)   129366 2023-08-08 09:01:38.000000 asent-0.7.2/docs/img/dep_parse.png
+-rw-r--r--   0 root         (0) root         (0)   143218 2023-08-08 09:01:38.000000 asent-0.7.2/docs/img/doc_polarity.png
+-rw-r--r--   0 root         (0) root         (0)    11937 2023-08-08 09:01:38.000000 asent-0.7.2/docs/img/icon.png
+-rw-r--r--   0 root         (0) root         (0)    29045 2023-08-08 09:01:38.000000 asent-0.7.2/docs/img/logo_black_font.png
+-rw-r--r--   0 root         (0) root         (0)    33481 2023-08-08 09:01:38.000000 asent-0.7.2/docs/img/logo_dark.png
+-rw-r--r--   0 root         (0) root         (0)    33247 2023-08-08 09:01:38.000000 asent-0.7.2/docs/img/logo_red_font.png
+-rw-r--r--   0 root         (0) root         (0)    37494 2023-08-08 09:01:38.000000 asent-0.7.2/docs/img/model_analysis.png
+-rw-r--r--   0 root         (0) root         (0)    37494 2023-08-08 09:01:38.000000 asent-0.7.2/docs/img/model_analysis1.png
+-rw-r--r--   0 root         (0) root         (0)    11308 2023-08-08 09:01:38.000000 asent-0.7.2/docs/img/model_pred.png
+-rw-r--r--   0 root         (0) root         (0)    16270 2023-08-08 09:01:38.000000 asent-0.7.2/docs/img/model_pred_sv.png
+-rw-r--r--   0 root         (0) root         (0)     9602 2023-08-08 09:01:38.000000 asent-0.7.2/docs/img/model_pred_sv1.png
+-rw-r--r--   0 root         (0) root         (0)    16771 2023-08-08 09:01:38.000000 asent-0.7.2/docs/img/model_pred_sv2.png
+-rw-r--r--   0 root         (0) root         (0)   184712 2023-08-08 09:01:38.000000 asent-0.7.2/docs/img/token_polarity.png
+-rw-r--r--   0 root         (0) root         (0)     1375 2023-08-08 09:01:38.000000 asent-0.7.2/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      582 2023-08-08 09:01:38.000000 asent-0.7.2/docs/installation.rst
+-rw-r--r--   0 root         (0) root         (0)     8116 2023-08-08 09:01:38.000000 asent-0.7.2/docs/introduction.rst
+-rw-r--r--   0 root         (0) root         (0)    81205 2023-08-08 09:01:38.000000 asent-0.7.2/docs/languages.rst
+-rw-r--r--   0 root         (0) root         (0)     2296 2023-08-08 09:01:38.000000 asent-0.7.2/docs/news.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:01:50.884127 asent-0.7.2/docs/tutorials/
+-rw-r--r--   0 root         (0) root         (0)    46116 2023-08-08 09:01:38.000000 asent-0.7.2/docs/tutorials/customizing_your_pipeline.ipynb
+-rw-r--r--   0 root         (0) root         (0)    18927 2023-08-08 09:01:38.000000 asent-0.7.2/docs/tutorials/introduction.ipynb
+-rw-r--r--   0 root         (0) root         (0)      289 2023-08-08 09:01:38.000000 asent-0.7.2/docs/tutorials/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     2959 2023-08-08 09:01:39.000000 asent-0.7.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-08 09:01:50.912130 asent-0.7.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:01:50.876126 asent-0.7.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:01:50.884127 asent-0.7.2/src/asent/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      222 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/about.py
+-rw-r--r--   0 root         (0) root         (0)     7060 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/component.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/constants.py
+-rw-r--r--   0 root         (0) root         (0)     4606 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/data_classes.py
+-rw-r--r--   0 root         (0) root         (0)    21762 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/getters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:01:50.888127 asent-0.7.2/src/asent/lang/
+-rw-r--r--   0 root         (0) root         (0)      318 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lang/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3030 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lang/autoconstructed.py
+-rw-r--r--   0 root         (0) root         (0)     2862 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lang/da.py
+-rw-r--r--   0 root         (0) root         (0)      372 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lang/emoji.py
+-rw-r--r--   0 root         (0) root         (0)     4048 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lang/en.py
+-rw-r--r--   0 root         (0) root         (0)     3574 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lang/no.py
+-rw-r--r--   0 root         (0) root         (0)     2940 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lang/sv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:01:50.912130 asent-0.7.2/src/asent/lexicons/
+-rw-r--r--   0 root         (0) root         (0)    26647 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/af_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)     1005 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/an_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    35208 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/ar_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    23404 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/az_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    29039 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/be_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    54863 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/bg_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    50771 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/bn_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/br_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    22886 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/bs_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    37694 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/ca_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    31326 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/cs_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    17668 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/cy_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    44942 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/da_lexicon_afinn_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    38777 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/da_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)   143899 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/da_lexicon_sentida_lemma_v1.csv
+-rw-r--r--   0 root         (0) root         (0)    48916 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/de_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    53585 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/el_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)   123881 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/emoji_v1.json
+-rwxr-xr-x   0 root         (0) root         (0)   426687 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/en_lexicon_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    28399 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/eo_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    51397 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/es_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    24253 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/et_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    23008 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/eu_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    32616 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/fa_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    40596 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/fi_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)     1171 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/fo_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    55988 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/fr_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)     2023 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/fy_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    12141 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/ga_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)     3505 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/gd_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    32556 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/gl_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    41926 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/gu_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    33531 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/he_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    73260 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/hi_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    25223 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/hr_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)     4273 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/ht_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    44684 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/hu_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    30612 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/hy_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)     3624 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/ia_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    32599 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/id_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/io_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    19690 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/is_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    54634 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/it_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    13231 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/ja_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    62779 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/ka_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    15013 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/km_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    52157 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/kn_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    23884 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/ko_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)     1275 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/ku_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)     3653 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/ky_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    21887 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/la_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)     2237 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/lb_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    26858 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/lt_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    23562 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/lv_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    56745 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/mk_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    33123 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/mr_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    32638 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/ms_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)     9570 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/mt_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    47020 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/nl_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    19930 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/nn_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    35292 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/no_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    38561 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/no_lexicon_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    43565 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/pl_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    47590 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/pt_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/rm_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    38145 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/ro_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    58383 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/ru_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    29290 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/sk_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    25541 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/sl_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    23026 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/sq_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    36153 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/sr_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    42702 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/sv_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)   302034 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/sv_lexicon_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    13897 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/sw_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    53790 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/ta_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    56076 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/te_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    23321 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/th_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)      752 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/tk_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    20509 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/tl_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    28309 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/tr_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    56455 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/uk_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    17160 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/ur_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)      988 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/uz_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)     9585 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/vi_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)      396 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/vo_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)     1839 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/wa_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)     5665 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/yi_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    17307 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/zh_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)    35755 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/lexicons/zhw_lexicon_chen_skiena_2014_v1.txt
+-rw-r--r--   0 root         (0) root         (0)     1367 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/utils.py
+-rw-r--r--   0 root         (0) root         (0)     7505 2023-08-08 09:01:38.000000 asent-0.7.2/src/asent/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:01:50.888127 asent-0.7.2/src/asent.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8023 2023-08-08 09:01:50.000000 asent-0.7.2/src/asent.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6715 2023-08-08 09:01:50.000000 asent-0.7.2/src/asent.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 09:01:50.000000 asent-0.7.2/src/asent.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      332 2023-08-08 09:01:50.000000 asent-0.7.2/src/asent.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-08-08 09:01:50.000000 asent-0.7.2/src/asent.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 09:01:50.912130 asent-0.7.2/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-08 09:01:38.000000 asent-0.7.2/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      140 2023-08-08 09:01:38.000000 asent-0.7.2/tests/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      406 2023-08-08 09:01:38.000000 asent-0.7.2/tests/test_all_langs.py
+-rw-r--r--   0 root         (0) root         (0)      687 2023-08-08 09:01:38.000000 asent-0.7.2/tests/test_bugs.py
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-08-08 09:01:38.000000 asent-0.7.2/tests/test_data_classes.py
+-rw-r--r--   0 root         (0) root         (0)     8791 2023-08-08 09:01:38.000000 asent-0.7.2/tests/test_getters.py
+-rw-r--r--   0 root         (0) root         (0)      645 2023-08-08 09:01:38.000000 asent-0.7.2/tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)      973 2023-08-08 09:01:38.000000 asent-0.7.2/tests/test_visualize.py
```

### Comparing `asent-0.7.1/.github/ISSUE_TEMPLATE/01_bugs.md` & `asent-0.7.2/.github/ISSUE_TEMPLATE/01_bugs.md`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/.github/ISSUE_TEMPLATE/config.yml` & `asent-0.7.2/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/.github/dependabot.yml` & `asent-0.7.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/.github/workflows/dependabot_automerge.yml` & `asent-0.7.2/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/.github/workflows/documentation.yml` & `asent-0.7.2/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/.github/workflows/release.yml` & `asent-0.7.2/.github/workflows/release.yml`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
       # Checkout action is required for token to persist
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
           token: ${{ secrets.RELEASE }}
 
       - name: Python Semantic Release
-        uses: relekang/python-semantic-release@v7.33.1
+        uses: relekang/python-semantic-release@v7.34.6
         with:
           github_token: ${{ secrets.RELEASE }}
           # Remember to copy the [semantic_release] section from pyproject.toml
           # as well
           # To enable pypi,
           # 1) Set upload_to_pypi to true in  pyproject.toml and
           # 2) Set the pypi_token in the repo
```

### Comparing `asent-0.7.1/.github/workflows/stale.yml` & `asent-0.7.2/.github/workflows/stale.yml`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/.github/workflows/tests.yml` & `asent-0.7.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/CHANGELOG.md` & `asent-0.7.2/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.7.2 (2023-08-08)
+
+### Fix
+
+* Removed upper bound ([`499ad72`](https://github.com/KennethEnevoldsen/asent/commit/499ad72b3db2049d4a3dd633483f1b6b119f9729))
+
 ## v0.7.1 (2023-03-08)
 ### Fix
 * Updated spacy dependency ([`bfe8424`](https://github.com/KennethEnevoldsen/asent/commit/bfe842446028ecae62899a684f2099f75b8ed2ae))
 
 ### Documentation
 * Fix badge ([`40a8d49`](https://github.com/KennethEnevoldsen/asent/commit/40a8d49731c5b2c100da1e64493a78bdeb7ea2e1))
```

### Comparing `asent-0.7.1/LICENSE` & `asent-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/PKG-INFO` & `asent-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asent
-Version: 0.7.1
+Version: 0.7.2
 Summary: A python package for flexible and transparent sentiment analysis.
 Author-email: Kenneth Enevoldsen <kennethcenevoldsen@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Kenneth Enevoldsen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: asent Version: 0.7.1 Summary: A python package for
+Metadata-Version: 2.1 Name: asent Version: 0.7.2 Summary: A python package for
 flexible and transparent sentiment analysis. Author-email: Kenneth Enevoldsen
 gmail.com> License: MIT License Copyright (c) 2021 Kenneth Enevoldsen
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
```

### Comparing `asent-0.7.1/README.md` & `asent-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/dev/add_new_language.py` & `asent-0.7.2/dev/add_new_language.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""convert into sentiment lexicon from:
+"""Convert into sentiment lexicon from:
 
 https://www.kaggle.com/datasets/rtatman/sentiment-lexicons-
 for-81-languages/discussion/39827?resource=download into txt files for
 each language with each positive word rated +1 and negative words rated
 -1.
 """
 from collections import defaultdict
```

### Comparing `asent-0.7.1/dev/emoji_sentiment_creator.py` & `asent-0.7.2/dev/emoji_sentiment_creator.py`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/dev/emoji_utf8_lexicon.txt` & `asent-0.7.2/dev/emoji_utf8_lexicon.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/docs/Makefile` & `asent-0.7.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/docs/_static/favicon.ico` & `asent-0.7.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/docs/_static/icon.png` & `asent-0.7.2/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/docs/_static/icon_dark.png` & `asent-0.7.2/docs/_static/icon_dark.png`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/docs/asent.component.rst` & `asent-0.7.2/docs/asent.component.rst`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/docs/conf.py` & `asent-0.7.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/docs/customizing.rst` & `asent-0.7.2/docs/customizing.rst`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/docs/faq.rst` & `asent-0.7.2/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/docs/img/Screenshot 2021-12-07 at 20.46.02.png` & `asent-0.7.2/docs/img/Screenshot 2021-12-07 at 20.46.02.png`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/docs/img/dep_parse.png` & `asent-0.7.2/docs/img/dep_parse.png`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/docs/img/doc_polarity.png` & `asent-0.7.2/docs/img/doc_polarity.png`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/docs/img/icon.png` & `asent-0.7.2/docs/img/icon.png`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/docs/img/logo_black_font.png` & `asent-0.7.2/docs/img/logo_black_font.png`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/docs/img/logo_dark.png` & `asent-0.7.2/docs/img/logo_dark.png`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/docs/img/logo_red_font.png` & `asent-0.7.2/docs/img/logo_red_font.png`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/docs/img/model_analysis.png` & `asent-0.7.2/docs/img/model_analysis.png`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/docs/img/model_analysis1.png` & `asent-0.7.2/docs/img/model_analysis1.png`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/docs/img/model_pred.png` & `asent-0.7.2/docs/img/model_pred.png`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/docs/img/model_pred_sv.png` & `asent-0.7.2/docs/img/model_pred_sv.png`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/docs/img/model_pred_sv1.png` & `asent-0.7.2/docs/img/model_pred_sv1.png`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/docs/img/model_pred_sv2.png` & `asent-0.7.2/docs/img/model_pred_sv2.png`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/docs/img/token_polarity.png` & `asent-0.7.2/docs/img/token_polarity.png`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/docs/index.rst` & `asent-0.7.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/docs/installation.rst` & `asent-0.7.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/docs/introduction.rst` & `asent-0.7.2/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/docs/languages.rst` & `asent-0.7.2/docs/languages.rst`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/docs/news.rst` & `asent-0.7.2/docs/news.rst`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/docs/tutorials/customizing_your_pipeline.ipynb` & `asent-0.7.2/docs/tutorials/customizing_your_pipeline.ipynb`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/docs/tutorials/introduction.ipynb` & `asent-0.7.2/docs/tutorials/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/pyproject.toml` & `asent-0.7.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "asent"
-version = "0.7.1"
+version = "0.7.2"
 description = "A python package for flexible and transparent sentiment analysis."
 authors = [{name = "Kenneth Enevoldsen", email = "kennethcenevoldsen@gmail.com"}]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
@@ -30,16 +30,16 @@
     "text analysis",
     "aspect-based sentiment analysis",
     "ABSA"
     ]
 requires-python = ">=3.8"
 
 dependencies = [
-    "spacy>=3.0.0,<3.6.0",
-    "matplotlib>=3.5.0,<4.0.0",
+    "spacy>=3.0.0",
+    "matplotlib>=3.5.0",
 ]
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [project.license]
@@ -49,35 +49,35 @@
 [project.urls]
 Homepage = "https://github.com/KennethEnevoldsen/asent"
 repository = "https://github.com/KennethEnevoldsen/asent"
 documentation = "https://kennethenevoldsen.github.io/asent/"
 
 [project.optional-dependencies]
 da = ["dacy>=1.1.0"]
-all = ["nltk>=3.6.7,<3.8.0"]
+all = ["nltk>=3.6.7"]
 style = [
-    "black==22.12.0",
-    "pre-commit>=2.20.0,<2.21.0",
-    "ruff==0.0.191",
-    "mypy==0.991"
+    "black>=22.12.0",
+    "pre-commit>=2.20.0",
+    "ruff>=0.0.263",
+    "mypy>=0.991"
 ]
 tests = [
-    "pytest>=7.1.3,<7.3.0",
-    "pytest-cov>=3.0.0,<3.0.1",   
+    "pytest>=7.1.3",
+    "pytest-cov>=3.0.0",   
 ]
 docs = [
-    "sphinx>=5.3.0,<5.4.0",
-    "furo==2022.12.7",
-    "sphinx-copybutton>=0.5.1,<0.5.2",
-    "sphinxext-opengraph>=0.7.3,<0.7.4",
-    "sphinx_design>=0.3.0,<0.3.1",
-     "myst-nb>=0.6.0,<1.17.0",
+    "sphinx>=5.3.0",
+    "furo>=2022.12.7",
+    "sphinx-copybutton>=0.5.1",
+    "sphinxext-opengraph>=0.7.3",
+    "sphinx_design>=0.3.0",
+     "myst-nb>=0.6.0",
 ]
 tutorials = [
-    "jupyter>=1.0.0,<1.1.0",
+    "jupyter>=1.0.0",
 ]
 
 [tool.coverage.run]
 omit = [
     "**/tests/*",
     "**/_vendorized/*",
     "**/about.py",
```

### Comparing `asent-0.7.1/src/asent/component.py` & `asent-0.7.2/src/asent/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     make_span_polarity_getter,
     make_token_polarity_getter,
     make_valance_getter,
 )
 
 
 class Asent:
-    """spaCy v.3.0 component for adding an asent sentiment models to `Doc`
+    """SpaCy v.3.0 component for adding an asent sentiment models to `Doc`
     objects.
 
     Ading the Token extentions 'valence', 'intensifier', 'is_negation',
     'is_negated', 'is_contrastive_conj' and 'polarity' as well as the
     Span and Doc extension 'polarity'.
     """
```

### Comparing `asent-0.7.1/src/asent/data_classes.py` & `asent-0.7.2/src/asent/data_classes.py`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/getters.py` & `asent-0.7.2/src/asent/getters.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     """
     t_getter = make_txt_getter(lemmatize, lowercase)
 
     if not Doc.has_extension("is_cap_diff"):
         Doc.set_extension("is_cap_diff", getter=allcap_differential_getter)
 
     def intensifier_scalar_getter(token: Token) -> float:
-        """get intensifier score for token."""
+        """Get intensifier score for token."""
         t = t_getter(token)
         if t in intensifiers:
             scalar = intensifiers[t]
             if token.is_upper and token.doc._.is_cap_diff:
                 scalar += C_INCR
             return scalar
         return 0.0
@@ -425,15 +425,15 @@
             sentiment[i] = s * before_but_scalar
         for i, s in enumerate(sentiment[but_idx:]):
             sentiment[i] = s * after_but_scalar
     return sentiment
 
 
 def sift_sentiment_scores(sentiments: Iterable[float]) -> Tuple[float, float, int]:
-    """separate positive and negative sentiment scores."""
+    """Separate positive and negative sentiment scores."""
     pos_sum = 0.0
     neg_sum = 0.0
     neu_count = 0
     for sentiment_score in sentiments:
         if sentiment_score > 0:
             pos_sum += (
                 float(sentiment_score) + 1
```

### Comparing `asent-0.7.1/src/asent/lang/autoconstructed.py` & `asent-0.7.2/src/asent/lang/autoconstructed.py`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lang/da.py` & `asent-0.7.2/src/asent/lang/da.py`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lang/en.py` & `asent-0.7.2/src/asent/lang/en.py`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lang/no.py` & `asent-0.7.2/src/asent/lang/no.py`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lang/sv.py` & `asent-0.7.2/src/asent/lang/sv.py`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/af_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/af_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/an_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/an_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/ar_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/ar_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/az_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/az_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/be_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/be_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/bg_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/bg_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/bn_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/bn_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/br_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/br_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/bs_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/bs_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/ca_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/ca_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/cs_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/cs_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/cy_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/cy_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/da_lexicon_afinn_v1.txt` & `asent-0.7.2/src/asent/lexicons/da_lexicon_afinn_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/da_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/da_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/da_lexicon_sentida_lemma_v1.csv` & `asent-0.7.2/src/asent/lexicons/da_lexicon_sentida_lemma_v1.csv`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/de_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/de_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/el_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/el_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/emoji_v1.json` & `asent-0.7.2/src/asent/lexicons/emoji_v1.json`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/en_lexicon_v1.txt` & `asent-0.7.2/src/asent/lexicons/en_lexicon_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/eo_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/eo_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/es_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/es_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/et_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/et_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/eu_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/eu_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/fa_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/fa_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/fi_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/fi_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/fo_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/fo_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/fr_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/fr_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/fy_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/fy_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/ga_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/ga_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/gd_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/gd_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/gl_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/gl_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/gu_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/gu_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/he_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/he_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/hi_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/hi_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/hr_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/hr_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/ht_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/ht_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/hu_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/hu_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/hy_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/hy_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/ia_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/ia_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/id_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/id_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/io_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/io_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/is_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/is_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/it_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/it_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/ja_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/ja_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/ka_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/ka_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/km_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/km_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/kn_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/kn_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/ko_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/ko_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/ku_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/ku_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/ky_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/ky_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/la_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/la_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/lb_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/lb_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/lt_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/lt_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/lv_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/lv_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/mk_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/mk_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/mr_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/mr_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/ms_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/ms_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/mt_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/mt_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/nl_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/nl_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/nn_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/nn_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/no_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/no_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/no_lexicon_v1.txt` & `asent-0.7.2/src/asent/lexicons/no_lexicon_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/pl_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/pl_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/pt_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/pt_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/rm_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/rm_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/ro_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/ro_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/ru_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/ru_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/sk_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/sk_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/sl_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/sl_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/sq_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/sq_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/sr_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/sr_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/sv_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/sv_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/sv_lexicon_v1.txt` & `asent-0.7.2/src/asent/lexicons/sv_lexicon_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/sw_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/sw_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/ta_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/ta_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/te_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/te_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/th_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/th_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/tk_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/tk_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/tl_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/tl_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/tr_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/tr_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/uk_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/uk_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/ur_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/ur_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/uz_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/uz_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/vi_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/vi_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/wa_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/wa_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/yi_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/yi_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/zh_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/zh_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/lexicons/zhw_lexicon_chen_skiena_2014_v1.txt` & `asent-0.7.2/src/asent/lexicons/zhw_lexicon_chen_skiena_2014_v1.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/utils.py` & `asent-0.7.2/src/asent/utils.py`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent/visualize.py` & `asent-0.7.2/src/asent/visualize.py`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/src/asent.egg-info/PKG-INFO` & `asent-0.7.2/src/asent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asent
-Version: 0.7.1
+Version: 0.7.2
 Summary: A python package for flexible and transparent sentiment analysis.
 Author-email: Kenneth Enevoldsen <kennethcenevoldsen@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Kenneth Enevoldsen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: asent Version: 0.7.1 Summary: A python package for
+Metadata-Version: 2.1 Name: asent Version: 0.7.2 Summary: A python package for
 flexible and transparent sentiment analysis. Author-email: Kenneth Enevoldsen
 gmail.com> License: MIT License Copyright (c) 2021 Kenneth Enevoldsen
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
```

### Comparing `asent-0.7.1/src/asent.egg-info/SOURCES.txt` & `asent-0.7.2/src/asent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/tests/test_bugs.py` & `asent-0.7.2/tests/test_bugs.py`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/tests/test_data_classes.py` & `asent-0.7.2/tests/test_data_classes.py`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/tests/test_getters.py` & `asent-0.7.2/tests/test_getters.py`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/tests/test_utils.py` & `asent-0.7.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `asent-0.7.1/tests/test_visualize.py` & `asent-0.7.2/tests/test_visualize.py`

 * *Files identical despite different names*

