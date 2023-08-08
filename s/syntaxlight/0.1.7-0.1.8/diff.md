# Comparing `tmp/syntaxlight-0.1.7.tar.gz` & `tmp/syntaxlight-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntaxlight-0.1.7.tar", max compression
+gzip compressed data, was "syntaxlight-0.1.8.tar", max compression
```

## Comparing `syntaxlight-0.1.7.tar` & `syntaxlight-0.1.8.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1064 2023-06-08 14:13:12.759574 syntaxlight-0.1.7/LICENSE
--rw-r--r--   0        0        0      463 2023-08-08 02:56:56.199393 syntaxlight-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2258 2023-07-30 13:40:10.383897 syntaxlight-0.1.7/README.md
--rw-r--r--   0        0        0      257 2023-08-05 06:18:14.085640 syntaxlight-0.1.7/syntaxlight/__init__.py
--rw-r--r--   0        0        0    15445 2023-08-02 07:08:27.516374 syntaxlight-0.1.7/syntaxlight/ast.py
--rw-r--r--   0        0        0     2244 2023-08-05 14:13:35.618950 syntaxlight-0.1.7/syntaxlight/css/all.css
--rw-r--r--   0        0        0      666 2023-08-01 01:05:24.175123 syntaxlight-0.1.7/syntaxlight/css/bnf.css
--rw-r--r--   0        0        0     2210 2023-08-01 01:05:24.173124 syntaxlight-0.1.7/syntaxlight/css/c.css
--rw-r--r--   0        0        0      627 2023-08-01 01:05:24.172126 syntaxlight-0.1.7/syntaxlight/css/css.css
--rw-r--r--   0        0        0    18397 2023-06-15 07:10:53.753178 syntaxlight-0.1.7/syntaxlight/css/index.css
--rw-r--r--   0        0        0      531 2023-08-01 01:05:24.171126 syntaxlight-0.1.7/syntaxlight/css/json.css
--rw-r--r--   0        0        0     1106 2023-08-01 01:05:24.170124 syntaxlight-0.1.7/syntaxlight/css/lua.css
--rw-r--r--   0        0        0      953 2023-08-02 09:02:28.094967 syntaxlight-0.1.7/syntaxlight/css/makefile.css
--rw-r--r--   0        0        0      876 2023-08-08 02:48:11.688084 syntaxlight-0.1.7/syntaxlight/css/riscvasm.css
--rw-r--r--   0        0        0      878 2023-08-05 14:06:43.880293 syntaxlight-0.1.7/syntaxlight/css/shell.css
--rw-r--r--   0        0        0     3068 2023-08-08 01:56:22.718774 syntaxlight-0.1.7/syntaxlight/css/themes.json
--rw-r--r--   0        0        0      558 2023-08-01 01:05:24.166692 syntaxlight-0.1.7/syntaxlight/css/toml.css
--rw-r--r--   0        0        0      625 2023-08-08 02:07:40.488130 syntaxlight-0.1.7/syntaxlight/css/x86asm.css
--rw-r--r--   0        0        0      497 2023-08-01 01:05:24.165690 syntaxlight-0.1.7/syntaxlight/css/xml.css
--rw-r--r--   0        0        0     2478 2023-07-30 12:33:41.489986 syntaxlight-0.1.7/syntaxlight/error.py
--rw-r--r--   0        0        0     1941 2023-08-08 02:05:48.378946 syntaxlight-0.1.7/syntaxlight/example.py
--rw-r--r--   0        0        0     1926 2023-08-08 01:51:12.605756 syntaxlight-0.1.7/syntaxlight/export.py
--rw-r--r--   0        0        0     2875 2023-07-30 12:21:15.272257 syntaxlight-0.1.7/syntaxlight/gdt.py
--rw-r--r--   0        0        0     2270 2023-08-08 02:03:57.826551 syntaxlight-0.1.7/syntaxlight/language.py
--rw-r--r--   0        0        0      655 2023-08-08 02:00:04.293166 syntaxlight-0.1.7/syntaxlight/lexers/__init__.py
--rw-r--r--   0        0        0     5624 2023-08-08 02:37:33.290993 syntaxlight-0.1.7/syntaxlight/lexers/asm_lexer.py
--rw-r--r--   0        0        0     1921 2023-07-26 05:57:52.779798 syntaxlight-0.1.7/syntaxlight/lexers/bnf_lexer.py
--rw-r--r--   0        0        0    12853 2023-07-31 01:57:07.230431 syntaxlight-0.1.7/syntaxlight/lexers/c_lexer.py
--rw-r--r--   0        0        0     3837 2023-07-31 03:00:49.403592 syntaxlight-0.1.7/syntaxlight/lexers/css_lexer.py
--rw-r--r--   0        0        0     1995 2023-07-26 05:58:05.904375 syntaxlight-0.1.7/syntaxlight/lexers/json_lexer.py
--rw-r--r--   0        0        0    24439 2023-08-05 06:20:18.443117 syntaxlight-0.1.7/syntaxlight/lexers/lexer.py
--rw-r--r--   0        0        0     8161 2023-07-31 02:35:08.122706 syntaxlight-0.1.7/syntaxlight/lexers/lua_lexer.py
--rw-r--r--   0        0        0     3407 2023-08-02 08:39:01.519231 syntaxlight-0.1.7/syntaxlight/lexers/makefile_lexer.py
--rw-r--r--   0        0        0     4485 2023-08-07 13:41:15.732684 syntaxlight-0.1.7/syntaxlight/lexers/shell_lexer.py
--rw-r--r--   0        0        0     3006 2023-07-30 13:42:04.120083 syntaxlight-0.1.7/syntaxlight/lexers/toml_lexer.py
--rw-r--r--   0        0        0     4576 2023-07-26 05:58:25.950097 syntaxlight-0.1.7/syntaxlight/lexers/xml_lexer.py
--rw-r--r--   0        0        0      432 2023-08-08 01:59:24.336858 syntaxlight-0.1.7/syntaxlight/parsers/__init__.py
--rw-r--r--   0        0        0     4621 2023-08-08 02:47:31.924199 syntaxlight-0.1.7/syntaxlight/parsers/asm_parser.py
--rw-r--r--   0        0        0     6950 2023-07-24 08:35:40.217597 syntaxlight-0.1.7/syntaxlight/parsers/bnf_parser.py
--rw-r--r--   0        0        0   106329 2023-08-05 13:55:32.850499 syntaxlight-0.1.7/syntaxlight/parsers/c_parser.py
--rw-r--r--   0        0        0     1719 2023-07-31 03:13:51.887478 syntaxlight-0.1.7/syntaxlight/parsers/css_parser.py
--rw-r--r--   0        0        0     5758 2023-07-24 01:35:24.219886 syntaxlight-0.1.7/syntaxlight/parsers/json_parser.py
--rw-r--r--   0        0        0    35078 2023-07-31 02:33:22.161465 syntaxlight-0.1.7/syntaxlight/parsers/lua_parser.py
--rw-r--r--   0        0        0     3283 2023-08-02 09:02:17.026646 syntaxlight-0.1.7/syntaxlight/parsers/makefile_parser.py
--rw-r--r--   0        0        0    13274 2023-08-07 13:44:41.858038 syntaxlight-0.1.7/syntaxlight/parsers/parser.py
--rw-r--r--   0        0        0     5269 2023-08-07 13:41:57.292919 syntaxlight-0.1.7/syntaxlight/parsers/shell_parser.py
--rw-r--r--   0        0        0    11810 2023-07-24 01:35:24.522506 syntaxlight-0.1.7/syntaxlight/parsers/toml_parser.py
--rw-r--r--   0        0        0     6531 2023-07-24 01:35:24.720887 syntaxlight-0.1.7/syntaxlight/parsers/xml_parser.py
--rw-r--r--   0        0        0     2335 2023-08-03 06:34:30.224044 syntaxlight-0.1.7/syntaxlight/syntax_parse.py
--rw-r--r--   0        0        0      349 2023-07-25 01:26:08.919200 syntaxlight-0.1.7/syntaxlight/template.html
--rw-r--r--   0        0        0     3049 1970-01-01 00:00:00.000000 syntaxlight-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-08 14:13:12.759574 syntaxlight-0.1.8/LICENSE
+-rw-r--r--   0        0        0      463 2023-08-08 08:07:50.096903 syntaxlight-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2258 2023-07-30 13:40:10.383897 syntaxlight-0.1.8/README.md
+-rw-r--r--   0        0        0      257 2023-08-05 06:18:14.085640 syntaxlight-0.1.8/syntaxlight/__init__.py
+-rw-r--r--   0        0        0    15445 2023-08-02 07:08:27.516374 syntaxlight-0.1.8/syntaxlight/ast.py
+-rw-r--r--   0        0        0     2244 2023-08-05 14:13:35.618950 syntaxlight-0.1.8/syntaxlight/css/all.css
+-rw-r--r--   0        0        0      666 2023-08-01 01:05:24.175123 syntaxlight-0.1.8/syntaxlight/css/bnf.css
+-rw-r--r--   0        0        0     2210 2023-08-01 01:05:24.173124 syntaxlight-0.1.8/syntaxlight/css/c.css
+-rw-r--r--   0        0        0      627 2023-08-01 01:05:24.172126 syntaxlight-0.1.8/syntaxlight/css/css.css
+-rw-r--r--   0        0        0    18397 2023-06-15 07:10:53.753178 syntaxlight-0.1.8/syntaxlight/css/index.css
+-rw-r--r--   0        0        0      531 2023-08-01 01:05:24.171126 syntaxlight-0.1.8/syntaxlight/css/json.css
+-rw-r--r--   0        0        0     1106 2023-08-01 01:05:24.170124 syntaxlight-0.1.8/syntaxlight/css/lua.css
+-rw-r--r--   0        0        0      953 2023-08-02 09:02:28.094967 syntaxlight-0.1.8/syntaxlight/css/makefile.css
+-rw-r--r--   0        0        0      876 2023-08-08 02:48:11.688084 syntaxlight-0.1.8/syntaxlight/css/riscvasm.css
+-rw-r--r--   0        0        0      878 2023-08-05 14:06:43.880293 syntaxlight-0.1.8/syntaxlight/css/shell.css
+-rw-r--r--   0        0        0     3068 2023-08-08 01:56:22.718774 syntaxlight-0.1.8/syntaxlight/css/themes.json
+-rw-r--r--   0        0        0      558 2023-08-01 01:05:24.166692 syntaxlight-0.1.8/syntaxlight/css/toml.css
+-rw-r--r--   0        0        0      625 2023-08-08 02:07:40.488130 syntaxlight-0.1.8/syntaxlight/css/x86asm.css
+-rw-r--r--   0        0        0      497 2023-08-01 01:05:24.165690 syntaxlight-0.1.8/syntaxlight/css/xml.css
+-rw-r--r--   0        0        0     2478 2023-07-30 12:33:41.489986 syntaxlight-0.1.8/syntaxlight/error.py
+-rw-r--r--   0        0        0     1941 2023-08-08 02:05:48.378946 syntaxlight-0.1.8/syntaxlight/example.py
+-rw-r--r--   0        0        0     1926 2023-08-08 01:51:12.605756 syntaxlight-0.1.8/syntaxlight/export.py
+-rw-r--r--   0        0        0     2875 2023-07-30 12:21:15.272257 syntaxlight-0.1.8/syntaxlight/gdt.py
+-rw-r--r--   0        0        0     2270 2023-08-08 02:03:57.826551 syntaxlight-0.1.8/syntaxlight/language.py
+-rw-r--r--   0        0        0      655 2023-08-08 02:00:04.293166 syntaxlight-0.1.8/syntaxlight/lexers/__init__.py
+-rw-r--r--   0        0        0     5624 2023-08-08 02:37:33.290993 syntaxlight-0.1.8/syntaxlight/lexers/asm_lexer.py
+-rw-r--r--   0        0        0     1921 2023-07-26 05:57:52.779798 syntaxlight-0.1.8/syntaxlight/lexers/bnf_lexer.py
+-rw-r--r--   0        0        0    12886 2023-08-08 07:48:52.889333 syntaxlight-0.1.8/syntaxlight/lexers/c_lexer.py
+-rw-r--r--   0        0        0     3837 2023-07-31 03:00:49.403592 syntaxlight-0.1.8/syntaxlight/lexers/css_lexer.py
+-rw-r--r--   0        0        0     1995 2023-07-26 05:58:05.904375 syntaxlight-0.1.8/syntaxlight/lexers/json_lexer.py
+-rw-r--r--   0        0        0    24439 2023-08-05 06:20:18.443117 syntaxlight-0.1.8/syntaxlight/lexers/lexer.py
+-rw-r--r--   0        0        0     8161 2023-07-31 02:35:08.122706 syntaxlight-0.1.8/syntaxlight/lexers/lua_lexer.py
+-rw-r--r--   0        0        0     3407 2023-08-02 08:39:01.519231 syntaxlight-0.1.8/syntaxlight/lexers/makefile_lexer.py
+-rw-r--r--   0        0        0     4485 2023-08-07 13:41:15.732684 syntaxlight-0.1.8/syntaxlight/lexers/shell_lexer.py
+-rw-r--r--   0        0        0     3006 2023-07-30 13:42:04.120083 syntaxlight-0.1.8/syntaxlight/lexers/toml_lexer.py
+-rw-r--r--   0        0        0     4576 2023-07-26 05:58:25.950097 syntaxlight-0.1.8/syntaxlight/lexers/xml_lexer.py
+-rw-r--r--   0        0        0      432 2023-08-08 01:59:24.336858 syntaxlight-0.1.8/syntaxlight/parsers/__init__.py
+-rw-r--r--   0        0        0     4621 2023-08-08 02:47:31.924199 syntaxlight-0.1.8/syntaxlight/parsers/asm_parser.py
+-rw-r--r--   0        0        0     6950 2023-07-24 08:35:40.217597 syntaxlight-0.1.8/syntaxlight/parsers/bnf_parser.py
+-rw-r--r--   0        0        0   107472 2023-08-08 08:07:35.217460 syntaxlight-0.1.8/syntaxlight/parsers/c_parser.py
+-rw-r--r--   0        0        0     1719 2023-07-31 03:13:51.887478 syntaxlight-0.1.8/syntaxlight/parsers/css_parser.py
+-rw-r--r--   0        0        0     5758 2023-07-24 01:35:24.219886 syntaxlight-0.1.8/syntaxlight/parsers/json_parser.py
+-rw-r--r--   0        0        0    35078 2023-07-31 02:33:22.161465 syntaxlight-0.1.8/syntaxlight/parsers/lua_parser.py
+-rw-r--r--   0        0        0     3283 2023-08-02 09:02:17.026646 syntaxlight-0.1.8/syntaxlight/parsers/makefile_parser.py
+-rw-r--r--   0        0        0    13274 2023-08-07 13:44:41.858038 syntaxlight-0.1.8/syntaxlight/parsers/parser.py
+-rw-r--r--   0        0        0     5269 2023-08-07 13:41:57.292919 syntaxlight-0.1.8/syntaxlight/parsers/shell_parser.py
+-rw-r--r--   0        0        0    11810 2023-07-24 01:35:24.522506 syntaxlight-0.1.8/syntaxlight/parsers/toml_parser.py
+-rw-r--r--   0        0        0     6531 2023-07-24 01:35:24.720887 syntaxlight-0.1.8/syntaxlight/parsers/xml_parser.py
+-rw-r--r--   0        0        0     2335 2023-08-03 06:34:30.224044 syntaxlight-0.1.8/syntaxlight/syntax_parse.py
+-rw-r--r--   0        0        0      349 2023-07-25 01:26:08.919200 syntaxlight-0.1.8/syntaxlight/template.html
+-rw-r--r--   0        0        0     3049 1970-01-01 00:00:00.000000 syntaxlight-0.1.8/PKG-INFO
```

### Comparing `syntaxlight-0.1.7/LICENSE` & `syntaxlight-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/README.md` & `syntaxlight-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/ast.py` & `syntaxlight-0.1.8/syntaxlight/ast.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/css/all.css` & `syntaxlight-0.1.8/syntaxlight/css/all.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/css/bnf.css` & `syntaxlight-0.1.8/syntaxlight/css/bnf.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/css/c.css` & `syntaxlight-0.1.8/syntaxlight/css/c.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/css/css.css` & `syntaxlight-0.1.8/syntaxlight/css/css.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/css/index.css` & `syntaxlight-0.1.8/syntaxlight/css/index.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/css/json.css` & `syntaxlight-0.1.8/syntaxlight/css/json.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/css/lua.css` & `syntaxlight-0.1.8/syntaxlight/css/lua.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/css/makefile.css` & `syntaxlight-0.1.8/syntaxlight/css/makefile.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/css/riscvasm.css` & `syntaxlight-0.1.8/syntaxlight/css/riscvasm.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/css/shell.css` & `syntaxlight-0.1.8/syntaxlight/css/shell.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/css/themes.json` & `syntaxlight-0.1.8/syntaxlight/css/themes.json`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/css/toml.css` & `syntaxlight-0.1.8/syntaxlight/css/toml.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/css/x86asm.css` & `syntaxlight-0.1.8/syntaxlight/css/x86asm.css`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/error.py` & `syntaxlight-0.1.8/syntaxlight/error.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/example.py` & `syntaxlight-0.1.8/syntaxlight/example.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/export.py` & `syntaxlight-0.1.8/syntaxlight/export.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/gdt.py` & `syntaxlight-0.1.8/syntaxlight/gdt.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/language.py` & `syntaxlight-0.1.8/syntaxlight/language.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/lexers/__init__.py` & `syntaxlight-0.1.8/syntaxlight/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/lexers/asm_lexer.py` & `syntaxlight-0.1.8/syntaxlight/lexers/asm_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/lexers/bnf_lexer.py` & `syntaxlight-0.1.8/syntaxlight/lexers/bnf_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/lexers/c_lexer.py` & `syntaxlight-0.1.8/syntaxlight/lexers/c_lexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     _GENERIC = "_Generic"
     _IMAGINARY = "_Imaginary"
     _NORETURN = "_Noreturn"
     _STATIC_ASSERT = "_Static_assert"  # C23 => STATIC_ASSERT
     _THREAD_LOCAL = "_Thread_local"  # C23 => THREAD_LOCAL
 
     # GNU C extension
