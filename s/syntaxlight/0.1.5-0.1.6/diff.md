# Comparing `tmp/syntaxlight-0.1.5.tar.gz` & `tmp/syntaxlight-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntaxlight-0.1.5.tar", max compression
+gzip compressed data, was "syntaxlight-0.1.6.tar", max compression
```

## Comparing `syntaxlight-0.1.5.tar` & `syntaxlight-0.1.6.tar`

### file list

```diff
@@ -1,50 +1,51 @@
--rw-r--r--   0        0        0     1064 2023-06-08 14:13:12.759574 syntaxlight-0.1.5/LICENSE
--rw-r--r--   0        0        0      463 2023-08-07 13:45:37.697727 syntaxlight-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2258 2023-07-30 13:40:10.383897 syntaxlight-0.1.5/README.md
--rw-r--r--   0        0        0      257 2023-08-05 06:18:14.085640 syntaxlight-0.1.5/syntaxlight/__init__.py
--rw-r--r--   0        0        0    15445 2023-08-02 07:08:27.516374 syntaxlight-0.1.5/syntaxlight/ast.py
--rw-r--r--   0        0        0     2244 2023-08-05 14:13:35.618950 syntaxlight-0.1.5/syntaxlight/css/all.css
--rw-r--r--   0        0        0      535 2023-08-01 01:05:24.164690 syntaxlight-0.1.5/syntaxlight/css/asm.css
--rw-r--r--   0        0        0      666 2023-08-01 01:05:24.175123 syntaxlight-0.1.5/syntaxlight/css/bnf.css
--rw-r--r--   0        0        0     2210 2023-08-01 01:05:24.173124 syntaxlight-0.1.5/syntaxlight/css/c.css
--rw-r--r--   0        0        0      627 2023-08-01 01:05:24.172126 syntaxlight-0.1.5/syntaxlight/css/css.css
--rw-r--r--   0        0        0    18397 2023-06-15 07:10:53.753178 syntaxlight-0.1.5/syntaxlight/css/index.css
--rw-r--r--   0        0        0      531 2023-08-01 01:05:24.171126 syntaxlight-0.1.5/syntaxlight/css/json.css
--rw-r--r--   0        0        0     1106 2023-08-01 01:05:24.170124 syntaxlight-0.1.5/syntaxlight/css/lua.css
--rw-r--r--   0        0        0      953 2023-08-02 09:02:28.094967 syntaxlight-0.1.5/syntaxlight/css/makefile.css
--rw-r--r--   0        0        0      878 2023-08-05 14:06:43.880293 syntaxlight-0.1.5/syntaxlight/css/shell.css
--rw-r--r--   0        0        0     3068 2023-08-07 13:38:06.334941 syntaxlight-0.1.5/syntaxlight/css/themes.json
--rw-r--r--   0        0        0      558 2023-08-01 01:05:24.166692 syntaxlight-0.1.5/syntaxlight/css/toml.css
--rw-r--r--   0        0        0      497 2023-08-01 01:05:24.165690 syntaxlight-0.1.5/syntaxlight/css/xml.css
--rw-r--r--   0        0        0     2478 2023-07-30 12:33:41.489986 syntaxlight-0.1.5/syntaxlight/error.py
--rw-r--r--   0        0        0     1947 2023-07-29 15:01:42.303917 syntaxlight-0.1.5/syntaxlight/example.py
--rw-r--r--   0        0        0     1926 2023-07-30 02:57:51.649503 syntaxlight-0.1.5/syntaxlight/export.py
--rw-r--r--   0        0        0     2875 2023-07-30 12:21:15.272257 syntaxlight-0.1.5/syntaxlight/gdt.py
--rw-r--r--   0        0        0     2189 2023-08-01 09:07:20.794987 syntaxlight-0.1.5/syntaxlight/language.py
--rw-r--r--   0        0        0      579 2023-08-05 06:18:01.794963 syntaxlight-0.1.5/syntaxlight/lexers/__init__.py
--rw-r--r--   0        0        0     2645 2023-07-31 03:00:16.388119 syntaxlight-0.1.5/syntaxlight/lexers/asm_lexer.py
--rw-r--r--   0        0        0     1921 2023-07-26 05:57:52.779798 syntaxlight-0.1.5/syntaxlight/lexers/bnf_lexer.py
--rw-r--r--   0        0        0    12853 2023-07-31 01:57:07.230431 syntaxlight-0.1.5/syntaxlight/lexers/c_lexer.py
--rw-r--r--   0        0        0     3837 2023-07-31 03:00:49.403592 syntaxlight-0.1.5/syntaxlight/lexers/css_lexer.py
--rw-r--r--   0        0        0     1995 2023-07-26 05:58:05.904375 syntaxlight-0.1.5/syntaxlight/lexers/json_lexer.py
--rw-r--r--   0        0        0    24439 2023-08-05 06:20:18.443117 syntaxlight-0.1.5/syntaxlight/lexers/lexer.py
--rw-r--r--   0        0        0     8161 2023-07-31 02:35:08.122706 syntaxlight-0.1.5/syntaxlight/lexers/lua_lexer.py
--rw-r--r--   0        0        0     3407 2023-08-02 08:39:01.519231 syntaxlight-0.1.5/syntaxlight/lexers/makefile_lexer.py
--rw-r--r--   0        0        0     4485 2023-08-07 13:41:15.732684 syntaxlight-0.1.5/syntaxlight/lexers/shell_lexer.py
--rw-r--r--   0        0        0     3006 2023-07-30 13:42:04.120083 syntaxlight-0.1.5/syntaxlight/lexers/toml_lexer.py
--rw-r--r--   0        0        0     4576 2023-07-26 05:58:25.950097 syntaxlight-0.1.5/syntaxlight/lexers/xml_lexer.py
--rw-r--r--   0        0        0      405 2023-08-01 12:25:00.965587 syntaxlight-0.1.5/syntaxlight/parsers/__init__.py
--rw-r--r--   0        0        0     1099 2023-07-31 01:38:18.589025 syntaxlight-0.1.5/syntaxlight/parsers/asm_parser.py
--rw-r--r--   0        0        0     6950 2023-07-24 08:35:40.217597 syntaxlight-0.1.5/syntaxlight/parsers/bnf_parser.py
--rw-r--r--   0        0        0   106329 2023-08-05 13:55:32.850499 syntaxlight-0.1.5/syntaxlight/parsers/c_parser.py
--rw-r--r--   0        0        0     1719 2023-07-31 03:13:51.887478 syntaxlight-0.1.5/syntaxlight/parsers/css_parser.py
--rw-r--r--   0        0        0     5758 2023-07-24 01:35:24.219886 syntaxlight-0.1.5/syntaxlight/parsers/json_parser.py
--rw-r--r--   0        0        0    35078 2023-07-31 02:33:22.161465 syntaxlight-0.1.5/syntaxlight/parsers/lua_parser.py
--rw-r--r--   0        0        0     3283 2023-08-02 09:02:17.026646 syntaxlight-0.1.5/syntaxlight/parsers/makefile_parser.py
--rw-r--r--   0        0        0    13274 2023-08-07 13:44:41.858038 syntaxlight-0.1.5/syntaxlight/parsers/parser.py
--rw-r--r--   0        0        0     5269 2023-08-07 13:41:57.292919 syntaxlight-0.1.5/syntaxlight/parsers/shell_parser.py
--rw-r--r--   0        0        0    11810 2023-07-24 01:35:24.522506 syntaxlight-0.1.5/syntaxlight/parsers/toml_parser.py
--rw-r--r--   0        0        0     6531 2023-07-24 01:35:24.720887 syntaxlight-0.1.5/syntaxlight/parsers/xml_parser.py
--rw-r--r--   0        0        0     2335 2023-08-03 06:34:30.224044 syntaxlight-0.1.5/syntaxlight/syntax_parse.py
--rw-r--r--   0        0        0      349 2023-07-25 01:26:08.919200 syntaxlight-0.1.5/syntaxlight/template.html
--rw-r--r--   0        0        0     3049 1970-01-01 00:00:00.000000 syntaxlight-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-08 14:13:12.759574 syntaxlight-0.1.6/LICENSE
+-rw-r--r--   0        0        0      463 2023-08-08 02:11:31.462683 syntaxlight-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2258 2023-07-30 13:40:10.383897 syntaxlight-0.1.6/README.md
+-rw-r--r--   0        0        0      257 2023-08-05 06:18:14.085640 syntaxlight-0.1.6/syntaxlight/__init__.py
+-rw-r--r--   0        0        0    15445 2023-08-02 07:08:27.516374 syntaxlight-0.1.6/syntaxlight/ast.py
+-rw-r--r--   0        0        0     2244 2023-08-05 14:13:35.618950 syntaxlight-0.1.6/syntaxlight/css/all.css
+-rw-r--r--   0        0        0      666 2023-08-01 01:05:24.175123 syntaxlight-0.1.6/syntaxlight/css/bnf.css
+-rw-r--r--   0        0        0     2210 2023-08-01 01:05:24.173124 syntaxlight-0.1.6/syntaxlight/css/c.css
+-rw-r--r--   0        0        0      627 2023-08-01 01:05:24.172126 syntaxlight-0.1.6/syntaxlight/css/css.css
+-rw-r--r--   0        0        0    18397 2023-06-15 07:10:53.753178 syntaxlight-0.1.6/syntaxlight/css/index.css
+-rw-r--r--   0        0        0      531 2023-08-01 01:05:24.171126 syntaxlight-0.1.6/syntaxlight/css/json.css
+-rw-r--r--   0        0        0     1106 2023-08-01 01:05:24.170124 syntaxlight-0.1.6/syntaxlight/css/lua.css
+-rw-r--r--   0        0        0      953 2023-08-02 09:02:28.094967 syntaxlight-0.1.6/syntaxlight/css/makefile.css
+-rw-r--r--   0        0        0      772 2023-08-08 02:05:55.970782 syntaxlight-0.1.6/syntaxlight/css/riscvasm.css
+-rw-r--r--   0        0        0      878 2023-08-05 14:06:43.880293 syntaxlight-0.1.6/syntaxlight/css/shell.css
+-rw-r--r--   0        0        0     3068 2023-08-08 01:56:22.718774 syntaxlight-0.1.6/syntaxlight/css/themes.json
+-rw-r--r--   0        0        0      558 2023-08-01 01:05:24.166692 syntaxlight-0.1.6/syntaxlight/css/toml.css
+-rw-r--r--   0        0        0      625 2023-08-08 02:07:40.488130 syntaxlight-0.1.6/syntaxlight/css/x86asm.css
+-rw-r--r--   0        0        0      497 2023-08-01 01:05:24.165690 syntaxlight-0.1.6/syntaxlight/css/xml.css
+-rw-r--r--   0        0        0     2478 2023-07-30 12:33:41.489986 syntaxlight-0.1.6/syntaxlight/error.py
+-rw-r--r--   0        0        0     1941 2023-08-08 02:05:48.378946 syntaxlight-0.1.6/syntaxlight/example.py
+-rw-r--r--   0        0        0     1926 2023-08-08 01:51:12.605756 syntaxlight-0.1.6/syntaxlight/export.py
+-rw-r--r--   0        0        0     2875 2023-07-30 12:21:15.272257 syntaxlight-0.1.6/syntaxlight/gdt.py
+-rw-r--r--   0        0        0     2270 2023-08-08 02:03:57.826551 syntaxlight-0.1.6/syntaxlight/language.py
+-rw-r--r--   0        0        0      655 2023-08-08 02:00:04.293166 syntaxlight-0.1.6/syntaxlight/lexers/__init__.py
+-rw-r--r--   0        0        0     5283 2023-08-08 02:00:04.275649 syntaxlight-0.1.6/syntaxlight/lexers/asm_lexer.py
+-rw-r--r--   0        0        0     1921 2023-07-26 05:57:52.779798 syntaxlight-0.1.6/syntaxlight/lexers/bnf_lexer.py
+-rw-r--r--   0        0        0    12853 2023-07-31 01:57:07.230431 syntaxlight-0.1.6/syntaxlight/lexers/c_lexer.py
+-rw-r--r--   0        0        0     3837 2023-07-31 03:00:49.403592 syntaxlight-0.1.6/syntaxlight/lexers/css_lexer.py
+-rw-r--r--   0        0        0     1995 2023-07-26 05:58:05.904375 syntaxlight-0.1.6/syntaxlight/lexers/json_lexer.py
+-rw-r--r--   0        0        0    24439 2023-08-05 06:20:18.443117 syntaxlight-0.1.6/syntaxlight/lexers/lexer.py
+-rw-r--r--   0        0        0     8161 2023-07-31 02:35:08.122706 syntaxlight-0.1.6/syntaxlight/lexers/lua_lexer.py
+-rw-r--r--   0        0        0     3407 2023-08-02 08:39:01.519231 syntaxlight-0.1.6/syntaxlight/lexers/makefile_lexer.py
+-rw-r--r--   0        0        0     4485 2023-08-07 13:41:15.732684 syntaxlight-0.1.6/syntaxlight/lexers/shell_lexer.py
+-rw-r--r--   0        0        0     3006 2023-07-30 13:42:04.120083 syntaxlight-0.1.6/syntaxlight/lexers/toml_lexer.py
+-rw-r--r--   0        0        0     4576 2023-07-26 05:58:25.950097 syntaxlight-0.1.6/syntaxlight/lexers/xml_lexer.py
+-rw-r--r--   0        0        0      432 2023-08-08 01:59:24.336858 syntaxlight-0.1.6/syntaxlight/parsers/__init__.py
+-rw-r--r--   0        0        0     4484 2023-08-08 02:09:13.417284 syntaxlight-0.1.6/syntaxlight/parsers/asm_parser.py
+-rw-r--r--   0        0        0     6950 2023-07-24 08:35:40.217597 syntaxlight-0.1.6/syntaxlight/parsers/bnf_parser.py
+-rw-r--r--   0        0        0   106329 2023-08-05 13:55:32.850499 syntaxlight-0.1.6/syntaxlight/parsers/c_parser.py
+-rw-r--r--   0        0        0     1719 2023-07-31 03:13:51.887478 syntaxlight-0.1.6/syntaxlight/parsers/css_parser.py
+-rw-r--r--   0        0        0     5758 2023-07-24 01:35:24.219886 syntaxlight-0.1.6/syntaxlight/parsers/json_parser.py
+-rw-r--r--   0        0        0    35078 2023-07-31 02:33:22.161465 syntaxlight-0.1.6/syntaxlight/parsers/lua_parser.py
+-rw-r--r--   0        0        0     3283 2023-08-02 09:02:17.026646 syntaxlight-0.1.6/syntaxlight/parsers/makefile_parser.py
+-rw-r--r--   0        0        0    13274 2023-08-07 13:44:41.858038 syntaxlight-0.1.6/syntaxlight/parsers/parser.py
+-rw-r--r--   0        0        0     5269 2023-08-07 13:41:57.292919 syntaxlight-0.1.6/syntaxlight/parsers/shell_parser.py
+-rw-r--r--   0        0        0    11810 2023-07-24 01:35:24.522506 syntaxlight-0.1.6/syntaxlight/parsers/toml_parser.py
+-rw-r--r--   0        0        0     6531 2023-07-24 01:35:24.720887 syntaxlight-0.1.6/syntaxlight/parsers/xml_parser.py
+-rw-r--r--   0        0        0     2335 2023-08-03 06:34:30.224044 syntaxlight-0.1.6/syntaxlight/syntax_parse.py
+-rw-r--r--   0        0        0      349 2023-07-25 01:26:08.919200 syntaxlight-0.1.6/syntaxlight/template.html
+-rw-r--r--   0        0        0     3049 1970-01-01 00:00:00.000000 syntaxlight-0.1.6/PKG-INFO
```

### Comparing `syntaxlight-0.1.5/LICENSE` & `syntaxlight-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/README.md` & `syntaxlight-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/syntaxlight/ast.py` & `syntaxlight-0.1.6/syntaxlight/ast.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/syntaxlight/css/all.css` & `syntaxlight-0.1.6/syntaxlight/css/all.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/syntaxlight/css/asm.css` & `syntaxlight-0.1.6/syntaxlight/css/x86asm.css`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-pre[class*="language-asm"] {
+pre[class*="language-x86asm"] {
     background: --background;
 }
 
 .Token {
     color: --punctuator;
 }
 
+.Token.ID {
+    color: --function;
+}
+
 .Token.BraceDepth-0 {
     color: --brace1;
 }
 
 .Token.BraceDepth-1 {
     color: --brace2;
 }
@@ -36,8 +40,12 @@
 
 .Token.ASM_KEYWORD {
     color: --define;
 }
 
 .Token.SECTION {
     color: --variant;
+}
+
+.Token.DOLLAR {
+    color: --variant;
 }
```

