# Comparing `tmp/not1mm-23.8.6.tar.gz` & `tmp/not1mm-23.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "not1mm-23.8.6.tar", last modified: Sun Aug  6 14:48:11 2023, max compression
+gzip compressed data, was "not1mm-23.8.7.tar", last modified: Tue Aug  8 00:03:30 2023, max compression
```

## Comparing `not1mm-23.8.6.tar` & `not1mm-23.8.7.tar`

### file list

```diff
@@ -1,150 +1,154 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-08-06 14:48:11.200721 not1mm-23.8.6/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-05-05 15:15:13.000000 not1mm-23.8.6/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23710 2023-08-06 14:48:11.199721 not1mm-23.8.6/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22965 2023-08-06 14:44:57.000000 not1mm-23.8.6/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-08-06 14:48:11.008719 not1mm-23.8.6/not1mm/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.8.6/not1mm/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    96702 2023-08-05 22:05:12.000000 not1mm-23.8.6/not1mm/__main__.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    26884 2023-08-05 22:05:12.000000 not1mm-23.8.6/not1mm/bandmap.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6451 2023-08-06 14:19:02.000000 not1mm-23.8.6/not1mm/checkwindow.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-08-06 14:48:11.051719 not1mm-23.8.6/not1mm/data/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-27 16:44:51.000000 not1mm-23.8.6/not1mm/data/JetBrainsMono-Regular.ttf
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   657382 2023-08-03 15:48:04.000000 not1mm-23.8.6/not1mm/data/MASTER.SCP
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2067 2023-05-18 23:48:17.000000 not1mm-23.8.6/not1mm/data/about.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2023-04-18 03:49:58.000000 not1mm-23.8.6/not1mm/data/alpha bravo charlie delta.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5246 2023-05-01 15:41:16.000000 not1mm-23.8.6/not1mm/data/bandmap.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2023-03-15 16:56:38.000000 not1mm-23.8.6/not1mm/data/check.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2572 2023-08-06 13:54:37.000000 not1mm-23.8.6/not1mm/data/checkwindow.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    41522 2023-07-13 12:57:36.000000 not1mm-23.8.6/not1mm/data/configuration.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2023-03-07 17:30:38.000000 not1mm-23.8.6/not1mm/data/contests.sql
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)  4667346 2023-08-03 14:57:05.000000 not1mm-23.8.6/not1mm/data/cty.json
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2023-04-11 19:54:10.000000 not1mm-23.8.6/not1mm/data/cwmacros.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      116 2023-06-20 14:51:41.000000 not1mm-23.8.6/not1mm/data/donors.html
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    19280 2023-03-20 20:22:09.000000 not1mm-23.8.6/not1mm/data/editcontact.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2273 2023-02-21 14:39:24.000000 not1mm-23.8.6/not1mm/data/editmacro.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2023-02-10 02:42:18.000000 not1mm-23.8.6/not1mm/data/greendot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-09 20:47:40.000000 not1mm-23.8.6/not1mm/data/k6gte-not1mm.desktop
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4010 2023-02-09 20:45:38.000000 not1mm-23.8.6/not1mm/data/k6gte.not1mm-128.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1108 2023-02-09 20:45:03.000000 not1mm-23.8.6/not1mm/data/k6gte.not1mm-32.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2152 2023-02-09 20:45:22.000000 not1mm-23.8.6/not1mm/data/k6gte.not1mm-64.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      970 2023-03-23 20:14:51.000000 not1mm-23.8.6/not1mm/data/logwindow.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45152 2023-08-05 22:05:12.000000 not1mm-23.8.6/not1mm/data/main.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    18584 2023-07-29 14:24:03.000000 not1mm-23.8.6/not1mm/data/new_contest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    20129 2023-06-17 01:47:05.000000 not1mm-23.8.6/not1mm/data/not1mm.html
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2018 2023-02-12 17:56:36.000000 not1mm-23.8.6/not1mm/data/opon.ui
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-08-06 14:48:11.152721 not1mm-23.8.6/not1mm/data/phonetics/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2023-04-21 20:24:24.000000 not1mm-23.8.6/not1mm/data/phonetics/0.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2023-04-21 20:25:33.000000 not1mm-23.8.6/not1mm/data/phonetics/1.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2023-04-21 20:27:16.000000 not1mm-23.8.6/not1mm/data/phonetics/2.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2023-04-21 20:29:07.000000 not1mm-23.8.6/not1mm/data/phonetics/3.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2023-04-21 20:29:49.000000 not1mm-23.8.6/not1mm/data/phonetics/4.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2023-04-21 21:46:26.000000 not1mm-23.8.6/not1mm/data/phonetics/5.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2023-04-21 21:08:45.000000 not1mm-23.8.6/not1mm/data/phonetics/6.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2023-04-21 21:10:50.000000 not1mm-23.8.6/not1mm/data/phonetics/7.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2023-04-21 21:13:51.000000 not1mm-23.8.6/not1mm/data/phonetics/73.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2023-04-21 21:11:40.000000 not1mm-23.8.6/not1mm/data/phonetics/8.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2023-04-21 21:12:32.000000 not1mm-23.8.6/not1mm/data/phonetics/9.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2023-04-21 21:14:36.000000 not1mm-23.8.6/not1mm/data/phonetics/a.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2023-04-21 21:15:20.000000 not1mm-23.8.6/not1mm/data/phonetics/again.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2023-04-21 21:16:10.000000 not1mm-23.8.6/not1mm/data/phonetics/b.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2023-04-21 21:17:07.000000 not1mm-23.8.6/not1mm/data/phonetics/c.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2023-04-21 13:38:05.000000 not1mm-23.8.6/not1mm/data/phonetics/contest.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2023-04-21 21:17:54.000000 not1mm-23.8.6/not1mm/data/phonetics/cq.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2023-04-21 21:18:24.000000 not1mm-23.8.6/not1mm/data/phonetics/d.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2023-04-21 21:19:02.000000 not1mm-23.8.6/not1mm/data/phonetics/e.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2023-04-21 21:19:38.000000 not1mm-23.8.6/not1mm/data/phonetics/f.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2023-04-21 21:20:18.000000 not1mm-23.8.6/not1mm/data/phonetics/g.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2023-04-21 21:21:03.000000 not1mm-23.8.6/not1mm/data/phonetics/h.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2023-04-21 21:23:33.000000 not1mm-23.8.6/not1mm/data/phonetics/i.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2023-04-21 21:24:12.000000 not1mm-23.8.6/not1mm/data/phonetics/j.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2023-04-21 21:24:57.000000 not1mm-23.8.6/not1mm/data/phonetics/k.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2023-04-21 21:25:43.000000 not1mm-23.8.6/not1mm/data/phonetics/k6gte.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2023-04-21 21:26:21.000000 not1mm-23.8.6/not1mm/data/phonetics/l.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2023-04-21 21:27:07.000000 not1mm-23.8.6/not1mm/data/phonetics/m.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2023-04-21 21:27:57.000000 not1mm-23.8.6/not1mm/data/phonetics/mynumber.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2023-04-21 21:28:42.000000 not1mm-23.8.6/not1mm/data/phonetics/n.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2023-04-21 21:29:54.000000 not1mm-23.8.6/not1mm/data/phonetics/nil.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2023-04-21 21:30:37.000000 not1mm-23.8.6/not1mm/data/phonetics/o.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2023-04-21 21:31:22.000000 not1mm-23.8.6/not1mm/data/phonetics/p.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2023-04-21 21:31:58.000000 not1mm-23.8.6/not1mm/data/phonetics/q.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2023-04-21 21:32:39.000000 not1mm-23.8.6/not1mm/data/phonetics/r.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2023-04-21 21:33:20.000000 not1mm-23.8.6/not1mm/data/phonetics/roger.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2023-04-21 21:33:59.000000 not1mm-23.8.6/not1mm/data/phonetics/s.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2023-04-17 20:43:04.000000 not1mm-23.8.6/not1mm/data/phonetics/space.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2023-04-21 21:35:28.000000 not1mm-23.8.6/not1mm/data/phonetics/t.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2023-04-21 21:36:54.000000 not1mm-23.8.6/not1mm/data/phonetics/thankyou.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2023-04-21 21:37:27.000000 not1mm-23.8.6/not1mm/data/phonetics/thankyouqrz.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2023-04-21 21:38:05.000000 not1mm-23.8.6/not1mm/data/phonetics/u.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2023-04-21 21:38:37.000000 not1mm-23.8.6/not1mm/data/phonetics/v.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2023-04-21 21:39:21.000000 not1mm-23.8.6/not1mm/data/phonetics/w.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2023-04-21 21:40:02.000000 not1mm-23.8.6/not1mm/data/phonetics/x.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2023-04-21 21:40:40.000000 not1mm-23.8.6/not1mm/data/phonetics/y.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2023-04-21 21:41:22.000000 not1mm-23.8.6/not1mm/data/phonetics/yourcall.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2023-04-21 21:41:59.000000 not1mm-23.8.6/not1mm/data/phonetics/z.wav
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2023-04-03 14:20:44.000000 not1mm-23.8.6/not1mm/data/pickcontest.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-02-10 02:42:40.000000 not1mm-23.8.6/not1mm/data/reddot.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35566 2023-04-15 16:43:11.000000 not1mm-23.8.6/not1mm/data/settings.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2023-04-18 18:00:45.000000 not1mm-23.8.6/not1mm/data/ssbmacros.txt
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-08-06 14:48:11.169721 not1mm-23.8.6/not1mm/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.8.6/not1mm/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      379 2023-04-10 20:24:21.000000 not1mm-23.8.6/not1mm/lib/about.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15676 2023-05-22 20:40:03.000000 not1mm-23.8.6/not1mm/lib/cat_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3123 2023-05-11 20:24:55.000000 not1mm-23.8.6/not1mm/lib/cwinterface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40117 2023-08-06 14:12:38.000000 not1mm-23.8.6/not1mm/lib/database.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      357 2023-03-20 13:17:21.000000 not1mm-23.8.6/not1mm/lib/edit_contact.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      559 2023-03-06 17:59:31.000000 not1mm-23.8.6/not1mm/lib/edit_macro.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-06 18:02:53.000000 not1mm-23.8.6/not1mm/lib/edit_opon.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1973 2023-04-11 17:58:02.000000 not1mm-23.8.6/not1mm/lib/edit_station.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8760 2023-04-05 20:29:02.000000 not1mm-23.8.6/not1mm/lib/ham_utility.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13916 2023-03-07 18:49:31.000000 not1mm-23.8.6/not1mm/lib/lookup.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1761 2023-05-12 16:20:09.000000 not1mm-23.8.6/not1mm/lib/multicast.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5713 2023-05-24 14:24:14.000000 not1mm-23.8.6/not1mm/lib/n1mm.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      354 2023-03-28 20:21:24.000000 not1mm-23.8.6/not1mm/lib/new_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-31 21:22:27.000000 not1mm-23.8.6/not1mm/lib/select_contest.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6885 2023-05-23 19:07:39.000000 not1mm-23.8.6/not1mm/lib/settings.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1692 2023-08-05 22:05:12.000000 not1mm-23.8.6/not1mm/lib/super_check_partial.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       46 2023-08-06 14:46:27.000000 not1mm-23.8.6/not1mm/lib/version.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1286 2023-05-19 19:40:38.000000 not1mm-23.8.6/not1mm/lib/versiontest.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    34331 2023-08-05 22:05:12.000000 not1mm-23.8.6/not1mm/logwindow.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-08-06 14:48:11.190721 not1mm-23.8.6/not1mm/plugins/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13883 2023-05-29 18:30:11.000000 not1mm-23.8.6/not1mm/plugins/10_10_fall_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13888 2023-05-29 18:30:48.000000 not1mm-23.8.6/not1mm/plugins/10_10_spring_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13895 2023-05-29 18:31:29.000000 not1mm-23.8.6/not1mm/plugins/10_10_summer_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13898 2023-05-29 18:31:57.000000 not1mm-23.8.6/not1mm/plugins/10_10_winter_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-20 21:20:03.000000 not1mm-23.8.6/not1mm/plugins/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14735 2023-07-29 14:29:55.000000 not1mm-23.8.6/not1mm/plugins/arrl_dx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14738 2023-07-29 14:29:58.000000 not1mm-23.8.6/not1mm/plugins/arrl_dx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13049 2023-07-29 02:50:49.000000 not1mm-23.8.6/not1mm/plugins/arrl_field_day.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2860 2023-05-05 16:10:11.000000 not1mm-23.8.6/not1mm/plugins/arrl_rtty_ru.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    16077 2023-05-29 18:33:47.000000 not1mm-23.8.6/not1mm/plugins/arrl_ss_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    16082 2023-05-29 18:34:01.000000 not1mm-23.8.6/not1mm/plugins/arrl_ss_phone.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14756 2023-07-29 03:28:01.000000 not1mm-23.8.6/not1mm/plugins/canada_day.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15352 2023-07-29 03:23:39.000000 not1mm-23.8.6/not1mm/plugins/cq_wpx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15374 2023-07-29 03:23:26.000000 not1mm-23.8.6/not1mm/plugins/cq_wpx_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14082 2023-07-29 03:21:19.000000 not1mm-23.8.6/not1mm/plugins/cq_ww_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14086 2023-07-29 03:21:22.000000 not1mm-23.8.6/not1mm/plugins/cq_ww_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14941 2023-07-29 03:16:59.000000 not1mm-23.8.6/not1mm/plugins/cwt.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7495 2023-07-13 13:24:37.000000 not1mm-23.8.6/not1mm/plugins/general_logging.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14878 2023-07-29 03:07:17.000000 not1mm-23.8.6/not1mm/plugins/iaru_hf.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13905 2023-07-29 03:12:54.000000 not1mm-23.8.6/not1mm/plugins/jidx_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13906 2023-07-29 03:13:05.000000 not1mm-23.8.6/not1mm/plugins/jidx_ph.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14791 2023-07-28 21:37:33.000000 not1mm-23.8.6/not1mm/plugins/naqp_cw.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14795 2023-07-28 21:37:47.000000 not1mm-23.8.6/not1mm/plugins/naqp_ssb.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3010 2023-07-29 03:01:06.000000 not1mm-23.8.6/not1mm/plugins/winter_field_day.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-08-06 14:48:11.197721 not1mm-23.8.6/not1mm/testing/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2083 2023-05-19 23:10:32.000000 not1mm-23.8.6/not1mm/testing/fakeflrig.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1658 2023-05-19 17:23:54.000000 not1mm-23.8.6/not1mm/testing/flrigclient.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)     1051 2023-03-01 19:35:50.000000 not1mm-23.8.6/not1mm/testing/multicast_listener.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1099 2023-06-28 22:12:28.000000 not1mm-23.8.6/not1mm/testing/n1mm_listener.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1660 2023-05-14 06:26:14.000000 not1mm-23.8.6/not1mm/testing/test.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-08-06 14:48:11.011719 not1mm-23.8.6/not1mm.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23710 2023-08-06 14:48:10.000000 not1mm-23.8.6/not1mm.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3809 2023-08-06 14:48:10.000000 not1mm-23.8.6/not1mm.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-08-06 14:48:10.000000 not1mm-23.8.6/not1mm.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-08-06 14:48:10.000000 not1mm-23.8.6/not1mm.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       92 2023-08-06 14:48:10.000000 not1mm-23.8.6/not1mm.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       33 2023-08-06 14:48:10.000000 not1mm-23.8.6/not1mm.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1271 2023-08-06 14:46:39.000000 not1mm-23.8.6/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-08-06 14:48:11.200721 not1mm-23.8.6/setup.cfg
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-08-06 14:48:11.197721 not1mm-23.8.6/testing/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      471 2023-06-26 02:26:39.000000 not1mm-23.8.6/testing/test.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-08-08 00:03:30.778498 not1mm-23.8.7/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2022-05-05 15:15:13.000000 not1mm-23.8.7/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    24034 2023-08-08 00:03:30.777498 not1mm-23.8.7/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    23289 2023-08-08 00:00:01.000000 not1mm-23.8.7/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-08-08 00:03:30.573495 not1mm-23.8.7/not1mm/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.8.7/not1mm/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    97019 2023-08-07 23:17:39.000000 not1mm-23.8.7/not1mm/__main__.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    26884 2023-08-05 22:05:12.000000 not1mm-23.8.7/not1mm/bandmap.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6451 2023-08-06 14:19:02.000000 not1mm-23.8.7/not1mm/checkwindow.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-08-08 00:03:30.636496 not1mm-23.8.7/not1mm/data/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2023-01-27 16:44:51.000000 not1mm-23.8.7/not1mm/data/JetBrainsMono-Regular.ttf
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   657382 2023-08-03 15:48:04.000000 not1mm-23.8.7/not1mm/data/MASTER.SCP
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2067 2023-05-18 23:48:17.000000 not1mm-23.8.7/not1mm/data/about.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      224 2023-04-18 03:49:58.000000 not1mm-23.8.7/not1mm/data/alpha bravo charlie delta.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5246 2023-05-01 15:41:16.000000 not1mm-23.8.7/not1mm/data/bandmap.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      387 2023-03-15 16:56:38.000000 not1mm-23.8.7/not1mm/data/check.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2572 2023-08-06 13:54:37.000000 not1mm-23.8.7/not1mm/data/checkwindow.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    41522 2023-07-13 12:57:36.000000 not1mm-23.8.7/not1mm/data/configuration.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    89307 2023-03-07 17:30:38.000000 not1mm-23.8.7/not1mm/data/contests.sql
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)  4667346 2023-08-03 14:57:05.000000 not1mm-23.8.7/not1mm/data/cty.json
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      451 2023-04-11 19:54:10.000000 not1mm-23.8.7/not1mm/data/cwmacros.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      116 2023-06-20 14:51:41.000000 not1mm-23.8.7/not1mm/data/donors.html
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    19280 2023-03-20 20:22:09.000000 not1mm-23.8.7/not1mm/data/editcontact.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2273 2023-02-21 14:39:24.000000 not1mm-23.8.7/not1mm/data/editmacro.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      474 2023-02-10 02:42:18.000000 not1mm-23.8.7/not1mm/data/greendot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      205 2023-02-09 20:47:40.000000 not1mm-23.8.7/not1mm/data/k6gte-not1mm.desktop
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4010 2023-02-09 20:45:38.000000 not1mm-23.8.7/not1mm/data/k6gte.not1mm-128.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1108 2023-02-09 20:45:03.000000 not1mm-23.8.7/not1mm/data/k6gte.not1mm-32.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2152 2023-02-09 20:45:22.000000 not1mm-23.8.7/not1mm/data/k6gte.not1mm-64.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      970 2023-03-23 20:14:51.000000 not1mm-23.8.7/not1mm/data/logwindow.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45292 2023-08-07 23:17:39.000000 not1mm-23.8.7/not1mm/data/main.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    18584 2023-07-29 14:24:03.000000 not1mm-23.8.7/not1mm/data/new_contest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    20129 2023-06-17 01:47:05.000000 not1mm-23.8.7/not1mm/data/not1mm.html
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2018 2023-02-12 17:56:36.000000 not1mm-23.8.7/not1mm/data/opon.ui
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-08-08 00:03:30.749497 not1mm-23.8.7/not1mm/data/phonetics/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42590 2023-04-21 20:24:24.000000 not1mm-23.8.7/not1mm/data/phonetics/0.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    30248 2023-04-21 20:25:33.000000 not1mm-23.8.7/not1mm/data/phonetics/1.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    29584 2023-04-21 20:27:16.000000 not1mm-23.8.7/not1mm/data/phonetics/2.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32072 2023-04-21 20:29:07.000000 not1mm-23.8.7/not1mm/data/phonetics/3.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43052 2023-04-21 20:29:49.000000 not1mm-23.8.7/not1mm/data/phonetics/4.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51976 2023-04-21 21:46:26.000000 not1mm-23.8.7/not1mm/data/phonetics/5.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58634 2023-04-21 21:08:45.000000 not1mm-23.8.7/not1mm/data/phonetics/6.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49154 2023-04-21 21:10:50.000000 not1mm-23.8.7/not1mm/data/phonetics/7.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    32842 2023-04-21 21:13:51.000000 not1mm-23.8.7/not1mm/data/phonetics/73.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35636 2023-04-21 21:11:40.000000 not1mm-23.8.7/not1mm/data/phonetics/8.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    39592 2023-04-21 21:12:32.000000 not1mm-23.8.7/not1mm/data/phonetics/9.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46800 2023-04-21 21:14:36.000000 not1mm-23.8.7/not1mm/data/phonetics/a.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    44594 2023-04-21 21:15:20.000000 not1mm-23.8.7/not1mm/data/phonetics/again.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40976 2023-04-21 21:16:10.000000 not1mm-23.8.7/not1mm/data/phonetics/b.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46746 2023-04-21 21:17:07.000000 not1mm-23.8.7/not1mm/data/phonetics/c.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    62558 2023-04-21 13:38:05.000000 not1mm-23.8.7/not1mm/data/phonetics/contest.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    92498 2023-04-21 21:17:54.000000 not1mm-23.8.7/not1mm/data/phonetics/cq.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52524 2023-04-21 21:18:24.000000 not1mm-23.8.7/not1mm/data/phonetics/d.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    45700 2023-04-21 21:19:02.000000 not1mm-23.8.7/not1mm/data/phonetics/e.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    53438 2023-04-21 21:19:38.000000 not1mm-23.8.7/not1mm/data/phonetics/f.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    42766 2023-04-21 21:20:18.000000 not1mm-23.8.7/not1mm/data/phonetics/g.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50040 2023-04-21 21:21:03.000000 not1mm-23.8.7/not1mm/data/phonetics/h.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46372 2023-04-21 21:23:33.000000 not1mm-23.8.7/not1mm/data/phonetics/i.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43434 2023-04-21 21:24:12.000000 not1mm-23.8.7/not1mm/data/phonetics/j.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    49066 2023-04-21 21:24:57.000000 not1mm-23.8.7/not1mm/data/phonetics/k.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   185562 2023-04-21 21:25:43.000000 not1mm-23.8.7/not1mm/data/phonetics/k6gte.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    43154 2023-04-21 21:26:21.000000 not1mm-23.8.7/not1mm/data/phonetics/l.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    54352 2023-04-21 21:27:07.000000 not1mm-23.8.7/not1mm/data/phonetics/m.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56798 2023-04-21 21:27:57.000000 not1mm-23.8.7/not1mm/data/phonetics/mynumber.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    52204 2023-04-21 21:28:42.000000 not1mm-23.8.7/not1mm/data/phonetics/n.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   154544 2023-04-21 21:29:54.000000 not1mm-23.8.7/not1mm/data/phonetics/nil.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47440 2023-04-21 21:30:37.000000 not1mm-23.8.7/not1mm/data/phonetics/o.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    38300 2023-04-21 21:31:22.000000 not1mm-23.8.7/not1mm/data/phonetics/p.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    55288 2023-04-21 21:31:58.000000 not1mm-23.8.7/not1mm/data/phonetics/q.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    47432 2023-04-21 21:32:39.000000 not1mm-23.8.7/not1mm/data/phonetics/r.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46122 2023-04-21 21:33:20.000000 not1mm-23.8.7/not1mm/data/phonetics/roger.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    60698 2023-04-21 21:33:59.000000 not1mm-23.8.7/not1mm/data/phonetics/s.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    70424 2023-04-17 20:43:04.000000 not1mm-23.8.7/not1mm/data/phonetics/space.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    58196 2023-04-21 21:35:28.000000 not1mm-23.8.7/not1mm/data/phonetics/t.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56320 2023-04-21 21:36:54.000000 not1mm-23.8.7/not1mm/data/phonetics/thankyou.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    94980 2023-04-21 21:37:27.000000 not1mm-23.8.7/not1mm/data/phonetics/thankyouqrz.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    65922 2023-04-21 21:38:05.000000 not1mm-23.8.7/not1mm/data/phonetics/u.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    50142 2023-04-21 21:38:37.000000 not1mm-23.8.7/not1mm/data/phonetics/v.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    37638 2023-04-21 21:39:21.000000 not1mm-23.8.7/not1mm/data/phonetics/w.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    61870 2023-04-21 21:40:02.000000 not1mm-23.8.7/not1mm/data/phonetics/x.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    56524 2023-04-21 21:40:40.000000 not1mm-23.8.7/not1mm/data/phonetics/y.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    46510 2023-04-21 21:41:22.000000 not1mm-23.8.7/not1mm/data/phonetics/yourcall.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    51768 2023-04-21 21:41:59.000000 not1mm-23.8.7/not1mm/data/phonetics/z.wav
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1600 2023-04-03 14:20:44.000000 not1mm-23.8.7/not1mm/data/pickcontest.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      565 2023-02-10 02:42:40.000000 not1mm-23.8.7/not1mm/data/reddot.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35566 2023-04-15 16:43:11.000000 not1mm-23.8.7/not1mm/data/settings.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      470 2023-04-18 18:00:45.000000 not1mm-23.8.7/not1mm/data/ssbmacros.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1873 2023-08-07 23:17:39.000000 not1mm-23.8.7/not1mm/data/vfo.ui
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-08-08 00:03:30.759498 not1mm-23.8.7/not1mm/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2022-11-03 15:04:39.000000 not1mm-23.8.7/not1mm/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      379 2023-04-10 20:24:21.000000 not1mm-23.8.7/not1mm/lib/about.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15676 2023-05-22 20:40:03.000000 not1mm-23.8.7/not1mm/lib/cat_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3123 2023-05-11 20:24:55.000000 not1mm-23.8.7/not1mm/lib/cwinterface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    40117 2023-08-06 14:12:38.000000 not1mm-23.8.7/not1mm/lib/database.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      357 2023-03-20 13:17:21.000000 not1mm-23.8.7/not1mm/lib/edit_contact.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      559 2023-03-06 17:59:31.000000 not1mm-23.8.7/not1mm/lib/edit_macro.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-06 18:02:53.000000 not1mm-23.8.7/not1mm/lib/edit_opon.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1973 2023-04-11 17:58:02.000000 not1mm-23.8.7/not1mm/lib/edit_station.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     8760 2023-04-05 20:29:02.000000 not1mm-23.8.7/not1mm/lib/ham_utility.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13916 2023-03-07 18:49:31.000000 not1mm-23.8.7/not1mm/lib/lookup.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1761 2023-05-12 16:20:09.000000 not1mm-23.8.7/not1mm/lib/multicast.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5713 2023-05-24 14:24:14.000000 not1mm-23.8.7/not1mm/lib/n1mm.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      354 2023-03-28 20:21:24.000000 not1mm-23.8.7/not1mm/lib/new_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2023-03-31 21:22:27.000000 not1mm-23.8.7/not1mm/lib/select_contest.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6885 2023-05-23 19:07:39.000000 not1mm-23.8.7/not1mm/lib/settings.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1692 2023-08-05 22:05:12.000000 not1mm-23.8.7/not1mm/lib/super_check_partial.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       46 2023-08-07 23:17:39.000000 not1mm-23.8.7/not1mm/lib/version.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1286 2023-05-19 19:40:38.000000 not1mm-23.8.7/not1mm/lib/versiontest.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    34331 2023-08-05 22:05:12.000000 not1mm-23.8.7/not1mm/logwindow.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-08-08 00:03:30.774498 not1mm-23.8.7/not1mm/plugins/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13883 2023-05-29 18:30:11.000000 not1mm-23.8.7/not1mm/plugins/10_10_fall_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13888 2023-05-29 18:30:48.000000 not1mm-23.8.7/not1mm/plugins/10_10_spring_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13895 2023-05-29 18:31:29.000000 not1mm-23.8.7/not1mm/plugins/10_10_summer_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13898 2023-05-29 18:31:57.000000 not1mm-23.8.7/not1mm/plugins/10_10_winter_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2023-02-20 21:20:03.000000 not1mm-23.8.7/not1mm/plugins/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14735 2023-07-29 14:29:55.000000 not1mm-23.8.7/not1mm/plugins/arrl_dx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14738 2023-07-29 14:29:58.000000 not1mm-23.8.7/not1mm/plugins/arrl_dx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13049 2023-07-29 02:50:49.000000 not1mm-23.8.7/not1mm/plugins/arrl_field_day.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2860 2023-05-05 16:10:11.000000 not1mm-23.8.7/not1mm/plugins/arrl_rtty_ru.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    16077 2023-05-29 18:33:47.000000 not1mm-23.8.7/not1mm/plugins/arrl_ss_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    16082 2023-05-29 18:34:01.000000 not1mm-23.8.7/not1mm/plugins/arrl_ss_phone.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14756 2023-07-29 03:28:01.000000 not1mm-23.8.7/not1mm/plugins/canada_day.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15352 2023-07-29 03:23:39.000000 not1mm-23.8.7/not1mm/plugins/cq_wpx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    15374 2023-07-29 03:23:26.000000 not1mm-23.8.7/not1mm/plugins/cq_wpx_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14082 2023-07-29 03:21:19.000000 not1mm-23.8.7/not1mm/plugins/cq_ww_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14086 2023-07-29 03:21:22.000000 not1mm-23.8.7/not1mm/plugins/cq_ww_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14941 2023-07-29 03:16:59.000000 not1mm-23.8.7/not1mm/plugins/cwt.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     7495 2023-07-13 13:24:37.000000 not1mm-23.8.7/not1mm/plugins/general_logging.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14878 2023-07-29 03:07:17.000000 not1mm-23.8.7/not1mm/plugins/iaru_hf.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13905 2023-07-29 03:12:54.000000 not1mm-23.8.7/not1mm/plugins/jidx_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13906 2023-07-29 03:13:05.000000 not1mm-23.8.7/not1mm/plugins/jidx_ph.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14791 2023-07-28 21:37:33.000000 not1mm-23.8.7/not1mm/plugins/naqp_cw.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14795 2023-07-28 21:37:47.000000 not1mm-23.8.7/not1mm/plugins/naqp_ssb.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3010 2023-07-29 03:01:06.000000 not1mm-23.8.7/not1mm/plugins/winter_field_day.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-08-08 00:03:30.776498 not1mm-23.8.7/not1mm/testing/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2083 2023-05-19 23:10:32.000000 not1mm-23.8.7/not1mm/testing/fakeflrig.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1658 2023-05-19 17:23:54.000000 not1mm-23.8.7/not1mm/testing/flrigclient.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)     1051 2023-03-01 19:35:50.000000 not1mm-23.8.7/not1mm/testing/multicast_listener.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1099 2023-06-28 22:12:28.000000 not1mm-23.8.7/not1mm/testing/n1mm_listener.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1660 2023-05-14 06:26:14.000000 not1mm-23.8.7/not1mm/testing/test.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     9431 2023-08-07 23:17:39.000000 not1mm-23.8.7/not1mm/vfo.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-08-08 00:03:30.575495 not1mm-23.8.7/not1mm.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    24034 2023-08-08 00:03:30.000000 not1mm-23.8.7/not1mm.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3863 2023-08-08 00:03:30.000000 not1mm-23.8.7/not1mm.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2023-08-08 00:03:30.000000 not1mm-23.8.7/not1mm.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2023-08-08 00:03:30.000000 not1mm-23.8.7/not1mm.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       92 2023-08-08 00:03:30.000000 not1mm-23.8.7/not1mm.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       46 2023-08-08 00:03:30.000000 not1mm-23.8.7/not1mm.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1271 2023-08-07 23:17:39.000000 not1mm-23.8.7/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2023-08-08 00:03:30.778498 not1mm-23.8.7/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-08-08 00:03:30.776498 not1mm-23.8.7/testing/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      471 2023-06-26 02:26:39.000000 not1mm-23.8.7/testing/test.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2023-08-08 00:03:30.777498 not1mm-23.8.7/usb_vfo_knob/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1057 2023-08-07 23:17:39.000000 not1mm-23.8.7/usb_vfo_knob/code.py
```

### Comparing `not1mm-23.8.6/LICENSE` & `not1mm-23.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/PKG-INFO` & `not1mm-23.8.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not1mm
-Version: 23.8.6
+Version: 23.8.7
 Summary: NOT1MM Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/not1mm
 Project-URL: Bug Tracker, https://github.com/mbridak/not1mm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -77,14 +77,15 @@
     - [The Main Window](#the-main-window)
       - [Keyboard commands](#keyboard-commands)
     - [Log Display](#log-display)
       - [Editing a contact](#editing-a-contact)
   - [Recalulate Mults](#recalulate-mults)
   - [Bandmap](#bandmap)
   - [Check Window](#check-window)
+  - [VFO](#vfo)
   - [Cabrillo](#cabrillo)
   - [ADIF](#adif)
   - [Dupe checking](#dupe-checking)
   - [Contest specific notes](#contest-specific-notes)
     - [ARRL Sweekstakes](#arrl-sweekstakes)
       - [The exchange parser](#the-exchange-parser)
       - [The exchange](#the-exchange)
@@ -138,14 +139,15 @@
 - Japan International DX SSB
 - NAQP CW
 - NAQP SSB
 - RAC Canada Day
 
 ## Recent Changes
 
+- [23-8-7] Control Remote Rig VFO with a bespoke USB VFO Knob.
 - [23-8-6] Add parsing of local log to check window.
 - [23-8-5] Add Check Window. Moved MASTER.SCP stuff to it's own class. Close sub windows when main app closes.
 
 See [CHANGELOG.md](CHANGELOG.md) for prior changes.
 
 ## Installing from PyPi
 
@@ -474,14 +476,23 @@
 
 `Window`>`Check Window`
 
 As you enter a callsign, the Check Window will show probable matches to calls either in the MASTER.SCP file, or your local log. The MASTER.SCP column will show results for strings of 3 or more matching from the start of the call string. The local log column will show matches of any length appearing anywhere in the string.
 
 ![Check Window](https://github.com/mbridak/not1mm/raw/master/pic/checkwindow.png)
 
+## VFO
+
+You can control the VFO on a remote rig by:
+
+1. Making the [VFO](https://github.com/mbridak/not1mm/blob/master/usb_vfo_knob/vfo.md)...
+2. Then... `Window`>`VFO`
+
+![VFO](https://github.com/mbridak/not1mm/raw/master/usb_vfo_knob/vfo.gif)
+
 ## Cabrillo
 
 Click on `File` > `Generate Cabrillo`
 
 The file will be placed in your home directory. The name will be in the format of:
 
 `StationCall`_`ContestName`.log
```

### Comparing `not1mm-23.8.6/README.md` & `not1mm-23.8.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     - [The Main Window](#the-main-window)
       - [Keyboard commands](#keyboard-commands)
     - [Log Display](#log-display)
       - [Editing a contact](#editing-a-contact)
   - [Recalulate Mults](#recalulate-mults)
   - [Bandmap](#bandmap)
   - [Check Window](#check-window)
+  - [VFO](#vfo)
   - [Cabrillo](#cabrillo)
   - [ADIF](#adif)
   - [Dupe checking](#dupe-checking)
   - [Contest specific notes](#contest-specific-notes)
     - [ARRL Sweekstakes](#arrl-sweekstakes)
       - [The exchange parser](#the-exchange-parser)
       - [The exchange](#the-exchange)
@@ -119,14 +120,15 @@
 - Japan International DX SSB
 - NAQP CW
 - NAQP SSB
 - RAC Canada Day
 
 ## Recent Changes
 
+- [23-8-7] Control Remote Rig VFO with a bespoke USB VFO Knob.
 - [23-8-6] Add parsing of local log to check window.
 - [23-8-5] Add Check Window. Moved MASTER.SCP stuff to it's own class. Close sub windows when main app closes.
 
 See [CHANGELOG.md](CHANGELOG.md) for prior changes.
 
 ## Installing from PyPi
 
@@ -455,14 +457,23 @@
 
 `Window`>`Check Window`
 
 As you enter a callsign, the Check Window will show probable matches to calls either in the MASTER.SCP file, or your local log. The MASTER.SCP column will show results for strings of 3 or more matching from the start of the call string. The local log column will show matches of any length appearing anywhere in the string.
 
 ![Check Window](https://github.com/mbridak/not1mm/raw/master/pic/checkwindow.png)
 
+## VFO
+
+You can control the VFO on a remote rig by:
+
+1. Making the [VFO](https://github.com/mbridak/not1mm/blob/master/usb_vfo_knob/vfo.md)...
+2. Then... `Window`>`VFO`
+
+![VFO](https://github.com/mbridak/not1mm/raw/master/usb_vfo_knob/vfo.gif)
+
 ## Cabrillo
 
 Click on `File` > `Generate Cabrillo`
 
 The file will be placed in your home directory. The name will be in the format of:
 
 `StationCall`_`ContestName`.log
```

### Comparing `not1mm-23.8.6/not1mm/__main__.py` & `not1mm-23.8.7/not1mm/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -413,5632 +413,5652 @@
 000019c0: 5f62 616e 646d 6170 5f77 696e 646f 7729  _bandmap_window)
 000019d0: 0a20 2020 2020 2020 2073 656c 662e 6163  .        self.ac
 000019e0: 7469 6f6e 4368 6563 6b5f 5769 6e64 6f77  tionCheck_Window
 000019f0: 2e74 7269 6767 6572 6564 2e63 6f6e 6e65  .triggered.conne
 00001a00: 6374 2873 656c 662e 6c61 756e 6368 5f63  ct(self.launch_c
 00001a10: 6865 636b 5f77 696e 646f 7729 0a20 2020  heck_window).   
 00001a20: 2020 2020 2073 656c 662e 6163 7469 6f6e       self.action
-00001a30: 5265 6361 6c63 756c 6174 655f 4d75 6c74  Recalculate_Mult
-00001a40: 732e 7472 6967 6765 7265 642e 636f 6e6e  s.triggered.conn
-00001a50: 6563 7428 7365 6c66 2e72 6563 616c 6375  ect(self.recalcu
-00001a60: 6c61 7465 5f6d 756c 7473 290a 0a20 2020  late_mults)..   
-00001a70: 2020 2020 2073 656c 662e 6163 7469 6f6e       self.action
-00001a80: 4765 6e65 7261 7465 5f43 6162 7269 6c6c  Generate_Cabrill
-00001a90: 6f2e 7472 6967 6765 7265 642e 636f 6e6e  o.triggered.conn
-00001aa0: 6563 7428 7365 6c66 2e67 656e 6572 6174  ect(self.generat
-00001ab0: 655f 6361 6272 696c 6c6f 290a 2020 2020  e_cabrillo).    
-00001ac0: 2020 2020 7365 6c66 2e61 6374 696f 6e47      self.actionG
-00001ad0: 656e 6572 6174 655f 4144 4946 2e74 7269  enerate_ADIF.tri
-00001ae0: 6767 6572 6564 2e63 6f6e 6e65 6374 2873  ggered.connect(s
-00001af0: 656c 662e 6765 6e65 7261 7465 5f61 6469  elf.generate_adi
-00001b00: 6629 0a0a 2020 2020 2020 2020 7365 6c66  f)..        self
-00001b10: 2e61 6374 696f 6e43 6f6e 6669 6775 7261  .actionConfigura
-00001b20: 7469 6f6e 5f53 6574 7469 6e67 732e 7472  tion_Settings.tr
-00001b30: 6967 6765 7265 642e 636f 6e6e 6563 7428  iggered.connect(
-00001b40: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00001b50: 662e 6564 6974 5f63 6f6e 6669 6775 7261  f.edit_configura
-00001b60: 7469 6f6e 5f73 6574 7469 6e67 730a 2020  tion_settings.  
-00001b70: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00001b80: 7365 6c66 2e61 6374 696f 6e53 7461 7469  self.actionStati
-00001b90: 6f6e 5365 7474 696e 6773 2e74 7269 6767  onSettings.trigg
-00001ba0: 6572 6564 2e63 6f6e 6e65 6374 2873 656c  ered.connect(sel
-00001bb0: 662e 6564 6974 5f73 7461 7469 6f6e 5f73  f.edit_station_s
-00001bc0: 6574 7469 6e67 7329 0a0a 2020 2020 2020  ettings)..      
-00001bd0: 2020 7365 6c66 2e61 6374 696f 6e4e 6577    self.actionNew
-00001be0: 5f43 6f6e 7465 7374 2e74 7269 6767 6572  _Contest.trigger
-00001bf0: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
-00001c00: 6e65 775f 636f 6e74 6573 745f 6469 616c  new_contest_dial
-00001c10: 6f67 290a 2020 2020 2020 2020 7365 6c66  og).        self
-00001c20: 2e61 6374 696f 6e4f 7065 6e5f 436f 6e74  .actionOpen_Cont
-00001c30: 6573 742e 7472 6967 6765 7265 642e 636f  est.triggered.co
-00001c40: 6e6e 6563 7428 7365 6c66 2e6f 7065 6e5f  nnect(self.open_
-00001c50: 636f 6e74 6573 7429 0a20 2020 2020 2020  contest).       
-00001c60: 2073 656c 662e 6163 7469 6f6e 4564 6974   self.actionEdit
-00001c70: 5f43 7572 7265 6e74 5f43 6f6e 7465 7374  _Current_Contest
-00001c80: 2e74 7269 6767 6572 6564 2e63 6f6e 6e65  .triggered.conne
-00001c90: 6374 2873 656c 662e 6564 6974 5f63 6f6e  ct(self.edit_con
-00001ca0: 7465 7374 290a 0a20 2020 2020 2020 2073  test)..        s
-00001cb0: 656c 662e 6163 7469 6f6e 4e65 775f 4461  elf.actionNew_Da
-00001cc0: 7461 6261 7365 2e74 7269 6767 6572 6564  tabase.triggered
-00001cd0: 2e63 6f6e 6e65 6374 2873 656c 662e 6e65  .connect(self.ne
-00001ce0: 775f 6461 7461 6261 7365 290a 2020 2020  w_database).    
-00001cf0: 2020 2020 7365 6c66 2e61 6374 696f 6e4f      self.actionO
-00001d00: 7065 6e5f 4461 7461 6261 7365 2e74 7269  pen_Database.tri
-00001d10: 6767 6572 6564 2e63 6f6e 6e65 6374 2873  ggered.connect(s
-00001d20: 656c 662e 6f70 656e 5f64 6174 6162 6173  elf.open_databas
-00001d30: 6529 0a0a 2020 2020 2020 2020 7365 6c66  e)..        self
-00001d40: 2e61 6374 696f 6e45 6469 745f 4d61 6372  .actionEdit_Macr
-00001d50: 6f73 2e74 7269 6767 6572 6564 2e63 6f6e  os.triggered.con
-00001d60: 6e65 6374 2873 656c 662e 6564 6974 5f63  nect(self.edit_c
-00001d70: 775f 6d61 6372 6f73 290a 0a20 2020 2020  w_macros)..     
-00001d80: 2020 2073 656c 662e 6163 7469 6f6e 4162     self.actionAb
-00001d90: 6f75 742e 7472 6967 6765 7265 642e 636f  out.triggered.co
-00001da0: 6e6e 6563 7428 7365 6c66 2e73 686f 775f  nnect(self.show_
-00001db0: 6162 6f75 745f 6469 616c 6f67 290a 2020  about_dialog).  
-00001dc0: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
-00001dd0: 6e48 6f74 4b65 7973 2e74 7269 6767 6572  nHotKeys.trigger
-00001de0: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
-00001df0: 7368 6f77 5f6b 6579 5f68 656c 7029 0a20  show_key_help). 
-00001e00: 2020 2020 2020 2073 656c 662e 6163 7469         self.acti
-00001e10: 6f6e 4865 6c70 2e74 7269 6767 6572 6564  onHelp.triggered
-00001e20: 2e63 6f6e 6e65 6374 2873 656c 662e 7368  .connect(self.sh
-00001e30: 6f77 5f68 656c 705f 6469 616c 6f67 290a  ow_help_dialog).
-00001e40: 2020 2020 2020 2020 7365 6c66 2e61 6374          self.act
-00001e50: 696f 6e55 7064 6174 655f 4354 592e 7472  ionUpdate_CTY.tr
-00001e60: 6967 6765 7265 642e 636f 6e6e 6563 7428  iggered.connect(
-00001e70: 7365 6c66 2e63 6865 636b 5f66 6f72 5f6e  self.check_for_n
-00001e80: 6577 5f63 7479 290a 2020 2020 2020 2020  ew_cty).        
-00001e90: 7365 6c66 2e61 6374 696f 6e55 7064 6174  self.actionUpdat
-00001ea0: 655f 4d41 5354 4552 5f53 4350 2e74 7269  e_MASTER_SCP.tri
-00001eb0: 6767 6572 6564 2e63 6f6e 6e65 6374 2873  ggered.connect(s
-00001ec0: 656c 662e 7570 6461 7465 5f6d 6173 7465  elf.update_maste
-00001ed0: 7273 6370 290a 2020 2020 2020 2020 7365  rscp).        se
-00001ee0: 6c66 2e61 6374 696f 6e51 7569 742e 7472  lf.actionQuit.tr
-00001ef0: 6967 6765 7265 642e 636f 6e6e 6563 7428  iggered.connect(
-00001f00: 7365 6c66 2e71 7569 745f 6170 7029 0a0a  self.quit_app)..
-00001f10: 2020 2020 2020 2020 7365 6c66 2e72 6164          self.rad
-00001f20: 696f 4275 7474 6f6e 5f72 756e 2e63 6c69  ioButton_run.cli
-00001f30: 636b 6564 2e63 6f6e 6e65 6374 2873 656c  cked.connect(sel
-00001f40: 662e 7275 6e5f 7370 5f62 7574 746f 6e73  f.run_sp_buttons
-00001f50: 5f63 6c69 636b 6564 290a 2020 2020 2020  _clicked).      
-00001f60: 2020 7365 6c66 2e72 6164 696f 4275 7474    self.radioButt
-00001f70: 6f6e 5f73 702e 636c 6963 6b65 642e 636f  on_sp.clicked.co
-00001f80: 6e6e 6563 7428 7365 6c66 2e72 756e 5f73  nnect(self.run_s
-00001f90: 705f 6275 7474 6f6e 735f 636c 6963 6b65  p_buttons_clicke
-00001fa0: 6429 0a20 2020 2020 2020 2073 656c 662e  d).        self.
-00001fb0: 7363 6f72 652e 7365 7454 6578 7428 2230  score.setText("0
-00001fc0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00001fd0: 6361 6c6c 7369 676e 2e74 6578 7445 6469  callsign.textEdi
-00001fe0: 7465 642e 636f 6e6e 6563 7428 7365 6c66  ted.connect(self
-00001ff0: 2e63 616c 6c73 6967 6e5f 6368 616e 6765  .callsign_change
-00002000: 6429 0a20 2020 2020 2020 2073 656c 662e  d).        self.
-00002010: 6361 6c6c 7369 676e 2e72 6574 7572 6e50  callsign.returnP
-00002020: 7265 7373 6564 2e63 6f6e 6e65 6374 2873  ressed.connect(s
-00002030: 656c 662e 7361 7665 5f63 6f6e 7461 6374  elf.save_contact
-00002040: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-00002050: 656e 742e 7265 7475 726e 5072 6573 7365  ent.returnPresse
-00002060: 642e 636f 6e6e 6563 7428 7365 6c66 2e73  d.connect(self.s
-00002070: 6176 655f 636f 6e74 6163 7429 0a20 2020  ave_contact).   
-00002080: 2020 2020 2073 656c 662e 7265 6365 6976       self.receiv
-00002090: 652e 7265 7475 726e 5072 6573 7365 642e  e.returnPressed.
-000020a0: 636f 6e6e 6563 7428 7365 6c66 2e73 6176  connect(self.sav
-000020b0: 655f 636f 6e74 6163 7429 0a20 2020 2020  e_contact).     
-000020c0: 2020 2073 656c 662e 6f74 6865 725f 312e     self.other_1.
-000020d0: 7265 7475 726e 5072 6573 7365 642e 636f  returnPressed.co
-000020e0: 6e6e 6563 7428 7365 6c66 2e73 6176 655f  nnect(self.save_
-000020f0: 636f 6e74 6163 7429 0a20 2020 2020 2020  contact).       
-00002100: 2073 656c 662e 6f74 6865 725f 312e 7465   self.other_1.te
-00002110: 7874 4564 6974 6564 2e63 6f6e 6e65 6374  xtEdited.connect
-00002120: 2873 656c 662e 6f74 6865 725f 315f 6368  (self.other_1_ch
-00002130: 616e 6765 6429 0a20 2020 2020 2020 2073  anged).        s
-00002140: 656c 662e 6f74 6865 725f 322e 7265 7475  elf.other_2.retu
-00002150: 726e 5072 6573 7365 642e 636f 6e6e 6563  rnPressed.connec
-00002160: 7428 7365 6c66 2e73 6176 655f 636f 6e74  t(self.save_cont
-00002170: 6163 7429 0a20 2020 2020 2020 2073 656c  act).        sel
-00002180: 662e 6f74 6865 725f 322e 7465 7874 4564  f.other_2.textEd
-00002190: 6974 6564 2e63 6f6e 6e65 6374 2873 656c  ited.connect(sel
-000021a0: 662e 6f74 6865 725f 325f 6368 616e 6765  f.other_2_change
-000021b0: 6429 0a0a 2020 2020 2020 2020 7365 6c66  d)..        self
-000021c0: 2e73 656e 742e 7365 7454 6578 7428 2235  .sent.setText("5
-000021d0: 3922 290a 2020 2020 2020 2020 7365 6c66  9").        self
-000021e0: 2e72 6563 6569 7665 2e73 6574 5465 7874  .receive.setText
-000021f0: 2822 3539 2229 0a20 2020 2020 2020 2069  ("59").        i
-00002200: 636f 6e5f 7061 7468 203d 2057 4f52 4b49  con_path = WORKI
-00002210: 4e47 5f50 4154 4820 2b20 222f 6461 7461  NG_PATH + "/data
-00002220: 2f22 0a20 2020 2020 2020 2073 656c 662e  /".        self.
-00002230: 6772 6565 6e64 6f74 203d 2051 7447 7569  greendot = QtGui
-00002240: 2e51 5069 786d 6170 2869 636f 6e5f 7061  .QPixmap(icon_pa
-00002250: 7468 202b 2022 6772 6565 6e64 6f74 2e70  th + "greendot.p
-00002260: 6e67 2229 0a20 2020 2020 2020 2073 656c  ng").        sel
-00002270: 662e 7265 6464 6f74 203d 2051 7447 7569  f.reddot = QtGui
-00002280: 2e51 5069 786d 6170 2869 636f 6e5f 7061  .QPixmap(icon_pa
-00002290: 7468 202b 2022 7265 6464 6f74 2e70 6e67  th + "reddot.png
-000022a0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-000022b0: 6c65 6674 646f 742e 7365 7450 6978 6d61  leftdot.setPixma
-000022c0: 7028 7365 6c66 2e67 7265 656e 646f 7429  p(self.greendot)
-000022d0: 0a20 2020 2020 2020 2073 656c 662e 7269  .        self.ri
-000022e0: 6768 7464 6f74 2e73 6574 5069 786d 6170  ghtdot.setPixmap
-000022f0: 2873 656c 662e 7265 6464 6f74 290a 0a20  (self.reddot).. 
-00002300: 2020 2020 2020 2073 656c 662e 4631 2e73         self.F1.s
-00002310: 6574 436f 6e74 6578 744d 656e 7550 6f6c  etContextMenuPol
-00002320: 6963 7928 5174 436f 7265 2e51 742e 4375  icy(QtCore.Qt.Cu
-00002330: 7374 6f6d 436f 6e74 6578 744d 656e 7529  stomContextMenu)
-00002340: 0a20 2020 2020 2020 2073 656c 662e 4631  .        self.F1
-00002350: 2e63 7573 746f 6d43 6f6e 7465 7874 4d65  .customContextMe
-00002360: 6e75 5265 7175 6573 7465 642e 636f 6e6e  nuRequested.conn
-00002370: 6563 7428 7365 6c66 2e65 6469 745f 4631  ect(self.edit_F1
-00002380: 290a 2020 2020 2020 2020 7365 6c66 2e46  ).        self.F
-00002390: 312e 636c 6963 6b65 642e 636f 6e6e 6563  1.clicked.connec
-000023a0: 7428 7365 6c66 2e73 656e 6466 3129 0a20  t(self.sendf1). 
-000023b0: 2020 2020 2020 2073 656c 662e 4632 2e73         self.F2.s
-000023c0: 6574 436f 6e74 6578 744d 656e 7550 6f6c  etContextMenuPol
-000023d0: 6963 7928 5174 436f 7265 2e51 742e 4375  icy(QtCore.Qt.Cu
-000023e0: 7374 6f6d 436f 6e74 6578 744d 656e 7529  stomContextMenu)
-000023f0: 0a20 2020 2020 2020 2073 656c 662e 4632  .        self.F2
-00002400: 2e63 7573 746f 6d43 6f6e 7465 7874 4d65  .customContextMe
-00002410: 6e75 5265 7175 6573 7465 642e 636f 6e6e  nuRequested.conn
-00002420: 6563 7428 7365 6c66 2e65 6469 745f 4632  ect(self.edit_F2
-00002430: 290a 2020 2020 2020 2020 7365 6c66 2e46  ).        self.F
-00002440: 322e 636c 6963 6b65 642e 636f 6e6e 6563  2.clicked.connec
-00002450: 7428 7365 6c66 2e73 656e 6466 3229 0a20  t(self.sendf2). 
-00002460: 2020 2020 2020 2073 656c 662e 4633 2e73         self.F3.s
-00002470: 6574 436f 6e74 6578 744d 656e 7550 6f6c  etContextMenuPol
-00002480: 6963 7928 5174 436f 7265 2e51 742e 4375  icy(QtCore.Qt.Cu
-00002490: 7374 6f6d 436f 6e74 6578 744d 656e 7529  stomContextMenu)
-000024a0: 0a20 2020 2020 2020 2073 656c 662e 4633  .        self.F3
-000024b0: 2e63 7573 746f 6d43 6f6e 7465 7874 4d65  .customContextMe
-000024c0: 6e75 5265 7175 6573 7465 642e 636f 6e6e  nuRequested.conn
-000024d0: 6563 7428 7365 6c66 2e65 6469 745f 4633  ect(self.edit_F3
-000024e0: 290a 2020 2020 2020 2020 7365 6c66 2e46  ).        self.F
-000024f0: 332e 636c 6963 6b65 642e 636f 6e6e 6563  3.clicked.connec
-00002500: 7428 7365 6c66 2e73 656e 6466 3329 0a20  t(self.sendf3). 
-00002510: 2020 2020 2020 2073 656c 662e 4634 2e73         self.F4.s
-00002520: 6574 436f 6e74 6578 744d 656e 7550 6f6c  etContextMenuPol
-00002530: 6963 7928 5174 436f 7265 2e51 742e 4375  icy(QtCore.Qt.Cu
-00002540: 7374 6f6d 436f 6e74 6578 744d 656e 7529  stomContextMenu)
-00002550: 0a20 2020 2020 2020 2073 656c 662e 4634  .        self.F4
-00002560: 2e63 7573 746f 6d43 6f6e 7465 7874 4d65  .customContextMe
-00002570: 6e75 5265 7175 6573 7465 642e 636f 6e6e  nuRequested.conn
-00002580: 6563 7428 7365 6c66 2e65 6469 745f 4634  ect(self.edit_F4
-00002590: 290a 2020 2020 2020 2020 7365 6c66 2e46  ).        self.F
-000025a0: 342e 636c 6963 6b65 642e 636f 6e6e 6563  4.clicked.connec
-000025b0: 7428 7365 6c66 2e73 656e 6466 3429 0a20  t(self.sendf4). 
-000025c0: 2020 2020 2020 2073 656c 662e 4635 2e73         self.F5.s
-000025d0: 6574 436f 6e74 6578 744d 656e 7550 6f6c  etContextMenuPol
-000025e0: 6963 7928 5174 436f 7265 2e51 742e 4375  icy(QtCore.Qt.Cu
-000025f0: 7374 6f6d 436f 6e74 6578 744d 656e 7529  stomContextMenu)
-00002600: 0a20 2020 2020 2020 2073 656c 662e 4635  .        self.F5
-00002610: 2e63 7573 746f 6d43 6f6e 7465 7874 4d65  .customContextMe
-00002620: 6e75 5265 7175 6573 7465 642e 636f 6e6e  nuRequested.conn
-00002630: 6563 7428 7365 6c66 2e65 6469 745f 4635  ect(self.edit_F5
-00002640: 290a 2020 2020 2020 2020 7365 6c66 2e46  ).        self.F
-00002650: 352e 636c 6963 6b65 642e 636f 6e6e 6563  5.clicked.connec
-00002660: 7428 7365 6c66 2e73 656e 6466 3529 0a20  t(self.sendf5). 
-00002670: 2020 2020 2020 2073 656c 662e 4636 2e73         self.F6.s
-00002680: 6574 436f 6e74 6578 744d 656e 7550 6f6c  etContextMenuPol
-00002690: 6963 7928 5174 436f 7265 2e51 742e 4375  icy(QtCore.Qt.Cu
-000026a0: 7374 6f6d 436f 6e74 6578 744d 656e 7529  stomContextMenu)
-000026b0: 0a20 2020 2020 2020 2073 656c 662e 4636  .        self.F6
-000026c0: 2e63 7573 746f 6d43 6f6e 7465 7874 4d65  .customContextMe
-000026d0: 6e75 5265 7175 6573 7465 642e 636f 6e6e  nuRequested.conn
-000026e0: 6563 7428 7365 6c66 2e65 6469 745f 4636  ect(self.edit_F6
-000026f0: 290a 2020 2020 2020 2020 7365 6c66 2e46  ).        self.F
-00002700: 362e 636c 6963 6b65 642e 636f 6e6e 6563  6.clicked.connec
-00002710: 7428 7365 6c66 2e73 656e 6466 3629 0a20  t(self.sendf6). 
-00002720: 2020 2020 2020 2073 656c 662e 4637 2e73         self.F7.s
-00002730: 6574 436f 6e74 6578 744d 656e 7550 6f6c  etContextMenuPol
-00002740: 6963 7928 5174 436f 7265 2e51 742e 4375  icy(QtCore.Qt.Cu
-00002750: 7374 6f6d 436f 6e74 6578 744d 656e 7529  stomContextMenu)
-00002760: 0a20 2020 2020 2020 2073 656c 662e 4637  .        self.F7
-00002770: 2e63 7573 746f 6d43 6f6e 7465 7874 4d65  .customContextMe
-00002780: 6e75 5265 7175 6573 7465 642e 636f 6e6e  nuRequested.conn
-00002790: 6563 7428 7365 6c66 2e65 6469 745f 4637  ect(self.edit_F7
-000027a0: 290a 2020 2020 2020 2020 7365 6c66 2e46  ).        self.F
-000027b0: 372e 636c 6963 6b65 642e 636f 6e6e 6563  7.clicked.connec
-000027c0: 7428 7365 6c66 2e73 656e 6466 3729 0a20  t(self.sendf7). 
-000027d0: 2020 2020 2020 2073 656c 662e 4638 2e73         self.F8.s
-000027e0: 6574 436f 6e74 6578 744d 656e 7550 6f6c  etContextMenuPol
-000027f0: 6963 7928 5174 436f 7265 2e51 742e 4375  icy(QtCore.Qt.Cu
-00002800: 7374 6f6d 436f 6e74 6578 744d 656e 7529  stomContextMenu)
-00002810: 0a20 2020 2020 2020 2073 656c 662e 4638  .        self.F8
-00002820: 2e63 7573 746f 6d43 6f6e 7465 7874 4d65  .customContextMe
-00002830: 6e75 5265 7175 6573 7465 642e 636f 6e6e  nuRequested.conn
-00002840: 6563 7428 7365 6c66 2e65 6469 745f 4638  ect(self.edit_F8
-00002850: 290a 2020 2020 2020 2020 7365 6c66 2e46  ).        self.F
-00002860: 382e 636c 6963 6b65 642e 636f 6e6e 6563  8.clicked.connec
-00002870: 7428 7365 6c66 2e73 656e 6466 3829 0a20  t(self.sendf8). 
-00002880: 2020 2020 2020 2073 656c 662e 4639 2e73         self.F9.s
-00002890: 6574 436f 6e74 6578 744d 656e 7550 6f6c  etContextMenuPol
-000028a0: 6963 7928 5174 436f 7265 2e51 742e 4375  icy(QtCore.Qt.Cu
-000028b0: 7374 6f6d 436f 6e74 6578 744d 656e 7529  stomContextMenu)
-000028c0: 0a20 2020 2020 2020 2073 656c 662e 4639  .        self.F9
-000028d0: 2e63 7573 746f 6d43 6f6e 7465 7874 4d65  .customContextMe
-000028e0: 6e75 5265 7175 6573 7465 642e 636f 6e6e  nuRequested.conn
-000028f0: 6563 7428 7365 6c66 2e65 6469 745f 4639  ect(self.edit_F9
-00002900: 290a 2020 2020 2020 2020 7365 6c66 2e46  ).        self.F
-00002910: 392e 636c 6963 6b65 642e 636f 6e6e 6563  9.clicked.connec
-00002920: 7428 7365 6c66 2e73 656e 6466 3929 0a20  t(self.sendf9). 
-00002930: 2020 2020 2020 2073 656c 662e 4631 302e         self.F10.
-00002940: 7365 7443 6f6e 7465 7874 4d65 6e75 506f  setContextMenuPo
-00002950: 6c69 6379 2851 7443 6f72 652e 5174 2e43  licy(QtCore.Qt.C
-00002960: 7573 746f 6d43 6f6e 7465 7874 4d65 6e75  ustomContextMenu
-00002970: 290a 2020 2020 2020 2020 7365 6c66 2e46  ).        self.F
-00002980: 3130 2e63 7573 746f 6d43 6f6e 7465 7874  10.customContext
-00002990: 4d65 6e75 5265 7175 6573 7465 642e 636f  MenuRequested.co
-000029a0: 6e6e 6563 7428 7365 6c66 2e65 6469 745f  nnect(self.edit_
-000029b0: 4631 3029 0a20 2020 2020 2020 2073 656c  F10).        sel
-000029c0: 662e 4631 302e 636c 6963 6b65 642e 636f  f.F10.clicked.co
-000029d0: 6e6e 6563 7428 7365 6c66 2e73 656e 6466  nnect(self.sendf
-000029e0: 3130 290a 2020 2020 2020 2020 7365 6c66  10).        self
-000029f0: 2e46 3131 2e73 6574 436f 6e74 6578 744d  .F11.setContextM
-00002a00: 656e 7550 6f6c 6963 7928 5174 436f 7265  enuPolicy(QtCore
-00002a10: 2e51 742e 4375 7374 6f6d 436f 6e74 6578  .Qt.CustomContex
-00002a20: 744d 656e 7529 0a20 2020 2020 2020 2073  tMenu).        s
-00002a30: 656c 662e 4631 312e 6375 7374 6f6d 436f  elf.F11.customCo
-00002a40: 6e74 6578 744d 656e 7552 6571 7565 7374  ntextMenuRequest
-00002a50: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
-00002a60: 6564 6974 5f46 3131 290a 2020 2020 2020  edit_F11).      
-00002a70: 2020 7365 6c66 2e46 3131 2e63 6c69 636b    self.F11.click
-00002a80: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
-00002a90: 7365 6e64 6631 3129 0a20 2020 2020 2020  sendf11).       
-00002aa0: 2073 656c 662e 4631 322e 7365 7443 6f6e   self.F12.setCon
-00002ab0: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
-00002ac0: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
-00002ad0: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
-00002ae0: 2020 2020 7365 6c66 2e46 3132 2e63 7573      self.F12.cus
-00002af0: 746f 6d43 6f6e 7465 7874 4d65 6e75 5265  tomContextMenuRe
-00002b00: 7175 6573 7465 642e 636f 6e6e 6563 7428  quested.connect(
-00002b10: 7365 6c66 2e65 6469 745f 4631 3229 0a20  self.edit_F12). 
-00002b20: 2020 2020 2020 2073 656c 662e 4631 322e         self.F12.
-00002b30: 636c 6963 6b65 642e 636f 6e6e 6563 7428  clicked.connect(
-00002b40: 7365 6c66 2e73 656e 6466 3132 290a 0a20  self.sendf12).. 
-00002b50: 2020 2020 2020 2073 656c 662e 7265 6164         self.read
-00002b60: 7072 6566 6572 656e 6365 7328 290a 2020  preferences().  
-00002b70: 2020 2020 2020 7365 6c66 2e64 626e 616d        self.dbnam
-00002b80: 6520 3d20 4441 5441 5f50 4154 4820 2b20  e = DATA_PATH + 
-00002b90: 222f 2220 2b20 7365 6c66 2e70 7265 662e  "/" + self.pref.
-00002ba0: 6765 7428 2263 7572 7265 6e74 5f64 6174  get("current_dat
-00002bb0: 6162 6173 6522 2c20 2268 616d 2e64 6222  abase", "ham.db"
-00002bc0: 290a 2020 2020 2020 2020 7365 6c66 2e64  ).        self.d
-00002bd0: 6174 6162 6173 6520 3d20 4461 7461 4261  atabase = DataBa
-00002be0: 7365 2873 656c 662e 6462 6e61 6d65 2c20  se(self.dbname, 
-00002bf0: 574f 524b 494e 475f 5041 5448 290a 2020  WORKING_PATH).  
-00002c00: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
-00002c10: 6f6e 203d 2073 656c 662e 6461 7461 6261  on = self.databa
-00002c20: 7365 2e66 6574 6368 5f73 7461 7469 6f6e  se.fetch_station
-00002c30: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-00002c40: 6c66 2e73 7461 7469 6f6e 2069 7320 4e6f  lf.station is No
-00002c50: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00002c60: 7365 6c66 2e73 7461 7469 6f6e 203d 207b  self.station = {
-00002c70: 7d0a 2020 2020 2020 2020 2020 2020 7365  }.            se
-00002c80: 6c66 2e65 6469 745f 7374 6174 696f 6e5f  lf.edit_station_
-00002c90: 7365 7474 696e 6773 2829 0a20 2020 2020  settings().     
-00002ca0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-00002cb0: 696f 6e20 3d20 7365 6c66 2e64 6174 6162  ion = self.datab
-00002cc0: 6173 652e 6665 7463 685f 7374 6174 696f  ase.fetch_statio
-00002cd0: 6e28 290a 2020 2020 2020 2020 2020 2020  n().            
-00002ce0: 6966 2073 656c 662e 7374 6174 696f 6e20  if self.station 
-00002cf0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00002d00: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
-00002d10: 6174 696f 6e20 3d20 7b7d 0a20 2020 2020  ation = {}.     
-00002d20: 2020 2073 656c 662e 636f 6e74 6163 7420     self.contact 
-00002d30: 3d20 7365 6c66 2e64 6174 6162 6173 652e  = self.database.
-00002d40: 656d 7074 795f 636f 6e74 6163 740a 2020  empty_contact.  
-00002d50: 2020 2020 2020 7365 6c66 2e63 7572 7265        self.curre
-00002d60: 6e74 5f6f 7020 3d20 7365 6c66 2e73 7461  nt_op = self.sta
-00002d70: 7469 6f6e 2e67 6574 2822 4361 6c6c 222c  tion.get("Call",
-00002d80: 2022 2229 0a20 2020 2020 2020 2073 656c   "").        sel
-00002d90: 662e 6d61 6b65 5f6f 705f 6469 7228 290a  f.make_op_dir().
-00002da0: 2020 2020 2020 2020 7365 6c66 2e72 6561          self.rea
-00002db0: 645f 6377 5f6d 6163 726f 7328 290a 2020  d_cw_macros().  
-00002dc0: 2020 2020 2020 7365 6c66 2e63 6c65 6172        self.clear
-00002dd0: 696e 7075 7473 2829 0a0a 2020 2020 2020  inputs()..      
-00002de0: 2020 7365 6c66 2e62 616e 645f 696e 6469    self.band_indi
-00002df0: 6361 746f 7273 5f63 7720 3d20 7b0a 2020  cators_cw = {.  
-00002e00: 2020 2020 2020 2020 2020 2231 3630 223a            "160":
-00002e10: 2073 656c 662e 6377 5f62 616e 645f 3136   self.cw_band_16
-00002e20: 302c 0a20 2020 2020 2020 2020 2020 2022  0,.            "
-00002e30: 3830 223a 2073 656c 662e 6377 5f62 616e  80": self.cw_ban
-00002e40: 645f 3830 2c0a 2020 2020 2020 2020 2020  d_80,.          
-00002e50: 2020 2234 3022 3a20 7365 6c66 2e63 775f    "40": self.cw_
-00002e60: 6261 6e64 5f34 302c 0a20 2020 2020 2020  band_40,.       
-00002e70: 2020 2020 2022 3230 223a 2073 656c 662e       "20": self.
-00002e80: 6377 5f62 616e 645f 3230 2c0a 2020 2020  cw_band_20,.    
-00002e90: 2020 2020 2020 2020 2231 3522 3a20 7365          "15": se
-00002ea0: 6c66 2e63 775f 6261 6e64 5f31 352c 0a20  lf.cw_band_15,. 
-00002eb0: 2020 2020 2020 2020 2020 2022 3130 223a             "10":
-00002ec0: 2073 656c 662e 6377 5f62 616e 645f 3130   self.cw_band_10
-00002ed0: 2c0a 2020 2020 2020 2020 7d0a 0a20 2020  ,.        }..   
-00002ee0: 2020 2020 2073 656c 662e 6261 6e64 5f69       self.band_i
-00002ef0: 6e64 6963 6174 6f72 735f 7373 6220 3d20  ndicators_ssb = 
-00002f00: 7b0a 2020 2020 2020 2020 2020 2020 2231  {.            "1
-00002f10: 3630 223a 2073 656c 662e 7373 625f 6261  60": self.ssb_ba
-00002f20: 6e64 5f31 3630 2c0a 2020 2020 2020 2020  nd_160,.        
-00002f30: 2020 2020 2238 3022 3a20 7365 6c66 2e73      "80": self.s
-00002f40: 7362 5f62 616e 645f 3830 2c0a 2020 2020  sb_band_80,.    
-00002f50: 2020 2020 2020 2020 2234 3022 3a20 7365          "40": se
-00002f60: 6c66 2e73 7362 5f62 616e 645f 3430 2c0a  lf.ssb_band_40,.
-00002f70: 2020 2020 2020 2020 2020 2020 2232 3022              "20"
-00002f80: 3a20 7365 6c66 2e73 7362 5f62 616e 645f  : self.ssb_band_
-00002f90: 3230 2c0a 2020 2020 2020 2020 2020 2020  20,.            
-00002fa0: 2231 3522 3a20 7365 6c66 2e73 7362 5f62  "15": self.ssb_b
-00002fb0: 616e 645f 3135 2c0a 2020 2020 2020 2020  and_15,.        
-00002fc0: 2020 2020 2231 3022 3a20 7365 6c66 2e73      "10": self.s
-00002fd0: 7362 5f62 616e 645f 3130 2c0a 2020 2020  sb_band_10,.    
-00002fe0: 2020 2020 7d0a 0a20 2020 2020 2020 2073      }..        s
-00002ff0: 656c 662e 6261 6e64 5f69 6e64 6963 6174  elf.band_indicat
-00003000: 6f72 735f 7274 7479 203d 207b 0a20 2020  ors_rtty = {.   
-00003010: 2020 2020 2020 2020 2022 3136 3022 3a20           "160": 
-00003020: 7365 6c66 2e72 7474 795f 6261 6e64 5f31  self.rtty_band_1
-00003030: 3630 2c0a 2020 2020 2020 2020 2020 2020  60,.            
-00003040: 2238 3022 3a20 7365 6c66 2e72 7474 795f  "80": self.rtty_
-00003050: 6261 6e64 5f38 302c 0a20 2020 2020 2020  band_80,.       
-00003060: 2020 2020 2022 3430 223a 2073 656c 662e       "40": self.
-00003070: 7274 7479 5f62 616e 645f 3430 2c0a 2020  rtty_band_40,.  
-00003080: 2020 2020 2020 2020 2020 2232 3022 3a20            "20": 
-00003090: 7365 6c66 2e72 7474 795f 6261 6e64 5f32  self.rtty_band_2
-000030a0: 302c 0a20 2020 2020 2020 2020 2020 2022  0,.            "
-000030b0: 3135 223a 2073 656c 662e 7274 7479 5f62  15": self.rtty_b
-000030c0: 616e 645f 3135 2c0a 2020 2020 2020 2020  and_15,.        
-000030d0: 2020 2020 2231 3022 3a20 7365 6c66 2e72      "10": self.r
-000030e0: 7474 795f 6261 6e64 5f31 302c 0a20 2020  tty_band_10,.   
-000030f0: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
-00003100: 7365 6c66 2e61 6c6c 5f6d 6f64 655f 696e  self.all_mode_in
-00003110: 6469 6361 746f 7273 203d 207b 0a20 2020  dicators = {.   
-00003120: 2020 2020 2020 2020 2022 4357 223a 2073           "CW": s
-00003130: 656c 662e 6261 6e64 5f69 6e64 6963 6174  elf.band_indicat
-00003140: 6f72 735f 6377 2c0a 2020 2020 2020 2020  ors_cw,.        
-00003150: 2020 2020 2253 5342 223a 2073 656c 662e      "SSB": self.
-00003160: 6261 6e64 5f69 6e64 6963 6174 6f72 735f  band_indicators_
-00003170: 7373 622c 0a20 2020 2020 2020 2020 2020  ssb,.           
-00003180: 2022 5254 5459 223a 2073 656c 662e 6261   "RTTY": self.ba
-00003190: 6e64 5f69 6e64 6963 6174 6f72 735f 7274  nd_indicators_rt
-000031a0: 7479 2c0a 2020 2020 2020 2020 7d0a 0a20  ty,.        }.. 
-000031b0: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-000031c0: 7265 662e 6765 7428 2263 6f6e 7465 7374  ref.get("contest
-000031d0: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-000031e0: 7365 6c66 2e6c 6f61 645f 636f 6e74 6573  self.load_contes
-000031f0: 7428 290a 0a20 2020 2020 2020 2069 6620  t()..        if 
-00003200: 5665 7273 696f 6e54 6573 7428 5f5f 7665  VersionTest(__ve
-00003210: 7273 696f 6e5f 5f29 2e74 6573 7428 293a  rsion__).test():
-00003220: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00003230: 662e 7368 6f77 5f6d 6573 7361 6765 5f62  f.show_message_b
-00003240: 6f78 280a 2020 2020 2020 2020 2020 2020  ox(.            
-00003250: 2020 2020 2254 6865 7265 2069 7320 6120      "There is a 
-00003260: 6e65 7765 7220 7665 7273 696f 6e20 6f66  newer version of
-00003270: 206e 6f74 316d 6d20 6176 6169 6c61 626c   not1mm availabl
-00003280: 652e 5c6e 220a 2020 2020 2020 2020 2020  e.\n".          
-00003290: 2020 2020 2020 2259 6f75 2063 616e 2075        "You can u
-000032a0: 6461 7465 2074 6f20 7468 6520 6375 7272  date to the curr
-000032b0: 656e 7420 7665 7273 696f 6e20 6279 2075  ent version by u
-000032c0: 7369 6e67 3a5c 6e70 6970 2069 6e73 7461  sing:\npip insta
-000032d0: 6c6c 202d 5520 6e6f 7431 6d6d 220a 2020  ll -U not1mm".  
-000032e0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-000032f0: 2064 6566 2071 7569 745f 6170 7028 7365   def quit_app(se
-00003300: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00003310: 646f 6322 2222 0a20 2020 2020 2020 2063  doc""".        c
-00003320: 6d64 203d 207b 7d0a 2020 2020 2020 2020  md = {}.        
-00003330: 636d 645b 2263 6d64 225d 203d 2022 4841  cmd["cmd"] = "HA
-00003340: 4c54 220a 2020 2020 2020 2020 636d 645b  LT".        cmd[
-00003350: 2273 7461 7469 6f6e 225d 203d 2070 6c61  "station"] = pla
-00003360: 7466 6f72 6d2e 6e6f 6465 2829 0a20 2020  tform.node().   
-00003370: 2020 2020 2073 656c 662e 6d75 6c74 6963       self.multic
-00003380: 6173 745f 696e 7465 7266 6163 652e 7365  ast_interface.se
-00003390: 6e64 5f61 735f 6a73 6f6e 2863 6d64 290a  nd_as_json(cmd).
-000033a0: 2020 2020 2020 2020 6170 702e 7175 6974          app.quit
-000033b0: 2829 0a0a 2020 2020 4073 7461 7469 636d  ()..    @staticm
-000033c0: 6574 686f 640a 2020 2020 6465 6620 6368  ethod.    def ch
-000033d0: 6563 6b5f 7072 6f63 6573 7328 6e61 6d65  eck_process(name
-000033e0: 3a20 7374 7229 202d 3e20 626f 6f6c 3a0a  : str) -> bool:.
-000033f0: 2020 2020 2020 2020 2222 2263 6865 636b          """check
-00003400: 7320 746f 2073 6565 2069 6620 7072 6f67  s to see if prog
-00003410: 7261 6d20 6f66 206e 616d 6520 6973 2069  ram of name is i
-00003420: 6e20 7468 6520 6163 7469 7665 2070 726f  n the active pro
-00003430: 6365 7373 206c 6973 7422 2222 0a20 2020  cess list""".   
-00003440: 2020 2020 2066 6f72 2070 726f 6320 696e       for proc in
-00003450: 2070 7375 7469 6c2e 7072 6f63 6573 735f   psutil.process_
-00003460: 6974 6572 2829 3a0a 2020 2020 2020 2020  iter():.        
-00003470: 2020 2020 6966 2062 6f6f 6c28 7265 2e6d      if bool(re.m
-00003480: 6174 6368 286e 616d 652c 2070 726f 632e  atch(name, proc.
-00003490: 6e61 6d65 2829 2e6c 6f77 6572 2829 2929  name().lower()))
-000034a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000034b0: 2020 7265 7475 726e 2054 7275 650a 2020    return True.  
-000034c0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-000034d0: 7365 0a0a 2020 2020 6465 6620 7368 6f77  se..    def show
-000034e0: 5f6d 6573 7361 6765 5f62 6f78 2873 656c  _message_box(sel
-000034f0: 662c 206d 6573 7361 6765 3a20 7374 7229  f, message: str)
-00003500: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00003510: 2020 2222 2264 6f63 2222 220a 2020 2020    """doc""".    
-00003520: 2020 2020 6d65 7373 6167 655f 626f 7820      message_box 
-00003530: 3d20 5174 5769 6467 6574 732e 514d 6573  = QtWidgets.QMes
-00003540: 7361 6765 426f 7828 290a 2020 2020 2020  sageBox().      
-00003550: 2020 6d65 7373 6167 655f 626f 782e 7365    message_box.se
-00003560: 7449 636f 6e28 5174 5769 6467 6574 732e  tIcon(QtWidgets.
-00003570: 514d 6573 7361 6765 426f 782e 496e 666f  QMessageBox.Info
-00003580: 726d 6174 696f 6e29 0a20 2020 2020 2020  rmation).       
-00003590: 206d 6573 7361 6765 5f62 6f78 2e73 6574   message_box.set
-000035a0: 5465 7874 286d 6573 7361 6765 290a 2020  Text(message).  
-000035b0: 2020 2020 2020 6d65 7373 6167 655f 626f        message_bo
-000035c0: 782e 7365 7457 696e 646f 7754 6974 6c65  x.setWindowTitle
-000035d0: 2822 496e 666f 726d 6174 696f 6e22 290a  ("Information").
-000035e0: 2020 2020 2020 2020 6d65 7373 6167 655f          message_
-000035f0: 626f 782e 7365 7453 7461 6e64 6172 6442  box.setStandardB
-00003600: 7574 746f 6e73 2851 7457 6964 6765 7473  uttons(QtWidgets
-00003610: 2e51 4d65 7373 6167 6542 6f78 2e4f 6b29  .QMessageBox.Ok)
-00003620: 0a20 2020 2020 2020 205f 203d 206d 6573  .        _ = mes
-00003630: 7361 6765 5f62 6f78 2e65 7865 635f 2829  sage_box.exec_()
-00003640: 0a0a 2020 2020 6465 6620 7368 6f77 5f61  ..    def show_a
-00003650: 626f 7574 5f64 6961 6c6f 6728 7365 6c66  bout_dialog(self
-00003660: 293a 0a20 2020 2020 2020 2022 2222 5368  ):.        """Sh
-00003670: 6f77 2061 626f 7574 2064 6961 6c6f 6722  ow about dialog"
-00003680: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
-00003690: 6162 6f75 745f 6469 616c 6f67 203d 2041  about_dialog = A
-000036a0: 626f 7574 2857 4f52 4b49 4e47 5f50 4154  bout(WORKING_PAT
-000036b0: 4829 0a20 2020 2020 2020 2073 656c 662e  H).        self.
-000036c0: 6162 6f75 745f 6469 616c 6f67 2e64 6f6e  about_dialog.don
-000036d0: 6f72 732e 7365 7453 6f75 7263 6528 0a20  ors.setSource(. 
-000036e0: 2020 2020 2020 2020 2020 2051 7443 6f72             QtCor
-000036f0: 652e 5155 726c 2e66 726f 6d4c 6f63 616c  e.QUrl.fromLocal
-00003700: 4669 6c65 2857 4f52 4b49 4e47 5f50 4154  File(WORKING_PAT
-00003710: 4820 2b20 222f 6461 7461 2f64 6f6e 6f72  H + "/data/donor
-00003720: 732e 6874 6d6c 2229 0a20 2020 2020 2020  s.html").       
-00003730: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
-00003740: 6162 6f75 745f 6469 616c 6f67 2e6f 7065  about_dialog.ope
-00003750: 6e28 290a 0a20 2020 2064 6566 2073 686f  n()..    def sho
-00003760: 775f 6865 6c70 5f64 6961 6c6f 6728 7365  w_help_dialog(se
-00003770: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00003780: 5368 6f77 2061 626f 7574 2064 6961 6c6f  Show about dialo
-00003790: 6722 2222 0a20 2020 2020 2020 2073 656c  g""".        sel
-000037a0: 662e 6162 6f75 745f 6469 616c 6f67 203d  f.about_dialog =
-000037b0: 2041 626f 7574 2857 4f52 4b49 4e47 5f50   About(WORKING_P
-000037c0: 4154 4829 0a20 2020 2020 2020 2073 656c  ATH).        sel
-000037d0: 662e 6162 6f75 745f 6469 616c 6f67 2e73  f.about_dialog.s
-000037e0: 6574 5769 6e64 6f77 5469 746c 6528 2248  etWindowTitle("H
-000037f0: 656c 7022 290a 2020 2020 2020 2020 7365  elp").        se
-00003800: 6c66 2e61 626f 7574 5f64 6961 6c6f 672e  lf.about_dialog.
-00003810: 7365 7447 656f 6d65 7472 7928 302c 2030  setGeometry(0, 0
-00003820: 2c20 3830 302c 2036 3030 290a 2020 2020  , 800, 600).    
-00003830: 2020 2020 7365 6c66 2e61 626f 7574 5f64      self.about_d
-00003840: 6961 6c6f 672e 646f 6e6f 7273 2e73 6574  ialog.donors.set
-00003850: 536f 7572 6365 280a 2020 2020 2020 2020  Source(.        
-00003860: 2020 2020 5174 436f 7265 2e51 5572 6c2e      QtCore.QUrl.
-00003870: 6672 6f6d 4c6f 6361 6c46 696c 6528 574f  fromLocalFile(WO
-00003880: 524b 494e 475f 5041 5448 202b 2022 2f64  RKING_PATH + "/d
-00003890: 6174 612f 6e6f 7431 6d6d 2e68 746d 6c22  ata/not1mm.html"
-000038a0: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
-000038b0: 2020 2020 7365 6c66 2e61 626f 7574 5f64      self.about_d
-000038c0: 6961 6c6f 672e 6f70 656e 2829 0a0a 2020  ialog.open()..  
-000038d0: 2020 6465 6620 7570 6461 7465 5f6d 6173    def update_mas
-000038e0: 7465 7273 6370 2873 656c 6629 202d 3e20  terscp(self) -> 
-000038f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-00003900: 2255 7064 6174 6520 7468 6520 4d41 5354  "Update the MAST
-00003910: 4552 2e53 4350 2066 696c 652e 2222 220a  ER.SCP file.""".
-00003920: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00003930: 6d73 6370 2e75 7064 6174 655f 6d61 7374  mscp.update_mast
-00003940: 6572 7363 7028 293a 0a20 2020 2020 2020  erscp():.       
-00003950: 2020 2020 2073 656c 662e 7368 6f77 5f6d       self.show_m
-00003960: 6573 7361 6765 5f62 6f78 2822 4d41 5354  essage_box("MAST
-00003970: 4552 2e53 4350 2066 696c 6520 7570 6461  ER.SCP file upda
-00003980: 7465 642e 2229 0a20 2020 2020 2020 2020  ted.").         
-00003990: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-000039a0: 2020 7365 6c66 2e73 686f 775f 6d65 7373    self.show_mess
-000039b0: 6167 655f 626f 7828 224d 4153 5445 522e  age_box("MASTER.
-000039c0: 5343 5020 636f 756c 6420 6e6f 7420 6265  SCP could not be
-000039d0: 2075 7064 6174 6564 2e22 290a 0a20 2020   updated.")..   
-000039e0: 2064 6566 2065 6469 745f 636f 6e66 6967   def edit_config
-000039f0: 7572 6174 696f 6e5f 7365 7474 696e 6773  uration_settings
-00003a00: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00003a10: 2222 2243 6f6e 6669 6775 7261 7469 6f6e  """Configuration
-00003a20: 2053 6574 7469 6e67 7320 7761 7320 636c   Settings was cl
-00003a30: 6963 6b65 6422 2222 0a20 2020 2020 2020  icked""".       
-00003a40: 2073 656c 662e 636f 6e66 6967 7572 6174   self.configurat
-00003a50: 696f 6e5f 6469 616c 6f67 203d 2053 6574  ion_dialog = Set
-00003a60: 7469 6e67 7328 574f 524b 494e 475f 5041  tings(WORKING_PA
-00003a70: 5448 2c20 434f 4e46 4947 5f50 4154 482c  TH, CONFIG_PATH,
-00003a80: 2073 656c 662e 7072 6566 290a 2020 2020   self.pref).    
-00003a90: 2020 2020 7365 6c66 2e63 6f6e 6669 6775      self.configu
-00003aa0: 7261 7469 6f6e 5f64 6961 6c6f 672e 7573  ration_dialog.us
-00003ab0: 6568 616d 6462 5f72 6164 696f 4275 7474  ehamdb_radioButt
-00003ac0: 6f6e 2e68 6964 6528 290a 2020 2020 2020  on.hide().      
-00003ad0: 2020 7365 6c66 2e63 6f6e 6669 6775 7261    self.configura
-00003ae0: 7469 6f6e 5f64 6961 6c6f 672e 7368 6f77  tion_dialog.show
-00003af0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-00003b00: 636f 6e66 6967 7572 6174 696f 6e5f 6469  configuration_di
-00003b10: 616c 6f67 2e61 6363 6570 7465 642e 636f  alog.accepted.co
-00003b20: 6e6e 6563 7428 7365 6c66 2e65 6469 745f  nnect(self.edit_
-00003b30: 636f 6e66 6967 7572 6174 696f 6e5f 7265  configuration_re
-00003b40: 7475 726e 290a 0a20 2020 2064 6566 2065  turn)..    def e
-00003b50: 6469 745f 636f 6e66 6967 7572 6174 696f  dit_configuratio
-00003b60: 6e5f 7265 7475 726e 2873 656c 6629 3a0a  n_return(self):.
-00003b70: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
-00003b80: 6e73 2068 6572 6520 7768 656e 2063 6f6e  ns here when con
-00003b90: 6669 6775 7261 7469 6f6e 2064 6961 6c6f  figuration dialo
-00003ba0: 6720 636c 6f73 6564 2077 6974 6820 6f6b  g closed with ok
-00003bb0: 6179 2e22 2222 0a20 2020 2020 2020 2073  ay.""".        s
-00003bc0: 656c 662e 636f 6e66 6967 7572 6174 696f  elf.configuratio
-00003bd0: 6e5f 6469 616c 6f67 2e73 6176 655f 6368  n_dialog.save_ch
-00003be0: 616e 6765 7328 290a 2020 2020 2020 2020  anges().        
-00003bf0: 7365 6c66 2e77 7269 7465 5f70 7265 6665  self.write_prefe
-00003c00: 7265 6e63 6528 290a 2020 2020 2020 2020  rence().        
-00003c10: 6c6f 6767 6572 2e64 6562 7567 2822 2573  logger.debug("%s
-00003c20: 222c 2066 227b 7365 6c66 2e70 7265 667d  ", f"{self.pref}
-00003c30: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-00003c40: 7265 6164 7072 6566 6572 656e 6365 7328  readpreferences(
-00003c50: 290a 0a20 2020 2064 6566 206e 6577 5f64  )..    def new_d
-00003c60: 6174 6162 6173 6528 7365 6c66 293a 0a20  atabase(self):. 
-00003c70: 2020 2020 2020 2022 2222 4372 6561 7465         """Create
-00003c80: 206e 6577 2064 6174 6162 6173 652e 2222   new database.""
-00003c90: 220a 2020 2020 2020 2020 6669 6c65 6e61  ".        filena
-00003ca0: 6d65 203d 2073 656c 662e 6669 6c65 7069  me = self.filepi
-00003cb0: 636b 6572 2822 6e65 7722 290a 2020 2020  cker("new").    
-00003cc0: 2020 2020 6966 2066 696c 656e 616d 653a      if filename:
-00003cd0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00003ce0: 6669 6c65 6e61 6d65 5b2d 333a 5d20 213d  filename[-3:] !=
-00003cf0: 2022 2e64 6222 3a0a 2020 2020 2020 2020   ".db":.        
-00003d00: 2020 2020 2020 2020 6669 6c65 6e61 6d65          filename
-00003d10: 202b 3d20 222e 6462 220a 2020 2020 2020   += ".db".      
-00003d20: 2020 2020 2020 7365 6c66 2e70 7265 665b        self.pref[
-00003d30: 2263 7572 7265 6e74 5f64 6174 6162 6173  "current_databas
-00003d40: 6522 5d20 3d20 6669 6c65 6e61 6d65 2e73  e"] = filename.s
-00003d50: 706c 6974 2822 2f22 295b 2d31 3a5d 5b30  plit("/")[-1:][0
-00003d60: 5d0a 2020 2020 2020 2020 2020 2020 7365  ].            se
-00003d70: 6c66 2e77 7269 7465 5f70 7265 6665 7265  lf.write_prefere
-00003d80: 6e63 6528 290a 2020 2020 2020 2020 2020  nce().          
-00003d90: 2020 7365 6c66 2e64 626e 616d 6520 3d20    self.dbname = 
-00003da0: 4441 5441 5f50 4154 4820 2b20 222f 2220  DATA_PATH + "/" 
-00003db0: 2b20 7365 6c66 2e70 7265 662e 6765 7428  + self.pref.get(
-00003dc0: 2263 7572 7265 6e74 5f64 6174 6162 6173  "current_databas
-00003dd0: 6522 2c20 2268 616d 2e64 6222 290a 2020  e", "ham.db").  
-00003de0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-00003df0: 6174 6162 6173 6520 3d20 4461 7461 4261  atabase = DataBa
-00003e00: 7365 2873 656c 662e 6462 6e61 6d65 2c20  se(self.dbname, 
-00003e10: 574f 524b 494e 475f 5041 5448 290a 2020  WORKING_PATH).  
-00003e20: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00003e30: 6f6e 7461 6374 203d 2073 656c 662e 6461  ontact = self.da
-00003e40: 7461 6261 7365 2e65 6d70 7479 5f63 6f6e  tabase.empty_con
-00003e50: 7461 6374 0a20 2020 2020 2020 2020 2020  tact.           
-00003e60: 2073 656c 662e 7374 6174 696f 6e20 3d20   self.station = 
-00003e70: 7365 6c66 2e64 6174 6162 6173 652e 6665  self.database.fe
-00003e80: 7463 685f 7374 6174 696f 6e28 290a 2020  tch_station().  
-00003e90: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00003ea0: 662e 7374 6174 696f 6e20 6973 204e 6f6e  f.station is Non
-00003eb0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00003ec0: 2020 2073 656c 662e 7374 6174 696f 6e20     self.station 
-00003ed0: 3d20 7b7d 0a20 2020 2020 2020 2020 2020  = {}.           
-00003ee0: 2073 656c 662e 6375 7272 656e 745f 6f70   self.current_op
-00003ef0: 203d 2073 656c 662e 7374 6174 696f 6e2e   = self.station.
-00003f00: 6765 7428 2243 616c 6c22 2c20 2222 290a  get("Call", "").
-00003f10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00003f20: 2e6d 616b 655f 6f70 5f64 6972 2829 0a20  .make_op_dir(). 
-00003f30: 2020 2020 2020 2020 2020 2063 6d64 203d             cmd =
-00003f40: 207b 7d0a 2020 2020 2020 2020 2020 2020   {}.            
-00003f50: 636d 645b 2263 6d64 225d 203d 2022 4e45  cmd["cmd"] = "NE
-00003f60: 5744 4222 0a20 2020 2020 2020 2020 2020  WDB".           
-00003f70: 2063 6d64 5b22 7374 6174 696f 6e22 5d20   cmd["station"] 
-00003f80: 3d20 706c 6174 666f 726d 2e6e 6f64 6528  = platform.node(
-00003f90: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00003fa0: 6c66 2e6d 756c 7469 6361 7374 5f69 6e74  lf.multicast_int
-00003fb0: 6572 6661 6365 2e73 656e 645f 6173 5f6a  erface.send_as_j
-00003fc0: 736f 6e28 636d 6429 0a20 2020 2020 2020  son(cmd).       
-00003fd0: 2020 2020 2073 656c 662e 636c 6561 7269       self.cleari
-00003fe0: 6e70 7574 7328 290a 2020 2020 2020 2020  nputs().        
-00003ff0: 2020 2020 7365 6c66 2e65 6469 745f 7374      self.edit_st
-00004000: 6174 696f 6e5f 7365 7474 696e 6773 2829  ation_settings()
-00004010: 0a0a 2020 2020 6465 6620 6f70 656e 5f64  ..    def open_d
-00004020: 6174 6162 6173 6528 7365 6c66 293a 0a20  atabase(self):. 
-00004030: 2020 2020 2020 2022 2222 4f70 656e 2065         """Open e
-00004040: 7869 7374 696e 6720 6461 7461 6261 7365  xisting database
-00004050: 2e22 2222 0a20 2020 2020 2020 2066 696c  .""".        fil
-00004060: 656e 616d 6520 3d20 7365 6c66 2e66 696c  ename = self.fil
-00004070: 6570 6963 6b65 7228 226f 7065 6e22 290a  epicker("open").
-00004080: 2020 2020 2020 2020 6966 2066 696c 656e          if filen
-00004090: 616d 653a 0a20 2020 2020 2020 2020 2020  ame:.           
-000040a0: 2073 656c 662e 7072 6566 5b22 6375 7272   self.pref["curr
-000040b0: 656e 745f 6461 7461 6261 7365 225d 203d  ent_database"] =
-000040c0: 2066 696c 656e 616d 652e 7370 6c69 7428   filename.split(
-000040d0: 222f 2229 5b2d 313a 5d5b 305d 0a20 2020  "/")[-1:][0].   
-000040e0: 2020 2020 2020 2020 2073 656c 662e 7772           self.wr
-000040f0: 6974 655f 7072 6566 6572 656e 6365 2829  ite_preference()
-00004100: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00004110: 662e 6462 6e61 6d65 203d 2044 4154 415f  f.dbname = DATA_
-00004120: 5041 5448 202b 2022 2f22 202b 2073 656c  PATH + "/" + sel
-00004130: 662e 7072 6566 2e67 6574 2822 6375 7272  f.pref.get("curr
-00004140: 656e 745f 6461 7461 6261 7365 222c 2022  ent_database", "
-00004150: 6861 6d2e 6462 2229 0a20 2020 2020 2020  ham.db").       
-00004160: 2020 2020 2073 656c 662e 6461 7461 6261       self.databa
-00004170: 7365 203d 2044 6174 6142 6173 6528 7365  se = DataBase(se
-00004180: 6c66 2e64 626e 616d 652c 2057 4f52 4b49  lf.dbname, WORKI
-00004190: 4e47 5f50 4154 4829 0a20 2020 2020 2020  NG_PATH).       
-000041a0: 2020 2020 2073 656c 662e 636f 6e74 6163       self.contac
-000041b0: 7420 3d20 7365 6c66 2e64 6174 6162 6173  t = self.databas
-000041c0: 652e 656d 7074 795f 636f 6e74 6163 740a  e.empty_contact.
-000041d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000041e0: 2e73 7461 7469 6f6e 203d 2073 656c 662e  .station = self.
-000041f0: 6461 7461 6261 7365 2e66 6574 6368 5f73  database.fetch_s
-00004200: 7461 7469 6f6e 2829 0a20 2020 2020 2020  tation().       
-00004210: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
-00004220: 7469 6f6e 2069 7320 4e6f 6e65 3a0a 2020  tion is None:.  
-00004230: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00004240: 6c66 2e73 7461 7469 6f6e 203d 207b 7d0a  lf.station = {}.
-00004250: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00004260: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
-00004270: 2243 616c 6c22 2c20 2222 2920 3d3d 2022  "Call", "") == "
-00004280: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-00004290: 2020 2073 656c 662e 6564 6974 5f73 7461     self.edit_sta
-000042a0: 7469 6f6e 5f73 6574 7469 6e67 7328 290a  tion_settings().
-000042b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000042c0: 2e63 7572 7265 6e74 5f6f 7020 3d20 7365  .current_op = se
-000042d0: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
-000042e0: 4361 6c6c 222c 2022 2229 0a20 2020 2020  Call", "").     
-000042f0: 2020 2020 2020 2073 656c 662e 6d61 6b65         self.make
-00004300: 5f6f 705f 6469 7228 290a 2020 2020 2020  _op_dir().      
-00004310: 2020 2020 2020 636d 6420 3d20 7b7d 0a20        cmd = {}. 
-00004320: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
-00004330: 636d 6422 5d20 3d20 224e 4557 4442 220a  cmd"] = "NEWDB".
-00004340: 2020 2020 2020 2020 2020 2020 636d 645b              cmd[
-00004350: 2273 7461 7469 6f6e 225d 203d 2070 6c61  "station"] = pla
-00004360: 7466 6f72 6d2e 6e6f 6465 2829 0a20 2020  tform.node().   
-00004370: 2020 2020 2020 2020 2073 656c 662e 6d75           self.mu
-00004380: 6c74 6963 6173 745f 696e 7465 7266 6163  lticast_interfac
-00004390: 652e 7365 6e64 5f61 735f 6a73 6f6e 2863  e.send_as_json(c
-000043a0: 6d64 290a 2020 2020 2020 2020 2020 2020  md).            
-000043b0: 7365 6c66 2e63 6c65 6172 696e 7075 7473  self.clearinputs
-000043c0: 2829 0a0a 2020 2020 6465 6620 6e65 775f  ()..    def new_
-000043d0: 636f 6e74 6573 7428 7365 6c66 293a 0a20  contest(self):. 
-000043e0: 2020 2020 2020 2022 2222 4372 6561 7465         """Create
-000043f0: 206e 6577 2063 6f6e 7465 7374 2069 6e20   new contest in 
-00004400: 6578 6973 7469 6e67 2064 6174 6162 6173  existing databas
-00004410: 652e 2222 220a 0a20 2020 2064 6566 206f  e."""..    def o
-00004420: 7065 6e5f 636f 6e74 6573 7428 7365 6c66  pen_contest(self
-00004430: 293a 0a20 2020 2020 2020 2022 2222 5377  ):.        """Sw
-00004440: 6974 6368 2074 6f20 6120 6469 6666 6572  itch to a differ
-00004450: 656e 7420 6578 6973 7469 6e67 2063 6f6e  ent existing con
-00004460: 7465 7374 2069 6e20 6578 6973 7469 6e67  test in existing
-00004470: 2064 6174 6162 6173 652e 2222 220a 2020   database.""".  
-00004480: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-00004490: 7567 2822 4f70 656e 2043 6f6e 7465 7374  ug("Open Contest
-000044a0: 2073 656c 6563 7465 6422 290a 2020 2020   selected").    
-000044b0: 2020 2020 636f 6e74 6573 7473 203d 2073      contests = s
-000044c0: 656c 662e 6461 7461 6261 7365 2e66 6574  elf.database.fet
-000044d0: 6368 5f61 6c6c 5f63 6f6e 7465 7374 7328  ch_all_contests(
-000044e0: 290a 2020 2020 2020 2020 6c6f 6767 6572  ).        logger
-000044f0: 2e64 6562 7567 2822 2573 222c 2066 227b  .debug("%s", f"{
-00004500: 636f 6e74 6573 7473 7d22 290a 0a20 2020  contests}")..   
-00004510: 2020 2020 2069 6620 636f 6e74 6573 7473       if contests
-00004520: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00004530: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-00004540: 6720 3d20 5365 6c65 6374 436f 6e74 6573  g = SelectContes
-00004550: 7428 574f 524b 494e 475f 5041 5448 290a  t(WORKING_PATH).
-00004560: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00004570: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
-00004580: 636f 6e74 6573 745f 6c69 7374 2e73 6574  contest_list.set
-00004590: 526f 7743 6f75 6e74 2830 290a 2020 2020  RowCount(0).    
-000045a0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-000045b0: 7465 7374 5f64 6961 6c6f 672e 636f 6e74  test_dialog.cont
-000045c0: 6573 745f 6c69 7374 2e73 6574 436f 6c75  est_list.setColu
-000045d0: 6d6e 436f 756e 7428 3429 0a20 2020 2020  mnCount(4).     
-000045e0: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-000045f0: 6573 745f 6469 616c 6f67 2e63 6f6e 7465  est_dialog.conte
-00004600: 7374 5f6c 6973 742e 7665 7274 6963 616c  st_list.vertical
-00004610: 4865 6164 6572 2829 2e73 6574 5669 7369  Header().setVisi
-00004620: 626c 6528 4661 6c73 6529 0a20 2020 2020  ble(False).     
-00004630: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-00004640: 6573 745f 6469 616c 6f67 2e63 6f6e 7465  est_dialog.conte
-00004650: 7374 5f6c 6973 742e 7365 7443 6f6c 756d  st_list.setColum
-00004660: 6e57 6964 7468 2831 2c20 3230 3029 0a20  nWidth(1, 200). 
-00004670: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00004680: 636f 6e74 6573 745f 6469 616c 6f67 2e63  contest_dialog.c
-00004690: 6f6e 7465 7374 5f6c 6973 742e 7365 7443  ontest_list.setC
-000046a0: 6f6c 756d 6e57 6964 7468 2832 2c20 3230  olumnWidth(2, 20
-000046b0: 3029 0a20 2020 2020 2020 2020 2020 2073  0).            s
-000046c0: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-000046d0: 6f67 2e63 6f6e 7465 7374 5f6c 6973 742e  og.contest_list.
-000046e0: 7365 7448 6f72 697a 6f6e 7461 6c48 6561  setHorizontalHea
-000046f0: 6465 7249 7465 6d28 0a20 2020 2020 2020  derItem(.       
-00004700: 2020 2020 2020 2020 2030 2c20 5174 5769           0, QtWi
-00004710: 6467 6574 732e 5154 6162 6c65 5769 6467  dgets.QTableWidg
-00004720: 6574 4974 656d 2822 436f 6e74 6573 7420  etItem("Contest 
-00004730: 4e72 2229 0a20 2020 2020 2020 2020 2020  Nr").           
-00004740: 2029 0a20 2020 2020 2020 2020 2020 2073   ).            s
-00004750: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-00004760: 6f67 2e63 6f6e 7465 7374 5f6c 6973 742e  og.contest_list.
-00004770: 7365 7448 6f72 697a 6f6e 7461 6c48 6561  setHorizontalHea
-00004780: 6465 7249 7465 6d28 0a20 2020 2020 2020  derItem(.       
-00004790: 2020 2020 2020 2020 2031 2c20 5174 5769           1, QtWi
-000047a0: 6467 6574 732e 5154 6162 6c65 5769 6467  dgets.QTableWidg
-000047b0: 6574 4974 656d 2822 436f 6e74 6573 7420  etItem("Contest 
-000047c0: 4e61 6d65 2229 0a20 2020 2020 2020 2020  Name").         
-000047d0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-000047e0: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
-000047f0: 616c 6f67 2e63 6f6e 7465 7374 5f6c 6973  alog.contest_lis
-00004800: 742e 7365 7448 6f72 697a 6f6e 7461 6c48  t.setHorizontalH
-00004810: 6561 6465 7249 7465 6d28 0a20 2020 2020  eaderItem(.     
-00004820: 2020 2020 2020 2020 2020 2032 2c20 5174             2, Qt
-00004830: 5769 6467 6574 732e 5154 6162 6c65 5769  Widgets.QTableWi
-00004840: 6467 6574 4974 656d 2822 436f 6e74 6573  dgetItem("Contes
-00004850: 7420 5374 6172 7422 290a 2020 2020 2020  t Start").      
-00004860: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00004870: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
-00004880: 5f64 6961 6c6f 672e 636f 6e74 6573 745f  _dialog.contest_
-00004890: 6c69 7374 2e73 6574 486f 7269 7a6f 6e74  list.setHorizont
-000048a0: 616c 4865 6164 6572 4974 656d 280a 2020  alHeaderItem(.  
-000048b0: 2020 2020 2020 2020 2020 2020 2020 332c                3,
-000048c0: 2051 7457 6964 6765 7473 2e51 5461 626c   QtWidgets.QTabl
-000048d0: 6557 6964 6765 7449 7465 6d28 224e 6f74  eWidgetItem("Not
-000048e0: 2055 4973 6564 2229 0a20 2020 2020 2020   UIsed").       
-000048f0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00004900: 2020 2073 656c 662e 636f 6e74 6573 745f     self.contest_
-00004910: 6469 616c 6f67 2e63 6f6e 7465 7374 5f6c  dialog.contest_l
-00004920: 6973 742e 7365 7443 6f6c 756d 6e48 6964  ist.setColumnHid
-00004930: 6465 6e28 302c 2054 7275 6529 0a20 2020  den(0, True).   
-00004940: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-00004950: 6e74 6573 745f 6469 616c 6f67 2e63 6f6e  ntest_dialog.con
-00004960: 7465 7374 5f6c 6973 742e 7365 7443 6f6c  test_list.setCol
-00004970: 756d 6e48 6964 6465 6e28 332c 2054 7275  umnHidden(3, Tru
-00004980: 6529 0a20 2020 2020 2020 2020 2020 2073  e).            s
-00004990: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-000049a0: 6f67 2e61 6363 6570 7465 642e 636f 6e6e  og.accepted.conn
-000049b0: 6563 7428 7365 6c66 2e6f 7065 6e5f 636f  ect(self.open_co
-000049c0: 6e74 6573 745f 7265 7475 726e 290a 2020  ntest_return).  
-000049d0: 2020 2020 2020 2020 2020 666f 7220 636f            for co
-000049e0: 6e74 6573 7420 696e 2063 6f6e 7465 7374  ntest in contest
-000049f0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-00004a00: 2020 206e 756d 6265 725f 6f66 5f72 6f77     number_of_row
-00004a10: 7320 3d20 7365 6c66 2e63 6f6e 7465 7374  s = self.contest
-00004a20: 5f64 6961 6c6f 672e 636f 6e74 6573 745f  _dialog.contest_
-00004a30: 6c69 7374 2e72 6f77 436f 756e 7428 290a  list.rowCount().
-00004a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a50: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
-00004a60: 6c6f 672e 636f 6e74 6573 745f 6c69 7374  log.contest_list
-00004a70: 2e69 6e73 6572 7452 6f77 286e 756d 6265  .insertRow(numbe
-00004a80: 725f 6f66 5f72 6f77 7329 0a20 2020 2020  r_of_rows).     
-00004a90: 2020 2020 2020 2020 2020 2063 6f6e 7465             conte
-00004aa0: 7374 5f69 6420 3d20 7374 7228 636f 6e74  st_id = str(cont
-00004ab0: 6573 742e 6765 7428 2243 6f6e 7465 7374  est.get("Contest
-00004ac0: 4944 222c 2031 2929 0a20 2020 2020 2020  ID", 1)).       
-00004ad0: 2020 2020 2020 2020 2063 6f6e 7465 7374           contest
-00004ae0: 5f6e 616d 6520 3d20 636f 6e74 6573 742e  _name = contest.
-00004af0: 6765 7428 2243 6f6e 7465 7374 4e61 6d65  get("ContestName
-00004b00: 222c 2031 290a 2020 2020 2020 2020 2020  ", 1).          
-00004b10: 2020 2020 2020 7374 6172 745f 6461 7465        start_date
-00004b20: 203d 2063 6f6e 7465 7374 2e67 6574 2822   = contest.get("
-00004b30: 5374 6172 7444 6174 6522 2c20 3129 0a20  StartDate", 1). 
-00004b40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00004b50: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-00004b60: 6f67 2e63 6f6e 7465 7374 5f6c 6973 742e  og.contest_list.
-00004b70: 7365 7449 7465 6d28 0a20 2020 2020 2020  setItem(.       
-00004b80: 2020 2020 2020 2020 2020 2020 206e 756d               num
-00004b90: 6265 725f 6f66 5f72 6f77 732c 2030 2c20  ber_of_rows, 0, 
-00004ba0: 5174 5769 6467 6574 732e 5154 6162 6c65  QtWidgets.QTable
-00004bb0: 5769 6467 6574 4974 656d 2863 6f6e 7465  WidgetItem(conte
-00004bc0: 7374 5f69 6429 0a20 2020 2020 2020 2020  st_id).         
-00004bd0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00004be0: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-00004bf0: 6e74 6573 745f 6469 616c 6f67 2e63 6f6e  ntest_dialog.con
-00004c00: 7465 7374 5f6c 6973 742e 7365 7449 7465  test_list.setIte
-00004c10: 6d28 0a20 2020 2020 2020 2020 2020 2020  m(.             
-00004c20: 2020 2020 2020 206e 756d 6265 725f 6f66         number_of
-00004c30: 5f72 6f77 732c 2031 2c20 5174 5769 6467  _rows, 1, QtWidg
-00004c40: 6574 732e 5154 6162 6c65 5769 6467 6574  ets.QTableWidget
-00004c50: 4974 656d 2863 6f6e 7465 7374 5f6e 616d  Item(contest_nam
-00004c60: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-00004c70: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00004c80: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
-00004c90: 745f 6469 616c 6f67 2e63 6f6e 7465 7374  t_dialog.contest
-00004ca0: 5f6c 6973 742e 7365 7449 7465 6d28 0a20  _list.setItem(. 
-00004cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cc0: 2020 206e 756d 6265 725f 6f66 5f72 6f77     number_of_row
-00004cd0: 732c 2032 2c20 5174 5769 6467 6574 732e  s, 2, QtWidgets.
-00004ce0: 5154 6162 6c65 5769 6467 6574 4974 656d  QTableWidgetItem
-00004cf0: 2873 7461 7274 5f64 6174 6529 0a20 2020  (start_date).   
-00004d00: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00004d10: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-00004d20: 6573 745f 6469 616c 6f67 2e73 686f 7728  est_dialog.show(
-00004d30: 290a 0a20 2020 2064 6566 206f 7065 6e5f  )..    def open_
-00004d40: 636f 6e74 6573 745f 7265 7475 726e 2873  contest_return(s
-00004d50: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-00004d60: 2243 616c 6c65 6420 6279 206f 7065 6e5f  "Called by open_
-00004d70: 636f 6e74 6573 7422 2222 0a20 2020 2020  contest""".     
-00004d80: 2020 2073 656c 6563 7465 645f 726f 7720     selected_row 
-00004d90: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f64  = self.contest_d
-00004da0: 6961 6c6f 672e 636f 6e74 6573 745f 6c69  ialog.contest_li
-00004db0: 7374 2e63 7572 7265 6e74 526f 7728 290a  st.currentRow().
-00004dc0: 2020 2020 2020 2020 636f 6e74 6573 7420          contest 
-00004dd0: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f64  = self.contest_d
-00004de0: 6961 6c6f 672e 636f 6e74 6573 745f 6c69  ialog.contest_li
-00004df0: 7374 2e69 7465 6d28 7365 6c65 6374 6564  st.item(selected
-00004e00: 5f72 6f77 2c20 3029 2e74 6578 7428 290a  _row, 0).text().
-00004e10: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
-00004e20: 665b 2263 6f6e 7465 7374 225d 203d 2063  f["contest"] = c
-00004e30: 6f6e 7465 7374 0a20 2020 2020 2020 2073  ontest.        s
-00004e40: 656c 662e 7772 6974 655f 7072 6566 6572  elf.write_prefer
-00004e50: 656e 6365 2829 0a20 2020 2020 2020 206c  ence().        l
-00004e60: 6f67 6765 722e 6465 6275 6728 2253 656c  ogger.debug("Sel
-00004e70: 6563 7465 6420 636f 6e74 6573 743a 2025  ected contest: %
-00004e80: 7322 2c20 6622 7b63 6f6e 7465 7374 7d22  s", f"{contest}"
-00004e90: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-00004ea0: 6f61 645f 636f 6e74 6573 7428 290a 2020  oad_contest().  
-00004eb0: 2020 2020 2020 7365 6c66 2e77 6f72 6b65        self.worke
-00004ec0: 645f 6c69 7374 203d 2073 656c 662e 6461  d_list = self.da
-00004ed0: 7461 6261 7365 2e67 6574 5f63 616c 6c73  tabase.get_calls
-00004ee0: 5f61 6e64 5f62 616e 6473 2829 0a20 2020  _and_bands().   
-00004ef0: 2020 2020 2073 656c 662e 7365 6e64 5f77       self.send_w
-00004f00: 6f72 6b65 645f 6c69 7374 2829 0a0a 2020  orked_list()..  
-00004f10: 2020 6465 6620 7265 6669 6c6c 5f64 726f    def refill_dro
-00004f20: 7064 6f77 6e28 7365 6c66 2c20 7461 7267  pdown(self, targ
-00004f30: 6574 2c20 736f 7572 6365 293a 0a20 2020  et, source):.   
-00004f40: 2020 2020 2022 2222 5265 6669 6c6c 2051       """Refill Q
-00004f50: 436f 6d62 6f62 6f78 2077 6964 6765 7420  Combobox widget 
-00004f60: 7769 7468 2076 616c 7565 2e22 2222 0a20  with value.""". 
-00004f70: 2020 2020 2020 2069 6e64 6578 203d 2074         index = t
-00004f80: 6172 6765 742e 6669 6e64 5465 7874 2873  arget.findText(s
-00004f90: 6f75 7263 6529 0a20 2020 2020 2020 2074  ource).        t
-00004fa0: 6172 6765 742e 7365 7443 7572 7265 6e74  arget.setCurrent
-00004fb0: 496e 6465 7828 696e 6465 7829 0a0a 2020  Index(index)..  
-00004fc0: 2020 6465 6620 6564 6974 5f63 6f6e 7465    def edit_conte
-00004fd0: 7374 2873 656c 6629 3a0a 2020 2020 2020  st(self):.      
-00004fe0: 2020 2222 2245 6469 7420 7468 6520 6375    """Edit the cu
-00004ff0: 7272 656e 7420 636f 6e74 6573 7422 2222  rrent contest"""
-00005000: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-00005010: 6465 6275 6728 2245 6469 7420 636f 6e74  debug("Edit cont
-00005020: 6573 7420 4469 616c 6f67 2229 0a20 2020  est Dialog").   
-00005030: 2020 2020 2069 6620 7365 6c66 2e63 6f6e       if self.con
-00005040: 7465 7374 2069 7320 4e6f 6e65 3a0a 2020  test is None:.  
-00005050: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00005060: 686f 775f 6d65 7373 6167 655f 626f 7828  how_message_box(
-00005070: 2259 6f75 2068 6176 6520 6e6f 2063 6f6e  "You have no con
-00005080: 7465 7374 2064 6566 696e 6564 2e22 290a  test defined.").
-00005090: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000050a0: 726e 0a20 2020 2020 2020 2069 6620 7365  rn.        if se
-000050b0: 6c66 2e63 6f6e 7465 7374 5f73 6574 7469  lf.contest_setti
-000050c0: 6e67 7320 6973 204e 6f6e 653a 0a20 2020  ngs is None:.   
-000050d0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-000050e0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-000050f0: 7465 7374 5f64 6961 6c6f 6720 3d20 4e65  test_dialog = Ne
-00005100: 7743 6f6e 7465 7374 2857 4f52 4b49 4e47  wContest(WORKING
-00005110: 5f50 4154 4829 0a20 2020 2020 2020 2073  _PATH).        s
-00005120: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-00005130: 6f67 2e73 6574 5769 6e64 6f77 5469 746c  og.setWindowTitl
-00005140: 6528 2245 6469 7420 436f 6e74 6573 7422  e("Edit Contest"
-00005150: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
-00005160: 6f6e 7465 7374 5f64 6961 6c6f 672e 7469  ontest_dialog.ti
-00005170: 746c 652e 7365 7454 6578 7428 2222 290a  tle.setText("").
-00005180: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-00005190: 7465 7374 5f64 6961 6c6f 672e 6163 6365  test_dialog.acce
-000051a0: 7074 6564 2e63 6f6e 6e65 6374 2873 656c  pted.connect(sel
-000051b0: 662e 7361 7665 5f65 6469 7465 645f 636f  f.save_edited_co
-000051c0: 6e74 6573 7429 0a20 2020 2020 2020 2076  ntest).        v
-000051d0: 616c 7565 203d 2073 656c 662e 636f 6e74  alue = self.cont
-000051e0: 6573 745f 7365 7474 696e 6773 2e67 6574  est_settings.get
-000051f0: 2822 436f 6e74 6573 744e 616d 6522 292e  ("ContestName").
-00005200: 7570 7065 7228 292e 7265 706c 6163 6528  upper().replace(
-00005210: 225f 222c 2022 2022 290a 2020 2020 2020  "_", " ").      
-00005220: 2020 6966 2076 616c 7565 203d 3d20 2247    if value == "G
-00005230: 454e 4552 414c 204c 4f47 4749 4e47 223a  ENERAL LOGGING":
-00005240: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
-00005250: 7565 203d 2022 4765 6e65 7261 6c20 4c6f  ue = "General Lo
-00005260: 6767 696e 6722 0a20 2020 2020 2020 2073  gging".        s
-00005270: 656c 662e 7265 6669 6c6c 5f64 726f 7064  elf.refill_dropd
-00005280: 6f77 6e28 7365 6c66 2e63 6f6e 7465 7374  own(self.contest
-00005290: 5f64 6961 6c6f 672e 636f 6e74 6573 742c  _dialog.contest,
-000052a0: 2076 616c 7565 290a 2020 2020 2020 2020   value).        
-000052b0: 7661 6c75 6520 3d20 7365 6c66 2e63 6f6e  value = self.con
-000052c0: 7465 7374 5f73 6574 7469 6e67 732e 6765  test_settings.ge
-000052d0: 7428 224f 7065 7261 746f 7243 6174 6567  t("OperatorCateg
-000052e0: 6f72 7922 290a 2020 2020 2020 2020 7365  ory").        se
-000052f0: 6c66 2e72 6566 696c 6c5f 6472 6f70 646f  lf.refill_dropdo
-00005300: 776e 2873 656c 662e 636f 6e74 6573 745f  wn(self.contest_
-00005310: 6469 616c 6f67 2e6f 7065 7261 746f 725f  dialog.operator_
-00005320: 636c 6173 732c 2076 616c 7565 290a 2020  class, value).  
-00005330: 2020 2020 2020 7661 6c75 6520 3d20 7365        value = se
-00005340: 6c66 2e63 6f6e 7465 7374 5f73 6574 7469  lf.contest_setti
-00005350: 6e67 732e 6765 7428 2242 616e 6443 6174  ngs.get("BandCat
-00005360: 6567 6f72 7922 290a 2020 2020 2020 2020  egory").        
-00005370: 7365 6c66 2e72 6566 696c 6c5f 6472 6f70  self.refill_drop
-00005380: 646f 776e 2873 656c 662e 636f 6e74 6573  down(self.contes
-00005390: 745f 6469 616c 6f67 2e62 616e 642c 2076  t_dialog.band, v
-000053a0: 616c 7565 290a 2020 2020 2020 2020 7661  alue).        va
-000053b0: 6c75 6520 3d20 7365 6c66 2e63 6f6e 7465  lue = self.conte
-000053c0: 7374 5f73 6574 7469 6e67 732e 6765 7428  st_settings.get(
-000053d0: 2250 6f77 6572 4361 7465 676f 7279 2229  "PowerCategory")
-000053e0: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-000053f0: 6669 6c6c 5f64 726f 7064 6f77 6e28 7365  fill_dropdown(se
-00005400: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-00005410: 672e 706f 7765 722c 2076 616c 7565 290a  g.power, value).
-00005420: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
-00005430: 7365 6c66 2e63 6f6e 7465 7374 5f73 6574  self.contest_set
-00005440: 7469 6e67 732e 6765 7428 224d 6f64 6543  tings.get("ModeC
-00005450: 6174 6567 6f72 7922 290a 2020 2020 2020  ategory").      
-00005460: 2020 7365 6c66 2e72 6566 696c 6c5f 6472    self.refill_dr
-00005470: 6f70 646f 776e 2873 656c 662e 636f 6e74  opdown(self.cont
-00005480: 6573 745f 6469 616c 6f67 2e6d 6f64 652c  est_dialog.mode,
-00005490: 2076 616c 7565 290a 2020 2020 2020 2020   value).        
-000054a0: 7661 6c75 6520 3d20 7365 6c66 2e63 6f6e  value = self.con
-000054b0: 7465 7374 5f73 6574 7469 6e67 732e 6765  test_settings.ge
-000054c0: 7428 224f 7665 726c 6179 4361 7465 676f  t("OverlayCatego
-000054d0: 7279 2229 0a20 2020 2020 2020 2073 656c  ry").        sel
-000054e0: 662e 7265 6669 6c6c 5f64 726f 7064 6f77  f.refill_dropdow
-000054f0: 6e28 7365 6c66 2e63 6f6e 7465 7374 5f64  n(self.contest_d
-00005500: 6961 6c6f 672e 6f76 6572 6c61 792c 2076  ialog.overlay, v
-00005510: 616c 7565 290a 2020 2020 2020 2020 7365  alue).        se
-00005520: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-00005530: 672e 6f70 6572 6174 6f72 732e 7365 7454  g.operators.setT
-00005540: 6578 7428 7365 6c66 2e63 6f6e 7465 7374  ext(self.contest
-00005550: 5f73 6574 7469 6e67 732e 6765 7428 224f  _settings.get("O
-00005560: 7065 7261 746f 7273 2229 290a 2020 2020  perators")).    
-00005570: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
-00005580: 5f64 6961 6c6f 672e 736f 6170 626f 782e  _dialog.soapbox.
-00005590: 7365 7450 6c61 696e 5465 7874 2873 656c  setPlainText(sel
-000055a0: 662e 636f 6e74 6573 745f 7365 7474 696e  f.contest_settin
-000055b0: 6773 2e67 6574 2822 536f 6170 626f 7822  gs.get("Soapbox"
-000055c0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-000055d0: 636f 6e74 6573 745f 6469 616c 6f67 2e65  contest_dialog.e
-000055e0: 7863 6861 6e67 652e 7365 7454 6578 7428  xchange.setText(
-000055f0: 7365 6c66 2e63 6f6e 7465 7374 5f73 6574  self.contest_set
-00005600: 7469 6e67 732e 6765 7428 2253 656e 7445  tings.get("SentE
-00005610: 7863 6861 6e67 6522 2929 0a20 2020 2020  xchange")).     
-00005620: 2020 2076 616c 7565 203d 2073 656c 662e     value = self.
-00005630: 636f 6e74 6573 745f 7365 7474 696e 6773  contest_settings
-00005640: 2e67 6574 2822 5374 6174 696f 6e43 6174  .get("StationCat
-00005650: 6567 6f72 7922 290a 2020 2020 2020 2020  egory").        
-00005660: 7365 6c66 2e72 6566 696c 6c5f 6472 6f70  self.refill_drop
-00005670: 646f 776e 2873 656c 662e 636f 6e74 6573  down(self.contes
-00005680: 745f 6469 616c 6f67 2e73 7461 7469 6f6e  t_dialog.station
-00005690: 2c20 7661 6c75 6529 0a20 2020 2020 2020  , value).       
-000056a0: 2076 616c 7565 203d 2073 656c 662e 636f   value = self.co
-000056b0: 6e74 6573 745f 7365 7474 696e 6773 2e67  ntest_settings.g
-000056c0: 6574 2822 4173 7369 7374 6564 4361 7465  et("AssistedCate
-000056d0: 676f 7279 2229 0a20 2020 2020 2020 2073  gory").        s
-000056e0: 656c 662e 7265 6669 6c6c 5f64 726f 7064  elf.refill_dropd
-000056f0: 6f77 6e28 7365 6c66 2e63 6f6e 7465 7374  own(self.contest
-00005700: 5f64 6961 6c6f 672e 6173 7369 7374 6564  _dialog.assisted
-00005710: 2c20 7661 6c75 6529 0a20 2020 2020 2020  , value).       
-00005720: 2076 616c 7565 203d 2073 656c 662e 636f   value = self.co
-00005730: 6e74 6573 745f 7365 7474 696e 6773 2e67  ntest_settings.g
-00005740: 6574 2822 5472 616e 736d 6974 7465 7243  et("TransmitterC
-00005750: 6174 6567 6f72 7922 290a 2020 2020 2020  ategory").      
-00005760: 2020 7365 6c66 2e72 6566 696c 6c5f 6472    self.refill_dr
-00005770: 6f70 646f 776e 2873 656c 662e 636f 6e74  opdown(self.cont
-00005780: 6573 745f 6469 616c 6f67 2e74 7261 6e73  est_dialog.trans
-00005790: 6d69 7474 6572 2c20 7661 6c75 6529 0a20  mitter, value). 
-000057a0: 2020 2020 2020 2076 616c 7565 203d 2073         value = s
-000057b0: 656c 662e 636f 6e74 6573 745f 7365 7474  elf.contest_sett
-000057c0: 696e 6773 2e67 6574 2822 5374 6172 7444  ings.get("StartD
-000057d0: 6174 6522 290a 2020 2020 2020 2020 7468  ate").        th
-000057e0: 655f 6461 7465 2c20 7468 655f 7469 6d65  e_date, the_time
-000057f0: 203d 2076 616c 7565 2e73 706c 6974 2829   = value.split()
-00005800: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-00005810: 6e74 6573 745f 6469 616c 6f67 2e64 6174  ntest_dialog.dat
-00005820: 6554 696d 6545 6469 742e 7365 7444 6174  eTimeEdit.setDat
-00005830: 6528 0a20 2020 2020 2020 2020 2020 2051  e(.            Q
-00005840: 7443 6f72 652e 5144 6174 652e 6672 6f6d  tCore.QDate.from
-00005850: 5374 7269 6e67 2874 6865 5f64 6174 652c  String(the_date,
-00005860: 2022 7979 7979 2d4d 4d2d 6464 2229 0a20   "yyyy-MM-dd"). 
-00005870: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00005880: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
-00005890: 616c 6f67 2e64 6174 6554 696d 6545 6469  alog.dateTimeEdi
-000058a0: 742e 7365 7443 616c 656e 6461 7250 6f70  t.setCalendarPop
-000058b0: 7570 2854 7275 6529 0a20 2020 2020 2020  up(True).       
-000058c0: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
-000058d0: 616c 6f67 2e64 6174 6554 696d 6545 6469  alog.dateTimeEdi
-000058e0: 742e 7365 7454 696d 6528 0a20 2020 2020  t.setTime(.     
-000058f0: 2020 2020 2020 2051 7443 6f72 652e 5154         QtCore.QT
-00005900: 696d 652e 6672 6f6d 5374 7269 6e67 2874  ime.fromString(t
-00005910: 6865 5f74 696d 652c 2022 6868 3a6d 6d3a  he_time, "hh:mm:
-00005920: 7373 2229 0a20 2020 2020 2020 2029 0a20  ss").        ). 
-00005930: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-00005940: 6573 745f 6469 616c 6f67 2e6f 7065 6e28  est_dialog.open(
-00005950: 290a 0a20 2020 2064 6566 2073 6176 655f  )..    def save_
-00005960: 6564 6974 6564 5f63 6f6e 7465 7374 2873  edited_contest(s
-00005970: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-00005980: 2253 6176 6520 7468 6520 6564 6974 6564  "Save the edited
-00005990: 2063 6f6e 7465 7374 2222 220a 2020 2020   contest""".    
-000059a0: 2020 2020 636f 6e74 6573 7420 3d20 7b7d      contest = {}
-000059b0: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
-000059c0: 5b22 436f 6e74 6573 744e 616d 6522 5d20  ["ContestName"] 
-000059d0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-000059e0: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
-000059f0: 6c6f 672e 636f 6e74 6573 742e 6375 7272  log.contest.curr
-00005a00: 656e 7454 6578 7428 292e 6c6f 7765 7228  entText().lower(
-00005a10: 292e 7265 706c 6163 6528 2220 222c 2022  ).replace(" ", "
-00005a20: 5f22 290a 2020 2020 2020 2020 290a 2020  _").        ).  
-00005a30: 2020 2020 2020 636f 6e74 6573 745b 2253        contest["S
-00005a40: 7461 7274 4461 7465 225d 203d 2073 656c  tartDate"] = sel
-00005a50: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
-00005a60: 2e64 6174 6554 696d 6545 6469 742e 6461  .dateTimeEdit.da
-00005a70: 7465 5469 6d65 2829 2e74 6f53 7472 696e  teTime().toStrin
-00005a80: 6728 0a20 2020 2020 2020 2020 2020 2022  g(.            "
-00005a90: 7979 7979 2d4d 4d2d 6464 2068 683a 6d6d  yyyy-MM-dd hh:mm
-00005aa0: 3a73 7322 0a20 2020 2020 2020 2029 0a20  :ss".        ). 
-00005ab0: 2020 2020 2020 2063 6f6e 7465 7374 5b22         contest["
-00005ac0: 4f70 6572 6174 6f72 4361 7465 676f 7279  OperatorCategory
-00005ad0: 225d 203d 2073 656c 662e 636f 6e74 6573  "] = self.contes
-00005ae0: 745f 6469 616c 6f67 2e6f 7065 7261 746f  t_dialog.operato
-00005af0: 725f 636c 6173 732e 6375 7272 656e 7454  r_class.currentT
-00005b00: 6578 7428 290a 2020 2020 2020 2020 636f  ext().        co
-00005b10: 6e74 6573 745b 2242 616e 6443 6174 6567  ntest["BandCateg
-00005b20: 6f72 7922 5d20 3d20 7365 6c66 2e63 6f6e  ory"] = self.con
-00005b30: 7465 7374 5f64 6961 6c6f 672e 6261 6e64  test_dialog.band
-00005b40: 2e63 7572 7265 6e74 5465 7874 2829 0a20  .currentText(). 
-00005b50: 2020 2020 2020 2063 6f6e 7465 7374 5b22         contest["
-00005b60: 506f 7765 7243 6174 6567 6f72 7922 5d20  PowerCategory"] 
-00005b70: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f64  = self.contest_d
-00005b80: 6961 6c6f 672e 706f 7765 722e 6375 7272  ialog.power.curr
-00005b90: 656e 7454 6578 7428 290a 2020 2020 2020  entText().      
-00005ba0: 2020 636f 6e74 6573 745b 224d 6f64 6543    contest["ModeC
-00005bb0: 6174 6567 6f72 7922 5d20 3d20 7365 6c66  ategory"] = self
-00005bc0: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
-00005bd0: 6d6f 6465 2e63 7572 7265 6e74 5465 7874  mode.currentText
-00005be0: 2829 0a20 2020 2020 2020 2063 6f6e 7465  ().        conte
-00005bf0: 7374 5b22 4f76 6572 6c61 7943 6174 6567  st["OverlayCateg
-00005c00: 6f72 7922 5d20 3d20 7365 6c66 2e63 6f6e  ory"] = self.con
-00005c10: 7465 7374 5f64 6961 6c6f 672e 6f76 6572  test_dialog.over
-00005c20: 6c61 792e 6375 7272 656e 7454 6578 7428  lay.currentText(
-00005c30: 290a 2020 2020 2020 2020 636f 6e74 6573  ).        contes
-00005c40: 745b 224f 7065 7261 746f 7273 225d 203d  t["Operators"] =
-00005c50: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
-00005c60: 616c 6f67 2e6f 7065 7261 746f 7273 2e74  alog.operators.t
-00005c70: 6578 7428 290a 2020 2020 2020 2020 636f  ext().        co
-00005c80: 6e74 6573 745b 2253 6f61 7062 6f78 225d  ntest["Soapbox"]
-00005c90: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
-00005ca0: 6469 616c 6f67 2e73 6f61 7062 6f78 2e74  dialog.soapbox.t
-00005cb0: 6f50 6c61 696e 5465 7874 2829 0a20 2020  oPlainText().   
-00005cc0: 2020 2020 2063 6f6e 7465 7374 5b22 5365       contest["Se
-00005cd0: 6e74 4578 6368 616e 6765 225d 203d 2073  ntExchange"] = s
-00005ce0: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-00005cf0: 6f67 2e65 7863 6861 6e67 652e 7465 7874  og.exchange.text
-00005d00: 2829 0a20 2020 2020 2020 2063 6f6e 7465  ().        conte
-00005d10: 7374 5b22 436f 6e74 6573 744e 5222 5d20  st["ContestNR"] 
-00005d20: 3d20 7365 6c66 2e70 7265 662e 6765 7428  = self.pref.get(
-00005d30: 2263 6f6e 7465 7374 222c 2031 290a 2020  "contest", 1).  
-00005d40: 2020 2020 2020 636f 6e74 6573 745b 2253        contest["S
-00005d50: 7461 7469 6f6e 4361 7465 676f 7279 225d  tationCategory"]
-00005d60: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
-00005d70: 6469 616c 6f67 2e73 7461 7469 6f6e 2e63  dialog.station.c
-00005d80: 7572 7265 6e74 5465 7874 2829 0a20 2020  urrentText().   
-00005d90: 2020 2020 2063 6f6e 7465 7374 5b22 4173       contest["As
-00005da0: 7369 7374 6564 4361 7465 676f 7279 225d  sistedCategory"]
-00005db0: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
-00005dc0: 6469 616c 6f67 2e61 7373 6973 7465 642e  dialog.assisted.
-00005dd0: 6375 7272 656e 7454 6578 7428 290a 2020  currentText().  
-00005de0: 2020 2020 2020 636f 6e74 6573 745b 2254        contest["T
-00005df0: 7261 6e73 6d69 7474 6572 4361 7465 676f  ransmitterCatego
-00005e00: 7279 225d 203d 2073 656c 662e 636f 6e74  ry"] = self.cont
-00005e10: 6573 745f 6469 616c 6f67 2e74 7261 6e73  est_dialog.trans
-00005e20: 6d69 7474 6572 2e63 7572 7265 6e74 5465  mitter.currentTe
-00005e30: 7874 2829 0a0a 2020 2020 2020 2020 6c6f  xt()..        lo
-00005e40: 6767 6572 2e64 6562 7567 2822 2573 222c  gger.debug("%s",
-00005e50: 2066 227b 636f 6e74 6573 747d 2229 0a20   f"{contest}"). 
-00005e60: 2020 2020 2020 2073 656c 662e 6461 7461         self.data
-00005e70: 6261 7365 2e75 7064 6174 655f 636f 6e74  base.update_cont
-00005e80: 6573 7428 636f 6e74 6573 7429 0a20 2020  est(contest).   
-00005e90: 2020 2020 2073 656c 662e 7772 6974 655f       self.write_
-00005ea0: 7072 6566 6572 656e 6365 2829 0a20 2020  preference().   
-00005eb0: 2020 2020 2073 656c 662e 6c6f 6164 5f63       self.load_c
-00005ec0: 6f6e 7465 7374 2829 0a0a 2020 2020 6465  ontest()..    de
-00005ed0: 6620 6c6f 6164 5f63 6f6e 7465 7374 2873  f load_contest(s
-00005ee0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-00005ef0: 226c 6f61 6420 6120 636f 6e74 6573 7422  "load a contest"
-00005f00: 2222 0a20 2020 2020 2020 2069 6620 7365  "".        if se
-00005f10: 6c66 2e70 7265 662e 6765 7428 2263 6f6e  lf.pref.get("con
-00005f20: 7465 7374 2229 3a0a 2020 2020 2020 2020  test"):.        
-00005f30: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
-00005f40: 5f73 6574 7469 6e67 7320 3d20 7365 6c66  _settings = self
-00005f50: 2e64 6174 6162 6173 652e 6665 7463 685f  .database.fetch_
-00005f60: 636f 6e74 6573 745f 6279 5f69 6428 0a20  contest_by_id(. 
-00005f70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00005f80: 656c 662e 7072 6566 2e67 6574 2822 636f  elf.pref.get("co
-00005f90: 6e74 6573 7422 290a 2020 2020 2020 2020  ntest").        
-00005fa0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00005fb0: 2020 6966 2073 656c 662e 636f 6e74 6573    if self.contes
-00005fc0: 745f 7365 7474 696e 6773 3a0a 2020 2020  t_settings:.    
-00005fd0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00005fe0: 2e64 6174 6162 6173 652e 6375 7272 656e  .database.curren
-00005ff0: 745f 636f 6e74 6573 7420 3d20 7365 6c66  t_contest = self
-00006000: 2e70 7265 662e 6765 7428 2263 6f6e 7465  .pref.get("conte
-00006010: 7374 2229 0a20 2020 2020 2020 2020 2020  st").           
-00006020: 2020 2020 2069 6620 7365 6c66 2e63 6f6e       if self.con
-00006030: 7465 7374 5f73 6574 7469 6e67 732e 6765  test_settings.ge
-00006040: 7428 2243 6f6e 7465 7374 4e61 6d65 2229  t("ContestName")
-00006050: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00006060: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
-00006070: 7374 203d 2064 6f69 6d70 2873 656c 662e  st = doimp(self.
-00006080: 636f 6e74 6573 745f 7365 7474 696e 6773  contest_settings
-00006090: 2e67 6574 2822 436f 6e74 6573 744e 616d  .get("ContestNam
-000060a0: 6522 2929 0a20 2020 2020 2020 2020 2020  e")).           
-000060b0: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-000060c0: 6465 6275 6728 224c 6f61 6465 6420 436f  debug("Loaded Co
-000060d0: 6e74 6573 7420 4e61 6d65 203d 2025 7322  ntest Name = %s"
-000060e0: 2c20 7365 6c66 2e63 6f6e 7465 7374 2e6e  , self.contest.n
-000060f0: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
-00006100: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-00006110: 745f 7769 6e64 6f77 5f74 6974 6c65 2829  t_window_title()
-00006120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006130: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
-00006140: 742e 696e 6974 5f63 6f6e 7465 7374 2873  t.init_contest(s
-00006150: 656c 6629 0a20 2020 2020 2020 2020 2020  elf).           
-00006160: 2020 2020 2020 2020 2073 656c 662e 6869           self.hi
-00006170: 6465 5f62 616e 645f 6d6f 6465 2873 656c  de_band_mode(sel
-00006180: 662e 636f 6e74 6573 745f 7365 7474 696e  f.contest_settin
-00006190: 6773 2e67 6574 2822 4d6f 6465 4361 7465  gs.get("ModeCate
-000061a0: 676f 7279 222c 2022 2229 290a 2020 2020  gory", "")).    
-000061b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061c0: 6c6f 6767 6572 2e64 6562 7567 2822 2573  logger.debug("%s
-000061d0: 222c 2066 227b 7365 6c66 2e63 6f6e 7465  ", f"{self.conte
-000061e0: 7374 5f73 6574 7469 6e67 737d 2229 0a20  st_settings}"). 
-000061f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006200: 2020 2069 6620 7365 6c66 2e63 6f6e 7465     if self.conte
-00006210: 7374 5f73 6574 7469 6e67 732e 6765 7428  st_settings.get(
-00006220: 224d 6f64 6543 6174 6567 6f72 7922 2c20  "ModeCategory", 
-00006230: 2222 2920 3d3d 2022 4357 223a 0a20 2020  "") == "CW":.   
-00006240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006250: 2020 2020 2073 656c 662e 7365 746d 6f64       self.setmod
-00006260: 6528 2243 5722 290a 2020 2020 2020 2020  e("CW").        
-00006270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006280: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
-00006290: 5b22 6d6f 6465 225d 203d 2022 4357 220a  ["mode"] = "CW".
-000062a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000062c0: 7269 675f 636f 6e74 726f 6c3a 0a20 2020  rig_control:.   
-000062d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062e0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-000062f0: 2e72 6967 5f63 6f6e 7472 6f6c 2e6f 6e6c  .rig_control.onl
-00006300: 696e 653a 0a20 2020 2020 2020 2020 2020  ine:.           
+00001a30: 5646 4f2e 7472 6967 6765 7265 642e 636f  VFO.triggered.co
+00001a40: 6e6e 6563 7428 7365 6c66 2e6c 6175 6e63  nnect(self.launc
+00001a50: 685f 7666 6f29 0a20 2020 2020 2020 2073  h_vfo).        s
+00001a60: 656c 662e 6163 7469 6f6e 5265 6361 6c63  elf.actionRecalc
+00001a70: 756c 6174 655f 4d75 6c74 732e 7472 6967  ulate_Mults.trig
+00001a80: 6765 7265 642e 636f 6e6e 6563 7428 7365  gered.connect(se
+00001a90: 6c66 2e72 6563 616c 6375 6c61 7465 5f6d  lf.recalculate_m
+00001aa0: 756c 7473 290a 0a20 2020 2020 2020 2073  ults)..        s
+00001ab0: 656c 662e 6163 7469 6f6e 4765 6e65 7261  elf.actionGenera
+00001ac0: 7465 5f43 6162 7269 6c6c 6f2e 7472 6967  te_Cabrillo.trig
+00001ad0: 6765 7265 642e 636f 6e6e 6563 7428 7365  gered.connect(se
+00001ae0: 6c66 2e67 656e 6572 6174 655f 6361 6272  lf.generate_cabr
+00001af0: 696c 6c6f 290a 2020 2020 2020 2020 7365  illo).        se
+00001b00: 6c66 2e61 6374 696f 6e47 656e 6572 6174  lf.actionGenerat
+00001b10: 655f 4144 4946 2e74 7269 6767 6572 6564  e_ADIF.triggered
+00001b20: 2e63 6f6e 6e65 6374 2873 656c 662e 6765  .connect(self.ge
+00001b30: 6e65 7261 7465 5f61 6469 6629 0a0a 2020  nerate_adif)..  
+00001b40: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
+00001b50: 6e43 6f6e 6669 6775 7261 7469 6f6e 5f53  nConfiguration_S
+00001b60: 6574 7469 6e67 732e 7472 6967 6765 7265  ettings.triggere
+00001b70: 642e 636f 6e6e 6563 7428 0a20 2020 2020  d.connect(.     
+00001b80: 2020 2020 2020 2073 656c 662e 6564 6974         self.edit
+00001b90: 5f63 6f6e 6669 6775 7261 7469 6f6e 5f73  _configuration_s
+00001ba0: 6574 7469 6e67 730a 2020 2020 2020 2020  ettings.        
+00001bb0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00001bc0: 6374 696f 6e53 7461 7469 6f6e 5365 7474  ctionStationSett
+00001bd0: 696e 6773 2e74 7269 6767 6572 6564 2e63  ings.triggered.c
+00001be0: 6f6e 6e65 6374 2873 656c 662e 6564 6974  onnect(self.edit
+00001bf0: 5f73 7461 7469 6f6e 5f73 6574 7469 6e67  _station_setting
+00001c00: 7329 0a0a 2020 2020 2020 2020 7365 6c66  s)..        self
+00001c10: 2e61 6374 696f 6e4e 6577 5f43 6f6e 7465  .actionNew_Conte
+00001c20: 7374 2e74 7269 6767 6572 6564 2e63 6f6e  st.triggered.con
+00001c30: 6e65 6374 2873 656c 662e 6e65 775f 636f  nect(self.new_co
+00001c40: 6e74 6573 745f 6469 616c 6f67 290a 2020  ntest_dialog).  
+00001c50: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
+00001c60: 6e4f 7065 6e5f 436f 6e74 6573 742e 7472  nOpen_Contest.tr
+00001c70: 6967 6765 7265 642e 636f 6e6e 6563 7428  iggered.connect(
+00001c80: 7365 6c66 2e6f 7065 6e5f 636f 6e74 6573  self.open_contes
+00001c90: 7429 0a20 2020 2020 2020 2073 656c 662e  t).        self.
+00001ca0: 6163 7469 6f6e 4564 6974 5f43 7572 7265  actionEdit_Curre
+00001cb0: 6e74 5f43 6f6e 7465 7374 2e74 7269 6767  nt_Contest.trigg
+00001cc0: 6572 6564 2e63 6f6e 6e65 6374 2873 656c  ered.connect(sel
+00001cd0: 662e 6564 6974 5f63 6f6e 7465 7374 290a  f.edit_contest).
+00001ce0: 0a20 2020 2020 2020 2073 656c 662e 6163  .        self.ac
+00001cf0: 7469 6f6e 4e65 775f 4461 7461 6261 7365  tionNew_Database
+00001d00: 2e74 7269 6767 6572 6564 2e63 6f6e 6e65  .triggered.conne
+00001d10: 6374 2873 656c 662e 6e65 775f 6461 7461  ct(self.new_data
+00001d20: 6261 7365 290a 2020 2020 2020 2020 7365  base).        se
+00001d30: 6c66 2e61 6374 696f 6e4f 7065 6e5f 4461  lf.actionOpen_Da
+00001d40: 7461 6261 7365 2e74 7269 6767 6572 6564  tabase.triggered
+00001d50: 2e63 6f6e 6e65 6374 2873 656c 662e 6f70  .connect(self.op
+00001d60: 656e 5f64 6174 6162 6173 6529 0a0a 2020  en_database)..  
+00001d70: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
+00001d80: 6e45 6469 745f 4d61 6372 6f73 2e74 7269  nEdit_Macros.tri
+00001d90: 6767 6572 6564 2e63 6f6e 6e65 6374 2873  ggered.connect(s
+00001da0: 656c 662e 6564 6974 5f63 775f 6d61 6372  elf.edit_cw_macr
+00001db0: 6f73 290a 0a20 2020 2020 2020 2073 656c  os)..        sel
+00001dc0: 662e 6163 7469 6f6e 4162 6f75 742e 7472  f.actionAbout.tr
+00001dd0: 6967 6765 7265 642e 636f 6e6e 6563 7428  iggered.connect(
+00001de0: 7365 6c66 2e73 686f 775f 6162 6f75 745f  self.show_about_
+00001df0: 6469 616c 6f67 290a 2020 2020 2020 2020  dialog).        
+00001e00: 7365 6c66 2e61 6374 696f 6e48 6f74 4b65  self.actionHotKe
+00001e10: 7973 2e74 7269 6767 6572 6564 2e63 6f6e  ys.triggered.con
+00001e20: 6e65 6374 2873 656c 662e 7368 6f77 5f6b  nect(self.show_k
+00001e30: 6579 5f68 656c 7029 0a20 2020 2020 2020  ey_help).       
+00001e40: 2073 656c 662e 6163 7469 6f6e 4865 6c70   self.actionHelp
+00001e50: 2e74 7269 6767 6572 6564 2e63 6f6e 6e65  .triggered.conne
+00001e60: 6374 2873 656c 662e 7368 6f77 5f68 656c  ct(self.show_hel
+00001e70: 705f 6469 616c 6f67 290a 2020 2020 2020  p_dialog).      
+00001e80: 2020 7365 6c66 2e61 6374 696f 6e55 7064    self.actionUpd
+00001e90: 6174 655f 4354 592e 7472 6967 6765 7265  ate_CTY.triggere
+00001ea0: 642e 636f 6e6e 6563 7428 7365 6c66 2e63  d.connect(self.c
+00001eb0: 6865 636b 5f66 6f72 5f6e 6577 5f63 7479  heck_for_new_cty
+00001ec0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00001ed0: 6374 696f 6e55 7064 6174 655f 4d41 5354  ctionUpdate_MAST
+00001ee0: 4552 5f53 4350 2e74 7269 6767 6572 6564  ER_SCP.triggered
+00001ef0: 2e63 6f6e 6e65 6374 2873 656c 662e 7570  .connect(self.up
+00001f00: 6461 7465 5f6d 6173 7465 7273 6370 290a  date_masterscp).
+00001f10: 2020 2020 2020 2020 7365 6c66 2e61 6374          self.act
+00001f20: 696f 6e51 7569 742e 7472 6967 6765 7265  ionQuit.triggere
+00001f30: 642e 636f 6e6e 6563 7428 7365 6c66 2e71  d.connect(self.q
+00001f40: 7569 745f 6170 7029 0a0a 2020 2020 2020  uit_app)..      
+00001f50: 2020 7365 6c66 2e72 6164 696f 4275 7474    self.radioButt
+00001f60: 6f6e 5f72 756e 2e63 6c69 636b 6564 2e63  on_run.clicked.c
+00001f70: 6f6e 6e65 6374 2873 656c 662e 7275 6e5f  onnect(self.run_
+00001f80: 7370 5f62 7574 746f 6e73 5f63 6c69 636b  sp_buttons_click
+00001f90: 6564 290a 2020 2020 2020 2020 7365 6c66  ed).        self
+00001fa0: 2e72 6164 696f 4275 7474 6f6e 5f73 702e  .radioButton_sp.
+00001fb0: 636c 6963 6b65 642e 636f 6e6e 6563 7428  clicked.connect(
+00001fc0: 7365 6c66 2e72 756e 5f73 705f 6275 7474  self.run_sp_butt
+00001fd0: 6f6e 735f 636c 6963 6b65 6429 0a20 2020  ons_clicked).   
+00001fe0: 2020 2020 2073 656c 662e 7363 6f72 652e       self.score.
+00001ff0: 7365 7454 6578 7428 2230 2229 0a20 2020  setText("0").   
+00002000: 2020 2020 2073 656c 662e 6361 6c6c 7369       self.callsi
+00002010: 676e 2e74 6578 7445 6469 7465 642e 636f  gn.textEdited.co
+00002020: 6e6e 6563 7428 7365 6c66 2e63 616c 6c73  nnect(self.calls
+00002030: 6967 6e5f 6368 616e 6765 6429 0a20 2020  ign_changed).   
+00002040: 2020 2020 2073 656c 662e 6361 6c6c 7369       self.callsi
+00002050: 676e 2e72 6574 7572 6e50 7265 7373 6564  gn.returnPressed
+00002060: 2e63 6f6e 6e65 6374 2873 656c 662e 7361  .connect(self.sa
+00002070: 7665 5f63 6f6e 7461 6374 290a 2020 2020  ve_contact).    
+00002080: 2020 2020 7365 6c66 2e73 656e 742e 7265      self.sent.re
+00002090: 7475 726e 5072 6573 7365 642e 636f 6e6e  turnPressed.conn
+000020a0: 6563 7428 7365 6c66 2e73 6176 655f 636f  ect(self.save_co
+000020b0: 6e74 6163 7429 0a20 2020 2020 2020 2073  ntact).        s
+000020c0: 656c 662e 7265 6365 6976 652e 7265 7475  elf.receive.retu
+000020d0: 726e 5072 6573 7365 642e 636f 6e6e 6563  rnPressed.connec
+000020e0: 7428 7365 6c66 2e73 6176 655f 636f 6e74  t(self.save_cont
+000020f0: 6163 7429 0a20 2020 2020 2020 2073 656c  act).        sel
+00002100: 662e 6f74 6865 725f 312e 7265 7475 726e  f.other_1.return
+00002110: 5072 6573 7365 642e 636f 6e6e 6563 7428  Pressed.connect(
+00002120: 7365 6c66 2e73 6176 655f 636f 6e74 6163  self.save_contac
+00002130: 7429 0a20 2020 2020 2020 2073 656c 662e  t).        self.
+00002140: 6f74 6865 725f 312e 7465 7874 4564 6974  other_1.textEdit
+00002150: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
+00002160: 6f74 6865 725f 315f 6368 616e 6765 6429  other_1_changed)
+00002170: 0a20 2020 2020 2020 2073 656c 662e 6f74  .        self.ot
+00002180: 6865 725f 322e 7265 7475 726e 5072 6573  her_2.returnPres
+00002190: 7365 642e 636f 6e6e 6563 7428 7365 6c66  sed.connect(self
+000021a0: 2e73 6176 655f 636f 6e74 6163 7429 0a20  .save_contact). 
+000021b0: 2020 2020 2020 2073 656c 662e 6f74 6865         self.othe
+000021c0: 725f 322e 7465 7874 4564 6974 6564 2e63  r_2.textEdited.c
+000021d0: 6f6e 6e65 6374 2873 656c 662e 6f74 6865  onnect(self.othe
+000021e0: 725f 325f 6368 616e 6765 6429 0a0a 2020  r_2_changed)..  
+000021f0: 2020 2020 2020 7365 6c66 2e73 656e 742e        self.sent.
+00002200: 7365 7454 6578 7428 2235 3922 290a 2020  setText("59").  
+00002210: 2020 2020 2020 7365 6c66 2e72 6563 6569        self.recei
+00002220: 7665 2e73 6574 5465 7874 2822 3539 2229  ve.setText("59")
+00002230: 0a20 2020 2020 2020 2069 636f 6e5f 7061  .        icon_pa
+00002240: 7468 203d 2057 4f52 4b49 4e47 5f50 4154  th = WORKING_PAT
+00002250: 4820 2b20 222f 6461 7461 2f22 0a20 2020  H + "/data/".   
+00002260: 2020 2020 2073 656c 662e 6772 6565 6e64       self.greend
+00002270: 6f74 203d 2051 7447 7569 2e51 5069 786d  ot = QtGui.QPixm
+00002280: 6170 2869 636f 6e5f 7061 7468 202b 2022  ap(icon_path + "
+00002290: 6772 6565 6e64 6f74 2e70 6e67 2229 0a20  greendot.png"). 
+000022a0: 2020 2020 2020 2073 656c 662e 7265 6464         self.redd
+000022b0: 6f74 203d 2051 7447 7569 2e51 5069 786d  ot = QtGui.QPixm
+000022c0: 6170 2869 636f 6e5f 7061 7468 202b 2022  ap(icon_path + "
+000022d0: 7265 6464 6f74 2e70 6e67 2229 0a20 2020  reddot.png").   
+000022e0: 2020 2020 2073 656c 662e 6c65 6674 646f       self.leftdo
+000022f0: 742e 7365 7450 6978 6d61 7028 7365 6c66  t.setPixmap(self
+00002300: 2e67 7265 656e 646f 7429 0a20 2020 2020  .greendot).     
+00002310: 2020 2073 656c 662e 7269 6768 7464 6f74     self.rightdot
+00002320: 2e73 6574 5069 786d 6170 2873 656c 662e  .setPixmap(self.
+00002330: 7265 6464 6f74 290a 0a20 2020 2020 2020  reddot)..       
+00002340: 2073 656c 662e 4631 2e73 6574 436f 6e74   self.F1.setCont
+00002350: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
+00002360: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
+00002370: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
+00002380: 2020 2073 656c 662e 4631 2e63 7573 746f     self.F1.custo
+00002390: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
+000023a0: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
+000023b0: 6c66 2e65 6469 745f 4631 290a 2020 2020  lf.edit_F1).    
+000023c0: 2020 2020 7365 6c66 2e46 312e 636c 6963      self.F1.clic
+000023d0: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
+000023e0: 2e73 656e 6466 3129 0a20 2020 2020 2020  .sendf1).       
+000023f0: 2073 656c 662e 4632 2e73 6574 436f 6e74   self.F2.setCont
+00002400: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
+00002410: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
+00002420: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
+00002430: 2020 2073 656c 662e 4632 2e63 7573 746f     self.F2.custo
+00002440: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
+00002450: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
+00002460: 6c66 2e65 6469 745f 4632 290a 2020 2020  lf.edit_F2).    
+00002470: 2020 2020 7365 6c66 2e46 322e 636c 6963      self.F2.clic
+00002480: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
+00002490: 2e73 656e 6466 3229 0a20 2020 2020 2020  .sendf2).       
+000024a0: 2073 656c 662e 4633 2e73 6574 436f 6e74   self.F3.setCont
+000024b0: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
+000024c0: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
+000024d0: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
+000024e0: 2020 2073 656c 662e 4633 2e63 7573 746f     self.F3.custo
+000024f0: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
+00002500: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
+00002510: 6c66 2e65 6469 745f 4633 290a 2020 2020  lf.edit_F3).    
+00002520: 2020 2020 7365 6c66 2e46 332e 636c 6963      self.F3.clic
+00002530: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
+00002540: 2e73 656e 6466 3329 0a20 2020 2020 2020  .sendf3).       
+00002550: 2073 656c 662e 4634 2e73 6574 436f 6e74   self.F4.setCont
+00002560: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
+00002570: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
+00002580: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
+00002590: 2020 2073 656c 662e 4634 2e63 7573 746f     self.F4.custo
+000025a0: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
+000025b0: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
+000025c0: 6c66 2e65 6469 745f 4634 290a 2020 2020  lf.edit_F4).    
+000025d0: 2020 2020 7365 6c66 2e46 342e 636c 6963      self.F4.clic
+000025e0: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
+000025f0: 2e73 656e 6466 3429 0a20 2020 2020 2020  .sendf4).       
+00002600: 2073 656c 662e 4635 2e73 6574 436f 6e74   self.F5.setCont
+00002610: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
+00002620: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
+00002630: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
+00002640: 2020 2073 656c 662e 4635 2e63 7573 746f     self.F5.custo
+00002650: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
+00002660: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
+00002670: 6c66 2e65 6469 745f 4635 290a 2020 2020  lf.edit_F5).    
+00002680: 2020 2020 7365 6c66 2e46 352e 636c 6963      self.F5.clic
+00002690: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
+000026a0: 2e73 656e 6466 3529 0a20 2020 2020 2020  .sendf5).       
+000026b0: 2073 656c 662e 4636 2e73 6574 436f 6e74   self.F6.setCont
+000026c0: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
+000026d0: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
+000026e0: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
+000026f0: 2020 2073 656c 662e 4636 2e63 7573 746f     self.F6.custo
+00002700: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
+00002710: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
+00002720: 6c66 2e65 6469 745f 4636 290a 2020 2020  lf.edit_F6).    
+00002730: 2020 2020 7365 6c66 2e46 362e 636c 6963      self.F6.clic
+00002740: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
+00002750: 2e73 656e 6466 3629 0a20 2020 2020 2020  .sendf6).       
+00002760: 2073 656c 662e 4637 2e73 6574 436f 6e74   self.F7.setCont
+00002770: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
+00002780: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
+00002790: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
+000027a0: 2020 2073 656c 662e 4637 2e63 7573 746f     self.F7.custo
+000027b0: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
+000027c0: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
+000027d0: 6c66 2e65 6469 745f 4637 290a 2020 2020  lf.edit_F7).    
+000027e0: 2020 2020 7365 6c66 2e46 372e 636c 6963      self.F7.clic
+000027f0: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
+00002800: 2e73 656e 6466 3729 0a20 2020 2020 2020  .sendf7).       
+00002810: 2073 656c 662e 4638 2e73 6574 436f 6e74   self.F8.setCont
+00002820: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
+00002830: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
+00002840: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
+00002850: 2020 2073 656c 662e 4638 2e63 7573 746f     self.F8.custo
+00002860: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
+00002870: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
+00002880: 6c66 2e65 6469 745f 4638 290a 2020 2020  lf.edit_F8).    
+00002890: 2020 2020 7365 6c66 2e46 382e 636c 6963      self.F8.clic
+000028a0: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
+000028b0: 2e73 656e 6466 3829 0a20 2020 2020 2020  .sendf8).       
+000028c0: 2073 656c 662e 4639 2e73 6574 436f 6e74   self.F9.setCont
+000028d0: 6578 744d 656e 7550 6f6c 6963 7928 5174  extMenuPolicy(Qt
+000028e0: 436f 7265 2e51 742e 4375 7374 6f6d 436f  Core.Qt.CustomCo
+000028f0: 6e74 6578 744d 656e 7529 0a20 2020 2020  ntextMenu).     
+00002900: 2020 2073 656c 662e 4639 2e63 7573 746f     self.F9.custo
+00002910: 6d43 6f6e 7465 7874 4d65 6e75 5265 7175  mContextMenuRequ
+00002920: 6573 7465 642e 636f 6e6e 6563 7428 7365  ested.connect(se
+00002930: 6c66 2e65 6469 745f 4639 290a 2020 2020  lf.edit_F9).    
+00002940: 2020 2020 7365 6c66 2e46 392e 636c 6963      self.F9.clic
+00002950: 6b65 642e 636f 6e6e 6563 7428 7365 6c66  ked.connect(self
+00002960: 2e73 656e 6466 3929 0a20 2020 2020 2020  .sendf9).       
+00002970: 2073 656c 662e 4631 302e 7365 7443 6f6e   self.F10.setCon
+00002980: 7465 7874 4d65 6e75 506f 6c69 6379 2851  textMenuPolicy(Q
+00002990: 7443 6f72 652e 5174 2e43 7573 746f 6d43  tCore.Qt.CustomC
+000029a0: 6f6e 7465 7874 4d65 6e75 290a 2020 2020  ontextMenu).    
+000029b0: 2020 2020 7365 6c66 2e46 3130 2e63 7573      self.F10.cus
+000029c0: 746f 6d43 6f6e 7465 7874 4d65 6e75 5265  tomContextMenuRe
+000029d0: 7175 6573 7465 642e 636f 6e6e 6563 7428  quested.connect(
+000029e0: 7365 6c66 2e65 6469 745f 4631 3029 0a20  self.edit_F10). 
+000029f0: 2020 2020 2020 2073 656c 662e 4631 302e         self.F10.
+00002a00: 636c 6963 6b65 642e 636f 6e6e 6563 7428  clicked.connect(
+00002a10: 7365 6c66 2e73 656e 6466 3130 290a 2020  self.sendf10).  
+00002a20: 2020 2020 2020 7365 6c66 2e46 3131 2e73        self.F11.s
+00002a30: 6574 436f 6e74 6578 744d 656e 7550 6f6c  etContextMenuPol
+00002a40: 6963 7928 5174 436f 7265 2e51 742e 4375  icy(QtCore.Qt.Cu
+00002a50: 7374 6f6d 436f 6e74 6578 744d 656e 7529  stomContextMenu)
+00002a60: 0a20 2020 2020 2020 2073 656c 662e 4631  .        self.F1
+00002a70: 312e 6375 7374 6f6d 436f 6e74 6578 744d  1.customContextM
+00002a80: 656e 7552 6571 7565 7374 6564 2e63 6f6e  enuRequested.con
+00002a90: 6e65 6374 2873 656c 662e 6564 6974 5f46  nect(self.edit_F
+00002aa0: 3131 290a 2020 2020 2020 2020 7365 6c66  11).        self
+00002ab0: 2e46 3131 2e63 6c69 636b 6564 2e63 6f6e  .F11.clicked.con
+00002ac0: 6e65 6374 2873 656c 662e 7365 6e64 6631  nect(self.sendf1
+00002ad0: 3129 0a20 2020 2020 2020 2073 656c 662e  1).        self.
+00002ae0: 4631 322e 7365 7443 6f6e 7465 7874 4d65  F12.setContextMe
+00002af0: 6e75 506f 6c69 6379 2851 7443 6f72 652e  nuPolicy(QtCore.
+00002b00: 5174 2e43 7573 746f 6d43 6f6e 7465 7874  Qt.CustomContext
+00002b10: 4d65 6e75 290a 2020 2020 2020 2020 7365  Menu).        se
+00002b20: 6c66 2e46 3132 2e63 7573 746f 6d43 6f6e  lf.F12.customCon
+00002b30: 7465 7874 4d65 6e75 5265 7175 6573 7465  textMenuRequeste
+00002b40: 642e 636f 6e6e 6563 7428 7365 6c66 2e65  d.connect(self.e
+00002b50: 6469 745f 4631 3229 0a20 2020 2020 2020  dit_F12).       
+00002b60: 2073 656c 662e 4631 322e 636c 6963 6b65   self.F12.clicke
+00002b70: 642e 636f 6e6e 6563 7428 7365 6c66 2e73  d.connect(self.s
+00002b80: 656e 6466 3132 290a 0a20 2020 2020 2020  endf12)..       
+00002b90: 2073 656c 662e 7265 6164 7072 6566 6572   self.readprefer
+00002ba0: 656e 6365 7328 290a 2020 2020 2020 2020  ences().        
+00002bb0: 7365 6c66 2e64 626e 616d 6520 3d20 4441  self.dbname = DA
+00002bc0: 5441 5f50 4154 4820 2b20 222f 2220 2b20  TA_PATH + "/" + 
+00002bd0: 7365 6c66 2e70 7265 662e 6765 7428 2263  self.pref.get("c
+00002be0: 7572 7265 6e74 5f64 6174 6162 6173 6522  urrent_database"
+00002bf0: 2c20 2268 616d 2e64 6222 290a 2020 2020  , "ham.db").    
+00002c00: 2020 2020 7365 6c66 2e64 6174 6162 6173      self.databas
+00002c10: 6520 3d20 4461 7461 4261 7365 2873 656c  e = DataBase(sel
+00002c20: 662e 6462 6e61 6d65 2c20 574f 524b 494e  f.dbname, WORKIN
+00002c30: 475f 5041 5448 290a 2020 2020 2020 2020  G_PATH).        
+00002c40: 7365 6c66 2e73 7461 7469 6f6e 203d 2073  self.station = s
+00002c50: 656c 662e 6461 7461 6261 7365 2e66 6574  elf.database.fet
+00002c60: 6368 5f73 7461 7469 6f6e 2829 0a20 2020  ch_station().   
+00002c70: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
+00002c80: 7469 6f6e 2069 7320 4e6f 6e65 3a0a 2020  tion is None:.  
+00002c90: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00002ca0: 7461 7469 6f6e 203d 207b 7d0a 2020 2020  tation = {}.    
+00002cb0: 2020 2020 2020 2020 7365 6c66 2e65 6469          self.edi
+00002cc0: 745f 7374 6174 696f 6e5f 7365 7474 696e  t_station_settin
+00002cd0: 6773 2829 0a20 2020 2020 2020 2020 2020  gs().           
+00002ce0: 2073 656c 662e 7374 6174 696f 6e20 3d20   self.station = 
+00002cf0: 7365 6c66 2e64 6174 6162 6173 652e 6665  self.database.fe
+00002d00: 7463 685f 7374 6174 696f 6e28 290a 2020  tch_station().  
+00002d10: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00002d20: 662e 7374 6174 696f 6e20 6973 204e 6f6e  f.station is Non
+00002d30: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00002d40: 2020 2073 656c 662e 7374 6174 696f 6e20     self.station 
+00002d50: 3d20 7b7d 0a20 2020 2020 2020 2073 656c  = {}.        sel
+00002d60: 662e 636f 6e74 6163 7420 3d20 7365 6c66  f.contact = self
+00002d70: 2e64 6174 6162 6173 652e 656d 7074 795f  .database.empty_
+00002d80: 636f 6e74 6163 740a 2020 2020 2020 2020  contact.        
+00002d90: 7365 6c66 2e63 7572 7265 6e74 5f6f 7020  self.current_op 
+00002da0: 3d20 7365 6c66 2e73 7461 7469 6f6e 2e67  = self.station.g
+00002db0: 6574 2822 4361 6c6c 222c 2022 2229 0a20  et("Call", ""). 
+00002dc0: 2020 2020 2020 2073 656c 662e 6d61 6b65         self.make
+00002dd0: 5f6f 705f 6469 7228 290a 2020 2020 2020  _op_dir().      
+00002de0: 2020 7365 6c66 2e72 6561 645f 6377 5f6d    self.read_cw_m
+00002df0: 6163 726f 7328 290a 2020 2020 2020 2020  acros().        
+00002e00: 7365 6c66 2e63 6c65 6172 696e 7075 7473  self.clearinputs
+00002e10: 2829 0a0a 2020 2020 2020 2020 7365 6c66  ()..        self
+00002e20: 2e62 616e 645f 696e 6469 6361 746f 7273  .band_indicators
+00002e30: 5f63 7720 3d20 7b0a 2020 2020 2020 2020  _cw = {.        
+00002e40: 2020 2020 2231 3630 223a 2073 656c 662e      "160": self.
+00002e50: 6377 5f62 616e 645f 3136 302c 0a20 2020  cw_band_160,.   
+00002e60: 2020 2020 2020 2020 2022 3830 223a 2073           "80": s
+00002e70: 656c 662e 6377 5f62 616e 645f 3830 2c0a  elf.cw_band_80,.
+00002e80: 2020 2020 2020 2020 2020 2020 2234 3022              "40"
+00002e90: 3a20 7365 6c66 2e63 775f 6261 6e64 5f34  : self.cw_band_4
+00002ea0: 302c 0a20 2020 2020 2020 2020 2020 2022  0,.            "
+00002eb0: 3230 223a 2073 656c 662e 6377 5f62 616e  20": self.cw_ban
+00002ec0: 645f 3230 2c0a 2020 2020 2020 2020 2020  d_20,.          
+00002ed0: 2020 2231 3522 3a20 7365 6c66 2e63 775f    "15": self.cw_
+00002ee0: 6261 6e64 5f31 352c 0a20 2020 2020 2020  band_15,.       
+00002ef0: 2020 2020 2022 3130 223a 2073 656c 662e       "10": self.
+00002f00: 6377 5f62 616e 645f 3130 2c0a 2020 2020  cw_band_10,.    
+00002f10: 2020 2020 7d0a 0a20 2020 2020 2020 2073      }..        s
+00002f20: 656c 662e 6261 6e64 5f69 6e64 6963 6174  elf.band_indicat
+00002f30: 6f72 735f 7373 6220 3d20 7b0a 2020 2020  ors_ssb = {.    
+00002f40: 2020 2020 2020 2020 2231 3630 223a 2073          "160": s
+00002f50: 656c 662e 7373 625f 6261 6e64 5f31 3630  elf.ssb_band_160
+00002f60: 2c0a 2020 2020 2020 2020 2020 2020 2238  ,.            "8
+00002f70: 3022 3a20 7365 6c66 2e73 7362 5f62 616e  0": self.ssb_ban
+00002f80: 645f 3830 2c0a 2020 2020 2020 2020 2020  d_80,.          
+00002f90: 2020 2234 3022 3a20 7365 6c66 2e73 7362    "40": self.ssb
+00002fa0: 5f62 616e 645f 3430 2c0a 2020 2020 2020  _band_40,.      
+00002fb0: 2020 2020 2020 2232 3022 3a20 7365 6c66        "20": self
+00002fc0: 2e73 7362 5f62 616e 645f 3230 2c0a 2020  .ssb_band_20,.  
+00002fd0: 2020 2020 2020 2020 2020 2231 3522 3a20            "15": 
+00002fe0: 7365 6c66 2e73 7362 5f62 616e 645f 3135  self.ssb_band_15
+00002ff0: 2c0a 2020 2020 2020 2020 2020 2020 2231  ,.            "1
+00003000: 3022 3a20 7365 6c66 2e73 7362 5f62 616e  0": self.ssb_ban
+00003010: 645f 3130 2c0a 2020 2020 2020 2020 7d0a  d_10,.        }.
+00003020: 0a20 2020 2020 2020 2073 656c 662e 6261  .        self.ba
+00003030: 6e64 5f69 6e64 6963 6174 6f72 735f 7274  nd_indicators_rt
+00003040: 7479 203d 207b 0a20 2020 2020 2020 2020  ty = {.         
+00003050: 2020 2022 3136 3022 3a20 7365 6c66 2e72     "160": self.r
+00003060: 7474 795f 6261 6e64 5f31 3630 2c0a 2020  tty_band_160,.  
+00003070: 2020 2020 2020 2020 2020 2238 3022 3a20            "80": 
+00003080: 7365 6c66 2e72 7474 795f 6261 6e64 5f38  self.rtty_band_8
+00003090: 302c 0a20 2020 2020 2020 2020 2020 2022  0,.            "
+000030a0: 3430 223a 2073 656c 662e 7274 7479 5f62  40": self.rtty_b
+000030b0: 616e 645f 3430 2c0a 2020 2020 2020 2020  and_40,.        
+000030c0: 2020 2020 2232 3022 3a20 7365 6c66 2e72      "20": self.r
+000030d0: 7474 795f 6261 6e64 5f32 302c 0a20 2020  tty_band_20,.   
+000030e0: 2020 2020 2020 2020 2022 3135 223a 2073           "15": s
+000030f0: 656c 662e 7274 7479 5f62 616e 645f 3135  elf.rtty_band_15
+00003100: 2c0a 2020 2020 2020 2020 2020 2020 2231  ,.            "1
+00003110: 3022 3a20 7365 6c66 2e72 7474 795f 6261  0": self.rtty_ba
+00003120: 6e64 5f31 302c 0a20 2020 2020 2020 207d  nd_10,.        }
+00003130: 0a0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
+00003140: 6c6c 5f6d 6f64 655f 696e 6469 6361 746f  ll_mode_indicato
+00003150: 7273 203d 207b 0a20 2020 2020 2020 2020  rs = {.         
+00003160: 2020 2022 4357 223a 2073 656c 662e 6261     "CW": self.ba
+00003170: 6e64 5f69 6e64 6963 6174 6f72 735f 6377  nd_indicators_cw
+00003180: 2c0a 2020 2020 2020 2020 2020 2020 2253  ,.            "S
+00003190: 5342 223a 2073 656c 662e 6261 6e64 5f69  SB": self.band_i
+000031a0: 6e64 6963 6174 6f72 735f 7373 622c 0a20  ndicators_ssb,. 
+000031b0: 2020 2020 2020 2020 2020 2022 5254 5459             "RTTY
+000031c0: 223a 2073 656c 662e 6261 6e64 5f69 6e64  ": self.band_ind
+000031d0: 6963 6174 6f72 735f 7274 7479 2c0a 2020  icators_rtty,.  
+000031e0: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
+000031f0: 2069 6620 7365 6c66 2e70 7265 662e 6765   if self.pref.ge
+00003200: 7428 2263 6f6e 7465 7374 2229 3a0a 2020  t("contest"):.  
+00003210: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
+00003220: 6f61 645f 636f 6e74 6573 7428 290a 0a20  oad_contest().. 
+00003230: 2020 2020 2020 2069 6620 5665 7273 696f         if Versio
+00003240: 6e54 6573 7428 5f5f 7665 7273 696f 6e5f  nTest(__version_
+00003250: 5f29 2e74 6573 7428 293a 0a20 2020 2020  _).test():.     
+00003260: 2020 2020 2020 2073 656c 662e 7368 6f77         self.show
+00003270: 5f6d 6573 7361 6765 5f62 6f78 280a 2020  _message_box(.  
+00003280: 2020 2020 2020 2020 2020 2020 2020 2254                "T
+00003290: 6865 7265 2069 7320 6120 6e65 7765 7220  here is a newer 
+000032a0: 7665 7273 696f 6e20 6f66 206e 6f74 316d  version of not1m
+000032b0: 6d20 6176 6169 6c61 626c 652e 5c6e 220a  m available.\n".
+000032c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032d0: 2259 6f75 2063 616e 2075 6461 7465 2074  "You can udate t
+000032e0: 6f20 7468 6520 6375 7272 656e 7420 7665  o the current ve
+000032f0: 7273 696f 6e20 6279 2075 7369 6e67 3a5c  rsion by using:\
+00003300: 6e70 6970 2069 6e73 7461 6c6c 202d 5520  npip install -U 
+00003310: 6e6f 7431 6d6d 220a 2020 2020 2020 2020  not1mm".        
+00003320: 2020 2020 290a 0a20 2020 2064 6566 2071      )..    def q
+00003330: 7569 745f 6170 7028 7365 6c66 293a 0a20  uit_app(self):. 
+00003340: 2020 2020 2020 2022 2222 646f 6322 2222         """doc"""
+00003350: 0a20 2020 2020 2020 2063 6d64 203d 207b  .        cmd = {
+00003360: 7d0a 2020 2020 2020 2020 636d 645b 2263  }.        cmd["c
+00003370: 6d64 225d 203d 2022 4841 4c54 220a 2020  md"] = "HALT".  
+00003380: 2020 2020 2020 636d 645b 2273 7461 7469        cmd["stati
+00003390: 6f6e 225d 203d 2070 6c61 7466 6f72 6d2e  on"] = platform.
+000033a0: 6e6f 6465 2829 0a20 2020 2020 2020 2073  node().        s
+000033b0: 656c 662e 6d75 6c74 6963 6173 745f 696e  elf.multicast_in
+000033c0: 7465 7266 6163 652e 7365 6e64 5f61 735f  terface.send_as_
+000033d0: 6a73 6f6e 2863 6d64 290a 2020 2020 2020  json(cmd).      
+000033e0: 2020 6170 702e 7175 6974 2829 0a0a 2020    app.quit()..  
+000033f0: 2020 4073 7461 7469 636d 6574 686f 640a    @staticmethod.
+00003400: 2020 2020 6465 6620 6368 6563 6b5f 7072      def check_pr
+00003410: 6f63 6573 7328 6e61 6d65 3a20 7374 7229  ocess(name: str)
+00003420: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
+00003430: 2020 2222 2263 6865 636b 7320 746f 2073    """checks to s
+00003440: 6565 2069 6620 7072 6f67 7261 6d20 6f66  ee if program of
+00003450: 206e 616d 6520 6973 2069 6e20 7468 6520   name is in the 
+00003460: 6163 7469 7665 2070 726f 6365 7373 206c  active process l
+00003470: 6973 7422 2222 0a20 2020 2020 2020 2066  ist""".        f
+00003480: 6f72 2070 726f 6320 696e 2070 7375 7469  or proc in psuti
+00003490: 6c2e 7072 6f63 6573 735f 6974 6572 2829  l.process_iter()
+000034a0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+000034b0: 2062 6f6f 6c28 7265 2e6d 6174 6368 286e   bool(re.match(n
+000034c0: 616d 652c 2070 726f 632e 6e61 6d65 2829  ame, proc.name()
+000034d0: 2e6c 6f77 6572 2829 2929 3a0a 2020 2020  .lower())):.    
+000034e0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000034f0: 726e 2054 7275 650a 2020 2020 2020 2020  rn True.        
+00003500: 7265 7475 726e 2046 616c 7365 0a0a 2020  return False..  
+00003510: 2020 6465 6620 7368 6f77 5f6d 6573 7361    def show_messa
+00003520: 6765 5f62 6f78 2873 656c 662c 206d 6573  ge_box(self, mes
+00003530: 7361 6765 3a20 7374 7229 202d 3e20 4e6f  sage: str) -> No
+00003540: 6e65 3a0a 2020 2020 2020 2020 2222 2264  ne:.        """d
+00003550: 6f63 2222 220a 2020 2020 2020 2020 6d65  oc""".        me
+00003560: 7373 6167 655f 626f 7820 3d20 5174 5769  ssage_box = QtWi
+00003570: 6467 6574 732e 514d 6573 7361 6765 426f  dgets.QMessageBo
+00003580: 7828 290a 2020 2020 2020 2020 6d65 7373  x().        mess
+00003590: 6167 655f 626f 782e 7365 7449 636f 6e28  age_box.setIcon(
+000035a0: 5174 5769 6467 6574 732e 514d 6573 7361  QtWidgets.QMessa
+000035b0: 6765 426f 782e 496e 666f 726d 6174 696f  geBox.Informatio
+000035c0: 6e29 0a20 2020 2020 2020 206d 6573 7361  n).        messa
+000035d0: 6765 5f62 6f78 2e73 6574 5465 7874 286d  ge_box.setText(m
+000035e0: 6573 7361 6765 290a 2020 2020 2020 2020  essage).        
+000035f0: 6d65 7373 6167 655f 626f 782e 7365 7457  message_box.setW
+00003600: 696e 646f 7754 6974 6c65 2822 496e 666f  indowTitle("Info
+00003610: 726d 6174 696f 6e22 290a 2020 2020 2020  rmation").      
+00003620: 2020 6d65 7373 6167 655f 626f 782e 7365    message_box.se
+00003630: 7453 7461 6e64 6172 6442 7574 746f 6e73  tStandardButtons
+00003640: 2851 7457 6964 6765 7473 2e51 4d65 7373  (QtWidgets.QMess
+00003650: 6167 6542 6f78 2e4f 6b29 0a20 2020 2020  ageBox.Ok).     
+00003660: 2020 205f 203d 206d 6573 7361 6765 5f62     _ = message_b
+00003670: 6f78 2e65 7865 635f 2829 0a0a 2020 2020  ox.exec_()..    
+00003680: 6465 6620 7368 6f77 5f61 626f 7574 5f64  def show_about_d
+00003690: 6961 6c6f 6728 7365 6c66 293a 0a20 2020  ialog(self):.   
+000036a0: 2020 2020 2022 2222 5368 6f77 2061 626f       """Show abo
+000036b0: 7574 2064 6961 6c6f 6722 2222 0a20 2020  ut dialog""".   
+000036c0: 2020 2020 2073 656c 662e 6162 6f75 745f       self.about_
+000036d0: 6469 616c 6f67 203d 2041 626f 7574 2857  dialog = About(W
+000036e0: 4f52 4b49 4e47 5f50 4154 4829 0a20 2020  ORKING_PATH).   
+000036f0: 2020 2020 2073 656c 662e 6162 6f75 745f       self.about_
+00003700: 6469 616c 6f67 2e64 6f6e 6f72 732e 7365  dialog.donors.se
+00003710: 7453 6f75 7263 6528 0a20 2020 2020 2020  tSource(.       
+00003720: 2020 2020 2051 7443 6f72 652e 5155 726c       QtCore.QUrl
+00003730: 2e66 726f 6d4c 6f63 616c 4669 6c65 2857  .fromLocalFile(W
+00003740: 4f52 4b49 4e47 5f50 4154 4820 2b20 222f  ORKING_PATH + "/
+00003750: 6461 7461 2f64 6f6e 6f72 732e 6874 6d6c  data/donors.html
+00003760: 2229 0a20 2020 2020 2020 2029 0a20 2020  ").        ).   
+00003770: 2020 2020 2073 656c 662e 6162 6f75 745f       self.about_
+00003780: 6469 616c 6f67 2e6f 7065 6e28 290a 0a20  dialog.open().. 
+00003790: 2020 2064 6566 2073 686f 775f 6865 6c70     def show_help
+000037a0: 5f64 6961 6c6f 6728 7365 6c66 293a 0a20  _dialog(self):. 
+000037b0: 2020 2020 2020 2022 2222 5368 6f77 2061         """Show a
+000037c0: 626f 7574 2064 6961 6c6f 6722 2222 0a20  bout dialog""". 
+000037d0: 2020 2020 2020 2073 656c 662e 6162 6f75         self.abou
+000037e0: 745f 6469 616c 6f67 203d 2041 626f 7574  t_dialog = About
+000037f0: 2857 4f52 4b49 4e47 5f50 4154 4829 0a20  (WORKING_PATH). 
+00003800: 2020 2020 2020 2073 656c 662e 6162 6f75         self.abou
+00003810: 745f 6469 616c 6f67 2e73 6574 5769 6e64  t_dialog.setWind
+00003820: 6f77 5469 746c 6528 2248 656c 7022 290a  owTitle("Help").
+00003830: 2020 2020 2020 2020 7365 6c66 2e61 626f          self.abo
+00003840: 7574 5f64 6961 6c6f 672e 7365 7447 656f  ut_dialog.setGeo
+00003850: 6d65 7472 7928 302c 2030 2c20 3830 302c  metry(0, 0, 800,
+00003860: 2036 3030 290a 2020 2020 2020 2020 7365   600).        se
+00003870: 6c66 2e61 626f 7574 5f64 6961 6c6f 672e  lf.about_dialog.
+00003880: 646f 6e6f 7273 2e73 6574 536f 7572 6365  donors.setSource
+00003890: 280a 2020 2020 2020 2020 2020 2020 5174  (.            Qt
+000038a0: 436f 7265 2e51 5572 6c2e 6672 6f6d 4c6f  Core.QUrl.fromLo
+000038b0: 6361 6c46 696c 6528 574f 524b 494e 475f  calFile(WORKING_
+000038c0: 5041 5448 202b 2022 2f64 6174 612f 6e6f  PATH + "/data/no
+000038d0: 7431 6d6d 2e68 746d 6c22 290a 2020 2020  t1mm.html").    
+000038e0: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
+000038f0: 6c66 2e61 626f 7574 5f64 6961 6c6f 672e  lf.about_dialog.
+00003900: 6f70 656e 2829 0a0a 2020 2020 6465 6620  open()..    def 
+00003910: 7570 6461 7465 5f6d 6173 7465 7273 6370  update_masterscp
+00003920: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
+00003930: 2020 2020 2020 2020 2222 2255 7064 6174          """Updat
+00003940: 6520 7468 6520 4d41 5354 4552 2e53 4350  e the MASTER.SCP
+00003950: 2066 696c 652e 2222 220a 2020 2020 2020   file.""".      
+00003960: 2020 6966 2073 656c 662e 6d73 6370 2e75    if self.mscp.u
+00003970: 7064 6174 655f 6d61 7374 6572 7363 7028  pdate_masterscp(
+00003980: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+00003990: 656c 662e 7368 6f77 5f6d 6573 7361 6765  elf.show_message
+000039a0: 5f62 6f78 2822 4d41 5354 4552 2e53 4350  _box("MASTER.SCP
+000039b0: 2066 696c 6520 7570 6461 7465 642e 2229   file updated.")
+000039c0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000039d0: 7572 6e0a 2020 2020 2020 2020 7365 6c66  urn.        self
+000039e0: 2e73 686f 775f 6d65 7373 6167 655f 626f  .show_message_bo
+000039f0: 7828 224d 4153 5445 522e 5343 5020 636f  x("MASTER.SCP co
+00003a00: 756c 6420 6e6f 7420 6265 2075 7064 6174  uld not be updat
+00003a10: 6564 2e22 290a 0a20 2020 2064 6566 2065  ed.")..    def e
+00003a20: 6469 745f 636f 6e66 6967 7572 6174 696f  dit_configuratio
+00003a30: 6e5f 7365 7474 696e 6773 2873 656c 6629  n_settings(self)
+00003a40: 3a0a 2020 2020 2020 2020 2222 2243 6f6e  :.        """Con
+00003a50: 6669 6775 7261 7469 6f6e 2053 6574 7469  figuration Setti
+00003a60: 6e67 7320 7761 7320 636c 6963 6b65 6422  ngs was clicked"
+00003a70: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
+00003a80: 636f 6e66 6967 7572 6174 696f 6e5f 6469  configuration_di
+00003a90: 616c 6f67 203d 2053 6574 7469 6e67 7328  alog = Settings(
+00003aa0: 574f 524b 494e 475f 5041 5448 2c20 434f  WORKING_PATH, CO
+00003ab0: 4e46 4947 5f50 4154 482c 2073 656c 662e  NFIG_PATH, self.
+00003ac0: 7072 6566 290a 2020 2020 2020 2020 7365  pref).        se
+00003ad0: 6c66 2e63 6f6e 6669 6775 7261 7469 6f6e  lf.configuration
+00003ae0: 5f64 6961 6c6f 672e 7573 6568 616d 6462  _dialog.usehamdb
+00003af0: 5f72 6164 696f 4275 7474 6f6e 2e68 6964  _radioButton.hid
+00003b00: 6528 290a 2020 2020 2020 2020 7365 6c66  e().        self
+00003b10: 2e63 6f6e 6669 6775 7261 7469 6f6e 5f64  .configuration_d
+00003b20: 6961 6c6f 672e 7368 6f77 2829 0a20 2020  ialog.show().   
+00003b30: 2020 2020 2073 656c 662e 636f 6e66 6967       self.config
+00003b40: 7572 6174 696f 6e5f 6469 616c 6f67 2e61  uration_dialog.a
+00003b50: 6363 6570 7465 642e 636f 6e6e 6563 7428  ccepted.connect(
+00003b60: 7365 6c66 2e65 6469 745f 636f 6e66 6967  self.edit_config
+00003b70: 7572 6174 696f 6e5f 7265 7475 726e 290a  uration_return).
+00003b80: 0a20 2020 2064 6566 2065 6469 745f 636f  .    def edit_co
+00003b90: 6e66 6967 7572 6174 696f 6e5f 7265 7475  nfiguration_retu
+00003ba0: 726e 2873 656c 6629 3a0a 2020 2020 2020  rn(self):.      
+00003bb0: 2020 2222 2252 6574 7572 6e73 2068 6572    """Returns her
+00003bc0: 6520 7768 656e 2063 6f6e 6669 6775 7261  e when configura
+00003bd0: 7469 6f6e 2064 6961 6c6f 6720 636c 6f73  tion dialog clos
+00003be0: 6564 2077 6974 6820 6f6b 6179 2e22 2222  ed with okay."""
+00003bf0: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
+00003c00: 6e66 6967 7572 6174 696f 6e5f 6469 616c  nfiguration_dial
+00003c10: 6f67 2e73 6176 655f 6368 616e 6765 7328  og.save_changes(
+00003c20: 290a 2020 2020 2020 2020 7365 6c66 2e77  ).        self.w
+00003c30: 7269 7465 5f70 7265 6665 7265 6e63 6528  rite_preference(
+00003c40: 290a 2020 2020 2020 2020 6c6f 6767 6572  ).        logger
+00003c50: 2e64 6562 7567 2822 2573 222c 2066 227b  .debug("%s", f"{
+00003c60: 7365 6c66 2e70 7265 667d 2229 0a20 2020  self.pref}").   
+00003c70: 2020 2020 2073 656c 662e 7265 6164 7072       self.readpr
+00003c80: 6566 6572 656e 6365 7328 290a 0a20 2020  eferences()..   
+00003c90: 2064 6566 206e 6577 5f64 6174 6162 6173   def new_databas
+00003ca0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+00003cb0: 2022 2222 4372 6561 7465 206e 6577 2064   """Create new d
+00003cc0: 6174 6162 6173 652e 2222 220a 2020 2020  atabase.""".    
+00003cd0: 2020 2020 6669 6c65 6e61 6d65 203d 2073      filename = s
+00003ce0: 656c 662e 6669 6c65 7069 636b 6572 2822  elf.filepicker("
+00003cf0: 6e65 7722 290a 2020 2020 2020 2020 6966  new").        if
+00003d00: 2066 696c 656e 616d 653a 0a20 2020 2020   filename:.     
+00003d10: 2020 2020 2020 2069 6620 6669 6c65 6e61         if filena
+00003d20: 6d65 5b2d 333a 5d20 213d 2022 2e64 6222  me[-3:] != ".db"
+00003d30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00003d40: 2020 6669 6c65 6e61 6d65 202b 3d20 222e    filename += ".
+00003d50: 6462 220a 2020 2020 2020 2020 2020 2020  db".            
+00003d60: 7365 6c66 2e70 7265 665b 2263 7572 7265  self.pref["curre
+00003d70: 6e74 5f64 6174 6162 6173 6522 5d20 3d20  nt_database"] = 
+00003d80: 6669 6c65 6e61 6d65 2e73 706c 6974 2822  filename.split("
+00003d90: 2f22 295b 2d31 3a5d 5b30 5d0a 2020 2020  /")[-1:][0].    
+00003da0: 2020 2020 2020 2020 7365 6c66 2e77 7269          self.wri
+00003db0: 7465 5f70 7265 6665 7265 6e63 6528 290a  te_preference().
+00003dc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003dd0: 2e64 626e 616d 6520 3d20 4441 5441 5f50  .dbname = DATA_P
+00003de0: 4154 4820 2b20 222f 2220 2b20 7365 6c66  ATH + "/" + self
+00003df0: 2e70 7265 662e 6765 7428 2263 7572 7265  .pref.get("curre
+00003e00: 6e74 5f64 6174 6162 6173 6522 2c20 2268  nt_database", "h
+00003e10: 616d 2e64 6222 290a 2020 2020 2020 2020  am.db").        
+00003e20: 2020 2020 7365 6c66 2e64 6174 6162 6173      self.databas
+00003e30: 6520 3d20 4461 7461 4261 7365 2873 656c  e = DataBase(sel
+00003e40: 662e 6462 6e61 6d65 2c20 574f 524b 494e  f.dbname, WORKIN
+00003e50: 475f 5041 5448 290a 2020 2020 2020 2020  G_PATH).        
+00003e60: 2020 2020 7365 6c66 2e63 6f6e 7461 6374      self.contact
+00003e70: 203d 2073 656c 662e 6461 7461 6261 7365   = self.database
+00003e80: 2e65 6d70 7479 5f63 6f6e 7461 6374 0a20  .empty_contact. 
+00003e90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003ea0: 7374 6174 696f 6e20 3d20 7365 6c66 2e64  station = self.d
+00003eb0: 6174 6162 6173 652e 6665 7463 685f 7374  atabase.fetch_st
+00003ec0: 6174 696f 6e28 290a 2020 2020 2020 2020  ation().        
+00003ed0: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
+00003ee0: 696f 6e20 6973 204e 6f6e 653a 0a20 2020  ion is None:.   
+00003ef0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00003f00: 662e 7374 6174 696f 6e20 3d20 7b7d 0a20  f.station = {}. 
+00003f10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003f20: 6375 7272 656e 745f 6f70 203d 2073 656c  current_op = sel
+00003f30: 662e 7374 6174 696f 6e2e 6765 7428 2243  f.station.get("C
+00003f40: 616c 6c22 2c20 2222 290a 2020 2020 2020  all", "").      
+00003f50: 2020 2020 2020 7365 6c66 2e6d 616b 655f        self.make_
+00003f60: 6f70 5f64 6972 2829 0a20 2020 2020 2020  op_dir().       
+00003f70: 2020 2020 2063 6d64 203d 207b 7d0a 2020       cmd = {}.  
+00003f80: 2020 2020 2020 2020 2020 636d 645b 2263            cmd["c
+00003f90: 6d64 225d 203d 2022 4e45 5744 4222 0a20  md"] = "NEWDB". 
+00003fa0: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
+00003fb0: 7374 6174 696f 6e22 5d20 3d20 706c 6174  station"] = plat
+00003fc0: 666f 726d 2e6e 6f64 6528 290a 2020 2020  form.node().    
+00003fd0: 2020 2020 2020 2020 7365 6c66 2e6d 756c          self.mul
+00003fe0: 7469 6361 7374 5f69 6e74 6572 6661 6365  ticast_interface
+00003ff0: 2e73 656e 645f 6173 5f6a 736f 6e28 636d  .send_as_json(cm
+00004000: 6429 0a20 2020 2020 2020 2020 2020 2073  d).            s
+00004010: 656c 662e 636c 6561 7269 6e70 7574 7328  elf.clearinputs(
+00004020: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00004030: 6c66 2e65 6469 745f 7374 6174 696f 6e5f  lf.edit_station_
+00004040: 7365 7474 696e 6773 2829 0a0a 2020 2020  settings()..    
+00004050: 6465 6620 6f70 656e 5f64 6174 6162 6173  def open_databas
+00004060: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+00004070: 2022 2222 4f70 656e 2065 7869 7374 696e   """Open existin
+00004080: 6720 6461 7461 6261 7365 2e22 2222 0a20  g database.""". 
+00004090: 2020 2020 2020 2066 696c 656e 616d 6520         filename 
+000040a0: 3d20 7365 6c66 2e66 696c 6570 6963 6b65  = self.filepicke
+000040b0: 7228 226f 7065 6e22 290a 2020 2020 2020  r("open").      
+000040c0: 2020 6966 2066 696c 656e 616d 653a 0a20    if filename:. 
+000040d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000040e0: 7072 6566 5b22 6375 7272 656e 745f 6461  pref["current_da
+000040f0: 7461 6261 7365 225d 203d 2066 696c 656e  tabase"] = filen
+00004100: 616d 652e 7370 6c69 7428 222f 2229 5b2d  ame.split("/")[-
+00004110: 313a 5d5b 305d 0a20 2020 2020 2020 2020  1:][0].         
+00004120: 2020 2073 656c 662e 7772 6974 655f 7072     self.write_pr
+00004130: 6566 6572 656e 6365 2829 0a20 2020 2020  eference().     
+00004140: 2020 2020 2020 2073 656c 662e 6462 6e61         self.dbna
+00004150: 6d65 203d 2044 4154 415f 5041 5448 202b  me = DATA_PATH +
+00004160: 2022 2f22 202b 2073 656c 662e 7072 6566   "/" + self.pref
+00004170: 2e67 6574 2822 6375 7272 656e 745f 6461  .get("current_da
+00004180: 7461 6261 7365 222c 2022 6861 6d2e 6462  tabase", "ham.db
+00004190: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
+000041a0: 656c 662e 6461 7461 6261 7365 203d 2044  elf.database = D
+000041b0: 6174 6142 6173 6528 7365 6c66 2e64 626e  ataBase(self.dbn
+000041c0: 616d 652c 2057 4f52 4b49 4e47 5f50 4154  ame, WORKING_PAT
+000041d0: 4829 0a20 2020 2020 2020 2020 2020 2073  H).            s
+000041e0: 656c 662e 636f 6e74 6163 7420 3d20 7365  elf.contact = se
+000041f0: 6c66 2e64 6174 6162 6173 652e 656d 7074  lf.database.empt
+00004200: 795f 636f 6e74 6163 740a 2020 2020 2020  y_contact.      
+00004210: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
+00004220: 6f6e 203d 2073 656c 662e 6461 7461 6261  on = self.databa
+00004230: 7365 2e66 6574 6368 5f73 7461 7469 6f6e  se.fetch_station
+00004240: 2829 0a20 2020 2020 2020 2020 2020 2069  ().            i
+00004250: 6620 7365 6c66 2e73 7461 7469 6f6e 2069  f self.station i
+00004260: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00004270: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+00004280: 7469 6f6e 203d 207b 7d0a 2020 2020 2020  tion = {}.      
+00004290: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
+000042a0: 6174 696f 6e2e 6765 7428 2243 616c 6c22  ation.get("Call"
+000042b0: 2c20 2222 2920 3d3d 2022 223a 0a20 2020  , "") == "":.   
+000042c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000042d0: 662e 6564 6974 5f73 7461 7469 6f6e 5f73  f.edit_station_s
+000042e0: 6574 7469 6e67 7328 290a 2020 2020 2020  ettings().      
+000042f0: 2020 2020 2020 7365 6c66 2e63 7572 7265        self.curre
+00004300: 6e74 5f6f 7020 3d20 7365 6c66 2e73 7461  nt_op = self.sta
+00004310: 7469 6f6e 2e67 6574 2822 4361 6c6c 222c  tion.get("Call",
+00004320: 2022 2229 0a20 2020 2020 2020 2020 2020   "").           
+00004330: 2073 656c 662e 6d61 6b65 5f6f 705f 6469   self.make_op_di
+00004340: 7228 290a 2020 2020 2020 2020 2020 2020  r().            
+00004350: 636d 6420 3d20 7b7d 0a20 2020 2020 2020  cmd = {}.       
+00004360: 2020 2020 2063 6d64 5b22 636d 6422 5d20       cmd["cmd"] 
+00004370: 3d20 224e 4557 4442 220a 2020 2020 2020  = "NEWDB".      
+00004380: 2020 2020 2020 636d 645b 2273 7461 7469        cmd["stati
+00004390: 6f6e 225d 203d 2070 6c61 7466 6f72 6d2e  on"] = platform.
+000043a0: 6e6f 6465 2829 0a20 2020 2020 2020 2020  node().         
+000043b0: 2020 2073 656c 662e 6d75 6c74 6963 6173     self.multicas
+000043c0: 745f 696e 7465 7266 6163 652e 7365 6e64  t_interface.send
+000043d0: 5f61 735f 6a73 6f6e 2863 6d64 290a 2020  _as_json(cmd).  
+000043e0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+000043f0: 6c65 6172 696e 7075 7473 2829 0a0a 2020  learinputs()..  
+00004400: 2020 6465 6620 6e65 775f 636f 6e74 6573    def new_contes
+00004410: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+00004420: 2022 2222 4372 6561 7465 206e 6577 2063   """Create new c
+00004430: 6f6e 7465 7374 2069 6e20 6578 6973 7469  ontest in existi
+00004440: 6e67 2064 6174 6162 6173 652e 2222 220a  ng database.""".
+00004450: 0a20 2020 2064 6566 206f 7065 6e5f 636f  .    def open_co
+00004460: 6e74 6573 7428 7365 6c66 293a 0a20 2020  ntest(self):.   
+00004470: 2020 2020 2022 2222 5377 6974 6368 2074       """Switch t
+00004480: 6f20 6120 6469 6666 6572 656e 7420 6578  o a different ex
+00004490: 6973 7469 6e67 2063 6f6e 7465 7374 2069  isting contest i
+000044a0: 6e20 6578 6973 7469 6e67 2064 6174 6162  n existing datab
+000044b0: 6173 652e 2222 220a 2020 2020 2020 2020  ase.""".        
+000044c0: 6c6f 6767 6572 2e64 6562 7567 2822 4f70  logger.debug("Op
+000044d0: 656e 2043 6f6e 7465 7374 2073 656c 6563  en Contest selec
+000044e0: 7465 6422 290a 2020 2020 2020 2020 636f  ted").        co
+000044f0: 6e74 6573 7473 203d 2073 656c 662e 6461  ntests = self.da
+00004500: 7461 6261 7365 2e66 6574 6368 5f61 6c6c  tabase.fetch_all
+00004510: 5f63 6f6e 7465 7374 7328 290a 2020 2020  _contests().    
+00004520: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+00004530: 2822 2573 222c 2066 227b 636f 6e74 6573  ("%s", f"{contes
+00004540: 7473 7d22 290a 0a20 2020 2020 2020 2069  ts}")..        i
+00004550: 6620 636f 6e74 6573 7473 3a0a 2020 2020  f contests:.    
+00004560: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+00004570: 7465 7374 5f64 6961 6c6f 6720 3d20 5365  test_dialog = Se
+00004580: 6c65 6374 436f 6e74 6573 7428 574f 524b  lectContest(WORK
+00004590: 494e 475f 5041 5448 290a 2020 2020 2020  ING_PATH).      
+000045a0: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
+000045b0: 7374 5f64 6961 6c6f 672e 636f 6e74 6573  st_dialog.contes
+000045c0: 745f 6c69 7374 2e73 6574 526f 7743 6f75  t_list.setRowCou
+000045d0: 6e74 2830 290a 2020 2020 2020 2020 2020  nt(0).          
+000045e0: 2020 7365 6c66 2e63 6f6e 7465 7374 5f64    self.contest_d
+000045f0: 6961 6c6f 672e 636f 6e74 6573 745f 6c69  ialog.contest_li
+00004600: 7374 2e73 6574 436f 6c75 6d6e 436f 756e  st.setColumnCoun
+00004610: 7428 3429 0a20 2020 2020 2020 2020 2020  t(4).           
+00004620: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+00004630: 616c 6f67 2e63 6f6e 7465 7374 5f6c 6973  alog.contest_lis
+00004640: 742e 7665 7274 6963 616c 4865 6164 6572  t.verticalHeader
+00004650: 2829 2e73 6574 5669 7369 626c 6528 4661  ().setVisible(Fa
+00004660: 6c73 6529 0a20 2020 2020 2020 2020 2020  lse).           
+00004670: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+00004680: 616c 6f67 2e63 6f6e 7465 7374 5f6c 6973  alog.contest_lis
+00004690: 742e 7365 7443 6f6c 756d 6e57 6964 7468  t.setColumnWidth
+000046a0: 2831 2c20 3230 3029 0a20 2020 2020 2020  (1, 200).       
+000046b0: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
+000046c0: 745f 6469 616c 6f67 2e63 6f6e 7465 7374  t_dialog.contest
+000046d0: 5f6c 6973 742e 7365 7443 6f6c 756d 6e57  _list.setColumnW
+000046e0: 6964 7468 2832 2c20 3230 3029 0a20 2020  idth(2, 200).   
+000046f0: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+00004700: 6e74 6573 745f 6469 616c 6f67 2e63 6f6e  ntest_dialog.con
+00004710: 7465 7374 5f6c 6973 742e 7365 7448 6f72  test_list.setHor
+00004720: 697a 6f6e 7461 6c48 6561 6465 7249 7465  izontalHeaderIte
+00004730: 6d28 0a20 2020 2020 2020 2020 2020 2020  m(.             
+00004740: 2020 2030 2c20 5174 5769 6467 6574 732e     0, QtWidgets.
+00004750: 5154 6162 6c65 5769 6467 6574 4974 656d  QTableWidgetItem
+00004760: 2822 436f 6e74 6573 7420 4e72 2229 0a20  ("Contest Nr"). 
+00004770: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00004780: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+00004790: 6e74 6573 745f 6469 616c 6f67 2e63 6f6e  ntest_dialog.con
+000047a0: 7465 7374 5f6c 6973 742e 7365 7448 6f72  test_list.setHor
+000047b0: 697a 6f6e 7461 6c48 6561 6465 7249 7465  izontalHeaderIte
+000047c0: 6d28 0a20 2020 2020 2020 2020 2020 2020  m(.             
+000047d0: 2020 2031 2c20 5174 5769 6467 6574 732e     1, QtWidgets.
+000047e0: 5154 6162 6c65 5769 6467 6574 4974 656d  QTableWidgetItem
+000047f0: 2822 436f 6e74 6573 7420 4e61 6d65 2229  ("Contest Name")
+00004800: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00004810: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00004820: 636f 6e74 6573 745f 6469 616c 6f67 2e63  contest_dialog.c
+00004830: 6f6e 7465 7374 5f6c 6973 742e 7365 7448  ontest_list.setH
+00004840: 6f72 697a 6f6e 7461 6c48 6561 6465 7249  orizontalHeaderI
+00004850: 7465 6d28 0a20 2020 2020 2020 2020 2020  tem(.           
+00004860: 2020 2020 2032 2c20 5174 5769 6467 6574       2, QtWidget
+00004870: 732e 5154 6162 6c65 5769 6467 6574 4974  s.QTableWidgetIt
+00004880: 656d 2822 436f 6e74 6573 7420 5374 6172  em("Contest Star
+00004890: 7422 290a 2020 2020 2020 2020 2020 2020  t").            
+000048a0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+000048b0: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
+000048c0: 672e 636f 6e74 6573 745f 6c69 7374 2e73  g.contest_list.s
+000048d0: 6574 486f 7269 7a6f 6e74 616c 4865 6164  etHorizontalHead
+000048e0: 6572 4974 656d 280a 2020 2020 2020 2020  erItem(.        
+000048f0: 2020 2020 2020 2020 332c 2051 7457 6964          3, QtWid
+00004900: 6765 7473 2e51 5461 626c 6557 6964 6765  gets.QTableWidge
+00004910: 7449 7465 6d28 224e 6f74 2055 4973 6564  tItem("Not UIsed
+00004920: 2229 0a20 2020 2020 2020 2020 2020 2029  ").            )
+00004930: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00004940: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+00004950: 2e63 6f6e 7465 7374 5f6c 6973 742e 7365  .contest_list.se
+00004960: 7443 6f6c 756d 6e48 6964 6465 6e28 302c  tColumnHidden(0,
+00004970: 2054 7275 6529 0a20 2020 2020 2020 2020   True).         
+00004980: 2020 2073 656c 662e 636f 6e74 6573 745f     self.contest_
+00004990: 6469 616c 6f67 2e63 6f6e 7465 7374 5f6c  dialog.contest_l
+000049a0: 6973 742e 7365 7443 6f6c 756d 6e48 6964  ist.setColumnHid
+000049b0: 6465 6e28 332c 2054 7275 6529 0a20 2020  den(3, True).   
+000049c0: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+000049d0: 6e74 6573 745f 6469 616c 6f67 2e61 6363  ntest_dialog.acc
+000049e0: 6570 7465 642e 636f 6e6e 6563 7428 7365  epted.connect(se
+000049f0: 6c66 2e6f 7065 6e5f 636f 6e74 6573 745f  lf.open_contest_
+00004a00: 7265 7475 726e 290a 2020 2020 2020 2020  return).        
+00004a10: 2020 2020 666f 7220 636f 6e74 6573 7420      for contest 
+00004a20: 696e 2063 6f6e 7465 7374 733a 0a20 2020  in contests:.   
+00004a30: 2020 2020 2020 2020 2020 2020 206e 756d               num
+00004a40: 6265 725f 6f66 5f72 6f77 7320 3d20 7365  ber_of_rows = se
+00004a50: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
+00004a60: 672e 636f 6e74 6573 745f 6c69 7374 2e72  g.contest_list.r
+00004a70: 6f77 436f 756e 7428 290a 2020 2020 2020  owCount().      
+00004a80: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00004a90: 6f6e 7465 7374 5f64 6961 6c6f 672e 636f  ontest_dialog.co
+00004aa0: 6e74 6573 745f 6c69 7374 2e69 6e73 6572  ntest_list.inser
+00004ab0: 7452 6f77 286e 756d 6265 725f 6f66 5f72  tRow(number_of_r
+00004ac0: 6f77 7329 0a20 2020 2020 2020 2020 2020  ows).           
+00004ad0: 2020 2020 2063 6f6e 7465 7374 5f69 6420       contest_id 
+00004ae0: 3d20 7374 7228 636f 6e74 6573 742e 6765  = str(contest.ge
+00004af0: 7428 2243 6f6e 7465 7374 4944 222c 2031  t("ContestID", 1
+00004b00: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+00004b10: 2020 2063 6f6e 7465 7374 5f6e 616d 6520     contest_name 
+00004b20: 3d20 636f 6e74 6573 742e 6765 7428 2243  = contest.get("C
+00004b30: 6f6e 7465 7374 4e61 6d65 222c 2031 290a  ontestName", 1).
+00004b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b50: 7374 6172 745f 6461 7465 203d 2063 6f6e  start_date = con
+00004b60: 7465 7374 2e67 6574 2822 5374 6172 7444  test.get("StartD
+00004b70: 6174 6522 2c20 3129 0a20 2020 2020 2020  ate", 1).       
+00004b80: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+00004b90: 6e74 6573 745f 6469 616c 6f67 2e63 6f6e  ntest_dialog.con
+00004ba0: 7465 7374 5f6c 6973 742e 7365 7449 7465  test_list.setIte
+00004bb0: 6d28 0a20 2020 2020 2020 2020 2020 2020  m(.             
+00004bc0: 2020 2020 2020 206e 756d 6265 725f 6f66         number_of
+00004bd0: 5f72 6f77 732c 2030 2c20 5174 5769 6467  _rows, 0, QtWidg
+00004be0: 6574 732e 5154 6162 6c65 5769 6467 6574  ets.QTableWidget
+00004bf0: 4974 656d 2863 6f6e 7465 7374 5f69 6429  Item(contest_id)
+00004c00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004c10: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00004c20: 2020 2073 656c 662e 636f 6e74 6573 745f     self.contest_
+00004c30: 6469 616c 6f67 2e63 6f6e 7465 7374 5f6c  dialog.contest_l
+00004c40: 6973 742e 7365 7449 7465 6d28 0a20 2020  ist.setItem(.   
+00004c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c60: 206e 756d 6265 725f 6f66 5f72 6f77 732c   number_of_rows,
+00004c70: 2031 2c20 5174 5769 6467 6574 732e 5154   1, QtWidgets.QT
+00004c80: 6162 6c65 5769 6467 6574 4974 656d 2863  ableWidgetItem(c
+00004c90: 6f6e 7465 7374 5f6e 616d 6529 0a20 2020  ontest_name).   
+00004ca0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00004cb0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00004cc0: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
+00004cd0: 6f67 2e63 6f6e 7465 7374 5f6c 6973 742e  og.contest_list.
+00004ce0: 7365 7449 7465 6d28 0a20 2020 2020 2020  setItem(.       
+00004cf0: 2020 2020 2020 2020 2020 2020 206e 756d               num
+00004d00: 6265 725f 6f66 5f72 6f77 732c 2032 2c20  ber_of_rows, 2, 
+00004d10: 5174 5769 6467 6574 732e 5154 6162 6c65  QtWidgets.QTable
+00004d20: 5769 6467 6574 4974 656d 2873 7461 7274  WidgetItem(start
+00004d30: 5f64 6174 6529 0a20 2020 2020 2020 2020  _date).         
+00004d40: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00004d50: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+00004d60: 616c 6f67 2e73 686f 7728 290a 0a20 2020  alog.show()..   
+00004d70: 2064 6566 206f 7065 6e5f 636f 6e74 6573   def open_contes
+00004d80: 745f 7265 7475 726e 2873 656c 6629 3a0a  t_return(self):.
+00004d90: 2020 2020 2020 2020 2222 2243 616c 6c65          """Calle
+00004da0: 6420 6279 206f 7065 6e5f 636f 6e74 6573  d by open_contes
+00004db0: 7422 2222 0a20 2020 2020 2020 2073 656c  t""".        sel
+00004dc0: 6563 7465 645f 726f 7720 3d20 7365 6c66  ected_row = self
+00004dd0: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
+00004de0: 636f 6e74 6573 745f 6c69 7374 2e63 7572  contest_list.cur
+00004df0: 7265 6e74 526f 7728 290a 2020 2020 2020  rentRow().      
+00004e00: 2020 636f 6e74 6573 7420 3d20 7365 6c66    contest = self
+00004e10: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
+00004e20: 636f 6e74 6573 745f 6c69 7374 2e69 7465  contest_list.ite
+00004e30: 6d28 7365 6c65 6374 6564 5f72 6f77 2c20  m(selected_row, 
+00004e40: 3029 2e74 6578 7428 290a 2020 2020 2020  0).text().      
+00004e50: 2020 7365 6c66 2e70 7265 665b 2263 6f6e    self.pref["con
+00004e60: 7465 7374 225d 203d 2063 6f6e 7465 7374  test"] = contest
+00004e70: 0a20 2020 2020 2020 2073 656c 662e 7772  .        self.wr
+00004e80: 6974 655f 7072 6566 6572 656e 6365 2829  ite_preference()
+00004e90: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+00004ea0: 6465 6275 6728 2253 656c 6563 7465 6420  debug("Selected 
+00004eb0: 636f 6e74 6573 743a 2025 7322 2c20 6622  contest: %s", f"
+00004ec0: 7b63 6f6e 7465 7374 7d22 290a 2020 2020  {contest}").    
+00004ed0: 2020 2020 7365 6c66 2e6c 6f61 645f 636f      self.load_co
+00004ee0: 6e74 6573 7428 290a 2020 2020 2020 2020  ntest().        
+00004ef0: 7365 6c66 2e77 6f72 6b65 645f 6c69 7374  self.worked_list
+00004f00: 203d 2073 656c 662e 6461 7461 6261 7365   = self.database
+00004f10: 2e67 6574 5f63 616c 6c73 5f61 6e64 5f62  .get_calls_and_b
+00004f20: 616e 6473 2829 0a20 2020 2020 2020 2073  ands().        s
+00004f30: 656c 662e 7365 6e64 5f77 6f72 6b65 645f  elf.send_worked_
+00004f40: 6c69 7374 2829 0a0a 2020 2020 6465 6620  list()..    def 
+00004f50: 7265 6669 6c6c 5f64 726f 7064 6f77 6e28  refill_dropdown(
+00004f60: 7365 6c66 2c20 7461 7267 6574 2c20 736f  self, target, so
+00004f70: 7572 6365 293a 0a20 2020 2020 2020 2022  urce):.        "
+00004f80: 2222 5265 6669 6c6c 2051 436f 6d62 6f62  ""Refill QCombob
+00004f90: 6f78 2077 6964 6765 7420 7769 7468 2076  ox widget with v
+00004fa0: 616c 7565 2e22 2222 0a20 2020 2020 2020  alue.""".       
+00004fb0: 2069 6e64 6578 203d 2074 6172 6765 742e   index = target.
+00004fc0: 6669 6e64 5465 7874 2873 6f75 7263 6529  findText(source)
+00004fd0: 0a20 2020 2020 2020 2074 6172 6765 742e  .        target.
+00004fe0: 7365 7443 7572 7265 6e74 496e 6465 7828  setCurrentIndex(
+00004ff0: 696e 6465 7829 0a0a 2020 2020 6465 6620  index)..    def 
+00005000: 6564 6974 5f63 6f6e 7465 7374 2873 656c  edit_contest(sel
+00005010: 6629 3a0a 2020 2020 2020 2020 2222 2245  f):.        """E
+00005020: 6469 7420 7468 6520 6375 7272 656e 7420  dit the current 
+00005030: 636f 6e74 6573 7422 2222 0a20 2020 2020  contest""".     
+00005040: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+00005050: 2245 6469 7420 636f 6e74 6573 7420 4469  "Edit contest Di
+00005060: 616c 6f67 2229 0a20 2020 2020 2020 2069  alog").        i
+00005070: 6620 7365 6c66 2e63 6f6e 7465 7374 2069  f self.contest i
+00005080: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00005090: 2020 2020 7365 6c66 2e73 686f 775f 6d65      self.show_me
+000050a0: 7373 6167 655f 626f 7828 2259 6f75 2068  ssage_box("You h
+000050b0: 6176 6520 6e6f 2063 6f6e 7465 7374 2064  ave no contest d
+000050c0: 6566 696e 6564 2e22 290a 2020 2020 2020  efined.").      
+000050d0: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+000050e0: 2020 2020 2069 6620 7365 6c66 2e63 6f6e       if self.con
+000050f0: 7465 7374 5f73 6574 7469 6e67 7320 6973  test_settings is
+00005100: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00005110: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+00005120: 2020 7365 6c66 2e63 6f6e 7465 7374 5f64    self.contest_d
+00005130: 6961 6c6f 6720 3d20 4e65 7743 6f6e 7465  ialog = NewConte
+00005140: 7374 2857 4f52 4b49 4e47 5f50 4154 4829  st(WORKING_PATH)
+00005150: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
+00005160: 6e74 6573 745f 6469 616c 6f67 2e73 6574  ntest_dialog.set
+00005170: 5769 6e64 6f77 5469 746c 6528 2245 6469  WindowTitle("Edi
+00005180: 7420 436f 6e74 6573 7422 290a 2020 2020  t Contest").    
+00005190: 2020 2020 7365 6c66 2e63 6f6e 7465 7374      self.contest
+000051a0: 5f64 6961 6c6f 672e 7469 746c 652e 7365  _dialog.title.se
+000051b0: 7454 6578 7428 2222 290a 2020 2020 2020  tText("").      
+000051c0: 2020 7365 6c66 2e63 6f6e 7465 7374 5f64    self.contest_d
+000051d0: 6961 6c6f 672e 6163 6365 7074 6564 2e63  ialog.accepted.c
+000051e0: 6f6e 6e65 6374 2873 656c 662e 7361 7665  onnect(self.save
+000051f0: 5f65 6469 7465 645f 636f 6e74 6573 7429  _edited_contest)
+00005200: 0a20 2020 2020 2020 2076 616c 7565 203d  .        value =
+00005210: 2073 656c 662e 636f 6e74 6573 745f 7365   self.contest_se
+00005220: 7474 696e 6773 2e67 6574 2822 436f 6e74  ttings.get("Cont
+00005230: 6573 744e 616d 6522 292e 7570 7065 7228  estName").upper(
+00005240: 292e 7265 706c 6163 6528 225f 222c 2022  ).replace("_", "
+00005250: 2022 290a 2020 2020 2020 2020 6966 2076   ").        if v
+00005260: 616c 7565 203d 3d20 2247 454e 4552 414c  alue == "GENERAL
+00005270: 204c 4f47 4749 4e47 223a 0a20 2020 2020   LOGGING":.     
+00005280: 2020 2020 2020 2076 616c 7565 203d 2022         value = "
+00005290: 4765 6e65 7261 6c20 4c6f 6767 696e 6722  General Logging"
+000052a0: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+000052b0: 6669 6c6c 5f64 726f 7064 6f77 6e28 7365  fill_dropdown(se
+000052c0: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
+000052d0: 672e 636f 6e74 6573 742c 2076 616c 7565  g.contest, value
+000052e0: 290a 2020 2020 2020 2020 7661 6c75 6520  ).        value 
+000052f0: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f73  = self.contest_s
+00005300: 6574 7469 6e67 732e 6765 7428 224f 7065  ettings.get("Ope
+00005310: 7261 746f 7243 6174 6567 6f72 7922 290a  ratorCategory").
+00005320: 2020 2020 2020 2020 7365 6c66 2e72 6566          self.ref
+00005330: 696c 6c5f 6472 6f70 646f 776e 2873 656c  ill_dropdown(sel
+00005340: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+00005350: 2e6f 7065 7261 746f 725f 636c 6173 732c  .operator_class,
+00005360: 2076 616c 7565 290a 2020 2020 2020 2020   value).        
+00005370: 7661 6c75 6520 3d20 7365 6c66 2e63 6f6e  value = self.con
+00005380: 7465 7374 5f73 6574 7469 6e67 732e 6765  test_settings.ge
+00005390: 7428 2242 616e 6443 6174 6567 6f72 7922  t("BandCategory"
+000053a0: 290a 2020 2020 2020 2020 7365 6c66 2e72  ).        self.r
+000053b0: 6566 696c 6c5f 6472 6f70 646f 776e 2873  efill_dropdown(s
+000053c0: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
+000053d0: 6f67 2e62 616e 642c 2076 616c 7565 290a  og.band, value).
+000053e0: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
+000053f0: 7365 6c66 2e63 6f6e 7465 7374 5f73 6574  self.contest_set
+00005400: 7469 6e67 732e 6765 7428 2250 6f77 6572  tings.get("Power
+00005410: 4361 7465 676f 7279 2229 0a20 2020 2020  Category").     
+00005420: 2020 2073 656c 662e 7265 6669 6c6c 5f64     self.refill_d
+00005430: 726f 7064 6f77 6e28 7365 6c66 2e63 6f6e  ropdown(self.con
+00005440: 7465 7374 5f64 6961 6c6f 672e 706f 7765  test_dialog.powe
+00005450: 722c 2076 616c 7565 290a 2020 2020 2020  r, value).      
+00005460: 2020 7661 6c75 6520 3d20 7365 6c66 2e63    value = self.c
+00005470: 6f6e 7465 7374 5f73 6574 7469 6e67 732e  ontest_settings.
+00005480: 6765 7428 224d 6f64 6543 6174 6567 6f72  get("ModeCategor
+00005490: 7922 290a 2020 2020 2020 2020 7365 6c66  y").        self
+000054a0: 2e72 6566 696c 6c5f 6472 6f70 646f 776e  .refill_dropdown
+000054b0: 2873 656c 662e 636f 6e74 6573 745f 6469  (self.contest_di
+000054c0: 616c 6f67 2e6d 6f64 652c 2076 616c 7565  alog.mode, value
+000054d0: 290a 2020 2020 2020 2020 7661 6c75 6520  ).        value 
+000054e0: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f73  = self.contest_s
+000054f0: 6574 7469 6e67 732e 6765 7428 224f 7665  ettings.get("Ove
+00005500: 726c 6179 4361 7465 676f 7279 2229 0a20  rlayCategory"). 
+00005510: 2020 2020 2020 2073 656c 662e 7265 6669         self.refi
+00005520: 6c6c 5f64 726f 7064 6f77 6e28 7365 6c66  ll_dropdown(self
+00005530: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
+00005540: 6f76 6572 6c61 792c 2076 616c 7565 290a  overlay, value).
+00005550: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+00005560: 7465 7374 5f64 6961 6c6f 672e 6f70 6572  test_dialog.oper
+00005570: 6174 6f72 732e 7365 7454 6578 7428 7365  ators.setText(se
+00005580: 6c66 2e63 6f6e 7465 7374 5f73 6574 7469  lf.contest_setti
+00005590: 6e67 732e 6765 7428 224f 7065 7261 746f  ngs.get("Operato
+000055a0: 7273 2229 290a 2020 2020 2020 2020 7365  rs")).        se
+000055b0: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
+000055c0: 672e 736f 6170 626f 782e 7365 7450 6c61  g.soapbox.setPla
+000055d0: 696e 5465 7874 2873 656c 662e 636f 6e74  inText(self.cont
+000055e0: 6573 745f 7365 7474 696e 6773 2e67 6574  est_settings.get
+000055f0: 2822 536f 6170 626f 7822 2929 0a20 2020  ("Soapbox")).   
+00005600: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
+00005610: 745f 6469 616c 6f67 2e65 7863 6861 6e67  t_dialog.exchang
+00005620: 652e 7365 7454 6578 7428 7365 6c66 2e63  e.setText(self.c
+00005630: 6f6e 7465 7374 5f73 6574 7469 6e67 732e  ontest_settings.
+00005640: 6765 7428 2253 656e 7445 7863 6861 6e67  get("SentExchang
+00005650: 6522 2929 0a20 2020 2020 2020 2076 616c  e")).        val
+00005660: 7565 203d 2073 656c 662e 636f 6e74 6573  ue = self.contes
+00005670: 745f 7365 7474 696e 6773 2e67 6574 2822  t_settings.get("
+00005680: 5374 6174 696f 6e43 6174 6567 6f72 7922  StationCategory"
+00005690: 290a 2020 2020 2020 2020 7365 6c66 2e72  ).        self.r
+000056a0: 6566 696c 6c5f 6472 6f70 646f 776e 2873  efill_dropdown(s
+000056b0: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
+000056c0: 6f67 2e73 7461 7469 6f6e 2c20 7661 6c75  og.station, valu
+000056d0: 6529 0a20 2020 2020 2020 2076 616c 7565  e).        value
+000056e0: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
+000056f0: 7365 7474 696e 6773 2e67 6574 2822 4173  settings.get("As
+00005700: 7369 7374 6564 4361 7465 676f 7279 2229  sistedCategory")
+00005710: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
+00005720: 6669 6c6c 5f64 726f 7064 6f77 6e28 7365  fill_dropdown(se
+00005730: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
+00005740: 672e 6173 7369 7374 6564 2c20 7661 6c75  g.assisted, valu
+00005750: 6529 0a20 2020 2020 2020 2076 616c 7565  e).        value
+00005760: 203d 2073 656c 662e 636f 6e74 6573 745f   = self.contest_
+00005770: 7365 7474 696e 6773 2e67 6574 2822 5472  settings.get("Tr
+00005780: 616e 736d 6974 7465 7243 6174 6567 6f72  ansmitterCategor
+00005790: 7922 290a 2020 2020 2020 2020 7365 6c66  y").        self
+000057a0: 2e72 6566 696c 6c5f 6472 6f70 646f 776e  .refill_dropdown
+000057b0: 2873 656c 662e 636f 6e74 6573 745f 6469  (self.contest_di
+000057c0: 616c 6f67 2e74 7261 6e73 6d69 7474 6572  alog.transmitter
+000057d0: 2c20 7661 6c75 6529 0a20 2020 2020 2020  , value).       
+000057e0: 2076 616c 7565 203d 2073 656c 662e 636f   value = self.co
+000057f0: 6e74 6573 745f 7365 7474 696e 6773 2e67  ntest_settings.g
+00005800: 6574 2822 5374 6172 7444 6174 6522 290a  et("StartDate").
+00005810: 2020 2020 2020 2020 7468 655f 6461 7465          the_date
+00005820: 2c20 7468 655f 7469 6d65 203d 2076 616c  , the_time = val
+00005830: 7565 2e73 706c 6974 2829 0a20 2020 2020  ue.split().     
+00005840: 2020 2073 656c 662e 636f 6e74 6573 745f     self.contest_
+00005850: 6469 616c 6f67 2e64 6174 6554 696d 6545  dialog.dateTimeE
+00005860: 6469 742e 7365 7444 6174 6528 0a20 2020  dit.setDate(.   
+00005870: 2020 2020 2020 2020 2051 7443 6f72 652e           QtCore.
+00005880: 5144 6174 652e 6672 6f6d 5374 7269 6e67  QDate.fromString
+00005890: 2874 6865 5f64 6174 652c 2022 7979 7979  (the_date, "yyyy
+000058a0: 2d4d 4d2d 6464 2229 0a20 2020 2020 2020  -MM-dd").       
+000058b0: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
+000058c0: 636f 6e74 6573 745f 6469 616c 6f67 2e64  contest_dialog.d
+000058d0: 6174 6554 696d 6545 6469 742e 7365 7443  ateTimeEdit.setC
+000058e0: 616c 656e 6461 7250 6f70 7570 2854 7275  alendarPopup(Tru
+000058f0: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
+00005900: 636f 6e74 6573 745f 6469 616c 6f67 2e64  contest_dialog.d
+00005910: 6174 6554 696d 6545 6469 742e 7365 7454  ateTimeEdit.setT
+00005920: 696d 6528 0a20 2020 2020 2020 2020 2020  ime(.           
+00005930: 2051 7443 6f72 652e 5154 696d 652e 6672   QtCore.QTime.fr
+00005940: 6f6d 5374 7269 6e67 2874 6865 5f74 696d  omString(the_tim
+00005950: 652c 2022 6868 3a6d 6d3a 7373 2229 0a20  e, "hh:mm:ss"). 
+00005960: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00005970: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+00005980: 616c 6f67 2e6f 7065 6e28 290a 0a20 2020  alog.open()..   
+00005990: 2064 6566 2073 6176 655f 6564 6974 6564   def save_edited
+000059a0: 5f63 6f6e 7465 7374 2873 656c 6629 3a0a  _contest(self):.
+000059b0: 2020 2020 2020 2020 2222 2253 6176 6520          """Save 
+000059c0: 7468 6520 6564 6974 6564 2063 6f6e 7465  the edited conte
+000059d0: 7374 2222 220a 2020 2020 2020 2020 636f  st""".        co
+000059e0: 6e74 6573 7420 3d20 7b7d 0a20 2020 2020  ntest = {}.     
+000059f0: 2020 2063 6f6e 7465 7374 5b22 436f 6e74     contest["Cont
+00005a00: 6573 744e 616d 6522 5d20 3d20 280a 2020  estName"] = (.  
+00005a10: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00005a20: 6f6e 7465 7374 5f64 6961 6c6f 672e 636f  ontest_dialog.co
+00005a30: 6e74 6573 742e 6375 7272 656e 7454 6578  ntest.currentTex
+00005a40: 7428 292e 6c6f 7765 7228 292e 7265 706c  t().lower().repl
+00005a50: 6163 6528 2220 222c 2022 5f22 290a 2020  ace(" ", "_").  
+00005a60: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00005a70: 636f 6e74 6573 745b 2253 7461 7274 4461  contest["StartDa
+00005a80: 7465 225d 203d 2073 656c 662e 636f 6e74  te"] = self.cont
+00005a90: 6573 745f 6469 616c 6f67 2e64 6174 6554  est_dialog.dateT
+00005aa0: 696d 6545 6469 742e 6461 7465 5469 6d65  imeEdit.dateTime
+00005ab0: 2829 2e74 6f53 7472 696e 6728 0a20 2020  ().toString(.   
+00005ac0: 2020 2020 2020 2020 2022 7979 7979 2d4d           "yyyy-M
+00005ad0: 4d2d 6464 2068 683a 6d6d 3a73 7322 0a20  M-dd hh:mm:ss". 
+00005ae0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00005af0: 2063 6f6e 7465 7374 5b22 4f70 6572 6174   contest["Operat
+00005b00: 6f72 4361 7465 676f 7279 225d 203d 2073  orCategory"] = s
+00005b10: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
+00005b20: 6f67 2e6f 7065 7261 746f 725f 636c 6173  og.operator_clas
+00005b30: 732e 6375 7272 656e 7454 6578 7428 290a  s.currentText().
+00005b40: 2020 2020 2020 2020 636f 6e74 6573 745b          contest[
+00005b50: 2242 616e 6443 6174 6567 6f72 7922 5d20  "BandCategory"] 
+00005b60: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f64  = self.contest_d
+00005b70: 6961 6c6f 672e 6261 6e64 2e63 7572 7265  ialog.band.curre
+00005b80: 6e74 5465 7874 2829 0a20 2020 2020 2020  ntText().       
+00005b90: 2063 6f6e 7465 7374 5b22 506f 7765 7243   contest["PowerC
+00005ba0: 6174 6567 6f72 7922 5d20 3d20 7365 6c66  ategory"] = self
+00005bb0: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
+00005bc0: 706f 7765 722e 6375 7272 656e 7454 6578  power.currentTex
+00005bd0: 7428 290a 2020 2020 2020 2020 636f 6e74  t().        cont
+00005be0: 6573 745b 224d 6f64 6543 6174 6567 6f72  est["ModeCategor
+00005bf0: 7922 5d20 3d20 7365 6c66 2e63 6f6e 7465  y"] = self.conte
+00005c00: 7374 5f64 6961 6c6f 672e 6d6f 6465 2e63  st_dialog.mode.c
+00005c10: 7572 7265 6e74 5465 7874 2829 0a20 2020  urrentText().   
+00005c20: 2020 2020 2063 6f6e 7465 7374 5b22 4f76       contest["Ov
+00005c30: 6572 6c61 7943 6174 6567 6f72 7922 5d20  erlayCategory"] 
+00005c40: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f64  = self.contest_d
+00005c50: 6961 6c6f 672e 6f76 6572 6c61 792e 6375  ialog.overlay.cu
+00005c60: 7272 656e 7454 6578 7428 290a 2020 2020  rrentText().    
+00005c70: 2020 2020 636f 6e74 6573 745b 224f 7065      contest["Ope
+00005c80: 7261 746f 7273 225d 203d 2073 656c 662e  rators"] = self.
+00005c90: 636f 6e74 6573 745f 6469 616c 6f67 2e6f  contest_dialog.o
+00005ca0: 7065 7261 746f 7273 2e74 6578 7428 290a  perators.text().
+00005cb0: 2020 2020 2020 2020 636f 6e74 6573 745b          contest[
+00005cc0: 2253 6f61 7062 6f78 225d 203d 2073 656c  "Soapbox"] = sel
+00005cd0: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+00005ce0: 2e73 6f61 7062 6f78 2e74 6f50 6c61 696e  .soapbox.toPlain
+00005cf0: 5465 7874 2829 0a20 2020 2020 2020 2063  Text().        c
+00005d00: 6f6e 7465 7374 5b22 5365 6e74 4578 6368  ontest["SentExch
+00005d10: 616e 6765 225d 203d 2073 656c 662e 636f  ange"] = self.co
+00005d20: 6e74 6573 745f 6469 616c 6f67 2e65 7863  ntest_dialog.exc
+00005d30: 6861 6e67 652e 7465 7874 2829 0a20 2020  hange.text().   
+00005d40: 2020 2020 2063 6f6e 7465 7374 5b22 436f       contest["Co
+00005d50: 6e74 6573 744e 5222 5d20 3d20 7365 6c66  ntestNR"] = self
+00005d60: 2e70 7265 662e 6765 7428 2263 6f6e 7465  .pref.get("conte
+00005d70: 7374 222c 2031 290a 2020 2020 2020 2020  st", 1).        
+00005d80: 636f 6e74 6573 745b 2253 7461 7469 6f6e  contest["Station
+00005d90: 4361 7465 676f 7279 225d 203d 2073 656c  Category"] = sel
+00005da0: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+00005db0: 2e73 7461 7469 6f6e 2e63 7572 7265 6e74  .station.current
+00005dc0: 5465 7874 2829 0a20 2020 2020 2020 2063  Text().        c
+00005dd0: 6f6e 7465 7374 5b22 4173 7369 7374 6564  ontest["Assisted
+00005de0: 4361 7465 676f 7279 225d 203d 2073 656c  Category"] = sel
+00005df0: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+00005e00: 2e61 7373 6973 7465 642e 6375 7272 656e  .assisted.curren
+00005e10: 7454 6578 7428 290a 2020 2020 2020 2020  tText().        
+00005e20: 636f 6e74 6573 745b 2254 7261 6e73 6d69  contest["Transmi
+00005e30: 7474 6572 4361 7465 676f 7279 225d 203d  tterCategory"] =
+00005e40: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+00005e50: 616c 6f67 2e74 7261 6e73 6d69 7474 6572  alog.transmitter
+00005e60: 2e63 7572 7265 6e74 5465 7874 2829 0a0a  .currentText()..
+00005e70: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+00005e80: 6562 7567 2822 2573 222c 2066 227b 636f  ebug("%s", f"{co
+00005e90: 6e74 6573 747d 2229 0a20 2020 2020 2020  ntest}").       
+00005ea0: 2073 656c 662e 6461 7461 6261 7365 2e75   self.database.u
+00005eb0: 7064 6174 655f 636f 6e74 6573 7428 636f  pdate_contest(co
+00005ec0: 6e74 6573 7429 0a20 2020 2020 2020 2073  ntest).        s
+00005ed0: 656c 662e 7772 6974 655f 7072 6566 6572  elf.write_prefer
+00005ee0: 656e 6365 2829 0a20 2020 2020 2020 2073  ence().        s
+00005ef0: 656c 662e 6c6f 6164 5f63 6f6e 7465 7374  elf.load_contest
+00005f00: 2829 0a0a 2020 2020 6465 6620 6c6f 6164  ()..    def load
+00005f10: 5f63 6f6e 7465 7374 2873 656c 6629 3a0a  _contest(self):.
+00005f20: 2020 2020 2020 2020 2222 226c 6f61 6420          """load 
+00005f30: 6120 636f 6e74 6573 7422 2222 0a20 2020  a contest""".   
+00005f40: 2020 2020 2069 6620 7365 6c66 2e70 7265       if self.pre
+00005f50: 662e 6765 7428 2263 6f6e 7465 7374 2229  f.get("contest")
+00005f60: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00005f70: 6c66 2e63 6f6e 7465 7374 5f73 6574 7469  lf.contest_setti
+00005f80: 6e67 7320 3d20 7365 6c66 2e64 6174 6162  ngs = self.datab
+00005f90: 6173 652e 6665 7463 685f 636f 6e74 6573  ase.fetch_contes
+00005fa0: 745f 6279 5f69 6428 0a20 2020 2020 2020  t_by_id(.       
+00005fb0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+00005fc0: 6566 2e67 6574 2822 636f 6e74 6573 7422  ef.get("contest"
+00005fd0: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
+00005fe0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00005ff0: 656c 662e 636f 6e74 6573 745f 7365 7474  elf.contest_sett
+00006000: 696e 6773 3a0a 2020 2020 2020 2020 2020  ings:.          
+00006010: 2020 2020 2020 7365 6c66 2e64 6174 6162        self.datab
+00006020: 6173 652e 6375 7272 656e 745f 636f 6e74  ase.current_cont
+00006030: 6573 7420 3d20 7365 6c66 2e70 7265 662e  est = self.pref.
+00006040: 6765 7428 2263 6f6e 7465 7374 2229 0a20  get("contest"). 
+00006050: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00006060: 6620 7365 6c66 2e63 6f6e 7465 7374 5f73  f self.contest_s
+00006070: 6574 7469 6e67 732e 6765 7428 2243 6f6e  ettings.get("Con
+00006080: 7465 7374 4e61 6d65 2229 3a0a 2020 2020  testName"):.    
+00006090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060a0: 7365 6c66 2e63 6f6e 7465 7374 203d 2064  self.contest = d
+000060b0: 6f69 6d70 2873 656c 662e 636f 6e74 6573  oimp(self.contes
+000060c0: 745f 7365 7474 696e 6773 2e67 6574 2822  t_settings.get("
+000060d0: 436f 6e74 6573 744e 616d 6522 2929 0a20  ContestName")). 
+000060e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060f0: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+00006100: 224c 6f61 6465 6420 436f 6e74 6573 7420  "Loaded Contest 
+00006110: 4e61 6d65 203d 2025 7322 2c20 7365 6c66  Name = %s", self
+00006120: 2e63 6f6e 7465 7374 2e6e 616d 6529 0a20  .contest.name). 
+00006130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006140: 2020 2073 656c 662e 7365 745f 7769 6e64     self.set_wind
+00006150: 6f77 5f74 6974 6c65 2829 0a20 2020 2020  ow_title().     
+00006160: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00006170: 656c 662e 636f 6e74 6573 742e 696e 6974  elf.contest.init
+00006180: 5f63 6f6e 7465 7374 2873 656c 6629 0a20  _contest(self). 
+00006190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000061a0: 2020 2073 656c 662e 6869 6465 5f62 616e     self.hide_ban
+000061b0: 645f 6d6f 6465 2873 656c 662e 636f 6e74  d_mode(self.cont
+000061c0: 6573 745f 7365 7474 696e 6773 2e67 6574  est_settings.get
+000061d0: 2822 4d6f 6465 4361 7465 676f 7279 222c  ("ModeCategory",
+000061e0: 2022 2229 290a 2020 2020 2020 2020 2020   "")).          
+000061f0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+00006200: 2e64 6562 7567 2822 2573 222c 2066 227b  .debug("%s", f"{
+00006210: 7365 6c66 2e63 6f6e 7465 7374 5f73 6574  self.contest_set
+00006220: 7469 6e67 737d 2229 0a20 2020 2020 2020  tings}").       
+00006230: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00006240: 7365 6c66 2e63 6f6e 7465 7374 5f73 6574  self.contest_set
+00006250: 7469 6e67 732e 6765 7428 224d 6f64 6543  tings.get("ModeC
+00006260: 6174 6567 6f72 7922 2c20 2222 2920 3d3d  ategory", "") ==
+00006270: 2022 4357 223a 0a20 2020 2020 2020 2020   "CW":.         
+00006280: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00006290: 656c 662e 7365 746d 6f64 6528 2243 5722  elf.setmode("CW"
+000062a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000062b0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+000062c0: 6164 696f 5f73 7461 7465 5b22 6d6f 6465  adio_state["mode
+000062d0: 225d 203d 2022 4357 220a 2020 2020 2020  "] = "CW".      
+000062e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062f0: 2020 6966 2073 656c 662e 7269 675f 636f    if self.rig_co
+00006300: 6e74 726f 6c3a 0a20 2020 2020 2020 2020  ntrol:.         
 00006310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006320: 2020 2020 2073 656c 662e 7269 675f 636f       self.rig_co
-00006330: 6e74 726f 6c2e 7365 745f 6d6f 6465 2822  ntrol.set_mode("
-00006340: 4357 2229 0a20 2020 2020 2020 2020 2020  CW").           
-00006350: 2020 2020 2020 2020 2020 2020 2062 616e               ban
-00006360: 6420 3d20 6765 7462 616e 6428 7374 7228  d = getband(str(
-00006370: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
-00006380: 2e67 6574 2822 7666 6f61 222c 2022 302e  .get("vfoa", "0.
-00006390: 3022 2929 290a 2020 2020 2020 2020 2020  0"))).          
-000063a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000063b0: 6c66 2e73 6574 5f62 616e 645f 696e 6469  lf.set_band_indi
-000063c0: 6361 746f 7228 6261 6e64 290a 2020 2020  cator(band).    
+00006320: 2020 2069 6620 7365 6c66 2e72 6967 5f63     if self.rig_c
+00006330: 6f6e 7472 6f6c 2e6f 6e6c 696e 653a 0a20  ontrol.online:. 
+00006340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006350: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00006360: 656c 662e 7269 675f 636f 6e74 726f 6c2e  elf.rig_control.
+00006370: 7365 745f 6d6f 6465 2822 4357 2229 0a20  set_mode("CW"). 
+00006380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006390: 2020 2020 2020 2062 616e 6420 3d20 6765         band = ge
+000063a0: 7462 616e 6428 7374 7228 7365 6c66 2e72  tband(str(self.r
+000063b0: 6164 696f 5f73 7461 7465 2e67 6574 2822  adio_state.get("
+000063c0: 7666 6f61 222c 2022 302e 3022 2929 290a  vfoa", "0.0"))).
 000063d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063e0: 2020 2020 7365 6c66 2e73 6574 5f77 696e      self.set_win
-000063f0: 646f 775f 7469 746c 6528 290a 2020 2020  dow_title().    
-00006400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006410: 6966 2073 656c 662e 636f 6e74 6573 745f  if self.contest_
-00006420: 7365 7474 696e 6773 2e67 6574 2822 4d6f  settings.get("Mo
-00006430: 6465 4361 7465 676f 7279 222c 2022 2229  deCategory", "")
-00006440: 203d 3d20 2253 5342 223a 0a20 2020 2020   == "SSB":.     
-00006450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006460: 2020 2073 656c 662e 7365 746d 6f64 6528     self.setmode(
-00006470: 2253 5342 2229 0a20 2020 2020 2020 2020  "SSB").         
-00006480: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00006490: 6620 696e 7428 7365 6c66 2e72 6164 696f  f int(self.radio
-000064a0: 5f73 7461 7465 2e67 6574 2822 7666 6f61  _state.get("vfoa
-000064b0: 222c 2030 2929 203e 2031 3030 3030 3030  ", 0)) > 1000000
-000064c0: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
-000064d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000064e0: 656c 662e 7261 6469 6f5f 7374 6174 655b  elf.radio_state[
-000064f0: 226d 6f64 6522 5d20 3d20 2255 5342 220a  "mode"] = "USB".
+000063e0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+000063f0: 5f62 616e 645f 696e 6469 6361 746f 7228  _band_indicator(
+00006400: 6261 6e64 290a 2020 2020 2020 2020 2020  band).          
+00006410: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00006420: 6c66 2e73 6574 5f77 696e 646f 775f 7469  lf.set_window_ti
+00006430: 746c 6528 290a 2020 2020 2020 2020 2020  tle().          
+00006440: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00006450: 662e 636f 6e74 6573 745f 7365 7474 696e  f.contest_settin
+00006460: 6773 2e67 6574 2822 4d6f 6465 4361 7465  gs.get("ModeCate
+00006470: 676f 7279 222c 2022 2229 203d 3d20 2253  gory", "") == "S
+00006480: 5342 223a 0a20 2020 2020 2020 2020 2020  SB":.           
+00006490: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000064a0: 662e 7365 746d 6f64 6528 2253 5342 2229  f.setmode("SSB")
+000064b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000064c0: 2020 2020 2020 2020 2069 6620 696e 7428           if int(
+000064d0: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
+000064e0: 2e67 6574 2822 7666 6f61 222c 2030 2929  .get("vfoa", 0))
+000064f0: 203e 2031 3030 3030 3030 303a 0a20 2020   > 10000000:.   
 00006500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006510: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00006520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006530: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-00006540: 6164 696f 5f73 7461 7465 5b22 6d6f 6465  adio_state["mode
-00006550: 225d 203d 2022 4c53 4222 0a20 2020 2020  "] = "LSB".     
+00006510: 2020 2020 2020 2020 2073 656c 662e 7261           self.ra
+00006520: 6469 6f5f 7374 6174 655b 226d 6f64 6522  dio_state["mode"
+00006530: 5d20 3d20 2255 5342 220a 2020 2020 2020  ] = "USB".      
+00006540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006550: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
 00006560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006570: 2020 2062 616e 6420 3d20 6765 7462 616e     band = getban
-00006580: 6428 7374 7228 7365 6c66 2e72 6164 696f  d(str(self.radio
-00006590: 5f73 7461 7465 2e67 6574 2822 7666 6f61  _state.get("vfoa
-000065a0: 222c 2022 302e 3022 2929 290a 2020 2020  ", "0.0"))).    
-000065b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065c0: 2020 2020 7365 6c66 2e73 6574 5f62 616e      self.set_ban
-000065d0: 645f 696e 6469 6361 746f 7228 6261 6e64  d_indicator(band
-000065e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000065f0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00006600: 6574 5f77 696e 646f 775f 7469 746c 6528  et_window_title(
-00006610: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00006620: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00006630: 662e 7269 675f 636f 6e74 726f 6c3a 0a20  f.rig_control:. 
-00006640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006650: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00006660: 7269 675f 636f 6e74 726f 6c2e 7365 745f  rig_control.set_
-00006670: 6d6f 6465 2873 656c 662e 7261 6469 6f5f  mode(self.radio_
-00006680: 7374 6174 652e 6765 7428 226d 6f64 6522  state.get("mode"
-00006690: 2929 0a0a 2020 2020 2020 2020 2020 2020  ))..            
-000066a0: 2020 2020 6966 2068 6173 6174 7472 2873      if hasattr(s
-000066b0: 656c 662e 636f 6e74 6573 742c 2022 6d6f  elf.contest, "mo
-000066c0: 6465 2229 3a0a 2020 2020 2020 2020 2020  de"):.          
-000066d0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-000066e0: 2e64 6562 7567 2822 2573 222c 2066 2220  .debug("%s", f" 
-000066f0: 202a 2a2a 2a20 207b 7365 6c66 2e63 6f6e   ****  {self.con
-00006700: 7465 7374 7d22 290a 2020 2020 2020 2020  test}").        
-00006710: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00006720: 656c 662e 636f 6e74 6573 742e 6d6f 6465  elf.contest.mode
-00006730: 2069 6e20 5b22 4357 222c 2022 424f 5448   in ["CW", "BOTH
-00006740: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
-00006750: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00006760: 2e63 775f 7370 6565 642e 7368 6f77 2829  .cw_speed.show()
-00006770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006780: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00006790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067a0: 2020 2073 656c 662e 6377 5f73 7065 6564     self.cw_speed
-000067b0: 2e68 6964 6528 290a 0a20 2020 2020 2020  .hide()..       
-000067c0: 2020 2020 2020 2020 2063 6d64 203d 207b           cmd = {
-000067d0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-000067e0: 2020 636d 645b 2263 6d64 225d 203d 2022    cmd["cmd"] = "
-000067f0: 4e45 5744 4222 0a20 2020 2020 2020 2020  NEWDB".         
-00006800: 2020 2020 2020 2063 6d64 5b22 7374 6174         cmd["stat
-00006810: 696f 6e22 5d20 3d20 706c 6174 666f 726d  ion"] = platform
-00006820: 2e6e 6f64 6528 290a 2020 2020 2020 2020  .node().        
-00006830: 2020 2020 2020 2020 7365 6c66 2e6d 756c          self.mul
-00006840: 7469 6361 7374 5f69 6e74 6572 6661 6365  ticast_interface
-00006850: 2e73 656e 645f 6173 5f6a 736f 6e28 636d  .send_as_json(cm
-00006860: 6429 0a20 2020 2020 2020 2020 2020 2020  d).             
-00006870: 2020 2069 6620 6861 7361 7474 7228 7365     if hasattr(se
-00006880: 6c66 2e63 6f6e 7465 7374 2c20 2263 6f6c  lf.contest, "col
-00006890: 756d 6e73 2229 3a0a 2020 2020 2020 2020  umns"):.        
-000068a0: 2020 2020 2020 2020 2020 2020 636d 6420              cmd 
-000068b0: 3d20 7b7d 0a20 2020 2020 2020 2020 2020  = {}.           
-000068c0: 2020 2020 2020 2020 2063 6d64 5b22 636d           cmd["cm
-000068d0: 6422 5d20 3d20 2253 484f 5743 4f4c 554d  d"] = "SHOWCOLUM
-000068e0: 4e53 220a 2020 2020 2020 2020 2020 2020  NS".            
-000068f0: 2020 2020 2020 2020 636d 645b 2273 7461          cmd["sta
-00006900: 7469 6f6e 225d 203d 2070 6c61 7466 6f72  tion"] = platfor
-00006910: 6d2e 6e6f 6465 2829 0a20 2020 2020 2020  m.node().       
-00006920: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
-00006930: 5b22 434f 4c55 4d4e 5322 5d20 3d20 7365  ["COLUMNS"] = se
-00006940: 6c66 2e63 6f6e 7465 7374 2e63 6f6c 756d  lf.contest.colum
-00006950: 6e73 0a20 2020 2020 2020 2020 2020 2020  ns.             
-00006960: 2020 2020 2020 2073 656c 662e 6d75 6c74         self.mult
-00006970: 6963 6173 745f 696e 7465 7266 6163 652e  icast_interface.
-00006980: 7365 6e64 5f61 735f 6a73 6f6e 2863 6d64  send_as_json(cmd
-00006990: 290a 0a20 2020 2064 6566 2063 6865 636b  )..    def check
-000069a0: 5f66 6f72 5f6e 6577 5f63 7479 2873 656c  _for_new_cty(sel
-000069b0: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
-000069c0: 2020 2020 2020 2020 4368 6563 6b73 2066          Checks f
-000069d0: 6f72 2061 206e 6577 2063 7479 2e64 6174  or a new cty.dat
-000069e0: 2066 696c 652e 0a20 2020 2020 2020 204c   file..        L
-000069f0: 6f61 6473 2069 7420 6966 2061 7661 696c  oads it if avail
-00006a00: 6162 6c65 2e0a 2020 2020 2020 2020 2222  able..        ""
-00006a10: 220a 2020 2020 2020 2020 7472 793a 0a20  ".        try:. 
-00006a20: 2020 2020 2020 2020 2020 2063 7479 203d             cty =
-00006a30: 206e 6f74 6374 7970 6172 7365 722e 4269   notctyparser.Bi
-00006a40: 6743 7479 2857 4f52 4b49 4e47 5f50 4154  gCty(WORKING_PAT
-00006a50: 4820 2b20 222f 6461 7461 2f63 7479 2e6a  H + "/data/cty.j
-00006a60: 736f 6e22 290a 2020 2020 2020 2020 2020  son").          
-00006a70: 2020 7570 6461 7465 5f61 7661 696c 6162    update_availab
-00006a80: 6c65 203d 2063 7479 2e63 6865 636b 5f75  le = cty.check_u
-00006a90: 7064 6174 6528 290a 2020 2020 2020 2020  pdate().        
-00006aa0: 6578 6365 7074 2041 7474 7269 6275 7465  except Attribute
-00006ab0: 4572 726f 7220 6173 2074 6865 5f65 7272  Error as the_err
-00006ac0: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
-00006ad0: 6c6f 6767 6572 2e64 6562 7567 2822 6374  logger.debug("ct
-00006ae0: 7920 7061 7273 6572 2072 6574 7572 6e65  y parser returne
-00006af0: 6420 616e 2065 7272 6f72 3a20 2573 222c  d an error: %s",
-00006b00: 2074 6865 5f65 7272 6f72 290a 2020 2020   the_error).    
-00006b10: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-00006b20: 2020 2020 2020 2065 7863 6570 7420 5661         except Va
-00006b30: 6c75 6545 7272 6f72 2061 7320 7468 655f  lueError as the_
-00006b40: 6572 726f 723a 0a20 2020 2020 2020 2020  error:.         
-00006b50: 2020 2070 7269 6e74 2822 6374 7920 7061     print("cty pa
-00006b60: 7273 6572 2072 6574 7572 6e65 6420 616e  rser returned an
-00006b70: 2065 7272 6f72 3a20 2573 222c 2074 6865   error: %s", the
-00006b80: 5f65 7272 6f72 290a 2020 2020 2020 2020  _error).        
-00006b90: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-00006ba0: 2822 6374 7920 7061 7273 6572 2072 6574  ("cty parser ret
-00006bb0: 7572 6e65 6420 616e 2065 7272 6f72 3a20  urned an error: 
-00006bc0: 2573 222c 2074 6865 5f65 7272 6f72 290a  %s", the_error).
-00006bd0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00006be0: 726e 0a20 2020 2020 2020 2065 7863 6570  rn.        excep
-00006bf0: 7420 6c6f 6361 6c65 2e45 7272 6f72 2061  t locale.Error a
-00006c00: 7320 7468 655f 6572 726f 723a 0a20 2020  s the_error:.   
-00006c10: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
-00006c20: 6374 7920 7061 7273 6572 2072 6574 7572  cty parser retur
-00006c30: 6e65 6420 616e 2065 7272 6f72 3a20 2573  ned an error: %s
-00006c40: 222c 2074 6865 5f65 7272 6f72 290a 2020  ", the_error).  
-00006c50: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-00006c60: 2e64 6562 7567 2822 6374 7920 7061 7273  .debug("cty pars
-00006c70: 6572 2072 6574 7572 6e65 6420 616e 2065  er returned an e
-00006c80: 7272 6f72 3a20 2573 222c 2074 6865 5f65  rror: %s", the_e
-00006c90: 7272 6f72 290a 2020 2020 2020 2020 2020  rror).          
-00006ca0: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-00006cb0: 206c 6f67 6765 722e 6465 6275 6728 224e   logger.debug("N
-00006cc0: 6577 6572 2063 7479 2066 696c 6520 6176  ewer cty file av
-00006cd0: 6169 6c61 626c 6520 2573 222c 2073 7472  ailable %s", str
-00006ce0: 2875 7064 6174 655f 6176 6169 6c61 626c  (update_availabl
-00006cf0: 6529 290a 0a20 2020 2020 2020 2069 6620  e))..        if 
-00006d00: 7570 6461 7465 5f61 7661 696c 6162 6c65  update_available
-00006d10: 3a0a 2020 2020 2020 2020 2020 2020 7472  :.            tr
-00006d20: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-00006d30: 2020 2075 7064 6174 6564 203d 2063 7479     updated = cty
-00006d40: 2e75 7064 6174 6528 290a 2020 2020 2020  .update().      
-00006d50: 2020 2020 2020 6578 6365 7074 2052 6573        except Res
-00006d60: 6f75 7263 6557 6172 6e69 6e67 2061 7320  ourceWarning as 
-00006d70: 7468 655f 6572 726f 723a 0a20 2020 2020  the_error:.     
-00006d80: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-00006d90: 722e 6465 6275 6728 2263 7479 2070 6172  r.debug("cty par
-00006da0: 7365 7220 7265 7475 726e 6564 2061 6e20  ser returned an 
-00006db0: 6572 726f 723a 2025 7322 2c20 7468 655f  error: %s", the_
-00006dc0: 6572 726f 7229 0a20 2020 2020 2020 2020  error).         
-00006dd0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-00006de0: 2020 2020 2020 2020 2020 6966 2075 7064            if upd
-00006df0: 6174 6564 3a0a 2020 2020 2020 2020 2020  ated:.          
-00006e00: 2020 2020 2020 6374 792e 6475 6d70 2857        cty.dump(W
-00006e10: 4f52 4b49 4e47 5f50 4154 4820 2b20 222f  ORKING_PATH + "/
-00006e20: 6461 7461 2f63 7479 2e6a 736f 6e22 290a  data/cty.json").
+00006570: 2020 2020 7365 6c66 2e72 6164 696f 5f73      self.radio_s
+00006580: 7461 7465 5b22 6d6f 6465 225d 203d 2022  tate["mode"] = "
+00006590: 4c53 4222 0a20 2020 2020 2020 2020 2020  LSB".           
+000065a0: 2020 2020 2020 2020 2020 2020 2062 616e               ban
+000065b0: 6420 3d20 6765 7462 616e 6428 7374 7228  d = getband(str(
+000065c0: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
+000065d0: 2e67 6574 2822 7666 6f61 222c 2022 302e  .get("vfoa", "0.
+000065e0: 3022 2929 290a 2020 2020 2020 2020 2020  0"))).          
+000065f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00006600: 6c66 2e73 6574 5f62 616e 645f 696e 6469  lf.set_band_indi
+00006610: 6361 746f 7228 6261 6e64 290a 2020 2020  cator(band).    
+00006620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006630: 2020 2020 7365 6c66 2e73 6574 5f77 696e      self.set_win
+00006640: 646f 775f 7469 746c 6528 290a 2020 2020  dow_title().    
+00006650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006660: 2020 2020 6966 2073 656c 662e 7269 675f      if self.rig_
+00006670: 636f 6e74 726f 6c3a 0a20 2020 2020 2020  control:.       
+00006680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006690: 2020 2020 2073 656c 662e 7269 675f 636f       self.rig_co
+000066a0: 6e74 726f 6c2e 7365 745f 6d6f 6465 2873  ntrol.set_mode(s
+000066b0: 656c 662e 7261 6469 6f5f 7374 6174 652e  elf.radio_state.
+000066c0: 6765 7428 226d 6f64 6522 2929 0a0a 2020  get("mode"))..  
+000066d0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000066e0: 2068 6173 6174 7472 2873 656c 662e 636f   hasattr(self.co
+000066f0: 6e74 6573 742c 2022 6d6f 6465 2229 3a0a  ntest, "mode"):.
+00006700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006710: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+00006720: 2822 2573 222c 2066 2220 202a 2a2a 2a20  ("%s", f"  **** 
+00006730: 207b 7365 6c66 2e63 6f6e 7465 7374 7d22   {self.contest}"
+00006740: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00006750: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
+00006760: 6e74 6573 742e 6d6f 6465 2069 6e20 5b22  ntest.mode in ["
+00006770: 4357 222c 2022 424f 5448 225d 3a0a 2020  CW", "BOTH"]:.  
+00006780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006790: 2020 2020 2020 7365 6c66 2e63 775f 7370        self.cw_sp
+000067a0: 6565 642e 7368 6f77 2829 0a20 2020 2020  eed.show().     
+000067b0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000067c0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+000067d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000067e0: 662e 6377 5f73 7065 6564 2e68 6964 6528  f.cw_speed.hide(
+000067f0: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+00006800: 2020 2063 6d64 203d 207b 7d0a 2020 2020     cmd = {}.    
+00006810: 2020 2020 2020 2020 2020 2020 636d 645b              cmd[
+00006820: 2263 6d64 225d 203d 2022 4e45 5744 4222  "cmd"] = "NEWDB"
+00006830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006840: 2063 6d64 5b22 7374 6174 696f 6e22 5d20   cmd["station"] 
+00006850: 3d20 706c 6174 666f 726d 2e6e 6f64 6528  = platform.node(
+00006860: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00006870: 2020 7365 6c66 2e6d 756c 7469 6361 7374    self.multicast
+00006880: 5f69 6e74 6572 6661 6365 2e73 656e 645f  _interface.send_
+00006890: 6173 5f6a 736f 6e28 636d 6429 0a20 2020  as_json(cmd).   
+000068a0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000068b0: 6861 7361 7474 7228 7365 6c66 2e63 6f6e  hasattr(self.con
+000068c0: 7465 7374 2c20 2263 6f6c 756d 6e73 2229  test, "columns")
+000068d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000068e0: 2020 2020 2020 636d 6420 3d20 7b7d 0a20        cmd = {}. 
+000068f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006900: 2020 2063 6d64 5b22 636d 6422 5d20 3d20     cmd["cmd"] = 
+00006910: 2253 484f 5743 4f4c 554d 4e53 220a 2020  "SHOWCOLUMNS".  
+00006920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006930: 2020 636d 645b 2273 7461 7469 6f6e 225d    cmd["station"]
+00006940: 203d 2070 6c61 7466 6f72 6d2e 6e6f 6465   = platform.node
+00006950: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00006960: 2020 2020 2020 2063 6d64 5b22 434f 4c55         cmd["COLU
+00006970: 4d4e 5322 5d20 3d20 7365 6c66 2e63 6f6e  MNS"] = self.con
+00006980: 7465 7374 2e63 6f6c 756d 6e73 0a20 2020  test.columns.   
+00006990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000069a0: 2073 656c 662e 6d75 6c74 6963 6173 745f   self.multicast_
+000069b0: 696e 7465 7266 6163 652e 7365 6e64 5f61  interface.send_a
+000069c0: 735f 6a73 6f6e 2863 6d64 290a 0a20 2020  s_json(cmd)..   
+000069d0: 2064 6566 2063 6865 636b 5f66 6f72 5f6e   def check_for_n
+000069e0: 6577 5f63 7479 2873 656c 6629 3a0a 2020  ew_cty(self):.  
+000069f0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00006a00: 2020 4368 6563 6b73 2066 6f72 2061 206e    Checks for a n
+00006a10: 6577 2063 7479 2e64 6174 2066 696c 652e  ew cty.dat file.
+00006a20: 0a20 2020 2020 2020 204c 6f61 6473 2069  .        Loads i
+00006a30: 7420 6966 2061 7661 696c 6162 6c65 2e0a  t if available..
+00006a40: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00006a50: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00006a60: 2020 2020 2063 7479 203d 206e 6f74 6374       cty = notct
+00006a70: 7970 6172 7365 722e 4269 6743 7479 2857  yparser.BigCty(W
+00006a80: 4f52 4b49 4e47 5f50 4154 4820 2b20 222f  ORKING_PATH + "/
+00006a90: 6461 7461 2f63 7479 2e6a 736f 6e22 290a  data/cty.json").
+00006aa0: 2020 2020 2020 2020 2020 2020 7570 6461              upda
+00006ab0: 7465 5f61 7661 696c 6162 6c65 203d 2063  te_available = c
+00006ac0: 7479 2e63 6865 636b 5f75 7064 6174 6528  ty.check_update(
+00006ad0: 290a 2020 2020 2020 2020 6578 6365 7074  ).        except
+00006ae0: 2041 7474 7269 6275 7465 4572 726f 7220   AttributeError 
+00006af0: 6173 2074 6865 5f65 7272 6f72 3a0a 2020  as the_error:.  
+00006b00: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+00006b10: 2e64 6562 7567 2822 6374 7920 7061 7273  .debug("cty pars
+00006b20: 6572 2072 6574 7572 6e65 6420 616e 2065  er returned an e
+00006b30: 7272 6f72 3a20 2573 222c 2074 6865 5f65  rror: %s", the_e
+00006b40: 7272 6f72 290a 2020 2020 2020 2020 2020  rror).          
+00006b50: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+00006b60: 2065 7863 6570 7420 5661 6c75 6545 7272   except ValueErr
+00006b70: 6f72 2061 7320 7468 655f 6572 726f 723a  or as the_error:
+00006b80: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00006b90: 6e74 2822 6374 7920 7061 7273 6572 2072  nt("cty parser r
+00006ba0: 6574 7572 6e65 6420 616e 2065 7272 6f72  eturned an error
+00006bb0: 3a20 2573 222c 2074 6865 5f65 7272 6f72  : %s", the_error
+00006bc0: 290a 2020 2020 2020 2020 2020 2020 6c6f  ).            lo
+00006bd0: 6767 6572 2e64 6562 7567 2822 6374 7920  gger.debug("cty 
+00006be0: 7061 7273 6572 2072 6574 7572 6e65 6420  parser returned 
+00006bf0: 616e 2065 7272 6f72 3a20 2573 222c 2074  an error: %s", t
+00006c00: 6865 5f65 7272 6f72 290a 2020 2020 2020  he_error).      
+00006c10: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+00006c20: 2020 2020 2065 7863 6570 7420 6c6f 6361       except loca
+00006c30: 6c65 2e45 7272 6f72 2061 7320 7468 655f  le.Error as the_
+00006c40: 6572 726f 723a 0a20 2020 2020 2020 2020  error:.         
+00006c50: 2020 2070 7269 6e74 2822 6374 7920 7061     print("cty pa
+00006c60: 7273 6572 2072 6574 7572 6e65 6420 616e  rser returned an
+00006c70: 2065 7272 6f72 3a20 2573 222c 2074 6865   error: %s", the
+00006c80: 5f65 7272 6f72 290a 2020 2020 2020 2020  _error).        
+00006c90: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+00006ca0: 2822 6374 7920 7061 7273 6572 2072 6574  ("cty parser ret
+00006cb0: 7572 6e65 6420 616e 2065 7272 6f72 3a20  urned an error: 
+00006cc0: 2573 222c 2074 6865 5f65 7272 6f72 290a  %s", the_error).
+00006cd0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00006ce0: 726e 0a20 2020 2020 2020 206c 6f67 6765  rn.        logge
+00006cf0: 722e 6465 6275 6728 224e 6577 6572 2063  r.debug("Newer c
+00006d00: 7479 2066 696c 6520 6176 6169 6c61 626c  ty file availabl
+00006d10: 6520 2573 222c 2073 7472 2875 7064 6174  e %s", str(updat
+00006d20: 655f 6176 6169 6c61 626c 6529 290a 0a20  e_available)).. 
+00006d30: 2020 2020 2020 2069 6620 7570 6461 7465         if update
+00006d40: 5f61 7661 696c 6162 6c65 3a0a 2020 2020  _available:.    
+00006d50: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+00006d60: 2020 2020 2020 2020 2020 2020 2075 7064               upd
+00006d70: 6174 6564 203d 2063 7479 2e75 7064 6174  ated = cty.updat
+00006d80: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+00006d90: 6578 6365 7074 2052 6573 6f75 7263 6557  except ResourceW
+00006da0: 6172 6e69 6e67 2061 7320 7468 655f 6572  arning as the_er
+00006db0: 726f 723a 0a20 2020 2020 2020 2020 2020  ror:.           
+00006dc0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+00006dd0: 6728 2263 7479 2070 6172 7365 7220 7265  g("cty parser re
+00006de0: 7475 726e 6564 2061 6e20 6572 726f 723a  turned an error:
+00006df0: 2025 7322 2c20 7468 655f 6572 726f 7229   %s", the_error)
+00006e00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006e10: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+00006e20: 2020 2020 6966 2075 7064 6174 6564 3a0a      if updated:.
 00006e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e40: 7365 6c66 2e73 686f 775f 6d65 7373 6167  self.show_messag
-00006e50: 655f 626f 7828 2263 7479 2066 696c 6520  e_box("cty file 
-00006e60: 7570 6461 7465 642e 2229 0a20 2020 2020  updated.").     
-00006e70: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-00006e80: 6f70 656e 280a 2020 2020 2020 2020 2020  open(.          
-00006e90: 2020 2020 2020 2020 2020 574f 524b 494e            WORKIN
-00006ea0: 475f 5041 5448 202b 2022 2f64 6174 612f  G_PATH + "/data/
-00006eb0: 6374 792e 6a73 6f6e 222c 2022 7274 222c  cty.json", "rt",
-00006ec0: 2065 6e63 6f64 696e 673d 2275 7466 2d38   encoding="utf-8
-00006ed0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00006ee0: 2020 2920 6173 2063 7479 6669 6c65 3a0a    ) as ctyfile:.
-00006ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f00: 2020 2020 676c 6f62 616c 7328 295b 2243      globals()["C
-00006f10: 5459 4649 4c45 225d 203d 206c 6f61 6473  TYFILE"] = loads
-00006f20: 2863 7479 6669 6c65 2e72 6561 6428 2929  (ctyfile.read())
-00006f30: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00006f40: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00006f50: 2020 2073 656c 662e 7368 6f77 5f6d 6573     self.show_mes
-00006f60: 7361 6765 5f62 6f78 2822 416e 2045 7272  sage_box("An Err
-00006f70: 6f72 206f 6363 7572 6564 2075 7064 6174  or occured updat
-00006f80: 696e 6720 6669 6c65 2e22 290a 2020 2020  ing file.").    
-00006f90: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00006fa0: 2020 2020 2020 7365 6c66 2e73 686f 775f        self.show_
-00006fb0: 6d65 7373 6167 655f 626f 7828 2243 5459  message_box("CTY
-00006fc0: 2066 696c 6520 6973 2075 7020 746f 2064   file is up to d
-00006fd0: 6174 652e 2229 0a0a 2020 2020 6465 6620  ate.")..    def 
-00006fe0: 6869 6465 5f62 616e 645f 6d6f 6465 2873  hide_band_mode(s
-00006ff0: 656c 662c 2074 6865 5f6d 6f64 653a 2073  elf, the_mode: s
-00007000: 7472 2920 2d3e 204e 6f6e 653a 0a20 2020  tr) -> None:.   
-00007010: 2020 2020 2022 2222 6869 6465 2222 220a       """hide""".
-00007020: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-00007030: 6562 7567 2822 2573 222c 2066 227b 7468  ebug("%s", f"{th
-00007040: 655f 6d6f 6465 7d22 290a 2020 2020 2020  e_mode}").      
-00007050: 2020 7365 6c66 2e42 616e 645f 4d6f 6465    self.Band_Mode
-00007060: 5f46 7261 6d65 5f43 572e 6869 6465 2829  _Frame_CW.hide()
-00007070: 0a20 2020 2020 2020 2073 656c 662e 4261  .        self.Ba
-00007080: 6e64 5f4d 6f64 655f 4672 616d 655f 5353  nd_Mode_Frame_SS
-00007090: 422e 6869 6465 2829 0a20 2020 2020 2020  B.hide().       
-000070a0: 2073 656c 662e 4261 6e64 5f4d 6f64 655f   self.Band_Mode_
-000070b0: 4672 616d 655f 5254 5459 2e68 6964 6528  Frame_RTTY.hide(
-000070c0: 290a 2020 2020 2020 2020 6d6f 6465 7320  ).        modes 
-000070d0: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
-000070e0: 2243 5722 3a20 2873 656c 662e 4261 6e64  "CW": (self.Band
-000070f0: 5f4d 6f64 655f 4672 616d 655f 4357 2c29  _Mode_Frame_CW,)
-00007100: 2c0a 2020 2020 2020 2020 2020 2020 2253  ,.            "S
-00007110: 5342 223a 2028 7365 6c66 2e42 616e 645f  SB": (self.Band_
-00007120: 4d6f 6465 5f46 7261 6d65 5f53 5342 2c29  Mode_Frame_SSB,)
-00007130: 2c0a 2020 2020 2020 2020 2020 2020 2252  ,.            "R
-00007140: 5454 5922 3a20 2873 656c 662e 4261 6e64  TTY": (self.Band
-00007150: 5f4d 6f64 655f 4672 616d 655f 5254 5459  _Mode_Frame_RTTY
-00007160: 2c29 2c0a 2020 2020 2020 2020 2020 2020  ,),.            
-00007170: 2250 534b 223a 2028 7365 6c66 2e42 616e  "PSK": (self.Ban
-00007180: 645f 4d6f 6465 5f46 7261 6d65 5f52 5454  d_Mode_Frame_RTT
-00007190: 592c 292c 0a20 2020 2020 2020 2020 2020  Y,),.           
-000071a0: 2022 5353 422b 4357 223a 2028 7365 6c66   "SSB+CW": (self
-000071b0: 2e42 616e 645f 4d6f 6465 5f46 7261 6d65  .Band_Mode_Frame
-000071c0: 5f43 572c 2073 656c 662e 4261 6e64 5f4d  _CW, self.Band_M
-000071d0: 6f64 655f 4672 616d 655f 5353 4229 2c0a  ode_Frame_SSB),.
-000071e0: 2020 2020 2020 2020 2020 2020 2242 4f54              "BOT
-000071f0: 4822 3a20 2873 656c 662e 4261 6e64 5f4d  H": (self.Band_M
-00007200: 6f64 655f 4672 616d 655f 4357 2c20 7365  ode_Frame_CW, se
-00007210: 6c66 2e42 616e 645f 4d6f 6465 5f46 7261  lf.Band_Mode_Fra
-00007220: 6d65 5f53 5342 292c 0a20 2020 2020 2020  me_SSB),.       
-00007230: 2020 2020 2022 4449 4749 5441 4c22 3a20       "DIGITAL": 
-00007240: 2873 656c 662e 4261 6e64 5f4d 6f64 655f  (self.Band_Mode_
-00007250: 4672 616d 655f 5254 5459 2c29 2c0a 2020  Frame_RTTY,),.  
-00007260: 2020 2020 2020 2020 2020 2253 5342 2b43            "SSB+C
-00007270: 572b 4449 4749 5441 4c22 3a20 280a 2020  W+DIGITAL": (.  
-00007280: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00007290: 6c66 2e42 616e 645f 4d6f 6465 5f46 7261  lf.Band_Mode_Fra
-000072a0: 6d65 5f52 5454 592c 0a20 2020 2020 2020  me_RTTY,.       
-000072b0: 2020 2020 2020 2020 2073 656c 662e 4261           self.Ba
-000072c0: 6e64 5f4d 6f64 655f 4672 616d 655f 4357  nd_Mode_Frame_CW
-000072d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000072e0: 2020 7365 6c66 2e42 616e 645f 4d6f 6465    self.Band_Mode
-000072f0: 5f46 7261 6d65 5f53 5342 2c0a 2020 2020  _Frame_SSB,.    
-00007300: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
-00007310: 2020 2020 2020 2022 464d 223a 2028 7365         "FM": (se
-00007320: 6c66 2e42 616e 645f 4d6f 6465 5f46 7261  lf.Band_Mode_Fra
-00007330: 6d65 5f53 5342 2c29 2c0a 2020 2020 2020  me_SSB,),.      
-00007340: 2020 7d0a 2020 2020 2020 2020 6672 616d    }.        fram
-00007350: 6573 203d 206d 6f64 6573 2e67 6574 2874  es = modes.get(t
-00007360: 6865 5f6d 6f64 6529 0a20 2020 2020 2020  he_mode).       
-00007370: 2069 6620 6672 616d 6573 3a0a 2020 2020   if frames:.    
-00007380: 2020 2020 2020 2020 666f 7220 6672 616d          for fram
-00007390: 6520 696e 2066 7261 6d65 733a 0a20 2020  e in frames:.   
-000073a0: 2020 2020 2020 2020 2020 2020 2066 7261               fra
-000073b0: 6d65 2e73 686f 7728 290a 0a20 2020 2064  me.show()..    d
-000073c0: 6566 2073 686f 775f 6b65 795f 6865 6c70  ef show_key_help
-000073d0: 2873 656c 6629 202d 3e20 4e6f 6e65 3a0a  (self) -> None:.
-000073e0: 2020 2020 2020 2020 2222 2253 686f 7720          """Show 
-000073f0: 6865 6c70 2062 6f78 2066 6f72 2068 6f74  help box for hot
-00007400: 6b65 7973 2222 220a 2020 2020 2020 2020  keys""".        
-00007410: 7365 6c66 2e73 686f 775f 6d65 7373 6167  self.show_messag
-00007420: 655f 626f 7828 0a20 2020 2020 2020 2020  e_box(.         
-00007430: 2020 2022 5b45 7363 5d5c 7443 6c65 6172     "[Esc]\tClear
-00007440: 7320 7468 6520 696e 7075 7420 6669 656c  s the input fiel
-00007450: 6473 206f 6620 616e 7920 7465 7874 2e5c  ds of any text.\
-00007460: 6e22 0a20 2020 2020 2020 2020 2020 2022  n".            "
-00007470: 5b43 5452 4c2d 4573 635d 5c74 5374 6f70  [CTRL-Esc]\tStop
-00007480: 7320 6377 6461 656d 6f6e 2066 726f 6d20  s cwdaemon from 
-00007490: 7365 6e64 696e 6720 4d6f 7273 652e 5c6e  sending Morse.\n
-000074a0: 220a 2020 2020 2020 2020 2020 2020 225b  ".            "[
-000074b0: 5067 5570 5d5c 7449 6e63 7265 6173 6573  PgUp]\tIncreases
-000074c0: 2074 6865 2063 7720 7365 6e64 696e 6720   the cw sending 
-000074d0: 7370 6565 642e 5c6e 220a 2020 2020 2020  speed.\n".      
-000074e0: 2020 2020 2020 225b 5067 446f 776e 5d5c        "[PgDown]\
-000074f0: 7444 6563 7265 6173 6573 2074 6865 2063  tDecreases the c
+00006e40: 6374 792e 6475 6d70 2857 4f52 4b49 4e47  cty.dump(WORKING
+00006e50: 5f50 4154 4820 2b20 222f 6461 7461 2f63  _PATH + "/data/c
+00006e60: 7479 2e6a 736f 6e22 290a 2020 2020 2020  ty.json").      
+00006e70: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00006e80: 686f 775f 6d65 7373 6167 655f 626f 7828  how_message_box(
+00006e90: 2263 7479 2066 696c 6520 7570 6461 7465  "cty file update
+00006ea0: 642e 2229 0a20 2020 2020 2020 2020 2020  d.").           
+00006eb0: 2020 2020 2077 6974 6820 6f70 656e 280a       with open(.
+00006ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ed0: 2020 2020 574f 524b 494e 475f 5041 5448      WORKING_PATH
+00006ee0: 202b 2022 2f64 6174 612f 6374 792e 6a73   + "/data/cty.js
+00006ef0: 6f6e 222c 2022 7274 222c 2065 6e63 6f64  on", "rt", encod
+00006f00: 696e 673d 2275 7466 2d38 220a 2020 2020  ing="utf-8".    
+00006f10: 2020 2020 2020 2020 2020 2020 2920 6173              ) as
+00006f20: 2063 7479 6669 6c65 3a0a 2020 2020 2020   ctyfile:.      
+00006f30: 2020 2020 2020 2020 2020 2020 2020 676c                gl
+00006f40: 6f62 616c 7328 295b 2243 5459 4649 4c45  obals()["CTYFILE
+00006f50: 225d 203d 206c 6f61 6473 2863 7479 6669  "] = loads(ctyfi
+00006f60: 6c65 2e72 6561 6428 2929 0a20 2020 2020  le.read()).     
+00006f70: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00006f80: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00006f90: 662e 7368 6f77 5f6d 6573 7361 6765 5f62  f.show_message_b
+00006fa0: 6f78 2822 416e 2045 7272 6f72 206f 6363  ox("An Error occ
+00006fb0: 7572 6564 2075 7064 6174 696e 6720 6669  ured updating fi
+00006fc0: 6c65 2e22 290a 2020 2020 2020 2020 656c  le.").        el
+00006fd0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00006fe0: 7365 6c66 2e73 686f 775f 6d65 7373 6167  self.show_messag
+00006ff0: 655f 626f 7828 2243 5459 2066 696c 6520  e_box("CTY file 
+00007000: 6973 2075 7020 746f 2064 6174 652e 2229  is up to date.")
+00007010: 0a0a 2020 2020 6465 6620 6869 6465 5f62  ..    def hide_b
+00007020: 616e 645f 6d6f 6465 2873 656c 662c 2074  and_mode(self, t
+00007030: 6865 5f6d 6f64 653a 2073 7472 2920 2d3e  he_mode: str) ->
+00007040: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
+00007050: 2222 6869 6465 2222 220a 2020 2020 2020  ""hide""".      
+00007060: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+00007070: 2573 222c 2066 227b 7468 655f 6d6f 6465  %s", f"{the_mode
+00007080: 7d22 290a 2020 2020 2020 2020 7365 6c66  }").        self
+00007090: 2e42 616e 645f 4d6f 6465 5f46 7261 6d65  .Band_Mode_Frame
+000070a0: 5f43 572e 6869 6465 2829 0a20 2020 2020  _CW.hide().     
+000070b0: 2020 2073 656c 662e 4261 6e64 5f4d 6f64     self.Band_Mod
+000070c0: 655f 4672 616d 655f 5353 422e 6869 6465  e_Frame_SSB.hide
+000070d0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+000070e0: 4261 6e64 5f4d 6f64 655f 4672 616d 655f  Band_Mode_Frame_
+000070f0: 5254 5459 2e68 6964 6528 290a 2020 2020  RTTY.hide().    
+00007100: 2020 2020 6d6f 6465 7320 3d20 7b0a 2020      modes = {.  
+00007110: 2020 2020 2020 2020 2020 2243 5722 3a20            "CW": 
+00007120: 2873 656c 662e 4261 6e64 5f4d 6f64 655f  (self.Band_Mode_
+00007130: 4672 616d 655f 4357 2c29 2c0a 2020 2020  Frame_CW,),.    
+00007140: 2020 2020 2020 2020 2253 5342 223a 2028          "SSB": (
+00007150: 7365 6c66 2e42 616e 645f 4d6f 6465 5f46  self.Band_Mode_F
+00007160: 7261 6d65 5f53 5342 2c29 2c0a 2020 2020  rame_SSB,),.    
+00007170: 2020 2020 2020 2020 2252 5454 5922 3a20          "RTTY": 
+00007180: 2873 656c 662e 4261 6e64 5f4d 6f64 655f  (self.Band_Mode_
+00007190: 4672 616d 655f 5254 5459 2c29 2c0a 2020  Frame_RTTY,),.  
+000071a0: 2020 2020 2020 2020 2020 2250 534b 223a            "PSK":
+000071b0: 2028 7365 6c66 2e42 616e 645f 4d6f 6465   (self.Band_Mode
+000071c0: 5f46 7261 6d65 5f52 5454 592c 292c 0a20  _Frame_RTTY,),. 
+000071d0: 2020 2020 2020 2020 2020 2022 5353 422b             "SSB+
+000071e0: 4357 223a 2028 7365 6c66 2e42 616e 645f  CW": (self.Band_
+000071f0: 4d6f 6465 5f46 7261 6d65 5f43 572c 2073  Mode_Frame_CW, s
+00007200: 656c 662e 4261 6e64 5f4d 6f64 655f 4672  elf.Band_Mode_Fr
+00007210: 616d 655f 5353 4229 2c0a 2020 2020 2020  ame_SSB),.      
+00007220: 2020 2020 2020 2242 4f54 4822 3a20 2873        "BOTH": (s
+00007230: 656c 662e 4261 6e64 5f4d 6f64 655f 4672  elf.Band_Mode_Fr
+00007240: 616d 655f 4357 2c20 7365 6c66 2e42 616e  ame_CW, self.Ban
+00007250: 645f 4d6f 6465 5f46 7261 6d65 5f53 5342  d_Mode_Frame_SSB
+00007260: 292c 0a20 2020 2020 2020 2020 2020 2022  ),.            "
+00007270: 4449 4749 5441 4c22 3a20 2873 656c 662e  DIGITAL": (self.
+00007280: 4261 6e64 5f4d 6f64 655f 4672 616d 655f  Band_Mode_Frame_
+00007290: 5254 5459 2c29 2c0a 2020 2020 2020 2020  RTTY,),.        
+000072a0: 2020 2020 2253 5342 2b43 572b 4449 4749      "SSB+CW+DIGI
+000072b0: 5441 4c22 3a20 280a 2020 2020 2020 2020  TAL": (.        
+000072c0: 2020 2020 2020 2020 7365 6c66 2e42 616e          self.Ban
+000072d0: 645f 4d6f 6465 5f46 7261 6d65 5f52 5454  d_Mode_Frame_RTT
+000072e0: 592c 0a20 2020 2020 2020 2020 2020 2020  Y,.             
+000072f0: 2020 2073 656c 662e 4261 6e64 5f4d 6f64     self.Band_Mod
+00007300: 655f 4672 616d 655f 4357 2c0a 2020 2020  e_Frame_CW,.    
+00007310: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00007320: 2e42 616e 645f 4d6f 6465 5f46 7261 6d65  .Band_Mode_Frame
+00007330: 5f53 5342 2c0a 2020 2020 2020 2020 2020  _SSB,.          
+00007340: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
+00007350: 2022 464d 223a 2028 7365 6c66 2e42 616e   "FM": (self.Ban
+00007360: 645f 4d6f 6465 5f46 7261 6d65 5f53 5342  d_Mode_Frame_SSB
+00007370: 2c29 2c0a 2020 2020 2020 2020 7d0a 2020  ,),.        }.  
+00007380: 2020 2020 2020 6672 616d 6573 203d 206d        frames = m
+00007390: 6f64 6573 2e67 6574 2874 6865 5f6d 6f64  odes.get(the_mod
+000073a0: 6529 0a20 2020 2020 2020 2069 6620 6672  e).        if fr
+000073b0: 616d 6573 3a0a 2020 2020 2020 2020 2020  ames:.          
+000073c0: 2020 666f 7220 6672 616d 6520 696e 2066    for frame in f
+000073d0: 7261 6d65 733a 0a20 2020 2020 2020 2020  rames:.         
+000073e0: 2020 2020 2020 2066 7261 6d65 2e73 686f         frame.sho
+000073f0: 7728 290a 0a20 2020 2064 6566 2073 686f  w()..    def sho
+00007400: 775f 6b65 795f 6865 6c70 2873 656c 6629  w_key_help(self)
+00007410: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00007420: 2020 2222 2253 686f 7720 6865 6c70 2062    """Show help b
+00007430: 6f78 2066 6f72 2068 6f74 6b65 7973 2222  ox for hotkeys""
+00007440: 220a 2020 2020 2020 2020 7365 6c66 2e73  ".        self.s
+00007450: 686f 775f 6d65 7373 6167 655f 626f 7828  how_message_box(
+00007460: 0a20 2020 2020 2020 2020 2020 2022 5b45  .            "[E
+00007470: 7363 5d5c 7443 6c65 6172 7320 7468 6520  sc]\tClears the 
+00007480: 696e 7075 7420 6669 656c 6473 206f 6620  input fields of 
+00007490: 616e 7920 7465 7874 2e5c 6e22 0a20 2020  any text.\n".   
+000074a0: 2020 2020 2020 2020 2022 5b43 5452 4c2d           "[CTRL-
+000074b0: 4573 635d 5c74 5374 6f70 7320 6377 6461  Esc]\tStops cwda
+000074c0: 656d 6f6e 2066 726f 6d20 7365 6e64 696e  emon from sendin
+000074d0: 6720 4d6f 7273 652e 5c6e 220a 2020 2020  g Morse.\n".    
+000074e0: 2020 2020 2020 2020 225b 5067 5570 5d5c          "[PgUp]\
+000074f0: 7449 6e63 7265 6173 6573 2074 6865 2063  tIncreases the c
 00007500: 7720 7365 6e64 696e 6720 7370 6565 642e  w sending speed.
 00007510: 5c6e 220a 2020 2020 2020 2020 2020 2020  \n".            
-00007520: 225b 4172 726f 772d 5570 5d20 4a75 6d70  "[Arrow-Up] Jump
-00007530: 2074 6f20 7468 6520 6e65 7874 2073 706f   to the next spo
-00007540: 7420 6162 6f76 6520 7468 6520 6375 7272  t above the curr
-00007550: 656e 7420 5646 4f20 6375 7273 6f72 5c6e  ent VFO cursor\n
-00007560: 220a 2020 2020 2020 2020 2020 2020 225c  ".            "\
-00007570: 7469 6e20 7468 6520 6261 6e64 6d61 7020  tin the bandmap 
-00007580: 7769 6e64 6f77 2028 4341 5420 5265 7175  window (CAT Requ
-00007590: 6972 6564 292e 5c6e 220a 2020 2020 2020  ired).\n".      
-000075a0: 2020 2020 2020 225b 4172 726f 772d 446f        "[Arrow-Do
-000075b0: 776e 5d20 4a75 6d70 2074 6f20 7468 6520  wn] Jump to the 
-000075c0: 6e65 7874 2073 706f 7420 6265 6c6f 7720  next spot below 
-000075d0: 7468 6520 6375 7272 656e 745c 6e22 0a20  the current\n". 
-000075e0: 2020 2020 2020 2020 2020 2022 5c74 5646             "\tVF
-000075f0: 4f20 6375 7273 6f72 2069 6e20 7468 6520  O cursor in the 
-00007600: 6261 6e64 6d61 7020 7769 6e64 6f77 2028  bandmap window (
-00007610: 4341 5420 5265 7175 6972 6564 292e 5c6e  CAT Required).\n
-00007620: 220a 2020 2020 2020 2020 2020 2020 225b  ".            "[
-00007630: 5441 425d 5c74 4d6f 7665 2063 7572 736f  TAB]\tMove curso
-00007640: 7220 746f 2074 6865 2072 6967 6874 206f  r to the right o
-00007650: 6e65 2066 6965 6c64 2e5c 6e22 0a20 2020  ne field.\n".   
-00007660: 2020 2020 2020 2020 2022 5b53 6869 6674           "[Shift
-00007670: 2d54 6162 5d5c 744d 6f76 6520 6375 7273  -Tab]\tMove curs
-00007680: 6f72 206c 6566 7420 4f6e 6520 6669 656c  or left One fiel
-00007690: 642e 5c6e 220a 2020 2020 2020 2020 2020  d.\n".          
-000076a0: 2020 225b 5350 4143 455d 5c74 5768 656e    "[SPACE]\tWhen
-000076b0: 2069 6e20 7468 6520 6361 6c6c 7369 676e   in the callsign
-000076c0: 2066 6965 6c64 2c20 7769 6c6c 206d 6f76   field, will mov
-000076d0: 6520 7468 6520 696e 7075 7420 746f 2074  e the input to t
-000076e0: 6865 5c6e 220a 2020 2020 2020 2020 2020  he\n".          
-000076f0: 2020 225c 7466 6972 7374 2066 6965 6c64    "\tfirst field
-00007700: 206e 6565 6465 6420 666f 7220 7468 6520   needed for the 
-00007710: 6578 6368 616e 6765 2e5c 6e22 0a20 2020  exchange.\n".   
-00007720: 2020 2020 2020 2020 2022 5b45 6e74 6572           "[Enter
-00007730: 5d5c 7453 7562 6d69 7473 2074 6865 2066  ]\tSubmits the f
-00007740: 6965 6c64 7320 746f 2074 6865 206c 6f67  ields to the log
-00007750: 2e5c 6e22 0a20 2020 2020 2020 2020 2020  .\n".           
-00007760: 2022 5b46 312d 4631 325d 5c74 5365 6e64   "[F1-F12]\tSend
-00007770: 2028 4357 206f 7220 566f 6963 6529 206d   (CW or Voice) m
-00007780: 6163 726f 732e 5c6e 220a 2020 2020 2020  acros.\n".      
-00007790: 2020 2020 2020 225b 4354 524c 2d53 5d5c        "[CTRL-S]\
-000077a0: 7453 706f 7420 4361 6c6c 7369 676e 2074  tSpot Callsign t
-000077b0: 6f20 7468 6520 636c 7573 7465 722e 5c6e  o the cluster.\n
-000077c0: 220a 2020 2020 2020 2020 2020 2020 225b  ".            "[
-000077d0: 4354 524c 2d47 5d5c 7454 756e 6520 746f  CTRL-G]\tTune to
-000077e0: 2061 2073 706f 7420 6d61 7463 6869 6e67   a spot matching
-000077f0: 2070 6172 7469 616c 2074 6578 7420 696e   partial text in
-00007800: 2074 6865 2063 616c 6c73 6967 6e5c 6e22   the callsign\n"
-00007810: 0a20 2020 2020 2020 2020 2020 2022 5c74  .            "\t
-00007820: 656e 7472 7920 6669 656c 6420 2843 4154  entry field (CAT
-00007830: 2052 6571 7569 7265 6429 2e5c 6e22 0a20   Required).\n". 
-00007840: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
-00007850: 6620 6669 6c65 7069 636b 6572 2873 656c  f filepicker(sel
-00007860: 662c 2061 6374 696f 6e3a 2073 7472 2920  f, action: str) 
-00007870: 2d3e 2073 7472 3a0a 2020 2020 2020 2020  -> str:.        
-00007880: 2222 220a 2020 2020 2020 2020 4765 7420  """.        Get 
-00007890: 6120 6669 6c65 6e61 6d65 0a20 2020 2020  a filename.     
-000078a0: 2020 2061 6374 696f 6e3a 2022 6e65 7722     action: "new"
-000078b0: 206f 7220 226f 7065 6e22 0a20 2020 2020   or "open".     
-000078c0: 2020 2022 2222 0a20 2020 2020 2020 206f     """.        o
-000078d0: 7074 696f 6e73 203d 2051 4669 6c65 4469  ptions = QFileDi
-000078e0: 616c 6f67 2e4f 7074 696f 6e73 2829 0a20  alog.Options(). 
-000078f0: 2020 2020 2020 206f 7074 696f 6e73 207c         options |
-00007900: 3d20 5146 696c 6544 6961 6c6f 672e 446f  = QFileDialog.Do
-00007910: 6e74 5573 654e 6174 6976 6544 6961 6c6f  ntUseNativeDialo
-00007920: 670a 2020 2020 2020 2020 6f70 7469 6f6e  g.        option
-00007930: 7320 7c3d 2051 4669 6c65 4469 616c 6f67  s |= QFileDialog
-00007940: 2e44 6f6e 7443 6f6e 6669 726d 4f76 6572  .DontConfirmOver
-00007950: 7772 6974 650a 2020 2020 2020 2020 6966  write.        if
-00007960: 2061 6374 696f 6e20 3d3d 2022 6e65 7722   action == "new"
-00007970: 3a0a 2020 2020 2020 2020 2020 2020 6669  :.            fi
-00007980: 6c65 2c20 5f20 3d20 5146 696c 6544 6961  le, _ = QFileDia
-00007990: 6c6f 672e 6765 7453 6176 6546 696c 654e  log.getSaveFileN
-000079a0: 616d 6528 0a20 2020 2020 2020 2020 2020  ame(.           
-000079b0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-000079c0: 2020 2020 2020 2020 2020 2022 4368 6f6f             "Choo
-000079d0: 7365 2061 2044 6174 6162 6173 6522 2c0a  se a Database",.
-000079e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079f0: 4441 5441 5f50 4154 482c 0a20 2020 2020  DATA_PATH,.     
-00007a00: 2020 2020 2020 2020 2020 2022 4461 7461             "Data
-00007a10: 6261 7365 2028 2a2e 6462 2922 2c0a 2020  base (*.db)",.  
-00007a20: 2020 2020 2020 2020 2020 2020 2020 6f70                op
-00007a30: 7469 6f6e 733d 6f70 7469 6f6e 732c 0a20  tions=options,. 
-00007a40: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00007a50: 2020 2020 2069 6620 6163 7469 6f6e 203d       if action =
-00007a60: 3d20 226f 7065 6e22 3a0a 2020 2020 2020  = "open":.      
-00007a70: 2020 2020 2020 6669 6c65 2c20 5f20 3d20        file, _ = 
-00007a80: 5146 696c 6544 6961 6c6f 672e 6765 744f  QFileDialog.getO
-00007a90: 7065 6e46 696c 654e 616d 6528 0a20 2020  penFileName(.   
-00007aa0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00007ab0: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
-00007ac0: 2020 2022 4368 6f6f 7365 2061 2044 6174     "Choose a Dat
-00007ad0: 6162 6173 6522 2c0a 2020 2020 2020 2020  abase",.        
-00007ae0: 2020 2020 2020 2020 4441 5441 5f50 4154          DATA_PAT
-00007af0: 482c 0a20 2020 2020 2020 2020 2020 2020  H,.             
-00007b00: 2020 2022 4461 7461 6261 7365 2028 2a2e     "Database (*.
-00007b10: 6462 2922 2c0a 2020 2020 2020 2020 2020  db)",.          
-00007b20: 2020 2020 2020 6f70 7469 6f6e 733d 6f70        options=op
-00007b30: 7469 6f6e 732c 0a20 2020 2020 2020 2020  tions,.         
-00007b40: 2020 2029 0a20 2020 2020 2020 2072 6574     ).        ret
-00007b50: 7572 6e20 6669 6c65 0a0a 2020 2020 6465  urn file..    de
-00007b60: 6620 7265 6361 6c63 756c 6174 655f 6d75  f recalculate_mu
-00007b70: 6c74 7328 7365 6c66 293a 0a20 2020 2020  lts(self):.     
-00007b80: 2020 2022 2222 5265 6361 6c63 756c 6174     """Recalculat
-00007b90: 6520 4d75 6c74 6970 6c69 6572 7322 2222  e Multipliers"""
-00007ba0: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-00007bb0: 6e74 6573 742e 7265 6361 6c63 756c 6174  ntest.recalculat
-00007bc0: 655f 6d75 6c74 7328 7365 6c66 290a 2020  e_mults(self).  
-00007bd0: 2020 2020 2020 7365 6c66 2e63 6c65 6172        self.clear
-00007be0: 696e 7075 7473 2829 0a0a 2020 2020 6465  inputs()..    de
-00007bf0: 6620 6c61 756e 6368 5f6c 6f67 5f77 696e  f launch_log_win
-00007c00: 646f 7728 7365 6c66 293a 0a20 2020 2020  dow(self):.     
-00007c10: 2020 2022 2222 6c61 756e 6368 2074 6865     """launch the
-00007c20: 204c 6f67 2057 696e 646f 7722 2222 0a20   Log Window""". 
-00007c30: 2020 2020 2020 2069 6620 6e6f 7420 6368         if not ch
-00007c40: 6563 6b5f 7072 6f63 6573 7328 226c 6f67  eck_process("log
-00007c50: 7769 6e64 6f77 2e70 7922 293a 0a20 2020  window.py"):.   
-00007c60: 2020 2020 2020 2020 205f 203d 2073 7562           _ = sub
-00007c70: 7072 6f63 6573 732e 506f 7065 6e28 5b73  process.Popen([s
-00007c80: 7973 2e65 7865 6375 7461 626c 652c 2057  ys.executable, W
-00007c90: 4f52 4b49 4e47 5f50 4154 4820 2b20 222f  ORKING_PATH + "/
-00007ca0: 6c6f 6777 696e 646f 772e 7079 225d 290a  logwindow.py"]).
-00007cb0: 0a20 2020 2064 6566 206c 6175 6e63 685f  .    def launch_
-00007cc0: 6261 6e64 6d61 705f 7769 6e64 6f77 2873  bandmap_window(s
-00007cd0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-00007ce0: 226c 6175 6e63 6820 7468 6520 4c6f 6720  "launch the Log 
-00007cf0: 5769 6e64 6f77 2222 220a 2020 2020 2020  Window""".      
-00007d00: 2020 6966 206e 6f74 2063 6865 636b 5f70    if not check_p
-00007d10: 726f 6365 7373 2822 6261 6e64 6d61 702e  rocess("bandmap.
-00007d20: 7079 2229 3a0a 2020 2020 2020 2020 2020  py"):.          
-00007d30: 2020 5f20 3d20 7375 6270 726f 6365 7373    _ = subprocess
-00007d40: 2e50 6f70 656e 285b 7379 732e 6578 6563  .Popen([sys.exec
-00007d50: 7574 6162 6c65 2c20 574f 524b 494e 475f  utable, WORKING_
-00007d60: 5041 5448 202b 2022 2f62 616e 646d 6170  PATH + "/bandmap
-00007d70: 2e70 7922 5d29 0a0a 2020 2020 6465 6620  .py"])..    def 
-00007d80: 6c61 756e 6368 5f63 6865 636b 5f77 696e  launch_check_win
-00007d90: 646f 7728 7365 6c66 293a 0a20 2020 2020  dow(self):.     
-00007da0: 2020 2022 2222 6c61 756e 6368 2074 6865     """launch the
-00007db0: 204c 6f67 2057 696e 646f 7722 2222 0a20   Log Window""". 
-00007dc0: 2020 2020 2020 2069 6620 6e6f 7420 6368         if not ch
-00007dd0: 6563 6b5f 7072 6f63 6573 7328 2263 6865  eck_process("che
-00007de0: 636b 7769 6e64 6f77 2e70 7922 293a 0a20  ckwindow.py"):. 
-00007df0: 2020 2020 2020 2020 2020 205f 203d 2073             _ = s
-00007e00: 7562 7072 6f63 6573 732e 506f 7065 6e28  ubprocess.Popen(
-00007e10: 5b73 7973 2e65 7865 6375 7461 626c 652c  [sys.executable,
-00007e20: 2057 4f52 4b49 4e47 5f50 4154 4820 2b20   WORKING_PATH + 
-00007e30: 222f 6368 6563 6b77 696e 646f 772e 7079  "/checkwindow.py
-00007e40: 225d 290a 0a20 2020 2064 6566 2063 6c65  "])..    def cle
-00007e50: 6172 5f62 616e 645f 696e 6469 6361 746f  ar_band_indicato
-00007e60: 7273 2873 656c 6629 3a0a 2020 2020 2020  rs(self):.      
-00007e70: 2020 2222 2243 6c65 6172 2074 6865 2069    """Clear the i
-00007e80: 6e64 6963 6174 6f72 7322 2222 0a20 2020  ndicators""".   
-00007e90: 2020 2020 2066 6f72 205f 2c20 696e 6469       for _, indi
-00007ea0: 6361 746f 7273 2069 6e20 7365 6c66 2e61  cators in self.a
-00007eb0: 6c6c 5f6d 6f64 655f 696e 6469 6361 746f  ll_mode_indicato
-00007ec0: 7273 2e69 7465 6d73 2829 3a0a 2020 2020  rs.items():.    
-00007ed0: 2020 2020 2020 2020 666f 7220 5f2c 2069          for _, i
-00007ee0: 6e64 6963 6174 6f72 2069 6e20 696e 6469  ndicator in indi
-00007ef0: 6361 746f 7273 2e69 7465 6d73 2829 3a0a  cators.items():.
-00007f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f10: 696e 6469 6361 746f 722e 7365 7446 7261  indicator.setFra
-00007f20: 6d65 5368 6170 6528 5174 5769 6467 6574  meShape(QtWidget
-00007f30: 732e 5146 7261 6d65 2e4e 6f46 7261 6d65  s.QFrame.NoFrame
-00007f40: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00007f50: 2020 696e 6469 6361 746f 722e 7365 7453    indicator.setS
-00007f60: 7479 6c65 5368 6565 7428 2266 6f6e 742d  tyleSheet("font-
-00007f70: 6661 6d69 6c79 3a20 4a65 7442 7261 696e  family: JetBrain
-00007f80: 7320 4d6f 6e6f 3b22 290a 0a20 2020 2064  s Mono;")..    d
-00007f90: 6566 2073 6574 5f62 616e 645f 696e 6469  ef set_band_indi
-00007fa0: 6361 746f 7228 7365 6c66 2c20 6261 6e64  cator(self, band
-00007fb0: 3a20 7374 7229 202d 3e20 4e6f 6e65 3a0a  : str) -> None:.
-00007fc0: 2020 2020 2020 2020 2222 2253 6574 2074          """Set t
-00007fd0: 6865 2062 616e 6420 696e 6469 6361 746f  he band indicato
-00007fe0: 7222 2222 0a20 2020 2020 2020 2023 206c  r""".        # l
-00007ff0: 6f67 6765 722e 6465 6275 6728 2225 7322  ogger.debug("%s"
-00008000: 2c20 6622 6261 6e64 3a7b 6261 6e64 7d20  , f"band:{band} 
-00008010: 6d6f 6465 3a20 7b73 656c 662e 6375 7272  mode: {self.curr
-00008020: 656e 745f 6d6f 6465 7d22 290a 2020 2020  ent_mode}").    
-00008030: 2020 2020 6966 2062 616e 6420 616e 6420      if band and 
-00008040: 7365 6c66 2e63 7572 7265 6e74 5f6d 6f64  self.current_mod
-00008050: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00008060: 656c 662e 636c 6561 725f 6261 6e64 5f69  elf.clear_band_i
-00008070: 6e64 6963 6174 6f72 7328 290a 2020 2020  ndicators().    
-00008080: 2020 2020 2020 2020 696e 6469 6361 746f          indicato
-00008090: 7220 3d20 7365 6c66 2e61 6c6c 5f6d 6f64  r = self.all_mod
-000080a0: 655f 696e 6469 6361 746f 7273 5b73 656c  e_indicators[sel
-000080b0: 662e 6375 7272 656e 745f 6d6f 6465 5d2e  f.current_mode].
-000080c0: 6765 7428 6261 6e64 2c20 4e6f 6e65 290a  get(band, None).
-000080d0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-000080e0: 6e64 6963 6174 6f72 3a0a 2020 2020 2020  ndicator:.      
-000080f0: 2020 2020 2020 2020 2020 696e 6469 6361            indica
-00008100: 746f 722e 7365 7446 7261 6d65 5368 6170  tor.setFrameShap
-00008110: 6528 5174 5769 6467 6574 732e 5146 7261  e(QtWidgets.QFra
-00008120: 6d65 2e42 6f78 290a 2020 2020 2020 2020  me.Box).        
-00008130: 2020 2020 2020 2020 696e 6469 6361 746f          indicato
-00008140: 722e 7365 7453 7479 6c65 5368 6565 7428  r.setStyleSheet(
-00008150: 2266 6f6e 742d 6661 6d69 6c79 3a20 4a65  "font-family: Je
-00008160: 7442 7261 696e 7320 4d6f 6e6f 3b20 636f  tBrains Mono; co
-00008170: 6c6f 723a 2067 7265 656e 3b22 290a 0a20  lor: green;").. 
-00008180: 2020 2064 6566 2063 6c6f 7365 4576 656e     def closeEven
-00008190: 7428 7365 6c66 2c20 5f65 7665 6e74 293a  t(self, _event):
-000081a0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000081b0: 2020 2020 2057 7269 7465 2077 696e 646f       Write windo
-000081c0: 7720 7369 7a65 2061 6e64 2070 6f73 6974  w size and posit
-000081d0: 696f 6e20 746f 2063 6f6e 6669 6720 6669  ion to config fi
-000081e0: 6c65 0a20 2020 2020 2020 2022 2222 0a20  le.        """. 
-000081f0: 2020 2020 2020 2063 6d64 203d 207b 7d0a         cmd = {}.
-00008200: 2020 2020 2020 2020 636d 645b 2263 6d64          cmd["cmd
-00008210: 225d 203d 2022 4841 4c54 220a 2020 2020  "] = "HALT".    
-00008220: 2020 2020 636d 645b 2273 7461 7469 6f6e      cmd["station
-00008230: 225d 203d 2070 6c61 7466 6f72 6d2e 6e6f  "] = platform.no
-00008240: 6465 2829 0a20 2020 2020 2020 2073 656c  de().        sel
-00008250: 662e 6d75 6c74 6963 6173 745f 696e 7465  f.multicast_inte
-00008260: 7266 6163 652e 7365 6e64 5f61 735f 6a73  rface.send_as_js
-00008270: 6f6e 2863 6d64 290a 2020 2020 2020 2020  on(cmd).        
-00008280: 7365 6c66 2e70 7265 665b 2277 696e 646f  self.pref["windo
-00008290: 775f 7769 6474 6822 5d20 3d20 7365 6c66  w_width"] = self
-000082a0: 2e73 697a 6528 292e 7769 6474 6828 290a  .size().width().
-000082b0: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
-000082c0: 665b 2277 696e 646f 775f 6865 6967 6874  f["window_height
-000082d0: 225d 203d 2073 656c 662e 7369 7a65 2829  "] = self.size()
-000082e0: 2e68 6569 6768 7428 290a 2020 2020 2020  .height().      
-000082f0: 2020 7365 6c66 2e70 7265 665b 2277 696e    self.pref["win
-00008300: 646f 775f 7822 5d20 3d20 7365 6c66 2e70  dow_x"] = self.p
-00008310: 6f73 2829 2e78 2829 0a20 2020 2020 2020  os().x().       
-00008320: 2073 656c 662e 7072 6566 5b22 7769 6e64   self.pref["wind
-00008330: 6f77 5f79 225d 203d 2073 656c 662e 706f  ow_y"] = self.po
-00008340: 7328 292e 7928 290a 2020 2020 2020 2020  s().y().        
-00008350: 7365 6c66 2e77 7269 7465 5f70 7265 6665  self.write_prefe
-00008360: 7265 6e63 6528 290a 0a20 2020 2064 6566  rence()..    def
-00008370: 2063 7479 5f6c 6f6f 6b75 7028 7365 6c66   cty_lookup(self
-00008380: 2c20 6361 6c6c 7369 676e 3a20 7374 7229  , callsign: str)
-00008390: 3a0a 2020 2020 2020 2020 2222 224c 6f6f  :.        """Loo
-000083a0: 6b75 7020 6361 6c6c 7369 676e 2069 6e20  kup callsign in 
-000083b0: 6374 792e 6461 7420 6669 6c65 2e0a 0a20  cty.dat file... 
-000083c0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-000083d0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-000083e0: 2d2d 2d2d 0a20 2020 2020 2020 2063 616c  ----.        cal
-000083f0: 6c73 6967 6e20 3a20 7374 720a 0a20 2020  lsign : str..   
-00008400: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
-00008410: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
-00008420: 2020 2020 2072 6574 7572 6e20 3a20 6c69       return : li
-00008430: 7374 206f 6620 6469 6374 730a 2020 2020  st of dicts.    
-00008440: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00008450: 6361 6c6c 7369 676e 203d 2063 616c 6c73  callsign = calls
-00008460: 6967 6e2e 7570 7065 7228 290a 2020 2020  ign.upper().    
-00008470: 2020 2020 666f 7220 636f 756e 7420 696e      for count in
-00008480: 2072 6576 6572 7365 6428 7261 6e67 6528   reversed(range(
-00008490: 6c65 6e28 6361 6c6c 7369 676e 2929 293a  len(callsign))):
-000084a0: 0a20 2020 2020 2020 2020 2020 2073 6561  .            sea
-000084b0: 7263 6869 7465 6d20 3d20 6361 6c6c 7369  rchitem = callsi
-000084c0: 676e 5b3a 2063 6f75 6e74 202b 2031 5d0a  gn[: count + 1].
-000084d0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000084e0: 6c74 203d 207b 6b65 793a 2076 616c 2066  lt = {key: val f
-000084f0: 6f72 206b 6579 2c20 7661 6c20 696e 2043  or key, val in C
-00008500: 5459 4649 4c45 2e69 7465 6d73 2829 2069  TYFILE.items() i
-00008510: 6620 6b65 7920 3d3d 2073 6561 7263 6869  f key == searchi
-00008520: 7465 6d7d 0a20 2020 2020 2020 2020 2020  tem}.           
-00008530: 2069 6620 6e6f 7420 7265 7375 6c74 3a0a   if not result:.
-00008540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008550: 636f 6e74 696e 7565 0a20 2020 2020 2020  continue.       
-00008560: 2020 2020 2069 6620 7265 7375 6c74 2e67       if result.g
-00008570: 6574 2873 6561 7263 6869 7465 6d29 2e67  et(searchitem).g
-00008580: 6574 2822 6578 6163 745f 6d61 7463 6822  et("exact_match"
-00008590: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000085a0: 2020 2069 6620 7365 6172 6368 6974 656d     if searchitem
-000085b0: 203d 3d20 6361 6c6c 7369 676e 3a0a 2020   == callsign:.  
-000085c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085d0: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-000085e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085f0: 636f 6e74 696e 7565 0a20 2020 2020 2020  continue.       
-00008600: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-00008610: 6c74 0a0a 2020 2020 6465 6620 6377 7370  lt..    def cwsp
-00008620: 6565 645f 7370 696e 626f 785f 6368 616e  eed_spinbox_chan
-00008630: 6765 6428 7365 6c66 293a 0a20 2020 2020  ged(self):.     
-00008640: 2020 2022 2222 7472 6967 6765 7265 6420     """triggered 
-00008650: 7768 656e 2076 616c 7565 206f 6620 4357  when value of CW
-00008660: 2073 7065 6564 2069 6e20 7468 6520 7370   speed in the sp
-00008670: 696e 626f 7820 6368 616e 6765 732e 2222  inbox changes.""
-00008680: 220a 2020 2020 2020 2020 6966 2073 656c  ".        if sel
-00008690: 662e 6377 2069 7320 4e6f 6e65 3a0a 2020  f.cw is None:.  
-000086a0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000086b0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-000086c0: 2e63 772e 7365 7276 6572 7479 7065 203d  .cw.servertype =
-000086d0: 3d20 313a 0a20 2020 2020 2020 2020 2020  = 1:.           
-000086e0: 2073 656c 662e 6377 2e73 7065 6564 203d   self.cw.speed =
-000086f0: 2073 656c 662e 6377 5f73 7065 6564 2e76   self.cw_speed.v
-00008700: 616c 7565 2829 0a20 2020 2020 2020 2020  alue().         
-00008710: 2020 2073 656c 662e 6377 2e73 656e 6463     self.cw.sendc
-00008720: 7728 6622 5c78 3162 327b 7365 6c66 2e63  w(f"\x1b2{self.c
-00008730: 772e 7370 6565 647d 2229 0a20 2020 2020  w.speed}").     
-00008740: 2020 2069 6620 7365 6c66 2e63 772e 7365     if self.cw.se
-00008750: 7276 6572 7479 7065 203d 3d20 323a 0a20  rvertype == 2:. 
-00008760: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00008770: 6377 2e73 6574 5f77 696e 6b65 7965 725f  cw.set_winkeyer_
-00008780: 7370 6565 6428 7365 6c66 2e63 775f 7370  speed(self.cw_sp
-00008790: 6565 642e 7661 6c75 6528 2929 0a0a 2020  eed.value())..  
-000087a0: 2020 6465 6620 6b65 7950 7265 7373 4576    def keyPressEv
-000087b0: 656e 7428 7365 6c66 2c20 6576 656e 7429  ent(self, event)
-000087c0: 3a20 2023 2070 796c 696e 743a 2064 6973  :  # pylint: dis
-000087d0: 6162 6c65 3d69 6e76 616c 6964 2d6e 616d  able=invalid-nam
-000087e0: 650a 2020 2020 2020 2020 2222 2254 6869  e.        """Thi
-000087f0: 7320 6f76 6572 7269 6465 7320 5174 206b  s overrides Qt k
-00008800: 6579 2065 7665 6e74 2e22 2222 0a20 2020  ey event.""".   
-00008810: 2020 2020 206d 6f64 6966 6965 7220 3d20       modifier = 
-00008820: 6576 656e 742e 6d6f 6469 6669 6572 7328  event.modifiers(
-00008830: 290a 2020 2020 2020 2020 6966 2065 7665  ).        if eve
-00008840: 6e74 2e6b 6579 2829 203d 3d20 5174 2e4b  nt.key() == Qt.K
-00008850: 6579 5f53 2061 6e64 206d 6f64 6966 6965  ey_S and modifie
-00008860: 7220 3d3d 2051 742e 436f 6e74 726f 6c4d  r == Qt.ControlM
-00008870: 6f64 6966 6965 723a 0a20 2020 2020 2020  odifier:.       
-00008880: 2020 2020 2066 7265 7120 3d20 7365 6c66       freq = self
-00008890: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
-000088a0: 2822 7666 6f61 2229 0a20 2020 2020 2020  ("vfoa").       
-000088b0: 2020 2020 2064 7820 3d20 7365 6c66 2e63       dx = self.c
-000088c0: 616c 6c73 6967 6e2e 7465 7874 2829 0a20  allsign.text(). 
-000088d0: 2020 2020 2020 2020 2020 2069 6620 6672             if fr
-000088e0: 6571 2061 6e64 2064 783a 0a20 2020 2020  eq and dx:.     
-000088f0: 2020 2020 2020 2020 2020 2063 6d64 203d             cmd =
-00008900: 207b 7d0a 2020 2020 2020 2020 2020 2020   {}.            
-00008910: 2020 2020 636d 645b 2263 6d64 225d 203d      cmd["cmd"] =
-00008920: 2022 5350 4f54 4458 220a 2020 2020 2020   "SPOTDX".      
-00008930: 2020 2020 2020 2020 2020 636d 645b 2273            cmd["s
-00008940: 7461 7469 6f6e 225d 203d 2070 6c61 7466  tation"] = platf
-00008950: 6f72 6d2e 6e6f 6465 2829 0a20 2020 2020  orm.node().     
-00008960: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
-00008970: 6478 225d 203d 2064 780a 2020 2020 2020  dx"] = dx.      
-00008980: 2020 2020 2020 2020 2020 636d 645b 2266            cmd["f
-00008990: 7265 7122 5d20 3d20 666c 6f61 7428 696e  req"] = float(in
-000089a0: 7428 6672 6571 2920 2f20 3130 3030 290a  t(freq) / 1000).
-000089b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089c0: 7365 6c66 2e6d 756c 7469 6361 7374 5f69  self.multicast_i
-000089d0: 6e74 6572 6661 6365 2e73 656e 645f 6173  nterface.send_as
-000089e0: 5f6a 736f 6e28 636d 6429 0a20 2020 2020  _json(cmd).     
-000089f0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-00008a00: 2020 2020 2020 6966 2065 7665 6e74 2e6b        if event.k
-00008a10: 6579 2829 203d 3d20 5174 2e4b 6579 5f47  ey() == Qt.Key_G
-00008a20: 2061 6e64 206d 6f64 6966 6965 7220 3d3d   and modifier ==
-00008a30: 2051 742e 436f 6e74 726f 6c4d 6f64 6966   Qt.ControlModif
-00008a40: 6965 723a 0a20 2020 2020 2020 2020 2020  ier:.           
-00008a50: 2064 7820 3d20 7365 6c66 2e63 616c 6c73   dx = self.calls
-00008a60: 6967 6e2e 7465 7874 2829 0a20 2020 2020  ign.text().     
-00008a70: 2020 2020 2020 2069 6620 6478 3a0a 2020         if dx:.  
-00008a80: 2020 2020 2020 2020 2020 2020 2020 636d                cm
-00008a90: 6420 3d20 7b7d 0a20 2020 2020 2020 2020  d = {}.         
-00008aa0: 2020 2020 2020 2063 6d64 5b22 636d 6422         cmd["cmd"
-00008ab0: 5d20 3d20 2246 494e 4444 5822 0a20 2020  ] = "FINDDX".   
-00008ac0: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
-00008ad0: 5b22 7374 6174 696f 6e22 5d20 3d20 706c  ["station"] = pl
-00008ae0: 6174 666f 726d 2e6e 6f64 6528 290a 2020  atform.node().  
-00008af0: 2020 2020 2020 2020 2020 2020 2020 636d                cm
-00008b00: 645b 2264 7822 5d20 3d20 6478 0a20 2020  d["dx"] = dx.   
-00008b10: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00008b20: 662e 6d75 6c74 6963 6173 745f 696e 7465  f.multicast_inte
-00008b30: 7266 6163 652e 7365 6e64 5f61 735f 6a73  rface.send_as_js
-00008b40: 6f6e 2863 6d64 290a 2020 2020 2020 2020  on(cmd).        
-00008b50: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-00008b60: 2020 2069 6620 280a 2020 2020 2020 2020     if (.        
-00008b70: 2020 2020 6576 656e 742e 6b65 7928 2920      event.key() 
-00008b80: 3d3d 2051 742e 4b65 792e 4b65 795f 4573  == Qt.Key.Key_Es
-00008b90: 6361 7065 2061 6e64 206d 6f64 6966 6965  cape and modifie
-00008ba0: 7220 213d 2051 742e 436f 6e74 726f 6c4d  r != Qt.ControlM
-00008bb0: 6f64 6966 6965 720a 2020 2020 2020 2020  odifier.        
-00008bc0: 293a 2020 2320 7079 6c69 6e74 3a20 6469  ):  # pylint: di
-00008bd0: 7361 626c 653d 6e6f 2d6d 656d 6265 720a  sable=no-member.
-00008be0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00008bf0: 2e63 6c65 6172 696e 7075 7473 2829 0a20  .clearinputs(). 
-00008c00: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00008c10: 6e0a 2020 2020 2020 2020 6966 2065 7665  n.        if eve
-00008c20: 6e74 2e6b 6579 2829 203d 3d20 5174 2e4b  nt.key() == Qt.K
-00008c30: 6579 2e4b 6579 5f45 7363 6170 6520 616e  ey.Key_Escape an
-00008c40: 6420 6d6f 6469 6669 6572 203d 3d20 5174  d modifier == Qt
-00008c50: 2e43 6f6e 7472 6f6c 4d6f 6469 6669 6572  .ControlModifier
-00008c60: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00008c70: 2073 656c 662e 6377 2069 7320 6e6f 7420   self.cw is not 
-00008c80: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00008c90: 2020 2020 2020 6966 2073 656c 662e 6377        if self.cw
-00008ca0: 2e73 6572 7665 7274 7970 6520 3d3d 2031  .servertype == 1
-00008cb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00008cc0: 2020 2020 2020 7365 6c66 2e63 772e 7365        self.cw.se
-00008cd0: 6e64 6377 2822 5c78 3162 3422 290a 2020  ndcw("\x1b4").  
-00008ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008cf0: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-00008d00: 2069 6620 6576 656e 742e 6b65 7928 2920   if event.key() 
-00008d10: 3d3d 2051 742e 4b65 792e 4b65 795f 5570  == Qt.Key.Key_Up
-00008d20: 3a0a 2020 2020 2020 2020 2020 2020 636d  :.            cm
-00008d30: 6420 3d20 7b7d 0a20 2020 2020 2020 2020  d = {}.         
-00008d40: 2020 2063 6d64 5b22 636d 6422 5d20 3d20     cmd["cmd"] = 
-00008d50: 2250 5245 5653 504f 5422 0a20 2020 2020  "PREVSPOT".     
-00008d60: 2020 2020 2020 2063 6d64 5b22 7374 6174         cmd["stat
-00008d70: 696f 6e22 5d20 3d20 706c 6174 666f 726d  ion"] = platform
-00008d80: 2e6e 6f64 6528 290a 2020 2020 2020 2020  .node().        
-00008d90: 2020 2020 7365 6c66 2e6d 756c 7469 6361      self.multica
-00008da0: 7374 5f69 6e74 6572 6661 6365 2e73 656e  st_interface.sen
-00008db0: 645f 6173 5f6a 736f 6e28 636d 6429 0a20  d_as_json(cmd). 
-00008dc0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00008dd0: 6e0a 2020 2020 2020 2020 6966 2065 7665  n.        if eve
-00008de0: 6e74 2e6b 6579 2829 203d 3d20 5174 2e4b  nt.key() == Qt.K
-00008df0: 6579 2e4b 6579 5f44 6f77 6e3a 0a20 2020  ey.Key_Down:.   
-00008e00: 2020 2020 2020 2020 2063 6d64 203d 207b           cmd = {
-00008e10: 7d0a 2020 2020 2020 2020 2020 2020 636d  }.            cm
-00008e20: 645b 2263 6d64 225d 203d 2022 4e45 5854  d["cmd"] = "NEXT
-00008e30: 5350 4f54 220a 2020 2020 2020 2020 2020  SPOT".          
-00008e40: 2020 636d 645b 2273 7461 7469 6f6e 225d    cmd["station"]
-00008e50: 203d 2070 6c61 7466 6f72 6d2e 6e6f 6465   = platform.node
-00008e60: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
-00008e70: 656c 662e 6d75 6c74 6963 6173 745f 696e  elf.multicast_in
-00008e80: 7465 7266 6163 652e 7365 6e64 5f61 735f  terface.send_as_
-00008e90: 6a73 6f6e 2863 6d64 290a 2020 2020 2020  json(cmd).      
-00008ea0: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-00008eb0: 2020 2020 2069 6620 6576 656e 742e 6b65       if event.ke
-00008ec0: 7928 2920 3d3d 2051 742e 4b65 792e 4b65  y() == Qt.Key.Ke
-00008ed0: 795f 5061 6765 5570 2061 6e64 206d 6f64  y_PageUp and mod
-00008ee0: 6966 6965 7220 213d 2051 742e 436f 6e74  ifier != Qt.Cont
-00008ef0: 726f 6c4d 6f64 6966 6965 723a 0a20 2020  rolModifier:.   
-00008f00: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00008f10: 2e63 7720 6973 206e 6f74 204e 6f6e 653a  .cw is not None:
-00008f20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008f30: 2073 656c 662e 6377 2e73 7065 6564 202b   self.cw.speed +
-00008f40: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
-00008f50: 2020 2020 7365 6c66 2e63 775f 7370 6565      self.cw_spee
-00008f60: 642e 7365 7456 616c 7565 2873 656c 662e  d.setValue(self.
-00008f70: 6377 2e73 7065 6564 290a 2020 2020 2020  cw.speed).      
-00008f80: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00008f90: 662e 6377 2e73 6572 7665 7274 7970 6520  f.cw.servertype 
-00008fa0: 3d3d 2031 3a0a 2020 2020 2020 2020 2020  == 1:.          
-00008fb0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00008fc0: 772e 7365 6e64 6377 2866 225c 7831 6232  w.sendcw(f"\x1b2
-00008fd0: 7b73 656c 662e 6377 2e73 7065 6564 7d22  {self.cw.speed}"
-00008fe0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00008ff0: 2020 6966 2073 656c 662e 6377 2e73 6572    if self.cw.ser
-00009000: 7665 7274 7970 6520 3d3d 2032 3a0a 2020  vertype == 2:.  
-00009010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009020: 2020 7365 6c66 2e63 772e 7365 745f 7769    self.cw.set_wi
-00009030: 6e6b 6579 6572 5f73 7065 6564 2873 656c  nkeyer_speed(sel
-00009040: 662e 6377 5f73 7065 6564 2e76 616c 7565  f.cw_speed.value
-00009050: 2829 290a 2020 2020 2020 2020 2020 2020  ()).            
-00009060: 7265 7475 726e 0a20 2020 2020 2020 2069  return.        i
-00009070: 6620 6576 656e 742e 6b65 7928 2920 3d3d  f event.key() ==
-00009080: 2051 742e 4b65 792e 4b65 795f 5061 6765   Qt.Key.Key_Page
-00009090: 446f 776e 2061 6e64 206d 6f64 6966 6965  Down and modifie
-000090a0: 7220 213d 2051 742e 436f 6e74 726f 6c4d  r != Qt.ControlM
-000090b0: 6f64 6966 6965 723a 0a20 2020 2020 2020  odifier:.       
-000090c0: 2020 2020 2069 6620 7365 6c66 2e63 7720       if self.cw 
-000090d0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000090e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000090f0: 662e 6377 2e73 7065 6564 202d 3d20 310a  f.cw.speed -= 1.
+00007520: 225b 5067 446f 776e 5d5c 7444 6563 7265  "[PgDown]\tDecre
+00007530: 6173 6573 2074 6865 2063 7720 7365 6e64  ases the cw send
+00007540: 696e 6720 7370 6565 642e 5c6e 220a 2020  ing speed.\n".  
+00007550: 2020 2020 2020 2020 2020 225b 4172 726f            "[Arro
+00007560: 772d 5570 5d20 4a75 6d70 2074 6f20 7468  w-Up] Jump to th
+00007570: 6520 6e65 7874 2073 706f 7420 6162 6f76  e next spot abov
+00007580: 6520 7468 6520 6375 7272 656e 7420 5646  e the current VF
+00007590: 4f20 6375 7273 6f72 5c6e 220a 2020 2020  O cursor\n".    
+000075a0: 2020 2020 2020 2020 225c 7469 6e20 7468          "\tin th
+000075b0: 6520 6261 6e64 6d61 7020 7769 6e64 6f77  e bandmap window
+000075c0: 2028 4341 5420 5265 7175 6972 6564 292e   (CAT Required).
+000075d0: 5c6e 220a 2020 2020 2020 2020 2020 2020  \n".            
+000075e0: 225b 4172 726f 772d 446f 776e 5d20 4a75  "[Arrow-Down] Ju
+000075f0: 6d70 2074 6f20 7468 6520 6e65 7874 2073  mp to the next s
+00007600: 706f 7420 6265 6c6f 7720 7468 6520 6375  pot below the cu
+00007610: 7272 656e 745c 6e22 0a20 2020 2020 2020  rrent\n".       
+00007620: 2020 2020 2022 5c74 5646 4f20 6375 7273       "\tVFO curs
+00007630: 6f72 2069 6e20 7468 6520 6261 6e64 6d61  or in the bandma
+00007640: 7020 7769 6e64 6f77 2028 4341 5420 5265  p window (CAT Re
+00007650: 7175 6972 6564 292e 5c6e 220a 2020 2020  quired).\n".    
+00007660: 2020 2020 2020 2020 225b 5441 425d 5c74          "[TAB]\t
+00007670: 4d6f 7665 2063 7572 736f 7220 746f 2074  Move cursor to t
+00007680: 6865 2072 6967 6874 206f 6e65 2066 6965  he right one fie
+00007690: 6c64 2e5c 6e22 0a20 2020 2020 2020 2020  ld.\n".         
+000076a0: 2020 2022 5b53 6869 6674 2d54 6162 5d5c     "[Shift-Tab]\
+000076b0: 744d 6f76 6520 6375 7273 6f72 206c 6566  tMove cursor lef
+000076c0: 7420 4f6e 6520 6669 656c 642e 5c6e 220a  t One field.\n".
+000076d0: 2020 2020 2020 2020 2020 2020 225b 5350              "[SP
+000076e0: 4143 455d 5c74 5768 656e 2069 6e20 7468  ACE]\tWhen in th
+000076f0: 6520 6361 6c6c 7369 676e 2066 6965 6c64  e callsign field
+00007700: 2c20 7769 6c6c 206d 6f76 6520 7468 6520  , will move the 
+00007710: 696e 7075 7420 746f 2074 6865 5c6e 220a  input to the\n".
+00007720: 2020 2020 2020 2020 2020 2020 225c 7466              "\tf
+00007730: 6972 7374 2066 6965 6c64 206e 6565 6465  irst field neede
+00007740: 6420 666f 7220 7468 6520 6578 6368 616e  d for the exchan
+00007750: 6765 2e5c 6e22 0a20 2020 2020 2020 2020  ge.\n".         
+00007760: 2020 2022 5b45 6e74 6572 5d5c 7453 7562     "[Enter]\tSub
+00007770: 6d69 7473 2074 6865 2066 6965 6c64 7320  mits the fields 
+00007780: 746f 2074 6865 206c 6f67 2e5c 6e22 0a20  to the log.\n". 
+00007790: 2020 2020 2020 2020 2020 2022 5b46 312d             "[F1-
+000077a0: 4631 325d 5c74 5365 6e64 2028 4357 206f  F12]\tSend (CW o
+000077b0: 7220 566f 6963 6529 206d 6163 726f 732e  r Voice) macros.
+000077c0: 5c6e 220a 2020 2020 2020 2020 2020 2020  \n".            
+000077d0: 225b 4354 524c 2d53 5d5c 7453 706f 7420  "[CTRL-S]\tSpot 
+000077e0: 4361 6c6c 7369 676e 2074 6f20 7468 6520  Callsign to the 
+000077f0: 636c 7573 7465 722e 5c6e 220a 2020 2020  cluster.\n".    
+00007800: 2020 2020 2020 2020 225b 4354 524c 2d47          "[CTRL-G
+00007810: 5d5c 7454 756e 6520 746f 2061 2073 706f  ]\tTune to a spo
+00007820: 7420 6d61 7463 6869 6e67 2070 6172 7469  t matching parti
+00007830: 616c 2074 6578 7420 696e 2074 6865 2063  al text in the c
+00007840: 616c 6c73 6967 6e5c 6e22 0a20 2020 2020  allsign\n".     
+00007850: 2020 2020 2020 2022 5c74 656e 7472 7920         "\tentry 
+00007860: 6669 656c 6420 2843 4154 2052 6571 7569  field (CAT Requi
+00007870: 7265 6429 2e5c 6e22 0a20 2020 2020 2020  red).\n".       
+00007880: 2029 0a0a 2020 2020 6465 6620 6669 6c65   )..    def file
+00007890: 7069 636b 6572 2873 656c 662c 2061 6374  picker(self, act
+000078a0: 696f 6e3a 2073 7472 2920 2d3e 2073 7472  ion: str) -> str
+000078b0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+000078c0: 2020 2020 2020 4765 7420 6120 6669 6c65        Get a file
+000078d0: 6e61 6d65 0a20 2020 2020 2020 2061 6374  name.        act
+000078e0: 696f 6e3a 2022 6e65 7722 206f 7220 226f  ion: "new" or "o
+000078f0: 7065 6e22 0a20 2020 2020 2020 2022 2222  pen".        """
+00007900: 0a20 2020 2020 2020 206f 7074 696f 6e73  .        options
+00007910: 203d 2051 4669 6c65 4469 616c 6f67 2e4f   = QFileDialog.O
+00007920: 7074 696f 6e73 2829 0a20 2020 2020 2020  ptions().       
+00007930: 206f 7074 696f 6e73 207c 3d20 5146 696c   options |= QFil
+00007940: 6544 6961 6c6f 672e 446f 6e74 5573 654e  eDialog.DontUseN
+00007950: 6174 6976 6544 6961 6c6f 670a 2020 2020  ativeDialog.    
+00007960: 2020 2020 6f70 7469 6f6e 7320 7c3d 2051      options |= Q
+00007970: 4669 6c65 4469 616c 6f67 2e44 6f6e 7443  FileDialog.DontC
+00007980: 6f6e 6669 726d 4f76 6572 7772 6974 650a  onfirmOverwrite.
+00007990: 2020 2020 2020 2020 6966 2061 6374 696f          if actio
+000079a0: 6e20 3d3d 2022 6e65 7722 3a0a 2020 2020  n == "new":.    
+000079b0: 2020 2020 2020 2020 6669 6c65 2c20 5f20          file, _ 
+000079c0: 3d20 5146 696c 6544 6961 6c6f 672e 6765  = QFileDialog.ge
+000079d0: 7453 6176 6546 696c 654e 616d 6528 0a20  tSaveFileName(. 
+000079e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000079f0: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+00007a00: 2020 2020 2022 4368 6f6f 7365 2061 2044       "Choose a D
+00007a10: 6174 6162 6173 6522 2c0a 2020 2020 2020  atabase",.      
+00007a20: 2020 2020 2020 2020 2020 4441 5441 5f50            DATA_P
+00007a30: 4154 482c 0a20 2020 2020 2020 2020 2020  ATH,.           
+00007a40: 2020 2020 2022 4461 7461 6261 7365 2028       "Database (
+00007a50: 2a2e 6462 2922 2c0a 2020 2020 2020 2020  *.db)",.        
+00007a60: 2020 2020 2020 2020 6f70 7469 6f6e 733d          options=
+00007a70: 6f70 7469 6f6e 732c 0a20 2020 2020 2020  options,.       
+00007a80: 2020 2020 2029 0a20 2020 2020 2020 2069       ).        i
+00007a90: 6620 6163 7469 6f6e 203d 3d20 226f 7065  f action == "ope
+00007aa0: 6e22 3a0a 2020 2020 2020 2020 2020 2020  n":.            
+00007ab0: 6669 6c65 2c20 5f20 3d20 5146 696c 6544  file, _ = QFileD
+00007ac0: 6961 6c6f 672e 6765 744f 7065 6e46 696c  ialog.getOpenFil
+00007ad0: 654e 616d 6528 0a20 2020 2020 2020 2020  eName(.         
+00007ae0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00007af0: 2020 2020 2020 2020 2020 2020 2022 4368               "Ch
+00007b00: 6f6f 7365 2061 2044 6174 6162 6173 6522  oose a Database"
+00007b10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00007b20: 2020 4441 5441 5f50 4154 482c 0a20 2020    DATA_PATH,.   
+00007b30: 2020 2020 2020 2020 2020 2020 2022 4461               "Da
+00007b40: 7461 6261 7365 2028 2a2e 6462 2922 2c0a  tabase (*.db)",.
+00007b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b60: 6f70 7469 6f6e 733d 6f70 7469 6f6e 732c  options=options,
+00007b70: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00007b80: 2020 2020 2020 2072 6574 7572 6e20 6669         return fi
+00007b90: 6c65 0a0a 2020 2020 6465 6620 7265 6361  le..    def reca
+00007ba0: 6c63 756c 6174 655f 6d75 6c74 7328 7365  lculate_mults(se
+00007bb0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+00007bc0: 5265 6361 6c63 756c 6174 6520 4d75 6c74  Recalculate Mult
+00007bd0: 6970 6c69 6572 7322 2222 0a20 2020 2020  ipliers""".     
+00007be0: 2020 2073 656c 662e 636f 6e74 6573 742e     self.contest.
+00007bf0: 7265 6361 6c63 756c 6174 655f 6d75 6c74  recalculate_mult
+00007c00: 7328 7365 6c66 290a 2020 2020 2020 2020  s(self).        
+00007c10: 7365 6c66 2e63 6c65 6172 696e 7075 7473  self.clearinputs
+00007c20: 2829 0a0a 2020 2020 6465 6620 6c61 756e  ()..    def laun
+00007c30: 6368 5f6c 6f67 5f77 696e 646f 7728 7365  ch_log_window(se
+00007c40: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+00007c50: 6c61 756e 6368 2074 6865 204c 6f67 2057  launch the Log W
+00007c60: 696e 646f 7722 2222 0a20 2020 2020 2020  indow""".       
+00007c70: 2069 6620 6e6f 7420 6368 6563 6b5f 7072   if not check_pr
+00007c80: 6f63 6573 7328 226c 6f67 7769 6e64 6f77  ocess("logwindow
+00007c90: 2e70 7922 293a 0a20 2020 2020 2020 2020  .py"):.         
+00007ca0: 2020 205f 203d 2073 7562 7072 6f63 6573     _ = subproces
+00007cb0: 732e 506f 7065 6e28 5b73 7973 2e65 7865  s.Popen([sys.exe
+00007cc0: 6375 7461 626c 652c 2057 4f52 4b49 4e47  cutable, WORKING
+00007cd0: 5f50 4154 4820 2b20 222f 6c6f 6777 696e  _PATH + "/logwin
+00007ce0: 646f 772e 7079 225d 290a 0a20 2020 2064  dow.py"])..    d
+00007cf0: 6566 206c 6175 6e63 685f 6261 6e64 6d61  ef launch_bandma
+00007d00: 705f 7769 6e64 6f77 2873 656c 6629 3a0a  p_window(self):.
+00007d10: 2020 2020 2020 2020 2222 226c 6175 6e63          """launc
+00007d20: 6820 7468 6520 4c6f 6720 5769 6e64 6f77  h the Log Window
+00007d30: 2222 220a 2020 2020 2020 2020 6966 206e  """.        if n
+00007d40: 6f74 2063 6865 636b 5f70 726f 6365 7373  ot check_process
+00007d50: 2822 6261 6e64 6d61 702e 7079 2229 3a0a  ("bandmap.py"):.
+00007d60: 2020 2020 2020 2020 2020 2020 5f20 3d20              _ = 
+00007d70: 7375 6270 726f 6365 7373 2e50 6f70 656e  subprocess.Popen
+00007d80: 285b 7379 732e 6578 6563 7574 6162 6c65  ([sys.executable
+00007d90: 2c20 574f 524b 494e 475f 5041 5448 202b  , WORKING_PATH +
+00007da0: 2022 2f62 616e 646d 6170 2e70 7922 5d29   "/bandmap.py"])
+00007db0: 0a0a 2020 2020 6465 6620 6c61 756e 6368  ..    def launch
+00007dc0: 5f63 6865 636b 5f77 696e 646f 7728 7365  _check_window(se
+00007dd0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+00007de0: 6c61 756e 6368 2074 6865 204c 6f67 2057  launch the Log W
+00007df0: 696e 646f 7722 2222 0a20 2020 2020 2020  indow""".       
+00007e00: 2069 6620 6e6f 7420 6368 6563 6b5f 7072   if not check_pr
+00007e10: 6f63 6573 7328 2263 6865 636b 7769 6e64  ocess("checkwind
+00007e20: 6f77 2e70 7922 293a 0a20 2020 2020 2020  ow.py"):.       
+00007e30: 2020 2020 205f 203d 2073 7562 7072 6f63       _ = subproc
+00007e40: 6573 732e 506f 7065 6e28 5b73 7973 2e65  ess.Popen([sys.e
+00007e50: 7865 6375 7461 626c 652c 2057 4f52 4b49  xecutable, WORKI
+00007e60: 4e47 5f50 4154 4820 2b20 222f 6368 6563  NG_PATH + "/chec
+00007e70: 6b77 696e 646f 772e 7079 225d 290a 0a20  kwindow.py"]).. 
+00007e80: 2020 2064 6566 206c 6175 6e63 685f 7666     def launch_vf
+00007e90: 6f28 7365 6c66 293a 0a20 2020 2020 2020  o(self):.       
+00007ea0: 2022 2222 6c61 756e 6368 2074 6865 204c   """launch the L
+00007eb0: 6f67 2057 696e 646f 7722 2222 0a20 2020  og Window""".   
+00007ec0: 2020 2020 2069 6620 6e6f 7420 6368 6563       if not chec
+00007ed0: 6b5f 7072 6f63 6573 7328 2276 666f 2e70  k_process("vfo.p
+00007ee0: 7922 293a 0a20 2020 2020 2020 2020 2020  y"):.           
+00007ef0: 205f 203d 2073 7562 7072 6f63 6573 732e   _ = subprocess.
+00007f00: 506f 7065 6e28 5b73 7973 2e65 7865 6375  Popen([sys.execu
+00007f10: 7461 626c 652c 2057 4f52 4b49 4e47 5f50  table, WORKING_P
+00007f20: 4154 4820 2b20 222f 7666 6f2e 7079 225d  ATH + "/vfo.py"]
+00007f30: 290a 0a20 2020 2064 6566 2063 6c65 6172  )..    def clear
+00007f40: 5f62 616e 645f 696e 6469 6361 746f 7273  _band_indicators
+00007f50: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00007f60: 2222 2243 6c65 6172 2074 6865 2069 6e64  """Clear the ind
+00007f70: 6963 6174 6f72 7322 2222 0a20 2020 2020  icators""".     
+00007f80: 2020 2066 6f72 205f 2c20 696e 6469 6361     for _, indica
+00007f90: 746f 7273 2069 6e20 7365 6c66 2e61 6c6c  tors in self.all
+00007fa0: 5f6d 6f64 655f 696e 6469 6361 746f 7273  _mode_indicators
+00007fb0: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
+00007fc0: 2020 2020 2020 666f 7220 5f2c 2069 6e64        for _, ind
+00007fd0: 6963 6174 6f72 2069 6e20 696e 6469 6361  icator in indica
+00007fe0: 746f 7273 2e69 7465 6d73 2829 3a0a 2020  tors.items():.  
+00007ff0: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00008000: 6469 6361 746f 722e 7365 7446 7261 6d65  dicator.setFrame
+00008010: 5368 6170 6528 5174 5769 6467 6574 732e  Shape(QtWidgets.
+00008020: 5146 7261 6d65 2e4e 6f46 7261 6d65 290a  QFrame.NoFrame).
+00008030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008040: 696e 6469 6361 746f 722e 7365 7453 7479  indicator.setSty
+00008050: 6c65 5368 6565 7428 2266 6f6e 742d 6661  leSheet("font-fa
+00008060: 6d69 6c79 3a20 4a65 7442 7261 696e 7320  mily: JetBrains 
+00008070: 4d6f 6e6f 3b22 290a 0a20 2020 2064 6566  Mono;")..    def
+00008080: 2073 6574 5f62 616e 645f 696e 6469 6361   set_band_indica
+00008090: 746f 7228 7365 6c66 2c20 6261 6e64 3a20  tor(self, band: 
+000080a0: 7374 7229 202d 3e20 4e6f 6e65 3a0a 2020  str) -> None:.  
+000080b0: 2020 2020 2020 2222 2253 6574 2074 6865        """Set the
+000080c0: 2062 616e 6420 696e 6469 6361 746f 7222   band indicator"
+000080d0: 2222 0a20 2020 2020 2020 2023 206c 6f67  "".        # log
+000080e0: 6765 722e 6465 6275 6728 2225 7322 2c20  ger.debug("%s", 
+000080f0: 6622 6261 6e64 3a7b 6261 6e64 7d20 6d6f  f"band:{band} mo
+00008100: 6465 3a20 7b73 656c 662e 6375 7272 656e  de: {self.curren
+00008110: 745f 6d6f 6465 7d22 290a 2020 2020 2020  t_mode}").      
+00008120: 2020 6966 2062 616e 6420 616e 6420 7365    if band and se
+00008130: 6c66 2e63 7572 7265 6e74 5f6d 6f64 653a  lf.current_mode:
+00008140: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00008150: 662e 636c 6561 725f 6261 6e64 5f69 6e64  f.clear_band_ind
+00008160: 6963 6174 6f72 7328 290a 2020 2020 2020  icators().      
+00008170: 2020 2020 2020 696e 6469 6361 746f 7220        indicator 
+00008180: 3d20 7365 6c66 2e61 6c6c 5f6d 6f64 655f  = self.all_mode_
+00008190: 696e 6469 6361 746f 7273 5b73 656c 662e  indicators[self.
+000081a0: 6375 7272 656e 745f 6d6f 6465 5d2e 6765  current_mode].ge
+000081b0: 7428 6261 6e64 2c20 4e6f 6e65 290a 2020  t(band, None).  
+000081c0: 2020 2020 2020 2020 2020 6966 2069 6e64            if ind
+000081d0: 6963 6174 6f72 3a0a 2020 2020 2020 2020  icator:.        
+000081e0: 2020 2020 2020 2020 696e 6469 6361 746f          indicato
+000081f0: 722e 7365 7446 7261 6d65 5368 6170 6528  r.setFrameShape(
+00008200: 5174 5769 6467 6574 732e 5146 7261 6d65  QtWidgets.QFrame
+00008210: 2e42 6f78 290a 2020 2020 2020 2020 2020  .Box).          
+00008220: 2020 2020 2020 696e 6469 6361 746f 722e        indicator.
+00008230: 7365 7453 7479 6c65 5368 6565 7428 2266  setStyleSheet("f
+00008240: 6f6e 742d 6661 6d69 6c79 3a20 4a65 7442  ont-family: JetB
+00008250: 7261 696e 7320 4d6f 6e6f 3b20 636f 6c6f  rains Mono; colo
+00008260: 723a 2067 7265 656e 3b22 290a 0a20 2020  r: green;")..   
+00008270: 2064 6566 2063 6c6f 7365 4576 656e 7428   def closeEvent(
+00008280: 7365 6c66 2c20 5f65 7665 6e74 293a 0a20  self, _event):. 
+00008290: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000082a0: 2020 2057 7269 7465 2077 696e 646f 7720     Write window 
+000082b0: 7369 7a65 2061 6e64 2070 6f73 6974 696f  size and positio
+000082c0: 6e20 746f 2063 6f6e 6669 6720 6669 6c65  n to config file
+000082d0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000082e0: 2020 2020 2063 6d64 203d 207b 7d0a 2020       cmd = {}.  
+000082f0: 2020 2020 2020 636d 645b 2263 6d64 225d        cmd["cmd"]
+00008300: 203d 2022 4841 4c54 220a 2020 2020 2020   = "HALT".      
+00008310: 2020 636d 645b 2273 7461 7469 6f6e 225d    cmd["station"]
+00008320: 203d 2070 6c61 7466 6f72 6d2e 6e6f 6465   = platform.node
+00008330: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+00008340: 6d75 6c74 6963 6173 745f 696e 7465 7266  multicast_interf
+00008350: 6163 652e 7365 6e64 5f61 735f 6a73 6f6e  ace.send_as_json
+00008360: 2863 6d64 290a 2020 2020 2020 2020 7365  (cmd).        se
+00008370: 6c66 2e70 7265 665b 2277 696e 646f 775f  lf.pref["window_
+00008380: 7769 6474 6822 5d20 3d20 7365 6c66 2e73  width"] = self.s
+00008390: 697a 6528 292e 7769 6474 6828 290a 2020  ize().width().  
+000083a0: 2020 2020 2020 7365 6c66 2e70 7265 665b        self.pref[
+000083b0: 2277 696e 646f 775f 6865 6967 6874 225d  "window_height"]
+000083c0: 203d 2073 656c 662e 7369 7a65 2829 2e68   = self.size().h
+000083d0: 6569 6768 7428 290a 2020 2020 2020 2020  eight().        
+000083e0: 7365 6c66 2e70 7265 665b 2277 696e 646f  self.pref["windo
+000083f0: 775f 7822 5d20 3d20 7365 6c66 2e70 6f73  w_x"] = self.pos
+00008400: 2829 2e78 2829 0a20 2020 2020 2020 2073  ().x().        s
+00008410: 656c 662e 7072 6566 5b22 7769 6e64 6f77  elf.pref["window
+00008420: 5f79 225d 203d 2073 656c 662e 706f 7328  _y"] = self.pos(
+00008430: 292e 7928 290a 2020 2020 2020 2020 7365  ).y().        se
+00008440: 6c66 2e77 7269 7465 5f70 7265 6665 7265  lf.write_prefere
+00008450: 6e63 6528 290a 0a20 2020 2064 6566 2063  nce()..    def c
+00008460: 7479 5f6c 6f6f 6b75 7028 7365 6c66 2c20  ty_lookup(self, 
+00008470: 6361 6c6c 7369 676e 3a20 7374 7229 3a0a  callsign: str):.
+00008480: 2020 2020 2020 2020 2222 224c 6f6f 6b75          """Looku
+00008490: 7020 6361 6c6c 7369 676e 2069 6e20 6374  p callsign in ct
+000084a0: 792e 6461 7420 6669 6c65 2e0a 0a20 2020  y.dat file...   
+000084b0: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+000084c0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+000084d0: 2d2d 0a20 2020 2020 2020 2063 616c 6c73  --.        calls
+000084e0: 6967 6e20 3a20 7374 720a 0a20 2020 2020  ign : str..     
+000084f0: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
+00008500: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+00008510: 2020 2072 6574 7572 6e20 3a20 6c69 7374     return : list
+00008520: 206f 6620 6469 6374 730a 2020 2020 2020   of dicts.      
+00008530: 2020 2222 220a 2020 2020 2020 2020 6361    """.        ca
+00008540: 6c6c 7369 676e 203d 2063 616c 6c73 6967  llsign = callsig
+00008550: 6e2e 7570 7065 7228 290a 2020 2020 2020  n.upper().      
+00008560: 2020 666f 7220 636f 756e 7420 696e 2072    for count in r
+00008570: 6576 6572 7365 6428 7261 6e67 6528 6c65  eversed(range(le
+00008580: 6e28 6361 6c6c 7369 676e 2929 293a 0a20  n(callsign))):. 
+00008590: 2020 2020 2020 2020 2020 2073 6561 7263             searc
+000085a0: 6869 7465 6d20 3d20 6361 6c6c 7369 676e  hitem = callsign
+000085b0: 5b3a 2063 6f75 6e74 202b 2031 5d0a 2020  [: count + 1].  
+000085c0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000085d0: 203d 207b 6b65 793a 2076 616c 2066 6f72   = {key: val for
+000085e0: 206b 6579 2c20 7661 6c20 696e 2043 5459   key, val in CTY
+000085f0: 4649 4c45 2e69 7465 6d73 2829 2069 6620  FILE.items() if 
+00008600: 6b65 7920 3d3d 2073 6561 7263 6869 7465  key == searchite
+00008610: 6d7d 0a20 2020 2020 2020 2020 2020 2069  m}.            i
+00008620: 6620 6e6f 7420 7265 7375 6c74 3a0a 2020  f not result:.  
+00008630: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00008640: 6e74 696e 7565 0a20 2020 2020 2020 2020  ntinue.         
+00008650: 2020 2069 6620 7265 7375 6c74 2e67 6574     if result.get
+00008660: 2873 6561 7263 6869 7465 6d29 2e67 6574  (searchitem).get
+00008670: 2822 6578 6163 745f 6d61 7463 6822 293a  ("exact_match"):
+00008680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008690: 2069 6620 7365 6172 6368 6974 656d 203d   if searchitem =
+000086a0: 3d20 6361 6c6c 7369 676e 3a0a 2020 2020  = callsign:.    
+000086b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000086c0: 7265 7475 726e 2072 6573 756c 740a 2020  return result.  
+000086d0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+000086e0: 6e74 696e 7565 0a20 2020 2020 2020 2020  ntinue.         
+000086f0: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+00008700: 0a0a 2020 2020 6465 6620 6377 7370 6565  ..    def cwspee
+00008710: 645f 7370 696e 626f 785f 6368 616e 6765  d_spinbox_change
+00008720: 6428 7365 6c66 293a 0a20 2020 2020 2020  d(self):.       
+00008730: 2022 2222 7472 6967 6765 7265 6420 7768   """triggered wh
+00008740: 656e 2076 616c 7565 206f 6620 4357 2073  en value of CW s
+00008750: 7065 6564 2069 6e20 7468 6520 7370 696e  peed in the spin
+00008760: 626f 7820 6368 616e 6765 732e 2222 220a  box changes.""".
+00008770: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00008780: 6377 2069 7320 4e6f 6e65 3a0a 2020 2020  cw is None:.    
+00008790: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+000087a0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+000087b0: 772e 7365 7276 6572 7479 7065 203d 3d20  w.servertype == 
+000087c0: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
+000087d0: 656c 662e 6377 2e73 7065 6564 203d 2073  elf.cw.speed = s
+000087e0: 656c 662e 6377 5f73 7065 6564 2e76 616c  elf.cw_speed.val
+000087f0: 7565 2829 0a20 2020 2020 2020 2020 2020  ue().           
+00008800: 2073 656c 662e 6377 2e73 656e 6463 7728   self.cw.sendcw(
+00008810: 6622 5c78 3162 327b 7365 6c66 2e63 772e  f"\x1b2{self.cw.
+00008820: 7370 6565 647d 2229 0a20 2020 2020 2020  speed}").       
+00008830: 2069 6620 7365 6c66 2e63 772e 7365 7276   if self.cw.serv
+00008840: 6572 7479 7065 203d 3d20 323a 0a20 2020  ertype == 2:.   
+00008850: 2020 2020 2020 2020 2073 656c 662e 6377           self.cw
+00008860: 2e73 6574 5f77 696e 6b65 7965 725f 7370  .set_winkeyer_sp
+00008870: 6565 6428 7365 6c66 2e63 775f 7370 6565  eed(self.cw_spee
+00008880: 642e 7661 6c75 6528 2929 0a0a 2020 2020  d.value())..    
+00008890: 6465 6620 6b65 7950 7265 7373 4576 656e  def keyPressEven
+000088a0: 7428 7365 6c66 2c20 6576 656e 7429 3a20  t(self, event): 
+000088b0: 2023 2070 796c 696e 743a 2064 6973 6162   # pylint: disab
+000088c0: 6c65 3d69 6e76 616c 6964 2d6e 616d 650a  le=invalid-name.
+000088d0: 2020 2020 2020 2020 2222 2254 6869 7320          """This 
+000088e0: 6f76 6572 7269 6465 7320 5174 206b 6579  overrides Qt key
+000088f0: 2065 7665 6e74 2e22 2222 0a20 2020 2020   event.""".     
+00008900: 2020 206d 6f64 6966 6965 7220 3d20 6576     modifier = ev
+00008910: 656e 742e 6d6f 6469 6669 6572 7328 290a  ent.modifiers().
+00008920: 2020 2020 2020 2020 6966 2065 7665 6e74          if event
+00008930: 2e6b 6579 2829 203d 3d20 5174 2e4b 6579  .key() == Qt.Key
+00008940: 5f53 2061 6e64 206d 6f64 6966 6965 7220  _S and modifier 
+00008950: 3d3d 2051 742e 436f 6e74 726f 6c4d 6f64  == Qt.ControlMod
+00008960: 6966 6965 723a 0a20 2020 2020 2020 2020  ifier:.         
+00008970: 2020 2066 7265 7120 3d20 7365 6c66 2e72     freq = self.r
+00008980: 6164 696f 5f73 7461 7465 2e67 6574 2822  adio_state.get("
+00008990: 7666 6f61 2229 0a20 2020 2020 2020 2020  vfoa").         
+000089a0: 2020 2064 7820 3d20 7365 6c66 2e63 616c     dx = self.cal
+000089b0: 6c73 6967 6e2e 7465 7874 2829 0a20 2020  lsign.text().   
+000089c0: 2020 2020 2020 2020 2069 6620 6672 6571           if freq
+000089d0: 2061 6e64 2064 783a 0a20 2020 2020 2020   and dx:.       
+000089e0: 2020 2020 2020 2020 2063 6d64 203d 207b           cmd = {
+000089f0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00008a00: 2020 636d 645b 2263 6d64 225d 203d 2022    cmd["cmd"] = "
+00008a10: 5350 4f54 4458 220a 2020 2020 2020 2020  SPOTDX".        
+00008a20: 2020 2020 2020 2020 636d 645b 2273 7461          cmd["sta
+00008a30: 7469 6f6e 225d 203d 2070 6c61 7466 6f72  tion"] = platfor
+00008a40: 6d2e 6e6f 6465 2829 0a20 2020 2020 2020  m.node().       
+00008a50: 2020 2020 2020 2020 2063 6d64 5b22 6478           cmd["dx
+00008a60: 225d 203d 2064 780a 2020 2020 2020 2020  "] = dx.        
+00008a70: 2020 2020 2020 2020 636d 645b 2266 7265          cmd["fre
+00008a80: 7122 5d20 3d20 666c 6f61 7428 696e 7428  q"] = float(int(
+00008a90: 6672 6571 2920 2f20 3130 3030 290a 2020  freq) / 1000).  
+00008aa0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00008ab0: 6c66 2e6d 756c 7469 6361 7374 5f69 6e74  lf.multicast_int
+00008ac0: 6572 6661 6365 2e73 656e 645f 6173 5f6a  erface.send_as_j
+00008ad0: 736f 6e28 636d 6429 0a20 2020 2020 2020  son(cmd).       
+00008ae0: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+00008af0: 2020 2020 6966 2065 7665 6e74 2e6b 6579      if event.key
+00008b00: 2829 203d 3d20 5174 2e4b 6579 5f47 2061  () == Qt.Key_G a
+00008b10: 6e64 206d 6f64 6966 6965 7220 3d3d 2051  nd modifier == Q
+00008b20: 742e 436f 6e74 726f 6c4d 6f64 6966 6965  t.ControlModifie
+00008b30: 723a 0a20 2020 2020 2020 2020 2020 2064  r:.            d
+00008b40: 7820 3d20 7365 6c66 2e63 616c 6c73 6967  x = self.callsig
+00008b50: 6e2e 7465 7874 2829 0a20 2020 2020 2020  n.text().       
+00008b60: 2020 2020 2069 6620 6478 3a0a 2020 2020       if dx:.    
+00008b70: 2020 2020 2020 2020 2020 2020 636d 6420              cmd 
+00008b80: 3d20 7b7d 0a20 2020 2020 2020 2020 2020  = {}.           
+00008b90: 2020 2020 2063 6d64 5b22 636d 6422 5d20       cmd["cmd"] 
+00008ba0: 3d20 2246 494e 4444 5822 0a20 2020 2020  = "FINDDX".     
+00008bb0: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
+00008bc0: 7374 6174 696f 6e22 5d20 3d20 706c 6174  station"] = plat
+00008bd0: 666f 726d 2e6e 6f64 6528 290a 2020 2020  form.node().    
+00008be0: 2020 2020 2020 2020 2020 2020 636d 645b              cmd[
+00008bf0: 2264 7822 5d20 3d20 6478 0a20 2020 2020  "dx"] = dx.     
+00008c00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00008c10: 6d75 6c74 6963 6173 745f 696e 7465 7266  multicast_interf
+00008c20: 6163 652e 7365 6e64 5f61 735f 6a73 6f6e  ace.send_as_json
+00008c30: 2863 6d64 290a 2020 2020 2020 2020 2020  (cmd).          
+00008c40: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+00008c50: 2069 6620 280a 2020 2020 2020 2020 2020   if (.          
+00008c60: 2020 6576 656e 742e 6b65 7928 2920 3d3d    event.key() ==
+00008c70: 2051 742e 4b65 792e 4b65 795f 4573 6361   Qt.Key.Key_Esca
+00008c80: 7065 2061 6e64 206d 6f64 6966 6965 7220  pe and modifier 
+00008c90: 213d 2051 742e 436f 6e74 726f 6c4d 6f64  != Qt.ControlMod
+00008ca0: 6966 6965 720a 2020 2020 2020 2020 293a  ifier.        ):
+00008cb0: 2020 2320 7079 6c69 6e74 3a20 6469 7361    # pylint: disa
+00008cc0: 626c 653d 6e6f 2d6d 656d 6265 720a 2020  ble=no-member.  
+00008cd0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00008ce0: 6c65 6172 696e 7075 7473 2829 0a20 2020  learinputs().   
+00008cf0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00008d00: 2020 2020 2020 2020 6966 2065 7665 6e74          if event
+00008d10: 2e6b 6579 2829 203d 3d20 5174 2e4b 6579  .key() == Qt.Key
+00008d20: 2e4b 6579 5f45 7363 6170 6520 616e 6420  .Key_Escape and 
+00008d30: 6d6f 6469 6669 6572 203d 3d20 5174 2e43  modifier == Qt.C
+00008d40: 6f6e 7472 6f6c 4d6f 6469 6669 6572 3a0a  ontrolModifier:.
+00008d50: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00008d60: 656c 662e 6377 2069 7320 6e6f 7420 4e6f  elf.cw is not No
+00008d70: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00008d80: 2020 2020 6966 2073 656c 662e 6377 2e73      if self.cw.s
+00008d90: 6572 7665 7274 7970 6520 3d3d 2031 3a0a  ervertype == 1:.
+00008da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008db0: 2020 2020 7365 6c66 2e63 772e 7365 6e64      self.cw.send
+00008dc0: 6377 2822 5c78 3162 3422 290a 2020 2020  cw("\x1b4").    
+00008dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008de0: 7265 7475 726e 0a20 2020 2020 2020 2069  return.        i
+00008df0: 6620 6576 656e 742e 6b65 7928 2920 3d3d  f event.key() ==
+00008e00: 2051 742e 4b65 792e 4b65 795f 5570 3a0a   Qt.Key.Key_Up:.
+00008e10: 2020 2020 2020 2020 2020 2020 636d 6420              cmd 
+00008e20: 3d20 7b7d 0a20 2020 2020 2020 2020 2020  = {}.           
+00008e30: 2063 6d64 5b22 636d 6422 5d20 3d20 2250   cmd["cmd"] = "P
+00008e40: 5245 5653 504f 5422 0a20 2020 2020 2020  REVSPOT".       
+00008e50: 2020 2020 2063 6d64 5b22 7374 6174 696f       cmd["statio
+00008e60: 6e22 5d20 3d20 706c 6174 666f 726d 2e6e  n"] = platform.n
+00008e70: 6f64 6528 290a 2020 2020 2020 2020 2020  ode().          
+00008e80: 2020 7365 6c66 2e6d 756c 7469 6361 7374    self.multicast
+00008e90: 5f69 6e74 6572 6661 6365 2e73 656e 645f  _interface.send_
+00008ea0: 6173 5f6a 736f 6e28 636d 6429 0a20 2020  as_json(cmd).   
+00008eb0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00008ec0: 2020 2020 2020 2020 6966 2065 7665 6e74          if event
+00008ed0: 2e6b 6579 2829 203d 3d20 5174 2e4b 6579  .key() == Qt.Key
+00008ee0: 2e4b 6579 5f44 6f77 6e3a 0a20 2020 2020  .Key_Down:.     
+00008ef0: 2020 2020 2020 2063 6d64 203d 207b 7d0a         cmd = {}.
+00008f00: 2020 2020 2020 2020 2020 2020 636d 645b              cmd[
+00008f10: 2263 6d64 225d 203d 2022 4e45 5854 5350  "cmd"] = "NEXTSP
+00008f20: 4f54 220a 2020 2020 2020 2020 2020 2020  OT".            
+00008f30: 636d 645b 2273 7461 7469 6f6e 225d 203d  cmd["station"] =
+00008f40: 2070 6c61 7466 6f72 6d2e 6e6f 6465 2829   platform.node()
+00008f50: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00008f60: 662e 6d75 6c74 6963 6173 745f 696e 7465  f.multicast_inte
+00008f70: 7266 6163 652e 7365 6e64 5f61 735f 6a73  rface.send_as_js
+00008f80: 6f6e 2863 6d64 290a 2020 2020 2020 2020  on(cmd).        
+00008f90: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+00008fa0: 2020 2069 6620 6576 656e 742e 6b65 7928     if event.key(
+00008fb0: 2920 3d3d 2051 742e 4b65 792e 4b65 795f  ) == Qt.Key.Key_
+00008fc0: 5061 6765 5570 2061 6e64 206d 6f64 6966  PageUp and modif
+00008fd0: 6965 7220 213d 2051 742e 436f 6e74 726f  ier != Qt.Contro
+00008fe0: 6c4d 6f64 6966 6965 723a 0a20 2020 2020  lModifier:.     
+00008ff0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+00009000: 7720 6973 206e 6f74 204e 6f6e 653a 0a20  w is not None:. 
+00009010: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00009020: 656c 662e 6377 2e73 7065 6564 202b 3d20  elf.cw.speed += 
+00009030: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
+00009040: 2020 7365 6c66 2e63 775f 7370 6565 642e    self.cw_speed.
+00009050: 7365 7456 616c 7565 2873 656c 662e 6377  setValue(self.cw
+00009060: 2e73 7065 6564 290a 2020 2020 2020 2020  .speed).        
+00009070: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00009080: 6377 2e73 6572 7665 7274 7970 6520 3d3d  cw.servertype ==
+00009090: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
+000090a0: 2020 2020 2020 2020 7365 6c66 2e63 772e          self.cw.
+000090b0: 7365 6e64 6377 2866 225c 7831 6232 7b73  sendcw(f"\x1b2{s
+000090c0: 656c 662e 6377 2e73 7065 6564 7d22 290a  elf.cw.speed}").
+000090d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000090e0: 6966 2073 656c 662e 6377 2e73 6572 7665  if self.cw.serve
+000090f0: 7274 7970 6520 3d3d 2032 3a0a 2020 2020  rtype == 2:.    
 00009100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009110: 7365 6c66 2e63 775f 7370 6565 642e 7365  self.cw_speed.se
-00009120: 7456 616c 7565 2873 656c 662e 6377 2e73  tValue(self.cw.s
-00009130: 7065 6564 290a 2020 2020 2020 2020 2020  peed).          
-00009140: 2020 2020 2020 6966 2073 656c 662e 6377        if self.cw
-00009150: 2e73 6572 7665 7274 7970 6520 3d3d 2031  .servertype == 1
-00009160: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00009170: 2020 2020 2020 7365 6c66 2e63 772e 7365        self.cw.se
-00009180: 6e64 6377 2866 225c 7831 6232 7b73 656c  ndcw(f"\x1b2{sel
-00009190: 662e 6377 2e73 7065 6564 7d22 290a 2020  f.cw.speed}").  
-000091a0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000091b0: 2073 656c 662e 6377 2e73 6572 7665 7274   self.cw.servert
-000091c0: 7970 6520 3d3d 2032 3a0a 2020 2020 2020  ype == 2:.      
-000091d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000091e0: 6c66 2e63 772e 7365 745f 7769 6e6b 6579  lf.cw.set_winkey
-000091f0: 6572 5f73 7065 6564 2873 656c 662e 6377  er_speed(self.cw
-00009200: 5f73 7065 6564 2e76 616c 7565 2829 290a  _speed.value()).
-00009210: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00009220: 726e 0a20 2020 2020 2020 2023 2069 6620  rn.        # if 
-00009230: 6576 656e 742e 6b65 7928 2920 3d3d 2051  event.key() == Q
-00009240: 742e 4b65 792e 4b65 795f 456e 7465 723a  t.Key.Key_Enter:
-00009250: 0a20 2020 2020 2020 2023 2020 2020 2073  .        #     s
-00009260: 656c 662e 7361 7665 5f63 6f6e 7461 6374  elf.save_contact
-00009270: 2829 0a20 2020 2020 2020 2069 6620 6576  ().        if ev
-00009280: 656e 742e 6b65 7928 2920 3d3d 2051 742e  ent.key() == Qt.
-00009290: 4b65 792e 4b65 795f 5461 6220 6f72 2065  Key.Key_Tab or e
-000092a0: 7665 6e74 2e6b 6579 2829 203d 3d20 5174  vent.key() == Qt
-000092b0: 2e4b 6579 2e4b 6579 5f42 6163 6b74 6162  .Key.Key_Backtab
-000092c0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-000092d0: 2073 656c 662e 7365 6e74 2e68 6173 466f   self.sent.hasFo
-000092e0: 6375 7328 293a 0a20 2020 2020 2020 2020  cus():.         
-000092f0: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-00009300: 6275 6728 2246 726f 6d20 7365 6e74 2229  bug("From sent")
-00009310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009320: 2069 6620 6d6f 6469 6669 6572 203d 3d20   if modifier == 
-00009330: 5174 2e53 6869 6674 4d6f 6469 6669 6572  Qt.ShiftModifier
-00009340: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00009350: 2020 2020 2020 7072 6576 5f74 6162 203d        prev_tab =
-00009360: 2073 656c 662e 7461 625f 7072 6576 2e67   self.tab_prev.g
-00009370: 6574 2873 656c 662e 7365 6e74 290a 2020  et(self.sent).  
-00009380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009390: 2020 7072 6576 5f74 6162 2e73 6574 466f    prev_tab.setFo
-000093a0: 6375 7328 290a 2020 2020 2020 2020 2020  cus().          
-000093b0: 2020 2020 2020 2020 2020 7072 6576 5f74            prev_t
-000093c0: 6162 2e64 6573 656c 6563 7428 290a 2020  ab.deselect().  
-000093d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000093e0: 2020 7072 6576 5f74 6162 2e65 6e64 2846    prev_tab.end(F
-000093f0: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
-00009400: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00009410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009420: 6e65 7874 5f74 6162 203d 2073 656c 662e  next_tab = self.
-00009430: 7461 625f 6e65 7874 2e67 6574 2873 656c  tab_next.get(sel
-00009440: 662e 7365 6e74 290a 2020 2020 2020 2020  f.sent).        
-00009450: 2020 2020 2020 2020 2020 2020 6e65 7874              next
-00009460: 5f74 6162 2e73 6574 466f 6375 7328 290a  _tab.setFocus().
+00009110: 7365 6c66 2e63 772e 7365 745f 7769 6e6b  self.cw.set_wink
+00009120: 6579 6572 5f73 7065 6564 2873 656c 662e  eyer_speed(self.
+00009130: 6377 5f73 7065 6564 2e76 616c 7565 2829  cw_speed.value()
+00009140: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00009150: 7475 726e 0a20 2020 2020 2020 2069 6620  turn.        if 
+00009160: 6576 656e 742e 6b65 7928 2920 3d3d 2051  event.key() == Q
+00009170: 742e 4b65 792e 4b65 795f 5061 6765 446f  t.Key.Key_PageDo
+00009180: 776e 2061 6e64 206d 6f64 6966 6965 7220  wn and modifier 
+00009190: 213d 2051 742e 436f 6e74 726f 6c4d 6f64  != Qt.ControlMod
+000091a0: 6966 6965 723a 0a20 2020 2020 2020 2020  ifier:.         
+000091b0: 2020 2069 6620 7365 6c66 2e63 7720 6973     if self.cw is
+000091c0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000091d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000091e0: 6377 2e73 7065 6564 202d 3d20 310a 2020  cw.speed -= 1.  
+000091f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00009200: 6c66 2e63 775f 7370 6565 642e 7365 7456  lf.cw_speed.setV
+00009210: 616c 7565 2873 656c 662e 6377 2e73 7065  alue(self.cw.spe
+00009220: 6564 290a 2020 2020 2020 2020 2020 2020  ed).            
+00009230: 2020 2020 6966 2073 656c 662e 6377 2e73      if self.cw.s
+00009240: 6572 7665 7274 7970 6520 3d3d 2031 3a0a  ervertype == 1:.
+00009250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009260: 2020 2020 7365 6c66 2e63 772e 7365 6e64      self.cw.send
+00009270: 6377 2866 225c 7831 6232 7b73 656c 662e  cw(f"\x1b2{self.
+00009280: 6377 2e73 7065 6564 7d22 290a 2020 2020  cw.speed}").    
+00009290: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+000092a0: 656c 662e 6377 2e73 6572 7665 7274 7970  elf.cw.servertyp
+000092b0: 6520 3d3d 2032 3a0a 2020 2020 2020 2020  e == 2:.        
+000092c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000092d0: 2e63 772e 7365 745f 7769 6e6b 6579 6572  .cw.set_winkeyer
+000092e0: 5f73 7065 6564 2873 656c 662e 6377 5f73  _speed(self.cw_s
+000092f0: 7065 6564 2e76 616c 7565 2829 290a 2020  peed.value()).  
+00009300: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00009310: 0a20 2020 2020 2020 2023 2069 6620 6576  .        # if ev
+00009320: 656e 742e 6b65 7928 2920 3d3d 2051 742e  ent.key() == Qt.
+00009330: 4b65 792e 4b65 795f 456e 7465 723a 0a20  Key.Key_Enter:. 
+00009340: 2020 2020 2020 2023 2020 2020 2073 656c         #     sel
+00009350: 662e 7361 7665 5f63 6f6e 7461 6374 2829  f.save_contact()
+00009360: 0a20 2020 2020 2020 2069 6620 6576 656e  .        if even
+00009370: 742e 6b65 7928 2920 3d3d 2051 742e 4b65  t.key() == Qt.Ke
+00009380: 792e 4b65 795f 5461 6220 6f72 2065 7665  y.Key_Tab or eve
+00009390: 6e74 2e6b 6579 2829 203d 3d20 5174 2e4b  nt.key() == Qt.K
+000093a0: 6579 2e4b 6579 5f42 6163 6b74 6162 3a0a  ey.Key_Backtab:.
+000093b0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+000093c0: 656c 662e 7365 6e74 2e68 6173 466f 6375  elf.sent.hasFocu
+000093d0: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
+000093e0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+000093f0: 6728 2246 726f 6d20 7365 6e74 2229 0a20  g("From sent"). 
+00009400: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00009410: 6620 6d6f 6469 6669 6572 203d 3d20 5174  f modifier == Qt
+00009420: 2e53 6869 6674 4d6f 6469 6669 6572 3a0a  .ShiftModifier:.
+00009430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009440: 2020 2020 7072 6576 5f74 6162 203d 2073      prev_tab = s
+00009450: 656c 662e 7461 625f 7072 6576 2e67 6574  elf.tab_prev.get
+00009460: 2873 656c 662e 7365 6e74 290a 2020 2020  (self.sent).    
 00009470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009480: 2020 2020 6e65 7874 5f74 6162 2e64 6573      next_tab.des
-00009490: 656c 6563 7428 290a 2020 2020 2020 2020  elect().        
-000094a0: 2020 2020 2020 2020 2020 2020 6e65 7874              next
-000094b0: 5f74 6162 2e65 6e64 2846 616c 7365 290a  _tab.end(False).
+00009480: 7072 6576 5f74 6162 2e73 6574 466f 6375  prev_tab.setFocu
+00009490: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
+000094a0: 2020 2020 2020 2020 7072 6576 5f74 6162          prev_tab
+000094b0: 2e64 6573 656c 6563 7428 290a 2020 2020  .deselect().    
 000094c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094d0: 7265 7475 726e 0a20 2020 2020 2020 2020  return.         
-000094e0: 2020 2069 6620 7365 6c66 2e72 6563 6569     if self.recei
-000094f0: 7665 2e68 6173 466f 6375 7328 293a 0a20  ve.hasFocus():. 
-00009500: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00009510: 6f67 6765 722e 6465 6275 6728 2246 726f  ogger.debug("Fro
-00009520: 6d20 7265 6365 6976 6522 290a 2020 2020  m receive").    
-00009530: 2020 2020 2020 2020 2020 2020 6966 206d              if m
-00009540: 6f64 6966 6965 7220 3d3d 2051 742e 5368  odifier == Qt.Sh
-00009550: 6966 744d 6f64 6966 6965 723a 0a20 2020  iftModifier:.   
+000094d0: 7072 6576 5f74 6162 2e65 6e64 2846 616c  prev_tab.end(Fal
+000094e0: 7365 290a 2020 2020 2020 2020 2020 2020  se).            
+000094f0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00009500: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+00009510: 7874 5f74 6162 203d 2073 656c 662e 7461  xt_tab = self.ta
+00009520: 625f 6e65 7874 2e67 6574 2873 656c 662e  b_next.get(self.
+00009530: 7365 6e74 290a 2020 2020 2020 2020 2020  sent).          
+00009540: 2020 2020 2020 2020 2020 6e65 7874 5f74            next_t
+00009550: 6162 2e73 6574 466f 6375 7328 290a 2020  ab.setFocus().  
 00009560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009570: 2070 7265 765f 7461 6220 3d20 7365 6c66   prev_tab = self
-00009580: 2e74 6162 5f70 7265 762e 6765 7428 7365  .tab_prev.get(se
-00009590: 6c66 2e72 6563 6569 7665 290a 2020 2020  lf.receive).    
-000095a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095b0: 7072 6576 5f74 6162 2e73 6574 466f 6375  prev_tab.setFocu
-000095c0: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
-000095d0: 2020 2020 2020 2020 7072 6576 5f74 6162          prev_tab
-000095e0: 2e64 6573 656c 6563 7428 290a 2020 2020  .deselect().    
-000095f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009600: 7072 6576 5f74 6162 2e65 6e64 2846 616c  prev_tab.end(Fal
-00009610: 7365 290a 2020 2020 2020 2020 2020 2020  se).            
-00009620: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00009630: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-00009640: 7874 5f74 6162 203d 2073 656c 662e 7461  xt_tab = self.ta
-00009650: 625f 6e65 7874 2e67 6574 2873 656c 662e  b_next.get(self.
-00009660: 7265 6365 6976 6529 0a20 2020 2020 2020  receive).       
-00009670: 2020 2020 2020 2020 2020 2020 206e 6578               nex
-00009680: 745f 7461 622e 7365 7446 6f63 7573 2829  t_tab.setFocus()
-00009690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000096a0: 2020 2020 206e 6578 745f 7461 622e 6465       next_tab.de
-000096b0: 7365 6c65 6374 2829 0a20 2020 2020 2020  select().       
-000096c0: 2020 2020 2020 2020 2020 2020 206e 6578               nex
-000096d0: 745f 7461 622e 656e 6428 4661 6c73 6529  t_tab.end(False)
-000096e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000096f0: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-00009700: 2020 2020 6966 2073 656c 662e 6f74 6865      if self.othe
-00009710: 725f 312e 6861 7346 6f63 7573 2829 3a0a  r_1.hasFocus():.
-00009720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009730: 6c6f 6767 6572 2e64 6562 7567 2822 4672  logger.debug("Fr
-00009740: 6f6d 206f 7468 6572 5f31 2229 0a20 2020  om other_1").   
-00009750: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00009760: 6d6f 6469 6669 6572 203d 3d20 5174 2e53  modifier == Qt.S
-00009770: 6869 6674 4d6f 6469 6669 6572 3a0a 2020  hiftModifier:.  
+00009570: 2020 6e65 7874 5f74 6162 2e64 6573 656c    next_tab.desel
+00009580: 6563 7428 290a 2020 2020 2020 2020 2020  ect().          
+00009590: 2020 2020 2020 2020 2020 6e65 7874 5f74            next_t
+000095a0: 6162 2e65 6e64 2846 616c 7365 290a 2020  ab.end(False).  
+000095b0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000095c0: 7475 726e 0a20 2020 2020 2020 2020 2020  turn.           
+000095d0: 2069 6620 7365 6c66 2e72 6563 6569 7665   if self.receive
+000095e0: 2e68 6173 466f 6375 7328 293a 0a20 2020  .hasFocus():.   
+000095f0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+00009600: 6765 722e 6465 6275 6728 2246 726f 6d20  ger.debug("From 
+00009610: 7265 6365 6976 6522 290a 2020 2020 2020  receive").      
+00009620: 2020 2020 2020 2020 2020 6966 206d 6f64            if mod
+00009630: 6966 6965 7220 3d3d 2051 742e 5368 6966  ifier == Qt.Shif
+00009640: 744d 6f64 6966 6965 723a 0a20 2020 2020  tModifier:.     
+00009650: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00009660: 7265 765f 7461 6220 3d20 7365 6c66 2e74  rev_tab = self.t
+00009670: 6162 5f70 7265 762e 6765 7428 7365 6c66  ab_prev.get(self
+00009680: 2e72 6563 6569 7665 290a 2020 2020 2020  .receive).      
+00009690: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+000096a0: 6576 5f74 6162 2e73 6574 466f 6375 7328  ev_tab.setFocus(
+000096b0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000096c0: 2020 2020 2020 7072 6576 5f74 6162 2e64        prev_tab.d
+000096d0: 6573 656c 6563 7428 290a 2020 2020 2020  eselect().      
+000096e0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+000096f0: 6576 5f74 6162 2e65 6e64 2846 616c 7365  ev_tab.end(False
+00009700: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00009710: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00009720: 2020 2020 2020 2020 2020 2020 6e65 7874              next
+00009730: 5f74 6162 203d 2073 656c 662e 7461 625f  _tab = self.tab_
+00009740: 6e65 7874 2e67 6574 2873 656c 662e 7265  next.get(self.re
+00009750: 6365 6976 6529 0a20 2020 2020 2020 2020  ceive).         
+00009760: 2020 2020 2020 2020 2020 206e 6578 745f             next_
+00009770: 7461 622e 7365 7446 6f63 7573 2829 0a20  tab.setFocus(). 
 00009780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009790: 2020 7072 6576 5f74 6162 203d 2073 656c    prev_tab = sel
-000097a0: 662e 7461 625f 7072 6576 2e67 6574 2873  f.tab_prev.get(s
-000097b0: 656c 662e 6f74 6865 725f 3129 0a20 2020  elf.other_1).   
-000097c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000097d0: 2070 7265 765f 7461 622e 7365 7446 6f63   prev_tab.setFoc
-000097e0: 7573 2829 0a20 2020 2020 2020 2020 2020  us().           
-000097f0: 2020 2020 2020 2020 2070 7265 765f 7461           prev_ta
-00009800: 622e 6465 7365 6c65 6374 2829 0a20 2020  b.deselect().   
-00009810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009820: 2070 7265 765f 7461 622e 656e 6428 4661   prev_tab.end(Fa
-00009830: 6c73 6529 0a20 2020 2020 2020 2020 2020  lse).           
-00009840: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00009850: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00009860: 6578 745f 7461 6220 3d20 7365 6c66 2e74  ext_tab = self.t
-00009870: 6162 5f6e 6578 742e 6765 7428 7365 6c66  ab_next.get(self
-00009880: 2e6f 7468 6572 5f31 290a 2020 2020 2020  .other_1).      
-00009890: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-000098a0: 7874 5f74 6162 2e73 6574 466f 6375 7328  xt_tab.setFocus(
-000098b0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000098c0: 2020 2020 2020 6e65 7874 5f74 6162 2e64        next_tab.d
-000098d0: 6573 656c 6563 7428 290a 2020 2020 2020  eselect().      
-000098e0: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-000098f0: 7874 5f74 6162 2e65 6e64 2846 616c 7365  xt_tab.end(False
-00009900: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00009910: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-00009920: 2020 2020 2069 6620 7365 6c66 2e6f 7468       if self.oth
-00009930: 6572 5f32 2e68 6173 466f 6375 7328 293a  er_2.hasFocus():
-00009940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009950: 206c 6f67 6765 722e 6465 6275 6728 2246   logger.debug("F
-00009960: 726f 6d20 6f74 6865 725f 3222 290a 2020  rom other_2").  
-00009970: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00009980: 206d 6f64 6966 6965 7220 3d3d 2051 742e   modifier == Qt.
-00009990: 5368 6966 744d 6f64 6966 6965 723a 0a20  ShiftModifier:. 
+00009790: 2020 206e 6578 745f 7461 622e 6465 7365     next_tab.dese
+000097a0: 6c65 6374 2829 0a20 2020 2020 2020 2020  lect().         
+000097b0: 2020 2020 2020 2020 2020 206e 6578 745f             next_
+000097c0: 7461 622e 656e 6428 4661 6c73 6529 0a20  tab.end(False). 
+000097d0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000097e0: 6574 7572 6e0a 2020 2020 2020 2020 2020  eturn.          
+000097f0: 2020 6966 2073 656c 662e 6f74 6865 725f    if self.other_
+00009800: 312e 6861 7346 6f63 7573 2829 3a0a 2020  1.hasFocus():.  
+00009810: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00009820: 6767 6572 2e64 6562 7567 2822 4672 6f6d  gger.debug("From
+00009830: 206f 7468 6572 5f31 2229 0a20 2020 2020   other_1").     
+00009840: 2020 2020 2020 2020 2020 2069 6620 6d6f             if mo
+00009850: 6469 6669 6572 203d 3d20 5174 2e53 6869  difier == Qt.Shi
+00009860: 6674 4d6f 6469 6669 6572 3a0a 2020 2020  ftModifier:.    
+00009870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009880: 7072 6576 5f74 6162 203d 2073 656c 662e  prev_tab = self.
+00009890: 7461 625f 7072 6576 2e67 6574 2873 656c  tab_prev.get(sel
+000098a0: 662e 6f74 6865 725f 3129 0a20 2020 2020  f.other_1).     
+000098b0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000098c0: 7265 765f 7461 622e 7365 7446 6f63 7573  rev_tab.setFocus
+000098d0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+000098e0: 2020 2020 2020 2070 7265 765f 7461 622e         prev_tab.
+000098f0: 6465 7365 6c65 6374 2829 0a20 2020 2020  deselect().     
+00009900: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00009910: 7265 765f 7461 622e 656e 6428 4661 6c73  rev_tab.end(Fals
+00009920: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+00009930: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00009940: 2020 2020 2020 2020 2020 2020 206e 6578               nex
+00009950: 745f 7461 6220 3d20 7365 6c66 2e74 6162  t_tab = self.tab
+00009960: 5f6e 6578 742e 6765 7428 7365 6c66 2e6f  _next.get(self.o
+00009970: 7468 6572 5f31 290a 2020 2020 2020 2020  ther_1).        
+00009980: 2020 2020 2020 2020 2020 2020 6e65 7874              next
+00009990: 5f74 6162 2e73 6574 466f 6375 7328 290a  _tab.setFocus().
 000099a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099b0: 2020 2070 7265 765f 7461 6220 3d20 7365     prev_tab = se
-000099c0: 6c66 2e74 6162 5f70 7265 762e 6765 7428  lf.tab_prev.get(
-000099d0: 7365 6c66 2e6f 7468 6572 5f32 290a 2020  self.other_2).  
-000099e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099f0: 2020 7072 6576 5f74 6162 2e73 6574 466f    prev_tab.setFo
-00009a00: 6375 7328 290a 2020 2020 2020 2020 2020  cus().          
-00009a10: 2020 2020 2020 2020 2020 7072 6576 5f74            prev_t
-00009a20: 6162 2e64 6573 656c 6563 7428 290a 2020  ab.deselect().  
-00009a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a40: 2020 7072 6576 5f74 6162 2e65 6e64 2846    prev_tab.end(F
-00009a50: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
-00009a60: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00009a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a80: 6e65 7874 5f74 6162 203d 2073 656c 662e  next_tab = self.
-00009a90: 7461 625f 6e65 7874 2e67 6574 2873 656c  tab_next.get(sel
-00009aa0: 662e 6f74 6865 725f 3229 0a20 2020 2020  f.other_2).     
-00009ab0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00009ac0: 6578 745f 7461 622e 7365 7446 6f63 7573  ext_tab.setFocus
-00009ad0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00009ae0: 2020 2020 2020 206e 6578 745f 7461 622e         next_tab.
-00009af0: 6465 7365 6c65 6374 2829 0a20 2020 2020  deselect().     
-00009b00: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00009b10: 6578 745f 7461 622e 656e 6428 4661 6c73  ext_tab.end(Fals
-00009b20: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-00009b30: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-00009b40: 2020 2020 2020 6966 2073 656c 662e 6361        if self.ca
-00009b50: 6c6c 7369 676e 2e68 6173 466f 6375 7328  llsign.hasFocus(
-00009b60: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00009b70: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-00009b80: 2246 726f 6d20 6361 6c6c 7369 676e 2229  "From callsign")
-00009b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009ba0: 2073 656c 662e 6368 6563 6b5f 6361 6c6c   self.check_call
-00009bb0: 7369 676e 2873 656c 662e 6361 6c6c 7369  sign(self.callsi
-00009bc0: 676e 2e74 6578 7428 2929 0a20 2020 2020  gn.text()).     
-00009bd0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00009be0: 6c66 2e63 6865 636b 5f64 7570 6528 7365  lf.check_dupe(se
-00009bf0: 6c66 2e63 616c 6c73 6967 6e2e 7465 7874  lf.callsign.text
-00009c00: 2829 293a 0a20 2020 2020 2020 2020 2020  ()):.           
-00009c10: 2020 2020 2020 2020 2073 656c 662e 6475           self.du
-00009c20: 7065 5f69 6e64 6963 6174 6f72 2e73 686f  pe_indicator.sho
-00009c30: 7728 290a 2020 2020 2020 2020 2020 2020  w().            
-00009c40: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00009c50: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00009c60: 6c66 2e64 7570 655f 696e 6469 6361 746f  lf.dupe_indicato
-00009c70: 722e 6869 6465 2829 0a20 2020 2020 2020  r.hide().       
-00009c80: 2020 2020 2020 2020 2069 6620 6d6f 6469           if modi
-00009c90: 6669 6572 203d 3d20 5174 2e53 6869 6674  fier == Qt.Shift
-00009ca0: 4d6f 6469 6669 6572 3a0a 2020 2020 2020  Modifier:.      
-00009cb0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00009cc0: 6576 5f74 6162 203d 2073 656c 662e 7461  ev_tab = self.ta
-00009cd0: 625f 7072 6576 2e67 6574 2873 656c 662e  b_prev.get(self.
-00009ce0: 6361 6c6c 7369 676e 290a 2020 2020 2020  callsign).      
-00009cf0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00009d00: 6576 5f74 6162 2e73 6574 466f 6375 7328  ev_tab.setFocus(
-00009d10: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00009d20: 2020 2020 2020 7072 6576 5f74 6162 2e64        prev_tab.d
-00009d30: 6573 656c 6563 7428 290a 2020 2020 2020  eselect().      
-00009d40: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00009d50: 6576 5f74 6162 2e65 6e64 2846 616c 7365  ev_tab.end(False
-00009d60: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00009d70: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00009d80: 2020 2020 2020 2020 2020 2020 7465 7874              text
-00009d90: 203d 2073 656c 662e 6361 6c6c 7369 676e   = self.callsign
-00009da0: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
-00009db0: 2020 2020 2020 2020 2020 2020 7465 7874              text
-00009dc0: 203d 2074 6578 742e 7570 7065 7228 290a   = text.upper().
-00009dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009de0: 2020 2020 5f74 6865 7468 7265 6164 203d      _thethread =
-00009df0: 2074 6872 6561 6469 6e67 2e54 6872 6561   threading.Threa
-00009e00: 6428 0a20 2020 2020 2020 2020 2020 2020  d(.             
-00009e10: 2020 2020 2020 2020 2020 2074 6172 6765             targe
-00009e20: 743d 7365 6c66 2e63 6865 636b 5f63 616c  t=self.check_cal
-00009e30: 6c73 6967 6e32 2c0a 2020 2020 2020 2020  lsign2,.        
-00009e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e50: 6172 6773 3d28 7465 7874 2c29 2c0a 2020  args=(text,),.  
-00009e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e70: 2020 2020 2020 6461 656d 6f6e 3d54 7275        daemon=Tru
-00009e80: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00009e90: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00009ea0: 2020 2020 2020 2020 2020 2020 205f 7468               _th
-00009eb0: 6574 6872 6561 642e 7374 6172 7428 290a  ethread.start().
+000099b0: 2020 2020 6e65 7874 5f74 6162 2e64 6573      next_tab.des
+000099c0: 656c 6563 7428 290a 2020 2020 2020 2020  elect().        
+000099d0: 2020 2020 2020 2020 2020 2020 6e65 7874              next
+000099e0: 5f74 6162 2e65 6e64 2846 616c 7365 290a  _tab.end(False).
+000099f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a00: 7265 7475 726e 0a20 2020 2020 2020 2020  return.         
+00009a10: 2020 2069 6620 7365 6c66 2e6f 7468 6572     if self.other
+00009a20: 5f32 2e68 6173 466f 6375 7328 293a 0a20  _2.hasFocus():. 
+00009a30: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00009a40: 6f67 6765 722e 6465 6275 6728 2246 726f  ogger.debug("Fro
+00009a50: 6d20 6f74 6865 725f 3222 290a 2020 2020  m other_2").    
+00009a60: 2020 2020 2020 2020 2020 2020 6966 206d              if m
+00009a70: 6f64 6966 6965 7220 3d3d 2051 742e 5368  odifier == Qt.Sh
+00009a80: 6966 744d 6f64 6966 6965 723a 0a20 2020  iftModifier:.   
+00009a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009aa0: 2070 7265 765f 7461 6220 3d20 7365 6c66   prev_tab = self
+00009ab0: 2e74 6162 5f70 7265 762e 6765 7428 7365  .tab_prev.get(se
+00009ac0: 6c66 2e6f 7468 6572 5f32 290a 2020 2020  lf.other_2).    
+00009ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ae0: 7072 6576 5f74 6162 2e73 6574 466f 6375  prev_tab.setFocu
+00009af0: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
+00009b00: 2020 2020 2020 2020 7072 6576 5f74 6162          prev_tab
+00009b10: 2e64 6573 656c 6563 7428 290a 2020 2020  .deselect().    
+00009b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b30: 7072 6576 5f74 6162 2e65 6e64 2846 616c  prev_tab.end(Fal
+00009b40: 7365 290a 2020 2020 2020 2020 2020 2020  se).            
+00009b50: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00009b60: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+00009b70: 7874 5f74 6162 203d 2073 656c 662e 7461  xt_tab = self.ta
+00009b80: 625f 6e65 7874 2e67 6574 2873 656c 662e  b_next.get(self.
+00009b90: 6f74 6865 725f 3229 0a20 2020 2020 2020  other_2).       
+00009ba0: 2020 2020 2020 2020 2020 2020 206e 6578               nex
+00009bb0: 745f 7461 622e 7365 7446 6f63 7573 2829  t_tab.setFocus()
+00009bc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009bd0: 2020 2020 206e 6578 745f 7461 622e 6465       next_tab.de
+00009be0: 7365 6c65 6374 2829 0a20 2020 2020 2020  select().       
+00009bf0: 2020 2020 2020 2020 2020 2020 206e 6578               nex
+00009c00: 745f 7461 622e 656e 6428 4661 6c73 6529  t_tab.end(False)
+00009c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009c20: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+00009c30: 2020 2020 6966 2073 656c 662e 6361 6c6c      if self.call
+00009c40: 7369 676e 2e68 6173 466f 6375 7328 293a  sign.hasFocus():
+00009c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009c60: 206c 6f67 6765 722e 6465 6275 6728 2246   logger.debug("F
+00009c70: 726f 6d20 6361 6c6c 7369 676e 2229 0a20  rom callsign"). 
+00009c80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00009c90: 656c 662e 6368 6563 6b5f 6361 6c6c 7369  elf.check_callsi
+00009ca0: 676e 2873 656c 662e 6361 6c6c 7369 676e  gn(self.callsign
+00009cb0: 2e74 6578 7428 2929 0a20 2020 2020 2020  .text()).       
+00009cc0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00009cd0: 2e63 6865 636b 5f64 7570 6528 7365 6c66  .check_dupe(self
+00009ce0: 2e63 616c 6c73 6967 6e2e 7465 7874 2829  .callsign.text()
+00009cf0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00009d00: 2020 2020 2020 2073 656c 662e 6475 7065         self.dupe
+00009d10: 5f69 6e64 6963 6174 6f72 2e73 686f 7728  _indicator.show(
+00009d20: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00009d30: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00009d40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00009d50: 2e64 7570 655f 696e 6469 6361 746f 722e  .dupe_indicator.
+00009d60: 6869 6465 2829 0a20 2020 2020 2020 2020  hide().         
+00009d70: 2020 2020 2020 2069 6620 6d6f 6469 6669         if modifi
+00009d80: 6572 203d 3d20 5174 2e53 6869 6674 4d6f  er == Qt.ShiftMo
+00009d90: 6469 6669 6572 3a0a 2020 2020 2020 2020  difier:.        
+00009da0: 2020 2020 2020 2020 2020 2020 7072 6576              prev
+00009db0: 5f74 6162 203d 2073 656c 662e 7461 625f  _tab = self.tab_
+00009dc0: 7072 6576 2e67 6574 2873 656c 662e 6361  prev.get(self.ca
+00009dd0: 6c6c 7369 676e 290a 2020 2020 2020 2020  llsign).        
+00009de0: 2020 2020 2020 2020 2020 2020 7072 6576              prev
+00009df0: 5f74 6162 2e73 6574 466f 6375 7328 290a  _tab.setFocus().
+00009e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e10: 2020 2020 7072 6576 5f74 6162 2e64 6573      prev_tab.des
+00009e20: 656c 6563 7428 290a 2020 2020 2020 2020  elect().        
+00009e30: 2020 2020 2020 2020 2020 2020 7072 6576              prev
+00009e40: 5f74 6162 2e65 6e64 2846 616c 7365 290a  _tab.end(False).
+00009e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e60: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00009e70: 2020 2020 2020 2020 2020 7465 7874 203d            text =
+00009e80: 2073 656c 662e 6361 6c6c 7369 676e 2e74   self.callsign.t
+00009e90: 6578 7428 290a 2020 2020 2020 2020 2020  ext().          
+00009ea0: 2020 2020 2020 2020 2020 7465 7874 203d            text =
+00009eb0: 2074 6578 742e 7570 7065 7228 290a 2020   text.upper().  
 00009ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ed0: 2020 2020 6e65 7874 5f74 6162 203d 2073      next_tab = s
-00009ee0: 656c 662e 7461 625f 6e65 7874 2e67 6574  elf.tab_next.get
-00009ef0: 2873 656c 662e 6361 6c6c 7369 676e 290a  (self.callsign).
-00009f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f10: 2020 2020 6e65 7874 5f74 6162 2e73 6574      next_tab.set
-00009f20: 466f 6375 7328 290a 2020 2020 2020 2020  Focus().        
-00009f30: 2020 2020 2020 2020 2020 2020 6e65 7874              next
-00009f40: 5f74 6162 2e64 6573 656c 6563 7428 290a  _tab.deselect().
+00009ed0: 2020 5f74 6865 7468 7265 6164 203d 2074    _thethread = t
+00009ee0: 6872 6561 6469 6e67 2e54 6872 6561 6428  hreading.Thread(
+00009ef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009f00: 2020 2020 2020 2020 2074 6172 6765 743d           target=
+00009f10: 7365 6c66 2e63 6865 636b 5f63 616c 6c73  self.check_calls
+00009f20: 6967 6e32 2c0a 2020 2020 2020 2020 2020  ign2,.          
+00009f30: 2020 2020 2020 2020 2020 2020 2020 6172                ar
+00009f40: 6773 3d28 7465 7874 2c29 2c0a 2020 2020  gs=(text,),.    
 00009f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f60: 2020 2020 6e65 7874 5f74 6162 2e65 6e64      next_tab.end
-00009f70: 2846 616c 7365 290a 2020 2020 2020 2020  (False).        
-00009f80: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-00009f90: 2020 2020 2020 2069 6620 6576 656e 742e         if event.
-00009fa0: 6b65 7928 2920 3d3d 2051 742e 4b65 795f  key() == Qt.Key_
-00009fb0: 4631 3a0a 2020 2020 2020 2020 2020 2020  F1:.            
-00009fc0: 7365 6c66 2e73 656e 6466 3128 290a 2020  self.sendf1().  
-00009fd0: 2020 2020 2020 6966 2065 7665 6e74 2e6b        if event.k
-00009fe0: 6579 2829 203d 3d20 5174 2e4b 6579 5f46  ey() == Qt.Key_F
-00009ff0: 323a 0a20 2020 2020 2020 2020 2020 2073  2:.            s
-0000a000: 656c 662e 7365 6e64 6632 2829 0a20 2020  elf.sendf2().   
-0000a010: 2020 2020 2069 6620 6576 656e 742e 6b65       if event.ke
-0000a020: 7928 2920 3d3d 2051 742e 4b65 795f 4633  y() == Qt.Key_F3
-0000a030: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000a040: 6c66 2e73 656e 6466 3328 290a 2020 2020  lf.sendf3().    
-0000a050: 2020 2020 6966 2065 7665 6e74 2e6b 6579      if event.key
-0000a060: 2829 203d 3d20 5174 2e4b 6579 5f46 343a  () == Qt.Key_F4:
-0000a070: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000a080: 662e 7365 6e64 6634 2829 0a20 2020 2020  f.sendf4().     
-0000a090: 2020 2069 6620 6576 656e 742e 6b65 7928     if event.key(
-0000a0a0: 2920 3d3d 2051 742e 4b65 795f 4635 3a0a  ) == Qt.Key_F5:.
-0000a0b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000a0c0: 2e73 656e 6466 3528 290a 2020 2020 2020  .sendf5().      
-0000a0d0: 2020 6966 2065 7665 6e74 2e6b 6579 2829    if event.key()
-0000a0e0: 203d 3d20 5174 2e4b 6579 5f46 363a 0a20   == Qt.Key_F6:. 
-0000a0f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000a100: 7365 6e64 6636 2829 0a20 2020 2020 2020  sendf6().       
-0000a110: 2069 6620 6576 656e 742e 6b65 7928 2920   if event.key() 
-0000a120: 3d3d 2051 742e 4b65 795f 4637 3a0a 2020  == Qt.Key_F7:.  
-0000a130: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-0000a140: 656e 6466 3728 290a 2020 2020 2020 2020  endf7().        
-0000a150: 6966 2065 7665 6e74 2e6b 6579 2829 203d  if event.key() =
-0000a160: 3d20 5174 2e4b 6579 5f46 383a 0a20 2020  = Qt.Key_F8:.   
-0000a170: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-0000a180: 6e64 6638 2829 0a20 2020 2020 2020 2069  ndf8().        i
-0000a190: 6620 6576 656e 742e 6b65 7928 2920 3d3d  f event.key() ==
-0000a1a0: 2051 742e 4b65 795f 4639 3a0a 2020 2020   Qt.Key_F9:.    
-0000a1b0: 2020 2020 2020 2020 7365 6c66 2e73 656e          self.sen
-0000a1c0: 6466 3928 290a 2020 2020 2020 2020 6966  df9().        if
-0000a1d0: 2065 7665 6e74 2e6b 6579 2829 203d 3d20   event.key() == 
-0000a1e0: 5174 2e4b 6579 5f46 3130 3a0a 2020 2020  Qt.Key_F10:.    
-0000a1f0: 2020 2020 2020 2020 7365 6c66 2e73 656e          self.sen
-0000a200: 6466 3130 2829 0a20 2020 2020 2020 2069  df10().        i
-0000a210: 6620 6576 656e 742e 6b65 7928 2920 3d3d  f event.key() ==
-0000a220: 2051 742e 4b65 795f 4631 313a 0a20 2020   Qt.Key_F11:.   
-0000a230: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-0000a240: 6e64 6631 3128 290a 2020 2020 2020 2020  ndf11().        
-0000a250: 6966 2065 7665 6e74 2e6b 6579 2829 203d  if event.key() =
-0000a260: 3d20 5174 2e4b 6579 5f46 3132 3a0a 2020  = Qt.Key_F12:.  
-0000a270: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-0000a280: 656e 6466 3132 2829 0a0a 2020 2020 6465  endf12()..    de
-0000a290: 6620 7365 745f 7769 6e64 6f77 5f74 6974  f set_window_tit
-0000a2a0: 6c65 2873 656c 6629 3a0a 2020 2020 2020  le(self):.      
-0000a2b0: 2020 2222 2253 6574 2077 696e 646f 7720    """Set window 
-0000a2c0: 7469 746c 6522 2222 0a20 2020 2020 2020  title""".       
-0000a2d0: 2076 666f 6120 3d20 7365 6c66 2e72 6164   vfoa = self.rad
-0000a2e0: 696f 5f73 7461 7465 2e67 6574 2822 7666  io_state.get("vf
-0000a2f0: 6f61 222c 2022 2229 0a20 2020 2020 2020  oa", "").       
-0000a300: 2069 6620 7666 6f61 3a0a 2020 2020 2020   if vfoa:.      
-0000a310: 2020 2020 2020 7666 6f61 203d 2069 6e74        vfoa = int
-0000a320: 2876 666f 6129 202f 2031 3030 300a 2020  (vfoa) / 1000.  
-0000a330: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000a340: 2020 2020 2020 2020 7666 6f61 203d 2030          vfoa = 0
-0000a350: 2e30 0a20 2020 2020 2020 2063 6f6e 7465  .0.        conte
-0000a360: 7374 5f6e 616d 6520 3d20 2222 0a20 2020  st_name = "".   
-0000a370: 2020 2020 2069 6620 7365 6c66 2e63 6f6e       if self.con
-0000a380: 7465 7374 3a0a 2020 2020 2020 2020 2020  test:.          
-0000a390: 2020 636f 6e74 6573 745f 6e61 6d65 203d    contest_name =
-0000a3a0: 2073 656c 662e 636f 6e74 6573 742e 6e61   self.contest.na
-0000a3b0: 6d65 0a20 2020 2020 2020 206c 696e 6520  me.        line 
-0000a3c0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-0000a3d0: 6622 7666 6f61 3a7b 726f 756e 6428 7666  f"vfoa:{round(vf
-0000a3e0: 6f61 2c32 297d 2022 0a20 2020 2020 2020  oa,2)} ".       
-0000a3f0: 2020 2020 2066 226d 6f64 653a 7b73 656c       f"mode:{sel
-0000a400: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
-0000a410: 7428 276d 6f64 6527 2c20 2727 297d 2022  t('mode', '')} "
-0000a420: 0a20 2020 2020 2020 2020 2020 2066 224f  .            f"O
-0000a430: 503a 7b73 656c 662e 6375 7272 656e 745f  P:{self.current_
-0000a440: 6f70 7d20 7b63 6f6e 7465 7374 5f6e 616d  op} {contest_nam
-0000a450: 657d 2022 0a20 2020 2020 2020 2020 2020  e} ".           
-0000a460: 2066 222d 204e 6f74 314d 4d20 767b 5f5f   f"- Not1MM v{__
-0000a470: 7665 7273 696f 6e5f 5f7d 220a 2020 2020  version__}".    
-0000a480: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
-0000a490: 6c66 2e73 6574 5769 6e64 6f77 5469 746c  lf.setWindowTitl
-0000a4a0: 6528 6c69 6e65 290a 0a20 2020 2064 6566  e(line)..    def
-0000a4b0: 2073 656e 645f 776f 726b 6564 5f6c 6973   send_worked_lis
-0000a4c0: 7428 7365 6c66 2920 2d3e 204e 6f6e 653a  t(self) -> None:
-0000a4d0: 0a20 2020 2020 2020 2022 2222 5365 6e64  .        """Send
-0000a4e0: 206d 6573 7361 6765 2063 6f6e 7461 696e   message contain
-0000a4f0: 696e 6720 776f 726b 6564 2063 6f6e 7461  ing worked conta
-0000a500: 6374 7320 616e 6420 6261 6e64 7322 2222  cts and bands"""
-0000a510: 0a20 2020 2020 2020 2063 6d64 203d 207b  .        cmd = {
-0000a520: 7d0a 2020 2020 2020 2020 636d 645b 2263  }.        cmd["c
-0000a530: 6d64 225d 203d 2022 574f 524b 4544 220a  md"] = "WORKED".
-0000a540: 2020 2020 2020 2020 636d 645b 2273 7461          cmd["sta
-0000a550: 7469 6f6e 225d 203d 2070 6c61 7466 6f72  tion"] = platfor
-0000a560: 6d2e 6e6f 6465 2829 0a20 2020 2020 2020  m.node().       
-0000a570: 2063 6d64 5b22 776f 726b 6564 225d 203d   cmd["worked"] =
-0000a580: 2073 656c 662e 776f 726b 6564 5f6c 6973   self.worked_lis
-0000a590: 740a 2020 2020 2020 2020 6c6f 6767 6572  t.        logger
-0000a5a0: 2e64 6562 7567 2822 2573 222c 2066 227b  .debug("%s", f"{
-0000a5b0: 636d 647d 2229 0a20 2020 2020 2020 2073  cmd}").        s
-0000a5c0: 656c 662e 6d75 6c74 6963 6173 745f 696e  elf.multicast_in
-0000a5d0: 7465 7266 6163 652e 7365 6e64 5f61 735f  terface.send_as_
-0000a5e0: 6a73 6f6e 2863 6d64 290a 0a20 2020 2064  json(cmd)..    d
-0000a5f0: 6566 2063 6c65 6172 696e 7075 7473 2873  ef clearinputs(s
-0000a600: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-0000a610: 2243 6c65 6172 7320 7468 6520 7465 7874  "Clears the text
-0000a620: 2069 6e70 7574 2066 6965 6c64 7320 616e   input fields an
-0000a630: 6420 7365 7473 2066 6f63 7573 2074 6f20  d sets focus to 
-0000a640: 6361 6c6c 7369 676e 2066 6965 6c64 2e22  callsign field."
-0000a650: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
-0000a660: 6475 7065 5f69 6e64 6963 6174 6f72 2e68  dupe_indicator.h
-0000a670: 6964 6528 290a 2020 2020 2020 2020 7365  ide().        se
-0000a680: 6c66 2e63 6f6e 7461 6374 203d 2073 656c  lf.contact = sel
-0000a690: 662e 6461 7461 6261 7365 2e65 6d70 7479  f.database.empty
-0000a6a0: 5f63 6f6e 7461 6374 0a20 2020 2020 2020  _contact.       
-0000a6b0: 2073 656c 662e 6865 6164 696e 675f 6469   self.heading_di
-0000a6c0: 7374 616e 6365 2e73 6574 5465 7874 2822  stance.setText("
-0000a6d0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-0000a6e0: 6478 5f65 6e74 6974 792e 7365 7454 6578  dx_entity.setTex
-0000a6f0: 7428 2222 290a 2020 2020 2020 2020 6966  t("").        if
-0000a700: 2073 656c 662e 636f 6e74 6573 743a 0a20   self.contest:. 
-0000a710: 2020 2020 2020 2020 2020 206d 756c 7473             mults
-0000a720: 203d 2073 656c 662e 636f 6e74 6573 742e   = self.contest.
-0000a730: 7368 6f77 5f6d 756c 7473 2873 656c 6629  show_mults(self)
-0000a740: 0a20 2020 2020 2020 2020 2020 2071 736f  .            qso
-0000a750: 7320 3d20 7365 6c66 2e63 6f6e 7465 7374  s = self.contest
-0000a760: 2e73 686f 775f 7173 6f28 7365 6c66 290a  .show_qso(self).
-0000a770: 2020 2020 2020 2020 2020 2020 6d75 6c74              mult
-0000a780: 7374 7269 6e67 203d 2066 227b 7173 6f73  string = f"{qsos
-0000a790: 7d2f 7b6d 756c 7473 7d22 0a20 2020 2020  }/{mults}".     
-0000a7a0: 2020 2020 2020 2073 656c 662e 6d75 6c74         self.mult
-0000a7b0: 732e 7365 7454 6578 7428 6d75 6c74 7374  s.setText(multst
-0000a7c0: 7269 6e67 290a 2020 2020 2020 2020 2020  ring).          
-0000a7d0: 2020 7363 6f72 6520 3d20 7365 6c66 2e63    score = self.c
-0000a7e0: 6f6e 7465 7374 2e63 616c 635f 7363 6f72  ontest.calc_scor
-0000a7f0: 6528 7365 6c66 290a 2020 2020 2020 2020  e(self).        
-0000a800: 2020 2020 7365 6c66 2e73 636f 7265 2e73      self.score.s
-0000a810: 6574 5465 7874 2873 7472 2873 636f 7265  etText(str(score
-0000a820: 2929 0a20 2020 2020 2020 2020 2020 2073  )).            s
-0000a830: 656c 662e 636f 6e74 6573 742e 7265 7365  elf.contest.rese
-0000a840: 745f 6c61 6265 6c28 7365 6c66 290a 2020  t_label(self).  
-0000a850: 2020 2020 2020 7365 6c66 2e63 616c 6c73        self.calls
-0000a860: 6967 6e2e 636c 6561 7228 290a 2020 2020  ign.clear().    
-0000a870: 2020 2020 6966 2073 656c 662e 6375 7272      if self.curr
-0000a880: 656e 745f 6d6f 6465 203d 3d20 2243 5722  ent_mode == "CW"
-0000a890: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000a8a0: 6c66 2e73 656e 742e 7365 7454 6578 7428  lf.sent.setText(
-0000a8b0: 2235 3939 2229 0a20 2020 2020 2020 2020  "599").         
-0000a8c0: 2020 2073 656c 662e 7265 6365 6976 652e     self.receive.
-0000a8d0: 7365 7454 6578 7428 2235 3939 2229 0a20  setText("599"). 
-0000a8e0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000a8f0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-0000a900: 6e74 2e73 6574 5465 7874 2822 3539 2229  nt.setText("59")
-0000a910: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000a920: 662e 7265 6365 6976 652e 7365 7454 6578  f.receive.setTex
-0000a930: 7428 2235 3922 290a 2020 2020 2020 2020  t("59").        
-0000a940: 7365 6c66 2e6f 7468 6572 5f31 2e63 6c65  self.other_1.cle
-0000a950: 6172 2829 0a20 2020 2020 2020 2073 656c  ar().        sel
-0000a960: 662e 6f74 6865 725f 322e 636c 6561 7228  f.other_2.clear(
-0000a970: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
-0000a980: 616c 6c73 6967 6e2e 7365 7446 6f63 7573  allsign.setFocus
-0000a990: 2829 0a20 2020 2020 2020 2063 6d64 203d  ().        cmd =
-0000a9a0: 207b 7d0a 2020 2020 2020 2020 636d 645b   {}.        cmd[
-0000a9b0: 2263 6d64 225d 203d 2022 4341 4c4c 4348  "cmd"] = "CALLCH
-0000a9c0: 414e 4745 4422 0a20 2020 2020 2020 2063  ANGED".        c
-0000a9d0: 6d64 5b22 7374 6174 696f 6e22 5d20 3d20  md["station"] = 
-0000a9e0: 706c 6174 666f 726d 2e6e 6f64 6528 290a  platform.node().
-0000a9f0: 2020 2020 2020 2020 636d 645b 2263 616c          cmd["cal
-0000aa00: 6c22 5d20 3d20 2222 0a20 2020 2020 2020  l"] = "".       
-0000aa10: 2073 656c 662e 6d75 6c74 6963 6173 745f   self.multicast_
-0000aa20: 696e 7465 7266 6163 652e 7365 6e64 5f61  interface.send_a
-0000aa30: 735f 6a73 6f6e 2863 6d64 290a 0a20 2020  s_json(cmd)..   
-0000aa40: 2064 6566 2073 6176 655f 636f 6e74 6163   def save_contac
-0000aa50: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
-0000aa60: 2022 2222 5361 7665 2074 6f20 6462 2222   """Save to db""
-0000aa70: 220a 2020 2020 2020 2020 6c6f 6767 6572  ".        logger
-0000aa80: 2e64 6562 7567 2822 7361 7669 6e67 2063  .debug("saving c
-0000aa90: 6f6e 7461 6374 2229 0a20 2020 2020 2020  ontact").       
-0000aaa0: 2069 6620 7365 6c66 2e63 6f6e 7465 7374   if self.contest
-0000aab0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-0000aac0: 2020 2020 2020 7365 6c66 2e73 686f 775f        self.show_
-0000aad0: 6d65 7373 6167 655f 626f 7828 2259 6f75  message_box("You
-0000aae0: 2068 6176 6520 6e6f 2063 6f6e 7465 7374   have no contest
-0000aaf0: 2064 6566 696e 6564 2e22 290a 2020 2020   defined.").    
-0000ab00: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-0000ab10: 2020 2020 2020 2069 6620 6c65 6e28 7365         if len(se
-0000ab20: 6c66 2e63 616c 6c73 6967 6e2e 7465 7874  lf.callsign.text
-0000ab30: 2829 2920 3c20 333a 0a20 2020 2020 2020  ()) < 3:.       
-0000ab40: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-0000ab50: 2020 2020 6966 206e 6f74 2061 6e79 2863      if not any(c
-0000ab60: 6861 722e 6973 6469 6769 7428 2920 666f  har.isdigit() fo
-0000ab70: 7220 6368 6172 2069 6e20 7365 6c66 2e63  r char in self.c
-0000ab80: 616c 6c73 6967 6e2e 7465 7874 2829 293a  allsign.text()):
-0000ab90: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000aba0: 7572 6e0a 2020 2020 2020 2020 6966 206e  urn.        if n
-0000abb0: 6f74 2061 6e79 2863 6861 722e 6973 616c  ot any(char.isal
-0000abc0: 7068 6128 2920 666f 7220 6368 6172 2069  pha() for char i
-0000abd0: 6e20 7365 6c66 2e63 616c 6c73 6967 6e2e  n self.callsign.
-0000abe0: 7465 7874 2829 293a 0a20 2020 2020 2020  text()):.       
-0000abf0: 2020 2020 2072 6574 7572 6e0a 0a20 2020       return..   
-0000ac00: 2020 2020 2073 656c 662e 636f 6e74 6163       self.contac
-0000ac10: 745b 2254 5322 5d20 3d20 6461 7465 7469  t["TS"] = dateti
-0000ac20: 6d65 2e75 7463 6e6f 7728 292e 6973 6f66  me.utcnow().isof
-0000ac30: 6f72 6d61 7428 2220 2229 5b3a 3139 5d0a  ormat(" ")[:19].
-0000ac40: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-0000ac50: 7461 6374 5b22 4361 6c6c 225d 203d 2073  tact["Call"] = s
-0000ac60: 656c 662e 6361 6c6c 7369 676e 2e74 6578  elf.callsign.tex
-0000ac70: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
-0000ac80: 2e63 6f6e 7461 6374 5b22 4672 6571 225d  .contact["Freq"]
-0000ac90: 203d 2072 6f75 6e64 2866 6c6f 6174 2873   = round(float(s
-0000aca0: 656c 662e 7261 6469 6f5f 7374 6174 652e  elf.radio_state.
-0000acb0: 6765 7428 2276 666f 6122 2c20 302e 3029  get("vfoa", 0.0)
-0000acc0: 2920 2f20 3130 3030 2c20 3229 0a20 2020  ) / 1000, 2).   
-0000acd0: 2020 2020 2073 656c 662e 636f 6e74 6163       self.contac
-0000ace0: 745b 2251 5358 4672 6571 225d 203d 2072  t["QSXFreq"] = r
-0000acf0: 6f75 6e64 280a 2020 2020 2020 2020 2020  ound(.          
-0000ad00: 2020 666c 6f61 7428 7365 6c66 2e72 6164    float(self.rad
-0000ad10: 696f 5f73 7461 7465 2e67 6574 2822 7666  io_state.get("vf
-0000ad20: 6f61 222c 2030 2e30 2929 202f 2031 3030  oa", 0.0)) / 100
-0000ad30: 302c 2032 0a20 2020 2020 2020 2029 0a20  0, 2.        ). 
-0000ad40: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-0000ad50: 6163 745b 224d 6f64 6522 5d20 3d20 7365  act["Mode"] = se
-0000ad60: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
-0000ad70: 6574 2822 6d6f 6465 222c 2022 2229 0a20  et("mode", ""). 
-0000ad80: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-0000ad90: 6163 745b 2243 6f6e 7465 7374 4e61 6d65  act["ContestName
-0000ada0: 225d 203d 2073 656c 662e 636f 6e74 6573  "] = self.contes
-0000adb0: 742e 6361 6272 696c 6c6f 5f6e 616d 650a  t.cabrillo_name.
-0000adc0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-0000add0: 7461 6374 5b22 436f 6e74 6573 744e 5222  tact["ContestNR"
-0000ade0: 5d20 3d20 7365 6c66 2e70 7265 662e 6765  ] = self.pref.ge
-0000adf0: 7428 2263 6f6e 7465 7374 222c 2022 3022  t("contest", "0"
-0000ae00: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
-0000ae10: 6f6e 7461 6374 5b22 5374 6174 696f 6e50  ontact["StationP
-0000ae20: 7265 6669 7822 5d20 3d20 7365 6c66 2e73  refix"] = self.s
-0000ae30: 7461 7469 6f6e 2e67 6574 2822 4361 6c6c  tation.get("Call
-0000ae40: 222c 2022 2229 0a20 2020 2020 2020 2073  ", "").        s
-0000ae50: 656c 662e 636f 6e74 6163 745b 2257 5058  elf.contact["WPX
-0000ae60: 5072 6566 6978 225d 203d 2063 616c 6375  Prefix"] = calcu
-0000ae70: 6c61 7465 5f77 7078 5f70 7265 6669 7828  late_wpx_prefix(
-0000ae80: 7365 6c66 2e63 616c 6c73 6967 6e2e 7465  self.callsign.te
-0000ae90: 7874 2829 290a 2020 2020 2020 2020 7365  xt()).        se
-0000aea0: 6c66 2e63 6f6e 7461 6374 5b22 4973 5275  lf.contact["IsRu
-0000aeb0: 6e51 534f 225d 203d 2073 656c 662e 7261  nQSO"] = self.ra
-0000aec0: 6469 6f42 7574 746f 6e5f 7275 6e2e 6973  dioButton_run.is
-0000aed0: 4368 6563 6b65 6428 290a 2020 2020 2020  Checked().      
-0000aee0: 2020 7365 6c66 2e63 6f6e 7461 6374 5b22    self.contact["
-0000aef0: 4f70 6572 6174 6f72 225d 203d 2073 656c  Operator"] = sel
-0000af00: 662e 6375 7272 656e 745f 6f70 0a20 2020  f.current_op.   
-0000af10: 2020 2020 2073 656c 662e 636f 6e74 6163       self.contac
-0000af20: 745b 224e 6574 4269 6f73 4e61 6d65 225d  t["NetBiosName"]
-0000af30: 203d 2073 6f63 6b65 742e 6765 7468 6f73   = socket.gethos
-0000af40: 746e 616d 6528 290a 2020 2020 2020 2020  tname().        
-0000af50: 7365 6c66 2e63 6f6e 7461 6374 5b22 4973  self.contact["Is
-0000af60: 4f72 6967 696e 616c 225d 203d 2031 0a20  Original"] = 1. 
-0000af70: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-0000af80: 6163 745b 2249 4422 5d20 3d20 7575 6964  act["ID"] = uuid
-0000af90: 2e75 7569 6434 2829 2e68 6578 0a20 2020  .uuid4().hex.   
-0000afa0: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
-0000afb0: 742e 7365 745f 636f 6e74 6163 745f 7661  t.set_contact_va
-0000afc0: 7273 2873 656c 6629 0a20 2020 2020 2020  rs(self).       
-0000afd0: 2073 656c 662e 636f 6e74 6163 745b 2250   self.contact["P
-0000afe0: 6f69 6e74 7322 5d20 3d20 7365 6c66 2e63  oints"] = self.c
-0000aff0: 6f6e 7465 7374 2e70 6f69 6e74 7328 7365  ontest.points(se
-0000b000: 6c66 290a 2020 2020 2020 2020 6465 6275  lf).        debu
-0000b010: 675f 6f75 7470 7574 203d 2066 227b 7365  g_output = f"{se
-0000b020: 6c66 2e63 6f6e 7461 6374 7d22 0a20 2020  lf.contact}".   
-0000b030: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-0000b040: 6728 6465 6275 675f 6f75 7470 7574 290a  g(debug_output).
-0000b050: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000b060: 2e6e 316d 6d3a 0a20 2020 2020 2020 2020  .n1mm:.         
-0000b070: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-0000b080: 2270 6163 6b65 7473 2025 7322 2c20 6622  "packets %s", f"
-0000b090: 7b73 656c 662e 6e31 6d6d 2e73 656e 645f  {self.n1mm.send_
-0000b0a0: 636f 6e74 6163 745f 7061 636b 6574 737d  contact_packets}
-0000b0b0: 2229 0a20 2020 2020 2020 2020 2020 2069  ").            i
-0000b0c0: 6620 7365 6c66 2e6e 316d 6d2e 7365 6e64  f self.n1mm.send
-0000b0d0: 5f63 6f6e 7461 6374 5f70 6163 6b65 7473  _contact_packets
-0000b0e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000b0f0: 2020 7365 6c66 2e6e 316d 6d2e 636f 6e74    self.n1mm.cont
-0000b100: 6163 745f 696e 666f 5b22 7469 6d65 7374  act_info["timest
-0000b110: 616d 7022 5d20 3d20 7365 6c66 2e63 6f6e  amp"] = self.con
-0000b120: 7461 6374 5b22 5453 225d 0a20 2020 2020  tact["TS"].     
-0000b130: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b140: 6e31 6d6d 2e63 6f6e 7461 6374 5f69 6e66  n1mm.contact_inf
-0000b150: 6f5b 226f 6c64 6361 6c6c 225d 203d 2073  o["oldcall"] = s
-0000b160: 656c 662e 6e31 6d6d 2e63 6f6e 7461 6374  elf.n1mm.contact
-0000b170: 5f69 6e66 6f5b 0a20 2020 2020 2020 2020  _info[.         
-0000b180: 2020 2020 2020 2020 2020 2022 6361 6c6c             "call
-0000b190: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0000b1a0: 2020 5d20 3d20 7365 6c66 2e63 6f6e 7461    ] = self.conta
-0000b1b0: 6374 5b22 4361 6c6c 225d 0a20 2020 2020  ct["Call"].     
-0000b1c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b1d0: 6e31 6d6d 2e63 6f6e 7461 6374 5f69 6e66  n1mm.contact_inf
-0000b1e0: 6f5b 2274 7866 7265 7122 5d20 3d20 7365  o["txfreq"] = se
-0000b1f0: 6c66 2e6e 316d 6d2e 636f 6e74 6163 745f  lf.n1mm.contact_
-0000b200: 696e 666f 5b0a 2020 2020 2020 2020 2020  info[.          
-0000b210: 2020 2020 2020 2020 2020 2272 7866 7265            "rxfre
-0000b220: 7122 0a20 2020 2020 2020 2020 2020 2020  q".             
-0000b230: 2020 205d 203d 2073 656c 662e 6e31 6d6d     ] = self.n1mm
-0000b240: 2e72 6164 696f 5f69 6e66 6f5b 2246 7265  .radio_info["Fre
-0000b250: 7122 5d0a 2020 2020 2020 2020 2020 2020  q"].            
-0000b260: 2020 2020 7365 6c66 2e6e 316d 6d2e 636f      self.n1mm.co
-0000b270: 6e74 6163 745f 696e 666f 5b22 6d6f 6465  ntact_info["mode
-0000b280: 225d 203d 2073 656c 662e 636f 6e74 6163  "] = self.contac
-0000b290: 745b 224d 6f64 6522 5d0a 2020 2020 2020  t["Mode"].      
-0000b2a0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-0000b2b0: 316d 6d2e 636f 6e74 6163 745f 696e 666f  1mm.contact_info
-0000b2c0: 5b22 636f 6e74 6573 746e 616d 6522 5d20  ["contestname"] 
-0000b2d0: 3d20 7365 6c66 2e63 6f6e 7461 6374 5b0a  = self.contact[.
-0000b2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2f0: 2020 2020 2243 6f6e 7465 7374 4e61 6d65      "ContestName
-0000b300: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0000b310: 2020 5d2e 7265 706c 6163 6528 222d 222c    ].replace("-",
-0000b320: 2022 2229 0a20 2020 2020 2020 2020 2020   "").           
-0000b330: 2020 2020 2073 656c 662e 6e31 6d6d 2e63       self.n1mm.c
-0000b340: 6f6e 7461 6374 5f69 6e66 6f5b 2263 6f6e  ontact_info["con
-0000b350: 7465 7374 6e72 225d 203d 2073 656c 662e  testnr"] = self.
-0000b360: 636f 6e74 6163 745b 2243 6f6e 7465 7374  contact["Contest
-0000b370: 4e52 225d 0a20 2020 2020 2020 2020 2020  NR"].           
-0000b380: 2020 2020 2073 656c 662e 6e31 6d6d 2e63       self.n1mm.c
-0000b390: 6f6e 7461 6374 5f69 6e66 6f5b 2273 7461  ontact_info["sta
-0000b3a0: 7469 6f6e 7072 6566 6978 225d 203d 2073  tionprefix"] = s
-0000b3b0: 656c 662e 636f 6e74 6163 745b 2253 7461  elf.contact["Sta
-0000b3c0: 7469 6f6e 5072 6566 6978 225d 0a20 2020  tionPrefix"].   
-0000b3d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000b3e0: 662e 6e31 6d6d 2e63 6f6e 7461 6374 5f69  f.n1mm.contact_i
-0000b3f0: 6e66 6f5b 2277 7078 7072 6566 6978 225d  nfo["wpxprefix"]
-0000b400: 203d 2073 656c 662e 636f 6e74 6163 745b   = self.contact[
-0000b410: 2257 5058 5072 6566 6978 225d 0a20 2020  "WPXPrefix"].   
-0000b420: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000b430: 662e 6e31 6d6d 2e63 6f6e 7461 6374 5f69  f.n1mm.contact_i
-0000b440: 6e66 6f5b 2249 7352 756e 5153 4f22 5d20  nfo["IsRunQSO"] 
-0000b450: 3d20 7365 6c66 2e63 6f6e 7461 6374 5b22  = self.contact["
-0000b460: 4973 5275 6e51 534f 225d 0a20 2020 2020  IsRunQSO"].     
-0000b470: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b480: 6e31 6d6d 2e63 6f6e 7461 6374 5f69 6e66  n1mm.contact_inf
-0000b490: 6f5b 226f 7065 7261 746f 7222 5d20 3d20  o["operator"] = 
-0000b4a0: 7365 6c66 2e63 6f6e 7461 6374 5b22 4f70  self.contact["Op
-0000b4b0: 6572 6174 6f72 225d 0a20 2020 2020 2020  erator"].       
-0000b4c0: 2020 2020 2020 2020 2073 656c 662e 6e31           self.n1
-0000b4d0: 6d6d 2e63 6f6e 7461 6374 5f69 6e66 6f5b  mm.contact_info[
-0000b4e0: 226d 7963 616c 6c22 5d20 3d20 7365 6c66  "mycall"] = self
-0000b4f0: 2e63 6f6e 7461 6374 5b22 4f70 6572 6174  .contact["Operat
-0000b500: 6f72 225d 0a20 2020 2020 2020 2020 2020  or"].           
-0000b510: 2020 2020 2073 656c 662e 6e31 6d6d 2e63       self.n1mm.c
-0000b520: 6f6e 7461 6374 5f69 6e66 6f5b 2253 7461  ontact_info["Sta
-0000b530: 7469 6f6e 4e61 6d65 225d 203d 2073 656c  tionName"] = sel
-0000b540: 662e 6e31 6d6d 2e63 6f6e 7461 6374 5f69  f.n1mm.contact_i
-0000b550: 6e66 6f5b 0a20 2020 2020 2020 2020 2020  nfo[.           
-0000b560: 2020 2020 2020 2020 2022 4e65 7442 696f           "NetBio
-0000b570: 734e 616d 6522 0a20 2020 2020 2020 2020  sName".         
-0000b580: 2020 2020 2020 205d 203d 2073 656c 662e         ] = self.
-0000b590: 636f 6e74 6163 745b 224e 6574 4269 6f73  contact["NetBios
-0000b5a0: 4e61 6d65 225d 0a20 2020 2020 2020 2020  Name"].         
-0000b5b0: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
-0000b5c0: 2e63 6f6e 7461 6374 5f69 6e66 6f5b 2249  .contact_info["I
-0000b5d0: 734f 7269 6769 6e61 6c22 5d20 3d20 7365  sOriginal"] = se
-0000b5e0: 6c66 2e63 6f6e 7461 6374 5b22 4973 4f72  lf.contact["IsOr
-0000b5f0: 6967 696e 616c 225d 0a20 2020 2020 2020  iginal"].       
-0000b600: 2020 2020 2020 2020 2073 656c 662e 6e31           self.n1
-0000b610: 6d6d 2e63 6f6e 7461 6374 5f69 6e66 6f5b  mm.contact_info[
-0000b620: 2249 4422 5d20 3d20 7365 6c66 2e63 6f6e  "ID"] = self.con
-0000b630: 7461 6374 5b22 4944 225d 0a20 2020 2020  tact["ID"].     
-0000b640: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b650: 6e31 6d6d 2e63 6f6e 7461 6374 5f69 6e66  n1mm.contact_inf
-0000b660: 6f5b 2270 6f69 6e74 7322 5d20 3d20 7365  o["points"] = se
-0000b670: 6c66 2e63 6f6e 7461 6374 5b22 506f 696e  lf.contact["Poin
-0000b680: 7473 225d 0a20 2020 2020 2020 2020 2020  ts"].           
-0000b690: 2020 2020 2073 656c 662e 6e31 6d6d 2e63       self.n1mm.c
-0000b6a0: 6f6e 7461 6374 5f69 6e66 6f5b 2273 6e74  ontact_info["snt
-0000b6b0: 225d 203d 2073 656c 662e 636f 6e74 6163  "] = self.contac
-0000b6c0: 745b 2253 4e54 225d 0a20 2020 2020 2020  t["SNT"].       
-0000b6d0: 2020 2020 2020 2020 2073 656c 662e 6e31           self.n1
-0000b6e0: 6d6d 2e63 6f6e 7461 6374 5f69 6e66 6f5b  mm.contact_info[
-0000b6f0: 2272 6376 225d 203d 2073 656c 662e 636f  "rcv"] = self.co
-0000b700: 6e74 6163 745b 2252 4356 225d 0a20 2020  ntact["RCV"].   
-0000b710: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000b720: 662e 6e31 6d6d 2e63 6f6e 7461 6374 5f69  f.n1mm.contact_i
-0000b730: 6e66 6f5b 2273 6e74 6e72 225d 203d 2073  nfo["sntnr"] = s
-0000b740: 656c 662e 636f 6e74 6163 745b 2253 656e  elf.contact["Sen
-0000b750: 744e 7222 5d0a 2020 2020 2020 2020 2020  tNr"].          
-0000b760: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
-0000b770: 636f 6e74 6163 745f 696e 666f 5b22 7263  contact_info["rc
-0000b780: 766e 7222 5d20 3d20 7365 6c66 2e63 6f6e  vnr"] = self.con
-0000b790: 7461 6374 5b22 4e52 225d 0a20 2020 2020  tact["NR"].     
-0000b7a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b7b0: 6e31 6d6d 2e63 6f6e 7461 6374 5f69 6e66  n1mm.contact_inf
-0000b7c0: 6f5b 2269 736d 756c 7469 706c 6965 7231  o["ismultiplier1
-0000b7d0: 225d 203d 2073 656c 662e 636f 6e74 6163  "] = self.contac
-0000b7e0: 742e 6765 7428 0a20 2020 2020 2020 2020  t.get(.         
-0000b7f0: 2020 2020 2020 2020 2020 2022 4973 4d75             "IsMu
-0000b800: 6c74 6970 6c69 6572 3122 2c20 300a 2020  ltiplier1", 0.  
-0000b810: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0000b820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b830: 7365 6c66 2e6e 316d 6d2e 636f 6e74 6163  self.n1mm.contac
-0000b840: 745f 696e 666f 5b22 6973 6d75 6c74 6970  t_info["ismultip
-0000b850: 6c69 6572 3222 5d20 3d20 7365 6c66 2e63  lier2"] = self.c
-0000b860: 6f6e 7461 6374 2e67 6574 280a 2020 2020  ontact.get(.    
-0000b870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b880: 2249 734d 756c 7469 706c 6965 7232 222c  "IsMultiplier2",
-0000b890: 2030 0a20 2020 2020 2020 2020 2020 2020   0.             
-0000b8a0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0000b8b0: 2020 2020 2073 656c 662e 6e31 6d6d 2e63       self.n1mm.c
-0000b8c0: 6f6e 7461 6374 5f69 6e66 6f5b 2269 736d  ontact_info["ism
-0000b8d0: 756c 7469 706c 6965 7233 225d 203d 2073  ultiplier3"] = s
-0000b8e0: 656c 662e 636f 6e74 6163 742e 6765 7428  elf.contact.get(
-0000b8f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b900: 2020 2020 2022 4973 4d75 6c74 6970 6c69       "IsMultipli
-0000b910: 6572 3322 2c20 2230 220a 2020 2020 2020  er3", "0".      
-0000b920: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000b930: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000b940: 2e6e 316d 6d2e 636f 6e74 6163 745f 696e  .n1mm.contact_in
-0000b950: 666f 5b22 7365 6374 696f 6e22 5d20 3d20  fo["section"] = 
-0000b960: 7365 6c66 2e63 6f6e 7461 6374 5b22 5365  self.contact["Se
-0000b970: 6374 225d 0a20 2020 2020 2020 2020 2020  ct"].           
-0000b980: 2020 2020 2073 656c 662e 6e31 6d6d 2e63       self.n1mm.c
-0000b990: 6f6e 7461 6374 5f69 6e66 6f5b 2270 7265  ontact_info["pre
-0000b9a0: 6322 5d20 3d20 7365 6c66 2e63 6f6e 7461  c"] = self.conta
-0000b9b0: 6374 5b22 5072 6563 225d 0a20 2020 2020  ct["Prec"].     
-0000b9c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000b9d0: 6e31 6d6d 2e63 6f6e 7461 6374 5f69 6e66  n1mm.contact_inf
-0000b9e0: 6f5b 2263 6b22 5d20 3d20 7365 6c66 2e63  o["ck"] = self.c
-0000b9f0: 6f6e 7461 6374 5b22 434b 225d 0a20 2020  ontact["CK"].   
-0000ba00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000ba10: 662e 6e31 6d6d 2e63 6f6e 7461 6374 5f69  f.n1mm.contact_i
-0000ba20: 6e66 6f5b 227a 6e22 5d20 3d20 7365 6c66  nfo["zn"] = self
-0000ba30: 2e63 6f6e 7461 6374 5b22 5a4e 225d 0a20  .contact["ZN"]. 
-0000ba40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000ba50: 656c 662e 6e31 6d6d 2e63 6f6e 7461 6374  elf.n1mm.contact
-0000ba60: 5f69 6e66 6f5b 2270 6f77 6572 225d 203d  _info["power"] =
-0000ba70: 2073 656c 662e 636f 6e74 6163 745b 2250   self.contact["P
-0000ba80: 6f77 6572 225d 0a20 2020 2020 2020 2020  ower"].         
-0000ba90: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
-0000baa0: 2e63 6f6e 7461 6374 5f69 6e66 6f5b 2262  .contact_info["b
-0000bab0: 616e 6422 5d20 3d20 7365 6c66 2e63 6f6e  and"] = self.con
-0000bac0: 7461 6374 5b22 4261 6e64 225d 0a20 2020  tact["Band"].   
-0000bad0: 2020 2020 2020 2020 2020 2020 2023 2073               # s
-0000bae0: 656c 662e 6e31 6d6d 2e63 6f6e 7461 6374  elf.n1mm.contact
-0000baf0: 5f69 6e66 6f5b 2727 5d0a 2020 2020 2020  _info[''].      
-0000bb00: 2020 2020 2020 2020 2020 2320 7365 6c66            # self
-0000bb10: 2e6e 316d 6d2e 636f 6e74 6163 745f 696e  .n1mm.contact_in
-0000bb20: 666f 5b27 275d 0a20 2020 2020 2020 2020  fo[''].         
-0000bb30: 2020 2020 2020 2023 2073 656c 662e 6e31         # self.n1
-0000bb40: 6d6d 2e63 6f6e 7461 6374 5f69 6e66 6f5b  mm.contact_info[
-0000bb50: 2727 5d0a 2020 2020 2020 2020 2020 2020  ''].            
-0000bb60: 2020 2020 2320 7365 6c66 2e6e 316d 6d2e      # self.n1mm.
-0000bb70: 636f 6e74 6163 745f 696e 666f 5b27 275d  contact_info['']
-0000bb80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bb90: 2023 2073 656c 662e 6e31 6d6d 2e63 6f6e   # self.n1mm.con
-0000bba0: 7461 6374 5f69 6e66 6f5b 2727 5d0a 2020  tact_info[''].  
-0000bbb0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000bbc0: 7365 6c66 2e6e 316d 6d2e 636f 6e74 6163  self.n1mm.contac
-0000bbd0: 745f 696e 666f 5b27 275d 0a20 2020 2020  t_info[''].     
-0000bbe0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-0000bbf0: 722e 6465 6275 6728 2225 7322 2c20 6622  r.debug("%s", f"
-0000bc00: 7b73 656c 662e 6e31 6d6d 2e63 6f6e 7461  {self.n1mm.conta
-0000bc10: 6374 5f69 6e66 6f7d 2229 0a20 2020 2020  ct_info}").     
-0000bc20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000bc30: 6e31 6d6d 2e73 656e 645f 636f 6e74 6163  n1mm.send_contac
-0000bc40: 745f 696e 666f 2829 0a0a 2020 2020 2020  t_info()..      
-0000bc50: 2020 7365 6c66 2e64 6174 6162 6173 652e    self.database.
-0000bc60: 6c6f 675f 636f 6e74 6163 7428 7365 6c66  log_contact(self
-0000bc70: 2e63 6f6e 7461 6374 290a 2020 2020 2020  .contact).      
-0000bc80: 2020 7365 6c66 2e77 6f72 6b65 645f 6c69    self.worked_li
-0000bc90: 7374 203d 2073 656c 662e 6461 7461 6261  st = self.databa
-0000bca0: 7365 2e67 6574 5f63 616c 6c73 5f61 6e64  se.get_calls_and
-0000bcb0: 5f62 616e 6473 2829 0a20 2020 2020 2020  _bands().       
-0000bcc0: 2073 656c 662e 7365 6e64 5f77 6f72 6b65   self.send_worke
-0000bcd0: 645f 6c69 7374 2829 0a20 2020 2020 2020  d_list().       
-0000bce0: 2073 656c 662e 636c 6561 7269 6e70 7574   self.clearinput
-0000bcf0: 7328 290a 0a20 2020 2020 2020 2063 6d64  s()..        cmd
-0000bd00: 203d 207b 7d0a 2020 2020 2020 2020 636d   = {}.        cm
-0000bd10: 645b 2263 6d64 225d 203d 2022 5550 4441  d["cmd"] = "UPDA
-0000bd20: 5445 4c4f 4722 0a20 2020 2020 2020 2063  TELOG".        c
-0000bd30: 6d64 5b22 7374 6174 696f 6e22 5d20 3d20  md["station"] = 
-0000bd40: 706c 6174 666f 726d 2e6e 6f64 6528 290a  platform.node().
-0000bd50: 2020 2020 2020 2020 7365 6c66 2e6d 756c          self.mul
-0000bd60: 7469 6361 7374 5f69 6e74 6572 6661 6365  ticast_interface
-0000bd70: 2e73 656e 645f 6173 5f6a 736f 6e28 636d  .send_as_json(cm
-0000bd80: 6429 0a0a 2020 2020 2020 2020 2320 7365  d)..        # se
-0000bd90: 6c66 2e63 6f6e 7461 6374 5b22 436f 6e74  lf.contact["Cont
-0000bda0: 6573 744e 616d 6522 5d20 3d20 7365 6c66  estName"] = self
-0000bdb0: 2e63 6f6e 7465 7374 2e6e 616d 650a 2020  .contest.name.  
-0000bdc0: 2020 2020 2020 2320 7365 6c66 2e63 6f6e        # self.con
-0000bdd0: 7461 6374 5b22 534e 5422 5d20 3d20 7365  tact["SNT"] = se
-0000bde0: 6c66 2e73 656e 742e 7465 7874 2829 0a20  lf.sent.text(). 
-0000bdf0: 2020 2020 2020 2023 2073 656c 662e 636f         # self.co
-0000be00: 6e74 6163 745b 2252 4356 225d 203d 2073  ntact["RCV"] = s
-0000be10: 656c 662e 7265 6365 6976 652e 7465 7874  elf.receive.text
-0000be20: 2829 0a20 2020 2020 2020 2023 2073 656c  ().        # sel
-0000be30: 662e 636f 6e74 6163 745b 2243 6f75 6e74  f.contact["Count
-0000be40: 7279 5072 6566 6978 225d 0a20 2020 2020  ryPrefix"].     
-0000be50: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
-0000be60: 745b 2253 7461 7469 6f6e 5072 6566 6978  t["StationPrefix
-0000be70: 225d 203d 2073 656c 662e 7072 6566 2e67  "] = self.pref.g
-0000be80: 6574 2822 6361 6c6c 7369 676e 222c 2022  et("callsign", "
-0000be90: 2229 0a20 2020 2020 2020 2023 2073 656c  ").        # sel
-0000bea0: 662e 636f 6e74 6163 745b 2251 5448 225d  f.contact["QTH"]
-0000beb0: 0a20 2020 2020 2020 2023 2073 656c 662e  .        # self.
-0000bec0: 636f 6e74 6163 745b 224e 616d 6522 5d20  contact["Name"] 
-0000bed0: 3d20 7365 6c66 2e6f 7468 6572 5f31 2e74  = self.other_1.t
-0000bee0: 6578 7428 290a 2020 2020 2020 2020 2320  ext().        # 
-0000bef0: 7365 6c66 2e63 6f6e 7461 6374 5b22 436f  self.contact["Co
-0000bf00: 6d6d 656e 7422 5d20 3d20 7365 6c66 2e6f  mment"] = self.o
-0000bf10: 7468 6572 5f32 2e74 6578 7428 290a 2020  ther_2.text().  
-0000bf20: 2020 2020 2020 2320 7365 6c66 2e63 6f6e        # self.con
-0000bf30: 7461 6374 5b22 4e52 225d 0a20 2020 2020  tact["NR"].     
-0000bf40: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
-0000bf50: 745b 2253 6563 7422 5d0a 2020 2020 2020  t["Sect"].      
-0000bf60: 2020 2320 7365 6c66 2e63 6f6e 7461 6374    # self.contact
-0000bf70: 5b22 5072 6563 225d 0a20 2020 2020 2020  ["Prec"].       
-0000bf80: 2023 2073 656c 662e 636f 6e74 6163 745b   # self.contact[
-0000bf90: 2243 4b22 5d0a 2020 2020 2020 2020 2320  "CK"].        # 
-0000bfa0: 7365 6c66 2e63 6f6e 7461 6374 5b22 5a4e  self.contact["ZN
-0000bfb0: 225d 0a20 2020 2020 2020 2023 2073 656c  "].        # sel
-0000bfc0: 662e 636f 6e74 6163 745b 2253 656e 744e  f.contact["SentN
-0000bfd0: 7222 5d0a 2020 2020 2020 2020 2320 7365  r"].        # se
-0000bfe0: 6c66 2e63 6f6e 7461 6374 5b22 506f 696e  lf.contact["Poin
-0000bff0: 7473 225d 0a20 2020 2020 2020 2023 2073  ts"].        # s
-0000c000: 656c 662e 636f 6e74 6163 745b 2249 734d  elf.contact["IsM
-0000c010: 756c 7469 706c 6965 7231 225d 0a20 2020  ultiplier1"].   
-0000c020: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
-0000c030: 6163 745b 2249 734d 756c 7469 706c 6965  act["IsMultiplie
-0000c040: 7232 225d 0a20 2020 2020 2020 2023 2073  r2"].        # s
-0000c050: 656c 662e 636f 6e74 6163 745b 2250 6f77  elf.contact["Pow
-0000c060: 6572 225d 0a20 2020 2020 2020 2023 2073  er"].        # s
-0000c070: 656c 662e 636f 6e74 6163 745b 2242 616e  elf.contact["Ban
-0000c080: 6422 5d0a 2020 2020 2020 2020 2320 7365  d"].        # se
-0000c090: 6c66 2e63 6f6e 7461 6374 5b22 5750 5850  lf.contact["WPXP
-0000c0a0: 7265 6669 7822 5d20 3d20 6361 6c63 756c  refix"] = calcul
-0000c0b0: 6174 655f 7770 785f 7072 6566 6978 2873  ate_wpx_prefix(s
-0000c0c0: 656c 662e 6361 6c6c 7369 676e 2e74 6578  elf.callsign.tex
-0000c0d0: 7428 2929 0a20 2020 2020 2020 2023 2073  t()).        # s
-0000c0e0: 656c 662e 636f 6e74 6163 745b 2245 7863  elf.contact["Exc
-0000c0f0: 6861 6e67 6531 225d 0a20 2020 2020 2020  hange1"].       
-0000c100: 2023 2073 656c 662e 636f 6e74 6163 745b   # self.contact[
-0000c110: 2252 6164 696f 4e52 225d 0a20 2020 2020  "RadioNR"].     
-0000c120: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
-0000c130: 745b 2269 734d 756c 7469 706c 6965 7233  t["isMultiplier3
-0000c140: 225d 0a20 2020 2020 2020 2023 2073 656c  "].        # sel
-0000c150: 662e 636f 6e74 6163 745b 224d 6973 6354  f.contact["MiscT
-0000c160: 6578 7422 5d0a 2020 2020 2020 2020 2320  ext"].        # 
-0000c170: 7365 6c66 2e63 6f6e 7461 6374 5b22 436f  self.contact["Co
-0000c180: 6e74 6163 7454 7970 6522 5d0a 2020 2020  ntactType"].    
-0000c190: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
-0000c1a0: 6374 5b22 5275 6e31 5275 6e32 225d 0a20  ct["Run1Run2"]. 
-0000c1b0: 2020 2020 2020 2023 2073 656c 662e 636f         # self.co
-0000c1c0: 6e74 6163 745b 2247 7269 6453 7175 6172  ntact["GridSquar
-0000c1d0: 6522 5d0a 2020 2020 2020 2020 2320 7365  e"].        # se
-0000c1e0: 6c66 2e63 6f6e 7461 6374 5b22 436f 6e74  lf.contact["Cont
-0000c1f0: 696e 656e 7422 5d0a 2020 2020 2020 2020  inent"].        
-0000c200: 2320 7365 6c66 2e63 6f6e 7461 6374 5b22  # self.contact["
-0000c210: 526f 7665 724c 6f63 6174 696f 6e22 5d0a  RoverLocation"].
-0000c220: 2020 2020 2020 2020 2320 7365 6c66 2e63          # self.c
-0000c230: 6f6e 7461 6374 5b22 5261 6469 6f49 6e74  ontact["RadioInt
-0000c240: 6572 6661 6365 6422 5d0a 2020 2020 2020  erfaced"].      
-0000c250: 2020 2320 7365 6c66 2e63 6f6e 7461 6374    # self.contact
-0000c260: 5b22 4e65 7477 6f72 6b65 6443 6f6d 704e  ["NetworkedCompN
-0000c270: 7222 5d0a 2020 2020 2020 2020 2320 7365  r"].        # se
-0000c280: 6c66 2e63 6f6e 7461 6374 5b22 434c 4149  lf.contact["CLAI
-0000c290: 4d45 4451 534f 225d 0a0a 2020 2020 6465  MEDQSO"]..    de
-0000c2a0: 6620 6e65 775f 636f 6e74 6573 745f 6469  f new_contest_di
-0000c2b0: 616c 6f67 2873 656c 6629 3a0a 2020 2020  alog(self):.    
-0000c2c0: 2020 2020 2222 2253 686f 7720 6e65 7720      """Show new 
-0000c2d0: 636f 6e74 6573 7420 6469 616c 6f67 2222  contest dialog""
-0000c2e0: 220a 2020 2020 2020 2020 6c6f 6767 6572  ".        logger
-0000c2f0: 2e64 6562 7567 2822 4e65 7720 636f 6e74  .debug("New cont
-0000c300: 6573 7420 4469 616c 6f67 2229 0a20 2020  est Dialog").   
-0000c310: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
-0000c320: 745f 6469 616c 6f67 203d 204e 6577 436f  t_dialog = NewCo
-0000c330: 6e74 6573 7428 574f 524b 494e 475f 5041  ntest(WORKING_PA
-0000c340: 5448 290a 2020 2020 2020 2020 7365 6c66  TH).        self
-0000c350: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
-0000c360: 6163 6365 7074 6564 2e63 6f6e 6e65 6374  accepted.connect
-0000c370: 2873 656c 662e 7361 7665 5f63 6f6e 7465  (self.save_conte
-0000c380: 7374 290a 2020 2020 2020 2020 7365 6c66  st).        self
-0000c390: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
-0000c3a0: 6461 7465 5469 6d65 4564 6974 2e73 6574  dateTimeEdit.set
-0000c3b0: 4461 7465 2851 7443 6f72 652e 5144 6174  Date(QtCore.QDat
-0000c3c0: 652e 6375 7272 656e 7444 6174 6528 2929  e.currentDate())
-0000c3d0: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-0000c3e0: 6e74 6573 745f 6469 616c 6f67 2e64 6174  ntest_dialog.dat
-0000c3f0: 6554 696d 6545 6469 742e 7365 7443 616c  eTimeEdit.setCal
-0000c400: 656e 6461 7250 6f70 7570 2854 7275 6529  endarPopup(True)
-0000c410: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-0000c420: 6e74 6573 745f 6469 616c 6f67 2e64 6174  ntest_dialog.dat
-0000c430: 6554 696d 6545 6469 742e 7365 7454 696d  eTimeEdit.setTim
-0000c440: 6528 5174 436f 7265 2e51 5469 6d65 2830  e(QtCore.QTime(0
-0000c450: 2c20 3029 290a 2020 2020 2020 2020 7365  , 0)).        se
-0000c460: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-0000c470: 672e 706f 7765 722e 7365 7443 7572 7265  g.power.setCurre
-0000c480: 6e74 5465 7874 2822 4c4f 5722 290a 2020  ntText("LOW").  
-0000c490: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
-0000c4a0: 7374 5f64 6961 6c6f 672e 7374 6174 696f  st_dialog.statio
-0000c4b0: 6e2e 7365 7443 7572 7265 6e74 5465 7874  n.setCurrentText
-0000c4c0: 2822 4649 5845 4422 290a 2020 2020 2020  ("FIXED").      
-0000c4d0: 2020 7365 6c66 2e63 6f6e 7465 7374 5f64    self.contest_d
-0000c4e0: 6961 6c6f 672e 6f70 656e 2829 0a0a 2020  ialog.open()..  
-0000c4f0: 2020 6465 6620 7361 7665 5f63 6f6e 7465    def save_conte
-0000c500: 7374 2873 656c 6629 3a0a 2020 2020 2020  st(self):.      
-0000c510: 2020 2222 2253 6176 6520 436f 6e74 6573    """Save Contes
-0000c520: 7422 2222 0a20 2020 2020 2020 206e 6578  t""".        nex
-0000c530: 745f 6e75 6d62 6572 203d 2073 656c 662e  t_number = self.
-0000c540: 6461 7461 6261 7365 2e67 6574 5f6e 6578  database.get_nex
-0000c550: 745f 636f 6e74 6573 745f 6e72 2829 0a20  t_contest_nr(). 
-0000c560: 2020 2020 2020 2063 6f6e 7465 7374 203d         contest =
-0000c570: 207b 7d0a 2020 2020 2020 2020 636f 6e74   {}.        cont
-0000c580: 6573 745b 2243 6f6e 7465 7374 4e61 6d65  est["ContestName
-0000c590: 225d 203d 2028 0a20 2020 2020 2020 2020  "] = (.         
-0000c5a0: 2020 2073 656c 662e 636f 6e74 6573 745f     self.contest_
-0000c5b0: 6469 616c 6f67 2e63 6f6e 7465 7374 2e63  dialog.contest.c
-0000c5c0: 7572 7265 6e74 5465 7874 2829 2e6c 6f77  urrentText().low
-0000c5d0: 6572 2829 2e72 6570 6c61 6365 2822 2022  er().replace(" "
-0000c5e0: 2c20 225f 2229 0a20 2020 2020 2020 2029  , "_").        )
-0000c5f0: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
-0000c600: 5b22 5374 6172 7444 6174 6522 5d20 3d20  ["StartDate"] = 
-0000c610: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
-0000c620: 6c6f 672e 6461 7465 5469 6d65 4564 6974  log.dateTimeEdit
-0000c630: 2e64 6174 6554 696d 6528 292e 746f 5374  .dateTime().toSt
-0000c640: 7269 6e67 280a 2020 2020 2020 2020 2020  ring(.          
-0000c650: 2020 2279 7979 792d 4d4d 2d64 6420 6868    "yyyy-MM-dd hh
-0000c660: 3a6d 6d3a 7373 220a 2020 2020 2020 2020  :mm:ss".        
-0000c670: 290a 2020 2020 2020 2020 636f 6e74 6573  ).        contes
-0000c680: 745b 224f 7065 7261 746f 7243 6174 6567  t["OperatorCateg
-0000c690: 6f72 7922 5d20 3d20 7365 6c66 2e63 6f6e  ory"] = self.con
-0000c6a0: 7465 7374 5f64 6961 6c6f 672e 6f70 6572  test_dialog.oper
-0000c6b0: 6174 6f72 5f63 6c61 7373 2e63 7572 7265  ator_class.curre
-0000c6c0: 6e74 5465 7874 2829 0a20 2020 2020 2020  ntText().       
-0000c6d0: 2063 6f6e 7465 7374 5b22 4261 6e64 4361   contest["BandCa
-0000c6e0: 7465 676f 7279 225d 203d 2073 656c 662e  tegory"] = self.
-0000c6f0: 636f 6e74 6573 745f 6469 616c 6f67 2e62  contest_dialog.b
-0000c700: 616e 642e 6375 7272 656e 7454 6578 7428  and.currentText(
-0000c710: 290a 2020 2020 2020 2020 636f 6e74 6573  ).        contes
-0000c720: 745b 2250 6f77 6572 4361 7465 676f 7279  t["PowerCategory
-0000c730: 225d 203d 2073 656c 662e 636f 6e74 6573  "] = self.contes
-0000c740: 745f 6469 616c 6f67 2e70 6f77 6572 2e63  t_dialog.power.c
-0000c750: 7572 7265 6e74 5465 7874 2829 0a20 2020  urrentText().   
-0000c760: 2020 2020 2063 6f6e 7465 7374 5b22 4d6f       contest["Mo
-0000c770: 6465 4361 7465 676f 7279 225d 203d 2073  deCategory"] = s
-0000c780: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-0000c790: 6f67 2e6d 6f64 652e 6375 7272 656e 7454  og.mode.currentT
-0000c7a0: 6578 7428 290a 2020 2020 2020 2020 636f  ext().        co
-0000c7b0: 6e74 6573 745b 224f 7665 726c 6179 4361  ntest["OverlayCa
-0000c7c0: 7465 676f 7279 225d 203d 2073 656c 662e  tegory"] = self.
-0000c7d0: 636f 6e74 6573 745f 6469 616c 6f67 2e6f  contest_dialog.o
-0000c7e0: 7665 726c 6179 2e63 7572 7265 6e74 5465  verlay.currentTe
-0000c7f0: 7874 2829 0a20 2020 2020 2020 2023 2063  xt().        # c
-0000c800: 6f6e 7465 7374 5b27 436c 6169 6d65 6453  ontest['ClaimedS
-0000c810: 636f 7265 275d 203d 2073 656c 662e 636f  core'] = self.co
-0000c820: 6e74 6573 745f 6469 616c 6f67 2e0a 2020  ntest_dialog..  
-0000c830: 2020 2020 2020 636f 6e74 6573 745b 224f        contest["O
-0000c840: 7065 7261 746f 7273 225d 203d 2073 656c  perators"] = sel
-0000c850: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
-0000c860: 2e6f 7065 7261 746f 7273 2e74 6578 7428  .operators.text(
-0000c870: 290a 2020 2020 2020 2020 636f 6e74 6573  ).        contes
-0000c880: 745b 2253 6f61 7062 6f78 225d 203d 2073  t["Soapbox"] = s
-0000c890: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
-0000c8a0: 6f67 2e73 6f61 7062 6f78 2e74 6f50 6c61  og.soapbox.toPla
-0000c8b0: 696e 5465 7874 2829 0a20 2020 2020 2020  inText().       
-0000c8c0: 2063 6f6e 7465 7374 5b22 5365 6e74 4578   contest["SentEx
-0000c8d0: 6368 616e 6765 225d 203d 2073 656c 662e  change"] = self.
-0000c8e0: 636f 6e74 6573 745f 6469 616c 6f67 2e65  contest_dialog.e
-0000c8f0: 7863 6861 6e67 652e 7465 7874 2829 0a20  xchange.text(). 
-0000c900: 2020 2020 2020 2063 6f6e 7465 7374 5b22         contest["
-0000c910: 436f 6e74 6573 744e 5222 5d20 3d20 6e65  ContestNR"] = ne
-0000c920: 7874 5f6e 756d 6265 722e 6765 7428 2263  xt_number.get("c
-0000c930: 6f75 6e74 222c 2031 290a 2020 2020 2020  ount", 1).      
-0000c940: 2020 7365 6c66 2e70 7265 665b 2263 6f6e    self.pref["con
-0000c950: 7465 7374 225d 203d 206e 6578 745f 6e75  test"] = next_nu
-0000c960: 6d62 6572 2e67 6574 2822 636f 756e 7422  mber.get("count"
-0000c970: 2c20 3129 0a20 2020 2020 2020 2023 2063  , 1).        # c
-0000c980: 6f6e 7465 7374 5b27 5375 6254 7970 6527  ontest['SubType'
-0000c990: 5d20 3d20 7365 6c66 2e63 6f6e 7465 7374  ] = self.contest
-0000c9a0: 5f64 6961 6c6f 672e 0a20 2020 2020 2020  _dialog..       
-0000c9b0: 2063 6f6e 7465 7374 5b22 5374 6174 696f   contest["Statio
-0000c9c0: 6e43 6174 6567 6f72 7922 5d20 3d20 7365  nCategory"] = se
-0000c9d0: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-0000c9e0: 672e 7374 6174 696f 6e2e 6375 7272 656e  g.station.curren
-0000c9f0: 7454 6578 7428 290a 2020 2020 2020 2020  tText().        
-0000ca00: 636f 6e74 6573 745b 2241 7373 6973 7465  contest["Assiste
-0000ca10: 6443 6174 6567 6f72 7922 5d20 3d20 7365  dCategory"] = se
-0000ca20: 6c66 2e63 6f6e 7465 7374 5f64 6961 6c6f  lf.contest_dialo
-0000ca30: 672e 6173 7369 7374 6564 2e63 7572 7265  g.assisted.curre
-0000ca40: 6e74 5465 7874 2829 0a20 2020 2020 2020  ntText().       
-0000ca50: 2063 6f6e 7465 7374 5b22 5472 616e 736d   contest["Transm
-0000ca60: 6974 7465 7243 6174 6567 6f72 7922 5d20  itterCategory"] 
-0000ca70: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f64  = self.contest_d
-0000ca80: 6961 6c6f 672e 7472 616e 736d 6974 7465  ialog.transmitte
-0000ca90: 722e 6375 7272 656e 7454 6578 7428 290a  r.currentText().
-0000caa0: 2020 2020 2020 2020 2320 636f 6e74 6573          # contes
-0000cab0: 745b 2754 696d 6543 6174 6567 6f72 7927  t['TimeCategory'
-0000cac0: 5d20 3d20 7365 6c66 2e63 6f6e 7465 7374  ] = self.contest
-0000cad0: 5f64 6961 6c6f 672e 0a20 2020 2020 2020  _dialog..       
-0000cae0: 206c 6f67 6765 722e 6465 6275 6728 2225   logger.debug("%
-0000caf0: 7322 2c20 6622 7b63 6f6e 7465 7374 7d22  s", f"{contest}"
-0000cb00: 290a 2020 2020 2020 2020 7365 6c66 2e64  ).        self.d
-0000cb10: 6174 6162 6173 652e 6164 645f 636f 6e74  atabase.add_cont
-0000cb20: 6573 7428 636f 6e74 6573 7429 0a20 2020  est(contest).   
-0000cb30: 2020 2020 2073 656c 662e 7772 6974 655f       self.write_
-0000cb40: 7072 6566 6572 656e 6365 2829 0a20 2020  preference().   
-0000cb50: 2020 2020 2073 656c 662e 6c6f 6164 5f63       self.load_c
-0000cb60: 6f6e 7465 7374 2829 0a0a 2020 2020 6465  ontest()..    de
-0000cb70: 6620 6564 6974 5f73 7461 7469 6f6e 5f73  f edit_station_s
-0000cb80: 6574 7469 6e67 7328 7365 6c66 293a 0a20  ettings(self):. 
-0000cb90: 2020 2020 2020 2022 2222 5368 6f77 2073         """Show s
-0000cba0: 6574 7469 6e67 7320 6469 616c 6f67 2222  ettings dialog""
-0000cbb0: 220a 2020 2020 2020 2020 6c6f 6767 6572  ".        logger
-0000cbc0: 2e64 6562 7567 2822 5374 6174 696f 6e20  .debug("Station 
-0000cbd0: 5365 7474 696e 6773 2073 656c 6563 7465  Settings selecte
-0000cbe0: 6422 290a 2020 2020 2020 2020 7365 6c66  d").        self
-0000cbf0: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
-0000cc00: 203d 2045 6469 7453 7461 7469 6f6e 2857   = EditStation(W
-0000cc10: 4f52 4b49 4e47 5f50 4154 4829 0a20 2020  ORKING_PATH).   
-0000cc20: 2020 2020 2073 656c 662e 7365 7474 696e       self.settin
-0000cc30: 6773 5f64 6961 6c6f 672e 6163 6365 7074  gs_dialog.accept
-0000cc40: 6564 2e63 6f6e 6e65 6374 2873 656c 662e  ed.connect(self.
-0000cc50: 7361 7665 5f73 6574 7469 6e67 7329 0a20  save_settings). 
-0000cc60: 2020 2020 2020 2073 656c 662e 7365 7474         self.sett
-0000cc70: 696e 6773 5f64 6961 6c6f 672e 4361 6c6c  ings_dialog.Call
-0000cc80: 2e73 6574 5465 7874 2873 656c 662e 7374  .setText(self.st
-0000cc90: 6174 696f 6e2e 6765 7428 2243 616c 6c22  ation.get("Call"
-0000cca0: 2c20 2222 2929 0a20 2020 2020 2020 2073  , "")).        s
-0000ccb0: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
-0000ccc0: 6c6f 672e 4e61 6d65 2e73 6574 5465 7874  log.Name.setText
-0000ccd0: 2873 656c 662e 7374 6174 696f 6e2e 6765  (self.station.ge
-0000cce0: 7428 224e 616d 6522 2c20 2222 2929 0a20  t("Name", "")). 
-0000ccf0: 2020 2020 2020 2073 656c 662e 7365 7474         self.sett
-0000cd00: 696e 6773 5f64 6961 6c6f 672e 4164 6472  ings_dialog.Addr
-0000cd10: 6573 7331 2e73 6574 5465 7874 2873 656c  ess1.setText(sel
-0000cd20: 662e 7374 6174 696f 6e2e 6765 7428 2253  f.station.get("S
-0000cd30: 7472 6565 7431 222c 2022 2229 290a 2020  treet1", "")).  
-0000cd40: 2020 2020 2020 7365 6c66 2e73 6574 7469        self.setti
-0000cd50: 6e67 735f 6469 616c 6f67 2e41 6464 7265  ngs_dialog.Addre
-0000cd60: 7373 322e 7365 7454 6578 7428 7365 6c66  ss2.setText(self
-0000cd70: 2e73 7461 7469 6f6e 2e67 6574 2822 5374  .station.get("St
-0000cd80: 7265 6574 3222 2c20 2222 2929 0a20 2020  reet2", "")).   
-0000cd90: 2020 2020 2073 656c 662e 7365 7474 696e       self.settin
-0000cda0: 6773 5f64 6961 6c6f 672e 4369 7479 2e73  gs_dialog.City.s
-0000cdb0: 6574 5465 7874 2873 656c 662e 7374 6174  etText(self.stat
-0000cdc0: 696f 6e2e 6765 7428 2243 6974 7922 2c20  ion.get("City", 
-0000cdd0: 2222 2929 0a20 2020 2020 2020 2073 656c  "")).        sel
-0000cde0: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
-0000cdf0: 672e 5374 6174 652e 7365 7454 6578 7428  g.State.setText(
-0000ce00: 7365 6c66 2e73 7461 7469 6f6e 2e67 6574  self.station.get
-0000ce10: 2822 5374 6174 6522 2c20 2222 2929 0a20  ("State", "")). 
-0000ce20: 2020 2020 2020 2073 656c 662e 7365 7474         self.sett
-0000ce30: 696e 6773 5f64 6961 6c6f 672e 5a69 702e  ings_dialog.Zip.
-0000ce40: 7365 7454 6578 7428 7365 6c66 2e73 7461  setText(self.sta
-0000ce50: 7469 6f6e 2e67 6574 2822 5a69 7022 2c20  tion.get("Zip", 
-0000ce60: 2222 2929 0a20 2020 2020 2020 2073 656c  "")).        sel
-0000ce70: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
-0000ce80: 672e 436f 756e 7472 792e 7365 7454 6578  g.Country.setTex
-0000ce90: 7428 7365 6c66 2e73 7461 7469 6f6e 2e67  t(self.station.g
-0000cea0: 6574 2822 436f 756e 7472 7922 2c20 2222  et("Country", ""
-0000ceb0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-0000cec0: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
-0000ced0: 4772 6964 5371 7561 7265 2e73 6574 5465  GridSquare.setTe
-0000cee0: 7874 2873 656c 662e 7374 6174 696f 6e2e  xt(self.station.
-0000cef0: 6765 7428 2247 7269 6453 7175 6172 6522  get("GridSquare"
-0000cf00: 2c20 2222 2929 0a20 2020 2020 2020 2073  , "")).        s
-0000cf10: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
-0000cf20: 6c6f 672e 4351 5a6f 6e65 2e73 6574 5465  log.CQZone.setTe
-0000cf30: 7874 2873 7472 2873 656c 662e 7374 6174  xt(str(self.stat
-0000cf40: 696f 6e2e 6765 7428 2243 515a 6f6e 6522  ion.get("CQZone"
-0000cf50: 2c20 2222 2929 290a 2020 2020 2020 2020  , ""))).        
-0000cf60: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
-0000cf70: 616c 6f67 2e49 5455 5a6f 6e65 2e73 6574  alog.ITUZone.set
-0000cf80: 5465 7874 2873 7472 2873 656c 662e 7374  Text(str(self.st
-0000cf90: 6174 696f 6e2e 6765 7428 2249 4152 555a  ation.get("IARUZ
-0000cfa0: 6f6e 6522 2c20 2222 2929 290a 2020 2020  one", ""))).    
-0000cfb0: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
-0000cfc0: 735f 6469 616c 6f67 2e4c 6963 656e 7365  s_dialog.License
-0000cfd0: 2e73 6574 5465 7874 2873 656c 662e 7374  .setText(self.st
-0000cfe0: 6174 696f 6e2e 6765 7428 224c 6963 656e  ation.get("Licen
-0000cff0: 7365 436c 6173 7322 2c20 2222 2929 0a20  seClass", "")). 
-0000d000: 2020 2020 2020 2073 656c 662e 7365 7474         self.sett
-0000d010: 696e 6773 5f64 6961 6c6f 672e 4c61 7469  ings_dialog.Lati
-0000d020: 7475 6465 2e73 6574 5465 7874 2873 7472  tude.setText(str
-0000d030: 2873 656c 662e 7374 6174 696f 6e2e 6765  (self.station.ge
-0000d040: 7428 224c 6174 6974 7564 6522 2c20 2222  t("Latitude", ""
-0000d050: 2929 290a 2020 2020 2020 2020 7365 6c66  ))).        self
-0000d060: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
-0000d070: 2e4c 6f6e 6769 7475 6465 2e73 6574 5465  .Longitude.setTe
-0000d080: 7874 2873 7472 2873 656c 662e 7374 6174  xt(str(self.stat
-0000d090: 696f 6e2e 6765 7428 224c 6f6e 6769 7475  ion.get("Longitu
-0000d0a0: 6465 222c 2022 2229 2929 0a20 2020 2020  de", ""))).     
-0000d0b0: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
-0000d0c0: 5f64 6961 6c6f 672e 5374 6174 696f 6e54  _dialog.StationT
-0000d0d0: 5852 582e 7365 7454 6578 7428 7365 6c66  XRX.setText(self
-0000d0e0: 2e73 7461 7469 6f6e 2e67 6574 2822 7374  .station.get("st
-0000d0f0: 6174 696f 6e74 7872 7822 2c20 2222 2929  ationtxrx", ""))
-0000d100: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-0000d110: 7474 696e 6773 5f64 6961 6c6f 672e 506f  ttings_dialog.Po
-0000d120: 7765 722e 7365 7454 6578 7428 7365 6c66  wer.setText(self
-0000d130: 2e73 7461 7469 6f6e 2e67 6574 2822 5350  .station.get("SP
-0000d140: 6f77 6522 2c20 2222 2929 0a20 2020 2020  owe", "")).     
-0000d150: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
-0000d160: 5f64 6961 6c6f 672e 416e 7465 6e6e 612e  _dialog.Antenna.
-0000d170: 7365 7454 6578 7428 7365 6c66 2e73 7461  setText(self.sta
-0000d180: 7469 6f6e 2e67 6574 2822 5341 6e74 6522  tion.get("SAnte"
-0000d190: 2c20 2222 2929 0a20 2020 2020 2020 2073  , "")).        s
-0000d1a0: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
-0000d1b0: 6c6f 672e 416e 7448 6569 6768 742e 7365  log.AntHeight.se
-0000d1c0: 7454 6578 7428 7365 6c66 2e73 7461 7469  tText(self.stati
-0000d1d0: 6f6e 2e67 6574 2822 5341 6e74 4831 222c  on.get("SAntH1",
-0000d1e0: 2022 2229 290a 2020 2020 2020 2020 7365   "")).        se
-0000d1f0: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
-0000d200: 6f67 2e41 534c 2e73 6574 5465 7874 2873  og.ASL.setText(s
-0000d210: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
-0000d220: 2253 416e 7448 3222 2c20 2222 2929 0a20  "SAntH2", "")). 
-0000d230: 2020 2020 2020 2073 656c 662e 7365 7474         self.sett
-0000d240: 696e 6773 5f64 6961 6c6f 672e 4152 524c  ings_dialog.ARRL
-0000d250: 5365 6374 696f 6e2e 7365 7454 6578 7428  Section.setText(
-0000d260: 7365 6c66 2e73 7461 7469 6f6e 2e67 6574  self.station.get
-0000d270: 2822 4152 524c 5365 6374 696f 6e22 2c20  ("ARRLSection", 
-0000d280: 2222 2929 0a20 2020 2020 2020 2073 656c  "")).        sel
-0000d290: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
-0000d2a0: 672e 526f 7665 7251 5448 2e73 6574 5465  g.RoverQTH.setTe
-0000d2b0: 7874 2873 656c 662e 7374 6174 696f 6e2e  xt(self.station.
-0000d2c0: 6765 7428 2252 6f76 6572 5154 4822 2c20  get("RoverQTH", 
-0000d2d0: 2222 2929 0a20 2020 2020 2020 2073 656c  "")).        sel
-0000d2e0: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
-0000d2f0: 672e 436c 7562 2e73 6574 5465 7874 2873  g.Club.setText(s
-0000d300: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
-0000d310: 2243 6c75 6222 2c20 2222 2929 0a20 2020  "Club", "")).   
-0000d320: 2020 2020 2073 656c 662e 7365 7474 696e       self.settin
-0000d330: 6773 5f64 6961 6c6f 672e 456d 6169 6c2e  gs_dialog.Email.
-0000d340: 7365 7454 6578 7428 7365 6c66 2e73 7461  setText(self.sta
-0000d350: 7469 6f6e 2e67 6574 2822 456d 6169 6c22  tion.get("Email"
-0000d360: 2c20 2222 2929 0a20 2020 2020 2020 2073  , "")).        s
-0000d370: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
-0000d380: 6c6f 672e 6f70 656e 2829 0a0a 2020 2020  log.open()..    
-0000d390: 6465 6620 7361 7665 5f73 6574 7469 6e67  def save_setting
-0000d3a0: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
-0000d3b0: 2022 2222 5361 7665 2073 6574 7469 6e67   """Save setting
-0000d3c0: 7322 2222 0a20 2020 2020 2020 2063 7320  s""".        cs 
-0000d3d0: 3d20 7365 6c66 2e73 6574 7469 6e67 735f  = self.settings_
-0000d3e0: 6469 616c 6f67 2e43 616c 6c2e 7465 7874  dialog.Call.text
-0000d3f0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-0000d400: 7374 6174 696f 6e20 3d20 7b7d 0a20 2020  station = {}.   
-0000d410: 2020 2020 2073 656c 662e 7374 6174 696f       self.statio
-0000d420: 6e5b 2243 616c 6c22 5d20 3d20 6373 2e75  n["Call"] = cs.u
-0000d430: 7070 6572 2829 0a20 2020 2020 2020 2073  pper().        s
-0000d440: 656c 662e 7374 6174 696f 6e5b 224e 616d  elf.station["Nam
-0000d450: 6522 5d20 3d20 7365 6c66 2e73 6574 7469  e"] = self.setti
-0000d460: 6e67 735f 6469 616c 6f67 2e4e 616d 652e  ngs_dialog.Name.
-0000d470: 7465 7874 2829 2e74 6974 6c65 2829 0a20  text().title(). 
-0000d480: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-0000d490: 696f 6e5b 2253 7472 6565 7431 225d 203d  ion["Street1"] =
-0000d4a0: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
-0000d4b0: 6961 6c6f 672e 4164 6472 6573 7331 2e74  ialog.Address1.t
-0000d4c0: 6578 7428 292e 7469 746c 6528 290a 2020  ext().title().  
-0000d4d0: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
-0000d4e0: 6f6e 5b22 5374 7265 6574 3222 5d20 3d20  on["Street2"] = 
-0000d4f0: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
-0000d500: 616c 6f67 2e41 6464 7265 7373 322e 7465  alog.Address2.te
-0000d510: 7874 2829 2e74 6974 6c65 2829 0a20 2020  xt().title().   
-0000d520: 2020 2020 2073 656c 662e 7374 6174 696f       self.statio
-0000d530: 6e5b 2243 6974 7922 5d20 3d20 7365 6c66  n["City"] = self
-0000d540: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
-0000d550: 2e43 6974 792e 7465 7874 2829 2e74 6974  .City.text().tit
-0000d560: 6c65 2829 0a20 2020 2020 2020 2073 656c  le().        sel
-0000d570: 662e 7374 6174 696f 6e5b 2253 7461 7465  f.station["State
-0000d580: 225d 203d 2073 656c 662e 7365 7474 696e  "] = self.settin
-0000d590: 6773 5f64 6961 6c6f 672e 5374 6174 652e  gs_dialog.State.
-0000d5a0: 7465 7874 2829 2e75 7070 6572 2829 0a20  text().upper(). 
-0000d5b0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-0000d5c0: 696f 6e5b 225a 6970 225d 203d 2073 656c  ion["Zip"] = sel
-0000d5d0: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
-0000d5e0: 672e 5a69 702e 7465 7874 2829 0a20 2020  g.Zip.text().   
-0000d5f0: 2020 2020 2073 656c 662e 7374 6174 696f       self.statio
-0000d600: 6e5b 2243 6f75 6e74 7279 225d 203d 2073  n["Country"] = s
-0000d610: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
-0000d620: 6c6f 672e 436f 756e 7472 792e 7465 7874  log.Country.text
-0000d630: 2829 2e74 6974 6c65 2829 0a20 2020 2020  ().title().     
-0000d640: 2020 2073 656c 662e 7374 6174 696f 6e5b     self.station[
-0000d650: 2247 7269 6453 7175 6172 6522 5d20 3d20  "GridSquare"] = 
-0000d660: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
-0000d670: 616c 6f67 2e47 7269 6453 7175 6172 652e  alog.GridSquare.
-0000d680: 7465 7874 2829 0a20 2020 2020 2020 2073  text().        s
-0000d690: 656c 662e 7374 6174 696f 6e5b 2243 515a  elf.station["CQZ
-0000d6a0: 6f6e 6522 5d20 3d20 7365 6c66 2e73 6574  one"] = self.set
-0000d6b0: 7469 6e67 735f 6469 616c 6f67 2e43 515a  tings_dialog.CQZ
-0000d6c0: 6f6e 652e 7465 7874 2829 0a20 2020 2020  one.text().     
-0000d6d0: 2020 2073 656c 662e 7374 6174 696f 6e5b     self.station[
-0000d6e0: 2249 4152 555a 6f6e 6522 5d20 3d20 7365  "IARUZone"] = se
-0000d6f0: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
-0000d700: 6f67 2e49 5455 5a6f 6e65 2e74 6578 7428  og.ITUZone.text(
-0000d710: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
-0000d720: 7461 7469 6f6e 5b22 4c69 6365 6e73 6543  tation["LicenseC
-0000d730: 6c61 7373 225d 203d 2073 656c 662e 7365  lass"] = self.se
-0000d740: 7474 696e 6773 5f64 6961 6c6f 672e 4c69  ttings_dialog.Li
-0000d750: 6365 6e73 652e 7465 7874 2829 2e74 6974  cense.text().tit
-0000d760: 6c65 2829 0a20 2020 2020 2020 2073 656c  le().        sel
-0000d770: 662e 7374 6174 696f 6e5b 224c 6174 6974  f.station["Latit
-0000d780: 7564 6522 5d20 3d20 7365 6c66 2e73 6574  ude"] = self.set
-0000d790: 7469 6e67 735f 6469 616c 6f67 2e4c 6174  tings_dialog.Lat
-0000d7a0: 6974 7564 652e 7465 7874 2829 0a20 2020  itude.text().   
-0000d7b0: 2020 2020 2073 656c 662e 7374 6174 696f       self.statio
-0000d7c0: 6e5b 224c 6f6e 6769 7475 6465 225d 203d  n["Longitude"] =
-0000d7d0: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
-0000d7e0: 6961 6c6f 672e 4c6f 6e67 6974 7564 652e  ialog.Longitude.
-0000d7f0: 7465 7874 2829 0a20 2020 2020 2020 2073  text().        s
-0000d800: 656c 662e 7374 6174 696f 6e5b 2253 5458  elf.station["STX
-0000d810: 6571 225d 203d 2073 656c 662e 7365 7474  eq"] = self.sett
-0000d820: 696e 6773 5f64 6961 6c6f 672e 5374 6174  ings_dialog.Stat
-0000d830: 696f 6e54 5852 582e 7465 7874 2829 0a20  ionTXRX.text(). 
-0000d840: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-0000d850: 696f 6e5b 2253 506f 7765 225d 203d 2073  ion["SPowe"] = s
-0000d860: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
-0000d870: 6c6f 672e 506f 7765 722e 7465 7874 2829  log.Power.text()
-0000d880: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
-0000d890: 6174 696f 6e5b 2253 416e 7465 225d 203d  ation["SAnte"] =
-0000d8a0: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
-0000d8b0: 6961 6c6f 672e 416e 7465 6e6e 612e 7465  ialog.Antenna.te
-0000d8c0: 7874 2829 0a20 2020 2020 2020 2073 656c  xt().        sel
-0000d8d0: 662e 7374 6174 696f 6e5b 2253 416e 7448  f.station["SAntH
-0000d8e0: 3122 5d20 3d20 7365 6c66 2e73 6574 7469  1"] = self.setti
-0000d8f0: 6e67 735f 6469 616c 6f67 2e41 6e74 4865  ngs_dialog.AntHe
-0000d900: 6967 6874 2e74 6578 7428 290a 2020 2020  ight.text().    
-0000d910: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
-0000d920: 5b22 5341 6e74 4832 225d 203d 2073 656c  ["SAntH2"] = sel
-0000d930: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
-0000d940: 672e 4153 4c2e 7465 7874 2829 0a20 2020  g.ASL.text().   
-0000d950: 2020 2020 2073 656c 662e 7374 6174 696f       self.statio
-0000d960: 6e5b 2241 5252 4c53 6563 7469 6f6e 225d  n["ARRLSection"]
-0000d970: 203d 2073 656c 662e 7365 7474 696e 6773   = self.settings
-0000d980: 5f64 6961 6c6f 672e 4152 524c 5365 6374  _dialog.ARRLSect
-0000d990: 696f 6e2e 7465 7874 2829 2e75 7070 6572  ion.text().upper
-0000d9a0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-0000d9b0: 7374 6174 696f 6e5b 2252 6f76 6572 5154  station["RoverQT
-0000d9c0: 4822 5d20 3d20 7365 6c66 2e73 6574 7469  H"] = self.setti
-0000d9d0: 6e67 735f 6469 616c 6f67 2e52 6f76 6572  ngs_dialog.Rover
-0000d9e0: 5154 482e 7465 7874 2829 0a20 2020 2020  QTH.text().     
-0000d9f0: 2020 2073 656c 662e 7374 6174 696f 6e5b     self.station[
-0000da00: 2243 6c75 6222 5d20 3d20 7365 6c66 2e73  "Club"] = self.s
-0000da10: 6574 7469 6e67 735f 6469 616c 6f67 2e43  ettings_dialog.C
-0000da20: 6c75 622e 7465 7874 2829 2e74 6974 6c65  lub.text().title
-0000da30: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
-0000da40: 7374 6174 696f 6e5b 2245 6d61 696c 225d  station["Email"]
-0000da50: 203d 2073 656c 662e 7365 7474 696e 6773   = self.settings
-0000da60: 5f64 6961 6c6f 672e 456d 6169 6c2e 7465  _dialog.Email.te
-0000da70: 7874 2829 0a20 2020 2020 2020 2073 656c  xt().        sel
-0000da80: 662e 6461 7461 6261 7365 2e61 6464 5f73  f.database.add_s
-0000da90: 7461 7469 6f6e 2873 656c 662e 7374 6174  tation(self.stat
-0000daa0: 696f 6e29 0a20 2020 2020 2020 2073 656c  ion).        sel
-0000dab0: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
-0000dac0: 672e 636c 6f73 6528 290a 2020 2020 2020  g.close().      
-0000dad0: 2020 6966 2073 656c 662e 6375 7272 656e    if self.curren
-0000dae0: 745f 6f70 203d 3d20 2222 3a0a 2020 2020  t_op == "":.    
-0000daf0: 2020 2020 2020 2020 7365 6c66 2e63 7572          self.cur
-0000db00: 7265 6e74 5f6f 7020 3d20 7365 6c66 2e73  rent_op = self.s
-0000db10: 7461 7469 6f6e 2e67 6574 2822 4361 6c6c  tation.get("Call
-0000db20: 222c 2022 2229 0a20 2020 2020 2020 2020  ", "").         
-0000db30: 2020 2073 656c 662e 6d61 6b65 5f6f 705f     self.make_op_
-0000db40: 6469 7228 290a 2020 2020 2020 2020 636f  dir().        co
-0000db50: 6e74 6573 745f 636f 756e 7420 3d20 7365  ntest_count = se
-0000db60: 6c66 2e64 6174 6162 6173 652e 6665 7463  lf.database.fetc
-0000db70: 685f 616c 6c5f 636f 6e74 6573 7473 2829  h_all_contests()
-0000db80: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-0000db90: 636f 6e74 6573 745f 636f 756e 7429 203d  contest_count) =
-0000dba0: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-0000dbb0: 2073 656c 662e 6e65 775f 636f 6e74 6573   self.new_contes
-0000dbc0: 745f 6469 616c 6f67 2829 0a0a 2020 2020  t_dialog()..    
-0000dbd0: 6465 6620 6564 6974 5f6d 6163 726f 2873  def edit_macro(s
-0000dbe0: 656c 662c 2066 756e 6374 696f 6e5f 6b65  elf, function_ke
-0000dbf0: 7929 3a0a 2020 2020 2020 2020 2222 2253  y):.        """S
-0000dc00: 686f 7720 6564 6974 206d 6163 726f 2064  how edit macro d
-0000dc10: 6961 6c6f 6722 2222 0a20 2020 2020 2020  ialog""".       
-0000dc20: 2073 656c 662e 6564 6974 5f6d 6163 726f   self.edit_macro
-0000dc30: 5f64 6961 6c6f 6720 3d20 4564 6974 4d61  _dialog = EditMa
-0000dc40: 6372 6f28 6675 6e63 7469 6f6e 5f6b 6579  cro(function_key
-0000dc50: 2c20 574f 524b 494e 475f 5041 5448 290a  , WORKING_PATH).
-0000dc60: 2020 2020 2020 2020 7365 6c66 2e65 6469          self.edi
-0000dc70: 745f 6d61 6372 6f5f 6469 616c 6f67 2e61  t_macro_dialog.a
-0000dc80: 6363 6570 7465 642e 636f 6e6e 6563 7428  ccepted.connect(
-0000dc90: 7365 6c66 2e65 6469 7465 645f 6d61 6372  self.edited_macr
-0000dca0: 6f29 0a20 2020 2020 2020 2073 656c 662e  o).        self.
-0000dcb0: 6564 6974 5f6d 6163 726f 5f64 6961 6c6f  edit_macro_dialo
-0000dcc0: 672e 6f70 656e 2829 0a0a 2020 2020 6465  g.open()..    de
-0000dcd0: 6620 6564 6974 6564 5f6d 6163 726f 2873  f edited_macro(s
-0000dce0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-0000dcf0: 2253 6176 6520 6564 6974 6564 206d 6163  "Save edited mac
-0000dd00: 726f 2222 220a 2020 2020 2020 2020 7365  ro""".        se
-0000dd10: 6c66 2e65 6469 745f 6d61 6372 6f5f 6469  lf.edit_macro_di
-0000dd20: 616c 6f67 2e66 756e 6374 696f 6e5f 6b65  alog.function_ke
-0000dd30: 792e 7365 7454 6578 7428 0a20 2020 2020  y.setText(.     
-0000dd40: 2020 2020 2020 2073 656c 662e 6564 6974         self.edit
-0000dd50: 5f6d 6163 726f 5f64 6961 6c6f 672e 6d61  _macro_dialog.ma
-0000dd60: 6372 6f5f 6c61 6265 6c2e 7465 7874 2829  cro_label.text()
-0000dd70: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-0000dd80: 2020 2073 656c 662e 6564 6974 5f6d 6163     self.edit_mac
-0000dd90: 726f 5f64 6961 6c6f 672e 6675 6e63 7469  ro_dialog.functi
-0000dda0: 6f6e 5f6b 6579 2e73 6574 546f 6f6c 5469  on_key.setToolTi
-0000ddb0: 7028 0a20 2020 2020 2020 2020 2020 2073  p(.            s
-0000ddc0: 656c 662e 6564 6974 5f6d 6163 726f 5f64  elf.edit_macro_d
-0000ddd0: 6961 6c6f 672e 7468 655f 6d61 6372 6f2e  ialog.the_macro.
-0000dde0: 7465 7874 2829 0a20 2020 2020 2020 2029  text().        )
-0000ddf0: 0a20 2020 2020 2020 2073 656c 662e 6564  .        self.ed
-0000de00: 6974 5f6d 6163 726f 5f64 6961 6c6f 672e  it_macro_dialog.
-0000de10: 636c 6f73 6528 290a 0a20 2020 2064 6566  close()..    def
-0000de20: 2065 6469 745f 4631 2873 656c 6629 3a0a   edit_F1(self):.
-0000de30: 2020 2020 2020 2020 2222 2273 7475 6222          """stub"
-0000de40: 2222 0a20 2020 2020 2020 206c 6f67 6765  "".        logge
-0000de50: 722e 6465 6275 6728 2246 3120 5269 6768  r.debug("F1 Righ
-0000de60: 7420 436c 6963 6b65 642e 2229 0a20 2020  t Clicked.").   
-0000de70: 2020 2020 2073 656c 662e 6564 6974 5f6d       self.edit_m
-0000de80: 6163 726f 2873 656c 662e 4631 290a 0a20  acro(self.F1).. 
-0000de90: 2020 2064 6566 2065 6469 745f 4632 2873     def edit_F2(s
-0000dea0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-0000deb0: 2273 7475 6222 2222 0a20 2020 2020 2020  "stub""".       
-0000dec0: 206c 6f67 6765 722e 6465 6275 6728 2246   logger.debug("F
-0000ded0: 3220 5269 6768 7420 436c 6963 6b65 642e  2 Right Clicked.
-0000dee0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-0000def0: 6564 6974 5f6d 6163 726f 2873 656c 662e  edit_macro(self.
-0000df00: 4632 290a 0a20 2020 2064 6566 2065 6469  F2)..    def edi
-0000df10: 745f 4633 2873 656c 6629 3a0a 2020 2020  t_F3(self):.    
-0000df20: 2020 2020 2222 2273 7475 6222 2222 0a20      """stub""". 
-0000df30: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-0000df40: 6275 6728 2246 3320 5269 6768 7420 436c  bug("F3 Right Cl
-0000df50: 6963 6b65 642e 2229 0a20 2020 2020 2020  icked.").       
-0000df60: 2073 656c 662e 6564 6974 5f6d 6163 726f   self.edit_macro
-0000df70: 2873 656c 662e 4633 290a 0a20 2020 2064  (self.F3)..    d
-0000df80: 6566 2065 6469 745f 4634 2873 656c 6629  ef edit_F4(self)
-0000df90: 3a0a 2020 2020 2020 2020 2222 2273 7475  :.        """stu
-0000dfa0: 6222 2222 0a20 2020 2020 2020 206c 6f67  b""".        log
-0000dfb0: 6765 722e 6465 6275 6728 2246 3420 5269  ger.debug("F4 Ri
-0000dfc0: 6768 7420 436c 6963 6b65 642e 2229 0a20  ght Clicked."). 
-0000dfd0: 2020 2020 2020 2073 656c 662e 6564 6974         self.edit
-0000dfe0: 5f6d 6163 726f 2873 656c 662e 4634 290a  _macro(self.F4).
-0000dff0: 0a20 2020 2064 6566 2065 6469 745f 4635  .    def edit_F5
-0000e000: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000e010: 2222 2273 7475 6222 2222 0a20 2020 2020  """stub""".     
-0000e020: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-0000e030: 2246 3520 5269 6768 7420 436c 6963 6b65  "F5 Right Clicke
-0000e040: 642e 2229 0a20 2020 2020 2020 2073 656c  d.").        sel
-0000e050: 662e 6564 6974 5f6d 6163 726f 2873 656c  f.edit_macro(sel
-0000e060: 662e 4635 290a 0a20 2020 2064 6566 2065  f.F5)..    def e
-0000e070: 6469 745f 4636 2873 656c 6629 3a0a 2020  dit_F6(self):.  
-0000e080: 2020 2020 2020 2222 2273 7475 6222 2222        """stub"""
-0000e090: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-0000e0a0: 6465 6275 6728 2246 3620 5269 6768 7420  debug("F6 Right 
-0000e0b0: 436c 6963 6b65 642e 2229 0a20 2020 2020  Clicked.").     
-0000e0c0: 2020 2073 656c 662e 6564 6974 5f6d 6163     self.edit_mac
-0000e0d0: 726f 2873 656c 662e 4636 290a 0a20 2020  ro(self.F6)..   
-0000e0e0: 2064 6566 2065 6469 745f 4637 2873 656c   def edit_F7(sel
-0000e0f0: 6629 3a0a 2020 2020 2020 2020 2222 2273  f):.        """s
-0000e100: 7475 6222 2222 0a20 2020 2020 2020 206c  tub""".        l
-0000e110: 6f67 6765 722e 6465 6275 6728 2246 3720  ogger.debug("F7 
-0000e120: 5269 6768 7420 436c 6963 6b65 642e 2229  Right Clicked.")
-0000e130: 0a20 2020 2020 2020 2073 656c 662e 6564  .        self.ed
-0000e140: 6974 5f6d 6163 726f 2873 656c 662e 4637  it_macro(self.F7
-0000e150: 290a 0a20 2020 2064 6566 2065 6469 745f  )..    def edit_
-0000e160: 4638 2873 656c 6629 3a0a 2020 2020 2020  F8(self):.      
-0000e170: 2020 2222 2273 7475 6222 2222 0a20 2020    """stub""".   
-0000e180: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-0000e190: 6728 2246 3820 5269 6768 7420 436c 6963  g("F8 Right Clic
-0000e1a0: 6b65 642e 2229 0a20 2020 2020 2020 2073  ked.").        s
-0000e1b0: 656c 662e 6564 6974 5f6d 6163 726f 2873  elf.edit_macro(s
-0000e1c0: 656c 662e 4638 290a 0a20 2020 2064 6566  elf.F8)..    def
-0000e1d0: 2065 6469 745f 4639 2873 656c 6629 3a0a   edit_F9(self):.
-0000e1e0: 2020 2020 2020 2020 2222 2273 7475 6222          """stub"
-0000e1f0: 2222 0a20 2020 2020 2020 206c 6f67 6765  "".        logge
-0000e200: 722e 6465 6275 6728 2246 3920 5269 6768  r.debug("F9 Righ
-0000e210: 7420 436c 6963 6b65 642e 2229 0a20 2020  t Clicked.").   
-0000e220: 2020 2020 2073 656c 662e 6564 6974 5f6d       self.edit_m
-0000e230: 6163 726f 2873 656c 662e 4639 290a 0a20  acro(self.F9).. 
-0000e240: 2020 2064 6566 2065 6469 745f 4631 3028     def edit_F10(
-0000e250: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-0000e260: 2222 7374 7562 2222 220a 2020 2020 2020  ""stub""".      
-0000e270: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
-0000e280: 4631 3020 5269 6768 7420 436c 6963 6b65  F10 Right Clicke
-0000e290: 642e 2229 0a20 2020 2020 2020 2073 656c  d.").        sel
-0000e2a0: 662e 6564 6974 5f6d 6163 726f 2873 656c  f.edit_macro(sel
-0000e2b0: 662e 4631 3029 0a0a 2020 2020 6465 6620  f.F10)..    def 
-0000e2c0: 6564 6974 5f46 3131 2873 656c 6629 3a0a  edit_F11(self):.
-0000e2d0: 2020 2020 2020 2020 2222 2273 7475 6222          """stub"
-0000e2e0: 2222 0a20 2020 2020 2020 206c 6f67 6765  "".        logge
-0000e2f0: 722e 6465 6275 6728 2246 3131 2052 6967  r.debug("F11 Rig
-0000e300: 6874 2043 6c69 636b 6564 2e22 290a 2020  ht Clicked.").  
-0000e310: 2020 2020 2020 7365 6c66 2e65 6469 745f        self.edit_
-0000e320: 6d61 6372 6f28 7365 6c66 2e46 3131 290a  macro(self.F11).
-0000e330: 0a20 2020 2064 6566 2065 6469 745f 4631  .    def edit_F1
-0000e340: 3228 7365 6c66 293a 0a20 2020 2020 2020  2(self):.       
-0000e350: 2022 2222 7374 7562 2222 220a 2020 2020   """stub""".    
-0000e360: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-0000e370: 2822 4631 3220 5269 6768 7420 436c 6963  ("F12 Right Clic
-0000e380: 6b65 642e 2229 0a20 2020 2020 2020 2073  ked.").        s
-0000e390: 656c 662e 6564 6974 5f6d 6163 726f 2873  elf.edit_macro(s
-0000e3a0: 656c 662e 4631 3229 0a0a 2020 2020 6465  elf.F12)..    de
-0000e3b0: 6620 7072 6f63 6573 735f 6d61 6372 6f28  f process_macro(
-0000e3c0: 7365 6c66 2c20 6d61 6372 6f3a 2073 7472  self, macro: str
-0000e3d0: 2920 2d3e 2073 7472 3a0a 2020 2020 2020  ) -> str:.      
-0000e3e0: 2020 2222 2250 726f 6365 7373 2043 5720    """Process CW 
-0000e3f0: 6d61 6372 6f20 7375 6273 7469 7475 7469  macro substituti
-0000e400: 6f6e 7322 2222 0a20 2020 2020 2020 2072  ons""".        r
-0000e410: 6573 756c 7420 3d20 7365 6c66 2e64 6174  esult = self.dat
-0000e420: 6162 6173 652e 6765 745f 7365 7269 616c  abase.get_serial
-0000e430: 2829 0a20 2020 2020 2020 206e 6578 745f  ().        next_
-0000e440: 7365 7269 616c 203d 2073 7472 2872 6573  serial = str(res
-0000e450: 756c 742e 6765 7428 2273 6572 6961 6c5f  ult.get("serial_
-0000e460: 6e72 222c 2022 3122 2929 0a20 2020 2020  nr", "1")).     
-0000e470: 2020 2069 6620 6e65 7874 5f73 6572 6961     if next_seria
-0000e480: 6c20 3d3d 2022 4e6f 6e65 223a 0a20 2020  l == "None":.   
-0000e490: 2020 2020 2020 2020 206e 6578 745f 7365           next_se
-0000e4a0: 7269 616c 203d 2022 3122 0a20 2020 2020  rial = "1".     
-0000e4b0: 2020 206d 6163 726f 203d 206d 6163 726f     macro = macro
-0000e4c0: 2e75 7070 6572 2829 0a20 2020 2020 2020  .upper().       
-0000e4d0: 206d 6163 726f 203d 206d 6163 726f 2e72   macro = macro.r
-0000e4e0: 6570 6c61 6365 2822 2322 2c20 6e65 7874  eplace("#", next
-0000e4f0: 5f73 6572 6961 6c29 0a20 2020 2020 2020  _serial).       
-0000e500: 206d 6163 726f 203d 206d 6163 726f 2e72   macro = macro.r
-0000e510: 6570 6c61 6365 2822 7b4d 5943 414c 4c7d  eplace("{MYCALL}
-0000e520: 222c 2073 656c 662e 7374 6174 696f 6e2e  ", self.station.
-0000e530: 6765 7428 2243 616c 6c22 2c20 2222 2929  get("Call", ""))
-0000e540: 0a20 2020 2020 2020 206d 6163 726f 203d  .        macro =
-0000e550: 206d 6163 726f 2e72 6570 6c61 6365 2822   macro.replace("
-0000e560: 7b48 4953 4341 4c4c 7d22 2c20 7365 6c66  {HISCALL}", self
-0000e570: 2e63 616c 6c73 6967 6e2e 7465 7874 2829  .callsign.text()
-0000e580: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-0000e590: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
-0000e5a0: 7428 226d 6f64 6522 2920 3d3d 2022 4357  t("mode") == "CW
-0000e5b0: 223a 0a20 2020 2020 2020 2020 2020 206d  ":.            m
-0000e5c0: 6163 726f 203d 206d 6163 726f 2e72 6570  acro = macro.rep
-0000e5d0: 6c61 6365 2822 7b53 4e54 7d22 2c20 7365  lace("{SNT}", se
-0000e5e0: 6c66 2e73 656e 742e 7465 7874 2829 2e72  lf.sent.text().r
-0000e5f0: 6570 6c61 6365 2822 3922 2c20 226e 2229  eplace("9", "n")
-0000e600: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-0000e610: 2020 2020 2020 2020 2020 2020 6d61 6372              macr
-0000e620: 6f20 3d20 6d61 6372 6f2e 7265 706c 6163  o = macro.replac
-0000e630: 6528 227b 534e 547d 222c 2073 656c 662e  e("{SNT}", self.
-0000e640: 7365 6e74 2e74 6578 7428 2929 0a20 2020  sent.text()).   
-0000e650: 2020 2020 206d 6163 726f 203d 206d 6163       macro = mac
-0000e660: 726f 2e72 6570 6c61 6365 2822 7b53 454e  ro.replace("{SEN
-0000e670: 544e 527d 222c 2073 656c 662e 6f74 6865  TNR}", self.othe
-0000e680: 725f 312e 7465 7874 2829 290a 2020 2020  r_1.text()).    
-0000e690: 2020 2020 6d61 6372 6f20 3d20 6d61 6372      macro = macr
-0000e6a0: 6f2e 7265 706c 6163 6528 0a20 2020 2020  o.replace(.     
-0000e6b0: 2020 2020 2020 2022 7b45 5843 487d 222c         "{EXCH}",
-0000e6c0: 2073 656c 662e 636f 6e74 6573 745f 7365   self.contest_se
-0000e6d0: 7474 696e 6773 2e67 6574 2822 5365 6e74  ttings.get("Sent
-0000e6e0: 4578 6368 616e 6765 222c 2022 7878 7822  Exchange", "xxx"
-0000e6f0: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
-0000e700: 2020 2020 7265 7475 726e 206d 6163 726f      return macro
-0000e710: 0a0a 2020 2020 6465 6620 766f 6963 655f  ..    def voice_
-0000e720: 7374 7269 6e67 2873 656c 662c 2074 6865  string(self, the
-0000e730: 5f73 7472 696e 673a 2073 7472 2920 2d3e  _string: str) ->
-0000e740: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-0000e750: 2222 766f 6963 6573 2073 7472 696e 6720  ""voices string 
-0000e760: 7573 696e 6720 6e61 746f 2070 686f 6e65  using nato phone
-0000e770: 7469 6373 2222 220a 2020 2020 2020 2020  tics""".        
-0000e780: 6c6f 6767 6572 2e64 6562 7567 2822 566f  logger.debug("Vo
-0000e790: 6963 696e 673a 2025 7322 2c20 7468 655f  icing: %s", the_
-0000e7a0: 7374 7269 6e67 290a 2020 2020 2020 2020  string).        
-0000e7b0: 6f70 5f70 6174 6820 3d20 5061 7468 2844  op_path = Path(D
-0000e7c0: 4154 415f 5041 5448 2920 2f20 7365 6c66  ATA_PATH) / self
-0000e7d0: 2e63 7572 7265 6e74 5f6f 700a 2020 2020  .current_op.    
-0000e7e0: 2020 2020 6966 2022 5b22 2069 6e20 7468      if "[" in th
-0000e7f0: 655f 7374 7269 6e67 3a0a 2020 2020 2020  e_string:.      
-0000e800: 2020 2020 2020 7375 625f 7374 7269 6e67        sub_string
-0000e810: 203d 2074 6865 5f73 7472 696e 672e 7374   = the_string.st
-0000e820: 7269 7028 225b 5d22 292e 6c6f 7765 7228  rip("[]").lower(
-0000e830: 290a 2020 2020 2020 2020 2020 2020 6669  ).            fi
-0000e840: 6c65 6e61 6d65 203d 2066 227b 7374 7228  lename = f"{str(
-0000e850: 6f70 5f70 6174 6829 7d2f 7b73 7562 5f73  op_path)}/{sub_s
-0000e860: 7472 696e 677d 2e77 6176 220a 2020 2020  tring}.wav".    
-0000e870: 2020 2020 2020 2020 6966 2050 6174 6828          if Path(
-0000e880: 6669 6c65 6e61 6d65 292e 6973 5f66 696c  filename).is_fil
-0000e890: 6528 293a 0a20 2020 2020 2020 2020 2020  e():.           
-0000e8a0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-0000e8b0: 6728 2256 6f69 6369 6e67 3a20 2573 222c  g("Voicing: %s",
-0000e8c0: 2066 696c 656e 616d 6529 0a20 2020 2020   filename).     
-0000e8d0: 2020 2020 2020 2020 2020 2064 6174 612c             data,
-0000e8e0: 205f 6673 203d 2073 662e 7265 6164 2866   _fs = sf.read(f
-0000e8f0: 696c 656e 616d 652c 2064 7479 7065 3d22  ilename, dtype="
-0000e900: 666c 6f61 7433 3222 290a 2020 2020 2020  float32").      
-0000e910: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-0000e920: 7474 5f6f 6e28 290a 2020 2020 2020 2020  tt_on().        
-0000e930: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-0000e940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e950: 2073 642e 6465 6661 756c 742e 6465 7669   sd.default.devi
-0000e960: 6365 203d 2073 656c 662e 7072 6566 2e67  ce = self.pref.g
-0000e970: 6574 2822 736f 756e 6464 6576 6963 6522  et("sounddevice"
-0000e980: 2c20 2264 6566 6175 6c74 2229 0a20 2020  , "default").   
-0000e990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9a0: 2073 642e 6465 6661 756c 742e 7361 6d70   sd.default.samp
-0000e9b0: 6c65 7261 7465 203d 2034 3431 3030 2e30  lerate = 44100.0
-0000e9c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e9d0: 2020 2020 2073 642e 706c 6179 2864 6174       sd.play(dat
-0000e9e0: 6129 0a20 2020 2020 2020 2020 2020 2020  a).             
-0000e9f0: 2020 2020 2020 205f 7374 6174 7573 203d         _status =
-0000ea00: 2073 642e 7761 6974 2829 0a20 2020 2020   sd.wait().     
-0000ea10: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000ea20: 2068 7474 7073 3a2f 2f73 6e79 6b2e 696f   https://snyk.io
-0000ea30: 2f61 6476 6973 6f72 2f70 7974 686f 6e2f  /advisor/python/
-0000ea40: 736f 756e 6464 6576 6963 652f 6675 6e63  sounddevice/func
-0000ea50: 7469 6f6e 732f 736f 756e 6464 6576 6963  tions/sounddevic
-0000ea60: 652e 506f 7274 4175 6469 6f45 7272 6f72  e.PortAudioError
-0000ea70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ea80: 2065 7863 6570 7420 7364 2e50 6f72 7441   except sd.PortA
-0000ea90: 7564 696f 4572 726f 7220 6173 2065 7272  udioError as err
-0000eaa0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000eab0: 2020 2020 2020 6c6f 6767 6572 2e77 6172        logger.war
-0000eac0: 6e69 6e67 2822 2573 222c 2066 227b 6572  ning("%s", f"{er
-0000ead0: 727d 2229 0a0a 2020 2020 2020 2020 2020  r}")..          
-0000eae0: 2020 2020 2020 7365 6c66 2e70 7474 5f6f        self.ptt_o
-0000eaf0: 6666 2829 0a20 2020 2020 2020 2020 2020  ff().           
-0000eb00: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-0000eb10: 7365 6c66 2e70 7474 5f6f 6e28 290a 2020  self.ptt_on().  
-0000eb20: 2020 2020 2020 666f 7220 6c65 7474 6572        for letter
-0000eb30: 2069 6e20 7468 655f 7374 7269 6e67 2e6c   in the_string.l
-0000eb40: 6f77 6572 2829 3a0a 2020 2020 2020 2020  ower():.        
-0000eb50: 2020 2020 6966 206c 6574 7465 7220 696e      if letter in
-0000eb60: 2022 6162 6364 6566 6768 696a 6b6c 6d6e   "abcdefghijklmn
-0000eb70: 6f70 7172 7374 7576 7778 797a 2031 3233  opqrstuvwxyz 123
-0000eb80: 3435 3637 3839 3022 3a0a 2020 2020 2020  4567890":.      
-0000eb90: 2020 2020 2020 2020 2020 6966 206c 6574            if let
-0000eba0: 7465 7220 3d3d 2022 2022 3a0a 2020 2020  ter == " ":.    
-0000ebb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ebc0: 6c65 7474 6572 203d 2022 7370 6163 6522  letter = "space"
-0000ebd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ebe0: 2066 696c 656e 616d 6520 3d20 6622 7b73   filename = f"{s
-0000ebf0: 7472 286f 705f 7061 7468 297d 2f7b 6c65  tr(op_path)}/{le
-0000ec00: 7474 6572 7d2e 7761 7622 0a20 2020 2020  tter}.wav".     
-0000ec10: 2020 2020 2020 2020 2020 2069 6620 5061             if Pa
-0000ec20: 7468 2866 696c 656e 616d 6529 2e69 735f  th(filename).is_
-0000ec30: 6669 6c65 2829 3a0a 2020 2020 2020 2020  file():.        
-0000ec40: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-0000ec50: 6572 2e64 6562 7567 2822 566f 6963 696e  er.debug("Voicin
-0000ec60: 673a 2025 7322 2c20 6669 6c65 6e61 6d65  g: %s", filename
-0000ec70: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000ec80: 2020 2020 2020 6461 7461 2c20 5f66 7320        data, _fs 
-0000ec90: 3d20 7366 2e72 6561 6428 6669 6c65 6e61  = sf.read(filena
-0000eca0: 6d65 2c20 6474 7970 653d 2266 6c6f 6174  me, dtype="float
-0000ecb0: 3332 2229 0a20 2020 2020 2020 2020 2020  32").           
-0000ecc0: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
-0000ecd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ece0: 2020 2020 2020 7364 2e64 6566 6175 6c74        sd.default
-0000ecf0: 2e64 6576 6963 6520 3d20 7365 6c66 2e70  .device = self.p
-0000ed00: 7265 662e 6765 7428 2273 6f75 6e64 6465  ref.get("soundde
-0000ed10: 7669 6365 222c 2022 6465 6661 756c 7422  vice", "default"
-0000ed20: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000ed30: 2020 2020 2020 2020 2020 7364 2e64 6566            sd.def
-0000ed40: 6175 6c74 2e73 616d 706c 6572 6174 6520  ault.samplerate 
-0000ed50: 3d20 3434 3130 302e 300a 2020 2020 2020  = 44100.0.      
-0000ed60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed70: 2020 7364 2e70 6c61 7928 6461 7461 290a    sd.play(data).
-0000ed80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed90: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-0000eda0: 6562 7567 2822 2573 222c 2066 227b 7364  ebug("%s", f"{sd
-0000edb0: 2e77 6169 7428 297d 2229 0a20 2020 2020  .wait()}").     
-0000edc0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000edd0: 7863 6570 7420 7364 2e50 6f72 7441 7564  xcept sd.PortAud
-0000ede0: 696f 4572 726f 7220 6173 2065 7272 3a0a  ioError as err:.
-0000edf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee00: 2020 2020 2020 2020 6c6f 6767 6572 2e77          logger.w
-0000ee10: 6172 6e69 6e67 2822 2573 222c 2066 227b  arning("%s", f"{
-0000ee20: 6572 727d 2229 0a20 2020 2020 2020 2073  err}").        s
-0000ee30: 656c 662e 7074 745f 6f66 6628 290a 0a20  elf.ptt_off().. 
-0000ee40: 2020 2064 6566 2070 7474 5f6f 6e28 7365     def ptt_on(se
-0000ee50: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-0000ee60: 7475 726e 206f 6e20 7074 7422 2222 0a20  turn on ptt""". 
-0000ee70: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
-0000ee80: 6967 5f63 6f6e 7472 6f6c 3a0a 2020 2020  ig_control:.    
-0000ee90: 2020 2020 2020 2020 7365 6c66 2e6c 6566          self.lef
-0000eea0: 7464 6f74 2e73 6574 5069 786d 6170 2873  tdot.setPixmap(s
-0000eeb0: 656c 662e 6772 6565 6e64 6f74 290a 2020  elf.greendot).  
-0000eec0: 2020 2020 2020 2020 2020 6170 702e 7072            app.pr
-0000eed0: 6f63 6573 7345 7665 6e74 7328 290a 2020  ocessEvents().  
-0000eee0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-0000eef0: 6967 5f63 6f6e 7472 6f6c 2e70 7474 5f6f  ig_control.ptt_o
-0000ef00: 6e28 290a 0a20 2020 2064 6566 2070 7474  n()..    def ptt
-0000ef10: 5f6f 6666 2873 656c 6629 3a0a 2020 2020  _off(self):.    
-0000ef20: 2020 2020 2222 2274 7572 6e20 6f66 6620      """turn off 
-0000ef30: 7074 7422 2222 0a20 2020 2020 2020 2069  ptt""".        i
-0000ef40: 6620 7365 6c66 2e72 6967 5f63 6f6e 7472  f self.rig_contr
-0000ef50: 6f6c 3a0a 2020 2020 2020 2020 2020 2020  ol:.            
-0000ef60: 7365 6c66 2e6c 6566 7464 6f74 2e73 6574  self.leftdot.set
-0000ef70: 5069 786d 6170 2873 656c 662e 7265 6464  Pixmap(self.redd
-0000ef80: 6f74 290a 2020 2020 2020 2020 2020 2020  ot).            
-0000ef90: 6170 702e 7072 6f63 6573 7345 7665 6e74  app.processEvent
-0000efa0: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
-0000efb0: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
-0000efc0: 2e70 7474 5f6f 6666 2829 0a0a 2020 2020  .ptt_off()..    
-0000efd0: 6465 6620 7365 6e64 6631 2873 656c 6629  def sendf1(self)
-0000efe0: 3a0a 2020 2020 2020 2020 2222 2273 7475  :.        """stu
-0000eff0: 6222 2222 0a20 2020 2020 2020 206c 6f67  b""".        log
-0000f000: 6765 722e 6465 6275 6728 2246 3120 436c  ger.debug("F1 Cl
-0000f010: 6963 6b65 6422 290a 2020 2020 2020 2020  icked").        
-0000f020: 6966 2073 656c 662e 6e31 6d6d 3a0a 2020  if self.n1mm:.  
-0000f030: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-0000f040: 316d 6d2e 7261 6469 6f5f 696e 666f 5b22  1mm.radio_info["
-0000f050: 4675 6e63 7469 6f6e 4b65 7943 6170 7469  FunctionKeyCapti
-0000f060: 6f6e 225d 203d 2073 656c 662e 4631 2e74  on"] = self.F1.t
-0000f070: 6578 7428 290a 2020 2020 2020 2020 6966  ext().        if
-0000f080: 2073 656c 662e 7261 6469 6f5f 7374 6174   self.radio_stat
-0000f090: 652e 6765 7428 226d 6f64 6522 2920 696e  e.get("mode") in
-0000f0a0: 205b 224c 5342 222c 2022 5553 4222 2c20   ["LSB", "USB", 
-0000f0b0: 2253 5342 225d 3a0a 2020 2020 2020 2020  "SSB"]:.        
-0000f0c0: 2020 2020 7365 6c66 2e76 6f69 6365 5f73      self.voice_s
-0000f0d0: 7472 696e 6728 7365 6c66 2e70 726f 6365  tring(self.proce
-0000f0e0: 7373 5f6d 6163 726f 2873 656c 662e 4631  ss_macro(self.F1
-0000f0f0: 2e74 6f6f 6c54 6970 2829 2929 0a20 2020  .toolTip())).   
-0000f100: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-0000f110: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000f120: 6377 3a0a 2020 2020 2020 2020 2020 2020  cw:.            
-0000f130: 7365 6c66 2e63 772e 7365 6e64 6377 2873  self.cw.sendcw(s
-0000f140: 656c 662e 7072 6f63 6573 735f 6d61 6372  elf.process_macr
-0000f150: 6f28 7365 6c66 2e46 312e 746f 6f6c 5469  o(self.F1.toolTi
-0000f160: 7028 2929 290a 0a20 2020 2064 6566 2073  p()))..    def s
-0000f170: 656e 6466 3228 7365 6c66 293a 0a20 2020  endf2(self):.   
-0000f180: 2020 2020 2022 2222 7374 7562 2222 220a       """stub""".
-0000f190: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-0000f1a0: 6562 7567 2822 4632 2043 6c69 636b 6564  ebug("F2 Clicked
-0000f1b0: 2229 0a20 2020 2020 2020 2069 6620 7365  ").        if se
-0000f1c0: 6c66 2e6e 316d 6d3a 0a20 2020 2020 2020  lf.n1mm:.       
-0000f1d0: 2020 2020 2073 656c 662e 6e31 6d6d 2e72       self.n1mm.r
-0000f1e0: 6164 696f 5f69 6e66 6f5b 2246 756e 6374  adio_info["Funct
-0000f1f0: 696f 6e4b 6579 4361 7074 696f 6e22 5d20  ionKeyCaption"] 
-0000f200: 3d20 7365 6c66 2e46 322e 7465 7874 2829  = self.F2.text()
-0000f210: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000f220: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
-0000f230: 2822 6d6f 6465 2229 2069 6e20 5b22 4c53  ("mode") in ["LS
-0000f240: 4222 2c20 2255 5342 222c 2022 5353 4222  B", "USB", "SSB"
-0000f250: 5d3a 0a20 2020 2020 2020 2020 2020 2073  ]:.            s
-0000f260: 656c 662e 766f 6963 655f 7374 7269 6e67  elf.voice_string
-0000f270: 2873 656c 662e 7072 6f63 6573 735f 6d61  (self.process_ma
-0000f280: 6372 6f28 7365 6c66 2e46 322e 746f 6f6c  cro(self.F2.tool
-0000f290: 5469 7028 2929 290a 2020 2020 2020 2020  Tip())).        
-0000f2a0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-0000f2b0: 2020 2069 6620 7365 6c66 2e63 773a 0a20     if self.cw:. 
-0000f2c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000f2d0: 6377 2e73 656e 6463 7728 7365 6c66 2e70  cw.sendcw(self.p
-0000f2e0: 726f 6365 7373 5f6d 6163 726f 2873 656c  rocess_macro(sel
-0000f2f0: 662e 4632 2e74 6f6f 6c54 6970 2829 2929  f.F2.toolTip()))
-0000f300: 0a0a 2020 2020 6465 6620 7365 6e64 6633  ..    def sendf3
-0000f310: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000f320: 2222 2273 7475 6222 2222 0a20 2020 2020  """stub""".     
-0000f330: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-0000f340: 2246 3320 436c 6963 6b65 6422 290a 2020  "F3 Clicked").  
-0000f350: 2020 2020 2020 6966 2073 656c 662e 6e31        if self.n1
-0000f360: 6d6d 3a0a 2020 2020 2020 2020 2020 2020  mm:.            
-0000f370: 7365 6c66 2e6e 316d 6d2e 7261 6469 6f5f  self.n1mm.radio_
-0000f380: 696e 666f 5b22 4675 6e63 7469 6f6e 4b65  info["FunctionKe
-0000f390: 7943 6170 7469 6f6e 225d 203d 2073 656c  yCaption"] = sel
-0000f3a0: 662e 4633 2e74 6578 7428 290a 2020 2020  f.F3.text().    
-0000f3b0: 2020 2020 6966 2073 656c 662e 7261 6469      if self.radi
-0000f3c0: 6f5f 7374 6174 652e 6765 7428 226d 6f64  o_state.get("mod
-0000f3d0: 6522 2920 696e 205b 224c 5342 222c 2022  e") in ["LSB", "
-0000f3e0: 5553 4222 2c20 2253 5342 225d 3a0a 2020  USB", "SSB"]:.  
-0000f3f0: 2020 2020 2020 2020 2020 7365 6c66 2e76            self.v
-0000f400: 6f69 6365 5f73 7472 696e 6728 7365 6c66  oice_string(self
-0000f410: 2e70 726f 6365 7373 5f6d 6163 726f 2873  .process_macro(s
-0000f420: 656c 662e 4633 2e74 6f6f 6c54 6970 2829  elf.F3.toolTip()
-0000f430: 2929 0a20 2020 2020 2020 2020 2020 2072  )).            r
-0000f440: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
-0000f450: 2073 656c 662e 6377 3a0a 2020 2020 2020   self.cw:.      
-0000f460: 2020 2020 2020 7365 6c66 2e63 772e 7365        self.cw.se
-0000f470: 6e64 6377 2873 656c 662e 7072 6f63 6573  ndcw(self.proces
-0000f480: 735f 6d61 6372 6f28 7365 6c66 2e46 332e  s_macro(self.F3.
-0000f490: 746f 6f6c 5469 7028 2929 290a 0a20 2020  toolTip()))..   
-0000f4a0: 2064 6566 2073 656e 6466 3428 7365 6c66   def sendf4(self
-0000f4b0: 293a 0a20 2020 2020 2020 2022 2222 7374  ):.        """st
-0000f4c0: 7562 2222 220a 2020 2020 2020 2020 6c6f  ub""".        lo
-0000f4d0: 6767 6572 2e64 6562 7567 2822 4634 2043  gger.debug("F4 C
-0000f4e0: 6c69 636b 6564 2229 0a20 2020 2020 2020  licked").       
-0000f4f0: 2069 6620 7365 6c66 2e6e 316d 6d3a 0a20   if self.n1mm:. 
-0000f500: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000f510: 6e31 6d6d 2e72 6164 696f 5f69 6e66 6f5b  n1mm.radio_info[
-0000f520: 2246 756e 6374 696f 6e4b 6579 4361 7074  "FunctionKeyCapt
-0000f530: 696f 6e22 5d20 3d20 7365 6c66 2e46 342e  ion"] = self.F4.
-0000f540: 7465 7874 2829 0a20 2020 2020 2020 2069  text().        i
-0000f550: 6620 7365 6c66 2e72 6164 696f 5f73 7461  f self.radio_sta
-0000f560: 7465 2e67 6574 2822 6d6f 6465 2229 2069  te.get("mode") i
-0000f570: 6e20 5b22 4c53 4222 2c20 2255 5342 222c  n ["LSB", "USB",
-0000f580: 2022 5353 4222 5d3a 0a20 2020 2020 2020   "SSB"]:.       
-0000f590: 2020 2020 2073 656c 662e 766f 6963 655f       self.voice_
-0000f5a0: 7374 7269 6e67 2873 656c 662e 7072 6f63  string(self.proc
-0000f5b0: 6573 735f 6d61 6372 6f28 7365 6c66 2e46  ess_macro(self.F
-0000f5c0: 342e 746f 6f6c 5469 7028 2929 290a 2020  4.toolTip())).  
-0000f5d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000f5e0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000f5f0: 2e63 773a 0a20 2020 2020 2020 2020 2020  .cw:.           
-0000f600: 2073 656c 662e 6377 2e73 656e 6463 7728   self.cw.sendcw(
-0000f610: 7365 6c66 2e70 726f 6365 7373 5f6d 6163  self.process_mac
-0000f620: 726f 2873 656c 662e 4634 2e74 6f6f 6c54  ro(self.F4.toolT
-0000f630: 6970 2829 2929 0a0a 2020 2020 6465 6620  ip()))..    def 
-0000f640: 7365 6e64 6635 2873 656c 6629 3a0a 2020  sendf5(self):.  
-0000f650: 2020 2020 2020 2222 2273 7475 6222 2222        """stub"""
-0000f660: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-0000f670: 6465 6275 6728 2246 3520 436c 6963 6b65  debug("F5 Clicke
-0000f680: 6422 290a 2020 2020 2020 2020 6966 2073  d").        if s
-0000f690: 656c 662e 6e31 6d6d 3a0a 2020 2020 2020  elf.n1mm:.      
-0000f6a0: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
-0000f6b0: 7261 6469 6f5f 696e 666f 5b22 4675 6e63  radio_info["Func
-0000f6c0: 7469 6f6e 4b65 7943 6170 7469 6f6e 225d  tionKeyCaption"]
-0000f6d0: 203d 2073 656c 662e 4635 2e74 6578 7428   = self.F5.text(
-0000f6e0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-0000f6f0: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
-0000f700: 7428 226d 6f64 6522 2920 696e 205b 224c  t("mode") in ["L
-0000f710: 5342 222c 2022 5553 4222 2c20 2253 5342  SB", "USB", "SSB
-0000f720: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
-0000f730: 7365 6c66 2e76 6f69 6365 5f73 7472 696e  self.voice_strin
-0000f740: 6728 7365 6c66 2e70 726f 6365 7373 5f6d  g(self.process_m
-0000f750: 6163 726f 2873 656c 662e 4635 2e74 6f6f  acro(self.F5.too
-0000f760: 6c54 6970 2829 2929 0a20 2020 2020 2020  lTip())).       
-0000f770: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-0000f780: 2020 2020 6966 2073 656c 662e 6377 3a0a      if self.cw:.
-0000f790: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f7a0: 2e63 772e 7365 6e64 6377 2873 656c 662e  .cw.sendcw(self.
-0000f7b0: 7072 6f63 6573 735f 6d61 6372 6f28 7365  process_macro(se
-0000f7c0: 6c66 2e46 352e 746f 6f6c 5469 7028 2929  lf.F5.toolTip())
-0000f7d0: 290a 0a20 2020 2064 6566 2073 656e 6466  )..    def sendf
-0000f7e0: 3628 7365 6c66 293a 0a20 2020 2020 2020  6(self):.       
-0000f7f0: 2022 2222 7374 7562 2222 220a 2020 2020   """stub""".    
-0000f800: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-0000f810: 2822 4636 2043 6c69 636b 6564 2229 0a20  ("F6 Clicked"). 
-0000f820: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
-0000f830: 316d 6d3a 0a20 2020 2020 2020 2020 2020  1mm:.           
-0000f840: 2073 656c 662e 6e31 6d6d 2e72 6164 696f   self.n1mm.radio
-0000f850: 5f69 6e66 6f5b 2246 756e 6374 696f 6e4b  _info["FunctionK
-0000f860: 6579 4361 7074 696f 6e22 5d20 3d20 7365  eyCaption"] = se
-0000f870: 6c66 2e46 362e 7465 7874 2829 0a20 2020  lf.F6.text().   
-0000f880: 2020 2020 2069 6620 7365 6c66 2e72 6164       if self.rad
-0000f890: 696f 5f73 7461 7465 2e67 6574 2822 6d6f  io_state.get("mo
-0000f8a0: 6465 2229 2069 6e20 5b22 4c53 4222 2c20  de") in ["LSB", 
-0000f8b0: 2255 5342 222c 2022 5353 4222 5d3a 0a20  "USB", "SSB"]:. 
-0000f8c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000f8d0: 766f 6963 655f 7374 7269 6e67 2873 656c  voice_string(sel
-0000f8e0: 662e 7072 6f63 6573 735f 6d61 6372 6f28  f.process_macro(
-0000f8f0: 7365 6c66 2e46 362e 746f 6f6c 5469 7028  self.F6.toolTip(
-0000f900: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
-0000f910: 7265 7475 726e 0a20 2020 2020 2020 2069  return.        i
-0000f920: 6620 7365 6c66 2e63 773a 0a20 2020 2020  f self.cw:.     
-0000f930: 2020 2020 2020 2073 656c 662e 6377 2e73         self.cw.s
-0000f940: 656e 6463 7728 7365 6c66 2e70 726f 6365  endcw(self.proce
-0000f950: 7373 5f6d 6163 726f 2873 656c 662e 4636  ss_macro(self.F6
-0000f960: 2e74 6f6f 6c54 6970 2829 2929 0a0a 2020  .toolTip()))..  
-0000f970: 2020 6465 6620 7365 6e64 6637 2873 656c    def sendf7(sel
-0000f980: 6629 3a0a 2020 2020 2020 2020 2222 2273  f):.        """s
-0000f990: 7475 6222 2222 0a20 2020 2020 2020 206c  tub""".        l
-0000f9a0: 6f67 6765 722e 6465 6275 6728 2246 3720  ogger.debug("F7 
-0000f9b0: 436c 6963 6b65 6422 290a 2020 2020 2020  Clicked").      
-0000f9c0: 2020 6966 2073 656c 662e 6e31 6d6d 3a0a    if self.n1mm:.
-0000f9d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f9e0: 2e6e 316d 6d2e 7261 6469 6f5f 696e 666f  .n1mm.radio_info
-0000f9f0: 5b22 4675 6e63 7469 6f6e 4b65 7943 6170  ["FunctionKeyCap
-0000fa00: 7469 6f6e 225d 203d 2073 656c 662e 4637  tion"] = self.F7
-0000fa10: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
-0000fa20: 6966 2073 656c 662e 7261 6469 6f5f 7374  if self.radio_st
-0000fa30: 6174 652e 6765 7428 226d 6f64 6522 2920  ate.get("mode") 
-0000fa40: 696e 205b 224c 5342 222c 2022 5553 4222  in ["LSB", "USB"
-0000fa50: 2c20 2253 5342 225d 3a0a 2020 2020 2020  , "SSB"]:.      
-0000fa60: 2020 2020 2020 7365 6c66 2e76 6f69 6365        self.voice
-0000fa70: 5f73 7472 696e 6728 7365 6c66 2e70 726f  _string(self.pro
-0000fa80: 6365 7373 5f6d 6163 726f 2873 656c 662e  cess_macro(self.
-0000fa90: 4637 2e74 6f6f 6c54 6970 2829 2929 0a20  F7.toolTip())). 
-0000faa0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000fab0: 6e0a 2020 2020 2020 2020 6966 2073 656c  n.        if sel
-0000fac0: 662e 6377 3a0a 2020 2020 2020 2020 2020  f.cw:.          
-0000fad0: 2020 7365 6c66 2e63 772e 7365 6e64 6377    self.cw.sendcw
-0000fae0: 2873 656c 662e 7072 6f63 6573 735f 6d61  (self.process_ma
-0000faf0: 6372 6f28 7365 6c66 2e46 372e 746f 6f6c  cro(self.F7.tool
-0000fb00: 5469 7028 2929 290a 0a20 2020 2064 6566  Tip()))..    def
-0000fb10: 2073 656e 6466 3828 7365 6c66 293a 0a20   sendf8(self):. 
-0000fb20: 2020 2020 2020 2022 2222 7374 7562 2222         """stub""
-0000fb30: 220a 2020 2020 2020 2020 6c6f 6767 6572  ".        logger
-0000fb40: 2e64 6562 7567 2822 4638 2043 6c69 636b  .debug("F8 Click
-0000fb50: 6564 2229 0a20 2020 2020 2020 2069 6620  ed").        if 
-0000fb60: 7365 6c66 2e6e 316d 6d3a 0a20 2020 2020  self.n1mm:.     
-0000fb70: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
-0000fb80: 2e72 6164 696f 5f69 6e66 6f5b 2246 756e  .radio_info["Fun
-0000fb90: 6374 696f 6e4b 6579 4361 7074 696f 6e22  ctionKeyCaption"
-0000fba0: 5d20 3d20 7365 6c66 2e46 382e 7465 7874  ] = self.F8.text
-0000fbb0: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-0000fbc0: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
-0000fbd0: 6574 2822 6d6f 6465 2229 2069 6e20 5b22  et("mode") in ["
-0000fbe0: 4c53 4222 2c20 2255 5342 222c 2022 5353  LSB", "USB", "SS
-0000fbf0: 4222 5d3a 0a20 2020 2020 2020 2020 2020  B"]:.           
-0000fc00: 2073 656c 662e 766f 6963 655f 7374 7269   self.voice_stri
-0000fc10: 6e67 2873 656c 662e 7072 6f63 6573 735f  ng(self.process_
-0000fc20: 6d61 6372 6f28 7365 6c66 2e46 382e 746f  macro(self.F8.to
-0000fc30: 6f6c 5469 7028 2929 290a 2020 2020 2020  olTip())).      
-0000fc40: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-0000fc50: 2020 2020 2069 6620 7365 6c66 2e63 773a       if self.cw:
-0000fc60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000fc70: 662e 6377 2e73 656e 6463 7728 7365 6c66  f.cw.sendcw(self
-0000fc80: 2e70 726f 6365 7373 5f6d 6163 726f 2873  .process_macro(s
-0000fc90: 656c 662e 4638 2e74 6f6f 6c54 6970 2829  elf.F8.toolTip()
-0000fca0: 2929 0a0a 2020 2020 6465 6620 7365 6e64  ))..    def send
-0000fcb0: 6639 2873 656c 6629 3a0a 2020 2020 2020  f9(self):.      
-0000fcc0: 2020 2222 2273 7475 6222 2222 0a20 2020    """stub""".   
-0000fcd0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-0000fce0: 6728 2246 3920 436c 6963 6b65 6422 290a  g("F9 Clicked").
+00009f60: 2020 2020 6461 656d 6f6e 3d54 7275 652c      daemon=True,
+00009f70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009f80: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00009f90: 2020 2020 2020 2020 2020 205f 7468 6574             _thet
+00009fa0: 6872 6561 642e 7374 6172 7428 290a 2020  hread.start().  
+00009fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009fc0: 2020 6e65 7874 5f74 6162 203d 2073 656c    next_tab = sel
+00009fd0: 662e 7461 625f 6e65 7874 2e67 6574 2873  f.tab_next.get(s
+00009fe0: 656c 662e 6361 6c6c 7369 676e 290a 2020  elf.callsign).  
+00009ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a000: 2020 6e65 7874 5f74 6162 2e73 6574 466f    next_tab.setFo
+0000a010: 6375 7328 290a 2020 2020 2020 2020 2020  cus().          
+0000a020: 2020 2020 2020 2020 2020 6e65 7874 5f74            next_t
+0000a030: 6162 2e64 6573 656c 6563 7428 290a 2020  ab.deselect().  
+0000a040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a050: 2020 6e65 7874 5f74 6162 2e65 6e64 2846    next_tab.end(F
+0000a060: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
+0000a070: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+0000a080: 2020 2020 2069 6620 6576 656e 742e 6b65       if event.ke
+0000a090: 7928 2920 3d3d 2051 742e 4b65 795f 4631  y() == Qt.Key_F1
+0000a0a0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000a0b0: 6c66 2e73 656e 6466 3128 290a 2020 2020  lf.sendf1().    
+0000a0c0: 2020 2020 6966 2065 7665 6e74 2e6b 6579      if event.key
+0000a0d0: 2829 203d 3d20 5174 2e4b 6579 5f46 323a  () == Qt.Key_F2:
+0000a0e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000a0f0: 662e 7365 6e64 6632 2829 0a20 2020 2020  f.sendf2().     
+0000a100: 2020 2069 6620 6576 656e 742e 6b65 7928     if event.key(
+0000a110: 2920 3d3d 2051 742e 4b65 795f 4633 3a0a  ) == Qt.Key_F3:.
+0000a120: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000a130: 2e73 656e 6466 3328 290a 2020 2020 2020  .sendf3().      
+0000a140: 2020 6966 2065 7665 6e74 2e6b 6579 2829    if event.key()
+0000a150: 203d 3d20 5174 2e4b 6579 5f46 343a 0a20   == Qt.Key_F4:. 
+0000a160: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000a170: 7365 6e64 6634 2829 0a20 2020 2020 2020  sendf4().       
+0000a180: 2069 6620 6576 656e 742e 6b65 7928 2920   if event.key() 
+0000a190: 3d3d 2051 742e 4b65 795f 4635 3a0a 2020  == Qt.Key_F5:.  
+0000a1a0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+0000a1b0: 656e 6466 3528 290a 2020 2020 2020 2020  endf5().        
+0000a1c0: 6966 2065 7665 6e74 2e6b 6579 2829 203d  if event.key() =
+0000a1d0: 3d20 5174 2e4b 6579 5f46 363a 0a20 2020  = Qt.Key_F6:.   
+0000a1e0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+0000a1f0: 6e64 6636 2829 0a20 2020 2020 2020 2069  ndf6().        i
+0000a200: 6620 6576 656e 742e 6b65 7928 2920 3d3d  f event.key() ==
+0000a210: 2051 742e 4b65 795f 4637 3a0a 2020 2020   Qt.Key_F7:.    
+0000a220: 2020 2020 2020 2020 7365 6c66 2e73 656e          self.sen
+0000a230: 6466 3728 290a 2020 2020 2020 2020 6966  df7().        if
+0000a240: 2065 7665 6e74 2e6b 6579 2829 203d 3d20   event.key() == 
+0000a250: 5174 2e4b 6579 5f46 383a 0a20 2020 2020  Qt.Key_F8:.     
+0000a260: 2020 2020 2020 2073 656c 662e 7365 6e64         self.send
+0000a270: 6638 2829 0a20 2020 2020 2020 2069 6620  f8().        if 
+0000a280: 6576 656e 742e 6b65 7928 2920 3d3d 2051  event.key() == Q
+0000a290: 742e 4b65 795f 4639 3a0a 2020 2020 2020  t.Key_F9:.      
+0000a2a0: 2020 2020 2020 7365 6c66 2e73 656e 6466        self.sendf
+0000a2b0: 3928 290a 2020 2020 2020 2020 6966 2065  9().        if e
+0000a2c0: 7665 6e74 2e6b 6579 2829 203d 3d20 5174  vent.key() == Qt
+0000a2d0: 2e4b 6579 5f46 3130 3a0a 2020 2020 2020  .Key_F10:.      
+0000a2e0: 2020 2020 2020 7365 6c66 2e73 656e 6466        self.sendf
+0000a2f0: 3130 2829 0a20 2020 2020 2020 2069 6620  10().        if 
+0000a300: 6576 656e 742e 6b65 7928 2920 3d3d 2051  event.key() == Q
+0000a310: 742e 4b65 795f 4631 313a 0a20 2020 2020  t.Key_F11:.     
+0000a320: 2020 2020 2020 2073 656c 662e 7365 6e64         self.send
+0000a330: 6631 3128 290a 2020 2020 2020 2020 6966  f11().        if
+0000a340: 2065 7665 6e74 2e6b 6579 2829 203d 3d20   event.key() == 
+0000a350: 5174 2e4b 6579 5f46 3132 3a0a 2020 2020  Qt.Key_F12:.    
+0000a360: 2020 2020 2020 2020 7365 6c66 2e73 656e          self.sen
+0000a370: 6466 3132 2829 0a0a 2020 2020 6465 6620  df12()..    def 
+0000a380: 7365 745f 7769 6e64 6f77 5f74 6974 6c65  set_window_title
+0000a390: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000a3a0: 2222 2253 6574 2077 696e 646f 7720 7469  """Set window ti
+0000a3b0: 746c 6522 2222 0a20 2020 2020 2020 2076  tle""".        v
+0000a3c0: 666f 6120 3d20 7365 6c66 2e72 6164 696f  foa = self.radio
+0000a3d0: 5f73 7461 7465 2e67 6574 2822 7666 6f61  _state.get("vfoa
+0000a3e0: 222c 2022 2229 0a20 2020 2020 2020 2069  ", "").        i
+0000a3f0: 6620 7666 6f61 3a0a 2020 2020 2020 2020  f vfoa:.        
+0000a400: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+0000a410: 2020 2020 2020 2020 2076 666f 6120 3d20           vfoa = 
+0000a420: 696e 7428 7666 6f61 2920 2f20 3130 3030  int(vfoa) / 1000
+0000a430: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
+0000a440: 6570 7420 5661 6c75 6545 7272 6f72 3a0a  ept ValueError:.
+0000a450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a460: 7666 6f61 203d 2030 2e30 0a20 2020 2020  vfoa = 0.0.     
+0000a470: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000a480: 2020 2020 2076 666f 6120 3d20 302e 300a       vfoa = 0.0.
+0000a490: 2020 2020 2020 2020 636f 6e74 6573 745f          contest_
+0000a4a0: 6e61 6d65 203d 2022 220a 2020 2020 2020  name = "".      
+0000a4b0: 2020 6966 2073 656c 662e 636f 6e74 6573    if self.contes
+0000a4c0: 743a 0a20 2020 2020 2020 2020 2020 2063  t:.            c
+0000a4d0: 6f6e 7465 7374 5f6e 616d 6520 3d20 7365  ontest_name = se
+0000a4e0: 6c66 2e63 6f6e 7465 7374 2e6e 616d 650a  lf.contest.name.
+0000a4f0: 2020 2020 2020 2020 6c69 6e65 203d 2028          line = (
+0000a500: 0a20 2020 2020 2020 2020 2020 2066 2276  .            f"v
+0000a510: 666f 613a 7b72 6f75 6e64 2876 666f 612c  foa:{round(vfoa,
+0000a520: 3229 7d20 220a 2020 2020 2020 2020 2020  2)} ".          
+0000a530: 2020 6622 6d6f 6465 3a7b 7365 6c66 2e72    f"mode:{self.r
+0000a540: 6164 696f 5f73 7461 7465 2e67 6574 2827  adio_state.get('
+0000a550: 6d6f 6465 272c 2027 2729 7d20 220a 2020  mode', '')} ".  
+0000a560: 2020 2020 2020 2020 2020 6622 4f50 3a7b            f"OP:{
+0000a570: 7365 6c66 2e63 7572 7265 6e74 5f6f 707d  self.current_op}
+0000a580: 207b 636f 6e74 6573 745f 6e61 6d65 7d20   {contest_name} 
+0000a590: 220a 2020 2020 2020 2020 2020 2020 6622  ".            f"
+0000a5a0: 2d20 4e6f 7431 4d4d 2076 7b5f 5f76 6572  - Not1MM v{__ver
+0000a5b0: 7369 6f6e 5f5f 7d22 0a20 2020 2020 2020  sion__}".       
+0000a5c0: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
+0000a5d0: 7365 7457 696e 646f 7754 6974 6c65 286c  setWindowTitle(l
+0000a5e0: 696e 6529 0a0a 2020 2020 6465 6620 7365  ine)..    def se
+0000a5f0: 6e64 5f77 6f72 6b65 645f 6c69 7374 2873  nd_worked_list(s
+0000a600: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
+0000a610: 2020 2020 2020 2222 2253 656e 6420 6d65        """Send me
+0000a620: 7373 6167 6520 636f 6e74 6169 6e69 6e67  ssage containing
+0000a630: 2077 6f72 6b65 6420 636f 6e74 6163 7473   worked contacts
+0000a640: 2061 6e64 2062 616e 6473 2222 220a 2020   and bands""".  
+0000a650: 2020 2020 2020 636d 6420 3d20 7b7d 0a20        cmd = {}. 
+0000a660: 2020 2020 2020 2063 6d64 5b22 636d 6422         cmd["cmd"
+0000a670: 5d20 3d20 2257 4f52 4b45 4422 0a20 2020  ] = "WORKED".   
+0000a680: 2020 2020 2063 6d64 5b22 7374 6174 696f       cmd["statio
+0000a690: 6e22 5d20 3d20 706c 6174 666f 726d 2e6e  n"] = platform.n
+0000a6a0: 6f64 6528 290a 2020 2020 2020 2020 636d  ode().        cm
+0000a6b0: 645b 2277 6f72 6b65 6422 5d20 3d20 7365  d["worked"] = se
+0000a6c0: 6c66 2e77 6f72 6b65 645f 6c69 7374 0a20  lf.worked_list. 
+0000a6d0: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+0000a6e0: 6275 6728 2225 7322 2c20 6622 7b63 6d64  bug("%s", f"{cmd
+0000a6f0: 7d22 290a 2020 2020 2020 2020 7365 6c66  }").        self
+0000a700: 2e6d 756c 7469 6361 7374 5f69 6e74 6572  .multicast_inter
+0000a710: 6661 6365 2e73 656e 645f 6173 5f6a 736f  face.send_as_jso
+0000a720: 6e28 636d 6429 0a0a 2020 2020 6465 6620  n(cmd)..    def 
+0000a730: 636c 6561 7269 6e70 7574 7328 7365 6c66  clearinputs(self
+0000a740: 293a 0a20 2020 2020 2020 2022 2222 436c  ):.        """Cl
+0000a750: 6561 7273 2074 6865 2074 6578 7420 696e  ears the text in
+0000a760: 7075 7420 6669 656c 6473 2061 6e64 2073  put fields and s
+0000a770: 6574 7320 666f 6375 7320 746f 2063 616c  ets focus to cal
+0000a780: 6c73 6967 6e20 6669 656c 642e 2222 220a  lsign field.""".
+0000a790: 2020 2020 2020 2020 7365 6c66 2e64 7570          self.dup
+0000a7a0: 655f 696e 6469 6361 746f 722e 6869 6465  e_indicator.hide
+0000a7b0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+0000a7c0: 636f 6e74 6163 7420 3d20 7365 6c66 2e64  contact = self.d
+0000a7d0: 6174 6162 6173 652e 656d 7074 795f 636f  atabase.empty_co
+0000a7e0: 6e74 6163 740a 2020 2020 2020 2020 7365  ntact.        se
+0000a7f0: 6c66 2e68 6561 6469 6e67 5f64 6973 7461  lf.heading_dista
+0000a800: 6e63 652e 7365 7454 6578 7428 2222 290a  nce.setText("").
+0000a810: 2020 2020 2020 2020 7365 6c66 2e64 785f          self.dx_
+0000a820: 656e 7469 7479 2e73 6574 5465 7874 2822  entity.setText("
+0000a830: 2229 0a20 2020 2020 2020 2069 6620 7365  ").        if se
+0000a840: 6c66 2e63 6f6e 7465 7374 3a0a 2020 2020  lf.contest:.    
+0000a850: 2020 2020 2020 2020 6d75 6c74 7320 3d20          mults = 
+0000a860: 7365 6c66 2e63 6f6e 7465 7374 2e73 686f  self.contest.sho
+0000a870: 775f 6d75 6c74 7328 7365 6c66 290a 2020  w_mults(self).  
+0000a880: 2020 2020 2020 2020 2020 7173 6f73 203d            qsos =
+0000a890: 2073 656c 662e 636f 6e74 6573 742e 7368   self.contest.sh
+0000a8a0: 6f77 5f71 736f 2873 656c 6629 0a20 2020  ow_qso(self).   
+0000a8b0: 2020 2020 2020 2020 206d 756c 7473 7472           multstr
+0000a8c0: 696e 6720 3d20 6622 7b71 736f 737d 2f7b  ing = f"{qsos}/{
+0000a8d0: 6d75 6c74 737d 220a 2020 2020 2020 2020  mults}".        
+0000a8e0: 2020 2020 7365 6c66 2e6d 756c 7473 2e73      self.mults.s
+0000a8f0: 6574 5465 7874 286d 756c 7473 7472 696e  etText(multstrin
+0000a900: 6729 0a20 2020 2020 2020 2020 2020 2073  g).            s
+0000a910: 636f 7265 203d 2073 656c 662e 636f 6e74  core = self.cont
+0000a920: 6573 742e 6361 6c63 5f73 636f 7265 2873  est.calc_score(s
+0000a930: 656c 6629 0a20 2020 2020 2020 2020 2020  elf).           
+0000a940: 2073 656c 662e 7363 6f72 652e 7365 7454   self.score.setT
+0000a950: 6578 7428 7374 7228 7363 6f72 6529 290a  ext(str(score)).
+0000a960: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000a970: 2e63 6f6e 7465 7374 2e72 6573 6574 5f6c  .contest.reset_l
+0000a980: 6162 656c 2873 656c 6629 0a20 2020 2020  abel(self).     
+0000a990: 2020 2073 656c 662e 6361 6c6c 7369 676e     self.callsign
+0000a9a0: 2e63 6c65 6172 2829 0a20 2020 2020 2020  .clear().       
+0000a9b0: 2069 6620 7365 6c66 2e63 7572 7265 6e74   if self.current
+0000a9c0: 5f6d 6f64 6520 3d3d 2022 4357 223a 0a20  _mode == "CW":. 
+0000a9d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000a9e0: 7365 6e74 2e73 6574 5465 7874 2822 3539  sent.setText("59
+0000a9f0: 3922 290a 2020 2020 2020 2020 2020 2020  9").            
+0000aa00: 7365 6c66 2e72 6563 6569 7665 2e73 6574  self.receive.set
+0000aa10: 5465 7874 2822 3539 3922 290a 2020 2020  Text("599").    
+0000aa20: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000aa30: 2020 2020 2020 7365 6c66 2e73 656e 742e        self.sent.
+0000aa40: 7365 7454 6578 7428 2235 3922 290a 2020  setText("59").  
+0000aa50: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+0000aa60: 6563 6569 7665 2e73 6574 5465 7874 2822  eceive.setText("
+0000aa70: 3539 2229 0a20 2020 2020 2020 2073 656c  59").        sel
+0000aa80: 662e 6f74 6865 725f 312e 636c 6561 7228  f.other_1.clear(
+0000aa90: 290a 2020 2020 2020 2020 7365 6c66 2e6f  ).        self.o
+0000aaa0: 7468 6572 5f32 2e63 6c65 6172 2829 0a20  ther_2.clear(). 
+0000aab0: 2020 2020 2020 2073 656c 662e 6361 6c6c         self.call
+0000aac0: 7369 676e 2e73 6574 466f 6375 7328 290a  sign.setFocus().
+0000aad0: 2020 2020 2020 2020 636d 6420 3d20 7b7d          cmd = {}
+0000aae0: 0a20 2020 2020 2020 2063 6d64 5b22 636d  .        cmd["cm
+0000aaf0: 6422 5d20 3d20 2243 414c 4c43 4841 4e47  d"] = "CALLCHANG
+0000ab00: 4544 220a 2020 2020 2020 2020 636d 645b  ED".        cmd[
+0000ab10: 2273 7461 7469 6f6e 225d 203d 2070 6c61  "station"] = pla
+0000ab20: 7466 6f72 6d2e 6e6f 6465 2829 0a20 2020  tform.node().   
+0000ab30: 2020 2020 2063 6d64 5b22 6361 6c6c 225d       cmd["call"]
+0000ab40: 203d 2022 220a 2020 2020 2020 2020 7365   = "".        se
+0000ab50: 6c66 2e6d 756c 7469 6361 7374 5f69 6e74  lf.multicast_int
+0000ab60: 6572 6661 6365 2e73 656e 645f 6173 5f6a  erface.send_as_j
+0000ab70: 736f 6e28 636d 6429 0a0a 2020 2020 6465  son(cmd)..    de
+0000ab80: 6620 7361 7665 5f63 6f6e 7461 6374 2873  f save_contact(s
+0000ab90: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+0000aba0: 2253 6176 6520 746f 2064 6222 2222 0a20  "Save to db""". 
+0000abb0: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+0000abc0: 6275 6728 2273 6176 696e 6720 636f 6e74  bug("saving cont
+0000abd0: 6163 7422 290a 2020 2020 2020 2020 6966  act").        if
+0000abe0: 2073 656c 662e 636f 6e74 6573 7420 6973   self.contest is
+0000abf0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000ac00: 2020 2073 656c 662e 7368 6f77 5f6d 6573     self.show_mes
+0000ac10: 7361 6765 5f62 6f78 2822 596f 7520 6861  sage_box("You ha
+0000ac20: 7665 206e 6f20 636f 6e74 6573 7420 6465  ve no contest de
+0000ac30: 6669 6e65 642e 2229 0a20 2020 2020 2020  fined.").       
+0000ac40: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+0000ac50: 2020 2020 6966 206c 656e 2873 656c 662e      if len(self.
+0000ac60: 6361 6c6c 7369 676e 2e74 6578 7428 2929  callsign.text())
+0000ac70: 203c 2033 3a0a 2020 2020 2020 2020 2020   < 3:.          
+0000ac80: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+0000ac90: 2069 6620 6e6f 7420 616e 7928 6368 6172   if not any(char
+0000aca0: 2e69 7364 6967 6974 2829 2066 6f72 2063  .isdigit() for c
+0000acb0: 6861 7220 696e 2073 656c 662e 6361 6c6c  har in self.call
+0000acc0: 7369 676e 2e74 6578 7428 2929 3a0a 2020  sign.text()):.  
+0000acd0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000ace0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+0000acf0: 616e 7928 6368 6172 2e69 7361 6c70 6861  any(char.isalpha
+0000ad00: 2829 2066 6f72 2063 6861 7220 696e 2073  () for char in s
+0000ad10: 656c 662e 6361 6c6c 7369 676e 2e74 6578  elf.callsign.tex
+0000ad20: 7428 2929 3a0a 2020 2020 2020 2020 2020  t()):.          
+0000ad30: 2020 7265 7475 726e 0a0a 2020 2020 2020    return..      
+0000ad40: 2020 7365 6c66 2e63 6f6e 7461 6374 5b22    self.contact["
+0000ad50: 5453 225d 203d 2064 6174 6574 696d 652e  TS"] = datetime.
+0000ad60: 7574 636e 6f77 2829 2e69 736f 666f 726d  utcnow().isoform
+0000ad70: 6174 2822 2022 295b 3a31 395d 0a20 2020  at(" ")[:19].   
+0000ad80: 2020 2020 2073 656c 662e 636f 6e74 6163       self.contac
+0000ad90: 745b 2243 616c 6c22 5d20 3d20 7365 6c66  t["Call"] = self
+0000ada0: 2e63 616c 6c73 6967 6e2e 7465 7874 2829  .callsign.text()
+0000adb0: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
+0000adc0: 6e74 6163 745b 2246 7265 7122 5d20 3d20  ntact["Freq"] = 
+0000add0: 726f 756e 6428 666c 6f61 7428 7365 6c66  round(float(self
+0000ade0: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
+0000adf0: 2822 7666 6f61 222c 2030 2e30 2929 202f  ("vfoa", 0.0)) /
+0000ae00: 2031 3030 302c 2032 290a 2020 2020 2020   1000, 2).      
+0000ae10: 2020 7365 6c66 2e63 6f6e 7461 6374 5b22    self.contact["
+0000ae20: 5153 5846 7265 7122 5d20 3d20 726f 756e  QSXFreq"] = roun
+0000ae30: 6428 0a20 2020 2020 2020 2020 2020 2066  d(.            f
+0000ae40: 6c6f 6174 2873 656c 662e 7261 6469 6f5f  loat(self.radio_
+0000ae50: 7374 6174 652e 6765 7428 2276 666f 6122  state.get("vfoa"
+0000ae60: 2c20 302e 3029 2920 2f20 3130 3030 2c20  , 0.0)) / 1000, 
+0000ae70: 320a 2020 2020 2020 2020 290a 2020 2020  2.        ).    
+0000ae80: 2020 2020 7365 6c66 2e63 6f6e 7461 6374      self.contact
+0000ae90: 5b22 4d6f 6465 225d 203d 2073 656c 662e  ["Mode"] = self.
+0000aea0: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
+0000aeb0: 226d 6f64 6522 2c20 2222 290a 2020 2020  "mode", "").    
+0000aec0: 2020 2020 7365 6c66 2e63 6f6e 7461 6374      self.contact
+0000aed0: 5b22 436f 6e74 6573 744e 616d 6522 5d20  ["ContestName"] 
+0000aee0: 3d20 7365 6c66 2e63 6f6e 7465 7374 2e63  = self.contest.c
+0000aef0: 6162 7269 6c6c 6f5f 6e61 6d65 0a20 2020  abrillo_name.   
+0000af00: 2020 2020 2073 656c 662e 636f 6e74 6163       self.contac
+0000af10: 745b 2243 6f6e 7465 7374 4e52 225d 203d  t["ContestNR"] =
+0000af20: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
+0000af30: 636f 6e74 6573 7422 2c20 2230 2229 0a20  contest", "0"). 
+0000af40: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
+0000af50: 6163 745b 2253 7461 7469 6f6e 5072 6566  act["StationPref
+0000af60: 6978 225d 203d 2073 656c 662e 7374 6174  ix"] = self.stat
+0000af70: 696f 6e2e 6765 7428 2243 616c 6c22 2c20  ion.get("Call", 
+0000af80: 2222 290a 2020 2020 2020 2020 7365 6c66  "").        self
+0000af90: 2e63 6f6e 7461 6374 5b22 5750 5850 7265  .contact["WPXPre
+0000afa0: 6669 7822 5d20 3d20 6361 6c63 756c 6174  fix"] = calculat
+0000afb0: 655f 7770 785f 7072 6566 6978 2873 656c  e_wpx_prefix(sel
+0000afc0: 662e 6361 6c6c 7369 676e 2e74 6578 7428  f.callsign.text(
+0000afd0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+0000afe0: 636f 6e74 6163 745b 2249 7352 756e 5153  contact["IsRunQS
+0000aff0: 4f22 5d20 3d20 7365 6c66 2e72 6164 696f  O"] = self.radio
+0000b000: 4275 7474 6f6e 5f72 756e 2e69 7343 6865  Button_run.isChe
+0000b010: 636b 6564 2829 0a20 2020 2020 2020 2073  cked().        s
+0000b020: 656c 662e 636f 6e74 6163 745b 224f 7065  elf.contact["Ope
+0000b030: 7261 746f 7222 5d20 3d20 7365 6c66 2e63  rator"] = self.c
+0000b040: 7572 7265 6e74 5f6f 700a 2020 2020 2020  urrent_op.      
+0000b050: 2020 7365 6c66 2e63 6f6e 7461 6374 5b22    self.contact["
+0000b060: 4e65 7442 696f 734e 616d 6522 5d20 3d20  NetBiosName"] = 
+0000b070: 736f 636b 6574 2e67 6574 686f 7374 6e61  socket.gethostna
+0000b080: 6d65 2829 0a20 2020 2020 2020 2073 656c  me().        sel
+0000b090: 662e 636f 6e74 6163 745b 2249 734f 7269  f.contact["IsOri
+0000b0a0: 6769 6e61 6c22 5d20 3d20 310a 2020 2020  ginal"] = 1.    
+0000b0b0: 2020 2020 7365 6c66 2e63 6f6e 7461 6374      self.contact
+0000b0c0: 5b22 4944 225d 203d 2075 7569 642e 7575  ["ID"] = uuid.uu
+0000b0d0: 6964 3428 292e 6865 780a 2020 2020 2020  id4().hex.      
+0000b0e0: 2020 7365 6c66 2e63 6f6e 7465 7374 2e73    self.contest.s
+0000b0f0: 6574 5f63 6f6e 7461 6374 5f76 6172 7328  et_contact_vars(
+0000b100: 7365 6c66 290a 2020 2020 2020 2020 7365  self).        se
+0000b110: 6c66 2e63 6f6e 7461 6374 5b22 506f 696e  lf.contact["Poin
+0000b120: 7473 225d 203d 2073 656c 662e 636f 6e74  ts"] = self.cont
+0000b130: 6573 742e 706f 696e 7473 2873 656c 6629  est.points(self)
+0000b140: 0a20 2020 2020 2020 2064 6562 7567 5f6f  .        debug_o
+0000b150: 7574 7075 7420 3d20 6622 7b73 656c 662e  utput = f"{self.
+0000b160: 636f 6e74 6163 747d 220a 2020 2020 2020  contact}".      
+0000b170: 2020 6c6f 6767 6572 2e64 6562 7567 2864    logger.debug(d
+0000b180: 6562 7567 5f6f 7574 7075 7429 0a0a 2020  ebug_output)..  
+0000b190: 2020 2020 2020 6966 2073 656c 662e 6e31        if self.n1
+0000b1a0: 6d6d 3a0a 2020 2020 2020 2020 2020 2020  mm:.            
+0000b1b0: 6c6f 6767 6572 2e64 6562 7567 2822 7061  logger.debug("pa
+0000b1c0: 636b 6574 7320 2573 222c 2066 227b 7365  ckets %s", f"{se
+0000b1d0: 6c66 2e6e 316d 6d2e 7365 6e64 5f63 6f6e  lf.n1mm.send_con
+0000b1e0: 7461 6374 5f70 6163 6b65 7473 7d22 290a  tact_packets}").
+0000b1f0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000b200: 656c 662e 6e31 6d6d 2e73 656e 645f 636f  elf.n1mm.send_co
+0000b210: 6e74 6163 745f 7061 636b 6574 733a 0a20  ntact_packets:. 
+0000b220: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000b230: 656c 662e 6e31 6d6d 2e63 6f6e 7461 6374  elf.n1mm.contact
+0000b240: 5f69 6e66 6f5b 2274 696d 6573 7461 6d70  _info["timestamp
+0000b250: 225d 203d 2073 656c 662e 636f 6e74 6163  "] = self.contac
+0000b260: 745b 2254 5322 5d0a 2020 2020 2020 2020  t["TS"].        
+0000b270: 2020 2020 2020 2020 7365 6c66 2e6e 316d          self.n1m
+0000b280: 6d2e 636f 6e74 6163 745f 696e 666f 5b22  m.contact_info["
+0000b290: 6f6c 6463 616c 6c22 5d20 3d20 7365 6c66  oldcall"] = self
+0000b2a0: 2e6e 316d 6d2e 636f 6e74 6163 745f 696e  .n1mm.contact_in
+0000b2b0: 666f 5b0a 2020 2020 2020 2020 2020 2020  fo[.            
+0000b2c0: 2020 2020 2020 2020 2263 616c 6c22 0a20          "call". 
+0000b2d0: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+0000b2e0: 203d 2073 656c 662e 636f 6e74 6163 745b   = self.contact[
+0000b2f0: 2243 616c 6c22 5d0a 2020 2020 2020 2020  "Call"].        
+0000b300: 2020 2020 2020 2020 7365 6c66 2e6e 316d          self.n1m
+0000b310: 6d2e 636f 6e74 6163 745f 696e 666f 5b22  m.contact_info["
+0000b320: 7478 6672 6571 225d 203d 2073 656c 662e  txfreq"] = self.
+0000b330: 6e31 6d6d 2e63 6f6e 7461 6374 5f69 6e66  n1mm.contact_inf
+0000b340: 6f5b 0a20 2020 2020 2020 2020 2020 2020  o[.             
+0000b350: 2020 2020 2020 2022 7278 6672 6571 220a         "rxfreq".
+0000b360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b370: 5d20 3d20 7365 6c66 2e6e 316d 6d2e 7261  ] = self.n1mm.ra
+0000b380: 6469 6f5f 696e 666f 5b22 4672 6571 225d  dio_info["Freq"]
+0000b390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b3a0: 2073 656c 662e 6e31 6d6d 2e63 6f6e 7461   self.n1mm.conta
+0000b3b0: 6374 5f69 6e66 6f5b 226d 6f64 6522 5d20  ct_info["mode"] 
+0000b3c0: 3d20 7365 6c66 2e63 6f6e 7461 6374 5b22  = self.contact["
+0000b3d0: 4d6f 6465 225d 0a20 2020 2020 2020 2020  Mode"].         
+0000b3e0: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
+0000b3f0: 2e63 6f6e 7461 6374 5f69 6e66 6f5b 2263  .contact_info["c
+0000b400: 6f6e 7465 7374 6e61 6d65 225d 203d 2073  ontestname"] = s
+0000b410: 656c 662e 636f 6e74 6163 745b 0a20 2020  elf.contact[.   
+0000b420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b430: 2022 436f 6e74 6573 744e 616d 6522 0a20   "ContestName". 
+0000b440: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+0000b450: 2e72 6570 6c61 6365 2822 2d22 2c20 2222  .replace("-", ""
+0000b460: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000b470: 2020 7365 6c66 2e6e 316d 6d2e 636f 6e74    self.n1mm.cont
+0000b480: 6163 745f 696e 666f 5b22 636f 6e74 6573  act_info["contes
+0000b490: 746e 7222 5d20 3d20 7365 6c66 2e63 6f6e  tnr"] = self.con
+0000b4a0: 7461 6374 5b22 436f 6e74 6573 744e 5222  tact["ContestNR"
+0000b4b0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0000b4c0: 2020 7365 6c66 2e6e 316d 6d2e 636f 6e74    self.n1mm.cont
+0000b4d0: 6163 745f 696e 666f 5b22 7374 6174 696f  act_info["statio
+0000b4e0: 6e70 7265 6669 7822 5d20 3d20 7365 6c66  nprefix"] = self
+0000b4f0: 2e63 6f6e 7461 6374 5b22 5374 6174 696f  .contact["Statio
+0000b500: 6e50 7265 6669 7822 5d0a 2020 2020 2020  nPrefix"].      
+0000b510: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+0000b520: 316d 6d2e 636f 6e74 6163 745f 696e 666f  1mm.contact_info
+0000b530: 5b22 7770 7870 7265 6669 7822 5d20 3d20  ["wpxprefix"] = 
+0000b540: 7365 6c66 2e63 6f6e 7461 6374 5b22 5750  self.contact["WP
+0000b550: 5850 7265 6669 7822 5d0a 2020 2020 2020  XPrefix"].      
+0000b560: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+0000b570: 316d 6d2e 636f 6e74 6163 745f 696e 666f  1mm.contact_info
+0000b580: 5b22 4973 5275 6e51 534f 225d 203d 2073  ["IsRunQSO"] = s
+0000b590: 656c 662e 636f 6e74 6163 745b 2249 7352  elf.contact["IsR
+0000b5a0: 756e 5153 4f22 5d0a 2020 2020 2020 2020  unQSO"].        
+0000b5b0: 2020 2020 2020 2020 7365 6c66 2e6e 316d          self.n1m
+0000b5c0: 6d2e 636f 6e74 6163 745f 696e 666f 5b22  m.contact_info["
+0000b5d0: 6f70 6572 6174 6f72 225d 203d 2073 656c  operator"] = sel
+0000b5e0: 662e 636f 6e74 6163 745b 224f 7065 7261  f.contact["Opera
+0000b5f0: 746f 7222 5d0a 2020 2020 2020 2020 2020  tor"].          
+0000b600: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
+0000b610: 636f 6e74 6163 745f 696e 666f 5b22 6d79  contact_info["my
+0000b620: 6361 6c6c 225d 203d 2073 656c 662e 636f  call"] = self.co
+0000b630: 6e74 6163 745b 224f 7065 7261 746f 7222  ntact["Operator"
+0000b640: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0000b650: 2020 7365 6c66 2e6e 316d 6d2e 636f 6e74    self.n1mm.cont
+0000b660: 6163 745f 696e 666f 5b22 5374 6174 696f  act_info["Statio
+0000b670: 6e4e 616d 6522 5d20 3d20 7365 6c66 2e6e  nName"] = self.n
+0000b680: 316d 6d2e 636f 6e74 6163 745f 696e 666f  1mm.contact_info
+0000b690: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+0000b6a0: 2020 2020 2020 224e 6574 4269 6f73 4e61        "NetBiosNa
+0000b6b0: 6d65 220a 2020 2020 2020 2020 2020 2020  me".            
+0000b6c0: 2020 2020 5d20 3d20 7365 6c66 2e63 6f6e      ] = self.con
+0000b6d0: 7461 6374 5b22 4e65 7442 696f 734e 616d  tact["NetBiosNam
+0000b6e0: 6522 5d0a 2020 2020 2020 2020 2020 2020  e"].            
+0000b6f0: 2020 2020 7365 6c66 2e6e 316d 6d2e 636f      self.n1mm.co
+0000b700: 6e74 6163 745f 696e 666f 5b22 4973 4f72  ntact_info["IsOr
+0000b710: 6967 696e 616c 225d 203d 2073 656c 662e  iginal"] = self.
+0000b720: 636f 6e74 6163 745b 2249 734f 7269 6769  contact["IsOrigi
+0000b730: 6e61 6c22 5d0a 2020 2020 2020 2020 2020  nal"].          
+0000b740: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
+0000b750: 636f 6e74 6163 745f 696e 666f 5b22 4944  contact_info["ID
+0000b760: 225d 203d 2073 656c 662e 636f 6e74 6163  "] = self.contac
+0000b770: 745b 2249 4422 5d0a 2020 2020 2020 2020  t["ID"].        
+0000b780: 2020 2020 2020 2020 7365 6c66 2e6e 316d          self.n1m
+0000b790: 6d2e 636f 6e74 6163 745f 696e 666f 5b22  m.contact_info["
+0000b7a0: 706f 696e 7473 225d 203d 2073 656c 662e  points"] = self.
+0000b7b0: 636f 6e74 6163 745b 2250 6f69 6e74 7322  contact["Points"
+0000b7c0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0000b7d0: 2020 7365 6c66 2e6e 316d 6d2e 636f 6e74    self.n1mm.cont
+0000b7e0: 6163 745f 696e 666f 5b22 736e 7422 5d20  act_info["snt"] 
+0000b7f0: 3d20 7365 6c66 2e63 6f6e 7461 6374 5b22  = self.contact["
+0000b800: 534e 5422 5d0a 2020 2020 2020 2020 2020  SNT"].          
+0000b810: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
+0000b820: 636f 6e74 6163 745f 696e 666f 5b22 7263  contact_info["rc
+0000b830: 7622 5d20 3d20 7365 6c66 2e63 6f6e 7461  v"] = self.conta
+0000b840: 6374 5b22 5243 5622 5d0a 2020 2020 2020  ct["RCV"].      
+0000b850: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+0000b860: 316d 6d2e 636f 6e74 6163 745f 696e 666f  1mm.contact_info
+0000b870: 5b22 736e 746e 7222 5d20 3d20 7365 6c66  ["sntnr"] = self
+0000b880: 2e63 6f6e 7461 6374 5b22 5365 6e74 4e72  .contact["SentNr
+0000b890: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+0000b8a0: 2020 2073 656c 662e 6e31 6d6d 2e63 6f6e     self.n1mm.con
+0000b8b0: 7461 6374 5f69 6e66 6f5b 2272 6376 6e72  tact_info["rcvnr
+0000b8c0: 225d 203d 2073 656c 662e 636f 6e74 6163  "] = self.contac
+0000b8d0: 745b 224e 5222 5d0a 2020 2020 2020 2020  t["NR"].        
+0000b8e0: 2020 2020 2020 2020 7365 6c66 2e6e 316d          self.n1m
+0000b8f0: 6d2e 636f 6e74 6163 745f 696e 666f 5b22  m.contact_info["
+0000b900: 6973 6d75 6c74 6970 6c69 6572 3122 5d20  ismultiplier1"] 
+0000b910: 3d20 7365 6c66 2e63 6f6e 7461 6374 2e67  = self.contact.g
+0000b920: 6574 280a 2020 2020 2020 2020 2020 2020  et(.            
+0000b930: 2020 2020 2020 2020 2249 734d 756c 7469          "IsMulti
+0000b940: 706c 6965 7231 222c 2030 0a20 2020 2020  plier1", 0.     
+0000b950: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000b960: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000b970: 662e 6e31 6d6d 2e63 6f6e 7461 6374 5f69  f.n1mm.contact_i
+0000b980: 6e66 6f5b 2269 736d 756c 7469 706c 6965  nfo["ismultiplie
+0000b990: 7232 225d 203d 2073 656c 662e 636f 6e74  r2"] = self.cont
+0000b9a0: 6163 742e 6765 7428 0a20 2020 2020 2020  act.get(.       
+0000b9b0: 2020 2020 2020 2020 2020 2020 2022 4973               "Is
+0000b9c0: 4d75 6c74 6970 6c69 6572 3222 2c20 300a  Multiplier2", 0.
+0000b9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b9e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000b9f0: 2020 7365 6c66 2e6e 316d 6d2e 636f 6e74    self.n1mm.cont
+0000ba00: 6163 745f 696e 666f 5b22 6973 6d75 6c74  act_info["ismult
+0000ba10: 6970 6c69 6572 3322 5d20 3d20 7365 6c66  iplier3"] = self
+0000ba20: 2e63 6f6e 7461 6374 2e67 6574 280a 2020  .contact.get(.  
+0000ba30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba40: 2020 2249 734d 756c 7469 706c 6965 7233    "IsMultiplier3
+0000ba50: 222c 2022 3022 0a20 2020 2020 2020 2020  ", "0".         
+0000ba60: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000ba70: 2020 2020 2020 2020 2073 656c 662e 6e31           self.n1
+0000ba80: 6d6d 2e63 6f6e 7461 6374 5f69 6e66 6f5b  mm.contact_info[
+0000ba90: 2273 6563 7469 6f6e 225d 203d 2073 656c  "section"] = sel
+0000baa0: 662e 636f 6e74 6163 745b 2253 6563 7422  f.contact["Sect"
+0000bab0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0000bac0: 2020 7365 6c66 2e6e 316d 6d2e 636f 6e74    self.n1mm.cont
+0000bad0: 6163 745f 696e 666f 5b22 7072 6563 225d  act_info["prec"]
+0000bae0: 203d 2073 656c 662e 636f 6e74 6163 745b   = self.contact[
+0000baf0: 2250 7265 6322 5d0a 2020 2020 2020 2020  "Prec"].        
+0000bb00: 2020 2020 2020 2020 7365 6c66 2e6e 316d          self.n1m
+0000bb10: 6d2e 636f 6e74 6163 745f 696e 666f 5b22  m.contact_info["
+0000bb20: 636b 225d 203d 2073 656c 662e 636f 6e74  ck"] = self.cont
+0000bb30: 6163 745b 2243 4b22 5d0a 2020 2020 2020  act["CK"].      
+0000bb40: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+0000bb50: 316d 6d2e 636f 6e74 6163 745f 696e 666f  1mm.contact_info
+0000bb60: 5b22 7a6e 225d 203d 2073 656c 662e 636f  ["zn"] = self.co
+0000bb70: 6e74 6163 745b 225a 4e22 5d0a 2020 2020  ntact["ZN"].    
+0000bb80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000bb90: 2e6e 316d 6d2e 636f 6e74 6163 745f 696e  .n1mm.contact_in
+0000bba0: 666f 5b22 706f 7765 7222 5d20 3d20 7365  fo["power"] = se
+0000bbb0: 6c66 2e63 6f6e 7461 6374 5b22 506f 7765  lf.contact["Powe
+0000bbc0: 7222 5d0a 2020 2020 2020 2020 2020 2020  r"].            
+0000bbd0: 2020 2020 7365 6c66 2e6e 316d 6d2e 636f      self.n1mm.co
+0000bbe0: 6e74 6163 745f 696e 666f 5b22 6261 6e64  ntact_info["band
+0000bbf0: 225d 203d 2073 656c 662e 636f 6e74 6163  "] = self.contac
+0000bc00: 745b 2242 616e 6422 5d0a 2020 2020 2020  t["Band"].      
+0000bc10: 2020 2020 2020 2020 2020 2320 7365 6c66            # self
+0000bc20: 2e6e 316d 6d2e 636f 6e74 6163 745f 696e  .n1mm.contact_in
+0000bc30: 666f 5b27 275d 0a20 2020 2020 2020 2020  fo[''].         
+0000bc40: 2020 2020 2020 2023 2073 656c 662e 6e31         # self.n1
+0000bc50: 6d6d 2e63 6f6e 7461 6374 5f69 6e66 6f5b  mm.contact_info[
+0000bc60: 2727 5d0a 2020 2020 2020 2020 2020 2020  ''].            
+0000bc70: 2020 2020 2320 7365 6c66 2e6e 316d 6d2e      # self.n1mm.
+0000bc80: 636f 6e74 6163 745f 696e 666f 5b27 275d  contact_info['']
+0000bc90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bca0: 2023 2073 656c 662e 6e31 6d6d 2e63 6f6e   # self.n1mm.con
+0000bcb0: 7461 6374 5f69 6e66 6f5b 2727 5d0a 2020  tact_info[''].  
+0000bcc0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000bcd0: 7365 6c66 2e6e 316d 6d2e 636f 6e74 6163  self.n1mm.contac
+0000bce0: 745f 696e 666f 5b27 275d 0a20 2020 2020  t_info[''].     
+0000bcf0: 2020 2020 2020 2020 2020 2023 2073 656c             # sel
+0000bd00: 662e 6e31 6d6d 2e63 6f6e 7461 6374 5f69  f.n1mm.contact_i
+0000bd10: 6e66 6f5b 2727 5d0a 2020 2020 2020 2020  nfo[''].        
+0000bd20: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+0000bd30: 6562 7567 2822 2573 222c 2066 227b 7365  ebug("%s", f"{se
+0000bd40: 6c66 2e6e 316d 6d2e 636f 6e74 6163 745f  lf.n1mm.contact_
+0000bd50: 696e 666f 7d22 290a 2020 2020 2020 2020  info}").        
+0000bd60: 2020 2020 2020 2020 7365 6c66 2e6e 316d          self.n1m
+0000bd70: 6d2e 7365 6e64 5f63 6f6e 7461 6374 5f69  m.send_contact_i
+0000bd80: 6e66 6f28 290a 0a20 2020 2020 2020 2073  nfo()..        s
+0000bd90: 656c 662e 6461 7461 6261 7365 2e6c 6f67  elf.database.log
+0000bda0: 5f63 6f6e 7461 6374 2873 656c 662e 636f  _contact(self.co
+0000bdb0: 6e74 6163 7429 0a20 2020 2020 2020 2073  ntact).        s
+0000bdc0: 656c 662e 776f 726b 6564 5f6c 6973 7420  elf.worked_list 
+0000bdd0: 3d20 7365 6c66 2e64 6174 6162 6173 652e  = self.database.
+0000bde0: 6765 745f 6361 6c6c 735f 616e 645f 6261  get_calls_and_ba
+0000bdf0: 6e64 7328 290a 2020 2020 2020 2020 7365  nds().        se
+0000be00: 6c66 2e73 656e 645f 776f 726b 6564 5f6c  lf.send_worked_l
+0000be10: 6973 7428 290a 2020 2020 2020 2020 7365  ist().        se
+0000be20: 6c66 2e63 6c65 6172 696e 7075 7473 2829  lf.clearinputs()
+0000be30: 0a0a 2020 2020 2020 2020 636d 6420 3d20  ..        cmd = 
+0000be40: 7b7d 0a20 2020 2020 2020 2063 6d64 5b22  {}.        cmd["
+0000be50: 636d 6422 5d20 3d20 2255 5044 4154 454c  cmd"] = "UPDATEL
+0000be60: 4f47 220a 2020 2020 2020 2020 636d 645b  OG".        cmd[
+0000be70: 2273 7461 7469 6f6e 225d 203d 2070 6c61  "station"] = pla
+0000be80: 7466 6f72 6d2e 6e6f 6465 2829 0a20 2020  tform.node().   
+0000be90: 2020 2020 2073 656c 662e 6d75 6c74 6963       self.multic
+0000bea0: 6173 745f 696e 7465 7266 6163 652e 7365  ast_interface.se
+0000beb0: 6e64 5f61 735f 6a73 6f6e 2863 6d64 290a  nd_as_json(cmd).
+0000bec0: 0a20 2020 2020 2020 2023 2073 656c 662e  .        # self.
+0000bed0: 636f 6e74 6163 745b 2243 6f6e 7465 7374  contact["Contest
+0000bee0: 4e61 6d65 225d 203d 2073 656c 662e 636f  Name"] = self.co
+0000bef0: 6e74 6573 742e 6e61 6d65 0a20 2020 2020  ntest.name.     
+0000bf00: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
+0000bf10: 745b 2253 4e54 225d 203d 2073 656c 662e  t["SNT"] = self.
+0000bf20: 7365 6e74 2e74 6578 7428 290a 2020 2020  sent.text().    
+0000bf30: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
+0000bf40: 6374 5b22 5243 5622 5d20 3d20 7365 6c66  ct["RCV"] = self
+0000bf50: 2e72 6563 6569 7665 2e74 6578 7428 290a  .receive.text().
+0000bf60: 2020 2020 2020 2020 2320 7365 6c66 2e63          # self.c
+0000bf70: 6f6e 7461 6374 5b22 436f 756e 7472 7950  ontact["CountryP
+0000bf80: 7265 6669 7822 5d0a 2020 2020 2020 2020  refix"].        
+0000bf90: 2320 7365 6c66 2e63 6f6e 7461 6374 5b22  # self.contact["
+0000bfa0: 5374 6174 696f 6e50 7265 6669 7822 5d20  StationPrefix"] 
+0000bfb0: 3d20 7365 6c66 2e70 7265 662e 6765 7428  = self.pref.get(
+0000bfc0: 2263 616c 6c73 6967 6e22 2c20 2222 290a  "callsign", "").
+0000bfd0: 2020 2020 2020 2020 2320 7365 6c66 2e63          # self.c
+0000bfe0: 6f6e 7461 6374 5b22 5154 4822 5d0a 2020  ontact["QTH"].  
+0000bff0: 2020 2020 2020 2320 7365 6c66 2e63 6f6e        # self.con
+0000c000: 7461 6374 5b22 4e61 6d65 225d 203d 2073  tact["Name"] = s
+0000c010: 656c 662e 6f74 6865 725f 312e 7465 7874  elf.other_1.text
+0000c020: 2829 0a20 2020 2020 2020 2023 2073 656c  ().        # sel
+0000c030: 662e 636f 6e74 6163 745b 2243 6f6d 6d65  f.contact["Comme
+0000c040: 6e74 225d 203d 2073 656c 662e 6f74 6865  nt"] = self.othe
+0000c050: 725f 322e 7465 7874 2829 0a20 2020 2020  r_2.text().     
+0000c060: 2020 2023 2073 656c 662e 636f 6e74 6163     # self.contac
+0000c070: 745b 224e 5222 5d0a 2020 2020 2020 2020  t["NR"].        
+0000c080: 2320 7365 6c66 2e63 6f6e 7461 6374 5b22  # self.contact["
+0000c090: 5365 6374 225d 0a20 2020 2020 2020 2023  Sect"].        #
+0000c0a0: 2073 656c 662e 636f 6e74 6163 745b 2250   self.contact["P
+0000c0b0: 7265 6322 5d0a 2020 2020 2020 2020 2320  rec"].        # 
+0000c0c0: 7365 6c66 2e63 6f6e 7461 6374 5b22 434b  self.contact["CK
+0000c0d0: 225d 0a20 2020 2020 2020 2023 2073 656c  "].        # sel
+0000c0e0: 662e 636f 6e74 6163 745b 225a 4e22 5d0a  f.contact["ZN"].
+0000c0f0: 2020 2020 2020 2020 2320 7365 6c66 2e63          # self.c
+0000c100: 6f6e 7461 6374 5b22 5365 6e74 4e72 225d  ontact["SentNr"]
+0000c110: 0a20 2020 2020 2020 2023 2073 656c 662e  .        # self.
+0000c120: 636f 6e74 6163 745b 2250 6f69 6e74 7322  contact["Points"
+0000c130: 5d0a 2020 2020 2020 2020 2320 7365 6c66  ].        # self
+0000c140: 2e63 6f6e 7461 6374 5b22 4973 4d75 6c74  .contact["IsMult
+0000c150: 6970 6c69 6572 3122 5d0a 2020 2020 2020  iplier1"].      
+0000c160: 2020 2320 7365 6c66 2e63 6f6e 7461 6374    # self.contact
+0000c170: 5b22 4973 4d75 6c74 6970 6c69 6572 3222  ["IsMultiplier2"
+0000c180: 5d0a 2020 2020 2020 2020 2320 7365 6c66  ].        # self
+0000c190: 2e63 6f6e 7461 6374 5b22 506f 7765 7222  .contact["Power"
+0000c1a0: 5d0a 2020 2020 2020 2020 2320 7365 6c66  ].        # self
+0000c1b0: 2e63 6f6e 7461 6374 5b22 4261 6e64 225d  .contact["Band"]
+0000c1c0: 0a20 2020 2020 2020 2023 2073 656c 662e  .        # self.
+0000c1d0: 636f 6e74 6163 745b 2257 5058 5072 6566  contact["WPXPref
+0000c1e0: 6978 225d 203d 2063 616c 6375 6c61 7465  ix"] = calculate
+0000c1f0: 5f77 7078 5f70 7265 6669 7828 7365 6c66  _wpx_prefix(self
+0000c200: 2e63 616c 6c73 6967 6e2e 7465 7874 2829  .callsign.text()
+0000c210: 290a 2020 2020 2020 2020 2320 7365 6c66  ).        # self
+0000c220: 2e63 6f6e 7461 6374 5b22 4578 6368 616e  .contact["Exchan
+0000c230: 6765 3122 5d0a 2020 2020 2020 2020 2320  ge1"].        # 
+0000c240: 7365 6c66 2e63 6f6e 7461 6374 5b22 5261  self.contact["Ra
+0000c250: 6469 6f4e 5222 5d0a 2020 2020 2020 2020  dioNR"].        
+0000c260: 2320 7365 6c66 2e63 6f6e 7461 6374 5b22  # self.contact["
+0000c270: 6973 4d75 6c74 6970 6c69 6572 3322 5d0a  isMultiplier3"].
+0000c280: 2020 2020 2020 2020 2320 7365 6c66 2e63          # self.c
+0000c290: 6f6e 7461 6374 5b22 4d69 7363 5465 7874  ontact["MiscText
+0000c2a0: 225d 0a20 2020 2020 2020 2023 2073 656c  "].        # sel
+0000c2b0: 662e 636f 6e74 6163 745b 2243 6f6e 7461  f.contact["Conta
+0000c2c0: 6374 5479 7065 225d 0a20 2020 2020 2020  ctType"].       
+0000c2d0: 2023 2073 656c 662e 636f 6e74 6163 745b   # self.contact[
+0000c2e0: 2252 756e 3152 756e 3222 5d0a 2020 2020  "Run1Run2"].    
+0000c2f0: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
+0000c300: 6374 5b22 4772 6964 5371 7561 7265 225d  ct["GridSquare"]
+0000c310: 0a20 2020 2020 2020 2023 2073 656c 662e  .        # self.
+0000c320: 636f 6e74 6163 745b 2243 6f6e 7469 6e65  contact["Contine
+0000c330: 6e74 225d 0a20 2020 2020 2020 2023 2073  nt"].        # s
+0000c340: 656c 662e 636f 6e74 6163 745b 2252 6f76  elf.contact["Rov
+0000c350: 6572 4c6f 6361 7469 6f6e 225d 0a20 2020  erLocation"].   
+0000c360: 2020 2020 2023 2073 656c 662e 636f 6e74       # self.cont
+0000c370: 6163 745b 2252 6164 696f 496e 7465 7266  act["RadioInterf
+0000c380: 6163 6564 225d 0a20 2020 2020 2020 2023  aced"].        #
+0000c390: 2073 656c 662e 636f 6e74 6163 745b 224e   self.contact["N
+0000c3a0: 6574 776f 726b 6564 436f 6d70 4e72 225d  etworkedCompNr"]
+0000c3b0: 0a20 2020 2020 2020 2023 2073 656c 662e  .        # self.
+0000c3c0: 636f 6e74 6163 745b 2243 4c41 494d 4544  contact["CLAIMED
+0000c3d0: 5153 4f22 5d0a 0a20 2020 2064 6566 206e  QSO"]..    def n
+0000c3e0: 6577 5f63 6f6e 7465 7374 5f64 6961 6c6f  ew_contest_dialo
+0000c3f0: 6728 7365 6c66 293a 0a20 2020 2020 2020  g(self):.       
+0000c400: 2022 2222 5368 6f77 206e 6577 2063 6f6e   """Show new con
+0000c410: 7465 7374 2064 6961 6c6f 6722 2222 0a20  test dialog""". 
+0000c420: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+0000c430: 6275 6728 224e 6577 2063 6f6e 7465 7374  bug("New contest
+0000c440: 2044 6961 6c6f 6722 290a 2020 2020 2020   Dialog").      
+0000c450: 2020 7365 6c66 2e63 6f6e 7465 7374 5f64    self.contest_d
+0000c460: 6961 6c6f 6720 3d20 4e65 7743 6f6e 7465  ialog = NewConte
+0000c470: 7374 2857 4f52 4b49 4e47 5f50 4154 4829  st(WORKING_PATH)
+0000c480: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
+0000c490: 6e74 6573 745f 6469 616c 6f67 2e61 6363  ntest_dialog.acc
+0000c4a0: 6570 7465 642e 636f 6e6e 6563 7428 7365  epted.connect(se
+0000c4b0: 6c66 2e73 6176 655f 636f 6e74 6573 7429  lf.save_contest)
+0000c4c0: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
+0000c4d0: 6e74 6573 745f 6469 616c 6f67 2e64 6174  ntest_dialog.dat
+0000c4e0: 6554 696d 6545 6469 742e 7365 7444 6174  eTimeEdit.setDat
+0000c4f0: 6528 5174 436f 7265 2e51 4461 7465 2e63  e(QtCore.QDate.c
+0000c500: 7572 7265 6e74 4461 7465 2829 290a 2020  urrentDate()).  
+0000c510: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
+0000c520: 7374 5f64 6961 6c6f 672e 6461 7465 5469  st_dialog.dateTi
+0000c530: 6d65 4564 6974 2e73 6574 4361 6c65 6e64  meEdit.setCalend
+0000c540: 6172 506f 7075 7028 5472 7565 290a 2020  arPopup(True).  
+0000c550: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
+0000c560: 7374 5f64 6961 6c6f 672e 6461 7465 5469  st_dialog.dateTi
+0000c570: 6d65 4564 6974 2e73 6574 5469 6d65 2851  meEdit.setTime(Q
+0000c580: 7443 6f72 652e 5154 696d 6528 302c 2030  tCore.QTime(0, 0
+0000c590: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+0000c5a0: 636f 6e74 6573 745f 6469 616c 6f67 2e70  contest_dialog.p
+0000c5b0: 6f77 6572 2e73 6574 4375 7272 656e 7454  ower.setCurrentT
+0000c5c0: 6578 7428 224c 4f57 2229 0a20 2020 2020  ext("LOW").     
+0000c5d0: 2020 2073 656c 662e 636f 6e74 6573 745f     self.contest_
+0000c5e0: 6469 616c 6f67 2e73 7461 7469 6f6e 2e73  dialog.station.s
+0000c5f0: 6574 4375 7272 656e 7454 6578 7428 2246  etCurrentText("F
+0000c600: 4958 4544 2229 0a20 2020 2020 2020 2073  IXED").        s
+0000c610: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
+0000c620: 6f67 2e6f 7065 6e28 290a 0a20 2020 2064  og.open()..    d
+0000c630: 6566 2073 6176 655f 636f 6e74 6573 7428  ef save_contest(
+0000c640: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+0000c650: 2222 5361 7665 2043 6f6e 7465 7374 2222  ""Save Contest""
+0000c660: 220a 2020 2020 2020 2020 6e65 7874 5f6e  ".        next_n
+0000c670: 756d 6265 7220 3d20 7365 6c66 2e64 6174  umber = self.dat
+0000c680: 6162 6173 652e 6765 745f 6e65 7874 5f63  abase.get_next_c
+0000c690: 6f6e 7465 7374 5f6e 7228 290a 2020 2020  ontest_nr().    
+0000c6a0: 2020 2020 636f 6e74 6573 7420 3d20 7b7d      contest = {}
+0000c6b0: 0a20 2020 2020 2020 2063 6f6e 7465 7374  .        contest
+0000c6c0: 5b22 436f 6e74 6573 744e 616d 6522 5d20  ["ContestName"] 
+0000c6d0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+0000c6e0: 7365 6c66 2e63 6f6e 7465 7374 5f64 6961  self.contest_dia
+0000c6f0: 6c6f 672e 636f 6e74 6573 742e 6375 7272  log.contest.curr
+0000c700: 656e 7454 6578 7428 292e 6c6f 7765 7228  entText().lower(
+0000c710: 292e 7265 706c 6163 6528 2220 222c 2022  ).replace(" ", "
+0000c720: 5f22 290a 2020 2020 2020 2020 290a 2020  _").        ).  
+0000c730: 2020 2020 2020 636f 6e74 6573 745b 2253        contest["S
+0000c740: 7461 7274 4461 7465 225d 203d 2073 656c  tartDate"] = sel
+0000c750: 662e 636f 6e74 6573 745f 6469 616c 6f67  f.contest_dialog
+0000c760: 2e64 6174 6554 696d 6545 6469 742e 6461  .dateTimeEdit.da
+0000c770: 7465 5469 6d65 2829 2e74 6f53 7472 696e  teTime().toStrin
+0000c780: 6728 0a20 2020 2020 2020 2020 2020 2022  g(.            "
+0000c790: 7979 7979 2d4d 4d2d 6464 2068 683a 6d6d  yyyy-MM-dd hh:mm
+0000c7a0: 3a73 7322 0a20 2020 2020 2020 2029 0a20  :ss".        ). 
+0000c7b0: 2020 2020 2020 2063 6f6e 7465 7374 5b22         contest["
+0000c7c0: 4f70 6572 6174 6f72 4361 7465 676f 7279  OperatorCategory
+0000c7d0: 225d 203d 2073 656c 662e 636f 6e74 6573  "] = self.contes
+0000c7e0: 745f 6469 616c 6f67 2e6f 7065 7261 746f  t_dialog.operato
+0000c7f0: 725f 636c 6173 732e 6375 7272 656e 7454  r_class.currentT
+0000c800: 6578 7428 290a 2020 2020 2020 2020 636f  ext().        co
+0000c810: 6e74 6573 745b 2242 616e 6443 6174 6567  ntest["BandCateg
+0000c820: 6f72 7922 5d20 3d20 7365 6c66 2e63 6f6e  ory"] = self.con
+0000c830: 7465 7374 5f64 6961 6c6f 672e 6261 6e64  test_dialog.band
+0000c840: 2e63 7572 7265 6e74 5465 7874 2829 0a20  .currentText(). 
+0000c850: 2020 2020 2020 2063 6f6e 7465 7374 5b22         contest["
+0000c860: 506f 7765 7243 6174 6567 6f72 7922 5d20  PowerCategory"] 
+0000c870: 3d20 7365 6c66 2e63 6f6e 7465 7374 5f64  = self.contest_d
+0000c880: 6961 6c6f 672e 706f 7765 722e 6375 7272  ialog.power.curr
+0000c890: 656e 7454 6578 7428 290a 2020 2020 2020  entText().      
+0000c8a0: 2020 636f 6e74 6573 745b 224d 6f64 6543    contest["ModeC
+0000c8b0: 6174 6567 6f72 7922 5d20 3d20 7365 6c66  ategory"] = self
+0000c8c0: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
+0000c8d0: 6d6f 6465 2e63 7572 7265 6e74 5465 7874  mode.currentText
+0000c8e0: 2829 0a20 2020 2020 2020 2063 6f6e 7465  ().        conte
+0000c8f0: 7374 5b22 4f76 6572 6c61 7943 6174 6567  st["OverlayCateg
+0000c900: 6f72 7922 5d20 3d20 7365 6c66 2e63 6f6e  ory"] = self.con
+0000c910: 7465 7374 5f64 6961 6c6f 672e 6f76 6572  test_dialog.over
+0000c920: 6c61 792e 6375 7272 656e 7454 6578 7428  lay.currentText(
+0000c930: 290a 2020 2020 2020 2020 2320 636f 6e74  ).        # cont
+0000c940: 6573 745b 2743 6c61 696d 6564 5363 6f72  est['ClaimedScor
+0000c950: 6527 5d20 3d20 7365 6c66 2e63 6f6e 7465  e'] = self.conte
+0000c960: 7374 5f64 6961 6c6f 672e 0a20 2020 2020  st_dialog..     
+0000c970: 2020 2063 6f6e 7465 7374 5b22 4f70 6572     contest["Oper
+0000c980: 6174 6f72 7322 5d20 3d20 7365 6c66 2e63  ators"] = self.c
+0000c990: 6f6e 7465 7374 5f64 6961 6c6f 672e 6f70  ontest_dialog.op
+0000c9a0: 6572 6174 6f72 732e 7465 7874 2829 0a20  erators.text(). 
+0000c9b0: 2020 2020 2020 2063 6f6e 7465 7374 5b22         contest["
+0000c9c0: 536f 6170 626f 7822 5d20 3d20 7365 6c66  Soapbox"] = self
+0000c9d0: 2e63 6f6e 7465 7374 5f64 6961 6c6f 672e  .contest_dialog.
+0000c9e0: 736f 6170 626f 782e 746f 506c 6169 6e54  soapbox.toPlainT
+0000c9f0: 6578 7428 290a 2020 2020 2020 2020 636f  ext().        co
+0000ca00: 6e74 6573 745b 2253 656e 7445 7863 6861  ntest["SentExcha
+0000ca10: 6e67 6522 5d20 3d20 7365 6c66 2e63 6f6e  nge"] = self.con
+0000ca20: 7465 7374 5f64 6961 6c6f 672e 6578 6368  test_dialog.exch
+0000ca30: 616e 6765 2e74 6578 7428 290a 2020 2020  ange.text().    
+0000ca40: 2020 2020 636f 6e74 6573 745b 2243 6f6e      contest["Con
+0000ca50: 7465 7374 4e52 225d 203d 206e 6578 745f  testNR"] = next_
+0000ca60: 6e75 6d62 6572 2e67 6574 2822 636f 756e  number.get("coun
+0000ca70: 7422 2c20 3129 0a20 2020 2020 2020 2073  t", 1).        s
+0000ca80: 656c 662e 7072 6566 5b22 636f 6e74 6573  elf.pref["contes
+0000ca90: 7422 5d20 3d20 6e65 7874 5f6e 756d 6265  t"] = next_numbe
+0000caa0: 722e 6765 7428 2263 6f75 6e74 222c 2031  r.get("count", 1
+0000cab0: 290a 2020 2020 2020 2020 2320 636f 6e74  ).        # cont
+0000cac0: 6573 745b 2753 7562 5479 7065 275d 203d  est['SubType'] =
+0000cad0: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+0000cae0: 616c 6f67 2e0a 2020 2020 2020 2020 636f  alog..        co
+0000caf0: 6e74 6573 745b 2253 7461 7469 6f6e 4361  ntest["StationCa
+0000cb00: 7465 676f 7279 225d 203d 2073 656c 662e  tegory"] = self.
+0000cb10: 636f 6e74 6573 745f 6469 616c 6f67 2e73  contest_dialog.s
+0000cb20: 7461 7469 6f6e 2e63 7572 7265 6e74 5465  tation.currentTe
+0000cb30: 7874 2829 0a20 2020 2020 2020 2063 6f6e  xt().        con
+0000cb40: 7465 7374 5b22 4173 7369 7374 6564 4361  test["AssistedCa
+0000cb50: 7465 676f 7279 225d 203d 2073 656c 662e  tegory"] = self.
+0000cb60: 636f 6e74 6573 745f 6469 616c 6f67 2e61  contest_dialog.a
+0000cb70: 7373 6973 7465 642e 6375 7272 656e 7454  ssisted.currentT
+0000cb80: 6578 7428 290a 2020 2020 2020 2020 636f  ext().        co
+0000cb90: 6e74 6573 745b 2254 7261 6e73 6d69 7474  ntest["Transmitt
+0000cba0: 6572 4361 7465 676f 7279 225d 203d 2073  erCategory"] = s
+0000cbb0: 656c 662e 636f 6e74 6573 745f 6469 616c  elf.contest_dial
+0000cbc0: 6f67 2e74 7261 6e73 6d69 7474 6572 2e63  og.transmitter.c
+0000cbd0: 7572 7265 6e74 5465 7874 2829 0a20 2020  urrentText().   
+0000cbe0: 2020 2020 2023 2063 6f6e 7465 7374 5b27       # contest['
+0000cbf0: 5469 6d65 4361 7465 676f 7279 275d 203d  TimeCategory'] =
+0000cc00: 2073 656c 662e 636f 6e74 6573 745f 6469   self.contest_di
+0000cc10: 616c 6f67 2e0a 2020 2020 2020 2020 6c6f  alog..        lo
+0000cc20: 6767 6572 2e64 6562 7567 2822 2573 222c  gger.debug("%s",
+0000cc30: 2066 227b 636f 6e74 6573 747d 2229 0a20   f"{contest}"). 
+0000cc40: 2020 2020 2020 2073 656c 662e 6461 7461         self.data
+0000cc50: 6261 7365 2e61 6464 5f63 6f6e 7465 7374  base.add_contest
+0000cc60: 2863 6f6e 7465 7374 290a 2020 2020 2020  (contest).      
+0000cc70: 2020 7365 6c66 2e77 7269 7465 5f70 7265    self.write_pre
+0000cc80: 6665 7265 6e63 6528 290a 2020 2020 2020  ference().      
+0000cc90: 2020 7365 6c66 2e6c 6f61 645f 636f 6e74    self.load_cont
+0000cca0: 6573 7428 290a 0a20 2020 2064 6566 2065  est()..    def e
+0000ccb0: 6469 745f 7374 6174 696f 6e5f 7365 7474  dit_station_sett
+0000ccc0: 696e 6773 2873 656c 6629 3a0a 2020 2020  ings(self):.    
+0000ccd0: 2020 2020 2222 2253 686f 7720 7365 7474      """Show sett
+0000cce0: 696e 6773 2064 6961 6c6f 6722 2222 0a20  ings dialog""". 
+0000ccf0: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+0000cd00: 6275 6728 2253 7461 7469 6f6e 2053 6574  bug("Station Set
+0000cd10: 7469 6e67 7320 7365 6c65 6374 6564 2229  tings selected")
+0000cd20: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+0000cd30: 7474 696e 6773 5f64 6961 6c6f 6720 3d20  ttings_dialog = 
+0000cd40: 4564 6974 5374 6174 696f 6e28 574f 524b  EditStation(WORK
+0000cd50: 494e 475f 5041 5448 290a 2020 2020 2020  ING_PATH).      
+0000cd60: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
+0000cd70: 6469 616c 6f67 2e61 6363 6570 7465 642e  dialog.accepted.
+0000cd80: 636f 6e6e 6563 7428 7365 6c66 2e73 6176  connect(self.sav
+0000cd90: 655f 7365 7474 696e 6773 290a 2020 2020  e_settings).    
+0000cda0: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
+0000cdb0: 735f 6469 616c 6f67 2e43 616c 6c2e 7365  s_dialog.Call.se
+0000cdc0: 7454 6578 7428 7365 6c66 2e73 7461 7469  tText(self.stati
+0000cdd0: 6f6e 2e67 6574 2822 4361 6c6c 222c 2022  on.get("Call", "
+0000cde0: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+0000cdf0: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+0000ce00: 2e4e 616d 652e 7365 7454 6578 7428 7365  .Name.setText(se
+0000ce10: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
+0000ce20: 4e61 6d65 222c 2022 2229 290a 2020 2020  Name", "")).    
+0000ce30: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
+0000ce40: 735f 6469 616c 6f67 2e41 6464 7265 7373  s_dialog.Address
+0000ce50: 312e 7365 7454 6578 7428 7365 6c66 2e73  1.setText(self.s
+0000ce60: 7461 7469 6f6e 2e67 6574 2822 5374 7265  tation.get("Stre
+0000ce70: 6574 3122 2c20 2222 2929 0a20 2020 2020  et1", "")).     
+0000ce80: 2020 2073 656c 662e 7365 7474 696e 6773     self.settings
+0000ce90: 5f64 6961 6c6f 672e 4164 6472 6573 7332  _dialog.Address2
+0000cea0: 2e73 6574 5465 7874 2873 656c 662e 7374  .setText(self.st
+0000ceb0: 6174 696f 6e2e 6765 7428 2253 7472 6565  ation.get("Stree
+0000cec0: 7432 222c 2022 2229 290a 2020 2020 2020  t2", "")).      
+0000ced0: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
+0000cee0: 6469 616c 6f67 2e43 6974 792e 7365 7454  dialog.City.setT
+0000cef0: 6578 7428 7365 6c66 2e73 7461 7469 6f6e  ext(self.station
+0000cf00: 2e67 6574 2822 4369 7479 222c 2022 2229  .get("City", "")
+0000cf10: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000cf20: 6574 7469 6e67 735f 6469 616c 6f67 2e53  ettings_dialog.S
+0000cf30: 7461 7465 2e73 6574 5465 7874 2873 656c  tate.setText(sel
+0000cf40: 662e 7374 6174 696f 6e2e 6765 7428 2253  f.station.get("S
+0000cf50: 7461 7465 222c 2022 2229 290a 2020 2020  tate", "")).    
+0000cf60: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
+0000cf70: 735f 6469 616c 6f67 2e5a 6970 2e73 6574  s_dialog.Zip.set
+0000cf80: 5465 7874 2873 656c 662e 7374 6174 696f  Text(self.statio
+0000cf90: 6e2e 6765 7428 225a 6970 222c 2022 2229  n.get("Zip", "")
+0000cfa0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000cfb0: 6574 7469 6e67 735f 6469 616c 6f67 2e43  ettings_dialog.C
+0000cfc0: 6f75 6e74 7279 2e73 6574 5465 7874 2873  ountry.setText(s
+0000cfd0: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
+0000cfe0: 2243 6f75 6e74 7279 222c 2022 2229 290a  "Country", "")).
+0000cff0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+0000d000: 7469 6e67 735f 6469 616c 6f67 2e47 7269  tings_dialog.Gri
+0000d010: 6453 7175 6172 652e 7365 7454 6578 7428  dSquare.setText(
+0000d020: 7365 6c66 2e73 7461 7469 6f6e 2e67 6574  self.station.get
+0000d030: 2822 4772 6964 5371 7561 7265 222c 2022  ("GridSquare", "
+0000d040: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+0000d050: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+0000d060: 2e43 515a 6f6e 652e 7365 7454 6578 7428  .CQZone.setText(
+0000d070: 7374 7228 7365 6c66 2e73 7461 7469 6f6e  str(self.station
+0000d080: 2e67 6574 2822 4351 5a6f 6e65 222c 2022  .get("CQZone", "
+0000d090: 2229 2929 0a20 2020 2020 2020 2073 656c  "))).        sel
+0000d0a0: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
+0000d0b0: 672e 4954 555a 6f6e 652e 7365 7454 6578  g.ITUZone.setTex
+0000d0c0: 7428 7374 7228 7365 6c66 2e73 7461 7469  t(str(self.stati
+0000d0d0: 6f6e 2e67 6574 2822 4941 5255 5a6f 6e65  on.get("IARUZone
+0000d0e0: 222c 2022 2229 2929 0a20 2020 2020 2020  ", ""))).       
+0000d0f0: 2073 656c 662e 7365 7474 696e 6773 5f64   self.settings_d
+0000d100: 6961 6c6f 672e 4c69 6365 6e73 652e 7365  ialog.License.se
+0000d110: 7454 6578 7428 7365 6c66 2e73 7461 7469  tText(self.stati
+0000d120: 6f6e 2e67 6574 2822 4c69 6365 6e73 6543  on.get("LicenseC
+0000d130: 6c61 7373 222c 2022 2229 290a 2020 2020  lass", "")).    
+0000d140: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
+0000d150: 735f 6469 616c 6f67 2e4c 6174 6974 7564  s_dialog.Latitud
+0000d160: 652e 7365 7454 6578 7428 7374 7228 7365  e.setText(str(se
+0000d170: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
+0000d180: 4c61 7469 7475 6465 222c 2022 2229 2929  Latitude", "")))
+0000d190: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+0000d1a0: 7474 696e 6773 5f64 6961 6c6f 672e 4c6f  ttings_dialog.Lo
+0000d1b0: 6e67 6974 7564 652e 7365 7454 6578 7428  ngitude.setText(
+0000d1c0: 7374 7228 7365 6c66 2e73 7461 7469 6f6e  str(self.station
+0000d1d0: 2e67 6574 2822 4c6f 6e67 6974 7564 6522  .get("Longitude"
+0000d1e0: 2c20 2222 2929 290a 2020 2020 2020 2020  , ""))).        
+0000d1f0: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
+0000d200: 616c 6f67 2e53 7461 7469 6f6e 5458 5258  alog.StationTXRX
+0000d210: 2e73 6574 5465 7874 2873 656c 662e 7374  .setText(self.st
+0000d220: 6174 696f 6e2e 6765 7428 2273 7461 7469  ation.get("stati
+0000d230: 6f6e 7478 7278 222c 2022 2229 290a 2020  ontxrx", "")).  
+0000d240: 2020 2020 2020 7365 6c66 2e73 6574 7469        self.setti
+0000d250: 6e67 735f 6469 616c 6f67 2e50 6f77 6572  ngs_dialog.Power
+0000d260: 2e73 6574 5465 7874 2873 656c 662e 7374  .setText(self.st
+0000d270: 6174 696f 6e2e 6765 7428 2253 506f 7765  ation.get("SPowe
+0000d280: 222c 2022 2229 290a 2020 2020 2020 2020  ", "")).        
+0000d290: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
+0000d2a0: 616c 6f67 2e41 6e74 656e 6e61 2e73 6574  alog.Antenna.set
+0000d2b0: 5465 7874 2873 656c 662e 7374 6174 696f  Text(self.statio
+0000d2c0: 6e2e 6765 7428 2253 416e 7465 222c 2022  n.get("SAnte", "
+0000d2d0: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+0000d2e0: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+0000d2f0: 2e41 6e74 4865 6967 6874 2e73 6574 5465  .AntHeight.setTe
+0000d300: 7874 2873 656c 662e 7374 6174 696f 6e2e  xt(self.station.
+0000d310: 6765 7428 2253 416e 7448 3122 2c20 2222  get("SAntH1", ""
+0000d320: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+0000d330: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
+0000d340: 4153 4c2e 7365 7454 6578 7428 7365 6c66  ASL.setText(self
+0000d350: 2e73 7461 7469 6f6e 2e67 6574 2822 5341  .station.get("SA
+0000d360: 6e74 4832 222c 2022 2229 290a 2020 2020  ntH2", "")).    
+0000d370: 2020 2020 7365 6c66 2e73 6574 7469 6e67      self.setting
+0000d380: 735f 6469 616c 6f67 2e41 5252 4c53 6563  s_dialog.ARRLSec
+0000d390: 7469 6f6e 2e73 6574 5465 7874 2873 656c  tion.setText(sel
+0000d3a0: 662e 7374 6174 696f 6e2e 6765 7428 2241  f.station.get("A
+0000d3b0: 5252 4c53 6563 7469 6f6e 222c 2022 2229  RRLSection", "")
+0000d3c0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000d3d0: 6574 7469 6e67 735f 6469 616c 6f67 2e52  ettings_dialog.R
+0000d3e0: 6f76 6572 5154 482e 7365 7454 6578 7428  overQTH.setText(
+0000d3f0: 7365 6c66 2e73 7461 7469 6f6e 2e67 6574  self.station.get
+0000d400: 2822 526f 7665 7251 5448 222c 2022 2229  ("RoverQTH", "")
+0000d410: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000d420: 6574 7469 6e67 735f 6469 616c 6f67 2e43  ettings_dialog.C
+0000d430: 6c75 622e 7365 7454 6578 7428 7365 6c66  lub.setText(self
+0000d440: 2e73 7461 7469 6f6e 2e67 6574 2822 436c  .station.get("Cl
+0000d450: 7562 222c 2022 2229 290a 2020 2020 2020  ub", "")).      
+0000d460: 2020 7365 6c66 2e73 6574 7469 6e67 735f    self.settings_
+0000d470: 6469 616c 6f67 2e45 6d61 696c 2e73 6574  dialog.Email.set
+0000d480: 5465 7874 2873 656c 662e 7374 6174 696f  Text(self.statio
+0000d490: 6e2e 6765 7428 2245 6d61 696c 222c 2022  n.get("Email", "
+0000d4a0: 2229 290a 2020 2020 2020 2020 7365 6c66  ")).        self
+0000d4b0: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+0000d4c0: 2e6f 7065 6e28 290a 0a20 2020 2064 6566  .open()..    def
+0000d4d0: 2073 6176 655f 7365 7474 696e 6773 2873   save_settings(s
+0000d4e0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+0000d4f0: 2253 6176 6520 7365 7474 696e 6773 2222  "Save settings""
+0000d500: 220a 2020 2020 2020 2020 6373 203d 2073  ".        cs = s
+0000d510: 656c 662e 7365 7474 696e 6773 5f64 6961  elf.settings_dia
+0000d520: 6c6f 672e 4361 6c6c 2e74 6578 7428 290a  log.Call.text().
+0000d530: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+0000d540: 7469 6f6e 203d 207b 7d0a 2020 2020 2020  tion = {}.      
+0000d550: 2020 7365 6c66 2e73 7461 7469 6f6e 5b22    self.station["
+0000d560: 4361 6c6c 225d 203d 2063 732e 7570 7065  Call"] = cs.uppe
+0000d570: 7228 290a 2020 2020 2020 2020 7365 6c66  r().        self
+0000d580: 2e73 7461 7469 6f6e 5b22 4e61 6d65 225d  .station["Name"]
+0000d590: 203d 2073 656c 662e 7365 7474 696e 6773   = self.settings
+0000d5a0: 5f64 6961 6c6f 672e 4e61 6d65 2e74 6578  _dialog.Name.tex
+0000d5b0: 7428 292e 7469 746c 6528 290a 2020 2020  t().title().    
+0000d5c0: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
+0000d5d0: 5b22 5374 7265 6574 3122 5d20 3d20 7365  ["Street1"] = se
+0000d5e0: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
+0000d5f0: 6f67 2e41 6464 7265 7373 312e 7465 7874  og.Address1.text
+0000d600: 2829 2e74 6974 6c65 2829 0a20 2020 2020  ().title().     
+0000d610: 2020 2073 656c 662e 7374 6174 696f 6e5b     self.station[
+0000d620: 2253 7472 6565 7432 225d 203d 2073 656c  "Street2"] = sel
+0000d630: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
+0000d640: 672e 4164 6472 6573 7332 2e74 6578 7428  g.Address2.text(
+0000d650: 292e 7469 746c 6528 290a 2020 2020 2020  ).title().      
+0000d660: 2020 7365 6c66 2e73 7461 7469 6f6e 5b22    self.station["
+0000d670: 4369 7479 225d 203d 2073 656c 662e 7365  City"] = self.se
+0000d680: 7474 696e 6773 5f64 6961 6c6f 672e 4369  ttings_dialog.Ci
+0000d690: 7479 2e74 6578 7428 292e 7469 746c 6528  ty.text().title(
+0000d6a0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000d6b0: 7461 7469 6f6e 5b22 5374 6174 6522 5d20  tation["State"] 
+0000d6c0: 3d20 7365 6c66 2e73 6574 7469 6e67 735f  = self.settings_
+0000d6d0: 6469 616c 6f67 2e53 7461 7465 2e74 6578  dialog.State.tex
+0000d6e0: 7428 292e 7570 7065 7228 290a 2020 2020  t().upper().    
+0000d6f0: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
+0000d700: 5b22 5a69 7022 5d20 3d20 7365 6c66 2e73  ["Zip"] = self.s
+0000d710: 6574 7469 6e67 735f 6469 616c 6f67 2e5a  ettings_dialog.Z
+0000d720: 6970 2e74 6578 7428 290a 2020 2020 2020  ip.text().      
+0000d730: 2020 7365 6c66 2e73 7461 7469 6f6e 5b22    self.station["
+0000d740: 436f 756e 7472 7922 5d20 3d20 7365 6c66  Country"] = self
+0000d750: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+0000d760: 2e43 6f75 6e74 7279 2e74 6578 7428 292e  .Country.text().
+0000d770: 7469 746c 6528 290a 2020 2020 2020 2020  title().        
+0000d780: 7365 6c66 2e73 7461 7469 6f6e 5b22 4772  self.station["Gr
+0000d790: 6964 5371 7561 7265 225d 203d 2073 656c  idSquare"] = sel
+0000d7a0: 662e 7365 7474 696e 6773 5f64 6961 6c6f  f.settings_dialo
+0000d7b0: 672e 4772 6964 5371 7561 7265 2e74 6578  g.GridSquare.tex
+0000d7c0: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
+0000d7d0: 2e73 7461 7469 6f6e 5b22 4351 5a6f 6e65  .station["CQZone
+0000d7e0: 225d 203d 2073 656c 662e 7365 7474 696e  "] = self.settin
+0000d7f0: 6773 5f64 6961 6c6f 672e 4351 5a6f 6e65  gs_dialog.CQZone
+0000d800: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
+0000d810: 7365 6c66 2e73 7461 7469 6f6e 5b22 4941  self.station["IA
+0000d820: 5255 5a6f 6e65 225d 203d 2073 656c 662e  RUZone"] = self.
+0000d830: 7365 7474 696e 6773 5f64 6961 6c6f 672e  settings_dialog.
+0000d840: 4954 555a 6f6e 652e 7465 7874 2829 0a20  ITUZone.text(). 
+0000d850: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+0000d860: 696f 6e5b 224c 6963 656e 7365 436c 6173  ion["LicenseClas
+0000d870: 7322 5d20 3d20 7365 6c66 2e73 6574 7469  s"] = self.setti
+0000d880: 6e67 735f 6469 616c 6f67 2e4c 6963 656e  ngs_dialog.Licen
+0000d890: 7365 2e74 6578 7428 292e 7469 746c 6528  se.text().title(
+0000d8a0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000d8b0: 7461 7469 6f6e 5b22 4c61 7469 7475 6465  tation["Latitude
+0000d8c0: 225d 203d 2073 656c 662e 7365 7474 696e  "] = self.settin
+0000d8d0: 6773 5f64 6961 6c6f 672e 4c61 7469 7475  gs_dialog.Latitu
+0000d8e0: 6465 2e74 6578 7428 290a 2020 2020 2020  de.text().      
+0000d8f0: 2020 7365 6c66 2e73 7461 7469 6f6e 5b22    self.station["
+0000d900: 4c6f 6e67 6974 7564 6522 5d20 3d20 7365  Longitude"] = se
+0000d910: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
+0000d920: 6f67 2e4c 6f6e 6769 7475 6465 2e74 6578  og.Longitude.tex
+0000d930: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
+0000d940: 2e73 7461 7469 6f6e 5b22 5354 5865 7122  .station["STXeq"
+0000d950: 5d20 3d20 7365 6c66 2e73 6574 7469 6e67  ] = self.setting
+0000d960: 735f 6469 616c 6f67 2e53 7461 7469 6f6e  s_dialog.Station
+0000d970: 5458 5258 2e74 6578 7428 290a 2020 2020  TXRX.text().    
+0000d980: 2020 2020 7365 6c66 2e73 7461 7469 6f6e      self.station
+0000d990: 5b22 5350 6f77 6522 5d20 3d20 7365 6c66  ["SPowe"] = self
+0000d9a0: 2e73 6574 7469 6e67 735f 6469 616c 6f67  .settings_dialog
+0000d9b0: 2e50 6f77 6572 2e74 6578 7428 290a 2020  .Power.text().  
+0000d9c0: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
+0000d9d0: 6f6e 5b22 5341 6e74 6522 5d20 3d20 7365  on["SAnte"] = se
+0000d9e0: 6c66 2e73 6574 7469 6e67 735f 6469 616c  lf.settings_dial
+0000d9f0: 6f67 2e41 6e74 656e 6e61 2e74 6578 7428  og.Antenna.text(
+0000da00: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000da10: 7461 7469 6f6e 5b22 5341 6e74 4831 225d  tation["SAntH1"]
+0000da20: 203d 2073 656c 662e 7365 7474 696e 6773   = self.settings
+0000da30: 5f64 6961 6c6f 672e 416e 7448 6569 6768  _dialog.AntHeigh
+0000da40: 742e 7465 7874 2829 0a20 2020 2020 2020  t.text().       
+0000da50: 2073 656c 662e 7374 6174 696f 6e5b 2253   self.station["S
+0000da60: 416e 7448 3222 5d20 3d20 7365 6c66 2e73  AntH2"] = self.s
+0000da70: 6574 7469 6e67 735f 6469 616c 6f67 2e41  ettings_dialog.A
+0000da80: 534c 2e74 6578 7428 290a 2020 2020 2020  SL.text().      
+0000da90: 2020 7365 6c66 2e73 7461 7469 6f6e 5b22    self.station["
+0000daa0: 4152 524c 5365 6374 696f 6e22 5d20 3d20  ARRLSection"] = 
+0000dab0: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
+0000dac0: 616c 6f67 2e41 5252 4c53 6563 7469 6f6e  alog.ARRLSection
+0000dad0: 2e74 6578 7428 292e 7570 7065 7228 290a  .text().upper().
+0000dae0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+0000daf0: 7469 6f6e 5b22 526f 7665 7251 5448 225d  tion["RoverQTH"]
+0000db00: 203d 2073 656c 662e 7365 7474 696e 6773   = self.settings
+0000db10: 5f64 6961 6c6f 672e 526f 7665 7251 5448  _dialog.RoverQTH
+0000db20: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
+0000db30: 7365 6c66 2e73 7461 7469 6f6e 5b22 436c  self.station["Cl
+0000db40: 7562 225d 203d 2073 656c 662e 7365 7474  ub"] = self.sett
+0000db50: 696e 6773 5f64 6961 6c6f 672e 436c 7562  ings_dialog.Club
+0000db60: 2e74 6578 7428 292e 7469 746c 6528 290a  .text().title().
+0000db70: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+0000db80: 7469 6f6e 5b22 456d 6169 6c22 5d20 3d20  tion["Email"] = 
+0000db90: 7365 6c66 2e73 6574 7469 6e67 735f 6469  self.settings_di
+0000dba0: 616c 6f67 2e45 6d61 696c 2e74 6578 7428  alog.Email.text(
+0000dbb0: 290a 2020 2020 2020 2020 7365 6c66 2e64  ).        self.d
+0000dbc0: 6174 6162 6173 652e 6164 645f 7374 6174  atabase.add_stat
+0000dbd0: 696f 6e28 7365 6c66 2e73 7461 7469 6f6e  ion(self.station
+0000dbe0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+0000dbf0: 6574 7469 6e67 735f 6469 616c 6f67 2e63  ettings_dialog.c
+0000dc00: 6c6f 7365 2829 0a20 2020 2020 2020 2069  lose().        i
+0000dc10: 6620 7365 6c66 2e63 7572 7265 6e74 5f6f  f self.current_o
+0000dc20: 7020 3d3d 2022 223a 0a20 2020 2020 2020  p == "":.       
+0000dc30: 2020 2020 2073 656c 662e 6375 7272 656e       self.curren
+0000dc40: 745f 6f70 203d 2073 656c 662e 7374 6174  t_op = self.stat
+0000dc50: 696f 6e2e 6765 7428 2243 616c 6c22 2c20  ion.get("Call", 
+0000dc60: 2222 290a 2020 2020 2020 2020 2020 2020  "").            
+0000dc70: 7365 6c66 2e6d 616b 655f 6f70 5f64 6972  self.make_op_dir
+0000dc80: 2829 0a20 2020 2020 2020 2063 6f6e 7465  ().        conte
+0000dc90: 7374 5f63 6f75 6e74 203d 2073 656c 662e  st_count = self.
+0000dca0: 6461 7461 6261 7365 2e66 6574 6368 5f61  database.fetch_a
+0000dcb0: 6c6c 5f63 6f6e 7465 7374 7328 290a 2020  ll_contests().  
+0000dcc0: 2020 2020 2020 6966 206c 656e 2863 6f6e        if len(con
+0000dcd0: 7465 7374 5f63 6f75 6e74 2920 3d3d 2030  test_count) == 0
+0000dce0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000dcf0: 6c66 2e6e 6577 5f63 6f6e 7465 7374 5f64  lf.new_contest_d
+0000dd00: 6961 6c6f 6728 290a 0a20 2020 2064 6566  ialog()..    def
+0000dd10: 2065 6469 745f 6d61 6372 6f28 7365 6c66   edit_macro(self
+0000dd20: 2c20 6675 6e63 7469 6f6e 5f6b 6579 293a  , function_key):
+0000dd30: 0a20 2020 2020 2020 2022 2222 5368 6f77  .        """Show
+0000dd40: 2065 6469 7420 6d61 6372 6f20 6469 616c   edit macro dial
+0000dd50: 6f67 2222 220a 2020 2020 2020 2020 7365  og""".        se
+0000dd60: 6c66 2e65 6469 745f 6d61 6372 6f5f 6469  lf.edit_macro_di
+0000dd70: 616c 6f67 203d 2045 6469 744d 6163 726f  alog = EditMacro
+0000dd80: 2866 756e 6374 696f 6e5f 6b65 792c 2057  (function_key, W
+0000dd90: 4f52 4b49 4e47 5f50 4154 4829 0a20 2020  ORKING_PATH).   
+0000dda0: 2020 2020 2073 656c 662e 6564 6974 5f6d       self.edit_m
+0000ddb0: 6163 726f 5f64 6961 6c6f 672e 6163 6365  acro_dialog.acce
+0000ddc0: 7074 6564 2e63 6f6e 6e65 6374 2873 656c  pted.connect(sel
+0000ddd0: 662e 6564 6974 6564 5f6d 6163 726f 290a  f.edited_macro).
+0000dde0: 2020 2020 2020 2020 7365 6c66 2e65 6469          self.edi
+0000ddf0: 745f 6d61 6372 6f5f 6469 616c 6f67 2e6f  t_macro_dialog.o
+0000de00: 7065 6e28 290a 0a20 2020 2064 6566 2065  pen()..    def e
+0000de10: 6469 7465 645f 6d61 6372 6f28 7365 6c66  dited_macro(self
+0000de20: 293a 0a20 2020 2020 2020 2022 2222 5361  ):.        """Sa
+0000de30: 7665 2065 6469 7465 6420 6d61 6372 6f22  ve edited macro"
+0000de40: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
+0000de50: 6564 6974 5f6d 6163 726f 5f64 6961 6c6f  edit_macro_dialo
+0000de60: 672e 6675 6e63 7469 6f6e 5f6b 6579 2e73  g.function_key.s
+0000de70: 6574 5465 7874 280a 2020 2020 2020 2020  etText(.        
+0000de80: 2020 2020 7365 6c66 2e65 6469 745f 6d61      self.edit_ma
+0000de90: 6372 6f5f 6469 616c 6f67 2e6d 6163 726f  cro_dialog.macro
+0000dea0: 5f6c 6162 656c 2e74 6578 7428 290a 2020  _label.text().  
+0000deb0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000dec0: 7365 6c66 2e65 6469 745f 6d61 6372 6f5f  self.edit_macro_
+0000ded0: 6469 616c 6f67 2e66 756e 6374 696f 6e5f  dialog.function_
+0000dee0: 6b65 792e 7365 7454 6f6f 6c54 6970 280a  key.setToolTip(.
+0000def0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000df00: 2e65 6469 745f 6d61 6372 6f5f 6469 616c  .edit_macro_dial
+0000df10: 6f67 2e74 6865 5f6d 6163 726f 2e74 6578  og.the_macro.tex
+0000df20: 7428 290a 2020 2020 2020 2020 290a 2020  t().        ).  
+0000df30: 2020 2020 2020 7365 6c66 2e65 6469 745f        self.edit_
+0000df40: 6d61 6372 6f5f 6469 616c 6f67 2e63 6c6f  macro_dialog.clo
+0000df50: 7365 2829 0a0a 2020 2020 6465 6620 6564  se()..    def ed
+0000df60: 6974 5f46 3128 7365 6c66 293a 0a20 2020  it_F1(self):.   
+0000df70: 2020 2020 2022 2222 7374 7562 2222 220a       """stub""".
+0000df80: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+0000df90: 6562 7567 2822 4631 2052 6967 6874 2043  ebug("F1 Right C
+0000dfa0: 6c69 636b 6564 2e22 290a 2020 2020 2020  licked.").      
+0000dfb0: 2020 7365 6c66 2e65 6469 745f 6d61 6372    self.edit_macr
+0000dfc0: 6f28 7365 6c66 2e46 3129 0a0a 2020 2020  o(self.F1)..    
+0000dfd0: 6465 6620 6564 6974 5f46 3228 7365 6c66  def edit_F2(self
+0000dfe0: 293a 0a20 2020 2020 2020 2022 2222 7374  ):.        """st
+0000dff0: 7562 2222 220a 2020 2020 2020 2020 6c6f  ub""".        lo
+0000e000: 6767 6572 2e64 6562 7567 2822 4632 2052  gger.debug("F2 R
+0000e010: 6967 6874 2043 6c69 636b 6564 2e22 290a  ight Clicked.").
+0000e020: 2020 2020 2020 2020 7365 6c66 2e65 6469          self.edi
+0000e030: 745f 6d61 6372 6f28 7365 6c66 2e46 3229  t_macro(self.F2)
+0000e040: 0a0a 2020 2020 6465 6620 6564 6974 5f46  ..    def edit_F
+0000e050: 3328 7365 6c66 293a 0a20 2020 2020 2020  3(self):.       
+0000e060: 2022 2222 7374 7562 2222 220a 2020 2020   """stub""".    
+0000e070: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+0000e080: 2822 4633 2052 6967 6874 2043 6c69 636b  ("F3 Right Click
+0000e090: 6564 2e22 290a 2020 2020 2020 2020 7365  ed.").        se
+0000e0a0: 6c66 2e65 6469 745f 6d61 6372 6f28 7365  lf.edit_macro(se
+0000e0b0: 6c66 2e46 3329 0a0a 2020 2020 6465 6620  lf.F3)..    def 
+0000e0c0: 6564 6974 5f46 3428 7365 6c66 293a 0a20  edit_F4(self):. 
+0000e0d0: 2020 2020 2020 2022 2222 7374 7562 2222         """stub""
+0000e0e0: 220a 2020 2020 2020 2020 6c6f 6767 6572  ".        logger
+0000e0f0: 2e64 6562 7567 2822 4634 2052 6967 6874  .debug("F4 Right
+0000e100: 2043 6c69 636b 6564 2e22 290a 2020 2020   Clicked.").    
+0000e110: 2020 2020 7365 6c66 2e65 6469 745f 6d61      self.edit_ma
+0000e120: 6372 6f28 7365 6c66 2e46 3429 0a0a 2020  cro(self.F4)..  
+0000e130: 2020 6465 6620 6564 6974 5f46 3528 7365    def edit_F5(se
+0000e140: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+0000e150: 7374 7562 2222 220a 2020 2020 2020 2020  stub""".        
+0000e160: 6c6f 6767 6572 2e64 6562 7567 2822 4635  logger.debug("F5
+0000e170: 2052 6967 6874 2043 6c69 636b 6564 2e22   Right Clicked."
+0000e180: 290a 2020 2020 2020 2020 7365 6c66 2e65  ).        self.e
+0000e190: 6469 745f 6d61 6372 6f28 7365 6c66 2e46  dit_macro(self.F
+0000e1a0: 3529 0a0a 2020 2020 6465 6620 6564 6974  5)..    def edit
+0000e1b0: 5f46 3628 7365 6c66 293a 0a20 2020 2020  _F6(self):.     
+0000e1c0: 2020 2022 2222 7374 7562 2222 220a 2020     """stub""".  
+0000e1d0: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+0000e1e0: 7567 2822 4636 2052 6967 6874 2043 6c69  ug("F6 Right Cli
+0000e1f0: 636b 6564 2e22 290a 2020 2020 2020 2020  cked.").        
+0000e200: 7365 6c66 2e65 6469 745f 6d61 6372 6f28  self.edit_macro(
+0000e210: 7365 6c66 2e46 3629 0a0a 2020 2020 6465  self.F6)..    de
+0000e220: 6620 6564 6974 5f46 3728 7365 6c66 293a  f edit_F7(self):
+0000e230: 0a20 2020 2020 2020 2022 2222 7374 7562  .        """stub
+0000e240: 2222 220a 2020 2020 2020 2020 6c6f 6767  """.        logg
+0000e250: 6572 2e64 6562 7567 2822 4637 2052 6967  er.debug("F7 Rig
+0000e260: 6874 2043 6c69 636b 6564 2e22 290a 2020  ht Clicked.").  
+0000e270: 2020 2020 2020 7365 6c66 2e65 6469 745f        self.edit_
+0000e280: 6d61 6372 6f28 7365 6c66 2e46 3729 0a0a  macro(self.F7)..
+0000e290: 2020 2020 6465 6620 6564 6974 5f46 3828      def edit_F8(
+0000e2a0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+0000e2b0: 2222 7374 7562 2222 220a 2020 2020 2020  ""stub""".      
+0000e2c0: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+0000e2d0: 4638 2052 6967 6874 2043 6c69 636b 6564  F8 Right Clicked
+0000e2e0: 2e22 290a 2020 2020 2020 2020 7365 6c66  .").        self
+0000e2f0: 2e65 6469 745f 6d61 6372 6f28 7365 6c66  .edit_macro(self
+0000e300: 2e46 3829 0a0a 2020 2020 6465 6620 6564  .F8)..    def ed
+0000e310: 6974 5f46 3928 7365 6c66 293a 0a20 2020  it_F9(self):.   
+0000e320: 2020 2020 2022 2222 7374 7562 2222 220a       """stub""".
+0000e330: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+0000e340: 6562 7567 2822 4639 2052 6967 6874 2043  ebug("F9 Right C
+0000e350: 6c69 636b 6564 2e22 290a 2020 2020 2020  licked.").      
+0000e360: 2020 7365 6c66 2e65 6469 745f 6d61 6372    self.edit_macr
+0000e370: 6f28 7365 6c66 2e46 3929 0a0a 2020 2020  o(self.F9)..    
+0000e380: 6465 6620 6564 6974 5f46 3130 2873 656c  def edit_F10(sel
+0000e390: 6629 3a0a 2020 2020 2020 2020 2222 2273  f):.        """s
+0000e3a0: 7475 6222 2222 0a20 2020 2020 2020 206c  tub""".        l
+0000e3b0: 6f67 6765 722e 6465 6275 6728 2246 3130  ogger.debug("F10
+0000e3c0: 2052 6967 6874 2043 6c69 636b 6564 2e22   Right Clicked."
+0000e3d0: 290a 2020 2020 2020 2020 7365 6c66 2e65  ).        self.e
+0000e3e0: 6469 745f 6d61 6372 6f28 7365 6c66 2e46  dit_macro(self.F
+0000e3f0: 3130 290a 0a20 2020 2064 6566 2065 6469  10)..    def edi
+0000e400: 745f 4631 3128 7365 6c66 293a 0a20 2020  t_F11(self):.   
+0000e410: 2020 2020 2022 2222 7374 7562 2222 220a       """stub""".
+0000e420: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+0000e430: 6562 7567 2822 4631 3120 5269 6768 7420  ebug("F11 Right 
+0000e440: 436c 6963 6b65 642e 2229 0a20 2020 2020  Clicked.").     
+0000e450: 2020 2073 656c 662e 6564 6974 5f6d 6163     self.edit_mac
+0000e460: 726f 2873 656c 662e 4631 3129 0a0a 2020  ro(self.F11)..  
+0000e470: 2020 6465 6620 6564 6974 5f46 3132 2873    def edit_F12(s
+0000e480: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+0000e490: 2273 7475 6222 2222 0a20 2020 2020 2020  "stub""".       
+0000e4a0: 206c 6f67 6765 722e 6465 6275 6728 2246   logger.debug("F
+0000e4b0: 3132 2052 6967 6874 2043 6c69 636b 6564  12 Right Clicked
+0000e4c0: 2e22 290a 2020 2020 2020 2020 7365 6c66  .").        self
+0000e4d0: 2e65 6469 745f 6d61 6372 6f28 7365 6c66  .edit_macro(self
+0000e4e0: 2e46 3132 290a 0a20 2020 2064 6566 2070  .F12)..    def p
+0000e4f0: 726f 6365 7373 5f6d 6163 726f 2873 656c  rocess_macro(sel
+0000e500: 662c 206d 6163 726f 3a20 7374 7229 202d  f, macro: str) -
+0000e510: 3e20 7374 723a 0a20 2020 2020 2020 2022  > str:.        "
+0000e520: 2222 5072 6f63 6573 7320 4357 206d 6163  ""Process CW mac
+0000e530: 726f 2073 7562 7374 6974 7574 696f 6e73  ro substitutions
+0000e540: 2222 220a 2020 2020 2020 2020 7265 7375  """.        resu
+0000e550: 6c74 203d 2073 656c 662e 6461 7461 6261  lt = self.databa
+0000e560: 7365 2e67 6574 5f73 6572 6961 6c28 290a  se.get_serial().
+0000e570: 2020 2020 2020 2020 6e65 7874 5f73 6572          next_ser
+0000e580: 6961 6c20 3d20 7374 7228 7265 7375 6c74  ial = str(result
+0000e590: 2e67 6574 2822 7365 7269 616c 5f6e 7222  .get("serial_nr"
+0000e5a0: 2c20 2231 2229 290a 2020 2020 2020 2020  , "1")).        
+0000e5b0: 6966 206e 6578 745f 7365 7269 616c 203d  if next_serial =
+0000e5c0: 3d20 224e 6f6e 6522 3a0a 2020 2020 2020  = "None":.      
+0000e5d0: 2020 2020 2020 6e65 7874 5f73 6572 6961        next_seria
+0000e5e0: 6c20 3d20 2231 220a 2020 2020 2020 2020  l = "1".        
+0000e5f0: 6d61 6372 6f20 3d20 6d61 6372 6f2e 7570  macro = macro.up
+0000e600: 7065 7228 290a 2020 2020 2020 2020 6d61  per().        ma
+0000e610: 6372 6f20 3d20 6d61 6372 6f2e 7265 706c  cro = macro.repl
+0000e620: 6163 6528 2223 222c 206e 6578 745f 7365  ace("#", next_se
+0000e630: 7269 616c 290a 2020 2020 2020 2020 6d61  rial).        ma
+0000e640: 6372 6f20 3d20 6d61 6372 6f2e 7265 706c  cro = macro.repl
+0000e650: 6163 6528 227b 4d59 4341 4c4c 7d22 2c20  ace("{MYCALL}", 
+0000e660: 7365 6c66 2e73 7461 7469 6f6e 2e67 6574  self.station.get
+0000e670: 2822 4361 6c6c 222c 2022 2229 290a 2020  ("Call", "")).  
+0000e680: 2020 2020 2020 6d61 6372 6f20 3d20 6d61        macro = ma
+0000e690: 6372 6f2e 7265 706c 6163 6528 227b 4849  cro.replace("{HI
+0000e6a0: 5343 414c 4c7d 222c 2073 656c 662e 6361  SCALL}", self.ca
+0000e6b0: 6c6c 7369 676e 2e74 6578 7428 2929 0a20  llsign.text()). 
+0000e6c0: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+0000e6d0: 6164 696f 5f73 7461 7465 2e67 6574 2822  adio_state.get("
+0000e6e0: 6d6f 6465 2229 203d 3d20 2243 5722 3a0a  mode") == "CW":.
+0000e6f0: 2020 2020 2020 2020 2020 2020 6d61 6372              macr
+0000e700: 6f20 3d20 6d61 6372 6f2e 7265 706c 6163  o = macro.replac
+0000e710: 6528 227b 534e 547d 222c 2073 656c 662e  e("{SNT}", self.
+0000e720: 7365 6e74 2e74 6578 7428 292e 7265 706c  sent.text().repl
+0000e730: 6163 6528 2239 222c 2022 6e22 2929 0a20  ace("9", "n")). 
+0000e740: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000e750: 2020 2020 2020 2020 206d 6163 726f 203d           macro =
+0000e760: 206d 6163 726f 2e72 6570 6c61 6365 2822   macro.replace("
+0000e770: 7b53 4e54 7d22 2c20 7365 6c66 2e73 656e  {SNT}", self.sen
+0000e780: 742e 7465 7874 2829 290a 2020 2020 2020  t.text()).      
+0000e790: 2020 6d61 6372 6f20 3d20 6d61 6372 6f2e    macro = macro.
+0000e7a0: 7265 706c 6163 6528 227b 5345 4e54 4e52  replace("{SENTNR
+0000e7b0: 7d22 2c20 7365 6c66 2e6f 7468 6572 5f31  }", self.other_1
+0000e7c0: 2e74 6578 7428 2929 0a20 2020 2020 2020  .text()).       
+0000e7d0: 206d 6163 726f 203d 206d 6163 726f 2e72   macro = macro.r
+0000e7e0: 6570 6c61 6365 280a 2020 2020 2020 2020  eplace(.        
+0000e7f0: 2020 2020 227b 4558 4348 7d22 2c20 7365      "{EXCH}", se
+0000e800: 6c66 2e63 6f6e 7465 7374 5f73 6574 7469  lf.contest_setti
+0000e810: 6e67 732e 6765 7428 2253 656e 7445 7863  ngs.get("SentExc
+0000e820: 6861 6e67 6522 2c20 2278 7878 2229 0a20  hange", "xxx"). 
+0000e830: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000e840: 2072 6574 7572 6e20 6d61 6372 6f0a 0a20   return macro.. 
+0000e850: 2020 2064 6566 2076 6f69 6365 5f73 7472     def voice_str
+0000e860: 696e 6728 7365 6c66 2c20 7468 655f 7374  ing(self, the_st
+0000e870: 7269 6e67 3a20 7374 7229 202d 3e20 4e6f  ring: str) -> No
+0000e880: 6e65 3a0a 2020 2020 2020 2020 2222 2276  ne:.        """v
+0000e890: 6f69 6365 7320 7374 7269 6e67 2075 7369  oices string usi
+0000e8a0: 6e67 206e 6174 6f20 7068 6f6e 6574 6963  ng nato phonetic
+0000e8b0: 7322 2222 0a20 2020 2020 2020 206c 6f67  s""".        log
+0000e8c0: 6765 722e 6465 6275 6728 2256 6f69 6369  ger.debug("Voici
+0000e8d0: 6e67 3a20 2573 222c 2074 6865 5f73 7472  ng: %s", the_str
+0000e8e0: 696e 6729 0a20 2020 2020 2020 206f 705f  ing).        op_
+0000e8f0: 7061 7468 203d 2050 6174 6828 4441 5441  path = Path(DATA
+0000e900: 5f50 4154 4829 202f 2073 656c 662e 6375  _PATH) / self.cu
+0000e910: 7272 656e 745f 6f70 0a20 2020 2020 2020  rrent_op.       
+0000e920: 2069 6620 225b 2220 696e 2074 6865 5f73   if "[" in the_s
+0000e930: 7472 696e 673a 0a20 2020 2020 2020 2020  tring:.         
+0000e940: 2020 2073 7562 5f73 7472 696e 6720 3d20     sub_string = 
+0000e950: 7468 655f 7374 7269 6e67 2e73 7472 6970  the_string.strip
+0000e960: 2822 5b5d 2229 2e6c 6f77 6572 2829 0a20  ("[]").lower(). 
+0000e970: 2020 2020 2020 2020 2020 2066 696c 656e             filen
+0000e980: 616d 6520 3d20 6622 7b73 7472 286f 705f  ame = f"{str(op_
+0000e990: 7061 7468 297d 2f7b 7375 625f 7374 7269  path)}/{sub_stri
+0000e9a0: 6e67 7d2e 7761 7622 0a20 2020 2020 2020  ng}.wav".       
+0000e9b0: 2020 2020 2069 6620 5061 7468 2866 696c       if Path(fil
+0000e9c0: 656e 616d 6529 2e69 735f 6669 6c65 2829  ename).is_file()
+0000e9d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000e9e0: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+0000e9f0: 566f 6963 696e 673a 2025 7322 2c20 6669  Voicing: %s", fi
+0000ea00: 6c65 6e61 6d65 290a 2020 2020 2020 2020  lename).        
+0000ea10: 2020 2020 2020 2020 6461 7461 2c20 5f66          data, _f
+0000ea20: 7320 3d20 7366 2e72 6561 6428 6669 6c65  s = sf.read(file
+0000ea30: 6e61 6d65 2c20 6474 7970 653d 2266 6c6f  name, dtype="flo
+0000ea40: 6174 3332 2229 0a20 2020 2020 2020 2020  at32").         
+0000ea50: 2020 2020 2020 2073 656c 662e 7074 745f         self.ptt_
+0000ea60: 6f6e 2829 0a20 2020 2020 2020 2020 2020  on().           
+0000ea70: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+0000ea80: 2020 2020 2020 2020 2020 2020 2020 7364                sd
+0000ea90: 2e64 6566 6175 6c74 2e64 6576 6963 6520  .default.device 
+0000eaa0: 3d20 7365 6c66 2e70 7265 662e 6765 7428  = self.pref.get(
+0000eab0: 2273 6f75 6e64 6465 7669 6365 222c 2022  "sounddevice", "
+0000eac0: 6465 6661 756c 7422 290a 2020 2020 2020  default").      
+0000ead0: 2020 2020 2020 2020 2020 2020 2020 7364                sd
+0000eae0: 2e64 6566 6175 6c74 2e73 616d 706c 6572  .default.sampler
+0000eaf0: 6174 6520 3d20 3434 3130 302e 300a 2020  ate = 44100.0.  
+0000eb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb10: 2020 7364 2e70 6c61 7928 6461 7461 290a    sd.play(data).
+0000eb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb30: 2020 2020 5f73 7461 7475 7320 3d20 7364      _status = sd
+0000eb40: 2e77 6169 7428 290a 2020 2020 2020 2020  .wait().        
+0000eb50: 2020 2020 2020 2020 2020 2020 2320 6874              # ht
+0000eb60: 7470 733a 2f2f 736e 796b 2e69 6f2f 6164  tps://snyk.io/ad
+0000eb70: 7669 736f 722f 7079 7468 6f6e 2f73 6f75  visor/python/sou
+0000eb80: 6e64 6465 7669 6365 2f66 756e 6374 696f  nddevice/functio
+0000eb90: 6e73 2f73 6f75 6e64 6465 7669 6365 2e50  ns/sounddevice.P
+0000eba0: 6f72 7441 7564 696f 4572 726f 720a 2020  ortAudioError.  
+0000ebb0: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+0000ebc0: 6365 7074 2073 642e 506f 7274 4175 6469  cept sd.PortAudi
+0000ebd0: 6f45 7272 6f72 2061 7320 6572 723a 0a20  oError as err:. 
+0000ebe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ebf0: 2020 206c 6f67 6765 722e 7761 726e 696e     logger.warnin
+0000ec00: 6728 2225 7322 2c20 6622 7b65 7272 7d22  g("%s", f"{err}"
+0000ec10: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000ec20: 2020 2073 656c 662e 7074 745f 6f66 6628     self.ptt_off(
+0000ec30: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+0000ec40: 7475 726e 0a20 2020 2020 2020 2073 656c  turn.        sel
+0000ec50: 662e 7074 745f 6f6e 2829 0a20 2020 2020  f.ptt_on().     
+0000ec60: 2020 2066 6f72 206c 6574 7465 7220 696e     for letter in
+0000ec70: 2074 6865 5f73 7472 696e 672e 6c6f 7765   the_string.lowe
+0000ec80: 7228 293a 0a20 2020 2020 2020 2020 2020  r():.           
+0000ec90: 2069 6620 6c65 7474 6572 2069 6e20 2261   if letter in "a
+0000eca0: 6263 6465 6667 6869 6a6b 6c6d 6e6f 7071  bcdefghijklmnopq
+0000ecb0: 7273 7475 7677 7879 7a20 3132 3334 3536  rstuvwxyz 123456
+0000ecc0: 3738 3930 223a 0a20 2020 2020 2020 2020  7890":.         
+0000ecd0: 2020 2020 2020 2069 6620 6c65 7474 6572         if letter
+0000ece0: 203d 3d20 2220 223a 0a20 2020 2020 2020   == " ":.       
+0000ecf0: 2020 2020 2020 2020 2020 2020 206c 6574               let
+0000ed00: 7465 7220 3d20 2273 7061 6365 220a 2020  ter = "space".  
+0000ed10: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+0000ed20: 6c65 6e61 6d65 203d 2066 227b 7374 7228  lename = f"{str(
+0000ed30: 6f70 5f70 6174 6829 7d2f 7b6c 6574 7465  op_path)}/{lette
+0000ed40: 727d 2e77 6176 220a 2020 2020 2020 2020  r}.wav".        
+0000ed50: 2020 2020 2020 2020 6966 2050 6174 6828          if Path(
+0000ed60: 6669 6c65 6e61 6d65 292e 6973 5f66 696c  filename).is_fil
+0000ed70: 6528 293a 0a20 2020 2020 2020 2020 2020  e():.           
+0000ed80: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+0000ed90: 6465 6275 6728 2256 6f69 6369 6e67 3a20  debug("Voicing: 
+0000eda0: 2573 222c 2066 696c 656e 616d 6529 0a20  %s", filename). 
+0000edb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000edc0: 2020 2064 6174 612c 205f 6673 203d 2073     data, _fs = s
+0000edd0: 662e 7265 6164 2866 696c 656e 616d 652c  f.read(filename,
+0000ede0: 2064 7479 7065 3d22 666c 6f61 7433 3222   dtype="float32"
+0000edf0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000ee00: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+0000ee10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee20: 2020 2073 642e 6465 6661 756c 742e 6465     sd.default.de
+0000ee30: 7669 6365 203d 2073 656c 662e 7072 6566  vice = self.pref
+0000ee40: 2e67 6574 2822 736f 756e 6464 6576 6963  .get("sounddevic
+0000ee50: 6522 2c20 2264 6566 6175 6c74 2229 0a20  e", "default"). 
+0000ee60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee70: 2020 2020 2020 2073 642e 6465 6661 756c         sd.defaul
+0000ee80: 742e 7361 6d70 6c65 7261 7465 203d 2034  t.samplerate = 4
+0000ee90: 3431 3030 2e30 0a20 2020 2020 2020 2020  4100.0.         
+0000eea0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000eeb0: 642e 706c 6179 2864 6174 6129 0a20 2020  d.play(data).   
+0000eec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eed0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+0000eee0: 6728 2225 7322 2c20 6622 7b73 642e 7761  g("%s", f"{sd.wa
+0000eef0: 6974 2829 7d22 290a 2020 2020 2020 2020  it()}").        
+0000ef00: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+0000ef10: 7074 2073 642e 506f 7274 4175 6469 6f45  pt sd.PortAudioE
+0000ef20: 7272 6f72 2061 7320 6572 723a 0a20 2020  rror as err:.   
+0000ef30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ef40: 2020 2020 206c 6f67 6765 722e 7761 726e       logger.warn
+0000ef50: 696e 6728 2225 7322 2c20 6622 7b65 7272  ing("%s", f"{err
+0000ef60: 7d22 290a 2020 2020 2020 2020 7365 6c66  }").        self
+0000ef70: 2e70 7474 5f6f 6666 2829 0a0a 2020 2020  .ptt_off()..    
+0000ef80: 6465 6620 7074 745f 6f6e 2873 656c 6629  def ptt_on(self)
+0000ef90: 3a0a 2020 2020 2020 2020 2222 2274 7572  :.        """tur
+0000efa0: 6e20 6f6e 2070 7474 2222 220a 2020 2020  n on ptt""".    
+0000efb0: 2020 2020 6966 2073 656c 662e 7269 675f      if self.rig_
+0000efc0: 636f 6e74 726f 6c3a 0a20 2020 2020 2020  control:.       
+0000efd0: 2020 2020 2073 656c 662e 6c65 6674 646f       self.leftdo
+0000efe0: 742e 7365 7450 6978 6d61 7028 7365 6c66  t.setPixmap(self
+0000eff0: 2e67 7265 656e 646f 7429 0a20 2020 2020  .greendot).     
+0000f000: 2020 2020 2020 2061 7070 2e70 726f 6365         app.proce
+0000f010: 7373 4576 656e 7473 2829 0a20 2020 2020  ssEvents().     
+0000f020: 2020 2020 2020 2073 656c 662e 7269 675f         self.rig_
+0000f030: 636f 6e74 726f 6c2e 7074 745f 6f6e 2829  control.ptt_on()
+0000f040: 0a0a 2020 2020 6465 6620 7074 745f 6f66  ..    def ptt_of
+0000f050: 6628 7365 6c66 293a 0a20 2020 2020 2020  f(self):.       
+0000f060: 2022 2222 7475 726e 206f 6666 2070 7474   """turn off ptt
+0000f070: 2222 220a 2020 2020 2020 2020 6966 2073  """.        if s
+0000f080: 656c 662e 7269 675f 636f 6e74 726f 6c3a  elf.rig_control:
+0000f090: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000f0a0: 662e 6c65 6674 646f 742e 7365 7450 6978  f.leftdot.setPix
+0000f0b0: 6d61 7028 7365 6c66 2e72 6564 646f 7429  map(self.reddot)
+0000f0c0: 0a20 2020 2020 2020 2020 2020 2061 7070  .            app
+0000f0d0: 2e70 726f 6365 7373 4576 656e 7473 2829  .processEvents()
+0000f0e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000f0f0: 662e 7269 675f 636f 6e74 726f 6c2e 7074  f.rig_control.pt
+0000f100: 745f 6f66 6628 290a 0a20 2020 2064 6566  t_off()..    def
+0000f110: 2073 656e 6466 3128 7365 6c66 293a 0a20   sendf1(self):. 
+0000f120: 2020 2020 2020 2022 2222 7374 7562 2222         """stub""
+0000f130: 220a 2020 2020 2020 2020 6c6f 6767 6572  ".        logger
+0000f140: 2e64 6562 7567 2822 4631 2043 6c69 636b  .debug("F1 Click
+0000f150: 6564 2229 0a20 2020 2020 2020 2069 6620  ed").        if 
+0000f160: 7365 6c66 2e6e 316d 6d3a 0a20 2020 2020  self.n1mm:.     
+0000f170: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
+0000f180: 2e72 6164 696f 5f69 6e66 6f5b 2246 756e  .radio_info["Fun
+0000f190: 6374 696f 6e4b 6579 4361 7074 696f 6e22  ctionKeyCaption"
+0000f1a0: 5d20 3d20 7365 6c66 2e46 312e 7465 7874  ] = self.F1.text
+0000f1b0: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+0000f1c0: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
+0000f1d0: 6574 2822 6d6f 6465 2229 2069 6e20 5b22  et("mode") in ["
+0000f1e0: 4c53 4222 2c20 2255 5342 222c 2022 5353  LSB", "USB", "SS
+0000f1f0: 4222 5d3a 0a20 2020 2020 2020 2020 2020  B"]:.           
+0000f200: 2073 656c 662e 766f 6963 655f 7374 7269   self.voice_stri
+0000f210: 6e67 2873 656c 662e 7072 6f63 6573 735f  ng(self.process_
+0000f220: 6d61 6372 6f28 7365 6c66 2e46 312e 746f  macro(self.F1.to
+0000f230: 6f6c 5469 7028 2929 290a 2020 2020 2020  olTip())).      
+0000f240: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+0000f250: 2020 2020 2069 6620 7365 6c66 2e63 773a       if self.cw:
+0000f260: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000f270: 662e 6377 2e73 656e 6463 7728 7365 6c66  f.cw.sendcw(self
+0000f280: 2e70 726f 6365 7373 5f6d 6163 726f 2873  .process_macro(s
+0000f290: 656c 662e 4631 2e74 6f6f 6c54 6970 2829  elf.F1.toolTip()
+0000f2a0: 2929 0a0a 2020 2020 6465 6620 7365 6e64  ))..    def send
+0000f2b0: 6632 2873 656c 6629 3a0a 2020 2020 2020  f2(self):.      
+0000f2c0: 2020 2222 2273 7475 6222 2222 0a20 2020    """stub""".   
+0000f2d0: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+0000f2e0: 6728 2246 3220 436c 6963 6b65 6422 290a  g("F2 Clicked").
+0000f2f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000f300: 6e31 6d6d 3a0a 2020 2020 2020 2020 2020  n1mm:.          
+0000f310: 2020 7365 6c66 2e6e 316d 6d2e 7261 6469    self.n1mm.radi
+0000f320: 6f5f 696e 666f 5b22 4675 6e63 7469 6f6e  o_info["Function
+0000f330: 4b65 7943 6170 7469 6f6e 225d 203d 2073  KeyCaption"] = s
+0000f340: 656c 662e 4632 2e74 6578 7428 290a 2020  elf.F2.text().  
+0000f350: 2020 2020 2020 6966 2073 656c 662e 7261        if self.ra
+0000f360: 6469 6f5f 7374 6174 652e 6765 7428 226d  dio_state.get("m
+0000f370: 6f64 6522 2920 696e 205b 224c 5342 222c  ode") in ["LSB",
+0000f380: 2022 5553 4222 2c20 2253 5342 225d 3a0a   "USB", "SSB"]:.
+0000f390: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f3a0: 2e76 6f69 6365 5f73 7472 696e 6728 7365  .voice_string(se
+0000f3b0: 6c66 2e70 726f 6365 7373 5f6d 6163 726f  lf.process_macro
+0000f3c0: 2873 656c 662e 4632 2e74 6f6f 6c54 6970  (self.F2.toolTip
+0000f3d0: 2829 2929 0a20 2020 2020 2020 2020 2020  ())).           
+0000f3e0: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+0000f3f0: 6966 2073 656c 662e 6377 3a0a 2020 2020  if self.cw:.    
+0000f400: 2020 2020 2020 2020 7365 6c66 2e63 772e          self.cw.
+0000f410: 7365 6e64 6377 2873 656c 662e 7072 6f63  sendcw(self.proc
+0000f420: 6573 735f 6d61 6372 6f28 7365 6c66 2e46  ess_macro(self.F
+0000f430: 322e 746f 6f6c 5469 7028 2929 290a 0a20  2.toolTip())).. 
+0000f440: 2020 2064 6566 2073 656e 6466 3328 7365     def sendf3(se
+0000f450: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+0000f460: 7374 7562 2222 220a 2020 2020 2020 2020  stub""".        
+0000f470: 6c6f 6767 6572 2e64 6562 7567 2822 4633  logger.debug("F3
+0000f480: 2043 6c69 636b 6564 2229 0a20 2020 2020   Clicked").     
+0000f490: 2020 2069 6620 7365 6c66 2e6e 316d 6d3a     if self.n1mm:
+0000f4a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000f4b0: 662e 6e31 6d6d 2e72 6164 696f 5f69 6e66  f.n1mm.radio_inf
+0000f4c0: 6f5b 2246 756e 6374 696f 6e4b 6579 4361  o["FunctionKeyCa
+0000f4d0: 7074 696f 6e22 5d20 3d20 7365 6c66 2e46  ption"] = self.F
+0000f4e0: 332e 7465 7874 2829 0a20 2020 2020 2020  3.text().       
+0000f4f0: 2069 6620 7365 6c66 2e72 6164 696f 5f73   if self.radio_s
+0000f500: 7461 7465 2e67 6574 2822 6d6f 6465 2229  tate.get("mode")
+0000f510: 2069 6e20 5b22 4c53 4222 2c20 2255 5342   in ["LSB", "USB
+0000f520: 222c 2022 5353 4222 5d3a 0a20 2020 2020  ", "SSB"]:.     
+0000f530: 2020 2020 2020 2073 656c 662e 766f 6963         self.voic
+0000f540: 655f 7374 7269 6e67 2873 656c 662e 7072  e_string(self.pr
+0000f550: 6f63 6573 735f 6d61 6372 6f28 7365 6c66  ocess_macro(self
+0000f560: 2e46 332e 746f 6f6c 5469 7028 2929 290a  .F3.toolTip())).
+0000f570: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000f580: 726e 0a20 2020 2020 2020 2069 6620 7365  rn.        if se
+0000f590: 6c66 2e63 773a 0a20 2020 2020 2020 2020  lf.cw:.         
+0000f5a0: 2020 2073 656c 662e 6377 2e73 656e 6463     self.cw.sendc
+0000f5b0: 7728 7365 6c66 2e70 726f 6365 7373 5f6d  w(self.process_m
+0000f5c0: 6163 726f 2873 656c 662e 4633 2e74 6f6f  acro(self.F3.too
+0000f5d0: 6c54 6970 2829 2929 0a0a 2020 2020 6465  lTip()))..    de
+0000f5e0: 6620 7365 6e64 6634 2873 656c 6629 3a0a  f sendf4(self):.
+0000f5f0: 2020 2020 2020 2020 2222 2273 7475 6222          """stub"
+0000f600: 2222 0a20 2020 2020 2020 206c 6f67 6765  "".        logge
+0000f610: 722e 6465 6275 6728 2246 3420 436c 6963  r.debug("F4 Clic
+0000f620: 6b65 6422 290a 2020 2020 2020 2020 6966  ked").        if
+0000f630: 2073 656c 662e 6e31 6d6d 3a0a 2020 2020   self.n1mm:.    
+0000f640: 2020 2020 2020 2020 7365 6c66 2e6e 316d          self.n1m
+0000f650: 6d2e 7261 6469 6f5f 696e 666f 5b22 4675  m.radio_info["Fu
+0000f660: 6e63 7469 6f6e 4b65 7943 6170 7469 6f6e  nctionKeyCaption
+0000f670: 225d 203d 2073 656c 662e 4634 2e74 6578  "] = self.F4.tex
+0000f680: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+0000f690: 656c 662e 7261 6469 6f5f 7374 6174 652e  elf.radio_state.
+0000f6a0: 6765 7428 226d 6f64 6522 2920 696e 205b  get("mode") in [
+0000f6b0: 224c 5342 222c 2022 5553 4222 2c20 2253  "LSB", "USB", "S
+0000f6c0: 5342 225d 3a0a 2020 2020 2020 2020 2020  SB"]:.          
+0000f6d0: 2020 7365 6c66 2e76 6f69 6365 5f73 7472    self.voice_str
+0000f6e0: 696e 6728 7365 6c66 2e70 726f 6365 7373  ing(self.process
+0000f6f0: 5f6d 6163 726f 2873 656c 662e 4634 2e74  _macro(self.F4.t
+0000f700: 6f6f 6c54 6970 2829 2929 0a20 2020 2020  oolTip())).     
+0000f710: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+0000f720: 2020 2020 2020 6966 2073 656c 662e 6377        if self.cw
+0000f730: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000f740: 6c66 2e63 772e 7365 6e64 6377 2873 656c  lf.cw.sendcw(sel
+0000f750: 662e 7072 6f63 6573 735f 6d61 6372 6f28  f.process_macro(
+0000f760: 7365 6c66 2e46 342e 746f 6f6c 5469 7028  self.F4.toolTip(
+0000f770: 2929 290a 0a20 2020 2064 6566 2073 656e  )))..    def sen
+0000f780: 6466 3528 7365 6c66 293a 0a20 2020 2020  df5(self):.     
+0000f790: 2020 2022 2222 7374 7562 2222 220a 2020     """stub""".  
+0000f7a0: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+0000f7b0: 7567 2822 4635 2043 6c69 636b 6564 2229  ug("F5 Clicked")
+0000f7c0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000f7d0: 2e6e 316d 6d3a 0a20 2020 2020 2020 2020  .n1mm:.         
+0000f7e0: 2020 2073 656c 662e 6e31 6d6d 2e72 6164     self.n1mm.rad
+0000f7f0: 696f 5f69 6e66 6f5b 2246 756e 6374 696f  io_info["Functio
+0000f800: 6e4b 6579 4361 7074 696f 6e22 5d20 3d20  nKeyCaption"] = 
+0000f810: 7365 6c66 2e46 352e 7465 7874 2829 0a20  self.F5.text(). 
+0000f820: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+0000f830: 6164 696f 5f73 7461 7465 2e67 6574 2822  adio_state.get("
+0000f840: 6d6f 6465 2229 2069 6e20 5b22 4c53 4222  mode") in ["LSB"
+0000f850: 2c20 2255 5342 222c 2022 5353 4222 5d3a  , "USB", "SSB"]:
+0000f860: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000f870: 662e 766f 6963 655f 7374 7269 6e67 2873  f.voice_string(s
+0000f880: 656c 662e 7072 6f63 6573 735f 6d61 6372  elf.process_macr
+0000f890: 6f28 7365 6c66 2e46 352e 746f 6f6c 5469  o(self.F5.toolTi
+0000f8a0: 7028 2929 290a 2020 2020 2020 2020 2020  p())).          
+0000f8b0: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+0000f8c0: 2069 6620 7365 6c66 2e63 773a 0a20 2020   if self.cw:.   
+0000f8d0: 2020 2020 2020 2020 2073 656c 662e 6377           self.cw
+0000f8e0: 2e73 656e 6463 7728 7365 6c66 2e70 726f  .sendcw(self.pro
+0000f8f0: 6365 7373 5f6d 6163 726f 2873 656c 662e  cess_macro(self.
+0000f900: 4635 2e74 6f6f 6c54 6970 2829 2929 0a0a  F5.toolTip()))..
+0000f910: 2020 2020 6465 6620 7365 6e64 6636 2873      def sendf6(s
+0000f920: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+0000f930: 2273 7475 6222 2222 0a20 2020 2020 2020  "stub""".       
+0000f940: 206c 6f67 6765 722e 6465 6275 6728 2246   logger.debug("F
+0000f950: 3620 436c 6963 6b65 6422 290a 2020 2020  6 Clicked").    
+0000f960: 2020 2020 6966 2073 656c 662e 6e31 6d6d      if self.n1mm
+0000f970: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000f980: 6c66 2e6e 316d 6d2e 7261 6469 6f5f 696e  lf.n1mm.radio_in
+0000f990: 666f 5b22 4675 6e63 7469 6f6e 4b65 7943  fo["FunctionKeyC
+0000f9a0: 6170 7469 6f6e 225d 203d 2073 656c 662e  aption"] = self.
+0000f9b0: 4636 2e74 6578 7428 290a 2020 2020 2020  F6.text().      
+0000f9c0: 2020 6966 2073 656c 662e 7261 6469 6f5f    if self.radio_
+0000f9d0: 7374 6174 652e 6765 7428 226d 6f64 6522  state.get("mode"
+0000f9e0: 2920 696e 205b 224c 5342 222c 2022 5553  ) in ["LSB", "US
+0000f9f0: 4222 2c20 2253 5342 225d 3a0a 2020 2020  B", "SSB"]:.    
+0000fa00: 2020 2020 2020 2020 7365 6c66 2e76 6f69          self.voi
+0000fa10: 6365 5f73 7472 696e 6728 7365 6c66 2e70  ce_string(self.p
+0000fa20: 726f 6365 7373 5f6d 6163 726f 2873 656c  rocess_macro(sel
+0000fa30: 662e 4636 2e74 6f6f 6c54 6970 2829 2929  f.F6.toolTip()))
+0000fa40: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000fa50: 7572 6e0a 2020 2020 2020 2020 6966 2073  urn.        if s
+0000fa60: 656c 662e 6377 3a0a 2020 2020 2020 2020  elf.cw:.        
+0000fa70: 2020 2020 7365 6c66 2e63 772e 7365 6e64      self.cw.send
+0000fa80: 6377 2873 656c 662e 7072 6f63 6573 735f  cw(self.process_
+0000fa90: 6d61 6372 6f28 7365 6c66 2e46 362e 746f  macro(self.F6.to
+0000faa0: 6f6c 5469 7028 2929 290a 0a20 2020 2064  olTip()))..    d
+0000fab0: 6566 2073 656e 6466 3728 7365 6c66 293a  ef sendf7(self):
+0000fac0: 0a20 2020 2020 2020 2022 2222 7374 7562  .        """stub
+0000fad0: 2222 220a 2020 2020 2020 2020 6c6f 6767  """.        logg
+0000fae0: 6572 2e64 6562 7567 2822 4637 2043 6c69  er.debug("F7 Cli
+0000faf0: 636b 6564 2229 0a20 2020 2020 2020 2069  cked").        i
+0000fb00: 6620 7365 6c66 2e6e 316d 6d3a 0a20 2020  f self.n1mm:.   
+0000fb10: 2020 2020 2020 2020 2073 656c 662e 6e31           self.n1
+0000fb20: 6d6d 2e72 6164 696f 5f69 6e66 6f5b 2246  mm.radio_info["F
+0000fb30: 756e 6374 696f 6e4b 6579 4361 7074 696f  unctionKeyCaptio
+0000fb40: 6e22 5d20 3d20 7365 6c66 2e46 372e 7465  n"] = self.F7.te
+0000fb50: 7874 2829 0a20 2020 2020 2020 2069 6620  xt().        if 
+0000fb60: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
+0000fb70: 2e67 6574 2822 6d6f 6465 2229 2069 6e20  .get("mode") in 
+0000fb80: 5b22 4c53 4222 2c20 2255 5342 222c 2022  ["LSB", "USB", "
+0000fb90: 5353 4222 5d3a 0a20 2020 2020 2020 2020  SSB"]:.         
+0000fba0: 2020 2073 656c 662e 766f 6963 655f 7374     self.voice_st
+0000fbb0: 7269 6e67 2873 656c 662e 7072 6f63 6573  ring(self.proces
+0000fbc0: 735f 6d61 6372 6f28 7365 6c66 2e46 372e  s_macro(self.F7.
+0000fbd0: 746f 6f6c 5469 7028 2929 290a 2020 2020  toolTip())).    
+0000fbe0: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+0000fbf0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+0000fc00: 773a 0a20 2020 2020 2020 2020 2020 2073  w:.            s
+0000fc10: 656c 662e 6377 2e73 656e 6463 7728 7365  elf.cw.sendcw(se
+0000fc20: 6c66 2e70 726f 6365 7373 5f6d 6163 726f  lf.process_macro
+0000fc30: 2873 656c 662e 4637 2e74 6f6f 6c54 6970  (self.F7.toolTip
+0000fc40: 2829 2929 0a0a 2020 2020 6465 6620 7365  ()))..    def se
+0000fc50: 6e64 6638 2873 656c 6629 3a0a 2020 2020  ndf8(self):.    
+0000fc60: 2020 2020 2222 2273 7475 6222 2222 0a20      """stub""". 
+0000fc70: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+0000fc80: 6275 6728 2246 3820 436c 6963 6b65 6422  bug("F8 Clicked"
+0000fc90: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+0000fca0: 662e 6e31 6d6d 3a0a 2020 2020 2020 2020  f.n1mm:.        
+0000fcb0: 2020 2020 7365 6c66 2e6e 316d 6d2e 7261      self.n1mm.ra
+0000fcc0: 6469 6f5f 696e 666f 5b22 4675 6e63 7469  dio_info["Functi
+0000fcd0: 6f6e 4b65 7943 6170 7469 6f6e 225d 203d  onKeyCaption"] =
+0000fce0: 2073 656c 662e 4638 2e74 6578 7428 290a   self.F8.text().
 0000fcf0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000fd00: 6e31 6d6d 3a0a 2020 2020 2020 2020 2020  n1mm:.          
-0000fd10: 2020 7365 6c66 2e6e 316d 6d2e 7261 6469    self.n1mm.radi
-0000fd20: 6f5f 696e 666f 5b22 4675 6e63 7469 6f6e  o_info["Function
-0000fd30: 4b65 7943 6170 7469 6f6e 225d 203d 2073  KeyCaption"] = s
-0000fd40: 656c 662e 4639 2e74 6578 7428 290a 2020  elf.F9.text().  
-0000fd50: 2020 2020 2020 6966 2073 656c 662e 7261        if self.ra
-0000fd60: 6469 6f5f 7374 6174 652e 6765 7428 226d  dio_state.get("m
-0000fd70: 6f64 6522 2920 696e 205b 224c 5342 222c  ode") in ["LSB",
-0000fd80: 2022 5553 4222 2c20 2253 5342 225d 3a0a   "USB", "SSB"]:.
-0000fd90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000fda0: 2e76 6f69 6365 5f73 7472 696e 6728 7365  .voice_string(se
-0000fdb0: 6c66 2e70 726f 6365 7373 5f6d 6163 726f  lf.process_macro
-0000fdc0: 2873 656c 662e 4639 2e74 6f6f 6c54 6970  (self.F9.toolTip
-0000fdd0: 2829 2929 0a20 2020 2020 2020 2020 2020  ())).           
-0000fde0: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-0000fdf0: 6966 2073 656c 662e 6377 3a0a 2020 2020  if self.cw:.    
-0000fe00: 2020 2020 2020 2020 7365 6c66 2e63 772e          self.cw.
-0000fe10: 7365 6e64 6377 2873 656c 662e 7072 6f63  sendcw(self.proc
-0000fe20: 6573 735f 6d61 6372 6f28 7365 6c66 2e46  ess_macro(self.F
-0000fe30: 392e 746f 6f6c 5469 7028 2929 290a 0a20  9.toolTip())).. 
-0000fe40: 2020 2064 6566 2073 656e 6466 3130 2873     def sendf10(s
-0000fe50: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-0000fe60: 2273 7475 6222 2222 0a20 2020 2020 2020  "stub""".       
-0000fe70: 206c 6f67 6765 722e 6465 6275 6728 2246   logger.debug("F
-0000fe80: 3130 2043 6c69 636b 6564 2229 0a20 2020  10 Clicked").   
-0000fe90: 2020 2020 2069 6620 7365 6c66 2e6e 316d       if self.n1m
-0000fea0: 6d3a 0a20 2020 2020 2020 2020 2020 2073  m:.            s
-0000feb0: 656c 662e 6e31 6d6d 2e72 6164 696f 5f69  elf.n1mm.radio_i
-0000fec0: 6e66 6f5b 2246 756e 6374 696f 6e4b 6579  nfo["FunctionKey
-0000fed0: 4361 7074 696f 6e22 5d20 3d20 7365 6c66  Caption"] = self
-0000fee0: 2e46 3130 2e74 6578 7428 290a 2020 2020  .F10.text().    
-0000fef0: 2020 2020 6966 2073 656c 662e 7261 6469      if self.radi
-0000ff00: 6f5f 7374 6174 652e 6765 7428 226d 6f64  o_state.get("mod
-0000ff10: 6522 2920 696e 205b 224c 5342 222c 2022  e") in ["LSB", "
-0000ff20: 5553 4222 2c20 2253 5342 225d 3a0a 2020  USB", "SSB"]:.  
-0000ff30: 2020 2020 2020 2020 2020 7365 6c66 2e76            self.v
-0000ff40: 6f69 6365 5f73 7472 696e 6728 7365 6c66  oice_string(self
-0000ff50: 2e70 726f 6365 7373 5f6d 6163 726f 2873  .process_macro(s
-0000ff60: 656c 662e 4631 302e 746f 6f6c 5469 7028  elf.F10.toolTip(
-0000ff70: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
-0000ff80: 7265 7475 726e 0a20 2020 2020 2020 2069  return.        i
-0000ff90: 6620 7365 6c66 2e63 773a 0a20 2020 2020  f self.cw:.     
-0000ffa0: 2020 2020 2020 2073 656c 662e 6377 2e73         self.cw.s
-0000ffb0: 656e 6463 7728 7365 6c66 2e70 726f 6365  endcw(self.proce
-0000ffc0: 7373 5f6d 6163 726f 2873 656c 662e 4631  ss_macro(self.F1
-0000ffd0: 302e 746f 6f6c 5469 7028 2929 290a 0a20  0.toolTip())).. 
-0000ffe0: 2020 2064 6566 2073 656e 6466 3131 2873     def sendf11(s
-0000fff0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-00010000: 2273 7475 6222 2222 0a20 2020 2020 2020  "stub""".       
-00010010: 206c 6f67 6765 722e 6465 6275 6728 2246   logger.debug("F
-00010020: 3131 2043 6c69 636b 6564 2229 0a20 2020  11 Clicked").   
-00010030: 2020 2020 2069 6620 7365 6c66 2e6e 316d       if self.n1m
-00010040: 6d3a 0a20 2020 2020 2020 2020 2020 2073  m:.            s
-00010050: 656c 662e 6e31 6d6d 2e72 6164 696f 5f69  elf.n1mm.radio_i
-00010060: 6e66 6f5b 2246 756e 6374 696f 6e4b 6579  nfo["FunctionKey
-00010070: 4361 7074 696f 6e22 5d20 3d20 7365 6c66  Caption"] = self
-00010080: 2e46 3131 2e74 6578 7428 290a 2020 2020  .F11.text().    
-00010090: 2020 2020 6966 2073 656c 662e 7261 6469      if self.radi
-000100a0: 6f5f 7374 6174 652e 6765 7428 226d 6f64  o_state.get("mod
-000100b0: 6522 2920 696e 205b 224c 5342 222c 2022  e") in ["LSB", "
-000100c0: 5553 4222 2c20 2253 5342 225d 3a0a 2020  USB", "SSB"]:.  
-000100d0: 2020 2020 2020 2020 2020 7365 6c66 2e76            self.v
-000100e0: 6f69 6365 5f73 7472 696e 6728 7365 6c66  oice_string(self
-000100f0: 2e70 726f 6365 7373 5f6d 6163 726f 2873  .process_macro(s
-00010100: 656c 662e 4631 312e 746f 6f6c 5469 7028  elf.F11.toolTip(
-00010110: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
-00010120: 7265 7475 726e 0a20 2020 2020 2020 2069  return.        i
-00010130: 6620 7365 6c66 2e63 773a 0a20 2020 2020  f self.cw:.     
-00010140: 2020 2020 2020 2073 656c 662e 6377 2e73         self.cw.s
-00010150: 656e 6463 7728 7365 6c66 2e70 726f 6365  endcw(self.proce
-00010160: 7373 5f6d 6163 726f 2873 656c 662e 4631  ss_macro(self.F1
-00010170: 312e 746f 6f6c 5469 7028 2929 290a 0a20  1.toolTip())).. 
-00010180: 2020 2064 6566 2073 656e 6466 3132 2873     def sendf12(s
-00010190: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-000101a0: 2273 7475 6222 2222 0a20 2020 2020 2020  "stub""".       
-000101b0: 206c 6f67 6765 722e 6465 6275 6728 2246   logger.debug("F
-000101c0: 3132 2043 6c69 636b 6564 2229 0a20 2020  12 Clicked").   
-000101d0: 2020 2020 2069 6620 7365 6c66 2e6e 316d       if self.n1m
-000101e0: 6d3a 0a20 2020 2020 2020 2020 2020 2073  m:.            s
-000101f0: 656c 662e 6e31 6d6d 2e72 6164 696f 5f69  elf.n1mm.radio_i
-00010200: 6e66 6f5b 2246 756e 6374 696f 6e4b 6579  nfo["FunctionKey
-00010210: 4361 7074 696f 6e22 5d20 3d20 7365 6c66  Caption"] = self
-00010220: 2e46 3132 2e74 6578 7428 290a 2020 2020  .F12.text().    
-00010230: 2020 2020 6966 2073 656c 662e 7261 6469      if self.radi
-00010240: 6f5f 7374 6174 652e 6765 7428 226d 6f64  o_state.get("mod
-00010250: 6522 2920 696e 205b 224c 5342 222c 2022  e") in ["LSB", "
-00010260: 5553 4222 2c20 2253 5342 225d 3a0a 2020  USB", "SSB"]:.  
-00010270: 2020 2020 2020 2020 2020 7365 6c66 2e76            self.v
-00010280: 6f69 6365 5f73 7472 696e 6728 7365 6c66  oice_string(self
-00010290: 2e70 726f 6365 7373 5f6d 6163 726f 2873  .process_macro(s
-000102a0: 656c 662e 4631 322e 746f 6f6c 5469 7028  elf.F12.toolTip(
-000102b0: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
-000102c0: 7265 7475 726e 0a20 2020 2020 2020 2069  return.        i
-000102d0: 6620 7365 6c66 2e63 773a 0a20 2020 2020  f self.cw:.     
-000102e0: 2020 2020 2020 2073 656c 662e 6377 2e73         self.cw.s
-000102f0: 656e 6463 7728 7365 6c66 2e70 726f 6365  endcw(self.proce
-00010300: 7373 5f6d 6163 726f 2873 656c 662e 4631  ss_macro(self.F1
-00010310: 322e 746f 6f6c 5469 7028 2929 290a 0a20  2.toolTip())).. 
-00010320: 2020 2064 6566 2072 756e 5f73 705f 6275     def run_sp_bu
-00010330: 7474 6f6e 735f 636c 6963 6b65 6428 7365  ttons_clicked(se
-00010340: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00010350: 4861 6e64 6c65 2072 756e 2f73 2670 206d  Handle run/s&p m
-00010360: 6f64 6522 2222 0a20 2020 2020 2020 2073  ode""".        s
-00010370: 656c 662e 7072 6566 5b22 7275 6e5f 7374  elf.pref["run_st
-00010380: 6174 6522 5d20 3d20 7365 6c66 2e72 6164  ate"] = self.rad
-00010390: 696f 4275 7474 6f6e 5f72 756e 2e69 7343  ioButton_run.isC
-000103a0: 6865 636b 6564 2829 0a20 2020 2020 2020  hecked().       
-000103b0: 2073 656c 662e 7772 6974 655f 7072 6566   self.write_pref
-000103c0: 6572 656e 6365 2829 0a20 2020 2020 2020  erence().       
-000103d0: 2073 656c 662e 7265 6164 5f63 775f 6d61   self.read_cw_ma
-000103e0: 6372 6f73 2829 0a0a 2020 2020 6465 6620  cros()..    def 
-000103f0: 7772 6974 655f 7072 6566 6572 656e 6365  write_preference
-00010400: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00010410: 2222 220a 2020 2020 2020 2020 5772 6974  """.        Writ
-00010420: 6520 7072 6566 6572 656e 6365 7320 746f  e preferences to
-00010430: 206a 736f 6e20 6669 6c65 2e0a 2020 2020   json file..    
-00010440: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00010450: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-00010460: 2077 6974 6820 6f70 656e 280a 2020 2020   with open(.    
-00010470: 2020 2020 2020 2020 2020 2020 434f 4e46              CONF
-00010480: 4947 5f50 4154 4820 2b20 222f 6e6f 7431  IG_PATH + "/not1
-00010490: 6d6d 2e6a 736f 6e22 2c20 2277 7422 2c20  mm.json", "wt", 
-000104a0: 656e 636f 6469 6e67 3d22 7574 662d 3822  encoding="utf-8"
-000104b0: 0a20 2020 2020 2020 2020 2020 2029 2061  .            ) a
-000104c0: 7320 6669 6c65 5f64 6573 6372 6970 746f  s file_descripto
-000104d0: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
-000104e0: 2020 2066 696c 655f 6465 7363 7269 7074     file_descript
-000104f0: 6f72 2e77 7269 7465 2864 756d 7073 2873  or.write(dumps(s
-00010500: 656c 662e 7072 6566 2c20 696e 6465 6e74  elf.pref, indent
-00010510: 3d34 2929 0a20 2020 2020 2020 2020 2020  =4)).           
-00010520: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
-00010530: 2822 7772 6974 696e 673a 2025 7322 2c20  ("writing: %s", 
-00010540: 7365 6c66 2e70 7265 6629 0a20 2020 2020  self.pref).     
-00010550: 2020 2065 7863 6570 7420 494f 4572 726f     except IOErro
-00010560: 7220 6173 2065 7863 6570 7469 6f6e 3a0a  r as exception:.
-00010570: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-00010580: 6572 2e63 7269 7469 6361 6c28 2277 7269  er.critical("wri
-00010590: 7465 7072 6566 6572 656e 6365 733a 2025  tepreferences: %
-000105a0: 7322 2c20 6578 6365 7074 696f 6e29 0a0a  s", exception)..
-000105b0: 2020 2020 6465 6620 7265 6164 7072 6566      def readpref
-000105c0: 6572 656e 6365 7328 7365 6c66 293a 0a20  erences(self):. 
-000105d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000105e0: 2020 2052 6573 746f 7265 2070 7265 6665     Restore prefe
-000105f0: 7265 6e63 6573 2069 6620 7468 6579 2065  rences if they e
-00010600: 7869 7374 2c20 6f74 6865 7277 6973 6520  xist, otherwise 
-00010610: 6372 6561 7465 2073 6f6d 6520 7361 6e65  create some sane
-00010620: 2064 6566 6175 6c74 732e 0a20 2020 2020   defaults..     
-00010630: 2020 2022 2222 0a20 2020 2020 2020 2074     """.        t
-00010640: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00010650: 6966 206f 732e 7061 7468 2e65 7869 7374  if os.path.exist
-00010660: 7328 434f 4e46 4947 5f50 4154 4820 2b20  s(CONFIG_PATH + 
-00010670: 222f 6e6f 7431 6d6d 2e6a 736f 6e22 293a  "/not1mm.json"):
-00010680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010690: 2077 6974 6820 6f70 656e 280a 2020 2020   with open(.    
-000106a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106b0: 434f 4e46 4947 5f50 4154 4820 2b20 222f  CONFIG_PATH + "/
-000106c0: 6e6f 7431 6d6d 2e6a 736f 6e22 2c20 2272  not1mm.json", "r
-000106d0: 7422 2c20 656e 636f 6469 6e67 3d22 7574  t", encoding="ut
-000106e0: 662d 3822 0a20 2020 2020 2020 2020 2020  f-8".           
-000106f0: 2020 2020 2029 2061 7320 6669 6c65 5f64       ) as file_d
-00010700: 6573 6372 6970 746f 723a 0a20 2020 2020  escriptor:.     
-00010710: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00010720: 656c 662e 7072 6566 203d 206c 6f61 6473  elf.pref = loads
-00010730: 2866 696c 655f 6465 7363 7269 7074 6f72  (file_descriptor
-00010740: 2e72 6561 6428 2929 0a20 2020 2020 2020  .read()).       
-00010750: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-00010760: 6765 722e 696e 666f 2822 2573 222c 2073  ger.info("%s", s
-00010770: 656c 662e 7072 6566 290a 2020 2020 2020  elf.pref).      
-00010780: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00010790: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-000107a0: 6572 2e69 6e66 6f28 224e 6f20 7072 6566  er.info("No pref
-000107b0: 6572 656e 6365 2066 696c 652e 2057 7269  erence file. Wri
-000107c0: 7469 6e67 2070 7265 6665 7265 6e63 652e  ting preference.
-000107d0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-000107e0: 2020 2077 6974 6820 6f70 656e 280a 2020     with open(.  
-000107f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010800: 2020 434f 4e46 4947 5f50 4154 4820 2b20    CONFIG_PATH + 
-00010810: 222f 6e6f 7431 6d6d 2e6a 736f 6e22 2c20  "/not1mm.json", 
-00010820: 2277 7422 2c20 656e 636f 6469 6e67 3d22  "wt", encoding="
-00010830: 7574 662d 3822 0a20 2020 2020 2020 2020  utf-8".         
-00010840: 2020 2020 2020 2029 2061 7320 6669 6c65         ) as file
-00010850: 5f64 6573 6372 6970 746f 723a 0a20 2020  _descriptor:.   
-00010860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010870: 2073 656c 662e 7072 6566 203d 2073 656c   self.pref = sel
-00010880: 662e 7072 6566 5f72 6566 2e63 6f70 7928  f.pref_ref.copy(
-00010890: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000108a0: 2020 2020 2020 6669 6c65 5f64 6573 6372        file_descr
-000108b0: 6970 746f 722e 7772 6974 6528 6475 6d70  iptor.write(dump
-000108c0: 7328 7365 6c66 2e70 7265 662c 2069 6e64  s(self.pref, ind
-000108d0: 656e 743d 3429 290a 2020 2020 2020 2020  ent=4)).        
-000108e0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-000108f0: 6572 2e69 6e66 6f28 2225 7322 2c20 7365  er.info("%s", se
-00010900: 6c66 2e70 7265 6629 0a20 2020 2020 2020  lf.pref).       
-00010910: 2065 7863 6570 7420 494f 4572 726f 7220   except IOError 
-00010920: 6173 2065 7863 6570 7469 6f6e 3a0a 2020  as exception:.  
-00010930: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-00010940: 2e63 7269 7469 6361 6c28 2245 7272 6f72  .critical("Error
-00010950: 3a20 2573 222c 2065 7863 6570 7469 6f6e  : %s", exception
-00010960: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00010970: 6c6f 6f6b 5f75 7020 3d20 4e6f 6e65 0a20  look_up = None. 
-00010980: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-00010990: 7265 662e 6765 7428 2275 7365 7172 7a22  ref.get("useqrz"
-000109a0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-000109b0: 656c 662e 6c6f 6f6b 5f75 7020 3d20 5152  elf.look_up = QR
-000109c0: 5a6c 6f6f 6b75 7028 0a20 2020 2020 2020  Zlookup(.       
-000109d0: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
-000109e0: 6566 2e67 6574 2822 6c6f 6f6b 7570 7573  ef.get("lookupus
-000109f0: 6572 6e61 6d65 2229 2c0a 2020 2020 2020  ername"),.      
-00010a00: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-00010a10: 7265 662e 6765 7428 226c 6f6f 6b75 7070  ref.get("lookupp
-00010a20: 6173 7377 6f72 6422 292c 0a20 2020 2020  assword"),.     
-00010a30: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00010a40: 2023 2069 6620 7365 6c66 2e70 7265 662e   # if self.pref.
-00010a50: 6765 7428 2275 7365 6861 6d64 6222 293a  get("usehamdb"):
-00010a60: 0a20 2020 2020 2020 2023 2020 2020 2073  .        #     s
-00010a70: 656c 662e 6c6f 6f6b 5f75 7020 3d20 4861  elf.look_up = Ha
-00010a80: 6d44 426c 6f6f 6b75 7028 290a 2020 2020  mDBlookup().    
-00010a90: 2020 2020 6966 2073 656c 662e 7072 6566      if self.pref
-00010aa0: 2e67 6574 2822 7573 6568 616d 7174 6822  .get("usehamqth"
-00010ab0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-00010ac0: 656c 662e 6c6f 6f6b 5f75 7020 3d20 4861  elf.look_up = Ha
-00010ad0: 6d51 5448 280a 2020 2020 2020 2020 2020  mQTH(.          
-00010ae0: 2020 2020 2020 7365 6c66 2e70 7265 662e        self.pref.
-00010af0: 6765 7428 226c 6f6f 6b75 7075 7365 726e  get("lookupusern
-00010b00: 616d 6522 292c 0a20 2020 2020 2020 2020  ame"),.         
-00010b10: 2020 2020 2020 2073 656c 662e 7072 6566         self.pref
-00010b20: 2e67 6574 2822 6c6f 6f6b 7570 7061 7373  .get("lookuppass
-00010b30: 776f 7264 2229 2c0a 2020 2020 2020 2020  word"),.        
-00010b40: 2020 2020 290a 0a20 2020 2020 2020 2069      )..        i
-00010b50: 6620 7365 6c66 2e70 7265 662e 6765 7428  f self.pref.get(
-00010b60: 2272 756e 5f73 7461 7465 2229 3a0a 2020  "run_state"):.  
-00010b70: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-00010b80: 6164 696f 4275 7474 6f6e 5f72 756e 2e73  adioButton_run.s
-00010b90: 6574 4368 6563 6b65 6428 5472 7565 290a  etChecked(True).
-00010ba0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00010bb0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-00010bc0: 6164 696f 4275 7474 6f6e 5f73 702e 7365  adioButton_sp.se
-00010bd0: 7443 6865 636b 6564 2854 7275 6529 0a0a  tChecked(True)..
-00010be0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00010bf0: 7072 6566 2e67 6574 2822 636f 6d6d 616e  pref.get("comman
-00010c00: 645f 6275 7474 6f6e 7322 293a 0a20 2020  d_buttons"):.   
-00010c10: 2020 2020 2020 2020 2073 656c 662e 6163           self.ac
-00010c20: 7469 6f6e 436f 6d6d 616e 645f 4275 7474  tionCommand_Butt
-00010c30: 6f6e 732e 7365 7443 6865 636b 6564 2854  ons.setChecked(T
-00010c40: 7275 6529 0a20 2020 2020 2020 2065 6c73  rue).        els
-00010c50: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00010c60: 656c 662e 6163 7469 6f6e 436f 6d6d 616e  elf.actionComman
-00010c70: 645f 4275 7474 6f6e 732e 7365 7443 6865  d_Buttons.setChe
-00010c80: 636b 6564 2846 616c 7365 290a 0a20 2020  cked(False)..   
-00010c90: 2020 2020 2069 6620 7365 6c66 2e70 7265       if self.pre
-00010ca0: 662e 6765 7428 2263 775f 6d61 6372 6f73  f.get("cw_macros
-00010cb0: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-00010cc0: 7365 6c66 2e61 6374 696f 6e43 575f 4d61  self.actionCW_Ma
-00010cd0: 6372 6f73 2e73 6574 4368 6563 6b65 6428  cros.setChecked(
-00010ce0: 5472 7565 290a 2020 2020 2020 2020 656c  True).        el
-00010cf0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00010d00: 7365 6c66 2e61 6374 696f 6e43 575f 4d61  self.actionCW_Ma
-00010d10: 6372 6f73 2e73 6574 4368 6563 6b65 6428  cros.setChecked(
-00010d20: 4661 6c73 6529 0a0a 2020 2020 2020 2020  False)..        
-00010d30: 6966 2073 656c 662e 7072 6566 2e67 6574  if self.pref.get
-00010d40: 2822 6261 6e64 735f 6d6f 6465 7322 293a  ("bands_modes"):
-00010d50: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00010d60: 662e 6163 7469 6f6e 4d6f 6465 5f61 6e64  f.actionMode_and
-00010d70: 5f42 616e 6473 2e73 6574 4368 6563 6b65  _Bands.setChecke
-00010d80: 6428 5472 7565 290a 2020 2020 2020 2020  d(True).        
-00010d90: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00010da0: 2020 7365 6c66 2e61 6374 696f 6e4d 6f64    self.actionMod
-00010db0: 655f 616e 645f 4261 6e64 732e 7365 7443  e_and_Bands.setC
-00010dc0: 6865 636b 6564 2846 616c 7365 290a 0a20  hecked(False).. 
-00010dd0: 2020 2020 2020 206d 756c 7469 6361 7374         multicast
-00010de0: 5f67 726f 7570 203d 2073 656c 662e 7072  _group = self.pr
-00010df0: 6566 2e67 6574 2822 6d75 6c74 6963 6173  ef.get("multicas
-00010e00: 745f 6772 6f75 7022 2c20 2232 3339 2e31  t_group", "239.1
-00010e10: 2e31 2e31 2229 0a20 2020 2020 2020 206d  .1.1").        m
-00010e20: 756c 7469 6361 7374 5f70 6f72 7420 3d20  ulticast_port = 
-00010e30: 7365 6c66 2e70 7265 662e 6765 7428 226d  self.pref.get("m
-00010e40: 756c 7469 6361 7374 5f70 6f72 7422 2c20  ulticast_port", 
-00010e50: 3232 3339 290a 2020 2020 2020 2020 696e  2239).        in
-00010e60: 7465 7266 6163 655f 6970 203d 2073 656c  terface_ip = sel
-00010e70: 662e 7072 6566 2e67 6574 2822 696e 7465  f.pref.get("inte
-00010e80: 7266 6163 655f 6970 222c 2022 302e 302e  rface_ip", "0.0.
-00010e90: 302e 3022 290a 2020 2020 2020 2020 7365  0.0").        se
-00010ea0: 6c66 2e6d 756c 7469 6361 7374 5f69 6e74  lf.multicast_int
-00010eb0: 6572 6661 6365 203d 204d 756c 7469 6361  erface = Multica
-00010ec0: 7374 280a 2020 2020 2020 2020 2020 2020  st(.            
-00010ed0: 6d75 6c74 6963 6173 745f 6772 6f75 702c  multicast_group,
-00010ee0: 206d 756c 7469 6361 7374 5f70 6f72 742c   multicast_port,
-00010ef0: 2069 6e74 6572 6661 6365 5f69 700a 2020   interface_ip.  
-00010f00: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00010f10: 7365 6c66 2e6d 756c 7469 6361 7374 5f69  self.multicast_i
-00010f20: 6e74 6572 6661 6365 2e72 6561 6479 5f72  nterface.ready_r
-00010f30: 6561 645f 636f 6e6e 6563 7428 7365 6c66  ead_connect(self
-00010f40: 2e77 6174 6368 5f75 6470 290a 0a20 2020  .watch_udp)..   
-00010f50: 2020 2020 2073 656c 662e 7269 675f 636f       self.rig_co
-00010f60: 6e74 726f 6c20 3d20 4e6f 6e65 0a0a 2020  ntrol = None..  
-00010f70: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
-00010f80: 6566 2e67 6574 2822 7573 6566 6c72 6967  ef.get("useflrig
-00010f90: 222c 2046 616c 7365 293a 0a20 2020 2020  ", False):.     
-00010fa0: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-00010fb0: 6275 6728 0a20 2020 2020 2020 2020 2020  bug(.           
-00010fc0: 2020 2020 2022 5573 696e 6720 666c 7269       "Using flri
-00010fd0: 673a 2025 7322 2c0a 2020 2020 2020 2020  g: %s",.        
-00010fe0: 2020 2020 2020 2020 6622 7b73 656c 662e          f"{self.
-00010ff0: 7072 6566 2e67 6574 2827 4341 545f 6970  pref.get('CAT_ip
-00011000: 2729 7d20 7b73 656c 662e 7072 6566 2e67  ')} {self.pref.g
-00011010: 6574 2827 4341 545f 706f 7274 2729 7d22  et('CAT_port')}"
-00011020: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-00011030: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00011040: 2e72 6967 5f63 6f6e 7472 6f6c 203d 2043  .rig_control = C
-00011050: 4154 280a 2020 2020 2020 2020 2020 2020  AT(.            
-00011060: 2020 2020 2266 6c72 6967 222c 0a20 2020      "flrig",.   
-00011070: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00011080: 662e 7072 6566 2e67 6574 2822 4341 545f  f.pref.get("CAT_
-00011090: 6970 222c 2022 3132 372e 302e 302e 3122  ip", "127.0.0.1"
-000110a0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-000110b0: 2020 2069 6e74 2873 656c 662e 7072 6566     int(self.pref
-000110c0: 2e67 6574 2822 4341 545f 706f 7274 222c  .get("CAT_port",
-000110d0: 2031 3233 3435 2929 2c0a 2020 2020 2020   12345)),.      
-000110e0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000110f0: 6966 2073 656c 662e 7072 6566 2e67 6574  if self.pref.get
-00011100: 2822 7573 6572 6967 6374 6c64 222c 2046  ("userigctld", F
-00011110: 616c 7365 293a 0a20 2020 2020 2020 2020  alse):.         
-00011120: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-00011130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011140: 2022 5573 696e 6720 7269 6763 746c 643a   "Using rigctld:
-00011150: 2025 7322 2c0a 2020 2020 2020 2020 2020   %s",.          
-00011160: 2020 2020 2020 6622 7b73 656c 662e 7072        f"{self.pr
-00011170: 6566 2e67 6574 2827 4341 545f 6970 2729  ef.get('CAT_ip')
-00011180: 7d20 7b73 656c 662e 7072 6566 2e67 6574  } {self.pref.get
-00011190: 2827 4341 545f 706f 7274 2729 7d22 2c0a  ('CAT_port')}",.
-000111a0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000111b0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-000111c0: 6967 5f63 6f6e 7472 6f6c 203d 2043 4154  ig_control = CAT
-000111d0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000111e0: 2020 2272 6967 6374 6c64 222c 0a20 2020    "rigctld",.   
-000111f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00011200: 662e 7072 6566 2e67 6574 2822 4341 545f  f.pref.get("CAT_
-00011210: 6970 222c 2022 3132 372e 302e 302e 3122  ip", "127.0.0.1"
-00011220: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00011230: 2020 2069 6e74 2873 656c 662e 7072 6566     int(self.pref
-00011240: 2e67 6574 2822 4341 545f 706f 7274 222c  .get("CAT_port",
-00011250: 2034 3533 3229 292c 0a20 2020 2020 2020   4532)),.       
-00011260: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-00011270: 6966 2073 656c 662e 7072 6566 2e67 6574  if self.pref.get
-00011280: 2822 6377 7479 7065 222c 2030 2920 3d3d  ("cwtype", 0) ==
-00011290: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
-000112a0: 7365 6c66 2e63 7720 3d20 4e6f 6e65 0a20  self.cw = None. 
-000112b0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000112c0: 2020 2020 2020 2020 2073 656c 662e 6377           self.cw
-000112d0: 203d 2043 5728 0a20 2020 2020 2020 2020   = CW(.         
-000112e0: 2020 2020 2020 2069 6e74 2873 656c 662e         int(self.
-000112f0: 7072 6566 2e67 6574 2822 6377 7479 7065  pref.get("cwtype
-00011300: 2229 292c 0a20 2020 2020 2020 2020 2020  ")),.           
-00011310: 2020 2020 2073 656c 662e 7072 6566 2e67       self.pref.g
-00011320: 6574 2822 6377 6970 2229 2c0a 2020 2020  et("cwip"),.    
-00011330: 2020 2020 2020 2020 2020 2020 696e 7428              int(
-00011340: 7365 6c66 2e70 7265 662e 6765 7428 2263  self.pref.get("c
-00011350: 7770 6f72 7422 2c20 3637 3839 2929 2c0a  wport", 6789)),.
-00011360: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00011370: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00011380: 772e 7370 6565 6420 3d20 3230 0a20 2020  w.speed = 20.   
-00011390: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-000113a0: 2e63 772e 7365 7276 6572 7479 7065 203d  .cw.servertype =
-000113b0: 3d20 323a 0a20 2020 2020 2020 2020 2020  = 2:.           
-000113c0: 2020 2020 2073 656c 662e 6377 2e73 6574       self.cw.set
-000113d0: 5f77 696e 6b65 7965 725f 7370 6565 6428  _winkeyer_speed(
-000113e0: 3230 290a 0a20 2020 2020 2020 2073 656c  20)..        sel
-000113f0: 662e 6e31 6d6d 203d 204e 6f6e 650a 2020  f.n1mm = None.  
-00011400: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
-00011410: 6566 2e67 6574 2822 7365 6e64 5f6e 316d  ef.get("send_n1m
-00011420: 6d5f 7061 636b 6574 7322 2c20 4661 6c73  m_packets", Fals
-00011430: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-00011440: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-00011450: 2020 2020 2073 656c 662e 6e31 6d6d 203d       self.n1mm =
-00011460: 204e 314d 4d28 0a20 2020 2020 2020 2020   N1MM(.         
-00011470: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00011480: 7072 6566 2e67 6574 2822 6e31 6d6d 5f72  pref.get("n1mm_r
-00011490: 6164 696f 706f 7274 222c 2022 3132 372e  adioport", "127.
-000114a0: 302e 302e 313a 3132 3036 3022 292c 0a20  0.0.1:12060"),. 
-000114b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000114c0: 2020 2073 656c 662e 7072 6566 2e67 6574     self.pref.get
-000114d0: 2822 6e31 6d6d 5f63 6f6e 7461 6374 706f  ("n1mm_contactpo
-000114e0: 7274 222c 2022 3132 372e 302e 302e 313a  rt", "127.0.0.1:
-000114f0: 3132 3036 3122 292c 0a20 2020 2020 2020  12061"),.       
-00011500: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00011510: 662e 7072 6566 2e67 6574 2822 6e31 6d6d  f.pref.get("n1mm
-00011520: 5f6c 6f6f 6b75 7070 6f72 7422 2c20 2231  _lookupport", "1
-00011530: 3237 2e30 2e30 2e31 3a31 3230 3630 2229  27.0.0.1:12060")
-00011540: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00011550: 2020 2020 2020 7365 6c66 2e70 7265 662e        self.pref.
-00011560: 6765 7428 226e 316d 6d5f 7363 6f72 6570  get("n1mm_scorep
-00011570: 6f72 7422 2c20 2231 3237 2e30 2e30 2e31  ort", "127.0.0.1
-00011580: 3a31 3230 3630 2229 2c0a 2020 2020 2020  :12060"),.      
-00011590: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-000115a0: 2020 2020 2020 2020 6578 6365 7074 2056          except V
-000115b0: 616c 7565 4572 726f 723a 0a20 2020 2020  alueError:.     
-000115c0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-000115d0: 722e 7761 726e 696e 6728 2225 7322 2c20  r.warning("%s", 
-000115e0: 6622 7b56 616c 7565 4572 726f 727d 2229  f"{ValueError}")
-000115f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00011600: 662e 6e31 6d6d 2e73 656e 645f 7261 6469  f.n1mm.send_radi
-00011610: 6f5f 7061 636b 6574 7320 3d20 7365 6c66  o_packets = self
-00011620: 2e70 7265 662e 6765 7428 2273 656e 645f  .pref.get("send_
-00011630: 6e31 6d6d 5f72 6164 696f 222c 2046 616c  n1mm_radio", Fal
-00011640: 7365 290a 2020 2020 2020 2020 2020 2020  se).            
-00011650: 7365 6c66 2e6e 316d 6d2e 7365 6e64 5f63  self.n1mm.send_c
-00011660: 6f6e 7461 6374 5f70 6163 6b65 7473 203d  ontact_packets =
-00011670: 2073 656c 662e 7072 6566 2e67 6574 2822   self.pref.get("
-00011680: 7365 6e64 5f6e 316d 6d5f 636f 6e74 6163  send_n1mm_contac
-00011690: 7422 2c20 4661 6c73 6529 0a20 2020 2020  t", False).     
-000116a0: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
-000116b0: 2e73 656e 645f 6c6f 6f6b 7570 5f70 6163  .send_lookup_pac
-000116c0: 6b65 7473 203d 2073 656c 662e 7072 6566  kets = self.pref
-000116d0: 2e67 6574 2822 7365 6e64 5f6e 316d 6d5f  .get("send_n1mm_
-000116e0: 6c6f 6f6b 7570 222c 2046 616c 7365 290a  lookup", False).
-000116f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00011700: 2e6e 316d 6d2e 7365 6e64 5f73 636f 7265  .n1mm.send_score
-00011710: 5f70 6163 6b65 7473 203d 2073 656c 662e  _packets = self.
-00011720: 7072 6566 2e67 6574 2822 7365 6e64 5f6e  pref.get("send_n
-00011730: 316d 6d5f 7363 6f72 6522 2c20 4661 6c73  1mm_score", Fals
-00011740: 6529 0a20 2020 2020 2020 2020 2020 2073  e).            s
-00011750: 656c 662e 6e31 6d6d 2e72 6164 696f 5f69  elf.n1mm.radio_i
-00011760: 6e66 6f5b 2253 7461 7469 6f6e 4e61 6d65  nfo["StationName
-00011770: 225d 203d 2073 656c 662e 7072 6566 2e67  "] = self.pref.g
-00011780: 6574 2822 6e31 6d6d 5f73 7461 7469 6f6e  et("n1mm_station
-00011790: 5f6e 616d 6522 2c20 2222 290a 0a20 2020  _name", "")..   
-000117a0: 2020 2020 2073 656c 662e 7368 6f77 5f63       self.show_c
-000117b0: 6f6d 6d61 6e64 5f62 7574 746f 6e73 2829  ommand_buttons()
-000117c0: 0a20 2020 2020 2020 2073 656c 662e 7368  .        self.sh
-000117d0: 6f77 5f43 575f 6d61 6372 6f73 2829 0a20  ow_CW_macros(). 
-000117e0: 2020 2020 2020 2023 2073 656c 662e 7368         # self.sh
-000117f0: 6f77 5f62 616e 645f 6d6f 6465 2829 0a0a  ow_band_mode()..
-00011800: 2020 2020 6465 6620 7761 7463 685f 7564      def watch_ud
-00011810: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-00011820: 2022 2222 5072 6f63 6573 7320 5544 5020   """Process UDP 
-00011830: 6461 7461 6772 616d 732e 2222 220a 2020  datagrams.""".  
-00011840: 2020 2020 2020 7768 696c 6520 7365 6c66        while self
-00011850: 2e6d 756c 7469 6361 7374 5f69 6e74 6572  .multicast_inter
-00011860: 6661 6365 2e73 6572 7665 725f 7564 702e  face.server_udp.
-00011870: 6861 7350 656e 6469 6e67 4461 7461 6772  hasPendingDatagr
-00011880: 616d 7328 293a 0a20 2020 2020 2020 2020  ams():.         
-00011890: 2020 2062 756e 646c 6520 3d20 7365 6c66     bundle = self
-000118a0: 2e6d 756c 7469 6361 7374 5f69 6e74 6572  .multicast_inter
-000118b0: 6661 6365 2e73 6572 7665 725f 7564 702e  face.server_udp.
-000118c0: 7265 6164 4461 7461 6772 616d 280a 2020  readDatagram(.  
-000118d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000118e0: 6c66 2e6d 756c 7469 6361 7374 5f69 6e74  lf.multicast_int
-000118f0: 6572 6661 6365 2e73 6572 7665 725f 7564  erface.server_ud
-00011900: 702e 7065 6e64 696e 6744 6174 6167 7261  p.pendingDatagra
-00011910: 6d53 697a 6528 290a 2020 2020 2020 2020  mSize().        
-00011920: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00011930: 2020 6461 7461 6772 616d 2c20 5f2c 205f    datagram, _, _
-00011940: 203d 2062 756e 646c 650a 2020 2020 2020   = bundle.      
-00011950: 2020 2020 2020 2320 6c6f 6767 6572 2e64        # logger.d
-00011960: 6562 7567 2864 6174 6167 7261 6d2e 6465  ebug(datagram.de
-00011970: 636f 6465 2829 290a 2020 2020 2020 2020  code()).        
-00011980: 2020 2020 6966 2064 6174 6167 7261 6d3a      if datagram:
-00011990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000119a0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-000119b0: 2020 2020 2020 2020 2020 2320 6465 6275            # debu
-000119c0: 675f 696e 666f 203d 2066 227b 6461 7461  g_info = f"{data
-000119d0: 6772 616d 2e64 6563 6f64 6528 297d 220a  gram.decode()}".
-000119e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000119f0: 2020 2020 2320 6c6f 6767 6572 2e64 6562      # logger.deb
-00011a00: 7567 2864 6562 7567 5f69 6e66 6f29 0a20  ug(debug_info). 
-00011a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a20: 2020 206a 736f 6e5f 6461 7461 203d 206c     json_data = l
-00011a30: 6f61 6473 2864 6174 6167 7261 6d2e 6465  oads(datagram.de
-00011a40: 636f 6465 2829 290a 2020 2020 2020 2020  code()).        
-00011a50: 2020 2020 2020 2020 6578 6365 7074 2055          except U
-00011a60: 6e69 636f 6465 4465 636f 6465 4572 726f  nicodeDecodeErro
-00011a70: 7220 6173 2065 7272 3a0a 2020 2020 2020  r as err:.      
-00011a80: 2020 2020 2020 2020 2020 2020 2020 7468                th
-00011a90: 655f 6572 726f 7220 3d20 6622 4e6f 7420  e_error = f"Not 
-00011aa0: 556e 6963 6f64 653a 207b 6572 727d 5c6e  Unicode: {err}\n
-00011ab0: 7b64 6174 6167 7261 6d7d 220a 2020 2020  {datagram}".    
-00011ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ad0: 6c6f 6767 6572 2e77 6172 6e69 6e67 2874  logger.warning(t
-00011ae0: 6865 5f65 7272 6f72 290a 2020 2020 2020  he_error).      
-00011af0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00011b00: 6e74 696e 7565 0a20 2020 2020 2020 2020  ntinue.         
-00011b10: 2020 2020 2020 2065 7863 6570 7420 4a53         except JS
-00011b20: 4f4e 4465 636f 6465 4572 726f 7220 6173  ONDecodeError as
-00011b30: 2065 7272 3a0a 2020 2020 2020 2020 2020   err:.          
-00011b40: 2020 2020 2020 2020 2020 7468 655f 6572            the_er
-00011b50: 726f 7220 3d20 6622 4e6f 7420 4a53 4f4e  ror = f"Not JSON
-00011b60: 3a20 7b65 7272 7d5c 6e7b 6461 7461 6772  : {err}\n{datagr
-00011b70: 616d 7d22 0a20 2020 2020 2020 2020 2020  am}".           
-00011b80: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-00011b90: 7761 726e 696e 6728 7468 655f 6572 726f  warning(the_erro
-00011ba0: 7229 0a20 2020 2020 2020 2020 2020 2020  r).             
-00011bb0: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
-00011bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011bd0: 6966 2028 0a20 2020 2020 2020 2020 2020  if (.           
-00011be0: 2020 2020 2020 2020 206a 736f 6e5f 6461           json_da
-00011bf0: 7461 2e67 6574 2822 636d 6422 2c20 2222  ta.get("cmd", ""
-00011c00: 2920 3d3d 2022 4745 5443 4f4c 554d 4e53  ) == "GETCOLUMNS
-00011c10: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00011c20: 2020 2020 2020 616e 6420 6a73 6f6e 5f64        and json_d
-00011c30: 6174 612e 6765 7428 2273 7461 7469 6f6e  ata.get("station
-00011c40: 222c 2022 2229 203d 3d20 706c 6174 666f  ", "") == platfo
-00011c50: 726d 2e6e 6f64 6528 290a 2020 2020 2020  rm.node().      
-00011c60: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
-00011c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c80: 2069 6620 6861 7361 7474 7228 7365 6c66   if hasattr(self
-00011c90: 2e63 6f6e 7465 7374 2c20 2263 6f6c 756d  .contest, "colum
-00011ca0: 6e73 2229 3a0a 2020 2020 2020 2020 2020  ns"):.          
-00011cb0: 2020 2020 2020 2020 2020 2020 2020 636d                cm
-00011cc0: 6420 3d20 7b7d 0a20 2020 2020 2020 2020  d = {}.         
-00011cd0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00011ce0: 6d64 5b22 636d 6422 5d20 3d20 2253 484f  md["cmd"] = "SHO
-00011cf0: 5743 4f4c 554d 4e53 220a 2020 2020 2020  WCOLUMNS".      
-00011d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d10: 2020 636d 645b 2273 7461 7469 6f6e 225d    cmd["station"]
-00011d20: 203d 2070 6c61 7466 6f72 6d2e 6e6f 6465   = platform.node
-00011d30: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00011d40: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
-00011d50: 434f 4c55 4d4e 5322 5d20 3d20 7365 6c66  COLUMNS"] = self
-00011d60: 2e63 6f6e 7465 7374 2e63 6f6c 756d 6e73  .contest.columns
-00011d70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011d80: 2020 2020 2020 2020 2073 656c 662e 6d75           self.mu
-00011d90: 6c74 6963 6173 745f 696e 7465 7266 6163  lticast_interfac
-00011da0: 652e 7365 6e64 5f61 735f 6a73 6f6e 2863  e.send_as_json(c
-00011db0: 6d64 290a 2020 2020 2020 2020 2020 2020  md).            
-00011dc0: 2020 2020 6966 2028 0a20 2020 2020 2020      if (.       
-00011dd0: 2020 2020 2020 2020 2020 2020 206a 736f               jso
-00011de0: 6e5f 6461 7461 2e67 6574 2822 636d 6422  n_data.get("cmd"
-00011df0: 2c20 2222 2920 3d3d 2022 5455 4e45 220a  , "") == "TUNE".
-00011e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e10: 2020 2020 616e 6420 6a73 6f6e 5f64 6174      and json_dat
-00011e20: 612e 6765 7428 2273 7461 7469 6f6e 222c  a.get("station",
-00011e30: 2022 2229 203d 3d20 706c 6174 666f 726d   "") == platform
-00011e40: 2e6e 6f64 6528 290a 2020 2020 2020 2020  .node().        
-00011e50: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
-00011e60: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00011e70: 2062 277b 2263 6d64 223a 2022 5455 4e45   b'{"cmd": "TUNE
-00011e80: 222c 2022 6672 6571 223a 2037 2e30 3233  ", "freq": 7.023
-00011e90: 352c 2022 7370 6f74 223a 2022 4d4d 3044  5, "spot": "MM0D
-00011ea0: 4749 227d 270a 2020 2020 2020 2020 2020  GI"}'.          
-00011eb0: 2020 2020 2020 2020 2020 7666 6f20 3d20            vfo = 
-00011ec0: 6a73 6f6e 5f64 6174 612e 6765 7428 2266  json_data.get("f
-00011ed0: 7265 7122 290a 2020 2020 2020 2020 2020  req").          
-00011ee0: 2020 2020 2020 2020 2020 7666 6f20 3d20            vfo = 
-00011ef0: 666c 6f61 7428 7666 6f29 202a 2031 3030  float(vfo) * 100
-00011f00: 3030 3030 0a20 2020 2020 2020 2020 2020  0000.           
-00011f10: 2020 2020 2020 2020 2073 656c 662e 7261           self.ra
-00011f20: 6469 6f5f 7374 6174 655b 2276 666f 6122  dio_state["vfoa"
-00011f30: 5d20 3d20 696e 7428 7666 6f29 0a20 2020  ] = int(vfo).   
+0000fd00: 7261 6469 6f5f 7374 6174 652e 6765 7428  radio_state.get(
+0000fd10: 226d 6f64 6522 2920 696e 205b 224c 5342  "mode") in ["LSB
+0000fd20: 222c 2022 5553 4222 2c20 2253 5342 225d  ", "USB", "SSB"]
+0000fd30: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000fd40: 6c66 2e76 6f69 6365 5f73 7472 696e 6728  lf.voice_string(
+0000fd50: 7365 6c66 2e70 726f 6365 7373 5f6d 6163  self.process_mac
+0000fd60: 726f 2873 656c 662e 4638 2e74 6f6f 6c54  ro(self.F8.toolT
+0000fd70: 6970 2829 2929 0a20 2020 2020 2020 2020  ip())).         
+0000fd80: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+0000fd90: 2020 6966 2073 656c 662e 6377 3a0a 2020    if self.cw:.  
+0000fda0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0000fdb0: 772e 7365 6e64 6377 2873 656c 662e 7072  w.sendcw(self.pr
+0000fdc0: 6f63 6573 735f 6d61 6372 6f28 7365 6c66  ocess_macro(self
+0000fdd0: 2e46 382e 746f 6f6c 5469 7028 2929 290a  .F8.toolTip())).
+0000fde0: 0a20 2020 2064 6566 2073 656e 6466 3928  .    def sendf9(
+0000fdf0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+0000fe00: 2222 7374 7562 2222 220a 2020 2020 2020  ""stub""".      
+0000fe10: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+0000fe20: 4639 2043 6c69 636b 6564 2229 0a20 2020  F9 Clicked").   
+0000fe30: 2020 2020 2069 6620 7365 6c66 2e6e 316d       if self.n1m
+0000fe40: 6d3a 0a20 2020 2020 2020 2020 2020 2073  m:.            s
+0000fe50: 656c 662e 6e31 6d6d 2e72 6164 696f 5f69  elf.n1mm.radio_i
+0000fe60: 6e66 6f5b 2246 756e 6374 696f 6e4b 6579  nfo["FunctionKey
+0000fe70: 4361 7074 696f 6e22 5d20 3d20 7365 6c66  Caption"] = self
+0000fe80: 2e46 392e 7465 7874 2829 0a20 2020 2020  .F9.text().     
+0000fe90: 2020 2069 6620 7365 6c66 2e72 6164 696f     if self.radio
+0000fea0: 5f73 7461 7465 2e67 6574 2822 6d6f 6465  _state.get("mode
+0000feb0: 2229 2069 6e20 5b22 4c53 4222 2c20 2255  ") in ["LSB", "U
+0000fec0: 5342 222c 2022 5353 4222 5d3a 0a20 2020  SB", "SSB"]:.   
+0000fed0: 2020 2020 2020 2020 2073 656c 662e 766f           self.vo
+0000fee0: 6963 655f 7374 7269 6e67 2873 656c 662e  ice_string(self.
+0000fef0: 7072 6f63 6573 735f 6d61 6372 6f28 7365  process_macro(se
+0000ff00: 6c66 2e46 392e 746f 6f6c 5469 7028 2929  lf.F9.toolTip())
+0000ff10: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+0000ff20: 7475 726e 0a20 2020 2020 2020 2069 6620  turn.        if 
+0000ff30: 7365 6c66 2e63 773a 0a20 2020 2020 2020  self.cw:.       
+0000ff40: 2020 2020 2073 656c 662e 6377 2e73 656e       self.cw.sen
+0000ff50: 6463 7728 7365 6c66 2e70 726f 6365 7373  dcw(self.process
+0000ff60: 5f6d 6163 726f 2873 656c 662e 4639 2e74  _macro(self.F9.t
+0000ff70: 6f6f 6c54 6970 2829 2929 0a0a 2020 2020  oolTip()))..    
+0000ff80: 6465 6620 7365 6e64 6631 3028 7365 6c66  def sendf10(self
+0000ff90: 293a 0a20 2020 2020 2020 2022 2222 7374  ):.        """st
+0000ffa0: 7562 2222 220a 2020 2020 2020 2020 6c6f  ub""".        lo
+0000ffb0: 6767 6572 2e64 6562 7567 2822 4631 3020  gger.debug("F10 
+0000ffc0: 436c 6963 6b65 6422 290a 2020 2020 2020  Clicked").      
+0000ffd0: 2020 6966 2073 656c 662e 6e31 6d6d 3a0a    if self.n1mm:.
+0000ffe0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000fff0: 2e6e 316d 6d2e 7261 6469 6f5f 696e 666f  .n1mm.radio_info
+00010000: 5b22 4675 6e63 7469 6f6e 4b65 7943 6170  ["FunctionKeyCap
+00010010: 7469 6f6e 225d 203d 2073 656c 662e 4631  tion"] = self.F1
+00010020: 302e 7465 7874 2829 0a20 2020 2020 2020  0.text().       
+00010030: 2069 6620 7365 6c66 2e72 6164 696f 5f73   if self.radio_s
+00010040: 7461 7465 2e67 6574 2822 6d6f 6465 2229  tate.get("mode")
+00010050: 2069 6e20 5b22 4c53 4222 2c20 2255 5342   in ["LSB", "USB
+00010060: 222c 2022 5353 4222 5d3a 0a20 2020 2020  ", "SSB"]:.     
+00010070: 2020 2020 2020 2073 656c 662e 766f 6963         self.voic
+00010080: 655f 7374 7269 6e67 2873 656c 662e 7072  e_string(self.pr
+00010090: 6f63 6573 735f 6d61 6372 6f28 7365 6c66  ocess_macro(self
+000100a0: 2e46 3130 2e74 6f6f 6c54 6970 2829 2929  .F10.toolTip()))
+000100b0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000100c0: 7572 6e0a 2020 2020 2020 2020 6966 2073  urn.        if s
+000100d0: 656c 662e 6377 3a0a 2020 2020 2020 2020  elf.cw:.        
+000100e0: 2020 2020 7365 6c66 2e63 772e 7365 6e64      self.cw.send
+000100f0: 6377 2873 656c 662e 7072 6f63 6573 735f  cw(self.process_
+00010100: 6d61 6372 6f28 7365 6c66 2e46 3130 2e74  macro(self.F10.t
+00010110: 6f6f 6c54 6970 2829 2929 0a0a 2020 2020  oolTip()))..    
+00010120: 6465 6620 7365 6e64 6631 3128 7365 6c66  def sendf11(self
+00010130: 293a 0a20 2020 2020 2020 2022 2222 7374  ):.        """st
+00010140: 7562 2222 220a 2020 2020 2020 2020 6c6f  ub""".        lo
+00010150: 6767 6572 2e64 6562 7567 2822 4631 3120  gger.debug("F11 
+00010160: 436c 6963 6b65 6422 290a 2020 2020 2020  Clicked").      
+00010170: 2020 6966 2073 656c 662e 6e31 6d6d 3a0a    if self.n1mm:.
+00010180: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010190: 2e6e 316d 6d2e 7261 6469 6f5f 696e 666f  .n1mm.radio_info
+000101a0: 5b22 4675 6e63 7469 6f6e 4b65 7943 6170  ["FunctionKeyCap
+000101b0: 7469 6f6e 225d 203d 2073 656c 662e 4631  tion"] = self.F1
+000101c0: 312e 7465 7874 2829 0a20 2020 2020 2020  1.text().       
+000101d0: 2069 6620 7365 6c66 2e72 6164 696f 5f73   if self.radio_s
+000101e0: 7461 7465 2e67 6574 2822 6d6f 6465 2229  tate.get("mode")
+000101f0: 2069 6e20 5b22 4c53 4222 2c20 2255 5342   in ["LSB", "USB
+00010200: 222c 2022 5353 4222 5d3a 0a20 2020 2020  ", "SSB"]:.     
+00010210: 2020 2020 2020 2073 656c 662e 766f 6963         self.voic
+00010220: 655f 7374 7269 6e67 2873 656c 662e 7072  e_string(self.pr
+00010230: 6f63 6573 735f 6d61 6372 6f28 7365 6c66  ocess_macro(self
+00010240: 2e46 3131 2e74 6f6f 6c54 6970 2829 2929  .F11.toolTip()))
+00010250: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00010260: 7572 6e0a 2020 2020 2020 2020 6966 2073  urn.        if s
+00010270: 656c 662e 6377 3a0a 2020 2020 2020 2020  elf.cw:.        
+00010280: 2020 2020 7365 6c66 2e63 772e 7365 6e64      self.cw.send
+00010290: 6377 2873 656c 662e 7072 6f63 6573 735f  cw(self.process_
+000102a0: 6d61 6372 6f28 7365 6c66 2e46 3131 2e74  macro(self.F11.t
+000102b0: 6f6f 6c54 6970 2829 2929 0a0a 2020 2020  oolTip()))..    
+000102c0: 6465 6620 7365 6e64 6631 3228 7365 6c66  def sendf12(self
+000102d0: 293a 0a20 2020 2020 2020 2022 2222 7374  ):.        """st
+000102e0: 7562 2222 220a 2020 2020 2020 2020 6c6f  ub""".        lo
+000102f0: 6767 6572 2e64 6562 7567 2822 4631 3220  gger.debug("F12 
+00010300: 436c 6963 6b65 6422 290a 2020 2020 2020  Clicked").      
+00010310: 2020 6966 2073 656c 662e 6e31 6d6d 3a0a    if self.n1mm:.
+00010320: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010330: 2e6e 316d 6d2e 7261 6469 6f5f 696e 666f  .n1mm.radio_info
+00010340: 5b22 4675 6e63 7469 6f6e 4b65 7943 6170  ["FunctionKeyCap
+00010350: 7469 6f6e 225d 203d 2073 656c 662e 4631  tion"] = self.F1
+00010360: 322e 7465 7874 2829 0a20 2020 2020 2020  2.text().       
+00010370: 2069 6620 7365 6c66 2e72 6164 696f 5f73   if self.radio_s
+00010380: 7461 7465 2e67 6574 2822 6d6f 6465 2229  tate.get("mode")
+00010390: 2069 6e20 5b22 4c53 4222 2c20 2255 5342   in ["LSB", "USB
+000103a0: 222c 2022 5353 4222 5d3a 0a20 2020 2020  ", "SSB"]:.     
+000103b0: 2020 2020 2020 2073 656c 662e 766f 6963         self.voic
+000103c0: 655f 7374 7269 6e67 2873 656c 662e 7072  e_string(self.pr
+000103d0: 6f63 6573 735f 6d61 6372 6f28 7365 6c66  ocess_macro(self
+000103e0: 2e46 3132 2e74 6f6f 6c54 6970 2829 2929  .F12.toolTip()))
+000103f0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00010400: 7572 6e0a 2020 2020 2020 2020 6966 2073  urn.        if s
+00010410: 656c 662e 6377 3a0a 2020 2020 2020 2020  elf.cw:.        
+00010420: 2020 2020 7365 6c66 2e63 772e 7365 6e64      self.cw.send
+00010430: 6377 2873 656c 662e 7072 6f63 6573 735f  cw(self.process_
+00010440: 6d61 6372 6f28 7365 6c66 2e46 3132 2e74  macro(self.F12.t
+00010450: 6f6f 6c54 6970 2829 2929 0a0a 2020 2020  oolTip()))..    
+00010460: 6465 6620 7275 6e5f 7370 5f62 7574 746f  def run_sp_butto
+00010470: 6e73 5f63 6c69 636b 6564 2873 656c 6629  ns_clicked(self)
+00010480: 3a0a 2020 2020 2020 2020 2222 2248 616e  :.        """Han
+00010490: 646c 6520 7275 6e2f 7326 7020 6d6f 6465  dle run/s&p mode
+000104a0: 2222 220a 2020 2020 2020 2020 7365 6c66  """.        self
+000104b0: 2e70 7265 665b 2272 756e 5f73 7461 7465  .pref["run_state
+000104c0: 225d 203d 2073 656c 662e 7261 6469 6f42  "] = self.radioB
+000104d0: 7574 746f 6e5f 7275 6e2e 6973 4368 6563  utton_run.isChec
+000104e0: 6b65 6428 290a 2020 2020 2020 2020 7365  ked().        se
+000104f0: 6c66 2e77 7269 7465 5f70 7265 6665 7265  lf.write_prefere
+00010500: 6e63 6528 290a 2020 2020 2020 2020 7365  nce().        se
+00010510: 6c66 2e72 6561 645f 6377 5f6d 6163 726f  lf.read_cw_macro
+00010520: 7328 290a 0a20 2020 2064 6566 2077 7269  s()..    def wri
+00010530: 7465 5f70 7265 6665 7265 6e63 6528 7365  te_preference(se
+00010540: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+00010550: 0a20 2020 2020 2020 2057 7269 7465 2070  .        Write p
+00010560: 7265 6665 7265 6e63 6573 2074 6f20 6a73  references to js
+00010570: 6f6e 2066 696c 652e 0a20 2020 2020 2020  on file..       
+00010580: 2022 2222 0a20 2020 2020 2020 2074 7279   """.        try
+00010590: 3a0a 2020 2020 2020 2020 2020 2020 7769  :.            wi
+000105a0: 7468 206f 7065 6e28 0a20 2020 2020 2020  th open(.       
+000105b0: 2020 2020 2020 2020 2043 4f4e 4649 475f           CONFIG_
+000105c0: 5041 5448 202b 2022 2f6e 6f74 316d 6d2e  PATH + "/not1mm.
+000105d0: 6a73 6f6e 222c 2022 7774 222c 2065 6e63  json", "wt", enc
+000105e0: 6f64 696e 673d 2275 7466 2d38 220a 2020  oding="utf-8".  
+000105f0: 2020 2020 2020 2020 2020 2920 6173 2066            ) as f
+00010600: 696c 655f 6465 7363 7269 7074 6f72 3a0a  ile_descriptor:.
+00010610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010620: 6669 6c65 5f64 6573 6372 6970 746f 722e  file_descriptor.
+00010630: 7772 6974 6528 6475 6d70 7328 7365 6c66  write(dumps(self
+00010640: 2e70 7265 662c 2069 6e64 656e 743d 3429  .pref, indent=4)
+00010650: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00010660: 2020 6c6f 6767 6572 2e69 6e66 6f28 2277    logger.info("w
+00010670: 7269 7469 6e67 3a20 2573 222c 2073 656c  riting: %s", sel
+00010680: 662e 7072 6566 290a 2020 2020 2020 2020  f.pref).        
+00010690: 6578 6365 7074 2049 4f45 7272 6f72 2061  except IOError a
+000106a0: 7320 6578 6365 7074 696f 6e3a 0a20 2020  s exception:.   
+000106b0: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+000106c0: 6372 6974 6963 616c 2822 7772 6974 6570  critical("writep
+000106d0: 7265 6665 7265 6e63 6573 3a20 2573 222c  references: %s",
+000106e0: 2065 7863 6570 7469 6f6e 290a 0a20 2020   exception)..   
+000106f0: 2064 6566 2072 6561 6470 7265 6665 7265   def readprefere
+00010700: 6e63 6573 2873 656c 6629 3a0a 2020 2020  nces(self):.    
+00010710: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00010720: 5265 7374 6f72 6520 7072 6566 6572 656e  Restore preferen
+00010730: 6365 7320 6966 2074 6865 7920 6578 6973  ces if they exis
+00010740: 742c 206f 7468 6572 7769 7365 2063 7265  t, otherwise cre
+00010750: 6174 6520 736f 6d65 2073 616e 6520 6465  ate some sane de
+00010760: 6661 756c 7473 2e0a 2020 2020 2020 2020  faults..        
+00010770: 2222 220a 2020 2020 2020 2020 7472 793a  """.        try:
+00010780: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00010790: 6f73 2e70 6174 682e 6578 6973 7473 2843  os.path.exists(C
+000107a0: 4f4e 4649 475f 5041 5448 202b 2022 2f6e  ONFIG_PATH + "/n
+000107b0: 6f74 316d 6d2e 6a73 6f6e 2229 3a0a 2020  ot1mm.json"):.  
+000107c0: 2020 2020 2020 2020 2020 2020 2020 7769                wi
+000107d0: 7468 206f 7065 6e28 0a20 2020 2020 2020  th open(.       
+000107e0: 2020 2020 2020 2020 2020 2020 2043 4f4e               CON
+000107f0: 4649 475f 5041 5448 202b 2022 2f6e 6f74  FIG_PATH + "/not
+00010800: 316d 6d2e 6a73 6f6e 222c 2022 7274 222c  1mm.json", "rt",
+00010810: 2065 6e63 6f64 696e 673d 2275 7466 2d38   encoding="utf-8
+00010820: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00010830: 2020 2920 6173 2066 696c 655f 6465 7363    ) as file_desc
+00010840: 7269 7074 6f72 3a0a 2020 2020 2020 2020  riptor:.        
+00010850: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010860: 2e70 7265 6620 3d20 6c6f 6164 7328 6669  .pref = loads(fi
+00010870: 6c65 5f64 6573 6372 6970 746f 722e 7265  le_descriptor.re
+00010880: 6164 2829 290a 2020 2020 2020 2020 2020  ad()).          
+00010890: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+000108a0: 2e69 6e66 6f28 2225 7322 2c20 7365 6c66  .info("%s", self
+000108b0: 2e70 7265 6629 0a20 2020 2020 2020 2020  .pref).         
+000108c0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000108d0: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+000108e0: 696e 666f 2822 4e6f 2070 7265 6665 7265  info("No prefere
+000108f0: 6e63 6520 6669 6c65 2e20 5772 6974 696e  nce file. Writin
+00010900: 6720 7072 6566 6572 656e 6365 2e22 290a  g preference.").
+00010910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010920: 7769 7468 206f 7065 6e28 0a20 2020 2020  with open(.     
+00010930: 2020 2020 2020 2020 2020 2020 2020 2043                 C
+00010940: 4f4e 4649 475f 5041 5448 202b 2022 2f6e  ONFIG_PATH + "/n
+00010950: 6f74 316d 6d2e 6a73 6f6e 222c 2022 7774  ot1mm.json", "wt
+00010960: 222c 2065 6e63 6f64 696e 673d 2275 7466  ", encoding="utf
+00010970: 2d38 220a 2020 2020 2020 2020 2020 2020  -8".            
+00010980: 2020 2020 2920 6173 2066 696c 655f 6465      ) as file_de
+00010990: 7363 7269 7074 6f72 3a0a 2020 2020 2020  scriptor:.      
+000109a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000109b0: 6c66 2e70 7265 6620 3d20 7365 6c66 2e70  lf.pref = self.p
+000109c0: 7265 665f 7265 662e 636f 7079 2829 0a20  ref_ref.copy(). 
+000109d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000109e0: 2020 2066 696c 655f 6465 7363 7269 7074     file_descript
+000109f0: 6f72 2e77 7269 7465 2864 756d 7073 2873  or.write(dumps(s
+00010a00: 656c 662e 7072 6566 2c20 696e 6465 6e74  elf.pref, indent
+00010a10: 3d34 2929 0a20 2020 2020 2020 2020 2020  =4)).           
+00010a20: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+00010a30: 696e 666f 2822 2573 222c 2073 656c 662e  info("%s", self.
+00010a40: 7072 6566 290a 2020 2020 2020 2020 6578  pref).        ex
+00010a50: 6365 7074 2049 4f45 7272 6f72 2061 7320  cept IOError as 
+00010a60: 6578 6365 7074 696f 6e3a 0a20 2020 2020  exception:.     
+00010a70: 2020 2020 2020 206c 6f67 6765 722e 6372         logger.cr
+00010a80: 6974 6963 616c 2822 4572 726f 723a 2025  itical("Error: %
+00010a90: 7322 2c20 6578 6365 7074 696f 6e29 0a0a  s", exception)..
+00010aa0: 2020 2020 2020 2020 7365 6c66 2e6c 6f6f          self.loo
+00010ab0: 6b5f 7570 203d 204e 6f6e 650a 2020 2020  k_up = None.    
+00010ac0: 2020 2020 6966 2073 656c 662e 7072 6566      if self.pref
+00010ad0: 2e67 6574 2822 7573 6571 727a 2229 3a0a  .get("useqrz"):.
+00010ae0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010af0: 2e6c 6f6f 6b5f 7570 203d 2051 525a 6c6f  .look_up = QRZlo
+00010b00: 6f6b 7570 280a 2020 2020 2020 2020 2020  okup(.          
+00010b10: 2020 2020 2020 7365 6c66 2e70 7265 662e        self.pref.
+00010b20: 6765 7428 226c 6f6f 6b75 7075 7365 726e  get("lookupusern
+00010b30: 616d 6522 292c 0a20 2020 2020 2020 2020  ame"),.         
+00010b40: 2020 2020 2020 2073 656c 662e 7072 6566         self.pref
+00010b50: 2e67 6574 2822 6c6f 6f6b 7570 7061 7373  .get("lookuppass
+00010b60: 776f 7264 2229 2c0a 2020 2020 2020 2020  word"),.        
+00010b70: 2020 2020 290a 2020 2020 2020 2020 2320      ).        # 
+00010b80: 6966 2073 656c 662e 7072 6566 2e67 6574  if self.pref.get
+00010b90: 2822 7573 6568 616d 6462 2229 3a0a 2020  ("usehamdb"):.  
+00010ba0: 2020 2020 2020 2320 2020 2020 7365 6c66        #     self
+00010bb0: 2e6c 6f6f 6b5f 7570 203d 2048 616d 4442  .look_up = HamDB
+00010bc0: 6c6f 6f6b 7570 2829 0a20 2020 2020 2020  lookup().       
+00010bd0: 2069 6620 7365 6c66 2e70 7265 662e 6765   if self.pref.ge
+00010be0: 7428 2275 7365 6861 6d71 7468 2229 3a0a  t("usehamqth"):.
+00010bf0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010c00: 2e6c 6f6f 6b5f 7570 203d 2048 616d 5154  .look_up = HamQT
+00010c10: 4828 0a20 2020 2020 2020 2020 2020 2020  H(.             
+00010c20: 2020 2073 656c 662e 7072 6566 2e67 6574     self.pref.get
+00010c30: 2822 6c6f 6f6b 7570 7573 6572 6e61 6d65  ("lookupusername
+00010c40: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
+00010c50: 2020 2020 7365 6c66 2e70 7265 662e 6765      self.pref.ge
+00010c60: 7428 226c 6f6f 6b75 7070 6173 7377 6f72  t("lookuppasswor
+00010c70: 6422 292c 0a20 2020 2020 2020 2020 2020  d"),.           
+00010c80: 2029 0a0a 2020 2020 2020 2020 6966 2073   )..        if s
+00010c90: 656c 662e 7072 6566 2e67 6574 2822 7275  elf.pref.get("ru
+00010ca0: 6e5f 7374 6174 6522 293a 0a20 2020 2020  n_state"):.     
+00010cb0: 2020 2020 2020 2073 656c 662e 7261 6469         self.radi
+00010cc0: 6f42 7574 746f 6e5f 7275 6e2e 7365 7443  oButton_run.setC
+00010cd0: 6865 636b 6564 2854 7275 6529 0a20 2020  hecked(True).   
+00010ce0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00010cf0: 2020 2020 2020 2073 656c 662e 7261 6469         self.radi
+00010d00: 6f42 7574 746f 6e5f 7370 2e73 6574 4368  oButton_sp.setCh
+00010d10: 6563 6b65 6428 5472 7565 290a 0a20 2020  ecked(True)..   
+00010d20: 2020 2020 2069 6620 7365 6c66 2e70 7265       if self.pre
+00010d30: 662e 6765 7428 2263 6f6d 6d61 6e64 5f62  f.get("command_b
+00010d40: 7574 746f 6e73 2229 3a0a 2020 2020 2020  uttons"):.      
+00010d50: 2020 2020 2020 7365 6c66 2e61 6374 696f        self.actio
+00010d60: 6e43 6f6d 6d61 6e64 5f42 7574 746f 6e73  nCommand_Buttons
+00010d70: 2e73 6574 4368 6563 6b65 6428 5472 7565  .setChecked(True
+00010d80: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+00010d90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010da0: 2e61 6374 696f 6e43 6f6d 6d61 6e64 5f42  .actionCommand_B
+00010db0: 7574 746f 6e73 2e73 6574 4368 6563 6b65  uttons.setChecke
+00010dc0: 6428 4661 6c73 6529 0a0a 2020 2020 2020  d(False)..      
+00010dd0: 2020 6966 2073 656c 662e 7072 6566 2e67    if self.pref.g
+00010de0: 6574 2822 6377 5f6d 6163 726f 7322 293a  et("cw_macros"):
+00010df0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00010e00: 662e 6163 7469 6f6e 4357 5f4d 6163 726f  f.actionCW_Macro
+00010e10: 732e 7365 7443 6865 636b 6564 2854 7275  s.setChecked(Tru
+00010e20: 6529 0a20 2020 2020 2020 2065 6c73 653a  e).        else:
+00010e30: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00010e40: 662e 6163 7469 6f6e 4357 5f4d 6163 726f  f.actionCW_Macro
+00010e50: 732e 7365 7443 6865 636b 6564 2846 616c  s.setChecked(Fal
+00010e60: 7365 290a 0a20 2020 2020 2020 2069 6620  se)..        if 
+00010e70: 7365 6c66 2e70 7265 662e 6765 7428 2262  self.pref.get("b
+00010e80: 616e 6473 5f6d 6f64 6573 2229 3a0a 2020  ands_modes"):.  
+00010e90: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00010ea0: 6374 696f 6e4d 6f64 655f 616e 645f 4261  ctionMode_and_Ba
+00010eb0: 6e64 732e 7365 7443 6865 636b 6564 2854  nds.setChecked(T
+00010ec0: 7275 6529 0a20 2020 2020 2020 2065 6c73  rue).        els
+00010ed0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00010ee0: 656c 662e 6163 7469 6f6e 4d6f 6465 5f61  elf.actionMode_a
+00010ef0: 6e64 5f42 616e 6473 2e73 6574 4368 6563  nd_Bands.setChec
+00010f00: 6b65 6428 4661 6c73 6529 0a0a 2020 2020  ked(False)..    
+00010f10: 2020 2020 6d75 6c74 6963 6173 745f 6772      multicast_gr
+00010f20: 6f75 7020 3d20 7365 6c66 2e70 7265 662e  oup = self.pref.
+00010f30: 6765 7428 226d 756c 7469 6361 7374 5f67  get("multicast_g
+00010f40: 726f 7570 222c 2022 3233 392e 312e 312e  roup", "239.1.1.
+00010f50: 3122 290a 2020 2020 2020 2020 6d75 6c74  1").        mult
+00010f60: 6963 6173 745f 706f 7274 203d 2073 656c  icast_port = sel
+00010f70: 662e 7072 6566 2e67 6574 2822 6d75 6c74  f.pref.get("mult
+00010f80: 6963 6173 745f 706f 7274 222c 2032 3233  icast_port", 223
+00010f90: 3929 0a20 2020 2020 2020 2069 6e74 6572  9).        inter
+00010fa0: 6661 6365 5f69 7020 3d20 7365 6c66 2e70  face_ip = self.p
+00010fb0: 7265 662e 6765 7428 2269 6e74 6572 6661  ref.get("interfa
+00010fc0: 6365 5f69 7022 2c20 2230 2e30 2e30 2e30  ce_ip", "0.0.0.0
+00010fd0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00010fe0: 6d75 6c74 6963 6173 745f 696e 7465 7266  multicast_interf
+00010ff0: 6163 6520 3d20 4d75 6c74 6963 6173 7428  ace = Multicast(
+00011000: 0a20 2020 2020 2020 2020 2020 206d 756c  .            mul
+00011010: 7469 6361 7374 5f67 726f 7570 2c20 6d75  ticast_group, mu
+00011020: 6c74 6963 6173 745f 706f 7274 2c20 696e  lticast_port, in
+00011030: 7465 7266 6163 655f 6970 0a20 2020 2020  terface_ip.     
+00011040: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
+00011050: 662e 6d75 6c74 6963 6173 745f 696e 7465  f.multicast_inte
+00011060: 7266 6163 652e 7265 6164 795f 7265 6164  rface.ready_read
+00011070: 5f63 6f6e 6e65 6374 2873 656c 662e 7761  _connect(self.wa
+00011080: 7463 685f 7564 7029 0a0a 2020 2020 2020  tch_udp)..      
+00011090: 2020 7365 6c66 2e72 6967 5f63 6f6e 7472    self.rig_contr
+000110a0: 6f6c 203d 204e 6f6e 650a 0a20 2020 2020  ol = None..     
+000110b0: 2020 2069 6620 7365 6c66 2e70 7265 662e     if self.pref.
+000110c0: 6765 7428 2275 7365 666c 7269 6722 2c20  get("useflrig", 
+000110d0: 4661 6c73 6529 3a0a 2020 2020 2020 2020  False):.        
+000110e0: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+000110f0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00011100: 2020 2255 7369 6e67 2066 6c72 6967 3a20    "Using flrig: 
+00011110: 2573 222c 0a20 2020 2020 2020 2020 2020  %s",.           
+00011120: 2020 2020 2066 227b 7365 6c66 2e70 7265       f"{self.pre
+00011130: 662e 6765 7428 2743 4154 5f69 7027 297d  f.get('CAT_ip')}
+00011140: 207b 7365 6c66 2e70 7265 662e 6765 7428   {self.pref.get(
+00011150: 2743 4154 5f70 6f72 7427 297d 222c 0a20  'CAT_port')}",. 
+00011160: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00011170: 2020 2020 2020 2020 2073 656c 662e 7269           self.ri
+00011180: 675f 636f 6e74 726f 6c20 3d20 4341 5428  g_control = CAT(
+00011190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000111a0: 2022 666c 7269 6722 2c0a 2020 2020 2020   "flrig",.      
+000111b0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+000111c0: 7265 662e 6765 7428 2243 4154 5f69 7022  ref.get("CAT_ip"
+000111d0: 2c20 2231 3237 2e30 2e30 2e31 2229 2c0a  , "127.0.0.1"),.
+000111e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000111f0: 696e 7428 7365 6c66 2e70 7265 662e 6765  int(self.pref.ge
+00011200: 7428 2243 4154 5f70 6f72 7422 2c20 3132  t("CAT_port", 12
+00011210: 3334 3529 292c 0a20 2020 2020 2020 2020  345)),.         
+00011220: 2020 2029 0a20 2020 2020 2020 2069 6620     ).        if 
+00011230: 7365 6c66 2e70 7265 662e 6765 7428 2275  self.pref.get("u
+00011240: 7365 7269 6763 746c 6422 2c20 4661 6c73  serigctld", Fals
+00011250: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+00011260: 6c6f 6767 6572 2e64 6562 7567 280a 2020  logger.debug(.  
+00011270: 2020 2020 2020 2020 2020 2020 2020 2255                "U
+00011280: 7369 6e67 2072 6967 6374 6c64 3a20 2573  sing rigctld: %s
+00011290: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000112a0: 2020 2066 227b 7365 6c66 2e70 7265 662e     f"{self.pref.
+000112b0: 6765 7428 2743 4154 5f69 7027 297d 207b  get('CAT_ip')} {
+000112c0: 7365 6c66 2e70 7265 662e 6765 7428 2743  self.pref.get('C
+000112d0: 4154 5f70 6f72 7427 297d 222c 0a20 2020  AT_port')}",.   
+000112e0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+000112f0: 2020 2020 2020 2073 656c 662e 7269 675f         self.rig_
+00011300: 636f 6e74 726f 6c20 3d20 4341 5428 0a20  control = CAT(. 
+00011310: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00011320: 7269 6763 746c 6422 2c0a 2020 2020 2020  rigctld",.      
+00011330: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+00011340: 7265 662e 6765 7428 2243 4154 5f69 7022  ref.get("CAT_ip"
+00011350: 2c20 2231 3237 2e30 2e30 2e31 2229 2c0a  , "127.0.0.1"),.
+00011360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011370: 696e 7428 7365 6c66 2e70 7265 662e 6765  int(self.pref.ge
+00011380: 7428 2243 4154 5f70 6f72 7422 2c20 3435  t("CAT_port", 45
+00011390: 3332 2929 2c0a 2020 2020 2020 2020 2020  32)),.          
+000113a0: 2020 290a 0a20 2020 2020 2020 2069 6620    )..        if 
+000113b0: 7365 6c66 2e70 7265 662e 6765 7428 2263  self.pref.get("c
+000113c0: 7774 7970 6522 2c20 3029 203d 3d20 303a  wtype", 0) == 0:
+000113d0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000113e0: 662e 6377 203d 204e 6f6e 650a 2020 2020  f.cw = None.    
+000113f0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00011400: 2020 2020 2020 7365 6c66 2e63 7720 3d20        self.cw = 
+00011410: 4357 280a 2020 2020 2020 2020 2020 2020  CW(.            
+00011420: 2020 2020 696e 7428 7365 6c66 2e70 7265      int(self.pre
+00011430: 662e 6765 7428 2263 7774 7970 6522 2929  f.get("cwtype"))
+00011440: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00011450: 2020 7365 6c66 2e70 7265 662e 6765 7428    self.pref.get(
+00011460: 2263 7769 7022 292c 0a20 2020 2020 2020  "cwip"),.       
+00011470: 2020 2020 2020 2020 2069 6e74 2873 656c           int(sel
+00011480: 662e 7072 6566 2e67 6574 2822 6377 706f  f.pref.get("cwpo
+00011490: 7274 222c 2036 3738 3929 292c 0a20 2020  rt", 6789)),.   
+000114a0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+000114b0: 2020 2020 2020 2073 656c 662e 6377 2e73         self.cw.s
+000114c0: 7065 6564 203d 2032 300a 2020 2020 2020  peed = 20.      
+000114d0: 2020 2020 2020 6966 2073 656c 662e 6377        if self.cw
+000114e0: 2e73 6572 7665 7274 7970 6520 3d3d 2032  .servertype == 2
+000114f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00011500: 2020 7365 6c66 2e63 772e 7365 745f 7769    self.cw.set_wi
+00011510: 6e6b 6579 6572 5f73 7065 6564 2832 3029  nkeyer_speed(20)
+00011520: 0a0a 2020 2020 2020 2020 7365 6c66 2e6e  ..        self.n
+00011530: 316d 6d20 3d20 4e6f 6e65 0a20 2020 2020  1mm = None.     
+00011540: 2020 2069 6620 7365 6c66 2e70 7265 662e     if self.pref.
+00011550: 6765 7428 2273 656e 645f 6e31 6d6d 5f70  get("send_n1mm_p
+00011560: 6163 6b65 7473 222c 2046 616c 7365 293a  ackets", False):
+00011570: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
+00011580: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00011590: 2020 7365 6c66 2e6e 316d 6d20 3d20 4e31    self.n1mm = N1
+000115a0: 4d4d 280a 2020 2020 2020 2020 2020 2020  MM(.            
+000115b0: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
+000115c0: 662e 6765 7428 226e 316d 6d5f 7261 6469  f.get("n1mm_radi
+000115d0: 6f70 6f72 7422 2c20 2231 3237 2e30 2e30  oport", "127.0.0
+000115e0: 2e31 3a31 3230 3630 2229 2c0a 2020 2020  .1:12060"),.    
+000115f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011600: 7365 6c66 2e70 7265 662e 6765 7428 226e  self.pref.get("n
+00011610: 316d 6d5f 636f 6e74 6163 7470 6f72 7422  1mm_contactport"
+00011620: 2c20 2231 3237 2e30 2e30 2e31 3a31 3230  , "127.0.0.1:120
+00011630: 3631 2229 2c0a 2020 2020 2020 2020 2020  61"),.          
+00011640: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+00011650: 7265 662e 6765 7428 226e 316d 6d5f 6c6f  ref.get("n1mm_lo
+00011660: 6f6b 7570 706f 7274 222c 2022 3132 372e  okupport", "127.
+00011670: 302e 302e 313a 3132 3036 3022 292c 0a20  0.0.1:12060"),. 
+00011680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011690: 2020 2073 656c 662e 7072 6566 2e67 6574     self.pref.get
+000116a0: 2822 6e31 6d6d 5f73 636f 7265 706f 7274  ("n1mm_scoreport
+000116b0: 222c 2022 3132 372e 302e 302e 313a 3132  ", "127.0.0.1:12
+000116c0: 3036 3022 292c 0a20 2020 2020 2020 2020  060"),.         
+000116d0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000116e0: 2020 2020 2065 7863 6570 7420 5661 6c75       except Valu
+000116f0: 6545 7272 6f72 3a0a 2020 2020 2020 2020  eError:.        
+00011700: 2020 2020 2020 2020 6c6f 6767 6572 2e77          logger.w
+00011710: 6172 6e69 6e67 2822 2573 222c 2066 227b  arning("%s", f"{
+00011720: 5661 6c75 6545 7272 6f72 7d22 290a 2020  ValueError}").  
+00011730: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00011740: 316d 6d2e 7365 6e64 5f72 6164 696f 5f70  1mm.send_radio_p
+00011750: 6163 6b65 7473 203d 2073 656c 662e 7072  ackets = self.pr
+00011760: 6566 2e67 6574 2822 7365 6e64 5f6e 316d  ef.get("send_n1m
+00011770: 6d5f 7261 6469 6f22 2c20 4661 6c73 6529  m_radio", False)
+00011780: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00011790: 662e 6e31 6d6d 2e73 656e 645f 636f 6e74  f.n1mm.send_cont
+000117a0: 6163 745f 7061 636b 6574 7320 3d20 7365  act_packets = se
+000117b0: 6c66 2e70 7265 662e 6765 7428 2273 656e  lf.pref.get("sen
+000117c0: 645f 6e31 6d6d 5f63 6f6e 7461 6374 222c  d_n1mm_contact",
+000117d0: 2046 616c 7365 290a 2020 2020 2020 2020   False).        
+000117e0: 2020 2020 7365 6c66 2e6e 316d 6d2e 7365      self.n1mm.se
+000117f0: 6e64 5f6c 6f6f 6b75 705f 7061 636b 6574  nd_lookup_packet
+00011800: 7320 3d20 7365 6c66 2e70 7265 662e 6765  s = self.pref.ge
+00011810: 7428 2273 656e 645f 6e31 6d6d 5f6c 6f6f  t("send_n1mm_loo
+00011820: 6b75 7022 2c20 4661 6c73 6529 0a20 2020  kup", False).   
+00011830: 2020 2020 2020 2020 2073 656c 662e 6e31           self.n1
+00011840: 6d6d 2e73 656e 645f 7363 6f72 655f 7061  mm.send_score_pa
+00011850: 636b 6574 7320 3d20 7365 6c66 2e70 7265  ckets = self.pre
+00011860: 662e 6765 7428 2273 656e 645f 6e31 6d6d  f.get("send_n1mm
+00011870: 5f73 636f 7265 222c 2046 616c 7365 290a  _score", False).
+00011880: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00011890: 2e6e 316d 6d2e 7261 6469 6f5f 696e 666f  .n1mm.radio_info
+000118a0: 5b22 5374 6174 696f 6e4e 616d 6522 5d20  ["StationName"] 
+000118b0: 3d20 7365 6c66 2e70 7265 662e 6765 7428  = self.pref.get(
+000118c0: 226e 316d 6d5f 7374 6174 696f 6e5f 6e61  "n1mm_station_na
+000118d0: 6d65 222c 2022 2229 0a0a 2020 2020 2020  me", "")..      
+000118e0: 2020 7365 6c66 2e73 686f 775f 636f 6d6d    self.show_comm
+000118f0: 616e 645f 6275 7474 6f6e 7328 290a 2020  and_buttons().  
+00011900: 2020 2020 2020 7365 6c66 2e73 686f 775f        self.show_
+00011910: 4357 5f6d 6163 726f 7328 290a 2020 2020  CW_macros().    
+00011920: 2020 2020 2320 7365 6c66 2e73 686f 775f      # self.show_
+00011930: 6261 6e64 5f6d 6f64 6528 290a 0a20 2020  band_mode()..   
+00011940: 2064 6566 2077 6174 6368 5f75 6470 2873   def watch_udp(s
+00011950: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00011960: 2250 726f 6365 7373 2055 4450 2064 6174  "Process UDP dat
+00011970: 6167 7261 6d73 2e22 2222 0a20 2020 2020  agrams.""".     
+00011980: 2020 2077 6869 6c65 2073 656c 662e 6d75     while self.mu
+00011990: 6c74 6963 6173 745f 696e 7465 7266 6163  lticast_interfac
+000119a0: 652e 7365 7276 6572 5f75 6470 2e68 6173  e.server_udp.has
+000119b0: 5065 6e64 696e 6744 6174 6167 7261 6d73  PendingDatagrams
+000119c0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+000119d0: 6275 6e64 6c65 203d 2073 656c 662e 6d75  bundle = self.mu
+000119e0: 6c74 6963 6173 745f 696e 7465 7266 6163  lticast_interfac
+000119f0: 652e 7365 7276 6572 5f75 6470 2e72 6561  e.server_udp.rea
+00011a00: 6444 6174 6167 7261 6d28 0a20 2020 2020  dDatagram(.     
+00011a10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00011a20: 6d75 6c74 6963 6173 745f 696e 7465 7266  multicast_interf
+00011a30: 6163 652e 7365 7276 6572 5f75 6470 2e70  ace.server_udp.p
+00011a40: 656e 6469 6e67 4461 7461 6772 616d 5369  endingDatagramSi
+00011a50: 7a65 2829 0a20 2020 2020 2020 2020 2020  ze().           
+00011a60: 2029 0a20 2020 2020 2020 2020 2020 2064   ).            d
+00011a70: 6174 6167 7261 6d2c 205f 2c20 5f20 3d20  atagram, _, _ = 
+00011a80: 6275 6e64 6c65 0a20 2020 2020 2020 2020  bundle.         
+00011a90: 2020 2023 206c 6f67 6765 722e 6465 6275     # logger.debu
+00011aa0: 6728 6461 7461 6772 616d 2e64 6563 6f64  g(datagram.decod
+00011ab0: 6528 2929 0a20 2020 2020 2020 2020 2020  e()).           
+00011ac0: 2069 6620 6461 7461 6772 616d 3a0a 2020   if datagram:.  
+00011ad0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00011ae0: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
+00011af0: 2020 2020 2020 2023 2064 6562 7567 5f69         # debug_i
+00011b00: 6e66 6f20 3d20 6622 7b64 6174 6167 7261  nfo = f"{datagra
+00011b10: 6d2e 6465 636f 6465 2829 7d22 0a20 2020  m.decode()}".   
+00011b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b30: 2023 206c 6f67 6765 722e 6465 6275 6728   # logger.debug(
+00011b40: 6465 6275 675f 696e 666f 290a 2020 2020  debug_info).    
+00011b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b60: 6a73 6f6e 5f64 6174 6120 3d20 6c6f 6164  json_data = load
+00011b70: 7328 6461 7461 6772 616d 2e64 6563 6f64  s(datagram.decod
+00011b80: 6528 2929 0a20 2020 2020 2020 2020 2020  e()).           
+00011b90: 2020 2020 2065 7863 6570 7420 556e 6963       except Unic
+00011ba0: 6f64 6544 6563 6f64 6545 7272 6f72 2061  odeDecodeError a
+00011bb0: 7320 6572 723a 0a20 2020 2020 2020 2020  s err:.         
+00011bc0: 2020 2020 2020 2020 2020 2074 6865 5f65             the_e
+00011bd0: 7272 6f72 203d 2066 224e 6f74 2055 6e69  rror = f"Not Uni
+00011be0: 636f 6465 3a20 7b65 7272 7d5c 6e7b 6461  code: {err}\n{da
+00011bf0: 7461 6772 616d 7d22 0a20 2020 2020 2020  tagram}".       
+00011c00: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+00011c10: 6765 722e 7761 726e 696e 6728 7468 655f  ger.warning(the_
+00011c20: 6572 726f 7229 0a20 2020 2020 2020 2020  error).         
+00011c30: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+00011c40: 6e75 650a 2020 2020 2020 2020 2020 2020  nue.            
+00011c50: 2020 2020 6578 6365 7074 204a 534f 4e44      except JSOND
+00011c60: 6563 6f64 6545 7272 6f72 2061 7320 6572  ecodeError as er
+00011c70: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
+00011c80: 2020 2020 2020 2074 6865 5f65 7272 6f72         the_error
+00011c90: 203d 2066 224e 6f74 204a 534f 4e3a 207b   = f"Not JSON: {
+00011ca0: 6572 727d 5c6e 7b64 6174 6167 7261 6d7d  err}\n{datagram}
+00011cb0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00011cc0: 2020 2020 2020 6c6f 6767 6572 2e77 6172        logger.war
+00011cd0: 6e69 6e67 2874 6865 5f65 7272 6f72 290a  ning(the_error).
+00011ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011cf0: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
+00011d00: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00011d10: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00011d20: 2020 2020 2020 6a73 6f6e 5f64 6174 612e        json_data.
+00011d30: 6765 7428 2263 6d64 222c 2022 2229 203d  get("cmd", "") =
+00011d40: 3d20 2247 4554 434f 4c55 4d4e 5322 0a20  = "GETCOLUMNS". 
+00011d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d60: 2020 2061 6e64 206a 736f 6e5f 6461 7461     and json_data
+00011d70: 2e67 6574 2822 7374 6174 696f 6e22 2c20  .get("station", 
+00011d80: 2222 2920 3d3d 2070 6c61 7466 6f72 6d2e  "") == platform.
+00011d90: 6e6f 6465 2829 0a20 2020 2020 2020 2020  node().         
+00011da0: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
+00011db0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00011dc0: 2068 6173 6174 7472 2873 656c 662e 636f   hasattr(self.co
+00011dd0: 6e74 6573 742c 2022 636f 6c75 6d6e 7322  ntest, "columns"
+00011de0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00011df0: 2020 2020 2020 2020 2020 2063 6d64 203d             cmd =
+00011e00: 207b 7d0a 2020 2020 2020 2020 2020 2020   {}.            
+00011e10: 2020 2020 2020 2020 2020 2020 636d 645b              cmd[
+00011e20: 2263 6d64 225d 203d 2022 5348 4f57 434f  "cmd"] = "SHOWCO
+00011e30: 4c55 4d4e 5322 0a20 2020 2020 2020 2020  LUMNS".         
+00011e40: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00011e50: 6d64 5b22 7374 6174 696f 6e22 5d20 3d20  md["station"] = 
+00011e60: 706c 6174 666f 726d 2e6e 6f64 6528 290a  platform.node().
+00011e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e80: 2020 2020 2020 2020 636d 645b 2243 4f4c          cmd["COL
+00011e90: 554d 4e53 225d 203d 2073 656c 662e 636f  UMNS"] = self.co
+00011ea0: 6e74 6573 742e 636f 6c75 6d6e 730a 2020  ntest.columns.  
+00011eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ec0: 2020 2020 2020 7365 6c66 2e6d 756c 7469        self.multi
+00011ed0: 6361 7374 5f69 6e74 6572 6661 6365 2e73  cast_interface.s
+00011ee0: 656e 645f 6173 5f6a 736f 6e28 636d 6429  end_as_json(cmd)
+00011ef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011f00: 2069 6620 280a 2020 2020 2020 2020 2020   if (.          
+00011f10: 2020 2020 2020 2020 2020 6a73 6f6e 5f64            json_d
+00011f20: 6174 612e 6765 7428 2263 6d64 222c 2022  ata.get("cmd", "
+00011f30: 2229 203d 3d20 2254 554e 4522 0a20 2020  ") == "TUNE".   
 00011f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f50: 2069 6620 7365 6c66 2e72 6967 5f63 6f6e   if self.rig_con
-00011f60: 7472 6f6c 3a0a 2020 2020 2020 2020 2020  trol:.          
-00011f70: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00011f80: 6c66 2e72 6967 5f63 6f6e 7472 6f6c 2e73  lf.rig_control.s
-00011f90: 6574 5f76 666f 2869 6e74 2876 666f 2929  et_vfo(int(vfo))
-00011fa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011fb0: 2020 2020 2073 706f 7420 3d20 6a73 6f6e       spot = json
-00011fc0: 5f64 6174 612e 6765 7428 2273 706f 7422  _data.get("spot"
-00011fd0: 2c20 2222 290a 2020 2020 2020 2020 2020  , "").          
-00011fe0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00011ff0: 616c 6c73 6967 6e2e 7365 7454 6578 7428  allsign.setText(
-00012000: 7370 6f74 290a 2020 2020 2020 2020 2020  spot).          
-00012010: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00012020: 616c 6c73 6967 6e5f 6368 616e 6765 6428  allsign_changed(
-00012030: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00012040: 2020 2020 2020 7365 6c66 2e63 616c 6c73        self.calls
-00012050: 6967 6e2e 7365 7446 6f63 7573 2829 0a20  ign.setFocus(). 
-00012060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012070: 2020 2073 656c 662e 6361 6c6c 7369 676e     self.callsign
-00012080: 2e61 6374 6976 6174 6557 696e 646f 7728  .activateWindow(
-00012090: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000120a0: 2020 2020 2020 7769 6e64 6f77 2e72 6169        window.rai
-000120b0: 7365 5f28 290a 0a20 2020 2020 2020 2020  se_()..         
-000120c0: 2020 2020 2020 2069 6620 280a 2020 2020         if (.    
-000120d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120e0: 6a73 6f6e 5f64 6174 612e 6765 7428 2263  json_data.get("c
-000120f0: 6d64 222c 2022 2229 203d 3d20 2247 4554  md", "") == "GET
-00012100: 574f 524b 4544 4c49 5354 220a 2020 2020  WORKEDLIST".    
-00012110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012120: 616e 6420 6a73 6f6e 5f64 6174 612e 6765  and json_data.ge
-00012130: 7428 2273 7461 7469 6f6e 222c 2022 2229  t("station", "")
-00012140: 203d 3d20 706c 6174 666f 726d 2e6e 6f64   == platform.nod
-00012150: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-00012160: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
-00012170: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00012180: 7420 3d20 7365 6c66 2e64 6174 6162 6173  t = self.databas
-00012190: 652e 6765 745f 6361 6c6c 735f 616e 645f  e.get_calls_and_
-000121a0: 6261 6e64 7328 290a 2020 2020 2020 2020  bands().        
-000121b0: 2020 2020 2020 2020 2020 2020 636d 6420              cmd 
-000121c0: 3d20 7b7d 0a20 2020 2020 2020 2020 2020  = {}.           
-000121d0: 2020 2020 2020 2020 2063 6d64 5b22 636d           cmd["cm
-000121e0: 6422 5d20 3d20 2257 4f52 4b45 4422 0a20  d"] = "WORKED". 
-000121f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012200: 2020 2063 6d64 5b22 7374 6174 696f 6e22     cmd["station"
-00012210: 5d20 3d20 706c 6174 666f 726d 2e6e 6f64  ] = platform.nod
-00012220: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-00012230: 2020 2020 2020 2020 636d 645b 2277 6f72          cmd["wor
-00012240: 6b65 6422 5d20 3d20 7265 7375 6c74 0a20  ked"] = result. 
-00012250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012260: 2020 2073 656c 662e 6d75 6c74 6963 6173     self.multicas
-00012270: 745f 696e 7465 7266 6163 652e 7365 6e64  t_interface.send
-00012280: 5f61 735f 6a73 6f6e 2863 6d64 290a 0a20  _as_json(cmd).. 
-00012290: 2020 2064 6566 2063 775f 6d61 6372 6f73     def cw_macros
-000122a0: 5f73 7461 7465 5f63 6861 6e67 6564 2873  _state_changed(s
-000122b0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-000122c0: 224d 656e 7520 6974 656d 2074 6f20 7368  "Menu item to sh
-000122d0: 6f77 2f68 6964 6520 6d61 6372 6f20 6275  ow/hide macro bu
-000122e0: 7474 6f6e 7322 2222 0a20 2020 2020 2020  ttons""".       
-000122f0: 2073 656c 662e 7072 6566 5b22 6377 5f6d   self.pref["cw_m
-00012300: 6163 726f 7322 5d20 3d20 7365 6c66 2e61  acros"] = self.a
-00012310: 6374 696f 6e43 575f 4d61 6372 6f73 2e69  ctionCW_Macros.i
-00012320: 7343 6865 636b 6564 2829 0a20 2020 2020  sChecked().     
-00012330: 2020 2073 656c 662e 7772 6974 655f 7072     self.write_pr
-00012340: 6566 6572 656e 6365 2829 0a20 2020 2020  eference().     
-00012350: 2020 2073 656c 662e 7368 6f77 5f43 575f     self.show_CW_
-00012360: 6d61 6372 6f73 2829 0a0a 2020 2020 6465  macros()..    de
-00012370: 6620 7368 6f77 5f43 575f 6d61 6372 6f73  f show_CW_macros
-00012380: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00012390: 2222 226d 6163 726f 2062 7574 746f 6e20  """macro button 
-000123a0: 7374 6174 6520 6368 616e 6765 2222 220a  state change""".
-000123b0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000123c0: 7072 6566 2e67 6574 2822 6377 5f6d 6163  pref.get("cw_mac
-000123d0: 726f 7322 293a 0a20 2020 2020 2020 2020  ros"):.         
-000123e0: 2020 2073 656c 662e 4275 7474 6f6e 5f52     self.Button_R
-000123f0: 6f77 312e 7368 6f77 2829 0a20 2020 2020  ow1.show().     
-00012400: 2020 2020 2020 2073 656c 662e 4275 7474         self.Butt
-00012410: 6f6e 5f52 6f77 322e 7368 6f77 2829 0a20  on_Row2.show(). 
-00012420: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00012430: 2020 2020 2020 2020 2073 656c 662e 4275           self.Bu
-00012440: 7474 6f6e 5f52 6f77 312e 6869 6465 2829  tton_Row1.hide()
-00012450: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00012460: 662e 4275 7474 6f6e 5f52 6f77 322e 6869  f.Button_Row2.hi
-00012470: 6465 2829 0a0a 2020 2020 6465 6620 636f  de()..    def co
-00012480: 6d6d 616e 645f 6275 7474 6f6e 735f 7374  mmand_buttons_st
-00012490: 6174 655f 6368 616e 6765 2873 656c 6629  ate_change(self)
-000124a0: 3a0a 2020 2020 2020 2020 2222 224d 656e  :.        """Men
-000124b0: 7520 6974 656d 2074 6f20 7368 6f77 2f68  u item to show/h
-000124c0: 6964 6520 636f 6d6d 616e 6420 6275 7474  ide command butt
-000124d0: 6f6e 7322 2222 0a20 2020 2020 2020 2073  ons""".        s
-000124e0: 656c 662e 7072 6566 5b22 636f 6d6d 616e  elf.pref["comman
-000124f0: 645f 6275 7474 6f6e 7322 5d20 3d20 7365  d_buttons"] = se
-00012500: 6c66 2e61 6374 696f 6e43 6f6d 6d61 6e64  lf.actionCommand
-00012510: 5f42 7574 746f 6e73 2e69 7343 6865 636b  _Buttons.isCheck
-00012520: 6564 2829 0a20 2020 2020 2020 2073 656c  ed().        sel
-00012530: 662e 7772 6974 655f 7072 6566 6572 656e  f.write_preferen
-00012540: 6365 2829 0a20 2020 2020 2020 2073 656c  ce().        sel
-00012550: 662e 7368 6f77 5f63 6f6d 6d61 6e64 5f62  f.show_command_b
-00012560: 7574 746f 6e73 2829 0a0a 2020 2020 6465  uttons()..    de
-00012570: 6620 7368 6f77 5f63 6f6d 6d61 6e64 5f62  f show_command_b
-00012580: 7574 746f 6e73 2873 656c 6629 3a0a 2020  uttons(self):.  
-00012590: 2020 2020 2020 2222 2263 6f6d 6d61 6e64        """command
-000125a0: 2062 7574 746f 6e20 7374 6174 6520 6368   button state ch
-000125b0: 616e 6765 2222 220a 2020 2020 2020 2020  ange""".        
-000125c0: 6966 2073 656c 662e 7072 6566 2e67 6574  if self.pref.get
-000125d0: 2822 636f 6d6d 616e 645f 6275 7474 6f6e  ("command_button
-000125e0: 7322 293a 0a20 2020 2020 2020 2020 2020  s"):.           
-000125f0: 2073 656c 662e 436f 6d6d 616e 645f 4275   self.Command_Bu
-00012600: 7474 6f6e 732e 7368 6f77 2829 0a20 2020  ttons.show().   
-00012610: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00012620: 2020 2020 2020 2073 656c 662e 436f 6d6d         self.Comm
-00012630: 616e 645f 4275 7474 6f6e 732e 6869 6465  and_Buttons.hide
-00012640: 2829 0a0a 2020 2020 6465 6620 6973 5f66  ()..    def is_f
-00012650: 6c6f 6174 6162 6c65 2873 656c 662c 2069  loatable(self, i
-00012660: 7465 6d3a 2073 7472 2920 2d3e 2062 6f6f  tem: str) -> boo
-00012670: 6c3a 0a20 2020 2020 2020 2022 2222 6368  l:.        """ch
-00012680: 6563 6b20 746f 2073 6565 2069 6620 7374  eck to see if st
-00012690: 7269 6e67 2063 616e 2062 6520 6120 666c  ring can be a fl
-000126a0: 6f61 7422 2222 0a20 2020 2020 2020 2069  oat""".        i
-000126b0: 6620 6974 656d 2e69 736e 756d 6572 6963  f item.isnumeric
-000126c0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-000126d0: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
-000126e0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-000126f0: 2020 2020 205f 7465 7374 203d 2066 6c6f       _test = flo
-00012700: 6174 2869 7465 6d29 0a20 2020 2020 2020  at(item).       
-00012710: 2065 7863 6570 7420 5661 6c75 6545 7272   except ValueErr
-00012720: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
-00012730: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
-00012740: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-00012750: 0a0a 2020 2020 6465 6620 6f74 6865 725f  ..    def other_
-00012760: 315f 6368 616e 6765 6428 7365 6c66 293a  1_changed(self):
-00012770: 0a20 2020 2020 2020 2022 2222 4361 6c6c  .        """Call
-00012780: 6564 2077 6865 6e2e 2e2e 2079 6f75 206b  ed when... you k
-00012790: 6e6f 772e 2222 220a 2020 2020 2020 2020  now.""".        
-000127a0: 6966 2073 656c 662e 636f 6e74 6573 743a  if self.contest:
-000127b0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000127c0: 6861 7361 7474 7228 7365 6c66 2e63 6f6e  hasattr(self.con
-000127d0: 7465 7374 2c20 2261 6476 616e 6365 5f6f  test, "advance_o
-000127e0: 6e5f 7370 6163 6522 293a 0a20 2020 2020  n_space"):.     
-000127f0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00012800: 6c66 2e63 6f6e 7465 7374 2e61 6476 616e  lf.contest.advan
-00012810: 6365 5f6f 6e5f 7370 6163 655b 335d 3a0a  ce_on_space[3]:.
-00012820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012830: 2020 2020 7465 7874 203d 2073 656c 662e      text = self.
-00012840: 6f74 6865 725f 312e 7465 7874 2829 0a20  other_1.text(). 
-00012850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012860: 2020 2074 6578 7420 3d20 7465 7874 2e75     text = text.u
-00012870: 7070 6572 2829 0a20 2020 2020 2020 2020  pper().         
-00012880: 2020 2020 2020 2020 2020 2023 2070 6f73             # pos
-00012890: 6974 696f 6e20 3d20 7365 6c66 2e6f 7468  ition = self.oth
-000128a0: 6572 5f31 2e63 7572 736f 7250 6f73 6974  er_1.cursorPosit
-000128b0: 696f 6e28 290a 2020 2020 2020 2020 2020  ion().          
-000128c0: 2020 2020 2020 2020 2020 7374 7269 7070            stripp
-000128d0: 6564 5f74 6578 7420 3d20 7465 7874 2e73  ed_text = text.s
-000128e0: 7472 6970 2829 2e72 6570 6c61 6365 2822  trip().replace("
-000128f0: 2022 2c20 2222 290a 2020 2020 2020 2020   ", "").        
-00012900: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00012910: 2e6f 7468 6572 5f31 2e73 6574 5465 7874  .other_1.setText
-00012920: 2873 7472 6970 7065 645f 7465 7874 290a  (stripped_text).
-00012930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012940: 2020 2020 2320 7365 6c66 2e6f 7468 6572      # self.other
-00012950: 5f31 2e73 6574 4375 7273 6f72 506f 7369  _1.setCursorPosi
-00012960: 7469 6f6e 2870 6f73 6974 696f 6e29 0a20  tion(position). 
-00012970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012980: 2020 2069 6620 2220 2220 696e 2074 6578     if " " in tex
-00012990: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-000129a0: 2020 2020 2020 2020 2020 206e 6578 745f             next_
-000129b0: 7461 6220 3d20 7365 6c66 2e74 6162 5f6e  tab = self.tab_n
-000129c0: 6578 742e 6765 7428 7365 6c66 2e6f 7468  ext.get(self.oth
-000129d0: 6572 5f31 290a 2020 2020 2020 2020 2020  er_1).          
-000129e0: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-000129f0: 7874 5f74 6162 2e73 6574 466f 6375 7328  xt_tab.setFocus(
-00012a00: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00012a10: 2020 2020 2020 2020 2020 6e65 7874 5f74            next_t
-00012a20: 6162 2e64 6573 656c 6563 7428 290a 2020  ab.deselect().  
-00012a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a40: 2020 2020 2020 6e65 7874 5f74 6162 2e65        next_tab.e
-00012a50: 6e64 2846 616c 7365 290a 0a20 2020 2064  nd(False)..    d
-00012a60: 6566 206f 7468 6572 5f32 5f63 6861 6e67  ef other_2_chang
-00012a70: 6564 2873 656c 6629 3a0a 2020 2020 2020  ed(self):.      
-00012a80: 2020 2222 2243 616c 6c65 6420 7768 656e    """Called when
-00012a90: 2077 6520 6e65 6564 2074 6f20 7061 7273   we need to pars
-00012aa0: 6520 5353 2065 7863 6861 6e67 652e 2222  e SS exchange.""
-00012ab0: 220a 2020 2020 2020 2020 6966 2073 656c  ".        if sel
-00012ac0: 662e 636f 6e74 6573 743a 0a20 2020 2020  f.contest:.     
-00012ad0: 2020 2020 2020 2069 6620 2241 5252 4c20         if "ARRL 
-00012ae0: 5377 6565 7073 7461 6b65 7322 2069 6e20  Sweepstakes" in 
-00012af0: 7365 6c66 2e63 6f6e 7465 7374 2e6e 616d  self.contest.nam
-00012b00: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00012b10: 2020 2073 656c 662e 636f 6e74 6573 742e     self.contest.
-00012b20: 7061 7273 655f 6578 6368 616e 6765 2873  parse_exchange(s
-00012b30: 656c 6629 0a20 2020 2020 2020 2020 2020  elf).           
-00012b40: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-00012b50: 2020 2020 2020 2020 6966 2068 6173 6174          if hasat
-00012b60: 7472 2873 656c 662e 636f 6e74 6573 742c  tr(self.contest,
-00012b70: 2022 6164 7661 6e63 655f 6f6e 5f73 7061   "advance_on_spa
-00012b80: 6365 2229 3a0a 2020 2020 2020 2020 2020  ce"):.          
-00012b90: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
-00012ba0: 6e74 6573 742e 6164 7661 6e63 655f 6f6e  ntest.advance_on
-00012bb0: 5f73 7061 6365 5b33 5d3a 0a20 2020 2020  _space[3]:.     
-00012bc0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00012bd0: 6578 7420 3d20 7365 6c66 2e6f 7468 6572  ext = self.other
-00012be0: 5f32 2e74 6578 7428 290a 2020 2020 2020  _2.text().      
-00012bf0: 2020 2020 2020 2020 2020 2020 2020 7465                te
-00012c00: 7874 203d 2074 6578 742e 7570 7065 7228  xt = text.upper(
-00012c10: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00012c20: 2020 2020 2020 2320 706f 7369 7469 6f6e        # position
-00012c30: 203d 2073 656c 662e 6f74 6865 725f 322e   = self.other_2.
-00012c40: 6375 7273 6f72 506f 7369 7469 6f6e 2829  cursorPosition()
-00012c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012c60: 2020 2020 2073 7472 6970 7065 645f 7465       stripped_te
-00012c70: 7874 203d 2074 6578 742e 7374 7269 7028  xt = text.strip(
-00012c80: 292e 7265 706c 6163 6528 2220 222c 2022  ).replace(" ", "
-00012c90: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00012ca0: 2020 2020 2020 2073 656c 662e 6f74 6865         self.othe
-00012cb0: 725f 322e 7365 7454 6578 7428 7374 7269  r_2.setText(stri
-00012cc0: 7070 6564 5f74 6578 7429 0a20 2020 2020  pped_text).     
-00012cd0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00012ce0: 2073 656c 662e 6f74 6865 725f 322e 7365   self.other_2.se
-00012cf0: 7443 7572 736f 7250 6f73 6974 696f 6e28  tCursorPosition(
-00012d00: 706f 7369 7469 6f6e 290a 2020 2020 2020  position).      
-00012d10: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00012d20: 2022 2022 2069 6e20 7465 7874 3a0a 2020   " " in text:.  
-00012d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d40: 2020 2020 2020 6e65 7874 5f74 6162 203d        next_tab =
-00012d50: 2073 656c 662e 7461 625f 6e65 7874 2e67   self.tab_next.g
-00012d60: 6574 2873 656c 662e 6f74 6865 725f 3229  et(self.other_2)
-00012d70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012d80: 2020 2020 2020 2020 206e 6578 745f 7461           next_ta
-00012d90: 622e 7365 7446 6f63 7573 2829 0a20 2020  b.setFocus().   
-00012da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012db0: 2020 2020 206e 6578 745f 7461 622e 6465       next_tab.de
-00012dc0: 7365 6c65 6374 2829 0a20 2020 2020 2020  select().       
+00011f50: 2061 6e64 206a 736f 6e5f 6461 7461 2e67   and json_data.g
+00011f60: 6574 2822 7374 6174 696f 6e22 2c20 2222  et("station", ""
+00011f70: 2920 3d3d 2070 6c61 7466 6f72 6d2e 6e6f  ) == platform.no
+00011f80: 6465 2829 0a20 2020 2020 2020 2020 2020  de().           
+00011f90: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
+00011fa0: 2020 2020 2020 2020 2020 2020 2320 6227              # b'
+00011fb0: 7b22 636d 6422 3a20 2254 554e 4522 2c20  {"cmd": "TUNE", 
+00011fc0: 2266 7265 7122 3a20 372e 3032 3335 2c20  "freq": 7.0235, 
+00011fd0: 2273 706f 7422 3a20 224d 4d30 4447 4922  "spot": "MM0DGI"
+00011fe0: 7d27 0a20 2020 2020 2020 2020 2020 2020  }'.             
+00011ff0: 2020 2020 2020 2076 666f 203d 206a 736f         vfo = jso
+00012000: 6e5f 6461 7461 2e67 6574 2822 6672 6571  n_data.get("freq
+00012010: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00012020: 2020 2020 2020 2076 666f 203d 2066 6c6f         vfo = flo
+00012030: 6174 2876 666f 2920 2a20 3130 3030 3030  at(vfo) * 100000
+00012040: 300a 2020 2020 2020 2020 2020 2020 2020  0.              
+00012050: 2020 2020 2020 7365 6c66 2e72 6164 696f        self.radio
+00012060: 5f73 7461 7465 5b22 7666 6f61 225d 203d  _state["vfoa"] =
+00012070: 2069 6e74 2876 666f 290a 2020 2020 2020   int(vfo).      
+00012080: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00012090: 2073 656c 662e 7269 675f 636f 6e74 726f   self.rig_contro
+000120a0: 6c3a 0a20 2020 2020 2020 2020 2020 2020  l:.             
+000120b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000120c0: 7269 675f 636f 6e74 726f 6c2e 7365 745f  rig_control.set_
+000120d0: 7666 6f28 696e 7428 7666 6f29 290a 2020  vfo(int(vfo)).  
+000120e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000120f0: 2020 7370 6f74 203d 206a 736f 6e5f 6461    spot = json_da
+00012100: 7461 2e67 6574 2822 7370 6f74 222c 2022  ta.get("spot", "
+00012110: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00012120: 2020 2020 2020 2073 656c 662e 6361 6c6c         self.call
+00012130: 7369 676e 2e73 6574 5465 7874 2873 706f  sign.setText(spo
+00012140: 7429 0a20 2020 2020 2020 2020 2020 2020  t).             
+00012150: 2020 2020 2020 2073 656c 662e 6361 6c6c         self.call
+00012160: 7369 676e 5f63 6861 6e67 6564 2829 0a20  sign_changed(). 
+00012170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012180: 2020 2073 656c 662e 6361 6c6c 7369 676e     self.callsign
+00012190: 2e73 6574 466f 6375 7328 290a 2020 2020  .setFocus().    
+000121a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000121b0: 7365 6c66 2e63 616c 6c73 6967 6e2e 6163  self.callsign.ac
+000121c0: 7469 7661 7465 5769 6e64 6f77 2829 0a20  tivateWindow(). 
+000121d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000121e0: 2020 2077 696e 646f 772e 7261 6973 655f     window.raise_
+000121f0: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
+00012200: 2020 2020 6966 2028 0a20 2020 2020 2020      if (.       
+00012210: 2020 2020 2020 2020 2020 2020 206a 736f               jso
+00012220: 6e5f 6461 7461 2e67 6574 2822 636d 6422  n_data.get("cmd"
+00012230: 2c20 2222 2920 3d3d 2022 4745 5457 4f52  , "") == "GETWOR
+00012240: 4b45 444c 4953 5422 0a20 2020 2020 2020  KEDLIST".       
+00012250: 2020 2020 2020 2020 2020 2020 2061 6e64               and
+00012260: 206a 736f 6e5f 6461 7461 2e67 6574 2822   json_data.get("
+00012270: 7374 6174 696f 6e22 2c20 2222 2920 3d3d  station", "") ==
+00012280: 2070 6c61 7466 6f72 6d2e 6e6f 6465 2829   platform.node()
+00012290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000122a0: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+000122b0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+000122c0: 2073 656c 662e 6461 7461 6261 7365 2e67   self.database.g
+000122d0: 6574 5f63 616c 6c73 5f61 6e64 5f62 616e  et_calls_and_ban
+000122e0: 6473 2829 0a20 2020 2020 2020 2020 2020  ds().           
+000122f0: 2020 2020 2020 2020 2063 6d64 203d 207b           cmd = {
+00012300: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00012310: 2020 2020 2020 636d 645b 2263 6d64 225d        cmd["cmd"]
+00012320: 203d 2022 574f 524b 4544 220a 2020 2020   = "WORKED".    
+00012330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012340: 636d 645b 2273 7461 7469 6f6e 225d 203d  cmd["station"] =
+00012350: 2070 6c61 7466 6f72 6d2e 6e6f 6465 2829   platform.node()
+00012360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012370: 2020 2020 2063 6d64 5b22 776f 726b 6564       cmd["worked
+00012380: 225d 203d 2072 6573 756c 740a 2020 2020  "] = result.    
+00012390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000123a0: 7365 6c66 2e6d 756c 7469 6361 7374 5f69  self.multicast_i
+000123b0: 6e74 6572 6661 6365 2e73 656e 645f 6173  nterface.send_as
+000123c0: 5f6a 736f 6e28 636d 6429 0a0a 2020 2020  _json(cmd)..    
+000123d0: 6465 6620 6377 5f6d 6163 726f 735f 7374  def cw_macros_st
+000123e0: 6174 655f 6368 616e 6765 6428 7365 6c66  ate_changed(self
+000123f0: 293a 0a20 2020 2020 2020 2022 2222 4d65  ):.        """Me
+00012400: 6e75 2069 7465 6d20 746f 2073 686f 772f  nu item to show/
+00012410: 6869 6465 206d 6163 726f 2062 7574 746f  hide macro butto
+00012420: 6e73 2222 220a 2020 2020 2020 2020 7365  ns""".        se
+00012430: 6c66 2e70 7265 665b 2263 775f 6d61 6372  lf.pref["cw_macr
+00012440: 6f73 225d 203d 2073 656c 662e 6163 7469  os"] = self.acti
+00012450: 6f6e 4357 5f4d 6163 726f 732e 6973 4368  onCW_Macros.isCh
+00012460: 6563 6b65 6428 290a 2020 2020 2020 2020  ecked().        
+00012470: 7365 6c66 2e77 7269 7465 5f70 7265 6665  self.write_prefe
+00012480: 7265 6e63 6528 290a 2020 2020 2020 2020  rence().        
+00012490: 7365 6c66 2e73 686f 775f 4357 5f6d 6163  self.show_CW_mac
+000124a0: 726f 7328 290a 0a20 2020 2064 6566 2073  ros()..    def s
+000124b0: 686f 775f 4357 5f6d 6163 726f 7328 7365  how_CW_macros(se
+000124c0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+000124d0: 6d61 6372 6f20 6275 7474 6f6e 2073 7461  macro button sta
+000124e0: 7465 2063 6861 6e67 6522 2222 0a20 2020  te change""".   
+000124f0: 2020 2020 2069 6620 7365 6c66 2e70 7265       if self.pre
+00012500: 662e 6765 7428 2263 775f 6d61 6372 6f73  f.get("cw_macros
+00012510: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+00012520: 7365 6c66 2e42 7574 746f 6e5f 526f 7731  self.Button_Row1
+00012530: 2e73 686f 7728 290a 2020 2020 2020 2020  .show().        
+00012540: 2020 2020 7365 6c66 2e42 7574 746f 6e5f      self.Button_
+00012550: 526f 7732 2e73 686f 7728 290a 2020 2020  Row2.show().    
+00012560: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00012570: 2020 2020 2020 7365 6c66 2e42 7574 746f        self.Butto
+00012580: 6e5f 526f 7731 2e68 6964 6528 290a 2020  n_Row1.hide().  
+00012590: 2020 2020 2020 2020 2020 7365 6c66 2e42            self.B
+000125a0: 7574 746f 6e5f 526f 7732 2e68 6964 6528  utton_Row2.hide(
+000125b0: 290a 0a20 2020 2064 6566 2063 6f6d 6d61  )..    def comma
+000125c0: 6e64 5f62 7574 746f 6e73 5f73 7461 7465  nd_buttons_state
+000125d0: 5f63 6861 6e67 6528 7365 6c66 293a 0a20  _change(self):. 
+000125e0: 2020 2020 2020 2022 2222 4d65 6e75 2069         """Menu i
+000125f0: 7465 6d20 746f 2073 686f 772f 6869 6465  tem to show/hide
+00012600: 2063 6f6d 6d61 6e64 2062 7574 746f 6e73   command buttons
+00012610: 2222 220a 2020 2020 2020 2020 7365 6c66  """.        self
+00012620: 2e70 7265 665b 2263 6f6d 6d61 6e64 5f62  .pref["command_b
+00012630: 7574 746f 6e73 225d 203d 2073 656c 662e  uttons"] = self.
+00012640: 6163 7469 6f6e 436f 6d6d 616e 645f 4275  actionCommand_Bu
+00012650: 7474 6f6e 732e 6973 4368 6563 6b65 6428  ttons.isChecked(
+00012660: 290a 2020 2020 2020 2020 7365 6c66 2e77  ).        self.w
+00012670: 7269 7465 5f70 7265 6665 7265 6e63 6528  rite_preference(
+00012680: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+00012690: 686f 775f 636f 6d6d 616e 645f 6275 7474  how_command_butt
+000126a0: 6f6e 7328 290a 0a20 2020 2064 6566 2073  ons()..    def s
+000126b0: 686f 775f 636f 6d6d 616e 645f 6275 7474  how_command_butt
+000126c0: 6f6e 7328 7365 6c66 293a 0a20 2020 2020  ons(self):.     
+000126d0: 2020 2022 2222 636f 6d6d 616e 6420 6275     """command bu
+000126e0: 7474 6f6e 2073 7461 7465 2063 6861 6e67  tton state chang
+000126f0: 6522 2222 0a20 2020 2020 2020 2069 6620  e""".        if 
+00012700: 7365 6c66 2e70 7265 662e 6765 7428 2263  self.pref.get("c
+00012710: 6f6d 6d61 6e64 5f62 7574 746f 6e73 2229  ommand_buttons")
+00012720: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00012730: 6c66 2e43 6f6d 6d61 6e64 5f42 7574 746f  lf.Command_Butto
+00012740: 6e73 2e73 686f 7728 290a 2020 2020 2020  ns.show().      
+00012750: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00012760: 2020 2020 7365 6c66 2e43 6f6d 6d61 6e64      self.Command
+00012770: 5f42 7574 746f 6e73 2e68 6964 6528 290a  _Buttons.hide().
+00012780: 0a20 2020 2064 6566 2069 735f 666c 6f61  .    def is_floa
+00012790: 7461 626c 6528 7365 6c66 2c20 6974 656d  table(self, item
+000127a0: 3a20 7374 7229 202d 3e20 626f 6f6c 3a0a  : str) -> bool:.
+000127b0: 2020 2020 2020 2020 2222 2263 6865 636b          """check
+000127c0: 2074 6f20 7365 6520 6966 2073 7472 696e   to see if strin
+000127d0: 6720 6361 6e20 6265 2061 2066 6c6f 6174  g can be a float
+000127e0: 2222 220a 2020 2020 2020 2020 6966 2069  """.        if i
+000127f0: 7465 6d2e 6973 6e75 6d65 7269 6328 293a  tem.isnumeric():
+00012800: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00012810: 7572 6e20 5472 7565 0a20 2020 2020 2020  urn True.       
+00012820: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00012830: 2020 5f74 6573 7420 3d20 666c 6f61 7428    _test = float(
+00012840: 6974 656d 290a 2020 2020 2020 2020 6578  item).        ex
+00012850: 6365 7074 2056 616c 7565 4572 726f 723a  cept ValueError:
+00012860: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00012870: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
+00012880: 2020 7265 7475 726e 2054 7275 650a 0a20    return True.. 
+00012890: 2020 2064 6566 206f 7468 6572 5f31 5f63     def other_1_c
+000128a0: 6861 6e67 6564 2873 656c 6629 3a0a 2020  hanged(self):.  
+000128b0: 2020 2020 2020 2222 2243 616c 6c65 6420        """Called 
+000128c0: 7768 656e 2e2e 2e20 796f 7520 6b6e 6f77  when... you know
+000128d0: 2e22 2222 0a20 2020 2020 2020 2069 6620  .""".        if 
+000128e0: 7365 6c66 2e63 6f6e 7465 7374 3a0a 2020  self.contest:.  
+000128f0: 2020 2020 2020 2020 2020 6966 2068 6173            if has
+00012900: 6174 7472 2873 656c 662e 636f 6e74 6573  attr(self.contes
+00012910: 742c 2022 6164 7661 6e63 655f 6f6e 5f73  t, "advance_on_s
+00012920: 7061 6365 2229 3a0a 2020 2020 2020 2020  pace"):.        
+00012930: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00012940: 636f 6e74 6573 742e 6164 7661 6e63 655f  contest.advance_
+00012950: 6f6e 5f73 7061 6365 5b33 5d3a 0a20 2020  on_space[3]:.   
+00012960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012970: 2074 6578 7420 3d20 7365 6c66 2e6f 7468   text = self.oth
+00012980: 6572 5f31 2e74 6578 7428 290a 2020 2020  er_1.text().    
+00012990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000129a0: 7465 7874 203d 2074 6578 742e 7570 7065  text = text.uppe
+000129b0: 7228 290a 2020 2020 2020 2020 2020 2020  r().            
+000129c0: 2020 2020 2020 2020 2320 706f 7369 7469          # positi
+000129d0: 6f6e 203d 2073 656c 662e 6f74 6865 725f  on = self.other_
+000129e0: 312e 6375 7273 6f72 506f 7369 7469 6f6e  1.cursorPosition
+000129f0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00012a00: 2020 2020 2020 2073 7472 6970 7065 645f         stripped_
+00012a10: 7465 7874 203d 2074 6578 742e 7374 7269  text = text.stri
+00012a20: 7028 292e 7265 706c 6163 6528 2220 222c  p().replace(" ",
+00012a30: 2022 2229 0a20 2020 2020 2020 2020 2020   "").           
+00012a40: 2020 2020 2020 2020 2073 656c 662e 6f74           self.ot
+00012a50: 6865 725f 312e 7365 7454 6578 7428 7374  her_1.setText(st
+00012a60: 7269 7070 6564 5f74 6578 7429 0a20 2020  ripped_text).   
+00012a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a80: 2023 2073 656c 662e 6f74 6865 725f 312e   # self.other_1.
+00012a90: 7365 7443 7572 736f 7250 6f73 6974 696f  setCursorPositio
+00012aa0: 6e28 706f 7369 7469 6f6e 290a 2020 2020  n(position).    
+00012ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ac0: 6966 2022 2022 2069 6e20 7465 7874 3a0a  if " " in text:.
+00012ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ae0: 2020 2020 2020 2020 6e65 7874 5f74 6162          next_tab
+00012af0: 203d 2073 656c 662e 7461 625f 6e65 7874   = self.tab_next
+00012b00: 2e67 6574 2873 656c 662e 6f74 6865 725f  .get(self.other_
+00012b10: 3129 0a20 2020 2020 2020 2020 2020 2020  1).             
+00012b20: 2020 2020 2020 2020 2020 206e 6578 745f             next_
+00012b30: 7461 622e 7365 7446 6f63 7573 2829 0a20  tab.setFocus(). 
+00012b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b50: 2020 2020 2020 206e 6578 745f 7461 622e         next_tab.
+00012b60: 6465 7365 6c65 6374 2829 0a20 2020 2020  deselect().     
+00012b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b80: 2020 206e 6578 745f 7461 622e 656e 6428     next_tab.end(
+00012b90: 4661 6c73 6529 0a0a 2020 2020 6465 6620  False)..    def 
+00012ba0: 6f74 6865 725f 325f 6368 616e 6765 6428  other_2_changed(
+00012bb0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+00012bc0: 2222 4361 6c6c 6564 2077 6865 6e20 7765  ""Called when we
+00012bd0: 206e 6565 6420 746f 2070 6172 7365 2053   need to parse S
+00012be0: 5320 6578 6368 616e 6765 2e22 2222 0a20  S exchange.""". 
+00012bf0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+00012c00: 6f6e 7465 7374 3a0a 2020 2020 2020 2020  ontest:.        
+00012c10: 2020 2020 6966 2022 4152 524c 2053 7765      if "ARRL Swe
+00012c20: 6570 7374 616b 6573 2220 696e 2073 656c  epstakes" in sel
+00012c30: 662e 636f 6e74 6573 742e 6e61 6d65 3a0a  f.contest.name:.
+00012c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c50: 7365 6c66 2e63 6f6e 7465 7374 2e70 6172  self.contest.par
+00012c60: 7365 5f65 7863 6861 6e67 6528 7365 6c66  se_exchange(self
+00012c70: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00012c80: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+00012c90: 2020 2020 2069 6620 6861 7361 7474 7228       if hasattr(
+00012ca0: 7365 6c66 2e63 6f6e 7465 7374 2c20 2261  self.contest, "a
+00012cb0: 6476 616e 6365 5f6f 6e5f 7370 6163 6522  dvance_on_space"
+00012cc0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00012cd0: 2020 2069 6620 7365 6c66 2e63 6f6e 7465     if self.conte
+00012ce0: 7374 2e61 6476 616e 6365 5f6f 6e5f 7370  st.advance_on_sp
+00012cf0: 6163 655b 335d 3a0a 2020 2020 2020 2020  ace[3]:.        
+00012d00: 2020 2020 2020 2020 2020 2020 7465 7874              text
+00012d10: 203d 2073 656c 662e 6f74 6865 725f 322e   = self.other_2.
+00012d20: 7465 7874 2829 0a20 2020 2020 2020 2020  text().         
+00012d30: 2020 2020 2020 2020 2020 2074 6578 7420             text 
+00012d40: 3d20 7465 7874 2e75 7070 6572 2829 0a20  = text.upper(). 
+00012d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d60: 2020 2023 2070 6f73 6974 696f 6e20 3d20     # position = 
+00012d70: 7365 6c66 2e6f 7468 6572 5f32 2e63 7572  self.other_2.cur
+00012d80: 736f 7250 6f73 6974 696f 6e28 290a 2020  sorPosition().  
+00012d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012da0: 2020 7374 7269 7070 6564 5f74 6578 7420    stripped_text 
+00012db0: 3d20 7465 7874 2e73 7472 6970 2829 2e72  = text.strip().r
+00012dc0: 6570 6c61 6365 2822 2022 2c20 2222 290a  eplace(" ", "").
 00012dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012de0: 206e 6578 745f 7461 622e 656e 6428 4661   next_tab.end(Fa
-00012df0: 6c73 6529 0a0a 2020 2020 6465 6620 6361  lse)..    def ca
-00012e00: 6c6c 7369 676e 5f63 6861 6e67 6564 2873  llsign_changed(s
-00012e10: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-00012e20: 2243 616c 6c65 6420 7768 656e 2074 6578  "Called when tex
-00012e30: 7420 696e 2074 6865 2063 616c 6c73 6967  t in the callsig
-00012e40: 6e20 6669 656c 6420 6861 7320 6368 616e  n field has chan
-00012e50: 6765 6422 2222 0a20 2020 2020 2020 2074  ged""".        t
-00012e60: 6578 7420 3d20 7365 6c66 2e63 616c 6c73  ext = self.calls
-00012e70: 6967 6e2e 7465 7874 2829 0a20 2020 2020  ign.text().     
-00012e80: 2020 2074 6578 7420 3d20 7465 7874 2e75     text = text.u
-00012e90: 7070 6572 2829 0a20 2020 2020 2020 2070  pper().        p
-00012ea0: 6f73 6974 696f 6e20 3d20 7365 6c66 2e63  osition = self.c
-00012eb0: 616c 6c73 6967 6e2e 6375 7273 6f72 506f  allsign.cursorPo
-00012ec0: 7369 7469 6f6e 2829 0a20 2020 2020 2020  sition().       
-00012ed0: 2073 7472 6970 7065 645f 7465 7874 203d   stripped_text =
-00012ee0: 2074 6578 742e 7374 7269 7028 292e 7265   text.strip().re
-00012ef0: 706c 6163 6528 2220 222c 2022 2229 0a20  place(" ", ""). 
-00012f00: 2020 2020 2020 2073 656c 662e 6361 6c6c         self.call
-00012f10: 7369 676e 2e73 6574 5465 7874 2873 7472  sign.setText(str
-00012f20: 6970 7065 645f 7465 7874 290a 2020 2020  ipped_text).    
-00012f30: 2020 2020 7365 6c66 2e63 616c 6c73 6967      self.callsig
-00012f40: 6e2e 7365 7443 7572 736f 7250 6f73 6974  n.setCursorPosit
-00012f50: 696f 6e28 706f 7369 7469 6f6e 290a 2020  ion(position).  
-00012f60: 2020 2020 2020 7265 7375 6c74 7320 3d20        results = 
-00012f70: 7365 6c66 2e6d 7363 702e 7375 7065 725f  self.mscp.super_
-00012f80: 6368 6563 6b28 7374 7269 7070 6564 5f74  check(stripped_t
-00012f90: 6578 7429 0a20 2020 2020 2020 206c 6f67  ext).        log
-00012fa0: 6765 722e 6465 6275 6728 6622 7b72 6573  ger.debug(f"{res
-00012fb0: 756c 7473 7d22 290a 0a20 2020 2020 2020  ults}")..       
-00012fc0: 2069 6620 2220 2220 696e 2074 6578 743a   if " " in text:
-00012fd0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00012fe0: 7374 7269 7070 6564 5f74 6578 7420 3d3d  stripped_text ==
-00012ff0: 2022 4357 223a 0a20 2020 2020 2020 2020   "CW":.         
-00013000: 2020 2020 2020 2073 656c 662e 7365 746d         self.setm
-00013010: 6f64 6528 2243 5722 290a 2020 2020 2020  ode("CW").      
-00013020: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-00013030: 6164 696f 5f73 7461 7465 5b22 6d6f 6465  adio_state["mode
-00013040: 225d 203d 2022 4357 220a 2020 2020 2020  "] = "CW".      
-00013050: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00013060: 662e 7269 675f 636f 6e74 726f 6c3a 0a20  f.rig_control:. 
-00013070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013080: 2020 2069 6620 7365 6c66 2e72 6967 5f63     if self.rig_c
-00013090: 6f6e 7472 6f6c 2e6f 6e6c 696e 653a 0a20  ontrol.online:. 
-000130a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000130b0: 2020 2020 2020 2073 656c 662e 7269 675f         self.rig_
-000130c0: 636f 6e74 726f 6c2e 7365 745f 6d6f 6465  control.set_mode
-000130d0: 2822 4357 2229 0a20 2020 2020 2020 2020  ("CW").         
-000130e0: 2020 2020 2020 2062 616e 6420 3d20 6765         band = ge
-000130f0: 7462 616e 6428 7374 7228 7365 6c66 2e72  tband(str(self.r
-00013100: 6164 696f 5f73 7461 7465 2e67 6574 2822  adio_state.get("
-00013110: 7666 6f61 222c 2022 302e 3022 2929 290a  vfoa", "0.0"))).
-00013120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013130: 7365 6c66 2e73 6574 5f62 616e 645f 696e  self.set_band_in
-00013140: 6469 6361 746f 7228 6261 6e64 290a 2020  dicator(band).  
-00013150: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00013160: 6c66 2e73 6574 5f77 696e 646f 775f 7469  lf.set_window_ti
-00013170: 746c 6528 290a 2020 2020 2020 2020 2020  tle().          
-00013180: 2020 2020 2020 7365 6c66 2e63 6c65 6172        self.clear
-00013190: 696e 7075 7473 2829 0a20 2020 2020 2020  inputs().       
-000131a0: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-000131b0: 6164 5f63 775f 6d61 6372 6f73 2829 0a20  ad_cw_macros(). 
-000131c0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000131d0: 6574 7572 6e0a 2020 2020 2020 2020 2020  eturn.          
-000131e0: 2020 6966 2073 7472 6970 7065 645f 7465    if stripped_te
-000131f0: 7874 203d 3d20 2252 5454 5922 3a0a 2020  xt == "RTTY":.  
-00013200: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00013210: 6c66 2e73 6574 6d6f 6465 2822 5254 5459  lf.setmode("RTTY
-00013220: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00013230: 2020 2069 6620 7365 6c66 2e72 6967 5f63     if self.rig_c
-00013240: 6f6e 7472 6f6c 3a0a 2020 2020 2020 2020  ontrol:.        
-00013250: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00013260: 656c 662e 7269 675f 636f 6e74 726f 6c2e  elf.rig_control.
-00013270: 6f6e 6c69 6e65 3a0a 2020 2020 2020 2020  online:.        
-00013280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013290: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
-000132a0: 2e73 6574 5f6d 6f64 6528 2252 5454 5922  .set_mode("RTTY"
-000132b0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000132c0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000132d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000132e0: 2020 2020 7365 6c66 2e72 6164 696f 5f73      self.radio_s
-000132f0: 7461 7465 5b22 6d6f 6465 225d 203d 2022  tate["mode"] = "
-00013300: 5254 5459 220a 2020 2020 2020 2020 2020  RTTY".          
-00013310: 2020 2020 2020 6261 6e64 203d 2067 6574        band = get
-00013320: 6261 6e64 2873 7472 2873 656c 662e 7261  band(str(self.ra
-00013330: 6469 6f5f 7374 6174 652e 6765 7428 2276  dio_state.get("v
-00013340: 666f 6122 2c20 2230 2e30 2229 2929 0a20  foa", "0.0"))). 
-00013350: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00013360: 656c 662e 7365 745f 6261 6e64 5f69 6e64  elf.set_band_ind
-00013370: 6963 6174 6f72 2862 616e 6429 0a20 2020  icator(band).   
-00013380: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00013390: 662e 7365 745f 7769 6e64 6f77 5f74 6974  f.set_window_tit
-000133a0: 6c65 2829 0a20 2020 2020 2020 2020 2020  le().           
-000133b0: 2020 2020 2073 656c 662e 636c 6561 7269       self.cleari
-000133c0: 6e70 7574 7328 290a 2020 2020 2020 2020  nputs().        
-000133d0: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-000133e0: 2020 2020 2020 2020 2020 2069 6620 7374             if st
-000133f0: 7269 7070 6564 5f74 6578 7420 3d3d 2022  ripped_text == "
-00013400: 5353 4222 3a0a 2020 2020 2020 2020 2020  SSB":.          
-00013410: 2020 2020 2020 7365 6c66 2e73 6574 6d6f        self.setmo
-00013420: 6465 2822 5353 4222 290a 2020 2020 2020  de("SSB").      
-00013430: 2020 2020 2020 2020 2020 6966 2069 6e74            if int
-00013440: 2873 656c 662e 7261 6469 6f5f 7374 6174  (self.radio_stat
-00013450: 652e 6765 7428 2276 666f 6122 2c20 3029  e.get("vfoa", 0)
-00013460: 2920 3e20 3130 3030 3030 3030 3a0a 2020  ) > 10000000:.  
-00013470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013480: 2020 7365 6c66 2e72 6164 696f 5f73 7461    self.radio_sta
-00013490: 7465 5b22 6d6f 6465 225d 203d 2022 5553  te["mode"] = "US
-000134a0: 4222 0a20 2020 2020 2020 2020 2020 2020  B".             
-000134b0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000134c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000134d0: 662e 7261 6469 6f5f 7374 6174 655b 226d  f.radio_state["m
-000134e0: 6f64 6522 5d20 3d20 224c 5342 220a 2020  ode"] = "LSB".  
-000134f0: 2020 2020 2020 2020 2020 2020 2020 6261                ba
-00013500: 6e64 203d 2067 6574 6261 6e64 2873 7472  nd = getband(str
-00013510: 2873 656c 662e 7261 6469 6f5f 7374 6174  (self.radio_stat
-00013520: 652e 6765 7428 2276 666f 6122 2c20 2230  e.get("vfoa", "0
-00013530: 2e30 2229 2929 0a20 2020 2020 2020 2020  .0"))).         
-00013540: 2020 2020 2020 2073 656c 662e 7365 745f         self.set_
-00013550: 6261 6e64 5f69 6e64 6963 6174 6f72 2862  band_indicator(b
-00013560: 616e 6429 0a20 2020 2020 2020 2020 2020  and).           
-00013570: 2020 2020 2073 656c 662e 7365 745f 7769       self.set_wi
-00013580: 6e64 6f77 5f74 6974 6c65 2829 0a20 2020  ndow_title().   
-00013590: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000135a0: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
-000135b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000135c0: 2020 2020 2020 7365 6c66 2e72 6967 5f63        self.rig_c
-000135d0: 6f6e 7472 6f6c 2e73 6574 5f6d 6f64 6528  ontrol.set_mode(
-000135e0: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
-000135f0: 2e67 6574 2822 6d6f 6465 2229 290a 2020  .get("mode")).  
-00013600: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00013610: 6c66 2e63 6c65 6172 696e 7075 7473 2829  lf.clearinputs()
-00013620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013630: 2073 656c 662e 7265 6164 5f63 775f 6d61   self.read_cw_ma
-00013640: 6372 6f73 2829 0a20 2020 2020 2020 2020  cros().         
-00013650: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-00013660: 2020 2020 2020 2020 2020 6966 2073 7472            if str
-00013670: 6970 7065 645f 7465 7874 203d 3d20 224f  ipped_text == "O
-00013680: 504f 4e22 3a0a 2020 2020 2020 2020 2020  PON":.          
-00013690: 2020 2020 2020 7365 6c66 2e67 6574 5f6f        self.get_o
-000136a0: 706f 6e28 290a 2020 2020 2020 2020 2020  pon().          
-000136b0: 2020 2020 2020 7365 6c66 2e63 6c65 6172        self.clear
-000136c0: 696e 7075 7473 2829 0a20 2020 2020 2020  inputs().       
-000136d0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-000136e0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-000136f0: 7472 6970 7065 645f 7465 7874 203d 3d20  tripped_text == 
-00013700: 2248 454c 5022 3a0a 2020 2020 2020 2020  "HELP":.        
-00013710: 2020 2020 2020 2020 7365 6c66 2e73 686f          self.sho
-00013720: 775f 6865 6c70 5f64 6961 6c6f 6728 290a  w_help_dialog().
-00013730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013740: 7365 6c66 2e63 6c65 6172 696e 7075 7473  self.clearinputs
-00013750: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00013760: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-00013770: 2020 2020 2020 6966 2073 7472 6970 7065        if strippe
-00013780: 645f 7465 7874 203d 3d20 2254 4553 5422  d_text == "TEST"
-00013790: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000137a0: 2020 7265 7375 6c74 203d 2073 656c 662e    result = self.
-000137b0: 6461 7461 6261 7365 2e67 6574 5f63 616c  database.get_cal
-000137c0: 6c73 5f61 6e64 5f62 616e 6473 2829 0a20  ls_and_bands(). 
-000137d0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000137e0: 6d64 203d 207b 7d0a 2020 2020 2020 2020  md = {}.        
-000137f0: 2020 2020 2020 2020 636d 645b 2263 6d64          cmd["cmd
-00013800: 225d 203d 2022 574f 524b 4544 220a 2020  "] = "WORKED".  
-00013810: 2020 2020 2020 2020 2020 2020 2020 636d                cm
-00013820: 645b 2273 7461 7469 6f6e 225d 203d 2070  d["station"] = p
-00013830: 6c61 7466 6f72 6d2e 6e6f 6465 2829 0a20  latform.node(). 
-00013840: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00013850: 6d64 5b22 776f 726b 6564 225d 203d 2072  md["worked"] = r
-00013860: 6573 756c 740a 2020 2020 2020 2020 2020  esult.          
-00013870: 2020 2020 2020 7365 6c66 2e6d 756c 7469        self.multi
-00013880: 6361 7374 5f69 6e74 6572 6661 6365 2e73  cast_interface.s
-00013890: 656e 645f 6173 5f6a 736f 6e28 636d 6429  end_as_json(cmd)
-000138a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000138b0: 2073 656c 662e 636c 6561 7269 6e70 7574   self.clearinput
-000138c0: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
-000138d0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-000138e0: 2020 2020 2020 2069 6620 7365 6c66 2e69         if self.i
-000138f0: 735f 666c 6f61 7461 626c 6528 7374 7269  s_floatable(stri
-00013900: 7070 6564 5f74 6578 7429 3a0a 2020 2020  pped_text):.    
-00013910: 2020 2020 2020 2020 2020 2020 7666 6f20              vfo 
-00013920: 3d20 666c 6f61 7428 7374 7269 7070 6564  = float(stripped
-00013930: 5f74 6578 7429 0a20 2020 2020 2020 2020  _text).         
-00013940: 2020 2020 2020 2076 666f 203d 2069 6e74         vfo = int
-00013950: 2876 666f 202a 2031 3030 3029 0a20 2020  (vfo * 1000).   
-00013960: 2020 2020 2020 2020 2020 2020 2062 616e               ban
-00013970: 6420 3d20 6765 7462 616e 6428 7374 7228  d = getband(str(
-00013980: 7666 6f29 290a 2020 2020 2020 2020 2020  vfo)).          
-00013990: 2020 2020 2020 7365 6c66 2e73 6574 5f62        self.set_b
-000139a0: 616e 645f 696e 6469 6361 746f 7228 6261  and_indicator(ba
-000139b0: 6e64 290a 2020 2020 2020 2020 2020 2020  nd).            
-000139c0: 2020 2020 2320 7365 6c66 2e63 6f6e 7461      # self.conta
-000139d0: 6374 5b22 4261 6e64 225d 203d 2067 6574  ct["Band"] = get
-000139e0: 5f6c 6f67 6765 645f 6261 6e64 2873 7472  _logged_band(str
-000139f0: 2873 656c 662e 7261 6469 6f5f 7374 6174  (self.radio_stat
-00013a00: 652e 6765 7428 2276 666f 6122 2c20 302e  e.get("vfoa", 0.
-00013a10: 3029 2929 0a20 2020 2020 2020 2020 2020  0))).           
-00013a20: 2020 2020 2073 656c 662e 7261 6469 6f5f       self.radio_
-00013a30: 7374 6174 655b 2276 666f 6122 5d20 3d20  state["vfoa"] = 
-00013a40: 7666 6f0a 2020 2020 2020 2020 2020 2020  vfo.            
-00013a50: 2020 2020 7365 6c66 2e72 6164 696f 5f73      self.radio_s
-00013a60: 7461 7465 5b22 6261 6e64 225d 203d 2062  tate["band"] = b
-00013a70: 616e 640a 2020 2020 2020 2020 2020 2020  and.            
-00013a80: 2020 2020 7365 6c66 2e63 6f6e 7461 6374      self.contact
-00013a90: 5b22 4261 6e64 225d 203d 2067 6574 5f6c  ["Band"] = get_l
-00013aa0: 6f67 6765 645f 6261 6e64 2873 7472 2876  ogged_band(str(v
-00013ab0: 666f 2929 0a20 2020 2020 2020 2020 2020  fo)).           
-00013ac0: 2020 2020 2073 656c 662e 7365 745f 7769       self.set_wi
-00013ad0: 6e64 6f77 5f74 6974 6c65 2829 0a20 2020  ndow_title().   
-00013ae0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00013af0: 662e 636c 6561 7269 6e70 7574 7328 290a  f.clearinputs().
-00013b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b10: 6966 2073 656c 662e 7269 675f 636f 6e74  if self.rig_cont
-00013b20: 726f 6c3a 0a20 2020 2020 2020 2020 2020  rol:.           
-00013b30: 2020 2020 2020 2020 2073 656c 662e 7269           self.ri
-00013b40: 675f 636f 6e74 726f 6c2e 7365 745f 7666  g_control.set_vf
-00013b50: 6f28 7666 6f29 0a20 2020 2020 2020 2020  o(vfo).         
-00013b60: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00013b70: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-00013b80: 2020 636d 6420 3d20 7b7d 0a20 2020 2020    cmd = {}.     
-00013b90: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
-00013ba0: 636d 6422 5d20 3d20 2252 4144 494f 5f53  cmd"] = "RADIO_S
-00013bb0: 5441 5445 220a 2020 2020 2020 2020 2020  TATE".          
-00013bc0: 2020 2020 2020 636d 645b 2273 7461 7469        cmd["stati
-00013bd0: 6f6e 225d 203d 2070 6c61 7466 6f72 6d2e  on"] = platform.
-00013be0: 6e6f 6465 2829 0a20 2020 2020 2020 2020  node().         
-00013bf0: 2020 2020 2020 2063 6d64 5b22 6261 6e64         cmd["band
-00013c00: 225d 203d 2062 616e 640a 2020 2020 2020  "] = band.      
-00013c10: 2020 2020 2020 2020 2020 636d 645b 2276            cmd["v
-00013c20: 666f 6122 5d20 3d20 7666 6f0a 2020 2020  foa"] = vfo.    
-00013c30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00013c40: 2e6d 756c 7469 6361 7374 5f69 6e74 6572  .multicast_inter
-00013c50: 6661 6365 2e73 656e 645f 6173 5f6a 736f  face.send_as_jso
-00013c60: 6e28 636d 6429 0a20 2020 2020 2020 2020  n(cmd).         
-00013c70: 2020 2020 2020 2072 6574 7572 6e0a 0a20         return.. 
-00013c80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00013c90: 6368 6563 6b5f 6361 6c6c 7369 676e 2873  check_callsign(s
-00013ca0: 7472 6970 7065 645f 7465 7874 290a 2020  tripped_text).  
-00013cb0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00013cc0: 662e 6368 6563 6b5f 6475 7065 2873 7472  f.check_dupe(str
-00013cd0: 6970 7065 645f 7465 7874 293a 0a20 2020  ipped_text):.   
-00013ce0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00013cf0: 662e 6475 7065 5f69 6e64 6963 6174 6f72  f.dupe_indicator
-00013d00: 2e73 686f 7728 290a 2020 2020 2020 2020  .show().        
-00013d10: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00013d20: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-00013d30: 7570 655f 696e 6469 6361 746f 722e 6869  upe_indicator.hi
-00013d40: 6465 2829 0a20 2020 2020 2020 2020 2020  de().           
-00013d50: 205f 7468 6574 6872 6561 6420 3d20 7468   _thethread = th
-00013d60: 7265 6164 696e 672e 5468 7265 6164 280a  reading.Thread(.
-00013d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d80: 7461 7267 6574 3d73 656c 662e 6368 6563  target=self.chec
-00013d90: 6b5f 6361 6c6c 7369 676e 322c 0a20 2020  k_callsign2,.   
-00013da0: 2020 2020 2020 2020 2020 2020 2061 7267               arg
-00013db0: 733d 2874 6578 742c 292c 0a20 2020 2020  s=(text,),.     
-00013dc0: 2020 2020 2020 2020 2020 2064 6165 6d6f             daemo
-00013dd0: 6e3d 5472 7565 2c0a 2020 2020 2020 2020  n=True,.        
-00013de0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00013df0: 2020 5f74 6865 7468 7265 6164 2e73 7461    _thethread.sta
-00013e00: 7274 2829 0a20 2020 2020 2020 2020 2020  rt().           
-00013e10: 2073 656c 662e 6e65 7874 5f66 6965 6c64   self.next_field
-00013e20: 2e73 6574 466f 6375 7328 290a 2020 2020  .setFocus().    
-00013e30: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-00013e40: 2020 2020 2020 2063 6d64 203d 207b 7d0a         cmd = {}.
-00013e50: 2020 2020 2020 2020 636d 645b 2263 6d64          cmd["cmd
-00013e60: 225d 203d 2022 4341 4c4c 4348 414e 4745  "] = "CALLCHANGE
-00013e70: 4422 0a20 2020 2020 2020 2063 6d64 5b22  D".        cmd["
-00013e80: 7374 6174 696f 6e22 5d20 3d20 706c 6174  station"] = plat
-00013e90: 666f 726d 2e6e 6f64 6528 290a 2020 2020  form.node().    
-00013ea0: 2020 2020 636d 645b 2263 616c 6c22 5d20      cmd["call"] 
-00013eb0: 3d20 7374 7269 7070 6564 5f74 6578 740a  = stripped_text.
-00013ec0: 2020 2020 2020 2020 7365 6c66 2e6d 756c          self.mul
-00013ed0: 7469 6361 7374 5f69 6e74 6572 6661 6365  ticast_interface
-00013ee0: 2e73 656e 645f 6173 5f6a 736f 6e28 636d  .send_as_json(cm
-00013ef0: 6429 0a20 2020 2020 2020 2073 656c 662e  d).        self.
-00013f00: 6368 6563 6b5f 6361 6c6c 7369 676e 2873  check_callsign(s
-00013f10: 7472 6970 7065 645f 7465 7874 290a 0a20  tripped_text).. 
-00013f20: 2020 2064 6566 2063 6865 636b 5f63 616c     def check_cal
-00013f30: 6c73 6967 6e28 7365 6c66 2c20 6361 6c6c  lsign(self, call
-00013f40: 7369 676e 293a 0a20 2020 2020 2020 2022  sign):.        "
-00013f50: 2222 4368 6563 6b20 6361 6c6c 2061 7320  ""Check call as 
-00013f60: 656e 7465 7265 6422 2222 0a20 2020 2020  entered""".     
-00013f70: 2020 2072 6573 756c 7420 3d20 7365 6c66     result = self
-00013f80: 2e63 7479 5f6c 6f6f 6b75 7028 6361 6c6c  .cty_lookup(call
-00013f90: 7369 676e 290a 2020 2020 2020 2020 6465  sign).        de
-00013fa0: 6275 675f 7265 7375 6c74 203d 2066 227b  bug_result = f"{
-00013fb0: 7265 7375 6c74 7d22 0a20 2020 2020 2020  result}".       
-00013fc0: 206c 6f67 6765 722e 6465 6275 6728 2225   logger.debug("%
-00013fd0: 7322 2c20 6465 6275 675f 7265 7375 6c74  s", debug_result
-00013fe0: 290a 2020 2020 2020 2020 6966 2072 6573  ).        if res
-00013ff0: 756c 743a 0a20 2020 2020 2020 2020 2020  ult:.           
-00014000: 2066 6f72 2061 2069 6e20 7265 7375 6c74   for a in result
-00014010: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
-00014020: 2020 2020 2020 2020 2020 656e 7469 7479            entity
-00014030: 203d 2061 5b31 5d2e 6765 7428 2265 6e74   = a[1].get("ent
-00014040: 6974 7922 2c20 2222 290a 2020 2020 2020  ity", "").      
-00014050: 2020 2020 2020 2020 2020 6371 203d 2061            cq = a
-00014060: 5b31 5d2e 6765 7428 2263 7122 2c20 2222  [1].get("cq", ""
-00014070: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00014080: 2020 6974 7520 3d20 615b 315d 2e67 6574    itu = a[1].get
-00014090: 2822 6974 7522 2c20 2222 290a 2020 2020  ("itu", "").    
-000140a0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-000140b0: 696e 656e 7420 3d20 615b 315d 2e67 6574  inent = a[1].get
-000140c0: 2822 636f 6e74 696e 656e 7422 290a 2020  ("continent").  
-000140d0: 2020 2020 2020 2020 2020 2020 2020 6c61                la
-000140e0: 7420 3d20 666c 6f61 7428 615b 315d 2e67  t = float(a[1].g
-000140f0: 6574 2822 6c61 7422 2c20 2230 2e30 2229  et("lat", "0.0")
-00014100: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00014110: 2020 6c6f 6e20 3d20 666c 6f61 7428 615b    lon = float(a[
-00014120: 315d 2e67 6574 2822 6c6f 6e67 222c 2022  1].get("long", "
-00014130: 302e 3022 2929 0a20 2020 2020 2020 2020  0.0")).         
-00014140: 2020 2020 2020 206c 6f6e 203d 206c 6f6e         lon = lon
-00014150: 202a 202d 3120 2023 2063 7479 2e64 6174   * -1  # cty.dat
-00014160: 2066 696c 6520 696e 7665 7274 7320 6c6f   file inverts lo
-00014170: 6e67 6974 7564 6573 0a20 2020 2020 2020  ngitudes.       
-00014180: 2020 2020 2020 2020 2070 7269 6d61 7279           primary
-00014190: 5f70 6678 203d 2061 5b31 5d2e 6765 7428  _pfx = a[1].get(
-000141a0: 2270 7269 6d61 7279 5f70 6678 222c 2022  "primary_pfx", "
-000141b0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-000141c0: 2020 2068 6561 6469 6e67 203d 2062 6561     heading = bea
-000141d0: 7269 6e67 5f77 6974 685f 6c61 746c 6f6e  ring_with_latlon
-000141e0: 2873 656c 662e 7374 6174 696f 6e2e 6765  (self.station.ge
-000141f0: 7428 2247 7269 6453 7175 6172 6522 292c  t("GridSquare"),
-00014200: 206c 6174 2c20 6c6f 6e29 0a20 2020 2020   lat, lon).     
-00014210: 2020 2020 2020 2020 2020 206b 696c 6f6d             kilom
-00014220: 6574 6572 7320 3d20 6469 7374 616e 6365  eters = distance
-00014230: 5f77 6974 685f 6c61 746c 6f6e 280a 2020  _with_latlon(.  
-00014240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014250: 2020 7365 6c66 2e73 7461 7469 6f6e 2e67    self.station.g
-00014260: 6574 2822 4772 6964 5371 7561 7265 2229  et("GridSquare")
-00014270: 2c20 6c61 742c 206c 6f6e 0a20 2020 2020  , lat, lon.     
-00014280: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00014290: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000142a0: 662e 6865 6164 696e 675f 6469 7374 616e  f.heading_distan
-000142b0: 6365 2e73 6574 5465 7874 280a 2020 2020  ce.setText(.    
-000142c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000142d0: 6622 5265 6769 6f6e 616c 2048 6467 207b  f"Regional Hdg {
-000142e0: 6865 6164 696e 677d c2b0 204c 5020 7b72  heading}.. LP {r
-000142f0: 6563 6970 726f 636f 6c28 6865 6164 696e  eciprocol(headin
-00014300: 6729 7dc2 b020 2f20 220a 2020 2020 2020  g)}.. / ".      
-00014310: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-00014320: 6469 7374 616e 6365 207b 696e 7428 6b69  distance {int(ki
-00014330: 6c6f 6d65 7465 7273 2a30 2e36 3231 3337  lometers*0.62137
-00014340: 3129 7d6d 6920 7b6b 696c 6f6d 6574 6572  1)}mi {kilometer
-00014350: 737d 6b6d 220a 2020 2020 2020 2020 2020  s}km".          
-00014360: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00014370: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-00014380: 7461 6374 5b22 436f 756e 7472 7950 7265  tact["CountryPre
-00014390: 6669 7822 5d20 3d20 7072 696d 6172 795f  fix"] = primary_
-000143a0: 7066 780a 2020 2020 2020 2020 2020 2020  pfx.            
-000143b0: 2020 2020 7365 6c66 2e63 6f6e 7461 6374      self.contact
-000143c0: 5b22 5a4e 225d 203d 2069 6e74 2863 7129  ["ZN"] = int(cq)
-000143d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000143e0: 2069 6620 7365 6c66 2e63 6f6e 7465 7374   if self.contest
-000143f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00014400: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
-00014410: 6e74 6573 742e 6e61 6d65 203d 3d20 2249  ntest.name == "I
-00014420: 4152 5520 4846 223a 0a20 2020 2020 2020  ARU HF":.       
-00014430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014440: 2073 656c 662e 636f 6e74 6163 745b 225a   self.contact["Z
-00014450: 4e22 5d20 3d20 696e 7428 6974 7529 0a20  N"] = int(itu). 
-00014460: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00014470: 656c 662e 636f 6e74 6163 745b 2243 6f6e  elf.contact["Con
-00014480: 7469 6e65 6e74 225d 203d 2063 6f6e 7469  tinent"] = conti
-00014490: 6e65 6e74 0a20 2020 2020 2020 2020 2020  nent.           
-000144a0: 2020 2020 2073 656c 662e 6478 5f65 6e74       self.dx_ent
-000144b0: 6974 792e 7365 7454 6578 7428 0a20 2020  ity.setText(.   
-000144c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000144d0: 2066 227b 7072 696d 6172 795f 7066 787d   f"{primary_pfx}
-000144e0: 3a20 7b63 6f6e 7469 6e65 6e74 7d2f 7b65  : {continent}/{e
-000144f0: 6e74 6974 797d 2063 713a 7b63 717d 2069  ntity} cq:{cq} i
-00014500: 7475 3a7b 6974 757d 220a 2020 2020 2020  tu:{itu}".      
-00014510: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00014520: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-00014530: 656e 2863 616c 6c73 6967 6e29 203e 2032  en(callsign) > 2
-00014540: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00014550: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
-00014560: 6e74 6573 743a 0a20 2020 2020 2020 2020  ntest:.         
-00014570: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00014580: 656c 662e 636f 6e74 6573 742e 7072 6566  elf.contest.pref
-00014590: 696c 6c28 7365 6c66 290a 0a20 2020 2064  ill(self)..    d
-000145a0: 6566 2063 6865 636b 5f63 616c 6c73 6967  ef check_callsig
-000145b0: 6e32 2873 656c 662c 2063 616c 6c73 6967  n2(self, callsig
-000145c0: 6e29 3a0a 2020 2020 2020 2020 2222 2243  n):.        """C
-000145d0: 6865 636b 2063 616c 6c20 6f6e 6365 2065  heck call once e
-000145e0: 6e74 6572 6564 2222 220a 2020 2020 2020  ntered""".      
-000145f0: 2020 6361 6c6c 7369 676e 203d 2063 616c    callsign = cal
-00014600: 6c73 6967 6e2e 7374 7269 7028 290a 2020  lsign.strip().  
-00014610: 2020 2020 2020 6465 6275 675f 6c6f 6f6b        debug_look
-00014620: 7570 203d 2066 227b 7365 6c66 2e6c 6f6f  up = f"{self.loo
-00014630: 6b5f 7570 7d22 0a20 2020 2020 2020 206c  k_up}".        l
-00014640: 6f67 6765 722e 6465 6275 6728 2225 732c  ogger.debug("%s,
-00014650: 2025 7322 2c20 6361 6c6c 7369 676e 2c20   %s", callsign, 
-00014660: 6465 6275 675f 6c6f 6f6b 7570 290a 2020  debug_lookup).  
-00014670: 2020 2020 2020 6966 2068 6173 6174 7472        if hasattr
-00014680: 2873 656c 662e 6c6f 6f6b 5f75 702c 2022  (self.look_up, "
-00014690: 7365 7373 696f 6e22 293a 0a20 2020 2020  session"):.     
-000146a0: 2020 2020 2020 2069 6620 7365 6c66 2e6c         if self.l
-000146b0: 6f6f 6b5f 7570 2e73 6573 7369 6f6e 3a0a  ook_up.session:.
-000146c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000146d0: 7265 7370 6f6e 7365 203d 2073 656c 662e  response = self.
-000146e0: 6c6f 6f6b 5f75 702e 6c6f 6f6b 7570 2863  look_up.lookup(c
-000146f0: 616c 6c73 6967 6e29 0a20 2020 2020 2020  allsign).       
-00014700: 2020 2020 2020 2020 2064 6562 7567 5f72           debug_r
-00014710: 6573 706f 6e73 6520 3d20 6622 7b72 6573  esponse = f"{res
-00014720: 706f 6e73 657d 220a 2020 2020 2020 2020  ponse}".        
-00014730: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-00014740: 6562 7567 2822 5468 6520 5265 7370 6f6e  ebug("The Respon
-00014750: 7365 3a20 2573 5c6e 222c 2064 6562 7567  se: %s\n", debug
-00014760: 5f72 6573 706f 6e73 6529 0a20 2020 2020  _response).     
-00014770: 2020 2020 2020 2020 2020 2069 6620 7265             if re
-00014780: 7370 6f6e 7365 3a0a 2020 2020 2020 2020  sponse:.        
-00014790: 2020 2020 2020 2020 2020 2020 7468 6569              thei
-000147a0: 7267 7269 6420 3d20 7265 7370 6f6e 7365  rgrid = response
-000147b0: 2e67 6574 2822 6772 6964 2229 0a20 2020  .get("grid").   
-000147c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000147d0: 2073 656c 662e 636f 6e74 6163 745b 2247   self.contact["G
-000147e0: 7269 6453 7175 6172 6522 5d20 3d20 7468  ridSquare"] = th
-000147f0: 6569 7267 7269 640a 2020 2020 2020 2020  eirgrid.        
-00014800: 2020 2020 2020 2020 2020 2020 5f74 6865              _the
-00014810: 6972 636f 756e 7472 7920 3d20 7265 7370  ircountry = resp
-00014820: 6f6e 7365 2e67 6574 2822 636f 756e 7472  onse.get("countr
-00014830: 7922 290a 2020 2020 2020 2020 2020 2020  y").            
-00014840: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00014850: 7374 6174 696f 6e2e 6765 7428 2247 7269  station.get("Gri
-00014860: 6453 7175 6172 6522 2c20 2222 293a 0a20  dSquare", ""):. 
-00014870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014880: 2020 2020 2020 2068 6561 6469 6e67 203d         heading =
-00014890: 2062 6561 7269 6e67 2873 656c 662e 7374   bearing(self.st
-000148a0: 6174 696f 6e2e 6765 7428 2247 7269 6453  ation.get("GridS
-000148b0: 7175 6172 6522 2c20 2222 292c 2074 6865  quare", ""), the
-000148c0: 6972 6772 6964 290a 2020 2020 2020 2020  irgrid).        
-000148d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148e0: 6b69 6c6f 6d65 7465 7273 203d 2064 6973  kilometers = dis
-000148f0: 7461 6e63 6528 7365 6c66 2e73 7461 7469  tance(self.stati
-00014900: 6f6e 2e67 6574 2822 4772 6964 5371 7561  on.get("GridSqua
-00014910: 7265 2229 2c20 7468 6569 7267 7269 6429  re"), theirgrid)
-00014920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014930: 2020 2020 2020 2020 2073 656c 662e 6865           self.he
-00014940: 6164 696e 675f 6469 7374 616e 6365 2e73  ading_distance.s
-00014950: 6574 5465 7874 280a 2020 2020 2020 2020  etText(.        
-00014960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014970: 2020 2020 6622 7b74 6865 6972 6772 6964      f"{theirgrid
-00014980: 7d20 4864 6720 7b68 6561 6469 6e67 7dc2  } Hdg {heading}.
-00014990: b020 4c50 207b 7265 6369 7072 6f63 6f6c  . LP {reciprocol
-000149a0: 2868 6561 6469 6e67 297d c2b0 202f 2022  (heading)}.. / "
-000149b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000149c0: 2020 2020 2020 2020 2020 2020 2066 2264               f"d
-000149d0: 6973 7461 6e63 6520 7b69 6e74 286b 696c  istance {int(kil
-000149e0: 6f6d 6574 6572 732a 302e 3632 3133 3731  ometers*0.621371
-000149f0: 297d 6d69 207b 6b69 6c6f 6d65 7465 7273  )}mi {kilometers
-00014a00: 7d6b 6d22 0a20 2020 2020 2020 2020 2020  }km".           
-00014a10: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00014a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a30: 2020 2023 2073 656c 662e 6478 5f65 6e74     # self.dx_ent
-00014a40: 6974 792e 7365 7454 6578 7428 6622 7b74  ity.setText(f"{t
-00014a50: 6865 6972 636f 756e 7472 797d 2229 0a20  heircountry}"). 
-00014a60: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00014a70: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00014a80: 2020 2020 2020 2023 2073 656c 662e 6865         # self.he
-00014a90: 6164 696e 675f 6469 7374 616e 6365 2e73  ading_distance.s
-00014aa0: 6574 5465 7874 2822 4c6f 6f6b 7570 2066  etText("Lookup f
-00014ab0: 6169 6c65 642e 2229 0a0a 2020 2020 6465  ailed.")..    de
-00014ac0: 6620 6368 6563 6b5f 6475 7065 2873 656c  f check_dupe(sel
-00014ad0: 662c 2063 616c 6c3a 2073 7472 2920 2d3e  f, call: str) ->
-00014ae0: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
-00014af0: 2222 4368 6563 6b73 2069 6620 6120 6361  ""Checks if a ca
-00014b00: 6c6c 7369 676e 2069 7320 6120 6475 7065  llsign is a dupe
-00014b10: 206f 6e20 6375 7272 656e 7420 6261 6e64   on current band
-00014b20: 2f6d 6f64 652e 2222 220a 2020 2020 2020  /mode.""".      
-00014b30: 2020 6966 2073 656c 662e 636f 6e74 6573    if self.contes
-00014b40: 7420 6973 204e 6f6e 653a 0a20 2020 2020  t is None:.     
-00014b50: 2020 2020 2020 2073 656c 662e 7368 6f77         self.show
-00014b60: 5f6d 6573 7361 6765 5f62 6f78 2822 596f  _message_box("Yo
-00014b70: 7520 6861 7665 206e 6f20 636f 6e74 6573  u have no contes
-00014b80: 7420 6c6f 6164 6564 2e22 290a 2020 2020  t loaded.").    
-00014b90: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-00014ba0: 616c 7365 0a20 2020 2020 2020 2073 656c  alse.        sel
-00014bb0: 662e 636f 6e74 6573 742e 7072 6564 7570  f.contest.predup
-00014bc0: 6528 7365 6c66 290a 2020 2020 2020 2020  e(self).        
-00014bd0: 6261 6e64 203d 2066 6c6f 6174 2867 6574  band = float(get
-00014be0: 5f6c 6f67 6765 645f 6261 6e64 2873 7472  _logged_band(str
-00014bf0: 2873 656c 662e 7261 6469 6f5f 7374 6174  (self.radio_stat
-00014c00: 652e 6765 7428 2276 666f 6122 2c20 302e  e.get("vfoa", 0.
-00014c10: 3029 2929 290a 2020 2020 2020 2020 6d6f  0)))).        mo
-00014c20: 6465 203d 2073 656c 662e 7261 6469 6f5f  de = self.radio_
-00014c30: 7374 6174 652e 6765 7428 226d 6f64 6522  state.get("mode"
-00014c40: 2c20 2222 290a 2020 2020 2020 2020 6465  , "").        de
-00014c50: 6275 676c 696e 6520 3d20 280a 2020 2020  bugline = (.    
-00014c60: 2020 2020 2020 2020 6622 4361 6c6c 3a20          f"Call: 
-00014c70: 7b63 616c 6c7d 2042 616e 643a 207b 6261  {call} Band: {ba
-00014c80: 6e64 7d20 4d6f 6465 3a20 7b6d 6f64 657d  nd} Mode: {mode}
-00014c90: 2044 7570 6574 7970 653a 207b 7365 6c66   Dupetype: {self
-00014ca0: 2e63 6f6e 7465 7374 2e64 7570 655f 7479  .contest.dupe_ty
-00014cb0: 7065 7d22 0a20 2020 2020 2020 2029 0a20  pe}".        ). 
-00014cc0: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-00014cd0: 6275 6728 2225 7322 2c20 6465 6275 676c  bug("%s", debugl
-00014ce0: 696e 6529 0a20 2020 2020 2020 2069 6620  ine).        if 
-00014cf0: 7365 6c66 2e63 6f6e 7465 7374 2e64 7570  self.contest.dup
-00014d00: 655f 7479 7065 203d 3d20 313a 0a20 2020  e_type == 1:.   
-00014d10: 2020 2020 2020 2020 2072 6573 756c 7420           result 
-00014d20: 3d20 7365 6c66 2e64 6174 6162 6173 652e  = self.database.
-00014d30: 6368 6563 6b5f 6475 7065 2863 616c 6c29  check_dupe(call)
-00014d40: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00014d50: 2e63 6f6e 7465 7374 2e64 7570 655f 7479  .contest.dupe_ty
-00014d60: 7065 203d 3d20 323a 0a20 2020 2020 2020  pe == 2:.       
-00014d70: 2020 2020 2072 6573 756c 7420 3d20 7365       result = se
-00014d80: 6c66 2e64 6174 6162 6173 652e 6368 6563  lf.database.chec
-00014d90: 6b5f 6475 7065 5f6f 6e5f 6261 6e64 2863  k_dupe_on_band(c
-00014da0: 616c 6c2c 2062 616e 6429 0a20 2020 2020  all, band).     
-00014db0: 2020 2069 6620 7365 6c66 2e63 6f6e 7465     if self.conte
-00014dc0: 7374 2e64 7570 655f 7479 7065 203d 3d20  st.dupe_type == 
-00014dd0: 333a 0a20 2020 2020 2020 2020 2020 2072  3:.            r
-00014de0: 6573 756c 7420 3d20 7365 6c66 2e64 6174  esult = self.dat
-00014df0: 6162 6173 652e 6368 6563 6b5f 6475 7065  abase.check_dupe
-00014e00: 5f6f 6e5f 6261 6e64 5f6d 6f64 6528 6361  _on_band_mode(ca
-00014e10: 6c6c 2c20 6261 6e64 2c20 6d6f 6465 290a  ll, band, mode).
-00014e20: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00014e30: 636f 6e74 6573 742e 6475 7065 5f74 7970  contest.dupe_typ
-00014e40: 6520 3d3d 2034 3a0a 2020 2020 2020 2020  e == 4:.        
-00014e50: 2020 2020 7265 7375 6c74 203d 207b 2269      result = {"i
-00014e60: 7364 7570 6522 3a20 4661 6c73 657d 0a20  sdupe": False}. 
-00014e70: 2020 2020 2020 2064 6562 7567 6c69 6e65         debugline
-00014e80: 203d 2066 227b 7265 7375 6c74 7d22 0a20   = f"{result}". 
-00014e90: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-00014ea0: 6275 6728 2225 7322 2c20 6465 6275 676c  bug("%s", debugl
-00014eb0: 696e 6529 0a20 2020 2020 2020 2072 6574  ine).        ret
-00014ec0: 7572 6e20 7265 7375 6c74 2e67 6574 2822  urn result.get("
-00014ed0: 6973 6475 7065 222c 2046 616c 7365 290a  isdupe", False).
-00014ee0: 0a20 2020 2064 6566 2073 6574 6d6f 6465  .    def setmode
-00014ef0: 2873 656c 662c 206d 6f64 653a 2073 7472  (self, mode: str
-00014f00: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-00014f10: 2020 2022 2222 7374 7562 2066 6f72 2077     """stub for w
-00014f20: 6865 6e20 7468 6520 6d6f 6465 2063 6861  hen the mode cha
-00014f30: 6e67 6573 2e22 2222 0a20 2020 2020 2020  nges.""".       
-00014f40: 2069 6620 6d6f 6465 203d 3d20 2243 5722   if mode == "CW"
-00014f50: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00014f60: 2073 656c 662e 6375 7272 656e 745f 6d6f   self.current_mo
-00014f70: 6465 2021 3d20 2243 5722 3a0a 2020 2020  de != "CW":.    
-00014f80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00014f90: 2e63 7572 7265 6e74 5f6d 6f64 6520 3d20  .current_mode = 
-00014fa0: 2243 5722 0a20 2020 2020 2020 2020 2020  "CW".           
-00014fb0: 2020 2020 2023 2073 656c 662e 6d6f 6465       # self.mode
-00014fc0: 2e73 6574 5465 7874 2822 4357 2229 0a20  .setText("CW"). 
-00014fd0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00014fe0: 656c 662e 7365 6e74 2e73 6574 5465 7874  elf.sent.setText
-00014ff0: 2822 3539 3922 290a 2020 2020 2020 2020  ("599").        
-00015000: 2020 2020 2020 2020 7365 6c66 2e72 6563          self.rec
-00015010: 6569 7665 2e73 6574 5465 7874 2822 3539  eive.setText("59
-00015020: 3922 290a 2020 2020 2020 2020 2020 2020  9").            
-00015030: 2020 2020 7365 6c66 2e72 6561 645f 6377      self.read_cw
-00015040: 5f6d 6163 726f 7328 290a 2020 2020 2020  _macros().      
-00015050: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-00015060: 2020 2020 2069 6620 6d6f 6465 203d 3d20       if mode == 
-00015070: 2253 5342 223a 0a20 2020 2020 2020 2020  "SSB":.         
-00015080: 2020 2069 6620 7365 6c66 2e63 7572 7265     if self.curre
-00015090: 6e74 5f6d 6f64 6520 213d 2022 5353 4222  nt_mode != "SSB"
-000150a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000150b0: 2020 7365 6c66 2e63 7572 7265 6e74 5f6d    self.current_m
-000150c0: 6f64 6520 3d20 2253 5342 220a 2020 2020  ode = "SSB".    
-000150d0: 2020 2020 2020 2020 2020 2020 2320 7365              # se
-000150e0: 6c66 2e6d 6f64 652e 7365 7454 6578 7428  lf.mode.setText(
-000150f0: 2253 5342 2229 0a20 2020 2020 2020 2020  "SSB").         
-00015100: 2020 2020 2020 2073 656c 662e 7365 6e74         self.sent
-00015110: 2e73 6574 5465 7874 2822 3539 2229 0a20  .setText("59"). 
-00015120: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015130: 656c 662e 7265 6365 6976 652e 7365 7454  elf.receive.setT
-00015140: 6578 7428 2235 3922 290a 2020 2020 2020  ext("59").      
-00015150: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-00015160: 6561 645f 6377 5f6d 6163 726f 7328 290a  ead_cw_macros().
-00015170: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00015180: 726e 0a20 2020 2020 2020 2069 6620 6d6f  rn.        if mo
-00015190: 6465 203d 3d20 2252 5454 5922 3a0a 2020  de == "RTTY":.  
-000151a0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-000151b0: 662e 6375 7272 656e 745f 6d6f 6465 2021  f.current_mode !
-000151c0: 3d20 2252 5454 5922 3a0a 2020 2020 2020  = "RTTY":.      
-000151d0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-000151e0: 7572 7265 6e74 5f6d 6f64 6520 3d20 2252  urrent_mode = "R
-000151f0: 5454 5922 0a20 2020 2020 2020 2020 2020  TTY".           
-00015200: 2020 2020 2023 2073 656c 662e 6d6f 6465       # self.mode
-00015210: 2e73 6574 5465 7874 2822 5254 5459 2229  .setText("RTTY")
-00015220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015230: 2073 656c 662e 7365 6e74 2e73 6574 5465   self.sent.setTe
-00015240: 7874 2822 3539 2229 0a20 2020 2020 2020  xt("59").       
-00015250: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-00015260: 6365 6976 652e 7365 7454 6578 7428 2235  ceive.setText("5
-00015270: 3922 290a 0a20 2020 2064 6566 2067 6574  9")..    def get
-00015280: 5f6f 706f 6e28 7365 6c66 293a 0a20 2020  _opon(self):.   
-00015290: 2020 2020 2022 2222 4374 726c 2b4f 206f       """Ctrl+O o
-000152a0: 7220 4f50 4f4e 2064 6961 6c6f 6722 2222  r OPON dialog"""
-000152b0: 0a20 2020 2020 2020 2073 656c 662e 6f70  .        self.op
-000152c0: 6f6e 5f64 6961 6c6f 6720 3d20 4f70 4f6e  on_dialog = OpOn
-000152d0: 2857 4f52 4b49 4e47 5f50 4154 4829 0a20  (WORKING_PATH). 
-000152e0: 2020 2020 2020 2073 656c 662e 6f70 6f6e         self.opon
-000152f0: 5f64 6961 6c6f 672e 6163 6365 7074 6564  _dialog.accepted
-00015300: 2e63 6f6e 6e65 6374 2873 656c 662e 6e65  .connect(self.ne
-00015310: 775f 6f70 290a 2020 2020 2020 2020 7365  w_op).        se
-00015320: 6c66 2e6f 706f 6e5f 6469 616c 6f67 2e6f  lf.opon_dialog.o
-00015330: 7065 6e28 290a 0a20 2020 2064 6566 206e  pen()..    def n
-00015340: 6577 5f6f 7028 7365 6c66 293a 0a20 2020  ew_op(self):.   
-00015350: 2020 2020 2022 2222 5361 7665 206e 6577       """Save new
-00015360: 204f 5022 2222 0a20 2020 2020 2020 2069   OP""".        i
-00015370: 6620 7365 6c66 2e6f 706f 6e5f 6469 616c  f self.opon_dial
-00015380: 6f67 2e4e 6577 4f70 6572 6174 6f72 2e74  og.NewOperator.t
-00015390: 6578 7428 293a 0a20 2020 2020 2020 2020  ext():.         
-000153a0: 2020 2073 656c 662e 6375 7272 656e 745f     self.current_
-000153b0: 6f70 203d 2073 656c 662e 6f70 6f6e 5f64  op = self.opon_d
-000153c0: 6961 6c6f 672e 4e65 774f 7065 7261 746f  ialog.NewOperato
-000153d0: 722e 7465 7874 2829 2e75 7070 6572 2829  r.text().upper()
-000153e0: 0a20 2020 2020 2020 2073 656c 662e 6f70  .        self.op
-000153f0: 6f6e 5f64 6961 6c6f 672e 636c 6f73 6528  on_dialog.close(
-00015400: 290a 2020 2020 2020 2020 6c6f 6767 6572  ).        logger
-00015410: 2e64 6562 7567 2822 4e65 7720 4f70 3a20  .debug("New Op: 
-00015420: 2573 222c 2073 656c 662e 6375 7272 656e  %s", self.curren
-00015430: 745f 6f70 290a 2020 2020 2020 2020 7365  t_op).        se
-00015440: 6c66 2e6d 616b 655f 6f70 5f64 6972 2829  lf.make_op_dir()
-00015450: 0a0a 2020 2020 6465 6620 6d61 6b65 5f6f  ..    def make_o
-00015460: 705f 6469 7228 7365 6c66 293a 0a20 2020  p_dir(self):.   
-00015470: 2020 2020 2022 2222 4372 6561 7465 204f       """Create O
-00015480: 5020 6469 7265 6374 6f72 7920 6966 2069  P directory if i
-00015490: 7420 646f 6573 206e 6f74 2065 7869 7374  t does not exist
-000154a0: 2e22 2222 0a20 2020 2020 2020 2069 6620  .""".        if 
-000154b0: 7365 6c66 2e63 7572 7265 6e74 5f6f 703a  self.current_op:
-000154c0: 0a20 2020 2020 2020 2020 2020 206f 705f  .            op_
-000154d0: 7061 7468 203d 2050 6174 6828 4441 5441  path = Path(DATA
-000154e0: 5f50 4154 4829 202f 2073 656c 662e 6375  _PATH) / self.cu
-000154f0: 7272 656e 745f 6f70 0a20 2020 2020 2020  rrent_op.       
-00015500: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-00015510: 6728 226f 705f 7061 7468 3a20 2573 222c  g("op_path: %s",
-00015520: 2073 7472 286f 705f 7061 7468 2929 0a20   str(op_path)). 
-00015530: 2020 2020 2020 2020 2020 2069 6620 6f70             if op
-00015540: 5f70 6174 682e 6973 5f64 6972 2829 2069  _path.is_dir() i
-00015550: 7320 4661 6c73 653a 0a20 2020 2020 2020  s False:.       
-00015560: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-00015570: 6465 6275 6728 2243 7265 6174 696e 6720  debug("Creating 
-00015580: 4f70 2044 6972 6563 746f 7279 3a20 2573  Op Directory: %s
-00015590: 222c 2073 7472 286f 705f 7061 7468 2929  ", str(op_path))
-000155a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000155b0: 206f 732e 6d6b 6469 7228 7374 7228 6f70   os.mkdir(str(op
-000155c0: 5f70 6174 6829 290a 2020 2020 2020 2020  _path)).        
-000155d0: 2020 2020 6966 206f 705f 7061 7468 2e69      if op_path.i
-000155e0: 735f 6469 7228 293a 0a20 2020 2020 2020  s_dir():.       
-000155f0: 2020 2020 2020 2020 2073 6f75 7263 655f           source_
-00015600: 7061 7468 203d 2050 6174 6828 574f 524b  path = Path(WORK
-00015610: 494e 475f 5041 5448 2920 2f20 2264 6174  ING_PATH) / "dat
-00015620: 6122 202f 2022 7068 6f6e 6574 6963 7322  a" / "phonetics"
-00015630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015640: 206c 6f67 6765 722e 6465 6275 6728 2273   logger.debug("s
-00015650: 6f75 7263 655f 7061 7468 3a20 2573 222c  ource_path: %s",
-00015660: 2073 7472 2873 6f75 7263 655f 7061 7468   str(source_path
-00015670: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-00015680: 2020 2066 6f72 2063 6869 6c64 2069 6e20     for child in 
-00015690: 736f 7572 6365 5f70 6174 682e 6974 6572  source_path.iter
-000156a0: 6469 7228 293a 0a20 2020 2020 2020 2020  dir():.         
-000156b0: 2020 2020 2020 2020 2020 2064 6573 7469             desti
-000156c0: 6e61 7469 6f6e 5f66 696c 6520 3d20 6f70  nation_file = op
-000156d0: 5f70 6174 6820 2f20 6368 696c 642e 6e61  _path / child.na
-000156e0: 6d65 0a20 2020 2020 2020 2020 2020 2020  me.             
-000156f0: 2020 2020 2020 2069 6620 6465 7374 696e         if destin
-00015700: 6174 696f 6e5f 6669 6c65 2e69 735f 6669  ation_file.is_fi
-00015710: 6c65 2829 2069 7320 4661 6c73 653a 0a20  le() is False:. 
-00015720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015730: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-00015740: 6275 6728 2244 6573 7469 6e61 7469 6f6e  bug("Destination
-00015750: 3a20 2573 222c 2073 7472 2864 6573 7469  : %s", str(desti
-00015760: 6e61 7469 6f6e 5f66 696c 6529 290a 2020  nation_file)).  
-00015770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015780: 2020 2020 2020 6465 7374 696e 6174 696f        destinatio
-00015790: 6e5f 6669 6c65 2e77 7269 7465 5f62 7974  n_file.write_byt
-000157a0: 6573 2863 6869 6c64 2e72 6561 645f 6279  es(child.read_by
-000157b0: 7465 7328 2929 0a0a 2020 2020 6465 6620  tes())..    def 
-000157c0: 706f 6c6c 5f72 6164 696f 2873 656c 6629  poll_radio(self)
-000157d0: 3a0a 2020 2020 2020 2020 2222 2273 7475  :.        """stu
-000157e0: 6222 2222 0a20 2020 2020 2020 2069 6620  b""".        if 
-000157f0: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
-00015800: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00015810: 2073 656c 662e 7269 675f 636f 6e74 726f   self.rig_contro
-00015820: 6c2e 6f6e 6c69 6e65 2069 7320 4661 6c73  l.online is Fals
-00015830: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00015840: 2020 2073 656c 662e 7269 675f 636f 6e74     self.rig_cont
-00015850: 726f 6c2e 7265 696e 6974 2829 0a20 2020  rol.reinit().   
-00015860: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00015870: 2e72 6967 5f63 6f6e 7472 6f6c 2e6f 6e6c  .rig_control.onl
-00015880: 696e 653a 0a20 2020 2020 2020 2020 2020  ine:.           
-00015890: 2020 2020 2069 6e66 6f5f 6469 7274 7920       info_dirty 
-000158a0: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
-000158b0: 2020 2020 2020 2020 7666 6f20 3d20 7365          vfo = se
-000158c0: 6c66 2e72 6967 5f63 6f6e 7472 6f6c 2e67  lf.rig_control.g
-000158d0: 6574 5f76 666f 2829 0a20 2020 2020 2020  et_vfo().       
-000158e0: 2020 2020 2020 2020 206d 6f64 6520 3d20           mode = 
-000158f0: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
-00015900: 2e67 6574 5f6d 6f64 6528 290a 2020 2020  .get_mode().    
-00015910: 2020 2020 2020 2020 2020 2020 6277 203d              bw =
-00015920: 2073 656c 662e 7269 675f 636f 6e74 726f   self.rig_contro
-00015930: 6c2e 6765 745f 6277 2829 0a20 2020 2020  l.get_bw().     
-00015940: 2020 2020 2020 2020 2020 2023 2073 656c             # sel
-00015950: 662e 7261 6469 6f5f 7374 6174 655b 2270  f.radio_state["p
-00015960: 7474 225d 203d 2073 656c 662e 7269 675f  tt"] = self.rig_
-00015970: 636f 6e74 726f 6c2e 6765 745f 7074 7428  control.get_ptt(
-00015980: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-00015990: 2020 2069 6620 6d6f 6465 203d 3d20 2243     if mode == "C
-000159a0: 5722 3a0a 2020 2020 2020 2020 2020 2020  W":.            
-000159b0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
-000159c0: 6d6f 6465 286d 6f64 6529 0a20 2020 2020  mode(mode).     
-000159d0: 2020 2020 2020 2020 2020 2069 6620 6d6f             if mo
-000159e0: 6465 203d 3d20 224c 5342 2220 6f72 206d  de == "LSB" or m
-000159f0: 6f64 6520 3d3d 2022 5553 4222 3a0a 2020  ode == "USB":.  
-00015a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a10: 2020 7365 6c66 2e73 6574 6d6f 6465 2822    self.setmode("
-00015a20: 5353 4222 290a 2020 2020 2020 2020 2020  SSB").          
-00015a30: 2020 2020 2020 6966 206d 6f64 6520 3d3d        if mode ==
-00015a40: 2022 5254 5459 223a 0a20 2020 2020 2020   "RTTY":.       
-00015a50: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00015a60: 662e 7365 746d 6f64 6528 2252 5454 5922  f.setmode("RTTY"
-00015a70: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-00015a80: 2020 2069 6620 7365 6c66 2e72 6164 696f     if self.radio
-00015a90: 5f73 7461 7465 2e67 6574 2822 7666 6f61  _state.get("vfoa
-00015aa0: 2229 2021 3d20 7666 6f3a 0a20 2020 2020  ") != vfo:.     
-00015ab0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00015ac0: 6e66 6f5f 6469 7274 7920 3d20 5472 7565  nfo_dirty = True
-00015ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015ae0: 2020 2020 2073 656c 662e 7261 6469 6f5f       self.radio_
-00015af0: 7374 6174 655b 2276 666f 6122 5d20 3d20  state["vfoa"] = 
-00015b00: 7666 6f0a 2020 2020 2020 2020 2020 2020  vfo.            
-00015b10: 2020 2020 6261 6e64 203d 2067 6574 6261      band = getba
-00015b20: 6e64 2873 7472 2876 666f 2929 0a20 2020  nd(str(vfo)).   
-00015b30: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00015b40: 662e 7261 6469 6f5f 7374 6174 655b 2262  f.radio_state["b
-00015b50: 616e 6422 5d20 3d20 6261 6e64 0a20 2020  and"] = band.   
-00015b60: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00015b70: 662e 636f 6e74 6163 745b 2242 616e 6422  f.contact["Band"
-00015b80: 5d20 3d20 6765 745f 6c6f 6767 6564 5f62  ] = get_logged_b
-00015b90: 616e 6428 7374 7228 7666 6f29 290a 2020  and(str(vfo)).  
-00015ba0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00015bb0: 6c66 2e73 6574 5f62 616e 645f 696e 6469  lf.set_band_indi
-00015bc0: 6361 746f 7228 6261 6e64 290a 0a20 2020  cator(band)..   
-00015bd0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00015be0: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
-00015bf0: 2e67 6574 2822 6d6f 6465 2229 2021 3d20  .get("mode") != 
-00015c00: 6d6f 6465 3a0a 2020 2020 2020 2020 2020  mode:.          
-00015c10: 2020 2020 2020 2020 2020 696e 666f 5f64            info_d
-00015c20: 6972 7479 203d 2054 7275 650a 2020 2020  irty = True.    
-00015c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015c40: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
-00015c50: 5b22 6d6f 6465 225d 203d 206d 6f64 650a  ["mode"] = mode.
-00015c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015c70: 2069 6620 7365 6c66 2e72 6164 696f 5f73   if self.radio_s
-00015c80: 7461 7465 2e67 6574 2822 6277 2229 2021  tate.get("bw") !
-00015c90: 3d20 6277 3a0a 2020 2020 2020 2020 2020  = bw:.          
-00015ca0: 2020 2020 2020 2020 2020 696e 666f 5f64            info_d
-00015cb0: 6972 7479 203d 2054 7275 650a 2020 2020  irty = True.    
-00015cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015cd0: 7365 6c66 2e72 6164 696f 5f73 7461 7465  self.radio_state
-00015ce0: 5b22 6277 225d 203d 2062 770a 0a20 2020  ["bw"] = bw..   
-00015cf0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00015d00: 6461 7465 7469 6d65 2e6e 6f77 2829 203e  datetime.now() >
-00015d10: 2067 6c6f 6261 6c73 2829 5b22 706f 6c6c   globals()["poll
-00015d20: 5f74 696d 6522 5d20 6f72 2069 6e66 6f5f  _time"] or info_
-00015d30: 6469 7274 793a 0a20 2020 2020 2020 2020  dirty:.         
-00015d40: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-00015d50: 722e 6465 6275 6728 2256 464f 3a20 2573  r.debug("VFO: %s
-00015d60: 2020 4d4f 4445 3a20 2573 2042 573a 2025    MODE: %s BW: %
-00015d70: 7322 2c20 7666 6f2c 206d 6f64 652c 2062  s", vfo, mode, b
-00015d80: 7729 0a20 2020 2020 2020 2020 2020 2020  w).             
-00015d90: 2020 2020 2020 2073 656c 662e 7365 745f         self.set_
-00015da0: 7769 6e64 6f77 5f74 6974 6c65 2829 0a20  window_title(). 
-00015db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015dc0: 2020 2063 6d64 203d 207b 7d0a 2020 2020     cmd = {}.    
-00015dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015de0: 636d 645b 2263 6d64 225d 203d 2022 5241  cmd["cmd"] = "RA
-00015df0: 4449 4f5f 5354 4154 4522 0a20 2020 2020  DIO_STATE".     
-00015e00: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00015e10: 6d64 5b22 7374 6174 696f 6e22 5d20 3d20  md["station"] = 
-00015e20: 706c 6174 666f 726d 2e6e 6f64 6528 290a  platform.node().
-00015e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015e40: 2020 2020 636d 645b 2262 616e 6422 5d20      cmd["band"] 
-00015e50: 3d20 6261 6e64 0a20 2020 2020 2020 2020  = band.         
-00015e60: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
-00015e70: 7666 6f61 225d 203d 2076 666f 0a20 2020  vfoa"] = vfo.   
-00015e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015e90: 2063 6d64 5b22 6d6f 6465 225d 203d 206d   cmd["mode"] = m
-00015ea0: 6f64 650a 2020 2020 2020 2020 2020 2020  ode.            
-00015eb0: 2020 2020 2020 2020 636d 645b 2262 7722          cmd["bw"
-00015ec0: 5d20 3d20 6277 0a20 2020 2020 2020 2020  ] = bw.         
-00015ed0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015ee0: 6d75 6c74 6963 6173 745f 696e 7465 7266  multicast_interf
-00015ef0: 6163 652e 7365 6e64 5f61 735f 6a73 6f6e  ace.send_as_json
-00015f00: 2863 6d64 290a 2020 2020 2020 2020 2020  (cmd).          
-00015f10: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00015f20: 662e 6e31 6d6d 3a0a 2020 2020 2020 2020  f.n1mm:.        
-00015f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015f40: 6966 2073 656c 662e 6e31 6d6d 2e73 656e  if self.n1mm.sen
-00015f50: 645f 7261 6469 6f5f 7061 636b 6574 733a  d_radio_packets:
-00015f60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015f70: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00015f80: 662e 6e31 6d6d 2e72 6164 696f 5f69 6e66  f.n1mm.radio_inf
-00015f90: 6f5b 2246 7265 7122 5d20 3d20 7666 6f5b  o["Freq"] = vfo[
-00015fa0: 3a2d 315d 0a20 2020 2020 2020 2020 2020  :-1].           
-00015fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015fc0: 2073 656c 662e 6e31 6d6d 2e72 6164 696f   self.n1mm.radio
-00015fd0: 5f69 6e66 6f5b 2254 5846 7265 7122 5d20  _info["TXFreq"] 
-00015fe0: 3d20 7666 6f5b 3a2d 315d 0a20 2020 2020  = vfo[:-1].     
-00015ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016000: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
-00016010: 2e72 6164 696f 5f69 6e66 6f5b 224d 6f64  .radio_info["Mod
-00016020: 6522 5d20 3d20 6d6f 6465 0a20 2020 2020  e"] = mode.     
-00016030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016040: 2020 2020 2020 2073 656c 662e 6e31 6d6d         self.n1mm
-00016050: 2e72 6164 696f 5f69 6e66 6f5b 224f 7043  .radio_info["OpC
-00016060: 616c 6c22 5d20 3d20 7365 6c66 2e63 7572  all"] = self.cur
-00016070: 7265 6e74 5f6f 700a 2020 2020 2020 2020  rent_op.        
-00016080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016090: 2020 2020 7365 6c66 2e6e 316d 6d2e 7261      self.n1mm.ra
-000160a0: 6469 6f5f 696e 666f 5b22 4973 5275 6e6e  dio_info["IsRunn
-000160b0: 696e 6722 5d20 3d20 7374 7228 0a20 2020  ing"] = str(.   
-000160c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000160d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000160e0: 662e 7072 6566 2e67 6574 2822 7275 6e5f  f.pref.get("run_
-000160f0: 7374 6174 6522 2c20 4661 6c73 6529 0a20  state", False). 
-00016100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016110: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00016120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016130: 2020 2020 2020 2020 2073 656c 662e 6e31           self.n1
-00016140: 6d6d 2e73 656e 645f 7261 6469 6f28 290a  mm.send_radio().
-00016150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016160: 2020 2020 676c 6f62 616c 7328 295b 2270      globals()["p
-00016170: 6f6c 6c5f 7469 6d65 225d 203d 2064 6174  oll_time"] = dat
-00016180: 6574 696d 652e 6e6f 7728 2920 2b20 6474  etime.now() + dt
-00016190: 2e74 696d 6564 656c 7461 2873 6563 6f6e  .timedelta(secon
-000161a0: 6473 3d31 3029 0a0a 2020 2020 6465 6620  ds=10)..    def 
-000161b0: 6564 6974 5f63 775f 6d61 6372 6f73 2873  edit_cw_macros(s
-000161c0: 656c 6629 202d 3e20 4e6f 6e65 3a0a 2020  elf) -> None:.  
-000161d0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000161e0: 2020 4361 6c6c 7320 7468 6520 6465 6661    Calls the defa
-000161f0: 756c 7420 7465 7874 2065 6469 746f 7220  ult text editor 
-00016200: 746f 2065 6469 7420 7468 6520 4357 206d  to edit the CW m
-00016210: 6163 726f 2066 696c 652e 0a20 2020 2020  acro file..     
-00016220: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-00016230: 6620 7365 6c66 2e72 6164 696f 5f73 7461  f self.radio_sta
-00016240: 7465 2e67 6574 2822 6d6f 6465 2229 203d  te.get("mode") =
-00016250: 3d20 2243 5722 3a0a 2020 2020 2020 2020  = "CW":.        
-00016260: 2020 2020 6d61 6372 6f5f 6669 6c65 203d      macro_file =
-00016270: 2022 2f63 776d 6163 726f 732e 7478 7422   "/cwmacros.txt"
-00016280: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00016290: 2020 2020 2020 2020 2020 206d 6163 726f             macro
-000162a0: 5f66 696c 6520 3d20 222f 7373 626d 6163  _file = "/ssbmac
-000162b0: 726f 732e 7478 7422 0a20 2020 2020 2020  ros.txt".       
-000162c0: 2069 6620 6e6f 7420 5061 7468 2844 4154   if not Path(DAT
-000162d0: 415f 5041 5448 202b 206d 6163 726f 5f66  A_PATH + macro_f
-000162e0: 696c 6529 2e65 7869 7374 7328 293a 0a20  ile).exists():. 
-000162f0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-00016300: 722e 6465 6275 6728 2272 6561 645f 6377  r.debug("read_cw
-00016310: 5f6d 6163 726f 733a 2063 6f70 7969 6e67  _macros: copying
-00016320: 2064 6566 6175 6c74 206d 6163 726f 2066   default macro f
-00016330: 696c 652e 2229 0a20 2020 2020 2020 2020  ile.").         
-00016340: 2020 2063 6f70 7966 696c 6528 574f 524b     copyfile(WORK
-00016350: 494e 475f 5041 5448 202b 2022 2f64 6174  ING_PATH + "/dat
-00016360: 6122 202b 206d 6163 726f 5f66 696c 652c  a" + macro_file,
-00016370: 2044 4154 415f 5041 5448 202b 206d 6163   DATA_PATH + mac
-00016380: 726f 5f66 696c 6529 0a20 2020 2020 2020  ro_file).       
-00016390: 206f 732e 7379 7374 656d 2866 2278 6467   os.system(f"xdg
-000163a0: 2d6f 7065 6e20 7b44 4154 415f 5041 5448  -open {DATA_PATH
-000163b0: 7d7b 6d61 6372 6f5f 6669 6c65 7d22 290a  }{macro_file}").
-000163c0: 0a20 2020 2064 6566 2072 6561 645f 6377  .    def read_cw
-000163d0: 5f6d 6163 726f 7328 7365 6c66 2920 2d3e  _macros(self) ->
-000163e0: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-000163f0: 2222 0a20 2020 2020 2020 2052 6561 6473  "".        Reads
-00016400: 2069 6e20 7468 6520 4357 206d 6163 726f   in the CW macro
-00016410: 732c 2066 6972 7374 7320 6974 2063 6865  s, firsts it che
-00016420: 636b 7320 746f 2073 6565 2069 6620 7468  cks to see if th
-00016430: 6520 6669 6c65 2065 7869 7374 732e 2049  e file exists. I
-00016440: 6620 6974 2064 6f65 7320 6e6f 742c 0a20  f it does not,. 
-00016450: 2020 2020 2020 2061 6e64 2074 6869 7320         and this 
-00016460: 6861 7320 6265 656e 2070 6163 6b61 6765  has been package
-00016470: 6420 7769 7468 2070 7969 6e73 7461 6c6c  d with pyinstall
-00016480: 6572 2069 7420 7769 6c6c 2063 6f70 7920  er it will copy 
-00016490: 7468 6520 6465 6661 756c 7420 6669 6c65  the default file
-000164a0: 2066 726f 6d20 7468 650a 2020 2020 2020   from the.      
-000164b0: 2020 7465 6d70 2064 6972 6563 746f 7279    temp directory
-000164c0: 2074 6869 7320 6973 2072 756e 6e69 6e67   this is running
-000164d0: 2066 726f 6d2e 2e2e 2049 6e20 7468 656f   from... In theo
-000164e0: 7279 2e0a 2020 2020 2020 2020 2222 220a  ry..        """.
-000164f0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00016500: 2e72 6164 696f 5f73 7461 7465 2e67 6574  .radio_state.get
-00016510: 2822 6d6f 6465 2229 203d 3d20 2243 5722  ("mode") == "CW"
-00016520: 3a0a 2020 2020 2020 2020 2020 2020 6d61  :.            ma
-00016530: 6372 6f5f 6669 6c65 203d 2022 2f63 776d  cro_file = "/cwm
-00016540: 6163 726f 732e 7478 7422 0a20 2020 2020  acros.txt".     
-00016550: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00016560: 2020 2020 206d 6163 726f 5f66 696c 6520       macro_file 
-00016570: 3d20 222f 7373 626d 6163 726f 732e 7478  = "/ssbmacros.tx
-00016580: 7422 0a0a 2020 2020 2020 2020 6966 206e  t"..        if n
-00016590: 6f74 2050 6174 6828 4441 5441 5f50 4154  ot Path(DATA_PAT
-000165a0: 4820 2b20 6d61 6372 6f5f 6669 6c65 292e  H + macro_file).
-000165b0: 6578 6973 7473 2829 3a0a 2020 2020 2020  exists():.      
-000165c0: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-000165d0: 7567 2822 7265 6164 5f63 775f 6d61 6372  ug("read_cw_macr
-000165e0: 6f73 3a20 636f 7079 696e 6720 6465 6661  os: copying defa
-000165f0: 756c 7420 6d61 6372 6f20 6669 6c65 2e22  ult macro file."
-00016600: 290a 2020 2020 2020 2020 2020 2020 636f  ).            co
-00016610: 7079 6669 6c65 2857 4f52 4b49 4e47 5f50  pyfile(WORKING_P
-00016620: 4154 4820 2b20 222f 6461 7461 2220 2b20  ATH + "/data" + 
-00016630: 6d61 6372 6f5f 6669 6c65 2c20 4441 5441  macro_file, DATA
-00016640: 5f50 4154 4820 2b20 6d61 6372 6f5f 6669  _PATH + macro_fi
-00016650: 6c65 290a 2020 2020 2020 2020 7769 7468  le).        with
-00016660: 206f 7065 6e28 4441 5441 5f50 4154 4820   open(DATA_PATH 
-00016670: 2b20 6d61 6372 6f5f 6669 6c65 2c20 2272  + macro_file, "r
-00016680: 222c 2065 6e63 6f64 696e 673d 2275 7466  ", encoding="utf
-00016690: 2d38 2229 2061 7320 6669 6c65 5f64 6573  -8") as file_des
-000166a0: 6372 6970 746f 723a 0a20 2020 2020 2020  criptor:.       
-000166b0: 2020 2020 2066 6f72 206c 696e 6520 696e       for line in
-000166c0: 2066 696c 655f 6465 7363 7269 7074 6f72   file_descriptor
-000166d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000166e0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-000166f0: 2020 2020 2020 2020 2020 206d 6f64 652c             mode,
-00016700: 2066 6b65 792c 2062 7574 746f 6e6e 616d   fkey, buttonnam
-00016710: 652c 2063 7774 6578 7420 3d20 6c69 6e65  e, cwtext = line
-00016720: 2e73 706c 6974 2822 7c22 290a 2020 2020  .split("|").    
-00016730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016740: 6966 206d 6f64 652e 7374 7269 7028 292e  if mode.strip().
-00016750: 7570 7065 7228 2920 3d3d 2022 5222 2061  upper() == "R" a
-00016760: 6e64 2073 656c 662e 7072 6566 2e67 6574  nd self.pref.get
-00016770: 2822 7275 6e5f 7374 6174 6522 293a 0a20  ("run_state"):. 
-00016780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016790: 2020 2020 2020 2073 656c 662e 666b 6579         self.fkey
-000167a0: 735b 666b 6579 2e73 7472 6970 2829 5d20  s[fkey.strip()] 
-000167b0: 3d20 2862 7574 746f 6e6e 616d 652e 7374  = (buttonname.st
-000167c0: 7269 7028 292c 2063 7774 6578 742e 7374  rip(), cwtext.st
-000167d0: 7269 7028 2929 0a20 2020 2020 2020 2020  rip()).         
-000167e0: 2020 2020 2020 2020 2020 2069 6620 6d6f             if mo
-000167f0: 6465 2e73 7472 6970 2829 2e75 7070 6572  de.strip().upper
-00016800: 2829 2021 3d20 2252 2220 616e 6420 6e6f  () != "R" and no
-00016810: 7420 7365 6c66 2e70 7265 662e 6765 7428  t self.pref.get(
-00016820: 2272 756e 5f73 7461 7465 2229 3a0a 2020  "run_state"):.  
-00016830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016840: 2020 2020 2020 7365 6c66 2e66 6b65 7973        self.fkeys
-00016850: 5b66 6b65 792e 7374 7269 7028 295d 203d  [fkey.strip()] =
-00016860: 2028 6275 7474 6f6e 6e61 6d65 2e73 7472   (buttonname.str
-00016870: 6970 2829 2c20 6377 7465 7874 2e73 7472  ip(), cwtext.str
-00016880: 6970 2829 290a 2020 2020 2020 2020 2020  ip()).          
-00016890: 2020 2020 2020 6578 6365 7074 2056 616c        except Val
-000168a0: 7565 4572 726f 7220 6173 2065 7272 3a0a  ueError as err:.
-000168b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000168c0: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
-000168d0: 2272 6561 645f 6377 5f6d 6163 726f 733a  "read_cw_macros:
-000168e0: 2025 7322 2c20 6572 7229 0a20 2020 2020   %s", err).     
-000168f0: 2020 206b 6579 7320 3d20 7365 6c66 2e66     keys = self.f
-00016900: 6b65 7973 2e6b 6579 7328 290a 2020 2020  keys.keys().    
-00016910: 2020 2020 6966 2022 4631 2220 696e 206b      if "F1" in k
-00016920: 6579 733a 0a20 2020 2020 2020 2020 2020  eys:.           
-00016930: 2073 656c 662e 4631 2e73 6574 5465 7874   self.F1.setText
-00016940: 2866 2246 313a 207b 7365 6c66 2e66 6b65  (f"F1: {self.fke
-00016950: 7973 5b27 4631 275d 5b30 5d7d 2229 0a20  ys['F1'][0]}"). 
-00016960: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016970: 4631 2e73 6574 546f 6f6c 5469 7028 7365  F1.setToolTip(se
-00016980: 6c66 2e66 6b65 7973 5b22 4631 225d 5b31  lf.fkeys["F1"][1
-00016990: 5d29 0a20 2020 2020 2020 2069 6620 2246  ]).        if "F
-000169a0: 3222 2069 6e20 6b65 7973 3a0a 2020 2020  2" in keys:.    
-000169b0: 2020 2020 2020 2020 7365 6c66 2e46 322e          self.F2.
-000169c0: 7365 7454 6578 7428 6622 4632 3a20 7b73  setText(f"F2: {s
-000169d0: 656c 662e 666b 6579 735b 2746 3227 5d5b  elf.fkeys['F2'][
-000169e0: 305d 7d22 290a 2020 2020 2020 2020 2020  0]}").          
-000169f0: 2020 7365 6c66 2e46 322e 7365 7454 6f6f    self.F2.setToo
-00016a00: 6c54 6970 2873 656c 662e 666b 6579 735b  lTip(self.fkeys[
-00016a10: 2246 3222 5d5b 315d 290a 2020 2020 2020  "F2"][1]).      
-00016a20: 2020 6966 2022 4633 2220 696e 206b 6579    if "F3" in key
-00016a30: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
-00016a40: 656c 662e 4633 2e73 6574 5465 7874 2866  elf.F3.setText(f
-00016a50: 2246 333a 207b 7365 6c66 2e66 6b65 7973  "F3: {self.fkeys
-00016a60: 5b27 4633 275d 5b30 5d7d 2229 0a20 2020  ['F3'][0]}").   
-00016a70: 2020 2020 2020 2020 2073 656c 662e 4633           self.F3
-00016a80: 2e73 6574 546f 6f6c 5469 7028 7365 6c66  .setToolTip(self
-00016a90: 2e66 6b65 7973 5b22 4633 225d 5b31 5d29  .fkeys["F3"][1])
-00016aa0: 0a20 2020 2020 2020 2069 6620 2246 3422  .        if "F4"
-00016ab0: 2069 6e20 6b65 7973 3a0a 2020 2020 2020   in keys:.      
-00016ac0: 2020 2020 2020 7365 6c66 2e46 342e 7365        self.F4.se
-00016ad0: 7454 6578 7428 6622 4634 3a20 7b73 656c  tText(f"F4: {sel
-00016ae0: 662e 666b 6579 735b 2746 3427 5d5b 305d  f.fkeys['F4'][0]
-00016af0: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
-00016b00: 7365 6c66 2e46 342e 7365 7454 6f6f 6c54  self.F4.setToolT
-00016b10: 6970 2873 656c 662e 666b 6579 735b 2246  ip(self.fkeys["F
-00016b20: 3422 5d5b 315d 290a 2020 2020 2020 2020  4"][1]).        
-00016b30: 6966 2022 4635 2220 696e 206b 6579 733a  if "F5" in keys:
-00016b40: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00016b50: 662e 4635 2e73 6574 5465 7874 2866 2246  f.F5.setText(f"F
-00016b60: 353a 207b 7365 6c66 2e66 6b65 7973 5b27  5: {self.fkeys['
-00016b70: 4635 275d 5b30 5d7d 2229 0a20 2020 2020  F5'][0]}").     
-00016b80: 2020 2020 2020 2073 656c 662e 4635 2e73         self.F5.s
-00016b90: 6574 546f 6f6c 5469 7028 7365 6c66 2e66  etToolTip(self.f
-00016ba0: 6b65 7973 5b22 4635 225d 5b31 5d29 0a20  keys["F5"][1]). 
-00016bb0: 2020 2020 2020 2069 6620 2246 3622 2069         if "F6" i
-00016bc0: 6e20 6b65 7973 3a0a 2020 2020 2020 2020  n keys:.        
-00016bd0: 2020 2020 7365 6c66 2e46 362e 7365 7454      self.F6.setT
-00016be0: 6578 7428 6622 4636 3a20 7b73 656c 662e  ext(f"F6: {self.
-00016bf0: 666b 6579 735b 2746 3627 5d5b 305d 7d22  fkeys['F6'][0]}"
-00016c00: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00016c10: 6c66 2e46 362e 7365 7454 6f6f 6c54 6970  lf.F6.setToolTip
-00016c20: 2873 656c 662e 666b 6579 735b 2246 3622  (self.fkeys["F6"
-00016c30: 5d5b 315d 290a 2020 2020 2020 2020 6966  ][1]).        if
-00016c40: 2022 4637 2220 696e 206b 6579 733a 0a20   "F7" in keys:. 
-00016c50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016c60: 4637 2e73 6574 5465 7874 2866 2246 373a  F7.setText(f"F7:
-00016c70: 207b 7365 6c66 2e66 6b65 7973 5b27 4637   {self.fkeys['F7
-00016c80: 275d 5b30 5d7d 2229 0a20 2020 2020 2020  '][0]}").       
-00016c90: 2020 2020 2073 656c 662e 4637 2e73 6574       self.F7.set
-00016ca0: 546f 6f6c 5469 7028 7365 6c66 2e66 6b65  ToolTip(self.fke
-00016cb0: 7973 5b22 4637 225d 5b31 5d29 0a20 2020  ys["F7"][1]).   
-00016cc0: 2020 2020 2069 6620 2246 3822 2069 6e20       if "F8" in 
-00016cd0: 6b65 7973 3a0a 2020 2020 2020 2020 2020  keys:.          
-00016ce0: 2020 7365 6c66 2e46 382e 7365 7454 6578    self.F8.setTex
-00016cf0: 7428 6622 4638 3a20 7b73 656c 662e 666b  t(f"F8: {self.fk
-00016d00: 6579 735b 2746 3827 5d5b 305d 7d22 290a  eys['F8'][0]}").
-00016d10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00016d20: 2e46 382e 7365 7454 6f6f 6c54 6970 2873  .F8.setToolTip(s
-00016d30: 656c 662e 666b 6579 735b 2246 3822 5d5b  elf.fkeys["F8"][
-00016d40: 315d 290a 2020 2020 2020 2020 6966 2022  1]).        if "
-00016d50: 4639 2220 696e 206b 6579 733a 0a20 2020  F9" in keys:.   
-00016d60: 2020 2020 2020 2020 2073 656c 662e 4639           self.F9
-00016d70: 2e73 6574 5465 7874 2866 2246 393a 207b  .setText(f"F9: {
-00016d80: 7365 6c66 2e66 6b65 7973 5b27 4639 275d  self.fkeys['F9']
-00016d90: 5b30 5d7d 2229 0a20 2020 2020 2020 2020  [0]}").         
-00016da0: 2020 2073 656c 662e 4639 2e73 6574 546f     self.F9.setTo
-00016db0: 6f6c 5469 7028 7365 6c66 2e66 6b65 7973  olTip(self.fkeys
-00016dc0: 5b22 4639 225d 5b31 5d29 0a20 2020 2020  ["F9"][1]).     
-00016dd0: 2020 2069 6620 2246 3130 2220 696e 206b     if "F10" in k
-00016de0: 6579 733a 0a20 2020 2020 2020 2020 2020  eys:.           
-00016df0: 2073 656c 662e 4631 302e 7365 7454 6578   self.F10.setTex
-00016e00: 7428 6622 4631 303a 207b 7365 6c66 2e66  t(f"F10: {self.f
-00016e10: 6b65 7973 5b27 4631 3027 5d5b 305d 7d22  keys['F10'][0]}"
-00016e20: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00016e30: 6c66 2e46 3130 2e73 6574 546f 6f6c 5469  lf.F10.setToolTi
-00016e40: 7028 7365 6c66 2e66 6b65 7973 5b22 4631  p(self.fkeys["F1
-00016e50: 3022 5d5b 315d 290a 2020 2020 2020 2020  0"][1]).        
-00016e60: 6966 2022 4631 3122 2069 6e20 6b65 7973  if "F11" in keys
-00016e70: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00016e80: 6c66 2e46 3131 2e73 6574 5465 7874 2866  lf.F11.setText(f
-00016e90: 2246 3131 3a20 7b73 656c 662e 666b 6579  "F11: {self.fkey
-00016ea0: 735b 2746 3131 275d 5b30 5d7d 2229 0a20  s['F11'][0]}"). 
-00016eb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016ec0: 4631 312e 7365 7454 6f6f 6c54 6970 2873  F11.setToolTip(s
-00016ed0: 656c 662e 666b 6579 735b 2246 3131 225d  elf.fkeys["F11"]
-00016ee0: 5b31 5d29 0a20 2020 2020 2020 2069 6620  [1]).        if 
-00016ef0: 2246 3132 2220 696e 206b 6579 733a 0a20  "F12" in keys:. 
-00016f00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00016f10: 4631 322e 7365 7454 6578 7428 6622 4631  F12.setText(f"F1
-00016f20: 323a 207b 7365 6c66 2e66 6b65 7973 5b27  2: {self.fkeys['
-00016f30: 4631 3227 5d5b 305d 7d22 290a 2020 2020  F12'][0]}").    
-00016f40: 2020 2020 2020 2020 7365 6c66 2e46 3132          self.F12
-00016f50: 2e73 6574 546f 6f6c 5469 7028 7365 6c66  .setToolTip(self
-00016f60: 2e66 6b65 7973 5b22 4631 3222 5d5b 315d  .fkeys["F12"][1]
-00016f70: 290a 0a20 2020 2064 6566 2067 656e 6572  )..    def gener
-00016f80: 6174 655f 6164 6966 2873 656c 6629 3a0a  ate_adif(self):.
-00016f90: 2020 2020 2020 2020 2222 2247 656e 6572          """Gener
-00016fa0: 6174 6520 4144 4946 2222 220a 2020 2020  ate ADIF""".    
-00016fb0: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-00016fc0: 2822 2a2a 2a2a 2a2a 4144 4946 2a2a 2a2a  ("******ADIF****
-00016fd0: 2a22 290a 2020 2020 2020 2020 7365 6c66  *").        self
-00016fe0: 2e63 6f6e 7465 7374 2e61 6469 6628 7365  .contest.adif(se
-00016ff0: 6c66 290a 0a20 2020 2064 6566 2067 656e  lf)..    def gen
-00017000: 6572 6174 655f 6361 6272 696c 6c6f 2873  erate_cabrillo(s
-00017010: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
-00017020: 2247 656e 6572 6174 6573 2043 6162 7269  "Generates Cabri
-00017030: 6c6c 6f20 6669 6c65 2e20 4d61 7962 652e  llo file. Maybe.
-00017040: 2222 220a 2020 2020 2020 2020 2320 6874  """.        # ht
-00017050: 7470 733a 2f2f 7777 772e 6371 7770 782e  tps://www.cqwpx.
-00017060: 636f 6d2f 6361 6272 696c 6c6f 2e68 746d  com/cabrillo.htm
-00017070: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-00017080: 6465 6275 6728 222a 2a2a 2a2a 2a43 6162  debug("******Cab
-00017090: 7269 6c6c 6f2a 2a2a 2a2a 2229 0a20 2020  rillo*****").   
-000170a0: 2020 2020 2073 656c 662e 636f 6e74 6573       self.contes
-000170b0: 742e 6361 6272 696c 6c6f 2873 656c 6629  t.cabrillo(self)
-000170c0: 0a0a 0a64 6566 206c 6f61 645f 666f 6e74  ...def load_font
-000170d0: 735f 6672 6f6d 5f64 6972 2864 6972 6563  s_from_dir(direc
-000170e0: 746f 7279 3a20 7374 7229 202d 3e20 7365  tory: str) -> se
-000170f0: 743a 0a20 2020 2022 2222 0a20 2020 2057  t:.    """.    W
-00017100: 656c 6c20 6974 206c 6f61 6473 2066 6f6e  ell it loads fon
-00017110: 7473 2066 726f 6d20 6120 6469 7265 6374  ts from a direct
-00017120: 6f72 792e 2e2e 0a20 2020 2022 2222 0a20  ory....    """. 
-00017130: 2020 2066 6f6e 745f 6661 6d69 6c69 6573     font_families
-00017140: 203d 2073 6574 2829 0a20 2020 2066 6f72   = set().    for
-00017150: 205f 6669 2069 6e20 5144 6972 2864 6972   _fi in QDir(dir
-00017160: 6563 746f 7279 292e 656e 7472 7949 6e66  ectory).entryInf
-00017170: 6f4c 6973 7428 5b22 2a2e 7474 6622 2c20  oList(["*.ttf", 
-00017180: 222a 2e77 6f66 6622 2c20 222a 2e77 6f66  "*.woff", "*.wof
-00017190: 6632 225d 293a 0a20 2020 2020 2020 205f  f2"]):.        _
-000171a0: 6964 203d 2051 466f 6e74 4461 7461 6261  id = QFontDataba
-000171b0: 7365 2e61 6464 4170 706c 6963 6174 696f  se.addApplicatio
-000171c0: 6e46 6f6e 7428 5f66 692e 6162 736f 6c75  nFont(_fi.absolu
-000171d0: 7465 4669 6c65 5061 7468 2829 290a 2020  teFilePath()).  
-000171e0: 2020 2020 2020 666f 6e74 5f66 616d 696c        font_famil
-000171f0: 6965 7320 7c3d 2073 6574 2851 466f 6e74  ies |= set(QFont
-00017200: 4461 7461 6261 7365 2e61 7070 6c69 6361  Database.applica
-00017210: 7469 6f6e 466f 6e74 4661 6d69 6c69 6573  tionFontFamilies
-00017220: 285f 6964 2929 0a20 2020 2072 6574 7572  (_id)).    retur
-00017230: 6e20 666f 6e74 5f66 616d 696c 6965 730a  n font_families.
-00017240: 0a0a 6465 6620 696e 7374 616c 6c5f 6963  ..def install_ic
-00017250: 6f6e 7328 293a 0a20 2020 2022 2222 496e  ons():.    """In
-00017260: 7374 616c 6c20 6963 6f6e 7322 2222 0a20  stall icons""". 
-00017270: 2020 206f 732e 7379 7374 656d 280a 2020     os.system(.  
-00017280: 2020 2020 2020 2278 6467 2d69 636f 6e2d        "xdg-icon-
-00017290: 7265 736f 7572 6365 2069 6e73 7461 6c6c  resource install
-000172a0: 202d 2d73 697a 6520 3332 202d 2d63 6f6e   --size 32 --con
-000172b0: 7465 7874 2061 7070 7320 2d2d 6d6f 6465  text apps --mode
-000172c0: 2075 7365 7220 220a 2020 2020 2020 2020   user ".        
-000172d0: 6622 7b57 4f52 4b49 4e47 5f50 4154 487d  f"{WORKING_PATH}
-000172e0: 2f64 6174 612f 6b36 6774 652e 6e6f 7431  /data/k6gte.not1
-000172f0: 6d6d 2d33 322e 706e 6720 6b36 6774 652d  mm-32.png k6gte-
-00017300: 6e6f 7431 6d6d 220a 2020 2020 290a 2020  not1mm".    ).  
-00017310: 2020 6f73 2e73 7973 7465 6d28 0a20 2020    os.system(.   
-00017320: 2020 2020 2022 7864 672d 6963 6f6e 2d72       "xdg-icon-r
-00017330: 6573 6f75 7263 6520 696e 7374 616c 6c20  esource install 
-00017340: 2d2d 7369 7a65 2036 3420 2d2d 636f 6e74  --size 64 --cont
-00017350: 6578 7420 6170 7073 202d 2d6d 6f64 6520  ext apps --mode 
-00017360: 7573 6572 2022 0a20 2020 2020 2020 2066  user ".        f
-00017370: 227b 574f 524b 494e 475f 5041 5448 7d2f  "{WORKING_PATH}/
-00017380: 6461 7461 2f6b 3667 7465 2e6e 6f74 316d  data/k6gte.not1m
-00017390: 6d2d 3634 2e70 6e67 206b 3667 7465 2d6e  m-64.png k6gte-n
-000173a0: 6f74 316d 6d22 0a20 2020 2029 0a20 2020  ot1mm".    ).   
-000173b0: 206f 732e 7379 7374 656d 280a 2020 2020   os.system(.    
-000173c0: 2020 2020 2278 6467 2d69 636f 6e2d 7265      "xdg-icon-re
-000173d0: 736f 7572 6365 2069 6e73 7461 6c6c 202d  source install -
-000173e0: 2d73 697a 6520 3132 3820 2d2d 636f 6e74  -size 128 --cont
-000173f0: 6578 7420 6170 7073 202d 2d6d 6f64 6520  ext apps --mode 
-00017400: 7573 6572 2022 0a20 2020 2020 2020 2066  user ".        f
-00017410: 227b 574f 524b 494e 475f 5041 5448 7d2f  "{WORKING_PATH}/
-00017420: 6461 7461 2f6b 3667 7465 2e6e 6f74 316d  data/k6gte.not1m
-00017430: 6d2d 3132 382e 706e 6720 6b36 6774 652d  m-128.png k6gte-
-00017440: 6e6f 7431 6d6d 220a 2020 2020 290a 2020  not1mm".    ).  
-00017450: 2020 6f73 2e73 7973 7465 6d28 6622 7864    os.system(f"xd
-00017460: 672d 6465 736b 746f 702d 6d65 6e75 2069  g-desktop-menu i
-00017470: 6e73 7461 6c6c 207b 574f 524b 494e 475f  nstall {WORKING_
-00017480: 5041 5448 7d2f 6461 7461 2f6b 3667 7465  PATH}/data/k6gte
-00017490: 2d6e 6f74 316d 6d2e 6465 736b 746f 7022  -not1mm.desktop"
-000174a0: 290a 0a0a 6465 6620 646f 696d 7028 6d6f  )...def doimp(mo
-000174b0: 646e 616d 6529 3a0a 2020 2020 2222 2272  dname):.    """r
-000174c0: 6574 7572 6e20 6d6f 6475 6c65 2070 6174  eturn module pat
-000174d0: 6822 2222 0a20 2020 2072 6574 7572 6e20  h""".    return 
-000174e0: 696d 706f 7274 6c69 622e 696d 706f 7274  importlib.import
-000174f0: 5f6d 6f64 756c 6528 6622 6e6f 7431 6d6d  _module(f"not1mm
-00017500: 2e70 6c75 6769 6e73 2e7b 6d6f 646e 616d  .plugins.{modnam
-00017510: 657d 2229 0a0a 0a64 6566 2072 756e 2829  e}")...def run()
-00017520: 3a0a 2020 2020 2222 220a 2020 2020 4d61  :.    """.    Ma
-00017530: 696e 2045 6e74 7279 0a20 2020 2022 2222  in Entry.    """
-00017540: 0a20 2020 2069 6e73 7461 6c6c 5f69 636f  .    install_ico
-00017550: 6e73 2829 0a20 2020 2074 696d 6572 2e73  ns().    timer.s
-00017560: 7461 7274 2832 3530 290a 2020 2020 7379  tart(250).    sy
-00017570: 732e 6578 6974 2861 7070 2e65 7865 6328  s.exit(app.exec(
-00017580: 2929 0a0a 0a6c 6f67 6765 7220 3d20 6c6f  ))...logger = lo
-00017590: 6767 696e 672e 6765 744c 6f67 6765 7228  gging.getLogger(
-000175a0: 225f 5f6d 6169 6e5f 5f22 290a 6861 6e64  "__main__").hand
-000175b0: 6c65 7220 3d20 6c6f 6767 696e 672e 5374  ler = logging.St
-000175c0: 7265 616d 4861 6e64 6c65 7228 290a 666f  reamHandler().fo
-000175d0: 726d 6174 7465 7220 3d20 6c6f 6767 696e  rmatter = loggin
-000175e0: 672e 466f 726d 6174 7465 7228 0a20 2020  g.Formatter(.   
-000175f0: 2064 6174 6566 6d74 3d22 2548 3a25 4d3a   datefmt="%H:%M:
-00017600: 2553 222c 0a20 2020 2066 6d74 3d22 5b25  %S",.    fmt="[%
-00017610: 2861 7363 7469 6d65 2973 5d20 2528 6c65  (asctime)s] %(le
-00017620: 7665 6c6e 616d 6529 7320 2528 6d6f 6475  velname)s %(modu
-00017630: 6c65 2973 202d 2025 2866 756e 634e 616d  le)s - %(funcNam
-00017640: 6529 7320 4c69 6e65 2025 286c 696e 656e  e)s Line %(linen
-00017650: 6f29 643a 2025 286d 6573 7361 6765 2973  o)d: %(message)s
-00017660: 222c 0a29 0a68 616e 646c 6572 2e73 6574  ",.).handler.set
-00017670: 466f 726d 6174 7465 7228 666f 726d 6174  Formatter(format
-00017680: 7465 7229 0a6c 6f67 6765 722e 6164 6448  ter).logger.addH
-00017690: 616e 646c 6572 2868 616e 646c 6572 290a  andler(handler).
-000176a0: 0a42 4554 415f 5445 5354 203d 2046 616c  .BETA_TEST = Fal
-000176b0: 7365 0a69 6620 5061 7468 2822 2e2f 6265  se.if Path("./be
-000176c0: 7461 7465 7374 2229 2e65 7869 7374 7328  tatest").exists(
-000176d0: 293a 0a20 2020 2042 4554 415f 5445 5354  ):.    BETA_TEST
-000176e0: 203d 2054 7275 650a 0a69 6620 5061 7468   = True..if Path
-000176f0: 2822 2e2f 6465 6275 6722 292e 6578 6973  ("./debug").exis
-00017700: 7473 2829 3a0a 2020 2020 6c6f 6767 6572  ts():.    logger
-00017710: 2e73 6574 4c65 7665 6c28 6c6f 6767 696e  .setLevel(loggin
-00017720: 672e 4445 4255 4729 0a20 2020 206c 6f67  g.DEBUG).    log
-00017730: 6765 722e 6465 6275 6728 2264 6562 7567  ger.debug("debug
-00017740: 6769 6e67 206f 6e22 290a 656c 7365 3a0a  ging on").else:.
-00017750: 2020 2020 6c6f 6767 6572 2e73 6574 4c65      logger.setLe
-00017760: 7665 6c28 6c6f 6767 696e 672e 5741 524e  vel(logging.WARN
-00017770: 494e 4729 0a20 2020 206c 6f67 6765 722e  ING).    logger.
-00017780: 7761 726e 696e 6728 2264 6562 7567 6769  warning("debuggi
-00017790: 6e67 206f 6666 2229 0a0a 6170 7020 3d20  ng off")..app = 
-000177a0: 5174 5769 6467 6574 732e 5141 7070 6c69  QtWidgets.QAppli
-000177b0: 6361 7469 6f6e 2873 7973 2e61 7267 7629  cation(sys.argv)
-000177c0: 0a61 7070 2e73 6574 5374 796c 6528 2241  .app.setStyle("A
-000177d0: 6477 6169 7461 2d44 6172 6b22 290a 666f  dwaita-Dark").fo
-000177e0: 6e74 5f70 6174 6820 3d20 574f 524b 494e  nt_path = WORKIN
-000177f0: 475f 5041 5448 202b 2022 2f64 6174 6122  G_PATH + "/data"
-00017800: 0a66 616d 696c 6965 7320 3d20 6c6f 6164  .families = load
-00017810: 5f66 6f6e 7473 5f66 726f 6d5f 6469 7228  _fonts_from_dir(
-00017820: 6f73 2e66 7370 6174 6828 666f 6e74 5f70  os.fspath(font_p
-00017830: 6174 6829 290a 6c6f 6767 6572 2e69 6e66  ath)).logger.inf
-00017840: 6f28 6661 6d69 6c69 6573 290a 7769 6e64  o(families).wind
-00017850: 6f77 203d 204d 6169 6e57 696e 646f 7728  ow = MainWindow(
-00017860: 290a 6865 6967 6874 203d 2077 696e 646f  ).height = windo
-00017870: 772e 7072 6566 2e67 6574 2822 7769 6e64  w.pref.get("wind
-00017880: 6f77 5f68 6569 6768 7422 2c20 3330 3029  ow_height", 300)
-00017890: 0a77 6964 7468 203d 2077 696e 646f 772e  .width = window.
-000178a0: 7072 6566 2e67 6574 2822 7769 6e64 6f77  pref.get("window
-000178b0: 5f77 6964 7468 222c 2037 3030 290a 7820  _width", 700).x 
-000178c0: 3d20 7769 6e64 6f77 2e70 7265 662e 6765  = window.pref.ge
-000178d0: 7428 2277 696e 646f 775f 7822 2c20 2d31  t("window_x", -1
-000178e0: 290a 7920 3d20 7769 6e64 6f77 2e70 7265  ).y = window.pre
-000178f0: 662e 6765 7428 2277 696e 646f 775f 7922  f.get("window_y"
-00017900: 2c20 2d31 290a 7769 6e64 6f77 2e73 6574  , -1).window.set
-00017910: 4765 6f6d 6574 7279 2878 2c20 792c 2077  Geometry(x, y, w
-00017920: 6964 7468 2c20 6865 6967 6874 290a 7769  idth, height).wi
-00017930: 6e64 6f77 2e63 616c 6c73 6967 6e2e 7365  ndow.callsign.se
-00017940: 7446 6f63 7573 2829 0a77 696e 646f 772e  tFocus().window.
-00017950: 7368 6f77 2829 0a74 696d 6572 203d 2051  show().timer = Q
-00017960: 7443 6f72 652e 5154 696d 6572 2829 0a74  tCore.QTimer().t
-00017970: 696d 6572 2e74 696d 656f 7574 2e63 6f6e  imer.timeout.con
-00017980: 6e65 6374 2877 696e 646f 772e 706f 6c6c  nect(window.poll
-00017990: 5f72 6164 696f 290a 0a69 6620 5f5f 6e61  _radio)..if __na
-000179a0: 6d65 5f5f 203d 3d20 225f 5f6d 6169 6e5f  me__ == "__main_
-000179b0: 5f22 3a0a 2020 2020 7275 6e28 290a       _":.    run().
+00012de0: 2020 2020 7365 6c66 2e6f 7468 6572 5f32      self.other_2
+00012df0: 2e73 6574 5465 7874 2873 7472 6970 7065  .setText(strippe
+00012e00: 645f 7465 7874 290a 2020 2020 2020 2020  d_text).        
+00012e10: 2020 2020 2020 2020 2020 2020 2320 7365              # se
+00012e20: 6c66 2e6f 7468 6572 5f32 2e73 6574 4375  lf.other_2.setCu
+00012e30: 7273 6f72 506f 7369 7469 6f6e 2870 6f73  rsorPosition(pos
+00012e40: 6974 696f 6e29 0a20 2020 2020 2020 2020  ition).         
+00012e50: 2020 2020 2020 2020 2020 2069 6620 2220             if " 
+00012e60: 2220 696e 2074 6578 743a 0a20 2020 2020  " in text:.     
+00012e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e80: 2020 206e 6578 745f 7461 6220 3d20 7365     next_tab = se
+00012e90: 6c66 2e74 6162 5f6e 6578 742e 6765 7428  lf.tab_next.get(
+00012ea0: 7365 6c66 2e6f 7468 6572 5f32 290a 2020  self.other_2).  
+00012eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ec0: 2020 2020 2020 6e65 7874 5f74 6162 2e73        next_tab.s
+00012ed0: 6574 466f 6375 7328 290a 2020 2020 2020  etFocus().      
+00012ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ef0: 2020 6e65 7874 5f74 6162 2e64 6573 656c    next_tab.desel
+00012f00: 6563 7428 290a 2020 2020 2020 2020 2020  ect().          
+00012f10: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+00012f20: 7874 5f74 6162 2e65 6e64 2846 616c 7365  xt_tab.end(False
+00012f30: 290a 0a20 2020 2064 6566 2063 616c 6c73  )..    def calls
+00012f40: 6967 6e5f 6368 616e 6765 6428 7365 6c66  ign_changed(self
+00012f50: 293a 0a20 2020 2020 2020 2022 2222 4361  ):.        """Ca
+00012f60: 6c6c 6564 2077 6865 6e20 7465 7874 2069  lled when text i
+00012f70: 6e20 7468 6520 6361 6c6c 7369 676e 2066  n the callsign f
+00012f80: 6965 6c64 2068 6173 2063 6861 6e67 6564  ield has changed
+00012f90: 2222 220a 2020 2020 2020 2020 7465 7874  """.        text
+00012fa0: 203d 2073 656c 662e 6361 6c6c 7369 676e   = self.callsign
+00012fb0: 2e74 6578 7428 290a 2020 2020 2020 2020  .text().        
+00012fc0: 7465 7874 203d 2074 6578 742e 7570 7065  text = text.uppe
+00012fd0: 7228 290a 2020 2020 2020 2020 706f 7369  r().        posi
+00012fe0: 7469 6f6e 203d 2073 656c 662e 6361 6c6c  tion = self.call
+00012ff0: 7369 676e 2e63 7572 736f 7250 6f73 6974  sign.cursorPosit
+00013000: 696f 6e28 290a 2020 2020 2020 2020 7374  ion().        st
+00013010: 7269 7070 6564 5f74 6578 7420 3d20 7465  ripped_text = te
+00013020: 7874 2e73 7472 6970 2829 2e72 6570 6c61  xt.strip().repla
+00013030: 6365 2822 2022 2c20 2222 290a 2020 2020  ce(" ", "").    
+00013040: 2020 2020 7365 6c66 2e63 616c 6c73 6967      self.callsig
+00013050: 6e2e 7365 7454 6578 7428 7374 7269 7070  n.setText(stripp
+00013060: 6564 5f74 6578 7429 0a20 2020 2020 2020  ed_text).       
+00013070: 2073 656c 662e 6361 6c6c 7369 676e 2e73   self.callsign.s
+00013080: 6574 4375 7273 6f72 506f 7369 7469 6f6e  etCursorPosition
+00013090: 2870 6f73 6974 696f 6e29 0a20 2020 2020  (position).     
+000130a0: 2020 2072 6573 756c 7473 203d 2073 656c     results = sel
+000130b0: 662e 6d73 6370 2e73 7570 6572 5f63 6865  f.mscp.super_che
+000130c0: 636b 2873 7472 6970 7065 645f 7465 7874  ck(stripped_text
+000130d0: 290a 2020 2020 2020 2020 6c6f 6767 6572  ).        logger
+000130e0: 2e64 6562 7567 2866 227b 7265 7375 6c74  .debug(f"{result
+000130f0: 737d 2229 0a0a 2020 2020 2020 2020 6966  s}")..        if
+00013100: 2022 2022 2069 6e20 7465 7874 3a0a 2020   " " in text:.  
+00013110: 2020 2020 2020 2020 2020 6966 2073 7472            if str
+00013120: 6970 7065 645f 7465 7874 203d 3d20 2243  ipped_text == "C
+00013130: 5722 3a0a 2020 2020 2020 2020 2020 2020  W":.            
+00013140: 2020 2020 7365 6c66 2e73 6574 6d6f 6465      self.setmode
+00013150: 2822 4357 2229 0a20 2020 2020 2020 2020  ("CW").         
+00013160: 2020 2020 2020 2073 656c 662e 7261 6469         self.radi
+00013170: 6f5f 7374 6174 655b 226d 6f64 6522 5d20  o_state["mode"] 
+00013180: 3d20 2243 5722 0a20 2020 2020 2020 2020  = "CW".         
+00013190: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+000131a0: 6967 5f63 6f6e 7472 6f6c 3a0a 2020 2020  ig_control:.    
+000131b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000131c0: 6966 2073 656c 662e 7269 675f 636f 6e74  if self.rig_cont
+000131d0: 726f 6c2e 6f6e 6c69 6e65 3a0a 2020 2020  rol.online:.    
+000131e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000131f0: 2020 2020 7365 6c66 2e72 6967 5f63 6f6e      self.rig_con
+00013200: 7472 6f6c 2e73 6574 5f6d 6f64 6528 2243  trol.set_mode("C
+00013210: 5722 290a 2020 2020 2020 2020 2020 2020  W").            
+00013220: 2020 2020 6261 6e64 203d 2067 6574 6261      band = getba
+00013230: 6e64 2873 7472 2873 656c 662e 7261 6469  nd(str(self.radi
+00013240: 6f5f 7374 6174 652e 6765 7428 2276 666f  o_state.get("vfo
+00013250: 6122 2c20 2230 2e30 2229 2929 0a20 2020  a", "0.0"))).   
+00013260: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00013270: 662e 7365 745f 6261 6e64 5f69 6e64 6963  f.set_band_indic
+00013280: 6174 6f72 2862 616e 6429 0a20 2020 2020  ator(band).     
+00013290: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000132a0: 7365 745f 7769 6e64 6f77 5f74 6974 6c65  set_window_title
+000132b0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+000132c0: 2020 2073 656c 662e 636c 6561 7269 6e70     self.clearinp
+000132d0: 7574 7328 290a 2020 2020 2020 2020 2020  uts().          
+000132e0: 2020 2020 2020 7365 6c66 2e72 6561 645f        self.read_
+000132f0: 6377 5f6d 6163 726f 7328 290a 2020 2020  cw_macros().    
+00013300: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00013310: 726e 0a20 2020 2020 2020 2020 2020 2069  rn.            i
+00013320: 6620 7374 7269 7070 6564 5f74 6578 7420  f stripped_text 
+00013330: 3d3d 2022 5254 5459 223a 0a20 2020 2020  == "RTTY":.     
+00013340: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00013350: 7365 746d 6f64 6528 2252 5454 5922 290a  setmode("RTTY").
+00013360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013370: 6966 2073 656c 662e 7269 675f 636f 6e74  if self.rig_cont
+00013380: 726f 6c3a 0a20 2020 2020 2020 2020 2020  rol:.           
+00013390: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+000133a0: 2e72 6967 5f63 6f6e 7472 6f6c 2e6f 6e6c  .rig_control.onl
+000133b0: 696e 653a 0a20 2020 2020 2020 2020 2020  ine:.           
+000133c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000133d0: 662e 7269 675f 636f 6e74 726f 6c2e 7365  f.rig_control.se
+000133e0: 745f 6d6f 6465 2822 5254 5459 2229 0a20  t_mode("RTTY"). 
+000133f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013400: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00013410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013420: 2073 656c 662e 7261 6469 6f5f 7374 6174   self.radio_stat
+00013430: 655b 226d 6f64 6522 5d20 3d20 2252 5454  e["mode"] = "RTT
+00013440: 5922 0a20 2020 2020 2020 2020 2020 2020  Y".             
+00013450: 2020 2062 616e 6420 3d20 6765 7462 616e     band = getban
+00013460: 6428 7374 7228 7365 6c66 2e72 6164 696f  d(str(self.radio
+00013470: 5f73 7461 7465 2e67 6574 2822 7666 6f61  _state.get("vfoa
+00013480: 222c 2022 302e 3022 2929 290a 2020 2020  ", "0.0"))).    
+00013490: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000134a0: 2e73 6574 5f62 616e 645f 696e 6469 6361  .set_band_indica
+000134b0: 746f 7228 6261 6e64 290a 2020 2020 2020  tor(band).      
+000134c0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+000134d0: 6574 5f77 696e 646f 775f 7469 746c 6528  et_window_title(
+000134e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000134f0: 2020 7365 6c66 2e63 6c65 6172 696e 7075    self.clearinpu
+00013500: 7473 2829 0a20 2020 2020 2020 2020 2020  ts().           
+00013510: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+00013520: 2020 2020 2020 2020 6966 2073 7472 6970          if strip
+00013530: 7065 645f 7465 7874 203d 3d20 2253 5342  ped_text == "SSB
+00013540: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+00013550: 2020 2073 656c 662e 7365 746d 6f64 6528     self.setmode(
+00013560: 2253 5342 2229 0a20 2020 2020 2020 2020  "SSB").         
+00013570: 2020 2020 2020 2069 6620 696e 7428 7365         if int(se
+00013580: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
+00013590: 6574 2822 7666 6f61 222c 2030 2929 203e  et("vfoa", 0)) >
+000135a0: 2031 3030 3030 3030 303a 0a20 2020 2020   10000000:.     
+000135b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000135c0: 656c 662e 7261 6469 6f5f 7374 6174 655b  elf.radio_state[
+000135d0: 226d 6f64 6522 5d20 3d20 2255 5342 220a  "mode"] = "USB".
+000135e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000135f0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00013600: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+00013610: 6164 696f 5f73 7461 7465 5b22 6d6f 6465  adio_state["mode
+00013620: 225d 203d 2022 4c53 4222 0a20 2020 2020  "] = "LSB".     
+00013630: 2020 2020 2020 2020 2020 2062 616e 6420             band 
+00013640: 3d20 6765 7462 616e 6428 7374 7228 7365  = getband(str(se
+00013650: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
+00013660: 6574 2822 7666 6f61 222c 2022 302e 3022  et("vfoa", "0.0"
+00013670: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
+00013680: 2020 2020 7365 6c66 2e73 6574 5f62 616e      self.set_ban
+00013690: 645f 696e 6469 6361 746f 7228 6261 6e64  d_indicator(band
+000136a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000136b0: 2020 7365 6c66 2e73 6574 5f77 696e 646f    self.set_windo
+000136c0: 775f 7469 746c 6528 290a 2020 2020 2020  w_title().      
+000136d0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+000136e0: 662e 7269 675f 636f 6e74 726f 6c3a 0a20  f.rig_control:. 
+000136f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013700: 2020 2073 656c 662e 7269 675f 636f 6e74     self.rig_cont
+00013710: 726f 6c2e 7365 745f 6d6f 6465 2873 656c  rol.set_mode(sel
+00013720: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
+00013730: 7428 226d 6f64 6522 2929 0a20 2020 2020  t("mode")).     
+00013740: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00013750: 636c 6561 7269 6e70 7574 7328 290a 2020  clearinputs().  
+00013760: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00013770: 6c66 2e72 6561 645f 6377 5f6d 6163 726f  lf.read_cw_macro
+00013780: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
+00013790: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+000137a0: 2020 2020 2020 2069 6620 7374 7269 7070         if stripp
+000137b0: 6564 5f74 6578 7420 3d3d 2022 4f50 4f4e  ed_text == "OPON
+000137c0: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+000137d0: 2020 2073 656c 662e 6765 745f 6f70 6f6e     self.get_opon
+000137e0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+000137f0: 2020 2073 656c 662e 636c 6561 7269 6e70     self.clearinp
+00013800: 7574 7328 290a 2020 2020 2020 2020 2020  uts().          
+00013810: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+00013820: 2020 2020 2020 2020 2069 6620 7374 7269           if stri
+00013830: 7070 6564 5f74 6578 7420 3d3d 2022 4845  pped_text == "HE
+00013840: 4c50 223a 0a20 2020 2020 2020 2020 2020  LP":.           
+00013850: 2020 2020 2073 656c 662e 7368 6f77 5f68       self.show_h
+00013860: 656c 705f 6469 616c 6f67 2829 0a20 2020  elp_dialog().   
+00013870: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00013880: 662e 636c 6561 7269 6e70 7574 7328 290a  f.clearinputs().
+00013890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000138a0: 7265 7475 726e 0a20 2020 2020 2020 2020  return.         
+000138b0: 2020 2069 6620 7374 7269 7070 6564 5f74     if stripped_t
+000138c0: 6578 7420 3d3d 2022 5445 5354 223a 0a20  ext == "TEST":. 
+000138d0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000138e0: 6573 756c 7420 3d20 7365 6c66 2e64 6174  esult = self.dat
+000138f0: 6162 6173 652e 6765 745f 6361 6c6c 735f  abase.get_calls_
+00013900: 616e 645f 6261 6e64 7328 290a 2020 2020  and_bands().    
+00013910: 2020 2020 2020 2020 2020 2020 636d 6420              cmd 
+00013920: 3d20 7b7d 0a20 2020 2020 2020 2020 2020  = {}.           
+00013930: 2020 2020 2063 6d64 5b22 636d 6422 5d20       cmd["cmd"] 
+00013940: 3d20 2257 4f52 4b45 4422 0a20 2020 2020  = "WORKED".     
+00013950: 2020 2020 2020 2020 2020 2063 6d64 5b22             cmd["
+00013960: 7374 6174 696f 6e22 5d20 3d20 706c 6174  station"] = plat
+00013970: 666f 726d 2e6e 6f64 6528 290a 2020 2020  form.node().    
+00013980: 2020 2020 2020 2020 2020 2020 636d 645b              cmd[
+00013990: 2277 6f72 6b65 6422 5d20 3d20 7265 7375  "worked"] = resu
+000139a0: 6c74 0a20 2020 2020 2020 2020 2020 2020  lt.             
+000139b0: 2020 2073 656c 662e 6d75 6c74 6963 6173     self.multicas
+000139c0: 745f 696e 7465 7266 6163 652e 7365 6e64  t_interface.send
+000139d0: 5f61 735f 6a73 6f6e 2863 6d64 290a 2020  _as_json(cmd).  
+000139e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000139f0: 6c66 2e63 6c65 6172 696e 7075 7473 2829  lf.clearinputs()
+00013a00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013a10: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+00013a20: 2020 2020 6966 2073 656c 662e 6973 5f66      if self.is_f
+00013a30: 6c6f 6174 6162 6c65 2873 7472 6970 7065  loatable(strippe
+00013a40: 645f 7465 7874 293a 0a20 2020 2020 2020  d_text):.       
+00013a50: 2020 2020 2020 2020 2076 666f 203d 2066           vfo = f
+00013a60: 6c6f 6174 2873 7472 6970 7065 645f 7465  loat(stripped_te
+00013a70: 7874 290a 2020 2020 2020 2020 2020 2020  xt).            
+00013a80: 2020 2020 7666 6f20 3d20 696e 7428 7666      vfo = int(vf
+00013a90: 6f20 2a20 3130 3030 290a 2020 2020 2020  o * 1000).      
+00013aa0: 2020 2020 2020 2020 2020 6261 6e64 203d            band =
+00013ab0: 2067 6574 6261 6e64 2873 7472 2876 666f   getband(str(vfo
+00013ac0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+00013ad0: 2020 2073 656c 662e 7365 745f 6261 6e64     self.set_band
+00013ae0: 5f69 6e64 6963 6174 6f72 2862 616e 6429  _indicator(band)
+00013af0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013b00: 2023 2073 656c 662e 636f 6e74 6163 745b   # self.contact[
+00013b10: 2242 616e 6422 5d20 3d20 6765 745f 6c6f  "Band"] = get_lo
+00013b20: 6767 6564 5f62 616e 6428 7374 7228 7365  gged_band(str(se
+00013b30: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
+00013b40: 6574 2822 7666 6f61 222c 2030 2e30 2929  et("vfoa", 0.0))
+00013b50: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00013b60: 2020 7365 6c66 2e72 6164 696f 5f73 7461    self.radio_sta
+00013b70: 7465 5b22 7666 6f61 225d 203d 2076 666f  te["vfoa"] = vfo
+00013b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013b90: 2073 656c 662e 7261 6469 6f5f 7374 6174   self.radio_stat
+00013ba0: 655b 2262 616e 6422 5d20 3d20 6261 6e64  e["band"] = band
+00013bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013bc0: 2073 656c 662e 636f 6e74 6163 745b 2242   self.contact["B
+00013bd0: 616e 6422 5d20 3d20 6765 745f 6c6f 6767  and"] = get_logg
+00013be0: 6564 5f62 616e 6428 7374 7228 7666 6f29  ed_band(str(vfo)
+00013bf0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00013c00: 2020 7365 6c66 2e73 6574 5f77 696e 646f    self.set_windo
+00013c10: 775f 7469 746c 6528 290a 2020 2020 2020  w_title().      
+00013c20: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00013c30: 6c65 6172 696e 7075 7473 2829 0a20 2020  learinputs().   
+00013c40: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00013c50: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
+00013c60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00013c70: 2020 2020 2020 7365 6c66 2e72 6967 5f63        self.rig_c
+00013c80: 6f6e 7472 6f6c 2e73 6574 5f76 666f 2876  ontrol.set_vfo(v
+00013c90: 666f 290a 2020 2020 2020 2020 2020 2020  fo).            
+00013ca0: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+00013cb0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00013cc0: 6d64 203d 207b 7d0a 2020 2020 2020 2020  md = {}.        
+00013cd0: 2020 2020 2020 2020 636d 645b 2263 6d64          cmd["cmd
+00013ce0: 225d 203d 2022 5241 4449 4f5f 5354 4154  "] = "RADIO_STAT
+00013cf0: 4522 0a20 2020 2020 2020 2020 2020 2020  E".             
+00013d00: 2020 2063 6d64 5b22 7374 6174 696f 6e22     cmd["station"
+00013d10: 5d20 3d20 706c 6174 666f 726d 2e6e 6f64  ] = platform.nod
+00013d20: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+00013d30: 2020 2020 636d 645b 2262 616e 6422 5d20      cmd["band"] 
+00013d40: 3d20 6261 6e64 0a20 2020 2020 2020 2020  = band.         
+00013d50: 2020 2020 2020 2063 6d64 5b22 7666 6f61         cmd["vfoa
+00013d60: 225d 203d 2076 666f 0a20 2020 2020 2020  "] = vfo.       
+00013d70: 2020 2020 2020 2020 2073 656c 662e 6d75           self.mu
+00013d80: 6c74 6963 6173 745f 696e 7465 7266 6163  lticast_interfac
+00013d90: 652e 7365 6e64 5f61 735f 6a73 6f6e 2863  e.send_as_json(c
+00013da0: 6d64 290a 2020 2020 2020 2020 2020 2020  md).            
+00013db0: 2020 2020 7265 7475 726e 0a0a 2020 2020      return..    
+00013dc0: 2020 2020 2020 2020 7365 6c66 2e63 6865          self.che
+00013dd0: 636b 5f63 616c 6c73 6967 6e28 7374 7269  ck_callsign(stri
+00013de0: 7070 6564 5f74 6578 7429 0a20 2020 2020  pped_text).     
+00013df0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+00013e00: 6865 636b 5f64 7570 6528 7374 7269 7070  heck_dupe(stripp
+00013e10: 6564 5f74 6578 7429 3a0a 2020 2020 2020  ed_text):.      
+00013e20: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+00013e30: 7570 655f 696e 6469 6361 746f 722e 7368  upe_indicator.sh
+00013e40: 6f77 2829 0a20 2020 2020 2020 2020 2020  ow().           
+00013e50: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00013e60: 2020 2020 2020 2073 656c 662e 6475 7065         self.dupe
+00013e70: 5f69 6e64 6963 6174 6f72 2e68 6964 6528  _indicator.hide(
+00013e80: 290a 2020 2020 2020 2020 2020 2020 5f74  ).            _t
+00013e90: 6865 7468 7265 6164 203d 2074 6872 6561  hethread = threa
+00013ea0: 6469 6e67 2e54 6872 6561 6428 0a20 2020  ding.Thread(.   
+00013eb0: 2020 2020 2020 2020 2020 2020 2074 6172               tar
+00013ec0: 6765 743d 7365 6c66 2e63 6865 636b 5f63  get=self.check_c
+00013ed0: 616c 6c73 6967 6e32 2c0a 2020 2020 2020  allsign2,.      
+00013ee0: 2020 2020 2020 2020 2020 6172 6773 3d28            args=(
+00013ef0: 7465 7874 2c29 2c0a 2020 2020 2020 2020  text,),.        
+00013f00: 2020 2020 2020 2020 6461 656d 6f6e 3d54          daemon=T
+00013f10: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+00013f20: 2029 0a20 2020 2020 2020 2020 2020 205f   ).            _
+00013f30: 7468 6574 6872 6561 642e 7374 6172 7428  thethread.start(
+00013f40: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00013f50: 6c66 2e6e 6578 745f 6669 656c 642e 7365  lf.next_field.se
+00013f60: 7446 6f63 7573 2829 0a20 2020 2020 2020  tFocus().       
+00013f70: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+00013f80: 2020 2020 636d 6420 3d20 7b7d 0a20 2020      cmd = {}.   
+00013f90: 2020 2020 2063 6d64 5b22 636d 6422 5d20       cmd["cmd"] 
+00013fa0: 3d20 2243 414c 4c43 4841 4e47 4544 220a  = "CALLCHANGED".
+00013fb0: 2020 2020 2020 2020 636d 645b 2273 7461          cmd["sta
+00013fc0: 7469 6f6e 225d 203d 2070 6c61 7466 6f72  tion"] = platfor
+00013fd0: 6d2e 6e6f 6465 2829 0a20 2020 2020 2020  m.node().       
+00013fe0: 2063 6d64 5b22 6361 6c6c 225d 203d 2073   cmd["call"] = s
+00013ff0: 7472 6970 7065 645f 7465 7874 0a20 2020  tripped_text.   
+00014000: 2020 2020 2073 656c 662e 6d75 6c74 6963       self.multic
+00014010: 6173 745f 696e 7465 7266 6163 652e 7365  ast_interface.se
+00014020: 6e64 5f61 735f 6a73 6f6e 2863 6d64 290a  nd_as_json(cmd).
+00014030: 2020 2020 2020 2020 7365 6c66 2e63 6865          self.che
+00014040: 636b 5f63 616c 6c73 6967 6e28 7374 7269  ck_callsign(stri
+00014050: 7070 6564 5f74 6578 7429 0a0a 2020 2020  pped_text)..    
+00014060: 6465 6620 6368 6563 6b5f 6361 6c6c 7369  def check_callsi
+00014070: 676e 2873 656c 662c 2063 616c 6c73 6967  gn(self, callsig
+00014080: 6e29 3a0a 2020 2020 2020 2020 2222 2243  n):.        """C
+00014090: 6865 636b 2063 616c 6c20 6173 2065 6e74  heck call as ent
+000140a0: 6572 6564 2222 220a 2020 2020 2020 2020  ered""".        
+000140b0: 7265 7375 6c74 203d 2073 656c 662e 6374  result = self.ct
+000140c0: 795f 6c6f 6f6b 7570 2863 616c 6c73 6967  y_lookup(callsig
+000140d0: 6e29 0a20 2020 2020 2020 2064 6562 7567  n).        debug
+000140e0: 5f72 6573 756c 7420 3d20 6622 7b72 6573  _result = f"{res
+000140f0: 756c 747d 220a 2020 2020 2020 2020 6c6f  ult}".        lo
+00014100: 6767 6572 2e64 6562 7567 2822 2573 222c  gger.debug("%s",
+00014110: 2064 6562 7567 5f72 6573 756c 7429 0a20   debug_result). 
+00014120: 2020 2020 2020 2069 6620 7265 7375 6c74         if result
+00014130: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+00014140: 7220 6120 696e 2072 6573 756c 742e 6974  r a in result.it
+00014150: 656d 7328 293a 0a20 2020 2020 2020 2020  ems():.         
+00014160: 2020 2020 2020 2065 6e74 6974 7920 3d20         entity = 
+00014170: 615b 315d 2e67 6574 2822 656e 7469 7479  a[1].get("entity
+00014180: 222c 2022 2229 0a20 2020 2020 2020 2020  ", "").         
+00014190: 2020 2020 2020 2063 7120 3d20 615b 315d         cq = a[1]
+000141a0: 2e67 6574 2822 6371 222c 2022 2229 0a20  .get("cq", ""). 
+000141b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000141c0: 7475 203d 2061 5b31 5d2e 6765 7428 2269  tu = a[1].get("i
+000141d0: 7475 222c 2022 2229 0a20 2020 2020 2020  tu", "").       
+000141e0: 2020 2020 2020 2020 2063 6f6e 7469 6e65           contine
+000141f0: 6e74 203d 2061 5b31 5d2e 6765 7428 2263  nt = a[1].get("c
+00014200: 6f6e 7469 6e65 6e74 2229 0a20 2020 2020  ontinent").     
+00014210: 2020 2020 2020 2020 2020 206c 6174 203d             lat =
+00014220: 2066 6c6f 6174 2861 5b31 5d2e 6765 7428   float(a[1].get(
+00014230: 226c 6174 222c 2022 302e 3022 2929 0a20  "lat", "0.0")). 
+00014240: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00014250: 6f6e 203d 2066 6c6f 6174 2861 5b31 5d2e  on = float(a[1].
+00014260: 6765 7428 226c 6f6e 6722 2c20 2230 2e30  get("long", "0.0
+00014270: 2229 290a 2020 2020 2020 2020 2020 2020  ")).            
+00014280: 2020 2020 6c6f 6e20 3d20 6c6f 6e20 2a20      lon = lon * 
+00014290: 2d31 2020 2320 6374 792e 6461 7420 6669  -1  # cty.dat fi
+000142a0: 6c65 2069 6e76 6572 7473 206c 6f6e 6769  le inverts longi
+000142b0: 7475 6465 730a 2020 2020 2020 2020 2020  tudes.          
+000142c0: 2020 2020 2020 7072 696d 6172 795f 7066        primary_pf
+000142d0: 7820 3d20 615b 315d 2e67 6574 2822 7072  x = a[1].get("pr
+000142e0: 696d 6172 795f 7066 7822 2c20 2222 290a  imary_pfx", "").
+000142f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014300: 6865 6164 696e 6720 3d20 6265 6172 696e  heading = bearin
+00014310: 675f 7769 7468 5f6c 6174 6c6f 6e28 7365  g_with_latlon(se
+00014320: 6c66 2e73 7461 7469 6f6e 2e67 6574 2822  lf.station.get("
+00014330: 4772 6964 5371 7561 7265 2229 2c20 6c61  GridSquare"), la
+00014340: 742c 206c 6f6e 290a 2020 2020 2020 2020  t, lon).        
+00014350: 2020 2020 2020 2020 6b69 6c6f 6d65 7465          kilomete
+00014360: 7273 203d 2064 6973 7461 6e63 655f 7769  rs = distance_wi
+00014370: 7468 5f6c 6174 6c6f 6e28 0a20 2020 2020  th_latlon(.     
+00014380: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00014390: 656c 662e 7374 6174 696f 6e2e 6765 7428  elf.station.get(
+000143a0: 2247 7269 6453 7175 6172 6522 292c 206c  "GridSquare"), l
+000143b0: 6174 2c20 6c6f 6e0a 2020 2020 2020 2020  at, lon.        
+000143c0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000143d0: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
+000143e0: 6561 6469 6e67 5f64 6973 7461 6e63 652e  eading_distance.
+000143f0: 7365 7454 6578 7428 0a20 2020 2020 2020  setText(.       
+00014400: 2020 2020 2020 2020 2020 2020 2066 2252               f"R
+00014410: 6567 696f 6e61 6c20 4864 6720 7b68 6561  egional Hdg {hea
+00014420: 6469 6e67 7dc2 b020 4c50 207b 7265 6369  ding}.. LP {reci
+00014430: 7072 6f63 6f6c 2868 6561 6469 6e67 297d  procol(heading)}
+00014440: c2b0 202f 2022 0a20 2020 2020 2020 2020  .. / ".         
+00014450: 2020 2020 2020 2020 2020 2066 2264 6973             f"dis
+00014460: 7461 6e63 6520 7b69 6e74 286b 696c 6f6d  tance {int(kilom
+00014470: 6574 6572 732a 302e 3632 3133 3731 297d  eters*0.621371)}
+00014480: 6d69 207b 6b69 6c6f 6d65 7465 7273 7d6b  mi {kilometers}k
+00014490: 6d22 0a20 2020 2020 2020 2020 2020 2020  m".             
+000144a0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+000144b0: 2020 2020 2073 656c 662e 636f 6e74 6163       self.contac
+000144c0: 745b 2243 6f75 6e74 7279 5072 6566 6978  t["CountryPrefix
+000144d0: 225d 203d 2070 7269 6d61 7279 5f70 6678  "] = primary_pfx
+000144e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000144f0: 2073 656c 662e 636f 6e74 6163 745b 225a   self.contact["Z
+00014500: 4e22 5d20 3d20 696e 7428 6371 290a 2020  N"] = int(cq).  
+00014510: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00014520: 2073 656c 662e 636f 6e74 6573 743a 0a20   self.contest:. 
+00014530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014540: 2020 2069 6620 7365 6c66 2e63 6f6e 7465     if self.conte
+00014550: 7374 2e6e 616d 6520 3d3d 2022 4941 5255  st.name == "IARU
+00014560: 2048 4622 3a0a 2020 2020 2020 2020 2020   HF":.          
+00014570: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00014580: 6c66 2e63 6f6e 7461 6374 5b22 5a4e 225d  lf.contact["ZN"]
+00014590: 203d 2069 6e74 2869 7475 290a 2020 2020   = int(itu).    
+000145a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000145b0: 2e63 6f6e 7461 6374 5b22 436f 6e74 696e  .contact["Contin
+000145c0: 656e 7422 5d20 3d20 636f 6e74 696e 656e  ent"] = continen
+000145d0: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+000145e0: 2020 7365 6c66 2e64 785f 656e 7469 7479    self.dx_entity
+000145f0: 2e73 6574 5465 7874 280a 2020 2020 2020  .setText(.      
+00014600: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+00014610: 7b70 7269 6d61 7279 5f70 6678 7d3a 207b  {primary_pfx}: {
+00014620: 636f 6e74 696e 656e 747d 2f7b 656e 7469  continent}/{enti
+00014630: 7479 7d20 6371 3a7b 6371 7d20 6974 753a  ty} cq:{cq} itu:
+00014640: 7b69 7475 7d22 0a20 2020 2020 2020 2020  {itu}".         
+00014650: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00014660: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
+00014670: 6361 6c6c 7369 676e 2920 3e20 323a 0a20  callsign) > 2:. 
+00014680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014690: 2020 2069 6620 7365 6c66 2e63 6f6e 7465     if self.conte
+000146a0: 7374 3a0a 2020 2020 2020 2020 2020 2020  st:.            
+000146b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000146c0: 2e63 6f6e 7465 7374 2e70 7265 6669 6c6c  .contest.prefill
+000146d0: 2873 656c 6629 0a0a 2020 2020 6465 6620  (self)..    def 
+000146e0: 6368 6563 6b5f 6361 6c6c 7369 676e 3228  check_callsign2(
+000146f0: 7365 6c66 2c20 6361 6c6c 7369 676e 293a  self, callsign):
+00014700: 0a20 2020 2020 2020 2022 2222 4368 6563  .        """Chec
+00014710: 6b20 6361 6c6c 206f 6e63 6520 656e 7465  k call once ente
+00014720: 7265 6422 2222 0a20 2020 2020 2020 2063  red""".        c
+00014730: 616c 6c73 6967 6e20 3d20 6361 6c6c 7369  allsign = callsi
+00014740: 676e 2e73 7472 6970 2829 0a20 2020 2020  gn.strip().     
+00014750: 2020 2064 6562 7567 5f6c 6f6f 6b75 7020     debug_lookup 
+00014760: 3d20 6622 7b73 656c 662e 6c6f 6f6b 5f75  = f"{self.look_u
+00014770: 707d 220a 2020 2020 2020 2020 6c6f 6767  p}".        logg
+00014780: 6572 2e64 6562 7567 2822 2573 2c20 2573  er.debug("%s, %s
+00014790: 222c 2063 616c 6c73 6967 6e2c 2064 6562  ", callsign, deb
+000147a0: 7567 5f6c 6f6f 6b75 7029 0a20 2020 2020  ug_lookup).     
+000147b0: 2020 2069 6620 6861 7361 7474 7228 7365     if hasattr(se
+000147c0: 6c66 2e6c 6f6f 6b5f 7570 2c20 2273 6573  lf.look_up, "ses
+000147d0: 7369 6f6e 2229 3a0a 2020 2020 2020 2020  sion"):.        
+000147e0: 2020 2020 6966 2073 656c 662e 6c6f 6f6b      if self.look
+000147f0: 5f75 702e 7365 7373 696f 6e3a 0a20 2020  _up.session:.   
+00014800: 2020 2020 2020 2020 2020 2020 2072 6573               res
+00014810: 706f 6e73 6520 3d20 7365 6c66 2e6c 6f6f  ponse = self.loo
+00014820: 6b5f 7570 2e6c 6f6f 6b75 7028 6361 6c6c  k_up.lookup(call
+00014830: 7369 676e 290a 2020 2020 2020 2020 2020  sign).          
+00014840: 2020 2020 2020 6465 6275 675f 7265 7370        debug_resp
+00014850: 6f6e 7365 203d 2066 227b 7265 7370 6f6e  onse = f"{respon
+00014860: 7365 7d22 0a20 2020 2020 2020 2020 2020  se}".           
+00014870: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+00014880: 6728 2254 6865 2052 6573 706f 6e73 653a  g("The Response:
+00014890: 2025 735c 6e22 2c20 6465 6275 675f 7265   %s\n", debug_re
+000148a0: 7370 6f6e 7365 290a 2020 2020 2020 2020  sponse).        
+000148b0: 2020 2020 2020 2020 6966 2072 6573 706f          if respo
+000148c0: 6e73 653a 0a20 2020 2020 2020 2020 2020  nse:.           
+000148d0: 2020 2020 2020 2020 2074 6865 6972 6772           theirgr
+000148e0: 6964 203d 2072 6573 706f 6e73 652e 6765  id = response.ge
+000148f0: 7428 2267 7269 6422 290a 2020 2020 2020  t("grid").      
+00014900: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00014910: 6c66 2e63 6f6e 7461 6374 5b22 4772 6964  lf.contact["Grid
+00014920: 5371 7561 7265 225d 203d 2074 6865 6972  Square"] = their
+00014930: 6772 6964 0a20 2020 2020 2020 2020 2020  grid.           
+00014940: 2020 2020 2020 2020 205f 7468 6569 7263           _theirc
+00014950: 6f75 6e74 7279 203d 2072 6573 706f 6e73  ountry = respons
+00014960: 652e 6765 7428 2263 6f75 6e74 7279 2229  e.get("country")
+00014970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014980: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
+00014990: 7469 6f6e 2e67 6574 2822 4772 6964 5371  tion.get("GridSq
+000149a0: 7561 7265 222c 2022 2229 3a0a 2020 2020  uare", ""):.    
+000149b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000149c0: 2020 2020 6865 6164 696e 6720 3d20 6265      heading = be
+000149d0: 6172 696e 6728 7365 6c66 2e73 7461 7469  aring(self.stati
+000149e0: 6f6e 2e67 6574 2822 4772 6964 5371 7561  on.get("GridSqua
+000149f0: 7265 222c 2022 2229 2c20 7468 6569 7267  re", ""), theirg
+00014a00: 7269 6429 0a20 2020 2020 2020 2020 2020  rid).           
+00014a10: 2020 2020 2020 2020 2020 2020 206b 696c               kil
+00014a20: 6f6d 6574 6572 7320 3d20 6469 7374 616e  ometers = distan
+00014a30: 6365 2873 656c 662e 7374 6174 696f 6e2e  ce(self.station.
+00014a40: 6765 7428 2247 7269 6453 7175 6172 6522  get("GridSquare"
+00014a50: 292c 2074 6865 6972 6772 6964 290a 2020  ), theirgrid).  
+00014a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014a70: 2020 2020 2020 7365 6c66 2e68 6561 6469        self.headi
+00014a80: 6e67 5f64 6973 7461 6e63 652e 7365 7454  ng_distance.setT
+00014a90: 6578 7428 0a20 2020 2020 2020 2020 2020  ext(.           
+00014aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ab0: 2066 227b 7468 6569 7267 7269 647d 2048   f"{theirgrid} H
+00014ac0: 6467 207b 6865 6164 696e 677d c2b0 204c  dg {heading}.. L
+00014ad0: 5020 7b72 6563 6970 726f 636f 6c28 6865  P {reciprocol(he
+00014ae0: 6164 696e 6729 7dc2 b020 2f20 220a 2020  ading)}.. / ".  
+00014af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014b00: 2020 2020 2020 2020 2020 6622 6469 7374            f"dist
+00014b10: 616e 6365 207b 696e 7428 6b69 6c6f 6d65  ance {int(kilome
+00014b20: 7465 7273 2a30 2e36 3231 3337 3129 7d6d  ters*0.621371)}m
+00014b30: 6920 7b6b 696c 6f6d 6574 6572 737d 6b6d  i {kilometers}km
+00014b40: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00014b50: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00014b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014b70: 2320 7365 6c66 2e64 785f 656e 7469 7479  # self.dx_entity
+00014b80: 2e73 6574 5465 7874 2866 227b 7468 6569  .setText(f"{thei
+00014b90: 7263 6f75 6e74 7279 7d22 290a 2020 2020  rcountry}").    
+00014ba0: 2020 2020 2020 2020 2020 2020 2320 656c              # el
+00014bb0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00014bc0: 2020 2020 2320 7365 6c66 2e68 6561 6469      # self.headi
+00014bd0: 6e67 5f64 6973 7461 6e63 652e 7365 7454  ng_distance.setT
+00014be0: 6578 7428 224c 6f6f 6b75 7020 6661 696c  ext("Lookup fail
+00014bf0: 6564 2e22 290a 0a20 2020 2064 6566 2063  ed.")..    def c
+00014c00: 6865 636b 5f64 7570 6528 7365 6c66 2c20  heck_dupe(self, 
+00014c10: 6361 6c6c 3a20 7374 7229 202d 3e20 626f  call: str) -> bo
+00014c20: 6f6c 3a0a 2020 2020 2020 2020 2222 2243  ol:.        """C
+00014c30: 6865 636b 7320 6966 2061 2063 616c 6c73  hecks if a calls
+00014c40: 6967 6e20 6973 2061 2064 7570 6520 6f6e  ign is a dupe on
+00014c50: 2063 7572 7265 6e74 2062 616e 642f 6d6f   current band/mo
+00014c60: 6465 2e22 2222 0a20 2020 2020 2020 2069  de.""".        i
+00014c70: 6620 7365 6c66 2e63 6f6e 7465 7374 2069  f self.contest i
+00014c80: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00014c90: 2020 2020 7365 6c66 2e73 686f 775f 6d65      self.show_me
+00014ca0: 7373 6167 655f 626f 7828 2259 6f75 2068  ssage_box("You h
+00014cb0: 6176 6520 6e6f 2063 6f6e 7465 7374 206c  ave no contest l
+00014cc0: 6f61 6465 642e 2229 0a20 2020 2020 2020  oaded.").       
+00014cd0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00014ce0: 650a 2020 2020 2020 2020 7365 6c66 2e63  e.        self.c
+00014cf0: 6f6e 7465 7374 2e70 7265 6475 7065 2873  ontest.predupe(s
+00014d00: 656c 6629 0a20 2020 2020 2020 2062 616e  elf).        ban
+00014d10: 6420 3d20 666c 6f61 7428 6765 745f 6c6f  d = float(get_lo
+00014d20: 6767 6564 5f62 616e 6428 7374 7228 7365  gged_band(str(se
+00014d30: 6c66 2e72 6164 696f 5f73 7461 7465 2e67  lf.radio_state.g
+00014d40: 6574 2822 7666 6f61 222c 2030 2e30 2929  et("vfoa", 0.0))
+00014d50: 2929 0a20 2020 2020 2020 206d 6f64 6520  )).        mode 
+00014d60: 3d20 7365 6c66 2e72 6164 696f 5f73 7461  = self.radio_sta
+00014d70: 7465 2e67 6574 2822 6d6f 6465 222c 2022  te.get("mode", "
+00014d80: 2229 0a20 2020 2020 2020 2064 6562 7567  ").        debug
+00014d90: 6c69 6e65 203d 2028 0a20 2020 2020 2020  line = (.       
+00014da0: 2020 2020 2066 2243 616c 6c3a 207b 6361       f"Call: {ca
+00014db0: 6c6c 7d20 4261 6e64 3a20 7b62 616e 647d  ll} Band: {band}
+00014dc0: 204d 6f64 653a 207b 6d6f 6465 7d20 4475   Mode: {mode} Du
+00014dd0: 7065 7479 7065 3a20 7b73 656c 662e 636f  petype: {self.co
+00014de0: 6e74 6573 742e 6475 7065 5f74 7970 657d  ntest.dupe_type}
+00014df0: 220a 2020 2020 2020 2020 290a 2020 2020  ".        ).    
+00014e00: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+00014e10: 2822 2573 222c 2064 6562 7567 6c69 6e65  ("%s", debugline
+00014e20: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+00014e30: 662e 636f 6e74 6573 742e 6475 7065 5f74  f.contest.dupe_t
+00014e40: 7970 6520 3d3d 2031 3a0a 2020 2020 2020  ype == 1:.      
+00014e50: 2020 2020 2020 7265 7375 6c74 203d 2073        result = s
+00014e60: 656c 662e 6461 7461 6261 7365 2e63 6865  elf.database.che
+00014e70: 636b 5f64 7570 6528 6361 6c6c 290a 2020  ck_dupe(call).  
+00014e80: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
+00014e90: 6e74 6573 742e 6475 7065 5f74 7970 6520  ntest.dupe_type 
+00014ea0: 3d3d 2032 3a0a 2020 2020 2020 2020 2020  == 2:.          
+00014eb0: 2020 7265 7375 6c74 203d 2073 656c 662e    result = self.
+00014ec0: 6461 7461 6261 7365 2e63 6865 636b 5f64  database.check_d
+00014ed0: 7570 655f 6f6e 5f62 616e 6428 6361 6c6c  upe_on_band(call
+00014ee0: 2c20 6261 6e64 290a 2020 2020 2020 2020  , band).        
+00014ef0: 6966 2073 656c 662e 636f 6e74 6573 742e  if self.contest.
+00014f00: 6475 7065 5f74 7970 6520 3d3d 2033 3a0a  dupe_type == 3:.
+00014f10: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00014f20: 6c74 203d 2073 656c 662e 6461 7461 6261  lt = self.databa
+00014f30: 7365 2e63 6865 636b 5f64 7570 655f 6f6e  se.check_dupe_on
+00014f40: 5f62 616e 645f 6d6f 6465 2863 616c 6c2c  _band_mode(call,
+00014f50: 2062 616e 642c 206d 6f64 6529 0a20 2020   band, mode).   
+00014f60: 2020 2020 2069 6620 7365 6c66 2e63 6f6e       if self.con
+00014f70: 7465 7374 2e64 7570 655f 7479 7065 203d  test.dupe_type =
+00014f80: 3d20 343a 0a20 2020 2020 2020 2020 2020  = 4:.           
+00014f90: 2072 6573 756c 7420 3d20 7b22 6973 6475   result = {"isdu
+00014fa0: 7065 223a 2046 616c 7365 7d0a 2020 2020  pe": False}.    
+00014fb0: 2020 2020 6465 6275 676c 696e 6520 3d20      debugline = 
+00014fc0: 6622 7b72 6573 756c 747d 220a 2020 2020  f"{result}".    
+00014fd0: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+00014fe0: 2822 2573 222c 2064 6562 7567 6c69 6e65  ("%s", debugline
+00014ff0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00015000: 2072 6573 756c 742e 6765 7428 2269 7364   result.get("isd
+00015010: 7570 6522 2c20 4661 6c73 6529 0a0a 2020  upe", False)..  
+00015020: 2020 6465 6620 7365 746d 6f64 6528 7365    def setmode(se
+00015030: 6c66 2c20 6d6f 6465 3a20 7374 7229 202d  lf, mode: str) -
+00015040: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+00015050: 2222 2273 7475 6220 666f 7220 7768 656e  """stub for when
+00015060: 2074 6865 206d 6f64 6520 6368 616e 6765   the mode change
+00015070: 732e 2222 220a 2020 2020 2020 2020 6966  s.""".        if
+00015080: 206d 6f64 6520 3d3d 2022 4357 223a 0a20   mode == "CW":. 
+00015090: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+000150a0: 6c66 2e63 7572 7265 6e74 5f6d 6f64 6520  lf.current_mode 
+000150b0: 213d 2022 4357 223a 0a20 2020 2020 2020  != "CW":.       
+000150c0: 2020 2020 2020 2020 2073 656c 662e 6375           self.cu
+000150d0: 7272 656e 745f 6d6f 6465 203d 2022 4357  rrent_mode = "CW
+000150e0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+000150f0: 2020 2320 7365 6c66 2e6d 6f64 652e 7365    # self.mode.se
+00015100: 7454 6578 7428 2243 5722 290a 2020 2020  tText("CW").    
+00015110: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015120: 2e73 656e 742e 7365 7454 6578 7428 2235  .sent.setText("5
+00015130: 3939 2229 0a20 2020 2020 2020 2020 2020  99").           
+00015140: 2020 2020 2073 656c 662e 7265 6365 6976       self.receiv
+00015150: 652e 7365 7454 6578 7428 2235 3939 2229  e.setText("599")
+00015160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015170: 2073 656c 662e 7265 6164 5f63 775f 6d61   self.read_cw_ma
+00015180: 6372 6f73 2829 0a20 2020 2020 2020 2020  cros().         
+00015190: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+000151a0: 2020 6966 206d 6f64 6520 3d3d 2022 5353    if mode == "SS
+000151b0: 4222 3a0a 2020 2020 2020 2020 2020 2020  B":.            
+000151c0: 6966 2073 656c 662e 6375 7272 656e 745f  if self.current_
+000151d0: 6d6f 6465 2021 3d20 2253 5342 223a 0a20  mode != "SSB":. 
+000151e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000151f0: 656c 662e 6375 7272 656e 745f 6d6f 6465  elf.current_mode
+00015200: 203d 2022 5353 4222 0a20 2020 2020 2020   = "SSB".       
+00015210: 2020 2020 2020 2020 2023 2073 656c 662e           # self.
+00015220: 6d6f 6465 2e73 6574 5465 7874 2822 5353  mode.setText("SS
+00015230: 4222 290a 2020 2020 2020 2020 2020 2020  B").            
+00015240: 2020 2020 7365 6c66 2e73 656e 742e 7365      self.sent.se
+00015250: 7454 6578 7428 2235 3922 290a 2020 2020  tText("59").    
+00015260: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015270: 2e72 6563 6569 7665 2e73 6574 5465 7874  .receive.setText
+00015280: 2822 3539 2229 0a20 2020 2020 2020 2020  ("59").         
+00015290: 2020 2020 2020 2073 656c 662e 7265 6164         self.read
+000152a0: 5f63 775f 6d61 6372 6f73 2829 0a20 2020  _cw_macros().   
+000152b0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+000152c0: 2020 2020 2020 2020 6966 206d 6f64 6520          if mode 
+000152d0: 3d3d 2022 5254 5459 223a 0a20 2020 2020  == "RTTY":.     
+000152e0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+000152f0: 7572 7265 6e74 5f6d 6f64 6520 213d 2022  urrent_mode != "
+00015300: 5254 5459 223a 0a20 2020 2020 2020 2020  RTTY":.         
+00015310: 2020 2020 2020 2073 656c 662e 6375 7272         self.curr
+00015320: 656e 745f 6d6f 6465 203d 2022 5254 5459  ent_mode = "RTTY
+00015330: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00015340: 2020 2320 7365 6c66 2e6d 6f64 652e 7365    # self.mode.se
+00015350: 7454 6578 7428 2252 5454 5922 290a 2020  tText("RTTY").  
+00015360: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00015370: 6c66 2e73 656e 742e 7365 7454 6578 7428  lf.sent.setText(
+00015380: 2235 3922 290a 2020 2020 2020 2020 2020  "59").          
+00015390: 2020 2020 2020 7365 6c66 2e72 6563 6569        self.recei
+000153a0: 7665 2e73 6574 5465 7874 2822 3539 2229  ve.setText("59")
+000153b0: 0a0a 2020 2020 6465 6620 6765 745f 6f70  ..    def get_op
+000153c0: 6f6e 2873 656c 6629 3a0a 2020 2020 2020  on(self):.      
+000153d0: 2020 2222 2243 7472 6c2b 4f20 6f72 204f    """Ctrl+O or O
+000153e0: 504f 4e20 6469 616c 6f67 2222 220a 2020  PON dialog""".  
+000153f0: 2020 2020 2020 7365 6c66 2e6f 706f 6e5f        self.opon_
+00015400: 6469 616c 6f67 203d 204f 704f 6e28 574f  dialog = OpOn(WO
+00015410: 524b 494e 475f 5041 5448 290a 2020 2020  RKING_PATH).    
+00015420: 2020 2020 7365 6c66 2e6f 706f 6e5f 6469      self.opon_di
+00015430: 616c 6f67 2e61 6363 6570 7465 642e 636f  alog.accepted.co
+00015440: 6e6e 6563 7428 7365 6c66 2e6e 6577 5f6f  nnect(self.new_o
+00015450: 7029 0a20 2020 2020 2020 2073 656c 662e  p).        self.
+00015460: 6f70 6f6e 5f64 6961 6c6f 672e 6f70 656e  opon_dialog.open
+00015470: 2829 0a0a 2020 2020 6465 6620 6e65 775f  ()..    def new_
+00015480: 6f70 2873 656c 6629 3a0a 2020 2020 2020  op(self):.      
+00015490: 2020 2222 2253 6176 6520 6e65 7720 4f50    """Save new OP
+000154a0: 2222 220a 2020 2020 2020 2020 6966 2073  """.        if s
+000154b0: 656c 662e 6f70 6f6e 5f64 6961 6c6f 672e  elf.opon_dialog.
+000154c0: 4e65 774f 7065 7261 746f 722e 7465 7874  NewOperator.text
+000154d0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+000154e0: 7365 6c66 2e63 7572 7265 6e74 5f6f 7020  self.current_op 
+000154f0: 3d20 7365 6c66 2e6f 706f 6e5f 6469 616c  = self.opon_dial
+00015500: 6f67 2e4e 6577 4f70 6572 6174 6f72 2e74  og.NewOperator.t
+00015510: 6578 7428 292e 7570 7065 7228 290a 2020  ext().upper().  
+00015520: 2020 2020 2020 7365 6c66 2e6f 706f 6e5f        self.opon_
+00015530: 6469 616c 6f67 2e63 6c6f 7365 2829 0a20  dialog.close(). 
+00015540: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
+00015550: 6275 6728 224e 6577 204f 703a 2025 7322  bug("New Op: %s"
+00015560: 2c20 7365 6c66 2e63 7572 7265 6e74 5f6f  , self.current_o
+00015570: 7029 0a20 2020 2020 2020 2073 656c 662e  p).        self.
+00015580: 6d61 6b65 5f6f 705f 6469 7228 290a 0a20  make_op_dir().. 
+00015590: 2020 2064 6566 206d 616b 655f 6f70 5f64     def make_op_d
+000155a0: 6972 2873 656c 6629 3a0a 2020 2020 2020  ir(self):.      
+000155b0: 2020 2222 2243 7265 6174 6520 4f50 2064    """Create OP d
+000155c0: 6972 6563 746f 7279 2069 6620 6974 2064  irectory if it d
+000155d0: 6f65 7320 6e6f 7420 6578 6973 742e 2222  oes not exist.""
+000155e0: 220a 2020 2020 2020 2020 6966 2073 656c  ".        if sel
+000155f0: 662e 6375 7272 656e 745f 6f70 3a0a 2020  f.current_op:.  
+00015600: 2020 2020 2020 2020 2020 6f70 5f70 6174            op_pat
+00015610: 6820 3d20 5061 7468 2844 4154 415f 5041  h = Path(DATA_PA
+00015620: 5448 2920 2f20 7365 6c66 2e63 7572 7265  TH) / self.curre
+00015630: 6e74 5f6f 700a 2020 2020 2020 2020 2020  nt_op.          
+00015640: 2020 6c6f 6767 6572 2e64 6562 7567 2822    logger.debug("
+00015650: 6f70 5f70 6174 683a 2025 7322 2c20 7374  op_path: %s", st
+00015660: 7228 6f70 5f70 6174 6829 290a 2020 2020  r(op_path)).    
+00015670: 2020 2020 2020 2020 6966 206f 705f 7061          if op_pa
+00015680: 7468 2e69 735f 6469 7228 2920 6973 2046  th.is_dir() is F
+00015690: 616c 7365 3a0a 2020 2020 2020 2020 2020  alse:.          
+000156a0: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+000156b0: 7567 2822 4372 6561 7469 6e67 204f 7020  ug("Creating Op 
+000156c0: 4469 7265 6374 6f72 793a 2025 7322 2c20  Directory: %s", 
+000156d0: 7374 7228 6f70 5f70 6174 6829 290a 2020  str(op_path)).  
+000156e0: 2020 2020 2020 2020 2020 2020 2020 6f73                os
+000156f0: 2e6d 6b64 6972 2873 7472 286f 705f 7061  .mkdir(str(op_pa
+00015700: 7468 2929 0a20 2020 2020 2020 2020 2020  th)).           
+00015710: 2069 6620 6f70 5f70 6174 682e 6973 5f64   if op_path.is_d
+00015720: 6972 2829 3a0a 2020 2020 2020 2020 2020  ir():.          
+00015730: 2020 2020 2020 736f 7572 6365 5f70 6174        source_pat
+00015740: 6820 3d20 5061 7468 2857 4f52 4b49 4e47  h = Path(WORKING
+00015750: 5f50 4154 4829 202f 2022 6461 7461 2220  _PATH) / "data" 
+00015760: 2f20 2270 686f 6e65 7469 6373 220a 2020  / "phonetics".  
+00015770: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00015780: 6767 6572 2e64 6562 7567 2822 736f 7572  gger.debug("sour
+00015790: 6365 5f70 6174 683a 2025 7322 2c20 7374  ce_path: %s", st
+000157a0: 7228 736f 7572 6365 5f70 6174 6829 290a  r(source_path)).
+000157b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000157c0: 666f 7220 6368 696c 6420 696e 2073 6f75  for child in sou
+000157d0: 7263 655f 7061 7468 2e69 7465 7264 6972  rce_path.iterdir
+000157e0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+000157f0: 2020 2020 2020 2020 6465 7374 696e 6174          destinat
+00015800: 696f 6e5f 6669 6c65 203d 206f 705f 7061  ion_file = op_pa
+00015810: 7468 202f 2063 6869 6c64 2e6e 616d 650a  th / child.name.
+00015820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015830: 2020 2020 6966 2064 6573 7469 6e61 7469      if destinati
+00015840: 6f6e 5f66 696c 652e 6973 5f66 696c 6528  on_file.is_file(
+00015850: 2920 6973 2046 616c 7365 3a0a 2020 2020  ) is False:.    
+00015860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015870: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+00015880: 2822 4465 7374 696e 6174 696f 6e3a 2025  ("Destination: %
+00015890: 7322 2c20 7374 7228 6465 7374 696e 6174  s", str(destinat
+000158a0: 696f 6e5f 6669 6c65 2929 0a20 2020 2020  ion_file)).     
+000158b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000158c0: 2020 2064 6573 7469 6e61 7469 6f6e 5f66     destination_f
+000158d0: 696c 652e 7772 6974 655f 6279 7465 7328  ile.write_bytes(
+000158e0: 6368 696c 642e 7265 6164 5f62 7974 6573  child.read_bytes
+000158f0: 2829 290a 0a20 2020 2064 6566 2070 6f6c  ())..    def pol
+00015900: 6c5f 7261 6469 6f28 7365 6c66 293a 0a20  l_radio(self):. 
+00015910: 2020 2020 2020 2022 2222 7374 7562 2222         """stub""
+00015920: 220a 2020 2020 2020 2020 6966 2073 656c  ".        if sel
+00015930: 662e 7269 675f 636f 6e74 726f 6c3a 0a20  f.rig_control:. 
+00015940: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00015950: 6c66 2e72 6967 5f63 6f6e 7472 6f6c 2e6f  lf.rig_control.o
+00015960: 6e6c 696e 6520 6973 2046 616c 7365 3a0a  nline is False:.
+00015970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015980: 7365 6c66 2e72 6967 5f63 6f6e 7472 6f6c  self.rig_control
+00015990: 2e72 6569 6e69 7428 290a 2020 2020 2020  .reinit().      
+000159a0: 2020 2020 2020 6966 2073 656c 662e 7269        if self.ri
+000159b0: 675f 636f 6e74 726f 6c2e 6f6e 6c69 6e65  g_control.online
+000159c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000159d0: 2020 696e 666f 5f64 6972 7479 203d 2046    info_dirty = F
+000159e0: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
+000159f0: 2020 2020 2076 666f 203d 2073 656c 662e       vfo = self.
+00015a00: 7269 675f 636f 6e74 726f 6c2e 6765 745f  rig_control.get_
+00015a10: 7666 6f28 290a 2020 2020 2020 2020 2020  vfo().          
+00015a20: 2020 2020 2020 6d6f 6465 203d 2073 656c        mode = sel
+00015a30: 662e 7269 675f 636f 6e74 726f 6c2e 6765  f.rig_control.ge
+00015a40: 745f 6d6f 6465 2829 0a20 2020 2020 2020  t_mode().       
+00015a50: 2020 2020 2020 2020 2062 7720 3d20 7365           bw = se
+00015a60: 6c66 2e72 6967 5f63 6f6e 7472 6f6c 2e67  lf.rig_control.g
+00015a70: 6574 5f62 7728 290a 2020 2020 2020 2020  et_bw().        
+00015a80: 2020 2020 2020 2020 2320 7365 6c66 2e72          # self.r
+00015a90: 6164 696f 5f73 7461 7465 5b22 7074 7422  adio_state["ptt"
+00015aa0: 5d20 3d20 7365 6c66 2e72 6967 5f63 6f6e  ] = self.rig_con
+00015ab0: 7472 6f6c 2e67 6574 5f70 7474 2829 0a0a  trol.get_ptt()..
+00015ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ad0: 6966 206d 6f64 6520 3d3d 2022 4357 223a  if mode == "CW":
+00015ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015af0: 2020 2020 2073 656c 662e 7365 746d 6f64       self.setmod
+00015b00: 6528 6d6f 6465 290a 2020 2020 2020 2020  e(mode).        
+00015b10: 2020 2020 2020 2020 6966 206d 6f64 6520          if mode 
+00015b20: 3d3d 2022 4c53 4222 206f 7220 6d6f 6465  == "LSB" or mode
+00015b30: 203d 3d20 2255 5342 223a 0a20 2020 2020   == "USB":.     
+00015b40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00015b50: 656c 662e 7365 746d 6f64 6528 2253 5342  elf.setmode("SSB
+00015b60: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00015b70: 2020 2069 6620 6d6f 6465 203d 3d20 2252     if mode == "R
+00015b80: 5454 5922 3a0a 2020 2020 2020 2020 2020  TTY":.          
+00015b90: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00015ba0: 6574 6d6f 6465 2822 5254 5459 2229 0a0a  etmode("RTTY")..
+00015bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015bc0: 6966 2073 656c 662e 7261 6469 6f5f 7374  if self.radio_st
+00015bd0: 6174 652e 6765 7428 2276 666f 6122 2920  ate.get("vfoa") 
+00015be0: 213d 2076 666f 3a0a 2020 2020 2020 2020  != vfo:.        
+00015bf0: 2020 2020 2020 2020 2020 2020 696e 666f              info
+00015c00: 5f64 6972 7479 203d 2054 7275 650a 2020  _dirty = True.  
+00015c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015c20: 2020 7365 6c66 2e72 6164 696f 5f73 7461    self.radio_sta
+00015c30: 7465 5b22 7666 6f61 225d 203d 2076 666f  te["vfoa"] = vfo
+00015c40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015c50: 2062 616e 6420 3d20 6765 7462 616e 6428   band = getband(
+00015c60: 7374 7228 7666 6f29 290a 2020 2020 2020  str(vfo)).      
+00015c70: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+00015c80: 6164 696f 5f73 7461 7465 5b22 6261 6e64  adio_state["band
+00015c90: 225d 203d 2062 616e 640a 2020 2020 2020  "] = band.      
+00015ca0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00015cb0: 6f6e 7461 6374 5b22 4261 6e64 225d 203d  ontact["Band"] =
+00015cc0: 2067 6574 5f6c 6f67 6765 645f 6261 6e64   get_logged_band
+00015cd0: 2873 7472 2876 666f 2929 0a20 2020 2020  (str(vfo)).     
+00015ce0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015cf0: 7365 745f 6261 6e64 5f69 6e64 6963 6174  set_band_indicat
+00015d00: 6f72 2862 616e 6429 0a0a 2020 2020 2020  or(band)..      
+00015d10: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00015d20: 662e 7261 6469 6f5f 7374 6174 652e 6765  f.radio_state.ge
+00015d30: 7428 226d 6f64 6522 2920 213d 206d 6f64  t("mode") != mod
+00015d40: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00015d50: 2020 2020 2020 2069 6e66 6f5f 6469 7274         info_dirt
+00015d60: 7920 3d20 5472 7565 0a20 2020 2020 2020  y = True.       
+00015d70: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015d80: 662e 7261 6469 6f5f 7374 6174 655b 226d  f.radio_state["m
+00015d90: 6f64 6522 5d20 3d20 6d6f 6465 0a0a 2020  ode"] = mode..  
+00015da0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00015db0: 2073 656c 662e 7261 6469 6f5f 7374 6174   self.radio_stat
+00015dc0: 652e 6765 7428 2262 7722 2920 213d 2062  e.get("bw") != b
+00015dd0: 773a 0a20 2020 2020 2020 2020 2020 2020  w:.             
+00015de0: 2020 2020 2020 2069 6e66 6f5f 6469 7274         info_dirt
+00015df0: 7920 3d20 5472 7565 0a20 2020 2020 2020  y = True.       
+00015e00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00015e10: 662e 7261 6469 6f5f 7374 6174 655b 2262  f.radio_state["b
+00015e20: 7722 5d20 3d20 6277 0a0a 2020 2020 2020  w"] = bw..      
+00015e30: 2020 2020 2020 2020 2020 6966 2064 6174            if dat
+00015e40: 6574 696d 652e 6e6f 7728 2920 3e20 676c  etime.now() > gl
+00015e50: 6f62 616c 7328 295b 2270 6f6c 6c5f 7469  obals()["poll_ti
+00015e60: 6d65 225d 206f 7220 696e 666f 5f64 6972  me"] or info_dir
+00015e70: 7479 3a0a 2020 2020 2020 2020 2020 2020  ty:.            
+00015e80: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+00015e90: 6562 7567 2822 5646 4f3a 2025 7320 204d  ebug("VFO: %s  M
+00015ea0: 4f44 453a 2025 7320 4257 3a20 2573 222c  ODE: %s BW: %s",
+00015eb0: 2076 666f 2c20 6d6f 6465 2c20 6277 290a   vfo, mode, bw).
+00015ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ed0: 2020 2020 7365 6c66 2e73 6574 5f77 696e      self.set_win
+00015ee0: 646f 775f 7469 746c 6528 290a 2020 2020  dow_title().    
+00015ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015f00: 636d 6420 3d20 7b7d 0a20 2020 2020 2020  cmd = {}.       
+00015f10: 2020 2020 2020 2020 2020 2020 2063 6d64               cmd
+00015f20: 5b22 636d 6422 5d20 3d20 2252 4144 494f  ["cmd"] = "RADIO
+00015f30: 5f53 5441 5445 220a 2020 2020 2020 2020  _STATE".        
+00015f40: 2020 2020 2020 2020 2020 2020 636d 645b              cmd[
+00015f50: 2273 7461 7469 6f6e 225d 203d 2070 6c61  "station"] = pla
+00015f60: 7466 6f72 6d2e 6e6f 6465 2829 0a20 2020  tform.node().   
+00015f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015f80: 2063 6d64 5b22 6261 6e64 225d 203d 2062   cmd["band"] = b
+00015f90: 616e 640a 2020 2020 2020 2020 2020 2020  and.            
+00015fa0: 2020 2020 2020 2020 636d 645b 2276 666f          cmd["vfo
+00015fb0: 6122 5d20 3d20 7666 6f0a 2020 2020 2020  a"] = vfo.      
+00015fc0: 2020 2020 2020 2020 2020 2020 2020 636d                cm
+00015fd0: 645b 226d 6f64 6522 5d20 3d20 6d6f 6465  d["mode"] = mode
+00015fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015ff0: 2020 2020 2063 6d64 5b22 6277 225d 203d       cmd["bw"] =
+00016000: 2062 770a 2020 2020 2020 2020 2020 2020   bw.            
+00016010: 2020 2020 2020 2020 7365 6c66 2e6d 756c          self.mul
+00016020: 7469 6361 7374 5f69 6e74 6572 6661 6365  ticast_interface
+00016030: 2e73 656e 645f 6173 5f6a 736f 6e28 636d  .send_as_json(cm
+00016040: 6429 0a20 2020 2020 2020 2020 2020 2020  d).             
+00016050: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
+00016060: 316d 6d3a 0a20 2020 2020 2020 2020 2020  1mm:.           
+00016070: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00016080: 7365 6c66 2e6e 316d 6d2e 7365 6e64 5f72  self.n1mm.send_r
+00016090: 6164 696f 5f70 6163 6b65 7473 3a0a 2020  adio_packets:.  
+000160a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000160b0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+000160c0: 316d 6d2e 7261 6469 6f5f 696e 666f 5b22  1mm.radio_info["
+000160d0: 4672 6571 225d 203d 2076 666f 5b3a 2d31  Freq"] = vfo[:-1
+000160e0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+000160f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00016100: 6c66 2e6e 316d 6d2e 7261 6469 6f5f 696e  lf.n1mm.radio_in
+00016110: 666f 5b22 5458 4672 6571 225d 203d 2076  fo["TXFreq"] = v
+00016120: 666f 5b3a 2d31 5d0a 2020 2020 2020 2020  fo[:-1].        
+00016130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016140: 2020 2020 7365 6c66 2e6e 316d 6d2e 7261      self.n1mm.ra
+00016150: 6469 6f5f 696e 666f 5b22 4d6f 6465 225d  dio_info["Mode"]
+00016160: 203d 206d 6f64 650a 2020 2020 2020 2020   = mode.        
+00016170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016180: 2020 2020 7365 6c66 2e6e 316d 6d2e 7261      self.n1mm.ra
+00016190: 6469 6f5f 696e 666f 5b22 4f70 4361 6c6c  dio_info["OpCall
+000161a0: 225d 203d 2073 656c 662e 6375 7272 656e  "] = self.curren
+000161b0: 745f 6f70 0a20 2020 2020 2020 2020 2020  t_op.           
+000161c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000161d0: 2073 656c 662e 6e31 6d6d 2e72 6164 696f   self.n1mm.radio
+000161e0: 5f69 6e66 6f5b 2249 7352 756e 6e69 6e67  _info["IsRunning
+000161f0: 225d 203d 2073 7472 280a 2020 2020 2020  "] = str(.      
+00016200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016210: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+00016220: 7265 662e 6765 7428 2272 756e 5f73 7461  ref.get("run_sta
+00016230: 7465 222c 2046 616c 7365 290a 2020 2020  te", False).    
+00016240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016250: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00016260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016270: 2020 2020 2020 7365 6c66 2e6e 316d 6d2e        self.n1mm.
+00016280: 7365 6e64 5f72 6164 696f 2829 0a20 2020  send_radio().   
+00016290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000162a0: 2067 6c6f 6261 6c73 2829 5b22 706f 6c6c   globals()["poll
+000162b0: 5f74 696d 6522 5d20 3d20 6461 7465 7469  _time"] = dateti
+000162c0: 6d65 2e6e 6f77 2829 202b 2064 742e 7469  me.now() + dt.ti
+000162d0: 6d65 6465 6c74 6128 7365 636f 6e64 733d  medelta(seconds=
+000162e0: 3130 290a 0a20 2020 2064 6566 2065 6469  10)..    def edi
+000162f0: 745f 6377 5f6d 6163 726f 7328 7365 6c66  t_cw_macros(self
+00016300: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00016310: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
+00016320: 616c 6c73 2074 6865 2064 6566 6175 6c74  alls the default
+00016330: 2074 6578 7420 6564 6974 6f72 2074 6f20   text editor to 
+00016340: 6564 6974 2074 6865 2043 5720 6d61 6372  edit the CW macr
+00016350: 6f20 6669 6c65 2e0a 2020 2020 2020 2020  o file..        
+00016360: 2222 220a 2020 2020 2020 2020 6966 2073  """.        if s
+00016370: 656c 662e 7261 6469 6f5f 7374 6174 652e  elf.radio_state.
+00016380: 6765 7428 226d 6f64 6522 2920 3d3d 2022  get("mode") == "
+00016390: 4357 223a 0a20 2020 2020 2020 2020 2020  CW":.           
+000163a0: 206d 6163 726f 5f66 696c 6520 3d20 222f   macro_file = "/
+000163b0: 6377 6d61 6372 6f73 2e74 7874 220a 2020  cwmacros.txt".  
+000163c0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+000163d0: 2020 2020 2020 2020 6d61 6372 6f5f 6669          macro_fi
+000163e0: 6c65 203d 2022 2f73 7362 6d61 6372 6f73  le = "/ssbmacros
+000163f0: 2e74 7874 220a 2020 2020 2020 2020 6966  .txt".        if
+00016400: 206e 6f74 2050 6174 6828 4441 5441 5f50   not Path(DATA_P
+00016410: 4154 4820 2b20 6d61 6372 6f5f 6669 6c65  ATH + macro_file
+00016420: 292e 6578 6973 7473 2829 3a0a 2020 2020  ).exists():.    
+00016430: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+00016440: 6562 7567 2822 7265 6164 5f63 775f 6d61  ebug("read_cw_ma
+00016450: 6372 6f73 3a20 636f 7079 696e 6720 6465  cros: copying de
+00016460: 6661 756c 7420 6d61 6372 6f20 6669 6c65  fault macro file
+00016470: 2e22 290a 2020 2020 2020 2020 2020 2020  .").            
+00016480: 636f 7079 6669 6c65 2857 4f52 4b49 4e47  copyfile(WORKING
+00016490: 5f50 4154 4820 2b20 222f 6461 7461 2220  _PATH + "/data" 
+000164a0: 2b20 6d61 6372 6f5f 6669 6c65 2c20 4441  + macro_file, DA
+000164b0: 5441 5f50 4154 4820 2b20 6d61 6372 6f5f  TA_PATH + macro_
+000164c0: 6669 6c65 290a 2020 2020 2020 2020 6f73  file).        os
+000164d0: 2e73 7973 7465 6d28 6622 7864 672d 6f70  .system(f"xdg-op
+000164e0: 656e 207b 4441 5441 5f50 4154 487d 7b6d  en {DATA_PATH}{m
+000164f0: 6163 726f 5f66 696c 657d 2229 0a0a 2020  acro_file}")..  
+00016500: 2020 6465 6620 7265 6164 5f63 775f 6d61    def read_cw_ma
+00016510: 6372 6f73 2873 656c 6629 202d 3e20 4e6f  cros(self) -> No
+00016520: 6e65 3a0a 2020 2020 2020 2020 2222 220a  ne:.        """.
+00016530: 2020 2020 2020 2020 5265 6164 7320 696e          Reads in
+00016540: 2074 6865 2043 5720 6d61 6372 6f73 2c20   the CW macros, 
+00016550: 6669 7273 7473 2069 7420 6368 6563 6b73  firsts it checks
+00016560: 2074 6f20 7365 6520 6966 2074 6865 2066   to see if the f
+00016570: 696c 6520 6578 6973 7473 2e20 4966 2069  ile exists. If i
+00016580: 7420 646f 6573 206e 6f74 2c0a 2020 2020  t does not,.    
+00016590: 2020 2020 616e 6420 7468 6973 2068 6173      and this has
+000165a0: 2062 6565 6e20 7061 636b 6167 6564 2077   been packaged w
+000165b0: 6974 6820 7079 696e 7374 616c 6c65 7220  ith pyinstaller 
+000165c0: 6974 2077 696c 6c20 636f 7079 2074 6865  it will copy the
+000165d0: 2064 6566 6175 6c74 2066 696c 6520 6672   default file fr
+000165e0: 6f6d 2074 6865 0a20 2020 2020 2020 2074  om the.        t
+000165f0: 656d 7020 6469 7265 6374 6f72 7920 7468  emp directory th
+00016600: 6973 2069 7320 7275 6e6e 696e 6720 6672  is is running fr
+00016610: 6f6d 2e2e 2e20 496e 2074 6865 6f72 792e  om... In theory.
+00016620: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
+00016630: 2020 2020 2020 6966 2073 656c 662e 7261        if self.ra
+00016640: 6469 6f5f 7374 6174 652e 6765 7428 226d  dio_state.get("m
+00016650: 6f64 6522 2920 3d3d 2022 4357 223a 0a20  ode") == "CW":. 
+00016660: 2020 2020 2020 2020 2020 206d 6163 726f             macro
+00016670: 5f66 696c 6520 3d20 222f 6377 6d61 6372  _file = "/cwmacr
+00016680: 6f73 2e74 7874 220a 2020 2020 2020 2020  os.txt".        
+00016690: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000166a0: 2020 6d61 6372 6f5f 6669 6c65 203d 2022    macro_file = "
+000166b0: 2f73 7362 6d61 6372 6f73 2e74 7874 220a  /ssbmacros.txt".
+000166c0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+000166d0: 5061 7468 2844 4154 415f 5041 5448 202b  Path(DATA_PATH +
+000166e0: 206d 6163 726f 5f66 696c 6529 2e65 7869   macro_file).exi
+000166f0: 7374 7328 293a 0a20 2020 2020 2020 2020  sts():.         
+00016700: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+00016710: 2272 6561 645f 6377 5f6d 6163 726f 733a  "read_cw_macros:
+00016720: 2063 6f70 7969 6e67 2064 6566 6175 6c74   copying default
+00016730: 206d 6163 726f 2066 696c 652e 2229 0a20   macro file."). 
+00016740: 2020 2020 2020 2020 2020 2063 6f70 7966             copyf
+00016750: 696c 6528 574f 524b 494e 475f 5041 5448  ile(WORKING_PATH
+00016760: 202b 2022 2f64 6174 6122 202b 206d 6163   + "/data" + mac
+00016770: 726f 5f66 696c 652c 2044 4154 415f 5041  ro_file, DATA_PA
+00016780: 5448 202b 206d 6163 726f 5f66 696c 6529  TH + macro_file)
+00016790: 0a20 2020 2020 2020 2077 6974 6820 6f70  .        with op
+000167a0: 656e 2844 4154 415f 5041 5448 202b 206d  en(DATA_PATH + m
+000167b0: 6163 726f 5f66 696c 652c 2022 7222 2c20  acro_file, "r", 
+000167c0: 656e 636f 6469 6e67 3d22 7574 662d 3822  encoding="utf-8"
+000167d0: 2920 6173 2066 696c 655f 6465 7363 7269  ) as file_descri
+000167e0: 7074 6f72 3a0a 2020 2020 2020 2020 2020  ptor:.          
+000167f0: 2020 666f 7220 6c69 6e65 2069 6e20 6669    for line in fi
+00016800: 6c65 5f64 6573 6372 6970 746f 723a 0a20  le_descriptor:. 
+00016810: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00016820: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00016830: 2020 2020 2020 2020 6d6f 6465 2c20 666b          mode, fk
+00016840: 6579 2c20 6275 7474 6f6e 6e61 6d65 2c20  ey, buttonname, 
+00016850: 6377 7465 7874 203d 206c 696e 652e 7370  cwtext = line.sp
+00016860: 6c69 7428 227c 2229 0a20 2020 2020 2020  lit("|").       
+00016870: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00016880: 6d6f 6465 2e73 7472 6970 2829 2e75 7070  mode.strip().upp
+00016890: 6572 2829 203d 3d20 2252 2220 616e 6420  er() == "R" and 
+000168a0: 7365 6c66 2e70 7265 662e 6765 7428 2272  self.pref.get("r
+000168b0: 756e 5f73 7461 7465 2229 3a0a 2020 2020  un_state"):.    
+000168c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000168d0: 2020 2020 7365 6c66 2e66 6b65 7973 5b66      self.fkeys[f
+000168e0: 6b65 792e 7374 7269 7028 295d 203d 2028  key.strip()] = (
+000168f0: 6275 7474 6f6e 6e61 6d65 2e73 7472 6970  buttonname.strip
+00016900: 2829 2c20 6377 7465 7874 2e73 7472 6970  (), cwtext.strip
+00016910: 2829 290a 2020 2020 2020 2020 2020 2020  ()).            
+00016920: 2020 2020 2020 2020 6966 206d 6f64 652e          if mode.
+00016930: 7374 7269 7028 292e 7570 7065 7228 2920  strip().upper() 
+00016940: 213d 2022 5222 2061 6e64 206e 6f74 2073  != "R" and not s
+00016950: 656c 662e 7072 6566 2e67 6574 2822 7275  elf.pref.get("ru
+00016960: 6e5f 7374 6174 6522 293a 0a20 2020 2020  n_state"):.     
+00016970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016980: 2020 2073 656c 662e 666b 6579 735b 666b     self.fkeys[fk
+00016990: 6579 2e73 7472 6970 2829 5d20 3d20 2862  ey.strip()] = (b
+000169a0: 7574 746f 6e6e 616d 652e 7374 7269 7028  uttonname.strip(
+000169b0: 292c 2063 7774 6578 742e 7374 7269 7028  ), cwtext.strip(
+000169c0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+000169d0: 2020 2065 7863 6570 7420 5661 6c75 6545     except ValueE
+000169e0: 7272 6f72 2061 7320 6572 723a 0a20 2020  rror as err:.   
+000169f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016a00: 206c 6f67 6765 722e 696e 666f 2822 7265   logger.info("re
+00016a10: 6164 5f63 775f 6d61 6372 6f73 3a20 2573  ad_cw_macros: %s
+00016a20: 222c 2065 7272 290a 2020 2020 2020 2020  ", err).        
+00016a30: 6b65 7973 203d 2073 656c 662e 666b 6579  keys = self.fkey
+00016a40: 732e 6b65 7973 2829 0a20 2020 2020 2020  s.keys().       
+00016a50: 2069 6620 2246 3122 2069 6e20 6b65 7973   if "F1" in keys
+00016a60: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00016a70: 6c66 2e46 312e 7365 7454 6578 7428 6622  lf.F1.setText(f"
+00016a80: 4631 3a20 7b73 656c 662e 666b 6579 735b  F1: {self.fkeys[
+00016a90: 2746 3127 5d5b 305d 7d22 290a 2020 2020  'F1'][0]}").    
+00016aa0: 2020 2020 2020 2020 7365 6c66 2e46 312e          self.F1.
+00016ab0: 7365 7454 6f6f 6c54 6970 2873 656c 662e  setToolTip(self.
+00016ac0: 666b 6579 735b 2246 3122 5d5b 315d 290a  fkeys["F1"][1]).
+00016ad0: 2020 2020 2020 2020 6966 2022 4632 2220          if "F2" 
+00016ae0: 696e 206b 6579 733a 0a20 2020 2020 2020  in keys:.       
+00016af0: 2020 2020 2073 656c 662e 4632 2e73 6574       self.F2.set
+00016b00: 5465 7874 2866 2246 323a 207b 7365 6c66  Text(f"F2: {self
+00016b10: 2e66 6b65 7973 5b27 4632 275d 5b30 5d7d  .fkeys['F2'][0]}
+00016b20: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
+00016b30: 656c 662e 4632 2e73 6574 546f 6f6c 5469  elf.F2.setToolTi
+00016b40: 7028 7365 6c66 2e66 6b65 7973 5b22 4632  p(self.fkeys["F2
+00016b50: 225d 5b31 5d29 0a20 2020 2020 2020 2069  "][1]).        i
+00016b60: 6620 2246 3322 2069 6e20 6b65 7973 3a0a  f "F3" in keys:.
+00016b70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00016b80: 2e46 332e 7365 7454 6578 7428 6622 4633  .F3.setText(f"F3
+00016b90: 3a20 7b73 656c 662e 666b 6579 735b 2746  : {self.fkeys['F
+00016ba0: 3327 5d5b 305d 7d22 290a 2020 2020 2020  3'][0]}").      
+00016bb0: 2020 2020 2020 7365 6c66 2e46 332e 7365        self.F3.se
+00016bc0: 7454 6f6f 6c54 6970 2873 656c 662e 666b  tToolTip(self.fk
+00016bd0: 6579 735b 2246 3322 5d5b 315d 290a 2020  eys["F3"][1]).  
+00016be0: 2020 2020 2020 6966 2022 4634 2220 696e        if "F4" in
+00016bf0: 206b 6579 733a 0a20 2020 2020 2020 2020   keys:.         
+00016c00: 2020 2073 656c 662e 4634 2e73 6574 5465     self.F4.setTe
+00016c10: 7874 2866 2246 343a 207b 7365 6c66 2e66  xt(f"F4: {self.f
+00016c20: 6b65 7973 5b27 4634 275d 5b30 5d7d 2229  keys['F4'][0]}")
+00016c30: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00016c40: 662e 4634 2e73 6574 546f 6f6c 5469 7028  f.F4.setToolTip(
+00016c50: 7365 6c66 2e66 6b65 7973 5b22 4634 225d  self.fkeys["F4"]
+00016c60: 5b31 5d29 0a20 2020 2020 2020 2069 6620  [1]).        if 
+00016c70: 2246 3522 2069 6e20 6b65 7973 3a0a 2020  "F5" in keys:.  
+00016c80: 2020 2020 2020 2020 2020 7365 6c66 2e46            self.F
+00016c90: 352e 7365 7454 6578 7428 6622 4635 3a20  5.setText(f"F5: 
+00016ca0: 7b73 656c 662e 666b 6579 735b 2746 3527  {self.fkeys['F5'
+00016cb0: 5d5b 305d 7d22 290a 2020 2020 2020 2020  ][0]}").        
+00016cc0: 2020 2020 7365 6c66 2e46 352e 7365 7454      self.F5.setT
+00016cd0: 6f6f 6c54 6970 2873 656c 662e 666b 6579  oolTip(self.fkey
+00016ce0: 735b 2246 3522 5d5b 315d 290a 2020 2020  s["F5"][1]).    
+00016cf0: 2020 2020 6966 2022 4636 2220 696e 206b      if "F6" in k
+00016d00: 6579 733a 0a20 2020 2020 2020 2020 2020  eys:.           
+00016d10: 2073 656c 662e 4636 2e73 6574 5465 7874   self.F6.setText
+00016d20: 2866 2246 363a 207b 7365 6c66 2e66 6b65  (f"F6: {self.fke
+00016d30: 7973 5b27 4636 275d 5b30 5d7d 2229 0a20  ys['F6'][0]}"). 
+00016d40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00016d50: 4636 2e73 6574 546f 6f6c 5469 7028 7365  F6.setToolTip(se
+00016d60: 6c66 2e66 6b65 7973 5b22 4636 225d 5b31  lf.fkeys["F6"][1
+00016d70: 5d29 0a20 2020 2020 2020 2069 6620 2246  ]).        if "F
+00016d80: 3722 2069 6e20 6b65 7973 3a0a 2020 2020  7" in keys:.    
+00016d90: 2020 2020 2020 2020 7365 6c66 2e46 372e          self.F7.
+00016da0: 7365 7454 6578 7428 6622 4637 3a20 7b73  setText(f"F7: {s
+00016db0: 656c 662e 666b 6579 735b 2746 3727 5d5b  elf.fkeys['F7'][
+00016dc0: 305d 7d22 290a 2020 2020 2020 2020 2020  0]}").          
+00016dd0: 2020 7365 6c66 2e46 372e 7365 7454 6f6f    self.F7.setToo
+00016de0: 6c54 6970 2873 656c 662e 666b 6579 735b  lTip(self.fkeys[
+00016df0: 2246 3722 5d5b 315d 290a 2020 2020 2020  "F7"][1]).      
+00016e00: 2020 6966 2022 4638 2220 696e 206b 6579    if "F8" in key
+00016e10: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
+00016e20: 656c 662e 4638 2e73 6574 5465 7874 2866  elf.F8.setText(f
+00016e30: 2246 383a 207b 7365 6c66 2e66 6b65 7973  "F8: {self.fkeys
+00016e40: 5b27 4638 275d 5b30 5d7d 2229 0a20 2020  ['F8'][0]}").   
+00016e50: 2020 2020 2020 2020 2073 656c 662e 4638           self.F8
+00016e60: 2e73 6574 546f 6f6c 5469 7028 7365 6c66  .setToolTip(self
+00016e70: 2e66 6b65 7973 5b22 4638 225d 5b31 5d29  .fkeys["F8"][1])
+00016e80: 0a20 2020 2020 2020 2069 6620 2246 3922  .        if "F9"
+00016e90: 2069 6e20 6b65 7973 3a0a 2020 2020 2020   in keys:.      
+00016ea0: 2020 2020 2020 7365 6c66 2e46 392e 7365        self.F9.se
+00016eb0: 7454 6578 7428 6622 4639 3a20 7b73 656c  tText(f"F9: {sel
+00016ec0: 662e 666b 6579 735b 2746 3927 5d5b 305d  f.fkeys['F9'][0]
+00016ed0: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
+00016ee0: 7365 6c66 2e46 392e 7365 7454 6f6f 6c54  self.F9.setToolT
+00016ef0: 6970 2873 656c 662e 666b 6579 735b 2246  ip(self.fkeys["F
+00016f00: 3922 5d5b 315d 290a 2020 2020 2020 2020  9"][1]).        
+00016f10: 6966 2022 4631 3022 2069 6e20 6b65 7973  if "F10" in keys
+00016f20: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00016f30: 6c66 2e46 3130 2e73 6574 5465 7874 2866  lf.F10.setText(f
+00016f40: 2246 3130 3a20 7b73 656c 662e 666b 6579  "F10: {self.fkey
+00016f50: 735b 2746 3130 275d 5b30 5d7d 2229 0a20  s['F10'][0]}"). 
+00016f60: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00016f70: 4631 302e 7365 7454 6f6f 6c54 6970 2873  F10.setToolTip(s
+00016f80: 656c 662e 666b 6579 735b 2246 3130 225d  elf.fkeys["F10"]
+00016f90: 5b31 5d29 0a20 2020 2020 2020 2069 6620  [1]).        if 
+00016fa0: 2246 3131 2220 696e 206b 6579 733a 0a20  "F11" in keys:. 
+00016fb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00016fc0: 4631 312e 7365 7454 6578 7428 6622 4631  F11.setText(f"F1
+00016fd0: 313a 207b 7365 6c66 2e66 6b65 7973 5b27  1: {self.fkeys['
+00016fe0: 4631 3127 5d5b 305d 7d22 290a 2020 2020  F11'][0]}").    
+00016ff0: 2020 2020 2020 2020 7365 6c66 2e46 3131          self.F11
+00017000: 2e73 6574 546f 6f6c 5469 7028 7365 6c66  .setToolTip(self
+00017010: 2e66 6b65 7973 5b22 4631 3122 5d5b 315d  .fkeys["F11"][1]
+00017020: 290a 2020 2020 2020 2020 6966 2022 4631  ).        if "F1
+00017030: 3222 2069 6e20 6b65 7973 3a0a 2020 2020  2" in keys:.    
+00017040: 2020 2020 2020 2020 7365 6c66 2e46 3132          self.F12
+00017050: 2e73 6574 5465 7874 2866 2246 3132 3a20  .setText(f"F12: 
+00017060: 7b73 656c 662e 666b 6579 735b 2746 3132  {self.fkeys['F12
+00017070: 275d 5b30 5d7d 2229 0a20 2020 2020 2020  '][0]}").       
+00017080: 2020 2020 2073 656c 662e 4631 322e 7365       self.F12.se
+00017090: 7454 6f6f 6c54 6970 2873 656c 662e 666b  tToolTip(self.fk
+000170a0: 6579 735b 2246 3132 225d 5b31 5d29 0a0a  eys["F12"][1])..
+000170b0: 2020 2020 6465 6620 6765 6e65 7261 7465      def generate
+000170c0: 5f61 6469 6628 7365 6c66 293a 0a20 2020  _adif(self):.   
+000170d0: 2020 2020 2022 2222 4765 6e65 7261 7465       """Generate
+000170e0: 2041 4449 4622 2222 0a20 2020 2020 2020   ADIF""".       
+000170f0: 206c 6f67 6765 722e 6465 6275 6728 222a   logger.debug("*
+00017100: 2a2a 2a2a 2a41 4449 462a 2a2a 2a2a 2229  *****ADIF*****")
+00017110: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
+00017120: 6e74 6573 742e 6164 6966 2873 656c 6629  ntest.adif(self)
+00017130: 0a0a 2020 2020 6465 6620 6765 6e65 7261  ..    def genera
+00017140: 7465 5f63 6162 7269 6c6c 6f28 7365 6c66  te_cabrillo(self
+00017150: 293a 0a20 2020 2020 2020 2022 2222 4765  ):.        """Ge
+00017160: 6e65 7261 7465 7320 4361 6272 696c 6c6f  nerates Cabrillo
+00017170: 2066 696c 652e 204d 6179 6265 2e22 2222   file. Maybe."""
+00017180: 0a20 2020 2020 2020 2023 2068 7474 7073  .        # https
+00017190: 3a2f 2f77 7777 2e63 7177 7078 2e63 6f6d  ://www.cqwpx.com
+000171a0: 2f63 6162 7269 6c6c 6f2e 6874 6d0a 2020  /cabrillo.htm.  
+000171b0: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+000171c0: 7567 2822 2a2a 2a2a 2a2a 4361 6272 696c  ug("******Cabril
+000171d0: 6c6f 2a2a 2a2a 2a22 290a 2020 2020 2020  lo*****").      
+000171e0: 2020 7365 6c66 2e63 6f6e 7465 7374 2e63    self.contest.c
+000171f0: 6162 7269 6c6c 6f28 7365 6c66 290a 0a0a  abrillo(self)...
+00017200: 6465 6620 6c6f 6164 5f66 6f6e 7473 5f66  def load_fonts_f
+00017210: 726f 6d5f 6469 7228 6469 7265 6374 6f72  rom_dir(director
+00017220: 793a 2073 7472 2920 2d3e 2073 6574 3a0a  y: str) -> set:.
+00017230: 2020 2020 2222 220a 2020 2020 5765 6c6c      """.    Well
+00017240: 2069 7420 6c6f 6164 7320 666f 6e74 7320   it loads fonts 
+00017250: 6672 6f6d 2061 2064 6972 6563 746f 7279  from a directory
+00017260: 2e2e 2e0a 2020 2020 2222 220a 2020 2020  ....    """.    
+00017270: 666f 6e74 5f66 616d 696c 6965 7320 3d20  font_families = 
+00017280: 7365 7428 290a 2020 2020 666f 7220 5f66  set().    for _f
+00017290: 6920 696e 2051 4469 7228 6469 7265 6374  i in QDir(direct
+000172a0: 6f72 7929 2e65 6e74 7279 496e 666f 4c69  ory).entryInfoLi
+000172b0: 7374 285b 222a 2e74 7466 222c 2022 2a2e  st(["*.ttf", "*.
+000172c0: 776f 6666 222c 2022 2a2e 776f 6666 3222  woff", "*.woff2"
+000172d0: 5d29 3a0a 2020 2020 2020 2020 5f69 6420  ]):.        _id 
+000172e0: 3d20 5146 6f6e 7444 6174 6162 6173 652e  = QFontDatabase.
+000172f0: 6164 6441 7070 6c69 6361 7469 6f6e 466f  addApplicationFo
+00017300: 6e74 285f 6669 2e61 6273 6f6c 7574 6546  nt(_fi.absoluteF
+00017310: 696c 6550 6174 6828 2929 0a20 2020 2020  ilePath()).     
+00017320: 2020 2066 6f6e 745f 6661 6d69 6c69 6573     font_families
+00017330: 207c 3d20 7365 7428 5146 6f6e 7444 6174   |= set(QFontDat
+00017340: 6162 6173 652e 6170 706c 6963 6174 696f  abase.applicatio
+00017350: 6e46 6f6e 7446 616d 696c 6965 7328 5f69  nFontFamilies(_i
+00017360: 6429 290a 2020 2020 7265 7475 726e 2066  d)).    return f
+00017370: 6f6e 745f 6661 6d69 6c69 6573 0a0a 0a64  ont_families...d
+00017380: 6566 2069 6e73 7461 6c6c 5f69 636f 6e73  ef install_icons
+00017390: 2829 3a0a 2020 2020 2222 2249 6e73 7461  ():.    """Insta
+000173a0: 6c6c 2069 636f 6e73 2222 220a 2020 2020  ll icons""".    
+000173b0: 6f73 2e73 7973 7465 6d28 0a20 2020 2020  os.system(.     
+000173c0: 2020 2022 7864 672d 6963 6f6e 2d72 6573     "xdg-icon-res
+000173d0: 6f75 7263 6520 696e 7374 616c 6c20 2d2d  ource install --
+000173e0: 7369 7a65 2033 3220 2d2d 636f 6e74 6578  size 32 --contex
+000173f0: 7420 6170 7073 202d 2d6d 6f64 6520 7573  t apps --mode us
+00017400: 6572 2022 0a20 2020 2020 2020 2066 227b  er ".        f"{
+00017410: 574f 524b 494e 475f 5041 5448 7d2f 6461  WORKING_PATH}/da
+00017420: 7461 2f6b 3667 7465 2e6e 6f74 316d 6d2d  ta/k6gte.not1mm-
+00017430: 3332 2e70 6e67 206b 3667 7465 2d6e 6f74  32.png k6gte-not
+00017440: 316d 6d22 0a20 2020 2029 0a20 2020 206f  1mm".    ).    o
+00017450: 732e 7379 7374 656d 280a 2020 2020 2020  s.system(.      
+00017460: 2020 2278 6467 2d69 636f 6e2d 7265 736f    "xdg-icon-reso
+00017470: 7572 6365 2069 6e73 7461 6c6c 202d 2d73  urce install --s
+00017480: 697a 6520 3634 202d 2d63 6f6e 7465 7874  ize 64 --context
+00017490: 2061 7070 7320 2d2d 6d6f 6465 2075 7365   apps --mode use
+000174a0: 7220 220a 2020 2020 2020 2020 6622 7b57  r ".        f"{W
+000174b0: 4f52 4b49 4e47 5f50 4154 487d 2f64 6174  ORKING_PATH}/dat
+000174c0: 612f 6b36 6774 652e 6e6f 7431 6d6d 2d36  a/k6gte.not1mm-6
+000174d0: 342e 706e 6720 6b36 6774 652d 6e6f 7431  4.png k6gte-not1
+000174e0: 6d6d 220a 2020 2020 290a 2020 2020 6f73  mm".    ).    os
+000174f0: 2e73 7973 7465 6d28 0a20 2020 2020 2020  .system(.       
+00017500: 2022 7864 672d 6963 6f6e 2d72 6573 6f75   "xdg-icon-resou
+00017510: 7263 6520 696e 7374 616c 6c20 2d2d 7369  rce install --si
+00017520: 7a65 2031 3238 202d 2d63 6f6e 7465 7874  ze 128 --context
+00017530: 2061 7070 7320 2d2d 6d6f 6465 2075 7365   apps --mode use
+00017540: 7220 220a 2020 2020 2020 2020 6622 7b57  r ".        f"{W
+00017550: 4f52 4b49 4e47 5f50 4154 487d 2f64 6174  ORKING_PATH}/dat
+00017560: 612f 6b36 6774 652e 6e6f 7431 6d6d 2d31  a/k6gte.not1mm-1
+00017570: 3238 2e70 6e67 206b 3667 7465 2d6e 6f74  28.png k6gte-not
+00017580: 316d 6d22 0a20 2020 2029 0a20 2020 206f  1mm".    ).    o
+00017590: 732e 7379 7374 656d 2866 2278 6467 2d64  s.system(f"xdg-d
+000175a0: 6573 6b74 6f70 2d6d 656e 7520 696e 7374  esktop-menu inst
+000175b0: 616c 6c20 7b57 4f52 4b49 4e47 5f50 4154  all {WORKING_PAT
+000175c0: 487d 2f64 6174 612f 6b36 6774 652d 6e6f  H}/data/k6gte-no
+000175d0: 7431 6d6d 2e64 6573 6b74 6f70 2229 0a0a  t1mm.desktop")..
+000175e0: 0a64 6566 2064 6f69 6d70 286d 6f64 6e61  .def doimp(modna
+000175f0: 6d65 293a 0a20 2020 2022 2222 7265 7475  me):.    """retu
+00017600: 726e 206d 6f64 756c 6520 7061 7468 2222  rn module path""
+00017610: 220a 2020 2020 7265 7475 726e 2069 6d70  ".    return imp
+00017620: 6f72 746c 6962 2e69 6d70 6f72 745f 6d6f  ortlib.import_mo
+00017630: 6475 6c65 2866 226e 6f74 316d 6d2e 706c  dule(f"not1mm.pl
+00017640: 7567 696e 732e 7b6d 6f64 6e61 6d65 7d22  ugins.{modname}"
+00017650: 290a 0a0a 6465 6620 7275 6e28 293a 0a20  )...def run():. 
+00017660: 2020 2022 2222 0a20 2020 204d 6169 6e20     """.    Main 
+00017670: 456e 7472 790a 2020 2020 2222 220a 2020  Entry.    """.  
+00017680: 2020 696e 7374 616c 6c5f 6963 6f6e 7328    install_icons(
+00017690: 290a 2020 2020 7469 6d65 722e 7374 6172  ).    timer.star
+000176a0: 7428 3235 3029 0a20 2020 2073 7973 2e65  t(250).    sys.e
+000176b0: 7869 7428 6170 702e 6578 6563 2829 290a  xit(app.exec()).
+000176c0: 0a0a 6c6f 6767 6572 203d 206c 6f67 6769  ..logger = loggi
+000176d0: 6e67 2e67 6574 4c6f 6767 6572 2822 5f5f  ng.getLogger("__
+000176e0: 6d61 696e 5f5f 2229 0a68 616e 646c 6572  main__").handler
+000176f0: 203d 206c 6f67 6769 6e67 2e53 7472 6561   = logging.Strea
+00017700: 6d48 616e 646c 6572 2829 0a66 6f72 6d61  mHandler().forma
+00017710: 7474 6572 203d 206c 6f67 6769 6e67 2e46  tter = logging.F
+00017720: 6f72 6d61 7474 6572 280a 2020 2020 6461  ormatter(.    da
+00017730: 7465 666d 743d 2225 483a 254d 3a25 5322  tefmt="%H:%M:%S"
+00017740: 2c0a 2020 2020 666d 743d 225b 2528 6173  ,.    fmt="[%(as
+00017750: 6374 696d 6529 735d 2025 286c 6576 656c  ctime)s] %(level
+00017760: 6e61 6d65 2973 2025 286d 6f64 756c 6529  name)s %(module)
+00017770: 7320 2d20 2528 6675 6e63 4e61 6d65 2973  s - %(funcName)s
+00017780: 204c 696e 6520 2528 6c69 6e65 6e6f 2964   Line %(lineno)d
+00017790: 3a20 2528 6d65 7373 6167 6529 7322 2c0a  : %(message)s",.
+000177a0: 290a 6861 6e64 6c65 722e 7365 7446 6f72  ).handler.setFor
+000177b0: 6d61 7474 6572 2866 6f72 6d61 7474 6572  matter(formatter
+000177c0: 290a 6c6f 6767 6572 2e61 6464 4861 6e64  ).logger.addHand
+000177d0: 6c65 7228 6861 6e64 6c65 7229 0a0a 4245  ler(handler)..BE
+000177e0: 5441 5f54 4553 5420 3d20 4661 6c73 650a  TA_TEST = False.
+000177f0: 6966 2050 6174 6828 222e 2f62 6574 6174  if Path("./betat
+00017800: 6573 7422 292e 6578 6973 7473 2829 3a0a  est").exists():.
+00017810: 2020 2020 4245 5441 5f54 4553 5420 3d20      BETA_TEST = 
+00017820: 5472 7565 0a0a 6966 2050 6174 6828 222e  True..if Path(".
+00017830: 2f64 6562 7567 2229 2e65 7869 7374 7328  /debug").exists(
+00017840: 293a 0a20 2020 206c 6f67 6765 722e 7365  ):.    logger.se
+00017850: 744c 6576 656c 286c 6f67 6769 6e67 2e44  tLevel(logging.D
+00017860: 4542 5547 290a 2020 2020 6c6f 6767 6572  EBUG).    logger
+00017870: 2e64 6562 7567 2822 6465 6275 6767 696e  .debug("debuggin
+00017880: 6720 6f6e 2229 0a65 6c73 653a 0a20 2020  g on").else:.   
+00017890: 206c 6f67 6765 722e 7365 744c 6576 656c   logger.setLevel
+000178a0: 286c 6f67 6769 6e67 2e57 4152 4e49 4e47  (logging.WARNING
+000178b0: 290a 2020 2020 6c6f 6767 6572 2e77 6172  ).    logger.war
+000178c0: 6e69 6e67 2822 6465 6275 6767 696e 6720  ning("debugging 
+000178d0: 6f66 6622 290a 0a61 7070 203d 2051 7457  off")..app = QtW
+000178e0: 6964 6765 7473 2e51 4170 706c 6963 6174  idgets.QApplicat
+000178f0: 696f 6e28 7379 732e 6172 6776 290a 6170  ion(sys.argv).ap
+00017900: 702e 7365 7453 7479 6c65 2822 4164 7761  p.setStyle("Adwa
+00017910: 6974 612d 4461 726b 2229 0a66 6f6e 745f  ita-Dark").font_
+00017920: 7061 7468 203d 2057 4f52 4b49 4e47 5f50  path = WORKING_P
+00017930: 4154 4820 2b20 222f 6461 7461 220a 6661  ATH + "/data".fa
+00017940: 6d69 6c69 6573 203d 206c 6f61 645f 666f  milies = load_fo
+00017950: 6e74 735f 6672 6f6d 5f64 6972 286f 732e  nts_from_dir(os.
+00017960: 6673 7061 7468 2866 6f6e 745f 7061 7468  fspath(font_path
+00017970: 2929 0a6c 6f67 6765 722e 696e 666f 2866  )).logger.info(f
+00017980: 616d 696c 6965 7329 0a77 696e 646f 7720  amilies).window 
+00017990: 3d20 4d61 696e 5769 6e64 6f77 2829 0a68  = MainWindow().h
+000179a0: 6569 6768 7420 3d20 7769 6e64 6f77 2e70  eight = window.p
+000179b0: 7265 662e 6765 7428 2277 696e 646f 775f  ref.get("window_
+000179c0: 6865 6967 6874 222c 2033 3030 290a 7769  height", 300).wi
+000179d0: 6474 6820 3d20 7769 6e64 6f77 2e70 7265  dth = window.pre
+000179e0: 662e 6765 7428 2277 696e 646f 775f 7769  f.get("window_wi
+000179f0: 6474 6822 2c20 3730 3029 0a78 203d 2077  dth", 700).x = w
+00017a00: 696e 646f 772e 7072 6566 2e67 6574 2822  indow.pref.get("
+00017a10: 7769 6e64 6f77 5f78 222c 202d 3129 0a79  window_x", -1).y
+00017a20: 203d 2077 696e 646f 772e 7072 6566 2e67   = window.pref.g
+00017a30: 6574 2822 7769 6e64 6f77 5f79 222c 202d  et("window_y", -
+00017a40: 3129 0a77 696e 646f 772e 7365 7447 656f  1).window.setGeo
+00017a50: 6d65 7472 7928 782c 2079 2c20 7769 6474  metry(x, y, widt
+00017a60: 682c 2068 6569 6768 7429 0a77 696e 646f  h, height).windo
+00017a70: 772e 6361 6c6c 7369 676e 2e73 6574 466f  w.callsign.setFo
+00017a80: 6375 7328 290a 7769 6e64 6f77 2e73 686f  cus().window.sho
+00017a90: 7728 290a 7469 6d65 7220 3d20 5174 436f  w().timer = QtCo
+00017aa0: 7265 2e51 5469 6d65 7228 290a 7469 6d65  re.QTimer().time
+00017ab0: 722e 7469 6d65 6f75 742e 636f 6e6e 6563  r.timeout.connec
+00017ac0: 7428 7769 6e64 6f77 2e70 6f6c 6c5f 7261  t(window.poll_ra
+00017ad0: 6469 6f29 0a0a 6966 205f 5f6e 616d 655f  dio)..if __name_
+00017ae0: 5f20 3d3d 2022 5f5f 6d61 696e 5f5f 223a  _ == "__main__":
+00017af0: 0a20 2020 2072 756e 2829 0a              .    run().
```

### Comparing `not1mm-23.8.6/not1mm/bandmap.py` & `not1mm-23.8.7/not1mm/bandmap.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/checkwindow.py` & `not1mm-23.8.7/not1mm/checkwindow.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/JetBrainsMono-Regular.ttf` & `not1mm-23.8.7/not1mm/data/JetBrainsMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/MASTER.SCP` & `not1mm-23.8.7/not1mm/data/MASTER.SCP`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/about.ui` & `not1mm-23.8.7/not1mm/data/about.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/bandmap.ui` & `not1mm-23.8.7/not1mm/data/bandmap.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/checkwindow.ui` & `not1mm-23.8.7/not1mm/data/checkwindow.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/configuration.ui` & `not1mm-23.8.7/not1mm/data/configuration.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/contests.sql` & `not1mm-23.8.7/not1mm/data/contests.sql`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/cty.json` & `not1mm-23.8.7/not1mm/data/cty.json`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/editcontact.ui` & `not1mm-23.8.7/not1mm/data/editcontact.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/editmacro.ui` & `not1mm-23.8.7/not1mm/data/editmacro.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/k6gte.not1mm-128.png` & `not1mm-23.8.7/not1mm/data/k6gte.not1mm-128.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/k6gte.not1mm-32.png` & `not1mm-23.8.7/not1mm/data/k6gte.not1mm-32.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/k6gte.not1mm-64.png` & `not1mm-23.8.7/not1mm/data/k6gte.not1mm-64.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/logwindow.ui` & `not1mm-23.8.7/not1mm/data/logwindow.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/main.ui` & `not1mm-23.8.7/not1mm/data/main.ui`

 * *Files 0% similar despite different names*

#### Comparing `not1mm-23.8.6/not1mm/data/main.ui` & `not1mm-23.8.7/not1mm/data/main.ui`

```diff
@@ -1079,14 +1079,15 @@
       <widget class="QMenu" name="menuWindow">
         <property name="title">
           <string>Window</string>
         </property>
         <addaction name="actionLog_Window"/>
         <addaction name="actionBandmap"/>
         <addaction name="actionCheck_Window"/>
+        <addaction name="actionVFO"/>
       </widget>
       <widget class="QMenu" name="menuOther">
         <property name="title">
           <string>Misc</string>
         </property>
         <addaction name="actionRecalculate_Mults"/>
       </widget>
@@ -1483,11 +1484,16 @@
       </property>
     </action>
     <action name="actionCheck_Window">
       <property name="text">
         <string>Check Window</string>
       </property>
     </action>
+    <action name="actionVFO">
+      <property name="text">
+        <string>VFO</string>
+      </property>
+    </action>
   </widget>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `not1mm-23.8.6/not1mm/data/new_contest.ui` & `not1mm-23.8.7/not1mm/data/new_contest.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/not1mm.html` & `not1mm-23.8.7/not1mm/data/not1mm.html`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/opon.ui` & `not1mm-23.8.7/not1mm/data/opon.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/0.wav` & `not1mm-23.8.7/not1mm/data/phonetics/0.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/1.wav` & `not1mm-23.8.7/not1mm/data/phonetics/1.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/2.wav` & `not1mm-23.8.7/not1mm/data/phonetics/2.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/3.wav` & `not1mm-23.8.7/not1mm/data/phonetics/3.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/4.wav` & `not1mm-23.8.7/not1mm/data/phonetics/4.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/5.wav` & `not1mm-23.8.7/not1mm/data/phonetics/5.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/6.wav` & `not1mm-23.8.7/not1mm/data/phonetics/6.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/7.wav` & `not1mm-23.8.7/not1mm/data/phonetics/7.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/73.wav` & `not1mm-23.8.7/not1mm/data/phonetics/73.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/8.wav` & `not1mm-23.8.7/not1mm/data/phonetics/8.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/9.wav` & `not1mm-23.8.7/not1mm/data/phonetics/9.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/a.wav` & `not1mm-23.8.7/not1mm/data/phonetics/a.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/again.wav` & `not1mm-23.8.7/not1mm/data/phonetics/again.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/b.wav` & `not1mm-23.8.7/not1mm/data/phonetics/b.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/c.wav` & `not1mm-23.8.7/not1mm/data/phonetics/c.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/contest.wav` & `not1mm-23.8.7/not1mm/data/phonetics/contest.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/cq.wav` & `not1mm-23.8.7/not1mm/data/phonetics/cq.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/d.wav` & `not1mm-23.8.7/not1mm/data/phonetics/d.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/e.wav` & `not1mm-23.8.7/not1mm/data/phonetics/e.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/f.wav` & `not1mm-23.8.7/not1mm/data/phonetics/f.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/g.wav` & `not1mm-23.8.7/not1mm/data/phonetics/g.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/h.wav` & `not1mm-23.8.7/not1mm/data/phonetics/h.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/i.wav` & `not1mm-23.8.7/not1mm/data/phonetics/i.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/j.wav` & `not1mm-23.8.7/not1mm/data/phonetics/j.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/k.wav` & `not1mm-23.8.7/not1mm/data/phonetics/k.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/k6gte.wav` & `not1mm-23.8.7/not1mm/data/phonetics/k6gte.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/l.wav` & `not1mm-23.8.7/not1mm/data/phonetics/l.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/m.wav` & `not1mm-23.8.7/not1mm/data/phonetics/m.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/mynumber.wav` & `not1mm-23.8.7/not1mm/data/phonetics/mynumber.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/n.wav` & `not1mm-23.8.7/not1mm/data/phonetics/n.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/nil.wav` & `not1mm-23.8.7/not1mm/data/phonetics/nil.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/o.wav` & `not1mm-23.8.7/not1mm/data/phonetics/o.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/p.wav` & `not1mm-23.8.7/not1mm/data/phonetics/p.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/q.wav` & `not1mm-23.8.7/not1mm/data/phonetics/q.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/r.wav` & `not1mm-23.8.7/not1mm/data/phonetics/r.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/roger.wav` & `not1mm-23.8.7/not1mm/data/phonetics/roger.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/s.wav` & `not1mm-23.8.7/not1mm/data/phonetics/s.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/space.wav` & `not1mm-23.8.7/not1mm/data/phonetics/space.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/t.wav` & `not1mm-23.8.7/not1mm/data/phonetics/t.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/thankyou.wav` & `not1mm-23.8.7/not1mm/data/phonetics/thankyou.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/thankyouqrz.wav` & `not1mm-23.8.7/not1mm/data/phonetics/thankyouqrz.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/u.wav` & `not1mm-23.8.7/not1mm/data/phonetics/u.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/v.wav` & `not1mm-23.8.7/not1mm/data/phonetics/v.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/w.wav` & `not1mm-23.8.7/not1mm/data/phonetics/w.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/x.wav` & `not1mm-23.8.7/not1mm/data/phonetics/x.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/y.wav` & `not1mm-23.8.7/not1mm/data/phonetics/y.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/yourcall.wav` & `not1mm-23.8.7/not1mm/data/phonetics/yourcall.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/phonetics/z.wav` & `not1mm-23.8.7/not1mm/data/phonetics/z.wav`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/pickcontest.ui` & `not1mm-23.8.7/not1mm/data/pickcontest.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/reddot.png` & `not1mm-23.8.7/not1mm/data/reddot.png`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/data/settings.ui` & `not1mm-23.8.7/not1mm/data/settings.ui`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/lib/cat_interface.py` & `not1mm-23.8.7/not1mm/lib/cat_interface.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/lib/cwinterface.py` & `not1mm-23.8.7/not1mm/lib/cwinterface.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/lib/database.py` & `not1mm-23.8.7/not1mm/lib/database.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/lib/edit_macro.py` & `not1mm-23.8.7/not1mm/lib/edit_macro.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/lib/edit_station.py` & `not1mm-23.8.7/not1mm/lib/edit_station.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/lib/ham_utility.py` & `not1mm-23.8.7/not1mm/lib/ham_utility.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/lib/lookup.py` & `not1mm-23.8.7/not1mm/lib/lookup.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/lib/multicast.py` & `not1mm-23.8.7/not1mm/lib/multicast.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/lib/n1mm.py` & `not1mm-23.8.7/not1mm/lib/n1mm.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/lib/settings.py` & `not1mm-23.8.7/not1mm/lib/settings.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/lib/super_check_partial.py` & `not1mm-23.8.7/not1mm/lib/super_check_partial.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/lib/versiontest.py` & `not1mm-23.8.7/not1mm/lib/versiontest.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/logwindow.py` & `not1mm-23.8.7/not1mm/logwindow.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/plugins/10_10_fall_cw.py` & `not1mm-23.8.7/not1mm/plugins/10_10_fall_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/plugins/10_10_spring_cw.py` & `not1mm-23.8.7/not1mm/plugins/10_10_spring_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/plugins/10_10_summer_phone.py` & `not1mm-23.8.7/not1mm/plugins/10_10_summer_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/plugins/10_10_winter_phone.py` & `not1mm-23.8.7/not1mm/plugins/10_10_winter_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/plugins/arrl_dx_cw.py` & `not1mm-23.8.7/not1mm/plugins/arrl_dx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/plugins/arrl_dx_ssb.py` & `not1mm-23.8.7/not1mm/plugins/arrl_dx_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/plugins/arrl_field_day.py` & `not1mm-23.8.7/not1mm/plugins/arrl_field_day.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/plugins/arrl_rtty_ru.py` & `not1mm-23.8.7/not1mm/plugins/arrl_rtty_ru.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/plugins/arrl_ss_cw.py` & `not1mm-23.8.7/not1mm/plugins/arrl_ss_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/plugins/arrl_ss_phone.py` & `not1mm-23.8.7/not1mm/plugins/arrl_ss_phone.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/plugins/canada_day.py` & `not1mm-23.8.7/not1mm/plugins/canada_day.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/plugins/cq_wpx_cw.py` & `not1mm-23.8.7/not1mm/plugins/cq_wpx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/plugins/cq_wpx_ssb.py` & `not1mm-23.8.7/not1mm/plugins/cq_wpx_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/plugins/cq_ww_cw.py` & `not1mm-23.8.7/not1mm/plugins/cq_ww_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/plugins/cq_ww_ssb.py` & `not1mm-23.8.7/not1mm/plugins/cq_ww_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/plugins/cwt.py` & `not1mm-23.8.7/not1mm/plugins/cwt.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/plugins/general_logging.py` & `not1mm-23.8.7/not1mm/plugins/general_logging.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/plugins/iaru_hf.py` & `not1mm-23.8.7/not1mm/plugins/iaru_hf.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/plugins/jidx_cw.py` & `not1mm-23.8.7/not1mm/plugins/jidx_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/plugins/jidx_ph.py` & `not1mm-23.8.7/not1mm/plugins/jidx_ph.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/plugins/naqp_cw.py` & `not1mm-23.8.7/not1mm/plugins/naqp_cw.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/plugins/naqp_ssb.py` & `not1mm-23.8.7/not1mm/plugins/naqp_ssb.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/plugins/winter_field_day.py` & `not1mm-23.8.7/not1mm/plugins/winter_field_day.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/testing/fakeflrig.py` & `not1mm-23.8.7/not1mm/testing/fakeflrig.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/testing/flrigclient.py` & `not1mm-23.8.7/not1mm/testing/flrigclient.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/testing/multicast_listener.py` & `not1mm-23.8.7/not1mm/testing/multicast_listener.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/testing/n1mm_listener.py` & `not1mm-23.8.7/not1mm/testing/n1mm_listener.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm/testing/test.py` & `not1mm-23.8.7/not1mm/testing/test.py`

 * *Files identical despite different names*

### Comparing `not1mm-23.8.6/not1mm.egg-info/PKG-INFO` & `not1mm-23.8.7/not1mm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not1mm
-Version: 23.8.6
+Version: 23.8.7
 Summary: NOT1MM Logger
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/not1mm
 Project-URL: Bug Tracker, https://github.com/mbridak/not1mm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -77,14 +77,15 @@
     - [The Main Window](#the-main-window)
       - [Keyboard commands](#keyboard-commands)
     - [Log Display](#log-display)
       - [Editing a contact](#editing-a-contact)
   - [Recalulate Mults](#recalulate-mults)
   - [Bandmap](#bandmap)
   - [Check Window](#check-window)
+  - [VFO](#vfo)
   - [Cabrillo](#cabrillo)
   - [ADIF](#adif)
   - [Dupe checking](#dupe-checking)
   - [Contest specific notes](#contest-specific-notes)
     - [ARRL Sweekstakes](#arrl-sweekstakes)
       - [The exchange parser](#the-exchange-parser)
       - [The exchange](#the-exchange)
@@ -138,14 +139,15 @@
 - Japan International DX SSB
 - NAQP CW
 - NAQP SSB
 - RAC Canada Day
 
 ## Recent Changes
 
+- [23-8-7] Control Remote Rig VFO with a bespoke USB VFO Knob.
 - [23-8-6] Add parsing of local log to check window.
 - [23-8-5] Add Check Window. Moved MASTER.SCP stuff to it's own class. Close sub windows when main app closes.
 
 See [CHANGELOG.md](CHANGELOG.md) for prior changes.
 
 ## Installing from PyPi
 
@@ -474,14 +476,23 @@
 
 `Window`>`Check Window`
 
 As you enter a callsign, the Check Window will show probable matches to calls either in the MASTER.SCP file, or your local log. The MASTER.SCP column will show results for strings of 3 or more matching from the start of the call string. The local log column will show matches of any length appearing anywhere in the string.
 
 ![Check Window](https://github.com/mbridak/not1mm/raw/master/pic/checkwindow.png)
 
+## VFO
+
+You can control the VFO on a remote rig by:
+
+1. Making the [VFO](https://github.com/mbridak/not1mm/blob/master/usb_vfo_knob/vfo.md)...
+2. Then... `Window`>`VFO`
+
+![VFO](https://github.com/mbridak/not1mm/raw/master/usb_vfo_knob/vfo.gif)
+
 ## Cabrillo
 
 Click on `File` > `Generate Cabrillo`
 
 The file will be placed in your home directory. The name will be in the format of:
 
 `StationCall`_`ContestName`.log
```

### Comparing `not1mm-23.8.6/not1mm.egg-info/SOURCES.txt` & `not1mm-23.8.7/not1mm.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 pyproject.toml
 not1mm/__init__.py
 not1mm/__main__.py
 not1mm/bandmap.py
 not1mm/checkwindow.py
 not1mm/logwindow.py
+not1mm/vfo.py
 not1mm.egg-info/PKG-INFO
 not1mm.egg-info/SOURCES.txt
 not1mm.egg-info/dependency_links.txt
 not1mm.egg-info/entry_points.txt
 not1mm.egg-info/requires.txt
 not1mm.egg-info/top_level.txt
 not1mm/data/JetBrainsMono-Regular.ttf
@@ -36,14 +37,15 @@
 not1mm/data/new_contest.ui
 not1mm/data/not1mm.html
 not1mm/data/opon.ui
 not1mm/data/pickcontest.ui
 not1mm/data/reddot.png
 not1mm/data/settings.ui
 not1mm/data/ssbmacros.txt
+not1mm/data/vfo.ui
 not1mm/data/phonetics/0.wav
 not1mm/data/phonetics/1.wav
 not1mm/data/phonetics/2.wav
 not1mm/data/phonetics/3.wav
 not1mm/data/phonetics/4.wav
 not1mm/data/phonetics/5.wav
 not1mm/data/phonetics/6.wav
@@ -132,8 +134,9 @@
 not1mm/plugins/naqp_ssb.py
 not1mm/plugins/winter_field_day.py
 not1mm/testing/fakeflrig.py
 not1mm/testing/flrigclient.py
 not1mm/testing/multicast_listener.py
 not1mm/testing/n1mm_listener.py
 not1mm/testing/test.py
-testing/test.py
+testing/test.py
+usb_vfo_knob/code.py
```

### Comparing `not1mm-23.8.6/pyproject.toml` & `not1mm-23.8.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "not1mm" 
-version = "23.8.6"
+version = "23.8.7"
 description = "NOT1MM Logger"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
 dependencies = [
```

