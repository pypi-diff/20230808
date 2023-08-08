# Comparing `tmp/psbs-0.2.3.tar.gz` & `tmp/psbs-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psbs-0.2.3.tar", last modified: Mon Aug  7 15:17:45 2023, max compression
+gzip compressed data, was "psbs-0.3.0.tar", last modified: Tue Aug  8 19:42:01 2023, max compression
```

## Comparing `psbs-0.2.3.tar` & `psbs-0.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-08-07 15:17:45.232893 psbs-0.2.3/
--rw-r--r--   0 jcmiller   (501) staff       (20)     1069 2023-06-04 01:40:38.000000 psbs-0.2.3/LICENSE
--rw-r--r--   0 jcmiller   (501) staff       (20)     6737 2023-08-07 15:17:45.233142 psbs-0.2.3/PKG-INFO
--rw-r--r--   0 jcmiller   (501) staff       (20)     6065 2023-08-04 20:30:44.000000 psbs-0.2.3/README.md
-drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-08-07 15:17:45.225998 psbs-0.2.3/psbs/
--rw-r--r--   0 jcmiller   (501) staff       (20)        0 2023-06-05 12:31:00.000000 psbs-0.2.3/psbs/__init__.py
--rw-r--r--   0 jcmiller   (501) staff       (20)       32 2023-06-11 15:36:36.000000 psbs-0.2.3/psbs/__main__.py
--rw-r--r--   0 jcmiller   (501) staff       (20)      383 2023-07-23 20:27:08.000000 psbs-0.2.3/psbs/config.py
--rw-r--r--   0 jcmiller   (501) staff       (20)      870 2023-07-29 00:01:45.000000 psbs-0.2.3/psbs/example.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)     1614 2023-08-04 01:50:46.000000 psbs-0.2.3/psbs/extension.py
-drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-08-07 15:17:45.231926 psbs-0.2.3/psbs/extensions/
--rw-r--r--   0 jcmiller   (501) staff       (20)        0 2023-06-18 20:00:51.000000 psbs-0.2.3/psbs/extensions/__init__.py
--rw-r--r--   0 jcmiller   (501) staff       (20)      568 2023-08-04 01:50:46.000000 psbs-0.2.3/psbs/extensions/build.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     1399 2023-08-07 15:09:24.000000 psbs-0.2.3/psbs/extensions/filters.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     3069 2023-08-04 01:50:46.000000 psbs-0.2.3/psbs/extensions/images.py
--rw-r--r--   0 jcmiller   (501) staff       (20)    20733 2023-08-04 01:50:46.000000 psbs-0.2.3/psbs/extensions/tiled.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     2916 2023-08-04 18:52:17.000000 psbs-0.2.3/psbs/gister.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     1820 2023-08-06 15:04:23.000000 psbs-0.2.3/psbs/htmlbuilder.py
--rwxr-xr-x   0 jcmiller   (501) staff       (20)     4301 2023-08-06 14:09:41.000000 psbs-0.2.3/psbs/project.py
--rwxr-xr-x   0 jcmiller   (501) staff       (20)     2944 2023-08-06 14:10:04.000000 psbs-0.2.3/psbs/psbs.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     9382 2023-08-06 15:00:57.000000 psbs-0.2.3/psbs/psparser.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     3086 2023-08-07 15:12:48.000000 psbs-0.2.3/psbs/template.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     1118 2023-08-04 23:04:04.000000 psbs-0.2.3/psbs/token.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     1945 2023-06-14 18:47:43.000000 psbs-0.2.3/psbs/utils.py
-drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-08-07 15:17:45.229307 psbs-0.2.3/psbs.egg-info/
--rw-r--r--   0 jcmiller   (501) staff       (20)     6737 2023-08-07 15:17:45.000000 psbs-0.2.3/psbs.egg-info/PKG-INFO
--rw-r--r--   0 jcmiller   (501) staff       (20)      547 2023-08-07 15:17:45.000000 psbs-0.2.3/psbs.egg-info/SOURCES.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)        1 2023-08-07 15:17:45.000000 psbs-0.2.3/psbs.egg-info/dependency_links.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)       40 2023-08-07 15:17:45.000000 psbs-0.2.3/psbs.egg-info/entry_points.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)       49 2023-08-07 15:17:45.000000 psbs-0.2.3/psbs.egg-info/requires.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)        5 2023-08-07 15:17:45.000000 psbs-0.2.3/psbs.egg-info/top_level.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)      103 2023-08-07 15:17:45.233859 psbs-0.2.3/setup.cfg
--rw-r--r--   0 jcmiller   (501) staff       (20)     1277 2023-08-07 15:15:53.000000 psbs-0.2.3/setup.py
+drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-08-08 19:42:01.004675 psbs-0.3.0/
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1069 2023-06-04 01:40:38.000000 psbs-0.3.0/LICENSE
+-rw-r--r--   0 jcmiller   (501) staff       (20)     6737 2023-08-08 19:42:01.004915 psbs-0.3.0/PKG-INFO
+-rw-r--r--   0 jcmiller   (501) staff       (20)     6065 2023-08-04 20:30:44.000000 psbs-0.3.0/README.md
+drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-08-08 19:42:00.997680 psbs-0.3.0/psbs/
+-rw-r--r--   0 jcmiller   (501) staff       (20)        0 2023-06-05 12:31:00.000000 psbs-0.3.0/psbs/__init__.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)       32 2023-06-11 15:36:36.000000 psbs-0.3.0/psbs/__main__.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)      383 2023-08-08 17:13:52.000000 psbs-0.3.0/psbs/config.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)      870 2023-07-29 00:01:45.000000 psbs-0.3.0/psbs/example.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)     2118 2023-08-08 19:35:35.000000 psbs-0.3.0/psbs/extension.py
+drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-08-08 19:42:01.003845 psbs-0.3.0/psbs/extensions/
+-rw-r--r--   0 jcmiller   (501) staff       (20)        0 2023-06-18 20:00:51.000000 psbs-0.3.0/psbs/extensions/__init__.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)      568 2023-08-04 01:50:46.000000 psbs-0.3.0/psbs/extensions/build.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     2597 2023-08-08 19:37:05.000000 psbs-0.3.0/psbs/extensions/filters.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     3069 2023-08-04 01:50:46.000000 psbs-0.3.0/psbs/extensions/images.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)    20733 2023-08-04 01:50:46.000000 psbs-0.3.0/psbs/extensions/tiled.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     2916 2023-08-04 18:52:17.000000 psbs-0.3.0/psbs/gister.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1820 2023-08-06 15:04:23.000000 psbs-0.3.0/psbs/htmlbuilder.py
+-rwxr-xr-x   0 jcmiller   (501) staff       (20)     4451 2023-08-08 19:35:35.000000 psbs-0.3.0/psbs/project.py
+-rwxr-xr-x   0 jcmiller   (501) staff       (20)     3307 2023-08-08 19:35:35.000000 psbs-0.3.0/psbs/psbs.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     9376 2023-08-08 13:27:52.000000 psbs-0.3.0/psbs/psparser.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     3223 2023-08-08 19:35:35.000000 psbs-0.3.0/psbs/template.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1118 2023-08-04 23:04:04.000000 psbs-0.3.0/psbs/token.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     3005 2023-08-08 19:35:35.000000 psbs-0.3.0/psbs/utils.py
+drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-08-08 19:42:01.000824 psbs-0.3.0/psbs.egg-info/
+-rw-r--r--   0 jcmiller   (501) staff       (20)     6737 2023-08-08 19:42:00.000000 psbs-0.3.0/psbs.egg-info/PKG-INFO
+-rw-r--r--   0 jcmiller   (501) staff       (20)      547 2023-08-08 19:42:00.000000 psbs-0.3.0/psbs.egg-info/SOURCES.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)        1 2023-08-08 19:42:00.000000 psbs-0.3.0/psbs.egg-info/dependency_links.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)       40 2023-08-08 19:42:00.000000 psbs-0.3.0/psbs.egg-info/entry_points.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)       59 2023-08-08 19:42:00.000000 psbs-0.3.0/psbs.egg-info/requires.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)        5 2023-08-08 19:42:00.000000 psbs-0.3.0/psbs.egg-info/top_level.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)      103 2023-08-08 19:42:01.005511 psbs-0.3.0/setup.cfg
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1298 2023-08-08 19:38:38.000000 psbs-0.3.0/setup.py
```

### Comparing `psbs-0.2.3/LICENSE` & `psbs-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `psbs-0.2.3/PKG-INFO` & `psbs-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: psbs
-Version: 0.2.3
+Version: 0.3.0
 Summary: PuzzleScript Build System
 Home-page: https://github.com/jcmiller11/PSBS
-Download-URL: https://github.com/jcmiller11/PSBS/archive/refs/tags/0.2.3.tar.gz
+Download-URL: https://github.com/jcmiller11/PSBS/archive/refs/tags/0.3.0.tar.gz
 Author: J.C. Miller
 Author-email: johncoreymiller@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `psbs-0.2.3/README.md` & `psbs-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `psbs-0.2.3/psbs/example.txt` & `psbs-0.3.0/psbs/example.txt`

 * *Files identical despite different names*

