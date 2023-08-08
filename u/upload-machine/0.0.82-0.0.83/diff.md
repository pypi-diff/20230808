# Comparing `tmp/upload_machine-0.0.82.tar.gz` & `tmp/upload_machine-0.0.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upload_machine-0.0.82.tar", last modified: Sun Aug  6 10:23:42 2023, max compression
+gzip compressed data, was "upload_machine-0.0.83.tar", last modified: Tue Aug  8 19:04:09 2023, max compression
```

## Comparing `upload_machine-0.0.82.tar` & `upload_machine-0.0.83.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 10:23:42.330377 upload_machine-0.0.82/
--rwx------   0 moyu       (501) staff       (20)     1063 2022-10-06 05:53:46.000000 upload_machine-0.0.82/LICENSE
--rwx------   0 moyu       (501) staff       (20)       37 2022-10-06 08:50:43.000000 upload_machine-0.0.82/MANIFEST.in
--rw-r--r--   0 moyu       (501) staff       (20)    14608 2023-08-06 10:23:42.329207 upload_machine-0.0.82/PKG-INFO
--rwxr-xr-x   0 moyu       (501) staff       (20)    14206 2023-08-06 07:01:29.000000 upload_machine-0.0.82/README.md
--rw-r--r--   0 moyu       (501) staff       (20)       38 2023-08-06 10:23:42.330612 upload_machine-0.0.82/setup.cfg
--rwx------   0 moyu       (501) staff       (20)     1110 2023-08-06 10:23:32.000000 upload_machine-0.0.82/setup.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 10:23:42.264490 upload_machine-0.0.82/upload_machine/
--rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.82/upload_machine/__init__.py
--rwx------   0 moyu       (501) staff       (20)      241 2022-10-06 08:12:01.000000 upload_machine-0.0.82/upload_machine/basicinfo.yaml
--rwx------   0 moyu       (501) staff       (20)     2622 2023-01-02 14:54:11.000000 upload_machine-0.0.82/upload_machine/main.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 10:23:42.271133 upload_machine-0.0.82/upload_machine/utils/
--rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.82/upload_machine/utils/__init__.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 10:23:42.272498 upload_machine-0.0.82/upload_machine/utils/edittorrent/
--rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.82/upload_machine/utils/edittorrent/__init__.py
--rwx------   0 moyu       (501) staff       (20)     3966 2022-10-06 05:53:46.000000 upload_machine-0.0.82/upload_machine/utils/edittorrent/edittorrent.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 10:23:42.282620 upload_machine-0.0.82/upload_machine/utils/img_upload/
--rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.82/upload_machine/utils/img_upload/__init__.py
--rwx------   0 moyu       (501) staff       (20)     7231 2022-10-06 05:53:46.000000 upload_machine-0.0.82/upload_machine/utils/img_upload/chevereto.py
--rwx------   0 moyu       (501) staff       (20)     2674 2022-10-06 05:53:46.000000 upload_machine-0.0.82/upload_machine/utils/img_upload/fapping_emp.py
--rwx------   0 moyu       (501) staff       (20)     4521 2022-10-06 05:53:46.000000 upload_machine-0.0.82/upload_machine/utils/img_upload/imgbox.py
--rwxr-xr-x   0 moyu       (501) staff       (20)     9014 2023-01-20 04:03:37.000000 upload_machine-0.0.82/upload_machine/utils/img_upload/imgupload.py
--rwx------   0 moyu       (501) staff       (20)     2510 2022-10-06 05:53:46.000000 upload_machine-0.0.82/upload_machine/utils/img_upload/ptpimg.py
--rwx------   0 moyu       (501) staff       (20)     1904 2022-11-06 06:50:27.000000 upload_machine-0.0.82/upload_machine/utils/img_upload/redleaves.py
--rw-r--r--   0 moyu       (501) staff       (20)     2426 2023-01-20 04:03:37.000000 upload_machine-0.0.82/upload_machine/utils/img_upload/sharkimg.py
--rwx------   0 moyu       (501) staff       (20)     2875 2022-10-06 05:53:46.000000 upload_machine-0.0.82/upload_machine/utils/img_upload/smms.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 10:23:42.289414 upload_machine-0.0.82/upload_machine/utils/mediafile/
--rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.82/upload_machine/utils/mediafile/__init__.py
--rwx------   0 moyu       (501) staff       (20)    17212 2022-10-06 05:53:46.000000 upload_machine-0.0.82/upload_machine/utils/mediafile/douban_book.py
--rwx------   0 moyu       (501) staff       (20)    24814 2022-10-06 05:53:46.000000 upload_machine-0.0.82/upload_machine/utils/mediafile/douban_movie.py
--rwx------   0 moyu       (501) staff       (20)     6861 2022-10-06 08:34:29.000000 upload_machine-0.0.82/upload_machine/utils/mediafile/doubaninfo.py
--rw-r--r--   0 moyu       (501) staff       (20)     2418 2023-01-03 18:41:08.000000 upload_machine-0.0.82/upload_machine/utils/mediafile/maketorrent.py
--rwx------   0 moyu       (501) staff       (20)    65406 2023-08-06 10:23:18.000000 upload_machine-0.0.82/upload_machine/utils/mediafile/mediafile.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 10:23:42.294577 upload_machine-0.0.82/upload_machine/utils/para_ctrl/
--rwx------   0 moyu       (501) staff       (20)      218 2022-10-06 08:34:43.000000 upload_machine-0.0.82/upload_machine/utils/para_ctrl/__init__.py
--rwx------   0 moyu       (501) staff       (20)     6779 2022-10-09 10:10:39.000000 upload_machine-0.0.82/upload_machine/utils/para_ctrl/para_ctrl.py
--rwxr-xr-x   0 moyu       (501) staff       (20)     2154 2023-01-20 04:03:37.000000 upload_machine-0.0.82/upload_machine/utils/para_ctrl/readargs.py
--rwx------   0 moyu       (501) staff       (20)     1901 2023-01-06 10:01:44.000000 upload_machine-0.0.82/upload_machine/utils/para_ctrl/readyaml.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 10:23:42.295827 upload_machine-0.0.82/upload_machine/utils/pathinfo/
--rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.82/upload_machine/utils/pathinfo/__init__.py
--rwx------   0 moyu       (501) staff       (20)    26791 2023-08-06 07:37:26.000000 upload_machine-0.0.82/upload_machine/utils/pathinfo/pathinfo.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 10:23:42.297103 upload_machine-0.0.82/upload_machine/utils/rss_ctrl/
--rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.82/upload_machine/utils/rss_ctrl/__init__.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 10:23:42.297871 upload_machine-0.0.82/upload_machine/utils/seed_machine/
--rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.82/upload_machine/utils/seed_machine/__init__.py
--rwx------   0 moyu       (501) staff       (20)    21911 2023-08-06 08:04:07.000000 upload_machine-0.0.82/upload_machine/utils/seed_machine/seed_machine.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 10:23:42.299514 upload_machine-0.0.82/upload_machine/utils/signer/
--rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.82/upload_machine/utils/signer/__init__.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 10:23:42.300451 upload_machine-0.0.82/upload_machine/utils/site/
--rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.82/upload_machine/utils/site/__init__.py
--rwx------   0 moyu       (501) staff       (20)     4302 2023-01-02 15:05:32.000000 upload_machine-0.0.82/upload_machine/utils/site/site.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 10:23:42.328210 upload_machine-0.0.82/upload_machine/utils/uploader/
--rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.82/upload_machine/utils/uploader/__init__.py
--rwx------   0 moyu       (501) staff       (20)     5800 2023-01-08 11:40:16.000000 upload_machine-0.0.82/upload_machine/utils/uploader/audience_upload.py
--rwx------   0 moyu       (501) staff       (20)     1706 2023-08-06 06:58:29.000000 upload_machine-0.0.82/upload_machine/utils/uploader/auto_upload.py
--rwx------   0 moyu       (501) staff       (20)     7397 2023-01-05 04:08:25.000000 upload_machine-0.0.82/upload_machine/utils/uploader/carpt_upload.py
--rw-r--r--   0 moyu       (501) staff       (20)     8198 2023-08-05 18:44:07.000000 upload_machine-0.0.82/upload_machine/utils/uploader/dajiao_upload.py
--rwx------   0 moyu       (501) staff       (20)    10309 2023-01-06 12:18:37.000000 upload_machine-0.0.82/upload_machine/utils/uploader/hares_upload.py
--rwx------   0 moyu       (501) staff       (20)     8922 2023-01-08 11:39:46.000000 upload_machine-0.0.82/upload_machine/utils/uploader/hdfans_upload.py
--rwx------   0 moyu       (501) staff       (20)     6032 2023-01-05 04:08:36.000000 upload_machine-0.0.82/upload_machine/utils/uploader/hdpt_upload.py
--rwx------   0 moyu       (501) staff       (20)     7263 2023-01-06 12:18:50.000000 upload_machine-0.0.82/upload_machine/utils/uploader/hdsky_upload.py
--rwx------   0 moyu       (501) staff       (20)     8361 2023-08-06 10:20:07.000000 upload_machine-0.0.82/upload_machine/utils/uploader/hdvideo_upload.py
--rwx------   0 moyu       (501) staff       (20)     9220 2023-01-06 12:18:58.000000 upload_machine-0.0.82/upload_machine/utils/uploader/hhclub_upload.py
--rwx------   0 moyu       (501) staff       (20)     8642 2023-01-06 12:19:01.000000 upload_machine-0.0.82/upload_machine/utils/uploader/ihdbits_upload.py
--rwx------   0 moyu       (501) staff       (20)    19758 2023-01-11 18:07:47.000000 upload_machine-0.0.82/upload_machine/utils/uploader/lemonhd_upload.py
--rwx------   0 moyu       (501) staff       (20)     7123 2023-01-06 12:19:07.000000 upload_machine-0.0.82/upload_machine/utils/uploader/mteam_upload.py
--rw-r--r--   0 moyu       (501) staff       (20)     8728 2023-08-05 18:44:22.000000 upload_machine-0.0.82/upload_machine/utils/uploader/pandapt_upload.py
--rwx------   0 moyu       (501) staff       (20)     7926 2023-02-12 10:09:06.000000 upload_machine-0.0.82/upload_machine/utils/uploader/piggo_upload.py
--rwx------   0 moyu       (501) staff       (20)     4804 2023-01-05 04:09:08.000000 upload_machine-0.0.82/upload_machine/utils/uploader/pter_upload.py
--rwx------   0 moyu       (501) staff       (20)     8888 2023-05-14 16:45:46.000000 upload_machine-0.0.82/upload_machine/utils/uploader/redleaves_upload.py
--rw-r--r--   0 moyu       (501) staff       (20)     8379 2023-08-06 09:32:35.000000 upload_machine-0.0.82/upload_machine/utils/uploader/rousi_upload.py
--rwxr-xr-x   0 moyu       (501) staff       (20)     8322 2023-02-28 11:45:25.000000 upload_machine-0.0.82/upload_machine/utils/uploader/sharkpt_upload.py
--rwx------   0 moyu       (501) staff       (20)     7308 2023-01-11 18:11:31.000000 upload_machine-0.0.82/upload_machine/utils/uploader/ssd_upload.py
--rwx------   0 moyu       (501) staff       (20)    10649 2023-01-06 04:48:18.000000 upload_machine-0.0.82/upload_machine/utils/uploader/upload_tools.py
--rwx------   0 moyu       (501) staff       (20)     7707 2023-01-06 12:19:20.000000 upload_machine-0.0.82/upload_machine/utils/uploader/wintersakura_upload.py
--rwx------   0 moyu       (501) staff       (20)    10462 2023-01-06 17:28:21.000000 upload_machine-0.0.82/upload_machine/utils/uploader/zhuque_upload.py
--rwx------   0 moyu       (501) staff       (20)     7858 2023-01-08 11:39:12.000000 upload_machine-0.0.82/upload_machine/utils/uploader/zmpt_upload.py
-drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-06 10:23:42.270455 upload_machine-0.0.82/upload_machine.egg-info/
--rwx------   0 moyu       (501) staff       (20)    14608 2023-08-06 10:23:40.000000 upload_machine-0.0.82/upload_machine.egg-info/PKG-INFO
--rwx------   0 moyu       (501) staff       (20)     2814 2023-08-06 10:23:42.000000 upload_machine-0.0.82/upload_machine.egg-info/SOURCES.txt
--rwx------   0 moyu       (501) staff       (20)        1 2023-08-06 10:23:41.000000 upload_machine-0.0.82/upload_machine.egg-info/dependency_links.txt
--rwx------   0 moyu       (501) staff       (20)       90 2023-08-06 10:23:41.000000 upload_machine-0.0.82/upload_machine.egg-info/entry_points.txt
--rwx------   0 moyu       (501) staff       (20)      137 2023-08-06 10:23:41.000000 upload_machine-0.0.82/upload_machine.egg-info/requires.txt
--rwx------   0 moyu       (501) staff       (20)       15 2023-08-06 10:23:41.000000 upload_machine-0.0.82/upload_machine.egg-info/top_level.txt
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-08 19:04:09.622733 upload_machine-0.0.83/
+-rwx------   0 moyu       (501) staff       (20)     1063 2022-10-06 05:53:46.000000 upload_machine-0.0.83/LICENSE
+-rwx------   0 moyu       (501) staff       (20)       37 2022-10-06 08:50:43.000000 upload_machine-0.0.83/MANIFEST.in
+-rw-r--r--   0 moyu       (501) staff       (20)    14608 2023-08-08 19:04:09.621825 upload_machine-0.0.83/PKG-INFO
+-rwxr-xr-x   0 moyu       (501) staff       (20)    14206 2023-08-06 07:01:29.000000 upload_machine-0.0.83/README.md
+-rw-r--r--   0 moyu       (501) staff       (20)       38 2023-08-08 19:04:09.622933 upload_machine-0.0.83/setup.cfg
+-rwx------   0 moyu       (501) staff       (20)     1110 2023-08-08 19:04:01.000000 upload_machine-0.0.83/setup.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-08 19:04:09.552486 upload_machine-0.0.83/upload_machine/
+-rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.83/upload_machine/__init__.py
+-rwx------   0 moyu       (501) staff       (20)      241 2022-10-06 08:12:01.000000 upload_machine-0.0.83/upload_machine/basicinfo.yaml
+-rwx------   0 moyu       (501) staff       (20)     2622 2023-01-02 14:54:11.000000 upload_machine-0.0.83/upload_machine/main.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-08 19:04:09.556772 upload_machine-0.0.83/upload_machine/utils/
+-rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.83/upload_machine/utils/__init__.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-08 19:04:09.557850 upload_machine-0.0.83/upload_machine/utils/edittorrent/
+-rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.83/upload_machine/utils/edittorrent/__init__.py
+-rwx------   0 moyu       (501) staff       (20)     3966 2022-10-06 05:53:46.000000 upload_machine-0.0.83/upload_machine/utils/edittorrent/edittorrent.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-08 19:04:09.568649 upload_machine-0.0.83/upload_machine/utils/img_upload/
+-rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.83/upload_machine/utils/img_upload/__init__.py
+-rwx------   0 moyu       (501) staff       (20)     7231 2022-10-06 05:53:46.000000 upload_machine-0.0.83/upload_machine/utils/img_upload/chevereto.py
+-rwx------   0 moyu       (501) staff       (20)     2674 2022-10-06 05:53:46.000000 upload_machine-0.0.83/upload_machine/utils/img_upload/fapping_emp.py
+-rwx------   0 moyu       (501) staff       (20)     4521 2022-10-06 05:53:46.000000 upload_machine-0.0.83/upload_machine/utils/img_upload/imgbox.py
+-rwxr-xr-x   0 moyu       (501) staff       (20)     9014 2023-01-20 04:03:37.000000 upload_machine-0.0.83/upload_machine/utils/img_upload/imgupload.py
+-rwx------   0 moyu       (501) staff       (20)     2510 2022-10-06 05:53:46.000000 upload_machine-0.0.83/upload_machine/utils/img_upload/ptpimg.py
+-rwx------   0 moyu       (501) staff       (20)     1904 2022-11-06 06:50:27.000000 upload_machine-0.0.83/upload_machine/utils/img_upload/redleaves.py
+-rw-r--r--   0 moyu       (501) staff       (20)     2426 2023-01-20 04:03:37.000000 upload_machine-0.0.83/upload_machine/utils/img_upload/sharkimg.py
+-rwx------   0 moyu       (501) staff       (20)     2875 2022-10-06 05:53:46.000000 upload_machine-0.0.83/upload_machine/utils/img_upload/smms.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-08 19:04:09.576367 upload_machine-0.0.83/upload_machine/utils/mediafile/
+-rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.83/upload_machine/utils/mediafile/__init__.py
+-rwx------   0 moyu       (501) staff       (20)    17212 2022-10-06 05:53:46.000000 upload_machine-0.0.83/upload_machine/utils/mediafile/douban_book.py
+-rwx------   0 moyu       (501) staff       (20)    24814 2022-10-06 05:53:46.000000 upload_machine-0.0.83/upload_machine/utils/mediafile/douban_movie.py
+-rwx------   0 moyu       (501) staff       (20)     6861 2022-10-06 08:34:29.000000 upload_machine-0.0.83/upload_machine/utils/mediafile/doubaninfo.py
+-rw-r--r--   0 moyu       (501) staff       (20)     2418 2023-01-03 18:41:08.000000 upload_machine-0.0.83/upload_machine/utils/mediafile/maketorrent.py
+-rwx------   0 moyu       (501) staff       (20)    65406 2023-08-06 10:23:18.000000 upload_machine-0.0.83/upload_machine/utils/mediafile/mediafile.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-08 19:04:09.581945 upload_machine-0.0.83/upload_machine/utils/para_ctrl/
+-rwx------   0 moyu       (501) staff       (20)      218 2022-10-06 08:34:43.000000 upload_machine-0.0.83/upload_machine/utils/para_ctrl/__init__.py
+-rwx------   0 moyu       (501) staff       (20)     6779 2022-10-09 10:10:39.000000 upload_machine-0.0.83/upload_machine/utils/para_ctrl/para_ctrl.py
+-rwxr-xr-x   0 moyu       (501) staff       (20)     2154 2023-01-20 04:03:37.000000 upload_machine-0.0.83/upload_machine/utils/para_ctrl/readargs.py
+-rwx------   0 moyu       (501) staff       (20)     1901 2023-01-06 10:01:44.000000 upload_machine-0.0.83/upload_machine/utils/para_ctrl/readyaml.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-08 19:04:09.583489 upload_machine-0.0.83/upload_machine/utils/pathinfo/
+-rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.83/upload_machine/utils/pathinfo/__init__.py
+-rwx------   0 moyu       (501) staff       (20)    26791 2023-08-06 07:37:26.000000 upload_machine-0.0.83/upload_machine/utils/pathinfo/pathinfo.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-08 19:04:09.585451 upload_machine-0.0.83/upload_machine/utils/rss_ctrl/
+-rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.83/upload_machine/utils/rss_ctrl/__init__.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-08 19:04:09.586322 upload_machine-0.0.83/upload_machine/utils/seed_machine/
+-rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.83/upload_machine/utils/seed_machine/__init__.py
+-rwx------   0 moyu       (501) staff       (20)    21911 2023-08-06 08:04:07.000000 upload_machine-0.0.83/upload_machine/utils/seed_machine/seed_machine.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-08 19:04:09.587853 upload_machine-0.0.83/upload_machine/utils/signer/
+-rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.83/upload_machine/utils/signer/__init__.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-08 19:04:09.588806 upload_machine-0.0.83/upload_machine/utils/site/
+-rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.83/upload_machine/utils/site/__init__.py
+-rwx------   0 moyu       (501) staff       (20)     4302 2023-01-02 15:05:32.000000 upload_machine-0.0.83/upload_machine/utils/site/site.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-08 19:04:09.620436 upload_machine-0.0.83/upload_machine/utils/uploader/
+-rwx------   0 moyu       (501) staff       (20)        0 2022-10-06 05:53:46.000000 upload_machine-0.0.83/upload_machine/utils/uploader/__init__.py
+-rwx------   0 moyu       (501) staff       (20)     5800 2023-01-08 11:40:16.000000 upload_machine-0.0.83/upload_machine/utils/uploader/audience_upload.py
+-rwx------   0 moyu       (501) staff       (20)     1706 2023-08-06 06:58:29.000000 upload_machine-0.0.83/upload_machine/utils/uploader/auto_upload.py
+-rwx------   0 moyu       (501) staff       (20)     7397 2023-01-05 04:08:25.000000 upload_machine-0.0.83/upload_machine/utils/uploader/carpt_upload.py
+-rw-r--r--   0 moyu       (501) staff       (20)     8198 2023-08-08 01:24:50.000000 upload_machine-0.0.83/upload_machine/utils/uploader/dajiao_upload.py
+-rwx------   0 moyu       (501) staff       (20)    10309 2023-01-06 12:18:37.000000 upload_machine-0.0.83/upload_machine/utils/uploader/hares_upload.py
+-rwx------   0 moyu       (501) staff       (20)     8922 2023-01-08 11:39:46.000000 upload_machine-0.0.83/upload_machine/utils/uploader/hdfans_upload.py
+-rwx------   0 moyu       (501) staff       (20)     6032 2023-01-05 04:08:36.000000 upload_machine-0.0.83/upload_machine/utils/uploader/hdpt_upload.py
+-rwx------   0 moyu       (501) staff       (20)     7263 2023-01-06 12:18:50.000000 upload_machine-0.0.83/upload_machine/utils/uploader/hdsky_upload.py
+-rwx------   0 moyu       (501) staff       (20)     8361 2023-08-08 19:01:57.000000 upload_machine-0.0.83/upload_machine/utils/uploader/hdvideo_upload.py
+-rwx------   0 moyu       (501) staff       (20)     9220 2023-01-06 12:18:58.000000 upload_machine-0.0.83/upload_machine/utils/uploader/hhclub_upload.py
+-rwx------   0 moyu       (501) staff       (20)     8642 2023-01-06 12:19:01.000000 upload_machine-0.0.83/upload_machine/utils/uploader/ihdbits_upload.py
+-rwx------   0 moyu       (501) staff       (20)    19758 2023-01-11 18:07:47.000000 upload_machine-0.0.83/upload_machine/utils/uploader/lemonhd_upload.py
+-rwx------   0 moyu       (501) staff       (20)     7123 2023-01-06 12:19:07.000000 upload_machine-0.0.83/upload_machine/utils/uploader/mteam_upload.py
+-rw-r--r--   0 moyu       (501) staff       (20)     8618 2023-08-08 19:02:10.000000 upload_machine-0.0.83/upload_machine/utils/uploader/pandapt_upload.py
+-rwx------   0 moyu       (501) staff       (20)     7926 2023-02-12 10:09:06.000000 upload_machine-0.0.83/upload_machine/utils/uploader/piggo_upload.py
+-rwx------   0 moyu       (501) staff       (20)     4804 2023-01-05 04:09:08.000000 upload_machine-0.0.83/upload_machine/utils/uploader/pter_upload.py
+-rwx------   0 moyu       (501) staff       (20)     8888 2023-05-14 16:45:46.000000 upload_machine-0.0.83/upload_machine/utils/uploader/redleaves_upload.py
+-rw-r--r--   0 moyu       (501) staff       (20)     8379 2023-08-08 01:25:54.000000 upload_machine-0.0.83/upload_machine/utils/uploader/rousi_upload.py
+-rwxr-xr-x   0 moyu       (501) staff       (20)     8322 2023-02-28 11:45:25.000000 upload_machine-0.0.83/upload_machine/utils/uploader/sharkpt_upload.py
+-rwx------   0 moyu       (501) staff       (20)     7308 2023-01-11 18:11:31.000000 upload_machine-0.0.83/upload_machine/utils/uploader/ssd_upload.py
+-rwx------   0 moyu       (501) staff       (20)    10649 2023-01-06 04:48:18.000000 upload_machine-0.0.83/upload_machine/utils/uploader/upload_tools.py
+-rwx------   0 moyu       (501) staff       (20)     7707 2023-01-06 12:19:20.000000 upload_machine-0.0.83/upload_machine/utils/uploader/wintersakura_upload.py
+-rwx------   0 moyu       (501) staff       (20)    10462 2023-01-06 17:28:21.000000 upload_machine-0.0.83/upload_machine/utils/uploader/zhuque_upload.py
+-rwx------   0 moyu       (501) staff       (20)     7858 2023-01-08 11:39:12.000000 upload_machine-0.0.83/upload_machine/utils/uploader/zmpt_upload.py
+drwxr-xr-x   0 moyu       (501) staff       (20)        0 2023-08-08 19:04:09.556176 upload_machine-0.0.83/upload_machine.egg-info/
+-rwx------   0 moyu       (501) staff       (20)    14608 2023-08-08 19:04:08.000000 upload_machine-0.0.83/upload_machine.egg-info/PKG-INFO
+-rwx------   0 moyu       (501) staff       (20)     2814 2023-08-08 19:04:09.000000 upload_machine-0.0.83/upload_machine.egg-info/SOURCES.txt
+-rwx------   0 moyu       (501) staff       (20)        1 2023-08-08 19:04:08.000000 upload_machine-0.0.83/upload_machine.egg-info/dependency_links.txt
+-rwx------   0 moyu       (501) staff       (20)       90 2023-08-08 19:04:08.000000 upload_machine-0.0.83/upload_machine.egg-info/entry_points.txt
+-rwx------   0 moyu       (501) staff       (20)      137 2023-08-08 19:04:08.000000 upload_machine-0.0.83/upload_machine.egg-info/requires.txt
+-rwx------   0 moyu       (501) staff       (20)       15 2023-08-08 19:04:08.000000 upload_machine-0.0.83/upload_machine.egg-info/top_level.txt
```

### Comparing `upload_machine-0.0.82/LICENSE` & `upload_machine-0.0.83/LICENSE`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/PKG-INFO` & `upload_machine-0.0.83/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upload_machine
-Version: 0.0.82
+Version: 0.0.83
 Summary: Upload local resources to PT trackers automatically.
 Home-page: https://github.com/dongshuyan/Upload_Machine
 Author: sauterne
 Author-email: ssauterne@qq.com
 License: MIT Licence
 Keywords: pip,autoupload,auto,upload,PT,private tracker
 Platform: any
```

