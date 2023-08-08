# Comparing `tmp/receptor_germline_tools-0.0.2.tar.gz` & `tmp/receptor_germline_tools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "receptor_germline_tools-0.0.2.tar", last modified: Sat Jul  9 14:22:58 2022, max compression
+gzip compressed data, was "receptor_germline_tools-0.0.4.tar", last modified: Tue Aug  8 08:46:51 2023, max compression
```

## Comparing `receptor_germline_tools-0.0.2.tar` & `receptor_germline_tools-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxrwx   0        0        0        0 2022-07-09 14:22:58.376432 receptor_germline_tools-0.0.2/
--rw-rw-rw-   0        0        0      240 2022-07-07 12:40:04.000000 receptor_germline_tools-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     7254 2022-07-09 14:22:58.376432 receptor_germline_tools-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     6612 2022-07-09 08:36:52.000000 receptor_germline_tools-0.0.2/README.md
--rw-rw-rw-   0        0        0      121 2022-07-07 12:40:04.000000 receptor_germline_tools-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0     1018 2022-07-09 14:22:58.376432 receptor_germline_tools-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-07-09 14:22:58.319568 receptor_germline_tools-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2022-07-09 14:22:58.335170 receptor_germline_tools-0.0.2/src/receptor_germline_tools/
--rw-rw-rw-   0        0        0        0 2022-07-07 12:40:04.000000 receptor_germline_tools-0.0.2/src/receptor_germline_tools/__init__.py
--rw-rw-rw-   0        0        0     3535 2022-07-09 14:22:08.000000 receptor_germline_tools-0.0.2/src/receptor_germline_tools/add_germline_annotations.py
--rw-rw-rw-   0        0        0     2117 2022-07-07 18:53:16.000000 receptor_germline_tools-0.0.2/src/receptor_germline_tools/convert_fasta_labels.py
--rw-rw-rw-   0        0        0     2850 2022-07-09 08:50:58.000000 receptor_germline_tools-0.0.2/src/receptor_germline_tools/germline_utils.py
-drwxrwxrwx   0        0        0        0 2022-07-09 14:22:58.360800 receptor_germline_tools-0.0.2/src/receptor_germline_tools.egg-info/
--rw-rw-rw-   0        0        0     7254 2022-07-09 14:22:58.000000 receptor_germline_tools-0.0.2/src/receptor_germline_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      494 2022-07-09 14:22:58.000000 receptor_germline_tools-0.0.2/src/receptor_germline_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-09 14:22:58.000000 receptor_germline_tools-0.0.2/src/receptor_germline_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      172 2022-07-09 14:22:58.000000 receptor_germline_tools-0.0.2/src/receptor_germline_tools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       24 2022-07-09 14:22:58.000000 receptor_germline_tools-0.0.2/src/receptor_germline_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-08 08:46:51.152140 receptor_germline_tools-0.0.4/
+-rw-rw-rw-   0        0        0      240 2022-07-06 10:12:30.000000 receptor_germline_tools-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1024 2023-08-08 08:46:51.152140 receptor_germline_tools-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2023-08-08 08:46:15.000000 receptor_germline_tools-0.0.4/README.md
+-rw-rw-rw-   0        0        0      121 2022-07-06 10:12:30.000000 receptor_germline_tools-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1077 2023-08-08 08:46:51.154139 receptor_germline_tools-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-08 08:46:51.029140 receptor_germline_tools-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-08-08 08:46:51.143139 receptor_germline_tools-0.0.4/src/receptor_germline_tools/
+-rw-rw-rw-   0        0        0        0 2022-07-06 10:12:30.000000 receptor_germline_tools-0.0.4/src/receptor_germline_tools/__init__.py
+-rw-rw-rw-   0        0        0     3640 2023-08-07 11:44:29.000000 receptor_germline_tools-0.0.4/src/receptor_germline_tools/add_germline_annotations.py
+-rw-rw-rw-   0        0        0     5142 2023-08-08 08:35:10.000000 receptor_germline_tools-0.0.4/src/receptor_germline_tools/annotate_rearrangements.py
+-rw-rw-rw-   0        0        0     2263 2023-08-07 11:43:48.000000 receptor_germline_tools-0.0.4/src/receptor_germline_tools/convert_fasta_labels.py
+-rw-rw-rw-   0        0        0     4491 2023-08-08 08:32:05.000000 receptor_germline_tools-0.0.4/src/receptor_germline_tools/create_fasta.py
+-rw-rw-rw-   0        0        0     4671 2023-08-06 13:43:51.000000 receptor_germline_tools-0.0.4/src/receptor_germline_tools/germline_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-08 08:46:51.151139 receptor_germline_tools-0.0.4/src/receptor_germline_tools.egg-info/
+-rw-rw-rw-   0        0        0     1024 2023-08-08 08:46:51.000000 receptor_germline_tools-0.0.4/src/receptor_germline_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      593 2023-08-08 08:46:51.000000 receptor_germline_tools-0.0.4/src/receptor_germline_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 08:46:51.000000 receptor_germline_tools-0.0.4/src/receptor_germline_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      229 2023-08-08 08:46:51.000000 receptor_germline_tools-0.0.4/src/receptor_germline_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       24 2023-08-08 08:46:51.000000 receptor_germline_tools-0.0.4/src/receptor_germline_tools.egg-info/top_level.txt
```

### Comparing `receptor_germline_tools-0.0.2/setup.cfg` & `receptor_germline_tools-0.0.4/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2072 6563 6570 746f 725f 6765 726d   = receptor_germ
 00000020: 6c69 6e65 5f74 6f6f 6c73 0d0a 7665 7273  line_tools..vers
