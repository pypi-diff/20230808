# Comparing `tmp/orbitkit-0.4.1.tar.gz` & `tmp/orbitkit-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/orbitkit-0.4.1.tar", last modified: Mon Jun  5 03:33:26 2023, max compression
+gzip compressed data, was "dist/orbitkit-0.4.2.tar", last modified: Tue Aug  8 05:23:08 2023, max compression
```

## Comparing `orbitkit-0.4.1.tar` & `orbitkit-0.4.2.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-06-05 03:33:26.000000 orbitkit-0.4.1/
--rw-r--r--   0 crown      (501) staff       (20)     1073 2020-10-28 02:45:18.000000 orbitkit-0.4.1/LICENSE
--rw-r--r--   0 crown      (501) staff       (20)      118 2022-01-24 08:00:21.000000 orbitkit-0.4.1/MANIFEST.in
--rw-r--r--   0 crown      (501) staff       (20)     3137 2023-06-05 03:33:26.000000 orbitkit-0.4.1/PKG-INFO
--rw-r--r--   0 crown      (501) staff       (20)     1684 2023-05-25 06:23:46.000000 orbitkit-0.4.1/README.md
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-06-05 03:33:26.000000 orbitkit-0.4.1/orbitkit/
--rw-r--r--   0 crown      (501) staff       (20)        6 2023-06-05 03:30:31.000000 orbitkit-0.4.1/orbitkit/VERSION
--rw-r--r--   0 crown      (501) staff       (20)      292 2023-05-25 06:23:46.000000 orbitkit-0.4.1/orbitkit/__init__.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-06-05 03:33:26.000000 orbitkit-0.4.1/orbitkit/id_srv/
--rw-r--r--   0 crown      (501) staff       (20)       22 2021-12-26 09:49:52.000000 orbitkit-0.4.1/orbitkit/id_srv/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)     1533 2021-12-26 11:07:53.000000 orbitkit-0.4.1/orbitkit/id_srv/id_gen.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-06-05 03:33:26.000000 orbitkit-0.4.1/orbitkit/lark_send/
--rw-r--r--   0 crown      (501) staff       (20)       20 2022-01-05 07:16:58.000000 orbitkit-0.4.1/orbitkit/lark_send/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)     5064 2022-01-05 07:16:58.000000 orbitkit-0.4.1/orbitkit/lark_send/lark.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-06-05 03:33:26.000000 orbitkit-0.4.1/orbitkit/pdf_extractor/
--rw-r--r--   0 crown      (501) staff       (20)        0 2023-05-10 05:20:41.000000 orbitkit-0.4.1/orbitkit/pdf_extractor/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)      621 2023-05-10 06:21:50.000000 orbitkit-0.4.1/orbitkit/pdf_extractor/pdf_block_extractor_base.py
--rw-r--r--   0 crown      (501) staff       (20)     6115 2023-05-24 08:44:38.000000 orbitkit-0.4.1/orbitkit/pdf_extractor/pdf_block_extractor_v1.py
--rw-r--r--   0 crown      (501) staff       (20)    13625 2023-05-24 09:10:22.000000 orbitkit-0.4.1/orbitkit/pdf_extractor/pdf_block_extractor_v2.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-06-05 03:33:26.000000 orbitkit-0.4.1/orbitkit/util/
--rw-r--r--   0 crown      (501) staff       (20)      438 2023-06-05 03:28:29.000000 orbitkit-0.4.1/orbitkit/util/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)      790 2023-05-10 05:20:41.000000 orbitkit-0.4.1/orbitkit/util/common.py
--rw-r--r--   0 crown      (501) staff       (20)      520 2023-05-10 05:26:36.000000 orbitkit-0.4.1/orbitkit/util/util_aws.py
--rw-r--r--   0 crown      (501) staff       (20)     1781 2023-05-20 01:15:42.000000 orbitkit-0.4.1/orbitkit/util/util_date.py
--rw-r--r--   0 crown      (501) staff       (20)      148 2023-05-10 05:19:04.000000 orbitkit-0.4.1/orbitkit/util/util_str.py
--rw-r--r--   0 crown      (501) staff       (20)    20634 2023-06-05 03:28:29.000000 orbitkit-0.4.1/orbitkit/util/util_type_mapping.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-06-05 03:33:26.000000 orbitkit-0.4.1/orbitkit.egg-info/
--rw-r--r--   0 crown      (501) staff       (20)     3137 2023-06-05 03:33:26.000000 orbitkit-0.4.1/orbitkit.egg-info/PKG-INFO
--rw-r--r--   0 crown      (501) staff       (20)      726 2023-06-05 03:33:26.000000 orbitkit-0.4.1/orbitkit.egg-info/SOURCES.txt
--rw-r--r--   0 crown      (501) staff       (20)        1 2023-06-05 03:33:26.000000 orbitkit-0.4.1/orbitkit.egg-info/dependency_links.txt
--rw-r--r--   0 crown      (501) staff       (20)        1 2023-06-05 03:33:26.000000 orbitkit-0.4.1/orbitkit.egg-info/not-zip-safe
--rw-r--r--   0 crown      (501) staff       (20)       89 2023-06-05 03:33:26.000000 orbitkit-0.4.1/orbitkit.egg-info/requires.txt
--rw-r--r--   0 crown      (501) staff       (20)        9 2023-06-05 03:33:26.000000 orbitkit-0.4.1/orbitkit.egg-info/top_level.txt
--rw-r--r--   0 crown      (501) staff       (20)       38 2023-06-05 03:33:26.000000 orbitkit-0.4.1/setup.cfg
--rw-r--r--   0 crown      (501) staff       (20)     1547 2023-05-10 05:35:02.000000 orbitkit-0.4.1/setup.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-08-08 05:23:08.000000 orbitkit-0.4.2/
+-rw-r--r--   0 crown      (501) staff       (20)     1073 2020-10-28 02:45:18.000000 orbitkit-0.4.2/LICENSE
+-rw-r--r--   0 crown      (501) staff       (20)      118 2022-01-24 08:00:21.000000 orbitkit-0.4.2/MANIFEST.in
+-rw-r--r--   0 crown      (501) staff       (20)     3137 2023-08-08 05:23:08.000000 orbitkit-0.4.2/PKG-INFO
+-rw-r--r--   0 crown      (501) staff       (20)     1684 2023-05-25 06:23:46.000000 orbitkit-0.4.2/README.md
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-08-08 05:23:08.000000 orbitkit-0.4.2/orbitkit/
+-rw-r--r--   0 crown      (501) staff       (20)        6 2023-08-08 05:21:22.000000 orbitkit-0.4.2/orbitkit/VERSION
+-rw-r--r--   0 crown      (501) staff       (20)      292 2023-05-25 06:23:46.000000 orbitkit-0.4.2/orbitkit/__init__.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-08-08 05:23:08.000000 orbitkit-0.4.2/orbitkit/id_srv/
+-rw-r--r--   0 crown      (501) staff       (20)       22 2021-12-26 09:49:52.000000 orbitkit-0.4.2/orbitkit/id_srv/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)     1533 2021-12-26 11:07:53.000000 orbitkit-0.4.2/orbitkit/id_srv/id_gen.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-08-08 05:23:08.000000 orbitkit-0.4.2/orbitkit/lark_send/
+-rw-r--r--   0 crown      (501) staff       (20)       20 2022-01-05 07:16:58.000000 orbitkit-0.4.2/orbitkit/lark_send/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)     5064 2022-01-05 07:16:58.000000 orbitkit-0.4.2/orbitkit/lark_send/lark.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-08-08 05:23:08.000000 orbitkit-0.4.2/orbitkit/pdf_extractor/
+-rw-r--r--   0 crown      (501) staff       (20)        0 2023-05-10 05:20:41.000000 orbitkit-0.4.2/orbitkit/pdf_extractor/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)      898 2023-08-07 08:25:29.000000 orbitkit-0.4.2/orbitkit/pdf_extractor/exceptions.py
+-rw-r--r--   0 crown      (501) staff       (20)      621 2023-05-10 06:21:50.000000 orbitkit-0.4.2/orbitkit/pdf_extractor/pdf_block_extractor_base.py
+-rw-r--r--   0 crown      (501) staff       (20)     6330 2023-08-07 10:18:13.000000 orbitkit-0.4.2/orbitkit/pdf_extractor/pdf_block_extractor_v1.py
+-rw-r--r--   0 crown      (501) staff       (20)    13780 2023-08-07 10:18:13.000000 orbitkit-0.4.2/orbitkit/pdf_extractor/pdf_block_extractor_v2.py
+-rw-r--r--   0 crown      (501) staff       (20)        5 2023-08-07 08:59:37.000000 orbitkit-0.4.2/orbitkit/pdf_extractor/pdf_extractor_azure.py
+-rw-r--r--   0 crown      (501) staff       (20)     8860 2023-08-08 03:38:34.000000 orbitkit-0.4.2/orbitkit/pdf_extractor/pdf_extractor_orbit.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-08-08 05:23:08.000000 orbitkit-0.4.2/orbitkit/util/
+-rw-r--r--   0 crown      (501) staff       (20)      464 2023-08-07 09:21:21.000000 orbitkit-0.4.2/orbitkit/util/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)     1667 2023-08-07 09:08:32.000000 orbitkit-0.4.2/orbitkit/util/common.py
+-rw-r--r--   0 crown      (501) staff       (20)      520 2023-05-10 05:26:36.000000 orbitkit-0.4.2/orbitkit/util/util_aws.py
+-rw-r--r--   0 crown      (501) staff       (20)     1781 2023-05-20 01:15:42.000000 orbitkit-0.4.2/orbitkit/util/util_date.py
+-rw-r--r--   0 crown      (501) staff       (20)      148 2023-05-10 05:19:04.000000 orbitkit-0.4.2/orbitkit/util/util_str.py
+-rw-r--r--   0 crown      (501) staff       (20)    20634 2023-06-05 03:28:29.000000 orbitkit-0.4.2/orbitkit/util/util_type_mapping.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-08-08 05:23:08.000000 orbitkit-0.4.2/orbitkit.egg-info/
+-rw-r--r--   0 crown      (501) staff       (20)     3137 2023-08-08 05:23:07.000000 orbitkit-0.4.2/orbitkit.egg-info/PKG-INFO
+-rw-r--r--   0 crown      (501) staff       (20)      855 2023-08-08 05:23:07.000000 orbitkit-0.4.2/orbitkit.egg-info/SOURCES.txt
+-rw-r--r--   0 crown      (501) staff       (20)        1 2023-08-08 05:23:07.000000 orbitkit-0.4.2/orbitkit.egg-info/dependency_links.txt
+-rw-r--r--   0 crown      (501) staff       (20)        1 2023-08-08 05:23:07.000000 orbitkit-0.4.2/orbitkit.egg-info/not-zip-safe
+-rw-r--r--   0 crown      (501) staff       (20)       63 2023-08-08 05:23:07.000000 orbitkit-0.4.2/orbitkit.egg-info/requires.txt
+-rw-r--r--   0 crown      (501) staff       (20)        9 2023-08-08 05:23:07.000000 orbitkit-0.4.2/orbitkit.egg-info/top_level.txt
+-rw-r--r--   0 crown      (501) staff       (20)       38 2023-08-08 05:23:08.000000 orbitkit-0.4.2/setup.cfg
+-rw-r--r--   0 crown      (501) staff       (20)     1508 2023-08-07 08:44:39.000000 orbitkit-0.4.2/setup.py
```

### Comparing `orbitkit-0.4.1/LICENSE` & `orbitkit-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `orbitkit-0.4.1/PKG-INFO` & `orbitkit-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbitkit
-Version: 0.4.1
+Version: 0.4.2
 Summary: This project is only for Orbit Tech internal use.
 Home-page: https://github.com/clown-0726/orbitkit
 Author: Lilu Cao
 Author-email: lilu.cao@qq.com
 Maintainer: Lilu Cao
 Maintainer-email: lilu.cao@qq.com
 License: MIT License
```

