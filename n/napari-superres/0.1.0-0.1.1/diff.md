# Comparing `tmp/napari-superres-0.1.0.tar.gz` & `tmp/napari-superres-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-superres-0.1.0.tar", last modified: Thu Jun 29 20:39:49 2023, max compression
+gzip compressed data, was "napari-superres-0.1.1.tar", last modified: Tue Aug  8 11:07:10 2023, max compression
```

## Comparing `napari-superres-0.1.0.tar` & `napari-superres-0.1.1.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 20:39:49.539107 napari-superres-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-06-29 20:39:49.276903 napari-superres-0.1.0/.github/
-drwxrwxrwx   0        0        0        0 2023-06-29 20:39:49.338085 napari-superres-0.1.0/.github/workflows/
--rw-rw-rw-   0        0        0     3092 2023-06-29 19:19:30.000000 napari-superres-0.1.0/.github/workflows/test_and_deploy.yml
--rw-rw-rw-   0        0        0     1076 2023-06-28 17:02:45.000000 napari-superres-0.1.0/.gitignore
-drwxrwxrwx   0        0        0        0 2023-06-29 20:39:49.341046 napari-superres-0.1.0/.napari/
--rw-rw-rw-   0        0        0     4295 2022-01-18 11:27:27.000000 napari-superres-0.1.0/.napari/DESCRIPTION.md
--rw-rw-rw-   0        0        0     1210 2023-06-28 17:02:45.000000 napari-superres-0.1.0/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0     1637 2023-06-28 17:02:45.000000 napari-superres-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      101 2023-06-28 17:02:45.000000 napari-superres-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     8627 2023-06-29 20:39:49.540103 napari-superres-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0   150036 2023-06-29 19:42:06.000000 napari-superres-0.1.0/README.html
--rw-rw-rw-   0        0        0     7119 2023-06-29 19:42:06.000000 napari-superres-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 20:39:49.444691 napari-superres-0.1.0/docs/
--rw-rw-rw-   0        0        0    11768 2023-06-29 16:13:21.000000 napari-superres-0.1.0/docs/ESI.png
--rw-rw-rw-   0        0        0   127583 2022-05-31 22:47:18.000000 napari-superres-0.1.0/docs/ESI_Original_donuts.png
--rw-rw-rw-   0        0        0    24650 2022-05-31 22:47:58.000000 napari-superres-0.1.0/docs/ESI_Processed_nrResImage_1_nrBins_2_esi_order_1_donuts.png
--rw-rw-rw-   0        0        0   404493 2022-05-29 20:40:08.000000 napari-superres-0.1.0/docs/Fig_2a_MSSR_Garcia_2021.png
--rw-rw-rw-   0        0        0   985552 2022-05-29 20:05:40.000000 napari-superres-0.1.0/docs/Fig_6_ESI_Alva_2022.png
--rw-rw-rw-   0        0        0   713398 2022-05-29 20:01:37.000000 napari-superres-0.1.0/docs/Fig_7_SRRF_Alva_2022.png
--rw-rw-rw-   0        0        0    23596 2023-06-28 17:02:45.000000 napari-superres-0.1.0/docs/MSSR.png
--rw-rw-rw-   0        0        0     4070 2022-05-31 16:22:56.000000 napari-superres-0.1.0/docs/MSSR_Processed_amp_2_PSFp_1_order_1_raw7_100_donuts.png
--rw-rw-rw-   0        0        0     4602 2022-05-31 16:23:31.000000 napari-superres-0.1.0/docs/MSSR_original_donuts.png
--rw-rw-rw-   0        0        0   104045 2023-06-29 16:13:21.000000 napari-superres-0.1.0/docs/MUSICAL-CardioMyoblast_Mitochondria.png
--rw-rw-rw-   0        0        0  1446365 2023-06-28 17:02:45.000000 napari-superres-0.1.0/docs/SOFI.png
--rw-rw-rw-   0        0        0    14707 2023-06-29 16:13:21.000000 napari-superres-0.1.0/docs/SRRF.png
--rw-rw-rw-   0        0        0   721108 2022-05-31 16:37:29.000000 napari-superres-0.1.0/docs/SRRF_Original_Microtubules.png
--rw-rw-rw-   0        0        0    93875 2022-05-31 16:25:59.000000 napari-superres-0.1.0/docs/SRRF_processed_mag_2_rad_3_symAxis_3_fstart_0_fend_3_Microtubules.png
--rw-rw-rw-   0        0        0    21295 2023-05-06 12:25:31.000000 napari-superres-0.1.0/docs/TMSSR.png
--rw-rw-rw-   0        0        0       76 2022-01-18 11:27:27.000000 napari-superres-0.1.0/docs/index.md
--rw-rw-rw-   0        0        0    12657 2023-06-28 17:02:45.000000 napari-superres-0.1.0/docs/musical_mean.png
--rw-rw-rw-   0        0        0    18915 2023-06-28 17:02:45.000000 napari-superres-0.1.0/docs/noMSSR.png
--rw-rw-rw-   0        0        0   367427 2023-06-28 17:02:45.000000 napari-superres-0.1.0/docs/noSOFI.png
--rw-rw-rw-   0        0        0    52408 2023-06-29 16:13:21.000000 napari-superres-0.1.0/docs/single-frame-good-exposure.png
--rw-rw-rw-   0        0        0    52547 2023-06-29 16:13:21.000000 napari-superres-0.1.0/docs/single-frame-good-exposure.tif
--rw-rw-rw-   0        0        0     9951 2023-06-29 16:13:21.000000 napari-superres-0.1.0/docs/synt.png
--rw-rw-rw-   0        0        0    41692 2023-06-29 16:13:21.000000 napari-superres-0.1.0/docs/tmssr-mean-mag2.png
--rw-rw-rw-   0        0        0      349 2023-06-28 17:02:45.000000 napari-superres-0.1.0/mkdocs.yml
--rw-rw-rw-   0        0        0     1981 2023-06-29 20:39:49.544272 napari-superres-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0       89 2023-06-29 20:31:37.000000 napari-superres-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 20:39:49.286320 napari-superres-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-29 20:39:49.502240 napari-superres-0.1.0/src/napari_superres/
--rw-rw-rw-   0        0        0      524 2023-06-28 17:02:45.000000 napari-superres-0.1.0/src/napari_superres/__init__.py
--rw-rw-rw-   0        0        0    40480 2023-06-29 16:13:21.000000 napari-superres-0.1.0/src/napari_superres/_gui_creator.py
--rw-rw-rw-   0        0        0     2556 2023-06-28 17:02:45.000000 napari-superres-0.1.0/src/napari_superres/_reader.py
-drwxrwxrwx   0        0        0        0 2023-06-29 20:39:49.536129 napari-superres-0.1.0/src/napari_superres/_tests/
--rw-rw-rw-   0        0        0        0 2022-01-18 11:27:27.000000 napari-superres-0.1.0/src/napari_superres/_tests/__init__.py
--rw-rw-rw-   0        0        0     1008 2023-06-28 17:02:45.000000 napari-superres-0.1.0/src/napari_superres/_tests/test_reader.py
--rw-rw-rw-   0        0        0     1284 2023-06-28 17:02:45.000000 napari-superres-0.1.0/src/napari_superres/_tests/test_widget.py
--rw-rw-rw-   0        0        0      131 2023-06-28 17:02:45.000000 napari-superres-0.1.0/src/napari_superres/_tests/test_writer.py
--rw-rw-rw-   0        0        0      200 2023-06-29 20:31:48.000000 napari-superres-0.1.0/src/napari_superres/_version.py
--rw-rw-rw-   0        0        0      956 2023-06-28 17:02:45.000000 napari-superres-0.1.0/src/napari_superres/_writer.py
--rw-rw-rw-   0        0        0     7782 2023-06-28 17:02:45.000000 napari-superres-0.1.0/src/napari_superres/core_decor.py
--rw-rw-rw-   0        0        0     6922 2023-06-28 17:02:45.000000 napari-superres-0.1.0/src/napari_superres/core_esi.py
--rw-rw-rw-   0        0        0     6783 2023-06-28 17:02:45.000000 napari-superres-0.1.0/src/napari_superres/core_mssr.py
--rw-rw-rw-   0        0        0     7075 2023-06-28 17:02:45.000000 napari-superres-0.1.0/src/napari_superres/core_mssr_numba.py
--rw-rw-rw-   0        0        0    15947 2023-06-28 17:02:45.000000 napari-superres-0.1.0/src/napari_superres/core_musical.py
--rw-rw-rw-   0        0        0     9680 2023-06-28 17:02:45.000000 napari-superres-0.1.0/src/napari_superres/core_sofi.py
--rw-rw-rw-   0        0        0     6876 2023-06-28 17:02:45.000000 napari-superres-0.1.0/src/napari_superres/core_srrf.py
--rw-rw-rw-   0        0        0    12541 2023-06-28 17:02:45.000000 napari-superres-0.1.0/src/napari_superres/deconvsk.py
--rw-rw-rw-   0        0        0    11426 2023-06-28 17:02:45.000000 napari-superres-0.1.0/src/napari_superres/finterp.py
--rw-rw-rw-   0        0        0     6845 2023-06-28 17:02:45.000000 napari-superres-0.1.0/src/napari_superres/my_popW.py
--rw-rw-rw-   0        0        0     2229 2023-06-28 17:02:45.000000 napari-superres-0.1.0/src/napari_superres/napari.yaml
-drwxrwxrwx   0        0        0        0 2023-06-29 20:39:49.522881 napari-superres-0.1.0/src/napari_superres.egg-info/
--rw-rw-rw-   0        0        0     8627 2023-06-29 20:39:48.000000 napari-superres-0.1.0/src/napari_superres.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1809 2023-06-29 20:39:49.000000 napari-superres-0.1.0/src/napari_superres.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 20:39:48.000000 napari-superres-0.1.0/src/napari_superres.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-06-29 20:39:48.000000 napari-superres-0.1.0/src/napari_superres.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       81 2023-06-29 20:39:48.000000 napari-superres-0.1.0/src/napari_superres.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-29 20:39:48.000000 napari-superres-0.1.0/src/napari_superres.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      646 2023-06-28 17:02:45.000000 napari-superres-0.1.0/tox.ini
+drwxrwxrwx   0        0        0        0 2023-08-08 11:07:10.995291 napari-superres-0.1.1/
+drwxrwxrwx   0        0        0        0 2023-08-08 11:07:10.863349 napari-superres-0.1.1/.github/
+drwxrwxrwx   0        0        0        0 2023-08-08 11:07:10.876753 napari-superres-0.1.1/.github/workflows/
+-rw-rw-rw-   0        0        0     3092 2023-06-29 19:19:30.000000 napari-superres-0.1.1/.github/workflows/test_and_deploy.yml
+-rw-rw-rw-   0        0        0     1076 2023-06-28 17:02:45.000000 napari-superres-0.1.1/.gitignore
+drwxrwxrwx   0        0        0        0 2023-08-08 11:07:10.881288 napari-superres-0.1.1/.napari/
+-rw-rw-rw-   0        0        0   151069 2023-08-08 10:40:09.000000 napari-superres-0.1.1/.napari/DESCRIPTION.html
+-rw-rw-rw-   0        0        0     8133 2023-08-08 10:40:09.000000 napari-superres-0.1.1/.napari/DESCRIPTION.md
+-rw-rw-rw-   0        0        0     1210 2023-06-28 17:02:45.000000 napari-superres-0.1.1/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0     1637 2023-06-28 17:02:45.000000 napari-superres-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      101 2023-06-28 17:02:45.000000 napari-superres-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     9563 2023-08-08 11:07:10.995678 napari-superres-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0   151069 2023-08-08 10:41:14.000000 napari-superres-0.1.1/README.html
+-rw-rw-rw-   0        0        0     8133 2023-08-08 10:41:14.000000 napari-superres-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 11:07:10.956922 napari-superres-0.1.1/docs/
+-rw-rw-rw-   0        0        0    11768 2023-06-29 16:13:21.000000 napari-superres-0.1.1/docs/ESI.png
+-rw-rw-rw-   0        0        0   127583 2022-05-31 22:47:18.000000 napari-superres-0.1.1/docs/ESI_Original_donuts.png
+-rw-rw-rw-   0        0        0    24650 2022-05-31 22:47:58.000000 napari-superres-0.1.1/docs/ESI_Processed_nrResImage_1_nrBins_2_esi_order_1_donuts.png
+-rw-rw-rw-   0        0        0   404493 2022-05-29 20:40:08.000000 napari-superres-0.1.1/docs/Fig_2a_MSSR_Garcia_2021.png
+-rw-rw-rw-   0        0        0   985552 2022-05-29 20:05:40.000000 napari-superres-0.1.1/docs/Fig_6_ESI_Alva_2022.png
+-rw-rw-rw-   0        0        0   713398 2022-05-29 20:01:37.000000 napari-superres-0.1.1/docs/Fig_7_SRRF_Alva_2022.png
+-rw-rw-rw-   0        0        0    23596 2023-06-28 17:02:45.000000 napari-superres-0.1.1/docs/MSSR.png
+-rw-rw-rw-   0        0        0     4070 2022-05-31 16:22:56.000000 napari-superres-0.1.1/docs/MSSR_Processed_amp_2_PSFp_1_order_1_raw7_100_donuts.png
+-rw-rw-rw-   0        0        0     4602 2022-05-31 16:23:31.000000 napari-superres-0.1.1/docs/MSSR_original_donuts.png
+-rw-rw-rw-   0        0        0   104045 2023-06-29 16:13:21.000000 napari-superres-0.1.1/docs/MUSICAL-CardioMyoblast_Mitochondria.png
+-rw-rw-rw-   0        0        0  1446365 2023-06-28 17:02:45.000000 napari-superres-0.1.1/docs/SOFI.png
+-rw-rw-rw-   0        0        0    14707 2023-06-29 16:13:21.000000 napari-superres-0.1.1/docs/SRRF.png
+-rw-rw-rw-   0        0        0   721108 2022-05-31 16:37:29.000000 napari-superres-0.1.1/docs/SRRF_Original_Microtubules.png
+-rw-rw-rw-   0        0        0    93875 2022-05-31 16:25:59.000000 napari-superres-0.1.1/docs/SRRF_processed_mag_2_rad_3_symAxis_3_fstart_0_fend_3_Microtubules.png
+-rw-rw-rw-   0        0        0    21295 2023-05-06 12:25:31.000000 napari-superres-0.1.1/docs/TMSSR.png
+-rw-rw-rw-   0        0        0       76 2022-01-18 11:27:27.000000 napari-superres-0.1.1/docs/index.md
+-rw-rw-rw-   0        0        0    12657 2023-06-28 17:02:45.000000 napari-superres-0.1.1/docs/musical_mean.png
+-rw-rw-rw-   0        0        0    18915 2023-06-28 17:02:45.000000 napari-superres-0.1.1/docs/noMSSR.png
+-rw-rw-rw-   0        0        0   367427 2023-06-28 17:02:45.000000 napari-superres-0.1.1/docs/noSOFI.png
+-rw-rw-rw-   0        0        0    52408 2023-06-29 16:13:21.000000 napari-superres-0.1.1/docs/single-frame-good-exposure.png
+-rw-rw-rw-   0        0        0    52547 2023-06-29 16:13:21.000000 napari-superres-0.1.1/docs/single-frame-good-exposure.tif
+-rw-rw-rw-   0        0        0     9951 2023-06-29 16:13:21.000000 napari-superres-0.1.1/docs/synt.png
+-rw-rw-rw-   0        0        0    41692 2023-06-29 16:13:21.000000 napari-superres-0.1.1/docs/tmssr-mean-mag2.png
+-rw-rw-rw-   0        0        0      349 2023-06-28 17:02:45.000000 napari-superres-0.1.1/mkdocs.yml
+-rw-rw-rw-   0        0        0     1926 2023-08-08 11:07:10.996776 napari-superres-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0       89 2023-06-29 20:31:37.000000 napari-superres-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 11:07:10.866000 napari-superres-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-08-08 11:07:10.978418 napari-superres-0.1.1/src/napari_superres/
+-rw-rw-rw-   0        0        0      524 2023-06-28 17:02:45.000000 napari-superres-0.1.1/src/napari_superres/__init__.py
+-rw-rw-rw-   0        0        0    43306 2023-08-08 10:32:01.000000 napari-superres-0.1.1/src/napari_superres/_gui_creator.py
+-rw-rw-rw-   0        0        0     2556 2023-06-28 17:02:45.000000 napari-superres-0.1.1/src/napari_superres/_reader.py
+drwxrwxrwx   0        0        0        0 2023-08-08 11:07:10.994295 napari-superres-0.1.1/src/napari_superres/_tests/
+-rw-rw-rw-   0        0        0        0 2022-01-18 11:27:27.000000 napari-superres-0.1.1/src/napari_superres/_tests/__init__.py
+-rw-rw-rw-   0        0        0     1008 2023-06-28 17:02:45.000000 napari-superres-0.1.1/src/napari_superres/_tests/test_reader.py
+-rw-rw-rw-   0        0        0     1284 2023-06-28 17:02:45.000000 napari-superres-0.1.1/src/napari_superres/_tests/test_widget.py
+-rw-rw-rw-   0        0        0      131 2023-06-28 17:02:45.000000 napari-superres-0.1.1/src/napari_superres/_tests/test_writer.py
+-rw-rw-rw-   0        0        0      200 2023-06-29 20:31:48.000000 napari-superres-0.1.1/src/napari_superres/_version.py
+-rw-rw-rw-   0        0        0      956 2023-06-28 17:02:45.000000 napari-superres-0.1.1/src/napari_superres/_writer.py
+-rw-rw-rw-   0        0        0     7782 2023-06-28 17:02:45.000000 napari-superres-0.1.1/src/napari_superres/core_decor.py
+-rw-rw-rw-   0        0        0     6922 2023-06-28 17:02:45.000000 napari-superres-0.1.1/src/napari_superres/core_esi.py
+-rw-rw-rw-   0        0        0     6783 2023-06-28 17:02:45.000000 napari-superres-0.1.1/src/napari_superres/core_mssr.py
+-rw-rw-rw-   0        0        0     7075 2023-06-28 17:02:45.000000 napari-superres-0.1.1/src/napari_superres/core_mssr_numba.py
+-rw-rw-rw-   0        0        0    15947 2023-06-28 17:02:45.000000 napari-superres-0.1.1/src/napari_superres/core_musical.py
+-rw-rw-rw-   0        0        0     9680 2023-06-28 17:02:45.000000 napari-superres-0.1.1/src/napari_superres/core_sofi.py
+-rw-rw-rw-   0        0        0     6876 2023-06-28 17:02:45.000000 napari-superres-0.1.1/src/napari_superres/core_srrf.py
+-rw-rw-rw-   0        0        0    12541 2023-06-28 17:02:45.000000 napari-superres-0.1.1/src/napari_superres/deconvsk.py
+-rw-rw-rw-   0        0        0    11426 2023-06-28 17:02:45.000000 napari-superres-0.1.1/src/napari_superres/finterp.py
+-rw-rw-rw-   0        0        0     6845 2023-06-28 17:02:45.000000 napari-superres-0.1.1/src/napari_superres/my_popW.py
+-rw-rw-rw-   0        0        0     2229 2023-06-28 17:02:45.000000 napari-superres-0.1.1/src/napari_superres/napari.yaml
+drwxrwxrwx   0        0        0        0 2023-08-08 11:07:10.988681 napari-superres-0.1.1/src/napari_superres.egg-info/
+-rw-rw-rw-   0        0        0     9563 2023-08-08 11:07:10.000000 napari-superres-0.1.1/src/napari_superres.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1834 2023-08-08 11:07:10.000000 napari-superres-0.1.1/src/napari_superres.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 11:07:10.000000 napari-superres-0.1.1/src/napari_superres.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-08-08 11:07:10.000000 napari-superres-0.1.1/src/napari_superres.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       81 2023-08-08 11:07:10.000000 napari-superres-0.1.1/src/napari_superres.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-08-08 11:07:10.000000 napari-superres-0.1.1/src/napari_superres.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      646 2023-06-28 17:02:45.000000 napari-superres-0.1.1/tox.ini
```

### Comparing `napari-superres-0.1.0/.github/workflows/test_and_deploy.yml` & `napari-superres-0.1.1/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/.gitignore` & `napari-superres-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/.pre-commit-config.yaml` & `napari-superres-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/LICENSE` & `napari-superres-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/README.html` & `napari-superres-0.1.1/.napari/DESCRIPTION.html`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 <a href="https://napari-hub.org/plugins/napari-superres"><img src="https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/RoccoDAnt/napari-superres" alt="napari hub"></a></p>
 <p>A collection of super-resolution microscopy FF-SRM methods.</p>
 <p>Open-source implementation of methods for Fluorescence Fluctuation based Super Resolution Microscopy (FF-SRM):</p>
 <p>Review: <a href="https://onlinelibrary.wiley.com/doi/10.1111/jmi.13135">Alva et al., 2022. &#x201C;Fluorescence Fluctuation-Based Super-Resolution Microscopy: Basic Concepts for an Easy Start.&#x201D; Journal of Microscopy, August.</a></p>
 <p>MSSR article: <a href="https://doi.org/10.1038/s41467-022-34693-9">Torres-Garc&#xED;a, E., Pinto-C&#xE1;mara, R., Linares, A. et al. Extending resolution within a single imaging frame. Nat Commun 13, 7452 (2022).</a></p>
 <p>ESI article: <a href="https://doi.org/10.1021/acsphotonics.5b00307">Idir Yahiatene, Simon Hennig, Marcel M&#xFC;ller, Thomas Huser (2015/2016). &quot;Entropy-based Super-resolution Imaging (ESI): From Disorder to Fine Detail&quot; ACS Photonics 8, 2 (2015)</a></p>
 <p>SOFI article: <a href="https://doi.org/10.1073/pnas.0907866106">T. Dertinger, R. Colyer, G. Iyer, and J. Enderlein. Fast, background-free, 3D super-resolution optical fluctuation imaging (SOFI). PNAS 52, 106 (2009) </a></p>
-<p>SRRF article: <a href="https://link.springer.com/protocol/10.1007/978-1-0716-2051-9_14">Salsman, J.,  and, Dellaire, G., Super-Resolution Radial Fluctuations (SRRF) Microscopy, Methods in Molecular Biology 2440 (2022)</a></p>
+<p>SRRF article: <a href="https://www.nature.com/articles/ncomms12471">Gustafsson, N., Culley, S., Ashdown, G., D. M. Owen, P. Matos Pereira, and R. Henriques. Fast live-cell conventional fluorophore nanoscopy with ImageJ through super-resolution radial fluctuations. Nat Commun 7, 12471 (2016)</a></p>
 <p>MUSICAL article: <a href="https://www.nature.com/articles/ncomms13752">K. Agarwal and R. Machan, Multiple Signal Classification Algorithm for super-resolution fluorescence microscopy, Nature Communications, vol. 7, article id. 13752, (2016)</a></p>
 <p>Methods implemented:</p>
 <ul>
 <li>MSSR</li>
 <li>ESI</li>
 <li>SOFI</li>
 <li>SRRF</li>
@@ -50,17 +50,17 @@
 <tr>
 <th><strong>Super Resolution Radial Fluctuations (SRRF)</strong></th>
 <th><strong>Mean-Shift Super Resolution (MSSR)</strong></th>
 <th><strong>Entropy-based Super-resolution Imaging (ESI)</strong></th>
 </tr>
 </thead>
 <tbody><tr>
-<td><img src="docs/Fig_7_SRRF_Alva_2022.png" alt></td>
-<td><img src="docs/Fig_2a_MSSR_Garcia_2021.png" alt></td>
-<td><img src="docs/Fig_6_ESI_Alva_2022.png" alt></td>
+<td><img src="https://raw.githubusercontent.com/RoccoDAnt/napari-superres/main/docs/Fig_7_SRRF_Alva_2022.png" alt></td>
+<td><img src="https://raw.githubusercontent.com/RoccoDAnt/napari-superres/main/docs/Fig_2a_MSSR_Garcia_2021.png" alt></td>
+<td><img src="https://raw.githubusercontent.com/RoccoDAnt/napari-superres/main/docs/Fig_6_ESI_Alva_2022.png" alt></td>
 </tr>
 <tr>
 <td>from Fig. 7 of <a href="https://onlinelibrary.wiley.com/doi/10.1111/jmi.13135">Alva et al., 2022</a></td>
 <td>from Fig. 2 of <a href="https://www.biorxiv.org/content/10.1101/2021.10.17.464398v2.full">Garc&#xED;a et al., 2021</a></td>
 <td>from Fig. 6 of <a href="https://onlinelibrary.wiley.com/doi/10.1111/jmi.13135">Alva et al., 2022</a></td>
 </tr>
 </tbody></table>
@@ -76,103 +76,99 @@
 Don't miss the full getting started guide to set up your new package:
 https://github.com/napari/cookiecutter-napari-plugin#getting-started
 
 and review the napari docs for plugin developers:
 https://napari.org/stable/plugins/index.html
 -->
 
+
 <h2 id="installation">Installation</h2>
-<p>First install napari viewer:</p>
+<p>First install napari viewer (if you haven&apos;t):</p>
 <pre><code>conda create -y -n napari-env -c conda-forge python=3.9
 conda activate napari-env
 pip install &quot;napari[all]&quot;</code></pre><p>For details check: <a href="https://napari.org/stable/">https://napari.org/stable/</a></p>
-<!-- Then, you can install `napari-superres` napari plugins via [pip]:
-
-    pip install napari-superres -->
-
-
-
-<p>To install latest development version :</p>
+<p>You can install the plugin <a href="https://github.com/LIBREhub/napari-LatAm-Workshop-2023/blob/napari-superres/docs/day3/napari-superres/napari-superres_installation_guide.pdf">graphically</a>.</p>
+<p>or install latest development version :</p>
 <pre><code>pip install git+https://github.com/RoccoDAnt/napari-superres.git</code></pre><p>You might need to install <a href="https://git-scm.com/book/en/v2/Getting-Started-Installing-Git">git</a> first.</p>
 <hr>
 <p>Examples of use:</p>
 <table>
 <thead>
 <tr>
 <th><strong>Original</strong></th>
 <th><strong>tMSSR</strong></th>
 </tr>
 </thead>
 <tbody><tr>
-<td><p align="center"> <img src="docs/single-frame-good-exposure.png" width="100%" height="100%"> </p></td>
-<td><p align="center"> <img src="docs/tmssr-mean-mag2.png" width="48%" height="48%"> </p></td>
+<td><p align="center"> <img src="https://raw.githubusercontent.com/RoccoDAnt/napari-superres/main/docs/single-frame-good-exposure.png" width="100%" height="100%"> </p></td>
+<td><p align="center"> <img src="https://raw.githubusercontent.com/RoccoDAnt/napari-superres/main/docs/tmssr-mean-mag2.png" width="48%" height="48%"> </p></td>
 </tr>
 <tr>
 <td>Parameters:</td>
 <td>Amplification: 2, Order: 0, PSF FWHM: 6, <br> Interpolation: Bicubic, Statistical integration: CV*sigma</td>
 </tr>
 </tbody></table>
 <table>
 <thead>
 <tr>
 <th><strong>Original</strong></th>
 <th><strong>ESI</strong></th>
 </tr>
 </thead>
 <tbody><tr>
-<td><p align="center"> <img src="docs/synt.png" width="40%" height="40%"> </p></td>
-<td><p align="center"> <img src="docs/ESI.png" width="50%" height="50%"> </p></td>
+<td><p align="center"> <img src="https://raw.githubusercontent.com/RoccoDAnt/napari-superres/main/docs/synt.png" width="40%" height="40%"> </p></td>
+<td><p align="center"> <img src="https://raw.githubusercontent.com/RoccoDAnt/napari-superres/main/docs/ESI.png" width="50%" height="50%"> </p></td>
 </tr>
 <tr>
 <td>Parameters:</td>
 <td>image in output: 2, bins: 2, Order: 2</td>
 </tr>
 </tbody></table>
 <table>
 <thead>
 <tr>
 <th><strong>Original</strong></th>
 <th><strong>SOFI</strong></th>
 </tr>
 </thead>
 <tbody><tr>
-<td><p align="center"> <img src="docs/noSOFI.png" width="100%" height="100%"> </p></td>
-<td><p align="center"> <img src="docs/SOFI.png" width="100%" height="100%"> </p></td>
+<td><p align="center"> <img src="https://raw.githubusercontent.com/RoccoDAnt/napari-superres/main/docs/noSOFI.png" width="100%" height="100%"> </p></td>
+<td><p align="center"> <img src="https://raw.githubusercontent.com/RoccoDAnt/napari-superres/main/docs/SOFI.png" width="100%" height="100%"> </p></td>
 </tr>
 <tr>
 <td>Parameters:</td>
 <td>Amplification factor: 2, Moment Order: 4, lambda parameter: 1.5, No. Iterations: 20, Window size: 100</td>
 </tr>
 </tbody></table>
 <table>
 <thead>
 <tr>
 <th><strong>Original</strong></th>
 <th><strong>SRRF</strong></th>
 </tr>
 </thead>
 <tbody><tr>
-<td><p align="center"> <img src="docs/synt.png" width="50%" height="50%"> </p></td>
-<td><p align="center"> <img src="docs/SRRF.png" width="50%" height="50%"> </p></td>
+<td><p align="center"> <img src="https://raw.githubusercontent.com/RoccoDAnt/napari-superres/main/docs/synt.png" width="50%" height="50%"> </p></td>
+<td><p align="center"> <img src="https://raw.githubusercontent.com/RoccoDAnt/napari-superres/main/docs/SRRF.png" width="50%" height="50%"> </p></td>
 </tr>
 <tr>
 <td>Parameters:</td>
 <td>Amplification: 2, Spatial radius: 5, Symmetry Axis: 6, Start frame: 0, End frame: 48</td>
 </tr>
 </tbody></table>
 <table>
 <thead>
 <tr>
 <th><strong>Original</strong></th>
 <th><strong>MUSICAL</strong></th>
 </tr>
 </thead>
 <tbody><tr>
-<td><p align="center"> <img src="docs/musical_mean.png" width="70%" height="100%"> </p></td>
-<td><p align="center"> <img src="docs/MUSICAL-CardioMyoblast_Mitochondria.png" width="70%" height="100%"> </p></td>
+<td><p align="center"> <img src="https://raw.githubusercontent.com/RoccoDAnt/napari-superres/main/docs/musical_mean.png" width="70%" height="100%"> </p></td>
+<td><p align="center"> <img src="https://raw.githubusercontent.com/RoccoDAnt/napari-superres/main/docs/MUSICAL-CardioMyoblast_Mitochondria.png" width="70%" height="100%"> </p></td>
 </tr>
 <tr>
 <td>Parameters:</td>
 <td>Emission [nm]: 510 NA: 1.4, Mag: 100, Pizel size: 8000, Threshold: -0.5, Alpha: 4, Subpixels per pixel: 20</td>
 </tr>
 <tr>
 <td>----------------------------------</td>
```

