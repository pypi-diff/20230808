# Comparing `tmp/ayla-1.0.3.tar.gz` & `tmp/ayla-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayla-1.0.3.tar", max compression
+gzip compressed data, was "ayla-1.0.4.tar", max compression
```

## Comparing `ayla-1.0.3.tar` & `ayla-1.0.4.tar`

### file list

```diff
@@ -1,29 +1,21 @@
--rwxr-xr-x   0        0        0     1201 2023-03-16 05:20:27.975394 ayla-1.0.3/Ayla/__init__.py
--rwxr-xr-x   0        0        0     1123 2023-03-25 04:48:24.915937 ayla-1.0.3/Ayla/ayla.egg-info/PKG-INFO
--rwxr-xr-x   0        0        0      361 2023-03-25 04:48:24.934191 ayla-1.0.3/Ayla/ayla.egg-info/SOURCES.txt
--rwxr-xr-x   0        0        0        1 2023-03-25 04:48:24.915937 ayla-1.0.3/Ayla/ayla.egg-info/dependency_links.txt
--rwxr-xr-x   0        0        0       14 2023-03-25 04:48:24.916937 ayla-1.0.3/Ayla/ayla.egg-info/requires.txt
--rwxr-xr-x   0        0        0       23 2023-03-25 04:48:24.918936 ayla-1.0.3/Ayla/ayla.egg-info/top_level.txt
--rwxr-xr-x   0        0        0     1126 2023-03-15 04:28:59.324531 ayla-1.0.3/Ayla/cards/__init__.py
--rwxr-xr-x   0        0        0     1276 2023-03-25 04:35:22.554521 ayla-1.0.3/Ayla/cards/__pycache__/__init__.cpython-39.pyc
--rwxr-xr-x   0        0        0     6706 2023-03-25 04:35:22.558032 ayla-1.0.3/Ayla/cards/__pycache__/card.cpython-39.pyc
--rwxr-xr-x   0        0        0        0 2023-03-20 03:46:26.405743 ayla-1.0.3/Ayla/cards/assets/__init__.py
--rwxr-xr-x   0        0        0      842 2023-01-24 08:46:18.000000 ayla-1.0.3/Ayla/cards/assets/curveborder.png
--rwxr-xr-x   0        0        0     2710 2023-02-18 02:17:04.000000 ayla-1.0.3/Ayla/cards/assets/curvedoverlay.png
--rwxr-xr-x   0        0        0        0 2023-03-20 03:46:34.392685 ayla-1.0.3/Ayla/cards/assets/fonts/__init__.py
--rwxr-xr-x   0        0        0    66976 2019-11-25 21:12:12.000000 ayla-1.0.3/Ayla/cards/assets/fonts/juice.otf
--rwxr-xr-x   0        0        0    60288 2023-01-24 08:46:18.000000 ayla-1.0.3/Ayla/cards/assets/fonts/levelfont.otf
--rwxr-xr-x   0        0        0   141612 2022-09-22 02:39:26.000000 ayla-1.0.3/Ayla/cards/assets/fonts/poppins.ttf
--rwxr-xr-x   0        0        0    26156 2012-09-26 21:36:18.000000 ayla-1.0.3/Ayla/cards/assets/fonts/rabbit.ttf
--rwxr-xr-x   0        0        0     9742 2023-01-24 08:46:18.000000 ayla-1.0.3/Ayla/cards/assets/mask_circle.jpg
--rwxr-xr-x   0        0        0     6394 2023-01-24 08:46:18.000000 ayla-1.0.3/Ayla/cards/assets/overlay1.png
--rwxr-xr-x   0        0        0     1339 2023-02-12 14:41:14.000000 ayla-1.0.3/Ayla/cards/assets/pic.png
--rwxr-xr-x   0        0        0      318 2023-02-17 05:28:00.000000 ayla-1.0.3/Ayla/cards/assets/transparent_mask.png
--rwxr-xr-x   0        0        0     9987 2023-03-16 05:09:41.540526 ayla-1.0.3/Ayla/cards/card.py
--rwxr-xr-x   0        0        0     1181 2023-03-16 04:31:17.158782 ayla-1.0.3/Ayla/errors/__init__.py
--rwxr-xr-x   0        0        0     1453 2023-03-25 04:35:22.566041 ayla-1.0.3/Ayla/errors/__pycache__/__init__.cpython-39.pyc
--rwxr-xr-x   0        0        0     1100 2023-03-15 04:08:47.084140 ayla-1.0.3/Ayla/scrobbles/__init__.py
--rwxr-xr-x   0        0        0     1067 2023-03-15 04:30:01.510284 ayla-1.0.3/LICENSE
--rwxr-xr-x   0        0        0      303 2023-03-16 02:25:08.662548 ayla-1.0.3/README.md
--rw-r--r--   0        0        0      588 2023-08-06 23:13:39.688187 ayla-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1097 1970-01-01 00:00:00.000000 ayla-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1201 2023-03-16 05:20:27.975394 ayla-1.0.4/Ayla/__init__.py
+-rw-r--r--   0        0        0     1126 2023-03-15 04:28:59.324531 ayla-1.0.4/Ayla/cards/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-20 03:46:26.405743 ayla-1.0.4/Ayla/cards/assets/__init__.py
+-rw-r--r--   0        0        0      842 2023-01-24 08:46:18.000000 ayla-1.0.4/Ayla/cards/assets/curveborder.png
+-rw-r--r--   0        0        0     2710 2023-02-18 02:17:04.000000 ayla-1.0.4/Ayla/cards/assets/curvedoverlay.png
+-rw-r--r--   0        0        0        0 2023-03-20 03:46:34.392685 ayla-1.0.4/Ayla/cards/assets/fonts/__init__.py
+-rw-r--r--   0        0        0    66976 2019-11-25 21:12:12.000000 ayla-1.0.4/Ayla/cards/assets/fonts/juice.otf
+-rw-r--r--   0        0        0    60288 2023-01-24 08:46:18.000000 ayla-1.0.4/Ayla/cards/assets/fonts/levelfont.otf
+-rw-r--r--   0        0        0   141612 2022-09-22 02:39:26.000000 ayla-1.0.4/Ayla/cards/assets/fonts/poppins.ttf
+-rw-r--r--   0        0        0    26156 2012-09-26 21:36:18.000000 ayla-1.0.4/Ayla/cards/assets/fonts/rabbit.ttf
+-rw-r--r--   0        0        0     9742 2023-01-24 08:46:18.000000 ayla-1.0.4/Ayla/cards/assets/mask_circle.jpg
+-rw-r--r--   0        0        0     6394 2023-01-24 08:46:18.000000 ayla-1.0.4/Ayla/cards/assets/overlay1.png
+-rw-r--r--   0        0        0     1339 2023-02-12 14:41:14.000000 ayla-1.0.4/Ayla/cards/assets/pic.png
+-rw-r--r--   0        0        0      318 2023-02-17 05:28:00.000000 ayla-1.0.4/Ayla/cards/assets/transparent_mask.png
+-rw-r--r--   0        0        0     9887 2023-08-08 00:16:14.990905 ayla-1.0.4/Ayla/cards/card.py
+-rw-r--r--   0        0        0     1181 2023-03-16 04:31:17.158782 ayla-1.0.4/Ayla/errors/__init__.py
+-rw-r--r--   0        0        0     1100 2023-03-15 04:08:47.084140 ayla-1.0.4/Ayla/scrobbles/__init__.py
+-rw-r--r--   0        0        0     1067 2023-03-15 04:30:01.510284 ayla-1.0.4/LICENSE
+-rw-r--r--   0        0        0      588 2023-08-08 00:17:26.691150 ayla-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      303 2023-03-16 02:25:08.662548 ayla-1.0.4/README.md
+-rw-r--r--   0        0        0     1097 1970-01-01 00:00:00.000000 ayla-1.0.4/PKG-INFO
```

### Comparing `ayla-1.0.3/Ayla/__init__.py` & `ayla-1.0.4/Ayla/__init__.py`

 * *Files identical despite different names*

### Comparing `ayla-1.0.3/Ayla/ayla.egg-info/PKG-INFO` & `ayla-1.0.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,47 @@
-Metadata-Version: 2.1
-Name: ayla
-Version: 1.0.3
-Summary: Some functions used in KuuhakuTeam projects
-Home-page: https://github.com/KuuhakuTeam/Ayla
-Author: fnixdev
-Author-email: luisgatn000@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Requires-Python: >3.6, <3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-## Usage
-
-```py
-from ayla import RankCard
-
-rank = RankCard(
-    pfp=pfp,
-    background=bg,
-    nickname=nick,
-    level=level,
-    current_xp=current,
-    xp_max=max_xp,
-    text_color=text_color,
-    bar_color=bar_color
-)
-
-image = rank.card1()
-```
-<br>
-
-## Functions
-
-- RankCard
-- ScrobbleCard (soon)
-
+Metadata-Version: 2.1
+Name: ayla
+Version: 1.0.4
+Summary: Some functions used in KuuhakuTeam projects
+Home-page: https://github.com/KuuhakuTeam/Ayla
+License: MIT
+Keywords: leveling,card,image
+Author: fnixdev
+Author-email: fenixdev@outlook.com
+Requires-Python: >=3.8,<4
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Pillow (>=9.2.0,<10.0.0)
+Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Project-URL: Repository, https://github.com/KuuhakuTeam/Ayla
+Description-Content-Type: text/markdown
+
+
+## Usage
+
+```py
+from ayla import RankCard
+
+rank = RankCard(
+    pfp=pfp,
+    background=bg,
+    nickname=nick,
+    level=level,
+    current_xp=current,
+    xp_max=max_xp,
+    text_color=text_color,
+    bar_color=bar_color
+)
+
+image = rank.card1()
+```
+<br>
+
+## Functions
+
+- RankCard
+- ScrobbleCard (soon)
```

### Comparing `ayla-1.0.3/Ayla/cards/__init__.py` & `ayla-1.0.4/Ayla/cards/__init__.py`

 * *Files identical despite different names*

### Comparing `ayla-1.0.3/Ayla/cards/__pycache__/__init__.cpython-39.pyc` & `ayla-1.0.4/LICENSE`

 * *Files 23% similar despite different names*

```diff
@@ -1,80 +1,67 @@
-00000000: 610d 0d0a 0000 0000 8b49 1164 6604 0000  a........I.df...
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 1400 0000 6400  .....@...s....d.
-00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6403  Z.d.d.l.m.Z...d.
-00000040: 5300 2904 612d 0400 000a 6b75 7568 616b  S.).a-....kuuhak
-00000050: 7520 7631 2e30 0a43 6f70 7972 6967 6874  u v1.0.Copyright
-00000060: 2028 6329 2032 3032 3320 4b75 7568 616b   (c) 2023 Kuuhak
-00000070: 7554 6561 6d0a 0a50 6572 6d69 7373 696f  uTeam..Permissio
-00000080: 6e20 6973 2068 6572 6562 7920 6772 616e  n is hereby gran
-00000090: 7465 642c 2066 7265 6520 6f66 2063 6861  ted, free of cha
-000000a0: 7267 652c 2074 6f20 616e 7920 7065 7273  rge, to any pers
-000000b0: 6f6e 206f 6274 6169 6e69 6e67 2061 2063  on obtaining a c
-000000c0: 6f70 790a 6f66 2074 6869 7320 736f 6674  opy.of this soft
-000000d0: 7761 7265 2061 6e64 2061 7373 6f63 6961  ware and associa
-000000e0: 7465 6420 646f 6375 6d65 6e74 6174 696f  ted documentatio
-000000f0: 6e20 6669 6c65 7320 2874 6865 2022 536f  n files (the "So
-00000100: 6674 7761 7265 2229 2c20 746f 2064 6561  ftware"), to dea
-00000110: 6c0a 696e 2074 6865 2053 6f66 7477 6172  l.in the Softwar
-00000120: 6520 7769 7468 6f75 7420 7265 7374 7269  e without restri
-00000130: 6374 696f 6e2c 2069 6e63 6c75 6469 6e67  ction, including
-00000140: 2077 6974 686f 7574 206c 696d 6974 6174   without limitat
-00000150: 696f 6e20 7468 6520 7269 6768 7473 0a74  ion the rights.t
-00000160: 6f20 7573 652c 2063 6f70 792c 206d 6f64  o use, copy, mod
-00000170: 6966 792c 206d 6572 6765 2c20 7075 626c  ify, merge, publ
-00000180: 6973 682c 2064 6973 7472 6962 7574 652c  ish, distribute,
-00000190: 2073 7562 6c69 6365 6e73 652c 2061 6e64   sublicense, and
-000001a0: 2f6f 7220 7365 6c6c 0a63 6f70 6965 7320  /or sell.copies 
-000001b0: 6f66 2074 6865 2053 6f66 7477 6172 652c  of the Software,
-000001c0: 2061 6e64 2074 6f20 7065 726d 6974 2070   and to permit p
-000001d0: 6572 736f 6e73 2074 6f20 7768 6f6d 2074  ersons to whom t
-000001e0: 6865 2053 6f66 7477 6172 6520 6973 0a66  he Software is.f
-000001f0: 7572 6e69 7368 6564 2074 6f20 646f 2073  urnished to do s
-00000200: 6f2c 2073 7562 6a65 6374 2074 6f20 7468  o, subject to th
-00000210: 6520 666f 6c6c 6f77 696e 6720 636f 6e64  e following cond
-00000220: 6974 696f 6e73 3a0a 0a54 6865 2061 626f  itions:..The abo
-00000230: 7665 2063 6f70 7972 6967 6874 206e 6f74  ve copyright not
-00000240: 6963 6520 616e 6420 7468 6973 2070 6572  ice and this per
-00000250: 6d69 7373 696f 6e20 6e6f 7469 6365 2073  mission notice s
-00000260: 6861 6c6c 2062 6520 696e 636c 7564 6564  hall be included
-00000270: 2069 6e20 616c 6c0a 636f 7069 6573 206f   in all.copies o
-00000280: 7220 7375 6273 7461 6e74 6961 6c20 706f  r substantial po
-00000290: 7274 696f 6e73 206f 6620 7468 6520 536f  rtions of the So
-000002a0: 6674 7761 7265 2e0a 0a54 4845 2053 4f46  ftware...THE SOF
-000002b0: 5457 4152 4520 4953 2050 524f 5649 4445  TWARE IS PROVIDE
-000002c0: 4420 2241 5320 4953 222c 2057 4954 484f  D "AS IS", WITHO
-000002d0: 5554 2057 4152 5241 4e54 5920 4f46 2041  UT WARRANTY OF A
-000002e0: 4e59 204b 494e 442c 2045 5850 5245 5353  NY KIND, EXPRESS
-000002f0: 204f 520a 494d 504c 4945 442c 2049 4e43   OR.IMPLIED, INC
-00000300: 4c55 4449 4e47 2042 5554 204e 4f54 204c  LUDING BUT NOT L
-00000310: 494d 4954 4544 2054 4f20 5448 4520 5741  IMITED TO THE WA
-00000320: 5252 414e 5449 4553 204f 4620 4d45 5243  RRANTIES OF MERC
-00000330: 4841 4e54 4142 494c 4954 592c 0a46 4954  HANTABILITY,.FIT
-00000340: 4e45 5353 2046 4f52 2041 2050 4152 5449  NESS FOR A PARTI
-00000350: 4355 4c41 5220 5055 5250 4f53 4520 414e  CULAR PURPOSE AN
-00000360: 4420 4e4f 4e49 4e46 5249 4e47 454d 454e  D NONINFRINGEMEN
-00000370: 542e 2049 4e20 4e4f 2045 5645 4e54 2053  T. IN NO EVENT S
-00000380: 4841 4c4c 2054 4845 0a41 5554 484f 5253  HALL THE.AUTHORS
-00000390: 204f 5220 434f 5059 5249 4748 5420 484f   OR COPYRIGHT HO
-000003a0: 4c44 4552 5320 4245 204c 4941 424c 4520  LDERS BE LIABLE 
-000003b0: 464f 5220 414e 5920 434c 4149 4d2c 2044  FOR ANY CLAIM, D
-000003c0: 414d 4147 4553 204f 5220 4f54 4845 520a  AMAGES OR OTHER.
-000003d0: 4c49 4142 494c 4954 592c 2057 4845 5448  LIABILITY, WHETH
-000003e0: 4552 2049 4e20 414e 2041 4354 494f 4e20  ER IN AN ACTION 
-000003f0: 4f46 2043 4f4e 5452 4143 542c 2054 4f52  OF CONTRACT, TOR
-00000400: 5420 4f52 204f 5448 4552 5749 5345 2c20  T OR OTHERWISE, 
-00000410: 4152 4953 494e 4720 4652 4f4d 2c0a 4f55  ARISING FROM,.OU
-00000420: 5420 4f46 204f 5220 494e 2043 4f4e 4e45  T OF OR IN CONNE
-00000430: 4354 494f 4e20 5749 5448 2054 4845 2053  CTION WITH THE S
-00000440: 4f46 5457 4152 4520 4f52 2054 4845 2055  OFTWARE OR THE U
-00000450: 5345 204f 5220 4f54 4845 5220 4445 414c  SE OR OTHER DEAL
-00000460: 494e 4753 2049 4e20 5448 450a 534f 4654  INGS IN THE.SOFT
-00000470: 5741 5245 2e0a e901 0000 0029 01da 0852  WARE.......)...R
-00000480: 616e 6b43 6172 644e 2903 da07 5f5f 646f  ankCardN)...__do
-00000490: 635f 5f5a 0463 6172 6472 0200 0000 a900  c__Z.cardr......
-000004a0: 7204 0000 0072 0400 0000 fa3b 433a 5c55  r....r.....;C:\U
-000004b0: 7365 7273 5c66 6e69 785c 5265 706f 735c  sers\fnix\Repos\
-000004c0: 4b75 7568 616b 7554 6561 6d5c 4179 6c61  KuuhakuTeam\Ayla
-000004d0: 5c61 796c 615c 6361 7264 735c 5f5f 696e  \ayla\cards\__in
-000004e0: 6974 5f5f 2e70 79da 083c 6d6f 6475 6c65  it__.py..<module
-000004f0: 3e01 0000 0073 0200 0000 0417            >....s......
+00000000: 4d49 5420 4c69 6365 6e73 650a 0a43 6f70  MIT License..Cop
+00000010: 7972 6967 6874 2028 6329 2032 3032 3320  yright (c) 2023 
+00000020: 4b75 7568 616b 7554 6561 6d0a 0a50 6572  KuuhakuTeam..Per
+00000030: 6d69 7373 696f 6e20 6973 2068 6572 6562  mission is hereb
+00000040: 7920 6772 616e 7465 642c 2066 7265 6520  y granted, free 
+00000050: 6f66 2063 6861 7267 652c 2074 6f20 616e  of charge, to an
+00000060: 7920 7065 7273 6f6e 206f 6274 6169 6e69  y person obtaini
+00000070: 6e67 2061 2063 6f70 790a 6f66 2074 6869  ng a copy.of thi
+00000080: 7320 736f 6674 7761 7265 2061 6e64 2061  s software and a
+00000090: 7373 6f63 6961 7465 6420 646f 6375 6d65  ssociated docume
+000000a0: 6e74 6174 696f 6e20 6669 6c65 7320 2874  ntation files (t
+000000b0: 6865 2022 536f 6674 7761 7265 2229 2c20  he "Software"), 
+000000c0: 746f 2064 6561 6c0a 696e 2074 6865 2053  to deal.in the S
+000000d0: 6f66 7477 6172 6520 7769 7468 6f75 7420  oftware without 
+000000e0: 7265 7374 7269 6374 696f 6e2c 2069 6e63  restriction, inc
+000000f0: 6c75 6469 6e67 2077 6974 686f 7574 206c  luding without l
+00000100: 696d 6974 6174 696f 6e20 7468 6520 7269  imitation the ri
+00000110: 6768 7473 0a74 6f20 7573 652c 2063 6f70  ghts.to use, cop
+00000120: 792c 206d 6f64 6966 792c 206d 6572 6765  y, modify, merge
+00000130: 2c20 7075 626c 6973 682c 2064 6973 7472  , publish, distr
+00000140: 6962 7574 652c 2073 7562 6c69 6365 6e73  ibute, sublicens
+00000150: 652c 2061 6e64 2f6f 7220 7365 6c6c 0a63  e, and/or sell.c
+00000160: 6f70 6965 7320 6f66 2074 6865 2053 6f66  opies of the Sof
+00000170: 7477 6172 652c 2061 6e64 2074 6f20 7065  tware, and to pe
+00000180: 726d 6974 2070 6572 736f 6e73 2074 6f20  rmit persons to 
+00000190: 7768 6f6d 2074 6865 2053 6f66 7477 6172  whom the Softwar
+000001a0: 6520 6973 0a66 7572 6e69 7368 6564 2074  e is.furnished t
+000001b0: 6f20 646f 2073 6f2c 2073 7562 6a65 6374  o do so, subject
+000001c0: 2074 6f20 7468 6520 666f 6c6c 6f77 696e   to the followin
+000001d0: 6720 636f 6e64 6974 696f 6e73 3a0a 0a54  g conditions:..T
+000001e0: 6865 2061 626f 7665 2063 6f70 7972 6967  he above copyrig
+000001f0: 6874 206e 6f74 6963 6520 616e 6420 7468  ht notice and th
+00000200: 6973 2070 6572 6d69 7373 696f 6e20 6e6f  is permission no
+00000210: 7469 6365 2073 6861 6c6c 2062 6520 696e  tice shall be in
+00000220: 636c 7564 6564 2069 6e20 616c 6c0a 636f  cluded in all.co
+00000230: 7069 6573 206f 7220 7375 6273 7461 6e74  pies or substant
+00000240: 6961 6c20 706f 7274 696f 6e73 206f 6620  ial portions of 
+00000250: 7468 6520 536f 6674 7761 7265 2e0a 0a54  the Software...T
+00000260: 4845 2053 4f46 5457 4152 4520 4953 2050  HE SOFTWARE IS P
+00000270: 524f 5649 4445 4420 2241 5320 4953 222c  ROVIDED "AS IS",
+00000280: 2057 4954 484f 5554 2057 4152 5241 4e54   WITHOUT WARRANT
+00000290: 5920 4f46 2041 4e59 204b 494e 442c 2045  Y OF ANY KIND, E
+000002a0: 5850 5245 5353 204f 520a 494d 504c 4945  XPRESS OR.IMPLIE
+000002b0: 442c 2049 4e43 4c55 4449 4e47 2042 5554  D, INCLUDING BUT
+000002c0: 204e 4f54 204c 494d 4954 4544 2054 4f20   NOT LIMITED TO 
+000002d0: 5448 4520 5741 5252 414e 5449 4553 204f  THE WARRANTIES O
+000002e0: 4620 4d45 5243 4841 4e54 4142 494c 4954  F MERCHANTABILIT
+000002f0: 592c 0a46 4954 4e45 5353 2046 4f52 2041  Y,.FITNESS FOR A
+00000300: 2050 4152 5449 4355 4c41 5220 5055 5250   PARTICULAR PURP
+00000310: 4f53 4520 414e 4420 4e4f 4e49 4e46 5249  OSE AND NONINFRI
+00000320: 4e47 454d 454e 542e 2049 4e20 4e4f 2045  NGEMENT. IN NO E
+00000330: 5645 4e54 2053 4841 4c4c 2054 4845 0a41  VENT SHALL THE.A
+00000340: 5554 484f 5253 204f 5220 434f 5059 5249  UTHORS OR COPYRI
+00000350: 4748 5420 484f 4c44 4552 5320 4245 204c  GHT HOLDERS BE L
+00000360: 4941 424c 4520 464f 5220 414e 5920 434c  IABLE FOR ANY CL
+00000370: 4149 4d2c 2044 414d 4147 4553 204f 5220  AIM, DAMAGES OR 
+00000380: 4f54 4845 520a 4c49 4142 494c 4954 592c  OTHER.LIABILITY,
+00000390: 2057 4845 5448 4552 2049 4e20 414e 2041   WHETHER IN AN A
+000003a0: 4354 494f 4e20 4f46 2043 4f4e 5452 4143  CTION OF CONTRAC
+000003b0: 542c 2054 4f52 5420 4f52 204f 5448 4552  T, TORT OR OTHER
+000003c0: 5749 5345 2c20 4152 4953 494e 4720 4652  WISE, ARISING FR
+000003d0: 4f4d 2c0a 4f55 5420 4f46 204f 5220 494e  OM,.OUT OF OR IN
+000003e0: 2043 4f4e 4e45 4354 494f 4e20 5749 5448   CONNECTION WITH
+000003f0: 2054 4845 2053 4f46 5457 4152 4520 4f52   THE SOFTWARE OR
+00000400: 2054 4845 2055 5345 204f 5220 4f54 4845   THE USE OR OTHE
+00000410: 5220 4445 414c 494e 4753 2049 4e20 5448  R DEALINGS IN TH
+00000420: 450a 534f 4654 5741 5245 2e              E.SOFTWARE.
```

### Comparing `ayla-1.0.3/Ayla/cards/assets/curveborder.png` & `ayla-1.0.4/Ayla/cards/assets/curveborder.png`

 * *Files identical despite different names*

### Comparing `ayla-1.0.3/Ayla/cards/assets/curvedoverlay.png` & `ayla-1.0.4/Ayla/cards/assets/curvedoverlay.png`

 * *Files identical despite different names*

### Comparing `ayla-1.0.3/Ayla/cards/assets/fonts/juice.otf` & `ayla-1.0.4/Ayla/cards/assets/fonts/juice.otf`

 * *Files identical despite different names*

### Comparing `ayla-1.0.3/Ayla/cards/assets/fonts/levelfont.otf` & `ayla-1.0.4/Ayla/cards/assets/fonts/levelfont.otf`

 * *Files identical despite different names*

### Comparing `ayla-1.0.3/Ayla/cards/assets/fonts/poppins.ttf` & `ayla-1.0.4/Ayla/cards/assets/fonts/poppins.ttf`

 * *Files identical despite different names*

### Comparing `ayla-1.0.3/Ayla/cards/assets/fonts/rabbit.ttf` & `ayla-1.0.4/Ayla/cards/assets/fonts/rabbit.ttf`

 * *Files identical despite different names*

### Comparing `ayla-1.0.3/Ayla/cards/assets/mask_circle.jpg` & `ayla-1.0.4/Ayla/cards/assets/mask_circle.jpg`

 * *Files identical despite different names*

### Comparing `ayla-1.0.3/Ayla/cards/assets/overlay1.png` & `ayla-1.0.4/Ayla/cards/assets/overlay1.png`

 * *Files identical despite different names*

### Comparing `ayla-1.0.3/Ayla/cards/assets/pic.png` & `ayla-1.0.4/Ayla/cards/assets/pic.png`

 * *Files identical despite different names*

### Comparing `ayla-1.0.3/Ayla/cards/card.py` & `ayla-1.0.4/Ayla/cards/card.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,14 @@
             # things
             path = str(Path(__file__).parent)
             avatar = Image.open(self.pfp)
             bg = Image.open(self.bg)
 
             # background
             W, H = (1000, 333)
