# Comparing `tmp/erpbrasil.edoc-2.5.0.tar.gz` & `tmp/erpbrasil.edoc-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erpbrasil.edoc-2.5.0.tar", last modified: Wed Jul 19 13:07:23 2023, max compression
+gzip compressed data, was "erpbrasil.edoc-2.5.1.tar", last modified: Tue Aug  8 11:52:11 2023, max compression
```

## Comparing `erpbrasil.edoc-2.5.0.tar` & `erpbrasil.edoc-2.5.1.tar`

### file list

```diff
@@ -1,97 +1,96 @@
-drwxrwxr-x   0 ygor-carvalho  (1000) ygor-carvalho  (1000)        0 2023-07-19 13:07:22.995649 erpbrasil.edoc-2.5.0/
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     1424 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/.appveyor.yml
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)      511 2023-07-19 13:06:46.000000 erpbrasil.edoc-2.5.0/.bumpversion.cfg
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     2893 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/.cookiecutterrc
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)      182 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/.coveragerc
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)      215 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/.editorconfig
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)      636 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/.gitignore
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)      915 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/.travis.yml
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)       64 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/AUTHORS.rst
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     1181 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/CHANGELOG.rst
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     2753 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/CONTRIBUTING.rst
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     1105 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/LICENSE
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)      359 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/MANIFEST.in
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     4536 2023-07-19 13:07:22.995649 erpbrasil.edoc-2.5.0/PKG-INFO
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     3582 2023-07-19 13:06:46.000000 erpbrasil.edoc-2.5.0/README.rst
-drwxrwxr-x   0 ygor-carvalho  (1000) ygor-carvalho  (1000)        0 2023-07-19 13:07:22.991649 erpbrasil.edoc-2.5.0/ci/
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     3995 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/ci/appveyor-bootstrap.py
--rwxrwxr-x   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     3827 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/ci/appveyor-download.py
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)      763 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/ci/appveyor-with-compiler.cmd
--rwxrwxr-x   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     2097 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/ci/bootstrap.py
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)       50 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/ci/requirements.txt
-drwxrwxr-x   0 ygor-carvalho  (1000) ygor-carvalho  (1000)        0 2023-07-19 13:07:22.991649 erpbrasil.edoc-2.5.0/ci/templates/
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     1756 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/ci/templates/.appveyor.yml
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)      956 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/ci/templates/.travis.yml
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     1816 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/ci/templates/appveyor.yml
-drwxrwxr-x   0 ygor-carvalho  (1000) ygor-carvalho  (1000)        0 2023-07-19 13:07:22.995649 erpbrasil.edoc-2.5.0/docs/
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)       28 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/docs/authors.rst
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)       30 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/docs/changelog.rst
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     1382 2023-07-19 13:06:46.000000 erpbrasil.edoc-2.5.0/docs/conf.py
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)       33 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/docs/contributing.rst
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)      245 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/docs/index.rst
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)       94 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/docs/installation.rst
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)       27 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/docs/readme.rst
-drwxrwxr-x   0 ygor-carvalho  (1000) ygor-carvalho  (1000)        0 2023-07-19 13:07:22.995649 erpbrasil.edoc-2.5.0/docs/reference/
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)      126 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/docs/reference/erpbrasil.edoc.rst
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)       66 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/docs/reference/index.rst
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)       29 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/docs/requirements.txt
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)      109 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/docs/spelling_wordlist.txt
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)       80 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/docs/usage.rst
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)       98 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/requirements.txt
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)      508 2023-07-19 13:07:22.995649 erpbrasil.edoc-2.5.0/setup.cfg
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     3749 2023-07-19 13:06:46.000000 erpbrasil.edoc-2.5.0/setup.py
-drwxrwxr-x   0 ygor-carvalho  (1000) ygor-carvalho  (1000)        0 2023-07-19 13:07:22.991649 erpbrasil.edoc-2.5.0/src/
-drwxrwxr-x   0 ygor-carvalho  (1000) ygor-carvalho  (1000)        0 2023-07-19 13:07:22.995649 erpbrasil.edoc-2.5.0/src/erpbrasil/
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)      271 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/src/erpbrasil/__init__.py
-drwxrwxr-x   0 ygor-carvalho  (1000) ygor-carvalho  (1000)        0 2023-07-19 13:07:22.995649 erpbrasil.edoc-2.5.0/src/erpbrasil/edoc/
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)      481 2023-07-19 13:06:46.000000 erpbrasil.edoc-2.5.0/src/erpbrasil/edoc/__init__.py
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)      397 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/src/erpbrasil/edoc/__main__.py
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     6739 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/src/erpbrasil/edoc/chave.py
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)      831 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/src/erpbrasil/edoc/cli.py
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     7116 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/src/erpbrasil/edoc/edoc.py
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)    11568 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/src/erpbrasil/edoc/mde.py
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     3916 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/src/erpbrasil/edoc/mdfe.py
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)    14351 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/src/erpbrasil/edoc/nfce.py
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)    45500 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/src/erpbrasil/edoc/nfe.py
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     3740 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/src/erpbrasil/edoc/nfse.py
-drwxrwxr-x   0 ygor-carvalho  (1000) ygor-carvalho  (1000)        0 2023-07-19 13:07:22.995649 erpbrasil.edoc-2.5.0/src/erpbrasil/edoc/provedores/
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)        0 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/src/erpbrasil/edoc/provedores/__init__.py
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     1037 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/src/erpbrasil/edoc/provedores/cidades.py
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     2463 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/src/erpbrasil/edoc/provedores/dsf.py
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)    10310 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/src/erpbrasil/edoc/provedores/ginfes.py
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)    12756 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/src/erpbrasil/edoc/provedores/issnet.py
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     6850 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/src/erpbrasil/edoc/provedores/paulistana.py
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     1595 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/src/erpbrasil/edoc/resposta.py
-drwxrwxr-x   0 ygor-carvalho  (1000) ygor-carvalho  (1000)        0 2023-07-19 13:07:22.995649 erpbrasil.edoc-2.5.0/src/erpbrasil.edoc.egg-info/
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     4536 2023-07-19 13:07:22.000000 erpbrasil.edoc-2.5.0/src/erpbrasil.edoc.egg-info/PKG-INFO
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     2618 2023-07-19 13:07:22.000000 erpbrasil.edoc-2.5.0/src/erpbrasil.edoc.egg-info/SOURCES.txt
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)        1 2023-07-19 13:07:22.000000 erpbrasil.edoc-2.5.0/src/erpbrasil.edoc.egg-info/dependency_links.txt
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)       59 2023-07-19 13:07:22.000000 erpbrasil.edoc-2.5.0/src/erpbrasil.edoc.egg-info/entry_points.txt
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)       25 2023-07-19 13:07:22.000000 erpbrasil.edoc-2.5.0/src/erpbrasil.edoc.egg-info/namespace_packages.txt
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)        1 2023-07-19 13:07:22.000000 erpbrasil.edoc-2.5.0/src/erpbrasil.edoc.egg-info/not-zip-safe
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)      281 2023-07-19 13:07:22.000000 erpbrasil.edoc-2.5.0/src/erpbrasil.edoc.egg-info/requires.txt
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)       10 2023-07-19 13:07:22.000000 erpbrasil.edoc-2.5.0/src/erpbrasil.edoc.egg-info/top_level.txt
-drwxrwxr-x   0 ygor-carvalho  (1000) ygor-carvalho  (1000)        0 2023-07-19 13:07:22.995649 erpbrasil.edoc-2.5.0/tests/
-drwxrwxr-x   0 ygor-carvalho  (1000) ygor-carvalho  (1000)        0 2023-07-19 13:07:22.995649 erpbrasil.edoc-2.5.0/tests/fixtures/
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     2597 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/tests/fixtures/dummy_cert.pfx
-drwxrwxr-x   0 ygor-carvalho  (1000) ygor-carvalho  (1000)        0 2023-07-19 13:07:22.995649 erpbrasil.edoc-2.5.0/tests/fixtures/vcr_cassettes/
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)    11491 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/tests/fixtures/vcr_cassettes/test_cancelar_documento.yaml
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     9234 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/tests/fixtures/vcr_cassettes/test_cancelar_documento_ginfes.yaml
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     3008 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/tests/fixtures/vcr_cassettes/test_chave.yaml
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     6682 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/tests/fixtures/vcr_cassettes/test_ciencia_da_operacao.yaml
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)    11477 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/tests/fixtures/vcr_cassettes/test_confirmacao_da_operacao.yaml
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     6969 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/tests/fixtures/vcr_cassettes/test_consulta_documento.yaml
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)    10324 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/tests/fixtures/vcr_cassettes/test_consulta_documento_ginfes.yaml
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     6744 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/tests/fixtures/vcr_cassettes/test_desconhecimento_da_operacao.yaml
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)    16217 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/tests/fixtures/vcr_cassettes/test_envia_documento.yaml
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)    17539 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/tests/fixtures/vcr_cassettes/test_envia_documento_ginfes.yaml
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     2497 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/tests/fixtures/vcr_cassettes/test_nsu_especifico.yaml
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     6764 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/tests/fixtures/vcr_cassettes/test_operacao_nao_realizada.yaml
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     6533 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/tests/fixtures/vcr_cassettes/test_status_servico.yaml
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)   144902 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/tests/fixtures/vcr_cassettes/test_ultimo_nsu.yaml
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     2620 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/tests/test_erpbrasil_edoc.py
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     3105 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/tests/test_erpbrasil_edoc_manifestacao.py
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     6921 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/tests/test_erpbrasil_edoc_nfse_ginfes.py
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     5431 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/tests/test_erpbrasil_edoc_nfse_paulistana.py
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     1261 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/tests/test_erpbrasil_edoc_situacao.py
--rw-rw-r--   0 ygor-carvalho  (1000) ygor-carvalho  (1000)     1989 2023-07-19 13:05:39.000000 erpbrasil.edoc-2.5.0/tox.ini
+drwxr-xr-x   0 ygorcarvalho  (1000) ygorcarvalho  (1000)        0 2023-08-08 11:52:11.080464 erpbrasil.edoc-2.5.1/
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     1424 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/.appveyor.yml
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)      511 2023-08-08 11:49:36.000000 erpbrasil.edoc-2.5.1/.bumpversion.cfg
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     2893 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/.cookiecutterrc
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)      182 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/.coveragerc
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)      215 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/.editorconfig
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)      915 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/.travis.yml
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)       64 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/AUTHORS.rst
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     1181 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/CHANGELOG.rst
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     2753 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/CONTRIBUTING.rst
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     1105 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/LICENSE
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)      359 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/MANIFEST.in
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     4536 2023-08-08 11:52:11.080464 erpbrasil.edoc-2.5.1/PKG-INFO
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     3582 2023-08-08 11:49:36.000000 erpbrasil.edoc-2.5.1/README.rst
+drwxr-xr-x   0 ygorcarvalho  (1000) ygorcarvalho  (1000)        0 2023-08-08 11:52:11.077463 erpbrasil.edoc-2.5.1/ci/
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     3995 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/ci/appveyor-bootstrap.py
+-rwxr-xr-x   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     3827 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/ci/appveyor-download.py
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)      763 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/ci/appveyor-with-compiler.cmd
+-rwxr-xr-x   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     2097 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/ci/bootstrap.py
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)       50 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/ci/requirements.txt
+drwxr-xr-x   0 ygorcarvalho  (1000) ygorcarvalho  (1000)        0 2023-08-08 11:52:11.077463 erpbrasil.edoc-2.5.1/ci/templates/
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     1756 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/ci/templates/.appveyor.yml
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)      956 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/ci/templates/.travis.yml
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     1816 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/ci/templates/appveyor.yml
+drwxr-xr-x   0 ygorcarvalho  (1000) ygorcarvalho  (1000)        0 2023-08-08 11:52:11.077463 erpbrasil.edoc-2.5.1/docs/
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)       28 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/docs/authors.rst
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)       30 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/docs/changelog.rst
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     1382 2023-08-08 11:49:36.000000 erpbrasil.edoc-2.5.1/docs/conf.py
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)       33 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/docs/contributing.rst
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)      245 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/docs/index.rst
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)       94 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/docs/installation.rst
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)       27 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/docs/readme.rst
+drwxr-xr-x   0 ygorcarvalho  (1000) ygorcarvalho  (1000)        0 2023-08-08 11:52:11.077463 erpbrasil.edoc-2.5.1/docs/reference/
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)      126 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/docs/reference/erpbrasil.edoc.rst
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)       66 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/docs/reference/index.rst
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)       29 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/docs/requirements.txt
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)      109 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/docs/spelling_wordlist.txt
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)       80 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/docs/usage.rst
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)       98 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/requirements.txt
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)      508 2023-08-08 11:52:11.080464 erpbrasil.edoc-2.5.1/setup.cfg
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     3749 2023-08-08 11:49:36.000000 erpbrasil.edoc-2.5.1/setup.py
+drwxr-xr-x   0 ygorcarvalho  (1000) ygorcarvalho  (1000)        0 2023-08-08 11:52:11.075463 erpbrasil.edoc-2.5.1/src/
+drwxr-xr-x   0 ygorcarvalho  (1000) ygorcarvalho  (1000)        0 2023-08-08 11:52:11.077463 erpbrasil.edoc-2.5.1/src/erpbrasil/
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)      271 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/src/erpbrasil/__init__.py
+drwxr-xr-x   0 ygorcarvalho  (1000) ygorcarvalho  (1000)        0 2023-08-08 11:52:11.079463 erpbrasil.edoc-2.5.1/src/erpbrasil/edoc/
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)      481 2023-08-08 11:49:36.000000 erpbrasil.edoc-2.5.1/src/erpbrasil/edoc/__init__.py
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)      397 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/src/erpbrasil/edoc/__main__.py
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     6739 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/src/erpbrasil/edoc/chave.py
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)      831 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/src/erpbrasil/edoc/cli.py
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     7116 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/src/erpbrasil/edoc/edoc.py
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)    11568 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/src/erpbrasil/edoc/mde.py
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     3916 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/src/erpbrasil/edoc/mdfe.py
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)    14199 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/src/erpbrasil/edoc/nfce.py
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)    45500 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/src/erpbrasil/edoc/nfe.py
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     3740 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/src/erpbrasil/edoc/nfse.py
+drwxr-xr-x   0 ygorcarvalho  (1000) ygorcarvalho  (1000)        0 2023-08-08 11:52:11.079463 erpbrasil.edoc-2.5.1/src/erpbrasil/edoc/provedores/
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)        0 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/src/erpbrasil/edoc/provedores/__init__.py
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     1037 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/src/erpbrasil/edoc/provedores/cidades.py
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     2463 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/src/erpbrasil/edoc/provedores/dsf.py
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)    10310 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/src/erpbrasil/edoc/provedores/ginfes.py
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)    12756 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/src/erpbrasil/edoc/provedores/issnet.py
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     6850 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/src/erpbrasil/edoc/provedores/paulistana.py
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     1595 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/src/erpbrasil/edoc/resposta.py
+drwxr-xr-x   0 ygorcarvalho  (1000) ygorcarvalho  (1000)        0 2023-08-08 11:52:11.078463 erpbrasil.edoc-2.5.1/src/erpbrasil.edoc.egg-info/
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     4536 2023-08-08 11:52:11.000000 erpbrasil.edoc-2.5.1/src/erpbrasil.edoc.egg-info/PKG-INFO
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     2607 2023-08-08 11:52:11.000000 erpbrasil.edoc-2.5.1/src/erpbrasil.edoc.egg-info/SOURCES.txt
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)        1 2023-08-08 11:52:11.000000 erpbrasil.edoc-2.5.1/src/erpbrasil.edoc.egg-info/dependency_links.txt
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)       59 2023-08-08 11:52:11.000000 erpbrasil.edoc-2.5.1/src/erpbrasil.edoc.egg-info/entry_points.txt
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)       25 2023-08-08 11:52:11.000000 erpbrasil.edoc-2.5.1/src/erpbrasil.edoc.egg-info/namespace_packages.txt
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)        1 2023-08-08 11:52:11.000000 erpbrasil.edoc-2.5.1/src/erpbrasil.edoc.egg-info/not-zip-safe
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)      281 2023-08-08 11:52:11.000000 erpbrasil.edoc-2.5.1/src/erpbrasil.edoc.egg-info/requires.txt
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)       10 2023-08-08 11:52:11.000000 erpbrasil.edoc-2.5.1/src/erpbrasil.edoc.egg-info/top_level.txt
+drwxr-xr-x   0 ygorcarvalho  (1000) ygorcarvalho  (1000)        0 2023-08-08 11:52:11.079463 erpbrasil.edoc-2.5.1/tests/
+drwxr-xr-x   0 ygorcarvalho  (1000) ygorcarvalho  (1000)        0 2023-08-08 11:52:11.079463 erpbrasil.edoc-2.5.1/tests/fixtures/
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     2597 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/tests/fixtures/dummy_cert.pfx
+drwxr-xr-x   0 ygorcarvalho  (1000) ygorcarvalho  (1000)        0 2023-08-08 11:52:11.080464 erpbrasil.edoc-2.5.1/tests/fixtures/vcr_cassettes/
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)    11491 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/tests/fixtures/vcr_cassettes/test_cancelar_documento.yaml
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     9234 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/tests/fixtures/vcr_cassettes/test_cancelar_documento_ginfes.yaml
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     3008 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/tests/fixtures/vcr_cassettes/test_chave.yaml
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     6682 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/tests/fixtures/vcr_cassettes/test_ciencia_da_operacao.yaml
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)    11477 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/tests/fixtures/vcr_cassettes/test_confirmacao_da_operacao.yaml
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     6969 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/tests/fixtures/vcr_cassettes/test_consulta_documento.yaml
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)    10324 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/tests/fixtures/vcr_cassettes/test_consulta_documento_ginfes.yaml
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     6744 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/tests/fixtures/vcr_cassettes/test_desconhecimento_da_operacao.yaml
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)    16217 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/tests/fixtures/vcr_cassettes/test_envia_documento.yaml
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)    17539 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/tests/fixtures/vcr_cassettes/test_envia_documento_ginfes.yaml
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     2497 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/tests/fixtures/vcr_cassettes/test_nsu_especifico.yaml
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     6764 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/tests/fixtures/vcr_cassettes/test_operacao_nao_realizada.yaml
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     6533 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/tests/fixtures/vcr_cassettes/test_status_servico.yaml
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)   144902 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/tests/fixtures/vcr_cassettes/test_ultimo_nsu.yaml
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     2620 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/tests/test_erpbrasil_edoc.py
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     3105 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/tests/test_erpbrasil_edoc_manifestacao.py
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     6921 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/tests/test_erpbrasil_edoc_nfse_ginfes.py
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     5431 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/tests/test_erpbrasil_edoc_nfse_paulistana.py
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     1261 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/tests/test_erpbrasil_edoc_situacao.py
+-rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     1989 2023-08-08 11:48:59.000000 erpbrasil.edoc-2.5.1/tox.ini
```

### Comparing `erpbrasil.edoc-2.5.0/.appveyor.yml` & `erpbrasil.edoc-2.5.1/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/.cookiecutterrc` & `erpbrasil.edoc-2.5.1/.cookiecutterrc`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/.travis.yml` & `erpbrasil.edoc-2.5.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/CHANGELOG.rst` & `erpbrasil.edoc-2.5.1/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/CONTRIBUTING.rst` & `erpbrasil.edoc-2.5.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/LICENSE` & `erpbrasil.edoc-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/PKG-INFO` & `erpbrasil.edoc-2.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erpbrasil.edoc
-Version: 2.5.0
+Version: 2.5.1
 Summary: Emissão de documentos fiscais e outras obrigações (NF-E, NFS-E, MDF-E, CT-E, REINF, E-SOCIAL)
 Home-page: https://github.com/erpbrasil/erpbrasil.edoc
 Author: Luis Felipe Mileo
 Author-email: mileo@kmee.com.br
 License: MIT
 Project-URL: Documentation, https://erpbrasiledoc.readthedocs.io/
 Project-URL: Changelog, https://erpbrasiledoc.readthedocs.io/en/latest/changelog.html
```