#### html2text {}

```diff
@@ -11,16 +11,18 @@
 Extending_resolution_within_a_single_imaging_frame._Nat_Commun_13,_7452_(2022).
 ESI article: Idir_Yahiatene,_Simon_Hennig,_Marcel_M&#xFC;ller,_Thomas_Huser_
 (2015/2016)._"Entropy-based_Super-resolution_Imaging_(ESI):_From_Disorder_to
 Fine_Detail"_ACS_Photonics_8,_2_(2015)
 SOFI article: T._Dertinger,_R._Colyer,_G._Iyer,_and_J._Enderlein._Fast,
 background-free,_3D_super-resolution_optical_fluctuation_imaging_(SOFI)._PNAS
 52,_106_(2009)
-SRRF article: Salsman,_J.,_and,_Dellaire,_G.,_Super-Resolution_Radial
-Fluctuations_(SRRF)_Microscopy,_Methods_in_Molecular_Biology_2440_(2022)
+SRRF article: Gustafsson,_N.,_Culley,_S.,_Ashdown,_G.,_D._M._Owen,_P._Matos
+Pereira,_and_R._Henriques._Fast_live-cell_conventional_fluorophore_nanoscopy
+with_ImageJ_through_super-resolution_radial_fluctuations._Nat_Commun_7,_12471_
+(2016)
 MUSICAL article: K._Agarwal_and_R._Machan,_Multiple_Signal_Classification
 Algorithm_for_super-resolution_fluorescence_microscopy,_Nature_Communications,
 vol._7,_article_id._13752,_(2016)
 Methods implemented:
     * MSSR
     * ESI
     * SOFI
@@ -35,48 +37,59 @@
     * ESI GitHub repository
     * PySOFI GitHub repository
     * MUSICAL Google site
 ===============================================================================
 This napari plugin was generated with Cookiecutter using @napari's
 cookiecutter-napari-plugin template.
 ***** Installation *****
-First install napari viewer:
+First install napari viewer (if you haven't):
 conda create -y -n napari-env -c conda-forge python=3.9
 conda activate napari-env
 pip install "napari[all]"
 For details check: https://napari.org/stable/
-To install latest development version :
+You can install the plugin graphically.
+or install latest development version :
 pip install git+https://github.com/RoccoDAnt/napari-superres.git
 You might need to install git first.
 ===============================================================================
 Examples of use:
-Original                               tMSSR
-[docs/single-frame-good-exposure.png]         [docs/tmssr-mean-mag2.png]
-                                       Amplification: 2, Order: 0, PSF FWHM: 6,
-Parameters:
-                                       Interpolation: Bicubic, Statistical
-                                       integration: CV*sigma
-Original                       ESI
-       [docs/synt.png]                         [docs/ESI.png]
-Parameters:                    image in output: 2, bins: 2, Order: 2
-Original                        SOFI
-       [docs/noSOFI.png]                       [docs/SOFI.png]
-                                Amplification factor: 2, Moment Order: 4,
-Parameters:                     lambda parameter: 1.5, No. Iterations: 20,
-                                Window size: 100
-Original                       SRRF
-       [docs/synt.png]                        [docs/SRRF.png]
-Parameters:                    Amplification: 2, Spatial radius: 5, Symmetry
-                               Axis: 6, Start frame: 0, End frame: 48
-Original                             MUSICAL
-      [docs/musical_mean.png]                     [docs/MUSICAL-
-                                         CardioMyoblast_Mitochondria.png]
-                                     Emission [nm]: 510 NA: 1.4, Mag: 100,
-Parameters:                          Pizel size: 8000, Threshold: -0.5, Alpha:
-                                     4, Subpixels per pixel: 20
+Original                                tMSSR
+  [https://raw.githubusercontent.com/    [https://raw.githubusercontent.com/
+ RoccoDAnt/napari-superres/main/docs/   RoccoDAnt/napari-superres/main/docs/
+    single-frame-good-exposure.png]             tmssr-mean-mag2.png]
+                                        Amplification: 2, Order: 0, PSF FWHM:
+Parameters:                             6,
+                                        Interpolation: Bicubic, Statistical
+                                        integration: CV*sigma
+Original                              ESI
+ [https://raw.githubusercontent.com/    [https://raw.githubusercontent.com/
+RoccoDAnt/napari-superres/main/docs/   RoccoDAnt/napari-superres/main/docs/
+              synt.png]                              ESI.png]
+Parameters:                           image in output: 2, bins: 2, Order: 2
+Original                                 SOFI
+  [https://raw.githubusercontent.com/     [https://raw.githubusercontent.com/
+  RoccoDAnt/napari-superres/main/docs/    RoccoDAnt/napari-superres/main/docs/
+              noSOFI.png]                              SOFI.png]
+                                         Amplification factor: 2, Moment Order:
+Parameters:                              4, lambda parameter: 1.5, No.
+                                         Iterations: 20, Window size: 100
+Original                              SRRF
+ [https://raw.githubusercontent.com/    [https://raw.githubusercontent.com/
+RoccoDAnt/napari-superres/main/docs/   RoccoDAnt/napari-superres/main/docs/
+              synt.png]                              SRRF.png]
+                                      Amplification: 2, Spatial radius: 5,
+Parameters:                           Symmetry Axis: 6, Start frame: 0, End
+                                      frame: 48
+Original                              MUSICAL
+ [https://raw.githubusercontent.com/    [https://raw.githubusercontent.com/
+RoccoDAnt/napari-superres/main/docs/    RoccoDAnt/napari-superres/main/docs/
+          musical_mean.png]           MUSICAL-CardioMyoblast_Mitochondria.png]
+                                      Emission [nm]: 510 NA: 1.4, Mag: 100,
+Parameters:                           Pizel size: 8000, Threshold: -0.5,
+                                      Alpha: 4, Subpixels per pixel: 20
 ----------------------------------
 ***** Contributing *****
 Contributions are very welcome. Tests can be run with tox, please ensure the
 coverage at least stays the same before you submit a pull request.
 ***** License *****
 Distributed under the terms of the BSD-3 license, "napari-superres" is free and
 open source software
```

