# Comparing `tmp/tinyfilter-0.1.5.tar.gz` & `tmp/tinyfilter-0.1.6.tar.gz`

## Comparing `tinyfilter-0.1.5.tar` & `tinyfilter-0.1.6.tar`

### file list

```diff
@@ -1,53 +1,54 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/.DS_Store
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/THANKS.txt
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/images/.DS_Store
--rw-r--r--   0        0        0    57662 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/images/apple.png
--rw-r--r--   0        0        0  1101570 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/images/art.png
--rw-r--r--   0        0        0   553076 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/images/balloon.png
--rw-r--r--   0        0        0   124068 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/images/chanel.png
--rw-r--r--   0        0        0   345256 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/images/einstein.png
--rw-r--r--   0        0        0  1087734 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/images/flowers.png
--rw-r--r--   0        0        0    22318 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/images/github.png
--rw-r--r--   0        0        0  2853008 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/images/king.png
--rw-r--r--   0        0        0   994322 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/images/lisa.png
--rw-r--r--   0        0        0   117684 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/images/mcdonalds.png
--rw-r--r--   0        0        0   816950 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/images/paint.png
--rw-r--r--   0        0        0    45319 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/images/pink.jpeg
--rw-r--r--   0        0        0    64531 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/images/target.png
--rw-r--r--   0        0        0   674360 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/images/test.png
--rw-r--r--   0        0        0    45661 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/images/tiny.png
--rw-r--r--   0        0        0    38785 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/images/youtube.png
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/new/pyvenv.cfg
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/new/bin/Activate.ps1
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/new/bin/activate
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/new/bin/activate.csh
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/new/bin/activate.fish
--rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/new/bin/f2py
--rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/new/bin/f2py3
--rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/new/bin/f2py3.10
--rwxr-xr-x   0        0        0      305 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/new/bin/helloworld
--rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/new/bin/pip
--rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/new/bin/pip3
--rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/new/bin/pip3.10
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/new/bin/python -> python3
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/new/bin/python3 -> /Library/Frameworks/Python.framework/Versions/3.10/bin/python3
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/new/bin/python3.10 -> python3
--rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/new/bin/tinyimggen
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/old/.DS_Store
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/old/README.md
--rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/old/__main__.py
--rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/old/backup.py
--rw-r--r--   0        0        0   674360 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/old/example_image.png
--rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/old/main.py
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/old/main_debug.py
--rw-r--r--   0        0        0     5683 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/old/nike.png
--rw-r--r--   0        0        0   155708 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/old/nike2.png
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/old/output_image.png
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/old/test.py
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/src/tinyfilter/__init__.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/src/tinyfilter/example.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/.gitignore
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/LICENSE
--rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/README.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 tinyfilter-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/.DS_Store
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/THANKS.txt
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/.DS_Store
+-rw-r--r--   0        0        0   119769 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/Cat03.jpg
+-rw-r--r--   0        0        0    57662 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/apple.png
+-rw-r--r--   0        0        0  1101570 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/art.png
+-rw-r--r--   0        0        0   553076 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/balloon.png
+-rw-r--r--   0        0        0   124068 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/chanel.png
+-rw-r--r--   0        0        0   345256 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/einstein.png
+-rw-r--r--   0        0        0  1087734 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/flowers.png
+-rw-r--r--   0        0        0    22318 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/github.png
+-rw-r--r--   0        0        0  2853008 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/king.png
+-rw-r--r--   0        0        0   994322 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/lisa.png
+-rw-r--r--   0        0        0   117684 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/mcdonalds.png
+-rw-r--r--   0        0        0     5683 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/nike.png
+-rw-r--r--   0        0        0   155708 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/nike2.png
+-rw-r--r--   0        0        0   816950 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/paint.png
+-rw-r--r--   0        0        0    45319 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/pink.jpeg
+-rw-r--r--   0        0        0    64531 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/target.png
+-rw-r--r--   0        0        0   674360 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/test.png
+-rw-r--r--   0        0        0    45661 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/tiny.png
+-rw-r--r--   0        0        0    38785 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/images/youtube.png
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/new/pyvenv.cfg
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/new/bin/Activate.ps1
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/new/bin/activate
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/new/bin/activate.csh
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/new/bin/activate.fish
+-rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/new/bin/f2py
+-rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/new/bin/f2py3
+-rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/new/bin/f2py3.10
+-rwxr-xr-x   0        0        0      305 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/new/bin/helloworld
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/new/bin/pip
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/new/bin/pip3
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/new/bin/pip3.10
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/new/bin/python -> python3
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/new/bin/python3 -> /Library/Frameworks/Python.framework/Versions/3.10/bin/python3
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/new/bin/python3.10 -> python3
+-rwxr-xr-x   0        0        0      291 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/new/bin/tinyimggen
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/old/.DS_Store
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/old/README.md
+-rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/old/__main__.py
+-rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/old/backup.py
+-rw-r--r--   0        0        0   674360 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/old/example_image.png
+-rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/old/main.py
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/old/main_debug.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/old/output_image.png
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/old/test.py
+-rw-r--r--   0        0        0     4522 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/src/tinyfilter/__init__.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/src/tinyfilter/example.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/LICENSE
+-rw-r--r--   0        0        0     5808 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/README.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     6425 2020-02-02 00:00:00.000000 tinyfilter-0.1.6/PKG-INFO
```

