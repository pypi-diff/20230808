# Comparing `tmp/tinyfilter-0.1.6.tar.gz` & `tmp/tinyfilter-0.1.7.tar.gz`

## Comparing `tinyfilter-0.1.6.tar` & `tinyfilter-0.1.7.tar`

### file list

```diff
@@ -1,54 +1,55 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/.DS_Store
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/THANKS.txt
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/.DS_Store
--rw-r--r--   0        0        0   119769 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/Cat03.jpg
--rw-r--r--   0        0        0    57662 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/apple.png
--rw-r--r--   0        0        0  1101570 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/art.png
--rw-r--r--   0        0        0   553076 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/balloon.png
--rw-r--r--   0        0        0   124068 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/chanel.png
--rw-r--r--   0        0        0   345256 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/einstein.png
--rw-r--r--   0        0        0  1087734 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/flowers.png
--rw-r--r--   0        0        0    22318 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/github.png
--rw-r--r--   0        0        0  2853008 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/king.png
--rw-r--r--   0        0        0   994322 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/lisa.png
--rw-r--r--   0        0        0   117684 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/mcdonalds.png
--rw-r--r--   0        0        0     5683 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/nike.png
--rw-r--r--   0        0        0   155708 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/nike2.png
--rw-r--r--   0        0        0   816950 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/paint.png
--rw-r--r--   0        0        0    45319 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/pink.jpeg
--rw-r--r--   0        0        0    64531 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/target.png
--rw-r--r--   0        0        0   674360 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/test.png
--rw-r--r--   0        0        0    45661 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/tiny.png
--rw-r--r--   0        0        0    38785 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/youtube.png
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/new/pyvenv.cfg
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/new/bin/Activate.ps1
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/new/bin/activate
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/new/bin/activate.csh
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/new/bin/activate.fish
--rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/new/bin/f2py
--rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/new/bin/f2py3
--rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/new/bin/f2py3.10
--rwxr-xr-x   0        0        0      305 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/new/bin/helloworld
--rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/new/bin/pip
--rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/new/bin/pip3
--rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/new/bin/pip3.10
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/new/bin/python -> python3
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/new/bin/python3 -> /Library/Frameworks/Python.framework/Versions/3.10/bin/python3
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/new/bin/python3.10 -> python3
--rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/new/bin/tinyimggen
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/old/.DS_Store
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/old/README.md
--rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/old/__main__.py
--rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/old/backup.py
--rw-r--r--   0        0        0   674360 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/old/example_image.png
--rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/old/main.py
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/old/main_debug.py
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/old/output_image.png
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/old/test.py
--rw-r--r--   0        0        0     4522 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/src/tinyfilter/__init__.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/src/tinyfilter/example.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/.gitignore
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/LICENSE
--rw-r--r--   0        0        0     5808 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/README.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     6425 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/.DS_Store
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/THANKS.txt
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/images/.DS_Store
+-rw-r--r--   0        0        0   119769 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/images/Cat03.jpg
+-rw-r--r--   0        0        0    57662 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/images/apple.png
+-rw-r--r--   0        0        0  1101570 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/images/art.png
+-rw-r--r--   0        0        0   553076 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/images/balloon.png
+-rw-r--r--   0        0        0   124068 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/images/chanel.png
+-rw-r--r--   0        0        0   345256 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/images/einstein.png
+-rw-r--r--   0        0        0  1087734 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/images/flowers.png
+-rw-r--r--   0        0        0    22318 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/images/github.png
+-rw-r--r--   0        0        0  2853008 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/images/king.png
+-rw-r--r--   0        0        0   994322 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/images/lisa.png
+-rw-r--r--   0        0        0   123901 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/images/marguerite-729510_1280.jpg
+-rw-r--r--   0        0        0   117684 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/images/mcdonalds.png
+-rw-r--r--   0        0        0     5683 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/images/nike.png
+-rw-r--r--   0        0        0   155708 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/images/nike2.png
+-rw-r--r--   0        0        0   816950 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/images/paint.png
+-rw-r--r--   0        0        0    45319 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/images/pink.jpeg
+-rw-r--r--   0        0        0    64531 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/images/target.png
+-rw-r--r--   0        0        0   674360 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/images/test.png
+-rw-r--r--   0        0        0    45661 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/images/tiny.png
+-rw-r--r--   0        0        0    38785 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/images/youtube.png
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/new/pyvenv.cfg
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/new/bin/Activate.ps1
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/new/bin/activate
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/new/bin/activate.csh
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/new/bin/activate.fish
+-rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/new/bin/f2py
+-rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/new/bin/f2py3
+-rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/new/bin/f2py3.10
+-rwxr-xr-x   0        0        0      305 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/new/bin/helloworld
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/new/bin/pip
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/new/bin/pip3
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/new/bin/pip3.10
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/new/bin/python -> python3
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/new/bin/python3 -> /Library/Frameworks/Python.framework/Versions/3.10/bin/python3
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/new/bin/python3.10 -> python3
+-rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/new/bin/tinyimggen
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/old/.DS_Store
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/old/README.md
+-rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/old/__main__.py
+-rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/old/backup.py
+-rw-r--r--   0        0        0   674360 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/old/example_image.png
+-rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/old/main.py
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/old/main_debug.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/old/output_image.png
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/old/test.py
+-rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/src/tinyfilter/__init__.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/src/tinyfilter/example.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/LICENSE
+-rw-r--r--   0        0        0     5808 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/README.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     6425 2020-02-02 00:00:00.000000 tinyfilter-0.1.7/PKG-INFO
```