### Comparing `upload_machine-0.0.82/README.md` & `upload_machine-0.0.83/README.md`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/setup.py` & `upload_machine-0.0.83/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import io
 
 setup(
     name = "upload_machine",     
-    version = "0.0.82", 
+    version = "0.0.83", 
     keywords = ["pip", "autoupload","auto","upload","PT","private tracker"],            
     description = "Upload local resources to PT trackers automatically.",    
     long_description=io.open("README.md", "r", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     license = "MIT Licence",    
 
     entry_points = {
```

### Comparing `upload_machine-0.0.82/upload_machine/main.py` & `upload_machine-0.0.83/upload_machine/main.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/edittorrent/edittorrent.py` & `upload_machine-0.0.83/upload_machine/utils/edittorrent/edittorrent.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/img_upload/chevereto.py` & `upload_machine-0.0.83/upload_machine/utils/img_upload/chevereto.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/img_upload/fapping_emp.py` & `upload_machine-0.0.83/upload_machine/utils/img_upload/fapping_emp.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/img_upload/imgbox.py` & `upload_machine-0.0.83/upload_machine/utils/img_upload/imgbox.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/img_upload/imgupload.py` & `upload_machine-0.0.83/upload_machine/utils/img_upload/imgupload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/img_upload/ptpimg.py` & `upload_machine-0.0.83/upload_machine/utils/img_upload/ptpimg.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/img_upload/redleaves.py` & `upload_machine-0.0.83/upload_machine/utils/img_upload/redleaves.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/img_upload/sharkimg.py` & `upload_machine-0.0.83/upload_machine/utils/img_upload/sharkimg.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/img_upload/smms.py` & `upload_machine-0.0.83/upload_machine/utils/img_upload/smms.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/mediafile/douban_book.py` & `upload_machine-0.0.83/upload_machine/utils/mediafile/douban_book.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/mediafile/douban_movie.py` & `upload_machine-0.0.83/upload_machine/utils/mediafile/douban_movie.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/mediafile/doubaninfo.py` & `upload_machine-0.0.83/upload_machine/utils/mediafile/doubaninfo.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/mediafile/maketorrent.py` & `upload_machine-0.0.83/upload_machine/utils/mediafile/maketorrent.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/mediafile/mediafile.py` & `upload_machine-0.0.83/upload_machine/utils/mediafile/mediafile.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/para_ctrl/para_ctrl.py` & `upload_machine-0.0.83/upload_machine/utils/para_ctrl/para_ctrl.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/para_ctrl/readargs.py` & `upload_machine-0.0.83/upload_machine/utils/para_ctrl/readargs.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/para_ctrl/readyaml.py` & `upload_machine-0.0.83/upload_machine/utils/para_ctrl/readyaml.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/pathinfo/pathinfo.py` & `upload_machine-0.0.83/upload_machine/utils/pathinfo/pathinfo.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/seed_machine/seed_machine.py` & `upload_machine-0.0.83/upload_machine/utils/seed_machine/seed_machine.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/site/site.py` & `upload_machine-0.0.83/upload_machine/utils/site/site.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/uploader/audience_upload.py` & `upload_machine-0.0.83/upload_machine/utils/uploader/audience_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/uploader/auto_upload.py` & `upload_machine-0.0.83/upload_machine/utils/uploader/auto_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/uploader/carpt_upload.py` & `upload_machine-0.0.83/upload_machine/utils/uploader/carpt_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/uploader/dajiao_upload.py` & `upload_machine-0.0.83/upload_machine/utils/uploader/dajiao_upload.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -121,18 +121,18 @@
         audiocodec_sel='9'
     elif 'FLAC' in file1.Audio_Format.upper():
         audiocodec_sel='1'
     elif 'APE' in file1.Audio_Format.upper():
         audiocodec_sel='2'
     elif 'MP3' in file1.Audio_Format.upper():
         audiocodec_sel='4'
-    elif 'AC3' in file1.Audio_Format.upper() or 'AC-3' in file1.Audio_Format.upper() or 'DD' in file1.Audio_Format.upper():
-        audiocodec_sel='13'
     elif 'EAC3' in file1.Audio_Format.upper() or 'EAC-3' in file1.Audio_Format.upper() or 'DDP' in file1.Audio_Format.upper():
         audiocodec_sel='13'
+    elif 'AC3' in file1.Audio_Format.upper() or 'AC-3' in file1.Audio_Format.upper() or 'DD' in file1.Audio_Format.upper():
+        audiocodec_sel='13'
     elif 'DTS:X' in file1.Audio_Format.upper() or 'DTS-X' in file1.Audio_Format.upper():
         audiocodec_sel='10'
     elif 'DTS' in file1.Audio_Format.upper():
         audiocodec_sel='3'
     elif 'WAV' in file1.Audio_Format.upper():
         audiocodec_sel='7'
     elif 'M4A' in file1.Audio_Format.upper():
```

### Comparing `upload_machine-0.0.82/upload_machine/utils/uploader/hares_upload.py` & `upload_machine-0.0.83/upload_machine/utils/uploader/hares_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/uploader/hdfans_upload.py` & `upload_machine-0.0.83/upload_machine/utils/uploader/hdfans_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/uploader/hdpt_upload.py` & `upload_machine-0.0.83/upload_machine/utils/uploader/hdpt_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/uploader/hdsky_upload.py` & `upload_machine-0.0.83/upload_machine/utils/uploader/hdsky_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/uploader/hdvideo_upload.py` & `upload_machine-0.0.83/upload_machine/utils/uploader/hdvideo_upload.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -125,18 +125,18 @@
         audiocodec_sel='11'
     elif 'FLAC' in file1.Audio_Format.upper():
         audiocodec_sel='1'
     elif 'APE' in file1.Audio_Format.upper():
         audiocodec_sel='2'
     elif 'MP3' in file1.Audio_Format.upper():
         audiocodec_sel='18'
-    elif 'AC3' in file1.Audio_Format.upper() or 'AC-3' in file1.Audio_Format.upper() or 'DD' in file1.Audio_Format.upper():
-        audiocodec_sel='9'
     elif 'EAC3' in file1.Audio_Format.upper() or 'EAC-3' in file1.Audio_Format.upper() or 'DDP' in file1.Audio_Format.upper():
         audiocodec_sel='10'
+    elif 'AC3' in file1.Audio_Format.upper() or 'AC-3' in file1.Audio_Format.upper() or 'DD' in file1.Audio_Format.upper():
+        audiocodec_sel='9'
     elif 'DTS:X' in file1.Audio_Format.upper() or 'DTS-X' in file1.Audio_Format.upper():
         audiocodec_sel='16'
     elif 'DTS' in file1.Audio_Format.upper():
         audiocodec_sel='17'
     elif 'WAV' in file1.Audio_Format.upper():
         audiocodec_sel='12'
     elif 'M4A' in file1.Audio_Format.upper():
```

### Comparing `upload_machine-0.0.82/upload_machine/utils/uploader/hhclub_upload.py` & `upload_machine-0.0.83/upload_machine/utils/uploader/hhclub_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/uploader/ihdbits_upload.py` & `upload_machine-0.0.83/upload_machine/utils/uploader/ihdbits_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/uploader/lemonhd_upload.py` & `upload_machine-0.0.83/upload_machine/utils/uploader/lemonhd_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/uploader/mteam_upload.py` & `upload_machine-0.0.83/upload_machine/utils/uploader/mteam_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/uploader/pandapt_upload.py` & `upload_machine-0.0.83/upload_machine/utils/uploader/pandapt_upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,18 +97,18 @@
         audiocodec_sel='1'
     elif 'FLAC' in file1.Audio_Format.upper():
         audiocodec_sel='11'
     elif 'APE' in file1.Audio_Format.upper():
         audiocodec_sel='12'
     elif 'MP3' in file1.Audio_Format.upper():
         audiocodec_sel='10'
-    elif 'AC3' in file1.Audio_Format.upper() or 'AC-3' in file1.Audio_Format.upper() or 'DD' in file1.Audio_Format.upper():
-        audiocodec_sel='5'
     elif 'EAC3' in file1.Audio_Format.upper() or 'EAC-3' in file1.Audio_Format.upper() or 'DDP' in file1.Audio_Format.upper():
         audiocodec_sel='6'
+    elif 'AC3' in file1.Audio_Format.upper() or 'AC-3' in file1.Audio_Format.upper() or 'DD' in file1.Audio_Format.upper():
+        audiocodec_sel='5'
     elif 'DTS:X' in file1.Audio_Format.upper() or 'DTS-X' in file1.Audio_Format.upper():
         audiocodec_sel='2'
     elif 'DTS' in file1.Audio_Format.upper():
         audiocodec_sel='4'
     elif 'WAV' in file1.Audio_Format.upper():
         audiocodec_sel='15'
     elif 'OGG' in file1.Audio_Format.upper():
@@ -185,17 +185,14 @@
         logger.info('已选择粤语')
     if not file1.sublan=='' and ('简' in file1.sublan or '繁' in file1.sublan or '中' in file1.sublan):
         tags.append(6)
         logger.info('已选择中字')
     if file1.pathinfo.complete==1:
         tags.append(10)
         logger.info('已选择完结')
-    if 'anime' in file1.pathinfo.type.lower():
-        tags.append(12)
-        logger.info('已选择动画')
 
     
     tags=list(set(tags))
     tags.sort()
     
     if siteinfo.uplver==1:
         uplver='yes'
```

### Comparing `upload_machine-0.0.82/upload_machine/utils/uploader/piggo_upload.py` & `upload_machine-0.0.83/upload_machine/utils/uploader/piggo_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/uploader/pter_upload.py` & `upload_machine-0.0.83/upload_machine/utils/uploader/pter_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/uploader/redleaves_upload.py` & `upload_machine-0.0.83/upload_machine/utils/uploader/redleaves_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/uploader/rousi_upload.py` & `upload_machine-0.0.83/upload_machine/utils/uploader/rousi_upload.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -121,18 +121,18 @@
         audiocodec_sel='9'
     elif 'FLAC' in file1.Audio_Format.upper():
         audiocodec_sel='1'
     elif 'APE' in file1.Audio_Format.upper():
         audiocodec_sel='2'
     elif 'MP3' in file1.Audio_Format.upper():
         audiocodec_sel='4'
-    elif 'AC3' in file1.Audio_Format.upper() or 'AC-3' in file1.Audio_Format.upper() or 'DD' in file1.Audio_Format.upper():
-        audiocodec_sel='13'
     elif 'EAC3' in file1.Audio_Format.upper() or 'EAC-3' in file1.Audio_Format.upper() or 'DDP' in file1.Audio_Format.upper():
         audiocodec_sel='13'
+    elif 'AC3' in file1.Audio_Format.upper() or 'AC-3' in file1.Audio_Format.upper() or 'DD' in file1.Audio_Format.upper():
+        audiocodec_sel='13'
     elif 'DTS:X' in file1.Audio_Format.upper() or 'DTS-X' in file1.Audio_Format.upper():
         audiocodec_sel='10'
     elif 'DTS' in file1.Audio_Format.upper():
         audiocodec_sel='3'
     elif 'WAV' in file1.Audio_Format.upper():
         audiocodec_sel='7'
     elif 'M4A' in file1.Audio_Format.upper():
```

### Comparing `upload_machine-0.0.82/upload_machine/utils/uploader/sharkpt_upload.py` & `upload_machine-0.0.83/upload_machine/utils/uploader/sharkpt_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/uploader/ssd_upload.py` & `upload_machine-0.0.83/upload_machine/utils/uploader/ssd_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/uploader/upload_tools.py` & `upload_machine-0.0.83/upload_machine/utils/uploader/upload_tools.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/uploader/wintersakura_upload.py` & `upload_machine-0.0.83/upload_machine/utils/uploader/wintersakura_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/uploader/zhuque_upload.py` & `upload_machine-0.0.83/upload_machine/utils/uploader/zhuque_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine/utils/uploader/zmpt_upload.py` & `upload_machine-0.0.83/upload_machine/utils/uploader/zmpt_upload.py`

 * *Files identical despite different names*

### Comparing `upload_machine-0.0.82/upload_machine.egg-info/PKG-INFO` & `upload_machine-0.0.83/upload_machine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upload-machine
-Version: 0.0.82
+Version: 0.0.83
 Summary: Upload local resources to PT trackers automatically.
 Home-page: https://github.com/dongshuyan/Upload_Machine
 Author: sauterne
 Author-email: ssauterne@qq.com
 License: MIT Licence
 Keywords: pip,autoupload,auto,upload,PT,private tracker
 Platform: any
```

### Comparing `upload_machine-0.0.82/upload_machine.egg-info/SOURCES.txt` & `upload_machine-0.0.83/upload_machine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