### Comparing `tinyfilter-0.1.5/.DS_Store` & `tinyfilter-0.1.6/.DS_Store`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 0000 0001 4275 6431 0000 1800 0000 0800  ....Bud1........
 00000010: 0000 1800 0000 100b 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0014  ................
+00000040: 0000 0000 0000 0002 0000 0000 0000 0015  ................
 00000050: 0000 0001 0000 1000 0065 0073 496c 6f63  .........e.sIloc
 00000060: 626c 6f62 0000 0000 0000 0000 0000 0000  blob............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -250,103 +250,103 @@
 00000f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001000: 0000 0000 0000 0000 0000 0014 0000 0006  ................
+00001000: 0000 0000 0000 0000 0000 0015 0000 0006  ................
 00001010: 0069 006d 0061 0067 0065 0073 496c 6f63  .i.m.a.g.e.sIloc
 00001020: 626c 6f62 0000 0010 0000 0318 0000 00e4  blob............
 00001030: ffff ffff ffff 0000 0000 0006 0069 006d  .............i.m
 00001040: 0061 0067 0065 0073 6277 7370 626c 6f62  .a.g.e.sbwspblob
-00001050: 0000 00b8 6270 6c69 7374 3030 d601 0203  ....bplist00....
+00001050: 0000 00b9 6270 6c69 7374 3030 d601 0203  ....bplist00....
 00001060: 0405 0607 0807 080b 085d 5368 6f77 5374  .........]ShowSt
 00001070: 6174 7573 4261 725b 5368 6f77 546f 6f6c  atusBar[ShowTool
 00001080: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
 00001090: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
 000010a0: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
 000010b0: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-000010c0: 0908 095f 1018 7b7b 3533 322c 2031 3930  ..._..{{532, 190
-000010d0: 7d2c 207b 3932 302c 2034 3336 7d7d 0908  }, {920, 436}}..
-000010e0: 1523 2f3b 525f 6b6c 6d6e 6f8a 0000 0000  .#/;R_klmno.....
-000010f0: 0000 0101 0000 0000 0000 000d 0000 0000  ................
-00001100: 0000 0000 0000 0000 0000 008b 0000 0006  ................
-00001110: 0069 006d 0061 0067 0065 0073 6963 7670  .i.m.a.g.e.sicvp
-00001120: 626c 6f62 0000 01cd 6270 6c69 7374 3030  blob....bplist00
-00001130: df10 1001 0203 0405 0607 0809 0a0b 0c0d  ................
-00001140: 0e0f 1011 1213 1114 1115 1515 1617 1819  ................
-00001150: 1a1b 195f 1013 6261 636b 6772 6f75 6e64  ..._..background
-00001160: 436f 6c6f 7242 6c75 655b 6772 6964 5370  ColorBlue[gridSp
-00001170: 6163 696e 6758 7465 7874 5369 7a65 5f10  acingXtextSize_.
-00001180: 1262 6163 6b67 726f 756e 6443 6f6c 6f72  .backgroundColor
-00001190: 5265 645e 6261 636b 6772 6f75 6e64 5479  Red^backgroundTy
-000011a0: 7065 5f10 1462 6163 6b67 726f 756e 6443  pe_..backgroundC
-000011b0: 6f6c 6f72 4772 6565 6e5b 6772 6964 4f66  olorGreen[gridOf
-000011c0: 6673 6574 585b 6772 6964 4f66 6673 6574  fsetX[gridOffset
-000011d0: 595f 100f 7363 726f 6c6c 506f 7369 7469  Y_..scrollPositi
-000011e0: 6f6e 595c 7368 6f77 4974 656d 496e 666f  onY\showItemInfo
-000011f0: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
-00001200: 7273 696f 6e5f 100f 7363 726f 6c6c 506f  rsion_..scrollPo
-00001210: 7369 7469 6f6e 585d 6c61 6265 6c4f 6e42  sitionX]labelOnB
-00001220: 6f74 746f 6d59 6172 7261 6e67 6542 7958  ottomYarrangeByX
-00001230: 6963 6f6e 5369 7a65 5f10 0f73 686f 7749  iconSize_..showI
-00001240: 636f 6e50 7265 7669 6577 233f f000 0000  conPreview#?....
-00001250: 0000 0023 404b 0000 0000 0000 2340 2800  ...#@K......#@(.
-00001260: 0000 0000 0010 0023 0000 0000 0000 0000  .......#........
-00001270: 0814 0000 0000 0000 0000 0000 0000 0000  ................
-00001280: 0001 2340 6c00 0000 0000 0009 546e 6f6e  ..#@l.......Tnon
-00001290: 6523 4050 0000 0000 0000 0900 0800 2b00  e#@P..........+.
-000012a0: 4100 4d00 5600 6b00 7a00 9100 9d00 a900  A.M.V.k.z.......
-000012b0: bb00 c800 dd00 ef00 fd01 0701 1001 2201  ..............".
-000012c0: 2b01 3401 3d01 3f01 4801 4901 5a01 6301  +.4.=.?.H.I.Z.c.
-000012d0: 6401 6901 7200 0000 0000 0002 0100 0000  d.i.r...........
-000012e0: 0000 0000 1d00 0000 0000 0000 0000 0000  ................
-000012f0: 0000 0001 7300 0000 0600 6900 6d00 6100  ....s.....i.m.a.
-00001300: 6700 6500 736c 6731 5363 6f6d 7000 0000  g.e.slg1Scomp...
-00001310: 0000 0000 0000 0000 0600 6900 6d00 6100  ..........i.m.a.
-00001320: 6700 6500 736d 6f44 4462 6c6f 6200 0000  g.e.smoDDblob...
-00001330: 084c acc3 5c9b 3fc5 4100 0000 0600 6900  .L..\.?.A.....i.
-00001340: 6d00 6100 6700 6500 736d 6f64 4462 6c6f  m.a.g.e.smodDblo
-00001350: 6200 0000 084c acc3 5c9b 3fc5 4100 0000  b....L..\.?.A...
-00001360: 0600 6900 6d00 6100 6700 6500 7370 6831  ..i.m.a.g.e.sph1
-00001370: 5363 6f6d 7000 0000 0000 0000 0000 0000  Scomp...........
-00001380: 0600 6900 6d00 6100 6700 6500 7376 5372  ..i.m.a.g.e.svSr
-00001390: 6e6c 6f6e 6700 0000 0100 0000 0700 4c00  nlong.........L.
-000013a0: 4900 4300 4500 4e00 5300 4549 6c6f 6362  I.C.E.N.S.EIlocb
-000013b0: 6c6f 6200 0000 1000 0001 8200 0000 87ff  lob.............
-000013c0: ffff ffff ff00 0000 0000 0300 6e00 6500  ............n.e.
-000013d0: 7749 6c6f 6362 6c6f 6200 0000 1000 0001  wIlocblob.......
-000013e0: 8200 0000 f7ff ffff ffff ff00 0000 0000  ................
-000013f0: 0300 6f00 6c00 6449 6c6f 6362 6c6f 6200  ..o.l.dIlocblob.
-00001400: 0000 1000 0002 ab00 0001 16ff ffff ffff  ................
-00001410: ff00 0000 0000 0300 6f00 6c00 646c 6731  ........o.l.dlg1
-00001420: 5363 6f6d 7000 0000 0000 0000 0000 0000  Scomp...........
-00001430: 0300 6f00 6c00 646d 6f44 4462 6c6f 6200  ..o.l.dmoDDblob.
-00001440: 0000 08eb ad90 c9f6 3ec5 4100 0000 0300  ........>.A.....
-00001450: 6f00 6c00 646d 6f64 4462 6c6f 6200 0000  o.l.dmodDblob...
-00001460: 08eb ad90 c9f6 3ec5 4100 0000 0300 6f00  ......>.A.....o.
-00001470: 6c00 6470 6831 5363 6f6d 7000 0000 0000  l.dph1Scomp.....
-00001480: 0000 0000 0000 0e00 7000 7900 7000 7200  ........p.y.p.r.
-00001490: 6f00 6a00 6500 6300 7400 2e00 7400 6f00  o.j.e.c.t...t.o.
-000014a0: 6d00 6c49 6c6f 6362 6c6f 6200 0000 1000  m.lIlocblob.....
-000014b0: 0002 5e00 0000 87ff ffff ffff ff00 0000  ..^.............
-000014c0: 0000 0900 5200 4500 4100 4400 4d00 4500  ....R.E.A.D.M.E.
-000014d0: 2e00 6d00 6449 6c6f 6362 6c6f 6200 0000  ..m.dIlocblob...
-000014e0: 1000 0002 cc00 0000 87ff ffff ffff ff00  ................
-000014f0: 0000 0000 0300 7300 7200 6349 6c6f 6362  ......s.r.cIlocb
-00001500: 6c6f 6200 0000 1000 0003 3a00 0000 87ff  lob.......:.....
-00001510: ffff ffff ff00 0000 0000 0500 7400 6500  ............t.e.
-00001520: 7300 7400 7349 6c6f 6362 6c6f 6200 0000  s.t.sIlocblob...
-00001530: 1000 0001 1400 0000 f7ff ffff ffff ff00  ................
-00001540: 0000 0000 0a00 5400 4800 4100 4e00 4b00  ......T.H.A.N.K.
-00001550: 5300 2e00 7400 7800 7449 6c6f 6362 6c6f  S...t.x.tIlocblo
-00001560: 6200 0000 1000 0001 0d00 0001 68ff ffff  b...........h...
-00001570: ffff ff00 0000 0000 0000 0000 0000 0000  ................
-00001580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000010c0: 0908 095f 1019 7b7b 3230 332c 2033 3239  ..._..{{203, 329
+000010d0: 7d2c 207b 3132 3337 2c20 3433 367d 7d09  }, {1237, 436}}.
+000010e0: 0815 232f 3b52 5f6b 6c6d 6e6f 8b00 0000  ..#/;R_klmno....
+000010f0: 0000 0001 0100 0000 0000 0000 0d00 0000  ................
+00001100: 0000 0000 0000 0000 0000 0000 8c00 0000  ................
+00001110: 0600 6900 6d00 6100 6700 6500 7369 6376  ..i.m.a.g.e.sicv
+00001120: 7062 6c6f 6200 0001 cd62 706c 6973 7430  pblob....bplist0
+00001130: 30df 1010 0102 0304 0506 0708 090a 0b0c  0...............
+00001140: 0d0e 0f10 1112 1311 1411 1515 1516 1718  ................
+00001150: 191a 1b19 5f10 1362 6163 6b67 726f 756e  ...._..backgroun
+00001160: 6443 6f6c 6f72 426c 7565 5b67 7269 6453  dColorBlue[gridS
+00001170: 7061 6369 6e67 5874 6578 7453 697a 655f  pacingXtextSize_
+00001180: 1012 6261 636b 6772 6f75 6e64 436f 6c6f  ..backgroundColo
+00001190: 7252 6564 5e62 6163 6b67 726f 756e 6454  rRed^backgroundT
+000011a0: 7970 655f 1014 6261 636b 6772 6f75 6e64  ype_..background
+000011b0: 436f 6c6f 7247 7265 656e 5b67 7269 644f  ColorGreen[gridO
+000011c0: 6666 7365 7458 5b67 7269 644f 6666 7365  ffsetX[gridOffse
+000011d0: 7459 5f10 0f73 6372 6f6c 6c50 6f73 6974  tY_..scrollPosit
+000011e0: 696f 6e59 5c73 686f 7749 7465 6d49 6e66  ionY\showItemInf
+000011f0: 6f5f 1012 7669 6577 4f70 7469 6f6e 7356  o_..viewOptionsV
+00001200: 6572 7369 6f6e 5f10 0f73 6372 6f6c 6c50  ersion_..scrollP
+00001210: 6f73 6974 696f 6e58 5d6c 6162 656c 4f6e  ositionX]labelOn
+00001220: 426f 7474 6f6d 5961 7272 616e 6765 4279  BottomYarrangeBy
+00001230: 5869 636f 6e53 697a 655f 100f 7368 6f77  XiconSize_..show
+00001240: 4963 6f6e 5072 6576 6965 7723 3ff0 0000  IconPreview#?...
+00001250: 0000 0000 2340 4b00 0000 0000 0023 4028  ....#@K......#@(
+00001260: 0000 0000 0000 1000 2300 0000 0000 0000  ........#.......
+00001270: 0008 1400 0000 0000 0000 0000 0000 0000  ................
+00001280: 0000 0123 406c 0000 0000 0000 0954 6e6f  ...#@l.......Tno
+00001290: 6e65 2340 5000 0000 0000 0009 0008 002b  ne#@P..........+
+000012a0: 0041 004d 0056 006b 007a 0091 009d 00a9  .A.M.V.k.z......
+000012b0: 00bb 00c8 00dd 00ef 00fd 0107 0110 0122  ..............."
+000012c0: 012b 0134 013d 013f 0148 0149 015a 0163  .+.4.=.?.H.I.Z.c
+000012d0: 0164 0169 0172 0000 0000 0000 0201 0000  .d.i.r..........
+000012e0: 0000 0000 001d 0000 0000 0000 0000 0000  ................
+000012f0: 0000 0000 0173 0000 0006 0069 006d 0061  .....s.....i.m.a
+00001300: 0067 0065 0073 6c67 3153 636f 6d70 0000  .g.e.slg1Scomp..
+00001310: 0000 0000 0000 0000 0006 0069 006d 0061  ...........i.m.a
+00001320: 0067 0065 0073 6d6f 4444 626c 6f62 0000  .g.e.smoDDblob..
+00001330: 0008 4cac c35c 9b3f c541 0000 0006 0069  ..L..\.?.A.....i
+00001340: 006d 0061 0067 0065 0073 6d6f 6444 626c  .m.a.g.e.smodDbl
+00001350: 6f62 0000 0008 4cac c35c 9b3f c541 0000  ob....L..\.?.A..
+00001360: 0006 0069 006d 0061 0067 0065 0073 7068  ...i.m.a.g.e.sph
+00001370: 3153 636f 6d70 0000 0000 0000 0000 0000  1Scomp..........
+00001380: 0006 0069 006d 0061 0067 0065 0073 7653  ...i.m.a.g.e.svS
+00001390: 726e 6c6f 6e67 0000 0001 0000 0007 004c  rnlong.........L
+000013a0: 0049 0043 0045 004e 0053 0045 496c 6f63  .I.C.E.N.S.EIloc
+000013b0: 626c 6f62 0000 0010 0000 0182 0000 0087  blob............
+000013c0: ffff ffff ffff 0000 0000 0003 006e 0065  .............n.e
+000013d0: 0077 496c 6f63 626c 6f62 0000 0010 0000  .wIlocblob......
+000013e0: 0182 0000 00f7 ffff ffff ffff 0000 0000  ................
+000013f0: 0003 006f 006c 0064 496c 6f63 626c 6f62  ...o.l.dIlocblob
+00001400: 0000 0010 0000 02ab 0000 0116 ffff ffff  ................
+00001410: ffff 0000 0000 0003 006f 006c 0064 6473  .........o.l.dds
+00001420: 636c 626f 6f6c 0100 0000 0300 6f00 6c00  clbool......o.l.
+00001430: 646c 6731 5363 6f6d 7000 0000 0000 0000  dlg1Scomp.......
+00001440: 0000 0000 0300 6f00 6c00 646d 6f44 4462  ......o.l.dmoDDb
+00001450: 6c6f 6200 0000 08eb ad90 c9f6 3ec5 4100  lob.........>.A.
+00001460: 0000 0300 6f00 6c00 646d 6f64 4462 6c6f  ....o.l.dmodDblo
+00001470: 6200 0000 08eb ad90 c9f6 3ec5 4100 0000  b.........>.A...
+00001480: 0300 6f00 6c00 6470 6831 5363 6f6d 7000  ..o.l.dph1Scomp.
+00001490: 0000 0000 0000 0000 0000 0e00 7000 7900  ............p.y.
+000014a0: 7000 7200 6f00 6a00 6500 6300 7400 2e00  p.r.o.j.e.c.t...
+000014b0: 7400 6f00 6d00 6c49 6c6f 6362 6c6f 6200  t.o.m.lIlocblob.
+000014c0: 0000 1000 0002 5e00 0000 87ff ffff ffff  ......^.........
+000014d0: ff00 0000 0000 0900 5200 4500 4100 4400  ........R.E.A.D.
+000014e0: 4d00 4500 2e00 6d00 6449 6c6f 6362 6c6f  M.E...m.dIlocblo
+000014f0: 6200 0000 1000 0002 cc00 0000 87ff ffff  b...............
+00001500: ffff ff00 0000 0000 0300 7300 7200 6349  ..........s.r.cI
+00001510: 6c6f 6362 6c6f 6200 0000 1000 0003 3a00  locblob.......:.
+00001520: 0000 87ff ffff ffff ff00 0000 0000 0500  ................
+00001530: 7400 6500 7300 7400 7349 6c6f 6362 6c6f  t.e.s.t.sIlocblo
+00001540: 6200 0000 1000 0001 1400 0000 f7ff ffff  b...............
+00001550: ffff ff00 0000 0000 0a00 5400 4800 4100  ..........T.H.A.
+00001560: 4e00 4b00 5300 2e00 7400 7800 7449 6c6f  N.K.S...t.x.tIlo
+00001570: 6362 6c6f 6200 0000 1000 0001 0d00 0001  cblob...........
+00001580: 68ff ffff ffff ff00 0000 0000 0000 0000  h...............
 00001590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000015f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -457,24 +457,24 @@
 00001c80: 0000 0000 0100 0100 0000 0000 0100 0200  ................
 00001c90: 0000 0000 0100 0400 0000 0000 0100 0800  ................
 00001ca0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
 00001cb0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
 00001cc0: 0000 0000 0101 0000 0000 0000 0102 0000  ................
 00001cd0: 0000 0000 0104 0000 0000 0000 0108 0000  ................
 00001ce0: 0000 0000 0110 0000 0000 0000 0120 0000  ............. ..
-00001cf0: 0000 0000 0140 0000 0000 0000 006f 6362  .....@.......ocb
-00001d00: 6c6f 6200 0000 1000 0003 3a00 0000 87ff  lob.......:.....
-00001d10: ffff ffff ff00 0000 0000 0500 7400 6500  ............t.e.
-00001d20: 7300 7400 7349 6c6f 6362 6c6f 6200 0000  s.t.sIlocblob...
-00001d30: 1000 0001 1400 0000 f7ff ffff ffff ff00  ................
-00001d40: 0000 0000 0a00 5400 4800 4100 4e00 4b00  ......T.H.A.N.K.
-00001d50: 5300 2e00 7400 7800 7449 6c6f 6362 6c6f  S...t.x.tIlocblo
-00001d60: 6200 0000 1000 0001 0d00 0001 68ff ffff  b...........h...
-00001d70: ffff ff00 0000 0000 0000 0000 0000 0000  ................
-00001d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001cf0: 0000 0000 0140 0000 0000 0000 00ff ffff  .....@..........
+00001d00: ffff ff00 0000 0000 0300 7300 7200 6349  ..........s.r.cI
+00001d10: 6c6f 6362 6c6f 6200 0000 1000 0003 3a00  locblob.......:.
+00001d20: 0000 87ff ffff ffff ff00 0000 0000 0500  ................
+00001d30: 7400 6500 7300 7400 7349 6c6f 6362 6c6f  t.e.s.t.sIlocblo
+00001d40: 6200 0000 1000 0001 1400 0000 f7ff ffff  b...............
+00001d50: ffff ff00 0000 0000 0a00 5400 4800 4100  ..........T.H.A.
+00001d60: 4e00 4b00 5300 2e00 7400 7800 7449 6c6f  N.K.S...t.x.tIlo
+00001d70: 6362 6c6f 6200 0000 1000 0001 0d00 0001  cblob...........
+00001d80: 68ff ffff ffff ff00 0000 0000 0000 0000  h...............
 00001d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `tinyfilter-0.1.5/THANKS.txt` & `tinyfilter-0.1.6/THANKS.txt`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.5/images/apple.png` & `tinyfilter-0.1.6/images/apple.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.5/images/art.png` & `tinyfilter-0.1.6/images/art.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.5/images/balloon.png` & `tinyfilter-0.1.6/images/balloon.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.5/images/chanel.png` & `tinyfilter-0.1.6/images/chanel.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.5/images/einstein.png` & `tinyfilter-0.1.6/images/einstein.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.5/images/flowers.png` & `tinyfilter-0.1.6/images/flowers.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.5/images/github.png` & `tinyfilter-0.1.6/images/github.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.5/images/king.png` & `tinyfilter-0.1.6/images/king.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.5/images/lisa.png` & `tinyfilter-0.1.6/images/lisa.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.5/images/mcdonalds.png` & `tinyfilter-0.1.6/images/mcdonalds.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.5/images/paint.png` & `tinyfilter-0.1.6/images/paint.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.5/images/pink.jpeg` & `tinyfilter-0.1.6/images/pink.jpeg`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.5/images/target.png` & `tinyfilter-0.1.6/images/target.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.5/images/test.png` & `tinyfilter-0.1.6/images/test.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.5/images/tiny.png` & `tinyfilter-0.1.6/images/tiny.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.5/images/youtube.png` & `tinyfilter-0.1.6/images/youtube.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.5/new/bin/Activate.ps1` & `tinyfilter-0.1.6/new/bin/Activate.ps1`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.5/new/bin/activate` & `tinyfilter-0.1.6/new/bin/activate`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.5/new/bin/activate.csh` & `tinyfilter-0.1.6/new/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.5/new/bin/activate.fish` & `tinyfilter-0.1.6/new/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.5/old/.DS_Store` & `tinyfilter-0.1.6/old/.DS_Store`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.5/old/__main__.py` & `tinyfilter-0.1.6/old/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.5/old/backup.py` & `tinyfilter-0.1.6/old/backup.py`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.5/old/example_image.png` & `tinyfilter-0.1.6/old/example_image.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.5/old/main.py` & `tinyfilter-0.1.6/old/main.py`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.5/old/main_debug.py` & `tinyfilter-0.1.6/old/main_debug.py`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.5/old/nike.png` & `tinyfilter-0.1.6/images/nike.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.5/old/nike2.png` & `tinyfilter-0.1.6/images/nike2.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.5/old/output_image.png` & `tinyfilter-0.1.6/old/output_image.png`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.5/src/tinyfilter/__init__.py` & `tinyfilter-0.1.6/src/tinyfilter/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,25 +88,36 @@
             print_filter_output(img_region)
 
 
 def tiny_print(img_filename=None) -> None:
     """Loads an image and prints it as ASCII characters to the console"""
     if img_filename == None:
         parser = argparse.ArgumentParser(
-            prog="ProgramName",
+            prog="tinyfilter",
             description="What the program does",
             epilog="Text at the bottom of help",
         )
         parser.add_argument("filename")
 
         args = parser.parse_args()
         img_raw = Image.open(args.filename)
     else:
         img_raw = Image.open(img_filename)
 
+    # checks if the image type is supported by tinyfilter
+    if img_raw.mode != "RGB" and img_raw.mode != "RGBA":
+        parser.error('''
+    
+    Image mode was {}. Currently tinyfilter only supports modes of "RGB" and 
+    "RGBA." To learn more about image modes visit the Pillow (a dependency 
+    of tinyfilter) documentation:
+
+    https://pillow.readthedocs.io/en/stable/handbook/concepts.html#concept-modes
+        '''.format(img_raw.mode))
+
     img_raw = img_raw.resize((LOAD_IMG_WIDTH, LOAD_IMG_HEIGHT))
     img: NDArray[np.uint8] = np.array(img_raw)
 
     # Removes alpha channel from an image if present
     if img_raw.mode == "RGBA":
         img = img[:, :, 0:3]
```

### Comparing `tinyfilter-0.1.5/.gitignore` & `tinyfilter-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.5/LICENSE` & `tinyfilter-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyfilter-0.1.5/README.md` & `tinyfilter-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,27 @@
+Metadata-Version: 2.1
+Name: tinyfilter
+Version: 0.1.6
+Summary: tinyfilter is the computer vision equivalent to micrograd. It convert images into ASCII art using the principles of CNNs (convolutional neural networks).
+Project-URL: Homepage, https://github.com/zroe1/tinyfilter/tree/main
+Author-email: Zephaniah Roe <zroe@uchicago.edu>
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Requires-Dist: numpy~=1.25.0
+Requires-Dist: pillow
+Description-Content-Type: text/markdown
+
 # tinyfilter
 <img width="1423" alt="Screenshot 2023-08-05 at 4 52 21 PM" src="https://github.com/zroe1/tinyfilter/assets/114773939/488e61be-3431-444c-9fcc-8ae8944c8b59">  
 </br></br>  
 <p align="center">
-<a href="https://github.com/zroe1/tinyfilter/blob/main/LICENSE"><img alt="link to license" src="https://img.shields.io/badge/pypi-v0.1.4-brightgreen"></a>
+<a href="https://pypi.org/project/tinyfilter/0.1.6/"><img alt="link to PyPi" src="https://img.shields.io/badge/pypi-v0.1.6-brightgreen"></a>
 <a href="https://github.com/zroe1/tinyfilter/blob/main/LICENSE"><img alt="link to license" src="https://img.shields.io/badge/License-MIT-purple"></a>
 <a href="https://github.com/psf/black/tree/main"><img alt="link to license" src="https://img.shields.io/badge/code%20style-black-black"></a>
 </p> 
 
 tinyfilter [^1] is the computer vision equivalent to Andrej Karpathy's <a href="https://github.com/karpathy/micrograd">micrograd</a>. It convert images into ASCII art using the principles of CNNs (convolutional neural networks).  
 </br>
 Unlike other tools of its type, which map pixel darkness to an ASCII character, tinyfilter uses filters and convolution to detect features in an image and prints ASCII characters that correspond to them. This leads to much better results compared to other libraries, especially for smaller images.
```

#### html2text {}

```diff
@@ -1,9 +1,18 @@
-# tinyfilter [Screenshot 2023-08-05 at 4 52 21 PM]
-             [link_to_license] [link_to_license] [link_to_license]
+Metadata-Version: 2.1 Name: tinyfilter Version: 0.1.6 Summary: tinyfilter is
+the computer vision equivalent to micrograd. It convert images into ASCII art
+using the principles of CNNs (convolutional neural networks). Project-URL:
+Homepage, https://github.com/zroe1/tinyfilter/tree/main Author-email: Zephaniah
+Roe
+uchicago.edu> License-File: LICENSE Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Classifier: Programming
+Language :: Python :: 3 Requires-Python: >=3.7 Requires-Dist: numpy~=1.25.0
+Requires-Dist: pillow Description-Content-Type: text/markdown # tinyfilter
+[Screenshot 2023-08-05 at 4 52 21 PM]
+              [link_to_PyPi] [link_to_license] [link_to_license]
 tinyfilter [^1] is the computer vision equivalent to Andrej Karpathy's
 micrograd. It convert images into ASCII art using the principles of CNNs
 (convolutional neural networks).  Unlike other tools of its type, which map
 pixel darkness to an ASCII character, tinyfilter uses filters and convolution
 to detect features in an image and prints ASCII characters that correspond to
 them. This leads to much better results compared to other libraries, especially
 for smaller images. [^1]: For consistency, the first letter in "tinyfilter" is
```

### Comparing `tinyfilter-0.1.5/pyproject.toml` & `tinyfilter-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tinyfilter"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Zephaniah Roe", email="zroe@uchicago.edu" },
 ]
 description = "tinyfilter is the computer vision equivalent to micrograd. It convert images into ASCII art using the principles of CNNs (convolutional neural networks)."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `tinyfilter-0.1.5/PKG-INFO` & `tinyfilter-0.1.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,12 @@
-Metadata-Version: 2.1
-Name: tinyfilter
-Version: 0.1.5
-Summary: tinyfilter is the computer vision equivalent to micrograd. It convert images into ASCII art using the principles of CNNs (convolutional neural networks).
-Project-URL: Homepage, https://github.com/zroe1/tinyfilter/tree/main
-Author-email: Zephaniah Roe <zroe@uchicago.edu>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Requires-Dist: numpy~=1.25.0
-Requires-Dist: pillow
-Description-Content-Type: text/markdown
-
 # tinyfilter
 <img width="1423" alt="Screenshot 2023-08-05 at 4 52 21 PM" src="https://github.com/zroe1/tinyfilter/assets/114773939/488e61be-3431-444c-9fcc-8ae8944c8b59">  
 </br></br>  
 <p align="center">
-<a href="https://github.com/zroe1/tinyfilter/blob/main/LICENSE"><img alt="link to license" src="https://img.shields.io/badge/pypi-v0.1.4-brightgreen"></a>
+<a href="https://pypi.org/project/tinyfilter/0.1.6/"><img alt="link to PyPi" src="https://img.shields.io/badge/pypi-v0.1.6-brightgreen"></a>
 <a href="https://github.com/zroe1/tinyfilter/blob/main/LICENSE"><img alt="link to license" src="https://img.shields.io/badge/License-MIT-purple"></a>
 <a href="https://github.com/psf/black/tree/main"><img alt="link to license" src="https://img.shields.io/badge/code%20style-black-black"></a>
 </p> 
 
 tinyfilter [^1] is the computer vision equivalent to Andrej Karpathy's <a href="https://github.com/karpathy/micrograd">micrograd</a>. It convert images into ASCII art using the principles of CNNs (convolutional neural networks).  
 </br>
 Unlike other tools of its type, which map pixel darkness to an ASCII character, tinyfilter uses filters and convolution to detect features in an image and prints ASCII characters that correspond to them. This leads to much better results compared to other libraries, especially for smaller images.
```

#### html2text {}

```diff
@@ -1,18 +1,9 @@
-Metadata-Version: 2.1 Name: tinyfilter Version: 0.1.5 Summary: tinyfilter is
-the computer vision equivalent to micrograd. It convert images into ASCII art
-using the principles of CNNs (convolutional neural networks). Project-URL:
-Homepage, https://github.com/zroe1/tinyfilter/tree/main Author-email: Zephaniah
-Roe
-uchicago.edu> License-File: LICENSE Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Classifier: Programming
-Language :: Python :: 3 Requires-Python: >=3.7 Requires-Dist: numpy~=1.25.0
-Requires-Dist: pillow Description-Content-Type: text/markdown # tinyfilter
-[Screenshot 2023-08-05 at 4 52 21 PM]
-             [link_to_license] [link_to_license] [link_to_license]
+# tinyfilter [Screenshot 2023-08-05 at 4 52 21 PM]
+              [link_to_PyPi] [link_to_license] [link_to_license]
 tinyfilter [^1] is the computer vision equivalent to Andrej Karpathy's
 micrograd. It convert images into ASCII art using the principles of CNNs
 (convolutional neural networks).  Unlike other tools of its type, which map
 pixel darkness to an ASCII character, tinyfilter uses filters and convolution
 to detect features in an image and prints ASCII characters that correspond to
 them. This leads to much better results compared to other libraries, especially
 for smaller images. [^1]: For consistency, the first letter in "tinyfilter" is
```