### Comparing `tinyfilter-0.1.6/.DS_Store` & `tinyfilter-0.1.7/.DS_Store`

 * *Files 5% similar despite different names*

```diff
@@ -262,48 +262,48 @@
 00001050: 0000 00b9 6270 6c69 7374 3030 d601 0203  ....bplist00....
 00001060: 0405 0607 0807 080b 085d 5368 6f77 5374  .........]ShowSt
 00001070: 6174 7573 4261 725b 5368 6f77 546f 6f6c  atusBar[ShowTool
 00001080: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
 00001090: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
 000010a0: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
 000010b0: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-000010c0: 0908 095f 1019 7b7b 3230 332c 2033 3239  ..._..{{203, 329
+000010c0: 0908 095f 1019 7b7b 3330 362c 2032 3537  ..._..{{306, 257
 000010d0: 7d2c 207b 3132 3337 2c20 3433 367d 7d09  }, {1237, 436}}.
 000010e0: 0815 232f 3b52 5f6b 6c6d 6e6f 8b00 0000  ..#/;R_klmno....
 000010f0: 0000 0001 0100 0000 0000 0000 0d00 0000  ................
 00001100: 0000 0000 0000 0000 0000 0000 8c00 0000  ................
 00001110: 0600 6900 6d00 6100 6700 6500 7369 6376  ..i.m.a.g.e.sicv
 00001120: 7062 6c6f 6200 0001 cd62 706c 6973 7430  pblob....bplist0
 00001130: 30df 1010 0102 0304 0506 0708 090a 0b0c  0...............
-00001140: 0d0e 0f10 1112 1311 1411 1515 1516 1718  ................
-00001150: 191a 1b19 5f10 1362 6163 6b67 726f 756e  ...._..backgroun
+00001140: 0d0e 0f10 1112 1311 1411 1516 1517 1815  ................
+00001150: 191a 191c 5f10 1362 6163 6b67 726f 756e  ...._..backgroun
 00001160: 6443 6f6c 6f72 426c 7565 5b67 7269 6453  dColorBlue[gridS
 00001170: 7061 6369 6e67 5874 6578 7453 697a 655f  pacingXtextSize_
 00001180: 1012 6261 636b 6772 6f75 6e64 436f 6c6f  ..backgroundColo
 00001190: 7252 6564 5e62 6163 6b67 726f 756e 6454  rRed^backgroundT
 000011a0: 7970 655f 1014 6261 636b 6772 6f75 6e64  ype_..background
 000011b0: 436f 6c6f 7247 7265 656e 5b67 7269 644f  ColorGreen[gridO
-000011c0: 6666 7365 7458 5b67 7269 644f 6666 7365  ffsetX[gridOffse
-000011d0: 7459 5f10 0f73 6372 6f6c 6c50 6f73 6974  tY_..scrollPosit
-000011e0: 696f 6e59 5c73 686f 7749 7465 6d49 6e66  ionY\showItemInf
+000011c0: 6666 7365 7458 5f10 0f73 6372 6f6c 6c50  ffsetX_..scrollP
+000011d0: 6f73 6974 696f 6e59 5b67 7269 644f 6666  ositionY[gridOff
+000011e0: 7365 7459 5c73 686f 7749 7465 6d49 6e66  setY\showItemInf
 000011f0: 6f5f 1012 7669 6577 4f70 7469 6f6e 7356  o_..viewOptionsV
 00001200: 6572 7369 6f6e 5f10 0f73 6372 6f6c 6c50  ersion_..scrollP
 00001210: 6f73 6974 696f 6e58 5d6c 6162 656c 4f6e  ositionX]labelOn
 00001220: 426f 7474 6f6d 5961 7272 616e 6765 4279  BottomYarrangeBy
-00001230: 5869 636f 6e53 697a 655f 100f 7368 6f77  XiconSize_..show
-00001240: 4963 6f6e 5072 6576 6965 7723 3ff0 0000  IconPreview#?...
+00001230: 5f10 0f73 686f 7749 636f 6e50 7265 7669  _..showIconPrevi
+00001240: 6577 5869 636f 6e53 697a 6523 3ff0 0000  ewXiconSize#?...
 00001250: 0000 0000 2340 4b00 0000 0000 0023 4028  ....#@K......#@(
 00001260: 0000 0000 0000 1000 2300 0000 0000 0000  ........#.......
-00001270: 0008 1400 0000 0000 0000 0000 0000 0000  ................
-00001280: 0000 0123 406c 0000 0000 0000 0954 6e6f  ...#@l.......Tno
-00001290: 6e65 2340 5000 0000 0000 0009 0008 002b  ne#@P..........+
-000012a0: 0041 004d 0056 006b 007a 0091 009d 00a9  .A.M.V.k.z......
-000012b0: 00bb 00c8 00dd 00ef 00fd 0107 0110 0122  ..............."
-000012c0: 012b 0134 013d 013f 0148 0149 015a 0163  .+.4.=.?.H.I.Z.c
-000012d0: 0164 0169 0172 0000 0000 0000 0201 0000  .d.i.r..........
+00001270: 0023 4054 8000 0000 0000 0814 0000 0000  .#@T............
+00001280: 0000 0000 0000 0000 0000 0001 0954 6e6f  .............Tno
+00001290: 6e65 0923 4050 0000 0000 0000 0008 002b  ne.#@P.........+
+000012a0: 0041 004d 0056 006b 007a 0091 009d 00af  .A.M.V.k.z......
+000012b0: 00bb 00c8 00dd 00ef 00fd 0107 0119 0122  ..............."
+000012c0: 012b 0134 013d 013f 0148 0151 0152 0163  .+.4.=.?.H.Q.R.c
+000012d0: 0164 0169 016a 0000 0000 0000 0201 0000  .d.i.j..........
 000012e0: 0000 0000 001d 0000 0000 0000 0000 0000  ................
 000012f0: 0000 0000 0173 0000 0006 0069 006d 0061  .....s.....i.m.a
 00001300: 0067 0065 0073 6c67 3153 636f 6d70 0000  .g.e.slg1Scomp..
 00001310: 0000 0000 0000 0000 0006 0069 006d 0061  ...........i.m.a
 00001320: 0067 0065 0073 6d6f 4444 626c 6f62 0000  .g.e.smoDDblob..
 00001330: 0008 4cac c35c 9b3f c541 0000 0006 0069  ..L..\.?.A.....i
 00001340: 006d 0061 0067 0065 0073 6d6f 6444 626c  .m.a.g.e.smodDbl
```