### Comparing `syntaxlight-0.1.5/syntaxlight/css/bnf.css` & `syntaxlight-0.1.6/syntaxlight/css/bnf.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/syntaxlight/css/c.css` & `syntaxlight-0.1.6/syntaxlight/css/c.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/syntaxlight/css/css.css` & `syntaxlight-0.1.6/syntaxlight/css/css.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/syntaxlight/css/index.css` & `syntaxlight-0.1.6/syntaxlight/css/index.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/syntaxlight/css/json.css` & `syntaxlight-0.1.6/syntaxlight/css/json.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/syntaxlight/css/lua.css` & `syntaxlight-0.1.6/syntaxlight/css/lua.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/syntaxlight/css/makefile.css` & `syntaxlight-0.1.6/syntaxlight/css/makefile.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/syntaxlight/css/shell.css` & `syntaxlight-0.1.6/syntaxlight/css/shell.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/syntaxlight/css/themes.json` & `syntaxlight-0.1.6/syntaxlight/css/themes.json`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/syntaxlight/css/toml.css` & `syntaxlight-0.1.6/syntaxlight/css/toml.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/syntaxlight/error.py` & `syntaxlight-0.1.6/syntaxlight/error.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/syntaxlight/example.py` & `syntaxlight-0.1.6/syntaxlight/example.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     language= None,
 ):
     example_folder_name = os.path.join(os.getcwd(), "syntaxlight_example")
     syntaxlight_path = os.path.dirname(__file__)
     html_template_file = os.path.join(syntaxlight_path, "template.html")
     index_css_file = os.path.join(syntaxlight_path, "css", "index.css")
     css_files = [index_css_file]
