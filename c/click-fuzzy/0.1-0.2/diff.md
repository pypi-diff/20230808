# Comparing `tmp/click_fuzzy-0.1.tar.gz` & `tmp/click_fuzzy-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "click_fuzzy-0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "click_fuzzy-0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `click_fuzzy-0.1.tar` & `click_fuzzy-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      171 2023-08-02 06:19:31.025111 click_fuzzy-0.1/.flake8
--rw-r--r--   0        0        0     1818 2023-08-02 08:15:25.067426 click_fuzzy-0.1/.gitignore
--rw-r--r--   0        0        0      405 2023-08-02 08:45:35.195780 click_fuzzy-0.1/CHANGELOG.md
--rw-r--r--   0        0        0     5483 2023-08-02 06:20:06.656301 click_fuzzy-0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      626 2023-08-02 06:20:06.656500 click_fuzzy-0.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1066 2023-08-02 06:20:06.656663 click_fuzzy-0.1/LICENSE
--rw-r--r--   0        0        0      818 2023-08-02 08:25:00.951978 click_fuzzy-0.1/README.md
--rw-r--r--   0        0        0      250 2023-08-02 08:15:50.446889 click_fuzzy-0.1/click_fuzzy/__init__.py
--rw-r--r--   0        0        0      154 2023-08-02 08:45:35.202096 click_fuzzy-0.1/click_fuzzy/__version__.py
--rw-r--r--   0        0        0     1784 2023-08-02 08:44:05.415223 click_fuzzy-0.1/click_fuzzy/core.py
--rw-r--r--   0        0        0       90 2023-08-02 08:15:50.445502 click_fuzzy-0.1/click_fuzzy/tests/__init__.py
--rw-r--r--   0        0        0     4089 2023-08-02 08:44:01.041472 click_fuzzy-0.1/click_fuzzy/tests/smoke.py
--rw-r--r--   0        0        0      547 2023-08-02 08:16:53.978712 click_fuzzy-0.1/makefile
--rw-r--r--   0        0        0      834 2023-08-02 08:29:00.507605 click_fuzzy-0.1/pyproject.toml
--rw-r--r--   0        0        0     1487 1970-01-01 00:00:00.000000 click_fuzzy-0.1/PKG-INFO
+-rw-r--r--   0        0        0      171 2023-08-02 06:19:31.025111 click_fuzzy-0.2/.flake8
+-rw-r--r--   0        0        0     1818 2023-08-02 08:15:25.067426 click_fuzzy-0.2/.gitignore
+-rw-r--r--   0        0        0      624 2023-08-08 06:07:08.632119 click_fuzzy-0.2/CHANGELOG.md
+-rw-r--r--   0        0        0     5483 2023-08-02 06:20:06.656301 click_fuzzy-0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      626 2023-08-02 06:20:06.656500 click_fuzzy-0.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1066 2023-08-02 06:20:06.656663 click_fuzzy-0.2/LICENSE
+-rw-r--r--   0        0        0     1298 2023-08-08 05:52:49.121397 click_fuzzy-0.2/README.md
+-rw-r--r--   0        0        0      428 2023-08-08 05:51:56.522722 click_fuzzy-0.2/click_fuzzy/__init__.py
+-rw-r--r--   0        0        0      154 2023-08-08 06:07:08.638183 click_fuzzy-0.2/click_fuzzy/__version__.py
+-rw-r--r--   0        0        0     5342 2023-08-08 05:42:53.470459 click_fuzzy-0.2/click_fuzzy/core.py
+-rw-r--r--   0        0        0       90 2023-08-02 08:15:50.445502 click_fuzzy-0.2/click_fuzzy/tests/__init__.py
+-rw-r--r--   0        0        0     4376 2023-08-08 05:53:28.777371 click_fuzzy-0.2/click_fuzzy/tests/smoke.py
+-rw-r--r--   0        0        0      547 2023-08-02 08:16:53.978712 click_fuzzy-0.2/makefile
+-rw-r--r--   0        0        0      898 2023-08-08 06:05:51.313133 click_fuzzy-0.2/pyproject.toml
+-rw-r--r--   0        0        0     2027 1970-01-01 00:00:00.000000 click_fuzzy-0.2/PKG-INFO
```

### Comparing `click_fuzzy-0.1/.gitignore` & `click_fuzzy-0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `click_fuzzy-0.1/CODE_OF_CONDUCT.md` & `click_fuzzy-0.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `click_fuzzy-0.1/CONTRIBUTING.md` & `click_fuzzy-0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `click_fuzzy-0.1/LICENSE` & `click_fuzzy-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `click_fuzzy-0.1/click_fuzzy/tests/smoke.py` & `click_fuzzy-0.2/click_fuzzy/tests/smoke.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,56 +14,65 @@
 @click.version_option("1.2.3")
 @click.pass_context
 def main(ctx: click.Context) -> None:
     pass
 
 
 @main.command("hello")
-@click.argument("name", type=str)
-def hello(name: str) -> None:
-    click.echo(f"hello {name}")
+@main.alias("hi")
+def hello() -> None:
+    """The traditional greeting"""
+    click.echo("hello there")
 
 
 @main.command("howdy")
 def howdy() -> None:
+    """Say hello the cowboy way"""
     click.echo("howdy partner")
 
 
 @main.command("bonjour")
 def bonjour() -> None:
