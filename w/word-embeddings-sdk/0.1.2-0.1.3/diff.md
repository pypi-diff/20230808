# Comparing `tmp/word_embeddings_sdk-0.1.2-py3-none-any.whl.zip` & `tmp/word_embeddings_sdk-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 6451 bytes, number of entries: 13
+Zip file size: 6398 bytes, number of entries: 13
 -rw-r--r--  2.0 unx       65 b- defN 23-Aug-08 07:24 word_embeddings_sdk/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Aug-08 07:24 word_embeddings_sdk/api/__init__.py
 -rw-r--r--  2.0 unx    10477 b- defN 23-Aug-08 07:24 word_embeddings_sdk/api/session.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Aug-08 07:24 word_embeddings_sdk/domain/__init__.py
 -rw-r--r--  2.0 unx       91 b- defN 23-Aug-08 07:24 word_embeddings_sdk/domain/exceptions.py
 -rw-r--r--  2.0 unx      138 b- defN 23-Aug-08 07:24 word_embeddings_sdk/domain/models.py
--rw-r--r--  2.0 unx       65 b- defN 23-Aug-08 07:34 word_embeddings_sdk/utils/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-08 07:45 word_embeddings_sdk/utils/__init__.py
 -rw-r--r--  2.0 unx      673 b- defN 23-Aug-08 07:24 word_embeddings_sdk/utils/utils.py
--rw-r--r--  2.0 unx     1064 b- defN 23-Aug-08 07:42 word_embeddings_sdk-0.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1373 b- defN 23-Aug-08 07:42 word_embeddings_sdk-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-08 07:42 word_embeddings_sdk-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-Aug-08 07:42 word_embeddings_sdk-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1174 b- defN 23-Aug-08 07:42 word_embeddings_sdk-0.1.2.dist-info/RECORD
-13 files, 15232 bytes uncompressed, 4433 bytes compressed:  70.9%
+-rw-r--r--  2.0 unx     1064 b- defN 23-Aug-08 07:48 word_embeddings_sdk-0.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1373 b- defN 23-Aug-08 07:48 word_embeddings_sdk-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-08 07:48 word_embeddings_sdk-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-Aug-08 07:48 word_embeddings_sdk-0.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1173 b- defN 23-Aug-08 07:48 word_embeddings_sdk-0.1.3.dist-info/RECORD
+13 files, 15166 bytes uncompressed, 4380 bytes compressed:  71.1%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: word_embeddings_sdk/utils/__init__.py
 Comment: 
 
 Filename: word_embeddings_sdk/utils/utils.py
 Comment: 
 
-Filename: word_embeddings_sdk-0.1.2.dist-info/LICENSE
+Filename: word_embeddings_sdk-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: word_embeddings_sdk-0.1.2.dist-info/METADATA
+Filename: word_embeddings_sdk-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: word_embeddings_sdk-0.1.2.dist-info/WHEEL
+Filename: word_embeddings_sdk-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: word_embeddings_sdk-0.1.2.dist-info/top_level.txt
+Filename: word_embeddings_sdk-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: word_embeddings_sdk-0.1.2.dist-info/RECORD
+Filename: word_embeddings_sdk-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## word_embeddings_sdk/utils/__init__.py

```diff
@@ -1,5 +0,0 @@
-00000000: 6672 6f6d 2077 6f72 645f 656d 6265 6464  from word_embedd
-00000010: 696e 6773 5f73 646b 2e61 7069 2e73 6573  ings_sdk.api.ses
-00000020: 7369 6f6e 2069 6d70 6f72 7420 576f 7264  sion import Word
-00000030: 456d 6265 6464 696e 6773 5365 7373 696f  EmbeddingsSessio
-00000040: 6e                                       n
```

## Comparing `word_embeddings_sdk-0.1.2.dist-info/LICENSE` & `word_embeddings_sdk-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `word_embeddings_sdk-0.1.2.dist-info/METADATA` & `word_embeddings_sdk-0.1.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: word-embeddings-sdk
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python sdk to interface with the WordEmbeddings API
 Home-page: https://github.com/Width-ai/embeddings-sdk
-Download-URL: https://github.com/Width-ai/embeddings-sdk/archive/refs/tags/v0.1.2.tar.gz
+Download-URL: https://github.com/Width-ai/embeddings-sdk/archive/refs/tags/v0.1.3.tar.gz
 Author: Patrick Hennis
 Author-email: patrick@width.ai
 License: MIT
 Keywords: Embeddings,SDK,WordEmbeddings,WordEmbeddings.Ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

## Comparing `word_embeddings_sdk-0.1.2.dist-info/RECORD` & `word_embeddings_sdk-0.1.3.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 word_embeddings_sdk/__init__.py,sha256=QJ0ixtacUVaQWMA0YLgtKbr8s5awLiRQaQ8Mv5yZWLI,65
 word_embeddings_sdk/api/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 word_embeddings_sdk/api/session.py,sha256=2f4fsqt9e3opMzBIKiXpZjgh1I-SmGD9iNIdSIWxpZc,10477
 word_embeddings_sdk/domain/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 word_embeddings_sdk/domain/exceptions.py,sha256=JjC-S9NHF0Rx0O0PSUHp4YTyW-wvjIuak9EiPt6LtaA,91
 word_embeddings_sdk/domain/models.py,sha256=1k3PPWBWGbs8z_2MOx6jGE98yeZShQnyCejkW-_158c,138
-word_embeddings_sdk/utils/__init__.py,sha256=QJ0ixtacUVaQWMA0YLgtKbr8s5awLiRQaQ8Mv5yZWLI,65
+word_embeddings_sdk/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 word_embeddings_sdk/utils/utils.py,sha256=M5Sv_B7-DE4BpdHAaf4wNK1_RC16EqQhh4tkD5R2doY,673
-word_embeddings_sdk-0.1.2.dist-info/LICENSE,sha256=sse_Ov29zMc9othQILVxu2BIBiydJyd-ppGKG88QwlQ,1064
-word_embeddings_sdk-0.1.2.dist-info/METADATA,sha256=QB4tXpP8ALKQBPSUobHxhEZ1-vTqKr0k8ZO8whxqBbo,1373
-word_embeddings_sdk-0.1.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-word_embeddings_sdk-0.1.2.dist-info/top_level.txt,sha256=93s_VZwYcsTg6DB3GtlNIW9Ioz8N8K7xKPZRbybaKtk,20
-word_embeddings_sdk-0.1.2.dist-info/RECORD,,
+word_embeddings_sdk-0.1.3.dist-info/LICENSE,sha256=sse_Ov29zMc9othQILVxu2BIBiydJyd-ppGKG88QwlQ,1064
+word_embeddings_sdk-0.1.3.dist-info/METADATA,sha256=pZoj63OCsJjUXHpekowABAwea0JE0-H_t68kY4WPKTI,1373
+word_embeddings_sdk-0.1.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+word_embeddings_sdk-0.1.3.dist-info/top_level.txt,sha256=93s_VZwYcsTg6DB3GtlNIW9Ioz8N8K7xKPZRbybaKtk,20
+word_embeddings_sdk-0.1.3.dist-info/RECORD,,
```