-    
 
     example_html_file = os.path.join(example_folder_name, "index.html")
 
     if not os.path.exists(example_folder_name):
         os.mkdir(example_folder_name)
 
     if type(file_path) == str:
```

### Comparing `syntaxlight-0.1.5/syntaxlight/export.py` & `syntaxlight-0.1.6/syntaxlight/export.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/syntaxlight/gdt.py` & `syntaxlight-0.1.6/syntaxlight/gdt.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/syntaxlight/language.py` & `syntaxlight-0.1.6/syntaxlight/language.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 import os
 from .lexers import *
 from .parsers import *
 import re
 from typing import List, TypedDict
 
+
 class SyntaxDict(TypedDict):
     lexer: Lexer
     parser: Parser
     suffix: List[str]
 
+
 SUPPORTED_SYNTAX = {
-    "json": SyntaxDict(lexer=JsonLexer, parser=JsonParser, suffix=['json']),
+    "json": SyntaxDict(lexer=JsonLexer, parser=JsonParser, suffix=["json"]),
     "c": SyntaxDict(lexer=CLexer, parser=CParser, suffix=["c", "h"]),
-    "lua": SyntaxDict(lexer=LuaLexer, parser=LuaParser, suffix=['lua']),
-    "bnf": SyntaxDict(lexer=BNFLexer, parser=BNFParser, suffix=['bnf']),
-    "toml": SyntaxDict(lexer=TomlLexer, parser=TomlParser, suffix=['toml']),
-    "xml": SyntaxDict(lexer=XmlLexer, parser=XmlParser, suffix=['xml']),
-    "shell": SyntaxDict(lexer=ShellLexer, parser=ShellParser, suffix=['sh']),
-    "asm": SyntaxDict(lexer=AssemblyLexer, parser=AssemblyParser, suffix=['asm']),
-    "css": SyntaxDict(lexer=CSSLexer,parser=CSSParser, suffix=['css']),
-    "makefile": SyntaxDict(lexer=MakefileLexer,parser=MakefileParser, suffix=['mk','mak'])
+    "lua": SyntaxDict(lexer=LuaLexer, parser=LuaParser, suffix=["lua"]),
+    "bnf": SyntaxDict(lexer=BNFLexer, parser=BNFParser, suffix=["bnf"]),
+    "toml": SyntaxDict(lexer=TomlLexer, parser=TomlParser, suffix=["toml"]),
+    "xml": SyntaxDict(lexer=XmlLexer, parser=XmlParser, suffix=["xml"]),
+    "shell": SyntaxDict(lexer=ShellLexer, parser=ShellParser, suffix=["sh"]),
+    "x86asm": SyntaxDict(lexer=X86AssemblyLexer, parser=X86AssemblyParser, suffix=["asm"]),
+    "riscvasm": SyntaxDict(lexer=RISCVAssemblyLexer, parser=RISCVAssmemblyParser, suffix=["S"]),
+    "css": SyntaxDict(lexer=CSSLexer, parser=CSSParser, suffix=["css"]),
+    "makefile": SyntaxDict(lexer=MakefileLexer, parser=MakefileParser, suffix=["mk", "mak"]),
 }
 