-00000030: 696f 6e20 3d20 302e 302e 320d 0a61 7574  ion = 0.0.2..aut
+00000030: 696f 6e20 3d20 302e 302e 340d 0a61 7574  ion = 0.0.4..aut
 00000040: 686f 7220 3d20 5769 6c6c 6961 6d20 4c65  hor = William Le
 00000050: 6573 0d0a 6175 7468 6f72 5f65 6d61 696c  es..author_email
 00000060: 203d 2077 696c 6c69 616d 406c 6565 732e   = william@lees.
 00000070: 6f72 672e 756b 0d0a 6465 7363 7269 7074  org.uk..descript
 00000080: 696f 6e20 3d20 546f 6f6c 7320 666f 7220  ion = Tools for 
 00000090: 776f 726b 696e 6720 7769 7468 2041 4952  working with AIR
 000000a0: 5220 7374 616e 6461 7264 2049 472f 5452  R standard IG/TR
@@ -54,11 +54,15 @@
 00000350: 7074 6f72 5f67 6572 6d6c 696e 655f 746f  ptor_germline_to
 00000360: 6f6c 732e 6164 645f 6765 726d 6c69 6e65  ols.add_germline
 00000370: 5f61 6e6e 6f74 6174 696f 6e73 3a6d 6169  _annotations:mai
 00000380: 6e0d 0a09 636f 6e76 6572 745f 6661 7374  n...convert_fast
 00000390: 615f 6c61 6265 6c73 203d 2072 6563 6570  a_labels = recep
 000003a0: 746f 725f 6765 726d 6c69 6e65 5f74 6f6f  tor_germline_too
 000003b0: 6c73 2e63 6f6e 7665 7274 5f66 6173 7461  ls.convert_fasta