### Comparing `tinyfilter-0.1.6/THANKS.txt` & `tinyfilter-0.1.7/THANKS.txt`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.6/images/.DS_Store` & `tinyfilter-0.1.7/images/.DS_Store`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 0000 0001 4275 6431 0000 1800 0000 0800  ....Bud1........
 00000010: 0000 1800 0000 100b 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0015  ................
+00000040: 0000 0000 0000 0002 0000 0000 0000 0016  ................
 00000050: 0000 0001 0000 1000 0065 002e 0070 006e  .........e...p.n
 00000060: 0067 496c 0000 0000 0000 0000 0000 0000  .gIl............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -250,15 +250,15 @@
 00000f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001000: 0000 0000 0000 0000 0000 0015 0000 0009  ................
+00001000: 0000 0000 0000 0000 0000 0016 0000 0009  ................
 00001010: 0061 0070 0070 006c 0065 002e 0070 006e  .a.p.p.l.e...p.n
 00001020: 0067 496c 6f63 626c 6f62 0000 0010 0000  .gIlocblob......
 00001030: 01f9 0000 0059 ffff ffff ffff 0000 0000  .....Y..........
 00001040: 0007 0061 0072 0074 002e 0070 006e 0067  ...a.r.t...p.n.g
 00001050: 496c 6f63 626c 6f62 0000 0010 0000 0041  Ilocblob.......A
 00001060: 0000 0059 ffff ffff ffff 0000 0000 000b  ...Y............
 00001070: 0062 0061 006c 006c 006f 006f 006e 002e  .b.a.l.l.o.o.n..