-def clean_language(language:str):
-    
+
+def clean_language(language: str):
     language = language.lower()
     rename_languages = {
-        r'^bash$': 'shell',
-        r'.*?asm.*?': 'asm'
+        r"^bash$": "shell",
     }
     for r_language in rename_languages:
         if bool(re.match(r_language, language)):
             return rename_languages[r_language]
-        
+
     return language
 
+
 def guess_language(file_path: str) -> str:
     """
     通过文件名猜测文法类型
     """
     suffix_name = file_path.split(os.sep)[-1].split(".")[-1]
     for language in SUPPORTED_SYNTAX:
         if suffix_name in SUPPORTED_SYNTAX[language]["suffix"]:
@@ -47,20 +50,22 @@
     if suffix_name in SUPPORTED_SYNTAX:
         return suffix_name
 
     print("fail to guess language")
     show_help_info()
     exit(1)
 
+
 def show_help_info():
     print(f"supported language:")
     for language in SUPPORTED_SYNTAX:
         print(f"{language:>10}:", SUPPORTED_SYNTAX[language]["suffix"])
     exit(1)
 
+
 def is_language_support(language: str):
     """
     检验 syntaxlight 是否支持当前语言
     """
     language = clean_language(language)
     global SUPPORTED_SYNTAX
     return language in SUPPORTED_SYNTAX
