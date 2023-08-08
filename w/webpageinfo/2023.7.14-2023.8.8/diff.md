# Comparing `tmp/webpageinfo-2023.7.14.tar.gz` & `tmp/webpageinfo-2023.8.8.tar.gz`

## Comparing `webpageinfo-2023.7.14.tar` & `webpageinfo-2023.8.8.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/.pre-commit-config.yaml
--rw-r--r--   0        0        0    83903 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/poetry.lock
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/webpageinfo/__init__.py
--rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/webpageinfo/browser.py
--rw-r--r--   0        0        0     9557 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/webpageinfo/page.py
--rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/webpageinfo/safe_html.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/webpageinfo/config/__init__.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/webpageinfo/config/ignored_html_tags.py
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/webpageinfo/config/ignored_word_in_tags.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/webpageinfo/config/rejected_content_class.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/webpageinfo/config/rejected_content_id.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/webpageinfo/config/removed_html_tags.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/webpageinfo/config/simple_html_tags.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/webpageinfo/config/svg_tags.py
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/.gitignore
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/LICENSE
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/README.md
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/pyproject.toml
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 webpageinfo-2023.7.14/PKG-INFO
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 webpageinfo-2023.8.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 webpageinfo-2023.8.8/webpageinfo/__init__.py
+-rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 webpageinfo-2023.8.8/webpageinfo/browser.py
+-rw-r--r--   0        0        0     9612 2020-02-02 00:00:00.000000 webpageinfo-2023.8.8/webpageinfo/page.py
+-rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 webpageinfo-2023.8.8/webpageinfo/safe_html.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 webpageinfo-2023.8.8/webpageinfo/config/__init__.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 webpageinfo-2023.8.8/webpageinfo/config/ignored_html_tags.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 webpageinfo-2023.8.8/webpageinfo/config/ignored_word_in_tags.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 webpageinfo-2023.8.8/webpageinfo/config/rejected_content_class.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 webpageinfo-2023.8.8/webpageinfo/config/rejected_content_id.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 webpageinfo-2023.8.8/webpageinfo/config/removed_html_tags.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 webpageinfo-2023.8.8/webpageinfo/config/simple_html_tags.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 webpageinfo-2023.8.8/webpageinfo/config/svg_tags.py
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 webpageinfo-2023.8.8/.gitignore
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 webpageinfo-2023.8.8/LICENSE
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 webpageinfo-2023.8.8/README.md
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 webpageinfo-2023.8.8/pyproject.toml
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 webpageinfo-2023.8.8/PKG-INFO
```

### Comparing `webpageinfo-2023.7.14/.pre-commit-config.yaml` & `webpageinfo-2023.8.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `webpageinfo-2023.7.14/webpageinfo/browser.py` & `webpageinfo-2023.8.8/webpageinfo/browser.py`

 * *Files identical despite different names*

### Comparing `webpageinfo-2023.7.14/webpageinfo/page.py` & `webpageinfo-2023.8.8/webpageinfo/page.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,16 @@
     def to_absolute_url(self, url: str) -> str:
         if url.startswith("/"):
             return self.server + url
         if url.startswith(("#", "?")):
             return (
                 self.url + url
             )  # TODO remove fragment + query from self.url (urlparse)
-        return url.replace("http://", "https://")
+        # return url.replace("http://", "https://") # some sites don't support HTTPS!
+        return url
 
     @property
     def attached_pdf(self) -> Iterable[str]:
         return [
             self.to_absolute_url(link) for link in self.links if link.endswith(".pdf")
         ]
```

### Comparing `webpageinfo-2023.7.14/webpageinfo/safe_html.py` & `webpageinfo-2023.8.8/webpageinfo/safe_html.py`

 * *Files identical despite different names*

### Comparing `webpageinfo-2023.7.14/webpageinfo/config/ignored_word_in_tags.py` & `webpageinfo-2023.8.8/webpageinfo/config/ignored_word_in_tags.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 ignored_word_in_tags = {
     "about",
     "alors",
     "anc",
     "apprenants",
     "auprès",
     "aussi",
-    "avec",
     "available",
+    "avec",
+    "avez",
     "avoir",
+    "avons",
     "beaucoup",
     "beau",
     "beaux",
     "belle",
     "belles",
     "bon",
     "bonne",
@@ -24,26 +26,29 @@
     "comme",
     "créé",
     "créée",
     "dans",
     "default",
     "des",
     "different",
+    "difficilement",
     "directory",
     "elle",
     "elles",
+    "entre",
     "est",
     "était",
     "example",
     "exemple",
     "faire",
     "faite",
     "faites",
     "fait",
     "faits",
+    "faut",
     "first",
     "following",
     "for",
     "from",
     "grâce",
     "how",
     "however",
@@ -62,14 +67,16 @@
     "name",
     "named",
     "never",
     "note",
     "notre",
     "other",
     "parce",
+    "partiellement",
+    "pdf",
     "petit",
     "petits",
     "petite",
     "petites",
     "plus",
     "pour",
     "project",
@@ -92,14 +99,16 @@
     "that",
     "the",
     "there",
     "these",
     "this",
     "tous",
     "tout",
+    "toute",
+    "toutes",
     "un",
     "une",
     "use",
     "using",
     "version",
     "votre",
     "voulez",
```

### Comparing `webpageinfo-2023.7.14/.gitignore` & `webpageinfo-2023.8.8/.gitignore`

 * *Files identical despite different names*

### Comparing `webpageinfo-2023.7.14/LICENSE` & `webpageinfo-2023.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `webpageinfo-2023.7.14/pyproject.toml` & `webpageinfo-2023.8.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "webpageinfo"
-version = "2023.7.14"
+version = "2023.8.8"
 description = "Web page information (title, content, tags…)"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
@@ -22,44 +22,32 @@
     "httpx >=0,<1",
     "pdfminer.six == 20220524",
     "pillow >=9,<10",
     "splinter[selenium4] >=0,<1",
 ]
 
 [project.optional-dependencies]
-dev = [
-    "python-dev-tools >= 2023",
-    "pre-commit >=3,<4",
-]
+dev = ["python-dev-tools >= 2023", "pre-commit >=3,<4"]
 
 [project.urls]
 "Source code" = "https://github.com/vpoulailleau/webpageinfo"
 Repository = "https://github.com/vpoulailleau/webpageinfo"
 Documentation = "https://webpageinfo.readthedocs.io/en/latest/"
 
 [tool.hatch.build.targets.sdist]
-exclude = [
-  ".gitignore",
-  "/.github",
-  "/docs",
-]
+exclude = [".gitignore", "/.github", "/docs"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["webpageinfo"]
 
 
 [tool.pytest.ini_options]
 minversion = "7.0"
 addopts = "-ra -q  -s -vv --cov=webpageinfo"
-testpaths = [
-    "tests",
-]
+testpaths = ["tests"]
 
 [tool.coverage.report]
-exclude_lines = [
-    "pragma: no cover",
-    "if TYPE_CHECKING:",
-]
+exclude_lines = ["pragma: no cover", "if TYPE_CHECKING:"]
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
```

### Comparing `webpageinfo-2023.7.14/PKG-INFO` & `webpageinfo-2023.8.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webpageinfo
-Version: 2023.7.14
+Version: 2023.8.8
 Summary: Web page information (title, content, tags…)
 Project-URL: Source code, https://github.com/vpoulailleau/webpageinfo
 Project-URL: Repository, https://github.com/vpoulailleau/webpageinfo
 Project-URL: Documentation, https://webpageinfo.readthedocs.io/en/latest/
 Author-email: Vincent Poulailleau <vpoulailleau@gmail.com>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
```