### Comparing `erpbrasil.edoc-2.5.0/README.rst` & `erpbrasil.edoc-2.5.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -26,17 +26,17 @@
     :alt: Coverage Status
     :target: https://codecov.io/github/erpbrasil/erpbrasil.edoc
 
 .. |version| image:: https://img.shields.io/pypi/v/erpbrasil.edoc.svg
     :alt: PyPI Package latest release
     :target: https://pypi.org/project/erpbrasil.edoc
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/erpbrasil/erpbrasil.edoc/v2.5.0.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/erpbrasil/erpbrasil.edoc/v2.5.1.svg
     :alt: Commits since latest release
-    :target: https://github.com/erpbrasil/erpbrasil.edoc/compare/v2.5.0...master
+    :target: https://github.com/erpbrasil/erpbrasil.edoc/compare/v2.5.1...master
 
 .. |wheel| image:: https://img.shields.io/pypi/wheel/erpbrasil.edoc.svg
     :alt: PyPI Wheel
     :target: https://pypi.org/project/erpbrasil.edoc
 
 .. |supported-versions| image:: https://img.shields.io/pypi/pyversions/erpbrasil.edoc.svg
     :alt: Supported versions
```

### Comparing `erpbrasil.edoc-2.5.0/ci/appveyor-bootstrap.py` & `erpbrasil.edoc-2.5.1/ci/appveyor-bootstrap.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/ci/appveyor-download.py` & `erpbrasil.edoc-2.5.1/ci/appveyor-download.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/ci/appveyor-with-compiler.cmd` & `erpbrasil.edoc-2.5.1/ci/appveyor-with-compiler.cmd`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/ci/bootstrap.py` & `erpbrasil.edoc-2.5.1/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/ci/templates/.appveyor.yml` & `erpbrasil.edoc-2.5.1/ci/templates/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/ci/templates/.travis.yml` & `erpbrasil.edoc-2.5.1/ci/templates/.travis.yml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/ci/templates/appveyor.yml` & `erpbrasil.edoc-2.5.1/ci/templates/appveyor.yml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/docs/conf.py` & `erpbrasil.edoc-2.5.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 source_suffix = '.rst'
 master_doc = 'index'
 project = 'erpbrasil.edoc'
 year = '2019'
 author = 'Luis Felipe Mileo'
 copyright = '{0}, {1}'.format(year, author)
-version = release = '2.5.0'
+version = release = '2.5.1'
 
 pygments_style = 'trac'
 templates_path = ['.']
 extlinks = {
     'issue': ('https://github.com/erpbrasil/erpbrasil.edoc/issues/%s', '#'),
     'pr': ('https://github.com/erpbrasil/erpbrasil.edoc/pull/%s', 'PR #'),
 }
```