@@ -282,66 +282,66 @@
 00001190: 6f63 626c 6f62 0000 0010 0000 00af 0000  ocblob..........
 000011a0: 0059 ffff ffff ffff 0000 0000 0008 006b  .Y.............k
 000011b0: 0069 006e 0067 002e 0070 006e 0067 496c  .i.n.g...p.n.gIl
 000011c0: 6f63 626c 6f62 0000 0010 0000 0343 0000  ocblob.......C..
 000011d0: 0059 ffff ffff ffff 0000 0000 0008 006c  .Y.............l
 000011e0: 0069 0073 0061 002e 0070 006e 0067 496c  .i.s.a...p.n.gIl
 000011f0: 6f63 626c 6f62 0000 0010 0000 00e4 0000  ocblob..........
-00001200: 0110 ffff ffff ffff 0000 0000 000d 006d  ...............m
-00001210: 0063 0064 006f 006e 0061 006c 0064 0073  .c.d.o.n.a.l.d.s
-00001220: 002e 0070 006e 0067 496c 6f63 626c 6f62  ...p.n.gIlocblob
-00001230: 0000 0010 0000 03b1 0000 0059 ffff ffff  ...........Y....
-00001240: ffff 0000 0000 0008 006e 0069 006b 0065  .........n.i.k.e
-00001250: 002e 0070 006e 0067 496c 6f63 626c 6f62  ...p.n.gIlocblob
-00001260: 0000 0010 0000 0072 0000 011a ffff ffff  .......r........
-00001270: ffff 0000 0000 0008 006e 0069 006b 0065  .........n.i.k.e
-00001280: 002e 0070 006e 0067 7074 624c 7573 7472  ...p.n.gptbLustr
-00001290: 0000 0061 0053 0079 0073 0074 0065 006d  ...a.S.y.s.t.e.m
-000012a0: 002f 0056 006f 006c 0075 006d 0065 0073  ./.V.o.l.u.m.e.s
-000012b0: 002f 0044 0061 0074 0061 002f 0055 0073  ./.D.a.t.a./.U.s
-000012c0: 0065 0072 0073 002f 007a 0065 0070 0068  .e.r.s./.z.e.p.h
-000012d0: 0061 006e 0069 0061 0068 0072 006f 0065  .a.n.i.a.h.r.o.e
-000012e0: 002f 0044 0065 0073 006b 0074 006f 0070  ./.D.e.s.k.t.o.p
-000012f0: 002f 0064 0065 0073 006b 0074 006f 0070  ./.d.e.s.k.t.o.p
-00001300: 005f 0069 006d 0070 006f 0072 0074 0061  ._.i.m.p.o.r.t.a
-00001310: 006e 0074 002f 0073 0075 006d 006d 0065  .n.t./.s.u.m.m.e
-00001320: 0072 002f 0074 0069 006e 0079 002d 0041  .r./.t.i.n.y.-.A
-00001330: 0053 0043 0049 0049 002d 0061 0072 0074  .S.C.I.I.-.a.r.t
-00001340: 002d 0067 0065 006e 0065 0072 0061 0074  .-.g.e.n.e.r.a.t
-00001350: 006f 0072 002f 0000 0008 006e 0069 006b  .o.r./.....n.i.k
-00001360: 0065 002e 0070 006e 0067 7074 624e 7573  .e...p.n.gptbNus
-00001370: 7472 0000 0008 006e 0069 006b 0065 002e  tr.....n.i.k.e..
-00001380: 0070 006e 0067 0000 0009 006e 0069 006b  .p.n.g.....n.i.k
-00001390: 0065 0032 002e 0070 006e 0067 496c 6f63  .e.2...p.n.gIloc
-000013a0: 626c 6f62 0000 0010 0000 0052 0000 0175  blob.......R...u
-000013b0: ffff ffff ffff 0000 0000 0009 0070 0061  .............p.a
-000013c0: 0069 006e 0074 002e 0070 006e 0067 496c  .i.n.t...p.n.gIl
-000013d0: 6f63 626c 6f62 0000 0010 0000 0309 0000  ocblob..........
-000013e0: 00fc ffff ffff ffff 0000 0000 0009 0070  ...............p
-000013f0: 0069 006e 006b 002e 006a 0070 0065 0067  .i.n.k...j.p.e.g
-00001400: 496c 6f63 626c 6f62 0000 0010 0000 0041  Ilocblob.......A
-00001410: 0000 00c9 ffff ffff ffff 0000 0000 000a  ................
-00001420: 0074 0061 0072 0067 0065 0074 002e 0070  .t.a.r.g.e.t...p
-00001430: 006e 0067 496c 6f63 626c 6f62 0000 0010  .n.gIlocblob....
-00001440: 0000 00af 0000 00c9 ffff ffff ffff 0000  ................
-00001450: 0000 0008 0074 0065 0073 0074 002e 0070  .....t.e.s.t...p
-00001460: 006e 0067 496c 6f63 626c 6f62 0000 0010  .n.gIlocblob....
-00001470: 0000 011d 0000 0059 ffff ffff ffff 0000  .......Y........
-00001480: 0000 0008 0074 0069 006e 0079 002e 0070  .....t.i.n.y...p
-00001490: 006e 0067 496c 6f63 626c 6f62 0000 0010  .n.gIlocblob....
-000014a0: 0000 018b 0000 0059 ffff ffff ffff 0000  .......Y........
-000014b0: 0000 000b 0079 006f 0075 0074 0075 0062  .....y.o.u.t.u.b
-000014c0: 0065 002e 0070 006e 0067 496c 6f63 626c  .e...p.n.gIlocbl
-000014d0: 6f62 0000 0010 0000 011d 0000 00c9 ffff  ob..............
-000014e0: ffff ffff 0000 0000 0000 0001 4000 0000  ............@...
-000014f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001500: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001510: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001520: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001530: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001200: 0110 ffff ffff ffff 0000 0000 001a 006d  ...............m
+00001210: 0061 0072 0067 0075 0065 0072 0069 0074  .a.r.g.u.e.r.i.t
+00001220: 0065 002d 0037 0032 0039 0035 0031 0030  .e.-.7.2.9.5.1.0
+00001230: 005f 0031 0032 0038 0030 002e 006a 0070  ._.1.2.8.0...j.p
+00001240: 0067 496c 6f63 626c 6f62 0000 0010 0000  .gIlocblob......
+00001250: 02d5 0000 017e ffff ffff ffff 0000 0000  .....~..........
+00001260: 000d 006d 0063 0064 006f 006e 0061 006c  ...m.c.d.o.n.a.l
+00001270: 0064 0073 002e 0070 006e 0067 496c 6f63  .d.s...p.n.gIloc
+00001280: 626c 6f62 0000 0010 0000 03b1 0000 0059  blob...........Y
+00001290: ffff ffff ffff 0000 0000 0008 006e 0069  .............n.i
+000012a0: 006b 0065 002e 0070 006e 0067 496c 6f63  .k.e...p.n.gIloc
+000012b0: 626c 6f62 0000 0010 0000 0072 0000 011a  blob.......r....
+000012c0: ffff ffff ffff 0000 0000 0008 006e 0069  .............n.i
+000012d0: 006b 0065 002e 0070 006e 0067 7074 624c  .k.e...p.n.gptbL
+000012e0: 7573 7472 0000 0061 0053 0079 0073 0074  ustr...a.S.y.s.t
+000012f0: 0065 006d 002f 0056 006f 006c 0075 006d  .e.m./.V.o.l.u.m
+00001300: 0065 0073 002f 0044 0061 0074 0061 002f  .e.s./.D.a.t.a./
+00001310: 0055 0073 0065 0072 0073 002f 007a 0065  .U.s.e.r.s./.z.e
+00001320: 0070 0068 0061 006e 0069 0061 0068 0072  .p.h.a.n.i.a.h.r
+00001330: 006f 0065 002f 0044 0065 0073 006b 0074  .o.e./.D.e.s.k.t
+00001340: 006f 0070 002f 0064 0065 0073 006b 0074  .o.p./.d.e.s.k.t
+00001350: 006f 0070 005f 0069 006d 0070 006f 0072  .o.p._.i.m.p.o.r
+00001360: 0074 0061 006e 0074 002f 0073 0075 006d  .t.a.n.t./.s.u.m
+00001370: 006d 0065 0072 002f 0074 0069 006e 0079  .m.e.r./.t.i.n.y
+00001380: 002d 0041 0053 0043 0049 0049 002d 0061  .-.A.S.C.I.I.-.a
+00001390: 0072 0074 002d 0067 0065 006e 0065 0072  .r.t.-.g.e.n.e.r
+000013a0: 0061 0074 006f 0072 002f 0000 0008 006e  .a.t.o.r./.....n
+000013b0: 0069 006b 0065 002e 0070 006e 0067 7074  .i.k.e...p.n.gpt
+000013c0: 624e 7573 7472 0000 0008 006e 0069 006b  bNustr.....n.i.k
+000013d0: 0065 002e 0070 006e 0067 0000 0009 006e  .e...p.n.g.....n
+000013e0: 0069 006b 0065 0032 002e 0070 006e 0067  .i.k.e.2...p.n.g
+000013f0: 496c 6f63 626c 6f62 0000 0010 0000 0052  Ilocblob.......R
+00001400: 0000 0175 ffff ffff ffff 0000 0000 0009  ...u............
+00001410: 0070 0061 0069 006e 0074 002e 0070 006e  .p.a.i.n.t...p.n
+00001420: 0067 496c 6f63 626c 6f62 0000 0010 0000  .gIlocblob......
+00001430: 0309 0000 00fc ffff ffff ffff 0000 0000  ................
+00001440: 0009 0070 0069 006e 006b 002e 006a 0070  ...p.i.n.k...j.p
+00001450: 0065 0067 496c 6f63 626c 6f62 0000 0010  .e.gIlocblob....
+00001460: 0000 0041 0000 00c9 ffff ffff ffff 0000  ...A............
+00001470: 0000 000a 0074 0061 0072 0067 0065 0074  .....t.a.r.g.e.t
+00001480: 002e 0070 006e 0067 496c 6f63 626c 6f62  ...p.n.gIlocblob
+00001490: 0000 0010 0000 00af 0000 00c9 ffff ffff  ................
+000014a0: ffff 0000 0000 0008 0074 0065 0073 0074  .........t.e.s.t
+000014b0: 002e 0070 006e 0067 496c 6f63 626c 6f62  ...p.n.gIlocblob
+000014c0: 0000 0010 0000 011d 0000 0059 ffff ffff  ...........Y....
+000014d0: ffff 0000 0000 0008 0074 0069 006e 0079  .........t.i.n.y
+000014e0: 002e 0070 006e 0067 496c 6f63 626c 6f62  ...p.n.gIlocblob
+000014f0: 0000 0010 0000 018b 0000 0059 ffff ffff  ...........Y....
+00001500: ffff 0000 0000 000b 0079 006f 0075 0074  .........y.o.u.t
+00001510: 0075 0062 0065 002e 0070 006e 0067 496c  .u.b.e...p.n.gIl
+00001520: 6f63 626c 6f62 0000 0010 0000 011d 0000  ocblob..........
+00001530: 00c9 ffff ffff ffff 0000 0000 0000 0000  ................
 00001540: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001550: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001560: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -457,19 +457,19 @@
 00001c80: 0000 0000 0100 0100 0000 0000 0100 0200  ................
 00001c90: 0000 0000 0100 0400 0000 0000 0100 0800  ................
 00001ca0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
 00001cb0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
 00001cc0: 0000 0000 0101 0000 0000 0000 0102 0000  ................
 00001cd0: 0000 0000 0104 0000 0000 0000 0108 0000  ................
 00001ce0: 0000 0000 0110 0000 0000 0000 0120 0000  ............. ..
