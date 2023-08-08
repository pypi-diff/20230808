# Comparing `tmp/gs_engine-0.24.0a20230807-py2.py3-none-macosx_11_0_x86_64.whl.zip` & `tmp/gs_engine-0.24.0a20230808-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 12193 bytes, number of entries: 9
--rw-r--r--  2.0 unx      694 b- defN 23-Aug-07 19:08 graphscope_runtime/__init__.py
--rw-rw-r--  2.0 unx      840 b- defN 23-Aug-07 21:17 gs_engine-0.24.0a20230807.dist-info/RECORD
--rw-r--r--  2.0 unx      140 b- defN 23-Aug-07 21:01 gs_engine-0.24.0a20230807.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-Aug-07 21:01 gs_engine-0.24.0a20230807.dist-info/top_level.txt
--rw-r--r--  2.0 unx    22193 b- defN 23-Aug-07 21:01 gs_engine-0.24.0a20230807.dist-info/METADATA
--rw-r--r--  2.0 unx     1573 b- defN 23-Aug-07 19:08 graphscope.runtime/conf/log4j2.xml
--rw-r--r--  2.0 unx      398 b- defN 23-Aug-07 19:08 graphscope.runtime/conf/executor.vineyard.properties
--rw-r--r--  2.0 unx      549 b- defN 23-Aug-07 19:08 graphscope.runtime/conf/frontend.vineyard.properties
--rw-r--r--  2.0 unx      204 b- defN 23-Aug-07 19:08 graphscope.runtime/conf/log4rs.yml
-9 files, 26610 bytes uncompressed, 10731 bytes compressed:  59.7%
+Zip file size: 12174 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      398 b- defN 23-Aug-08 19:01 graphscope.runtime/conf/executor.vineyard.properties
+-rw-r--r--  2.0 unx      549 b- defN 23-Aug-08 19:01 graphscope.runtime/conf/frontend.vineyard.properties
+-rw-r--r--  2.0 unx     1573 b- defN 23-Aug-08 19:01 graphscope.runtime/conf/log4j2.xml
+-rw-r--r--  2.0 unx      204 b- defN 23-Aug-08 19:01 graphscope.runtime/conf/log4rs.yml
+-rw-r--r--  2.0 unx      694 b- defN 23-Aug-08 19:01 graphscope_runtime/__init__.py
+-rw-r--r--  2.0 unx    22193 b- defN 23-Aug-08 20:32 gs_engine-0.24.0a20230808.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Aug-08 20:32 gs_engine-0.24.0a20230808.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-Aug-08 20:32 gs_engine-0.24.0a20230808.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      831 b- defN 23-Aug-08 20:32 gs_engine-0.24.0a20230808.dist-info/RECORD
+9 files, 26571 bytes uncompressed, 10712 bytes compressed:  59.7%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
-Filename: graphscope_runtime/__init__.py
+Filename: graphscope.runtime/conf/executor.vineyard.properties
 Comment: 
 
-Filename: gs_engine-0.24.0a20230807.dist-info/RECORD
+Filename: graphscope.runtime/conf/frontend.vineyard.properties
 Comment: 
 
-Filename: gs_engine-0.24.0a20230807.dist-info/WHEEL
+Filename: graphscope.runtime/conf/log4j2.xml
 Comment: 
 
-Filename: gs_engine-0.24.0a20230807.dist-info/top_level.txt
+Filename: graphscope.runtime/conf/log4rs.yml
 Comment: 
 
-Filename: gs_engine-0.24.0a20230807.dist-info/METADATA
+Filename: graphscope_runtime/__init__.py
 Comment: 
 
-Filename: graphscope.runtime/conf/log4j2.xml
+Filename: gs_engine-0.24.0a20230808.dist-info/METADATA
 Comment: 
 
-Filename: graphscope.runtime/conf/executor.vineyard.properties
+Filename: gs_engine-0.24.0a20230808.dist-info/WHEEL
 Comment: 
 