### Comparing `erpbrasil.edoc-2.5.0/setup.py` & `erpbrasil.edoc-2.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         encoding=kwargs.get('encoding', 'utf8')
     ) as fh:
         return fh.read()
 
 
 setup(
     name='erpbrasil.edoc',
-    version='2.5.0',
+    version='2.5.1',
     license='MIT',
     description='Emissão de documentos fiscais e outras obrigações (NF-E, NFS-E, MDF-E, CT-E, REINF, E-SOCIAL)',
     long_description='%s\n%s' % (
         re.compile('^.. start-badges.*^.. end-badges', re.M | re.S).sub('', read('README.rst')),
         re.sub(':[a-z]+:`~?(.*?)`', r'``\1``', read('CHANGELOG.rst'))
     ),
     author='Luis Felipe Mileo',
```

### Comparing `erpbrasil.edoc-2.5.0/src/erpbrasil/edoc/chave.py` & `erpbrasil.edoc-2.5.1/src/erpbrasil/edoc/chave.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/src/erpbrasil/edoc/cli.py` & `erpbrasil.edoc-2.5.1/src/erpbrasil/edoc/cli.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/src/erpbrasil/edoc/edoc.py` & `erpbrasil.edoc-2.5.1/src/erpbrasil/edoc/edoc.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/src/erpbrasil/edoc/mde.py` & `erpbrasil.edoc-2.5.1/src/erpbrasil/edoc/mde.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/src/erpbrasil/edoc/mdfe.py` & `erpbrasil.edoc-2.5.1/src/erpbrasil/edoc/mdfe.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/src/erpbrasil/edoc/nfce.py` & `erpbrasil.edoc-2.5.1/src/erpbrasil/edoc/nfce.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,21 +253,19 @@
                  qrcode_versao="2", csc_token=None, csc_code=None):
         super().__init__(transmissao, uf, versao, ambiente)
         self.mod = str(mod)
         self.qrcode_versao = str(qrcode_versao)
         self.csc_token = str(csc_token)
         self.csc_code = str(csc_code)
 