-00001cf0: 0000 0000 0140 0000 0000 0000 0000 0000  .....@..........
-00001d00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001cf0: 0000 0000 0140 0000 0000 0000 00ff ffff  .....@..........
+00001d00: ffff 0000 0000 000b 0079 006f 0075 0074  .........y.o.u.t
+00001d10: 0075 0062 0065 002e 0070 006e 0067 496c  .u.b.e...p.n.gIl
+00001d20: 6f63 626c 6f62 0000 0010 0000 011d 0000  ocblob..........
+00001d30: 00c9 ffff ffff ffff 0000 0000 0000 0000  ................
 00001d40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `tinyfilter-0.1.6/images/Cat03.jpg` & `tinyfilter-0.1.7/images/Cat03.jpg`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.6/images/apple.png` & `tinyfilter-0.1.7/images/apple.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.6/images/art.png` & `tinyfilter-0.1.7/images/art.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.6/images/balloon.png` & `tinyfilter-0.1.7/images/balloon.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.6/images/chanel.png` & `tinyfilter-0.1.7/images/chanel.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.6/images/einstein.png` & `tinyfilter-0.1.7/images/einstein.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.6/images/flowers.png` & `tinyfilter-0.1.7/images/flowers.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.6/images/github.png` & `tinyfilter-0.1.7/images/github.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.6/images/king.png` & `tinyfilter-0.1.7/images/king.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.6/images/lisa.png` & `tinyfilter-0.1.7/images/lisa.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.6/images/mcdonalds.png` & `tinyfilter-0.1.7/images/mcdonalds.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.6/images/nike.png` & `tinyfilter-0.1.7/images/nike.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.6/images/nike2.png` & `tinyfilter-0.1.7/images/nike2.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.6/images/paint.png` & `tinyfilter-0.1.7/images/paint.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.6/images/pink.jpeg` & `tinyfilter-0.1.7/images/pink.jpeg`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.6/images/target.png` & `tinyfilter-0.1.7/images/target.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.6/images/test.png` & `tinyfilter-0.1.7/images/test.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.6/images/tiny.png` & `tinyfilter-0.1.7/images/tiny.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.6/images/youtube.png` & `tinyfilter-0.1.7/images/youtube.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.6/new/bin/Activate.ps1` & `tinyfilter-0.1.7/new/bin/Activate.ps1`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.6/new/bin/activate` & `tinyfilter-0.1.7/new/bin/activate`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.6/new/bin/activate.csh` & `tinyfilter-0.1.7/new/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.6/new/bin/activate.fish` & `tinyfilter-0.1.7/new/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.6/old/.DS_Store` & `tinyfilter-0.1.7/old/.DS_Store`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.6/old/__main__.py` & `tinyfilter-0.1.7/old/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.6/old/backup.py` & `tinyfilter-0.1.7/old/backup.py`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.6/old/example_image.png` & `tinyfilter-0.1.7/old/example_image.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.6/old/main.py` & `tinyfilter-0.1.7/old/main.py`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.6/old/main_debug.py` & `tinyfilter-0.1.7/old/main_debug.py`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.6/old/output_image.png` & `tinyfilter-0.1.7/old/output_image.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.6/src/tinyfilter/__init__.py` & `tinyfilter-0.1.7/src/tinyfilter/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from PIL import Image  # type: ignore
 import numpy as np
 from numpy.typing import NDArray
 import shutil
 import argparse
 
 LOAD_IMG_WIDTH = shutil.get_terminal_size().columns + 2
-LOAD_IMG_HEIGHT = int(LOAD_IMG_WIDTH * (5 / 8))
+load_img_height = 0
 
 # Filters applied to the image to detect features
 BACKSLASH_FILTER = np.array([[3, -1, -1], [-1, 3, -1], [-1, -1, 3]], dtype="int32")
 FORWARDSLASH_FILTER = np.array([[-1, -1, 3], [-1, 3, -1], [3, -1, -1]], dtype="int32")
 VERTICAL_BAR_FILTER = np.array([[-1, 3, -1], [-1, 3, -1], [-1, 3, -1]], dtype="int32")
 HYPEN_FILTER = np.array([[-1, -1, -1], [3, 4, 3], [-1, -1, -1]], dtype="int32")
 UNDERSCORE_FILTER = np.array([[-1, -1, -1], [-1, -1, -1], [3, 4, 3]], dtype="int32")
@@ -71,15 +71,15 @@
 
 def print_grayscale_img(img: NDArray[np.uint8]) -> None:
     """Prints a grayscale image as ASCII characters to console.
 
     Args:
         img: a numpy array of grayscale pixels (shape = (x, x, 3))
     """
-    for i in range(1, LOAD_IMG_HEIGHT - 1):
+    for i in range(1, load_img_height - 1):
         for j in range(1, LOAD_IMG_WIDTH - 1):
             # Loads a 9 pixel region of the image
             img_region = img[i - 1 : i + 2, j - 1 : j + 2]
 
             # Load the pixels as a 3 * 3 array (one int representing the
             # grayscale value of each pixel in the region)
             img_region = img_region[:, :, 0:1]
@@ -89,16 +89,16 @@
 
 
 def tiny_print(img_filename=None) -> None:
     """Loads an image and prints it as ASCII characters to the console"""
     if img_filename == None:
         parser = argparse.ArgumentParser(
             prog="tinyfilter",
-            description="What the program does",
-            epilog="Text at the bottom of help",
+            description="""tinyfilter converts images into ASCII art using filters.""",
+            epilog="For information about how to use tinfilter visit: https://github.com/zroe1/tinyfilter",
         )
         parser.add_argument("filename")
 
         args = parser.parse_args()
         img_raw = Image.open(args.filename)
     else:
         img_raw = Image.open(img_filename)
@@ -110,15 +110,22 @@
     Image mode was {}. Currently tinyfilter only supports modes of "RGB" and 
     "RGBA." To learn more about image modes visit the Pillow (a dependency 
     of tinyfilter) documentation:
 
     https://pillow.readthedocs.io/en/stable/handbook/concepts.html#concept-modes
         '''.format(img_raw.mode))
 
-    img_raw = img_raw.resize((LOAD_IMG_WIDTH, LOAD_IMG_HEIGHT))
+    # Loads image as NumPy array to derive the height
+    original_img = np.array(img_raw)
+
+    # Applys formula to calculate how many caracters high the output should be
+    global load_img_height
+    load_img_height = int(original_img.shape[0] * (LOAD_IMG_WIDTH / original_img.shape[1]) * (4/8))
+
+    img_raw = img_raw.resize((LOAD_IMG_WIDTH, load_img_height))
     img: NDArray[np.uint8] = np.array(img_raw)
 
     # Removes alpha channel from an image if present
     if img_raw.mode == "RGBA":
         img = img[:, :, 0:3]
 
     np.apply_along_axis(change_pixel_to_gray_scale, axis=2, arr=img)
```