### Comparing `napari-superres-0.1.0/docs/ESI.png` & `napari-superres-0.1.1/docs/ESI.png`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/docs/ESI_Original_donuts.png` & `napari-superres-0.1.1/docs/ESI_Original_donuts.png`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/docs/ESI_Processed_nrResImage_1_nrBins_2_esi_order_1_donuts.png` & `napari-superres-0.1.1/docs/ESI_Processed_nrResImage_1_nrBins_2_esi_order_1_donuts.png`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/docs/Fig_2a_MSSR_Garcia_2021.png` & `napari-superres-0.1.1/docs/Fig_2a_MSSR_Garcia_2021.png`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/docs/Fig_6_ESI_Alva_2022.png` & `napari-superres-0.1.1/docs/Fig_6_ESI_Alva_2022.png`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/docs/Fig_7_SRRF_Alva_2022.png` & `napari-superres-0.1.1/docs/Fig_7_SRRF_Alva_2022.png`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/docs/MSSR.png` & `napari-superres-0.1.1/docs/MSSR.png`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/docs/MSSR_Processed_amp_2_PSFp_1_order_1_raw7_100_donuts.png` & `napari-superres-0.1.1/docs/MSSR_Processed_amp_2_PSFp_1_order_1_raw7_100_donuts.png`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/docs/MSSR_original_donuts.png` & `napari-superres-0.1.1/docs/MSSR_original_donuts.png`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/docs/MUSICAL-CardioMyoblast_Mitochondria.png` & `napari-superres-0.1.1/docs/MUSICAL-CardioMyoblast_Mitochondria.png`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/docs/SOFI.png` & `napari-superres-0.1.1/docs/SOFI.png`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/docs/SRRF.png` & `napari-superres-0.1.1/docs/SRRF.png`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/docs/SRRF_Original_Microtubules.png` & `napari-superres-0.1.1/docs/SRRF_Original_Microtubules.png`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/docs/SRRF_processed_mag_2_rad_3_symAxis_3_fstart_0_fend_3_Microtubules.png` & `napari-superres-0.1.1/docs/SRRF_processed_mag_2_rad_3_symAxis_3_fstart_0_fend_3_Microtubules.png`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/docs/TMSSR.png` & `napari-superres-0.1.1/docs/TMSSR.png`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/docs/musical_mean.png` & `napari-superres-0.1.1/docs/musical_mean.png`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/docs/noMSSR.png` & `napari-superres-0.1.1/docs/noMSSR.png`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/docs/noSOFI.png` & `napari-superres-0.1.1/docs/noSOFI.png`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/docs/single-frame-good-exposure.png` & `napari-superres-0.1.1/docs/single-frame-good-exposure.png`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/docs/single-frame-good-exposure.tif` & `napari-superres-0.1.1/docs/single-frame-good-exposure.tif`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/docs/synt.png` & `napari-superres-0.1.1/docs/synt.png`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/docs/tmssr-mean-mag2.png` & `napari-superres-0.1.1/docs/tmssr-mean-mag2.png`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/setup.cfg` & `napari-superres-0.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,124 +1,121 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6170 6172 692d 7375 7065 7272   = napari-superr
 00000020: 6573 0d0a 7665 7273 696f 6e20 3d20 302e  es..version = 0.
