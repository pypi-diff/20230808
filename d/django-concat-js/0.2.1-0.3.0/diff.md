# Comparing `tmp/django_concat_js-0.2.1.tar.gz` & `tmp/django_concat_js-0.3.0.tar.gz`

## Comparing `django_concat_js-0.2.1.tar` & `django_concat_js-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/tox.ini
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/__about__.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/__init__.py
--rw-r--r--   0        0        0    14068 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/dep_graph.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/settings.py
--rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/watch_src.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/management/commands/__init__.py
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/management/commands/watch_js.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/test_app/__init__.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/test_app/concat.json
--rwxr-xr-x   0        0        0      674 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/test_app/manage.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/test_app/settings.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/test_app/settings_base.py
--rw-r--r--   0        0        0     9463 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/test_app/tests.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/test_app/urls.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/test_app/wsgi.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/test_app/static/src/s1.js
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/test_app/static/src/s2.js
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/test_app/static/src/s3.js
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/concat_js/test_app/static/src/s4.js
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/.gitignore
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/LICENSE.txt
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/README.md
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4021 2020-02-02 00:00:00.000000 django_concat_js-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 django_concat_js-0.3.0/pypi-token
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 django_concat_js-0.3.0/tox.ini
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 django_concat_js-0.3.0/concat_js/__about__.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 django_concat_js-0.3.0/concat_js/__init__.py
+-rw-r--r--   0        0        0    14596 2020-02-02 00:00:00.000000 django_concat_js-0.3.0/concat_js/dep_graph.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 django_concat_js-0.3.0/concat_js/settings.py
+-rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 django_concat_js-0.3.0/concat_js/watch_src.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_concat_js-0.3.0/concat_js/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_concat_js-0.3.0/concat_js/management/commands/__init__.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 django_concat_js-0.3.0/concat_js/management/commands/watch_js.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 django_concat_js-0.3.0/concat_js/test_app/__init__.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 django_concat_js-0.3.0/concat_js/test_app/concat.json
+-rwxr-xr-x   0        0        0      674 2020-02-02 00:00:00.000000 django_concat_js-0.3.0/concat_js/test_app/manage.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 django_concat_js-0.3.0/concat_js/test_app/settings.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 django_concat_js-0.3.0/concat_js/test_app/settings_base.py
+-rw-r--r--   0        0        0     9463 2020-02-02 00:00:00.000000 django_concat_js-0.3.0/concat_js/test_app/tests.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 django_concat_js-0.3.0/concat_js/test_app/urls.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 django_concat_js-0.3.0/concat_js/test_app/wsgi.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 django_concat_js-0.3.0/concat_js/test_app/static/src/s1.js
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_concat_js-0.3.0/concat_js/test_app/static/src/s2.js
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 django_concat_js-0.3.0/concat_js/test_app/static/src/s3.js
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_concat_js-0.3.0/concat_js/test_app/static/src/s4.js
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 django_concat_js-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 django_concat_js-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 django_concat_js-0.3.0/README.md
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 django_concat_js-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4021 2020-02-02 00:00:00.000000 django_concat_js-0.3.0/PKG-INFO
```

### Comparing `django_concat_js-0.2.1/tox.ini` & `django_concat_js-0.3.0/tox.ini`

 * *Files identical despite different names*

### Comparing `django_concat_js-0.2.1/concat_js/dep_graph.py` & `django_concat_js-0.3.0/concat_js/dep_graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,24 +158,29 @@
         self.printer = printer
         self.extra_files = set([conf.JSON_DEPS])
         self.lint_js = conf.LINT_COMMAND
         self.create_sourcemaps = conf.CREATE_SOURCEMAPS
     
     def reload(self, json_file : Union[Path, str]=conf.JSON_DEPS) -> None:
         self._builds = {}
+        self._by_name = {}
         with open(json_file) as f:
             build_list = json.load(f)
             for elt in build_list:
+                name = False
                 if isinstance(elt, list):
                     # get rid of optionnal name
                     descr = elt[1]
+                    name = elt[0]
                 else:
                     descr = elt
                 brick = Brick(**descr)
                 self._builds[brick.dest] = brick
+                if name is not False:
+                    self._by_name = brick
             self.checker = DAG(self._builds.values())
             # Warning in case of redondant concatenation
             self.checker.check()
             # raise exception in case of cycle(s)
             self.checker.get_order()
             self.build_change_deps()
 
@@ -234,14 +239,25 @@
         self._write_bundle(build, out)
         if self.create_sourcemaps:
             map_out = str(out) + ".map"
             smap = self.mapper.sourcemap(build)
             self.printer("Writing source map.") 
             with open(map_out, "w") as map_file:
                 json.dump(smap, map_file)