### Comparing `tinyfilter-0.1.6/.gitignore` & `tinyfilter-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.6/LICENSE` & `tinyfilter-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.6/README.md` & `tinyfilter-0.1.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # tinyfilter
 <img width="1423" alt="Screenshot 2023-08-05 at 4 52 21 PM" src="https://github.com/zroe1/tinyfilter/assets/114773939/488e61be-3431-444c-9fcc-8ae8944c8b59">  
 </br></br>  
 <p align="center">
-<a href="https://pypi.org/project/tinyfilter/0.1.6/"><img alt="link to PyPi" src="https://img.shields.io/badge/pypi-v0.1.6-brightgreen"></a>
+<a href="https://pypi.org/project/tinyfilter/0.1.7/"><img alt="link to PyPi" src="https://img.shields.io/badge/pypi-v0.1.7-brightgreen"></a>
 <a href="https://github.com/zroe1/tinyfilter/blob/main/LICENSE"><img alt="link to license" src="https://img.shields.io/badge/License-MIT-purple"></a>
 <a href="https://github.com/psf/black/tree/main"><img alt="link to license" src="https://img.shields.io/badge/code%20style-black-black"></a>
 </p> 
 
 tinyfilter [^1] is the computer vision equivalent to Andrej Karpathy's <a href="https://github.com/karpathy/micrograd">micrograd</a>. It convert images into ASCII art using the principles of CNNs (convolutional neural networks).  
 </br>
 Unlike other tools of its type, which map pixel darkness to an ASCII character, tinyfilter uses filters and convolution to detect features in an image and prints ASCII characters that correspond to them. This leads to much better results compared to other libraries, especially for smaller images.