-00000030: 312e 300d 0a64 6573 6372 6970 7469 6f6e  1.0..description
+00000030: 312e 310d 0a64 6573 6372 6970 7469 6f6e  1.1..description
 00000040: 203d 2046 6c75 6f72 6573 6365 6e63 6520   = Fluorescence 
 00000050: 466c 7563 7475 6174 696f 6e2d 6261 7365  Fluctuation-base
 00000060: 6420 5375 7065 7220 5265 736f 6c75 7469  d Super Resoluti
 00000070: 6f6e 2028 4646 2d53 524d 2920 4d65 7468  on (FF-SRM) Meth
 00000080: 6f64 730d 0a6c 6f6e 675f 6465 7363 7269  ods..long_descri
 00000090: 7074 696f 6e20 3d20 6669 6c65 3a20 5245  ption = file: RE
 000000a0: 4144 4d45 2e6d 640d 0a6c 6f6e 675f 6465  ADME.md..long_de
 000000b0: 7363 7269 7074 696f 6e5f 636f 6e74 656e  scription_conten
 000000c0: 745f 7479 7065 203d 2074 6578 742f 6d61  t_type = text/ma
 000000d0: 726b 646f 776e 0d0a 7572 6c20 3d20 6874  rkdown..url = ht
 000000e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 000000f0: 2f52 6f63 636f 4441 6e74 2f6e 6170 6172  /RoccoDAnt/napar
 00000100: 692d 7375 7065 7272 6573 0d0a 6175 7468  i-superres..auth
 00000110: 6f72 203d 2022 526f 6363 6f20 4427 416e  or = "Rocco D'An