-    def monta_qrcode(self, edoc):
-        nfce_chave = edoc.infNFe.Id.replace("NFe", "")
-        pre_qrcode = self._build_pre_qrcode(nfce_chave)
+    def monta_qrcode(self, chave):
+        pre_qrcode = self._build_pre_qrcode(chave)
         pre_qrcode_with_csc = pre_qrcode + f"{self.csc_code}"
         qr_hash = self._compute_qr_hash(pre_qrcode_with_csc)
-        qrcode = self._build_qrcode(pre_qrcode, qr_hash)
-        edoc.infNFeSupl = infNFeSuplType(qrCode=qrcode, urlChave=self.consulta_qrcode_url)
+        return self._build_qrcode(pre_qrcode, qr_hash)
 
     def _build_pre_qrcode(self, nfce_chave):
         return f"{nfce_chave}|{self.qrcode_versao}|{self.ambiente}|{self.csc_token}"
 
     def _compute_qr_hash(self, pre_qrcode_with_csc):
         hash_object = hashlib.sha1(pre_qrcode_with_csc.encode("utf-8"))
         return hash_object.hexdigest().upper()
```

### Comparing `erpbrasil.edoc-2.5.0/src/erpbrasil/edoc/nfe.py` & `erpbrasil.edoc-2.5.1/src/erpbrasil/edoc/nfe.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/src/erpbrasil/edoc/nfse.py` & `erpbrasil.edoc-2.5.1/src/erpbrasil/edoc/nfse.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/src/erpbrasil/edoc/provedores/cidades.py` & `erpbrasil.edoc-2.5.1/src/erpbrasil/edoc/provedores/cidades.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/src/erpbrasil/edoc/provedores/dsf.py` & `erpbrasil.edoc-2.5.1/src/erpbrasil/edoc/provedores/dsf.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/src/erpbrasil/edoc/provedores/ginfes.py` & `erpbrasil.edoc-2.5.1/src/erpbrasil/edoc/provedores/ginfes.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/src/erpbrasil/edoc/provedores/issnet.py` & `erpbrasil.edoc-2.5.1/src/erpbrasil/edoc/provedores/issnet.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/src/erpbrasil/edoc/provedores/paulistana.py` & `erpbrasil.edoc-2.5.1/src/erpbrasil/edoc/provedores/paulistana.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/src/erpbrasil/edoc/resposta.py` & `erpbrasil.edoc-2.5.1/src/erpbrasil/edoc/resposta.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/src/erpbrasil.edoc.egg-info/PKG-INFO` & `erpbrasil.edoc-2.5.1/src/erpbrasil.edoc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erpbrasil.edoc
-Version: 2.5.0
+Version: 2.5.1
 Summary: Emissão de documentos fiscais e outras obrigações (NF-E, NFS-E, MDF-E, CT-E, REINF, E-SOCIAL)
 Home-page: https://github.com/erpbrasil/erpbrasil.edoc
 Author: Luis Felipe Mileo
 Author-email: mileo@kmee.com.br
 License: MIT
 Project-URL: Documentation, https://erpbrasiledoc.readthedocs.io/
 Project-URL: Changelog, https://erpbrasiledoc.readthedocs.io/en/latest/changelog.html