### Comparing `orbitkit-0.4.1/README.md` & `orbitkit-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `orbitkit-0.4.1/orbitkit/id_srv/id_gen.py` & `orbitkit-0.4.2/orbitkit/id_srv/id_gen.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.4.1/orbitkit/lark_send/lark.py` & `orbitkit-0.4.2/orbitkit/lark_send/lark.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.4.1/orbitkit/pdf_extractor/pdf_block_extractor_base.py` & `orbitkit-0.4.2/orbitkit/pdf_extractor/pdf_block_extractor_base.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.4.1/orbitkit/pdf_extractor/pdf_block_extractor_v1.py` & `orbitkit-0.4.2/orbitkit/pdf_extractor/pdf_block_extractor_v1.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 import time
 from typing import Optional, List
-from pdfminer.high_level import extract_pages
-from pdfminer.layout import LTTextContainer, LTFigure, LTChar
 from orbitkit import id_srv
 from orbitkit.pdf_extractor.pdf_block_extractor_base import PdfBlockExtractBase
 import logging
-from Crypto.Cipher import AES
+
+try:
+    from pdfminer.high_level import extract_pages
+    from pdfminer.layout import LTTextContainer, LTFigure, LTChar
+    import pdfplumber
+    from Crypto.Cipher import AES
+except ImportError:
+    raise ValueError(
+        "Please install below packages before using PDF Extractor function."
+        "- pdfminer"
+        "- pdfplumber >= 0.9.0"
+        "- pycryptodome >= 3.11.0"
+    )
 
 logger = logging.getLogger(__name__)
 
 """
 >>> 注意事项 <<<
 pdfminer.six page 索引是从 1 开始的
 pdfplumber page 索引是从 0 开始的
@@ -146,11 +156,7 @@
         else:
             # 解析所有页面
             for page_layout in page_layouts:
                 yield self.loop_pages(page_layout)
 
         end_extract_time = time.perf_counter() - start_extract_time
         logger.warning(f'End extract pdf with cost time {str(end_extract_time * 1000)}')
-
-
-if __name__ == '__main__':
-    pass
```

### Comparing `orbitkit-0.4.1/orbitkit/pdf_extractor/pdf_block_extractor_v2.py` & `orbitkit-0.4.2/orbitkit/pdf_extractor/pdf_block_extractor_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 import time
 from typing import Optional, List, Union
-from pdfminer.high_level import extract_pages
-from pdfminer.layout import LTTextContainer, LTFigure, LTChar
-import pdfplumber
 import logging
 from orbitkit import id_srv
 from prettytable import PrettyTable
 from orbitkit.pdf_extractor.pdf_block_extractor_base import PdfBlockExtractBase
-from Crypto.Cipher import AES
+
+try:
+    from pdfminer.high_level import extract_pages
+    from pdfminer.layout import LTTextContainer, LTFigure, LTChar
+    import pdfplumber
+    from Crypto.Cipher import AES
+except ImportError:
+    raise ValueError(
+        "Please install below packages before using PDF Extractor function."
+        "- pdfminer"
+        "- pdfplumber >= 0.9.0"
+        "- pycryptodome >= 3.11.0"
+    )
 
 logger = logging.getLogger(__name__)
 
 """方法说明：
 >>> 安装包 <<<
 pip install pdfplumber # pdfplumber 是基于 pdfminer.six 的，安装这个包的同时也会安装 pdfminer.six
 pip install pycryptodome # 有些 pdf 是加密的，可以通过这个包进行有效的解密