+    """Like you might say in French class"""
     click.echo("bonjour mon ami")
 
 
 class SmokeTest(TestCase):
     def setUp(self) -> None:
         self.runner = click.testing.CliRunner(mix_stderr=False)
+        FuzzyCommandGroup.WARN_ON_PREFIX_MATCH = True
+        FuzzyCommandGroup.WARN_ON_FUZZY_MATCH = True
 
     def test_version(self) -> None:
         result = self.runner.invoke(main, "--version", catch_exceptions=False)
         self.assertIn("version 1.2.3", result.stdout)
         self.assertEqual("", result.stderr)
         self.assertEqual(result.exit_code, 0)
 
+    def test_help(self) -> None:
+        result = self.runner.invoke(main, "--help", catch_exceptions=False)
+        self.assertRegex(result.stdout, r"hello, hi\s+The traditional greeting")
+
     def test_direct(self) -> None:
-        result = self.runner.invoke(main, ["hello", "cutie"], catch_exceptions=False)
-        self.assertEqual("hello cutie\n", result.stdout)
+        result = self.runner.invoke(main, ["hello"], catch_exceptions=False)
+        self.assertIn("hello there", result.stdout)
         self.assertEqual("", result.stderr)
         self.assertEqual(result.exit_code, 0)
 
     def test_ambiguous_prefix(self) -> None:
         result = self.runner.invoke(main, ["h"], catch_exceptions=False)
         self.assertIn("Error: 'h' is not a command", result.stderr)
-        self.assertIn("Similar commands:\n  hello\n  howdy", result.stderr)
+        self.assertIn("Similar commands:\n  hello\n  hi\n  howdy", result.stderr)
         self.assertEqual(result.exit_code, 2)
 
     def test_definitive_prefix(self) -> None:
         with self.subTest("he"):
-            result = self.runner.invoke(main, ["he", "cutie"], catch_exceptions=False)
+            result = self.runner.invoke(main, ["he"], catch_exceptions=False)
             self.assertIn("Warning: Assuming 'he' is short for 'hello'", result.stderr)
-            self.assertIn("hello cutie", result.stdout)
+            self.assertIn("hello there", result.stdout)
             self.assertEqual(result.exit_code, 0)
 
         with self.subTest("how"):
             result = self.runner.invoke(main, ["how"], catch_exceptions=False)
             self.assertIn("Warning: Assuming 'how' is short for 'howdy'", result.stderr)
             self.assertIn("howdy partner", result.stdout)
             self.assertEqual(result.exit_code, 0)
@@ -72,31 +81,27 @@
             result = self.runner.invoke(main, ["b"], catch_exceptions=False)
             self.assertIn("Warning: Assuming 'b' is short for 'bonjour'", result.stderr)
             self.assertIn("bonjour mon ami", result.stdout)
             self.assertEqual(result.exit_code, 0)
 
     def test_misspelling(self) -> None:
         with self.subTest("helo"):
-            result = self.runner.invoke(
-                main, ["helo", "mother"], catch_exceptions=False
-            )
+            result = self.runner.invoke(main, ["helo"], catch_exceptions=False)
             self.assertIn(
                 "Warning: Assuming 'helo' is slang for 'hello'", result.stderr
             )
-            self.assertIn("hello mother", result.stdout)
+            self.assertIn("hello there", result.stdout)
             self.assertEqual(result.exit_code, 0)
 
         with self.subTest("helol"):
-            result = self.runner.invoke(
-                main, ["helol", "father"], catch_exceptions=False
-            )
+            result = self.runner.invoke(main, ["helol"], catch_exceptions=False)
             self.assertIn(
                 "Warning: Assuming 'helol' is slang for 'hello'", result.stderr
             )
-            self.assertIn("hello father", result.stdout)
+            self.assertIn("hello there", result.stdout)
             self.assertEqual(result.exit_code, 0)
 
         with self.subTest("rowdy"):
             result = self.runner.invoke(main, ["rowdy"], catch_exceptions=False)
             self.assertIn(
                 "Warning: Assuming 'rowdy' is slang for 'howdy'", result.stderr
             )
```

### Comparing `click_fuzzy-0.1/makefile` & `click_fuzzy-0.2/makefile`

 * *Files identical despite different names*

### Comparing `click_fuzzy-0.1/pyproject.toml` & `click_fuzzy-0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -6,28 +6,31 @@
 name = "click-fuzzy"
 readme = "README.md"
 authors = [
     {name="Amethyst Reese", email="amethyst@n7.gg"},
 ]
 license = {file="LICENSE"}
 dynamic = ["version", "description"]
+classifiers = [
+    "License :: OSI Approved :: MIT License",
+]
 requires-python = ">=3.8"
 dependencies = [
     "click >= 8",
     "editdistance >= 0.6",
 ]
 
 [project.optional-dependencies]
 dev = [
     "attribution==1.6.2",
-    "black==23.3.0",
-    "flake8==6.0.0",
-    "flit==3.8.0",
-    "mypy==1.2.0",
-    "ufmt==2.0.1",
+    "black==23.7.0",
+    "flake8==6.1.0",
+    "flit==3.9.0",
+    "mypy==1.4.1",
+    "ufmt==2.2.0",
     "usort==1.0.6",
 ]
 
 [project.urls]
 Home = "https://github.com/amyreese/click-fuzzy"
 
 [tool.flit.sdist]
```