```

### Comparing `syntaxlight-0.1.5/syntaxlight/lexers/asm_lexer.py` & `syntaxlight-0.1.6/syntaxlight/lexers/makefile_lexer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,67 +1,92 @@
 from syntaxlight.lexers.lexer import Token
-from .lexer import Lexer, Token, TokenType, ErrorCode
+from .lexer import Lexer, Token, TokenType, ErrorCode, TokenSet
 from enum import Enum
-import re
 
 
-class AssemblyTokenType(Enum):
-    ASM_KEYWORD = "ASM_KEYWORD"
-    REGISTER = "REGISTER"
-    FUNCTION_CALL = "FUNCTION_CALL"
-    SECTION = "SECTION"
+class MakefileTokenType(Enum):
+    RESERVED_KEYWORD_START = "RESERVED_KEYWORD_START"
+    INCLUDE = "include"
+    IFEQ = "ifeq"
+    IFNEQ = "ifneq"
+    IFDEF = "ifdef"
+    IFNDEF = "ifndef"
+    ELSE = 'else'
+    ENDIF = "endif"
+    EXPORT = "export"
+    UNEXPORT = "unexport"
+    RESERVED_KEYWORD_END = "RESERVED_KEYWORD_END"
+    PATH_SLASH = "/"
+    LATER_ASSIGN = ":="
+    REDIRECT_TO = ">"
+    REDIRECT_FROM = "<"
+    AUTO_VARIABLE = "AUTO_VARIABLE"
+    OPTION = 'OPTION'
 
 
-class AssemblyLexer(Lexer):
-    def __init__(self, text: str, LanguageTokenType: Enum = AssemblyTokenType):
+class MakefileLexer(Lexer):
+    def __init__(self, text: str, LanguageTokenType: Enum = MakefileTokenType):
         super().__init__(text, LanguageTokenType)
