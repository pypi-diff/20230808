# Comparing `tmp/conda-pack-0.7.0.tar.gz` & `tmp/conda-pack-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conda-pack-0.7.0.tar", last modified: Tue Aug  8 06:14:14 2023, max compression
+gzip compressed data, was "conda-pack-0.7.1.tar", last modified: Tue Aug  8 06:17:58 2023, max compression
```

## Comparing `conda-pack-0.7.0.tar` & `conda-pack-0.7.1.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:14:14.131151 conda-pack-0.7.0/
--rw-r--r--   0 uwe        (501) staff       (20)      106 2023-08-08 06:13:31.000000 conda-pack-0.7.0/.coveragerc
--rw-r--r--   0 uwe        (501) staff       (20)       36 2021-04-23 10:05:58.000000 conda-pack-0.7.0/.gitattributes
-drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:14:14.113653 conda-pack-0.7.0/.github/
-drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:14:14.116427 conda-pack-0.7.0/.github/workflows/
--rw-r--r--   0 uwe        (501) staff       (20)     5875 2023-08-08 06:13:31.000000 conda-pack-0.7.0/.github/workflows/main.yml
--rw-r--r--   0 uwe        (501) staff       (20)      107 2021-04-23 10:05:58.000000 conda-pack-0.7.0/.gitignore
--rw-r--r--   0 uwe        (501) staff       (20)     1512 2023-08-08 06:13:31.000000 conda-pack-0.7.0/LICENSE.txt
--rw-r--r--   0 uwe        (501) staff       (20)      180 2023-03-15 20:44:54.000000 conda-pack-0.7.0/MANIFEST.in
--rw-r--r--   0 uwe        (501) staff       (20)     2507 2023-08-08 06:14:14.131223 conda-pack-0.7.0/PKG-INFO
--rw-r--r--   0 uwe        (501) staff       (20)     1588 2023-08-08 06:13:31.000000 conda-pack-0.7.0/README.md
-drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:14:14.116552 conda-pack-0.7.0/conda-recipe/
--rw-r--r--   0 uwe        (501) staff       (20)     1135 2023-08-08 06:13:31.000000 conda-pack-0.7.0/conda-recipe/meta.yaml
-drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:14:14.131662 conda-pack-0.7.0/conda_pack/
--rw-r--r--   0 uwe        (501) staff       (20)      188 2023-08-08 06:13:31.000000 conda-pack-0.7.0/conda_pack/__init__.py
--rw-r--r--   0 uwe        (501) staff       (20)     3014 2023-08-08 06:13:31.000000 conda-pack-0.7.0/conda_pack/_progress.py
--rw-r--r--   0 uwe        (501) staff       (20)      497 2023-08-08 06:14:14.131693 conda-pack-0.7.0/conda_pack/_version.py
--rw-r--r--   0 uwe        (501) staff       (20)     8939 2023-08-08 06:13:31.000000 conda-pack-0.7.0/conda_pack/cli.py
--rw-r--r--   0 uwe        (501) staff       (20)     1301 2023-08-08 06:13:31.000000 conda-pack-0.7.0/conda_pack/compat.py
--rw-r--r--   0 uwe        (501) staff       (20)    45493 2023-08-08 06:13:31.000000 conda-pack-0.7.0/conda_pack/core.py
--rw-r--r--   0 uwe        (501) staff       (20)    17342 2023-08-08 06:13:31.000000 conda-pack-0.7.0/conda_pack/formats.py
--rw-r--r--   0 uwe        (501) staff       (20)     7473 2023-08-08 06:13:31.000000 conda-pack-0.7.0/conda_pack/prefixes.py
-drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:14:14.114023 conda-pack-0.7.0/conda_pack/scripts/
-drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:14:14.119733 conda-pack-0.7.0/conda_pack/scripts/posix/
--rw-r--r--   0 uwe        (501) staff       (20)     2368 2023-08-08 06:13:31.000000 conda-pack-0.7.0/conda_pack/scripts/posix/activate
--rw-r--r--   0 uwe        (501) staff       (20)      878 2021-04-23 10:05:58.000000 conda-pack-0.7.0/conda_pack/scripts/posix/deactivate
--rw-r--r--   0 uwe        (501) staff       (20)      387 2023-08-08 06:13:31.000000 conda-pack-0.7.0/conda_pack/scripts/posix/parcel
-drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:14:14.120117 conda-pack-0.7.0/conda_pack/scripts/windows/
--rw-r--r--   0 uwe        (501) staff       (20)     1906 2021-04-23 10:05:58.000000 conda-pack-0.7.0/conda_pack/scripts/windows/activate.bat
--rw-r--r--   0 uwe        (501) staff       (20)     1564 2023-08-08 06:13:31.000000 conda-pack-0.7.0/conda_pack/scripts/windows/deactivate.bat
-drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:14:14.120755 conda-pack-0.7.0/conda_pack/tests/
--rw-r--r--   0 uwe        (501) staff       (20)        0 2021-04-23 10:05:58.000000 conda-pack-0.7.0/conda_pack/tests/__init__.py
--rw-r--r--   0 uwe        (501) staff       (20)      747 2023-08-08 06:13:31.000000 conda-pack-0.7.0/conda_pack/tests/conftest.py
--rw-r--r--   0 uwe        (501) staff       (20)     4000 2023-08-08 06:13:31.000000 conda-pack-0.7.0/conda_pack/tests/test_cli.py
--rw-r--r--   0 uwe        (501) staff       (20)    20960 2023-08-08 06:13:31.000000 conda-pack-0.7.0/conda_pack/tests/test_core.py
--rw-r--r--   0 uwe        (501) staff       (20)     8125 2023-08-08 06:13:31.000000 conda-pack-0.7.0/conda_pack/tests/test_formats.py
-drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:14:14.119145 conda-pack-0.7.0/conda_pack.egg-info/
--rw-r--r--   0 uwe        (501) staff       (20)     2507 2023-08-08 06:14:14.000000 conda-pack-0.7.0/conda_pack.egg-info/PKG-INFO
--rw-r--r--   0 uwe        (501) staff       (20)     2004 2023-08-08 06:14:14.000000 conda-pack-0.7.0/conda_pack.egg-info/SOURCES.txt
--rw-r--r--   0 uwe        (501) staff       (20)        1 2023-08-08 06:14:14.000000 conda-pack-0.7.0/conda_pack.egg-info/dependency_links.txt
--rw-r--r--   0 uwe        (501) staff       (20)       51 2023-08-08 06:14:14.000000 conda-pack-0.7.0/conda_pack.egg-info/entry_points.txt
--rw-r--r--   0 uwe        (501) staff       (20)        1 2021-04-23 10:07:30.000000 conda-pack-0.7.0/conda_pack.egg-info/not-zip-safe
--rw-r--r--   0 uwe        (501) staff       (20)       11 2023-08-08 06:14:14.000000 conda-pack-0.7.0/conda_pack.egg-info/requires.txt
--rw-r--r--   0 uwe        (501) staff       (20)       11 2023-08-08 06:14:14.000000 conda-pack-0.7.0/conda_pack.egg-info/top_level.txt
-drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:14:14.121004 conda-pack-0.7.0/docs/
--rw-r--r--   0 uwe        (501) staff       (20)      611 2023-08-08 06:13:31.000000 conda-pack-0.7.0/docs/Makefile
--rw-r--r--   0 uwe        (501) staff       (20)      818 2021-04-23 10:05:58.000000 conda-pack-0.7.0/docs/make.bat
-drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:14:14.122256 conda-pack-0.7.0/docs/source/
-drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:14:14.122374 conda-pack-0.7.0/docs/source/_static/
--rw-r--r--   0 uwe        (501) staff       (20)       31 2021-04-23 10:05:58.000000 conda-pack-0.7.0/docs/source/_static/custom.css
-drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:14:14.122599 conda-pack-0.7.0/docs/source/_templates/
--rw-r--r--   0 uwe        (501) staff       (20)      125 2021-04-23 10:05:58.000000 conda-pack-0.7.0/docs/source/_templates/help.html
--rw-r--r--   0 uwe        (501) staff       (20)      217 2021-04-23 10:05:58.000000 conda-pack-0.7.0/docs/source/api.rst
--rw-r--r--   0 uwe        (501) staff       (20)       80 2021-04-23 10:05:58.000000 conda-pack-0.7.0/docs/source/cli.rst
--rw-r--r--   0 uwe        (501) staff       (20)     1081 2023-08-08 06:13:31.000000 conda-pack-0.7.0/docs/source/conf.py
--rw-r--r--   0 uwe        (501) staff       (20)     5590 2023-08-08 06:13:31.000000 conda-pack-0.7.0/docs/source/index.rst
--rw-r--r--   0 uwe        (501) staff       (20)     3160 2023-08-08 06:13:31.000000 conda-pack-0.7.0/docs/source/parcel.rst
--rw-r--r--   0 uwe        (501) staff       (20)     5875 2021-04-23 10:05:58.000000 conda-pack-0.7.0/docs/source/spark.rst
--rw-r--r--   0 uwe        (501) staff       (20)     4511 2023-08-08 06:13:31.000000 conda-pack-0.7.0/docs/source/squashfs.rst
--rw-r--r--   0 uwe        (501) staff       (20)      292 2023-08-08 06:14:14.131490 conda-pack-0.7.0/setup.cfg
--rw-r--r--   0 uwe        (501) staff       (20)     1491 2023-08-08 06:13:31.000000 conda-pack-0.7.0/setup.py
-drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:14:14.122841 conda-pack-0.7.0/testing/
-drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:14:14.123239 conda-pack-0.7.0/testing/env_yamls/
--rw-r--r--   0 uwe        (501) staff       (20)       84 2023-08-08 06:13:31.000000 conda-pack-0.7.0/testing/env_yamls/activate_scripts.yml
--rw-r--r--   0 uwe        (501) staff       (20)       55 2021-04-23 10:05:58.000000 conda-pack-0.7.0/testing/env_yamls/has_conda.yml
--rw-r--r--   0 uwe        (501) staff       (20)       72 2021-04-23 10:05:58.000000 conda-pack-0.7.0/testing/env_yamls/nopython.yml
-drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:14:14.129902 conda-pack-0.7.0/testing/extra_scripts/
--rw-r--r--   0 uwe        (501) staff       (20)       28 2021-04-23 10:05:58.000000 conda-pack-0.7.0/testing/extra_scripts/conda_pack_test_activate.bat
--rw-r--r--   0 uwe        (501) staff       (20)       29 2021-04-23 10:05:58.000000 conda-pack-0.7.0/testing/extra_scripts/conda_pack_test_activate.sh
--rw-r--r--   0 uwe        (501) staff       (20)       29 2021-04-23 10:05:58.000000 conda-pack-0.7.0/testing/extra_scripts/conda_pack_test_deactivate.bat
--rw-r--r--   0 uwe        (501) staff       (20)       26 2021-04-23 10:05:58.000000 conda-pack-0.7.0/testing/extra_scripts/conda_pack_test_deactivate.sh
--rwxr-xr-x   0 uwe        (501) staff       (20)     2967 2023-08-08 06:13:31.000000 conda-pack-0.7.0/testing/setup_envs.sh
-drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:14:14.114828 conda-pack-0.7.0/testing/test_packages/
-drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:14:14.130061 conda-pack-0.7.0/testing/test_packages/conda_pack_test_lib1/
-drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:14:14.130214 conda-pack-0.7.0/testing/test_packages/conda_pack_test_lib1/conda.recipe/
--rw-r--r--   0 uwe        (501) staff       (20)      423 2023-08-08 06:13:31.000000 conda-pack-0.7.0/testing/test_packages/conda_pack_test_lib1/conda.recipe/meta.yaml
-drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:14:14.130459 conda-pack-0.7.0/testing/test_packages/conda_pack_test_lib1/conda_pack_test_lib1/
--rw-r--r--   0 uwe        (501) staff       (20)        0 2021-04-23 10:05:58.000000 conda-pack-0.7.0/testing/test_packages/conda_pack_test_lib1/conda_pack_test_lib1/__init__.py
--rw-r--r--   0 uwe        (501) staff       (20)       21 2021-04-23 10:05:58.000000 conda-pack-0.7.0/testing/test_packages/conda_pack_test_lib1/conda_pack_test_lib1/cli.py
--rw-r--r--   0 uwe        (501) staff       (20)      328 2021-04-23 10:05:58.000000 conda-pack-0.7.0/testing/test_packages/conda_pack_test_lib1/setup.py
-drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:14:14.130612 conda-pack-0.7.0/testing/test_packages/conda_pack_test_lib2/
-drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:14:14.130772 conda-pack-0.7.0/testing/test_packages/conda_pack_test_lib2/conda.recipe/
--rw-r--r--   0 uwe        (501) staff       (20)      406 2023-08-08 06:13:31.000000 conda-pack-0.7.0/testing/test_packages/conda_pack_test_lib2/conda.recipe/meta.yaml
-drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:14:14.131011 conda-pack-0.7.0/testing/test_packages/conda_pack_test_lib2/conda_pack_test_lib2/
--rw-r--r--   0 uwe        (501) staff       (20)        0 2021-04-23 10:05:58.000000 conda-pack-0.7.0/testing/test_packages/conda_pack_test_lib2/conda_pack_test_lib2/__init__.py
--rw-r--r--   0 uwe        (501) staff       (20)       21 2021-04-23 10:05:58.000000 conda-pack-0.7.0/testing/test_packages/conda_pack_test_lib2/conda_pack_test_lib2/cli.py
--rw-r--r--   0 uwe        (501) staff       (20)      328 2021-04-23 10:05:58.000000 conda-pack-0.7.0/testing/test_packages/conda_pack_test_lib2/setup.py
--rw-r--r--   0 uwe        (501) staff       (20)    80044 2023-08-08 06:13:31.000000 conda-pack-0.7.0/versioneer.py
+drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:17:58.686389 conda-pack-0.7.1/
+-rw-r--r--   0 uwe        (501) staff       (20)      105 2023-08-08 06:17:51.000000 conda-pack-0.7.1/.coveragerc
+-rw-r--r--   0 uwe        (501) staff       (20)       36 2021-04-23 10:05:58.000000 conda-pack-0.7.1/.gitattributes
+drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:17:58.669729 conda-pack-0.7.1/.github/
+drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:17:58.679402 conda-pack-0.7.1/.github/workflows/
+-rw-r--r--   0 uwe        (501) staff       (20)     5506 2023-08-08 06:17:51.000000 conda-pack-0.7.1/.github/workflows/main.yml
+-rw-r--r--   0 uwe        (501) staff       (20)      107 2021-04-23 10:05:58.000000 conda-pack-0.7.1/.gitignore
+-rw-r--r--   0 uwe        (501) staff       (20)     1509 2023-08-08 06:17:51.000000 conda-pack-0.7.1/LICENSE.txt
+-rw-r--r--   0 uwe        (501) staff       (20)      180 2023-03-15 20:44:54.000000 conda-pack-0.7.1/MANIFEST.in
+-rw-r--r--   0 uwe        (501) staff       (20)     2617 2023-08-08 06:17:58.686456 conda-pack-0.7.1/PKG-INFO
+-rw-r--r--   0 uwe        (501) staff       (20)     1748 2023-08-08 06:17:51.000000 conda-pack-0.7.1/README.md
+drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:17:58.679521 conda-pack-0.7.1/conda-recipe/
+-rw-r--r--   0 uwe        (501) staff       (20)     1147 2023-08-08 06:17:51.000000 conda-pack-0.7.1/conda-recipe/meta.yaml
+drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:17:58.686882 conda-pack-0.7.1/conda_pack/
+-rw-r--r--   0 uwe        (501) staff       (20)      132 2023-08-08 06:17:51.000000 conda-pack-0.7.1/conda_pack/__init__.py
+-rw-r--r--   0 uwe        (501) staff       (20)     2920 2023-08-08 06:17:51.000000 conda-pack-0.7.1/conda_pack/_progress.py
+-rw-r--r--   0 uwe        (501) staff       (20)      497 2023-08-08 06:17:58.686921 conda-pack-0.7.1/conda_pack/_version.py
+-rw-r--r--   0 uwe        (501) staff       (20)     8722 2023-08-08 06:17:51.000000 conda-pack-0.7.1/conda_pack/cli.py
+-rw-r--r--   0 uwe        (501) staff       (20)     1302 2023-08-08 06:17:51.000000 conda-pack-0.7.1/conda_pack/compat.py
+-rw-r--r--   0 uwe        (501) staff       (20)    45440 2023-08-08 06:17:51.000000 conda-pack-0.7.1/conda_pack/core.py
+-rw-r--r--   0 uwe        (501) staff       (20)    16469 2023-08-08 06:17:51.000000 conda-pack-0.7.1/conda_pack/formats.py
+-rw-r--r--   0 uwe        (501) staff       (20)     7766 2023-08-08 06:17:51.000000 conda-pack-0.7.1/conda_pack/prefixes.py
+drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:17:58.670101 conda-pack-0.7.1/conda_pack/scripts/
+drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:17:58.681828 conda-pack-0.7.1/conda_pack/scripts/posix/
+-rw-r--r--   0 uwe        (501) staff       (20)     2364 2023-08-08 06:17:51.000000 conda-pack-0.7.1/conda_pack/scripts/posix/activate
+-rw-r--r--   0 uwe        (501) staff       (20)      878 2021-04-23 10:05:58.000000 conda-pack-0.7.1/conda_pack/scripts/posix/deactivate
+-rwxr-xr-x   0 uwe        (501) staff       (20)      387 2023-08-08 06:17:51.000000 conda-pack-0.7.1/conda_pack/scripts/posix/parcel
+drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:17:58.682216 conda-pack-0.7.1/conda_pack/scripts/windows/
+-rw-r--r--   0 uwe        (501) staff       (20)     1906 2021-04-23 10:05:58.000000 conda-pack-0.7.1/conda_pack/scripts/windows/activate.bat
+-rw-r--r--   0 uwe        (501) staff       (20)     1562 2023-08-08 06:17:51.000000 conda-pack-0.7.1/conda_pack/scripts/windows/deactivate.bat
+drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:17:58.682778 conda-pack-0.7.1/conda_pack/tests/
+-rw-r--r--   0 uwe        (501) staff       (20)        0 2021-04-23 10:05:58.000000 conda-pack-0.7.1/conda_pack/tests/__init__.py
+-rw-r--r--   0 uwe        (501) staff       (20)      683 2023-08-08 06:17:51.000000 conda-pack-0.7.1/conda_pack/tests/conftest.py
+-rw-r--r--   0 uwe        (501) staff       (20)     3714 2023-08-08 06:17:51.000000 conda-pack-0.7.1/conda_pack/tests/test_cli.py
+-rw-r--r--   0 uwe        (501) staff       (20)    20668 2023-08-08 06:17:51.000000 conda-pack-0.7.1/conda_pack/tests/test_core.py
+-rw-r--r--   0 uwe        (501) staff       (20)     8125 2023-08-08 06:17:51.000000 conda-pack-0.7.1/conda_pack/tests/test_formats.py
+drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:17:58.681370 conda-pack-0.7.1/conda_pack.egg-info/
+-rw-r--r--   0 uwe        (501) staff       (20)     2617 2023-08-08 06:17:58.000000 conda-pack-0.7.1/conda_pack.egg-info/PKG-INFO
+-rw-r--r--   0 uwe        (501) staff       (20)     2004 2023-08-08 06:17:58.000000 conda-pack-0.7.1/conda_pack.egg-info/SOURCES.txt
+-rw-r--r--   0 uwe        (501) staff       (20)        1 2023-08-08 06:17:58.000000 conda-pack-0.7.1/conda_pack.egg-info/dependency_links.txt
+-rw-r--r--   0 uwe        (501) staff       (20)       51 2023-08-08 06:17:58.000000 conda-pack-0.7.1/conda_pack.egg-info/entry_points.txt
+-rw-r--r--   0 uwe        (501) staff       (20)        1 2021-04-23 10:07:30.000000 conda-pack-0.7.1/conda_pack.egg-info/not-zip-safe
+-rw-r--r--   0 uwe        (501) staff       (20)       11 2023-08-08 06:17:58.000000 conda-pack-0.7.1/conda_pack.egg-info/requires.txt
+-rw-r--r--   0 uwe        (501) staff       (20)       11 2023-08-08 06:17:58.000000 conda-pack-0.7.1/conda_pack.egg-info/top_level.txt
+drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:17:58.683013 conda-pack-0.7.1/docs/
+-rw-r--r--   0 uwe        (501) staff       (20)      612 2023-08-08 06:17:51.000000 conda-pack-0.7.1/docs/Makefile
+-rw-r--r--   0 uwe        (501) staff       (20)      818 2021-04-23 10:05:58.000000 conda-pack-0.7.1/docs/make.bat
+drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:17:58.683867 conda-pack-0.7.1/docs/source/
+drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:17:58.683975 conda-pack-0.7.1/docs/source/_static/
+-rw-r--r--   0 uwe        (501) staff       (20)       31 2021-04-23 10:05:58.000000 conda-pack-0.7.1/docs/source/_static/custom.css
+drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:17:58.684118 conda-pack-0.7.1/docs/source/_templates/
+-rw-r--r--   0 uwe        (501) staff       (20)      125 2021-04-23 10:05:58.000000 conda-pack-0.7.1/docs/source/_templates/help.html
+-rw-r--r--   0 uwe        (501) staff       (20)      217 2021-04-23 10:05:58.000000 conda-pack-0.7.1/docs/source/api.rst
+-rw-r--r--   0 uwe        (501) staff       (20)       80 2021-04-23 10:05:58.000000 conda-pack-0.7.1/docs/source/cli.rst
+-rw-r--r--   0 uwe        (501) staff       (20)     1082 2023-08-08 06:17:51.000000 conda-pack-0.7.1/docs/source/conf.py
+-rw-r--r--   0 uwe        (501) staff       (20)     5761 2023-08-08 06:17:51.000000 conda-pack-0.7.1/docs/source/index.rst
+-rw-r--r--   0 uwe        (501) staff       (20)     3158 2023-08-08 06:17:51.000000 conda-pack-0.7.1/docs/source/parcel.rst
+-rw-r--r--   0 uwe        (501) staff       (20)     5875 2021-04-23 10:05:58.000000 conda-pack-0.7.1/docs/source/spark.rst
+-rw-r--r--   0 uwe        (501) staff       (20)     4512 2023-08-08 06:17:51.000000 conda-pack-0.7.1/docs/source/squashfs.rst
+-rw-r--r--   0 uwe        (501) staff       (20)      335 2023-08-08 06:17:58.686706 conda-pack-0.7.1/setup.cfg
+-rw-r--r--   0 uwe        (501) staff       (20)     1432 2023-08-08 06:17:51.000000 conda-pack-0.7.1/setup.py
+drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:17:58.684256 conda-pack-0.7.1/testing/
+drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:17:58.684610 conda-pack-0.7.1/testing/env_yamls/
+-rw-r--r--   0 uwe        (501) staff       (20)       84 2023-08-08 06:17:51.000000 conda-pack-0.7.1/testing/env_yamls/activate_scripts.yml
+-rw-r--r--   0 uwe        (501) staff       (20)       55 2021-04-23 10:05:58.000000 conda-pack-0.7.1/testing/env_yamls/has_conda.yml
+-rw-r--r--   0 uwe        (501) staff       (20)       72 2021-04-23 10:05:58.000000 conda-pack-0.7.1/testing/env_yamls/nopython.yml
+drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:17:58.685181 conda-pack-0.7.1/testing/extra_scripts/
+-rw-r--r--   0 uwe        (501) staff       (20)       28 2021-04-23 10:05:58.000000 conda-pack-0.7.1/testing/extra_scripts/conda_pack_test_activate.bat
+-rw-r--r--   0 uwe        (501) staff       (20)       29 2021-04-23 10:05:58.000000 conda-pack-0.7.1/testing/extra_scripts/conda_pack_test_activate.sh
+-rw-r--r--   0 uwe        (501) staff       (20)       29 2021-04-23 10:05:58.000000 conda-pack-0.7.1/testing/extra_scripts/conda_pack_test_deactivate.bat
+-rw-r--r--   0 uwe        (501) staff       (20)       26 2021-04-23 10:05:58.000000 conda-pack-0.7.1/testing/extra_scripts/conda_pack_test_deactivate.sh
+-rwxr-xr-x   0 uwe        (501) staff       (20)     2972 2023-08-08 06:17:51.000000 conda-pack-0.7.1/testing/setup_envs.sh
+drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:17:58.670855 conda-pack-0.7.1/testing/test_packages/
+drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:17:58.685326 conda-pack-0.7.1/testing/test_packages/conda_pack_test_lib1/
+drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:17:58.685476 conda-pack-0.7.1/testing/test_packages/conda_pack_test_lib1/conda.recipe/
+-rw-r--r--   0 uwe        (501) staff       (20)      434 2023-08-08 06:17:51.000000 conda-pack-0.7.1/testing/test_packages/conda_pack_test_lib1/conda.recipe/meta.yaml
+drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:17:58.685703 conda-pack-0.7.1/testing/test_packages/conda_pack_test_lib1/conda_pack_test_lib1/
+-rw-r--r--   0 uwe        (501) staff       (20)        0 2021-04-23 10:05:58.000000 conda-pack-0.7.1/testing/test_packages/conda_pack_test_lib1/conda_pack_test_lib1/__init__.py
+-rw-r--r--   0 uwe        (501) staff       (20)       21 2021-04-23 10:05:58.000000 conda-pack-0.7.1/testing/test_packages/conda_pack_test_lib1/conda_pack_test_lib1/cli.py
+-rw-r--r--   0 uwe        (501) staff       (20)      328 2021-04-23 10:05:58.000000 conda-pack-0.7.1/testing/test_packages/conda_pack_test_lib1/setup.py
+drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:17:58.685847 conda-pack-0.7.1/testing/test_packages/conda_pack_test_lib2/
+drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:17:58.686004 conda-pack-0.7.1/testing/test_packages/conda_pack_test_lib2/conda.recipe/
+-rw-r--r--   0 uwe        (501) staff       (20)      405 2023-08-08 06:17:51.000000 conda-pack-0.7.1/testing/test_packages/conda_pack_test_lib2/conda.recipe/meta.yaml
+drwxr-xr-x   0 uwe        (501) staff       (20)        0 2023-08-08 06:17:58.686238 conda-pack-0.7.1/testing/test_packages/conda_pack_test_lib2/conda_pack_test_lib2/
+-rw-r--r--   0 uwe        (501) staff       (20)        0 2021-04-23 10:05:58.000000 conda-pack-0.7.1/testing/test_packages/conda_pack_test_lib2/conda_pack_test_lib2/__init__.py
+-rw-r--r--   0 uwe        (501) staff       (20)       21 2021-04-23 10:05:58.000000 conda-pack-0.7.1/testing/test_packages/conda_pack_test_lib2/conda_pack_test_lib2/cli.py
+-rw-r--r--   0 uwe        (501) staff       (20)      328 2021-04-23 10:05:58.000000 conda-pack-0.7.1/testing/test_packages/conda_pack_test_lib2/setup.py
+-rw-r--r--   0 uwe        (501) staff       (20)    80045 2023-08-08 06:17:51.000000 conda-pack-0.7.1/versioneer.py
```

### Comparing `conda-pack-0.7.0/.github/workflows/main.yml` & `conda-pack-0.7.1/.github/workflows/main.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,150 +1,142 @@
 name: Build
 on:
   push:
     branches:
-      - master
+      - main
     tags:
       - '*'
   pull_request:
     branches:
-      - master
+      - main
 jobs:
   package:
     runs-on: ubuntu-latest
     steps:
     - name: Retrieve the source code
-      uses: actions/checkout@v2
+      uses: actions/checkout@v3
       with:
         fetch-depth: 0
     - name: Install build dependencies
       run: |
         source $CONDA/bin/activate
         conda config --append channels conda-forge
-        conda install -y conda-build conda-verify flake8 sphinx numpydoc sphinxcontrib-autoprogram make
+        conda install -y conda-build conda-verify sphinx numpydoc sphinxcontrib-autoprogram make
         python -m pip install -e .
-    - name: Verify flake8 compliance
-      run: |
-        source $CONDA/bin/activate
-        flake8 conda_pack
     - name: Build the documentation as a test
       run: |
         source $CONDA/bin/activate
         cd docs
         make html
     - name: Build the package
       run: conda build conda-recipe --no-test
     - name: Reduce the size of the build artifact
       run: rm -rf /usr/share/miniconda/conda-bld/{git_cache,work,conda-pack*,*/.cache}
     - name: Upload the build artifact
-      uses: actions/upload-artifact@v2
+      uses: actions/upload-artifact@v3
       with:
         name: package-${{ github.sha }}
         path: /usr/share/miniconda/conda-bld
+        retention-days: 5
   testbed:
     defaults:
       run:
         shell: bash
     runs-on: ${{ matrix.os }}
-    # Need to allow the ::set-env command until we get it replaced
-    env:
-        ACTIONS_ALLOW_UNSECURE_COMMANDS: 'true'
     strategy:
       matrix:
         os: [ubuntu-latest,macos-latest,windows-latest]
     steps:
     - name: Retrieve the source code
-      uses: actions/checkout@v2
+      uses: actions/checkout@v3
     - id: conda-root
       name: Set CONDA_ROOT
       run: |
           CONDA_ROOT=$(dirname $GITHUB_WORKSPACE)/conda
-          echo "::set-output name=value::$(dirname $GITHUB_WORKSPACE)/conda"
-          echo "::set-env name=CONDA_ROOT::$CONDA_ROOT"
+          echo "value=$(dirname $GITHUB_WORKSPACE)/conda" >> $GITHUB_OUTPUT
+          echo "CONDA_ROOT=$CONDA_ROOT" >> $GITHUB_ENV
           echo "CONDA_ROOT: $CONDA_ROOT"
     # Use a smaller cache entry to enable a quicker exit if we
     # have already built the testbed. Any small file will do
     - id: cache-key
       name: Retrieve cache key
-      uses: actions/cache@v2
+      uses: actions/cache@v3
       with:
         path: LICENSE.txt
         key: key-${{ matrix.os }}-${{ hashFiles('testing') }}-5
     - name: Retrieve or create the testbed cache
       if: steps.cache-key.outputs.cache-hit != 'true'