### Comparing `psbs-0.2.3/psbs/extensions/build.py` & `psbs-0.3.0/psbs/extensions/build.py`

 * *Files identical despite different names*

### Comparing `psbs-0.2.3/psbs/extensions/images.py` & `psbs-0.3.0/psbs/extensions/images.py`

 * *Files identical despite different names*

### Comparing `psbs-0.2.3/psbs/extensions/tiled.py` & `psbs-0.3.0/psbs/extensions/tiled.py`

 * *Files identical despite different names*

### Comparing `psbs-0.2.3/psbs/gister.py` & `psbs-0.3.0/psbs/gister.py`

 * *Files identical despite different names*

### Comparing `psbs-0.2.3/psbs/htmlbuilder.py` & `psbs-0.3.0/psbs/htmlbuilder.py`

 * *Files identical despite different names*

### Comparing `psbs-0.2.3/psbs/project.py` & `psbs-0.3.0/psbs/project.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,23 +4,30 @@
 
 from .config import Config
 from .extension import Extension
 from .htmlbuilder import build_html
 from .gister import Gister
 from .psparser import PSParser
 from .template import Template
-from .utils import read_file, write_file, write_yaml, make_dir, run_in_browser
+from .utils import (
+    read_file,
+    write_file,
+    write_yaml,
+    make_dir,
+    run_in_browser,
+    print_ps_console,
+)
 
 
 class PSBSProject:
     def __init__(self, config_filename="config.yaml"):
         self.config = Config(config_filename)
         self.filename = None
 