+        self.build_long_op_dict([":=", "+="])
+
+    def get_option(self):
+        """
+        长短选项
+        -s --options
+        """
+        result = ""
+        while self.current_char is not None:
+            if self.current_char.isalnum() or self.current_char in ("-", "_"):
+                result += self.current_char
+                self.advance()
+            else:
+                break
+
+        return Token(MakefileTokenType.OPTION, result, self.line, self.column - 1)
 
     def get_next_token(self) -> Token:
         while self.current_char is not None:
             if self.current_char == TokenType.SPACE.value:
                 return self.skip_whitespace()
 
             if self.current_char in self.invisible_characters:
                 return self.skip_invisiable_character()
 
-            if self.current_char.isdigit():
-                return self.get_number(accept_bit=True, accept_hex=True)
+            if self.current_char == '"':
+                return self.get_string()
 
-            if self.current_char.isalnum() or self.current_char in ("_"):
-                return self.get_id(extend_chars=["@", "_"])
+            if self.current_char == TokenType.HASH.value:
+                # match comment
+                return self.get_comment()
+            
+            if self.current_char == "-" and (self.peek().isalpha() or self.peek() == '-'):
+                return self.get_option()
 
-            if self.current_char == ".":
-                result = "."
-                self.advance()
-                while self.current_char is not None and self.current_char.isalnum():
-                    result += self.current_char
-                    self.advance()
+            if self.current_char in self.long_op_dict:
+                return self.get_long_op()
 
-                token = Token(AssemblyTokenType.ASM_KEYWORD, result, self.line, self.column - 1)
-                return token
+            if self.current_char.isdigit():
+                return self.get_number()
 
