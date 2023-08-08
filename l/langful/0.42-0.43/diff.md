# Comparing `tmp/langful-0.42-py3-none-any.whl.zip` & `tmp/langful-0.43-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5771 bytes, number of entries: 8
+Zip file size: 5831 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat      166 b- defN 23-Jul-30 07:47 langful/__init__.py
 -rw-rw-rw-  2.0 fat      382 b- defN 23-Jul-30 12:15 langful/errors.py
--rw-rw-rw-  2.0 fat     8961 b- defN 23-Aug-04 11:05 langful/lang.py
--rw-rw-rw-  2.0 fat     1066 b- defN 23-Aug-04 11:07 langful-0.42.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2984 b- defN 23-Aug-04 11:07 langful-0.42.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-04 11:07 langful-0.42.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Aug-04 11:07 langful-0.42.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      600 b- defN 23-Aug-04 11:07 langful-0.42.dist-info/RECORD
-8 files, 14259 bytes uncompressed, 4731 bytes compressed:  66.8%
+-rw-rw-rw-  2.0 fat     9281 b- defN 23-Aug-08 15:01 langful/lang.py
+-rw-rw-rw-  2.0 fat     1066 b- defN 23-Aug-08 15:25 langful-0.43.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3004 b- defN 23-Aug-08 15:25 langful-0.43.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-08 15:25 langful-0.43.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Aug-08 15:25 langful-0.43.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      600 b- defN 23-Aug-08 15:25 langful-0.43.dist-info/RECORD
+8 files, 14599 bytes uncompressed, 4791 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: langful/errors.py
 Comment: 
 
 Filename: langful/lang.py
 Comment: 
 
-Filename: langful-0.42.dist-info/LICENSE
+Filename: langful-0.43.dist-info/LICENSE
 Comment: 
 
-Filename: langful-0.42.dist-info/METADATA
+Filename: langful-0.43.dist-info/METADATA
 Comment: 
 
-Filename: langful-0.42.dist-info/WHEEL
+Filename: langful-0.43.dist-info/WHEEL
 Comment: 
 
-Filename: langful-0.42.dist-info/top_level.txt
+Filename: langful-0.43.dist-info/top_level.txt
 Comment: 
 
-Filename: langful-0.42.dist-info/RECORD
+Filename: langful-0.43.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langful/lang.py

```diff
@@ -4,15 +4,15 @@
 
 from . import errors
 
 import json
 import os
 
 __all__ = [ "__version__" , "to_json" , "to_lang" , "getdefaultlocale" , "lang" ]
-__version__ = "0.42"
+__version__ = "0.43"
 
 def to_json( text : str ) -> dict[ str , str ] :
     from re import split
     ret = {}
     for line in text.split( "\n" ) :
         try :
             ret.update( dict( [ split( "\\s=\\s" , line.split( "#" )[ 0 ] , 1 ) ] ) )
@@ -86,32 +86,32 @@
     def __exit__( self , *args ) -> None :
         self.save() if all( item is None for item in args ) else ...
 
     def __bool__( self ) -> bool :
         return self.locale_system in self.languages
 
     def __repr__( self ) -> str :
-        return str( self.languages )
+        return json.dumps( self.languages )
 
     def __call__( self ) -> None :
         self.init()
 
     def __str__( self ) -> str :
         return json.dumps( self.languages , indent = 4 , ensure_ascii = False , separators = self.configs[ "separators" ] )
 
     def __len__( self ) -> int :
-        return len( self.language )
+        return len( self.languages )
 
     def __init__( self , path : str | dict = "lang" , locale_default : str = "en_us" , json_first : bool = True ) -> None :
         """
         path: lang files dir, if use dict to set that to a dictionary or False
         locale_default: default locale
         load: is load json file first
         """
-        self.configs = { "separators" : [ " ," , ": " ] , "replace" : "%" , "load" : json_first , "file" : False }
+        self.configs = { "separators" : [ " ," , ": " ] , "load" : json_first , "file" : False }
         self.locale_default = locale_default
         self.locale_use = None
         self.languages = {}
         self.path = path
         self.types = {}
         self.init()
 
@@ -184,23 +184,23 @@
         return locale if locale else self.locale
 
     def locale_set( self , locale : str = None  ) -> None :
         if locale and locale not in self.locales :
             raise errors.LocaleError( f"no such locale '{ locale }'" )
         self.locale_use = locale
 
-    def lang_get( self , locale : str ) -> dict[ str , str ] :
+    def lang_get( self , locale : str = None ) -> dict[ str , str ] :
         return self.languages[ self.locale_get( locale ) ]
 
-    def lang_set( self , locale : str , value : dict = {} , suffix : str = ".json" ) -> None :
+    def lang_set( self , locale : str = None , value : dict = {} , suffix : str = ".json" ) -> None :
         locale = self.locale_get( locale )
         self.languages[ locale ] = value
         self.types[ locale ] = suffix
 
-    def lang_remove( self , locale : str ) -> None :
+    def lang_remove( self , locale : str = None ) -> None :
         locale = self.locale_get( locale )
         del self.languages[ locale ]
         del self.types[ locale ]
 
     def lang_merge( self , to : str , locale : str = None , args : str | list[ str ] = [] ) -> None :
         self.lang_set( to , self.merge( locale , args ) )
 
@@ -225,21 +225,28 @@
                 with open( os.path.join( self.path , key + suffix ) , "w" , encoding = "utf-8" ) as file :
                     if suffix == ".json" :
                         json.dump( value , file , indent = 4 , separators = self.configs[ "separators" ] , ensure_ascii = False )
                     elif suffix == ".lang" :
                         file.write( to_lang( value ) )
         return self.languages
 
-    def replace( self , key : str = None , args : list[ str ] = None , locale : str = None ) -> str :
-        symbol = self.configs[ "replace" ]
+    def replace( self , key : str = None , args : list[ str ] | dict[ str , str ] = [] , locale : str = None ) -> str :
+        from re import findall
+        text = self.get( key , locale )
         index = 0
-        ret = ""
-        for text in self.get( key , locale ) :
-            if text == symbol :
-                if len( ret ) and ret[ -1 ] == "\\" :
-                    ret = ret[ : -1 ] + symbol
+        for texts in findall( "{[^{^}]*}" , text ) :
+            if isinstance( args , ( list , tuple ) ) :
+                if len( args ) :
+                    s = args[ index ]
+                    index += 1 if index < len( args ) - 1 else 0
                 else :
-                    ret += str( args[ index ] )
-                    index += index < len( args ) - 1
+                    continue
+            elif isinstance( args , dict ) :
+                item = texts[ 1 : -1 ].replace( " " , "" )
+                if item in args :
+                    s = args[ item ]
+                else :
+                    continue
             else :
-                ret += text
-        return ret
+                s = args
+            text = text.replace( texts , str( s ) , 1 )
+        return text
```