-    def build(self):
+    def build(self, verbose=False):
         # Check for target directory
         if not path.exists("bin"):
             print("bin directory does not exist, creating one")
             make_dir("bin")
 
         readme_path = path.join("bin", "readme.txt")
         script_path = path.join("bin", "script.txt")
@@ -31,20 +38,22 @@
             readme_path,
             "Play this game by pasting the script in "
             f"{self.config['engine']}editor.html",
         )
 
         # Build the script.txt
         print("Building script.txt")
-        template = Template(
+        source = Template(
             path.join("src", self.config["template"]), self.config
-        )
+        ).render()
 
         print(f"Writing file {script_path}")
-        write_file(script_path, template.render())
+        write_file(script_path, source)
+        if verbose:
+            print_ps_console(source)
 
     def export(self):
         if not self.config["gist_id"]:
             print("Writing game to html file")
             self.filename = build_html(
                 self.config["engine"],
                 read_file(path.join("bin", "script.txt")),
@@ -92,14 +101,15 @@
             gist = Gister()
             gist_id = gist.create(name=project_name)
 
         config_dict = {
             "gist_id": gist_id,
             "engine": engine,
             "template": "main.pss",
+            "user_extensions": [],
         }
         config_dict.update(Extension.get_extension_configs())
 
         print("Building directory structure")
         make_dir(project_name)
         try:
             make_dir(path.join(project_name, "src"))
```

### Comparing `psbs-0.2.3/psbs/psbs.py` & `psbs-0.3.0/psbs/psbs.py`

 * *Files 7% similar despite different names*

```diff
@@ -66,26 +66,38 @@
         "topic",
         nargs="?",
         choices=list(commands.keys()),
         help="Select command you would like help with",
         type=str,
     )
 
+    for verbosible_command in [
+        commands["build"],
+        commands["run"],
+        commands["export"],
+    ]:
+        verbosible_command.add_argument(
+            "--verbose",
+            "-v",
+            help="Display PuzzleScript console output",
+            action="store_true",
+        )
+
     args = parser.parse_args()
 
     if args.command == "build":
         project = PSBSProject()