-            if self.current_char == "%":
-                result = "%"
-                self.advance()
-                while self.current_char is not None and self.current_char.isalnum():
-                    result += self.current_char
-                    self.advance()
+            if self.current_char.isalpha() or self.current_char in ("-", "_", ".", "%"):
+                return self.get_id(extend_chars=["_", "-", ".", "%",'/'])
 
-                token = Token(AssemblyTokenType.REGISTER, result, self.line, self.column - 1)
+            if self.current_char == "$" and self.peek() in ["@", "%", "<", "?", "^", "+", "*"]:
+                result = "$"
+                self.advance()
+                result += self.current_char
+                token = Token(MakefileTokenType.AUTO_VARIABLE, result, self.line, self.column)
+                self.advance()
                 return token
 
-            if self.current_char == "#":
-                return self.get_comment()
-
             try:
                 token_type = TokenType(self.current_char)
             except ValueError:  # pragma: no cover
-                token = Token(TokenType.TEXT, self.current_char, self.line, self.column)
-                self.advance()
-                return token
+                token = Token(None, self.current_char, self.line, self.column)
+                self.error(ErrorCode.UNKNOWN_CHARACTER, token)
             else:
                 token = Token(
                     type=token_type,
                     value=token_type.value,  # e.g. ';', '.', etc
                     line=self.line,
                     column=self.column,
                 )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `syntaxlight-0.1.5/syntaxlight/lexers/bnf_lexer.py` & `syntaxlight-0.1.6/syntaxlight/lexers/bnf_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/syntaxlight/lexers/c_lexer.py` & `syntaxlight-0.1.6/syntaxlight/lexers/c_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/syntaxlight/lexers/css_lexer.py` & `syntaxlight-0.1.6/syntaxlight/lexers/css_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/syntaxlight/lexers/json_lexer.py` & `syntaxlight-0.1.6/syntaxlight/lexers/json_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/syntaxlight/lexers/lexer.py` & `syntaxlight-0.1.6/syntaxlight/lexers/lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/syntaxlight/lexers/lua_lexer.py` & `syntaxlight-0.1.6/syntaxlight/lexers/lua_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/syntaxlight/lexers/makefile_lexer.py` & `syntaxlight-0.1.6/syntaxlight/lexers/toml_lexer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,86 +1,65 @@
-from syntaxlight.lexers.lexer import Token
-from .lexer import Lexer, Token, TokenType, ErrorCode, TokenSet
+from .lexer import Lexer, Token, TokenType
+from ..error import ErrorCode
 from enum import Enum
 
 
-class MakefileTokenType(Enum):
+class TomlTokenType(Enum):
     RESERVED_KEYWORD_START = "RESERVED_KEYWORD_START"
-    INCLUDE = "include"
-    IFEQ = "ifeq"
-    IFNEQ = "ifneq"
-    IFDEF = "ifdef"
-    IFNDEF = "ifndef"
-    ELSE = 'else'
-    ENDIF = "endif"
-    EXPORT = "export"
-    UNEXPORT = "unexport"
+    TRUE = "true"
+    FALSE = "false"
     RESERVED_KEYWORD_END = "RESERVED_KEYWORD_END"
-    PATH_SLASH = "/"
-    LATER_ASSIGN = ":="
-    REDIRECT_TO = ">"
-    REDIRECT_FROM = "<"
-    AUTO_VARIABLE = "AUTO_VARIABLE"
-    OPTION = 'OPTION'
 
+    DATE = "DATE"
 
-class MakefileLexer(Lexer):
-    def __init__(self, text: str, LanguageTokenType: Enum = MakefileTokenType):
+
+class TomlLexer(Lexer):
+    def __init__(self, text: str, LanguageTokenType: Enum = TomlTokenType):
         super().__init__(text, LanguageTokenType)
-        self.build_long_op_dict([":=", "+="])
 
-    def get_option(self):
-        """
-        长短选项
-        -s --options
-        """
-        result = ""
+    def get_next_token(self):
         while self.current_char is not None:
-            if self.current_char.isalnum() or self.current_char in ("-", "_"):
-                result += self.current_char
-                self.advance()
-            else:
-                break
+            if self.current_char == "'" and self.peek(2) == "''":
+                return self.get_extend_str(("'''", "'''"))
+            if self.current_char == '"' and self.peek(2) == '""':
+                return self.get_extend_str(('"""', '"""'))
+
+            # TOML 单双引号都可以
+            if self.current_char in ('"', "'"):
+                return self.get_str()
 
-        return Token(MakefileTokenType.OPTION, result, self.line, self.column - 1)
-
-    def get_next_token(self) -> Token:
-        while self.current_char is not None:
             if self.current_char == TokenType.SPACE.value:
                 return self.skip_whitespace()
 
             if self.current_char in self.invisible_characters:
                 return self.skip_invisiable_character()
 
-            if self.current_char == '"':
-                return self.get_string()
-
             if self.current_char == TokenType.HASH.value:
                 # match comment
                 return self.get_comment()
-            
-            if self.current_char == "-" and (self.peek().isalpha() or self.peek() == '-'):
-                return self.get_option()
-
-            if self.current_char in self.long_op_dict:
-                return self.get_long_op()
 
             if self.current_char.isdigit():
-                return self.get_number()
-
-            if self.current_char.isalpha() or self.current_char in ("-", "_", ".", "%"):
-                return self.get_id(extend_chars=["_", "-", ".", "%",'/'])
+                token = self.get_number()
+                # https://datatracker.ietf.org/doc/html/rfc3339
+                # a tricky implementation
+                if self.current_char in (TokenType.MINUS.value, TokenType.COLON.value):
+                    result = token.value
+                    while self.current_char is not None and self.current_char not in (
+                        TokenType.HASH.value,
+                        TokenType.CR.value,
+                        TokenType.LF.value,
+                    ):
+                        result += self.current_char
+                        self.advance()
+                    return Token(TomlTokenType.DATE, result, self.line, self.column - 1)
+                else:
+                    return token
 
-            if self.current_char == "$" and self.peek() in ["@", "%", "<", "?", "^", "+", "*"]:
-                result = "$"
-                self.advance()
-                result += self.current_char
-                token = Token(MakefileTokenType.AUTO_VARIABLE, result, self.line, self.column)
-                self.advance()
-                return token
+            if self.current_char.isalpha():
+                return self.get_id(extend_chars=["_",'-'])
 
             try:
                 token_type = TokenType(self.current_char)
             except ValueError:  # pragma: no cover
                 token = Token(None, self.current_char, self.line, self.column)
                 self.error(ErrorCode.UNKNOWN_CHARACTER, token)
             else:
@@ -89,9 +68,10 @@
                     value=token_type.value,  # e.g. ';', '.', etc
                     line=self.line,
                     column=self.column,
                 )
                 self.advance()
                 return token
 
-        # End of File
+        # EOF (end-of-file) token indicates that there is no more
+        # input left for lexical analysis
         return Token(type=TokenType.EOF, value="EOF", line=self.line, column=self.column)
```