```

### Comparing `erpbrasil.edoc-2.5.0/src/erpbrasil.edoc.egg-info/SOURCES.txt` & `erpbrasil.edoc-2.5.1/src/erpbrasil.edoc.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 .appveyor.yml
 .bumpversion.cfg
 .cookiecutterrc
 .coveragerc
 .editorconfig
-.gitignore
 .travis.yml
 AUTHORS.rst
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE
 MANIFEST.in
 README.rst
```

### Comparing `erpbrasil.edoc-2.5.0/tests/fixtures/dummy_cert.pfx` & `erpbrasil.edoc-2.5.1/tests/fixtures/dummy_cert.pfx`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/tests/fixtures/vcr_cassettes/test_cancelar_documento.yaml` & `erpbrasil.edoc-2.5.1/tests/fixtures/vcr_cassettes/test_cancelar_documento.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/tests/fixtures/vcr_cassettes/test_cancelar_documento_ginfes.yaml` & `erpbrasil.edoc-2.5.1/tests/fixtures/vcr_cassettes/test_cancelar_documento_ginfes.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/tests/fixtures/vcr_cassettes/test_chave.yaml` & `erpbrasil.edoc-2.5.1/tests/fixtures/vcr_cassettes/test_chave.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/tests/fixtures/vcr_cassettes/test_ciencia_da_operacao.yaml` & `erpbrasil.edoc-2.5.1/tests/fixtures/vcr_cassettes/test_ciencia_da_operacao.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/tests/fixtures/vcr_cassettes/test_confirmacao_da_operacao.yaml` & `erpbrasil.edoc-2.5.1/tests/fixtures/vcr_cassettes/test_confirmacao_da_operacao.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/tests/fixtures/vcr_cassettes/test_consulta_documento.yaml` & `erpbrasil.edoc-2.5.1/tests/fixtures/vcr_cassettes/test_consulta_documento.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/tests/fixtures/vcr_cassettes/test_consulta_documento_ginfes.yaml` & `erpbrasil.edoc-2.5.1/tests/fixtures/vcr_cassettes/test_consulta_documento_ginfes.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/tests/fixtures/vcr_cassettes/test_desconhecimento_da_operacao.yaml` & `erpbrasil.edoc-2.5.1/tests/fixtures/vcr_cassettes/test_desconhecimento_da_operacao.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/tests/fixtures/vcr_cassettes/test_envia_documento.yaml` & `erpbrasil.edoc-2.5.1/tests/fixtures/vcr_cassettes/test_envia_documento.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/tests/fixtures/vcr_cassettes/test_envia_documento_ginfes.yaml` & `erpbrasil.edoc-2.5.1/tests/fixtures/vcr_cassettes/test_envia_documento_ginfes.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/tests/fixtures/vcr_cassettes/test_nsu_especifico.yaml` & `erpbrasil.edoc-2.5.1/tests/fixtures/vcr_cassettes/test_nsu_especifico.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/tests/fixtures/vcr_cassettes/test_operacao_nao_realizada.yaml` & `erpbrasil.edoc-2.5.1/tests/fixtures/vcr_cassettes/test_operacao_nao_realizada.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/tests/fixtures/vcr_cassettes/test_status_servico.yaml` & `erpbrasil.edoc-2.5.1/tests/fixtures/vcr_cassettes/test_status_servico.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/tests/fixtures/vcr_cassettes/test_ultimo_nsu.yaml` & `erpbrasil.edoc-2.5.1/tests/fixtures/vcr_cassettes/test_ultimo_nsu.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/tests/test_erpbrasil_edoc.py` & `erpbrasil.edoc-2.5.1/tests/test_erpbrasil_edoc.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/tests/test_erpbrasil_edoc_manifestacao.py` & `erpbrasil.edoc-2.5.1/tests/test_erpbrasil_edoc_manifestacao.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/tests/test_erpbrasil_edoc_nfse_ginfes.py` & `erpbrasil.edoc-2.5.1/tests/test_erpbrasil_edoc_nfse_ginfes.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/tests/test_erpbrasil_edoc_nfse_paulistana.py` & `erpbrasil.edoc-2.5.1/tests/test_erpbrasil_edoc_nfse_paulistana.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/tests/test_erpbrasil_edoc_situacao.py` & `erpbrasil.edoc-2.5.1/tests/test_erpbrasil_edoc_situacao.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.5.0/tox.ini` & `erpbrasil.edoc-2.5.1/tox.ini`

 * *Files identical despite different names*