-            bg = bg.filter(ImageFilter.BLUR)
             background = bg.resize((1000, 333))
             position = (420, 30)
             avatar = avatar.resize((160, 160))
             mask = Image.open(path + "/assets/mask_circle.jpg").resize((160, 160))
             new = Image.new("RGBA", avatar.size, (0, 0, 0))
             try:
                 new.paste(avatar, mask=avatar.convert("RGBA").split()[3])
@@ -179,15 +178,14 @@
         try:
             # things
             path = str(Path(__file__).parent)
             avatar = Image.open(self.pfp)
             bg = Image.open(self.bg)
 
             # background
-            background = bg.filter(ImageFilter.BLUR)
             background = bg.resize((1000, 333))
             avatar = avatar.resize((210, 210))
             mask = Image.open(path + "/assets/mask_circle.jpg").resize((210, 210))
             new = Image.new("RGBA", avatar.size, (0, 0, 0))
             try:
                 new.paste(avatar, mask=avatar.convert("RGBA").split()[3])
             except:
```

### Comparing `ayla-1.0.3/Ayla/errors/__init__.py` & `ayla-1.0.4/Ayla/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `ayla-1.0.3/Ayla/scrobbles/__init__.py` & `ayla-1.0.4/Ayla/scrobbles/__init__.py`

 * *Files identical despite different names*

### Comparing `ayla-1.0.3/pyproject.toml` & `ayla-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Ayla"
-version = "1.0.3"
+version = "1.0.4"
 readme = "README.md"
 description = "Some functions used in KuuhakuTeam projects"
 repository = "https://github.com/KuuhakuTeam/Ayla"
 authors = ["fnixdev <fenixdev@outlook.com>"]
 license = "MIT"
 keywords = [
     "leveling", "card", "image"
```