```

### Comparing `tinyfilter-0.1.6/pyproject.toml` & `tinyfilter-0.1.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tinyfilter"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="Zephaniah Roe", email="zroe@uchicago.edu" },
 ]
 description = "tinyfilter is the computer vision equivalent to micrograd. It convert images into ASCII art using the principles of CNNs (convolutional neural networks)."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `tinyfilter-0.1.6/PKG-INFO` & `tinyfilter-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyfilter
-Version: 0.1.6
+Version: 0.1.7
 Summary: tinyfilter is the computer vision equivalent to micrograd. It convert images into ASCII art using the principles of CNNs (convolutional neural networks).
 Project-URL: Homepage, https://github.com/zroe1/tinyfilter/tree/main
 Author-email: Zephaniah Roe <zroe@uchicago.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Requires-Dist: pillow
 Description-Content-Type: text/markdown
 
 # tinyfilter
 <img width="1423" alt="Screenshot 2023-08-05 at 4 52 21 PM" src="https://github.com/zroe1/tinyfilter/assets/114773939/488e61be-3431-444c-9fcc-8ae8944c8b59">  
 </br></br>  
 <p align="center">
-<a href="https://pypi.org/project/tinyfilter/0.1.6/"><img alt="link to PyPi" src="https://img.shields.io/badge/pypi-v0.1.6-brightgreen"></a>
+<a href="https://pypi.org/project/tinyfilter/0.1.7/"><img alt="link to PyPi" src="https://img.shields.io/badge/pypi-v0.1.7-brightgreen"></a>
 <a href="https://github.com/zroe1/tinyfilter/blob/main/LICENSE"><img alt="link to license" src="https://img.shields.io/badge/License-MIT-purple"></a>
 <a href="https://github.com/psf/black/tree/main"><img alt="link to license" src="https://img.shields.io/badge/code%20style-black-black"></a>
 </p> 
 
 tinyfilter [^1] is the computer vision equivalent to Andrej Karpathy's <a href="https://github.com/karpathy/micrograd">micrograd</a>. It convert images into ASCII art using the principles of CNNs (convolutional neural networks).  
 </br>
 Unlike other tools of its type, which map pixel darkness to an ASCII character, tinyfilter uses filters and convolution to detect features in an image and prints ASCII characters that correspond to them. This leads to much better results compared to other libraries, especially for smaller images.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tinyfilter Version: 0.1.6 Summary: tinyfilter is
+Metadata-Version: 2.1 Name: tinyfilter Version: 0.1.7 Summary: tinyfilter is
 the computer vision equivalent to micrograd. It convert images into ASCII art
 using the principles of CNNs (convolutional neural networks). Project-URL:
 Homepage, https://github.com/zroe1/tinyfilter/tree/main Author-email: Zephaniah
 Roe
 uchicago.edu> License-File: LICENSE Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.7 Requires-Dist: numpy~=1.25.0
```