-000003c0: 5f6c 6162 656c 733a 6d61 696e 0d0a 0d0a  _labels:main....
-000003d0: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
-000003e0: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
-000003f0: 7465 203d 2030 0d0a 0d0a                 te = 0....
+000003c0: 5f6c 6162 656c 733a 6d61 696e 0d0a 0963  _labels:main...c
+000003d0: 7265 6174 655f 6661 7374 6120 3d20 7265  reate_fasta = re
+000003e0: 6365 7074 6f72 5f67 6572 6d6c 696e 655f  ceptor_germline_
+000003f0: 746f 6f6c 732e 6372 6561 7465 5f66 6173  tools.create_fas
+00000400: 7461 3a6d 6169 6e0d 0a0d 0a5b 6567 675f  ta:main....[egg_
+00000410: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
+00000420: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
+00000430: 300d 0a0d 0a                             0....
```

### Comparing `receptor_germline_tools-0.0.2/src/receptor_germline_tools/add_germline_annotations.py` & `receptor_germline_tools-0.0.4/src/receptor_germline_tools/add_germline_annotations.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,28 +7,37 @@
 # the English version of which is available here: https://perma.cc/DK5U-NDVE
 
 
 import csv
 import argparse
 import os
 import csv
-from receptor_germline_tools.germline_utils import *
 
+try:
+    from receptor_germline_tools.germline_utils import *
+except:
+    from germline_utils import *
 
-def main():
+
+
+
+def get_parser():
     parser = argparse.ArgumentParser(description='Convert IgLabel-style labels in an alignment file to dummy IUIS format')
     parser.add_argument('input_file', help='alignments to annotate (csv, tsv)')
     parser.add_argument('output_file', help='output with added annotations')
     parser.add_argument('germline_set', help='AIRR standard germline set to use for metadata (JSON)')
     parser.add_argument('-c', '--call_columns', help='Names of one or more columns to be processed, separated by commas', default='v_call,d_call,j_call')
     parser.add_argument('-s', '--dummy_subgroup', help='The subgroup to be used, where no value is specified in the germline set metadata', default='0')
     parser.add_argument('-a', '--dummy_allele', help='The allele to be used, where no value is specified in the germline set metadata', default='00')
     parser.add_argument('-u', '--un_dummy', help='translate dummy names back to label form', action="store_true")
+    return parser
+
 
-    args = parser.parse_args()
+def main():
+    args = get_parser().parse_args()
     call_columns = args.call_columns.split(',')
 
     missing_files = False
     for filespec in [(args.input_file, 'input_file'), (args.germline_set, 'germline_set')]:
         if not os.path.isfile(filespec[0]):
             print(f'{filespec[1]} {filespec[0]} does not exist.')
             missing_files = True
```

### Comparing `receptor_germline_tools-0.0.2/src/receptor_germline_tools/convert_fasta_labels.py` & `receptor_germline_tools-0.0.4/src/receptor_germline_tools/convert_fasta_labels.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,48 +9,56 @@
 
 import csv
 import argparse
 import os
 import json
 from collections import namedtuple
 import csv
-from receptor_germline_tools.germline_utils import *
 
+try:
+    from receptor_germline_tools.germline_utils import *
+except:
+    from germline_utils import *
 
-def main():
+
+def get_parser():
     parser = argparse.ArgumentParser(description='Convert IgLabel-style labels in a FASTA file to dummy IUIS format')
     parser.add_argument('input_file', help='records to convert (FASTA)')
     parser.add_argument('output_file', help='converted output (FASTA)')
-    parser.add_argument('germline_set', help='AIRR standard germline set to use for metadata (JSON)')
+    parser.add_argument('-g', '--germline_set', help='AIRR standard germline set to use for metadata (JSON)', default=None)
     parser.add_argument('-s', '--dummy_subgroup', help='subgroup to use when no subgroup has been defined', default='0')
     parser.add_argument('-a', '--dummy_allele', help='allele to use when no allele has been defined', default='00')
-    parser.add_argument('-u', '--un_dummy', help='translate dummy names back to label form', action="store_true")
-
-    args = parser.parse_args()
+    parser.add_argument('-u', '--un_dummy', help='translate dummy names back to label form', action="store_true", default=False)
+    return parser
 
-    missing_files = False
-    for filespec in [(args.input_file, 'input_file'), (args.germline_set, 'germline_set')]:
-        if not os.path.isfile(filespec[0]):
-            print(f'{filespec[1]} {filespec[0]} does not exist.')
-            missing_files = True
 
-    if missing_files:
-        exit(1)
+def main():
+    args = get_parser().parse_args()
 
-    germline_data = read_germline_data(args)
+    if not os.path.isfile(args.input_file):
+        print(f'{args.input_file} does not exist.')
+        exit(0)
+
+    germline_data = {}
+    if args.germline_set:
+        if os.path.isfile(args.germline_set):
+            germline_data = read_germline_data(args)
+        else:
+            print(f'{args.germline_set} does not exist.')
+            exit(0)
 
     recs = read_fasta(args.input_file)
     converted_recs = {}
 
     for name, seq in recs.items():
         if '|' in name:
             name = name.split('|')[0].replace(' ', '')
         if args.un_dummy:
             converted_recs[undummify(name, args.dummy_allele)] = seq
         else:
             converted_recs[dummify(name, germline_data, args.dummy_subgroup, args.dummy_allele)] = seq
 
-    write_fasta(converted_recs, args.output_file)
+    write_fasta(args.output_file, converted_recs)
 
 
 if __name__ == "__main__":
     main()
```