+    
+    def build_by_name(self, name: str) -> bool:
+        """
+        Build one Bundle, gicen by it's optionnal name.
+        Returns a boolean indicating if given name was found
+        and bundle has been built.
+        """
+        if name in self._by_name:
+            self._bundle_one(self._by_name[name])
+            return True
+        return False
 
     def bundle(self, changed_file: Union[Path, str]) -> None:
         # we must invalidate previous line count
         self.mapper.changed(changed_file)
         builds = self.get_rebuilds(changed_file)
         for b in builds:
             self._bundle_one(b)
```

### Comparing `django_concat_js-0.2.1/concat_js/settings.py` & `django_concat_js-0.3.0/concat_js/settings.py`

 * *Files identical despite different names*

### Comparing `django_concat_js-0.2.1/concat_js/watch_src.py` & `django_concat_js-0.3.0/concat_js/watch_src.py`

 * *Files identical despite different names*

### Comparing `django_concat_js-0.2.1/concat_js/management/commands/watch_js.py` & `django_concat_js-0.3.0/concat_js/management/commands/watch_js.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 class Command(BaseCommand):
     help_text="Watch for file changes and concatenate when needed."
 
     def add_arguments(self, parser):
         parser.add_argument(
             "--rebuild",
-            action="store_true",
-            help="Only rebuild all bundle and exit."
+            action='store', nargs="?", default=False, const="True",
+            help="Rebuild all bundle and exit or rebuild one bundle given by its name"
         )
         group = parser.add_mutually_exclusive_group()
         group.add_argument(
             "--maps",
             action="store_true",
             help="Override CRETE_SOURCEMAPS settings for this run."
         )
@@ -32,16 +32,24 @@
             bundler.create_sourcemaps = True
         elif options["no_maps"]:
             bundler.create_sourcemaps = False
         if conf.LINT_BASE:
             self.stdout.write("Linting files in {}.".format(conf.LINT_BASE))
             subprocess.run([bundler.lint_js, conf.LINT_BASE])
         if options["rebuild"]:
-            self.stdout.write("Rebuild all bundles.")
-            bundler.rebuild_all()
+            if options["rebuild"] is True:
+                self.stdout.write("Rebuild all bundles.")
+                bundler.rebuild_all()
+            else:
+                # a name is given, try to rebuild that
+                res = bundler.build_by_name(options["rebuild"])
+                if res:
+                    self.stdout.write("{} rebuilt.".format(options["rebuild"]))
+                else:
+                    self.stdout.write("{} not found.".format(options["rebuild"]))
             return
         self.stdout.write("Watching for file changes.")
         try:
             bundler.check_timestamps()
             watcher = watch_src.JsWatcher()
             watcher.register(bundler)
             watcher.run()
```

### Comparing `django_concat_js-0.2.1/concat_js/test_app/concat.json` & `django_concat_js-0.3.0/concat_js/test_app/concat.json`

 * *Files identical despite different names*

### Comparing `django_concat_js-0.2.1/concat_js/test_app/manage.py` & `django_concat_js-0.3.0/concat_js/test_app/manage.py`

 * *Files identical despite different names*

### Comparing `django_concat_js-0.2.1/concat_js/test_app/settings_base.py` & `django_concat_js-0.3.0/concat_js/test_app/settings_base.py`

 * *Files identical despite different names*

### Comparing `django_concat_js-0.2.1/concat_js/test_app/tests.py` & `django_concat_js-0.3.0/concat_js/test_app/tests.py`

 * *Files identical despite different names*

### Comparing `django_concat_js-0.2.1/concat_js/test_app/urls.py` & `django_concat_js-0.3.0/concat_js/test_app/urls.py`

 * *Files identical despite different names*

### Comparing `django_concat_js-0.2.1/LICENSE.txt` & `django_concat_js-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_concat_js-0.2.1/README.md` & `django_concat_js-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `django_concat_js-0.2.1/pyproject.toml` & `django_concat_js-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_concat_js-0.2.1/PKG-INFO` & `django_concat_js-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-concat-js
-Version: 0.2.1
+Version: 0.3.0
 Summary: Simple tool to concatenate js files when changed.
 Project-URL: Documentation, https://github.com/unknown/concat-js#readme
 Project-URL: Issues, https://github.com/unknown/concat-js/issues
 Project-URL: Source, https://github.com/unknown/concat-js
 Author-email: Antoine Louatron <antoine.louatron@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