-      uses: actions/cache@v2
+      uses: actions/cache@v3
       with:
         path: ${{ steps.conda-root.outputs.value }}
         key: testbed-${{ matrix.os }}-${{ hashFiles('testing') }}-5
     - name: Verify or create the testbed
       if: steps.cache-key.outputs.cache-hit != 'true'
       run: testing/setup_envs.sh
   tests:
     defaults:
       run:
         shell: bash
     runs-on: ${{ matrix.os }}
-    # Need to allow the ::set-env command until we get it replaced
-    env:
-        ACTIONS_ALLOW_UNSECURE_COMMANDS: 'true'
     needs: [package,testbed]
     strategy:
       fail-fast: false
       matrix:
         os: [macos-latest,ubuntu-latest,windows-latest]
-        pyver: ["3.6","3.7","3.8","3.9","3.10"]
+        pyver: ["3.7","3.8","3.9","3.10"]
         include:
           # include the appropriate dependencies for testing SquashFS on each OS
           - os: macos-latest
             squashfs_deps: "conda-forge::squashfs-tools"
           - os: ubuntu-latest
             squashfs_deps: "conda-forge::squashfs-tools conda-forge::squashfuse"
           - os: windows-latest
             squashfs_deps: ""
     steps:
     - name: Retrieve the source code
-      uses: actions/checkout@v2
+      uses: actions/checkout@v3
     - id: conda-root
       name: Set CONDA_ROOT
       run: |
           CONDA_ROOT=$(dirname $GITHUB_WORKSPACE)/conda
-          echo "::set-output name=value::$(dirname $GITHUB_WORKSPACE)/conda"
-          echo "::set-env name=CONDA_ROOT::$CONDA_ROOT"
+          echo "value=$(dirname $GITHUB_WORKSPACE)/conda" >> $GITHUB_OUTPUT
+          echo "CONDA_ROOT=$CONDA_ROOT" >> $GITHUB_ENV
           echo "CONDA_ROOT: $CONDA_ROOT"
     - name: Retrieve the testbed cache
-      uses: actions/cache@v2
+      uses: actions/cache@v3
       with:
         path: ${{ steps.conda-root.outputs.value }}
         key: testbed-${{ matrix.os }}-${{ hashFiles('testing') }}-5
     - name: Download the build artifact
-      uses: actions/download-artifact@v2
+      uses: actions/download-artifact@v3
       with:
         name: package-${{ github.sha }}
         path: conda-bld
     - name: Verify or create the testbed
       run: testing/setup_envs.sh
     - name: Create the test environment and run the tests
       run: |
         source $CONDA_ROOT/etc/profile.d/conda.sh
         conda info -a
         mv conda-bld $CONDA_ROOT/conda-bld
-        conda create -n cptest local::conda-pack conda-forge::pytest python=${{ matrix.pyver }} ${{ matrix.squashfs_deps }}
+        conda create -n cptest local::conda-pack conda-forge::pytest conda-forge::pytest-cov python=${{ matrix.pyver }} ${{ matrix.squashfs_deps }}
         conda activate cptest
-        pytest -v -ss conda_pack/tests
+        pytest -v -ss --cov=conda_pack --cov-branch --cov-report=xml conda_pack/tests
+    - uses: codecov/codecov-action@v3
   upload:
     needs: tests
     runs-on: ubuntu-latest
     if: github.event_name == 'push'
     steps:
     - name: Retrieve the source code
-      uses: actions/checkout@v2
+      uses: actions/checkout@v3
       with:
         fetch-depth: 0
     - name: Download the build artifacts
-      uses: actions/download-artifact@v2
+      uses: actions/download-artifact@v3
       with:
         name: package-${{ github.sha }}
         path: conda-bld
     - name: Install deployment dependencies and build the docs
       run: |
         source $CONDA/bin/activate
         conda config --append channels conda-forge
