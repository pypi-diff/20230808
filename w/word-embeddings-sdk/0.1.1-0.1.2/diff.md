# Comparing `tmp/word_embeddings_sdk-0.1.1-py3-none-any.whl.zip` & `tmp/word_embeddings_sdk-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,15 @@
-Zip file size: 5776 bytes, number of entries: 11
+Zip file size: 6451 bytes, number of entries: 13
 -rw-r--r--  2.0 unx       65 b- defN 23-Aug-08 07:24 word_embeddings_sdk/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Aug-08 07:24 word_embeddings_sdk/api/__init__.py
 -rw-r--r--  2.0 unx    10477 b- defN 23-Aug-08 07:24 word_embeddings_sdk/api/session.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Aug-08 07:24 word_embeddings_sdk/domain/__init__.py
 -rw-r--r--  2.0 unx       91 b- defN 23-Aug-08 07:24 word_embeddings_sdk/domain/exceptions.py
 -rw-r--r--  2.0 unx      138 b- defN 23-Aug-08 07:24 word_embeddings_sdk/domain/models.py
--rw-r--r--  2.0 unx     1064 b- defN 23-Aug-08 07:30 word_embeddings_sdk-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1383 b- defN 23-Aug-08 07:30 word_embeddings_sdk-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-08 07:30 word_embeddings_sdk-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-Aug-08 07:30 word_embeddings_sdk-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      992 b- defN 23-Aug-08 07:30 word_embeddings_sdk-0.1.1.dist-info/RECORD
-11 files, 14322 bytes uncompressed, 4052 bytes compressed:  71.7%
+-rw-r--r--  2.0 unx       65 b- defN 23-Aug-08 07:34 word_embeddings_sdk/utils/__init__.py
+-rw-r--r--  2.0 unx      673 b- defN 23-Aug-08 07:24 word_embeddings_sdk/utils/utils.py
+-rw-r--r--  2.0 unx     1064 b- defN 23-Aug-08 07:42 word_embeddings_sdk-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1373 b- defN 23-Aug-08 07:42 word_embeddings_sdk-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-08 07:42 word_embeddings_sdk-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-Aug-08 07:42 word_embeddings_sdk-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1174 b- defN 23-Aug-08 07:42 word_embeddings_sdk-0.1.2.dist-info/RECORD
+13 files, 15232 bytes uncompressed, 4433 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -12,23 +12,29 @@
 
 Filename: word_embeddings_sdk/domain/exceptions.py
 Comment: 
 
 Filename: word_embeddings_sdk/domain/models.py
 Comment: 
 
-Filename: word_embeddings_sdk-0.1.1.dist-info/LICENSE
+Filename: word_embeddings_sdk/utils/__init__.py
 Comment: 
 
-Filename: word_embeddings_sdk-0.1.1.dist-info/METADATA
+Filename: word_embeddings_sdk/utils/utils.py
 Comment: 
 
-Filename: word_embeddings_sdk-0.1.1.dist-info/WHEEL
+Filename: word_embeddings_sdk-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: word_embeddings_sdk-0.1.1.dist-info/top_level.txt
+Filename: word_embeddings_sdk-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: word_embeddings_sdk-0.1.1.dist-info/RECORD
+Filename: word_embeddings_sdk-0.1.2.dist-info/WHEEL
+Comment: 
+
+Filename: word_embeddings_sdk-0.1.2.dist-info/top_level.txt
+Comment: 
+
+Filename: word_embeddings_sdk-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `word_embeddings_sdk-0.1.1.dist-info/LICENSE` & `word_embeddings_sdk-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `word_embeddings_sdk-0.1.1.dist-info/METADATA` & `word_embeddings_sdk-0.1.2.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: word-embeddings-sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python sdk to interface with the WordEmbeddings API
 Home-page: https://github.com/Width-ai/embeddings-sdk
-Download-URL: https://github.com/Width-ai/embeddings-sdk/archive/refs/tags/v0.1.1.tar.gz
+Download-URL: https://github.com/Width-ai/embeddings-sdk/archive/refs/tags/v0.1.2.tar.gz
 Author: Patrick Hennis
 Author-email: patrick@width.ai
 License: MIT
 Keywords: Embeddings,SDK,WordEmbeddings,WordEmbeddings.Ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests (==2.31.0)
-Requires-Dist: pydantic (==2.1.1)
+Requires-Dist: pydantic
 
 # WordEmbeddings SDK
 Python sdk to interface with the Word Embeddings API
 
 
 ## Example Usage
 ```python
```

## Comparing `word_embeddings_sdk-0.1.1.dist-info/RECORD` & `word_embeddings_sdk-0.1.2.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 word_embeddings_sdk/__init__.py,sha256=QJ0ixtacUVaQWMA0YLgtKbr8s5awLiRQaQ8Mv5yZWLI,65
 word_embeddings_sdk/api/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 word_embeddings_sdk/api/session.py,sha256=2f4fsqt9e3opMzBIKiXpZjgh1I-SmGD9iNIdSIWxpZc,10477
 word_embeddings_sdk/domain/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 word_embeddings_sdk/domain/exceptions.py,sha256=JjC-S9NHF0Rx0O0PSUHp4YTyW-wvjIuak9EiPt6LtaA,91
 word_embeddings_sdk/domain/models.py,sha256=1k3PPWBWGbs8z_2MOx6jGE98yeZShQnyCejkW-_158c,138
-word_embeddings_sdk-0.1.1.dist-info/LICENSE,sha256=sse_Ov29zMc9othQILVxu2BIBiydJyd-ppGKG88QwlQ,1064
-word_embeddings_sdk-0.1.1.dist-info/METADATA,sha256=SnYr-7ANN8hMvrZZAHQGmClY6ajBgZpZpjuHIsqB8Cc,1383
-word_embeddings_sdk-0.1.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-word_embeddings_sdk-0.1.1.dist-info/top_level.txt,sha256=93s_VZwYcsTg6DB3GtlNIW9Ioz8N8K7xKPZRbybaKtk,20
-word_embeddings_sdk-0.1.1.dist-info/RECORD,,
+word_embeddings_sdk/utils/__init__.py,sha256=QJ0ixtacUVaQWMA0YLgtKbr8s5awLiRQaQ8Mv5yZWLI,65
+word_embeddings_sdk/utils/utils.py,sha256=M5Sv_B7-DE4BpdHAaf4wNK1_RC16EqQhh4tkD5R2doY,673
+word_embeddings_sdk-0.1.2.dist-info/LICENSE,sha256=sse_Ov29zMc9othQILVxu2BIBiydJyd-ppGKG88QwlQ,1064
+word_embeddings_sdk-0.1.2.dist-info/METADATA,sha256=QB4tXpP8ALKQBPSUobHxhEZ1-vTqKr0k8ZO8whxqBbo,1373
+word_embeddings_sdk-0.1.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+word_embeddings_sdk-0.1.2.dist-info/top_level.txt,sha256=93s_VZwYcsTg6DB3GtlNIW9Ioz8N8K7xKPZRbybaKtk,20
+word_embeddings_sdk-0.1.2.dist-info/RECORD,,
```