-00000120: 7475 6f6e 6f20 3c72 6f63 636f 2e64 616e  tuono <rocco.dan
-00000130: 7475 6f6e 6f40 686f 746d 6169 6c2e 6974  tuono@hotmail.it
-00000140: 3e2c 2041 64c3 a16e 2047 7565 7272 6572  >, Ad..n Guerrer
-00000150: 6f2c 2052 61c3 ba6c 2050 696e 746f 2043  o, Ra..l Pinto C
-00000160: c3a1 6d61 7261 2c20 5061 c3ba 6c20 4865  ..mara, Pa..l He
-00000170: 726e c3a1 6e64 657a 2048 6572 7265 7261  rn..ndez Herrera
-00000180: 2c20 4573 6c65 7920 546f 7272 6573 2047  , Esley Torres G
-00000190: 6172 6369 612c 2048 6179 6465 6520 4865  arcia, Haydee He
-000001a0: 726e c3a1 6e64 657a 2c20 4a75 6c69 c3a1  rn..ndez, Juli..
-000001b0: 6e20 4d65 6ac3 ad61 203c 6a75 6c69 616e  n Mej..a <julian
-000001c0: 2e6d 656a 6961 4069 6274 2e75 6e61 6d2e  .mejia@ibt.unam.
-000001d0: 6d78 3e22 0d0a 6175 7468 6f72 5f65 6d61  mx>"..author_ema
-000001e0: 696c 203d 2072 6f63 636f 2e64 616e 7475  il = rocco.dantu
-000001f0: 6f6e 6f40 686f 746d 6169 6c2e 6974 0d0a  ono@hotmail.it..
-00000200: 6c69 6365 6e73 6520 3d20 4253 442d 332d  license = BSD-3-
-00000210: 436c 6175 7365 0d0a 6c69 6365 6e73 655f  Clause..license_
-00000220: 6669 6c65 7320 3d20 4c49 4345 4e53 450d  files = LICENSE.
-00000230: 0a63 6c61 7373 6966 6965 7273 203d 200d  .classifiers = .
-00000240: 0a09 4465 7665 6c6f 706d 656e 7420 5374  ..Development St
-00000250: 6174 7573 203a 3a20 3220 2d20 5072 652d  atus :: 2 - Pre-
-00000260: 416c 7068 610d 0a09 4672 616d 6577 6f72  Alpha...Framewor
-00000270: 6b20 3a3a 206e 6170 6172 690d 0a09 496e  k :: napari...In
-00000280: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
-00000290: 3a3a 2044 6576 656c 6f70 6572 730d 0a09  :: Developers...
-000002a0: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
-000002b0: 7070 726f 7665 6420 3a3a 2042 5344 204c  pproved :: BSD L
-000002c0: 6963 656e 7365 0d0a 094f 7065 7261 7469  icense...Operati
-000002d0: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
-000002e0: 496e 6465 7065 6e64 656e 740d 0a09 5072  Independent...Pr
-000002f0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000300: 6765 203a 3a20 5079 7468 6f6e 0d0a 0950  ge :: Python...P
-00000310: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000320: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000330: 2033 0d0a 0950 726f 6772 616d 6d69 6e67   3...Programming
-00000340: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000350: 686f 6e20 3a3a 2033 203a 3a20 4f6e 6c79  hon :: 3 :: Only
-00000360: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-00000370: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000380: 6e20 3a3a 2033 2e38 0d0a 0950 726f 6772  n :: 3.8...Progr
-00000390: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000003a0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e39  :: Python :: 3.9
-000003b0: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-000003c0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000003d0: 6e20 3a3a 2033 2e31 300d 0a09 546f 7069  n :: 3.10...Topi
-000003e0: 6320 3a3a 2053 6369 656e 7469 6669 632f  c :: Scientific/
-000003f0: 456e 6769 6e65 6572 696e 6720 3a3a 2049  Engineering :: I
-00000400: 6d61 6765 2050 726f 6365 7373 696e 670d  mage Processing.
-00000410: 0a70 726f 6a65 6374 5f75 726c 7320 3d20  .project_urls = 
-00000420: 0d0a 0942 7567 2054 7261 636b 6572 203d  ...Bug Tracker =
-00000430: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000440: 636f 6d2f 526f 6363 6f44 416e 742f 6e61  com/RoccoDAnt/na
-00000450: 7061 7269 2d73 7570 6572 7265 732f 6973  pari-superres/is
-00000460: 7375 6573 0d0a 0944 6f63 756d 656e 7461  sues...Documenta
-00000470: 7469 6f6e 203d 2068 7474 7073 3a2f 2f67  tion = https://g
-00000480: 6974 6875 622e 636f 6d2f 526f 6363 6f44  ithub.com/RoccoD
-00000490: 416e 742f 6e61 7061 7269 2d73 7570 6572  Ant/napari-super
-000004a0: 7265 7323 5245 4144 4d45 2e6d 640d 0a09  res#README.md...
-000004b0: 536f 7572 6365 2043 6f64 6520 3d20 6874  Source Code = ht
-000004c0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000004d0: 2f52 6f63 636f 4441 6e74 2f6e 6170 6172  /RoccoDAnt/napar
-000004e0: 692d 7375 7065 7272 6573 0d0a 0955 7365  i-superres...Use
-000004f0: 7220 5375 7070 6f72 7420 3d20 6874 7470  r Support = http
-00000500: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f52  s://github.com/R
-00000510: 6f63 636f 4441 6e74 2f6e 6170 6172 692d  occoDAnt/napari-
-00000520: 7375 7065 7272 6573 2f69 7373 7565 730d  superres/issues.
-00000530: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 7061  ...[options]..pa
-00000540: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
-00000550: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
-00000560: 203d 200d 0a09 6d61 7470 6c6f 746c 6962   = ...matplotlib
-00000570: 0d0a 096d 6167 6963 6775 690d 0a09 7174  ...magicgui...qt
-00000580: 7079 0d0a 7079 7468 6f6e 5f72 6571 7569  py..python_requi
-00000590: 7265 7320 3d20 3e3d 332e 380d 0a69 6e63  res = >=3.8..inc
-000005a0: 6c75 6465 5f70 6163 6b61 6765 5f64 6174  lude_package_dat
-000005b0: 6120 3d20 5472 7565 0d0a 7061 636b 6167  a = True..packag
-000005c0: 655f 6469 7220 3d20 0d0a 093d 7372 630d  e_dir = ...=src.
-000005d0: 0a73 6574 7570 5f72 6571 7569 7265 7320  .setup_requires 
-000005e0: 3d20 7365 7475 7074 6f6f 6c73 5f73 636d  = setuptools_scm
-000005f0: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
-00000600: 6b61 6765 732e 6669 6e64 5d0d 0a77 6865  kages.find]..whe
-00000610: 7265 203d 2073 7263 0d0a 0d0a 5b6f 7074  re = src....[opt
-00000620: 696f 6e73 2e65 6e74 7279 5f70 6f69 6e74  ions.entry_point
-00000630: 735d 0d0a 6e61 7061 7269 2e6d 616e 6966  s]..napari.manif
-00000640: 6573 7420 3d20 0d0a 096e 6170 6172 692d  est = ...napari-
-00000650: 7375 7065 7272 6573 203d 206e 6170 6172  superres = napar
-00000660: 695f 7375 7065 7272 6573 3a6e 6170 6172  i_superres:napar
-00000670: 692e 7961 6d6c 0d0a 0d0a 5b6f 7074 696f  i.yaml....[optio
-00000680: 6e73 2e65 7874 7261 735f 7265 7175 6972  ns.extras_requir
-00000690: 655d 0d0a 7465 7374 696e 6720 3d20 0d0a  e]..testing = ..
-000006a0: 0974 6f78 0d0a 0970 7974 6573 7420 2023  .tox...pytest  #
-000006b0: 2068 7474 7073 3a2f 2f64 6f63 732e 7079   https://docs.py
-000006c0: 7465 7374 2e6f 7267 2f65 6e2f 6c61 7465  test.org/en/late
-000006d0: 7374 2f63 6f6e 7465 6e74 732e 6874 6d6c  st/contents.html
-000006e0: 0d0a 0970 7974 6573 742d 636f 7620 2023  ...pytest-cov  #
-000006f0: 2068 7474 7073 3a2f 2f70 7974 6573 742d   https://pytest-
-00000700: 636f 762e 7265 6164 7468 6564 6f63 732e  cov.readthedocs.
-00000710: 696f 2f65 6e2f 6c61 7465 7374 2f0d 0a09  io/en/latest/...
-00000720: 7079 7465 7374 2d71 7420 2023 2068 7474  pytest-qt  # htt
-00000730: 7073 3a2f 2f70 7974 6573 742d 7174 2e72  ps://pytest-qt.r
-00000740: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00000750: 2f6c 6174 6573 742f 0d0a 096e 6170 6172  /latest/...napar
-00000760: 690d 0a09 7079 7174 350d 0a0d 0a5b 6f70  i...pyqt5....[op
-00000770: 7469 6f6e 732e 7061 636b 6167 655f 6461  tions.package_da
-00000780: 7461 5d0d 0a2a 203d 202a 2e79 616d 6c0d  ta]..* = *.yaml.
-00000790: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
-000007a0: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
-000007b0: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
+00000120: 7475 6f6e 6f2c 2041 64c3 a16e 2047 7565  tuono, Ad..n Gue
+00000130: 7272 6572 6f2c 2052 61c3 ba6c 2050 696e  rrero, Ra..l Pin
+00000140: 746f 2043 c3a1 6d61 7261 2c20 5061 c3ba  to C..mara, Pa..
+00000150: 6c20 4865 726e c3a1 6e64 657a 2048 6572  l Hern..ndez Her
+00000160: 7265 7261 2c20 4573 6c65 7920 546f 7272  rera, Esley Torr
+00000170: 6573 2047 6172 6369 612c 2048 6179 6465  es Garcia, Hayde
+00000180: 6520 4865 726e c3a1 6e64 657a 2c20 4a75  e Hern..ndez, Ju
+00000190: 6c69 c3a1 6e20 4d65 6ac3 ad61 220d 0a61  li..n Mej..a"..a
+000001a0: 7574 686f 725f 656d 6169 6c20 3d20 726f  uthor_email = ro
+000001b0: 6363 6f2e 6461 6e74 756f 6e6f 4068 6f74  cco.dantuono@hot
+000001c0: 6d61 696c 2e69 740d 0a6c 6963 656e 7365  mail.it..license
+000001d0: 203d 2042 5344 2d33 2d43 6c61 7573 650d   = BSD-3-Clause.
+000001e0: 0a6c 6963 656e 7365 5f66 696c 6573 203d  .license_files =
+000001f0: 204c 4943 454e 5345 0d0a 636c 6173 7369   LICENSE..classi
+00000200: 6669 6572 7320 3d20 0d0a 0944 6576 656c  fiers = ...Devel
+00000210: 6f70 6d65 6e74 2053 7461 7475 7320 3a3a  opment Status ::
+00000220: 2032 202d 2050 7265 2d41 6c70 6861 0d0a   2 - Pre-Alpha..
+00000230: 0946 7261 6d65 776f 726b 203a 3a20 6e61  .Framework :: na
+00000240: 7061 7269 0d0a 0949 6e74 656e 6465 6420  pari...Intended 
+00000250: 4175 6469 656e 6365 203a 3a20 4465 7665  Audience :: Deve
+00000260: 6c6f 7065 7273 0d0a 094c 6963 656e 7365  lopers...License
+00000270: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
+00000280: 203a 3a20 4253 4420 4c69 6365 6e73 650d   :: BSD License.
+00000290: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
+000002a0: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
+000002b0: 6465 6e74 0d0a 0950 726f 6772 616d 6d69  dent...Programmi
+000002c0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000002d0: 7974 686f 6e0d 0a09 5072 6f67 7261 6d6d  ython...Programm
+000002e0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000002f0: 5079 7468 6f6e 203a 3a20 330d 0a09 5072  Python :: 3...Pr
+00000300: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000310: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000320: 3320 3a3a 204f 6e6c 790d 0a09 5072 6f67  3 :: Only...Prog
+00000330: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000340: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000350: 380d 0a09 5072 6f67 7261 6d6d 696e 6720  8...Programming 
+00000360: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000370: 6f6e 203a 3a20 332e 390d 0a09 5072 6f67  on :: 3.9...Prog
+00000380: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000390: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+000003a0: 3130 0d0a 0954 6f70 6963 203a 3a20 5363  10...Topic :: Sc
+000003b0: 6965 6e74 6966 6963 2f45 6e67 696e 6565  ientific/Enginee
+000003c0: 7269 6e67 203a 3a20 496d 6167 6520 5072  ring :: Image Pr
+000003d0: 6f63 6573 7369 6e67 0d0a 7072 6f6a 6563  ocessing..projec
+000003e0: 745f 7572 6c73 203d 200d 0a09 4275 6720  t_urls = ...Bug 
+000003f0: 5472 6163 6b65 7220 3d20 6874 7470 733a  Tracker = https:
+00000400: 2f2f 6769 7468 7562 2e63 6f6d 2f52 6f63  //github.com/Roc
+00000410: 636f 4441 6e74 2f6e 6170 6172 692d 7375  coDAnt/napari-su
+00000420: 7065 7272 6573 2f69 7373 7565 730d 0a09  perres/issues...
+00000430: 446f 6375 6d65 6e74 6174 696f 6e20 3d20  Documentation = 
+00000440: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000450: 6f6d 2f52 6f63 636f 4441 6e74 2f6e 6170  om/RoccoDAnt/nap
+00000460: 6172 692d 7375 7065 7272 6573 2352 4541  ari-superres#REA
+00000470: 444d 452e 6d64 0d0a 0953 6f75 7263 6520  DME.md...Source 
+00000480: 436f 6465 203d 2068 7474 7073 3a2f 2f67  Code = https://g
+00000490: 6974 6875 622e 636f 6d2f 526f 6363 6f44  ithub.com/RoccoD
+000004a0: 416e 742f 6e61 7061 7269 2d73 7570 6572  Ant/napari-super
+000004b0: 7265 730d 0a09 5573 6572 2053 7570 706f  res...User Suppo
+000004c0: 7274 203d 2068 7474 7073 3a2f 2f67 6974  rt = https://git
+000004d0: 6875 622e 636f 6d2f 526f 6363 6f44 416e  hub.com/RoccoDAn
+000004e0: 742f 6e61 7061 7269 2d73 7570 6572 7265  t/napari-superre
+000004f0: 732f 6973 7375 6573 0d0a 0d0a 5b6f 7074  s/issues....[opt
+00000500: 696f 6e73 5d0d 0a70 6163 6b61 6765 7320  ions]..packages 
+00000510: 3d20 6669 6e64 3a0d 0a69 6e73 7461 6c6c  = find:..install
+00000520: 5f72 6571 7569 7265 7320 3d20 0d0a 096d  _requires = ...m
+00000530: 6174 706c 6f74 6c69 620d 0a09 6d61 6769  atplotlib...magi
+00000540: 6367 7569 0d0a 0971 7470 790d 0a70 7974  cgui...qtpy..pyt
+00000550: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
+00000560: 3d33 2e38 0d0a 696e 636c 7564 655f 7061  =3.8..include_pa
+00000570: 636b 6167 655f 6461 7461 203d 2054 7275  ckage_data = Tru
+00000580: 650d 0a70 6163 6b61 6765 5f64 6972 203d  e..package_dir =
+00000590: 200d 0a09 3d73 7263 0d0a 7365 7475 705f   ...=src..setup_
+000005a0: 7265 7175 6972 6573 203d 2073 6574 7570  requires = setup
+000005b0: 746f 6f6c 735f 7363 6d0d 0a0d 0a5b 6f70  tools_scm....[op
+000005c0: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
+000005d0: 696e 645d 0d0a 7768 6572 6520 3d20 7372  ind]..where = sr
+000005e0: 630d 0a0d 0a5b 6f70 7469 6f6e 732e 656e  c....[options.en
+000005f0: 7472 795f 706f 696e 7473 5d0d 0a6e 6170  try_points]..nap
+00000600: 6172 692e 6d61 6e69 6665 7374 203d 200d  ari.manifest = .
+00000610: 0a09 6e61 7061 7269 2d73 7570 6572 7265  ..napari-superre
+00000620: 7320 3d20 6e61 7061 7269 5f73 7570 6572  s = napari_super
+00000630: 7265 733a 6e61 7061 7269 2e79 616d 6c0d  res:napari.yaml.
+00000640: 0a0d 0a5b 6f70 7469 6f6e 732e 6578 7472  ...[options.extr
+00000650: 6173 5f72 6571 7569 7265 5d0d 0a74 6573  as_require]..tes
+00000660: 7469 6e67 203d 200d 0a09 746f 780d 0a09  ting = ...tox...
+00000670: 7079 7465 7374 2020 2320 6874 7470 733a  pytest  # https:
+00000680: 2f2f 646f 6373 2e70 7974 6573 742e 6f72  //docs.pytest.or
+00000690: 672f 656e 2f6c 6174 6573 742f 636f 6e74  g/en/latest/cont
+000006a0: 656e 7473 2e68 746d 6c0d 0a09 7079 7465  ents.html...pyte
+000006b0: 7374 2d63 6f76 2020 2320 6874 7470 733a  st-cov  # https:
+000006c0: 2f2f 7079 7465 7374 2d63 6f76 2e72 6561  //pytest-cov.rea
+000006d0: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+000006e0: 6174 6573 742f 0d0a 0970 7974 6573 742d  atest/...pytest-
+000006f0: 7174 2020 2320 6874 7470 733a 2f2f 7079  qt  # https://py
+00000700: 7465 7374 2d71 742e 7265 6164 7468 6564  test-qt.readthed
+00000710: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00000720: 2f0d 0a09 6e61 7061 7269 0d0a 0970 7971  /...napari...pyq
+00000730: 7435 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  t5....[options.p
+00000740: 6163 6b61 6765 5f64 6174 615d 0d0a 2a20  ackage_data]..* 
+00000750: 3d20 2a2e 7961 6d6c 0d0a 0d0a 5b65 6767  = *.yaml....[egg
+00000760: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
+00000770: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
+00000780: 2030 0d0a 0d0a                            0....
```

### Comparing `napari-superres-0.1.0/src/napari_superres/__init__.py` & `napari-superres-0.1.1/src/napari_superres/__init__.py`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/src/napari_superres/_gui_creator.py` & `napari-superres-0.1.1/src/napari_superres/_gui_creator.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,14 +113,23 @@
         self.spinBoxS.setMinimum(1)
         self.spinBoxS.setMaximum(3)
         self.spinBoxS.setHidden(True)
 
         btnB = QPushButton("Batch Analysis")
         btnB.clicked.connect(self.batch)
 
+        self.label_chanels = QLabel()
+        self.label_chanels.setText("Select channel")
+        self.spinBox5 = QSpinBox()
+        self.spinBox5.setMinimum(0)
+        self.spinBox5.setMaximum(2)
+        self.spinBox5.setValue(0)
+        self.label_chanels.setHidden(True)
+        self.spinBox5.setHidden(True)
+
         btnG = QPushButton("Run")
         myFont=QtGui.QFont()
         myFont.setBold(True)
         btnG.setFont(myFont)
         btnG.clicked.connect(self._run)
 
 #Adding the items to the QBoxLayout (vertical configuration)
@@ -143,14 +152,16 @@
         self.layout().addWidget(self.CheckBox5)
         self.layout().addSpacing(30)
         self.layout().addWidget(self.labelT)
         self.layout().addWidget(self.ComboBoxT)
         self.layout().addWidget(self.spinBoxS)
         self.layout().addSpacing(20)
         self.layout().addWidget(btnB)
+        self.layout().addWidget(self.label_chanels)
+        self.layout().addWidget(self.spinBox5)
         self.layout().addSpacing(30)
         self.layout().addWidget(btnG)
 
 #Rest of methods of the mssr_caller class
     def setTemp(self,d):
         if d == True:
             self.labelT.setHidden(False)
@@ -213,24 +224,28 @@
         #print(f'kcMax : {kcMax:.3f}, A0 : {A0[0]:.3f}')
         #print(f'Resolution: {2/kcMax:.3f}, [pixels]')
         self.DoubleSpinBox1.setValue(res)
         self.msg.close()
 
 
     def batch(self):
+        self.label_chanels.setHidden(False)
+        self.spinBox5.setHidden(False)
         self.flagBatch = True
         self.my_files, other_data = QFileDialog.getOpenFileNames(self, "Select Files")
         first = self.my_files[0].split("/")
         first.pop()
         my_dir = "/".join(first)
-        self.results_dir = my_dir+"/MSSR_resuslts"
+        self.results_dir = my_dir+"/MSSR_results"
 
 
     def _run(self):
-        if str(self.viewer.layers.selection.active) == 'None' and self.flagBatch == True:
+        #This section is for the batch analysis
+        #if str(self.viewer.layers.selection.active) == 'None' and self.flagBatch == True:
+        if self.flagBatch == True:
             self.flagBatch = False
             fwhm = self.DoubleSpinBox1.value()
             amp = self.spinBox1.value()
             order = self.spinBox3.value()
 
             if self.CheckBox1.checkState() == 0:
                 mesh = False
@@ -247,71 +262,104 @@
             if self.CheckBox5.checkState() == 0:
                 tempAn = False
             else:
                 tempAn = True
 
             if tempAn == False:
                 os.mkdir(self.results_dir)
+                napari.utils.notifications.show_info("MSSR_results file created")
                 for el in self.my_files:
                     try:
                         img = io.imread(el)
                     except:
                         continue
                     if len(img.shape) == 2:
                         processed_img = my_mssr.sfMSSR(img, fwhm, amp, order, mesh, ftI, intNorm)
                         io.imsave(self.results_dir+"/"+"MSSR "+el.split("/").pop(),processed_img)
+
                     elif len(img.shape) == 3:
                         processed_img = my_mssr.tMSSR(img, fwhm, amp, order, mesh, ftI, intNorm)
                         io.imsave(self.results_dir+"/"+"MSSR "+el.split("/").pop(),processed_img)
+
+                    elif len(img.shape) == 4:
+                        channel_val = self.spinBox5.value()
+                        sch_im = img[:,:,:,channel_val]
+                        processed_img = my_mssr.tMSSR(sch_im, fwhm, amp, order, mesh, ftI, intNorm)
+                        io.imsave(self.results_dir+"/"+"MSSR "+ "ch_" + str(channel_val) + "_" + el.split("/").pop(),processed_img)
             else:
                 first = self.results_dir.split("/")
                 first.pop()
                 my_dir = "/".join(first)
-                if  first[-1] == "MSSR_resuslts":
-                    tempAn_dir = my_dir + "/tMSSR_resuslts"
+                if  first[-1] == "MSSR_results":
+                    tempAn_dir = my_dir + "/tMSSR_results"
                     if os.path.exists(tempAn_dir) == False:
                         os.mkdir(tempAn_dir)
+                        napari.utils.notifications.show_info("tMSSR_results file created")
+                    else:
+                        napari.utils.notifications.show_info("adding processed images to tMSSR_results")
+
 
                     for el in self.my_files:
                         try:
                             img = io.imread(el)
                         except:
                             continue
                         if len(img.shape) == 3:
                             temp_procesed, staMeth = self.call_statistical_int_batch(img)
                             el_name = el.split("/")[-1].split(".")[0]
                             el_format = el.split(".")[-1]
                             io.imsave(tempAn_dir+"/"+"t"+ el_name + " " + staMeth + "." + el_format,temp_procesed)
 
                 else:
                     os.mkdir(self.results_dir)
+                    napari.utils.notifications.show_info("MSSR_results file created")
                     for el in self.my_files:
                         try:
                             img = io.imread(el)
                         except:
                             continue
                         if len(img.shape) == 2:
                             processed_img = my_mssr.sfMSSR(img, fwhm, amp, order, mesh, ftI, intNorm)
                             io.imsave(self.results_dir+"/"+"MSSR "+el.split("/").pop(),processed_img)
+
                         elif len(img.shape) == 3:
-                            tempAn_dir = self.results_dir + "/tMSSR_resuslts"
+                            tempAn_dir = self.results_dir + "/tMSSR_results"
                             if os.path.exists(tempAn_dir) == False:
                                 os.mkdir(tempAn_dir)
+                                napari.utils.notifications.show_info("tMSSR_results file created")
+
                             processed_img = my_mssr.tMSSR(img, fwhm, amp, order, mesh, ftI, intNorm)
                             io.imsave(self.results_dir+"/"+"MSSR "+el.split("/").pop(),processed_img)
                             temp_procesed, staMeth = self.call_statistical_int_batch(processed_img)
                             el_name = el.split("/").pop().split(".")[0]
                             el_format = el.split("/").pop().split(".")[-1]
                             io.imsave(tempAn_dir+"/"+"tMSSR "+ el_name + " " + staMeth + "." + el_format,temp_procesed)
 
+                        elif len(img.shape) == 4:
+                            tempAn_dir = self.results_dir + "/tMSSR_results"
+                            if os.path.exists(tempAn_dir) == False:
+                                os.mkdir(tempAn_dir)
+                                napari.utils.notifications.show_info("tMSSR_results file created")
+                                
+                            channel_val = self.spinBox5.value()
+                            sch_im = img[:,:,:,channel_val]
+                            processed_img = my_mssr.tMSSR(sch_im, fwhm, amp, order, mesh, ftI, intNorm)
+                            io.imsave(self.results_dir+"/"+"MSSR "+ "ch_" + str(channel_val) + "_" + el.split("/").pop(),processed_img)
+                            temp_procesed, staMeth = self.call_statistical_int_batch(processed_img)
+                            el_name = el.split("/").pop().split(".")[0]
+                            el_format = el.split("/").pop().split(".")[-1]
+                            io.imsave(tempAn_dir+"/"+"tMSSR "+ el_name + " " + staMeth + "." + el_format,temp_procesed)
+
+
 
 
         elif self.viewer.layers.selection.active.rgb == True:
             raise TypeError("Only single channel images are allowed")
 
+        #Here goes the viewer image analysis
         else:
             self.selected_im_name = str(self.viewer.layers.selection.active)
             img = self.viewer.layers[self.selected_im_name].data
 
             fwhm = self.DoubleSpinBox1.value()
             amp = self.spinBox1.value()
             order = self.spinBox3.value()
@@ -351,14 +399,18 @@
                 else:
                     processed_img = my_mssr.tMSSR(img, fwhm, amp, order, mesh, ftI, intNorm)
                     self.track_name = "MSSR "+self.selected_im_name
                     self.viewer.add_image(processed_img, name= self.track_name)
                     self.call_statistical_int(processed_img)
                     self.flag = True
 
+        #removing the channels selction from the batch analysis option
+        self.label_chanels.setHidden(True)
+        self.spinBox5.setHidden(True)
+
         napari.utils.notifications.show_info("Process complete")
 
 
 
 
     def call_statistical_int(self,processed_img):
         staMeth = self.ComboBoxT.currentText()
@@ -701,15 +753,15 @@
         label2.setText("Spatial radius")
         self.spinBox2 = QSpinBox()
         self.spinBox2.setMinimum(1)
         self.spinBox2.setMaximum(10)
         self.spinBox2.setValue(5)
 
         label3 = QLabel()
-        label3.setText("Symmetry Axis")
+        label3.setText("Symetry Axis")
         self.spinBox3 = QSpinBox()
         self.spinBox3.setMinimum(1)
         self.spinBox3.setMaximum(10)
         self.spinBox3.setValue(6)
 
         label4 = QLabel()
         label4.setText("Start frame")
```

### Comparing `napari-superres-0.1.0/src/napari_superres/_reader.py` & `napari-superres-0.1.1/src/napari_superres/_reader.py`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/src/napari_superres/_tests/test_reader.py` & `napari-superres-0.1.1/src/napari_superres/_tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/src/napari_superres/_tests/test_widget.py` & `napari-superres-0.1.1/src/napari_superres/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/src/napari_superres/_writer.py` & `napari-superres-0.1.1/src/napari_superres/_writer.py`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/src/napari_superres/core_decor.py` & `napari-superres-0.1.1/src/napari_superres/core_decor.py`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/src/napari_superres/core_esi.py` & `napari-superres-0.1.1/src/napari_superres/core_esi.py`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/src/napari_superres/core_mssr.py` & `napari-superres-0.1.1/src/napari_superres/core_mssr.py`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/src/napari_superres/core_mssr_numba.py` & `napari-superres-0.1.1/src/napari_superres/core_mssr_numba.py`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/src/napari_superres/core_musical.py` & `napari-superres-0.1.1/src/napari_superres/core_musical.py`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/src/napari_superres/core_sofi.py` & `napari-superres-0.1.1/src/napari_superres/core_sofi.py`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/src/napari_superres/core_srrf.py` & `napari-superres-0.1.1/src/napari_superres/core_srrf.py`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/src/napari_superres/deconvsk.py` & `napari-superres-0.1.1/src/napari_superres/deconvsk.py`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/src/napari_superres/finterp.py` & `napari-superres-0.1.1/src/napari_superres/finterp.py`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/src/napari_superres/my_popW.py` & `napari-superres-0.1.1/src/napari_superres/my_popW.py`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/src/napari_superres/napari.yaml` & `napari-superres-0.1.1/src/napari_superres/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-superres-0.1.0/src/napari_superres.egg-info/SOURCES.txt` & `napari-superres-0.1.1/src/napari_superres.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 README.html
 README.md
 mkdocs.yml
 setup.cfg
 setup.py
 tox.ini
 .github/workflows/test_and_deploy.yml
+.napari/DESCRIPTION.html
 .napari/DESCRIPTION.md
 docs/ESI.png
 docs/ESI_Original_donuts.png
 docs/ESI_Processed_nrResImage_1_nrBins_2_esi_order_1_donuts.png
 docs/Fig_2a_MSSR_Garcia_2021.png
 docs/Fig_6_ESI_Alva_2022.png
 docs/Fig_7_SRRF_Alva_2022.png
```

### Comparing `napari-superres-0.1.0/tox.ini` & `napari-superres-0.1.1/tox.ini`

 * *Files identical despite different names*