-        project.build()
+        project.build(verbose=args.verbose)
     elif args.command == "export":
         project = PSBSProject()
-        project.build()
+        project.build(verbose=args.verbose)
         project.export()
     elif args.command == "run":
         project = PSBSProject()
-        project.build()
+        project.build(verbose=args.verbose)
         project.export()
         project.run(editor=args.editor)
     elif args.command == "new":
         PSBSProject.create(
             args.name,
             gist_id=args.gist_id,
             file=args.file,
```

### Comparing `psbs-0.2.3/psbs/psparser.py` & `psbs-0.3.0/psbs/psparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             if len(tokens) == 2:
                 self.prelude_options[tokens[0].lower()] = tokens[1]
 
     class ParseError(Exception):
         """Thrown when unable to parse the input PS"""
 
     @staticmethod
-    def __redact_comments(input_str, redact_char=" "):
+    def redact_comments(input_str, redact_char=" "):
         depth = 0
         output = ""
         in_a_message = False
         for character in input_str:
             if output[-8:].lower() == "message ":
                 in_a_message = True
             if character == "\n":
@@ -38,15 +38,15 @@
             if character == ")" and not in_a_message:
                 depth -= 1
             depth = max(depth, 0)
         return output
 
     @staticmethod
     def __clean(input_str):
-        input_str = PSParser.__redact_comments(input_str, redact_char="")
+        input_str = PSParser.redact_comments(input_str, redact_char="")
         output = "\n".join([line.strip() for line in input_str.splitlines()])
         return output
 
     @staticmethod
     def get_engine(input_str):
         match = re.search(r"(http.*)(?:editor\.html)", input_str)
         return match.group(1) if match else "https://www.puzzlescript.net/"
@@ -64,15 +64,15 @@
             "winconditions": [],
             "levels": [],
         }
         optional_sections = ["tags", "mappings"]
         section_headers = list(sections.keys())[1:]
         headers = re.finditer(
             r"^(" + "|".join(section_headers) + ") *$",
-            PSParser.__redact_comments(self.source),
+            PSParser.redact_comments(self.source),
             flags=re.IGNORECASE | re.MULTILINE,
         )
 
         section = "prelude"
         start = 0
         for header in headers:
             content = self.source[start : header.span()[0]]
```

### Comparing `psbs-0.2.3/psbs/template.py` & `psbs-0.3.0/psbs/template.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,18 +13,21 @@
             autoescape=False,
             block_start_string="(%",
             block_end_string="%)",
             variable_start_string="((",
             variable_end_string="))",
             comment_start_string="(#",
             comment_end_string="#)",
-            extensions=['jinja2.ext.do'],
+            extensions=["jinja2.ext.do"],
+            trim_blocks=True,
+            lstrip_blocks=True,
         )
         self.postprocessing_steps = []
-        extensions = Extension.get_extensions()
+        user_extensions = config.get("user_extensions", [])
+        extensions = Extension.get_extensions(user_extensions)
         for extension in extensions:
             if extension.__name__ not in config:
                 config[extension.__name__] = {}
             ext_object = extension(config[extension.__name__])
             for func_name, function in ext_object.methods.items():
                 self.jinja_env.globals[func_name] = function
             for func_name, function in ext_object.filters.items():
```

### Comparing `psbs-0.2.3/psbs/token.py` & `psbs-0.3.0/psbs/token.py`

 * *Files identical despite different names*

### Comparing `psbs-0.2.3/psbs.egg-info/PKG-INFO` & `psbs-0.3.0/psbs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: psbs
-Version: 0.2.3
+Version: 0.3.0
 Summary: PuzzleScript Build System
 Home-page: https://github.com/jcmiller11/PSBS
-Download-URL: https://github.com/jcmiller11/PSBS/archive/refs/tags/0.2.3.tar.gz
+Download-URL: https://github.com/jcmiller11/PSBS/archive/refs/tags/0.3.0.tar.gz
 Author: J.C. Miller
 Author-email: johncoreymiller@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `psbs-0.2.3/psbs.egg-info/SOURCES.txt` & `psbs-0.3.0/psbs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