+    ASM = 'asm'
     _ASM = "__asm__"
     _ATTRIBUTE = "__attribute__"
 
     RESERVED_KEYWORD_END = "RESERVED_KEYWORD_END"
     # start - end 之间为对应语言的保留关键字
     # -----------------------------------------------
 
@@ -314,15 +315,15 @@
         self.expression_statement = TokenSet(self.expression, TokenType.SEMI)
         self.compound_statement = TokenSet(TokenType.LCURLY_BRACE)
         self.selection_statement = TokenSet(CTokenType.IF, CTokenType.SWITCH)
         self.iteration_statement = TokenSet(CTokenType.WHILE, CTokenType.DO, CTokenType.FOR)
         self.jump_statement = TokenSet(
             CTokenType.GOTO, CTokenType.CONTINUE, CTokenType.BREAK, CTokenType.RETURN
         )
-        self.gnu_c_statement_extension = TokenSet(CTokenType._ASM)
+        self.gnu_c_statement_extension = TokenSet(CTokenType._ASM, CTokenType.ASM)
         self.statement = TokenSet(
             self.labeled_statement,
             self.expression_statement,
             self.compound_statement,
             self.selection_statement,
             self.iteration_statement,
             self.jump_statement,
```

### Comparing `syntaxlight-0.1.7/syntaxlight/lexers/css_lexer.py` & `syntaxlight-0.1.8/syntaxlight/lexers/css_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/lexers/json_lexer.py` & `syntaxlight-0.1.8/syntaxlight/lexers/json_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/lexers/lexer.py` & `syntaxlight-0.1.8/syntaxlight/lexers/lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/lexers/lua_lexer.py` & `syntaxlight-0.1.8/syntaxlight/lexers/lua_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/lexers/makefile_lexer.py` & `syntaxlight-0.1.8/syntaxlight/lexers/makefile_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/lexers/shell_lexer.py` & `syntaxlight-0.1.8/syntaxlight/lexers/shell_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/lexers/toml_lexer.py` & `syntaxlight-0.1.8/syntaxlight/lexers/toml_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/lexers/xml_lexer.py` & `syntaxlight-0.1.8/syntaxlight/lexers/xml_lexer.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/parsers/asm_parser.py` & `syntaxlight-0.1.8/syntaxlight/parsers/asm_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/parsers/bnf_parser.py` & `syntaxlight-0.1.8/syntaxlight/parsers/bnf_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/parsers/c_parser.py` & `syntaxlight-0.1.8/syntaxlight/parsers/c_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -844,15 +844,15 @@
         node.register_token(self.eat(TokenType.RPAREN))
         add_ast_type(node, C_CSS.ATOMAIC_TYPE_SPECIFIER)
         return node
 
     def struct_or_union_specifier(self):
         """
         <struct-or-union-specifier> ::= <struct-or-union> <identifier> ("{" {<struct-declaration>}* "}")?
-                                      | <struct-or-union>              "{" {<struct-declaration>}* "}"
+                                      | <struct-or-union>              "{" {<struct-declaration>}* "}" <GNU-attribute>?
         """
         if self.current_token.type not in self.cfirst_set.struct_or_union_specifier:
             self.error(ErrorCode.UNEXPECTED_TOKEN, "should be struct or union")
 
         node = Structure()
 
         node.update(structure_type=self.struct_or_union())
@@ -888,14 +888,17 @@
             node.update(declarations=struct_declarations)
             node.register_token(self.eat(TokenType.RCURLY_BRACE))
 
             # 匿名 struct 且未定义成员
             if len(struct_declarations) == 0 and node.id is None:
                 self.warning("unnamed struct/union that defines no instances", node)
         add_ast_type(node.id, C_CSS.STRUCTURE_CLASS)
+
+        if self.current_token.type == CTokenType._ATTRIBUTE:
+            node.update(gnu_attribute = self.gnu_c_attribute())
         return node
 
     def struct_or_union(self):
         """
         <struct-or-union> ::= "struct"
                             | "union"
         """
@@ -1026,14 +1029,16 @@
                               | "(" <declarator> ")"
                               | <direct-declarator> "[" <type-qualifier-list>? <assignment-expression>? "]"
                               | <direct-declarator> "[" static <type-qualifier-list>? <assignment-expression> "]"
                               | <direct-declarator> "[" <type-qualifier-list> static <assignment-expression> "]"
                               | <direct-declarator> "[" <type-qualifier-list>? "*" "]"
                               | <direct-declarator> "(" <parameter-list> ")"
                               | <direct-declarator> "(" (<identifier-list>)? ")"
+
+        <direct-declarator> <GNU-attribute>?
         """
         node = DirectDeclaractor()
         if self.current_token.type == TokenType.ID:
             node.update(id=self.identifier())
             # 对于初始化的变量去掉其 DefineName 的 tag
             if node.id.id in GDT and GDT[node.id.id] == CSS.MACRO_DEFINE:
                 delete_ast_type(node.id, CSS.MACRO_DEFINE)
@@ -1109,14 +1114,17 @@
                 elif self.current_token.type in self.cfirst_set.identifier:
                     sub_node.update(identifier_list=self.identifier_list())
                 node.register_token(self.eat(TokenType.RPAREN))
 
             sub_nodes.append(sub_node)
 
         node.update(sub_nodes=sub_nodes)
+
+        if self.current_token.type == CTokenType._ATTRIBUTE:
+            node.update(gnu_attribute = self.gnu_c_attribute())
         return node
 
     def type_qualifier_list(self) -> List[AST]:
         """
         <type-qualifier-list> ::= <type-qualifier>+
         """
         result = []
@@ -1274,19 +1282,19 @@
         @修改文法
         个人感觉这里存在问题, 对于 Person* ptr = &(Person) { "Bob", 30, { 50, 60 } }; 这里的 <type-name> 会被优先匹配到, 而不是匹配后面 <primary-expression> => "(" <type-name> ")" "{" <initializer-list> (",")? "}"
 
         所以这里做了一个对于 <initializer-list> 的补充
         """
         node = CastExpression()
         type_names = []
-        
-        '''
+
+        """
         @特殊处理
         对于强制类型转换 (uint64)trampoline (见 test/c/40.c)
-        '''
+        """
         while self.current_token.type == TokenType.LPAREN and (
             self.peek_next_token().type in self.cfirst_set.type_name or self._type_cast_check()
         ):
             if self.peek_next_token().type in self.cfirst_set.type_name:
                 node.register_token(self.eat(TokenType.LPAREN))
                 type_names.append(self.type_name())
                 node.register_token(self.eat(TokenType.RPAREN))
@@ -1307,29 +1315,35 @@
                 node.register_token(self.eat())
             node.register_token(self.eat(TokenType.RCURLY_BRACE))
         else:
             self.error(ErrorCode.UNEXPECTED_TOKEN, "should be unary expression or (")
         return node
 
     def _type_cast_check(self):
-        '''
+        """
         强制类型转换的情况
 
         (uint8) <unary-expression>
         (uint8 *) <unary-expression>
         (uint8 ****) <unary-expression>
-        '''
+        """
         if self.peek_next_token().type == TokenType.ID:
-            if self.peek_next_token(2).type == TokenType.RPAREN and self.peek_next_token(3).type in self.cfirst_set.unary_expression:
+            if (
+                self.peek_next_token(2).type == TokenType.RPAREN
+                and self.peek_next_token(3).type in self.cfirst_set.unary_expression
+            ):
                 return True
             elif self.peek_next_token(2).type == TokenType.MUL:
                 n = 3
                 while self.peek_next_token(n).type == TokenType.MUL:
                     n += 1
-                if self.peek_next_token(n).type == TokenType.RPAREN and self.peek_next_token(n+1).type in self.cfirst_set.unary_expression:
+                if (
+                    self.peek_next_token(n).type == TokenType.RPAREN
+                    and self.peek_next_token(n + 1).type in self.cfirst_set.unary_expression
+                ):
                     return True
 
         return False
 
     def unary_expression(self):
         """
         <unary-expression> ::= <postfix-expression>
@@ -1817,15 +1831,15 @@
     def declaration(self):
         """
         <declaration> ::= <declaration-specifier>+ (<init-declarator-list>)? ";"
                         | <static-assert-declaration>
 
         也有可能是 <function-definition>, 如果 <init-declarator-list> 的只有一个元素且没有 <initializer> 且后面跟着的是 <declaration>* <compound-statement>
 
-        <function-definition> ::= <declaration-specifier>* <declarator> <declaration>* <compound-statement>
+        <function-definition> ::= <declaration-specifier>* <declarator>  <GNU-attribute>? <declaration>* <compound-statement>
         """
         node = Declaration()
         if self.current_token.type in self.cfirst_set.static_assert_declaration:
             node.update(static_assert=self.static_assert_declaration())
             return node
 
         declaration_specifiers: List[AST] = [self.declaration_sepcifier()]
@@ -1865,14 +1879,16 @@
                 )
             else:
                 self.error(
                     ErrorCode.UNEXPECTED_TOKEN, "miss not declaration or function definition"
                 )
         if self.current_token.type == TokenType.SEMI:
             node.register_token(self.eat(TokenType.SEMI))
+        elif self.current_token.type == CTokenType._ATTRIBUTE:
+            node.update(gnu_attribute = self.gnu_c_attribute())
         else:
             self.error(ErrorCode.UNEXPECTED_TOKEN, "miss ;")
 
         return node
 
     def _is_C_function(self, init_declarator_list: List[InitDeclarator]):
         """
@@ -2223,24 +2239,25 @@
         node.register_token(self.eat(TokenType.SEMI))
         return node
 
     def gnu_c_statement_extension(self):
         """
         https://gcc.gnu.org/onlinedocs/gcc/Extended-Asm.html
 
-        <gnu-c-statement-extension> ::= __asm__ <asm-qualifiers> "(" <STRING>+ <OutputOperands >* ")"
+        <gnu-c-statement-extension> ::= (__asm__ | asm ) <asm-qualifiers> "(" <STRING>+ <OutputOperands >* ")"
 
         <asm-qualifiers> ::= volatile
                            | inline
                            | goto
 
         <OutputOperands> ::= ":" <STRING>? ( "(" <constant_expression> ")" ) ("," <STRING>? ( "(" <constant_expression> ")" ))*
         """
         node = GNU_C_Assembly()
-        node.update(keyword=self.get_keyword(CTokenType._ASM, css_type=C_CSS.GNU_C_EXTENSION))
+        assert self.current_token.type in self.cfirst_set.gnu_c_statement_extension
+        node.update(keyword=self.get_keyword(css_type=C_CSS.GNU_C_EXTENSION))
         if self.current_token.type in (CTokenType.VOLATILE, CTokenType.INLINE, CTokenType.GOTO):
             node.update(asm_qualifier=self.get_keyword(css_type=C_CSS.GNU_C_EXTENSION))
         node.register_token(self.eat(TokenType.LPAREN))
 
         while self.current_token.type == TokenType.STRING:
             self.string_inside_format()
 
@@ -2575,7 +2592,23 @@
             file_path.register_token([new_token])
             self.manual_register_token(new_token)
             node.update(file_path=file_path)
             node.register_token(self.eat(TokenType.RANGLE_BRACE))
         else:
             self.error(ErrorCode.UNEXPECTED_TOKEN, '<> or ""')
         return node
+
+
+    def gnu_c_attribute(self):
+        '''
+        GNU C Extension
+
+        __attribute__ "(" <expression> ")"
+        '''
+        # if self.current_token.type == CTokenType._ATTRIBUTE:
+        node = GNU_C_Assembly()
+        node.register_token(self.eat(CTokenType._ATTRIBUTE))
+        node.register_token(self.eat(TokenType.LPAREN))
+        node.update(expression = self.expression())
+        node.register_token(self.eat(TokenType.RPAREN))
+        return node
+
```

### Comparing `syntaxlight-0.1.7/syntaxlight/parsers/css_parser.py` & `syntaxlight-0.1.8/syntaxlight/parsers/css_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/parsers/json_parser.py` & `syntaxlight-0.1.8/syntaxlight/parsers/json_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/parsers/lua_parser.py` & `syntaxlight-0.1.8/syntaxlight/parsers/lua_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/parsers/makefile_parser.py` & `syntaxlight-0.1.8/syntaxlight/parsers/makefile_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/parsers/parser.py` & `syntaxlight-0.1.8/syntaxlight/parsers/parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/parsers/shell_parser.py` & `syntaxlight-0.1.8/syntaxlight/parsers/shell_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/parsers/toml_parser.py` & `syntaxlight-0.1.8/syntaxlight/parsers/toml_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/parsers/xml_parser.py` & `syntaxlight-0.1.8/syntaxlight/parsers/xml_parser.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/syntaxlight/syntax_parse.py` & `syntaxlight-0.1.8/syntaxlight/syntax_parse.py`

 * *Files identical despite different names*

### Comparing `syntaxlight-0.1.7/PKG-INFO` & `syntaxlight-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syntaxlight
-Version: 0.1.7
+Version: 0.1.8
 Summary: syntax highlight based on EBNF
 Home-page: https://github.com/luzhixing12345/syntaxlight
 License: MIT
 Author: luzhixing12345
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