## Comparing `langful-0.42.dist-info/LICENSE` & `langful-0.43.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langful-0.42.dist-info/METADATA` & `langful-0.43.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: langful
-Version: 0.42
-Summary: Help to localization
+Version: 0.43
+Summary: provides internationalization for python
 Home-page: https://github.com/cueavy/langful
 Author: cueavyqwp
 Author-email: cueavyqwp@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >= 3.9
```

## Comparing `langful-0.42.dist-info/RECORD` & `langful-0.43.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 langful/__init__.py,sha256=BSJ-BT1Yr3Xz-SFnmZu7QvgV5pgg2WEqUO42oM3Py2w,166
 langful/errors.py,sha256=2Ag2tnAPSzozEIzye5U-mnyvSmvk5X8ZqB3kwLhGOIs,382
-langful/lang.py,sha256=vxWyvoqf2zMMscimKBNUlBm2_7nkLzSIc_fUvgHdr14,8961
-langful-0.42.dist-info/LICENSE,sha256=JrQca6fL66RGTmf-hkJU9UEX64JB0yE9gKNsOhpmZVE,1066
-langful-0.42.dist-info/METADATA,sha256=8K6zixJvXukIPEtxZr2d7nCSDqkL60FBjfofOg7oUXI,2984
-langful-0.42.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-langful-0.42.dist-info/top_level.txt,sha256=EkKV_WnIZfE3A6EhWwDIt2uwZhMVHWXTUueKJL6K15w,8
-langful-0.42.dist-info/RECORD,,
+langful/lang.py,sha256=T5fl9sqBUNu7lVTbR3rx_aU3a9Saz0rtA_6KdtKxtdc,9281
+langful-0.43.dist-info/LICENSE,sha256=JrQca6fL66RGTmf-hkJU9UEX64JB0yE9gKNsOhpmZVE,1066
+langful-0.43.dist-info/METADATA,sha256=i1zoteoxLaLjzh0Yy3YmbkQ-JBEBGvkxztAfLJdhc6Q,3004
+langful-0.43.dist-info/WHEEL,sha256=5sUXSg9e4bi7lTLOHcm6QEYwO5TIF1TNbTSVFVjcJcc,92
+langful-0.43.dist-info/top_level.txt,sha256=EkKV_WnIZfE3A6EhWwDIt2uwZhMVHWXTUueKJL6K15w,8
+langful-0.43.dist-info/RECORD,,
```