@@ -162,11 +154,7 @@
       env:
         ANACONDA_TOKEN: ${{ secrets.ANACONDA_TOKEN }}
         GITHUB_REF: ${{ github.ref }}
       run: |
         source $CONDA/bin/activate
         [[ "$GITHUB_REF" =~ ^refs/tags/ ]] || export LABEL="--label dev"
         anaconda --verbose --token $ANACONDA_TOKEN upload --user ctools $LABEL conda-bld/*/*.tar.bz2 --force
-    - name: Clean up older artifacts
-      uses: glassechidna/artifact-cleaner@master
-      with:
-        minimumAge: 86400
```

### Comparing `conda-pack-0.7.0/LICENSE.txt` & `conda-pack-0.7.1/LICENSE.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿Copyright (c) 2017, Jim Crist and contributors
+Copyright (c) 2017, Jim Crist and contributors
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `conda-pack-0.7.0/PKG-INFO` & `conda-pack-0.7.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 Metadata-Version: 2.1
 Name: conda-pack
-Version: 0.7.0
+Version: 0.7.1
 Summary: Package conda environments for redistribution
 Home-page: https://conda.github.io/conda-pack/
 Maintainer: Jim Crist
 Maintainer-email: jiminy.crist@gmail.com
 License: BSD
 Project-URL: Source Code, https://github.com/conda/conda-pack
 Keywords: conda packaging
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Topic :: System :: Software Distribution
 Classifier: Topic :: Software Development :: Build Tools
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Conda-Pack
 
 `conda-pack` is a command line tool for creating relocatable conda
 environments. This is useful for deploying code in a consistent environment,
 potentially in locations where python or conda isn't already installed.
 
 See the <a href="https://conda.github.io/conda-pack/">documentation</a>
 for more information.
 
 Conda-pack is offered under a New BSD license; see the
-<a href="https://github.com/conda/conda-pack/blob/master/LICENSE.txt">license file</a>.
+<a href="https://github.com/conda/conda-pack/blob/main/LICENSE.txt">license file</a>.
 
 ## Build status
 
-| [![Build status](https://github.com/conda/conda-pack/workflows/Build%20and%20test%20the%20package/badge.svg)](https://github.com/conda/conda-pack/actions) [![codecov](https://codecov.io/gh/conda/conda-pack/branch/master/graph/badge.svg)](https://codecov.io/gh/conda/conda-pack) | [![Anaconda-Server Badge](https://anaconda.org/ctools/conda-pack/badges/latest_release_date.svg)](https://anaconda.org/ctools/conda-pack) |
+| [![Build status](https://github.com/conda/conda-pack/actions/workflows/main.yml/badge.svg)](https://github.com/conda/conda-pack/actions/workflows/main.yml) [![codecov](https://codecov.io/gh/conda/conda-pack/branch/main/graph/badge.svg)](https://codecov.io/gh/conda/conda-pack) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/conda/conda-pack/main.svg)](https://results.pre-commit.ci/latest/github/conda/conda-pack/main) | [![Anaconda-Server Badge](https://anaconda.org/ctools/conda-pack/badges/latest_release_date.svg)](https://anaconda.org/ctools/conda-pack) |
 | --- | :-: |
 | [`conda install ctools/label/dev::conda-pack`](https://anaconda.org/ctools/conda-pack) | [![Anaconda-Server Badge](https://anaconda.org/ctools/conda-pack/badges/version.svg)](https://anaconda.org/ctools/conda-pack) |
 | [`conda install defaults::conda-pack`](https://anaconda.org/anaconda/conda-pack) | [![Anaconda-Server Badge](https://anaconda.org/anaconda/conda-pack/badges/version.svg)](https://anaconda.org/anaconda/conda-pack) |
 | [`conda install conda-forge::conda-pack`](https://anaconda.org/conda-forge/conda-pack) | [![Anaconda-Server Badge](https://anaconda.org/conda-forge/conda-pack/badges/version.svg)](https://anaconda.org/conda-forge/conda-pack) |
```

#### html2text {}

```diff
@@ -1,32 +1,33 @@
-Metadata-Version: 2.1 Name: conda-pack Version: 0.7.0 Summary: Package conda
+Metadata-Version: 2.1 Name: conda-pack Version: 0.7.1 Summary: Package conda
 environments for redistribution Home-page: https://conda.github.io/conda-pack/
 Maintainer: Jim Crist Maintainer-email: jiminy.crist@gmail.com License: BSD
 Project-URL: Source Code, https://github.com/conda/conda-pack Keywords: conda
 packaging Classifier: Development Status :: 4 - Beta Classifier: License :: OSI
-Approved :: BSD License Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Topic :: System
-:: Archiving :: Packaging Classifier: Topic :: System :: Software Distribution
-Classifier: Topic :: Software Development :: Build Tools Requires-Python: >=3.6
-Description-Content-Type: text/markdown License-File: LICENSE.txt # Conda-Pack
-`conda-pack` is a command line tool for creating relocatable conda
-environments. This is useful for deploying code in a consistent environment,
-potentially in locations where python or conda isn't already installed. See the
-documentation for more information. Conda-pack is offered under a New BSD
-license; see the license_file. ## Build status | [![Build status](https://
-github.com/conda/conda-pack/workflows/Build%20and%20test%20the%20package/
-badge.svg)](https://github.com/conda/conda-pack/actions) [![codecov](https://
-codecov.io/gh/conda/conda-pack/branch/master/graph/badge.svg)](https://
-codecov.io/gh/conda/conda-pack) | [![Anaconda-Server Badge](https://
-anaconda.org/ctools/conda-pack/badges/latest_release_date.svg)](https://
-anaconda.org/ctools/conda-pack) | | --- | :-: | | [`conda install ctools/label/
-dev::conda-pack`](https://anaconda.org/ctools/conda-pack) | [![Anaconda-Server
-Badge](https://anaconda.org/ctools/conda-pack/badges/version.svg)](https://
-anaconda.org/ctools/conda-pack) | | [`conda install defaults::conda-pack`]
-(https://anaconda.org/anaconda/conda-pack) | [![Anaconda-Server Badge](https://
-anaconda.org/anaconda/conda-pack/badges/version.svg)](https://anaconda.org/
-anaconda/conda-pack) | | [`conda install conda-forge::conda-pack`](https://
-anaconda.org/conda-forge/conda-pack) | [![Anaconda-Server Badge](https://
-anaconda.org/conda-forge/conda-pack/badges/version.svg)](https://anaconda.org/
-conda-forge/conda-pack) |
+Approved :: BSD License Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: System :: Archiving :: Packaging Classifier: Topic ::
+System :: Software Distribution Classifier: Topic :: Software Development ::
+Build Tools Requires-Python: >=3.7 Description-Content-Type: text/markdown
+License-File: LICENSE.txt # Conda-Pack `conda-pack` is a command line tool for
+creating relocatable conda environments. This is useful for deploying code in a
+consistent environment, potentially in locations where python or conda isn't
+already installed. See the documentation for more information. Conda-pack is
+offered under a New BSD license; see the license_file. ## Build status | [!
+[Build status](https://github.com/conda/conda-pack/actions/workflows/main.yml/
+badge.svg)](https://github.com/conda/conda-pack/actions/workflows/main.yml) [!
+[codecov](https://codecov.io/gh/conda/conda-pack/branch/main/graph/badge.svg)]
+(https://codecov.io/gh/conda/conda-pack) [![pre-commit.ci status](https://
+results.pre-commit.ci/badge/github/conda/conda-pack/main.svg)](https://
+results.pre-commit.ci/latest/github/conda/conda-pack/main) | [![Anaconda-Server
+Badge](https://anaconda.org/ctools/conda-pack/badges/latest_release_date.svg)]
+(https://anaconda.org/ctools/conda-pack) | | --- | :-: | | [`conda install
+ctools/label/dev::conda-pack`](https://anaconda.org/ctools/conda-pack) | [!
+[Anaconda-Server Badge](https://anaconda.org/ctools/conda-pack/badges/
+version.svg)](https://anaconda.org/ctools/conda-pack) | | [`conda install
+defaults::conda-pack`](https://anaconda.org/anaconda/conda-pack) | [![Anaconda-
+Server Badge](https://anaconda.org/anaconda/conda-pack/badges/version.svg)]
+(https://anaconda.org/anaconda/conda-pack) | | [`conda install conda-forge::
+conda-pack`](https://anaconda.org/conda-forge/conda-pack) | [![Anaconda-Server
+Badge](https://anaconda.org/conda-forge/conda-pack/badges/version.svg)](https:/
+/anaconda.org/conda-forge/conda-pack) |
```

### Comparing `conda-pack-0.7.0/README.md` & `conda-pack-0.7.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 environments. This is useful for deploying code in a consistent environment,
 potentially in locations where python or conda isn't already installed.
 
 See the <a href="https://conda.github.io/conda-pack/">documentation</a>
 for more information.
 
 Conda-pack is offered under a New BSD license; see the
-<a href="https://github.com/conda/conda-pack/blob/master/LICENSE.txt">license file</a>.
+<a href="https://github.com/conda/conda-pack/blob/main/LICENSE.txt">license file</a>.
 
 ## Build status
 
-| [![Build status](https://github.com/conda/conda-pack/workflows/Build%20and%20test%20the%20package/badge.svg)](https://github.com/conda/conda-pack/actions) [![codecov](https://codecov.io/gh/conda/conda-pack/branch/master/graph/badge.svg)](https://codecov.io/gh/conda/conda-pack) | [![Anaconda-Server Badge](https://anaconda.org/ctools/conda-pack/badges/latest_release_date.svg)](https://anaconda.org/ctools/conda-pack) |
+| [![Build status](https://github.com/conda/conda-pack/actions/workflows/main.yml/badge.svg)](https://github.com/conda/conda-pack/actions/workflows/main.yml) [![codecov](https://codecov.io/gh/conda/conda-pack/branch/main/graph/badge.svg)](https://codecov.io/gh/conda/conda-pack) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/conda/conda-pack/main.svg)](https://results.pre-commit.ci/latest/github/conda/conda-pack/main) | [![Anaconda-Server Badge](https://anaconda.org/ctools/conda-pack/badges/latest_release_date.svg)](https://anaconda.org/ctools/conda-pack) |
 | --- | :-: |
 | [`conda install ctools/label/dev::conda-pack`](https://anaconda.org/ctools/conda-pack) | [![Anaconda-Server Badge](https://anaconda.org/ctools/conda-pack/badges/version.svg)](https://anaconda.org/ctools/conda-pack) |
 | [`conda install defaults::conda-pack`](https://anaconda.org/anaconda/conda-pack) | [![Anaconda-Server Badge](https://anaconda.org/anaconda/conda-pack/badges/version.svg)](https://anaconda.org/anaconda/conda-pack) |
 | [`conda install conda-forge::conda-pack`](https://anaconda.org/conda-forge/conda-pack) | [![Anaconda-Server Badge](https://anaconda.org/conda-forge/conda-pack/badges/version.svg)](https://anaconda.org/conda-forge/conda-pack) |
```

#### html2text {}

```diff
@@ -1,20 +1,22 @@
 # Conda-Pack `conda-pack` is a command line tool for creating relocatable conda
 environments. This is useful for deploying code in a consistent environment,
 potentially in locations where python or conda isn't already installed. See the
 documentation for more information. Conda-pack is offered under a New BSD
 license; see the license_file. ## Build status | [![Build status](https://
-github.com/conda/conda-pack/workflows/Build%20and%20test%20the%20package/
-badge.svg)](https://github.com/conda/conda-pack/actions) [![codecov](https://
-codecov.io/gh/conda/conda-pack/branch/master/graph/badge.svg)](https://
-codecov.io/gh/conda/conda-pack) | [![Anaconda-Server Badge](https://
-anaconda.org/ctools/conda-pack/badges/latest_release_date.svg)](https://
-anaconda.org/ctools/conda-pack) | | --- | :-: | | [`conda install ctools/label/
-dev::conda-pack`](https://anaconda.org/ctools/conda-pack) | [![Anaconda-Server
-Badge](https://anaconda.org/ctools/conda-pack/badges/version.svg)](https://
-anaconda.org/ctools/conda-pack) | | [`conda install defaults::conda-pack`]
-(https://anaconda.org/anaconda/conda-pack) | [![Anaconda-Server Badge](https://
-anaconda.org/anaconda/conda-pack/badges/version.svg)](https://anaconda.org/
-anaconda/conda-pack) | | [`conda install conda-forge::conda-pack`](https://
-anaconda.org/conda-forge/conda-pack) | [![Anaconda-Server Badge](https://
-anaconda.org/conda-forge/conda-pack/badges/version.svg)](https://anaconda.org/
-conda-forge/conda-pack) |
+github.com/conda/conda-pack/actions/workflows/main.yml/badge.svg)](https://
+github.com/conda/conda-pack/actions/workflows/main.yml) [![codecov](https://
+codecov.io/gh/conda/conda-pack/branch/main/graph/badge.svg)](https://
+codecov.io/gh/conda/conda-pack) [![pre-commit.ci status](https://results.pre-
+commit.ci/badge/github/conda/conda-pack/main.svg)](https://results.pre-
+commit.ci/latest/github/conda/conda-pack/main) | [![Anaconda-Server Badge]
+(https://anaconda.org/ctools/conda-pack/badges/latest_release_date.svg)](https:
+//anaconda.org/ctools/conda-pack) | | --- | :-: | | [`conda install ctools/
+label/dev::conda-pack`](https://anaconda.org/ctools/conda-pack) | [![Anaconda-
+Server Badge](https://anaconda.org/ctools/conda-pack/badges/version.svg)]
+(https://anaconda.org/ctools/conda-pack) | | [`conda install defaults::conda-
+pack`](https://anaconda.org/anaconda/conda-pack) | [![Anaconda-Server Badge]
+(https://anaconda.org/anaconda/conda-pack/badges/version.svg)](https://
+anaconda.org/anaconda/conda-pack) | | [`conda install conda-forge::conda-pack`]
+(https://anaconda.org/conda-forge/conda-pack) | [![Anaconda-Server Badge]
+(https://anaconda.org/conda-forge/conda-pack/badges/version.svg)](https://
+anaconda.org/conda-forge/conda-pack) |
```

### Comparing `conda-pack-0.7.0/conda-recipe/meta.yaml` & `conda-pack-0.7.1/conda-recipe/meta.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -13,18 +13,18 @@
   script:
       - {{ PYTHON }} -m pip install . --no-deps --ignore-installed -vv
   entry_points:
     - conda-pack = conda_pack.cli:main
 
 requirements:
   host:
-    - python
+    - python >=3.7
     - pip
   run:
-    - python
+    - python >=3.7
     - setuptools
 
 test:
   source_files:
     - testing
     - conda_pack/tests
   requires:
```

### Comparing `conda-pack-0.7.0/conda_pack/_progress.py` & `conda-pack-0.7.1/conda_pack/_progress.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import division, absolute_import
-
 import sys
 import threading
 import time
 from timeit import default_timer
 
 
 def format_time(t):
@@ -13,22 +11,22 @@
     '10.4s'
     >>> format_time(1000.4)
     '16min 40.4s'
     """
     m, s = divmod(t, 60)
     h, m = divmod(m, 60)
     if h:
-        return '{0:2.0f}hr {1:2.0f}min {2:4.1f}s'.format(h, m, s)
+        return f"{h:2.0f}hr {m:2.0f}min {s:4.1f}s"
     elif m:
-        return '{0:2.0f}min {1:4.1f}s'.format(m, s)
+        return f"{m:2.0f}min {s:4.1f}s"
     else:
-        return '{0:4.1f}s'.format(s)
+        return f"{s:4.1f}s"
 
 
-class progressbar(object):
+class progressbar:
     """A simple progressbar for iterables.
 
     Displays a progress bar showing progress through an iterable.
 
     Parameters
     ----------
     iterable : iterable
```

### Comparing `conda-pack-0.7.0/conda_pack/cli.py` & `conda-pack-0.7.1/conda_pack/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,31 @@
-from __future__ import print_function, absolute_import
-
 import argparse
 import sys
 import traceback
 
 from . import __version__
-from .core import pack, CondaPackException, context
+from .core import CondaPackException, context, pack
 
 
 class MultiAppendAction(argparse.Action):
     def __init__(self, option_strings, dest, nargs=None, **kwargs):
         if nargs is not None:
             raise ValueError("nargs not allowed")
-        super(MultiAppendAction, self).__init__(option_strings, dest, **kwargs)
+        super().__init__(option_strings, dest, **kwargs)
 
     def __call__(self, parser, namespace, values, option_string=None):
         if getattr(namespace, self.dest) is None:
             setattr(namespace, self.dest, [])
         getattr(namespace, self.dest).append((option_string.strip('-'), values))
 
 
 def build_parser():
     description = "Package an existing conda environment into an archive file."
-    kwargs = dict(prog="conda-pack",
-                  description=description,
-                  add_help=False)
-    if sys.version_info >= (3, 5):
-        kwargs['allow_abbrev'] = False
+    kwargs = dict(prog="conda-pack", description=description, add_help=False)
+    kwargs["allow_abbrev"] = False
     parser = argparse.ArgumentParser(**kwargs)
     parser.add_argument("--name", "-n",
                         metavar="ENV",
                         help="The name of the environment to pack. "
                         "If neither --name nor --prefix are supplied, "
                         "the current activated environment is packed.")
     parser.add_argument("--prefix", "-p",
@@ -76,16 +71,15 @@
                               "inferred by the output file extension."))
     parser.add_argument("--compress-level",
                         metavar="LEVEL",
                         type=int,
                         default=4,
                         help=("The compression level to use, from 0 to 9. "
                               "Higher numbers decrease output file size at "
-                              "the expense of compression time. Ignored for "
-                              "``format='zip'``. Default is 4."))
+                              "the expense of compression time. Default is 4."))
     parser.add_argument("--n-threads", "-j",
                         metavar="N",
                         type=int,
                         default=1,
                         help=("The number of threads to use. Set to -1 to use "
                               "the number of cpus on this machine. If a file "
                               "format doesn't support threaded packaging, this "
```

### Comparing `conda-pack-0.7.0/conda_pack/compat.py` & `conda-pack-0.7.1/conda_pack/compat.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 is_32bit = sys.maxsize < 2**32 or os.environ.get('CONDA_FORCE_32BIT', '0') == '1'
 
 PY2 = sys.version_info.major == 2
 
 
 if PY2:
     from imp import load_source
+
     from Queue import Queue
 
     def source_from_cache(path):
         if path.endswith('.pyc') or path.endswith('.pyo'):
             return path[:-1]
         raise ValueError("Path %s is not a python bytecode file" % path)
 else:
```

### Comparing `conda-pack-0.7.0/conda_pack/core.py` & `conda-pack-0.7.1/conda_pack/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-from __future__ import absolute_import, print_function
-
 import glob
 import json
 import os
-import pkg_resources
 import re
 import shlex
 import shutil
 import subprocess
 import sys
 import tempfile
 import warnings
 from contextlib import contextmanager
 from datetime import datetime
 from fnmatch import fnmatch
 
-from .compat import on_win, default_encoding, find_py_source, is_32bit
-from .prefixes import SHEBANG_REGEX, replace_prefix
-from ._progress import progressbar
+import pkg_resources
 
+from ._progress import progressbar
+from .compat import default_encoding, find_py_source, is_32bit, on_win
+from .prefixes import SHEBANG_REGEX, replace_prefix
 
 __all__ = ('CondaPackException', 'CondaEnv', 'File', 'pack')
 
 
 class CondaPackException(Exception):
     """Internal exception to report to user"""
     pass
@@ -43,15 +41,15 @@
 else:
     _scripts = [(os.path.join(_current_dir, 'scripts', 'posix', 'activate'),
                  os.path.join(BIN_DIR, 'activate')),
                 (os.path.join(_current_dir, 'scripts', 'posix', 'deactivate'),
                  os.path.join(BIN_DIR, 'deactivate'))]
 
 
-class _Context(object):
+class _Context:
     def __init__(self):
         self.is_cli = False
 
     def warn(self, msg):
         if self.is_cli:
             print(msg + "\n", file=sys.stderr)
         else:
@@ -66,15 +64,15 @@
         finally:
             self.is_cli = old
 
 
 context = _Context()
 
 
-class CondaEnv(object):
+class CondaEnv:
     """A Conda environment for packaging.
 
     Use :func:`CondaEnv.from_prefix`, :func:`CondaEnv.from_name`, or
     :func:`CondaEnv.from_default` instead of the default constructor.
 
     Attributes
     ----------
@@ -105,15 +103,15 @@
     "/full/path/to/output.tar.gz"
 
     Create a CondaEnv object from the current environment, excluding all
     ``*.pyx`` files, except those from ``cytoolz``.
 
     >>> env = (CondaEnv.from_default()
     ...                .exclude("*.pyx")
-    ...                .include("lib/python3.6/site-packages/cytoolz/*.pyx"))
+    ...                .include("lib/python3.7/site-packages/cytoolz/*.pyx"))
     CondaEnv<'~/miniconda/envs/example', 1234 files>
     """
     def __init__(self, prefix, files, excluded_files=None):
         self.prefix = prefix
         self.files = files
         self._excluded_files = excluded_files or []
 
@@ -361,15 +359,15 @@
             # Ensure the prefix is a relative path
             arcroot = arcroot.strip(os.path.sep) if arcroot else ''
 
         if os.path.exists(output) and not force:
             raise CondaPackException("File %r already exists" % output)
 
         if verbose:
-            print("Packing environment at %r to %r" % (self.prefix, output))
+            print(f"Packing environment at {self.prefix!r} to {output!r}")
 
         fd, temp_path = tempfile.mkstemp()
 
         try:
             with os.fdopen(fd, 'wb') as temp_file:
                 with archive(temp_file, temp_path, arcroot, format,
                              compress_level=compress_level,
@@ -392,15 +390,15 @@
         else:
             # Writing succeeded, move archive to desired location
             shutil.move(temp_path, output)
 
         return output
 
 
-class File(object):
+class File:
     """A single archive record.
 
     Parameters
     ----------
     source : str
         Absolute path to the source.
     target : str
@@ -420,15 +418,15 @@
         self.source = source
         self.target = target
         self.is_conda = is_conda
         self.file_mode = file_mode
         self.prefix_placeholder = prefix_placeholder
 
     def __repr__(self):
-        return 'File<%r, is_conda=%r>' % (self.target, self.is_conda)
+        return f"File<{self.target!r}, is_conda={self.is_conda!r}>"
 
 
 def pack(name=None, prefix=None, output=None, format='infer',
          arcroot='', dest_prefix=None,
          parcel_root=None, parcel_name=None,
          parcel_version=None, parcel_distro=None,
          verbose=False, force=False,
@@ -598,18 +596,18 @@
                "`pip install -e`). Editable packages found:\n\n"
                "%s") % '\n'.join('- %s' % p for p in sorted(editable_packages))
         raise CondaPackException(msg)
 
 
 def name_to_prefix(name=None):
     try:
-        conda_exe = os.environ.get('CONDA_EXE', 'conda')
-        info = (subprocess.check_output("{} info --json".format(conda_exe),
-                                        shell=True, stderr=subprocess.PIPE)
-                          .decode(default_encoding))
+        conda_exe = os.environ.get("CONDA_EXE", "conda")
+        info = subprocess.check_output(
+            f"{conda_exe} info --json", shell=True, stderr=subprocess.PIPE
+        ).decode(default_encoding)
     except subprocess.CalledProcessError as exc:
         kind = ('current environment' if name is None
                 else 'environment: %r' % name)
         raise CondaPackException("Failed to determine path to %s. This may "
                                  "be due to conda not being on your PATH. The "
                                  "full error is below:\n\n"
                                  "%s" % (kind, exc.output))
@@ -651,15 +649,15 @@
                 out[rec[2]] = rec[:2]
             else:
                 raise ValueError("Failed to parse has_prefix file")
     return out
 
 
 def load_files(prefix):
-    from os.path import relpath, join, isfile, islink
+    from os.path import isfile, islink, join, relpath
 
     ignore = {'pkgs', 'envs', 'conda-bld', '.conda_lock', 'users',
               'conda-recipes', '.index', '.unionfs', '.nonadmin', 'python.app',
               'Launcher.app'}
 
     res = set()
 
@@ -760,15 +758,15 @@
 Conda-managed packages were found without entries in the package cache. This
 is usually due to `conda clean -p` being unaware of symlinked or copied
 packages. Uncached packages:
 
 {0}"""
 
 _uncached_warning = """\
-{0}
+{}
 
 Continuing with packing, treating these packages as if they were unmanaged
 files (e.g. from `pip`). This is usually fine, but may cause issues as
 prefixes aren't being handled as robustly.""".format(_uncached_error)
 
 
 _missing_files_error = """
@@ -907,29 +905,30 @@
             # More than one occurrence of prefix, can't fully cleanup.
             return data, False
 
         shebang, executable, options = shebang_match.groups()
 
         if executable.startswith(prefix_b):
             # shebang points inside environment, rewrite
-            executable_name = executable.decode('utf-8').split('/')[-1]
-            new_shebang = '#!/usr/bin/env %s%s' % (executable_name,
-                                                   options.decode('utf-8'))
-            data = data.replace(shebang, new_shebang.encode('utf-8'))
+            executable_name = executable.decode("utf-8").split("/")[-1]
+            new_shebang = "#!/usr/bin/env {}{}".format(
+                executable_name, options.decode("utf-8")
+            )
+            data = data.replace(shebang, new_shebang.encode("utf-8"))
 
             return data, True
 
     return data, False
 
 
 def rewrite_conda_meta(source):
     """Remove absolute paths in conda-meta that reference local install.
 
     These are unnecessary for install/uninstall on the destination machine."""
-    with open(source, 'r') as f:
+    with open(source) as f:
         original = f.read()
 
     data = json.loads(original)
     for field in ["extracted_package_dir", "package_tarball_full_path"]:
         if field in data:
             data[field] = ""
 
@@ -986,43 +985,45 @@
 ]
 
 if __name__ == '__main__':
     import os
     import argparse
     parser = argparse.ArgumentParser(
             prog='conda-unpack',
-            description=('Finish unpacking the environment after unarchiving.'
+            description=('Finish unpacking the environment after unarchiving. '
                          'Cleans up absolute prefixes in any remaining files'))
     parser.add_argument('--version',
                         action='store_true',
                         help='Show version then exit')
     args = parser.parse_args()
     # Manually handle version printing to output to stdout in python < 3.4
     if args.version:
         print('conda-unpack {version}')
     else:
         script_dir = os.path.dirname(__file__)
         new_prefix = os.path.abspath(os.path.dirname(script_dir))
         for path, placeholder, mode in _prefix_records:
-            update_prefix(os.path.join(new_prefix, path), new_prefix,
-                          placeholder, mode=mode)
+            new_path = os.path.join(new_prefix, path)
+            if on_win:
+                new_path = new_path.replace('\\\\', '/')
+            update_prefix(new_path, new_prefix, placeholder, mode=mode)
 """
 
 
 # Deduce file type for unmanaged packages. If decoding utf-8 is
 # successful, we assume text, otherwise binary.
 def is_binary_file(data):
     try:
         data.decode('utf-8')
         return False
     except UnicodeDecodeError:
         return True
 
 
-class Packer(object):
+class Packer:
     def __init__(self, prefix, archive, dest_prefix=None, parcel=None):
         self.prefix = prefix
         self.archive = archive
         self.dest = dest_prefix
         self.has_dest = dest_prefix is not None
         self.parcel = parcel
         self.prefixes = []
@@ -1061,17 +1062,20 @@
 
         elif os.path.isdir(file.source) or os.path.islink(file.source):
             self.archive.add(file.source, file.target)
             return
 
         file_mode = file.file_mode
         placeholder = file.prefix_placeholder
-        if ((self.has_dest or
-             file_mode == 'unknown' or
-             file_mode == 'text' and file.target.startswith(BIN_DIR))):
+        if (
+            self.has_dest
+            or file_mode == "unknown"
+            or file_mode == "text"
+            and file.target.startswith(BIN_DIR)
+        ):
             # In each of these cases, we need to inspect the file contents here.
             with open(file.source, 'rb') as fil:
                 data = fil.read()
         else:
             # No need to read the file; just pass the filename to the archiver.
             self.archive.add(file.source, file.target)
             self.prefixes.append((file.target, placeholder, file_mode))
```

### Comparing `conda-pack-0.7.0/conda_pack/formats.py` & `conda-pack-0.7.1/conda_pack/formats.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,19 @@
-from __future__ import print_function, division, absolute_import
-
 import errno
 import os
+import shutil
 import stat
 import struct
 import subprocess
-import sys
-import shutil
 import tarfile
 import tempfile
 import threading
 import time
 import zipfile
 import zlib
-
 from contextlib import closing
 from functools import partial
 from io import BytesIO
 from multiprocessing.pool import ThreadPool
 
 from .compat import Queue, on_win
 from .core import CondaPackException
@@ -34,16 +30,16 @@
 
 def archive(fileobj, path, arcroot, format, compress_level=4, zip_symlinks=False,
             zip_64=True, n_threads=1, verbose=False):
 
     n_threads = _parse_n_threads(n_threads)
 
     if format == 'zip':
-        return ZipArchive(fileobj, arcroot, zip_symlinks=zip_symlinks,
-                          zip_64=zip_64)
+        return ZipArchive(fileobj, arcroot, compresslevel=compress_level,
+                          zip_symlinks=zip_symlinks, zip_64=zip_64)
 
     # Tar archives
     if format in ('tar.gz', 'tgz', 'parcel'):
         if n_threads == 1:
             mode = 'w:gz'
             close_file = False
         else:
@@ -75,15 +71,15 @@
     else:  # format == 'tar'
         mode = 'w'
         close_file = False
     return TarArchive(fileobj, arcroot, close_file=close_file,
                       mode=mode, compresslevel=compress_level)
 
 
-class ParallelFileWriter(object):
+class ParallelFileWriter:
     def __init__(self, fileobj, compresslevel=9, n_threads=1):
         self.fileobj = fileobj
         self.compresslevel = compresslevel
         self.n_threads = n_threads
 
         # Initialize file state
         self.size = 0
@@ -237,15 +233,15 @@
     def _write_footer(self):
         pass
 
     def _flush_compressor(self, compressor):
         return compressor.flush()
 
 
-class ArchiveBase(object):
+class ArchiveBase:
     def add(self, source, target):
         target = os.path.join(self.arcroot, target)
         self._add(source, target)
 
     def add_bytes(self, source, sourcebytes, target):
         target = os.path.join(self.arcroot, target)
         self._add_bytes(source, sourcebytes, target)
@@ -294,23 +290,25 @@
 a dependency. Unfortunately, conda-pack does not support this practice
 for zip files unless the --zip-symlinks option is engaged. Please see
 "conda-pack --help" for more information about this option, or use a
 tar-based archive format instead."""
 
 
 class ZipArchive(ArchiveBase):
-    def __init__(self, fileobj, arcroot, zip_symlinks=False, zip_64=True):
+    def __init__(self, fileobj, arcroot, compresslevel=4, zip_symlinks=False, zip_64=True):
         self.fileobj = fileobj
         self.arcroot = arcroot
+        self.compresslevel = compresslevel
         self.zip_symlinks = zip_symlinks
         self.zip_64 = zip_64
 
     def __enter__(self):
         self.archive = zipfile.ZipFile(self.fileobj, "w",
                                        allowZip64=self.zip_64,
+                                       compresslevel=self.compresslevel,
                                        compression=zipfile.ZIP_DEFLATED)
         return self
 
     def __exit__(self, type, value, traceback):
         self.archive.close()
         if isinstance(value, zipfile.LargeZipFile):
             raise CondaPackException(
@@ -347,53 +345,28 @@
                         self.archive.write(source, target)
                     except OSError as e:
                         if e.errno == errno.ENOENT:
                             if source[-len(target):] == target:
                                 # For managed packages, this will give us the package name
                                 # followed by the relative path within the environment, a
                                 # more readable result.
-                                source = os.path.basename(source[:-len(target)-1])
-                                source = '{}: {}'.format(source, target)
+                                source = os.path.basename(source[: -len(target) - 1])
+                                source = f"{source}: {target}"
                             msg = _dangling_link_error.format(source)
                             raise CondaPackException(msg)
                         raise
         else:
             self.archive.write(source, target)
 
     def _add_bytes(self, source, sourcebytes, target):
         info = zipinfo_from_file(source, target)
         self.archive.writestr(info, sourcebytes)
 
 
-if sys.version_info >= (3, 6):
-    zipinfo_from_file = zipfile.ZipInfo.from_file
-else:  # pragma: no cover
-    # Backported from python 3.6
-    def zipinfo_from_file(filename, arcname=None):
-        st = os.stat(filename)
-        isdir = stat.S_ISDIR(st.st_mode)
-        mtime = time.localtime(st.st_mtime)
-        date_time = mtime[0:6]
-        # Create ZipInfo instance to store file information
-        if arcname is None:
-            arcname = filename
-        arcname = os.path.normpath(os.path.splitdrive(arcname)[1])
-        while arcname[0] in (os.sep, os.altsep):
-            arcname = arcname[1:]
-        if isdir:
-            arcname += '/'
-        zinfo = zipfile.ZipInfo(arcname, date_time)
-        zinfo.external_attr = (st.st_mode & 0xFFFF) << 16  # Unix attributes
-        if isdir:
-            zinfo.file_size = 0
-            zinfo.external_attr |= 0x10  # MS-DOS directory flag
-        else:
-            zinfo.file_size = st.st_size
-
-        return zinfo
+zipinfo_from_file = zipfile.ZipInfo.from_file
 
 
 class SquashFSArchive(ArchiveBase):
     def __init__(self, fileobj, target_path, arcroot, n_threads, verbose=False,
                  compress_level=4):
         if shutil.which("mksquashfs") is None:
             raise SystemError("Command 'mksquashfs' not found. Please install it, "
@@ -433,15 +406,15 @@
             comp_algo_str = "None"
             cmd += ["-noI", "-noD", "-noF", "-noX"]
         elif self.compress_level == 9:
             comp_algo_str = "xz"
             cmd += ["-comp", comp_algo_str]
         else:
             comp_level = int(self.compress_level / 8 * 20)
-            comp_algo_str = "zstd (level {})".format(comp_level)
+            comp_algo_str = f"zstd (level {comp_level})"
             # 256KB block size instead of the default 128KB for slightly smaller archive sizes
             cmd += ["-comp", "zstd", "-Xcompression-level", str(comp_level), "-b", str(256*1024)]
 
         if self.verbose:
             s = "Running mksquashfs with {} compression (processors: {}).".format(
                 comp_algo_str, self.n_threads)
             if self.compress_level != 9:
```

### Comparing `conda-pack-0.7.0/conda_pack/prefixes.py` & `conda-pack-0.7.1/conda_pack/prefixes.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,16 +31,18 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
+import platform
 import re
 import struct
+import subprocess
 import sys
 
 on_win = sys.platform == 'win32'
 
 # three capture groups: whole_shebang, executable, options
 SHEBANG_REGEX = (
         # pretty much the whole match string
@@ -58,24 +60,31 @@
 
 def update_prefix(path, new_prefix, placeholder, mode='text'):
     if on_win and mode == 'text':
         # force all prefix replacements to forward slashes to simplify need to
         # escape backslashes replace with unix-style path separators
         new_prefix = new_prefix.replace('\\', '/')
 
+    file_changed = False
     with open(path, 'rb+') as fh:
         original_data = fh.read()
         fh.seek(0)
 
         data = replace_prefix(original_data, mode, placeholder, new_prefix)
 
         # If the before and after content is the same, skip writing
         if data != original_data:
             fh.write(data)
             fh.truncate()
+            file_changed = True
+
+    if file_changed and platform.system() == "Darwin" and platform.machine() == "arm64":
+        subprocess.run(
+            ["/usr/bin/codesign", "-s", "-", "-f", path], capture_output=True
+        )
 
 
 def replace_prefix(data, mode, placeholder, new_prefix):
     if mode == 'text':
         data2 = text_replace(data, placeholder, new_prefix)
     elif mode == 'binary':
         data2 = binary_replace(data,
```

### Comparing `conda-pack-0.7.0/conda_pack/scripts/posix/activate` & `conda-pack-0.7.1/conda_pack/scripts/posix/activate`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     local script_dir
     case "$_CONDA_SHELL_FLAVOR" in
         bash) script_dir="$(dirname "${BASH_SOURCE[0]}")";;
         zsh) script_dir="$(dirname "${(%):-%x}")";;  # http://stackoverflow.com/a/28336473/2127762
         dash) x=$(lsof -p $$ -Fn0 | tail -1); script_dir="$(dirname "${x#*n}")";;
         *) script_dir="$(cd "$(dirname "$_")" && echo "$PWD")";;
     esac
-    
+
     local full_path_script_dir="$(cd "${script_dir}" > /dev/null && pwd)"
     local full_path_env="$(dirname "$full_path_script_dir")"
     local env_name="$(basename "$full_path_env")"
 
     # If there's already a source env
     if [ -n "$CONDA_PREFIX" ]; then
         # If the source env differs from this env
```

### Comparing `conda-pack-0.7.0/conda_pack/scripts/posix/deactivate` & `conda-pack-0.7.1/conda_pack/scripts/posix/deactivate`

 * *Files identical despite different names*

### Comparing `conda-pack-0.7.0/conda_pack/scripts/windows/activate.bat` & `conda-pack-0.7.1/conda_pack/scripts/windows/activate.bat`

 * *Files identical despite different names*

### Comparing `conda-pack-0.7.0/conda_pack/scripts/windows/deactivate.bat` & `conda-pack-0.7.1/conda_pack/scripts/windows/deactivate.bat`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 @SET "TARGETS=;%CONDA_PREFIX%;%CONDA_PREFIX%\Library\mingw-w64\bin;%CONDA_PREFIX%\Library\usr\bin;%CONDA_PREFIX%\Library\bin;%CONDA_PREFIX%\Scripts"
 @SET "NEW_PATH="
 @FOR %%i IN ("%PATH:;=";"%") DO @(CALL :filterPath "%%~i")
 
 @REM Restore the command prompt
 @SET "PROMPT=%_CONDA_PACK_OLD_PS1%"
 @SET "CONDA_PS1_BACKUP="
-  
+
 @REM This persists env variables, which are otherwise local to this script right now.
 @endlocal & (
     @REM Used for deactivate, to make sure we restore original state after deactivation
     @SET "_CONDA_PACK_OLD_PS1=%CONDA_PS1_BACKUP%"
     @SET "PROMPT=%PROMPT%"
     @SET "PATH=%NEW_PATH:~1%"
     @SET "CONDA_PREFIX="
```

### Comparing `conda-pack-0.7.0/conda_pack/tests/conftest.py` & `conda-pack-0.7.1/conda_pack/tests/conftest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-from __future__ import print_function, division, absolute_import
-
 import os
 
 test_dir = os.path.dirname(os.path.abspath(__file__))
 croot = os.environ.get('CONDA_ROOT')
 if croot is None:
     croot = os.path.join(test_dir, '..', '..', 'testing', 'conda')
 env_dir = os.path.join(os.path.abspath(croot), 'envs')
 
-py27_path = os.path.join(env_dir, 'py27')
-py36_path = os.path.join(env_dir, 'py36')
-py36_editable_path = os.path.join(env_dir, 'py36_editable')
-py36_broken_path = os.path.join(env_dir, 'py36_broken')
-py36_missing_files_path = os.path.join(env_dir, 'py36_missing_files')
+py37_path = os.path.join(env_dir, 'py37')
+py37_editable_path = os.path.join(env_dir, 'py37_editable')
+py37_broken_path = os.path.join(env_dir, 'py37_broken')
+py37_missing_files_path = os.path.join(env_dir, 'py37_missing_files')
+py310_path = os.path.join(env_dir, 'py310')
 nopython_path = os.path.join(env_dir, 'nopython')
 has_conda_path = os.path.join(env_dir, 'has_conda')
 activate_scripts_path = os.path.join(env_dir, 'activate_scripts')
```

### Comparing `conda-pack-0.7.0/conda_pack/tests/test_cli.py` & `conda-pack-0.7.1/conda_pack/tests/test_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,20 @@
-from __future__ import absolute_import, print_function, division
-
 import os
-import sys
 import signal
 import tarfile
 import time
 from threading import Thread
 
 import pytest
 
 import conda_pack
 from conda_pack.cli import main
 from conda_pack.compat import on_win
 
-from .conftest import py36_path, py27_path
-
-on_p2 = sys.version[0] == '2'
+from .conftest import py37_path, py310_path
 
 
 def test_help(capsys):
     with pytest.raises(SystemExit) as exc:
         main(["-h"])
 
     assert exc.value.code == 0
@@ -58,38 +53,38 @@
     assert out['filters'] == [("exclude", "foo/*"),
                               ("include", "*.py"),
                               ("include", "*.pyx"),
                               ("exclude", "foo/bar/*.pyx")]
 
 
 def test_cli_roundtrip(capsys, tmpdir):
-    out_path = os.path.join(str(tmpdir), 'py36.tar')
+    out_path = os.path.join(str(tmpdir), 'py37.tar')
 
     with pytest.raises(SystemExit) as exc:
-        main(["-p", py36_path, "-o", out_path])
+        main(["-p", py37_path, "-o", out_path])
 
     assert exc.value.code == 0
 
     assert os.path.exists(out_path)
     assert tarfile.is_tarfile(out_path)
 
     out, err = capsys.readouterr()
     assert not err
 
-    bar, percent, time = [i.strip() for i in out.split('\r')[-1].split('|')]
-    assert bar == '[' + '#' * 40 + ']'
-    assert percent == '100% Completed'
+    bar, percent, time = (i.strip() for i in out.split("\r")[-1].split("|"))
+    assert bar == "[" + "#" * 40 + "]"
+    assert percent == "100% Completed"
     assert time
 
 
 def test_quiet(capsys, tmpdir):
-    out_path = os.path.join(str(tmpdir), 'py36.tar')
+    out_path = os.path.join(str(tmpdir), 'py37.tar')
 
     with pytest.raises(SystemExit) as exc:
-        main(["-p", py36_path, "-o", out_path, "-q"])
+        main(["-p", py37_path, "-o", out_path, "-q"])
 
     assert exc.value.code == 0
 
     assert os.path.exists(out_path)
     assert tarfile.is_tarfile(out_path)
 
     out, err = capsys.readouterr()
@@ -112,46 +107,43 @@
     assert exc.value.code != 0
 
     out, err = capsys.readouterr()
     assert not out
     assert "usage: conda-pack" in err
 
 
-@pytest.mark.xfail(on_p2, reason='Relaxing python 2 tests on CI')
 def test_cli_warnings(capsys, tmpdir):
-    out_path = os.path.join(str(tmpdir), 'py27.tar')
+    out_path = os.path.join(str(tmpdir), 'py310.tar')
 
     with pytest.raises(SystemExit) as exc:
-        main(["-p", py27_path, "-o", out_path])
+        main(["-p", py310_path, "-o", out_path])
 
-    # Test fails in some CI systems for Python 2
     assert exc.value.code == 0
 
     assert os.path.exists(out_path)
     assert tarfile.is_tarfile(out_path)
 
     out, err = capsys.readouterr()
     assert "Conda-managed packages were found" in err
     assert "UserWarning" not in err  # printed, not from python warning
 
 
 @pytest.mark.skipif(on_win, reason='SIGINT terminates the tests on Windows')
-@pytest.mark.xfail(on_p2, reason='Relaxing python 2 tests on CI')
 def test_keyboard_interrupt(capsys, tmpdir):
     def interrupt():
         time.sleep(0.2)
         os.kill(os.getpid(), signal.SIGINT)
 
     interrupter = Thread(target=interrupt)
 
-    out_path = os.path.join(str(tmpdir), 'py36.tar')
+    out_path = os.path.join(str(tmpdir), 'py37.tar')
     try:
         with pytest.raises(SystemExit) as exc:
             interrupter.start()
-            main(["-p", py36_path, "-o", out_path])
+            main(["-p", py37_path, "-o", out_path])
     except KeyboardInterrupt:
         assert False, "Should have been caught by the CLI"
 
     assert exc.value.code == 1
     out, err = capsys.readouterr()
     assert err == 'Interrupted\n'
     assert not os.path.exists(out_path)
```

### Comparing `conda-pack-0.7.0/conda_pack/tests/test_core.py` & `conda-pack-0.7.1/conda_pack/tests/test_core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,48 @@
-from __future__ import absolute_import, print_function, division
-
 import json
-import sys
 import os
 import re
 import subprocess
 import tarfile
 from glob import glob
 
 import pytest
 
 from conda_pack import CondaEnv, CondaPackException, pack
-from conda_pack.compat import on_win, load_source
-from conda_pack.core import name_to_prefix, File, BIN_DIR
+from conda_pack.compat import load_source, on_win
+from conda_pack.core import BIN_DIR, File, name_to_prefix
 
-from .conftest import (py36_path, py36_editable_path, py36_broken_path,
-                       py27_path, nopython_path, has_conda_path,
-                       activate_scripts_path, env_dir, py36_missing_files_path)
+from .conftest import (
+    activate_scripts_path,
+    env_dir,
+    has_conda_path,
+    nopython_path,
+    py37_broken_path,
+    py37_editable_path,
+    py37_missing_files_path,
+    py37_path,
+    py310_path,
+)
 
 BIN_DIR_L = BIN_DIR.lower()
-SP_36 = 'Lib\\site-packages' if on_win else 'lib/python3.6/site-packages'
-SP_36_L = SP_36.lower().replace('\\', '/')
+SP_37 = 'Lib\\site-packages' if on_win else 'lib/python3.7/site-packages'
+SP_37_L = SP_37.lower().replace('\\', '/')
 
 
 if on_win:
     def normpath(f):
         return os.path.normcase(f).replace('\\', '/')
 else:
     def normpath(f):
         return f
 
 
 @pytest.fixture(scope="module")
-def py36_env():
-    return CondaEnv.from_prefix(py36_path)
+def py37_env():
+    return CondaEnv.from_prefix(py37_path)
 
 
 @pytest.fixture
 def bad_conda_exe(tmpdir_factory, monkeypatch):
     tmpdir = str(tmpdir_factory.mktemp('bin'))
     fake_conda = os.path.join(tmpdir, 'conda.bat' if on_win else 'conda')
     with open(fake_conda, 'w') as f:
@@ -53,213 +58,212 @@
     name_to_prefix()
 
     with pytest.raises(CondaPackException):
         name_to_prefix("this_is_probably_not_a_real_env_name")
 
 
 def test_from_prefix():
-    rel_env_dir = os.path.relpath(py36_path, os.getcwd())
+    rel_env_dir = os.path.relpath(py37_path, os.getcwd())
     env = CondaEnv.from_prefix(rel_env_dir)
     assert len(env)
     # relative path is normalized
-    assert os.path.normcase(env.prefix) == os.path.normcase(py36_path)
+    assert os.path.normcase(env.prefix) == os.path.normcase(py37_path)
 
     # Path is missing
     with pytest.raises(CondaPackException):
         CondaEnv.from_prefix(os.path.join(env_dir, "this_path_doesnt_exist"))
 
     # Path exists, but isn't a conda environment
     with pytest.raises(CondaPackException):
         CondaEnv.from_prefix(os.path.join(env_dir))
 
 
-@pytest.mark.xfail(sys.version[0] == '2', reason="Python 2 failure")
 def test_missing_package_cache():
     with pytest.warns(UserWarning) as record:
-        env = CondaEnv.from_prefix(py27_path)
+        env = CondaEnv.from_prefix(py310_path)
 
     assert len(env)
 
     assert len(record) == 1
     msg = str(record[0].message)
     assert 'conda_pack_test_lib2' in msg
 
     with pytest.raises(CondaPackException):
-        CondaEnv.from_prefix(py27_path, on_missing_cache='raise')
+        CondaEnv.from_prefix(py310_path, on_missing_cache='raise')
 
 
 def test_errors_editable_packages():
     with pytest.raises(CondaPackException) as exc:
-        CondaEnv.from_prefix(py36_editable_path)
+        CondaEnv.from_prefix(py37_editable_path)
 
     assert "Editable packages found" in str(exc.value)
 
 
 def test_ignore_errors_editable_packages():
-    CondaEnv.from_prefix(py36_editable_path, ignore_editable_packages=True)
+    CondaEnv.from_prefix(py37_editable_path, ignore_editable_packages=True)
 
 
 def test_errors_pip_overwrites():
     with pytest.raises(CondaPackException) as exc:
-        CondaEnv.from_prefix(py36_broken_path)
+        CondaEnv.from_prefix(py37_broken_path)
 
     msg = str(exc.value)
     assert "pip" in msg
     assert "toolz" in msg
 
 
 def test_missing_files():
     with pytest.raises(CondaPackException) as exc:
-        CondaEnv.from_prefix(py36_missing_files_path)
+        CondaEnv.from_prefix(py37_missing_files_path)
 
     msg = str(exc.value)
-    assert "{}toolz{}__init__.py".format(os.sep, os.sep) in msg, msg
-    assert "{}toolz{}_signatures.py".format(os.sep, os.sep) in msg, msg
+    assert f"{os.sep}toolz{os.sep}__init__.py" in msg, msg
+    assert f"{os.sep}toolz{os.sep}_signatures.py" in msg, msg
 
 
 def test_missing_files_ignored():
-    CondaEnv.from_prefix(py36_missing_files_path, ignore_missing_files=True)
+    CondaEnv.from_prefix(py37_missing_files_path, ignore_missing_files=True)
 
 
 def test_errors_conda_missing(bad_conda_exe):
     with pytest.raises(CondaPackException) as exc:
         CondaEnv.from_name('probably_fake_env')
 
     assert 'Failed to determine path to environment' in str(exc.value)
 
 
-def test_env_properties(py36_env):
-    assert py36_env.name == 'py36'
-    assert py36_env.prefix == py36_path
+def test_env_properties(py37_env):
+    assert py37_env.name == 'py37'
+    assert py37_env.prefix == py37_path
 
     # Env has a length
-    assert len(py36_env) == len(py36_env.files)
+    assert len(py37_env) == len(py37_env.files)
 
     # Env is iterable
-    assert len(list(py36_env)) == len(py36_env)
+    assert len(list(py37_env)) == len(py37_env)
 
     # Smoketest repr
-    assert 'CondaEnv<' in repr(py36_env)
+    assert 'CondaEnv<' in repr(py37_env)
 
 
-def test_load_environment_ignores(py36_env):
-    lk = {normpath(f.target): f for f in py36_env}
-    for fname in ('conda', 'conda.bat'):
-        assert '{}/{}'.format(BIN_DIR_L, fname) not in lk
-    for fname in ('activate', 'activate.bat', 'deactivate', 'deactivate.bat'):
-        fpath = '{}/{}'.format(BIN_DIR_L, fname)
-        assert fpath not in lk or not lk[fpath].source.startswith(py36_path)
+def test_load_environment_ignores(py37_env):
+    lk = {normpath(f.target): f for f in py37_env}
+    for fname in ("conda", "conda.bat"):
+        assert f"{BIN_DIR_L}/{fname}" not in lk
+    for fname in ("activate", "activate.bat", "deactivate", "deactivate.bat"):
+        fpath = f"{BIN_DIR_L}/{fname}"
+        assert fpath not in lk or not lk[fpath].source.startswith(py37_path)
 
 
 def test_file():
     f = File('/root/path/to/foo/bar', 'foo/bar')
     # smoketest repr
     repr(f)
 
 
-def test_loaded_file_properties(py36_env):
-    lk = {normpath(f.target): f for f in py36_env}
+def test_loaded_file_properties(py37_env):
+    lk = {normpath(f.target): f for f in py37_env}
 
     # Pip installed entrypoint
-    exe_suffix = '.exe' if on_win else ''
-    fil = lk['{}/pytest{}'.format(BIN_DIR_L, exe_suffix)]
+    exe_suffix = ".exe" if on_win else ""
+    fil = lk[f"{BIN_DIR_L}/pytest{exe_suffix}"]
     assert not fil.is_conda
     assert fil.file_mode == 'unknown'
     assert fil.prefix_placeholder is None
 
     # Conda installed noarch entrypoint
-    fil = lk['{}/conda-pack-test-lib1'.format(BIN_DIR_L)]
+    fil = lk[f"{BIN_DIR_L}/conda-pack-test-lib1"]
     assert fil.is_conda
     assert fil.file_mode == 'text'
-    assert fil.prefix_placeholder != py36_env.prefix
+    assert fil.prefix_placeholder != py37_env.prefix
 
     # Conda installed entrypoint
-    suffix = '-script.py' if on_win else ''
-    fil = lk['{}/conda-pack-test-lib2{}'.format(BIN_DIR_L, suffix)]
+    suffix = "-script.py" if on_win else ""
+    fil = lk[f"{BIN_DIR_L}/conda-pack-test-lib2{suffix}"]
     assert fil.is_conda
     assert fil.file_mode == 'text'
-    assert fil.prefix_placeholder != py36_env.prefix
+    assert fil.prefix_placeholder != py37_env.prefix
 
     # Conda installed file
-    fil = lk['{}/conda_pack_test_lib1/cli.py'.format(SP_36_L)]
+    fil = lk[f"{SP_37_L}/conda_pack_test_lib1/cli.py"]
     assert fil.is_conda
     assert fil.file_mode is None
     assert fil.prefix_placeholder is None
 
 
 def test_works_with_no_python():
     # Collection doesn't require python
     env = CondaEnv.from_prefix(nopython_path)
     # non-empty
     assert len(env)
 
 
-def test_include_exclude(py36_env):
-    old_len = len(py36_env)
-    env2 = py36_env.exclude("*.pyc")
+def test_include_exclude(py37_env):
+    old_len = len(py37_env)
+    env2 = py37_env.exclude("*.pyc")
     # No mutation
-    assert len(py36_env) == old_len
-    assert env2 is not py36_env
-    assert len(env2) < len(py36_env)
+    assert len(py37_env) == old_len
+    assert env2 is not py37_env
+    assert len(env2) < len(py37_env)
 
     # Re-add the removed files, envs are equivalent
-    assert len(env2.include("*.pyc")) == len(py36_env)
+    assert len(env2.include("*.pyc")) == len(py37_env)
 
-    env3 = env2.exclude(os.path.join(SP_36, "conda_pack_test_lib1", "*"))
-    env4 = env3.include(os.path.join(SP_36, "conda_pack_test_lib1", "cli.py"))
+    env3 = env2.exclude(os.path.join(SP_37, "conda_pack_test_lib1", "*"))
+    env4 = env3.include(os.path.join(SP_37, "conda_pack_test_lib1", "cli.py"))
     assert len(env3) + 1 == len(env4)
 
 
-def test_output_and_format(py36_env):
-    output, format = py36_env._output_and_format()
-    assert output == 'py36.tar.gz'
+def test_output_and_format(py37_env):
+    output, format = py37_env._output_and_format()
+    assert output == 'py37.tar.gz'
     assert format == 'tar.gz'
 
     for format in ['tar.gz', 'tar.bz2', 'tar.xz', 'tar', 'zip', 'parcel']:
-        output = os.extsep.join([py36_env.name, format])
+        output = os.extsep.join([py37_env.name, format])
 
-        o, f = py36_env._output_and_format(format=format)
+        o, f = py37_env._output_and_format(format=format)
         assert f == format
         assert o == (None if f == 'parcel' else output)
 
-        o, f = py36_env._output_and_format(output=output)
+        o, f = py37_env._output_and_format(output=output)
         assert o == output
         assert f == format
 
-        o, f = py36_env._output_and_format(output='foo.zip', format=format)
+        o, f = py37_env._output_and_format(output='foo.zip', format=format)
         assert f == format
         assert o == 'foo.zip'
 
     with pytest.raises(CondaPackException):
-        py36_env._output_and_format(format='foo')
+        py37_env._output_and_format(format='foo')
 
     with pytest.raises(CondaPackException):
-        py36_env._output_and_format(output='foo.bar')
+        py37_env._output_and_format(output='foo.bar')
 
     with pytest.raises(CondaPackException):
-        py36_env._output_and_format(output='foo.parcel', format='zip')
+        py37_env._output_and_format(output='foo.parcel', format='zip')
 
 
-def test_roundtrip(tmpdir, py36_env):
-    out_path = os.path.join(str(tmpdir), 'py36.tar')
-    py36_env.pack(out_path)
+def test_roundtrip(tmpdir, py37_env):
+    out_path = os.path.join(str(tmpdir), 'py37.tar')
+    py37_env.pack(out_path)
     assert os.path.exists(out_path)
     assert tarfile.is_tarfile(out_path)
 
     with tarfile.open(out_path) as fil:
         # Check all files are relative paths
         for member in fil.getnames():
             assert not member.startswith(os.path.sep)
 
         extract_path = str(tmpdir.join('env'))
         fil.extractall(extract_path)
 
     # Shebang rewriting happens before prefixes are fixed
     textfile = os.path.join(extract_path, BIN_DIR, 'conda-pack-test-lib1')
-    with open(textfile, 'r') as fil:
+    with open(textfile) as fil:
         shebang = fil.readline().strip()
         assert shebang == '#!/usr/bin/env python'
 
     # Check conda-unpack --help and --version
     if on_win:
         binary_name = 'conda-unpack.exe'
         script_name = 'conda-unpack-script.py'
@@ -348,34 +352,40 @@
         if fix_dest:
             # XXX: Conda windows activatation scripts now seem to assume a base
             # conda install, rather than relative paths. Given that this tool
             # is mostly for deploying code, and usually on servers (not
             # windows), this failure isn't critical but isn't 100% correct.
             # Ideally this test shouldn't need to special case `fix_dest`, and
             # use the same batch commands in both cases.
-            commands = (r"@call {path}\condabin\conda activate".format(path=extract_path),
-                        r"@conda info --json",
-                        r"@conda deactivate")
+            commands = (
+                fr"@call {extract_path}\condabin\conda activate",
+                r"@conda info --json",
+                r"@conda deactivate",
+            )
         else:
-            commands = (r"@set CONDA_PREFIX=",
-                        r"@set CONDA_SHVL=",
-                        r"@call {path}\Scripts\activate".format(path=extract_path),
-                        r"@conda info --json",
-                        r"@deactivate")
-        script_file = tmpdir.join('unpack.bat')
-        cmd = ['cmd', '/c', str(script_file)]
+            commands = (
+                r"@set CONDA_PREFIX=",
+                r"@set CONDA_SHVL=",
+                fr"@call {extract_path}\Scripts\activate",
+                r"@conda info --json",
+                r"@deactivate",
+            )
+        script_file = tmpdir.join("unpack.bat")
+        cmd = ["cmd", "/c", str(script_file)]
 
     else:
-        commands = ("unset CONDA_PREFIX",
-                    "unset CONDA_SHLVL",
-                    ". {path}/bin/activate".format(path=extract_path),
-                    "conda info --json",
-                    ". deactivate >/dev/null 2>/dev/null")
-        script_file = tmpdir.join('unpack.sh')
-        cmd = ['/usr/bin/env', 'bash', str(script_file)]
+        commands = (
+            "unset CONDA_PREFIX",
+            "unset CONDA_SHLVL",
+            f". {extract_path}/bin/activate",
+            "conda info --json",
+            ". deactivate >/dev/null 2>/dev/null",
+        )
+        script_file = tmpdir.join("unpack.sh")
+        cmd = ["/usr/bin/env", "bash", str(script_file)]
 
     script_file.write('\n'.join(commands))
     out = subprocess.check_output(cmd, stderr=subprocess.STDOUT).decode()
     conda_info = json.loads(out)
     extract_path_n = normpath(extract_path)
     for var in ('conda_prefix', 'sys.prefix', 'default_prefix', 'root_prefix'):
         assert normpath(conda_info[var]) == extract_path_n
@@ -390,22 +400,22 @@
             if field in data:
                 assert data[field] == ""
 
         if "link" in data and "source" in data["link"]:
             assert data["link"]["source"] == ""
 
 
-def test_pack_exceptions(py36_env):
+def test_pack_exceptions(py37_env):
     # Can't pass both prefix and name
     with pytest.raises(CondaPackException):
-        pack(prefix=py36_path, name='py36')
+        pack(prefix=py37_path, name='py37')
 
     # Unknown filter type
     with pytest.raises(CondaPackException):
-        pack(prefix=py36_path,
+        pack(prefix=py37_path,
              filters=[("exclude", "*.py"),
                       ("foo", "*.pyc")])
 
 
 def test_zip64(tmpdir):
     # Create an environment that requires ZIP64 extensions, but doesn't use a
     # lot of disk/RAM
@@ -425,63 +435,63 @@
     assert not os.path.exists(out_path)
 
     # Works fine if ZIP64 not disabled
     large_env.pack(output=out_path)
     assert os.path.exists(out_path)
 
 
-def test_force(tmpdir, py36_env):
-    already_exists = os.path.join(str(tmpdir), 'py36.tar')
+def test_force(tmpdir, py37_env):
+    already_exists = os.path.join(str(tmpdir), 'py37.tar')
     with open(already_exists, 'wb'):
         pass
 
     # file already exists
     with pytest.raises(CondaPackException):
-        py36_env.pack(output=already_exists)
+        py37_env.pack(output=already_exists)
 
-    py36_env.pack(output=already_exists, force=True)
+    py37_env.pack(output=already_exists, force=True)
     assert tarfile.is_tarfile(already_exists)
 
 
-def test_pack(tmpdir, py36_env):
-    out_path = os.path.join(str(tmpdir), 'py36.tar')
+def test_pack(tmpdir, py37_env):
+    out_path = os.path.join(str(tmpdir), 'py37.tar')
 
     exclude1 = "*.py"
     exclude2 = "*.pyc"
-    include = os.path.join(SP_36, 'conda_pack_test_lib1', '*')
+    include = os.path.join(SP_37, 'conda_pack_test_lib1', '*')
 
-    res = pack(prefix=py36_path,
+    res = pack(prefix=py37_path,
                output=out_path,
                filters=[("exclude", exclude1),
                         ("exclude", exclude2),
                         ("include", include)])
 
     assert res == out_path
     assert os.path.exists(out_path)
     assert tarfile.is_tarfile(out_path)
 
     with tarfile.open(out_path) as fil:
         paths = fil.getnames()
 
-    filtered = (py36_env
+    filtered = (py37_env
                 .exclude(exclude1)
                 .exclude(exclude2)
                 .include(include))
 
     # Files line up with filtering, with extra conda-unpack command
-    sol = set(os.path.normcase(f.target) for f in filtered.files)
-    res = set(os.path.normcase(p) for p in paths)
+    sol = {os.path.normcase(f.target) for f in filtered.files}
+    res = {os.path.normcase(p) for p in paths}
     diff = res.difference(sol)
 
     if on_win:
         fnames = ('conda-unpack.exe', 'conda-unpack-script.py',
                   'activate.bat', 'deactivate.bat')
     else:
         fnames = ('conda-unpack', 'activate', 'deactivate')
-    assert diff == set(os.path.join(BIN_DIR_L, f) for f in fnames)
+    assert diff == {os.path.join(BIN_DIR_L, f) for f in fnames}
 
 
 def _test_dest_prefix(src_prefix, dest_prefix, arcroot, out_path, format):
     if on_win:
         test_files = ['Scripts/conda-pack-test-lib1',
                       'Scripts/pytest.exe']
     else:
@@ -507,64 +517,64 @@
                 orig_data = fil2.read()
             if orig_bytes in orig_data:
                 data = fil.extractfile(dest_path).read()
                 assert orig_bytes not in data and orig_bytes_l not in data, test_file
                 assert new_bytes in data or new_bytes_l in data, test_file
 
 
-def test_dest_prefix(tmpdir, py36_env):
-    out_path = os.path.join(str(tmpdir), 'py36.tar')
+def test_dest_prefix(tmpdir, py37_env):
+    out_path = os.path.join(str(tmpdir), 'py37.tar')
     dest = r'c:\foo\bar\baz\biz' if on_win else '/foo/bar/baz/biz'
-    res = pack(prefix=py36_path,
+    res = pack(prefix=py37_path,
                dest_prefix=dest,
                output=out_path)
 
     assert res == out_path
     assert os.path.exists(out_path)
     assert tarfile.is_tarfile(out_path)
 
-    _test_dest_prefix(py36_env.prefix, dest, '', out_path, 'r')
+    _test_dest_prefix(py37_env.prefix, dest, '', out_path, 'r')
 
 
-def test_parcel(tmpdir, py36_env):
+def test_parcel(tmpdir, py37_env):
     if on_win:
         pytest.skip("Not parcel tests on Windows")
-    arcroot = 'py36-1234.56'
+    arcroot = 'py37-1234.56'
 
     out_path = os.path.join(str(tmpdir), arcroot + '-el7.parcel')
 
     pdir = os.getcwd()
     try:
         os.chdir(str(tmpdir))
-        res = pack(prefix=py36_path, format='parcel', parcel_version='1234.56')
+        res = pack(prefix=py37_path, format='parcel', parcel_version='1234.56')
     finally:
         os.chdir(pdir)
 
     assert os.path.join(str(tmpdir), res) == out_path
     assert os.path.exists(out_path)
 
     # Verify that only the parcel files were added
     with tarfile.open(out_path, 'r:gz') as fil:
         paths = fil.getnames()
-    sol = set(os.path.join(arcroot, f.target) for f in py36_env.files)
+    sol = {os.path.join(arcroot, f.target) for f in py37_env.files}
     diff = set(paths).difference(sol)
-    fnames = ('conda_env.sh', 'parcel.json')
-    assert diff == set(os.path.join(arcroot, 'meta', f) for f in fnames)
+    fnames = ("conda_env.sh", "parcel.json")
+    assert diff == {os.path.join(arcroot, "meta", f) for f in fnames}
 
     # Verify correct metadata in parcel.json
     with tarfile.open(out_path) as fil:
         fpath = os.path.join(arcroot, 'meta', 'parcel.json')
         data = fil.extractfile(fpath).read()
     data = json.loads(data)
-    assert data['name'] == 'py36' and data['components'][0]['name'] == 'py36'
+    assert data['name'] == 'py37' and data['components'][0]['name'] == 'py37'
     assert data['version'] == '1234.56' and data['components'][0]['version'] == '1234.56'
 
     # Verify the correct dest_prefix substitution
     dest = os.path.join('/opt/cloudera/parcels', arcroot)
-    _test_dest_prefix(py36_env.prefix, dest, arcroot, out_path, 'r:gz')
+    _test_dest_prefix(py37_env.prefix, dest, arcroot, out_path, 'r:gz')
 
 
 def test_activate(tmpdir):
     out_path = os.path.join(str(tmpdir), 'activate_scripts.tar')
     extract_path = str(tmpdir.join('env'))
 
     env = CondaEnv.from_prefix(activate_scripts_path)
```

### Comparing `conda-pack-0.7.0/conda_pack/tests/test_formats.py` & `conda-pack-0.7.1/conda_pack/tests/test_formats.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 import shutil
 import subprocess
 import tarfile
 import threading
 import time
 import zipfile
 from multiprocessing import cpu_count
-from os.path import isdir, isfile, islink, join, exists
-from subprocess import check_output, STDOUT
+from os.path import exists, isdir, isfile, islink, join
+from subprocess import STDOUT, check_output
 
 import pytest
 
+from conda_pack.compat import PY2, on_linux, on_mac, on_win
 from conda_pack.core import CondaPackException
-from conda_pack.formats import archive, _parse_n_threads
-from conda_pack.compat import on_win, on_mac, on_linux, PY2
+from conda_pack.formats import _parse_n_threads, archive
 
 
 @pytest.fixture(scope="module")
 def root_and_paths(tmpdir_factory):
     root = str(tmpdir_factory.mktemp('example_dir'))
 
     def mkfil(*paths):
```

### Comparing `conda-pack-0.7.0/conda_pack.egg-info/PKG-INFO` & `conda-pack-0.7.1/conda_pack.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 Metadata-Version: 2.1
 Name: conda-pack
-Version: 0.7.0
+Version: 0.7.1
 Summary: Package conda environments for redistribution
 Home-page: https://conda.github.io/conda-pack/
 Maintainer: Jim Crist
 Maintainer-email: jiminy.crist@gmail.com
 License: BSD
 Project-URL: Source Code, https://github.com/conda/conda-pack
 Keywords: conda packaging
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Topic :: System :: Software Distribution
 Classifier: Topic :: Software Development :: Build Tools
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Conda-Pack
 
 `conda-pack` is a command line tool for creating relocatable conda
 environments. This is useful for deploying code in a consistent environment,
 potentially in locations where python or conda isn't already installed.
 
 See the <a href="https://conda.github.io/conda-pack/">documentation</a>
 for more information.
 
 Conda-pack is offered under a New BSD license; see the
-<a href="https://github.com/conda/conda-pack/blob/master/LICENSE.txt">license file</a>.
+<a href="https://github.com/conda/conda-pack/blob/main/LICENSE.txt">license file</a>.
 
 ## Build status
 
-| [![Build status](https://github.com/conda/conda-pack/workflows/Build%20and%20test%20the%20package/badge.svg)](https://github.com/conda/conda-pack/actions) [![codecov](https://codecov.io/gh/conda/conda-pack/branch/master/graph/badge.svg)](https://codecov.io/gh/conda/conda-pack) | [![Anaconda-Server Badge](https://anaconda.org/ctools/conda-pack/badges/latest_release_date.svg)](https://anaconda.org/ctools/conda-pack) |
+| [![Build status](https://github.com/conda/conda-pack/actions/workflows/main.yml/badge.svg)](https://github.com/conda/conda-pack/actions/workflows/main.yml) [![codecov](https://codecov.io/gh/conda/conda-pack/branch/main/graph/badge.svg)](https://codecov.io/gh/conda/conda-pack) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/conda/conda-pack/main.svg)](https://results.pre-commit.ci/latest/github/conda/conda-pack/main) | [![Anaconda-Server Badge](https://anaconda.org/ctools/conda-pack/badges/latest_release_date.svg)](https://anaconda.org/ctools/conda-pack) |
 | --- | :-: |
 | [`conda install ctools/label/dev::conda-pack`](https://anaconda.org/ctools/conda-pack) | [![Anaconda-Server Badge](https://anaconda.org/ctools/conda-pack/badges/version.svg)](https://anaconda.org/ctools/conda-pack) |
 | [`conda install defaults::conda-pack`](https://anaconda.org/anaconda/conda-pack) | [![Anaconda-Server Badge](https://anaconda.org/anaconda/conda-pack/badges/version.svg)](https://anaconda.org/anaconda/conda-pack) |
 | [`conda install conda-forge::conda-pack`](https://anaconda.org/conda-forge/conda-pack) | [![Anaconda-Server Badge](https://anaconda.org/conda-forge/conda-pack/badges/version.svg)](https://anaconda.org/conda-forge/conda-pack) |
```

#### html2text {}

```diff
@@ -1,32 +1,33 @@
-Metadata-Version: 2.1 Name: conda-pack Version: 0.7.0 Summary: Package conda
+Metadata-Version: 2.1 Name: conda-pack Version: 0.7.1 Summary: Package conda
 environments for redistribution Home-page: https://conda.github.io/conda-pack/
 Maintainer: Jim Crist Maintainer-email: jiminy.crist@gmail.com License: BSD
 Project-URL: Source Code, https://github.com/conda/conda-pack Keywords: conda
 packaging Classifier: Development Status :: 4 - Beta Classifier: License :: OSI
-Approved :: BSD License Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Topic :: System
-:: Archiving :: Packaging Classifier: Topic :: System :: Software Distribution
-Classifier: Topic :: Software Development :: Build Tools Requires-Python: >=3.6
-Description-Content-Type: text/markdown License-File: LICENSE.txt # Conda-Pack
-`conda-pack` is a command line tool for creating relocatable conda
-environments. This is useful for deploying code in a consistent environment,
-potentially in locations where python or conda isn't already installed. See the
-documentation for more information. Conda-pack is offered under a New BSD
-license; see the license_file. ## Build status | [![Build status](https://
-github.com/conda/conda-pack/workflows/Build%20and%20test%20the%20package/
-badge.svg)](https://github.com/conda/conda-pack/actions) [![codecov](https://
-codecov.io/gh/conda/conda-pack/branch/master/graph/badge.svg)](https://
-codecov.io/gh/conda/conda-pack) | [![Anaconda-Server Badge](https://
-anaconda.org/ctools/conda-pack/badges/latest_release_date.svg)](https://
-anaconda.org/ctools/conda-pack) | | --- | :-: | | [`conda install ctools/label/
-dev::conda-pack`](https://anaconda.org/ctools/conda-pack) | [![Anaconda-Server
-Badge](https://anaconda.org/ctools/conda-pack/badges/version.svg)](https://
-anaconda.org/ctools/conda-pack) | | [`conda install defaults::conda-pack`]
-(https://anaconda.org/anaconda/conda-pack) | [![Anaconda-Server Badge](https://
-anaconda.org/anaconda/conda-pack/badges/version.svg)](https://anaconda.org/
-anaconda/conda-pack) | | [`conda install conda-forge::conda-pack`](https://
-anaconda.org/conda-forge/conda-pack) | [![Anaconda-Server Badge](https://
-anaconda.org/conda-forge/conda-pack/badges/version.svg)](https://anaconda.org/
-conda-forge/conda-pack) |
+Approved :: BSD License Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: System :: Archiving :: Packaging Classifier: Topic ::
+System :: Software Distribution Classifier: Topic :: Software Development ::
+Build Tools Requires-Python: >=3.7 Description-Content-Type: text/markdown
+License-File: LICENSE.txt # Conda-Pack `conda-pack` is a command line tool for
+creating relocatable conda environments. This is useful for deploying code in a
+consistent environment, potentially in locations where python or conda isn't
+already installed. See the documentation for more information. Conda-pack is
+offered under a New BSD license; see the license_file. ## Build status | [!
+[Build status](https://github.com/conda/conda-pack/actions/workflows/main.yml/
+badge.svg)](https://github.com/conda/conda-pack/actions/workflows/main.yml) [!
+[codecov](https://codecov.io/gh/conda/conda-pack/branch/main/graph/badge.svg)]
+(https://codecov.io/gh/conda/conda-pack) [![pre-commit.ci status](https://
+results.pre-commit.ci/badge/github/conda/conda-pack/main.svg)](https://
+results.pre-commit.ci/latest/github/conda/conda-pack/main) | [![Anaconda-Server
+Badge](https://anaconda.org/ctools/conda-pack/badges/latest_release_date.svg)]
+(https://anaconda.org/ctools/conda-pack) | | --- | :-: | | [`conda install
+ctools/label/dev::conda-pack`](https://anaconda.org/ctools/conda-pack) | [!
+[Anaconda-Server Badge](https://anaconda.org/ctools/conda-pack/badges/
+version.svg)](https://anaconda.org/ctools/conda-pack) | | [`conda install
+defaults::conda-pack`](https://anaconda.org/anaconda/conda-pack) | [![Anaconda-
+Server Badge](https://anaconda.org/anaconda/conda-pack/badges/version.svg)]
+(https://anaconda.org/anaconda/conda-pack) | | [`conda install conda-forge::
+conda-pack`](https://anaconda.org/conda-forge/conda-pack) | [![Anaconda-Server
+Badge](https://anaconda.org/conda-forge/conda-pack/badges/version.svg)](https:/
+/anaconda.org/conda-forge/conda-pack) |
```

### Comparing `conda-pack-0.7.0/conda_pack.egg-info/SOURCES.txt` & `conda-pack-0.7.1/conda_pack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `conda-pack-0.7.0/docs/Makefile` & `conda-pack-0.7.1/docs/Makefile`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
 .PHONY: help Makefile
 
 # Catch-all target: route all unknown targets to Sphinx using the new
 # "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
 %: Makefile
-	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `conda-pack-0.7.0/docs/make.bat` & `conda-pack-0.7.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `conda-pack-0.7.0/docs/source/conf.py` & `conda-pack-0.7.1/docs/source/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import alabaster
+
 import conda_pack
 
 # Project settings
 project = 'conda-pack'
 copyright = '2017, Jim Crist'
 author = 'Jim Crist'
 release = version = conda_pack.__version__
```

### Comparing `conda-pack-0.7.0/docs/source/index.rst` & `conda-pack-0.7.1/docs/source/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,17 @@
   this is to use `Skein <https://jcrist.github.io/skein/>`_.
 
 - Archiving an environment in a functioning state. Note that a more sustainable
   way to do this is to specify your environment as a `environment.yml
   <https://conda.io/docs/user-guide/tasks/manage-environments.html#sharing-an-environment>`_,
   and recreate the environment when needed.
 
+- Packaging an environment as single executable with entrypoint to run on execution (see the
+  instructions for :doc:`Linux and macOS <unix-binary>`).
+
 - *BETA*: Packaging a conda environment as a standard Cloudera parcel. This is
   a newly added capability. It has been tested on a live cluster, but different
   cluster configurations may produce different results. We welcome users to
   `file an issue <https://github.com/conda/conda-pack/issues>`_ if necessary.
   :doc:`See here <parcel>` for more information).
 
 Installation
@@ -175,8 +178,8 @@
     :hidden:
 
     cli.rst
     api.rst
     spark.rst
     parcel.rst
     squashfs.rst
-
+    unix-binary.rst
```

#### html2text {}

```diff
@@ -12,19 +12,20 @@
 deployment - Packaging a conda environment for use with Apache Spark when
 deploying on YARN (:doc:`see here ` for more information). - Packaging a conda
 environment for deployment on Apache YARN. One way to do this is to use `Skein
 jcrist.github.io/skein/>`_. - Archiving an environment in a functioning state.
 Note that a more sustainable way to do this is to specify your environment as a
 `environment.yml
 conda.io/docs/user-guide/tasks/manage-environments.html#sharing-an-
-environment>`_, and recreate the environment when needed. - *BETA*: Packaging a
-conda environment as a standard Cloudera parcel. This is a newly added
-capability. It has been tested on a live cluster, but different cluster
-configurations may produce different results. We welcome users to `file an
-issue
+environment>`_, and recreate the environment when needed. - Packaging an
+environment as single executable with entrypoint to run on execution (see the
+instructions for :doc:`Linux and macOS `). - *BETA*: Packaging a conda
+environment as a standard Cloudera parcel. This is a newly added capability. It
+has been tested on a live cluster, but different cluster configurations may
+produce different results. We welcome users to `file an issue
 github.com/conda/conda-pack/issues>`_ if necessary. :doc:`See here ` for more
 information). Installation ------------ It's recommended to install in your
 root conda environment - the ``conda pack`` command will then be available in
 all sub-environments as well. **Install with conda:** ``conda-pack`` is
 available from `Anaconda
 anaconda.com>`_ as well as from `conda-forge
 conda-forge.org/>`_: .. code:: conda install conda-pack conda install -c conda-
@@ -65,8 +66,9 @@
 environment was built must match the OS of the target. This means that
 environments built on Windows can't be relocated to Linux. - Once an
 environment is unpacked and ``conda-unpack`` has been executed, it *cannot* be
 relocated. Re-applying ``conda-pack`` is unlikely to work. - ``conda-pack`` is
 not well-suited for archiving old environments, because it requires that
 conda's package cache have all of the environment's packages present. It is
 intended for building archives from actively maintained conda environments. ..
-toctree:: :hidden: cli.rst api.rst spark.rst parcel.rst squashfs.rst
+toctree:: :hidden: cli.rst api.rst spark.rst parcel.rst squashfs.rst unix-
+binary.rst
```

### Comparing `conda-pack-0.7.0/docs/source/parcel.rst` & `conda-pack-0.7.1/docs/source/parcel.rst`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   directory. Parcel names may not have dashes ``-``, however, so if the name of the
   environment contains a dash, use this option to provide a compliant alternative.
 - ``--parcel-version``: the version of the parcel
 
   This is generally expected to follow a standard `semver <https://semver.org/>`_
   format. If not supplied, conda-pack will autogenerate one from today's date in
   ``YYYY.MM.DD`` format.
-- ``--parcel-distribution``: the target distribution for the parcel. 
+- ``--parcel-distribution``: the target distribution for the parcel.
 
   This is an abbreviation describing the specific operating system on which
   your Cloudera clsuter runs. Its default value is ``el7``, corresponding
   to RHEL7/CentOS7. Other common values include ``el6``, ``sles12``, ``bionic``,
   and ``xenial``.
 
 - ``--parcel-root``: the location where parcels are unpacked on the cluster
@@ -69,8 +69,7 @@
 
 .. code-block:: bash
 
     $ conda pack -n example --format parcel --parcel-name=sklearn
     Collecting packages...
     Packing environment at '/Users/mgrant/miniconda3/envs/example' to 'sklearn-2020.09.15-el7.parcel'
     [########################################] | 100% Completed |  9.8s
-
```

### Comparing `conda-pack-0.7.0/docs/source/spark.rst` & `conda-pack-0.7.1/docs/source/spark.rst`

 * *Files identical despite different names*

### Comparing `conda-pack-0.7.0/docs/source/squashfs.rst` & `conda-pack-0.7.1/docs/source/squashfs.rst`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -114,8 +114,8 @@
 .. code-block:: bash
 
     $ mkdir writeable_env
     $ sudo mount -t overlay overlay \
         -o lowerdir=squashFS_mountpoint,upperdir=upperdir,workdir=workdir writeable_env
 
 Any files created in the ``writeable_env`` directory will also show up in ``upperdir``.
-After unmounting, delete ``upperdir`` and ``workdir`` and all changes made to the environment will be gone.
+After unmounting, delete ``upperdir`` and ``workdir`` and all changes made to the environment will be gone.
```

### Comparing `conda-pack-0.7.0/setup.py` & `conda-pack-0.7.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
+
 import versioneer
 
 setup(name='conda-pack',
       version=versioneer.get_version(),
       cmdclass=versioneer.get_cmdclass(),
       url='https://conda.github.io/conda-pack/',
       project_urls={"Source Code": "https://github.com/conda/conda-pack"},
       maintainer='Jim Crist',
       maintainer_email='jiminy.crist@gmail.com',
       keywords='conda packaging',
       classifiers=["Development Status :: 4 - Beta",
                    "License :: OSI Approved :: BSD License",
-                   "Programming Language :: Python :: 3.6",
                    "Programming Language :: Python :: 3.7",
                    "Programming Language :: Python :: 3.8",
                    "Programming Language :: Python :: 3.9",
                    "Programming Language :: Python :: 3.10",
                    "Topic :: System :: Archiving :: Packaging",
                    "Topic :: System :: Software Distribution",
                    "Topic :: Software Development :: Build Tools"],
@@ -26,9 +26,9 @@
       packages=['conda_pack'],
       package_data={'conda_pack': ['scripts/windows/*', 'scripts/posix/*']},
       entry_points='''
         [console_scripts]
         conda-pack=conda_pack.cli:main
       ''',
       install_requires=['setuptools'],
-      python_requires='>=3.6',
+      python_requires='>=3.7',
       zip_safe=False)
```

### Comparing `conda-pack-0.7.0/testing/setup_envs.sh` & `conda-pack-0.7.1/testing/setup_envs.sh`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#/usr/bin/env bash
+#!/usr/bin/env bash
 
 set -Eeo pipefail
 
 echo Setting up environments for testing
 
 # GitHub action specific items. These are no-ops locally
 [ "$RUNNER_OS" == "Windows" ] && CONDA_EXE="$CONDA/Scripts/conda.exe"
@@ -31,59 +31,59 @@
     exit 0
 fi
 
 mkdir -p $envs
 # Make sure the local package cache is used
 rm -rf $croot/pkgs
 
-echo Creating py27 environment
-env=$envs/py27
-conda env create -f $ymls/py27.yml -p $env
-# Remove this package from the cache for testing
-rm -rf $croot/pkgs/conda_pack_test_lib2*py27*
-
-echo Creating py36 environment
-env=$envs/py36
-conda env create -f $ymls/py36.yml -p $env
+echo Creating py37 environment
+env=$envs/py37
+conda env create -f $ymls/py37.yml -p $env
 # Create unmanaged conda-related files for conda-pack to remove
 if [ -f $env/python.exe ]; then
     touch $env/Scripts/activate
     touch $env/Scripts/activate.bat
     touch $env/Scripts/deactivate
     touch $env/Scripts/deactivate.bat
     touch $env/Scripts/conda
     touch $env/Scripts/conda.bat
 else
     touch $env/bin/activate
     touch $env/bin/deactivate
     touch $env/bin/conda
 fi
 
-echo Creating py36_editable environment
-env=$envs/py36_editable
-conda env create -f $ymls/py36.yml -p $env
+echo Creating py310 environment
+env=$envs/py310
+conda env create -f $ymls/py310.yml -p $env
+# Remove this package from the cache for testing
+rm -rf $croot/pkgs/conda_pack_test_lib2*py310*
+
+echo Creating py37_editable environment
+env=$envs/py37_editable
+conda env create -f $ymls/py37.yml -p $env
 pushd $cwd/test_packages/conda_pack_test_lib1
 if [ -f $env/python.exe ]; then
     $env/python.exe setup.py develop
 else
     $env/bin/python setup.py develop
 fi
 popd
 
-echo Creating py36_broken environment
-env=$envs/py36_broken
-conda env create -f $ymls/py36_broken.yml -p $env
-
-echo Creating py36_missing_files environment
-env=$envs/py36_missing_files
-conda env create -f $ymls/py36.yml -p $env
+echo Creating py37_broken environment
+env=$envs/py37_broken
+conda env create -f $ymls/py37_broken.yml -p $env
+
+echo Creating py37_missing_files environment
+env=$envs/py37_missing_files
+conda env create -f $ymls/py37.yml -p $env
 if [ -f $env/python.exe ]; then
     rm $env/lib/site-packages/toolz/*.py
 else
-    rm $env/lib/python3.6/site-packages/toolz/*.py
+    rm $env/lib/python3.7/site-packages/toolz/*.py
 fi
 
 echo Creating nopython environment
 env=$envs/nopython
 conda env create -f $ymls/nopython.yml -p $env
 
 echo Creating conda environment
```

### Comparing `conda-pack-0.7.0/versioneer.py` & `conda-pack-0.7.1/versioneer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1834,14 +1834,15 @@
                                               cfg.versionfile_build)
             print("UPDATING %s" % target_versionfile)
             write_to_version_file(target_versionfile, versions)
     cmds["build_ext"] = cmd_build_ext
 
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
         from cx_Freeze.dist import build_exe as _build_exe
+
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
         #   ...
```