@@ -84,16 +93,15 @@
                 if page_layout.pageid in self.pages:
                     yield self.loop_pages(page_layout)
         else:
             # 解析所有页面
             for page_layout in page_layouts:
                 yield self.loop_pages(page_layout)
 
-        end_extract_time = time.perf_counter() - start_extract_time
-        logger.warning(f'End extract pdf with cost time {str(end_extract_time * 1000)}')
+        logger.warning(f'End extract pdf with cost time {str((time.perf_counter() - start_extract_time) * 1000)}')
 
     def loop_pages(self, page_layout):
         """处理单独一页的数据
         1. 通过 pdfplumber 提取表格信息
         2. 通过 pdfminer 提取文本 block 信息
         """
         logger.info(f"Start inspect page {str(page_layout.pageid)}...")
@@ -322,11 +330,7 @@
 
     def _get_html_table_format(self, table):
         tb = PrettyTable()
         for row in table:
             tb.add_row(row)
 
         return tb.get_html_string(header=False)
-
-
-if __name__ == '__main__':
-    pass
```

### Comparing `orbitkit-0.4.1/orbitkit/util/util_aws.py` & `orbitkit-0.4.2/orbitkit/util/util_aws.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.4.1/orbitkit/util/util_date.py` & `orbitkit-0.4.2/orbitkit/util/util_date.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.4.1/orbitkit/util/util_type_mapping.py` & `orbitkit-0.4.2/orbitkit/util/util_type_mapping.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.4.1/orbitkit.egg-info/PKG-INFO` & `orbitkit-0.4.2/orbitkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbitkit
-Version: 0.4.1
+Version: 0.4.2
 Summary: This project is only for Orbit Tech internal use.
 Home-page: https://github.com/clown-0726/orbitkit
 Author: Lilu Cao
 Author-email: lilu.cao@qq.com
 Maintainer: Lilu Cao
 Maintainer-email: lilu.cao@qq.com
 License: MIT License