### Comparing `syntaxlight-0.1.5/syntaxlight/lexers/shell_lexer.py` & `syntaxlight-0.1.6/syntaxlight/lexers/shell_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/syntaxlight/lexers/xml_lexer.py` & `syntaxlight-0.1.6/syntaxlight/lexers/xml_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/syntaxlight/parsers/bnf_parser.py` & `syntaxlight-0.1.6/syntaxlight/parsers/bnf_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/syntaxlight/parsers/c_parser.py` & `syntaxlight-0.1.6/syntaxlight/parsers/c_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/syntaxlight/parsers/css_parser.py` & `syntaxlight-0.1.6/syntaxlight/parsers/css_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/syntaxlight/parsers/json_parser.py` & `syntaxlight-0.1.6/syntaxlight/parsers/json_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/syntaxlight/parsers/lua_parser.py` & `syntaxlight-0.1.6/syntaxlight/parsers/lua_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/syntaxlight/parsers/makefile_parser.py` & `syntaxlight-0.1.6/syntaxlight/parsers/makefile_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/syntaxlight/parsers/parser.py` & `syntaxlight-0.1.6/syntaxlight/parsers/parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/syntaxlight/parsers/shell_parser.py` & `syntaxlight-0.1.6/syntaxlight/parsers/shell_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/syntaxlight/parsers/toml_parser.py` & `syntaxlight-0.1.6/syntaxlight/parsers/toml_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/syntaxlight/parsers/xml_parser.py` & `syntaxlight-0.1.6/syntaxlight/parsers/xml_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/syntaxlight/syntax_parse.py` & `syntaxlight-0.1.6/syntaxlight/syntax_parse.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.5/PKG-INFO` & `syntaxlight-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syntaxlight
-Version: 0.1.5
+Version: 0.1.6
 Summary: syntax highlight based on EBNF
 Home-page: https://github.com/luzhixing12345/syntaxlight
 License: MIT
 Author: luzhixing12345
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