-Filename: graphscope.runtime/conf/frontend.vineyard.properties
+Filename: gs_engine-0.24.0a20230808.dist-info/top_level.txt
 Comment: 
 
-Filename: graphscope.runtime/conf/log4rs.yml
+Filename: gs_engine-0.24.0a20230808.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `gs_engine-0.24.0a20230807.dist-info/RECORD` & `gs_engine-0.24.0a20230808.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-graphscope_runtime/__init__.py,sha256=w_Me0NHI5zy8GitMCD7mzOi0Qz7ZfeE2zUI5wGfZIyM,694
-gs_engine-0.24.0a20230807.dist-info/RECORD,,
-gs_engine-0.24.0a20230807.dist-info/WHEEL,sha256=Us10RuDuoYRxbrGPvcONEZ8KDv19qxnuqzd5oEo2fQY,140
-gs_engine-0.24.0a20230807.dist-info/top_level.txt,sha256=8OYX8275H-myeSCvZ0ZHMFaQrPlxRlQfm6Z2pK0SbFw,19
-gs_engine-0.24.0a20230807.dist-info/METADATA,sha256=GjIx6gvxQEr8Qcp9mReyoFergHL0-qYNqL9rOyCOwp0,22193
-graphscope.runtime/conf/log4j2.xml,sha256=JiMUDFQ779aE33kOkah4-VlGQqMVW1_xlzWVZsvhHWQ,1573
-graphscope.runtime/conf/executor.vineyard.properties,sha256=FX6Og8G2x4VrMvdtT-XGjTsDGkY0iTWrLlNUg2aFX6o,398
-graphscope.runtime/conf/frontend.vineyard.properties,sha256=EaH9P5c8ZDA0YrjcVX_4OeASQXI7rF1yIxGO6lblr-c,549
-graphscope.runtime/conf/log4rs.yml,sha256=jFXF2AwsTarQhUr2vH4qD9-TJGdY2vVbvBtGYm-fotM,204
+graphscope.runtime/conf/executor.vineyard.properties,sha256=FX6Og8G2x4VrMvdtT-XGjTsDGkY0iTWrLlNUg2aFX6o,398
+graphscope.runtime/conf/frontend.vineyard.properties,sha256=EaH9P5c8ZDA0YrjcVX_4OeASQXI7rF1yIxGO6lblr-c,549
+graphscope.runtime/conf/log4j2.xml,sha256=JiMUDFQ779aE33kOkah4-VlGQqMVW1_xlzWVZsvhHWQ,1573
+graphscope.runtime/conf/log4rs.yml,sha256=jFXF2AwsTarQhUr2vH4qD9-TJGdY2vVbvBtGYm-fotM,204
+graphscope_runtime/__init__.py,sha256=w_Me0NHI5zy8GitMCD7mzOi0Qz7ZfeE2zUI5wGfZIyM,694
+gs_engine-0.24.0a20230808.dist-info/METADATA,sha256=kmQ32254UR16_IERDGFArdaxLq81NhsBYuta77JU8KQ,22193
+gs_engine-0.24.0a20230808.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+gs_engine-0.24.0a20230808.dist-info/top_level.txt,sha256=8OYX8275H-myeSCvZ0ZHMFaQrPlxRlQfm6Z2pK0SbFw,19
+gs_engine-0.24.0a20230808.dist-info/RECORD,,
```

## Comparing `gs_engine-0.24.0a20230807.dist-info/METADATA` & `gs_engine-0.24.0a20230808.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gs-engine
-Version: 0.24.0a20230807
+Version: 0.24.0a20230808
 Home-page: https://github.com/alibaba/GraphScope
 Author: GraphScope Team, Damo Academy
 Author-email: graphscope@alibaba-inc.com
 License: Apache License 2.0
 Keywords: GraphScope,Graph Computations
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