```

### Comparing `orbitkit-0.4.1/orbitkit.egg-info/SOURCES.txt` & `orbitkit-0.4.2/orbitkit.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -11,16 +11,19 @@
 orbitkit.egg-info/requires.txt
 orbitkit.egg-info/top_level.txt
 orbitkit/id_srv/__init__.py
 orbitkit/id_srv/id_gen.py
 orbitkit/lark_send/__init__.py
 orbitkit/lark_send/lark.py
 orbitkit/pdf_extractor/__init__.py
+orbitkit/pdf_extractor/exceptions.py
 orbitkit/pdf_extractor/pdf_block_extractor_base.py
 orbitkit/pdf_extractor/pdf_block_extractor_v1.py
 orbitkit/pdf_extractor/pdf_block_extractor_v2.py
+orbitkit/pdf_extractor/pdf_extractor_azure.py
+orbitkit/pdf_extractor/pdf_extractor_orbit.py
 orbitkit/util/__init__.py
 orbitkit/util/common.py
 orbitkit/util/util_aws.py
 orbitkit/util/util_date.py
 orbitkit/util/util_str.py
 orbitkit/util/util_type_mapping.py
```

### Comparing `orbitkit-0.4.1/setup.py` & `orbitkit-0.4.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,12 +35,11 @@
         'Topic :: Software Development :: Libraries'
     ],
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         "boto3 >= 1.16.0",
         "requests >= 2.12.1",
-        "pdfplumber >= 0.9.0",
-        "pycryptodome >= 3.11.0",
         "prettytable >= 3.0.0",
+        "pytz >= 2022.1",
     ]
 )
```

